# Comparing `tmp/playwright-recaptcha-0.2.0.tar.gz` & `tmp/playwright-recaptcha-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwright-recaptcha-0.2.0.tar", last modified: Sun Apr 16 21:45:00 2023, max compression
+gzip compressed data, was "playwright-recaptcha-0.3.0.tar", last modified: Wed Jul 19 02:38:43 2023, max compression
```

## Comparing `playwright-recaptcha-0.2.0.tar` & `playwright-recaptcha-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.484198 playwright-recaptcha-0.2.0/playwright_recaptcha/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/async_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    19070 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/recaptcha_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/sync_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/async_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/sync_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-16 21:45:00.000000 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-16 21:45:00.000000 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:45:00.000000 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-16 21:45:00.000000 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-16 21:45:00.000000 playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:45:00.488198 playwright-recaptcha-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/tests/test_async_recaptchav2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/tests/test_async_recaptchav3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/tests/test_sync_recaptchav2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-16 21:44:47.000000 playwright-recaptcha-0.2.0/tests/test_sync_recaptchav3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/playwright_recaptcha/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19244 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/async_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/recaptcha_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18050 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/sync_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/async_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/sync_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-19 02:38:43.000000 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-19 02:38:43.000000 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:38:43.000000 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 02:38:43.000000 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 02:38:43.000000 playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:38:43.581489 playwright-recaptcha-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/tests/test_async_recaptchav2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/tests/test_async_recaptchav3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/tests/test_sync_recaptchav2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-19 02:38:32.000000 playwright-recaptcha-0.3.0/tests/test_sync_recaptchav3.py
```

### Comparing `playwright-recaptcha-0.2.0/LICENSE` & `playwright-recaptcha-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.2.0/playwright_recaptcha/__init__.py` & `playwright-recaptcha-0.3.0/playwright_recaptcha/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """A library for solving reCAPTCHA v2 and v3 with Playwright."""
+
+__author__ = "Xewdy444"
+__version__ = "0.3.0"
+__license__ = "MIT"
+
 from playwright_recaptcha.errors import (
+    CapSolverError,
     RecaptchaError,
     RecaptchaNotFoundError,
     RecaptchaRateLimitError,
     RecaptchaSolveError,
     RecaptchaTimeoutError,
 )
 from playwright_recaptcha.recaptchav2.async_solver import AsyncSolver as AsyncSolverV2
 from playwright_recaptcha.recaptchav2.sync_solver import SyncSolver as SyncSolverV2
 from playwright_recaptcha.recaptchav3.async_solver import AsyncSolver as AsyncSolverV3
 from playwright_recaptcha.recaptchav3.sync_solver import SyncSolver as SyncSolverV3
 
 __all__ = [
+    "CapSolverError",
     "RecaptchaError",
     "RecaptchaNotFoundError",
     "RecaptchaRateLimitError",
     "RecaptchaSolveError",
     "RecaptchaTimeoutError",
     "AsyncSolverV2",
     "SyncSolverV2",
```

### Comparing `playwright-recaptcha-0.2.0/playwright_recaptcha/errors.py` & `playwright-recaptcha-0.3.0/playwright_recaptcha/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from typing import Optional
 
 
+class CapSolverError(Exception):
+    """An exception raised when the CapSolver API returns an error."""
+
+    def __init__(self, message: Optional[str] = None) -> None:
+        super().__init__(message or "The CapSolver API returned an error.")
+
+
 class RecaptchaError(Exception):
     """Base class for reCAPTCHA exceptions."""
 
 
-class RecaptchaSolveError(RecaptchaError):
-    """Base class for reCAPTCHA solve exceptions."""
+class RecaptchaNotFoundError(RecaptchaError):
+    """An exception raised when the reCAPTCHA was not found."""
 
     def __init__(self, message: Optional[str] = None) -> None:
-        super().__init__(message or "The reCAPTCHA could not be solved.")
+        super().__init__(message or "The reCAPTCHA was not found.")
 
 
-class RecaptchaNotFoundError(RecaptchaError):
-    """An exception raised when the reCAPTCHA was not found."""
+class RecaptchaSolveError(RecaptchaError):
+    """Base class for reCAPTCHA solve exceptions."""
 
-    def __init__(self) -> None:
-        super().__init__("The reCAPTCHA was not found.")
+    def __init__(self, message: Optional[str] = None) -> None:
+        super().__init__(message or "The reCAPTCHA could not be solved.")
 
 
 class RecaptchaRateLimitError(RecaptchaSolveError):
     """An exception raised when the reCAPTCHA rate limit has been exceeded."""
 
     def __init__(self) -> None:
         super().__init__("The reCAPTCHA rate limit has been exceeded.")
```

### Comparing `playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav2/recaptcha_box.py` & `playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav2/recaptcha_box.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,28 @@
 from __future__ import annotations
 
 import asyncio
 import re
 from abc import ABC, abstractmethod
 from functools import wraps
-from typing import Awaitable, Callable, Iterable, List, Tuple, Union
+from typing import Awaitable, Callable, Iterable, List, Tuple, Union, overload
 
 from playwright.async_api import Frame as AsyncFrame
 from playwright.async_api import Locator as AsyncLocator
 from playwright.sync_api import Frame as SyncFrame
 from playwright.sync_api import Locator as SyncLocator
 
-from playwright_recaptcha.errors import RecaptchaNotFoundError, RecaptchaSolveError
+from playwright_recaptcha.errors import RecaptchaNotFoundError
 
 Locator = Union[AsyncLocator, SyncLocator]
 Frame = Union[AsyncFrame, SyncFrame]
 
 
 class RecaptchaBox(ABC):
-    """
-    The base class for reCAPTCHA v2 boxes.
-
-    Attributes
-    ----------
-    anchor_frame : Frame
-        The reCAPTCHA anchor frame.
-    bframe_frame : Frame
-        The reCAPTCHA bframe frame.
-    checkbox : Locator
-        The reCAPTCHA checkbox locator.
-    audio_challenge_button : Locator
-        The reCAPTCHA audio challenge button locator.
-    new_challenge_button : Locator
-        The reCAPTCHA new challenge button locator.
-    audio_download_button : Locator
-        The reCAPTCHA audio download button locator.
-    audio_challenge_textbox : Locator
-        The reCAPTCHA audio challenge textbox locator.
-    audio_challenge_verify_button : Locator
-        The reCAPTCHA audio challenge verify button locator.
-
-    Methods
-    -------
-    from_frames(frames: Iterable[Frame]) -> Union[AsyncRecaptchaBox, SyncRecaptchaBox]
-        Create a reCAPTCHA box using a list of frames.
-    frames_are_attached() -> bool
-        Check if the reCAPTCHA frames are attached.
-    rate_limit_is_visible() -> bool
-        Check if the reCAPTCHA rate limit message is visible.
-    solve_failure_is_visible() -> bool
-        Check if the reCAPTCHA solve failure message is visible.
-    audio_challenge_is_visible() -> bool
-        Check if the reCAPTCHA audio challenge is visible.
-    is_solved() -> bool
-        Check if the reCAPTCHA challenge is solved.
-
-    Raises
-    ------
-    RecaptchaNotFoundError
-        If the reCAPTCHA was not found.
-    RecaptchaSolveError
-        If no unchecked reCAPTCHA boxes were found.
-    """
+    """The base class for reCAPTCHA v2 boxes."""
 
     @staticmethod
     def _get_recaptcha_frame_pairs(
         frames: Iterable[Frame],
     ) -> List[Tuple[Frame, Frame]]:
         """
         Get the reCAPTCHA anchor and bframe frame pairs.
@@ -81,33 +38,25 @@
             A list of reCAPTCHA anchor and bframe frame pairs.
 
         Raises
         ------
         RecaptchaNotFoundError
             If no reCAPTCHA anchor and bframe frame pairs were found.
         """
-        anchor_frames = list(
-            filter(
-                lambda frame: re.search(
-                    "/recaptcha/(api2|enterprise)/anchor", frame.url
-                )
-                is not None,
-                frames,
-            )
-        )
+        anchor_frames = [
+            frame
+            for frame in frames
+            if re.search("/recaptcha/(api2|enterprise)/anchor", frame.url) is not None
+        ]
 
-        bframe_frames = list(
-            filter(
-                lambda frame: re.search(
-                    "/recaptcha/(api2|enterprise)/bframe", frame.url
-                )
-                is not None,
-                frames,
-            )
-        )
+        bframe_frames = [
+            frame
+            for frame in frames
+            if re.search("/recaptcha/(api2|enterprise)/bframe", frame.url) is not None
+        ]
 
         frame_pairs = []
 
         for anchor_frame in anchor_frames:
             frame_id = anchor_frame.name[2:]
 
             for bframe_frame in bframe_frames:
@@ -115,56 +64,56 @@
                     frame_pairs.append((anchor_frame, bframe_frame))
 
         if not frame_pairs:
             raise RecaptchaNotFoundError
 
         return frame_pairs
 
-    @staticmethod
+    @overload
     def _check_if_attached(
-        func: Union[
-            Callable[[AsyncRecaptchaBox], Awaitable[bool]],
-            Callable[[SyncRecaptchaBox], bool],
-        ]
-    ) -> Union[
-        Callable[[AsyncRecaptchaBox], Awaitable[bool]],
-        Callable[[SyncRecaptchaBox], bool],
-    ]:
+        func: Callable[[AsyncRecaptchaBox], Awaitable[bool]]
+    ) -> Callable[[AsyncRecaptchaBox], Awaitable[bool]]:
+        ...
+
+    @overload
+    def _check_if_attached(
+        func: Callable[[SyncRecaptchaBox], bool]
+    ) -> Callable[[SyncRecaptchaBox], bool]:
+        ...
+
+    @staticmethod
+    def _check_if_attached(func):
         """
         Check if the reCAPTCHA frames are attached before running the decorated function,
         otherwise return False.
 
         Parameters
         ----------
-        func : Union[
-            Callable[[AsyncRecaptchaBox], Awaitable[bool]], Callable[[SyncRecaptchaBox], bool]
-        ]
+        func : Callable[[AsyncRecaptchaBox], Awaitable[bool]] or Callable[[SyncRecaptchaBox], bool]
             The function to decorate.
 
         Returns
         -------
-        Union[
-            Callable[[AsyncRecaptchaBox], Awaitable[bool]], Callable[[SyncRecaptchaBox], bool]
-        ]
+        Callable[[AsyncRecaptchaBox], Awaitable[bool]] or Callable[[SyncRecaptchaBox], bool]
             The decorated function.
         """
 
         @wraps(func)
