# Comparing `tmp/ansys-systemcoupling-core-0.1.3.tar.gz` & `tmp/ansys_systemcoupling_core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-systemcoupling-core-0.1.3.tar", last modified: Mon Apr  3 14:32:10 2023, max compression
+gzip compressed data, was "ansys_systemcoupling_core-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys-systemcoupling-core-0.1.3.tar` & `ansys_systemcoupling_core-0.2.0.tar`

### file list

```diff
@@ -1,123 +1,129 @@
--rw-r--r--   0        0        0     1090 2023-04-03 14:30:50.252350 ansys-systemcoupling-core-0.1.3/LICENSE
--rw-r--r--   0        0        0     7934 2023-04-03 14:30:50.252350 ansys-systemcoupling-core-0.1.3/README.rst
--rw-r--r--   0        0        0     2798 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4017 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/__init__.py
--rw-r--r--   0        0        0      425 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/_version.py
--rw-r--r--   0        0        0      858 2023-04-03 14:31:57.088730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/abort.py
--rw-r--r--   0        0        0     1421 2023-04-03 14:31:55.148719 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/activate_hidden.py
--rw-r--r--   0        0        0     8249 2023-04-03 14:31:56.680728 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer.py
--rw-r--r--   0        0        0     8052 2023-04-03 14:31:56.704728 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer_by_display_names.py
--rw-r--r--   0        0        0     2044 2023-04-03 14:31:56.816729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_expression_function.py
--rw-r--r--   0        0        0     2163 2023-04-03 14:31:56.640728 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface.py
--rw-r--r--   0        0        0     2212 2023-04-03 14:31:56.652728 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface_by_display_names.py
--rw-r--r--   0        0        0     1150 2023-04-03 14:31:56.808729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_named_expression.py
--rw-r--r--   0        0        0     3659 2023-04-03 14:31:56.764729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_participant.py
--rw-r--r--   0        0        0     1170 2023-04-03 14:31:56.720728 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_reference_frame.py
--rw-r--r--   0        0        0     3347 2023-04-03 14:31:56.736729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_transformation.py
--rw-r--r--   0        0        0     9171 2023-04-03 14:31:56.124725 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/analysis_control.py
--rw-r--r--   0        0        0      839 2023-04-03 14:31:55.904724 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/apip.py
--rw-r--r--   0        0        0     1015 2023-04-03 14:31:56.576727 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/ascii_output.py
--rw-r--r--   0        0        0      403 2023-04-03 14:31:55.396721 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/attribute.py
--rw-r--r--   0        0        0     1456 2023-04-03 14:31:55.392721 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/attribute_child.py
--rw-r--r--   0        0        0     1200 2023-04-03 14:31:56.480727 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/available_ports.py
--rw-r--r--   0        0        0      980 2023-04-03 14:31:55.920724 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/avoid_data_reconstruction.py
--rw-r--r--   0        0        0     1385 2023-04-03 14:31:56.992730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/case_root.py
--rw-r--r--   0        0        0      380 2023-04-03 14:31:56.928730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/clear_state.py
--rw-r--r--   0        0        0      471 2023-04-03 14:31:56.464727 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_interface.py
--rw-r--r--   0        0        0     1089 2023-04-03 14:31:56.456727 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_interface_child.py
--rw-r--r--   0        0        0      579 2023-04-03 14:31:55.832723 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant.py
--rw-r--r--   0        0        0     5540 2023-04-03 14:31:55.824723 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant_child.py
--rw-r--r--   0        0        0     1118 2023-04-03 14:31:57.064730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/create_restart_point.py
--rw-r--r--   0        0        0      450 2023-04-03 14:31:56.312726 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/data_transfer.py
--rw-r--r--   0        0        0     6375 2023-04-03 14:31:56.304726 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/data_transfer_child.py
--rw-r--r--   0        0        0      509 2023-04-03 14:31:56.968730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/delete_snapshot.py
--rw-r--r--   0        0        0     1069 2023-04-03 14:31:56.748729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/delete_transformation.py
--rw-r--r--   0        0        0     2822 2023-04-03 14:31:55.368721 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/dimensionality.py
--rw-r--r--   0        0        0     6688 2023-04-03 14:31:55.744723 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/execution_control.py
--rw-r--r--   0        0        0      447 2023-04-03 14:31:55.188720 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/expression.py
--rw-r--r--   0        0        0     1039 2023-04-03 14:31:55.180719 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_child.py
--rw-r--r--   0        0        0      510 2023-04-03 14:31:55.216720 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_function.py
--rw-r--r--   0        0        0     1265 2023-04-03 14:31:55.208720 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_function_child.py
--rw-r--r--   0        0        0      595 2023-04-03 14:31:55.756723 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/external_data_file.py
--rw-r--r--   0        0        0     1879 2023-04-03 14:31:55.664722 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/fluent_input.py
--rw-r--r--   0        0        0      454 2023-04-03 14:31:55.636722 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/fmu_parameter.py
--rw-r--r--   0        0        0     3845 2023-04-03 14:31:55.632722 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/fmu_parameter_child.py
--rw-r--r--   0        0        0     1030 2023-04-03 14:31:56.788729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/generate_input_file.py
--rw-r--r--   0        0        0      660 2023-04-03 14:31:56.780729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/get_execution_command.py
--rw-r--r--   0        0        0      227 2023-04-03 14:31:57.072730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/get_machines.py
--rw-r--r--   0        0        0      730 2023-04-03 14:31:56.712728 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/get_region_names_for_participant.py
--rw-r--r--   0        0        0      772 2023-04-03 14:31:56.836729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/get_setup_summary.py
--rw-r--r--   0        0        0      277 2023-04-03 14:31:56.976730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/get_snapshots.py
--rw-r--r--   0        0        0     2222 2023-04-03 14:31:56.840729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/get_status_messages.py
--rw-r--r--   0        0        0     4506 2023-04-03 14:31:55.888724 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/global_stabilization.py
--rw-r--r--   0        0        0      903 2023-04-03 14:31:56.828729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/has_input_file_changed.py
--rw-r--r--   0        0        0      993 2023-04-03 14:31:56.796729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/import_system_coupling_input_file.py
--rw-r--r--   0        0        0     1025 2023-04-03 14:31:57.008730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/initialize.py
--rw-r--r--   0        0        0      507 2023-04-03 14:31:55.312720 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/instancing.py
--rw-r--r--   0        0        0     2231 2023-04-03 14:31:55.304720 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/instancing_child.py
--rw-r--r--   0        0        0      906 2023-04-03 14:31:57.080731 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/interrupt.py
--rw-r--r--   0        0        0      932 2023-04-03 14:31:55.324720 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/library.py
--rw-r--r--   0        0        0     8521 2023-04-03 14:31:56.440727 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/mapping_control.py
--rw-r--r--   0        0        0     4810 2023-04-03 14:31:56.940730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/open.py
--rw-r--r--   0        0        0     1063 2023-04-03 14:31:57.048730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/open_results_in_ensight.py
--rw-r--r--   0        0        0     1153 2023-04-03 14:31:56.964730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/open_snapshot.py
--rw-r--r--   0        0        0     4386 2023-04-03 14:31:56.624728 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/output_control.py
--rw-r--r--   0        0        0     6261 2023-04-03 14:31:57.044730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/partition_participants.py
--rw-r--r--   0        0        0      476 2023-04-03 14:31:55.284720 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/reference_frame.py
--rw-r--r--   0        0        0     2421 2023-04-03 14:31:55.276720 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/reference_frame_child.py
--rw-r--r--   0        0        0      393 2023-04-03 14:31:55.528721 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/region.py
--rw-r--r--   0        0        0     2238 2023-04-03 14:31:55.520722 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/region_child.py
--rw-r--r--   0        0        0      357 2023-04-03 14:31:56.824729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/reload_expression_function_modules.py
--rw-r--r--   0        0        0     2658 2023-04-03 14:31:56.560727 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/results.py
--rw-r--r--   0        0        0     1684 2023-04-03 14:31:56.948730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/save.py
--rw-r--r--   0        0        0     1950 2023-04-03 14:31:56.956730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/save_snapshot.py
--rw-r--r--   0        0        0     6233 2023-04-03 14:31:56.920729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/setup_root.py
--rw-r--r--   0        0        0      808 2023-04-03 14:31:57.016730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/shutdown.py
--rw-r--r--   0        0        0      372 2023-04-03 14:31:56.160725 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/side.py
--rw-r--r--   0        0        0     1721 2023-04-03 14:31:56.152725 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/side_child.py
--rw-r--r--   0        0        0     2845 2023-04-03 14:31:56.516727 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_control.py
--rw-r--r--   0        0        0     2604 2023-04-03 14:31:57.120731 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_root.py
--rw-r--r--   0        0        0     1057 2023-04-03 14:31:57.020730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/solve.py
--rw-r--r--   0        0        0     5536 2023-04-03 14:31:56.232725 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/stabilization.py
--rw-r--r--   0        0        0     1769 2023-04-03 14:31:57.004730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/start_participants.py
--rw-r--r--   0        0        0     1986 2023-04-03 14:31:57.028730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/step.py
--rw-r--r--   0        0        0      509 2023-04-03 14:31:55.248720 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/transformation.py
--rw-r--r--   0        0        0     1837 2023-04-03 14:31:55.240720 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/transformation_child.py
--rw-r--r--   0        0        0      879 2023-04-03 14:31:56.532727 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/type.py
--rw-r--r--   0        0        0     5626 2023-04-03 14:31:56.024724 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/unmapped_value_options.py
--rw-r--r--   0        0        0     1086 2023-04-03 14:31:55.544722 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/update_control.py
--rw-r--r--   0        0        0     2211 2023-04-03 14:31:56.772729 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/update_participant.py
--rw-r--r--   0        0        0      411 2023-04-03 14:31:55.488721 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/variable.py
--rw-r--r--   0        0        0     6137 2023-04-03 14:31:55.484721 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/variable_child.py
--rw-r--r--   0        0        0      656 2023-04-03 14:31:57.068730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/write_csv_chart_files.py
--rw-r--r--   0        0        0     1278 2023-04-03 14:31:57.060730 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/write_ensight.py
--rw-r--r--   0        0        0     3056 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/get_status_messages.py
--rw-r--r--   0        0        0     6915 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/injected_commands.py
--rw-r--r--   0        0        0    11596 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/root_source.py
--rw-r--r--   0        0        0    12043 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/static_info.py
--rw-r--r--   0        0        0     3568 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy.py
--rw-r--r--   0        0        0     1127 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy_interface.py
--rw-r--r--   0        0        0    23435 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/types.py
--rw-r--r--   0        0        0     9921 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/grpc_client.py
--rw-r--r--   0        0        0     1102 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/services/command_query.py
--rw-r--r--   0        0        0      994 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/services/output_stream.py
--rw-r--r--   0        0        0      529 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/services/process.py
--rw-r--r--   0        0        0     1364 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/services/solution.py
--rw-r--r--   0        0        0     1205 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/syc_container.py
--rw-r--r--   0        0        0     3499 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/syc_process.py
--rw-r--r--   0        0        0     1910 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/variant.py
--rw-r--r--   0        0        0       69 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/examples/__init__.py
--rw-r--r--   0        0        0     2950 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/examples/downloads.py
--rw-r--r--   0        0        0       34 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/native_api/__init__.py
--rw-r--r--   0        0        0      579 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/native_api/command_metadata.py
--rw-r--r--   0        0        0     3682 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/native_api/datamodel_metadata.py
--rw-r--r--   0        0        0      307 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/native_api/meta_wrapper.py
--rw-r--r--   0        0        0     5962 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/native_api/native_api.py
--rw-r--r--   0        0        0     2999 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/native_api/object_path.py
--rw-r--r--   0        0        0     7075 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/session.py
--rw-r--r--   0        0        0     3886 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/util/logging.py
--rw-r--r--   0        0        0      316 2023-04-03 14:30:50.260350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/util/name_util.py
--rw-r--r--   0        0        0      788 2023-04-03 14:30:50.264350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/util/pathstr.py
--rw-r--r--   0        0        0     3391 2023-04-03 14:30:50.264350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/util/state_keys.py
--rw-r--r--   0        0        0     1828 2023-04-03 14:30:50.264350 ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/util/yaml_helper.py
--rw-r--r--   0        0        0    10741 1970-01-01 00:00:00.000000 ansys-systemcoupling-core-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-07-19 15:23:52.241656 ansys_systemcoupling_core-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8080 2023-07-19 15:23:52.241656 ansys_systemcoupling_core-0.2.0/README.rst
+-rw-r--r--   0        0        0     2795 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4710 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/__init__.py
+-rw-r--r--   0        0        0      425 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/_version.py
+-rw-r--r--   0        0        0      858 2023-07-19 15:25:34.576585 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/abort.py
+-rw-r--r--   0        0        0     1421 2023-07-19 15:25:32.732606 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/activate_hidden.py
+-rw-r--r--   0        0        0     8249 2023-07-19 15:25:34.192589 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer.py
+-rw-r--r--   0        0        0     8052 2023-07-19 15:25:34.216589 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer_by_display_names.py
+-rw-r--r--   0        0        0     2044 2023-07-19 15:25:34.320588 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_expression_function.py
+-rw-r--r--   0        0        0     2163 2023-07-19 15:25:34.152590 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface.py
+-rw-r--r--   0        0        0     2212 2023-07-19 15:25:34.168590 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface_by_display_names.py
+-rw-r--r--   0        0        0     1150 2023-07-19 15:25:34.308588 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_named_expression.py
+-rw-r--r--   0        0        0     3659 2023-07-19 15:25:34.268588 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_participant.py
+-rw-r--r--   0        0        0     1170 2023-07-19 15:25:34.228589 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_reference_frame.py
+-rw-r--r--   0        0        0     3347 2023-07-19 15:25:34.244589 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_transformation.py
+-rw-r--r--   0        0        0     9461 2023-07-19 15:25:33.668595 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/analysis_control.py
+-rw-r--r--   0        0        0      839 2023-07-19 15:25:33.444598 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/apip.py
+-rw-r--r--   0        0        0     1015 2023-07-19 15:25:34.068591 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/ascii_output.py
+-rw-r--r--   0        0        0      403 2023-07-19 15:25:32.960603 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/attribute.py
+-rw-r--r--   0        0        0     1456 2023-07-19 15:25:32.956603 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/attribute_child.py
+-rw-r--r--   0        0        0     1428 2023-07-19 15:25:33.576596 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/automatic_alignment_options.py
+-rw-r--r--   0        0        0     1200 2023-07-19 15:25:33.980592 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/available_ports.py
+-rw-r--r--   0        0        0     1353 2023-07-19 15:25:33.464598 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/avoid_data_reconstruction.py
+-rw-r--r--   0        0        0     1385 2023-07-19 15:25:34.476586 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/case_root.py
+-rw-r--r--   0        0        0      380 2023-07-19 15:25:34.412587 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/clear_state.py
+-rw-r--r--   0        0        0      471 2023-07-19 15:25:33.964592 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_interface.py
+-rw-r--r--   0        0        0     1089 2023-07-19 15:25:33.960592 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_interface_child.py
+-rw-r--r--   0        0        0      579 2023-07-19 15:25:33.380598 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant.py
+-rw-r--r--   0        0        0     5540 2023-07-19 15:25:33.372599 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant_child.py
+-rw-r--r--   0        0        0     1118 2023-07-19 15:25:34.544585 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/create_restart_point.py
+-rw-r--r--   0        0        0      450 2023-07-19 15:25:33.836593 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/data_transfer.py
+-rw-r--r--   0        0        0     6375 2023-07-19 15:25:33.828593 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/data_transfer_child.py
+-rw-r--r--   0        0        0      509 2023-07-19 15:25:34.452587 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/delete_snapshot.py
+-rw-r--r--   0        0        0     1069 2023-07-19 15:25:34.252589 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/delete_transformation.py
+-rw-r--r--   0        0        0     2822 2023-07-19 15:25:32.932603 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/dimensionality.py
+-rw-r--r--   0        0        0     6688 2023-07-19 15:25:33.300599 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/execution_control.py
+-rw-r--r--   0        0        0      447 2023-07-19 15:25:32.764605 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression.py
+-rw-r--r--   0        0        0     1039 2023-07-19 15:25:32.760605 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_child.py
+-rw-r--r--   0        0        0      510 2023-07-19 15:25:32.792605 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_function.py
+-rw-r--r--   0        0        0     1265 2023-07-19 15:25:32.784605 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_function_child.py
+-rw-r--r--   0        0        0      595 2023-07-19 15:25:33.312599 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/external_data_file.py
+-rw-r--r--   0        0        0     1879 2023-07-19 15:25:33.224600 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/fluent_input.py
+-rw-r--r--   0        0        0      454 2023-07-19 15:25:33.200600 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/fmu_parameter.py
+-rw-r--r--   0        0        0     4880 2023-07-19 15:25:33.196601 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/fmu_parameter_child.py
+-rw-r--r--   0        0        0     1030 2023-07-19 15:25:34.292588 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/generate_input_file.py
+-rw-r--r--   0        0        0      660 2023-07-19 15:25:34.284588 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_execution_command.py
+-rw-r--r--   0        0        0      227 2023-07-19 15:25:34.564585 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_machines.py
+-rw-r--r--   0        0        0      730 2023-07-19 15:25:34.224589 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_region_names_for_participant.py
+-rw-r--r--   0        0        0      772 2023-07-19 15:25:34.336588 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_setup_summary.py
+-rw-r--r--   0        0        0      277 2023-07-19 15:25:34.456586 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_snapshots.py
+-rw-r--r--   0        0        0     2222 2023-07-19 15:25:34.340588 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_status_messages.py
+-rw-r--r--   0        0        0      999 2023-07-19 15:25:34.552585 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_transformation.py
+-rw-r--r--   0        0        0     4506 2023-07-19 15:25:33.432598 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/global_stabilization.py
+-rw-r--r--   0        0        0      903 2023-07-19 15:25:34.332588 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/has_input_file_changed.py
+-rw-r--r--   0        0        0      993 2023-07-19 15:25:34.300588 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/import_system_coupling_input_file.py
+-rw-r--r--   0        0        0     1025 2023-07-19 15:25:34.488586 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/initialize.py
+-rw-r--r--   0        0        0      507 2023-07-19 15:25:32.880604 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/instancing.py
+-rw-r--r--   0        0        0     2231 2023-07-19 15:25:32.876604 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/instancing_child.py
+-rw-r--r--   0        0        0      906 2023-07-19 15:25:34.568585 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/interrupt.py
+-rw-r--r--   0        0        0      932 2023-07-19 15:25:32.892604 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/library.py
+-rw-r--r--   0        0        0      486 2023-07-19 15:25:34.092590 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/live_visualization.py
+-rw-r--r--   0        0        0     2250 2023-07-19 15:25:34.088590 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/live_visualization_child.py
+-rw-r--r--   0        0        0     8521 2023-07-19 15:25:33.944592 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/mapping_control.py
+-rw-r--r--   0        0        0     4810 2023-07-19 15:25:34.424587 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open.py
+-rw-r--r--   0        0        0     1903 2023-07-19 15:25:34.532585 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open_results_in_en_sight.py
+-rw-r--r--   0        0        0     1063 2023-07-19 15:24:54.289057 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open_results_in_ensight.py
+-rw-r--r--   0        0        0     1153 2023-07-19 15:25:34.448587 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open_snapshot.py
+-rw-r--r--   0        0        0     4587 2023-07-19 15:25:34.140590 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/output_control.py
+-rw-r--r--   0        0        0     6261 2023-07-19 15:25:34.520586 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/partition_participants.py
+-rw-r--r--   0        0        0      476 2023-07-19 15:25:32.856604 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/reference_frame.py
+-rw-r--r--   0        0        0     2421 2023-07-19 15:25:32.848604 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/reference_frame_child.py
+-rw-r--r--   0        0        0      393 2023-07-19 15:25:33.092602 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/region.py
+-rw-r--r--   0        0        0     2238 2023-07-19 15:25:33.088602 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/region_child.py
+-rw-r--r--   0        0        0      357 2023-07-19 15:25:34.324588 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/reload_expression_function_modules.py
+-rw-r--r--   0        0        0     2658 2023-07-19 15:25:34.052591 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/results.py
+-rw-r--r--   0        0        0     1684 2023-07-19 15:25:34.432587 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/save.py
+-rw-r--r--   0        0        0     1950 2023-07-19 15:25:34.440587 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/save_snapshot.py
+-rw-r--r--   0        0        0     6233 2023-07-19 15:25:34.404587 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/setup_root.py
+-rw-r--r--   0        0        0      808 2023-07-19 15:25:34.496586 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/shutdown.py
+-rw-r--r--   0        0        0      372 2023-07-19 15:25:33.700595 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/side.py
+-rw-r--r--   0        0        0     1721 2023-07-19 15:25:33.696595 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/side_child.py
+-rw-r--r--   0        0        0     2845 2023-07-19 15:25:34.016591 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_control.py
+-rw-r--r--   0        0        0     2821 2023-07-19 15:25:34.604585 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_root.py
+-rw-r--r--   0        0        0     1057 2023-07-19 15:25:34.500586 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solve.py
+-rw-r--r--   0        0        0     5536 2023-07-19 15:25:33.764594 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/stabilization.py
+-rw-r--r--   0        0        0     1769 2023-07-19 15:25:34.484586 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/start_participants.py
+-rw-r--r--   0        0        0     1986 2023-07-19 15:25:34.508586 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/step.py
+-rw-r--r--   0        0        0      509 2023-07-19 15:25:32.820605 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/transformation.py
+-rw-r--r--   0        0        0     1837 2023-07-19 15:25:32.816605 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/transformation_child.py
+-rw-r--r--   0        0        0      879 2023-07-19 15:25:34.032591 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/type.py
+-rw-r--r--   0        0        0     5626 2023-07-19 15:25:33.556596 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/unmapped_value_options.py
+-rw-r--r--   0        0        0     1086 2023-07-19 15:25:33.108601 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/update_control.py
+-rw-r--r--   0        0        0     2211 2023-07-19 15:25:34.276588 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/update_participant.py
+-rw-r--r--   0        0        0      411 2023-07-19 15:25:33.056602 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/variable.py
+-rw-r--r--   0        0        0     7249 2023-07-19 15:25:33.052602 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/variable_child.py
+-rw-r--r--   0        0        0      656 2023-07-19 15:25:34.556585 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/write_csv_chart_files.py
+-rw-r--r--   0        0        0     1278 2023-07-19 15:25:34.540585 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/write_ensight.py
+-rw-r--r--   0        0        0     3056 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/get_status_messages.py
+-rw-r--r--   0        0        0     6915 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/injected_commands.py
+-rw-r--r--   0        0        0    11596 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/root_source.py
+-rw-r--r--   0        0        0    12126 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/static_info.py
+-rw-r--r--   0        0        0     3568 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy.py
+-rw-r--r--   0        0        0     1127 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy_interface.py
+-rw-r--r--   0        0        0    23435 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/types.py
+-rw-r--r--   0        0        0    10124 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/grpc_client.py
+-rw-r--r--   0        0        0     1102 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/services/command_query.py
+-rw-r--r--   0        0        0      994 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/services/output_stream.py
+-rw-r--r--   0        0        0      529 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/services/process.py
+-rw-r--r--   0        0        0     1364 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/services/solution.py
+-rw-r--r--   0        0        0     1547 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/syc_container.py
+-rw-r--r--   0        0        0     4481 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/syc_process.py
+-rw-r--r--   0        0        0     1910 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/variant.py
+-rw-r--r--   0        0        0       69 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/examples/__init__.py
+-rw-r--r--   0        0        0     2946 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/examples/downloads.py
+-rw-r--r--   0        0        0       34 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/native_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/native_api/command_metadata.py
+-rw-r--r--   0        0        0     3682 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/native_api/datamodel_metadata.py
+-rw-r--r--   0        0        0      307 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/native_api/meta_wrapper.py
+-rw-r--r--   0        0        0     5962 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/native_api/native_api.py
+-rw-r--r--   0        0        0     2999 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/native_api/object_path.py
+-rw-r--r--   0        0        0     7079 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/session.py
+-rw-r--r--   0        0        0     1913 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/syc_version.py
+-rw-r--r--   0        0        0     3886 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/util/logging.py
+-rw-r--r--   0        0        0      316 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/util/name_util.py
+-rw-r--r--   0        0        0      788 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/util/pathstr.py
+-rw-r--r--   0        0        0     3391 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/util/state_keys.py
+-rw-r--r--   0        0        0     1828 2023-07-19 15:23:52.249656 ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/util/yaml_helper.py
+-rw-r--r--   0        0        0    10883 1970-01-01 00:00:00.000000 ansys_systemcoupling_core-0.2.0/PKG-INFO
```

