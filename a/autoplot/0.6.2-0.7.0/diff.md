# Comparing `tmp/autoplot-0.6.2.tar.gz` & `tmp/autoplot-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoplot-0.6.2.tar", last modified: Mon Apr 24 14:54:45 2023, max compression
+gzip compressed data, was "dist/autoplot-0.7.0.tar", last modified: Wed Jul 19 14:45:40 2023, max compression
```

## Comparing `autoplot-0.6.2.tar` & `autoplot-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:54:45.490496 autoplot-0.6.2/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1456 2023-04-11 14:05:55.000000 autoplot-0.6.2/LICENSE.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     2069 2023-04-24 14:54:45.490496 autoplot-0.6.2/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     1818 2023-04-24 14:22:53.000000 autoplot-0.6.2/README.rst
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:54:45.490496 autoplot-0.6.2/autoplot/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      310 2023-04-24 14:19:03.000000 autoplot-0.6.2/autoplot/__init__.py
--rw-rw-r--   0 jbf       (1210) jbf       (1210)    22099 2023-04-24 14:47:20.000000 autoplot-0.6.2/autoplot/autoplot.py
-drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-04-24 14:54:45.490496 autoplot-0.6.2/autoplot.egg-info/
--rw-rw-r--   0 jbf       (1210) jbf       (1210)     2069 2023-04-24 14:54:45.000000 autoplot-0.6.2/autoplot.egg-info/PKG-INFO
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      232 2023-04-24 14:54:45.000000 autoplot-0.6.2/autoplot.egg-info/SOURCES.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)        1 2023-04-24 14:54:45.000000 autoplot-0.6.2/autoplot.egg-info/dependency_links.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)       13 2023-04-24 14:54:45.000000 autoplot-0.6.2/autoplot.egg-info/requires.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)        9 2023-04-24 14:54:45.000000 autoplot-0.6.2/autoplot.egg-info/top_level.txt
--rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2023-04-24 14:54:45.490496 autoplot-0.6.2/setup.cfg
--rw-rw-r--   0 jbf       (1210) jbf       (1210)      759 2023-04-24 14:47:57.000000 autoplot-0.6.2/setup.py
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-07-19 14:45:40.000000 autoplot-0.7.0/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1664 2023-07-19 14:41:54.000000 autoplot-0.7.0/README.rst
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      759 2023-07-18 09:33:04.000000 autoplot-0.7.0/setup.py
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1456 2023-07-18 09:32:00.000000 autoplot-0.7.0/LICENSE.txt
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-07-19 14:45:40.000000 autoplot-0.7.0/autoplot/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)    23265 2023-07-18 14:11:49.000000 autoplot-0.7.0/autoplot/autoplot.py
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      346 2023-07-18 09:34:37.000000 autoplot-0.7.0/autoplot/__init__.py
+drwxrwxr-x   0 jbf       (1210) jbf       (1210)        0 2023-07-19 14:45:40.000000 autoplot-0.7.0/autoplot.egg-info/
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        1 2023-07-19 14:45:40.000000 autoplot-0.7.0/autoplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       13 2023-07-19 14:45:40.000000 autoplot-0.7.0/autoplot.egg-info/requires.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)        9 2023-07-19 14:45:40.000000 autoplot-0.7.0/autoplot.egg-info/top_level.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1935 2023-07-19 14:45:40.000000 autoplot-0.7.0/autoplot.egg-info/PKG-INFO
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)      232 2023-07-19 14:45:40.000000 autoplot-0.7.0/autoplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)       38 2023-07-19 14:45:40.000000 autoplot-0.7.0/setup.cfg
+-rw-rw-r--   0 jbf       (1210) jbf       (1210)     1935 2023-07-19 14:45:40.000000 autoplot-0.7.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `autoplot-0.6.2/LICENSE.txt` & `autoplot-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoplot-0.6.2/PKG-INFO` & `autoplot-0.7.0/autoplot.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 Metadata-Version: 2.1
 Name: autoplot
-Version: 0.6.2
+Version: 0.7.0
 Summary: Interface to Autoplot Java library
 Home-page: https://github.com/autoplot/python/
 Author: Jeremy Faden
 Author-email: faden@cottagesystems.com
 License: LICENSE.txt
+Platform: UNKNOWN
 License-File: LICENSE.txt
 
-Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can 
-also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
+Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
 Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
 
 Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
 These URIs can be created using the Autoplot application, available at http://autoplot.org/.
 Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
-Helper procedures from the Autoplot package convert QDataSets into ndarrays.
+Helper procedures from the autoplot package convert QDataSets into ndarrays.
 
 Autoplot/Python Interface Tools
 -------------------------------
 
 Install using `pip install autoplot`
 
 .. code:: python
 
   from autoplot import *
 
-  # Download autoplot.jar, if needed, and load it into JPype's classpath.
-  javaaddpath('http://autoplot.org/latest/autoplot.jar')
-  
-  # Create Autoplot Data Set, which is an object that loads and temporarily holds data.
-  apds = APDataSet()
+  # Download autoplot.jar if needed and return Python bridge object
+  org = javaaddpath('http://autoplot.org/latest/autoplot.jar')
 
-  # Set URI which will be loaded.
+  # Create Autoplot Data Set
+  apds = org.autoplot.idlsupport.APDataSet()
+
+  # Set URI
   apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
 
-  # Load the data, initially downloading files into Autoplot's cache.
+  # Get the data
   apds.doGetDataSet()
 
   print(apds.toString())
   # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
   # data: data[dep0=288] (dimensionless)
   # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
 
   # Extract data values
-  vv = to_ndarray(apds)
+  vv = to_ndarray(apds, 'data')
   tt = to_ndarray(apds, 'dep0')
 
   from matplotlib import pyplot as plt
   plt.plot(tt,vv)
   plt.show()
 
 Contact
 -------------------------------
 Jeremy Faden <faden@cottagesystems.com>
 
-See also https://github.com/autoplot/python/wiki
+
+
```

