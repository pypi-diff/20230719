# Comparing `tmp/OpenFisca-France-Data-1.2.0.tar.gz` & `tmp/OpenFisca-France-Data-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-France-Data-1.2.0.tar", last modified: Fri Jun 30 14:24:02 2023, max compression
+gzip compressed data, was "OpenFisca-France-Data-1.3.0.tar", last modified: Wed Jul 19 09:52:08 2023, max compression
```

## Comparing `OpenFisca-France-Data-1.2.0.tar` & `OpenFisca-France-Data-1.3.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.681681 OpenFisca-France-Data-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)    10720 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.661681 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4093 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-06-30 14:24:02.000000 OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-06-30 14:24:02.681681 OpenFisca-France-Data-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.661681 OpenFisca-France-Data-1.2.0/openfisca_france_data/
--rw-r--r--   0 runner    (1001) docker     (122)     7682 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4356 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.665681 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.665681 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.665681 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/
--rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/base_survey.py
--rw-r--r--   0 runner    (1001) docker     (122)    21046 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/common.py
--rw-r--r--   0 runner    (1001) docker     (122)    23193 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/comparator.py
--rw-r--r--   0 runner    (1001) docker     (122)      996 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.657681 OpenFisca-France-Data-1.2.0/openfisca_france_data/dads/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.665681 OpenFisca-France-Data-1.2.0/openfisca_france_data/dads/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/dads/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.665681 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/
--rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.669681 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/run_all.py
--rw-r--r--   0 runner    (1001) docker     (122)     8932 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (122)    21783 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11919 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
--rw-r--r--   0 runner    (1001) docker     (122)    26165 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (122)    13995 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
--rw-r--r--   0 runner    (1001) docker     (122)    36615 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
--rw-r--r--   0 runner    (1001) docker     (122)     8399 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
--rw-r--r--   0 runner    (1001) docker     (122)    13216 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py
--rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.669681 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/old/
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/old/aggregates.py
--rw-r--r--   0 runner    (1001) docker     (122)    19211 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/old/datatable.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.669681 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)     7108 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.673681 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)     6660 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15394 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (122)    25444 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
--rw-r--r--   0 runner    (1001) docker     (122)    45059 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
--rw-r--r--   0 runner    (1001) docker     (122)    35127 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
--rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/test_case_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.657681 OpenFisca-France-Data-1.2.0/openfisca_france_data/felin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.673681 OpenFisca-France-Data-1.2.0/openfisca_france_data/felin/input_data_builder/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/felin/input_data_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.673681 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      541 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/calage.py
--rw-r--r--   0 runner    (1001) docker     (122)    11373 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/id_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/model/survey_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.673681 OpenFisca-France-Data-1.2.0/openfisca_france_data/reforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12440 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/reforms/inversion_directe_salaires.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.677681 OpenFisca-France-Data-1.2.0/openfisca_france_data/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/scripts/build_input_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/smic.py
--rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)    15060 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/openfisca_france_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-30 14:24:02.681681 OpenFisca-France-Data-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.677681 OpenFisca-France-Data-1.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.657681 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.681681 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/
--rw-r--r--   0 runner    (1001) docker     (122)     2466 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_af.py
--rw-r--r--   0 runner    (1001) docker     (122)     8456 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_al.py
--rw-r--r--   0 runner    (1001) docker     (122)    10685 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_impot_revenu.py
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_inflation.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_input_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_pivot_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_rebuild_input_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_salaire_imposable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 14:24:02.681681 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/unit/
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/unit/test_get_survey_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/erfs_fpr/unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/test_fake_survey_simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/test_get_baremes_salarie.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-06-30 14:23:37.000000 OpenFisca-France-Data-1.2.0/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.638103 OpenFisca-France-Data-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10956 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.626102 OpenFisca-France-Data-1.3.0/OpenFisca_France_Data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-07-19 09:52:08.000000 OpenFisca-France-Data-1.3.0/OpenFisca_France_Data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4093 2023-07-19 09:52:08.000000 OpenFisca-France-Data-1.3.0/OpenFisca_France_Data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 09:52:08.000000 OpenFisca-France-Data-1.3.0/OpenFisca_France_Data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-07-19 09:52:08.000000 OpenFisca-France-Data-1.3.0/OpenFisca_France_Data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-07-19 09:52:08.000000 OpenFisca-France-Data-1.3.0/OpenFisca_France_Data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-07-19 09:52:08.000000 OpenFisca-France-Data-1.3.0/OpenFisca_France_Data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11506 2023-07-19 09:52:08.642103 OpenFisca-France-Data-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.630102 OpenFisca-France-Data-1.3.0/openfisca_france_data/
+-rw-r--r--   0 runner    (1001) docker     (122)     7682 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4356 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.630102 OpenFisca-France-Data-1.3.0/openfisca_france_data/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.630102 OpenFisca-France-Data-1.3.0/openfisca_france_data/assets/zone_apl_data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/assets/zone_apl_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/assets/zone_apl_data/codeAplReader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.630102 OpenFisca-France-Data-1.3.0/openfisca_france_data/assets/zone_apl_data/zone_apl/
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/assets/zone_apl_data/zone_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1814 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/base_survey.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21046 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24951 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      996 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.626102 OpenFisca-France-Data-1.3.0/openfisca_france_data/dads/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.630102 OpenFisca-France-Data-1.3.0/openfisca_france_data/dads/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/dads/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.630102 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.634103 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8932 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21783 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11919 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26165 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13995 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36615 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8399 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13216 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1536 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.634103 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/old/
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/old/aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19211 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/old/datatable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.634103 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4805 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7108 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.634103 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)     6660 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15394 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25444 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45059 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35127 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/test_case_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.626102 OpenFisca-France-Data-1.3.0/openfisca_france_data/felin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.634103 OpenFisca-France-Data-1.3.0/openfisca_france_data/felin/input_data_builder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/felin/input_data_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.634103 OpenFisca-France-Data-1.3.0/openfisca_france_data/model/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      541 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8882 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/model/calage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11373 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/model/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/model/id_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/model/survey_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.638103 OpenFisca-France-Data-1.3.0/openfisca_france_data/reforms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12440 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/reforms/inversion_directe_salaires.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.638103 OpenFisca-France-Data-1.3.0/openfisca_france_data/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/scripts/build_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/smic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15060 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/openfisca_france_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-07-19 09:52:08.642103 OpenFisca-France-Data-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.638103 OpenFisca-France-Data-1.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.626102 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.638103 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)     2466 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_af.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8456 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_al.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10685 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_impot_revenu.py
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_input_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_pivot_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_rebuild_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_salaire_imposable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 09:52:08.638103 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/unit/test_get_survey_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/erfs_fpr/unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/test_fake_survey_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/test_get_baremes_salarie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-07-19 09:51:39.000000 OpenFisca-France-Data-1.3.0/tests/test_misc.py
```

### Comparing `OpenFisca-France-Data-1.2.0/CHANGELOG.md` & `OpenFisca-France-Data-1.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+# 1.3.0 [#227](https://github.com/openfisca/openfisca-france-data/pull/227)
+* Technical changes
+- Adapte le comparator pour effectuer plus de tests en distribution
+- Permet l'utilisation d'un SurveyScenario facilement personnalisable
+
+
 # 1.2.0 [#226](https://github.com/openfisca/openfisca-france-data/pull/226)
 * Technical changes
 - Adapte le comparator pour permettre de changer les agrégats cibles.
 - Ajoute les agrégats de la note de validation d'INES
 
 # 1.1.0 [#225](https://github.com/openfisca/openfisca-france-data/pull/225)