### Comparing `ansys-systemcoupling-core-0.1.3/LICENSE` & `ansys_systemcoupling_core-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/README.rst` & `ansys_systemcoupling_core-0.2.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 PySystemCoupling
 ================
-.. TODO : add codecov badge once public
 
-|pyansys| |GH-CI| |MIT| |black|
+|pyansys| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
 
-.. |GH-CI| image:: https://github.com/pyansys/pysystem-coupling/actions/workflows/ci.yml/badge.svg
-   :target: https://github.com/pyansys/pysystem-coupling/actions/workflows/ci.yml
+.. |GH-CI| image:: https://github.com/ansys/pysystem-coupling/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/ansys/pysystem-coupling/actions/workflows/ci.yml
 
 .. |codecov| image:: https://codecov.io/gh/pysystem-coupling/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/pysystem-coupling
+   :target: https://codecov.io/gh/ansys/pysystem-coupling
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
   :target: https://github.com/psf/black
   :alt: black
@@ -43,47 +42,50 @@
 
 
 Alternatively, clone and install PySystemCoupling in *development mode*
 with this code:
 
 .. code::
 
-   git clone https://github.com/pyansys/pysystem-coupling.git
+   git clone https://github.com/ansys/pysystem-coupling.git
    cd pysystem-coupling
    python -m pip install --upgrade pip
    pip install -e .
    pip install .[classesgen]
    python scripts\generate_datamodel.py
 
 
 Documentation and Issues
 ------------------------
 
 For more information, see the `Documentation <https://systemcoupling.docs.pyansys.com>`_ page.
 
