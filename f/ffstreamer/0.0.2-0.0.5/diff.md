# Comparing `tmp/ffstreamer-0.0.2-py3-none-any.whl.zip` & `tmp/ffstreamer-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,69 @@
-Zip file size: 8450 bytes, number of entries: 16
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-11 09:27 ffstreamer/__init__.py
--rw-r--r--  2.0 unx      147 b- defN 23-Jul-11 09:27 ffstreamer/__main__.py
--rw-r--r--  2.0 unx     4006 b- defN 23-Jul-11 09:27 ffstreamer/arguments.py
--rw-r--r--  2.0 unx     2134 b- defN 23-Jul-11 09:27 ffstreamer/entrypoint.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 09:27 ffstreamer/apps/__init__.py
--rw-r--r--  2.0 unx      286 b- defN 23-Jul-11 09:27 ffstreamer/assets/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 09:27 ffstreamer/logging/__init__.py
--rw-r--r--  2.0 unx     1099 b- defN 23-Jul-11 09:27 ffstreamer/logging/colored_formatter.py
--rw-r--r--  2.0 unx     6015 b- defN 23-Jul-11 09:27 ffstreamer/logging/logging.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 09:27 ffstreamer/www/__init__.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jul-11 09:28 ffstreamer-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1408 b- defN 23-Jul-11 09:28 ffstreamer-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 09:28 ffstreamer-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Jul-11 09:28 ffstreamer-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-11 09:28 ffstreamer-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1327 b- defN 23-Jul-11 09:28 ffstreamer-0.0.2.dist-info/RECORD
-16 files, 17696 bytes uncompressed, 6236 bytes compressed:  64.8%
+Zip file size: 35382 bytes, number of entries: 67
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-19 15:16 ffstreamer/__init__.py
+-rw-r--r--  2.0 unx      147 b- defN 23-Jul-19 15:16 ffstreamer/__main__.py
+-rw-r--r--  2.0 unx     4408 b- defN 23-Jul-19 15:16 ffstreamer/arguments.py
+-rw-r--r--  2.0 unx     1816 b- defN 23-Jul-19 15:16 ffstreamer/entrypoint.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/aio/__init__.py
+-rw-r--r--  2.0 unx      860 b- defN 23-Jul-19 15:16 ffstreamer/aio/stream.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/apps/__init__.py
+-rw-r--r--  2.0 unx     5760 b- defN 23-Jul-19 15:16 ffstreamer/apps/default.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/argparse/__init__.py
+-rw-r--r--  2.0 unx      286 b- defN 23-Jul-19 15:16 ffstreamer/argparse/argument_utils.py
+-rw-r--r--  2.0 unx     1427 b- defN 23-Jul-19 15:16 ffstreamer/argparse/namespace_utils.py
+-rw-r--r--  2.0 unx     2670 b- defN 23-Jul-19 15:16 ffstreamer/argparse/typing_namespace.py
+-rw-r--r--  2.0 unx      286 b- defN 23-Jul-19 15:16 ffstreamer/assets/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/chrono/__init__.py
+-rw-r--r--  2.0 unx      121 b- defN 23-Jul-19 15:16 ffstreamer/chrono/datetime.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/ffmpeg/__init__.py
+-rw-r--r--  2.0 unx     5268 b- defN 23-Jul-19 15:16 ffstreamer/ffmpeg/ffmpeg.py
+-rw-r--r--  2.0 unx     2362 b- defN 23-Jul-19 15:16 ffstreamer/ffmpeg/ffmpeg_process.py
+-rw-r--r--  2.0 unx     2358 b- defN 23-Jul-19 15:16 ffstreamer/ffmpeg/ffmpeg_receiver.py
+-rw-r--r--  2.0 unx     1161 b- defN 23-Jul-19 15:16 ffstreamer/ffmpeg/ffmpeg_sender.py
+-rw-r--r--  2.0 unx     1022 b- defN 23-Jul-19 15:16 ffstreamer/ffmpeg/ffprobe.py
+-rw-r--r--  2.0 unx     1940 b- defN 23-Jul-19 15:16 ffstreamer/ffmpeg/static_lib.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/inspect/__init__.py
+-rw-r--r--  2.0 unx     1242 b- defN 23-Jul-19 15:16 ffstreamer/inspect/type_origin.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/logging/__init__.py
+-rw-r--r--  2.0 unx     1099 b- defN 23-Jul-19 15:16 ffstreamer/logging/colored_formatter.py
+-rw-r--r--  2.0 unx     6328 b- defN 23-Jul-19 15:16 ffstreamer/logging/logging.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/memory/__init__.py
+-rw-r--r--  2.0 unx     4051 b- defN 23-Jul-19 15:16 ffstreamer/memory/shared_memory_queue.py
+-rw-r--r--  2.0 unx      974 b- defN 23-Jul-19 15:16 ffstreamer/memory/shared_memory_utils.py
+-rw-r--r--  2.0 unx     1325 b- defN 23-Jul-19 15:16 ffstreamer/memory/shared_memory_validator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/module/__init__.py
+-rw-r--r--  2.0 unx     3553 b- defN 23-Jul-19 15:16 ffstreamer/module/errors.py
+-rw-r--r--  2.0 unx     1749 b- defN 23-Jul-19 15:16 ffstreamer/module/module.py
+-rw-r--r--  2.0 unx     1357 b- defN 23-Jul-19 15:16 ffstreamer/module/module_printer.py
+-rw-r--r--  2.0 unx      298 b- defN 23-Jul-19 15:16 ffstreamer/module/variables.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/module/mixin/__init__.py
+-rw-r--r--  2.0 unx     2111 b- defN 23-Jul-19 15:16 ffstreamer/module/mixin/_module_base.py
+-rw-r--r--  2.0 unx     1031 b- defN 23-Jul-19 15:16 ffstreamer/module/mixin/module_doc.py
+-rw-r--r--  2.0 unx      702 b- defN 23-Jul-19 15:16 ffstreamer/module/mixin/module_frame.py
+-rw-r--r--  2.0 unx     1949 b- defN 23-Jul-19 15:16 ffstreamer/module/mixin/module_open.py
+-rw-r--r--  2.0 unx     1071 b- defN 23-Jul-19 15:16 ffstreamer/module/mixin/module_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/network/__init__.py
+-rw-r--r--  2.0 unx      389 b- defN 23-Jul-19 15:16 ffstreamer/network/address_family.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/package/__init__.py
+-rw-r--r--  2.0 unx     1562 b- defN 23-Jul-19 15:16 ffstreamer/package/package_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/parse/__init__.py
+-rw-r--r--  2.0 unx      817 b- defN 23-Jul-19 15:16 ffstreamer/parse/cfg_parse.py
+-rw-r--r--  2.0 unx     2257 b- defN 23-Jul-19 15:16 ffstreamer/parse/env_parse.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/regex/__init__.py
+-rw-r--r--  2.0 unx     1693 b- defN 23-Jul-19 15:16 ffstreamer/regex/access_filter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/system/__init__.py
+-rw-r--r--  2.0 unx      419 b- defN 23-Jul-19 15:16 ffstreamer/system/environ.py
+-rw-r--r--  2.0 unx      915 b- defN 23-Jul-19 15:16 ffstreamer/system/path_context.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/types/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/types/any/__init__.py
+-rw-r--r--  2.0 unx      545 b- defN 23-Jul-19 15:16 ffstreamer/types/any/to_string.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/types/string/__init__.py
+-rw-r--r--  2.0 unx      535 b- defN 23-Jul-19 15:16 ffstreamer/types/string/to_any.py
+-rw-r--r--  2.0 unx      395 b- defN 23-Jul-19 15:16 ffstreamer/types/string/to_boolean.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 15:16 ffstreamer/www/__init__.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jul-19 15:16 ffstreamer-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1445 b- defN 23-Jul-19 15:16 ffstreamer-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 15:16 ffstreamer-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-19 15:16 ffstreamer-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-19 15:16 ffstreamer-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5831 b- defN 23-Jul-19 15:16 ffstreamer-0.0.5.dist-info/RECORD
+67 files, 78809 bytes uncompressed, 25976 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -6,44 +6,197 @@
 
 Filename: ffstreamer/arguments.py
 Comment: 
 
 Filename: ffstreamer/entrypoint.py
 Comment: 
 
