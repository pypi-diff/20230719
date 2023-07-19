# Comparing `tmp/z3c.form-5.0.tar.gz` & `tmp/z3c.form-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.form-5.0.tar", last modified: Mon Jul 17 05:51:57 2023, max compression
+gzip compressed data, was "z3c.form-5.1.tar", last modified: Wed Jul 19 06:22:34 2023, max compression
```

## Comparing `z3c.form-5.0.tar` & `z3c.form-5.1.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.955147 z3c.form-5.0/
--rw-r--r--   0 m.howitz   (502) staff       (20)      550 2023-07-17 05:51:57.000000 z3c.form-5.0/AUTHOR.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    49995 2023-07-17 05:51:57.000000 z3c.form-5.0/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-17 05:51:57.000000 z3c.form-5.0/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-17 05:51:57.000000 z3c.form-5.0/COPYRIGHT.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-17 05:51:57.000000 z3c.form-5.0/LICENSE.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      625 2023-07-17 05:51:57.000000 z3c.form-5.0/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)    52692 2023-07-17 05:51:57.955221 z3c.form-5.0/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     1457 2023-07-17 05:51:57.000000 z3c.form-5.0/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1529 2023-07-17 05:51:57.000000 z3c.form-5.0/TODOS.rst
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.915246 z3c.form-5.0/benchmark/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.915500 z3c.form-5.0/benchmark/benchmark/
--rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.000000 z3c.form-5.0/benchmark/benchmark/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5453 2023-07-17 05:51:57.000000 z3c.form-5.0/benchmark/benchmark/tests.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      639 2023-07-17 05:51:57.000000 z3c.form-5.0/benchmark/setup.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1925 2023-07-17 05:51:57.000000 z3c.form-5.0/buildout.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)       74 2023-07-17 05:51:57.000000 z3c.form-5.0/doc-requirements.txt
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.916355 z3c.form-5.0/docs/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.917182 z3c.form-5.0/docs/advanced/
--rw-r--r--   0 m.howitz   (502) staff       (20)       43 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/advanced/action.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/advanced/browser-readme.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       52 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/advanced/contentprovider.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      440 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/advanced/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       46 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/advanced/validator.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       43 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/advanced/widget.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       27 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/authors.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/changelog.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     8817 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/conf.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      507 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/index.rst
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.918429 z3c.form-5.0/docs/informative/
--rw-r--r--   0 m.howitz   (502) staff       (20)       43 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/informative/adding.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       46 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/informative/converter.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       48 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/informative/datamanager.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      370 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/informative/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/informative/object-caveat.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       41 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/informative/term.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       44 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/informative/testing.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       41 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/informative/util.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       42 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/informative/value.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      194 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/interfaces.rst
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.919376 z3c.form-5.0/docs/mustread/
--rw-r--r--   0 m.howitz   (502) staff       (20)       43 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/mustread/button.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       42 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/mustread/field.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       41 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/mustread/form.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       42 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/mustread/group.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      501 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/mustread/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       44 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/mustread/subform.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       41 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/mustread/zcml.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       26 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/todos.rst
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.923048 z3c.form-5.0/docs/widgets/
--rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/button.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       53 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/checkbox.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       57 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/file-testing.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       49 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/file.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/image.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      331 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      232 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/multi-index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/multi.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       67 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/multi_dict_integration.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       67 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/multi_list_integration.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      440 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/object-index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/object.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       74 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/object_multi_dict_integration.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       74 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/object_multi_list_integration.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       70 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/object_single_integration.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/objectmulti.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       58 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/orderedselect.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       53 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/password.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/radio.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      241 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/select-index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       65 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/select-missing-terms.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       58 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/select-source.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/select.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/submit.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       49 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/text.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       53 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/textarea.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       54 2023-07-17 05:51:57.000000 z3c.form-5.0/docs/widgets/textlines.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      468 2023-07-17 05:51:57.955484 z3c.form-5.0/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     3535 2023-07-17 05:51:57.000000 z3c.form-5.0/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.910336 z3c.form-5.0/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.923182 z3c.form-5.0/src/z3c/
--rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.934688 z3c.form-5.0/src/z3c/form/
--rw-r--r--   0 m.howitz   (502) staff       (20)     3769 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       18 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3531 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/action.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     7116 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/action.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1009 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/adding.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3822 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/adding.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     2062 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/apidoc.zcml
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.950047 z3c.form-5.0/src/z3c/form/browser/
--rw-r--r--   0 m.howitz   (502) staff       (20)   108467 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       18 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1569 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/button.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2112 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/button.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      504 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/button.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      400 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/button_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1341 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/button_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     3550 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/checkbox.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    12977 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/checkbox.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1394 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/checkbox.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     1032 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/checkbox_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1719 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/checkbox_hidden.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     3630 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/checkbox_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      650 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/configure.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     3684 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/file-testing.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1627 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/file.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2744 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/file.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      795 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/file.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      901 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/file_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1506 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/file_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      803 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/file_testing.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     1748 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/file_testing_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2216 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/image.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2236 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/image.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      561 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/image.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      443 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/image_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1391 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/image_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      402 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    11574 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3017 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/multi.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    53182 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/multi.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1769 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/multi.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)    21277 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/multi_dict_integration.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     2543 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/multi_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      775 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/multi_hidden.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2711 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/multi_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)    13342 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/multi_list_integration.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1378 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/object.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    41342 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/object.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      993 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/object.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      573 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/object_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      167 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/object_hidden.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      814 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/object_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)    20538 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/object_multi_dict_integration.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    17265 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/object_multi_list_integration.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     6409 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/object_single_integration.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    66284 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/objectmulti.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     3570 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/orderedselect.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     8257 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/orderedselect.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1414 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/orderedselect.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     1032 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/orderedselect_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     3530 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/orderedselect_input.js
--rw-r--r--   0 m.howitz   (502) staff       (20)     4681 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/orderedselect_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1406 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/password.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2513 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/password.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      834 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/password.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      901 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/password_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1630 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/password_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     3379 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/radio.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    11113 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/radio.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1557 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/radio.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     1032 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/radio_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1129 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/radio_display_single.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      254 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/radio_hidden.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      591 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/radio_hidden_single.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      526 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/radio_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1679 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/radio_input_single.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     8116 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/select-missing-terms.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     2419 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/select-source.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     5303 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/select.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    12457 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/select.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1129 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/select.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     1032 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/select_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      553 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/select_hidden.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1884 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/select_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1431 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/submit.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2079 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/submit.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      567 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/submit.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      400 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/submit_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1348 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/submit_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     6459 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/tests.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1501 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/text.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2872 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/text.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     2555 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/text.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      973 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/text_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      492 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/text_hidden.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1817 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/text_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1637 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textarea.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2957 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textarea.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1165 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textarea.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      973 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textarea_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      491 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textarea_hidden.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1344 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textarea_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1447 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textlines.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2596 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textlines.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      941 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textlines.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      901 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textlines_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      492 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textlines_hidden.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1383 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/textlines_input.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     8118 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/widget.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1139 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/widget.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      752 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/widget.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      746 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/widget_layout.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      179 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/browser/widget_layout_hidden.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)    10774 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/button.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    20250 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/button.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      474 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/button.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      936 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/configure.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     4170 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/contentprovider.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    10529 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/contentprovider.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    15934 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/converter.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    32345 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/converter.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1192 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/converter.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     5439 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/datamanager.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     9790 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/datamanager.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      252 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/datamanager.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      187 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/error.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     4652 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/error.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     7618 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/error.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      658 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/error.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      276 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/events.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    12662 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/field.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    30679 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/field.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      645 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/file.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)      201 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/file_testing.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)    54362 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/form-chameleon-issue-repeat-addons.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1589 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/form-graph.dot
--rw-r--r--   0 m.howitz   (502) staff       (20)    11877 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/form-graph.png
--rw-r--r--   0 m.howitz   (502) staff       (20)    14191 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/form-graph.ps
--rw-r--r--   0 m.howitz   (502) staff       (20)    11240 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/form.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    62369 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/form.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     5215 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/group.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    34362 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/group.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1531 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/hint.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    24637 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/hint.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      806 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/i18n.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      450 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    34868 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/interfaces.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.950192 z3c.form-5.0/src/z3c/form/locales/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.910751 z3c.form-5.0/src/z3c/form/locales/cs/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.950329 z3c.form-5.0/src/z3c/form/locales/cs/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    15838 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/cs/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.910906 z3c.form-5.0/src/z3c/form/locales/da/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.950473 z3c.form-5.0/src/z3c/form/locales/da/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    20237 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/da/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.911071 z3c.form-5.0/src/z3c/form/locales/de/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.950632 z3c.form-5.0/src/z3c/form/locales/de/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    21286 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/de/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.911223 z3c.form-5.0/src/z3c/form/locales/en/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.950804 z3c.form-5.0/src/z3c/form/locales/en/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    20088 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/en/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.911374 z3c.form-5.0/src/z3c/form/locales/es/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.950976 z3c.form-5.0/src/z3c/form/locales/es/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    21695 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/es/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.911525 z3c.form-5.0/src/z3c/form/locales/fi/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.951146 z3c.form-5.0/src/z3c/form/locales/fi/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    20304 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/fi/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.911670 z3c.form-5.0/src/z3c/form/locales/fr/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.951400 z3c.form-5.0/src/z3c/form/locales/fr/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    21371 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/fr/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.911850 z3c.form-5.0/src/z3c/form/locales/hu/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.951596 z3c.form-5.0/src/z3c/form/locales/hu/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    20407 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/hu/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.912006 z3c.form-5.0/src/z3c/form/locales/it/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.951778 z3c.form-5.0/src/z3c/form/locales/it/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    17134 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/it/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.912165 z3c.form-5.0/src/z3c/form/locales/ja/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.951963 z3c.form-5.0/src/z3c/form/locales/ja/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    22129 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/ja/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.912315 z3c.form-5.0/src/z3c/form/locales/nl/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.952147 z3c.form-5.0/src/z3c/form/locales/nl/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    15569 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/nl/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.912474 z3c.form-5.0/src/z3c/form/locales/no/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.952317 z3c.form-5.0/src/z3c/form/locales/no/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    19695 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/no/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.912639 z3c.form-5.0/src/z3c/form/locales/pt_BR/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.952502 z3c.form-5.0/src/z3c/form/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    21108 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/pt_BR/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.912800 z3c.form-5.0/src/z3c/form/locales/ru/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.952666 z3c.form-5.0/src/z3c/form/locales/ru/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    24489 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/ru/LC_MESSAGES/z3c.form.po
--rw-r--r--   0 m.howitz   (502) staff       (20)    15117 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/z3c.form.pot
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.912952 z3c.form-5.0/src/z3c/form/locales/zh_CN/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.952822 z3c.form-5.0/src/z3c/form/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    18293 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/zh_CN/LC_MESSAGES/z3c.form.po
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.913102 z3c.form-5.0/src/z3c/form/locales/zh_TW/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.952988 z3c.form-5.0/src/z3c/form/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 m.howitz   (502) staff       (20)    16824 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/locales/zh_TW/LC_MESSAGES/z3c.form.po
--rw-r--r--   0 m.howitz   (502) staff       (20)      701 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/meta.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     2587 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/object-caveat.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    16848 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/object.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      234 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/object.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     4300 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/outputchecker.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2192 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/subform.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    21774 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/subform.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)    11141 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/term.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    17576 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/term.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      550 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/term.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)    30239 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/testing.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1333 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/testing.rst
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.955011 z3c.form-5.0/src/z3c/form/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)       18 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      248 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/custom_error.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      206 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/integration.css
--rw-r--r--   0 m.howitz   (502) staff       (20)     1336 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/integration_edit.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1263 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/simple_caredit.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      367 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/simple_display.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1139 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/simple_edit.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1565 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/simple_edit_with_providers.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2253 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/simple_groupedit.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2047 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/simple_nested_groupedit.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      880 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/simple_owneredit.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)      749 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/simple_subedit.pt
--rw-r--r--   0 m.howitz   (502) staff       (20)     4642 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/test_bugfix.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5583 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/tests/test_doc.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      114 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/translation.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     8232 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/util.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    14778 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/util.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     7672 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/validator.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    19325 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/validator.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      322 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/validator.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     3092 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/value.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     7810 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/value.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1510 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/widget-graph.dot
--rw-r--r--   0 m.howitz   (502) staff       (20)    13789 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/widget-graph.png
--rw-r--r--   0 m.howitz   (502) staff       (20)    13773 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/widget-graph.ps
--rw-r--r--   0 m.howitz   (502) staff       (20)    24310 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/widget.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    31408 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/widget.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     5832 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/zcml.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     7561 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c/form/zcml.rst
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-17 05:51:57.924208 z3c.form-5.0/src/z3c.form.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)    52692 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c.form.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     8888 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c.form.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c.form.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c.form.egg-info/namespace_packages.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c.form.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)      550 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c.form.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-07-17 05:51:57.000000 z3c.form-5.0/src/z3c.form.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1599 2023-07-17 05:51:57.000000 z3c.form-5.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.247236 z3c.form-5.1/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      550 2023-07-19 06:22:33.000000 z3c.form-5.1/AUTHOR.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    50112 2023-07-19 06:22:33.000000 z3c.form-5.1/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-19 06:22:33.000000 z3c.form-5.1/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-19 06:22:33.000000 z3c.form-5.1/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-19 06:22:33.000000 z3c.form-5.1/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      625 2023-07-19 06:22:33.000000 z3c.form-5.1/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    52809 2023-07-19 06:22:34.247320 z3c.form-5.1/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1457 2023-07-19 06:22:33.000000 z3c.form-5.1/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1529 2023-07-19 06:22:33.000000 z3c.form-5.1/TODOS.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.206644 z3c.form-5.1/benchmark/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.206943 z3c.form-5.1/benchmark/benchmark/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:33.000000 z3c.form-5.1/benchmark/benchmark/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5453 2023-07-19 06:22:33.000000 z3c.form-5.1/benchmark/benchmark/tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      639 2023-07-19 06:22:33.000000 z3c.form-5.1/benchmark/setup.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1925 2023-07-19 06:22:33.000000 z3c.form-5.1/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)       74 2023-07-19 06:22:33.000000 z3c.form-5.1/doc-requirements.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.207821 z3c.form-5.1/docs/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.208667 z3c.form-5.1/docs/advanced/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       43 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/advanced/action.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/advanced/browser-readme.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       52 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/advanced/contentprovider.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      440 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/advanced/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       46 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/advanced/validator.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       43 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/advanced/widget.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       27 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/authors.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/changelog.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8817 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      507 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/index.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.209925 z3c.form-5.1/docs/informative/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       43 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/informative/adding.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       46 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/informative/converter.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       48 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/informative/datamanager.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      370 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/informative/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/informative/object-caveat.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       41 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/informative/term.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       44 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/informative/testing.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       41 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/informative/util.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       42 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/informative/value.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      194 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/interfaces.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.210893 z3c.form-5.1/docs/mustread/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       43 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/mustread/button.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       42 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/mustread/field.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       41 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/mustread/form.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       42 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/mustread/group.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      501 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/mustread/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       44 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/mustread/subform.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       41 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/mustread/zcml.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       26 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/todos.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.214728 z3c.form-5.1/docs/widgets/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/button.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       53 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/checkbox.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       57 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/file-testing.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       49 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/file.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/image.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      331 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      232 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/multi-index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/multi.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       67 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/multi_dict_integration.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       67 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/multi_list_integration.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      440 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/object-index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/object.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       74 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/object_multi_dict_integration.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       74 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/object_multi_list_integration.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       70 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/object_single_integration.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/objectmulti.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       58 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/orderedselect.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       53 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/password.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/radio.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      241 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/select-index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       65 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/select-missing-terms.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       58 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/select-source.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/select.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/submit.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       49 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/text.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       53 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/textarea.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       54 2023-07-19 06:22:33.000000 z3c.form-5.1/docs/widgets/textlines.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      468 2023-07-19 06:22:34.247612 z3c.form-5.1/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3535 2023-07-19 06:22:33.000000 z3c.form-5.1/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.201620 z3c.form-5.1/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.214883 z3c.form-5.1/src/z3c/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.227008 z3c.form-5.1/src/z3c/form/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3769 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       18 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3531 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/action.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7116 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/action.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1009 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/adding.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3822 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/adding.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2062 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/apidoc.zcml
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.242493 z3c.form-5.1/src/z3c/form/browser/
+-rw-r--r--   0 m.howitz   (502) staff       (20)   108467 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       18 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1569 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/button.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2112 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/button.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      504 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/button.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      400 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/button_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1341 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/button_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3550 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/checkbox.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12977 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/checkbox.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1394 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/checkbox.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1032 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/checkbox_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1719 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/checkbox_hidden.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3630 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/checkbox_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      650 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3684 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/file-testing.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1627 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/file.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2744 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/file.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      795 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/file.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      901 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/file_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1506 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/file_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      803 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/file_testing.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1748 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/file_testing_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2216 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/image.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2236 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/image.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      561 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/image.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      443 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/image_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1391 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/image_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      402 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11574 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3017 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/multi.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    53182 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/multi.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1769 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/multi.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21277 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/multi_dict_integration.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2543 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/multi_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      775 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/multi_hidden.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2711 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/multi_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13342 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/multi_list_integration.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1378 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/object.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    41342 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/object.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      993 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/object.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      573 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/object_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      167 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/object_hidden.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      814 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/object_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20538 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/object_multi_dict_integration.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17265 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/object_multi_list_integration.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6409 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/object_single_integration.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    66284 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/objectmulti.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3570 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/orderedselect.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8257 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/orderedselect.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1414 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/orderedselect.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1032 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/orderedselect_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3530 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/orderedselect_input.js
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4681 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/orderedselect_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1406 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/password.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2513 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/password.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      834 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/password.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      901 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/password_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1630 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/password_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3379 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/radio.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11113 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/radio.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1557 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/radio.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1032 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/radio_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1129 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/radio_display_single.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      254 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/radio_hidden.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      591 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/radio_hidden_single.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      526 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/radio_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1679 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/radio_input_single.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8116 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/select-missing-terms.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2419 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/select-source.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5303 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/select.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12457 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/select.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1129 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/select.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1032 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/select_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      553 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/select_hidden.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1884 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/select_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1431 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/submit.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2079 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/submit.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      567 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/submit.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      400 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/submit_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1348 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/submit_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6459 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1501 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/text.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2872 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/text.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2555 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/text.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      973 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/text_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      492 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/text_hidden.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1817 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/text_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1637 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textarea.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2957 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textarea.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1165 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textarea.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      973 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textarea_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      491 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textarea_hidden.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1344 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textarea_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1447 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textlines.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2596 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textlines.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      941 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textlines.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      901 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textlines_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      492 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textlines_hidden.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1383 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/textlines_input.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10797 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/widget.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3288 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/widget.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      752 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/widget.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      746 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/widget_layout.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/browser/widget_layout_hidden.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10774 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/button.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20250 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/button.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      474 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/button.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      936 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4170 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/contentprovider.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10529 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/contentprovider.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    15934 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/converter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    32345 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/converter.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1192 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/converter.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5439 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/datamanager.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9790 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/datamanager.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      252 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/datamanager.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      187 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/error.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4652 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/error.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7618 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/error.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      658 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/error.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      276 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/events.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12662 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/field.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    30679 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/field.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      645 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/file.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      201 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/file_testing.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)    54362 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/form-chameleon-issue-repeat-addons.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1589 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/form-graph.dot
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11877 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/form-graph.png
+-rw-r--r--   0 m.howitz   (502) staff       (20)    14191 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/form-graph.ps
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11240 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/form.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    62369 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/form.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5215 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/group.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    34362 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/group.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1531 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/hint.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    24637 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/hint.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      806 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/i18n.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      450 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    34868 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/interfaces.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.242640 z3c.form-5.1/src/z3c/form/locales/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.202043 z3c.form-5.1/src/z3c/form/locales/cs/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.242787 z3c.form-5.1/src/z3c/form/locales/cs/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    15838 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/cs/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.202206 z3c.form-5.1/src/z3c/form/locales/da/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.242926 z3c.form-5.1/src/z3c/form/locales/da/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20237 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/da/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.202360 z3c.form-5.1/src/z3c/form/locales/de/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.243096 z3c.form-5.1/src/z3c/form/locales/de/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21286 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/de/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.202514 z3c.form-5.1/src/z3c/form/locales/en/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.243257 z3c.form-5.1/src/z3c/form/locales/en/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20088 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/en/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.202675 z3c.form-5.1/src/z3c/form/locales/es/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.243420 z3c.form-5.1/src/z3c/form/locales/es/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21695 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/es/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.202839 z3c.form-5.1/src/z3c/form/locales/fi/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.243573 z3c.form-5.1/src/z3c/form/locales/fi/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20304 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/fi/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.202996 z3c.form-5.1/src/z3c/form/locales/fr/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.243733 z3c.form-5.1/src/z3c/form/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21371 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/fr/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.203150 z3c.form-5.1/src/z3c/form/locales/hu/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.243892 z3c.form-5.1/src/z3c/form/locales/hu/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20407 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/hu/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.203304 z3c.form-5.1/src/z3c/form/locales/it/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.244048 z3c.form-5.1/src/z3c/form/locales/it/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17134 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/it/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.203467 z3c.form-5.1/src/z3c/form/locales/ja/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.244206 z3c.form-5.1/src/z3c/form/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    22129 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/ja/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.203633 z3c.form-5.1/src/z3c/form/locales/nl/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.244368 z3c.form-5.1/src/z3c/form/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    15569 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/nl/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.203800 z3c.form-5.1/src/z3c/form/locales/no/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.244511 z3c.form-5.1/src/z3c/form/locales/no/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    19695 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/no/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.203952 z3c.form-5.1/src/z3c/form/locales/pt_BR/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.244668 z3c.form-5.1/src/z3c/form/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21108 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/pt_BR/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.204112 z3c.form-5.1/src/z3c/form/locales/ru/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.244826 z3c.form-5.1/src/z3c/form/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    24489 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/ru/LC_MESSAGES/z3c.form.po
+-rw-r--r--   0 m.howitz   (502) staff       (20)    15117 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/z3c.form.pot
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.204272 z3c.form-5.1/src/z3c/form/locales/zh_CN/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.244986 z3c.form-5.1/src/z3c/form/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    18293 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/zh_CN/LC_MESSAGES/z3c.form.po
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.204442 z3c.form-5.1/src/z3c/form/locales/zh_TW/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.245144 z3c.form-5.1/src/z3c/form/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    16824 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/locales/zh_TW/LC_MESSAGES/z3c.form.po
+-rw-r--r--   0 m.howitz   (502) staff       (20)      701 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2587 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/object-caveat.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    16848 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/object.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      234 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/object.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4300 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/outputchecker.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2192 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/subform.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21774 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/subform.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11141 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/term.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17576 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/term.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      550 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/term.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)    30239 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/testing.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1333 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/testing.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.247083 z3c.form-5.1/src/z3c/form/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       18 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      248 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/custom_error.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      206 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/integration.css
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1336 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/integration_edit.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1263 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/simple_caredit.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      367 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/simple_display.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1139 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/simple_edit.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1565 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/simple_edit_with_providers.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2253 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/simple_groupedit.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2047 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/simple_nested_groupedit.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      880 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/simple_owneredit.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      749 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/simple_subedit.pt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4642 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/test_bugfix.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5583 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/tests/test_doc.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      114 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/translation.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8232 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/util.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    14778 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/util.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7672 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/validator.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    19325 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/validator.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      322 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/validator.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3092 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/value.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7810 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/value.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1510 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/widget-graph.dot
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13789 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/widget-graph.png
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13773 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/widget-graph.ps
+-rw-r--r--   0 m.howitz   (502) staff       (20)    24310 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/widget.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    31408 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/widget.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5832 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/zcml.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7561 2023-07-19 06:22:33.000000 z3c.form-5.1/src/z3c/form/zcml.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-19 06:22:34.216032 z3c.form-5.1/src/z3c.form.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    52809 2023-07-19 06:22:34.000000 z3c.form-5.1/src/z3c.form.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8888 2023-07-19 06:22:34.000000 z3c.form-5.1/src/z3c.form.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-19 06:22:34.000000 z3c.form-5.1/src/z3c.form.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-07-19 06:22:34.000000 z3c.form-5.1/src/z3c.form.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-19 06:22:34.000000 z3c.form-5.1/src/z3c.form.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      550 2023-07-19 06:22:34.000000 z3c.form-5.1/src/z3c.form.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-07-19 06:22:34.000000 z3c.form-5.1/src/z3c.form.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1599 2023-07-19 06:22:33.000000 z3c.form-5.1/tox.ini
```

### Comparing `z3c.form-5.0/AUTHOR.rst` & `z3c.form-5.1/AUTHOR.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/CHANGES.rst` & `z3c.form-5.1/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+5.1 (2023-07-19)
+----------------
+
+- HTMLFormElement.attributes: Allow to extend HTML attributes programmatically.
+
+
 5.0 (2023-07-17)
 ----------------
 
 - Add support for Python 3.11.
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `z3c.form-5.0/CONTRIBUTING.md` & `z3c.form-5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/LICENSE.txt` & `z3c.form-5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/MANIFEST.in` & `z3c.form-5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/PKG-INFO` & `z3c.form-5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.form
-Version: 5.0
+Version: 5.1
 Summary: An advanced form and widget framework for Zope 3
 Home-page: https://github.com/zopefoundation/z3c.form
 Author: Stephan Richter, Roger Ineichen and the Zope Community
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope3 form widget
 Classifier: Development Status :: 5 - Production/Stable
@@ -74,14 +74,20 @@
 
 
 
 =========
 Changelog
 =========
 
+5.1 (2023-07-19)
+----------------
+
+- HTMLFormElement.attributes: Allow to extend HTML attributes programmatically.
+
+
 5.0 (2023-07-17)
 ----------------
 
 - Add support for Python 3.11.
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `z3c.form-5.0/README.rst` & `z3c.form-5.1/README.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/TODOS.rst` & `z3c.form-5.1/TODOS.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/benchmark/benchmark/tests.py` & `z3c.form-5.1/benchmark/benchmark/tests.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/benchmark/setup.py` & `z3c.form-5.1/benchmark/setup.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/buildout.cfg` & `z3c.form-5.1/buildout.cfg`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/docs/conf.py` & `z3c.form-5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/setup.py` & `z3c.form-5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     if isinstance(text, bytes):
         text = text.decode('utf-8')
     return text.encode('ascii', 'xmlcharrefreplace').decode()
 
 
 setup(
     name='z3c.form',
-    version='5.0',
+    version='5.1',
     author="Stephan Richter, Roger Ineichen and the Zope Community",
     author_email="zope-dev@zope.dev",
     description="An advanced form and widget framework for Zope 3",
     long_description=(
         read('README.rst')
         + '\n\n' +
         '.. contents:: \n\n'
```

