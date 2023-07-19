# Comparing `tmp/alchemite_apiclient-0.57.0.tar.gz` & `tmp/alchemite_apiclient-0.58.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemite_apiclient-0.57.0.tar", last modified: Wed Jul  5 09:28:13 2023, max compression
+gzip compressed data, was "alchemite_apiclient-0.58.0.tar", last modified: Wed Jul 19 09:27:44 2023, max compression
```

## Comparing `alchemite_apiclient-0.57.0.tar` & `alchemite_apiclient-0.58.0.tar`

### file list

```diff
@@ -1,605 +1,606 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-05 09:28:13.724333 alchemite_apiclient-0.57.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4935 2023-07-05 09:28:13.724333 alchemite_apiclient-0.57.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4232 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-05 09:28:13.636333 alchemite_apiclient-0.57.0/alchemite_apiclient/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22403 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-05 09:28:13.636333 alchemite_apiclient-0.57.0/alchemite_apiclient/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   111028 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/api/datasets_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34995 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/api/default_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5113 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/api/metrics_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    57863 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/api/model_dataset_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   235552 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/api/models_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    37770 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/api_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-05 09:28:13.636333 alchemite_apiclient-0.57.0/alchemite_apiclient/apis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/apis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17318 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5079 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15773 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/extensions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-05 09:28:13.676333 alchemite_apiclient-0.57.0/alchemite_apiclient/model/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14502 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/additive_sensitivity_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15940 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/analyse_validate_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12717 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/analyse_validate_request_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24816 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/analyse_validate_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18046 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12124 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15273 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11771 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14958 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_column_info_stats.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17661 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_model_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13506 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11411 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11432 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11554 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_group_batch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_group_patch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11605 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_group_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13897 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_group_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11120 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_group_response_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16155 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11587 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11749 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_value_nullable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15595 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/continuous_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11760 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/continuous_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/continuous_column_info_stats.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16839 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/continuous_model_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12255 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11280 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27957 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11519 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset1.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_chunk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14079 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_or_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11454 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14432 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_query_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12022 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_query_request_row_ids.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11619 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_query_request_sort.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11888 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_query_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11530 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_query_response_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14166 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14730 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14585 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14493 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14338 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15173 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14716 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14627 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14486 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11971 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12802 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12505 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dimensionality_reduction_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12947 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dimensionality_reduction_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12516 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_dataset_reduction_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13100 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11332 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13072 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_job_reduction_metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11829 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12971 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_model_reduction_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11523 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_one_dimension_point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12103 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_three_dimension_point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11810 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_two_dimension_point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11759 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/drpca_reduction_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13502 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/drumap_reduction_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12701 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/empty_categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12903 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/empty_continuous_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12586 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/error.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11685 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_all_opt_jobs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15543 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11951 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15300 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11638 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_failed_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15422 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_optimizing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11784 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15176 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11437 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_pending_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16376 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11926 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16185 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16061 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11464 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16265 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_running.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11778 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16322 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_historic_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11906 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16155 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_historic_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16031 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_historic_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16235 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_historic_running.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16295 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11896 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16215 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11746 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16016 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16220 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_running.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_categorical_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12150 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11426 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_scalar_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10976 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_target_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11839 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_vector_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12403 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_vector_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12954 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/importance_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13832 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/impute_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11377 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/int_cat_arr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11426 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/job_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11133 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/load_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34713 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18541 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/model_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11440 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/model_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11754 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/model_permitted_column_relationships.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10999 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/models_dataset_put_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11775 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12259 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14076 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_col.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11795 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14640 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12340 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11409 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14495 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12142 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11451 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14403 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_product.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12061 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11607 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14248 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15083 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12869 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11581 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12265 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11958 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14537 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12178 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11981 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14354 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12440 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12307 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/non_empty_categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12381 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/non_empty_continuous_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17508 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/optimize_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12405 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/ot_sample_def_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12087 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/ot_sample_def_continuous.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/ot_sample_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10877 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/ot_set_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13043 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/outliers_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13158 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12571 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11980 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11919 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_response_predictions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11857 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11129 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_univariate_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11449 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_dependent_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12668 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_get_optimize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11837 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13493 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_get_suggest_additional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13473 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_get_suggest_historic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13463 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_get_suggest_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11353 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_new_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13513 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11670 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_categoricals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14407 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_single_tar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13421 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13415 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/predict_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12027 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16555 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/query_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14001 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/query_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12844 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10940 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_categorical_column_values.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16961 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_composition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15367 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_composition_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12213 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_continuous.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14847 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_continuous_with_start.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12546 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_discrete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_integer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11515 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_start_prop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12389 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_weighted_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10958 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11402 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/scalar_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11456 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/scalar_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13086 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/sensitivity_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10871 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/set_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11163 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/share_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12251 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/si_sample_def_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/si_sample_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11386 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/string_cat_arr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23791 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_additional_parameters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19951 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24667 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_additional_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11828 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_additional_request_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11688 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_additional_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13065 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_historic_parameters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15809 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_historic_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12283 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_historic_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13828 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_historic_result_samples.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12045 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_initial_parameters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15023 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_initial_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11821 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_initial_request_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17283 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_initial_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11679 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_initial_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13582 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19333 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11439 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_data_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19913 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_dataset_id.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12068 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21491 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_imputed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13609 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23011 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12222 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14071 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_specific.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17194 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_above_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17194 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_below_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17421 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11507 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_between_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17938 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_exclude_categories.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11673 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17930 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_include_categories.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16619 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11624 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16767 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10952 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/target_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23224 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/train_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11148 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/training_dataset_outliers_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/validate_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12755 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/validation_split.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12070 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/vector_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12058 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/vector_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12055 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/vector_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model/version_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    82086 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/model_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-05 09:28:13.676333 alchemite_apiclient-0.57.0/alchemite_apiclient/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21574 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14208 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/alchemite_apiclient/rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-05 09:28:13.636333 alchemite_apiclient-0.57.0/alchemite_apiclient.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4935 2023-07-05 09:28:13.000000 alchemite_apiclient-0.57.0/alchemite_apiclient.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24066 2023-07-05 09:28:13.000000 alchemite_apiclient-0.57.0/alchemite_apiclient.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-05 09:28:13.000000 alchemite_apiclient-0.57.0/alchemite_apiclient.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-07-05 09:28:13.000000 alchemite_apiclient-0.57.0/alchemite_apiclient.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2023-07-05 09:28:13.000000 alchemite_apiclient-0.57.0/alchemite_apiclient.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-05 09:28:13.712333 alchemite_apiclient-0.57.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1757 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/AdditiveSensitivityRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1477 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/AnalyseValidateRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1123 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/AnalyseValidateRequestAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5720 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/AnalyseValidateResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2764 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/AnalyseValidateResponseColumnAnalytics.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      797 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/CategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      990 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/CategoricalColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/CategoricalColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      959 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/CategoricalColumnInfoStats.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2073 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/CategoricalModelColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1557 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/CategoricalModelColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      529 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/CategoricalPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/CategoricalResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      547 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ColumnGroupBatchRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      720 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ColumnGroupPatchRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      600 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ColumnGroupRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ColumnGroupResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      545 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ColumnGroupResponseAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1582 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      624 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ColumnValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ColumnValueNullable.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1129 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ContinuousColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      582 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ContinuousColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ContinuousColumnInfoStats.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1676 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ContinuousModelColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1020 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ContinuousModelColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      802 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DRDatasetReductionData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DRDatasetReductionMetadata.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DRDatasetReductionMetadataSources.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1038 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DRJobReductionMetadata.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      725 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DRJobReductionMetadataSources.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1016 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DRModelReductionData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DROneDimensionPoint.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DRPCAReductionType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DRThreeDimensionPoint.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DRTwoDimensionPoint.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DRUMAPReductionType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      578 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/Data.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7250 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/Dataset.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/Dataset1.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DatasetChunk.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DatasetOrData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      571 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DatasetPatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1507 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DatasetQueryRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DatasetQueryRequestRowIDs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DatasetQueryRequestSort.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DatasetQueryResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DatasetQueryResponseResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61432 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DatasetsApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18436 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DefaultApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      791 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DependentColFnArgCol.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DependentColFnArgColWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      748 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DependentColFnArgConstantSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      731 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DependentColFnArgProduct.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      737 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DependentColFnArgRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DependentColFnArgSummandsWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      772 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DependentColFnArgWeightedConstSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      756 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DependentColFnArgWeightedRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DependentColFnArgZeroIfZero.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      661 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DependentColFnArgZeroIfZeroAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DependentColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DimensionalityReductionRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/DimensionalityReductionResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      881 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/EmptyCategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1021 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/EmptyContinuousColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1027 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/Error.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetAllOptJobs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1025 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetOptimizeDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      630 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetOptimizeDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetOptimizeFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetOptimizeFailedAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetOptimizeOptimizing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetOptimizeOptimizingAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetOptimizePending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetOptimizePendingAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1175 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalFailedAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalPending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalPendingAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalRunning.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalRunningAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestHistoricDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestHistoricDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1169 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestHistoricFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1144 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestHistoricPending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1186 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestHistoricRunning.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1206 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestInitialDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestInitialDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1210 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestInitialFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestInitialFailedAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestInitialPending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1183 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/GetSuggestInitialRunning.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/HistoricCategoricalPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/HistoricPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/HistoricScalarPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      700 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/HistoricTargetFunction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/HistoricValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/HistoricVectorPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/HistoricVectorValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ImportanceRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1583 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ImputeRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/IntCatArr.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/JobPatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/LoadRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/MetricsApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7976 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/Model.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2665 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ModelColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34815 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ModelDatasetApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ModelPatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ModelPermittedColumnRelationships.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)   143019 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ModelsApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ModelsDatasetPutRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ModelsIdAdditiveSensitivityOrigin.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ModelsIdTrainPermittedColumnRelationships.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      773 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgCol.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      679 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgColAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      953 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgColWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgColWeightsAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgColWeightsAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      730 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgConstantSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgConstantSumAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgConstantSumAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgProduct.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgProductAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgProductAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      719 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgRatioAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgSummandsWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgSummandsWeightsAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      754 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedConstSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      660 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedConstSumAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      698 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      738 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedRatioAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      852 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedRatioAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      743 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgZeroIfZero.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColFnArgZeroIfZeroAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      799 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NewColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      770 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NonEmptyCategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      843 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NonEmptyContinuousColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      777 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/NonEmptyIntegerCategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1254 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OTSampleDefCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OTSampleDefContinuous.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OTSampleDefinition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      494 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OTSetInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2953 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OptimizeRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1255 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OutliersRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OutputToleranceRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OutputToleranceResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OutputToleranceResponseFixedInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OutputToleranceResponsePredictedOutputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OutputToleranceResponsePredictions.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      741 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OutputToleranceResponseSampledInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/OutputToleranceUnivariateResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartDependentColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartGetOptimize.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartGetOptimizeDoneResultArray.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1099 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartGetSuggestAdditional.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartGetSuggestHistoric.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1090 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartGetSuggestInitial.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartNewColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartTarFnAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartTarFnBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartTarFnBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartTarFnCategoricals.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1968 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartTarFnSingleTar.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartTarFnSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PartTarFnWeightedSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/PredictRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/Prediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/QueryRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/QueryResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SISampleDefCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SISampleDefinition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SampleDefCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SampleDefCategoricalColumnValues.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2029 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SampleDefComposition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1933 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SampleDefCompositionAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SampleDefContinuous.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SampleDefContinuousWithStart.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SampleDefDiscrete.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SampleDefInteger.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SampleDefStartProp.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SampleDefWeightedCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SampleDefinition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ScalarPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ScalarResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1196 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SensitivityRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SetInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      512 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ShareGroup.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      319 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/StringCatArr.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4837 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestAdditionalParameters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3870 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestAdditionalParametersAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestAdditionalRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestAdditionalRequestAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestAdditionalResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1050 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestHistoricParameters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestHistoricRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      922 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestHistoricResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1358 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestHistoricResultSamples.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestInitialParameters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestInitialRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      740 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestInitialRequestAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestInitialResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      393 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestInitialResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1440 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestMissingCommon.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2955 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestMissingData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      648 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestMissingDataAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3155 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestMissingDatasetID.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      848 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestMissingDatasetIDAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4011 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestMissingImputedData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestMissingImputedDataAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4589 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestMissingRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      909 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestMissingResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/SuggestMissingSpecific.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2090 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnAboveAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2090 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnBelowAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnBetweenAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2226 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnExcludeCategories.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      612 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnExcludeCategoriesAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2222 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnIncludeCategories.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnIncludeCategoriesAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnSumAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnSumAboveAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnSumBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnSumBelowAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1828 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnSumBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnSumBetweenAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnWeightedSumAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnWeightedSumAboveAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnWeightedSumBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnWeightedSumBelowAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1835 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnWeightedSumBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      678 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TarFnWeightedSumBetweenAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1592 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TargetFunction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5666 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TrainRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/TrainingDatasetOutliersRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1595 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ValidateRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1096 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/ValidationSplit.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/Value.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/VectorPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/VectorResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/VectorValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      945 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/docs/VersionResponse.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-05 09:28:13.720333 alchemite_apiclient-0.57.0/example/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   701201 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/adrenergic.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)   243835 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/adrenergic_holdout.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1654 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/adrenergic_row.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/categorical.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/credentials_auth_code_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/credentials_client_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/credentials_pass_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/credentials_pass_prompted_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4566 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_additive_sensitivity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3944 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2775 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_chunk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4120 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_column_groups.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_connect.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5769 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_custom_validation_splits.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1175 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_delete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5634 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_dimensionality_reduction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_download.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_export_import.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4185 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_hyperopt.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3833 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_importance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5574 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_optimize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3181 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_outliers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4774 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_output_tolerance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4511 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_preload.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4054 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4504 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_sensitivity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5511 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_suggest_additional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5547 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_suggest_historic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1980 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_suggest_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4598 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_suggest_missing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3419 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_training_outliers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_validate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5497 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/example_vector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      759 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/optimize_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/optimize_args_vector.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1290 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/optimize_dependentColumns_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1189 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/steels.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/steels_impute.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      854 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/suggest_additional_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/suggest_additional_args_vector.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/suggest_historic_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/suggest_historic_args_vector.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/suggest_initial_args.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      503 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/example/vector.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-05 09:28:13.724333 alchemite_apiclient-0.57.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1178 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-05 09:28:13.724333 alchemite_apiclient-0.57.0/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_additive_sensitivity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2591 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2506 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1985 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_chunk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2873 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_column_groups.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_connect.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2255 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_cornercases.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3803 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_custom_validation_splits.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_delete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2493 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_dimensionality_reduction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      682 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_download.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3819 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_examples.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1538 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_hyperopt.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      932 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_importance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_optimize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_outliers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1848 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_output_tolerance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1502 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_preload.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_sensitivity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1042 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_suggest_additional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1152 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_suggest_historic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_suggest_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_suggest_missing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      489 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_training_outliers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      833 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_validate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2431 2023-07-05 09:28:07.000000 alchemite_apiclient-0.57.0/test/test_vector.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 09:27:44.024548 alchemite_apiclient-0.58.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4935 2023-07-19 09:27:44.024548 alchemite_apiclient-0.58.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4232 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 09:27:43.944548 alchemite_apiclient-0.58.0/alchemite_apiclient/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22403 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 09:27:43.948548 alchemite_apiclient-0.58.0/alchemite_apiclient/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   111028 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/api/datasets_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34995 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/api/default_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5113 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/api/metrics_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57863 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/api/model_dataset_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   240401 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/api/models_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37920 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/api_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 09:27:43.948548 alchemite_apiclient-0.58.0/alchemite_apiclient/apis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/apis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17318 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5079 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15773 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/extensions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 09:27:43.980548 alchemite_apiclient-0.58.0/alchemite_apiclient/model/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14502 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/additive_sensitivity_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15940 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/analyse_validate_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12717 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/analyse_validate_request_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24816 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/analyse_validate_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18046 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12124 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15273 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11771 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14958 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_column_info_stats.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17661 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_model_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13506 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11411 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11432 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11554 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_group_batch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_group_patch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11605 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_group_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13897 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_group_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11120 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_group_response_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16155 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11587 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11749 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_value_nullable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15595 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/continuous_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11760 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/continuous_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/continuous_column_info_stats.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16839 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/continuous_model_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12255 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11280 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27957 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11519 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset1.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_chunk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14079 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_or_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11454 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14432 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_query_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12022 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_query_request_row_ids.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11619 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_query_request_sort.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11888 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_query_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11530 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_query_response_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14166 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14730 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14585 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14493 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14338 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15173 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14716 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14627 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14486 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11971 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12802 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12505 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dimensionality_reduction_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12947 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dimensionality_reduction_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12516 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_dataset_reduction_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13100 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11332 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13072 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_job_reduction_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11829 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12971 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_model_reduction_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11523 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_one_dimension_point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12103 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_three_dimension_point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11810 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_two_dimension_point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11759 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/drpca_reduction_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13502 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/drumap_reduction_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12701 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/empty_categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12903 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/empty_continuous_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12586 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/error.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11685 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_all_opt_jobs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15543 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11951 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15300 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11638 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_failed_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15422 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_optimizing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11784 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15176 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11437 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_pending_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16376 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11926 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16185 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16061 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11464 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16265 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_running.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11778 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16322 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_historic_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11906 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16155 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_historic_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16031 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_historic_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16235 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_historic_running.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16295 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11896 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16215 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11746 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16016 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16220 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_running.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_categorical_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12150 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11426 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_scalar_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10976 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_target_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11839 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_vector_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12403 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_vector_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12954 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/importance_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13832 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/impute_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11377 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/int_cat_arr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11426 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/job_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11133 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/load_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34713 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18541 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/model_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11440 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/model_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11754 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/model_permitted_column_relationships.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10999 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/models_dataset_put_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11775 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12259 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14076 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_col.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11795 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14640 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12340 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11409 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14495 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12142 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11451 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14403 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_product.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12061 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11607 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14248 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15083 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12869 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11581 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12265 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11958 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14537 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12178 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11981 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14354 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12440 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12307 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/non_empty_categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12381 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/non_empty_continuous_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17508 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/optimize_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12405 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/ot_sample_def_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12087 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/ot_sample_def_continuous.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/ot_sample_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10877 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/ot_set_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13043 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/outliers_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13158 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12571 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11980 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11919 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_response_predictions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11857 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11129 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_univariate_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11449 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_dependent_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12668 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_get_optimize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11837 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13493 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_get_suggest_additional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13473 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_get_suggest_historic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13463 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_get_suggest_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11353 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_new_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13513 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11670 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_categoricals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14407 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_single_tar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13421 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13415 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/predict_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12027 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16555 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/query_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14001 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/query_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12844 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10940 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_categorical_column_values.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16961 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_composition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15367 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_composition_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12213 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_continuous.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14847 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_continuous_with_start.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12546 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_discrete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_integer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11515 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_start_prop.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12389 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_weighted_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10958 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11402 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/scalar_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11456 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/scalar_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13086 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/sensitivity_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10871 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/set_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11163 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/share_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12251 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/si_sample_def_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/si_sample_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11386 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/string_cat_arr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23791 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_additional_parameters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19951 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24667 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_additional_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11828 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_additional_request_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11688 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_additional_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13065 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_historic_parameters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15809 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_historic_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12283 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_historic_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13828 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_historic_result_samples.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12045 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_initial_parameters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15023 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_initial_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11821 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_initial_request_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17283 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_initial_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11679 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_initial_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13582 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19333 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11439 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_data_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19913 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_dataset_id.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12068 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21491 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_imputed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13609 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23011 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12222 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14071 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_specific.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17194 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_above_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17194 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_below_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17421 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11507 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_between_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17938 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_exclude_categories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11673 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17930 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_include_categories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16619 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11624 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16767 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10952 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/target_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23224 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/train_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11148 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/training_dataset_outliers_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/validate_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12755 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/validation_split.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12070 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/vector_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12058 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/vector_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12055 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/vector_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model/version_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    82086 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/model_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 09:27:43.980548 alchemite_apiclient-0.58.0/alchemite_apiclient/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21574 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14208 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/alchemite_apiclient/rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 09:27:43.948548 alchemite_apiclient-0.58.0/alchemite_apiclient.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4935 2023-07-19 09:27:43.000000 alchemite_apiclient-0.58.0/alchemite_apiclient.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24092 2023-07-19 09:27:43.000000 alchemite_apiclient-0.58.0/alchemite_apiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-19 09:27:43.000000 alchemite_apiclient-0.58.0/alchemite_apiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-07-19 09:27:43.000000 alchemite_apiclient-0.58.0/alchemite_apiclient.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2023-07-19 09:27:43.000000 alchemite_apiclient-0.58.0/alchemite_apiclient.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 09:27:44.012548 alchemite_apiclient-0.58.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1757 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/AdditiveSensitivityRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1477 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/AnalyseValidateRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1123 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/AnalyseValidateRequestAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5720 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/AnalyseValidateResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2764 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/AnalyseValidateResponseColumnAnalytics.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      797 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/CategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      990 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/CategoricalColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/CategoricalColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      959 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/CategoricalColumnInfoStats.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2073 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/CategoricalModelColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1557 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/CategoricalModelColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      529 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/CategoricalPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/CategoricalResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      547 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ColumnGroupBatchRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      720 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ColumnGroupPatchRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      600 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ColumnGroupRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ColumnGroupResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      545 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ColumnGroupResponseAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1582 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      624 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ColumnValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ColumnValueNullable.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1129 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ContinuousColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      582 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ContinuousColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ContinuousColumnInfoStats.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1676 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ContinuousModelColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1020 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ContinuousModelColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      802 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DRDatasetReductionData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DRDatasetReductionMetadata.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DRDatasetReductionMetadataSources.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1038 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DRJobReductionMetadata.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      725 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DRJobReductionMetadataSources.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1016 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DRModelReductionData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DROneDimensionPoint.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DRPCAReductionType.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DRThreeDimensionPoint.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DRTwoDimensionPoint.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DRUMAPReductionType.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      578 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/Data.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7250 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/Dataset.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/Dataset1.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DatasetChunk.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DatasetOrData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      571 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DatasetPatch.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1507 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DatasetQueryRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DatasetQueryRequestRowIDs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DatasetQueryRequestSort.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DatasetQueryResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DatasetQueryResponseResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61432 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DatasetsApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18436 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DefaultApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      791 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DependentColFnArgCol.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DependentColFnArgColWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      748 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DependentColFnArgConstantSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      731 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DependentColFnArgProduct.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      737 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DependentColFnArgRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DependentColFnArgSummandsWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      772 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DependentColFnArgWeightedConstSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      756 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DependentColFnArgWeightedRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DependentColFnArgZeroIfZero.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      661 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DependentColFnArgZeroIfZeroAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DependentColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DimensionalityReductionRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/DimensionalityReductionResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      881 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/EmptyCategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1021 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/EmptyContinuousColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1027 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/Error.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetAllOptJobs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1025 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetOptimizeDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      630 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetOptimizeDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetOptimizeFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetOptimizeFailedAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetOptimizeOptimizing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetOptimizeOptimizingAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetOptimizePending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetOptimizePendingAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1175 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalFailedAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalPending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalPendingAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalRunning.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalRunningAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestHistoricDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestHistoricDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1169 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestHistoricFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1144 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestHistoricPending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1186 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestHistoricRunning.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1206 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestInitialDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestInitialDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1210 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestInitialFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestInitialFailedAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestInitialPending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1183 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/GetSuggestInitialRunning.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/HistoricCategoricalPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/HistoricPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/HistoricScalarPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      700 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/HistoricTargetFunction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/HistoricValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/HistoricVectorPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/HistoricVectorValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ImportanceRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1583 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ImputeRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/IntCatArr.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/JobPatch.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/LoadRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/MetricsApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7976 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/Model.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2665 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ModelColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34815 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ModelDatasetApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ModelPatch.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ModelPermittedColumnRelationships.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   145583 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ModelsApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ModelsDatasetPutRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ModelsIdAdditiveSensitivityOrigin.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ModelsIdTrainPermittedColumnRelationships.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      773 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgCol.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      679 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgColAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      953 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgColWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgColWeightsAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgColWeightsAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      730 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgConstantSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgConstantSumAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgConstantSumAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgProduct.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgProductAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgProductAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      719 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgRatioAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgSummandsWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgSummandsWeightsAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      754 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedConstSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      660 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedConstSumAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      698 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      738 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedRatioAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      852 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedRatioAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      743 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgZeroIfZero.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColFnArgZeroIfZeroAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      799 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NewColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      770 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NonEmptyCategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      843 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NonEmptyContinuousColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      777 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/NonEmptyIntegerCategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1254 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OTSampleDefCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OTSampleDefContinuous.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OTSampleDefinition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      494 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OTSetInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2953 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OptimizeRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1255 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OutliersRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OutputToleranceRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OutputToleranceResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OutputToleranceResponseFixedInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OutputToleranceResponsePredictedOutputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OutputToleranceResponsePredictions.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      741 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OutputToleranceResponseSampledInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/OutputToleranceUnivariateResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartDependentColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartGetOptimize.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartGetOptimizeDoneResultArray.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1099 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartGetSuggestAdditional.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartGetSuggestHistoric.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1090 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartGetSuggestInitial.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartNewColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartTarFnAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartTarFnBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartTarFnBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartTarFnCategoricals.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1968 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartTarFnSingleTar.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartTarFnSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PartTarFnWeightedSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/PredictRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/Prediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/QueryRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/QueryResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SISampleDefCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SISampleDefinition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SampleDefCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SampleDefCategoricalColumnValues.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2029 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SampleDefComposition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1933 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SampleDefCompositionAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SampleDefContinuous.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SampleDefContinuousWithStart.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SampleDefDiscrete.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SampleDefInteger.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SampleDefStartProp.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SampleDefWeightedCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SampleDefinition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ScalarPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ScalarResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1196 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SensitivityRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SetInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      512 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ShareGroup.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      319 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/StringCatArr.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4837 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestAdditionalParameters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3870 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestAdditionalParametersAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestAdditionalRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestAdditionalRequestAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestAdditionalResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1050 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestHistoricParameters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestHistoricRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      922 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestHistoricResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1358 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestHistoricResultSamples.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestInitialParameters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestInitialRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      740 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestInitialRequestAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestInitialResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      393 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestInitialResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1440 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestMissingCommon.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2955 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestMissingData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      648 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestMissingDataAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3155 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestMissingDatasetID.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      848 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestMissingDatasetIDAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4011 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestMissingImputedData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestMissingImputedDataAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4589 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestMissingRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      909 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestMissingResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/SuggestMissingSpecific.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2090 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnAboveAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2090 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnBelowAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2164 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnBetweenAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2226 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnExcludeCategories.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      612 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnExcludeCategoriesAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2222 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnIncludeCategories.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnIncludeCategoriesAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnSumAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnSumAboveAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnSumBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnSumBelowAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1828 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnSumBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnSumBetweenAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnWeightedSumAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnWeightedSumAboveAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnWeightedSumBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnWeightedSumBelowAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1835 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnWeightedSumBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      678 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TarFnWeightedSumBetweenAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1592 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TargetFunction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5666 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TrainRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/TrainingDatasetOutliersRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1595 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ValidateRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1096 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/ValidationSplit.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/Value.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/VectorPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/VectorResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/VectorValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      945 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/docs/VersionResponse.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 09:27:44.020548 alchemite_apiclient-0.58.0/example/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   701201 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/adrenergic.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   243835 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/adrenergic_holdout.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1654 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/adrenergic_row.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/categorical.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/credentials_auth_code_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/credentials_client_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/credentials_pass_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/credentials_pass_prompted_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4545 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_additive_sensitivity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3944 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2775 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_chunk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4120 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_column_groups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_connect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5769 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_custom_validation_splits.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1175 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_delete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5634 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_dimensionality_reduction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      555 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_download.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1528 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_export_import.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4185 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_hyperopt.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3821 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_importance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5574 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_optimize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3169 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_outliers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4774 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_output_tolerance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4511 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_preload.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4054 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3823 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4492 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_sensitivity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5511 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_suggest_additional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5547 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_suggest_historic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1980 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_suggest_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4598 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_suggest_missing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3401 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_training_outliers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_validate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5497 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/example_vector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      759 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/optimize_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/optimize_args_vector.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1290 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/optimize_dependentColumns_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1189 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/steels.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/steels_impute.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      854 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/suggest_additional_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/suggest_additional_args_vector.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/suggest_historic_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/suggest_historic_args_vector.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/suggest_initial_args.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      503 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/example/vector.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-19 09:27:44.024548 alchemite_apiclient-0.58.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1178 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 09:27:44.024548 alchemite_apiclient-0.58.0/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_additive_sensitivity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2591 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2506 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1985 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_chunk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2873 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_column_groups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_connect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2255 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_cornercases.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3803 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_custom_validation_splits.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_delete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2493 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_dimensionality_reduction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      682 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_download.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3819 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_examples.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1538 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_hyperopt.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      932 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_importance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_optimize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_outliers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1848 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_output_tolerance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1502 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_preload.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_sensitivity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1042 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_suggest_additional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1152 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_suggest_historic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_suggest_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_suggest_missing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      489 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_training_outliers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      833 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_validate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2431 2023-07-19 09:27:36.000000 alchemite_apiclient-0.58.0/test/test_vector.py
```

### Comparing `alchemite_apiclient-0.57.0/PKG-INFO` & `alchemite_apiclient-0.58.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemite_apiclient
-Version: 0.57.0
+Version: 0.58.0
 Summary: A python API client for using Alchemite Analytics
 Home-page: 
 Author: Intellegens
 Author-email: Intellegens <support@intellegens.com>
 Project-URL: Homepage, https://intellegens.com
 Project-URL: Docs, https://docs.intellegens.com
 Keywords: Alchemite,Alchemite API,Machine Learning,Artificial Intelligence