-Use the `PySystemCoupling Issues <https://github.com/pyansys/pysystem-coupling/issues>`_ page to
+Use the `PySystemCoupling Issues <https://github.com/ansys/pysystem-coupling/issues>`_ page to
 post bug reports, questions and feature requests.
 
 Usage
 -----
 
 It is assumed that an Ansys installation is available and that this installation
 includes System Coupling and the participant products needed for the coupled analysis.
 
 The System Coupling installation is found by examining the following environment variables
 in this order:
 
 * ``SYSC_ROOT``
 * ``AWP_ROOT``
-* ``AWP_ROOT231``
+* ``AWP_ROOT232``
 
 If a variable is set but does not refer to a valid installation, PySystemCoupling
-fail at that point, rather than attempting to use the next variable.
+fails at that point, rather than attempting to use the next variable.
 
-In a standard user installation, the expectation is that only ``AWP_ROOT231`` is set.
+In a standard user installation, the expectation is that only ``AWP_ROOT232`` is set.
+
+(It is also possible to provide a different version number as an argument to the ``launch()``
+function. This will affect which ``AWP_ROOT<version>`` environment variable is examined.)
 
 The System Coupling API is exposed to PySystemCoupling in two forms:
 
 * A documented interface based on concrete Python classes, following Pythonic conventions
 * A dynamic interface, undocumented in PySystemCoupling, that replicates the native System Coupling API
 
 Both forms are strongly related to each other. A key difference in the Pythonic API is that naming
