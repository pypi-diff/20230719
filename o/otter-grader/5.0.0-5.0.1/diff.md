# Comparing `tmp/otter-grader-5.0.0.tar.gz` & `tmp/otter-grader-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter-grader-5.0.0.tar", last modified: Tue Jul 18 03:45:31 2023, max compression
+gzip compressed data, was "otter-grader-5.0.1.tar", last modified: Wed Jul 19 03:36:39 2023, max compression
```

## Comparing `otter-grader-5.0.0.tar` & `otter-grader-5.0.1.tar`

### file list

```diff
@@ -1,198 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.904800 otter-grader-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-18 03:45:03.000000 otter-grader-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-18 03:45:03.000000 otter-grader-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-18 03:45:31.904800 otter-grader-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-18 03:45:03.000000 otter-grader-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.888800 otter-grader-5.0.0/otter/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/feature_toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/question_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/r_adapter/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/r_adapter/rmarkdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/r_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/r_adapter/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/v0/
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/cell_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/v0/convert/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/convert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/convert/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/v0/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/r_adapter/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/check/
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/check/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/check/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/check/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/check/validate_export/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/check/validate_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/check/validate_export/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/execute/
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/execute_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/execute_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/base_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/exporters/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/exporters/templates/via_html/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_html/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_html/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_html.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/exporters/templates/via_latex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/export/exporters/via_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/export/exporters/via_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/generate/
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.888800 otter-grader-5.0.0/otter/generate/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/generate/templates/common/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/common/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/common/run_otter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/generate/templates/python/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/python/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/python/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/python/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/python/run_otter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/python/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/generate/templates/r/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/requirements.r
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/run_otter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/generate/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/grade/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/grade/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/grade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/grade/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/grade/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/plugins/abstract_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/plugins/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/grade_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/otter/run/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/otter/run/run_autograder/
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/run/run_autograder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/run/run_autograder/autograder_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/otter/run/run_autograder/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/run/run_autograder/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/run/run_autograder/runners/abstract_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/run/run_autograder/runners/python_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/run/run_autograder/runners/r_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/run/run_autograder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/otter/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/test_files/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/test_files/exception_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/test_files/metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/test_files/ok_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/test_files/ottr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/otter_grader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-18 03:45:30.000000 otter-grader-5.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:45:31.904800 otter-grader-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-18 03:45:04.000000 otter-grader-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/test_assign/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_assign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_assign/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_assign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/test_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_check/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_check/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_check/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    20296 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/test_execute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_execute/test_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_execute/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/test_export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_export/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/test_generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:04.000000 otter-grader-5.0.0/test/test_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_generate/test_autograder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-18 03:45:04.000000 otter-grader-5.0.0/test/test_generate/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_generate/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.904800 otter-grader-5.0.0/test/test_grade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_grade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_grade/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_grade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.904800 otter-grader-5.0.0/test/test_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_run/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 03:45:04.000000 otter-grader-5.0.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-19 03:36:10.000000 otter-grader-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-19 03:36:10.000000 otter-grader-5.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-19 03:36:39.489056 otter-grader-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-19 03:36:10.000000 otter-grader-5.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/assign/
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/feature_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/question_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/assign/r_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/r_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/r_adapter/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/r_adapter/rmarkdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/r_adapter/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/r_adapter/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/assign/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/check/validate_export/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/validate_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/check/validate_export/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/execute/
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-19 03:36:37.000000 otter-grader-5.0.1/otter/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/execute/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/execute/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/export/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/base_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/export/exporters/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/export/exporters/templates/via_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_html/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_html/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_html.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.481056 otter-grader-5.0.1/otter/export/exporters/templates/via_latex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/via_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/exporters/via_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/export/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.477056 otter-grader-5.0.1/otter/generate/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/generate/templates/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/templates/common/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/templates/common/run_otter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/generate/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/templates/python/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/generate/templates/r/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/templates/r/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/generate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/grade/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/grade/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/grade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/grade/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/grade/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/abstract_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/plugins/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/grade_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/plugins/builtin/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/run/run_autograder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/autograder_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/run/run_autograder/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/runners/abstract_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/runners/python_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/runners/r_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/run/run_autograder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.485056 otter-grader-5.0.1/otter/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/exception_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/ok_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/test_files/ottr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-19 03:36:10.000000 otter-grader-5.0.1/otter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-19 03:36:37.000000 otter-grader-5.0.1/otter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/otter_grader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 03:36:39.000000 otter-grader-5.0.1/otter_grader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-19 03:36:37.000000 otter-grader-5.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 03:36:39.489056 otter-grader-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-19 03:36:10.000000 otter-grader-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_assign/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_assign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_assign/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_check/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_check/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_check/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20296 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_execute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_execute/test_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_execute/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_export/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_generate/test_autograder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_generate/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_generate/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_grade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_grade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_grade/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:39.489056 otter-grader-5.0.1/test/test_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_run/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 03:36:10.000000 otter-grader-5.0.1/test/test_utils.py
```

### Comparing `otter-grader-5.0.0/LICENSE` & `otter-grader-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/PKG-INFO` & `otter-grader-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 5.0.0
+Version: 5.0.1
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-5.0.0/README.md` & `otter-grader-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/api.py` & `otter-grader-5.0.1/otter/api.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/__init__.py` & `otter-grader-5.0.1/otter/assign/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/assignment.py` & `otter-grader-5.0.1/otter/assign/assignment.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/blocks.py` & `otter-grader-5.0.1/otter/assign/blocks.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/cell_factory.py` & `otter-grader-5.0.1/otter/assign/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/feature_toggle.py` & `otter-grader-5.0.1/otter/assign/feature_toggle.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/notebook_transformer.py` & `otter-grader-5.0.1/otter/assign/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/output.py` & `otter-grader-5.0.1/otter/assign/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/plugins.py` & `otter-grader-5.0.1/otter/assign/plugins.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/question_config.py` & `otter-grader-5.0.1/otter/assign/question_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/r_adapter/cell_factory.py` & `otter-grader-5.0.1/otter/assign/r_adapter/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/r_adapter/rmarkdown_converter.py` & `otter-grader-5.0.1/otter/assign/r_adapter/rmarkdown_converter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/r_adapter/solutions.py` & `otter-grader-5.0.1/otter/assign/r_adapter/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/r_adapter/tests_manager.py` & `otter-grader-5.0.1/otter/assign/r_adapter/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/solutions.py` & `otter-grader-5.0.1/otter/assign/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/tests_manager.py` & `otter-grader-5.0.1/otter/assign/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/utils.py` & `otter-grader-5.0.1/otter/assign/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/assign/v0/r_adapter/tests.py` & `otter-grader-5.0.1/otter/test_files/metadata_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,137 +1,136 @@
-"""
-ottr test adapters for Otter Assign
-"""
+"""Support for notebook metadata test files"""
 
