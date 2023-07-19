# Comparing `tmp/collective.behavior.relatedmedia-3.3.0.tar.gz` & `tmp/collective.behavior.relatedmedia-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.behavior.relatedmedia-3.3.0.tar", last modified: Mon Jul 17 15:03:02 2023, max compression
+gzip compressed data, was "collective.behavior.relatedmedia-3.3.1.tar", last modified: Wed Jul 19 09:45:26 2023, max compression
```

## Comparing `collective.behavior.relatedmedia-3.3.0.tar` & `collective.behavior.relatedmedia-3.3.1.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.675646 collective.behavior.relatedmedia-3.3.0/
--rw-r--r--   0 peterm     (501) staff       (20)      749 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/.gitignore
--rw-r--r--   0 peterm     (501) staff       (20)     3330 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/CHANGES.md
--rw-r--r--   0 peterm     (501) staff       (20)      107 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/MANIFEST.in
--rw-r--r--   0 peterm     (501) staff       (20)    11526 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/Makefile
--rw-r--r--   0 peterm     (501) staff       (20)     5972 2023-07-17 15:03:02.675713 collective.behavior.relatedmedia-3.3.0/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     1626 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/README.md
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.667471 collective.behavior.relatedmedia-3.3.0/collective/
--rw-r--r--   0 peterm     (501) staff       (20)      245 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.668717 collective.behavior.relatedmedia-3.3.0/collective/behavior/
--rw-r--r--   0 peterm     (501) staff       (20)      245 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.670846 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/
--rw-r--r--   0 peterm     (501) staff       (20)      124 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)     8209 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/behavior.py
--rw-r--r--   0 peterm     (501) staff       (20)     8652 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/browser.py
--rw-r--r--   0 peterm     (501) staff       (20)     5973 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     3977 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/events.py
--rw-r--r--   0 peterm     (501) staff       (20)     2790 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/interfaces.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.670987 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.665001 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/de/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.671137 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/
--rw-r--r--   0 peterm     (501) staff       (20)     7885 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.po
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.665135 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/en/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.671288 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/
--rw-r--r--   0 peterm     (501) staff       (20)     6392 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.po
--rwxr-xr-x   0 peterm     (501) staff       (20)      503 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/update.sh
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.665568 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.671840 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/
--rw-r--r--   0 peterm     (501) staff       (20)      205 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/browserlayer.xml
--rw-r--r--   0 peterm     (501) staff       (20)      610 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/controlpanel.xml
--rw-r--r--   0 peterm     (501) staff       (20)       71 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/metadata.xml
--rw-r--r--   0 peterm     (501) staff       (20)     1258 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.671964 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/types/
--rw-r--r--   0 peterm     (501) staff       (20)      288 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/types/Document.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.672356 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/
--rw-r--r--   0 peterm     (501) staff       (20)      230 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 peterm     (501) staff       (20)      357 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 peterm     (501) staff       (20)      407 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.672493 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/types/
--rw-r--r--   0 peterm     (501) staff       (20)      304 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/uninstall/types/Document.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.665856 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.672641 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/local_config/
--rw-r--r--   0 peterm     (501) staff       (20)      541 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/local_config/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.672783 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/
--rw-r--r--   0 peterm     (501) staff       (20)      539 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.672925 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/types/
--rw-r--r--   0 peterm     (501) staff       (20)      305 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/types/Document.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.673084 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/registry_cleanup/
--rw-r--r--   0 peterm     (501) staff       (20)      223 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/registry_cleanup/registry.xml
--rw-r--r--   0 peterm     (501) staff       (20)      841 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/related_attachments.pt
--rw-r--r--   0 peterm     (501) staff       (20)      931 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/related_images.pt
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.673359 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/resources/
--rw-r--r--   0 peterm     (501) staff       (20)      824 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/resources/relateditems_selection.xml
--rw-r--r--   0 peterm     (501) staff       (20)      797 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/resources/relatedmedia.js
--rw-r--r--   0 peterm     (501) staff       (20)     1597 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/testing.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.673648 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/tests/
--rw-r--r--   0 peterm     (501) staff       (20)        2 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/tests/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)     2195 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/tests/test_setup.py
--rw-r--r--   0 peterm     (501) staff       (20)     2621 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/upgrades.py
--rw-r--r--   0 peterm     (501) staff       (20)     3699 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/upgrades.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     2974 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/utils.py
--rw-r--r--   0 peterm     (501) staff       (20)      480 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/viewlet_uploader.pt
--rw-r--r--   0 peterm     (501) staff       (20)     1165 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/widget.py
--rw-r--r--   0 peterm     (501) staff       (20)       60 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/widget_attachments_display.pt
--rw-r--r--   0 peterm     (501) staff       (20)       55 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/widget_images_display.pt
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.668576 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/
--rw-r--r--   0 peterm     (501) staff       (20)     5972 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     2974 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/SOURCES.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/dependency_links.txt
--rw-r--r--   0 peterm     (501) staff       (20)       40 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/entry_points.txt
--rw-r--r--   0 peterm     (501) staff       (20)       31 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/namespace_packages.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/not-zip-safe
--rw-r--r--   0 peterm     (501) staff       (20)      231 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/requires.txt
--rw-r--r--   0 peterm     (501) staff       (20)       11 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/top_level.txt
--rw-r--r--   0 peterm     (501) staff       (20)       58 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/constraints.txt
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-17 15:03:02.674695 collective.behavior.relatedmedia-3.3.0/docs/
--rw-r--r--   0 peterm     (501) staff       (20)    17987 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/docs/LICENSE.GPL
--rw-r--r--   0 peterm     (501) staff       (20)      747 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/docs/LICENSE.txt
--rw-r--r--   0 peterm     (501) staff       (20)   299492 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_basepath.png
--rw-r--r--   0 peterm     (501) staff       (20)   189513 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_settings.png
--rw-r--r--   0 peterm     (501) staff       (20)  1497793 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_view.png
--rw-r--r--   0 peterm     (501) staff       (20)      647 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/mx.ini
--rw-r--r--   0 peterm     (501) staff       (20)      182 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/requirements.txt
--rw-r--r--   0 peterm     (501) staff       (20)      418 2023-07-17 15:03:02.675985 collective.behavior.relatedmedia-3.3.0/setup.cfg
--rw-r--r--   0 peterm     (501) staff       (20)     2266 2023-07-17 15:03:02.000000 collective.behavior.relatedmedia-3.3.0/setup.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.470131 collective.behavior.relatedmedia-3.3.1/
+-rw-r--r--   0 peterm     (501) staff       (20)      749 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/.gitignore
+-rw-r--r--   0 peterm     (501) staff       (20)     3436 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/CHANGES.md
+-rw-r--r--   0 peterm     (501) staff       (20)      107 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/MANIFEST.in
+-rw-r--r--   0 peterm     (501) staff       (20)    11526 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/Makefile
+-rw-r--r--   0 peterm     (501) staff       (20)     6078 2023-07-19 09:45:26.470195 collective.behavior.relatedmedia-3.3.1/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     1626 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/README.md
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.461887 collective.behavior.relatedmedia-3.3.1/collective/
+-rw-r--r--   0 peterm     (501) staff       (20)      245 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.463134 collective.behavior.relatedmedia-3.3.1/collective/behavior/
+-rw-r--r--   0 peterm     (501) staff       (20)      245 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.465298 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/
+-rw-r--r--   0 peterm     (501) staff       (20)      124 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     8209 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/behavior.py
+-rw-r--r--   0 peterm     (501) staff       (20)     8652 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/browser.py
+-rw-r--r--   0 peterm     (501) staff       (20)     5973 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     3977 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/events.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2790 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/interfaces.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.465418 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.459337 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/de/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.465695 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/
+-rw-r--r--   0 peterm     (501) staff       (20)     3818 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.mo
+-rw-r--r--   0 peterm     (501) staff       (20)     7885 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.po
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.459466 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/en/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.465961 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/
+-rw-r--r--   0 peterm     (501) staff       (20)      458 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.mo
+-rw-r--r--   0 peterm     (501) staff       (20)     6392 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.po
+-rwxr-xr-x   0 peterm     (501) staff       (20)      503 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/update.sh
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.459876 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.466470 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/default/
+-rw-r--r--   0 peterm     (501) staff       (20)      205 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/default/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      610 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/default/controlpanel.xml
+-rw-r--r--   0 peterm     (501) staff       (20)       71 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/default/metadata.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     1258 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/default/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.466614 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/default/types/
+-rw-r--r--   0 peterm     (501) staff       (20)      256 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/default/types/Document.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.467033 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/uninstall/
+-rw-r--r--   0 peterm     (501) staff       (20)      230 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      357 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      407 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/uninstall/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.467174 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/uninstall/types/
+-rw-r--r--   0 peterm     (501) staff       (20)      304 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/uninstall/types/Document.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.460150 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/upgrades/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.467315 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/upgrades/local_config/
+-rw-r--r--   0 peterm     (501) staff       (20)      541 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/upgrades/local_config/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.467459 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/upgrades/package_rename/
+-rw-r--r--   0 peterm     (501) staff       (20)      539 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/upgrades/package_rename/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.467593 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/upgrades/package_rename/types/
+-rw-r--r--   0 peterm     (501) staff       (20)      305 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/upgrades/package_rename/types/Document.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.467717 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/upgrades/registry_cleanup/
+-rw-r--r--   0 peterm     (501) staff       (20)      223 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/upgrades/registry_cleanup/registry.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      841 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/related_attachments.pt
+-rw-r--r--   0 peterm     (501) staff       (20)      931 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/related_images.pt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.468006 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/resources/
+-rw-r--r--   0 peterm     (501) staff       (20)      824 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/resources/relateditems_selection.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      797 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/resources/relatedmedia.js
+-rw-r--r--   0 peterm     (501) staff       (20)     1597 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/testing.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.468270 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/tests/
+-rw-r--r--   0 peterm     (501) staff       (20)        2 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/tests/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2195 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/tests/test_setup.py
+-rw-r--r--   0 peterm     (501) staff       (20)     2621 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/upgrades.py
+-rw-r--r--   0 peterm     (501) staff       (20)     3699 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/upgrades.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     2974 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/utils.py
+-rw-r--r--   0 peterm     (501) staff       (20)      480 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/viewlet_uploader.pt
+-rw-r--r--   0 peterm     (501) staff       (20)     1165 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/widget.py
+-rw-r--r--   0 peterm     (501) staff       (20)       60 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/widget_attachments_display.pt
+-rw-r--r--   0 peterm     (501) staff       (20)       55 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/widget_images_display.pt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.463009 collective.behavior.relatedmedia-3.3.1/collective.behavior.relatedmedia.egg-info/
+-rw-r--r--   0 peterm     (501) staff       (20)     6078 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/collective.behavior.relatedmedia.egg-info/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     3158 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/collective.behavior.relatedmedia.egg-info/SOURCES.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/collective.behavior.relatedmedia.egg-info/dependency_links.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       40 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/collective.behavior.relatedmedia.egg-info/entry_points.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       31 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/collective.behavior.relatedmedia.egg-info/namespace_packages.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/collective.behavior.relatedmedia.egg-info/not-zip-safe
+-rw-r--r--   0 peterm     (501) staff       (20)      231 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/collective.behavior.relatedmedia.egg-info/requires.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       11 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/collective.behavior.relatedmedia.egg-info/top_level.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       58 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/constraints.txt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-07-19 09:45:26.469235 collective.behavior.relatedmedia-3.3.1/docs/
+-rw-r--r--   0 peterm     (501) staff       (20)    17987 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/docs/LICENSE.GPL
+-rw-r--r--   0 peterm     (501) staff       (20)      747 2023-07-19 09:45:25.000000 collective.behavior.relatedmedia-3.3.1/docs/LICENSE.txt
+-rw-r--r--   0 peterm     (501) staff       (20)   299492 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/docs/collective.behavior.relatedmedia_basepath.png
+-rw-r--r--   0 peterm     (501) staff       (20)   189513 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/docs/collective.behavior.relatedmedia_settings.png
+-rw-r--r--   0 peterm     (501) staff       (20)  1497793 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/docs/collective.behavior.relatedmedia_view.png
+-rw-r--r--   0 peterm     (501) staff       (20)      647 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/mx.ini
+-rw-r--r--   0 peterm     (501) staff       (20)      182 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/requirements.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      418 2023-07-19 09:45:26.470450 collective.behavior.relatedmedia-3.3.1/setup.cfg
+-rw-r--r--   0 peterm     (501) staff       (20)     2266 2023-07-19 09:45:26.000000 collective.behavior.relatedmedia-3.3.1/setup.py
```

### Comparing `collective.behavior.relatedmedia-3.3.0/.gitignore` & `collective.behavior.relatedmedia-3.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/CHANGES.md` & `collective.behavior.relatedmedia-3.3.1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+## 3.3.1 (2023-07-19)
+---------------------
+
+- Fix default behavior assignment for "Page".
+  [petschki]
+
+
 ## 3.3.0 (2023-07-17)
 ------------------
 
 Feature:
 
 - Mark `base_path` concept as deprecated and add a migration script for it.
   [petschki]
