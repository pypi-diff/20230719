# Comparing `tmp/z3c.schema-1.2.0.tar.gz` & `tmp/z3c.schema-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.schema-1.2.0.tar", last modified: Mon Apr 11 05:59:31 2022, max compression
+gzip compressed data, was "z3c.schema-2.0.tar", last modified: Wed Jul 19 06:33:34 2023, max compression
```

## Comparing `z3c.schema-1.2.0.tar` & `z3c.schema-2.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.308285 z3c.schema-1.2.0/
--rw-r--r--   0 mac        (513) staff       (20)     1759 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      427 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     1773 2022-04-11 05:59:31.308403 z3c.schema-1.2.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      426 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      724 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)       75 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/doc-requirements.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.290789 z3c.schema-1.2.0/docs/
--rw-r--r--   0 mac        (513) staff       (20)     7618 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      160 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/baseurl.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)    10576 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      173 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/dateselect.rst
--rw-r--r--   0 mac        (513) staff       (20)      154 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/email.rst
--rw-r--r--   0 mac        (513) staff       (20)      163 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/hostname.rst
--rw-r--r--   0 mac        (513) staff       (20)      611 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)      145 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/ip.rst
--rw-r--r--   0 mac        (513) staff       (20)      166 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/optchoice.rst
--rw-r--r--   0 mac        (513) staff       (20)      163 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/payments.rst
--rw-r--r--   0 mac        (513) staff       (20)      154 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/docs/regex.rst
--rw-r--r--   0 mac        (513) staff       (20)      426 2022-04-11 05:59:31.308878 z3c.schema-1.2.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2742 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.278272 z3c.schema-1.2.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.291102 z3c.schema-1.2.0/src/z3c/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.294068 z3c.schema-1.2.0/src/z3c/schema/
--rw-r--r--   0 mac        (513) staff       (20)       85 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/README.txt
--rw-r--r--   0 mac        (513) staff       (20)      636 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.295644 z3c.schema-1.2.0/src/z3c/schema/baseurl/
--rw-r--r--   0 mac        (513) staff       (20)     1883 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/baseurl/README.txt
--rw-r--r--   0 mac        (513) staff       (20)      891 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/baseurl/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1487 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/baseurl/field.py
--rw-r--r--   0 mac        (513) staff       (20)     1071 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/baseurl/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     2265 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/baseurl/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.297230 z3c.schema-1.2.0/src/z3c/schema/dateselect/
--rw-r--r--   0 mac        (513) staff       (20)     1063 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/dateselect/README.txt
--rw-r--r--   0 mac        (513) staff       (20)      797 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/dateselect/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1175 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/dateselect/field.py
--rw-r--r--   0 mac        (513) staff       (20)      982 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/dateselect/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      795 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/dateselect/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.298702 z3c.schema-1.2.0/src/z3c/schema/email/
--rw-r--r--   0 mac        (513) staff       (20)     1711 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/email/README.txt
--rw-r--r--   0 mac        (513) staff       (20)      992 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/email/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2805 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/email/field.py
--rw-r--r--   0 mac        (513) staff       (20)      954 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/email/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      873 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/email/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.300194 z3c.schema-1.2.0/src/z3c/schema/hostname/
--rw-r--r--   0 mac        (513) staff       (20)     1463 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/hostname/README.txt
--rw-r--r--   0 mac        (513) staff       (20)      902 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/hostname/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1565 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/hostname/field.py
--rw-r--r--   0 mac        (513) staff       (20)     1022 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/hostname/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     2346 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/hostname/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.300744 z3c.schema-1.2.0/src/z3c/schema/i18n/
--rw-r--r--   0 mac        (513) staff       (20)      756 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/i18n/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      201 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/i18n/configure.zcml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.301013 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.280653 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/de/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.301291 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/de/LC_MESSAGES/
--rw-r--r--   0 mac        (513) staff       (20)     2029 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/de/LC_MESSAGES/z3c.schema.po
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.281204 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/fr/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.301560 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/fr/LC_MESSAGES/
--rw-r--r--   0 mac        (513) staff       (20)     2108 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/fr/LC_MESSAGES/z3c.schema.po
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.281681 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/nl/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.301827 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/nl/LC_MESSAGES/
--rw-r--r--   0 mac        (513) staff       (20)     2098 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/nl/LC_MESSAGES/z3c.schema.po
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.282142 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/ru/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.302094 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/ru/LC_MESSAGES/
--rw-r--r--   0 mac        (513) staff       (20)     2265 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/ru/LC_MESSAGES/z3c.schema.po
--rw-r--r--   0 mac        (513) staff       (20)     1802 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/i18n/locales/z3c.schema.pot
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.303466 z3c.schema-1.2.0/src/z3c/schema/ip/
--rw-r--r--   0 mac        (513) staff       (20)     1159 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/ip/README.txt
--rw-r--r--   0 mac        (513) staff       (20)      892 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/ip/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1519 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/ip/field.py
--rw-r--r--   0 mac        (513) staff       (20)      969 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/ip/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      873 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/ip/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.304975 z3c.schema-1.2.0/src/z3c/schema/optchoice/
--rw-r--r--   0 mac        (513) staff       (20)     1687 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/optchoice/README.txt
--rw-r--r--   0 mac        (513) staff       (20)      812 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/optchoice/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1656 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/optchoice/field.py
--rw-r--r--   0 mac        (513) staff       (20)     1624 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/optchoice/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      873 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/optchoice/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.306494 z3c.schema-1.2.0/src/z3c/schema/payments/
--rw-r--r--   0 mac        (513) staff       (20)     4850 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/payments/README.txt
--rw-r--r--   0 mac        (513) staff       (20)     1091 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/payments/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2133 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/payments/field.py
--rw-r--r--   0 mac        (513) staff       (20)     1013 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/payments/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      873 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/payments/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.308063 z3c.schema-1.2.0/src/z3c/schema/regex/
--rw-r--r--   0 mac        (513) staff       (20)      685 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/regex/README.txt
--rw-r--r--   0 mac        (513) staff       (20)      801 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/regex/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1260 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/regex/field.py
--rw-r--r--   0 mac        (513) staff       (20)      985 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/regex/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     1969 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/src/z3c/schema/regex/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-04-11 05:59:31.293436 z3c.schema-1.2.0/src/z3c.schema.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     1773 2022-04-11 05:59:30.000000 z3c.schema-1.2.0/src/z3c.schema.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     2378 2022-04-11 05:59:31.000000 z3c.schema-1.2.0/src/z3c.schema.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-04-11 05:59:30.000000 z3c.schema-1.2.0/src/z3c.schema.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        4 2022-04-11 05:59:30.000000 z3c.schema-1.2.0/src/z3c.schema.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-04-11 05:59:30.000000 z3c.schema-1.2.0/src/z3c.schema.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      159 2022-04-11 05:59:30.000000 z3c.schema-1.2.0/src/z3c.schema.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        4 2022-04-11 05:59:31.000000 z3c.schema-1.2.0/src/z3c.schema.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1381 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/tox.ini
--rw-r--r--   0 mac        (513) staff       (20)        6 2022-04-11 05:59:29.000000 z3c.schema-1.2.0/version.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.314383 z3c.schema-2.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1869 2023-07-19 06:33:33.000000 z3c.schema-2.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-19 06:33:33.000000 z3c.schema-2.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-19 06:33:33.000000 z3c.schema-2.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-19 06:33:33.000000 z3c.schema-2.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      427 2023-07-19 06:33:33.000000 z3c.schema-2.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1627 2023-07-19 06:33:34.314470 z3c.schema-2.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      426 2023-07-19 06:33:33.000000 z3c.schema-2.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      724 2023-07-19 06:33:33.000000 z3c.schema-2.0/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)       75 2023-07-19 06:33:33.000000 z3c.schema-2.0/doc-requirements.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.305656 z3c.schema-2.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7618 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)      160 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/baseurl.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/changelog.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10578 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      173 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/dateselect.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      154 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/email.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      163 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/hostname.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      611 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      145 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/ip.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      166 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/optchoice.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      163 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/payments.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      154 2023-07-19 06:33:33.000000 z3c.schema-2.0/docs/regex.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      699 2023-07-19 06:33:34.314736 z3c.schema-2.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2651 2023-07-19 06:33:33.000000 z3c.schema-2.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.300421 z3c.schema-2.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.305793 z3c.schema-2.0/src/z3c/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.307054 z3c.schema-2.0/src/z3c/schema/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       85 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/README.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      636 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.307770 z3c.schema-2.0/src/z3c/schema/baseurl/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1883 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/baseurl/README.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      932 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/baseurl/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1488 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/baseurl/field.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1071 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/baseurl/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2319 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/baseurl/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.308465 z3c.schema-2.0/src/z3c/schema/dateselect/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1063 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/dateselect/README.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      797 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/dateselect/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1159 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/dateselect/field.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      980 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/dateselect/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      795 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/dateselect/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.309168 z3c.schema-2.0/src/z3c/schema/email/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1711 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/email/README.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      992 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/email/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2783 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/email/field.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      954 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/email/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      873 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/email/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.309861 z3c.schema-2.0/src/z3c/schema/hostname/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1463 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/hostname/README.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      944 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/hostname/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1565 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/hostname/field.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1022 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/hostname/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2401 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/hostname/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.310151 z3c.schema-2.0/src/z3c/schema/i18n/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      757 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/i18n/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      201 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/i18n/configure.zcml
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.310298 z3c.schema-2.0/src/z3c/schema/i18n/locales/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.301217 z3c.schema-2.0/src/z3c/schema/i18n/locales/de/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.310439 z3c.schema-2.0/src/z3c/schema/i18n/locales/de/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2029 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/i18n/locales/de/LC_MESSAGES/z3c.schema.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.301369 z3c.schema-2.0/src/z3c/schema/i18n/locales/fr/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.310589 z3c.schema-2.0/src/z3c/schema/i18n/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2108 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/i18n/locales/fr/LC_MESSAGES/z3c.schema.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.301523 z3c.schema-2.0/src/z3c/schema/i18n/locales/nl/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.310729 z3c.schema-2.0/src/z3c/schema/i18n/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2098 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/i18n/locales/nl/LC_MESSAGES/z3c.schema.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.301683 z3c.schema-2.0/src/z3c/schema/i18n/locales/ru/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.310867 z3c.schema-2.0/src/z3c/schema/i18n/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2265 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/i18n/locales/ru/LC_MESSAGES/z3c.schema.po
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1802 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/i18n/locales/z3c.schema.pot
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.311561 z3c.schema-2.0/src/z3c/schema/ip/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1159 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/ip/README.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      928 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/ip/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1504 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/ip/field.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      969 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/ip/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      873 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/ip/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.312389 z3c.schema-2.0/src/z3c/schema/optchoice/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1687 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/optchoice/README.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      812 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/optchoice/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1630 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/optchoice/field.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1623 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/optchoice/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      873 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/optchoice/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.313216 z3c.schema-2.0/src/z3c/schema/payments/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4850 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/payments/README.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1092 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/payments/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2111 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/payments/field.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1013 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/payments/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      873 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/payments/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.314202 z3c.schema-2.0/src/z3c/schema/regex/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      685 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/regex/README.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      840 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/regex/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1256 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/regex/field.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      985 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/regex/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1993 2023-07-19 06:33:33.000000 z3c.schema-2.0/src/z3c/schema/regex/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:33:34.306783 z3c.schema-2.0/src/z3c.schema.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1627 2023-07-19 06:33:34.000000 z3c.schema-2.0/src/z3c.schema.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2378 2023-07-19 06:33:34.000000 z3c.schema-2.0/src/z3c.schema.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-19 06:33:34.000000 z3c.schema-2.0/src/z3c.schema.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-07-19 06:33:34.000000 z3c.schema-2.0/src/z3c.schema.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-19 06:33:34.000000 z3c.schema-2.0/src/z3c.schema.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      159 2023-07-19 06:33:34.000000 z3c.schema-2.0/src/z3c.schema.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-07-19 06:33:34.000000 z3c.schema-2.0/src/z3c.schema.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1610 2023-07-19 06:33:33.000000 z3c.schema-2.0/tox.ini
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-07-19 06:33:33.000000 z3c.schema-2.0/version.txt
```

### Comparing `z3c.schema-1.2.0/CHANGES.rst` & `z3c.schema-2.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =======
 CHANGES
 =======
 
