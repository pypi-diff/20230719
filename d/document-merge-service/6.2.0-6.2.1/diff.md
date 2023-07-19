# Comparing `tmp/document_merge_service-6.2.0.tar.gz` & `tmp/document_merge_service-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_merge_service-6.2.0.tar", max compression
+gzip compressed data, was "document_merge_service-6.2.1.tar", max compression
```

## Comparing `document_merge_service-6.2.0.tar` & `document_merge_service-6.2.1.tar`

### file list

```diff
@@ -1,67 +1,72 @@
--rw-r--r--   0        0        0    11148 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/LICENSE
--rw-r--r--   0        0        0     2261 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/__init__.py
--rw-r--r--   0        0        0      405 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/apps.py
--rw-r--r--   0        0        0     3159 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/authentication.py
--rw-r--r--   0        0        0      504 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/__init__.py
--rw-r--r--   0        0        0      559 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/black.png
--rw-r--r--   0        0        0     9125 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-mailmerge-syntax.docx
--rw-r--r--   0        0        0    11489 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-mailmerge.docx
--rw-r--r--   0        0        0     5735 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-template-filters.docx
--rw-r--r--   0        0        0     6087 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-template-loopcontrols.docx
--rw-r--r--   0        0        0     5952 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-template-placeholdercheck.docx
--rw-r--r--   0        0        0     5091 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-template-syntax.docx
--rw-r--r--   0        0        0     5490 2023-07-11 13:55:30.165032 document_merge_service-6.2.0/document_merge_service/api/data/docx-template.docx
--rw-r--r--   0        0        0  1127936 2023-07-11 13:55:30.169032 document_merge_service-6.2.0/document_merge_service/api/data/loadtest/1.doc
--rw-r--r--   0        0        0   175922 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/loadtest/2.docx
--rw-r--r--   0        0        0   163307 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/loadtest/3.docx
--rw-r--r--   0        0        0   141498 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/loadtest/4.docx
--rw-r--r--   0        0        0       22 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/test.txt
--rw-r--r--   0        0        0        5 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/xlsx-not-valid.xlsx
--rw-r--r--   0        0        0     6467 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/xlsx-structure.xlsx
--rw-r--r--   0        0        0     6432 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/xlsx-syntax.xlsx
--rw-r--r--   0        0        0     4750 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/data/xlsx-template.xlsx
--rw-r--r--   0        0        0     9774 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/engines.py
--rw-r--r--   0        0        0      389 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/factories.py
--rw-r--r--   0        0        0     2841 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/filters.py
--rw-r--r--   0        0        0     2546 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/jinja.py
--rw-r--r--   0        0        0        0 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/management/commands/__init__.py
--rw-r--r--   0        0        0     1582 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/management/commands/clean_dangling_files.py
--rw-r--r--   0        0        0     1249 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      489 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0002_template_group.py
--rw-r--r--   0        0        0      375 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0003_template_meta.py
--rw-r--r--   0        0        0      145 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0004_cleanup_files.py
--rw-r--r--   0        0        0     1005 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py
--rw-r--r--   0        0        0      328 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/0006_remove_template_group.py
--rw-r--r--   0        0        0        0 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/migrations/__init__.py
--rw-r--r--   0        0        0     1876 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/models.py
--rw-r--r--   0        0        0      231 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/pagination.py
--rw-r--r--   0        0        0      289 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/permissions.py
--rw-r--r--   0        0        0     4651 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/serializers.py
--rw-r--r--   0        0        0        0 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/snapshots/__init__.py
--rw-r--r--   0        0        0    29399 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/snapshots/snap_test_template.py
--rw-r--r--   0        0        0     2270 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/test_authentication.py
--rw-r--r--   0        0        0      942 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/test_clean_dangling_files.py
--rw-r--r--   0        0        0     1963 2023-07-11 13:55:30.173032 document_merge_service-6.2.0/document_merge_service/api/tests/test_excel.py
--rw-r--r--   0        0        0     1372 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/tests/test_filters.py
--rw-r--r--   0        0        0     1300 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/tests/test_jinja.py
--rw-r--r--   0        0        0      749 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/tests/test_pagination.py
--rw-r--r--   0        0        0    25635 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/tests/test_template.py
--rw-r--r--   0        0        0     3425 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/tests/test_unoconv.py
--rw-r--r--   0        0        0     6947 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/unoconv.py
--rw-r--r--   0        0        0      356 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/urls.py
--rw-r--r--   0        0        0     3570 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/api/views.py
--rw-r--r--   0        0        0     2794 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/conftest.py
--rw-r--r--   0        0        0      789 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/sentry.py
--rw-r--r--   0        0        0     8581 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/settings.py
--rw-r--r--   0        0        0        0 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/tests/__init__.py
--rw-r--r--   0        0        0      434 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/tests/test_sentry.py
--rw-r--r--   0        0        0      615 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/tests/test_settings.py
--rw-r--r--   0        0        0      225 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/urls.py
--rw-r--r--   0        0        0      412 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/document_merge_service/wsgi.py
--rw-r--r--   0        0        0     3592 2023-07-11 13:55:30.177033 document_merge_service-6.2.0/pyproject.toml
--rw-r--r--   0        0        0     4247 1970-01-01 00:00:00.000000 document_merge_service-6.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11511 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/LICENSE
+-rw-r--r--   0        0        0     2243 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/__init__.py
+-rw-r--r--   0        0        0      405 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/apps.py
+-rw-r--r--   0        0        0     3159 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/authentication.py
+-rw-r--r--   0        0        0      504 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/__init__.py
+-rw-r--r--   0        0        0      559 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/black.png
+-rw-r--r--   0        0        0     9125 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-mailmerge-syntax.docx
+-rw-r--r--   0        0        0    11489 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-mailmerge.docx
+-rw-r--r--   0        0        0     5735 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-template-filters.docx
+-rw-r--r--   0        0        0     6087 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-template-loopcontrols.docx
+-rw-r--r--   0        0        0     5952 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-template-placeholdercheck.docx
+-rw-r--r--   0        0        0     5091 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-template-syntax.docx
+-rw-r--r--   0        0        0     5490 2023-07-19 13:15:19.469111 document_merge_service-6.2.1/document_merge_service/api/data/docx-template.docx
+-rw-r--r--   0        0        0  1127936 2023-07-19 13:15:19.473111 document_merge_service-6.2.1/document_merge_service/api/data/loadtest/1.doc
+-rw-r--r--   0        0        0   175922 2023-07-19 13:15:19.473111 document_merge_service-6.2.1/document_merge_service/api/data/loadtest/2.docx
+-rw-r--r--   0        0        0   163307 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/loadtest/3.docx
+-rw-r--r--   0        0        0   141498 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/loadtest/4.docx
+-rw-r--r--   0        0        0       22 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/test.txt
+-rw-r--r--   0        0        0        5 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/xlsx-not-valid.xlsx
+-rw-r--r--   0        0        0     6467 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/xlsx-structure.xlsx
+-rw-r--r--   0        0        0     6432 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/xlsx-syntax.xlsx
+-rw-r--r--   0        0        0     4750 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/data/xlsx-template.xlsx
+-rw-r--r--   0        0        0     9772 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/engines.py
+-rw-r--r--   0        0        0      389 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/factories.py
+-rw-r--r--   0        0        0     2841 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/filters.py
+-rw-r--r--   0        0        0     2546 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/jinja.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/management/commands/__init__.py
+-rw-r--r--   0        0        0     1628 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/management/commands/clean_dangling_files.py
+-rw-r--r--   0        0        0     1354 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/management/commands/upload_local_templates.py
+-rw-r--r--   0        0        0     1248 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0002_template_group.py
+-rw-r--r--   0        0        0      374 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0003_template_meta.py
+-rw-r--r--   0        0        0      145 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0004_cleanup_files.py
+-rw-r--r--   0        0        0     1004 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py
+-rw-r--r--   0        0        0      327 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/0006_remove_template_group.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/migrations/__init__.py
+-rw-r--r--   0        0        0     1845 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/models.py
+-rw-r--r--   0        0        0      231 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/pagination.py
+-rw-r--r--   0        0        0      289 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/permissions.py
+-rw-r--r--   0        0        0     4651 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0    29399 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/snapshots/snap_test_template.py
+-rw-r--r--   0        0        0     2270 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_authentication.py
+-rw-r--r--   0        0        0      942 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_clean_dangling_files.py
+-rw-r--r--   0        0        0     1963 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_excel.py
+-rw-r--r--   0        0        0     1372 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_filters.py
+-rw-r--r--   0        0        0     1300 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_jinja.py
+-rw-r--r--   0        0        0      749 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_pagination.py
+-rw-r--r--   0        0        0    25634 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_template.py
+-rw-r--r--   0        0        0     3425 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_unoconv.py
+-rw-r--r--   0        0        0      597 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/tests/test_upload_local_templates.py
+-rw-r--r--   0        0        0     6947 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/unoconv.py
+-rw-r--r--   0        0        0      356 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/urls.py
+-rw-r--r--   0        0        0     3570 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/api/views.py
+-rw-r--r--   0        0        0     2909 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/extensions/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/extensions/permissions.py
+-rw-r--r--   0        0        0       52 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/extensions/visibilities.py
+-rw-r--r--   0        0        0      789 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/sentry.py
+-rw-r--r--   0        0        0     8818 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/settings.py
+-rw-r--r--   0        0        0        0 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/tests/__init__.py
+-rw-r--r--   0        0        0      434 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/tests/test_sentry.py
+-rw-r--r--   0        0        0      615 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/tests/test_settings.py
+-rw-r--r--   0        0        0      225 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/urls.py
+-rw-r--r--   0        0        0      412 2023-07-19 13:15:19.477111 document_merge_service-6.2.1/document_merge_service/wsgi.py
+-rw-r--r--   0        0        0     3571 2023-07-19 13:15:19.481111 document_merge_service-6.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4191 1970-01-01 00:00:00.000000 document_merge_service-6.2.1/PKG-INFO
```

### Comparing `document_merge_service-6.2.0/CHANGELOG.md` & `document_merge_service-6.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 6.2.1 (19 July 2023)
+### Fix
+
+* **dgap:** Add env variables to configure permissions and visibilities ([`67fc95a`](https://github.com/adfinis/document-merge-service/commit/67fc95a16f72e7afed37342972c6101c492d529a))
+* Storage generic file cleanup ([`0633fd2`](https://github.com/adfinis/document-merge-service/commit/0633fd20a7a11f00a8d7eb6aa903aa38520fe8b1))
+
 ## 6.2.0 (11 July 2023)
 ### Feature
 * Add django storages and settings for s3 storage ([`6df1a83`](https://github.com/Yelinz/document-merge-service/commit/6df1a83a4befbb8687a951d45fe6910deba83272))
 
 ## 6.1.2 (10 May 2023)
 Maintenance release only containing dependency updates.
```

### Comparing `document_merge_service-6.2.0/LICENSE` & `document_merge_service-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/README.md` & `document_merge_service-6.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,38 +5,39 @@
 [![License: GPL-3.0-or-later](https://img.shields.io/github/license/adfinis/document-merge-service)](https://spdx.org/licenses/GPL-3.0-or-later.html)
 
 A document template merge service providing an API to manage templates and merge them with given data.
 
 ## Installation
 
 **Requirements**
-* docker
-* docker-compose
+
+- docker
+- docker-compose
 
 After installing and configuring those, download [docker-compose.yml](https://raw.githubusercontent.com/adfinis/document-merge-service/master/docker-compose.yml) and run the following command:
 
 ```bash
 docker-compose up -d
 ```
 
 You can now access the api at [http://localhost:8000/api/v1/](http://localhost:8000/api/v1/) which includes a browsable api.
 
 ### Workaround LibreOffice lockup
 
-The workaround has a setting called ISOLATE_UNOCONV, it is only enabled in the
-development environment. If ISOLATE_UNOCONV is enabled the container needs
-CAP_SYS_ADMIN. See docker-compose.override.yml.
+The workaround has a setting called `ISOLATE_UNOCONV`, it is only enabled in the
+development environment. If `ISOLATE_UNOCONV` is enabled the container needs
+`CAP_SYS_ADMIN`. See docker-compose.override.yml.
 
 ```yaml
-    cap_add:
-      - CAP_SYS_ADMIN
-    security_opt:
-      - apparmor:unconfined
-    environment:
-      - ISOLATE_UNOCONV=true
+cap_add:
+  - CAP_SYS_ADMIN
+security_opt:
+  - apparmor:unconfined
+environment:
+  - ISOLATE_UNOCONV=true
 ```
 
 ## Getting started
 
 ### Uploading templates
 
 Upload templates using the following:
@@ -49,18 +50,17 @@
 
 After uploading successfully, you can merge a template with the following call:
 
 ```bash
 curl -H "Content-Type: application/json" --data '{"data": {"test": "Test Input"}}' http://localhost:8000/api/v1/template/test-template/merge/ > output.docx
 ```
 
-
 ## Further reading
 
-* [Configuration](CONFIGURATION.md) - Further configuration and how to do a production setup
-* [Usage](USAGE.md) - How to use the DMS and it's features
-* [Contributing](CONTRIBUTING.md) - Look here to see how to start with your first
+- [Configuration](CONFIGURATION.md) - Further configuration and how to do a production setup
+- [Usage](USAGE.md) - How to use the DMS and it's features
+- [Contributing](CONTRIBUTING.md) - Look here to see how to start with your first
   contribution. Contributions are welcome!
 
 ## License
 
 Code released under the [GPL-3.0-or-later license](LICENSE).
```

### Comparing `document_merge_service-6.2.0/document_merge_service/api/authentication.py` & `document_merge_service-6.2.1/document_merge_service/api/authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/black.png` & `document_merge_service-6.2.1/document_merge_service/api/data/black.png`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/docx-mailmerge-syntax.docx` & `document_merge_service-6.2.1/document_merge_service/api/data/docx-mailmerge-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/docx-mailmerge.docx` & `document_merge_service-6.2.1/document_merge_service/api/data/docx-mailmerge.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/docx-template-filters.docx` & `document_merge_service-6.2.1/document_merge_service/api/data/docx-template-filters.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/docx-template-loopcontrols.docx` & `document_merge_service-6.2.1/document_merge_service/api/data/docx-template-loopcontrols.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/docx-template-placeholdercheck.docx` & `document_merge_service-6.2.1/document_merge_service/api/data/docx-template-placeholdercheck.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/docx-template-syntax.docx` & `document_merge_service-6.2.1/document_merge_service/api/data/docx-template-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/docx-template.docx` & `document_merge_service-6.2.1/document_merge_service/api/data/docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/loadtest/1.doc` & `document_merge_service-6.2.1/document_merge_service/api/data/loadtest/1.doc`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/loadtest/2.docx` & `document_merge_service-6.2.1/document_merge_service/api/data/loadtest/2.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/loadtest/3.docx` & `document_merge_service-6.2.1/document_merge_service/api/data/loadtest/3.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/loadtest/4.docx` & `document_merge_service-6.2.1/document_merge_service/api/data/loadtest/4.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/xlsx-structure.xlsx` & `document_merge_service-6.2.1/document_merge_service/api/data/xlsx-structure.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/xlsx-syntax.xlsx` & `document_merge_service-6.2.1/document_merge_service/api/data/xlsx-syntax.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/data/xlsx-template.xlsx` & `document_merge_service-6.2.1/document_merge_service/api/data/xlsx-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/engines.py` & `document_merge_service-6.2.1/document_merge_service/api/engines.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
 
 
 class DocxTemplateEngine(DocxValidator):
     def __init__(self, template):
         self.template = template
 
     def validate_template_syntax(self, available_placeholders=None, sample_data=None):
-
         try:
             doc = DocxTemplate(self.template)
             root = _MagicPlaceholder()
             env = get_jinja_env()
             ph = {
                 name: root[name] for name in doc.get_undeclared_template_variables(env)
             }
@@ -241,15 +240,14 @@
         try:
             self.merge(sample_data, buf, is_test_merge=True)
         except TemplateSyntaxError as exc:
             arg_str = ";".join(exc.args)
             raise exceptions.ValidationError(f"Syntax error in template: {arg_str}")
 
         if available_placeholders and magic is not None:
-
             missing_set = (
                 set(magic.reports)
                 - set(self._expand_available_placeholders(available_placeholders))
                 - set(self.BUILTIN_VARS)
             )
             if not missing_set:
                 return
```

### Comparing `document_merge_service-6.2.0/document_merge_service/api/filters.py` & `document_merge_service-6.2.1/document_merge_service/api/filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/jinja.py` & `document_merge_service-6.2.1/document_merge_service/api/jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/management/commands/clean_dangling_files.py` & `document_merge_service-6.2.1/document_merge_service/api/management/commands/clean_dangling_files.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.conf import settings
 from django.core.management.base import BaseCommand
 
 from document_merge_service.api.models import Template
 
 
 class Command(BaseCommand):
-    help = "Remove dangling template files that are not attached to a template model anymore"
+    help = "Remove dangling template files that are not attached to a template model anymore. Currently only usable with local filesystem."
 
     def add_arguments(self, parser):
         parser.add_argument("--dry-run", dest="dry", action="store_true", default=False)
 
     def handle(self, *args, **options):
         used_files = [template.template.path for template in Template.objects.all()]
```

### Comparing `document_merge_service-6.2.0/document_merge_service/api/migrations/0001_initial.py` & `document_merge_service-6.2.1/document_merge_service/api/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.11.17 on 2019-01-03 10:24
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Template",
```

### Comparing `document_merge_service-6.2.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py` & `document_merge_service-6.2.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.9 on 2022-03-29 07:52
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("api", "0004_cleanup_files"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="template",
```

### Comparing `document_merge_service-6.2.0/document_merge_service/api/models.py` & `document_merge_service-6.2.1/document_merge_service/api/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import os
-
+from django.core.files.storage import DefaultStorage
 from django.db import models
 from django.dispatch import receiver
 
 
 class Template(models.Model):
     DOCX_TEMPLATE = "docx-template"
     DOCX_MAILMERGE = "docx-mailmerge"
@@ -33,25 +32,23 @@
     meta = models.JSONField(default=dict)
 
 
 @receiver(models.signals.post_delete, sender=Template)
 def auto_delete_file_on_delete(sender, instance, **kwargs):
     """Delete template file from filesystem when `Template` object is deleted."""
 
-    if os.path.isfile(instance.template.path):
-        os.remove(instance.template.path)
+    DefaultStorage().delete(instance.template.name)
 
 
 @receiver(models.signals.pre_save, sender=Template)
 def auto_delete_file_on_change(sender, instance, **kwargs):
     """Delete old template file from filesystem when `Template` is given a new template file."""
 
     try:
         old_file = Template.objects.get(pk=instance.pk).template
     except Template.DoesNotExist:
         return
 
     if old_file:
         new_file = instance.template
         if not old_file == new_file:
-            if os.path.isfile(old_file.path):
-                os.remove(old_file.path)
+            DefaultStorage().delete(old_file.name)
```

### Comparing `document_merge_service-6.2.0/document_merge_service/api/serializers.py` & `document_merge_service-6.2.1/document_merge_service/api/serializers.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/tests/snapshots/snap_test_template.py` & `document_merge_service-6.2.1/document_merge_service/api/tests/snapshots/snap_test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/tests/test_authentication.py` & `document_merge_service-6.2.1/document_merge_service/api/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/tests/test_clean_dangling_files.py` & `document_merge_service-6.2.1/document_merge_service/api/tests/test_clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/tests/test_excel.py` & `document_merge_service-6.2.1/document_merge_service/api/tests/test_excel.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/tests/test_filters.py` & `document_merge_service-6.2.1/document_merge_service/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/tests/test_jinja.py` & `document_merge_service-6.2.1/document_merge_service/api/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/tests/test_pagination.py` & `document_merge_service-6.2.1/document_merge_service/api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/tests/test_template.py` & `document_merge_service-6.2.1/document_merge_service/api/tests/test_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,14 @@
     available_placeholders,
     sample_data,
     files,
     status_code,
     settings,
     expect_missing_placeholders,
 ):
-
     settings.DOCXTEMPLATE_JINJA_EXTENSIONS = ["jinja2.ext.loopcontrols"]
     url = reverse("template-list")
 
     template_file = django_file(template_name)
     data = {
         "slug": "test-slug",
         "template": template_file.file,
```

### Comparing `document_merge_service-6.2.0/document_merge_service/api/tests/test_unoconv.py` & `document_merge_service-6.2.1/document_merge_service/api/tests/test_unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/unoconv.py` & `document_merge_service-6.2.1/document_merge_service/api/unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/api/views.py` & `document_merge_service-6.2.1/document_merge_service/api/views.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/conftest.py` & `document_merge_service-6.2.1/document_merge_service/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import shutil
 from io import BytesIO
 from pathlib import Path
 
 import pytest
 import sentry_sdk
 from django.core.cache import cache
+from django.core.files.storage import DefaultStorage
 from pytest_factoryboy import register
 from rest_framework.test import APIClient
 
 from document_merge_service.api import engines, factories, models
 from document_merge_service.api.data import django_file
 
 from .api.authentication import AnonymousUser
@@ -72,14 +73,15 @@
     def make_template(placeholder):
         engine = engines.get_engine(template.engine, template.template)
         binary = BytesIO()
         engine.merge({"test": placeholder}, binary)
         binary.seek(0)
         template.template.save("foo.docx", binary)
         template.save()
+        DefaultStorage().save(template.template.name, binary)
         return template
 
     return make_template
 
 
 @pytest.fixture
 def dms_test_bin():
```

### Comparing `document_merge_service-6.2.0/document_merge_service/sentry.py` & `document_merge_service-6.2.1/document_merge_service/sentry.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/document_merge_service/settings.py` & `document_merge_service-6.2.1/document_merge_service/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,7 +264,11 @@
 if SENTRY_DSN:  # pragma: no cover
     sentry_init(
         SENTRY_DSN,
         SENTRY_ENVIRONMENT,
         SENTRY_TRACES_SAMPLE_RATE,
         SENTRY_SEND_DEFAULT_PII,
     )
+
+# https://github.com/adfinis/django-generic-api-permissions
+GENERIC_PERMISSIONS_PERMISSION_CLASSES = env.list("DMS_PERMISSION_CLASSES", default=[])
+GENERIC_PERMISSIONS_VISIBILITY_CLASSES = env.list("DMS_VISIBILITY_CLASSES", default=[])
```

### Comparing `document_merge_service-6.2.0/document_merge_service/tests/test_settings.py` & `document_merge_service-6.2.1/document_merge_service/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.0/pyproject.toml` & `document_merge_service-6.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "document-merge-service"
-version = "6.2.0"
+version = "6.2.1"
 description = "Merge Document Template Service"
 license = "GPL-3.0-or-later"
 authors = ["Adfinis AG <info@adfinis.com>"]
 homepage = "https://github.com/adfinis/document-merge-service"
 repository = "https://github.com/adfinis/document-merge-service"
 documentation = "https://github.com/adfinis/document-merge-service/blob/main/README.md"
 readme = "README.md"
@@ -16,66 +16,65 @@
 ]
 include = ["CHANGELOG.md"]
 exclude = [
     "document-merge-service/**/tests",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.8.1"
 Babel = "^2.11.0"
-Django = "^3.2.16"
-django-cors-headers = "^3.13.0"
-django-environ = "^0.9.0"
-django-filter = "^22.1"
+Django = "^3.2.20"
+django-cors-headers = "^4.2.0"
+django-environ = "^0.10.0"
+django-filter = "^23.2"
+django-generic-api-permissions = "^0.2.0"
+django-storages = "^1.13.2"
 djangorestframework = "^3.14.0"
 docx-mailmerge = "^0.5.0"
-docxtpl = "^0.16.4"
+docxtpl = "^0.16.7"
 Jinja2 = "^3.1.2"
-mysqlclient = { version = "^2.1.1", optional = true }
-psycopg2-binary = { version = "^2.9.5", optional = true }
+mysqlclient = { version = "^2.2.0", optional = true }
+psycopg2-binary = { version = "^2.9.6", optional = true }
 python-dateutil = "^2.8.2"
 python-memcached = "^1.59"
-requests = "^2.28.1"
+requests = "^2.31.0"
+sentry-sdk = "^1.28.1"
 uWSGI = "^2.0.21"
-xltpl = "^0.16"
-openpyxl = "^3.0.10"
-django-generic-api-permissions = "^0.2.0"
-sentry-sdk = "^1.12.1"
-django-storages = "^1.13.2"
+xltpl = "^0.18"
 
 [tool.poetry.group.dev.dependencies]
-black = "22.10.0"
-django-stubs = "1.13.0"
-factory-boy = "3.2.1"
-flake8 = "5.0.4"
+black = "23.7.0"
+django-stubs = "4.2.3"
+factory-boy = "3.3.0"
+flake8 = "6.0.0"
 flake8-debugger = "4.1.2"
-flake8-docstrings = "1.6.0"
-flake8-isort = "5.0.0"
+flake8-docstrings = "1.7.0"
+flake8-isort = "6.0.0"
 flake8-string-format = "0.3.0"
 flake8-tuple = "0.4.1"
-gitlint = "0.18.0"
-isort = "5.10.1"
-mypy = "0.991"
+gitlint = "0.19.1"
+isort = "5.12.0"
+mypy = "1.4.1"
 pdbpp = "0.10.3"
-psutil = "5.9.4"
-pydocstyle = "6.1.1"
-pytest = "7.2.0"
-pytest-cov = "4.0.0"
+psutil = "5.9.5"
+pydocstyle = "6.3.0"
+pytest = "7.4.0"
+pytest-cov = "4.1.0"
 pytest-django = "4.5.2"
-pytest-env = "0.8.1"
-pytest-factoryboy = "2.5.0"
-pytest-mock = "3.10.0"
-pytest-randomly = "3.12.0"
-python-semantic-release = "7.32.2"
-requests-mock = "1.10.0"
+pytest-env = "0.8.2"
+pytest-factoryboy = "2.5.1"
+pytest-mock = "3.11.1"
+pytest-randomly = "3.13.0"
+python-semantic-release = "7.34.6"
+requests-mock = "1.11.0"
 snapshottest = "0.6.0"
-types-python-dateutil = "2.8.19.4"
-types-requests = "2.28.11.5"
-types-setuptools = "65.5.0.3"
-types-toml = "0.10.8.1"
+types-python-dateutil = "2.8.19.13"
+types-requests = "2.31.0.1"
+types-setuptools = "68.0.0.2"
+types-toml = "0.10.8.6"
 
 [tool.poetry.extras]
 mysql = ["mysqlclient"]
 pgsql = ["psycopg2-binary"]
 databases = ["mysqlclient", "psycopg2-binary"]
 
 [build-system]
```

### Comparing `document_merge_service-6.2.0/PKG-INFO` & `document_merge_service-6.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 Metadata-Version: 2.1
 Name: document-merge-service
-Version: 6.2.0
+Version: 6.2.1
 Summary: Merge Document Template Service
 Home-page: https://github.com/adfinis/document-merge-service
 License: GPL-3.0-or-later
 Author: Adfinis AG
 Author-email: info@adfinis.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: databases
 Provides-Extra: mysql
 Provides-Extra: pgsql
 Requires-Dist: Babel (>=2.11.0,<3.0.0)
-Requires-Dist: Django (>=3.2.16,<4.0.0)
+Requires-Dist: Django (>=3.2.20,<4.0.0)
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: django-cors-headers (>=3.13.0,<4.0.0)
-Requires-Dist: django-environ (>=0.9.0,<0.10.0)
-Requires-Dist: django-filter (>=22.1,<23.0)
+Requires-Dist: django-cors-headers (>=4.2.0,<5.0.0)
+Requires-Dist: django-environ (>=0.10.0,<0.11.0)
+Requires-Dist: django-filter (>=23.2,<24.0)
 Requires-Dist: django-generic-api-permissions (>=0.2.0,<0.3.0)
 Requires-Dist: django-storages (>=1.13.2,<2.0.0)
 Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
 Requires-Dist: docx-mailmerge (>=0.5.0,<0.6.0)
-Requires-Dist: docxtpl (>=0.16.4,<0.17.0)
-Requires-Dist: mysqlclient (>=2.1.1,<3.0.0) ; extra == "mysql" or extra == "databases"
-Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
-Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0) ; extra == "pgsql" or extra == "databases"
+Requires-Dist: docxtpl (>=0.16.7,<0.17.0)
+Requires-Dist: mysqlclient (>=2.2.0,<3.0.0) ; extra == "mysql" or extra == "databases"
+Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0) ; extra == "pgsql" or extra == "databases"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-memcached (>=1.59,<2.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: sentry-sdk (>=1.12.1,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: sentry-sdk (>=1.28.1,<2.0.0)
 Requires-Dist: uWSGI (>=2.0.21,<3.0.0)
-Requires-Dist: xltpl (>=0.16,<0.17)
+Requires-Dist: xltpl (>=0.18,<0.19)
 Project-URL: Documentation, https://github.com/adfinis/document-merge-service/blob/main/README.md
 Project-URL: Repository, https://github.com/adfinis/document-merge-service
 Description-Content-Type: text/markdown
 
 # Document Merge Service
 
 [![Build Status](https://github.com/adfinis/document-merge-service/actions/workflows/tests.yml/badge.svg)](https://github.com/adfinis/document-merge-service/actions/workflows/tests.yml)
@@ -49,38 +48,39 @@
 [![License: GPL-3.0-or-later](https://img.shields.io/github/license/adfinis/document-merge-service)](https://spdx.org/licenses/GPL-3.0-or-later.html)
 
 A document template merge service providing an API to manage templates and merge them with given data.
 
 ## Installation
 
 **Requirements**
-* docker
-* docker-compose
+
+- docker
+- docker-compose
 
 After installing and configuring those, download [docker-compose.yml](https://raw.githubusercontent.com/adfinis/document-merge-service/master/docker-compose.yml) and run the following command:
 
 ```bash
 docker-compose up -d
 ```
 
 You can now access the api at [http://localhost:8000/api/v1/](http://localhost:8000/api/v1/) which includes a browsable api.
 
 ### Workaround LibreOffice lockup
 
-The workaround has a setting called ISOLATE_UNOCONV, it is only enabled in the
-development environment. If ISOLATE_UNOCONV is enabled the container needs
-CAP_SYS_ADMIN. See docker-compose.override.yml.
+The workaround has a setting called `ISOLATE_UNOCONV`, it is only enabled in the
+development environment. If `ISOLATE_UNOCONV` is enabled the container needs
+`CAP_SYS_ADMIN`. See docker-compose.override.yml.
 
 ```yaml
-    cap_add:
-      - CAP_SYS_ADMIN
-    security_opt:
-      - apparmor:unconfined
-    environment:
-      - ISOLATE_UNOCONV=true
+cap_add:
+  - CAP_SYS_ADMIN
+security_opt:
+  - apparmor:unconfined
+environment:
+  - ISOLATE_UNOCONV=true
 ```
 
 ## Getting started
 
 ### Uploading templates
 
 Upload templates using the following:
@@ -93,19 +93,18 @@
 
 After uploading successfully, you can merge a template with the following call:
 
 ```bash
 curl -H "Content-Type: application/json" --data '{"data": {"test": "Test Input"}}' http://localhost:8000/api/v1/template/test-template/merge/ > output.docx
 ```
 
-
 ## Further reading
 
-* [Configuration](CONFIGURATION.md) - Further configuration and how to do a production setup
-* [Usage](USAGE.md) - How to use the DMS and it's features
-* [Contributing](CONTRIBUTING.md) - Look here to see how to start with your first
+- [Configuration](CONFIGURATION.md) - Further configuration and how to do a production setup
+- [Usage](USAGE.md) - How to use the DMS and it's features
+- [Contributing](CONTRIBUTING.md) - Look here to see how to start with your first
   contribution. Contributions are welcome!
 
 ## License
 
 Code released under the [GPL-3.0-or-later license](LICENSE).
```

