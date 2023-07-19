# Comparing `tmp/scargo-1.6.0.tar.gz` & `tmp/scargo-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scargo-1.6.0.tar", last modified: Wed May 31 13:51:20 2023, max compression
+gzip compressed data, was "scargo-1.6.1.tar", last modified: Wed Jul 19 10:03:34 2023, max compression
```

## Comparing `scargo-1.6.0.tar` & `scargo-1.6.1.tar`

### file list

```diff
@@ -1,95 +1,96 @@
--rw-r--r--   0        0        0     4508 2023-05-31 13:51:14.577332 scargo-1.6.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     1066 2023-05-31 13:51:14.577332 scargo-1.6.0/LICENSE
--rw-r--r--   0        0        0     2494 2023-05-31 13:51:14.581332 scargo-1.6.0/README.md
--rw-r--r--   0        0        0     2748 2023-05-31 13:51:14.589332 scargo-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      108 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/__init__.py
--rwxr-xr-x   0        0        0    19734 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/certs/certGen.sh
--rwxr-xr-x   0        0        0     5226 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/certs/generateAllCertificates.sh
--rw-r--r--   0        0        0     3967 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/certs/openssl_device_intermediate_ca.cnf
--rw-r--r--   0        0        0     3957 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/certs/openssl_root_ca.cnf
--rw-r--r--   0        0        0      698 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/clang_utils.py
--rw-r--r--   0        0        0    12830 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/cli.py
--rw-r--r--   0        0        0       86 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/commands/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/commands/build.py
--rw-r--r--   0        0        0    12319 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/commands/check.py
--rw-r--r--   0        0        0     1142 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/clean.py
--rw-r--r--   0        0        0     4168 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/debug.py
--rw-r--r--   0        0        0     3402 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/doc.py
--rw-r--r--   0        0        0     3286 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/docker.py
--rw-r--r--   0        0        0     1124 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/fix.py
--rw-r--r--   0        0        0     3835 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/flash.py
--rw-r--r--   0        0        0     6677 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/gen.py
--rw-r--r--   0        0        0     2857 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/new.py
--rw-r--r--   0        0        0     3405 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/publish.py
--rw-r--r--   0        0        0     1688 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/run.py
--rw-r--r--   0        0        0     3651 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/test.py
--rw-r--r--   0        0        0     4419 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/update.py
--rw-r--r--   0        0        0      228 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/version.py
--rw-r--r--   0        0        0     6707 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/config.py
--rw-r--r--   0        0        0     2255 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/config_utils.py
--rw-r--r--   0        0        0     2174 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/docker_utils.py
--rw-r--r--   0        0        0       86 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/__init__.py
--rw-r--r--   0        0        0     1658 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/base_gen.py
--rw-r--r--   0        0        0      441 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/cicd_gen.py
--rw-r--r--   0        0        0       86 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/clang_parser/__init__.py
--rw-r--r--   0        0        0     2251 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/clang_parser/data_classes.py
--rw-r--r--   0        0        0     1197 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/clang_parser/header_parser.py
--rw-r--r--   0        0        0     2385 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/clang_parser/params_extractor.py
--rw-r--r--   0        0        0      395 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/cmake_gen.py
--rw-r--r--   0        0        0      569 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/conan_gen.py
--rw-r--r--   0        0        0     2468 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/cpp_gen.py
--rw-r--r--   0        0        0     3186 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/docker_gen.py
--rw-r--r--   0        0        0     1115 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/env_gen.py
--rwxr-xr-x   0        0        0     1607 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/mock_gen.py
--rw-r--r--   0        0        0      454 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/readme_gen.py
--rw-r--r--   0        0        0     4834 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/.gitlab-ci.yml.j2
--rw-r--r--   0        0        0     1580 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/CMakeLists.txt.j2
--rw-r--r--   0        0        0     4275 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/README.md.j2
--rw-r--r--   0        0        0     1693 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/conan/conanfile.py.j2
--rw-r--r--   0        0        0     1464 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/conan/conanfiletest.j2
--rw-r--r--   0        0        0      150 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
--rw-r--r--   0        0        0     2423 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
--rw-r--r--   0        0        0      886 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2
--rw-r--r--   0        0        0      181 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/lib.cpp.j2
--rw-r--r--   0        0        0      213 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/lib.h.j2
--rw-r--r--   0        0        0      715 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/main.cpp.j2
--rw-r--r--   0        0        0      159 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2
--rw-r--r--   0        0        0     2128 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
--rw-r--r--   0        0        0      754 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
--rw-r--r--   0        0        0       49 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-x86.j2
--rw-r--r--   0        0        0     2363 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile.j2
--rw-r--r--   0        0        0      158 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/devcontainer.json.j2
--rw-r--r--   0        0        0     1000 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2
--rw-r--r--   0        0        0      287 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/env.txt.j2
--rw-r--r--   0        0        0       22 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/stm32.cfg.j2
--rw-r--r--   0        0        0      294 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/esp32.cmake.j2
--rw-r--r--   0        0        0       39 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/mock/.clang-format
--rw-r--r--   0        0        0      475 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/mock/CMakeLists.txt
--rw-r--r--   0        0        0      594 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/mock/class_interface.h.j2
--rw-r--r--   0        0        0      835 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/mock/class_mock.cpp.j2
--rw-r--r--   0        0        0      697 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/mock/class_mock.h.j2
--rw-r--r--   0        0        0      510 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/project.cmake.j2
--rw-r--r--   0        0        0     2228 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/scargo.toml.j2
--rw-r--r--   0        0        0      802 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/stm32.cmake.j2
--rw-r--r--   0        0        0       91 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
--rw-r--r--   0        0        0      100 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
--rw-r--r--   0        0        0     1079 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
--rw-r--r--   0        0        0       84 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
--rw-r--r--   0        0        0      326 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
--rw-r--r--   0        0        0     1046 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/static_mock/static_mock.h
--rw-r--r--   0        0        0       39 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/ut/.clang-format
--rw-r--r--   0        0        0      575 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2
--rw-r--r--   0        0        0      716 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/ut/ut.cpp.j2
--rw-r--r--   0        0        0      213 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/x86.cmake.j2
--rw-r--r--   0        0        0     1597 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/tests_gen.py
--rw-r--r--   0        0        0      550 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/toml_gen.py
--rw-r--r--   0        0        0     5357 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/ut_gen.py
--rw-r--r--   0        0        0      629 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/global_values.py
--rw-r--r--   0        0        0     2044 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/logger.py
--rw-r--r--   0        0        0     1137 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/path_utils.py
--rw-r--r--   0        0        0     2953 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/templates/.clang-format
--rw-r--r--   0        0        0     8780 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/templates/.clang-tidy
--rw-r--r--   0        0        0     2361 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/templates/.gitignore
--rw-r--r--   0        0        0     1066 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/templates/LICENSE
--rw-r--r--   0        0        0      519 2023-05-31 13:51:14.593332 scargo-1.6.0/setup.cfg
--rw-r--r--   0        0        0     5235 1970-01-01 00:00:00.000000 scargo-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     4508 2023-07-19 10:03:29.503412 scargo-1.6.1/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     1066 2023-07-19 10:03:29.503412 scargo-1.6.1/LICENSE
+-rw-r--r--   0        0        0     2494 2023-07-19 10:03:29.503412 scargo-1.6.1/README.md
+-rw-r--r--   0        0        0     2748 2023-07-19 10:03:29.515412 scargo-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/__init__.py
+-rwxr-xr-x   0        0        0    19734 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/certs/certGen.sh
+-rwxr-xr-x   0        0        0     5226 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/certs/generateAllCertificates.sh
+-rw-r--r--   0        0        0     3967 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/certs/openssl_device_intermediate_ca.cnf
+-rw-r--r--   0        0        0     3957 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/certs/openssl_root_ca.cnf
+-rw-r--r--   0        0        0      698 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/clang_utils.py
+-rw-r--r--   0        0        0    12830 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/cli.py
+-rw-r--r--   0        0        0       86 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/commands/__init__.py
+-rw-r--r--   0        0        0     1767 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/commands/build.py
+-rw-r--r--   0        0        0    12319 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/commands/check.py
+-rw-r--r--   0        0        0     1142 2023-07-19 10:03:29.515412 scargo-1.6.1/scargo/commands/clean.py
+-rw-r--r--   0        0        0     4168 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/debug.py
+-rw-r--r--   0        0        0     3402 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/doc.py
+-rw-r--r--   0        0        0     3918 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/docker.py
+-rw-r--r--   0        0        0     1124 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/fix.py
+-rw-r--r--   0        0        0     3835 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/flash.py
+-rw-r--r--   0        0        0     6677 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/gen.py
+-rw-r--r--   0        0        0     2857 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/new.py
+-rw-r--r--   0        0        0     3405 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/publish.py
+-rw-r--r--   0        0        0     1688 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/run.py
+-rw-r--r--   0        0        0     3651 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/test.py
+-rw-r--r--   0        0        0     4553 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/update.py
+-rw-r--r--   0        0        0      228 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/commands/version.py
+-rw-r--r--   0        0        0     6707 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/config.py
+-rw-r--r--   0        0        0     2255 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/config_utils.py
+-rw-r--r--   0        0        0     2290 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/docker_utils.py
+-rw-r--r--   0        0        0       86 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/__init__.py
+-rw-r--r--   0        0        0     1658 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/base_gen.py
+-rw-r--r--   0        0        0      441 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/cicd_gen.py
+-rw-r--r--   0        0        0       86 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/clang_parser/__init__.py
+-rw-r--r--   0        0        0     2251 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/clang_parser/data_classes.py
+-rw-r--r--   0        0        0     1197 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/clang_parser/header_parser.py
+-rw-r--r--   0        0        0     2385 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/clang_parser/params_extractor.py
+-rw-r--r--   0        0        0      395 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/cmake_gen.py
+-rw-r--r--   0        0        0      940 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/conan_gen.py
+-rw-r--r--   0        0        0     2468 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/cpp_gen.py
+-rw-r--r--   0        0        0     3186 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/docker_gen.py
+-rw-r--r--   0        0        0     1115 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/env_gen.py
+-rwxr-xr-x   0        0        0     1607 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/mock_gen.py
+-rw-r--r--   0        0        0      454 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/readme_gen.py
+-rw-r--r--   0        0        0     4834 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/.gitlab-ci.yml.j2
+-rw-r--r--   0        0        0     1067 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/CMakeLists.txt.j2
+-rw-r--r--   0        0        0     4275 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/README.md.j2
+-rw-r--r--   0        0        0     1865 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/conan/conanfile.py.j2
+-rw-r--r--   0        0        0     1464 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/conan/conanfiletest.j2
+-rw-r--r--   0        0        0     2192 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/conan/profile.j2
+-rw-r--r--   0        0        0      150 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
+-rw-r--r--   0        0        0     2423 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
+-rw-r--r--   0        0        0      886 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/cmake-src-x86.j2
+-rw-r--r--   0        0        0      181 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/lib.cpp.j2
+-rw-r--r--   0        0        0      213 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/lib.h.j2
+-rw-r--r--   0        0        0      715 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/cpp/main.cpp.j2
+-rw-r--r--   0        0        0      159 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-custom.j2
+-rw-r--r--   0        0        0     2128 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
+-rw-r--r--   0        0        0      754 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
+-rw-r--r--   0        0        0       49 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-x86.j2
+-rw-r--r--   0        0        0     2363 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile.j2
+-rw-r--r--   0        0        0      158 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/devcontainer.json.j2
+-rw-r--r--   0        0        0     1000 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/docker-compose.yaml.j2
+-rw-r--r--   0        0        0      287 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/env.txt.j2
+-rw-r--r--   0        0        0       22 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/docker/stm32.cfg.j2
+-rw-r--r--   0        0        0      294 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/esp32.cmake.j2
+-rw-r--r--   0        0        0       39 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/mock/.clang-format
+-rw-r--r--   0        0        0      475 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/mock/CMakeLists.txt
+-rw-r--r--   0        0        0      594 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/mock/class_interface.h.j2
+-rw-r--r--   0        0        0      835 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/mock/class_mock.cpp.j2
+-rw-r--r--   0        0        0      697 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/mock/class_mock.h.j2
+-rw-r--r--   0        0        0      470 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/project.cmake.j2
+-rw-r--r--   0        0        0     2228 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/scargo.toml.j2
+-rw-r--r--   0        0        0      227 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/stm32.cmake.j2
+-rw-r--r--   0        0        0       91 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
+-rw-r--r--   0        0        0      100 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
+-rw-r--r--   0        0        0     1079 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
+-rw-r--r--   0        0        0       84 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
+-rw-r--r--   0        0        0      326 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
+-rw-r--r--   0        0        0     1046 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/tests/static_mock/static_mock.h
+-rw-r--r--   0        0        0       39 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/ut/.clang-format
+-rw-r--r--   0        0        0      575 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/ut/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      716 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/ut/ut.cpp.j2
+-rw-r--r--   0        0        0      213 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/templates/x86.cmake.j2
+-rw-r--r--   0        0        0     1597 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/tests_gen.py
+-rw-r--r--   0        0        0      550 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/toml_gen.py
+-rw-r--r--   0        0        0     5357 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/file_generators/ut_gen.py
+-rw-r--r--   0        0        0      629 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/global_values.py
+-rw-r--r--   0        0        0     2044 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/logger.py
+-rw-r--r--   0        0        0     1137 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/path_utils.py
+-rw-r--r--   0        0        0     2953 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/templates/.clang-format
+-rw-r--r--   0        0        0     8780 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/templates/.clang-tidy
+-rw-r--r--   0        0        0     2361 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/templates/.gitignore
+-rw-r--r--   0        0        0     1066 2023-07-19 10:03:29.519412 scargo-1.6.1/scargo/templates/LICENSE
+-rw-r--r--   0        0        0      519 2023-07-19 10:03:29.519412 scargo-1.6.1/setup.cfg
+-rw-r--r--   0        0        0     5235 1970-01-01 00:00:00.000000 scargo-1.6.1/PKG-INFO
```

### Comparing `scargo-1.6.0/CODE-OF-CONDUCT.md` & `scargo-1.6.1/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/LICENSE` & `scargo-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/README.md` & `scargo-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/pyproject.toml` & `scargo-1.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/certs/certGen.sh` & `scargo-1.6.1/scargo/certs/certGen.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/certs/generateAllCertificates.sh` & `scargo-1.6.1/scargo/certs/generateAllCertificates.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/certs/openssl_device_intermediate_ca.cnf` & `scargo-1.6.1/scargo/certs/openssl_device_intermediate_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/certs/openssl_root_ca.cnf` & `scargo-1.6.1/scargo/certs/openssl_root_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/clang_utils.py` & `scargo-1.6.1/scargo/clang_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/cli.py` & `scargo-1.6.1/scargo/cli.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/build.py` & `scargo-1.6.1/scargo/commands/build.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,21 +43,28 @@
     conan_clean_remote()
 
     conan_add_remote(project_dir, config)
     conan_add_conancenter()
 
     try:
         subprocess.check_call(
-            ["conan", "install", ".", "-if", build_dir],
+            [
+                "conan",
+                "install",
+                ".",
+                "-if",
+                build_dir,
+                "-pr:b",
+                "default",
+                "-pr:h",
+                f"./.conan/profiles/{config.project.target.family}_{profile}",
+            ],
             cwd=project_dir,
         )
         subprocess.check_call(
-            ["cmake", f"-DCMAKE_BUILD_TYPE={profile}", project_dir],
-            cwd=build_dir,
+            ["conan", "build", ".", "-if", build_dir, "-bf", build_dir],
+            cwd=project_dir,
         )
