# Comparing `tmp/wagtail-katex-0.0.5.tar.gz` & `tmp/wagtail-katex-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-katex-0.0.5.tar", last modified: Thu Jun 15 13:37:30 2023, max compression
+gzip compressed data, was "wagtail-katex-0.0.6.tar", last modified: Wed Jul 19 11:21:41 2023, max compression
```

## Comparing `wagtail-katex-0.0.5.tar` & `wagtail-katex-0.0.6.tar`

### file list

```diff
@@ -1,90 +1,92 @@
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.901672 wagtail-katex-0.0.5/
--rw-r--r--   0 chii       (501) staff       (20)    11357 2022-03-05 02:43:30.000000 wagtail-katex-0.0.5/LICENSE
--rw-r--r--   0 chii       (501) staff       (20)      100 2023-06-14 14:55:14.000000 wagtail-katex-0.0.5/MANIFEST.in
--rw-r--r--   0 chii       (501) staff       (20)     1810 2023-06-15 13:37:30.901507 wagtail-katex-0.0.5/PKG-INFO
--rw-r--r--   0 chii       (501) staff       (20)      717 2023-06-15 13:35:13.000000 wagtail-katex-0.0.5/README.md
--rw-r--r--   0 chii       (501) staff       (20)       38 2023-06-15 13:37:30.901725 wagtail-katex-0.0.5/setup.cfg
--rw-r--r--   0 chii       (501) staff       (20)     1436 2023-06-14 14:44:59.000000 wagtail-katex-0.0.5/setup.py
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.887086 wagtail-katex-0.0.5/wagtail_katex.egg-info/
--rw-r--r--   0 chii       (501) staff       (20)     1810 2023-06-15 13:37:30.000000 wagtail-katex-0.0.5/wagtail_katex.egg-info/PKG-INFO
--rw-r--r--   0 chii       (501) staff       (20)     4897 2023-06-15 13:37:30.000000 wagtail-katex-0.0.5/wagtail_katex.egg-info/SOURCES.txt
--rw-r--r--   0 chii       (501) staff       (20)        1 2023-06-15 13:37:30.000000 wagtail-katex-0.0.5/wagtail_katex.egg-info/dependency_links.txt
--rw-r--r--   0 chii       (501) staff       (20)       11 2023-06-15 13:37:30.000000 wagtail-katex-0.0.5/wagtail_katex.egg-info/requires.txt
--rw-r--r--   0 chii       (501) staff       (20)       13 2023-06-15 13:37:30.000000 wagtail-katex-0.0.5/wagtail_katex.egg-info/top_level.txt
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.887632 wagtail-katex-0.0.5/wagtailkatex/
--rw-r--r--   0 chii       (501) staff       (20)       22 2023-06-15 13:31:02.000000 wagtail-katex-0.0.5/wagtailkatex/__init__.py
--rwxr-xr-x   0 chii       (501) staff       (20)      860 2023-06-15 12:07:36.000000 wagtail-katex-0.0.5/wagtailkatex/richtext.py
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.887817 wagtail-katex-0.0.5/wagtailkatex/static/
--rw-r--r--   0 chii       (501) staff       (20)     6148 2021-03-04 07:31:57.000000 wagtail-katex-0.0.5/wagtailkatex/static/.DS_Store
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.888182 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.888808 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/
--rw-r--r--   0 chii       (501) staff       (20)     7119 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/README.md
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.901032 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/
--rw-r--r--   0 chii       (501) staff       (20)    63632 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    33516 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    28076 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    12368 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)     7716 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)     6912 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    12344 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     7656 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     6908 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    19584 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)    13296 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)    11348 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    19572 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    13208 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    11316 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    51336 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)    29912 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)    25324 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    32968 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    19412 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16780 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    33580 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    19676 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16988 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    53580 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    30772 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    26272 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    31196 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    18668 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16400 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    31308 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    18748 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16440 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    24504 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)    14408 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)    12216 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    22364 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    14112 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 chii       (501) staff       (20)    12028 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    19436 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    12316 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    10344 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    16648 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    10588 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     9644 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    12228 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     6496 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     5468 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    11508 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     6188 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     5208 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)     7588 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     4420 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     3624 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    10364 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     5980 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     4928 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    27556 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    16028 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    13568 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    23112 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/katex.min.css
--rw-r--r--   0 chii       (501) staff       (20)   270375 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/katex.min.js
--rw-r--r--   0 chii       (501) staff       (20)      736 2023-06-15 13:12:39.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/wagtailkatex.css
--rwxr-xr-x   0 chii       (501) staff       (20)     5380 2023-06-15 12:07:10.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/wagtailkatex.js
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.885483 wagtail-katex-0.0.5/wagtailkatex/templates/
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.901237 wagtail-katex-0.0.5/wagtailkatex/templates/wagtailkatex/
--rw-r--r--   0 chii       (501) staff       (20)      875 2023-06-14 14:42:43.000000 wagtail-katex-0.0.5/wagtailkatex/templates/wagtailkatex/square-root-variable.svg
--rwxr-xr-x   0 chii       (501) staff       (20)     1700 2023-06-15 13:27:25.000000 wagtail-katex-0.0.5/wagtailkatex/wagtail_hooks.py
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-07-19 11:21:41.006165 wagtail-katex-0.0.6/
+-rw-r--r--   0 chii       (501) staff       (20)    11357 2022-03-05 02:43:30.000000 wagtail-katex-0.0.6/LICENSE
+-rw-r--r--   0 chii       (501) staff       (20)      100 2023-06-26 13:33:02.000000 wagtail-katex-0.0.6/MANIFEST.in
+-rw-r--r--   0 chii       (501) staff       (20)     2314 2023-07-19 11:21:41.005972 wagtail-katex-0.0.6/PKG-INFO
+-rw-r--r--   0 chii       (501) staff       (20)     1190 2023-07-02 11:46:52.000000 wagtail-katex-0.0.6/README.md
+-rw-r--r--   0 chii       (501) staff       (20)     1349 2023-07-02 11:46:52.000000 wagtail-katex-0.0.6/pyproject.toml
+-rw-r--r--   0 chii       (501) staff       (20)       38 2023-07-19 11:21:41.006236 wagtail-katex-0.0.6/setup.cfg
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-07-19 11:21:40.983648 wagtail-katex-0.0.6/tests/
+-rw-r--r--   0 chii       (501) staff       (20)     1072 2023-07-02 11:46:52.000000 wagtail-katex-0.0.6/tests/tests.py
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-07-19 11:21:40.984614 wagtail-katex-0.0.6/wagtail_katex.egg-info/
+-rw-r--r--   0 chii       (501) staff       (20)     2314 2023-07-19 11:21:40.000000 wagtail-katex-0.0.6/wagtail_katex.egg-info/PKG-INFO
+-rw-r--r--   0 chii       (501) staff       (20)     4918 2023-07-19 11:21:40.000000 wagtail-katex-0.0.6/wagtail_katex.egg-info/SOURCES.txt
+-rw-r--r--   0 chii       (501) staff       (20)        1 2023-07-19 11:21:40.000000 wagtail-katex-0.0.6/wagtail_katex.egg-info/dependency_links.txt
+-rw-r--r--   0 chii       (501) staff       (20)       11 2023-07-19 11:21:40.000000 wagtail-katex-0.0.6/wagtail_katex.egg-info/requires.txt
+-rw-r--r--   0 chii       (501) staff       (20)       13 2023-07-19 11:21:40.000000 wagtail-katex-0.0.6/wagtail_katex.egg-info/top_level.txt
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-07-19 11:21:40.985201 wagtail-katex-0.0.6/wagtailkatex/
+-rw-r--r--   0 chii       (501) staff       (20)       22 2023-07-19 11:18:30.000000 wagtail-katex-0.0.6/wagtailkatex/__init__.py
+-rwxr-xr-x   0 chii       (501) staff       (20)      860 2023-07-19 02:39:32.000000 wagtail-katex-0.0.6/wagtailkatex/richtext.py
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-07-19 11:21:40.985385 wagtail-katex-0.0.6/wagtailkatex/static/
+-rw-r--r--   0 chii       (501) staff       (20)     6148 2021-03-04 07:31:57.000000 wagtail-katex-0.0.6/wagtailkatex/static/.DS_Store
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-07-19 11:21:40.986099 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-07-19 11:21:40.986932 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/
+-rw-r--r--   0 chii       (501) staff       (20)     7119 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/README.md
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-07-19 11:21:41.005452 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/
+-rw-r--r--   0 chii       (501) staff       (20)    63632 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    33516 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    28076 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    12368 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     7716 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)     6912 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    12344 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     7656 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     6908 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    19584 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    13296 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)    11348 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    19572 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    13208 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    11316 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    51336 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    29912 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)    25324 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    32968 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    19412 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16780 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    33580 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    19676 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16988 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    53580 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    30772 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    26272 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    31196 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    18668 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16400 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    31308 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    18748 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16440 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    24504 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    14408 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)    12216 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    22364 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    14112 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    12028 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    19436 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    12316 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    10344 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    16648 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    10588 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     9644 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    12228 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     6496 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     5468 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    11508 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     6188 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     5208 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)     7588 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     4420 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     3624 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    10364 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     5980 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     4928 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    27556 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    16028 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    13568 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    23112 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/katex.min.css
+-rw-r--r--   0 chii       (501) staff       (20)   270375 2023-06-26 13:02:32.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/katex.min.js
+-rw-r--r--   0 chii       (501) staff       (20)      724 2023-07-19 11:14:50.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/wagtailkatex.css
+-rwxr-xr-x   0 chii       (501) staff       (20)     5686 2023-07-19 11:14:50.000000 wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/wagtailkatex.js
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-07-19 11:21:40.982525 wagtail-katex-0.0.6/wagtailkatex/templates/
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-07-19 11:21:41.005672 wagtail-katex-0.0.6/wagtailkatex/templates/wagtailkatex/
+-rw-r--r--   0 chii       (501) staff       (20)      875 2023-06-26 13:33:02.000000 wagtail-katex-0.0.6/wagtailkatex/templates/wagtailkatex/square-root-variable.svg
+-rwxr-xr-x   0 chii       (501) staff       (20)     1700 2023-07-19 02:39:32.000000 wagtail-katex-0.0.6/wagtailkatex/wagtail_hooks.py
```

### Comparing `wagtail-katex-0.0.5/LICENSE` & `wagtail-katex-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/PKG-INFO` & `wagtail-katex-0.0.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 Metadata-Version: 2.1
 Name: wagtail-katex
