# Comparing `tmp/factory_boy-3.2.1.tar.gz` & `tmp/factory_boy-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/factory_boy-3.2.1.tar", last modified: Tue Oct 26 14:02:30 2021, max compression
+gzip compressed data, was "factory_boy-3.3.0.tar", last modified: Wed Jul 19 09:03:57 2023, max compression
```

## Comparing `factory_boy-3.2.1.tar` & `factory_boy-3.3.0.tar`

### file list

```diff
@@ -1,116 +1,118 @@
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3235 2021-10-26 14:02:29.000000 factory_boy-3.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2773 2021-10-26 14:02:29.000000 factory_boy-3.2.1/CONTRIBUTING.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     4317 2021-10-26 14:02:29.000000 factory_boy-3.2.1/CREDITS
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    28895 2021-10-26 14:02:29.000000 factory_boy-3.2.1/ChangeLog
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1136 2021-10-26 14:02:29.000000 factory_boy-3.2.1/LICENSE
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      264 2021-10-26 14:02:29.000000 factory_boy-3.2.1/MANIFEST.in
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3323 2021-10-26 14:02:29.000000 factory_boy-3.2.1/Makefile
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    13801 2021-10-26 14:02:30.000000 factory_boy-3.2.1/PKG-INFO
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    12295 2021-10-26 14:02:29.000000 factory_boy-3.2.1/README.rst
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/docs/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      634 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/Makefile
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/docs/_static/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/_static/.keep_dir
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    28895 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/changelog.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3072 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/conf.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     4317 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/credits.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3775 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/examples.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    10457 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/fuzzy.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      416 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/ideas.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      298 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/index.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3482 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/internals.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     9383 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/introduction.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    21638 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/logo.png
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     6729 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/logo.svg
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      795 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/make.bat
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    17600 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/orms.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    18379 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/recipes.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    63507 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/reference.rst
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      321 2021-10-26 14:02:29.000000 factory_boy-3.2.1/docs/spelling_wordlist.txt
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/examples/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      164 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/Makefile
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/examples/django_demo/
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/examples/django_demo/django_demo/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/django_demo/__init__.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3134 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/django_demo/settings.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      768 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/django_demo/urls.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      400 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/django_demo/wsgi.py
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/examples/django_demo/generic_foreignkey/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/generic_foreignkey/__init__.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      110 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/generic_foreignkey/apps.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      998 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/generic_foreignkey/factories.py
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/examples/django_demo/generic_foreignkey/migrations/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      837 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/generic_foreignkey/migrations/0001_initial.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/generic_foreignkey/migrations/__init__.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      513 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/generic_foreignkey/models.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1080 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/generic_foreignkey/tests.py
--rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)      823 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/manage.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        7 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/requirements.txt
--rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)       51 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/django_demo/runtests.sh
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/examples/flask_alchemy/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      994 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/flask_alchemy/demoapp.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      537 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/flask_alchemy/demoapp_factories.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)       23 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/flask_alchemy/requirements.txt
--rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)       88 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/flask_alchemy/runtests.sh
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      933 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/flask_alchemy/test_demoapp.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)       66 2021-10-26 14:02:29.000000 factory_boy-3.2.1/examples/requirements.txt
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/factory/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1507 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/__init__.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3984 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/alchemy.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    23836 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/base.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    12170 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/builder.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    24694 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/declarations.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    10904 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/django.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      557 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/enums.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      748 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/errors.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1958 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/faker.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     8887 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/fuzzy.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3408 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/helpers.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      526 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/mogo.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      586 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/mongoengine.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      729 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/random.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3106 2021-10-26 14:02:29.000000 factory_boy-3.2.1/factory/utils.py
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/factory_boy.egg-info/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    13801 2021-10-26 14:02:30.000000 factory_boy-3.2.1/factory_boy.egg-info/PKG-INFO
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2459 2021-10-26 14:02:30.000000 factory_boy-3.2.1/factory_boy.egg-info/SOURCES.txt
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        1 2021-10-26 14:02:30.000000 factory_boy-3.2.1/factory_boy.egg-info/dependency_links.txt
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        1 2021-10-26 14:02:30.000000 factory_boy-3.2.1/factory_boy.egg-info/not-zip-safe
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      178 2021-10-26 14:02:30.000000 factory_boy-3.2.1/factory_boy.egg-info/requires.txt
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        8 2021-10-26 14:02:30.000000 factory_boy-3.2.1/factory_boy.egg-info/top_level.txt
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1850 2021-10-26 14:02:30.000000 factory_boy-3.2.1/setup.cfg
--rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)       61 2021-10-26 14:02:29.000000 factory_boy-3.2.1/setup.py
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/tests/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/__init__.py
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/tests/alchemyapp/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/alchemyapp/__init__.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1300 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/alchemyapp/models.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3556 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/alter_time.py
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/tests/cyclic/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/cyclic/__init__.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      330 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/cyclic/bar.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      355 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/cyclic/foo.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      435 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/cyclic/self_ref.py
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/tests/djapp/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/djapp/__init__.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2789 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/djapp/models.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      653 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/djapp/settings.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     9609 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_alchemy.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    16471 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_base.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    11113 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_declarations.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1902 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_dev_experience.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    34762 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_django.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     4271 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_docs_internals.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     5835 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_faker.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    21305 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_fuzzy.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1980 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_helpers.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2146 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_mongoengine.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1134 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_regression.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)    94459 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_using.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     5303 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/test_utils.py
-drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2021-10-26 14:02:30.000000 factory_boy-3.2.1/tests/testdata/
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      233 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/testdata/__init__.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)       13 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/testdata/example.data
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)      301 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/testdata/example.jpeg
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2057 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tests/utils.py
--rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1151 2021-10-26 14:02:29.000000 factory_boy-3.2.1/tox.ini
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.918965 factory_boy-3.3.0/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3235 2023-07-19 09:03:57.000000 factory_boy-3.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2773 2023-07-19 09:03:57.000000 factory_boy-3.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     4444 2023-07-19 09:03:57.000000 factory_boy-3.3.0/CREDITS
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    31112 2023-07-19 09:03:57.000000 factory_boy-3.3.0/ChangeLog
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1136 2023-07-19 09:03:57.000000 factory_boy-3.3.0/LICENSE
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      264 2023-07-19 09:03:57.000000 factory_boy-3.3.0/MANIFEST.in
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3335 2023-07-19 09:03:57.000000 factory_boy-3.3.0/Makefile
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    14790 2023-07-19 09:03:57.918965 factory_boy-3.3.0/PKG-INFO
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    13254 2023-07-19 09:03:57.000000 factory_boy-3.3.0/README.rst
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.911965 factory_boy-3.3.0/docs/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      634 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/Makefile
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.911965 factory_boy-3.3.0/docs/_static/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/_static/.keep_dir
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    31112 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/changelog.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3297 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/conf.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     4444 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/credits.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3757 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/examples.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    10167 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/fuzzy.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      416 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/ideas.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      298 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/index.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3481 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/internals.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     9776 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/introduction.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    21638 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/logo.png
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     6729 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/logo.svg
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      795 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/make.bat
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    19500 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/orms.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    18687 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/recipes.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    64658 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/reference.rst
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      321 2023-07-19 09:03:57.000000 factory_boy-3.3.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.911965 factory_boy-3.3.0/examples/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      164 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/Makefile
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.911965 factory_boy-3.3.0/examples/django_demo/
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.912965 factory_boy-3.3.0/examples/django_demo/django_demo/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/django_demo/__init__.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3134 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/django_demo/settings.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      763 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/django_demo/urls.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      400 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/django_demo/wsgi.py
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.912965 factory_boy-3.3.0/examples/django_demo/generic_foreignkey/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/generic_foreignkey/__init__.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      110 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/generic_foreignkey/apps.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      998 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/generic_foreignkey/factories.py
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.912965 factory_boy-3.3.0/examples/django_demo/generic_foreignkey/migrations/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      837 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/generic_foreignkey/migrations/0001_initial.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/generic_foreignkey/migrations/__init__.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      513 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/generic_foreignkey/models.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1080 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/generic_foreignkey/tests.py
+-rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)      252 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/manage.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        7 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/requirements.txt
+-rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)       51 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/django_demo/runtests.sh
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.913965 factory_boy-3.3.0/examples/flask_alchemy/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      994 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/flask_alchemy/demoapp.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      537 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/flask_alchemy/demoapp_factories.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)       23 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/flask_alchemy/requirements.txt
+-rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)       88 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/flask_alchemy/runtests.sh
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1051 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/flask_alchemy/test_demoapp.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)       66 2023-07-19 09:03:57.000000 factory_boy-3.3.0/examples/requirements.txt
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.914965 factory_boy-3.3.0/factory/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1480 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/__init__.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     4637 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/alchemy.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    23836 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/base.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    12923 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/builder.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    26652 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/declarations.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    12084 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/django.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      557 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/enums.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      748 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/errors.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1958 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/faker.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     8887 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/fuzzy.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3408 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/helpers.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      526 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/mogo.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      586 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/mongoengine.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      729 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/random.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3106 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory/utils.py
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.915965 factory_boy-3.3.0/factory_boy.egg-info/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    14790 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory_boy.egg-info/PKG-INFO
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2500 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory_boy.egg-info/SOURCES.txt
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        1 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory_boy.egg-info/dependency_links.txt
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      241 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory_boy.egg-info/requires.txt
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        8 2023-07-19 09:03:57.000000 factory_boy-3.3.0/factory_boy.egg-info/top_level.txt
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2092 2023-07-19 09:03:57.918965 factory_boy-3.3.0/setup.cfg
+-rwxr-xr-x   0 xelnor    (1000) xelnet    (1000)       61 2023-07-19 09:03:57.000000 factory_boy-3.3.0/setup.py
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.916965 factory_boy-3.3.0/tests/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/__init__.py
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.917966 factory_boy-3.3.0/tests/alchemyapp/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/alchemyapp/__init__.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2182 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/alchemyapp/models.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     3556 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/alter_time.py
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.917966 factory_boy-3.3.0/tests/cyclic/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/cyclic/__init__.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      330 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/cyclic/bar.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      355 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/cyclic/foo.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      435 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/cyclic/self_ref.py
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.917966 factory_boy-3.3.0/tests/djapp/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/djapp/__init__.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2977 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/djapp/models.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      783 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/djapp/settings.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1257 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/djapp/settings_pg.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    11427 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_alchemy.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    16467 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_base.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    11319 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_declarations.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1902 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_dev_experience.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    39506 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_django.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     4271 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_docs_internals.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     5836 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_faker.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    21305 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_fuzzy.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1980 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_helpers.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2150 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_mongoengine.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1134 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_regression.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     6894 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_transformer.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)    94980 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_using.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     5303 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_utils.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      200 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/test_version.py
+drwxr-xr-x   0 xelnor    (1000) xelnet    (1000)        0 2023-07-19 09:03:57.918965 factory_boy-3.3.0/tests/testdata/
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      233 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/testdata/__init__.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)       13 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/testdata/example.data
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)      301 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/testdata/example.jpeg
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     2057 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tests/utils.py
+-rw-r--r--   0 xelnor    (1000) xelnet    (1000)     1688 2023-07-19 09:03:57.000000 factory_boy-3.3.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `factory_boy-3.2.1/CODE_OF_CONDUCT.md` & `factory_boy-3.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/CONTRIBUTING.rst` & `factory_boy-3.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/CREDITS` & `factory_boy-3.3.0/CREDITS`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 * Hugo Osvaldo Barrera <hugo@barrera.io>
 * Ilya Baryshev <baryshev@gmail.com>
 * Ilya Pirogov <ilja.pirogov@gmail.com>
 * Ionuț Arțăriși <ionut@artarisi.eu>
 * Issa Jubril <issa.jubril@andela.com>
 * Ivan Miric <imiric@gmail.com>
 * Janusz Skonieczny <wooyek@users.noreply.github.com>