```

### Comparing `ansys-systemcoupling-core-0.1.3/pyproject.toml` & `ansys_systemcoupling_core-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-systemcoupling-core"
-version = "0.1.3"
+version = "0.2.0"
 description = "A Python wrapper for Ansys System Coupling."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.support@ansys.com"},
 ]
 maintainers = [
     {name = "PyAnsys developers", email = "pyansys.maintainers@ansys.com"},
 ]
 dependencies = [
 	"ansys-api-systemcoupling==0.1.0",
 	"grpcio>=1.30.0",
-	"grpcio-status>=1.30.0,<1.51.2",
+	"grpcio-status>=1.30.0,<1.56.1",
 	"googleapis-common-protos>=1.50.0",
 	"protobuf>=3.20.1,<4.0.0",
 	"psutil>=5.7.0",
 	"pyyaml",
 	"appdirs>=1.4.0",
 	"importlib-metadata>=4.0",
 ]
@@ -48,61 +48,61 @@
 classesgen = [
 	# Dependencies for API class generation from System Coupling metadata
 
 	# NB
 	# black and isort are called programmatically to keep generated code
 	# consistent with style elsewhere. We need to keep the versions in
 	# sync with the precommit dependencies.
-	"black==23.1.0",
+	"black==23.7.0",
 	"isort==5.12.0",
 ]
 doc = [
-	"ansys-sphinx-theme==0.9.5",
+	"ansys-sphinx-theme==0.9.9",
 	"jupyter_sphinx==0.4.0",
 	"matplotlib",
 	"numpydoc==1.5.0",
 	"pypandoc==1.11",
 	"pytest-sphinx==0.5.0",
-	"Sphinx==5.3.0",
+	"Sphinx==7.0.1",
 	"sphinx-autobuild==2021.3.14",
-	"sphinx-autodoc-typehints==1.22",
-	"sphinx-copybutton==0.5.1",
-	"sphinx-gallery==0.12.2",
+	"sphinx-autodoc-typehints==1.23.3",
+	"sphinx-copybutton==0.5.2",
+	"sphinx-gallery==0.13.0",
 	"sphinx-notfound-page==0.8.3",
 	"sphinxcontrib-websupport==1.2.4",
 	"sphinxemoji==0.2.0",
 
 	# pyansys dependencies for sphinx gallery examples
 	"ansys-fluent-core",
 	"ansys-dpf-core",
 ]
 style = [
-	"codespell==2.2.4",
+	"codespell==2.2.5",
 	"flake8==6.0.0",
 ]
 tests = [
 	"pytest",
 	"pytest-cov",
 	"psutil>=5.7.0",
 ]
 
 [tool.flit.module]
 name = "ansys.systemcoupling.core"
 
 [project.urls]
-Source = "https://github.com/pyansys/pysystem-coupling/"
-Homepage = "https://github.com/pyansys/pysystem-coupling/"
+Source = "https://github.com/ansys/pysystem-coupling/"
+Homepage = "https://github.com/ansys/pysystem-coupling/"
 Documentation = "https://systemcoupling.docs.pyansys.com/"
