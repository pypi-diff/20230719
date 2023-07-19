# Comparing `tmp/aleksis_app_resint-3.0b2.tar.gz` & `tmp/aleksis_app_resint-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_resint-3.0b2.tar", max compression
+gzip compressed data, was "aleksis_app_resint-3.1.tar", max compression
```

## Comparing `aleksis_app_resint-3.0b2.tar` & `aleksis_app_resint-3.1.tar`

### file list

```diff
@@ -1,72 +1,74 @@
--rw-r--r--   0        0        0     2652 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/LICENCE.rst
--rw-r--r--   0        0        0     1596 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/README.rst
--rw-r--r--   0        0        0      214 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/__init__.py
--rw-r--r--   0        0        0      517 2023-03-20 17:25:05.537333 aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      489 2023-03-20 17:25:06.629331 aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0     2624 2023-03-20 17:25:05.949332 aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0    16275 2023-03-20 17:25:06.569331 aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     5858 2023-03-20 17:25:06.641331 aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0      136 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/admin.py
--rw-r--r--   0        0        0     1508 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/apps.py
--rw-r--r--   0        0        0     1226 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/forms.py
--rw-r--r--   0        0        0     4975 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/frontend/index.js
--rw-r--r--   0        0        0      263 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/frontend/messages/de.json
--rw-r--r--   0        0        0      254 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/frontend/messages/en.json
--rw-r--r--   0        0        0      463 2023-03-20 17:25:06.833330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7819 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4985 2023-03-20 17:25:06.841330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9987 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-03-20 17:25:06.841330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7735 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-20 17:25:06.845330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7689 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-20 17:25:06.845330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7689 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6180 2023-03-20 17:25:06.841330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10692 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-20 17:25:06.841330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7689 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6291 2023-03-20 17:25:06.845330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10806 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4747 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0001_initial.py
--rw-r--r--   0        0        0      605 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0002_permissions.py
--rw-r--r--   0        0        0      549 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0003_group_in_unique_constraint.py
--rw-r--r--   0        0        0      692 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0004_edit_permission.py
--rw-r--r--   0        0        0      681 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0005_fix_permissions.py
--rw-r--r--   0        0        0     1847 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0006_livedocument.py
--rw-r--r--   0        0        0      510 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0007_current_file_not_null.py
--rw-r--r--   0        0        0        0 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/__init__.py
--rw-r--r--   0        0        0     9460 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/models.py
--rw-r--r--   0        0        0     4957 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/rules.py
--rw-r--r--   0        0        0     1187 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/tables.py
--rw-r--r--   0        0        0      464 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/group/create.html
--rw-r--r--   0        0        0      418 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/group/edit.html
--rw-r--r--   0        0        0     2675 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/group/list.html
--rw-r--r--   0        0        0      642 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/create.html
--rw-r--r--   0        0        0      640 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/edit.html
--rw-r--r--   0        0        0     1214 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/list.html
--rw-r--r--   0        0        0      406 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/poster/edit.html
--rw-r--r--   0        0        0     3361 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/poster/list.html
--rw-r--r--   0        0        0      537 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/poster/upload.html
--rw-r--r--   0        0        0     1929 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/urls.py
--rw-r--r--   0        0        0     9180 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/views.py
--rw-r--r--   0        0        0      581 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/docs/Makefile
--rw-r--r--   0        0        0   154961 2023-03-20 17:18:45.881957 aleksis_app_resint-3.0b2/docs/_static/create_live_document.png
--rw-r--r--   0        0        0   164973 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/_static/create_poster_group.png
--rw-r--r--   0        0        0   180288 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/_static/manage_posters_list.png
--rw-r--r--   0        0        0   137796 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/_static/upload_poster.png
--rw-r--r--   0        0        0      116 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/admin/00_index.rst
--rw-r--r--   0        0        0     1868 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/admin/01_poster_groups.rst
--rw-r--r--   0        0        0      972 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/admin/02_live_documents.rst
--rw-r--r--   0        0        0     6399 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/conf.py
--rw-r--r--   0        0        0      120 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/dev/00_index.rst
--rw-r--r--   0        0        0     1753 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/dev/01_live_document_types.rst
--rw-r--r--   0        0        0      526 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/index.rst
--rw-r--r--   0        0        0      787 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/make.bat
--rw-r--r--   0        0        0       96 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/user/00_index.rst
--rw-r--r--   0        0        0     1007 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/user/01_posters.rst
--rw-r--r--   0        0        0     1552 2023-03-20 17:23:24.865499 aleksis_app_resint-3.0b2/pyproject.toml
--rw-r--r--   0        0        0     2730 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/tox.ini
--rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 aleksis_app_resint-3.0b2/setup.py
--rw-r--r--   0        0        0     2534 1970-01-01 00:00:00.000000 aleksis_app_resint-3.0b2/PKG-INFO
+-rw-r--r--   0        0        0     3004 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/LICENCE.rst
+-rw-r--r--   0        0        0     1596 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/README.rst
+-rw-r--r--   0        0        0      214 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/aleksis/apps/resint/__init__.py
+-rw-r--r--   0        0        0      517 2023-07-19 07:11:11.422247 aleksis_app_resint-3.1/aleksis/apps/resint/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      489 2023-07-19 07:11:15.174388 aleksis_app_resint-3.1/aleksis/apps/resint/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0     2624 2023-07-19 07:11:13.038308 aleksis_app_resint-3.1/aleksis/apps/resint/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0    16378 2023-07-19 07:11:14.966380 aleksis_app_resint-3.1/aleksis/apps/resint/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     5898 2023-07-19 07:11:15.198389 aleksis_app_resint-3.1/aleksis/apps/resint/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0      136 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/aleksis/apps/resint/admin.py
+-rw-r--r--   0        0        0     1508 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/aleksis/apps/resint/apps.py
+-rw-r--r--   0        0        0     1226 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/aleksis/apps/resint/forms.py
+-rw-r--r--   0        0        0     4103 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/aleksis/apps/resint/frontend/index.js
+-rw-r--r--   0        0        0      263 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/aleksis/apps/resint/frontend/messages/de.json
+-rw-r--r--   0        0        0      254 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/aleksis/apps/resint/frontend/messages/en.json
+-rw-r--r--   0        0        0      329 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/aleksis/apps/resint/frontend/messages/ru.json
+-rw-r--r--   0        0        0      325 2023-07-19 07:09:12.977812 aleksis_app_resint-3.1/aleksis/apps/resint/frontend/messages/uk.json
+-rw-r--r--   0        0        0      463 2023-07-19 07:11:15.814412 aleksis_app_resint-3.1/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7819 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4985 2023-07-19 07:11:15.814412 aleksis_app_resint-3.1/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9987 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-07-19 07:11:15.810412 aleksis_app_resint-3.1/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7735 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-19 07:11:15.822412 aleksis_app_resint-3.1/aleksis/apps/resint/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7689 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-19 07:11:15.814412 aleksis_app_resint-3.1/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7689 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6193 2023-07-19 07:11:15.818412 aleksis_app_resint-3.1/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10696 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-19 07:11:15.818412 aleksis_app_resint-3.1/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7689 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6291 2023-07-19 07:11:15.814412 aleksis_app_resint-3.1/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10806 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4747 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0001_initial.py
+-rw-r--r--   0        0        0      605 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0002_permissions.py
+-rw-r--r--   0        0        0      549 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0003_group_in_unique_constraint.py
+-rw-r--r--   0        0        0      692 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0004_edit_permission.py
+-rw-r--r--   0        0        0      681 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0005_fix_permissions.py
+-rw-r--r--   0        0        0     1847 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0006_livedocument.py
+-rw-r--r--   0        0        0      510 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0007_current_file_not_null.py
+-rw-r--r--   0        0        0      441 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0008_public_live_documents.py
+-rw-r--r--   0        0        0        0 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/migrations/__init__.py
+-rw-r--r--   0        0        0     9556 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/models.py
+-rw-r--r--   0        0        0     4979 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/rules.py
+-rw-r--r--   0        0        0     1187 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/tables.py
+-rw-r--r--   0        0        0      464 2023-07-19 07:09:12.981812 aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/group/create.html
+-rw-r--r--   0        0        0      418 2023-07-19 07:09:12.985812 aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/group/edit.html
+-rw-r--r--   0        0        0     2675 2023-07-19 07:09:12.985812 aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/group/list.html
+-rw-r--r--   0        0        0      642 2023-07-19 07:09:12.985812 aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/live_document/create.html
+-rw-r--r--   0        0        0      640 2023-07-19 07:09:12.985812 aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/live_document/edit.html
+-rw-r--r--   0        0        0     1214 2023-07-19 07:09:12.985812 aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/live_document/list.html
+-rw-r--r--   0        0        0      406 2023-07-19 07:09:12.985812 aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/poster/edit.html
+-rw-r--r--   0        0        0     3361 2023-07-19 07:09:12.985812 aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/poster/list.html
+-rw-r--r--   0        0        0      537 2023-07-19 07:09:12.985812 aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/poster/upload.html
+-rw-r--r--   0        0        0     1952 2023-07-19 07:09:12.985812 aleksis_app_resint-3.1/aleksis/apps/resint/urls.py
+-rw-r--r--   0        0        0     9180 2023-07-19 07:09:12.985812 aleksis_app_resint-3.1/aleksis/apps/resint/views.py
+-rw-r--r--   0        0        0      581 2023-07-19 07:09:12.985812 aleksis_app_resint-3.1/docs/Makefile
+-rw-r--r--   0        0        0   154961 2023-07-19 07:09:12.989812 aleksis_app_resint-3.1/docs/_static/create_live_document.png
+-rw-r--r--   0        0        0   164973 2023-07-19 07:09:12.989812 aleksis_app_resint-3.1/docs/_static/create_poster_group.png
+-rw-r--r--   0        0        0   180288 2023-07-19 07:09:12.993812 aleksis_app_resint-3.1/docs/_static/manage_posters_list.png
+-rw-r--r--   0        0        0   137796 2023-07-19 07:09:12.993812 aleksis_app_resint-3.1/docs/_static/upload_poster.png
+-rw-r--r--   0        0        0      116 2023-07-19 07:09:12.993812 aleksis_app_resint-3.1/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     1868 2023-07-19 07:09:12.993812 aleksis_app_resint-3.1/docs/admin/01_poster_groups.rst
+-rw-r--r--   0        0        0      972 2023-07-19 07:09:12.997812 aleksis_app_resint-3.1/docs/admin/02_live_documents.rst
+-rw-r--r--   0        0        0     6397 2023-07-19 07:09:12.997812 aleksis_app_resint-3.1/docs/conf.py
+-rw-r--r--   0        0        0      120 2023-07-19 07:09:12.997812 aleksis_app_resint-3.1/docs/dev/00_index.rst
+-rw-r--r--   0        0        0     1753 2023-07-19 07:09:12.997812 aleksis_app_resint-3.1/docs/dev/01_live_document_types.rst
+-rw-r--r--   0        0        0      526 2023-07-19 07:09:12.997812 aleksis_app_resint-3.1/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-07-19 07:09:12.997812 aleksis_app_resint-3.1/docs/make.bat
+-rw-r--r--   0        0        0       96 2023-07-19 07:09:12.997812 aleksis_app_resint-3.1/docs/user/00_index.rst
+-rw-r--r--   0        0        0     1007 2023-07-19 07:09:12.997812 aleksis_app_resint-3.1/docs/user/01_posters.rst
+-rw-r--r--   0        0        0     2393 2023-07-19 07:09:40.106828 aleksis_app_resint-3.1/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-07-19 07:09:12.997812 aleksis_app_resint-3.1/tox.ini
+-rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 aleksis_app_resint-3.1/PKG-INFO
```

### Comparing `aleksis_app_resint-3.0b2/CHANGELOG.rst` & `aleksis_app_resint-3.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,32 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
+`3.1`_ – 2023-07-17
+-------------------
+
+Added
+~~~~~
+
+* Support public live documents
+
+Fixed
+~~~~~
+
+* API urls were in the wrong namespace.
+
+`3.0`_ - 2023-05-12
+-------------------
+
+Nothing changed.
+
 `3.0b2`_ - 2023-03-20
 ---------------------
 
 Fixed
 ~~~~~
 
 * Menu item was shown for all users independent of permissions.
@@ -101,7 +119,9 @@
 .. _2.0b1: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/2.0b1
 .. _2.0: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/2.0
 .. _2.1: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/2.1
 .. _2.2: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/2.2
 .. _3.0b0: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/3.0b0
 .. _3.0b1: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/3.0b1
 .. _3.0b2: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/3.0b2
+.. _3.0: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/3.0
+.. _3.1: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/3.1
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aleksis_app_resint-3.0b2/LICENCE.rst` & `aleksis_app_resint-3.1/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/README.rst` & `aleksis_app_resint-3.1/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/__init__.cpython-311.pyc` & `aleksis_app_resint-3.1/aleksis/apps/resint/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x75951864 (Mon Mar 20 17:18:45 2023 UTC)
+moddate:  0x188cb764 (Wed Jul 19 07:09:12 2023 UTC)
 files sz: 214
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/apps.cpython-311.pyc` & `aleksis_app_resint-3.1/aleksis/apps/resint/__pycache__/apps.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x75951864 (Mon Mar 20 17:18:45 2023 UTC)
+moddate:  0x188cb764 (Wed Jul 19 07:09:12 2023 UTC)
 files sz: 1508
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/models.cpython-311.pyc` & `aleksis_app_resint-3.1/aleksis/apps/resint/__pycache__/models.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x75951864 (Mon Mar 20 17:18:45 2023 UTC)
-files sz: 9460
+moddate:  0x188cb764 (Wed Jul 19 07:09:12 2023 UTC)
+files sz: 9556
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d005a000100640064026c016d025a026d035a0301
@@ -1498,27 +1498,29 @@
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364025a0464035a05020065066a
             070000000000000000020065086404a6010000ab01000000000000000002
             0065086405a6010000ab010000000000000000ac06a6020000ab02000000
             00000000005a09020065066a0a00000000000000006407020065086408a6
             010000ab010000000000000000ac09a6020000ab0200000000000000005a
