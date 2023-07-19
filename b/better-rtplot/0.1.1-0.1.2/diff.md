# Comparing `tmp/better_rtplot-0.1.1.tar.gz` & `tmp/better_rtplot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_rtplot-0.1.1.tar", max compression
+gzip compressed data, was "better_rtplot-0.1.2.tar", max compression
```

## Comparing `better_rtplot-0.1.1.tar` & `better_rtplot-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-06-28 20:16:53.824192 better_rtplot-0.1.1/LICENSE
--rw-r--r--   0        0        0     8211 2023-06-28 19:48:45.454291 better_rtplot-0.1.1/README.md
--rw-r--r--   0        0        0      439 2023-07-17 19:14:25.480852 better_rtplot-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7588 2023-07-17 19:06:32.364262 better_rtplot-0.1.1/rtplot/client.py
--rw-r--r--   0        0        0     6240 2023-03-09 21:43:09.016987 better_rtplot-0.1.1/rtplot/example_code.py
--rw-r--r--   0        0        0     1062 2023-07-13 18:31:13.985659 better_rtplot-0.1.1/rtplot/plot_log.py
--rw-r--r--   0        0        0       71 2023-03-09 21:43:09.016987 better_rtplot-0.1.1/rtplot/saved_plots/.gitignore
--rw-r--r--   0        0        0    22802 2023-07-17 19:02:58.496380 better_rtplot-0.1.1/rtplot/server.py
--rw-r--r--   0        0        0     8860 1970-01-01 00:00:00.000000 better_rtplot-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2023-06-28 20:16:53.824192 better_rtplot-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0     7489 2023-07-19 02:18:57.469955 better_rtplot-0.1.2/README.md
+-rwxr-xr-x   0        0        0      497 2023-07-19 03:43:12.471342 better_rtplot-0.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0     7588 2023-07-17 19:06:32.364262 better_rtplot-0.1.2/rtplot/client.py
+-rwxr-xr-x   0        0        0     6240 2023-03-09 21:43:09.016987 better_rtplot-0.1.2/rtplot/example_code.py
+-rwxr-xr-x   0        0        0     1062 2023-07-13 18:31:13.985659 better_rtplot-0.1.2/rtplot/plot_log.py
+-rwxr-xr-x   0        0        0       71 2023-03-09 21:43:09.016987 better_rtplot-0.1.2/rtplot/saved_plots/.gitignore
+-rwxr-xr-x   0        0        0    22802 2023-07-17 19:02:58.496380 better_rtplot-0.1.2/rtplot/server.py
+-rw-r--r--   0        0        0     8138 1970-01-01 00:00:00.000000 better_rtplot-0.1.2/PKG-INFO
```

### Comparing `better_rtplot-0.1.1/LICENSE` & `better_rtplot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.1/README.md` & `better_rtplot-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,42 @@
+Metadata-Version: 2.1
+Name: better-rtplot
+Version: 0.1.2
+Summary: 
+License: GPL V3.0
+Author: jmontp
+Author-email: jmontp@umich.edu
+Requires-Python: >=3.8,<3.11
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: numpy (==1.23.5)
+Requires-Dist: pandas (==1.5.3)
+Requires-Dist: pyarrow (==11.0.0)
+Requires-Dist: pyqtgraph (==0.13.0)
+Requires-Dist: pyside6 (<=6.4.0)
+Requires-Dist: pyzmq (==25.0.0)
+Description-Content-Type: text/markdown
+
 ![Logo of the project](https://github.com/jmontp/rtplot/blob/master/.images/signature-stationery.png)
 
 # Real Time Plotting with pyqtgraph and ZMQ
 
 The point of this module is to be able to plot remotely over socket protocols using the [ZMQ library](https://zeromq.org/). The use cases that I have in mind is plotting information from the raspberry pi to a host computer so that they can plot the data. This is very useful for setting up real time plots given pyqtgraph's performance. This can also be used to plot local information in real time by using the localhost as the address to publish/subscribe data from. 
 
 The main highlight in this plotter are the following:
 * **Fast Performance**. Can do 500+ fps on one trace using an i7-9750H processor
 * **Remote Plot Customizability**. The plot configuration is defined by the provider of the data. E.g. if you are using a pi to collect data, the plot configuration is also stored on the pi so you only have to change code in one location 
 * **Save data**. Once you plot the data, you can save it locally by clicking one button.
 
 
 # Install 
-
-Run in the parent folder containing the repo (requires [setuptools](https://pypi.org/project/setuptools/))
-
-> python3 -m pip install -e rtplot/
-
-
-# Dependencies
-
-| Data-Plotting Computer  | Both Computers|
-| ------------- |:-------------:|
-| [pyqtgraph](https://pyqtgraph.readthedocs.io/en/latest/installation.html) ```pip3 install pyqtgraph ``` ```pip3 install pyside6``` | [PyZMQ](https://zeromq.org/languages/python/) ```pip3 install pyzmq```  |
-| [Pandas](https://pandas.pydata.org/docs/getting_started/install.html) ```pip3 install pandas```      |       |
-| [Pyarrow](https://arrow.apache.org/docs/python/install.html) ```pip3 install pyarrow``` |      |
-
-One-liner to install everything:
-```pip3 install pyarrow pyqtgraph pyside6 pyzmq pandas```
+```pip install better-rtplot```
 
 
 If you are using WSL, you need to install an xorg server such as [vcXsrv](https://sourceforge.net/projects/vcxsrv/)
 
 # How to use
 
 ### Step 1: On the computer that will be used to plot run:
@@ -180,7 +186,8 @@
 # [Example Code](https://github.com/jmontp/rtplot/blob/master/rtplot/example_code.py)
 
 
 # Example Image
 ![alt text](https://github.com/jmontp/rtplot/blob/master/.images/rtplot_example1.png "Example 1")
 
 ![alt text](https://github.com/jmontp/rtplot/blob/master/.images/rtplot_example2.png "Example 2")
+
```

### Comparing `better_rtplot-0.1.1/rtplot/client.py` & `better_rtplot-0.1.2/rtplot/client.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.1/rtplot/example_code.py` & `better_rtplot-0.1.2/rtplot/example_code.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.1/rtplot/plot_log.py` & `better_rtplot-0.1.2/rtplot/plot_log.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.1/rtplot/server.py` & `better_rtplot-0.1.2/rtplot/server.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.1/PKG-INFO` & `better_rtplot-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,21 @@
-Metadata-Version: 2.1
-Name: better-rtplot
-Version: 0.1.1
-Summary: 
-License: GPL V3.0
-Author: jmontp
-Author-email: jmontp@umich.edu
-Requires-Python: >=3.8,<3.11
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: numpy (==1.23.5)
-Requires-Dist: pandas (==1.5.3)
-Requires-Dist: pyarrow (==11.0.0)
-Requires-Dist: pyqtgraph (==0.13.0)
-Requires-Dist: pyside6 (<=6.4.0)
-Requires-Dist: pyzmq (==25.0.0)
-Description-Content-Type: text/markdown
-
 ![Logo of the project](https://github.com/jmontp/rtplot/blob/master/.images/signature-stationery.png)
 
 # Real Time Plotting with pyqtgraph and ZMQ
 
 The point of this module is to be able to plot remotely over socket protocols using the [ZMQ library](https://zeromq.org/). The use cases that I have in mind is plotting information from the raspberry pi to a host computer so that they can plot the data. This is very useful for setting up real time plots given pyqtgraph's performance. This can also be used to plot local information in real time by using the localhost as the address to publish/subscribe data from. 
 
 The main highlight in this plotter are the following:
 * **Fast Performance**. Can do 500+ fps on one trace using an i7-9750H processor
 * **Remote Plot Customizability**. The plot configuration is defined by the provider of the data. E.g. if you are using a pi to collect data, the plot configuration is also stored on the pi so you only have to change code in one location 
 * **Save data**. Once you plot the data, you can save it locally by clicking one button.
 
 
 # Install 
-
-Run in the parent folder containing the repo (requires [setuptools](https://pypi.org/project/setuptools/))
-
-> python3 -m pip install -e rtplot/
-
-
-# Dependencies
-
-| Data-Plotting Computer  | Both Computers|
-| ------------- |:-------------:|
-| [pyqtgraph](https://pyqtgraph.readthedocs.io/en/latest/installation.html) ```pip3 install pyqtgraph ``` ```pip3 install pyside6``` | [PyZMQ](https://zeromq.org/languages/python/) ```pip3 install pyzmq```  |
-| [Pandas](https://pandas.pydata.org/docs/getting_started/install.html) ```pip3 install pandas```      |       |
-| [Pyarrow](https://arrow.apache.org/docs/python/install.html) ```pip3 install pyarrow``` |      |
-
-One-liner to install everything:
-```pip3 install pyarrow pyqtgraph pyside6 pyzmq pandas```
+```pip install better-rtplot```
 
 
 If you are using WSL, you need to install an xorg server such as [vcXsrv](https://sourceforge.net/projects/vcxsrv/)
 
 # How to use
 
 ### Step 1: On the computer that will be used to plot run:
@@ -201,8 +165,7 @@
 # [Example Code](https://github.com/jmontp/rtplot/blob/master/rtplot/example_code.py)
 
 
 # Example Image
 ![alt text](https://github.com/jmontp/rtplot/blob/master/.images/rtplot_example1.png "Example 1")
 
 ![alt text](https://github.com/jmontp/rtplot/blob/master/.images/rtplot_example2.png "Example 2")
-
```