+Filename: ffstreamer/aio/__init__.py
+Comment: 
+
+Filename: ffstreamer/aio/stream.py
+Comment: 
+
 Filename: ffstreamer/apps/__init__.py
 Comment: 
 
+Filename: ffstreamer/apps/default.py
+Comment: 
+
+Filename: ffstreamer/argparse/__init__.py
+Comment: 
+
+Filename: ffstreamer/argparse/argument_utils.py
+Comment: 
+
+Filename: ffstreamer/argparse/namespace_utils.py
+Comment: 
+
+Filename: ffstreamer/argparse/typing_namespace.py
+Comment: 
+
 Filename: ffstreamer/assets/__init__.py
 Comment: 
 
+Filename: ffstreamer/chrono/__init__.py
+Comment: 
+
+Filename: ffstreamer/chrono/datetime.py
+Comment: 
+
+Filename: ffstreamer/ffmpeg/__init__.py
+Comment: 
+
+Filename: ffstreamer/ffmpeg/ffmpeg.py
+Comment: 
+
+Filename: ffstreamer/ffmpeg/ffmpeg_process.py
+Comment: 
+
+Filename: ffstreamer/ffmpeg/ffmpeg_receiver.py
+Comment: 
+
+Filename: ffstreamer/ffmpeg/ffmpeg_sender.py
+Comment: 
+
+Filename: ffstreamer/ffmpeg/ffprobe.py
+Comment: 
+
+Filename: ffstreamer/ffmpeg/static_lib.py
+Comment: 
+
+Filename: ffstreamer/inspect/__init__.py
+Comment: 
+
+Filename: ffstreamer/inspect/type_origin.py
+Comment: 
+
 Filename: ffstreamer/logging/__init__.py
 Comment: 
 
 Filename: ffstreamer/logging/colored_formatter.py
 Comment: 
 
 Filename: ffstreamer/logging/logging.py
 Comment: 
 
