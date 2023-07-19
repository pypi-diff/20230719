# Comparing `tmp/alpaqa-1.0.0a6.tar.gz` & `tmp/alpaqa-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaqa-1.0.0a6.tar", last modified: Tue Nov 22 13:27:13 2022, max compression
+gzip compressed data, was "alpaqa-1.0.0a7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `alpaqa-1.0.0a6.tar` & `alpaqa-1.0.0a7.tar`

### file list

```diff
@@ -1,110 +1,272 @@
--rw-r--r--   0        0        0     2735 2022-11-22 13:26:33.382262 alpaqa-1.0.0a6/CMakeLists.txt
--rw-r--r--   0        0        0     7652 2022-11-22 13:26:33.382262 alpaqa-1.0.0a6/LICENSE
--rw-r--r--   0        0        0     2079 2022-11-22 13:26:33.382262 alpaqa-1.0.0a6/README.md
--rw-r--r--   0        0        0      821 2022-11-22 13:26:33.382262 alpaqa-1.0.0a6/cmake/Sanitizers.cmake
--rw-r--r--   0        0        0     2790 2022-11-22 13:26:33.382262 alpaqa-1.0.0a6/cmake/Warnings.cmake
--rw-r--r--   0        0        0       77 2022-11-22 13:26:33.434262 alpaqa-1.0.0a6/interfaces/CMakeLists.txt
--rw-r--r--   0        0        0     2984 2022-11-22 13:26:33.434262 alpaqa-1.0.0a6/interfaces/python/CMakeLists.txt
--rw-r--r--   0        0        0      788 2022-11-22 13:26:33.434262 alpaqa-1.0.0a6/interfaces/python/cmake/Pybind11Stubgen.cmake
--rw-r--r--   0        0        0     3547 2022-11-22 13:26:33.434262 alpaqa-1.0.0a6/interfaces/python/cmake/QueryPythonForPybind11.cmake
--rw-r--r--   0        0        0       58 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/.clang-format
--rw-r--r--   0        0        0    10805 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/alm.py.cpp
--rw-r--r--   0        0        0     1914 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/alpaqa.py.cpp
--rw-r--r--   0        0        0     7629 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/counters.py.cpp
--rw-r--r--   0        0        0     2746 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/enums.py.cpp
--rw-r--r--   0        0        0     7538 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/kwargs-to-struct.hpp
--rw-r--r--   0        0        0      634 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/lbfgs-params.hpp
--rw-r--r--   0        0        0    31122 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/panoc.py.cpp
--rw-r--r--   0        0        0    32813 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/problems.py.cpp
--rw-r--r--   0        0        0     5107 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/stats-to-dict.hpp
--rw-r--r--   0        0        0     9788 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/structured-panoc.py.cpp
--rw-r--r--   0        0        0     2287 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/type-erased-inner-solver.hpp
--rw-r--r--   0        0        0     4179 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/type-erased-panoc-direction.hpp
--rw-r--r--   0        0        0     2689 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/interfaces/python/src/type-erased-solver-stats.hpp
--rw-r--r--   0        0        0     2854 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     2027 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/python/README.rst
--rw-r--r--   0        0        0      689 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/python/alpaqa/__init__.py
--rw-r--r--   0        0        0     1551 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/python/alpaqa/__main__.py
--rw-r--r--   0        0        0     1449 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/python/alpaqa/cache.py
--rw-r--r--   0        0        0     9218 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/python/alpaqa/casadi_generator/__init__.py
--rw-r--r--   0        0        0    10660 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/python/alpaqa/casadi_loader/__init__.py
--rw-r--r--   0        0        0     3216 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/CMakeLists.txt
--rw-r--r--   0        0        0      642 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/alpaqa.dox
--rw-r--r--   0        0        0      149 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/cmake/Config.cmake.in
--rw-r--r--   0        0        0     2412 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/cmake/Install.cmake
--rw-r--r--   0        0        0     9484 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/accelerators/lbfgs.hpp
--rw-r--r--   0        0        0     7137 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/accelerators/src/lbfgs.tpp
--rw-r--r--   0        0        0       46 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/alpaqa.hpp
--rw-r--r--   0        0        0      614 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/casadi-loader-export.hpp
--rw-r--r--   0        0        0     5821 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/config/config.hpp
--rw-r--r--   0        0        0      720 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/export.hpp
--rw-r--r--   0        0        0     3352 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/directions/panoc-direction-update.hpp
--rw-r--r--   0        0        0     9817 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/directions/panoc-ocp/dynamics-eval.hpp
--rw-r--r--   0        0        0    11898 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/directions/panoc-ocp/lqr.hpp
--rw-r--r--   0        0        0     2207 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/directions/panoc-ocp/src/lqr.tpp
--rw-r--r--   0        0        0     2444 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/directions/panoc/lbfgs.hpp
--rw-r--r--   0        0        0     4708 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/directions/panoc/src/structured-lbfgs.tpp
--rw-r--r--   0        0        0     3094 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/directions/panoc/structured-lbfgs.hpp
--rw-r--r--   0        0        0      726 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/internal/lipschitz.hpp
--rw-r--r--   0        0        0      153 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/internal/panoc-helpers.hpp
--rw-r--r--   0        0        0     4569 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/internal/panoc-stop-crit.hpp
--rw-r--r--   0        0        0     1317 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/internal/solverstatus.hpp
--rw-r--r--   0        0        0     5847 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/panoc-ocp.hpp
--rw-r--r--   0        0        0     7728 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/panoc.hpp
--rw-r--r--   0        0        0    17658 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/src/panoc-helpers.tpp
--rw-r--r--   0        0        0    28056 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/src/panoc-ocp.tpp
--rw-r--r--   0        0        0    15565 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/src/panoc.tpp
--rw-r--r--   0        0        0    24170 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/src/structured-panoc.tpp
--rw-r--r--   0        0        0     9542 2022-11-22 13:26:33.438262 alpaqa-1.0.0a6/src/include/alpaqa/inner/structured-panoc.hpp
--rw-r--r--   0        0        0     2493 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/CasADiControlProblem.hpp
--rw-r--r--   0        0        0     3671 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/CasADiFunctionWrapper.hpp
--rw-r--r--   0        0        0     3734 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/CasADiProblem.hpp
--rw-r--r--   0        0        0     3016 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/CasADiQuadraticControlProblem.hpp
--rw-r--r--   0        0        0     7782 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/src/CasADiControlProblem.tpp
--rw-r--r--   0        0        0     1045 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/src/CasADiLoader-util.hpp
--rw-r--r--   0        0        0    10533 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/src/CasADiProblem.tpp
--rw-r--r--   0        0        0     9081 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/src/CasADiQuadraticControlProblem.tpp
--rw-r--r--   0        0        0     7708 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/outer/alm.hpp
--rw-r--r--   0        0        0      114 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/outer/internal/alm-helpers.hpp
--rw-r--r--   0        0        0     9557 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/outer/src/alm.tpp
--rw-r--r--   0        0        0     3023 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/outer/src/internal/alm-helpers.tpp
--rw-r--r--   0        0        0     1055 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/panoc-alm.hpp
--rw-r--r--   0        0        0     2185 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/problem/box.hpp
--rw-r--r--   0        0        0     8482 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/problem/dynamics.hpp
--rw-r--r--   0        0        0     3706 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/problem/problem-counters.hpp
--rw-r--r--   0        0        0      162 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/problem/structure.hpp
--rw-r--r--   0        0        0    48598 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/problem/type-erased-problem.hpp
--rw-r--r--   0        0        0      732 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/structured-panoc-alm.hpp
--rw-r--r--   0        0        0      620 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/alloc-check.hpp
--rw-r--r--   0        0        0      644 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/atomic-stop-signal.hpp
--rw-r--r--   0        0        0     1269 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/check-dim.hpp
--rw-r--r--   0        0        0     1022 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/copyable_unique_ptr.hpp
--rw-r--r--   0        0        0      165 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/demangled-typename.hpp
--rw-r--r--   0        0        0      546 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/float.hpp
--rw-r--r--   0        0        0     2920 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/index-set.hpp
--rw-r--r--   0        0        0     1149 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/max-history.hpp
--rw-r--r--   0        0        0      173 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/not-implemented.hpp
--rw-r--r--   0        0        0      429 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/print.hpp
--rw-r--r--   0        0        0       58 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/quadmath/.clang-format
--rw-r--r--   0        0        0      464 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/quadmath/quadmath-print.hpp
--rw-r--r--   0        0        0     6989 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/quadmath/quadmath.hpp
--rw-r--r--   0        0        0     3515 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/src/print.tpp
--rw-r--r--   0        0        0    13871 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/type-erasure.hpp
--rw-r--r--   0        0        0      892 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/include/alpaqa/util/type-traits.hpp
--rw-r--r--   0        0        0      288 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/interop/casadi/CasADiControlProblem.cpp
--rw-r--r--   0        0        0      267 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/interop/casadi/CasADiProblem.cpp
--rw-r--r--   0        0        0      375 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/interop/casadi/CasADiQuadraticControlProblem.cpp
--rw-r--r--   0        0        0     1103 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/accelerators/lbfgs.cpp
--rw-r--r--   0        0        0      211 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/inner/internal/panoc-stop-crit.cpp
--rw-r--r--   0        0        0      207 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/inner/internal/solverstatus.cpp
--rw-r--r--   0        0        0      815 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/inner/panoc-ocp.cpp
--rw-r--r--   0        0        0     1119 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/inner/panoc.cpp
--rw-r--r--   0        0        0     1802 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/inner/structured-panoc.cpp
--rw-r--r--   0        0        0      402 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/outer/alm.cpp
--rw-r--r--   0        0        0      939 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/panoc-alm.cpp
--rw-r--r--   0        0        0     2340 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/problem/problem-counters.cpp
--rw-r--r--   0        0        0      737 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/structured-panoc-alm.cpp
--rw-r--r--   0        0        0      367 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/util/demangled-typename.cpp
--rw-r--r--   0        0        0     2019 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/util/print.cpp
--rw-r--r--   0        0        0       39 2022-11-22 13:26:33.442263 alpaqa-1.0.0a6/src/src/util/type-erasure.cpp
--rw-r--r--   0        0        0     3351 1970-01-01 00:00:00.000000 alpaqa-1.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0     4668 2023-07-19 07:49:31.276489 alpaqa-1.0.0a7/CMakeLists.txt
+-rw-r--r--   0        0        0     7652 2023-07-19 07:49:31.276489 alpaqa-1.0.0a7/LICENSE
+-rw-r--r--   0        0        0     1763 2023-07-19 07:49:31.276489 alpaqa-1.0.0a7/README.md
+-rw-r--r--   0        0        0     1165 2023-07-19 07:49:31.276489 alpaqa-1.0.0a7/cmake/Debug.cmake
+-rw-r--r--   0        0        0      821 2023-07-19 07:49:31.280489 alpaqa-1.0.0a7/cmake/Sanitizers.cmake
+-rw-r--r--   0        0        0     4052 2023-07-19 07:49:31.280489 alpaqa-1.0.0a7/cmake/Warnings.cmake
+-rw-r--r--   0        0        0      335 2023-07-19 07:49:31.280489 alpaqa-1.0.0a7/cmake/alpaqa-version.h.in
+-rw-r--r--   0        0        0     3275 2023-07-19 07:49:31.280489 alpaqa-1.0.0a7/cmake/find/FindCOINMUMPS.cmake
+-rw-r--r--   0        0        0     2909 2023-07-19 07:49:31.280489 alpaqa-1.0.0a7/cmake/find/FindIpopt.cmake
+-rw-r--r--   0        0        0       77 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/CMakeLists.txt
+-rw-r--r--   0        0        0     4565 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/CMakeLists.txt
+-rw-r--r--   0        0        0      788 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/cmake/Pybind11Stubgen.cmake
+-rw-r--r--   0        0        0     3547 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/cmake/QueryPythonForPybind11.cmake
+-rw-r--r--   0        0        0       58 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/.clang-format
+-rw-r--r--   0        0        0     1639 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/accel/anderson.py.cpp
+-rw-r--r--   0        0        0     4702 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/accel/lbfgs.py.cpp
+-rw-r--r--   0        0        0     3278 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/alpaqa.py.cpp
+-rw-r--r--   0        0        0    17776 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/counters.py.cpp
+-rw-r--r--   0        0        0      505 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/dict/dict-tup.hpp
+-rw-r--r--   0        0        0     8114 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/dict/kwargs-to-struct.hpp
+-rw-r--r--   0        0        0    10161 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/dict/stats-to-dict.hpp
+-rw-r--r--   0        0        0     2262 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/enums.py.cpp
+-rw-r--r--   0        0        0     3585 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/inner/inner-solve.hpp
+-rw-r--r--   0        0        0     1911 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/inner/inner-solver.py.cpp
+-rw-r--r--   0        0        0    11255 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/inner/ocp.py.cpp
+-rw-r--r--   0        0        0     9902 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/inner/panoc-directions.py.cpp
+-rw-r--r--   0        0        0     5102 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/inner/panoc-ocp.py.cpp
+-rw-r--r--   0        0        0     7226 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/inner/panoc.py.cpp
+-rw-r--r--   0        0        0     5586 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/inner/pantr-directions.py.cpp
+-rw-r--r--   0        0        0     6743 2023-07-19 07:49:31.368496 alpaqa-1.0.0a7/interfaces/python/src/inner/pantr.py.cpp
+-rw-r--r--   0        0        0     3225 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/inner/type-erased-inner-solver.hpp
+-rw-r--r--   0        0        0     4957 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/inner/type-erased-panoc-direction.hpp
+-rw-r--r--   0        0        0     3086 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/inner/type-erased-solver-stats.hpp
+-rw-r--r--   0        0        0     4945 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/inner/type-erased-tr-direction.hpp
+-rw-r--r--   0        0        0     6753 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/inner/zerofpr.py.cpp
+-rw-r--r--   0        0        0     5281 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/outer/alm.py.cpp
+-rw-r--r--   0        0        0     5452 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/outer/type-erased-alm-solver.hpp
+-rw-r--r--   0        0        0     1985 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/alm-params.cpp
+-rw-r--r--   0        0        0      439 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/alm-params.hpp
+-rw-r--r--   0        0        0      488 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/anderson-direction-params.cpp
+-rw-r--r--   0        0        0      530 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/anderson-direction-params.hpp
+-rw-r--r--   0        0        0      529 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/anderson-params.cpp
+-rw-r--r--   0        0        0      500 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/anderson-params.hpp
+-rw-r--r--   0        0        0      573 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/inner-solve-options.cpp
+-rw-r--r--   0        0        0      494 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/inner-solve-options.hpp
+-rw-r--r--   0        0        0      475 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/lbfgs-direction-params.cpp
+-rw-r--r--   0        0        0      512 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/lbfgs-direction-params.hpp
+-rw-r--r--   0        0        0     1108 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/lbfgs-params.cpp
+-rw-r--r--   0        0        0      821 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/lbfgs-params.hpp
+-rw-r--r--   0        0        0      709 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/newton-tr-direction-params.cpp
+-rw-r--r--   0        0        0      523 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/newton-tr-direction-params.hpp
+-rw-r--r--   0        0        0     1893 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/panoc-ocp-params.cpp
+-rw-r--r--   0        0        0      469 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/panoc-ocp-params.hpp
+-rw-r--r--   0        0        0     2305 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/panoc-params.cpp
+-rw-r--r--   0        0        0      874 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/panoc-params.hpp
+-rw-r--r--   0        0        0     2314 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/pantr-params.cpp
+-rw-r--r--   0        0        0      442 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/pantr-params.hpp
+-rw-r--r--   0        0        0      530 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/params.hpp
+-rw-r--r--   0        0        0      605 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/steihaug-params.cpp
+-rw-r--r--   0        0        0      479 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/steihaug-params.hpp
+-rw-r--r--   0        0        0      687 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/structured-lbfgs-direction-params.cpp
+-rw-r--r--   0        0        0      573 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/structured-lbfgs-direction-params.hpp
+-rw-r--r--   0        0        0     1167 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/structured-newton-direction-params.cpp
+-rw-r--r--   0        0        0     1068 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/structured-newton-direction-params.hpp
+-rw-r--r--   0        0        0     1754 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/zerofpr-params.cpp
+-rw-r--r--   0        0        0      454 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/params/zerofpr-params.hpp
+-rw-r--r--   0        0        0     5647 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/problem/control-problems.py.cpp
+-rw-r--r--   0        0        0    22524 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/problem/problems.py.cpp
+-rw-r--r--   0        0        0     2131 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/util/async.hpp
+-rw-r--r--   0        0        0      835 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/util/copy.hpp
+-rw-r--r--   0        0        0     1989 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/util/member.hpp
+-rw-r--r--   0        0        0      712 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/util/stream-replacer.hpp
+-rw-r--r--   0        0        0     1370 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/interfaces/python/src/util/thread-checker.hpp
+-rw-r--r--   0        0        0     2868 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0     2011 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/python/README.rst
+-rw-r--r--   0        0        0      225 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/python/alpaqa/__init__.py
+-rw-r--r--   0        0        0     1551 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/python/alpaqa/__main__.py
+-rw-r--r--   0        0        0      572 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/python/alpaqa/alpaqa.py
+-rw-r--r--   0        0        0     2068 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/python/alpaqa/cache.py
+-rw-r--r--   0        0        0    17347 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/python/alpaqa/casadi_generator/__init__.py
+-rw-r--r--   0        0        0     4718 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/python/alpaqa/casadi_loader/__init__.py
+-rw-r--r--   0        0        0     4399 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/python/alpaqa/casadi_loader/ocp.py
+-rw-r--r--   0        0        0       79 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/python/alpaqa/pyapi/__init__.py
+-rw-r--r--   0        0        0     7241 2023-07-19 07:49:31.372497 alpaqa-1.0.0a7/python/alpaqa/pyapi/minimize.py
+-rw-r--r--   0        0        0    12246 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/CMakeLists.txt
+-rw-r--r--   0        0        0      635 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa.dox
+-rw-r--r--   0        0        0     4692 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/accelerators/anderson.hpp
+-rw-r--r--   0        0        0     3617 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/accelerators/internal/anderson-helpers.hpp
+-rw-r--r--   0        0        0    11686 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/accelerators/internal/limited-memory-qr.hpp
+-rw-r--r--   0        0        0     9544 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/accelerators/lbfgs.hpp
+-rw-r--r--   0        0        0     5152 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/accelerators/steihaugcg.hpp
+-rw-r--r--   0        0        0       46 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/alpaqa.hpp
+-rw-r--r--   0        0        0      614 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/casadi-loader-export.hpp
+-rw-r--r--   0        0        0      627 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/casadi-ocp-loader-export.hpp
+-rw-r--r--   0        0        0     6707 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/config/config.hpp
+-rw-r--r--   0        0        0      720 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/export.hpp
+-rw-r--r--   0        0        0     7178 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/accelerators/lbfgs.tpp
+-rw-r--r--   0        0        0     7143 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/inner/directions/panoc/structured-lbfgs.tpp
+-rw-r--r--   0        0        0    16685 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/inner/panoc-helpers.tpp
+-rw-r--r--   0        0        0    32283 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/inner/panoc-ocp.tpp
+-rw-r--r--   0        0        0    17888 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/inner/panoc.tpp
+-rw-r--r--   0        0        0    18779 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/inner/pantr.tpp
+-rw-r--r--   0        0        0    19497 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/inner/zerofpr.tpp
+-rw-r--r--   0        0        0    10219 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/outer/alm.tpp
+-rw-r--r--   0        0        0     2922 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/outer/internal/alm-helpers.tpp
+-rw-r--r--   0        0        0     4800 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/params/params.tpp
+-rw-r--r--   0        0        0       58 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/problem/.clang-format
+-rw-r--r--   0        0        0     2516 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/problem/ocproblem.tpp
+-rw-r--r--   0        0        0     8592 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/problem/type-erased-problem.tpp
+-rw-r--r--   0        0        0     3966 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/util/io/csv.tpp
+-rw-r--r--   0        0        0     4899 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/util/print.tpp
+-rw-r--r--   0        0        0     3580 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/directions/panoc-direction-update.hpp
+-rw-r--r--   0        0        0     6469 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/directions/panoc-ocp/lqr.hpp
+-rw-r--r--   0        0        0    18192 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/directions/panoc-ocp/ocp-vars.hpp
+-rw-r--r--   0        0        0     3631 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/directions/panoc/anderson.hpp
+-rw-r--r--   0        0        0     3393 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/directions/panoc/lbfgs.hpp
+-rw-r--r--   0        0        0     5923 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/directions/panoc/structured-lbfgs.hpp
+-rw-r--r--   0        0        0    10416 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/directions/panoc/structured-newton.hpp
+-rw-r--r--   0        0        0     7301 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/directions/pantr/newton-tr.hpp
+-rw-r--r--   0        0        0     3690 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/directions/pantr/pantr-direction.hpp
+-rw-r--r--   0        0        0      923 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/inner-solve-options.hpp
+-rw-r--r--   0        0        0      750 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/internal/lipschitz.hpp
+-rw-r--r--   0        0        0      153 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/internal/panoc-helpers.hpp
+-rw-r--r--   0        0        0     4569 2023-07-19 07:49:31.376497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/internal/panoc-stop-crit.hpp
+-rw-r--r--   0        0        0     1427 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/internal/solverstatus.hpp
+-rw-r--r--   0        0        0    11518 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/panoc-ocp.hpp
+-rw-r--r--   0        0        0    10113 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/panoc.hpp
+-rw-r--r--   0        0        0    10701 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/pantr.hpp
+-rw-r--r--   0        0        0    10231 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/zerofpr.hpp
+-rw-r--r--   0        0        0     1198 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/newton-tr-pantr-alm.hpp
+-rw-r--r--   0        0        0     8121 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/outer/alm.hpp
+-rw-r--r--   0        0        0      151 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/outer/internal/alm-helpers.hpp
+-rw-r--r--   0        0        0     1164 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/panoc-alm.hpp
+-rw-r--r--   0        0        0     1197 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/panoc-anderson-alm.hpp
+-rw-r--r--   0        0        0     2259 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/params/params.hpp
+-rw-r--r--   0        0        0       58 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/.clang-format
+-rw-r--r--   0        0        0     9125 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/box-constr-problem.hpp
+-rw-r--r--   0        0        0     2861 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/box.hpp
+-rw-r--r--   0        0        0     3634 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/functional-problem.hpp
+-rw-r--r--   0        0        0     1621 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/kkt-error.hpp
+-rw-r--r--   0        0        0     3542 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/ocproblem-counters.hpp
+-rw-r--r--   0        0        0    50542 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/ocproblem.hpp
+-rw-r--r--   0        0        0     3491 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/problem-counters.hpp
+-rw-r--r--   0        0        0    14899 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/problem-with-counters.hpp
+-rw-r--r--   0        0        0    41346 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/type-erased-problem.hpp
+-rw-r--r--   0        0        0     1146 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/unconstr-problem.hpp
+-rw-r--r--   0        0        0     1275 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/structured-panoc-alm.hpp
+-rw-r--r--   0        0        0     1297 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/structured-zerofpr-alm.hpp
+-rw-r--r--   0        0        0      620 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/alloc-check.hpp
+-rw-r--r--   0        0        0      644 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/atomic-stop-signal.hpp
+-rw-r--r--   0        0        0     1692 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/check-dim.hpp
+-rw-r--r--   0        0        0     1106 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/copyable_unique_ptr.hpp
+-rw-r--r--   0        0        0      209 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/demangled-typename.hpp
+-rw-r--r--   0        0        0     1998 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/enumerate.hpp
+-rw-r--r--   0        0        0      546 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/float.hpp
+-rw-r--r--   0        0        0     3676 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/index-set.hpp
+-rw-r--r--   0        0        0     1512 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/io/csv.hpp
+-rw-r--r--   0        0        0     2285 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/iter-adapter.hpp
+-rw-r--r--   0        0        0     1149 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/max-history.hpp
+-rw-r--r--   0        0        0      400 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/noop-delete.hpp
+-rw-r--r--   0        0        0      214 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/not-implemented.hpp
+-rw-r--r--   0        0        0     3698 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/print.hpp
+-rw-r--r--   0        0        0       58 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/quadmath/.clang-format
+-rw-r--r--   0        0        0      464 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/quadmath/quadmath-print.hpp
+-rw-r--r--   0        0        0     6989 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/quadmath/quadmath.hpp
+-rw-r--r--   0        0        0     1906 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/required-method.hpp
+-rw-r--r--   0        0        0     6770 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/ringbuffer.hpp
+-rw-r--r--   0        0        0     4779 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/set-intersection.hpp
+-rw-r--r--   0        0        0     5504 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/sparse-ops.hpp
+-rw-r--r--   0        0        0      572 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/timed.hpp
+-rw-r--r--   0        0        0    21921 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/type-erasure.hpp
+-rw-r--r--   0        0        0     1422 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/type-traits.hpp
+-rw-r--r--   0        0        0     1186 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/zerofpr-alm.hpp
+-rw-r--r--   0        0        0     1219 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/zerofpr-anderson-alm.hpp
+-rw-r--r--   0        0        0     1114 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/accelerators/lbfgs.cpp
+-rw-r--r--   0        0        0     4900 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/alm-driver.hpp
+-rw-r--r--   0        0        0    10515 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/alpaqa-driver.cpp
+-rw-r--r--   0        0        0     1801 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/cancel.hpp
+-rw-r--r--   0        0        0        0 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/experiment.hpp
+-rw-r--r--   0        0        0     5278 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/ipopt-driver.cpp
+-rw-r--r--   0        0        0      226 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/ipopt-driver.hpp
+-rw-r--r--   0        0        0     1522 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/lbfgsb-driver.cpp
+-rw-r--r--   0        0        0      227 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/lbfgsb-driver.hpp
+-rw-r--r--   0        0        0      867 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/options.hpp
+-rw-r--r--   0        0        0     2565 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/panoc-driver.cpp
+-rw-r--r--   0        0        0      304 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/panoc-driver.hpp
+-rw-r--r--   0        0        0     2082 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/pantr-driver.cpp
+-rw-r--r--   0        0        0      226 2023-07-19 07:49:31.380497 alpaqa-1.0.0a7/src/alpaqa/src/driver/pantr-driver.hpp
+-rw-r--r--   0        0        0     4522 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/driver/problem.cpp
+-rw-r--r--   0        0        0      827 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/driver/problem.hpp
+-rw-r--r--   0        0        0     5986 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/driver/results.hpp
+-rw-r--r--   0        0        0      313 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/driver/solver-driver.hpp
+-rw-r--r--   0        0        0      604 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/driver/util.hpp
+-rw-r--r--   0        0        0      522 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/inner/directions/panoc/structured-lbfgs.cpp
+-rw-r--r--   0        0        0     1113 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/inner/directions/panoc/structured-newton.cpp
+-rw-r--r--   0        0        0      458 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/inner/internal/panoc-helpers.cpp
+-rw-r--r--   0        0        0      211 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/inner/internal/panoc-stop-crit.cpp
+-rw-r--r--   0        0        0      207 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/inner/internal/solverstatus.cpp
+-rw-r--r--   0        0        0      826 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/inner/panoc-ocp.cpp
+-rw-r--r--   0        0        0     1130 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/inner/panoc.cpp
+-rw-r--r--   0        0        0     1130 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/inner/pantr.cpp
+-rw-r--r--   0        0        0     1162 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/inner/zerofpr.cpp
+-rw-r--r--   0        0        0     1130 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/newton-tr-pantr-alm.cpp
+-rw-r--r--   0        0        0      402 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/outer/alm.cpp
+-rw-r--r--   0        0        0      447 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/outer/internal/alm-helpers.cpp
+-rw-r--r--   0        0        0     1090 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/panoc-alm.cpp
+-rw-r--r--   0        0        0     1129 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/panoc-anderson-alm.cpp
+-rw-r--r--   0        0        0     3800 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/params/from_chars-compat.ipp
+-rw-r--r--   0        0        0    21600 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/params/params.cpp
+-rw-r--r--   0        0        0     2832 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/problem/ocproblem-counters.cpp
+-rw-r--r--   0        0        0      480 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/problem/ocproblem.cpp
+-rw-r--r--   0        0        0     2692 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/problem/problem-counters.cpp
+-rw-r--r--   0        0        0      455 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/problem/type-erased-problem.cpp
+-rw-r--r--   0        0        0     1278 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/structured-panoc-alm.cpp
+-rw-r--r--   0        0        0     1302 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/structured-zerofpr-alm.cpp
+-rw-r--r--   0        0        0      367 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/util/demangled-typename.cpp
+-rw-r--r--   0        0        0     1024 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/util/io/csv.cpp
+-rw-r--r--   0        0        0     4066 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/util/print.cpp
+-rw-r--r--   0        0        0       39 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/util/type-erasure.cpp
+-rw-r--r--   0        0        0     1114 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/zerofpr-alm.cpp
+-rw-r--r--   0        0        0     1153 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/alpaqa/src/zerofpr-anderson-alm.cpp
+-rw-r--r--   0        0        0      571 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/cmake/Config.cmake.in
+-rw-r--r--   0        0        0     4365 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/cmake/Install.cmake
+-rw-r--r--   0        0        0     8762 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/casadi/include/alpaqa/casadi/CasADiControlProblem.hpp
+-rw-r--r--   0        0        0     3965 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/casadi/include/alpaqa/casadi/CasADiFunctionWrapper.hpp
+-rw-r--r--   0        0        0     4723 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/casadi/include/alpaqa/casadi/CasADiProblem.hpp
+-rw-r--r--   0        0        0    23587 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/casadi/include/alpaqa/implementation/casadi/CasADiControlProblem.tpp
+-rw-r--r--   0        0        0     1434 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/casadi/include/alpaqa/implementation/casadi/CasADiLoader-util.hpp
+-rw-r--r--   0        0        0    16416 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/casadi/include/alpaqa/implementation/casadi/CasADiProblem.tpp
+-rw-r--r--   0        0        0      299 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/casadi/src/CasADiControlProblem.cpp
+-rw-r--r--   0        0        0      270 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/casadi/src/CasADiProblem.cpp
+-rw-r--r--   0        0        0    15258 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/dl-api/include/alpaqa/dl/dl-problem.h
+-rw-r--r--   0        0        0    13376 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/dl/include/alpaqa/dl/dl-problem.hpp
+-rw-r--r--   0        0        0    17042 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/dl/src/dl-problem.cpp
+-rw-r--r--   0        0        0     2856 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/ipopt/include/alpaqa/ipopt/ipopt-adapter.hpp
+-rw-r--r--   0        0        0     1780 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/ipopt/include/alpaqa/ipopt/ipopt-enums.hpp
+-rw-r--r--   0        0        0     7242 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/ipopt/src/ipopt-adapter.cpp
+-rw-r--r--   0        0        0     2689 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/ipopt/src/ipopt-params.cpp
+-rw-r--r--   0        0        0     3456 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/lbfgsb/include/alpaqa/lbfgsb/lbfgsb-adapter.hpp
+-rw-r--r--   0        0        0     8235 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/lbfgsb/src/lbfgsb-adapter.cpp
+-rw-r--r--   0        0        0      680 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/lbfgsb/src/lbfgsb-params.cpp
+-rw-r--r--   0        0        0     2166 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/lbfgsb/src/lbfgsb_c.f90
+-rw-r--r--   0        0        0     3798 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/lbfgspp/include/alpaqa/implementation/lbfgsb-adapter.tpp
+-rw-r--r--   0        0        0     3553 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/lbfgspp/include/alpaqa/lbfgsb-adapter.hpp
+-rw-r--r--   0        0        0      770 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/lbfgspp/include/alpaqa/lbfgspp-adapter-export.hpp
+-rw-r--r--   0        0        0      868 2023-07-19 07:49:31.384498 alpaqa-1.0.0a7/src/interop/lbfgspp/src/lbfgsb-adapter.cpp
+-rw-r--r--   0        0        0       86 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/src/thirdparty/lbfgsb/Lbfgsb.3.0/.gitignore
+-rw-r--r--   0        0        0     4557 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/src/thirdparty/lbfgsb/Lbfgsb.3.0/License.txt
+-rw-r--r--   0        0        0    10166 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/src/thirdparty/lbfgsb/Lbfgsb.3.0/README
+-rw-r--r--   0        0        0     6312 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/src/thirdparty/lbfgsb/Lbfgsb.3.0/blas.f
+-rw-r--r--   0        0        0   130488 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/src/thirdparty/lbfgsb/Lbfgsb.3.0/lbfgsb.f
+-rw-r--r--   0        0        0     6383 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/src/thirdparty/lbfgsb/Lbfgsb.3.0/linpack.f
+-rw-r--r--   0        0        0     1157 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/src/thirdparty/lbfgsb/Lbfgsb.3.0/timer.f
+-rw-r--r--   0        0        0      196 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/src/thirdparty/lbfgsb/README.md
+-rw-r--r--   0        0        0     2344 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/CMakeLists.txt
+-rw-r--r--   0        0        0     2138 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/accelerators/test-lbfgs.cpp
+-rw-r--r--   0        0        0    12432 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/inner/test-panoc.cpp
+-rw-r--r--   0        0        0      674 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/outer/codegen-rosenbrock.py
+-rw-r--r--   0        0        0     2808 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/outer/matrices/test-alm.mat.ipp
+-rw-r--r--   0        0        0    32805 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/outer/rosenbrock_functions_test.c
+-rw-r--r--   0        0        0      177 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/outer/rosenbrock_functions_test.csv
+-rw-r--r--   0        0        0    13610 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/outer/test-alm.cpp
+-rw-r--r--   0        0        0     3034 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/outer/test-casadi.cpp
+-rw-r--r--   0        0        0    21867 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/problem/test-type-erased-problem.cpp
+-rw-r--r--   0        0        0     1938 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/test-util/eigen-matchers.hpp
+-rw-r--r--   0        0        0    10701 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/util/io/test-csv.cpp
+-rw-r--r--   0        0        0     1649 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/util/test-index-set.cpp
+-rw-r--r--   0        0        0     1648 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/util/test-print.cpp
+-rw-r--r--   0        0        0     1847 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/util/test-set-intersection.cpp
+-rw-r--r--   0        0        0     2516 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/util/test-sparse-ops.cpp
+-rw-r--r--   0        0        0    18232 2023-07-19 07:49:31.388498 alpaqa-1.0.0a7/test/util/test-type-erasure.cpp
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 alpaqa-1.0.0a7/PKG-INFO
```

### Comparing `alpaqa-1.0.0a6/LICENSE` & `alpaqa-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/README.md` & `alpaqa-1.0.0a7/python/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-# alpaqa
+alpaqa
+======
 
-`alpaqa` is an efficient implementation of an augmented Lagrangian method for
+``alpaqa`` is an efficient implementation of an augmented Lagrangian method for
 general nonlinear programming problems, which uses the first-order, matrix-free
 PANOC algorithm as an inner solver.
 The numerical algorithms themselves are implemented in C++ for optimal
 performance, and they are exposed as an easy-to-use Python package.
 
 The solvers in this library solve minimization problems of the following form:
 