-        def sync_wrapper(self: SyncRecaptchaBox) -> bool:
-            if self.frames_are_detached():
+        def sync_wrapper(recaptcha_box: SyncRecaptchaBox) -> bool:
+            if recaptcha_box.frames_are_detached():
                 return False
 
-            return func(self)
+            return func(recaptcha_box)
 
         @wraps(func)
-        async def async_wrapper(self: AsyncRecaptchaBox) -> bool:
-            if self.frames_are_detached():
+        async def async_wrapper(recaptcha_box: AsyncRecaptchaBox) -> bool:
+            if recaptcha_box.frames_are_detached():
                 return False
 
-            return await func(self)
+            return await func(recaptcha_box)
 
         if asyncio.iscoroutinefunction(func):
             return async_wrapper
 
         return sync_wrapper
 
     @property
@@ -191,30 +140,48 @@
 
     @property
     def audio_challenge_textbox(self) -> Locator:
         """The reCAPTCHA audio challenge textbox locator."""
         return self.bframe_frame.get_by_role("textbox", name="Enter what you hear")
 
     @property
-    def audio_challenge_verify_button(self) -> Locator:
-        """The reCAPTCHA audio challenge verify button locator."""
+    def skip_button(self) -> Locator:
+        """The reCAPTCHA skip button locator."""
+        return self.bframe_frame.get_by_role("button", name="Skip")
+
+    @property
+    def next_button(self) -> Locator:
+        """The reCAPTCHA next button locator."""
+        return self.bframe_frame.get_by_role("button", name="Next")
+
+    @property
+    def verify_button(self) -> Locator:
+        """The reCAPTCHA verify button locator."""
         return self.bframe_frame.get_by_role("button", name="Verify")
 
