# Comparing `tmp/rapid_videocr-2.2.3-py3-none-any.whl.zip` & `tmp/rapid_videocr-2.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15661 bytes, number of entries: 11
--rw-r--r--  2.0 unx      174 b- defN 23-Jul-08 11:38 rapid_videocr/__init__.py
--rw-r--r--  2.0 unx     4723 b- defN 23-Jul-08 11:38 rapid_videocr/main.py
--rw-r--r--  2.0 unx    13456 b- defN 23-Jul-08 11:38 rapid_videocr/rapid_videocr.py
--rw-r--r--  2.0 unx     4479 b- defN 23-Jul-08 11:38 rapid_videocr/utils.py
--rw-r--r--  2.0 unx     1264 b- defN 23-Jul-08 11:38 rapid_videocr/video_sub_finder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-08 11:38 rapid_videocr-2.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4650 b- defN 23-Jul-08 11:38 rapid_videocr-2.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 11:38 rapid_videocr-2.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Jul-08 11:38 rapid_videocr-2.2.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Jul-08 11:38 rapid_videocr-2.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      934 b- defN 23-Jul-08 11:38 rapid_videocr-2.2.3.dist-info/RECORD
-11 files, 41202 bytes uncompressed, 14071 bytes compressed:  65.8%
+Zip file size: 18371 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      174 b- defN 23-Jul-19 06:30 rapid_videocr/__init__.py
+-rw-r--r--  2.0 unx    10508 b- defN 23-Jul-19 06:30 rapid_videocr/main.py
+-rw-r--r--  2.0 unx    13571 b- defN 23-Jul-19 06:30 rapid_videocr/rapid_videocr.py
+-rw-r--r--  2.0 unx     5423 b- defN 23-Jul-19 06:30 rapid_videocr/utils.py
+-rw-r--r--  2.0 unx     3025 b- defN 23-Jul-19 06:30 rapid_videocr/video_sub_finder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8165 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      935 b- defN 23-Jul-19 06:30 rapid_videocr-2.2.4.dist-info/RECORD
+11 files, 53323 bytes uncompressed, 16781 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: rapid_videocr/utils.py
 Comment: 
 
 Filename: rapid_videocr/video_sub_finder.py
 Comment: 
 
-Filename: rapid_videocr-2.2.3.dist-info/LICENSE
+Filename: rapid_videocr-2.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: rapid_videocr-2.2.3.dist-info/METADATA
+Filename: rapid_videocr-2.2.4.dist-info/METADATA
 Comment: 
 
-Filename: rapid_videocr-2.2.3.dist-info/WHEEL
+Filename: rapid_videocr-2.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_videocr-2.2.3.dist-info/entry_points.txt
+Filename: rapid_videocr-2.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.3.dist-info/top_level.txt
+Filename: rapid_videocr-2.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.3.dist-info/RECORD
+Filename: rapid_videocr-2.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_videocr/main.py

