# Comparing `tmp/video2gif-1.1.0.tar.gz` & `tmp/video2gif-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video2gif-1.1.0.tar", max compression
+gzip compressed data, was "video2gif-1.1.1.tar", max compression
```

## Comparing `video2gif-1.1.0.tar` & `video2gif-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34523 2023-07-16 14:37:00.569535 video2gif-1.1.0/LICENSE
--rw-r--r--   0        0        0      248 2023-07-16 14:37:00.569535 video2gif-1.1.0/README.md
--rw-r--r--   0        0        0      615 2023-07-18 21:38:13.413635 video2gif-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 14:37:00.570535 video2gif-1.1.0/video2gif/__init__.py
--rw-r--r--   0        0        0     2352 2023-07-18 21:38:13.428635 video2gif-1.1.0/video2gif/main.py
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 video2gif-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-16 14:37:00.569535 video2gif-1.1.1/LICENSE
+-rw-r--r--   0        0        0      248 2023-07-16 14:37:00.569535 video2gif-1.1.1/README.md
+-rw-r--r--   0        0        0      615 2023-07-19 00:33:21.163485 video2gif-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 14:37:00.570535 video2gif-1.1.1/video2gif/__init__.py
+-rw-r--r--   0        0        0     2493 2023-07-19 00:32:45.644439 video2gif-1.1.1/video2gif/main.py
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 video2gif-1.1.1/PKG-INFO
```

### Comparing `video2gif-1.1.0/LICENSE` & `video2gif-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `video2gif-1.1.0/pyproject.toml` & `video2gif-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "video2gif"
-version = "1.1.0"
+version = "1.1.1"
 description = "a simple program that converts a video to gif. it will also download a video for you using yt-dlp. Depends on ffmpeg"
 authors = ["Mae Miller <maeborow@posteo.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 yt-dlp = "^2023.7.6"
```

### Comparing `video2gif-1.1.0/video2gif/main.py` & `video2gif-1.1.1/video2gif/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 import argparse
 import datetime
 import ffmpeg
 import os
 import validators
 import yt_dlp
+import uuid
 
 parser = argparse.ArgumentParser()
 parser.add_argument("video", help="url or path of the video you'd like to gif-ify")
 parser.add_argument("start", type=lambda d: datetime.datetime.strptime(d, '%M:%S'), help="start time in minutes:seconds")
 parser.add_argument("end", type=lambda d: datetime.datetime.strptime(d, '%M:%S'), help="end time in minutes:seconds")
 parser.add_argument("--output", required=False, help="output file")
 args = parser.parse_args()
 
 start_sec = int(datetime.timedelta(minutes=args.start.minute, seconds=args.start.second).total_seconds())
 end_sec = int(datetime.timedelta(minutes=args.end.minute, seconds=args.end.second).total_seconds())
 
+projectRand = str(uuid.uuid4())
 if args.output:
     outputFile = args.output
 else:
-    outputFile = "result/output.gif"
+    outputFile = f"{projectRand}.gif"
+
 
 if validators.url(args.video):
     URLS = [args.video]
-    if os.path.exists("result/inter.mp4"):
-        os.remove("result/inter.mp4")
-    ydl_opts = {'final_ext': 'mkv',
+    if os.path.exists(f"result/{projectRand}.mp4"):
+        os.remove(f"result/{projectRand}.mp4")
+    ydl_opts = {'final_ext': 'mp4',
                 'download_ranges': yt_dlp.utils.download_range_func([], [[start_sec, end_sec]]),
                 'format': 'bv*[ext=mp4]+ba[ext=vorbis]/b[ext=mp4] / bv*+ba/b',
-                'outtmpl': {'default': 'result/inter.mp4'}}
+                'outtmpl': {'default': f'result/{projectRand}.mp4'}}
 
     with yt_dlp.YoutubeDL(ydl_opts) as ydl:
         ydl.download(URLS)
-    stream = ffmpeg.input('result/inter.mp4')
+    stream = ffmpeg.input(f'result/{projectRand}.mp4')
 else:
     stream = ffmpeg.input(args.video)
 
-stream = ffmpeg.filter(stream, 'scale', height=300, width=-2).output('result/inter-scale.mp4').run(overwrite_output=True)
-stream = ffmpeg.input('result/inter-scale.mp4').filter('palettegen', stats_mode='full').output('result/palettegen_full.png')
+stream = ffmpeg.filter(stream, 'scale', height=300, width=-2).output(f'result/{projectRand}-scale.mp4').run(overwrite_output=True)
+stream = ffmpeg.input(f'result/{projectRand}-scale.mp4').filter('palettegen', stats_mode='full').output(f'result/{projectRand}.png')
 stream = ffmpeg.run(stream, overwrite_output=True)
 stream = ffmpeg.filter(
          [
-            ffmpeg.input('result/inter-scale.mp4'),
-            ffmpeg.input('result/palettegen_full.png'),
+            ffmpeg.input(f'result/{projectRand}-scale.mp4'),
+            ffmpeg.input(f'result/{projectRand}.png'),
 
          ],
          filter_name='paletteuse',
          dither='heckbert',
          new='False',
          )
 stream = ffmpeg.output(stream, outputFile, framerate=30)
 
 
 def run() -> None:
     stream.run(overwrite_output=True)
-    if os.path.exists("result/inter.mp4"):
-        os.remove("result/inter.mp4")
-    if os.path.exists("result/inter-scale.mp4"):
-        os.remove("result/inter-scale.mp4")
-    if os.path.exists("result/palettegen_full.png"):
-        os.remove("result/palettegen_full.png")
+    if os.path.exists(f"result/{projectRand}.mp4"):
+        os.remove(f"result/{projectRand}.mp4")
+    if os.path.exists(f"result/{projectRand}-scale.mp4"):
+        os.remove(f"result/{projectRand}-scale.mp4")
+    if os.path.exists(f"result/{projectRand}.png"):
+        os.remove(f"result/{projectRand}.png")
```

### Comparing `video2gif-1.1.0/PKG-INFO` & `video2gif-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video2gif
-Version: 1.1.0
+Version: 1.1.1
 Summary: a simple program that converts a video to gif. it will also download a video for you using yt-dlp. Depends on ffmpeg
 Author: Mae Miller
 Author-email: maeborow@posteo.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
```