+    @property
+    def tile_selector(self) -> Locator:
+        """The reCAPTCHA tile selector locator."""
+        return self.bframe_frame.locator(".rc-imageselect-tile")
+
+    @property
+    def image_challenge(self) -> Locator:
+        """The reCAPTCHA image challenge locator."""
+        return self.bframe_frame.locator(".rc-imageselect-challenge")
+
     def frames_are_attached(self) -> bool:
         """
-        Check if the reCAPTCHA frames are attached.
+        Check if all of the reCAPTCHA frames are attached.
 
         Returns
         -------
         bool
-            True if the reCAPTCHA frames are attached, False otherwise.
+            True if all of the reCAPTCHA frames are attached, False otherwise.
         """
-        return (
-            not self.anchor_frame.is_detached() and not self.bframe_frame.is_detached()
-        )
+        return not self.frames_are_detached()
 
     def frames_are_detached(self) -> bool:
         """
         Check if any of the reCAPTCHA frames are detached.
 
         Returns
         -------
@@ -251,17 +218,15 @@
         -------
         Union[AsyncRecaptchaBox, SyncRecaptchaBox]
             The reCAPTCHA box.
 
         Raises
         ------
         RecaptchaNotFoundError
-            If the reCAPTCHA frames were not found.
-        RecaptchaSolveError
-            If no unchecked reCAPTCHA boxes were found.
+            If the reCAPTCHA frames were not found or if no unchecked reCAPTCHA boxes were found.
         """
 
     @abstractmethod
     def rate_limit_is_visible(self) -> bool:
         """
         Check if the reCAPTCHA rate limit message is visible.
 
@@ -290,76 +255,79 @@
         Returns
         -------
         bool
             True if the reCAPTCHA audio challenge is visible, False otherwise.
         """
 
     @abstractmethod
