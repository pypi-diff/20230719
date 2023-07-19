# Comparing `tmp/sphinxcontrib-xlsxtable-0.1.9.dev20200315.tar.gz` & `tmp/sphinxcontrib-xlsxtable-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sphinxcontrib-xlsxtable-0.1.9.dev20200315.tar", last modified: Sun Mar 15 06:55:04 2020, max compression
+gzip compressed data, was "dist\sphinxcontrib-xlsxtable-1.0.0.tar", last modified: Sun Jul 19 12:54:46 2020, max compression
```

## Comparing `sphinxcontrib-xlsxtable-0.1.9.dev20200315.tar` & `sphinxcontrib-xlsxtable-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxrwx   0        0        0        0 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/
--rw-rw-rw-   0        0        0      288 2020-03-15 01:24:14.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1087 2020-03-03 12:57:07.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/LICENSE
--rw-rw-rw-   0        0        0       54 2020-03-11 14:09:26.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/MANIFEST.in
--rw-rw-rw-   0        0        0     2421 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/PKG-INFO
--rw-rw-rw-   0        0        0      999 2020-03-11 12:53:48.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/README.rst
--rw-rw-rw-   0        0        0       95 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/setup.cfg
--rw-rw-rw-   0        0        0     1338 2020-03-15 06:52:50.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/setup.py
-drwxrwxrwx   0        0        0        0 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib/
--rw-rw-rw-   0        0        0      380 2020-03-08 01:51:57.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib/__init__.py
-drwxrwxrwx   0        0        0        0 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib/xlsxtable/
--rw-rw-rw-   0        0        0       26 2020-03-15 00:14:27.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib/xlsxtable/__init__.py
--rw-rw-rw-   0        0        0     4911 2020-03-14 14:05:13.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib/xlsxtable/xlsx2gridtable.py
--rw-rw-rw-   0        0        0     1729 2020-03-15 06:52:56.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib/xlsxtable/xlsxtable.py
-drwxrwxrwx   0        0        0        0 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib_xlsxtable.egg-info/
--rw-rw-rw-   0        0        0     2421 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib_xlsxtable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib_xlsxtable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib_xlsxtable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib_xlsxtable.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0        2 2020-03-08 01:54:19.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib_xlsxtable.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib_xlsxtable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2020-03-15 06:55:04.000000 sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib_xlsxtable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/
+-rw-rw-rw-   0        0        0      593 2020-07-19 12:53:29.000000 sphinxcontrib-xlsxtable-1.0.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1087 2020-03-03 12:57:07.000000 sphinxcontrib-xlsxtable-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       54 2020-03-11 14:09:26.000000 sphinxcontrib-xlsxtable-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5873 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3307 2020-07-19 07:45:18.000000 sphinxcontrib-xlsxtable-1.0.0/README.rst
+-rw-rw-rw-   0        0        0       83 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1401 2020-07-19 12:53:29.000000 sphinxcontrib-xlsxtable-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/
+-rw-rw-rw-   0        0        0      380 2020-03-08 01:51:57.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/__init__.py
+drwxrwxrwx   0        0        0        0 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/xlsxtable/
+-rw-rw-rw-   0        0        0      151 2020-03-29 11:12:05.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/xlsxtable/__init__.py
+-rw-rw-rw-   0        0        0       55 2020-03-29 11:12:05.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/xlsxtable/__main__.py
+-rw-rw-rw-   0        0        0     8710 2020-07-19 08:09:34.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/xlsxtable/xlsx2gridtable.py
+-rw-rw-rw-   0        0        0     2381 2020-07-19 12:53:29.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib/xlsxtable/xlsxtable.py
+drwxrwxrwx   0        0        0        0 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/
+-rw-rw-rw-   0        0        0     5873 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      589 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0        2 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       30 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2020-07-19 12:54:45.000000 sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-07-19 12:54:46.000000 sphinxcontrib-xlsxtable-1.0.0/test/
+-rw-rw-rw-   0        0        0     4518 2020-07-19 08:14:11.000000 sphinxcontrib-xlsxtable-1.0.0/test/test.py
```

### Comparing `sphinxcontrib-xlsxtable-0.1.9.dev20200315/LICENSE` & `sphinxcontrib-xlsxtable-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-xlsxtable-0.1.9.dev20200315/setup.py` & `sphinxcontrib-xlsxtable-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,39 +4,40 @@
 
 long_desc = ''
 with open("README.rst", "r") as fh:
     long_desc = fh.read()
 
 setup(
     name='sphinxcontrib-xlsxtable',
-    version='0.1.9',
+    version='1.0.0',
     url='https://github.com/kkAyataka/sphinxcontrib-xlsxtable',
     download_url='http://pypi.python.org/pypi/sphinxcontrib-xlsxtable',
     license='MIT',
     author='kkAyataka',
     author_email='kk.ayataka@gmail.com',
     description='A sphinx extension for making table from Excel file',
     long_description=long_desc,
     long_description_content_type='text/x-rst',
     zip_safe=False,
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.0',
         'Framework :: Sphinx :: Extension',
         'Topic :: Documentation',
         'Topic :: Utilities',
     ],
     platforms='any',
-    packages=find_packages(),
+    packages=find_packages(exclude=['test', 'test.*']),
     include_package_data=True,
     install_requires=[
         'Sphinx >= 2.0.0',
         'openpyxl >= 3.0.0',
     ],
     namespace_packages=['sphinxcontrib'],
+    test_suite='test',
 )
```

### Comparing `sphinxcontrib-xlsxtable-0.1.9.dev20200315/sphinxcontrib_xlsxtable.egg-info/SOURCES.txt` & `sphinxcontrib-xlsxtable-1.0.0/sphinxcontrib_xlsxtable.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 sphinxcontrib/__init__.py
 sphinxcontrib/xlsxtable/__init__.py
+sphinxcontrib/xlsxtable/__main__.py
 sphinxcontrib/xlsxtable/xlsx2gridtable.py
 sphinxcontrib/xlsxtable/xlsxtable.py
 sphinxcontrib_xlsxtable.egg-info/PKG-INFO
 sphinxcontrib_xlsxtable.egg-info/SOURCES.txt
 sphinxcontrib_xlsxtable.egg-info/dependency_links.txt
 sphinxcontrib_xlsxtable.egg-info/namespace_packages.txt
 sphinxcontrib_xlsxtable.egg-info/not-zip-safe
 sphinxcontrib_xlsxtable.egg-info/requires.txt
-sphinxcontrib_xlsxtable.egg-info/top_level.txt
+sphinxcontrib_xlsxtable.egg-info/top_level.txt
+test/test.py
```