-$$
-    \begin{equation}
-        \begin{aligned}
-            & \underset{x}{\textbf{minimize}}
-            & & f(x) &&&& f : {{\rm I\mathchoice{\hspace{-2pt}}{\hspace{-2pt}}{\hspace{-1.75pt}}{\hspace{-1.7pt}}R}}^n \rightarrow {{\rm I\mathchoice{\hspace{-2pt}}{\hspace{-2pt}}{\hspace{-1.75pt}}{\hspace{-1.7pt}}R}} \\
-            & \textbf{subject to}
-            & & \underline{x} \le x \le \overline{x} \\
-            &&& \underline{z} \le g(x) \le \overline{z} &&&& g : {{\rm I\mathchoice{\hspace{-2pt}}{\hspace{-2pt}}{\hspace{-1.75pt}}{\hspace{-1.7pt}}R}}^n \rightarrow {{\rm I\mathchoice{\hspace{-2pt}}{\hspace{-2pt}}{\hspace{-1.75pt}}{\hspace{-1.7pt}}R}}^m
-        \end{aligned}
-    \end{equation}
-$$
-
-## Documentation
-
-- [**Sphinx documentation**](https://kul-optec.github.io/alpaqa/develop/Sphinx/index.html)
-- [**Python examples**](https://kul-optec.github.io/alpaqa/develop/Sphinx/examples/examples_landing_page.html)
-- [**Doxygen documentation**](https://kul-optec.github.io/alpaqa/develop/Doxygen/index.html)
-- [**C++ examples**](https://kul-optec.github.io/alpaqa/develop/Doxygen/examples.html)
-
-## Installation
-
-The Python interface can be installed directly from [PyPI](https://pypi.org/project/alpaqa):
-
-```sh
-python3 -m pip install alpaqa
-```
+.. math::
+
+    \begin{aligned}
+        & \underset{x}{\textbf{minimize}}
+        & & f(x) &&&& f : {{\rm I\mathchoice{\hspace{-2pt}}{\hspace{-2pt}}{\hspace{-1.75pt}}{\hspace{-1.7pt}}R}}^n \rightarrow {{\rm I\mathchoice{\hspace{-2pt}}{\hspace{-2pt}}{\hspace{-1.75pt}}{\hspace{-1.7pt}}R}} \\
+        & \textbf{subject to}
+        & & \underline{x} \le x \le \overline{x} \\
+        &&& \underline{z} \le g(x) \le \overline{z} &&&& g : {{\rm I\mathchoice{\hspace{-2pt}}{\hspace{-2pt}}{\hspace{-1.75pt}}{\hspace{-1.7pt}}R}}^n \rightarrow {{\rm I\mathchoice{\hspace{-2pt}}{\hspace{-2pt}}{\hspace{-1.75pt}}{\hspace{-1.7pt}}R}}^m
+    \end{aligned}
+
+Documentation
+-------------
+
+- `Sphinx documentation <https://kul-optec.github.io/alpaqa/develop/Sphinx/index.html>`_
+- `Python examples <https://kul-optec.github.io/alpaqa/develop/Sphinx/examples/index.html>`_
+- `Doxygen documentation <https://kul-optec.github.io/alpaqa/develop/Doxygen/index.html>`_
+- `C++ examples <https://kul-optec.github.io/alpaqa/develop/Doxygen/examples.html>`_
+
+Installation
+------------
+
+The Python interface can be installed directly from PyPI:
+
+.. code-block:: sh
+
+    python3 -m pip install alpaqa
 
 For more information, please see the full
-[installation instructions](https://kul-optec.github.io/alpaqa/develop/Sphinx/install/installation.html).
+`installation instructions <https://kul-optec.github.io/alpaqa/develop/Sphinx/install/installation.html>`_.
 
-## Publications
+Publications
+------------
 
-- [P. Pas, M. Schuurmans, and P. Patrinos, “Alpaqa: A matrix-free solver for nonlinear MPC and large-scale nonconvex optimization,” _20th European Control Conference (ECC)_, Jul. 2022 (arXiv)](https://arxiv.org/abs/2112.02370)
+- `P. Pas, M. Schuurmans, and P. Patrinos, “Alpaqa: A matrix-free solver for nonlinear MPC and large-scale nonconvex optimization,” 20th European Control Conference (ECC), Jul. 2022 (arXiv) <https://arxiv.org/abs/2112.02370>`_
```

### Comparing `alpaqa-1.0.0a6/cmake/Sanitizers.cmake` & `alpaqa-1.0.0a7/cmake/Sanitizers.cmake`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/interfaces/python/cmake/Pybind11Stubgen.cmake` & `alpaqa-1.0.0a7/interfaces/python/cmake/Pybind11Stubgen.cmake`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/interfaces/python/cmake/QueryPythonForPybind11.cmake` & `alpaqa-1.0.0a7/interfaces/python/cmake/QueryPythonForPybind11.cmake`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/interfaces/python/src/enums.py.cpp` & `alpaqa-1.0.0a7/interfaces/python/src/enums.py.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 #include <alpaqa/accelerators/lbfgs.hpp>
 #include <alpaqa/inner/internal/panoc-stop-crit.hpp>
 #include <alpaqa/inner/internal/solverstatus.hpp>
-#include <alpaqa/problem/structure.hpp>
 #include <pybind11/pybind11.h>
 
 namespace py = pybind11;
 
 void register_enums(py::module_ &m) {
 
     py::enum_<alpaqa::LBFGSStepSize>(m, "LBFGSStepsize",
                                      "C++ documentation: :cpp:enum:`alpaqa::LBFGSStepSize`")
         .value("BasedOnExternalStepSize", alpaqa::LBFGSStepSize::BasedOnExternalStepSize)
         .value("BasedOnCurvature", alpaqa::LBFGSStepSize::BasedOnCurvature)
         .export_values();
 
-    py::enum_<alpaqa::CostStructure>(m, "CostStructure",
-                                     "C++ documentation: :cpp:enum:`alpaqa::CostStructure`")
-        .value("General", alpaqa::CostStructure::General)
-        .value("Separable", alpaqa::CostStructure::DiagonalHessian)
-        .value("Quadratic", alpaqa::CostStructure::Quadratic)
-        .value("SeparableQuadratic", alpaqa::CostStructure::DiagonalQuadratic)
-        .export_values();
-
     using SolverStatus = alpaqa::SolverStatus;
     py::enum_<SolverStatus>(m, "SolverStatus", py::arithmetic(),
                             "C++ documentation: :cpp:enum:`alpaqa::SolverStatus`")
         .value("Busy", SolverStatus::Busy, "In progress.")
         .value("Converged", SolverStatus::Converged, "Converged and reached given tolerance")
         .value("MaxTime", SolverStatus::MaxTime, "Maximum allowed execution time exceeded")
         .value("MaxIter", SolverStatus::MaxIter, "Maximum number of iterations exceeded")
```

### Comparing `alpaqa-1.0.0a6/interfaces/python/src/kwargs-to-struct.hpp` & `alpaqa-1.0.0a7/interfaces/python/src/dict/kwargs-to-struct.hpp`

 * *Files 23% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 
 #include <alpaqa/util/demangled-typename.hpp>
 #include <functional>
 #include <map>
 #include <typeinfo>
 #include <variant>
 
-#include <pybind11/detail/typeid.h>
+#include <pybind11/chrono.h>
 #include <pybind11/pybind11.h>
+#include <pybind11/stl.h>
 namespace py = pybind11;
 
 template <class T>
 T dict_to_struct(const py::dict &);
 
 struct cast_error_with_types : py::cast_error {
     cast_error_with_types(const py::cast_error &e, std::string from, std::string to)
@@ -56,37 +57,50 @@
 template <class T>
 using dict_to_struct_table_t = std::map<std::string, attr_setter_fun_t<T>>;
 
 template <class T>
 struct dict_to_struct_table {};
 
 template <class T>
+auto possible_dict_keys(const std::string &input) {
+    const auto &tbl = dict_to_struct_table<T>::table;
+    py::list keys;
+    for (const auto &[k, v] : tbl)
+        keys.append(py::str(k));
+    auto dl     = py::module::import("difflib");
+    auto sorted = dl.attr("get_close_matches")(input, keys, keys.size(), 0.);
+    return py::cast<std::string>(py::str(sorted));
+}
+
+template <class T>
     requires requires { dict_to_struct_table<T>::table; }
 void dict_to_struct_helper(T &t, const py::dict &kwargs) {
     const auto &m = dict_to_struct_table<T>::table;
     for (auto &&[key, val] : kwargs) {
         auto skey = key.template cast<std::string>();
         auto it   = m.find(skey);
         if (it == m.end())
-            throw py::key_error("Unknown parameter " + skey);
+            throw py::key_error("Unknown parameter '" + skey +
+                                "', possible keys are: " + possible_dict_keys<T>(skey));
         try {
             it->second.set(t, val);
         } catch (const cast_error_with_types &e) {
             throw std::runtime_error("Error converting parameter '" + skey + "' from " + e.from +
                                      " to '" + e.to + "': " + e.what());
         } catch (const std::runtime_error &e) {
             throw std::runtime_error("Error setting parameter '" + skey + "': " + e.what());
         }
     }
 }
 
 template <class T>
     requires(!requires { dict_to_struct_table<T>::table; })
 void dict_to_struct_helper(T &, const py::dict &) {
-    throw std::runtime_error("Cannot convert dict to '" + demangled_typename(typeid(T)) + '\'');
+    throw std::runtime_error("No known conversion from Python dict to C++ type '" +
+                             demangled_typename(typeid(T)) + '\'');
 }
 
 template <class T>
 py::dict struct_to_dict_helper(const T &t) {
     const auto &m = dict_to_struct_table<T>::table;
     py::dict d;
     for (auto &&[key, val] : m) {
@@ -120,14 +134,39 @@
 
 template <class T>
 T var_kwargs_to_struct(const params_or_dict<T> &p) {
     return std::holds_alternative<T>(p) ? std::get<T>(p)
                                         : kwargs_to_struct<T>(std::get<py::dict>(p));
 }
 
+/// Helper macro to easily specialize @ref dict_to_struct_table.
+#define PARAMS_TABLE_DECL(type_)                                                                   \
+    template <alpaqa::Config Conf>                                                                 \
+    struct dict_to_struct_table<type_> {                                                           \
+        using type = type_;                                                                        \
+        static const dict_to_struct_table_t<type> table;                                           \
+    }
+
+/// Helper macro to easily initialize a
+/// @ref dict_to_struct_table_t.
+#define PARAMS_MEMBER(name)                                                                        \
+    {                                                                                              \
+#name, &type::name                                                                         \
+    }
+
+/// Helper macro to easily define a specialization @ref dict_to_struct_table.
+#define PARAMS_TABLE_DEF(type_, ...)                                                               \
+    template <alpaqa::Config Conf>                                                                 \
+    const dict_to_struct_table_t<type_> dict_to_struct_table<type_>::table {                       \
+        __VA_ARGS__                                                                                \
+    }
+
+/// Helper macro to easily instantiate a @ref dict_to_struct_table.
+#define PARAMS_TABLE_INST(type_) template struct dict_to_struct_table<type_>
+
 #if 0
 #include <alpaqa/inner/pga.hpp>
 
 template <>
 inline const dict_to_struct_table_t<alpaqa::PGAParams>
     dict_to_struct_table<alpaqa::PGAParams>{
         {"Lipschitz", &alpaqa::PGAParams::Lipschitz},
@@ -161,47 +200,25 @@
         {"linesearch_tolerance_factor",
          &alpaqa::GAAPGAParams::linesearch_tolerance_factor},
         {"max_no_progress", &alpaqa::GAAPGAParams::max_no_progress},
         {"full_flush_on_γ_change",
          &alpaqa::GAAPGAParams::full_flush_on_γ_change},
     };
 
-#include <alpaqa/inner/decl/structured-panoc-lbfgs.hpp>
-
-template <>
-inline const dict_to_struct_table_t<alpaqa::StructuredPANOCLBFGSParams>
-    dict_to_struct_table<alpaqa::StructuredPANOCLBFGSParams>{
-        {"Lipschitz", &alpaqa::StructuredPANOCLBFGSParams::Lipschitz},
-        {"max_iter", &alpaqa::StructuredPANOCLBFGSParams::max_iter},
-        {"max_time", &alpaqa::StructuredPANOCLBFGSParams::max_time},
-        {"τ_min", &alpaqa::StructuredPANOCLBFGSParams::τ_min},
-        {"L_min", &alpaqa::StructuredPANOCLBFGSParams::L_min},
-        {"L_max", &alpaqa::StructuredPANOCLBFGSParams::L_max},
-        {"nonmonotone_linesearch",
-         &alpaqa::StructuredPANOCLBFGSParams::nonmonotone_linesearch},
-        {"fpr_shortcut_accept_factor",
-         &alpaqa::StructuredPANOCLBFGSParams::fpr_shortcut_accept_factor},
-        {"fpr_shortcut_history",
-         &alpaqa::StructuredPANOCLBFGSParams::fpr_shortcut_history},
-        {"stop_crit", &alpaqa::StructuredPANOCLBFGSParams::stop_crit},
-        {"max_no_progress",
-         &alpaqa::StructuredPANOCLBFGSParams::max_no_progress},
-        {"print_interval", &alpaqa::StructuredPANOCLBFGSParams::print_interval},
-        {"quadratic_upperbound_tolerance_factor",
-         &alpaqa::StructuredPANOCLBFGSParams::
-             quadratic_upperbound_tolerance_factor},
-        {"linesearch_tolerance_factor",
-         &alpaqa::StructuredPANOCLBFGSParams::
-             linesearch_tolerance_factor},
-        {"update_lipschitz_in_linesearch",
-         &alpaqa::StructuredPANOCLBFGSParams::update_lipschitz_in_linesearch},
-        {"alternative_linesearch_cond",
-         &alpaqa::StructuredPANOCLBFGSParams::alternative_linesearch_cond},
-        {"hessian_vec", &alpaqa::StructuredPANOCLBFGSParams::hessian_vec},
-        {"hessian_vec_finite_differences",
-         &alpaqa::StructuredPANOCLBFGSParams::hessian_vec_finite_differences},
-        {"full_augmented_hessian",
-         &alpaqa::StructuredPANOCLBFGSParams::full_augmented_hessian},
-        {"hessian_step_size_heuristic",
-         &alpaqa::StructuredPANOCLBFGSParams::hessian_step_size_heuristic},
-    };
 #endif
+
+template <class T>
+void make_dataclass(py::class_<T> &cls) {
+    cls //
+        .def(py::init(&dict_to_struct<T>))
+        .def(py::init(&kwargs_to_struct<T>))
+        .def("to_dict", &struct_to_dict<T>);
+    for (auto &&[key, getset] : dict_to_struct_table<T>::table)
+        cls.def_property(key.c_str(), getset.get, getset.set);
+}
+
+template <class T, class... Extra>
+auto register_dataclass(py::handle scope, const char *name, const Extra &...extra) {
+    py::class_<T> cls(scope, name, extra...);
+    make_dataclass(cls);
+    return cls;
+}
```

### Comparing `alpaqa-1.0.0a6/interfaces/python/src/type-erased-inner-solver.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/enumerate.hpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 #pragma once
 
-#include <alpaqa/problem/type-erased-problem.hpp>
-#include "type-erased-solver-stats.hpp"
+#include <ranges>
+#include <utility>
 
-namespace alpaqa {
+namespace alpaqa::util {
 
-template <Config Conf>
-struct InnerSolverVTable : util::BasicVTable {
-    USING_ALPAQA_CONFIG(Conf);
-    using Stats   = TypeErasedInnerSolverStats<Conf>;
-    using Problem = TypeErasedProblem<Conf>;
-
-    // clang-format off
-    required_function_t<Stats(const Problem &, crvec, real_t, bool, rvec, rvec, rvec)>
-        call = nullptr;
-    required_function_t<void()>
-        stop = nullptr;
-    required_const_function_t<std::string()>
-        get_name = nullptr;
-    // clang-format on
-
-    template <class T>
-    InnerSolverVTable(util::VTableTypeTag<T> t) : util::BasicVTable{t} {
-        stop     = util::type_erased_wrapped<&T::stop>();
-        get_name = util::type_erased_wrapped<&T::get_name>();
-        call     = [](void *self, const Problem &p, auto... valargs) {
-            constexpr auto call = util::type_erased_wrapped<&T::operator()>();
-            return Stats{call(self, p, valargs...)};
-        };
-    }
-    InnerSolverVTable() = default;
-};
+template <class Rng>
+struct enumerate_t : std::ranges::view_interface<enumerate_t<Rng>> {
+    Rng rng;
+
+    // P2325R3: https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2021/p2325r3.html
+    enumerate_t() = default;
+    enumerate_t(Rng rng) : rng{std::forward<Rng>(rng)} {}
+
+    using begin_t = decltype(std::ranges::begin(std::as_const(rng)));
+    using end_t   = decltype(std::ranges::end(std::as_const(rng)));
+
+    struct sentinel_t {
+        end_t it;
+    };
+
+    struct iter_t {
+        // P2325R3: https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2021/p2325r3.html
+        iter_t() = default;
+        iter_t(begin_t &&it) : it{std::forward<begin_t>(it)} {}
+
+        using index_t = std::ranges::range_difference_t<Rng>;
+        index_t index{};
+        begin_t it;
+
+        using difference_type = std::ptrdiff_t;
+        using value_type      = std::tuple<index_t, decltype(*it)>;
+
+        bool operator!=(sentinel_t s) const { return s.it != it; }
+        bool operator==(sentinel_t s) const { return s.it == it; }
+        // TODO: For Clang bug
+        friend bool operator!=(sentinel_t s, const iter_t &i) { return i != s; }
+        friend bool operator==(sentinel_t s, const iter_t &i) { return i == s; }
+
+        iter_t &operator++() {
+            ++it;
+            ++index;
+            return *this;
+        }
+        iter_t operator++(int) const {
+            auto tmp = *this;
+            ++*this;
+            return tmp;
+        }
 
-template <Config Conf = DefaultConfig, class Allocator = std::allocator<std::byte>>
-class TypeErasedInnerSolver : util::TypeErased<InnerSolverVTable<Conf>, Allocator> {
-  public:
-    USING_ALPAQA_CONFIG(Conf);
-    using VTable         = InnerSolverVTable<Conf>;
-    using allocator_type = Allocator;
-    using TypeErased     = util::TypeErased<VTable, allocator_type>;
-    using Stats          = typename VTable::Stats;
-    using TypeErased::TypeErased;
-
-  private:
-    using TypeErased::self;
-    using TypeErased::vtable;
-
-  public:
-    template <class T, class... Args>
-    static TypeErasedInnerSolver make(Args &&...args) {
-        return TypeErased::template make<TypeErasedInnerSolver, T>(std::forward<Args>(args)...);
-    }
+        value_type operator*() const { return {index, *it}; }
+    };
 
-    template <class... Args>
-    decltype(auto) operator()(Args &&...args) {
-        return vtable.call(self, std::forward<Args>(args)...);
+    auto begin() const -> std::input_or_output_iterator auto{
+        return iter_t{std::ranges::begin(rng)};
     }
-    template <class... Args>
-    decltype(auto) stop(Args &&...args) {
-        return vtable.stop(self, std::forward<Args>(args)...);
-    }
-    template <class... Args>
-    decltype(auto) get_name(Args &&...args) const {
-        return vtable.get_name(self, std::forward<Args>(args)...);
+    auto end() const
+    // -> std::sentinel_for<iter_t> auto
+    {
+        return sentinel_t{std::ranges::end(rng)};
     }
 };
 
-} // namespace alpaqa
+template <class Rng>
+auto enumerate(Rng &&rng) {
+    return enumerate_t<std::views::all_t<Rng>>{std::forward<Rng>(rng)};
+}
+
+} // namespace alpaqa::util
```

### Comparing `alpaqa-1.0.0a6/interfaces/python/src/type-erased-panoc-direction.hpp` & `alpaqa-1.0.0a7/interfaces/python/src/inner/type-erased-panoc-direction.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 #pragma once
 
 #include <alpaqa/config/config.hpp>
 #include <alpaqa/inner/directions/panoc-direction-update.hpp>
 #include <alpaqa/inner/directions/panoc/lbfgs.hpp>
 #include <alpaqa/util/type-erasure.hpp>
 
+#include <dict/dict-tup.hpp>
+#include <dict/kwargs-to-struct.hpp>
+
 #include <new>
 #include <string>
 #include <utility>
 
+#include <pybind11/pytypes.h>
+namespace py = pybind11;
+
 namespace alpaqa {
 
 template <Config Conf>
 struct PANOCDirectionVTable : util::BasicVTable {
     USING_ALPAQA_CONFIG(Conf);
     using Problem = TypeErasedProblem<config_t>;
 
     // clang-format off
     required_function_t<void(const Problem &problem, crvec y, crvec Σ, real_t γ_0, crvec x_0, crvec x̂_0, crvec p_0, crvec grad_ψx_0)>
         initialize = nullptr;
     required_function_t<bool(real_t γₖ, real_t γₙₑₓₜ, crvec xₖ, crvec xₙₑₓₜ, crvec pₖ, crvec pₙₑₓₜ, crvec grad_ψxₖ, crvec grad_ψxₙₑₓₜ)>
         update = nullptr;
+    required_const_function_t<bool()>
+        has_initial_direction = nullptr;
     required_const_function_t<bool(real_t γₖ, crvec xₖ, crvec x̂ₖ, crvec pₖ, crvec grad_ψxₖ, rvec qₖ)>
         apply = nullptr;
     required_function_t<void(real_t γₖ, real_t old_γₖ)>
         changed_γ = nullptr;
     required_function_t<void()>
         reset = nullptr;
+    required_const_function_t<py::object()>
+        get_params = nullptr;
     required_const_function_t<std::string()>
         get_name = nullptr;
     // clang-format on
 
     template <class T>
-    PANOCDirectionVTable(util::VTableTypeTag<T> t) : util::BasicVTable{t} {
-        initialize = util::type_erased_wrapped<&T::initialize>();
-        update     = util::type_erased_wrapped<&T::update>();
-        apply      = util::type_erased_wrapped<&T::apply>();
-        changed_γ  = util::type_erased_wrapped<&T::changed_γ>();
-        reset      = util::type_erased_wrapped<&T::reset>();
-        get_name   = util::type_erased_wrapped<&T::get_name>();
+    PANOCDirectionVTable(std::in_place_t, T &t) : util::BasicVTable{std::in_place, t} {
+        initialize            = util::type_erased_wrapped<T, &T::initialize>();
+        update                = util::type_erased_wrapped<T, &T::update>();
+        has_initial_direction = util::type_erased_wrapped<T, &T::has_initial_direction>();
+        apply                 = util::type_erased_wrapped<T, &T::apply>();
+        changed_γ             = util::type_erased_wrapped<T, &T::changed_γ>();
+        reset                 = util::type_erased_wrapped<T, &T::reset>();
+        get_params            = util::type_erased_wrapped<T, &T::get_params>();
+        get_name              = util::type_erased_wrapped<T, &T::get_name>();
     }
     PANOCDirectionVTable() = default;
 };
 
 template <Config Conf>
-constexpr size_t te_pd_buff_size = util::required_te_buffer_size_for<PANOCDirection<LBFGS<Conf>>>();
+constexpr size_t te_pd_buff_size = util::required_te_buffer_size_for<LBFGSDirection<Conf>>();
 
 template <Config Conf = DefaultConfig, class Allocator = std::allocator<std::byte>>
 class TypeErasedPANOCDirection
     : public util::TypeErased<PANOCDirectionVTable<Conf>, Allocator, te_pd_buff_size<Conf>> {
   public:
     USING_ALPAQA_CONFIG(Conf);
     using VTable         = PANOCDirectionVTable<Conf>;
@@ -73,39 +85,45 @@
         return call(vtable.initialize, std::forward<Args>(args)...);
     }
     template <class... Args>
     decltype(auto) update(Args &&...args) {
         return call(vtable.update, std::forward<Args>(args)...);
     }
     template <class... Args>
+    decltype(auto) has_initial_direction(Args &&...args) const {
+        return call(vtable.has_initial_direction, std::forward<Args>(args)...);
+    }
+    template <class... Args>
     decltype(auto) apply(Args &&...args) const {
         return call(vtable.apply, std::forward<Args>(args)...);
     }
     template <class... Args>
     decltype(auto) changed_γ(Args &&...args) {
         return call(vtable.changed_γ, std::forward<Args>(args)...);
     }
     template <class... Args>
     decltype(auto) reset(Args &&...args) {
         return call(vtable.reset, std::forward<Args>(args)...);
     }
     template <class... Args>
+    decltype(auto) get_params(Args &&...args) const {
+        return call(vtable.get_params, std::forward<Args>(args)...);
+    }
+    template <class... Args>
     decltype(auto) get_name(Args &&...args) const {
         return call(vtable.get_name, std::forward<Args>(args)...);
     }
 };
 
-template <Config Conf>
-struct PANOCDirection<TypeErasedPANOCDirection<Conf>> : TypeErasedPANOCDirection<Conf> {
-    PANOCDirection(const TypeErasedPANOCDirection<Conf> &other)
-        : TypeErasedPANOCDirection<Conf>(other) {}
-    PANOCDirection(TypeErasedPANOCDirection<Conf> &&other)
-        : TypeErasedPANOCDirection<Conf>(std::move(other)) {}
-};
-
 template <class T, class... Args>
-auto erase_direction(Args &&...args) {
-    return TypeErasedPANOCDirection<typename T::config_t>::template make<PANOCDirection<T>>(
+auto erase_direction_with_params_dict(Args &&...args) {
+    struct DirectionWrapper : T {
+        DirectionWrapper(const T &d) : T{d} {}
+        DirectionWrapper(T &&d) : T{std::move(d)} {}
+        using T::T;
+        py::object get_params() const { return to_dict_tup(T::get_params()); }
+    };
+    return TypeErasedPANOCDirection<typename T::config_t>::template make<DirectionWrapper>(
         std::forward<Args>(args)...);
 }
 
 } // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/pyproject.toml` & `alpaqa-1.0.0a7/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,101 @@
 [project]
 name = "alpaqa"
 readme = "python/README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = { "file" = "LICENSE" }
 authors = [{ "name" = "Pieter P", "email" = "pieter.p.dev@outlook.com" }]
 keywords = ["optimization", "panoc", "alm", "mpc"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
 ]
-dependencies = ["numpy", "casadi"]
+dependencies = ["numpy", "casadi~=3.6.0"]
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
-docs = [
-    "sphinx~=5.1",
-    "matplotlib",
-    "breathe",
-    "furo",
-]
+docs = ["sphinx>=5.1,<7.1", "matplotlib", "breathe", "furo"]
+debug = ["alpaqa-debug==1.0.0a7"]
+test = ["pytest>=7.2.0,<7.5", "qpalm~=1.1.4", "scipy>=1.9.3,<1.12"]
 
 [project.urls]
 "Documentation" = "https://kul-optec.github.io/alpaqa"
 "Source" = "https://github.com/kul-optec/alpaqa"
 "Bug Tracker" = "https://github.com/kul-optec/alpaqa/issues"
 
 [project.scripts]
 alpaqa = "alpaqa.__main__:main"
 
 [build-system]
-requires = ["py-build-cmake~=0.0.16a2", "pybind11", "pybind11-stubgen"]
+requires = [
+    "py-build-cmake~=0.1.8",
+    "pybind11>=2.10.1,!=2.10.2,!=2.10.3,!=2.10.4",
+    "pybind11-stubgen",
+]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module]
 name = "alpaqa"
 directory = "python"
 
 [tool.py-build-cmake.sdist]
-include = ["README.md", "CMakeLists.txt", "src", "cmake", "interfaces"]
+include = [
+    "README.md",
+    "CMakeLists.txt",
+    "src",
+    "cmake",
+    "interfaces",
+    "applications",
+    "test",
+]
 exclude = []
 
 [tool.py-build-cmake.cmake]
-minimum_version = "3.21"
+minimum_version = "3.24"
 source_path = "."
 config = []
 args = ["-Wdev"]
 build_args = ["-j"]
 install_components = ["python_modules", "python_stubs"]
 [tool.py-build-cmake.cmake.options]
 "ALPAQA_WITH_PYTHON:BOOL" = "On"
-"ALPAQA_WITH_PY_STUBS:BOOL" = "On"
 "ALPAQA_WITH_TESTS:BOOL" = "Off"
 "ALPAQA_WITH_EXAMPLES:BOOL" = "Off"
+"ALPAQA_WITH_DRIVERS:BOOL" = "Off"
 "ALPAQA_WITH_QUAD_PRECISION:BOOL" = "Off"
 "ALPAQA_WITH_UBSAN_DEBUG:BOOL" = "Off"
 "ALPAQA_WITH_ASAN_DEBUG:BOOL" = "Off"
-"ALPAQA_INCLUDE_DEBUG_INFO:BOOL" = "Off"
 
 [tool.py-build-cmake.linux.cmake]
 config = ["Debug", "Release"]
 generator = "Ninja Multi-Config"
 [tool.py-build-cmake.mac.cmake]
 config = ["Debug", "Release"]
 generator = "Ninja Multi-Config"
 [tool.py-build-cmake.windows.cmake]
-config = ["Release"]
+config = ["RelWithDebInfo", "Release"]
+[tool.py-build-cmake.windows.cmake.options]
+CMAKE_CXX_FLAGS_RELWITHDEBINFO = "/Zi /Ob0 /Od /RTC1"
+CMAKE_MODULE_LINKER_FLAGS_RELWITHDEBINFO = "/INCREMENTAL:NO /DEBUG:FULL /OPT:REF"
+ALPAQA_PYTHON_DEBUG_CONFIG = "RelWithDebInfo"
 
 [tool.py-build-cmake.stubgen]
 args = ["-v"]
 
+[tool.py-build-cmake.editable]
+mode = "symlink"
+
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["python/test"]
 
 [tool.mypy]
 plugins = ["numpy.typing.mypy_plugin"]
-
-[tool.pyright]
-# Pyright stops looking after the first match, which is usually in the 
-# site-packages folder. When doing an editable install, it should look in both
-# site-packages and the source folder. To get the search order correct, 
-# explicitly point it to the source folder first (it will still look for the C++ 
-# extension module stubs in site-packages).
-extraPaths = ["python"]
```

### Comparing `alpaqa-1.0.0a6/python/alpaqa/__main__.py` & `alpaqa-1.0.0a7/python/alpaqa/__main__.py`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/src/alpaqa.dox` & `alpaqa-1.0.0a7/src/alpaqa.dox`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * @defgroup    grp_ALMSolver Augmented Lagrangian Method solver 
+ * @defgroup    grp_ALMSolver Augmented Lagrangian solver 
  * @brief   Augmented Lagrangian Method solver (ALM).
  */
 
 /**
  * @defgroup    grp_InnerSolvers Inner solvers
  * @brief   Solvers for the inner problem, such as PANOC.
  */
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/accelerators/lbfgs.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/accelerators/lbfgs.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 
     /// The sign of the vectors @f$ p @f$ passed to the @ref update method.
     enum class Sign {
         Positive, ///< @f$ p \sim \nabla \psi(x) @f$
         Negative, ///< @f$ p \sim -\nabla \psi(x) @f$
     };
 
+    LBFGS() = default;
     LBFGS(Params params) : params(params) {}
     LBFGS(Params params, length_t n) : params(params) { resize(n); }
 
     /// Check if the new vectors s and y allow for a valid BFGS update that
     /// preserves the positive definiteness of the Hessian approximation.
     static bool update_valid(const Params &params, real_t yᵀs, real_t sᵀs,
                              real_t pᵀp);
@@ -141,17 +142,17 @@
     /// Initial inverse Hessian approximation is set to @f$ H_0 = \gamma I @f$.
     /// If @p γ is negative, @f$ H_0 = \frac{s^\top y}{y^\top y} I @f$.
     bool apply(rvec q, real_t γ = -1) const;
 
     /// Apply the inverse Hessian approximation to the given vector q, applying
     /// only the columns and rows of the Hessian in the index set J.
     bool apply_masked(rvec q, real_t γ, crindexvec J) const;
-    /// @copydoc apply_masked(rvec, real_t, crindexvec)
+    /// @copydoc apply_masked(rvec, real_t, crindexvec) const
     bool apply_masked(rvec q, real_t γ, const std::vector<index_t> &J) const;
-    /// @see @ref apply_masked
+    /// @copydoc apply_masked(rvec, real_t, crindexvec) const
     bool apply_masked_impl(rvec q, real_t γ, const auto &J) const;
 
     /// Throw away the approximation and all previous vectors s and y.
     void reset();
     /// Re-allocate storage for a problem with a different size. Causes
     /// a @ref reset.
     void resize(length_t n);
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/accelerators/src/lbfgs.tpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/accelerators/lbfgs.tpp`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         // case for the smaller vectors s(J) and y(J).
         real_t yᵀs = dotJ(s(i), y(i));
         real_t sᵀs = dotJ(s(i), s(i));
         ρ(i)       = 1 / yᵀs;
         // Check if we should include this pair of vectors
         if (not update_valid(params, yᵀs, sᵀs, 0)) {
             ρ(i) = NaN<config_t>;
-            return;
+            return; // continue foreach
         }
 
         α(i) = ρ(i) * dotJ(s(i), q); // αᵢ = ρᵢ〈sᵢ, q〉
         axmyJ(α(i), y(i), q);        // q -= αᵢ yᵢ
 
         if (γ < 0) {
             // Compute step size based on most recent valid yᵀs/yᵀy
@@ -179,15 +179,16 @@
         return false;
 
     // r ← H_0 q
     scalJ(γ, q); // q *= γ
 
     foreach_fwd([&](index_t i) {
         if (std::isnan(ρ(i)))
-            return;
+            return; // continue foreach
+
         real_t β = ρ(i) * dotJ(y(i), q); // βᵢ = ρᵢ〈yᵢ, q〉
         axmyJ(β - α(i), s(i), q);        // q -= (βᵢ - αᵢ) sᵢ
     });
 
     return true;
 }
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/casadi-loader-export.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/casadi-loader-export.hpp`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/config/config.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/config/config.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,21 @@
 struct DefaultConfig;
 template <>
 struct is_config<DefaultConfig> : std::true_type {};
 
 #define USING_ALPAQA_CONFIG_NO_TYPENAME(Conf)                                  \
     using real_t [[maybe_unused]]     = Conf::real_t;                          \
     using vec [[maybe_unused]]        = Conf::vec;                             \
+    using mvec [[maybe_unused]]       = Conf::mvec;                            \
+    using cmvec [[maybe_unused]]      = Conf::cmvec;                           \
     using rvec [[maybe_unused]]       = Conf::rvec;                            \
     using crvec [[maybe_unused]]      = Conf::crvec;                           \
     using mat [[maybe_unused]]        = Conf::mat;                             \
+    using mmat [[maybe_unused]]       = Conf::mmat;                            \
+    using cmmat [[maybe_unused]]      = Conf::cmmat;                           \
     using rmat [[maybe_unused]]       = Conf::rmat;                            \
     using crmat [[maybe_unused]]      = Conf::crmat;                           \
     using length_t [[maybe_unused]]   = Conf::length_t;                        \
     using index_t [[maybe_unused]]    = Conf::index_t;                         \
     using indexvec [[maybe_unused]]   = Conf::indexvec;                        \
     using rindexvec [[maybe_unused]]  = Conf::rindexvec;                       \
     using crindexvec [[maybe_unused]] = Conf::crindexvec
@@ -42,17 +46,21 @@
 #define USING_ALPAQA_CONFIG_TEMPLATE(Conf) /** @cond CONFIG_TYPES */           \
     using config_t [[maybe_unused]] = typename Conf;                           \
     USING_ALPAQA_CONFIG_NO_TYPENAME(typename Conf) /** @endcond */
 
 // clang-format off
 template <Config Conf = DefaultConfig> using real_t = typename Conf::real_t;
 template <Config Conf = DefaultConfig> using vec = typename Conf::vec;
+template <Config Conf = DefaultConfig> using mvec = typename Conf::mvec;
+template <Config Conf = DefaultConfig> using cmvec = typename Conf::cmvec;
 template <Config Conf = DefaultConfig> using rvec = typename Conf::rvec;
 template <Config Conf = DefaultConfig> using crvec = typename Conf::crvec;
 template <Config Conf = DefaultConfig> using mat = typename Conf::mat;
+template <Config Conf = DefaultConfig> using mmat = typename Conf::mmat;
+template <Config Conf = DefaultConfig> using cmmat = typename Conf::cmmat;
 template <Config Conf = DefaultConfig> using rmat = typename Conf::rmat;
 template <Config Conf = DefaultConfig> using crmat = typename Conf::crmat;
 template <Config Conf = DefaultConfig> using length_t = typename Conf::length_t;
 template <Config Conf = DefaultConfig> using index_t = typename Conf::index_t;
 template <Config Conf = DefaultConfig> using indexvec = typename Conf::indexvec;
 template <Config Conf = DefaultConfig> using rindexvec = typename Conf::rindexvec;
 template <Config Conf = DefaultConfig> using crindexvec = typename Conf::crindexvec;
@@ -65,20 +73,28 @@
 
 template <class RealT>
 struct EigenConfig {
     /// Real scalar element type.
     using real_t = RealT;
     /// Dynamic vector type.
     using vec = Eigen::VectorX<real_t>;
+    /// Map of vector type.
+    using mvec = Eigen::Map<vec>;
+    /// Immutable map of vector type.
+    using cmvec = Eigen::Map<const vec>;
     /// Reference to mutable vector.
     using rvec = Eigen::Ref<vec>;
     /// Reference to immutable vector.
     using crvec = Eigen::Ref<const vec>;
     /// Dynamic matrix type.
     using mat = Eigen::MatrixX<real_t>;
+    /// Map of matrix type.
+    using mmat = Eigen::Map<mat>;
+    /// Immutable map of matrix type.
+    using cmmat = Eigen::Map<const mat>;
     /// Reference to mutable matrix.
     using rmat = Eigen::Ref<mat>;
     /// Reference to immutable matrix.
     using crmat = Eigen::Ref<const mat>;
     /// Type for lengths and sizes.
     using length_t = Eigen::Index;
     /// Type for vector and matrix indices.
@@ -87,24 +103,29 @@
     using indexvec = Eigen::VectorX<index_t>;
     /// Reference to mutable index vector.
     using rindexvec = Eigen::Ref<indexvec>;
     /// Reference to immutable index vector.
     using crindexvec = Eigen::Ref<const indexvec>;
 };
 
+/// Single-precision `float` configuration.
 struct EigenConfigf : EigenConfig<float> {
     static constexpr const char *get_name() { return "EigenConfigf"; }
 };
+/// Double-precision `double` configuration.
 struct EigenConfigd : EigenConfig<double> {
     static constexpr const char *get_name() { return "EigenConfigd"; }
 };
+/// `long double` configuration. (Quad precision on ARM64, 80-bit x87 floats
+/// on Intel/AMD x86)
 struct EigenConfigl : EigenConfig<long double> {
     static constexpr const char *get_name() { return "EigenConfigl"; }
 };
 #ifdef ALPAQA_WITH_QUAD_PRECISION
+/// Quad-precision `__float128` configuration.
 struct EigenConfigq : EigenConfig<__float128> {
     static constexpr const char *get_name() { return "EigenConfigq"; }
 };
 template <>
 struct is_config<EigenConfigq> : std::true_type {};
 #endif
 
@@ -113,37 +134,32 @@
 template <>
 struct is_config<EigenConfigf> : std::true_type {};
 template <>
 struct is_config<EigenConfigd> : std::true_type {};
 template <>
 struct is_config<EigenConfigl> : std::true_type {};
 
-namespace vec_util {
+/// Global empty vector for convenience.
+template <Config Conf>
+inline const rvec<Conf> null_vec = mvec<Conf>{nullptr, 0};
 
-/// Get the Σ norm squared of a given vector, with Σ a diagonal matrix.
-/// @returns @f$ \langle v, \Sigma v \rangle @f$
-template <class Derived>
-auto norm_squared_weighted(const Eigen::MatrixBase<Derived> &v,
-                           const Eigen::MatrixBase<Derived> &Σ) //
-    requires(Derived::ColsAtCompileTime == 1) {
-    return v.dot(Σ.asDiagonal() * v);
-}
+namespace vec_util {
 
 /// Get the maximum or infinity-norm of the given vector.
 /// @returns @f$ \left\|v\right\|_\infty @f$
 template <class Derived>
-auto norm_inf(const Eigen::MatrixBase<Derived> &v) //
-    requires(Derived::ColsAtCompileTime == 1) {
+    requires(Derived::ColsAtCompileTime == 1)
+auto norm_inf(const Eigen::MatrixBase<Derived> &v) {
     return v.template lpNorm<Eigen::Infinity>();
 }
 
 /// Get the 1-norm of the given vector.
 /// @returns @f$ \left\|v\right\|_1 @f$
 template <class Derived>
-auto norm_1(const Eigen::MatrixBase<Derived> &v) //
-    requires(Derived::ColsAtCompileTime == 1) {
+    requires(Derived::ColsAtCompileTime == 1)
+auto norm_1(const Eigen::MatrixBase<Derived> &v) {
     return v.template lpNorm<1>();
 }
 
 } // namespace vec_util
 
-} // namespace alpaqa
+} // namespace alpaqa
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/export.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/export.hpp`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/inner/directions/panoc-direction-update.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/directions/panoc-direction-update.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #pragma once
 
 #include <alpaqa/config/config.hpp>
 #include <alpaqa/problem/type-erased-problem.hpp>
 
 namespace alpaqa {
 
+/// This class outlines the interface for direction providers used by PANOC-like
+/// algorithms.
+///
 /// @ingroup grp_DirectionProviders
-template <class DirectionProviderT>
+template <Config Conf>
 struct PANOCDirection {
-    USING_ALPAQA_CONFIG_TEMPLATE(DirectionProviderT::config_t);
+    USING_ALPAQA_CONFIG(Conf);
     using Problem = TypeErasedProblem<config_t>;
 
     /// Initialize the direction provider.
     ///
     /// @param[in]  problem
     ///             Problem description.
     /// @param[in]  y
@@ -32,14 +35,18 @@
     ///
     /// The references @p problem, @p y and @p Σ are guaranteed to remain valid
     /// for subsequent calls to @ref update, @ref apply, @ref changed_γ and
     /// @ref reset.
     void initialize(const Problem &problem, crvec y, crvec Σ, real_t γ_0,
                     crvec x_0, crvec x̂_0, crvec p_0, crvec grad_ψx_0) = delete;
 
+    /// Return whether a direction is available on the very first iteration,
+    /// before the first call to @ref update.
+    bool has_initial_direction() const = delete;
+
     /// Update the direction provider when accepting the next iterate.
     ///
     /// @param[in]  γₖ
     ///             Current step size.
     /// @param[in]  γₙₑₓₜ
     ///             Step size for the next iterate.
     /// @param[in]  xₖ
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/inner/directions/panoc/lbfgs.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/directions/panoc/lbfgs.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -2,68 +2,93 @@
 
 #include <alpaqa/accelerators/lbfgs.hpp>
 #include <alpaqa/inner/directions/panoc-direction-update.hpp>
 #include <alpaqa/problem/type-erased-problem.hpp>
 
 namespace alpaqa {
 
+/// Parameters for the @ref LBFGSDirection class.
+template <Config Conf>
+struct LBFGSDirectionParams {
+    bool rescale_on_step_size_changes = false;
+};
+
 /// @ingroup grp_DirectionProviders
 template <Config Conf>
-struct PANOCDirection<LBFGS<Conf>> {
+struct LBFGSDirection {
     USING_ALPAQA_CONFIG(Conf);
 
-    using Problem = TypeErasedProblem<Conf>;
-    using LBFGS   = alpaqa::LBFGS<Conf>;
+    using Problem           = TypeErasedProblem<config_t>;
+    using LBFGS             = alpaqa::LBFGS<config_t>;
+    using AcceleratorParams = typename LBFGS::Params;
+    using DirectionParams   = LBFGSDirectionParams<config_t>;
 
     LBFGS lbfgs;
 
-    struct ExtraParams {
-        bool rescale_when_γ_changes = false;
+    struct Params {
+        AcceleratorParams accelerator = {};
+        DirectionParams direction     = {};
     };
-    struct Params : LBFGS::Params, ExtraParams {};
 
-    PANOCDirection(const Params &params) : lbfgs(params), extraparams(params) {}
-    PANOCDirection(const typename LBFGS::Params &params,
-                   const ExtraParams &extraparams = {})
-        : lbfgs(params), extraparams(extraparams) {}
-    PANOCDirection(const LBFGS &lbfgs, const ExtraParams &extraparams = {})
-        : lbfgs(lbfgs), extraparams(extraparams) {}
-    PANOCDirection(LBFGS &&lbfgs, const ExtraParams &extraparams = {})
-        : lbfgs(std::move(lbfgs)), extraparams(extraparams) {}
+    LBFGSDirection() = default;
+    LBFGSDirection(const Params &params)
+        : lbfgs(params.accelerator), direction_params(params.direction) {}
+    LBFGSDirection(const typename LBFGS::Params &params,
+                   const DirectionParams &directionparams = {})
+        : lbfgs(params), direction_params(directionparams) {}
+    LBFGSDirection(const LBFGS &lbfgs,
+                   const DirectionParams &directionparams = {})
+        : lbfgs(lbfgs), direction_params(directionparams) {}
+    LBFGSDirection(LBFGS &&lbfgs, const DirectionParams &directionparams = {})
+        : lbfgs(std::move(lbfgs)), direction_params(directionparams) {}
 
+    /// @see @ref PANOCDirection::initialize
     void initialize(const Problem &problem, [[maybe_unused]] crvec y,
                     [[maybe_unused]] crvec Σ, [[maybe_unused]] real_t γ_0,
                     [[maybe_unused]] crvec x_0, [[maybe_unused]] crvec x̂_0,
                     [[maybe_unused]] crvec p_0,
                     [[maybe_unused]] crvec grad_ψx_0) {
         lbfgs.resize(problem.get_n());
     }
 
+    /// @see @ref PANOCDirection::has_initial_direction
+    bool has_initial_direction() const { return false; }
+
+    /// @see @ref PANOCDirection::update
     bool update([[maybe_unused]] real_t γₖ, [[maybe_unused]] real_t γₙₑₓₜ,
                 crvec xₖ, crvec xₙₑₓₜ, crvec pₖ, crvec pₙₑₓₜ,
                 [[maybe_unused]] crvec grad_ψxₖ,
                 [[maybe_unused]] crvec grad_ψxₙₑₓₜ) {
         return lbfgs.update(xₖ, xₙₑₓₜ, pₖ, pₙₑₓₜ, LBFGS::Sign::Negative);
     }
 
+    /// @see @ref PANOCDirection::apply
     bool apply([[maybe_unused]] real_t γₖ, [[maybe_unused]] crvec xₖ,
                [[maybe_unused]] crvec x̂ₖ, crvec pₖ,
                [[maybe_unused]] crvec grad_ψxₖ, rvec qₖ) const {
         qₖ = pₖ;
         return lbfgs.apply(qₖ, γₖ);
     }
 
+    /// @see @ref PANOCDirection::changed_γ
     void changed_γ(real_t γₖ, real_t old_γₖ) {
-        if (extraparams.rescale_when_γ_changes)
+        if (direction_params.rescale_on_step_size_changes)
             lbfgs.scale_y(γₖ / old_γₖ);
         else
             lbfgs.reset();
     }
 
+    /// @see @ref PANOCDirection::reset
     void reset() { lbfgs.reset(); }
 
-    std::string get_name() const { return lbfgs.get_name(); }
+    /// @see @ref PANOCDirection::get_name
+    std::string get_name() const {
+        return "LBFGSDirection<" + std::string(config_t::get_name()) + '>';
+    }
+    auto get_params() const {
+        return std::tie(lbfgs.get_params(), direction_params);
+    }
 
-    ExtraParams extraparams;
+    DirectionParams direction_params;
 };
 
 } // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/inner/internal/lipschitz.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/internal/lipschitz.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 template <Config Conf = DefaultConfig>
 struct LipschitzEstimateParams {
     USING_ALPAQA_CONFIG(Conf);
 
     /// Initial estimate of the Lipschitz constant of ∇ψ(x)
     real_t L_0 = 0;
     /// Relative step size for initial finite difference Lipschitz estimate.
-    real_t ε = 1e-6;
+    real_t ε = real_t(1e-6);
     /// Minimum step size for initial finite difference Lipschitz estimate.
-    real_t δ = 1e-12;
+    real_t δ = real_t(1e-12);
     /// Factor that relates step size γ and Lipschitz constant.
     /// Parameter α in Algorithm 2 of @cite de_marchi_proximal_2022.
     /// @f$ 0 < \alpha < 1 @f$
-    real_t Lγ_factor = 0.95;
+    real_t Lγ_factor = real_t(0.95);
 
     void verify() const {
         // TODO
     }
 };
 
 } // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/inner/internal/panoc-stop-crit.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/internal/panoc-stop-crit.hpp`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/inner/internal/solverstatus.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/internal/solverstatus.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -12,27 +12,29 @@
     Busy = 0,    ///< In progress.
     Converged,   ///< Converged and reached given tolerance.
     MaxTime,     ///< Maximum allowed execution time exceeded.
     MaxIter,     ///< Maximum number of iterations exceeded.
     NotFinite,   ///< Intermediate results were infinite or not-a-number.
     NoProgress,  ///< No progress was made in the last iteration.
     Interrupted, ///< Solver was interrupted by the user.
+    Exception,   ///< An unexpected exception was thrown.
 };
 
 /// @related    SolverStatus
 inline constexpr const char *enum_name(SolverStatus s) {
     using Status = SolverStatus;
     switch (s) {
         case Status::Busy: return "Busy";
         case Status::Converged: return "Converged";
         case Status::MaxTime: return "MaxTime";
         case Status::MaxIter: return "MaxIter";
         case Status::NotFinite: return "NotFinite";
         case Status::NoProgress: return "NoProgress";
         case Status::Interrupted: return "Interrupted";
+        case Status::Exception: return "Exception";
         default:;
     }
     throw std::out_of_range("invalid value for alpaqa::SolverStatus");
 }
 
 /// @related    SolverStatus
 ALPAQA_EXPORT std::ostream &operator<<(std::ostream &, SolverStatus);
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/inner/panoc.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/inner/panoc.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 #pragma once
 
 #include <alpaqa/export.hpp>
 #include <alpaqa/inner/directions/panoc-direction-update.hpp>
+#include <alpaqa/inner/inner-solve-options.hpp>
 #include <alpaqa/inner/internal/lipschitz.hpp>
 #include <alpaqa/inner/internal/panoc-helpers.hpp>
 #include <alpaqa/inner/internal/panoc-stop-crit.hpp>
 #include <alpaqa/inner/internal/solverstatus.hpp>
 #include <alpaqa/problem/type-erased-problem.hpp>
 #include <alpaqa/util/atomic-stop-signal.hpp>
 
 #include <chrono>
+#include <iostream>
 #include <limits>
+#include <stdexcept>
 #include <string>
+#include <type_traits>
 
 namespace alpaqa {
 
 /// Tuning parameters for the PANOC algorithm.
 template <Config Conf = DefaultConfig>
 struct PANOCParams {
     USING_ALPAQA_CONFIG(Conf);
 
     /// Parameters related to the Lipschitz constant estimate and step size.
     LipschitzEstimateParams<config_t> Lipschitz;
     /// Maximum number of inner PANOC iterations.
     unsigned max_iter = 100;
     /// Maximum duration.
-    std::chrono::microseconds max_time = std::chrono::minutes(5);
+    std::chrono::nanoseconds max_time = std::chrono::minutes(5);
     /// Minimum weight factor between Newton step and projected gradient step.
-    real_t τ_min = 1. / 256;
+    real_t min_linesearch_coefficient = real_t(1. / 256);
+    /// Ignore the line search condition and always accept the accelerated step.
+    /// (For testing purposes only).
+    bool force_linesearch = false;
+    /// Parameter β used in the line search (see Algorithm 2 in
+    /// @cite de_marchi_proximal_2022). @f$ 0 < \beta < 1 @f$
+    real_t linesearch_strictness_factor = real_t(0.95);
     /// Minimum Lipschitz constant estimate.
-    real_t L_min = 1e-5;
+    real_t L_min = real_t(1e-5);
     /// Maximum Lipschitz constant estimate.
-    real_t L_max = 1e20;
+    real_t L_max = real_t(1e20);
     /// What stopping criterion to use.
     PANOCStopCrit stop_crit = PANOCStopCrit::ApproxKKT;
     /// Maximum number of iterations without any progress before giving up.
     unsigned max_no_progress = 10;
 
     /// When to print progress. If set to zero, nothing will be printed.
     /// If set to N != 0, progress is printed every N iterations.
@@ -44,85 +54,110 @@
     int print_precision = std::numeric_limits<real_t>::max_digits10 / 2;
 
     real_t quadratic_upperbound_tolerance_factor =
         10 * std::numeric_limits<real_t>::epsilon();
     real_t linesearch_tolerance_factor =
         10 * std::numeric_limits<real_t>::epsilon();
 
-    bool update_lipschitz_in_linesearch = true;
-    bool alternative_linesearch_cond    = false;
+    bool update_direction_in_candidate              = false;
+    bool recompute_last_prox_step_after_lbfgs_flush = false;
 };
 
 template <Config Conf = DefaultConfig>
 struct PANOCStats {
     USING_ALPAQA_CONFIG(Conf);
 
     SolverStatus status = SolverStatus::Busy;
     real_t ε            = inf<config_t>;
-    std::chrono::nanoseconds elapsed_time;
-    unsigned iterations          = 0;
-    unsigned linesearch_failures = 0;
-    unsigned lbfgs_failures      = 0;
-    unsigned lbfgs_rejected      = 0;
-    unsigned τ_1_accepted        = 0;
-    unsigned count_τ             = 0;
-    real_t sum_τ                 = 0;
-    real_t final_γ               = 0;
+    std::chrono::nanoseconds elapsed_time{};
+    std::chrono::nanoseconds time_progress_callback{};
+    unsigned iterations            = 0;
+    unsigned linesearch_failures   = 0;
+    unsigned linesearch_backtracks = 0;
+    unsigned stepsize_backtracks   = 0;
+    unsigned lbfgs_failures        = 0;
+    unsigned lbfgs_rejected        = 0;
+    unsigned τ_1_accepted          = 0;
+    unsigned count_τ               = 0;
+    real_t sum_τ                   = 0;
+    real_t final_γ                 = 0;
+    real_t final_ψ                 = 0;
+    real_t final_h                 = 0;
+    real_t final_φγ                = 0;
 };
 
 template <Config Conf = DefaultConfig>
 struct PANOCProgressInfo {
     USING_ALPAQA_CONFIG(Conf);
 
     unsigned k;
+    SolverStatus status;
     crvec x;
     crvec p;
     real_t norm_sq_p;
     crvec x̂;
     real_t φγ;
     real_t ψ;
     crvec grad_ψ;
     real_t ψ_hat;
     crvec grad_ψ_hat;
+    crvec q;
     real_t L;
     real_t γ;
     real_t τ;
     real_t ε;
     crvec Σ;
     crvec y;
-    const TypeErasedProblem<config_t> &problem;
-    const PANOCParams<config_t> &params;
+    unsigned outer_iter;
+    const TypeErasedProblem<config_t> *problem;
+    const PANOCParams<config_t> *params;
 };
 
 /// PANOC solver for ALM.
 /// @ingroup    grp_InnerSolvers
-template <class DirectionProviderT>
+template <class DirectionT>
 class PANOCSolver {
   public:
-    USING_ALPAQA_CONFIG_TEMPLATE(DirectionProviderT::config_t);
+    USING_ALPAQA_CONFIG_TEMPLATE(DirectionT::config_t);
+
+    using Problem      = TypeErasedProblem<config_t>;
+    using Params       = PANOCParams<config_t>;
+    using Direction    = DirectionT;
+    using Stats        = PANOCStats<config_t>;
+    using ProgressInfo = PANOCProgressInfo<config_t>;
+    using SolveOptions = InnerSolveOptions<config_t>;
+
+    PANOCSolver(const Params &params)
+        requires std::default_initializable<Direction>
+        : params(params) {}
+    PANOCSolver(const Params &params, Direction &&direction)
+        : params(params), direction(std::move(direction)) {}
+    PANOCSolver(const Params &params, const Direction &direction)
+        : params(params), direction(direction) {}
+
+    Stats operator()(const Problem &problem,   // in
+                     const SolveOptions &opts, // in
+                     rvec x,                   // inout
+                     rvec y,                   // inout
+                     crvec Σ,                  // in
+                     rvec err_z);              // out
+
+    template <class P>
+    Stats operator()(const P &problem, const SolveOptions &opts, rvec x, rvec y,
+                     crvec Σ, rvec e) {
+        return operator()(Problem::template make<P>(problem), opts, x, y, Σ, e);
+    }
 
-    using Problem           = TypeErasedProblem<config_t>;
-    using Params            = PANOCParams<config_t>;
-    using DirectionProvider = DirectionProviderT;
-    using Direction         = PANOCDirection<DirectionProvider>;
-    using Stats             = PANOCStats<config_t>;
-    using ProgressInfo      = PANOCProgressInfo<config_t>;
-
-    PANOCSolver(const Params &params, Direction &&direction_provider)
-        : params(params), direction_provider(std::move(direction_provider)) {}
-    PANOCSolver(const Params &params, const Direction &direction_provider)
-        : params(params), direction_provider(direction_provider) {}
-
-    Stats operator()(const Problem &problem,        // in
-                     crvec Σ,                       // in
-                     real_t ε,                      // in
-                     bool always_overwrite_results, // in
-                     rvec x,                        // inout
-                     rvec y,                        // inout
-                     rvec err_z);                   // out
+    template <class P>
+    Stats operator()(const P &problem, const SolveOptions &opts, rvec x) {
+        if (problem.get_m() != 0)
+            throw std::invalid_argument("Missing arguments y, Σ, e");
+        mvec y{nullptr, 0}, Σ{nullptr, 0}, e{nullptr, 0};
+        return operator()(problem, opts, x, y, Σ, e);
+    }
 
     /// Specify a callable that is invoked with some intermediate results on
     /// each iteration of the algorithm.
     /// @see @ref ProgressInfo
     PANOCSolver &
     set_progress_callback(std::function<void(const ProgressInfo &)> cb) {
         this->progress_cb = cb;
@@ -138,58 +173,81 @@
   private:
     Params params;
     AtomicStopSignal stop_signal;
     std::function<void(const ProgressInfo &)> progress_cb;
     using Helpers = detail::PANOCHelpers<config_t>;
 
   public:
-    Direction direction_provider;
+    Direction direction;
+    std::ostream *os = &std::cout;
 };
 
 template <class InnerSolverStats>
 struct InnerStatsAccumulator;
 
 template <Config Conf>
 struct InnerStatsAccumulator<PANOCStats<Conf>> {
     USING_ALPAQA_CONFIG(Conf);
 
     /// Total elapsed time in the inner solver.
-    std::chrono::nanoseconds elapsed_time;
+    std::chrono::nanoseconds elapsed_time{};
+    /// Total time spent in the user-provided progress callback.
+    std::chrono::nanoseconds time_progress_callback{};
     /// Total number of inner PANOC iterations.
     unsigned iterations = 0;
     /// Total number of PANOC line search failures.
     unsigned linesearch_failures = 0;
+    /// Total number of PANOC line search backtracking steps.
+    unsigned linesearch_backtracks = 0;
+    /// Total number of PANOC step size reductions.
+    unsigned stepsize_backtracks = 0;
     /// Total number of times that the L-BFGS direction was not finite.
     unsigned lbfgs_failures = 0;
     /// Total number of times that the L-BFGS update was rejected (i.e. it
     /// could have resulted in a non-positive definite Hessian estimate).
     unsigned lbfgs_rejected = 0;
     /// Total number of times that a line search parameter of @f$ \tau = 1 @f$
     /// was accepted (i.e. no backtracking necessary).
     unsigned τ_1_accepted = 0;
     /// The total number of line searches performed (used for computing the
     /// average value of @f$ \tau @f$).
     unsigned count_τ = 0;
     /// The sum of the line search parameter @f$ \tau @f$ in all iterations
     /// (used for computing the average value of @f$ \tau @f$).
     real_t sum_τ = 0;
+    /// The final PANOC step size γ.
+    real_t final_γ = 0;
+    /// Final value of the smooth cost @f$ \psi(\hat x) @f$.
+    real_t final_ψ = 0;
+    /// Final value of the nonsmooth cost @f$ h(\hat x) @f$.
+    real_t final_h = 0;
+    /// Final value of the forward-backward envelope, @f$ \varphi_\gamma(x) @f$
+    /// (note that this is in the point @f$ x @f$, not @f$ \hat x @f$).
+    real_t final_φγ = 0;
 };
 
 template <Config Conf>
 InnerStatsAccumulator<PANOCStats<Conf>> &
 operator+=(InnerStatsAccumulator<PANOCStats<Conf>> &acc,
            const PANOCStats<Conf> &s) {
     acc.iterations += s.iterations;
     acc.elapsed_time += s.elapsed_time;
+    acc.time_progress_callback += s.time_progress_callback;
     acc.linesearch_failures += s.linesearch_failures;
+    acc.linesearch_backtracks += s.linesearch_backtracks;
+    acc.stepsize_backtracks += s.stepsize_backtracks;
     acc.lbfgs_failures += s.lbfgs_failures;
     acc.lbfgs_rejected += s.lbfgs_rejected;
     acc.τ_1_accepted += s.τ_1_accepted;
     acc.count_τ += s.count_τ;
     acc.sum_τ += s.sum_τ;
+    acc.final_γ  = s.final_γ;
+    acc.final_ψ  = s.final_ψ;
+    acc.final_h  = s.final_h;
+    acc.final_φγ = s.final_φγ;
     return acc;
 }
 
 ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, PANOCParams, DefaultConfig);
 ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, PANOCParams, EigenConfigf);
 ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, PANOCParams, EigenConfigd);
 ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, PANOCParams, EigenConfigl);
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/inner/src/panoc-helpers.tpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/inner/panoc-helpers.tpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #pragma once
 
 #include <alpaqa/config/config.hpp>
+#include <alpaqa/export.hpp>
+#include <alpaqa/inner/inner-solve-options.hpp>
 #include <alpaqa/inner/internal/panoc-stop-crit.hpp>
 #include <alpaqa/inner/internal/solverstatus.hpp>
 #include <alpaqa/problem/type-erased-problem.hpp>
 #include <alpaqa/util/atomic-stop-signal.hpp>
 #include <alpaqa/util/not-implemented.hpp>
 
 #include <stdexcept>
@@ -210,92 +212,46 @@
     /// Check all stop conditions (required tolerance reached, out of time,
     /// maximum number of iterations exceeded, interrupted by user,
     /// infinite iterate, no progress made)
     template <class ParamsT, class DurationT>
     static SolverStatus check_all_stop_conditions(
         /// [in]    Parameters including `max_iter`, `max_time` and `max_no_progress`
         const ParamsT &params,
+        /// [in]    Options for the current solve
+        const InnerSolveOptions<config_t> &opts,
         /// [in]    Time elapsed since the start of the algorithm
         DurationT time_elapsed,
         /// [in]    The current iteration number
         unsigned iteration,
         /// [in]    A stop signal for the user to interrupt the algorithm
         const AtomicStopSignal &stop_signal,
-        /// [in]    Desired primal tolerance
-        real_t ε,
         /// [in]    Tolerance of the current iterate
         real_t εₖ,
         /// [in]    The number of successive iterations no progress was made
         unsigned no_progress) {
 
-        bool out_of_time     = time_elapsed > params.max_time;
-        bool out_of_iter     = iteration == params.max_iter;
-        bool interrupted     = stop_signal.stop_requested();
-        bool not_finite      = not std::isfinite(εₖ);
-        bool conv            = εₖ <= ε;
+        auto max_time = params.max_time;
+        if (opts.max_time)
+            max_time = std::min(max_time, *opts.max_time);
+        auto tolerance   = opts.tolerance > 0 ? opts.tolerance : real_t(1e-8);
+        bool out_of_time = time_elapsed > max_time;
+        bool out_of_iter = iteration == params.max_iter;
+        bool interrupted = stop_signal.stop_requested();
+        bool not_finite  = not std::isfinite(εₖ);
+        bool converged   = εₖ <= tolerance;
         bool max_no_progress = no_progress > params.max_no_progress;
-        return conv              ? SolverStatus::Converged
+        return converged         ? SolverStatus::Converged
                : out_of_time     ? SolverStatus::MaxTime
                : out_of_iter     ? SolverStatus::MaxIter
                : not_finite      ? SolverStatus::NotFinite
                : max_no_progress ? SolverStatus::NoProgress
                : interrupted     ? SolverStatus::Interrupted
                                  : SolverStatus::Busy;
     }
 
-    /// Compute the Hessian matrix of the augmented Lagrangian function
-    /// @f[ \nabla^2_{xx} L_\Sigma(x, y) =
-    ///     \Big. \nabla_{xx}^2 L(x, y) \Big|_{\big(x,\, \hat y(x, y)\big)}
-    ///   + \sum_{i\in\mathcal{I}} \Sigma_i\,\nabla g_i(x) \nabla g_i(x)^\top @f]
-    static void calc_augmented_lagrangian_hessian(
-        /// [in]  Problem description
-        const Problem &problem,
-        /// [in]    Current iterate @f$ x^k @f$
-        crvec xₖ,
-        /// [in]   Intermediate vector @f$ \hat y(x^k) @f$
-        crvec ŷxₖ,
-        /// [in]    Lagrange multipliers @f$ y @f$
-        crvec y,
-        /// [in]    Penalty weights @f$ \Sigma @f$
-        crvec Σ,
-        /// [out]   The constraint values @f$ g(x^k) @f$
-        rvec g,
-        /// [out]   Hessian matrix @f$ H(x, y) @f$
-        mat &H,
-        ///         Dimension n
-        rvec work_n) {
-
-        // // Compute the Hessian of the Lagrangian
-        // problem.eval_hess_L(xₖ, ŷxₖ, H);
-        // // Compute the Hessian of the augmented Lagrangian
-        // problem.eval_g(xₖ, g);
-        // auto &&D = problem.get_D();
-        // for (index_t i = 0; i < problem.m; ++i) {
-        //     real_t ζ      = g(i) + y(i) / Σ(i);
-        //     bool inactive = D.lowerbound(i) < ζ && ζ < D.upperbound(i);
-        //     if (not inactive) {
-        //         problem.eval_grad_gi(xₖ, i, work_n);
-        //         H += work_n * Σ(i) * work_n.transpose();
-        //     }
-        // }
-
-        throw not_implemented_error(
-            "TODO: implement calc_augmented_lagrangian_hessian in "
-            "TypeErasedProblem");
-
-        (void)problem;
-        (void)xₖ;
-        (void)ŷxₖ;
-        (void)y;
-        (void)Σ;
-        (void)g;
-        (void)H;
-        (void)work_n;
-    }
-
     /// Compute the Hessian matrix of the augmented Lagrangian function multiplied
     /// by the given vector, using finite differences.
     /// @f[ \nabla^2_{xx} L_\Sigma(x, y)\, v \approx
     ///     \frac{\nabla_x L_\Sigma(x+hv, y) - \nabla_x L_\Sigma(x, y)}{h} @f]
     static void calc_augmented_lagrangian_hessian_prod_fd(
         /// [in]    Problem description
         const Problem &problem,
@@ -329,52 +285,55 @@
 
     /// Estimate the Lipschitz constant of the gradient @f$ \nabla \psi @f$ using
     /// finite differences.
     static real_t initial_lipschitz_estimate(
         /// [in]    Problem description
         const Problem &problem,
         /// [in]    Current iterate @f$ x^k @f$
-        crvec xₖ,
+        crvec x,
         /// [in]    Lagrange multipliers @f$ y @f$
         crvec y,
         /// [in]    Penalty weights @f$ \Sigma @f$
         crvec Σ,
-        /// [in]    Finite difference step size relative to xₖ
+        /// [in]    Finite difference step size relative to x
         real_t ε,
         /// [in]    Minimum absolute finite difference step size
         real_t δ,
         /// [in]    Minimum allowed Lipschitz estimate.
         real_t L_min,
         /// [in]    Maximum allowed Lipschitz estimate.
         real_t L_max,
         /// [out]   @f$ \psi(x^k) @f$
         real_t &ψ,
         /// [out]   Gradient @f$ \nabla \psi(x^k) @f$
         rvec grad_ψ,
         ///         Dimension n
-        rvec work_n1,
+        rvec work_x,
         ///         Dimension n
-        rvec work_n2,
+        rvec work_grad_ψ,
         ///         Dimension n
-        rvec work_n3,
+        rvec work_n,
         ///         Dimension m
         rvec work_m) {
 
-        auto h        = (xₖ * ε).cwiseAbs().cwiseMax(δ);
-        work_n1       = xₖ + h;
-        real_t norm_h = h.norm();
-        // Calculate ∇ψ(x₀ + h)
-        problem.eval_grad_ψ(work_n1, y, Σ, /* in ⟹ out */ work_n2, work_n3,
-                            work_m);
         // Calculate ψ(x₀), ∇ψ(x₀)
-        ψ = problem.eval_ψ_grad_ψ(xₖ, y, Σ, /* in ⟹ out */ grad_ψ, work_n1,
+        ψ = problem.eval_ψ_grad_ψ(x, y, Σ, /* in ⟹ out */ grad_ψ, work_n,
                                   work_m);
+        // Select a small step h for finite differences
+        auto h        = grad_ψ.unaryExpr([&](real_t g) {
+            return g > 0 ? std::max(g * ε, δ) : std::min(g * ε, -δ);
+        });
+        work_x        = x - h;
+        real_t norm_h = h.norm();
+        // Calculate ∇ψ(x₀ - h)
+        problem.eval_grad_ψ(work_x, y, Σ, /* in ⟹ out */ work_grad_ψ, work_n,
+                            work_m);
 
         // Estimate Lipschitz constant using finite differences
-        real_t L = (work_n2 - grad_ψ).norm() / norm_h;
+        real_t L = (work_grad_ψ - grad_ψ).norm() / norm_h;
         return std::clamp(L, L_min, L_max);
     }
 
     /// Estimate the Lipschitz constant of the gradient @f$ \nabla \psi @f$ using
     /// finite differences.
     static real_t initial_lipschitz_estimate(
         /// [in]    Problem description
@@ -415,8 +374,16 @@
 
         // Estimate Lipschitz constant using finite differences
         real_t L = (work_n2 - grad_ψ).norm() / norm_h;
         return std::clamp(L, L_min, L_max);
     }
 };
 
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, PANOCHelpers, DefaultConfig);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, PANOCHelpers, EigenConfigf);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, PANOCHelpers, EigenConfigd);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, PANOCHelpers, EigenConfigl);
+#ifdef ALPAQA_WITH_QUAD_PRECISION
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, PANOCHelpers, EigenConfigq);
+#endif
+
 } // namespace alpaqa::detail
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/inner/src/panoc-ocp.tpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/inner/panoc-ocp.tpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,184 +1,187 @@
 #include <alpaqa/accelerators/lbfgs.hpp>
-#include <alpaqa/inner/directions/panoc-ocp/dynamics-eval.hpp>
+#include <alpaqa/config/config.hpp>
+#include <alpaqa/implementation/util/print.tpp>
 #include <alpaqa/inner/directions/panoc-ocp/lqr.hpp>
+#include <alpaqa/inner/directions/panoc-ocp/ocp-vars.hpp>
 #include <alpaqa/inner/panoc-ocp.hpp>
+#include <alpaqa/problem/box.hpp>
+#include <alpaqa/problem/ocproblem.hpp>
 #include <alpaqa/util/index-set.hpp>
-#include <alpaqa/util/src/print.tpp>
+#include <alpaqa/util/timed.hpp>
+#include <concepts>
 #include <iomanip>
 #include <iostream>
+#include <numeric>
 #include <stdexcept>
+#include <type_traits>
 
 namespace alpaqa {
 
-namespace detail {
-
-template <Config Conf>
-void assign_interleave_xu(OCPDim<Conf> dim, crvec<Conf> u, rvec<Conf> xu) {
-    for (index_t<Conf> t = 0; t < dim.N; ++t)
-        xu.segment(t * (dim.nx + dim.nu) + dim.nx, dim.nu) =
-            u.segment(t * dim.nu, dim.nu);
-}
-template <Config Conf>
-void assign_interleave_xu(OCPDim<Conf> dim, crvec<Conf> x, crvec<Conf> u,
-                          rvec<Conf> xu) {
-    for (index_t<Conf> t = 0; t < dim.N; ++t) {
-        xu.segment(t * (dim.nx + dim.nu), dim.nx) =
-            x.segment(t * dim.nx, dim.nx);
-        xu.segment(t * (dim.nx + dim.nu) + dim.nx, dim.nu) =
-            u.segment(t * dim.nu, dim.nu);
-    }
-    xu.segment(dim.N * (dim.nx + dim.nu), dim.nx) =
-        x.segment(dim.N * dim.nx, dim.nx);
-}
-template <Config Conf>
-void assign_extract_u(OCPDim<Conf> dim, crvec<Conf> xu, rvec<Conf> u) {
-    for (index_t<Conf> t = 0; t < dim.N; ++t)
-        u.segment(t * dim.nu, dim.nu) =
-            xu.segment(t * (dim.nx + dim.nu) + dim.nx, dim.nu);
-}
-template <Config Conf>
-void assign_extract_x(OCPDim<Conf> dim, crvec<Conf> xu, rvec<Conf> x) {
-    for (index_t<Conf> t = 0; t < dim.N + 1; ++t)
-        x.segment(t * dim.nx, dim.nx) =
-            xu.segment(t * (dim.nx + dim.nu), dim.nx);
-}
-
-template <Config Conf>
-vec<Conf> extract_u(const TypeErasedControlProblem<Conf> &problem,
-                    crvec<Conf> xu) {
-    auto dim = problem.get_dimensions();
-    vec<Conf> u(dim.N * dim.nu);
-    assign_extract_u(dim, xu, u);
-    return u;
-}
-template <Config Conf>
-vec<Conf> extract_x(const TypeErasedControlProblem<Conf> &problem,
-                    crvec<Conf> xu) {
-    auto dim = problem.get_dimensions();
-    vec<Conf> x((dim.N + 1) * (dim.nx + dim.nu));
-    assign_extract_x(dim, xu, x);
-    return x;
-}
-
-} // namespace detail
-
 template <Config Conf>
 auto PANOCOCPProgressInfo<Conf>::u() const -> vec {
-    return detail::extract_u(problem, xu);
+    return detail::extract_u(*problem, xu);
 }
 
 template <Config Conf>
 auto PANOCOCPProgressInfo<Conf>::x() const -> vec {
-    return detail::extract_x(problem, xu);
+    return detail::extract_x(*problem, xu);
 }
 
 template <Config Conf>
 auto PANOCOCPProgressInfo<Conf>::û() const -> vec {
-    return detail::extract_u(problem, x̂u);
+    return detail::extract_u(*problem, x̂u);
 }
 
 template <Config Conf>
 auto PANOCOCPProgressInfo<Conf>::x̂() const -> vec {
-    return detail::extract_x(problem, x̂u);
-}
-
-template <Config Conf>
-auto PANOCOCPProgressInfo<Conf>::qu() const -> vec {
-    return detail::extract_u(problem, q);
-}
-
-template <Config Conf>
-auto PANOCOCPProgressInfo<Conf>::qx() const -> vec {
-    return detail::extract_x(problem, q);
+    return detail::extract_x(*problem, x̂u);
 }
 
 template <Config Conf>
 std::string PANOCOCPSolver<Conf>::get_name() const {
     return "PANOCOCPSolver<" + std::string(config_t::get_name()) + '>';
 }
 
 template <Config Conf>
 auto PANOCOCPSolver<Conf>::operator()(
     /// [in]    Problem description
     const Problem &problem,
-    /// [in]    Tolerance @f$ \varepsilon @f$
-    const real_t ε,
+    /// [in]    Solve options
+    const SolveOptions &opts,
     /// [inout] Decision variable @f$ u @f$
-    rvec u) -> Stats {
+    rvec u,
+    /// [inout] Lagrange multipliers @f$ y @f$
+    rvec y,
+    /// [in]    Penalty factors @f$ \mu @f$
+    crvec μ,
+    /// [out]   Slack variable error @f$ c(x) - \Pi_D(c(x) + \mu^{-1} y) @f$
+    rvec err_z) -> Stats {
+
+    if (opts.check)
+        problem.check();
 
     using std::chrono::nanoseconds;
+    auto os         = opts.os ? opts.os : this->os;
     auto start_time = std::chrono::steady_clock::now();
     Stats s;
 
-    const auto N   = problem.get_N();
-    const auto nu  = problem.get_nu();
-    const auto nx  = problem.get_nx();
-    const auto n   = nu * N;
-    const auto Nxu = n + nx * (N + 1);
+    const auto N    = problem.get_N();
+    const auto nu   = problem.get_nu();
+    const auto nx   = problem.get_nx();
+    const auto nc   = problem.get_nc();
+    const auto nc_N = problem.get_nc_N();
+    const auto n    = nu * N;
 
     bool enable_lbfgs = params.gn_interval != 1;
 
     // Allocate storage --------------------------------------------------------
 
     // TODO: the L-BFGS objects and vectors allocate on each iteration of ALM,
     //       and there are more vectors than strictly necessary.
 
-    vec quₖ(enable_lbfgs ? n : 0), // For L-BFGS update
-        qxuₖ(Nxu),                 // Newton step, including states
-        work_p(nx),                //
-        work_w(nx + nu);           //
-    Box<config_t> U{vec::Constant(nu, NaN<config_t>),
-                    vec::Constant(n, NaN<config_t>)};
-
-    DynamicsEvaluator<config_t> eval{problem};
-    detail::IndexSet<config_t> J{N, nu};
+    OCPEvaluator<config_t> eval{problem};
+    auto &vars = eval.vars;
+    alpaqa::detail::IndexSet<config_t> J{N, nu};
     using LQRFactor = alpaqa::StatefulLQRFactor<config_t>;
     LQRFactor lqr{{.N = N, .nx = nx, .nu = nu}};
-    LBFGSParams<config_t> lbfgs_param{.memory = N}; // TODO: make configurable
-    LBFGS<config_t> lbfgs{lbfgs_param, enable_lbfgs ? n : 0};
+    LBFGS<config_t> lbfgs{params.lbfgs_params, enable_lbfgs ? n : 0};
+    mat jacs = vars.create_AB();
+    vec qr   = vars.create_qr();
+
+    vec q(n); // Newton step, including states
+    Box<config_t> U   = Box<config_t>::NaN(nu);
+    Box<config_t> D   = Box<config_t>::NaN(nc);
+    Box<config_t> D_N = Box<config_t>::NaN(nc_N);
+
+    // Workspace storage
+    vec work_2x(nx * 2);
+
+    // ALM
+    assert(μ.size() == nc * N + nc_N);
+    assert(y.size() == nc * N + nc_N);
 
     // Functions for accessing the LQR matrices and index sets
-    auto Ak    = [&](index_t i) -> crmat { return eval.Ak(i); };
-    auto Bk    = [&](index_t i) -> crmat { return eval.Bk(i); };
-    auto Qk    = [&](index_t k) -> crmat { return eval.Qk(k); };
-    auto Rk    = [&](index_t k) -> crmat { return eval.Rk(k); };
-    auto qk    = [&](index_t k) -> crvec { return eval.qk(k); };
-    auto rk    = [&](index_t k) -> crvec { return eval.rk(k); };
-    auto uk_eq = [&](index_t k) -> crvec { return eval.uk(qxuₖ, k); };
-    auto Jk    = [&](index_t k) -> crindexvec { return J.indices(k); };
-    auto Kk    = [&](index_t k) -> crindexvec { return J.compl_indices(k); };
+    auto ABk = [&](index_t i) -> crmat { return vars.ABk(jacs, i); };
+    auto Qk  = [&](rvec storage) {
+        return [&, storage](index_t k) {
+            return [&, k](rmat out) {
+                alpaqa::util::Timed t{s.time_hessians};
+                return eval.Qk(storage, y, μ, D, D_N, k, out);
+            };
+        };
+    };
+    auto Rk = [&](rvec storage) {
+        return [&, storage](index_t k) {
+            return [&, k](crindexvec mask, rmat out) {
+                alpaqa::util::Timed t{s.time_hessians};
+                return eval.Rk(storage, k, mask, out);
+            };
+        };
+    };
+    auto Sk = [&](rvec storage) {
+        return [&, storage](index_t k) {
+            return [&, k](crindexvec mask, rmat out) {
+                alpaqa::util::Timed t{s.time_hessians};
+                return eval.Sk(storage, k, mask, out);
+            };
+        };
+    };
+    auto Rk_prod = [&](rvec storage) {
+        return [&, storage](index_t k) {
+            return [&, k](crindexvec mask_J, crindexvec mask_K, crvec v,
+                          rvec out) {
+                alpaqa::util::Timed t{s.time_hessians};
+                return eval.Rk_prod(storage, k, mask_J, mask_K, v, out);
+            };
+        };
+    };
+    auto Sk_prod = [&](rvec storage) {
+        return [&, storage](index_t k) {
+            return [&, k](crindexvec mask_K, crvec v, rvec out) {
+                alpaqa::util::Timed t{s.time_hessians};
+                return eval.Sk_prod(storage, k, mask_K, v, out);
+            };
+        };
+    };
+    auto mut_qrk = [&](index_t k) -> rvec { return vars.qrk(qr, k); };
+    auto mut_q_N = [&]() -> rvec { return vars.qk(qr, N); };
+    auto qk      = [&](index_t k) -> crvec { return vars.qk(qr, k); };
+    auto rk      = [&](index_t k) -> crvec { return vars.rk(qr, k); };
+    auto uk_eq   = [&](index_t k) -> crvec { return q.segment(k * nu, nu); };
+    auto Jk      = [&](index_t k) -> crindexvec { return J.indices(k); };
+    auto Kk      = [&](index_t k) -> crindexvec { return J.compl_indices(k); };
 
     // Iterates ----------------------------------------------------------------
 
+    // Represents an iterate in the algorithm, keeping track of some
+    // intermediate values and function evaluations.
     struct Iterate {
-        vec xu;     ///< Inputs u interleaved with states x
-        vec xû;     ///< Inputs u interleaved with states x after prox grad
-        vec grad_ψ; ///< Gradient of cost in u
-        vec p;      ///< Proximal gradient step in u
-        vec u;      ///< Inputs u (used for L-BFGS only)
-        real_t ψu           = NaN<config_t>; ///< Cost in u
-        real_t ψû           = NaN<config_t>; ///< Cost in û
-        real_t γ            = NaN<config_t>; ///< Step size γ
-        real_t L            = NaN<config_t>; ///< Lipschitz estimate L
-        real_t pᵀp          = NaN<config_t>; ///< Norm squared of p
-        real_t grad_ψᵀp     = NaN<config_t>; ///< Dot product of gradient and p
-        bool have_jacobians = false;
+        vec xu;     //< Inputs u interleaved with states x
+        vec xû;     //< Inputs u interleaved with states x after prox grad
+        vec grad_ψ; //< Gradient of cost in u
+        vec p;      //< Proximal gradient step in u
+        vec u;      //< Inputs u (used for L-BFGS only)
+        real_t ψu       = NaN<config_t>; //< Cost in u
+        real_t ψû       = NaN<config_t>; //< Cost in û
+        real_t γ        = NaN<config_t>; //< Step size γ
+        real_t L        = NaN<config_t>; //< Lipschitz estimate L
+        real_t pᵀp      = NaN<config_t>; //< Norm squared of p
+        real_t grad_ψᵀp = NaN<config_t>; //< Dot product of gradient and p
 
-        /// @pre    @ref ψu, @ref pᵀp, @pre grad_ψᵀp
-        /// @return φγ
+        // @pre    @ref ψu, @ref pᵀp, @pre grad_ψᵀp
+        // @return φγ
         real_t fbe() const { return ψu + pᵀp / (2 * γ) + grad_ψᵀp; }
 
-        Iterate(OCPDim<config_t> dim, bool enable_lbfgs)
-            : xu{dim.N * (dim.nx + dim.nu) + dim.nx},
-              xû{dim.N * (dim.nx + dim.nu) + dim.nx}, grad_ψ{dim.N * dim.nu},
-              p{dim.N * dim.nu}, u{enable_lbfgs ? dim.N * dim.nu : 0} {}
+        Iterate(const OCPVariables<config_t> &vars, bool enable_lbfgs)
+            : xu{vars.create()}, xû{vars.create()}, grad_ψ{vars.N * vars.nu()},
+              p{vars.N * vars.nu()}, u{enable_lbfgs ? vars.N * vars.nu() : 0} {}
     } iterates[2]{
-        {problem.get_dimensions(), enable_lbfgs},
-        {problem.get_dimensions(), enable_lbfgs},
+        {vars, enable_lbfgs},
+        {vars, enable_lbfgs},
     };
     Iterate *curr = &iterates[0];
     Iterate *next = &iterates[1];
 
     // Helper functions --------------------------------------------------------
 
     auto eval_proj_grad_step_box = [&U](real_t γ, crvec x, crvec grad_ψ, rvec x̂,
@@ -186,24 +189,24 @@
         using binary_real_f = real_t (*)(real_t, real_t);
         p                   = (-γ * grad_ψ)
                 .binaryExpr(U.lowerbound - x, binary_real_f(std::fmax))
                 .binaryExpr(U.upperbound - x, binary_real_f(std::fmin));
         x̂ = x + p;
     };
 
-    auto eval_prox_impl = [&eval_proj_grad_step_box, &eval, N,
-                           nu](real_t γ, crvec xu, crvec grad_ψ, rvec x̂u,
-                               rvec p) {
+    auto eval_prox_impl = [&](real_t γ, crvec xu, crvec grad_ψ, rvec x̂u,
+                              rvec p) {
+        alpaqa::util::Timed t{s.time_prox};
         real_t pᵀp      = 0;
         real_t grad_ψᵀp = 0;
         for (index_t t = 0; t < N; ++t) {
             auto &&grad_ψ_t = grad_ψ.segment(t * nu, nu);
             auto &&p_t      = p.segment(t * nu, nu);
-            eval_proj_grad_step_box(γ, eval.uk(xu, t), grad_ψ_t,
-                                    /* in ⟹ out */ eval.uk(x̂u, t), p_t);
+            eval_proj_grad_step_box(γ, vars.uk(xu, t), grad_ψ_t,
+                                    /* in ⟹ out */ vars.uk(x̂u, t), p_t);
             // Calculate ∇ψ(x)ᵀp and ‖p‖²
             pᵀp += p_t.squaredNorm();
             grad_ψᵀp += grad_ψ_t.dot(p_t);
         }
         return std::make_tuple(pᵀp, grad_ψᵀp);
     };
 
@@ -239,182 +242,269 @@
             case PANOCStopCrit::LBFGSBpp: [[fallthrough]];
             default:
                 throw std::invalid_argument("Unsupported stopping criterion");
         }
     };
 
     auto check_all_stop_conditions =
-        [this, ε](
+        [this, &opts](
             /// [in]    Time elapsed since the start of the algorithm
             auto time_elapsed,
             /// [in]    The current iteration number
             unsigned iteration,
             /// [in]    Tolerance of the current iterate
             real_t εₖ,
             /// [in]    The number of successive iterations no progress was made
             unsigned no_progress) {
-            bool out_of_time     = time_elapsed > params.max_time;
+            auto max_time = params.max_time;
+            if (opts.max_time)
+                max_time = std::min(max_time, *opts.max_time);
+            auto tolerance = opts.tolerance > 0 ? opts.tolerance : real_t(1e-8);
+            bool out_of_time     = time_elapsed > max_time;
             bool out_of_iter     = iteration == params.max_iter;
             bool interrupted     = stop_signal.stop_requested();
             bool not_finite      = not std::isfinite(εₖ);
-            bool conv            = εₖ <= ε;
+            bool conv            = εₖ <= tolerance;
             bool max_no_progress = no_progress > params.max_no_progress;
             return conv              ? SolverStatus::Converged
                    : out_of_time     ? SolverStatus::MaxTime
                    : out_of_iter     ? SolverStatus::MaxIter
                    : not_finite      ? SolverStatus::NotFinite
                    : max_no_progress ? SolverStatus::NoProgress
                    : interrupted     ? SolverStatus::Interrupted
                                      : SolverStatus::Busy;
         };
 
-    auto assign_interleave_xu = [dim{problem.get_dimensions()}](crvec u,
-                                                                rvec xu) {
-        detail::assign_interleave_xu(dim, u, xu);
-    };
-    auto assign_extract_u = [dim{problem.get_dimensions()}](crvec xu, rvec u) {
-        detail::assign_extract_u(dim, xu, u);
+    auto assign_interleave_xu = [&vars](crvec u, rvec xu) {
+        detail::assign_interleave_xu(vars, u, xu);
+    };
+    auto assign_extract_u = [&vars](crvec xu, rvec u) {
+        detail::assign_extract_u(vars, xu, u);
     };
 
-    /// @pre    @ref Iterate::γ, @ref Iterate::xu, @ref Iterate::grad_ψ
-    /// @post   @ref Iterate::xû, @ref Iterate::p, @ref Iterate::pᵀp,
-    ///         @ref Iterate::grad_ψᵀp
-    auto eval_prox = [&eval_prox_impl](Iterate &i) {
+    auto write_solution = [&](Iterate &it) {
+        // Update multipliers and constraint error
+        if (nc > 0 || nc_N > 0) {
+            for (index_t t = 0; t < N; ++t) {
+                auto ct = vars.ck(it.xû, t);
+                auto yt = y.segment(nc * t, nc);
+                auto μt = μ.segment(nc * t, nc);
+                auto ζ  = ct + μt.asDiagonal().inverse() * yt;
+                auto et = err_z.segment(nc * t, nc);
+                et      = projecting_difference(ζ, D);
+                et -= μt.asDiagonal().inverse() * yt;
+                yt += μt.asDiagonal() * et;
+            }
+            auto ct = vars.ck(it.xû, N);
+            auto yt = y.segment(nc * N, nc_N);
+            auto μt = μ.segment(nc * N, nc_N);
+            auto ζ  = ct + μt.asDiagonal().inverse() * yt;
+            auto et = err_z.segment(nc * N, nc_N);
+            et      = projecting_difference(ζ, D_N);
+            et -= μt.asDiagonal().inverse() * yt;
+            yt += μt.asDiagonal() * et;
+        }
+        assign_extract_u(it.xû, u);
+    };
+
+    // @pre    @ref Iterate::γ, @ref Iterate::xu, @ref Iterate::grad_ψ
+    // @post   @ref Iterate::xû, @ref Iterate::p, @ref Iterate::pᵀp,
+    //         @ref Iterate::grad_ψᵀp
+    auto eval_prox = [&](Iterate &i) {
         std::tie(i.pᵀp, i.grad_ψᵀp) =
             eval_prox_impl(i.γ, i.xu, i.grad_ψ, i.xû, i.p);
     };
 
-    /// @pre    @ref Iterate::xu
-    /// @post   @ref Iterate::ψu
-    auto eval_forward = [&eval](Iterate &i) { i.ψu = eval.forward(i.xu); };
-    /// @pre    @ref Iterate::xû
-    /// @post   @ref Iterate::ψû
-    auto eval_forward_hat = [&eval](Iterate &i) { i.ψû = eval.forward(i.xû); };
-
-    /// @pre    @ref Iterate::xu
-    /// @post   @ref Iterate::grad_ψ, @ref Iterate::have_jacobians
-    auto eval_backward = [&eval, &work_p, &work_w](Iterate &i, bool with_jac) {
-        with_jac ? eval.backward_with_jac(i.xu, i.grad_ψ, work_p)
-                 : eval.backward(i.xu, i.grad_ψ, work_p, work_w);
-        i.have_jacobians = with_jac;
+    // @pre    @ref Iterate::xu
+    // @post   @ref Iterate::ψu
+    auto eval_forward = [&](Iterate &i) {
+        alpaqa::util::Timed t{s.time_forward};
+        i.ψu = eval.forward(i.xu, D, D_N, μ, y);
+    };
+    // @pre    @ref Iterate::xû
+    // @post   @ref Iterate::ψû
+    auto eval_forward_hat = [&](Iterate &i) {
+        alpaqa::util::Timed t{s.time_forward};
+        i.ψû = eval.forward(i.xû, D, D_N, μ, y);
+    };
+
+    // @pre    @ref Iterate::xu
+    // @post   @ref Iterate::grad_ψ, q, q_N
+    auto eval_backward = [&](Iterate &i) {
+        alpaqa::util::Timed t{s.time_backward};
+        eval.backward(i.xu, i.grad_ψ, mut_qrk, mut_q_N, D, D_N, μ, y);
     };
 
     auto qub_violated = [this](const Iterate &i) {
         real_t margin =
             (1 + std::abs(i.ψu)) * params.quadratic_upperbound_tolerance_factor;
         return i.ψû > i.ψu + i.grad_ψᵀp + real_t(0.5) * i.L * i.pᵀp + margin;
     };
 
     auto linesearch_violated = [this](const Iterate &curr,
                                       const Iterate &next) {
-        real_t σ  = params.β * (1 - curr.γ * curr.L) / (2 * curr.γ);
+        real_t β  = params.linesearch_strictness_factor;
+        real_t σ  = β * (1 - curr.γ * curr.L) / (2 * curr.γ);
         real_t φγ = curr.fbe();
         real_t margin = (1 + std::abs(φγ)) * params.linesearch_tolerance_factor;
         return next.fbe() > φγ - σ * curr.pᵀp + margin;
     };
 
     auto initial_lipschitz_estimate =
-        [&eval, &eval_forward, &eval_backward, &work_p, &work_w, N, nu](
+        [&](
             /// Iterate, updates xu, ψ, grad_ψ, have_jacobians, L
             Iterate *it,
-            /// Whether to compute the Jacobians of the dynamics in xu
-            bool do_gn_step,
             /// [in]    Finite difference step size relative to x
             real_t ε,
             /// [in]    Minimum absolute finite difference step size
             real_t δ,
             /// [in]    Minimum allowed Lipschitz estimate.
             real_t L_min,
             /// [in]    Maximum allowed Lipschitz estimate.
             real_t L_max,
             ///         Workspace with the same dimensions as xu, with x_init
             rvec work_xu,
             ///         Workspace with the same dimensions as grad_ψ
             rvec work_grad_ψ) {
             // Calculate ψ(x₀), ∇ψ(x₀)
             eval_forward(*it);
-            eval_backward(*it, do_gn_step);
+            eval_backward(*it);
             // Select a small step h for finite differences
-            // TODO: remove abs
-            auto h        = (it->grad_ψ * -ε).cwiseAbs().cwiseMax(δ);
+            auto h        = it->grad_ψ.unaryExpr([&](real_t g) {
+                return g > 0 ? std::max(g * ε, δ) : std::min(g * ε, -δ);
+            });
             real_t norm_h = h.norm();
-            // work_xu = xu + h
+            // work_xu = xu - h
             for (index_t t = 0; t < N; ++t)
-                eval.uk(work_xu, t) =
-                    eval.uk(it->xu, t) + h.segment(t * nu, nu);
-            // Calculate ψ(x₀ + h)
-            eval.forward_simulate(work_xu); // needed for backwards sweep
-            // Calculate ∇ψ(x₀ + h)
-            eval.backward(work_xu, work_grad_ψ, work_p, work_w);
+                vars.uk(work_xu, t) =
+                    vars.uk(it->xu, t) - h.segment(t * nu, nu);
 
+            { // Calculate ψ(x₀ - h)
+                alpaqa::util::Timed t{s.time_forward};
+                eval.forward_simulate(work_xu); // needed for backwards sweep
+            }
+            { // Calculate ∇ψ(x₀ + h)
+                alpaqa::util::Timed t{s.time_backward};
+                eval.backward(work_xu, work_grad_ψ, mut_qrk, mut_q_N, D, D_N, μ,
+                              y);
+            }
             // Estimate Lipschitz constant using finite differences
             it->L = (work_grad_ψ - it->grad_ψ).norm() / norm_h;
             it->L = std::clamp(it->L, L_min, L_max);
         };
 
     // Printing ----------------------------------------------------------------
 
     std::array<char, 64> print_buf;
     auto print_real = [&](real_t x) {
         return float_to_str_vw(print_buf, x, params.print_precision);
     };
     auto print_real3 = [&](real_t x) {
         return float_to_str_vw(print_buf, x, 3);
     };
-    auto print_progress = [&](unsigned k, real_t φₖ, real_t ψₖ, crvec grad_ψₖ,
-                              real_t pₖᵀpₖ, crvec qₖ, real_t γₖ, real_t τₖ,
-                              real_t εₖ, bool did_gn, length_t nJ,
-                              real_t min_rcond) {
-        std::cout << "[PANOC] " << std::setw(6) << k
-                  << ": φγ = " << print_real(φₖ) << ", ψ = " << print_real(ψₖ)
-                  << ", ‖∇ψ‖ = " << print_real(grad_ψₖ.norm())
-                  << ", ‖p‖ = " << print_real(std::sqrt(pₖᵀpₖ))
-                  << ", γ = " << print_real(γₖ) << ", εₖ = " << print_real(εₖ);
-        if (k > 0)
-            std::cout << ", τ = " << print_real3(τₖ)
-                      << ", ‖q‖ = " << print_real(qₖ.norm())
-                      << ", #J =" << std::setw(5) << nJ
-                      << ", rcond = " << print_real3(min_rcond) << ", "
-                      << (did_gn ? "GN" : "L-BFGS");
-        std::cout << std::endl; // Flush for Python buffering
+    auto print_progress_1 = [&](unsigned k, real_t φₖ, real_t ψₖ, crvec grad_ψₖ,
+                                real_t pₖᵀpₖ, real_t γₖ, real_t εₖ) {
+        if (k == 0)
+            *os << "┌─[PANOCOCP]\n";
+        else
+            *os << "├─ " << std::setw(6) << k << '\n';
+        *os << "│   φγ = " << print_real(φₖ)               //
+            << ",    ψ = " << print_real(ψₖ)               //
+            << ", ‖∇ψ‖ = " << print_real(grad_ψₖ.norm())   //
+            << ",  ‖p‖ = " << print_real(std::sqrt(pₖᵀpₖ)) //
+            << ",    γ = " << print_real(γₖ)               //
+            << ",    ε = " << print_real(εₖ) << '\n';
+    };
+    auto print_progress_2 = [&](crvec qₖ, real_t τₖ, bool did_gn, length_t nJ,
+                                real_t min_rcond, bool reject) {
+        const char *color = τₖ == 1  ? "\033[0;32m"
+                            : τₖ > 0 ? "\033[0;33m"
+                                     : "\033[0;35m";
+        *os << "│  ‖q‖ = " << print_real(qₖ.norm())                       //
+            << ",   #J = " << std::setw(7 + params.print_precision) << nJ //
+            << ", cond = " << print_real3(real_t(1) / min_rcond)          //
+            << ",    τ = " << color << print_real3(τₖ) << "\033[0m"       //
+            << ",    " << (did_gn ? "GN" : "L-BFGS")                      //
+            << ",      dir update "
+            << (reject ? "\033[0;31mrejected\033[0m"
+                       : "\033[0;32maccepted\033[0m") //
+            << std::endl; // Flush for Python buffering
+    };
+    auto print_progress_n = [&](SolverStatus status) {
+        *os << "└─ " << status << " ──"
+            << std::endl; // Flush for Python buffering
+    };
+
+    auto do_progress_cb = [this, &s, &problem, &lqr,
+                           &opts](unsigned k, Iterate &curr, crvec q, real_t τ,
+                                  real_t εₖ, bool did_gn, index_t nJ,
+                                  SolverStatus status) {
+        if (!progress_cb)
+            return;
+        ScopedMallocAllower ma;
+        alpaqa::util::Timed t{s.time_progress_callback};
+        progress_cb({
+            .k             = k,
+            .status        = status,
+            .xu            = curr.xu,
+            .p             = curr.p,
+            .norm_sq_p     = curr.pᵀp,
+            .x̂u            = curr.xû,
+            .φγ            = curr.fbe(),
+            .ψ             = curr.ψu,
+            .grad_ψ        = curr.grad_ψ,
+            .ψ_hat         = curr.ψû,
+            .q             = q,
+            .gn            = did_gn,
+            .nJ            = nJ,
+            .lqr_min_rcond = lqr.min_rcond,
+            .L             = curr.L,
+            .γ             = curr.γ,
+            .τ             = status == SolverStatus::Busy ? τ : NaN<config_t>,
+            .ε             = εₖ,
+            .outer_iter    = opts.outer_iter,
+            .problem       = &problem,
+            .params        = &params,
+        });
     };
 
     // Initialize inputs and initial state (do not simulate states yet) --------
 
     assign_interleave_xu(u, curr->xu);           // initial guess
     problem.get_x_init(curr->xu.topRows(nx));    // initial state
     curr->xû.topRows(nx) = curr->xu.topRows(nx); // initial state
     next->xu.topRows(nx) = curr->xu.topRows(nx); // initial state
     next->xû.topRows(nx) = curr->xu.topRows(nx); // initial state
-    qxuₖ.setZero();                              // set the states to zero
     if (enable_lbfgs)
         curr->u = u;
 
-    problem.get_U(U); // input box constraints
+    problem.get_U(U);     // input box constraints
+    problem.get_D(D);     // general constraints
+    problem.get_D_N(D_N); // general terminal constraints
 
     bool do_gn_step = params.gn_interval > 0 and !params.disable_acceleration;
     bool did_gn     = false;
 
     // Make sure that we don't allocate any memory in the inner loop
     ScopedMallocBlocker mb;
 
     // Estimate Lipschitz constant ---------------------------------------------
 
     // Finite difference approximation of ∇²ψ in starting point
     if (params.Lipschitz.L_0 <= 0) {
-        initial_lipschitz_estimate(curr, do_gn_step, params.Lipschitz.ε,
-                                   params.Lipschitz.δ, params.L_min,
-                                   params.L_max, next->xu, next->grad_ψ);
+        initial_lipschitz_estimate(curr, params.Lipschitz.ε, params.Lipschitz.δ,
+                                   params.L_min, params.L_max, next->xu,
+                                   next->grad_ψ);
     }
     // Initial Lipschitz constant provided by the user
     else {
         curr->L = params.Lipschitz.L_0;
         // Calculate ψ(x₀), ∇ψ(x₀)
         eval_forward(*curr);
-        eval_backward(*curr, do_gn_step);
+        eval_backward(*curr);
     }
     if (not std::isfinite(curr->L)) {
         s.status = SolverStatus::NotFinite;
         return s;
     }
     curr->γ = params.Lipschitz.Lγ_factor / curr->L;
     eval_prox(*curr);
@@ -433,255 +523,276 @@
 
         // Check stop condition ------------------------------------------------
 
         real_t εₖ = calc_error_stop_crit(curr->γ, curr->xu, curr->grad_ψ,
                                          curr->p, curr->pᵀp, next->xû, next->p);
 
         // Print progress ------------------------------------------------------
-
-        if (params.print_interval != 0 && k % params.print_interval == 0)
-            print_progress(k, curr->fbe(), curr->ψu, curr->grad_ψ, curr->pᵀp,
-                           qxuₖ, curr->γ, τ, εₖ, did_gn,
-                           did_gn ? J.sizes().sum() : nJ, lqr.min_rcond);
-        if (progress_cb) {
-            ScopedMallocAllower ma;
-            progress_cb({.k             = k,
-                         .xu            = curr->xu,
-                         .p             = curr->p,
-                         .norm_sq_p     = curr->pᵀp,
-                         .x̂u            = curr->xû,
-                         .φγ            = curr->fbe(),
-                         .ψ             = curr->ψu,
-                         .grad_ψ        = curr->grad_ψ,
-                         .ψ_hat         = curr->ψû,
-                         .q             = qxuₖ,
-                         .gn            = did_gn,
-                         .nJ            = did_gn ? J.sizes().sum() : nJ,
-                         .lqr_min_rcond = lqr.min_rcond,
-                         .L             = curr->L,
-                         .γ             = curr->γ,
-                         .τ             = τ,
-                         .ε             = εₖ,
-                         .problem       = problem,
-                         .params        = params});
-        }
+        bool do_print =
+            params.print_interval != 0 && k % params.print_interval == 0;
+        if (do_print)
+            print_progress_1(k, curr->fbe(), curr->ψu, curr->grad_ψ, curr->pᵀp,
+                             curr->γ, εₖ);
 
         // Return solution -----------------------------------------------------
 
         auto time_elapsed = std::chrono::steady_clock::now() - start_time;
         auto stop_status =
             check_all_stop_conditions(time_elapsed, k, εₖ, no_progress);
         if (stop_status != SolverStatus::Busy) {
-            assign_extract_u(curr->xû, u);
-            s.iterations    = k;
-            s.ε             = εₖ;
-            s.elapsed_time  = duration_cast<nanoseconds>(time_elapsed);
-            s.time_forward  = eval.time.forward;
-            s.time_backward = eval.time.backward;
-            s.time_backward_jacobians = eval.time.backward_jacobians;
-            s.time_hessians           = eval.time.hessians;
-            s.status                  = stop_status;
-            s.final_γ                 = curr->γ;
+            do_progress_cb(k, *curr, null_vec<config_t>, -1, εₖ, false, 0,
+                           stop_status);
+            bool do_final_print = params.print_interval != 0;
+            if (!do_print && do_final_print)
+                print_progress_1(k, curr->fbe(), curr->ψu, curr->grad_ψ,
+                                 curr->pᵀp, curr->γ, εₖ);
+            if (do_print || do_final_print)
+                print_progress_n(stop_status);
+            if (stop_status == SolverStatus::Converged ||
+                stop_status == SolverStatus::Interrupted ||
+                opts.always_overwrite_results) {
+                write_solution(*curr);
+            }
+            s.iterations   = k;
+            s.ε            = εₖ;
+            s.elapsed_time = duration_cast<nanoseconds>(time_elapsed);
+            s.time_lqr_factor -= s.time_hessians;
+            s.status   = stop_status;
+            s.final_γ  = curr->γ;
+            s.final_ψ  = curr->ψû;
+            s.final_h  = 0; // only box constraints
+            s.final_φγ = curr->fbe();
             return s;
         }
 
         // Calculate Gauss-Newton step -----------------------------------------
 
         real_t τ_init = 1;
         did_gn        = do_gn_step;
         if (params.disable_acceleration) {
             τ_init = 0;
         } else if (do_gn_step) {
-            // Forward simulation has been carried out on xuₖ and the Jacobians
-            // are stored in 'eval'
-            if (!curr->have_jacobians)
-                throw std::logic_error("have_jacobians");
-
-            // Make sure that Q and R are stored as well
-            eval.hessians(curr->xu);
-
             auto is_constr_inactive = [&](index_t t, index_t i) {
-                real_t ui = eval.uk(curr->xu, t)(i);
+                real_t ui = vars.uk(curr->xu, t)(i);
                 // Gradient descent step.
                 real_t gs = ui - curr->γ * curr->grad_ψ(t * nu + i);
                 // Check whether the box constraints are active for this index.
                 bool active_lb = gs <= U.lowerbound(i);
                 bool active_ub = gs >= U.upperbound(i);
                 if (active_ub) {
-                    eval.uk(qxuₖ, t)(i) = U.upperbound(i) - ui;
+                    q(nu * t + i) = U.upperbound(i) - ui;
                     return false;
                 } else if (active_lb) {
-                    eval.uk(qxuₖ, t)(i) = U.lowerbound(i) - ui;
+                    q(nu * t + i) = U.lowerbound(i) - ui;
                     return false;
                 } else { // Store inactive indices
                     return true;
                 }
             };
             { // Find active indices J
-                detail::Timed t{s.time_indices};
+                alpaqa::util::Timed t{s.time_indices};
                 J.update(is_constr_inactive);
+                nJ = J.sizes().sum();
+            }
+            { // evaluate the Jacobians
+                alpaqa::util::Timed t{s.time_jacobians};
+                for (index_t t = 0; t < N; ++t)
+                    problem.eval_jac_f(t, vars.xk(curr->xu, t),
+                                       vars.uk(curr->xu, t), vars.ABk(jacs, t));
             }
-
             { // LQR factor
-                detail::Timed t{s.time_lqr_factor};
-                lqr.factor_masked(Ak, Bk, Qk, Rk, qk, rk, uk_eq, Jk, Kk,
-                                  params.lqr_factor_cholesky);
+                alpaqa::util::Timed t{s.time_lqr_factor};
+                lqr.factor_masked(ABk, Qk(curr->xu), Rk(curr->xu), Sk(curr->xu),
+                                  Rk_prod(curr->xu), Sk_prod(curr->xu), qk, rk,
+                                  uk_eq, Jk, Kk, params.lqr_factor_cholesky);
             }
             { // LQR solve
-                detail::Timed t{s.time_lqr_solve};
-                lqr.solve_masked(Ak, Bk, Jk, qxuₖ);
+                alpaqa::util::Timed t{s.time_lqr_solve};
+                lqr.solve_masked(ABk, Jk, q, work_2x);
             }
         } else {
             if (!enable_lbfgs)
                 throw std::logic_error("enable_lbfgs");
 
             // Find inactive indices J
             auto is_constr_inactive = [&](index_t t, index_t i) {
-                real_t ui     = eval.uk(curr->xu, t)(i);
+                real_t ui     = vars.uk(curr->xu, t)(i);
                 real_t grad_i = curr->grad_ψ(t * nu + i);
                 // Gradient descent step.
                 real_t gs = ui - curr->γ * grad_i;
                 // Check whether the box constraints are active for this index.
                 bool active_lb = gs <= U.lowerbound(i);
                 bool active_ub = gs >= U.upperbound(i);
                 if (active_ub || active_lb) {
-                    quₖ(t * nu + i) = curr->p(t * nu + i);
+                    q(t * nu + i) = curr->p(t * nu + i);
                     return false;
                 } else { // Store inactive indices
-                    quₖ(t * nu + i) = -grad_i;
+                    q(t * nu + i) = -grad_i;
                     return true;
                 }
             };
 
             auto J_idx = J.indices();
             nJ         = 0;
             {
-                detail::Timed t{s.time_lbfgs_indices};
+                alpaqa::util::Timed t{s.time_lbfgs_indices};
                 for (index_t t = 0; t < N; ++t)
                     for (index_t i = 0; i < nu; ++i)
                         if (is_constr_inactive(t, i))
                             J_idx(nJ++) = t * nu + i;
             }
             auto J_lbfgs = J_idx.topRows(nJ);
 
             // If all indices are inactive, we can use standard L-BFGS,
             // if there are active indices, we need the specialized version
             // that only applies L-BFGS to the inactive indices
             bool success = [&] {
-                detail::Timed t{s.time_lbfgs_apply};
-                return lbfgs.apply_masked(quₖ, curr->γ, J_lbfgs);
+                alpaqa::util::Timed t{s.time_lbfgs_apply};
+                return lbfgs.apply_masked(q, curr->γ, J_lbfgs);
             }();
             // If L-BFGS application failed, qₖ(J) still contains
             // -∇ψ(x)(J) - HqK(J) or -∇ψ(x)(J), which is not a valid step.
-            if (not success) {
+            if (not success)
                 τ_init = 0;
-            } else {
-                // for (index_t t = N; t-- > 0;)
-                //     for (index_t i = nu; i-- > 0;)
-                //         qxuₖ(t * (nx + nu) + nx + i) = qxuₖ(t * (0 + nu) + nx + i);
-                assign_interleave_xu(quₖ, qxuₖ);
-            }
         }
 
         // Make sure quasi-Newton step is valid
-        if (not qxuₖ.allFinite()) {
+        if (not q.allFinite()) {
             τ_init = 0;
             // Is there anything we can do?
             if (not did_gn)
                 lbfgs.reset();
         }
         s.lbfgs_failures += (τ_init == 0 && k > 0);
 
         bool do_next_gn = params.gn_interval > 0 &&
                           ((k + 1) % params.gn_interval) == 0 &&
                           !params.disable_acceleration;
         do_gn_step = do_next_gn || (do_gn_step && params.gn_sticky);
 
         // Line search ---------------------------------------------------------
 
-        next->γ = curr->γ;
-        next->L = curr->L;
-        τ       = τ_init;
+        next->γ           = curr->γ;
+        next->L           = curr->L;
+        τ                 = τ_init;
+        real_t τ_prev     = -1;
+        bool dir_rejected = true;
+
+        // xₖ₊₁ = xₖ + pₖ
+        auto take_safe_step = [&] {
+            next->xu = curr->xû;
+            next->ψu = curr->ψû;
+            // Calculate ∇ψ(xₖ₊₁)
+            eval_backward(*next);
+        };
+
+        // xₖ₊₁ = xₖ + (1-τ) pₖ + τ qₖ
+        auto take_accelerated_step = [&](real_t τ) {
+            if (τ == 1) {
+                for (index_t t = 0; t < N; ++t)
+                    vars.uk(next->xu, t) =
+                        vars.uk(curr->xu, t) + q.segment(t * nu, nu);
+            } else {
+                do_gn_step = do_next_gn;
+                for (index_t t = 0; t < N; ++t)
+                    vars.uk(next->xu, t) =
+                        vars.uk(curr->xu, t) +
+                        (1 - τ) * curr->p.segment(t * nu, nu) +
+                        τ * q.segment(t * nu, nu);
+            }
+            // Calculate ψ(xₖ₊₁), ∇ψ(xₖ₊₁)
+            eval_forward(*next); // Not necessary for DDP
+            eval_backward(*next);
+        };
 
+        // Backtracking line search loop
         while (!stop_signal.stop_requested()) {
 
-            // xₖ₊₁ = xₖ + (1-τ) pₖ + τ qₖ
-            if (τ == 0) {
-                next->xu = curr->xû;
-                next->ψu = curr->ψû;
-                // Calculate ∇ψ(xₖ₊₁)
-                curr->have_jacobians = false;
-                eval_backward(*next, do_gn_step);
-            } else {
-                if (τ == 1) {
-                    next->xu = curr->xu + qxuₖ;
-                } else {
-                    do_gn_step = do_next_gn;
-                    for (index_t t = 0; t < N; ++t)
-                        eval.uk(next->xu, t) =
-                            eval.uk(curr->xu, t) +
-                            (1 - τ) * curr->p.segment(t * nu, nu) +
-                            τ * eval.uk(qxuₖ, t);
-                }
-                // Calculate ψ(xₖ₊₁), ∇ψ(xₖ₊₁)
-                eval_forward(*next); // Not necessary for DDP
-                curr->have_jacobians = false;
-                eval_backward(*next, do_gn_step);
+            // Recompute step only if τ changed
+            if (τ != τ_prev) {
+                τ != 0 ? take_accelerated_step(τ) : take_safe_step();
+                τ_prev = τ;
+            }
+
+            // If the cost is not finite, or if the quadratic upper bound could
+            // not be satisfied, abandon the direction entirely, don't even
+            // bother backtracking.
+            bool fail = next->L >= params.L_max || !std::isfinite(next->ψu);
+            if (τ > 0 && fail) {
+                // Don't allow a bad accelerated step to destroy the FBS step
+                // size
+                next->L = curr->L;
+                next->γ = curr->γ;
+                // Line search failed
+                τ = 0;
+                if (enable_lbfgs)
+                    lbfgs.reset();
+                continue;
             }
 
             // Calculate x̂ₖ₊₁, ψ(x̂ₖ₊₁)
             eval_prox(*next);
             eval_forward_hat(*next);
 
-            // Quadratic upper bound
+            // Quadratic upper bound step size condition
             if (next->L < params.L_max && qub_violated(*next)) {
                 next->γ /= 2;
                 next->L *= 2;
-                τ = τ_init;
+                if (τ > 0)
+                    τ = τ_init;
+                ++s.stepsize_backtracks;
                 continue;
             }
 
             // Line search condition
             if (τ > 0 && linesearch_violated(*curr, *next)) {
                 τ /= 2;
-                if (τ < params.τ_min)
+                if (τ < params.min_linesearch_coefficient)
                     τ = 0;
+                ++s.linesearch_backtracks;
                 continue;
             }
 
-            // QUB and line search satisfied
+            // QUB and line search satisfied (or τ is 0 and L > L_max)
             break;
         }
 
         // If τ < τ_min the line search failed and we accepted the prox step
         s.linesearch_failures += (τ == 0 && τ_init > 0);
         s.τ_1_accepted += τ == 1;
-        s.count_τ += 1;
+        s.count_τ += (τ_init > 0);
         s.sum_τ += τ;
 
         // Check if we made any progress
         if (no_progress > 0 || k % params.max_no_progress == 0)
             no_progress = curr->xu == next->xu ? no_progress + 1 : 0;
 
         // Update L-BFGS -------------------------------------------------------
 
         if (enable_lbfgs) {
             const bool force = true;
             assign_extract_u(next->xu, next->u);
-            if (did_gn && params.reset_lbfgs_on_gn_step) {
+            bool reset_because_gn = did_gn && params.reset_lbfgs_on_gn_step;
+            if (reset_because_gn || curr->γ != next->γ) {
                 lbfgs.reset();
-            } else {
-                detail::Timed t{s.time_lbfgs_update};
-                s.lbfgs_rejected += not lbfgs.update(
+            }
+            if (!reset_because_gn) { // TODO: this may be too restrictive
+                alpaqa::util::Timed t{s.time_lbfgs_update};
+                s.lbfgs_rejected += dir_rejected = not lbfgs.update(
                     curr->u, next->u, curr->grad_ψ, next->grad_ψ,
                     LBFGS<config_t>::Sign::Positive, force);
             }
         }
 
+        // Print ---------------------------------------------------------------
+        do_progress_cb(k, *curr, q, τ, εₖ, did_gn, nJ, SolverStatus::Busy);
+        if (do_print && (k != 0 || did_gn))
+            print_progress_2(q, τ, did_gn, nJ, lqr.min_rcond, dir_rejected);
+
         // Advance step --------------------------------------------------------
         std::swap(curr, next);
         ++k;
     }
     throw std::logic_error("[PANOC] loop error");
 }
 
-} // namespace alpaqa
+} // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/CasADiFunctionWrapper.hpp` & `alpaqa-1.0.0a7/src/interop/casadi/include/alpaqa/casadi/CasADiFunctionWrapper.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     USING_ALPAQA_CONFIG(Conf);
     static_assert(std::is_same_v<real_t, casadi_real>);
 
     using casadi_dim = std::pair<casadi_int, casadi_int>;
 
     /// @throws std::invalid_argument
     CasADiFunctionEvaluator(casadi::Function &&f)
-        : fun(std::move(f)), iwork(fun.sz_iw()), dwork(fun.sz_w()) {
+        : fun(std::move(f)), iwork(fun.sz_iw()), dwork(fun.sz_w()),
+          arg_work(fun.sz_arg()), res_work(fun.sz_res()) {
         using namespace std::literals::string_literals;
         if (N_in != fun.n_in())
             throw std::invalid_argument(
                 "Invalid number of input arguments: got "s +
                 std::to_string(fun.n_in()) + ", should be " +
                 std::to_string(N_in) + ".");
         if (N_out != fun.n_out())
@@ -46,18 +47,19 @@
     }
 
     /// @throws std::invalid_argument
     void
     validate_dimensions(const std::array<casadi_dim, N_in> &dim_in   = {},
                         const std::array<casadi_dim, N_out> &dim_out = {}) {
         using namespace std::literals::string_literals;
-        static constexpr const char *count[]{"first",  "second", "third",
-                                             "fourth", "fifth",  "sixth"};
-        static_assert(N_in <= 6);
-        static_assert(N_out <= 6);
+        static constexpr std::array count{"first",   "second", "third",
+                                          "fourth",  "fifth",  "sixth",
+                                          "seventh", "eighth"};
+        static_assert(N_in <= count.size());
+        static_assert(N_out <= count.size());
         auto to_string = [](casadi_dim d) {
             return "(" + std::to_string(d.first) + ", " +
                    std::to_string(d.second) + ")";
         };
         for (size_t n = 0; n < N_in; ++n) {
             auto cs_n = static_cast<casadi_int>(n);
             if (dim_in[n].first != 0 && dim_in[n] != fun.size_in(cs_n))
@@ -74,26 +76,29 @@
                     " output argument: got " + to_string(fun.size_out(cs_n)) +
                     ", should be " + to_string(dim_out[n]) + ".");
         }
     }
 
   protected:
     void operator()(const double *const *in, double *const *out) const {
-        fun(const_cast<const double **>(in), const_cast<double **>(out),
-            iwork.data(), dwork.data(), 0);
+        std::copy_n(in, N_in, arg_work.begin());
+        std::copy_n(out, N_out, res_work.begin());
+        fun(arg_work.data(), res_work.data(), iwork.data(), dwork.data(), 0);
     }
 
   public:
     void operator()(const double *const (&in)[N_in],
                     double *const (&out)[N_out]) const {
         this->operator()(&in[0], &out[0]);
     }
 
   public:
     casadi::Function fun;
 
   private:
     mutable std::vector<casadi_int> iwork;
     mutable std::vector<double> dwork;
+    mutable std::vector<const double *> arg_work;
+    mutable std::vector<double *> res_work;
 };
 
 } // namespace alpaqa::casadi_loader
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/CasADiProblem.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/functional-problem.hpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,87 +1,73 @@
 #pragma once
 
-#include <alpaqa/casadi-loader-export.hpp>
-#include <alpaqa/config/config.hpp>
-#include <alpaqa/problem/type-erased-problem.hpp>
-#include "alpaqa/util/copyable_unique_ptr.hpp"
+#include <alpaqa/problem/box-constr-problem.hpp>
+#include <alpaqa/util/alloc-check.hpp>
 
 namespace alpaqa {
-namespace casadi_loader {
-template <Config>
-struct CasADiFunctionsWithParam;
-} // namespace casadi_loader
 
-/// Problem definition for a CasADi problem, loaded from a DLL.
+/// Problem class that allows specifying the basic functions as C++
+/// `std::function`s.
 /// @ingroup grp_Problems
 template <Config Conf = DefaultConfig>
-class CasADiProblem : public BoxConstrProblem<Conf> {
+class FunctionalProblem : public BoxConstrProblem<Conf> {
   public:
     USING_ALPAQA_CONFIG(Conf);
-    vec param;
+    using BoxConstrProblem<Conf>::BoxConstrProblem;
 
-    /// Load a problem generated by CasADi (with parameters).
-    ///
-    /// @param  filename
-    ///         Filename of the shared library to load the functions from.
-    /// @param  n
-    ///         Number of decision variables (@f$ x \in \R^n @f$).
-    /// @param  m
-    ///         Number of general constraints (@f$ g(x) \in \R^m @f$).
-    /// @param  p
-    ///         The number of parameters of the problem (second argument to all
-    ///         CasADi functions).
-    /// @param  second_order
-    ///         Load the additional functions required for second-order PANOC.
-    ///
-    /// The file should contain functions with the names `f`, `grad_f`, `g` and
-    /// `grad_g`. These functions evaluate the objective function, its gradient,
-    /// the constraints, and the constraint gradient times a vector respecitvely.
-    /// If @p second_order is true, additional functions `hess_L` and
-    /// `hess_L_prod` should be provided to evaluate the Hessian of the
-    /// Lagrangian and Hessian-vector products.
-    ///
-    /// If any of the dimensions are less than or equal to zero, they are
-    /// determined from the `g` function in the given file.
-    ///
-    /// @throws std::invalid_argument
-    ///         The dimensions of the loaded functions do not match.
-    CasADiProblem(const std::string &filename, length_t n = 0, length_t m = 0,
-                  length_t p = 0, bool second_order = false);
-    ~CasADiProblem();
-
-    CasADiProblem(const CasADiProblem &);
-    CasADiProblem &operator=(const CasADiProblem &);
-    CasADiProblem(CasADiProblem &&) noexcept;
-    CasADiProblem &operator=(CasADiProblem &&) noexcept;
+    std::function<real_t(crvec)> f;
+    std::function<void(crvec, rvec)> grad_f;
+    std::function<void(crvec, rvec)> g;
+    std::function<void(crvec, crvec, rvec)> grad_g_prod;
+    std::function<void(crvec, index_t, rvec)> grad_gi;
+    std::function<void(crvec, rmat)> jac_g;
+    std::function<void(crvec, crvec, real_t, crvec, rvec)> hess_L_prod;
+    std::function<void(crvec, crvec, real_t, rmat)> hess_L;
+    std::function<void(crvec, crvec, crvec, real_t, crvec, rvec)> hess_ψ_prod;
+    std::function<void(crvec, crvec, crvec, real_t, rmat)> hess_ψ;
 
     // clang-format off
-    [[nodiscard]] real_t eval_f(crvec x) const;
-    void eval_grad_f(crvec x, rvec grad_fx) const;
-    void eval_g(crvec x, rvec g) const;
-    void eval_grad_g_prod(crvec x, crvec y, rvec grad_gxy) const;
-    void eval_grad_ψ(crvec x, crvec y, crvec Σ, rvec grad_ψ, rvec work_n, rvec work_m) const;
-    [[nodiscard]] real_t eval_ψ_grad_ψ(crvec x, crvec y, crvec Σ, rvec grad_ψ, rvec work_n, rvec work_m) const;
-    void eval_grad_L(crvec x, crvec y, rvec grad_L, rvec work_n) const;
-    [[nodiscard]] real_t eval_ψ(crvec x, crvec y, crvec Σ, rvec ŷ) const;
-    void eval_grad_ψ_from_ŷ(crvec x, crvec ŷ, rvec grad_ψ, rvec work_n) const;
-    void eval_grad_gi(crvec x, index_t i, rvec grad_i) const;
-    void eval_hess_L_prod(crvec x, crvec y, crvec v, rvec Hv) const;
-    void eval_hess_L(crvec x, crvec y, rmat H) const;
+    real_t eval_f(crvec x) const { ScopedMallocAllower ma; return f(x); }
+    void eval_grad_f(crvec x, rvec grad_fx) const { ScopedMallocAllower ma; grad_f(x, grad_fx); }
+    void eval_g(crvec x, rvec gx) const { ScopedMallocAllower ma; g(x, gx); }
+    void eval_grad_g_prod(crvec x, crvec y, rvec grad_gxy) const { ScopedMallocAllower ma; grad_g_prod(x, y, grad_gxy); }
+    void eval_grad_gi(crvec x, index_t i, rvec grad_gix) const { ScopedMallocAllower ma; grad_gi(x, i, grad_gix); }
+    void eval_hess_L_prod(crvec x, crvec y, real_t scale, crvec v, rvec Hv) const { ScopedMallocAllower ma; hess_L_prod(x, y, scale, v, Hv); }
+    void eval_hess_ψ_prod(crvec x, crvec y, crvec Σ, real_t scale, crvec v, rvec Hv) const { ScopedMallocAllower ma; hess_ψ_prod(x, y, Σ, scale, v, Hv); }
     // clang-format on
+    void eval_jac_g(crvec x, rindexvec, rindexvec, rvec J_values) const {
+        ScopedMallocAllower ma;
+        if (J_values.size() > 0)
+            jac_g(x, J_values.reshaped(this->m, this->n));
+    }
+    void eval_hess_L(crvec x, crvec y, real_t scale, rindexvec, rindexvec, rvec H_values) const {
+        ScopedMallocAllower ma;
+        if (H_values.size() > 0)
+            hess_L(x, y, scale, H_values.reshaped(this->n, this->n));
+    }
+    void eval_hess_ψ(crvec x, crvec y, crvec Σ, real_t scale, rindexvec, rindexvec,
+                     rvec H_values) const {
+        ScopedMallocAllower ma;
+        if (H_values.size() > 0)
+            hess_ψ(x, y, Σ, scale, H_values.reshaped(this->n, this->n));
+    }
 
     /// @see @ref TypeErasedProblem::provides_eval_grad_gi
-    [[nodiscard]] bool provides_eval_grad_gi() const;
+    bool provides_eval_grad_gi() const { return bool{grad_gi}; }
+    /// @see @ref TypeErasedProblem::provides_eval_jac_g
+    bool provides_eval_jac_g() const { return bool{jac_g}; }
     /// @see @ref TypeErasedProblem::provides_eval_hess_L_prod
-    [[nodiscard]] bool provides_eval_hess_L_prod() const;
+    bool provides_eval_hess_L_prod() const { return bool{hess_L_prod}; }
     /// @see @ref TypeErasedProblem::provides_eval_hess_L
-    [[nodiscard]] bool provides_eval_hess_L() const;
-
-  private:
-    using Functions = casadi_loader::CasADiFunctionsWithParam<Conf>;
-    util::copyable_unique_ptr<Functions> impl;
+    bool provides_eval_hess_L() const { return bool{hess_L}; }
+    /// @see @ref TypeErasedProblem::provides_eval_hess_ψ_prod
+    bool provides_eval_hess_ψ_prod() const { return bool{hess_ψ_prod}; }
+    /// @see @ref TypeErasedProblem::provides_eval_hess_ψ
+    bool provides_eval_hess_ψ() const { return bool{hess_ψ}; }
+
+    FunctionalProblem(const FunctionalProblem &)                = default;
+    FunctionalProblem &operator=(const FunctionalProblem &)     = default;
+    FunctionalProblem(FunctionalProblem &&) noexcept            = default;
+    FunctionalProblem &operator=(FunctionalProblem &&) noexcept = default;
 };
 
-CASADI_LOADER_EXPORT_EXTERN_TEMPLATE(class, CasADiProblem, EigenConfigd);
-CASADI_LOADER_EXPORT_EXTERN_TEMPLATE(class, CasADiProblem, DefaultConfig);
-
-} // namespace alpaqa
+} // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/src/CasADiLoader-util.hpp` & `alpaqa-1.0.0a7/src/interop/casadi/include/alpaqa/implementation/casadi/CasADiLoader-util.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #pragma once
 
 #include <casadi/core/casadi_types.hpp>
 #include <casadi/core/external.hpp>
 #include <array>
+#include <optional>
 #include <stdexcept>
 #include <string>
+#include <utility>
 
 namespace alpaqa::casadi_loader {
 
 template <class F>
 auto wrap_load(const std::string &so_name, const char *name, F f) {
     try {
         return f();
@@ -22,14 +24,25 @@
 auto wrapped_load(const std::string &so_name, const char *name,
                   Args &&...args) {
     return wrap_load(so_name, name, [&] {
         return T(casadi::external(name, so_name), std::forward<Args>(args)...);
     });
 }
 
+template <class T, class... Args>
+std::optional<T> try_load(const std::string &so_name, const char *name,
+                          Args &&...args) {
+    try {
+        return std::make_optional(
+            wrapped_load<T>(so_name, name, std::forward<Args>(args)...));
+    } catch (casadi::CasadiException &e) {
+        return std::nullopt;
+    }
+}
+
 using dim = std::pair<casadi_int, casadi_int>;
 inline constexpr auto dims(auto... a) {
     if constexpr ((... && std::is_constructible_v<dim, decltype(a)>))
         return std::array{a...};
     else
         return std::array{dim{a, 1}...};
 }
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/interop/casadi/src/CasADiProblem.tpp` & `alpaqa-1.0.0a7/src/interop/casadi/include/alpaqa/implementation/casadi/CasADiProblem.tpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,70 @@
 #pragma once
 
-#include <alpaqa/interop/casadi/CasADiFunctionWrapper.hpp>
-#include <alpaqa/interop/casadi/CasADiProblem.hpp>
+#include <alpaqa/casadi/CasADiFunctionWrapper.hpp>
+#include <alpaqa/casadi/CasADiProblem.hpp>
+#include <alpaqa/util/io/csv.hpp>
 #include <alpaqa/util/not-implemented.hpp>
 #include "CasADiLoader-util.hpp"
 
 #include <casadi/core/external.hpp>
 
+#include <algorithm>
+#include <filesystem>
+#include <fstream>
 #include <memory>
 #include <optional>
 #include <stdexcept>
 #include <type_traits>
 
 namespace alpaqa {
 
+namespace fs = std::filesystem;
+
 namespace casadi_loader {
 
 template <Config Conf>
 struct CasADiFunctionsWithParam {
-    static constexpr bool WithParam = true;
-    CasADiFunctionEvaluator<Conf, 1 + WithParam, 1> f;
-    // CasADiFunctionEvaluator<5 + WithParam, 1> grad_ψ;
-    CasADiFunctionEvaluator<Conf, 5 + WithParam, 2> ψ_grad_ψ;
+    USING_ALPAQA_CONFIG(Conf);
+    CasADiFunctionEvaluator<Conf, 2, 1> f;
+    CasADiFunctionEvaluator<Conf, 2, 2> f_grad_f;
+    // CasADiFunctionEvaluator<6, 1> grad_ψ;
+    CasADiFunctionEvaluator<Conf, 6, 2> ψ_grad_ψ;
     struct ConstrFun {
-        CasADiFunctionEvaluator<Conf, 1 + WithParam, 1> g;
-        CasADiFunctionEvaluator<Conf, 2 + WithParam, 1> grad_L;
-        CasADiFunctionEvaluator<Conf, 5 + WithParam, 2> ψ;
-    };
-    std::optional<ConstrFun> constr;
-    struct HessFun {
-        CasADiFunctionEvaluator<Conf, 3 + WithParam, 1> hess_L_prod;
-        CasADiFunctionEvaluator<Conf, 2 + WithParam, 1> hess_L;
+        CasADiFunctionEvaluator<Conf, 2, 1> g;
+        CasADiFunctionEvaluator<Conf, 3, 1> grad_L;
+        CasADiFunctionEvaluator<Conf, 6, 2> ψ;
     };
-    std::optional<HessFun> hess;
+    std::optional<ConstrFun> constr = std::nullopt;
+    std::optional<CasADiFunctionEvaluator<Conf, 5, 1>> hess_L_prod =
+        std::nullopt;
+    std::optional<CasADiFunctionEvaluator<Conf, 4, 1>> hess_L = std::nullopt;
+    std::optional<CasADiFunctionEvaluator<Conf, 8, 1>> hess_ψ_prod =
+        std::nullopt;
+    std::optional<CasADiFunctionEvaluator<Conf, 7, 1>> hess_ψ = std::nullopt;
+    std::optional<CasADiFunctionEvaluator<Conf, 2, 1>> jac_g  = std::nullopt;
+    indexvec inner_H{}, outer_H{};
+    indexvec inner_J{}, outer_J{};
 };
 
 } // namespace casadi_loader
 
+namespace detail {
+
+template <Config Conf>
+auto casadi_to_index(casadi_int i) -> index_t<Conf> {
+    return static_cast<index_t<Conf>>(i);
+}
+} // namespace detail
+
 template <Config Conf>
-CasADiProblem<Conf>::CasADiProblem(const std::string &so_name, length_t n,
-                                   length_t m, length_t p, bool second_order)
-    : BoxConstrProblem<Conf>{n, m} {
+CasADiProblem<Conf>::CasADiProblem(const std::string &so_name)
+    : BoxConstrProblem<Conf>{0, 0} {
     using namespace casadi_loader;
+    length_t n = 0, m = 0, p = 0;
     auto load_g_unknown_dims =
         [&]() -> std::optional<CasADiFunctionEvaluator<Conf, 2, 1>> {
         casadi::Function gfun = casadi::external("g", so_name);
         using namespace std::literals::string_literals;
         if (gfun.n_in() != 2)
             throw std::invalid_argument(
                 "Invalid number of input arguments: got "s +
@@ -59,92 +78,128 @@
                 "First input argument should be a column vector.");
         if (gfun.size2_in(1) != 1)
             throw std::invalid_argument(
                 "Second input argument should be a column vector.");
         if (gfun.n_out() == 1 && gfun.size2_out(0) != 1)
             throw std::invalid_argument(
                 "First output argument should be a column vector.");
-        if (n <= 0)
-            n = static_cast<length_t>(gfun.size1_in(0));
-        if (m <= 0 && gfun.n_out() == 1)
+        n = static_cast<length_t>(gfun.size1_in(0));
+        if (gfun.n_out() == 1)
             m = static_cast<length_t>(gfun.size1_out(0));
-        if (p <= 0)
-            p = static_cast<length_t>(gfun.size1_in(1));
+        p = static_cast<length_t>(gfun.size1_in(1));
         if (gfun.n_out() == 0) {
             if (m != 0)
                 throw std::invalid_argument(
                     "Function g has no outputs but m != 0");
             return std::nullopt;
         }
         CasADiFunctionEvaluator<Conf, 2, 1> g{std::move(gfun)};
         g.validate_dimensions({dim(n, 1), dim(p, 1)}, {dim(m, 1)});
         return std::make_optional(std::move(g));
     };
 
-    auto load_g_known_dims = [&] {
-        CasADiFunctionEvaluator<Conf, 2, 1> g{casadi::external("g", so_name),
-                                              {dim(n, 1), dim(p, 1)},
-                                              {dim(m, 1)}};
-        return g;
-    };
-
-    std::optional<CasADiFunctionEvaluator<Conf, 2, 1>> g =
-        (n <= 0 || m <= 0 || p <= 0)
-            // If not all dimensions are specified, load the function "g" to
-            // determine the missing dimensions.
-            ? wrap_load(so_name, "g", load_g_unknown_dims)
-            // Otherwise, load the function "g" and compare its dimensions to
-            // the dimensions specified by the user.
-            : wrap_load(so_name, "g", load_g_known_dims);
+    auto g = wrap_load(so_name, "g", load_g_unknown_dims);
 
     this->n     = n;
     this->m     = m;
     this->param = vec::Constant(p, alpaqa::NaN<Conf>);
-    this->C     = {vec::Constant(n, +alpaqa::inf<Conf>),
-                   vec::Constant(n, -alpaqa::inf<Conf>)};
-    this->D     = {vec::Constant(m, +alpaqa::inf<Conf>),
-                   vec::Constant(m, -alpaqa::inf<Conf>)};
+    this->C     = Box<config_t>{n};
+    this->D     = Box<config_t>{m};
 
     impl = std::make_unique<CasADiFunctionsWithParam<Conf>>(
         CasADiFunctionsWithParam<Conf>{
-            wrapped_load<CasADiFunctionEvaluator<Conf, 2, 1>>( //
+            .f        = wrapped_load<CasADiFunctionEvaluator<Conf, 2, 1>>( //
                 so_name, "f", dims(n, p), dims(1)),
-            // wrapped_load<CasADiFunctionEvaluator<6, 1>>( //
+            .f_grad_f = wrapped_load<CasADiFunctionEvaluator<Conf, 2, 2>>( //
+                so_name, "f_grad_f", dims(n, p), dims(1, n)),
+            // .grad_ψ = wrapped_load<CasADiFunctionEvaluator<6, 1>>( //
             //     so_name, "grad_psi", dims(n, p, m, m, m, m), dims(n)),
-            wrapped_load<CasADiFunctionEvaluator<Conf, 6, 2>>( //
+            .ψ_grad_ψ = wrapped_load<CasADiFunctionEvaluator<Conf, 6, 2>>( //
                 so_name, "psi_grad_psi", dims(n, p, m, m, m, m), dims(1, n)),
-            std::nullopt,
-            std::nullopt,
         });
 
     if (g)
-        impl->constr = std::make_optional(
-            typename CasADiFunctionsWithParam<Conf>::ConstrFun{
-                std::move(*g),
-                wrapped_load<CasADiFunctionEvaluator<Conf, 3, 1>>( //
-                    so_name, "grad_L", dims(n, p, m), dims(n)),
-                wrapped_load<CasADiFunctionEvaluator<Conf, 6, 2>>( //
-                    so_name, "psi", dims(n, p, m, m, m, m), dims(1, m)),
-            });
-
-    if (second_order)
-        impl->hess =
-            std::make_optional(typename CasADiFunctionsWithParam<Conf>::HessFun{
-                wrapped_load<CasADiFunctionEvaluator<Conf, 4, 1>>( //
-                    so_name, "hess_L_prod", dims(n, p, m, n), dims(n)),
-                wrapped_load<CasADiFunctionEvaluator<Conf, 3, 1>>( //
-                    so_name, "hess_L", dims(n, p, m), dims(dim(n, n))),
-            });
+        impl->constr = {
+            std::move(*g),
+            wrapped_load<CasADiFunctionEvaluator<Conf, 3, 1>>( //
+                so_name, "grad_L", dims(n, p, m), dims(n)),
+            wrapped_load<CasADiFunctionEvaluator<Conf, 6, 2>>( //
+                so_name, "psi", dims(n, p, m, m, m, m), dims(1, m)),
+        };
+
+    impl->hess_L_prod = try_load<CasADiFunctionEvaluator<Conf, 5, 1>>( //
+        so_name, "hess_L_prod", dims(n, p, m, 1, n), dims(n));
+    impl->hess_L      = try_load<CasADiFunctionEvaluator<Conf, 4, 1>>( //
+        so_name, "hess_L", dims(n, p, m, 1), dims(dim(n, n)));
+    impl->hess_ψ_prod = try_load<CasADiFunctionEvaluator<Conf, 8, 1>>( //
+        so_name, "hess_psi_prod", dims(n, p, m, m, 1, m, m, n), dims(n));
+    impl->hess_ψ      = try_load<CasADiFunctionEvaluator<Conf, 7, 1>>( //
+        so_name, "hess_psi", dims(n, p, m, m, 1, m, m), dims(dim(n, n)));
+    impl->jac_g       = try_load<CasADiFunctionEvaluator<Conf, 2, 1>>( //
+        so_name, "jacobian_g", dims(n, p), dims(dim(m, n)));
+
+    auto data_filepath = fs::path{so_name}.replace_extension("csv");
+    if (fs::exists(data_filepath))
+        load_numerical_data(data_filepath);
 }
 
 template <Config Conf>
-CasADiProblem<Conf>::CasADiProblem(const CasADiProblem &o) = default;
+void CasADiProblem<Conf>::load_numerical_data(
+    const std::filesystem::path &filepath, char sep) {
+    // Open data file
+    std::ifstream data_file{filepath};
+    if (!data_file)
+        throw std::runtime_error("Unable to open data file \"" +
+                                 filepath.string() + '"');
+
+    // Helper function for reading single line of (float) data
+    index_t line        = 0;
+    auto wrap_data_load = [&](std::string_view name, auto &v, bool fixed_size) {
+        try {
+            ++line;
+            if (data_file.peek() == '\n') // Ignore empty lines
+                return static_cast<void>(data_file.get());
+            if (fixed_size) {
+                csv::read_row(data_file, v, sep);
+            } else { // Dynamic size
+                auto s = csv::read_row_std_vector<real_t>(data_file, sep);
+                v      = cmvec{s.data(), static_cast<index_t>(s.size())};
+            }
+        } catch (csv::read_error &e) {
+            // Transform any errors in something more readable
+            throw std::runtime_error("Unable to read " + std::string(name) +
+                                     " from data file \"" +
+                                     filepath.string() + ':' +
+                                     std::to_string(line) + "\": " + e.what());
+        }
+    };
+    // Helper function for reading a single value
+    auto read_single = [&](std::string_view name, auto &v) {
+        data_file >> v;
+        if (!data_file)
+            throw std::runtime_error(
+                "Unable to read " + std::string(name) + " from data file \"" +
+                filepath.string() + ':' + std::to_string(line) + '"');
+    };
+    // Read the bounds, parameter value, and regularization
+    wrap_data_load("C.lowerbound", this->C.lowerbound, true);
+    wrap_data_load("C.upperbound", this->C.upperbound, true);
+    wrap_data_load("D.lowerbound", this->D.lowerbound, true);
+    wrap_data_load("D.upperbound", this->D.upperbound, true);
+    wrap_data_load("param", this->param, true);
+    wrap_data_load("l1_reg", this->l1_reg, false);
+    // Penalty/ALM split is a single integer
+    read_single("penalty_alm_split", this->penalty_alm_split);
+}
+
+template <Config Conf>
+CasADiProblem<Conf>::CasADiProblem(const CasADiProblem &) = default;
 template <Config Conf>
 CasADiProblem<Conf> &
-CasADiProblem<Conf>::operator=(const CasADiProblem &o) = default;
+CasADiProblem<Conf>::operator=(const CasADiProblem &) = default;
 template <Config Conf>
 CasADiProblem<Conf>::CasADiProblem(CasADiProblem &&) noexcept = default;
 template <Config Conf>
 CasADiProblem<Conf> &
 CasADiProblem<Conf>::operator=(CasADiProblem &&) noexcept = default;
 
 template <Config Conf>
@@ -154,24 +209,30 @@
 auto CasADiProblem<Conf>::eval_f(crvec x) const -> real_t {
     real_t f;
     impl->f({x.data(), param.data()}, {&f});
     return f;
 }
 
 template <Config Conf>
-void CasADiProblem<Conf>::eval_grad_f(crvec, rvec) const {
-    throw not_implemented_error("CasADiProblem::eval_grad_f"); // TODO
+void CasADiProblem<Conf>::eval_grad_f(crvec x, rvec grad_fx) const {
+    real_t f;
+    impl->f_grad_f({x.data(), param.data()}, {&f, grad_fx.data()});
+}
+
+template <Config Conf>
+auto CasADiProblem<Conf>::eval_f_grad_f(crvec x, rvec grad_fx) const -> real_t {
+    real_t f;
+    impl->f_grad_f({x.data(), param.data()}, {&f, grad_fx.data()});
+    return f;
 }
 
 template <Config Conf>
 void CasADiProblem<Conf>::eval_g(crvec x, rvec g) const {
     if (impl->constr)
         impl->constr->g({x.data(), param.data()}, {g.data()});
-    else
-        throw std::logic_error("No constraints function g"); // TODO
 }
 
 template <Config Conf>
 void CasADiProblem<Conf>::eval_grad_g_prod(crvec, crvec, rvec) const {
     throw not_implemented_error("CasADiProblem::eval_grad_g_prod"); // TODO
 }
 
@@ -206,15 +267,15 @@
 template <Config Conf>
 void CasADiProblem<Conf>::eval_grad_L(crvec x, crvec y, rvec grad_L,
                                       rvec) const {
     if (impl->constr)
         impl->constr->grad_L({x.data(), param.data(), y.data()},
                              {grad_L.data()});
     else
-        throw std::logic_error("No function grad_L");
+        eval_f_grad_f(x, grad_L);
 }
 
 template <Config Conf>
 typename CasADiProblem<Conf>::real_t
 CasADiProblem<Conf>::eval_ψ(crvec x, crvec y, crvec Σ, rvec ŷ) const {
     real_t ψ;
     if (impl->constr)
@@ -223,59 +284,142 @@
                         {&ψ, ŷ.data()});
     else
         impl->f({x.data(), param.data()}, {&ψ});
     return ψ;
 }
 
 template <Config Conf>
-void CasADiProblem<Conf>::eval_grad_ψ_from_ŷ(crvec x, crvec ŷ, rvec grad_ψ,
-                                             rvec) const {
-    if (this->m == 0) {
-        real_t ψ;
-        impl->ψ_grad_ψ(
-            {x.data(), param.data(), nullptr, nullptr, nullptr, nullptr},
-            {&ψ, grad_ψ.data()});
+void CasADiProblem<Conf>::eval_grad_gi(crvec, index_t, rvec) const {
+    throw not_implemented_error("CasADiProblem::eval_grad_gi"); // TODO
+}
+
+template <Config Conf>
+auto CasADiProblem<Conf>::get_jac_g_num_nonzeros() const -> length_t {
+    if (!impl->jac_g.has_value())
+        return 0;
+    auto &&sparsity = impl->jac_g->fun.sparsity_out(0);
+    return sparsity.is_dense() ? 0 : static_cast<length_t>(sparsity.nnz());
+}
+
+template <Config Conf>
+void CasADiProblem<Conf>::eval_jac_g(crvec x, rindexvec inner_idx,
+                                     rindexvec outer_ptr, rvec J_values) const {
+    assert(impl->jac_g.has_value());
+    if (J_values.size() > 0) {
+        (*impl->jac_g)({x.data(), param.data()}, {J_values.data()});
     } else {
-        impl->constr->grad_L({x.data(), param.data(), ŷ.data()},
-                             {grad_ψ.data()});
+        auto &&sparsity = impl->jac_g->fun.sparsity_out(0);
+        using detail::casadi_to_index;
+        if (!sparsity.is_dense()) {
+            std::transform(sparsity.row(), sparsity.row() + sparsity.nnz(),
+                           inner_idx.begin(), casadi_to_index<config_t>);
+            std::transform(sparsity.colind(),
+                           sparsity.colind() + this->get_n() + 1,
+                           outer_ptr.begin(), casadi_to_index<config_t>);
+        }
     }
 }
 
 template <Config Conf>
-void CasADiProblem<Conf>::eval_grad_gi(crvec, index_t, rvec) const {
-    throw not_implemented_error("CasADiProblem::eval_grad_gi"); // TODO
+void CasADiProblem<Conf>::eval_hess_L_prod(crvec x, crvec y, real_t scale,
+                                           crvec v, rvec Hv) const {
+    assert(impl->hess_L_prod.has_value());
+    (*impl->hess_L_prod)({x.data(), param.data(), y.data(), &scale, v.data()},
+                         {Hv.data()});
+}
+
+template <Config Conf>
+auto CasADiProblem<Conf>::get_hess_L_num_nonzeros() const -> length_t {
+    if (!impl->hess_L.has_value())
+        return 0;
+    auto &&sparsity = impl->hess_L->fun.sparsity_out(0);
+    return sparsity.is_dense() ? 0 : static_cast<length_t>(sparsity.nnz());
+}
+
+template <Config Conf>
+void CasADiProblem<Conf>::eval_hess_L(crvec x, crvec y, real_t scale,
+                                      rindexvec inner_idx, rindexvec outer_ptr,
+                                      rvec H_values) const {
+    assert(impl->hess_L.has_value());
+    if (H_values.size() > 0) {
+        (*impl->hess_L)({x.data(), param.data(), y.data(), &scale},
+                        {H_values.data()});
+    } else {
+        auto &&sparsity = impl->hess_L->fun.sparsity_out(0);
+        using detail::casadi_to_index;
+        if (!sparsity.is_dense()) {
+            std::transform(sparsity.row(), sparsity.row() + sparsity.nnz(),
+                           inner_idx.begin(), casadi_to_index<config_t>);
+            std::transform(sparsity.colind(),
+                           sparsity.colind() + this->get_n() + 1,
+                           outer_ptr.begin(), casadi_to_index<config_t>);
+        }
+    }
 }
 
 template <Config Conf>
-void CasADiProblem<Conf>::eval_hess_L_prod(crvec x, crvec y, crvec v,
+void CasADiProblem<Conf>::eval_hess_ψ_prod(crvec x, crvec y, crvec Σ,
+                                           real_t scale, crvec v,
                                            rvec Hv) const {
-    impl->hess->hess_L_prod({x.data(), param.data(), y.data(), v.data()},
-                            {Hv.data()});
+    assert(impl->hess_ψ_prod.has_value());
+    (*impl->hess_ψ_prod)({x.data(), param.data(), y.data(), Σ.data(), &scale,
+                          this->D.lowerbound.data(), this->D.upperbound.data(),
+                          v.data()},
+                         {Hv.data()});
 }
+
 template <Config Conf>
-void CasADiProblem<Conf>::eval_hess_L(crvec x, crvec y, rmat H) const {
-    impl->hess->hess_L({x.data(), param.data(), y.data()}, {H.data()});
+auto CasADiProblem<Conf>::get_hess_ψ_num_nonzeros() const -> length_t {
+    if (!impl->hess_ψ.has_value())
+        return 0;
+    auto &&sparsity = impl->hess_ψ->fun.sparsity_out(0);
+    return sparsity.is_dense() ? 0 : static_cast<length_t>(sparsity.nnz());
+}
+
+template <Config Conf>
+void CasADiProblem<Conf>::eval_hess_ψ(crvec x, crvec y, crvec Σ, real_t scale,
+                                      rindexvec inner_idx, rindexvec outer_ptr,
+                                      rvec H_values) const {
+    assert(impl->hess_ψ.has_value());
+    if (H_values.size() > 0) {
+        (*impl->hess_ψ)({x.data(), param.data(), y.data(), Σ.data(), &scale,
+                         this->D.lowerbound.data(), this->D.upperbound.data()},
+                        {H_values.data()});
+    } else {
+        auto &&sparsity = impl->hess_ψ->fun.sparsity_out(0);
+        using detail::casadi_to_index;
+        if (!sparsity.is_dense()) {
+            std::transform(sparsity.row(), sparsity.row() + sparsity.nnz(),
+                           inner_idx.begin(), casadi_to_index<config_t>);
+            std::transform(sparsity.colind(),
+                           sparsity.colind() + this->get_n() + 1,
+                           outer_ptr.begin(), casadi_to_index<config_t>);
+        }
+    }
 }
 
 template <Config Conf>
 bool CasADiProblem<Conf>::provides_eval_grad_gi() const {
     return false; // TODO
 }
 template <Config Conf>
+bool CasADiProblem<Conf>::provides_eval_jac_g() const {
+    return impl->jac_g.has_value();
+}
+template <Config Conf>
 bool CasADiProblem<Conf>::provides_eval_hess_L_prod() const {
-    return impl->hess.has_value();
+    return impl->hess_L_prod.has_value();
 }
 template <Config Conf>
 bool CasADiProblem<Conf>::provides_eval_hess_L() const {
-    return impl->hess.has_value();
+    return impl->hess_L.has_value();
+}
+template <Config Conf>
+bool CasADiProblem<Conf>::provides_eval_hess_ψ_prod() const {
+    return impl->hess_ψ_prod.has_value();
 }
-
 template <Config Conf>
-auto load_CasADi_problem_with_param(const std::string &filename,
-                                    typename Conf::length_t n,
-                                    typename Conf::length_t m,
-                                    typename Conf::length_t p,
-                                    bool second_order) {
-    return CasADiProblem<Conf>{filename, n, m, p, second_order};
+bool CasADiProblem<Conf>::provides_eval_hess_ψ() const {
+    return impl->hess_ψ.has_value();
 }
 
 } // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/outer/alm.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/outer/alm.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -3,85 +3,81 @@
 #include <alpaqa/config/config.hpp>
 #include <alpaqa/export.hpp>
 #include <alpaqa/inner/internal/solverstatus.hpp>
 #include <alpaqa/outer/internal/alm-helpers.hpp>
 #include <alpaqa/problem/type-erased-problem.hpp>
 
 #include <chrono>
+#include <iostream>
 #include <string>
 
 namespace alpaqa {
 
 template <class InnerSolverStats>
 struct InnerStatsAccumulator;
 
 /// Parameters for the Augmented Lagrangian solver.
 template <Config Conf = DefaultConfig>
 struct ALMParams {
     USING_ALPAQA_CONFIG(Conf);
 
-    /// Primal tolerance.
-    real_t ε = 1e-5;
-    /// Dual tolerance.
-    real_t δ = 1e-5;
+    /// Primal tolerance (used for stopping criterion of inner solver).
+    real_t tolerance = real_t(1e-5);
+    /// Dual tolerance (constraint violation and complementarity).
+    real_t dual_tolerance = real_t(1e-5);
     /// Factor used in updating the penalty parameters.
-    real_t Δ = 10;
-    /// Factor to reduce @ref Δ when inner convergence fails.
-    real_t Δ_lower = 0.8;
-    /// Minimum value for @ref Δ after reduction because of inner convergence
+    real_t penalty_update_factor = 10;
+    /// Factor to reduce @ref penalty_update_factor when inner convergence fails.
+    real_t penalty_update_factor_lower = real_t(0.8);
+    /// Minimum value for @ref penalty_update_factor after reduction because of inner convergence
     /// failure.
-    real_t Δ_min = 1.1;
+    real_t min_penalty_update_factor = real_t(1.1);
     /// Initial penalty parameter. When set to zero (which is the default),
     /// it is computed automatically, based on the constraint violation in the
-    /// starting point and the parameter @ref σ_0.
+    /// starting point and the parameter @ref initial_penalty_factor.
     /// @todo Change default to 0.
-    real_t Σ_0 = 1;
-    /// Initial penalty parameter factor. Active if @ref Σ_0 is set
+    real_t initial_penalty = 1;
+    /// Initial penalty parameter factor. Active if @ref initial_penalty is set
     /// to zero.
-    real_t σ_0 = 20;
+    real_t initial_penalty_factor = 20;
     /// Factor to reduce the initial penalty factor by if convergence fails in
     /// in the first iteration.
-    real_t Σ_0_lower = 0.6;
+    real_t initial_penalty_lower = real_t(0.6);
     /// Initial primal tolerance.
-    real_t ε_0 = 1;
+    real_t initial_tolerance = 1;
     /// Factor to increase the initial primal tolerance if convergence fails in
     /// the first iteration.
-    real_t ε_0_increase = 1.1;
+    real_t initial_tolerance_increase = real_t(1.1);
     /// Update factor for primal tolerance.
-    real_t ρ = 1e-1;
+    real_t tolerance_update_factor = real_t(1e-1);
     /// Factor to increase the primal tolerance update factor by if convergence
     /// fails.
-    real_t ρ_increase = 2;
-    /// Maximum value of @ref ρ after increase because of inner convergence
+    real_t ρ_increase = real_t(2);
+    /// Maximum value of @ref tolerance_update_factor after increase because of inner convergence
     /// failure.
-    real_t ρ_max = 0.5;
+    real_t ρ_max = real_t(0.5);
     /// Error tolerance for penalty increase
-    real_t θ = 0.1;
+    real_t rel_penalty_increase_threshold = real_t(0.1);
     /// Lagrange multiplier bound.
-    real_t M = 1e9;
-    /// Components of the constraint function with indices below this number are
-    /// handled using the quadratic penalty method rather than using an
-    /// augmented Lagrangian method. Specifically, the Lagrange multipliers for
-    /// these components (which determine the shifts in ALM) are kept at zero.
-    index_t penalty_alm_split = 0;
+    real_t max_multiplier = real_t(1e9);
     /// Maximum penalty factor.
-    real_t Σ_max = 1e9;
+    real_t max_penalty = real_t(1e9);
     /// Minimum penalty factor (used during initialization).
-    real_t Σ_min = 1e-9;
+    real_t min_penalty = real_t(1e-9);
     /// Maximum number of outer ALM iterations.
     unsigned int max_iter = 100;
     /// Maximum duration.
-    std::chrono::microseconds max_time = std::chrono::minutes(5);
+    std::chrono::nanoseconds max_time = std::chrono::minutes(5);
 
-    /// How many times can the initial penalty @ref Σ_0 or
-    /// @ref σ_0 and the initial primal tolerance @ref ε_0
+    /// How many times can the initial penalty @ref initial_penalty or
+    /// @ref initial_penalty_factor and the initial primal tolerance @ref initial_tolerance
     /// be reduced.
     unsigned max_num_initial_retries = 0;
-    /// How many times can the penalty update factor @ref Δ and the
-    /// primal tolerance factor @ref ρ be reduced.
+    /// How many times can the penalty update factor @ref penalty_update_factor and the
+    /// primal tolerance factor @ref tolerance_update_factor be reduced.
     unsigned max_num_retries = 0;
     /// Combined limit for @ref max_num_initial_retries and
     /// @ref max_num_retries.
     unsigned max_total_num_retries = 0;
 
     /// When to print progress. If set to zero, nothing will be printed.
     /// If set to N != 0, progress is printed every N iterations.
@@ -97,39 +93,39 @@
 ///
 /// @ingroup    grp_ALMSolver
 template <class InnerSolverT>
 class ALMSolver {
   public:
     USING_ALPAQA_CONFIG_TEMPLATE(InnerSolverT::config_t);
 
-    using Problem     = TypeErasedProblem<config_t>;
     using Params      = ALMParams<config_t>;
     using InnerSolver = InnerSolverT;
+    using Problem     = typename InnerSolver::Problem;
 
     struct Stats {
         /// Total number of outer ALM iterations (i.e. the number of times that
         /// the inner solver was invoked).
         unsigned outer_iterations = 0;
         /// Total elapsed time.
-        std::chrono::nanoseconds elapsed_time;
+        std::chrono::nanoseconds elapsed_time{};
         /// The number of times that the initial penalty factor was reduced by
-        /// @ref ALMParams::Σ_0_lower and that the initial tolerance was
-        /// increased by @ref ALMParams::ε_0_increase because the inner solver
+        /// @ref ALMParams::initial_penalty_lower and that the initial tolerance was
+        /// increased by @ref ALMParams::initial_tolerance_increase because the inner solver
         /// failed to converge in the first ALM iteration. If this number is
         /// greater than zero, consider lowering the initial penalty factor
-        /// @ref ALMParams::Σ_0 or @ref ALMParams::σ_0 or increasing the initial
-        /// tolerance @ref ALMParams::ε_0 (or both).
+        /// @ref ALMParams::initial_penalty or @ref ALMParams::initial_penalty_factor or increasing the initial
+        /// tolerance @ref ALMParams::initial_tolerance (or both).
         unsigned initial_penalty_reduced = 0;
-        /// The number of times that the penalty update factor @ref ALMParams::Δ
-        /// was reduced, that the tolerance update factor @ref ALMParams::ρ was
+        /// The number of times that the penalty update factor @ref ALMParams::penalty_update_factor
+        /// was reduced, that the tolerance update factor @ref ALMParams::tolerance_update_factor was
         /// increased, and that an ALM iteration had to be restarted with a
         /// lower penalty factor and a higher tolerance because the inner solver
         /// failed to converge (not applicable in the first ALM iteration).
         /// If this number is greater than zero, consider lowerering the
-        /// penalty update factor @ref ALMParams::Δ or increasing the tolerance
+        /// penalty update factor @ref ALMParams::penalty_update_factor or increasing the tolerance
         /// update factor (or both). Lowering the initial penalty factor could
         /// help as well.
         unsigned penalty_reduced = 0;
         /// The total number of times that the inner solver failed to converge.
         unsigned inner_convergence_failures = 0;
         /// Final primal tolerance that was reached, depends on the stopping
         /// criterion used by the inner solver, see for example
@@ -154,18 +150,18 @@
 
     ALMSolver(Params params, InnerSolver &&inner_solver)
         : params(params),
           inner_solver(std::forward<InnerSolver>(inner_solver)) {}
     ALMSolver(Params params, const InnerSolver &inner_solver)
         : params(params), inner_solver(inner_solver) {}
 
-    Stats operator()(const Problem &problem, rvec y, rvec x);
+    Stats operator()(const Problem &problem, rvec x, rvec y);
     template <class P>
-    Stats operator()(const P &problem, rvec y, rvec x) {
-        return operator()(Problem::template make<P>(problem), y, x);
+    Stats operator()(const P &problem, rvec x, rvec y) {
+        return operator()(Problem::template make<P>(problem), x, y);
     }
 
     std::string get_name() const {
         return "ALMSolver<" + inner_solver.get_name() + ">";
     }
 
     /// Abort the computation and return the result so far.
@@ -176,14 +172,15 @@
 
   private:
     Params params;
     using Helpers = detail::ALMHelpers<config_t>;
 
   public:
     InnerSolver inner_solver;
+    std::ostream *os = &std::cout;
 };
 
 ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ALMParams, DefaultConfig);
 ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ALMParams, EigenConfigf);
 ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ALMParams, EigenConfigd);
 ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ALMParams, EigenConfigl);
 #ifdef ALPAQA_WITH_QUAD_PRECISION
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/outer/src/alm.tpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/outer/alm.tpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 #pragma once
 
-#include <alpaqa/inner/internal/solverstatus.hpp>
 #include <alpaqa/outer/alm.hpp>
-#include <alpaqa/outer/src/internal/alm-helpers.tpp>
 
 #include <algorithm>
 #include <iomanip>
 #include <iostream>
 #include <utility>
 
 #include <alpaqa/config/config.hpp>
+#include <alpaqa/implementation/outer/internal/alm-helpers.tpp>
+#include <alpaqa/implementation/util/print.tpp>
+#include <alpaqa/inner/inner-solve-options.hpp>
+#include <alpaqa/inner/internal/solverstatus.hpp>
 #include <alpaqa/util/quadmath/quadmath-print.hpp>
-#include <alpaqa/util/src/print.tpp>
 
 namespace alpaqa {
 
 template <class InnerSolverT>
 typename ALMSolver<InnerSolverT>::Stats
-ALMSolver<InnerSolverT>::operator()(const Problem &p, rvec y, rvec x) {
+ALMSolver<InnerSolverT>::operator()(const Problem &p, rvec x, rvec y) {
     using std::chrono::duration_cast;
     using std::chrono::nanoseconds;
     auto start_time = std::chrono::steady_clock::now();
 
     // Check the problem dimensions etc.
     p.check();
 
-    // Lagrange multipliers corresponding to penalty constraints are always 0.
-    auto &&y_penalty = y.topRows(params.penalty_alm_split);
-    y_penalty.setZero();
-
     auto m = p.get_m();
     if (m == 0) { // No general constraints, only box constraints
         Stats s;
         vec Σ(0), error(0);
-        auto ps = inner_solver(p, Σ, params.ε, true, x, y, error);
+        InnerSolveOptions<config_t> opts{
+            .always_overwrite_results = true,
+            .max_time                 = params.max_time,
+            .tolerance                = params.tolerance,
+            .os                       = os,
+            .check                    = false,
+        };
+        auto ps              = inner_solver(p, opts, x, y, Σ, error);
         bool inner_converged = ps.status == SolverStatus::Converged;
         auto time_elapsed    = std::chrono::steady_clock::now() - start_time;
         s.inner_convergence_failures = not inner_converged;
         s.inner += ps;
         s.ε                = ps.ε;
         s.δ                = 0;
         s.norm_penalty     = 0;
@@ -59,33 +63,33 @@
     auto print_real = [&](real_t x) {
         return float_to_str_vw(printbuf, x, params.print_precision);
     };
 
     Stats s;
 
     // Initialize the penalty weights
-    if (params.Σ_0 > 0) {
-        Σ.fill(params.Σ_0);
+    if (params.initial_penalty > 0) {
+        Σ.fill(params.initial_penalty);
     }
     // Initial penalty weights from problem
     else {
         Helpers::initialize_penalty(p, params, x, Σ);
     }
 
-    real_t ε                      = params.ε_0;
+    real_t ε                      = params.initial_tolerance;
     [[maybe_unused]] real_t ε_old = NaN;
-    real_t Δ                      = params.Δ;
-    real_t ρ                      = params.ρ;
+    real_t Δ                      = params.penalty_update_factor;
+    real_t ρ                      = params.tolerance_update_factor;
 
     unsigned num_successful_iters = 0;
 
-    for (unsigned int i = 0; i < params.max_iter; ++i) {
+    for (unsigned i = 0; i < params.max_iter; ++i) {
         // TODO: this is unnecessary when the previous iteration lowered the
         // penalty update factor.
-        p.eval_proj_multipliers(y, params.M, params.penalty_alm_split);
+        p.eval_proj_multipliers(y, params.max_multiplier);
         // Check if we're allowed to lower the penalty factor even further.
         bool out_of_penalty_factor_updates =
             (num_successful_iters == 0
                  ? s.initial_penalty_reduced == params.max_num_initial_retries
                  : s.penalty_reduced == params.max_num_retries) ||
             (s.initial_penalty_reduced + s.penalty_reduced ==
              params.max_total_num_retries);
@@ -94,44 +98,50 @@
         // penalty update factor, the inner solver can just return its results,
         // even if it doesn't converge.
         bool overwrite_results = out_of_iter || out_of_penalty_factor_updates;
 
         // Inner solver
         // ------------
 
+        auto time_elapsed = std::chrono::steady_clock::now() - start_time;
+        InnerSolveOptions<config_t> opts{
+            .always_overwrite_results = overwrite_results,
+            .max_time                 = params.max_time - time_elapsed,
+            .tolerance                = ε,
+            .os                       = os,
+            .outer_iter               = i,
+            .check                    = false,
+        };
         // Call the inner solver to minimize the augmented lagrangian for fixed
         // Lagrange multipliers y.
-        auto ps = inner_solver(p, Σ, ε, overwrite_results, x, y, error_2);
-        // Reset the Lagrange multipliers for the penalty constraints to 0 again.
-        y_penalty.setZero();
+        auto ps = inner_solver(p, opts, x, y, Σ, error_2);
         // Check if the inner solver converged
         bool inner_converged = ps.status == SolverStatus::Converged;
         // Accumulate the inner solver statistics
         s.inner_convergence_failures += not inner_converged;
         s.inner += ps;
 
-        auto time_elapsed = std::chrono::steady_clock::now() - start_time;
-        bool out_of_time  = time_elapsed > params.max_time;
+        time_elapsed     = std::chrono::steady_clock::now() - start_time;
+        bool out_of_time = time_elapsed > params.max_time;
         bool backtrack =
             not inner_converged && not overwrite_results && not out_of_time;
 
         // Print statistics of current iteration
         if (params.print_interval != 0 && i % params.print_interval == 0) {
-            real_t δ       = backtrack ? NaN : vec_util::norm_inf(error_2);
-            auto color     = inner_converged ? "\x1b[0;32m" : "\x1b[0;31m";
-            auto color_end = "\x1b[0m";
-            std::cout << "[\x1b[0;34mALM\x1b[0m]   " << std::setw(5) << i
-                      << ": ‖Σ‖ = " << print_real(Σ.norm())
-                      << ", ‖y‖ = " << print_real(y.norm())
-                      << ", δ = " << print_real(δ)
-                      << ", ε = " << print_real(ps.ε)
-                      << ", Δ = " << print_real(Δ) << ", status = " << color
-                      << std::setw(13) << ps.status << color_end
-                      << ", iter = " << std::setw(13) << ps.iterations
-                      << std::endl; // Flush for Python buffering
+            real_t δ          = backtrack ? NaN : vec_util::norm_inf(error_2);
+            const char *color = inner_converged ? "\x1b[0;32m" : "\x1b[0;31m";
+            const char *color_end = "\x1b[0m";
+            *os << "[\x1b[0;34mALM\x1b[0m]   " << std::setw(5) << i
+                << ": ‖Σ‖ = " << print_real(Σ.norm())
+                << ", ‖y‖ = " << print_real(y.norm())
+                << ", δ = " << print_real(δ) << ", ε = " << print_real(ps.ε)
+                << ", Δ = " << print_real(Δ) << ", status = " << color
+                << std::setw(13) << ps.status << color_end
+                << ", iter = " << std::setw(13) << ps.iterations
+                << std::endl; // Flush for Python buffering
         }
 
         // TODO: check penalty size?
         if (ps.status == SolverStatus::Interrupted) {
             s.ε                = ps.ε;
             s.δ                = vec_util::norm_inf(error_2);
             s.norm_penalty     = Σ.norm();
@@ -154,42 +164,43 @@
             // the previous successful iteration. error_1 contains the error of
             // the last successful iteration. (Unless, of course, there hasn't
             // been a successful iteration yet, which is covered by the second
             // branch of the following if statement.)
             if (num_successful_iters > 0) {
                 // We have a previous Σ and error
                 // Recompute penalty with smaller Δ
-                Δ = std::fmax(params.Δ_min, Δ * params.Δ_lower);
+                Δ = std::fmax(params.min_penalty_update_factor,
+                              Δ * params.penalty_update_factor_lower);
                 Helpers::update_penalty_weights(params, Δ, false, error_1,
                                                 error_2, norm_e_1, norm_e_2,
                                                 Σ_old, Σ, true);
                 // Recompute the primal tolerance with larger ρ
                 ρ = std::fmin(params.ρ_max, ρ * params.ρ_increase);
-                ε = std::fmax(ρ * ε_old, params.ε);
+                ε = std::fmax(ρ * ε_old, params.tolerance);
                 ++s.penalty_reduced;
             } else {
                 // We don't have a previous Σ, simply lower the current Σ and
                 // increase ε
-                Σ *= params.Σ_0_lower;
-                ε *= params.ε_0_increase;
+                Σ *= params.initial_penalty_lower;
+                ε *= params.initial_tolerance_increase;
                 ++s.initial_penalty_reduced;
             }
         }
 
         // If the inner solver did converge, increase penalty
         else {
             // After this line, error_1 contains the error of the current
             // (successful) iteration, and error_2 contains the error of the
             // previous successful iteration.
             error_2.swap(error_1);
             norm_e_2 = std::exchange(norm_e_1, vec_util::norm_inf(error_1));
 
             // Check the termination criteria
-            bool alm_converged =
-                ps.ε <= params.ε && inner_converged && norm_e_1 <= params.δ;
+            bool alm_converged = ps.ε <= params.tolerance && inner_converged &&
+                                 norm_e_1 <= params.dual_tolerance;
             bool exit = alm_converged || out_of_iter || out_of_time;
             if (exit) {
                 s.ε                = ps.ε;
                 s.δ                = norm_e_1;
                 s.norm_penalty     = Σ.norm();
                 s.outer_iterations = i + 1;
                 s.elapsed_time     = duration_cast<nanoseconds>(time_elapsed);
@@ -203,15 +214,15 @@
             // (successful) iteration.
             Σ_old.swap(Σ);
             // Update Σ to contain the penalty to use on the next iteration.
             Helpers::update_penalty_weights(
                 params, Δ, num_successful_iters == 0, error_1, error_2,
                 norm_e_1, norm_e_2, Σ_old, Σ, true);
             // Lower the primal tolerance for the inner solver.
-            ε_old = std::exchange(ε, std::fmax(ρ * ε, params.ε));
+            ε_old = std::exchange(ε, std::fmax(ρ * ε, params.tolerance));
             ++num_successful_iters;
         }
     }
     throw std::logic_error("[ALM]   loop error");
 }
 
 } // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/outer/src/internal/alm-helpers.tpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/implementation/outer/internal/alm-helpers.tpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,43 @@
 #pragma once
 
 #include <alpaqa/outer/alm.hpp>
+#if ALPAQA_WITH_OCP
+#include <alpaqa/problem/ocproblem.hpp>
+#endif
 
 #include <algorithm>
 
 namespace alpaqa::detail {
 
 template <Config Conf>
 struct ALMHelpers {
     USING_ALPAQA_CONFIG(Conf);
 
-    static void project_y(rvec y,                   // inout
-                          crvec z_lb,               // in
-                          crvec z_ub,               // in
-                          real_t M,                 // in
-                          index_t penalty_alm_split // in
-    ) {
-        // TODO: Handle NaN correctly
-        auto max_lb = [M](real_t y, real_t z_lb) {
-            real_t y_lb = z_lb == -inf<config_t> ? 0 : -M;
-            return std::max(y, y_lb);
-        };
-        auto min_ub = [M](real_t y, real_t z_ub) {
-            real_t y_ub = z_ub == inf<config_t> ? 0 : M;
-            return std::min(y, y_ub);
-        };
-        auto num_alm    = y.size() - penalty_alm_split;
-        auto &&y_alm    = y.bottomRows(num_alm);
-        auto &&z_alm_lb = z_lb.bottomRows(num_alm);
-        auto &&z_alm_ub = z_ub.bottomRows(num_alm);
-        y_alm = y_alm.binaryExpr(z_alm_lb, max_lb).binaryExpr(z_alm_ub, min_ub);
-    }
-
     static void update_penalty_weights(const ALMParams<config_t> &params,
                                        real_t Δ, bool first_iter, rvec e,
                                        rvec old_e, real_t norm_e,
                                        real_t old_norm_e, crvec Σ_old, rvec Σ,
                                        bool monotone) {
-        if (norm_e <= params.δ) {
+        const real_t θ = params.rel_penalty_increase_threshold;
+        if (norm_e <= params.dual_tolerance) {
             Σ = Σ_old;
             return;
         }
         if (params.single_penalty_factor) {
-            if (first_iter || norm_e > params.θ * old_norm_e) {
-                real_t new_Σ = std::fmin(params.Σ_max, Δ * Σ_old(0));
+            if (first_iter || norm_e > θ * old_norm_e) {
+                real_t new_Σ = std::fmin(params.max_penalty, Δ * Σ_old(0));
                 Σ.setConstant(new_Σ);
             } else {
                 Σ = Σ_old;
             }
         } else {
             for (index_t i = 0; i < e.rows(); ++i) {
-                if (first_iter ||
-                    std::abs(e(i)) > params.θ * std::abs(old_e(i))) {
-                    Σ(i) = std::fmin(params.Σ_max,
+                if (first_iter || std::abs(e(i)) > θ * std::abs(old_e(i))) {
+                    Σ(i) = std::fmin(params.max_penalty,
                                      std::fmax(Δ * std::abs(e(i)) / norm_e,
                                                real_t(1) * monotone) *
                                          Σ_old(i));
                 } else {
                     Σ(i) = Σ_old(i);
                 }
             }
@@ -66,16 +47,34 @@
     static void initialize_penalty(const TypeErasedProblem<config_t> &p,
                                    const ALMParams<config_t> &params, crvec x0,
                                    rvec Σ) {
         real_t f0 = p.eval_f(x0);
         vec g0(p.get_m());
         p.eval_g(x0, g0);
         // TODO: reuse evaluations of f ang g in PANOC?
-        real_t σ = params.σ_0 * std::max(real_t(1), std::abs(f0)) /
+        real_t σ = params.initial_penalty_factor *
+                   std::max(real_t(1), std::abs(f0)) /
                    std::max(real_t(1), real_t(0.5) * g0.squaredNorm());
-        σ = std::max(σ, params.Σ_min);
-        σ = std::min(σ, params.Σ_max);
+        σ = std::clamp(σ, params.min_penalty, params.max_penalty);
+        Σ.fill(σ);
+    }
+
+#if ALPAQA_WITH_OCP
+    static void initialize_penalty(
+        [[maybe_unused]] const TypeErasedControlProblem<config_t> &p,
+        const ALMParams<config_t> &params, [[maybe_unused]] crvec x0, rvec Σ) {
+        real_t σ = 1;
+        σ        = std::clamp(σ, params.min_penalty, params.max_penalty);
         Σ.fill(σ);
     }
+#endif
 };
 
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ALMHelpers, DefaultConfig);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ALMHelpers, EigenConfigf);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ALMHelpers, EigenConfigd);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ALMHelpers, EigenConfigl);
+#ifdef ALPAQA_WITH_QUAD_PRECISION
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ALMHelpers, EigenConfigq);
+#endif
+
 } // namespace alpaqa::detail
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/panoc-alm.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/structured-panoc-alm.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #pragma once
 
-#include <alpaqa/inner/directions/panoc/lbfgs.hpp>
+#include <alpaqa/inner/directions/panoc/structured-lbfgs.hpp>
 #include <alpaqa/inner/panoc.hpp>
 #include <alpaqa/outer/alm.hpp>
 
 namespace alpaqa {
 
 // clang-format off
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, PANOCSolver, LBFGS<DefaultConfig>);
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, PANOCSolver, LBFGS<EigenConfigf>);
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, PANOCSolver, LBFGS<EigenConfigd>);
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, PANOCSolver, LBFGS<EigenConfigl>);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(class, PANOCSolver, StructuredLBFGSDirection<DefaultConfig>);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(class, PANOCSolver, StructuredLBFGSDirection<EigenConfigf>);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(class, PANOCSolver, StructuredLBFGSDirection<EigenConfigd>);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(class, PANOCSolver, StructuredLBFGSDirection<EigenConfigl>);
 #ifdef ALPAQA_WITH_QUAD_PRECISION
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, PANOCSolver, LBFGS<EigenConfigq>);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(class, PANOCSolver, StructuredLBFGSDirection<EigenConfigq>);
 #endif
 
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGS<DefaultConfig>>);
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGS<EigenConfigf>>);
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGS<EigenConfigd>>);
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGS<EigenConfigl>>);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGSDirection<DefaultConfig>>);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGSDirection<EigenConfigf>>);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGSDirection<EigenConfigd>>);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGSDirection<EigenConfigl>>);
 #ifdef ALPAQA_WITH_QUAD_PRECISION
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGS<EigenConfigq>>);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGSDirection<EigenConfigq>>);
 #endif
+// clang-format on
 
 } // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/problem/box.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/box.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -5,16 +5,32 @@
 
 namespace alpaqa {
 
 template <Config Conf = DefaultConfig>
 struct Box {
     USING_ALPAQA_CONFIG(Conf);
 
-    vec upperbound;
+    Box() : Box{0} {}
+    Box(length_t n)
+        : lowerbound{vec::Constant(n, -inf<config_t>)}, upperbound{
+                                                            vec::Constant(n, +inf<config_t>)} {}
+
+    static Box NaN(length_t n) {
+        return Box{vec::Constant(n, alpaqa::NaN<config_t>),
+                   vec::Constant(n, alpaqa::NaN<config_t>)};
+    }
+    static Box from_lower_upper(vec lower, vec upper) {
+        return Box{std::move(lower), std::move(upper)};
+    }
+
     vec lowerbound;
+    vec upperbound;
+
+  private:
+    Box(vec lower, vec upper) : lowerbound{std::move(lower)}, upperbound{std::move(upper)} {}
 };
 
 /// Project a vector onto a box.
 /// @f[ \Pi_C(v) @f]
 template <Config Conf>
 inline auto project(const auto &v,       ///< [in] The vector to project
                     const Box<Conf> &box ///< [in] The box to project onto
@@ -25,15 +41,15 @@
         .binaryExpr(box.upperbound, binary_real_f(std::fmin));
 }
 
 /// Get the difference between the given vector and its projection.
 /// @f[ v - \Pi_C(v) @f]
 /// @warning    Beware catastrophic cancellation!
 template <Config Conf>
-inline auto
+inline auto                                //
 projecting_difference(const auto &v,       ///< [in] The vector to project
                       const Box<Conf> &box ///< [in] The box to project onto
 ) {
     return v - project(v, box);
 }
 
 /// Get the distance squared between the given vector and its projection.
@@ -51,16 +67,16 @@
 /// Σ norm.
 /// @f[ \left\| v - \Pi_C(v) \right\|_\Sigma^2
 /// = \left(v - \Pi_C(v)\right)^\top \Sigma \left(v - \Pi_C(v)\right) @f]
 /// @warning    Beware catastrophic cancellation!
 template <Config Conf>
 inline auto dist_squared(const auto &v,        ///< [in] The vector to project
                          const Box<Conf> &box, ///< [in] The box to project onto
-                         const auto &Σ ///< [in] Diagonal matrix defining norm
-) {
+                         const auto &Σ         ///< [in] Diagonal matrix defining norm
+                         ) -> real_t<Conf> {
     // TODO: Does this allocate?
     //       Does it have dangling references to temporaries?
     auto d = v - project(v, box);
     return d.dot(Σ.asDiagonal() * d);
 }
 
 } // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/problem/type-erased-problem.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/problem/type-erased-problem.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,309 +1,228 @@
 #pragma once
 
 #include <alpaqa/config/config.hpp>
+#include <alpaqa/export.hpp>
 #include <alpaqa/problem/box.hpp>
-#include <alpaqa/problem/problem-counters.hpp>
 #include <alpaqa/util/alloc-check.hpp>
 #include <alpaqa/util/check-dim.hpp>
 #include <alpaqa/util/not-implemented.hpp>
+#include <alpaqa/util/required-method.hpp>
 #include <alpaqa/util/type-erasure.hpp>
 #include <chrono>
 #include <stdexcept>
 #include <type_traits>
+#include <utility>
 
 namespace alpaqa {
 
-#define ALPAQA_TE_REQUIRED_METHOD(vtable, type, member)                                            \
-    vtable.member = util::type_erased_wrapped<&type::member>()
-#define ALPAQA_TE_OPTIONAL_METHOD(vtable, type, member)                                            \
-    if constexpr (requires { &type::member; })                                                     \
-    vtable.member =                                                                                \
-        util::type_erased_wrapped<&type::member, const std::remove_cvref_t<decltype(vtable)> &>()
-#define ALPAQA_TE_DISABLED_METHOD(vtable, member, instance_p)                                      \
-    if constexpr (requires { (instance_p)->provides_##member(); })                                 \
-        if (!(instance_p)->provides_##member())                                                    \
-    vtable.member = nullptr
-#define ALPAQA_TE_DEFAULT_METHOD(vtable, member, default_)                                         \
-    if (vtable.member == nullptr)                                                                  \
-    vtable.member = default_
-
+/// Struct containing function pointers to all problem functions (like the
+/// objective and constraint functions, with their derivatives, and more).
+/// Some default implementations are available.
+/// Internal struct, it is used by @ref TypeErasedProblem.
 template <Config Conf>
 struct ProblemVTable : util::BasicVTable {
     USING_ALPAQA_CONFIG(Conf);
     using Box = alpaqa::Box<config_t>;
 
     template <class F>
     using optional_function_t = util::BasicVTable::optional_function_t<F, ProblemVTable>;
     template <class F>
     using optional_const_function_t =
         util::BasicVTable::optional_const_function_t<F, ProblemVTable>;
 
     // clang-format off
 
     // Required
-    required_const_function_t<void(crvec z, rvec p)>
+    required_const_function_t<void(crvec z, rvec e)>
         eval_proj_diff_g;
-    required_const_function_t<void(rvec y, real_t M, index_t penalty_alm_split)>
+    required_const_function_t<void(rvec y, real_t M)>
         eval_proj_multipliers;
-    required_const_function_t<void(real_t γ, crvec x, crvec grad_ψ, rvec x̂, rvec p)>
+    required_const_function_t<real_t(real_t γ, crvec x, crvec grad_ψ, rvec x̂, rvec p)>
         eval_prox_grad_step;
     required_const_function_t<real_t(crvec x)>
         eval_f;
     required_const_function_t<void(crvec x, rvec grad_fx)>
         eval_grad_f;
     required_const_function_t<void(crvec x, rvec gx)>
         eval_g;
     required_const_function_t<void(crvec x, crvec y, rvec grad_gxy)>
         eval_grad_g_prod;
+    optional_const_function_t<index_t(real_t γ, crvec x, crvec grad_ψ, rindexvec J)>
+        eval_inactive_indices_res_lna = default_eval_inactive_indices_res_lna;
 
     // Second order
+    optional_const_function_t<void(crvec x, rindexvec inner_idx, rindexvec outer_ptr, rvec J_values)>
+        eval_jac_g = default_eval_jac_g;
+    optional_const_function_t<length_t()>
+        get_jac_g_num_nonzeros = default_get_jac_g_num_nonzeros;
     optional_const_function_t<void(crvec x, index_t i, rvec grad_gi)>
-        eval_grad_gi = nullptr;
-    optional_const_function_t<void(crvec x, crvec y, crvec v, rvec Hv)>
-        eval_hess_L_prod = nullptr;
-    optional_const_function_t<void(crvec x, crvec y, rmat H)>
-        eval_hess_L = nullptr;
+        eval_grad_gi = default_eval_grad_gi;
+    optional_const_function_t<void(crvec x, crvec y, real_t scale, crvec v, rvec Hv)>
+        eval_hess_L_prod = default_eval_hess_L_prod;
+    optional_const_function_t<void(crvec x, crvec y, real_t scale, rindexvec inner_idx, rindexvec outer_ptr, rvec H_values)>
+        eval_hess_L = default_eval_hess_L;
+    optional_const_function_t<length_t()>
+        get_hess_L_num_nonzeros = default_get_hess_L_num_nonzeros;
+    optional_const_function_t<void(crvec x, crvec y, crvec Σ, real_t scale, crvec v, rvec Hv)>
+        eval_hess_ψ_prod = default_eval_hess_ψ_prod;
+    optional_const_function_t<void(crvec x, crvec y, crvec Σ, real_t scale, rindexvec inner_idx, rindexvec outer_ptr, rvec H_values)>
+        eval_hess_ψ = default_eval_hess_ψ;
+    optional_const_function_t<length_t()>
+        get_hess_ψ_num_nonzeros = default_get_hess_ψ_num_nonzeros;
 
     // Combined evaluations
     optional_const_function_t<real_t(crvec x, rvec grad_fx)>
-        eval_f_grad_f = nullptr;
+        eval_f_grad_f = default_eval_f_grad_f;
     optional_const_function_t<real_t(crvec x, rvec g)>
-        eval_f_g = nullptr;
-    optional_const_function_t<real_t(crvec x, rvec grad_fx, rvec g)>
-        eval_f_grad_f_g = nullptr;
+        eval_f_g = default_eval_f_g;
     optional_const_function_t<void(crvec x, crvec y, rvec grad_f, rvec grad_gxy)>
-        eval_grad_f_grad_g_prod = nullptr;
+        eval_grad_f_grad_g_prod = default_eval_grad_f_grad_g_prod;
 
     // Lagrangian and augmented lagrangian evaluations
     optional_const_function_t<void(crvec x, crvec y, rvec grad_L, rvec work_n)>
-        eval_grad_L = nullptr;
+        eval_grad_L = default_eval_grad_L;
     optional_const_function_t<real_t(crvec x, crvec y, crvec Σ, rvec ŷ)>
-        eval_ψ = nullptr;
-    optional_const_function_t<void(crvec x, crvec ŷ, rvec grad_ψ, rvec work_n)>
-        eval_grad_ψ_from_ŷ = nullptr;
+        eval_ψ = default_eval_ψ;
     optional_const_function_t<void(crvec x, crvec y, crvec Σ, rvec grad_ψ, rvec work_n, rvec work_m)>
-        eval_grad_ψ = nullptr;
+        eval_grad_ψ = default_eval_grad_ψ;
     optional_const_function_t<real_t(crvec x, crvec y, crvec Σ, rvec grad_ψ, rvec work_n, rvec work_m)>
-        eval_ψ_grad_ψ = nullptr;
+        eval_ψ_grad_ψ = default_eval_ψ_grad_ψ;
 
     // Constraint sets
     optional_const_function_t<const Box &()>
-        get_box_C = nullptr;
+        get_box_C = default_get_box_C;
     optional_const_function_t<const Box &()>
-        get_box_D = nullptr;
+        get_box_D = default_get_box_D;
 
     // Check
-    required_const_function_t<void()>
-        check;
+    optional_const_function_t<void()>
+        check = default_check;
 
     // clang-format on
 
-    length_t n, m;
+    ALPAQA_EXPORT static real_t calc_ŷ_dᵀŷ(const void *self, rvec g_ŷ, crvec y, crvec Σ,
+                                           const ProblemVTable &vtable);
+    ALPAQA_EXPORT static index_t default_eval_inactive_indices_res_lna(const void *, real_t, crvec,
+                                                                       crvec, rindexvec,
+                                                                       const ProblemVTable &);
+    ALPAQA_EXPORT static void default_eval_jac_g(const void *, crvec, rindexvec, rindexvec, rvec,
+                                                 const ProblemVTable &);
+    ALPAQA_EXPORT static length_t default_get_jac_g_num_nonzeros(const void *,
+                                                                 const ProblemVTable &);
+    ALPAQA_EXPORT static void default_eval_grad_gi(const void *, crvec, index_t, rvec,
+                                                   const ProblemVTable &);
+    ALPAQA_EXPORT static void default_eval_hess_L_prod(const void *, crvec, crvec, real_t, crvec,
+                                                       rvec, const ProblemVTable &);
+    ALPAQA_EXPORT static void default_eval_hess_L(const void *, crvec, crvec, real_t, rindexvec,
+                                                  rindexvec, rvec, const ProblemVTable &);
+    ALPAQA_EXPORT static length_t default_get_hess_L_num_nonzeros(const void *,
+                                                                  const ProblemVTable &);
+    ALPAQA_EXPORT static void default_eval_hess_ψ_prod(const void *self, crvec x, crvec y, crvec,
+                                                       real_t scale, crvec v, rvec Hv,
+                                                       const ProblemVTable &vtable);
+    ALPAQA_EXPORT static void default_eval_hess_ψ(const void *self, crvec x, crvec y, crvec,
+                                                  real_t scale, rindexvec inner_idx,
+                                                  rindexvec outer_ptr, rvec H_values,
+                                                  const ProblemVTable &vtable);
+    ALPAQA_EXPORT static length_t default_get_hess_ψ_num_nonzeros(const void *,
+                                                                  const ProblemVTable &);
+    ALPAQA_EXPORT static real_t default_eval_f_grad_f(const void *self, crvec x, rvec grad_fx,
+                                                      const ProblemVTable &vtable);
+    ALPAQA_EXPORT static real_t default_eval_f_g(const void *self, crvec x, rvec g,
+                                                 const ProblemVTable &vtable);
+    ALPAQA_EXPORT static void default_eval_grad_f_grad_g_prod(const void *self, crvec x, crvec y,
+                                                              rvec grad_f, rvec grad_gxy,
+                                                              const ProblemVTable &vtable);
+    ALPAQA_EXPORT static void default_eval_grad_L(const void *self, crvec x, crvec y, rvec grad_L,
+                                                  rvec work_n, const ProblemVTable &vtable);
+    ALPAQA_EXPORT static real_t default_eval_ψ(const void *self, crvec x, crvec y, crvec Σ, rvec ŷ,
+                                               const ProblemVTable &vtable);
+    ALPAQA_EXPORT static void default_eval_grad_ψ(const void *self, crvec x, crvec y, crvec Σ,
+                                                  rvec grad_ψ, rvec work_n, rvec work_m,
+                                                  const ProblemVTable &vtable);
+    ALPAQA_EXPORT static real_t default_eval_ψ_grad_ψ(const void *self, crvec x, crvec y, crvec Σ,
+                                                      rvec grad_ψ, rvec work_n, rvec work_m,
+                                                      const ProblemVTable &vtable);
+    ALPAQA_EXPORT static const Box &default_get_box_C(const void *, const ProblemVTable &);
+    ALPAQA_EXPORT static const Box &default_get_box_D(const void *, const ProblemVTable &);
+    ALPAQA_EXPORT static void default_check(const void *, const ProblemVTable &);
 
-    static real_t calc_ŷ_dᵀŷ(const void *self, rvec g_ŷ, crvec y, crvec Σ,
-                             const ProblemVTable &vtable) {
-        if (Σ.size() == 1) {
-            // ζ = g(x) + Σ⁻¹y
-            g_ŷ += (1 / Σ(0)) * y;
-            // d = ζ - Π(ζ, D)
-            vtable.eval_proj_diff_g(self, g_ŷ, g_ŷ);
-            // dᵀŷ, ŷ = Σ d
-            real_t dᵀŷ = Σ(0) * g_ŷ.dot(g_ŷ);
-            g_ŷ *= Σ(0);
-            return dᵀŷ;
-        } else {
-            // ζ = g(x) + Σ⁻¹y
-            g_ŷ += Σ.asDiagonal().inverse() * y;
-            // d = ζ - Π(ζ, D)
-            vtable.eval_proj_diff_g(self, g_ŷ, g_ŷ);
-            // dᵀŷ, ŷ = Σ d
-            real_t dᵀŷ = 0;
-            for (index_t i = 0; i < y.size(); ++i) {
-                dᵀŷ += g_ŷ(i) * Σ(i) * g_ŷ(i); // TODO: vectorize
-                g_ŷ(i) = Σ(i) * g_ŷ(i);
-            }
-            return dᵀŷ;
-        }
-    }
-
-    static void default_eval_grad_gi(const void *, crvec, index_t, rvec, const ProblemVTable &) {
-        throw not_implemented_error("eval_grad_gi");
-    }
-    static void default_eval_hess_L_prod(const void *, crvec, crvec, crvec, rvec,
-                                         const ProblemVTable &) {
-        throw not_implemented_error("eval_hess_L_prod");
-    }
-    static void default_eval_hess_L(const void *, crvec, crvec, rmat, const ProblemVTable &) {
-        throw not_implemented_error("eval_hess_L");
-    }
-
-    static real_t default_eval_f_grad_f(const void *self, crvec x, rvec grad_fx,
-                                        const ProblemVTable &vtable) {
-        vtable.eval_grad_f(self, x, grad_fx);
-        return vtable.eval_f(self, x);
-    }
-    static real_t default_eval_f_g(const void *self, crvec x, rvec g, const ProblemVTable &vtable) {
-        vtable.eval_g(self, x, g);
-        return vtable.eval_f(self, x);
-    }
-    static real_t default_eval_f_grad_f_g(const void *self, crvec x, rvec grad_fx, rvec g,
-                                          const ProblemVTable &vtable) {
-        vtable.eval_g(self, x, g);
-        return vtable.eval_f_grad_f(self, x, grad_fx, vtable);
-    }
-    static void default_eval_grad_f_grad_g_prod(const void *self, crvec x, crvec y, rvec grad_f,
-                                                rvec grad_gxy, const ProblemVTable &vtable) {
-        vtable.eval_grad_f(self, x, grad_f);
-        vtable.eval_grad_g_prod(self, x, y, grad_gxy);
-    }
-    static void default_eval_grad_L(const void *self, crvec x, crvec y, rvec grad_L, rvec work_n,
-                                    const ProblemVTable &vtable) {
-        vtable.eval_grad_f_grad_g_prod(self, x, y, grad_L, work_n, vtable);
-        grad_L += work_n;
-    }
-    static real_t default_eval_ψ(const void *self, crvec x, crvec y, crvec Σ, rvec ŷ,
-                                 const ProblemVTable &vtable) {
-        if (y.size() == 0) /* [[unlikely]] */
-            return vtable.eval_f(self, x);
-
-        real_t f   = vtable.eval_f_g(self, x, ŷ, vtable);
-        real_t dᵀŷ = calc_ŷ_dᵀŷ(self, ŷ, y, Σ, vtable);
-        // ψ(x) = f(x) + ½ dᵀŷ
-        real_t ψ = f + real_t(0.5) * dᵀŷ;
-        return ψ;
-    }
-    static void default_eval_grad_ψ_from_ŷ(const void *self, crvec x, crvec ŷ, rvec grad_ψ,
-                                           rvec work_n, const ProblemVTable &vtable) {
-        if (ŷ.size() == 0) /* [[unlikely]] */
-            vtable.eval_grad_f(self, x, grad_ψ);
-        else
-            vtable.eval_grad_L(self, x, ŷ, grad_ψ, work_n, vtable);
-    }
-    static void default_eval_grad_ψ(const void *self, crvec x, crvec y, crvec Σ, rvec grad_ψ,
-                                    rvec work_n, rvec work_m, const ProblemVTable &vtable) {
-        if (y.size() == 0) /* [[unlikely]] */ {
-            vtable.eval_grad_f(self, x, grad_ψ);
-        } else {
-            vtable.eval_g(self, x, work_m);
-            (void)calc_ŷ_dᵀŷ(self, work_m, y, Σ, vtable);
-            vtable.eval_grad_ψ_from_ŷ(self, x, work_m, grad_ψ, work_n, vtable);
-        }
-    }
-    static real_t default_eval_ψ_grad_ψ(const void *self, crvec x, crvec y, crvec Σ, rvec grad_ψ,
-                                        rvec work_n, rvec work_m, const ProblemVTable &vtable) {
-        if (y.size() == 0) /* [[unlikely]] */
-            return vtable.eval_f_grad_f(self, x, grad_ψ, vtable);
-
-        auto &ŷ = work_m;
-        // ψ(x) = f(x) + ½ dᵀŷ
-        real_t f   = vtable.eval_f_g(self, x, ŷ, vtable);
-        real_t dᵀŷ = calc_ŷ_dᵀŷ(self, ŷ, y, Σ, vtable);
-        real_t ψ   = f + real_t(0.5) * dᵀŷ;
-        // ∇ψ(x) = ∇f(x) + ∇g(x) ŷ
-        vtable.eval_grad_L(self, x, ŷ, grad_ψ, work_n, vtable);
-        return ψ;
-    }
-    static const Box &default_get_box_C(const void *, const ProblemVTable &) {
-        throw not_implemented_error("get_box_C");
-    }
-    static const Box &default_get_box_D(const void *, const ProblemVTable &) {
-        throw not_implemented_error("get_box_D");
-    }
+    length_t n, m;
 
     template <class P>
-    ProblemVTable(util::VTableTypeTag<P> t) : util::BasicVTable{t} {
+    ProblemVTable(std::in_place_t, P &p) : util::BasicVTable{std::in_place, p} {
         auto &vtable = *this;
-        assert(t.t);
 
         // Initialize all methods
 
         // Required
         ALPAQA_TE_REQUIRED_METHOD(vtable, P, eval_proj_diff_g);
         ALPAQA_TE_REQUIRED_METHOD(vtable, P, eval_proj_multipliers);
         ALPAQA_TE_REQUIRED_METHOD(vtable, P, eval_prox_grad_step);
         ALPAQA_TE_REQUIRED_METHOD(vtable, P, eval_f);
         ALPAQA_TE_REQUIRED_METHOD(vtable, P, eval_grad_f);
         ALPAQA_TE_REQUIRED_METHOD(vtable, P, eval_g);
         ALPAQA_TE_REQUIRED_METHOD(vtable, P, eval_grad_g_prod);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_inactive_indices_res_lna, p);
         // Second order
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_grad_gi);
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_hess_L_prod);
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_hess_L);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_jac_g, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, get_jac_g_num_nonzeros, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_grad_gi, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_hess_L_prod, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_hess_L, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, get_hess_L_num_nonzeros, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_hess_ψ_prod, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_hess_ψ, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, get_hess_ψ_num_nonzeros, p);
         // Combined evaluations
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_f_grad_f);
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_f_g);
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_f_grad_f_g);
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_grad_f_grad_g_prod);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_f_grad_f, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_f_g, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_grad_f_grad_g_prod, p);
         // Lagrangian and augmented lagrangian evaluations
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_grad_L);
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_ψ);
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_grad_ψ_from_ŷ);
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_grad_ψ);
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_ψ_grad_ψ);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_grad_L, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_ψ, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_grad_ψ, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, eval_ψ_grad_ψ, p);
         // Constraint set
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, get_box_C);
-        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, get_box_D);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, get_box_C, p);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, get_box_D, p);
         // Check
-        ALPAQA_TE_REQUIRED_METHOD(vtable, P, check);
-
-        // Disable optional methods
-
-        // Second order
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_grad_gi, t.t);
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_hess_L_prod, t.t);
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_hess_L, t.t);
-        // Combined evaluations
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_f_grad_f, t.t);
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_f_g, t.t);
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_f_grad_f_g, t.t);
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_grad_f_grad_g_prod, t.t);
-        // Lagrangian and augmented lagrangian evaluations
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_grad_L, t.t);
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_ψ, t.t);
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_grad_ψ_from_ŷ, t.t);
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_grad_ψ, t.t);
-        ALPAQA_TE_DISABLED_METHOD(vtable, eval_ψ_grad_ψ, t.t);
-        // Constraint sets
-        ALPAQA_TE_DISABLED_METHOD(vtable, P, get_box_C);
-        ALPAQA_TE_DISABLED_METHOD(vtable, P, get_box_D);
-
-        // Provide defaults
-
-        // Second order
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_grad_gi, default_eval_grad_gi);
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_hess_L_prod, default_eval_hess_L_prod);
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_hess_L, default_eval_hess_L);
-        // Combined evaluations
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_f_grad_f, default_eval_f_grad_f);
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_f_g, default_eval_f_g);
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_f_grad_f_g, default_eval_f_grad_f_g);
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_grad_f_grad_g_prod, default_eval_grad_f_grad_g_prod);
-        // Lagrangian and augmented lagrangian evaluations
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_grad_L, default_eval_grad_L);
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_ψ, default_eval_ψ);
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_grad_ψ_from_ŷ, default_eval_grad_ψ_from_ŷ);
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_grad_ψ, default_eval_grad_ψ);
-        ALPAQA_TE_DEFAULT_METHOD(vtable, eval_ψ_grad_ψ, default_eval_ψ_grad_ψ);
-        // Constraint sets
-        ALPAQA_TE_DEFAULT_METHOD(vtable, get_box_C, default_get_box_C);
-        ALPAQA_TE_DEFAULT_METHOD(vtable, get_box_D, default_get_box_D);
+        ALPAQA_TE_OPTIONAL_METHOD(vtable, P, check, p);
 
         // Dimensions