-    def is_solved(self) -> bool:
+    def try_again_is_visible(self) -> bool:
         """
-        Check if the reCAPTCHA challenge is solved.
+        Check if the reCAPTCHA try again message is visible.
 
         Returns
         -------
         bool
-            True if the reCAPTCHA challenge is solved, False otherwise.
+            True if the reCAPTCHA try again message is visible, False otherwise.
+        """
+
+    @abstractmethod
+    def check_new_images_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA check new images message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA check new images message is visible, False otherwise.
+        """
+
+    @abstractmethod
+    def select_all_matching_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA select all matching images message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA select all matching images message is visible, False otherwise.
+        """
+
+    @abstractmethod
+    def challenge_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA challenge is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA challenge is visible, False otherwise.
+        """
+
+    @abstractmethod
+    def challenge_is_solved(self) -> bool:
+        """
+        Check if the reCAPTCHA challenge has been solved.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA challenge has been solved, False otherwise.
         """
 
 
 class SyncRecaptchaBox(RecaptchaBox):
     """
     The synchronous class for reCAPTCHA v2 boxes.
 
     Parameters
     ----------
     anchor_frame : SyncFrame
         The reCAPTCHA anchor frame.
     bframe_frame : SyncFrame
         The reCAPTCHA bframe frame.
-
-    Attributes
-    ----------
-    anchor_frame : Frame
-        The reCAPTCHA anchor frame.
-    bframe_frame : Frame
-        The reCAPTCHA bframe frame.
-    checkbox : Locator
-        The reCAPTCHA checkbox locator.
-    audio_challenge_button : Locator
-        The reCAPTCHA audio challenge button locator.
-    new_challenge_button : Locator
-        The reCAPTCHA new challenge button locator.
-    audio_download_button : Locator
-        The reCAPTCHA audio download button locator.
-    audio_challenge_textbox : Locator
-        The reCAPTCHA audio challenge textbox locator.
-    audio_challenge_verify_button : Locator
-        The reCAPTCHA audio challenge verify button locator.
-
-    Methods
-    -------
-    from_frames(frames: Iterable[SyncFrame]) -> SyncRecaptchaBox
-        Create a reCAPTCHA box using a list of frames.
-    frames_are_attached() -> bool
-        Check if the reCAPTCHA frames are attached.
-    rate_limit_is_visible() -> bool
-        Check if the reCAPTCHA rate limit message is visible.
-    solve_failure_is_visible() -> bool
-        Check if the reCAPTCHA solve failure message is visible.
-    audio_challenge_is_visible() -> bool
-        Check if the reCAPTCHA audio challenge is visible.
-    is_solved() -> bool
-        Check if the reCAPTCHA challenge is solved.
-
-    Raises
-    ------
-    RecaptchaNotFoundError
-        If the reCAPTCHA was not found.
-    RecaptchaSolveError
-        If no unchecked reCAPTCHA boxes were found.
     """
 
     def __init__(self, anchor_frame: SyncFrame, bframe_frame: SyncFrame) -> None:
         self._anchor_frame = anchor_frame
         self._bframe_frame = bframe_frame
 
     def __repr__(self) -> str:
@@ -379,17 +347,15 @@
         -------
         SyncRecaptchaBox
             The reCAPTCHA box.
 
         Raises
         ------
         RecaptchaNotFoundError
-            If the reCAPTCHA frames were not found.
-        RecaptchaSolveError
-            If no unchecked reCAPTCHA boxes were found.
+            If the reCAPTCHA frames were not found or if no unchecked reCAPTCHA boxes were found.
         """
         frame_pairs = cls._get_recaptcha_frame_pairs(frames)
 
         for anchor_frame, bframe_frame in frame_pairs:
             checkbox = anchor_frame.get_by_role("checkbox", name="I'm not a robot")
 
             if (
@@ -397,15 +363,15 @@
                     "button", name="Get an audio challenge"
                 ).is_visible()
                 or checkbox.is_visible()
                 and not checkbox.is_checked()
             ):
                 return cls(anchor_frame, bframe_frame)
 
-        raise RecaptchaSolveError("No unchecked reCAPTCHA boxes were found.")
+        raise RecaptchaNotFoundError("No unchecked reCAPTCHA boxes were found.")
 
     @property
     def anchor_frame(self) -> SyncFrame:
         """The reCAPTCHA anchor frame."""
         return self._anchor_frame
 
     @property
@@ -448,77 +414,91 @@
         -------
         bool
             True if the reCAPTCHA audio challenge is visible, False otherwise.
         """
         return self.bframe_frame.get_by_text("Press PLAY to listen").is_visible()
 
     @RecaptchaBox._check_if_attached
-    def is_solved(self) -> bool:
+    def try_again_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA try again message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA try again message is visible, False otherwise.
+        """
+        return self.bframe_frame.get_by_text(
+            re.compile("Please try again")
+        ).is_visible()
+
+    @RecaptchaBox._check_if_attached
+    def check_new_images_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA check new images message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA check new images message is visible, False otherwise.
+        """
+        return self.bframe_frame.get_by_text(
+            re.compile("Please also check the new images")
+        ).is_visible()
+
+    @RecaptchaBox._check_if_attached
+    def select_all_matching_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA select all matching images message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA select all matching images message is visible, False otherwise.
+        """
+        return self.bframe_frame.get_by_text(
+            re.compile("Please select all matching images")
+        ).is_visible()
+
+    @RecaptchaBox._check_if_attached
+    def challenge_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA challenge is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA challenge is visible, False otherwise.
+        """
+        button = self.skip_button.or_(self.next_button).or_(self.verify_button)
+        return button.is_enabled()
+
+    @RecaptchaBox._check_if_attached
+    def challenge_is_solved(self) -> bool:
         """