```

### Comparing `OpenFisca-France-Data-1.2.0/CONTRIBUTING.md` & `OpenFisca-France-Data-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/LICENSE` & `OpenFisca-France-Data-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/PKG-INFO` & `OpenFisca-France-Data-1.3.0/OpenFisca_France_Data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 1.2.0
+Version: 1.3.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-France-Data-1.2.0/OpenFisca_France_Data.egg-info/SOURCES.txt` & `OpenFisca-France-Data-1.3.0/OpenFisca_France_Data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/PKG-INFO` & `OpenFisca-France-Data-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-France-Data
-Version: 1.2.0
+Version: 1.3.0
 Summary: OpenFisca-France-Data module to work with French survey data
 Home-page: https://github.com/openfisca/openfisca-france-data
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit social survey data microsimulation
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-France-Data-1.2.0/README.md` & `OpenFisca-France-Data-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/__init__.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/aggregates.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/assets/zone_apl_data/zone_apl/zone_apl_imputation_data_reader.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/base_survey.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/base_survey.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/common.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/common.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/comparator.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/comparator.py`

 * *Files 4% similar despite different names*

```diff
@@ -300,15 +300,32 @@
 
 class AbstractComparator(object):
     name = None
     default_target_variables = None
     filter_expr_by_label = None
     period = None
     messages = list()