-Version: 0.0.5
-Summary: KaTex for Wagtail CMS Draftail editor
-Home-page: https://github.com/ongchi/wagtail-katex
-Author: ongchi
-Author-email: ongchi@users.noreply.github.com
+Version: 0.0.6
+Summary: Math typesetting for Wagtail CMS powered by KaTeX
+Author-email: ongchi <ongchi@users.noreply.github.com>
+License: MIT
+Project-URL: Homepage, https://github.com/ongchi/wagtail-katex
 Project-URL: Bug Tracker, https://github.com/ongchi/wagtail-katex/issues
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Django
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 3
-Classifier: Framework :: Wagtail :: 4
-Classifier: Framework :: Wagtail :: 5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# wagtail-katex ![Wagtail 3.x](https://img.shields.io/badge/wagtail-3.x-g.svg) ![Wagtail 4.x](https://img.shields.io/badge/wagtail-4.x-g.svg) ![Wagtail 5.x](https://img.shields.io/badge/wagtail-5.x-g.svg)
+![PyPI Package Version](https://img.shields.io/pypi/v/wagtail-katex)
+![Python Version](https://img.shields.io/pypi/pyversions/wagtail-cjkcms)
+![Wagtail Version](https://img.shields.io/pypi/frameworkversions/wagtail/wagtail-katex)
+![License](https://img.shields.io/github/license/ongchi/wagtail-katex)
 
-> This package is modified from [gatensj/wagtail-draftail-katex](https://github.com/gatensj/wagtail-draftail-katex)
+Math typesetting for [Wagtail CMS](https://wagtail.org/) powered by **[KaTeX](https://katex.org)**.
 
-**[KaTeX](https://katex.org)** support for Wagtail RichTextField.
+> This package is forked from [gatensj/wagtail-draftail-katex](https://github.com/gatensj/wagtail-draftail-katex).  
+> This package contains svg icon from [Font Awesome](http://fontawesome.io), which is licensed under the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0).
 
-![KaTeX Editor](https://raw.githubusercontent.com/ongchi/wagtail-katex/master/images/screenshot.png)
+![KaTeX Editor Screenshot](https://raw.githubusercontent.com/ongchi/wagtail-katex/master/screenshots/screenshot_katex_editor.png)
 
 ## Quick Start
 
-Install the package with
+Install the package using the following command:
 
 ```sh
 pip install wagtail-katex
 ```
 
-Add `wagtailkatex` to your `settings.py` in the `INSTALLED_APPS` section:
+Add `wagtailkatex` to the `INSTALLED_APPS` section in your `settings.py` file:
 
 ```python
 INSTALLED_APPS = [
     ...
     "wagtailkatex",
     ...
 ]
 ```
+
+Now you will see the math typesetting icon displayed in the toolbar of
+rich text fields in Wagtail admin views.
```

### Comparing `wagtail-katex-0.0.5/README.md` & `wagtail-katex-0.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-# wagtail-katex ![Wagtail 3.x](https://img.shields.io/badge/wagtail-3.x-g.svg) ![Wagtail 4.x](https://img.shields.io/badge/wagtail-4.x-g.svg) ![Wagtail 5.x](https://img.shields.io/badge/wagtail-5.x-g.svg)
+![PyPI Package Version](https://img.shields.io/pypi/v/wagtail-katex)
+![Python Version](https://img.shields.io/pypi/pyversions/wagtail-cjkcms)
+![Wagtail Version](https://img.shields.io/pypi/frameworkversions/wagtail/wagtail-katex)
+![License](https://img.shields.io/github/license/ongchi/wagtail-katex)
 
-> This package is modified from [gatensj/wagtail-draftail-katex](https://github.com/gatensj/wagtail-draftail-katex)
+Math typesetting for [Wagtail CMS](https://wagtail.org/) powered by **[KaTeX](https://katex.org)**.
 
-**[KaTeX](https://katex.org)** support for Wagtail RichTextField.
+> This package is forked from [gatensj/wagtail-draftail-katex](https://github.com/gatensj/wagtail-draftail-katex).  
+> This package contains svg icon from [Font Awesome](http://fontawesome.io), which is licensed under the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0).
 
-![KaTeX Editor](https://raw.githubusercontent.com/ongchi/wagtail-katex/master/images/screenshot.png)
+![KaTeX Editor Screenshot](https://raw.githubusercontent.com/ongchi/wagtail-katex/master/screenshots/screenshot_katex_editor.png)
 
 ## Quick Start
 
-Install the package with
+Install the package using the following command:
 
 ```sh
 pip install wagtail-katex
 ```
 
-Add `wagtailkatex` to your `settings.py` in the `INSTALLED_APPS` section:
+Add `wagtailkatex` to the `INSTALLED_APPS` section in your `settings.py` file:
 
 ```python
 INSTALLED_APPS = [
     ...
     "wagtailkatex",
     ...
 ]
 ```
+
+Now you will see the math typesetting icon displayed in the toolbar of
+rich text fields in Wagtail admin views.
```

### Comparing `wagtail-katex-0.0.5/setup.py` & `wagtail-katex-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-from setuptools import setup, find_packages
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 
-from wagtailkatex import __version__
+[project]
+name = "wagtail-katex"
+description = "Math typesetting for Wagtail CMS powered by KaTeX"
+authors = [
+    {name = "ongchi", email = "ongchi@users.noreply.github.com"},
+]
+dependencies = [
+    "wagtail>=3",
+]
+requires-python = ">=3.6"
+license = {text = "MIT"}
+readme = "README.md"
+classifiers = [
+    "Environment :: Web Environment",
+    "Framework :: Django",
+    "Framework :: Wagtail",
+    "Framework :: Wagtail :: 3",
+    "Framework :: Wagtail :: 4",
+    "Framework :: Wagtail :: 5",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+]
+dynamic = ["version"]
 
-with open("README.md", "r") as fp:
-    long_description = fp.read()
+[project.urls]
+Homepage = "https://github.com/ongchi/wagtail-katex"
+"Bug Tracker" = "https://github.com/ongchi/wagtail-katex/issues"
 
-setup(
-    name='wagtail-katex',
-    version=__version__,
-    author="ongchi",
-    author_email="ongchi@users.noreply.github.com",
-    description='KaTex for Wagtail CMS Draftail editor',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url='https://github.com/ongchi/wagtail-katex',
-    project_urls={
-        "Bug Tracker": "https://github.com/ongchi/wagtail-katex/issues",
-    },
-    install_requires=['wagtail>=3'],
-    classifiers=[
-        'Environment :: Web Environment',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        "Operating System :: OS Independent",
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Framework :: Django',
-        'Framework :: Wagtail',
-        'Framework :: Wagtail :: 3',
-        'Framework :: Wagtail :: 4',
-        'Framework :: Wagtail :: 5',
-    ],
-    packages=find_packages(),
-    include_package_data=True,
-    python_requires=">=3.6",
-)
+[tool.setuptools]
+packages = ["wagtailkatex"]
+
+[tool.setuptools.dynamic]
+version = {attr = "wagtailkatex.__version__"}
+
+[tool.black]
+skip_string_normalization = true
```

### Comparing `wagtail-katex-0.0.5/wagtail_katex.egg-info/PKG-INFO` & `wagtail-katex-0.0.6/wagtail_katex.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 Metadata-Version: 2.1
 Name: wagtail-katex
-Version: 0.0.5
-Summary: KaTex for Wagtail CMS Draftail editor
-Home-page: https://github.com/ongchi/wagtail-katex
-Author: ongchi
-Author-email: ongchi@users.noreply.github.com
+Version: 0.0.6
+Summary: Math typesetting for Wagtail CMS powered by KaTeX
+Author-email: ongchi <ongchi@users.noreply.github.com>
+License: MIT
+Project-URL: Homepage, https://github.com/ongchi/wagtail-katex
 Project-URL: Bug Tracker, https://github.com/ongchi/wagtail-katex/issues
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Django
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 3
-Classifier: Framework :: Wagtail :: 4
-Classifier: Framework :: Wagtail :: 5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# wagtail-katex ![Wagtail 3.x](https://img.shields.io/badge/wagtail-3.x-g.svg) ![Wagtail 4.x](https://img.shields.io/badge/wagtail-4.x-g.svg) ![Wagtail 5.x](https://img.shields.io/badge/wagtail-5.x-g.svg)
+![PyPI Package Version](https://img.shields.io/pypi/v/wagtail-katex)
+![Python Version](https://img.shields.io/pypi/pyversions/wagtail-cjkcms)
+![Wagtail Version](https://img.shields.io/pypi/frameworkversions/wagtail/wagtail-katex)
+![License](https://img.shields.io/github/license/ongchi/wagtail-katex)
 
-> This package is modified from [gatensj/wagtail-draftail-katex](https://github.com/gatensj/wagtail-draftail-katex)
+Math typesetting for [Wagtail CMS](https://wagtail.org/) powered by **[KaTeX](https://katex.org)**.
 
-**[KaTeX](https://katex.org)** support for Wagtail RichTextField.
+> This package is forked from [gatensj/wagtail-draftail-katex](https://github.com/gatensj/wagtail-draftail-katex).  
+> This package contains svg icon from [Font Awesome](http://fontawesome.io), which is licensed under the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0).
 
-![KaTeX Editor](https://raw.githubusercontent.com/ongchi/wagtail-katex/master/images/screenshot.png)
+![KaTeX Editor Screenshot](https://raw.githubusercontent.com/ongchi/wagtail-katex/master/screenshots/screenshot_katex_editor.png)
 
 ## Quick Start
 
-Install the package with
+Install the package using the following command:
 
 ```sh
 pip install wagtail-katex
 ```
 
-Add `wagtailkatex` to your `settings.py` in the `INSTALLED_APPS` section:
+Add `wagtailkatex` to the `INSTALLED_APPS` section in your `settings.py` file:
 
 ```python
 INSTALLED_APPS = [
     ...
     "wagtailkatex",
     ...
 ]
 ```
+
+Now you will see the math typesetting icon displayed in the toolbar of
+rich text fields in Wagtail admin views.
```

### Comparing `wagtail-katex-0.0.5/wagtail_katex.egg-info/SOURCES.txt` & `wagtail-katex-0.0.6/wagtail_katex.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+tests/tests.py
 wagtail_katex.egg-info/PKG-INFO
 wagtail_katex.egg-info/SOURCES.txt
 wagtail_katex.egg-info/dependency_links.txt
 wagtail_katex.egg-info/requires.txt
 wagtail_katex.egg-info/top_level.txt
 wagtailkatex/__init__.py
 wagtailkatex/richtext.py
```

### Comparing `wagtail-katex-0.0.5/wagtailkatex/richtext.py` & `wagtail-katex-0.0.6/wagtailkatex/richtext.py`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/.DS_Store` & `wagtail-katex-0.0.6/wagtailkatex/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/README.md` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/katex.min.css` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/katex.min.css`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/katex.min.js` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/wagtailkatex.css` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/wagtailkatex.css`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #wagtailkatex-modal {
   display: block;
-  position: absolute;
+  position: fixed;
   z-index: 100;
-  left: 0;
+  left: inherit;
   top: 0;
-  width: 100%;
   height: 100%;
   overflow: auto;
   background-color: rgb(0, 0, 0);
   background-color: rgba(0, 0, 0, 0.4);
   display: flex;
   justify-content: center;
   align-items: center;
```

### Comparing `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/wagtailkatex.js` & `wagtail-katex-0.0.6/wagtailkatex/static/wagtailkatex/wagtailkatex.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -40,15 +40,18 @@
         contentDiv.appendChild(katexOutputDiv);
         contentDiv.appendChild(actionDiv);
 
         const modal = document.createElement("div");
         modal.id = "wagtailkatex-modal";
         modal.appendChild(contentDiv);
 
-        document.querySelector("main#main").appendChild(modal);
+        const mainContent = document.querySelector("main#main");
+        modal.style.width = `${mainContent.offsetWidth}px`;
+        mainContent.appendChild(modal);
+
         katex.render(inputArea.value, katexOutputDiv, {
             throwOnError: false
         });
 
         // Event handling
         cancelBtn.onclick = () => closeKatexModal();
         confirmBtn.onclick = () => closeKatexModal(onConfirm);
@@ -56,14 +59,21 @@
             katex.render(event.target.value, katexOutputDiv, {
                 throwOnError: false
             });
         });
         window.onclick = (event) => {
             if (event.target == modal) closeKatexModal();
         }
+
+        const resizeObserver = new ResizeObserver((entries) => {
+            entries.map((entry) => {
+                modal.style.width = `${entry.target.offsetWidth}px`;
+            })
+        });
+        resizeObserver.observe(mainContent);
     }
 
     function closeKatexModal(onConfirm) {
         let modal = document.getElementById("wagtailkatex-modal");
 
         if (onConfirm === undefined) {
             // Discard changes and close modal
```

### Comparing `wagtail-katex-0.0.5/wagtailkatex/templates/wagtailkatex/square-root-variable.svg` & `wagtail-katex-0.0.6/wagtailkatex/templates/wagtailkatex/square-root-variable.svg`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.5/wagtailkatex/wagtail_hooks.py` & `wagtail-katex-0.0.6/wagtailkatex/wagtail_hooks.py`

 * *Files identical despite different names*