-        Check if the reCAPTCHA challenge is solved.
+        Check if the reCAPTCHA challenge has been solved.
 
         Returns
         -------
         bool
-            True if the reCAPTCHA challenge is solved, False otherwise.
+            True if the reCAPTCHA challenge has been solved, False otherwise.
         """
         return self.checkbox.is_visible() and self.checkbox.is_checked()
 
 
 class AsyncRecaptchaBox(RecaptchaBox):
     """
     The asynchronous class for reCAPTCHA v2 boxes.
 
     Parameters
     ----------
     anchor_frame : AsyncFrame
         The reCAPTCHA anchor frame.
     bframe_frame : AsyncFrame
         The reCAPTCHA bframe frame.
-
-    Attributes
-    ----------
-    anchor_frame : Frame
-        The reCAPTCHA anchor frame.
-    bframe_frame : Frame
-        The reCAPTCHA bframe frame.
-    checkbox : Locator
-        The reCAPTCHA checkbox locator.
-    audio_challenge_button : Locator
-        The reCAPTCHA audio challenge button locator.
-    new_challenge_button : Locator
-        The reCAPTCHA new challenge button locator.
-    audio_download_button : Locator
-        The reCAPTCHA audio download button locator.
-    audio_challenge_textbox : Locator
-        The reCAPTCHA audio challenge textbox locator.
-    audio_challenge_verify_button : Locator
-        The reCAPTCHA audio challenge verify button locator.
-
-    Methods
-    -------
-    from_frames(frames: Iterable[AsyncFrame]) -> AsyncRecaptchaBox
-        Create a reCAPTCHA box using a list of frames.
-    frames_are_attached() -> bool
-        Check if the reCAPTCHA frames are attached.
-    rate_limit_is_visible() -> bool
-        Check if the reCAPTCHA rate limit message is visible.
-    solve_failure_is_visible() -> bool
-        Check if the reCAPTCHA solve failure message is visible.
-    audio_challenge_is_visible() -> bool
-        Check if the reCAPTCHA audio challenge is visible.
-    is_solved() -> bool
-        Check if the reCAPTCHA challenge is solved.
-
-    Raises
-    ------
-    RecaptchaNotFoundError
-        If the reCAPTCHA was not found.
-    RecaptchaSolveError
-        If no unchecked reCAPTCHA boxes were found.
     """
 
     def __init__(self, anchor_frame: AsyncFrame, bframe_frame: AsyncFrame) -> None:
         self._anchor_frame = anchor_frame
         self._bframe_frame = bframe_frame
 
     def __repr__(self) -> str:
@@ -538,17 +518,15 @@
         -------
         AsyncRecaptchaBox
             The reCAPTCHA box.
 
         Raises
         ------
         RecaptchaNotFoundError
-            If the reCAPTCHA frames were not found.
-        RecaptchaSolveError
-            If no unchecked reCAPTCHA boxes were found.
+            If the reCAPTCHA frames were not found or if no unchecked reCAPTCHA boxes were found.
         """
         frame_pairs = cls._get_recaptcha_frame_pairs(frames)
 
         for anchor_frame, bframe_frame in frame_pairs:
             checkbox = anchor_frame.get_by_role("checkbox", name="I'm not a robot")
 
             if (
@@ -556,15 +534,15 @@
                     "button", name="Get an audio challenge"
                 ).is_visible()
                 or await checkbox.is_visible()
                 and not await checkbox.is_checked()
             ):
                 return cls(anchor_frame, bframe_frame)
 
-        raise RecaptchaSolveError("No unchecked reCAPTCHA boxes were found.")
+        raise RecaptchaNotFoundError("No unchecked reCAPTCHA boxes were found.")
 
     @property
     def anchor_frame(self) -> AsyncFrame:
         """The reCAPTCHA anchor frame."""
         return self._anchor_frame
 
     @property