-Tracker = "https://github.com/pyansys/pysystem-coupling/issues"
+Tracker = "https://github.com/ansys/pysystem-coupling/issues"
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 default_section = "THIRDPARTY"
 skip_glob = ["*__init__.py"]
 filter_files = "true"
 src_paths = ["doc", "src", "tests"]
 
 [tool.coverage.run]
 omit = [
     "*/adaptor/api/*",
-]
+]
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/__init__.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 def launch(
     *,
     port: int = None,
     working_dir: str = None,
     nprocs: int = None,
     sycnprocs: int = None,
+    version: str = None,
     extra_args: List[str] = [],
 ) -> Session:
     """Start a local instance of System Coupling and connect to it.
 
     Parameters
     ----------
     port : int, optional
@@ -36,14 +37,23 @@
         the client process is used.
     nprocs : int, optional
         Number of processes for coupling participants. The default is
         ``None``, in which case the System Coupling server uses its own default.
     sycnprocs : int, optional
         Number of processes for the System Coupling engine. The default is
         ``None``, in which case the System Coupling server uses its own default.
+    version : str, optional
+        String specifying the version of System Coupling to use. For example,
+        to use System Coupling from the Ansys "2023 R1" release, specify ``"231"``.
+        (The forms ``"23.1"`` and ``"23_1"`` are also acceptable.)
+        The version will be sought in the standard installation location. The
+        default is ``None``, which is equivalent to specifying
+        ``"232"`` ("2023 R2" release), unless either of the environment
+        variables ``SYSC_ROOT`` or ``AWP_ROOT`` has been set. It is considered
+        to be an error if either these is set *and* ``version`` is provided.
     extra_args : List[str]
         List of any additional arguments to specify when the server
         process is launched. The default is ``[]``. If a list of additional
         arguments is provided, it is concatenated as-is to the list of
         arguments already being passed when the process is started. If
         an argument has an associated value, the argument name and its
         value should be specified as two consecutive items of the list.
@@ -56,37 +66,41 @@
     """
     rpc = SycGrpc()
     rpc.start_and_connect(
         port=port,
         working_dir=working_dir,
         nprocs=nprocs,
         sycnprocs=sycnprocs,
+        version=version,
         extra_args=extra_args,
     )
     syc = Session(rpc)
     return syc
 
 
 def launch_container(
-    mounted_from: str = "./", mounted_to: str = "/working", network: str = None
+    mounted_from: str = "./",
+    mounted_to: str = "/working",
+    network: str = None,
+    version: str = None,
 ) -> Session:
     """Start a System Coupling container instance and connect to it.
 
     .. note::
        The container is currently only intended to be used for
        testing and development purposes.
 
     Returns
     -------
     ansys.systemcoupling.core.session.Session
         Session object, providing access to a set up and solve API controlling a
         remote System Coupling instance.
     """
     rpc = SycGrpc()
-    rpc.start_container_and_connect(mounted_from, mounted_to, network)
+    rpc.start_container_and_connect(mounted_from, mounted_to, network, version=version)
     syc = Session(rpc)
     return syc
 
 
 def connect(host: str, port: int) -> Session:  # pragma: no cover
     """Connect to an instance of System Coupling already running in server mode.
 
@@ -106,20 +120,18 @@
     rpc = SycGrpc()
     rpc.connect(host, port)
     syc = Session(rpc)
     return syc
 
 
 # Set up data directory
-try:
-    USER_DATA_PATH = appdirs.user_data_dir("ansys_systemcoupling_core")
-    if not os.path.exists(USER_DATA_PATH):  # pragma: no cover
-        os.makedirs(USER_DATA_PATH)
-
-    EXAMPLES_PATH = os.path.join(USER_DATA_PATH, "examples")
-    if not os.path.exists(EXAMPLES_PATH):  # pragma: no cover
-        os.makedirs(EXAMPLES_PATH)
-
-except:  # pragma: no cover
-    pass
+USER_DATA_PATH = appdirs.user_data_dir(
+    appname="ansys_systemcoupling_core", appauthor="Ansys"
+)
+if not os.path.exists(USER_DATA_PATH):  # pragma: no cover
+    os.makedirs(USER_DATA_PATH)
+
+EXAMPLES_PATH = os.path.join(USER_DATA_PATH, "examples")
+if not os.path.exists(EXAMPLES_PATH):  # pragma: no cover
+    os.makedirs(EXAMPLES_PATH)
 
 BUILDING_GALLERY = False
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/abort.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/abort.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/activate_hidden.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/activate_hidden.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer_by_display_names.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer_by_display_names.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_expression_function.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_expression_function.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface_by_display_names.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface_by_display_names.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_named_expression.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_named_expression.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_participant.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_participant.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_reference_frame.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_reference_frame.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/add_transformation.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_transformation.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/analysis_control.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/analysis_control.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #
 # This is an auto-generated file.  DO NOT EDIT!
 #
 
 from ansys.systemcoupling.core.adaptor.impl.types import *
 
 from .apip import apip
+from .automatic_alignment_options import automatic_alignment_options
 from .avoid_data_reconstruction import avoid_data_reconstruction
 from .global_stabilization import global_stabilization
 from .unmapped_value_options import unmapped_value_options
 
 
 class analysis_control(Container):
     """
@@ -18,14 +19,15 @@
     syc_name = "AnalysisControl"
 
     child_names = [
         "global_stabilization",
         "apip",
         "avoid_data_reconstruction",
         "unmapped_value_options",
+        "automatic_alignment_options",
     ]
 
     global_stabilization: global_stabilization = global_stabilization
     """
     global_stabilization child of analysis_control.
     """
     apip: apip = apip
@@ -36,14 +38,20 @@
     """
     avoid_data_reconstruction child of analysis_control.
     """
     unmapped_value_options: unmapped_value_options = unmapped_value_options
     """
     unmapped_value_options child of analysis_control.
     """
