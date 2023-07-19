# Comparing `tmp/pytest_cmake-0.2.1.tar.gz` & `tmp/pytest_cmake-0.3.0.tar.gz`

## Comparing `pytest_cmake-0.2.1.tar` & `pytest_cmake-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pytest_cmake-0.2.1/build_backend.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 pytest_cmake-0.2.1/build_config.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 pytest_cmake-0.2.1/cmake/FindPytest.cmake
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 pytest_cmake-0.2.1/cmake/PytestAddTests.cmake
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 pytest_cmake-0.2.1/setup.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pytest_cmake-0.2.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytest_cmake-0.2.1/LICENSE
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 pytest_cmake-0.2.1/README.md
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 pytest_cmake-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pytest_cmake-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pytest_cmake-0.3.0/build_backend.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 pytest_cmake-0.3.0/build_config.py
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 pytest_cmake-0.3.0/cmake/FindPytest.cmake
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pytest_cmake-0.3.0/cmake/PytestAddTests.cmake
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 pytest_cmake-0.3.0/setup.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pytest_cmake-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pytest_cmake-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 pytest_cmake-0.3.0/README.md
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 pytest_cmake-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pytest_cmake-0.3.0/PKG-INFO
```

### Comparing `pytest_cmake-0.2.1/build_config.py` & `pytest_cmake-0.3.0/build_config.py`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.2.1/cmake/FindPytest.cmake` & `pytest_cmake-0.3.0/cmake/FindPytest.cmake`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         PROPERTIES
             IMPORTED_LOCATION "${PYTEST_EXECUTABLE}")
 
     function(pytest_discover_tests NAME)
         cmake_parse_arguments(
             PARSE_ARGV 1 "" ""
             "WORKING_DIRECTORY;TRIM_FROM_NAME;BUNDLE_TESTS"
-            "LIBRARY_PATH_PREPEND;PYTHON_PATH_PREPEND;DEPENDS"
+            "LIBRARY_PATH_PREPEND;PYTHON_PATH_PREPEND;ENVIRONMENT;DEPENDS"
         )
 
         # Set library path depending on the platform.
         if (CMAKE_SYSTEM_NAME STREQUAL Windows)
             set(LIB_ENV_PATH PATH)
             set(_env_sep "\\\;")
         elseif(CMAKE_SYSTEM_NAME STREQUAL Darwin)
@@ -115,14 +115,15 @@
             -D "TEST_GROUP_NAME=${NAME}"
             -D "BUNDLE_TESTS=${_BUNDLE_TESTS}"
             -D "LIB_ENV_PATH=${LIB_ENV_PATH}"
             -D "LIBRARY_PATH=${libpath}"
             -D "PYTHON_PATH=${pythonpath}"
             -D "TRIM_FROM_NAME=${_TRIM_FROM_NAME}"
             -D "WORKING_DIRECTORY=${_WORKING_DIRECTORY}"
+            -D "ENVIRONMENT=${_ENVIRONMENT}"
             -D "PROJECT_SOURCE_DIR=${PROJECT_SOURCE_DIR}"
             -D "CTEST_FILE=${_tests_file}"
             -P "${CMAKE_CURRENT_FUNCTION_LIST_DIR}/PytestAddTests.cmake")
 
         # Add discovered tests to directory TEST_INCLUDE_FILES
         set_property(DIRECTORY
             APPEND PROPERTY TEST_INCLUDE_FILES "${_tests_file}")
```

### Comparing `pytest_cmake-0.2.1/cmake/PytestAddTests.cmake` & `pytest_cmake-0.3.0/cmake/PytestAddTests.cmake`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,24 @@
             "set_tests_properties(\n"
             "     \"${TEST_GROUP_NAME}\"\n"
             "     APPEND PROPERTIES\n"
             "     ENVIRONMENT \"PYTHONPATH=${PYTHON_PATH}\"\n"
             ")\n"
         )
 
+        foreach(env ${ENVIRONMENT})
+            string(APPEND _content
+                "set_tests_properties(\n"
+                "     \"${TEST_GROUP_NAME}\"\n"
+                "     APPEND PROPERTIES\n"
+                "     ENVIRONMENT ${env}\n"
+                ")\n"
+            )
+        endforeach()
+
     else()
         # Set environment for collecting tests.
         set(ENV{${LIB_ENV_PATH}} "${LIBRARY_PATH}")
         set(ENV{PYTHONPATH} "${PYTHON_PATH}")
 
         execute_process(
             COMMAND ${PYTEST_EXECUTABLE}
@@ -85,14 +95,24 @@
                 "set_tests_properties(\n"
                 "     \"${test_name}\"\n"
                 "     APPEND PROPERTIES\n"
                 "     ENVIRONMENT \"PYTHONPATH=${PYTHON_PATH}\"\n"
                 ")\n"
             )
 
+            foreach(env ${ENVIRONMENT})
+                string(APPEND _content
+                    "set_tests_properties(\n"
+                    "     \"${test_name}\"\n"
+                    "     APPEND PROPERTIES\n"
+                    "     ENVIRONMENT ${env}\n"
+                    ")\n"
+                )
+            endforeach()
+
         endforeach()
 
         if(NOT _content)
             message(WARNING "No Python tests have been discovered.")
         endif()
     endif()
```

### Comparing `pytest_cmake-0.2.1/setup.py` & `pytest_cmake-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         subprocess.call(["cmake", "-P", str(script_path), "-VV"])
         return install.run(self)
 
 
 setup(
     name="pytest-cmake",
-    version="0.2.1",
+    version="0.3.0",
     data_files=[
         (
             "share/Pytest/cmake",
             [
                 "build/PytestConfig.cmake",
                 "build/PytestConfigVersion.cmake",
                 "cmake/FindPytest.cmake",
```

### Comparing `pytest_cmake-0.2.1/.gitignore` & `pytest_cmake-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.2.1/LICENSE` & `pytest_cmake-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.2.1/README.md` & `pytest_cmake-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_cmake-0.2.1/pyproject.toml` & `pytest_cmake-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "cmake >= 3.20, < 3.26"
 ]
 build-backend = "build_backend"
 backend-path = ["."]
 
 [project]
 name = "pytest-cmake"
-version = "0.2.1"
+version = "0.3.0"
 description = "Provide CMake module for Pytest"
 readme = "README.md"
 requires-python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, <4"
 license = {file = "LICENSE"}
 keywords = ["cmake", "pytest", "development"]
 authors = [
     {name = "Jeremy Retailleau", email = "jeremy.retailleau@gmail.com" }
```

### Comparing `pytest_cmake-0.2.1/PKG-INFO` & `pytest_cmake-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-cmake
-Version: 0.2.1
+Version: 0.3.0
 Summary: Provide CMake module for Pytest
 Author-email: Jeremy Retailleau <jeremy.retailleau@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Jeremy Retailleau
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

