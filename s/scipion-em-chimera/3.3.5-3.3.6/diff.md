# Comparing `tmp/scipion-em-chimera-3.3.5.tar.gz` & `tmp/scipion-em-chimera-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-chimera-3.3.5.tar", last modified: Fri Jan 13 12:30:17 2023, max compression
+gzip compressed data, was "scipion-em-chimera-3.3.6.tar", last modified: Wed Jul 19 07:47:44 2023, max compression
```

## Comparing `scipion-em-chimera-3.3.5.tar` & `scipion-em-chimera-3.3.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.901647 scipion-em-chimera-3.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/FAQ.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-01-13 12:30:17.901647 scipion-em-chimera-3.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.893647 scipion-em-chimera-3.3.5/chimera/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.893647 scipion-em-chimera-3.3.5/chimera/Bundles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.897647 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/bundle_info.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.897647 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.893647 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.893647 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.897647 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipion.html
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipioncombine.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipionrs.html
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipionshell.html
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipionshellcrown.html
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipionss.html
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipionwrite.html
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.897647 scipion-em-chimera-3.3.5/chimera/colabs/
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/colabs/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    37529 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/colabs/chimera_alphafold21_colab.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31585 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/colabs/chimera_alphafold_colab.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/colabs/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/colabs/down.py
--rw-r--r--   0 runner    (1001) docker     (123)    28433 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/colabs/kk.colab
--rw-r--r--   0 runner    (1001) docker     (123)    28445 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/colabs/kk.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/colabs/mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    24431 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/colabs/phenix_alphafold_colab.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/colabs/test_colab.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/editList.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/getchimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/parser_h1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.897647 scipion-em-chimera-3.3.5/chimera/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42124 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/protocols/protocol_alphafold.py
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/protocols/protocol_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/protocols/protocol_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    36801 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/protocols/protocol_modeller_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/protocols/protocol_operate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/protocols/protocol_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)    35621 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/protocols/protocol_subtraction_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.897647 scipion-em-chimera-3.3.5/chimera/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/tests/test_alpha_fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    21249 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/tests/test_protocol_chimera_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    49109 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/tests/test_protocol_chimera_map_subtraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/tests/test_protocol_chimera_operate.py
--rw-r--r--   0 runner    (1001) docker     (123)    38616 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/tests/test_protocol_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/tests/test_protocol_modeller_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.897647 scipion-em-chimera-3.3.5/chimera/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/viewers/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/viewers/viewer_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/chimera/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 12:30:17.901647 scipion-em-chimera-3.3.5/scipion_em_chimera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-01-13 12:30:17.000000 scipion-em-chimera-3.3.5/scipion_em_chimera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-01-13 12:30:17.000000 scipion-em-chimera-3.3.5/scipion_em_chimera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 12:30:17.000000 scipion-em-chimera-3.3.5/scipion_em_chimera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-13 12:30:17.000000 scipion-em-chimera-3.3.5/scipion_em_chimera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-13 12:30:17.000000 scipion-em-chimera-3.3.5/scipion_em_chimera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-13 12:30:17.000000 scipion-em-chimera-3.3.5/scipion_em_chimera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 12:30:17.901647 scipion-em-chimera-3.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-01-13 12:27:36.000000 scipion-em-chimera-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.131862 scipion-em-chimera-3.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/FAQ.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-19 07:47:44.131862 scipion-em-chimera-3.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.123861 scipion-em-chimera-3.3.6/chimera/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.119861 scipion-em-chimera-3.3.6/chimera/Bundles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.123861 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/bundle_info.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.127861 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.119861 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.119861 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.127861 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipion.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipioncombine.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipionrs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipionshell.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipionshellcrown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipionss.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipionwrite.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.127861 scipion-em-chimera-3.3.6/chimera/colabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/colabs/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37529 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/colabs/chimera_alphafold21_colab.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31585 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/colabs/chimera_alphafold_colab.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/colabs/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/colabs/down.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28433 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/colabs/kk.colab
+-rw-r--r--   0 runner    (1001) docker     (123)    28445 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/colabs/kk.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/colabs/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24431 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/colabs/phenix_alphafold_colab.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/colabs/test_colab.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/editList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/getchimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/parser_h1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.131862 scipion-em-chimera-3.3.6/chimera/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42124 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/protocols/protocol_alphafold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/protocols/protocol_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/protocols/protocol_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36801 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/protocols/protocol_modeller_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/protocols/protocol_operate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/protocols/protocol_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35621 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/protocols/protocol_subtraction_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.131862 scipion-em-chimera-3.3.6/chimera/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/tests/test_alpha_fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21249 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/tests/test_protocol_chimera_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49109 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/tests/test_protocol_chimera_map_subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/tests/test_protocol_chimera_operate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38616 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/tests/test_protocol_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/tests/test_protocol_modeller_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.131862 scipion-em-chimera-3.3.6/chimera/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/viewers/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/viewers/viewer_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/chimera/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 07:47:44.131862 scipion-em-chimera-3.3.6/scipion_em_chimera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-19 07:47:43.000000 scipion-em-chimera-3.3.6/scipion_em_chimera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-19 07:47:44.000000 scipion-em-chimera-3.3.6/scipion_em_chimera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 07:47:43.000000 scipion-em-chimera-3.3.6/scipion_em_chimera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-19 07:47:43.000000 scipion-em-chimera-3.3.6/scipion_em_chimera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 07:47:43.000000 scipion-em-chimera-3.3.6/scipion_em_chimera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 07:47:43.000000 scipion-em-chimera-3.3.6/scipion_em_chimera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 07:47:44.131862 scipion-em-chimera-3.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-19 07:45:50.000000 scipion-em-chimera-3.3.6/setup.py
```

### Comparing `scipion-em-chimera-3.3.5/CHANGES.txt` & `scipion-em-chimera-3.3.6/CHANGES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 Sep 18, 2020   - update to chimerax (from chimera)
 10-Nov-2020    - add scipioncpmbine
 11-Jan-2021    - change tml dir by extra since tmp is deleted as soon as the protocol ends
 27-April-2021  - add sonarcloud to github actions
  8-June-2021   - update tests with dinamic names that include the id of the protocol
 28-July-2021   - upddate to chimerax 1.2.5 (from chimera 1.1)
                - add command scipionshell that allow to visualice a virus shell by shell