@@ -19,15 +19,15 @@
 
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.57.0
+API version: 0.58.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.57.0/README.md` & `alchemite_apiclient-0.58.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.57.0
+API version: 0.58.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/__init__.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
     Contact: support@intellegens.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.57.0"
+__version__ = "0.58.0"
 
 # import ApiClient
 from alchemite_apiclient.api_client import ApiClient
 
 # import Configuration
 from alchemite_apiclient.configuration import Configuration
```

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/api/datasets_api.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/api/default_api.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/api/default_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/api/metrics_api.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/api/model_dataset_api.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/api/model_dataset_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/api/models_api.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/api/models_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1254,14 +1254,66 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.models_id_report_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (file_type,),
+                'auth': [
+                    'oauth'
+                ],
+                'endpoint_path': '/models/{id}/report',
+                'operation_id': 'models_id_report_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'id',
+                ],
+                'required': [
+                    'id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'id': 'id',
+                },
+                'location_map': {
+                    'id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/pdf',
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.models_id_sensitivity_put_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
                     'oauth'
                 ],
                 'endpoint_path': '/models/{id}/sensitivity',
@@ -4253,14 +4305,92 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['id'] = \
             id
         return self.models_id_predict_put_endpoint.call_with_http_info(**kwargs)
 
+    def models_id_report_get(
+        self,
+        id,
+        **kwargs
+    ):
+        """Get a PDF report for the model  # noqa: E501
+
+        Generate a PDF report for the chosen model. This report will contain statistical information on the training dataset, notable features of the model, and multiple plots explaining trends in the data.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.models_id_report_get(id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            id (str): Unique identifier for the model.
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            file_type
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['id'] = \
+            id
+        return self.models_id_report_get_endpoint.call_with_http_info(**kwargs)
+
     def models_id_sensitivity_put(
         self,
         id,
         **kwargs
     ):
         """Get model sensitivity at a point  # noqa: E501
```

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/api_client.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.57.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.58.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -205,14 +205,18 @@
 
         return_data = response_data
 
         if not _preload_content:
             return (return_data)
             return return_data
 
