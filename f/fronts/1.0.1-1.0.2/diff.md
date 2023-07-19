# Comparing `tmp/fronts-1.0.1.tar.gz` & `tmp/fronts-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fronts-1.0.1.tar", last modified: Fri Feb 24 14:13:19 2023, max compression
+gzip compressed data, was "fronts-1.0.2.tar", last modified: Wed Jul 19 00:59:49 2023, max compression
```

## Comparing `fronts-1.0.1.tar` & `fronts-1.0.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.554664 fronts-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-24 14:12:55.000000 fronts-1.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-02-24 14:12:55.000000 fronts-1.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-02-24 14:12:55.000000 fronts-1.0.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-02-24 14:12:55.000000 fronts-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-24 14:12:55.000000 fronts-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-02-24 14:13:19.554664 fronts-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-02-24 14:12:55.000000 fronts-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.550664 fronts-1.0.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-24 14:12:55.000000 fronts-1.0.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-02-24 14:12:55.000000 fronts-1.0.1/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.550664 fronts-1.0.1/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-02-24 14:12:55.000000 fronts-1.0.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-02-24 14:12:55.000000 fronts-1.0.1/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.550664 fronts-1.0.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.550664 fronts-1.0.1/examples/1INFILTR/
--rwxr-xr-x   0 runner    (1001) docker     (123)      729 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/1INFILTR/D.py
--rw-r--r--   0 runner    (1001) docker     (123)   567061 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/1INFILTR/Nod_Inf.out
--rwxr-xr-x   0 runner    (1001) docker     (123)     1403 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/1INFILTR/solve.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2196 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/1INFILTR/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.550664 fronts-1.0.1/examples/HF135/
--rwxr-xr-x   0 runner    (1001) docker     (123)      904 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/HF135/D.py
--rw-r--r--   0 runner    (1001) docker     (123)    32297 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/HF135/groundwaterFoam_results.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     1994 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/HF135/inverse1.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/HF135/inverse2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1893 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/HF135/radial.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2498 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/HF135/refine.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/HF135/solve.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/HF135/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.550664 fronts-1.0.1/examples/exact/
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/exact/D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      685 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/exact/fromguess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/exact/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.550664 fronts-1.0.1/examples/powerlaw/
--rwxr-xr-x   0 runner    (1001) docker     (123)      393 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/powerlaw/D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1341 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/powerlaw/inverse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-02-24 14:12:55.000000 fronts-1.0.1/examples/powerlaw/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.554664 fronts-1.0.1/fronts/
--rw-r--r--   0 runner    (1001) docker     (123)    33379 2023-02-24 14:12:55.000000 fronts-1.0.1/fronts/D.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-24 14:12:55.000000 fronts-1.0.1/fronts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-02-24 14:12:55.000000 fronts-1.0.1/fronts/_boltzmann.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-02-24 14:12:55.000000 fronts-1.0.1/fronts/_rootfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    49649 2023-02-24 14:12:55.000000 fronts-1.0.1/fronts/_semiinfinite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.554664 fronts-1.0.1/fronts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-02-24 14:13:19.000000 fronts-1.0.1/fronts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-02-24 14:13:19.000000 fronts-1.0.1/fronts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 14:13:19.000000 fronts-1.0.1/fronts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-24 14:13:19.000000 fronts-1.0.1/fronts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-24 14:13:19.000000 fronts-1.0.1/fronts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-24 14:12:55.000000 fronts-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.554664 fronts-1.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-02-24 14:12:55.000000 fronts-1.0.1/resources/CIMEC.png
--rw-r--r--   0 runner    (1001) docker     (123)   174760 2023-02-24 14:12:55.000000 fronts-1.0.1/resources/GSaMLogo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-02-24 14:12:55.000000 fronts-1.0.1/resources/INTEC.png
--rw-r--r--   0 runner    (1001) docker     (123)    24144 2023-02-24 14:12:55.000000 fronts-1.0.1/resources/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    34790 2023-02-24 14:12:55.000000 fronts-1.0.1/resources/powerlaw_c.png
--rw-r--r--   0 runner    (1001) docker     (123)    44856 2023-02-24 14:12:55.000000 fronts-1.0.1/resources/powerlaw_flux.png
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-02-24 14:13:19.558664 fronts-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-24 14:12:55.000000 fronts-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.554664 fronts-1.0.1/symbolic/
--rwxr-xr-x   0 runner    (1001) docker     (123)      912 2023-02-24 14:12:55.000000 fronts-1.0.1/symbolic/brooks_and_corey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-02-24 14:12:55.000000 fronts-1.0.1/symbolic/generate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      699 2023-02-24 14:12:55.000000 fronts-1.0.1/symbolic/letd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2023-02-24 14:12:55.000000 fronts-1.0.1/symbolic/letxs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-02-24 14:12:55.000000 fronts-1.0.1/symbolic/ode_jac.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      892 2023-02-24 14:12:55.000000 fronts-1.0.1/symbolic/van_genuchten.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.554664 fronts-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-24 14:12:55.000000 fronts-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-02-24 14:12:55.000000 fronts-1.0.1/tests/test_D.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-24 14:12:55.000000 fronts-1.0.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-24 14:12:55.000000 fronts-1.0.1/tests/test_inverse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:13:19.554664 fronts-1.0.1/tests/test_rootfinding/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-02-24 14:12:55.000000 fronts-1.0.1/tests/test_rootfinding/checkobj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-02-24 14:12:55.000000 fronts-1.0.1/tests/test_rootfinding/test_bisect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-02-24 14:12:55.000000 fronts-1.0.1/tests/test_rootfinding/test_bracket_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-02-24 14:12:55.000000 fronts-1.0.1/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-02-24 14:12:55.000000 fronts-1.0.1/tests/test_solve_flowrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-24 14:12:55.000000 fronts-1.0.1/tests/test_solve_from_guess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.594539 fronts-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-19 00:59:38.000000 fronts-1.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-07-19 00:59:38.000000 fronts-1.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-19 00:59:38.000000 fronts-1.0.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-19 00:59:38.000000 fronts-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-19 00:59:38.000000 fronts-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-07-19 00:59:49.594539 fronts-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-07-19 00:59:38.000000 fronts-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.590538 fronts-1.0.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-19 00:59:38.000000 fronts-1.0.2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-19 00:59:38.000000 fronts-1.0.2/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.590538 fronts-1.0.2/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-19 00:59:38.000000 fronts-1.0.2/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-19 00:59:38.000000 fronts-1.0.2/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.590538 fronts-1.0.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.590538 fronts-1.0.2/examples/1INFILTR/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      729 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/1INFILTR/D.py
+-rw-r--r--   0 runner    (1001) docker     (123)   567061 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/1INFILTR/Nod_Inf.out
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1403 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/1INFILTR/solve.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2196 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/1INFILTR/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.590538 fronts-1.0.2/examples/HF135/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      904 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/HF135/D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32297 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/HF135/groundwaterFoam_results.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1994 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/HF135/inverse1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/HF135/inverse2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1893 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/HF135/radial.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2498 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/HF135/refine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/HF135/solve.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/HF135/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.590538 fronts-1.0.2/examples/exact/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/exact/D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      685 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/exact/fromguess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/exact/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.590538 fronts-1.0.2/examples/powerlaw/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      393 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/powerlaw/D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1341 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/powerlaw/inverse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-07-19 00:59:38.000000 fronts-1.0.2/examples/powerlaw/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.594539 fronts-1.0.2/fronts/
+-rw-r--r--   0 runner    (1001) docker     (123)    33379 2023-07-19 00:59:38.000000 fronts-1.0.2/fronts/D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-19 00:59:38.000000 fronts-1.0.2/fronts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-07-19 00:59:38.000000 fronts-1.0.2/fronts/_boltzmann.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-19 00:59:38.000000 fronts-1.0.2/fronts/_rootfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49649 2023-07-19 00:59:38.000000 fronts-1.0.2/fronts/_semiinfinite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.594539 fronts-1.0.2/fronts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-07-19 00:59:49.000000 fronts-1.0.2/fronts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-19 00:59:49.000000 fronts-1.0.2/fronts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 00:59:49.000000 fronts-1.0.2/fronts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-19 00:59:49.000000 fronts-1.0.2/fronts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 00:59:49.000000 fronts-1.0.2/fronts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-19 00:59:38.000000 fronts-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.594539 fronts-1.0.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-07-19 00:59:38.000000 fronts-1.0.2/resources/CIMEC.png
+-rw-r--r--   0 runner    (1001) docker     (123)   174760 2023-07-19 00:59:38.000000 fronts-1.0.2/resources/GSaMLogo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-19 00:59:38.000000 fronts-1.0.2/resources/INTEC.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24144 2023-07-19 00:59:38.000000 fronts-1.0.2/resources/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34790 2023-07-19 00:59:38.000000 fronts-1.0.2/resources/powerlaw_c.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44856 2023-07-19 00:59:38.000000 fronts-1.0.2/resources/powerlaw_flux.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-19 00:59:49.594539 fronts-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 00:59:38.000000 fronts-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.594539 fronts-1.0.2/symbolic/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      912 2023-07-19 00:59:38.000000 fronts-1.0.2/symbolic/brooks_and_corey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-19 00:59:38.000000 fronts-1.0.2/symbolic/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      699 2023-07-19 00:59:38.000000 fronts-1.0.2/symbolic/letd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2023-07-19 00:59:38.000000 fronts-1.0.2/symbolic/letxs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-07-19 00:59:38.000000 fronts-1.0.2/symbolic/ode_jac.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      892 2023-07-19 00:59:38.000000 fronts-1.0.2/symbolic/van_genuchten.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.594539 fronts-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 00:59:38.000000 fronts-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-19 00:59:38.000000 fronts-1.0.2/tests/test_D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-19 00:59:38.000000 fronts-1.0.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-19 00:59:38.000000 fronts-1.0.2/tests/test_inverse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 00:59:49.594539 fronts-1.0.2/tests/test_rootfinding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-19 00:59:38.000000 fronts-1.0.2/tests/test_rootfinding/checkobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-19 00:59:38.000000 fronts-1.0.2/tests/test_rootfinding/test_bisect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-19 00:59:38.000000 fronts-1.0.2/tests/test_rootfinding/test_bracket_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-19 00:59:38.000000 fronts-1.0.2/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-19 00:59:38.000000 fronts-1.0.2/tests/test_solve_flowrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-19 00:59:38.000000 fronts-1.0.2/tests/test_solve_from_guess.py
```

### Comparing `fronts-1.0.1/CHANGELOG.md` & `fronts-1.0.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.2] - 2023-07-18
+
+### Changed
+
+- Update packaging and dependencies.
+
 ## [1.0.1] - 2023-02-24
 
 ### Changed
 
 - Add new references to the documentation.
 
 ## [1.0.0] - 2023-02-23