+Filename: ffstreamer/memory/__init__.py
+Comment: 
+
+Filename: ffstreamer/memory/shared_memory_queue.py
+Comment: 
+
+Filename: ffstreamer/memory/shared_memory_utils.py
+Comment: 
+
+Filename: ffstreamer/memory/shared_memory_validator.py
+Comment: 
+
+Filename: ffstreamer/module/__init__.py
+Comment: 
+
+Filename: ffstreamer/module/errors.py
+Comment: 
+
+Filename: ffstreamer/module/module.py
+Comment: 
+
+Filename: ffstreamer/module/module_printer.py
+Comment: 
+
+Filename: ffstreamer/module/variables.py
+Comment: 
+
+Filename: ffstreamer/module/mixin/__init__.py
+Comment: 
+
+Filename: ffstreamer/module/mixin/_module_base.py
+Comment: 
+
+Filename: ffstreamer/module/mixin/module_doc.py
+Comment: 
+
+Filename: ffstreamer/module/mixin/module_frame.py
+Comment: 
+
+Filename: ffstreamer/module/mixin/module_open.py
+Comment: 
+
+Filename: ffstreamer/module/mixin/module_version.py
+Comment: 
+
+Filename: ffstreamer/network/__init__.py
+Comment: 
+
+Filename: ffstreamer/network/address_family.py
+Comment: 
+
+Filename: ffstreamer/package/__init__.py
+Comment: 
+
+Filename: ffstreamer/package/package_utils.py
+Comment: 
+
+Filename: ffstreamer/parse/__init__.py
+Comment: 
+
+Filename: ffstreamer/parse/cfg_parse.py
+Comment: 
+
+Filename: ffstreamer/parse/env_parse.py
+Comment: 
+
+Filename: ffstreamer/regex/__init__.py
+Comment: 
+
+Filename: ffstreamer/regex/access_filter.py
+Comment: 
+
+Filename: ffstreamer/system/__init__.py
+Comment: 
+
+Filename: ffstreamer/system/environ.py
+Comment: 
+
+Filename: ffstreamer/system/path_context.py
+Comment: 
+
+Filename: ffstreamer/types/__init__.py
+Comment: 
+
+Filename: ffstreamer/types/any/__init__.py
+Comment: 
+
+Filename: ffstreamer/types/any/to_string.py
+Comment: 
+
+Filename: ffstreamer/types/string/__init__.py
+Comment: 
+
+Filename: ffstreamer/types/string/to_any.py
+Comment: 
+
+Filename: ffstreamer/types/string/to_boolean.py
+Comment: 
+
 Filename: ffstreamer/www/__init__.py
 Comment: 
 