+        # DEV-3871 convert CSV files to strings
+        if 'text/csv' in response_data.getheader('content-type'):
+            response_type = (str,)
+
         # deserialize response data
         if response_type:
             if response_type != (file_type,):
                 encoding = "utf-8"
                 content_type = response_data.getheader('content-type')
                 if content_type is not None:
                     match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
```

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/apis/__init__.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/configuration.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,16 +403,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.57.0\n"\
-               "SDK Package Version: 0.57.0".\
+               "Version of the API: 0.58.0\n"\
+               "SDK Package Version: 0.58.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/exceptions.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/extensions.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/extensions.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/additive_sensitivity_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/additive_sensitivity_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/analyse_validate_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/analyse_validate_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/analyse_validate_request_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/analyse_validate_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/analyse_validate_response.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/analyse_validate_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_column.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_column_info.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_column_info_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_column_info_stats.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_column_info_stats.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_model_column_info.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_prediction.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/categorical_result.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/categorical_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_group_batch_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_group_batch_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_group_patch_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_group_patch_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_group_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_group_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_group_response.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_group_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_group_response_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_group_response_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_info.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_value.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/column_value_nullable.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/column_value_nullable.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/continuous_column_info.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/continuous_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/continuous_column_info_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/continuous_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/continuous_column_info_stats.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/continuous_column_info_stats.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/continuous_model_column_info.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/continuous_model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/data.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset1.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset1.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_chunk.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_chunk.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_or_data.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_or_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_patch.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_query_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_query_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_query_request_row_ids.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_query_request_row_ids.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_query_request_sort.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_query_request_sort.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_query_response.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_query_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dataset_query_response_result.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dataset_query_response_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dependent_columns.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dependent_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dimensionality_reduction_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dimensionality_reduction_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dimensionality_reduction_response.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dimensionality_reduction_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_dataset_reduction_data.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_dataset_reduction_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_job_reduction_metadata.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_job_reduction_metadata.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_model_reduction_data.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_model_reduction_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_one_dimension_point.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_one_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_three_dimension_point.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_three_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/dr_two_dimension_point.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/dr_two_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/drpca_reduction_type.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/drpca_reduction_type.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/drumap_reduction_type.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/drumap_reduction_type.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/empty_categorical_column.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/empty_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/empty_continuous_column.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/empty_continuous_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/error.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/error.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_all_opt_jobs.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_all_opt_jobs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_done.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_done_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_failed.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_failed_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_optimizing.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_optimizing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_pending.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_optimize_pending_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_optimize_pending_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_done.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_failed.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_pending.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_running.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_running.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_historic_done.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_historic_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_historic_failed.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_historic_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_historic_pending.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_historic_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_historic_running.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_historic_running.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_done.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_failed.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_pending.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/get_suggest_initial_running.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/get_suggest_initial_running.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_categorical_prediction.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_categorical_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_prediction.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_scalar_prediction.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_scalar_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_target_function.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_target_function.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_value.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_vector_prediction.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_vector_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/historic_vector_value.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/historic_vector_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/importance_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/importance_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/impute_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/impute_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/int_cat_arr.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/int_cat_arr.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/job_patch.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/job_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/load_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/load_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/model.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/model.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/model_column_info.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/model_patch.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/model_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/model_permitted_column_relationships.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/model_permitted_column_relationships.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/models_dataset_put_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/models_dataset_put_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_col.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_col.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_product.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_product.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/new_columns.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/new_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/non_empty_categorical_column.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/non_empty_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/non_empty_continuous_column.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/non_empty_continuous_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/optimize_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/optimize_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/ot_sample_def_categorical.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/ot_sample_def_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/ot_sample_def_continuous.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/ot_sample_def_continuous.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/ot_sample_definition.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/ot_sample_definition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/ot_set_inputs.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/ot_set_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/outliers_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/outliers_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_response.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_response_predictions.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_response_predictions.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/output_tolerance_univariate_response.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/output_tolerance_univariate_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_dependent_columns.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_dependent_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_get_optimize.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_get_optimize.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_get_suggest_additional.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_get_suggest_additional.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_get_suggest_historic.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_get_suggest_historic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_get_suggest_initial.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_get_suggest_initial.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_new_columns.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_new_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_above.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_below.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_between.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_categoricals.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_categoricals.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_single_tar.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_single_tar.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_sum.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/predict_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/predict_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/prediction.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/query_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/query_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/query_response.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/query_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_categorical.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_categorical_column_values.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_categorical_column_values.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_composition.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_composition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_composition_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_composition_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_continuous.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_continuous.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_continuous_with_start.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_continuous_with_start.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_discrete.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_discrete.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_integer.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_integer.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_start_prop.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_start_prop.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_def_weighted_categorical.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_def_weighted_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sample_definition.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sample_definition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/scalar_prediction.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/scalar_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/scalar_result.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/scalar_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/sensitivity_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/sensitivity_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/set_inputs.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/set_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/share_group.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/share_group.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/si_sample_def_categorical.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/si_sample_def_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/si_sample_definition.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/si_sample_definition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/string_cat_arr.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/string_cat_arr.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_additional_parameters.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_additional_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_additional_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_additional_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_additional_request_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_additional_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_additional_result.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_additional_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_historic_parameters.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_historic_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_historic_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_historic_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_historic_result.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_historic_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_historic_result_samples.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_historic_result_samples.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_initial_parameters.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_initial_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_initial_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_initial_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_initial_request_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_initial_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_initial_response.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_initial_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_initial_result.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_initial_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_common.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_common.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_data.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_data_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_data_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_dataset_id.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_dataset_id.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_imputed_data.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_imputed_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_response.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/suggest_missing_specific.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/suggest_missing_specific.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_above.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_above_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_below.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_below_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_between.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_between_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_exclude_categories.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_exclude_categories.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_include_categories.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_include_categories.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_above.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_below.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_between.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/target_function.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/target_function.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/train_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/train_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/training_dataset_outliers_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/training_dataset_outliers_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/validate_request.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/validate_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/validation_split.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/validation_split.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/value.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/vector_prediction.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/vector_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/vector_result.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/vector_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/vector_value.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/vector_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model/version_response.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model/version_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/model_utils.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/model_utils.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/models/__init__.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient/rest.py` & `alchemite_apiclient-0.58.0/alchemite_apiclient/rest.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient.egg-info/PKG-INFO` & `alchemite_apiclient-0.58.0/alchemite_apiclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemite-apiclient
-Version: 0.57.0
+Version: 0.58.0
 Summary: A python API client for using Alchemite Analytics
 Home-page: 
 Author: Intellegens
 Author-email: Intellegens <support@intellegens.com>
 Project-URL: Homepage, https://intellegens.com
 Project-URL: Docs, https://docs.intellegens.com
 Keywords: Alchemite,Alchemite API,Machine Learning,Artificial Intelligence
@@ -19,15 +19,15 @@
 
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.57.0
+API version: 0.58.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.57.0/alchemite_apiclient.egg-info/SOURCES.txt` & `alchemite_apiclient-0.58.0/alchemite_apiclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -541,14 +541,15 @@
 example/example_hyperopt.py
 example/example_importance.py
 example/example_optimize.py
 example/example_outliers.py
 example/example_output_tolerance.py
 example/example_preload.py
 example/example_query.py
+example/example_report.py
 example/example_sensitivity.py
 example/example_suggest_additional.py
 example/example_suggest_historic.py
 example/example_suggest_initial.py
 example/example_suggest_missing.py
 example/example_training_outliers.py
 example/example_validate.py
```