-import re
-import pprint
-import yaml
-import nbformat
+import json
 
-from collections import namedtuple
-from dataclasses import dataclass, replace
-from typing import Optional, Union
+from .exception_test import ExceptionTestFile
+from .ok_test import OKTestFile
 
-from ..constants import TEST_REGEX, OTTR_TEST_NAME_REGEX, OTTR_TEST_FILE_TEMPLATE
-from ..tests import write_test
-from ..utils import get_source, lock
+from ..utils import NOTEBOOK_METADATA_KEY
 
-Test = namedtuple('Test', ['name', 'hidden', 'points', 'body', 'success_message', 'failure_message'])
 
-@dataclass
-class Test:
-
-    name: str
-
-    hidden: bool
-
-    points: Union[int, float]
-
-    body: str
-
-    success_message: Optional[str]
-
-    failure_message: Optional[str]
-
-
-def read_test(cell, question, assignment, rmd=False):
-    """
-    Returns the contents of a test as a ``(name, hidden, body)`` named tuple
-
-    Args:
-        cell (``nbformat.NotebookNode``): a test cell
-        question (``dict``): question metadata
-        assignment (``otter.assign.assignment.Assignment``): the assignment configurations
-        rmd (``bool``, optional): whether the cell is from an Rmd file; if true, the first and last
-            lines of ``cell``'s source are trimmed, since they should be backtick delimeters
-
-    Returns:
-        ``Test``: test named tuple
+class NotebookMetadataExceptionTestFile(ExceptionTestFile):
     """