@@ -166,14 +172,15 @@
 - Fix typo in name of _examples/1INFILTR_.
 - Fix wrong name used in mention of _examples/refine.py_ in the README file.
 
 ## [0.9.2] - 2019-09-16
 
 First public pre-release version.
 
+[1.0.2]: https://github.com/gerlero/fronts/compare/v1.0.1...1.0.2
 [1.0.1]: https://github.com/gerlero/fronts/compare/v1.0.0...1.0.1
 [1.0.0]: https://github.com/gerlero/fronts/compare/v0.9.12...v1.0.0
 [0.9.12]: https://github.com/gerlero/fronts/compare/v0.9.11...v0.9.12
 [0.9.11]: https://github.com/gerlero/fronts/compare/v0.9.10...v0.9.11
 [0.9.10]: https://github.com/gerlero/fronts/compare/v0.9.9...v0.9.10
 [0.9.9]: https://github.com/gerlero/fronts/compare/v0.9.8...v0.9.9
 [0.9.8]: https://github.com/gerlero/fronts/compare/v0.9.7...v0.9.8
```

### Comparing `fronts-1.0.1/LICENSE.txt` & `fronts-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/MANIFEST.in` & `fronts-1.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/PKG-INFO` & `fronts-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fronts
-Version: 1.0.1
+Version: 1.0.2
 Summary: Numerical library for nonlinear diffusion problems in semi-infinite domains
 Home-page: https://github.com/gerlero/fronts
 Author: Gabriel S. Gerlero
 Author-email: ggerlero@cimec.unl.edu.ar
 Project-URL: Documentation, https://fronts.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/gerlero/fronts/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fronts-1.0.1/README.md` & `fronts-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/doc/Makefile` & `fronts-1.0.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/doc/make.bat` & `fronts-1.0.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/doc/source/conf.py` & `fronts-1.0.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/doc/source/index.rst` & `fronts-1.0.2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/1INFILTR/D.py` & `fronts-1.0.2/examples/1INFILTR/D.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/1INFILTR/Nod_Inf.out` & `fronts-1.0.2/examples/1INFILTR/Nod_Inf.out`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/1INFILTR/solve.py` & `fronts-1.0.2/examples/1INFILTR/solve.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/1INFILTR/validation.py` & `fronts-1.0.2/examples/1INFILTR/validation.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/HF135/D.py` & `fronts-1.0.2/examples/HF135/D.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/HF135/groundwaterFoam_results.csv` & `fronts-1.0.2/examples/HF135/groundwaterFoam_results.csv`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/HF135/inverse1.py` & `fronts-1.0.2/examples/HF135/inverse1.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/HF135/inverse2.py` & `fronts-1.0.2/examples/HF135/inverse2.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/HF135/radial.py` & `fronts-1.0.2/examples/HF135/radial.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/HF135/refine.py` & `fronts-1.0.2/examples/HF135/refine.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/HF135/solve.py` & `fronts-1.0.2/examples/HF135/solve.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/HF135/validation.py` & `fronts-1.0.2/examples/HF135/validation.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/README.md` & `fronts-1.0.2/examples/README.md`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/exact/D.py` & `fronts-1.0.2/examples/exact/D.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/exact/fromguess.py` & `fronts-1.0.2/examples/exact/fromguess.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/exact/solve.py` & `fronts-1.0.2/examples/exact/solve.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/powerlaw/inverse.py` & `fronts-1.0.2/examples/powerlaw/inverse.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/examples/powerlaw/solve.py` & `fronts-1.0.2/examples/powerlaw/solve.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/fronts/D.py` & `fronts-1.0.2/fronts/D.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/fronts/_boltzmann.py` & `fronts-1.0.2/fronts/_boltzmann.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/fronts/_rootfinding.py` & `fronts-1.0.2/fronts/_rootfinding.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/fronts/_semiinfinite.py` & `fronts-1.0.2/fronts/_semiinfinite.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/fronts.egg-info/PKG-INFO` & `fronts-1.0.2/fronts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fronts