-        vtable.n = t.t->get_n();
-        vtable.m = t.t->get_m();
+        vtable.n = p.get_n();
+        vtable.m = p.get_m();
     }
     ProblemVTable() = default;
 };
 
-#undef ALPAQA_TE_OPTIONAL_METHOD
-#undef ALPAQA_TE_REQUIRED_METHOD
-#undef ALPAQA_TE_DISABLED_METHOD
-#undef ALPAQA_TE_DEFAULT_METHOD
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ProblemVTable, DefaultConfig);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ProblemVTable, EigenConfigf);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ProblemVTable, EigenConfigd);
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ProblemVTable, EigenConfigl);
+#ifdef ALPAQA_WITH_QUAD_PRECISION
+ALPAQA_EXPORT_EXTERN_TEMPLATE(struct, ProblemVTable, EigenConfigq);
+#endif
+
+/// @addtogroup grp_Problems
+/// @{
 
+/// The main polymorphic minimization problem interface.
+///
+/// This class wraps the actual problem implementation class, filling in the
+/// missing member functions with sensible defaults, and providing a uniform
+/// interface that is used by the solvers.
+///
+/// The problem implementations do not inherit from an abstract base class.
+/// Instead, [structural typing](https://en.wikipedia.org/wiki/Structural_type_system)
+/// is used. The @ref ProblemVTable constructor uses reflection to discover
+/// which member functions are provided by the problem implementation. See
+/// @ref page_problem_formulations for more information, and
+/// @ref C++/CustomCppProblem/main.cpp for an example.
 template <Config Conf = DefaultConfig, class Allocator = std::allocator<std::byte>>
 class TypeErasedProblem : public util::TypeErased<ProblemVTable<Conf>, Allocator> {
   public:
     USING_ALPAQA_CONFIG(Conf);
     using Box            = alpaqa::Box<config_t>;
     using VTable         = ProblemVTable<config_t>;
     using allocator_type = Allocator;
@@ -320,291 +239,469 @@
     static TypeErasedProblem make(Args &&...args) {
         return TypeErased::template make<TypeErasedProblem, T>(std::forward<Args>(args)...);
     }
 
     /// @name Problem dimensions
     /// @{
 
+    /// **[Required]**
     /// Number of decision variables.
     length_t get_n() const;
+    /// **[Required]**
     /// Number of constraints.
     length_t get_m() const;
 
     /// @}
 
-    /// @name Basic functions
+    /// @name Required cost and constraint functions
     /// @{
 
-    /// Function that evaluates the difference between the given point @f$ z @f$
-    /// and its projection onto the constraint set @f$ D @f$.
-    /// @param  [in] z
-    ///         Slack variable, @f$ z \in \R^m @f$
-    /// @param  [out] p
-    ///         The difference relative to its projection,
-    ///         @f$ p = z - \Pi_D(z) \in \R^m @f$
-    /// @note   @p z and @p p can refer to the same vector.
-    void eval_proj_diff_g(crvec z, rvec p) const;
-    /// Function that projects the Lagrange multipliers for ALM.
-    /// @param  [inout] y
-    ///         Multipliers, @f$ y \leftarrow \Pi_Y(y) \in \R^m @f$
-    /// @param  [in] M
-    ///         The radius/size of the set @f$ Y @f$. See @ref ALMParams::M.
-    /// @param  [in] penalty_alm_split
-    ///         See @ref ALMParams::penalty_alm_split.
-    void eval_proj_multipliers(rvec y, real_t M, index_t penalty_alm_split) const;
-    /// Function that evaluates a proximal gradient step.
-    /// @param  [in] γ
-    ///         Step size, @f$ \gamma \in \R_{>0} @f$
-    /// @param  [in] x
-    ///         Decision variable @f$ x \in \R^n @f$
-    /// @param  [in] grad_ψ
-    ///         Gradient of the subproblem cost, @f$ \nabla\psi(x) \in \R^n @f$
-    /// @param  [out] x̂
-    ///         Next proximal gradient iterate, @f$ \hat x = T_\gamma(x) =
-    ///         \prox_{\gamma h}(x - \gamma\nabla\psi(x)) \in \R^n @f$
-    /// @param  [out] p
-    ///         The proximal gradient step,
-    ///         @f$ p = \hat x - x \in \R^n @f$
-    /// @note   The vector @f$ p @f$ is often used in stopping criteria, so its
-    ///         numerical accuracy is more important than that of @f$ \hat x @f$.
-    void eval_prox_grad_step(real_t γ, crvec x, crvec grad_ψ, rvec x̂, rvec p) const;
-
+    /// **[Required]**
     /// Function that evaluates the cost, @f$ f(x) @f$
     /// @param  [in] x
     ///         Decision variable @f$ x \in \R^n @f$
     real_t eval_f(crvec x) const;
+    /// **[Required]**
     /// Function that evaluates the gradient of the cost, @f$ \nabla f(x) @f$
     /// @param  [in] x
     ///         Decision variable @f$ x \in \R^n @f$
     /// @param  [out] grad_fx
     ///         Gradient of cost function @f$ \nabla f(x) \in \R^n @f$
     void eval_grad_f(crvec x, rvec grad_fx) const;
+    /// **[Required]**
     /// Function that evaluates the constraints, @f$ g(x) @f$
     /// @param  [in] x
     ///         Decision variable @f$ x \in \R^n @f$
     /// @param  [out] gx
     ///         Value of the constraints @f$ g(x) \in \R^m @f$
     void eval_g(crvec x, rvec gx) const;
+    /// **[Required]**
     /// Function that evaluates the gradient of the constraints times a vector,
-    /// @f$ \nabla g(x)\,y @f$
+    /// @f$ \nabla g(x)\,y = \tp{\jac_g(x)}y @f$
     /// @param  [in] x
     ///         Decision variable @f$ x \in \R^n @f$
     /// @param  [in] y
     ///         Vector @f$ y \in \R^m @f$ to multiply the gradient by
     /// @param  [out] grad_gxy
     ///         Gradient of the constraints
     ///         @f$ \nabla g(x)\,y \in \R^n @f$
     void eval_grad_g_prod(crvec x, crvec y, rvec grad_gxy) const;
 
     /// @}
 
+    /// @name Projections onto constraint sets and proximal mappings
+    /// @{
+
+    /// **[Required]**
+    /// Function that evaluates the difference between the given point @f$ z @f$
+    /// and its projection onto the constraint set @f$ D @f$.
+    /// @param  [in] z
+    ///         Slack variable, @f$ z \in \R^m @f$
+    /// @param  [out] e
+    ///         The difference relative to its projection,
+    ///         @f$ e = z - \Pi_D(z) \in \R^m @f$
+    /// @note   @p z and @p e can refer to the same vector.
+    void eval_proj_diff_g(crvec z, rvec e) const;
+    /// **[Required]**
+    /// Function that projects the Lagrange multipliers for ALM.
+    /// @param  [inout] y
+    ///         Multipliers, @f$ y \leftarrow \Pi_Y(y) \in \R^m @f$
+    /// @param  [in] M
+    ///         The radius/size of the set @f$ Y @f$.
+    ///         See @ref ALMParams::max_multiplier.
+    void eval_proj_multipliers(rvec y, real_t M) const;
+    /// **[Required]**
+    /// Function that computes a proximal gradient step.
+    /// @param  [in] γ
+    ///         Step size, @f$ \gamma \in \R_{>0} @f$
+    /// @param  [in] x
+    ///         Decision variable @f$ x \in \R^n @f$
+    /// @param  [in] grad_ψ
+    ///         Gradient of the subproblem cost, @f$ \nabla\psi(x) \in \R^n @f$
+    /// @param  [out] x̂
+    ///         Next proximal gradient iterate, @f$ \hat x = T_\gamma(x) =
+    ///         \prox_{\gamma h}(x - \gamma\nabla\psi(x)) \in \R^n @f$
+    /// @param  [out] p
+    ///         The proximal gradient step,
+    ///         @f$ p = \hat x - x \in \R^n @f$
+    /// @return The nonsmooth function evaluated at x̂,
+    ///         @f$ h(\hat x) @f$.
+    /// @note   The vector @f$ p @f$ is often used in stopping criteria, so its
+    ///         numerical accuracy is more important than that of @f$ \hat x @f$.
+    real_t eval_prox_grad_step(real_t γ, crvec x, crvec grad_ψ, rvec x̂, rvec p) const;
+    /// **[Optional]**
+    /// Function that computes the inactive indices @f$ \mathcal J(x) @f$ for
+    /// the evaluation of the linear Newton approximation of the residual, as in
+    /// @cite pas2022alpaqa.
+    /// @param  [in] γ
+    ///         Step size, @f$ \gamma \in \R_{>0} @f$
+    /// @param  [in] x
+    ///         Decision variable @f$ x \in \R^n @f$
+    /// @param  [in] grad_ψ
+    ///         Gradient of the subproblem cost, @f$ \nabla\psi(x) \in \R^n @f$
+    /// @param  [out] J
+    ///         The indices of the components of @f$ x @f$ that are in the
+    ///         index set @f$ \mathcal J(x) @f$. In ascending order, at most n.
+    /// @return The number of inactive constraints, @f$ \# \mathcal J(x) @f$.
+    ///
+    /// For example, in the case of box constraints, we have
+    /// @f[ \mathcal J(x) \defeq \defset{i \in \N_{[0, n-1]}}{\underline x_i
+    /// \lt x_i - \gamma\nabla_{\!x_i}\psi(x) \lt \overline x_i}. @f]
+    index_t eval_inactive_indices_res_lna(real_t γ, crvec x, crvec grad_ψ, rindexvec J) const;
+
+    /// @}
+
+    /// @name Constraint sets
+    /// @{
+
+    /// **[Optional]**
+    /// Get the rectangular constraint set of the decision variables,
+    /// @f$ x \in C @f$.
+    const Box &get_box_C() const;
+    /// **[Optional]**
+    /// Get the rectangular constraint set of the general constraint function,
+    /// @f$ g(x) \in D @f$.
+    const Box &get_box_D() const;
+
+    /// @}
+
     /// @name Functions for second-order solvers
     /// @{
 
+    /// **[Optional]**
+    /// Function that evaluates the Jacobian of the constraints as a sparse
+    /// matrix, @f$ \jac_g(x) @f$
+    /// @param  [in] x
+    ///         Decision variable @f$ x \in \R^n @f$
+    /// @param  [inout] inner_idx
+    ///         Inner indices (row indices of nonzeros).
+    /// @param  [inout] outer_ptr
+    ///         Outer pointers (points to the first nonzero in each column).
+    /// @param  [out] J_values
+    ///         Nonzero values of the Jacobian
+    ///         @f$ \jac_g(x) \in \R^{m\times n} @f$
+    /// If @p J_values has size zero, this function should initialize
+    /// @p inner_idx and @p outer_ptr. If @p J_values is nonempty, @p inner_idx
+    /// and @p outer_ptr can be assumed to be initialized, and this function
+    /// should evaluate @p J_values.
+    ///
+    /// Required for second-order solvers only.
+    void eval_jac_g(crvec x, rindexvec inner_idx, rindexvec outer_ptr, rvec J_values) const;
+    /// **[Optional]**
+    /// Function that gets the number of nonzeros of the Jacobian of the
+    /// constraints.
+    ///
+    /// Required for second-order solvers only.
+    length_t get_jac_g_num_nonzeros() const;
+    /// **[Optional]**
     /// Function that evaluates the gradient of one specific constraint,
     /// @f$ \nabla g_i(x) @f$
     /// @param  [in] x
     ///         Decision variable @f$ x \in \R^n @f$
     /// @param  [in] i
     ///         Which constraint @f$ 0 \le i \lt m @f$
     /// @param  [out] grad_gi
     ///         Gradient of the constraint
     ///         @f$ \nabla g_i(x) \in \R^n @f$
     ///
     /// Required for second-order solvers only.
     void eval_grad_gi(crvec x, index_t i, rvec grad_gi) const;
+    /// **[Optional]**
     /// Function that evaluates the Hessian of the Lagrangian multiplied by a
     /// vector,
     /// @f$ \nabla_{xx}^2L(x, y)\,v @f$
     /// @param  [in] x
     ///         Decision variable @f$ x \in \R^n @f$
     /// @param  [in] y
     ///         Lagrange multipliers @f$ y \in \R^m @f$
+    /// @param  [in] scale
+    ///         Scale factor for the cost function.
     /// @param  [in] v
     ///         Vector to multiply by @f$ v \in \R^n @f$
     /// @param  [out] Hv
     ///         Hessian-vector product
     ///         @f$ \nabla_{xx}^2 L(x, y)\,v \in \R^{n} @f$
     ///
     /// Required for second-order solvers only.
-    void eval_hess_L_prod(crvec x, crvec y, crvec v, rvec Hv) const;
-    /// Function that evaluates the Hessian of the Lagrangian,
+    void eval_hess_L_prod(crvec x, crvec y, real_t scale, crvec v, rvec Hv) const;
+    /// **[Optional]**
+    /// Function that evaluates the Hessian of the Lagrangian as a sparse matrix,
     /// @f$ \nabla_{xx}^2L(x, y) @f$
     /// @param  [in] x
     ///         Decision variable @f$ x \in \R^n @f$
     /// @param  [in] y
     ///         Lagrange multipliers @f$ y \in \R^m @f$
-    /// @param  [out] H
-    ///         Hessian @f$ \nabla_{xx}^2 L(x, y) \in \R^{n\times n} @f$
+    /// @param  [in] scale
+    ///         Scale factor for the cost function.
+    /// @param  [inout] inner_idx
+    ///         Inner indices (row indices of nonzeros).
+    /// @param  [inout] outer_ptr
+    ///         Outer pointers (points to the first nonzero in each column).
+    /// @param  [out] H_values
+    ///         Nonzero values of the Hessian
+    ///         @f$ \nabla_{xx}^2 L(x, y) \in \R^{n\times n} @f$.
+    /// If @p H_values has size zero, this function should initialize
+    /// @p inner_idx and @p outer_ptr. If @p H_values is nonempty, @p inner_idx
+    /// and @p outer_ptr can be assumed to be initialized, and this function
+    /// should evaluate @p H_values.
+    ///
+    /// Required for second-order solvers only.
+    void eval_hess_L(crvec x, crvec y, real_t scale, rindexvec inner_idx, rindexvec outer_ptr,
+                     rvec H_values) const;
+    /// **[Optional]**
+    /// Function that gets the number of nonzeros of the Hessian of the
+    /// Lagrangian.
+    ///
+    /// Required for second-order solvers only.
+    length_t get_hess_L_num_nonzeros() const;
+    /// **[Optional]**
+    /// Function that evaluates the Hessian of the augmented Lagrangian
+    /// multiplied by a vector,
+    /// @f$ \nabla_{xx}^2L_\Sigma(x, y)\,v @f$
+    /// @param  [in] x
+    ///         Decision variable @f$ x \in \R^n @f$
+    /// @param  [in] y
+    ///         Lagrange multipliers @f$ y \in \R^m @f$
+    /// @param  [in] Σ
+    ///         Penalty weights @f$ \Sigma @f$
+    /// @param  [in] scale
+    ///         Scale factor for the cost function.
+    /// @param  [in] v
+    ///         Vector to multiply by @f$ v \in \R^n @f$
+    /// @param  [out] Hv
+    ///         Hessian-vector product
+    ///         @f$ \nabla_{xx}^2 L_\Sigma(x, y)\,v \in \R^{n} @f$
+    ///
+    /// Required for second-order solvers only.
+    void eval_hess_ψ_prod(crvec x, crvec y, crvec Σ, real_t scale, crvec v, rvec Hv) const;
+    /// **[Optional]**
+    /// Function that evaluates the Hessian of the augmented Lagrangian,
+    /// @f$ \nabla_{xx}^2L_\Sigma(x, y) @f$
+    /// @param  [in] x
+    ///         Decision variable @f$ x \in \R^n @f$
+    /// @param  [in] y
+    ///         Lagrange multipliers @f$ y \in \R^m @f$
+    /// @param  [in] Σ
+    ///         Penalty weights @f$ \Sigma @f$
+    /// @param  [in] scale
+    ///         Scale factor for the cost function.
+    /// @param  [inout] inner_idx
+    ///         Inner indices (row indices of nonzeros).
+    /// @param  [inout] outer_ptr
+    ///         Outer pointers (points to the first nonzero in each column).
+    /// @param  [out] H_values
+    ///         Nonzero values of the Hessian
+    ///         @f$ \nabla_{xx}^2 L_\Sigma(x, y) \in \R^{n\times n} @f$
+    /// If @p H_values has size zero, this function should initialize
+    /// @p inner_idx and @p outer_ptr. If @p H_values is nonempty, @p inner_idx
+    /// and @p outer_ptr can be assumed to be initialized, and this function
+    /// should evaluate @p H_values.
+    ///
+    /// Required for second-order solvers only.
+    void eval_hess_ψ(crvec x, crvec y, crvec Σ, real_t scale, rindexvec inner_idx,
+                     rindexvec outer_ptr, rvec H_values) const;
+    /// **[Optional]**
+    /// Function that gets the number of nonzeros of the Hessian of the
+    /// augmented Lagrangian.
     ///
     /// Required for second-order solvers only.
-    void eval_hess_L(crvec x, crvec y, rmat H) const;
+    length_t get_hess_ψ_num_nonzeros() const;
 
     /// @}
 
     /// @name Combined evaluations
     /// @{
 
+    /// **[Optional]**
     /// Evaluate both @f$ f(x) @f$ and its gradient, @f$ \nabla f(x) @f$.
+    /// @default_impl   ProblemVTable::default_eval_f_grad_f
     real_t eval_f_grad_f(crvec x, rvec grad_fx) const;
+    /// **[Optional]**
     /// Evaluate both @f$ f(x) @f$ and @f$ g(x) @f$.
+    /// @default_impl   ProblemVTable::default_eval_f_g
     real_t eval_f_g(crvec x, rvec g) const;
-    /// Evaluate @f$ f(x) @f$, its gradient @f$ \nabla f(x) @f$ and @f$ g(x) @f$.
-    real_t eval_f_grad_f_g(crvec x, rvec grad_fx, rvec g) const;
+    /// **[Optional]**
     /// Evaluate both @f$ \nabla f(x) @f$ and @f$ \nabla g(x)\,y @f$.
+    /// @default_impl   ProblemVTable::default_eval_grad_f_grad_g_prod
     void eval_grad_f_grad_g_prod(crvec x, crvec y, rvec grad_f, rvec grad_gxy) const;
+    /// **[Optional]**
     /// Evaluate the gradient of the Lagrangian
     /// @f$ \nabla_x L(x, y) = \nabla f(x) + \nabla g(x)\,y @f$
+    /// @default_impl   ProblemVTable::default_eval_grad_L
     void eval_grad_L(crvec x, crvec y, rvec grad_L, rvec work_n) const;
 
     /// @}
 
     /// @name Augmented Lagrangian
     /// @{
 
+    /// **[Optional]**
     /// Calculate both ψ(x) and the vector ŷ that can later be used to compute
     /// ∇ψ.
     /// @f[ \psi(x) = f(x) + \tfrac{1}{2}
     ///   \text{dist}_\Sigma^2\left(g(x) + \Sigma^{-1}y,\;D\right) @f]
     /// @f[ \hat y = \Sigma\, \left(g(x) + \Sigma^{-1}y - \Pi_D\left(g(x)
     ///   + \Sigma^{-1}y\right)\right) @f]
+    /// @default_impl   ProblemVTable::default_eval_ψ
     real_t eval_ψ(crvec x, ///< [in]  Decision variable @f$ x @f$
                   crvec y, ///< [in]  Lagrange multipliers @f$ y @f$
                   crvec Σ, ///< [in]  Penalty weights @f$ \Sigma @f$
                   rvec ŷ   ///< [out] @f$ \hat y @f$
     ) const;
-    /// Calculate ∇ψ(x) using ŷ.
-    void eval_grad_ψ_from_ŷ(crvec x,     ///< [in]  Decision variable @f$ x @f$
-                            crvec ŷ,     ///< [in]  @f$ \hat y @f$
-                            rvec grad_ψ, ///< [out] @f$ \nabla \psi(x) @f$
-                            rvec work_n  ///<       Dimension @f$ n @f$
-    ) const;
+    /// **[Optional]**
     /// Calculate the gradient ∇ψ(x).
     /// @f[ \nabla \psi(x) = \nabla f(x) + \nabla g(x)\,\hat y(x) @f]
+    /// @default_impl   ProblemVTable::default_eval_grad_ψ
     void eval_grad_ψ(crvec x,     ///< [in]  Decision variable @f$ x @f$
                      crvec y,     ///< [in]  Lagrange multipliers @f$ y @f$
                      crvec Σ,     ///< [in]  Penalty weights @f$ \Sigma @f$
                      rvec grad_ψ, ///< [out] @f$ \nabla \psi(x) @f$
                      rvec work_n, ///<       Dimension @f$ n @f$
                      rvec work_m  ///<       Dimension @f$ m @f$
     ) const;
+    /// **[Optional]**
     /// Calculate both ψ(x) and its gradient ∇ψ(x).
     /// @f[ \psi(x) = f(x) + \tfrac{1}{2}
     /// \text{dist}_\Sigma^2\left(g(x) + \Sigma^{-1}y,\;D\right) @f]
     /// @f[ \nabla \psi(x) = \nabla f(x) + \nabla g(x)\,\hat y(x) @f]
+    /// @default_impl   ProblemVTable::default_eval_ψ_grad_ψ
     real_t eval_ψ_grad_ψ(crvec x,     ///< [in]  Decision variable @f$ x @f$
                          crvec y,     ///< [in]  Lagrange multipliers @f$ y @f$
                          crvec Σ,     ///< [in]  Penalty weights @f$ \Sigma @f$
                          rvec grad_ψ, ///< [out] @f$ \nabla \psi(x) @f$
                          rvec work_n, ///<       Dimension @f$ n @f$
                          rvec work_m  ///<       Dimension @f$ m @f$
     ) const;
 
     /// @}
 
-    /// @name Helpers
-    /// @{
-
-    /// Given g(x), compute the intermediate results ŷ and dᵀŷ that can later be
-    /// used to compute ψ(x) and ∇ψ(x).
-    /// @param[inout]   g_ŷ
-    ///                 Input @f$ g(x) @f$, outputs @f$ \hat y @f$
-    /// @param[in]      y
-    ///                 Lagrange multipliers @f$ y @f$
-    /// @param[in]      Σ
-    ///                 Penalty weights @f$ \Sigma @f$
-    /// @return The inner product @f$ d^\top \hat y @f$
-    real_t calc_ŷ_dᵀŷ(rvec g_ŷ, crvec y, crvec Σ) const;
-
-    /// @}
-
-    /// @name Constraint sets
-    /// @{
-
-    /// Get the rectangular constraint set of the decision variables,
-    /// @f$ x \in C @f$.
-    const Box &get_box_C() const;
-    /// Get the rectangular constraint set of the general constraint function,
-    /// @f$ g(x) \in D @f$.
-    const Box &get_box_D() const;
-
-    /// @}
-
     /// @name Checks
     /// @{
 
+    /// **[Optional]**
     /// Check that the problem formulation is well-defined, the dimensions match,
     /// etc. Throws an exception if this is not the case.
     void check() const;
 
-    /// }
+    /// @}
 
     /// @name Querying specialized implementations
     /// @{
 
     /// Returns true if the problem provides an implementation of
+    /// @ref eval_inactive_indices_res_lna.
+    bool provides_eval_inactive_indices_res_lna() const {
+        return vtable.eval_inactive_indices_res_lna != vtable.default_eval_inactive_indices_res_lna;
+    }
+    /// Returns true if the problem provides an implementation of
+    /// @ref eval_jac_g.
+    bool provides_eval_jac_g() const { return vtable.eval_jac_g != vtable.default_eval_jac_g; }
+    /// Returns true if the problem provides an implementation of
+    /// @ref get_jac_g_num_nonzeros.
+    bool provides_get_jac_g_num_nonzeros() const {
+        return vtable.get_jac_g_num_nonzeros != vtable.default_get_jac_g_num_nonzeros;
+    }
+    /// Returns true if the problem provides an implementation of
     /// @ref eval_grad_gi.
     bool provides_eval_grad_gi() const {
         return vtable.eval_grad_gi != vtable.default_eval_grad_gi;
     }
     /// Returns true if the problem provides an implementation of
     /// @ref eval_hess_L_prod.
     bool provides_eval_hess_L_prod() const {
         return vtable.eval_hess_L_prod != vtable.default_eval_hess_L_prod;
     }
     /// Returns true if the problem provides an implementation of
     /// @ref eval_hess_L.
     bool provides_eval_hess_L() const { return vtable.eval_hess_L != vtable.default_eval_hess_L; }
+    /// Returns true if the problem provides an implementation of
+    /// @ref get_hess_L_num_nonzeros.
+    bool provides_get_hess_L_num_nonzeros() const {
+        return vtable.get_hess_L_num_nonzeros != vtable.default_get_hess_L_num_nonzeros;
+    }
+    /// Returns true if the problem provides an implementation of
+    /// @ref eval_hess_ψ_prod.
+    bool provides_eval_hess_ψ_prod() const {
+        return vtable.eval_hess_ψ_prod != vtable.default_eval_hess_ψ_prod;
+    }
+    /// Returns true if the problem provides an implementation of
+    /// @ref eval_hess_ψ.
+    bool provides_eval_hess_ψ() const { return vtable.eval_hess_ψ != vtable.default_eval_hess_ψ; }
+    /// Returns true if the problem provides an implementation of
+    /// @ref get_hess_ψ_num_nonzeros.
+    bool provides_get_hess_ψ_num_nonzeros() const {
+        return vtable.get_hess_ψ_num_nonzeros != vtable.default_get_hess_ψ_num_nonzeros;
+    }
     /// Returns true if the problem provides a specialized implementation of
     /// @ref eval_f_grad_f, false if it uses the default implementation.
     bool provides_eval_f_grad_f() const {
         return vtable.eval_f_grad_f != vtable.default_eval_f_grad_f;
     }
     /// Returns true if the problem provides a specialized implementation of
     /// @ref eval_f_g, false if it uses the default implementation.
     bool provides_eval_f_g() const { return vtable.eval_f_g != vtable.default_eval_f_g; }
     /// Returns true if the problem provides a specialized implementation of
-    /// @ref eval_f_grad_f_g, false if it uses the default implementation.
-    bool provides_eval_f_grad_f_g() const {
-        return vtable.eval_f_grad_f_g != vtable.default_eval_f_grad_f_g;
-    }
-    /// Returns true if the problem provides a specialized implementation of
     /// @ref eval_grad_f_grad_g_prod, false if it uses the default implementation.
     bool provides_eval_grad_f_grad_g_prod() const {
         return vtable.eval_grad_f_grad_g_prod != vtable.default_eval_grad_f_grad_g_prod;
     }
     /// Returns true if the problem provides a specialized implementation of
     /// @ref eval_grad_L, false if it uses the default implementation.
     bool provides_eval_grad_L() const { return vtable.eval_grad_L != vtable.default_eval_grad_L; }
     /// Returns true if the problem provides a specialized implementation of
     /// @ref eval_ψ, false if it uses the default implementation.
     bool provides_eval_ψ() const { return vtable.eval_ψ != vtable.default_eval_ψ; }
     /// Returns true if the problem provides a specialized implementation of
-    /// @ref eval_grad_ψ_from_ŷ, false if it uses the default implementation.
-    bool provides_eval_grad_ψ_from_ŷ() const {
-        return vtable.eval_grad_ψ_from_ŷ != vtable.default_eval_grad_ψ_from_ŷ;
-    }
-    /// Returns true if the problem provides a specialized implementation of
     /// @ref eval_grad_ψ, false if it uses the default implementation.
     bool provides_eval_grad_ψ() const { return vtable.eval_grad_ψ != vtable.default_eval_grad_ψ; }
     /// Returns true if the problem provides a specialized implementation of
     /// @ref eval_ψ_grad_ψ, false if it uses the default implementation.
     bool provides_eval_ψ_grad_ψ() const {
         return vtable.eval_ψ_grad_ψ != vtable.default_eval_ψ_grad_ψ;
     }
     /// Returns true if the problem provides an implementation of
     /// @ref get_box_C.
     bool provides_get_box_C() const { return vtable.get_box_C != vtable.default_get_box_C; }
     /// Returns true if the problem provides an implementation of
     /// @ref get_box_D.
     bool provides_get_box_D() const { return vtable.get_box_D != vtable.default_get_box_D; }
+    /// Returns true if the problem provides an implementation of @ref check.
+    bool provides_check() const { return vtable.check != vtable.default_check; }
+
+    /// @}
+
+    /// @name Helpers
+    /// @{
+
+    /// Given g(x), compute the intermediate results ŷ and dᵀŷ that can later be
+    /// used to compute ψ(x) and ∇ψ(x).
+    ///
+    /// Computes the result using the following algorithm:
+    /// @f[ \begin{aligned}
+    ///     \zeta &= g(x) + \Sigma^{-1} y \\[]
+    ///     d &= \zeta - \Pi_D(\zeta)
+    ///        = \operatorname{eval\_proj\_diff\_g}(\zeta, \zeta) \\[]
+    ///     \hat y &= \Sigma d \\[]
+    /// \end{aligned} @f]
+    /// @see @ref page_math
+    ///
+    /// @param[inout]   g_ŷ
+    ///                 Input @f$ g(x) @f$, outputs @f$ \hat y @f$
+    /// @param[in]      y
+    ///                 Lagrange multipliers @f$ y @f$
+    /// @param[in]      Σ
+    ///                 Penalty weights @f$ \Sigma @f$
+    /// @return The inner product @f$ d^\top \hat y @f$
+    real_t calc_ŷ_dᵀŷ(rvec g_ŷ, crvec y, crvec Σ) const;
 
     /// @}
 };
 