+17-July-2023   - 3.3.6. Hot fix of tk-html-widgets package installation.
```

### Comparing `scipion-em-chimera-3.3.5/FAQ.rst` & `scipion-em-chimera-3.3.6/FAQ.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/LICENSE` & `scipion-em-chimera-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/PKG-INFO` & `scipion-em-chimera-3.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-chimera
-Version: 3.3.5
+Version: 3.3.6
 Summary: Plugin to use chimera programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-chimera
 Author: Marta Martinez, Roberto Marabini
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ======================
         Chimera scipion plugin
```

### Comparing `scipion-em-chimera-3.3.5/README.rst` & `scipion-em-chimera-3.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/Bundles/scipion/bundle_info.xml` & `scipion-em-chimera-3.3.6/chimera/Bundles/scipion/bundle_info.xml`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/api.py` & `scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/api.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/cmd.py` & `scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/cmd.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipion.html` & `scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipion.html`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipioncombine.html` & `scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipioncombine.html`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipionrs.html` & `scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipionrs.html`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipionshell.html` & `scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipionshell.html`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipionshellcrown.html` & `scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipionshellcrown.html`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipionss.html` & `scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipionss.html`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/Bundles/scipion/src/docs/user/commands/scipionwrite.html` & `scipion-em-chimera-3.3.6/chimera/Bundles/scipion/src/docs/user/commands/scipionwrite.html`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/__init__.py` & `scipion-em-chimera-3.3.6/chimera/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 import pwem
 import pyworkflow.utils as pwutils
 from glob import glob
 from .constants import (CHIMERA_HOME, ALPHAFOLD_HOME, ALPHAFOLD_DATABASE_DIR, 
                         V1_0, V1_1, V1_2_5, V1_3, V1_4, chimeraTARs)
 
-__version__ = "3.3.5"
+__version__ = "3.3.6"
 _logo = "chimerax_logo.png"
 _references = ['Goddard2018']
 
 
 class Plugin(pwem.Plugin):
     _homeVar = CHIMERA_HOME
     _pathVars = [CHIMERA_HOME]
@@ -122,17 +122,18 @@
         getchimera_script = os.path.join(os.path.dirname(__file__),
                                         "getchimera.py")
 
         extractionDir = finalDir = os.path.join("bin", "ChimeraX")
         if tarDir:
             extractionDir = os.path.join("..", tarDir, extractionDir)
 