-            0b020065066a0c0000000000000000640a640b02006508640ca6010000ab
-            010000000000000000640dac0ea6040000ab0400000000000000005a0d02
-            0065066a0e0000000000000000640d02006508640fa6010000ab01000000
-            0000000000640dac10a6030000ab0300000000000000005a0f6510641165
-            11651219000000000000000000660264128404a6000000ab000000000000
-            0000005a13651064116511651419000000000000000000660264138404a6
-            000000ab0000000000000000005a15641165116516190000000000000000
-            006602641484045a17651064116518660264158404a6000000ab00000000
-            00000000005a19651064116518660264168404a6000000ab000000000000
-            0000005a1a88006601641784085a1b6411651c6518651d66021900000000
-            00000000006602641884045a1e641e6419651f6602641a84055a20641165
-            186602641b84045a2102004700641c8400641da6020000ab020000000000
-            0000005a22880078015a235300
+            0b020065066a0c0000000000000000640a02006508640ba6010000ab0100
+            00000000000000ac0ca6020000ab0200000000000000005a0d020065066a
+            0e0000000000000000640d640e02006508640fa6010000ab010000000000
+            000000640aac10a6040000ab0400000000000000005a0f020065066a0c00
+            00000000000000640a020065086411a6010000ab01000000000000000064
+            0aac12a6030000ab0300000000000000005a1002004700641384006414a6
+            020000ab0200000000000000005a11641565126602641684045a13880066
+            01641784085a146515641565166517190000000000000000006602641884
+            04a6000000ab0000000000000000005a1865156415651665191900000000
+            0000000000660264198404a6000000ab0000000000000000005a1a641565
+            16651b190000000000000000006602641a84045a1c651564156512660264
+            1b8404a6000000ab0000000000000000005a1d6515641565126602641c84
+            04a6000000ab0000000000000000005a1e6415651f651265206602190000
+            000000000000006602641d84045a216420641e65226602641f84055a2388
+            0078015a245300
                        0 MAKE_CELL                0 (__class__)
          
          187           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('LiveDocument')
                       10 STORE_NAME               2 (__qualname__)
@@ -1563,338 +1565,487 @@
                      118 PRECALL                  1
                      122 CALL                     1
                      132 KW_NAMES                 9
                      134 PRECALL                  2
                      138 CALL                     2
                      148 STORE_NAME              11 (name)
          
-         200         150 PUSH_NULL
+         199         150 PUSH_NULL
                      152 LOAD_NAME                6 (models)
-                     154 LOAD_ATTR               12 (FileField)
-         
-         201         164 LOAD_CONST              10 ('live_documents/')
-         
-         202         166 LOAD_CONST              11 (True)
-         
-         203         168 PUSH_NULL
-                     170 LOAD_NAME                8 (_)
-                     172 LOAD_CONST              12 ('Current file')
-                     174 PRECALL                  1
-                     178 CALL                     1
-         
-         204         188 LOAD_CONST              13 (False)
-         
-         200         190 KW_NAMES                14
-                     192 PRECALL                  4
-                     196 CALL                     4
-                     206 STORE_NAME              13 (current_file)
-         
-         206         208 PUSH_NULL
-                     210 LOAD_NAME                6 (models)
-                     212 LOAD_ATTR               14 (BooleanField)
-         
-         207         222 LOAD_CONST              13 (False)
-                     224 PUSH_NULL
-                     226 LOAD_NAME                8 (_)
-                     228 LOAD_CONST              15 ('Was the last update triggered manually?')
-                     230 PRECALL                  1
-                     234 CALL                     1
-                     244 LOAD_CONST              13 (False)
+                     154 LOAD_ATTR               12 (BooleanField)
+                     164 LOAD_CONST              10 (False)
+                     166 PUSH_NULL
+                     168 LOAD_NAME                8 (_)
+                     170 LOAD_CONST              11 ('Show for not logged-in users')
+                     172 PRECALL                  1
+                     176 CALL                     1
+                     186 KW_NAMES                12
+                     188 PRECALL                  2
+                     192 CALL                     2
+                     202 STORE_NAME              13 (public)
+         
+         201         204 PUSH_NULL
+                     206 LOAD_NAME                6 (models)
+                     208 LOAD_ATTR               14 (FileField)
+         
+         202         218 LOAD_CONST              13 ('live_documents/')
+         
+         203         220 LOAD_CONST              14 (True)
+         
+         204         222 PUSH_NULL
+                     224 LOAD_NAME                8 (_)
+                     226 LOAD_CONST              15 ('Current file')
+                     228 PRECALL                  1
+                     232 CALL                     1
+         
+         205         242 LOAD_CONST              10 (False)
+         
+         201         244 KW_NAMES                16
+                     246 PRECALL                  4
+                     250 CALL                     4
+                     260 STORE_NAME              15 (current_file)
+         
+         207         262 PUSH_NULL
+                     264 LOAD_NAME                6 (models)
+                     266 LOAD_ATTR               12 (BooleanField)
+         
+         208         276 LOAD_CONST              10 (False)
+                     278 PUSH_NULL
+                     280 LOAD_NAME                8 (_)
+                     282 LOAD_CONST              17 ('Was the last update triggered manually?')
+                     284 PRECALL                  1
+                     288 CALL                     1
+                     298 LOAD_CONST              10 (False)
          