-Filename: ffstreamer-0.0.2.dist-info/LICENSE
+Filename: ffstreamer-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: ffstreamer-0.0.2.dist-info/METADATA
+Filename: ffstreamer-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: ffstreamer-0.0.2.dist-info/WHEEL
+Filename: ffstreamer-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: ffstreamer-0.0.2.dist-info/entry_points.txt
+Filename: ffstreamer-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: ffstreamer-0.0.2.dist-info/top_level.txt
+Filename: ffstreamer-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ffstreamer-0.0.2.dist-info/RECORD
+Filename: ffstreamer-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ffstreamer/__init__.py

```diff
@@ -1,3 +1,3 @@
 # -*- coding: utf-8 -*-
 
-__version__ = "0.0.2"
+__version__ = "0.0.5"
```

## ffstreamer/arguments.py

```diff
@@ -1,118 +1,53 @@
 # -*- coding: utf-8 -*-
 
 from argparse import REMAINDER, ArgumentParser, Namespace, RawDescriptionHelpFormatter
 from functools import lru_cache
 from typing import Final, List, Optional
 
+from ffstreamer.ffmpeg.ffmpeg import (
+    DEFAULT_FFMPEG_INPUT_FORMAT,
+    DEFAULT_FFMPEG_OUTPUT_FORMAT,
+)
 from ffstreamer.logging.logging import SEVERITIES, SEVERITY_NAME_INFO
-
-CMD_CLIENT: Final[str] = "client"
-CMD_MODULES: Final[str] = "modules"
-CMD_SERVER: Final[str] = "server"
+from ffstreamer.module.variables import MODULE_NAME_PREFIX, MODULE_PIPE_SEPARATOR
 
 PROG: Final[str] = "ffstreamer"
 DESCRIPTION: Final[str] = "FFmpeg Streamer"
-EPILOG: Final[str] = ""
+EPILOG = f"""
+Examples:
 
-DEFAULT_SEVERITY: Final[str] = SEVERITY_NAME_INFO
+  Debugging options:
+    $ {PROG} -c -d -vv ...
+
+  RTSP to RTSP:
+    $ {PROG} "rtsp://ip-camera/stream" rtsp "rtsp://localhost:8554/stream"
+"""
 
-CMD1 = "cmd1"
-CMD2 = "cmd2"
-CMDS = (CMD1, CMD2)
-
-CMD1_HELP: Final[str] = ""
-CMD1_EPILOG: Final[str] = ""
-
-CMD2_HELP: Final[str] = ""
-CMD2_EPILOG: Final[str] = ""
-
-DEFAULT_BIND: Final[str] = "0.0.0.0"
-DEFAULT_PORT: Final[int] = 8080
-DEFAULT_TIMEOUT: Final[float] = 1.0
+
+DEFAULT_SEVERITY: Final[str] = SEVERITY_NAME_INFO
+DEFAULT_MODULE_PREFIX: Final[str] = MODULE_NAME_PREFIX
 
 
 @lru_cache
 def version() -> str:
     # [IMPORTANT] Avoid 'circular import' issues
     from ffstreamer import __version__
 
     return __version__
 
 
-def add_cmd1_parser(subparsers) -> None:
-    # noinspection SpellCheckingInspection
-    parser = subparsers.add_parser(
-        name=CMD1,
-        help=CMD1_HELP,
-        formatter_class=RawDescriptionHelpFormatter,
-        epilog=CMD1_EPILOG,
-    )
-    assert isinstance(parser, ArgumentParser)
-
-    parser.add_argument(
-        "--bind",
-        "-b",
-        default=DEFAULT_BIND,
-        metavar="bind",
-        help=f"Bind address (default: '{DEFAULT_BIND}')",
-    )
-    parser.add_argument(
-        "--port",
-        "-p",
-        default=DEFAULT_PORT,
-        metavar="port",
-        help=f"Port number (default: '{DEFAULT_PORT}')",
-    )
-    parser.add_argument(
-        "--timeout",
-        "-t",
-        default=DEFAULT_TIMEOUT,
-        type=float,
-        help=f"Request timeout in seconds (default: {DEFAULT_TIMEOUT})",
-    )
-
-
-def add_cmd2_parser(subparsers) -> None:
-    # noinspection SpellCheckingInspection
-    parser = subparsers.add_parser(
-        name=CMD2,
-        help=CMD2_HELP,
-        formatter_class=RawDescriptionHelpFormatter,
-        epilog=CMD2_EPILOG,
-    )
-    assert isinstance(parser, ArgumentParser)
-
-    parser.add_argument(
-        "--config",
-        "-c",
-        default=None,
-        metavar="file",
-        help="Configuration file path",
-    )
-    parser.add_argument(
-        "module",
-        default=None,
-        nargs="?",
-        help="Module name",
-    )
-    parser.add_argument(
-        "opts",
-        nargs=REMAINDER,
-        help="Arguments of module",
-    )
-
-
 def default_argument_parser() -> ArgumentParser:
     parser = ArgumentParser(
         prog=PROG,
         description=DESCRIPTION,
         epilog=EPILOG,
         formatter_class=RawDescriptionHelpFormatter,
     )
+
     parser.add_argument(
         "--colored-logging",
         "-c",
         action="store_true",
         default=False,
         help="Use colored logging",
     )
@@ -146,17 +81,99 @@
     parser.add_argument(
         "--version",
         "-V",
         action="version",
         version=version(),
     )
 
-    subparsers = parser.add_subparsers(dest="cmd")
-    add_cmd1_parser(subparsers)
-    add_cmd2_parser(subparsers)
+    # --------------
+    # Module options
+    # --------------
+
+    parser.add_argument(
+        "--module-prefix",
+        metavar="prefix",
+        default=DEFAULT_MODULE_PREFIX,
+        help=f"The prefix of the module (default: '{DEFAULT_MODULE_PREFIX}')",
+    )
+    parser.add_argument(
+        "--list",
+        "-l",
+        action="store_true",
+        default=False,
+        help="Prints a list of available modules",
+    )
+
+    # --------------
+    # FFmpeg options
+    # --------------
+
+    parser.add_argument(
+        "--ffmpeg-path",
+        default="ffmpeg",
+        help="FFmpeg command path",
+    )
+    parser.add_argument(
+        "--ffprobe-path",
+        default="ffprobe",
+        help="FFprobe command path",
+    )
+    parser.add_argument(
+        "--input",
+        "-i",
+        default=DEFAULT_FFMPEG_INPUT_FORMAT,
+        help=(
+            "Commandline arguments of the FFmpeg input pipeline"
+            f" (Default is '{DEFAULT_FFMPEG_INPUT_FORMAT}')"
+        ),
+    )
+    parser.add_argument(
+        "--input-channels",
+        type=int,
+        default=3,
+        help="Number of channels to pipeline",
+    )
+    parser.add_argument(
+        "--output",
+        "-o",
+        default=DEFAULT_FFMPEG_OUTPUT_FORMAT,
+        help=(
+            "Commandline arguments of the FFmpeg output pipeline"
+            f" (Default is '{DEFAULT_FFMPEG_OUTPUT_FORMAT}')"
+        ),
+    )
+    parser.add_argument(
+        "--format",
+        "-f",
+        default="auto",
+        help="Output file format",
+    )
+    parser.add_argument(
+        "--preview",
+        "-p",
+        action="store_true",
+        default=False,
+        help="Display the preview window",
+    )
+
+    parser.add_argument(
+        "source",
+        help="Input source URL",
+    )
+    parser.add_argument(
+        "destination",
+        help="Output URL",
+    )
+
+    parser.add_argument(
+        "opts",
+        nargs=REMAINDER,
+        help=f"Module pipelines (Module pipe separator is '{MODULE_PIPE_SEPARATOR}')",
+    )
+
     return parser
 
 
 def get_default_arguments(
     cmdline: Optional[List[str]] = None,
     namespace: Optional[Namespace] = None,
 ) -> Namespace:
```