### Comparing `alchemite_apiclient-0.57.0/docs/AdditiveSensitivityRequest.md` & `alchemite_apiclient-0.58.0/docs/AdditiveSensitivityRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/AnalyseValidateRequest.md` & `alchemite_apiclient-0.58.0/docs/AnalyseValidateRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/AnalyseValidateRequestAllOf.md` & `alchemite_apiclient-0.58.0/docs/AnalyseValidateRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/AnalyseValidateResponse.md` & `alchemite_apiclient-0.58.0/docs/AnalyseValidateResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/AnalyseValidateResponseColumnAnalytics.md` & `alchemite_apiclient-0.58.0/docs/AnalyseValidateResponseColumnAnalytics.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/CategoricalColumn.md` & `alchemite_apiclient-0.58.0/docs/CategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/CategoricalColumnInfo.md` & `alchemite_apiclient-0.58.0/docs/CategoricalColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/CategoricalColumnInfoAllOf.md` & `alchemite_apiclient-0.58.0/docs/CategoricalColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/CategoricalColumnInfoStats.md` & `alchemite_apiclient-0.58.0/docs/CategoricalColumnInfoStats.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/CategoricalModelColumnInfo.md` & `alchemite_apiclient-0.58.0/docs/CategoricalModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/CategoricalModelColumnInfoAllOf.md` & `alchemite_apiclient-0.58.0/docs/CategoricalModelColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/CategoricalPrediction.md` & `alchemite_apiclient-0.58.0/docs/CategoricalPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/CategoricalResult.md` & `alchemite_apiclient-0.58.0/docs/CategoricalResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ColumnGroupBatchRequest.md` & `alchemite_apiclient-0.58.0/docs/ColumnGroupBatchRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ColumnGroupPatchRequest.md` & `alchemite_apiclient-0.58.0/docs/ColumnGroupPatchRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ColumnGroupRequest.md` & `alchemite_apiclient-0.58.0/docs/ColumnGroupRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ColumnGroupResponse.md` & `alchemite_apiclient-0.58.0/docs/ColumnGroupResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ColumnGroupResponseAllOf.md` & `alchemite_apiclient-0.58.0/docs/ColumnGroupResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ColumnInfo.md` & `alchemite_apiclient-0.58.0/docs/ColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ColumnValue.md` & `alchemite_apiclient-0.58.0/docs/ColumnValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ColumnValueNullable.md` & `alchemite_apiclient-0.58.0/docs/ColumnValueNullable.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ContinuousColumnInfo.md` & `alchemite_apiclient-0.58.0/docs/ContinuousColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ContinuousColumnInfoAllOf.md` & `alchemite_apiclient-0.58.0/docs/ContinuousColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ContinuousColumnInfoStats.md` & `alchemite_apiclient-0.58.0/docs/ContinuousColumnInfoStats.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ContinuousModelColumnInfo.md` & `alchemite_apiclient-0.58.0/docs/ContinuousModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ContinuousModelColumnInfoAllOf.md` & `alchemite_apiclient-0.58.0/docs/ContinuousModelColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DRDatasetReductionData.md` & `alchemite_apiclient-0.58.0/docs/DRDatasetReductionData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DRDatasetReductionMetadata.md` & `alchemite_apiclient-0.58.0/docs/DRDatasetReductionMetadata.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DRDatasetReductionMetadataSources.md` & `alchemite_apiclient-0.58.0/docs/DRDatasetReductionMetadataSources.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DRJobReductionMetadata.md` & `alchemite_apiclient-0.58.0/docs/DRJobReductionMetadata.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DRJobReductionMetadataSources.md` & `alchemite_apiclient-0.58.0/docs/DRJobReductionMetadataSources.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DRModelReductionData.md` & `alchemite_apiclient-0.58.0/docs/DRModelReductionData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DRPCAReductionType.md` & `alchemite_apiclient-0.58.0/docs/DRPCAReductionType.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DRThreeDimensionPoint.md` & `alchemite_apiclient-0.58.0/docs/DRThreeDimensionPoint.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DRTwoDimensionPoint.md` & `alchemite_apiclient-0.58.0/docs/DRTwoDimensionPoint.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DRUMAPReductionType.md` & `alchemite_apiclient-0.58.0/docs/DRUMAPReductionType.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/Data.md` & `alchemite_apiclient-0.58.0/docs/Data.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/Dataset.md` & `alchemite_apiclient-0.58.0/docs/Dataset.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/Dataset1.md` & `alchemite_apiclient-0.58.0/docs/Dataset1.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DatasetChunk.md` & `alchemite_apiclient-0.58.0/docs/DatasetChunk.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DatasetOrData.md` & `alchemite_apiclient-0.58.0/docs/DatasetOrData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DatasetPatch.md` & `alchemite_apiclient-0.58.0/docs/DatasetPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DatasetQueryRequest.md` & `alchemite_apiclient-0.58.0/docs/DatasetQueryRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DatasetQueryRequestRowIDs.md` & `alchemite_apiclient-0.58.0/docs/DatasetQueryRequestRowIDs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DatasetQueryRequestSort.md` & `alchemite_apiclient-0.58.0/docs/DatasetQueryRequestSort.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DatasetQueryResponseResult.md` & `alchemite_apiclient-0.58.0/docs/DatasetQueryResponseResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DatasetsApi.md` & `alchemite_apiclient-0.58.0/docs/DatasetsApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DefaultApi.md` & `alchemite_apiclient-0.58.0/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DependentColFnArgCol.md` & `alchemite_apiclient-0.58.0/docs/DependentColFnArgCol.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DependentColFnArgColWeights.md` & `alchemite_apiclient-0.58.0/docs/DependentColFnArgColWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DependentColFnArgConstantSum.md` & `alchemite_apiclient-0.58.0/docs/DependentColFnArgConstantSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DependentColFnArgProduct.md` & `alchemite_apiclient-0.58.0/docs/DependentColFnArgProduct.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DependentColFnArgRatio.md` & `alchemite_apiclient-0.58.0/docs/DependentColFnArgRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DependentColFnArgSummandsWeights.md` & `alchemite_apiclient-0.58.0/docs/DependentColFnArgSummandsWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DependentColFnArgWeightedConstSum.md` & `alchemite_apiclient-0.58.0/docs/DependentColFnArgWeightedConstSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DependentColFnArgWeightedRatio.md` & `alchemite_apiclient-0.58.0/docs/DependentColFnArgWeightedRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DependentColFnArgZeroIfZero.md` & `alchemite_apiclient-0.58.0/docs/DependentColFnArgZeroIfZero.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DependentColFnArgZeroIfZeroAllOf.md` & `alchemite_apiclient-0.58.0/docs/DependentColFnArgZeroIfZeroAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DependentColumns.md` & `alchemite_apiclient-0.58.0/docs/DependentColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DimensionalityReductionRequest.md` & `alchemite_apiclient-0.58.0/docs/DimensionalityReductionRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/DimensionalityReductionResponse.md` & `alchemite_apiclient-0.58.0/docs/DimensionalityReductionResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/EmptyCategoricalColumn.md` & `alchemite_apiclient-0.58.0/docs/EmptyCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/EmptyContinuousColumn.md` & `alchemite_apiclient-0.58.0/docs/EmptyContinuousColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/Error.md` & `alchemite_apiclient-0.58.0/docs/Error.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetOptimizeDone.md` & `alchemite_apiclient-0.58.0/docs/GetOptimizeDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetOptimizeDoneAllOf.md` & `alchemite_apiclient-0.58.0/docs/GetOptimizeDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetOptimizeFailed.md` & `alchemite_apiclient-0.58.0/docs/GetOptimizeFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetOptimizeFailedAllOf.md` & `alchemite_apiclient-0.58.0/docs/GetOptimizeFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetOptimizeOptimizing.md` & `alchemite_apiclient-0.58.0/docs/GetOptimizeOptimizing.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetOptimizeOptimizingAllOf.md` & `alchemite_apiclient-0.58.0/docs/GetOptimizeOptimizingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetOptimizePending.md` & `alchemite_apiclient-0.58.0/docs/GetOptimizePending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetOptimizePendingAllOf.md` & `alchemite_apiclient-0.58.0/docs/GetOptimizePendingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalDone.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalDoneAllOf.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalFailed.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalFailedAllOf.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalPending.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalPending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalPendingAllOf.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalPendingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalRunning.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalRunning.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestAdditionalRunningAllOf.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestAdditionalRunningAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestHistoricDone.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestHistoricDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestHistoricDoneAllOf.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestHistoricDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestHistoricFailed.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestHistoricFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestHistoricPending.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestHistoricPending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestHistoricRunning.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestHistoricRunning.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestInitialDone.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestInitialDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestInitialDoneAllOf.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestInitialDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestInitialFailed.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestInitialFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestInitialFailedAllOf.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestInitialFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestInitialPending.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestInitialPending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/GetSuggestInitialRunning.md` & `alchemite_apiclient-0.58.0/docs/GetSuggestInitialRunning.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/HistoricCategoricalPrediction.md` & `alchemite_apiclient-0.58.0/docs/HistoricCategoricalPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/HistoricPrediction.md` & `alchemite_apiclient-0.58.0/docs/HistoricPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/HistoricScalarPrediction.md` & `alchemite_apiclient-0.58.0/docs/HistoricScalarPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/HistoricTargetFunction.md` & `alchemite_apiclient-0.58.0/docs/HistoricTargetFunction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/HistoricValue.md` & `alchemite_apiclient-0.58.0/docs/HistoricValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/HistoricVectorPrediction.md` & `alchemite_apiclient-0.58.0/docs/HistoricVectorPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/HistoricVectorValue.md` & `alchemite_apiclient-0.58.0/docs/HistoricVectorValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ImportanceRequest.md` & `alchemite_apiclient-0.58.0/docs/ImportanceRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ImputeRequest.md` & `alchemite_apiclient-0.58.0/docs/ImputeRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/JobPatch.md` & `alchemite_apiclient-0.58.0/docs/JobPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/MetricsApi.md` & `alchemite_apiclient-0.58.0/docs/MetricsApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/Model.md` & `alchemite_apiclient-0.58.0/docs/Model.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ModelColumnInfo.md` & `alchemite_apiclient-0.58.0/docs/ModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ModelDatasetApi.md` & `alchemite_apiclient-0.58.0/docs/ModelDatasetApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ModelPatch.md` & `alchemite_apiclient-0.58.0/docs/ModelPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ModelPermittedColumnRelationships.md` & `alchemite_apiclient-0.58.0/docs/ModelPermittedColumnRelationships.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ModelsApi.md` & `alchemite_apiclient-0.58.0/docs/ModelsApi.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 [**models_id_optimize_job_id_patch**](ModelsApi.md#models_id_optimize_job_id_patch) | **PATCH** /models/{id}/optimize/{job_id} | Update an optimize jobs&#39;s metadata
 [**models_id_optimize_post**](ModelsApi.md#models_id_optimize_post) | **POST** /models/{id}/optimize | Optimize for specified targets using set of constraints
 [**models_id_outliers_put**](ModelsApi.md#models_id_outliers_put) | **PUT** /models/{id}/outliers | Find the outlying values in a dataset
 [**models_id_output_tolerance_put**](ModelsApi.md#models_id_output_tolerance_put) | **PUT** /models/{id}/output-tolerance | Get tolerance of predicted outputs from variations in inputs
 [**models_id_output_tolerance_univariate_put**](ModelsApi.md#models_id_output_tolerance_univariate_put) | **PUT** /models/{id}/output-tolerance-univariate | Get the univariate tolerances of predicted outputs from variations in inputs
 [**models_id_patch**](ModelsApi.md#models_id_patch) | **PATCH** /models/{id} | Update a model&#39;s metadata
 [**models_id_predict_put**](ModelsApi.md#models_id_predict_put) | **PUT** /models/{id}/predict | Predict given and missing data
+[**models_id_report_get**](ModelsApi.md#models_id_report_get) | **GET** /models/{id}/report | Get a PDF report for the model
 [**models_id_sensitivity_put**](ModelsApi.md#models_id_sensitivity_put) | **PUT** /models/{id}/sensitivity | Get model sensitivity at a point
 [**models_id_share_delete**](ModelsApi.md#models_id_share_delete) | **DELETE** /models/{id}/share | Stop sharing model with group
 [**models_id_share_get**](ModelsApi.md#models_id_share_get) | **GET** /models/{id}/share | Get groups with which model is shared
 [**models_id_share_put**](ModelsApi.md#models_id_share_put) | **PUT** /models/{id}/share | Share model with a group
 [**models_id_suggest_additional_get**](ModelsApi.md#models_id_suggest_additional_get) | **GET** /models/{id}/suggest-additional | Get all suggest-additional jobs for a model
 [**models_id_suggest_additional_job_id_delete**](ModelsApi.md#models_id_suggest_additional_job_id_delete) | **DELETE** /models/{id}/suggest-additional/{job_id} | Delete suggest-additional job
 [**models_id_suggest_additional_job_id_get**](ModelsApi.md#models_id_suggest_additional_job_id_get) | **GET** /models/{id}/suggest-additional/{job_id} | Get suggest-additional job data
@@ -1857,14 +1858,89 @@
 **200** | Returning predictions |  -  |
 **400** | Bad request, eg. CSV malformed or missing column headers |  -  |
 **401** | Licence expired |  -  |
 **404** | Model ID not found or model is not trained or has not been trained on the dataset attached to it. |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
+# **models_id_report_get**
+> file_type models_id_report_get(id)
+
+Get a PDF report for the model
+
+Generate a PDF report for the chosen model. This report will contain statistical information on the training dataset, notable features of the model, and multiple plots explaining trends in the data.
+
+### Example
+
+* OAuth Authentication (oauth):
+* OAuth Authentication (oauth):
+* OAuth Authentication (oauth):
+* OAuth Authentication (oauth):
+
+```python
+import time
+import alchemite_apiclient
+from alchemite_apiclient.api import models_api
+from alchemite_apiclient.model.error import Error
+from pprint import pprint
+from alchemite_apiclient.extensions import Configuration
+
+configuration = Configuration()
+
+# Provide path to the JSON containing your credentials
+configuration.credentials = "credentials.json"
+
+# Please see readme for details about the contents of credentials.json
+# Enter a context with an instance of the API client
+with alchemite_apiclient.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = models_api.ModelsApi(api_client)
+    id = "00112233-4455-6677-8899-aabbccddeeff" # str | Unique identifier for the model.
+
+    # example passing only required values which don't have defaults set
+    try:
+        # Get a PDF report for the model
+        api_response = api_instance.models_id_report_get(id)
+        pprint(api_response)
+    except alchemite_apiclient.ApiException as e:
+        print("Exception when calling ModelsApi->models_id_report_get: %s\n" % e)
+```
+
+
+### Parameters
+
+Name | Type | Description  | Notes
+------------- | ------------- | ------------- | -------------
+ **id** | **str**| Unique identifier for the model. |
+
+### Return type
+
+**file_type**
+
+### Authorization
+
+[oauth](../README.md#oauth), [oauth](../README.md#oauth), [oauth](../README.md#oauth), [oauth](../README.md#oauth)
+
+### HTTP request headers
+
+ - **Content-Type**: Not defined
+ - **Accept**: application/pdf, application/json
+
+
+### HTTP response details
+
+| Status code | Description | Response headers |
+|-------------|-------------|------------------|
+**200** | Returning model report |  -  |
+**202** | Report is being generated |  -  |
+**400** | Invalid model ID |  -  |
+**404** | Model ID not found |  -  |
+
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+
 # **models_id_sensitivity_put**
 > file_type models_id_sensitivity_put(id)
 
 Get model sensitivity at a point
 
 Generate a sensitivity analysis around a point. This reports how strongly each column depends on each other column at that point.
```

### Comparing `alchemite_apiclient-0.57.0/docs/ModelsIdAdditiveSensitivityOrigin.md` & `alchemite_apiclient-0.58.0/docs/ModelsIdAdditiveSensitivityOrigin.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ModelsIdTrainPermittedColumnRelationships.md` & `alchemite_apiclient-0.58.0/docs/ModelsIdTrainPermittedColumnRelationships.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgCol.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgCol.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgColAllOf.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgColAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgColWeights.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgColWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgColWeightsAllOf.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgColWeightsAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgColWeightsAllOfArguments.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgColWeightsAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgConstantSum.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgConstantSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgConstantSumAllOf.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgConstantSumAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgConstantSumAllOfArguments.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgConstantSumAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgProduct.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgProduct.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgProductAllOf.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgProductAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgProductAllOfArguments.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgProductAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgRatio.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgRatioAllOf.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgRatioAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgSummandsWeights.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgSummandsWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgSummandsWeightsAllOf.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgSummandsWeightsAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedConstSum.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedConstSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedConstSumAllOf.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedConstSumAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedRatio.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedRatioAllOf.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedRatioAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgWeightedRatioAllOfArguments.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgWeightedRatioAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgZeroIfZero.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgZeroIfZero.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColFnArgZeroIfZeroAllOf.md` & `alchemite_apiclient-0.58.0/docs/NewColFnArgZeroIfZeroAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NewColumns.md` & `alchemite_apiclient-0.58.0/docs/NewColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NonEmptyCategoricalColumn.md` & `alchemite_apiclient-0.58.0/docs/NonEmptyCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NonEmptyContinuousColumn.md` & `alchemite_apiclient-0.58.0/docs/NonEmptyContinuousColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/NonEmptyIntegerCategoricalColumn.md` & `alchemite_apiclient-0.58.0/docs/NonEmptyIntegerCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/OTSampleDefCategorical.md` & `alchemite_apiclient-0.58.0/docs/OTSampleDefCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/OTSampleDefContinuous.md` & `alchemite_apiclient-0.58.0/docs/OTSampleDefContinuous.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/OTSampleDefinition.md` & `alchemite_apiclient-0.58.0/docs/OTSampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/OptimizeRequest.md` & `alchemite_apiclient-0.58.0/docs/OptimizeRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/OutliersRequest.md` & `alchemite_apiclient-0.58.0/docs/OutliersRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/OutputToleranceRequest.md` & `alchemite_apiclient-0.58.0/docs/OutputToleranceRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/OutputToleranceResponse.md` & `alchemite_apiclient-0.58.0/docs/OutputToleranceResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/OutputToleranceResponseFixedInputs.md` & `alchemite_apiclient-0.58.0/docs/OutputToleranceResponseFixedInputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/OutputToleranceResponsePredictedOutputs.md` & `alchemite_apiclient-0.58.0/docs/OutputToleranceResponsePredictedOutputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/OutputToleranceResponsePredictions.md` & `alchemite_apiclient-0.58.0/docs/OutputToleranceResponsePredictions.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/OutputToleranceResponseSampledInputs.md` & `alchemite_apiclient-0.58.0/docs/OutputToleranceResponseSampledInputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PartDependentColumns.md` & `alchemite_apiclient-0.58.0/docs/PartDependentColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PartGetOptimize.md` & `alchemite_apiclient-0.58.0/docs/PartGetOptimize.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PartGetSuggestAdditional.md` & `alchemite_apiclient-0.58.0/docs/PartGetSuggestAdditional.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PartGetSuggestHistoric.md` & `alchemite_apiclient-0.58.0/docs/PartGetSuggestHistoric.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PartGetSuggestInitial.md` & `alchemite_apiclient-0.58.0/docs/PartGetSuggestInitial.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PartNewColumns.md` & `alchemite_apiclient-0.58.0/docs/PartNewColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PartTarFnBetween.md` & `alchemite_apiclient-0.58.0/docs/PartTarFnBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PartTarFnCategoricals.md` & `alchemite_apiclient-0.58.0/docs/PartTarFnCategoricals.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PartTarFnSingleTar.md` & `alchemite_apiclient-0.58.0/docs/PartTarFnSingleTar.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PartTarFnSum.md` & `alchemite_apiclient-0.58.0/docs/PartTarFnSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PartTarFnWeightedSum.md` & `alchemite_apiclient-0.58.0/docs/PartTarFnWeightedSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/PredictRequest.md` & `alchemite_apiclient-0.58.0/docs/PredictRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/Prediction.md` & `alchemite_apiclient-0.58.0/docs/Prediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/QueryRequest.md` & `alchemite_apiclient-0.58.0/docs/QueryRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/QueryResponse.md` & `alchemite_apiclient-0.58.0/docs/QueryResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SISampleDefCategorical.md` & `alchemite_apiclient-0.58.0/docs/SISampleDefCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SISampleDefinition.md` & `alchemite_apiclient-0.58.0/docs/SISampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SampleDefCategorical.md` & `alchemite_apiclient-0.58.0/docs/SampleDefCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SampleDefCategoricalColumnValues.md` & `alchemite_apiclient-0.58.0/docs/SampleDefCategoricalColumnValues.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SampleDefComposition.md` & `alchemite_apiclient-0.58.0/docs/SampleDefComposition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SampleDefCompositionAllOf.md` & `alchemite_apiclient-0.58.0/docs/SampleDefCompositionAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SampleDefContinuous.md` & `alchemite_apiclient-0.58.0/docs/SampleDefContinuous.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SampleDefContinuousWithStart.md` & `alchemite_apiclient-0.58.0/docs/SampleDefContinuousWithStart.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SampleDefDiscrete.md` & `alchemite_apiclient-0.58.0/docs/SampleDefDiscrete.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SampleDefInteger.md` & `alchemite_apiclient-0.58.0/docs/SampleDefInteger.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SampleDefStartProp.md` & `alchemite_apiclient-0.58.0/docs/SampleDefStartProp.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SampleDefWeightedCategorical.md` & `alchemite_apiclient-0.58.0/docs/SampleDefWeightedCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SampleDefinition.md` & `alchemite_apiclient-0.58.0/docs/SampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ScalarPrediction.md` & `alchemite_apiclient-0.58.0/docs/ScalarPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ScalarResult.md` & `alchemite_apiclient-0.58.0/docs/ScalarResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SensitivityRequest.md` & `alchemite_apiclient-0.58.0/docs/SensitivityRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ShareGroup.md` & `alchemite_apiclient-0.58.0/docs/ShareGroup.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestAdditionalParameters.md` & `alchemite_apiclient-0.58.0/docs/SuggestAdditionalParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestAdditionalParametersAllOf.md` & `alchemite_apiclient-0.58.0/docs/SuggestAdditionalParametersAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestAdditionalRequest.md` & `alchemite_apiclient-0.58.0/docs/SuggestAdditionalRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestAdditionalRequestAllOf.md` & `alchemite_apiclient-0.58.0/docs/SuggestAdditionalRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestHistoricParameters.md` & `alchemite_apiclient-0.58.0/docs/SuggestHistoricParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestHistoricRequest.md` & `alchemite_apiclient-0.58.0/docs/SuggestHistoricRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestHistoricResult.md` & `alchemite_apiclient-0.58.0/docs/SuggestHistoricResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestHistoricResultSamples.md` & `alchemite_apiclient-0.58.0/docs/SuggestHistoricResultSamples.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestInitialParameters.md` & `alchemite_apiclient-0.58.0/docs/SuggestInitialParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestInitialRequest.md` & `alchemite_apiclient-0.58.0/docs/SuggestInitialRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestInitialRequestAllOf.md` & `alchemite_apiclient-0.58.0/docs/SuggestInitialRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestInitialResponse.md` & `alchemite_apiclient-0.58.0/docs/SuggestInitialResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestMissingCommon.md` & `alchemite_apiclient-0.58.0/docs/SuggestMissingCommon.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestMissingData.md` & `alchemite_apiclient-0.58.0/docs/SuggestMissingData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestMissingDataAllOf.md` & `alchemite_apiclient-0.58.0/docs/SuggestMissingDataAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestMissingDatasetID.md` & `alchemite_apiclient-0.58.0/docs/SuggestMissingDatasetID.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestMissingDatasetIDAllOf.md` & `alchemite_apiclient-0.58.0/docs/SuggestMissingDatasetIDAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestMissingImputedData.md` & `alchemite_apiclient-0.58.0/docs/SuggestMissingImputedData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestMissingImputedDataAllOf.md` & `alchemite_apiclient-0.58.0/docs/SuggestMissingImputedDataAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestMissingRequest.md` & `alchemite_apiclient-0.58.0/docs/SuggestMissingRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestMissingResponse.md` & `alchemite_apiclient-0.58.0/docs/SuggestMissingResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/SuggestMissingSpecific.md` & `alchemite_apiclient-0.58.0/docs/SuggestMissingSpecific.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnAbove.md` & `alchemite_apiclient-0.58.0/docs/TarFnAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnAboveAllOf.md` & `alchemite_apiclient-0.58.0/docs/TarFnAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnBelow.md` & `alchemite_apiclient-0.58.0/docs/TarFnBelow.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnBelowAllOf.md` & `alchemite_apiclient-0.58.0/docs/TarFnBelowAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnBetween.md` & `alchemite_apiclient-0.58.0/docs/TarFnBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnBetweenAllOf.md` & `alchemite_apiclient-0.58.0/docs/TarFnBetweenAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnExcludeCategories.md` & `alchemite_apiclient-0.58.0/docs/TarFnExcludeCategories.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnExcludeCategoriesAllOf.md` & `alchemite_apiclient-0.58.0/docs/TarFnExcludeCategoriesAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnIncludeCategories.md` & `alchemite_apiclient-0.58.0/docs/TarFnIncludeCategories.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnIncludeCategoriesAllOf.md` & `alchemite_apiclient-0.58.0/docs/TarFnIncludeCategoriesAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnSumAbove.md` & `alchemite_apiclient-0.58.0/docs/TarFnSumAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnSumAboveAllOf.md` & `alchemite_apiclient-0.58.0/docs/TarFnSumAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnSumBelow.md` & `alchemite_apiclient-0.58.0/docs/TarFnSumBelow.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnSumBelowAllOf.md` & `alchemite_apiclient-0.58.0/docs/TarFnSumBelowAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnSumBetween.md` & `alchemite_apiclient-0.58.0/docs/TarFnSumBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnSumBetweenAllOf.md` & `alchemite_apiclient-0.58.0/docs/TarFnSumBetweenAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnWeightedSumAbove.md` & `alchemite_apiclient-0.58.0/docs/TarFnWeightedSumAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnWeightedSumAboveAllOf.md` & `alchemite_apiclient-0.58.0/docs/TarFnWeightedSumAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnWeightedSumBelow.md` & `alchemite_apiclient-0.58.0/docs/TarFnWeightedSumBelow.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnWeightedSumBelowAllOf.md` & `alchemite_apiclient-0.58.0/docs/TarFnWeightedSumBelowAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnWeightedSumBetween.md` & `alchemite_apiclient-0.58.0/docs/TarFnWeightedSumBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TarFnWeightedSumBetweenAllOf.md` & `alchemite_apiclient-0.58.0/docs/TarFnWeightedSumBetweenAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TargetFunction.md` & `alchemite_apiclient-0.58.0/docs/TargetFunction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/TrainRequest.md` & `alchemite_apiclient-0.58.0/docs/TrainRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ValidateRequest.md` & `alchemite_apiclient-0.58.0/docs/ValidateRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/ValidationSplit.md` & `alchemite_apiclient-0.58.0/docs/ValidationSplit.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/Value.md` & `alchemite_apiclient-0.58.0/docs/Value.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/VectorPrediction.md` & `alchemite_apiclient-0.58.0/docs/VectorPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/VectorResult.md` & `alchemite_apiclient-0.58.0/docs/VectorResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/VectorValue.md` & `alchemite_apiclient-0.58.0/docs/VectorValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/docs/VersionResponse.md` & `alchemite_apiclient-0.58.0/docs/VersionResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/adrenergic.csv` & `alchemite_apiclient-0.58.0/example/adrenergic.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/adrenergic_holdout.csv` & `alchemite_apiclient-0.58.0/example/adrenergic_holdout.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/adrenergic_row.csv` & `alchemite_apiclient-0.58.0/example/adrenergic_row.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/categorical.csv` & `alchemite_apiclient-0.58.0/example/categorical.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_additive_sensitivity.py` & `alchemite_apiclient-0.58.0/example/example_additive_sensitivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,13 +102,11 @@
     ]
 }
 
 ############################################################################
 ### Get the sensitivity matrix of each column based on our input data point
 ############################################################################
 r = api_models.models_id_additive_sensitivity_put(
-    model_id,
-    additive_sensitivity_request=additive_sensitivity_request,
-    _preload_content=False,
+    model_id, additive_sensitivity_request=additive_sensitivity_request
 )
-with open(additive_sensitivity_output_file, "wb") as f:
-    f.write(r.data)
+with open(additive_sensitivity_output_file, "w", encoding="UTF-8") as f:
+    f.write(r)
```

### Comparing `alchemite_apiclient-0.57.0/example/example_basic.py` & `alchemite_apiclient-0.58.0/example/example_basic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_categorical.py` & `alchemite_apiclient-0.58.0/example/example_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_chunk.py` & `alchemite_apiclient-0.58.0/example/example_chunk.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_column_groups.py` & `alchemite_apiclient-0.58.0/example/example_column_groups.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_connect.py` & `alchemite_apiclient-0.58.0/example/example_connect.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_custom_validation_splits.py` & `alchemite_apiclient-0.58.0/example/example_custom_validation_splits.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_delete.py` & `alchemite_apiclient-0.58.0/example/example_delete.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_dimensionality_reduction.py` & `alchemite_apiclient-0.58.0/example/example_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_download.py` & `alchemite_apiclient-0.58.0/example/example_download.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,12 +7,10 @@
 api_datasets = client.DatasetsApi(client.ApiClient(configuration))
 
 # Provide path to the JSON containing your credentials
 configuration.credentials = "credentials.json"
 
 dataset_id_to_download = "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
 
-r = api_datasets.datasets_id_download_get(
-    dataset_id_to_download, _preload_content=False
-)
+r = api_datasets.datasets_id_download_get(dataset_id_to_download)
 with open(dataset_id_to_download + ".csv", "w", encoding="UTF-8") as f:
-    f.write(r.data.decode())
+    f.write(r)
```

### Comparing `alchemite_apiclient-0.57.0/example/example_export_import.py` & `alchemite_apiclient-0.58.0/example/example_export_import.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 model_id = "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
 #######################
 
 ### Export model
 # - This zip file contains the model and its metadata.  The zip file does not
 # contain the training dataset itself, although it may contain some summary
 # statistics about the model's training dataset (eg. min, max, mean)
-response = api_models.models_id_export_get(model_id, _preload_content=False)
-with open("exported_model.zip", "wb") as f:
-    f.write(response.data)
+model_file = api_models.models_id_export_get(model_id)
+with open("exported_model.zip", "wb") as f, model_file:
+    f.write(model_file.read())
 
 
 ### Import model
 # - If a model with the same ID already exists then a new ID will be created
 # for the imported model
 # - If the user importing the model is not the same user who uploaded the training
 # dataset then they will not be able to access that dataset.  Therefore certain
```

### Comparing `alchemite_apiclient-0.57.0/example/example_hyperopt.py` & `alchemite_apiclient-0.58.0/example/example_hyperopt.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_importance.py` & `alchemite_apiclient-0.58.0/example/example_importance.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,11 +87,11 @@
 ############################################################################
 importance_request = {
     # This flag will cause Alchemite to only return descriptor-to-target relationships if set to True.
     # Otherwise, target-to-target relationships will also be returned
     "useOnlyDescriptors": True
 }
 r = api_models.models_id_importance_put(
-    model_id, importance_request=importance_request, _preload_content=False
+    model_id, importance_request=importance_request
 )
-with open(importance_output_file, "wb") as f:
-    f.write(r.data)
+with open(importance_output_file, "w", encoding="UTF-8") as f:
+    f.write(r)
```

### Comparing `alchemite_apiclient-0.57.0/example/example_optimize.py` & `alchemite_apiclient-0.58.0/example/example_optimize.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_outliers.py` & `alchemite_apiclient-0.58.0/example/example_outliers.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 model = await_trained(lambda: api_models.models_id_get(model_id))
 
 ################################################################################
 ### Identify outliers in the model's training dataset
 ################################################################################
 outliers_request = {"dataset_id": dataset_id}
 response = api_models.models_id_outliers_put(
-    model_id, outliers_request=outliers_request, _preload_content=False
+    model_id, outliers_request=outliers_request
 )
-with open(output_outliers_file, "wb") as f:
-    f.write(response.data)
+with open(output_outliers_file, "w", encoding="UTF-8") as f:
+    f.write(response)
 
 ### Delete model and dataset
 api_models.models_id_delete(model_id)
 api_datasets.datasets_id_delete(dataset_id)
```

### Comparing `alchemite_apiclient-0.57.0/example/example_output_tolerance.py` & `alchemite_apiclient-0.58.0/example/example_output_tolerance.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_preload.py` & `alchemite_apiclient-0.58.0/example/example_preload.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_query.py` & `alchemite_apiclient-0.58.0/example/example_query.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_sensitivity.py` & `alchemite_apiclient-0.58.0/example/example_sensitivity.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,11 +102,11 @@
     ]
 }
 
 ############################################################################
 ### Get the sensitivity matrix of each column based on our input data point
 ############################################################################
 r = api_models.models_id_sensitivity_put(
-    model_id, sensitivity_request=sensitivity_request, _preload_content=False
+    model_id, sensitivity_request=sensitivity_request
 )
-with open(sensitivity_output_file, "wb") as f:
-    f.write(r.data)
+with open(sensitivity_output_file, "w", encoding="UTF-8") as f:
+    f.write(r)
```

### Comparing `alchemite_apiclient-0.57.0/example/example_suggest_additional.py` & `alchemite_apiclient-0.58.0/example/example_suggest_additional.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_suggest_historic.py` & `alchemite_apiclient-0.58.0/example/example_suggest_historic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_suggest_initial.py` & `alchemite_apiclient-0.58.0/example/example_suggest_initial.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_suggest_missing.py` & `alchemite_apiclient-0.58.0/example/example_suggest_missing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_training_outliers.py` & `alchemite_apiclient-0.58.0/example/example_training_outliers.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,12 +81,10 @@
 model = await_trained(lambda: api_models.models_id_get(model_id))
 print("--- model hyperparameters ---")
 print(model.training_hyperparameters)
 
 ############################################################################
 ### Get the training dataset outliers
 ############################################################################
-response = api_models.models_id_training_dataset_outliers_get(
-    model_id, _preload_content=False
-)
-with open(training_datset_outliers_file, "wb") as f:
-    f.write(response.data)
+response = api_models.models_id_training_dataset_outliers_put(model_id)
+with open(training_datset_outliers_file, "w", encoding="UTF-8") as f:
+    f.write(response)
```

### Comparing `alchemite_apiclient-0.57.0/example/example_validate.py` & `alchemite_apiclient-0.58.0/example/example_validate.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/example_vector.py` & `alchemite_apiclient-0.58.0/example/example_vector.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/optimize_args_steel.json` & `alchemite_apiclient-0.58.0/example/optimize_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/optimize_dependentColumns_args_steel.json` & `alchemite_apiclient-0.58.0/example/optimize_dependentColumns_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/steels.csv` & `alchemite_apiclient-0.58.0/example/steels.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/example/suggest_additional_args_steel.json` & `alchemite_apiclient-0.58.0/example/suggest_additional_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/pyproject.toml` & `alchemite_apiclient-0.58.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alchemite_apiclient"
-version = "0.57.0"
+version = "0.58.0"
 authors = [
   { name="Intellegens", email="support@intellegens.com" },
 ]
 description = "A python API client for using Alchemite Analytics"
 keywords = ["Alchemite", "Alchemite API", "Machine Learning", "Artificial Intelligence"]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `alchemite_apiclient-0.57.0/setup.py` & `alchemite_apiclient-0.58.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "alchemite-apiclient"
-VERSION = "0.57.0"
+VERSION = "0.58.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `alchemite_apiclient-0.57.0/test/test_additive_sensitivity.py` & `alchemite_apiclient-0.58.0/test/test_additive_sensitivity.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_basic.py` & `alchemite_apiclient-0.58.0/test/test_basic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_categorical.py` & `alchemite_apiclient-0.58.0/test/test_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_chunk.py` & `alchemite_apiclient-0.58.0/test/test_chunk.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_column_groups.py` & `alchemite_apiclient-0.58.0/test/test_column_groups.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_cornercases.py` & `alchemite_apiclient-0.58.0/test/test_cornercases.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_custom_validation_splits.py` & `alchemite_apiclient-0.58.0/test/test_custom_validation_splits.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_delete.py` & `alchemite_apiclient-0.58.0/test/test_delete.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_dimensionality_reduction.py` & `alchemite_apiclient-0.58.0/test/test_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_download.py` & `alchemite_apiclient-0.58.0/test/test_download.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_examples.py` & `alchemite_apiclient-0.58.0/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_hyperopt.py` & `alchemite_apiclient-0.58.0/test/test_hyperopt.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_importance.py` & `alchemite_apiclient-0.58.0/test/test_importance.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_optimize.py` & `alchemite_apiclient-0.58.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_output_tolerance.py` & `alchemite_apiclient-0.58.0/test/test_output_tolerance.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_preload.py` & `alchemite_apiclient-0.58.0/test/test_preload.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_query.py` & `alchemite_apiclient-0.58.0/test/test_query.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_sensitivity.py` & `alchemite_apiclient-0.58.0/test/test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_suggest_additional.py` & `alchemite_apiclient-0.58.0/test/test_suggest_additional.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_suggest_historic.py` & `alchemite_apiclient-0.58.0/test/test_suggest_historic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_suggest_initial.py` & `alchemite_apiclient-0.58.0/test/test_suggest_initial.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_suggest_missing.py` & `alchemite_apiclient-0.58.0/test/test_suggest_missing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_validate.py` & `alchemite_apiclient-0.58.0/test/test_validate.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.57.0/test/test_vector.py` & `alchemite_apiclient-0.58.0/test/test_vector.py`

 * *Files identical despite different names*