-        command = ["cmake", "--build", ".", "--parallel"]
-        if config.project.max_build_jobs is not None:
-            command.append(str(config.project.max_build_jobs))
-        subprocess.check_call(command, cwd=build_dir)
+
     except subprocess.CalledProcessError:
         logger.error("Unable to build exec file")
         sys.exit(1)
```

### Comparing `scargo-1.6.0/scargo/commands/check.py` & `scargo-1.6.1/scargo/commands/check.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/clean.py` & `scargo-1.6.1/scargo/commands/clean.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/debug.py` & `scargo-1.6.1/scargo/commands/debug.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/doc.py` & `scargo-1.6.1/scargo/commands/doc.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/docker.py` & `scargo-1.6.1/scargo/commands/docker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # #
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
 
 """Handle docker for project"""
+import shutil
 import subprocess
 import sys
 from pathlib import Path
 from typing import List, Optional, Sequence
 
 import docker
 
@@ -23,23 +24,25 @@
     Build docker
 
     :param docker_opts: additional docker options
     :param project_root
     :raises CalledProcessError: if docker build fail
     """
     logger.debug("Build docker environment.")
-
+    print(docker_opts)
     if not project_root:
         project_root = get_scargo_config_or_exit().project_root
     docker_path = _get_docker_path(project_root)
+    print(docker_path)
+
+    cmd = get_docker_compose_command()
+    cmd.extend(["build", *docker_opts])
 
     try:
-        subprocess.run(
-            ["docker-compose", "build", *docker_opts], cwd=docker_path, check=True
-        )
+        subprocess.run(cmd, cwd=docker_path, check=True)
         logger.info("Initialize docker environment.")
     except subprocess.CalledProcessError:
         logger.error("Build docker fail.")
         sys.exit(1)
 
 
 def scargo_docker_run(
@@ -55,20 +58,22 @@
     """
     logger.debug("Run docker environment.")
 
     config = get_scargo_config_or_exit()
     docker_path = _get_docker_path(config.project_root)
     project_config_name = config.project.name
 