-Version: 1.0.1
+Version: 1.0.2
 Summary: Numerical library for nonlinear diffusion problems in semi-infinite domains
 Home-page: https://github.com/gerlero/fronts
 Author: Gabriel S. Gerlero
 Author-email: ggerlero@cimec.unl.edu.ar
 Project-URL: Documentation, https://fronts.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/gerlero/fronts/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fronts-1.0.1/fronts.egg-info/SOURCES.txt` & `fronts-1.0.2/fronts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/resources/CIMEC.png` & `fronts-1.0.2/resources/CIMEC.png`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/resources/GSaMLogo.png` & `fronts-1.0.2/resources/GSaMLogo.png`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/resources/INTEC.png` & `fronts-1.0.2/resources/INTEC.png`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/resources/logo.png` & `fronts-1.0.2/resources/logo.png`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/resources/powerlaw_c.png` & `fronts-1.0.2/resources/powerlaw_c.png`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/resources/powerlaw_flux.png` & `fronts-1.0.2/resources/powerlaw_flux.png`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/setup.cfg` & `fronts-1.0.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fronts
-version = 1.0.1
+version = attr: fronts.__version__
 author = Gabriel S. Gerlero
 author_email = ggerlero@cimec.unl.edu.ar
 description = Numerical library for nonlinear diffusion problems in semi-infinite domains
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gerlero/fronts
 project_urls = 