+2.0 (2023-07-19)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 1.2.0 (2022-04-11)
 ------------------
 
 - Add support for Python 3.6, 3.7, 3.8, 3.9, 3.10, PyPy3.
 
 - Drop support for Python 3.3 and 3.4.
```

### Comparing `z3c.schema-1.2.0/CONTRIBUTING.md` & `z3c.schema-2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/LICENSE.txt` & `z3c.schema-2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/PKG-INFO` & `z3c.schema-2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: z3c.schema
-Version: 1.2.0
+Version: 2.0
 Summary: Additional schema fields for Zope 3
 Home-page: https://github.com/zopefoundation/z3c.schema
 Author: Zope Community
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope zope3 z3c schema
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 This package provides different additional Zope 3 schema fields.
 
 The provided fields include support for:
@@ -45,9 +42,7 @@
 - Optional choices
 
 Complete documentation can be found at https://z3cschema.readthedocs.io.
 
 The `full change log <https://z3cschema.readthedocs.io/en/latest/changelog.html>`_ is available.
 
 
-
-
```

### Comparing `z3c.schema-1.2.0/buildout.cfg` & `z3c.schema-2.0/buildout.cfg`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/docs/Makefile` & `z3c.schema-2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/docs/conf.py` & `z3c.schema-2.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,14 +349,14 @@
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     'https://docs.python.org/': None,
     'http://zopeschema.readthedocs.io/en/latest/': None,
 }
 
 extlinks = {'issue': ('https://github.com/zopefoundation/z3c.schema/issues/%s',
-                      'issue #'),
+                      'issue %s'),
             'pr': ('https://github.com/zopefoundation/z3c.schema/pull/%s',
-                   'pull request #')}
+                   'pull request %s')}
 
 autodoc_default_flags = ['members', 'show-inheritance']
 autoclass_content = 'both'
 autodoc_member_order = 'bysource'
```