```diff
@@ -1,26 +1,80 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
 from pathlib import Path
 from typing import Optional
 
-from .rapid_videocr import RapidVideOCR
-from .utils import get_logger
-from .video_sub_finder import VideoSubFinder
+try:
+    from .rapid_videocr import RapidVideOCR
+    from .utils import float_range, get_logger
+    from .video_sub_finder import VideoSubFinder
+except:
+    from utils import float_range, get_logger
+    from video_sub_finder import VideoSubFinder
+
+    from rapid_videocr import RapidVideOCR
 
 
 class RapidVideoSubFinderOCR:
-    def __init__(self, vsf_exe_path: Optional[str] = None, **ocr_params) -> None:
-        if vsf_exe_path is None:
-            raise ValueError("vsf_exe_path must not be None.")
+    def __init__(
+        self,
+        is_concat_rec: bool = False,
+        concat_batch: int = 10,
+        out_format: str = "all",
+        print_console: bool = False,
+        vsf_exe_path: Optional[str] = None,
+        clear_dirs: bool = True,
+        run_search: bool = True,
+        create_cleared_text_images: bool = True,
+        create_empty_sub: Optional[str] = None,
+        create_sub_from_cleared_txt_images: Optional[str] = None,
+        create_sub_from_txt_results: Optional[str] = None,
+        open_video_opencv: bool = True,
+        open_video_ffmpeg: bool = False,
+        use_cuda: bool = False,
+        start_time: Optional[str] = None,
+        end_time: Optional[str] = None,
+        top_video_image_percent_end: float = 0.2,
+        bottom_video_image_percent_end: float = 0.0,
+        left_video_image_percent_end: float = 0.0,
+        right_video_image_percent_end: float = 1.0,
+        general_settings: Optional[str] = None,
+        num_threads: int = -1,
+        num_ocr_threads: int = 1,
+    ) -> None:
+        self.vsf = VideoSubFinder(
+            vsf_exe_path,
+            clear_dirs,
+            run_search,
+            create_cleared_text_images,
+            create_empty_sub,
+            create_sub_from_cleared_txt_images,
+            create_sub_from_txt_results,
+            open_video_opencv,
+            open_video_ffmpeg,
+            use_cuda,
+            start_time,
+            end_time,
+            top_video_image_percent_end,
+            bottom_video_image_percent_end,
+            left_video_image_percent_end,
+            right_video_image_percent_end,
+            general_settings,
+            num_threads,
+            num_ocr_threads,
+        )
 
-        self.vsf = VideoSubFinder(vsf_exe_path)
-        self.video_ocr = RapidVideOCR(**ocr_params)
+        self.video_ocr = RapidVideOCR(
+            is_concat_rec=is_concat_rec,
+            concat_batch=concat_batch,
+            out_format=out_format,
+            is_print_console=print_console,
+        )
         self.video_formats = [".mp4", ".avi", ".mov", ".mkv"]
         self.logger = get_logger()
 
     def __call__(self, video_path: str, output_dir: str = "outputs"):
         if Path(video_path).is_dir():
             video_list = Path(video_path).rglob("*.*")
             video_list = [
@@ -31,121 +85,248 @@
 
         self.logger.info(
             "Extracting subtitle images with VideoSubFinder (takes quite a long time) ..."
         )
         video_num = len(video_list)
         for i, one_video in enumerate(video_list):
             self.logger.info(
-                f"[{i+1}/{video_num}] Starting to extract {one_video} key frame"
+                "[%s/%s] Starting to extract %s key frame",
+                i + 1,
+                video_num,
+                one_video,
             )
 
             save_name = Path(one_video).stem
             save_dir = Path(output_dir) / save_name
             save_vsf_dir = save_dir / "VSF_Results"
 
             try:
                 self.vsf(str(one_video), str(save_vsf_dir))
             except Exception as e:
-                self.logger.error(f"Extract {one_video} error, {e}, skip")
+                self.logger.error("Extract %s error, %s, skip", one_video, e)
                 continue
 
-            self.logger.info(f"[{i+1}/{video_num}] Starting to run {one_video} ocr")
+            self.logger.info(
+                "[%s/%s] Starting to run %s ocr", i + 1, video_num, one_video
+            )
 
             rgb_dir = Path(save_vsf_dir) / "RGBImages"
             if not list(rgb_dir.iterdir()):
-                self.logger.warning(f"Extracting frames from {one_video} is 0, skip")
+                self.logger.warning("Extracting frames from %s is 0, skip", one_video)
                 continue
             self.video_ocr(rgb_dir, save_dir, save_name=save_name)
 
 
-def main() -> None:
+def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-vsf",
-        "--vsf_exe_path",
-        type=str,
-        default=None,
-        help="The full path of VideoSubFinderWXW.exe.",
-    )
-    parser.add_argument(
+
+    videocr_param_group = parser.add_argument_group(title="VideOCRParameters")
+    videocr_param_group.add_argument(
         "-video_dir",
         "--video_dir",
         type=str,
         default=None,
         help="The full path of video or the path of video directory.",
     )
-    parser.add_argument(
+    videocr_param_group.add_argument(
         "-i",
         "--img_dir",
         type=str,
         default=None,
         help="The full path of RGBImages or TXTImages.",
     )
-    parser.add_argument(
+    videocr_param_group.add_argument(
         "-s",
         "--save_dir",
         type=str,
         default="outputs",
         help='The path of saving the recognition result. Default is "outputs" under the current directory.',
     )
-    parser.add_argument(
+    videocr_param_group.add_argument(
         "-o",
         "--out_format",
         type=str,
         default="all",
         choices=["srt", "txt", "all"],
         help='Output file format. Default is "all".',
     )
-    parser.add_argument(
-        "-m",
-        "--mode",
-        type=str,
-        default="single",
-        choices=["single", "concat"],
-        help='Which mode to run (concat recognition or single recognition). Default is "single".',
+    videocr_param_group.add_argument(
+        "--is_concat_rec",
+        action="store_true",
+        default=False,
+        help="Which mode to run (concat recognition or single recognition). Default is False.",
     )
-    parser.add_argument(
+    videocr_param_group.add_argument(
         "-b",
         "--concat_batch",
         type=int,
         default=10,
         help="The batch of concating image nums in concat recognition mode. Default is 10.",
     )
-    parser.add_argument(
+    videocr_param_group.add_argument(
         "-p",
         "--print_console",
-        type=bool,
-        default=0,
-        choices=[0, 1],
-        help="Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.",
+        action="store_true",
+        default=False,
+        help="Whether to print the subtitle results to console. -p means to print.",
     )
-    args = parser.parse_args()
 
-    is_concat_rec = "concat" in args.mode
+    vsf_param_group = parser.add_argument_group(title="VSFParameters")
+    vsf_param_group.add_argument(
+        "-vsf",
+        "--vsf_exe_path",
+        type=str,
+        default=None,
+        help="The full path of VideoSubFinderWXW.exe.",
+    )
+    vsf_param_group.add_argument(
+        "-c",
+        "--clear_dirs",
+        action="store_false",
+        default=True,
+        help="Clear Folders (remove all images), performed before any other steps. Default is True",
+    )
+    vsf_param_group.add_argument(
+        "-r",
+        "--run_search",
+        action="store_false",
+        default=True,
+        help="Run Search (find frames with hardcoded text (hardsub) on video) Default is True",
+    )
+    vsf_param_group.add_argument(
+        "-ccti",
+        "--create_cleared_text_images",
+        action="store_true",
+        default=False,
+        help="Create Cleared Text Images. Default is True",
+    )
+    vsf_param_group.add_argument(
+        "-ces",
+        "--create_empty_sub",
+        type=str,
+        default=None,
+        help="Create Empty Sub With Provided Output File Name (*.ass or *.srt)",
+    )
+    vsf_param_group.add_argument(
+        "-cscti",
+        "--create_sub_from_cleared_txt_images",
+        type=str,
+        default=None,
+        help="Create Sub From Cleared TXT Images With Provided Output File Name (*.ass or *.srt)",
+    )
+    vsf_param_group.add_argument(
+        "-cstxt",
+        "--create_sub_from_txt_results",
+        type=str,
+        default=None,
+        help="Create Sub From TXT Results With Provided Output File Name (*.ass or *.srt)",
+    )
+    vsf_param_group.add_argument(
+        "-ovocv",
+        "--open_video_opencv",
+        action="store_false",
+        default=True,
+        help="open video by OpenCV (default). Default is True",
+    )
+    vsf_param_group.add_argument(
+        "-ovffmpeg",
+        "--open_video_ffmpeg",
+        action="store_true",
+        default=False,
+        help="open video by FFMPEG",
+    )
+    vsf_param_group.add_argument(
+        "-uc", "--use_cuda", action="store_true", default=False, help="use cuda"
+    )
+    vsf_param_group.add_argument(
+        "--start_time",
+        type=str,
+        default="0:00:00:000",
+        help="start time, default = 0:00:00:000 (in format hour:min:sec:milisec)",
+    )
+    vsf_param_group.add_argument(
+        "--end_time",
+        type=str,
+        default=None,
+        help="end time, default = video length",
+    )
+    vsf_param_group.add_argument(
+        "-te",
+        "--top_video_image_percent_end",
+        type=float_range(0, 1.0),
+        default=0.2,
+        help="top video image percent offset from image bottom, can be in range [0.0,1.0], default = 1.0",
+    )
+    vsf_param_group.add_argument(
+        "-be",
+        "--bottom_video_image_percent_end",
+        type=float_range(0, 1.0),
+        default=0.0,
+        help="bottom video image percent offset from image bottom, can be in range [0.0,1.0], default = 0.0",
+    )
+    vsf_param_group.add_argument(
+        "-le",
+        "--left_video_image_percent_end",
+        type=float_range(0, 1.0),
+        default=0.0,
+        help="left video image percent end, can be in range [0.0,1.0], default = 0.0",
+    )
+    vsf_param_group.add_argument(
+        "-re",
+        "--right_video_image_percent_end",
+        type=float_range(0, 1.0),
+        default=1.0,
+        help="right video image percent end, can be in range [0.0,1.0], default = 1.0",
+    )
+    vsf_param_group.add_argument(
+        "-gs",
+        "--general_settings",
+        default=None,
+        help="general settings (path to general settings *.cfg file, default = settings/general.cfg)",
+    )
+    vsf_param_group.add_argument(
+        "-nthr",
+        "--num_threads",
+        type=int,
+        default=1,
+        help="number of threads used for Run Search",
+    )
+    vsf_param_group.add_argument(
+        "-nocrthr",
+        "--num_ocr_threads",
+        type=int,
+        default=1,
+        help="number of threads used for Create Cleared TXT Images",
+    )
+    args = parser.parse_args()
 
-    if not (args.vsf_exe_path is None and args.video_dir is None):
+    if args.vsf_exe_path is None and args.video_dir is None:
         raise ValueError(
             "--vsf_exe_path or --video_dir must not be None at the same time."
         )
 
-    if args.vsf_exe_path and args.video_dir:
-        extractor = RapidVideoSubFinderOCR(
-            vsf_exe_path=args.vsf_exe_path,
-            is_concat_rec=is_concat_rec,
-            concat_batch=args.concat_batch,
-            out_format=args.out_format,
-            is_print_console=args.print_console,
-        )
-        extractor(args.video_dir, args.save_dir)
-
-    if args.img_dir:
+    video_dir = args.video_dir
+    save_dir = args.save_dir
+    img_dir = args.img_dir
+
+    args_dict = vars(args)
+    del args_dict["video_dir"]
+    del args_dict["save_dir"]
+    del args_dict["img_dir"]
+
+    if args.vsf_exe_path and video_dir:
+        extractor = RapidVideoSubFinderOCR(**vars(args))
+        extractor(video_dir, save_dir)
+    elif img_dir:
         extractor = RapidVideOCR(
-            is_concat_rec=is_concat_rec,
+            is_concat_rec=args.is_concat_rec,
             concat_batch=args.concat_batch,
             out_format=args.out_format,
             is_print_console=args.print_console,
         )
-        extractor(args.img_dir, args.save_dir)
+        extractor(img_dir, save_dir)
+    else:
+        pass
 
 
 if __name__ == "__main__":
     main()
```