### Comparing `autoplot-0.6.2/README.rst` & `autoplot-0.7.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,46 @@
-Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can 
-also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
+Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
 Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
 
 Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
 These URIs can be created using the Autoplot application, available at http://autoplot.org/.
 Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
-Helper procedures from the Autoplot package convert QDataSets into ndarrays.
+Helper procedures from the autoplot package convert QDataSets into ndarrays.
 
 Autoplot/Python Interface Tools
 -------------------------------
 
 Install using `pip install autoplot`
 
 .. code:: python
 
   from autoplot import *
 
-  # Download autoplot.jar, if needed, and load it into JPype's classpath.
-  javaaddpath('http://autoplot.org/latest/autoplot.jar')
-  
-  # Create Autoplot Data Set, which is an object that loads and temporarily holds data.
-  apds = APDataSet()
+  # Download autoplot.jar if needed and return Python bridge object
+  org = javaaddpath('http://autoplot.org/latest/autoplot.jar')
 
-  # Set URI which will be loaded.
+  # Create Autoplot Data Set
+  apds = org.autoplot.idlsupport.APDataSet()
+
+  # Set URI
   apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
 
-  # Load the data, initially downloading files into Autoplot's cache.
+  # Get the data
   apds.doGetDataSet()
 
   print(apds.toString())
   # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
   # data: data[dep0=288] (dimensionless)
   # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
 
   # Extract data values
-  vv = to_ndarray(apds)
+  vv = to_ndarray(apds, 'data')
   tt = to_ndarray(apds, 'dep0')
 
   from matplotlib import pyplot as plt
   plt.plot(tt,vv)
   plt.show()
 
 Contact
 -------------------------------
 Jeremy Faden <faden@cottagesystems.com>
 
-See also https://github.com/autoplot/python/wiki
```

### Comparing `autoplot-0.6.2/autoplot/autoplot.py` & `autoplot-0.7.0/autoplot/autoplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,46 @@
     return '0.6.2'
 
 
 def printNoNewline(s):
     print(s, end=' ')
 
 