-        chimera_cmds = [("cd .. && python %s %s" % (getchimera_script, version), "../ChimeraX-%s.tar.gz" %version),
-                        ("cd .. && tar -xf ChimeraX-%s.tar.gz" % version, extractionDir)
-                        ]
+        chimera_cmds = [
+            ("pip install https://github.com/scipion-em/tk_html_widgets/archive/master.zip", []),
+            ("cd .. && python %s %s" % (getchimera_script, version), "../ChimeraX-%s.tar.gz" %version),
+            ("cd .. && tar -xf ChimeraX-%s.tar.gz" % version, extractionDir)]
 
         if tarDir:
             chimera_cmds.append(("mv ../%s/* ." % tarDir,  finalDir))
 
         env.addPackage('chimerax', version=version,
                        tar=VOID_TGZ,
                        default=default,
```

### Comparing `scipion-em-chimera-3.3.5/chimera/bibtex.py` & `scipion-em-chimera-3.3.6/chimera/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/colabs/browser.py` & `scipion-em-chimera-3.3.6/chimera/colabs/browser.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/colabs/chimera_alphafold21_colab.ipynb` & `scipion-em-chimera-3.3.6/chimera/colabs/chimera_alphafold21_colab.ipynb`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/colabs/chimera_alphafold_colab.ipynb` & `scipion-em-chimera-3.3.6/chimera/colabs/chimera_alphafold_colab.ipynb`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/colabs/click.py` & `scipion-em-chimera-3.3.6/chimera/colabs/click.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/colabs/down.py` & `scipion-em-chimera-3.3.6/chimera/colabs/down.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/colabs/kk.colab` & `scipion-em-chimera-3.3.6/chimera/colabs/kk.colab`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/colabs/kk.ipynb` & `scipion-em-chimera-3.3.6/chimera/colabs/kk.ipynb`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/colabs/mouse.py` & `scipion-em-chimera-3.3.6/chimera/colabs/mouse.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/colabs/phenix_alphafold_colab.ipynb` & `scipion-em-chimera-3.3.6/chimera/colabs/phenix_alphafold_colab.ipynb`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/colabs/test_colab.ipynb` & `scipion-em-chimera-3.3.6/chimera/colabs/test_colab.ipynb`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/constants.py` & `scipion-em-chimera-3.3.6/chimera/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/convert.py` & `scipion-em-chimera-3.3.6/chimera/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/editList.py` & `scipion-em-chimera-3.3.6/chimera/editList.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/getchimera.py` & `scipion-em-chimera-3.3.6/chimera/getchimera.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/objects.py` & `scipion-em-chimera-3.3.6/chimera/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/parser_h1.py` & `scipion-em-chimera-3.3.6/chimera/parser_h1.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/protocols/__init__.py` & `scipion-em-chimera-3.3.6/chimera/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/protocols/protocol_alphafold.py` & `scipion-em-chimera-3.3.6/chimera/protocols/protocol_alphafold.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/protocols/protocol_base.py` & `scipion-em-chimera-3.3.6/chimera/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/protocols/protocol_contacts.py` & `scipion-em-chimera-3.3.6/chimera/protocols/protocol_contacts.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/protocols/protocol_fit.py` & `scipion-em-chimera-3.3.6/chimera/protocols/protocol_fit.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/protocols/protocol_modeller_search.py` & `scipion-em-chimera-3.3.6/chimera/protocols/protocol_modeller_search.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/protocols/protocol_operate.py` & `scipion-em-chimera-3.3.6/chimera/protocols/protocol_operate.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/protocols/protocol_restore.py` & `scipion-em-chimera-3.3.6/chimera/protocols/protocol_restore.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/protocols/protocol_subtraction_maps.py` & `scipion-em-chimera-3.3.6/chimera/protocols/protocol_subtraction_maps.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/protocols.conf` & `scipion-em-chimera-3.3.6/chimera/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/tests/__init__.py` & `scipion-em-chimera-3.3.6/chimera/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/tests/test_alpha_fold.py` & `scipion-em-chimera-3.3.6/chimera/tests/test_alpha_fold.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/tests/test_objects.py` & `scipion-em-chimera-3.3.6/chimera/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/tests/test_protocol_chimera_fit.py` & `scipion-em-chimera-3.3.6/chimera/tests/test_protocol_chimera_fit.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/tests/test_protocol_chimera_map_subtraction.py` & `scipion-em-chimera-3.3.6/chimera/tests/test_protocol_chimera_map_subtraction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/tests/test_protocol_chimera_operate.py` & `scipion-em-chimera-3.3.6/chimera/tests/test_protocol_chimera_operate.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/tests/test_protocol_contact.py` & `scipion-em-chimera-3.3.6/chimera/tests/test_protocol_contact.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/tests/test_protocol_modeller_search.py` & `scipion-em-chimera-3.3.6/chimera/tests/test_protocol_modeller_search.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/utils.py` & `scipion-em-chimera-3.3.6/chimera/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/viewers/viewer.py` & `scipion-em-chimera-3.3.6/chimera/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/viewers/viewer_contacts.py` & `scipion-em-chimera-3.3.6/chimera/viewers/viewer_contacts.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/chimera/wizards.py` & `scipion-em-chimera-3.3.6/chimera/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/scipion_em_chimera.egg-info/PKG-INFO` & `scipion-em-chimera-3.3.6/scipion_em_chimera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-chimera
-Version: 3.3.5
+Version: 3.3.6
 Summary: Plugin to use chimera programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-chimera
 Author: Marta Martinez, Roberto Marabini
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ======================
         Chimera scipion plugin
```

### Comparing `scipion-em-chimera-3.3.5/scipion_em_chimera.egg-info/SOURCES.txt` & `scipion-em-chimera-3.3.6/scipion_em_chimera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-chimera-3.3.5/setup.py` & `scipion-em-chimera-3.3.6/setup.py`

 * *Files identical despite different names*

