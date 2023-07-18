# Comparing `tmp/sardine_system-0.2.1.tar.gz` & `tmp/sardine-system-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "sardine-system-0.4.0.tar", last modified: Tue Jul 18 22:59:10 2023, max compression
```

## Comparing `sardine_system-0.2.1.tar` & `sardine-system-0.4.0.tar`

### file list

```diff
@@ -1,81 +1,109 @@
--rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 sardine_system-0.2.1/fishery/UserConfig.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sardine_system-0.2.1/fishery/__init__.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 sardine_system-0.2.1/fishery/__main__.py
--rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 sardine_system-0.2.1/fishery/console.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 sardine_system-0.2.1/fishery/profiler.py
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 sardine_system-0.2.1/fishery/runners.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/__init__.py
--rw-r--r--   0        0        0    13526 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/fish_bowl.py
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/run.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/base/__init__.py
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/base/clock.py
--rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/base/handler.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/base/parser.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/base/runner.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/cli/README.md
--rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/cli/main.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/clock/__init__.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/clock/internal_clock.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/clock/link_clock.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/clock/time.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/event_loop/__init__.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/event_loop/loop.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/event_loop/mixin.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/event_loop/policy.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/event_loop/sansio.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/__init__.py
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/midi.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/midi_in.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/missile.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/osc.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/osc_in.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/osc_loop.py
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/player.py
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/sender.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/superdirt.py
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/sleep_handler/__init__.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/handlers/sleep_handler/time_handle.py
--rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/io/UserConfig.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/io/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/scheduler/__init__.py
--rw-r--r--   0        0        0    22455 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/scheduler/async_runner.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/scheduler/constants.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/scheduler/errors.py
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/scheduler/scheduler.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/__init__.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/chance.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/iterators.py
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/sequence.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/variables.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/sardine_parser/__init__.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/sardine_parser/chord.py
--rw-r--r--   0        0        0    17391 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/sardine_parser/funclib.py
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/sardine_parser/list_parser.py
--rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/sardine_parser/sardine.lark
--rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/sardine_parser/tree_calc.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/sardine_parser/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/ziffers_parser/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/ziffers_parser/ziffers.lark
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/ziffers_parser/ziffers_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/sequences/ziffers_parser/ziffers_tree.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/superdirt/__init__.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/superdirt/default_superdirt.scd
--rw-r--r--   0        0        0    10183 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/superdirt/process.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/utils/Messages.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 sardine_system-0.2.1/sardine/utils/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 sardine_system-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 sardine_system-0.2.1/tests/test_patterns.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 sardine_system-0.2.1/tests/test_utils.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 sardine_system-0.2.1/tests/fish_bowl/__init__.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 sardine_system-0.2.1/tests/fish_bowl/test_clock.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 sardine_system-0.2.1/tests/fish_bowl/test_hooks.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 sardine_system-0.2.1/tests/fish_bowl/test_sleep.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 sardine_system-0.2.1/tests/fish_bowl/test_transports.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sardine_system-0.2.1/tests/handlers/__init__.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 sardine_system-0.2.1/tests/handlers/test_child.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sardine_system-0.2.1/tests/handlers/test_osc.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 sardine_system-0.2.1/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 sardine_system-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 sardine_system-0.2.1/README.md
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 sardine_system-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 sardine_system-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.090012 sardine-system-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-18 22:58:57.000000 sardine-system-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 22:58:57.000000 sardine-system-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-18 22:59:10.090012 sardine-system-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-18 22:58:57.000000 sardine-system-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-18 22:58:57.000000 sardine-system-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.082012 sardine-system-0.4.0/sardine/
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.082012 sardine-system-0.4.0/sardine_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.082012 sardine-system-0.4.0/sardine_core/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/base/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/base/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/base/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/base/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.082012 sardine-system-0.4.0/sardine_core/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.082012 sardine-system-0.4.0/sardine_core/clock/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/clock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/clock/internal_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/clock/link_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/clock/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.082012 sardine-system-0.4.0/sardine_core/event_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/event_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/event_loop/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/event_loop/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/event_loop/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/event_loop/sansio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/fish_bowl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.086012 sardine-system-0.4.0/sardine_core/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/midi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/midi_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/missile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/osc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/osc_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/osc_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.086012 sardine-system-0.4.0/sardine_core/handlers/sleep_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/sleep_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/sleep_handler/time_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/handlers/superdirt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.086012 sardine-system-0.4.0/sardine_core/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/io/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.086012 sardine-system-0.4.0/sardine_core/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22624 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.086012 sardine-system-0.4.0/sardine_core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/scheduler/async_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/scheduler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/scheduler/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.086012 sardine-system-0.4.0/sardine_core/sequences/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/chance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/iterators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.086012 sardine-system-0.4.0/sardine_core/sequences/sardine_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/sardine_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/sardine_parser/chord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/sardine_parser/funclib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/sardine_parser/list_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/sardine_parser/sardine.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    23078 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/sardine_parser/tree_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/sardine_parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.090012 sardine-system-0.4.0/sardine_core/sequences/tidal_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/tidal_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/tidal_parser/control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.090012 sardine-system-0.4.0/sardine_core/sequences/tidal_parser/mini/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/tidal_parser/mini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/tidal_parser/mini/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/tidal_parser/mini/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39658 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/tidal_parser/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/tidal_parser/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/tidal_parser/tidal_euclid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/tidal_parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.090012 sardine-system-0.4.0/sardine_core/sequences/ziffers_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/ziffers_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/sequences/ziffers_parser/ziffers_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.090012 sardine-system-0.4.0/sardine_core/superdirt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/superdirt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/superdirt/default_superdirt.scd
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/superdirt/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.090012 sardine-system-0.4.0/sardine_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/utils/Messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-18 22:58:57.000000 sardine-system-0.4.0/sardine_core/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.090012 sardine-system-0.4.0/sardine_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-18 22:59:10.000000 sardine-system-0.4.0/sardine_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-18 22:59:10.000000 sardine-system-0.4.0/sardine_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:59:10.000000 sardine-system-0.4.0/sardine_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 22:59:10.000000 sardine-system-0.4.0/sardine_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-18 22:59:10.000000 sardine-system-0.4.0/sardine_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 22:59:10.000000 sardine-system-0.4.0/sardine_system.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 22:59:10.090012 sardine-system-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:59:10.090012 sardine-system-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-07-18 22:58:57.000000 sardine-system-0.4.0/tests/test_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 22:58:57.000000 sardine-system-0.4.0/tests/test_utils.py
```

### Comparing `sardine_system-0.2.1/fishery/UserConfig.py` & `sardine-system-0.4.0/sardine/UserConfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 
 TEMPLATE_CONFIGURATION = {
     "config": {
         "midi": None,
         "bpm": 125,
         "beats": 4,
         "parameters": [],
+        "parser": str,
         "superdirt_handler": True,
-        "boot_supercollider": False,
+        "boot_supercollider": True,
         "sardine_boot_file": True,
         "verbose_superdirt": False,
         "link_clock": False,
         "superdirt_config_path": str(USER_DIR / "default_superdirt.scd"),
         "user_config_path": str(USER_DIR / "user_configuration.py"),
         "deferred_scheduling": True,
+        "editor": False,
     }
 }
 
 
 def _recursive_update(dest: dict, src: dict):
     """Recursively updates the `dest` dictionary in-place using `src`."""
     for k, vsrc in src.items():
@@ -47,56 +49,62 @@
 
 @dataclass
 class Config:
     midi: Union[str, None]
     beats: int
     parameters: list
     bpm: int
+    parser: str
     superdirt_config_path: str
     verbose_superdirt: bool
     user_config_path: str
     boot_supercollider: bool
     superdirt_handler: bool
     sardine_boot_file: bool
     link_clock: bool
     deferred_scheduling: bool
+    editor: bool
 
     @classmethod
     def from_dict(cls, data: dict) -> "Config":
         config = data["config"]
         return cls(
             midi=config["midi"],
             beats=config["beats"],
             parameters=config["parameters"],
             bpm=config["bpm"],
+            parser=config["parser"],
             superdirt_handler=config["superdirt_handler"],
             boot_supercollider=config["boot_supercollider"],
             sardine_boot_file=config["sardine_boot_file"],
             verbose_superdirt=config["verbose_superdirt"],
             link_clock=config["link_clock"],
             superdirt_config_path=config["superdirt_config_path"],
             user_config_path=config["user_config_path"],
             deferred_scheduling=config["deferred_scheduling"],
+            editor=config["editor"],
         )
 
     def to_dict(self) -> dict:
         return {
             "config": {
                 "midi": self.midi,
                 "beats": self.beats,
                 "parameters": self.parameters,
                 "bpm": self.bpm,
+                "parser": self.parser,
                 "superdirt_handler": self.superdirt_handler,
                 "boot_supercollider": self.boot_supercollider,
                 "sardine_boot_file": self.sardine_boot_file,
                 "verbose_superdirt": self.verbose_superdirt,
                 "superdirt_config_path": self.superdirt_config_path,
                 "link_clock": self.link_clock,
                 "user_config_path": self.user_config_path,
                 "deferred_scheduling": self.deferred_scheduling,
+                "editor": self.editor,
             }
         }
 
 
 def write_configuration_file(config: Config, file_path: Path):
     """Write config JSON file"""
     with open(file_path, "w") as file:
```

### Comparing `sardine_system-0.2.1/fishery/console.py` & `sardine-system-0.4.0/sardine/console.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,36 @@
 # https://github.com/python/cpython/blob/main/Lib/asyncio/__main__.py
 # Taken from the CPython Github Repository. Custom version of the
 # asyncio REPL that will autoload Sardine whenever started.
 
-import ast
-import asyncio
-import code
 import concurrent.futures
-import inspect
-
-# import os
-# import platform
 import threading
-import types
 import warnings
-from asyncio import futures
-from pathlib import Path
-from typing import Optional
+import inspect
+import asyncio
+import types
+import code
+import ast
 
-# import psutil
 from appdirs import user_data_dir
-from rich import print as pretty_print
-from rich.panel import Panel
-
-import sardine
-
+from typing import Optional
+from asyncio import futures
 from .runners import Runner
+from pathlib import Path
 
-# system = platform.system()
-# # Setting very high priority for this process (time-critical)
-# warning_text = "[yellow]/!\\\\[/yellow] [red bold]  Run Sardine faster by starting it using\
-# \nadministrator priviledges (sudo on Unix..)[/red bold] [yellow]/!\\\\[/yellow]"
-# if system == "Windows":
-#     try:
-#         p = psutil.Process(os.getpid())
-#         p.nice(psutil.HIGH_PRIORITY_CLASS)
-#     except psutil.AccessDenied:
-#         pretty_print(Panel.fit(warning_text))
-#         pass
-# else:
-#     try:
-#         p = psutil.Process(os.getpid())
-#         p.nice(-20)
-#     except psutil.AccessDenied:
-#         pretty_print(Panel.fit(warning_text))
-#         pass
-
+import sardine_core
 
 # Appdirs boilerplate
 APP_NAME, APP_AUTHOR = "Sardine", "Bubobubobubo"
 USER_DIR = Path(user_data_dir(APP_NAME, APP_AUTHOR))
+LOG_FILE = USER_DIR / "sardine.log"
+
+# The file needs to exist to actually log something
+if not LOG_FILE.exists():
+    LOG_FILE.touch()
 
 
 class AsyncIOInteractiveConsole(code.InteractiveConsole):
     def __init__(self, locals: dict, loop: asyncio.BaseEventLoop):
         super().__init__(locals)
         self.compile.compiler.flags |= ast.PyCF_ALLOW_TOP_LEVEL_AWAIT
 
@@ -109,59 +87,61 @@
         self.console = console
 
     def run(self):
         try:
             banner = ()
             self.console.push("""import os""")
             self.console.push("""os.environ['SARDINE_INIT_SESSION'] = 'YES'""")
-            self.console.push("""from sardine.run import *""")
+            self.console.push("""from sardine_core.run import *""")
             self.console.interact(banner=banner, exitmsg="exiting asyncio REPL...")
         finally:
             warnings.filterwarnings(
                 "ignore",
                 message=r"^coroutine .* was never awaited$",
                 category=RuntimeWarning,
             )
 
 
 async def run_forever():
     loop = asyncio.get_running_loop()
     await loop.create_future()
 
 
-def start():
-    loop = sardine.event_loop.new_event_loop()
+class ConsoleManager:
+    def __init__(self):
+        self.loop = sardine_core.event_loop.new_event_loop()
+
+        repl_locals = {"asyncio": asyncio}
+        for key in (
+            "__name__",
+            "__package__",
+            "__loader__",
+            "__spec__",
+            "__builtins__",
+            "__file__",
+        ):
+            repl_locals[key] = globals()[key]
 
