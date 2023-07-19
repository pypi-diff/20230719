# Comparing `tmp/splink-3.9.3.tar.gz` & `tmp/splink-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splink-3.9.3.tar", max compression
+gzip compressed data, was "splink-3.9.4.tar", max compression
```

## Comparing `splink-3.9.3.tar` & `splink-3.9.4.tar`

### file list

```diff
@@ -1,150 +1,162 @@
--rw-r--r--   0        0        0     1076 2023-07-05 16:14:53.842971 splink-3.9.3/LICENSE
--rw-r--r--   0        0        0     8777 2023-07-05 16:14:53.842971 splink-3.9.3/README.md
--rw-r--r--   0        0        0     2110 2023-07-05 16:14:53.878971 splink-3.9.3/pyproject.toml
--rw-r--r--   0        0        0       23 2023-07-05 16:14:53.882971 splink-3.9.3/splink/__init__.py
--rw-r--r--   0        0        0    10852 2023-07-05 16:14:53.882971 splink-3.9.3/splink/accuracy.py
--rw-r--r--   0        0        0     4803 2023-07-05 16:14:53.882971 splink-3.9.3/splink/analyse_blocking.py
--rw-r--r--   0        0        0      387 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_comparison_library.py
--rw-r--r--   0        0        0      396 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_comparison_template_library.py
--rw-r--r--   0        0        0     1365 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_helpers/athena_base.py
--rw-r--r--   0        0        0     3322 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_helpers/athena_comparison_imports.py
--rw-r--r--   0        0        0      350 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_helpers/athena_transforms.py
--rw-r--r--   0        0        0     2903 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_helpers/athena_utils.py
--rw-r--r--   0        0        0      361 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/athena_linker.py
--rw-r--r--   0        0        0      386 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/comparison_level_library.py
--rw-r--r--   0        0        0      249 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/comparison_library.py
--rw-r--r--   0        0        0      252 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/comparison_template_library.py
--rw-r--r--   0        0        0    21171 2023-07-05 16:14:53.882971 splink-3.9.3/splink/athena/linker.py
--rw-r--r--   0        0        0     2867 2023-07-05 16:14:53.882971 splink-3.9.3/splink/block_from_labels.py
--rw-r--r--   0        0        0     6439 2023-07-05 16:14:53.882971 splink-3.9.3/splink/blocking.py
--rw-r--r--   0        0        0     2223 2023-07-05 16:14:53.882971 splink-3.9.3/splink/cache_dict_with_logging.py
--rw-r--r--   0        0        0    11249 2023-07-05 16:14:53.882971 splink-3.9.3/splink/charts.py
--rw-r--r--   0        0        0     9266 2023-07-05 16:14:53.882971 splink-3.9.3/splink/cluster_studio.py
--rw-r--r--   0        0        0    16881 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison.py
--rw-r--r--   0        0        0     8766 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_helpers.py
--rw-r--r--   0        0        0      554 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_helpers_utils.py
--rw-r--r--   0        0        0    25479 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_level.py
--rw-r--r--   0        0        0    16560 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_level_composition.py
--rw-r--r--   0        0        0    57737 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_level_library.py
--rw-r--r--   0        0        0     1237 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_level_sql.py
--rw-r--r--   0        0        0    63328 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_library.py
--rw-r--r--   0        0        0     4922 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_library_utils.py
--rw-r--r--   0        0        0    81390 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_template_library.py
--rw-r--r--   0        0        0      972 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_vector_distribution.py
--rw-r--r--   0        0        0      868 2023-07-05 16:14:53.882971 splink-3.9.3/splink/comparison_vector_values.py
--rw-r--r--   0        0        0    16699 2023-07-05 16:14:53.882971 splink-3.9.3/splink/connected_components.py
--rw-r--r--   0        0        0       67 2023-07-05 16:14:53.882971 splink-3.9.3/splink/constants.py
--rw-r--r--   0        0        0     6089 2023-07-05 16:14:53.882971 splink-3.9.3/splink/convert_v2_to_v3.py
--rw-r--r--   0        0        0     1338 2023-07-05 16:14:53.882971 splink-3.9.3/splink/databricks/enable_splink.py
--rw-r--r--   0        0        0     5562 2023-07-05 16:14:53.882971 splink-3.9.3/splink/datasets/__init__.py
--rw-r--r--   0        0        0      609 2023-07-05 16:14:53.882971 splink-3.9.3/splink/default_from_jsonschema.py
--rw-r--r--   0        0        0     1608 2023-07-05 16:14:53.882971 splink-3.9.3/splink/dialect_base.py
--rw-r--r--   0        0        0      476 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/comparison_level_library.py
--rw-r--r--   0        0        0      371 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/comparison_library.py
--rw-r--r--   0        0        0      194 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/comparison_template_library.py
--rw-r--r--   0        0        0      387 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_comparison_library.py
--rw-r--r--   0        0        0      396 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_comparison_template_library.py
--rw-r--r--   0        0        0     1555 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_base.py
--rw-r--r--   0        0        0     5623 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py
--rw-r--r--   0        0        0     1750 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_helpers.py
--rw-r--r--   0        0        0      367 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/duckdb_linker.py
--rw-r--r--   0        0        0    11906 2023-07-05 16:14:53.882971 splink-3.9.3/splink/duckdb/linker.py
--rw-r--r--   0        0        0    17650 2023-07-05 16:14:53.882971 splink-3.9.3/splink/em_training_session.py
--rw-r--r--   0        0        0     5743 2023-07-05 16:14:53.882971 splink-3.9.3/splink/estimate_u.py
--rw-r--r--   0        0        0      269 2023-07-05 16:14:53.882971 splink-3.9.3/splink/exceptions.py
--rw-r--r--   0        0        0     9070 2023-07-05 16:14:53.882971 splink-3.9.3/splink/expectation_maximisation.py
--rw-r--r--   0        0        0     1562 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/blocking_rule_generated_comparisons.json
--rw-r--r--   0        0        0     5153 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/comparator_score_chart.json
--rw-r--r--   0        0        0     1836 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/comparator_score_threshold_chart.json
--rw-r--r--   0        0        0     2775 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/completeness.json
--rw-r--r--   0        0        0     5795 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/m_u_parameters_interactive_history.json
--rw-r--r--   0        0        0     1111 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/match_weight_histogram.json
--rw-r--r--   0        0        0     5691 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/match_weights_interactive_history.json
--rw-r--r--   0        0        0     9113 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/match_weights_waterfall.json
--rw-r--r--   0        0        0     1714 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/missingness.json
--rw-r--r--   0        0        0     2753 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/parameter_estimate_comparisons.json
--rw-r--r--   0        0        0     1891 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/phonetic_match_chart.json
--rw-r--r--   0        0        0     1654 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/precision_recall.json
--rw-r--r--   0        0        0     1125 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/probability_two_random_records_match_iteration.json
--rw-r--r--   0        0        0     2326 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/profile_data.json
--rw-r--r--   0        0        0     1805 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/roc.json
--rw-r--r--   0        0        0     9910 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/tf_adjustment_chart.json
--rw-r--r--   0        0        0     2910 2023-07-05 16:14:53.882971 splink-3.9.3/splink/files/chart_defs/unlinkables_chart_def.json
--rw-r--r--   0        0        0    66064 2023-07-05 16:14:53.886971 splink-3.9.3/splink/files/external_js/vega-embed@6.20.2
--rw-r--r--   0        0        0   256817 2023-07-05 16:14:53.886971 splink-3.9.3/splink/files/external_js/vega-lite@5.2.0
--rw-r--r--   0        0        0   501599 2023-07-05 16:14:53.890971 splink-3.9.3/splink/files/external_js/vega@5.21.0
--rw-r--r--   0        0        0   974616 2023-07-05 16:14:53.894971 splink-3.9.3/splink/files/labelling_tool/slt.js
--rw-r--r--   0        0        0     2971 2023-07-05 16:14:53.894971 splink-3.9.3/splink/files/labelling_tool/template.j2
--rw-r--r--   0        0        0    13833 2023-07-05 16:14:53.894971 splink-3.9.3/splink/files/settings_jsonschema.json
--rw-r--r--   0        0        0  1228220 2023-07-05 16:14:53.898971 splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
--rw-r--r--   0        0        0   944614 2023-07-05 16:14:53.906971 splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
--rw-r--r--   0        0        0   949562 2023-07-05 16:14:53.910971 splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
--rw-r--r--   0        0        0     5486 2023-07-05 16:14:53.910971 splink-3.9.3/splink/files/splink_cluster_studio/cluster_template.j2
--rw-r--r--   0        0        0     2269 2023-07-05 16:14:53.910971 splink-3.9.3/splink/files/splink_cluster_studio/custom.css
--rw-r--r--   0        0        0     2269 2023-07-05 16:14:53.910971 splink-3.9.3/splink/files/splink_comparison_viewer/custom.css
--rw-r--r--   0        0        0     3115 2023-07-05 16:14:53.910971 splink-3.9.3/splink/files/splink_comparison_viewer/template.j2
--rw-r--r--   0        0        0   269522 2023-07-05 16:14:53.914971 splink-3.9.3/splink/files/splink_vis_utils/splink_vis_utils.js
--rw-r--r--   0        0        0      404 2023-07-05 16:14:53.914971 splink-3.9.3/splink/files/templates/single_chart_template.txt
--rw-r--r--   0        0        0      195 2023-07-05 16:14:53.914971 splink-3.9.3/splink/format_sql.py
--rw-r--r--   0        0        0     7955 2023-07-05 16:14:53.914971 splink-3.9.3/splink/input_column.py
--rw-r--r--   0        0        0     3413 2023-07-05 16:14:53.914971 splink-3.9.3/splink/labelling_tool.py
--rw-r--r--   0        0        0   133602 2023-07-05 16:14:53.914971 splink-3.9.3/splink/linker.py
--rw-r--r--   0        0        0      300 2023-07-05 16:14:53.914971 splink-3.9.3/splink/logging_messages.py
--rw-r--r--   0        0        0     3132 2023-07-05 16:14:53.914971 splink-3.9.3/splink/lower_id_on_lhs.py
--rw-r--r--   0        0        0     1834 2023-07-05 16:14:53.914971 splink-3.9.3/splink/m_from_labels.py
--rw-r--r--   0        0        0     2465 2023-07-05 16:14:53.914971 splink-3.9.3/splink/m_training.py
--rw-r--r--   0        0        0     2420 2023-07-05 16:14:53.914971 splink-3.9.3/splink/m_u_records_to_parameters.py
--rw-r--r--   0        0        0      623 2023-07-05 16:14:53.914971 splink-3.9.3/splink/match_key_analysis.py
--rw-r--r--   0        0        0     2028 2023-07-05 16:14:53.914971 splink-3.9.3/splink/match_weights_histogram.py
--rw-r--r--   0        0        0     5911 2023-07-05 16:14:53.914971 splink-3.9.3/splink/misc.py
--rw-r--r--   0        0        0     2791 2023-07-05 16:14:53.914971 splink-3.9.3/splink/missingness.py
--rw-r--r--   0        0        0     1221 2023-07-05 16:14:53.914971 splink-3.9.3/splink/parse_sql.py
--rw-r--r--   0        0        0     2909 2023-07-05 16:14:53.914971 splink-3.9.3/splink/pipeline.py
--rw-r--r--   0        0        0      390 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/comparison_level_library.py
--rw-r--r--   0        0        0      253 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/comparison_library.py
--rw-r--r--   0        0        0      394 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/comparison_template_library.py
--rw-r--r--   0        0        0    10873 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/linker.py
--rw-r--r--   0        0        0      393 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_comparison_level_library.py
--rw-r--r--   0        0        0      375 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_comparison_library.py
--rw-r--r--   0        0        0      402 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_comparison_template_library.py
--rw-r--r--   0        0        0     1530 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_helpers/postgres_base.py
--rw-r--r--   0        0        0     3129 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_helpers/postgres_comparison_imports.py
--rw-r--r--   0        0        0      362 2023-07-05 16:14:53.914971 splink-3.9.3/splink/postgres/postgres_linker.py
--rw-r--r--   0        0        0     5624 2023-07-05 16:14:53.914971 splink-3.9.3/splink/predict.py
--rw-r--r--   0        0        0     8245 2023-07-05 16:14:53.914971 splink-3.9.3/splink/profile_data.py
--rw-r--r--   0        0        0    18987 2023-07-05 16:14:53.914971 splink-3.9.3/splink/settings.py
--rw-r--r--   0        0        0    17972 2023-07-05 16:14:53.914971 splink-3.9.3/splink/settings_validator.py
--rw-r--r--   0        0        0      474 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/comparison_library.py
--rw-r--r--   0        0        0      192 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/comparison_template_library.py
--rw-r--r--   0        0        0      473 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/jar_location.py
--rw-r--r--   0        0        0    23599 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/linker.py
--rw-r--r--   0        0        0      384 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_comparison_level_library.py
--rw-r--r--   0        0        0      366 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_comparison_library.py
--rw-r--r--   0        0        0      393 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_comparison_template_library.py
--rw-r--r--   0        0        0     1083 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_helpers/custom_spark_dialect.py
--rw-r--r--   0        0        0     1875 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_helpers/spark_base.py
--rw-r--r--   0        0        0     5584 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_helpers/spark_comparison_imports.py
--rw-r--r--   0        0        0      356 2023-07-05 16:14:53.914971 splink-3.9.3/splink/spark/spark_linker.py
--rw-r--r--   0        0        0     4507 2023-07-05 16:14:53.914971 splink-3.9.3/splink/splink_comparison_viewer.py
--rw-r--r--   0        0        0     4152 2023-07-05 16:14:53.914971 splink-3.9.3/splink/splink_dataframe.py
--rw-r--r--   0        0        0     1205 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sql_transform.py
--rw-r--r--   0        0        0      384 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/comparison_level_library.py
--rw-r--r--   0        0        0      252 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/comparison_library.py
--rw-r--r--   0        0        0      126 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/comparison_template_library.py
--rw-r--r--   0        0        0     8562 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/linker.py
--rw-r--r--   0        0        0      387 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_comparison_level_library.py
--rw-r--r--   0        0        0      369 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_comparison_library.py
--rw-r--r--   0        0        0      396 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_comparison_template_library.py
--rw-r--r--   0        0        0      270 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_helpers/sqlite_base.py
--rw-r--r--   0        0        0     3761 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py
--rw-r--r--   0        0        0      361 2023-07-05 16:14:53.914971 splink-3.9.3/splink/sqlite/sqlite_linker.py
--rw-r--r--   0        0        0     9772 2023-07-05 16:14:53.914971 splink-3.9.3/splink/term_frequencies.py
--rw-r--r--   0        0        0     1030 2023-07-05 16:14:53.914971 splink-3.9.3/splink/unique_id_concat.py
--rw-r--r--   0        0        0     1673 2023-07-05 16:14:53.914971 splink-3.9.3/splink/unlinkables.py
--rw-r--r--   0        0        0     2431 2023-07-05 16:14:53.914971 splink-3.9.3/splink/validate_jsonschema.py
--rw-r--r--   0        0        0     2326 2023-07-05 16:14:53.914971 splink-3.9.3/splink/vertically_concatenate.py
--rw-r--r--   0        0        0     5342 2023-07-05 16:14:53.914971 splink-3.9.3/splink/waterfall_chart.py
--rw-r--r--   0        0        0     9760 1970-01-01 00:00:00.000000 splink-3.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-19 13:19:55.452417 splink-3.9.4/LICENSE
+-rw-r--r--   0        0        0     8866 2023-07-19 13:19:55.452417 splink-3.9.4/README.md
+-rw-r--r--   0        0        0     2110 2023-07-19 13:19:55.492420 splink-3.9.4/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-07-19 13:19:55.496420 splink-3.9.4/splink/__init__.py
+-rw-r--r--   0        0        0    10852 2023-07-19 13:19:55.496420 splink-3.9.4/splink/accuracy.py
+-rw-r--r--   0        0        0     7765 2023-07-19 13:19:55.496420 splink-3.9.4/splink/analyse_blocking.py
+-rw-r--r--   0        0        0      387 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_comparison_template_library.py
+-rw-r--r--   0        0        0     1365 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_helpers/athena_base.py
+-rw-r--r--   0        0        0      165 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_helpers/athena_blocking_rule_imports.py
+-rw-r--r--   0        0        0     3322 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_helpers/athena_comparison_imports.py
+-rw-r--r--   0        0        0      350 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_helpers/athena_transforms.py
+-rw-r--r--   0        0        0     2903 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_helpers/athena_utils.py
+-rw-r--r--   0        0        0      361 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/athena_linker.py
+-rw-r--r--   0        0        0      175 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/blocking_rule_library.py
+-rw-r--r--   0        0        0      403 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/comparison_level_library.py
+-rw-r--r--   0        0        0      249 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/comparison_library.py
+-rw-r--r--   0        0        0      252 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/comparison_template_library.py
+-rw-r--r--   0        0        0    21171 2023-07-19 13:19:55.496420 splink-3.9.4/splink/athena/linker.py
+-rw-r--r--   0        0        0     2867 2023-07-19 13:19:55.496420 splink-3.9.4/splink/block_from_labels.py
+-rw-r--r--   0        0        0     9907 2023-07-19 13:19:55.496420 splink-3.9.4/splink/blocking.py
+-rw-r--r--   0        0        0    12386 2023-07-19 13:19:55.496420 splink-3.9.4/splink/blocking_rule_composition.py
+-rw-r--r--   0        0        0     2135 2023-07-19 13:19:55.496420 splink-3.9.4/splink/blocking_rules_library.py
+-rw-r--r--   0        0        0     2223 2023-07-19 13:19:55.496420 splink-3.9.4/splink/cache_dict_with_logging.py
+-rw-r--r--   0        0        0    11044 2023-07-19 13:19:55.496420 splink-3.9.4/splink/charts.py
+-rw-r--r--   0        0        0     9155 2023-07-19 13:19:55.496420 splink-3.9.4/splink/cluster_studio.py
+-rw-r--r--   0        0        0    16881 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison.py
+-rw-r--r--   0        0        0     8766 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_helpers.py
+-rw-r--r--   0        0        0      554 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_helpers_utils.py
+-rw-r--r--   0        0        0    25557 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_level.py
+-rw-r--r--   0        0        0    16609 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_level_composition.py
+-rw-r--r--   0        0        0    57707 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_level_library.py
+-rw-r--r--   0        0        0     1237 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_level_sql.py
+-rw-r--r--   0        0        0    63328 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_library.py
+-rw-r--r--   0        0        0     4922 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_library_utils.py
+-rw-r--r--   0        0        0    81390 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_template_library.py
+-rw-r--r--   0        0        0      972 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_vector_distribution.py
+-rw-r--r--   0        0        0      868 2023-07-19 13:19:55.496420 splink-3.9.4/splink/comparison_vector_values.py
+-rw-r--r--   0        0        0    16699 2023-07-19 13:19:55.496420 splink-3.9.4/splink/connected_components.py
+-rw-r--r--   0        0        0       67 2023-07-19 13:19:55.496420 splink-3.9.4/splink/constants.py
+-rw-r--r--   0        0        0     6089 2023-07-19 13:19:55.496420 splink-3.9.4/splink/convert_v2_to_v3.py
+-rw-r--r--   0        0        0     1338 2023-07-19 13:19:55.496420 splink-3.9.4/splink/databricks/enable_splink.py
+-rw-r--r--   0        0        0     5562 2023-07-19 13:19:55.496420 splink-3.9.4/splink/datasets/__init__.py
+-rw-r--r--   0        0        0      609 2023-07-19 13:19:55.496420 splink-3.9.4/splink/default_from_jsonschema.py
+-rw-r--r--   0        0        0     1608 2023-07-19 13:19:55.496420 splink-3.9.4/splink/dialect_base.py
+-rw-r--r--   0        0        0      175 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/blocking_rule_library.py
+-rw-r--r--   0        0        0      493 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/comparison_level_library.py
+-rw-r--r--   0        0        0      371 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/comparison_library.py
+-rw-r--r--   0        0        0      194 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/comparison_template_library.py
+-rw-r--r--   0        0        0      387 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_comparison_template_library.py
+-rw-r--r--   0        0        0     1555 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_base.py
+-rw-r--r--   0        0        0      165 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_blocking_rule_imports.py
+-rw-r--r--   0        0        0     5623 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py
+-rw-r--r--   0        0        0     1750 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_helpers.py
+-rw-r--r--   0        0        0      367 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/duckdb_linker.py
+-rw-r--r--   0        0        0    11906 2023-07-19 13:19:55.496420 splink-3.9.4/splink/duckdb/linker.py
+-rw-r--r--   0        0        0    17650 2023-07-19 13:19:55.496420 splink-3.9.4/splink/em_training_session.py
+-rw-r--r--   0        0        0     5743 2023-07-19 13:19:55.496420 splink-3.9.4/splink/estimate_u.py
+-rw-r--r--   0        0        0      269 2023-07-19 13:19:55.496420 splink-3.9.4/splink/exceptions.py
+-rw-r--r--   0        0        0     9070 2023-07-19 13:19:55.496420 splink-3.9.4/splink/expectation_maximisation.py
+-rw-r--r--   0        0        0     1562 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/blocking_rule_generated_comparisons.json
+-rw-r--r--   0        0        0     5153 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/comparator_score_chart.json
+-rw-r--r--   0        0        0     1836 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/comparator_score_threshold_chart.json
+-rw-r--r--   0        0        0     2775 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/completeness.json
+-rw-r--r--   0        0        0     5795 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/m_u_parameters_interactive_history.json
+-rw-r--r--   0        0        0     1111 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/match_weight_histogram.json
+-rw-r--r--   0        0        0     5691 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/match_weights_interactive_history.json
+-rw-r--r--   0        0        0     9113 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/match_weights_waterfall.json
+-rw-r--r--   0        0        0     1714 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/missingness.json
+-rw-r--r--   0        0        0     2753 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/parameter_estimate_comparisons.json
+-rw-r--r--   0        0        0     1891 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/phonetic_match_chart.json
+-rw-r--r--   0        0        0     1654 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/precision_recall.json
+-rw-r--r--   0        0        0     1125 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/probability_two_random_records_match_iteration.json
+-rw-r--r--   0        0        0     2326 2023-07-19 13:19:55.496420 splink-3.9.4/splink/files/chart_defs/profile_data.json
+-rw-r--r--   0        0        0     1805 2023-07-19 13:19:55.500420 splink-3.9.4/splink/files/chart_defs/roc.json
+-rw-r--r--   0        0        0     9910 2023-07-19 13:19:55.500420 splink-3.9.4/splink/files/chart_defs/tf_adjustment_chart.json
+-rw-r--r--   0        0        0     2910 2023-07-19 13:19:55.500420 splink-3.9.4/splink/files/chart_defs/unlinkables_chart_def.json
+-rw-r--r--   0        0        0    66064 2023-07-19 13:19:55.500420 splink-3.9.4/splink/files/external_js/vega-embed@6.20.2
+-rw-r--r--   0        0        0   256817 2023-07-19 13:19:55.500420 splink-3.9.4/splink/files/external_js/vega-lite@5.2.0
+-rw-r--r--   0        0        0   501599 2023-07-19 13:19:55.504420 splink-3.9.4/splink/files/external_js/vega@5.21.0
+-rw-r--r--   0        0        0   974616 2023-07-19 13:19:55.508421 splink-3.9.4/splink/files/labelling_tool/slt.js
+-rw-r--r--   0        0        0     2971 2023-07-19 13:19:55.508421 splink-3.9.4/splink/files/labelling_tool/template.j2
+-rw-r--r--   0        0        0    13833 2023-07-19 13:19:55.508421 splink-3.9.4/splink/files/settings_jsonschema.json
+-rw-r--r--   0        0        0  1228220 2023-07-19 13:19:55.516421 splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
+-rw-r--r--   0        0        0   944614 2023-07-19 13:19:55.524422 splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
+-rw-r--r--   0        0        0   949562 2023-07-19 13:19:55.528422 splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
+-rw-r--r--   0        0        0     5486 2023-07-19 13:19:55.528422 splink-3.9.4/splink/files/splink_cluster_studio/cluster_template.j2
+-rw-r--r--   0        0        0     2269 2023-07-19 13:19:55.528422 splink-3.9.4/splink/files/splink_cluster_studio/custom.css
+-rw-r--r--   0        0        0     2269 2023-07-19 13:19:55.528422 splink-3.9.4/splink/files/splink_comparison_viewer/custom.css
+-rw-r--r--   0        0        0     3115 2023-07-19 13:19:55.528422 splink-3.9.4/splink/files/splink_comparison_viewer/template.j2
+-rw-r--r--   0        0        0   269522 2023-07-19 13:19:55.532422 splink-3.9.4/splink/files/splink_vis_utils/splink_vis_utils.js
+-rw-r--r--   0        0        0      404 2023-07-19 13:19:55.532422 splink-3.9.4/splink/files/templates/single_chart_template.html
+-rw-r--r--   0        0        0      195 2023-07-19 13:19:55.532422 splink-3.9.4/splink/format_sql.py
+-rw-r--r--   0        0        0     7955 2023-07-19 13:19:55.532422 splink-3.9.4/splink/input_column.py
+-rw-r--r--   0        0        0     3279 2023-07-19 13:19:55.532422 splink-3.9.4/splink/labelling_tool.py
+-rw-r--r--   0        0        0   135622 2023-07-19 13:19:55.532422 splink-3.9.4/splink/linker.py
+-rw-r--r--   0        0        0      300 2023-07-19 13:19:55.532422 splink-3.9.4/splink/logging_messages.py
+-rw-r--r--   0        0        0     3132 2023-07-19 13:19:55.532422 splink-3.9.4/splink/lower_id_on_lhs.py
+-rw-r--r--   0        0        0     1834 2023-07-19 13:19:55.532422 splink-3.9.4/splink/m_from_labels.py
+-rw-r--r--   0        0        0     2465 2023-07-19 13:19:55.532422 splink-3.9.4/splink/m_training.py
+-rw-r--r--   0        0        0     2420 2023-07-19 13:19:55.532422 splink-3.9.4/splink/m_u_records_to_parameters.py
+-rw-r--r--   0        0        0      623 2023-07-19 13:19:55.532422 splink-3.9.4/splink/match_key_analysis.py
+-rw-r--r--   0        0        0     2028 2023-07-19 13:19:55.532422 splink-3.9.4/splink/match_weights_histogram.py
+-rw-r--r--   0        0        0     6135 2023-07-19 13:19:55.532422 splink-3.9.4/splink/misc.py
+-rw-r--r--   0        0        0     2791 2023-07-19 13:19:55.532422 splink-3.9.4/splink/missingness.py
+-rw-r--r--   0        0        0     1221 2023-07-19 13:19:55.532422 splink-3.9.4/splink/parse_sql.py
+-rw-r--r--   0        0        0     2909 2023-07-19 13:19:55.532422 splink-3.9.4/splink/pipeline.py
+-rw-r--r--   0        0        0      188 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/blocking_rule_library.py
+-rw-r--r--   0        0        0      407 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/comparison_level_library.py
+-rw-r--r--   0        0        0      253 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/comparison_library.py
+-rw-r--r--   0        0        0      394 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/comparison_template_library.py
+-rw-r--r--   0        0        0    11226 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/linker.py
+-rw-r--r--   0        0        0      393 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_comparison_level_library.py
+-rw-r--r--   0        0        0      375 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_comparison_library.py
+-rw-r--r--   0        0        0      402 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_comparison_template_library.py
+-rw-r--r--   0        0        0     1530 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_helpers/postgres_base.py
+-rw-r--r--   0        0        0      171 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_helpers/postgres_blocking_rule_imports.py
+-rw-r--r--   0        0        0     3129 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_helpers/postgres_comparison_imports.py
+-rw-r--r--   0        0        0      362 2023-07-19 13:19:55.532422 splink-3.9.4/splink/postgres/postgres_linker.py
+-rw-r--r--   0        0        0     5624 2023-07-19 13:19:55.532422 splink-3.9.4/splink/predict.py
+-rw-r--r--   0        0        0     8245 2023-07-19 13:19:55.532422 splink-3.9.4/splink/profile_data.py
+-rw-r--r--   0        0        0    18835 2023-07-19 13:19:55.532422 splink-3.9.4/splink/settings.py
+-rw-r--r--   0        0        0    17972 2023-07-19 13:19:55.532422 splink-3.9.4/splink/settings_validator.py
+-rw-r--r--   0        0        0      173 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/blocking_rule_library.py
+-rw-r--r--   0        0        0      491 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/comparison_library.py
+-rw-r--r--   0        0        0      192 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/comparison_template_library.py
+-rw-r--r--   0        0        0      473 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/jar_location.py
+-rw-r--r--   0        0        0    23599 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/linker.py
+-rw-r--r--   0        0        0      384 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_comparison_level_library.py
+-rw-r--r--   0        0        0      366 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_comparison_library.py
+-rw-r--r--   0        0        0      393 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_comparison_template_library.py
+-rw-r--r--   0        0        0     1083 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_helpers/custom_spark_dialect.py
+-rw-r--r--   0        0        0     1875 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_helpers/spark_base.py
+-rw-r--r--   0        0        0      162 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_helpers/spark_blocking_rule_imports.py
+-rw-r--r--   0        0        0     5584 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_helpers/spark_comparison_imports.py
+-rw-r--r--   0        0        0      356 2023-07-19 13:19:55.532422 splink-3.9.4/splink/spark/spark_linker.py
+-rw-r--r--   0        0        0     4397 2023-07-19 13:19:55.532422 splink-3.9.4/splink/splink_comparison_viewer.py
+-rw-r--r--   0        0        0     4152 2023-07-19 13:19:55.532422 splink-3.9.4/splink/splink_dataframe.py
+-rw-r--r--   0        0        0     1205 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sql_transform.py
+-rw-r--r--   0        0        0      175 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/blocking_rule_library.py
+-rw-r--r--   0        0        0      401 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/comparison_level_library.py
+-rw-r--r--   0        0        0      252 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/comparison_library.py
+-rw-r--r--   0        0        0      126 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/comparison_template_library.py
+-rw-r--r--   0        0        0     8562 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/linker.py
+-rw-r--r--   0        0        0      387 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_comparison_library.py
+-rw-r--r--   0        0        0      396 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_comparison_template_library.py
+-rw-r--r--   0        0        0      270 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_helpers/sqlite_base.py
+-rw-r--r--   0        0        0      165 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_helpers/sqlite_blocking_rule_imports.py
+-rw-r--r--   0        0        0     3761 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py
+-rw-r--r--   0        0        0      361 2023-07-19 13:19:55.532422 splink-3.9.4/splink/sqlite/sqlite_linker.py
+-rw-r--r--   0        0        0     9772 2023-07-19 13:19:55.532422 splink-3.9.4/splink/term_frequencies.py
+-rw-r--r--   0        0        0     1030 2023-07-19 13:19:55.532422 splink-3.9.4/splink/unique_id_concat.py
+-rw-r--r--   0        0        0     1673 2023-07-19 13:19:55.532422 splink-3.9.4/splink/unlinkables.py
+-rw-r--r--   0        0        0     2383 2023-07-19 13:19:55.532422 splink-3.9.4/splink/validate_jsonschema.py
+-rw-r--r--   0        0        0     2326 2023-07-19 13:19:55.532422 splink-3.9.4/splink/vertically_concatenate.py
+-rw-r--r--   0        0        0     5342 2023-07-19 13:19:55.532422 splink-3.9.4/splink/waterfall_chart.py
+-rw-r--r--   0        0        0     9849 1970-01-01 00:00:00.000000 splink-3.9.4/PKG-INFO
```

### Comparing `splink-3.9.3/LICENSE` & `splink-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/README.md` & `splink-3.9.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -77,40 +77,45 @@
 
 For more detailed tutorial, please see [here](https://moj-analytical-services.github.io/splink/demos/00_Tutorial_Introduction.html).
 
 ```py
 from splink.duckdb.linker import DuckDBLinker
 import splink.duckdb.comparison_library as cl
 import splink.duckdb.comparison_template_library as ctl
+import splink.duckdb.blocking_rule_library as brl
 from splink.datasets import splink_datasets
 
 df = splink_datasets.fake_1000
 
 settings = {
     "link_type": "dedupe_only",
     "blocking_rules_to_generate_predictions": [
-        "l.first_name = r.first_name",
-        "l.surname = r.surname",
+        brl.exact_match_rule("first_name"),
+        brl.exact_match_rule("surname"),
     ],
     "comparisons": [
         ctl.name_comparison("first_name"),
         ctl.name_comparison("surname"),
         ctl.date_comparison("dob", cast_strings_to_date=True),
         cl.exact_match("city", term_frequency_adjustments=True),
         ctl.email_comparison("email"),
     ],
 }
 
 linker = DuckDBLinker(df, settings)
 linker.estimate_u_using_random_sampling(max_pairs=1e6)
 
-blocking_rule_for_training = "l.first_name = r.first_name and l.surname = r.surname"
+blocking_rule_for_training = brl.and_(
+                                brl.exact_match_rule("first_name"), 
+                                brl.exact_match_rule("surname")
+                                )
+
 linker.estimate_parameters_using_expectation_maximisation(blocking_rule_for_training)
 
-blocking_rule_for_training = "l.dob = r.dob"
+blocking_rule_for_training = brl.exact_match_rule("dob")
 linker.estimate_parameters_using_expectation_maximisation(blocking_rule_for_training)
 
 pairwise_predictions = linker.predict()
 
 clusters = linker.cluster_pairwise_predictions_at_threshold(pairwise_predictions, 0.95)
 clusters.as_pandas_dataframe(limit=5)
 ```
@@ -118,15 +123,15 @@
 ## Videos
 
 - [A introductory presentation on Splink](https://www.youtube.com/watch?v=msz3T741KQI)
 - [An introduction to the Splink Comparison Viewer dashboard](https://www.youtube.com/watch?v=DNvCMqjipis)
 
 ## Support
 
-Please post on the [discussion forums](https://github.com/moj-analytical-services/splink/discussions) if you have any questions. If you think you have found a bug, please raise an [issue](https://github.com/moj-analytical-services/splink/issues).
+To find the best place to ask a question, report a bug or get general advice, please refer to our [Contributing Guide](./CONTRIBUTING.md).
 
 ## Awards
 
 🥇 Analysis in Government Awards 2020: Innovative Methods: [Winner](https://www.gov.uk/government/news/launch-of-the-analysis-in-government-awards)
 
 🥇 MoJ DASD Awards 2020: Innovation and Impact - Winner
```

### Comparing `splink-3.9.3/pyproject.toml` & `splink-3.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "splink"
-version = "3.9.3"
+version = "3.9.4"
 description = "Fast probabilistic data linkage at scale"
 authors = ["Robin Linacre <robinlinacre@hotmail.com>", "Sam Lindsay", "Theodore Manassis", "Tom Hepworth", "Andy Bond", "Ross Kennedy"]
 license = "MIT"
 homepage = "https://github.com/moj-analytical-services/splink"
 repository = "https://github.com/moj-analytical-services/splink"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 jsonschema = ">=3.2,<5.0"
 pandas = ">=1.0.0"
-duckdb = ">=0.6.0"
+duckdb = ">=0.8.0"
 # normalize issue in sqlglot - temporarily exclude updates
-sqlglot = ">=5.1.0,<11.4.2"
+sqlglot = ">=7.0.0,<11.4.2"
 altair = "^5.0.1"
 Jinja2 = ">=3.0.3"
 phonetics = "^1.0.5"
 
 [tool.poetry.group.dev]
 [tool.poetry.group.dev.dependencies]
 tabulate = "0.8.9"
```

### Comparing `splink-3.9.3/splink/accuracy.py` & `splink-3.9.4/splink/accuracy.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/analyse_blocking.py` & `splink-3.9.4/splink/analyse_blocking.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 
-from .blocking import _sql_gen_where_condition, block_using_rules_sql
+from .blocking import BlockingRule, _sql_gen_where_condition, block_using_rules_sql
 from .misc import calculate_cartesian, calculate_reduction_ratio
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
 
 
-def number_of_comparisons_generated_by_blocking_rule_sql(
+def number_of_comparisons_generated_by_blocking_rule_post_filters_sql(
     linker: Linker,
     blocking_rule,
 ) -> str:
     settings_obj = linker._settings_obj
 
     where_condition = _sql_gen_where_condition(
         settings_obj._link_type, settings_obj._unique_id_input_columns
@@ -135,7 +135,107 @@
             out_dict = {**out_dict, **additional_vals}
 
         br_comparisons.append(out_dict.copy())
 
     linker._analyse_blocking_mode = False
 
     return br_comparisons
+
+
+def count_comparisons_from_blocking_rule_pre_filter_conditions_sqls(
+    linker: "Linker", blocking_rule: Union[str, "BlockingRule"]
+):
+    if isinstance(blocking_rule, str):
+        blocking_rule = BlockingRule(blocking_rule, sqlglot_dialect=linker._sql_dialect)
+
+    join_conditions = blocking_rule._join_conditions
+
+    l_cols_sel = []
+    r_cols_sel = []
+    l_cols_gb = []
+    r_cols_gb = []
+    using = []
+    for (
+        i,
+        (l_key, r_key),
+    ) in enumerate(join_conditions):
+        l_cols_sel.append(f"{l_key} as key_{i}")
+        r_cols_sel.append(f"{r_key} as key_{i}")
+        l_cols_gb.append(l_key)
+        r_cols_gb.append(r_key)
+        using.append(f"key_{i}")
+
+    l_cols_sel = ", ".join(l_cols_sel)
+    r_cols_sel = ", ".join(r_cols_sel)
+    l_cols_gb = ", ".join(l_cols_gb)
+    r_cols_gb = ", ".join(r_cols_gb)
+    using = ", ".join(using)
+
+    sqls = []
+
+    if linker._two_dataset_link_only:
+        #    Can just use the raw input datasets
+        keys = list(linker._input_tables_dict.keys())
+        input_tablename_l = linker._input_tables_dict[keys[0]].physical_name
+        input_tablename_r = linker._input_tables_dict[keys[1]].physical_name
+
+    else:
+        input_tablename_l = "__splink__df_concat"
+        input_tablename_r = "__splink__df_concat"
+
+    if not join_conditions:
+        if linker._two_dataset_link_only:
+            sql = f"""
+            SELECT
+                (SELECT COUNT(*) FROM {input_tablename_l})
+                *
+                (SELECT COUNT(*) FROM {input_tablename_r})
+                    AS count_of_pairwise_comparisons_generated
+            """
+        else:
+            sql = """
+            select count(*) * count(*) as count_of_pairwise_comparisons_generated
+            from __splink__df_concat
+
+            """
+        sqls.append(
+            {"sql": sql, "output_table_name": "__splink__total_of_block_counts"}
+        )
+        return sqls
+
+    sql = f"""
+    select {l_cols_sel}, count(*) as count_l
+    from {input_tablename_l}
+    group by {l_cols_gb}
+    """
+
+    sqls.append(
+        {"sql": sql, "output_table_name": "__splink__count_comparisons_from_blocking_l"}
+    )
+
+    sql = f"""
+    select {r_cols_sel}, count(*) as count_r
+    from {input_tablename_r}
+    group by {r_cols_gb}
+    """
+
+    sqls.append(
+        {"sql": sql, "output_table_name": "__splink__count_comparisons_from_blocking_r"}
+    )
+
+    sql = f"""
+    select *, count_l, count_r, count_l * count_r as block_count
+    from __splink__count_comparisons_from_blocking_l
+    inner join __splink__count_comparisons_from_blocking_r
+    using ({using})
+    """
+
+    sqls.append({"sql": sql, "output_table_name": "__splink__block_counts"})
+
+    sql = """
+    select sum(block_count) as count_of_pairwise_comparisons_generated
+    from __splink__block_counts
+    """
+
+    sqls.append({"sql": sql, "output_table_name": "__splink__total_of_block_counts"})
+
+    return sqls
```

### Comparing `splink-3.9.3/splink/athena/athena_helpers/athena_base.py` & `splink-3.9.4/splink/athena/athena_helpers/athena_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/athena/athena_helpers/athena_comparison_imports.py` & `splink-3.9.4/splink/athena/athena_helpers/athena_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/athena/athena_helpers/athena_utils.py` & `splink-3.9.4/splink/athena/athena_helpers/athena_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/athena/linker.py` & `splink-3.9.4/splink/athena/linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/block_from_labels.py` & `splink-3.9.4/splink/block_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/cache_dict_with_logging.py` & `splink-3.9.4/splink/cache_dict_with_logging.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/charts.py` & `splink-3.9.4/splink/charts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,33 @@
 import json
 import os
-import pkgutil
 
+from .misc import read_resource
 from .waterfall_chart import records_to_waterfall_data
 
 altair_installed = True
 
 try:
     import altair as alt
 except ImportError:
     altair_installed = False
 
 
 def load_chart_definition(filename):
     path = f"files/chart_defs/{filename}"
-    data = pkgutil.get_data(__name__, path)
-    schema = json.loads(data)
-    return schema
+    return json.loads(read_resource(path))
 
 
 def _load_external_libs():
     to_load = {
         "vega-embed": "files/external_js/vega-embed@6.20.2",
         "vega-lite": "files/external_js/vega-lite@5.2.0",
         "vega": "files/external_js/vega@5.21.0",
     }
-
-    loaded = {}
-    for k, v in to_load.items():
-        script = pkgutil.get_data(__name__, v).decode("utf-8")
-        loaded[k] = script
-
-    return loaded
+    return {k: read_resource(v) for k, v in to_load.items()}
 
 
 def altair_or_json(chart_dict, as_dict=False):
     if altair_installed:
         if not as_dict:
             try:
                 return alt.Chart.from_dict(chart_dict)
@@ -73,17 +65,15 @@
         raise ValueError(
             f"The path {filename} already exists. Please provide a different path."
         )
 
     if type(chart_dict).__name__ == "VegaliteNoValidate":
         chart_dict = chart_dict.spec
 
-    # get altair chart as json
-    path = "files/templates/single_chart_template.txt"
-    template = pkgutil.get_data(__name__, path).decode("utf-8")
+    template = read_resource("files/templates/single_chart_template.html")
 
     fmt_dict = _load_external_libs()
 
     fmt_dict["mychart"] = json.dumps(chart_dict)
 
     with open(filename, "w", encoding="utf-8") as f:
         f.write(template.format(**fmt_dict))
```

### Comparing `splink-3.9.3/splink/cluster_studio.py` & `splink-3.9.4/splink/cluster_studio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 import json
 import os
-import pkgutil
 import random
 from typing import TYPE_CHECKING
 
 from jinja2 import Template
 
-from .misc import EverythingEncoder
+from .misc import EverythingEncoder, read_resource
 from .splink_dataframe import SplinkDataFrame
 from .unique_id_concat import (
     _composite_unique_id_from_edges_sql,
     _composite_unique_id_from_nodes_sql,
 )
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
@@ -227,16 +226,15 @@
     cluster_recs = df_clusters_as_records(linker, df_clustered_nodes, cluster_ids)
     df_nodes = create_df_nodes(linker, df_clustered_nodes, cluster_ids)
     nodes_recs = df_nodes.as_record_dict()
     edges_recs = df_edges_as_records(linker, df_predicted_edges, df_nodes)
 
     # Render template with cluster, nodes and edges
     template_path = "files/splink_cluster_studio/cluster_template.j2"
-    template = pkgutil.get_data(__name__, template_path).decode("utf-8")
-    template = Template(template)
+    template = Template(read_resource(template_path))
 
     template_data = {
         "raw_edge_data": json.dumps(edges_recs, cls=EverythingEncoder),
         "raw_node_data": json.dumps(nodes_recs, cls=EverythingEncoder),
         "raw_clusters_data": json.dumps(cluster_recs, cls=EverythingEncoder),
         "splink_settings": json.dumps(
             linker._settings_obj._as_completed_dict(), cls=EverythingEncoder
@@ -255,19 +253,16 @@
     files = {
         "embed": "files/external_js/vega-embed@6.20.2",
         "vega": "files/external_js/vega@5.21.0",
         "vegalite": "files/external_js/vega-lite@5.2.0",
         "svu_text": "files/splink_vis_utils/splink_vis_utils.js",
         "custom_css": "files/splink_cluster_studio/custom.css",
     }
-
     for k, v in files.items():
-        f = pkgutil.get_data(__name__, v)
-        f = f.decode("utf-8")
-        template_data[k] = f
+        template_data[k] = read_resource(v)
 
     template_data["bundle_observable_notebook"] = bundle_observable_notebook
 
     rendered = template.render(**template_data)
 
     if os.path.isfile(out_path) and not overwrite:
         raise ValueError(
```

### Comparing `splink-3.9.3/splink/comparison.py` & `splink-3.9.4/splink/comparison.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/comparison_helpers.py` & `splink-3.9.4/splink/comparison_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/comparison_helpers_utils.py` & `splink-3.9.4/splink/comparison_helpers_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/comparison_level.py` & `splink-3.9.4/splink/comparison_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,18 @@
         # Enable the level to 'know' when it's been trained
         self._trained_m_probabilities: list = []
         self._trained_u_probabilities: list = []
 
         self._validate()
 
     @property
+    def sql_dialect(self):
+        return self._sql_dialect
+
+    @property
     def is_null_level(self) -> bool:
         return self._is_null_level
 
     @property
     def sql_condition(self) -> str:
         return self._sql_condition
 
@@ -182,15 +186,15 @@
             val = default_value_from_schema(key, "comparison_level")
         return val
 
     @property
     def _tf_adjustment_input_column(self):
         val = self._level_dict_val_else_default("tf_adjustment_column")
         if val:
-            return InputColumn(val, sql_dialect=self._sql_dialect)
+            return InputColumn(val, sql_dialect=self.sql_dialect)
         else:
             return None
 
     @property
     def _tf_adjustment_input_column_name(self):
         input_column = self._tf_adjustment_input_column
         if input_column:
@@ -406,16 +410,16 @@
         col = self._level_dict.get("tf_adjustment_column")
         return col is not None
 
     def _validate_sql(self):
         sql = self.sql_condition
         if self._is_else_level:
             return True
-        dialect = self._sql_dialect
-        # TODO: really self._sql_dialect should always be set, something gets
+        dialect = self.sql_dialect
+        # TODO: really self._sql_dialect_ should always be set, something gets
         # messed up during the deepcopy()ing of a Comparison
         if dialect is None:
             dialect = "spark"
         try:
             sqlglot.parse_one(sql, read=dialect)
         except sqlglot.ParseError as e:
             raise ValueError(f"Error parsing sql_statement:\n{sql}") from e
@@ -425,28 +429,28 @@
     @property
     def _input_columns_used_by_sql_condition(self) -> list[InputColumn]:
         # returns e.g. InputColumn(first_name), InputColumn(surname)
 
         if self._is_else_level:
             return []
 
-        cols = get_columns_used_from_sql(self.sql_condition, dialect=self._sql_dialect)
+        cols = get_columns_used_from_sql(self.sql_condition, dialect=self.sql_dialect)
         # Parsed order seems to be roughly in reverse order of apearance
         cols = cols[::-1]
 
         cols = [re.sub(r"_L$|_R$", "", c, flags=re.IGNORECASE) for c in cols]
         cols = dedupe_preserving_order(cols)
 
         input_cols = []
         for c in cols:
             # We could have tf adjustments for surname on a dmeta_surname column
             # If so, we want to set the tf adjustments against the surname col,
             # not the dmeta_surname one
 
-            input_cols.append(InputColumn(c, sql_dialect=self._sql_dialect))
+            input_cols.append(InputColumn(c, sql_dialect=self.sql_dialect))
 
         return input_cols
 
     @property
     def _columns_to_select_for_blocking(self):
         # e.g. l.first_name as first_name_l, r.first_name as first_name_r
         output_cols = []
@@ -478,28 +482,28 @@
 
     @property
     def _is_exact_match(self):
         if self._is_else_level:
             return False
 
         sql_syntax_tree = sqlglot.parse_one(
-            self.sql_condition.lower(), read=self._sql_dialect
+            self.sql_condition.lower(), read=self.sql_dialect
         )
         sql_cnf = normalize(sql_syntax_tree)
 
         exprs = _get_and_subclauses(sql_cnf)
         for expr in exprs:
             if not _is_exact_match(expr):
                 return False
         return True
 
     @property
     def _exact_match_colnames(self):
         sql_syntax_tree = sqlglot.parse_one(
-            self.sql_condition.lower(), read=self._sql_dialect
+            self.sql_condition.lower(), read=self.sql_dialect
         )
         sql_cnf = normalize(sql_syntax_tree)
 
         exprs = _get_and_subclauses(sql_cnf)
         for expr in exprs:
             if not _is_exact_match(expr):
                 raise ValueError(
@@ -701,15 +705,15 @@
         return output_records
 
     def _validate(self):
         self._validate_sql()
 
     def _abbreviated_sql(self, cutoff=75):
         sql = self.sql_condition
-        return (sql[:75] + "...") if len(sql) > 75 else sql
+        return (sql[:cutoff] + "...") if len(sql) > cutoff else sql
 
     def __repr__(self):
         return f"<{self._human_readable_succinct}>"
 
     @property
     def _human_readable_succinct(self):
         sql = self._abbreviated_sql(75)
```

### Comparing `splink-3.9.3/splink/comparison_level_composition.py` & `splink-3.9.4/splink/comparison_level_composition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import Iterable
 
+from .blocking import BlockingRule
 from .comparison_level import ComparisonLevel
 
 
 def and_(
     *clls: ComparisonLevel | dict,
     label_for_charts=None,
     m_probability=None,
@@ -413,15 +414,15 @@
 def _to_comparison_level(cl: ComparisonLevel | dict) -> ComparisonLevel:
     if isinstance(cl, ComparisonLevel):
         return cl
     else:
         return ComparisonLevel(cl)
 
 
-def _unify_sql_dialects(cls: Iterable[ComparisonLevel]) -> str | None:
-    sql_dialects = set(cl._sql_dialect for cl in cls)
+def _unify_sql_dialects(cls: Iterable[ComparisonLevel | BlockingRule]) -> str | None:
+    sql_dialects = set(cl.sql_dialect for cl in cls)
     sql_dialects.discard(None)
     if len(sql_dialects) > 1:
         raise ValueError("Cannot combine comparison levels with different SQL dialects")
     elif len(sql_dialects) == 0:
         return None
     return sql_dialects.pop()
```

### Comparing `splink-3.9.3/splink/comparison_level_library.py` & `splink-3.9.4/splink/comparison_level_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,34 +228,34 @@
         """Represents a comparison level for all cases which have not been
         considered by preceding comparison levels,
 
         Examples:
             === ":simple-duckdb: DuckDB"
                 ``` python
                 import splink.duckdb.comparison_level_library as cll
-                cll.else_level("name")
+                cll.else_level()
                 ```
             === ":simple-apachespark: Spark"
                 ``` python
                 import splink.spark.comparison_level_library as cll
-                cll.else_level("name")
+                cll.else_level()
                 ```
             === ":simple-amazonaws: Athena"
                 ``` python
                 import splink.athena.comparison_level_library as cll
-                cll.else_level("name")
+                cll.else_level()
                 ```
             === ":simple-sqlite: SQLite"
                 ``` python
                 import splink.sqlite.comparison_level_library as cll
-                cll.else_level("name")
+                cll.else_level()
             === ":simple-postgresql: PostgreSql"
                 ``` python
                 import splink.postgres.comparison_level_library as cll
-                cll.else_level("name")
+                cll.else_level()
                 ```
         """
         if isinstance(m_probability, str):
             raise ValueError(
                 "You provided a string for the value of m probability when it should "
                 "be numeric.  Perhaps you passed a column name.  Note that you do "
                 "not need to pass a column name into the else level."
```

### Comparing `splink-3.9.3/splink/comparison_level_sql.py` & `splink-3.9.4/splink/comparison_level_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/comparison_library.py` & `splink-3.9.4/splink/comparison_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/comparison_library_utils.py` & `splink-3.9.4/splink/comparison_library_utils.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/comparison_template_library.py` & `splink-3.9.4/splink/comparison_template_library.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/comparison_vector_distribution.py` & `splink-3.9.4/splink/comparison_vector_distribution.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/comparison_vector_values.py` & `splink-3.9.4/splink/comparison_vector_values.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/connected_components.py` & `splink-3.9.4/splink/connected_components.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/convert_v2_to_v3.py` & `splink-3.9.4/splink/convert_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/databricks/enable_splink.py` & `splink-3.9.4/splink/databricks/enable_splink.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/datasets/__init__.py` & `splink-3.9.4/splink/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/default_from_jsonschema.py` & `splink-3.9.4/splink/default_from_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/dialect_base.py` & `splink-3.9.4/splink/dialect_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_base.py` & `splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py` & `splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/duckdb/duckdb_helpers/duckdb_helpers.py` & `splink-3.9.4/splink/duckdb/duckdb_helpers/duckdb_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/duckdb/linker.py` & `splink-3.9.4/splink/duckdb/linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/em_training_session.py` & `splink-3.9.4/splink/em_training_session.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/estimate_u.py` & `splink-3.9.4/splink/estimate_u.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/expectation_maximisation.py` & `splink-3.9.4/splink/expectation_maximisation.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/blocking_rule_generated_comparisons.json` & `splink-3.9.4/splink/files/chart_defs/blocking_rule_generated_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/comparator_score_chart.json` & `splink-3.9.4/splink/files/chart_defs/comparator_score_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/comparator_score_threshold_chart.json` & `splink-3.9.4/splink/files/chart_defs/comparator_score_threshold_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/completeness.json` & `splink-3.9.4/splink/files/chart_defs/completeness.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/m_u_parameters_interactive_history.json` & `splink-3.9.4/splink/files/chart_defs/m_u_parameters_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/match_weight_histogram.json` & `splink-3.9.4/splink/files/chart_defs/match_weight_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/match_weights_interactive_history.json` & `splink-3.9.4/splink/files/chart_defs/match_weights_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/match_weights_waterfall.json` & `splink-3.9.4/splink/files/chart_defs/match_weights_waterfall.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/missingness.json` & `splink-3.9.4/splink/files/chart_defs/missingness.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/parameter_estimate_comparisons.json` & `splink-3.9.4/splink/files/chart_defs/parameter_estimate_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/phonetic_match_chart.json` & `splink-3.9.4/splink/files/chart_defs/phonetic_match_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/precision_recall.json` & `splink-3.9.4/splink/files/chart_defs/precision_recall.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/probability_two_random_records_match_iteration.json` & `splink-3.9.4/splink/files/chart_defs/probability_two_random_records_match_iteration.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/profile_data.json` & `splink-3.9.4/splink/files/chart_defs/profile_data.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/roc.json` & `splink-3.9.4/splink/files/chart_defs/roc.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/tf_adjustment_chart.json` & `splink-3.9.4/splink/files/chart_defs/tf_adjustment_chart.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/chart_defs/unlinkables_chart_def.json` & `splink-3.9.4/splink/files/chart_defs/unlinkables_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/external_js/vega-embed@6.20.2` & `splink-3.9.4/splink/files/external_js/vega-embed@6.20.2`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/external_js/vega-lite@5.2.0` & `splink-3.9.4/splink/files/external_js/vega-lite@5.2.0`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/external_js/vega@5.21.0` & `splink-3.9.4/splink/files/external_js/vega@5.21.0`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/labelling_tool/slt.js` & `splink-3.9.4/splink/files/labelling_tool/slt.js`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/labelling_tool/template.j2` & `splink-3.9.4/splink/files/labelling_tool/template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/settings_jsonschema.json` & `splink-3.9.4/splink/files/settings_jsonschema.json`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar` & `splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar` & `splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar` & `splink-3.9.4/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/splink_cluster_studio/cluster_template.j2` & `splink-3.9.4/splink/files/splink_cluster_studio/cluster_template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/splink_cluster_studio/custom.css` & `splink-3.9.4/splink/files/splink_cluster_studio/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/splink_comparison_viewer/custom.css` & `splink-3.9.4/splink/files/splink_comparison_viewer/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/splink_comparison_viewer/template.j2` & `splink-3.9.4/splink/files/splink_comparison_viewer/template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/files/splink_vis_utils/splink_vis_utils.js` & `splink-3.9.4/splink/files/splink_vis_utils/splink_vis_utils.js`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/input_column.py` & `splink-3.9.4/splink/input_column.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/labelling_tool.py` & `splink-3.9.4/splink/labelling_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import json
 import logging
 import os
-import pkgutil
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 from jinja2 import Template
 
-from .misc import EverythingEncoder
+from .misc import EverythingEncoder, read_resource
 from .splink_dataframe import SplinkDataFrame
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
 
 logger = logging.getLogger(__name__)
 
 
 def generate_labelling_tool_comparisons(
     linker: "Linker", unique_id, source_dataset, match_weight_threshold=-4
 ):
-
     # ensure the tf table exists
     concat_with_tf = linker._initialise_df_concat_with_tf()
 
     settings = linker._settings_obj
 
     source_dataset_condition = ""
 
@@ -56,15 +54,14 @@
     linker: "Linker",
     df_comparisons: SplinkDataFrame,
     out_path="labelling_tool.html",
     view_in_jupyter=False,
     show_splink_predictions_in_interface=True,
     overwrite: bool = True,
 ):
-
     settings: dict = linker._settings_obj.as_dict()
 
     logger.warning(
         "\nWARNING:\n"
         "The Splink labelling tool is still in development, which means some "
         "features may change and there may be bugs.\nYour feedback will help us "
         "improve it. Go to\n"
@@ -79,33 +76,28 @@
     comparisons_recs = comparisons_recs.fillna(np.nan).replace(
         [np.nan, pd.NA], ["", ""]
     )
 
     comparisons_recs = comparisons_recs.to_dict(orient="records")
     # Render template with cluster, nodes and edges
     template_path = "files/labelling_tool/template.j2"
-    template = pkgutil.get_data(__name__, template_path).decode("utf-8")
-    template = Template(template)
-
-    slt_text = pkgutil.get_data(__name__, "files/labelling_tool/slt.js")
-    slt_text = slt_text.decode("utf-8")
+    template = Template(read_resource(template_path))
 
     template_data = {
-        "slt": slt_text,
+        "slt": read_resource("files/labelling_tool/slt.js"),
         "pairwise_comparison_data": json.dumps(comparisons_recs, cls=EverythingEncoder),
         "splink_settings_data": json.dumps(settings, cls=EverythingEncoder),
         "view_in_jupyter": view_in_jupyter,
         "show_splink_predictions_in_interface": show_splink_predictions_in_interface,
     }
 
     rendered = template.render(**template_data)
 
     if os.path.isfile(out_path) and not overwrite:
         raise ValueError(
             f"The path {out_path} already exists. Please provide a different path."
         )
     else:
-
         with open(out_path, "w", encoding="utf-8") as html_file:
             html_file.write(rendered)
         # return the rendered dashboard html for inline viewing in the notebook
         return rendered
```

### Comparing `splink-3.9.3/splink/linker.py` & `splink-3.9.4/splink/linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,23 @@
 from .accuracy import (
     prediction_errors_from_label_column,
     prediction_errors_from_labels_table,
     truth_space_table_from_labels_column,
     truth_space_table_from_labels_table,
 )
 from .analyse_blocking import (
+    count_comparisons_from_blocking_rule_pre_filter_conditions_sqls,
     cumulative_comparisons_generated_by_blocking_rules,
-    number_of_comparisons_generated_by_blocking_rule_sql,
+    number_of_comparisons_generated_by_blocking_rule_post_filters_sql,
+)
+from .blocking import (
+    BlockingRule,
+    block_using_rules_sql,
+    blocking_rule_to_obj,
 )
-from .blocking import BlockingRule, block_using_rules_sql
 from .cache_dict_with_logging import CacheDictWithLogging
 from .charts import (
     completeness_chart,
     cumulative_blocking_rule_comparisons_generated,
     match_weights_histogram,
     missingness_chart,
     parameter_estimate_comparisons,
@@ -1060,19 +1065,14 @@
                 the path to your settings json file.
             validate_settings (bool, optional): When True, check your settings
                 dictionary for any potential errors that may cause splink to fail.
         """
 
         if not isinstance(settings_dict, dict):
             p = Path(settings_dict)
-            if not p.is_file():  # check if it's a valid file/filepath
-                raise FileNotFoundError(
-                    "The filepath you have provided is either not a valid file "
-                    "or doesn't exist along the path provided."
-                )
             settings_dict = json.loads(p.read_text())
 
         # Store the cache ID so it can be reloaded after cache invalidation
         cache_id = self._cache_uid
         # So we don't run into any issues with generated tables having
         # invalid columns as settings have been tweaked, invalidate
         # the cache and allow these tables to be recomputed.
@@ -1530,16 +1530,16 @@
                 br_training,
                 comparisons_to_deactivate=["first_name"],
                 comparison_levels_to_reverse_blocking_rule=[dmeta_level],
             )
             ```
 
         Args:
-            blocking_rule (str): The blocking rule used to generate pairwise record
-                comparisons.
+            blocking_rule (BlockingRule | str): The blocking rule used to generate
+                pairwise record comparisons.
             comparisons_to_deactivate (list, optional): By default, splink will
                 analyse the blocking rule provided and estimate the m parameters for
                 all comaprisons except those included in the blocking rule.  If
                 comparisons_to_deactivate are provided, spink will instead
                 estimate m parameters for all comparison except those specified
                 in the comparisons_to_deactivate list.  This list can either contain
                 the output_column_name of the Comparison as a string, or Comparison
@@ -1566,24 +1566,36 @@
                 the blocked value. Defaults to False.
 
         Examples:
             ```py
             blocking_rule = "l.first_name = r.first_name and l.dob = r.dob"
             linker.estimate_parameters_using_expectation_maximisation(blocking_rule)
             ```
+            or using pre-built rules
+            ```py
+            import splink.duckdb.blocking_rule_library as brl
+            blocking_rule = brl.and_(
+                brl.exact_match_rule("first_name"),
+                brl.exact_match_rule("surname"),
+            )
+            linker.estimate_parameters_using_expectation_maximisation(blocking_rule)
+            ```
 
         Returns:
             EMTrainingSession:  An object containing information about the training
                 session such as how parameters changed during the iteration history
 
         """
         # Ensure this has been run on the main linker so that it's in the cache
         # to be used by the training linkers
         self._initialise_df_concat_with_tf()
 
+        # Extract the blocking rule
+        blocking_rule = blocking_rule_to_obj(blocking_rule).blocking_rule
+
         if comparisons_to_deactivate:
             # If user provided a string, convert to Comparison object
             comparisons_to_deactivate = [
                 self._settings_obj._get_comparison_by_output_column_name(n)
                 if isinstance(n, str)
                 else n
                 for n in comparisons_to_deactivate
@@ -1747,14 +1759,16 @@
         """
 
         original_blocking_rules = (
             self._settings_obj._blocking_rules_to_generate_predictions
         )
         original_link_type = self._settings_obj._link_type
 
+        blocking_rules = ensure_is_list(blocking_rules)
+
         if not isinstance(records_or_tablename, str):
             uid = ascii_uid(8)
             new_records_tablename = f"__splink__df_new_records_{uid}"
             self.register_table(
                 records_or_tablename, new_records_tablename, overwrite=True
             )
 
@@ -1778,20 +1792,17 @@
         else:
             # This queues up our cols_with_tf and df_concat_with_tf tables.
             concat_with_tf = self._initialise_df_concat_with_tf(materialise=False)
 
         if concat_with_tf:
             input_dfs.append(concat_with_tf)
 
-        rules = []
-        for r in blocking_rules:
-            br_as_obj = BlockingRule(r) if not isinstance(r, BlockingRule) else r
-            br_as_obj.preceding_rules = rules.copy()
-            rules.append(br_as_obj)
-        blocking_rules = rules
+        blocking_rules = [blocking_rule_to_obj(br) for br in blocking_rules]
+        for n, br in enumerate(blocking_rules):
+            br.add_preceding_rules(blocking_rules[:n])
 
         self._settings_obj._blocking_rules_to_generate_predictions = blocking_rules
 
         self._find_new_matches_mode = True
 
         sql = _join_tf_to_input_df_sql(self)
         sql = sql.replace("__splink__df_concat", new_records_tablename)
@@ -2677,80 +2688,129 @@
             ```
         """
         records = completeness_data(self, input_dataset, cols)
         return completeness_chart(records)
 
     def count_num_comparisons_from_blocking_rule(
         self,
-        blocking_rule: str,
+        blocking_rule: str | BlockingRule,
     ) -> int:
         """Compute the number of pairwise record comparisons that would be generated by
         a blocking rule
 
         Args:
-            blocking_rule (str): The blocking rule to analyse
+            blocking_rule (str | BlockingRule): The blocking rule to analyse
             link_type (str, optional): The link type.  This is needed only if the
                 linker has not yet been provided with a settings dictionary.  Defaults
                 to None.
             unique_id_column_name (str, optional):  This is needed only if the
                 linker has not yet been provided with a settings dictionary.  Defaults
                 to None.
 
         Examples:
             ```py
-            br = "l.first_name = r.first_name"
+            br = "l.surname = r.surname"
             linker.count_num_comparisons_from_blocking_rule(br)
             ```
             > 19387
+
             ```py
             br = "l.name = r.name and substr(l.dob,1,4) = substr(r.dob,1,4)"
             linker.count_num_comparisons_from_blocking_rule(br)
             ```
             > 394
+            Alternatively, you can use the blocking rule library functions
+            ```py
+            import splink.duckdb.blocking_rule_library as brl
+            br = brl.exact_match_rule("surname")
+            linker.count_num_comparisons_from_blocking_rule(br)
+            ```
+            > 3167
 
         Returns:
             int: The number of comparisons generated by the blocking rule
         """
 
+        blocking_rule = blocking_rule_to_obj(blocking_rule).blocking_rule
+
         sql = vertically_concatenate_sql(self)
         self._enqueue_sql(sql, "__splink__df_concat")
 
-        sql = number_of_comparisons_generated_by_blocking_rule_sql(self, blocking_rule)
+        sql = number_of_comparisons_generated_by_blocking_rule_post_filters_sql(
+            self, blocking_rule
+        )
         self._enqueue_sql(sql, "__splink__analyse_blocking_rule")
         res = self._execute_sql_pipeline().as_record_dict()[0]
         return res["count_of_pairwise_comparisons_generated"]
 
+    def _count_num_comparisons_from_blocking_rule_pre_filter_conditions(
+        self,
+        blocking_rule: str,
+    ) -> int:
+        """Compute the number of pairwise record comparisons that would be generated by
+        a blocking rule, prior to any filters (non equi-join conditions) being applied
+        by the SQL engine.
+
+        For more information on what this means, see
+        https://github.com/moj-analytical-services/splink/discussions/1391
+
+        Args:
+            blocking_rule (str): The blocking rule to analyse
+
+        Returns:
+            int: The number of comparisons generated by the blocking rule
+        """
+
+        input_dataframes = []
+        df_concat = self._initialise_df_concat()
+
+        if df_concat:
+            input_dataframes.append(df_concat)
+
+        sqls = count_comparisons_from_blocking_rule_pre_filter_conditions_sqls(
+            self, blocking_rule
+        )
+        for sql in sqls:
+            self._enqueue_sql(sql["sql"], sql["output_table_name"])
+
+        res = self._execute_sql_pipeline(input_dataframes).as_record_dict()[0]
+        return int(res["count_of_pairwise_comparisons_generated"])
+
     def cumulative_comparisons_from_blocking_rules_records(
         self,
-        blocking_rules: str or list = None,
+        blocking_rules: str | BlockingRule | list = None,
     ):
         """Output the number of comparisons generated by each successive blocking rule.
 
         This is equivalent to the output size of df_predict and details how many
         comparisons each of your individual blocking rules will contribute to the
         total.
 
         Args:
             blocking_rules (str or list): The blocking rule(s) to compute comparisons
                 for. If null, the rules set out in your settings object will be used.
 
         Examples:
+            Generate total comparisons from Blocking Rules defined in settings
+            dictionary
             ```py
             linker_settings = DuckDBLinker(df, settings)
             # Compute the cumulative number of comparisons generated by the rules
             # in your settings object.
             linker_settings.cumulative_comparisons_from_blocking_rules_records()
-            >>>
-            # Generate total comparisons with custom blocking rules.
+            ```
+
+            Generate total comparisons with custom blocking rules.
+            ```py
             blocking_rules = [
                "l.surname = r.surname",
                "l.first_name = r.first_name
                 and substr(l.dob,1,4) = substr(r.dob,1,4)"
             ]
-            >>>
+
             linker_settings.cumulative_comparisons_from_blocking_rules_records(
                 blocking_rules
              )
             ```
 
         Returns:
             List: A list of blocking rules and the corresponding number of
@@ -2763,15 +2823,15 @@
             self, blocking_rules, output_chart=False
         )
 
         return records
 
     def cumulative_num_comparisons_from_blocking_rules_chart(
         self,
-        blocking_rules: str or list = None,
+        blocking_rules: str | BlockingRule | list = None,
     ):
         """Display a chart with the cumulative number of comparisons generated by a
         selection of blocking rules.
 
         This is equivalent to the output size of df_predict and details how many
         comparisons each of your individual blocking rules will contribute to the
         total.
@@ -2809,30 +2869,30 @@
         records = cumulative_comparisons_generated_by_blocking_rules(
             self, blocking_rules, output_chart=True
         )
 
         return cumulative_blocking_rule_comparisons_generated(records)
 
     def count_num_comparisons_from_blocking_rules_for_prediction(self, df_predict):
-        """Counts the maginal number of edges created from each of the blocking rules
+        """Counts the marginal number of edges created from each of the blocking rules
         in `blocking_rules_to_generate_predictions`
 
         This is different to `count_num_comparisons_from_blocking_rule`
         because it (a) analyses multiple blocking rules rather than a single rule, and
         (b) deduplicates any comparisons that are generated, to tell you the
         marginal effect of each entry in `blocking_rules_to_generate_predictions`
 
         Args:
             df_predict (SplinkDataFrame): SplinkDataFrame with match weights
             and probabilities of rows matching
 
         Examples:
             ```py
-            linker = DuckDBLinker(df, connection=":memory:")
-            linker.load_settings("saved_settings.json")
+            linker = DuckDBLinker(df)
+            linker.load_model("settings.json")
             df_predict = linker.predict(threshold_match_probability=0.95)
             count_pairwise = linker.count_num_comparisons_from_blocking_rules_for_prediction(df_predict)
             count_pairwise.as_pandas_dataframe(limit=5)
             ```
 
         Returns:
             SplinkDataFrame: A SplinkDataFrame of the pairwise comparisons and
```

### Comparing `splink-3.9.3/splink/lower_id_on_lhs.py` & `splink-3.9.4/splink/lower_id_on_lhs.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/m_from_labels.py` & `splink-3.9.4/splink/m_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/m_training.py` & `splink-3.9.4/splink/m_training.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/m_u_records_to_parameters.py` & `splink-3.9.4/splink/m_u_records_to_parameters.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/match_key_analysis.py` & `splink-3.9.4/splink/match_key_analysis.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/match_weights_histogram.py` & `splink-3.9.4/splink/match_weights_histogram.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/misc.py` & `splink-3.9.4/splink/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
+import pkgutil
 import random
 import string
 from collections import namedtuple
 from datetime import datetime, timedelta
 from math import ceil, inf, log2
 from typing import Iterable
 
 import numpy as np
-import pkg_resources
 
 
 def dedupe_preserving_order(list_of_items):
     return list(dict.fromkeys(list_of_items))
 
 
 def prob_to_bayes_factor(prob):
@@ -141,24 +141,14 @@
     in the comparison space as a result of using your given blocking
     rule. This is a measure of how much the Blocking Rule reduces
     the total search space.
     """
     return 1 - (N / cartesian)
 
 
-def _check_dependency_installed(module):
-    try:
-        pkg_resources.get_distribution(module)
-    except pkg_resources.DistributionNotFound as e:
-        raise ValueError(
-            f"{module} is not installed.",
-            "Please install and import it before continuing.",
-        ) from e
-
-
 def major_minor_version_greater_equal_than(this_version, base_comparison_version):
     this_version = this_version.split(".")[:2]
     this_version = [v.zfill(10) for v in this_version]
 
     base_version = base_comparison_version.split(".")[:2]
     base_version = [v.zfill(10) for v in base_version]
 
@@ -209,7 +199,18 @@
     GREEN = "\033[92m"
     YELLOW = "\033[93m"
     RED = "\033[91m"
     BOLD = "\033[1m"
     UNDERLINE = "\033[4m"
     ITALICS = "\033[3m"
     END = "\033[0m"
+
+
+def read_resource(path: str) -> str:
+    """Reads a resource file from the splink package"""
+    # In the future we may have to move to importlib.resources
+    # https://github.com/python/cpython/issues/89838#issuecomment-1093935933
+    # But for now this API avoids having to do conditional imports
+    # depending on python version.
+    # Also, if you use importlib.resources, then you have to add an
+    # __init__.py file to every subdirectory, which is annoying.
+    return pkgutil.get_data("splink", path).decode("utf-8")
```

### Comparing `splink-3.9.3/splink/missingness.py` & `splink-3.9.4/splink/missingness.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/parse_sql.py` & `splink-3.9.4/splink/parse_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/pipeline.py` & `splink-3.9.4/splink/pipeline.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/postgres/linker.py` & `splink-3.9.4/splink/postgres/linker.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         input_table_or_tables,
         settings_dict=None,
         engine: Engine = None,
         set_up_basic_logging=True,
         input_table_aliases: str | list = None,
         validate_settings: bool = True,
         schema="splink",
+        other_schemas_to_search: str | list = [],
     ):
         self._sql_dialect_ = "postgres"
         if not isinstance(engine, Engine):
             raise ValueError(
                 "You must supply a sqlalchemy engine " "to create a PostgresLinker."
             )
 
@@ -96,22 +97,21 @@
 
         input_tables = ensure_is_list(input_table_or_tables)
         input_aliases = self._ensure_aliases_populated_and_is_list(
             input_table_or_tables, input_table_aliases
         )
         accepted_df_dtypes = pd.DataFrame
         self._db_schema = schema
+        # Create splink schema
+        self._create_splink_schema(other_schemas_to_search)
 
         # Create custom SQL functions in database
         self._register_custom_functions()
         self._register_extensions()
 
-        # Create splink schema
-        self._create_splink_schema()
-
         super().__init__(
             input_tables,
             settings_dict,
             accepted_df_dtypes,
             set_up_basic_logging,
             input_table_aliases=input_aliases,
             validate_settings=validate_settings,
@@ -302,13 +302,17 @@
 
     def _register_extensions(self):
         sql = """
         CREATE EXTENSION IF NOT EXISTS fuzzystrmatch;
         """
         self._run_sql_execution(sql)
 
-    def _create_splink_schema(self):
+    def _create_splink_schema(self, other_schemas_to_search):
+        other_schemas_to_search = ensure_is_list(other_schemas_to_search)
+        # always search _db_schema first, and public last
+        schemas_to_search = [self._db_schema] + other_schemas_to_search + ["public"]
+        search_path = ",".join(schemas_to_search)
         sql = f"""
         CREATE SCHEMA IF NOT EXISTS {self._db_schema};
-        SET search_path TO {self._db_schema},public;
+        SET search_path TO {search_path};
         """
         self._run_sql_execution(sql)
```

### Comparing `splink-3.9.3/splink/postgres/postgres_helpers/postgres_base.py` & `splink-3.9.4/splink/postgres/postgres_helpers/postgres_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/postgres/postgres_helpers/postgres_comparison_imports.py` & `splink-3.9.4/splink/postgres/postgres_helpers/postgres_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/predict.py` & `splink-3.9.4/splink/predict.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/profile_data.py` & `splink-3.9.4/splink/profile_data.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/settings.py` & `splink-3.9.4/splink/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 from copy import deepcopy
 
-from .blocking import BlockingRule
+from .blocking import blocking_rule_to_obj
 from .charts import m_u_parameters_chart, match_weights_chart
 from .comparison import Comparison
 from .comparison_level import ComparisonLevel
 from .default_from_jsonschema import default_value_from_schema
 from .input_column import InputColumn
 from .misc import dedupe_preserving_order, prob_to_bayes_factor, prob_to_match_weight
 from .parse_sql import get_columns_used_from_sql
@@ -122,15 +122,17 @@
         a_cols = self._from_settings_dict_else_default("additional_columns_to_retain")
 
         # Add any columns used in blocking rules but not model
         if self._retain_matching_columns:
             # Want to add any columns not already by the model
             used_by_brs = []
             for br in self._blocking_rules_to_generate_predictions:
-                used_by_brs.extend(get_columns_used_from_sql(br.blocking_rule))
+                used_by_brs.extend(
+                    get_columns_used_from_sql(br.blocking_rule, br.sql_dialect)
+                )
 
             used_by_brs = [InputColumn(c) for c in used_by_brs]
 
             used_by_brs = [c.unquote().name() for c in used_by_brs]
             already_used = self._columns_used_by_comparisons
             already_used = [InputColumn(c) for c in already_used]
             already_used = [c.unquote().name() for c in already_used]
@@ -297,27 +299,17 @@
     def _get_comparison_by_output_column_name(self, name):
         for cc in self.comparisons:
             if cc._output_column_name == name:
                 return cc
         raise ValueError(f"No comparison column with name {name}")
 
     def _brs_as_objs(self, brs_as_strings):
-        brs_as_objs = []
-        for br in brs_as_strings:
-            if isinstance(br, dict):
-                br = BlockingRule(
-                    br["blocking_rule"], salting_partitions=br["salting_partitions"]
-                )
-                br.preceding_rules = brs_as_objs.copy()
-                brs_as_objs.append(br)
-            else:
-                br = BlockingRule(br)
-                br.preceding_rules = brs_as_objs.copy()
-                brs_as_objs.append(br)
-
+        brs_as_objs = [blocking_rule_to_obj(br) for br in brs_as_strings]
+        for n, br in enumerate(brs_as_objs):
+            br.add_preceding_rules(brs_as_objs[:n])
         return brs_as_objs
 
     def _get_comparison_levels_corresponding_to_training_blocking_rule(
         self, blocking_rule
     ):
         """
         If we block on (say) first name and surname, then all blocked comparisons are
@@ -333,15 +325,20 @@
         name, and one for an exact match on surname
 
         Or alternatively (and preferably, to avoid correlation issues), a comparison
         level for an exact match on first_name AND surname.   i.e. a single level for
         exact match on full name
 
         """
-        blocking_exact_match_columns = set(get_columns_used_from_sql(blocking_rule))
+        blocking_exact_match_columns = set(
+            get_columns_used_from_sql(
+                blocking_rule,
+                dialect=self._sql_dialect,
+            )
+        )
 
         ccs = self.comparisons
 
         exact_comparison_levels = []
         for cc in ccs:
             for cl in cc.comparison_levels:
                 if cl._is_exact_match:
```

### Comparing `splink-3.9.3/splink/settings_validator.py` & `splink-3.9.4/splink/settings_validator.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/spark/linker.py` & `splink-3.9.4/splink/spark/linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/spark/spark_helpers/custom_spark_dialect.py` & `splink-3.9.4/splink/spark/spark_helpers/custom_spark_dialect.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/spark/spark_helpers/spark_base.py` & `splink-3.9.4/splink/spark/spark_helpers/spark_base.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/spark/spark_helpers/spark_comparison_imports.py` & `splink-3.9.4/splink/spark/spark_helpers/spark_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/splink_comparison_viewer.py` & `splink-3.9.4/splink/splink_comparison_viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 import json
 import os
-import pkgutil
 from typing import TYPE_CHECKING
 
 from jinja2 import Template
 
-from .misc import EverythingEncoder
+from .misc import EverythingEncoder, read_resource
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
 
 
 def row_examples(linker: Linker, example_rows_per_category=2):
@@ -105,16 +104,15 @@
 ):
     # When developing the package, it can be easier to point
     # ar the script live on observable using <script src=>
     # rather than bundling the whole thing into the html
     bundle_observable_notebook = True
 
     template_path = "files/splink_comparison_viewer/template.j2"
-    template = pkgutil.get_data(__name__, template_path).decode("utf-8")
-    template = Template(template)
+    template = Template(read_resource(template_path))
 
     template_data = {
         "comparison_vector_data": json.dumps(
             comparison_vector_data, cls=EverythingEncoder
         ),
         "splink_settings": json.dumps(splink_settings),
     }
@@ -123,17 +121,15 @@
         "embed": "files/external_js/vega-embed@6.20.2",
         "vega": "files/external_js/vega@5.21.0",
         "vegalite": "files/external_js/vega-lite@5.2.0",
         "svu_text": "files/splink_vis_utils/splink_vis_utils.js",
         "custom_css": "files/splink_comparison_viewer/custom.css",
     }
     for k, v in files.items():
-        f = pkgutil.get_data(__name__, v)
-        f = f.decode("utf-8")
-        template_data[k] = f
+        template_data[k] = read_resource(v)
 
     template_data["bundle_observable_notebook"] = bundle_observable_notebook
 
     rendered = template.render(**template_data)
 
     if os.path.isfile(out_path) and not overwrite:
         raise ValueError(
```

### Comparing `splink-3.9.3/splink/splink_dataframe.py` & `splink-3.9.4/splink/splink_dataframe.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/sql_transform.py` & `splink-3.9.4/splink/sql_transform.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/sqlite/linker.py` & `splink-3.9.4/splink/sqlite/linker.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py` & `splink-3.9.4/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/term_frequencies.py` & `splink-3.9.4/splink/term_frequencies.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/unique_id_concat.py` & `splink-3.9.4/splink/unique_id_concat.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/unlinkables.py` & `splink-3.9.4/splink/unlinkables.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/validate_jsonschema.py` & `splink-3.9.4/splink/validate_jsonschema.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import operator
 from functools import lru_cache, reduce
 
-import pkg_resources
 from jsonschema import Draft7Validator
 
+from .misc import read_resource
+
 
 @lru_cache()
 def get_schema():
-    schema_loc = "files/settings_jsonschema.json"
-    with pkg_resources.resource_stream(__name__, schema_loc) as io:
-        return json.load(io)
+    path = "files/settings_jsonschema.json"
+    return json.loads(read_resource(path))
 
 
 def get_from_dict(dataDict, mapList):
     return reduce(operator.getitem, mapList, dataDict)
 
 
 def get_comparison_level(e, settings_dict):
```

### Comparing `splink-3.9.3/splink/vertically_concatenate.py` & `splink-3.9.4/splink/vertically_concatenate.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/splink/waterfall_chart.py` & `splink-3.9.4/splink/waterfall_chart.py`

 * *Files identical despite different names*

### Comparing `splink-3.9.3/PKG-INFO` & `splink-3.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splink
-Version: 3.9.3
+Version: 3.9.4
 Summary: Fast probabilistic data linkage at scale
 Home-page: https://github.com/moj-analytical-services/splink
 License: MIT
 Author: Robin Linacre
 Author-email: robinlinacre@hotmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -12,19 +12,19 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.0.3)
 Requires-Dist: altair (>=5.0.1,<6.0.0)
-Requires-Dist: duckdb (>=0.6.0)
+Requires-Dist: duckdb (>=0.8.0)
 Requires-Dist: jsonschema (>=3.2,<5.0)
 Requires-Dist: pandas (>=1.0.0)
 Requires-Dist: phonetics (>=1.0.5,<2.0.0)
-Requires-Dist: sqlglot (>=5.1.0,<11.4.2)
+Requires-Dist: sqlglot (>=7.0.0,<11.4.2)
 Project-URL: Repository, https://github.com/moj-analytical-services/splink
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/7570107/85285114-3969ac00-b488-11ea-88ff-5fca1b34af1f.png" alt="Splink Logo" height="150px">
 </p>
 
@@ -103,40 +103,45 @@
 
 For more detailed tutorial, please see [here](https://moj-analytical-services.github.io/splink/demos/00_Tutorial_Introduction.html).
 
 ```py
 from splink.duckdb.linker import DuckDBLinker
 import splink.duckdb.comparison_library as cl
 import splink.duckdb.comparison_template_library as ctl
+import splink.duckdb.blocking_rule_library as brl
 from splink.datasets import splink_datasets
 
 df = splink_datasets.fake_1000
 
 settings = {
     "link_type": "dedupe_only",
     "blocking_rules_to_generate_predictions": [
-        "l.first_name = r.first_name",
-        "l.surname = r.surname",
+        brl.exact_match_rule("first_name"),
+        brl.exact_match_rule("surname"),
     ],
     "comparisons": [
         ctl.name_comparison("first_name"),
         ctl.name_comparison("surname"),
         ctl.date_comparison("dob", cast_strings_to_date=True),
         cl.exact_match("city", term_frequency_adjustments=True),
         ctl.email_comparison("email"),
     ],
 }
 
 linker = DuckDBLinker(df, settings)
 linker.estimate_u_using_random_sampling(max_pairs=1e6)
 
-blocking_rule_for_training = "l.first_name = r.first_name and l.surname = r.surname"
+blocking_rule_for_training = brl.and_(
+                                brl.exact_match_rule("first_name"), 
+                                brl.exact_match_rule("surname")
+                                )
+
 linker.estimate_parameters_using_expectation_maximisation(blocking_rule_for_training)
 
-blocking_rule_for_training = "l.dob = r.dob"
+blocking_rule_for_training = brl.exact_match_rule("dob")
 linker.estimate_parameters_using_expectation_maximisation(blocking_rule_for_training)
 
 pairwise_predictions = linker.predict()
 
 clusters = linker.cluster_pairwise_predictions_at_threshold(pairwise_predictions, 0.95)
 clusters.as_pandas_dataframe(limit=5)
 ```
@@ -144,15 +149,15 @@
 ## Videos
 
 - [A introductory presentation on Splink](https://www.youtube.com/watch?v=msz3T741KQI)
 - [An introduction to the Splink Comparison Viewer dashboard](https://www.youtube.com/watch?v=DNvCMqjipis)
 
 ## Support
 
-Please post on the [discussion forums](https://github.com/moj-analytical-services/splink/discussions) if you have any questions. If you think you have found a bug, please raise an [issue](https://github.com/moj-analytical-services/splink/issues).
+To find the best place to ask a question, report a bug or get general advice, please refer to our [Contributing Guide](./CONTRIBUTING.md).
 
 ## Awards
 
 🥇 Analysis in Government Awards 2020: Innovative Methods: [Winner](https://www.gov.uk/government/news/launch-of-the-analysis-in-government-awards)
 
 🥇 MoJ DASD Awards 2020: Innovation and Impact - Winner
```