+* Javier Buzzi <kingbuzzman@users.noreply.github.com> (https://github.com/kingbuzzman)
 * Jeff Widman <jeff@jeffwidman.com> (https://github.com/jeffwidman)
 * Jon Dufresne <jon.dufresne@gmail.com>
 * Jonathan Tushman <jtushman@pipewave.com>
 * Joshua Carp <jm.carp@gmail.com>
 * Leonardo Lazzaro <llazzaro@dc.uba.ar>
 * Luke GB <github@lukegb.com>
 * Marc Abramowitz <marc@marc-abramowitz.com>
@@ -67,14 +68,15 @@
 * QuantumGhost <obelisk.reg+github@gmail.com>
 * Raphaël Barrois <raphael.barrois+fboy@polytechnique.org> (https://github.com/rbarrois)
 * Rich Rauenzahn <rich@vmware.com>
 * Richard Moch <richard@mbp.polyconseil.fr>
 * Rob Zyskowski <zyskowski.rob@gmail.com>
 * Robrecht De Rouck <Robrecht.De.Rouck@gmail.com>
 * Samuel Paccoud <samuel@sampaccoud.com>
+* Sarah Boyce <sarahvboyce95@gmail.com>
 * Saul Shanabrook <s.shanabrook@gmail.com>
 * Sean Löfgren <SeanBE@users.noreply.github.com>
 * Shahriar Tajbakhsh <shahriar@metaview.ai>
 * Tom <tom@tomleo.com>
 * alex-netquity <alex@netquity.com>
 * anentropic <ego@anentropic.com>
 * minimumserious <commande.romain@gmail.com>
```

### Comparing `factory_boy-3.2.1/ChangeLog` & `factory_boy-3.3.0/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,87 @@
 ChangeLog
 =========
 
 .. Note for v4.x: don't forget to check "Deprecated" sections for removal.
 
-3.2.1 (2021-10-26)
+3.3.0 (2023-07-19)
 ------------------
 
 *New:*
 
+    - :issue:`366`: Add :class:`factory.django.Password` to generate Django :class:`~django.contrib.auth.models.User`
+      passwords.
+    - :issue:`304`: Add :attr:`~factory.alchemy.SQLAlchemyOptions.sqlalchemy_session_factory` to dynamically
+      create sessions for use by the :class:`~factory.alchemy.SQLAlchemyModelFactory`.
+    - Add support for Django 4.0
+    - Add support for Django 4.1
+    - Add support for Python 3.10
+    - Add support for Python 3.11
+
+*Bugfix:*
+
+    - Make :meth:`~factory.django.mute_signals` mute signals during post-generation.
+
+    - :issue:`775`: Change the signature for :meth:`~factory.alchemy.SQLAlchemyModelFactory._save` and
+      :meth:`~factory.alchemy.SQLAlchemyModelFactory._get_or_create` to avoid argument names clashes with a field named
+      ``session``.
+
+*Deprecated:*
+
+    - :class:`~factory.django.DjangoModelFactory` will stop issuing a second call to
+      :meth:`~django.db.models.Model.save` on the created instance when :ref:`post-generation-hooks` return a value.
+
+      To help with the transition, :class:`factory.django.DjangoModelFactory._after_postgeneration` raises a
+      :class:`DeprecationWarning` when calling :meth:`~django.db.models.Model.save`. Inspect your
+      :class:`~factory.django.DjangoModelFactory` subclasses:
+
+      - If the :meth:`~django.db.models.Model.save` call is not needed after :class:`~factory.PostGeneration`, set
+        :attr:`factory.django.DjangoOptions.skip_postgeneration_save` to ``True`` in the factory meta.
+
+      - Otherwise, the instance has been modified by :class:`~factory.PostGeneration` hooks and needs to be
+        :meth:`~django.db.models.Model.save`\ d. Either:
+
+          - call :meth:`django.db.models.Model.save` in the :class:`~factory.PostGeneration` hook that modifies the
+            instance, or
+          - override :class:`~factory.django.DjangoModelFactory._after_postgeneration` to
+            :meth:`~django.db.models.Model.save` the instance.
+
+*Removed:*
+
+    - Drop support for Django 2.2
+    - Drop support for Django 3.0
+    - Drop support for Django 3.1
+    - Drop support for Python 3.6
+
+3.2.1 (2021-10-26)
+------------------
+
+*New:*
     - Add support for Django 3.2
 
 *Bugfix:*
 
     - Do not override signals receivers registered in a :meth:`~factory.django.mute_signals` context.
 
     - :issue:`775`: Change the signature for :meth:`~factory.alchemy.SQLAlchemyModelFactory._save` and
       :meth:`~factory.alchemy.SQLAlchemyModelFactory._get_or_create` to avoid argument names clashes with a field named
       ``session``.
 
-
 3.2.0 (2020-12-28)
 ------------------
 
 *New:*
 
     - Add support for Django 3.1
     - Add support for Python 3.9
 
 *Removed:*
 
     - Drop support for Django 1.11. This version `is not maintained anymore <https://www.djangoproject.com/download/#supported-versions>`__.
-    - Drop support for Python 3.5. This version `is not maintained anymore <https://devguide.python.org/devcycle/#end-of-life-branches>`__.
+    - Drop support for Python 3.5. This version `is not maintained anymore <https://devguide.python.org/developer-workflow/development-cycle/index.html#end-of-life-branches>`__.
 
 *Deprecated:*
 
     - :func:`factory.use_strategy`. Use :attr:`factory.FactoryOptions.strategy` instead.
       The purpose of :func:`~factory.use_strategy` duplicates the factory option. Follow :pep:`20`: *There should be
       one-- and preferably only one --obvious way to do it.*
 
@@ -83,15 +130,15 @@
 | ``from factory.fuzzy import set_random_state`` | ``from factory.random import set_random_state``   |
 +------------------------------------------------+---------------------------------------------------+
 | ``from factory.fuzzy import reseed_random``    | ``from factory.random import reseed_random``      |
 +------------------------------------------------+---------------------------------------------------+
 
 *Removed:*
 
-    - Drop support for Python 2 and 3.4. These versions `are not maintained anymore <https://devguide.python.org/devcycle/#end-of-life-branches>`__.
+    - Drop support for Python 2 and 3.4. These versions `are not maintained anymore <https://devguide.python.org/developer-workflow/development-cycle/index.html#end-of-life-branches>`__.
     - Drop support for Django 2.0 and 2.1. These versions `are not maintained anymore <https://www.djangoproject.com/download/#supported-versions>`__.
     - Remove deprecated ``force_flush`` from ``SQLAlchemyModelFactory`` options. Use
       ``sqlalchemy_session_persistence = "flush"`` instead.
     - Drop deprecated ``attributes()`` from :class:`~factory.Factory` subclasses; use
       ``factory.make_factory(dict, FactoryClass._meta.pre_declarations)`` instead.
     - Drop deprecated ``declarations()`` from :class:`~factory.Factory` subclasses; use ``FactoryClass._meta.pre_declarations`` instead.
     - Drop ``factory.compat`` module.
@@ -415,15 +462,15 @@
 .. _v2.3.1:
 
 2.3.1 (2014-01-22)
 ------------------
 
 *Bug fix:*
 
-    - Fix badly written assert containing state-changing code, spotted by `chsigi <https://github.com/chsigi>`_ (:pr:`126`)
+    - Fix badly written assert containing state-changing code, spotted by ``chsigi`` (:pr:`126`)
     - Don't crash when handling objects whose ``__repr__`` is non-pure-ASCII bytes on Python 2,
       discovered by `mbertheau <https://github.com/mbertheau>`_ (:issue:`123`) and `strycore <https://github.com/strycore>`_ (:pr:`127`)
 
 .. _v2.3.0:
 
 2.3.0 (2013-12-25)
 ------------------
```

### Comparing `factory_boy-3.2.1/LICENSE` & `factory_boy-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/Makefile` & `factory_boy-3.3.0/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -48,161 +48,162 @@
 000002f0: 616c 6c20 7375 7070 6f72 7465 6420 7665  all supported ve
 00000300: 7273 696f 6e73 2028 6372 6561 7465 7320  rsions (creates 
 00000310: 6120 7365 7420 6f66 2076 6972 7475 616c  a set of virtual
 00000320: 656e 7673 290a 7465 7374 616c 6c3a 0a09  envs).testall:..
 00000330: 746f 780a 0a23 2044 4f43 3a20 5275 6e20  tox..# DOC: Run 
 00000340: 7465 7374 7320 666f 7220 7468 6520 6375  tests for the cu
 00000350: 7272 656e 746c 7920 696e 7374 616c 6c65  rrently installe
-00000360: 6420 7665 7273 696f 6e0a 7465 7374 3a0a  d version.test:.
-00000370: 0970 7974 686f 6e20 5c0a 0909 2d62 205c  .python \...-b \
-00000380: 0a09 092d 5820 6465 7620 5c0a 0909 2d57  ...-X dev \...-W
-00000390: 6572 726f 7220 5c0a 0909 2d57 6465 6661  error \...-Wdefa
-000003a0: 756c 743a 2274 6865 2069 6d70 206d 6f64  ult:"the imp mod
-000003b0: 756c 6520 6973 2064 6570 7265 6361 7465  ule is deprecate
-000003c0: 6420 696e 2066 6176 6f75 7220 6f66 2069  d in favour of i
-000003d0: 6d70 6f72 746c 6962 3b20 7365 6520 7468  mportlib; see th
-000003e0: 6520 6d6f 6475 6c65 2773 2064 6f63 756d  e module's docum
-000003f0: 656e 7461 7469 6f6e 2066 6f72 2061 6c74  entation for alt
-00000400: 6572 6e61 7469 7665 2075 7365 7322 3a44  ernative uses":D
-00000410: 6570 7265 6361 7469 6f6e 5761 726e 696e  eprecationWarnin
-00000420: 673a 6469 7374 7574 696c 733a 205c 0a09  g:distutils: \..
-00000430: 092d 5764 6566 6175 6c74 3a22 5573 696e  .-Wdefault:"Usin
-00000440: 6720 6f72 2069 6d70 6f72 7469 6e67 2074  g or importing t
-00000450: 6865 2041 4243 7320 6672 6f6d 2027 636f  he ABCs from 'co
-00000460: 6c6c 6563 7469 6f6e 7327 2069 6e73 7465  llections' inste
-00000470: 6164 206f 6620 6672 6f6d 2027 636f 6c6c  ad of from 'coll
-00000480: 6563 7469 6f6e 732e 6162 6327 2069 7320  ections.abc' is 
-00000490: 6465 7072 6563 6174 6564 2c20 616e 6420  deprecated, and 
-000004a0: 696e 2033 2e38 2069 7420 7769 6c6c 2073  in 3.8 it will s
-000004b0: 746f 7020 776f 726b 696e 6722 3a44 6570  top working":Dep
-000004c0: 7265 6361 7469 6f6e 5761 726e 696e 673a  recationWarning:
-000004d0: 3a20 5c0a 0909 2d57 6465 6661 756c 743a  : \...-Wdefault:
-000004e0: 2255 7369 6e67 206f 7220 696d 706f 7274  "Using or import
-000004f0: 696e 6720 7468 6520 4142 4373 2066 726f  ing the ABCs fro
-00000500: 6d20 2763 6f6c 6c65 6374 696f 6e73 2720  m 'collections' 
-00000510: 696e 7374 6561 6420 6f66 2066 726f 6d20  instead of from 
-00000520: 2763 6f6c 6c65 6374 696f 6e73 2e61 6263  'collections.abc
-00000530: 2720 6973 2064 6570 7265 6361 7465 6420  ' is deprecated 
-00000540: 7369 6e63 6520 5079 7468 6f6e 2033 2e33  since Python 3.3
-00000550: 2c20 616e 6420 696e 2033 2e39 2069 7420  , and in 3.9 it 
-00000560: 7769 6c6c 2073 746f 7020 776f 726b 696e  will stop workin
-00000570: 6722 3a44 6570 7265 6361 7469 6f6e 5761  g":DeprecationWa
-00000580: 726e 696e 673a 3a20 5c0a 0909 2d57 6465  rning:: \...-Wde
-00000590: 6661 756c 743a 2273 6574 5f6f 7574 7075  fault:"set_outpu
-000005a0: 745f 6368 6172 7365 7428 2920 6973 2064  t_charset() is d
-000005b0: 6570 7265 6361 7465 6422 3a44 6570 7265  eprecated":Depre
-000005c0: 6361 7469 6f6e 5761 726e 696e 673a 3a20  cationWarning:: 
-000005d0: 5c0a 0909 2d57 6465 6661 756c 743a 2270  \...-Wdefault:"p
-000005e0: 6172 616d 6574 6572 2063 6f64 6573 6574  arameter codeset
-000005f0: 2069 7320 6465 7072 6563 6174 6564 223a   is deprecated":
-00000600: 4465 7072 6563 6174 696f 6e57 6172 6e69  DeprecationWarni
-00000610: 6e67 3a3a 205c 0a09 092d 6d20 756e 6974  ng:: \...-m unit
-00000620: 7465 7374 0a0a 2320 444f 433a 2054 6573  test..# DOC: Tes
-00000630: 7420 7468 6520 6578 616d 706c 6573 0a65  t the examples.e
-00000640: 7861 6d70 6c65 2d74 6573 743a 0a09 2428  xample-test:..$(
-00000650: 4d41 4b45 2920 2d43 2024 2845 5841 4d50  MAKE) -C $(EXAMP
-00000660: 4c45 535f 4449 5229 2074 6573 740a 0a0a  LES_DIR) test...
-00000670: 0a23 204e 6f74 653a 2077 6520 7275 6e20  .# Note: we run 
-00000680: 7468 6520 6c69 6e74 6572 2069 6e20 7477  the linter in tw
-00000690: 6f20 7275 6e73 2c20 6265 6361 7573 6520  o runs, because 
-000006a0: 6f75 7220 5f5f 696e 6974 5f5f 2e70 7920  our __init__.py 
-000006b0: 6669 6c65 7320 6861 7320 7370 6563 6966  files has specif
-000006c0: 6963 2077 6172 6e69 6e67 7320 7765 2077  ic warnings we w
-000006d0: 616e 7420 746f 2065 7863 6c75 6465 0a23  ant to exclude.#
-000006e0: 2044 4f43 3a20 5065 7266 6f72 6d20 636f   DOC: Perform co
-000006f0: 6465 2071 7561 6c69 7479 2074 6173 6b73  de quality tasks
-00000700: 0a6c 696e 743a 0a09 2428 464c 414b 4538  .lint:..$(FLAKE8
-00000710: 2920 2d2d 6578 636c 7564 6520 2428 5041  ) --exclude $(PA
-00000720: 434b 4147 4529 2f5f 5f69 6e69 745f 5f2e  CKAGE)/__init__.
-00000730: 7079 2024 2845 5841 4d50 4c45 535f 4449  py $(EXAMPLES_DI
-00000740: 5229 2024 2850 4143 4b41 4745 2920 2428  R) $(PACKAGE) $(
-00000750: 5345 5455 505f 5059 2920 2428 5445 5354  SETUP_PY) $(TEST
-00000760: 535f 4449 5229 0a09 2428 464c 414b 4538  S_DIR)..$(FLAKE8
-00000770: 2920 2d2d 6967 6e6f 7265 2046 3430 3120  ) --ignore F401 
-00000780: 2428 5041 434b 4147 4529 2f5f 5f69 6e69  $(PACKAGE)/__ini
-00000790: 745f 5f2e 7079 0a09 2428 4953 4f52 5429  t__.py..$(ISORT)
-000007a0: 202d 2d63 6865 636b 2d6f 6e6c 7920 2d2d   --check-only --
-000007b0: 6469 6666 2024 2845 5841 4d50 4c45 535f  diff $(EXAMPLES_
-000007c0: 4449 5229 2024 2850 4143 4b41 4745 2920  DIR) $(PACKAGE) 
-000007d0: 2428 5345 5455 505f 5059 2920 2428 5445  $(SETUP_PY) $(TE
-000007e0: 5354 535f 4449 5229 0a09 6368 6563 6b2d  STS_DIR)..check-
-000007f0: 6d61 6e69 6665 7374 0a0a 636f 7665 7261  manifest..covera
-00000800: 6765 3a0a 0924 2843 4f56 4552 4147 4529  ge:..$(COVERAGE)
-00000810: 2065 7261 7365 0a09 2428 434f 5645 5241   erase..$(COVERA
-00000820: 4745 2920 7275 6e20 222d 2d69 6e63 6c75  GE) run "--inclu
-00000830: 6465 3d24 2850 4143 4b41 4745 292f 2a2e  de=$(PACKAGE)/*.
-00000840: 7079 2c24 2854 4553 5453 5f44 4952 292f  py,$(TESTS_DIR)/
-00000850: 2a2e 7079 2220 2d2d 6272 616e 6368 2024  *.py" --branch $
-00000860: 2853 4554 5550 5f50 5929 2074 6573 740a  (SETUP_PY) test.
-00000870: 0924 2843 4f56 4552 4147 4529 2072 6570  .$(COVERAGE) rep
-00000880: 6f72 7420 222d 2d69 6e63 6c75 6465 3d24  ort "--include=$
-00000890: 2850 4143 4b41 4745 292f 2a2e 7079 2c24  (PACKAGE)/*.py,$
-000008a0: 2854 4553 5453 5f44 4952 292f 2a2e 7079  (TESTS_DIR)/*.py
-000008b0: 220a 0924 2843 4f56 4552 4147 4529 2068  "..$(COVERAGE) h
-000008c0: 746d 6c20 222d 2d69 6e63 6c75 6465 3d24  tml "--include=$
-000008d0: 2850 4143 4b41 4745 292f 2a2e 7079 2c24  (PACKAGE)/*.py,$
-000008e0: 2854 4553 5453 5f44 4952 292f 2a2e 7079  (TESTS_DIR)/*.py
-000008f0: 220a 0a0a 2e50 484f 4e59 3a20 7465 7374  "....PHONY: test
-00000900: 2074 6573 7461 6c6c 2065 7861 6d70 6c65   testall example
-00000910: 2d74 6573 7420 6c69 6e74 2063 6f76 6572  -test lint cover
-00000920: 6167 650a 0a0a 2320 4465 7665 6c6f 706d  age...# Developm
-00000930: 656e 740a 2320 3d3d 3d3d 3d3d 3d3d 3d3d  ent.# ==========
-00000940: 3d0a 0a23 2044 4f43 3a20 4765 6e65 7261  =..# DOC: Genera
-00000950: 7465 2061 2022 7461 6773 2220 6669 6c65  te a "tags" file
-00000960: 0a54 4147 533a 0a09 2428 4354 4147 5329  .TAGS:..$(CTAGS)
-00000970: 202d 2d72 6563 7572 7365 2024 2850 4143   --recurse $(PAC
-00000980: 4b41 4745 2920 2428 5445 5354 535f 4449  KAGE) $(TESTS_DI
-00000990: 5229 0a0a 2e50 484f 4e59 3a20 5441 4753  R)...PHONY: TAGS
-000009a0: 0a0a 0a23 2044 6f63 756d 656e 7461 7469  ...# Documentati
-000009b0: 6f6e 0a23 203d 3d3d 3d3d 3d3d 3d3d 3d3d  on.# ===========
-000009c0: 3d3d 0a0a 0a23 2044 4f43 3a20 436f 6d70  ==...# DOC: Comp
-000009d0: 696c 6520 7468 6520 646f 6375 6d65 6e74  ile the document
-000009e0: 6174 696f 6e0a 646f 633a 0a09 2428 4d41  ation.doc:..$(MA
-000009f0: 4b45 2920 2d43 2024 2844 4f43 5f44 4952  KE) -C $(DOC_DIR
-00000a00: 2920 5350 4849 4e58 4f50 5453 3d2d 5720  ) SPHINXOPTS=-W 
-00000a10: 6874 6d6c 0a0a 6c69 6e6b 6368 6563 6b3a  html..linkcheck:
-00000a20: 0a09 2428 4d41 4b45 2920 2d43 2024 2844  ..$(MAKE) -C $(D
-00000a30: 4f43 5f44 4952 2920 6c69 6e6b 6368 6563  OC_DIR) linkchec
-00000a40: 6b0a 0a73 7065 6c6c 696e 673a 0a09 2428  k..spelling:..$(
-00000a50: 4d41 4b45 2920 2d43 2024 2844 4f43 5f44  MAKE) -C $(DOC_D
-00000a60: 4952 2920 5350 4849 4e58 4f50 5453 3d2d  IR) SPHINXOPTS=-
-00000a70: 5720 7370 656c 6c69 6e67 0a0a 2320 444f  W spelling..# DO
-00000a80: 433a 2053 686f 7720 7468 6973 2068 656c  C: Show this hel
-00000a90: 7020 6d65 7373 6167 650a 6865 6c70 3a0a  p message.help:.
-00000aa0: 0940 6772 6570 202d 4131 2027 5e23 2044  .@grep -A1 '^# D
-00000ab0: 4f43 3a27 204d 616b 6566 696c 6520 5c0a  OC:' Makefile \.
-00000ac0: 0920 7c20 6177 6b20 2720 2020 2009 0909  . | awk '    ...
-00000ad0: 0909 5c0a 0920 2020 2042 4547 494e 207b  ..\..    BEGIN {
-00000ae0: 2046 533d 225c 6e22 3b20 5253 3d22 2d2d   FS="\n"; RS="--
-00000af0: 5c6e 223b 206f 7074 5f6c 656e 3d30 3b20  \n"; opt_len=0; 
-00000b00: 7d20 2020 205c 0a09 2020 2020 7b20 2020  }    \..    {   
-00000b10: 2009 0909 0909 5c0a 0909 646f 633d 2424   .....\...doc=$$
-00000b20: 313b 206e 616d 653d 2424 323b 2020 2020  1; name=$$2;    
-00000b30: 0909 095c 0a09 0973 7562 2822 2320 444f  ...\...sub("# DO
-00000b40: 433a 2022 2c20 2222 2c20 646f 6329 3b20  C: ", "", doc); 
-00000b50: 2020 2009 095c 0a09 0973 7562 2822 3a22     ..\...sub(":"
-00000b60: 2c20 2222 2c20 6e61 6d65 293b 2020 2020  , "", name);    
-00000b70: 0909 095c 0a09 0969 6620 286c 656e 6774  ...\...if (lengt
-00000b80: 6828 6e61 6d65 2920 3e20 6f70 745f 6c65  h(name) > opt_le
-00000b90: 6e29 207b 2020 2020 095c 0a09 0920 2020  n) {    .\...   
-00000ba0: 206f 7074 5f6c 656e 203d 206c 656e 6774   opt_len = lengt
-00000bb0: 6828 6e61 6d65 2920 2020 2009 095c 0a09  h(name)    ..\..
-00000bc0: 097d 2020 2020 0909 0909 095c 0a09 096f  .}    .....\...o
-00000bd0: 7074 735b 4e52 5d20 3d20 6e61 6d65 3b20  pts[NR] = name; 
-00000be0: 2020 2009 0909 5c0a 0909 646f 6373 5b6e     ...\...docs[n
-00000bf0: 616d 655d 203d 2064 6f63 3b20 2020 2009  ame] = doc;    .
-00000c00: 0909 5c0a 0920 2020 207d 2020 2020 0909  ..\..    }    ..
-00000c10: 0909 095c 0a09 2020 2020 454e 4420 7b20  ...\..    END { 
-00000c20: 2020 2009 0909 0909 5c0a 0909 7061 743d     .....\...pat=
-00000c30: 2225 2d22 2028 6f70 745f 6c65 6e20 2b20  "%-" (opt_len + 
-00000c40: 3429 2022 7320 2573 5c6e 223b 2020 2020  4) "s %s\n";    
-00000c50: 095c 0a09 0961 736f 7274 286f 7074 7329  .\...asort(opts)
-00000c60: 3b20 2020 2009 0909 5c0a 0909 666f 7220  ;    ...\...for 
-00000c70: 2869 2069 6e20 6f70 7473 2920 7b20 2020  (i in opts) {   
-00000c80: 2009 0909 5c0a 0909 2020 2020 6f70 743d   ...\...    opt=
-00000c90: 6f70 7473 5b69 5d3b 2020 2020 0909 095c  opts[i];    ...\
-00000ca0: 0a09 0920 2020 2070 7269 6e74 6620 7061  ...    printf pa
-00000cb0: 742c 206f 7074 2c20 646f 6373 5b6f 7074  t, opt, docs[opt
-00000cc0: 5d20 2020 2009 5c0a 0909 7d20 2020 2009  ]    .\...}    .
-00000cd0: 0909 0909 5c0a 0920 2020 207d 270a 0a0a  ....\..    }'...
-00000ce0: 2e50 484f 4e59 3a20 646f 6320 6c69 6e6b  .PHONY: doc link
-00000cf0: 6368 6563 6b20 6865 6c70 0a              check help.
+00000360: 6420 7665 7273 696f 6e0a 2320 5265 6d6f  d version.# Remo
+00000370: 7665 2063 6769 2077 6172 6e69 6e67 2077  ve cgi warning w
+00000380: 6865 6e20 6472 6f70 7069 6e67 2073 7570  hen dropping sup
+00000390: 706f 7274 2066 6f72 2044 6a61 6e67 6f3c  port for Django<
+000003a0: 3d34 2e31 2e0a 7465 7374 3a0a 0970 7974  =4.1..test:..pyt
+000003b0: 686f 6e20 5c0a 0909 2d62 205c 0a09 092d  hon \...-b \...-
+000003c0: 5820 6465 7620 5c0a 0909 2d57 6572 726f  X dev \...-Werro
+000003d0: 7220 5c0a 0909 2d57 6465 6661 756c 743a  r \...-Wdefault:
+000003e0: 2274 6865 2069 6d70 206d 6f64 756c 6520  "the imp module 
+000003f0: 6973 2064 6570 7265 6361 7465 6420 696e  is deprecated in
+00000400: 2066 6176 6f75 7220 6f66 2069 6d70 6f72   favour of impor
+00000410: 746c 6962 3b20 7365 6520 7468 6520 6d6f  tlib; see the mo
+00000420: 6475 6c65 2773 2064 6f63 756d 656e 7461  dule's documenta
+00000430: 7469 6f6e 2066 6f72 2061 6c74 6572 6e61  tion for alterna
+00000440: 7469 7665 2075 7365 7322 3a44 6570 7265  tive uses":Depre
+00000450: 6361 7469 6f6e 5761 726e 696e 673a 6469  cationWarning:di
+00000460: 7374 7574 696c 733a 205c 0a09 092d 5764  stutils: \...-Wd
+00000470: 6566 6175 6c74 3a22 5573 696e 6720 6f72  efault:"Using or
+00000480: 2069 6d70 6f72 7469 6e67 2074 6865 2041   importing the A
+00000490: 4243 7320 6672 6f6d 2027 636f 6c6c 6563  BCs from 'collec
+000004a0: 7469 6f6e 7327 2069 6e73 7465 6164 206f  tions' instead o
+000004b0: 6620 6672 6f6d 2027 636f 6c6c 6563 7469  f from 'collecti
+000004c0: 6f6e 732e 6162 6327 2069 7320 6465 7072  ons.abc' is depr
+000004d0: 6563 6174 6564 2c20 616e 6420 696e 2033  ecated, and in 3
+000004e0: 2e38 2069 7420 7769 6c6c 2073 746f 7020  .8 it will stop 
+000004f0: 776f 726b 696e 6722 3a44 6570 7265 6361  working":Depreca
+00000500: 7469 6f6e 5761 726e 696e 673a 3a20 5c0a  tionWarning:: \.
+00000510: 0909 2d57 6465 6661 756c 743a 2255 7369  ..-Wdefault:"Usi
+00000520: 6e67 206f 7220 696d 706f 7274 696e 6720  ng or importing 
+00000530: 7468 6520 4142 4373 2066 726f 6d20 2763  the ABCs from 'c
+00000540: 6f6c 6c65 6374 696f 6e73 2720 696e 7374  ollections' inst
+00000550: 6561 6420 6f66 2066 726f 6d20 2763 6f6c  ead of from 'col
+00000560: 6c65 6374 696f 6e73 2e61 6263 2720 6973  lections.abc' is
+00000570: 2064 6570 7265 6361 7465 6420 7369 6e63   deprecated sinc
+00000580: 6520 5079 7468 6f6e 2033 2e33 2c20 616e  e Python 3.3, an
+00000590: 6420 696e 2033 2e39 2069 7420 7769 6c6c  d in 3.9 it will
+000005a0: 2073 746f 7020 776f 726b 696e 6722 3a44   stop working":D
+000005b0: 6570 7265 6361 7469 6f6e 5761 726e 696e  eprecationWarnin
+000005c0: 673a 3a20 5c0a 0909 2d57 6465 6661 756c  g:: \...-Wdefaul
+000005d0: 743a 2273 6574 5f6f 7574 7075 745f 6368  t:"set_output_ch
+000005e0: 6172 7365 7428 2920 6973 2064 6570 7265  arset() is depre
+000005f0: 6361 7465 6422 3a44 6570 7265 6361 7469  cated":Deprecati
+00000600: 6f6e 5761 726e 696e 673a 3a20 5c0a 0909  onWarning:: \...
+00000610: 2d57 6465 6661 756c 743a 2270 6172 616d  -Wdefault:"param
+00000620: 6574 6572 2063 6f64 6573 6574 2069 7320  eter codeset is 
+00000630: 6465 7072 6563 6174 6564 223a 4465 7072  deprecated":Depr
+00000640: 6563 6174 696f 6e57 6172 6e69 6e67 3a3a  ecationWarning::
+00000650: 205c 0a09 092d 5764 6566 6175 6c74 3a22   \...-Wdefault:"
+00000660: 2763 6769 2720 6973 2064 6570 7265 6361  'cgi' is depreca
+00000670: 7465 6420 616e 6420 736c 6174 6564 2066  ted and slated f
+00000680: 6f72 2072 656d 6f76 616c 2069 6e20 5079  or removal in Py
+00000690: 7468 6f6e 2033 2e31 3322 3a44 6570 7265  thon 3.13":Depre
+000006a0: 6361 7469 6f6e 5761 726e 696e 673a 3a20  cationWarning:: 
+000006b0: 5c0a 0909 2d6d 2075 6e69 7474 6573 740a  \...-m unittest.
+000006c0: 0a23 2044 4f43 3a20 5465 7374 2074 6865  .# DOC: Test the
+000006d0: 2065 7861 6d70 6c65 730a 6578 616d 706c   examples.exampl
+000006e0: 652d 7465 7374 3a0a 0924 284d 414b 4529  e-test:..$(MAKE)
+000006f0: 202d 4320 2428 4558 414d 504c 4553 5f44   -C $(EXAMPLES_D
+00000700: 4952 2920 7465 7374 0a0a 0a0a 2320 4e6f  IR) test....# No
+00000710: 7465 3a20 7765 2072 756e 2074 6865 206c  te: we run the l
+00000720: 696e 7465 7220 696e 2074 776f 2072 756e  inter in two run
+00000730: 732c 2062 6563 6175 7365 206f 7572 205f  s, because our _
+00000740: 5f69 6e69 745f 5f2e 7079 2066 696c 6573  _init__.py files
+00000750: 2068 6173 2073 7065 6369 6669 6320 7761   has specific wa
+00000760: 726e 696e 6773 2077 6520 7761 6e74 2074  rnings we want t
+00000770: 6f20 6578 636c 7564 650a 2320 444f 433a  o exclude.# DOC:
+00000780: 2050 6572 666f 726d 2063 6f64 6520 7175   Perform code qu
+00000790: 616c 6974 7920 7461 736b 730a 6c69 6e74  ality tasks.lint
+000007a0: 3a0a 0924 2846 4c41 4b45 3829 202d 2d65  :..$(FLAKE8) --e
+000007b0: 7863 6c75 6465 2024 2850 4143 4b41 4745  xclude $(PACKAGE
+000007c0: 292f 5f5f 696e 6974 5f5f 2e70 7920 2428  )/__init__.py $(
+000007d0: 4558 414d 504c 4553 5f44 4952 2920 2428  EXAMPLES_DIR) $(
+000007e0: 5041 434b 4147 4529 2024 2853 4554 5550  PACKAGE) $(SETUP
+000007f0: 5f50 5929 2024 2854 4553 5453 5f44 4952  _PY) $(TESTS_DIR
+00000800: 290a 0924 2846 4c41 4b45 3829 202d 2d69  )..$(FLAKE8) --i
+00000810: 676e 6f72 6520 4634 3031 2024 2850 4143  gnore F401 $(PAC
+00000820: 4b41 4745 292f 5f5f 696e 6974 5f5f 2e70  KAGE)/__init__.p
+00000830: 790a 0924 2849 534f 5254 2920 2d2d 6368  y..$(ISORT) --ch
+00000840: 6563 6b2d 6f6e 6c79 202d 2d64 6966 6620  eck-only --diff 
+00000850: 2428 4558 414d 504c 4553 5f44 4952 2920  $(EXAMPLES_DIR) 
+00000860: 2428 5041 434b 4147 4529 2024 2853 4554  $(PACKAGE) $(SET
+00000870: 5550 5f50 5929 2024 2854 4553 5453 5f44  UP_PY) $(TESTS_D
+00000880: 4952 290a 0963 6865 636b 2d6d 616e 6966  IR)..check-manif
+00000890: 6573 740a 0a63 6f76 6572 6167 653a 0a09  est..coverage:..
+000008a0: 2428 434f 5645 5241 4745 2920 6572 6173  $(COVERAGE) eras
+000008b0: 650a 0924 2843 4f56 4552 4147 4529 2072  e..$(COVERAGE) r
+000008c0: 756e 202d 2d62 7261 6e63 6820 2d6d 2075  un --branch -m u
+000008d0: 6e69 7474 6573 740a 0924 2843 4f56 4552  nittest..$(COVER
+000008e0: 4147 4529 2072 6570 6f72 740a 0924 2843  AGE) report..$(C
+000008f0: 4f56 4552 4147 4529 2068 746d 6c0a 0a0a  OVERAGE) html...
+00000900: 2e50 484f 4e59 3a20 7465 7374 2074 6573  .PHONY: test tes
+00000910: 7461 6c6c 2065 7861 6d70 6c65 2d74 6573  tall example-tes
+00000920: 7420 6c69 6e74 2063 6f76 6572 6167 650a  t lint coverage.
+00000930: 0a0a 2320 4465 7665 6c6f 706d 656e 740a  ..# Development.
+00000940: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a23  # ===========..#
+00000950: 2044 4f43 3a20 4765 6e65 7261 7465 2061   DOC: Generate a
+00000960: 2022 7461 6773 2220 6669 6c65 0a54 4147   "tags" file.TAG
+00000970: 533a 0a09 2428 4354 4147 5329 202d 2d72  S:..$(CTAGS) --r
+00000980: 6563 7572 7365 2024 2850 4143 4b41 4745  ecurse $(PACKAGE
+00000990: 2920 2428 5445 5354 535f 4449 5229 0a0a  ) $(TESTS_DIR)..
+000009a0: 2e50 484f 4e59 3a20 5441 4753 0a0a 0a23  .PHONY: TAGS...#
+000009b0: 2044 6f63 756d 656e 7461 7469 6f6e 0a23   Documentation.#
+000009c0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a   =============..
+000009d0: 0a23 2044 4f43 3a20 436f 6d70 696c 6520  .# DOC: Compile 
+000009e0: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+000009f0: 6e0a 646f 633a 0a09 2428 4d41 4b45 2920  n.doc:..$(MAKE) 
+00000a00: 2d43 2024 2844 4f43 5f44 4952 2920 5350  -C $(DOC_DIR) SP
+00000a10: 4849 4e58 4f50 5453 3d2d 5720 6874 6d6c  HINXOPTS=-W html
+00000a20: 0a0a 6c69 6e6b 6368 6563 6b3a 0a09 2428  ..linkcheck:..$(
+00000a30: 4d41 4b45 2920 2d43 2024 2844 4f43 5f44  MAKE) -C $(DOC_D
+00000a40: 4952 2920 6c69 6e6b 6368 6563 6b0a 0a73  IR) linkcheck..s
+00000a50: 7065 6c6c 696e 673a 0a09 2428 4d41 4b45  pelling:..$(MAKE
+00000a60: 2920 2d43 2024 2844 4f43 5f44 4952 2920  ) -C $(DOC_DIR) 
+00000a70: 5350 4849 4e58 4f50 5453 3d2d 5720 7370  SPHINXOPTS=-W sp
+00000a80: 656c 6c69 6e67 0a0a 2320 444f 433a 2053  elling..# DOC: S
+00000a90: 686f 7720 7468 6973 2068 656c 7020 6d65  how this help me
+00000aa0: 7373 6167 650a 6865 6c70 3a0a 0940 6772  ssage.help:..@gr
+00000ab0: 6570 202d 4131 2027 5e23 2044 4f43 3a27  ep -A1 '^# DOC:'
+00000ac0: 204d 616b 6566 696c 6520 5c0a 0920 7c20   Makefile \.. | 
+00000ad0: 6177 6b20 2720 2020 2009 0909 0909 5c0a  awk '    .....\.
+00000ae0: 0920 2020 2042 4547 494e 207b 2046 533d  .    BEGIN { FS=
+00000af0: 225c 6e22 3b20 5253 3d22 2d2d 5c6e 223b  "\n"; RS="--\n";
+00000b00: 206f 7074 5f6c 656e 3d30 3b20 7d20 2020   opt_len=0; }   
+00000b10: 205c 0a09 2020 2020 7b20 2020 2009 0909   \..    {    ...
+00000b20: 0909 5c0a 0909 646f 633d 2424 313b 206e  ..\...doc=$$1; n
+00000b30: 616d 653d 2424 323b 2020 2020 0909 095c  ame=$$2;    ...\
+00000b40: 0a09 0973 7562 2822 2320 444f 433a 2022  ...sub("# DOC: "
+00000b50: 2c20 2222 2c20 646f 6329 3b20 2020 2009  , "", doc);    .
+00000b60: 095c 0a09 0973 7562 2822 3a22 2c20 2222  .\...sub(":", ""
+00000b70: 2c20 6e61 6d65 293b 2020 2020 0909 095c  , name);    ...\
+00000b80: 0a09 0969 6620 286c 656e 6774 6828 6e61  ...if (length(na
+00000b90: 6d65 2920 3e20 6f70 745f 6c65 6e29 207b  me) > opt_len) {
+00000ba0: 2020 2020 095c 0a09 0920 2020 206f 7074      .\...    opt
+00000bb0: 5f6c 656e 203d 206c 656e 6774 6828 6e61  _len = length(na
+00000bc0: 6d65 2920 2020 2009 095c 0a09 097d 2020  me)    ..\...}  
+00000bd0: 2020 0909 0909 095c 0a09 096f 7074 735b    .....\...opts[
+00000be0: 4e52 5d20 3d20 6e61 6d65 3b20 2020 2009  NR] = name;    .
+00000bf0: 0909 5c0a 0909 646f 6373 5b6e 616d 655d  ..\...docs[name]
+00000c00: 203d 2064 6f63 3b20 2020 2009 0909 5c0a   = doc;    ...\.
+00000c10: 0920 2020 207d 2020 2020 0909 0909 095c  .    }    .....\
+00000c20: 0a09 2020 2020 454e 4420 7b20 2020 2009  ..    END {    .
+00000c30: 0909 0909 5c0a 0909 7061 743d 2225 2d22  ....\...pat="%-"
+00000c40: 2028 6f70 745f 6c65 6e20 2b20 3429 2022   (opt_len + 4) "
+00000c50: 7320 2573 5c6e 223b 2020 2020 095c 0a09  s %s\n";    .\..
+00000c60: 0961 736f 7274 286f 7074 7329 3b20 2020  .asort(opts);   
+00000c70: 2009 0909 5c0a 0909 666f 7220 2869 2069   ...\...for (i i
+00000c80: 6e20 6f70 7473 2920 7b20 2020 2009 0909  n opts) {    ...
+00000c90: 5c0a 0909 2020 2020 6f70 743d 6f70 7473  \...    opt=opts
+00000ca0: 5b69 5d3b 2020 2020 0909 095c 0a09 0920  [i];    ...\... 
+00000cb0: 2020 2070 7269 6e74 6620 7061 742c 206f     printf pat, o
+00000cc0: 7074 2c20 646f 6373 5b6f 7074 5d20 2020  pt, docs[opt]   
+00000cd0: 2009 5c0a 0909 7d20 2020 2009 0909 0909   .\...}    .....
+00000ce0: 5c0a 0920 2020 207d 270a 0a0a 2e50 484f  \..    }'....PHO
+00000cf0: 4e59 3a20 646f 6320 6c69 6e6b 6368 6563  NY: doc linkchec
+00000d00: 6b20 6865 6c70 0a                        k help.
```

### Comparing `factory_boy-3.2.1/PKG-INFO` & `factory_boy-3.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: factory_boy
-Version: 3.2.1
+Version: 3.3.0
 Summary: A versatile test fixtures replacement based on thoughtbot's factory_bot for Ruby.
 Home-page: https://github.com/FactoryBoy/factory_boy
 Author: Mark Sandstrom
 Author-email: mark@deliciouslynerdy.com
 Maintainer: Raphaël Barrois
 Maintainer-email: raphael.barrois+fboy@polytechnique.org
 License: MIT
 Keywords: factory_boy,factory,fixtures
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 factory_boy
 ===========
 
@@ -188,30 +188,30 @@
 
 More details can be found in the ORM section.
 
 
 Using factories
 """""""""""""""
 
-factory_boy supports several different build strategies: build, create, and stub:
+factory_boy supports several different instantiation strategies: build, create, and stub:
 
 .. code-block:: python
 
     # Returns a User instance that's not saved
     user = UserFactory.build()
 
     # Returns a saved User instance.
     # UserFactory must subclass an ORM base class, such as DjangoModelFactory.
     user = UserFactory.create()
 
     # Returns a stub object (just a bunch of attributes)
     obj = UserFactory.stub()
 
 
-You can use the Factory class as a shortcut for the default build strategy:
+You can use the Factory class as a shortcut for the default instantiation strategy:
 
 .. code-block:: python
 
     # Same as UserFactory.create()
     user = UserFactory()
 
 
@@ -357,15 +357,15 @@
 
 Support Policy
 --------------
 
 ``factory_boy`` supports active Python versions as well as PyPy3.
 
 - **Python**'s `supported versions
-  <https://devguide.python.org/#status-of-python-branches>`__.
+  <https://devguide.python.org/versions/#supported-versions>`__.
 - **Django**'s `supported
   versions <https://www.djangoproject.com/download/#supported-versions>`__.
 - **SQLAlchemy**: `latest version on PyPI <https://pypi.org/project/SQLAlchemy/>`__.
 - **MongoEngine**: `latest version on PyPI <https://pypi.org/project/mongoengine/>`__.
 
 Debugging factory_boy
 ---------------------
@@ -433,24 +433,60 @@
 To test with a specific framework version, you may use a ``tox`` target:
 
 .. code-block:: sh
 
     # list all tox environments
     $ tox --listenvs
 
-    # run tests inside a specific environment
-    $ tox -e py36-django20-alchemy13-mongoengine017
+    # run tests inside a specific environment (django/mongoengine/SQLAlchemy are not installed)
+    $ tox -e py310
 
-Valid options are:
+    # run tests inside a specific environment (django)
+    $ tox -e py310-djangomain
+    $ tox -e py310-djangomain-postgres
 
-* ``DJANGO`` for ``Django``
-* ``MONGOENGINE`` for ``mongoengine``
-* ``ALCHEMY`` for ``SQLAlchemy``
+    # run tests inside a specific environment (alchemy)
+    $ tox -e py310-alchemy
+    $ tox -e py310-alchemy-postgres
 
+    # run tests inside a specific environment (mongoengine)
+    $ tox -e py310-mongo
 
-To avoid running ``mongoengine`` tests (e.g no MongoDB server installed), run:
+
+Packaging
+---------
+
+For users interesting in packaging FactoryBoy into downstream distribution channels
+(e.g. ``.deb``, ``.rpm``, ``.ebuild``), the following tips might be helpful:
+
+Dependencies
+""""""""""""
+
+The package's run-time dependencies are listed in ``setup.cfg``.
+The dependencies useful for building and testing the library are covered by the
+``dev`` and ``doc`` extras.
+
+Moreover, all development / testing tasks are driven through ``make(1)``.
+
+Building
+""""""""
+
+In order to run the build steps (currently only for docs), run:
+
+.. code-block:: sh
+
+    python setup.py egg_info
+    make doc
+
+Testing
+"""""""
+
+When testing for the active Python environment, run the following:
 
 .. code-block:: sh
 
-    $ make SKIP_MONGOENGINE=1 test
+    make test
 
+.. note::
 
+    You must make sure that the ``factory`` module is importable, as it is imported from
+    the testing code.
```

### Comparing `factory_boy-3.2.1/README.rst` & `factory_boy-3.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -151,30 +151,30 @@
 
 More details can be found in the ORM section.
 
 
 Using factories
 """""""""""""""
 
-factory_boy supports several different build strategies: build, create, and stub:
+factory_boy supports several different instantiation strategies: build, create, and stub:
 
 .. code-block:: python
 
     # Returns a User instance that's not saved
     user = UserFactory.build()
 
     # Returns a saved User instance.
     # UserFactory must subclass an ORM base class, such as DjangoModelFactory.
     user = UserFactory.create()
 
     # Returns a stub object (just a bunch of attributes)
     obj = UserFactory.stub()
 
 
-You can use the Factory class as a shortcut for the default build strategy:
+You can use the Factory class as a shortcut for the default instantiation strategy:
 
 .. code-block:: python
 
     # Same as UserFactory.create()
     user = UserFactory()
 
 
@@ -320,15 +320,15 @@
 
 Support Policy
 --------------
 
 ``factory_boy`` supports active Python versions as well as PyPy3.
 
 - **Python**'s `supported versions
-  <https://devguide.python.org/#status-of-python-branches>`__.
+  <https://devguide.python.org/versions/#supported-versions>`__.
 - **Django**'s `supported
   versions <https://www.djangoproject.com/download/#supported-versions>`__.
 - **SQLAlchemy**: `latest version on PyPI <https://pypi.org/project/SQLAlchemy/>`__.
 - **MongoEngine**: `latest version on PyPI <https://pypi.org/project/mongoengine/>`__.
 
 Debugging factory_boy
 ---------------------
@@ -396,22 +396,60 @@
 To test with a specific framework version, you may use a ``tox`` target:
 
 .. code-block:: sh
 
     # list all tox environments
     $ tox --listenvs
 
-    # run tests inside a specific environment
-    $ tox -e py36-django20-alchemy13-mongoengine017
+    # run tests inside a specific environment (django/mongoengine/SQLAlchemy are not installed)
+    $ tox -e py310
 
-Valid options are:
+    # run tests inside a specific environment (django)
+    $ tox -e py310-djangomain
+    $ tox -e py310-djangomain-postgres
 
-* ``DJANGO`` for ``Django``
-* ``MONGOENGINE`` for ``mongoengine``
-* ``ALCHEMY`` for ``SQLAlchemy``
+    # run tests inside a specific environment (alchemy)
+    $ tox -e py310-alchemy
+    $ tox -e py310-alchemy-postgres
 
+    # run tests inside a specific environment (mongoengine)
+    $ tox -e py310-mongo
 
-To avoid running ``mongoengine`` tests (e.g no MongoDB server installed), run:
+
+Packaging
+---------
+
+For users interesting in packaging FactoryBoy into downstream distribution channels
+(e.g. ``.deb``, ``.rpm``, ``.ebuild``), the following tips might be helpful:
+
+Dependencies
+""""""""""""
+
+The package's run-time dependencies are listed in ``setup.cfg``.
+The dependencies useful for building and testing the library are covered by the
+``dev`` and ``doc`` extras.
+
+Moreover, all development / testing tasks are driven through ``make(1)``.
+
+Building
+""""""""
+
+In order to run the build steps (currently only for docs), run:
 
 .. code-block:: sh
 
-    $ make SKIP_MONGOENGINE=1 test
+    python setup.py egg_info
+    make doc
+
+Testing
+"""""""
+
+When testing for the active Python environment, run the following:
+
+.. code-block:: sh
+
+    make test
+
+.. note::
+
+    You must make sure that the ``factory`` module is importable, as it is imported from
+    the testing code.
```

### Comparing `factory_boy-3.2.1/docs/Makefile` & `factory_boy-3.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/docs/changelog.rst` & `factory_boy-3.3.0/docs/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,87 @@
 ChangeLog
 =========
 
 .. Note for v4.x: don't forget to check "Deprecated" sections for removal.
 
-3.2.1 (2021-10-26)
+3.3.0 (2023-07-19)
 ------------------
 
 *New:*
 
+    - :issue:`366`: Add :class:`factory.django.Password` to generate Django :class:`~django.contrib.auth.models.User`
+      passwords.
+    - :issue:`304`: Add :attr:`~factory.alchemy.SQLAlchemyOptions.sqlalchemy_session_factory` to dynamically
+      create sessions for use by the :class:`~factory.alchemy.SQLAlchemyModelFactory`.
+    - Add support for Django 4.0
+    - Add support for Django 4.1
+    - Add support for Python 3.10
+    - Add support for Python 3.11
+
+*Bugfix:*
+
+    - Make :meth:`~factory.django.mute_signals` mute signals during post-generation.
+
+    - :issue:`775`: Change the signature for :meth:`~factory.alchemy.SQLAlchemyModelFactory._save` and
+      :meth:`~factory.alchemy.SQLAlchemyModelFactory._get_or_create` to avoid argument names clashes with a field named
+      ``session``.
+
+*Deprecated:*
+
+    - :class:`~factory.django.DjangoModelFactory` will stop issuing a second call to
+      :meth:`~django.db.models.Model.save` on the created instance when :ref:`post-generation-hooks` return a value.
+
+      To help with the transition, :class:`factory.django.DjangoModelFactory._after_postgeneration` raises a
+      :class:`DeprecationWarning` when calling :meth:`~django.db.models.Model.save`. Inspect your
+      :class:`~factory.django.DjangoModelFactory` subclasses:
+
+      - If the :meth:`~django.db.models.Model.save` call is not needed after :class:`~factory.PostGeneration`, set
+        :attr:`factory.django.DjangoOptions.skip_postgeneration_save` to ``True`` in the factory meta.
+
+      - Otherwise, the instance has been modified by :class:`~factory.PostGeneration` hooks and needs to be
+        :meth:`~django.db.models.Model.save`\ d. Either:
+
+          - call :meth:`django.db.models.Model.save` in the :class:`~factory.PostGeneration` hook that modifies the
+            instance, or
+          - override :class:`~factory.django.DjangoModelFactory._after_postgeneration` to
+            :meth:`~django.db.models.Model.save` the instance.
+
+*Removed:*
+
+    - Drop support for Django 2.2
+    - Drop support for Django 3.0
+    - Drop support for Django 3.1
+    - Drop support for Python 3.6
+
+3.2.1 (2021-10-26)
+------------------
+
+*New:*
     - Add support for Django 3.2
 
 *Bugfix:*
 
     - Do not override signals receivers registered in a :meth:`~factory.django.mute_signals` context.
 
     - :issue:`775`: Change the signature for :meth:`~factory.alchemy.SQLAlchemyModelFactory._save` and
       :meth:`~factory.alchemy.SQLAlchemyModelFactory._get_or_create` to avoid argument names clashes with a field named
       ``session``.
 
-
 3.2.0 (2020-12-28)
 ------------------
 
 *New:*
 
     - Add support for Django 3.1
     - Add support for Python 3.9
 
 *Removed:*
 
     - Drop support for Django 1.11. This version `is not maintained anymore <https://www.djangoproject.com/download/#supported-versions>`__.
-    - Drop support for Python 3.5. This version `is not maintained anymore <https://devguide.python.org/devcycle/#end-of-life-branches>`__.
+    - Drop support for Python 3.5. This version `is not maintained anymore <https://devguide.python.org/developer-workflow/development-cycle/index.html#end-of-life-branches>`__.
 
 *Deprecated:*
 
     - :func:`factory.use_strategy`. Use :attr:`factory.FactoryOptions.strategy` instead.
       The purpose of :func:`~factory.use_strategy` duplicates the factory option. Follow :pep:`20`: *There should be
       one-- and preferably only one --obvious way to do it.*
 
@@ -83,15 +130,15 @@
 | ``from factory.fuzzy import set_random_state`` | ``from factory.random import set_random_state``   |
 +------------------------------------------------+---------------------------------------------------+
 | ``from factory.fuzzy import reseed_random``    | ``from factory.random import reseed_random``      |
 +------------------------------------------------+---------------------------------------------------+
 
 *Removed:*
 
-    - Drop support for Python 2 and 3.4. These versions `are not maintained anymore <https://devguide.python.org/devcycle/#end-of-life-branches>`__.
+    - Drop support for Python 2 and 3.4. These versions `are not maintained anymore <https://devguide.python.org/developer-workflow/development-cycle/index.html#end-of-life-branches>`__.
     - Drop support for Django 2.0 and 2.1. These versions `are not maintained anymore <https://www.djangoproject.com/download/#supported-versions>`__.
     - Remove deprecated ``force_flush`` from ``SQLAlchemyModelFactory`` options. Use
       ``sqlalchemy_session_persistence = "flush"`` instead.
     - Drop deprecated ``attributes()`` from :class:`~factory.Factory` subclasses; use
       ``factory.make_factory(dict, FactoryClass._meta.pre_declarations)`` instead.
     - Drop deprecated ``declarations()`` from :class:`~factory.Factory` subclasses; use ``FactoryClass._meta.pre_declarations`` instead.
     - Drop ``factory.compat`` module.
@@ -415,15 +462,15 @@
 .. _v2.3.1:
 
 2.3.1 (2014-01-22)
 ------------------
 
 *Bug fix:*
 
-    - Fix badly written assert containing state-changing code, spotted by `chsigi <https://github.com/chsigi>`_ (:pr:`126`)
+    - Fix badly written assert containing state-changing code, spotted by ``chsigi`` (:pr:`126`)
     - Don't crash when handling objects whose ``__repr__`` is non-pure-ASCII bytes on Python 2,
       discovered by `mbertheau <https://github.com/mbertheau>`_ (:issue:`123`) and `strycore <https://github.com/strycore>`_ (:pr:`127`)
 
 .. _v2.3.0:
 
 2.3.0 (2013-12-25)
 ------------------
```

### Comparing `factory_boy-3.2.1/docs/conf.py` & `factory_boy-3.3.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Path setup --------------------------------------------------------------
 
 import os
 import sys
 
-import factory
-
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.dirname(os.path.abspath('.')))
 
+# Must be imported after the parent directory was added to sys.path for global sphinx installation.
+import factory  # noqa
 
 # -- Project information -----------------------------------------------------
 
 project = 'Factory Boy'
 copyright = '2011-2015, Raphaël Barrois, Mark Sandstrom'
 author = 'adfasf'
 
@@ -37,16 +37,16 @@
     'sphinx.ext.autodoc',
     'sphinx.ext.extlinks',
     'sphinx.ext.intersphinx',
     'sphinx.ext.viewcode',
 ]
 
 extlinks = {
-    'issue': ('https://github.com/FactoryBoy/factory_boy/issues/%s', 'issue #'),
-    'pr': ('https://github.com/FactoryBoy/factory_boy/pull/%s', 'pull request #'),
+    'issue': ('https://github.com/FactoryBoy/factory_boy/issues/%s', 'issue %s'),
+    'pr': ('https://github.com/FactoryBoy/factory_boy/pull/%s', 'pull request %s'),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The master toctree document.
 master_doc = 'index'
@@ -69,17 +69,21 @@
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 
+# -- linkcheck ---------------------------------------------------------------
+linkcheck_retries = 3
+
+
 # -- intersphinx -------------------------------------------------------------
 intersphinx_mapping = {
-    'https://docs.python.org/': None,
+    'python': ('https://docs.python.org/3', None),
     'django': (
         'https://docs.djangoproject.com/en/dev/',
         'https://docs.djangoproject.com/en/dev/_objects/',
     ),
     'sqlalchemy': (
         'https://docs.sqlalchemy.org/en/latest/',
         'https://docs.sqlalchemy.org/en/latest/objects.inv',
```

### Comparing `factory_boy-3.2.1/docs/credits.rst` & `factory_boy-3.3.0/docs/credits.rst`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 * Hugo Osvaldo Barrera <hugo@barrera.io>
 * Ilya Baryshev <baryshev@gmail.com>
 * Ilya Pirogov <ilja.pirogov@gmail.com>
 * Ionuț Arțăriși <ionut@artarisi.eu>
 * Issa Jubril <issa.jubril@andela.com>
 * Ivan Miric <imiric@gmail.com>
 * Janusz Skonieczny <wooyek@users.noreply.github.com>
+* Javier Buzzi <kingbuzzman@users.noreply.github.com> (https://github.com/kingbuzzman)
 * Jeff Widman <jeff@jeffwidman.com> (https://github.com/jeffwidman)
 * Jon Dufresne <jon.dufresne@gmail.com>
 * Jonathan Tushman <jtushman@pipewave.com>
 * Joshua Carp <jm.carp@gmail.com>
 * Leonardo Lazzaro <llazzaro@dc.uba.ar>
 * Luke GB <github@lukegb.com>
 * Marc Abramowitz <marc@marc-abramowitz.com>
@@ -67,14 +68,15 @@
 * QuantumGhost <obelisk.reg+github@gmail.com>
 * Raphaël Barrois <raphael.barrois+fboy@polytechnique.org> (https://github.com/rbarrois)
 * Rich Rauenzahn <rich@vmware.com>
 * Richard Moch <richard@mbp.polyconseil.fr>
 * Rob Zyskowski <zyskowski.rob@gmail.com>
 * Robrecht De Rouck <Robrecht.De.Rouck@gmail.com>
 * Samuel Paccoud <samuel@sampaccoud.com>
+* Sarah Boyce <sarahvboyce95@gmail.com>
 * Saul Shanabrook <s.shanabrook@gmail.com>
 * Sean Löfgren <SeanBE@users.noreply.github.com>
 * Shahriar Tajbakhsh <shahriar@metaview.ai>
 * Tom <tom@tomleo.com>
 * alex-netquity <alex@netquity.com>
 * anentropic <ego@anentropic.com>
 * minimumserious <commande.romain@gmail.com>
```

### Comparing `factory_boy-3.2.1/docs/examples.rst` & `factory_boy-3.3.0/docs/examples.rst`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 And now, we'll define the related factories:
 
 
 .. code-block:: python
 
     import datetime
     import factory
-    import random
 
     from . import objects
 
 
     class AccountFactory(factory.Factory):
         class Meta:
             model = objects.Account
```

### Comparing `factory_boy-3.2.1/docs/fuzzy.rst` & `factory_boy-3.3.0/docs/fuzzy.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 ================
 
 .. module:: factory.fuzzy
 
 .. note:: Now that FactoryBoy includes the :class:`factory.Faker` class, most of
           these built-in fuzzers are deprecated in favor of their
           `Faker <https://faker.readthedocs.io/>`_ equivalents. Further
-          discussion here:
-          `<https://github.com/FactoryBoy/factory_boy/issues/271/>`_
+          discussion in :issue:`271`.
 
 Some tests may be interested in testing with fuzzy, random values.
 
 This is handled by the :mod:`factory.fuzzy` module, which provides a few
 random declarations.
 
 .. note:: Use ``import factory.fuzzy`` to load this module.
@@ -72,23 +71,14 @@
 
     .. note:: The passed in :attr:`choices` will be converted into a list upon
               first use, not at declaration time.
 
               This allows passing in, for instance, a Django queryset that will
               only hit the database during the database, not at import time.
 
-    .. warning:: When using Python2 and list comprehension, use private variable
-                 names as in:
-
-                 `[_x.name for _x in items]`
-
-                 instead of:
-
-                 `[x.name for x in items]`
-
     .. attribute:: choices
 
         The list of choices to select randomly
 
 
 FuzzyInteger
 ------------
```

### Comparing `factory_boy-3.2.1/docs/internals.rst` & `factory_boy-3.3.0/docs/internals.rst`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
   :meth:`~Factory.create_batch`, ...), use it
 - If it is generic (:meth:`~Factory.generate`, :meth:`Factory.__call__`),
   use the strategy defined at the :attr:`class Meta <Factory.Meta>` level
 
 
 Then, we'll pass the strategy and passed-in overrides to the :meth:`~Factory._generate` method.
 
-.. note:: According to the project road map, a future version will use a :meth:`~Factory._generate_batch`` at its core instead.
+.. note:: According to the project road map, a future version will use a :meth:`~Factory._generate_batch` at its core instead.
 
 A factory's :meth:`~Factory._generate` function actually delegates to a ``StepBuilder()`` object.
 This object will carry the overall "build an object" context (strategy, depth, and possibly other).
 
 
 Instantiating, Step 2: Preparing values
 ---------------------------------------
```

### Comparing `factory_boy-3.2.1/docs/introduction.rst` & `factory_boy-3.3.0/docs/introduction.rst`

 * *Files 3% similar despite different names*

```diff
@@ -95,31 +95,40 @@
         class Meta:
             model = models.User
 
         username = factory.Sequence(lambda n: 'user%d' % n)
 
 .. code-block:: pycon
 
+    >>> # The sequence counter starts at 0 by default
     >>> UserFactory()
     <User: user0>
     >>> UserFactory()
     <User: user1>
 
+    >>> # A value can be provided for a sequence-driven field
+    >>> # but this still increments the sequence counter
+    >>> UserFactory(username="ada.lovelace")
+    <User: ada.lovelace>
+    >>> UserFactory()
+    <User: user3>
+
 .. note:: For more complex situations, you may also use the :meth:`~factory.@sequence` decorator (note that ``self`` is not added as first parameter):
 
           .. code-block:: python
 
             class UserFactory(factory.Factory):
                 class Meta:
                     model = models.User
 
                 @factory.sequence
                 def username(n):
                     return 'user%d' % n
 
+    To set or reset the sequence counter see :ref:`Forcing a sequence counter <forcing-a-sequence-counter>`.
 
 LazyFunction
 ------------
 
 In simple cases, calling a function is enough to compute the value. If that function doesn't depend on the object
 being built, use :class:`~factory.LazyFunction` to call that function; it should receive a function taking no
 argument and returning the value for the field:
@@ -161,23 +170,23 @@
 
         username = factory.Sequence(lambda n: 'user%d' % n)
         email = factory.LazyAttribute(lambda obj: '%s@example.com' % obj.username)
 
 .. code-block:: pycon
 
     >>> UserFactory()
-    <User: user1 (user1@example.com)>
+    <User: user0 (user0@example.com)>
 
     >>> # The LazyAttribute handles overridden fields
     >>> UserFactory(username='john')
     <User: john (john@example.com)>
 
     >>> # They can be directly overridden as well
     >>> UserFactory(email='doe@example.com')
-    <User: user3 (doe@example.com)>
+    <User: user2 (doe@example.com)>
 
 
 .. note:: As for :class:`~factory.Sequence`, a :meth:`~factory.@lazy_attribute` decorator is available:
 
 
 .. code-block:: python
```

### Comparing `factory_boy-3.2.1/docs/logo.png` & `factory_boy-3.3.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/docs/logo.svg` & `factory_boy-3.3.0/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/docs/make.bat` & `factory_boy-3.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/docs/orms.rst` & `factory_boy-3.3.0/docs/orms.rst`

 * *Files 3% similar despite different names*

```diff
@@ -105,18 +105,55 @@
                 >>>     email="a_new_email@example.com"
                 >>> )
                 <User: john>
 
                 >>> john.email                            # The email value was not updated
                 "john@example.com"
 
+    .. attribute:: skip_postgeneration_save
+
+        Transitional option to prevent
+        :meth:`~factory.django.DjangoModelFactory._after_postgeneration` from
+        issuing a duplicate call to :meth:`~django.db.models.Model.save` on the
+        created instance when :class:`factory.PostGeneration` hooks return a
+        value.
+
 
 Extra fields
 """"""""""""
 
+.. class:: Password
+
+    Applies :func:`~django.contrib.auth.hashers.make_password` to the
+    clear-text argument before to generate the object.
+
+    .. method:: __init__(self, password)
+
+        :param str password: Default password.
+
+    .. code-block:: python
+
+        class UserFactory(factory.django.DjangoModelFactory):
+            class Meta:
+                model = models.User
+
+            password = factory.django.Password('pw')
+
+    .. code-block:: pycon
+
+        >>> from django.contrib.auth.hashers import check_password
+        >>> # Create user with the default password from the factory.
+        >>> user = UserFactory.create()
+        >>> check_password('pw', user.password)
+        True
+        >>> # Override user password at call time.
+        >>> other_user = UserFactory.create(password='other_pw')
+        >>> check_password('other_pw', other_user.password)
+        True
+
 
 .. class:: FileField
 
     Custom declarations for :class:`django.db.models.FileField`
 
     .. method:: __init__(self, from_path='', from_file='', from_func='', data=b'', filename='example.dat')
 
@@ -328,14 +365,33 @@
     a :class:`SQLAlchemyModelFactory` also supports the following settings:
 
     .. attribute:: sqlalchemy_session
 
         SQLAlchemy session to use to communicate with the database when creating
         an object through this :class:`SQLAlchemyModelFactory`.
 
+    .. attribute:: sqlalchemy_session_factory
+
+       .. versionadded:: 3.3.0
+
+         :class:`~collections.abc.Callable` returning a :class:`~sqlalchemy.orm.Session` instance to use to communicate
+         with the database. You can either provide the session through this attribute, or through
+         :attr:`~factory.alchemy.SQLAlchemyOptions.sqlalchemy_session`, but not both at the same time.
+
+        .. code-block:: python
+
+            from . import common
+
+            class UserFactory(factory.alchemy.SQLAlchemyModelFactory):
+                class Meta:
+                    model = User
+                    sqlalchemy_session_factory = lambda: common.Session()
+
+                username = 'john'
+
     .. attribute:: sqlalchemy_session_persistence
 
         Control the action taken by ``sqlalchemy_session`` at the end of a create call.
 
         Valid values are:
 
         * ``None``: do nothing
@@ -403,16 +459,15 @@
 
 
 A (very) simple example:
 
 .. code-block:: python
 
     from sqlalchemy import Column, Integer, Unicode, create_engine
-    from sqlalchemy.ext.declarative import declarative_base
-    from sqlalchemy.orm import scoped_session, sessionmaker
+    from sqlalchemy.orm import declarative_base, scoped_session, sessionmaker
 
     engine = create_engine('sqlite://')
     session = scoped_session(sessionmaker(bind=engine))
     Base = declarative_base()
 
 
     class User(Base):
@@ -435,17 +490,17 @@
         name = factory.Sequence(lambda n: 'User %d' % n)
 
 .. code-block:: pycon
 
     >>> session.query(User).all()
     []
     >>> UserFactory()
-    <User: User 1>
+    <User: User 0>
     >>> session.query(User).all()
-    [<User: User 1>]
+    [<User: User 0>]
 
 
 Managing sessions
 """""""""""""""""
 
 Since `SQLAlchemy`_ is a general purpose library,
 there is no "global" session management system.
@@ -473,15 +528,15 @@
 
 Here is an example layout:
 
 - A global (test-only?) file holds the :class:`~sqlalchemy.orm.scoping.scoped_session`:
 
 .. code-block:: python
 
-    # myprojet/test/common.py
+    # myproject/test/common.py
 
     from sqlalchemy import orm
     Session = orm.scoped_session(orm.sessionmaker())
 
 
 - All factory access it:
```

### Comparing `factory_boy-3.2.1/docs/recipes.rst` & `factory_boy-3.3.0/docs/recipes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,18 @@
 
     class UserFactory(factory.django.DjangoModelFactory):
         class Meta:
             model = models.User
 
         language = factory.Iterator(models.Language.objects.all())
 
-Here, ``models.Language.objects.all()`` won't be evaluated until the
-first call to ``UserFactory``; thus avoiding DB queries at import time.
+Here, ``models.Language.objects.all()`` is a
+:class:`~django.db.models.query.QuerySet` and will only hit the database when
+``factory_boy`` starts iterating on it, i.e on the first call to
+``UserFactory``; thus avoiding DB queries at import time.
 
 
 Reverse dependencies (reverse ForeignKey)
 -----------------------------------------
 
 When a related object should be created upon object creation
 (e.g a reverse :class:`~django.db.models.ForeignKey` from another :class:`~django.db.models.Model`),
@@ -102,14 +104,16 @@
 Prior to version 2.9, the solution to this was to override the :meth:`~factory.Factory._generate` method on the factory.
 
 Since version 2.9, the :meth:`~factory.django.mute_signals` decorator should be used:
 
 
 .. code-block:: python
 
+    from django.db.models.signals import post_save
+    
     @factory.django.mute_signals(post_save)
     class ProfileFactory(factory.django.DjangoModelFactory):
         class Meta:
             model = my_models.Profile
 
         title = 'Dr'
         # We pass in profile=None to prevent UserFactory from creating another profile
@@ -137,14 +141,18 @@
     "Lord"
 
 Such behavior can be extended to other situations where a signal interferes with
 factory_boy related factories.
 
 Any factories that call these classes with :class:`~factory.SubFactory` will also need to be decorated in the same manner.
 
+..
+   _DEPRECATED: Release 4.0: post_generation and RelatedFactory will stop
+                issuing calls to save(). Refs issues 316 and 366.
+
 .. note:: When any :class:`~factory.RelatedFactory` or :class:`~factory.post_generation`
           attribute is defined on the :class:`~factory.django.DjangoModelFactory` subclass,
           a second ``save()`` is performed *after* the call to ``_create()``.
 
           Code working with signals should thus use the :meth:`~factory.django.mute_signals` decorator
 
 
@@ -181,22 +189,20 @@
         class Meta:
             model = models.User
 
         name = "John Doe"
 
         @factory.post_generation
         def groups(self, create, extracted, **kwargs):
-            if not create:
-                # Simple build, do nothing.
+            if not create or not extracted:
+                # Simple build, or nothing to add, do nothing.
                 return
 
-            if extracted:
-                # A list of groups were passed in, use them
-                for group in extracted:
-                    self.groups.add(group)
+            # Add the iterable of groups using bulk addition
+            self.groups.add(*extracted)
 
 .. OHAI_VIM**
 
 When calling ``UserFactory()`` or ``UserFactory.build()``, no group binding
 will be created.
 
 But when ``UserFactory.create(groups=(group1, group2, group3))`` is called,
@@ -541,21 +547,21 @@
 
 .. code-block:: python
 
     class UserFactory(factory.django.DjangoModelFactory):
         class Meta:
             model = models.User
 
-        first_name = factory.Sequence(lambda n: "Agent %03d" % n)
+        first_name = factory.Sequence(lambda n: "Agent %03d" % n)  # Agent 000, Agent 001, Agent 002
         username = factory.Faker('user_name')
 
 .. code-block:: pycon
 
     >>> factory.build(dict, FACTORY_CLASS=UserFactory)
-    {'first_name': "Agent 001", 'username': 'john_doe'}
+    {'first_name': "Agent 000", 'username': 'john_doe'}
 
 
 Fuzzying Django model field choices
 -----------------------------------
 
 When defining a :class:`~factory.fuzzy.FuzzyChoice` you can reuse the same choice list from the model field descriptor.
```

### Comparing `factory_boy-3.2.1/docs/reference.rst` & `factory_boy-3.3.0/docs/reference.rst`

 * *Files 1% similar despite different names*

```diff
@@ -699,30 +699,30 @@
         >>> user.name
         'Lucy Cechtelar'
 
     Some providers accept parameters; they should be passed after the provider name:
 
     .. code-block:: python
 
-        class UserFactory(fatory.Factory):
+        class UserFactory(factory.Factory):
             class Meta:
                 model = User
 
             arrival = factory.Faker(
                 'date_between_dates',
                 date_start=datetime.date(2020, 1, 1),
                 date_end=datetime.date(2020, 5, 31),
             )
 
     As with :class:`~factory.SubFactory`, the parameters can be any valid declaration.
     This does not apply to the provider name or the locale.
 
     .. code-block:: python
 
-        class TripFactory(fatory.Factory):
+        class TripFactory(factory.Factory):
             class Meta:
                 model = Trip
 
             departure = factory.Faker(
                 'date',
                 end_datetime=datetime.date.today(),
             )
@@ -900,14 +900,53 @@
 .. code-block:: pycon
 
     >>> joel = UserFactory(name="Joël")
     >>> joel.email
     'joel@example.com'
 
 
+Transformer
+"""""""""""
+
+.. class:: Transformer(default_value, *, transform)
+
+A :class:`Transformer` applies a ``transform`` function to the provided value
+before to set the transformed value on the generated object.
+
+It expects one positional argument and one keyword argument:
+
+- ``default_value``: the default value, which passes through the ``transform``
+  function.
+- ``transform``: a function taking the value as parameter and returning the
+  transformed value,
+
+.. code-block:: python
+
+   class UpperFactory(factory.Factory):
+       name = factory.Transformer("Joe", transform=str.upper)
+
+       class Meta:
+           model = Upper
+
+.. code-block:: pycon
+
+   >>> UpperFactory().name
+   'JOE'
+   >>> UpperFactory(name="John").name
+   'JOHN'
+
+Disabling
+~~~~~~~~~
+To disable a :class:`Transformer`, wrap the value in ``Transformer.Force``:
+
+.. code-block:: pycon
+
+   >>> UpperFactory(name=factory.Transformer.Force("John")).name
+   'John'
+
 Sequence
 """"""""
 
 .. class:: Sequence(lambda)
 
 If a field should be unique, and thus different for all built instances,
 use a :class:`Sequence`.
@@ -922,18 +961,20 @@
             model = User
 
         phone = factory.Sequence(lambda n: '123-555-%04d' % n)
 
 .. code-block:: pycon
 
     >>> UserFactory().phone
-    '123-555-0001'
+    '123-555-0000'
     >>> UserFactory().phone
-    '123-555-0002'
+    '123-555-0001'
 
+.. note:: The sequence counter starts at 0 and can be set or reset,
+          see :ref:`Forcing a sequence counter <forcing-a-sequence-counter>`.
 
 Decorator
 ~~~~~~~~~
 
 .. function:: sequence
 
 As with :meth:`lazy_attribute`, a decorator is available for complex situations.
@@ -951,17 +992,17 @@
         def phone(n):
             a = n // 10000
             b = n % 10000
             return '%03d-555-%04d' % (a, b)
 
 .. code-block:: pycon
 
-    >>> UserFactory().phone
+    >>> UserFactory().phone  # current sequence counter at 9999
     '000-555-9999'
-    >>> UserFactory().phone
+    >>> UserFactory().phone  # current sequence counter at 10000
     '001-555-0000'
 
 
 Sharing
 ~~~~~~~
 
 The sequence counter is shared across all :class:`Sequence` attributes of the
@@ -976,18 +1017,18 @@
         phone = factory.Sequence(lambda n: '%04d' % n)
         office = factory.Sequence(lambda n: 'A23-B%03d' % n)
 
 .. code-block:: pycon
 
     >>> u = UserFactory()
     >>> u.phone, u.office
-    '0041', 'A23-B041'
+    '0040', 'A23-B040'
     >>> u2 = UserFactory()
     >>> u2.phone, u2.office
-    '0042', 'A23-B042'
+    '0041', 'A23-B041'
 
 
 Inheritance
 ~~~~~~~~~~~
 
 When a :class:`Factory` inherits from another :class:`Factory` and the `model`
 of the subclass inherits from the `model` of the parent, the sequence counter
@@ -1005,24 +1046,25 @@
     class EmployeeFactory(UserFactory):
         office_phone = factory.Sequence(lambda n: '%04d' % n)
 
 .. code-block:: pycon
 
     >>> u = UserFactory()
     >>> u.phone
-    '123-555-0001'
+    '123-555-0000'
 
     >>> e = EmployeeFactory()
     >>> e.phone, e.office_phone
-    '123-555-0002', '0002'
+    '123-555-0001', '0001'
 
     >>> u2 = UserFactory()
     >>> u2.phone
-    '123-555-0003'
+    '123-555-0002'
 
+.. _forcing-a-sequence-counter:
 
 Forcing a sequence counter
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 If a specific value of the sequence counter is required for one instance, the
 ``__sequence`` keyword argument should be passed to the factory method.
 
@@ -1073,17 +1115,17 @@
 
         login = 'john'
         email = factory.LazyAttributeSequence(lambda o, n: '%s@s%d.example.com' % (o.login, n))
 
 .. code-block:: pycon
 
     >>> UserFactory().email
-    'john@s1.example.com'
+    'john@s0.example.com'
     >>> UserFactory(login='jack').email
-    'jack@s2.example.com'
+    'jack@s1.example.com'
 
 
 Decorator
 ~~~~~~~~~
 
 .. function:: lazy_attribute_sequence(method_to_call)
 
@@ -1271,15 +1313,15 @@
 
 .. code-block:: python
 
     class UserFactory(factory.Factory):
         class Meta:
             model = User
 
-        birthdate = factory.Sequence(lambda n: datetime.date(2000, 1, 1) + datetime.timedelta(days=n))
+        birthdate = factory.fuzzy.FuzzyDate()
         birthmonth = factory.SelfAttribute('birthdate.month')
 
 .. code-block:: pycon
 
     >>> u = UserFactory()
     >>> u.birthdate
     date(2000, 3, 15)
@@ -1588,14 +1630,15 @@
     >>> u.deactivation_date
     datetime.datetime(2017, 4, 1, 23, 21, 23, tzinfo=UTC)
 
 .. note:: If the condition for the decider is complex, use a :class:`LazyAttribute`
           defined in the :attr:`~Factory.Params` section of your factory to
           handle the computation.
 
+.. _post-generation-hooks:
 
 Post-generation hooks
 """""""""""""""""""""
 
 Some objects expect additional method calls or complex processing for proper definition.
 For instance, a ``User`` may need to have a related ``Profile``, where the ``Profile`` is built from the ``User`` object.
 
@@ -1853,15 +1896,14 @@
 
         @factory.post_generation
         def mbox(obj, create, extracted, **kwargs):
             if not create:
                 return
             path = extracted or os.path.join('/tmp/mbox/', obj.login)
             os.path.makedirs(path)
-            return path
 
 .. OHAI_VIM**
 
 .. code-block:: pycon
 
     >>> UserFactory.build()                  # Nothing was created
     >>> UserFactory.create()                 # Creates dir /tmp/mbox/john
@@ -1908,15 +1950,15 @@
     class User(models.Model):
         name = models.CharField(max_length=191)
 
         def register(self, system, auth_token="ABC"):
             self.registration_id = system.register(auth_token)
 
 
-    class UserFactory(factory.DjangoModelFactory):
+    class UserFactory(factory.django.DjangoModelFactory):
         class Meta:
             model = User
 
         name = 'user'
         register = factory.PostGenerationMethodCall("register", DefaultRegistry())
 
 If the :class:`PostGenerationMethodCall` declaration contained no
```

### Comparing `factory_boy-3.2.1/examples/django_demo/django_demo/settings.py` & `factory_boy-3.3.0/examples/django_demo/django_demo/settings.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/examples/django_demo/django_demo/urls.py` & `factory_boy-3.3.0/examples/django_demo/django_demo/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 Class-based views
     1. Add an import:  from other_app.views import Home
     2. Add a URL to urlpatterns:  url(r'^$', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.conf.urls import url, include
     2. Add a URL to urlpatterns:  url(r'^blog/', include('blog.urls'))
 """
-from django.conf.urls import url
 from django.contrib import admin
+from django.urls import path
 
 urlpatterns = [
-    url(r'^admin/', admin.site.urls),
+    path('admin/', admin.site.urls),
 ]
```

### Comparing `factory_boy-3.2.1/examples/django_demo/generic_foreignkey/factories.py` & `factory_boy-3.3.0/examples/django_demo/generic_foreignkey/factories.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/examples/django_demo/generic_foreignkey/migrations/0001_initial.py` & `factory_boy-3.3.0/examples/django_demo/generic_foreignkey/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/examples/django_demo/generic_foreignkey/models.py` & `factory_boy-3.3.0/examples/django_demo/generic_foreignkey/models.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/examples/django_demo/generic_foreignkey/tests.py` & `factory_boy-3.3.0/examples/django_demo/generic_foreignkey/tests.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/examples/flask_alchemy/demoapp.py` & `factory_boy-3.3.0/examples/flask_alchemy/demoapp.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/examples/flask_alchemy/demoapp_factories.py` & `factory_boy-3.3.0/examples/flask_alchemy/demoapp_factories.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/examples/flask_alchemy/test_demoapp.py` & `factory_boy-3.3.0/examples/flask_alchemy/test_demoapp.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,25 @@
 
 
 class DemoAppTestCase(unittest.TestCase):
 
     def setUp(self):
         demoapp.app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite://'
         demoapp.app.config['TESTING'] = True
+
+        self.app_context = demoapp.app.app_context()
+        self.app_context.push()
+
         self.app = demoapp.app.test_client()
         self.db = demoapp.db
         self.db.create_all()
 
     def tearDown(self):
         self.db.drop_all()
+        self.app_context.pop()
 
     def test_user_factory(self):
         user = demoapp_factories.UserFactory()
         self.db.session.commit()
         self.assertIsNotNone(user.id)
         self.assertEqual(1, len(demoapp.User.query.all()))
```

### Comparing `factory_boy-3.2.1/factory/__init__.py` & `factory_boy-3.3.0/factory/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     PostGenerationMethodCall,
     RelatedFactory,
     RelatedFactoryList,
     SelfAttribute,
     Sequence,
     SubFactory,
     Trait,
+    Transformer,
 )
 from .enums import BUILD_STRATEGY, CREATE_STRATEGY, STUB_STRATEGY
 from .errors import FactoryError
 from .faker import Faker
 from .helpers import (
     build,
     build_batch,
@@ -67,14 +68,12 @@
     from . import mongoengine
 except ImportError:
     pass
 
 __author__ = 'Raphaël Barrois <raphael.barrois+fboy@polytechnique.org>'
 try:
     # Python 3.8+
-    from importlib.metadata import version
-
-    __version__ = version("factory_boy")
+    import importlib.metadata as importlib_metadata
 except ImportError:
-    import pkg_resources
+    import importlib_metadata
 
-    __version__ = pkg_resources.get_distribution("factory_boy").version
+__version__ = importlib_metadata.version("factory_boy")
```

### Comparing `factory_boy-3.2.1/factory/alchemy.py` & `factory_boy-3.3.0/factory/alchemy.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,31 +18,40 @@
     def _check_sqlalchemy_session_persistence(self, meta, value):
         if value not in VALID_SESSION_PERSISTENCE_TYPES:
             raise TypeError(
                 "%s.sqlalchemy_session_persistence must be one of %s, got %r" %
                 (meta, VALID_SESSION_PERSISTENCE_TYPES, value)
             )
 
+    @staticmethod
+    def _check_has_sqlalchemy_session_set(meta, value):
+        if value and meta.sqlalchemy_session:
+            raise RuntimeError("Provide either a sqlalchemy_session or a sqlalchemy_session_factory, not both")
+
     def _build_default_options(self):
         return super()._build_default_options() + [
             base.OptionDefault('sqlalchemy_get_or_create', (), inherit=True),
             base.OptionDefault('sqlalchemy_session', None, inherit=True),
             base.OptionDefault(
+                'sqlalchemy_session_factory', None, inherit=True, checker=self._check_has_sqlalchemy_session_set
+            ),
+            base.OptionDefault(
                 'sqlalchemy_session_persistence',
                 None,
                 inherit=True,
                 checker=self._check_sqlalchemy_session_persistence,
             ),
         ]
 
 
 class SQLAlchemyModelFactory(base.Factory):
     """Factory for SQLAlchemy models. """
 
     _options_class = SQLAlchemyOptions
+    _original_params = None
 
     class Meta:
         abstract = True
 
     @classmethod
     def _generate(cls, strategy, params):
         # Original params are used in _get_or_create if it cannot build an
@@ -65,14 +74,18 @@
             *args, **key_fields).one_or_none()
 
         if not obj:
             try:
                 obj = cls._save(model_class, session, args, {**key_fields, **kwargs})
             except IntegrityError as e:
                 session.rollback()
+
+                if cls._original_params is None:
+                    raise e
+
                 get_or_create_params = {
                     lookup: value
                     for lookup, value in cls._original_params.items()
                     if lookup in cls._meta.sqlalchemy_get_or_create
                 }
                 if get_or_create_params:
                     try:
@@ -86,14 +99,18 @@
                     raise e
 
         return obj
 
     @classmethod
     def _create(cls, model_class, *args, **kwargs):
         """Create an instance of the model, and save it to the database."""
+        session_factory = cls._meta.sqlalchemy_session_factory
+        if session_factory:
+            cls._meta.sqlalchemy_session = session_factory()
+
         session = cls._meta.sqlalchemy_session
 
         if session is None:
             raise RuntimeError("No session provided.")
         if cls._meta.sqlalchemy_get_or_create:
             return cls._get_or_create(model_class, session, args, kwargs)
         return cls._save(model_class, session, args, kwargs)
```

### Comparing `factory_boy-3.2.1/factory/base.py` & `factory_boy-3.3.0/factory/base.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/factory/builder.py` & `factory_boy-3.3.0/factory/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,14 +130,22 @@
         """Return a dict() suitable for our __init__."""
         return dict(self._items())
 
     def __repr__(self):
         return '<DeclarationSet: %r>' % self.as_dict()
 
 
+def _captures_overrides(declaration_with_context):
+    declaration = declaration_with_context.declaration
+    if enums.get_builder_phase(declaration) == enums.BuilderPhase.ATTRIBUTE_RESOLUTION:
+        return declaration.CAPTURE_OVERRIDES
+    else:
+        return False
+
+
 def parse_declarations(decls, base_pre=None, base_post=None):
     pre_declarations = base_pre.copy() if base_pre else DeclarationSet()
     post_declarations = base_post.copy() if base_post else DeclarationSet()
 
     # Inject extra declarations, splitting between known-to-be-post and undetermined
     extra_post = {}
     extra_maybenonpost = {}
@@ -159,27 +167,31 @@
         else:
             extra_maybenonpost[k] = v
 
     # Start with adding new post-declarations
     post_declarations.update(extra_post)
 
     # Fill in extra post-declaration context
+    extra_pre_declarations = {}
+    extra_post_declarations = {}
     post_overrides = post_declarations.filter(extra_maybenonpost)
-    post_declarations.update({
-        k: v
-        for k, v in extra_maybenonpost.items()
-        if k in post_overrides
-    })
-
-    # Anything else is pre_declarations
-    pre_declarations.update({
-        k: v
-        for k, v in extra_maybenonpost.items()
-        if k not in post_overrides
-    })
+    for k, v in extra_maybenonpost.items():
+        if k in post_overrides:
+            extra_post_declarations[k] = v
+        elif k in pre_declarations and _captures_overrides(pre_declarations[k]):
+            # Send the overriding value to the existing declaration.
+            # By symmetry with the behaviour of PostGenerationDeclaration,
+            # we send it as `key__` -- i.e under the '' key.
+            magic_key = pre_declarations.join(k, '')
+            extra_pre_declarations[magic_key] = v
+        else:
+            # Anything else is pre_declarations
+            extra_pre_declarations[k] = v
+    pre_declarations.update(extra_pre_declarations)
+    post_declarations.update(extra_post_declarations)
 
     return pre_declarations, post_declarations
 
 
 class BuildStep:
     def __init__(self, builder, sequence, parent_step=None):
         self.builder = builder
```

### Comparing `factory_boy-3.2.1/factory/declarations.py` & `factory_boy-3.3.0/factory/declarations.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,19 @@
     Declarations mark an attribute as needing lazy evaluation.
     This allows them to refer to attributes defined by other BaseDeclarations
     in the same factory.
     """
 
     FACTORY_BUILDER_PHASE = enums.BuilderPhase.ATTRIBUTE_RESOLUTION
 
+    #: Whether this declaration has a special handling for call-time overrides
+    #: (e.g. Tranformer).
+    #: Overridden values will be passed in the `extra` args.
+    CAPTURE_OVERRIDES = False
+
     #: Whether to unroll the context before evaluating the declaration.
     #: Set to False on declarations that perform their own unrolling.
     UNROLL_CONTEXT_BEFORE_EVALUATION = True
 
     def __init__(self, **defaults):
         super().__init__()
         self._defaults = defaults or {}
@@ -39,14 +44,28 @@
             # Optimization for simple contexts - don't do anything.
             return full_context
 
         import factory.base
         subfactory = factory.base.DictFactory
         return step.recurse(subfactory, full_context, force_sequence=step.sequence)
 
+    def _unwrap_evaluate_pre(self, wrapped, *, instance, step, overrides):
+        """Evaluate a wrapped pre-declaration.
+
+        This is especially useful for declarations wrapping another one,
+        e.g. Maybe or Transformer.
+        """
+        if isinstance(wrapped, BaseDeclaration):
+            return wrapped.evaluate_pre(
+                instance=instance,
+                step=step,
+                overrides=overrides,
+            )
+        return wrapped
+
     def evaluate_pre(self, instance, step, overrides):
         context = self.unroll_context(instance, step, overrides)
         return self.evaluate(instance, step, context)
 
     def evaluate(self, instance, step, extra):
         """Evaluate this declaration.
 
@@ -96,14 +115,57 @@
         self.function = function
 
     def evaluate(self, instance, step, extra):
         logger.debug("LazyAttribute: Evaluating %r on %r", self.function, instance)
         return self.function(instance)
 
 
+class Transformer(BaseDeclaration):
+    CAPTURE_OVERRIDES = True
+    UNROLL_CONTEXT_BEFORE_EVALUATION = False
+
+    class Force:
+        """
+        Bypass a transformer's transformation.
+
+        The forced value can be any declaration, and will be evaluated as if it
+        had been passed instead of the Transformer declaration.
+        """
+        def __init__(self, forced_value):
+            self.forced_value = forced_value
+
+        def __repr__(self):
+            return f'Transformer.Force({repr(self.forced_value)})'
+
+    def __init__(self, default, *, transform):
+        super().__init__()
+        self.default = default
+        self.transform = transform
+
+    def evaluate_pre(self, instance, step, overrides):
+        # The call-time value, if present, is set under the "" key.
+        value_or_declaration = overrides.pop("", self.default)
+
+        if isinstance(value_or_declaration, self.Force):
+            bypass_transform = True
+            value_or_declaration = value_or_declaration.forced_value
+        else:
+            bypass_transform = False
+
+        value = self._unwrap_evaluate_pre(
+            value_or_declaration,
+            instance=instance,
+            step=step,
+            overrides=overrides,
+        )
+        if bypass_transform:
+            return value
+        return self.transform(value)
+
+
 class _UNSPECIFIED:
     pass
 
 
 def deepgetattr(obj, name, default=_UNSPECIFIED):
     """Try to retrieve the given attribute of an object, digging on '.'.
 
@@ -472,24 +534,22 @@
         else:
             # Flat value (can't be ATTRIBUTE_RESOLUTION, checked in __init__)
             return target
 
     def evaluate_pre(self, instance, step, overrides):
         choice = self.decider.evaluate(instance=instance, step=step, extra={})
         target = self.yes if choice else self.no
-
-        if isinstance(target, BaseDeclaration):
-            return target.evaluate_pre(
-                instance=instance,
-                step=step,
-                overrides=overrides,
-            )
-        else:
-            # Flat value (can't be POST_INSTANTIATION, checked in __init__)
-            return target
+        # The value can't be POST_INSTANTIATION, checked in __init__;
+        # evaluate it as `evaluate_pre`
+        return self._unwrap_evaluate_pre(
+            target,
+            instance=instance,
+            step=step,
+            overrides=overrides,
+        )
 
     def __repr__(self):
         return f'Maybe({self.decider!r}, yes={self.yes!r}, no={self.no!r})'
 
 
 class Parameter(utils.OrderedBase):
     """A complex parameter, to be used in a Factory.Params section.
@@ -591,16 +651,16 @@
         )
         return self.call(instance, step, postgen_context)
 
     def call(self, instance, step, context):  # pragma: no cover
         """Call this hook; no return value is expected.
 
         Args:
-            obj (object): the newly generated object
-            create (bool): whether the object was 'built' or 'created'
+            instance (object): the newly generated object
+            step (bool): whether the object was 'built' or 'created'
             context: a builder.PostGenerationContext containing values
                 extracted from the containing factory's declaration
         """
         raise NotImplementedError()
 
 
 class PostGeneration(PostGenerationDeclaration):
```

### Comparing `factory_boy-3.2.1/factory/django.py` & `factory_boy-3.3.0/factory/django.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 """factory_boy extensions for use with the Django framework."""
 
 
 import functools
 import io
 import logging
 import os
+import warnings
 
+from django.contrib.auth.hashers import make_password
 from django.core import files as django_files
 from django.db import IntegrityError
 
 from . import base, declarations, errors
 
 logger = logging.getLogger('factory.generate')
 
@@ -43,14 +45,15 @@
 
 
 class DjangoOptions(base.FactoryOptions):
     def _build_default_options(self):
         return super()._build_default_options() + [
             base.OptionDefault('django_get_or_create', (), inherit=True),
             base.OptionDefault('database', DEFAULT_DB_ALIAS, inherit=True),
+            base.OptionDefault('skip_postgeneration_save', False, inherit=True),
         ]
 
     def _get_counter_reference(self):
         counter_reference = super()._get_counter_reference()
         if (counter_reference == self.base_factory
                 and self.base_factory._meta.model is not None
                 and self.base_factory._meta.model._meta.abstract
@@ -75,14 +78,15 @@
     This makes sure that the 'sequence' field of created objects is a new id.
 
     Possible improvement: define a new 'attribute' type, AutoField, which would
     handle those for non-numerical primary keys.
     """
 
     _options_class = DjangoOptions
+    _original_params = None
 
     class Meta:
         abstract = True  # Optional, but explicit.
 
     @classmethod
     def _load_model_class(cls, definition):
 
@@ -135,14 +139,18 @@
                     (field, cls.__name__))
             key_fields[field] = kwargs.pop(field)
         key_fields['defaults'] = kwargs
 
         try:
             instance, _created = manager.get_or_create(*args, **key_fields)
         except IntegrityError as e:
+
+            if cls._original_params is None:
+                raise e
+
             get_or_create_params = {
                 lookup: value
                 for lookup, value in cls._original_params.items()
                 if lookup in cls._meta.django_get_or_create
             }
             if get_or_create_params:
                 try:
@@ -161,53 +169,71 @@
         """Create an instance of the model, and save it to the database."""
         if cls._meta.django_get_or_create:
             return cls._get_or_create(model_class, *args, **kwargs)
 
         manager = cls._get_manager(model_class)
         return manager.create(*args, **kwargs)
 
+    # DEPRECATED. Remove this override with the next major release.
     @classmethod
     def _after_postgeneration(cls, instance, create, results=None):
         """Save again the instance if creating and at least one hook ran."""
-        if create and results:
+        if create and results and not cls._meta.skip_postgeneration_save:
+            warnings.warn(
+                f"{cls.__name__}._after_postgeneration will stop saving the instance "
+                "after postgeneration hooks in the next major release.\n"
+                "If the save call is extraneous, set skip_postgeneration_save=True "
+                f"in the {cls.__name__}.Meta.\n"
+                "To keep saving the instance, move the save call to your "
+                "postgeneration hooks or override _after_postgeneration.",
+                DeprecationWarning,
+            )
             # Some post-generation hooks ran, and may have modified us.
             instance.save()
 
 
+class Password(declarations.Transformer):
+    def __init__(self, password, transform=make_password, **kwargs):
+        super().__init__(password, transform=transform, **kwargs)
+
+
 class FileField(declarations.BaseDeclaration):
     """Helper to fill in django.db.models.FileField from a Factory."""
 
     DEFAULT_FILENAME = 'example.dat'
 
     def _make_data(self, params):
         """Create data for the field."""
         return params.get('data', b'')
 
     def _make_content(self, params):
         path = ''
 
-        _content_params = [params.get('from_path'), params.get('from_file'), params.get('from_func')]
-        if len([p for p in _content_params if p]) > 1:
+        from_path = params.get('from_path')
+        from_file = params.get('from_file')
+        from_func = params.get('from_func')
+
+        if len([p for p in (from_path, from_file, from_func) if p]) > 1:
             raise ValueError(
                 "At most one argument from 'from_file', 'from_path', and 'from_func' should "
                 "be non-empty when calling factory.django.FileField."
             )
 
-        if params.get('from_path'):
-            path = params['from_path']
+        if from_path:
+            path = from_path
             with open(path, 'rb') as f:
                 content = django_files.base.ContentFile(f.read())
 
-        elif params.get('from_file'):
-            f = params['from_file']
+        elif from_file:
+            f = from_file
             content = django_files.File(f)
             path = content.name
 
-        elif params.get('from_func'):
-            func = params['from_func']
+        elif from_func:
+            func = from_func
             content = django_files.File(func())
             path = content.name
 
         else:
             data = self._make_data(params)
             content = django_files.base.ContentFile(data)
 
@@ -297,14 +323,17 @@
         return mute_signals(*self.signals)
 
     def __call__(self, callable_obj):
         if isinstance(callable_obj, base.FactoryMetaClass):
             # Retrieve __func__, the *actual* callable object.
             callable_obj._create = self.wrap_method(callable_obj._create.__func__)
             callable_obj._generate = self.wrap_method(callable_obj._generate.__func__)
+            callable_obj._after_postgeneration = self.wrap_method(
+                callable_obj._after_postgeneration.__func__
+            )
             return callable_obj
 
         else:
             @functools.wraps(callable_obj)
             def wrapper(*args, **kwargs):
                 # A mute_signals() object is not reentrant; use a copy every time.
                 with self.copy():
```

### Comparing `factory_boy-3.2.1/factory/enums.py` & `factory_boy-3.3.0/factory/enums.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/factory/errors.py` & `factory_boy-3.3.0/factory/errors.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/factory/faker.py` & `factory_boy-3.3.0/factory/faker.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/factory/fuzzy.py` & `factory_boy-3.3.0/factory/fuzzy.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/factory/helpers.py` & `factory_boy-3.3.0/factory/helpers.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/factory/mogo.py` & `factory_boy-3.3.0/factory/mogo.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/factory/mongoengine.py` & `factory_boy-3.3.0/factory/mongoengine.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/factory/random.py` & `factory_boy-3.3.0/factory/random.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/factory/utils.py` & `factory_boy-3.3.0/factory/utils.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/factory_boy.egg-info/PKG-INFO` & `factory_boy-3.3.0/factory_boy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: factory-boy
-Version: 3.2.1
+Version: 3.3.0
 Summary: A versatile test fixtures replacement based on thoughtbot's factory_bot for Ruby.
 Home-page: https://github.com/FactoryBoy/factory_boy
 Author: Mark Sandstrom
 Author-email: mark@deliciouslynerdy.com
 Maintainer: Raphaël Barrois
 Maintainer-email: raphael.barrois+fboy@polytechnique.org
 License: MIT
 Keywords: factory_boy,factory,fixtures
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 factory_boy
 ===========
 
@@ -188,30 +188,30 @@
 
 More details can be found in the ORM section.
 
 
 Using factories
 """""""""""""""
 
-factory_boy supports several different build strategies: build, create, and stub:
+factory_boy supports several different instantiation strategies: build, create, and stub:
 
 .. code-block:: python
 
     # Returns a User instance that's not saved
     user = UserFactory.build()
 
     # Returns a saved User instance.
     # UserFactory must subclass an ORM base class, such as DjangoModelFactory.
     user = UserFactory.create()
 
     # Returns a stub object (just a bunch of attributes)
     obj = UserFactory.stub()
 
 
-You can use the Factory class as a shortcut for the default build strategy:
+You can use the Factory class as a shortcut for the default instantiation strategy:
 
 .. code-block:: python
 
     # Same as UserFactory.create()
     user = UserFactory()
 
 
@@ -357,15 +357,15 @@
 
 Support Policy
 --------------
 
 ``factory_boy`` supports active Python versions as well as PyPy3.
 
 - **Python**'s `supported versions
-  <https://devguide.python.org/#status-of-python-branches>`__.
+  <https://devguide.python.org/versions/#supported-versions>`__.
 - **Django**'s `supported
   versions <https://www.djangoproject.com/download/#supported-versions>`__.
 - **SQLAlchemy**: `latest version on PyPI <https://pypi.org/project/SQLAlchemy/>`__.
 - **MongoEngine**: `latest version on PyPI <https://pypi.org/project/mongoengine/>`__.
 
 Debugging factory_boy
 ---------------------
@@ -433,24 +433,60 @@
 To test with a specific framework version, you may use a ``tox`` target:
 
 .. code-block:: sh
 
     # list all tox environments
     $ tox --listenvs
 
-    # run tests inside a specific environment
-    $ tox -e py36-django20-alchemy13-mongoengine017
+    # run tests inside a specific environment (django/mongoengine/SQLAlchemy are not installed)
+    $ tox -e py310
 
-Valid options are:
+    # run tests inside a specific environment (django)
+    $ tox -e py310-djangomain
+    $ tox -e py310-djangomain-postgres
 
-* ``DJANGO`` for ``Django``
-* ``MONGOENGINE`` for ``mongoengine``
-* ``ALCHEMY`` for ``SQLAlchemy``
+    # run tests inside a specific environment (alchemy)
+    $ tox -e py310-alchemy
+    $ tox -e py310-alchemy-postgres
 
+    # run tests inside a specific environment (mongoengine)
+    $ tox -e py310-mongo
 
-To avoid running ``mongoengine`` tests (e.g no MongoDB server installed), run:
+
+Packaging
+---------
+
+For users interesting in packaging FactoryBoy into downstream distribution channels
+(e.g. ``.deb``, ``.rpm``, ``.ebuild``), the following tips might be helpful:
+
+Dependencies
+""""""""""""
+
+The package's run-time dependencies are listed in ``setup.cfg``.
+The dependencies useful for building and testing the library are covered by the
+``dev`` and ``doc`` extras.
+
+Moreover, all development / testing tasks are driven through ``make(1)``.
+
+Building
+""""""""
+
+In order to run the build steps (currently only for docs), run:
+
+.. code-block:: sh
+
+    python setup.py egg_info
+    make doc
+
+Testing
+"""""""
+
+When testing for the active Python environment, run the following:
 
 .. code-block:: sh
 
-    $ make SKIP_MONGOENGINE=1 test
+    make test
 
+.. note::
 
+    You must make sure that the ``factory`` module is importable, as it is imported from
+    the testing code.
```

### Comparing `factory_boy-3.2.1/factory_boy.egg-info/SOURCES.txt` & `factory_boy-3.3.0/factory_boy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 factory/mogo.py
 factory/mongoengine.py
 factory/random.py
 factory/utils.py
 factory_boy.egg-info/PKG-INFO
 factory_boy.egg-info/SOURCES.txt
 factory_boy.egg-info/dependency_links.txt
-factory_boy.egg-info/not-zip-safe
 factory_boy.egg-info/requires.txt
 factory_boy.egg-info/top_level.txt
 tests/__init__.py
 tests/alter_time.py
 tests/test_alchemy.py
 tests/test_base.py
 tests/test_declarations.py
@@ -78,22 +77,25 @@
 tests/test_django.py
 tests/test_docs_internals.py
 tests/test_faker.py
 tests/test_fuzzy.py
 tests/test_helpers.py
 tests/test_mongoengine.py
 tests/test_regression.py
+tests/test_transformer.py
 tests/test_using.py
 tests/test_utils.py
+tests/test_version.py
 tests/utils.py
 tests/alchemyapp/__init__.py
 tests/alchemyapp/models.py
 tests/cyclic/__init__.py
 tests/cyclic/bar.py
 tests/cyclic/foo.py
 tests/cyclic/self_ref.py
 tests/djapp/__init__.py
 tests/djapp/models.py
 tests/djapp/settings.py
+tests/djapp/settings_pg.py
 tests/testdata/__init__.py
 tests/testdata/example.data
 tests/testdata/example.jpeg
```

### Comparing `factory_boy-3.2.1/setup.cfg` & `factory_boy-3.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 [metadata]
 name = factory_boy
-version = 3.2.1
+version = 3.3.0
 description = A versatile test fixtures replacement based on thoughtbot's factory_bot for Ruby.
 long_description = file: README.rst
+long_description_content_type = text/x-rst
 author = Mark Sandstrom
 author_email = mark@deliciouslynerdy.com
 maintainer = Raphaël Barrois
 maintainer_email = raphael.barrois+fboy@polytechnique.org
 url = https://github.com/FactoryBoy/factory_boy
 keywords = factory_boy, factory, fixtures
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
-	Framework :: Django :: 2.2
-	Framework :: Django :: 3.0
-	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
+	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development :: Testing
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
-zip_safe = false
 packages = factory
-python_requires = >=3.6
-install_requires = Faker>=0.7.0
+python_requires = >=3.7
+install_requires = 
+	Faker>=0.7.0
+	importlib_metadata;python_version<"3.8"
 
 [options.extras_require]
 dev = 
 	coverage
 	Django
 	flake8
 	isort
 	Pillow
 	SQLAlchemy
+	sqlalchemy_utils
 	mongoengine
 	wheel>=0.32.0
 	tox
 	zest.releaser[recommended]
 doc = 
 	Sphinx
 	sphinx_rtd_theme
@@ -73,11 +76,22 @@
 [isort]
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
 line_length = 88
 
+[coverage:run]
+dynamic_context = test_function
+
+[coverage:report]
+include = 
+	factory/*.py
+	tests/*.py
+
+[coverage:html]
+show_contexts = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `factory_boy-3.2.1/tests/alter_time.py` & `factory_boy-3.3.0/tests/alter_time.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/tests/djapp/models.py` & `factory_boy-3.3.0/tests/djapp/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class NonIntegerPk(models.Model):
     foo = models.CharField(max_length=20, primary_key=True)
     bar = models.CharField(max_length=20, blank=True)
 
 
 class MultifieldModel(models.Model):
     slug = models.SlugField(max_length=20, unique=True)
-    text = models.CharField(max_length=20)
+    text = models.TextField()
 
 
 class MultifieldUniqueModel(models.Model):
     slug = models.SlugField(max_length=20, unique=True)
     text = models.CharField(max_length=20, unique=True)
     title = models.CharField(max_length=20, unique=True)
 
@@ -72,14 +72,18 @@
     )
 
 
 class WithDefaultValue(models.Model):
     foo = models.CharField(max_length=20, default='')
 
 
+class WithPassword(models.Model):
+    pw = models.CharField(max_length=128)
+
+
 WITHFILE_UPLOAD_TO = 'django'
 WITHFILE_UPLOAD_DIR = os.path.join(settings.MEDIA_ROOT, WITHFILE_UPLOAD_TO)
 
 
 class WithFile(models.Model):
     afile = models.FileField(upload_to=WITHFILE_UPLOAD_TO)
 
@@ -125,7 +129,11 @@
 
     class Meta:
         abstract = True
 
 
 class FromAbstractWithCustomManager(AbstractWithCustomManager):
     pass
+
+
+class HasMultifieldModel(models.Model):
+    multifield = models.ForeignKey(to=MultifieldModel, on_delete=models.CASCADE)
```

### Comparing `factory_boy-3.2.1/tests/djapp/settings.py` & `factory_boy-3.3.0/tests/djapp/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,7 +25,11 @@
 INSTALLED_APPS = [
     'tests.djapp'
 ]
 
 MIDDLEWARE_CLASSES = ()
 
 SECRET_KEY = 'testing.'
+
+# TODO: Will be the default after Django 5.0. Remove this setting when
+# Django 5.0 is the last supported version.
+USE_TZ = True
```

### Comparing `factory_boy-3.2.1/tests/test_alchemy.py` & `factory_boy-3.3.0/tests/test_alchemy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # Copyright: See the LICENSE file.
 
 """Tests for factory_boy/SQLAlchemy interactions."""
 
 import unittest
 from unittest import mock
 
-import sqlalchemy
+try:
+    import sqlalchemy
+except ImportError:
+    raise unittest.SkipTest("sqlalchemy tests disabled.")
+
+from sqlalchemy_utils import create_database, database_exists, drop_database
 
 import factory
 from factory.alchemy import SQLAlchemyModelFactory
 
 from .alchemyapp import models
 
 
@@ -68,19 +73,38 @@
         sqlalchemy_session_persistence = 'commit'
 
     id = factory.Sequence(lambda n: n)
     slug = factory.Sequence(lambda n: "slug%s" % n)
     text = factory.Sequence(lambda n: "text%s" % n)
 
 
-class SQLAlchemyPkSequenceTestCase(unittest.TestCase):
+if models.USING_POSTGRES:
+    # sqlite test database gets created/destroyed automatically, postgres does not.
+
+    def setUpModule():
+        if not database_exists(models.engine.url):
+            create_database(models.engine.url)
+
+    def tearDownModule():
+        drop_database(models.engine.url)
+
+
+class TransactionTestCase(unittest.TestCase):
+    def setUp(self):
+        models.Base.metadata.create_all(models.engine)
+
+    def tearDown(self):
+        models.session.remove()
+        models.Base.metadata.drop_all(models.engine)
+
+
+class SQLAlchemyPkSequenceTestCase(TransactionTestCase):
     def setUp(self):
         super().setUp()
         StandardFactory.reset_sequence(1)
-        NonIntegerPkFactory._meta.sqlalchemy_session.rollback()
 
     def test_pk_first(self):
         std = StandardFactory.build()
         self.assertEqual('foo1', std.foo)
 
     def test_pk_many(self):
         std1 = StandardFactory.build()
@@ -105,18 +129,15 @@
 
         StandardFactory.reset_sequence()
         std2 = StandardFactory.create()
         self.assertEqual('foo0', std2.foo)  # Sequence doesn't care about pk
         self.assertEqual(0, std2.id)
 
 
-class SQLAlchemyGetOrCreateTests(unittest.TestCase):
-    def setUp(self):
-        models.session.rollback()
-
+class SQLAlchemyGetOrCreateTests(TransactionTestCase):
     def test_simple_call(self):
         obj1 = WithGetOrCreateFieldFactory(foo='foo1')
         obj2 = WithGetOrCreateFieldFactory(foo='foo1')
         self.assertEqual(obj1, obj2)
 
     def test_missing_arg(self):
         with self.assertRaises(factory.FactoryError):
@@ -134,24 +155,21 @@
         )
         self.assertEqual(6, len(objs))
         self.assertEqual(2, len(set(objs)))
         self.assertEqual(
             list(
                 obj.slug for obj in models.session.query(
                     models.MultiFieldModel.slug
-                )
+                ).order_by(models.MultiFieldModel.slug)
             ),
             ["alt", "main"],
         )
 
 
-class MultipleGetOrCreateFieldsTest(unittest.TestCase):
-    def setUp(self):
-        models.session.rollback()
-
+class MultipleGetOrCreateFieldsTest(TransactionTestCase):
     def test_one_defined(self):
         obj1 = WithMultipleGetOrCreateFieldsFactory()
         obj2 = WithMultipleGetOrCreateFieldsFactory(slug=obj1.slug)
         self.assertEqual(obj1, obj2)
 
     def test_both_defined(self):
         obj1 = WithMultipleGetOrCreateFieldsFactory()
@@ -212,19 +230,18 @@
         with self.assertRaises(TypeError):
             class BadPersistenceFactory(StandardFactory):
                 class Meta:
                     sqlalchemy_session_persistence = 'invalid_persistence_option'
                     model = models.StandardModel
 
 
-class SQLAlchemyNonIntegerPkTestCase(unittest.TestCase):
-    def setUp(self):
-        super().setUp()
+class SQLAlchemyNonIntegerPkTestCase(TransactionTestCase):
+    def tearDown(self):
+        super().tearDown()
         NonIntegerPkFactory.reset_sequence()
-        NonIntegerPkFactory._meta.sqlalchemy_session.rollback()
 
     def test_first(self):
         nonint = NonIntegerPkFactory.build()
         self.assertEqual('foo0', nonint.id)
 
     def test_many(self):
         nonint1 = NonIntegerPkFactory.build()
@@ -246,28 +263,56 @@
         self.assertEqual('foo10', nonint1.id)
 
         NonIntegerPkFactory.reset_sequence()
         nonint2 = NonIntegerPkFactory.create()
         self.assertEqual('foo0', nonint2.id)
 
 
-class SQLAlchemyNoSessionTestCase(unittest.TestCase):
+class SQLAlchemyNoSessionTestCase(TransactionTestCase):
 
     def test_create_raises_exception_when_no_session_was_set(self):
         with self.assertRaises(RuntimeError):
             NoSessionFactory.create()
 
     def test_build_does_not_raises_exception_when_no_session_was_set(self):
+        NoSessionFactory.reset_sequence()  # Make sure we start at test ID 0
         inst0 = NoSessionFactory.build()
         inst1 = NoSessionFactory.build()
         self.assertEqual(inst0.id, 0)
         self.assertEqual(inst1.id, 1)
 
 
-class NameConflictTests(unittest.TestCase):
+class SQLAlchemySessionFactoryTestCase(TransactionTestCase):
+    def test_create_get_session_from_sqlalchemy_session_factory(self):
+        class SessionGetterFactory(SQLAlchemyModelFactory):
+            class Meta:
+                model = models.StandardModel
+                sqlalchemy_session = None
+                sqlalchemy_session_factory = lambda: models.session
+
+            id = factory.Sequence(lambda n: n)
+
+        SessionGetterFactory.create()
+        self.assertEqual(SessionGetterFactory._meta.sqlalchemy_session, models.session)
+        # Reuse the session obtained from sqlalchemy_session_factory.
+        SessionGetterFactory.create()
+
+    def test_create_raise_exception_sqlalchemy_session_factory_not_callable(self):
+        message = "^Provide either a sqlalchemy_session or a sqlalchemy_session_factory, not both$"
+        with self.assertRaisesRegex(RuntimeError, message):
+            class SessionAndGetterFactory(SQLAlchemyModelFactory):
+                class Meta:
+                    model = models.StandardModel
+                    sqlalchemy_session = models.session
+                    sqlalchemy_session_factory = lambda: models.session
+
+                id = factory.Sequence(lambda n: n)
+
+
+class NameConflictTests(TransactionTestCase):
     """Regression test for `TypeError: _save() got multiple values for argument 'session'`
 
     See #775.
     """
     def test_no_name_conflict_on_save(self):
         class SpecialFieldWithSaveFactory(SQLAlchemyModelFactory):
             class Meta:
```

### Comparing `factory_boy-3.2.1/tests/test_base.py` & `factory_boy-3.3.0/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
         self.assertEqual(1, o2.one)
 
         self.TestObjectFactory.reset_sequence(42)
         o3 = self.TestObjectFactory()
         self.assertEqual(42, o3.one)
 
     def test_reset_sequence_subclass_fails(self):
-        """Tests that the sequence of a 'slave' factory cannot be reseted."""
+        """Tests that the sequence of a 'slave' factory cannot be reset."""
         class SubTestObjectFactory(self.TestObjectFactory):
             pass
 
         with self.assertRaises(ValueError):
             SubTestObjectFactory.reset_sequence()
 
     def test_reset_sequence_subclass_force(self):
@@ -339,15 +339,15 @@
         self.assertEqual(0, o3.one)
 
         # The master sequence counter has been reset
         o4 = self.TestObjectFactory()
         self.assertEqual(1, o4.one)
 
     def test_reset_sequence_subclass_parent(self):
-        """Tests that the sequence of a 'slave' factory cannot be reseted."""
+        """Tests that the sequence of a 'slave' factory cannot be reset."""
         class SubTestObjectFactory(self.TestObjectFactory):
             pass
 
         o1 = SubTestObjectFactory()
         self.assertEqual(0, o1.one)
 
         o2 = SubTestObjectFactory()
```

### Comparing `factory_boy-3.2.1/tests/test_declarations.py` & `factory_boy-3.3.0/tests/test_declarations.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,20 @@
         it = declarations.Iterator([(1, 2), (1, 3)], getter=lambda p: p[1])
         self.assertEqual(2, utils.evaluate_declaration(it, force_sequence=0))
         self.assertEqual(3, utils.evaluate_declaration(it, force_sequence=1))
         self.assertEqual(2, utils.evaluate_declaration(it, force_sequence=2))
         self.assertEqual(3, utils.evaluate_declaration(it, force_sequence=3))
 
 
+class TransformerTestCase(unittest.TestCase):
+    def test_transform(self):
+        t = declarations.Transformer('foo', transform=str.upper)
+        self.assertEqual("FOO", utils.evaluate_declaration(t))
+
+
 class PostGenerationDeclarationTestCase(unittest.TestCase):
     def test_post_generation(self):
         call_params = []
 
         def foo(*args, **kwargs):
             call_params.append(args)
             call_params.append(kwargs)
```

### Comparing `factory_boy-3.2.1/tests/test_dev_experience.py` & `factory_boy-3.3.0/tests/test_dev_experience.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/tests/test_django.py` & `factory_boy-3.3.0/tests/test_django.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,28 @@
 """Tests for factory_boy/Django interactions."""
 
 import io
 import os
 import unittest
 from unittest import mock
 
-import django
+try:
+    import django
+except ImportError:
+    raise unittest.SkipTest("django tests disabled.")
+
 from django import test as django_test
 from django.conf import settings
+from django.contrib.auth.hashers import check_password
+from django.core.management import color
+from django.db import IntegrityError, connections
 from django.db.models import signals
 from django.test import utils as django_test_utils
 
+import factory
 import factory.django
 
 from . import testdata
 
 try:
     from PIL import Image
 except ImportError:
@@ -93,14 +101,24 @@
 
 
 class ConcreteGrandSonFactory(AbstractBaseFactory):
     class Meta:
         model = models.ConcreteGrandSon
 
 
+PASSWORD = 's0_s3cr3t'
+
+
+class WithPasswordFactory(factory.django.DjangoModelFactory):
+    class Meta:
+        model = models.WithPassword
+
+    pw = factory.django.Password(password=PASSWORD)
+
+
 class WithFileFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = models.WithFile
 
     afile = factory.django.FileField()
 
 
@@ -149,15 +167,24 @@
                 database = 'replica'
 
         obj = OtherDBFactory()
         self.assertFalse(models.StandardModel.objects.exists())
         self.assertEqual(obj, models.StandardModel.objects.using('replica').get())
 
 
-class DjangoPkSequenceTestCase(django_test.TestCase):
+class DjangoResetTestCase(django_test.TestCase):
+    def reset_database_sequences(self, *models):
+        using = factory.django.DEFAULT_DB_ALIAS
+        with connections[using].cursor() as cursor:
+            sequence_sql = connections[using].ops.sequence_reset_sql(color.no_style(), models)
+            for command in sequence_sql:
+                cursor.execute(command)
+
+
+class DjangoPkSequenceTestCase(DjangoResetTestCase):
     def setUp(self):
         super().setUp()
         StandardFactory.reset_sequence()
 
     def test_pk_first(self):
         std = StandardFactory.build()
         self.assertEqual('foo0', std.foo)
@@ -165,28 +192,32 @@
     def test_pk_many(self):
         std1 = StandardFactory.build()
         std2 = StandardFactory.build()
         self.assertEqual('foo0', std1.foo)
         self.assertEqual('foo1', std2.foo)
 
     def test_pk_creation(self):
+        self.reset_database_sequences(StandardFactory._meta.model)
+
         std1 = StandardFactory.create()
         self.assertEqual('foo0', std1.foo)
         self.assertEqual(1, std1.pk)
 
         StandardFactory.reset_sequence()
         std2 = StandardFactory.create()
         self.assertEqual('foo0', std2.foo)
         self.assertEqual(2, std2.pk)
 
     def test_pk_force_value(self):
         std1 = StandardFactory.create(pk=10)
         self.assertEqual('foo0', std1.foo)  # sequence is unrelated to pk
         self.assertEqual(10, std1.pk)
 
+        self.reset_database_sequences(StandardFactory._meta.model)
+
         StandardFactory.reset_sequence()
         std2 = StandardFactory.create()
         self.assertEqual('foo0', std2.foo)
         self.assertEqual(11, std2.pk)
 
 
 class DjangoGetOrCreateTests(django_test.TestCase):
@@ -359,15 +390,15 @@
 
         NonIntegerPkFactory.reset_sequence()
         nonint2 = NonIntegerPkFactory.create()
         self.assertEqual('foo0', nonint2.foo)
         self.assertEqual('foo0', nonint2.pk)
 
 
-class DjangoAbstractBaseSequenceTestCase(django_test.TestCase):
+class DjangoAbstractBaseSequenceTestCase(DjangoResetTestCase):
     def test_auto_sequence_son(self):
         """The sequence of the concrete son of an abstract model should be autonomous."""
         obj = ConcreteSonFactory()
         self.assertEqual(1, obj.pk)
 
     def test_auto_sequence_grandson(self):
         """The sequence of the concrete grandson of an abstract model should be autonomous."""
@@ -382,14 +413,16 @@
 
             foo = factory.Sequence(lambda n: "foo%d" % n)
 
         class ConcreteSonFactory(AbstractBaseFactory):
             class Meta:
                 model = models.ConcreteSon
 
+        self.reset_database_sequences(models.ConcreteSon)
+
         obj = ConcreteSonFactory()
         self.assertEqual(1, obj.pk)
         self.assertEqual("foo0", obj.foo)
 
 
 class DjangoRelatedFieldTestCase(django_test.TestCase):
 
@@ -410,14 +443,17 @@
 
         class PointedRelatedFactory(PointedFactory):
             pointer = factory.RelatedFactory(
                 PointerFactory,
                 factory_related_name='pointed',
             )
 
+            class Meta:
+                skip_postgeneration_save = True
+
         class PointerExtraFactory(PointerFactory):
             pointed__foo = 'extra_new_foo'
 
         class PointedRelatedExtraFactory(PointedRelatedFactory):
             pointer__bar = 'extra_new_bar'
 
         class PointedRelatedWithTraitFactory(PointedFactory):
@@ -426,14 +462,17 @@
                     pointer=factory.RelatedFactory(
                         PointerFactory,
                         factory_related_name='pointed',
                         bar='with_trait',
                     )
                 )
 
+            class Meta:
+                skip_postgeneration_save = True
+
         cls.PointedFactory = PointedFactory
         cls.PointerFactory = PointerFactory
         cls.PointedRelatedFactory = PointedRelatedFactory
         cls.PointerExtraFactory = PointerExtraFactory
         cls.PointedRelatedExtraFactory = PointedRelatedExtraFactory
         cls.PointedRelatedWithTraitFactory = PointedRelatedWithTraitFactory
 
@@ -488,14 +527,29 @@
         )
         self.assertEqual(pointed, models.PointedModel.objects.get())
         self.assertEqual(pointed.foo, 'foo')
         self.assertEqual(pointed.pointer, models.PointerModel.objects.get())
         self.assertEqual(pointed.pointer.bar, 'with_trait')
 
 
+class DjangoPasswordTestCase(django_test.TestCase):
+    def test_build(self):
+        u = WithPasswordFactory.build()
+        self.assertTrue(check_password(PASSWORD, u.pw))
+
+    def test_build_with_kwargs(self):
+        password = 'V3R¥.S€C®€T'
+        u = WithPasswordFactory.build(pw=password)
+        self.assertTrue(check_password(password, u.pw))
+
+    def test_create(self):
+        u = WithPasswordFactory.create()
+        self.assertTrue(check_password(PASSWORD, u.pw))
+
+
 class DjangoFileFieldTestCase(django_test.TestCase):
 
     def tearDown(self):
         super().tearDown()
         for path in os.listdir(models.WITHFILE_UPLOAD_DIR):
             # Remove temporary files written during tests.
             os.unlink(os.path.join(models.WITHFILE_UPLOAD_DIR, path))
@@ -915,14 +969,15 @@
         self.assertSignalsReactivated()
 
     def test_class_decorator_with_subfactory(self):
         @factory.django.mute_signals(signals.pre_save, signals.post_save)
         class WithSignalsDecoratedFactory(factory.django.DjangoModelFactory):
             class Meta:
                 model = models.WithSignals
+                skip_postgeneration_save = True
 
             @factory.post_generation
             def post(obj, create, extracted, **kwargs):
                 if not extracted:
                     WithSignalsDecoratedFactory.create(post=42)
 
         # This will disable the signals (twice), create two objects,
@@ -931,14 +986,49 @@
 
         self.assertEqual(self.handlers.pre_init.call_count, 2)
         self.assertFalse(self.handlers.pre_save.called)
         self.assertFalse(self.handlers.post_save.called)
 
         self.assertSignalsReactivated()
 
+    def test_class_decorator_related_model_with_post_hook(self):
+        """
+        Related factory with post_generation hook should not call disabled signals.
+
+        Refs https://github.com/FactoryBoy/factory_boy/issues/424
+        """
+
+        @factory.django.mute_signals(signals.post_save)
+        class PointedFactory(factory.django.DjangoModelFactory):
+            class Meta:
+                model = models.PointedModel
+                skip_postgeneration_save = True
+
+            @factory.post_generation
+            def post_action(obj, create, extracted, **kwargs):
+                pass
+
+        class PointerFactory(factory.django.DjangoModelFactory):
+            pointed = factory.SubFactory(PointedFactory)
+
+            class Meta:
+                model = models.PointerModel
+
+        PointerFactory.create()
+
+        self.handlers.post_save.assert_called_once_with(
+            signal=mock.ANY,
+            sender=models.PointerModel,
+            instance=mock.ANY,
+            created=True,
+            update_fields=None,
+            raw=False,
+            using="default",
+        )
+
     def test_class_decorator_build(self):
         @factory.django.mute_signals(signals.pre_save, signals.post_save)
         class WithSignalsDecoratedFactory(factory.django.DjangoModelFactory):
             class Meta:
                 model = models.WithSignals
 
         WithSignalsDecoratedFactory.build()
@@ -1001,14 +1091,15 @@
         UndecoratedFactory()
         self.post_save_mock.assert_not_called()
 
     def test_class_decorator_with_muted_related_factory(self):
         class UndecoratedFactory(factory.django.DjangoModelFactory):
             class Meta:
                 model = models.PointerModel
+                skip_postgeneration_save = True
             pointed = factory.RelatedFactory(self.WithSignalsDecoratedFactory)
 
         UndecoratedFactory()
         self.post_save_mock.assert_not_called()
 
 
 class DjangoCustomManagerTestCase(django_test.TestCase):
@@ -1021,7 +1112,58 @@
         class ObjFactory(factory.django.DjangoModelFactory):
             class Meta:
                 model = models.FromAbstractWithCustomManager
 
         # Our CustomManager will remove the 'arg=' argument,
         # invalid for the actual model.
         ObjFactory.create(arg='invalid')
+
+
+class DjangoModelFactoryDuplicateSaveDeprecationTest(django_test.TestCase):
+    class StandardFactoryWithPost(StandardFactory):
+        @factory.post_generation
+        def post_action(obj, create, extracted, **kwargs):
+            return 3
+
+    def test_create_warning(self):
+        with self.assertWarns(DeprecationWarning) as cm:
+            self.StandardFactoryWithPost.create()
+
+        [msg] = cm.warning.args
+        self.assertEqual(
+            msg,
+            "StandardFactoryWithPost._after_postgeneration will stop saving the "
+            "instance after postgeneration hooks in the next major release.\n"
+            "If the save call is extraneous, set skip_postgeneration_save=True in the "
+            "StandardFactoryWithPost.Meta.\n"
+            "To keep saving the instance, move the save call to your postgeneration "
+            "hooks or override _after_postgeneration.",
+        )
+
+    def test_build_no_warning(self):
+        self.StandardFactoryWithPost.build()
+
+
+class IntegrityErrorForMissingOriginalParamsTest(django_test.TestCase):
+
+    def test_raises_integrity_error(self):
+        """
+        In factory.django.DjangoModelFactory._get_or_create
+        _original_params can give some trouble when None
+
+        This test case verifies if the IntegrityError is correctly re-raised
+        """
+
+        class MultifieldModelFactory2(MultifieldModelFactory):
+            class Meta:
+                model = models.MultifieldModel
+                django_get_or_create = ['text']
+
+        class HasMultifieldModelFactory(factory.django.DjangoModelFactory):
+            multifield = factory.SubFactory(MultifieldModelFactory2)
+
+            class Meta:
+                model = models.HasMultifieldModel
+
+        HasMultifieldModelFactory(multifield__slug="test")
+        with self.assertRaises(IntegrityError):
+            HasMultifieldModelFactory(multifield__slug="test")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `factory_boy-3.2.1/tests/test_docs_internals.py` & `factory_boy-3.3.0/tests/test_docs_internals.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/tests/test_faker.py` & `factory_boy-3.3.0/tests/test_faker.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                 'date_between_dates',
                 start_date=factory.SelfAttribute('..departure'),
                 end_date=factory.SelfAttribute('..arrival'),
             )
 
         def fake_select_date(start_date, end_date):
             """Fake date_between_dates."""
-            # Ensure that dates have been transfered from the factory
+            # Ensure that dates have been transferred from the factory
             # to Faker parameters.
             self.assertEqual(start_date, may_4th)
             self.assertEqual(end_date, may_25th)
             return october_19th
 
         self._setup_advanced_mock_faker(
             date_between_dates=fake_select_date,
```

### Comparing `factory_boy-3.2.1/tests/test_fuzzy.py` & `factory_boy-3.3.0/tests/test_fuzzy.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/tests/test_helpers.py` & `factory_boy-3.3.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/tests/test_mongoengine.py` & `factory_boy-3.3.0/tests/test_mongoengine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Copyright: See the LICENSE file.
 
 """Tests for factory_boy/MongoEngine interactions."""
 
 import os
 import unittest
 
-import mongoengine
+try:
+    import mongoengine
+except ImportError:
+    raise unittest.SkipTest("mongodb tests disabled.")
 
 import factory
 from factory.mongoengine import MongoEngineFactory
 
 
 class Address(mongoengine.EmbeddedDocument):
     street = mongoengine.StringField()
@@ -31,18 +34,14 @@
     class Meta:
         model = Person
 
     name = factory.Sequence(lambda n: 'name%d' % n)
     address = factory.SubFactory(AddressFactory)
 
 
-SKIP_MONGODB = bool(os.environ.get('SKIP_MONGOENGINE') == '1')
-
-
-@unittest.skipIf(SKIP_MONGODB, "mongodb tests disabled.")
 class MongoEngineTestCase(unittest.TestCase):
 
     db_name = os.environ.get('MONGO_DATABASE', 'factory_boy_test')
     db_host = os.environ.get('MONGO_HOST', 'localhost')
     db_port = int(os.environ.get('MONGO_PORT', '27017'))
     server_timeout_ms = int(os.environ.get('MONGO_TIMEOUT', '300'))
 
@@ -53,14 +52,15 @@
             db=cls.db_name,
             host=cls.db_host,
             port=cls.db_port,
             # PyMongo>=2.1 requires an explicit read_preference.
             read_preference=mongo_rp.ReadPreference.PRIMARY,
             # PyMongo>=2.1 has a 20s timeout, use 100ms instead
             serverselectiontimeoutms=cls.server_timeout_ms,
+            uuidRepresentation='standard',
         )
 
     @classmethod
     def tearDownClass(cls):
         cls.db.drop_database(cls.db_name)
 
     def test_build(self):
```

### Comparing `factory_boy-3.2.1/tests/test_regression.py` & `factory_boy-3.3.0/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/tests/test_using.py` & `factory_boy-3.3.0/tests/test_using.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 import unittest
 
 import factory
 from factory import errors
 
 from . import utils
 
+try:
+    import django  # noqa: F401
+    SKIP_DJANGO = False
+except ImportError:
+    SKIP_DJANGO = True
+
 
 class TestObject:
     def __init__(self, one=None, two=None, three=None, four=None, five=None):
         self.one = one
         self.two = two
         self.three = three
         self.four = four
@@ -137,14 +143,15 @@
             self.assertEqual(obj.four, None)
 
     def test_create(self):
         obj = factory.create(FakeModel, foo='bar')
         self.assertEqual(obj.id, None)
         self.assertEqual(obj.foo, 'bar')
 
+    @unittest.skipIf(SKIP_DJANGO, "django tests disabled.")
     def test_create_custom_base(self):
         obj = factory.create(FakeModel, foo='bar', FACTORY_CLASS=factory.django.DjangoModelFactory)
         self.assertEqual(obj.id, 2)
         self.assertEqual(obj.foo, 'bar')
 
     def test_create_batch(self):
         objs = factory.create_batch(FakeModel, 4, foo='bar')
@@ -152,14 +159,15 @@
         self.assertEqual(4, len(objs))
         self.assertEqual(4, len(set(objs)))
 
         for obj in objs:
             self.assertEqual(obj.id, None)
             self.assertEqual(obj.foo, 'bar')
 
+    @unittest.skipIf(SKIP_DJANGO, "django tests disabled.")
     def test_create_batch_custom_base(self):
         objs = factory.create_batch(
             FakeModel,
             4,
             foo='bar',
             FACTORY_CLASS=factory.django.DjangoModelFactory,
         )
@@ -192,14 +200,15 @@
         self.assertEqual(obj.foo, 'bar')
 
     def test_generate_create(self):
         obj = factory.generate(FakeModel, factory.CREATE_STRATEGY, foo='bar')
         self.assertEqual(obj.id, None)
         self.assertEqual(obj.foo, 'bar')
 
+    @unittest.skipIf(SKIP_DJANGO, "django tests disabled.")
     def test_generate_create_custom_base(self):
         obj = factory.generate(
             FakeModel,
             factory.CREATE_STRATEGY,
             foo='bar',
             FACTORY_CLASS=factory.django.DjangoModelFactory,
         )
@@ -227,14 +236,15 @@
         self.assertEqual(20, len(objs))
         self.assertEqual(20, len(set(objs)))
 
         for obj in objs:
             self.assertEqual(obj.id, None)
             self.assertEqual(obj.foo, 'bar')
 
+    @unittest.skipIf(SKIP_DJANGO, "django tests disabled.")
     def test_generate_batch_create_custom_base(self):
         objs = factory.generate_batch(
             FakeModel,
             factory.CREATE_STRATEGY,
             20,
             foo='bar',
             FACTORY_CLASS=factory.django.DjangoModelFactory,
@@ -263,14 +273,15 @@
         self.assertEqual(obj.foo, 'bar')
 
     def test_simple_generate_create(self):
         obj = factory.simple_generate(FakeModel, True, foo='bar')
         self.assertEqual(obj.id, None)
         self.assertEqual(obj.foo, 'bar')
 
+    @unittest.skipIf(SKIP_DJANGO, "django tests disabled.")
     def test_simple_generate_create_custom_base(self):
         obj = factory.simple_generate(FakeModel, True, foo='bar', FACTORY_CLASS=factory.django.DjangoModelFactory)
         self.assertEqual(obj.id, 2)
         self.assertEqual(obj.foo, 'bar')
 
     def test_simple_generate_batch_build(self):
         objs = factory.simple_generate_batch(FakeModel, False, 20, foo='bar')
@@ -288,14 +299,15 @@
         self.assertEqual(20, len(objs))
         self.assertEqual(20, len(set(objs)))
 
         for obj in objs:
             self.assertEqual(obj.id, None)
             self.assertEqual(obj.foo, 'bar')
 
+    @unittest.skipIf(SKIP_DJANGO, "django tests disabled.")
     def test_simple_generate_batch_create_custom_base(self):
         objs = factory.simple_generate_batch(
             FakeModel,
             True,
             20,
             foo='bar',
             FACTORY_CLASS=factory.django.DjangoModelFactory,
@@ -2042,14 +2054,15 @@
 
     def __init__(self, **kwargs):
         for name, value in kwargs.items():
             setattr(self, name, value)
             self.id = None
 
 
+@unittest.skipIf(SKIP_DJANGO, "django tests disabled.")
 class DjangoModelFactoryTestCase(unittest.TestCase):
     def test_simple(self):
         class FakeModelFactory(factory.django.DjangoModelFactory):
             class Meta:
                 model = FakeModel
 
         obj = FakeModelFactory(one=1)
```

### Comparing `factory_boy-3.2.1/tests/test_utils.py` & `factory_boy-3.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/tests/utils.py` & `factory_boy-3.3.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `factory_boy-3.2.1/tox.ini` & `factory_boy-3.3.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,58 @@
 [tox]
 minversion = 1.9
 envlist =
     lint
-    py{36,37,38,39,py3}-django22-alchemy-mongoengine
-    py{36,37,38,39,py3}-django30-alchemy-mongoengine
-    py{36,37,38,39,py3}-django31-alchemy-mongoengine
-    py{36,37,38,39,py3}-django32-alchemy-mongoengine
-    py39-djangomaster-alchemy-mongoengine
     docs
     examples
     linkcheck
+    py{37,38,39,310,311,py37,py38,py39}-sqlite
+    py{37,38,39,310,311,py37,py38,py39}-django32-mongo-alchemy-{sqlite,postgres}
+    py{38,39,310,311,py38,py39}-django40-mongo-alchemy-{sqlite,postgres}
+    py{38,39,310,311,py38,py39}-django41-mongo-alchemy-{sqlite,postgres}
+    py310-djangomain-mongo-alchemy-{sqlite,postgres}
 
-toxworkdir = {env:TOX_WORKDIR:.tox}
+[gh-actions]
+python =
+    3.7: py37
+    3.8: py38
+    3.9: py39
+    3.10: py310
+    3.11: py311
+    pypy-3.7: pypy37
+    pypy-3.8: pypy38
+    pypy-3.9: pypy39
+
+[gh-actions:env]
+DATABASE_TYPE =
+    sqlite: sqlite
+    postgres: postgres
 
 [testenv]
+passenv =
+    MONGO_HOST
+    POSTGRES_HOST
+    POSTGRES_DATABASE
 deps =
-    django22: Django>=2.2,<2.3
-    django30: Django>=3.0,<3.1
-    django31: Django>=3.1,<3.2
-    django32: Django>=3.2,<3.3
-    djangomaster: https://github.com/django/django/archive/master.tar.gz
-    django{22,30,31,32,master}: Pillow
     alchemy: SQLAlchemy
-    mongoengine: mongoengine
+    alchemy: sqlalchemy_utils
+    mongo: mongoengine
+    django{32,40,41,main}: Pillow
+    django32: Django>=3.2,<3.3
+    django40: Django>=4.0,<4.1
+    django41: Django>=4.1,<4.2
+    djangomain: https://github.com/django/django/archive/main.tar.gz
+    py{37,38,39,310,311}-postgres: psycopg2-binary
+    pypy{37,38,39}-postgres: psycopg2cffi
 
-whitelist_externals = make
+setenv =
+    py: DJANGO_SETTINGS_MODULE=tests.djapp.settings
+    postgres: DJANGO_SETTINGS_MODULE=tests.djapp.settings_pg
+
+allowlist_externals = make
 commands = make test
 
 [testenv:docs]
 extras = doc
 
 whitelist_externals = make
 commands = make doc spelling
```