## rapid_videocr/rapid_videocr.py

```diff
@@ -6,21 +6,30 @@
 from typing import Dict, List, Optional, Tuple, Union
 
 import cv2
 import numpy as np
 from rapidocr_onnxruntime import RapidOCR
 from tqdm import tqdm
 
-from .utils import (
-    CropByProject,
-    compute_poly_iou,
-    get_logger,
-    is_inclusive_each_other,
-    mkdir,
-)
+try:
+    from .utils import (
+        CropByProject,
+        compute_poly_iou,
+        get_logger,
+        is_inclusive_each_other,
+        mkdir,
+    )
+except:
+    from utils import (
+        CropByProject,
+        compute_poly_iou,
+        get_logger,
+        is_inclusive_each_other,
+        mkdir,
+    )
 
 CUR_DIR = Path(__file__).resolve().parent
 logger = get_logger()
 
 
 class RapidVideOCR:
     def __init__(
@@ -289,15 +298,15 @@
         elif self.out_format == "srt":
             self.save_file(srt_path, srt_result)
         elif self.out_format == "all":
             self.save_file(txt_path, txt_result)
             self.save_file(srt_path, srt_result)
         else:
             raise ValueError(f"The {self.out_format} dost not support.")
-        logger.info(f"[OCR] The result has been saved to {save_dir} directory.")
+        logger.info("[OCR] The result has been saved to %s directory.", save_dir)
 
     def print_console(self, txt_result: List) -> None:
         for v in txt_result:
             print(v.strip())
 
     @staticmethod
     def save_file(save_path: Union[str, Path], content: List, mode: str = "w") -> None:
@@ -306,15 +315,15 @@
 
         if not isinstance(content, list):
             content = [content]
 
         with open(save_path, mode, encoding="utf-8") as f:
             for value in content:
                 f.write(f"{value}\n")
-        logger.info(f"[OCR] The file has been saved in the {save_path}")
+        logger.info("[OCR] The file has been saved in the %s", save_path)
 
     @staticmethod
     def _compute_centroid(points: np.ndarray) -> List:
         """计算所给框的质心坐标
 
         :param points ([type]): (4, 2)
         :return: [description]
@@ -361,20 +370,18 @@
         "--out_format",
         type=str,
         default="all",
         choices=["srt", "txt", "all"],
         help='Output file format. Default is "all".',
     )
     parser.add_argument(
-        "-m",
-        "--mode",
-        type=str,
-        default="single",
-        choices=["single", "concat"],
-        help='Which mode to run (concat recognition or single recognition). Default is "single".',
+        "--is_concat_rec",
+        action="store_true",
+        default=False,
+        help="Which mode to run (concat recognition or single recognition). Default is False.",
     )
     parser.add_argument(
         "-b",
         "--concat_batch",
         type=int,
         default=10,
         help="The batch of concating image nums in concat recognition mode. Default is 10.",
@@ -385,17 +392,16 @@
         type=bool,
         default=0,
         choices=[0, 1],
         help="Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.",
     )
     args = parser.parse_args()
 
-    is_concat_rec = "concat" in args.mode
     extractor = RapidVideOCR(
-        is_concat_rec=is_concat_rec,
+        is_concat_rec=args.is_concat_rec,
         concat_batch=args.concat_batch,
         out_format=args.out_format,
         is_print_console=args.print_console,
     )
     extractor(args.img_dir, args.save_dir)
```