### Comparing `z3c.form-5.0/src/z3c/form/README.rst` & `z3c.form-5.1/src/z3c/form/README.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/action.py` & `z3c.form-5.1/src/z3c/form/action.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/action.rst` & `z3c.form-5.1/src/z3c/form/action.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/adding.py` & `z3c.form-5.1/src/z3c/form/adding.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/adding.rst` & `z3c.form-5.1/src/z3c/form/adding.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/apidoc.zcml` & `z3c.form-5.1/src/z3c/form/apidoc.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/README.rst` & `z3c.form-5.1/src/z3c/form/browser/README.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/button.py` & `z3c.form-5.1/src/z3c/form/browser/button.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/button.rst` & `z3c.form-5.1/src/z3c/form/browser/button.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/button_input.pt` & `z3c.form-5.1/src/z3c/form/browser/button_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/checkbox.py` & `z3c.form-5.1/src/z3c/form/browser/checkbox.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/checkbox.rst` & `z3c.form-5.1/src/z3c/form/browser/checkbox.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/checkbox.zcml` & `z3c.form-5.1/src/z3c/form/browser/checkbox.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/checkbox_display.pt` & `z3c.form-5.1/src/z3c/form/browser/checkbox_display.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/checkbox_hidden.pt` & `z3c.form-5.1/src/z3c/form/browser/checkbox_hidden.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/checkbox_input.pt` & `z3c.form-5.1/src/z3c/form/browser/checkbox_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/configure.zcml` & `z3c.form-5.1/src/z3c/form/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/file-testing.rst` & `z3c.form-5.1/src/z3c/form/browser/file-testing.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/file.py` & `z3c.form-5.1/src/z3c/form/browser/file.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/file.rst` & `z3c.form-5.1/src/z3c/form/browser/file.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/file.zcml` & `z3c.form-5.1/src/z3c/form/browser/file.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/file_display.pt` & `z3c.form-5.1/src/z3c/form/browser/file_display.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/file_input.pt` & `z3c.form-5.1/src/z3c/form/browser/file_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/file_testing.zcml` & `z3c.form-5.1/src/z3c/form/browser/file_testing.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/file_testing_input.pt` & `z3c.form-5.1/src/z3c/form/browser/file_testing_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/image.py` & `z3c.form-5.1/src/z3c/form/browser/image.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/image.rst` & `z3c.form-5.1/src/z3c/form/browser/image.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/image.zcml` & `z3c.form-5.1/src/z3c/form/browser/image.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/image_input.pt` & `z3c.form-5.1/src/z3c/form/browser/image_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/interfaces.py` & `z3c.form-5.1/src/z3c/form/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/multi.py` & `z3c.form-5.1/src/z3c/form/browser/multi.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/multi.rst` & `z3c.form-5.1/src/z3c/form/browser/multi.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/multi.zcml` & `z3c.form-5.1/src/z3c/form/browser/multi.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/multi_dict_integration.rst` & `z3c.form-5.1/src/z3c/form/browser/multi_dict_integration.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/multi_display.pt` & `z3c.form-5.1/src/z3c/form/browser/multi_display.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/multi_hidden.pt` & `z3c.form-5.1/src/z3c/form/browser/multi_hidden.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/multi_input.pt` & `z3c.form-5.1/src/z3c/form/browser/multi_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/multi_list_integration.rst` & `z3c.form-5.1/src/z3c/form/browser/multi_list_integration.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/object.py` & `z3c.form-5.1/src/z3c/form/browser/object.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/object.rst` & `z3c.form-5.1/src/z3c/form/browser/object.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/object.zcml` & `z3c.form-5.1/src/z3c/form/browser/object.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/object_display.pt` & `z3c.form-5.1/src/z3c/form/browser/object_display.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/object_input.pt` & `z3c.form-5.1/src/z3c/form/browser/object_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/object_multi_dict_integration.rst` & `z3c.form-5.1/src/z3c/form/browser/object_multi_dict_integration.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/object_multi_list_integration.rst` & `z3c.form-5.1/src/z3c/form/browser/object_multi_list_integration.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/object_single_integration.rst` & `z3c.form-5.1/src/z3c/form/browser/object_single_integration.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/objectmulti.rst` & `z3c.form-5.1/src/z3c/form/browser/objectmulti.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/orderedselect.py` & `z3c.form-5.1/src/z3c/form/browser/orderedselect.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/orderedselect.rst` & `z3c.form-5.1/src/z3c/form/browser/orderedselect.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/orderedselect.zcml` & `z3c.form-5.1/src/z3c/form/browser/orderedselect.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/orderedselect_display.pt` & `z3c.form-5.1/src/z3c/form/browser/orderedselect_display.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/orderedselect_input.js` & `z3c.form-5.1/src/z3c/form/browser/orderedselect_input.js`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/orderedselect_input.pt` & `z3c.form-5.1/src/z3c/form/browser/orderedselect_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/password.py` & `z3c.form-5.1/src/z3c/form/browser/password.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/password.rst` & `z3c.form-5.1/src/z3c/form/browser/password.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/password.zcml` & `z3c.form-5.1/src/z3c/form/browser/password.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/password_display.pt` & `z3c.form-5.1/src/z3c/form/browser/password_display.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/password_input.pt` & `z3c.form-5.1/src/z3c/form/browser/password_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/radio.py` & `z3c.form-5.1/src/z3c/form/browser/radio.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/radio.rst` & `z3c.form-5.1/src/z3c/form/browser/radio.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/radio.zcml` & `z3c.form-5.1/src/z3c/form/browser/radio.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/radio_display.pt` & `z3c.form-5.1/src/z3c/form/browser/radio_display.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/radio_display_single.pt` & `z3c.form-5.1/src/z3c/form/browser/radio_display_single.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/radio_hidden_single.pt` & `z3c.form-5.1/src/z3c/form/browser/radio_hidden_single.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/radio_input.pt` & `z3c.form-5.1/src/z3c/form/browser/radio_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/radio_input_single.pt` & `z3c.form-5.1/src/z3c/form/browser/radio_input_single.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/select-missing-terms.rst` & `z3c.form-5.1/src/z3c/form/browser/select-missing-terms.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/select-source.rst` & `z3c.form-5.1/src/z3c/form/browser/select-source.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/select.py` & `z3c.form-5.1/src/z3c/form/browser/select.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/select.rst` & `z3c.form-5.1/src/z3c/form/browser/select.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/select.zcml` & `z3c.form-5.1/src/z3c/form/browser/select.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/select_display.pt` & `z3c.form-5.1/src/z3c/form/browser/select_display.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/select_hidden.pt` & `z3c.form-5.1/src/z3c/form/browser/select_hidden.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/select_input.pt` & `z3c.form-5.1/src/z3c/form/browser/select_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/submit.py` & `z3c.form-5.1/src/z3c/form/browser/submit.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/submit.rst` & `z3c.form-5.1/src/z3c/form/browser/submit.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/submit.zcml` & `z3c.form-5.1/src/z3c/form/browser/submit.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/submit_input.pt` & `z3c.form-5.1/src/z3c/form/browser/submit_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/tests.py` & `z3c.form-5.1/src/z3c/form/browser/tests.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/text.py` & `z3c.form-5.1/src/z3c/form/browser/text.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/text.rst` & `z3c.form-5.1/src/z3c/form/browser/text.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/text.zcml` & `z3c.form-5.1/src/z3c/form/browser/text.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/text_display.pt` & `z3c.form-5.1/src/z3c/form/browser/text_display.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/text_input.pt` & `z3c.form-5.1/src/z3c/form/browser/text_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/textarea.py` & `z3c.form-5.1/src/z3c/form/browser/textarea.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/textarea.rst` & `z3c.form-5.1/src/z3c/form/browser/textarea.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/textarea.zcml` & `z3c.form-5.1/src/z3c/form/browser/textarea.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/textarea_display.pt` & `z3c.form-5.1/src/z3c/form/browser/textarea_display.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/textarea_input.pt` & `z3c.form-5.1/src/z3c/form/browser/textarea_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/textlines.py` & `z3c.form-5.1/src/z3c/form/browser/textlines.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/textlines.rst` & `z3c.form-5.1/src/z3c/form/browser/textlines.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/textlines.zcml` & `z3c.form-5.1/src/z3c/form/browser/textlines.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/textlines_display.pt` & `z3c.form-5.1/src/z3c/form/browser/textlines_display.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/textlines_input.pt` & `z3c.form-5.1/src/z3c/form/browser/textlines_input.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/widget.py` & `z3c.form-5.1/src/z3c/form/browser/widget.py`

 * *Files 20% similar despite different names*