```

### Comparing `collective.behavior.relatedmedia-3.3.0/Makefile` & `collective.behavior.relatedmedia-3.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/PKG-INFO` & `collective.behavior.relatedmedia-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.behavior.relatedmedia
-Version: 3.3.0
+Version: 3.3.1
 Summary: Adds Various configuration fields and viewlets to manage and show content related images and attachments
 Home-page: https://github.com/kombinat/collective.behavior.relatedmedia
 Author: petschki
 Author-email: peter.mathis@kombinat.at
 License: gpl
 Keywords: plone richmedia relatedmedia
 Classifier: Development Status :: 5 - Production/Stable
@@ -84,14 +84,21 @@
 - Peter Holzer [agitator]
 
 
 Changelog
 =========
 
 
+## 3.3.1 (2023-07-19)
+---------------------
+
+- Fix default behavior assignment for "Page".
+  [petschki]
+
+
 ## 3.3.0 (2023-07-17)
 ------------------
 
 Feature:
 
 - Mark `base_path` concept as deprecated and add a migration script for it.
   [petschki]
```

### Comparing `collective.behavior.relatedmedia-3.3.0/README.md` & `collective.behavior.relatedmedia-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/behavior.py` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/behavior.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/browser.py` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/browser.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/configure.zcml` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/events.py` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/events.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/interfaces.py` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.po` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.po`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.po` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.po`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/controlpanel.xml` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/default/registry.xml` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/local_config/registry.xml` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/upgrades/local_config/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/profiles/upgrades/package_rename/registry.xml` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/profiles/upgrades/package_rename/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/related_attachments.pt` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/related_attachments.pt`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/related_images.pt` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/related_images.pt`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/resources/relateditems_selection.xml` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/resources/relateditems_selection.xml`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/resources/relatedmedia.js` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/resources/relatedmedia.js`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/testing.py` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/testing.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/tests/test_setup.py` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/upgrades.py` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/upgrades.zcml` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/utils.py` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/utils.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective/behavior/relatedmedia/widget.py` & `collective.behavior.relatedmedia-3.3.1/collective/behavior/relatedmedia/widget.py`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/PKG-INFO` & `collective.behavior.relatedmedia-3.3.1/collective.behavior.relatedmedia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.behavior.relatedmedia
-Version: 3.3.0
+Version: 3.3.1
 Summary: Adds Various configuration fields and viewlets to manage and show content related images and attachments
 Home-page: https://github.com/kombinat/collective.behavior.relatedmedia
 Author: petschki
 Author-email: peter.mathis@kombinat.at
 License: gpl
 Keywords: plone richmedia relatedmedia
 Classifier: Development Status :: 5 - Production/Stable
@@ -84,14 +84,21 @@
 - Peter Holzer [agitator]
 
 
 Changelog
 =========
 
 
+## 3.3.1 (2023-07-19)
+---------------------
+
+- Fix default behavior assignment for "Page".
+  [petschki]
+
+
 ## 3.3.0 (2023-07-17)
 ------------------
 
 Feature:
 
 - Mark `base_path` concept as deprecated and add a migration script for it.
   [petschki]
```

