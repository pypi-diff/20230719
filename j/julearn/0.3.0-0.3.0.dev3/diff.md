# Comparing `tmp/julearn-0.3.0.tar.gz` & `tmp/julearn-0.3.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julearn-0.3.0.tar", last modified: Wed Jul 19 12:22:36 2023, max compression
+gzip compressed data, was "julearn-0.3.0.dev3.tar", last modified: Wed Jul 19 12:19:19 2023, max compression
```

## Comparing `julearn-0.3.0.tar` & `julearn-0.3.0.dev3.tar`

### file list

```diff
@@ -1,282 +1,282 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.740053 julearn-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.708053 julearn-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.716053 julearn-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-19 12:22:27.000000 julearn-0.3.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 12:22:27.000000 julearn-0.3.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-19 12:22:27.000000 julearn-0.3.0/.github/ISSUE_TEMPLATE/documentation_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-19 12:22:27.000000 julearn-0.3.0/.github/ISSUE_TEMPLATE/feature_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.716053 julearn-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-19 12:22:27.000000 julearn-0.3.0/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-19 12:22:27.000000 julearn-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-19 12:22:27.000000 julearn-0.3.0/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-19 12:22:27.000000 julearn-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-19 12:22:27.000000 julearn-0.3.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-19 12:22:27.000000 julearn-0.3.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-19 12:22:27.000000 julearn-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-19 12:22:27.000000 julearn-0.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34353 2023-07-19 12:22:27.000000 julearn-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-19 12:22:36.740053 julearn-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-19 12:22:27.000000 julearn-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-19 12:22:27.000000 julearn-0.3.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.716053 julearn-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.708053 julearn-0.3.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.716053 julearn-0.3.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.716053 julearn-0.3.0/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.720053 julearn-0.3.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/_templates/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/_templates/function_warning.rst
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.720053 julearn-0.3.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/inspect.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/main.rst
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/model_selection.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/scoring.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/transformers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/api/viz.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/available_pipeline_steps.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.720053 julearn-0.3.0/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/changes/contributors.inc
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/changes/latest.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.720053 julearn-0.3.0/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/changes/newsfragments/151.bugfix
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/changes/newsfragments/170.enh
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/changes/newsfragments/47.feature
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/changes/v0.2.5.inc
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.724053 julearn-0.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    69241 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/corrected_ttest.png
--rw-r--r--   0 runner    (1001) docker     (123)    39468 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/final_estimator.png
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/iris_X.png
--rw-r--r--   0 runner    (1001) docker     (123)    51228 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/iris_df.png
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/iris_y.png
--rw-r--r--   0 runner    (1001) docker     (123)    54482 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/julearn_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    74874 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/julearn_logo_calm.png
--rw-r--r--   0 runner    (1001) docker     (123)    78884 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/julearn_logo_confbias.png
--rw-r--r--   0 runner    (1001) docker     (123)    61311 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/julearn_logo_cv.png
--rw-r--r--   0 runner    (1001) docker     (123)    73031 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/julearn_logo_generalization.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    60581 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/julearn_logo_it.png
--rw-r--r--   0 runner    (1001) docker     (123)    66833 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/julearn_logo_ml.png
--rw-r--r--   0 runner    (1001) docker     (123)    60581 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/julearn_logo_mlit.png
--rw-r--r--   0 runner    (1001) docker     (123)    94858 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/multiple_scorers_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (123)    84126 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/plot_scores.png
--rw-r--r--   0 runner    (1001) docker     (123)    43199 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/scores_run_cv.png
--rw-r--r--   0 runner    (1001) docker     (123)    83552 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/scores_run_cv_splitter.png
--rw-r--r--   0 runner    (1001) docker     (123)    47133 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/images/scores_run_cv_train.png
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.724053 julearn-0.3.0/docs/selected_deeper_topics/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/selected_deeper_topics/CBPM.rst
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/selected_deeper_topics/confound_removal.rst
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/selected_deeper_topics/cross_validation_splitter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/selected_deeper_topics/hyperparameter_tuning.rst
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/selected_deeper_topics/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/selected_deeper_topics/model_inspect.rst
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/selected_deeper_topics/stacked_models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/selected_deeper_topics/target_transformers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.724053 julearn-0.3.0/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/sphinxext/gh_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.724053 julearn-0.3.0/docs/what_really_need_know/
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/what_really_need_know/cross_validation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/what_really_need_know/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/what_really_need_know/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/what_really_need_know/model_comparison.rst
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/what_really_need_know/model_evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/what_really_need_know/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-19 12:22:27.000000 julearn-0.3.0/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.724053 julearn-0.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.728053 julearn-0.3.0/examples/00_starting/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/00_starting/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/00_starting/plot_cm_acc_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/00_starting/plot_example_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/00_starting/plot_stratified_kfold_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/00_starting/run_combine_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/00_starting/run_grouped_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/00_starting/run_simple_binary_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.728053 julearn-0.3.0/examples/01_model_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/01_model_comparison/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/01_model_comparison/plot_simple_model_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.728053 julearn-0.3.0/examples/02_inspection/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/02_inspection/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/02_inspection/plot_groupcv_inspect_svm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/02_inspection/plot_inspect_random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/02_inspection/plot_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/02_inspection/run_binary_inspect_folds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.728053 julearn-0.3.0/examples/03_complex_models/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/03_complex_models/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/03_complex_models/run_apply_to_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/03_complex_models/run_example_pca_featsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/03_complex_models/run_hyperparameter_multiple_grids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/03_complex_models/run_hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/03_complex_models/run_stacked_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.728053 julearn-0.3.0/examples/04_confounds/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/04_confounds/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/04_confounds/plot_confound_removal_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/04_confounds/run_return_confounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.728053 julearn-0.3.0/examples/05_customization/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/05_customization/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/05_customization/run_custom_scorers_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.732053 julearn-0.3.0/examples/99_docs/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/run_cbpm_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/run_confound_removal_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/run_cv_splitters_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/run_data_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/run_hyperparameters_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/run_model_comparison_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/run_model_evaluation_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/run_model_inspection_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15260 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/run_pipeline_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/run_stacked_models_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/99_docs/run_target_transformer_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.732053 julearn-0.3.0/examples/XX_disabled/
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/XX_disabled/dis_run_n_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-19 12:22:27.000000 julearn-0.3.0/examples/XX_disabled/dis_run_target_confound_removal.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 12:22:27.000000 julearn-0.3.0/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.732053 julearn-0.3.0/julearn/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-19 12:22:36.000000 julearn-0.3.0/julearn/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.732053 julearn-0.3.0/julearn/base/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/base/column_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/base/estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.732053 julearn-0.3.0/julearn/base/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/base/tests/test_base_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/base/tests/test_column_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.732053 julearn-0.3.0/julearn/inspect/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/inspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/inspect/_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/inspect/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/inspect/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/inspect/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.732053 julearn-0.3.0/julearn/inspect/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/inspect/tests/test_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/inspect/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/inspect/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/inspect/tests/test_preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.732053 julearn-0.3.0/julearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/model_selection/available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/model_selection/continuous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/model_selection/stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.732053 julearn-0.3.0/julearn/model_selection/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/model_selection/tests/test_available_searchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/model_selection/tests/test_continous_stratified_kfold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/model_selection/tests/test_stratified_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.736053 julearn-0.3.0/julearn/models/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/models/available_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/models/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.736053 julearn-0.3.0/julearn/models/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/models/tests/test_available_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/models/tests/test_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/models/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.736053 julearn-0.3.0/julearn/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/pipeline/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    32577 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/pipeline/pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/pipeline/target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/pipeline/target_pipeline_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.736053 julearn-0.3.0/julearn/pipeline/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/pipeline/test/test_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/pipeline/test/test_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/pipeline/test/test_target_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/pipeline/test/test_target_pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16536 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.736053 julearn-0.3.0/julearn/scoring/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/scoring/available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/scoring/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.736053 julearn-0.3.0/julearn/scoring/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/scoring/tests/test_available_scorers.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/scoring/tests/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.736053 julearn-0.3.0/julearn/stats/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/stats/corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.736053 julearn-0.3.0/julearn/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/stats/tests/test_corrected_ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.736053 julearn-0.3.0/julearn/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35890 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24535 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/tests/test_prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.736053 julearn-0.3.0/julearn/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/cbpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.740053 julearn-0.3.0/julearn/transformers/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/dataframe/change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/dataframe/drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/dataframe/filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/dataframe/set_column_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.740053 julearn-0.3.0/julearn/transformers/dataframe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/dataframe/tests/test_change_column_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/dataframe/tests/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/dataframe/tests/test_filter_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/dataframe/tests/test_set_column_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/ju_column_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.740053 julearn-0.3.0/julearn/transformers/target/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/target/available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/target/ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/target/ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/target/target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.740053 julearn-0.3.0/julearn/transformers/target/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/target/tests/test_available_target_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/target/tests/test_ju_target_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/target/tests/test_ju_transformed_target_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/target/tests/test_target_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.740053 julearn-0.3.0/julearn/transformers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/tests/test_available_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/tests/test_cbpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/tests/test_confounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/transformers/tests/test_jucolumntransformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.740053 julearn-0.3.0/julearn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/utils/_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.740053 julearn-0.3.0/julearn/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/utils/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/utils/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.740053 julearn-0.3.0/julearn/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/viz/_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.740053 julearn-0.3.0/julearn/viz/res/
--rw-r--r--   0 runner    (1001) docker     (123)    73031 2023-07-19 12:22:27.000000 julearn-0.3.0/julearn/viz/res/julearn_logo_generalization.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:22:36.732053 julearn-0.3.0/julearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-19 12:22:36.000000 julearn-0.3.0/julearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-19 12:22:36.000000 julearn-0.3.0/julearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:22:36.000000 julearn-0.3.0/julearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-19 12:22:36.000000 julearn-0.3.0/julearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 12:22:36.000000 julearn-0.3.0/julearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-19 12:22:27.000000 julearn-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:22:36.740053 julearn-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-19 12:22:27.000000 julearn-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-19 12:22:27.000000 julearn-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.453210 julearn-0.3.0.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.417210 julearn-0.3.0.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.425210 julearn-0.3.0.dev3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/.github/ISSUE_TEMPLATE/documentation_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/.github/ISSUE_TEMPLATE/feature_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.425210 julearn-0.3.0.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34353 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-19 12:19:19.453210 julearn-0.3.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.425210 julearn-0.3.0.dev3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.417210 julearn-0.3.0.dev3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.425210 julearn-0.3.0.dev3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.425210 julearn-0.3.0.dev3/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.425210 julearn-0.3.0.dev3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/_templates/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/_templates/function_warning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.429210 julearn-0.3.0.dev3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/model_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/scoring.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/api/viz.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/available_pipeline_steps.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.429210 julearn-0.3.0.dev3/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/changes/contributors.inc
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/changes/latest.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.429210 julearn-0.3.0.dev3/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/changes/newsfragments/151.bugfix
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/changes/newsfragments/170.enh
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/changes/newsfragments/47.feature
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/changes/v0.2.5.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.433210 julearn-0.3.0.dev3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    69241 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/corrected_ttest.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39468 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/final_estimator.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/iris_X.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51228 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/iris_df.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/iris_y.png
+-rw-r--r--   0 runner    (1001) docker     (123)    54482 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/julearn_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    74874 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/julearn_logo_calm.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78884 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/julearn_logo_confbias.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61311 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/julearn_logo_cv.png
+-rw-r--r--   0 runner    (1001) docker     (123)    73031 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/julearn_logo_generalization.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60581 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/julearn_logo_it.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66833 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/julearn_logo_ml.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60581 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/julearn_logo_mlit.png
+-rw-r--r--   0 runner    (1001) docker     (123)    94858 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/multiple_scorers_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84126 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/plot_scores.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43199 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/scores_run_cv.png
+-rw-r--r--   0 runner    (1001) docker     (123)    83552 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/scores_run_cv_splitter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47133 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/images/scores_run_cv_train.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.433210 julearn-0.3.0.dev3/docs/selected_deeper_topics/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/selected_deeper_topics/CBPM.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/selected_deeper_topics/confound_removal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/selected_deeper_topics/cross_validation_splitter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/selected_deeper_topics/hyperparameter_tuning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/selected_deeper_topics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/selected_deeper_topics/model_inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/selected_deeper_topics/stacked_models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/selected_deeper_topics/target_transformers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.433210 julearn-0.3.0.dev3/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/sphinxext/gh_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.433210 julearn-0.3.0.dev3/docs/what_really_need_know/
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/what_really_need_know/cross_validation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/what_really_need_know/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/what_really_need_know/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/what_really_need_know/model_comparison.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/what_really_need_know/model_evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/what_really_need_know/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.433210 julearn-0.3.0.dev3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.437210 julearn-0.3.0.dev3/examples/00_starting/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/00_starting/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/00_starting/plot_cm_acc_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/00_starting/plot_example_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/00_starting/plot_stratified_kfold_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/00_starting/run_combine_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/00_starting/run_grouped_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/00_starting/run_simple_binary_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.437210 julearn-0.3.0.dev3/examples/01_model_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/01_model_comparison/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/01_model_comparison/plot_simple_model_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.437210 julearn-0.3.0.dev3/examples/02_inspection/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/02_inspection/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/02_inspection/plot_groupcv_inspect_svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/02_inspection/plot_inspect_random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/02_inspection/plot_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/02_inspection/run_binary_inspect_folds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.437210 julearn-0.3.0.dev3/examples/03_complex_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/03_complex_models/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/03_complex_models/run_apply_to_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/03_complex_models/run_example_pca_featsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/03_complex_models/run_hyperparameter_multiple_grids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/03_complex_models/run_hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/03_complex_models/run_stacked_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.437210 julearn-0.3.0.dev3/examples/04_confounds/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/04_confounds/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/04_confounds/plot_confound_removal_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/04_confounds/run_return_confounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.437210 julearn-0.3.0.dev3/examples/05_customization/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/05_customization/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/05_customization/run_custom_scorers_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.437210 julearn-0.3.0.dev3/examples/99_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/run_cbpm_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/run_confound_removal_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/run_cv_splitters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/run_data_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/run_hyperparameters_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/run_model_comparison_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/run_model_evaluation_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/run_model_inspection_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15260 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/run_pipeline_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/run_stacked_models_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/99_docs/run_target_transformer_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.441210 julearn-0.3.0.dev3/examples/XX_disabled/
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/XX_disabled/dis_run_n_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/examples/XX_disabled/dis_run_target_confound_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.441210 julearn-0.3.0.dev3/julearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-19 12:19:19.000000 julearn-0.3.0.dev3/julearn/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.441210 julearn-0.3.0.dev3/julearn/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/base/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/base/estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.441210 julearn-0.3.0.dev3/julearn/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/base/tests/test_base_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/base/tests/test_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.441210 julearn-0.3.0.dev3/julearn/inspect/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/inspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/inspect/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/inspect/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/inspect/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/inspect/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.441210 julearn-0.3.0.dev3/julearn/inspect/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/inspect/tests/test_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/inspect/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/inspect/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/inspect/tests/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.441210 julearn-0.3.0.dev3/julearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/model_selection/available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/model_selection/continuous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/model_selection/stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.445210 julearn-0.3.0.dev3/julearn/model_selection/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/model_selection/tests/test_available_searchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/model_selection/tests/test_continous_stratified_kfold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/model_selection/tests/test_stratified_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.445210 julearn-0.3.0.dev3/julearn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/models/available_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/models/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.445210 julearn-0.3.0.dev3/julearn/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/models/tests/test_available_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/models/tests/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/models/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.445210 julearn-0.3.0.dev3/julearn/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/pipeline/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32577 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/pipeline/pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/pipeline/target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/pipeline/target_pipeline_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.445210 julearn-0.3.0.dev3/julearn/pipeline/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/pipeline/test/test_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/pipeline/test/test_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/pipeline/test/test_target_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/pipeline/test/test_target_pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16536 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.445210 julearn-0.3.0.dev3/julearn/scoring/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/scoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/scoring/available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/scoring/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.445210 julearn-0.3.0.dev3/julearn/scoring/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/scoring/tests/test_available_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/scoring/tests/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.445210 julearn-0.3.0.dev3/julearn/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/stats/corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.445210 julearn-0.3.0.dev3/julearn/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/stats/tests/test_corrected_ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.445210 julearn-0.3.0.dev3/julearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35890 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24535 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/tests/test_prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.445210 julearn-0.3.0.dev3/julearn/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.449210 julearn-0.3.0.dev3/julearn/transformers/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/dataframe/change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/dataframe/drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/dataframe/filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/dataframe/set_column_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.449210 julearn-0.3.0.dev3/julearn/transformers/dataframe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/dataframe/tests/test_change_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/dataframe/tests/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/dataframe/tests/test_filter_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/dataframe/tests/test_set_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/ju_column_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.449210 julearn-0.3.0.dev3/julearn/transformers/target/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/target/available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/target/ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/target/ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/target/target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.449210 julearn-0.3.0.dev3/julearn/transformers/target/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/target/tests/test_available_target_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/target/tests/test_ju_target_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/target/tests/test_ju_transformed_target_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/target/tests/test_target_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.449210 julearn-0.3.0.dev3/julearn/transformers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/tests/test_available_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/tests/test_cbpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/tests/test_confounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/transformers/tests/test_jucolumntransformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.449210 julearn-0.3.0.dev3/julearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/utils/_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.449210 julearn-0.3.0.dev3/julearn/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/utils/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/utils/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.453210 julearn-0.3.0.dev3/julearn/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/viz/_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.453210 julearn-0.3.0.dev3/julearn/viz/res/
+-rw-r--r--   0 runner    (1001) docker     (123)    73031 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/julearn/viz/res/julearn_logo_generalization.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:19:19.441210 julearn-0.3.0.dev3/julearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-19 12:19:19.000000 julearn-0.3.0.dev3/julearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-19 12:19:19.000000 julearn-0.3.0.dev3/julearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:19:19.000000 julearn-0.3.0.dev3/julearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-19 12:19:19.000000 julearn-0.3.0.dev3/julearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 12:19:19.000000 julearn-0.3.0.dev3/julearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:19:19.453210 julearn-0.3.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-19 12:19:09.000000 julearn-0.3.0.dev3/tox.ini
```

### Comparing `julearn-0.3.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `julearn-0.3.0.dev3/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/.github/ISSUE_TEMPLATE/documentation_request.yaml` & `julearn-0.3.0.dev3/.github/ISSUE_TEMPLATE/documentation_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `julearn-0.3.0.dev3/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/.github/workflows/ci-docs.yml` & `julearn-0.3.0.dev3/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/.github/workflows/ci.yml` & `julearn-0.3.0.dev3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/.github/workflows/docs-preview.yml` & `julearn-0.3.0.dev3/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/.github/workflows/docs.yml` & `julearn-0.3.0.dev3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/.github/workflows/lint.yml` & `julearn-0.3.0.dev3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/.github/workflows/pypi.yml` & `julearn-0.3.0.dev3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/.gitignore` & `julearn-0.3.0.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/LICENSE.md` & `julearn-0.3.0.dev3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/PKG-INFO` & `julearn-0.3.0.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.0
+Version: 0.3.0.dev3
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
```

### Comparing `julearn-0.3.0/README.md` & `julearn-0.3.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/codecov.yml` & `julearn-0.3.0.dev3/codecov.yml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/Makefile` & `julearn-0.3.0.dev3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/_templates/class.rst` & `julearn-0.3.0.dev3/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/_templates/function_warning.rst` & `julearn-0.3.0.dev3/docs/_templates/function_warning.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/_templates/versions.html` & `julearn-0.3.0.dev3/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/api/base.rst` & `julearn-0.3.0.dev3/docs/api/base.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/api/model_selection.rst` & `julearn-0.3.0.dev3/docs/api/model_selection.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/api/models.rst` & `julearn-0.3.0.dev3/docs/api/models.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/api/scoring.rst` & `julearn-0.3.0.dev3/docs/api/scoring.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/api/transformers.rst` & `julearn-0.3.0.dev3/docs/api/transformers.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/api/utils.rst` & `julearn-0.3.0.dev3/docs/api/utils.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/api/viz.rst` & `julearn-0.3.0.dev3/docs/api/viz.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/available_pipeline_steps.rst` & `julearn-0.3.0.dev3/docs/available_pipeline_steps.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/changes/latest.inc` & `julearn-0.3.0.dev3/docs/changes/latest.inc`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/changes/v0.2.5.inc` & `julearn-0.3.0.dev3/docs/changes/v0.2.5.inc`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/conf.py` & `julearn-0.3.0.dev3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/configuration.rst` & `julearn-0.3.0.dev3/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/contributing.rst` & `julearn-0.3.0.dev3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/examples.rst` & `julearn-0.3.0.dev3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/faq.rst` & `julearn-0.3.0.dev3/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/getting_started.rst` & `julearn-0.3.0.dev3/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/corrected_ttest.png` & `julearn-0.3.0.dev3/docs/images/corrected_ttest.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/final_estimator.png` & `julearn-0.3.0.dev3/docs/images/final_estimator.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/iris_X.png` & `julearn-0.3.0.dev3/docs/images/iris_X.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/iris_df.png` & `julearn-0.3.0.dev3/docs/images/iris_df.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/iris_y.png` & `julearn-0.3.0.dev3/docs/images/iris_y.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/julearn_logo.png` & `julearn-0.3.0.dev3/docs/images/julearn_logo.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/julearn_logo_calm.png` & `julearn-0.3.0.dev3/docs/images/julearn_logo_calm.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/julearn_logo_confbias.png` & `julearn-0.3.0.dev3/docs/images/julearn_logo_confbias.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/julearn_logo_cv.png` & `julearn-0.3.0.dev3/docs/images/julearn_logo_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/julearn_logo_generalization.png` & `julearn-0.3.0.dev3/docs/images/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/julearn_logo_it.png` & `julearn-0.3.0.dev3/docs/images/julearn_logo_it.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/julearn_logo_ml.png` & `julearn-0.3.0.dev3/docs/images/julearn_logo_ml.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/julearn_logo_mlit.png` & `julearn-0.3.0.dev3/docs/images/julearn_logo_mlit.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/multiple_scorers_run_cv.png` & `julearn-0.3.0.dev3/docs/images/multiple_scorers_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/plot_scores.png` & `julearn-0.3.0.dev3/docs/images/plot_scores.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/scores_run_cv.png` & `julearn-0.3.0.dev3/docs/images/scores_run_cv.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/scores_run_cv_splitter.png` & `julearn-0.3.0.dev3/docs/images/scores_run_cv_splitter.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/images/scores_run_cv_train.png` & `julearn-0.3.0.dev3/docs/images/scores_run_cv_train.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/index.rst` & `julearn-0.3.0.dev3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/links.inc` & `julearn-0.3.0.dev3/docs/links.inc`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/maintaining.rst` & `julearn-0.3.0.dev3/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/sphinxext/gh_substitutions.py` & `julearn-0.3.0.dev3/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/what_really_need_know/cross_validation.rst` & `julearn-0.3.0.dev3/docs/what_really_need_know/cross_validation.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/what_really_need_know/index.rst` & `julearn-0.3.0.dev3/docs/what_really_need_know/index.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/docs/whats_new.rst` & `julearn-0.3.0.dev3/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/00_starting/plot_cm_acc_multiclass.py` & `julearn-0.3.0.dev3/examples/00_starting/plot_cm_acc_multiclass.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/00_starting/plot_example_regression.py` & `julearn-0.3.0.dev3/examples/00_starting/plot_example_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/00_starting/plot_stratified_kfold_reg.py` & `julearn-0.3.0.dev3/examples/00_starting/plot_stratified_kfold_reg.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/00_starting/run_combine_pandas.py` & `julearn-0.3.0.dev3/examples/00_starting/run_combine_pandas.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/00_starting/run_grouped_cv.py` & `julearn-0.3.0.dev3/examples/00_starting/run_grouped_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/00_starting/run_simple_binary_classification.py` & `julearn-0.3.0.dev3/examples/00_starting/run_simple_binary_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/01_model_comparison/plot_simple_model_comparison.py` & `julearn-0.3.0.dev3/examples/01_model_comparison/plot_simple_model_comparison.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/02_inspection/plot_groupcv_inspect_svm.py` & `julearn-0.3.0.dev3/examples/02_inspection/plot_groupcv_inspect_svm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/02_inspection/plot_inspect_random_forest.py` & `julearn-0.3.0.dev3/examples/02_inspection/plot_inspect_random_forest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/02_inspection/plot_preprocess.py` & `julearn-0.3.0.dev3/examples/02_inspection/plot_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/02_inspection/run_binary_inspect_folds.py` & `julearn-0.3.0.dev3/examples/02_inspection/run_binary_inspect_folds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/03_complex_models/run_apply_to_target.py` & `julearn-0.3.0.dev3/examples/03_complex_models/run_apply_to_target.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/03_complex_models/run_example_pca_featsets.py` & `julearn-0.3.0.dev3/examples/03_complex_models/run_example_pca_featsets.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/03_complex_models/run_hyperparameter_multiple_grids.py` & `julearn-0.3.0.dev3/examples/03_complex_models/run_hyperparameter_multiple_grids.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/03_complex_models/run_hyperparameter_tuning.py` & `julearn-0.3.0.dev3/examples/03_complex_models/run_hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/03_complex_models/run_stacked_models.py` & `julearn-0.3.0.dev3/examples/03_complex_models/run_stacked_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/04_confounds/plot_confound_removal_classification.py` & `julearn-0.3.0.dev3/examples/04_confounds/plot_confound_removal_classification.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/04_confounds/run_return_confounds.py` & `julearn-0.3.0.dev3/examples/04_confounds/run_return_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/05_customization/run_custom_scorers_regression.py` & `julearn-0.3.0.dev3/examples/05_customization/run_custom_scorers_regression.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/99_docs/run_cbpm_docs.py` & `julearn-0.3.0.dev3/examples/99_docs/run_cbpm_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/99_docs/run_confound_removal_docs.py` & `julearn-0.3.0.dev3/examples/99_docs/run_confound_removal_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/99_docs/run_cv_splitters_docs.py` & `julearn-0.3.0.dev3/examples/99_docs/run_cv_splitters_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/99_docs/run_data_docs.py` & `julearn-0.3.0.dev3/examples/99_docs/run_data_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/99_docs/run_hyperparameters_docs.py` & `julearn-0.3.0.dev3/examples/99_docs/run_hyperparameters_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/99_docs/run_model_comparison_docs.py` & `julearn-0.3.0.dev3/examples/99_docs/run_model_comparison_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/99_docs/run_model_evaluation_docs.py` & `julearn-0.3.0.dev3/examples/99_docs/run_model_evaluation_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/99_docs/run_model_inspection_docs.py` & `julearn-0.3.0.dev3/examples/99_docs/run_model_inspection_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/99_docs/run_pipeline_docs.py` & `julearn-0.3.0.dev3/examples/99_docs/run_pipeline_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/99_docs/run_stacked_models_docs.py` & `julearn-0.3.0.dev3/examples/99_docs/run_stacked_models_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/99_docs/run_target_transformer_docs.py` & `julearn-0.3.0.dev3/examples/99_docs/run_target_transformer_docs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/XX_disabled/dis_run_n_jobs.py` & `julearn-0.3.0.dev3/examples/XX_disabled/dis_run_n_jobs.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/examples/XX_disabled/dis_run_target_confound_removal.py` & `julearn-0.3.0.dev3/examples/XX_disabled/dis_run_target_confound_removal.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/api.py` & `julearn-0.3.0.dev3/julearn/api.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/base/column_types.py` & `julearn-0.3.0.dev3/julearn/base/column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/base/estimators.py` & `julearn-0.3.0.dev3/julearn/base/estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/base/tests/test_base_estimators.py` & `julearn-0.3.0.dev3/julearn/base/tests/test_base_estimators.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/base/tests/test_column_types.py` & `julearn-0.3.0.dev3/julearn/base/tests/test_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/config.py` & `julearn-0.3.0.dev3/julearn/config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/conftest.py` & `julearn-0.3.0.dev3/julearn/conftest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/inspect/_cv.py` & `julearn-0.3.0.dev3/julearn/inspect/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/inspect/_pipeline.py` & `julearn-0.3.0.dev3/julearn/inspect/_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/inspect/_preprocess.py` & `julearn-0.3.0.dev3/julearn/inspect/_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/inspect/inspector.py` & `julearn-0.3.0.dev3/julearn/inspect/inspector.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/inspect/tests/test_cv.py` & `julearn-0.3.0.dev3/julearn/inspect/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/inspect/tests/test_inspector.py` & `julearn-0.3.0.dev3/julearn/inspect/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/inspect/tests/test_pipeline.py` & `julearn-0.3.0.dev3/julearn/inspect/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/inspect/tests/test_preprocess.py` & `julearn-0.3.0.dev3/julearn/inspect/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/model_selection/available_searchers.py` & `julearn-0.3.0.dev3/julearn/model_selection/available_searchers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/model_selection/continuous_stratified_kfold.py` & `julearn-0.3.0.dev3/julearn/model_selection/continuous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/model_selection/stratified_bootstrap.py` & `julearn-0.3.0.dev3/julearn/model_selection/stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/model_selection/tests/test_available_searchers.py` & `julearn-0.3.0.dev3/julearn/model_selection/tests/test_available_searchers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/model_selection/tests/test_continous_stratified_kfold.py` & `julearn-0.3.0.dev3/julearn/model_selection/tests/test_continous_stratified_kfold.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/model_selection/tests/test_stratified_bootstrap.py` & `julearn-0.3.0.dev3/julearn/model_selection/tests/test_stratified_bootstrap.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/models/available_models.py` & `julearn-0.3.0.dev3/julearn/models/available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/models/dynamic.py` & `julearn-0.3.0.dev3/julearn/models/dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/models/tests/test_available_models.py` & `julearn-0.3.0.dev3/julearn/models/tests/test_available_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/models/tests/test_dynamic.py` & `julearn-0.3.0.dev3/julearn/models/tests/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/models/tests/test_models.py` & `julearn-0.3.0.dev3/julearn/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/pipeline/merger.py` & `julearn-0.3.0.dev3/julearn/pipeline/merger.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/pipeline/pipeline_creator.py` & `julearn-0.3.0.dev3/julearn/pipeline/pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/pipeline/target_pipeline.py` & `julearn-0.3.0.dev3/julearn/pipeline/target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/pipeline/target_pipeline_creator.py` & `julearn-0.3.0.dev3/julearn/pipeline/target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/pipeline/test/test_merger.py` & `julearn-0.3.0.dev3/julearn/pipeline/test/test_merger.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/pipeline/test/test_pipeline_creator.py` & `julearn-0.3.0.dev3/julearn/pipeline/test/test_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/pipeline/test/test_target_pipeline.py` & `julearn-0.3.0.dev3/julearn/pipeline/test/test_target_pipeline.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/pipeline/test/test_target_pipeline_creator.py` & `julearn-0.3.0.dev3/julearn/pipeline/test/test_target_pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/prepare.py` & `julearn-0.3.0.dev3/julearn/prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/scoring/available_scorers.py` & `julearn-0.3.0.dev3/julearn/scoring/available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/scoring/metrics.py` & `julearn-0.3.0.dev3/julearn/scoring/metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/scoring/tests/test_available_scorers.py` & `julearn-0.3.0.dev3/julearn/scoring/tests/test_available_scorers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/scoring/tests/test_metrics.py` & `julearn-0.3.0.dev3/julearn/scoring/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/stats/corrected_ttest.py` & `julearn-0.3.0.dev3/julearn/stats/corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/stats/tests/test_corrected_ttest.py` & `julearn-0.3.0.dev3/julearn/stats/tests/test_corrected_ttest.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/tests/test_api.py` & `julearn-0.3.0.dev3/julearn/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/tests/test_config.py` & `julearn-0.3.0.dev3/julearn/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/tests/test_prepare.py` & `julearn-0.3.0.dev3/julearn/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/__init__.py` & `julearn-0.3.0.dev3/julearn/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/available_transformers.py` & `julearn-0.3.0.dev3/julearn/transformers/available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/cbpm.py` & `julearn-0.3.0.dev3/julearn/transformers/cbpm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/confound_remover.py` & `julearn-0.3.0.dev3/julearn/transformers/confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/dataframe/change_column_types.py` & `julearn-0.3.0.dev3/julearn/transformers/dataframe/change_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/dataframe/drop_columns.py` & `julearn-0.3.0.dev3/julearn/transformers/dataframe/drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/dataframe/filter_columns.py` & `julearn-0.3.0.dev3/julearn/transformers/dataframe/filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/dataframe/set_column_types.py` & `julearn-0.3.0.dev3/julearn/transformers/dataframe/set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/dataframe/tests/test_change_column_types.py` & `julearn-0.3.0.dev3/julearn/transformers/dataframe/tests/test_change_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/dataframe/tests/test_drop_columns.py` & `julearn-0.3.0.dev3/julearn/transformers/dataframe/tests/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/dataframe/tests/test_filter_columns.py` & `julearn-0.3.0.dev3/julearn/transformers/dataframe/tests/test_filter_columns.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/dataframe/tests/test_set_column_types.py` & `julearn-0.3.0.dev3/julearn/transformers/dataframe/tests/test_set_column_types.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/ju_column_transformer.py` & `julearn-0.3.0.dev3/julearn/transformers/ju_column_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/target/__init__.py` & `julearn-0.3.0.dev3/julearn/transformers/target/__init__.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/target/available_target_transformers.py` & `julearn-0.3.0.dev3/julearn/transformers/target/available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/target/ju_target_transformer.py` & `julearn-0.3.0.dev3/julearn/transformers/target/ju_target_transformer.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/target/ju_transformed_target_model.py` & `julearn-0.3.0.dev3/julearn/transformers/target/ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/target/target_confound_remover.py` & `julearn-0.3.0.dev3/julearn/transformers/target/target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/target/tests/test_available_target_transformers.py` & `julearn-0.3.0.dev3/julearn/transformers/target/tests/test_available_target_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/target/tests/test_ju_transformed_target_model.py` & `julearn-0.3.0.dev3/julearn/transformers/target/tests/test_ju_transformed_target_model.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/target/tests/test_target_confound_remover.py` & `julearn-0.3.0.dev3/julearn/transformers/target/tests/test_target_confound_remover.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/tests/test_available_transformers.py` & `julearn-0.3.0.dev3/julearn/transformers/tests/test_available_transformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/tests/test_cbpm.py` & `julearn-0.3.0.dev3/julearn/transformers/tests/test_cbpm.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/tests/test_confounds.py` & `julearn-0.3.0.dev3/julearn/transformers/tests/test_confounds.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/transformers/tests/test_jucolumntransformers.py` & `julearn-0.3.0.dev3/julearn/transformers/tests/test_jucolumntransformers.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/utils/_cv.py` & `julearn-0.3.0.dev3/julearn/utils/_cv.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/utils/checks.py` & `julearn-0.3.0.dev3/julearn/utils/checks.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/utils/logging.py` & `julearn-0.3.0.dev3/julearn/utils/logging.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/utils/testing.py` & `julearn-0.3.0.dev3/julearn/utils/testing.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/utils/tests/test_logging.py` & `julearn-0.3.0.dev3/julearn/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/utils/tests/test_version.py` & `julearn-0.3.0.dev3/julearn/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/utils/typing.py` & `julearn-0.3.0.dev3/julearn/utils/typing.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/utils/versions.py` & `julearn-0.3.0.dev3/julearn/utils/versions.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/viz/_scores.py` & `julearn-0.3.0.dev3/julearn/viz/_scores.py`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn/viz/res/julearn_logo_generalization.png` & `julearn-0.3.0.dev3/julearn/viz/res/julearn_logo_generalization.png`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/julearn.egg-info/PKG-INFO` & `julearn-0.3.0.dev3/julearn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julearn
-Version: 0.3.0
+Version: 0.3.0.dev3
 Summary: Juelich Machine Learning Library
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Sami Hamdan <s.hamdan@fz-juelich.de>
 Maintainer-email: Sami Hamdan <s.hamdan@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/julearn
 Project-URL: documentation, https://juaml.github.io/julearn
 Project-URL: repository, https://github.com/juaml/julearn
```

### Comparing `julearn-0.3.0/julearn.egg-info/SOURCES.txt` & `julearn-0.3.0.dev3/julearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/pyproject.toml` & `julearn-0.3.0.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `julearn-0.3.0/tox.ini` & `julearn-0.3.0.dev3/tox.ini`

 * *Files identical despite different names*