```diff
@@ -159,50 +159,150 @@
 
     def update(self):
         """See z3c.form.interfaces.IWidget"""
         super().update()
         if self.mode == INPUT_MODE and self.required:
             self.addClass('required')
 
+    @property
+    def _html_attributes(self) -> list:
+        """Return a list of HTML attributes managed by this class."""
+        # This is basically a list of all the FieldProperty names except for
+        # the `css` property, which is not an HTML attribute.
+        return [
+            "id",
+            "klass",  # will be changed to `class`
+            "style",
+            "title",
+            "lang",
+            "onclick",
+            "ondblclick",
+            "onmousedown",
+            "onmouseup",
+            "onmouseover",
+            "onmousemove",
+            "onmouseout",
+            "onkeypress",
+            "onkeydown",
+            "onkeyup",
+            "disabled",
+            "tabindex",
+            "onfocus",
+            "onblur",
+            "onchange",
+        ]
+
+    _attributes = None
+
+    @property
+    def attributes(self) -> dict:
+        # If `attributes` were explicitly set, return them.
+        if isinstance(self._attributes, dict):
+            return self._attributes
+
+        # Otherwise return the default set of non-empty HTML attributes.
+        attributes_items = [
+            ("class" if attr == "klass" else attr, getattr(self, attr, None))
+            for attr in self._html_attributes
+        ]
+        self._attributes = {key: val for key, val in attributes_items if val}
+        return self._attributes
+
+    @attributes.setter
+    def attributes(self, value: dict):
+        # Store the explicitly set attributes.
+        self._attributes = value
+
 
 @zope.interface.implementer(interfaces.IHTMLInputWidget)
 class HTMLInputWidget(HTMLFormElement):
 
     readonly = FieldProperty(interfaces.IHTMLInputWidget['readonly'])
     alt = FieldProperty(interfaces.IHTMLInputWidget['alt'])
     accesskey = FieldProperty(interfaces.IHTMLInputWidget['accesskey'])
     onselect = FieldProperty(interfaces.IHTMLInputWidget['onselect'])
 
+    @property
+    def _html_attributes(self) -> list:
+        attributes = super()._html_attributes
+        attributes.extend(
+            [
+                "readonly",
+                "alt",
+                "accesskey",
+                "onselect",
+            ]
+        )
+        return attributes
+
 
 @zope.interface.implementer(interfaces.IHTMLTextInputWidget)
 class HTMLTextInputWidget(HTMLInputWidget):
 
     size = FieldProperty(interfaces.IHTMLTextInputWidget['size'])
     maxlength = FieldProperty(interfaces.IHTMLTextInputWidget['maxlength'])
     placeholder = FieldProperty(interfaces.IHTMLTextInputWidget['placeholder'])
     autocapitalize = FieldProperty(
         interfaces.IHTMLTextInputWidget['autocapitalize'])
 
+    @property
+    def _html_attributes(self) -> list:
+        attributes = super()._html_attributes
+        attributes.extend(
+            [
+                "size",
+                "maxlength",
+                "placeholder",
+                "autocapitalize",
+            ]
+        )
+        return attributes
+
 
 @zope.interface.implementer(interfaces.IHTMLTextAreaWidget)
 class HTMLTextAreaWidget(HTMLFormElement):
 
     rows = FieldProperty(interfaces.IHTMLTextAreaWidget['rows'])
     cols = FieldProperty(interfaces.IHTMLTextAreaWidget['cols'])
     readonly = FieldProperty(interfaces.IHTMLTextAreaWidget['readonly'])
     accesskey = FieldProperty(interfaces.IHTMLTextAreaWidget['accesskey'])
     onselect = FieldProperty(interfaces.IHTMLTextAreaWidget['onselect'])
 
+    @property
+    def _html_attributes(self) -> list:
+        attributes = super()._html_attributes
+        attributes.extend(
+            [
+                "rows",
+                "cols",
+                "readonly",
+                "accesskey",
+                "onselect",
+            ]
+        )
+        return attributes
+
 
 @zope.interface.implementer(interfaces.IHTMLSelectWidget)
 class HTMLSelectWidget(HTMLFormElement):
 
     multiple = FieldProperty(interfaces.IHTMLSelectWidget['multiple'])
     size = FieldProperty(interfaces.IHTMLSelectWidget['size'])
 
+    @property
+    def _html_attributes(self) -> list:
+        attributes = super()._html_attributes
+        attributes.extend(
+            [
+                "multiple",
+                "size",
+            ]
+        )
+        return attributes
+
 
 def addFieldClass(widget):
     """Add a class to the widget that is based on the field type name.
 
     If the widget does not have field, then nothing is done.
     """
     if IFieldWidget.providedBy(widget):
```