### Comparing `collective.behavior.relatedmedia-3.3.0/collective.behavior.relatedmedia.egg-info/SOURCES.txt` & `collective.behavior.relatedmedia-3.3.1/collective.behavior.relatedmedia.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 collective/behavior/relatedmedia/upgrades.zcml
 collective/behavior/relatedmedia/utils.py
 collective/behavior/relatedmedia/viewlet_uploader.pt
 collective/behavior/relatedmedia/widget.py
 collective/behavior/relatedmedia/widget_attachments_display.pt
 collective/behavior/relatedmedia/widget_images_display.pt
 collective/behavior/relatedmedia/locales/update.sh
+collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.mo
 collective/behavior/relatedmedia/locales/de/LC_MESSAGES/collective.behavior.relatedmedia.po
+collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.mo
 collective/behavior/relatedmedia/locales/en/LC_MESSAGES/collective.behavior.relatedmedia.po
 collective/behavior/relatedmedia/profiles/default/browserlayer.xml
 collective/behavior/relatedmedia/profiles/default/controlpanel.xml
 collective/behavior/relatedmedia/profiles/default/metadata.xml
 collective/behavior/relatedmedia/profiles/default/registry.xml
 collective/behavior/relatedmedia/profiles/default/types/Document.xml
 collective/behavior/relatedmedia/profiles/uninstall/browserlayer.xml
```

### Comparing `collective.behavior.relatedmedia-3.3.0/docs/LICENSE.GPL` & `collective.behavior.relatedmedia-3.3.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/docs/LICENSE.txt` & `collective.behavior.relatedmedia-3.3.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_basepath.png` & `collective.behavior.relatedmedia-3.3.1/docs/collective.behavior.relatedmedia_basepath.png`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_settings.png` & `collective.behavior.relatedmedia-3.3.1/docs/collective.behavior.relatedmedia_settings.png`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/docs/collective.behavior.relatedmedia_view.png` & `collective.behavior.relatedmedia-3.3.1/docs/collective.behavior.relatedmedia_view.png`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/mx.ini` & `collective.behavior.relatedmedia-3.3.1/mx.ini`

 * *Files identical despite different names*

### Comparing `collective.behavior.relatedmedia-3.3.0/setup.py` & `collective.behavior.relatedmedia-3.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.3.0"
+version = "3.3.1"
 
 this_directory = Path(__file__).parent
 long_description = (
     (this_directory / "README.md").read_text()
     + "\n\n"
     + (this_directory / "CHANGES.md").read_text()
 )
```

