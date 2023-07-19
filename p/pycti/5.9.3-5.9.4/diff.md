# Comparing `tmp/pycti-5.9.3.tar.gz` & `tmp/pycti-5.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-5.9.3.tar", last modified: Tue Jul 18 16:45:53 2023, max compression
+gzip compressed data, was "pycti-5.9.4.tar", last modified: Wed Jul 19 02:58:30 2023, max compression
```

## Comparing `pycti-5.9.3.tar` & `pycti-5.9.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 16:45:53.636886 pycti-5.9.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-07-18 16:45:39.000000 pycti-5.9.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-18 16:45:53.636886 pycti-5.9.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-18 16:45:39.000000 pycti-5.9.3/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 16:45:53.628886 pycti-5.9.3/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4457 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 16:45:53.628886 pycti-5.9.3/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28771 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 16:45:53.628886 pycti-5.9.3/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45760 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/connector/opencti_connector_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 16:45:53.636886 pycti-5.9.3/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14340 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25352 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24724 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24705 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15508 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15549 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15139 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11897 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23072 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18533 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15126 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23083 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15950 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22773 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23099 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21404 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23941 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23507 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10147 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18610 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18872 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 16:45:53.636886 pycti-5.9.3/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6827 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106275 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14515 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-07-18 16:45:39.000000 pycti-5.9.3/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 16:45:53.628886 pycti-5.9.3/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-18 16:45:53.000000 pycti-5.9.3/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-18 16:45:53.000000 pycti-5.9.3/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-18 16:45:53.000000 pycti-5.9.3/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-07-18 16:45:53.000000 pycti-5.9.3/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-18 16:45:53.000000 pycti-5.9.3/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-07-18 16:45:39.000000 pycti-5.9.3/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-07-18 16:45:53.636886 pycti-5.9.3/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.072955 pycti-5.9.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-07-19 02:58:17.000000 pycti-5.9.4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-19 02:58:30.072955 pycti-5.9.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-19 02:58:17.000000 pycti-5.9.4/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.060955 pycti-5.9.4/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4457 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.064955 pycti-5.9.4/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28771 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.064955 pycti-5.9.4/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45760 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/connector/opencti_connector_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.072955 pycti-5.9.4/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14340 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25926 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24724 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24705 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15508 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15549 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15139 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11897 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23072 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18533 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15126 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23083 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15950 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22773 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23099 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21404 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23941 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23507 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10147 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18610 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18872 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.072955 pycti-5.9.4/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6827 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106275 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14515 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.064955 pycti-5.9.4/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-19 02:58:30.000000 pycti-5.9.4/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-19 02:58:30.000000 pycti-5.9.4/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-19 02:58:30.000000 pycti-5.9.4/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-07-19 02:58:30.000000 pycti-5.9.4/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-19 02:58:30.000000 pycti-5.9.4/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-07-19 02:58:17.000000 pycti-5.9.4/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-07-19 02:58:30.076955 pycti-5.9.4/setup.cfg
```

### Comparing `pycti-5.9.3/LICENSE` & `pycti-5.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/PKG-INFO` & `pycti-5.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.9.3
+Version: 5.9.4
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.9.3 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.9.4 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.9.3/README.md` & `pycti-5.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/__init__.py` & `pycti-5.9.4/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "5.9.3"
+__version__ = "5.9.4"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-5.9.3/pycti/api/opencti_api_client.py` & `pycti-5.9.4/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/api/opencti_api_connector.py` & `pycti-5.9.4/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/api/opencti_api_work.py` & `pycti-5.9.4/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/connector/opencti_connector.py` & `pycti-5.9.4/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/connector/opencti_connector_helper.py` & `pycti-5.9.4/pycti/connector/opencti_connector_helper.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_attack_pattern.py` & `pycti-5.9.4/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_campaign.py` & `pycti-5.9.4/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_case_incident.py` & `pycti-5.9.4/pycti/entities/opencti_case_incident.py`

 * *Files 4% similar despite different names*

```diff
@@ -467,14 +467,15 @@
         description = kwargs.get("description", None)
         severity = kwargs.get("severity", None)
         priority = kwargs.get("priority", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
         response_types = kwargs.get("response_types", None)
+        x_opencti_workflow_id = kwargs.get("x_opencti_workflow_id", None)
 
         if name is not None:
             self.opencti.log("info", "Creating Case Incident {" + name + "}.")
             query = """
                 mutation CaseIncidentAdd($input: CaseIncidentAddInput!) {
                     caseIncidentAdd(input: $input) {
                         id
@@ -503,14 +504,15 @@
                         "name": name,
                         "description": description,
                         "severity": severity,
                         "priority": priority,
                         "x_opencti_stix_ids": x_opencti_stix_ids,
                         "update": update,
                         "response_types": response_types,
+                        "x_opencti_workflow_id": x_opencti_workflow_id,
                     }
                 },
             )
             return self.opencti.process_multiple_fields(
                 result["data"]["caseIncidentAdd"]
             )
         else:
@@ -632,14 +634,20 @@
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
             if "granted_refs" not in stix_object:
                 stix_object["granted_refs"] = self.opencti.get_attribute_in_extension(
                     "granted_refs", stix_object
                 )
+            if "x_opencti_workflow_id" not in stix_object:
+                stix_object[
+                    "x_opencti_workflow_id"
+                ] = self.opencti.get_attribute_in_extension(
+                    "x_opencti_workflow_id", stix_object
+                )
 
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
@@ -672,14 +680,17 @@
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
+                x_opencti_workflow_id=stix_object["x_opencti_workflow_id"]
+                if "x_opencti_workflow_id" in stix_object
+                else None,
                 update=update,
             )
         else:
             self.opencti.log(
                 "error", "[opencti_caseIncident] Missing parameters: stixObject"
             )
```

### Comparing `pycti-5.9.3/pycti/entities/opencti_case_rfi.py` & `pycti-5.9.4/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_case_rft.py` & `pycti-5.9.4/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_channel.py` & `pycti-5.9.4/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_course_of_action.py` & `pycti-5.9.4/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_data_component.py` & `pycti-5.9.4/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_data_source.py` & `pycti-5.9.4/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_event.py` & `pycti-5.9.4/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_external_reference.py` & `pycti-5.9.4/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_feedback.py` & `pycti-5.9.4/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_grouping.py` & `pycti-5.9.4/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_identity.py` & `pycti-5.9.4/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_incident.py` & `pycti-5.9.4/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_indicator.py` & `pycti-5.9.4/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_infrastructure.py` & `pycti-5.9.4/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_intrusion_set.py` & `pycti-5.9.4/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_kill_chain_phase.py` & `pycti-5.9.4/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_label.py` & `pycti-5.9.4/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_language.py` & `pycti-5.9.4/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_location.py` & `pycti-5.9.4/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_malware.py` & `pycti-5.9.4/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_malware_analysis.py` & `pycti-5.9.4/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_marking_definition.py` & `pycti-5.9.4/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_narrative.py` & `pycti-5.9.4/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_note.py` & `pycti-5.9.4/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_observed_data.py` & `pycti-5.9.4/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_opinion.py` & `pycti-5.9.4/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_report.py` & `pycti-5.9.4/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_stix.py` & `pycti-5.9.4/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_stix_core_object.py` & `pycti-5.9.4/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_stix_core_relationship.py` & `pycti-5.9.4/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-5.9.4/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_stix_domain_object.py` & `pycti-5.9.4/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-5.9.4/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-5.9.4/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-5.9.4/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_task.py` & `pycti-5.9.4/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_threat_actor.py` & `pycti-5.9.4/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_threat_actor_group.py` & `pycti-5.9.4/pycti/entities/opencti_threat_actor_group.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_threat_actor_individual.py` & `pycti-5.9.4/pycti/entities/opencti_threat_actor_individual.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_tool.py` & `pycti-5.9.4/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_vocabulary.py` & `pycti-5.9.4/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/entities/opencti_vulnerability.py` & `pycti-5.9.4/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/utils/constants.py` & `pycti-5.9.4/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/utils/opencti_stix2.py` & `pycti-5.9.4/pycti/utils/opencti_stix2.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/utils/opencti_stix2_splitter.py` & `pycti-5.9.4/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/utils/opencti_stix2_update.py` & `pycti-5.9.4/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti/utils/opencti_stix2_utils.py` & `pycti-5.9.4/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti.egg-info/PKG-INFO` & `pycti-5.9.4/pycti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.9.3
+Version: 5.9.4
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.9.3 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.9.4 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.9.3/pycti.egg-info/SOURCES.txt` & `pycti-5.9.4/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pycti.egg-info/requires.txt` & `pycti-5.9.4/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/pyproject.toml` & `pycti-5.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-5.9.3/setup.cfg` & `pycti-5.9.4/setup.cfg`

 * *Files identical despite different names*