## ffstreamer/entrypoint.py

```diff
@@ -1,57 +1,40 @@
 # -*- coding: utf-8 -*-
 
-from argparse import Namespace
 from sys import exit as sys_exit
 from typing import Callable, List, Optional
 
-from ffstreamer.arguments import CMD1, CMD2, CMDS, get_default_arguments
+from ffstreamer.apps.default import main as default_main
+from ffstreamer.arguments import get_default_arguments
 from ffstreamer.logging.logging import (
     SEVERITY_NAME_DEBUG,
     logger,
     set_colored_formatter_logging_config,
     set_root_level,
     set_simple_logging_config,
 )
-
-
-def cmd1_main(args: Namespace, printer: Callable[..., None] = print) -> int:
-    assert args is not None
-    assert printer is not None
-    raise NotImplementedError
-
-
-def cmd2_main(args: Namespace, printer: Callable[..., None] = print) -> int:
-    assert args is not None
-    assert printer is not None
-    raise NotImplementedError
+from ffstreamer.module.module_printer import print_modules
 
 
 def main(
     cmdline: Optional[List[str]] = None,
     printer: Callable[..., None] = print,
 ) -> int:
     args = get_default_arguments(cmdline)
 
-    if not args.cmd:
-        printer("The command does not exist")
-        return 1
-
     if args.colored_logging and args.simple_logging:
         printer("The 'colored_logging' and 'simple_logging' flags cannot coexist")
         return 1
 
-    cmd = args.cmd
     colored_logging = args.colored_logging
     simple_logging = args.simple_logging
     severity = args.severity
     debug = args.debug
     verbose = args.verbose
 
-    assert cmd in CMDS
     assert isinstance(colored_logging, bool)
     assert isinstance(simple_logging, bool)
     assert isinstance(severity, str)
     assert isinstance(debug, bool)
     assert isinstance(verbose, int)
 
     if colored_logging:
@@ -62,21 +45,25 @@
     if debug:
         set_root_level(SEVERITY_NAME_DEBUG)
     else:
         set_root_level(severity)
 
     logger.debug(f"Arguments: {args}")
 
+    module_prefix = args.module_prefix
+    module_list = args.list
+    assert isinstance(module_prefix, str)
+    assert isinstance(module_list, bool)
+
+    if module_list:
+        print_modules(module_prefix, verbose, printer)
+        return 0
+
     try:
-        if cmd == CMD1:
-            return cmd1_main(args, printer=printer)
-        elif cmd == CMD2:
-            return cmd2_main(args, printer=printer)
-        else:
-            assert False, "Inaccessible section"
+        return default_main(args, printer=printer)
     except BaseException as e:
         logger.exception(e)
         return 1
 
 
 if __name__ == "__main__":
     sys_exit(main())
```