@@ -25,35 +25,32 @@
 	Topic :: Software Development :: Libraries
 	Operating System :: OS Independent
 
 [options]
 packages = fronts
 python_requires = >=3.7
 install_requires = 
-	scipy >= 1.4.0
+	scipy>=1.4.0,<2
 	numpy
-	sympy >= 1.0
-	importlib_metadata; python_version <= "3.8"
+	sympy==1.*
 
 [options.extras_require]
 examples = 
-	matplotlib
+	matplotlib==3.*
 test = 
-	pytest-cov
 	check-manifest
-	matplotlib
-	autograd
+	pytest==7.*
+	pytest-cov
+	autograd>=1.3,<2
+	%(examples)s
 doc = 
 	sphinx
 	sphinx_rtd_theme
 dev = 
-	matplotlib
-	pytest-cov
-	check-manifest
-	autograd
-	sphinx
-	sphinx_rtd_theme
+	%(examples)s
+	%(test)s
+	%(doc)s
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fronts-1.0.1/symbolic/brooks_and_corey.py` & `fronts-1.0.2/symbolic/brooks_and_corey.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/symbolic/generate.py` & `fronts-1.0.2/symbolic/generate.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/symbolic/letd.py` & `fronts-1.0.2/symbolic/letd.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/symbolic/letxs.py` & `fronts-1.0.2/symbolic/letxs.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/symbolic/ode_jac.py` & `fronts-1.0.2/symbolic/ode_jac.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/symbolic/van_genuchten.py` & `fronts-1.0.2/symbolic/van_genuchten.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/tests/test_D.py` & `fronts-1.0.2/tests/test_D.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/tests/test_inverse.py` & `fronts-1.0.2/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/tests/test_rootfinding/checkobj.py` & `fronts-1.0.2/tests/test_rootfinding/checkobj.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/tests/test_rootfinding/test_bisect.py` & `fronts-1.0.2/tests/test_rootfinding/test_bisect.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/tests/test_rootfinding/test_bracket_root.py` & `fronts-1.0.2/tests/test_rootfinding/test_bracket_root.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/tests/test_solve.py` & `fronts-1.0.2/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `fronts-1.0.1/tests/test_solve_flowrate.py` & `fronts-1.0.2/tests/test_solve_flowrate.py`

 * *Files identical despite different names*