+/// @}
+
 #ifndef DOXYGEN
 template <class Tref>
 explicit TypeErasedProblem(Tref &&d)
     -> TypeErasedProblem<typename std::remove_cvref_t<Tref>::config_t>;
 
 template <class Tref, class Allocator>
 explicit TypeErasedProblem(Tref &&d, Allocator alloc)
@@ -617,28 +714,34 @@
 }
 template <Config Conf, class Allocator>
 auto TypeErasedProblem<Conf, Allocator>::get_m() const -> length_t {
     return vtable.m;
 }
 
 template <Config Conf, class Allocator>
-void TypeErasedProblem<Conf, Allocator>::eval_proj_diff_g(crvec z, rvec p) const {
-    return call(vtable.eval_proj_diff_g, z, p);
+void TypeErasedProblem<Conf, Allocator>::eval_proj_diff_g(crvec z, rvec e) const {
+    return call(vtable.eval_proj_diff_g, z, e);
 }
 template <Config Conf, class Allocator>
-void TypeErasedProblem<Conf, Allocator>::eval_proj_multipliers(rvec y, real_t M,
-                                                               index_t penalty_alm_split) const {
-    return call(vtable.eval_proj_multipliers, y, M, penalty_alm_split);
+void TypeErasedProblem<Conf, Allocator>::eval_proj_multipliers(rvec y, real_t M) const {
+    return call(vtable.eval_proj_multipliers, y, M);
 }
 template <Config Conf, class Allocator>
-void TypeErasedProblem<Conf, Allocator>::eval_prox_grad_step(real_t γ, crvec x, crvec grad_ψ,
-                                                             rvec x̂, rvec p) const {
+auto TypeErasedProblem<Conf, Allocator>::eval_prox_grad_step(real_t γ, crvec x, crvec grad_ψ,
+                                                             rvec x̂, rvec p) const -> real_t {
     return call(vtable.eval_prox_grad_step, γ, x, grad_ψ, x̂, p);
 }
 template <Config Conf, class Allocator>
+auto TypeErasedProblem<Conf, Allocator>::eval_inactive_indices_res_lna(real_t γ, crvec x,
+                                                                       crvec grad_ψ,
+                                                                       rindexvec J) const
+    -> index_t {
+    return call(vtable.eval_inactive_indices_res_lna, γ, x, grad_ψ, J);
+}
+template <Config Conf, class Allocator>
 auto TypeErasedProblem<Conf, Allocator>::eval_f(crvec x) const -> real_t {
     return call(vtable.eval_f, x);
 }
 template <Config Conf, class Allocator>
 void TypeErasedProblem<Conf, Allocator>::eval_grad_f(crvec x, rvec grad_fx) const {
     return call(vtable.eval_grad_f, x, grad_fx);
 }
@@ -651,55 +754,75 @@
     return call(vtable.eval_grad_g_prod, x, y, grad_gxy);
 }
 template <Config Conf, class Allocator>
 void TypeErasedProblem<Conf, Allocator>::eval_grad_gi(crvec x, index_t i, rvec grad_gi) const {
     return call(vtable.eval_grad_gi, x, i, grad_gi);
 }
 template <Config Conf, class Allocator>
-void TypeErasedProblem<Conf, Allocator>::eval_hess_L_prod(crvec x, crvec y, crvec v,
+void TypeErasedProblem<Conf, Allocator>::eval_jac_g(crvec x, rindexvec inner_idx,
+                                                    rindexvec outer_ptr, rvec J_values) const {
+    return call(vtable.eval_jac_g, x, inner_idx, outer_ptr, J_values);
+}
+template <Config Conf, class Allocator>
+auto TypeErasedProblem<Conf, Allocator>::get_jac_g_num_nonzeros() const -> length_t {
+    return call(vtable.get_jac_g_num_nonzeros);
+}
+template <Config Conf, class Allocator>
+void TypeErasedProblem<Conf, Allocator>::eval_hess_L_prod(crvec x, crvec y, real_t scale, crvec v,
                                                           rvec Hv) const {
-    return call(vtable.eval_hess_L_prod, x, y, v, Hv);
+    return call(vtable.eval_hess_L_prod, x, y, scale, v, Hv);
+}
+template <Config Conf, class Allocator>
+void TypeErasedProblem<Conf, Allocator>::eval_hess_L(crvec x, crvec y, real_t scale,
+                                                     rindexvec inner_idx, rindexvec outer_ptr,
+                                                     rvec H_values) const {
+    return call(vtable.eval_hess_L, x, y, scale, inner_idx, outer_ptr, H_values);
+}
+template <Config Conf, class Allocator>
+auto TypeErasedProblem<Conf, Allocator>::get_hess_L_num_nonzeros() const -> length_t {
+    return call(vtable.get_hess_L_num_nonzeros);
 }
 template <Config Conf, class Allocator>
-void TypeErasedProblem<Conf, Allocator>::eval_hess_L(crvec x, crvec y, rmat H) const {
-    return call(vtable.eval_hess_L, x, y, H);
+void TypeErasedProblem<Conf, Allocator>::eval_hess_ψ_prod(crvec x, crvec y, crvec Σ, real_t scale,
+                                                          crvec v, rvec Hv) const {
+    return call(vtable.eval_hess_ψ_prod, x, y, Σ, scale, v, Hv);
+}
+template <Config Conf, class Allocator>
+void TypeErasedProblem<Conf, Allocator>::eval_hess_ψ(crvec x, crvec y, crvec Σ, real_t scale,
+                                                     rindexvec inner_idx, rindexvec outer_ptr,
+                                                     rvec H_values) const {
+    return call(vtable.eval_hess_ψ, x, y, Σ, scale, inner_idx, outer_ptr, H_values);
+}
+template <Config Conf, class Allocator>
+auto TypeErasedProblem<Conf, Allocator>::get_hess_ψ_num_nonzeros() const -> length_t {
+    return call(vtable.get_hess_ψ_num_nonzeros);
 }
 template <Config Conf, class Allocator>
 auto TypeErasedProblem<Conf, Allocator>::eval_f_grad_f(crvec x, rvec grad_fx) const -> real_t {
     return call(vtable.eval_f_grad_f, x, grad_fx);
 }
 template <Config Conf, class Allocator>
 auto TypeErasedProblem<Conf, Allocator>::eval_f_g(crvec x, rvec g) const -> real_t {
     return call(vtable.eval_f_g, x, g);
 }
 template <Config Conf, class Allocator>
-auto TypeErasedProblem<Conf, Allocator>::eval_f_grad_f_g(crvec x, rvec grad_fx, rvec g) const
-    -> real_t {
-    return call(vtable.eval_f_grad_f_g, x, grad_fx, g);
-}
-template <Config Conf, class Allocator>
 void TypeErasedProblem<Conf, Allocator>::eval_grad_f_grad_g_prod(crvec x, crvec y, rvec grad_f,
                                                                  rvec grad_gxy) const {
     return call(vtable.eval_grad_f_grad_g_prod, x, y, grad_f, grad_gxy);
 }
 template <Config Conf, class Allocator>
 void TypeErasedProblem<Conf, Allocator>::eval_grad_L(crvec x, crvec y, rvec grad_L,
                                                      rvec work_n) const {
     return call(vtable.eval_grad_L, x, y, grad_L, work_n);
 }
 template <Config Conf, class Allocator>
 auto TypeErasedProblem<Conf, Allocator>::eval_ψ(crvec x, crvec y, crvec Σ, rvec ŷ) const -> real_t {
     return call(vtable.eval_ψ, x, y, Σ, ŷ);
 }
 template <Config Conf, class Allocator>
-void TypeErasedProblem<Conf, Allocator>::eval_grad_ψ_from_ŷ(crvec x, crvec ŷ, rvec grad_ψ,
-                                                            rvec work_n) const {
-    return call(vtable.eval_grad_ψ_from_ŷ, x, ŷ, grad_ψ, work_n);
-}
-template <Config Conf, class Allocator>
 void TypeErasedProblem<Conf, Allocator>::eval_grad_ψ(crvec x, crvec y, crvec Σ, rvec grad_ψ,
                                                      rvec work_n, rvec work_m) const {
     return call(vtable.eval_grad_ψ, x, y, Σ, grad_ψ, work_n, work_m);
 }
 template <Config Conf, class Allocator>
 auto TypeErasedProblem<Conf, Allocator>::eval_ψ_grad_ψ(crvec x, crvec y, crvec Σ, rvec grad_ψ,
                                                        rvec work_n, rvec work_m) const -> real_t {
@@ -718,222 +841,34 @@
     return call(vtable.get_box_D);
 }
 template <Config Conf, class Allocator>
 void TypeErasedProblem<Conf, Allocator>::check() const {
     return call(vtable.check);
 }
 
-template <class Problem>
-struct ProblemWithCounters {
-    USING_ALPAQA_CONFIG_TEMPLATE(std::remove_cvref_t<Problem>::config_t);
-    using Box = typename TypeErasedProblem<config_t>::Box;
-
-    // clang-format off
-    void eval_proj_diff_g(crvec z, rvec p) const { ++evaluations->proj_diff_g; return timed(evaluations->time.proj_diff_g, std::bind(&std::remove_cvref_t<Problem>::eval_proj_diff_g, &problem, z, p)); }
-    void eval_proj_multipliers(rvec y, real_t M, index_t penalty_alm_split) const { ++evaluations->proj_multipliers; return timed(evaluations->time.proj_multipliers, std::bind(&std::remove_cvref_t<Problem>::eval_proj_multipliers, &problem, y, M, penalty_alm_split)); }
-    void eval_prox_grad_step(real_t γ, crvec x, crvec grad_ψ, rvec x̂, rvec p) const { ++evaluations->prox_grad_step; return timed(evaluations->time.prox_grad_step, std::bind(&std::remove_cvref_t<Problem>::eval_prox_grad_step, &problem, γ, x, grad_ψ, x̂, p)); }
-    real_t eval_f(crvec x) const { ++evaluations->f; return timed(evaluations->time.f, std::bind(&std::remove_cvref_t<Problem>::eval_f, &problem, x)); }
-    void eval_grad_f(crvec x, rvec grad_fx) const { ++evaluations->grad_f; return timed(evaluations->time.grad_f, std::bind(&std::remove_cvref_t<Problem>::eval_grad_f, &problem, x, grad_fx)); }
-    void eval_g(crvec x, rvec gx) const { ++evaluations->g; return timed(evaluations->time.g, std::bind(&std::remove_cvref_t<Problem>::eval_g, &problem, x, gx)); }
-    void eval_grad_g_prod(crvec x, crvec y, rvec grad_gxy) const { ++evaluations->grad_g_prod; return timed(evaluations->time.grad_g_prod, std::bind(&std::remove_cvref_t<Problem>::eval_grad_g_prod, &problem, x, y, grad_gxy)); }
-    void eval_grad_gi(crvec x, index_t i, rvec grad_gi) const requires requires { &std::remove_cvref_t<Problem>::eval_grad_gi; } { ++evaluations->grad_gi; return timed(evaluations->time.grad_gi, std::bind(&std::remove_cvref_t<Problem>::eval_grad_gi, &problem, x, i, grad_gi)); }
-    void eval_hess_L_prod(crvec x, crvec y, crvec v, rvec Hv) const requires requires { &std::remove_cvref_t<Problem>::eval_hess_L_prod; } { ++evaluations->hess_L_prod; return timed(evaluations->time.hess_L_prod, std::bind(&std::remove_cvref_t<Problem>::eval_hess_L_prod, &problem, x, y, v, Hv)); }
-    void eval_hess_L(crvec x, crvec y, rmat H) const requires requires { &std::remove_cvref_t<Problem>::eval_hess_L; } { ++evaluations->hess_L; return timed(evaluations->time.hess_L, std::bind(&std::remove_cvref_t<Problem>::eval_hess_L, &problem, x, y, H)); }
-    real_t eval_f_grad_f(crvec x, rvec grad_fx) const requires requires { &std::remove_cvref_t<Problem>::eval_f_grad_f; } { ++evaluations->f_grad_f; return timed(evaluations->time.f_grad_f, std::bind(&std::remove_cvref_t<Problem>::eval_f_grad_f, &problem, x, grad_fx)); }
-    real_t eval_f_g(crvec x, rvec g) const requires requires { &std::remove_cvref_t<Problem>::eval_f_g; } { ++evaluations->f_g; return timed(evaluations->time.f_g, std::bind(&std::remove_cvref_t<Problem>::eval_f_g, &problem, x, g)); }
-    real_t eval_f_grad_f_g(crvec x, rvec grad_fx, rvec g) const requires requires { &std::remove_cvref_t<Problem>::eval_f_grad_f_g; } { ++evaluations->f_grad_f_g; return timed(evaluations->time.f_grad_f_g, std::bind(&std::remove_cvref_t<Problem>::eval_f_grad_f_g, &problem, x, grad_fx, g)); }
-    void eval_grad_f_grad_g_prod(crvec x, crvec y, rvec grad_f, rvec grad_gxy) const requires requires { &std::remove_cvref_t<Problem>::eval_grad_f_grad_g_prod; } { ++evaluations->grad_f_grad_g_prod; return timed(evaluations->time.grad_f_grad_g_prod, std::bind(&std::remove_cvref_t<Problem>::eval_grad_f_grad_g_prod, &problem, x, y, grad_f, grad_gxy)); }
-    void eval_grad_L(crvec x, crvec y, rvec grad_L, rvec work_n) const requires requires { &std::remove_cvref_t<Problem>::eval_grad_L; } { ++evaluations->grad_L; return timed(evaluations->time.grad_L, std::bind(&std::remove_cvref_t<Problem>::eval_grad_L, &problem, x, y, grad_L, work_n)); }
-    real_t eval_ψ(crvec x, crvec y, crvec Σ, rvec ŷ) const requires requires { &std::remove_cvref_t<Problem>::eval_ψ; } { ++evaluations->ψ; return timed(evaluations->time.ψ, std::bind(&std::remove_cvref_t<Problem>::eval_ψ, &problem, x, y, Σ, ŷ)); }
-    void eval_grad_ψ_from_ŷ(crvec x, crvec ŷ, rvec grad_ψ, rvec work_n) const requires requires { &std::remove_cvref_t<Problem>::eval_grad_ψ_from_ŷ; } { ++evaluations->grad_ψ_from_ŷ; return timed(evaluations->time.grad_ψ_from_ŷ, std::bind(&std::remove_cvref_t<Problem>::eval_grad_ψ_from_ŷ, &problem, x, ŷ, grad_ψ, work_n)); }
-    void eval_grad_ψ(crvec x, crvec y, crvec Σ, rvec grad_ψ, rvec work_n, rvec work_m) const requires requires { &std::remove_cvref_t<Problem>::eval_grad_ψ; } { ++evaluations->grad_ψ; return timed(evaluations->time.grad_ψ, std::bind(&std::remove_cvref_t<Problem>::eval_grad_ψ, &problem, x, y, Σ, grad_ψ, work_n, work_m)); }
-    real_t eval_ψ_grad_ψ(crvec x, crvec y, crvec Σ, rvec grad_ψ, rvec work_n, rvec work_m) const requires requires { &std::remove_cvref_t<Problem>::eval_ψ_grad_ψ; } { ++evaluations->ψ_grad_ψ; return timed(evaluations->time.ψ_grad_ψ, std::bind(&std::remove_cvref_t<Problem>::eval_ψ_grad_ψ, &problem, x, y, Σ, grad_ψ, work_n, work_m)); }
-    const Box &get_box_C() const requires requires { &std::remove_cvref_t<Problem>::get_box_C; } { ++evaluations->f_g; return timed(evaluations->time.f_g, std::bind(&std::remove_cvref_t<Problem>::get_box_C, &problem)); }
-    const Box &get_box_D() const requires requires { &std::remove_cvref_t<Problem>::get_box_D; } { ++evaluations->f_g; return timed(evaluations->time.f_g, std::bind(&std::remove_cvref_t<Problem>::get_box_D, &problem)); }
-    void check() const { problem.check(); }
-
-    template <class... Args> decltype(auto) provides_eval_grad_gi(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_grad_gi; } { return problem.provides_eval_grad_gi(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_eval_hess_L_prod(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_hess_L_prod; } { return problem.provides_eval_hess_L_prod(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_eval_hess_L(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_hess_L; } { return problem.provides_eval_hess_L(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_eval_f_grad_f(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_f_grad_f; } { return problem.provides_eval_f_grad_f(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_eval_f_g(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_f_g; } { return problem.provides_eval_f_g(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_eval_f_grad_f_g(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_f_grad_f_g; } { return problem.provides_eval_f_grad_f_g(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_eval_grad_f_grad_g_prod(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_grad_f_grad_g_prod; } { return problem.provides_eval_grad_f_grad_g_prod(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_eval_grad_L(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_grad_L; } { return problem.provides_eval_grad_L(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_eval_ψ(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_ψ; } { return problem.provides_eval_ψ(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_eval_grad_ψ_from_ŷ(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_grad_ψ_from_ŷ; } { return problem.provides_eval_grad_ψ_from_ŷ(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_eval_grad_ψ(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_grad_ψ; } { return problem.provides_eval_grad_ψ(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_eval_ψ_grad_ψ(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_eval_ψ_grad_ψ; } { return problem.provides_eval_ψ_grad_ψ(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_get_box_C(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_get_box_C; } { return problem.provides_get_box_C(std::forward<Args>(args)...); }
-    template <class... Args> decltype(auto) provides_get_box_D(Args... args) const requires requires { &std::remove_cvref_t<Problem>::provides_get_box_D; } { return problem.provides_get_box_D(std::forward<Args>(args)...); }
-    // clang-format on
-
-    length_t get_n() const { return problem.get_n(); }
-    length_t get_m() const { return problem.get_m(); }
-
-    std::shared_ptr<EvalCounter> evaluations = std::make_shared<EvalCounter>();
-    Problem problem;
-
-    ProblemWithCounters(const Problem &problem) : problem(problem) {}
-    ProblemWithCounters(Problem &&problem)
-        requires(!std::is_lvalue_reference_v<Problem>)
-        : problem(std::forward<Problem>(problem)) {}
-
-  private:
-    template <class TimeT, class FunT>
-    static decltype(auto) timed(TimeT &time, FunT &&f) {
-        detail::Timed timed{time};
-        return std::forward<FunT>(f)();
-    }
-};
-
-template <class Problem>
-auto problem_with_counters(Problem &&p) {
-    using Prob        = std::remove_cvref_t<Problem>;
-    using ProbWithCnt = ProblemWithCounters<Prob>;
-    return ProbWithCnt{std::forward<Problem>(p)};
-}
-
-template <class Problem>
-auto problem_with_counters_ref(Problem &p) {
-    using Prob        = std::remove_cvref_t<Problem>;
-    using ProbWithCnt = ProblemWithCounters<const Prob &>;
-    return ProbWithCnt{p};
-}
+/// @addtogroup grp_Problems
+/// @{
 
 template <Config Conf>
-class BoxConstrProblem {
-  public:
-    USING_ALPAQA_CONFIG(Conf);
-    using Box = alpaqa::Box<config_t>;
-
-    /// Number of decision variables, dimension of x
-    length_t n;
-    /// Number of constraints, dimension of g(x) and z
-    length_t m;
-
-    BoxConstrProblem(length_t n, ///< Number of decision variables
-                     length_t m) ///< Number of constraints
-        : n{n}, m{m} {}
-
-    BoxConstrProblem(Box C, Box D)
-        : n{C.lowerbound.size()}, m{D.lowerbound.size()}, C{std::move(C)}, D{std::move(D)} {}
-
-    BoxConstrProblem(const BoxConstrProblem &)                = default;
-    BoxConstrProblem &operator=(const BoxConstrProblem &)     = default;
-    BoxConstrProblem(BoxConstrProblem &&) noexcept            = default;
-    BoxConstrProblem &operator=(BoxConstrProblem &&) noexcept = default;
-
-    /// Constraints of the decision variables, @f$ x \in C @f$
-    Box C{vec::Constant(this->n, +inf<Conf>), vec::Constant(this->n, -inf<Conf>)};
-    /// Other constraints, @f$ g(x) \in D @f$
-    Box D{vec::Constant(this->m, +inf<Conf>), vec::Constant(this->m, -inf<Conf>)};
-
-    /// Number of decision variables, @ref n
-    length_t get_n() const { return n; }
-    /// Number of constraints, @ref m
-    length_t get_m() const { return m; }
-
-    /// @f$ \hat x = \Pi_C(x - \gamma\nabla\psi(x)) @f$
-    /// @f$ p = \hat x - x @f$
-    static void eval_proj_grad_step_box(const Box &C, real_t γ, crvec x, crvec grad_ψ, rvec x̂,
-                                        rvec p) {
-        using binary_real_f = real_t (*)(real_t, real_t);
-        p                   = (-γ * grad_ψ)
-                .binaryExpr(C.lowerbound - x, binary_real_f(std::fmax))
-                .binaryExpr(C.upperbound - x, binary_real_f(std::fmin));
-        x̂ = x + p;
-    }
-
-    /// @see @ref TypeErasedProblem::eval_prox_grad_step
-    void eval_prox_grad_step(real_t γ, crvec x, crvec grad_ψ, rvec x̂, rvec p) const {
-        eval_proj_grad_step_box(C, γ, x, grad_ψ, x̂, p);
-    }
-
-    /// @see @ref TypeErasedProblem::eval_proj_diff_g
-    void eval_proj_diff_g(crvec z, rvec p) const { p = alpaqa::projecting_difference(z, D); }
-
-    static void eval_proj_multipliers_box(const Box &D, rvec y, real_t M,
-                                          index_t penalty_alm_split) {
-        auto max_lb = [M](real_t y, real_t z_lb) {
-            real_t y_lb = z_lb == -alpaqa::inf<config_t> ? 0 : -M;
-            return std::max(y, y_lb);
-        };
-        auto min_ub = [M](real_t y, real_t z_ub) {
-            real_t y_ub = z_ub == alpaqa::inf<config_t> ? 0 : M;
-            return std::min(y, y_ub);
-        };
-        auto num_alm    = y.size() - penalty_alm_split;
-        auto &&y_alm    = y.bottomRows(num_alm);
-        auto &&z_alm_lb = D.lowerbound.bottomRows(num_alm);
-        auto &&z_alm_ub = D.upperbound.bottomRows(num_alm);
-        y_alm           = y_alm.binaryExpr(z_alm_lb, max_lb).binaryExpr(z_alm_ub, min_ub);
-    }
-
-    /// @see @ref TypeErasedProblem::eval_proj_multipliers
-    void eval_proj_multipliers(rvec y, real_t M, index_t penalty_alm_split) const {
-        eval_proj_multipliers_box(D, y, M, penalty_alm_split);
-    }
-
-    /// @see @ref TypeErasedProblem::get_box_C
-    const Box &get_box_C() const { return C; }
-    /// @see @ref TypeErasedProblem::get_box_D
-    const Box &get_box_D() const { return D; }
-
-    /// @see @ref TypeErasedProblem::check
-    void check() const {
-        util::check_dim_msg<config_t>(
-            C.lowerbound, n,
-            "Length of problem.C.lowerbound does not match problem size problem.n");
-        util::check_dim_msg<config_t>(
-            C.upperbound, n,
-            "Length of problem.C.upperbound does not match problem size problem.n");
-        util::check_dim_msg<config_t>(
-            D.lowerbound, m,
-            "Length of problem.D.lowerbound does not match problem size problem.m");
-        util::check_dim_msg<config_t>(
-            D.upperbound, m,
-            "Length of problem.D.upperbound does not match problem size problem.m");
-    }
-};
-
-/// @ref Problem class that allows specifying the basic functions as C++
-/// `std::function`s.
-/// @ingroup grp_Problems
-template <Config Conf = DefaultConfig>
-class FunctionalProblem : public BoxConstrProblem<Conf> {
-  public:
-    USING_ALPAQA_CONFIG(Conf);
-    using BoxConstrProblem<Conf>::BoxConstrProblem;
-
-    std::function<real_t(crvec)> f;
-    std::function<void(crvec, rvec)> grad_f;
-    std::function<void(crvec, rvec)> g;
-    std::function<void(crvec, crvec, rvec)> grad_g_prod;
-    std::function<void(crvec, index_t, rvec)> grad_gi;
-    std::function<void(crvec, crvec, crvec, rvec)> hess_L_prod;
-    std::function<void(crvec, crvec, rmat)> hess_L;
-
-    // clang-format off
-    real_t eval_f(crvec x) const { ScopedMallocAllower ma; return f(x); }
-    void eval_grad_f(crvec x, rvec grad_fx) const { ScopedMallocAllower ma; grad_f(x, grad_fx); }
-    void eval_g(crvec x, rvec gx) const { ScopedMallocAllower ma; g(x, gx); }
-    void eval_grad_g_prod(crvec x, crvec y, rvec grad_gxy) const { ScopedMallocAllower ma; grad_g_prod(x, y, grad_gxy); }
-    void eval_grad_gi(crvec x, index_t i, rvec grad_i) const { ScopedMallocAllower ma; grad_gi(x, i, grad_i); }
-    void eval_hess_L_prod(crvec x, crvec y, crvec v, rvec Hv) const { ScopedMallocAllower ma; hess_L_prod(x, y, v, Hv); }
-    void eval_hess_L(crvec x, crvec y, rmat H) const { ScopedMallocAllower ma; hess_L(x, y, H); }
-    // clang-format on
+void print_provided_functions(std::ostream &os, const TypeErasedProblem<Conf> &problem) {
+    os << "inactive_indices_res_lna: " << problem.provides_eval_inactive_indices_res_lna() << '\n'
+       << "                 grad_gi: " << problem.provides_eval_grad_gi() << '\n'
+       << "                   jac_g: " << problem.provides_eval_jac_g() << '\n'
+       << "             hess_L_prod: " << problem.provides_eval_hess_L_prod() << '\n'
+       << "                  hess_L: " << problem.provides_eval_hess_L() << '\n'
+       << "             hess_ψ_prod: " << problem.provides_eval_hess_ψ_prod() << '\n'
+       << "                  hess_ψ: " << problem.provides_eval_hess_ψ() << '\n'
+       << "                f_grad_f: " << problem.provides_eval_f_grad_f() << '\n'
+       << "                     f_g: " << problem.provides_eval_f_g() << '\n'
+       << "      grad_f_grad_g_prod: " << problem.provides_eval_grad_f_grad_g_prod() << '\n'
+       << "                  grad_L: " << problem.provides_eval_grad_L() << '\n'
+       << "                       ψ: " << problem.provides_eval_ψ() << '\n'
+       << "                  grad_ψ: " << problem.provides_eval_grad_ψ() << '\n'
+       << "                ψ_grad_ψ: " << problem.provides_eval_ψ_grad_ψ() << '\n'
+       << "               get_box_C: " << problem.provides_get_box_C() << '\n'
+       << "               get_box_D: " << problem.provides_get_box_D() << '\n'
+       << "                   check: " << problem.provides_check() << '\n';
+}
 
-    /// @see @ref TypeErasedProblem::provides_eval_grad_gi
-    bool provides_eval_grad_gi() const { return bool{grad_gi}; }
-    /// @see @ref TypeErasedProblem::provides_eval_hess_L_prod
-    bool provides_eval_hess_L_prod() const { return bool{hess_L_prod}; }
-    /// @see @ref TypeErasedProblem::provides_eval_hess_L
-    bool provides_eval_hess_L() const { return bool{hess_L}; }
-
-    FunctionalProblem(const FunctionalProblem &)                = default;
-    FunctionalProblem &operator=(const FunctionalProblem &)     = default;
-    FunctionalProblem(FunctionalProblem &&) noexcept            = default;
-    FunctionalProblem &operator=(FunctionalProblem &&) noexcept = default;
-};
+/// @}
 
 } // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/structured-panoc-alm.hpp` & `alpaqa-1.0.0a7/src/alpaqa/src/panoc-alm.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-#pragma once
-
-#include <alpaqa/inner/directions/panoc/structured-lbfgs.hpp>
-#include <alpaqa/inner/panoc.hpp>
-#include <alpaqa/outer/alm.hpp>
+#include <alpaqa/implementation/inner/panoc.tpp>
+#include <alpaqa/implementation/outer/alm.tpp>
+#include <alpaqa/panoc-alm.hpp>
 
 namespace alpaqa {
 
 // clang-format off
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGS<DefaultConfig>>);
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGS<EigenConfigf>>);
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGS<EigenConfigd>>);
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGS<EigenConfigl>>);
+ALPAQA_EXPORT_TEMPLATE(class, PANOCSolver, LBFGSDirection<DefaultConfig>);
+ALPAQA_EXPORT_TEMPLATE(class, PANOCSolver, LBFGSDirection<EigenConfigf>);
+ALPAQA_EXPORT_TEMPLATE(class, PANOCSolver, LBFGSDirection<EigenConfigd>);
+ALPAQA_EXPORT_TEMPLATE(class, PANOCSolver, LBFGSDirection<EigenConfigl>);
+#ifdef ALPAQA_WITH_QUAD_PRECISION
+ALPAQA_EXPORT_TEMPLATE(class, PANOCSolver, LBFGSDirection<EigenConfigq>);
+#endif
+
+ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGSDirection<DefaultConfig>>);
+ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGSDirection<EigenConfigf>>);
+ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGSDirection<EigenConfigd>>);
+ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGSDirection<EigenConfigl>>);
 #ifdef ALPAQA_WITH_QUAD_PRECISION
-ALPAQA_EXPORT_EXTERN_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGS<EigenConfigq>>);
+ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGSDirection<EigenConfigq>>);
 #endif
 // clang-format on
 
-} // namespace alpaqa
+} // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/util/alloc-check.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/alloc-check.hpp`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/util/atomic-stop-signal.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/atomic-stop-signal.hpp`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/util/check-dim.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/check-dim.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #pragma once
 
 #include <alpaqa/config/config.hpp>
+#include <optional>
 #include <stdexcept>
 #include <string>
 
 namespace alpaqa::util {
 
 template <Config Conf>
 void check_dim_msg(crvec<Conf> v, auto sz, std::string msg) {
@@ -15,17 +16,31 @@
         msg += std::to_string(v.size());
         msg += ")";
         throw std::invalid_argument(msg);
     }
 }
 
 template <Config Conf>
-void check_dim(std::string name, crvec<Conf> v, auto sz) {
+void check_dim_msg(std::optional<vec<Conf>> &v, auto sz, std::string msg) {
+    if (!v) {
+        v = vec<Conf>::Zero(sz);
+    } else if (v->size() != sz) {
+        msg += "\n(should be ";
+        msg += std::to_string(sz);
+        msg += ", got ";
+        msg += std::to_string(v->size());
+        msg += ")";
+        throw std::invalid_argument(msg);
+    }
+}
+
+template <Config Conf, class V>
+void check_dim(std::string name, V &&v, auto sz) {
     name += ": dimension mismatch";
-    check_dim_msg<Conf>(v, sz, name);
+    check_dim_msg<Conf>(std::forward<V>(v), sz, name);
 }
 
 template <Config Conf>
 void check_dim_msg(crmat<Conf> m, auto rows, auto cols, std::string msg) {
     if (m.cols() != cols || m.rows() != rows) {
         msg += "\n(should be ";
         msg += std::to_string(rows);
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/util/copyable_unique_ptr.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/copyable_unique_ptr.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -19,12 +19,14 @@
 
     operator std::unique_ptr<T> &() & { return ptr; }
     operator const std::unique_ptr<T> &() const & { return ptr; }
     operator std::unique_ptr<T> &&() && { return std::move(ptr); }
 
     std::unique_ptr<T> &operator->() { return ptr; }
     const std::unique_ptr<T> &operator->() const { return ptr; }
+    auto &operator*() { return *ptr; }
+    auto &operator*() const { return *ptr; }
 
     std::unique_ptr<T> ptr;
 };
 
 } // namespace alpaqa::util
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/util/float.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/float.hpp`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/util/index-set.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/index-set.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #pragma once
 
 #include <alpaqa/config/config.hpp>
+#include <span>
 
 namespace alpaqa::detail {
 
 template <Config Conf>
 struct IndexSet {
     USING_ALPAQA_CONFIG(Conf);
 
@@ -26,52 +27,71 @@
 
     crindexvec compl_indices(index_t i) const {
         length_t nJ = sizes()(i);
         length_t nK = n - nJ;
         return indices().segment(n * i + nJ, nK);
     }
 
+    // Compute the complement of the index set `in`. Write the indices not in
+    // the input to 'out'.
+    static void compute_complement(std::span<const index_t> in,
+                                   std::span<index_t> out) {
+        compute_complement(in, out.data(),
+                           static_cast<length_t>(in.size() + out.size()));
+    }
+    static void compute_complement(std::span<const index_t> in,
+                                   std::span<index_t> out, length_t n) {
+        assert(in.size() + out.size() == static_cast<size_t>(n));
+        compute_complement(in, out.data(), n);
+    }
+    static void compute_complement(crindexvec in, rindexvec out, length_t n) {
+        assert(in.size() + out.size() == n);
+        compute_complement(std::span{in.data(), static_cast<size_t>(in.size())},
+                           out.data(), n);
+    }
+
     template <class F>
     void update(const F &condition) {
         // Evaluate the condition for all indices in the given 'time_step',
         // append the indices evaluating to true to 'out', and return the number
         // of indices that were appended.
         auto build_Jt = [&](index_t time_step, index_t *out) {
             index_t j = 0; // index into the array of inactive indices
             for (index_t c = 0; c < n; ++c) { // components within time step
                 if (condition(time_step, c))  // if the component is active,
                     out[j++] = c; // append the index of this component to J
             }
             return j; // return the number of elements in J
         };
-        // Compute the complement of the index set defined by the range
-        // 'in' and 'n_in'. Append the indices not in the input to 'out'.
-        auto complement = [&](const index_t *in, length_t n_in, index_t *out) {
-            length_t c = 0; // components within time step
-            length_t k = 0; // index into the array of active indices
-            // iterate over the array with indices 'in'
-            for (index_t i = 0; i < n_in; ++i) { //
-                index_t j = in[i];
-                for (; c < j; ++c) // for all indices not in J
-                    out[k++] = c;  // append the index of this component
-                ++c;               // skip indices in J, i.e. c == j
-            }
-            // add final indices not in J
-            for (; c < n; ++c)
-                out[k++] = c;
-        };
 
         auto sizes    = this->sizes();
         auto *indices = this->indices().data();
         for (index_t t = 0; t < N; ++t) { // time steps
             // Generate the set of inactive indices, J
             index_t num_J = build_Jt(t, indices);
             sizes(t)      = num_J; // save number of inactive indices for later
+            std::span J{indices, static_cast<size_t>(num_J)};
             // Generate the complement, the set of active indices, K
-            complement(indices, num_J, indices + num_J);
+            compute_complement(J, indices + num_J, n);
             // Prepare for next time step
             indices += n;
         }
     }
+
+  private:
+    static void compute_complement(std::span<const index_t> in, index_t *out,
+                                   length_t n) {
+        length_t c = 0; // components within time step
+        length_t k = 0; // index into the array of active indices
+        // iterate over the array with indices 'in'
+        for (index_t j : in) { //
+            for (; c < j; ++c) // for all indices not in J
+                out[k++] = c;  // append the index of this component
+            ++c;               // skip indices in J, i.e. c == j
+        }
+        // add final indices not in J
+        for (; c < n; ++c)
+            out[k++] = c;
+    }
 };
 
 } // namespace alpaqa::detail
```

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/util/max-history.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/max-history.hpp`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/util/quadmath/quadmath.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/quadmath/quadmath.hpp`

 * *Files identical despite different names*

### Comparing `alpaqa-1.0.0a6/src/include/alpaqa/util/type-traits.hpp` & `alpaqa-1.0.0a7/src/alpaqa/include/alpaqa/util/type-traits.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #pragma once
 
+#include <concepts>
+#include <memory>
 #include <type_traits>
 
 namespace alpaqa::util {
 
 template <class M>
 struct class_from_member_ptr_impl {};
 
@@ -31,8 +33,26 @@
 template <class Only>
 struct last_type<Only> {
     using type = Only;
 };
 template <class... Pack>
 using last_type_t = typename last_type<Pack...>::type;
 
+template <class... Pack>
+struct first_type_or_void;
+template <class First, class... Pack>
+struct first_type_or_void<First, Pack...> {
+    using type = First;
+};
+template <>
+struct first_type_or_void<> {
+    using type = void;
+};
+template <class... Pack>
+using first_type_or_void_t = typename first_type_or_void<Pack...>::type;
+
+template <class... Pack>
+concept no_leading_allocator = !
+std::is_same_v<std::remove_cvref_t<first_type_or_void_t<Pack...>>,
+               std::allocator_arg_t>;
+
 } // namespace alpaqa::util
```

### Comparing `alpaqa-1.0.0a6/src/src/accelerators/lbfgs.cpp` & `alpaqa-1.0.0a7/src/alpaqa/src/accelerators/lbfgs.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include <alpaqa/config/config.hpp>
 
-#include <alpaqa/accelerators/src/lbfgs.tpp>
+#include <alpaqa/implementation/accelerators/lbfgs.tpp>
 
 namespace alpaqa {
 
 ALPAQA_EXPORT_TEMPLATE(struct, CBFGSParams, DefaultConfig);
 ALPAQA_EXPORT_TEMPLATE(struct, CBFGSParams, EigenConfigf);
 ALPAQA_EXPORT_TEMPLATE(struct, CBFGSParams, EigenConfigd);
 ALPAQA_EXPORT_TEMPLATE(struct, CBFGSParams, EigenConfigl);
```

### Comparing `alpaqa-1.0.0a6/src/src/inner/panoc-ocp.cpp` & `alpaqa-1.0.0a7/src/alpaqa/src/inner/panoc-ocp.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <alpaqa/inner/src/panoc-ocp.tpp>
+#include <alpaqa/implementation/inner/panoc-ocp.tpp>
 
 namespace alpaqa {
 
 ALPAQA_EXPORT_TEMPLATE(struct, PANOCOCPProgressInfo, DefaultConfig);
 ALPAQA_EXPORT_TEMPLATE(struct, PANOCOCPProgressInfo, EigenConfigf);
 ALPAQA_EXPORT_TEMPLATE(struct, PANOCOCPProgressInfo, EigenConfigd);
 ALPAQA_EXPORT_TEMPLATE(struct, PANOCOCPProgressInfo, EigenConfigl);
```

### Comparing `alpaqa-1.0.0a6/src/src/inner/panoc.cpp` & `alpaqa-1.0.0a7/src/alpaqa/src/inner/panoc.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#include <alpaqa/inner/src/panoc.tpp>
+#include <alpaqa/implementation/inner/panoc.tpp>
 
 namespace alpaqa {
 
 ALPAQA_EXPORT_TEMPLATE(struct, PANOCParams, DefaultConfig);
 ALPAQA_EXPORT_TEMPLATE(struct, PANOCParams, EigenConfigf);
 ALPAQA_EXPORT_TEMPLATE(struct, PANOCParams, EigenConfigd);
 ALPAQA_EXPORT_TEMPLATE(struct, PANOCParams, EigenConfigl);
```

### Comparing `alpaqa-1.0.0a6/src/src/panoc-alm.cpp` & `alpaqa-1.0.0a7/src/interop/lbfgspp/src/lbfgsb-adapter.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-#include <alpaqa/inner/src/panoc.tpp>
-#include <alpaqa/outer/src/alm.tpp>
-#include <alpaqa/panoc-alm.hpp>
+#include <alpaqa/implementation/lbfgsb-adapter.tpp>
 
-namespace alpaqa {
+namespace alpaqa::lbfgspp {
 
-ALPAQA_EXPORT_TEMPLATE(class, PANOCSolver, LBFGS<DefaultConfig>);
-ALPAQA_EXPORT_TEMPLATE(class, PANOCSolver, LBFGS<EigenConfigf>);
-ALPAQA_EXPORT_TEMPLATE(class, PANOCSolver, LBFGS<EigenConfigd>);
-ALPAQA_EXPORT_TEMPLATE(class, PANOCSolver, LBFGS<EigenConfigl>);
+ALPAQA_LBFGSPP_EXPORT_TEMPLATE(struct, LBFGSBStats, DefaultConfig);
+ALPAQA_LBFGSPP_EXPORT_TEMPLATE(struct, LBFGSBStats, EigenConfigf);
+ALPAQA_LBFGSPP_EXPORT_TEMPLATE(struct, LBFGSBStats, EigenConfigd);
+ALPAQA_LBFGSPP_EXPORT_TEMPLATE(struct, LBFGSBStats, EigenConfigl);
 #ifdef ALPAQA_WITH_QUAD_PRECISION
-ALPAQA_EXPORT_TEMPLATE(class, PANOCSolver, LBFGS<EigenConfigq>);
+ALPAQA_LBFGSPP_EXPORT_TEMPLATE(struct, LBFGSBStats, EigenConfigq);
 #endif
 
-ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGS<DefaultConfig>>);
-ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGS<EigenConfigf>>);
-ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGS<EigenConfigd>>);
-ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGS<EigenConfigl>>);
+ALPAQA_LBFGSPP_EXPORT_TEMPLATE(class, LBFGSBSolver, DefaultConfig);
+ALPAQA_LBFGSPP_EXPORT_TEMPLATE(class, LBFGSBSolver, EigenConfigf);
+ALPAQA_LBFGSPP_EXPORT_TEMPLATE(class, LBFGSBSolver, EigenConfigd);
+ALPAQA_LBFGSPP_EXPORT_TEMPLATE(class, LBFGSBSolver, EigenConfigl);
 #ifdef ALPAQA_WITH_QUAD_PRECISION
-ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<LBFGS<EigenConfigq>>);
+ALPAQA_LBFGSPP_EXPORT_TEMPLATE(class, LBFGSBSolver, EigenConfigq);
 #endif
 
-} // namespace alpaqa
+} // namespace alpaqa::lbfgspp
```

### Comparing `alpaqa-1.0.0a6/src/src/structured-panoc-alm.cpp` & `alpaqa-1.0.0a7/src/alpaqa/src/inner/directions/panoc/structured-lbfgs.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-#include <alpaqa/inner/directions/panoc/src/structured-lbfgs.tpp>
-#include <alpaqa/inner/src/panoc.tpp>
-#include <alpaqa/outer/src/alm.tpp>
-#include <alpaqa/structured-panoc-alm.hpp>
+#include <alpaqa/implementation/inner/directions/panoc/structured-lbfgs.tpp>
 
 namespace alpaqa {
 
-// clang-format off
-ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGS<DefaultConfig>>);
-ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGS<EigenConfigf>>);
-ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGS<EigenConfigd>>);
-ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGS<EigenConfigl>>);
+ALPAQA_EXPORT_TEMPLATE(struct, StructuredLBFGSDirection, DefaultConfig);
+ALPAQA_EXPORT_TEMPLATE(struct, StructuredLBFGSDirection, EigenConfigf);
+ALPAQA_EXPORT_TEMPLATE(struct, StructuredLBFGSDirection, EigenConfigd);
+ALPAQA_EXPORT_TEMPLATE(struct, StructuredLBFGSDirection, EigenConfigl);
 #ifdef ALPAQA_WITH_QUAD_PRECISION
-ALPAQA_EXPORT_TEMPLATE(class, ALMSolver, PANOCSolver<StructuredLBFGS<EigenConfigq>>);
+ALPAQA_EXPORT_TEMPLATE(struct, StructuredLBFGSDirection, EigenConfigq);
 #endif
-// clang-format on
 
 } // namespace alpaqa
```

### Comparing `alpaqa-1.0.0a6/PKG-INFO` & `alpaqa-1.0.0a7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: alpaqa
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: Augmented Lagrangian and PANOC solvers for nonconvex numerical optimization.
 Keywords: optimization,panoc,alm,mpc
 Author-email: Pieter P <pieter.p.dev@outlook.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Dist: numpy
-Requires-Dist: casadi
-Requires-Dist: sphinx~=5.1 ; extra == "docs"
+Requires-Dist: casadi~=3.6.0
+Requires-Dist: alpaqa-debug==1.0.0a7 ; extra == "debug"
+Requires-Dist: sphinx>=5.1,<7.1 ; extra == "docs"
 Requires-Dist: matplotlib ; extra == "docs"
 Requires-Dist: breathe ; extra == "docs"
 Requires-Dist: furo ; extra == "docs"
+Requires-Dist: pytest>=7.2.0,<7.5 ; extra == "test"
+Requires-Dist: qpalm~=1.1.4 ; extra == "test"
+Requires-Dist: scipy>=1.9.3,<1.12 ; extra == "test"
 Project-URL: Bug Tracker, https://github.com/kul-optec/alpaqa/issues
 Project-URL: Documentation, https://kul-optec.github.io/alpaqa
 Project-URL: Source, https://github.com/kul-optec/alpaqa
+Provides-Extra: debug
 Provides-Extra: docs
+Provides-Extra: test
 
 alpaqa
 ======
 
 ``alpaqa`` is an efficient implementation of an augmented Lagrangian method for
 general nonlinear programming problems, which uses the first-order, matrix-free
 PANOC algorithm as an inner solver.
@@ -50,15 +55,15 @@
         &&& \underline{z} \le g(x) \le \overline{z} &&&& g : {{\rm I\mathchoice{\hspace{-2pt}}{\hspace{-2pt}}{\hspace{-1.75pt}}{\hspace{-1.7pt}}R}}^n \rightarrow {{\rm I\mathchoice{\hspace{-2pt}}{\hspace{-2pt}}{\hspace{-1.75pt}}{\hspace{-1.7pt}}R}}^m
     \end{aligned}
 
 Documentation
 -------------
 
 - `Sphinx documentation <https://kul-optec.github.io/alpaqa/develop/Sphinx/index.html>`_
-- `Python examples <https://kul-optec.github.io/alpaqa/develop/Sphinx/examples/examples_landing_page.html>`_
+- `Python examples <https://kul-optec.github.io/alpaqa/develop/Sphinx/examples/index.html>`_
 - `Doxygen documentation <https://kul-optec.github.io/alpaqa/develop/Doxygen/index.html>`_
 - `C++ examples <https://kul-optec.github.io/alpaqa/develop/Doxygen/examples.html>`_
 
 Installation
 ------------
 
 The Python interface can be installed directly from PyPI:
```