## ffstreamer/logging/logging.py

```diff
@@ -6,14 +6,15 @@
     ERROR,
     FATAL,
     INFO,
     NOTSET,
     WARN,
     WARNING,
     Formatter,
+    Logger,
     StreamHandler,
 )
 from logging import config as logging_config
 from logging import getLogger
 from sys import stdout
 from typing import Final, Literal, Optional, Union
 
@@ -95,31 +96,39 @@
             "formatter": "color",
             "stream": "ext://sys.stdout",
         },
         "file_default": {
             "class": "logging.FileHandler",
             "level": "DEBUG",
             "formatter": "default",
-            "filename": "recc.log",
+            "filename": "default.log",
             "mode": "a",
             "encoding": "utf-8",
             "delay": False,
         },
     },
     "loggers": {
         "": {  # root logger
             "handlers": ["console_color"],
             "level": "DEBUG",
         },
     },
 }
 
 DEFAULT_LOGGER_NAME = "ffstreamer"
+DEFAULT_LOGGER_INPUT_NAME = "ffstreamer.input"
+DEFAULT_LOGGER_OUTPUT_NAME = "ffstreamer.output"
 
 logger = getLogger(DEFAULT_LOGGER_NAME)
+input_logger = getLogger(DEFAULT_LOGGER_INPUT_NAME)
+output_logger = getLogger(DEFAULT_LOGGER_OUTPUT_NAME)
+
+
+def get_module_logger(name: str) -> Logger:
+    return getLogger(f"ffstreamer.module.{name}")
 
 
 def convert_level_number(level: Optional[Union[str, int]] = None) -> int:
     if level is None:
         return DEBUG
 
     if isinstance(level, str):
```

## Comparing `ffstreamer-0.0.2.dist-info/LICENSE` & `ffstreamer-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ffstreamer-0.0.2.dist-info/METADATA` & `ffstreamer-0.0.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffstreamer
-Version: 0.0.2
+Version: 0.0.5
 Summary: FFmpeg Streamer
 Home-page: https://github.com/osom8979/ffstreamer
 Author: zer0
 Author-email: osom8979@gmail.com
 Maintainer: zer0
 Maintainer-email: osom8979@gmail.com
 License: MIT License
@@ -20,14 +20,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs (>=15.0.1)
+Requires-Dist: static-ffmpeg (>=2.5)
 
 # ffstreamer
 
 [![PyPI](https://img.shields.io/pypi/v/ffstreamer?style=flat-square)](https://pypi.org/project/ffstreamer/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ffstreamer?style=flat-square)
 [![GitHub](https://img.shields.io/github/license/osom8979/ffstreamer?style=flat-square)](https://github.com/osom8979/ffstreamer/)
```