@@ -607,17 +585,72 @@
         -------
         bool
             True if the reCAPTCHA audio challenge is visible, False otherwise.
         """
         return await self.bframe_frame.get_by_text("Press PLAY to listen").is_visible()
 
     @RecaptchaBox._check_if_attached
-    async def is_solved(self) -> bool:
+    async def try_again_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA try again message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA try again message is visible, False otherwise.
+        """
+        return await self.bframe_frame.get_by_text(
+            re.compile("Please try again")
+        ).is_visible()
+
+    @RecaptchaBox._check_if_attached
+    async def check_new_images_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA check new images message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA check new images message is visible, False otherwise.
+        """
+        return await self.bframe_frame.get_by_text(
+            re.compile("Please also check the new images")
+        ).is_visible()
+
+    @RecaptchaBox._check_if_attached
+    async def select_all_matching_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA select all matching images message is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA select all matching images message is visible, False otherwise.
+        """
+        return await self.bframe_frame.get_by_text(
+            re.compile("Please select all matching images")
+        ).is_visible()
+
+    @RecaptchaBox._check_if_attached
+    async def challenge_is_visible(self) -> bool:
+        """
+        Check if the reCAPTCHA challenge is visible.
+
+        Returns
+        -------
+        bool
+            True if the reCAPTCHA challenge is visible, False otherwise.
+        """
+        button = self.skip_button.or_(self.next_button).or_(self.verify_button)
+        return await button.is_enabled()
+
+    @RecaptchaBox._check_if_attached
+    async def challenge_is_solved(self) -> bool:
         """
-        Check if the reCAPTCHA challenge is solved.
+        Check if the reCAPTCHA challenge has been solved.
 
         Returns
         -------
         bool
-            True if the reCAPTCHA challenge is solved, False otherwise.
+            True if the reCAPTCHA challenge has been solved, False otherwise.
         """
         return await self.checkbox.is_visible() and await self.checkbox.is_checked()
```

### Comparing `playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/async_solver.py` & `playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/async_solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,55 +15,40 @@
 
     Parameters
     ----------
     page : Page
         The playwright page to solve the reCAPTCHA on.
     timeout : int, optional
         The solve timeout in seconds, by default 30.
-
-    Attributes
-    ----------
-    token : Optional[str]
-        The g-recaptcha-response token.
-
-    Methods
-    -------
-    close() -> None
-        Remove the reload response listener.
-    solve_recaptcha(timeout: Optional[int] = None) -> str
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
-
-    Raises
-    ------
-    RecaptchaTimeoutError
-        If the solve timeout has been exceeded.
     """
 
     def __init__(self, page: Page, timeout: int = 30) -> None:
         self._page = page
         self._timeout = timeout
+
         self.token: Optional[str] = None
+        self._page.on("response", self._extract_token)
 
     def __repr__(self) -> str:
         return f"AsyncSolver(page={self._page!r}, timeout={self._timeout!r})"
 
     async def __aenter__(self) -> AsyncSolver:
         return self
 
     async def __aexit__(self, *args: Any) -> None:
         self.close()
 
     async def _extract_token(self, response: Response) -> None:
         """
-        Extract the g-recaptcha-response token from the userverify response.
+        Extract the `g-recaptcha-response` token from the userverify response.
 
         Parameters
         ----------
         response : Response
-            The response to extract the g-recaptcha-response token from.
+            The response to extract the `g-recaptcha-response` token from.
         """
         if re.search("/recaptcha/(api2|enterprise)/reload", response.url) is None:
             return
 
         token_match = re.search('"rresp","(.*?)"', await response.text())
 
         if token_match is not None:
@@ -74,34 +59,32 @@
         try:
             self._page.remove_listener("response", self._extract_token)
         except KeyError:
             pass
 
     async def solve_recaptcha(self, timeout: Optional[int] = None) -> str:
         """
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
+        Wait for the reCAPTCHA to be solved and return the `g-recaptcha-response` token.
 
         Parameters
         ----------
         timeout : Optional[int], optional
             The solve timeout in seconds, by default 30.
 
         Returns
         -------
         str
-            The g-recaptcha-response token.
+            The `g-recaptcha-response` token.
 
         Raises
         ------
         RecaptchaTimeoutError
             If the solve timeout has been exceeded.
         """
         self.token = None
-        self._page.on("response", self._extract_token)
-
         timeout = timeout or self._timeout
         start_time = time.time()
 
         while self.token is None:
             if time.time() - start_time >= timeout:
                 raise RecaptchaTimeoutError
```

### Comparing `playwright-recaptcha-0.2.0/playwright_recaptcha/recaptchav3/sync_solver.py` & `playwright-recaptcha-0.3.0/playwright_recaptcha/recaptchav3/sync_solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,55 +15,40 @@
 
     Parameters
     ----------
     page : Page
         The playwright page to solve the reCAPTCHA on.
     timeout : int, optional
         The solve timeout in seconds, by default 30.
-
-    Attributes
-    ----------
-    token : Optional[str]
-        The g-recaptcha-response token.
-
-    Methods
-    -------
-    close() -> None
-        Remove the reload response listener.
-    solve_recaptcha(timeout: Optional[int] = None) -> str
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
-
-    Raises
-    ------
-    RecaptchaTimeoutError
-        If the solve timeout has been exceeded.
     """
 
     def __init__(self, page: Page, timeout: int = 30) -> None:
         self._page = page
         self._timeout = timeout
+
         self.token: Optional[str] = None
