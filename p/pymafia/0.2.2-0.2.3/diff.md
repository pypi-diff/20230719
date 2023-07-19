# Comparing `tmp/pymafia-0.2.2.tar.gz` & `tmp/pymafia-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymafia-0.2.2.tar", max compression
+gzip compressed data, was "pymafia-0.2.3.tar", max compression
```

## Comparing `pymafia-0.2.2.tar` & `pymafia-0.2.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1068 2023-07-12 19:04:30.209512 pymafia-0.2.2/LICENSE
--rw-r--r--   0        0        0     5241 2023-07-12 19:04:30.209512 pymafia-0.2.2/README.md
--rw-r--r--   0        0        0     1283 2023-07-12 19:05:15.994309 pymafia-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      390 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/__init__.py
--rw-r--r--   0        0        0      283 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/ash/__init__.py
--rw-r--r--   0        0        0     3251 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/ash/conversion.py
--rw-r--r--   0        0        0     1421 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/ash/library.py
--rw-r--r--   0        0        0     3315 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/combat.py
--rw-r--r--   0        0        0     1527 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/datatypes/__init__.py
--rw-r--r--   0        0        0     2442 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/datatypes/bounty.py
--rw-r--r--   0        0        0     1836 2023-07-12 19:04:30.209512 pymafia-0.2.2/src/pymafia/datatypes/class_.py
--rw-r--r--   0        0        0     2464 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/coinmaster.py
--rw-r--r--   0        0        0     2526 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/effect.py
--rw-r--r--   0        0        0     2653 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/element.py
--rw-r--r--   0        0        0     6826 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/familiar.py
--rw-r--r--   0        0        0    11495 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/item.py
--rw-r--r--   0        0        0     5338 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/location.py
--rw-r--r--   0        0        0     1813 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/modifier.py
--rw-r--r--   0        0        0     6712 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/monster.py
--rw-r--r--   0        0        0     1976 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/path.py
--rw-r--r--   0        0        0     2772 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/phylum.py
--rw-r--r--   0        0        0     2765 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/servant.py
--rw-r--r--   0        0        0     3160 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/skill.py
--rw-r--r--   0        0        0     2542 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/slot.py
--rw-r--r--   0        0        0     1314 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/stat.py
--rw-r--r--   0        0        0     2610 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/thrall.py
--rw-r--r--   0        0        0     2889 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/datatypes/vykea.py
--rw-r--r--   0        0        0      545 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/__init__.py
--rw-r--r--   0        0        0      583 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/barrel_god.py
--rw-r--r--   0        0        0      890 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/boxing_daycare.py
--rw-r--r--   0        0        0     1350 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/cartography.py
--rw-r--r--   0        0        0     1030 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/cosplay_saber.py
--rw-r--r--   0        0        0     1784 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/crimbo_shrub.py
--rw-r--r--   0        0        0     1286 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/god_lobster.py
--rw-r--r--   0        0        0     1569 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/love_tunnel.py
--rw-r--r--   0        0        0     1044 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/mumming_trunk.py
--rw-r--r--   0        0        0     3518 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/pantogram.py
--rw-r--r--   0        0        0     1597 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/protonic_pack.py
--rw-r--r--   0        0        0     1139 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/snojo.py
--rw-r--r--   0        0        0     1299 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/songboom.py
--rw-r--r--   0        0        0      670 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/stomping_boots.py
--rw-r--r--   0        0        0     1408 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/iotms/witchess.py
--rw-r--r--   0        0        0      125 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/kolmafia/__init__.py
--rw-r--r--   0        0        0     1397 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/kolmafia/kolmafia.py
--rw-r--r--   0        0        0     1572 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/kolmafia/patch.py
--rw-r--r--   0        0        0     1682 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/player.py
--rw-r--r--   0        0        0     1148 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/preference.py
--rw-r--r--   0        0        0     1277 2023-07-12 19:04:30.213512 pymafia-0.2.2/src/pymafia/utils.py
--rw-r--r--   0        0        0     5913 1970-01-01 00:00:00.000000 pymafia-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-19 00:19:44.272158 pymafia-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5694 2023-07-19 00:19:44.276158 pymafia-0.2.3/README.md
+-rw-r--r--   0        0        0     1283 2023-07-19 00:20:21.588134 pymafia-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      390 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/__init__.py
+-rw-r--r--   0        0        0      283 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/ash/__init__.py
+-rw-r--r--   0        0        0     3251 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/ash/conversion.py
+-rw-r--r--   0        0        0     1421 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/ash/library.py
+-rw-r--r--   0        0        0     3315 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/combat.py
+-rw-r--r--   0        0        0     1527 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/__init__.py
+-rw-r--r--   0        0        0     2442 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/bounty.py
+-rw-r--r--   0        0        0     1836 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/class_.py
+-rw-r--r--   0        0        0     2464 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/coinmaster.py
+-rw-r--r--   0        0        0     2526 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/effect.py
+-rw-r--r--   0        0        0     2653 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/element.py
+-rw-r--r--   0        0        0     6826 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/familiar.py
+-rw-r--r--   0        0        0    11495 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/item.py
+-rw-r--r--   0        0        0     5338 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/location.py
+-rw-r--r--   0        0        0     1813 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/modifier.py
+-rw-r--r--   0        0        0     6712 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/monster.py
+-rw-r--r--   0        0        0     1976 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/path.py
+-rw-r--r--   0        0        0     2772 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/phylum.py
+-rw-r--r--   0        0        0     2765 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/servant.py
+-rw-r--r--   0        0        0     3160 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/skill.py
+-rw-r--r--   0        0        0     2542 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/slot.py
+-rw-r--r--   0        0        0     1314 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/stat.py
+-rw-r--r--   0        0        0     2610 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/thrall.py
+-rw-r--r--   0        0        0     2889 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/vykea.py
+-rw-r--r--   0        0        0      545 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/__init__.py
+-rw-r--r--   0        0        0      583 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/barrel_god.py
+-rw-r--r--   0        0        0      890 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/boxing_daycare.py
+-rw-r--r--   0        0        0     1350 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/cartography.py
+-rw-r--r--   0        0        0     1030 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/cosplay_saber.py
+-rw-r--r--   0        0        0     1784 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/crimbo_shrub.py
+-rw-r--r--   0        0        0     1286 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/god_lobster.py
+-rw-r--r--   0        0        0     1569 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/love_tunnel.py
+-rw-r--r--   0        0        0     1044 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/mumming_trunk.py
+-rw-r--r--   0        0        0     3518 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/pantogram.py
+-rw-r--r--   0        0        0     1597 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/protonic_pack.py
+-rw-r--r--   0        0        0     1139 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/snojo.py
+-rw-r--r--   0        0        0     1299 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/songboom.py
+-rw-r--r--   0        0        0      670 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/stomping_boots.py
+-rw-r--r--   0        0        0     1408 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/witchess.py
+-rw-r--r--   0        0        0      125 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/kolmafia/__init__.py
+-rw-r--r--   0        0        0     1875 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/kolmafia/kolmafia.py
+-rw-r--r--   0        0        0     1504 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/kolmafia/patch.py
+-rw-r--r--   0        0        0     1682 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/player.py
+-rw-r--r--   0        0        0     1148 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/preference.py
+-rw-r--r--   0        0        0     1277 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/utils.py
+-rw-r--r--   0        0        0     6366 1970-01-01 00:00:00.000000 pymafia-0.2.3/PKG-INFO
```

### Comparing `pymafia-0.2.2/LICENSE` & `pymafia-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/README.md` & `pymafia-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,29 @@
 ```
 pip install pymafia
 ```
 
 *pymafia* uses [JPype](https://github.com/kivy/pyjnius) to reflect KoLmafia's Java environment, so you will need to install a Java Development Kit (JDK) on your operating system — KoLmafia's developers recommend [Adoptium v17](https://adoptium.net/index.html). For information on troubleshooting your Java installation, see [JPype's troubleshooting guide](https://jpype.readthedocs.io/en/latest/install.html#if-it-fails).
 
 ## Usage
-To get started, simply import *pymafia* or any of its components. Doing so will download a KoLmafia jar file (if it is not present in the current working directory) and start a Java Virtual Machine (JVM) with the jar file included in the JVM's classpath. This process can take over a minute depending on your internet connection. You can change the revision of KoLmafia to use by setting the revision in the `pymafia_config` module prior to importing *pymafia*.
+To get started, simply import *pymafia* or any of its components. Doing so will download a KoLmafia jar file (if it is not present in the configured location) and start a Java Virtual Machine (JVM) with the jar file included in the JVM's classpath. This process can take over a minute depending on your internet connection. 
+
+You can choose the revision of KoLmafia to use or location to run it from by setting these properties in the `pymafia_config` module prior to importing *pymafia*. The revision defaults to the last known working revision at the time of release and the location defaults to a folder named "kolmafia" in the current working directory.
 
 ```python
 >>> import pymafia_config
 
 >>> pymafia_config.set_revision(27467)
 
->>> pymafia_config.set_revision("latest")
+>>> pymafia_config.set_location("C:\\Users\\Documents\\kolmafia\\")
+
+>>> import pymafia # Start the JVM
 ```
 
-Once you have set your desired revision, you will most likely want to launch the KoLmafia GUI and login to your character. Both of these actions can be performed using the `utils` module.
+Once you have configured *pymafia* and started, you will most likely want to launch the KoLmafia GUI and login to your character. Both of these actions can be performed using the `utils` module.
 
 ```python
 >>> from pymafia.utils import launch_gui, login
 
 >>> launch_gui()
 
 >>> login("devster6")
@@ -44,15 +48,15 @@
 ```python
 >>> from pymafia.kolmafia import km
 
 >>> km.AdventureResult
 <java class 'net.sourceforge.kolmafia.AdventureResult'>
 ```
 
-The Java classes behave similar to how they do in Java with the exception of returning Python objects when possible. For more information on the type conversions, see [JPype's type matching guide](https://jpype.readthedocs.io/en/latest/userguide.html#type-matching).
+These classes behave similar to how they do in Java with the exception of returning Python objects when possible. For more information on type conversion, see [JPype's type matching guide](https://jpype.readthedocs.io/en/latest/userguide.html#type-matching).
 
 ```
 >>> km.AdventureResult.tallyItem("big rock")
 <java object 'net.sourceforge.kolmafia.AdventureResult'>
 
 >>> km.AdventureResult.tallyItem("big rock").isBountyItem()
 False
@@ -110,14 +114,17 @@
 >>> Coinmaster.NONE
 Coinmaster('none')
 
 >>> Slot.HAT
 Slot('hat')
 ```
 
+### Non-Documented Functionality
+There are  modules and subpackages and available within *pymafia* that have not been described here; I hope to provide comprehensive documentation in the future.
+
 ## Contributing
 To contribute to *pymafia*, you will need to set up a development environment using the following steps:
 1. Install [poetry](https://python-poetry.org/)
 2. Clone this repository
 3. Run `poetry install` inside the cloned repository
```

### Comparing `pymafia-0.2.2/pyproject.toml` & `pymafia-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymafia"
-version = "0.2.2"  # This is the standard placeholder for poetry-dynamic-versioning
+version = "0.2.3"  # This is the standard placeholder for poetry-dynamic-versioning
 description = "A Python module and bridge for reflecting KoLmafia's Java environment"
 license = "MIT"
 authors = ["MrFizzyBubbs <MrFizzyBubbs@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MrFizzyBubbs/pymafia"
 
 [tool.poetry.dependencies]
```

### Comparing `pymafia-0.2.2/src/pymafia/ash/conversion.py` & `pymafia-0.2.3/src/pymafia/ash/conversion.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/ash/library.py` & `pymafia-0.2.3/src/pymafia/ash/library.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/combat.py` & `pymafia-0.2.3/src/pymafia/combat.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/__init__.py` & `pymafia-0.2.3/src/pymafia/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/bounty.py` & `pymafia-0.2.3/src/pymafia/datatypes/bounty.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/class_.py` & `pymafia-0.2.3/src/pymafia/datatypes/class_.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/coinmaster.py` & `pymafia-0.2.3/src/pymafia/datatypes/coinmaster.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/effect.py` & `pymafia-0.2.3/src/pymafia/datatypes/effect.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/element.py` & `pymafia-0.2.3/src/pymafia/datatypes/element.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/familiar.py` & `pymafia-0.2.3/src/pymafia/datatypes/familiar.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/item.py` & `pymafia-0.2.3/src/pymafia/datatypes/item.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/location.py` & `pymafia-0.2.3/src/pymafia/datatypes/location.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/modifier.py` & `pymafia-0.2.3/src/pymafia/datatypes/modifier.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/monster.py` & `pymafia-0.2.3/src/pymafia/datatypes/monster.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/path.py` & `pymafia-0.2.3/src/pymafia/datatypes/path.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/phylum.py` & `pymafia-0.2.3/src/pymafia/datatypes/phylum.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/servant.py` & `pymafia-0.2.3/src/pymafia/datatypes/servant.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/skill.py` & `pymafia-0.2.3/src/pymafia/datatypes/skill.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/slot.py` & `pymafia-0.2.3/src/pymafia/datatypes/slot.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/stat.py` & `pymafia-0.2.3/src/pymafia/datatypes/stat.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/thrall.py` & `pymafia-0.2.3/src/pymafia/datatypes/thrall.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/datatypes/vykea.py` & `pymafia-0.2.3/src/pymafia/datatypes/vykea.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/__init__.py` & `pymafia-0.2.3/src/pymafia/iotms/__init__.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/barrel_god.py` & `pymafia-0.2.3/src/pymafia/iotms/barrel_god.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/boxing_daycare.py` & `pymafia-0.2.3/src/pymafia/iotms/boxing_daycare.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/cartography.py` & `pymafia-0.2.3/src/pymafia/iotms/cartography.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/cosplay_saber.py` & `pymafia-0.2.3/src/pymafia/iotms/cosplay_saber.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/crimbo_shrub.py` & `pymafia-0.2.3/src/pymafia/iotms/crimbo_shrub.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/god_lobster.py` & `pymafia-0.2.3/src/pymafia/iotms/god_lobster.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/love_tunnel.py` & `pymafia-0.2.3/src/pymafia/iotms/love_tunnel.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/mumming_trunk.py` & `pymafia-0.2.3/src/pymafia/iotms/mumming_trunk.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/pantogram.py` & `pymafia-0.2.3/src/pymafia/iotms/pantogram.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/protonic_pack.py` & `pymafia-0.2.3/src/pymafia/iotms/protonic_pack.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/snojo.py` & `pymafia-0.2.3/src/pymafia/iotms/snojo.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/songboom.py` & `pymafia-0.2.3/src/pymafia/iotms/songboom.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/stomping_boots.py` & `pymafia-0.2.3/src/pymafia/iotms/stomping_boots.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/iotms/witchess.py` & `pymafia-0.2.3/src/pymafia/iotms/witchess.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/kolmafia/kolmafia.py` & `pymafia-0.2.3/src/pymafia/kolmafia/kolmafia.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,59 @@
 import os
 import re
 import urllib.request
 import zipfile
+from contextlib import contextmanager
 from typing import Any, Iterable
 
 import jpype
 
 import pymafia.kolmafia.patch as patch
 import pymafia_config
 
 GITHUB_DOWNLOAD_URL = "https://github.com/kolmafia/kolmafia/releases/download/"
 JAVA_PATTERN = "(net\\/sourceforge\\/kolmafia.*\\/([^\\$]*))\\.class"
 
 
-def download_kolmafia(revision: int, location: str):
-    jar_url = GITHUB_DOWNLOAD_URL + f"r{revision}/KoLmafia-{revision}.jar"
-    urllib.request.urlretrieve(jar_url, filename=location)
+@contextmanager
+def chdir(path: str):
+    old_cwd = os.getcwd()
+    os.chdir(path)
+    try:
+        yield
+    finally:
+        os.chdir(old_cwd)
 
 
-class KoLmafia:
-    def __init__(self, revision: int):
-        location = f"KoLmafia-{revision}.jar"
+def download_kolmafia(revision: int, filename: str):
+    jar_url = GITHUB_DOWNLOAD_URL + f"r{revision}/KoLmafia-{revision}.jar"
+    urllib.request.urlretrieve(jar_url, filename=filename)
 
-        if not os.path.isfile(location):
-            download_kolmafia(revision, location)
 
-        jpype.startJVM(classpath=location, convertStrings=True)
+class KoLmafia:
+    def __init__(self, revision: int, location: str):
+        jar_location = os.path.join(location, f"KoLmafia-{revision}.jar")
+        os.makedirs(location, exist_ok=True)
+        if not os.path.isfile(jar_location):
+            download_kolmafia(revision, jar_location)
+
+        # KoLmafia will place its files in the current working directory, regardless of where the jar file is located
+        with chdir(location):
+            jpype.startJVM(classpath=jar_location, convertStrings=True)
         patch.apply()
 
         self.classes = {}
-        with zipfile.ZipFile(location) as archive:
+        with zipfile.ZipFile(jar_location) as archive:
             for filename in archive.namelist():
                 if match := re.search(JAVA_PATTERN, filename):
                     self.classes[match.group(2)] = match.group(1)
 
     def __dir__(self) -> Iterable[str]:
         return sorted(list(self.classes.keys()))
 
     def __getattr__(self, name: str) -> Any:
         if name in self.classes:
             return jpype.JClass(self.classes[name])
         return super().__getattribute__(name)
 
 
-km = KoLmafia(pymafia_config.revision)
+km = KoLmafia(pymafia_config.revision, pymafia_config.location)
```

### Comparing `pymafia-0.2.2/src/pymafia/kolmafia/patch.py` & `pymafia-0.2.3/src/pymafia/kolmafia/patch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import _jpype
 import jpype
 import wrapt
 
-PATCH_ENABLED = True
+enabled = True
 
 
 class KoLmafiaError(Exception):
     pass
 
 
 # wrapt's wrap_function_wrapper does not allow specifying "enabled"
@@ -22,17 +22,17 @@
     This patch does the following:
     * Automatically cast method arguments of type int to java.lang.Integer
     * Raise an exception if mafia is in a non-continue state after method invocation
     """
     KoLmafia = jpype.JClass("net.sourceforge.kolmafia.KoLmafia")
 
     def wrapper(wrapped, instance, args, kwargs):
-        global PATCH_ENABLED
+        global enabled
         try:
-            PATCH_ENABLED = False
+            enabled = False
 
             args = [
                 jpype.JInt(arg)
                 if isinstance(arg, int) and not isinstance(arg, bool)
                 else arg
                 for arg in args
             ]
@@ -40,15 +40,11 @@
 
             if not KoLmafia.permitsContinue():
                 KoLmafia.forceContinue()
                 raise KoLmafiaError(KoLmafia.getLastMessage())
 
             return result
         finally:
-            PATCH_ENABLED = True
+            enabled = True
 
-    wrap_function_wrapper(
-        _jpype, "_JMethod.__call__", wrapper, enabled=lambda: PATCH_ENABLED
-    )
-    wrap_function_wrapper(
-        _jpype, "_JClass.__call__", wrapper, enabled=lambda: PATCH_ENABLED
-    )
+    wrap_function_wrapper(_jpype, "_JMethod.__call__", wrapper, enabled=lambda: enabled)
+    wrap_function_wrapper(_jpype, "_JClass.__call__", wrapper, enabled=lambda: enabled)
```

### Comparing `pymafia-0.2.2/src/pymafia/player.py` & `pymafia-0.2.3/src/pymafia/player.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/preference.py` & `pymafia-0.2.3/src/pymafia/preference.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/src/pymafia/utils.py` & `pymafia-0.2.3/src/pymafia/utils.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.2/PKG-INFO` & `pymafia-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymafia
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python module and bridge for reflecting KoLmafia's Java environment
 Home-page: https://github.com/MrFizzyBubbs/pymafia
 License: MIT
 Author: MrFizzyBubbs
 Author-email: MrFizzyBubbs@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -26,25 +26,29 @@
 ```
 pip install pymafia
 ```
 
 *pymafia* uses [JPype](https://github.com/kivy/pyjnius) to reflect KoLmafia's Java environment, so you will need to install a Java Development Kit (JDK) on your operating system — KoLmafia's developers recommend [Adoptium v17](https://adoptium.net/index.html). For information on troubleshooting your Java installation, see [JPype's troubleshooting guide](https://jpype.readthedocs.io/en/latest/install.html#if-it-fails).
 
 ## Usage
-To get started, simply import *pymafia* or any of its components. Doing so will download a KoLmafia jar file (if it is not present in the current working directory) and start a Java Virtual Machine (JVM) with the jar file included in the JVM's classpath. This process can take over a minute depending on your internet connection. You can change the revision of KoLmafia to use by setting the revision in the `pymafia_config` module prior to importing *pymafia*.
+To get started, simply import *pymafia* or any of its components. Doing so will download a KoLmafia jar file (if it is not present in the configured location) and start a Java Virtual Machine (JVM) with the jar file included in the JVM's classpath. This process can take over a minute depending on your internet connection. 
+
+You can choose the revision of KoLmafia to use or location to run it from by setting these properties in the `pymafia_config` module prior to importing *pymafia*. The revision defaults to the last known working revision at the time of release and the location defaults to a folder named "kolmafia" in the current working directory.
 
 ```python
 >>> import pymafia_config
 
 >>> pymafia_config.set_revision(27467)
 
->>> pymafia_config.set_revision("latest")
+>>> pymafia_config.set_location("C:\\Users\\Documents\\kolmafia\\")
+
+>>> import pymafia # Start the JVM
 ```
 
-Once you have set your desired revision, you will most likely want to launch the KoLmafia GUI and login to your character. Both of these actions can be performed using the `utils` module.
+Once you have configured *pymafia* and started, you will most likely want to launch the KoLmafia GUI and login to your character. Both of these actions can be performed using the `utils` module.
 
 ```python
 >>> from pymafia.utils import launch_gui, login
 
 >>> launch_gui()
 
 >>> login("devster6")
@@ -62,15 +66,15 @@
 ```python
 >>> from pymafia.kolmafia import km
 
 >>> km.AdventureResult
 <java class 'net.sourceforge.kolmafia.AdventureResult'>
 ```
 
-The Java classes behave similar to how they do in Java with the exception of returning Python objects when possible. For more information on the type conversions, see [JPype's type matching guide](https://jpype.readthedocs.io/en/latest/userguide.html#type-matching).
+These classes behave similar to how they do in Java with the exception of returning Python objects when possible. For more information on type conversion, see [JPype's type matching guide](https://jpype.readthedocs.io/en/latest/userguide.html#type-matching).
 
 ```
 >>> km.AdventureResult.tallyItem("big rock")
 <java object 'net.sourceforge.kolmafia.AdventureResult'>
 
 >>> km.AdventureResult.tallyItem("big rock").isBountyItem()
 False
@@ -128,14 +132,17 @@
 >>> Coinmaster.NONE
 Coinmaster('none')
 
 >>> Slot.HAT
 Slot('hat')
 ```
 
+### Non-Documented Functionality
+There are  modules and subpackages and available within *pymafia* that have not been described here; I hope to provide comprehensive documentation in the future.
+
 ## Contributing
 To contribute to *pymafia*, you will need to set up a development environment using the following steps:
 1. Install [poetry](https://python-poetry.org/)
 2. Clone this repository
 3. Run `poetry install` inside the cloned repository
```