-    cmd = [
-        "docker-compose",
-        "run",
-        *docker_opts,
-        f"{project_config_name}_dev",
-    ]
+    cmd = get_docker_compose_command()
+    cmd.extend(
+        [
+            "run",
+            *docker_opts,
+            f"{project_config_name}_dev",
+        ]
+    )
     if command:
         cmd.extend(["bash", "-c", command])
 
     try:
         subprocess.run(cmd, cwd=docker_path, check=True)
         logger.info("Stop docker environment.")
     except subprocess.CalledProcessError:
@@ -111,7 +116,26 @@
 
 def _get_docker_path(project_path: Path) -> Path:
     # do not rebuild dockers in the docker
     if Path("/.dockerenv").exists():
         logger.error("Cannot used docker command inside the docker container.")
         sys.exit(1)
     return Path(project_path, ".devcontainer")
+
+
+def get_docker_compose_command() -> List[str]:
+    """Get docker command
+
+    Returns:
+        List[str]: _description_
+    """
+    command = ["docker-compose"]
+    # Check if docker-compose or docker compose is available
+    if shutil.which("docker-compose"):
+        command = ["docker-compose"]
+    elif shutil.which("docker"):
+        command = ["docker", "compose"]
+    else:
+        logger.error("Neither docker-compose nor docker compose are available.")
+        sys.exit(1)
+
+    return command
```

### Comparing `scargo-1.6.0/scargo/commands/fix.py` & `scargo-1.6.1/scargo/commands/fix.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/flash.py` & `scargo-1.6.1/scargo/commands/flash.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/gen.py` & `scargo-1.6.1/scargo/commands/gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/new.py` & `scargo-1.6.1/scargo/commands/new.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/publish.py` & `scargo-1.6.1/scargo/commands/publish.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/run.py` & `scargo-1.6.1/scargo/commands/run.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/test.py` & `scargo-1.6.1/scargo/commands/test.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/commands/update.py` & `scargo-1.6.1/scargo/commands/update.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 """Update project"""
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 
-from scargo.commands.docker import scargo_docker_build
+from scargo.commands.docker import get_docker_compose_command, scargo_docker_build
 from scargo.config_utils import add_version_to_scargo_lock, get_scargo_config_or_exit
 from scargo.file_generators.cicd_gen import generate_cicd
 from scargo.file_generators.cmake_gen import generate_cmake
