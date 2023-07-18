# Comparing `tmp/ci_cmg_mb_cruise_migration-1.1.tar.gz` & `tmp/ci_cmg_mb_cruise_migration-1.2.tar.gz`

## Comparing `ci_cmg_mb_cruise_migration-1.1.tar` & `ci_cmg_mb_cruise_migration-1.2.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/config.yaml
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/requirements.txt
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/run.sh
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/start_background.sh
--rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/stop_background.sh
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/.gitignore
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/pyvenv.cfg
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.csh
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.fish
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.ps1
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate_this.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/deactivate.nu
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/docutils
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/futurize
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/keyring
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/markdown-it
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/normalizer
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pasteurize
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pip
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pip3
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pip3.10
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pkginfo
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pygmentize
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pyproject-build
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/python -> /opt/homebrew/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/python3.10 -> python
--rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html.py
--rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html5.py
--rwxr-xr-x   0        0        0      836 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2latex.py
--rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2man.py
--rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2odt.py
--rwxr-xr-x   0        0        0     1763 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2s5.py
--rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2xml.py
--rwxr-xr-x   0        0        0      713 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/twine
--rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/virtualenv
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/wheel
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/wheel-3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/wheel3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/wheel3.10
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/clean_cruise.py
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/cleaner.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/migration_properties.py
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/migrator.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/start_migration.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/cruise_connection.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/cruise_db.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/mb_db.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/oracledb_pooled.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/query_builder.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/cache.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_decoder.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_filter.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_labeler.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_validator.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/paginator.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/parsed_data_file.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/survey_filter.py
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/const_initializer.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/data_file_consts.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/data_file_part_consts.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/dataset_type_consts.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/date_consts.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/error_consts.py
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/file_format_consts.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/file_label_consts.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/file_type_consts.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/instrument_consts.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/log_level_consts.py
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/parameter_detail_consts.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/platform_type_consts.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/survey_blacklist.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/version_consts.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/version_description_consts.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/dataset_type_resolver.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/file_format_resolver.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/file_type_resolver.py
--rw-r--r--   0        0        0    23209 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/instrument_resolver.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/platform_designator_resolver.py
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/version_description_resolver.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/batch_error.py
--rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_log.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_logger.py
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_report.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_access_path.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_dataset.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_dataset_types.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_file_formats.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_file_types.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_files.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_instruments.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_parameter.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_parameter_details.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_people_and_sources.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_platforms.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_projects.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_shape.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_surveys.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_version_descriptions.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/cruise_cargo.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/mb_cargo.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/migrating_survey.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/prefab.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/transfer.py
--rw-r--r--   0        0        0    15525 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_mbinfo_file_tsql.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_mbinfo_formats.py
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_ngdcid_and_file.py
--rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_survey.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_survey_reference.py
--rw-r--r--   0        0        0    20861 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/cruise_processor.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/mb_processor.py
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/prefab_factory.py
--rw-r--r--   0        0        0    37050 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/schema_mapper.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/transfer_station.py
--rw-r--r--   0        0        0    47113 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/services/cruise_service.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/services/mb_service.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/utility/common.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/utility/dataset.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/config_test.yaml
--rwxr-xr-x   0        0        0     1355 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/start-it.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/stop-it.sh
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_batch_insert.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cleaner.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_configurable_survey_query.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_const_initializer.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_designator_resolver.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_instrument_resolver.py
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_processor.py
--rw-r--r--   0        0        0    18004 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_service_crud.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_service_mappings.py
--rw-r--r--   0        0        0    20064 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_end_to_end_it.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_loggers.py
--rw-r--r--   0        0        0    16438 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_mb_filters.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_mb_paginator.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_mb_processor.py
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_mb_service.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_mb_survey_blacklist.py
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_provider_from_source.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_scratch.py
--rw-r--r--   0        0        0    36368 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_standard_mapping.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_survey_metadata_mapping.py
--rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/testutils.py
--rw-r--r--   0        0        0    53753 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/create_mb.sql
--rw-r--r--   0        0        0   213608 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/migrate_cruise.sql
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/setup-user.sql
--rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/setup_cruise.sh
--rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/setup_mb.sh
--rw-r--r--   0        0        0   683665 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1208.sql
--rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1208_lite.sql
--rw-r--r--   0        0        0   856973 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1570.sql
--rw-r--r--   0        0        0   584287 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW2176.sql
--rw-r--r--   0        0        0  2082204 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3020.sql
--rw-r--r--   0        0        0   688103 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3106.sql
--rw-r--r--   0        0        0   222391 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3206.sql
--rw-r--r--   0        0        0    48250 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3370.sql
--rw-r--r--   0        0        0    74691 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3403.sql
--rw-r--r--   0        0        0   828582 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3549.sql
--rw-r--r--   0        0        0   419998 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW523.sql
--rw-r--r--   0        0        0   352532 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/RR1808.sql
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/RR1808_lite.sql
--rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/test_blacklist.sql
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/LICENSE
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/README.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/pyproject.toml
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/PKG-INFO
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/config.yaml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/requirements.txt
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/run.sh
+-rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/start_background.sh
+-rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/stop_background.sh
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/.gitignore
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/pyvenv.cfg
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate.csh
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate.fish
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate.ps1
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate_this.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/docutils
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/futurize
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/keyring
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/markdown-it
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/normalizer
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/pasteurize
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/pip
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/pip3
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/pip3.10
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/pkginfo
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/pygmentize
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/pyproject-build
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/python -> /opt/homebrew/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/python3.10 -> python
+-rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2html.py
+-rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      836 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2man.py
+-rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2odt.py
+-rwxr-xr-x   0        0        0     1763 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      713 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/twine
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/virtualenv
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/wheel
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/wheel-3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/wheel3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/migenv/bin/wheel3.10
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/clean_cruise.py
+-rw-r--r--   0        0        0    15266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/cleaner.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/migration_properties.py
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/migrator.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/start_migration.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/db/cruise_connection.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/db/cruise_db.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/db/mb_db.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/db/oracledb_pooled.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/db/query_builder.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/cache.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/file_decoder.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/file_filter.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/file_labeler.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/file_validator.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/paginator.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/parsed_data_file.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/survey_filter.py
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/const_initializer.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/data_file_consts.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/data_file_part_consts.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/dataset_type_consts.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/date_consts.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/error_consts.py
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/file_format_consts.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/file_label_consts.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/file_type_consts.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/instrument_consts.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/log_level_consts.py
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/parameter_detail_consts.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/platform_type_consts.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/survey_blacklist.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/version_consts.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/version_description_consts.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/dataset_type_resolver.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/file_format_resolver.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/file_type_resolver.py
+-rw-r--r--   0        0        0    23578 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/instrument_resolver.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/platform_designator_resolver.py
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/version_description_resolver.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/logging/batch_error.py
+-rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/logging/migration_log.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/logging/migration_logger.py
+-rw-r--r--   0        0        0     8111 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/logging/migration_report.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_access_path.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_dataset.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_dataset_types.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_file_formats.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_file_types.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_files.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_instruments.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_parameter.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_parameter_details.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_people_and_sources.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_platforms.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_projects.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_shape.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_surveys.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_version_descriptions.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/intermediary/cruise_cargo.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/intermediary/mb_cargo.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/intermediary/migrating_survey.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/intermediary/prefab.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/intermediary/transfer.py
+-rw-r--r--   0        0        0    15525 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/mb/mb_mbinfo_file_tsql.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/mb/mb_mbinfo_formats.py
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/mb/mb_ngdcid_and_file.py
+-rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/mb/mb_survey.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/mb/mb_survey_reference.py
+-rw-r--r--   0        0        0    20861 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/processors/cruise_processor.py
+-rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/processors/mb_processor.py
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/processors/prefab_factory.py
+-rw-r--r--   0        0        0    37050 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/processors/schema_mapper.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/processors/transfer_station.py
+-rw-r--r--   0        0        0    47164 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/services/cruise_service.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/services/mb_service.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/utility/common.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/utility/dataset.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/config_test.yaml
+-rwxr-xr-x   0        0        0     1355 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/start-it.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/stop-it.sh
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_batch_insert.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_cleaner.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_configurable_survey_query.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_const_initializer.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_cruise_designator_resolver.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_cruise_instrument_resolver.py
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_cruise_processor.py
+-rw-r--r--   0        0        0    18004 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_cruise_service_crud.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_cruise_service_mappings.py
+-rw-r--r--   0        0        0    20064 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_end_to_end_it.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_loggers.py
+-rw-r--r--   0        0        0    16438 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_mb_filters.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_mb_paginator.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_mb_processor.py
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_mb_service.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_mb_survey_blacklist.py
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_provider_from_source.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_scratch.py
+-rw-r--r--   0        0        0    36368 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_standard_mapping.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/test_survey_metadata_mapping.py
+-rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/testutils.py
+-rw-r--r--   0        0        0    53753 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/create_mb.sql
+-rw-r--r--   0        0        0   213608 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/migrate_cruise.sql
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/setup-user.sql
+-rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/setup_cruise.sh
+-rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/setup_mb.sh
+-rw-r--r--   0        0        0   683665 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW1208.sql
+-rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW1208_lite.sql
+-rw-r--r--   0        0        0   856973 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW1570.sql
+-rw-r--r--   0        0        0   584287 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW2176.sql
+-rw-r--r--   0        0        0  2082204 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3020.sql
+-rw-r--r--   0        0        0   688103 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3106.sql
+-rw-r--r--   0        0        0   222391 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3206.sql
+-rw-r--r--   0        0        0    48250 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3370.sql
+-rw-r--r--   0        0        0    74691 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3403.sql
+-rw-r--r--   0        0        0   828582 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3549.sql
+-rw-r--r--   0        0        0   419998 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW523.sql
+-rw-r--r--   0        0        0   352532 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/RR1808.sql
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/RR1808_lite.sql
+-rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/test_blacklist.sql
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/LICENSE
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/pyproject.toml
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.2/PKG-INFO
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/config.yaml` & `ci_cmg_mb_cruise_migration-1.2/config.yaml`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.csh` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.fish` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.nu` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.ps1` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate_this.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html4.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html5.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2latex.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2man.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2odt.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2odt_prepstyles.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2pseudoxml.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2s5.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2xetex.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2xml.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rstpep2html.py` & `ci_cmg_mb_cruise_migration-1.2/migenv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/cleaner.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/cleaner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import datetime
 
 from src.mb_cruise_migration.db.cruise_connection import CruiseConnection
 from src.mb_cruise_migration.logging.migration_log import MigrationLog
-from src.mb_cruise_migration.logging.migration_report import MigrationReport
 from src.mb_cruise_migration.migration_properties import MigrationProperties
 
 
 class Cleaner(object):
+    start = None
+
     def __init__(self, config_file):
+        Cleaner.start = datetime.datetime.now()
         MigrationProperties(config_file)
         MigrationLog()
-        MigrationReport()
         self.cruise = CruiseConnection()
 
     def delete_multibeam_data_from_cruise(self):
-        MigrationReport.start = datetime.datetime.now()
+        self.__log_start()
 
         self.__delete_file_shapes()
         self.__delete_file_access_paths()
         self.__delete_file_parameters()
         self.__delete_files()
         self.__delete_dataset_shapes()
         self.__delete_dataset_surveys()
@@ -28,16 +29,15 @@
         self.__delete_dataset_platforms()
         self.__delete_dataset_instruments()
         self.__delete_dataset_parameters()
         self.__delete_datasets()
         self.__delete_unreferenced_shapes()
         self.__delete_unreferenced_access_paths()
 
-        MigrationReport.end = datetime.datetime.now()
-        MigrationReport.clean_final_report()
+        self.__log_end()
 
     def __delete_file_shapes(self):
         MigrationLog.log.info("START -- DELETING FILE SHAPES")
         command = "DELETE FROM CRUISE.FILE_SHAPES WHERE FILE_ID IN (SELECT FILE_ID FROM CRUISE.FILES all_files WHERE all_files.DATASET_ID IN (SELECT DATASET_ID FROM CRUISE.DATASETS WHERE DATASET_TYPE_ID IN (SELECT TYPE_ID FROM CRUISE.DATASET_TYPES WHERE TYPE_NAME = 'MB RAW' OR TYPE_NAME = 'MB PROCESSED' OR TYPE_NAME = 'MB PRODUCT' OR TYPE_NAME = 'MB RAW NONPUBLIC' OR TYPE_NAME = 'MB PROCESSED NONPUBLIC' OR TYPE_NAME = 'MB PRODUCT NONPUBLIC' OR TYPE_NAME = 'ANCILLARY' OR TYPE_NAME = 'DOCUMENT' OR TYPE_NAME = 'METADATA' OR TYPE_NAME = 'ANCILLARY NONPUBLIC' OR TYPE_NAME = 'DOCUMENT NONPUBLIC' OR TYPE_NAME = 'METADATA NONPUBLIC')))"
         self.cruise.execute(command)
         MigrationLog.log.info("END -- DELETING FILE SHAPES")
 
@@ -48,24 +48,42 @@
         MigrationLog.log.info("END -- DELETING FILE ACCESS PATHS")
 
     def __delete_file_parameters(self):
         MigrationLog.log.info("START -- DELETING FILE PARAMETERS")
         count_query = "SELECT COUNT(*) FROM CRUISE.FILE_PARAMETERS WHERE FILE_ID IN (SELECT FILE_ID FROM CRUISE.FILES all_files WHERE all_files.DATASET_ID IN (SELECT DATASET_ID FROM CRUISE.DATASETS WHERE DATASET_TYPE_ID IN (SELECT TYPE_ID FROM CRUISE.DATASET_TYPES WHERE TYPE_NAME = 'MB RAW' OR TYPE_NAME = 'MB PROCESSED' OR TYPE_NAME = 'MB PRODUCT' OR TYPE_NAME = 'MB RAW NONPUBLIC' OR TYPE_NAME = 'MB PROCESSED NONPUBLIC' OR TYPE_NAME = 'MB PRODUCT NONPUBLIC' OR TYPE_NAME = 'ANCILLARY' OR TYPE_NAME = 'DOCUMENT' OR TYPE_NAME = 'METADATA' OR TYPE_NAME = 'ANCILLARY NONPUBLIC' OR TYPE_NAME = 'DOCUMENT NONPUBLIC' OR TYPE_NAME = 'METADATA NONPUBLIC')))"
         fp_count = list(self.cruise.query(count_query))[0]
         while fp_count > 0:
-            MigrationLog.log.info("...deleting block")
-            delete_command = "DELETE FROM CRUISE.FILE_PARAMETERS WHERE FILE_PARAMETER_ID IN (SELECT FILE_PARAMETER_ID FROM CRUISE.FILE_PARAMETERS WHERE FILE_ID IN (SELECT FILE_ID FROM CRUISE.FILES all_files WHERE all_files.DATASET_ID IN (SELECT DATASET_ID FROM CRUISE.DATASETS WHERE DATASET_TYPE_ID IN (SELECT TYPE_ID FROM CRUISE.DATASET_TYPES WHERE TYPE_NAME = 'MB RAW' OR TYPE_NAME = 'MB PROCESSED' OR TYPE_NAME = 'MB PRODUCT' OR TYPE_NAME = 'MB RAW NONPUBLIC' OR TYPE_NAME = 'MB PROCESSED NONPUBLIC' OR TYPE_NAME = 'MB PRODUCT NONPUBLIC' OR TYPE_NAME = 'ANCILLARY' OR TYPE_NAME = 'DOCUMENT' OR TYPE_NAME = 'METADATA' OR TYPE_NAME = 'ANCILLARY NONPUBLIC' OR TYPE_NAME = 'DOCUMENT NONPUBLIC' OR TYPE_NAME = 'METADATA NONPUBLIC'))) FETCH FIRST 1000000 ROWS ONLY)"
+            MigrationLog.log.info("...deleting block of 1,000,000")
+            delete_command = "DELETE FROM CRUISE.FILE_PARAMETERS WHERE FILE_PARAMETER_ID IN " \
+                             "(SELECT FILE_PARAMETER_ID FROM CRUISE.FILE_PARAMETERS WHERE FILE_ID IN " \
+                             "(SELECT FILE_ID FROM CRUISE.FILES all_files WHERE all_files.DATASET_ID IN " \
+                             "(SELECT DATASET_ID FROM CRUISE.DATASETS WHERE DATASET_TYPE_ID IN " \
+                             "(SELECT TYPE_ID FROM CRUISE.DATASET_TYPES WHERE TYPE_NAME = 'MB RAW' OR TYPE_NAME = 'MB PROCESSED' OR TYPE_NAME = 'MB PRODUCT' OR TYPE_NAME = 'MB RAW NONPUBLIC' OR TYPE_NAME = 'MB PROCESSED NONPUBLIC' OR TYPE_NAME = 'MB PRODUCT NONPUBLIC' OR TYPE_NAME = 'ANCILLARY' OR TYPE_NAME = 'DOCUMENT' OR TYPE_NAME = 'METADATA' OR TYPE_NAME = 'ANCILLARY NONPUBLIC' OR TYPE_NAME = 'DOCUMENT NONPUBLIC' OR TYPE_NAME = 'METADATA NONPUBLIC'" \
+                             ")" \
+                             ")" \
+                             ")" \
+                             " FETCH FIRST 1000000 ROWS ONLY" \
+                             ")"
             self.cruise.execute(delete_command)
             fp_count = list(self.cruise.query(count_query))[0]
         MigrationLog.log.info("END -- DELETING FILE PARAMETERS")
 
     def __delete_files(self):
         MigrationLog.log.info("START -- DELETING FILES")
-        command = "DELETE FROM CRUISE.FILES all_files WHERE all_files.DATASET_ID IN (SELECT DATASET_ID FROM CRUISE.DATASETS WHERE DATASET_TYPE_ID IN (SELECT TYPE_ID FROM CRUISE.DATASET_TYPES WHERE TYPE_NAME = 'MB RAW' OR TYPE_NAME = 'MB PROCESSED' OR TYPE_NAME = 'MB PRODUCT' OR TYPE_NAME = 'MB RAW NONPUBLIC' OR TYPE_NAME = 'MB PROCESSED NONPUBLIC' OR TYPE_NAME = 'MB PRODUCT NONPUBLIC' OR TYPE_NAME = 'ANCILLARY' OR TYPE_NAME = 'DOCUMENT' OR TYPE_NAME = 'METADATA' OR TYPE_NAME = 'ANCILLARY NONPUBLIC' OR TYPE_NAME = 'DOCUMENT NONPUBLIC' OR TYPE_NAME = 'METADATA NONPUBLIC'))"
-        self.cruise.execute(command)
+        count_query = "SELECT COUNT(*) FROM CRUISE.FILES all_files WHERE all_files.DATASET_ID IN (SELECT DATASET_ID FROM CRUISE.DATASETS WHERE DATASET_TYPE_ID IN (SELECT TYPE_ID FROM CRUISE.DATASET_TYPES WHERE TYPE_NAME = 'MB RAW' OR TYPE_NAME = 'MB PROCESSED' OR TYPE_NAME = 'MB PRODUCT' OR TYPE_NAME = 'MB RAW NONPUBLIC' OR TYPE_NAME = 'MB PROCESSED NONPUBLIC' OR TYPE_NAME = 'MB PRODUCT NONPUBLIC' OR TYPE_NAME = 'ANCILLARY' OR TYPE_NAME = 'DOCUMENT' OR TYPE_NAME = 'METADATA' OR TYPE_NAME = 'ANCILLARY NONPUBLIC' OR TYPE_NAME = 'DOCUMENT NONPUBLIC' OR TYPE_NAME = 'METADATA NONPUBLIC'))"
+        total = list(self.cruise.query(count_query))[0]
+        fp_count = total
+        deleted_count = 0
+        while fp_count > 0:
+            MigrationLog.log.info("...deleting block of 50,000")
+            delete_command = "DELETE FROM CRUISE.FILES all_files WHERE all_files.FILE_ID IN (SELECT FILE_ID FROM CRUISE.FILES some_files WHERE some_files.DATASET_ID IN (SELECT DATASET_ID FROM CRUISE.DATASETS WHERE DATASET_TYPE_ID IN (SELECT TYPE_ID FROM CRUISE.DATASET_TYPES WHERE TYPE_NAME = 'MB RAW' OR TYPE_NAME = 'MB PROCESSED' OR TYPE_NAME = 'MB PRODUCT' OR TYPE_NAME = 'MB RAW NONPUBLIC' OR TYPE_NAME = 'MB PROCESSED NONPUBLIC' OR TYPE_NAME = 'MB PRODUCT NONPUBLIC' OR TYPE_NAME = 'ANCILLARY' OR TYPE_NAME = 'DOCUMENT' OR TYPE_NAME = 'METADATA' OR TYPE_NAME = 'ANCILLARY NONPUBLIC' OR TYPE_NAME = 'DOCUMENT NONPUBLIC' OR TYPE_NAME = 'METADATA NONPUBLIC')) FETCH FIRST 50000 ROWS ONLY)"
+            self.cruise.execute(delete_command)
+            fp_count = list(self.cruise.query(count_query))[0]
+            deleted_count += 50000
+            MigrationLog.log.info(f"{int(deleted_count / total)}% -- {deleted_count} deleted, {fp_count} left.")
         MigrationLog.log.info("END -- DELETING FILES")
 
     def __delete_dataset_shapes(self):
         MigrationLog.log.info("START -- DELETING DATASET SHAPES")
         command = "DELETE FROM CRUISE.DATASET_SHAPES WHERE DATASET_ID IN (SELECT DATASET_ID FROM CRUISE.DATASETS WHERE DATASET_TYPE_ID IN (SELECT TYPE_ID FROM CRUISE.DATASET_TYPES WHERE TYPE_NAME = 'MB RAW' OR TYPE_NAME = 'MB PROCESSED' OR TYPE_NAME = 'MB PRODUCT' OR TYPE_NAME = 'MB RAW NONPUBLIC' OR TYPE_NAME = 'MB PROCESSED NONPUBLIC' OR TYPE_NAME = 'MB PRODUCT NONPUBLIC' OR TYPE_NAME = 'ANCILLARY' OR TYPE_NAME = 'DOCUMENT' OR TYPE_NAME = 'METADATA' OR TYPE_NAME = 'ANCILLARY NONPUBLIC' OR TYPE_NAME = 'DOCUMENT NONPUBLIC' OR TYPE_NAME = 'METADATA NONPUBLIC'))"
         self.cruise.execute(command)
         MigrationLog.log.info("END -- DELETING DATASET SHAPES")
@@ -125,7 +143,21 @@
         MigrationLog.log.info("END -- DELETING UNREFERENCED SHAPES")
 
     def __delete_unreferenced_access_paths(self):
         MigrationLog.log.info("START -- DELETING UNREFERENCED ACCESS PATHS")
         command = "DELETE FROM (SELECT * FROM CRUISE.ACCESS_PATHS WHERE PATH_ID NOT IN (SELECT DISTINCT PATH_ID FROM CRUISE.FILE_ACCESS_PATHS))"
         self.cruise.execute(command)
         MigrationLog.log.info("END -- DELETING UNREFERENCED ACCESS PATHS")
+
+    @staticmethod
+    def __log_start():
+        MigrationLog.log.info(f"DELETING ALL MB SPECIFIC DATA FROM CRUISE -- {Cleaner.start}")
+        MigrationLog.log.info(f"\r")
+
+    @staticmethod
+    def __log_end():
+        end = datetime.datetime.now()
+        total_time = (end - Cleaner.start).total_seconds() / 60
+
+        MigrationLog.log.info(f"DELETION OF MULTIBEAM DATA COMPLETED")
+        MigrationLog.log.info(f'Elapsed time in minutes: {total_time}')
+        MigrationLog.log.info(f"\r")
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/migration_properties.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/migration_properties.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/migrator.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/migrator.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/cruise_connection.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/db/cruise_connection.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/cruise_db.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/db/cruise_db.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/mb_db.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/db/mb_db.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/oracledb_pooled.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/db/oracledb_pooled.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/query_builder.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/db/query_builder.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/cache.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/cache.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_decoder.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/file_decoder.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_filter.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/file_filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,24 +40,33 @@
         if parsed_file.is_canadian_data():
             MigrationLog.log_skipped_file(file)
             return True
 
         return False
 
     @classmethod
-    def __is_being_migrated(cls, file: MbFile):
+    def __is_being_migrated(cls, file: MbFile) -> bool:
+
+        migrate: bool = False
         parsed_file = file.parsed_file
         if parsed_file.is_survey_metadata():
-            return MigrationProperties.migrate.survey_metadata
+            return cls.__to_filter_or_not_to_filter(file, MigrationProperties.migrate.survey_metadata, "survey_metadata")
         if parsed_file.has_extraneous():
-            return MigrationProperties.migrate.extraneous
+            return cls.__to_filter_or_not_to_filter(file, MigrationProperties.migrate.extraneous, "extraneous")
         if parsed_file.has_leg():
-            return MigrationProperties.migrate.legs
+            return cls.__to_filter_or_not_to_filter(file, MigrationProperties.migrate.legs, "legs")
         if parsed_file.has_zone():
-            return MigrationProperties.migrate.zones
+            return cls.__to_filter_or_not_to_filter(file, MigrationProperties.migrate.zones, "zone")
         if parsed_file.has_region():
-            return MigrationProperties.migrate.regions
+            return cls.__to_filter_or_not_to_filter(file, MigrationProperties.migrate.regions, "region")
         if parsed_file.is_standard():
-            return MigrationProperties.migrate.standard
+            return cls.__to_filter_or_not_to_filter(file, MigrationProperties.migrate.standard, "standard")
 
         MigrationLog.log_no_file_category_error(file)
-        raise ValueError(f"no valid file category identified for file {file.data_file} with ngdc_id {file.ngdc_id}")
+        return migrate
+
+    @staticmethod
+    def __to_filter_or_not_to_filter(file: MbFile, config: bool, category: str):
+        if not config:
+            MigrationLog.log_filtered_file(file, category)
+        return config
+
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_labeler.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/file_labeler.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_validator.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/file_validator.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/paginator.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/paginator.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/parsed_data_file.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/parsed_data_file.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/survey_filter.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/survey_filter.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/const_initializer.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/const_initializer.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/data_file_consts.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/data_file_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/data_file_part_consts.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/data_file_part_consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         "me70",
         "8125",
         "em710",
         "sea_swathplus",
         "sb2120",
         "em304",
         "em2040",
+        "em2040p"
         "em712",
         "sb2112",
         "em3002",
         "em3002d",
         "EM3000",
         "2112",
         "reson7125_400",
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/dataset_type_consts.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/dataset_type_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/error_consts.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/error_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/file_format_consts.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/file_format_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/instrument_consts.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/instrument_consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     HOLLMINGECHOS625 = "HOLLMINGECHOS625"
     ATLASHYDROSWEEPDS = "ATLASHYDROSWEEPDS"
     RESONSEABAT9001 = "RESONSEABAT9001"
     SEABEAM2100 = "SEABEAM2100"
     RESONSEABAT8150 = "RESONSEABAT8150"
     MR1 = "MR1"
     KONGSBERGEM2040 = "KONGSBERGEM2040"
+    KONGSBERGEM2040P = "KONGSBERGEM2040P"
     RESONSEABAT7101 = "RESONSEABAT7101"
     RESONSEABATT20P = "RESONSEABATT20P"
     KONGSBERGEM120 = "KONGSBERGEM120"
     R2SONIC2024 = "R2SONIC2024"
     KONGSBERGEM304 = "KONGSBERGEM304"
     SEABEAM2112 = "SEABEAM2112"
     ATLASHYDROSWEEPDS2 = "ATLASHYDROSWEEPDS2"
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/parameter_detail_consts.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/parameter_detail_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/platform_type_consts.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/consts/platform_type_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/dataset_type_resolver.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/dataset_type_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/file_format_resolver.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/file_format_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/file_type_resolver.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/file_type_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/instrument_resolver.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/instrument_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,16 @@
             return InstrumentConsts.SEABEAM2120
         if data_file_inst == "7101":
             return InstrumentConsts.RESONSEABAT7101
         if data_file_inst == "em304":
             return InstrumentConsts.KONGSBERGEM304
         if data_file_inst == "em2040":
             return InstrumentConsts.KONGSBERGEM2040
+        if data_file_inst == "em2040p":
+            return  InstrumentConsts.KONGSBERGEM2040P
         if data_file_inst == "r2sonic2024":
             return InstrumentConsts.R2SONIC2024
 
     @staticmethod
     def get_const_from_mb_survey_instrument(survey_instrument):
         if survey_instrument is None:
             raise ValueError(ErrorConsts.NONE_VALUE_PROVIDED_WHERE_DISALLOWED)
@@ -189,14 +191,16 @@
             return InstrumentConsts.SEABEAM2100
         if survey_instrument == "Reson SeaBat 8150":
             return InstrumentConsts.RESONSEABAT8150
         if survey_instrument == "MR1":
             return InstrumentConsts.MR1
         if survey_instrument == "Kongsberg EM2040":
             return InstrumentConsts.KONGSBERGEM2040
+        if survey_instrument == "Kongsberg EM2040p":
+            return InstrumentConsts.KONGSBERGEM2040P
         if survey_instrument == "Reson SeaBat 7101":
             return InstrumentConsts.RESONSEABAT7101
         if survey_instrument == "Reson SeaBat T20-P":
             return InstrumentConsts.RESONSEABATT20P
         if survey_instrument == "Kongsberg EM120":
             return InstrumentConsts.KONGSBERGEM120
         if survey_instrument == "R2Sonic 2024":
@@ -329,14 +333,16 @@
             return CruiseInstrument(instrument_name="SB2100", docucomp_uuid=None, long_name="SeaBeam 2100")
         if const == InstrumentConsts.RESONSEABAT8150:
             return CruiseInstrument(instrument_name="SB8150", docucomp_uuid=None, long_name="Reson SeaBat 8150")
         if const == InstrumentConsts.MR1:
             return CruiseInstrument(instrument_name="MR1", docucomp_uuid=None, long_name="MR1")
         if const == InstrumentConsts.KONGSBERGEM2040:
             return CruiseInstrument(instrument_name="EM2040", docucomp_uuid=None, long_name="Kongsberg EM2040")
+        if const == InstrumentConsts.KONGSBERGEM2040P:
+            return CruiseInstrument(instrument_name="EM2040P", docucomp_uuid=None, long_name="Kongsberg EM2040P")
         if const == InstrumentConsts.RESONSEABAT7101:
             return CruiseInstrument(instrument_name="SB7101", docucomp_uuid=None, long_name="Reson SeaBat 7101")
         if const == InstrumentConsts.RESONSEABATT20P:
             return CruiseInstrument(instrument_name="SBT20-P", docucomp_uuid=None, long_name="Reson SeaBat T20-P")
         if const == InstrumentConsts.KONGSBERGEM120:
             return CruiseInstrument(instrument_name="EM120", docucomp_uuid=None, long_name="Kongsberg EM120")
         if const == InstrumentConsts.R2SONIC2024:
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/platform_designator_resolver.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/platform_designator_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/version_description_resolver.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/framework/resolvers/version_description_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_log.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/logging/migration_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 class MigrationLog(object):
     log: logging.Logger = None
     review: logging.Logger = None
 
     def __init__(self):
         self.__pre_check()
         self.__initialize_log()
+        self.__initialize_file_info()
         self.__initialize_review()
 
     def __initialize_log(self):
         keyword = "migration_log"
 
         level = MigrationProperties.log_config.level
         log_size_mb = MigrationProperties.log_config.log_size_mb
@@ -99,14 +100,18 @@
         MigrationLog.log.info(f"{LogConsts.END} -- Migration end at {datetime.datetime.now()}")
 
     @staticmethod
     def log_skipped_file(file: MbFile):
         MigrationLog.log.debug(f"{LogConsts.SKIP} -- File: skipping migration of file {file.data_file} with ngdc_id {file.ngdc_id}")
 
     @staticmethod
+    def log_filtered_file(file: MbFile, category: str):
+        MigrationLog.log.debug(f"{LogConsts.SKIP} -- File: removing file {file.data_file} with ngdc_id {file.ngdc_id} from migration: not configured to migrate files in category {category}")
+
+    @staticmethod
     def log_invalidated_file(file: MbFileCrate, reason: str):
         filename = file.mb_file.data_file
         MigrationLog.review.warning(f"{LogConsts.REVIEW} -- File migration skipped for {filename} due to: \n {reason}")
 
     @staticmethod
     def log_file_for_manual_review(mb_file_crate: MbFileCrate, instrument: str):
         file = mb_file_crate.mb_file.data_file
@@ -210,21 +215,21 @@
 
     @staticmethod
     def log_exception(exception):
         MigrationLog.log.exception(exception)
 
     @staticmethod
     def log_no_raw_processed_product(survey):
-        MigrationLog.log.warning(f"No raw, processed, or product dataset found for survey {survey}. Survey will not be migrated.")
+        MigrationLog.log.warning(f"{LogConsts.SKIP} -- Survey: No raw, processed, or product dataset found for survey {survey}. Survey will not be migrated.")
 
     @staticmethod
     def log_no_file_label_error(mb_file: MbFile):
         MigrationLog.log.error(f"no valid file label identified for file {mb_file.data_file} with ngdc_id {mb_file.ngdc_id}")
 
     @staticmethod
     def log_no_file_category_error(mb_file: MbFile):
-        MigrationLog.log.error(f"no valid file category identified for file {mb_file.data_file} with ngdc_id {mb_file.ngdc_id}")
+        MigrationLog.log.error(f"{LogConsts.ERROR} -- File: no valid file category identified for file {mb_file.data_file} with ngdc_id {mb_file.ngdc_id}. Survey will be skipped.")
 
     @staticmethod
     def log_paged_surveys(surveys: [MbSurvey]):
         survey_names = [survey.survey_name for survey in surveys]
         MigrationLog.log.info("Surveys paged: " + ", ".join(survey_names))
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_logger.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/logging/migration_logger.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_report.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/logging/migration_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,23 +197,14 @@
 
         logger.info(f"Failed surveys (migration was attempted, but an error occurred):")
         for survey in MigrationReport.failed_surveys:
             # logger.info(f"\t{survey.survey_name};\r{survey.error_message}\r")
             logger.info(f"\t{survey.survey_name}")
 
     @staticmethod
-    def clean_final_report():
-        logger = MigrationReport.report
-        total_time = (MigrationReport.end - MigrationReport.start).total_seconds() / 60
-
-        logger.info(f"DELETION OF MULTIBEAM DATA COMPLETED")
-        logger.info(f'Elapsed time in minutes: {total_time}')
-        logger.info(f"\r")
-
-    @staticmethod
     def get_successful_surveys_without_problems():
         successful = MigrationReport.migrated_surveys
         problems = MigrationReport.problem_surveys
         problems = [problem.survey_name for problem in problems]
         if problems and successful:
             successful = [survey for survey in successful if survey not in problems]
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_access_path.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_access_path.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_dataset.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_dataset.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_files.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_files.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_parameter.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_parameter.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_people_and_sources.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_people_and_sources.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_surveys.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/cruise/cruise_surveys.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/cruise_cargo.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/intermediary/cruise_cargo.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/mb_cargo.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/intermediary/mb_cargo.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/migrating_survey.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/intermediary/migrating_survey.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/prefab.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/intermediary/prefab.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/transfer.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/intermediary/transfer.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_mbinfo_file_tsql.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/mb/mb_mbinfo_file_tsql.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_ngdcid_and_file.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/mb/mb_ngdcid_and_file.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_survey.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/mb/mb_survey.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_survey_reference.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/models/mb/mb_survey_reference.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/cruise_processor.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/processors/cruise_processor.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/mb_processor.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/processors/mb_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         if not files:
             self.__skip_survey(survey.survey_name, "no associated files found for survey in mb schema.")
             return None
 
         files = FileFilter.filter_invalid_files(files)
         files, files_filtered = FileFilter.filter_files_not_configured_for_migration(files)
         if files_filtered > 0:  # cancel survey migration if any files are filtered.
-            self.__skip_survey(survey.survey_name, f"at least {files_filtered} files were filtered due to being marked for non-migration in config.")
+            self.__skip_survey(survey.survey_name, f"at least {files_filtered} files were filtered, causing the survey to be skipped.")
             return None
 
         files = FileLabeler.label(files)
         file_crates = [self.build_file_crate(file) for file in files]
         file_crates = FileDecoder.decode(file_crates)
 
         file_crates_validated, files_invalidated = FileValidator.validate(file_crates, survey.instrument)
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/prefab_factory.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/processors/prefab_factory.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/schema_mapper.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/processors/schema_mapper.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/transfer_station.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/processors/transfer_station.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/services/cruise_service.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/services/cruise_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,15 @@
             parent=model.parent,
             platform_name=model.platform_name,
             start_date=oracle_date_format(model.start_date, "cruise.survey.start_date"),
             end_date=oracle_date_format(model.end_date, "cruise.survey.end_date"),
             departure_port=model.departure_port,
             arrival_port=model.arrival_port,
             last_update=oracle_date_format(model.last_update, "cruise.survey.last_update"),
-            creation_date=model.creation_date
+            creation_date=oracle_date_format(model.creation_date, "cruise.survey.creation_date")
         )
 
     @staticmethod
     def from_entity(entity: Survey) -> CruiseSurvey:
         return CruiseSurvey(
             id=entity.id,
             survey_name=entity.name,
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/services/mb_service.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/services/mb_service.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/utility/common.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/utility/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 
     date_field_type = type(date_field_value)
 
     if date_field_type == str:
         try:
             date = datetime.datetime.strptime(date_field_value, ORACLE_DATE_FORMAT)
         except ValueError:
-            try:
-                date = datetime.datetime.fromisoformat(date_field_value)
-            except ValueError:
-                raise ValueError("Date " + date_field_value + " did not match expected format " + ORACLE_DATE_FORMAT + " for field " + date_field_name)
+            raise ValueError("Date " + date_field_value + " did not match expected format " + ORACLE_DATE_FORMAT + " for field " + date_field_name)
+            # try:
+            #   date = datetime.datetime.fromisoformat(date_field_value)
+            # except ValueError:
+            #   raise ValueError("Date " + date_field_value + " did not match expected format " + ORACLE_DATE_FORMAT + " for field " + date_field_name)
 
         return date.strftime(date_format_out).upper()
 
     if date_field_type == datetime or date_field_type == datetime.datetime:
         return date_field_value.strftime(date_format_out)
 
     raise ValueError("date field " + date_field_name + " contained unsupported type: " + str(type(date_field_value)))
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/utility/dataset.py` & `ci_cmg_mb_cruise_migration-1.2/src/mb_cruise_migration/utility/dataset.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/config_test.yaml` & `ci_cmg_mb_cruise_migration-1.2/tests/config_test.yaml`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/start-it.sh` & `ci_cmg_mb_cruise_migration-1.2/tests/start-it.sh`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_batch_insert.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_batch_insert.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_cleaner.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_cleaner.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_configurable_survey_query.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_configurable_survey_query.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_const_initializer.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_const_initializer.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_designator_resolver.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_cruise_designator_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_instrument_resolver.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_cruise_instrument_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_processor.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_cruise_processor.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_service_crud.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_cruise_service_crud.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_end_to_end_it.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_end_to_end_it.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_loggers.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_loggers.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_mb_filters.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_mb_filters.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_mb_paginator.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_mb_paginator.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_mb_processor.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_mb_processor.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_mb_service.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_mb_service.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_mb_survey_blacklist.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_mb_survey_blacklist.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_provider_from_source.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_provider_from_source.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_scratch.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_standard_mapping.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_standard_mapping.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/test_survey_metadata_mapping.py` & `ci_cmg_mb_cruise_migration-1.2/tests/test_survey_metadata_mapping.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/testutils.py` & `ci_cmg_mb_cruise_migration-1.2/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/create_mb.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/create_mb.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/migrate_cruise.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/migrate_cruise.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1208.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW1208.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1208_lite.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW1208_lite.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1570.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW1570.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW2176.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW2176.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3020.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3020.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3106.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3106.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3206.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3206.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3370.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3370.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3403.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3403.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3549.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW3549.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW523.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/NEW523.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/RR1808.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/RR1808.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/RR1808_lite.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/RR1808_lite.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/test_blacklist.sql` & `ci_cmg_mb_cruise_migration-1.2/tests/setup-files/test_data/test_blacklist.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/.gitignore` & `ci_cmg_mb_cruise_migration-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/LICENSE` & `ci_cmg_mb_cruise_migration-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/README.md` & `ci_cmg_mb_cruise_migration-1.2/README.md`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.1/pyproject.toml` & `ci_cmg_mb_cruise_migration-1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "oracledb", "pyyaml", "ci-cmg-cruise-schema-orm"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ci-cmg-mb-cruise-migration"
-version = "1.1"
+version = "1.2"
 description = "migrates multibeam metadata from mb schema to cruise schema"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `ci_cmg_mb_cruise_migration-1.1/PKG-INFO` & `ci_cmg_mb_cruise_migration-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ci-cmg-mb-cruise-migration
-Version: 1.1
+Version: 1.2
 Summary: migrates multibeam metadata from mb schema to cruise schema
 Project-URL: Github, https://github.com/CI-CMG/mb-cruise-migration
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