## rapid_videocr/utils.py

```diff
@@ -1,25 +1,32 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
+import argparse
 import functools
 import logging
 import sys
+from enum import Enum
 from pathlib import Path
 from typing import List, Union
 
 import colorlog
 import cv2
 import numpy as np
 import shapely
 from shapely.geometry import MultiPoint, Polygon
 
 logger_initialized = {}
 
 
+class RecMode(Enum):
+    SINGLE = "single"
+    CONCAT = "concat"
+
+
 class CropByProject:
     """投影法裁剪"""
 
     def __init__(self, threshold=250):
         self.threshold = threshold
 
     def __call__(self, origin_img):
@@ -85,15 +92,15 @@
     for logger_name in logger_initialized:
         if name.startswith(logger_name):
             return logger
 
     fmt_string = "%(log_color)s[%(asctime)s] [%(name)s] %(levelname)s: %(message)s"
     log_colors = {
         "DEBUG": "white",
-        "INFO": "white",
+        "INFO": "green",
         "WARNING": "yellow",
         "ERROR": "red",
         "CRITICAL": "purple",
     }
     fmt = colorlog.ColoredFormatter(fmt_string, log_colors=log_colors)
     stream_handler = logging.StreamHandler(stream=sys.stdout)
     stream_handler.setFormatter(fmt)
@@ -164,7 +171,32 @@
 
     edge_x0, edge_y0 = np.min(box_max[:, 0]), np.min(box_max[:, 1])
     edge_x1, edge_y1 = np.max(box_max[:, 0]), np.max(box_max[:, 1])
 
     if x0 >= edge_x0 and y0 >= edge_y0 and x1 <= edge_x1 and y1 <= edge_y1:
         return True
     return False
+
+
+def float_range(mini, maxi):
+    """Return function handle of an argument type function for
+    ArgumentParser checking a float range: mini <= arg <= maxi
+      mini - minimum acceptable argument
+      maxi - maximum acceptable argument"""
+
+    # Define the function with default arguments
+    def float_range_checker(arg):
+        """New Type function for argparse - a float within predefined range."""
+
+        try:
+            f = float(arg)
+        except ValueError as exc:
+            raise argparse.ArgumentTypeError("must be a floating point number") from exc
+
+        if f < mini or f > maxi:
+            raise argparse.ArgumentTypeError(
+                "must be in range [" + str(mini) + " .. " + str(maxi) + "]"
+            )
+        return f
+
+    # Return function handle to checking function
+    return float_range_checker
```