-         206         246 KW_NAMES                16
-                     248 PRECALL                  3
-                     252 CALL                     3
-                     262 STORE_NAME              15 (last_update_triggered_manually)
-         
-         210         264 LOAD_NAME               16 (property)
-         
-         211         266 LOAD_CONST              17 ('return')
-                     268 LOAD_NAME               17 (Optional)
-                     270 LOAD_NAME               18 (Revision)
-                     272 BINARY_SUBSCR
-                     282 BUILD_TUPLE              2
-                     284 LOAD_CONST              18 (<code object last_version, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 210>)
-                     286 MAKE_FUNCTION            4 (annotations)
-         
-         210         288 PRECALL                  0
-                     292 CALL                     0
-         
-         211         302 STORE_NAME              19 (last_version)
-         
-         218         304 LOAD_NAME               16 (property)
-         
-         219         306 LOAD_CONST              17 ('return')
-                     308 LOAD_NAME               17 (Optional)
-                     310 LOAD_NAME               20 (datetime)
-                     312 BINARY_SUBSCR
-                     322 BUILD_TUPLE              2
-                     324 LOAD_CONST              19 (<code object last_update, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 218>)
-                     326 MAKE_FUNCTION            4 (annotations)
-         
-         218         328 PRECALL                  0
-                     332 CALL                     0
-         
-         219         342 STORE_NAME              21 (last_update)
-         
-         226         344 LOAD_CONST              17 ('return')
-                     346 LOAD_NAME               17 (Optional)
-                     348 LOAD_NAME               22 (File)
-                     350 BINARY_SUBSCR
-                     360 BUILD_TUPLE              2
-                     362 LOAD_CONST              20 (<code object get_current_file, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 226>)
-                     364 MAKE_FUNCTION            4 (annotations)
-                     366 STORE_NAME              23 (get_current_file)
-         
-         232         368 LOAD_NAME               16 (property)
-         
-         233         370 LOAD_CONST              17 ('return')
-                     372 LOAD_NAME               24 (str)
-                     374 BUILD_TUPLE              2
-                     376 LOAD_CONST              21 (<code object filename, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 232>)
-                     378 MAKE_FUNCTION            4 (annotations)
-         
-         232         380 PRECALL                  0
-                     384 CALL                     0
-         
-         233         394 STORE_NAME              25 (filename)
-         
-         237         396 LOAD_NAME               16 (property)
-         
-         238         398 LOAD_CONST              17 ('return')
-                     400 LOAD_NAME               24 (str)
-                     402 BUILD_TUPLE              2
-                     404 LOAD_CONST              22 (<code object scope, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 237>)
-                     406 MAKE_FUNCTION            4 (annotations)
-         
-         237         408 PRECALL                  0
-                     412 CALL                     0
-         
-         238         422 STORE_NAME              26 (scope)
-         
-         242         424 LOAD_CLOSURE             0 (__class__)
-                     426 BUILD_TUPLE              1
-                     428 LOAD_CONST              23 (<code object save, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 242>)
-                     430 MAKE_FUNCTION            8 (closure)
-                     432 STORE_NAME              27 (save)
-         
-         246         434 LOAD_CONST              17 ('return')
-                     436 LOAD_NAME               28 (dict)
-                     438 LOAD_NAME               24 (str)
-                     440 LOAD_NAME               29 (Any)
-                     442 BUILD_TUPLE              2
-                     444 BINARY_SUBSCR
-                     454 BUILD_TUPLE              2
-                     456 LOAD_CONST              24 (<code object get_context_data, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 246>)
-                     458 MAKE_FUNCTION            4 (annotations)
-                     460 STORE_NAME              30 (get_context_data)
-         
-         250         462 LOAD_CONST              30 ((True,))
-                     464 LOAD_CONST              25 ('triggered_manually')
-                     466 LOAD_NAME               31 (bool)
-                     468 BUILD_TUPLE              2
-                     470 LOAD_CONST              26 (<code object update, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 250>)
-                     472 MAKE_FUNCTION            5 (defaults, annotations)
-                     474 STORE_NAME              32 (update)
-         
-         267         476 LOAD_CONST              17 ('return')
-                     478 LOAD_NAME               24 (str)
-                     480 BUILD_TUPLE              2
-                     482 LOAD_CONST              27 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 267>)
-                     484 MAKE_FUNCTION            4 (annotations)
-                     486 STORE_NAME              33 (__str__)
-         
-         270         488 PUSH_NULL
-                     490 LOAD_BUILD_CLASS
-                     492 LOAD_CONST              28 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 270>)
-                     494 MAKE_FUNCTION            0
-                     496 LOAD_CONST              29 ('Meta')
-                     498 PRECALL                  2
-                     502 CALL                     2
-                     512 STORE_NAME              34 (Meta)
-                     514 LOAD_CLOSURE             0 (__class__)
-                     516 COPY                     1
-                     518 STORE_NAME              35 (__classcell__)
-                     520 RETURN_VALUE
+         207         300 KW_NAMES                18
+                     302 PRECALL                  3
+                     306 CALL                     3
+                     316 STORE_NAME              16 (last_update_triggered_manually)
+         
+         211         318 PUSH_NULL
+                     320 LOAD_BUILD_CLASS
+                     322 LOAD_CONST              19 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 211>)
+                     324 MAKE_FUNCTION            0
+                     326 LOAD_CONST              20 ('Meta')
+                     328 PRECALL                  2
+                     332 CALL                     2
+                     342 STORE_NAME              17 (Meta)
+         
+         215         344 LOAD_CONST              21 ('return')
+                     346 LOAD_NAME               18 (str)
+                     348 BUILD_TUPLE              2
+                     350 LOAD_CONST              22 (<code object __str__, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 215>)
+                     352 MAKE_FUNCTION            4 (annotations)
+                     354 STORE_NAME              19 (__str__)
+         
+         218         356 LOAD_CLOSURE             0 (__class__)
+                     358 BUILD_TUPLE              1
+                     360 LOAD_CONST              23 (<code object save, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 218>)
+                     362 MAKE_FUNCTION            8 (closure)
+                     364 STORE_NAME              20 (save)
+         
+         222         366 LOAD_NAME               21 (property)
+         
+         223         368 LOAD_CONST              21 ('return')
+                     370 LOAD_NAME               22 (Optional)
+                     372 LOAD_NAME               23 (Revision)
+                     374 BINARY_SUBSCR
+                     384 BUILD_TUPLE              2
+                     386 LOAD_CONST              24 (<code object last_version, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 222>)
+                     388 MAKE_FUNCTION            4 (annotations)
+         
+         222         390 PRECALL                  0
+                     394 CALL                     0
+         
+         223         404 STORE_NAME              24 (last_version)
+         
+         230         406 LOAD_NAME               21 (property)
+         
+         231         408 LOAD_CONST              21 ('return')
+                     410 LOAD_NAME               22 (Optional)
+                     412 LOAD_NAME               25 (datetime)
+                     414 BINARY_SUBSCR
+                     424 BUILD_TUPLE              2
+                     426 LOAD_CONST              25 (<code object last_update, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 230>)
+                     428 MAKE_FUNCTION            4 (annotations)
+         
+         230         430 PRECALL                  0
+                     434 CALL                     0
+         
+         231         444 STORE_NAME              26 (last_update)
+         
+         238         446 LOAD_CONST              21 ('return')
+                     448 LOAD_NAME               22 (Optional)
+                     450 LOAD_NAME               27 (File)
+                     452 BINARY_SUBSCR
+                     462 BUILD_TUPLE              2
+                     464 LOAD_CONST              26 (<code object get_current_file, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 238>)
+                     466 MAKE_FUNCTION            4 (annotations)
+                     468 STORE_NAME              28 (get_current_file)
+         
+         244         470 LOAD_NAME               21 (property)
+         
+         245         472 LOAD_CONST              21 ('return')
+                     474 LOAD_NAME               18 (str)
+                     476 BUILD_TUPLE              2
+                     478 LOAD_CONST              27 (<code object filename, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 244>)
+                     480 MAKE_FUNCTION            4 (annotations)
+         
+         244         482 PRECALL                  0
+                     486 CALL                     0
+         
+         245         496 STORE_NAME              29 (filename)
+         
+         249         498 LOAD_NAME               21 (property)
+         
+         250         500 LOAD_CONST              21 ('return')
+                     502 LOAD_NAME               18 (str)
+                     504 BUILD_TUPLE              2
+                     506 LOAD_CONST              28 (<code object scope, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 249>)
+                     508 MAKE_FUNCTION            4 (annotations)
+         
+         249         510 PRECALL                  0
+                     514 CALL                     0
+         
+         250         524 STORE_NAME              30 (scope)
+         
+         254         526 LOAD_CONST              21 ('return')
+                     528 LOAD_NAME               31 (dict)
+                     530 LOAD_NAME               18 (str)
+                     532 LOAD_NAME               32 (Any)
+                     534 BUILD_TUPLE              2
+                     536 BINARY_SUBSCR
+                     546 BUILD_TUPLE              2
+                     548 LOAD_CONST              29 (<code object get_context_data, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 254>)
+                     550 MAKE_FUNCTION            4 (annotations)
+                     552 STORE_NAME              33 (get_context_data)
+         
+         258         554 LOAD_CONST              32 ((True,))
+                     556 LOAD_CONST              30 ('triggered_manually')
+                     558 LOAD_NAME               34 (bool)
+                     560 BUILD_TUPLE              2
+                     562 LOAD_CONST              31 (<code object update, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py", line 258>)
+                     564 MAKE_FUNCTION            5 (defaults, annotations)
+                     566 STORE_NAME              35 (update)
+                     568 LOAD_CLOSURE             0 (__class__)
+                     570 COPY                     1
+                     572 STORE_NAME              36 (__classcell__)
+                     574 RETURN_VALUE
          consts
             'LiveDocument'
             'Model for periodically/automatically updated files.'
             'live_document_pdf'
             None
             'Slug'
             'This will be used for the name of the current PDF file.'
             ('verbose_name', 'help_text')
             255
             'Name'
             ('max_length', 'verbose_name')
+            False
+            'Show for not logged-in users'
+            ('default', 'verbose_name')
             'live_documents/'
             True
             'Current file'
-            False
             ('upload_to', 'blank', 'verbose_name', 'editable')
             'Was the last update triggered manually?'
             ('default', 'verbose_name', 'editable')
+            code
+               argcount  : 0
+               nlocals   : 0
+               stacksize : 3
+               flags     : 0
+               code
+                  0x970065005a0164005a02020065036401a6010000ab0100000000000000
+                  005a04020065036402a6010000ab0100000000000000005a0564035300
+               211           0 RESUME                   0
+                             2 LOAD_NAME                0 (__name__)
+                             4 STORE_NAME               1 (__module__)
+                             6 LOAD_CONST               0 ('LiveDocument.Meta')
+                             8 STORE_NAME               2 (__qualname__)
+               
+               212          10 PUSH_NULL
+                            12 LOAD_NAME                3 (_)
+                            14 LOAD_CONST               1 ('Live document')
+                            16 PRECALL                  1
+                            20 CALL                     1
+                            30 STORE_NAME               4 (verbose_name)
+               
+               213          32 PUSH_NULL
+                            34 LOAD_NAME                3 (_)
+                            36 LOAD_CONST               2 ('Live documents')
+                            38 PRECALL                  1
+                            42 CALL                     1
+                            52 STORE_NAME               5 (verbose_name_plural)
+                            54 LOAD_CONST               3 (None)
+                            56 RETURN_VALUE
+               consts
+                  'LiveDocument.Meta'
+                  'Live document'
+                  'Live documents'
+                  None
+               names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
+               varnames   ()
+               freevars   ()
+               cellvars   ()
+               filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
+               name       'Meta'
+               firstlineno 211
+               lnotab 0x0a011601
+            'Meta'
             'return'
             code
                argcount  : 1
+               nlocals   : 1
+               stacksize : 1
+               flags     : 3
+               code 0x97007c006a0000000000000000005300
+               215           0 RESUME                   0
+               
+               216           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (name)
+                            14 RETURN_VALUE
+               consts
+                  None
+               names      ('name',)
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
+               name       '__str__'
+               firstlineno 215
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 6
+               flags     : 15
+               code
+                  0x950197007401000000000000000000006a010000000000000000a60000
+                  00ab000000000000000000350001000200740500000000000000000000a6
+                  000000ab0000000000000000006a0300000000000000007c0169007c02a4
+                  018e010100640064006400a6020000ab0200000000000000000100640053
+                  002300310073047702780359007701010059000100010064005300
+                             0 COPY_FREE_VARS           1
+               
+               218           2 RESUME                   0
+               
+               219           4 LOAD_GLOBAL              1 (NULL + reversion)
+                            16 LOAD_ATTR                1 (create_revision)
+                            26 PRECALL                  0
+                            30 CALL                     0
+                            40 BEFORE_WITH
+                            42 POP_TOP
+               
+               220          44 PUSH_NULL
+                            46 LOAD_GLOBAL              5 (NULL + super)
+                            58 PRECALL                  0
+                            62 CALL                     0
+                            72 LOAD_ATTR                3 (save)
+                            82 LOAD_FAST                1 (args)
+                            84 BUILD_MAP                0
+                            86 LOAD_FAST                2 (kwargs)
+                            88 DICT_MERGE               1
+                            90 CALL_FUNCTION_EX         1
+                            92 POP_TOP
+               
+               219          94 LOAD_CONST               0 (None)
+                            96 LOAD_CONST               0 (None)
+                            98 LOAD_CONST               0 (None)
+                           100 PRECALL                  2
+                           104 CALL                     2
+                           114 POP_TOP
+                           116 LOAD_CONST               0 (None)
+                           118 RETURN_VALUE
+                       >>  120 PUSH_EXC_INFO
+                           122 WITH_EXCEPT_START
+                           124 POP_JUMP_FORWARD_IF_TRUE     4 (to 134)
+                           126 RERAISE                  2
+                       >>  128 COPY                     3
+                           130 POP_EXCEPT
+                           132 RERAISE                  1
+                       >>  134 POP_TOP
+                           136 POP_EXCEPT
+                           138 POP_TOP
+                           140 POP_TOP
+                           142 LOAD_CONST               0 (None)
+                           144 RETURN_VALUE
+               ExceptionTable:
+                 42 to 92 -> 120 [1] lasti
+                 120 to 126 -> 128 [3] lasti
+                 134 to 134 -> 128 [3] lasti
+               consts
+                  None
+               names      ('reversion', 'create_revision', 'super', 'save')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ('__class__',)
+               cellvars   ()
+               filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
+               name       'save'
+               firstlineno 218
+               lnotab 0x0401280132ff
+            code
+               argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c00a6010000ab010000000000
                   000000a00300000000000000000000000000000000000000006401a60100
                   00ab0100000000000000007d017c01a00400000000000000000000000000
                   00000000000000a6000000ab00000000000000000072147c01a005000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   00530064025300
-               210           0 RESUME                   0
+               222           0 RESUME                   0
                
-               213           2 LOAD_GLOBAL              0 (Version)
+               225           2 LOAD_GLOBAL              0 (Version)
                             14 LOAD_ATTR                1 (objects)
                             24 LOAD_METHOD              2 (get_for_object)
                             46 LOAD_FAST                0 (self)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 LOAD_METHOD              3 (order_by)
                             84 LOAD_CONST               1 ('revision__date_created')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 STORE_FAST               1 (versions)
                
-               214         102 LOAD_FAST                1 (versions)
+               226         102 LOAD_FAST                1 (versions)
                            104 LOAD_METHOD              4 (exists)
                            126 PRECALL                  0
                            130 CALL                     0
                            140 POP_JUMP_FORWARD_IF_FALSE    20 (to 182)
                
-               215         142 LOAD_FAST                1 (versions)
+               227         142 LOAD_FAST                1 (versions)
                            144 LOAD_METHOD              5 (last)
                            166 PRECALL                  0
                            170 CALL                     0
                            180 RETURN_VALUE
                
-               216     >>  182 LOAD_CONST               2 (None)
+               228     >>  182 LOAD_CONST               2 (None)
                            184 RETURN_VALUE
                consts
                   'Get django-reversion version of last file update.'
                   'revision__date_created'
                   None
                names      ('Version', 'objects', 'get_for_object', 'order_by', 'exists', 'last')
                varnames   ('self', 'versions')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
                name       'last_version'
-               firstlineno 210
+               firstlineno 222
                lnotab 0x0203640128012801
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code
                   0x97007c006a0000000000000000007d017c01720c7c016a010000000000
                   0000006a020000000000000000530064015300
-               218           0 RESUME                   0
+               230           0 RESUME                   0
                
-               221           2 LOAD_FAST                0 (self)
+               233           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (last_version)
                             14 STORE_FAST               1 (last_version)
                
-               222          16 LOAD_FAST                1 (last_version)
+               234          16 LOAD_FAST                1 (last_version)
                             18 POP_JUMP_FORWARD_IF_FALSE    12 (to 44)
                
-               223          20 LOAD_FAST                1 (last_version)
+               235          20 LOAD_FAST                1 (last_version)
                             22 LOAD_ATTR                1 (revision)
                             32 LOAD_ATTR                2 (date_created)
                             42 RETURN_VALUE
                
-               224     >>   44 LOAD_CONST               1 (None)
+               236     >>   44 LOAD_CONST               1 (None)
                             46 RETURN_VALUE
                consts
                   'Get datetime of last file update.'
                   None
                names      ('last_version', 'revision', 'date_created')
                varnames   ('self', 'last_version')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
                name       'last_update'
-               firstlineno 218
+               firstlineno 230
                lnotab 0x02030e0104011801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a00000000000000000073147c00a001000000000000000000
                   0000000000000000000000a6000000ab00000000000000000001007c006a
                   0000000000000000005300
-               226           0 RESUME                   0
+               238           0 RESUME                   0
                
-               228           2 LOAD_FAST                0 (self)
+               240           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (current_file)
                             14 POP_JUMP_FORWARD_IF_TRUE    20 (to 56)
                
-               229          16 LOAD_FAST                0 (self)
+               241          16 LOAD_FAST                0 (self)
                             18 LOAD_METHOD              1 (update)
                             40 PRECALL                  0
                             44 CALL                     0
                             54 POP_TOP
                
-               230     >>   56 LOAD_FAST                0 (self)
+               242     >>   56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                0 (current_file)
                             68 RETURN_VALUE
                consts
                   'Get current file.'
                names      ('current_file', 'update')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
                name       'get_current_file'
-               firstlineno 226
+               firstlineno 238
                lnotab 0x02020e012801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code 0x97007c006a0000000000000000009b0064019d025300
-               232           0 RESUME                   0
+               244           0 RESUME                   0
                
-               235           2 LOAD_FAST                0 (self)
+               247           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (slug)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 ('.pdf')
                             18 BUILD_STRING             2
                             20 RETURN_VALUE
                consts
                   'Get the filename without path of the PDF file.'
                   '.pdf'
                names      ('slug',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
                name       'filename'
-               firstlineno 232
+               firstlineno 244
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b009d035300
-               237           0 RESUME                   0
+               249           0 RESUME                   0
                
-               240           2 LOAD_FAST                0 (self)
+               252           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (SCOPE_PREFIX)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 ('_')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (slug)
                             30 FORMAT_VALUE             0
                             32 BUILD_STRING             3
@@ -1904,104 +2055,35 @@
                   '_'
                names      ('SCOPE_PREFIX', 'slug')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
                name       'scope'
-               firstlineno 237
+               firstlineno 249
                lnotab 0x0203
             code
                argcount  : 1
-               nlocals   : 3
-               stacksize : 6
-               flags     : 15
-               code
-                  0x950197007401000000000000000000006a010000000000000000a60000
-                  00ab000000000000000000350001000200740500000000000000000000a6
-                  000000ab0000000000000000006a0300000000000000007c0169007c02a4
-                  018e010100640064006400a6020000ab0200000000000000000100640053
-                  002300310073047702780359007701010059000100010064005300
-                             0 COPY_FREE_VARS           1
-               
-               242           2 RESUME                   0
-               
-               243           4 LOAD_GLOBAL              1 (NULL + reversion)
-                            16 LOAD_ATTR                1 (create_revision)
-                            26 PRECALL                  0
-                            30 CALL                     0
-                            40 BEFORE_WITH
-                            42 POP_TOP
-               
-               244          44 PUSH_NULL
-                            46 LOAD_GLOBAL              5 (NULL + super)
-                            58 PRECALL                  0
-                            62 CALL                     0
-                            72 LOAD_ATTR                3 (save)
-                            82 LOAD_FAST                1 (args)
-                            84 BUILD_MAP                0
-                            86 LOAD_FAST                2 (kwargs)
-                            88 DICT_MERGE               1
-                            90 CALL_FUNCTION_EX         1
-                            92 POP_TOP
-               
-               243          94 LOAD_CONST               0 (None)
-                            96 LOAD_CONST               0 (None)
-                            98 LOAD_CONST               0 (None)
-                           100 PRECALL                  2
-                           104 CALL                     2
-                           114 POP_TOP
-                           116 LOAD_CONST               0 (None)
-                           118 RETURN_VALUE
-                       >>  120 PUSH_EXC_INFO
-                           122 WITH_EXCEPT_START
-                           124 POP_JUMP_FORWARD_IF_TRUE     4 (to 134)
-                           126 RERAISE                  2
-                       >>  128 COPY                     3
-                           130 POP_EXCEPT
-                           132 RERAISE                  1
-                       >>  134 POP_TOP
-                           136 POP_EXCEPT
-                           138 POP_TOP
-                           140 POP_TOP
-                           142 LOAD_CONST               0 (None)
-                           144 RETURN_VALUE
-               ExceptionTable:
-                 42 to 92 -> 120 [1] lasti
-                 120 to 126 -> 128 [3] lasti
-                 134 to 134 -> 128 [3] lasti
-               consts
-                  None
-               names      ('reversion', 'create_revision', 'super', 'save')
-               varnames   ('self', 'args', 'kwargs')
-               freevars   ('__class__',)
-               cellvars   ()
-               filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
-               name       'save'
-               firstlineno 242
-               lnotab 0x0401280132ff
-            code
-               argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970069005300
-               246           0 RESUME                   0
+               254           0 RESUME                   0
                
-               248           2 BUILD_MAP                0
+               256           2 BUILD_MAP                0
                              4 RETURN_VALUE
                consts
                   'Get context to pass to the PDF template.'
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
                name       'get_context_data'
-               firstlineno 246
+               firstlineno 254
                lnotab 0x0202
             'triggered_manually'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 6
                flags     : 3
@@ -2018,89 +2100,89 @@
                   00724c7c026a09000000000000000072457c017c005f0a00000000000000
                   007c006a0b0000000000000000a00c000000000000000000000000000000
                   00000000007c006a0d00000000000000007c026a0900000000000000006a
                   090000000000000000a6020000ab02000000000000000001007c00a00c00
                   00000000000000000000000000000000000000a6000000ab000000000000
                   0000000100640264026402a6020000ab0200000000000000000100640253
                   002300310073047702780359007701010059000100010064025300
-               250           0 RESUME                   0
+               258           0 RESUME                   0
                
-               255           2 LOAD_FAST                0 (self)
+               263           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (template)
                             14 POP_JUMP_FORWARD_IF_TRUE    15 (to 46)
                
-               256          16 LOAD_GLOBAL              3 (NULL + NotImplementedError)
+               264          16 LOAD_GLOBAL              3 (NULL + NotImplementedError)
                             28 LOAD_CONST               1 ('Subclasses of LiveDocument must implement update()')
                             30 PRECALL                  1
                             34 CALL                     1
                             44 RAISE_VARARGS            1
                
-               258     >>   46 LOAD_GLOBAL              5 (NULL + generate_pdf_from_template)
+               266     >>   46 LOAD_GLOBAL              5 (NULL + generate_pdf_from_template)
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                0 (template)
                             70 LOAD_FAST                0 (self)
                             72 LOAD_METHOD              3 (get_context_data)
                             94 PRECALL                  0
                             98 CALL                     0
                            108 PRECALL                  2
                            112 CALL                     2
                            122 UNPACK_SEQUENCE          2
                            126 STORE_FAST               2 (file_object)
                            128 STORE_FAST               3 (result)
                
-               259         130 LOAD_GLOBAL              9 (NULL + allow_join_result)
+               267         130 LOAD_GLOBAL              9 (NULL + allow_join_result)
                            142 PRECALL                  0
                            146 CALL                     0
                            156 BEFORE_WITH
                            158 POP_TOP
                
-               260         160 LOAD_FAST                3 (result)
+               268         160 LOAD_FAST                3 (result)
                            162 LOAD_METHOD              5 (wait)
                            184 PRECALL                  0
                            188 CALL                     0
                            198 POP_TOP
                
-               261         200 LOAD_FAST                2 (file_object)
+               269         200 LOAD_FAST                2 (file_object)
                            202 LOAD_METHOD              6 (refresh_from_db)
                            224 PRECALL                  0
                            228 CALL                     0
                            238 POP_TOP
                
-               262         240 LOAD_FAST                3 (result)
+               270         240 LOAD_FAST                3 (result)
                            242 LOAD_ATTR                7 (status)
                            252 LOAD_GLOBAL             16 (SUCCESS)
                            264 COMPARE_OP               2 (==)
                            270 POP_JUMP_FORWARD_IF_FALSE    76 (to 424)
                            272 LOAD_FAST                2 (file_object)
                            274 LOAD_ATTR                9 (file)
                            284 POP_JUMP_FORWARD_IF_FALSE    69 (to 424)
                
-               263         286 LOAD_FAST                1 (triggered_manually)
+               271         286 LOAD_FAST                1 (triggered_manually)
                            288 LOAD_FAST                0 (self)
                            290 STORE_ATTR              10 (last_update_triggered_manually)
                
-               264         300 LOAD_FAST                0 (self)
+               272         300 LOAD_FAST                0 (self)
                            302 LOAD_ATTR               11 (current_file)
                            312 LOAD_METHOD             12 (save)
                            334 LOAD_FAST                0 (self)
                            336 LOAD_ATTR               13 (filename)
                            346 LOAD_FAST                2 (file_object)
                            348 LOAD_ATTR                9 (file)
                            358 LOAD_ATTR                9 (file)
                            368 PRECALL                  2
                            372 CALL                     2
                            382 POP_TOP
                
-               265         384 LOAD_FAST                0 (self)
+               273         384 LOAD_FAST                0 (self)
                            386 LOAD_METHOD             12 (save)
                            408 PRECALL                  0
                            412 CALL                     0
                            422 POP_TOP
                
-               259     >>  424 LOAD_CONST               2 (None)
+               267     >>  424 LOAD_CONST               2 (None)
                            426 LOAD_CONST               2 (None)
                            428 LOAD_CONST               2 (None)
                            430 PRECALL                  2
                            434 CALL                     2
                            444 POP_TOP
                            446 LOAD_CONST               2 (None)
                            448 RETURN_VALUE
@@ -2127,92 +2209,28 @@
                   None
                names      ('template', 'NotImplementedError', 'generate_pdf_from_template', 'get_context_data', 'allow_join_result', 'wait', 'refresh_from_db', 'status', 'SUCCESS', 'file', 'last_update_triggered_manually', 'current_file', 'save', 'filename')
                varnames   ('self', 'triggered_manually', 'file_object', 'result')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
                name       'update'
-               firstlineno 250
+               firstlineno 258
                lnotab 0x02050e011e0254011e01280128012e010e01540128fa
-            code
-               argcount  : 1
-               nlocals   : 1
-               stacksize : 1
-               flags     : 3
-               code 0x97007c006a0000000000000000005300
-               267           0 RESUME                   0
-               
-               268           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (name)
-                            14 RETURN_VALUE
-               consts
-                  None
-               names      ('name',)
-               varnames   ('self',)
-               freevars   ()
-               cellvars   ()
-               filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
-               name       '__str__'
-               firstlineno 267
-               lnotab 0x0201
-            code
-               argcount  : 0
-               nlocals   : 0
-               stacksize : 3
-               flags     : 0
-               code
-                  0x970065005a0164005a02020065036401a6010000ab0100000000000000
-                  005a04020065036402a6010000ab0100000000000000005a0564035300
-               270           0 RESUME                   0
-                             2 LOAD_NAME                0 (__name__)
-                             4 STORE_NAME               1 (__module__)
-                             6 LOAD_CONST               0 ('LiveDocument.Meta')
-                             8 STORE_NAME               2 (__qualname__)
-               
-               271          10 PUSH_NULL
-                            12 LOAD_NAME                3 (_)
-                            14 LOAD_CONST               1 ('Live document')
-                            16 PRECALL                  1
-                            20 CALL                     1
-                            30 STORE_NAME               4 (verbose_name)
-               
-               272          32 PUSH_NULL
-                            34 LOAD_NAME                3 (_)
-                            36 LOAD_CONST               2 ('Live documents')
-                            38 PRECALL                  1
-                            42 CALL                     1
-                            52 STORE_NAME               5 (verbose_name_plural)
-                            54 LOAD_CONST               3 (None)
-                            56 RETURN_VALUE
-               consts
-                  'LiveDocument.Meta'
-                  'Live document'
-                  'Live documents'
-                  None
-               names      ('__name__', '__module__', '__qualname__', '_', 'verbose_name', 'verbose_name_plural')
-               varnames   ()
-               freevars   ()
-               cellvars   ()
-               filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
-               name       'Meta'
-               firstlineno 270
-               lnotab 0x0a011601
-            'Meta'
             (True,)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'SCOPE_PREFIX', 'template', 'models', 'SlugField', '_', 'slug', 'CharField', 'name', 'FileField', 'current_file', 'BooleanField', 'last_update_triggered_manually', 'property', 'Optional', 'Revision', 'last_version', 'datetime', 'last_update', 'File', 'get_current_file', 'str', 'filename', 'scope', 'save', 'dict', 'Any', 'get_context_data', 'bool', 'update', '__str__', 'Meta', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'SCOPE_PREFIX', 'template', 'models', 'SlugField', '_', 'slug', 'CharField', 'name', 'BooleanField', 'public', 'FileField', 'current_file', 'last_update_triggered_manually', 'Meta', 'str', '__str__', 'save', 'property', 'Optional', 'Revision', 'last_version', 'datetime', 'last_update', 'File', 'get_current_file', 'filename', 'scope', 'dict', 'Any', 'get_context_data', 'bool', 'update', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
          name       'LiveDocument'
          firstlineno 187
          lnotab
-            0x0c010402040204020e01140114fe120436020e0102010201140102fc12
-            060e0118ff1204020116ff0e010207020116ff0e010207180602010aff0e
-            01020402010aff0e0102040a041c040e110c03
+            0x0c010402040204020e01140114fe1204360136020e0102010201140102
+            fc12060e0118ff12041a040c030a04020116ff0e010207020116ff0e0102
+            07180602010aff0e01020402010aff0e0102041c04
       'LiveDocument'
    names      ('datetime', 'typing', 'Any', 'Optional', 'django.core.files', 'File', 'django.core.validators', 'FileExtensionValidator', 'MaxValueValidator', 'MinValueValidator', 'django.db', 'models', 'django.urls', 'reverse', 'django.utils', 'timezone', 'django.utils.translation', 'gettext_lazy', '_', 'reversion', 'calendarweek', 'CalendarWeek', 'calendarweek.django', 'i18n_day_name_choices_lazy', 'celery.result', 'allow_join_result', 'celery.states', 'SUCCESS', 'reversion.models', 'Revision', 'Version', 'aleksis.core.mixins', 'ExtensibleModel', 'ExtensiblePolymorphicModel', 'aleksis.core.models', 'DynamicRoute', 'aleksis.core.util.pdf', 'generate_pdf_from_template', 'PosterGroupDynamicRoute', 'PosterGroup', 'int', '_get_current_year', 'range', 'calendar_weeks', 'Poster', 'LiveDocument')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/models.py'
    name       '<module>'
```

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/rules.cpython-311.pyc` & `aleksis_app_resint-3.1/aleksis/apps/resint/__pycache__/rules.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,62 +1,63 @@
 magic:    0xa70d0d0a
-moddate:  0x75951864 (Mon Mar 20 17:18:45 2023 UTC)
-files sz: 4957
+moddate:  0x188cb764 (Wed Jul 19 07:09:12 2023 UTC)
+files sz: 4979
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c046d055a056d065a060100640064046c076d085a086d095a09010064
-      0064056c0a6d0b5a0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f0100640665
-      106602640784045a116408650364066510640965126606640a84045a1365
-      06640b6501640c65096604640d8404a6000000ab0000000000000000005a
-      146506640b6501640c65096604640e8404a6000000ab0000000000000000
-      005a15650f0200650d640fa6010000ab0100000000000000000200650c64
-      0f6509a6020000ab0200000000000000007a0700007a0100005a16020065
-      0564106516a6020000ab020000000000000000010065160200650d6411a6
-      010000ab0100000000000000007a0100005a170200650564126517a60200
-      00ab020000000000000000010065160200650d6413a6010000ab01000000
-      00000000000200650e6413a6010000ab0100000000000000007a0700007a
-      0100005a180200650564146518a6020000ab020000000000000000010065
-      160200650d6415a6010000ab0100000000000000000200650e6415a60100
-      00ab0100000000000000007a0700007a0100005a190200650564166519a6
-      020000ab0200000000000000000100650f0200650d6417a6010000ab0100
-      000000000000000200650c64176508a6020000ab0200000000000000007a
-      0700000200650c64186509a6020000ab0200000000000000007a0700007a
-      0100005a1a020065056419651aa6020000ab020000000000000000010065
-      1a0200650d641aa6010000ab0100000000000000000200650c641b6509a6
-      020000ab0200000000000000007a0700007a0100005a1b02006505641c65
-      1ba6020000ab0200000000000000000100651a0200650d641da6010000ab
-      0100000000000000000200650e641da6010000ab0100000000000000007a
-      07000002006511641ea6010000ab0100000000000000007a0700007a0100
-      005a1c02006505641f651ca6020000ab0200000000000000000100651a02
-      00650d6420a6010000ab0100000000000000000200650e6420a6010000ab
-      0100000000000000007a070000020065116421a6010000ab010000000000
-      0000007a0700007a0100005a1d020065056422651da6020000ab02000000
-      000000000001006514650f0200650d640fa6010000ab0100000000000000
-      000200650d6417a6010000ab0100000000000000007a0700007a0100007a
-      0700005a1e020065056423651ea6020000ab020000000000000000010065
-      0f0200650d640fa6010000ab0100000000000000000200650d6417a60100
-      00ab0100000000000000007a0700007a0100005a1f020065056424651fa6
-      020000ab0200000000000000000100651a65167a0700005a200200650564
-      256520a6020000ab0200000000000000000100650f0200650d6426a60100
-      00ab0100000000000000007a0100005a210200650564276521a6020000ab
-      0200000000000000000100650f0200650d6426a6010000ab010000000000
-      0000000200650e6426a6010000ab0100000000000000007a0700007a0100
-      005a220200650564286522a6020000ab0200000000000000000100652102
-      00650d6429a6010000ab0100000000000000007a0100005a230200650564
-      2a6523a6020000ab020000000000000000010065210200650d642ba60100
-      00ab0100000000000000007a0100005a2402006505642c6524a6020000ab
-      020000000000000000010065210200650d642da6010000ab010000000000
-      0000007a0100005a2502006505642e6525a6020000ab0200000000000000
-      000100651a65167a07000065217a0700005a2602006505642f6526a60200
-      00ab020000000000000000010064305300
+      036c046d055a056d065a060100640064046c076d085a086d095a096d0a5a
+      0a0100640064056c0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a1001
+      00640665116602640784045a126408650364066511640965136606640a84
+      045a146506640b6501640c6508650a67026604640d8404a6000000ab0000
+      000000000000005a156506640b6501640c650a6604640e8404a6000000ab
+      0000000000000000005a1665100200650e640fa6010000ab010000000000
+      0000000200650d640f650aa6020000ab0200000000000000007a0700007a
+      0100005a170200650564106517a6020000ab020000000000000000010065
+      170200650e6411a6010000ab0100000000000000007a0100005a18020065
+      0564126518a6020000ab020000000000000000010065170200650e6413a6
+      010000ab0100000000000000000200650f6413a6010000ab010000000000
+      0000007a0700007a0100005a190200650564146519a6020000ab02000000
+      0000000000010065170200650e6415a6010000ab01000000000000000002
+      00650f6415a6010000ab0100000000000000007a0700007a0100005a1a02
+      0065056416651aa6020000ab020000000000000000010065100200650e64
+      17a6010000ab0100000000000000000200650d64176509a6020000ab0200
+      000000000000007a0700000200650d6418650aa6020000ab020000000000
+      0000007a0700007a0100005a1b020065056419651ba6020000ab02000000
+      00000000000100651b0200650e641aa6010000ab01000000000000000002
+      00650d641b650aa6020000ab0200000000000000007a0700007a0100005a
+      1c02006505641c651ca6020000ab0200000000000000000100651b020065
+      0e641da6010000ab0100000000000000000200650f641da6010000ab0100
+      000000000000007a07000002006512641ea6010000ab0100000000000000
+      007a0700007a0100005a1d02006505641f651da6020000ab020000000000
+      0000000100651b0200650e6420a6010000ab010000000000000000020065
+      0f6420a6010000ab0100000000000000007a070000020065126421a60100
+      00ab0100000000000000007a0700007a0100005a1e020065056422651ea6
+      020000ab0200000000000000000100651565100200650e640fa6010000ab
+      0100000000000000000200650e6417a6010000ab0100000000000000007a
+      0700007a0100007a0700005a1f020065056423651fa6020000ab02000000
+      0000000000010065100200650e640fa6010000ab01000000000000000002
+      00650e6417a6010000ab0100000000000000007a0700007a0100005a2002
+      00650564246520a6020000ab0200000000000000000100651b65177a0700
+      005a210200650564256521a6020000ab0200000000000000000100651002
+      00650e6426a6010000ab0100000000000000007a0100005a220200650564
+      276522a6020000ab0200000000000000000100651565100200650e6426a6
+      010000ab0100000000000000000200650f6426a6010000ab010000000000
+      0000007a0700007a0100007a0700005a230200650564286523a6020000ab
+      020000000000000000010065220200650e6429a6010000ab010000000000
+      0000007a0100005a2402006505642a6524a6020000ab0200000000000000
+      00010065220200650e642ba6010000ab0100000000000000007a0100005a
+      2502006505642c6525a6020000ab02000000000000000001006522020065
+      0e642da6010000ab0100000000000000007a0100005a2602006505642e65
+      26a6020000ab0200000000000000000100651b65177a07000065227a0700
+      005a2702006505642f6527a6020000ab0200000000000000000100643053
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('User',))
                  6 IMPORT_NAME              0 (django.contrib.auth.models)
                  8 IMPORT_FROM              1 (User)
                 10 STORE_NAME               1 (User)
@@ -75,506 +76,514 @@
                 32 IMPORT_FROM              5 (add_perm)
                 34 STORE_NAME               5 (add_perm)
                 36 IMPORT_FROM              6 (predicate)
                 38 STORE_NAME               6 (predicate)
                 40 POP_TOP
    
      6          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               4 (('Poster', 'PosterGroup'))
+                44 LOAD_CONST               4 (('LiveDocument', 'Poster', 'PosterGroup'))
                 46 IMPORT_NAME              7 (aleksis.apps.resint.models)
-                48 IMPORT_FROM              8 (Poster)
-                50 STORE_NAME               8 (Poster)
-                52 IMPORT_FROM              9 (PosterGroup)
-                54 STORE_NAME               9 (PosterGroup)
-                56 POP_TOP
-   
-     7          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               5 (('check_object_permission', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person'))
-                62 IMPORT_NAME             10 (aleksis.core.util.predicates)
-                64 IMPORT_FROM             11 (check_object_permission)
-                66 STORE_NAME              11 (check_object_permission)
-                68 IMPORT_FROM             12 (has_any_object)
-                70 STORE_NAME              12 (has_any_object)
-                72 IMPORT_FROM             13 (has_global_perm)
-                74 STORE_NAME              13 (has_global_perm)
-                76 IMPORT_FROM             14 (has_object_perm)
-                78 STORE_NAME              14 (has_object_perm)
-                80 IMPORT_FROM             15 (has_person)
-                82 STORE_NAME              15 (has_person)
-                84 POP_TOP
-   
-    16          86 LOAD_CONST               6 ('perm')
-                88 LOAD_NAME               16 (str)
-                90 BUILD_TUPLE              2
-                92 LOAD_CONST               7 (<code object has_poster_group_object_perm, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/rules.py", line 16>)
-                94 MAKE_FUNCTION            4 (annotations)
-                96 STORE_NAME              17 (has_poster_group_object_perm)
-   
-    26          98 LOAD_CONST               8 ('request')
-               100 LOAD_NAME                3 (HttpRequest)
-               102 LOAD_CONST               6 ('perm')
-               104 LOAD_NAME               16 (str)
-               106 LOAD_CONST               9 ('return')
-               108 LOAD_NAME               18 (bool)
-               110 BUILD_TUPLE              6
-               112 LOAD_CONST              10 (<code object permission_validator, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/rules.py", line 26>)
-               114 MAKE_FUNCTION            4 (annotations)
-               116 STORE_NAME              19 (permission_validator)
-   
-    33         118 LOAD_NAME                6 (predicate)
-   
-    34         120 LOAD_CONST              11 ('user')
-               122 LOAD_NAME                1 (User)
-               124 LOAD_CONST              12 ('obj')
-               126 LOAD_NAME                9 (PosterGroup)
-               128 BUILD_TUPLE              4
-               130 LOAD_CONST              13 (<code object is_public_poster_group, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/rules.py", line 33>)
-               132 MAKE_FUNCTION            4 (annotations)
-   
-    33         134 PRECALL                  0
-               138 CALL                     0
-   
-    34         148 STORE_NAME              20 (is_public_poster_group)
-   
-    38         150 LOAD_NAME                6 (predicate)
-   
-    39         152 LOAD_CONST              11 ('user')
-               154 LOAD_NAME                1 (User)
-               156 LOAD_CONST              12 ('obj')
-               158 LOAD_NAME                9 (PosterGroup)
-               160 BUILD_TUPLE              4
-               162 LOAD_CONST              14 (<code object show_poster_group_in_menu, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/rules.py", line 38>)
-               164 MAKE_FUNCTION            4 (annotations)
-   
-    38         166 PRECALL                  0
-               170 CALL                     0
-   
-    39         180 STORE_NAME              21 (show_poster_group_in_menu)
-   
-    44         182 LOAD_NAME               15 (has_person)
-   
-    45         184 PUSH_NULL
-               186 LOAD_NAME               13 (has_global_perm)
-               188 LOAD_CONST              15 ('resint.view_postergroup')
-               190 PRECALL                  1
-               194 CALL                     1
-   
-    46         204 PUSH_NULL
-               206 LOAD_NAME               12 (has_any_object)
-               208 LOAD_CONST              15 ('resint.view_postergroup')
-               210 LOAD_NAME                9 (PosterGroup)
-               212 PRECALL                  2
-               216 CALL                     2
-   
-    45         226 BINARY_OP                7 (|)
-   
-    44         230 BINARY_OP                1 (&)
-               234 STORE_NAME              22 (view_poster_groups_predicate)
-   
-    48         236 PUSH_NULL
-               238 LOAD_NAME                5 (add_perm)
-               240 LOAD_CONST              16 ('resint.view_postergroups_rule')
-               242 LOAD_NAME               22 (view_poster_groups_predicate)
-               244 PRECALL                  2
-               248 CALL                     2
-               258 POP_TOP
-   
-    51         260 LOAD_NAME               22 (view_poster_groups_predicate)
-               262 PUSH_NULL
-               264 LOAD_NAME               13 (has_global_perm)
-   
-    52         266 LOAD_CONST              17 ('resint.add_postergroup')
-   
-    51         268 PRECALL                  1
-               272 CALL                     1
-               282 BINARY_OP                1 (&)
-               286 STORE_NAME              23 (add_poster_group_predicate)
-   
-    54         288 PUSH_NULL
-               290 LOAD_NAME                5 (add_perm)
-               292 LOAD_CONST              18 ('resint.add_postergroup_rule')
-               294 LOAD_NAME               23 (add_poster_group_predicate)
-               296 PRECALL                  2
-               300 CALL                     2
-               310 POP_TOP
-   
-    57         312 LOAD_NAME               22 (view_poster_groups_predicate)
-   
-    58         314 PUSH_NULL
-               316 LOAD_NAME               13 (has_global_perm)
-               318 LOAD_CONST              19 ('resint.change_postergroup')
-               320 PRECALL                  1
-               324 CALL                     1
-               334 PUSH_NULL
-               336 LOAD_NAME               14 (has_object_perm)
-               338 LOAD_CONST              19 ('resint.change_postergroup')
-               340 PRECALL                  1
-               344 CALL                     1
-               354 BINARY_OP                7 (|)
-   
-    57         358 BINARY_OP                1 (&)
-               362 STORE_NAME              24 (edit_poster_group_predicate)
-   
-    60         364 PUSH_NULL
-               366 LOAD_NAME                5 (add_perm)
-               368 LOAD_CONST              20 ('resint.edit_postergroup_rule')
-               370 LOAD_NAME               24 (edit_poster_group_predicate)
-               372 PRECALL                  2
-               376 CALL                     2
-               386 POP_TOP
-   
-    63         388 LOAD_NAME               22 (view_poster_groups_predicate)
-   
-    64         390 PUSH_NULL
-               392 LOAD_NAME               13 (has_global_perm)
-               394 LOAD_CONST              21 ('resint.delete_postergroup')
-               396 PRECALL                  1
-               400 CALL                     1
-               410 PUSH_NULL
-               412 LOAD_NAME               14 (has_object_perm)
-               414 LOAD_CONST              21 ('resint.delete_postergroup')
-               416 PRECALL                  1
-               420 CALL                     1
-               430 BINARY_OP                7 (|)
-   
-    63         434 BINARY_OP                1 (&)
-               438 STORE_NAME              25 (delete_poster_group_predicate)
-   
-    66         440 PUSH_NULL
-               442 LOAD_NAME                5 (add_perm)
-               444 LOAD_CONST              22 ('resint.delete_postergroup_rule')
-               446 LOAD_NAME               25 (delete_poster_group_predicate)
-               448 PRECALL                  2
-               452 CALL                     2
-               462 POP_TOP
-   
-    68         464 LOAD_NAME               15 (has_person)
-   
-    69         466 PUSH_NULL
-               468 LOAD_NAME               13 (has_global_perm)
-               470 LOAD_CONST              23 ('resint.view_poster')
-               472 PRECALL                  1
-               476 CALL                     1
-   
-    70         486 PUSH_NULL
-               488 LOAD_NAME               12 (has_any_object)
-               490 LOAD_CONST              23 ('resint.view_poster')
-               492 LOAD_NAME                8 (Poster)
-               494 PRECALL                  2
-               498 CALL                     2
-   
-    69         508 BINARY_OP                7 (|)
-   
-    71         512 PUSH_NULL
-               514 LOAD_NAME               12 (has_any_object)
-               516 LOAD_CONST              24 ('resint.view_poster_of_group')
-               518 LOAD_NAME                9 (PosterGroup)
-               520 PRECALL                  2
-               524 CALL                     2
-   
-    69         534 BINARY_OP                7 (|)
-   
-    68         538 BINARY_OP                1 (&)
-               542 STORE_NAME              26 (view_posters_predicate)
-   
-    73         544 PUSH_NULL
-               546 LOAD_NAME                5 (add_perm)
-               548 LOAD_CONST              25 ('resint.view_posters_rule')
-               550 LOAD_NAME               26 (view_posters_predicate)
-               552 PRECALL                  2
-               556 CALL                     2
-               566 POP_TOP
-   
-    76         568 LOAD_NAME               26 (view_posters_predicate)
-   
-    77         570 PUSH_NULL
-               572 LOAD_NAME               13 (has_global_perm)
-               574 LOAD_CONST              26 ('resint.add_poster')
-               576 PRECALL                  1
-               580 CALL                     1
-   
-    78         590 PUSH_NULL
-               592 LOAD_NAME               12 (has_any_object)
-               594 LOAD_CONST              27 ('resint.upload_poster_to_group')
-               596 LOAD_NAME                9 (PosterGroup)
-               598 PRECALL                  2
-               602 CALL                     2
-   
-    77         612 BINARY_OP                7 (|)
-   
-    76         616 BINARY_OP                1 (&)
-               620 STORE_NAME              27 (upload_poster_predicate)
-   
-    80         622 PUSH_NULL
-               624 LOAD_NAME                5 (add_perm)
-               626 LOAD_CONST              28 ('resint.upload_poster_rule')
-               628 LOAD_NAME               27 (upload_poster_predicate)
-               630 PRECALL                  2
-               634 CALL                     2
-               644 POP_TOP
-   
-    83         646 LOAD_NAME               26 (view_posters_predicate)
-   
-    84         648 PUSH_NULL
-               650 LOAD_NAME               13 (has_global_perm)
-               652 LOAD_CONST              29 ('resint.change_poster')
-               654 PRECALL                  1
-               658 CALL                     1
-   
-    85         668 PUSH_NULL
-               670 LOAD_NAME               14 (has_object_perm)
-               672 LOAD_CONST              29 ('resint.change_poster')
-               674 PRECALL                  1
-               678 CALL                     1
-   
-    84         688 BINARY_OP                7 (|)
-   
-    86         692 PUSH_NULL
-               694 LOAD_NAME               17 (has_poster_group_object_perm)
-               696 LOAD_CONST              30 ('resint.change_poster_of_group')
-               698 PRECALL                  1
-               702 CALL                     1
-   
-    84         712 BINARY_OP                7 (|)
-   
-    83         716 BINARY_OP                1 (&)
-               720 STORE_NAME              28 (edit_poster_predicate)
-   
-    88         722 PUSH_NULL
-               724 LOAD_NAME                5 (add_perm)
-               726 LOAD_CONST              31 ('resint.edit_poster_rule')
-               728 LOAD_NAME               28 (edit_poster_predicate)
-               730 PRECALL                  2
-               734 CALL                     2
-               744 POP_TOP
-   
-    91         746 LOAD_NAME               26 (view_posters_predicate)
-   
-    92         748 PUSH_NULL
-               750 LOAD_NAME               13 (has_global_perm)
-               752 LOAD_CONST              32 ('resint.delete_poster')
-               754 PRECALL                  1
-               758 CALL                     1
-   
-    93         768 PUSH_NULL
-               770 LOAD_NAME               14 (has_object_perm)
-               772 LOAD_CONST              32 ('resint.delete_poster')
-               774 PRECALL                  1
-               778 CALL                     1
-   
-    92         788 BINARY_OP                7 (|)
-   
-    94         792 PUSH_NULL
-               794 LOAD_NAME               17 (has_poster_group_object_perm)
-               796 LOAD_CONST              33 ('resint.delete_poster_of_group')
-               798 PRECALL                  1
-               802 CALL                     1
-   
-    92         812 BINARY_OP                7 (|)
-   
-    91         816 BINARY_OP                1 (&)
-               820 STORE_NAME              29 (delete_poster_predicate)
-   
-    96         822 PUSH_NULL
-               824 LOAD_NAME                5 (add_perm)
-               826 LOAD_CONST              34 ('resint.delete_poster_rule')
-               828 LOAD_NAME               29 (delete_poster_predicate)
-               830 PRECALL                  2
-               834 CALL                     2
-               844 POP_TOP
-   
-    99         846 LOAD_NAME               20 (is_public_poster_group)
-   
-   100         848 LOAD_NAME               15 (has_person)
-   
-   101         850 PUSH_NULL
-               852 LOAD_NAME               13 (has_global_perm)
-               854 LOAD_CONST              15 ('resint.view_postergroup')
-               856 PRECALL                  1
-               860 CALL                     1
-               870 PUSH_NULL
-               872 LOAD_NAME               13 (has_global_perm)
-               874 LOAD_CONST              23 ('resint.view_poster')
-               876 PRECALL                  1
-               880 CALL                     1
-               890 BINARY_OP                7 (|)
-   
-   100         894 BINARY_OP                1 (&)
-   
-    99         898 BINARY_OP                7 (|)
-               902 STORE_NAME              30 (view_poster_pdf_predicate)
-   
-   103         904 PUSH_NULL
-               906 LOAD_NAME                5 (add_perm)
-               908 LOAD_CONST              35 ('resint.view_poster_pdf')
-               910 LOAD_NAME               30 (view_poster_pdf_predicate)
-               912 PRECALL                  2
-               916 CALL                     2
-               926 POP_TOP
-   
-   106         928 LOAD_NAME               15 (has_person)
-   
-   107         930 PUSH_NULL
-               932 LOAD_NAME               13 (has_global_perm)
-               934 LOAD_CONST              15 ('resint.view_postergroup')
-               936 PRECALL                  1
-               940 CALL                     1
-               950 PUSH_NULL
-               952 LOAD_NAME               13 (has_global_perm)
-               954 LOAD_CONST              23 ('resint.view_poster')
-               956 PRECALL                  1
-               960 CALL                     1
-               970 BINARY_OP                7 (|)
-   
-   106         974 BINARY_OP                1 (&)
-               978 STORE_NAME              31 (view_poster_pdf_menu_predicate)
-   
-   109         980 PUSH_NULL
-               982 LOAD_NAME                5 (add_perm)
-               984 LOAD_CONST              36 ('resint.view_poster_pdf_menu')
-               986 LOAD_NAME               31 (view_poster_pdf_menu_predicate)
-               988 PRECALL                  2
-               992 CALL                     2
-              1002 POP_TOP
-   
-   112        1004 LOAD_NAME               26 (view_posters_predicate)
-              1006 LOAD_NAME               22 (view_poster_groups_predicate)
-              1008 BINARY_OP                7 (|)
-              1012 STORE_NAME              32 (view_poster_menu_predicate)
-   
-   113        1014 PUSH_NULL
-              1016 LOAD_NAME                5 (add_perm)
-              1018 LOAD_CONST              37 ('resint.view_poster_menu')
-              1020 LOAD_NAME               32 (view_poster_menu_predicate)
-              1022 PRECALL                  2
-              1026 CALL                     2
-              1036 POP_TOP
-   
-   117        1038 LOAD_NAME               15 (has_person)
-              1040 PUSH_NULL
-              1042 LOAD_NAME               13 (has_global_perm)
-              1044 LOAD_CONST              38 ('resint.view_livedocument')
-              1046 PRECALL                  1
-              1050 CALL                     1
-              1060 BINARY_OP                1 (&)
-              1064 STORE_NAME              33 (view_live_documents_predicate)
-   
-   118        1066 PUSH_NULL
-              1068 LOAD_NAME                5 (add_perm)
-              1070 LOAD_CONST              39 ('resint.view_livedocuments_rule')
-              1072 LOAD_NAME               33 (view_live_documents_predicate)
-              1074 PRECALL                  2
-              1078 CALL                     2
-              1088 POP_TOP
-   
-   121        1090 LOAD_NAME               15 (has_person)
-   
-   122        1092 PUSH_NULL
-              1094 LOAD_NAME               13 (has_global_perm)
-              1096 LOAD_CONST              38 ('resint.view_livedocument')
-              1098 PRECALL                  1
-              1102 CALL                     1
-              1112 PUSH_NULL
-              1114 LOAD_NAME               14 (has_object_perm)
-              1116 LOAD_CONST              38 ('resint.view_livedocument')
-              1118 PRECALL                  1
-              1122 CALL                     1
-              1132 BINARY_OP                7 (|)
-   
-   121        1136 BINARY_OP                1 (&)
-              1140 STORE_NAME              34 (view_live_document_predicate)
-   
-   124        1142 PUSH_NULL
-              1144 LOAD_NAME                5 (add_perm)
-              1146 LOAD_CONST              40 ('resint.view_livedocument_rule')
-              1148 LOAD_NAME               34 (view_live_document_predicate)
-              1150 PRECALL                  2
-              1154 CALL                     2
-              1164 POP_TOP
-   
-   127        1166 LOAD_NAME               33 (view_live_documents_predicate)
-              1168 PUSH_NULL
-              1170 LOAD_NAME               13 (has_global_perm)
-   
-   128        1172 LOAD_CONST              41 ('resint.add_livedocument')
-   
-   127        1174 PRECALL                  1
-              1178 CALL                     1
-              1188 BINARY_OP                1 (&)
-              1192 STORE_NAME              35 (add_live_document_predicate)
-   
-   130        1194 PUSH_NULL
-              1196 LOAD_NAME                5 (add_perm)
-              1198 LOAD_CONST              42 ('resint.add_livedocument_rule')
-              1200 LOAD_NAME               35 (add_live_document_predicate)
-              1202 PRECALL                  2
-              1206 CALL                     2
-              1216 POP_TOP
-   
-   133        1218 LOAD_NAME               33 (view_live_documents_predicate)
-              1220 PUSH_NULL
-              1222 LOAD_NAME               13 (has_global_perm)
-   
-   134        1224 LOAD_CONST              43 ('resint.change_livedocument')
-   
-   133        1226 PRECALL                  1
-              1230 CALL                     1
-              1240 BINARY_OP                1 (&)
-              1244 STORE_NAME              36 (edit_live_document_predicate)
-   
-   136        1246 PUSH_NULL
-              1248 LOAD_NAME                5 (add_perm)
-              1250 LOAD_CONST              44 ('resint.edit_livedocument_rule')
-              1252 LOAD_NAME               36 (edit_live_document_predicate)
-              1254 PRECALL                  2
-              1258 CALL                     2
-              1268 POP_TOP
-   
-   139        1270 LOAD_NAME               33 (view_live_documents_predicate)
-              1272 PUSH_NULL
-              1274 LOAD_NAME               13 (has_global_perm)
-   
-   140        1276 LOAD_CONST              45 ('resint.delete_livedocument')
-   
-   139        1278 PRECALL                  1
-              1282 CALL                     1
-              1292 BINARY_OP                1 (&)
-              1296 STORE_NAME              37 (delete_live_document_predicate)
-   
-   142        1298 PUSH_NULL
-              1300 LOAD_NAME                5 (add_perm)
-              1302 LOAD_CONST              46 ('resint.delete_livedocument_rule')
-              1304 LOAD_NAME               37 (delete_live_document_predicate)
-              1306 PRECALL                  2
-              1310 CALL                     2
-              1320 POP_TOP
-   
-   147        1322 LOAD_NAME               26 (view_posters_predicate)
-              1324 LOAD_NAME               22 (view_poster_groups_predicate)
-              1326 BINARY_OP                7 (|)
-              1330 LOAD_NAME               33 (view_live_documents_predicate)
-              1332 BINARY_OP                7 (|)
-   
-   146        1336 STORE_NAME              38 (view_menu_predicate)
-   
-   149        1338 PUSH_NULL
-              1340 LOAD_NAME                5 (add_perm)
-              1342 LOAD_CONST              47 ('resint.view_menu_rule')
-              1344 LOAD_NAME               38 (view_menu_predicate)
-              1346 PRECALL                  2
-              1350 CALL                     2
-              1360 POP_TOP
-              1362 LOAD_CONST              48 (None)
-              1364 RETURN_VALUE
+                48 IMPORT_FROM              8 (LiveDocument)
+                50 STORE_NAME               8 (LiveDocument)
+                52 IMPORT_FROM              9 (Poster)
+                54 STORE_NAME               9 (Poster)
+                56 IMPORT_FROM             10 (PosterGroup)
+                58 STORE_NAME              10 (PosterGroup)
+                60 POP_TOP
+   
+     7          62 LOAD_CONST               0 (0)
+                64 LOAD_CONST               5 (('check_object_permission', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person'))
+                66 IMPORT_NAME             11 (aleksis.core.util.predicates)
+                68 IMPORT_FROM             12 (check_object_permission)
+                70 STORE_NAME              12 (check_object_permission)
+                72 IMPORT_FROM             13 (has_any_object)
+                74 STORE_NAME              13 (has_any_object)
+                76 IMPORT_FROM             14 (has_global_perm)
+                78 STORE_NAME              14 (has_global_perm)
+                80 IMPORT_FROM             15 (has_object_perm)
+                82 STORE_NAME              15 (has_object_perm)
+                84 IMPORT_FROM             16 (has_person)
+                86 STORE_NAME              16 (has_person)
+                88 POP_TOP
+   
+    16          90 LOAD_CONST               6 ('perm')
+                92 LOAD_NAME               17 (str)
+                94 BUILD_TUPLE              2
+                96 LOAD_CONST               7 (<code object has_poster_group_object_perm, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/rules.py", line 16>)
+                98 MAKE_FUNCTION            4 (annotations)
+               100 STORE_NAME              18 (has_poster_group_object_perm)
+   
+    26         102 LOAD_CONST               8 ('request')
+               104 LOAD_NAME                3 (HttpRequest)
+               106 LOAD_CONST               6 ('perm')
+               108 LOAD_NAME               17 (str)
+               110 LOAD_CONST               9 ('return')
+               112 LOAD_NAME               19 (bool)
+               114 BUILD_TUPLE              6
+               116 LOAD_CONST              10 (<code object permission_validator, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/rules.py", line 26>)
+               118 MAKE_FUNCTION            4 (annotations)
+               120 STORE_NAME              20 (permission_validator)
+   
+    33         122 LOAD_NAME                6 (predicate)
+   
+    34         124 LOAD_CONST              11 ('user')
+               126 LOAD_NAME                1 (User)
+               128 LOAD_CONST              12 ('obj')
+               130 LOAD_NAME                8 (LiveDocument)
+               132 LOAD_NAME               10 (PosterGroup)
+               134 BUILD_LIST               2
+               136 BUILD_TUPLE              4
+               138 LOAD_CONST              13 (<code object is_public, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/rules.py", line 33>)
+               140 MAKE_FUNCTION            4 (annotations)
+   
+    33         142 PRECALL                  0
+               146 CALL                     0
+   
+    34         156 STORE_NAME              21 (is_public)
+   
+    38         158 LOAD_NAME                6 (predicate)
+   
+    39         160 LOAD_CONST              11 ('user')
+               162 LOAD_NAME                1 (User)
+               164 LOAD_CONST              12 ('obj')
+               166 LOAD_NAME               10 (PosterGroup)
+               168 BUILD_TUPLE              4
+               170 LOAD_CONST              14 (<code object show_poster_group_in_menu, file "/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/rules.py", line 38>)
+               172 MAKE_FUNCTION            4 (annotations)
+   
+    38         174 PRECALL                  0
+               178 CALL                     0
+   
+    39         188 STORE_NAME              22 (show_poster_group_in_menu)
+   
+    44         190 LOAD_NAME               16 (has_person)
+   
+    45         192 PUSH_NULL
+               194 LOAD_NAME               14 (has_global_perm)
+               196 LOAD_CONST              15 ('resint.view_postergroup')
+               198 PRECALL                  1
+               202 CALL                     1
+   
+    46         212 PUSH_NULL
+               214 LOAD_NAME               13 (has_any_object)
+               216 LOAD_CONST              15 ('resint.view_postergroup')
+               218 LOAD_NAME               10 (PosterGroup)
+               220 PRECALL                  2
+               224 CALL                     2
+   
+    45         234 BINARY_OP                7 (|)
+   
+    44         238 BINARY_OP                1 (&)
+               242 STORE_NAME              23 (view_poster_groups_predicate)
+   
+    48         244 PUSH_NULL
+               246 LOAD_NAME                5 (add_perm)
+               248 LOAD_CONST              16 ('resint.view_postergroups_rule')
+               250 LOAD_NAME               23 (view_poster_groups_predicate)
+               252 PRECALL                  2
+               256 CALL                     2
+               266 POP_TOP
+   
+    51         268 LOAD_NAME               23 (view_poster_groups_predicate)
+               270 PUSH_NULL
+               272 LOAD_NAME               14 (has_global_perm)
+   
+    52         274 LOAD_CONST              17 ('resint.add_postergroup')
+   
+    51         276 PRECALL                  1
+               280 CALL                     1
+               290 BINARY_OP                1 (&)
+               294 STORE_NAME              24 (add_poster_group_predicate)
+   
+    54         296 PUSH_NULL
+               298 LOAD_NAME                5 (add_perm)
+               300 LOAD_CONST              18 ('resint.add_postergroup_rule')
+               302 LOAD_NAME               24 (add_poster_group_predicate)
+               304 PRECALL                  2
+               308 CALL                     2
+               318 POP_TOP
+   
+    57         320 LOAD_NAME               23 (view_poster_groups_predicate)
+   
+    58         322 PUSH_NULL
+               324 LOAD_NAME               14 (has_global_perm)
+               326 LOAD_CONST              19 ('resint.change_postergroup')
+               328 PRECALL                  1
+               332 CALL                     1
+               342 PUSH_NULL
+               344 LOAD_NAME               15 (has_object_perm)
+               346 LOAD_CONST              19 ('resint.change_postergroup')
+               348 PRECALL                  1
+               352 CALL                     1
+               362 BINARY_OP                7 (|)
+   
+    57         366 BINARY_OP                1 (&)
+               370 STORE_NAME              25 (edit_poster_group_predicate)
+   
+    60         372 PUSH_NULL
+               374 LOAD_NAME                5 (add_perm)
+               376 LOAD_CONST              20 ('resint.edit_postergroup_rule')
+               378 LOAD_NAME               25 (edit_poster_group_predicate)
+               380 PRECALL                  2
+               384 CALL                     2
+               394 POP_TOP
+   
+    63         396 LOAD_NAME               23 (view_poster_groups_predicate)
+   
+    64         398 PUSH_NULL
+               400 LOAD_NAME               14 (has_global_perm)
+               402 LOAD_CONST              21 ('resint.delete_postergroup')
+               404 PRECALL                  1
+               408 CALL                     1
+               418 PUSH_NULL
+               420 LOAD_NAME               15 (has_object_perm)
+               422 LOAD_CONST              21 ('resint.delete_postergroup')
+               424 PRECALL                  1
+               428 CALL                     1
+               438 BINARY_OP                7 (|)
+   
+    63         442 BINARY_OP                1 (&)
+               446 STORE_NAME              26 (delete_poster_group_predicate)
+   
+    66         448 PUSH_NULL
+               450 LOAD_NAME                5 (add_perm)
+               452 LOAD_CONST              22 ('resint.delete_postergroup_rule')
+               454 LOAD_NAME               26 (delete_poster_group_predicate)
+               456 PRECALL                  2
+               460 CALL                     2
+               470 POP_TOP
+   
+    68         472 LOAD_NAME               16 (has_person)
+   
+    69         474 PUSH_NULL
+               476 LOAD_NAME               14 (has_global_perm)
+               478 LOAD_CONST              23 ('resint.view_poster')
+               480 PRECALL                  1
+               484 CALL                     1
+   
+    70         494 PUSH_NULL
+               496 LOAD_NAME               13 (has_any_object)
+               498 LOAD_CONST              23 ('resint.view_poster')
+               500 LOAD_NAME                9 (Poster)
+               502 PRECALL                  2
+               506 CALL                     2
+   
+    69         516 BINARY_OP                7 (|)
+   
+    71         520 PUSH_NULL
+               522 LOAD_NAME               13 (has_any_object)
+               524 LOAD_CONST              24 ('resint.view_poster_of_group')
+               526 LOAD_NAME               10 (PosterGroup)
+               528 PRECALL                  2
+               532 CALL                     2
+   
+    69         542 BINARY_OP                7 (|)
+   
+    68         546 BINARY_OP                1 (&)
+               550 STORE_NAME              27 (view_posters_predicate)
+   
+    73         552 PUSH_NULL
+               554 LOAD_NAME                5 (add_perm)
+               556 LOAD_CONST              25 ('resint.view_posters_rule')
+               558 LOAD_NAME               27 (view_posters_predicate)
+               560 PRECALL                  2
+               564 CALL                     2
+               574 POP_TOP
+   
+    76         576 LOAD_NAME               27 (view_posters_predicate)
+   
+    77         578 PUSH_NULL
+               580 LOAD_NAME               14 (has_global_perm)
+               582 LOAD_CONST              26 ('resint.add_poster')
+               584 PRECALL                  1
+               588 CALL                     1
+   
+    78         598 PUSH_NULL
+               600 LOAD_NAME               13 (has_any_object)
+               602 LOAD_CONST              27 ('resint.upload_poster_to_group')
+               604 LOAD_NAME               10 (PosterGroup)
+               606 PRECALL                  2
+               610 CALL                     2
+   
+    77         620 BINARY_OP                7 (|)
+   
+    76         624 BINARY_OP                1 (&)
+               628 STORE_NAME              28 (upload_poster_predicate)
+   
+    80         630 PUSH_NULL
+               632 LOAD_NAME                5 (add_perm)
+               634 LOAD_CONST              28 ('resint.upload_poster_rule')
+               636 LOAD_NAME               28 (upload_poster_predicate)
+               638 PRECALL                  2
+               642 CALL                     2
+               652 POP_TOP
+   
+    83         654 LOAD_NAME               27 (view_posters_predicate)
+   
+    84         656 PUSH_NULL
+               658 LOAD_NAME               14 (has_global_perm)
+               660 LOAD_CONST              29 ('resint.change_poster')
+               662 PRECALL                  1
+               666 CALL                     1
+   
+    85         676 PUSH_NULL
+               678 LOAD_NAME               15 (has_object_perm)
+               680 LOAD_CONST              29 ('resint.change_poster')
+               682 PRECALL                  1
+               686 CALL                     1
+   
+    84         696 BINARY_OP                7 (|)
+   
+    86         700 PUSH_NULL
+               702 LOAD_NAME               18 (has_poster_group_object_perm)
+               704 LOAD_CONST              30 ('resint.change_poster_of_group')
+               706 PRECALL                  1
+               710 CALL                     1
+   
+    84         720 BINARY_OP                7 (|)
+   
+    83         724 BINARY_OP                1 (&)
+               728 STORE_NAME              29 (edit_poster_predicate)
+   
+    88         730 PUSH_NULL
+               732 LOAD_NAME                5 (add_perm)
+               734 LOAD_CONST              31 ('resint.edit_poster_rule')
+               736 LOAD_NAME               29 (edit_poster_predicate)
+               738 PRECALL                  2
+               742 CALL                     2
+               752 POP_TOP
+   
+    91         754 LOAD_NAME               27 (view_posters_predicate)
+   
+    92         756 PUSH_NULL
+               758 LOAD_NAME               14 (has_global_perm)
+               760 LOAD_CONST              32 ('resint.delete_poster')
+               762 PRECALL                  1
+               766 CALL                     1
+   
+    93         776 PUSH_NULL
+               778 LOAD_NAME               15 (has_object_perm)
+               780 LOAD_CONST              32 ('resint.delete_poster')
+               782 PRECALL                  1
+               786 CALL                     1
+   
+    92         796 BINARY_OP                7 (|)
+   
+    94         800 PUSH_NULL
+               802 LOAD_NAME               18 (has_poster_group_object_perm)
+               804 LOAD_CONST              33 ('resint.delete_poster_of_group')
+               806 PRECALL                  1
+               810 CALL                     1
+   
+    92         820 BINARY_OP                7 (|)
+   
+    91         824 BINARY_OP                1 (&)
+               828 STORE_NAME              30 (delete_poster_predicate)
+   
+    96         830 PUSH_NULL
+               832 LOAD_NAME                5 (add_perm)
+               834 LOAD_CONST              34 ('resint.delete_poster_rule')
+               836 LOAD_NAME               30 (delete_poster_predicate)
+               838 PRECALL                  2
+               842 CALL                     2
+               852 POP_TOP
+   
+    99         854 LOAD_NAME               21 (is_public)
+   
+   100         856 LOAD_NAME               16 (has_person)
+   
+   101         858 PUSH_NULL
+               860 LOAD_NAME               14 (has_global_perm)
+               862 LOAD_CONST              15 ('resint.view_postergroup')
+               864 PRECALL                  1
+               868 CALL                     1
+               878 PUSH_NULL
+               880 LOAD_NAME               14 (has_global_perm)
+               882 LOAD_CONST              23 ('resint.view_poster')
+               884 PRECALL                  1
+               888 CALL                     1
+               898 BINARY_OP                7 (|)
+   
+   100         902 BINARY_OP                1 (&)
+   
+    99         906 BINARY_OP                7 (|)
+               910 STORE_NAME              31 (view_poster_pdf_predicate)
+   
+   103         912 PUSH_NULL
+               914 LOAD_NAME                5 (add_perm)
+               916 LOAD_CONST              35 ('resint.view_poster_pdf')
+               918 LOAD_NAME               31 (view_poster_pdf_predicate)
+               920 PRECALL                  2
+               924 CALL                     2
+               934 POP_TOP
+   
+   106         936 LOAD_NAME               16 (has_person)
+   
+   107         938 PUSH_NULL
+               940 LOAD_NAME               14 (has_global_perm)
+               942 LOAD_CONST              15 ('resint.view_postergroup')
+               944 PRECALL                  1
+               948 CALL                     1
+               958 PUSH_NULL
+               960 LOAD_NAME               14 (has_global_perm)
+               962 LOAD_CONST              23 ('resint.view_poster')
+               964 PRECALL                  1
+               968 CALL                     1
+               978 BINARY_OP                7 (|)
+   
+   106         982 BINARY_OP                1 (&)
+               986 STORE_NAME              32 (view_poster_pdf_menu_predicate)
+   
+   109         988 PUSH_NULL
+               990 LOAD_NAME                5 (add_perm)
+               992 LOAD_CONST              36 ('resint.view_poster_pdf_menu')
+               994 LOAD_NAME               32 (view_poster_pdf_menu_predicate)
+               996 PRECALL                  2
+              1000 CALL                     2
+              1010 POP_TOP
+   
+   112        1012 LOAD_NAME               27 (view_posters_predicate)
+              1014 LOAD_NAME               23 (view_poster_groups_predicate)
+              1016 BINARY_OP                7 (|)
+              1020 STORE_NAME              33 (view_poster_menu_predicate)
+   
+   113        1022 PUSH_NULL
+              1024 LOAD_NAME                5 (add_perm)
+              1026 LOAD_CONST              37 ('resint.view_poster_menu')
+              1028 LOAD_NAME               33 (view_poster_menu_predicate)
+              1030 PRECALL                  2
+              1034 CALL                     2
+              1044 POP_TOP
+   
+   117        1046 LOAD_NAME               16 (has_person)
+              1048 PUSH_NULL
+              1050 LOAD_NAME               14 (has_global_perm)
+              1052 LOAD_CONST              38 ('resint.view_livedocument')
+              1054 PRECALL                  1
+              1058 CALL                     1
+              1068 BINARY_OP                1 (&)
+              1072 STORE_NAME              34 (view_live_documents_predicate)
+   
+   118        1074 PUSH_NULL
+              1076 LOAD_NAME                5 (add_perm)
+              1078 LOAD_CONST              39 ('resint.view_livedocuments_rule')
+              1080 LOAD_NAME               34 (view_live_documents_predicate)
+              1082 PRECALL                  2
+              1086 CALL                     2
+              1096 POP_TOP
+   
+   121        1098 LOAD_NAME               21 (is_public)
+   
+   122        1100 LOAD_NAME               16 (has_person)
+   
+   123        1102 PUSH_NULL
+              1104 LOAD_NAME               14 (has_global_perm)
+              1106 LOAD_CONST              38 ('resint.view_livedocument')
+              1108 PRECALL                  1
+              1112 CALL                     1
+              1122 PUSH_NULL
+              1124 LOAD_NAME               15 (has_object_perm)
+              1126 LOAD_CONST              38 ('resint.view_livedocument')
+              1128 PRECALL                  1
+              1132 CALL                     1
+              1142 BINARY_OP                7 (|)
+   
+   122        1146 BINARY_OP                1 (&)
+   
+   121        1150 BINARY_OP                7 (|)
+              1154 STORE_NAME              35 (view_live_document_predicate)
+   
+   125        1156 PUSH_NULL
+              1158 LOAD_NAME                5 (add_perm)
+              1160 LOAD_CONST              40 ('resint.view_livedocument_rule')
+              1162 LOAD_NAME               35 (view_live_document_predicate)
+              1164 PRECALL                  2
+              1168 CALL                     2
+              1178 POP_TOP
+   
+   128        1180 LOAD_NAME               34 (view_live_documents_predicate)
+              1182 PUSH_NULL
+              1184 LOAD_NAME               14 (has_global_perm)
+   
+   129        1186 LOAD_CONST              41 ('resint.add_livedocument')
+   
+   128        1188 PRECALL                  1
+              1192 CALL                     1
+              1202 BINARY_OP                1 (&)
+              1206 STORE_NAME              36 (add_live_document_predicate)
+   
+   131        1208 PUSH_NULL
+              1210 LOAD_NAME                5 (add_perm)
+              1212 LOAD_CONST              42 ('resint.add_livedocument_rule')
+              1214 LOAD_NAME               36 (add_live_document_predicate)
+              1216 PRECALL                  2
+              1220 CALL                     2
+              1230 POP_TOP
+   
+   134        1232 LOAD_NAME               34 (view_live_documents_predicate)
+              1234 PUSH_NULL
+              1236 LOAD_NAME               14 (has_global_perm)
+   
+   135        1238 LOAD_CONST              43 ('resint.change_livedocument')
+   
+   134        1240 PRECALL                  1
+              1244 CALL                     1
+              1254 BINARY_OP                1 (&)
+              1258 STORE_NAME              37 (edit_live_document_predicate)
+   
+   137        1260 PUSH_NULL
+              1262 LOAD_NAME                5 (add_perm)
+              1264 LOAD_CONST              44 ('resint.edit_livedocument_rule')
+              1266 LOAD_NAME               37 (edit_live_document_predicate)
+              1268 PRECALL                  2
+              1272 CALL                     2
+              1282 POP_TOP
+   
+   140        1284 LOAD_NAME               34 (view_live_documents_predicate)
+              1286 PUSH_NULL
+              1288 LOAD_NAME               14 (has_global_perm)
+   
+   141        1290 LOAD_CONST              45 ('resint.delete_livedocument')
+   
+   140        1292 PRECALL                  1
+              1296 CALL                     1
+              1306 BINARY_OP                1 (&)
+              1310 STORE_NAME              38 (delete_live_document_predicate)
+   
+   143        1312 PUSH_NULL
+              1314 LOAD_NAME                5 (add_perm)
+              1316 LOAD_CONST              46 ('resint.delete_livedocument_rule')
+              1318 LOAD_NAME               38 (delete_live_document_predicate)
+              1320 PRECALL                  2
+              1324 CALL                     2
+              1334 POP_TOP
+   
+   148        1336 LOAD_NAME               27 (view_posters_predicate)
+              1338 LOAD_NAME               23 (view_poster_groups_predicate)
+              1340 BINARY_OP                7 (|)
+              1344 LOAD_NAME               34 (view_live_documents_predicate)
+              1346 BINARY_OP                7 (|)
+   
+   147        1350 STORE_NAME              39 (view_menu_predicate)
+   
+   150        1352 PUSH_NULL
+              1354 LOAD_NAME                5 (add_perm)
+              1356 LOAD_CONST              47 ('resint.view_menu_rule')
+              1358 LOAD_NAME               39 (view_menu_predicate)
+              1360 PRECALL                  2
+              1364 CALL                     2
+              1374 POP_TOP
+              1376 LOAD_CONST              48 (None)
+              1378 RETURN_VALUE
    consts
       0
       ('User',)
       ('HttpRequest',)
       ('add_perm', 'predicate')
-      ('Poster', 'PosterGroup')
+      ('LiveDocument', 'Poster', 'PosterGroup')
       ('check_object_permission', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person')
       'perm'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
          flags     : 3
@@ -719,15 +728,15 @@
          consts
             None
          names      ('public',)
          varnames   ('user', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/rules.py'
-         name       'is_public_poster_group'
+         name       'is_public'
          firstlineno 33
          lnotab 0x0202
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 1
          flags     : 3
@@ -777,22 +786,22 @@
       'resint.add_livedocument_rule'
       'resint.change_livedocument'
       'resint.edit_livedocument_rule'
       'resint.delete_livedocument'
       'resint.delete_livedocument_rule'
       'resint.view_menu_rule'
       None
-   names      ('django.contrib.auth.models', 'User', 'django.http', 'HttpRequest', 'rules', 'add_perm', 'predicate', 'aleksis.apps.resint.models', 'Poster', 'PosterGroup', 'aleksis.core.util.predicates', 'check_object_permission', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person', 'str', 'has_poster_group_object_perm', 'bool', 'permission_validator', 'is_public_poster_group', 'show_poster_group_in_menu', 'view_poster_groups_predicate', 'add_poster_group_predicate', 'edit_poster_group_predicate', 'delete_poster_group_predicate', 'view_posters_predicate', 'upload_poster_predicate', 'edit_poster_predicate', 'delete_poster_predicate', 'view_poster_pdf_predicate', 'view_poster_pdf_menu_predicate', 'view_poster_menu_predicate', 'view_live_documents_predicate', 'view_live_document_predicate', 'add_live_document_predicate', 'edit_live_document_predicate', 'delete_live_document_predicate', 'view_menu_predicate')
+   names      ('django.contrib.auth.models', 'User', 'django.http', 'HttpRequest', 'rules', 'add_perm', 'predicate', 'aleksis.apps.resint.models', 'LiveDocument', 'Poster', 'PosterGroup', 'aleksis.core.util.predicates', 'check_object_permission', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person', 'str', 'has_poster_group_object_perm', 'bool', 'permission_validator', 'is_public', 'show_poster_group_in_menu', 'view_poster_groups_predicate', 'add_poster_group_predicate', 'edit_poster_group_predicate', 'delete_poster_group_predicate', 'view_posters_predicate', 'upload_poster_predicate', 'edit_poster_predicate', 'delete_poster_predicate', 'view_poster_pdf_predicate', 'view_poster_pdf_menu_predicate', 'view_poster_menu_predicate', 'view_live_documents_predicate', 'view_live_document_predicate', 'add_live_document_predicate', 'edit_live_document_predicate', 'delete_live_document_predicate', 'view_menu_predicate')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/rules.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c010c02100210011c090c0a140702010eff0e01020402010e
+      0x00ff02010c010c02100214011c090c0a1407020112ff0e01020402010e
       ff0e0102050201140116ff04ff06041803060102ff1403180302012cff06
       03180302012cff060318020201140116ff040216fe04ff06051803020114
       0116ff04ff060418030201140114ff040214fe04ff060518030201140114
       ff040214fe04ff06051803020102012cff04ff0604180302012cff060318
-      030a0118041c01180302012cff06031803060102ff14031803060102ff14
-      031803060102ff140318050eff0203
+      030a0118041c011803020102012cff04ff06041803060102ff1403180306
+      0102ff14031803060102ff140318050eff0203
```

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/apps.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/forms.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/frontend/index.js` & `aleksis_app_resint-3.1/aleksis/apps/resint/frontend/index.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -36,21 +36,14 @@
         path: ":pk/delete/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "resint.posterDelete",
         props: {
             byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
         },
     }, {
-        path: ":slug.pdf",
-        component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
-        name: "resint.posterShowCurrent",
-        props: {
-            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-        },
-    }, {
         path: "groups/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "resint.posterGroupList",
         meta: {
             inMenu: true,
             titleKey: "resint.poster_groups.menu_title",
             icon: "mdi-folder-multiple-outline",
@@ -110,23 +103,9 @@
     }, {
         path: "live_documents/:pk/delete/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "resint.deleteLiveDocument",
         props: {
             byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
         },
-    }, {
-        path: "live_documents/:slug.pdf",
-        component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
-        name: "resint.showLiveDocument",
-        props: {
-            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-        },
-    }, {
-        path: "api/live_documents/:slug.pdf",
-        component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
-        name: "resint.apiShowLiveDocument",
-        props: {
-            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-        },
     }, ],
 };