+    automatic_alignment_options: automatic_alignment_options = (
+        automatic_alignment_options
+    )
+    """
+    automatic_alignment_options child of analysis_control.
+    """
     property_names_types = [
         ("analysis_type", "AnalysisType", "str"),
         ("optimize_if_one_way", "OptimizeIfOneWay", "bool"),
         ("warped_face_tolerance", "WarpedFaceTolerance", "RealType"),
         ("allow_simultaneous_update", "AllowSimultaneousUpdate", "bool"),
         ("simultaneous_participants", "SimultaneousParticipants", "str"),
         ("partitioning_algorithm", "PartitioningAlgorithm", "str"),
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/apip.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/apip.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/ascii_output.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/ascii_output.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/attribute_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/attribute_child.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/available_ports.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/available_ports.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/avoid_data_reconstruction.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/avoid_data_reconstruction.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     """
 
     syc_name = "AvoidDataReconstruction"
 
     property_names_types = [
         ("volume_mapping", "VolumeMapping", "bool"),
         ("surface_mapping", "SurfaceMapping", "bool"),
+        ("surface_volume_mapping", "SurfaceVolumeMapping", "bool"),
     ]
 
     @property
     def volume_mapping(self) -> bool:
         """UNDOCUMENTED"""
         return self.get_property_state("volume_mapping")
 
@@ -30,7 +31,16 @@
     def surface_mapping(self) -> bool:
         """UNDOCUMENTED"""
         return self.get_property_state("surface_mapping")
 
     @surface_mapping.setter
     def surface_mapping(self, value: bool):
         self.set_property_state("surface_mapping", value)
+
+    @property
+    def surface_volume_mapping(self) -> bool:
+        """UNDOCUMENTED"""
+        return self.get_property_state("surface_volume_mapping")
+
+    @surface_volume_mapping.setter
+    def surface_volume_mapping(self, value: bool):
+        self.set_property_state("surface_volume_mapping", value)
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/case_root.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/case_root.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_interface_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_interface_child.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant_child.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
     @participant_analysis_type.setter
     def participant_analysis_type(self, value: str):
         self.set_property_state("participant_analysis_type", value)
 
     @property
     def use_new_apis(self) -> bool:
-        """Controls whether a Fluent or MAPDL participant should communicate using new APIs."""
+        """Controls whether Fluent/MAPDL/AEDT participant should communicate using new APIs."""
         return self.get_property_state("use_new_apis")
 
     @use_new_apis.setter
     def use_new_apis(self, value: bool):
         self.set_property_state("use_new_apis", value)
 
     @property
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/create_restart_point.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/create_restart_point.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/data_transfer_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/data_transfer_child.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/delete_transformation.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/delete_transformation.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/dimensionality.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/dimensionality.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/execution_control.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/execution_control.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_child.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_function_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_function_child.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/external_data_file.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/external_data_file.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/fluent_input.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/fluent_input.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/generate_input_file.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/generate_input_file.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/get_execution_command.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_execution_command.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/get_region_names_for_participant.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_region_names_for_participant.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/get_setup_summary.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_setup_summary.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/get_status_messages.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_status_messages.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/global_stabilization.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/global_stabilization.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/has_input_file_changed.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/has_input_file_changed.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/import_system_coupling_input_file.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/import_system_coupling_input_file.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/initialize.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/initialize.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/instancing_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/instancing_child.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/interrupt.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/interrupt.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/library.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/library.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/mapping_control.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/mapping_control.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/open.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/open_results_in_ensight.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open_results_in_ensight.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/open_snapshot.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open_snapshot.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/output_control.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/output_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 #
 # This is an auto-generated file.  DO NOT EDIT!
 #
 
 from ansys.systemcoupling.core.adaptor.impl.types import *
 
 from .ascii_output import ascii_output
+from .live_visualization import live_visualization
 from .results import results
 
 
 class output_control(Container):
     """
     Configure output controls.
     """
 
     syc_name = "OutputControl"
 
-    child_names = ["results", "ascii_output"]
+    child_names = ["results", "ascii_output", "live_visualization"]
 
     results: results = results
     """
     results child of output_control.
     """
     ascii_output: ascii_output = ascii_output
     """
     ascii_output child of output_control.
     """
+    live_visualization: live_visualization = live_visualization
+    """
+    live_visualization child of output_control.
+    """
     property_names_types = [
         ("option", "Option", "str"),
         ("generate_csv_chart_output", "GenerateCSVChartOutput", "bool"),
         ("write_initial_snapshot", "WriteInitialSnapshot", "bool"),
         ("transcript_precision", "TranscriptPrecision", "int"),
         ("write_diagnostics", "WriteDiagnostics", "bool"),
         ("write_weights_matrix", "WriteWeightsMatrix", "bool"),
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/partition_participants.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/partition_participants.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/reference_frame_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/reference_frame_child.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/region_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/region_child.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/results.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/results.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/save.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/save.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/save_snapshot.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/save_snapshot.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/setup_root.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/setup_root.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This is an auto-generated file.  DO NOT EDIT!
 #
 
-SHASH = "e31caa885d130e78b88ec2e8887d2f24196dd0c65cc56a2868f7cc08799f5c0f"
+SHASH = "f0b84f45a076885c3300d060703c9aa41ff964ebaf19d26017f53d9b71df370f"
 
 from ansys.systemcoupling.core.adaptor.impl.types import *
 
 from .activate_hidden import activate_hidden
 from .add_data_transfer import add_data_transfer
 from .add_data_transfer_by_display_names import add_data_transfer_by_display_names
 from .add_expression_function import add_expression_function
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/shutdown.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/shutdown.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/side_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/side_child.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_control.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_control.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_root.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_root.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #
 # This is an auto-generated file.  DO NOT EDIT!
 #
 
-SHASH = "e7829f64a4064be60caa10ab0c964633e99d1ffb276762c0ac858a2631050c69"
+SHASH = "5ea5d97aed6965ab7eb7bb9d10061e138b000af99b3419e5b772e92989f1c903"
 
 from ansys.systemcoupling.core.adaptor.impl.types import *
 
 from .abort import abort
 from .create_restart_point import create_restart_point
 from .get_machines import get_machines
+from .get_transformation import get_transformation
 from .initialize import initialize
 from .interrupt import interrupt
-from .open_results_in_ensight import open_results_in_ensight
+from .open_results_in_en_sight import open_results_in_en_sight
 from .partition_participants import partition_participants
 from .shutdown import shutdown
 from .solve import solve
 from .start_participants import start_participants
 from .step import step
 from .write_csv_chart_files import write_csv_chart_files
 from .write_ensight import write_ensight
@@ -31,17 +32,18 @@
     command_names = [
         "start_participants",
         "initialize",
         "shutdown",
         "solve",
         "step",
         "partition_participants",
-        "open_results_in_ensight",
+        "open_results_in_en_sight",
         "write_ensight",
         "create_restart_point",
+        "get_transformation",
         "write_csv_chart_files",
         "get_machines",
         "interrupt",
         "abort",
     ]
 
     start_participants: start_participants = start_participants
@@ -64,26 +66,30 @@
     """
     step command of solution_root.
     """
     partition_participants: partition_participants = partition_participants
     """
     partition_participants command of solution_root.
     """
-    open_results_in_ensight: open_results_in_ensight = open_results_in_ensight
+    open_results_in_en_sight: open_results_in_en_sight = open_results_in_en_sight
     """
-    open_results_in_ensight command of solution_root.
+    open_results_in_en_sight command of solution_root.
     """
     write_ensight: write_ensight = write_ensight
     """
     write_ensight command of solution_root.
     """
     create_restart_point: create_restart_point = create_restart_point
     """
     create_restart_point command of solution_root.
     """
+    get_transformation: get_transformation = get_transformation
+    """
+    get_transformation command of solution_root.
+    """
     write_csv_chart_files: write_csv_chart_files = write_csv_chart_files
     """
     write_csv_chart_files command of solution_root.
     """
     get_machines: get_machines = get_machines
     """
     get_machines command of solution_root.
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/solve.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solve.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/stabilization.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/stabilization.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/start_participants.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/start_participants.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/step.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/step.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/transformation_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/transformation_child.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/type.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/type.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/unmapped_value_options.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/unmapped_value_options.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/update_control.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/update_control.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/update_participant.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/update_participant.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/variable_child.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/variable_child.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,18 +26,21 @@
         ("participant_display_name", "ParticipantDisplayName", "str"),
         ("display_name", "DisplayName", "str"),
         ("data_type", "DataType", "str"),
         ("real_initial_value", "RealInitialValue", "RealType"),
         ("integer_initial_value", "IntegerInitialValue", "int"),
         ("logical_initial_value", "LogicalInitialValue", "bool"),
         ("string_initial_value", "StringInitialValue", "str"),
+        ("enumeration_initial_value", "EnumerationInitialValue", "int"),
         ("real_min", "RealMin", "RealType"),
         ("real_max", "RealMax", "RealType"),
         ("integer_min", "IntegerMin", "int"),
         ("integer_max", "IntegerMax", "int"),
+        ("enumeration_min", "EnumerationMin", "int"),
+        ("enumeration_max", "EnumerationMax", "int"),
         ("tensor_type", "TensorType", "str"),
         ("is_extensive", "IsExtensive", "bool"),
     ]
 
     @property
     def quantity_type(self) -> str:
         """Quantity type of the variable.
@@ -97,14 +100,15 @@
 
         Allowed values (FMU):
 
         - Real
         - Integer
         - Logical
         - String
+        - Enumeration
         - None"""
         return self.get_property_state("data_type")
 
     @data_type.setter
     def data_type(self, value: str):
         self.set_property_state("data_type", value)
 
@@ -141,14 +145,23 @@
         return self.get_property_state("string_initial_value")
 
     @string_initial_value.setter
     def string_initial_value(self, value: str):
         self.set_property_state("string_initial_value", value)
 
     @property
+    def enumeration_initial_value(self) -> int:
+        """Enumeration data start value."""
+        return self.get_property_state("enumeration_initial_value")
+
+    @enumeration_initial_value.setter
+    def enumeration_initial_value(self, value: int):
+        self.set_property_state("enumeration_initial_value", value)
+
+    @property
     def real_min(self) -> RealType:
         """Real data minimum value."""
         return self.get_property_state("real_min")
 
     @real_min.setter
     def real_min(self, value: RealType):
         self.set_property_state("real_min", value)
@@ -177,14 +190,32 @@
         return self.get_property_state("integer_max")
 
     @integer_max.setter
     def integer_max(self, value: int):
         self.set_property_state("integer_max", value)
 
     @property