-    if rmd:
-        source = get_source(cell)[1:-1]
-    else:
-        source = get_source(cell)
-    hidden = bool(re.search("hidden", source[0], flags=re.IGNORECASE))
-    lines = source[1:]
-    test_name = None
-    # for line in lines:
-    #     match = re.match(OTTR_TEST_NAME_REGEX, line)
-    #     if match:
-    #         test_name = match.group(1)
-    #         break
-    # assert test_name is not None, f"Could not parse test name:\n{cell}"
-    # TODO: hook up success_message and failure_message
-    # TODO: add parsing for TEST CONFIG blocks
-    return Test(test_name, hidden, None, '\n'.join(lines), "", "")
+    A single notebook metadata test file for Otter.
 
-def gen_test_cell(question, tests, tests_dict, assignment):
-    """
-    Parses a list of test named tuples and creates a single test file. Adds this test file as a value
-    to ``tests_dict`` with a key corresponding to the test's name, taken from ``question``. Returns
-    a code cell that runs the check on this test.
-
-    Args:
-        question (``dict``): question metadata
-        tests (``list`` of ``Test``): tests to be written
-        tests_dict (``dict``): the tests for this assignment
-        assignment (``otter.assign.assignment.Assignment``): the assignment configurations
+    Tests are defined in the metadata of a jupyter notebook as a JSON object with the ``otter`` key.
+    The tests themselves are assumed to be base-64-encoded compiled ``code`` objects from test files.
 
-    Returns:
-        ``nbformat.NotebookNode``: code cell calling ``ottr::check`` on this test
-    """
-    cell = nbformat.v4.new_code_cell()
-    cell.source = ['. = ottr::check("tests/{}.R")'.format(question['name'])]
-
-    points = question.get('points', len(tests))
-    if isinstance(points, (int, float)):
-        if points % len(tests) == 0:
-            points = [points // len(tests) for _ in range(len(tests))]
-        else:
-            points = [points / len(tests) for _ in range(len(tests))]
-    assert isinstance(points, list) and len(points) == len(tests), \
-        f"Points for question {question['name']} could not be parsed:\n{points}"
-
-    # update point values
-    tests = [replace(tc, points=p) for tc, p in zip(tests, points)]
-    test = gen_suite(question['name'], tests, points)
-
-    tests_dict[question['name']] = test
-    lock(cell)
-    return cell
+    .. code-block:: json
 
-def gen_suite(name, tests, points):
-    """
-    Generates an R-formatted test file for ottr
+    {
+        "metadata": {
+            "otter": {
+                "tests": {
+                    "q1": ""
+                }
+            }
+        }
+    }
 
     Args:
-        name (``str``): the test name
-        tests (``list`` of ``Test``): the test case named tuples that define this test file
-        points (``float`` or ``int`` or ``list`` of ``float`` or ``int``): th points per question
-
-    Returns:
-        ``str``: the rendered R test file
-    """
-    template_data = {'name': name, 'test_cases': tests}
-    return OTTR_TEST_FILE_TEMPLATE.render(**template_data)
-
-def remove_hidden_tests_from_dir(nb, test_dir, assignment, use_files=True):
-    """
-    Rewrites test files in a directory to remove hidden tests
+        name (``str``): the name of test file
+        path (``str``): the path to the test file
+        test_cases (``list`` of ``TestCase``): a list of parsed tests to be run
+        value (``int``, optional): the point value of this test, defaults to 1
+        all_or_nothing (``bool``, optional): whether the test should be graded all-or-nothing across
+            cases
+
+    Attributes:
+        name (``str``): the name of test file
+        path (``str``): the path to the test file
+        test_cases (``list`` of ``TestCase``): a list of parsed tests to be run
+        value (``int``): the point value of this test, defaults to 1
+        all_or_nothing (``bool``): whether the test should be graded all-or-nothing across
+            cases
+        passed_all (``bool``): whether all of the test cases were passed
+        test_case_results (``list`` of ``TestCaseResult``): a list of results for the test cases in
+            ``test_cases``
+        grade (``float``): the percentage of ``points`` earned for this test file as a decimal
+    """
+
+    @classmethod
+    def from_file(cls, path, test_name):
+        """
+        Parse an exception-based test from a Jupyter notebook's metadata and return an 
+        ``ExceptionTestFile``.
+
+        Args:
+            path (``str``): the path to the notebook
+            test_name (``str``): the name of the test to extract from the metadata
+
+        Returns:
+            ``ExceptionTestFile``: the new ``ExceptionTestFile`` object created from the given file
+        """
+        with open(path, encoding="utf-8") as f:
+            nb = json.load(f)
+
+        test_spec = nb["metadata"][NOTEBOOK_METADATA_KEY]["tests"]
+        if test_name not in test_spec:
+            raise ValueError(f"Test {test_name} not found")
+
+        test_spec = test_spec[test_name]
+        return cls.from_string(test_spec, path=path)
+
+
+class NotebookMetadataOKTestFile(OKTestFile):
+    """
+    A single notebook metadata test file for Otter.
+
+    Tests are defined in the metadata of a jupyter notebook as a JSON object with the ``otter`` key.
+    The tests themselves are OK-formatted.
+
+    .. code-block:: json
+
+    {
+        "metadata": {
+            "otter": {
+                "tests": {
+                    "q1": {}
+                }
+            }
+        }
+    }
 
     Args:
-        nb (``nbformat.NotebookNode``): the student notebook
-        test_dir (``pathlib.Path``): path to test files directory
-        assignment (``otter.assign.assignment.Assignment``): the assignment configurations
-        use_files (``bool``, optional): ignored for R assignments
-    """
-    for f in test_dir.iterdir():
-        if f.suffix != '.R':
-            continue
-
-        with open(f) as f2:
-            test = f2.read()
+        name (``str``): the name of test file
+        path (``str``): the path to the test file
+        test_cases (``list`` of ``TestCase``): a list of parsed tests to be run
+        value (``int``, optional): the point value of this test, defaults to 1
+        all_or_nothing (``bool``, optional): whether the test should be graded all-or-nothing across
+            cases
+
+    Attributes:
+        name (``str``): the name of test file
+        path (``str``): the path to the test file
+        test_cases (``list`` of ``TestCase``): a list of parsed tests to be run
+        value (``int``): the point value of this test, defaults to 1
+        all_or_nothing (``bool``): whether the test should be graded all-or-nothing across
+            cases
+        passed_all (``bool``): whether all of the test cases were passed
+        test_case_results (``list`` of ``TestCaseResult``): a list of results for the test cases in
+            ``test_cases``
+        grade (``float``): the percentage of ``points`` earned for this test file as a decimal
+    """
+
+    @classmethod
+    def from_file(cls, path, test_name):
+        """
+        Parse an OK-formatted test from a Jupyter notebook's metadata and return an ``OKTestFile``.
+
+        Args:
+            path (``str``): the path to the notebook
+            test_name (``str``): the name of the test to extract from the metadata
+
+        Returns:
+            ``OKTestFile``: the new ``OKTestFile`` object created from the given file
+        """
+        with open(path, encoding="utf-8") as f:
+            nb = json.load(f)
+
+        test_spec = nb["metadata"][NOTEBOOK_METADATA_KEY]["tests"]
+        if test_name not in test_spec:
+            raise ValueError(f"Test {test_name} not found")
 
-        test = re.sub(r"    ottr::TestCase\$new\(\s*hidden = TRUE[\w\W]+?^    \),?", "", test, flags=re.MULTILINE)
-        test = re.sub(r",(\s*  \))", r"\1", test, flags=re.MULTILINE)  # removes a trailing comma if present
+        test_spec = test_spec[test_name]
 
-        write_test({}, f, test, use_file=True)
+        return cls.from_spec(test_spec, path=path)
```

### Comparing `otter-grader-5.0.0/otter/check/__init__.py` & `otter-grader-5.0.1/otter/check/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/check/logs.py` & `otter-grader-5.0.1/otter/check/logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/check/notebook.py` & `otter-grader-5.0.1/otter/check/notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/check/utils.py` & `otter-grader-5.0.1/otter/check/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/check/validate_export/__main__.py` & `otter-grader-5.0.1/otter/check/validate_export/__main__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/cli.py` & `otter-grader-5.0.1/otter/cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/execute/__init__.py` & `otter-grader-5.0.1/otter/execute/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Execution and grading internals for Otter-Grader"""
 
 import nbformat
 import pickle
 import tempfile
 
-from nbconvert.preprocessors import ExecutePreprocessor
 from traitlets.config import Config
 
 from .checker import Checker
 from .preprocessor import GradingPreprocessor
 
 from ..test_files import GradingResults
 from ..utils import NBFORMAT_VERSION
@@ -49,14 +48,16 @@
             checking values deserialized from ``log``
         plugin_collection (``otter.plugins.PluginCollection``): a set of plugins to run the
             ``before_execution`` and ``after_grading`` events on this submission
 
     Returns:
         ``otter.test_files.GradingResults``: the results of grading
     """
+    from nbconvert.preprocessors import ExecutePreprocessor
+
     if not script:
         nb = nbformat.read(submission_path, as_version=NBFORMAT_VERSION)
 
     else:
         with open(submission_path) as f:
             nb = f.read()
```

### Comparing `otter-grader-5.0.0/otter/execute/checker.py` & `otter-grader-5.0.1/otter/execute/checker.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/execute/preprocessor.py` & `otter-grader-5.0.1/otter/execute/preprocessor.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/__init__.py` & `otter-grader-5.0.1/otter/export/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/exporters/__init__.py` & `otter-grader-5.0.1/otter/export/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/exporters/base_exporter.py` & `otter-grader-5.0.1/otter/export/exporters/base_exporter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/exporters/templates/via_html/index.html.j2` & `otter-grader-5.0.1/otter/export/exporters/templates/via_html/index.html.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/exporters/templates/via_html.tpl` & `otter-grader-5.0.1/otter/export/exporters/templates/via_html.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/exporters/templates/via_latex/index.tex.j2` & `otter-grader-5.0.1/otter/export/exporters/templates/via_latex/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/exporters/templates/via_latex.tpl` & `otter-grader-5.0.1/otter/export/exporters/templates/via_latex.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2` & `otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk.tpl` & `otter-grader-5.0.1/otter/export/exporters/templates/via_latex_xecjk.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/exporters/utils.py` & `otter-grader-5.0.1/otter/export/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/exporters/via_html.py` & `otter-grader-5.0.1/otter/export/exporters/via_html.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/export/exporters/via_latex.py` & `otter-grader-5.0.1/otter/export/exporters/via_latex.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/generate/__init__.py` & `otter-grader-5.0.1/otter/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/generate/templates/python/setup.sh` & `otter-grader-5.0.1/otter/generate/templates/python/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/generate/templates/r/setup.sh` & `otter-grader-5.0.1/otter/generate/templates/r/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/generate/token.py` & `otter-grader-5.0.1/otter/generate/token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/generate/utils.py` & `otter-grader-5.0.1/otter/generate/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/grade/Dockerfile` & `otter-grader-5.0.1/otter/grade/Dockerfile`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/grade/__init__.py` & `otter-grader-5.0.1/otter/grade/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/grade/containers.py` & `otter-grader-5.0.1/otter/grade/containers.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/grade/utils.py` & `otter-grader-5.0.1/otter/grade/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/plugins/__init__.py` & `otter-grader-5.0.1/otter/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/plugins/abstract_plugin.py` & `otter-grader-5.0.1/otter/plugins/abstract_plugin.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/__init__.py` & `otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py` & `otter-grader-5.0.1/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/plugins/builtin/grade_override.py` & `otter-grader-5.0.1/otter/plugins/builtin/grade_override.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/plugins/builtin/rate_limiting.py` & `otter-grader-5.0.1/otter/plugins/builtin/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/run/__init__.py` & `otter-grader-5.0.1/otter/run/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/run/run_autograder/__init__.py` & `otter-grader-5.0.1/otter/run/run_autograder/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/run/run_autograder/autograder_config.py` & `otter-grader-5.0.1/otter/run/run_autograder/autograder_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/run/run_autograder/runners/__init__.py` & `otter-grader-5.0.1/otter/run/run_autograder/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/run/run_autograder/runners/abstract_runner.py` & `otter-grader-5.0.1/otter/run/run_autograder/runners/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/run/run_autograder/runners/python_runner.py` & `otter-grader-5.0.1/otter/run/run_autograder/runners/python_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/run/run_autograder/runners/r_runner.py` & `otter-grader-5.0.1/otter/run/run_autograder/runners/r_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/test_files/__init__.py` & `otter-grader-5.0.1/otter/test_files/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/test_files/abstract_test.py` & `otter-grader-5.0.1/otter/test_files/abstract_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/test_files/exception_test.py` & `otter-grader-5.0.1/otter/test_files/exception_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/test_files/ok_test.py` & `otter-grader-5.0.1/otter/test_files/ok_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/utils.py` & `otter-grader-5.0.1/otter/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/otter/version.py` & `otter-grader-5.0.1/otter/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Version and printable logo"""
 
 import sys
 
 from textwrap import dedent
 
 
-__version__ = "5.0.0"
+__version__ = "5.0.1"
 
 
 LOGO_WITH_VERSION = fr"""
   _________        __          __               
  /  _____  \    __|  |__    __|  |__               
 |  /     \  |  |__    __|  |__    __|   _______    _  _____
 | |       | |     |  |        |  |     |  ___  |  | |/ ____|
```

### Comparing `otter-grader-5.0.0/otter_grader.egg-info/PKG-INFO` & `otter-grader-5.0.1/otter_grader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 5.0.0
+Version: 5.0.1
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-5.0.0/otter_grader.egg-info/SOURCES.txt` & `otter-grader-5.0.1/otter_grader.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -22,49 +22,23 @@
 otter/assign/tests_manager.py
 otter/assign/utils.py
 otter/assign/r_adapter/__init__.py
 otter/assign/r_adapter/cell_factory.py
 otter/assign/r_adapter/rmarkdown_converter.py
 otter/assign/r_adapter/solutions.py
 otter/assign/r_adapter/tests_manager.py
-otter/assign/v0/__init__.py
-otter/assign/v0/assignment.py
-otter/assign/v0/cell_generators.py
-otter/assign/v0/constants.py
-otter/assign/v0/notebook_transformer.py
-otter/assign/v0/output.py
-otter/assign/v0/plugins.py
-otter/assign/v0/questions.py
-otter/assign/v0/solutions.py
-otter/assign/v0/tests.py
-otter/assign/v0/utils.py
-otter/assign/v0/convert/__init__.py
-otter/assign/v0/convert/__main__.py
-otter/assign/v0/convert/notebook_transformer.py
-otter/assign/v0/r_adapter/__init__.py
-otter/assign/v0/r_adapter/tests.py
-otter/assign/v0/rmarkdown_adapter/__init__.py
-otter/assign/v0/rmarkdown_adapter/constants.py
-otter/assign/v0/rmarkdown_adapter/notebook_transformer.py
-otter/assign/v0/rmarkdown_adapter/output.py
-otter/assign/v0/rmarkdown_adapter/solutions.py
-otter/assign/v0/rmarkdown_adapter/tests.py
-otter/assign/v0/rmarkdown_adapter/utils.py
 otter/check/__init__.py
 otter/check/logs.py
 otter/check/notebook.py
 otter/check/utils.py
 otter/check/validate_export/__init__.py
 otter/check/validate_export/__main__.py
 otter/execute/__init__.py
 otter/execute/checker.py
-otter/execute/execute_log.py
-otter/execute/execute_notebook.py
 otter/execute/preprocessor.py
-otter/execute/transforms.py
 otter/export/__init__.py
 otter/export/utils.py
 otter/export/exporters/__init__.py
 otter/export/exporters/base_exporter.py
 otter/export/exporters/utils.py
 otter/export/exporters/via_html.py
 otter/export/exporters/via_latex.py
@@ -78,24 +52,15 @@
 otter/export/exporters/templates/via_latex_xecjk/conf.json
 otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
 otter/generate/__init__.py
 otter/generate/token.py
 otter/generate/utils.py
 otter/generate/templates/common/run_autograder
 otter/generate/templates/common/run_otter.py
-otter/generate/templates/python/environment.yml
-otter/generate/templates/python/requirements.txt
-otter/generate/templates/python/run_autograder
-otter/generate/templates/python/run_otter.py
 otter/generate/templates/python/setup.sh
-otter/generate/templates/r/environment.yml
-otter/generate/templates/r/requirements.r
-otter/generate/templates/r/requirements.txt
-otter/generate/templates/r/run_autograder
-otter/generate/templates/r/run_otter.py
 otter/generate/templates/r/setup.sh
 otter/grade/Dockerfile
 otter/grade/__init__.py
 otter/grade/containers.py
 otter/grade/utils.py
 otter/plugins/__init__.py
 otter/plugins/abstract_plugin.py
@@ -122,22 +87,15 @@
 otter_grader.egg-info/PKG-INFO
 otter_grader.egg-info/SOURCES.txt
 otter_grader.egg-info/dependency_links.txt
 otter_grader.egg-info/entry_points.txt
 otter_grader.egg-info/requires.txt
 otter_grader.egg-info/top_level.txt
 test/test_api.py
-test/test_assign.py
-test/test_check.py
 test/test_cli.py
-test/test_export.py
-test/test_grade.py
-test/test_logs.py
-test/test_notebook.py
-test/test_run.py
 test/test_utils.py
 test/test_assign/__init__.py
 test/test_assign/test_integration.py
 test/test_check/__init__.py
 test/test_check/test_cli.py
 test/test_check/test_logs.py
 test/test_check/test_notebook.py
```

### Comparing `otter-grader-5.0.0/setup.py` & `otter-grader-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_api.py` & `otter-grader-5.0.1/test/test_api.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_assign/test_integration.py` & `otter-grader-5.0.1/test/test_assign/test_integration.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_check/test_cli.py` & `otter-grader-5.0.1/test/test_check/test_cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_check/test_logs.py` & `otter-grader-5.0.1/test/test_check/test_logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_check/test_notebook.py` & `otter-grader-5.0.1/test/test_check/test_notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_cli.py` & `otter-grader-5.0.1/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_execute/test_checker.py` & `otter-grader-5.0.1/test/test_execute/test_checker.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_execute/test_integration.py` & `otter-grader-5.0.1/test/test_execute/test_integration.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_export/test_integration.py` & `otter-grader-5.0.1/test/test_export/test_integration.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_generate/test_autograder.py` & `otter-grader-5.0.1/test/test_generate/test_autograder.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_generate/test_token.py` & `otter-grader-5.0.1/test/test_generate/test_token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_generate/test_utils.py` & `otter-grader-5.0.1/test/test_generate/test_utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_grade/test_integration.py` & `otter-grader-5.0.1/test/test_grade/test_integration.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.0/test/test_run/test_integration.py` & `otter-grader-5.0.1/test/test_run/test_integration.py`

 * *Files identical despite different names*