```

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_resint-3.1/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_resint-3.1/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_resint-3.1/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_resint-3.1/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/la/LC_MESSAGES/django.po` & `aleksis_app_resint-3.1/aleksis/apps/resint/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_resint-3.1/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_resint-3.1/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-06-12 05:32+0000\n"
+"PO-Revision-Date: 2023-05-26 04:38+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
 "Language-Team: Russian <https://translate.edugit.org/projects/aleksis/"
 "aleksis-app-resint/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -105,15 +105,15 @@
 msgid "Live documents"
 msgstr "Онлайн-документы"
 
 msgid "Manage posters"
 msgstr "Управление документами"
 
 msgid "Name"
-msgstr "Имя"
+msgstr "Полное имя"
 
 msgid "Open"
 msgstr "Открыть"
 
 msgid "PDF"
 msgstr "PDF"
```

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_resint-3.1/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,22 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-04-23 12:52+0000\n"
-"PO-Revision-Date: 2022-06-12 05:32+0000\n"
+"PO-Revision-Date: 2023-05-26 04:38+0000\n"
 "Last-Translator: Serhii Horichenko <m@sgg.im>\n"
-"Language-Team: Russian <https://translate.edugit.org/projects/aleksis/"
-"aleksis-app-resint/ru/>\n"
+"Language-Team: Russian <https://translate.edugit.org/projects/aleksis/aleksis-app-resint/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
-"%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 "X-Generator: Weblate 4.12.1\n"
 
 #: aleksis/apps/resint/apps.py:27
 msgid "Access PDF file for live document"
 msgstr "Доступ PDF файла для онлайн-документа"
 
 #: aleksis/apps/resint/menus.py:37