+    def enumeration_min(self) -> int:
+        """Enumeration data minimum value."""
+        return self.get_property_state("enumeration_min")
+
+    @enumeration_min.setter
+    def enumeration_min(self, value: int):
+        self.set_property_state("enumeration_min", value)
+
+    @property
+    def enumeration_max(self) -> int:
+        """Enumeration data maximum value."""
+        return self.get_property_state("enumeration_max")
+
+    @enumeration_max.setter
+    def enumeration_max(self, value: int):
+        self.set_property_state("enumeration_max", value)
+
+    @property
     def tensor_type(self) -> str:
         """Indicates the variable tensor type (\"Scalar\" or \"Vector\").
 
         \"Vector\" is not supported for the FMU case."""
         return self.get_property_state("tensor_type")
 
     @tensor_type.setter
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/write_csv_chart_files.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/write_csv_chart_files.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/api_23_1/write_ensight.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/api_23_2/write_ensight.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/get_status_messages.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/get_status_messages.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/injected_commands.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/injected_commands.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/root_source.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/root_source.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/static_info.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/static_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from copy import deepcopy
 from typing import Tuple
 
 from ansys.systemcoupling.core.adaptor.impl.injected_commands import (
     get_injected_cmd_data,
 )
+from ansys.systemcoupling.core.syc_version import SYC_VERSION_DOT
 from ansys.systemcoupling.core.util.name_util import to_python_name
 
 
 def process_cmd_data(raw_data: list, category: str = None) -> dict:
     """Take the raw command and query metadata provided by System Coupling
         and manipulate it into a form that can be used by the data model
         generation functionality.
@@ -320,17 +321,17 @@
 
 def get_syc_version(api) -> str:
     """Get the System Coupling version.
 
     The version is returned in a string like ``"23.2"``.
 
     System Coupling versions earlier than 23.2 (2023 R2) do not expose
-    the ``GetVersion`` command. Because the server that PySystemCoupling
-    connects to did not exist prior to 23.1 (2023 R1), if no version query
-    exists, the version is assumed to be 23.1.
+    the ``GetVersion`` query. Because the first version of the server
+    that PySystemCoupling is able to connect to is 23.1 (2023 R1), the
+    version is assumed to be 23.1 if no version query exists.
 
     Parameters
     ----------
     api : NativeApi
         Object providing access to the System Coupling *native API* .
     """
 
@@ -345,8 +346,8 @@
                 pass
         raise RuntimeError(
             f"Version string {version_in} has invalid format (expect '20yy Rn')."
         )
 
     cmds = api.GetCommandAndQueryMetadata()
     exists = any(cmd["name"] == "GetVersion" for cmd in cmds)
-    return clean_version_string(api.GetVersion()) if exists else "23.1"
+    return clean_version_string(api.GetVersion()) if exists else SYC_VERSION_DOT
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy_interface.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy_interface.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/adaptor/impl/types.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/adaptor/impl/types.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/grpc_client.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/grpc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,36 +86,46 @@
         # For example, we might want to default to launching installation
         # locally but container on GitHub (for build tasks like code generation).
         # You could still switch to the container locally by setting the
         # environment variable.
 
         working_dir = kwargs.pop("working_dir", None)
         port = kwargs.pop("port", None)
+        version = kwargs.pop("version", None)
 
         if os.environ.get("SYC_LAUNCH_CONTAINER") == "1":
             mounted_from = working_dir if working_dir else "./"
             mounted_to = "/working"
-            self.start_container_and_connect(mounted_from, mounted_to, port=port)
+            self.start_container_and_connect(
+                mounted_from, mounted_to, port=port, version=version
+            )
         else:  # pragma: no cover
             if port is None:
                 port = _find_port()
             if working_dir is None:
                 working_dir = "."
             LOG.debug("Starting process...")
-            self.__process = SycProcess(_LOCALHOST_IP, port, working_dir, **kwargs)
+            self.__process = SycProcess(
+                _LOCALHOST_IP, port, working_dir, version, **kwargs
+            )
             LOG.debug("...started")
             self._connect(_LOCALHOST_IP, port)
 
     def start_container_and_connect(
-        self, mounted_from: str, mounted_to: str, network: str = None, port: int = None
+        self,
+        mounted_from: str,
+        mounted_to: str,
+        network: str = None,
+        port: int = None,
+        version: str = None,
     ):
         """Start the System Coupling container and establish a connection."""
         LOG.debug("Starting container...")
         port = port if port is not None else _find_port()
-        start_container(mounted_from, mounted_to, network, port)
+        start_container(mounted_from, mounted_to, network, port, version)
         LOG.debug("...started")
         self._connect(_LOCALHOST_IP, port)
 
     def connect(self, host, port):
         """Connect to an already running System Coupling server running on a known
         host and port.
         """
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/services/command_query.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/services/command_query.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/services/output_stream.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/services/output_stream.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/services/process.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/services/process.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/services/solution.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/services/solution.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/syc_process.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/syc_process.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from copy import deepcopy
 import os
 import platform
 import subprocess
 
 import psutil
 
+from ansys.systemcoupling.core.syc_version import SYC_VERSION_CONCAT, normalize_version
 from ansys.systemcoupling.core.util.logging import LOG
 
 _isWindows = any(platform.win32_ver())
 
-_CURR_VER = "231"
+_CURR_VER = SYC_VERSION_CONCAT
 _INSTALL_ROOT_ENV = "AWP_ROOT"
 _INSTALL_ROOT_VER_ENV = _INSTALL_ROOT_ENV + _CURR_VER
 _SC_ROOT_ENV = "SYSC_ROOT"
 
 _SCRIPT_EXT = ".bat" if _isWindows else ""
 _SCRIPT_NAME = "systemcoupling" + _SCRIPT_EXT
 
 # NB: Coverage disabled in this file as coverage is obtained in context of
 #     GitHub CI where we are restricted to launching SyC in container mode.
 
 
 class SycProcess:  # pragma: no cover
-    def __init__(self, host, port, working_dir, **kwargs):
-        self.__process = _start_system_coupling(host, port, working_dir, **kwargs)
+    def __init__(self, host, port, working_dir, version=None, **kwargs):
+        self.__process = _start_system_coupling(
+            host, port, working_dir, version, **kwargs
+        )
 
     def end(self):
         if self.__process and self.__process.poll() is None:
             pid = self.__process.pid
             try:
                 LOG.info("Waiting for process to exit...")
                 self.__process.wait(5)
@@ -37,19 +40,26 @@
                     "Process still alive - forcible kill of "
                     "process and children will be attempted."
                 )
                 _kill_process_tree(pid, timeout=0.5)
             self.__process = None
 
 
-def _start_system_coupling(host, port, working_dir, **kwargs):  # pragma: no cover
+def _start_system_coupling(
+    host, port, working_dir, version, **kwargs
+):  # pragma: no cover
     env = deepcopy(os.environ)
     env["PYTHONUNBUFFERED"] = "1"
     env["SYC_GUI_SILENT_SERVER"] = "1"
-    args = [_path_to_system_coupling(), "-m", "cosimgui", f"--grpcport={host}:{port}"]
+    args = [
+        _path_to_system_coupling(version),
+        "-m",
+        "cosimgui",
+        f"--grpcport={host}:{port}",
+    ]
 
     # Extract arguments that we currently recognize - scope to extend in future
     nprocs = kwargs.pop("nprocs", None)
     if nprocs:
         args += ["--nprocs", str(nprocs)]
 
     sycnprocs = kwargs.pop("sycnprocs", None)
@@ -68,21 +78,37 @@
         env=env,
         cwd=working_dir,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.STDOUT,
     )
 
 
-def _path_to_system_coupling():  # pragma: no cover
+def _path_to_system_coupling(version):  # pragma: no cover
+    if version is not None:
+        if os.environ.get(_SC_ROOT_ENV, None) or os.environ.get(
+            _INSTALL_ROOT_ENV, None
+        ):
+            raise ValueError(
+                f"An explicit version, {version}, has been specified for "
+                "launching System Coupling, while at least one of the "
+                f"environment variables {_SC_ROOT_ENV} and {_INSTALL_ROOT_ENV} "
+                "is set. To remove the ambiguity, either unset the environment "
+                "variable(s) or do not provide the version argument."
+            )
+
     scroot = os.environ.get(_SC_ROOT_ENV, None)
 
     if not scroot:
         scroot = os.environ.get(_INSTALL_ROOT_ENV, None)
         if scroot is None:
-            scroot = os.environ.get(_INSTALL_ROOT_VER_ENV, None)
+            if version is None:
+                scroot = os.environ.get(_INSTALL_ROOT_VER_ENV, None)
+            else:
+                ver_maj, ver_min = normalize_version(version)
+                scroot = os.environ.get(f"{_INSTALL_ROOT_ENV}{ver_maj}{ver_min}", None)
         if scroot:
             scroot = os.path.join(scroot, "SystemCoupling")
 
     if scroot is None:
         raise RuntimeError("Failed to locate System Coupling from environment.")
 
     script_path = os.path.join(scroot, "bin", _SCRIPT_NAME)
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/client/variant.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/client/variant.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/examples/downloads.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/examples/downloads.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 def _decompress(filename: str) -> None:
     zip_ref = zipfile.ZipFile(filename, "r")
     zip_ref.extractall(pysyc.EXAMPLES_PATH)
     return zip_ref.close()
 
 
 def _get_file_url(filename: str, directory: Optional[str] = None) -> str:
-    root_url = "https://github.com/pyansys/example-data/raw/master/"
-    # root_url = "https://github.com/pyansys/pysystem-coupling/raw/feature/more_doc/"
+    root_url = "https://github.com/ansys/example-data/raw/master/"
+    # root_url = "https://github.com/ansys/pysystem-coupling/raw/feature/more_doc/"
     if directory:
         return f"{root_url}" f"{directory}/{filename}"
     return f"{root_url}/{filename}"
 
 
 def _retrieve_file(url: str, filename: str):
     # First check if file has already been downloaded
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/native_api/command_metadata.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/native_api/command_metadata.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/native_api/datamodel_metadata.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/native_api/datamodel_metadata.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/native_api/native_api.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/native_api/native_api.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/native_api/object_path.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/native_api/object_path.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/session.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
     @property
     def _native_api(self) -> NativeApi:
         """Access to the *native* System Coupling API and data model.
 
         Use of this API is not particularly encouraged, but there may be
         situations where it is useful to access functionality that, for
