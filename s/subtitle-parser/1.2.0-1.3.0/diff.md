# Comparing `tmp/subtitle-parser-1.2.0.tar.gz` & `tmp/subtitle_parser-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtitle-parser-1.2.0.tar", max compression
+gzip compressed data, was "subtitle_parser-1.3.0.tar", max compression
```

## Comparing `subtitle-parser-1.2.0.tar` & `subtitle_parser-1.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      928 2022-01-28 19:47:27.291742 subtitle-parser-1.2.0/README.md
--rw-r--r--   0        0        0      838 2023-01-11 15:32:42.562754 subtitle-parser-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    12556 2023-01-11 15:32:49.370780 subtitle-parser-1.2.0/subtitle_parser.py
--rw-r--r--   0        0        0     6383 2023-01-11 15:26:54.461404 subtitle-parser-1.2.0/tests.py
--rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 subtitle-parser-1.2.0/setup.py
--rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 subtitle-parser-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      756 2023-07-18 23:55:36.581555 subtitle_parser-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1068 2023-05-08 21:06:25.687596 subtitle_parser-1.3.0/LICENSE
+-rw-r--r--   0        0        0      928 2022-01-28 19:47:27.291742 subtitle_parser-1.3.0/README.md
+-rw-r--r--   0        0        0      854 2023-07-18 23:57:11.255162 subtitle_parser-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13630 2023-07-18 23:57:13.835204 subtitle_parser-1.3.0/subtitle_parser.py
+-rw-r--r--   0        0        0     9368 2023-07-18 23:53:55.307689 subtitle_parser-1.3.0/tests.py
+-rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 subtitle_parser-1.3.0/PKG-INFO
```

### Comparing `subtitle-parser-1.2.0/README.md` & `subtitle_parser-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `subtitle-parser-1.2.0/pyproject.toml` & `subtitle_parser-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subtitle-parser"
-version = "1.2.0"
+version = "1.3.0"
 description = "Parser for SRT and WebVTT subtitle files"
 
 license = "MIT"
 
 authors = [
     "Remi Rampin <remi@rampin.org>",
 ]
@@ -19,15 +19,15 @@
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Topic :: Text Processing",
     "Topic :: Utilities",
 ]
 
 include = [
-    "tests.py",
+    "tests.py", "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/remram44/subtitle-parser/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4"
```

### Comparing `subtitle-parser-1.2.0/subtitle_parser.py` & `subtitle_parser-1.3.0/subtitle_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os.path
 import re
 import sys
 import traceback
 
 
-__version__ = '1.2.0'
+__version__ = '1.3.0'
 
 
 __all__ = [
     'SubtitleError', 'Subtitle',
     'SrtParser', 'WebVttParser',
     'render_html', 'render_csv',
 ]
@@ -21,38 +21,40 @@
 
 
 def format_timestamp(ts):
     return '{0:02}:{1:02}:{2:02}.{3:03}'.format(*ts)
 
 
 class Subtitle(object):
-    def __init__(self, number, start, end, text):
+    def __init__(self, number, start, end, text, *, name=None):
         self.number = number
+        self.name = name
         self.start = start
         self.end = end
         self.text = text
 
     def __eq__(self, other):
         return (
-            self.number, self.start, self.end, self.text,
+            self.number, self.name, self.start, self.end, self.text,
         ) == (
-            other.number, other.start, other.end, other.text,
+            other.number, other.name, other.start, other.end, other.text,
         )
 
     def __hash__(self):
         return hash((
-            self.number, self.start, self.end, self.text,
+            self.number, self.name, self.start, self.end, self.text,
         ))
 
     def __repr__(self):
         return (
-            '<Subtitle number={number} '
+            '<Subtitle number={number} name={name} '
             + 'start={start} end={end} text={text}>'
         ).format(
             number=self.number,
+            name=self.name,
             start=format_timestamp(self.start),
             end=format_timestamp(self.end),
             text=self.text,
         )
 
 
 class SrtParser(object):
@@ -97,16 +99,21 @@
         # Read subtitles
         while self.parse_subtitle():
             pass
 
     def parse_subtitle(self):
         # Read subtitle number
         line = self.next_line()