@@ -52,15 +49,15 @@
 #: aleksis/apps/resint/models.py:26
 msgid "If you use 'example', the filename will be 'example.pdf'."
 msgstr "При использовании 'пример' имя файла будет 'пример.pdf'."
 
 #: aleksis/apps/resint/models.py:28 aleksis/apps/resint/models.py:163
 #: aleksis/apps/resint/templates/resint/group/list.html:19
 msgid "Name"
-msgstr "Имя"
+msgstr "Полное имя"
 
 #: aleksis/apps/resint/models.py:30
 msgid "Publishing weekday"
 msgstr "День недели публикации"
 
 #: aleksis/apps/resint/models.py:32
 #: aleksis/apps/resint/templates/resint/group/list.html:22
```

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_resint-3.1/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_resint-3.1/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_resint-3.1/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0001_initial.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0002_permissions.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0002_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0003_group_in_unique_constraint.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0003_group_in_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0004_edit_permission.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0004_edit_permission.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0005_fix_permissions.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0005_fix_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0006_livedocument.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/migrations/0006_livedocument.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/models.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,25 +192,37 @@
     template = None
 
     slug = models.SlugField(
         verbose_name=_("Slug"),
         help_text=_("This will be used for the name of the current PDF file."),
     )
     name = models.CharField(max_length=255, verbose_name=_("Name"))
+    public = models.BooleanField(default=False, verbose_name=_("Show for not logged-in users"))
 
     current_file = models.FileField(
         upload_to="live_documents/",
         blank=True,
         verbose_name=_("Current file"),
         editable=False,
     )
     last_update_triggered_manually = models.BooleanField(
         default=False, verbose_name=_("Was the last update triggered manually?"), editable=False
     )
 
+    class Meta:
+        verbose_name = _("Live document")
+        verbose_name_plural = _("Live documents")
+
+    def __str__(self) -> str:
+        return self.name
+
+    def save(self, *args, **kwargs):
+        with reversion.create_revision():
+            super().save(*args, **kwargs)
+
     @property
     def last_version(self) -> Optional[Revision]:
         """Get django-reversion version of last file update."""
         versions = Version.objects.get_for_object(self).order_by("revision__date_created")
         if versions.exists():
             return versions.last()
         return None
@@ -235,18 +247,14 @@
         return f"{self.slug}.pdf"
 
     @property
     def scope(self) -> str:
         """Return OAuth2 scope name to access PDF file via API."""
         return f"{self.SCOPE_PREFIX}_{self.slug}"
 
-    def save(self, *args, **kwargs):
-        with reversion.create_revision():
-            super().save(*args, **kwargs)
-
     def get_context_data(self) -> dict[str, Any]:
         """Get context to pass to the PDF template."""
         return {}
 
     def update(self, triggered_manually: bool = True):
         """Update the file with a new version.
 
@@ -259,14 +267,7 @@
         with allow_join_result():
             result.wait()
             file_object.refresh_from_db()
             if result.status == SUCCESS and file_object.file:
                 self.last_update_triggered_manually = triggered_manually
                 self.current_file.save(self.filename, file_object.file.file)
                 self.save()
-
-    def __str__(self) -> str:
-        return self.name
-
-    class Meta:
-        verbose_name = _("Live document")
-        verbose_name_plural = _("Live documents")
```

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/rules.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.contrib.auth.models import User
 from django.http import HttpRequest
 
 from rules import add_perm, predicate
 