-        some reason, not been fully exposed in PySystemCoupling.
+        some reason, has not been fully exposed in PySystemCoupling.
 
         Furthermore, existing users of the System Coupling CLI may initially
         find it comfortable to work with the familiar API while transitioning
         to using PySystemCoupling.
 
         This API is exposed dynamically on the client side and provides
         little runtime assistance and documentation.
```

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/util/logging.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/util/logging.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/util/pathstr.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/util/pathstr.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/util/state_keys.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/util/state_keys.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/src/ansys/systemcoupling/core/util/yaml_helper.py` & `ansys_systemcoupling_core-0.2.0/src/ansys/systemcoupling/core/util/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `ansys-systemcoupling-core-0.1.3/PKG-INFO` & `ansys_systemcoupling_core-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-systemcoupling-core
-Version: 0.1.3
+Version: 0.2.0
 Summary: A Python wrapper for Ansys System Coupling.
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -15,69 +15,68 @@
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: ansys-api-systemcoupling==0.1.0
 Requires-Dist: grpcio>=1.30.0
-Requires-Dist: grpcio-status>=1.30.0,<1.51.2
+Requires-Dist: grpcio-status>=1.30.0,<1.56.1
 Requires-Dist: googleapis-common-protos>=1.50.0
 Requires-Dist: protobuf>=3.20.1,<4.0.0
 Requires-Dist: psutil>=5.7.0
 Requires-Dist: pyyaml
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: importlib-metadata>=4.0
 Requires-Dist: build ; extra == "build"
-Requires-Dist: black==23.1.0 ; extra == "classesgen"
+Requires-Dist: black==23.7.0 ; extra == "classesgen"
 Requires-Dist: isort==5.12.0 ; extra == "classesgen"
-Requires-Dist: ansys-sphinx-theme==0.9.5 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.4.0 ; extra == "doc"
 Requires-Dist: matplotlib ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
-Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
+Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==1.22 ; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: sphinx-gallery==0.12.2 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==1.23.3 ; extra == "doc"
+Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
+Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.2.0 ; extra == "doc"
 Requires-Dist: ansys-fluent-core ; extra == "doc"
 Requires-Dist: ansys-dpf-core ; extra == "doc"
-Requires-Dist: codespell==2.2.4 ; extra == "style"
+Requires-Dist: codespell==2.2.5 ; extra == "style"
 Requires-Dist: flake8==6.0.0 ; extra == "style"
 Requires-Dist: pytest ; extra == "tests"
 Requires-Dist: pytest-cov ; extra == "tests"
 Requires-Dist: psutil>=5.7.0 ; extra == "tests"
 Project-URL: Documentation, https://systemcoupling.docs.pyansys.com/
-Project-URL: Homepage, https://github.com/pyansys/pysystem-coupling/
-Project-URL: Source, https://github.com/pyansys/pysystem-coupling/
-Project-URL: Tracker, https://github.com/pyansys/pysystem-coupling/issues
+Project-URL: Homepage, https://github.com/ansys/pysystem-coupling/
+Project-URL: Source, https://github.com/ansys/pysystem-coupling/
+Project-URL: Tracker, https://github.com/ansys/pysystem-coupling/issues
 Provides-Extra: build
 Provides-Extra: classesgen
 Provides-Extra: doc
 Provides-Extra: style
 Provides-Extra: tests
 
 PySystemCoupling
 ================
-.. TODO : add codecov badge once public
 
-|pyansys| |GH-CI| |MIT| |black|
+|pyansys| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
 
-.. |GH-CI| image:: https://github.com/pyansys/pysystem-coupling/actions/workflows/ci.yml/badge.svg
-   :target: https://github.com/pyansys/pysystem-coupling/actions/workflows/ci.yml
+.. |GH-CI| image:: https://github.com/ansys/pysystem-coupling/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/ansys/pysystem-coupling/actions/workflows/ci.yml
 
 .. |codecov| image:: https://codecov.io/gh/pysystem-coupling/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/pysystem-coupling
+   :target: https://codecov.io/gh/ansys/pysystem-coupling
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
   :target: https://github.com/psf/black
   :alt: black
@@ -105,47 +104,50 @@
 
 
 Alternatively, clone and install PySystemCoupling in *development mode*
 with this code:
 
 .. code::
 
-   git clone https://github.com/pyansys/pysystem-coupling.git
+   git clone https://github.com/ansys/pysystem-coupling.git
    cd pysystem-coupling
    python -m pip install --upgrade pip
    pip install -e .
    pip install .[classesgen]
    python scripts\generate_datamodel.py
 
 
 Documentation and Issues
 ------------------------
 
 For more information, see the `Documentation <https://systemcoupling.docs.pyansys.com>`_ page.
 
-Use the `PySystemCoupling Issues <https://github.com/pyansys/pysystem-coupling/issues>`_ page to
+Use the `PySystemCoupling Issues <https://github.com/ansys/pysystem-coupling/issues>`_ page to
 post bug reports, questions and feature requests.
 
 Usage
 -----
 
 It is assumed that an Ansys installation is available and that this installation
 includes System Coupling and the participant products needed for the coupled analysis.
 
 The System Coupling installation is found by examining the following environment variables
 in this order:
 
 * ``SYSC_ROOT``
 * ``AWP_ROOT``
-* ``AWP_ROOT231``
+* ``AWP_ROOT232``
 
 If a variable is set but does not refer to a valid installation, PySystemCoupling
-fail at that point, rather than attempting to use the next variable.
+fails at that point, rather than attempting to use the next variable.
 
-In a standard user installation, the expectation is that only ``AWP_ROOT231`` is set.
+In a standard user installation, the expectation is that only ``AWP_ROOT232`` is set.
+
+(It is also possible to provide a different version number as an argument to the ``launch()``
+function. This will affect which ``AWP_ROOT<version>`` environment variable is examined.)
 
 The System Coupling API is exposed to PySystemCoupling in two forms:
 
 * A documented interface based on concrete Python classes, following Pythonic conventions
 * A dynamic interface, undocumented in PySystemCoupling, that replicates the native System Coupling API
 
 Both forms are strongly related to each other. A key difference in the Pythonic API is that naming
```