## rapid_videocr/video_sub_finder.py

```diff
@@ -1,45 +1,84 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import subprocess
 from pathlib import Path
+from typing import Optional
 
 cur_dir = Path(__file__).resolve().parent
 
 
 class VideoSubFinder:
     def __init__(
         self,
-        vsf_exe_path: str,
-        num_threads: int = -1,
+        vsf_exe_path: Optional[str] = None,
+        clear_dirs: bool = True,
+        run_search: bool = True,
+        create_cleared_text_images: bool = True,
+        create_empty_sub: Optional[str] = None,
+        create_sub_from_cleared_txt_images: Optional[str] = None,
+        create_sub_from_txt_results: Optional[str] = None,
+        open_video_opencv: bool = True,
+        open_video_ffmpeg: bool = False,
+        use_cuda: bool = False,
+        start_time: Optional[str] = None,
+        end_time: Optional[str] = None,
         top_video_image_percent_end: float = 0.2,
+        bottom_video_image_percent_end: float = 0.0,
+        left_video_image_percent_end: float = 0.0,
+        right_video_image_percent_end: float = 1.0,
+        general_settings: Optional[str] = None,
+        num_threads: int = 2,
+        num_ocr_threads: int = 1,
     ) -> None:
-        self.te = top_video_image_percent_end
-        self.num_threads = num_threads
         self.exe_path = vsf_exe_path
+        if self.exe_path is None:
+            raise ValueError("VSF Exe path must not be None.")
+
+        param_dict = {
+            "clear_dirs": clear_dirs,
+            "run_search": run_search,
+            "create_cleared_text_images": create_cleared_text_images,
+            "create_empty_sub": create_empty_sub,
+            "create_sub_from_cleared_txt_images": create_sub_from_cleared_txt_images,
+            "create_sub_from_txt_results": create_sub_from_txt_results,
+            "open_video_opencv": open_video_opencv,
+            "open_video_ffmpeg": open_video_ffmpeg,
+            "use_cuda": use_cuda,
+            "start_time": start_time,
+            "end_time": end_time,
+            "top_video_image_percent_end": top_video_image_percent_end,
+            "bottom_video_image_percent_end": bottom_video_image_percent_end,
+            "left_video_image_percent_end": left_video_image_percent_end,
+            "right_video_image_percent_end": right_video_image_percent_end,
+            "general_settings": general_settings,
+            "num_threads": num_threads,
+            "num_ocr_threads": num_ocr_threads,
+        }
+
+        run_list = [self.exe_path]
+        for k, v in param_dict.items():
+            if v is None or str(v) == "False":
+                continue
+
+            if str(v) == "True":
+                run_list.append(f"--{str(k)}")
+            else:
+                run_list.extend([f"--{k}", str(v)])
+
+        self.run_list = run_list
 
     def __call__(self, video_path: str, output_dir: str) -> str:
+        self.run_list.extend(["--input_video", video_path, "--output_dir", output_dir])
+        print(self.run_list)
+
         try:
             subprocess.run(
-                [
-                    self.exe_path,
-                    "--clear_dirs",
-                    "--run_search",
-                    "--create_cleared_text_images",
-                    "--num_threads",
-                    str(self.num_threads),
-                    "--input_video",
-                    video_path,
-                    "--use_cuda",
-                    "--output_dir",
-                    output_dir,
-                    "--top_video_image_percent_end",
-                    str(self.te),
-                ],
+                self.run_list,
                 check=False,
             )
             return output_dir
         except Exception as e:
             raise e
```

## Comparing `rapid_videocr-2.2.3.dist-info/LICENSE` & `rapid_videocr-2.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