-    survey_name = None
+    survey_scenario = None
+
+    def __init__(self):
+        name = self.get_name()
+        assert name is not None and isinstance(name, str)
+
+        figures_directory = Path(config.get("paths", "figures_directory")) / name
+
+        if not figures_directory.exists():
+            figures_directory.mkdir(parents = True, exist_ok = True)
+
+        self.figures_directory = figures_directory
+
+    def compute_aggregates_comparison(self, input_dataframe_by_entity = None):
+        pass
+
+    def compute_distibution_comparison(self, input_dataframe_by_entity = None):
+        pass
 
     def get_name(self):
         return self.name + "_" + str(self.period)
 
     def get_test_dataframes(self, rebuild = False, noindivs = None):
         start_time = datetime.datetime.now()
         if not rebuild:
@@ -335,41 +352,34 @@
                 }
             target_dataframe_by_entity = {
                 "individu": target_dataframe_by_entity["individu"].query(f"noindiv in {selected_noindivs}"),
                 "menage": target_dataframe_by_entity["menage"].query(menage_query),
                 }
         return input_dataframe_by_entity, target_dataframe_by_entity
 
-    def compare(self, browse, load, verbose, debug, target_variables = None, period = None, rebuild = False, summary = False):
+    def compare(self, browse, load, verbose, debug, target_variables = None, period = None, rebuild = False, summary = False, compute_divergence = False):
         """Compare actual data with openfisca-france-data computation."""
         log.setLevel(level = logging.DEBUG if verbose else logging.WARNING)
 
-        name = self.get_name()
-
-        assert name is not None and isinstance(name, str)
-
-        figures_directory = Path(config.get("paths", "figures_directory")) / name
-
-        if not figures_directory.exists():
-            figures_directory.mkdir(parents = True, exist_ok = True)
-
         if target_variables is not None and isinstance(target_variables, str):
             target_variables = [target_variables]
 
         assert (target_variables is None) or isinstance(target_variables, list)
 
         if target_variables is None:
             target_variables = self.default_target_variables
 
+        self.target_variables = target_variables   
+
         if period is not None:
             period = int(period)
 
         backup_directory = PurePath.joinpath(Path(config.get("paths", "backup")))
         backup_directory.mkdir(parents = True, exist_ok = True)