-from aleksis.apps.resint.models import Poster, PosterGroup
+from aleksis.apps.resint.models import LiveDocument, Poster, PosterGroup
 from aleksis.core.util.predicates import (
     check_object_permission,
     has_any_object,
     has_global_perm,
     has_object_perm,
     has_person,
 )
@@ -27,15 +27,15 @@
     """Check whether the request user has a permission."""
     if request.user:
         return request.user.has_perm(perm, obj)
     return False
 
 
 @predicate
-def is_public_poster_group(user: User, obj: PosterGroup):
+def is_public(user: User, obj: [LiveDocument, PosterGroup]):
     return obj.public
 
 
 @predicate
 def show_poster_group_in_menu(user: User, obj: PosterGroup):
     return obj.show_in_menu
 
@@ -92,15 +92,15 @@
     has_global_perm("resint.delete_poster")
     | has_object_perm("resint.delete_poster")
     | has_poster_group_object_perm("resint.delete_poster_of_group")
 )
 add_perm("resint.delete_poster_rule", delete_poster_predicate)
 
 # View poster PDF file
-view_poster_pdf_predicate = is_public_poster_group | (
+view_poster_pdf_predicate = is_public | (
     has_person
     & (has_global_perm("resint.view_postergroup") | has_global_perm("resint.view_poster"))
 )
 add_perm("resint.view_poster_pdf", view_poster_pdf_predicate)
 
 # View poster PDF file in menu
 view_poster_pdf_menu_predicate = has_person & (
@@ -114,16 +114,17 @@
 
 
 # View live document list
 view_live_documents_predicate = has_person & has_global_perm("resint.view_livedocument")
 add_perm("resint.view_livedocuments_rule", view_live_documents_predicate)
 
 # View live document
-view_live_document_predicate = has_person & (
-    has_global_perm("resint.view_livedocument") | has_object_perm("resint.view_livedocument")
+view_live_document_predicate = is_public | (
+    has_person
+    & (has_global_perm("resint.view_livedocument") | has_object_perm("resint.view_livedocument"))
 )
 add_perm("resint.view_livedocument_rule", view_live_document_predicate)
 
 # Add live document
 add_live_document_predicate = view_live_documents_predicate & has_global_perm(
     "resint.add_livedocument"
 )
```

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/tables.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/group/list.html` & `aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/group/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/create.html` & `aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/live_document/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/edit.html` & `aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/live_document/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/list.html` & `aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/live_document/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/poster/list.html` & `aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/poster/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/poster/upload.html` & `aleksis_app_resint-3.1/aleksis/apps/resint/templates/resint/poster/upload.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/urls.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 )
 
 urlpatterns = [
     path("", PosterListView.as_view(), name="poster_index"),
     path("upload/", PosterUploadView.as_view(), name="poster_upload"),
     path("<int:pk>/edit/", PosterEditView.as_view(), name="poster_edit"),
     path("<int:pk>/delete/", PosterDeleteView.as_view(), name="poster_delete"),
-    path("<str:slug>.pdf", PosterCurrentView.as_view(), name="poster_show_current"),
     path("groups/", PosterGroupListView.as_view(), name="poster_group_list"),
     path("groups/create/", PosterGroupCreateView.as_view(), name="create_poster_group"),
     path("groups/<int:pk>/edit/", PosterGroupEditView.as_view(), name="edit_poster_group"),
     path("groups/<int:pk>/delete/", PosterGroupDeleteView.as_view(), name="delete_poster_group"),
     path("live/", LiveDocumentListView.as_view(), name="live_documents"),
     path(
         "live/<str:app>/<str:model>/create/",
@@ -40,14 +39,18 @@
         name="edit_live_document",
     ),
     path(
         "live_documents/<int:pk>/delete/",
         LiveDocumentDeleteView.as_view(),
         name="delete_live_document",
     ),
+]
+
+api_urlpatterns = [
+    path("<str:slug>.pdf", PosterCurrentView.as_view(), name="poster_show_current"),
     path(
         "live_documents/<str:slug>.pdf",
         LiveDocumentShowView.as_view(),
         name="show_live_document",
     ),
     path(
         "api/live_documents/<str:slug>.pdf",
```

### Comparing `aleksis_app_resint-3.0b2/aleksis/apps/resint/views.py` & `aleksis_app_resint-3.1/aleksis/apps/resint/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/docs/Makefile` & `aleksis_app_resint-3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/docs/_static/create_live_document.png` & `aleksis_app_resint-3.1/docs/_static/create_live_document.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/docs/_static/create_poster_group.png` & `aleksis_app_resint-3.1/docs/_static/create_poster_group.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/docs/_static/manage_posters_list.png` & `aleksis_app_resint-3.1/docs/_static/manage_posters_list.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/docs/_static/upload_poster.png` & `aleksis_app_resint-3.1/docs/_static/upload_poster.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/docs/admin/01_poster_groups.rst` & `aleksis_app_resint-3.1/docs/admin/01_poster_groups.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/docs/admin/02_live_documents.rst` & `aleksis_app_resint-3.1/docs/admin/02_live_documents.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/docs/conf.py` & `aleksis_app_resint-3.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 # -- Project information -----------------------------------------------------
 
 project = "AlekSIS-App-Resint"
 copyright = "2018-2022 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
-version = "3.0"
+version = "3.1"
 # The full version, including alpha/beta/rc tags
-release = "3.0b2"
+release = "3.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_app_resint-3.0b2/docs/dev/01_live_document_types.rst` & `aleksis_app_resint-3.1/docs/dev/01_live_document_types.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/docs/index.rst` & `aleksis_app_resint-3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/docs/make.bat` & `aleksis_app_resint-3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/docs/user/01_posters.rst` & `aleksis_app_resint-3.1/docs/user/01_posters.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/tox.ini` & `aleksis_app_resint-3.1/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b2/PKG-INFO` & `aleksis_app_resint-3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aleksis-app-resint
-Version: 3.0b2
+Version: 3.1
 Summary: AlekSIS (School Information System) — App Resint (Public poster)
-Home-page: https://aleksis.org/
+Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Author: Julian Leucker
 Author-email: leuckeju@katharineum.de
 Maintainer: Jonathan Weth
 Maintainer-email: dev@jonathanweth.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: AlekSIS-Core (>=3.0b0,<4.0)
+Requires-Dist: AlekSIS-Core (>=3.0,<4.0)
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS-App-Resint
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Resint (Public poster)
 ================================================================
 
 AlekSIS
```