### Comparing `z3c.form-5.0/src/z3c/form/browser/widget.zcml` & `z3c.form-5.1/src/z3c/form/browser/widget.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/browser/widget_layout.pt` & `z3c.form-5.1/src/z3c/form/browser/widget_layout.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/button.py` & `z3c.form-5.1/src/z3c/form/button.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/button.rst` & `z3c.form-5.1/src/z3c/form/button.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/configure.zcml` & `z3c.form-5.1/src/z3c/form/configure.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/contentprovider.py` & `z3c.form-5.1/src/z3c/form/contentprovider.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/contentprovider.rst` & `z3c.form-5.1/src/z3c/form/contentprovider.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/converter.py` & `z3c.form-5.1/src/z3c/form/converter.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/converter.rst` & `z3c.form-5.1/src/z3c/form/converter.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/converter.zcml` & `z3c.form-5.1/src/z3c/form/converter.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/datamanager.py` & `z3c.form-5.1/src/z3c/form/datamanager.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/datamanager.rst` & `z3c.form-5.1/src/z3c/form/datamanager.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/error.py` & `z3c.form-5.1/src/z3c/form/error.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/error.rst` & `z3c.form-5.1/src/z3c/form/error.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/error.zcml` & `z3c.form-5.1/src/z3c/form/error.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/field.py` & `z3c.form-5.1/src/z3c/form/field.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/field.rst` & `z3c.form-5.1/src/z3c/form/field.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/file.zcml` & `z3c.form-5.1/src/z3c/form/file.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/form-chameleon-issue-repeat-addons.rst` & `z3c.form-5.1/src/z3c/form/form-chameleon-issue-repeat-addons.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/form-graph.dot` & `z3c.form-5.1/src/z3c/form/form-graph.dot`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/form-graph.png` & `z3c.form-5.1/src/z3c/form/form-graph.png`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/form-graph.ps` & `z3c.form-5.1/src/z3c/form/form-graph.ps`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/form.py` & `z3c.form-5.1/src/z3c/form/form.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/form.rst` & `z3c.form-5.1/src/z3c/form/form.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/group.py` & `z3c.form-5.1/src/z3c/form/group.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/group.rst` & `z3c.form-5.1/src/z3c/form/group.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/hint.py` & `z3c.form-5.1/src/z3c/form/hint.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/hint.rst` & `z3c.form-5.1/src/z3c/form/hint.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/i18n.py` & `z3c.form-5.1/src/z3c/form/i18n.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/interfaces.py` & `z3c.form-5.1/src/z3c/form/interfaces.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/cs/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/cs/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/da/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/da/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/de/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/de/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/en/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/en/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/es/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/es/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/fi/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/fi/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/fr/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/fr/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/hu/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/hu/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/it/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/it/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/ja/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/ja/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/nl/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/nl/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/no/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/no/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/pt_BR/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/pt_BR/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/ru/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/ru/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/z3c.form.pot` & `z3c.form-5.1/src/z3c/form/locales/z3c.form.pot`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/zh_CN/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/zh_CN/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/locales/zh_TW/LC_MESSAGES/z3c.form.po` & `z3c.form-5.1/src/z3c/form/locales/zh_TW/LC_MESSAGES/z3c.form.po`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/meta.zcml` & `z3c.form-5.1/src/z3c/form/meta.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/object-caveat.rst` & `z3c.form-5.1/src/z3c/form/object-caveat.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/object.py` & `z3c.form-5.1/src/z3c/form/object.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/outputchecker.py` & `z3c.form-5.1/src/z3c/form/outputchecker.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/subform.py` & `z3c.form-5.1/src/z3c/form/subform.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/subform.rst` & `z3c.form-5.1/src/z3c/form/subform.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/term.py` & `z3c.form-5.1/src/z3c/form/term.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/term.rst` & `z3c.form-5.1/src/z3c/form/term.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/term.zcml` & `z3c.form-5.1/src/z3c/form/term.zcml`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/testing.py` & `z3c.form-5.1/src/z3c/form/testing.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/testing.rst` & `z3c.form-5.1/src/z3c/form/testing.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/tests/integration_edit.pt` & `z3c.form-5.1/src/z3c/form/tests/integration_edit.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/tests/simple_caredit.pt` & `z3c.form-5.1/src/z3c/form/tests/simple_caredit.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/tests/simple_edit.pt` & `z3c.form-5.1/src/z3c/form/tests/simple_edit.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/tests/simple_edit_with_providers.pt` & `z3c.form-5.1/src/z3c/form/tests/simple_edit_with_providers.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/tests/simple_groupedit.pt` & `z3c.form-5.1/src/z3c/form/tests/simple_groupedit.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/tests/simple_nested_groupedit.pt` & `z3c.form-5.1/src/z3c/form/tests/simple_nested_groupedit.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/tests/simple_owneredit.pt` & `z3c.form-5.1/src/z3c/form/tests/simple_owneredit.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/tests/simple_subedit.pt` & `z3c.form-5.1/src/z3c/form/tests/simple_subedit.pt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/tests/test_bugfix.py` & `z3c.form-5.1/src/z3c/form/tests/test_bugfix.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/tests/test_doc.py` & `z3c.form-5.1/src/z3c/form/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/util.py` & `z3c.form-5.1/src/z3c/form/util.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/util.rst` & `z3c.form-5.1/src/z3c/form/util.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/validator.py` & `z3c.form-5.1/src/z3c/form/validator.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/validator.rst` & `z3c.form-5.1/src/z3c/form/validator.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/value.py` & `z3c.form-5.1/src/z3c/form/value.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/value.rst` & `z3c.form-5.1/src/z3c/form/value.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/widget-graph.dot` & `z3c.form-5.1/src/z3c/form/widget-graph.dot`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/widget-graph.png` & `z3c.form-5.1/src/z3c/form/widget-graph.png`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/widget-graph.ps` & `z3c.form-5.1/src/z3c/form/widget-graph.ps`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/widget.py` & `z3c.form-5.1/src/z3c/form/widget.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/widget.rst` & `z3c.form-5.1/src/z3c/form/widget.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/zcml.py` & `z3c.form-5.1/src/z3c/form/zcml.py`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c/form/zcml.rst` & `z3c.form-5.1/src/z3c/form/zcml.rst`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c.form.egg-info/PKG-INFO` & `z3c.form-5.1/src/z3c.form.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.form
-Version: 5.0
+Version: 5.1
 Summary: An advanced form and widget framework for Zope 3
 Home-page: https://github.com/zopefoundation/z3c.form
 Author: Stephan Richter, Roger Ineichen and the Zope Community
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: zope3 form widget
 Classifier: Development Status :: 5 - Production/Stable
@@ -74,14 +74,20 @@
 
 
 
 =========
 Changelog
 =========
 
+5.1 (2023-07-19)
+----------------
+
+- HTMLFormElement.attributes: Allow to extend HTML attributes programmatically.
+
+
 5.0 (2023-07-17)
 ----------------
 
 - Add support for Python 3.11.
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `z3c.form-5.0/src/z3c.form.egg-info/SOURCES.txt` & `z3c.form-5.1/src/z3c.form.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/src/z3c.form.egg-info/requires.txt` & `z3c.form-5.1/src/z3c.form.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `z3c.form-5.0/tox.ini` & `z3c.form-5.1/tox.ini`

 * *Files identical despite different names*