+        self._page.on("response", self._extract_token)
 
     def __repr__(self) -> str:
         return f"SyncSolver(page={self._page!r}, timeout={self._timeout!r})"
 
     def __enter__(self) -> SyncSolver:
         return self
 
     def __exit__(self, *args: Any) -> None:
         self.close()
 
     def _extract_token(self, response: Response) -> None:
         """
-        Extract the g-recaptcha-response token from the userverify response.
+        Extract the `g-recaptcha-response` token from the userverify response.
 
         Parameters
         ----------
         response : Response
-            The response to extract the g-recaptcha-response token from.
+            The response to extract the `g-recaptcha-response` token from.
         """
         if re.search("/recaptcha/(api2|enterprise)/reload", response.url) is None:
             return
 
         token_match = re.search('"rresp","(.*?)"', response.text())
 
         if token_match is not None:
@@ -74,25 +59,25 @@
         try:
             self._page.remove_listener("response", self._extract_token)
         except KeyError:
             pass
 
     def solve_recaptcha(self, timeout: Optional[int] = None) -> str:
         """
-        Solve the reCAPTCHA and return the g-recaptcha-response token.
+        Wait for the reCAPTCHA to be solved and return the `g-recaptcha-response` token.
 
         Parameters
         ----------
         timeout : Optional[int], optional
             The solve timeout in seconds, by default 30.
 
         Returns
         -------
         str
-            The g-recaptcha-response token.
+            The `g-recaptcha-response` token.
 
         Raises
         ------
         RecaptchaTimeoutError
             If the solve timeout has been exceeded.
         """
         self.token = None
```

### Comparing `playwright-recaptcha-0.2.0/playwright_recaptcha.egg-info/SOURCES.txt` & `playwright-recaptcha-0.3.0/playwright_recaptcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playwright-recaptcha-0.2.0/setup.py` & `playwright-recaptcha-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf-8") as file:
     long_description = file.read()
 
 setup(
     name="playwright-recaptcha",
-    version="0.2.0",
+    version="0.3.0",
     author="Xewdy444",
     author_email="xewdy@xewdy.tech",
     description="A library for solving reCAPTCHA v2 and v3 with Playwright",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xewdy444/Playwright-reCAPTCHA",
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=[
-        "playwright==1.32.1",
+        "playwright==1.36.0",
         "pydub==0.25.1",
         "SpeechRecognition==3.10.0",
+        "tenacity==8.2.2",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

### Comparing `playwright-recaptcha-0.2.0/tests/test_async_recaptchav2.py` & `playwright-recaptcha-0.3.0/tests/test_async_recaptchav2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 import pytest
 from playwright.async_api import async_playwright
 
 from playwright_recaptcha import (
+    CapSolverError,
     RecaptchaNotFoundError,
     RecaptchaRateLimitError,
     recaptchav2,
 )
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=RecaptchaRateLimitError)
 async def test_solver_with_normal_recaptcha() -> None:
     """Test the solver with a normal reCAPTCHA."""
     async with async_playwright() as playwright:
         browser = await playwright.firefox.launch()
         page = await browser.new_page()
-
-        await page.goto(
-            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-        )
+        await page.goto("https://www.google.com/recaptcha/api2/demo")
 
         async with recaptchav2.AsyncSolver(page) as solver:
-            await solver.solve_recaptcha()
+            await solver.solve_recaptcha(wait=True)
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=(RecaptchaNotFoundError, RecaptchaRateLimitError))
 async def test_solver_with_hidden_recaptcha() -> None:
     """Test the solver with a hidden reCAPTCHA."""
     async with async_playwright() as playwright:
         browser = await playwright.firefox.launch()
         page = await browser.new_page()
 
-        await page.goto(
-            "https://www.google.com/recaptcha/api2/demo?invisible=true",
-            wait_until="networkidle",
-        )
-
+        await page.goto("https://www.google.com/recaptcha/api2/demo?invisible=true")
         await page.get_by_role("button").click()
 
         async with recaptchav2.AsyncSolver(page) as solver:
-            await solver.solve_recaptcha()
+            await solver.solve_recaptcha(wait=True)
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=RecaptchaRateLimitError)
 async def test_solver_with_slow_browser() -> None:
     """Test the solver with a slow browser."""
     async with async_playwright() as playwright:
         browser = await playwright.firefox.launch(slow_mo=1000)
         page = await browser.new_page()
+        await page.goto("https://www.google.com/recaptcha/api2/demo")
+
+        async with recaptchav2.AsyncSolver(page) as solver:
+            await solver.solve_recaptcha(wait=True)
+
 
-        await page.goto(
-            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-        )
+@pytest.mark.asyncio
+@pytest.mark.xfail(raises=CapSolverError)
+async def test_solver_with_image_challenge() -> None:
+    """Test the solver with an image challenge."""
+    async with async_playwright() as playwright:
+        browser = await playwright.firefox.launch()
+        page = await browser.new_page()
+        await page.goto("https://www.google.com/recaptcha/api2/demo")
 
         async with recaptchav2.AsyncSolver(page) as solver:
-            await solver.solve_recaptcha()
+            await solver.solve_recaptcha(wait=True, image_challenge=True)
 
 
 @pytest.mark.asyncio
 async def test_recaptcha_not_found_error() -> None:
     """Test the solver with a page that does not have a reCAPTCHA."""
     async with async_playwright() as playwright:
         browser = await playwright.firefox.launch()
```

### Comparing `playwright-recaptcha-0.2.0/tests/test_async_recaptchav3.py` & `playwright-recaptcha-0.3.0/tests/test_async_recaptchav3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import pytest
 from playwright.async_api import async_playwright
 
-from playwright_recaptcha import (
-    RecaptchaTimeoutError,
-    recaptchav3,
-)
+from playwright_recaptcha import RecaptchaTimeoutError, recaptchav3
 
 
 @pytest.mark.asyncio
 async def test_solver_with_normal_browser() -> None:
     """Test the solver with a normal browser."""
     async with async_playwright() as playwright:
         browser = await playwright.firefox.launch()
```

### Comparing `playwright-recaptcha-0.2.0/tests/test_sync_recaptchav2.py` & `playwright-recaptcha-0.3.0/tests/test_sync_recaptchav2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 import pytest
 from playwright.sync_api import sync_playwright
 
 from playwright_recaptcha import (
+    CapSolverError,
     RecaptchaNotFoundError,
     RecaptchaRateLimitError,
     recaptchav2,
 )
 
 
 @pytest.mark.xfail(raises=RecaptchaRateLimitError)
 def test_solver_with_normal_recaptcha() -> None:
     """Test the solver with a normal reCAPTCHA."""
     with sync_playwright() as playwright:
         browser = playwright.firefox.launch()
         page = browser.new_page()
-
-        page.goto(
-            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-        )
+        page.goto("https://www.google.com/recaptcha/api2/demo")
 
         with recaptchav2.SyncSolver(page) as solver:
-            solver.solve_recaptcha()
+            solver.solve_recaptcha(wait=True)
 
 
 @pytest.mark.xfail(raises=(RecaptchaNotFoundError, RecaptchaRateLimitError))
 def test_solver_with_hidden_recaptcha() -> None:
     """Test the solver with a hidden reCAPTCHA."""
     with sync_playwright() as playwright:
         browser = playwright.firefox.launch()
         page = browser.new_page()
 
-        page.goto(
-            "https://www.google.com/recaptcha/api2/demo?invisible=true",
-            wait_until="networkidle",
-        )
-
+        page.goto("https://www.google.com/recaptcha/api2/demo?invisible=true")
         page.get_by_role("button").click()
 
         with recaptchav2.SyncSolver(page) as solver:
-            solver.solve_recaptcha()
+            solver.solve_recaptcha(wait=True)
 
 
 @pytest.mark.xfail(raises=RecaptchaRateLimitError)
 def test_solver_with_slow_browser() -> None:
     """Test the solver with a slow browser."""
     with sync_playwright() as playwright:
         browser = playwright.firefox.launch(slow_mo=1000)
         page = browser.new_page()
+        page.goto("https://www.google.com/recaptcha/api2/demo")
+
+        with recaptchav2.SyncSolver(page) as solver:
+            solver.solve_recaptcha(wait=True)
 
-        page.goto(
-            "https://www.google.com/recaptcha/api2/demo", wait_until="networkidle"
-        )
+
+@pytest.mark.xfail(raises=CapSolverError)
+def test_solver_with_image_challenge() -> None:
+    """Test the solver with an image challenge."""
+    with sync_playwright() as playwright:
+        browser = playwright.firefox.launch()
+        page = browser.new_page()
+        page.goto("https://www.google.com/recaptcha/api2/demo")
 
         with recaptchav2.SyncSolver(page) as solver:
-            solver.solve_recaptcha()
+            solver.solve_recaptcha(wait=True, image_challenge=True)
 
 
 def test_recaptcha_not_found_error() -> None:
     """Test the solver with a page that does not have a reCAPTCHA."""
     with sync_playwright() as playwright:
         browser = playwright.firefox.launch()
         page = browser.new_page()
```

### Comparing `playwright-recaptcha-0.2.0/tests/test_sync_recaptchav3.py` & `playwright-recaptcha-0.3.0/tests/test_sync_recaptchav3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import pytest
 from playwright.sync_api import sync_playwright
 
-from playwright_recaptcha import (
-    RecaptchaTimeoutError,
-    recaptchav3,
-)
+from playwright_recaptcha import RecaptchaTimeoutError, recaptchav3
 
 
 def test_solver_with_normal_browser() -> None:
     """Test the solver with a normal browser."""
     with sync_playwright() as playwright:
         browser = playwright.firefox.launch()
         page = browser.new_page()
```