-
+        name = self.name
         backup_path = PurePath.joinpath(backup_directory, f"{name}_backup.h5")
 
         if load:
             assert Path.exists(backup_path), f"Backup file {backup_path} doesn't exist"
             shown = pd.read_hdf(
                 backup_path,
                 'result',
@@ -382,32 +392,44 @@
 
         try:
             start_time = datetime.datetime.now()
             input_dataframe_by_entity, target_dataframe_by_entity = self.get_test_dataframes(rebuild)
 
             log.debug(f"Test data has been prepared in {datetime.datetime.now() - start_time}")
 
-            # specific_figures_directory = PurePath.joinpath(figures_directory, self.name)
-            specific_figures_directory = figures_directory
-            specific_figures_directory.mkdir(parents = True, exist_ok = True)
-
-            result_by_variable = self.compute_divergence(
-                # input_dataframe_by_entity,
-                None,  # To force load the data_table from hdf file
-                target_dataframe_by_entity,
-                specific_figures_directory,
-                target_variables = target_variables,
-                period = period,
-                summary = summary,
+            self.compute_aggregates_comparison(
+                input_dataframe_by_entity = input_dataframe_by_entity,
                 )
 
-            result = pd.concat(result_by_variable, ignore_index = True)
+            self.compute_distibution_comparison(input_dataframe_by_entity = input_dataframe_by_entity)
+
+            if compute_divergence:
+                result_by_variable, markdown_section_by_variable, markdown_summary_section_by_variable = self.compute_divergence(
+                    input_dataframe_by_entity = None,  # To force load the data_table from hdf file
+                    target_dataframe_by_entity = target_dataframe_by_entity,
+                    target_variables = target_variables,
+                    period = period,
+                    summary = summary,
+                    )
+
+            # Deal with markdown_section
+
+                self.create_report(markdown_section_by_variable, markdown_summary_section_by_variable)
+
+                if result_by_variable is None:
+                    return
+
+                result = pd.concat(result_by_variable, ignore_index = True)
+            else:
+                self.create_report(None,None)
 
             log.debug(f"Eveyrthing has been computed in {datetime.datetime.now() - start_time}")
             del input_dataframe_by_entity, target_dataframe_by_entity
+
+
             if browse:
                 start_browsing_time = datetime.datetime.now()
                 result = result.dropna(axis = 1, how = 'all')
                 matching_variables = ["noindiv"]
                 assert set(matching_variables) <= set(result.columns)
                 cols_to_use = result.columns.tolist() + matching_variables
                 shown = result
@@ -430,29 +452,30 @@
 
         except Exception as error:
             if debug:
                 print(error)
                 pdb.post_mortem(sys.exc_info()[2])
             raise error
 
-    def compute_divergence(self, input_dataframe_by_entity, target_dataframe_by_entity, figures_directory, target_variables = None, period = None, summary = False):
+    def compute_divergence(self, input_dataframe_by_entity, target_dataframe_by_entity,
+            target_variables = None, period = None, summary = False):
         """
         Compare openfisca-france-data computation with data targets.
 
         Args:
             input_dataframe_by_period (dict): Input data
             target_dataframe_by_period (dict): Targets to macth
             figures_directory (path): Where to store the figures
         """
-        figures_directory = figures_directory.resolve()
+        figures_directory = self.figures_directory.resolve()
         assert Path.exists(figures_directory)
 
         if target_variables is None:
             log.info(f"No target variables. Exiting divergence computation.")
-            return
+            return None, None, None
 
         data = (
             dict(input_dataframe_by_entity = input_dataframe_by_entity)
             if input_dataframe_by_entity is not None
             else None
             )
 
@@ -501,72 +524,90 @@
                 figures_directory,
                 )
 
             if variable_markdown_section is not None:
                 markdown_section_by_variable[variable] = variable_markdown_section
 
             if summary:
-                # create_stats_by_period_figure(variable, result, period, figures_directory = figures_directory)
                 variable_markdown_summary_section = create_variable_markdown_summary_section(
                     variable,
                     stats,
                     figures_directory,
                     )
                 if variable_markdown_summary_section is not None:
                     markdown_summary_section_by_variable[variable] = variable_markdown_summary_section
 
-        messages_markdown_section = """
+        return result_by_variable, markdown_section_by_variable, markdown_summary_section_by_variable
+
+    def compute_test_dataframes(self):
+        NotImplementedError
+
+    def create_report(self, markdown_section_by_variable, markdown_summary_section_by_variable):
+        figures_directory = self.figures_directory
+
+        if self.messages:
+            messages_markdown_section = """
 Filtres appliqués:
 
 """ + "\n".join(f"- {message}" for message in self.messages) + """
 """
-        with open(figures_directory / "filters.md", "w", encoding = 'utf-8') as filters_md_file:
-            filters_md_file.write(messages_markdown_section)
+        else:
+            messages_markdown_section = ""
 
-        markdown_sections = list(filter(
-            lambda x: x is not None,
-            [messages_markdown_section] + list(markdown_section_by_variable.values()),
-            ))
-        create_output_files(
-            markdown_sections,
-            figures_directory,
-            "variables",
-            )
-        if summary:
-            markdown_sections = list(filter(
-                lambda x: x is not None,
-                [messages_markdown_section] + list(markdown_summary_section_by_variable.values()),
-                ))
+        table_agregats_markdown = None
+        if PurePath.joinpath(figures_directory, "table_agregats.md").exists():
+            with open(figures_directory / "table_agregats.md", "r", encoding = 'utf-8') as table_agregats_md_file:
+                table_agregats_markdown = table_agregats_md_file.read()
+
+        distribution_comparison_markdown = None
+        if PurePath.joinpath(figures_directory, "distribution_comparison_md").exists():
+            with open(figures_directory / "distribution_comparison_md", "r", encoding = 'utf-8') as distribution_comparison_md_file:
+                distribution_comparison_markdown = distribution_comparison_md_file.read()
+
+        front_sections = [messages_markdown_section, table_agregats_markdown, distribution_comparison_markdown]
+        sections_by_filename = {
+            "variables": markdown_section_by_variable,
+            "summary_variables": markdown_summary_section_by_variable
+            }
+
+        for filename, section_by_variable in sections_by_filename.items():
+            if section_by_variable is not None:
+                markdown_sections = list(filter(
+                    lambda x: x is not None,
+                    front_sections + list(section_by_variable.values()),
+                    ))
+            else:
+                markdown_sections = list(filter(
+                    lambda x: x is not None,front_sections
+                    ))
             create_output_files(
                 markdown_sections,
                 figures_directory,
-                "summary_variables",
+                filename,
                 )
 
-        return result_by_variable
-
-    def compute_test_dataframes(self):
-        NotImplementedError
-
     def filter(self, data_frame):
         for label, filter_expr in self.filter_expr_by_label.items():
             obs_before = data_frame.noind.nunique()
             selection = (data_frame
                 .eval("keep = " + filter_expr)
                 .groupby("noindiv")["keep"]
                 .transform('all')
                 )
             data_frame.drop(data_frame.index[~selection], inplace = True)
             obs_after = data_frame.noind.nunique()
             log_message = f"Applying filter '{label}': dropping {obs_before - obs_after}, keeping {obs_after} observations."
             log.info(log_message)
             self.messages.append(log_message + "\n")
 
-    def get_survey_scenario(self, data = None):
-        survey_name = self.survey_name
+    def get_survey_scenario(self, data = None, survey_name = None):
+
+        if self.survey_scenario is not None:
+            return self.survey_scenario
+
         return get_survey_scenario(
             year = str(self.period),
             data = data,
             survey_name = f'openfisca_erfs_fpr_{self.period}' if survey_name is None else survey_name,
             )
 
     def _load_test_dataframes(self, noindivs = None, idents = None):
```

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/config.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/dads/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/__init__.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/__init__.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/base.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/run_all.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/run_all.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_01_pre_processing.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_03_fip.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_05_foyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_06_rebuild.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_07_invalides.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_08_final.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/input_data_builder/step_10_check_final2.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/old/aggregates.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/old/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/old/datatable.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/old/datatable.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs/scenario.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs/scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/comparison.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/comparison.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_01_preprocessing.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_imputation_loyer.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_02_menage.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_03_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_04_famille.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/input_data_builder/step_06_final.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/scenario.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/erfs_fpr/test_case_creation.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/erfs_fpr/test_case_creation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/felin/input_data_builder/create_variables_individuelles.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/model/base.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/model/base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/model/calage.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/model/calage.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/model/common.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/model/common.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/model/id_variables.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/model/id_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/model/survey_variables.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/model/survey_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/reforms/inversion_directe_salaires.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/reforms/inversion_directe_salaires.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/scripts/build_input_data.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/scripts/build_input_data.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/smic.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/smic.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/surveys.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/openfisca_france_data/utils.py` & `OpenFisca-France-Data-1.3.0/openfisca_france_data/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/setup.cfg` & `OpenFisca-France-Data-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/setup.py` & `OpenFisca-France-Data-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name = "OpenFisca-France-Data",
-    version = "1.2.0",
+    version = "1.3.0",
     description = "OpenFisca-France-Data module to work with French survey data",
     long_description = long_description,
     long_description_content_type="text/markdown",
     author = "OpenFisca Team",
     author_email = "contact@openfisca.fr",
     url = "https://github.com/openfisca/openfisca-france-data",
     license = "http://www.fsf.org/licensing/licenses/agpl-3.0.html",
@@ -49,14 +49,13 @@
             "dtale",
             "flake8 >= 3.7.0, < 4.0.0",
             "ipdb >=0.13, <1.0",
             "ipython >= 7.5.0, < 8.0.0",
             "mypy >= 0.670, < 1.0.0",
             "pypandoc",
             'pytest >= 7.2.2, < 8.0',
-            # "pytest-cov >= 2.6.0, < 3.0.0",
             "scipy >= 1.2.1, < 2.0.0",
             "toolz >= 0.9.0, < 1.0.0",
             ],
         },
     packages = find_namespace_packages(exclude = ("docs", "tests")),
     )
```

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_af.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_af.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_aggregates.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_al.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_al.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_create_salaire_de_base.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_impot_revenu.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_impot_revenu.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_inflation.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_inflation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_input_variables.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_input_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_pivot_table.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_pivot_table.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_rebuild_input_data.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_rebuild_input_data.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_rsa.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_rsa.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/integration/test_salaire_imposable.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/integration/test_salaire_imposable.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/erfs_fpr/unit/test_get_survey_scenario.py` & `OpenFisca-France-Data-1.3.0/tests/erfs_fpr/unit/test_get_survey_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/test_aggregate.py` & `OpenFisca-France-Data-1.3.0/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/test_calibration.py` & `OpenFisca-France-Data-1.3.0/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/test_fake_survey_simulation.py` & `OpenFisca-France-Data-1.3.0/tests/test_fake_survey_simulation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/test_get_baremes_salarie.py` & `OpenFisca-France-Data-1.3.0/tests/test_get_baremes_salarie.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-France-Data-1.2.0/tests/test_misc.py` & `OpenFisca-France-Data-1.3.0/tests/test_misc.py`

 * *Files identical despite different names*