### Comparing `z3c.schema-1.2.0/docs/index.rst` & `z3c.schema-2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/setup.py` & `z3c.schema-2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,61 +10,61 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Setup
 """
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         text = f.read()
     return text + '\n\n'
 
 
 setup(
     name='z3c.schema',
     version=read('version.txt').strip(),
     author='Zope Community',
-    author_email="zope-dev@zope.org",
+    author_email="zope-dev@zope.dev",
     description="Additional schema fields for Zope 3",
     long_description=(
         read('README.rst')
     ),
     license='ZPL 2.1',
     keywords='zope zope3 z3c schema',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP',
-        'Framework :: Zope :: 3'
+        'Framework :: Zope :: 3',
     ],
     url='https://github.com/zopefoundation/z3c.schema',
     packages=find_packages('src'),
     include_package_data=True,
     package_dir={'': 'src'},
     namespace_packages=['z3c', ],
+    python_requires='>=3.7',
     extras_require=dict(
         test=[
             'zope.testing',
             'zope.testrunner',
         ],
         docs=[
             'Sphinx',
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/__init__.py` & `z3c.schema-2.0/src/z3c/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/baseurl/README.txt` & `z3c.schema-2.0/src/z3c/schema/baseurl/README.txt`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/baseurl/__init__.py` & `z3c.schema-2.0/src/z3c/schema/baseurl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from z3c.schema.baseurl.interfaces import IBaseURL, InvalidBaseURL
-from z3c.schema.baseurl.field import isValidBaseURL
 from z3c.schema.baseurl.field import BaseURL
+from z3c.schema.baseurl.field import isValidBaseURL
+from z3c.schema.baseurl.interfaces import IBaseURL
+from z3c.schema.baseurl.interfaces import InvalidBaseURL
 
 
 __all__ = [
     'IBaseURL',
     'InvalidBaseURL',
     'isValidBaseURL',
     'BaseURL',
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/baseurl/field.py` & `z3c.schema-2.0/src/z3c/schema/baseurl/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import re
 
 import zope.interface
 import zope.schema
 
 from z3c.schema.baseurl import interfaces
 
+
 #: Determine whether the URL is a base URL.
 isValidBaseURL = re.compile(
     r"[a-zA-Z0-9+.-]+:"   # scheme
     r"\S*$"               # non space (should be pickier)
 ).match
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/baseurl/interfaces.py` & `z3c.schema-2.0/src/z3c/schema/baseurl/interfaces.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/baseurl/tests.py` & `z3c.schema-2.0/src/z3c/schema/baseurl/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,50 +11,52 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Base URL Field
 """
 import doctest
 import unittest