+def init(url='', jdwpPort=-1):
+    """Start up JVM, import JAR at URL.
+      com= jpype.JPackage('com') 
+    can be used to the com package into the Python namespace.
+    Example:
+      javaaddpath('http://autoplot.org/devel/autoplot.jar')
+    if no url is provided, then the default http://autoplot.org/latest/autoplot.jar is used.
+    """
+    javaaddpath(url='', jdwpPort=jdwpPort)
+
+def handleShutdown():
+    'shutdown hook which shuts down the JVM.'
+    print( 'shut down JVM...' )
+    import jpype
+    System=jpype.JClass('java.lang.System')
+    System.exit(-15)
+    
+def start():
+    """start up the JVM and launch Autoplot.  This also disables Java's system.exit, which also shuts down Python."""
+    #javaaddpath(url='https://ci-pw.physics.uiowa.edu/job/autoplot-release-2022/lastSuccessfulBuild/artifact/autoplot/Autoplot/dist/autoplot.jar')
+    javaaddpath()
+    import jpype
+    AppManager=jpype.JClass('org.autoplot.AppManager')    
+    AppManager.getInstance().setAllowExit(False)
+    AutoplotUI=jpype.JClass('org.autoplot.AutoplotUI')
+    AutoplotUI.main([])
+    import atexit
+    atexit.register(handleShutdown)
+    import time
+    time.sleep(5)
+
+    
 def javaaddpath(url='', jdwpPort=-1):
     """Start up JVM, import JAR at URL.
       com= jpype.JPackage('com') 
     can be used to the com package into the Python namespace.
     Example:
       javaaddpath('http://autoplot.org/devel/autoplot.jar')
     if no url is provided, then the default http://autoplot.org/latest/autoplot.jar is used.
```

### Comparing `autoplot-0.6.2/autoplot.egg-info/PKG-INFO` & `autoplot-0.7.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 Metadata-Version: 2.1
 Name: autoplot
-Version: 0.6.2
+Version: 0.7.0
 Summary: Interface to Autoplot Java library
 Home-page: https://github.com/autoplot/python/
 Author: Jeremy Faden
 Author-email: faden@cottagesystems.com
 License: LICENSE.txt
+Platform: UNKNOWN
 License-File: LICENSE.txt
 
-Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can 
-also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
+Autoplot is a Java application which can read data from many sources, such as ASCII tables, NASA CDF files, and HDF5 files.  It can also read data from data servers, such as the server at NASA/Goddard/CDAWeb, Das2Servers used by the Radio and
 Plasma Wave Group at the University of Iowa, and servers supporting the HAPI API.
 
 Autoplot identifies data using "URIs", which are one-line strings containing a data source ID and configuration to read the data.  
 These URIs can be created using the Autoplot application, available at http://autoplot.org/.
 Data are read into a standard data model, QDataSet, which is easily adapted to Python using "JPype".
-Helper procedures from the Autoplot package convert QDataSets into ndarrays.
+Helper procedures from the autoplot package convert QDataSets into ndarrays.
 
 Autoplot/Python Interface Tools
 -------------------------------
 
 Install using `pip install autoplot`
 
 .. code:: python
 
   from autoplot import *
 
-  # Download autoplot.jar, if needed, and load it into JPype's classpath.
-  javaaddpath('http://autoplot.org/latest/autoplot.jar')
-  
-  # Create Autoplot Data Set, which is an object that loads and temporarily holds data.
-  apds = APDataSet()
+  # Download autoplot.jar if needed and return Python bridge object
+  org = javaaddpath('http://autoplot.org/latest/autoplot.jar')
 
-  # Set URI which will be loaded.
+  # Create Autoplot Data Set
+  apds = org.autoplot.idlsupport.APDataSet()
+
+  # Set URI
   apds.setDataSetURI('http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0')
 
-  # Load the data, initially downloading files into Autoplot's cache.
+  # Get the data
   apds.doGetDataSet()
 
   print(apds.toString())
   # http://autoplot.org/data/swe-np.xls?column=data&depend0=dep0
   # data: data[dep0=288] (dimensionless)
   # dep0: dep0[288] (days since 1899-12-30T00:00:00.000Z) (DEPEND_0)
 
   # Extract data values
-  vv = to_ndarray(apds)
+  vv = to_ndarray(apds, 'data')
   tt = to_ndarray(apds, 'dep0')
 
   from matplotlib import pyplot as plt
   plt.plot(tt,vv)
   plt.show()
 
 Contact
 -------------------------------
 Jeremy Faden <faden@cottagesystems.com>
 
-See also https://github.com/autoplot/python/wiki
+
+
```

### Comparing `autoplot-0.6.2/setup.py` & `autoplot-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = ["jpype1","numpy"]
 
 if sys.argv[1] == 'develop':
     install_requires.append("pytest")
 
 setup(
     name='autoplot',
-    version='0.6.2',
+    version='0.7.0',
     author='Jeremy Faden',
     author_email='faden@cottagesystems.com',
     packages=find_packages(), 
     url='https://github.com/autoplot/python/',
     license='LICENSE.txt',
     description='Interface to Autoplot Java library',
     long_description=open('README.rst').read(),
```