-    repl_locals = {"asyncio": asyncio}
-    for key in (
-        "__name__",
-        "__package__",
-        "__loader__",
-        "__spec__",
-        "__builtins__",
-        "__file__",
-    ):
-        repl_locals[key] = globals()[key]
-
-    console = AsyncIOInteractiveConsole(repl_locals, loop)
-
-    try:
-        import readline  # NoQA
-    except ImportError:
-        pass
-
-    repl_thread = REPLThread(console=console)
-    repl_thread.daemon = True
-    repl_thread.start()
-
-    with Runner(loop=loop) as runner:
-        while True:
-            try:
-                runner.run(run_forever())
-            except KeyboardInterrupt:
-                if console.repl_future and not console.repl_future.done():
-                    console.repl_future.cancel()
-                    console.repl_future_interrupted = True
+        self.console = AsyncIOInteractiveConsole(repl_locals, self.loop)
+
+    def start(self):
+        try:
+            import readline  # NoQA
+        except ImportError:
+            pass
+
+        repl_thread = REPLThread(console=self.console)
+        repl_thread.daemon = True
+        repl_thread.start()
+
+        with Runner(loop=self.loop) as runner:
+            while True:
+                try:
+                    runner.run(run_forever())
+                except KeyboardInterrupt:
+                    if self.console.repl_future and not self.console.repl_future.done():
+                        self.console.repl_future.cancel()
+                        self.console.repl_future_interrupted = True
+                    else:
+                        break
                 else:
                     break
-            else:
-                break
```

### Comparing `sardine_system-0.2.1/fishery/runners.py` & `sardine-system-0.4.0/sardine/runners.py`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/fish_bowl.py` & `sardine-system-0.4.0/sardine_core/fish_bowl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import asyncio
 import collections
-from typing import Hashable, Iterable, Optional, Protocol, Union
-
-from exceptiongroup import BaseExceptionGroup
 
+from typing import Hashable, Iterable, Optional, Protocol, Union
+from .sequences import Iterator, ListParser, Variables
 from .base import BaseClock, BaseHandler, BaseParser
+from exceptiongroup import BaseExceptionGroup
 from .clock import InternalClock, Time
 from .handlers import SleepHandler
 from .scheduler import Scheduler
-from .sequences import Iterator, ListParser, Variables
 
 __all__ = ("FishBowl",)
 
 
 class HookProtocol(Hashable, Protocol):
     """A callable object that accepts an event and any number of arguments."""
 
@@ -40,14 +39,15 @@
         self.sleeper = sleeper or SleepHandler()
         self.time = time or Time()
         self.variables = variables or Variables()
 
         self._handlers: dict[BaseHandler, None] = {}
         self._alive = asyncio.Event()
         self._resumed = asyncio.Event()
+        self._vortex_subscribers: list = []
 
         self._event_hooks: dict[
             Optional[str], dict[HookProtocol, None]
         ] = collections.defaultdict(dict)
         # Reverse mapping for easier removal of hooks
         self._hook_events: dict[
             HookProtocol, dict[Optional[str], None]
@@ -169,14 +169,18 @@
     async def sleep(self, duration: Union[int, float]):
         """Sleeps for the given duration.
 
         This method is simply a shorthand for `self.sleeper.sleep(duration)`.
         """
         return await self.sleeper.sleep(duration)
 
+    async def sleep_beats(self, beats: Union[int, float]):
+        """Sleeps for the given number of beats."""
+        return await self.sleep(beats * self.clock.beat_duration)
+
     # Hot-swap methods ############################################################
 
     def swap_clock(self, clock: "BaseClock"):
         """Hot-swap the current clock for a different clock.
 
         This method will perform the following procedure:
             1. Pause the fish bowl
@@ -188,14 +192,20 @@
         self.pause()
         self.remove_handler(self.clock)
         self.clock = clock
         self.add_handler(clock)
         self.resume()
         self.dispatch("clock_swap", clock)
 
+    def swap_parser(self, parser: "BaseParser"):
+        """Hot-swap the current parser for a different one (eg. base -> ziffers)."""
+        self.remove_handler(self.parser)
+        self.add_handler(parser)
+        self.dispatch("parser_swap", parser)
+
     ## HANDLERS ############################################################
 
     def add_handler(self, handler: "BaseHandler"):
         """Adds a new handler to the fish bowl.
 
         If the handler has any child handlers, they will be
         recursively added to the fish bowl as well.
@@ -215,24 +225,25 @@
             ValueError:
                 The handler is either already added to a different fish bowl
                 or the handler's parent was not yet added to this fish bowl.
         """
         if handler.env is not None:
             if handler.env is self:
                 return
-            raise ValueError(f"{handler!r} was already added to {handler.env!r}")
+            message = f"{handler!r} was already added to {handler.env!r}"
+            raise ValueError(message)
         elif handler.parent is not None and handler.parent.env is not self:
             if handler.parent.env is None:
-                raise ValueError(
+                parent_message = (
                     f"The parent {handler.parent!r} must be added to the fish bowl"
                 )
+                raise ValueError(parent_message)
             else:
-                raise ValueError(
-                    f"The parent {handler.parent!r} was already added to {handler.env!r}"
-                )
+                parent_message_alt = f"The parent {handler.parent!r} was already added to {handler.env!r}"
+                raise ValueError(parent_message_alt)
 
         # It may be possible that the user set `env` to None, but
         # given that `register_hook()` is idempotent, it's probably
         # fine to call `BaseHandler.setup()` again
 
         handler._env = self  # pylint: disable=protected-access
         self._handlers[handler] = None
```

### Comparing `sardine_system-0.2.1/sardine/base/clock.py` & `sardine-system-0.4.0/sardine_core/base/clock.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,23 @@
         This should setup any external time source, assign the current
         time to `internal_origin`, and then continuously
         update the `internal_time`.
         """
 
     @property
     @abstractmethod
+    def tick(self) -> int:
+        """The tick of the clock's.
+
+        This property is used by the Tidal Scheduler in the lookahead
+        mechanism that queries and schedules patterns in advance.
+        """
+
+    @property
+    @abstractmethod
     def bar(self) -> int:
         """The bar of the clock's current time.
 
         This property should account for time shift, but it is not expected
         to be consistent across clocks or after any updates to the tempo.
         """
 
@@ -213,17 +222,17 @@
             return interval
 
         duration = interval - time % interval
 
         # Due to potential rounding errors, we might get a duration
         # that should be, but isn't actually equal to the interval.
         # To mitigate this, we will replace any durations below 10
-        # microseconds.
+        # nanoseconds.
         # Rounding errors will worsen over time, but it is unlikely
-        # we'll get to a point where 10 microseconds is too little
+        # we'll get to a point where 10 nanoseconds is too little
         # (but possible if sardine goes on for 5-6 years).
         if math.isclose(duration, 0.0, rel_tol=0.0, abs_tol=1e-8):
             return interval
 
         return duration
 
     def get_bar_time(
```

### Comparing `sardine_system-0.2.1/sardine/base/handler.py` & `sardine-system-0.4.0/sardine_core/base/handler.py`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/base/runner.py` & `sardine-system-0.4.0/sardine_core/base/runner.py`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/cli/main.py` & `sardine-system-0.4.0/sardine_core/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-import json
-from itertools import chain
+from ..io.UserConfig import create_template_configuration_file
+from InquirerPy.validator import EmptyInputValidator
+from InquirerPy.base.control import Choice
+from InquirerPy import inquirer
+from rich.panel import Panel
 from pathlib import Path
-
+from ..logger import print
+from appdirs import *  # Wildcard used in docs
 import click
+import json
 import mido
 
-# Wildcard used in docs..
-from appdirs import *
-from InquirerPy import inquirer, prompt
-from InquirerPy.base.control import Choice
-from InquirerPy.validator import EmptyInputValidator
-from rich import print
-from rich.panel import Panel
-
-from ..io.UserConfig import create_template_configuration_file
 
 FUNNY_TEXT = """
 ░█████╗░░█████╗░███╗░░██╗███████╗██╗░██████╗░
 ██╔══██╗██╔══██╗████╗░██║██╔════╝██║██╔════╝░
 ██║░░╚═╝██║░░██║██╔██╗██║█████╗░░██║██║░░██╗░
 ██║░░██╗██║░░██║██║╚████║██╔══╝░░██║██║░░╚██╗
 ╚█████╔╝╚█████╔╝██║░╚███║██║░░░░░██║╚██████╔╝
 ░╚════╝░░╚════╝░╚═╝░░╚══╝╚═╝░░░░░╚═╝░╚═════╝░
 
- This is the configuration tool for Sardine
+ This is the configuration tool for Sardine.
+ This tool can configure the default session.
+ Use it wisely, discover all the options!
 """
 
 # Appdirs boilerplate code
 APP_NAME, APP_AUTHOR = "Sardine", "Bubobubobubo"
 USER_DIR = Path(user_data_dir(APP_NAME, APP_AUTHOR))
 CONFIG_JSON = USER_DIR / "config.json"
 
@@ -79,14 +77,17 @@
     - Manual selection (using mido for autocompletion)
     - Automatic selection (select Sardine port)
     - Custom port (write it at the command line)
     """
 
     choices = ["Automatic", "Manual", "Custom (advanced)"]
     midi_ports = mido.get_output_names()