+        name = None
         if line is None:
             return False
+        line_with_name = re.match(r'(\d+) "(.+)"', line)
+        if line_with_name is not None:
+            line = line_with_name.group(1)
+            name = line_with_name.group(2)
         if '-->' not in line:
             self.read_line()
             try:
                 subtitle_number = int(line)
             except (ValueError, OverflowError):
                 raise SubtitleError(
                     "Invalid subtitle number line {lineno}".format(
@@ -159,14 +166,15 @@
                     lineno=first_line_lineno,
                 ),
             )
 
         self.subtitles.append(Subtitle(
             subtitle_number, start, end,
             '\n'.join(lines),
+            name=name,
         ))
 
         self.skip_blank_lines()
 
         return True
 
     def skip_blank_lines(self):
@@ -291,46 +299,69 @@
         line = self.next_line()
         while line:
             self.read_line()
             line = self.next_line()
         self.skip_blank_lines()
 
 
-def render_html(subtitles, file_out):
+def render_html(subtitles, file_out, *, show_name=None):
     import html
 
     for subtitle in subtitles:
+        name = ''
+        if show_name is not False and subtitle.name:
+            name = ' ' + html.escape(subtitle.name)
         print(
-            "<p>{ts} {text}</p>".format(
+            "<p>{ts}{name} {text}</p>".format(
                 ts=format_timestamp(subtitle.start),
+                name=name,
                 text=html.escape(subtitle.text).replace('\n', '<br>'),
             ),
             file=file_out,
         )
 
 
-def render_csv(subtitles, file_out):
+def render_csv(subtitles, file_out, *, show_name=None):
     import csv
 
     writer = csv.writer(file_out)
-    writer.writerow(['start', 'end', 'text'])
+    writer.writerow(
+        ['start', 'end']
+        + (['name'] if show_name else [])
+        + ['text']
+    )
     for subtitle in subtitles:
-        writer.writerow([
-            format_timestamp(subtitle.start),
-            format_timestamp(subtitle.end),
-            subtitle.text,
-        ])
+        writer.writerow(
+            [
+                format_timestamp(subtitle.start),
+                format_timestamp(subtitle.end),
+            ]
+            + ([subtitle.name] if show_name else [])
+            + [
+                subtitle.text,
+            ]
+        )
 
 
 def main():
     arg_parser = argparse.ArgumentParser()
     arg_parser.add_argument('--to', help="Output format")
     arg_parser.add_argument('--input-charset', default=None)
     arg_parser.add_argument('input', help="Input subtitles")
     arg_parser.add_argument('--output', '-o', help="Output file name")
+    arg_parser.add_argument(
+        '--with-name',
+        default=None, action='store_true', dest='show_name',
+        help="Show the speaker's name",
+    )
+    arg_parser.add_argument(
+        '--without-name',
+        default=None, action='store_false', dest='show_name',
+        help="Don't show the speaker's name",
+    )
 
     args = arg_parser.parse_args()
 
     # Pick format
     if not args.to:
         arg_parser.error("No output format specified (use --to)")
         return
@@ -431,13 +462,13 @@
                 lineno=lineno,
                 text=text,
             ),
             file=sys.stderr,
         )
 
     # Write output
-    render_func(parser.subtitles, file_output)
+    render_func(parser.subtitles, file_output, show_name=args.show_name)
     file_output.close()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `subtitle-parser-1.2.0/PKG-INFO` & `subtitle_parser-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: subtitle-parser
-Version: 1.2.0
+Version: 1.3.0
 Summary: Parser for SRT and WebVTT subtitle files
 Home-page: https://github.com/remram44/subtitle-parser
 License: MIT
 Keywords: subtitle,srt,webvtt,video,text track,subrip
 Author: Remi Rampin
 Author-email: remi@rampin.org
 Requires-Python: >=3.7,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Dist: chardet (>=4,<6)
 Project-URL: Bug Tracker, https://github.com/remram44/subtitle-parser/issues
 Project-URL: Repository, https://github.com/remram44/subtitle-parser
 Description-Content-Type: text/markdown
```