+
 from zope.schema.interfaces import RequiredMissing
 
-from z3c.schema.baseurl import BaseURL, InvalidBaseURL
+from z3c.schema.baseurl import BaseURL
+from z3c.schema.baseurl import InvalidBaseURL
 
 
 class BaseURLTest(unittest.TestCase):
 
     _Field_Factory = BaseURL
     _convert = str
 
     def testValidate(self):
-        field = self._Field_Factory(title=u'BaseURL field', description=u'',
+        field = self._Field_Factory(title='BaseURL field', description='',
                                     readonly=False, required=False)
         field.validate(None)
         field.validate(self._convert('host:123.123.123.123/'))
         field.validate(self._convert('host:123/'))
         field.validate(self._convert('http://www.host.com:123/'))
         field.validate(self._convert('http://123.123.123.123:123/'))
 
     def testValidateRequired(self):
-        field = self._Field_Factory(title=u'BaseURL field', description=u'',
+        field = self._Field_Factory(title='BaseURL field', description='',
                                     readonly=False, required=True)
         self.assertRaises(RequiredMissing, field.validate, None)
 
     def testBadStringType(self):
-        field = self._Field_Factory(title=u'BaseURL field')
-        self.assertRaises(InvalidBaseURL, field.validate, u'123.123')
+        field = self._Field_Factory(title='BaseURL field')
+        self.assertRaises(InvalidBaseURL, field.validate, '123.123')
 
     def test_newlines(self):
-        field = self._Field_Factory(title=u'BaseURL field')
+        field = self._Field_Factory(title='BaseURL field')
         self.assertRaises(InvalidBaseURL, field.validate,
                           self._convert('host\nfoo'))
 
 
 def test_suite():
     return unittest.TestSuite((
         doctest.DocFileSuite(
             'README.txt',
             optionflags=(doctest.NORMALIZE_WHITESPACE
                          | doctest.ELLIPSIS
                          | doctest.IGNORE_EXCEPTION_DETAIL)),
-        unittest.makeSuite(BaseURLTest),
+        unittest.defaultTestLoader.loadTestsFromTestCase(BaseURLTest),
     ))
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/dateselect/README.txt` & `z3c.schema-2.0/src/z3c/schema/dateselect/README.txt`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/dateselect/__init__.py` & `z3c.schema-2.0/src/z3c/schema/dateselect/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from z3c.schema.dateselect.interfaces import IDateSelect
 from z3c.schema.dateselect.field import DateSelect
+from z3c.schema.dateselect.interfaces import IDateSelect
 
 
 __all__ = [
     'IDateSelect',
     'DateSelect',
 ]
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/dateselect/field.py` & `z3c.schema-2.0/src/z3c/schema/dateselect/field.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 @zope.interface.implementer(interfaces.IDateSelect)
 class DateSelect(zope.schema.Date):
 
     yearRange = list(range(1900, 2100))
     initialDate = None  # set a date or today is used
 
     def __init__(self, yearRange=None, initialDate=None, **kw):
-        super(DateSelect, self).__init__(**kw)
+        super().__init__(**kw)
         self.initialDate = initialDate
         if yearRange is not None:
             self.yearRange = yearRange
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/dateselect/interfaces.py` & `z3c.schema-2.0/src/z3c/schema/dateselect/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 __docformat__ = "reStructuredText"
 
 import zope.schema.interfaces
 
 
 class IDateSelect(zope.schema.interfaces.IDate):
 
-    yearRange = zope.interface.Attribute(u"Year range.")
+    yearRange = zope.interface.Attribute("Year range.")
 
     initialDate = zope.interface.Attribute(
-        u"Initial date displayed or ``None``. If ``None``, `today()`` is used."
+        "Initial date displayed or ``None``. If ``None``, `today()`` is used."
     )
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/dateselect/tests.py` & `z3c.schema-2.0/src/z3c/schema/dateselect/tests.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/email/README.txt` & `z3c.schema-2.0/src/z3c/schema/email/README.txt`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/email/__init__.py` & `z3c.schema-2.0/src/z3c/schema/email/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
+from z3c.schema.email.field import RFC822MailAddress
+from z3c.schema.email.field import isValidMailAddress
 from z3c.schema.email.interfaces import IRFC822MailAddress
 from z3c.schema.email.interfaces import NotValidRFC822MailAdress
-from z3c.schema.email.field import isValidMailAddress
-from z3c.schema.email.field import RFC822MailAddress
 
 
 __all__ = [
     'IRFC822MailAddress',
     'NotValidRFC822MailAdress',
     'isValidMailAddress',
     'RFC822MailAddress',
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/email/field.py` & `z3c.schema-2.0/src/z3c/schema/email/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 __docformat__ = "reStructuredText"
 
 import zope.interface
 import zope.schema
 
 from z3c.schema.email import interfaces
 
+
 rfc822_specials = '()<>@,;:\\"[]'
 
 
 def isValidMailAddress(addr):
     """Returns True if the email address is valid and False if not."""
 
     # First we validate the name portion (name@domain)
@@ -78,10 +79,10 @@
 class RFC822MailAddress(zope.schema.TextLine):
     """A valid email address."""
 
     def constraint(self, value):
         return '\n' not in value and '\r' not in value
 
     def _validate(self, value):
-        super(RFC822MailAddress, self)._validate(value)
+        super()._validate(value)
         if not isValidMailAddress(value):
             raise interfaces.NotValidRFC822MailAdress(value)
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/email/interfaces.py` & `z3c.schema-2.0/src/z3c/schema/email/interfaces.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/email/tests.py` & `z3c.schema-2.0/src/z3c/schema/email/tests.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/hostname/README.txt` & `z3c.schema-2.0/src/z3c/schema/hostname/README.txt`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/hostname/__init__.py` & `z3c.schema-2.0/src/z3c/schema/hostname/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from z3c.schema.hostname.interfaces import IHostName, InvalidHostName
-from z3c.schema.hostname.field import isValidHostName
 from z3c.schema.hostname.field import HostName
+from z3c.schema.hostname.field import isValidHostName
+from z3c.schema.hostname.interfaces import IHostName
+from z3c.schema.hostname.interfaces import InvalidHostName
 
 
 __all__ = [
     'IHostName',
     'InvalidHostName',
     'isValidHostName',
     'HostName',
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/hostname/field.py` & `z3c.schema-2.0/src/z3c/schema/hostname/field.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/hostname/interfaces.py` & `z3c.schema-2.0/src/z3c/schema/hostname/interfaces.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/hostname/tests.py` & `z3c.schema-2.0/src/z3c/schema/hostname/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,52 +11,54 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Hostname Field
 """
 import doctest
 import unittest
+
 from zope.schema.interfaces import RequiredMissing
 
-from z3c.schema.hostname import HostName, InvalidHostName
+from z3c.schema.hostname import HostName
+from z3c.schema.hostname import InvalidHostName
 
 
 class HostNameTest(unittest.TestCase):
 
     _Field_Factory = HostName
     _convert = str
 
     def testValidate(self):
-        field = self._Field_Factory(title=u'HostName field', description=u'',
+        field = self._Field_Factory(title='HostName field', description='',
                                     readonly=False, required=False)
         field.validate(None)
         field.validate(self._convert('host'))
         field.validate(self._convert('123.123.123.123'))
         field.validate(self._convert('host:123'))
         field.validate(self._convert('www.host.com:123'))
         field.validate(self._convert('123.123.123.123:123'))
 
     def testValidateRequired(self):
-        field = self._Field_Factory(title=u'HostName field', description=u'',
+        field = self._Field_Factory(title='HostName field', description='',
                                     readonly=False, required=True)
         field.validate(self._convert('host'))
         self.assertRaises(RequiredMissing, field.validate, None)
 
     def testBadStringType(self):
-        field = self._Field_Factory(title=u'HostName field')
-        self.assertRaises(InvalidHostName, field.validate, u'123.123')
+        field = self._Field_Factory(title='HostName field')
+        self.assertRaises(InvalidHostName, field.validate, '123.123')
 
     def test_newlines(self):
-        field = self._Field_Factory(title=u'HostName field')
+        field = self._Field_Factory(title='HostName field')
         self.assertRaises(InvalidHostName, field.validate,
                           self._convert('host\nfoo'))
 
 
 def test_suite():
     return unittest.TestSuite((
         doctest.DocFileSuite(
             'README.txt',
             optionflags=(doctest.NORMALIZE_WHITESPACE
                          | doctest.ELLIPSIS
                          | doctest.IGNORE_EXCEPTION_DETAIL)),
-        unittest.makeSuite(HostNameTest),
+        unittest.defaultTestLoader.loadTestsFromTestCase(HostNameTest),
     ))
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/i18n/__init__.py` & `z3c.schema-2.0/src/z3c/schema/regex/interfaces.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 ##############################################################################
 #
-# Copyright (c) 2005 Zope Foundation and Contributors.
+# Copyright (c) 2006 Zope Foundation and Contributors.
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-"""I18n utils for zope3."""
-import zope.i18nmessageid
+"""
+"""
+__docformat__ = "reStructuredText"
 
-MessageFactory = zope.i18nmessageid.MessageFactory('z3c.schema')
+import zope.schema
+import zope.schema.interfaces
+
+from z3c.schema.i18n import MessageFactory as _
+
+
+class IRegex(zope.schema.interfaces.IASCIILine):
+    """Regular Expression field"""
+
+
+class InvalidRegex(zope.schema.ValidationError):
+    __doc__ = _("""The specified regular expression is not valid.""")
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/i18n/locales/de/LC_MESSAGES/z3c.schema.po` & `z3c.schema-2.0/src/z3c/schema/i18n/locales/de/LC_MESSAGES/z3c.schema.po`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/i18n/locales/fr/LC_MESSAGES/z3c.schema.po` & `z3c.schema-2.0/src/z3c/schema/i18n/locales/fr/LC_MESSAGES/z3c.schema.po`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/i18n/locales/nl/LC_MESSAGES/z3c.schema.po` & `z3c.schema-2.0/src/z3c/schema/i18n/locales/nl/LC_MESSAGES/z3c.schema.po`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/i18n/locales/ru/LC_MESSAGES/z3c.schema.po` & `z3c.schema-2.0/src/z3c/schema/i18n/locales/ru/LC_MESSAGES/z3c.schema.po`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/i18n/locales/z3c.schema.pot` & `z3c.schema-2.0/src/z3c/schema/i18n/locales/z3c.schema.pot`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/ip/README.txt` & `z3c.schema-2.0/src/z3c/schema/ip/README.txt`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/ip/__init__.py` & `z3c.schema-2.0/src/z3c/schema/ip/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from z3c.schema.ip.interfaces import IIPAddress, NotValidIPAdress
-from z3c.schema.ip.field import isValidIPAddress
 from z3c.schema.ip.field import IPAddress
+from z3c.schema.ip.field import isValidIPAddress
+from z3c.schema.ip.interfaces import IIPAddress
+from z3c.schema.ip.interfaces import NotValidIPAdress
 
 
 __all__ = [
     'IIPAddress',
     'NotValidIPAdress',
     'isValidIPAddress',
     'IPAddress',
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/ip/field.py` & `z3c.schema-2.0/src/z3c/schema/ip/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,11 +37,11 @@
 
 
 @zope.interface.implementer(interfaces.IIPAddress)
 class IPAddress(zope.schema.NativeStringLine):
     """A valid IP address."""
 
     def _validate(self, value):
-        super(IPAddress, self)._validate(value)
+        super()._validate(value)
 
         if not isValidIPAddress(value):
             raise interfaces.NotValidIPAdress(value)
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/ip/interfaces.py` & `z3c.schema-2.0/src/z3c/schema/ip/interfaces.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/ip/tests.py` & `z3c.schema-2.0/src/z3c/schema/ip/tests.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/optchoice/README.txt` & `z3c.schema-2.0/src/z3c/schema/optchoice/README.txt`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/optchoice/__init__.py` & `z3c.schema-2.0/src/z3c/schema/optchoice/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from z3c.schema.optchoice.interfaces import IOptionalChoice
 from z3c.schema.optchoice.field import OptionalChoice
+from z3c.schema.optchoice.interfaces import IOptionalChoice
 
 
 __all__ = [
 
     'IOptionalChoice',
     'OptionalChoice',
 ]
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/optchoice/field.py` & `z3c.schema-2.0/src/z3c/schema/optchoice/field.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,34 +13,35 @@
 ##############################################################################
 """
 """
 __docformat__ = "reStructuredText"
 
 import zope.interface
 import zope.schema
-from zope.schema.interfaces import IField, ValidationError
+from zope.schema.interfaces import IField
+from zope.schema.interfaces import ValidationError
 
 from z3c.schema.optchoice import interfaces
 
 
 @zope.interface.implementer(interfaces.IOptionalChoice)
 class OptionalChoice(zope.schema.Choice):
     """Optional Choice field."""
 
     def __init__(self, value_type, **kw):
-        super(OptionalChoice, self).__init__(**kw)
+        super().__init__(**kw)
         # whine if value_type is not a field
         if value_type is not None and not IField.providedBy(value_type):
             raise ValueError("'value_type' must be field instance.")
         self.value_type = value_type
 
     def _validate(self, value):
         try:
-            super(OptionalChoice, self)._validate(value)
+            super()._validate(value)
         except ValidationError:
             self.value_type._validate(value)
 
     def fromUnicode(self, value):
         try:
-            return super(OptionalChoice, self).fromUnicode(value)
+            return super().fromUnicode(value)
         except ValidationError:
             return self.value_type.fromUnicode(value)
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/optchoice/interfaces.py` & `z3c.schema-2.0/src/z3c/schema/optchoice/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,9 +41,9 @@
 
     2. If no match was made, call the unicode conversion method of the
        ``value_type`` field.
     """
 
     value_type = zope.schema.Field(
         title=_("Value Type"),
-        description=_(u"The freely entered values must be of this type."),
+        description=_("The freely entered values must be of this type."),
         required=True)
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/optchoice/tests.py` & `z3c.schema-2.0/src/z3c/schema/optchoice/tests.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/payments/README.txt` & `z3c.schema-2.0/src/z3c/schema/payments/README.txt`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/payments/__init__.py` & `z3c.schema-2.0/src/z3c/schema/payments/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from z3c.schema.payments.interfaces import IISO7812CreditCard
-from z3c.schema.payments.interfaces import NotValidISO7812CreditCard
-from z3c.schema.payments.field import isValidCreditCard
 from z3c.schema.payments.field import ISO7812CreditCard
 from z3c.schema.payments.field import ISO7812CreditCard as CreditCard
+from z3c.schema.payments.field import isValidCreditCard
+from z3c.schema.payments.interfaces import IISO7812CreditCard
+from z3c.schema.payments.interfaces import NotValidISO7812CreditCard
+
 
 __all__ = [
     'IISO7812CreditCard',
     'NotValidISO7812CreditCard',
     'isValidCreditCard',
     'ISO7812CreditCard',
     'CreditCard',
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/payments/field.py` & `z3c.schema-2.0/src/z3c/schema/payments/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """
 """
 import zope.interface
+
 from . import interfaces
 
 
 def isValidCreditCard(cardNum):
     """Returns True if the credit card number is a valid Luhn (Mod 10) number
        and False if not. This, of course, does not validate the number, but
        will catch typos. There is the chance that two typographic errors could
@@ -51,10 +52,10 @@
         allDigits = True
         for char in value[:]:
             if not char.isdigit():
                 allDigits = False
         return '\n' not in value and '\r' not in value and allDigits
 
     def _validate(self, value):
-        super(ISO7812CreditCard, self)._validate(value)
+        super()._validate(value)
         if not isValidCreditCard(value):
             raise interfaces.NotValidISO7812CreditCard(value)
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/payments/interfaces.py` & `z3c.schema-2.0/src/z3c/schema/payments/interfaces.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/payments/tests.py` & `z3c.schema-2.0/src/z3c/schema/payments/tests.py`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/regex/README.txt` & `z3c.schema-2.0/src/z3c/schema/regex/README.txt`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/src/z3c/schema/regex/__init__.py` & `z3c.schema-2.0/src/z3c/schema/regex/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from z3c.schema.regex.interfaces import IRegex, InvalidRegex
 from z3c.schema.regex.field import Regex
+from z3c.schema.regex.interfaces import InvalidRegex
+from z3c.schema.regex.interfaces import IRegex
 
 
 __all__ = [
     'IRegex',
     'InvalidRegex',
     'Regex',
 ]
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/regex/field.py` & `z3c.schema-2.0/src/z3c/schema/regex/field.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,31 +12,32 @@
 #
 ##############################################################################
 """
 """
 __docformat__ = "reStructuredText"
 
 import re
+
 import zope.interface
 import zope.schema
 
 from z3c.schema.regex import interfaces
 
 
 @zope.interface.implementer(interfaces.IRegex)
 class Regex(zope.schema.ASCIILine):
     """Regex schema field.
 
     Must be a compilable regular expression
     """
 
     def _validate(self, value):
-        super(Regex, self)._validate(value)
+        super()._validate(value)
         try:
             re.compile(value)
         except re.error as e:
-            raise interfaces.InvalidRegex('%r, %s' % (value, e))
+            raise interfaces.InvalidRegex('{!r}, {}'.format(value, e))
 
     def fromUnicode(self, value):
         v = str(value.strip())
         self.validate(v)
         return v
```

### Comparing `z3c.schema-1.2.0/src/z3c/schema/regex/tests.py` & `z3c.schema-2.0/src/z3c/schema/regex/tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 ###############################################################################
 #
 # Copyright 2006 by refline (Schweiz) AG, CH-5630 Muri
 #
 ###############################################################################
 """Refline Recruiter Tests
 """
-from zope.schema.interfaces import RequiredMissing
 import doctest
 import unittest
 
+from zope.schema.interfaces import RequiredMissing
+
 from z3c.schema.hostname import HostName
 from z3c.schema.hostname import InvalidHostName
 
 
 class HostNameTest(unittest.TestCase):
 
     _Field_Factory = HostName
     _convert = str
 
     def testValidate(self):
-        field = self._Field_Factory(title=u'HostName field', description=u'',
+        field = self._Field_Factory(title='HostName field', description='',
                                     readonly=False, required=False)
         field.validate(None)
         field.validate(self._convert('host'))
         field.validate(self._convert('123.123.123.123'))
         field.validate(self._convert('host:123'))
         field.validate(self._convert('www.host.com:123'))
         field.validate(self._convert('123.123.123.123:123'))
 
     def testValidateRequired(self):
-        field = self._Field_Factory(title=u'HostName field', description=u'',
+        field = self._Field_Factory(title='HostName field', description='',
                                     readonly=False, required=True)
         field.validate(self._convert('host'))
         self.assertRaises(RequiredMissing, field.validate, None)
 
     def testBadStringType(self):
-        field = self._Field_Factory(title=u'HostName field')
-        self.assertRaises(InvalidHostName, field.validate, u'123.123')
+        field = self._Field_Factory(title='HostName field')
+        self.assertRaises(InvalidHostName, field.validate, '123.123')
 
     def test_newlines(self):
-        field = self._Field_Factory(title=u'HostName field')
+        field = self._Field_Factory(title='HostName field')
         self.assertRaises(InvalidHostName, field.validate,
                           self._convert('host\nfoo'))
 
 
 def test_suite():
     return unittest.TestSuite((
         doctest.DocFileSuite(
             'README.txt',
             optionflags=(doctest.NORMALIZE_WHITESPACE
                          | doctest.ELLIPSIS
                          | doctest.IGNORE_EXCEPTION_DETAIL)),
-        unittest.makeSuite(HostNameTest),
+        unittest.defaultTestLoader.loadTestsFromTestCase(HostNameTest),
     ))
```

### Comparing `z3c.schema-1.2.0/src/z3c.schema.egg-info/PKG-INFO` & `z3c.schema-2.0/src/z3c.schema.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: z3c.schema
-Version: 1.2.0
+Version: 2.0
 Summary: Additional schema fields for Zope 3
 Home-page: https://github.com/zopefoundation/z3c.schema
 Author: Zope Community
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope zope3 z3c schema
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 This package provides different additional Zope 3 schema fields.
 
 The provided fields include support for:
@@ -45,9 +42,7 @@
 - Optional choices
 
 Complete documentation can be found at https://z3cschema.readthedocs.io.
 
 The `full change log <https://z3cschema.readthedocs.io/en/latest/changelog.html>`_ is available.
 
 
-
-
```

### Comparing `z3c.schema-1.2.0/src/z3c.schema.egg-info/SOURCES.txt` & `z3c.schema-2.0/src/z3c.schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `z3c.schema-1.2.0/tox.ini` & `z3c.schema-2.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
-    pypy
+    py311
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
+package = wheel
+wheel_build_env = .pkg
 deps =
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
+    check-manifest
+    check-python-versions
 deps =
-    flake8
     check-manifest
     check-python-versions >= 0.19.1
     wheel
+    flake8
+    isort
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
 commands =
-    flake8 src setup.py
-    check-manifest
-    check-python-versions
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
 basepython = python3
 skip_install = false
 extras =
     docs
 commands_pre =
@@ -48,24 +58,22 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=99
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=99
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = z3c.schema
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

