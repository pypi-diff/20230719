# Comparing `tmp/fileformats_medimage-0.4.0.tar.gz` & `tmp/fileformats_medimage-0.4.1.tar.gz`

## Comparing `fileformats_medimage-0.4.0.tar` & `fileformats_medimage-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.codespell-ignorewords
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.coveragerc
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/_version.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/base.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/dicom.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/diffusion.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/misc.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/mrtrix.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/nifti.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/raw.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/tests/test_dicom.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/fileformats/medimage/tests/test_nifti.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/LICENSE
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/README.rst
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    19004 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/.codespell-ignorewords
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/.coveragerc
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/fileformats/medimage/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/fileformats/medimage/_version.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/fileformats/medimage/base.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/fileformats/medimage/dicom.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/fileformats/medimage/diffusion.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/fileformats/medimage/misc.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/fileformats/medimage/mrtrix3.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/fileformats/medimage/nifti.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/fileformats/medimage/raw.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/fileformats/medimage/tests/test_dicom.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/fileformats/medimage/tests/test_nifti.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/README.rst
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    18977 2020-02-02 00:00:00.000000 fileformats_medimage-0.4.1/PKG-INFO
```

### Comparing `fileformats_medimage-0.4.0/.pre-commit-config.yaml` & `fileformats_medimage-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.0/conftest.py` & `fileformats_medimage-0.4.1/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.0/.github/workflows/publish.yml` & `fileformats_medimage-0.4.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.0/.github/workflows/tests.yml` & `fileformats_medimage-0.4.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.0/fileformats/medimage/__init__.py` & `fileformats_medimage-0.4.1/fileformats/medimage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Nifti,
     Nifti1,
     Nifti2,
     NiftiGz,
     NiftiX,
     NiftiGzX,
 )
-from .mrtrix import MrtrixImage, MrtrixImageHeader
+from .mrtrix3 import MrtrixImage, MrtrixImageHeader
 from .diffusion import (
     DwiEncoding,
     MrtrixTrack,
     Bvec,
     Bfile,
     NiftiBvec,
     NiftiGzBvec,
```

### Comparing `fileformats_medimage-0.4.0/fileformats/medimage/mrtrix.py` & `fileformats_medimage-0.4.1/fileformats/medimage/mrtrix3.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from pathlib import Path
 from fileformats.core import mark
 from fileformats.generic import File
 from fileformats.core.mixin import WithMagicNumber
 from fileformats.numeric import DataFile
 from fileformats.core.exceptions import FormatMismatchError
-from fileformats.core.utils import MissingExtendedDependency
 from .misc import MedicalImage
-try:
-    import numpy
-except ImportError:
-    numpy = MissingExtendedDependency("numpy", __name__)
 
 
 class BaseMrtrixImage(WithMagicNumber, MedicalImage, File):
 
     magic_number = b"mrtrix image\n"
     binary = True
 
@@ -67,24 +62,14 @@
     def vox_sizes(self):
         return self.metadata["vox"]
 
     @property
     def dims(self):
         return self.metadata["dim"]
 
-    @property
-    def data_array(self):
-        data = self.read_contents(offset=self.data_offset)
-        array = numpy.asarray(data)
-        data_array = array.reshape(self.dims)
-        raise NotImplementedError(
-            "Need to work out how to use the metadata to read the array in the correct order"
-        )
-        return data_array
-
 
 class MrtrixImage(BaseMrtrixImage):
 
     ext = ".mif"
 
     @mark.check
     def check_data_file(self):
```

### Comparing `fileformats_medimage-0.4.0/fileformats/medimage/raw.py` & `fileformats_medimage-0.4.1/fileformats/medimage/raw.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.0/LICENSE` & `fileformats_medimage-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.0/README.rst` & `fileformats_medimage-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.4.0/pyproject.toml` & `fileformats_medimage-0.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 [project]
 name = "fileformats-medimage"
 description = "Classes for representing various medical imaging file formats in Python classes for use in type hinting in data workflows"
 readme = "README.rst"
 requires-python = ">=3.8"
 dependencies = [
-    "numpy >= 1.24",
-    "fileformats >=0.4.0",
+    "fileformats >=0.7.1",
 ]
 license = {file = "LICENSE"}
 authors = [
     {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
 ]
 maintainers = [
     {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
```

### Comparing `fileformats_medimage-0.4.0/PKG-INFO` & `fileformats_medimage-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-medimage
-Version: 0.4.0
+Version: 0.4.1
 Summary: Classes for representing various medical imaging file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -107,16 +107,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: fileformats>=0.4.0
-Requires-Dist: numpy>=1.24
+Requires-Dist: fileformats>=0.7.1
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
```