+    if sys.platform == "win32":
+        for i, port in enumerate(midi_ports):
+            midi_ports[i] = " ".join(port.split(" ")[:-1])
     print(
         Panel.fit(
             f"[red]Current MIDI Output: [green]{config_file['midi']}[/green][/red]"
         )
     )
     menu_select = inquirer.select(
         message="Select a method for choosing output port:", choices=choices
@@ -279,59 +280,57 @@
     TUI and CLI. Simple contextual menu that allows the user to change values in
     the JSON file without the need of writing too much. It is based on a very
     primitive while loop that ends when the user is done editing to its liking.
 
     Just like before, we are building a monolothic configuration dict that we
     inject into the current config.json file. Not fancy but cool nonetheless!
     """
+
     MENU_CHOICES = [
         "Show Config",
         "Reset",
         "MIDI",
         "Clock",
         "SuperCollider",
         "More",
         "Exit",
     ]
+
     try:
         USER_CONFIG = read_json_file()["config"]
     except FileNotFoundError as e:
         print(
             "[bold red]No Sardine Configuration found. Please boot Sardine first![/bold red]"
         )
         exit()
+
+    # This panel can stay because it is a splashscreen
     print(Panel.fit("[red]" + FUNNY_TEXT + "[/red]"))
+
     while True:
         menu_select = inquirer.select(
             message="Select an option", choices=MENU_CHOICES
         ).execute()
+
         if menu_select == "Exit":
             write_to_file = inquirer.confirm(
-                message="Do you wish to save the current config file?"
+                message="Do you wish to save and exit?"
             ).execute()
             if write_to_file:
                 try:
                     write_json_file({"config": USER_CONFIG})
+                    exit()
                 except Exception:
                     raise SystemError("Couldn't write config file!")
-            exit_from_conf = inquirer.confirm(message="Do you wish to exit?").execute()
-            if exit_from_conf:
-                exit()
-            else:
-                continue
         elif menu_select == "Reset":
             create_template_configuration_file(CONFIG_JSON)
             USER_CONFIG = read_json_file()["config"]
         elif menu_select == "Show Config":
             print(USER_CONFIG)
         elif menu_select == "MIDI":
             USER_CONFIG = _select_midi_output(config_file=USER_CONFIG)
         elif menu_select == "Clock":
             USER_CONFIG = _select_bpm_and_timing(config_file=USER_CONFIG)
         elif menu_select == "SuperCollider":
             USER_CONFIG = _select_supercollider_settings(config_file=USER_CONFIG)
         elif menu_select == "More":
             USER_CONFIG = _select_additional_options(config_file=USER_CONFIG)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `sardine_system-0.2.1/sardine/clock/time.py` & `sardine-system-0.4.0/sardine_core/clock/time.py`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/event_loop/__init__.py` & `sardine-system-0.4.0/sardine_core/event_loop/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,19 +33,21 @@
     return True
 
 
 def _install_uvloop() -> bool:
     try:
         import uvloop
     except ImportError:
-        rich.print("[green]uvloop[/green] [yellow]is not installed")
+        # Commenting this line: it scares new users!
+        # rich.print("[green]uvloop[/green] [yellow]is not installed")
         return False
 
     asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
-    rich.print("[yellow]Installed uvloop event loop")
+    # I don't think that this information is necessary anymore for users
+    # rich.print("[yellow]Installed uvloop event loop")
     return True
 
 
 def install_policy():
     """Installs the best-available event loop policy into asyncio.
 
     This method must be called before any event loop is created, otherwise
@@ -61,15 +63,16 @@
     for func in methods:
         successful = func()
         if successful:
             break
 
     if not successful:
         rich.print(
-            "[yellow]No custom event loop applied; rhythm accuracy may be impacted"
+            "[yellow]Warning: No custom event loop applied; rhythm accuracy may be impacted."
+            "[yellow]Windows users, ignore this warning!"
         )
 
 
 def new_event_loop() -> asyncio.BaseEventLoop:
     """Creates the best-available event loop without permanently installing
     a new policy for asyncio.
     """
```

### Comparing `sardine_system-0.2.1/sardine/event_loop/loop.py` & `sardine-system-0.4.0/sardine_core/event_loop/loop.py`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/event_loop/policy.py` & `sardine-system-0.4.0/sardine_core/event_loop/policy.py`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/event_loop/sansio.py` & `sardine-system-0.4.0/sardine_core/event_loop/sansio.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import threading
 from typing import Optional
 
 __all__ = ("SansIOEventLoop", "SansSelector")
 
 
 class SansSelector:
-
     _event_list = []
 
     def __init__(self, wake_cond: threading.Condition):
         self._wake_cond = wake_cond
 
     def select(self, timeout: Optional[int]):
         timeout = timeout or 0.0
```

### Comparing `sardine_system-0.2.1/sardine/handlers/midi_in.py` & `sardine-system-0.4.0/sardine_core/handlers/midi_in.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,107 @@
 from collections import deque
 from dataclasses import dataclass
 from typing import Optional, Union
+import sys
 
 import mido
 from mido import Message, get_input_names, open_input, parse_string_stream
-from rich import print
+from ..logger import print
 
 from ..base.handler import BaseHandler
 
-__all__ = ("MidiInHandler", "ControlTarget", "NoteTarget")
+__all__ = ("MidiInHandler",)
 
 
-@dataclass
-class ControlTarget:
-    control: int
-    channel: int
-
-
-@dataclass
-class NoteTarget:
-    channel: int
+def find_midi_in_port(name: str) -> Optional[str]:
+    """Find the port name of a MIDI-In port by name."""
+    for port in mido.get_input_names():
+        port_without_number = port
+        if sys.platform == "win32":
+            port_without_number = " ".join(port.split(" ")[:-1])
+        if name == port_without_number:
+            return port
+    return None
 
 
 class MidiInHandler(BaseHandler):
     """
     MIDI-In Listener: listen to incoming MIDI events from a selected port.
     Useful for mapping controllers to control / interact with Sardine.
+
+    The incoming messages are stored in a queue and retrieved in FIFO order.
     """
 
-    def __init__(
-        self,
-        target: Union[ControlTarget, NoteTarget, None] = None,
-        port: Optional[str] = None,
-    ):
+    def __init__(self, port_name: Optional[str] = None):
         super().__init__()
-        self.target = target
-        self.queue = deque(maxlen=20)
-        self._last_item: Optional[Message] = None
+        self.queues = {}
+        self._last_item = {}
         self._last_value = 0
 
-        if port:
+        if port_name:
+            port_name = find_midi_in_port(port_name)
             try:
-                self._input = open_input(port)
+                self._input = open_input(port_name)
                 self._input.callback = self._callback
             except Exception:
-                raise OSError(f"Couldn't listen on port {port}")
+                error_message = f"Couldn't listen on port {port_name}"
+                raise OSError(error_message)
         else:
             try:
                 self._input = open_input()
                 self._input.callback = self._callback
                 listened_port = mido.get_input_names()[0]
             except Exception:
-                raise OSError(f"Couldn't listen on port {port}")
+                raise OSError(f"Couldn't listen on port {listened_port}")
 
     def __str__(self):
         """String representation of the MIDI Listener"""
-        return f"<MidiListener: {self._input} target={self.target}>"
-
-    def _callback(self, message):
-        """Callback for MidiListener Port"""
-        # Add more filters
-        if message:
-            self.queue.append(message)
+        return f"<MidiListener: {self._input}>"
 
-    def _get_control(self, control: int, channel: int) -> None:
-        """Get a specific control change"""
-        if self.queue:
-            message = self.queue.pop()
-            if (
-                message.type == "control_change"
-                and message.control == control
-                and message.channel == channel
-            ):
-                self._last_item = message
+    def _get_index_for_control_change(self, control: int, channel: int):
+        """Generate a new dictionnary key for each control change route"""
+        return f"ctrl:{control},{channel}"
+
+    def _get_index_for_note(self, channel: int):
+        """Generate a new dictionnary key for each channel"""
+        return f"note:{channel}"
+
+    def _callback(self, message) -> None:
+        """Callback for MidiListener Port."""
+
+        def _push_message_to_dict(index: str, message: mido.Message) -> None:
+            if index in self.queues:
+                self.queues[index].appendleft(message)
             else:
-                self._last_item = self._last_item
+                self.queues[index] = deque(maxlen=20)
+                self.queues[index].appendleft(message)
 
-    def _get_note(self, channel: int) -> None:
-        """Get notes from a specific MIDI channel"""
-        if self.queue:
-            message = self.queue.pop()
-            if message.channel == channel:
-                self._last_item = message
+        if message:
+            # Case where the message is a control change
+            if hasattr(message, "control"):
+                queue_dictionnary_index = self._get_index_for_control_change(
+                    control=message.control,
+                    channel=message.channel,
+                )
+                if not message.type == "control_change":
+                    return
+                else:
+                    _push_message_to_dict(queue_dictionnary_index, message)
+                return
+            # Case where the message is a note
+            elif hasattr(message, "note"):
+                queue_dictionnary_index = self._get_index_for_note(message.channel)
+                if not message.type in ("note_off", "note_in"):
+                    return
+                else:
+                    _push_message_to_dict(queue_dictionnary_index, message)
+                return
             else:
-                self._last_item = self._last_item
+                # Case where the message is just garbage to dispose of
+                return
 
     def _extract_value(self, message: Union[mido.Message, None]) -> Union[Message, int]:
         """
         Given a mido.Message, extract needed value based on message type
         """
 
         if message is None:
@@ -98,29 +112,45 @@
             value = message.value
         elif mtype in ["note_on", "note_off"]:
             value = message.note
         else:
             return message
         return value
 
-    def get(self):
-        """Get an item from the MidiListener"""
-        target = self.target
-
-        if isinstance(target, ControlTarget):
-            self._get_control(channel=target.channel, control=target.control)
-        elif isinstance(target, NoteTarget):
-            self._get_note(channel=target.channel)
+    def _get(self, control: Optional[int], channel: int, last: bool = False):
+        """Get an item from the MidiListener event dictionnary. IF last is True,
+        return the last element that was inserted and clear the queue. If Control
+        is None, then it must be a note"""
+        if control:
+            idx = self._get_index_for_control_change(control, channel)
         else:
-            if self.queue:
-                self._last_item = self.queue.pop()
+            idx = self._get_index_for_note()
+        try:
+            queue = self.queues[idx]
+        except KeyError:
+            return 0
+
+        if queue:
+            if last:
+                self._last_item[idx] = queue.popleft()
+                queue.clear()
             else:
-                self._last_item = self._last_item
+                self._last_item[idx] = queue.pop()
+
+        return self._extract_value(self._last_item[idx])
 
-        return self._extract_value(self._last_item)
+    def get_control(self, channel: int, control: int, last: bool = False):
+        """Get a control change from the MidiListener event dictionnary. If last
+        is True, return the last element that was inserted and clear the queue."""
+        return self._get(control=control, channel=channel, last=last)
+
+    def get_note(self, channel: int, last: bool = False):
+        """Get a note from the MidiListener event dictionnary. If last
+        is True, return the last element that was inserted and clear the queue."""
+        return self._get(channel=channel, last=last)
 
-    def inspect_queue(self):
-        print(f"{self.queue}")
+    def inspect_queues(self):
+        print(f"{self.queues}")
 
     def kill(self):
         """Close the MIDIListener"""
         self._input.close()
```

### Comparing `sardine_system-0.2.1/sardine/handlers/missile.py` & `sardine-system-0.4.0/sardine_core/handlers/missile.py`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/handlers/osc.py` & `sardine-system-0.4.0/sardine_core/handlers/osc.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,52 +26,75 @@
         self.loop = loop
 
         # Setting up OSC Connexion
         self._ip, self._port, self._name = (ip, port, name)
         self._ahead_amount = ahead_amount
         self.client = osc_udp_client(address=self._ip, port=self._port, name=self._name)
         self._events = {"send": self._send}
+        self._defaults: dict = {}
 
         loop.add_child(self, setup=True)
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__} {self._name} ip={self._ip!r} port={self._port}>"
 
     def setup(self):
         for event in self._events:
             self.env.register_hook(event, self)
 
     def hook(self, event: str, *args):
         func = self._events[event]
         func(*args)
 
+    # Global parameters
+    @property
+    def defaults(self):
+        return self._defaults
+
     def _send(self, address: str, message: list) -> None:
         msg = oscbuildparse.OSCMessage(address, None, message)
         bun = oscbuildparse.OSCBundle(
             oscbuildparse.unixtime2timetag(time.time() + self._ahead_amount),
             [msg],
         )
         osc_send(bun, self._name)
 
+    def send_raw(self, address: str, message: list) -> None:
+        """
+        Public alias for the _send function. It can sometimes be useful to have it
+        when we do want to write some raw OSC message without formatting it in the
+        expected SuperDirt format.
+        """
+        self._send(address, message)
+
     @alias_param(name="iterator", alias="i")
     @alias_param(name="divisor", alias="d")
     @alias_param(name="rate", alias="r")
+    @alias_param(name="sorted", alias="s")
     def send(
         self,
         address: Optional[StringElement],
         iterator: Number = 0,
         divisor: NumericElement = 1,
         rate: NumericElement = 1,
+        sort: bool = True,
         **pattern: NumericElement,
     ) -> None:
-
         if address is None:
             return
 
+        if self.apply_conditional_mask_to_bars(
+            pattern=pattern,
+        ):
+            return
+
         pattern["address"] = address
         deadline = self.env.clock.shifted_time
         for message in self.pattern_reduce(pattern, iterator, divisor, rate):
             if message["address"] is None:
                 continue
             address = message.pop("address")
-            serialized = list(chain(*sorted(message.items())))
+            if sort:
+                serialized = list(chain(*sorted(message.items())))
+            else:
+                serialized = list(chain(*message.items()))
             self.call_timed(deadline, self._send, f"/{address}", serialized)
```

### Comparing `sardine_system-0.2.1/sardine/handlers/osc_in.py` & `sardine-system-0.4.0/sardine_core/handlers/osc_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Callable, Optional, Union
 
 from osc4py3.as_eventloop import *
 from osc4py3.oscchannel import TransportChannel, get_channel
 from osc4py3.oscmethod import *
-from rich import print
+from ..logger import print
 
 from ..base.handler import BaseHandler
 from .osc_loop import OSCLoop
 
 __all__ = ("OSCInHandler",)
```

### Comparing `sardine_system-0.2.1/sardine/handlers/sleep_handler/__init__.py` & `sardine-system-0.4.0/sardine_core/handlers/sleep_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/handlers/sleep_handler/time_handle.py` & `sardine-system-0.4.0/sardine_core/handlers/sleep_handler/time_handle.py`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/io/UserConfig.py` & `sardine-system-0.4.0/sardine_core/io/UserConfig.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Union
 
 from appdirs import *
-from rich import print
+from ..logger import print
 
 __all__ = (
     "Config",
     "create_template_configuration_file",
     "read_configuration_file",
     "read_user_configuration",
     "pretty_print_configuration_file",
@@ -19,23 +19,26 @@
 
 TEMPLATE_CONFIGURATION = {
     "config": {
         "midi": "Sardine",
         "bpm": 135,
         "beats": 4,
         "debug": False,
-        "superdirt_handler": False,
+        "parser": "sardine",
+        "superdirt_handler": True,
         "sardine_boot_file": True,
-        "boot_supercollider": False,
+        "boot_supercollider": True,
         "verbose_superdirt": False,
         "link_clock": False,
         "superdirt_config_path": str(USER_DIR / "default_superdirt.scd"),
         "user_config_path": str(USER_DIR / "user_configuration.py"),
         "deferred_scheduling": True,
-    }
+        "editor": False,
+    },
+    "extensions": [],
 }
 
 
 def _recursive_update(dest: dict, src: dict):
     """Recursively updates the `dest` dictionary in-place using `src`."""
     for k, vsrc in src.items():
         vdest = dest.get(k)
@@ -47,57 +50,66 @@
 
 @dataclass
 class Config:
     midi: Union[str, None]
     beats: int
     bpm: int
     debug: bool
+    parser: str
     superdirt_config_path: str
     verbose_superdirt: bool
     user_config_path: str
     superdirt_handler: bool
     boot_supercollider: bool
     sardine_boot_file: bool
     link_clock: bool
     deferred_scheduling: bool
+    editor: bool
+    extensions: list
 
     @classmethod
     def from_dict(cls, data: dict) -> "Config":
         config = data["config"]
         return cls(
             midi=config["midi"],
             beats=config["beats"],
             debug=config["debug"],
             bpm=config["bpm"],
+            parser=config["parser"],
             superdirt_handler=config["superdirt_handler"],
             boot_supercollider=config["boot_supercollider"],
             sardine_boot_file=config["sardine_boot_file"],
             verbose_superdirt=config["verbose_superdirt"],
             link_clock=config["link_clock"],
             superdirt_config_path=config["superdirt_config_path"],
             user_config_path=config["user_config_path"],
             deferred_scheduling=config["deferred_scheduling"],
+            editor=config["editor"],
+            extensions=data["extensions"],
         )
 
     def to_dict(self) -> dict:
         return {
             "config": {
                 "midi": self.midi,
                 "beats": self.beats,
                 "debug": self.debug,
                 "bpm": self.bpm,
+                "parser": self.parser,
                 "superdirt_handler": self.superdirt_handler,
                 "boot_supercollider": self.boot_supercollider,
                 "sardine_boot_file": self.sardine_boot_file,
                 "verbose_superdirt": self.verbose_superdirt,
                 "superdirt_config_path": self.superdirt_config_path,
                 "link_clock": self.link_clock,
                 "user_config_path": self.user_config_path,
                 "deferred_scheduling": self.deferred_scheduling,
-            }
+                "editor": self.editor,
+            },
+            "extensions": self.extensions,
         }
 
 
 def write_configuration_file(config: Config, file_path: Path):
     """Write config JSON file"""
     with open(file_path, "w") as file:
         json.dump(config.to_dict(), file, indent=4, sort_keys=True)
@@ -142,15 +154,31 @@
             config = read_configuration_file(config_file)
         else:
             config = create_template_configuration_file(config_file)
     # If the configuration folder doesn't exist, create it and create config
     else:
         USER_DIR.mkdir(parents=True)
         config = create_template_configuration_file(config_file)
+
+        # Creating console file for the web editor
+        Path(USER_DIR / "console.log").touch(exist_ok=True)
+
+        # Create the buffers for the web editor
+        Path(USER_DIR / "buffers").mkdir(parents=True)
+        for number in list(range(0, 10)):
+            Path(USER_DIR / "buffers" / f"{number}.py").touch(exist_ok=True)
+
     return config
 
 
+def read_extension_configuration(file_path: str) -> dict:
+    """Read extension config JSON file."""
+    with open(file_path, "r") as f:
+        ext_data = json.load(f)
+    return ext_data
+
+
 if __name__ == "__main__":
     try:
         config = read_user_configuration()
     except FileNotFoundError as e:
         raise FileNotFoundError("No Sardine Config found. Please start Sardine first")
```

### Comparing `sardine_system-0.2.1/sardine/scheduler/async_runner.py` & `sardine-system-0.4.0/sardine_core/scheduler/async_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 import asyncio
 import heapq
 import inspect
+import math
 import traceback
 from collections import deque
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, MutableSequence, NamedTuple, Optional, Union
-
-from rich import print
-from rich.panel import Panel
+from ..logger import print
 
 from ..base import BaseClock
 from ..clock import Time
 from ..utils import MISSING, maybe_coro
 from .constants import MaybeCoroFunc
 from .errors import *
 
 if TYPE_CHECKING:
     from ..fish_bowl import FishBowl
     from .scheduler import Scheduler
 
 __all__ = ("AsyncRunner", "FunctionState")
 
 
-def print_panel(text: str) -> None:
-    """
-    Print swimming function event inside a Rich based Panel.
-    The box is automatically resized to fit text length.
-    """
-    print("\n", Panel.fit(text), end="")
-
-
 def _assert_function_signature(sig: inspect.Signature, args, kwargs):
     if args:
         message = "Positional arguments cannot be used in scheduling"
         if missing := _missing_kwargs(sig, args, kwargs):
             message += "; perhaps you meant `{}`?".format(
                 ", ".join(f"{k}={v!r}" for k, v in missing.items())
             )
@@ -124,14 +115,20 @@
     """
 
     MAX_FUNCTION_STATES = 3
 
     name: str
     """Uniquely identifies a runner when it is added to a scheduler."""
 
+    background_job: bool
+    """Determines if the asyncrunner should be running the background
+    and never be interrupted by silence(), panic() or any manual stop
+    function.
+    """
+
     scheduler: "Optional[Scheduler]"
     """The scheduler this runner was added to."""
     states: MutableSequence[FunctionState]
     """
     The function stack, used for auto-restoring functions.
 
     This is implemented with a deque to ensure a limit on how many functions
@@ -190,37 +187,38 @@
     _has_reverted: bool
 
     _deferred_state_index: int
 
     _can_correct_interval: bool
     _expected_time: float
     _last_interval: float
-    _last_iteration_called: bool
+    _last_expected_time: float
     _last_state: Optional[FunctionState]
 
     def __init__(self, name: str):
         self.name = name
         self.scheduler = None
         self.states = deque(maxlen=self.MAX_FUNCTION_STATES)
         self.deferred_states = []
         self.interval_shift = 0.0
         self.snap = None
+        self.background_job = False
 
         self._swimming = False
         self._stop = False
         self._task = None
         self._reload_event = asyncio.Event()
         self._has_reverted = False
 
         self._deferred_state_index = 0
 
         self._can_correct_interval = False
         self._expected_time = 0.0
         self._last_interval = 0.0
-        self._last_iteration_called = False
+        self._last_expected_time = -math.inf
         self._last_state = None
 
     def __repr__(self):
         cls_name = type(self).__name__
         status = "running" if self.is_running() else "stopped"
         attrs = " ".join(
             f"{attr}={getattr(self, attr)!r}"
@@ -278,19 +276,18 @@
             raise BadFunctionError(f"Expected a callable, got {func!r}")
         elif not self.states:
             state = FunctionState(func, args, kwargs)
             return self.states.append(state)
 
         last_state = self.states[-1]
 
-        # Transfer arguments from last state if possible
-        # (`_runner()` will discard excess arguments later)
-        args = args + last_state.args[len(args) :]
-        kwargs = last_state.kwargs | kwargs
-        self.states.append(FunctionState(func, args, kwargs))
+        new_state = FunctionState(func, args, kwargs)
+        self._merge_states(last_state, new_state)
+
+        self.states.append(new_state)
 
     def push_deferred(
         self, deadline: Union[float, int], func: "MaybeCoroFunc", *args, **kwargs
     ):
         """Adds a function to a queue to eventually be run.
 
         It is recommended to reload the runner after this in case the
@@ -340,14 +337,18 @@
         """Triggers an immediate state reload.
 
         This method is useful when changes to the clock occur,
         or when a new function is pushed to the runner.
         """
         self._reload_event.set()
 
+    def _merge_states(self, old: FunctionState, new: FunctionState) -> None:
+        new.args = new.args + old.args[len(new.args) :]
+        new.kwargs = old.kwargs | new.kwargs
+
     # Lifecycle control
 
     def start(self):
         """Initializes the background runner task.
 
         If the task has already started, this is a no-op.
         """
@@ -436,15 +437,29 @@
         if self._can_correct_interval and interval != self._last_interval:
             time = self._expected_time
             self.interval_shift = self.clock.get_beat_time(period, time=time)
 
         self._last_interval = interval
         self._can_correct_interval = False
 
-    def _get_corrected_interval(self, period: Union[float, int]) -> float:
+    def _correct_interval_background_job(self, period: Union[float, int]):
+        """
+        Alternative version for fixed-rate background jobs. The interval or
+        period is not indexed on the clock like with the _correct_interval
+        method above.
+        """
+        interval = period
+        if self._can_correct_interval and interval != self._last_interval:
+            time = self._expected_time
+            self.interval_shift = self.clock.get_beat_time(period, time=time)
+
+        self._last_interval = interval
+        self._can_correct_interval = False
+
+    def _get_next_deadline(self, period: Union[float, int]) -> float:
         """Returns the amount of time until the next interval.
 
         The base interval is determined by the `period` argument,
         and then offsetted by the `interval_shift` attribute.
 
         If the `snap` attribute is set to an absolute time
         and the current clock time has not passed the snap,
@@ -453,60 +468,74 @@
         Args:
             period (Union[float, int]):
                 The number of beats in the interval.
 
         Returns:
             float: The deadline for the next interval.
         """
-        # We only want to use the expected time if the last iteration
-        # ran its function normally - if the runner skipped the iteration,
-        # that means we haven't yet reached the deadline
-        if self._last_iteration_called:
-            time = self._expected_time
-        else:
-            time = self.clock.time
+        # If this is called earlier than the expected time, we should use
+        # the current time to avoid calculating the next beat too far ahead,
+        # which would cause an unusually long gap between iterations.
+        #
+        # If this is called after the expected time has already passed,
+        # we should continue from that iteration and ignore the current time.
+        # This allows returning an overdue deadline potentially caused by a
+        # high delta, letting missed iterations fire ASAP.
+        #
+        # Given the above requirements, this would be the ideal solution:
+        #     time = min(self.clock.time, self._expected_time)
+        #
+        # However, this is complicated by SleepHandler which does not guarantee
+        # that a successful iteration will never be earlier than the deadline.
+        # As such, we will additionally prevent the time from being sooner than
+        # the last successful iteration.
+        # If we ignored this and allowed deadlines earlier than the last iteration,
+        # the above solution could potentially trigger non-missed iterations too early.
+        time = max(self._last_expected_time, min(self.clock.time, self._expected_time))
 
         self._check_snap(time)
         if self.snap is not None:
             return self.snap
 
         shifted_time = time + self.interval_shift
 
         # If the interval was corrected, this should equal to:
         #    `period * beat_duration`
         expected_duration = self.clock.get_beat_time(period, time=shifted_time)
-        # print('wait for', expected_duration, 'time:', time, 'shift:', self.interval_shift)
+
         return time + expected_duration
 
     # Runner loop
 
     async def _runner(self):
         try:
             self._prepare()
         except Exception as exc:
             self._revert_state()
             raise exc
 
-        print_panel(f"[yellow][[red]{self.name}[/red] is swimming][/yellow]")
+        if not self.background_job:
+            print(f"[yellow][[red]{self.name}[/red] is swimming][/yellow]")
 
         try:
             while self._is_ready_for_iteration():
+                # self._last_interval = self._get_period(self._last_state) * self.clock.beat_duration
                 try:
                     await self._run_once()
                 except Exception as exc:
                     print(f"[red][Function exception | ({self.name})]")
                     traceback.print_exception(type(exc), exc, exc.__traceback__)
 
                     self._revert_state()
                     self.swim()
         finally:
-            print_panel(f"[yellow][Stopped [red]{self.name}[/red]][/yellow]")
+            print(f"[yellow][Stopped [red]{self.name}[/red]][/yellow]")
 
     def _prepare(self):
-        self._last_iteration_called = False
+        self._last_expected_time = -math.inf
         self._last_state = self._get_state()
         self._swimming = True
         self._stop = False
 
         period = self._get_period(self._last_state)
         self._last_interval = period * self.clock.beat_duration
 
@@ -523,27 +552,36 @@
 
             _assert_function_signature(signature, state.args, state.kwargs)
             args = state.args
             # Prevent any TypeErrors when the user reduces the signature
             kwargs = _discard_kwargs(signature, state.kwargs)
             period = _extract_new_period(signature, state.kwargs)
 
-            self._correct_interval(period)
-            deadline = self._get_corrected_interval(period)
+            if not self.background_job:
+                self._correct_interval(period)
+            else:
+                self._correct_interval_background_job(period)
+            deadline = self._get_next_deadline(period)
 
         # Push any deferred states that have or will arrive onto the stack
         arriving_states: list[DeferredState] = []
         while self.deferred_states:
             entry = self.deferred_states[0]
             if (
                 self.clock.time >= entry.deadline
                 or state is not None
                 and deadline >= entry.deadline
             ):
                 heapq.heappop(self.deferred_states)
+
+                # Transfer any arguments from previous function if any
+                # (similar to what `push()` does)
+                if state is not None:
+                    self._merge_states(state, entry.state)
+
                 arriving_states.append(entry)
             else:
                 break
 
         if arriving_states:
             latest_entry = arriving_states[-1]
             self.states.extend(e.state for e in arriving_states)
@@ -568,15 +606,15 @@
         try:
             # Use copied context in function by creating it as a task
             await asyncio.create_task(
                 self._call_func(state.func, args, kwargs),
                 name=f"asyncrunner-func-{self.name}",
             )
         finally:
-            self._last_iteration_called = True
+            self._last_expected_time = self._expected_time
 
     async def _call_func(self, func, args, kwargs):
         """Calls the given function and optionally applies time shift
         according to the `defer_beats` attribute.
         """
         if self.defer_beats:
             delta = self.clock.time - self._expected_time
@@ -601,17 +639,17 @@
             and self._swimming  # self.swim()
             and not self._stop  # self.stop()
         )
 
     def _maybe_print_new_state(self, state: FunctionState):
         if self._last_state is not None and state is not self._last_state:
             if not self._has_reverted:
-                print_panel(f"[yellow][Updating [red]{self.name}[/red]]")
+                print(f"[yellow][Updating [red]{self.name}[/red]]")
             else:
-                print_panel(f"[yellow][Saving [red]{self.name}[/red] from crash]")
+                print(f"[yellow][Saving [red]{self.name}[/red] from crash]")
                 self._has_reverted = False
 
     async def _sleep_until(self, deadline: Union[float, int]) -> bool:
         """Sleeps until the given deadline or until the runner is reloaded.
 
         Args:
             duration (Union[float, int]): The amount of time to sleep.
@@ -639,9 +677,8 @@
 
     def _revert_state(self):
         if self.states:
             self.states.pop()
         self._has_reverted = True
 
     def _skip_iteration(self) -> None:
-        self._last_iteration_called = False
         self.swim()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sardine_system-0.2.1/sardine/scheduler/scheduler.py` & `sardine-system-0.4.0/sardine_core/scheduler/scheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,25 @@
         self,
         deferred_scheduling: bool = True,
     ):
         super().__init__()
         self._runners: dict[str, AsyncRunner] = {}
         self.deferred = deferred_scheduling
 
+    def _react_to_tempo_change(self, old_tempo: int | float, new_tempo: int | float):
+        """
+        In reaction to a tempo change, the scheduler should
+        trigger an event for each runner prompting to update
+        their current interval_shift. This prevents runners
+        from desynchronization everytime tempo change happens.
+        """
+        scale = old_tempo / new_tempo
+        for runner in self._runners.values():
+            runner.interval_shift *= scale
+
     def __repr__(self) -> str:
         n_runners = len(self._runners)
         return "<{} ({} {}) deferred={}>".format(
             type(self).__name__,
             n_runners,
             plural(n_runners, "runner"),
             self.deferred,
@@ -100,24 +111,28 @@
         """Stops and removes all runners from the scheduler.
 
         Args:
             *args: Positional arguments to be passed to `stop_runner()`.
             **kwargs: Keyword arguments to be passed to `stop_runner()`.
         """
         for runner in self.runners:
-            self.stop_runner(runner, *args, **kwargs)
+            if not runner.background_job:
+                self.stop_runner(runner, *args, **kwargs)
 
     # Internal methods
 
     def _reload_runners(self, *, interval_correction: bool):
         for runner in self._runners.values():
             runner.reload()
 
             if interval_correction:
                 runner.allow_interval_correction()
 
     def setup(self):
         self.register("stop")
+        self.register("tempo_change")
 
     def hook(self, event: str, *args):
         if event == "stop":
             self.reset()
+        if event == "tempo_change":
+            self._react_to_tempo_change(*args)
```

### Comparing `sardine_system-0.2.1/sardine/sequences/chance.py` & `sardine-system-0.4.0/sardine_core/sequences/chance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from random import choices as randomChoices
 from random import randint, random
 
 # ==============================================================================#
 
+
 # Inspired by TidalCycles
 def always():
     return True
 
 
 def almostAlways():
     return True if random() < 0.90 else False
```

### Comparing `sardine_system-0.2.1/sardine/sequences/iterators.py` & `sardine-system-0.4.0/sardine_core/sequences/iterators.py`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/sequences/variables.py` & `sardine-system-0.4.0/sardine_core/sequences/variables.py`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/sequences/sardine_parser/list_parser.py` & `sardine-system-0.4.0/sardine_core/sequences/sardine_parser/list_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,57 @@
-from pathlib import Path
-
-from lark import Lark, Tree
-from rich import print
-
+from .tree_calc import CalculateTree
 from ...base import BaseParser
+from lark import Lark, Tree
+from lark.exceptions import LarkError, UnexpectedCharacters, UnexpectedToken
+from pathlib import Path
 from .chord import Chord
-from .tree_calc import CalculateTree
+from ...logger import print
+import traceback
 
-# __all__ = ("ListParser", "Pnote", "Pname", "Pnum")
-__all__ = ("ListParser", "Pat")
+__all__ = ("ListParser",)
 
 
 class ParserError(Exception):
     pass
 
 
-# This section of the code is charged with retrieval and loading of grammar
-# files stored in the grammars/ subfolder next to ListParser.py. Each file
-# contains the formal specification of the grammar, and is used by Lark to
-# build an abstract syntax tree and get the combination rules for each token.
+class ShortParserError(Exception):
+    def __init__(self, message):
+        self.message = message
+
+    def __str__(self):
+        return self.message
+
 
 grammar_path = Path(__file__).parent
 grammar = grammar_path / "sardine.lark"
 
 
 class ListParser(BaseParser):
     def __init__(
         self,
         parser_type: str = "sardine",
         debug: bool = False,
     ):
-        """ListParser is the main interface for the pattern syntax. It can be
-        initialised in three different modes: 'number', 'note', 'name'. It is
-        up to the user to choose the parser that fits best to a task. Each
-        parser will be initialised two times, in two different modes:
-        - full: the parser as it is used for parsing expressions and returning
-        a result.
-        - raw: the parser as it is used to print the syntax tree in debug mode.
-
-        Args:
-            parser_type (str, optional): Type of parser. Defaults to "number".
         """
+        ListParser is the main interface to the SPL pattern language. ListParser is
+        a programming language capable of handling notes, names, samples, OSC
+        addresses, etc...
+        """
+
         super().__init__()
         self.debug = debug
         self.parser_type = parser_type
 
+        # Variables usable only in the SPL environment
+        self.inner_variables = {}
+
+        # Current Global Scale
+        self.global_scale: str = "major"
+
     def __repr__(self) -> str:
         return f"<{type(self).__name__} debug={self.debug} type={self.parser_type!r}>"
 
     def setup(self):
         parsers = {
             "sardine": {
                 "raw": Lark.open(
@@ -63,29 +66,32 @@
                     grammar,
                     rel_to=__file__,
                     parser="lalr",
                     start="start",
                     cache=True,
                     lexer="contextual",
                     transformer=CalculateTree(
-                        self.env.clock, self.env.iterators, self.env.variables
+                        clock=self.env.clock,
+                        variables=self.env.variables,
+                        inner_variables=self.inner_variables,
+                        global_scale=self.global_scale,
                     ),
                 ),
             },
         }
 
         try:
             self._result_parser = parsers[self.parser_type]["full"]
             self._printing_parser = parsers[self.parser_type]["raw"]
         except KeyError:
             ParserError(f"Invalid Parser grammar, {self.parser_type} is not a grammar.")
 
     def __flatten_result(self, pat):
-        """Flatten a nested list, for usage after parsing a pattern. Will
-        flatten deeply nested lists and return a one dimensional array.
+        """Flatten a nested list, for usage after parsing a pattern. Will flatten deeply
+        nested lists and return a one dimensional array.
 
         Args:
             pat (list): A potentially nested list
 
         Returns:
             list: A flat list (one-dimensional)
         """
@@ -138,18 +144,19 @@
             ParserError: Raised if the pattern is invalid
 
         Returns:
             list: The parsed pattern as a list of values
         """
         pattern = args[0]
         final_pattern = []
+
         try:
             final_pattern = self._result_parser.parse(pattern)
         except Exception as e:
-            raise ParserError(f"Non valid token: {pattern}: {e}")
+            print(f"[red][Pattern Language Error][/red]")
 
         if self.debug:
             print(f"Pat: {self._flatten_result(final_pattern)}")
         return self._flatten_result(final_pattern)
 
     def _parse_debug(self, pattern: str):
         """Parses a whole pattern in debug mode. 'Debug mode' refers to
@@ -159,25 +166,12 @@
 
         Args:
             pattern (str): A pattern to be parse.
         """
         try:
             self.pretty_print(expression=pattern)
         except Exception as e:
-            import traceback
-
-            print(f"Error: {e}: {traceback.format_exc()}")
-
-
-def Pat(pattern: str, i: int = 0):
-    """Generates a pattern
-
-    Args:
-        pattern (str): A pattern to be parsed
-        i (int, optional): Index for iterators. Defaults to 0.
-
-    Returns:
-        int: The ith element from the resulting pattern
-    """
-    parser = ListParser(clock=c, parser_type="sardine")
-    result = parser.parse(pattern)
-    return result[i % len(result)]
+            tb_str = traceback.format_exception(
+                etype=type(e), value=e, tb=e.__traceback__
+            )
+            error_message = "".join(tb_str)
+            raise ParserError(f"Error parsing pattern {pattern}: {error_message}")
```

### Comparing `sardine_system-0.2.1/sardine/sequences/sardine_parser/utils.py` & `sardine-system-0.4.0/sardine_core/sequences/sardine_parser/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,16 +69,18 @@
     """Apply an binary function to a value or a list of values
 
     Args:
         func: The function to apply
         left: The left value or list of values
         right: The right value or list of values
     """
-    if any(isinstance(x, Chord) for x in (left, right)):
-        return Chord(*[allow_silence_2(func)(x, y) for x, y in zip_cycle(left, right)])
+    if isinstance(left, Chord) and not isinstance(right, Chord):
+        return [allow_silence_2(func)(left, y) for y in right]
+    elif isinstance(right, Chord) and not isinstance(left, Chord):
+        return [allow_silence_2(func)(x, right) for x in left]
     else:
         return [allow_silence_2(func)(x, y) for x, y in zip_cycle(left, right)]
 
 
 # Taken from:
 # https://stackoverflow.com/questions/26531116/is-it-a-way-to-know-index-using-itertools-cycle
```

### Comparing `sardine_system-0.2.1/sardine/superdirt/default_superdirt.scd` & `sardine-system-0.4.0/sardine_core/superdirt/default_superdirt.scd`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/sardine/superdirt/process.py` & `sardine-system-0.4.0/sardine_core/superdirt/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/usr/bin/env python3
+
+import sys
 import asyncio
 import platform
 import shutil
 import subprocess
 import tempfile
 from os import path, walk
 from pathlib import Path
 from typing import Optional, Union
+from ..logger import print
 
 import psutil
 from appdirs import *
-from rich import print
 from rich.console import Console
-from rich.panel import Panel
 
 __all__ = ("SuperDirtProcess",)
 
 
 class SuperDirtProcess:
     def __init__(
         self, startup_file: Optional[str] = None, preemptive=True, verbose=False
     ):
-
         appname, appauthor = "Sardine", "Bubobubobubo"
         self._user_dir = Path(user_data_dir(appname, appauthor))
         self._sclang_path = self.find_sclang_path()
         self._synth_directory = self._find_synths_directory()
         self._startup_file = (
             self._find_startup_file(user_file=startup_file)
             if startup_file is not None
@@ -47,15 +47,15 @@
         """Find the startup file when booting Sardine"""
         cur_path = Path(__file__).parent.resolve()
         return "".join([str(cur_path), "/default_superdirt.scd"])
 
     def _find_startup_file(self, user_file: Union[str, None] = None) -> Path:
         """Find the SuperDirt startup file"""
         if not user_file:
-            file_path = Path("/".join([str(self._user_dir), "default_superdirt.scd"]))
+            file_path = self._user_dir / "default_superdirt.scd"
             if file_path.is_file():
                 return file_path
             else:
                 # This should definitely be a try/except case
                 vanilla_file_path = self._find_vanilla_startup_file()
                 shutil.copy(str(vanilla_file_path), self._user_dir)
                 return file_path
@@ -65,91 +65,85 @@
                 return user_file_path
             else:
                 # recurse to base case with no user_file
                 return self._find_startup_file()
 
     def _find_synths_directory(self) -> Path:
         """Find or create the synths directory needed"""
-        path = Path("/".join([str(self._user_dir), "synths/"]))
+        path = self._user_dir / "synths/"
         exists = path.is_dir()
         if exists:
             return path
         else:
             path.mkdir(parents=True)
             return path
 
+    def __call__(self, code: str) -> None:
+        """Send code to the SuperCollider sub-process"""
+        self._write_stdin(code)
+
     def terminate(self) -> None:
         """Terminate the SCLang process"""
         self._write_stdin("Server.killAll; 0.exit;")
         self._sclang.terminate()
 
     def _analyze_and_warn(self, decoded_line: str):
         """
         Analyse the last line from SuperCollider logs and warn the user if something
         shady is going on (like not being able to boot the server, late messages)
         """
         if "no synth or sample" in decoded_line:
             sample_name = decoded_line.split("'")
-            print("\n")
-            print(Panel.fit(f"[red]/!\\\\[/red] - Sample {sample_name[1]} not found."))
+            print(f"[[red]/!\\\\[/red] - Sample {sample_name[1]} not found]")
         if "late 0." in decoded_line:
-            print("\n")
-            print(Panel.fit(f"[red]/!\\\\[/red] - Late messages. Increase SC latency."))
-        if "listening to Tidal on port 57120" in decoded_line:
-            print("\n")
-            print(Panel.fit(f"[green]/!\\\\[/green] - Audio server ready!"))
+            print(f"[[red]/!\\\\[/red] - Late messages. Increase SC latency]")
+        if "listening on port 57120" in decoded_line:
+            print(f"[[green]/!\\\\[/green] - Audio server ready!]")
+            if self._synth_directory is not None:
+                self.load_custom_synthdefs()
         if "ERROR: failed to open UDP socket: address in use" in decoded_line:
-            print("\n")
             print(
-                Panel.fit(
-                    (
-                        f"[red]/!\\\\[/red] - Socket in use! SuperCollider is already"
-                        + "\nrunning somewhere. It might be a mistake or a"
-                        + "\nzombie process. Run `Server.killAll` in an SC"
-                        + "\nwindow (can be the IDE of `sclang` in term..)"
-                    )
+                (
+                    f"[red]/!\\\\[/red] - Socket in use! SuperCollider is already"
+                    + "\nrunning somewhere. It might be a mistake or a"
+                    + "\nzombie process. Run `Server.killAll` in an SC"
+                    + "\nwindow (can be the IDE of `sclang` in term..)"
                 )
             )
         if "Mismatched sample rates are not supported" in decoded_line:
-            print("\n")
             print(
-                Panel.fit(
-                    (
-                        f"[red]/!\\\\[/red] - Mismatched sample rates. Please make"
-                        + "\nsure that your audio input sample rate and"
-                        + "\nyour audio output sample rate are the same."
-                        + "\nThis is usually modified in your OS audio"
-                        + "\nconfiguration menus. Reboot Sardine!"
-                    )
+                (
+                    f"[red]/!\\\\[/red] - Mismatched sample rates. Please make"
+                    + "\nsure that your audio input sample rate and"
+                    + "\nyour audio output sample rate are the same."
+                    + "\nThis is usually modified in your OS audio"
+                    + "\nconfiguration menus. Reboot Sardine!"
                 )
             )
 
     async def monitor(self):
         """
         Monitoring SuperCollider output using an asynchronous function
         that runs on a loop and prints to output. Can be quite verbose at
         boot time!
         """
-        import sys
 
         try:
             while self._sclang.poll() is None:
                 where = self.temp_file.tell()
                 lines = self.temp_file.read()
                 if not lines:
-                    await asyncio.sleep(0.1)
+                    await asyncio.sleep(0.05)
                     self.temp_file.seek(where)
                 else:
+                    decoded_lines = lines.decode()
                     if self._verbose:
-                        sys.__stdout__.write(lines.decode())
+                        print(decoded_lines.strip())
                     else:
-                        self._analyze_and_warn(lines.decode())
-                    sys.__stdout__.flush()
-            sys.__stdout__.write(self.temp_file.read())
-            sys.__stdout__.flush()
+                        self._analyze_and_warn(decoded_lines)
         except UnboundLocalError:
             raise UnboundLocalError("SCLang is not reachable...")
 
     def hard_kill(self) -> None:
         """Look for all instances of SuperCollider, kill them."""
         try:
             for proc in psutil.process_iter():
@@ -194,14 +188,18 @@
         """Open SuperCollider frequency scope"""
         self._write_stdin("s.freqscope()")
 
     def meterscope(self) -> None:
         """Open SuperCollider frequency scope + VUmeter"""
         self._write_stdin("s.scope(); s.meter()")
 
+    def info(self) -> None:
+        """Open makeWindow window"""
+        self._write_stdin("s.makeWindow")
+
     def _check_synth_file_extension(self, string: str) -> bool:
         return string.endswith(".scd") or string.endswith(".sc")
 
     def startup_file_path(self) -> str | None:
         return self._startup_file
 
     def load_custom_synthdefs(self) -> None:
@@ -220,15 +218,15 @@
             # sending the string to the interpreter
             self._write_stdin(buffer)
             for f in files:
                 loaded_synthdefs_message.append("- {}".format(f))
         if len(loaded_synthdefs_message) == 1:
             return
         else:
-            print(Panel.fit("\n".join(loaded_synthdefs_message)))
+            print("\n".join(loaded_synthdefs_message))
 
     def find_sclang_path(self) -> str:
         """Find path to sclang binary, cross-platform"""
         os_name = platform.system()
         if os_name == "Linux":
             return "sclang"
         elif os_name == "Windows":
@@ -263,15 +261,18 @@
                 stdout=self.temp_file,
                 stderr=self.temp_file,
                 bufsize=1,
                 universal_newlines=True,
                 start_new_session=True,
             )
             if self._startup_file is not None:
-                self._write_stdin(message="""load("{}")""".format(self._startup_file))
-            if self._synth_directory is not None:
-                self.load_custom_synthdefs()
+                startup_file_path = (
+                    str(self._startup_file).replace("\\", "\\\\")
+                    if platform.system() == "Windows"
+                    else self._startup_file
+                )
+                self._write_stdin(message="""load("{}")""".format(startup_file_path))
 
     def kill(self) -> None:
         """Kill the connexion with the SC Interpreter"""
         self._write_stdin("Server.killAll")
         self._write_stdin("0.exit")
```

### Comparing `sardine_system-0.2.1/sardine/utils/Messages.py` & `sardine-system-0.4.0/sardine_core/utils/Messages.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 def _ticked(condition: bool):
     """Print an ASCII Art [X] if True or [ ] if false"""
     return "[X]" if condition else "[ ]"
 
 
 def config_line_printer(config: dict):
+    midi_port = "Automatic" if config.midi == "Sardine" else config.midi
     return (
         f"[yellow]BPM: [red]{config.bpm}[/red],"
         + f"[yellow]BEATS: [red]{config.beats}[/red] "
         + f"[yellow]SC: [red]{_ticked(config.superdirt_handler)}[/red], "
         + f"[yellow]DEFER: [red]{_ticked(config.deferred_scheduling)}[/red] "
         + f"[yellow]MIDI: [red]{config.midi}[/red]"
     )
```

### Comparing `sardine_system-0.2.1/sardine/utils/__init__.py` & `sardine-system-0.4.0/sardine_core/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,7 +60,23 @@
     if inspect.iscoroutinefunction(func):
         return await func(*args, **kwargs)
     return func(*args, **kwargs)
 
 
 def plural(n: int, word: str, suffix: str = "s"):
     return word if n == 1 else word + suffix
+
+
+def join(*args):
+    """Alternative to the str.join function. Better in live contexts!
+
+    Parameters:
+    *args (list[string]): a list of strings to join with a whitespace
+
+    Returns:
+    list[string]: strings joined using ' '.join(args)
+
+    """
+    if all(isinstance(e, str) for e in args):
+        return " ".join(args)
+    else:
+        return args[0]
```

### Comparing `sardine_system-0.2.1/tests/test_patterns.py` & `sardine-system-0.4.0/tests/test_patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 import pytest_asyncio
 
-from sardine import FishBowl
-from sardine.sequences import ListParser
+from sardine_core import FishBowl
+from sardine_core.sequences import ListParser
 
 
 # NOTE: only put new parsers here if they support sardine's patterning syntax
 @pytest_asyncio.fixture(scope="module", params=[ListParser])
 def fish_bowl(request: pytest.FixtureRequest):
     return FishBowl(parser=request.param())
```

### Comparing `sardine_system-0.2.1/tests/test_utils.py` & `sardine-system-0.4.0/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 from typing import Sequence, Union
 
 import pytest
 
-from sardine import utils
+from sardine_core import utils
 
 Number = Union[float, int]
 
 
 @pytest.mark.parametrize(
     "x,in_min,in_max,out_min,out_max,expected",
     [
```

### Comparing `sardine_system-0.2.1/LICENSE.txt` & `sardine-system-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sardine_system-0.2.1/README.md` & `sardine-system-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,100 @@
+Metadata-Version: 2.1
+Name: sardine-system
+Version: 0.4.0
+Summary: Python's missing algorave module
+Author: Raphaël Forment, thegamecracks
+Author-email: raphael.forment@gmail.com
+License: GPL-3.0-only
+Project-URL: Homepage, https://sardine.raphaelforment.fr
+Project-URL: Documentation, https://sardine.raphaelforment.fr
+Project-URL: Source Code, https://github.com/Bubobubobubobubo/sardine
+Project-URL: Bug Tracker, https://github.com/Bubobubobubobubo/sardine/issues
+Keywords: algorave,live-coding,music,patterns
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Artistic Software
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: profile
+License-File: LICENSE.txt
+
 <h2 align="center">
   <b>Sardine</b>: ✨ Live Coding Library for Python ✨
 </h2>
 <p align="center"><i>
-  Python's missing algorave module.
-  Simple/hackable live coding tool for modern Python (3.10+)
+  Python's missing algorave module. Hackable live coding tool for modern Python (3.10+)
 </i></p>
 
 <p align="center">
   <img src=https://img.shields.io/discord/1029399269574193203 />
   <img src=https://img.shields.io/github/license/Bubobubobubobubo/sardine />
   <img src=https://img.shields.io/github/stars/Bubobubobubobubo/sardine />
+  <img src=https://img.shields.io/pypi/wheel/sardine-system>
+  <img src=https://img.shields.io/pypi/v/sardine-system>
+  <img src=https://img.shields.io/pypi/status/sardine-system>
 </p>
 
 <p align="center">
   <a href="https://discord.gg/aPgV7mSFZh">Discord</a> |
   <a href="https://sardine.raphaelforment.fr/">Website</a> |
-  <a href="https://sardine.raphaelforment.fr/documentation/sardinopedia/introduction/">Examples</a> |
-  <a href="https://sardine.raphaelforment.fr/technical/installation/">Installation</a> |
+  <a href="https://sardine.raphaelforment.fr/showcase">Examples</a> |
+  <a href="https://sardine.raphaelforment.fr/installation/">Installation</a> |
   <a href="https://raphaelforment.fr/">Author</a>  |
   <a href="https://toplap.org/">About Live Coding</a>
   <br><br>
   <p align='center'>
     <a href="https://github.com/bubobubobubobubo/sardine/graphs/contributors">
     <img src="https://contrib.rocks/image?repo=bubobubobubobubo/sardine" />
     </a>
   </p>
 </p>
 
 -----------
 
 ![Sardine algorave picture](pictures/sardine_intro_picture_repo.png)
 
-Sardine is a hacker-friendly Python library tailored for musical improvisation,
-algorithmic composition and much more. **Sardine** is transforming your typical
-**Python** interpreter into a music instrument that allows you to write melodic
-and rhythmic patterns of any kind and to map them to any electronic instrument:
-**MIDI**, **OSC** and/or **SuperCollider**. Using **Sardine**, you can:
-
-- **Improvise music freely on stage / in the studio / for your own enjoyment.**
-  - **Sardine** can talk to any MIDI/OSC device and to the **SuperCollider**
-    audio engine.
-  - Bindings for **SuperDirt**, a well-known synthesis engine used by
-    live coders around the world.
-- **Build complex and rich audio/visual installations using MIDI and OSC *I/O*.**
-  - Attach **callbacks** to any OSC event, turn **Sardine** into a complex
-    reactive toolbox.
-  - Watch values as they change and propagate them to your musical patterns or code.
-- **Synchronise with other computers / other musical instruments**
-  - **MIDI Clock** Out.
-  - **Link Protocol** synchronization.
-- **Make Python code time-aware**
-  - Using temporal recursion, you can make any Python code time and tempo aware.
-  - Launch any sync or async function precisely in time,
-    with results falling back on time.
-  - Hack your own **Senders** or **Receivers** to pattern whatever you see fit!
+**Sardine** is a versatile and hacker-friendly Python library designed for musical improvisation, algorithmic composition, and beyond.
+It transforms your standard **Python** interpreter into a powerful music instrument, enabling you to create and map melodic and rhythmic
+patterns to any electronic instrument (**MIDI**, **OSC**, and **SuperCollider**).
+With **Sardine**, you can:
+
+- **Unleash your musical creativity on stage, in the studio, or for personal enjoyment**
+  - Seamlessly communicate with any MIDI/OSC device and the **SuperCollider** audio engine using **Sardine**.
+  - Utilize bindings for **SuperDirt**, a widely recognized synthesis engine embraced by live coders globally.
+
+- **Empower your Python code with time-aware capabilities**
+  - Employ temporal recursion to make any Python code time and tempo aware.
+  - Accurately launch synchronous or asynchronous functions with time-specific results.
+  - Customize your own **Senders** or **Receivers** to pattern any desired elements!
+
+- **Develop intricate audio/visual installations with MIDI and OSC *I/O***
+  - Assign **callbacks** to any OSC event, transforming **Sardine** into a sophisticated reactive toolbox.
+  - Monitor changing values and incorporate them into your musical patterns or code.
+
+- **Synchronize with other computers and musical instruments**
+  - Synchronise your hardware with **MIDI Clocks**.
+  - Synchronize effortlessly with other tools or players using the **Link Protocol**.
 
 ## Installation
 
-In order to install Sardine, your system will require a recent version of Python (3.10+). We now support 3.11 versions as well. A more detailed installation guide can be found on [Sardine's website](https://sardine.raphaelforment.fr/technical/installation/).
-
-1) Run: `python -m pip install --find-links https://thegamecracks.github.io/python-rtmidi-wheels/ sardine-system`.
-    - the `--find-links` option is used as a temporary fix to the unavailability of some dependencies in the Pypi repositories for Python 3.10/3.11.
-2) Install [SuperCollider](https://supercollider.github.io/) and [SuperDirt](https://github.com/musikinformatik/SuperDirt) for an additional supported audio backend.
-3) Run `sardine-config` and configure Sardine to your liking following [this guide](https://sardine.raphaelforment.fr/technical/configuration/)
-4) Install the text editor of your choice: VSCode, Neovim, Vim, Emacs, Jupyter Notebook, etc... There are many options you can pick from. They have all been tested with Sardine.
+Refer to the [installation section](https://sardine.raphaelforment.fr/installation.html).
 
 ## Contributions
 
-Sardine is currently in the early development phase. We are looking for contributors! Anybody is welcome to contribute with code / documentation / thoughts, etc... You can contact the **Sardine** community directly on **Discord** or **PM** me if you have specific questions.
-
-### Documenting Sardine
-
-**Sardine** is a **Python** library that you learn to use as a musical instrument. For this reason, documentation is of paramount importance so that others can learn your cool tricks too :). The documentation resides in the `docs/` folder. It is a bunch of loosely organised Markdown files. You can contribute by editing these files and adding the missing bit of information you would like to see being updated or added.
+Sardine is in its early stages of development, and we're actively seeking contributors to help enhance the project. If you're passionate
+about music and technology, we welcome your expertise, whether it's code, documentation, or ideas. We are looking for contributors! 
 
-Source code is contained to the `sardine/` and `fishery/` folder. Most functions are already documented but the architecture of **Sardine** needs some time to get used to. You can contact me directly if you would like to learn more about it. There are no contributions rules for the moment, and I will explore each and every request that you would like to propose!
+To collaborate with the Sardine community, connect with us on **Discord**, **Github** or send a private message if you have specific inquiries.
+Together, we can create an even more powerful tool for musical expression and creativity!
```

#### html2text {}

```diff
@@ -1,56 +1,58 @@
+Metadata-Version: 2.1 Name: sardine-system Version: 0.4.0 Summary: Python's
+missing algorave module Author: RaphaÃ«l Forment, thegamecracks Author-email:
+raphael.forment@gmail.com License: GPL-3.0-only Project-URL: Homepage, https://
+sardine.raphaelforment.fr Project-URL: Documentation, https://
+sardine.raphaelforment.fr Project-URL: Source Code, https://github.com/
+Bubobubobubobubo/sardine Project-URL: Bug Tracker, https://github.com/
+Bubobubobubobubo/sardine/issues Keywords: algorave,live-coding,music,patterns
+Classifier: Development Status :: 3 - Alpha Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Artistic Software Classifier:
+Topic :: Multimedia Classifier: Topic :: Multimedia :: Sound/Audio Classifier:
+Topic :: Multimedia :: Sound/Audio :: MIDI Requires-Python: >=3.10 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: profile
+License-File: LICENSE.txt
           ***** Sardine: â¨ Live Coding Library for Python â¨ *****
- Python's missing algorave module. Simple/hackable live coding tool for modern
-                                Python (3.10+)
+Python's missing algorave module. Hackable live coding tool for modern Python
+                                    (3.10+)
  [https://img.shields.io/discord/1029399269574193203] [https://img.shields.io/
 github/license/Bubobubobubobubo/sardine] [https://img.shields.io/github/stars/
-                           Bubobubobubobubo/sardine]
+ Bubobubobubobubo/sardine] [https://img.shields.io/pypi/wheel/sardine-system]
+ [https://img.shields.io/pypi/v/sardine-system] [https://img.shields.io/pypi/
+                            status/sardine-system]
    Discord | Website | Examples | Installation | Author | About_Live_Coding
 
           [https://contrib.rocks/image?repo=bubobubobubobubo/sardine]
 ----------- ![Sardine algorave picture](pictures/
-sardine_intro_picture_repo.png) Sardine is a hacker-friendly Python library
-tailored for musical improvisation, algorithmic composition and much more.
-**Sardine** is transforming your typical **Python** interpreter into a music
-instrument that allows you to write melodic and rhythmic patterns of any kind
-and to map them to any electronic instrument: **MIDI**, **OSC** and/or
-**SuperCollider**. Using **Sardine**, you can: - **Improvise music freely on
-stage / in the studio / for your own enjoyment.** - **Sardine** can talk to any
-MIDI/OSC device and to the **SuperCollider** audio engine. - Bindings for
-**SuperDirt**, a well-known synthesis engine used by live coders around the
-world. - **Build complex and rich audio/visual installations using MIDI and OSC
-*I/O*.** - Attach **callbacks** to any OSC event, turn **Sardine** into a
-complex reactive toolbox. - Watch values as they change and propagate them to
-your musical patterns or code. - **Synchronise with other computers / other
-musical instruments** - **MIDI Clock** Out. - **Link Protocol**
-synchronization. - **Make Python code time-aware** - Using temporal recursion,
-you can make any Python code time and tempo aware. - Launch any sync or async
-function precisely in time, with results falling back on time. - Hack your own
-**Senders** or **Receivers** to pattern whatever you see fit! ## Installation
-In order to install Sardine, your system will require a recent version of
-Python (3.10+). We now support 3.11 versions as well. A more detailed
-installation guide can be found on [Sardine's website](https://
-sardine.raphaelforment.fr/technical/installation/). 1) Run: `python -m pip
-install --find-links https://thegamecracks.github.io/python-rtmidi-wheels/
-sardine-system`. - the `--find-links` option is used as a temporary fix to the
-unavailability of some dependencies in the Pypi repositories for Python 3.10/
-3.11. 2) Install [SuperCollider](https://supercollider.github.io/) and
-[SuperDirt](https://github.com/musikinformatik/SuperDirt) for an additional
-supported audio backend. 3) Run `sardine-config` and configure Sardine to your
-liking following [this guide](https://sardine.raphaelforment.fr/technical/
-configuration/) 4) Install the text editor of your choice: VSCode, Neovim, Vim,
-Emacs, Jupyter Notebook, etc... There are many options you can pick from. They
-have all been tested with Sardine. ## Contributions Sardine is currently in the
-early development phase. We are looking for contributors! Anybody is welcome to
-contribute with code / documentation / thoughts, etc... You can contact the
-**Sardine** community directly on **Discord** or **PM** me if you have specific
-questions. ### Documenting Sardine **Sardine** is a **Python** library that you
-learn to use as a musical instrument. For this reason, documentation is of
-paramount importance so that others can learn your cool tricks too :). The
-documentation resides in the `docs/` folder. It is a bunch of loosely organised
-Markdown files. You can contribute by editing these files and adding the
-missing bit of information you would like to see being updated or added. Source
-code is contained to the `sardine/` and `fishery/` folder. Most functions are
-already documented but the architecture of **Sardine** needs some time to get
-used to. You can contact me directly if you would like to learn more about it.
-There are no contributions rules for the moment, and I will explore each and
-every request that you would like to propose!
+sardine_intro_picture_repo.png) **Sardine** is a versatile and hacker-friendly
+Python library designed for musical improvisation, algorithmic composition, and
+beyond. It transforms your standard **Python** interpreter into a powerful
+music instrument, enabling you to create and map melodic and rhythmic patterns
+to any electronic instrument (**MIDI**, **OSC**, and **SuperCollider**). With
+**Sardine**, you can: - **Unleash your musical creativity on stage, in the
+studio, or for personal enjoyment** - Seamlessly communicate with any MIDI/OSC
+device and the **SuperCollider** audio engine using **Sardine**. - Utilize
+bindings for **SuperDirt**, a widely recognized synthesis engine embraced by
+live coders globally. - **Empower your Python code with time-aware
+capabilities** - Employ temporal recursion to make any Python code time and
+tempo aware. - Accurately launch synchronous or asynchronous functions with
+time-specific results. - Customize your own **Senders** or **Receivers** to
+pattern any desired elements! - **Develop intricate audio/visual installations
+with MIDI and OSC *I/O*** - Assign **callbacks** to any OSC event, transforming
+**Sardine** into a sophisticated reactive toolbox. - Monitor changing values
+and incorporate them into your musical patterns or code. - **Synchronize with
+other computers and musical instruments** - Synchronise your hardware with
+**MIDI Clocks**. - Synchronize effortlessly with other tools or players using
+the **Link Protocol**. ## Installation Refer to the [installation section]
+(https://sardine.raphaelforment.fr/installation.html). ## Contributions Sardine
+is in its early stages of development, and we're actively seeking contributors
+to help enhance the project. If you're passionate about music and technology,
+we welcome your expertise, whether it's code, documentation, or ideas. We are
+looking for contributors! To collaborate with the Sardine community, connect
+with us on **Discord**, **Github** or send a private message if you have
+specific inquiries. Together, we can create an even more powerful tool for
+musical expression and creativity!
```

### Comparing `sardine_system-0.2.1/pyproject.toml` & `sardine-system-0.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=67.6.0"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "sardine-system"
 dynamic = ["version"]
 description = "Python's missing algorave module"
 authors = [
     { name = "Raphaël Forment" },
     { email = "raphael.forment@gmail.com" },
-    { name = "thegamecracks" }, 
+    { name = "thegamecracks" },
 ]
-license = "GPL-3.0-only"
-license-files = { paths = ["LICENSE.txt"] }
+license = { text = "GPL-3.0-only" }
 readme = "README.md"
 requires-python = ">=3.10"
 
 keywords = ["algorave", "live-coding", "music", "patterns"]
 
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -33,14 +32,16 @@
     "Topic :: Multimedia",
     "Topic :: Multimedia :: Sound/Audio",
     "Topic :: Multimedia :: Sound/Audio :: MIDI",
 ]
 
 # Requirements: This is done differently by poetry!
 dependencies = [
+    "ziffers>=0.0.1",
+    "parsimonious>=0.10.0",
     "Click>=8.1.3",
     "LinkPython-extern>=1.0.2",
     "python-rtmidi>=1.4.9",
     "inquirerpy>=0.3.4",
     "easing-functions>=1.0.4",
     "mido>=1.2",
     "osc4py3>=1.0.8",
@@ -48,30 +49,33 @@
     "appdirs>=1.4",
     "psutil>=5.9",
     "rich>=12.5",
     "lark>=1.1",
     "exceptiongroup>=1.0.4",
 ]
 
-[tool.hatch.build]
-packages = ["fishery", "sardine"]
+[tool.setuptools]
+# Explicitly declare data files in [tool.setuptools.package-data]
+include-package-data = false
 
-[tool.hatch.build.targets.sdist]
-packages = ["sardine", "fishery", "tests"]
+[tool.setuptools.dynamic]
+version = { attr = "sardine_core.__version__" }
 
-[tool.hatch.version]
-path = "sardine/__init__.py"
+[tool.setuptools.packages.find]
+include = ["sardine_core**", "sardine**"]
+namespaces = false
+
+[tool.setuptools.package-data]
+"sardine_core.sequences.sardine_parser" = ["*.lark"]
+"sardine_core.superdirt" = ["*.scd"]
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 
-[tool.setuptools]
-py-modules = []
-
 [project.optional-dependencies]
 dev = [
     "black>=22.8",
     "pylint>=2.15",
     "pytest>= 7.2.0",
     "pytest-asyncio>=0.20.2",
 ]
@@ -82,18 +86,15 @@
 [project.urls]
 Homepage = "https://sardine.raphaelforment.fr"
 Documentation = "https://sardine.raphaelforment.fr"
 "Source Code" = "https://github.com/Bubobubobubobubo/sardine"
 "Bug Tracker" = "https://github.com/Bubobubobubobubo/sardine/issues"
 
 [project.scripts]
-fishery = 'fishery.__main__:main'
-sardine-config-python = 'sardine.cli.main:edit_python_configuration'
-sardine-config-superdirt = 'sardine.cli.main:edit_superdirt_configuration'
-sardine-config = 'sardine.cli.main:main'
+sardine = 'sardine.__main__:run'
 
 [tool.black]
 target_version = ['py311']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
```

### Comparing `sardine_system-0.2.1/PKG-INFO` & `sardine-system-0.4.0/sardine_system.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sardine-system
-Version: 0.2.1
+Version: 0.4.0
 Summary: Python's missing algorave module
+Author: Raphaël Forment, thegamecracks
+Author-email: raphael.forment@gmail.com
+License: GPL-3.0-only
 Project-URL: Homepage, https://sardine.raphaelforment.fr
 Project-URL: Documentation, https://sardine.raphaelforment.fr
 Project-URL: Source Code, https://github.com/Bubobubobubobubo/sardine
 Project-URL: Bug Tracker, https://github.com/Bubobubobubobubo/sardine/issues
-Author: Raphaël Forment, thegamecracks
-Author-email: raphael.forment@gmail.com
-License-File: LICENSE.txt
 Keywords: algorave,live-coding,music,patterns
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -21,105 +21,80 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Requires-Python: >=3.10
-Requires-Dist: appdirs>=1.4
-Requires-Dist: click>=8.1.3
-Requires-Dist: easing-functions>=1.0.4
-Requires-Dist: exceptiongroup>=1.0.4
-Requires-Dist: inquirerpy>=0.3.4
-Requires-Dist: lark>=1.1
-Requires-Dist: linkpython-extern>=1.0.2
-Requires-Dist: mido>=1.2
-Requires-Dist: osc4py3>=1.0.8
-Requires-Dist: psutil>=5.9
-Requires-Dist: python-rtmidi>=1.4.9
-Requires-Dist: rich>=12.5
-Requires-Dist: uvloop>=0.16; sys_platform != 'win32'
+Description-Content-Type: text/markdown
 Provides-Extra: dev
-Requires-Dist: black>=22.8; extra == 'dev'
-Requires-Dist: pylint>=2.15; extra == 'dev'
-Requires-Dist: pytest-asyncio>=0.20.2; extra == 'dev'
-Requires-Dist: pytest>=7.2.0; extra == 'dev'
 Provides-Extra: profile
-Requires-Dist: yappi>=1.4.0; extra == 'profile'
-Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 <h2 align="center">
   <b>Sardine</b>: ✨ Live Coding Library for Python ✨
 </h2>
 <p align="center"><i>
-  Python's missing algorave module.
-  Simple/hackable live coding tool for modern Python (3.10+)
+  Python's missing algorave module. Hackable live coding tool for modern Python (3.10+)
 </i></p>
 
 <p align="center">
   <img src=https://img.shields.io/discord/1029399269574193203 />
   <img src=https://img.shields.io/github/license/Bubobubobubobubo/sardine />
   <img src=https://img.shields.io/github/stars/Bubobubobubobubo/sardine />
+  <img src=https://img.shields.io/pypi/wheel/sardine-system>
+  <img src=https://img.shields.io/pypi/v/sardine-system>
+  <img src=https://img.shields.io/pypi/status/sardine-system>
 </p>
 
 <p align="center">
   <a href="https://discord.gg/aPgV7mSFZh">Discord</a> |
   <a href="https://sardine.raphaelforment.fr/">Website</a> |
-  <a href="https://sardine.raphaelforment.fr/documentation/sardinopedia/introduction/">Examples</a> |
-  <a href="https://sardine.raphaelforment.fr/technical/installation/">Installation</a> |
+  <a href="https://sardine.raphaelforment.fr/showcase">Examples</a> |
+  <a href="https://sardine.raphaelforment.fr/installation/">Installation</a> |
   <a href="https://raphaelforment.fr/">Author</a>  |
   <a href="https://toplap.org/">About Live Coding</a>
   <br><br>
   <p align='center'>
     <a href="https://github.com/bubobubobubobubo/sardine/graphs/contributors">
     <img src="https://contrib.rocks/image?repo=bubobubobubobubo/sardine" />
     </a>
   </p>
 </p>
 
 -----------
 
 ![Sardine algorave picture](pictures/sardine_intro_picture_repo.png)
 
-Sardine is a hacker-friendly Python library tailored for musical improvisation,
-algorithmic composition and much more. **Sardine** is transforming your typical
-**Python** interpreter into a music instrument that allows you to write melodic
-and rhythmic patterns of any kind and to map them to any electronic instrument:
-**MIDI**, **OSC** and/or **SuperCollider**. Using **Sardine**, you can:
-
-- **Improvise music freely on stage / in the studio / for your own enjoyment.**
-  - **Sardine** can talk to any MIDI/OSC device and to the **SuperCollider**
-    audio engine.
-  - Bindings for **SuperDirt**, a well-known synthesis engine used by
-    live coders around the world.
-- **Build complex and rich audio/visual installations using MIDI and OSC *I/O*.**
-  - Attach **callbacks** to any OSC event, turn **Sardine** into a complex
-    reactive toolbox.
-  - Watch values as they change and propagate them to your musical patterns or code.
-- **Synchronise with other computers / other musical instruments**
-  - **MIDI Clock** Out.
-  - **Link Protocol** synchronization.
-- **Make Python code time-aware**
-  - Using temporal recursion, you can make any Python code time and tempo aware.
-  - Launch any sync or async function precisely in time,
-    with results falling back on time.
-  - Hack your own **Senders** or **Receivers** to pattern whatever you see fit!
+**Sardine** is a versatile and hacker-friendly Python library designed for musical improvisation, algorithmic composition, and beyond.
+It transforms your standard **Python** interpreter into a powerful music instrument, enabling you to create and map melodic and rhythmic
+patterns to any electronic instrument (**MIDI**, **OSC**, and **SuperCollider**).
+With **Sardine**, you can:
+
+- **Unleash your musical creativity on stage, in the studio, or for personal enjoyment**
+  - Seamlessly communicate with any MIDI/OSC device and the **SuperCollider** audio engine using **Sardine**.
+  - Utilize bindings for **SuperDirt**, a widely recognized synthesis engine embraced by live coders globally.
+
+- **Empower your Python code with time-aware capabilities**
+  - Employ temporal recursion to make any Python code time and tempo aware.
+  - Accurately launch synchronous or asynchronous functions with time-specific results.
+  - Customize your own **Senders** or **Receivers** to pattern any desired elements!
+
+- **Develop intricate audio/visual installations with MIDI and OSC *I/O***
+  - Assign **callbacks** to any OSC event, transforming **Sardine** into a sophisticated reactive toolbox.
+  - Monitor changing values and incorporate them into your musical patterns or code.
+
+- **Synchronize with other computers and musical instruments**
+  - Synchronise your hardware with **MIDI Clocks**.
+  - Synchronize effortlessly with other tools or players using the **Link Protocol**.
 
 ## Installation
 
-In order to install Sardine, your system will require a recent version of Python (3.10+). We now support 3.11 versions as well. A more detailed installation guide can be found on [Sardine's website](https://sardine.raphaelforment.fr/technical/installation/).
-
-1) Run: `python -m pip install --find-links https://thegamecracks.github.io/python-rtmidi-wheels/ sardine-system`.
-    - the `--find-links` option is used as a temporary fix to the unavailability of some dependencies in the Pypi repositories for Python 3.10/3.11.
-2) Install [SuperCollider](https://supercollider.github.io/) and [SuperDirt](https://github.com/musikinformatik/SuperDirt) for an additional supported audio backend.
-3) Run `sardine-config` and configure Sardine to your liking following [this guide](https://sardine.raphaelforment.fr/technical/configuration/)
-4) Install the text editor of your choice: VSCode, Neovim, Vim, Emacs, Jupyter Notebook, etc... There are many options you can pick from. They have all been tested with Sardine.
+Refer to the [installation section](https://sardine.raphaelforment.fr/installation.html).
 
 ## Contributions
 
-Sardine is currently in the early development phase. We are looking for contributors! Anybody is welcome to contribute with code / documentation / thoughts, etc... You can contact the **Sardine** community directly on **Discord** or **PM** me if you have specific questions.
-
-### Documenting Sardine
-
-**Sardine** is a **Python** library that you learn to use as a musical instrument. For this reason, documentation is of paramount importance so that others can learn your cool tricks too :). The documentation resides in the `docs/` folder. It is a bunch of loosely organised Markdown files. You can contribute by editing these files and adding the missing bit of information you would like to see being updated or added.
+Sardine is in its early stages of development, and we're actively seeking contributors to help enhance the project. If you're passionate
+about music and technology, we welcome your expertise, whether it's code, documentation, or ideas. We are looking for contributors! 
 
-Source code is contained to the `sardine/` and `fishery/` folder. Most functions are already documented but the architecture of **Sardine** needs some time to get used to. You can contact me directly if you would like to learn more about it. There are no contributions rules for the moment, and I will explore each and every request that you would like to propose!
+To collaborate with the Sardine community, connect with us on **Discord**, **Github** or send a private message if you have specific inquiries.
+Together, we can create an even more powerful tool for musical expression and creativity!
```

#### html2text {}

```diff
@@ -1,83 +1,58 @@
-Metadata-Version: 2.1 Name: sardine-system Version: 0.2.1 Summary: Python's
-missing algorave module Project-URL: Homepage, https://
+Metadata-Version: 2.1 Name: sardine-system Version: 0.4.0 Summary: Python's
+missing algorave module Author: RaphaÃ«l Forment, thegamecracks Author-email:
+raphael.forment@gmail.com License: GPL-3.0-only Project-URL: Homepage, https://
 sardine.raphaelforment.fr Project-URL: Documentation, https://
 sardine.raphaelforment.fr Project-URL: Source Code, https://github.com/
 Bubobubobubobubo/sardine Project-URL: Bug Tracker, https://github.com/
-Bubobubobubobubo/sardine/issues Author: RaphaÃ«l Forment, thegamecracks Author-
-email: raphael.forment@gmail.com License-File: LICENSE.txt Keywords:
-algorave,live-coding,music,patterns Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: AsyncIO Classifier: Intended Audience :: End Users/
-Desktop Classifier: Intended Audience :: Science/Research Classifier: License
-:: OSI Approved Classifier: License :: OSI Approved :: GNU General Public
-License v3 (GPLv3) Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Artistic Software Classifier: Topic :: Multimedia Classifier: Topic ::
-Multimedia :: Sound/Audio Classifier: Topic :: Multimedia :: Sound/Audio ::
-MIDI Requires-Python: >=3.10 Requires-Dist: appdirs>=1.4 Requires-Dist:
-click>=8.1.3 Requires-Dist: easing-functions>=1.0.4 Requires-Dist:
-exceptiongroup>=1.0.4 Requires-Dist: inquirerpy>=0.3.4 Requires-Dist: lark>=1.1
-Requires-Dist: linkpython-extern>=1.0.2 Requires-Dist: mido>=1.2 Requires-Dist:
-osc4py3>=1.0.8 Requires-Dist: psutil>=5.9 Requires-Dist: python-rtmidi>=1.4.9
-Requires-Dist: rich>=12.5 Requires-Dist: uvloop>=0.16; sys_platform != 'win32'
-Provides-Extra: dev Requires-Dist: black>=22.8; extra == 'dev' Requires-Dist:
-pylint>=2.15; extra == 'dev' Requires-Dist: pytest-asyncio>=0.20.2; extra ==
-'dev' Requires-Dist: pytest>=7.2.0; extra == 'dev' Provides-Extra: profile
-Requires-Dist: yappi>=1.4.0; extra == 'profile' Description-Content-Type: text/
-markdown
+Bubobubobubobubo/sardine/issues Keywords: algorave,live-coding,music,patterns
+Classifier: Development Status :: 3 - Alpha Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Artistic Software Classifier:
+Topic :: Multimedia Classifier: Topic :: Multimedia :: Sound/Audio Classifier:
+Topic :: Multimedia :: Sound/Audio :: MIDI Requires-Python: >=3.10 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: profile
+License-File: LICENSE.txt
           ***** Sardine: â¨ Live Coding Library for Python â¨ *****
- Python's missing algorave module. Simple/hackable live coding tool for modern
-                                Python (3.10+)
+Python's missing algorave module. Hackable live coding tool for modern Python
+                                    (3.10+)
  [https://img.shields.io/discord/1029399269574193203] [https://img.shields.io/
 github/license/Bubobubobubobubo/sardine] [https://img.shields.io/github/stars/
-                           Bubobubobubobubo/sardine]
+ Bubobubobubobubo/sardine] [https://img.shields.io/pypi/wheel/sardine-system]
+ [https://img.shields.io/pypi/v/sardine-system] [https://img.shields.io/pypi/
+                            status/sardine-system]
    Discord | Website | Examples | Installation | Author | About_Live_Coding
 
           [https://contrib.rocks/image?repo=bubobubobubobubo/sardine]
 ----------- ![Sardine algorave picture](pictures/
-sardine_intro_picture_repo.png) Sardine is a hacker-friendly Python library
-tailored for musical improvisation, algorithmic composition and much more.
-**Sardine** is transforming your typical **Python** interpreter into a music
-instrument that allows you to write melodic and rhythmic patterns of any kind
-and to map them to any electronic instrument: **MIDI**, **OSC** and/or
-**SuperCollider**. Using **Sardine**, you can: - **Improvise music freely on
-stage / in the studio / for your own enjoyment.** - **Sardine** can talk to any
-MIDI/OSC device and to the **SuperCollider** audio engine. - Bindings for
-**SuperDirt**, a well-known synthesis engine used by live coders around the
-world. - **Build complex and rich audio/visual installations using MIDI and OSC
-*I/O*.** - Attach **callbacks** to any OSC event, turn **Sardine** into a
-complex reactive toolbox. - Watch values as they change and propagate them to
-your musical patterns or code. - **Synchronise with other computers / other
-musical instruments** - **MIDI Clock** Out. - **Link Protocol**
-synchronization. - **Make Python code time-aware** - Using temporal recursion,
-you can make any Python code time and tempo aware. - Launch any sync or async
-function precisely in time, with results falling back on time. - Hack your own
-**Senders** or **Receivers** to pattern whatever you see fit! ## Installation
-In order to install Sardine, your system will require a recent version of
-Python (3.10+). We now support 3.11 versions as well. A more detailed
-installation guide can be found on [Sardine's website](https://
-sardine.raphaelforment.fr/technical/installation/). 1) Run: `python -m pip
-install --find-links https://thegamecracks.github.io/python-rtmidi-wheels/
-sardine-system`. - the `--find-links` option is used as a temporary fix to the
-unavailability of some dependencies in the Pypi repositories for Python 3.10/
-3.11. 2) Install [SuperCollider](https://supercollider.github.io/) and
-[SuperDirt](https://github.com/musikinformatik/SuperDirt) for an additional
-supported audio backend. 3) Run `sardine-config` and configure Sardine to your
-liking following [this guide](https://sardine.raphaelforment.fr/technical/
-configuration/) 4) Install the text editor of your choice: VSCode, Neovim, Vim,
-Emacs, Jupyter Notebook, etc... There are many options you can pick from. They
-have all been tested with Sardine. ## Contributions Sardine is currently in the
-early development phase. We are looking for contributors! Anybody is welcome to
-contribute with code / documentation / thoughts, etc... You can contact the
-**Sardine** community directly on **Discord** or **PM** me if you have specific
-questions. ### Documenting Sardine **Sardine** is a **Python** library that you
-learn to use as a musical instrument. For this reason, documentation is of
-paramount importance so that others can learn your cool tricks too :). The
-documentation resides in the `docs/` folder. It is a bunch of loosely organised
-Markdown files. You can contribute by editing these files and adding the
-missing bit of information you would like to see being updated or added. Source
-code is contained to the `sardine/` and `fishery/` folder. Most functions are
-already documented but the architecture of **Sardine** needs some time to get
-used to. You can contact me directly if you would like to learn more about it.
-There are no contributions rules for the moment, and I will explore each and
-every request that you would like to propose!
+sardine_intro_picture_repo.png) **Sardine** is a versatile and hacker-friendly
+Python library designed for musical improvisation, algorithmic composition, and
+beyond. It transforms your standard **Python** interpreter into a powerful
+music instrument, enabling you to create and map melodic and rhythmic patterns
+to any electronic instrument (**MIDI**, **OSC**, and **SuperCollider**). With
+**Sardine**, you can: - **Unleash your musical creativity on stage, in the
+studio, or for personal enjoyment** - Seamlessly communicate with any MIDI/OSC
+device and the **SuperCollider** audio engine using **Sardine**. - Utilize
+bindings for **SuperDirt**, a widely recognized synthesis engine embraced by
+live coders globally. - **Empower your Python code with time-aware
+capabilities** - Employ temporal recursion to make any Python code time and
+tempo aware. - Accurately launch synchronous or asynchronous functions with
+time-specific results. - Customize your own **Senders** or **Receivers** to
+pattern any desired elements! - **Develop intricate audio/visual installations
+with MIDI and OSC *I/O*** - Assign **callbacks** to any OSC event, transforming
+**Sardine** into a sophisticated reactive toolbox. - Monitor changing values
+and incorporate them into your musical patterns or code. - **Synchronize with
+other computers and musical instruments** - Synchronise your hardware with
+**MIDI Clocks**. - Synchronize effortlessly with other tools or players using
+the **Link Protocol**. ## Installation Refer to the [installation section]
+(https://sardine.raphaelforment.fr/installation.html). ## Contributions Sardine
+is in its early stages of development, and we're actively seeking contributors
+to help enhance the project. If you're passionate about music and technology,
+we welcome your expertise, whether it's code, documentation, or ideas. We are
+looking for contributors! To collaborate with the Sardine community, connect
+with us on **Discord**, **Github** or send a private message if you have
+specific inquiries. Together, we can create an even more powerful tool for
+musical expression and creativity!
```