-from scargo.file_generators.conan_gen import generate_conanfile
+from scargo.file_generators.conan_gen import generate_conanfile, generate_conanprofile
 from scargo.file_generators.docker_gen import generate_docker_compose
 from scargo.file_generators.env_gen import generate_env
 from scargo.file_generators.readme_gen import generate_readme
 from scargo.file_generators.tests_gen import generate_tests
 from scargo.global_values import SCARGO_DOCKER_ENV, SCARGO_LOCK_FILE, SCARGO_PKG_PATH
 from scargo.logger import get_logger
 
@@ -68,14 +68,15 @@
 
     # Copy docker env files to repo directory
     generate_docker_compose(docker_path, config)
     generate_env(docker_path, config)
 
     generate_cmake(config)
     generate_conanfile(config)
+    generate_conanprofile(config)
 
     if target.family == "esp32":
         Path(config.source_dir_path, "fs").mkdir(parents=True, exist_ok=True)
         with open(Path(project_path, "version.txt"), "w", encoding="utf-8") as out:
             out.write(project_config.version)
         with open(Path(project_path, "partitions.csv"), "w", encoding="utf-8") as out:
             out.write(
@@ -104,16 +105,18 @@
         else:
             logger.warning("Cannot run docker inside docker")
 
 
 def pull_docker_image(docker_path: Path) -> bool:
     logger.info("Pulling the image from docker registry...")
     try:
+        cmd = get_docker_compose_command()
+        cmd.extend(["pull"])
         result = subprocess.run(
-            ["docker-compose", "pull"],
+            cmd,
             cwd=docker_path,
             stderr=subprocess.PIPE,
             check=True,
         )
     except subprocess.CalledProcessError as e:
         logger.warning(e.stderr.decode())
     else:
```

### Comparing `scargo-1.6.0/scargo/config.py` & `scargo-1.6.1/scargo/config.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/config_utils.py` & `scargo-1.6.1/scargo/config_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/docker_utils.py` & `scargo-1.6.1/scargo/docker_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from pathlib import Path
+from pathlib import Path, PurePosixPath
 from typing import List
 
 import docker as dock
 from docker import DockerClient
 
 from scargo.config import ProjectConfig
 from scargo.global_values import SCARGO_DOCKER_ENV
@@ -21,35 +21,34 @@
     :param dict project_config: project configuration
     :param Path project_path: path to project root
     :return: None
     """
     build_env = project_config.build_env
     if build_env != SCARGO_DOCKER_ENV or Path("/.dockerenv").exists():
         return
+
     relative_path = Path.cwd().relative_to(project_path)
-    path_in_docker = Path("/workspace", relative_path)
+    path_in_docker = PurePosixPath("/workspace", relative_path)
 
     cmd_args = sys.argv[1:]
+    try:
+        # Correct base-dir arg for command in docker
+        for idx, val in enumerate(cmd_args):
+            if val == "-B" or val == "--base-dir":
+                cmd_args[idx + 1] = "."
+    except Exception as e:
+        logger.error(e)
 
     entrypoint = ""
     if project_config.target.family == "esp32":
         entrypoint = "/opt/esp/entrypoint.sh"
 
     docker_tag = project_config.docker_image_tag
     client = dock.from_env()
 
-    run_command_in_docker(
-        ["scargo", "version"],
-        client,
-        docker_tag,
-        entrypoint,
-        project_path,
-        path_in_docker,
-    )
-
     status_code = run_command_in_docker(
         ["scargo", *cmd_args],
         client,
         docker_tag,
         entrypoint,
         project_path,
         path_in_docker,
@@ -59,15 +58,15 @@
 
 def run_command_in_docker(  # type: ignore[no-any-unimported]
     command: List[str],
     client: DockerClient,
     docker_tag: str,
     entrypoint: str,
     project_path: Path,
-    path_in_docker: Path,
+    path_in_docker: PurePosixPath,
 ) -> int:
     logger.info(f"Running '{' '.join(command)}' command in docker.")
     container = client.containers.run(
         docker_tag,
         command,
         volumes=[f"{project_path}:/workspace/", "/dev/:/dev/"],
         entrypoint=entrypoint,
```

### Comparing `scargo-1.6.0/scargo/file_generators/base_gen.py` & `scargo-1.6.1/scargo/file_generators/base_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/clang_parser/data_classes.py` & `scargo-1.6.1/scargo/file_generators/clang_parser/data_classes.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/clang_parser/header_parser.py` & `scargo-1.6.1/scargo/file_generators/clang_parser/header_parser.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/clang_parser/params_extractor.py` & `scargo-1.6.1/scargo/file_generators/clang_parser/params_extractor.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/conan_gen.py` & `scargo-1.6.1/scargo/file_generators/conan_gen.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,7 +15,18 @@
     )
     create_file_from_template(
         "conan/conanfiletest.j2",
         "tests/conanfile.py",
         template_params={"config": config},
         config=config,
     )
+
+
+def generate_conanprofile(config: Config) -> None:
+    profiles = list(config.profiles.keys())
+    for profile in profiles:
+        create_file_from_template(
+            "conan/profile.j2",
+            f".conan/profiles/{config.project.target.family}_{profile}",
+            template_params={"config": config, "profile": profile},
+            config=config,
+        )
```

### Comparing `scargo-1.6.0/scargo/file_generators/cpp_gen.py` & `scargo-1.6.1/scargo/file_generators/cpp_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/docker_gen.py` & `scargo-1.6.1/scargo/file_generators/docker_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/env_gen.py` & `scargo-1.6.1/scargo/file_generators/env_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/mock_gen.py` & `scargo-1.6.1/scargo/file_generators/mock_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/.gitlab-ci.yml.j2` & `scargo-1.6.1/scargo/file_generators/templates/.gitlab-ci.yml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/CMakeLists.txt.j2` & `scargo-1.6.1/scargo/file_generators/templates/CMakeLists.txt.j2`

 * *Files 20% similar despite different names*

```diff
@@ -8,48 +8,33 @@
 #
 {% if config.project.target.family == "esp32" %}
 cmake_minimum_required(VERSION 3.14)
 {% else %}
 cmake_minimum_required(VERSION 3.16)
 {% endif %}
 
-{% if config.project.target.family != 'x86' %}
-set(CONAN_DISABLE_CHECK_COMPILER ON)
-{% endif %}
-
 {% if config.project.target.family == 'stm32' %}
 {% include 'stm32.cmake.j2' %}
 {% elif config.project.target.family == 'x86' %}
 {% include 'x86.cmake.j2' %}
 {% endif %}
 
 set(CMAKE_CXX_STANDARD {{ config.project.cxxstandard }})
 
-{% if config.project.cflags %}
-set(CMAKE_C_FLAGS   "{{ config.project.cflags }}")
-{% endif %}
-{% if config.project.cxxflags %}
-set(CMAKE_CXX_FLAGS "{{ config.project.cxxflags }}")
-{% endif %}
 {% for key, value in config.project.cmake_variables.items() %}
 set({{ key }} "{{ value }}")
 {% endfor %}
+
 {% for profile_name, profile in config.profiles.items() %}
-# {{ profile_name }}
-    {% if profile.cflags  %}
-set(CMAKE_C_FLAGS_{{ profile_name.upper() }}   "{{ profile.cflags }}")
-    {% endif %}
-    {% if profile.cxxflags  %}
-set(CMAKE_CXX_FLAGS_{{ profile_name.upper() }} "{{ profile.cxxflags }}")
-	{% endif %}
     {% if profile.extras %}
+# {{ profile_name }}
 IF("${CMAKE_BUILD_TYPE}" STREQUAL "{{ profile_name }}")
-    {% for key, value in profile.extras.items() %}
+        {% for key, value in profile.extras.items() %}
     SET({{ key }} {{ value }})
-    {% endfor %}
+        {% endfor %}
 ENDIF()
     {% endif %}
 
 {% endfor %}
 
 {% if config.project.target.family == "esp32" %}
 {% include 'esp32.cmake.j2' %}
```

### Comparing `scargo-1.6.0/scargo/file_generators/templates/README.md.j2` & `scargo-1.6.1/scargo/file_generators/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/conan/conanfile.py.j2` & `scargo-1.6.1/scargo/file_generators/templates/conan/conanfile.py.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-from conans import CMake, ConanFile, tools  # type: ignore[misc, no-any-unimported]
-
+from conan import ConanFile
+from conan.tools.cmake import CMakeToolchain, CMake
+from conans import tools  # type: ignore[misc, no-any-unimported]
 
 class {{ config.project.name|capitalize|replace("-", "") }}Conan(ConanFile):  # type: ignore[misc, no-any-unimported]
     name = "{{ config.project.name }}"
     version = "{{ config.project.version }}"
     settings = "os", "compiler", "build_type", "arch"
     description = "{{ config.project.description }}"
     url = "{{ config.project.homepage_url }}"
-    generators = "cmake_find_package", "cmake"
+    generators = "CMakeDeps"
+    exports_sources = "src/*", "CMakeLists.txt"
+
+    def generate(self):
+        tc = CMakeToolchain(self)
+        tc.generate()
 
     def package(self) -> None:
         self.copy("*", src='build/Debug/bin/', dst='bin', keep_path=False)
         self.copy("*", src='build/Debug/lib/', dst='lib', keep_path=False)
 
     def package_info(self) -> None:
         self.cpp_info.libs = tools.collect_libs(self)
```

### Comparing `scargo-1.6.0/scargo/file_generators/templates/conan/conanfiletest.j2` & `scargo-1.6.1/scargo/file_generators/templates/conan/conanfiletest.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2` & `scargo-1.6.1/scargo/file_generators/templates/cpp/cmake-src-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2` & `scargo-1.6.1/scargo/file_generators/templates/cpp/cmake-src-x86.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/cpp/main.cpp.j2` & `scargo-1.6.1/scargo/file_generators/templates/cpp/main.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2` & `scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-esp32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2` & `scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile.j2` & `scargo-1.6.1/scargo/file_generators/templates/docker/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2` & `scargo-1.6.1/scargo/file_generators/templates/docker/docker-compose.yaml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/mock/class_interface.h.j2` & `scargo-1.6.1/scargo/file_generators/templates/mock/class_interface.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/mock/class_mock.cpp.j2` & `scargo-1.6.1/scargo/file_generators/templates/mock/class_mock.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/mock/class_mock.h.j2` & `scargo-1.6.1/scargo/file_generators/templates/mock/class_mock.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/scargo.toml.j2` & `scargo-1.6.1/scargo/file_generators/templates/scargo.toml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2` & `scargo-1.6.1/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/tests/static_mock/static_mock.h` & `scargo-1.6.1/scargo/file_generators/templates/tests/static_mock/static_mock.h`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2` & `scargo-1.6.1/scargo/file_generators/templates/ut/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/templates/ut/ut.cpp.j2` & `scargo-1.6.1/scargo/file_generators/templates/ut/ut.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/tests_gen.py` & `scargo-1.6.1/scargo/file_generators/tests_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/toml_gen.py` & `scargo-1.6.1/scargo/file_generators/toml_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/file_generators/ut_gen.py` & `scargo-1.6.1/scargo/file_generators/ut_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/global_values.py` & `scargo-1.6.1/scargo/global_values.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/logger.py` & `scargo-1.6.1/scargo/logger.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/path_utils.py` & `scargo-1.6.1/scargo/path_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/templates/.clang-format` & `scargo-1.6.1/scargo/templates/.clang-format`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/templates/.clang-tidy` & `scargo-1.6.1/scargo/templates/.clang-tidy`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/templates/.gitignore` & `scargo-1.6.1/scargo/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/scargo/templates/LICENSE` & `scargo-1.6.1/scargo/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/setup.cfg` & `scargo-1.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `scargo-1.6.0/PKG-INFO` & `scargo-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scargo
-Version: 1.6.0
+Version: 1.6.1
 Summary: C/C++ package and software development life cycle manager inspired by RUST cargo idea.
 Keywords: scargo,Package manager,C++
 Author-email: "Spyrosoft Solutions S.A." <aak@spyro-soft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

