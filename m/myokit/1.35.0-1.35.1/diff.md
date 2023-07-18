# Comparing `tmp/myokit-1.35.0.tar.gz` & `tmp/myokit-1.35.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myokit-1.35.0.tar", last modified: Wed Jun 21 11:10:29 2023, max compression
+gzip compressed data, was "myokit-1.35.1.tar", last modified: Tue Jul 18 23:29:26 2023, max compression
```

## Comparing `myokit-1.35.0.tar` & `myokit-1.35.1.tar`

### file list

```diff
@@ -1,454 +1,458 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.836466 myokit-1.35.0/
--rw-r--r--   0 michael   (1000) michael   (1000)     1833 2023-06-07 13:48:59.000000 myokit-1.35.0/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-06-07 13:48:23.000000 myokit-1.35.0/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     5059 2023-06-21 11:10:29.836466 myokit-1.35.0/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     3821 2023-06-07 13:48:59.000000 myokit-1.35.0/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.803465 myokit-1.35.0/myokit/
--rw-r--r--   0 michael   (1000) michael   (1000)    14173 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    58017 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23743 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_aux.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.803465 myokit-1.35.0/myokit/_bin/
--rw-r--r--   0 michael   (1000) michael   (1000)     6226 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/example.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.806465 myokit-1.35.0/myokit/_bin/gui/
--rw-r--r--   0 michael   (1000) michael   (1000)      784 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/find.png
--rw-r--r--   0 michael   (1000) michael   (1000)    96412 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-128.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     3528 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-16.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-24.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   233500 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-256.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    12232 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-32.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    23817 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-48.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    36761 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-64.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    65257 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-96.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer.ico
--rw-r--r--   0 michael   (1000) michael   (1000)    30396 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer.png
--rw-r--r--   0 michael   (1000) michael   (1000)    47406 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-128.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     2987 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-16.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     4971 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-24.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   152751 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-256.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     7355 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-32.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     9835 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-48.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    16235 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-64.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    30683 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide-96.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide.ico
--rw-r--r--   0 michael   (1000) michael   (1000)    15096 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/icon-ide.png
--rw-r--r--   0 michael   (1000) michael   (1000)      571 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/new.png
--rw-r--r--   0 michael   (1000) michael   (1000)      544 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/open.png
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/redo.png
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/run.png
--rw-r--r--   0 michael   (1000) michael   (1000)      565 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/save.png
--rw-r--r--   0 michael   (1000) michael   (1000)      284 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/_bin/gui/undo.png
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.807466 myokit-1.35.0/myokit/_bin/install-lin/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      254 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/_bin/install-lin/myokit-datablock-viewer.desktop
--rwxr-xr-x   0 michael   (1000) michael   (1000)      266 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/_bin/install-lin/myokit-datalog-viewer.desktop
--rwxr-xr-x   0 michael   (1000) michael   (1000)      264 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/install-lin/myokit-ide.desktop
--rw-r--r--   0 michael   (1000) michael   (1000)     4338 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/_bin/install-lin/myokit.lang
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-07 13:47:50.000000 myokit-1.35.0/myokit/_bin/install-lin/x-abf.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      246 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/install-lin/x-cellml.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      247 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/_bin/install-lin/x-myokit.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      275 2023-06-07 13:47:50.000000 myokit-1.35.0/myokit/_bin/install-lin/x-wcp.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.807466 myokit-1.35.0/myokit/_bin/install-win/
--rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_bin/install-win/menu.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.807466 myokit-1.35.0/myokit/_bin/sundials-win-vs/
--rw-r--r--   0 michael   (1000) michael   (1000)     1758 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/LICENSE
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.799466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.807466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/
--rw-r--r--   0 michael   (1000) michael   (1000)    27506 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h
--rw-r--r--   0 michael   (1000) michael   (1000)     2427 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h
--rw-r--r--   0 michael   (1000) michael   (1000)    12344 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.807466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/nvector/
--rw-r--r--   0 michael   (1000) michael   (1000)     8934 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.808466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/
--rw-r--r--   0 michael   (1000) michael   (1000)     5785 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h
--rw-r--r--   0 michael   (1000) michael   (1000)     8997 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h
--rw-r--r--   0 michael   (1000) michael   (1000)    13330 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h
--rw-r--r--   0 michael   (1000) michael   (1000)     1024 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h
--rw-r--r--   0 michael   (1000) michael   (1000)    10283 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h
--rw-r--r--   0 michael   (1000) michael   (1000)     9385 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5420 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h
--rw-r--r--   0 michael   (1000) michael   (1000)     9190 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h
--rw-r--r--   0 michael   (1000) michael   (1000)    12559 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5165 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h
--rw-r--r--   0 michael   (1000) michael   (1000)     1266 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.808466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunlinsol/
--rw-r--r--   0 michael   (1000) michael   (1000)     2983 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.808466 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunmatrix/
--rw-r--r--   0 michael   (1000) michael   (1000)     3647 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.809466 myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/
--rw-r--r--   0 michael   (1000) michael   (1000)   677888 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll
--rw-r--r--   0 michael   (1000) michael   (1000)   169196 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib
--rw-r--r--   0 michael   (1000) michael   (1000)   160768 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll
--rw-r--r--   0 michael   (1000) michael   (1000)    59576 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib
--rw-r--r--   0 michael   (1000) michael   (1000)    12048 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_config.py
--rw-r--r--   0 michael   (1000) michael   (1000)    66499 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_datablock.py
--rw-r--r--   0 michael   (1000) michael   (1000)    67472 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_datalog.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11060 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_err.py
--rw-r--r--   0 michael   (1000) michael   (1000)   103962 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_expressions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8948 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_io.py
--rw-r--r--   0 michael   (1000) michael   (1000)   193097 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_model_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)      726 2023-06-21 10:54:06.000000 myokit-1.35.0/myokit/_myokit_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)    74065 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_parsing.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4410 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_progress.py
--rw-r--r--   0 michael   (1000) michael   (1000)    30572 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_protocol.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.811466 myokit-1.35.0/myokit/_sim/
--rw-r--r--   0 michael   (1000) michael   (1000)    13412 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19150 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)    18810 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cable.py
--rw-r--r--   0 michael   (1000) michael   (1000)    38703 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cmodel.h
--rw-r--r--   0 michael   (1000) michael   (1000)    15775 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cmodel.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4047 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_sim/compiler.c
--rw-r--r--   0 michael   (1000) michael   (1000)     2664 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/compiler.py
--rw-r--r--   0 michael   (1000) michael   (1000)    71253 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cvodessim.c
--rw-r--r--   0 michael   (1000) michael   (1000)    42507 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/cvodessim.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15446 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/differential.hpp
--rw-r--r--   0 michael   (1000) michael   (1000)    47438 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/fiber_tissue.c
--rw-r--r--   0 michael   (1000) michael   (1000)    50694 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/fiber_tissue.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8012 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/jacobian.cpp
--rw-r--r--   0 michael   (1000) michael   (1000)    12957 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/jacobian.py
--rw-r--r--   0 michael   (1000) michael   (1000)    32352 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/mcl.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5037 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_sim/opencl.c
--rw-r--r--   0 michael   (1000) michael   (1000)    16446 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/opencl.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46535 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/openclsim.c
--rw-r--r--   0 michael   (1000) michael   (1000)    19360 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/openclsim.cl
--rw-r--r--   0 michael   (1000) michael   (1000)    69220 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/openclsim.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29511 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/pacing.h
--rw-r--r--   0 michael   (1000) michael   (1000)    10914 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/rhs.c
--rw-r--r--   0 michael   (1000) michael   (1000)     7392 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/rhs.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1720 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/_sim/sundials.c
--rw-r--r--   0 michael   (1000) michael   (1000)     2972 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_sim/sundials.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4602 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_system.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29848 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/_unit.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3066 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/float.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.811466 myokit-1.35.0/myokit/formats/
--rw-r--r--   0 michael   (1000) michael   (1000)    20096 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.812466 myokit-1.35.0/myokit/formats/ansic/
--rw-r--r--   0 michael   (1000) michael   (1000)     3347 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/ansic/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3566 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/ansic/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5361 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/ansic/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.812466 myokit-1.35.0/myokit/formats/ansic/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    11965 2023-06-20 10:29:46.000000 myokit-1.35.0/myokit/formats/ansic/template/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)     6044 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/ansic/template/euler.c
--rw-r--r--   0 michael   (1000) michael   (1000)    14244 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/ansic/template/sim.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.812466 myokit-1.35.0/myokit/formats/axon/
--rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/axon/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    69921 2023-06-21 10:30:12.000000 myokit-1.35.0/myokit/formats/axon/_abf.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10165 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/axon/_atf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      833 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/axon/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.812466 myokit-1.35.0/myokit/formats/cellml/
--rw-r--r--   0 michael   (1000) michael   (1000)     1466 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2719 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2283 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2229 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.813466 myokit-1.35.0/myokit/formats/cellml/v1/
--rw-r--r--   0 michael   (1000) michael   (1000)      608 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v1/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59011 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v1/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)    43554 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v1/_parser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15055 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v1/_writer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.813466 myokit-1.35.0/myokit/formats/cellml/v2/
--rw-r--r--   0 michael   (1000) michael   (1000)      598 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v2/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59012 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v2/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29536 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v2/_parser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11994 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cellml/v2/_writer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.813466 myokit-1.35.0/myokit/formats/channelml/
--rw-r--r--   0 michael   (1000) michael   (1000)      443 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/channelml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    14605 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/channelml/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.814466 myokit-1.35.0/myokit/formats/cpp/
--rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cpp/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      421 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cpp/_ewriter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.814466 myokit-1.35.0/myokit/formats/cuda/
--rw-r--r--   0 michael   (1000) michael   (1000)      816 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cuda/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4472 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cuda/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2059 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cuda/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.814466 myokit-1.35.0/myokit/formats/cuda/template/
--rw-r--r--   0 michael   (1000) michael   (1000)     8863 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/cuda/template/kernel.cu
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.814466 myokit-1.35.0/myokit/formats/easyml/
--rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/easyml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3482 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/easyml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15771 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/easyml/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.814466 myokit-1.35.0/myokit/formats/html/
--rw-r--r--   0 michael   (1000) michael   (1000)      457 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/html/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2343 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/html/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6606 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/html/_flatten.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.815466 myokit-1.35.0/myokit/formats/latex/
--rw-r--r--   0 michael   (1000) michael   (1000)      682 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/latex/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6690 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/latex/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5117 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/latex/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.815466 myokit-1.35.0/myokit/formats/mathml/
--rw-r--r--   0 michael   (1000) michael   (1000)      637 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/mathml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    12194 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/mathml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)    34289 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/mathml/_parser.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.815466 myokit-1.35.0/myokit/formats/matlab/
--rw-r--r--   0 michael   (1000) michael   (1000)      695 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/matlab/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3172 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/matlab/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2868 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/matlab/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.815466 myokit-1.35.0/myokit/formats/matlab/template/
--rw-r--r--   0 michael   (1000) michael   (1000)      528 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/formats/matlab/template/constants.m
--rw-r--r--   0 michael   (1000) michael   (1000)      374 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/formats/matlab/template/ifthenelse.m
--rw-r--r--   0 michael   (1000) michael   (1000)     2095 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/formats/matlab/template/main.m
--rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/formats/matlab/template/model.m
--rw-r--r--   0 michael   (1000) michael   (1000)      461 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/formats/matlab/template/model_wrapper.m
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.816466 myokit-1.35.0/myokit/formats/opencl/
--rw-r--r--   0 michael   (1000) michael   (1000)     6962 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/opencl/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5261 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/opencl/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3903 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/opencl/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.816466 myokit-1.35.0/myokit/formats/opencl/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    11633 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/formats/opencl/template/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)     8158 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/opencl/template/kernel.cl
--rw-r--r--   0 michael   (1000) michael   (1000)     9018 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/formats/opencl/template/minilog.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1042 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/formats/opencl/template/plot.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      162 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/formats/opencl/template/test.sh
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.816466 myokit-1.35.0/myokit/formats/python/
--rw-r--r--   0 michael   (1000) michael   (1000)     1049 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/python/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6751 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/python/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)      969 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/python/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.816466 myokit-1.35.0/myokit/formats/python/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    10311 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/python/template/sim.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.817466 myokit-1.35.0/myokit/formats/sbml/
--rw-r--r--   0 michael   (1000) michael   (1000)      653 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sbml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59396 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sbml/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)      987 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sbml/_importer.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29181 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sbml/_parser.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.817466 myokit-1.35.0/myokit/formats/stan/
--rw-r--r--   0 michael   (1000) michael   (1000)     2877 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/stan/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3102 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/stan/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3745 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/stan/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.817466 myokit-1.35.0/myokit/formats/stan/template/
--rw-r--r--   0 michael   (1000) michael   (1000)     5305 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/stan/template/cell.stan
--rwxr-xr-x   0 michael   (1000) michael   (1000)       92 2023-02-05 15:45:10.000000 myokit-1.35.0/myokit/formats/stan/template/run.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.817466 myokit-1.35.0/myokit/formats/sympy/
--rw-r--r--   0 michael   (1000) michael   (1000)     1638 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sympy/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6758 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sympy/_ereader.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4875 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/sympy/_ewriter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.818466 myokit-1.35.0/myokit/formats/wcp/
--rw-r--r--   0 michael   (1000) michael   (1000)      254 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/wcp/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10234 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/wcp/_wcp.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.818466 myokit-1.35.0/myokit/formats/xml/
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/xml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1494 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/xml/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)      393 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/formats/xml/_split.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.819466 myokit-1.35.0/myokit/gui/
--rw-r--r--   0 michael   (1000) michael   (1000)     6154 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46576 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/datablock_viewer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    32560 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/datalog_viewer.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8588 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/explorer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)   108238 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/ide.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2157 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/progress.py
--rw-r--r--   0 michael   (1000) michael   (1000)    52418 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/source.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6072 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/gui/vargrapher.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.819466 myokit-1.35.0/myokit/lib/
--rw-r--r--   0 michael   (1000) michael   (1000)      216 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/lib/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23859 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/deps.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28056 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/guess.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46678 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/hh.py
--rw-r--r--   0 michael   (1000) michael   (1000)    67773 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/markov.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4408 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/multi.py
--rw-r--r--   0 michael   (1000) michael   (1000)    13874 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/lib/plots.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4552 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/pacing.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8230 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/pype.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.826466 myokit-1.35.0/myokit/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2697 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/ansic_event_based_pacing.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1244 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/ansic_fixed_form_pacing.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.827466 myokit-1.35.0/myokit/tests/data/
--rw-r--r--   0 michael   (1000) michael   (1000)     3022 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-model-compare-a.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     2889 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-model-compare-b.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3137 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-model.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-protocol.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-script.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3287 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/beeler-1977-units.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     5091 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/clancy-1999-fitting.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3128 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/conditional.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6067 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/cv1d.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/cv1d.zip
--rw-r--r--   0 michael   (1000) michael   (1000)    23916 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/decker-2009.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)    18350 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/decker.model
--rw-r--r--   0 michael   (1000) michael   (1000)    10416 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/dn-1985-normalised.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      800 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/dom-markov.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.828466 myokit-1.35.0/myokit/tests/data/formats/
--rw-r--r--   0 michael   (1000) michael   (1000)     8192 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/abf-protocol.pro
--rw-r--r--   0 michael   (1000) michael   (1000)    98376 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/abf-v1.abf
--rw-r--r--   0 michael   (1000) michael   (1000)    24576 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/abf-v2.abf
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.829466 myokit-1.35.0/myokit/tests/data/formats/cellml/
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)    59093 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/br-1977-dot.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    58593 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/br-1977.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)   117223 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/corrias.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)   221953 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/decker-2009.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)     1595 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/documentation.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/invalid-file.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    44837 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    44947 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.830466 myokit-1.35.0/myokit/tests/data/formats/channelml/
--rw-r--r--   0 michael   (1000) michael   (1000)     2648 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      557 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     2702 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     2369 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1258 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1539 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1290 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1374 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1373 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      675 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1398 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1317 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.831466 myokit-1.35.0/myokit/tests/data/formats/sbml/
--rw-r--r--   0 michael   (1000) michael   (1000)     8719 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     9801 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml
--rw-r--r--   0 michael   (1000) michael   (1000)    31408 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/HodgkinHuxley.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/LICENSE
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.831466 myokit-1.35.0/myokit/tests/data/formats/sbml/model/
--rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     2952 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     1226 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.831466 myokit-1.35.0/myokit/tests/data/formats/sbml/result/
--rw-r--r--   0 michael   (1000) michael   (1000)     2457 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/result/00001-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     2206 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/result/00004-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/sbml/result/01103-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)    25600 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/formats/wcp-file.wcp
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.836466 myokit-1.35.0/myokit/tests/data/io/
--rw-r--r--   0 michael   (1000) michael   (1000)      735 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-1-not-enough-files.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109429 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-2-no-header.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   104768 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-3-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-4-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109458 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-5-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1549 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-6-time-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-7-0d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad1d-8-1d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)      739 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-1-not-enough-files.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346240 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-2-no-header.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   333091 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-3-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-4-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346257 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-5-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1553 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-6-time-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1588 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-7-0d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/bad2d-8-2d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)      623 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-1-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1281 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-2-no-structure.zip
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-3-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-4-invalid-n-fields.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-5-invalid-data-size.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1457 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-6-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/badlog-7-not-enough-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     6031 2023-06-07 13:48:59.000000 myokit-1.35.0/myokit/tests/data/io/block2d.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/block2d.zip
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-1-empty.csv
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-10-just-spaces.csv
--rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-11-just-a-semicolon.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-12-bad-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-13-header-with-empty-1.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-14-header-with-empty-2.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-15-header-with-empty-3.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-16-wrong-columns-in-data.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-17-non-float-data.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      112 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-2-windows.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      103 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-3-old-mac.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-4-empty-lines.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-5-semicolons.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-6-open-string.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-7-empty-lines-2.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-8-unquoted-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      114 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog-9-double-quoted-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/datalog.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     1421 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/io/goodlog.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     4992 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/lr-1991-dep.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     2315 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/lr-1991-fitting.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     4571 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/lr-1991-testing.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6124 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/lr-1991.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.836466 myokit-1.35.0/myokit/tests/data/multi/
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/beeler-1977-protocol.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/beeler-1977-script.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/beeler-no-name.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6013 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/lr-1991.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/not-a-model.csv
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.836466 myokit-1.35.0/myokit/tests/data/multi/subdir/
--rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/multi/subdir/beeler-no-name.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3754 2023-06-07 13:48:23.000000 myokit-1.35.0/myokit/tests/data/noble-1962.mmt
--rwxr-xr-x   0 michael   (1000) michael   (1000)    22536 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_aux.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    56981 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v1_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    41869 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v1_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12532 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v1_writer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    73319 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v2_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    26345 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v2_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10977 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cellml_v2_writer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4058 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_cmodel.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      476 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_compiler_detection.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14096 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_component.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11511 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_config.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    49755 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_datablock.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    82813 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_datalog.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    60654 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_dependency_checking.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)   138508 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_expressions.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4882 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_float.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4236 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14876 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_axon.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    19078 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_cellml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6703 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_channelml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11358 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_easyml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     9169 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_exporters.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    40800 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_expression_writers.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3539 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_html.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1531 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_importers.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    37444 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_mathml_content.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8726 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_mathml_presentation.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    17298 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_opencl.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4672 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_sbml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10324 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_sympy.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1786 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_formats_wcp.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14334 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_io.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1821 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_jacobian_calculator.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1767 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_jacobian_tracer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     7476 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_deps.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    42333 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_guess.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    31014 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_hh.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    39983 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_markov.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5145 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_multi.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6062 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_lib_plots.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2829 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_meta.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    84972 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_model.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    16720 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_model_building.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3834 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_opencl_info.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8193 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_pacing_factory.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5161 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_pacing_system_c.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2948 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_pacing_system_py.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    50865 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_parsing.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2762 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_progress_reporters.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    15092 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_protocol.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12565 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_protocol_floating_point.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2318 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_protocol_time_series.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2402 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_pype.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     7353 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_quantity.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3452 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_rhs_benchmarker.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    71633 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_sbml_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    54542 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_sbml_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    17713 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_1d.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    42191 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_cvodes.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1853 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_cvodes_from_disk.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    35421 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_fiber_tissue.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14033 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_log_interval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    59195 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_opencl.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3005 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_opencl_log_interval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    20114 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_opencl_vs_cvode.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5216 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_simulation_opencl_vs_sim1d.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      562 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_system_info.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10358 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_tools.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    13635 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_unit.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1721 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_user_functions.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    33331 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tests/test_variable.py
--rw-r--r--   0 michael   (1000) michael   (1000)    16868 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/tools.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8503 2023-06-20 10:29:48.000000 myokit-1.35.0/myokit/units.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-21 11:10:29.803465 myokit-1.35.0/myokit.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)     5059 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)    15007 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       48 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-01-04 14:18:38.000000 myokit-1.35.0/myokit.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      176 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        7 2023-06-21 11:10:29.000000 myokit-1.35.0/myokit.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-21 11:10:29.837466 myokit-1.35.0/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     3183 2023-06-21 10:33:11.000000 myokit-1.35.0/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.739545 myokit-1.35.1/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1833 2023-07-11 14:14:16.000000 myokit-1.35.1/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-06-07 13:48:23.000000 myokit-1.35.1/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     5059 2023-07-18 23:29:26.739545 myokit-1.35.1/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     3821 2023-06-25 10:52:15.000000 myokit-1.35.1/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.703545 myokit-1.35.1/myokit/
+-rw-r--r--   0 michael   (1000) michael   (1000)    14034 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    57971 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23743 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_aux.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.704545 myokit-1.35.1/myokit/_bin/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6226 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_bin/example.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.707545 myokit-1.35.1/myokit/_bin/gui/
+-rw-r--r--   0 michael   (1000) michael   (1000)      784 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/find.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    96412 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-128.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     3528 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-16.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-24.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   233500 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-256.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    12232 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-32.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    23817 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-48.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    36761 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-64.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    65257 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-96.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)    30396 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    47406 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-ide-128.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     2987 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-ide-16.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     4971 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-ide-24.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   152751 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-ide-256.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     7355 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-ide-32.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     9835 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-ide-48.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    16235 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-ide-64.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    30683 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-ide-96.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-ide.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)    15096 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/icon-ide.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      571 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/new.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      544 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/open.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/redo.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/run.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      565 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/save.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      284 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/_bin/gui/undo.png
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.708545 myokit-1.35.1/myokit/_bin/install-lin/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      254 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/_bin/install-lin/myokit-datablock-viewer.desktop
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      266 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/_bin/install-lin/myokit-datalog-viewer.desktop
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      264 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/install-lin/myokit-ide.desktop
+-rw-r--r--   0 michael   (1000) michael   (1000)     4338 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/_bin/install-lin/myokit.lang
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-07 13:47:50.000000 myokit-1.35.1/myokit/_bin/install-lin/x-abf.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      246 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/install-lin/x-cellml.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      247 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/_bin/install-lin/x-myokit.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      275 2023-06-07 13:47:50.000000 myokit-1.35.1/myokit/_bin/install-lin/x-wcp.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.708545 myokit-1.35.1/myokit/_bin/install-win/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_bin/install-win/menu.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.708545 myokit-1.35.1/myokit/_bin/sundials-win-vs/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1758 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/LICENSE
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.700545 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.708545 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/cvodes/
+-rw-r--r--   0 michael   (1000) michael   (1000)    27506 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     2427 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    12344 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.708545 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/nvector/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8934 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.709545 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5785 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     8997 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    13330 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     1024 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    10283 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     9385 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5420 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     9190 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    12559 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5165 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     1266 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.709545 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sunlinsol/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2983 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.709545 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sunmatrix/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3647 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.710545 myokit-1.35.1/myokit/_bin/sundials-win-vs/lib/
+-rw-r--r--   0 michael   (1000) michael   (1000)   677888 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll
+-rw-r--r--   0 michael   (1000) michael   (1000)   169196 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib
+-rw-r--r--   0 michael   (1000) michael   (1000)   160768 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll
+-rw-r--r--   0 michael   (1000) michael   (1000)    59576 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib
+-rw-r--r--   0 michael   (1000) michael   (1000)    11987 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_config.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    89061 2023-07-18 23:19:29.000000 myokit-1.35.1/myokit/_datablock.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    67472 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_datalog.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11060 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_err.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   103962 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_expressions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8948 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_io.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   193081 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_model_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      726 2023-07-18 23:20:18.000000 myokit-1.35.1/myokit/_myokit_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    74065 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_parsing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4410 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_progress.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    30595 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_protocol.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.712545 myokit-1.35.1/myokit/_sim/
+-rw-r--r--   0 michael   (1000) michael   (1000)    13412 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19156 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_sim/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    18908 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_sim/cable.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    38785 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_sim/cmodel.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    15775 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/cmodel.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4047 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_sim/compiler.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     2664 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/compiler.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    72435 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_sim/cvodessim.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    43186 2023-07-18 22:48:59.000000 myokit-1.35.1/myokit/_sim/cvodessim.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15446 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/differential.hpp
+-rw-r--r--   0 michael   (1000) michael   (1000)    47444 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_sim/fiber_tissue.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    50792 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_sim/fiber_tissue.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8012 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/jacobian.cpp
+-rw-r--r--   0 michael   (1000) michael   (1000)    12957 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/jacobian.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    32352 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/mcl.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5037 2023-06-25 10:43:52.000000 myokit-1.35.1/myokit/_sim/opencl.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    16446 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/opencl.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46541 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_sim/openclsim.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    19360 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/openclsim.cl
+-rw-r--r--   0 michael   (1000) michael   (1000)    69159 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_sim/openclsim.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29888 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/_sim/pacing.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    10914 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/rhs.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     7392 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/rhs.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1720 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/_sim/sundials.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     2972 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_sim/sundials.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4602 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/_system.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29849 2023-07-12 17:16:09.000000 myokit-1.35.1/myokit/_unit.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3066 2023-07-14 13:14:46.000000 myokit-1.35.1/myokit/float.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.712545 myokit-1.35.1/myokit/formats/
+-rw-r--r--   0 michael   (1000) michael   (1000)    26714 2023-07-14 10:16:32.000000 myokit-1.35.1/myokit/formats/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.713545 myokit-1.35.1/myokit/formats/ansic/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3347 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/ansic/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3566 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/ansic/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5361 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/ansic/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.713545 myokit-1.35.1/myokit/formats/ansic/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11965 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/ansic/template/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     6044 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/ansic/template/euler.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    14244 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/ansic/template/sim.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.713545 myokit-1.35.1/myokit/formats/axon/
+-rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/axon/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    74286 2023-07-14 10:16:32.000000 myokit-1.35.1/myokit/formats/axon/_abf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10543 2023-07-12 17:16:09.000000 myokit-1.35.1/myokit/formats/axon/_atf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      826 2023-07-12 17:16:09.000000 myokit-1.35.1/myokit/formats/axon/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.714545 myokit-1.35.1/myokit/formats/cellml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1466 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2719 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2283 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2229 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.714545 myokit-1.35.1/myokit/formats/cellml/v1/
+-rw-r--r--   0 michael   (1000) michael   (1000)      608 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/v1/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59011 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/v1/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    43554 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/v1/_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15055 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/v1/_writer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.714545 myokit-1.35.1/myokit/formats/cellml/v2/
+-rw-r--r--   0 michael   (1000) michael   (1000)      598 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/v2/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59012 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/v2/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29536 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/v2/_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11994 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cellml/v2/_writer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.714545 myokit-1.35.1/myokit/formats/channelml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      443 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/channelml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    14605 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/channelml/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.715545 myokit-1.35.1/myokit/formats/cpp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cpp/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      421 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cpp/_ewriter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.715545 myokit-1.35.1/myokit/formats/cuda/
+-rw-r--r--   0 michael   (1000) michael   (1000)      816 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cuda/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4472 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cuda/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2059 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cuda/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.715545 myokit-1.35.1/myokit/formats/cuda/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8863 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/cuda/template/kernel.cu
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.715545 myokit-1.35.1/myokit/formats/easyml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/easyml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3482 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/easyml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15771 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/easyml/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.715545 myokit-1.35.1/myokit/formats/heka/
+-rw-r--r--   0 michael   (1000) michael   (1000)      761 2023-07-14 10:16:32.000000 myokit-1.35.1/myokit/formats/heka/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1154 2023-07-14 10:16:32.000000 myokit-1.35.1/myokit/formats/heka/_importer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    90645 2023-07-18 23:18:20.000000 myokit-1.35.1/myokit/formats/heka/_patchmaster.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.716545 myokit-1.35.1/myokit/formats/html/
+-rw-r--r--   0 michael   (1000) michael   (1000)      457 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/html/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2343 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/html/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6606 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/html/_flatten.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.716545 myokit-1.35.1/myokit/formats/latex/
+-rw-r--r--   0 michael   (1000) michael   (1000)      682 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/latex/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6690 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/latex/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5117 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/latex/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.716545 myokit-1.35.1/myokit/formats/mathml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      637 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/mathml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    12194 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/mathml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    34289 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/mathml/_parser.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.716545 myokit-1.35.1/myokit/formats/matlab/
+-rw-r--r--   0 michael   (1000) michael   (1000)      695 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/matlab/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3172 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/matlab/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2868 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/matlab/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.717545 myokit-1.35.1/myokit/formats/matlab/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)      528 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/formats/matlab/template/constants.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      374 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/formats/matlab/template/ifthenelse.m
+-rw-r--r--   0 michael   (1000) michael   (1000)     2095 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/matlab/template/main.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/formats/matlab/template/model.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      461 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/formats/matlab/template/model_wrapper.m
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.717545 myokit-1.35.1/myokit/formats/opencl/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6962 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/opencl/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5261 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/opencl/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3903 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/opencl/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.717545 myokit-1.35.1/myokit/formats/opencl/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11633 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/opencl/template/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     8158 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/opencl/template/kernel.cl
+-rw-r--r--   0 michael   (1000) michael   (1000)     9018 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/opencl/template/minilog.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1042 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/formats/opencl/template/plot.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      162 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/opencl/template/test.sh
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.718545 myokit-1.35.1/myokit/formats/python/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1049 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/python/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6751 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/python/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      969 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/python/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.718545 myokit-1.35.1/myokit/formats/python/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    10311 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/python/template/sim.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.718545 myokit-1.35.1/myokit/formats/sbml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      653 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/sbml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59396 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/sbml/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      987 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/sbml/_importer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29181 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/sbml/_parser.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.718545 myokit-1.35.1/myokit/formats/stan/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2877 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/stan/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3102 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/stan/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3745 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/stan/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.718545 myokit-1.35.1/myokit/formats/stan/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5305 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/stan/template/cell.stan
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       92 2023-02-05 15:45:10.000000 myokit-1.35.1/myokit/formats/stan/template/run.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.719545 myokit-1.35.1/myokit/formats/sympy/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1638 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/sympy/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6758 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/sympy/_ereader.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4875 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/sympy/_ewriter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.719545 myokit-1.35.1/myokit/formats/wcp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      254 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/wcp/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    17140 2023-07-14 10:16:32.000000 myokit-1.35.1/myokit/formats/wcp/_wcp.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.719545 myokit-1.35.1/myokit/formats/xml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/xml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1494 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/xml/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      393 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/formats/xml/_split.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.720545 myokit-1.35.1/myokit/gui/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6154 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/gui/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    49561 2023-07-18 23:19:29.000000 myokit-1.35.1/myokit/gui/datablock_viewer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    32561 2023-07-18 22:48:59.000000 myokit-1.35.1/myokit/gui/datalog_viewer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8588 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/gui/explorer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)   108238 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/gui/ide.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2157 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/gui/progress.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    52418 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/gui/source.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6072 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/gui/vargrapher.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.721545 myokit-1.35.1/myokit/lib/
+-rw-r--r--   0 michael   (1000) michael   (1000)      216 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/lib/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23859 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/lib/deps.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28056 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/lib/guess.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46678 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/lib/hh.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    67773 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/lib/markov.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4408 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/lib/multi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    13874 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/lib/plots.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4552 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/pacing.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8230 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/pype.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.728545 myokit-1.35.1/myokit/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2738 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/tests/ansic_event_based_pacing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1250 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/tests/ansic_time_series_pacing.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.730545 myokit-1.35.1/myokit/tests/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3022 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/tests/data/beeler-1977-model-compare-a.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2889 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/data/beeler-1977-model-compare-b.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3137 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/tests/data/beeler-1977-model.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/beeler-1977-protocol.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/beeler-1977-script.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3287 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/tests/data/beeler-1977-units.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     5091 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/data/clancy-1999-fitting.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3128 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/conditional.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6067 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/tests/data/cv1d.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/cv1d.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)    23916 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/decker-2009.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)    18350 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/decker.model
+-rw-r--r--   0 michael   (1000) michael   (1000)    10416 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/dn-1985-normalised.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      800 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/dom-markov.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.730545 myokit-1.35.1/myokit/tests/data/formats/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8192 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/abf-protocol.pro
+-rw-r--r--   0 michael   (1000) michael   (1000)    98376 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/abf-v1.abf
+-rw-r--r--   0 michael   (1000) michael   (1000)    44544 2023-07-12 17:16:09.000000 myokit-1.35.1/myokit/tests/data/formats/abf-v2.abf
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.731545 myokit-1.35.1/myokit/tests/data/formats/cellml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/cellml/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)    59093 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/cellml/br-1977-dot.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    58593 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/cellml/br-1977.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)   117223 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/cellml/corrias.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)   221953 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/cellml/decker-2009.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1595 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/cellml/documentation.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/cellml/invalid-file.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    44837 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    44947 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.733545 myokit-1.35.1/myokit/tests/data/formats/channelml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2648 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      557 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2702 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2369 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1258 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1539 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1290 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1374 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1373 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      675 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1398 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1317 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.733545 myokit-1.35.1/myokit/tests/data/formats/sbml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8719 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     9801 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)    31408 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/sbml/HodgkinHuxley.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/sbml/LICENSE
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.733545 myokit-1.35.1/myokit/tests/data/formats/sbml/model/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2952 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1226 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.734545 myokit-1.35.1/myokit/tests/data/formats/sbml/result/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2457 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/sbml/result/00001-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     2206 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/sbml/result/00004-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/sbml/result/01103-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)    25600 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/formats/wcp-file.wcp
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.739545 myokit-1.35.1/myokit/tests/data/io/
+-rw-r--r--   0 michael   (1000) michael   (1000)      735 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad1d-1-not-enough-files.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109429 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad1d-2-no-header.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   104768 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad1d-3-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad1d-4-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109458 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad1d-5-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1549 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad1d-6-time-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad1d-7-0d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad1d-8-1d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)      739 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad2d-1-not-enough-files.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346240 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad2d-2-no-header.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   333091 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad2d-3-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad2d-4-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346257 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad2d-5-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1553 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad2d-6-time-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1588 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad2d-7-0d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/bad2d-8-2d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)      623 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/badlog-1-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1281 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/badlog-2-no-structure.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/badlog-3-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/badlog-4-invalid-n-fields.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/badlog-5-invalid-data-size.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1457 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/badlog-6-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/badlog-7-not-enough-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     6031 2023-06-07 13:48:59.000000 myokit-1.35.1/myokit/tests/data/io/block2d.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/block2d.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-1-empty.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-10-just-spaces.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-11-just-a-semicolon.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-12-bad-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-13-header-with-empty-1.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-14-header-with-empty-2.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-15-header-with-empty-3.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-16-wrong-columns-in-data.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-17-non-float-data.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      112 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-2-windows.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      103 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-3-old-mac.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-4-empty-lines.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-5-semicolons.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-6-open-string.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-7-empty-lines-2.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-8-unquoted-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      114 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog-9-double-quoted-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/datalog.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     1421 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/io/goodlog.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     4992 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/lr-1991-dep.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2315 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/lr-1991-fitting.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4571 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/lr-1991-testing.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6124 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/lr-1991.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.739545 myokit-1.35.1/myokit/tests/data/multi/
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/multi/beeler-1977-protocol.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/multi/beeler-1977-script.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/multi/beeler-no-name.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6013 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/multi/lr-1991.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/multi/not-a-model.csv
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.739545 myokit-1.35.1/myokit/tests/data/multi/subdir/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/multi/subdir/beeler-no-name.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3754 2023-06-07 13:48:23.000000 myokit-1.35.1/myokit/tests/data/noble-1962.mmt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    22536 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_aux.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    56981 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_cellml_v1_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    41869 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_cellml_v1_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12532 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_cellml_v1_writer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    73319 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_cellml_v2_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    26345 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_cellml_v2_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10977 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_cellml_v2_writer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4058 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_cmodel.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      476 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_compiler_detection.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14096 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_component.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11511 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_config.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    52565 2023-07-18 23:19:29.000000 myokit-1.35.1/myokit/tests/test_datablock.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    82855 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/tests/test_datalog.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    60654 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_dependency_checking.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)   138508 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_expressions.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4882 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_float.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4236 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    32603 2023-07-13 10:36:29.000000 myokit-1.35.1/myokit/tests/test_formats_axon.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    19078 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_cellml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6703 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_channelml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11358 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_easyml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     9169 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_exporters.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    40800 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_expression_writers.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3539 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_html.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1531 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_importers.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    37444 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_mathml_content.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8726 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_mathml_presentation.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    17298 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_opencl.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4672 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_sbml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10324 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_formats_sympy.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7658 2023-07-13 10:36:31.000000 myokit-1.35.1/myokit/tests/test_formats_wcp.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14334 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_io.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1821 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_jacobian_calculator.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1767 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_jacobian_tracer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7476 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_lib_deps.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    42333 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_lib_guess.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    31014 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_lib_hh.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    39983 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_lib_markov.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5145 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_lib_multi.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6062 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_lib_plots.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2829 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_meta.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    84972 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_model.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    16720 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_model_building.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3834 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_opencl_info.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8193 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_pacing_factory.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6504 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/tests/test_pacing_system_c.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3637 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/tests/test_pacing_system_py.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    50865 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_parsing.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2762 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_progress_reporters.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    15092 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_protocol.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12565 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_protocol_floating_point.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2318 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_protocol_time_series.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2402 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_pype.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7353 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_quantity.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3452 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_rhs_benchmarker.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    71633 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_sbml_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    54542 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_sbml_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    19281 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/tests/test_simulation_1d.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    44343 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/tests/test_simulation_cvodes.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1853 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_simulation_cvodes_from_disk.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    36596 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/tests/test_simulation_fiber_tissue.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14033 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_simulation_log_interval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    60162 2023-07-11 14:14:16.000000 myokit-1.35.1/myokit/tests/test_simulation_opencl.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3005 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_simulation_opencl_log_interval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    20114 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_simulation_opencl_vs_cvode.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5216 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_simulation_opencl_vs_sim1d.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      562 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_system_info.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10358 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_tools.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    13635 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_unit.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1721 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_user_functions.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    33331 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tests/test_variable.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    16868 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/tools.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8503 2023-06-25 10:52:15.000000 myokit-1.35.1/myokit/units.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-18 23:29:26.704545 myokit-1.35.1/myokit.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5059 2023-07-18 23:29:26.000000 myokit-1.35.1/myokit.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15109 2023-07-18 23:29:26.000000 myokit-1.35.1/myokit.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-07-18 23:29:26.000000 myokit-1.35.1/myokit.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       48 2023-07-18 23:29:26.000000 myokit-1.35.1/myokit.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-01-04 14:18:38.000000 myokit-1.35.1/myokit.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      176 2023-07-18 23:29:26.000000 myokit-1.35.1/myokit.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        7 2023-07-18 23:29:26.000000 myokit-1.35.1/myokit.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-07-18 23:29:26.739545 myokit-1.35.1/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     3183 2023-06-25 10:52:15.000000 myokit-1.35.1/setup.py
```

### Comparing `myokit-1.35.0/LICENSE.txt` & `myokit-1.35.1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 BSD 3-Clause License
 
 Copyright (c) 2011-2017 Maastricht University. All rights reserved.
 Copyright (c) 2017-2020 University of Oxford. All rights reserved.
 (University of Oxford means the Chancellor, Masters and Scholars of the University of Oxford, having an administrative office at Wellington Square, Oxford OX1 2JD, UK).
-Copyright (c) 2020-2022 University of Nottingham. All rights reserved.
+Copyright (c) 2020-2023 University of Nottingham. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `myokit-1.35.0/PKG-INFO` & `myokit-1.35.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myokit
-Version: 1.35.0
+Version: 1.35.1
 Summary: A simple interface to cardiac cellular electrophysiology
 Home-page: http://myokit.org
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/MichaelClerx/myokit/issues
 Project-URL: Documentation, http://docs.myokit.org
```

### Comparing `myokit-1.35.0/README.md` & `myokit-1.35.1/README.md`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/__init__.py` & `myokit-1.35.1/myokit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,40 +37,37 @@
 #  F    PY_RELEASE_LEVEL, A for alpha, B for beta, C for candidate, F for final
 #  0    PY_RELEASE_SERIAL, increments with every release
 #
 import sys  # noqa
 if sys.hexversion < 0x03000000:  # pragma: no cover
     raise Exception('This version of Myokit does not support Python 2.')
 elif sys.hexversion < 0x03070000:  # pragma: no cover
-    import logging  # noqa
-    log = logging.getLogger(__name__)
-    log.warning(
-        'Myokit is not tested on Python 3 versions older than 3.7. Detected'
-        ' Python version: ' + sys.version)
-    del logging, log
+    import warnings  # noqa
+    warnings.warn(
+        'Myokit is not tested on Python versions before 3.7. Detected'
+        f' version {sys.version}.')
+    del warnings
 del sys
 
 
 #
 # Version information
 #
 from ._myokit_version import (  # noqa
     __release__,
     __version__,
     __version_tuple__,
 )
 
 
 # Warn about development version
-import logging  # noqa
-log = logging.getLogger(__name__)
-log.info('Loading Myokit version ' + __version__)
 if not __release__:     # pragma: no cover
-    log.warning('Using development version of Myokit (' + __version__ + ').')
-del log, logging
+    import warnings  # noqa
+    warnings.warn(f'Using development version of Myokit ({__version__}).')
+    del warnings
 
 
 #
 # Licensing
 #
 
 # Full license text
@@ -78,15 +75,15 @@
 BSD 3-Clause License
 
 Copyright (c) 2011-2017 Maastricht University. All rights reserved.
 Copyright (c) 2017-2020 University of Oxford. All rights reserved.
  (University of Oxford means the Chancellor, Masters and Scholars of the
   University of Oxford, having an administrative office at Wellington Square,
   Oxford OX1 2JD, UK).
-Copyright (c) 2020-2022 University of Nottingham. All rights reserved.
+Copyright (c) 2020-2023 University of Nottingham. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
 
@@ -117,15 +114,15 @@
     BSD 3-Clause License
     <br />
     <br />Copyright (c) 2011-2017 Maastricht University. All rights reserved.
     <br />Copyright (c) 2017-2020 University of Oxford. All rights reserved.
     <br />(University of Oxford means the Chancellor, Masters and Scholars of
     the University of Oxford, having an administrative office at Wellington
     Square, Oxford OX1 2JD, UK).
-    <br />Copyright (c) 2020-2022 University of Nottingham. All rights
+    <br />Copyright (c) 2020-2023 University of Nottingham. All rights
     reserved.</br></p>
 <p>
     Redistribution and use in source and binary forms, with or without
     modification, are permitted provided that the following conditions are met:
 </p>
 <ul>
     <li>
@@ -198,15 +195,15 @@
         shutil.move(DIR_USER_OLD, DIR_USER)
         del shutil
 
 # Ensure the user config directory exists and is writable
 if os.path.exists(DIR_USER):    # pragma: no cover
     if not os.path.isdir(DIR_USER):
         raise Exception(
-            'File or link found in place of user directory: ' + str(DIR_USER))
+            f'File or link found in place of user directory: {DIR_USER}')
 else:                           # pragma: no cover
     os.makedirs(DIR_USER)
 
 # Example mmt file
 EXAMPLE = os.path.join(DIR_DATA, 'example.mmt')
 
 # Don't expose standard libraries as part of Myokit
```

### Comparing `myokit-1.35.0/myokit/__main__.py` & `myokit-1.35.1/myokit/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2136,11 +2136,8 @@
         default='traditional',
         choices=myokit.ColorMap.names(),
     )
     parser.set_defaults(func=video)
 
 
 if __name__ == '__main__':
-    import logging
-    logging.basicConfig()
-
     main()
```

### Comparing `myokit-1.35.0/myokit/_aux.py` & `myokit-1.35.1/myokit/_aux.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/example.mmt` & `myokit-1.35.1/myokit/_bin/example.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/find.png` & `myokit-1.35.1/myokit/_bin/gui/find.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-128.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-128.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-16.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-16.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-24.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-24.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-256.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-256.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-32.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-32.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-48.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-48.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-64.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-64.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer-96.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer-96.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer.ico` & `myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer.ico`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-datablock-viewer.png` & `myokit-1.35.1/myokit/_bin/gui/icon-datablock-viewer.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-ide-128.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-ide-128.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-ide-16.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-ide-16.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-ide-24.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-ide-24.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-ide-256.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-ide-256.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-ide-32.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-ide-32.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-ide-48.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-ide-48.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-ide-64.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-ide-64.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-ide-96.xpm` & `myokit-1.35.1/myokit/_bin/gui/icon-ide-96.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-ide.ico` & `myokit-1.35.1/myokit/_bin/gui/icon-ide.ico`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/icon-ide.png` & `myokit-1.35.1/myokit/_bin/gui/icon-ide.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/new.png` & `myokit-1.35.1/myokit/_bin/gui/new.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/open.png` & `myokit-1.35.1/myokit/_bin/gui/open.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/gui/save.png` & `myokit-1.35.1/myokit/_bin/gui/save.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/install-lin/myokit.lang` & `myokit-1.35.1/myokit/_bin/install-lin/myokit.lang`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/install-win/menu.json` & `myokit-1.35.1/myokit/_bin/install-win/menu.json`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/LICENSE` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/LICENSE`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib` & `myokit-1.35.1/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_config.py` & `myokit-1.35.1/myokit/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Loads settings from configuration file in user home directory or attempts to
 # guess best settings.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 import configparser
-import logging
 import os
 import platform
 import sys
 import warnings
 
 # Load Myokit, at least, the bit that's been setup so far. This just means
 # this method will add a link to the myokit module already being loaded
@@ -175,16 +174,15 @@
         config.set('opencl', 'inc', ';'.join(paths))
 
     # Write ini file
     try:
         with open(path, 'w') as configfile:
             config.write(configfile)
     except IOError:     # pragma: no cover
-        logger = logging.getLogger('myokit')
-        logger.warning('Warning: Unable to write settings to ' + str(path))
+        warnings.warn('Warning: Unable to write settings to ' + str(path))
 
 
 def _load():
     """
     Reads the configuration file and attempts to set the library paths.
     """
     # Location of configuration file
```

### Comparing `myokit-1.35.0/myokit/_datablock.py` & `myokit-1.35.1/myokit/_datalog.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1865 +1,1981 @@
 #
-# Containers for time-series of 1d and 2d rectangular data arrays.
+# Functions relating to the DataLog class for storing time series data.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-import array
 import os
+import re
 import sys
-
-import myokit
+import array
 
 import numpy as np
 
+from collections import OrderedDict
 
-# Readme file for DataBlock1d binary files
-README_SAVE_1D = """
-Myokit DataBlock1d Binary File
-==============================
-This zip file contains simulation data in the form of multiple time series.
-Zero-dimensional time series, such as time or a global pace variable are
-stored, as well as one-dimensional time series, such as the membrane potential
-of a linear sequence of cells, as it varies over time.
-
-This file has the following entries:
-
-header_block1d.txt
-------------------
-A header file containing the following information (line by line):
-
-  - nt     the number of points in time in each entry
-  - nx     the width of each 1d block
-  - dtype  the used datatype (either "d" or "f")
-  - name   the names of all 0d entries, each on its own line
-  - 1      the indication that the 1d entries are starting
-  - name   the names of all 1d entries, each on its own line
-
-data.bin
---------
-A binary file containing the following data, in the data type specified by the
-header, and little-endian:
-
-  - The nt time values
-  - All 0d entries
-  - All 1d entries, reshaped using numpy order='C'
+import myokit
 
-""".strip()
 
-# Readme file for DataBlock2d binary files
-README_SAVE_2D = """
-Myokit DataBlock2d Binary File
-==============================
-This zip file contains simulation data in the form of multiple time series.
-Zero-dimensional time series, such as time or a global pace variable are
-stored, as well as two-dimensional time series, such as the membrane potential
-of a 2d grid of cells, as it varies over time.
-
-This file has the following entries:
-
-header_block2d.txt
-------------------
-A header file containing the following information (line by line):
-
-  - nt     the number of points in time in each entry
-  - ny     the height of each 2d block
-  - nx     the width of each 2d block
-  - dtype  the used datatype (either "d" or "f")
-  - name   the names of all 0d entries, each on its own line
-  - 2      the indication that the 2d entries are starting
-  - name   the names of all 2d entries, each on its own line
-
-data.bin
---------
-A binary file containing the following data, in the data type specified by the
-header, and little-endian:
-
-  - The nt time values
-  - All 0d entries
-  - All 2d entries, reshaped using numpy order='C'
+# Function to split keys into dimension-key,qname-key pairs
+ID_NAME_PATTERN = re.compile(r'(\d+.)+')
 
+# Readme file for DataLog binary files
+README_SAVE_BIN = """
+Myokit DataLog Binary File
+--------------------------
+This zip file contains binary time series data for one or multiple variables.
+The file structure.txt contains structural information about the data in plain
+text. The first line lists the number of fields. The second line gives the
+length of the data arrays. The third line specifies the data type, either
+single ("f") or double ("d") precision. The fourth line indicates which entry
+corresponds to a time variable, or is blank if no time variable was explicitly
+specified. Each following line contains the name of a data field, in the order
+its data occurs in the binary data file "data.bin". All data is stored
+little-endian.
 """.strip()
 
 # Encoding used for text portions of zip files
 ENC = 'utf-8'
 
 
-class DataBlock1d:
+class DataLog(OrderedDict):
     """
-    Container for time-series of 1d rectangular data arrays.
+    A dictionary time-series, for example data logged during a simulation or
+    experiment.
+
+    A :class:`DataLog` is expected but not required to contain a single
+    entry indicating time and any number of entries representing a variable
+    varying over time.
+
+    Single cell data is accessed simply by the variable name::
+
+        v = log['membrane.V']
+
+    Multi-cell data is accessed by appending the index of the cell before the
+    variable name. For example::
+
+        v = log['1.2.membrane.V']
+
+    This returns the membrane potential for cell (1, 2). Another way to obtain
+    the same result is::
+
+        v = log['membrane.V', 1, 2]
 
-    Each ``DataBlock1d`` has a fixed width ``w``, and a 0d time series vector
-    containing a sequence of ``n`` times.
+    or, finally::
 
-    One-dimensional time series can be added to the block, provided the data
-    also contains ``n`` instances of ``w`` data points. The data should be
-    passed in as a numpy array with shape ``(n, w)``.
+        v = log['membrane.V', (1, 2)]
 
-    Zero-dimensional time series can be added, provided they have length ``n``.
+    Every array stored in the log must have the same length. This condition can
+    be checked by calling the method :meth:`validate`.
 
-    A "one-dimensional time-series" is a series of equally sized 1d arrays
-    (sequences), such that the first corresponds to a time ``t[0]``, the second
-    to ``t[1]``, etc. Each array has shape ``(n, w)``.
+    A new ``DataLog`` can be created in a number of ways::
 
-    A "zero-dimensional time-series" is a series of single values where the
-    first corresponds to a time ``t[0]``, the second to ``t[1]``, etc.
+        # Create an empty DataLog:
+        d = myokit.DataLog()
+        d['time'] = [1, 2, 3]
+        d['data'] = [2, 4, 5]
+        d.set_time_key('time')
+
+        # Create a clone of d
+        e = myokit.DataLog(d)
+
+        # Create a DataLog based on a dictionary
+        d = myokit.DataLog({'time':[1, 2, 3], 'data':[2, 4, 5]}, time='time')
 
-    Constructor info:
+    Arguments:
 
-    ``w``
-        Each 1d block should have dimension ``w`` by ``1``.
+    ``other``
+        A DataLog to clone or a dictionary to use as basis.
     ``time``
-        A sequence of ``n`` times.
-    ``copy``
-        By default, a copy of the given time sequence will be stored. To
-        prevent this copy, set ``copy=False``.
+        The log key to use for the time variable. When cloning a log, adding
+        the ``time`` argument will overwrite the cloned value.
 
     """
-    def __init__(self, w, time, copy=True):
-        # Width
-        w = int(w)
-        if w < 1:
-            raise ValueError('Minimum w is 1.')
-        self._nx = w
-        # Time
-        time = np.array(time, copy=copy)
-        if len(time.shape) != 1:
-            raise ValueError('Time must be a sequence.')
-        if np.any(np.diff(time) < 0):
-            raise ValueError('Time must be non-decreasing.')
-        self._time = time
-        self._nt = len(time)
-        # 0d variables
-        self._0d = {}
-        # 1d variables
-        self._1d = {}
+
+    def __init__(self, other=None, time=None):
+        if other is None:
+            # Create new
+            super().__init__()
+            self._time = None
+        else:
+            # Clone
+            super().__init__(other)
+            try:
+                self._time = str(other._time)
+            except Exception:
+                self._time = None
+        if time is not None:
+            self.set_time_key(time)
+
+    def apd(self, v='membrane.V', threshold=-70):
+        """
+        Calculates one or more Action Potential Durations (APDs) in a single
+        cell's membrane potential.
+
+        *Note 1: More accuracte APD measurements can be obtained using the*
+        :class:`Simulation` *object's APD tracking functionality. See*
+        :meth:`Simulation.run()` *for details.*
+
+        *Note 2: This APD is defined by simply checking crossing of a threshold
+        potential, and does not look at lowest or highest voltages in a
+        signal.*
+
+        The membrane potential data should be listed in the log under the key
+        given by ``v``.
+
+        The returned value is a list of tuples (AP_start, APD).
+        """
+        def crossings(x, y, t):
+            """
+            Calculates the ``x``-values where ``y`` crosses threshold ``t``.
+            Returns a list of tuples ``(xc, sc)`` where ``xc`` is the ``x``
+            coordinate of the crossing and ``sc`` is the slope at this point.
+            """
+            x = np.asarray(x)
+            y = np.asarray(y)
+
+            # Get array of places where v exceeds the threshold (1s and 0s)
+            h = (y > t) * 1
+
+            # Get array of indices just before a crossing
+            c = np.argwhere(h[1:] - h[:-1])
+
+            # Gather crossing times
+            crossings = []
+            for i in c:
+                i = i[0]
+                sc = (y[i + 1] - y[i]) / (x[i + 1] - x[i])
+                if y[i] == t:
+                    xc = x[i]
+                else:
+                    xc = x[i] + (t - y[i]) / sc
+                crossings.append((xc, sc))
+            return crossings
+
+        # Check time variable
+        t = np.asarray(self.time())
+
+        # Check voltage variable
+        v = np.asarray(self[v])
+
+        # Check threshold
+        threshold = float(threshold)
+
+        # Initial status: check if already in AP
+        apds = myokit.DataLog()
+        apds['start'] = []
+        apds['duration'] = []
+        last = t[0]
+
+        # Evaluate crossings
+        for time, slope in crossings(t, v, threshold):
+            if slope < 0:
+                # End of AP
+                if last != t[0]:    # Don't inlcude AP started before t[0]
+                    apds['start'].append(last)
+                    apds['duration'].append(time - last)
+            last = time
+        return apds
+
+    def block1d(self):
+        """
+        Returns a copy of this log as a :class:`DataBlock1d`.
+        """
+        return myokit.DataBlock1d.from_log(self)
 
     def block2d(self):
         """
-        Returns a :class:`myokit.DataBlock2d` based on this 1d data block.
+        Returns a copy of this log as a :class:`DataBlock2d`.
         """
-        b = DataBlock2d(self._nx, 1, self._time)
-        for k, v in self._0d.items():
-            b.set0d(k, v)
-        shape = (self._nt, 1, self._nx)
-        for k, v in self._1d.items():
-            b.set2d(k, v.reshape(shape))
-        return b
+        return myokit.DataBlock2d.from_log(self)
 
-    def cv(self, name, threshold=-30, length=0.01, time_multiplier=1e-3,
-            border=None):
+    def clone(self, numpy=False):
         """
-        Calculates conduction velocity (CV) in a cable.
+        Returns a deep clone of this log.
 
-        Accepts the following arguments:
+        All lists in the log will be duplicated, but the list contents are
+        assumed to be numerical (and thereby immutable) and won't be cloned.
 
-        ``name``
-            The name (as string) of the membrane potential variable. This
-            should be a 1d variable in this datablock.
-        ``threshold``
-            The start of an action potential is determined as the first time
-            the membrane potential crosses this threshold (default=-30mV) and
-            has a positive direction.
-        ``length``
-            The length of a single cell in cm, in the direction of the cable.
-            The default is ``length=0.01cm``.
-        ``time_multiplier``
-            A multiplier used to convert the used time units to seconds. Most
-            simulations use milliseconds, so the default value is 1e-3.
-        ``border``
-            The number of cells to exclude from the analysis on each end of the
-            cable to avoid boundary effects. If not given, 1/3 of the number of
-            cells will be used, with a maximum of 50 cells on each side.
-
-        Returns the approximate conduction velocity in cm/s. If no cv can be
-        """
-        # Check border
-        if border is None:
-            border = min(50, self._nx // 3)
+        A log with numpy arrays instead of lists can be created by setting
+        ``numpy=True``.
+        """
+        log = DataLog()
+        log._time = self._time
+        if numpy:
+            for k, v in self.items():
+                log[str(k)] = np.array(v, copy=True, dtype=float)
         else:
-            border = int(border)
-            if border < 0:
-                raise ValueError('The argument `border` cannot be negative.')
-            elif border >= self._nx // 2:
-                raise ValueError(
-                    'The argument `border` must be less than half the number'
-                    ' of cells.')
+            for k, v in self.items():
+                log[str(k)] = list(v)
+        return log
 
-        # Get indices of selected cells
-        ilo = border                # First index
-        ihi = self._nx - border     # Last index + 1
-
-        # Indices of cells with AP
-        i1 = None
-        i2 = None
-
-        # Get Vm, reshaped to get each cell's time-series successively.
-        v_series = self._1d[name].reshape(self._nt * self._nx, order='F')
-
-        # Split Vm into a series per cell (returns views!)
-        v_series = np.split(v_series, self._nx)
-
-        # Find first activation time
-        have_crossing = False
-        t = []
-        for i in range(ilo, ihi):
-            v = v_series[i]
-            # Get index of first threshold crossing with positive flank
-            # Don't include crossings at log index 0
-            itime = np.where((v[1:] > -30) & (v[1:] - v[:-1] > 0))[0]
-            if len(itime) == 0 or itime[0] == 0:
-                # No crossing found
-                if have_crossing:
-                    # CV calculation ends here
-                    i2 = i - 1
-                    break
-            else:
-                # Crossing found!
-                if have_crossing:
-                    i2 = i
-                else:
-                    i1 = i
-                    have_crossing = True
-                itime = 1 + itime[0]
-                # Interpolate to get better estimate
-                v0 = v[itime - 1]
-                v1 = v[itime]
-                t0 = self._time[itime - 1]
-                t1 = self._time[itime]
-                t.append(t0 + (threshold - v0) * (t1 - t0) / (v1 - v0))
-        if not have_crossing:
-            return 0
+    def __contains__(self, key):
+        return super().__contains__(self._parse_key(key))
 
-        # No propagation: all depolarisations at the same time
-        if np.all(t == t[0]):
-            return 0
+    def __delitem__(self, key):
+        return super().__delitem__(self._parse_key(key))
 
-        # Get times in seconds, lengths in cm
-        t = np.array(t, copy=False) * time_multiplier
-        x = np.arange(i1, 1 + i2, dtype=float) * length
+    def extend(self, other):
+        """
+        Returns a copy of this log, extended with the data of another.
 
-        # Use linear least squares to find the conduction velocity
-        A = np.vstack([t, np.ones(len(t))]).T
-        try:
-            # Newer numpy wants rcond=None
-            cv = np.linalg.lstsq(A, x, rcond=None)[0][0]
-        except TypeError:   # pragma: no cover
-            cv = np.linalg.lstsq(A, x)[0][0]
+        Both logs must have the same keys and the same time key. The added data
+        must be from later time points than in the log being extended.
+        """
+        if other._time != self._time:
+            raise ValueError('Both logs must have the same time key.')
+        if other[self._time][0] < self[self._time][-1]:
+            raise ValueError(
+                'Cannot extend DataLog with data from an earlier time.')
+        if set(self.keys()) != set(other.keys()):
+            raise ValueError('Both logs must have the same keys.')
+
+        # Create new log
+        log = DataLog()
+        log._time = self._time
+
+        # Add data
+        for k, v1 in self.items():
+            v2 = other[k]
+            if isinstance(v1, np.ndarray) or isinstance(v2, np.ndarray):
+                # Concatenation copies data
+                log[k] = np.concatenate((np.asarray(v1), np.asarray(v2)))
+            else:
+                log[k] = list(v1)   # Copies v1 data
+                log[k].extend(v2)   # Copies v2 data
 
         # Return
-        return cv
+        return log
 
-    @staticmethod
-    def from_DataLog(log):
-        """Deprecated alias of :meth:`from_log()`."""
-        # Deprecated since 2020-09-14
+    def find(self, time):
+        """
+        Deprecated alias of :meth:`find_after()`.
+        """
+        # Deprecated since 2019-08-16
         import warnings
         warnings.warn(
-            'The method `DataBlock1d.from_DataLog` is deprecated. Please use'
-            ' `DataBlock1d.from_log` instead.')
-        return DataBlock1d.from_log(log)
+            'The method `find` is deprecated. Please use `find_after`'
+            ' instead.')
 
-    @staticmethod
-    def from_log(log):
-        """
-        Creates a DataBlock1d from a :class:`myokit.DataLog`.
+        return self.find_after(time)
+
+    def find_after(self, time):
         """
-        log.validate()
+        Returns the lowest index ``i`` such that
 
-        # Get time variable name
-        time = log.time_key()
-        if time is None:
-            raise ValueError('No time variable set in data log.')
+            times[i] >= time
 
-        # Get log info
-        infos = log.variable_info()
+        where ``times`` are the times stored in this ``DataLog``.
 
-        # Check time variable
-        if time not in infos:
-            # Already checked time variable exists, so if not found now must
-            # be multi-dimensional
-            raise ValueError('Time variable must be 0-dimensional.')
-
-        # Check if everything is 0d or 1d, get size
-        size = None
-        for name, info in infos.items():
-            d = info.dimension()
-            if d not in (0, 1):
-                raise ValueError(
-                    'The given simulation log should only contain 0d or 1d'
-                    ' variables. Found <' + str(name) + '> with d = '
-                    + str(d) + '.')
-            if d == 1:
-                if size is None:
-                    size = info.size()
-                elif info.size() != size:
-                    raise ValueError(
-                        'The given simulation log contains 1d'
-                        ' data sets of different sizes.')
+        If no such value exists in the log, ``len(time)`` is returned.
+        """
+        times = self[self._time]
 
-        # Get dimensions
-        nt = len(log[time])
-        nx = size[0]
-
-        # Create data block
-        block = DataBlock1d(nx, log[time], copy=True)
-        for name, info in infos.items():
-            if info.dimension() == 0:
-                # Add 0d time series
-                if name == time:
-                    continue
-                block.set0d(name, log[name], copy=True)
+        # Border cases
+        n = len(times)
+        if n == 0 or time <= times[0]:
+            return 0
+        if time > times[-1]:
+            return n
 
+        # Find t
+        def find(lo, hi):
+            # lo = first index, hi = last index + 1
+            if (lo + 1 == hi):
+                return lo + 1
+            m = int((lo + hi) / 2)
+            if time > times[m]:
+                return find(m, hi)
             else:
+                return find(lo, m)
 
-                # Convert to 1d time series
-                data = np.zeros(nt * nx)
-                # Iterate over info.keys(), this has the correct order!
-                for i, key in enumerate(info.keys()):
-                    # Copy data into array (really copies)
-                    data[i * nt:(i + 1) * nt] = log[key]
-                # Reshape
-                data = data.reshape((nt, nx), order='F')
-                # If this is a view of existing data, make a copy!
-                if data.base is not None:
-                    data = np.array(data)
-                block.set1d(name, data, copy=False)
-
-        return block
+        return find(0, n)
 
-    def get0d(self, name):
-        """
-        Returns the 0d time-series identified by ``name``. The data is returned
-        directly, no copy is made.
+    def fold(self, period, discard_remainder=True):
         """
-        return self._0d[name]
+        Creates a copy of the log, split with the given period. Split signals
+        are given indexes so that "current" becomes "0.current", "1.current"
+        "2.current", etc.
+
+        If the logs entries do not divide well by 'period', the remainder will
+        be ignored. This happens commonly due to rounding point errors (in
+        which case the remainder is a single entry). To disable this behavior,
+        set ``discard_remainder=False``.
+        """
+        # Note: Using closed intervals can lead to logs of unequal length, so
+        # it should be disabled here to ensure a valid log
+        logs = self.split_periodic(period, adjust=True, closed_intervals=False)
+        # Discard remainder if present
+        if discard_remainder:
+            if len(logs) > 1:
+                n = logs[0].length()
+                if logs[-1].length() < n:
+                    logs = logs[:-1]
+        # Create new log with folded data
+        out = myokit.DataLog()
+        out._time = self._time
+        out[self._time] = logs[0][self._time]
+        for i, log in enumerate(logs):
+            for k, v in log.items():
+                if k != self._time:
+                    out[k, i] = v
+        return out
 
-    def get1d(self, name):
-        """
-        Returns the 1d time-series identified by ``name``. The data is returned
-        directly, no copy is made.
+    def __getitem__(self, key):
+        return super().__getitem__(self._parse_key(key))
 
-        The returned data is a 2d array of the shape given by :meth:`shape`.
+    def has_nan(self):
+        """
+        Returns True if one of the variables in this DataLog has a ``NaN`` as
+        its final logged value.
         """
-        return self._1d[name]
+        for k, d in self.items():
+            if len(d) > 0 and np.isnan(d[-1]):
+                return True
+        return False
 
-    def grid(self, name, transpose=True):
+    def integrate(self, name, *cell):
         """
-        Returns a 2d grid representation suitable for plotting color maps or
-        contours with ``matplotlib.pyplot`` methods such as ``pcolor`` and
-        ``pcolormesh``.
+        Integrates a field from this log and returns it::
 
-        When used for example with
-        ``pyplot.pcolormesh(*block.grid('membrane.V'))`` this will create a 2d
-        plot where the horizontal axis shows time and the vertical axis shows
-        the cell index.
+            # Run a simulation and calculate the total current carried by INa
+            s = myokit.Simulation(m, p)
+            d = s.run(1000)
+            q = d.integrate('ina.INa')
 
         Arguments:
 
         ``name``
-            The name identifying the 1d data-values to return.
-        ``transpose``
-            By default (``transpose=True``) the data is returned so that ``x``
-            represents time and ``y`` represents space. To reverse this (and
-            use the order used internally in the datablocks), set
-            ``transpose=False``.
-
-        The returned format is a tuple ``(x, y, z)`` where ``x``, ``y`` and
-        ``z`` are all 2d numpy arrays.
-        Here, ``x`` (time) and ``y`` (space) describe the x and y-coordinates
-        of rectangles, with a color (data value) given by ``z``.
-
-        In particular, each rectangle ``(x[i, j], y[i, j])``,
-        ``(x[i + 1, j], y[i + 1, j])``, ``(x[i, j + 1], y[i, j + 1])``,
-        ``(x[i + 1,j + 1], y[i + 1,j + 1])``, has a color given by ``z[i, j]``.
-
-        As a result, for a block of width ``w`` (e.g., ``w`` cells) containing
-        ``n`` logged time points, the method returns arrays ``x`` and ``y`` of
-        shape ``(w + 1, n + 1)`` and an array ``z`` of shape ``(w, n)``.
-
-        See :meth:`image_grid()` for a method where ``x``, ``y`` and ``z`` all
-        have shape ``(w, n)``.
-        """
-        # Append point in time at pos [-1] + ([-1] - [-2])
-        ts = np.append(self._time, 2 * self._time[-1] - self._time[-2])
-        # Append one extra cell or node
-        xs = np.arange(0, self._nx + 1)
-        # Make grid
-        return self._grid(ts, xs, self._1d[name], transpose)
-
-    def image_grid(self, name, transpose=True):
-        """
-        Returns a 2d grid representation of the data.
-
-        The returned format is a tuple ``(x, y, z)`` where ``x``, ``y`` and
-        ``z`` are all 2d numpy arrays.
-        Here, ``x`` and ``y`` describe the time and space-coordinates of the
-        logged points respectively, and ``z`` describes the corresponding data
-        value.
-        For a block of width ``w`` (e.g., ``w`` cells) containing ``n`` logged
-        time points, each returned array has the shape ``(w, n)``.
+            The name of the variable to return, for example 'ik1.IK1' or
+            '2.1.membrane.V'.
+        ``*cell``
+            An optional cell index, for easy access to multi-cellular data, for
+            example ``log.integrate('membrane.V', 2, 1)``.
+
+        """
+        # Get data to integrate
+        key = [str(x) for x in cell]
+        key.append(str(name))
+        key = '.'.join(key)
+        data = np.array(self[key], copy=True)
+        time = np.asarray(self.time())
+
+        # Integration using the midpoint Riemann sum:
+        #  At point i=0, the value is 0
+        #  At each point i>0, the value increases by step[i, i-1]*mean[i, i-1]
+        #data[1:] = 0.5 * (data[1:] + data[:-1]) * (time[1:] - time[:-1])
+        #data[0]  = 0
+
+        # For discontinuities (esp. with CVODES), it makes more sense to treat
+        # the signal as a zero-order hold, IE use the left-point integration
+        # rule:
+        data[1:] = data[:-1] * (time[1:] - time[:-1])
+        data[0] = 0
+        return data.cumsum()
+
+    def interpolate_at(self, name, time):
+        """
+        Returns the value for variable ``name`` at a given ``time``, determined
+        using linear interpolation between the nearest matching times.
+        """
+        t = self[self._time]
+        v = self[name]
 
-        Arguments:
+        # Don't extrapolate
+        if time < t[0] or time > t[-1]:
+            raise ValueError(
+                'Requested time is outside of logged range, would require'
+                ' extrapolation.')
 
-        ``name``
-            The name identifying the 1d data-values to return.
-        ``transpose``
-            By default, the data is transposed so that the ``x`` coordinates
-            become time and the ``y`` coordinates become space. Use
-            ``transpose=False`` to return untransposed results.
+        # Get first time *after or at* requested time
+        i1 = self.find_after(time)
 
-        """
-        return self._grid(
-            self._time, np.arange(0, self._nx), self._1d[name], transpose)
+        # Return directly, if possible
+        if t[i1] == time:
+            return v[i1]
+
+        # Interpolate
+        i0 = i1 - 1
+        return v[i0] + (time - t[i0]) * (v[i1] - v[i0]) / (t[i1] - t[i0])
+
+    def isplit(self, i):
+        """
+        Returns two logs, where the first contains all this log's entries up to
+        index ``i``, and the second contains all entries starting from ``i``
+        and higher.
+        """
+        log1 = DataLog()
+        log2 = DataLog()
+        log1._time = self._time
+        log2._time = self._time
+        for k, v in self.items():
+            if isinstance(v, np.ndarray):
+                log1[k] = np.array(v[:i], copy=True, dtype=float)
+                log2[k] = np.array(v[i:], copy=True, dtype=float)
+            else:
+                log1[k] = v[:i]
+                log2[k] = v[i:]
+        return log1, log2
+
+    def itrim(self, a, b):
+        """
+        Returns a copy of this log, with all entries trimmed to the region
+        between indices ``a`` and ``b`` (similar to performing ``x = x[a:b]``
+        on a list).
+        """
+        log = DataLog()
+        log._time = self._time
+        for k, v in self.items():
+            if isinstance(v, np.ndarray):
+                log[k] = np.array(v[a:b], copy=True, dtype=float)
+            else:
+                log[k] = v[a:b]
+        return log
 
-    def _grid(self, ts, xs, vs, transpose):
+    def itrim_left(self, i):
         """
-        Make a grid for the given times, spatial coordinates and data values.
+        Returns a copy of this log, with all entries before index ``i``
+        removed (similar to performing ``x = x[i:]`` on a list).
         """
-        if transpose:
-            x, y = np.meshgrid(ts, xs)
-            z = np.reshape(vs, (self._nx * self._nt,), order='F')
-            z = np.reshape(z, (self._nx, self._nt), order='C')
-        else:
-            x, y = np.meshgrid(xs, ts)
-            z = np.reshape(vs, (self._nx * self._nt,), order='C')
-            z = np.reshape(z, (self._nt, self._nx), order='C')
-        # If z is a view, create a copy
-        if z.base is not None:
-            z = np.array(z, copy=True)
-        return x, y, z
+        log = DataLog()
+        log._time = self._time
+        for k, v in self.items():
+            if isinstance(v, np.ndarray):
+                log[k] = np.array(v[i:], copy=True, dtype=float)
+            else:
+                log[k] = v[i:]
+        return log
 
-    def keys0d(self):
+    def itrim_right(self, i):
         """
-        Returns an iterator over this block's 0d time series.
+        Returns a copy of this log, with all entries starting from index ``i``
+        removed (similar to performing ``x = x[:i]`` on a list).
         """
-        return iter(self._0d)
+        log = DataLog()
+        log._time = self._time
+        for k, v in self.items():
+            if isinstance(v, np.ndarray):
+                log[k] = np.array(v[:i], copy=True, dtype=float)
+            else:
+                log[k] = v[:i]
+        return log
 
-    def keys1d(self):
-        """
-        Returns an iterator over this block's 1d time series.
+    def keys_like(self, query):
         """
-        return iter(self._1d)
+        Returns all keys that match the pattern ``*.query``, sorted
+        alphabetically.
 
-    def len0d(self):
-        """
-        Returns the number of 0d time series in this block.
+        For example, ``log.keys_like('membrane.V')`` could return a list
+        ``['0.membrane.V', '1.membrane.V', '2.membrane,V', ...]``, or
+        ``['0.0.membrane.V', '0.1.membrane.V', '1.0.membrane,V', ...]``.
         """
-        return len(self._0d)
+        keys = [x for x in self.keys() if x.endswith('.' + str(query))]
+        keys.sort()
+        return keys
 
-    def len1d(self):
+    def length(self):
         """
-        Returns the number of 1d time series in this block.
+        Returns the length of the entries in this log. If the log is empty,
+        zero is returned.
         """
-        return len(self._1d)
+        if len(self) == 0:
+            return 0
+        return len(next(iter(self.values())))
 
     @staticmethod
-    def load(filename, progress=None, msg='Loading DataBlock1d'):
+    def load(filename, progress=None, msg='Loading DataLog'):
         """
-        Loads a :class:`DataBlock1d` from the specified file.
+        Loads a :class:`DataLog` from the binary format used by myokit.
+
+        The values in the log will be stored in an :class:`array.array`. The
+        data type used by the array will be the one specified in the binary
+        file. Notice that an `array.array` storing single precision floats will
+        make conversions to ``Float`` objects when items are accessed.
 
         To obtain feedback on the simulation progress, an object implementing
         the :class:`myokit.ProgressReporter` interface can be passed in.
         passed in as ``progress``. An optional description of the current
         simulation to use in the ProgressReporter can be passed in as `msg`.
         """
+        # Check filename
         filename = os.path.expanduser(filename)
 
         # Load compression modules
         import zipfile
         try:
+            # Ensure zlib is available
             import zlib
             del zlib
         except ImportError:
             raise Exception(
                 'This method requires the ``zlib`` module to be installed.')
 
         # Get size of single and double types on this machine
         dsize = {
             'd': len(array.array('d', [1]).tobytes()),
             'f': len(array.array('f', [1]).tobytes()),
         }
 
-        # Read data from file
+        # Read data
         try:
             f = None
             f = zipfile.ZipFile(filename, 'r')
-            info = f.infolist()
-            if len(info) < 3:
-                raise myokit.DataBlockReadError(
-                    'Invalid DataBlock1d file format: Not enough files in'
-                    ' zip.')
-
             # Get ZipInfo objects
-            names = [x.filename for x in info]
             try:
-                head = names.index('header_block1d.txt')
-            except ValueError:
-                raise myokit.DataBlockReadError(
-                    'Invalid DataBlock1d file format: Header not found.')
+                body = f.getinfo('data.bin')
+            except KeyError:
+                raise myokit.DataLogReadError('Invalid log file format.')
             try:
-                body = names.index('data.bin')
-            except ValueError:
-                raise myokit.DataBlockReadError(
-                    'Invalid DataBlock1d file format: Data not found.')
-
-            # Read head and body into memory (let's assume it fits...)
-            head = f.read(info[head]).decode(ENC)
-            body = f.read(info[body])
-
+                head = f.getinfo('structure.txt')
+            except KeyError:
+                raise myokit.DataLogReadError('Invalid log file format.')
+            # Read file contents
+            head = f.read(head).decode(ENC)
+            body = f.read(body)
         except zipfile.BadZipfile:
-            raise myokit.DataBlockReadError(
-                'Unable to read DataBlock1d: Bad zip file.')
-
+            raise myokit.DataLogReadError('Unable to read log: bad zip file.')
         except zipfile.LargeZipFile:    # pragma: no cover
-            raise myokit.DataBlockReadError(
-                'Unable to read DataBlock1d: Zip file requires zip64 support'
-                ' and this has not been enabled on this system.')
-
+            raise myokit.DataLogReadError(
+                'Unable to read log: zip file requires zip64 support and this'
+                ' has not been enabled on this system.')
         finally:
             if f:
                 f.close()
 
-        # Parse head
-        head = head.splitlines()
+        # Create empty log
+        log = DataLog()
+
+        # Parse header
+        # Number of fields, length of data arrays, data type, time, fields
+        head = iter(head.splitlines())
+        n = int(next(head))
+        data_size = int(next(head))
+        data_type = next(head)
+        time = next(head)
+        if time:
+            # Note, this field doesn't have to be present in the log!
+            log._time = time
+        fields = [x for x in head]
+        if len(fields) != n:
+            raise myokit.DataLogReadError(
+                'Invalid number of fields specified.')
+
+        # Get size of each entry on disk
+        if data_size < 0:
+            raise myokit.DataLogReadError(
+                'Invalid data size: ' + str(data_size) + '.')
         try:
-            if progress:
-                progress.enter(msg)
+            data_size *= dsize[data_type]
+        except KeyError:
+            raise myokit.DataLogReadError(
+                'Invalid data type: "' + data_type + '".')
 
-                # Avoid divide by zero
-                fraction = float(len(head) - 3)
-                if fraction > 0:
-                    fraction = 1.0 / fraction
-                iprogress = 0
-                progress.update(iprogress * fraction)
-            head = iter(head)
-            nt = int(next(head))
-            nx = int(next(head))
-            dtype = next(head)[1:-1]
-            if dtype not in dsize:
-                raise myokit.DataBlockReadError(
-                    'Unable to read DataBlock1d: Unrecognized data type "'
-                    + dtype + '".')
-            names_0d = []
-            names_1d = []
-            name = next(head)
-            while name != '1':
-                names_0d.append(name[1:-1])
-                name = next(head)
-            for name in head:
-                names_1d.append(name[1:-1])
-            del head
-
-            # Parse body
-            start, end = 0, 0
-            n0 = dsize[dtype] * nt
-            n1 = n0 * nx
-            nb = len(body)
-
-            # Read time
-            end += n0
-            if end > nb:
-                raise myokit.DataBlockReadError(
-                    'Unable to read DataBlock1d: Header indicates larger data'
-                    ' than found in the body.')
-            data = array.array(dtype)
-            data.frombytes(body[start:end])
-            if sys.byteorder == 'big':  # pragma: no cover
-                data.byteswap()
-            data = np.array(data)
+        # Parse read data
+        fraction = 1.0 / len(fields)
+        start, end = 0, 0
+        nbody = len(body)
+        try:
             if progress:
-                iprogress += 1
-                if not progress.update(iprogress * fraction):
+                progress.enter(msg)
+            for k, field in enumerate(fields):
+                if progress and not progress.update(k * fraction):
                     return
 
-            # Create data block
-            block = DataBlock1d(nx, data, copy=False)
-
-            # Read 0d data
-            for name in names_0d:
+                # Get new data position
                 start = end
-                end += n0
-                if end > nb:
-                    raise myokit.DataBlockReadError(
-                        'Unable to read DataBlock1d: Header indicates larger'
-                        ' data than found in the body.')
-                data = array.array(dtype)
-                data.frombytes(body[start:end])
+                end += data_size
+                if end > nbody:
+                    raise myokit.DataLogReadError(
+                        'Header indicates larger data size than found in body.'
+                    )
+
+                # Read data
+                ar = array.array(data_type)
+                ar.frombytes(body[start:end])
                 if sys.byteorder == 'big':  # pragma: no cover
-                    data.byteswap()
-                data = np.array(data)
-                block.set0d(name, data, copy=False)
-                if progress:
-                    iprogress += 1
-                    if not progress.update(iprogress * fraction):
-                        return
-
-            # Read 1d data
-            for name in names_1d:
-                start = end
-                end += n1
-                if end > nb:
-                    raise myokit.DataBlockReadError(
-                        'Unable to read DataBlock1d: Header indicates larger'
-                        ' data than found in the body.')
-                data = array.array(dtype)
-                data.frombytes(body[start:end])
-                if sys.byteorder == 'big':  # pragma: no cover
-                    data.byteswap()
-                data = np.array(data).reshape(nt, nx, order='C')
-                block.set1d(name, data, copy=False)
-                if progress:
-                    iprogress += 1
-                    if not progress.update(iprogress * fraction):
-                        return
-            return block
+                    ar.byteswap()
+                log[field] = ar
         finally:
             if progress:
                 progress.exit()
+        return log
 
-    def remove0d(self, name):
-        """Removes the 0d time-series identified by ``name``."""
-        del self._0d[name]
-
-    def remove1d(self, name):
-        """Removes the 1d time-series identified by ``name``."""
-        del self._1d[name]
-
-    def save(self, filename):
+    @staticmethod
+    def load_csv(filename, precision=myokit.DOUBLE_PRECISION):
         """
-        Writes this ``DataBlock1d`` to a binary file.
-
-        The resulting file will be a zip file with the following entries:
+        Loads a CSV file from disk and returns it as a :class:`DataLog`.
 
-        ``header_block1d.txt``: A header file containing the following
-        information (line by line):
+        The CSV file must start with a header line indicating the variable
+        names, separated by commas. Each subsequent row should contain the
+        values at a single point in time for all logged variables.
 
-        - ``nt`` the number of points in time in each entry
-        - ``nx`` the length of each 1d block
-        - ``"dtype"`` the used datatype (either "d" or "f")
-        - ``"name"`` the names of all 0d entries, each on its own line
-        - ``1`` the indication that the 1d entries are starting
-        - ``"name"`` the names of all 1d entries, each on its own line
-
-        ``data.bin``: A binary file containing the following data, in the data
-        type specified by the header, and little-endian:
-
-        - The ``nt`` time values
-        - All 0d entries
-        - All 1d entries, reshaped using numpy order='C'
+        The ``DataLog`` is created using the data type specified by the
+        argument ``precision``, regardless of the data type of the stored data.
 
+        The log attempts to set a time variable by searching for a strictly
+        increasing variable. In the case of a tie the first strictly increasing
+        variable is used. This means logs stored with :meth:`save_csv` can
+        safely be read.
         """
+        log = DataLog()
         # Check filename
         filename = os.path.expanduser(filename)
-        # Load compression modules
-        import zipfile
-        try:
-            import zlib
-            del zlib
-        except ImportError:
-            raise Exception(
-                'This method requires the ``zlib`` module to be installed.')
 
-        # Data type
-        dtype = 'd'     # Only supporting doubles right now
+        # Typecode dependent on precision
+        typecode = 'd' if precision == myokit.DOUBLE_PRECISION else 'f'
 
-        # Create header
-        head_str = []
-        head_str.append(str(self._nt))
-        head_str.append(str(self._nx))
-        head_str.append('"' + dtype + '"')
-        for name in self._0d:
-            head_str.append('"' + name + '"')
-        head_str.append(str(1))
-        for name in self._1d:
-            head_str.append('"' + name + '"')
-        head_str = '\n'.join(head_str)
+        # Error raising function
+        def e(line, char, msg):
+            raise myokit.DataLogReadError(
+                'Syntax error on line ' + str(line) + ', character '
+                + str(1 + char) + ': ' + msg)
+
+        quote = '"'
+        delim = ','
+        with open(filename, 'r', newline=None) as f:
+            # Read header
+            keys = []   # The log keys, in order of appearance
+
+            # Read first line
+            line = f.readline()
+
+            # Ignore comments
+            while line.lstrip()[:1] == '#':
+                line = f.readline()
+
+            # Stop on EOF (indicated by blank line without line ending)
+            if line == '':
+                return log
 
-        # Create body
-        n = self._nt * self._nx
-        body_str = []
-        body_str.append(array.array(dtype, self._time))
-        for name, data in self._0d.items():
-            body_str.append(array.array(dtype, data))
-        for name, data in self._1d.items():
-            body_str.append(array.array(dtype, data.reshape(n, order='C')))
-        if sys.byteorder == 'big':  # pragma: no cover
-            for ar in body_str:
-                ar.byteswap()
-        body_str = b''.join([ar.tobytes() for ar in body_str])
+            # Trim end of line
+            line = line.rstrip(' \r\n\f;')
 
-        # Write
-        head = zipfile.ZipInfo('header_block1d.txt')
-        head.compress_type = zipfile.ZIP_DEFLATED
-        body = zipfile.ZipInfo('data.bin')
-        body.compress_type = zipfile.ZIP_DEFLATED
-        read = zipfile.ZipInfo('readme.txt')
-        read.compress_type = zipfile.ZIP_DEFLATED
-        with zipfile.ZipFile(filename, 'w') as f:
-            f.writestr(head, head_str.encode(ENC))
-            f.writestr(body, body_str)
-            f.writestr(read, README_SAVE_1D.encode(ENC))
+            # Get enumerated iterator over characters
+            line = enumerate(line)
+            try:
+                i, c = next(line)
+            except StopIteration:
+                # Empty line
+                return log
+
+            # Whitespace characters to ignore
+            whitespace = ' \f\t'
+
+            # Start parsing header fields
+            run1 = True
+            while run1:
+                text = []
+
+                # Skip whitespace
+                # (Note: rtrim above and check below mean this will never
+                #  raise a StopIteration)
+                while c in whitespace:
+                    i, c = next(line)
+
+                # Read!
+                if c == quote:
+
+                    # Read quoted field + delimiter
+                    run2 = True
+                    while run2:
+                        try:
+                            i, c = next(line)
+                        except StopIteration:
+                            e(1, i, 'Unexpected end-of-line inside quoted'
+                                ' string.')
+
+                        if c == quote:
+                            try:
+                                i, c = next(line)
+                                if c == quote:
+                                    text.append(quote)
+                                elif c == delim or c in whitespace:
+                                    run2 = False
+                                else:
+                                    e(1, i, 'Expecting double quote, delimiter'
+                                        ' or end-of-line. Found "' + c + '".')
+                            except StopIteration:
+                                run1 = run2 = False
+                        else:
+                            text.append(c)
+                else:
 
-    def set0d(self, name, data, copy=True):
-        """
-        Adds or updates a zero-dimensional time series ``data`` for the
-        variable named by the string ``name``.
+                    # Read unquoted field + delimiter
+                    while run1 and c != delim:
+                        try:
+                            text.append(c)
+                            i, c = next(line)
+                        except StopIteration:
+                            run1 = False
+
+                # Append new field to list
+                key = ''.join(text)
+                if key == '':
+                    e(1, i, 'Empty field in header.')
+                keys.append(key)
 
-        The ``data`` must be specified as a sequence of length ``n``, where
-        ``n`` is the first value returned by :meth:`DataBlock1d.shape()`.
+                # Read next character
+                try:
+                    i, c = next(line)
+                except StopIteration:
+                    run1 = False
+
+            if c == delim:
+                e(1, i, 'Empty field in header.')
+
+            # Create data structure
+            m = len(keys)
+            lists = []
+            for key in keys:
+                x = array.array(typecode)
+                lists.append(x)
+                log[key] = x
+
+            # Read remaining data
+            n = 0
+            while True:
+                row = f.readline()
+
+                # Stop if a blank line is returned: indicates EOF!
+                # (Empty line in file still has line ending)
+                if row == '':
+                    break
 
-        By default, a copy of the given data will be stored. To prevent this
-        and store a reference instead, set ``copy=False``.
-        """
-        name = str(name)
-        if not name:
-            raise ValueError('Name cannot be empty.')
-        data = np.array(data, copy=copy)
-        if data.shape != (self._nt,):
-            raise ValueError(
-                'Data must be sequence of length ' + str(self._nt) + '.')
-        self._0d[name] = data
+                # Strip leading and/or trailing whitespace
+                row = row.lstrip().rstrip(' \r\n\f;')
 
-    def set1d(self, name, data, copy=True):
-        """
-        Adds or updates a one-dimensional time series ``data`` for the variable
-        named by the string ``name``.
+                # Skip blank lines
+                if row == '':
+                    continue
 
-        The ``data`` must be specified as a numpy array with shape ``(n, w)``,
-        where ``(n, w)`` is the value returned by :meth:`DataBlock1d.shape()`.
+                # Ignore lines commented with #
+                if row[:1] == '#':
+                    continue
 
-        By default, a copy of the given data will be stored. To prevent this
-        and store a reference instead, set ``copy=False``.
-        """
-        name = str(name)
-        if not name:
-            raise ValueError('Name cannot be empty.')
-        data = np.array(data, copy=copy)
-        shape = (self._nt, self._nx)
-        if data.shape != shape:
-            raise ValueError('Data must have shape ' + str(shape) + '.')
-        self._1d[name] = data
+                # Split row into cells
+                row = row.split(delim)
+                n += 1
+                if len(row) != m:
+                    e(
+                        n, 0, 'Wrong number of columns found in row '
+                        + str(n) + '. Expecting ' + str(m) + ', found '
+                        + str(len(row)) + '.')
+                try:
+                    for k, v in enumerate(row):
+                        lists[k].append(float(v))
+                except ValueError:
+                    e(n, 0, 'Unable to convert found data to floats.')
 
-    def shape(self):
-        """
-        Returns the required shape for 1d data passed to this data block. Zero
-        dimensional series passed in must have length ``shape()[0]``.
-        """
-        return (self._nt, self._nx)
+            # Guess time variable
+            for key in keys:
+                x = np.array(log[key], copy=False)
+                y = x[1:] - x[:-1]
+                if np.all(y > 0):
+                    log.set_time_key(key)
+                    break
 
-    def time(self):
-        """
-        Returns the time data for this datablock. The data is returned
-        directly, no copy is made.
-        """
-        return self._time
+            # Return log
+            return log
 
-    def to_log(self, copy=True):
+    def npview(self):
         """
-        Returns a :class:`myokit.DataLog` containing the same information as
-        this block.
-
-        The data will be copied, unless ``copy`` is set to ``False``.
+        Returns a ``DataLog`` with numpy array views of this log's data.
         """
-        d = myokit.DataLog()
-        d.set_time_key('time')
-        d['time'] = np.array(self._time, copy=copy)
-        for k, v in self._0d.items():
-            d[k] = np.array(v, copy=copy)
-        for k, v in self._1d.items():
-            for i in range(self._nx):
-                d[str(i) + '.' + k] = np.array(v[:, i], copy=copy)
-        return d
+        log = DataLog()
+        log._time = self._time
+        for k, v in self.items():
+            log[k] = np.asarray(v)
+        return log
 
-    def trace(self, variable, x):
+    def _parse_key(self, key):
         """
-        Returns a 0d time series of the value ``variable``, corresponding to
-        the cell at position ``x``. The data is returned directly, no copy is
-        made.
+        Parses a key used for __getitem__, __setitem__, __delitem__ and
+        __contains__.
         """
-        return self._1d[variable][:, x]
+        if type(key) == tuple:
+            name = str(key[0])
+            if len(key) == 2 and type(key[1]) not in [int, float]:
+                parts = [str(x) for x in key[1]]
+            else:
+                parts = [str(x) for x in key[1:]]
+            parts.append(str(name))
+            key = '.'.join(parts)
+        return str(key)
+
+    def regularize(self, dt, tmin=None, tmax=None):  # pragma: no cover
+        """
+        Returns a copy of this DataLog with data points at regularly spaced
+        times.
+
+        This method is deprecated and will be removed in future versions of
+        Myokit.
+
+        This method requires ``SciPy`` to be installed.
+
+        *Note: While regularize() can be used post-simulation to create fixed
+        time-step data from variable time-step data, it is usually better to
+        re-run a simulation with fixed time step logging. See*
+        :meth:`Simulation.run()` *for details.*
+
+        The first point will be at ``tmin`` if specified or otherwise the first
+        time present in the log. All following points will be spaced ``dt``
+        time units apart and the final point will be less than or equal to
+        ``tmax``. If no value for ``tmax`` is given the final value in the log
+        is used.
+
+        This method works by
+
+          1. Finding the indices corresponding to ``tmin`` and ``tmax``.
+          2. Creating a spline interpolant with all the data from ``tmin`` to
+             ``tmax``. If possible, two points to the left and right of
+             ``tmin`` and ``tmax`` will be included in the interpolated data
+             set (so *only* if there are at least two values before ``tmin`` or
+             two values after ``tmax`` in the data respectively).
+          3. Evaluating the interpolant at the regularly spaced points.
 
+        As a result of the cubic spline interpolation, the function may perform
+        poorly on large data sets.
+        """
+        # Deprecated since 2023-06-06
+        import warnings
+        warnings.warn(
+            'The method `regularize` is deprecated and will be removed in'
+            ' future versions of Myokit.')
 
-class DataBlock2d:
-    """
-    Container for time-series of 2d rectangular data arrays.
+        from scipy.interpolate import UnivariateSpline as Spline
+        self.validate()
 
-    Each ``DataBlock2d`` has a fixed width ``w`` and height ``h``, and a 0d
-    time series vector containing a sequence of ``n`` times.
+        # Check time variable
+        time = self.time()
+        n = len(time)
 
-    Two-dimensional time series can be added to the block, provided the data
-    also contains ``n`` instances of ``w`` by ``h`` data points. The
-    data should be passed in as a numpy array with shape ``(n, h, w)``.
+        # Get left index for splines
+        imin = 0
+        if tmin is None:
+            tmin = time[0]
+        elif tmin > time[0]:
+            # Find position of tmin in time list, then add two points to the
+            # left so that the spline has 4 points
+            imin = max(0, np.searchsorted(time, tmin) - 2)
+
+        # Get right index for splines
+        imax = n
+        if tmax is None:
+            tmax = time[-1]
+        elif tmax < time[-1]:
+            imax = min(n, np.searchsorted(time, tmax) + 2)
+
+        # Get time steps
+        steps = 1 + np.floor((tmax - tmin) / dt)
+        rtime = tmin + dt * np.arange(0, steps)
+
+        # Create output and return
+        out = DataLog()
+        out._time = self._time
+        out[self._time] = rtime
+        time_part = time[imin:imax]
+        for key, data in self.items():
+            if key != self._time:
+                s = Spline(time_part, data[imin:imax], k=1, s=0)
+                out[key] = s(rtime)
+        return out
 
-    Zero-dimensional time series can be added, provided they have length ``n``.
+    def save(self, filename, precision=myokit.DOUBLE_PRECISION):
+        """
+        Writes this ``DataLog`` to a binary file.
 
-    A "two-dimensional time-series" is a series of equally sized 2d arrays
-    (sequences), such that the first corresponds to a time ``t[0]``, the second
-    to ``t[1]``, etc.
+        The resulting file will be a zip file with the following entries:
 
-    A "zero-dimensional time-series" is a series of single values where the
-    first corresponds to a time ``t[0]``, the second to ``t[1]``, etc.
+        ``header.txt``
+            A csv file with the fields ``name, dtype, len`` for each variable.
+        ``data.bin``
+            The binary data in the order specified by the header.
+        ``readme.txt``
+            A text file explaining the file format.
 
-    Constructor info:
+        The optional argument ``precision`` allows logs to be stored in single
+        precision format, which saves space.
+        """
+        self.validate()
 
-    ``w``
-        The width of a 2d block. Each block should have shape (n, h, w)
-    ``h``
-        The height of a 2d block. Each block should have shape (n, h, w)
-    ``time``
-        A sequence of ``n`` times.
-    ``copy``
-        By default, a copy of the given time sequence will be stored. To
-        prevent this copy, set ``copy=False``.
+        # Check filename
+        filename = os.path.expanduser(filename)
 
-    """
-    def __init__(self, w, h, time, copy=True):
-        # Width and height
-        w, h = int(w), int(h)
-        if w < 1:
-            raise ValueError('Minimum width is 1.')
-        if h < 1:
-            raise ValueError('Minimum height is 1.')
-        self._ny = h
-        self._nx = w
-        # Time
-        time = np.array(time, copy=copy)
-        if len(time.shape) != 1:
-            raise ValueError('Time must be a sequence.')
-        if not np.all(np.diff(time) >= 0):
-            raise ValueError('Time must be non-decreasing.')
-        self._time = time
-        self._nt = len(time)
-        # 0d variables
-        self._0d = {}
-        # 2d variables
-        self._2d = {}
+        # Load compression modules
+        import zipfile
+        try:
+            # Make sure zlib is available
+            import zlib
+            del zlib
+        except ImportError:
+            raise Exception(
+                'This method requires the `zlib` module to be installed.')
 
-    def colors(self, name, colormap='traditional', lower=None, upper=None,
-               multiplier=1):
-        """
-        Converts the 2d series indicated by ``name`` into a list of ``W*H*RGB``
-        arrays, with each entry represented as an 8 bit unsigned integer.
+        # Data type
+        dtype = 'd' if precision == myokit.DOUBLE_PRECISION else 'f'
 
-        Arguments:
+        # Create data strings
+        head_str = []
+        body_str = []   # Will be filled with bytes
 
-        ``name``
-            The 2d variable to create arrays for.
-        ``colormap``
-            The colormap to use when converting to RGB.
-        ``lower``
-            An optional lower bound on the data (anything below this will
-            become the lowest index in the colormap).
-        ``upper``
-            An optional upper bound on the data (anything above this will
-            become the highest index in the colormap).
-        ``multiplier``
-            An optional integer greater than zero. If given, every point in the
-            data set will be represented as a square of ``multiplier`` by
-            ``multiplier`` pixels.
-
-        """
-        data = self._2d[name]
-        # Get color map
-        color_map = ColorMap.get(colormap)
-        # Get lower and upper bounds for colormap scaling
-        lower = np.min(data) if lower is None else float(lower)
-        upper = np.max(data) if upper is None else float(upper)
-        # Get multiplier
-        multiplier = int(multiplier) if multiplier > 1 else 1
-        # Create images
-        frames = []
-        for frame in data:
-            # Convert 2d array into row-strided array
-            frame = frame.reshape(self._ny * self._nx, order='C')
-            # Apply colormap
-            frame = color_map(
-                frame, lower=lower, upper=upper, alpha=False, rgb=True)
-            # Reshape to nx * ny * 3 color array
-            frame = frame.reshape((self._ny, self._nx, 3))
-            # Grow
-            if multiplier > 1:
-                frame = frame.repeat(multiplier, axis=0)
-                frame = frame.repeat(multiplier, axis=1)
-            # Append to list
-            frames.append(frame)
-        return frames
+        # Number of fields, length of data arrays, data type, time, fields
+        head_str.append(str(len(self)))
+        head_str.append(str(len(next(iter(self.values())))))
+        head_str.append(dtype)
+
+        # Note: the time field might not be present in the log!
+        head_str.append(self._time if self._time else '')
+
+        # Write field names and data
+        enc = 'utf8'
+        for k, v in self.items():
+            head_str.append(k)
+            # Create array, ensure it's litte-endian
+            ar = array.array(dtype, v)
+            if sys.byteorder == 'big':  # pragma: no cover
+                ar.byteswap()
+            body_str.append(ar.tobytes())
+        head_str = '\n'.join(head_str)
+        body_str = b''.join(body_str)
 
-    @staticmethod
-    def combine(block1, block2, map2d, map0d=None, pos1=None, pos2=None):
-        """
-        Combines two blocks, containing information about different areas, into
-        a single :class:`DataBlock2d`.
+        # 2018-07-15: Wondering why I chose body-head-readme ordering now...
 
-        Both blocks must contain data from the same points in time.
+        # Write
+        head = zipfile.ZipInfo('structure.txt')
+        head.compress_type = zipfile.ZIP_DEFLATED
+        body = zipfile.ZipInfo('data.bin')
+        body.compress_type = zipfile.ZIP_DEFLATED
+        read = zipfile.ZipInfo('readme.txt')
+        read.compress_type = zipfile.ZIP_DEFLATED
+        with zipfile.ZipFile(filename, 'w') as f:
+            f.writestr(body, body_str)
+            f.writestr(head, head_str.encode(enc))
+            f.writestr(read, README_SAVE_BIN.encode(enc))
 
-        A mapping from old to new variables must be passed in as a dictionary
-        ``map2d``. The blocks can have different sizes but must have the same
-        time vector. If any empty space is created it is padded with a value
-        taken from one of the data blocks or a padding value specified as part
-        of ``map2d``.
-
-        Positions for the datablocks can be specified as ``pos1`` and ``pos2``,
-        the new datablock will have indices ranging from ``(0, 0)`` to
-        ``(max(pos1[0] + w1, pos2[0] + w2), max(pos1[0] + w1, pos2[0] + w2))``,
-        where ``w1`` and ``w2`` are the widths of ``block1`` and ``block2``
-        respectively. Negative indices are not supported and the blocks are not
-        allowed to overlap.
+    def save_csv(
+            self, filename, precision=myokit.DOUBLE_PRECISION, order=None,
+            delimiter=',', header=True):
+        """
+        Writes this ``DataLog`` to a CSV file, following the syntax
+        outlined in RFC 4180 and with a header indicating the field names.
+
+        The resulting file will consist of:
+
+          - A header line containing the names of all logged variables,
+            separated by commas. If present, the time variable will be the
+            first entry on the line. The remaining keys are ordered using a
+            natural sort order.
+          - Each following line will be a comma separated list of values in the
+            same order as the header line. A line is added for each time point
+            logged.
 
         Arguments:
 
-        ``block1``
-            The first DataBlock2d
-        ``block2``
-            The second DataBlock2d. This must have the same time vector as the
-            first.
-        ``map2d``
-            A dictionary object showing how to map 2d variables from both
-            blocks into the newly created datablock. The format must be:
-            ``new_name : (old_name_1, old_name_2, padding_value)``. Here,
-            ``new_name`` is the name of the new 2d variable, ``old_name_1`` is
-            the name of a 2d variable in ``block1``, ``old_name_2`` is the name
-            of a 2d variable in ``block2`` and ``padding_value`` is an optional
-            value indicating the value to use for undefined spaces in the new
-            block.
-        ``map0d=None``,
-            A dictionary object showing how to map 0d variables from both
-            blocks into the newly created datablock. Each entry must take the
-            format: ``new_name : (old_name_1, None)`` or
-            ``new_name : (None, old_name_2)``.
-        ``pos1=None``
-            Optional value indicating the position ``(x, y)`` of the first
-            datablock. By default ``(0, 0)`` is used.
-        ``pos2=None``
-            Optional value indicating the position ``(x, y)`` of the first
-            datablock. By default ``(w1, 0)`` is used, where ``w1`` is the
-            width of ``block1``.
-
-        """
-        # Check time vector
-        time = block1.time()
-        if not np.allclose(time, block2.time()):
-            raise ValueError(
-                'Both datablocks must contain data from the same points in'
-                ' time.')
+        ``filename``
+            The file to write (existing files will be overwritten without
+            warning.
+        ``precision``
+            If a precision argument (for example ``myokit.DOUBLE_PRECISION``)
+            is given, the output will be stored in such a way that this amount
+            of precision is guaranteed to be present in the string. If the
+            precision argument is set to ``None`` Python's default formatting
+            is used, which may lead to smaller files.
+        ``order``
+            To specify the ordering of the log's arguments, pass in a sequence
+            ``order`` with the log's keys.
+        ``delimiter``
+            This field can be used to set an alternative delimiter. To use
+            spaces set ``delimiter=' '``, for tabs: ``delimiter='\\t'``. Note
+            that some delimiters (for example '\\n' or '1234') will produce an
+            unreadable or invalid csv file.
+        ``header``
+            Set this to ``False`` to avoid adding a header to the file. Note
+            that Myokit will no longer be able to read the written csv file
+            without this header.
+
+        *A note about locale settings*: On Windows systems with a locale
+        setting that uses the comma as a decimal separator, importing CSV files
+        into Microsoft Excel can be troublesome. To correctly import a CSV,
+        either (1) Change your locale settings to use "." as a decimal
+        separator or (2) Use the import wizard under Data > Get External Data
+        to manually specify the correct separator and delimiter.
+        """
+        self.validate()
 
-        # Check indices
-        nt, h1, w1 = block1.shape()
-        nt, h2, w2 = block2.shape()
-
-        if pos1:
-            x1, y1 = [int(i) for i in pos1]
-            if x1 < 0 or y1 < 0:
-                raise ValueError(
-                    'Negative indices not supported: pos1=('
-                    + str(x1) + ', ' + str(y1) + ').')
-        else:
-            x1, y1 = 0, 0
+        # Check filename
+        filename = os.path.expanduser(filename)
 
-        if pos2:
-            x2, y2 = [int(i) for i in pos2]
-            if x2 < 0 or y2 < 0:
-                raise ValueError(
-                    'Negative indices not supported: pos2=('
-                    + str(x2) + ', ' + str(y2) + ').')
+        # Set precision
+        if precision is None:
+            fmat = lambda x: str(x)
+        elif precision == myokit.DOUBLE_PRECISION:
+            fmat = lambda x: myokit.SFDOUBLE.format(x)
+        elif precision == myokit.SINGLE_PRECISION:
+            fmat = lambda x: myokit.SFSINGLE.format(x)
         else:
-            x2, y2 = x1 + w1, 0
+            raise ValueError('Precision level not supported.')
 
-        # Check for overlap
-        if not (x1 >= x2 + w2 or x2 >= x1 + w1
-                or y1 >= y2 + h2 or y2 >= y1 + h2):
-            raise ValueError('The two data blocks indices cannot overlap.')
-
-        # Create new datablock
-        nx = max(x1 + w1, x2 + w2)
-        ny = max(y1 + h1, y2 + h2)
-        block = DataBlock2d(nx, ny, time, copy=True)
-
-        # Enter 0d data
-        if map0d:
-            for name, old in map0d.items():
-                if old[0] is None:
-                    b = block2
-                    n = old[1]
-                elif old[1] is None:
-                    b = block1
-                    n = old[0]
-                else:
+        # Write file
+        # EOL: CSV files have DOS line endings by convention. On windows,
+        # writing '\n' to a file opened in mode 'w' will actually write '\r\n'
+        # which means writing '\r\n' writes '\r\r\n'. To prevent this, open the
+        # file in mode 'wb'.
+        eol = '\r\n'
+        quote = '"'
+        escape = '""'
+        with open(filename, 'wb') as f:
+            # Convert dict structure to ordered sequences
+            if order:
+                order = [str(x) for x in order]
+                if set(order) != set(self.keys()):
                     raise ValueError(
-                        'The dictionary map0d must map the names of new 0d'
-                        ' entries to a tuple (a, b) where either a or b must'
-                        ' be None.')
-                block.set0d(name, b.get0d(n))
-
-        # Enter 2d data
-        for name, source in map2d.items():
-            # Get data sources
-            name1, name2 = source[0], source[1]
-            source1 = block1.get2d(name1)
-            source2 = block2.get2d(name2)
-
-            # Get padding value
-            try:
-                pad = float(source[2])
-            except IndexError:
-                # Get lowest value
-                pad = min(np.min(source1), np.min(source2))
+                        'The given `order` sequence must contain all the same'
+                        ' keys present in the log.')
+                keys = order
+                data = [self[x] for x in keys]
+            else:
+                keys = []
+                data = []
+                if self._time and self._time in self.keys():
+                    # Save time as first variable
+                    dat = self[self._time]
+                    keys.append(self._time)
+                    data.append(dat)
+                for key, dat in sorted(
+                        self.items(),
+                        key=lambda i: myokit.tools.natural_sort_key(i[0])):
+                    if key != self._time:
+                        keys.append(key)
+                        data.append(dat)
+
+            # Number of entries
+            m = len(keys)
+            if m == 0:
+                return
+
+            # Get length of entries
+            n = self.length()
+
+            # Write header
+            if header:
+                line = []
+                for key in keys:
+                    # Escape quotes within strings
+                    line.append(quote + key.replace(quote, escape) + quote)
+                f.write((delimiter.join(line) + eol).encode('ascii'))
+
+            # Write data
+            data = [iter(x) for x in data]
+            for i in range(0, n):
+                line = []
+                for d in data:
+                    line.append(fmat(next(d)))
+                f.write((delimiter.join(line) + eol).encode('ascii'))
+
+    def set_time_key(self, key):
+        """
+        Sets the key under which the time data is stored.
+        """
+        self._time = None if key is None else str(key)
+
+    def __setitem__(self, key, value):
+        return super().__setitem__(
+            self._parse_key(key), value)
+
+    def split(self, value):
+        """
+        Splits the log into a part before and after the time ``value``::
+
+            s = myokit.Simulation(m, p)
+            d = s.run(1000)
+            d1, d2 = d.split(100)
+
+        In this example, d1 will contain all values up to, but not including,
+        t=100. While d2 will contain the values from t=100 and upwards.
+        """
+        return self.isplit(self.find_after(value))
+
+    def split_periodic(self, period, adjust=False, closed_intervals=True):
+        """
+        Splits this log into multiple logs, each covering an equal period of
+        time. For example a log covering the time span ``[0, 10000]`` can be
+        split with period ``1000`` to obtain ten logs covering ``[0, 1000]``,
+        ``[1000, 2000]`` etc.
+
+        The split log files can be returned as-is, or with the time variable's
+        value adjusted so that all logs appear to cover the same span. To
+        enable this option, set ``adjust`` to ``True``.
+
+        By default, the returned intervals are *closed*, so both the left and
+        right endpoint are included (if present in the data). This may involve
+        the duplication of some data points. To disable this behavior and
+        return half-closed endpoints (containing only the left point), set
+        ``closed_intervals`` to ``False``.
+        """
+        # Validate log before starting
+        self.validate()
 
-            # Create new data field
-            field = pad * np.ones((nt, ny, nx))
-            field[:, y1:y1 + h1, x1:x1 + w1] = source1
-            field[:, y2:y2 + h2, x2:x2 + w2] = source2
-            block.set2d(name, field)
+        # Check time variable
+        time = self.time()
+        if len(time) < 1:
+            raise RuntimeError('DataLog entries have zero length.')
+
+        # Check period
+        period = float(period)
+        if period <= 0:
+            raise ValueError('Period must be greater than zero')
+
+        # Get start, end, etc
+        tmin = 0    # time[0]
+        tmax = time[len(time) - 1]
+        nlogs = int(np.ceil((tmax - tmin) / period))
+
+        # No splitting needed? Return clone!
+        if nlogs < 2:
+            return self.clone()
+
+        # Find split points
+        tstarts = tmin + np.arange(nlogs) * period
+        istarts = [0] * nlogs
+        k = 0
+        for i, t in enumerate(time):
+            while k < nlogs and t >= tstarts[k]:
+                istarts[k] = i
+                k += 1
+
+        # Create logs
+        logs = []
+        for i in range(0, nlogs - 1):
+            log = DataLog()
+            log._time = self._time
+
+            # Get indices
+            imin = istarts[i]
+            imax = istarts[i + 1]
+
+            # Include right point endpoint if needed
+            if closed_intervals and time[imax] == tstarts[i + 1]:
+                imax += 1
+
+            # Select sections of log and append
+            for k, v in self.items():
+                d = self[k][imin:imax]
+                # NumPy? Then copy data
+                if isinstance(d, np.ndarray):
+                    d = np.array(d, copy=True, dtype=float)
+                log[k] = d
+            logs.append(log)
+
+        # Last log
+        log = DataLog()
+        log._time = self._time
+        imin = istarts[-1]
+        imax = len(time)
+
+        # Not including right endpoints? Then may be required to omit last pt
+        if not closed_intervals and time[-1] >= tmin + nlogs * period:
+            imax -= 1
+
+        # Select sections of log and append
+        for k, v in self.items():
+            d = self[k][imin:imax]
+            # NumPy? Then copy data
+            if isinstance(d, np.ndarray):
+                d = np.array(d, copy=True, dtype=float)
+            log[k] = d
+        logs.append(log)
+
+        # Adjust
+        if adjust:
+            if isinstance(time, np.ndarray):
+                # Fast method for numpy arrays
+                for k, log in enumerate(logs):
+                    log[self._time] -= k * period
+            else:
+                for k, log in enumerate(logs):
+                    tlist = log[self._time]
+                    tdiff = k * period
+                    for i in range(len(tlist)):
+                        tlist[i] -= tdiff
 
-        # Return new block
-        return block
+        # Return
+        return logs
 
-    def dominant_eigenvalues(self, name):
+    def time(self):
         """
-        Takes the 2d data specified by ``name`` and computes the dominant
-        eigenvalue for each point in time (this only works for datablocks with
-        a square 2d grid).
-
-        The "dominant eigenvalue" is defined as the eigenvalue with the largest
-        magnitude (``sqrt(a + bi)``).
+        Returns this log's time array.
 
-        The returned data is a 1d numpy array.
+        Raises a :class:`myokit.InvalidDataLogError` if the time variable for
+        this log has not been specified or an invalid key was given for the
+        time variable.
         """
-        if self._nx != self._ny:
-            raise Exception(
-                'Eigenvalues can only be determined for square data blocks.')
-        data = self._2d[name]
-        dominants = []
-        for t in range(self._nt):
-            e = np.linalg.eigvals(data[t])
-            dominants.append(e[np.argmax(np.absolute(e))])
-        return np.array(dominants)
-
-    def eigenvalues(self, name):
-        """
-        Takes the 2d data specified as ``name`` and computes the eigenvalues of
-        its data matrix at every point in time (this only works for datablocks
-        with a square 2d grid).
+        try:
+            return self[self._time]
+        except KeyError:
+            if self._time is None:
+                raise myokit.InvalidDataLogError('No time variable set.')
+            else:
+                raise myokit.InvalidDataLogError(
+                    'Invalid key <' + str(self._time)
+                    + '> set for time variable.')
 
-        The returned data is a 2d numpy array where the first axis is time and
-        the second axis is the index of each eigenvalue.
+    def time_key(self):
         """
-        if self._nx != self._ny:
-            raise Exception(
-                'Eigenvalues can only be determined for square data blocks.')
-        data = self._2d[name]
-        eigenvalues = []
-        for t in range(self._nt):
-            eigenvalues.append(np.linalg.eigvals(data[t]))
-        return np.array(eigenvalues)
-
-    @staticmethod
-    def from_DataLog(log):
-        """Deprecated alias of :meth:`from_log()`."""
-        # Deprecated since 2020-09-14
-        import warnings
-        warnings.warn(
-            'The method `DataBlock2d.from_DataLog` is deprecated. Please use'
-            ' `DataBlock2d.from_log` instead.')
-        return DataBlock2d.from_log(log)
-
-    @staticmethod
-    def from_log(log):
+        Returns the name of the time variable stored in this log, or ``None``
+        if no time variable was set.
         """
-        Creates a DataBlock2d from a :class:`myokit.DataLog`.
+        return self._time
+
+    def trim(self, a, b, adjust=False):
         """
-        log.validate()
+        Returns a copy of this log, with all data before time ``a`` and after
+        (and including) time ``b`` removed.
 
-        # Get time variable name
-        time = log.time_key()
-        if time is None:
-            raise ValueError('No time variable set in data log.')
+        If ``adjust`` is set to ``True``, all logged times will be lowered by
+        ``a``.
+        """
+        self.validate()
+        log = self.itrim(self.find_after(a), self.find_after(b))
+        if adjust and self._time in log:
+            if isinstance(log[self._time], np.ndarray):
+                log[self._time] -= a
+            else:
+                log[self._time] = [x - a for x in log[self._time]]
+        return log
 
-        # Get log info
-        infos = log.variable_info()
+    def trim_left(self, value, adjust=False):
+        """
+        Returns a copy of this log, with all data before time ``value``
+        removed.
 
-        # Check time variable
-        if time not in infos:
-            # Already checked time variable exists, so if not found now must
-            # be multi-dimensional
-            raise ValueError('Time variable must be 0-dimensional.')
-
-        # Check if everything is 0d or 2d, get size
-        size = None
-        for name, info in infos.items():
-            d = info.dimension()
-            if d not in (0, 2):
-                raise ValueError(
-                    'The given simulation log should only contain 0d or 2d'
-                    ' variables. Found <' + str(name) + '> with d = '
-                    + str(d) + '.')
-            if d == 2:
-                if size is None:
-                    size = info.size()
-                elif info.size() != size:
-                    raise ValueError(
-                        'The given simulation log contains 2d data sets of'
-                        ' different sizes.')
-        # Get dimensions
-        nt = len(log[time])
-        nx, ny = size
-        # Create data block
-        block = DataBlock2d(nx, ny, log[time], copy=True)
-        for name, info in infos.items():
-            if info.dimension() == 0:
-                # Add 0d time series
-                if name == time:
-                    continue
-                block.set0d(name, log[name], copy=True)
+        If ``adjust`` is set to ``True``, all logged times will be lowered by
+        ``value``.
+        """
+        self.validate()
+        log = self.itrim_left(self.find_after(value))
+        if adjust and self._time in log:
+            if isinstance(log[self._time], np.ndarray):
+                log[self._time] -= value
             else:
-                # Convert to 2d time series
-                data = np.zeros(nt * ny * nx)
-                # Iterate over info.keys()
-                for i, key in enumerate(info.keys()):
-                    # Copy data into array (really copies)
-                    data[i * nt:(i + 1) * nt] = log[key]
-                # Reshape
-                data = data.reshape((nt, ny, nx), order='F')
-                # If this is a view of existing data, make a copy!
-                if data.base is not None:
-                    data = np.array(data)
-                block.set2d(name, data, copy=False)
-        return block
+                log[self._time] = [x - value for x in log[self._time]]
+        return log
 
-    def get0d(self, name):
+    def trim_right(self, value):
         """
-        Returns the 0d time-series identified by ``name``. The data is returned
-        directly, no copy is made.
+        Returns a copy of this log, with all data at times after and including
+        ``value`` removed.
         """
-        return self._0d[name]
+        return self.itrim_right(self.find_after(value))
+
+    def validate(self):
+        """
+        Validates this ``DataLog``. Raises a
+        :class:`myokit.InvalidDataLogError` if the log has inconsistencies.
+        """
+        if self._time:
+            if self._time not in self:
+                raise myokit.InvalidDataLogError(
+                    'Time variable <' + str(self._time)
+                    + '> specified but not found in log.')
+            dt = np.asarray(self[self._time])
+            if np.any(dt[1:] - dt[:-1] < 0):
+                raise myokit.InvalidDataLogError(
+                    'Time must be non-decreasing.')
+        if len(self) > 0:
+            n = set([len(v) for v in self.values()])
+            if len(n) > 1:
+                raise myokit.InvalidDataLogError(
+                    'All entries in a data log must have the same length.')
+
+    def variable_info(self):
+        """
+        Returns a dictionary mapping fully qualified variable names to
+        :class:`LoggedvariableInfo` instances, providing information about the
+        logged data.
+
+        Comes with the following constraints:
+
+        - Per variable, the data must have a consistent dimensionality. For
+          example having a key ``0.membrane.V`` and a key ``1.1.membrane.V``
+          would violate this constraint.
+        - Per variable, the data must be regular accross dimensions. For
+          example if there are ``n`` entries ``0.x.membrane.V``, and there are
+          also entries of the form ``1.x.membrane.V`` then the values of ``x``
+          must be the same for both cases.
+
+        An example of a dataset that violates the second constraint is::
+
+            0.0.membrane.V
+            0.1.membrane.V
+            0.2.membrane.V
+            1.0.membrane.V
+            1.1.membrane.V
+
+        If either of the constraints is violated a ``ValueError`` is raised.
+        """
+        # The algorithm for condition 2 works by creating a set of the unique
+        # entries in each column. The product of the sizes of these sets should
+        # equal the total number of entries for a variable.
+        # For example:
+        #   0 1
+        #   0 2     Results in id_sets [(0,1), (1,2,3,4)]
+        #   0 3     2 * 4 = 8 != len(id_list)
+        #   1 1     So this data must be irregular.
+        #   1 2
+        #   1 4
+        #
+        id_lists = {}
+        id_sets = {}
+        for key in self:
+            # Split key into id / name parts
+            idx, name = split_key(key)
+
+            # Create tuple version of id
+            idx = idx.split('.')
+            idx = idx[:-1]
+            idx = tuple([int(i) for i in idx])
 
-    def get2d(self, name):
-        """
-        Returns the 2d time-series identified by ``name``. The data is returned
-        directly, no copy is made.
-        """
-        return self._2d[name]
+            # Find or create entry in dict of id lists
+            try:
+                id_list = id_lists[name]
+                id_set = id_sets[name]
+            except KeyError:
+                # Create entry in id lists dict
+                id_lists[name] = id_list = []
+
+                # Create entry in id sets dict (one set for every dimension)
+                id_sets[name] = id_set = [set() for x in idx]
+
+            # Check if the dimensions are the same each time a name occurs.
+            if id_list and len(id_list[0]) != len(idx):
+                key1 = '.'.join([str(x) for x in id_list[0]]) + '.' + name
+                key2 = '.'.join([str(x) for x in idx]) + '.' + name
+                raise RuntimeError(
+                    'Different dimensions used for the same variable. Found: <'
+                    + key1 + '> and <' + key2 + '>.')
+
+            # Update the id list
+            id_list.append(idx)
+
+            # Update the id set
+            for k, i in enumerate(idx):
+                id_set[k].add(i)
+
+        # Create variable info objects
+        infos = {}
+        for name, id_list in id_lists.items():
+            id_set = id_sets[name]
+
+            # Check if the data is regular.
+            n = len(id_list)
+            m = 1
+            for x in id_set:
+                m *= len(x)
+
+            if n != m:
+                raise RuntimeError(
+                    'Irregular data used for variable <' + str(name) + '>')
+
+            # Create variable info object
+            infos[name] = info = LoggedVariableInfo()
+            info._name = name
+            info._dimension = len(id_set)
+            info._size = tuple([len(x) for x in id_set])
+
+            # Add sorted ids
+            if id_list[0]:
+                id_list.sort()
+            info._ids = id_list
+
+            # Add sorted keys
+            s = '.' + name if id_list[0] else name
+            info._keys = ['.'.join([str(x) for x in y]) + s for y in id_list]
 
-    def images(self, name, colormap='traditional', lower=None, upper=None):
-        """
-        Converts the 2d series indicated by ``name`` into a list of 1d arrays
-        in a row-strided image format ``ARGB32``.
-        """
-        data = self._2d[name]
-        # Get color map
-        color_map = ColorMap.get(colormap)
-        # Get lower and upper bounds for colormap scaling
-        lower = np.min(data) if lower is None else float(lower)
-        upper = np.max(data) if upper is None else float(upper)
-        # Create images
-        frames = []
-        for frame in data:
-            # Convert 2d array into row-strided array
-            frame = frame.reshape(self._ny * self._nx, order='C')
-            frames.append(color_map(frame, lower=lower, upper=upper))
-        return frames
+        return infos
 
-    def is_square(self):
-        """
-        Returns True if this data block's grid is square.
-        """
-        return self._nx == self._ny
 
-    def items0d(self):
-        """
-        Returns an iterator over ``(name, value)`` pairs for the 0d series
-        stored in this block. The given values are references! No copy of the
-        data is made.
-        """
-        return self._0d.items()
+class LoggedVariableInfo:
+    """
+    Contains information about the log entries for each variable. These objects
+    should only be created by :meth:`DataLog.variable_info()`.
+    """
+    def __init__(self):
+        self._dimension = None
+        self._ids = None
+        self._keys = None
+        self._size = None
+        self._name = None
 
-    def items2d(self):
+    def dimension(self):
         """
-        Returns an iterator over ``(name, value)`` pairs for the 2d series
-        stored in this block. The given values are references! No copy of the
-        data is made.
+        Returns the dimensions of the logged data for this variable, as an
+        integer.
         """
-        return self._2d.items()
+        return self._dimension
 
-    def keys0d(self):
-        """
-        Returns an iterator over this block's 0d time series.
+    def ids(self):
         """
-        return iter(self._0d)
+        Returns an iterator over all available ids for this variable, such
+        that the second index (y in the simulation) changes fastest. For
+        example, for log entries::
 
-    def keys2d(self):
-        """
-        Returns an iterator over this block's 2d time series.
-        """
-        return iter(self._2d)
+            0.0.membrane.V
+            0.1.membrane.V
+            0.2.membrane.V
+            1.0.membrane.V
+            1.1.membrane.V
+            1.2.membrane.V
 
-    def largest_eigenvalues(self, name):
-        """
-        Takes the 2d data specified by ``name`` and computes the largest
-        eigenvalue for each point in time (this only works for datablocks with
-        a square 2d grid).
+        the returned result would iterate over::
 
-        The "largest eigenvalue" is defined as the eigenvalue with the most
-        positive real part. Note that the returned values may be complex.
+            [(0, 0), (0, 1), (0, 2), (1, 0), (1, 1), (1, 2)]
 
-        The returned data is a 1d numpy array.
+        The keys are returned in the same order as the ids.
         """
-        if self._nx != self._ny:
-            raise Exception(
-                'Eigenvalues can only be determined for square data blocks.')
-        data = self._2d[name]
-        largest = []
-        for t in range(self._nt):
-            e = np.linalg.eigvals(data[t])
-            largest.append(e[np.argmax(np.real(e))])
-        return np.array(largest)
+        return iter(self._ids)
 
-    def len0d(self):
+    def is_regular_grid(self):
         """
-        Returns the number of 0d time series in this block.
-        """
-        return len(self._0d)
+        Returns True if the following conditions are met:
+
+        - The data 2 dimensional
+        - The data is continuous: along each dimension the first data point is
+          indexed as ``0`` and the last as ``Ni-1``, where ``Ni`` is the size
+          in that dimension.
 
-    def len2d(self):
-        """
-        Returns the number of 2d time series in this block.
         """
-        return len(self._2d)
+        nx, ny = self._size
+        return (
+            self._dimension == 2
+            and self._ids[0][0] == 0
+            and self._ids[0][1] == 0
+            and self._ids[-1][0] == nx - 1
+            and self._ids[-1][1] == ny - 1
+        )
 
-    @staticmethod
-    def load(filename, progress=None, msg='Loading DataBlock2d'):
+    def keys(self):
         """
-        Loads a :class:`DataBlock2d` from the specified file.
+        Returns an iterator over all available keys for this variable, such
+        that the second index (y in the simulation) changes fastest. For
+        example, for log entries::
 
-        To obtain feedback on the simulation progress, an object implementing
-        the :class:`myokit.ProgressReporter` interface can be passed in.
-        passed in as ``progress``. An optional description of the current
-        simulation to use in the ProgressReporter can be passed in as `msg`.
+            0.0.membrane.V
+            1.0.membrane.V
+            0.1.membrane.V
+            1.1.membrane.V
+            0.2.membrane.V
+            1.2.membrane.V
 
-        If the given file contains a :class:`DataBlock1d` this is read and
-        converted to a 2d block without warning.
+        the returned iterator would produce ``"0.0.membrane.V"``, then
+        ``"0.1.membrane.V"`` etc.
+
+        The ids are returned in the same order as the keys.
         """
-        filename = os.path.expanduser(filename)
+        return iter(self._keys)
 
-        # Load compression modules
-        import zipfile
-        try:
-            import zlib
-            del zlib
-        except ImportError:
-            raise Exception(
-                'This method requires the ``zlib`` module to be installed.')
+    def size(self):
+        """
+        Returns a tuple containing the size i.e. the number of entries for
+        the corresponding variable in each dimension.
 
-        # Get size of single and double types on this machine
-        dsize = {
-            'd': len(array.array('d', [1]).tobytes()),
-            'f': len(array.array('f', [1]).tobytes()),
-        }
+        For example, with the following log entries for `membrane.V`::
 
-        # Read data from file
-        try:
-            f = None
-            f = zipfile.ZipFile(filename, 'r')
-            info = f.infolist()
-            if len(info) < 3:
-                raise myokit.DataBlockReadError(
-                    'Invalid DataBlock2d file format: Not enough files in'
-                    ' zip.')
+            0.membrane.V
+            1.membrane.V
+            2.membrane.V
 
-            # Get ZipInfo objects
-            names = [x.filename for x in info]
-            try:
-                head = names.index('header_block2d.txt')
-            except ValueError:
-                # Attempt reading as DataBlock1d
-                try:
-                    names.index('header_block1d.txt')
-                except ValueError:
-                    raise myokit.DataBlockReadError(
-                        'Invalid DataBlock2d file format: Header not found.')
+        the corresponding size would be ``(3)``.
 
-                # It's a DataBlock1d, attempt reading as such
-                f.close()
-                block1d = DataBlock1d.load(filename, progress, msg)
-                return None if block1d is None else block1d.block2d()
+        A size of ``3`` doesn't guarantee the final entry is for cell number
+        ``2``. For example::
 
-            try:
-                body = names.index('data.bin')
-            except ValueError:
-                raise myokit.DataBlockReadError(
-                    'Invalid DataBlock2d file format: Data not found.')
-
-            # Read head and body into memory (let's assume it fits...)
-            head = f.read(info[head]).decode(ENC)
-            body = f.read(info[body])
+            0.membrane.V
+            10.membrane.V
+            20.membrane.V
 
-        except zipfile.BadZipfile:
-            raise myokit.DataBlockReadError(
-                'Unable to read DataBlock2d: Bad zip file.')
+        would also return size ``(3)``
 
-        except zipfile.LargeZipFile:    # pragma: no cover
-            raise myokit.DataBlockReadError(
-                'Unable to read DataBlock2d: zip file requires zip64 support'
-                ' and this has not been enabled on this system.')
+        In higher dimensions::
 
-        finally:
-            if f:
-                f.close()
+            0.0.membrane.V
+            0.1.membrane.V
+            0.2.membrane.V
+            1.0.membrane.V
+            1.1.membrane.V
+            1.2.membrane.V
 
-        # Parse head
-        head = head.splitlines()
-        try:
-            if progress:
-                progress.enter(msg)
-                # Avoid divide by zero
-                fraction = float(len(head) - 4)
-                if fraction > 0:
-                    fraction = 1.0 / fraction
-                iprogress = 0
-                progress.update(iprogress * fraction)
-            head = iter(head)
-            nt = int(next(head))
-            ny = int(next(head))
-            nx = int(next(head))
-
-            # Get dtype
-            dtype = next(head)[1:-1]
-            if dtype not in dsize:
-                raise myokit.DataBlockReadError(
-                    'Unable to read DataBlock2d: Unrecognized data type "'
-                    + str(dtype) + '".')
-
-            names_0d = []
-            names_2d = []
-            name = next(head)
-            while name != '2':
-                names_0d.append(name[1:-1])
-                name = next(head)
-            for name in head:
-                names_2d.append(name[1:-1])
-            del head
-
-            # Parse body
-            start, end = 0, 0
-            n0 = dsize[dtype] * nt
-            n2 = n0 * ny * nx
-            nb = len(body)
-
-            # Read time
-            end += n0
-            if end > nb:
-                raise myokit.DataBlockReadError(
-                    'Unable to read DataBlock2d: Header indicates larger data'
-                    ' than found in the body.')
+        This would return ``(2,3)``.
 
-            data = array.array(dtype)
-            data.frombytes(body[start:end])
-            if sys.byteorder == 'big':  # pragma: no cover
-                data.byteswap()
-            data = np.array(data)
-            if progress:
-                iprogress += 1
-                if not progress.update(iprogress * fraction):
-                    return
+        Similarly, in a single cell scenario or for global variables, for
+        exmaple::
 
-            # Create data block
-            block = DataBlock2d(nx, ny, data, copy=False)
+            engine.time
 
-            # Read 0d data
-            for name in names_0d:
-                start = end
-                end += n0
-                if end > nb:
-                    raise myokit.DataBlockReadError(
-                        'Unable to read DataBlock2d: Header indicates larger'
-                        ' data than found in the body.')
-                data = array.array(dtype)
-                data.frombytes(body[start:end])
-                if sys.byteorder == 'big':  # pragma: no cover
-                    data.byteswap()
-                data = np.array(data)
-                block.set0d(name, data, copy=False)
-                if progress:
-                    iprogress += 1
-                    if not progress.update(iprogress * fraction):
-                        return
+        Would have size ``()``.
+        """
+        return self._size
 
-            # Read 2d data
-            for name in names_2d:
-                start = end
-                end += n2
-                if end > nb:
-                    raise myokit.DataBlockReadError(
-                        'Unable to read DataBlock2d: Header indicates larger'
-                        ' data than found in the body.')
-                data = array.array(dtype)
-                data.frombytes(body[start:end])
-                if sys.byteorder == 'big':  # pragma: no cover
-                    data.byteswap()
-                data = np.array(data).reshape(nt, ny, nx, order='C')
-                block.set2d(name, data, copy=False)
-                if progress:
-                    iprogress += 1
-                    if not progress.update(iprogress * fraction):
-                        return
-            return block
+    def name(self):
+        """
+        Returns the variable name.
+        """
+        return self._name
 
-        finally:
+    def to_long_string(self):   # pragma: no cover (debug function)
+        out = [self._name]
+        out.append('  dimension: ' + str(self._dimension))
+        out.append('  size: ' + ', '.join([str(x) for x in self._size]))
+        out.append('  keys:')
+        out.extend(['    ' + x for x in self._keys])
+        return '\n'.join(out)
 
-            if progress:
-                progress.exit()
 
-    def remove0d(self, name):
-        """Removes the 0d time-series identified by ``name``."""
-        del self._0d[name]
+def prepare_log(
+        log, model, dims=None, global_vars=None, if_empty=myokit.LOG_NONE,
+        allowed_classes=myokit.LOG_ALL, precision=myokit.DOUBLE_PRECISION):
+    """
+    Returns a :class:`DataLog` for simulation classes based on a ``log``
+    argument passed in by the user. The model the simulations will be based on
+    should be passed in as ``model``.
+
+    The ``log`` argument can take on one of four forms:
+
+    An existing simulation log
+        In this case, the log is tested for compatibility with the given model
+        and simulation dimensions. For single-cell simulations all keys in the
+        log must correspond to the qname of a loggable variable (IE not a
+        constant). For multi-cellular simulations this means all keys in the
+        log must have the form "x.component.variable" where "x" is the cell
+        index (for example "1" or "0.3").
+    A list (or other sequence) of variable names to log.
+        In this case, the list is converted to a DataLog object. All
+        arguments in the list must be either strings corresponding to the
+        variables' qnames (so "membrane.V") or variable objects from the given
+        model.
+        In multi-cell scenarios, passing in the qname of a variable (for
+        example "membrane.V") will cause every cell's instance of this variable
+        to be logged. To log only specific cells' values, pass in the indexed
+        name (for example "1.2.membrane.V").
+    An integer flag
+        One of the following integer flags:
+
+        ``myokit.LOG_NONE``
+            Don't log any variables.
+        ``myokit.LOG_STATE``
+            Log all state variables.
+        ``myokit.LOG_BOUND``
+            Log all variables bound to an external value. The method will
+            assume any bound variables still present in the model will be
+            provided by the simulation engine.
+        ``myokit.LOG_INTER``
+            Log all intermediary variables.
+        ``myokit.LOG_DERIV``
+            Log the derivatives of the state variables.
+        ``myokit.LOG_ALL``
+            Combines all the previous flags.
+
+        Flags can be chained together, for example
+        ``log=myokit.LOG_STATE+myokit.LOG_BOUND`` will log all bound variables
+        and all states.
+    ``None``
+        In this case the value from ``if_empty`` will be copied into log before
+        the function proceeds to build a log.
+
+    For multi-dimensional logs the simulation dimensions can be passed in as a
+    tuple of dimension sizes, for example (10,) for a cable of 10 cells and
+    (30,20) for a 30 by 20 piece of tissue.
+
+    Simulations can define variables to be either `per-cell` or `global`. Time,
+    for example, is typically a global variable while membrane potential will
+    be stored per cell. To indicate which is which, a list of global variables
+    can be passed in as ``global_vars``.
+
+    The argument ``if_empty`` is used to set a default argument if ``log`` is
+    is given as ``None``.
+
+    The argument ``allowed_classes`` is an integer flag that determines which
+    type of variables are allowed in this log.
+
+    When a new DataLog is created by this method, the internal storage
+    uses arrays from the array module. The data type for these new arrays can
+    be specified using the ``precision`` argument.
+    """
+    # Typecode dependent on precision
+    typecode = 'd' if precision == myokit.DOUBLE_PRECISION else 'f'
 
-    def remove2d(self, name):
-        """Removes the 2d time-series identified by ``name``."""
-        del self._2d[name]
+    # Get all options for dimensionality
+    if dims is None:
+        dims = ()
+    ndims = len(dims)
+    if ndims == 0:
+        dcombos = ['']
+    else:
+        dcombos = ['.'.join([str(y) for y in x]) + '.' for x in _dimco(*dims)]
+
+    # Check given list of global variables
+    if global_vars is None:
+        global_vars = []
+    else:
+        for var in global_vars:
+            try:
+                v = model.get(var)
+            except KeyError:
+                raise ValueError(
+                    'Unknown variable specified in global_vars <'
+                    + str(var) + '>.')
+            if v.is_state():
+                raise ValueError('State cannot be global variable.')
+
+    # Function to check if variable is allowed (doesn't handle derivatives)
+    def check_if_allowed_class(var):
+        if var.is_constant():
+            raise ValueError(
+                'This log does not support constants, got <'
+                + str(var) + '>.')
+        elif var.is_state():
+            if not myokit.LOG_STATE & allowed_classes:
+                raise ValueError(
+                    'This log does not support state variables, got <'
+                    + str(var) + '>.')
+        elif var.is_bound():
+            if not myokit.LOG_BOUND & allowed_classes:
+                raise ValueError(
+                    'This log does not support bound variables, got <'
+                    + str(var) + '>.')
+        elif not myokit.LOG_INTER & allowed_classes:
+            raise ValueError(
+                'This log does not support intermediary variables, got <'
+                + str(var) + '>.')
 
-    def save(self, filename):
-        """
-        Writes this ``DataBlock2d`` to a binary file.
+    #
+    # First option, no log argument given, use the "if_empty" option
+    #
+
+    if log is None:
+        # Check if if_empty matches allowed_classes
+        # (AKA test if ``if_empty`` is contained in ``allowed_classes``)
+        if if_empty & allowed_classes == if_empty:
+            log = if_empty
+        else:
+            # This one's only for programmers :-)
+            raise ValueError(
+                'The option given for `if_empty` should be an allowed class.')
 
-        The resulting file will be a zip file with the following entries:
+    #
+    # Second option, log given as integer flag: create a simulation log and
+    # return it.
+    #
+
+    if type(log) == int:
+
+        # Log argument given as flag
+        flag = log
+        log = myokit.DataLog()
+        if flag == myokit.LOG_ALL:
+            flag = allowed_classes
+
+        if myokit.LOG_STATE & flag:
+
+            # Check if allowed
+            if not (myokit.LOG_STATE & allowed_classes):
+                raise ValueError('This log does not support state variables.')
+
+            # Add states
+            for s in model.states():
+                name = s.qname()
+                for c in dcombos:
+                    log[c + name] = array.array(typecode)
+            flag -= myokit.LOG_STATE
+
+        if myokit.LOG_BOUND & flag:
+
+            # Check if allowed
+            if not (myokit.LOG_BOUND & allowed_classes):
+                raise ValueError('This log does not support bound variables.')
+
+            # Add bound variables
+            for label, var in model.bindings():
+                name = var.qname()
+                if name in global_vars:
+                    log[name] = array.array(typecode)
+                else:
+                    for c in dcombos:
+                        log[c + name] = array.array(typecode)
+            flag -= myokit.LOG_BOUND
 
-        ``header_block2d.txt``: A header file containing the following
-        information (line by line):
+        if myokit.LOG_INTER & flag:
 
-        - ``nt`` the number of points in time in each entry
-        - ``ny`` the height of each 2d block
-        - ``nx`` the width of each 2d block
-        - ``"dtype"`` the used datatype (either "d" or "f")
-        - ``"name"`` the names of all 0d entries, each on its own line
-        - ``2`` the indication that the 2d entries are starting
-        - ``"name"`` the names of all 2d entries, each on its own line
-
-        ``data.bin``: A binary file containing the following data, in the data
-        type specified by the header, and little-endian:
-
-        - The ``nt`` time values
-        - All 0d entries
-        - All 2d entries, reshaped using numpy order='C'
+            # Check if allowed
+            if not (myokit.LOG_INTER & allowed_classes):
+                raise ValueError(
+                    'This log does not support intermediary variables.')
 
-        """
-        # Check filename
-        filename = os.path.expanduser(filename)
+            # Add intermediary variables
+            for var in model.variables(inter=True, deep=True):
+                name = var.qname()
+                if name in global_vars:
+                    log[name] = array.array(typecode)
+                else:
+                    for c in dcombos:
+                        log[c + name] = array.array(typecode)
+            flag -= myokit.LOG_INTER
+
+        if myokit.LOG_DERIV & flag:
+
+            # Check if allowed
+            if not (myokit.LOG_DERIV & allowed_classes):
+                raise ValueError('This log does not support time-derivatives.')
+
+            # Add state derivatives
+            for var in model.states():
+                name = var.qname()
+                for c in dcombos:
+                    log['dot(' + c + name + ')'] = array.array(typecode)
+            flag -= myokit.LOG_DERIV
+
+        if flag != 0:
+            raise ValueError('One or more unknown flags given as log.')
+
+        # Set time variable
+        time = model.time().qname()
+        if time in log:
+            log.set_time_key(time)
 
-        # Load compression modules
-        import zipfile
-        try:
-            # Check zlib is available
-            import zlib
-            del zlib
-        except ImportError:
-            raise Exception(
-                'This method requires the ``zlib`` module to be installed.')
+        # Return
+        return log
 
-        # Data type
-        dtype = 'd'     # Only supporting doubles right now
+    #
+    # Third option, a dict or DataLog is given. Test if it's suitable for this
+    # simulation.
+    #
 
-        # Create header
-        head_str = []
-        head_str.append(str(self._nt))
-        head_str.append(str(self._ny))
-        head_str.append(str(self._nx))
-        head_str.append('"' + dtype + '"')
-        for name in self._0d:
-            head_str.append('"' + name + '"')
-        head_str.append(str(2))
-        for name in self._2d:
-            head_str.append('"' + name + '"')
-        head_str = '\n'.join(head_str)
+    if isinstance(log, dict):
 
-        # Create body
-        n = self._nt * self._ny * self._nx
-        body_str = []
-        body_str.append(array.array(dtype, self._time))
-        for name, data in self._0d.items():
-            body_str.append(array.array(dtype, data))
-        for name, data in self._2d.items():
-            body_str.append(array.array(dtype, data.reshape(n, order='C')))
-        if sys.byteorder == 'big':  # pragma: no cover
-            for ar in body_str:
-                ar.byteswap()
-        body_str = b''.join([ar.tobytes() for ar in body_str])
+        # Ensure it's a DataLog
+        if not isinstance(log, myokit.DataLog):
+            log = myokit.DataLog(log)
 
-        # Write
-        head = zipfile.ZipInfo('header_block2d.txt')
-        head.compress_type = zipfile.ZIP_DEFLATED
-        body = zipfile.ZipInfo('data.bin')
-        body.compress_type = zipfile.ZIP_DEFLATED
-        read = zipfile.ZipInfo('readme.txt')
-        read.compress_type = zipfile.ZIP_DEFLATED
-        with zipfile.ZipFile(filename, 'w') as f:
-            f.writestr(head, head_str.encode(ENC))
-            f.writestr(body, body_str)
-            f.writestr(read, README_SAVE_2D.encode(ENC))
+        # Set time variable
+        time = model.time().qname()
+        if time in log:
+            log.set_time_key(time)
 
-    def save_frame_csv(
-            self, filename, name, frame, xname='x', yname='y', zname='value'):
-        """
-        Stores a single 2d variable's data at a single point in time to disk,
-        using a csv format where each point in the frame is stored on a
-        separate line as a tuple ``x, y, value``.
-        """
-        # Check filename
-        filename = os.path.expanduser(filename)
-        # Save
-        delimx = ','
-        delimy = '\n'
-        data = self._2d[name]
-        data = data[frame]
-        text = [delimx.join('"' + str(x) + '"' for x in [xname, yname, zname])]
-        for y, row in enumerate(data):
-            for x, z in enumerate(row):
-                text.append(delimx.join([str(x), str(y), myokit.float.str(z)]))
-        text = delimy.join(text)
-        with open(filename, 'w') as f:
-            f.write(text)
-
-    def save_frame_grid(self, filename, name, frame, delimx=' ', delimy='\n'):
-        """
-        Stores a single 2d variable's data at a single point in time to disk,
-        using a simple 2d format where each row of the resulting data file
-        represents a row of the frame.
-
-        Data from 2d variable ``name`` at frame ``frame`` will be stored in
-        ``filename`` row by row. Each column is separated by ``delimx`` (by
-        default a space) and rows are separated by ``delimy`` (by default this
-        will be a newline character).
-        """
-        # Check filename
-        filename = os.path.expanduser(filename)
-        # Save
-        data = self._2d[name]
-        data = data[frame]
-        text = []
-        for row in data:
-            text.append(delimx.join([myokit.float.str(x) for x in row]))
-        text = delimy.join(text)
-        with open(filename, 'w') as f:
-            f.write(text)
-
-    def set0d(self, name, data, copy=True):
-        """
-        Adds or updates a zero-dimensional time series ``data`` for the
-        variable named by the string ``name``.
-
-        The ``data`` must be specified as a sequence of length ``n``, where
-        ``n`` is the first value returned by :meth:`DataBlock2d.shape()`.
-
-        By default, a copy of the given data will be stored. To prevent this
-        and store a reference instead, set ``copy=False``.
-        """
-        name = str(name)
-        if not name:
-            raise ValueError('Name cannot be empty.')
-        data = np.array(data, copy=copy)
-        if data.shape != (self._nt,):
-            raise ValueError(
-                'Data must be sequence of length ' + str(self._nt) + '.')
-        self._0d[name] = data
+        # Ensure the log is valid
+        log.validate()
 
-    def set2d(self, name, data, copy=True):
-        """
-        Adds or updates a two-dimensional time series ``data`` for the variable
-        named by the string ``name``.
+        # Check dict keys
+        keys = set(log.keys())
+        if len(keys) == 0:
+            return log
+
+        for key in keys:
+            # Handle derivatives
+            deriv = key[0:4] == 'dot(' and key[-1:] == ')'
+            if deriv:
+                key = key[4:-1]
 
-        The ``data`` must be specified as a numpy array with shape ``(n, w)``,
-        where ``(n, w)`` is the value returned by :meth:`DataBlock2d.shape()`.
+            # Split of index / name
+            kdims, kname = split_key(key)
 
-        By default, a copy of the given data will be stored. To prevent this
-        and store a reference instead, set ``copy=False``.
-        """
-        name = str(name)
-        if not name:
-            raise ValueError('Name cannot be empty.')
-        data = np.array(data, copy=copy)
-        shape = (self._nt, self._ny, self._nx)
-        if data.shape != shape:
-            raise ValueError('Data must have shape ' + str(shape) + '.')
-        self._2d[name] = data
+            # Test name-key
+            try:
+                var = model.get(kname)
+            except KeyError:
+                raise ValueError(
+                    'Unknown variable <' + str(kname) + '> in log.')
 
-    def shape(self):
-        """
-        Returns the required shape for 2d data passed to this data block. Zero
-        dimensional series passed in must have length ``shape()[0]``.
-        """
-        return (self._nt, self._ny, self._nx)
+            # Check if in class of allowed variables
+            if deriv:
+                if not myokit.LOG_DERIV & allowed_classes:
+                    raise ValueError(
+                        'This log does not support derivatives, got <'
+                        + key + '>.')
+                if not var.is_state():
+                    raise ValueError(
+                        'Cannot log time derivative of non-state <'
+                        + var.qname() + '>.')
+            else:
+                check_if_allowed_class(var)
 
-    def time(self):
-        """
-        Returns the time data for this datablock. The data is returned
-        directly, no copy is made.
-        """
-        return self._time
+            # Check dimensions
+            if kdims:
 
-    def to_log(self, copy=True):
-        """
-        Returns a :class:`myokit.DataLog` containing the same information as
-        this block.
+                # Raise error if global
+                if kname in global_vars:
+                    raise ValueError(
+                        'Cannot specify a cell index for global logging'
+                        ' variable <' + str(kname) + '>.')
 
-        The data will be copied, unless ``copy`` is set to ``False``.
-        """
-        d = myokit.DataLog()
+                # Test dim key
+                if kdims not in dcombos:
+                    raise ValueError(
+                        'Invalid index <' + str(kdims) + '> in log.')
 
-        # Add 0d vectors
-        d.set_time_key('time')
-        d['time'] = np.array(self._time, copy=copy)
-        for k, v in self._0d.items():
-            d[k] = np.array(v, copy=copy)
+            elif dims:
 
-        # Add 2d fields
-        for k, v in self._2d.items():
-            for x in range(self._nx):
-                s = str(x) + '.'
-                for y in range(self._ny):
-                    d[s + str(y) + '.' + k] = np.array(v[:, y, x], copy=copy)
-        return d
+                # Raise error if non-global variable is used in multi-cell log
+                if kname not in global_vars:
+                    raise ValueError(
+                        'DataLog contains non-indexed entry for'
+                        ' cell-specific variable <' + str(kname) + '>.')
 
-    def trace(self, variable, x, y):
-        """
-        Returns a 0d time series of the value ``variable``, corresponding to
-        the cell at position ``x``, ``y``. The data is returned directly, no
-        copy is made.
-        """
-        return self._2d[variable][:, y, x]
+        # Check dict values can be appended to
+        m = 'append'
+        for v in log.values():
+            if not (hasattr(v, m) and callable(getattr(v, m))):
+                raise ValueError(
+                    'Logging dict must map qnames to objects'
+                    ' that support the append() method.')
 
+        # Return
+        return log
 
-class ColorMap:
-    """
-    *Abstract class*
+    #
+    # Fourth option, a sequence of variable names, either global or local.
+    #
+
+    # Check if list interface works
+    # If not, then raise exception
+    try:
+        if len(log) > 0:
+            log[0]
+    except Exception:
+        raise ValueError(
+            'Argument `log` has unexpected type. Expecting None, integer flag,'
+            ' sequence of names, dict or DataLog.')
+
+    if isinstance(log, str):
+        raise ValueError(
+            'String passed in as `log` argument, should be list'
+            ' or other sequence containing strings.')
+
+    # Parse log argument as list
+    lst = log
+    log = myokit.DataLog()
+    checked_knames = set()
+    for key in lst:
+
+        # Allow variable objects and LhsExpressions
+        if isinstance(key, myokit.Variable):
+            key = key.qname()
+        elif isinstance(key, myokit.LhsExpression):
+            key = str(key)
+
+        # Handle derivatives
+        deriv = key[0:4] == 'dot(' and key[-1:] == ')'
+        if deriv:
+            key = key[4:-1]
 
-    Applies colormap transformations to floating point data and returns RGB
-    data.
+        # Split off cell indexes
+        kdims, kname = split_key(key)
 
-    :class:`ColorMaps <ColorMap>` are callable objects and take the following
-    arguments:
+        # Don't re-test multi-dim vars
+        if kname not in checked_knames:
 
-    ``floats``
-        A 1-dimensional numpy array of floating point numbers.
-    ``lower=None``
-        A lower bound for the floats in the input. The ``lower`` and ``upper``
-        values are used to normalize the input before applying the colormap. If
-        this bound is omitted the lowest value in the input data is used.
-    ``upper=None``
-        An upper bound for the floats in the input. The ``lower`` and ``upper``
-        values are used to normalize the input before applying the colormap. If
-        this bound is omitted the highest value in the input data is used.
-    ``alpha=True``
-        Set to ``False`` to omit an alpha channel from the output.
-    ``rgb=None``
-        Set to ``True`` to return bytes in the order ``0xARGB``, to ``False``
-        to return the order ``0xBGRA`` or to ``None`` to let the system's
-        endianness determine the correct order. In the last case, big-endian
-        systems will return ``0xARGB`` while little-endian systems use the
-        order ``0xBGRA``.
-
-    A 1-dimensional array of ``n`` floating point numbers will be converted to
-    a 1-dimensional array of ``4n`` ``uints``, or ``3n`` if the alpha channel
-    is disabled. The array will be ordered sequentially: the first four (or
-    three) bytes describe the first float, the next four (or three) describe
-    the second float and so on.
-    """
-    _colormaps = {}
+            # Test if name key points to valid variable
+            try:
+                var = model.get(kname)
+            except KeyError:
+                raise ValueError(
+                    'Unknown variable <' + str(kname) + '> in list.')
 
-    def __call__(self, floats, lower=None, upper=None, alpha=True, rgb=None):
-        raise NotImplementedError
+            # Check if in class of allowed variables
+            if deriv:
+                if not myokit.LOG_DERIV & allowed_classes:
+                    raise ValueError(
+                        'This log does not support derivatives, got <'
+                        + key + '>.')
 
-    @staticmethod
-    def exists(name):
-        """
-        Returns True if the given name corresponds to a colormap.
-        """
-        return name in ColorMap._colormaps
+                if not var.is_state():
+                    raise ValueError(
+                        'Cannot log time derivative of non-state <'
+                        + var.qname() + '>.')
+            else:
+                check_if_allowed_class(var)
+            checked_knames.add(kname)
 
-    @staticmethod
-    def get(name):
-        """
-        Returns the colormap method indicated by the given name.
-        """
-        try:
-            return ColorMap._colormaps[name]()
-        except KeyError:
-            raise KeyError('Non-existent ColorMap "' + str(name) + '".')
+        # Add key to log
+        if kdims:
 
-    @staticmethod
-    def hsv_to_rgb(h, s, v):
-        """
-        Converts hsv values in the range [0,1] to rgb values in the range
-        [0,255]. Adapted from Matplotlib.
-        """
-        r, g, b = np.empty_like(h), np.empty_like(h), np.empty_like(h)
-        i = (h * 6).astype(int) % 6
-        f = (h * 6) - i
-        p = v * (1 - s)
-        q = v * (1 - s * f)
-        t = v * (1 - s * (1 - f))
-        idx = (i == 0)
-        r[idx], g[idx], b[idx] = v[idx], t[idx], p[idx]
-        idx = (i == 1)
-        r[idx], g[idx], b[idx] = q[idx], v[idx], p[idx]
-        idx = (i == 2)
-        r[idx], g[idx], b[idx] = p[idx], v[idx], t[idx]
-        idx = (i == 3)
-        r[idx], g[idx], b[idx] = p[idx], q[idx], v[idx]
-        idx = (i == 4)
-        r[idx], g[idx], b[idx] = t[idx], p[idx], v[idx]
-        idx = (i == 5)
-        r[idx], g[idx], b[idx] = v[idx], p[idx], q[idx]
-        out = (
-            np.array(r * 255, dtype=np.uint8, copy=False),
-            np.array(g * 255, dtype=np.uint8, copy=False),
-            np.array(b * 255, dtype=np.uint8, copy=False),
-        )
-        return out
+            # Raise error if global
+            if kname in global_vars:
+                raise ValueError(
+                    'Cannot specify a cell index for global logging variable'
+                    ' <' + str(kname) + '>.')
 
-    @staticmethod
-    def image(name, x, y):
-        """
-        Returns image data (such as returned by :meth:`DataBlock2d.images()`)
-        representing the colormap specified by ``name``. The image dimensions
-        can be set using ``x`` and ``y``.
-        """
-        data = np.linspace(1, 0, y)
-        data = np.tile(data, (x, 1)).transpose()
-        data = np.reshape(data, (1, y, x))
-        block = myokit.DataBlock2d(x, y, [0])
-        block.set2d('colormap', data, copy=False)
-        return block.images('colormap', colormap=name)[0]
+            # Test dim key
+            if kdims not in dcombos:
+                raise ValueError(
+                    'Invalid index <' + str(kdims) + '> in list.')
 
-    @staticmethod
-    def names():
-        """
-        Returns an iterator over the names of all available colormaps.
-        """
-        return ColorMap._colormaps.keys()
+            key = kdims + kname if not deriv else 'dot(' + kdims + kname + ')'
+            log[key] = array.array(typecode)
 
-    @staticmethod
-    def normalize(floats, lower, upper):
-        """
-        Normalizes the given float data based on the specified lower and upper
-        bounds.
-        """
-        floats = np.array(floats, copy=True)
-        # Enforce lower and upper bounds
-        floats[floats < lower] = lower
-        floats[floats > upper] = upper
-        # Normalize
-        n = floats - lower
-        r = upper - lower
-        if r == 0:
-            return n
         else:
-            return n / r
 
+            if kname in global_vars:
+                key = kname if not deriv else 'dot(' + kname + ')'
+                log[key] = array.array(typecode)
+            else:
+                for c in dcombos:
+                    key = c + kname if not deriv else 'dot(' + c + kname + ')'
+                    log[key] = array.array(typecode)
 
-class ColorMapBlue(ColorMap):
-    """
-    A nice red colormap.
-    """
-    def __call__(self, floats, lower=None, upper=None, alpha=True, rgb=None):
-        # Normalize floats
-        f = ColorMap.normalize(floats, lower, upper)
-        # Calculate h,s,v and convert to rgb
-        h = np.zeros(f.shape)
-        s = f
-        v = np.ones(f.shape)
-        b, g, r = ColorMap.hsv_to_rgb(h, s, v)
-        # Color order
-        rgb = (sys.byteorder == 'big') if rgb is None else rgb
-        # Offset for first color in (a)rgb or rgb(a)
-        m = 1 if (alpha and rgb) else 0
-        # Number of bytes per float
-        n = 4 if alpha else 3
-        # Create output
-        out = 255 * np.ones(n * len(floats), dtype=np.uint8)
-        out[m + 0::n] = r if rgb else b
-        out[m + 1::n] = g
-        out[m + 2::n] = b if rgb else r
-        return out
+    # Set time variable
+    time = model.time().qname()
+    if time in log:
+        log.set_time_key(time)
 
+    # Return
+    return log
 
-class ColorMapGreen(ColorMap):
-    """
-    A nice green colormap.
+
+def _dimco(*dims):
     """
-    def __call__(self, floats, lower=None, upper=None, alpha=True, rgb=None):
-        # Normalize floats
-        f = ColorMap.normalize(floats, lower, upper)
-        # Calculate h,s,v and convert to rgb
-        h = np.zeros(f.shape)
-        s = f
-        v = np.ones(f.shape)
-        g, r, b = ColorMap.hsv_to_rgb(h, s, v)
-        # Color order
-        rgb = (sys.byteorder == 'big') if rgb is None else rgb
-        # Offset for first color in (a)rgb or rgb(a)
-        m = 1 if (alpha and rgb) else 0
-        # Number of bytes per float
-        n = 4 if alpha else 3
-        # Create output
-        out = 255 * np.ones(n * len(floats), dtype=np.uint8)
-        out[m + 0::n] = r if rgb else b
-        out[m + 1::n] = g
-        out[m + 2::n] = b if rgb else r
-        return out
+    Generates all the combinations of a certain set of integer dimensions. For
+    example given ``dims=(2, 3)`` it returns::
 
+        (0, 0), (1, 0), (0, 1), (1, 1), (0, 2), (1, 2)
 
-class ColorMapRed(ColorMap):
     """
-    A nice red colormap.
+    n = len(dims) - 1
     """
-    def __call__(self, floats, lower=None, upper=None, alpha=True, rgb=None):
-        # Normalize floats
-        f = ColorMap.normalize(floats, lower, upper)
-        # Calculate h,s,v and convert to rgb
-        h = np.zeros(f.shape)
-        s = f
-        v = np.ones(f.shape)
-        r, g, b = ColorMap.hsv_to_rgb(h, s, v)
-        # Color order
-        rgb = (sys.byteorder == 'big') if rgb is None else rgb
-        # Offset for first color in (a)rgb or rgb(a)
-        m = 1 if (alpha and rgb) else 0
-        # Number of bytes per float
-        n = 4 if alpha else 3
-        # Create output
-        out = 255 * np.ones(n * len(floats), dtype=np.uint8)
-        out[m + 0::n] = r if rgb else b
-        out[m + 1::n] = g
-        out[m + 2::n] = b if rgb else r
-        return out
+    def inner(dims, index, prefix):
+        if index == n:
+            for i in range(0,dims[index]):
+                yield prefix + (i,)
+        else:
+            for i in range(0,dims[index]):
+                prefix2 = prefix + (i, )
+                for y in inner(dims, index + 1, prefix2):
+                    yield y
+    return inner(dims, 0, ())
+    """
+    def inner(dims, index, postfix):
+        if index == 0:
+            for i in range(0, dims[index]):
+                yield (i,) + postfix
+        else:
+            for i in range(0, dims[index]):
+                postfix2 = (i, ) + postfix
+                for y in inner(dims, index - 1, postfix2):
+                    yield y
+    return inner(dims, n, ())
 
 
-class ColorMapTraditional(ColorMap):
+def split_key(key):
     """
-    Traditional hue-cycling colormap.
-    """
-    def __call__(self, floats, lower=None, upper=None, alpha=True, rgb=None):
-        # Normalize floats
-        f = ColorMap.normalize(floats, lower, upper)
-        # Calculate h,s,v and convert to rgb
-        g = 0.6
-        s = g + (1 - g) * np.sin(f * 3.14)
-        h = (0.85 - 0.85 * f) % 1
-        r, g, b = ColorMap.hsv_to_rgb(h, s, s)
-        # Color order
-        rgb = (sys.byteorder == 'big') if rgb is None else rgb
-        # Offset for first color in (a)rgb or rgb(a)
-        m = 1 if (alpha and rgb) else 0
-        # Number of bytes per float
-        n = 4 if alpha else 3
-        # Create output
-        out = 255 * np.ones(n * len(floats), dtype=np.uint8)
-        out[m + 0::n] = r if rgb else b
-        out[m + 1::n] = g
-        out[m + 2::n] = b if rgb else r
-        return out
+    Splits a log entry name into a cell index part and a variable name part.
 
+    The cell index will be an empty string for 0d entries or global variables.
+    For higher dimensional cases it will be the cell index in each dimension,
+    followed by a period, for example: ``15.2.``.
 
-ColorMap._colormaps['blue'] = ColorMapBlue
-ColorMap._colormaps['green'] = ColorMapGreen
-ColorMap._colormaps['red'] = ColorMapRed
-ColorMap._colormaps['traditional'] = ColorMapTraditional
+    The two parts returned by split_key may always be concatenated to obtain
+    the original entry.
+    """
+    m = ID_NAME_PATTERN.match(key, 0)
+    if m:
+        return key[:m.end()], key[m.end():]
+    else:
+        return '', key
```

### Comparing `myokit-1.35.0/myokit/_datalog.py` & `myokit-1.35.1/myokit/lib/markov.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1981 +1,1993 @@
 #
-# Functions relating to the DataLog class for storing time series data.
+# Tools for working with Markov models of ion channels.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
-import os
-import re
-import sys
-import array
+import collections
 
 import numpy as np
 
-from collections import OrderedDict
-
 import myokit
 
 
-# Function to split keys into dimension-key,qname-key pairs
-ID_NAME_PATTERN = re.compile(r'(\d+.)+')
+class LinearModel:
+    """
+    Represents a linear Markov model of an ion channel extracted from a
+    :class:`myokit.Model`.
 
-# Readme file for DataLog binary files
-README_SAVE_BIN = """
-Myokit DataLog Binary File
---------------------------
-This zip file contains binary time series data for one or multiple variables.
-The file structure.txt contains structural information about the data in plain
-text. The first line lists the number of fields. The second line gives the
-length of the data arrays. The third line specifies the data type, either
-single ("f") or double ("d") precision. The fourth line indicates which entry
-corresponds to a time variable, or is blank if no time variable was explicitly
-specified. Each following line contains the name of a data field, in the order
-its data occurs in the binary data file "data.bin". All data is stored
-little-endian.
-""".strip()
+    The class assumes the markov model can be written as::
 
-# Encoding used for text portions of zip files
-ENC = 'utf-8'
+        dot(x) = A(V,p) * x
+        I = B(V,p) * x
 
+    where ``V`` is the membrane potential, ``p`` is a set of parameters and
+    ``A`` and ``B`` are the matrices that relate the state ``x`` to its
+    derivative ``dot(x)`` and a current ``I``.
+
+    ``A`` and ``B`` can contain non-linear functions, but should be simple
+    scalar matrices when evaluated for a fixed ``V`` and ``p``. For example,
+    the current equation ``I = g * O * (V - E)`` would have ``p = [g, E]``, so
+    that for fixed ``p`` and ``V`` this would resolve to
+    ``I = (g * (V - E)) * O``, such that ``g * (V - E)`` is a constant that can
+    be included in ``B``.
+
+    The model variables to treat as parameter are specified by the user when
+    the model is created. Any other variables, for example state variables such
+    as intercellular calcium or constants such as temperature, are fixed when
+    the markov model is created and can no longer be changed. Initial values
+    written as expressions are evaluated when the model is made.
+
+    To create a :class:`Markov`, pass in a :class:`myokit.Model` and select a
+    list of states. All other states will be fixed at their current value and
+    an attempt will be made to write the remaining state equations as linear
+    combinations of the states. If this is not possible, a :class:`ValueError`
+    is raised. The membrane potential must be indicated using the label
+    ``membrane_potential`` or by passing it in as ``vm``.
+
+    The current variable is optional, if no current is specified by the user
+    the relation ``I = B * x`` is dropped and no ``B`` is calculated.
+
+    Example::
+
+        import myokit
+        import myokit.lib.markov as markov
+
+        # Load a model from disk
+        model = myokit.load_model('some-model.mmt')
+
+        # Select the relevant states and parameters
+        states = [
+            'ina.C1',
+            'ina.C2',
+            'ina.O',
+            ...
+            ]
+        parameters = [
+            'ina.p1',
+            'ina.p2',
+            ...
+            ]
+        current = 'ina.INa'
+
+        # Extract a markov model
+        mm = markov.LinearModel(model, states, parameters, current)
+
+        # Get the matrices A and B such that dot(x) = A * x and I = B * x
+        # where ``x`` is the state vector and ``I`` is the current.
+        A, B = mm.matrices(membrane_potential=-40)
+        print(A)
+
+    Alternatively, a LinearModel can be constructed from a single component
+    using the method :meth:`from_component() <LinearModel.from_component()>`::
 
-class DataLog(OrderedDict):
-    """
-    A dictionary time-series, for example data logged during a simulation or
-    experiment.
+        import myokit
+        import myokit.lib.markov as markov
 
-    A :class:`DataLog` is expected but not required to contain a single
-    entry indicating time and any number of entries representing a variable
-    varying over time.
+        # Load a model from disk
+        model = myokit.load_model('some-model.mmt')
 
-    Single cell data is accessed simply by the variable name::
+        # Extract a markov model
+        mm = markov.LinearModel.from_component(model.get('ina'))
 
-        v = log['membrane.V']
+    Arguments:
 
-    Multi-cell data is accessed by appending the index of the cell before the
-    variable name. For example::
+    ``model``
+        The model to work with.
+    ``states``
+        An ordered list of state variables (or state variable names) from
+        ``model``. All remaining state variables will be frozen in place. Each
+        state's derivative must be a linear combination of the other states.
+    ``parameters``
+        A list of parameters to maintain in their symbolic form.
+    ``current``
+        The markov model's current variable. The current must be a linear
+        combination of the states (for example ``g * (V - E) * (O1 + O2)``)
+        where ``O1`` and ``O2`` are states. If no current variable is specified
+        ``None`` can be used instead.
+    ``vm``
+        The variable indicating membrane potential. If set to ``None``
+        (default) the method will search for a variable with the label
+        ``membrane_potential``.
 
-        v = log['1.2.membrane.V']
+    """
+    # NOTE: A LinearModel must be immutable!
+    # This ensures that the simulations don't have to clone it (which would be
+    # costly and difficult).
+    # A LinearModel has a method "matrices()" which can evaluate A and B
+    # for its default values or newly passed in values, but it never updates
+    # its internal state in any way!
+    def __init__(self, model, states, parameters=None, current=None, vm=None):
+        super().__init__()
+
+        # Get a clone of the model, with all markov models written in full ODE
+        # form.
+        self._model = convert_markov_models_to_full_ode_form(model)
+        del model
 
-    This returns the membrane potential for cell (1, 2). Another way to obtain
-    the same result is::
+        #
+        # Check input
+        #
 
-        v = log['membrane.V', 1, 2]
+        # Check and collect state variables
+        self._states = []
+        for state in states:
+            if isinstance(state, myokit.Variable):
+                state = state.qname()
+            try:
+                state = self._model.get(str(state), myokit.Variable)
+            except KeyError:
+                raise LinearModelError('Unknown state: <' + str(state) + '>.')
+            if not state.is_state():
+                raise LinearModelError(
+                    'Variable <' + state.qname() + '> is not a state.')
+            if state in self._states:
+                raise LinearModelError(
+                    'State <' + state.qname() + '> was added twice.')
+            self._states.append(state)
+        del states
+
+        # Check and collect parameter variables
+        unique = set()
+        self._parameters = []
+        if parameters is None:
+            parameters = []
+        for parameter in parameters:
+            if isinstance(parameter, myokit.Variable):
+                parameter = parameter.qname()
+            try:
+                parameter = self._model.get(parameter, myokit.Variable)
+            except KeyError:
+                raise LinearModelError(
+                    'Unknown parameter: <' + str(parameter) + '>.')
+            if not parameter.is_literal():
+                raise LinearModelError(
+                    'Unsuitable parameter: <' + str(parameter) + '>.')
+            if parameter in unique:
+                raise LinearModelError(
+                    'Parameter listed twice: <' + str(parameter) + '>.')
+            unique.add(parameter)
+            self._parameters.append(parameter)
+        del unique
+        del parameters
+
+        # Check current variable
+        if current is not None:
+            if isinstance(current, myokit.Variable):
+                current = current.qname()
+            current = self._model.get(current, myokit.Variable)
+            if current.is_state():
+                raise LinearModelError('Current variable can not be a state.')
+        self._current = current
+        del current
+
+        # Check membrane potential variable
+        if vm is None:
+            vm = self._model.label('membrane_potential')
+        if vm is None:
+            raise LinearModelError(
+                'A membrane potential must be specified as `vm` or using the'
+                ' label `membrane_potential`.')
+        if isinstance(vm, myokit.Variable):
+            vm = vm.qname()
+        self._membrane_potential = self._model.get(vm)
+        if self._membrane_potential in self._parameters:
+            raise LinearModelError(
+                'Membrane potential should not be included in the list of'
+                ' parameters.')
+        if self._membrane_potential in self._states:
+            raise LinearModelError(
+                'The membrane potential should not be included in the list of'
+                ' states.')
+        if self._membrane_potential == self._current:
+            raise LinearModelError(
+                'The membrane potential should not be the current variable.')
+        del vm
+
+        # Get values of all states
+        # Note: Do this _before_ changing the model!
+        s = self._model.initial_values(True)
+        self._default_state = np.array(
+            [v.initial_value(True) for v in self._states])
 
-    or, finally::
+        #
+        # Demote unnecessary states, remove bindings and validate model.
+        #
 
-        v = log['membrane.V', (1, 2)]
+        # Freeze remaining, non-markov-model states
+        for k, state in enumerate(self._model.states()):
+            if state not in self._states:
+                state.demote()
+                state.set_rhs(s[k])
+        del s
+
+        # Unbind everything except time
+        for label, var in self._model.bindings():
+            if label != 'time':
+                var.set_binding(None)
+
+        # Check if current variable depends on selected states
+        # (At this point, anything not dependent on the states is a constant)
+        if self._current is not None and self._current.is_constant():
+            raise LinearModelError(
+                'Current must be a function of the markov model\'s state'
+                ' variables.')
 
-    Every array stored in the log must have the same length. This condition can
-    be checked by calling the method :meth:`validate`.
+        # Validate modified model
+        self._model.validate()
 
-    A new ``DataLog`` can be created in a number of ways::
+        #
+        # Create functions:
+        #   matrix_function(vm, p1, p2, ...   ) --> A, B
+        #       where dot(x) = Ax and I = Bx
+        #   rate_list_function(vm, p1, p2, ...) --> R
+        #       where R contains tuples (i, j, rij)
+        #
 
-        # Create an empty DataLog:
-        d = myokit.DataLog()
-        d['time'] = [1, 2, 3]
-        d['data'] = [2, 4, 5]
-        d.set_time_key('time')
+        # Create a list of inputs to the functions
+        self._inputs = self._parameters + [self._membrane_potential]
 
-        # Create a clone of d
-        e = myokit.DataLog(d)
+        # Get the default values for all inputs
+        self._default_inputs = np.array([v.eval() for v in self._inputs])
 
-        # Create a DataLog based on a dictionary
-        d = myokit.DataLog({'time':[1, 2, 3], 'data':[2, 4, 5]}, time='time')
+        # Create functions
+        self._matrix_function = None
+        self._rate_list_function = None
+        self._generate_functions()
 
-    Arguments:
+        #
+        # Partial validation
+        #
+        # Check if dependencies are bidirectional
+        for s in self._states:
+            for d in s.refs_to(state_refs=True):
+                if s not in d.refs_to(state_refs=True):
+                    raise LinearModelError(
+                        'State <' + s.qname() + '> depends on <' + d.qname()
+                        + '> but not vice versa.')
+
+        # Check the sum of all states is 1
+        tolerance = 1e-8
+        x = np.sum(self._default_state)
+        if np.abs(x - 1) > tolerance:
+            raise LinearModelError(
+                'The sum of states is not equal to 1: ' + str(x))
+
+        # Check the sum of all derivatives per column
+        A, B = self.matrices()
+        for k, x in enumerate(np.sum(A, axis=0)):
+            if abs(x) > tolerance:
+                raise LinearModelError(
+                    'Derivatives in column ' + str(1 + k) + ' sum to non-zero'
+                    ' value: ' + str(x) + '.')
+
+    def _generate_functions(self):
+        """
+        Creates a function that takes parameters as input and returns matrices
+        A and B.
+
+        (This method is called only once, by the constructor, but it's
+        complicated enough to warrant its own method...)
+        """
+        # Create mapping from states to index
+        state_indices = {}
+        for k, state in enumerate(self._states):
+            state_indices[state] = k
+
+        # Get expressions for state & current variables, but with all
+        # references to variables (except states and parameters) replaced by
+        # inlined expressions.
+        expressions = []
+        for v in self._states:
+            expressions.append(v.rhs().clone(expand=True, retain=self._inputs))
+        if self._current is not None:
+            current_expression = self._current.rhs().clone(
+                expand=True, retain=self._inputs)
+
+        # Create parametrisable matrices to evaluate the state & current
+        # This checks that each state's RHS can be written as a linear
+        # combination of the states, and gathers the corresponding multipliers.
+
+        # Matrix of linear factors
+        n = len(self._states)
+        A = [[myokit.Number(0) for j in range(n)] for i in range(n)]
 
-    ``other``
-        A DataLog to clone or a dictionary to use as basis.
-    ``time``
-        The log key to use for the time variable. When cloning a log, adding
-        the ``time`` argument will overwrite the cloned value.
+        # List of transitions
+        T = set()
 
-    """
+        # Populate A and T
+        for row, e in enumerate(expressions):
 
-    def __init__(self, other=None, time=None):
-        if other is None:
-            # Create new
-            super().__init__()
-            self._time = None
-        else:
-            # Clone
-            super().__init__(other)
+            # Check if this expression is a linear combination of the states
+            try:
+                factors = _linear_combination(e, self._states)
+            except ValueError:
+                raise LinearModelError(
+                    'Unable to write expression as linear combination of'
+                    ' states: ' + str(e) + '.')
+
+            # Scan factors
+            for col, state in enumerate(self._states):
+                factor = factors[col]
+                if factor is not None:
+                    # Add factor to transition matrix
+                    A[row][col] = factor
+
+                    # Store transition in transition list
+                    if row != col:
+                        T.add((col, row))   # A is mirrored
+
+        # Create a parametrisable matrix for the current
+        B = [myokit.Number(0) for i in range(n)]
+        if self._current is not None:
             try:
-                self._time = str(other._time)
-            except Exception:
-                self._time = None
-        if time is not None:
-            self.set_time_key(time)
+                factors = _linear_combination(current_expression, self._states)
+            except ValueError:
+                raise LinearModelError(
+                    'Unable to write expression as linear combination of'
+                    ' states: ' + str(e) + '.')
+
+            for col, state in enumerate(self._states):
+                factor = factors[col]
+                if factor is not None:
+                    B[col] = factor
+
+        # Create list of transition rates and associated equations
+        T = list(T)
+        T.sort()
+        R = []
+        for i in range(len(A)):
+            for j in range(len(A)):
+                if (i, j) in T:
+                    R.append((i, j, A[j][i]))   # A is mirrored
+        del T
 
-    def apd(self, v='membrane.V', threshold=-70):
+        #
+        # Create function to create parametrisable matrices
+        #
+        self._model.reserve_unique_names('A', 'B', 'n', 'numpy')
+        writer = myokit.numpy_writer()
+        w = writer.ex
+        head = 'def matrix_function('
+        head += ','.join([w(p.lhs()) for p in self._inputs])
+        head += '):'
+        body = []
+        body.append('A = numpy.zeros((n, n))')
+        zero = myokit.Number(0)
+        for i, row in enumerate(A):
+            for j, e in enumerate(row):
+                if e != zero:
+                    body.append('A[' + str(i) + ',' + str(j) + '] = ' + w(e))
+        body.append('B = numpy.zeros(n)')
+        for j, e in enumerate(B):
+            if e != zero:
+                body.append('B[' + str(j) + '] = ' + w(e))
+        body.append('return A, B')
+        code = head + '\n' + '\n'.join(['    ' + line for line in body])
+        globl = {'numpy': np, 'n': n}
+        local = {}
+
+        exec(code, globl, local)
+        self._matrix_function = local['matrix_function']
+
+        #
+        # Create function to return list of transition rates
+        #
+        self._model.reserve_unique_names('R', 'n', 'numpy')
+        head = 'def rate_list_function('
+        head += ','.join([w(p.lhs()) for p in self._inputs])
+        head += '):'
+        body = []
+        body.append('R = []')
+        for i, j, e in R:
+            body.append(
+                'R.append((' + str(i) + ',' + str(j) + ',' + w(e) + '))')
+        body.append('return R')
+        code = head + '\n' + '\n'.join(['    ' + line for line in body])
+        globl = {'numpy': np}
+        local = {}
+        exec(code, globl, local)
+        self._rate_list_function = local['rate_list_function']
+
+    def current(self):
+        """
+        Returns the name of the current variable used by this model, or None if
+        no current variable was specified.
         """
-        Calculates one or more Action Potential Durations (APDs) in a single
-        cell's membrane potential.
+        return self._current
 
-        *Note 1: More accuracte APD measurements can be obtained using the*
-        :class:`Simulation` *object's APD tracking functionality. See*
-        :meth:`Simulation.run()` *for details.*
+    def default_membrane_potential(self):
+        """
+        Returns this markov model's default membrane potential value.
+        """
+        return self._default_inputs[-1]
 
-        *Note 2: This APD is defined by simply checking crossing of a threshold
-        potential, and does not look at lowest or highest voltages in a
-        signal.*
+    def default_parameters(self):
+        """
+        Returns this markov model's default parameter values
+        """
+        return list(self._default_inputs[:-1])
 
-        The membrane potential data should be listed in the log under the key
-        given by ``v``.
+    def default_state(self):
+        """
+        Returns this markov model's default state values.
+        """
+        return list(self._default_state)
 
-        The returned value is a list of tuples (AP_start, APD).
+    @staticmethod
+    def from_component(
+            component, states=None, parameters=None, current=None, vm=None):
         """
-        def crossings(x, y, t):
-            """
-            Calculates the ``x``-values where ``y`` crosses threshold ``t``.
-            Returns a list of tuples ``(xc, sc)`` where ``xc`` is the ``x``
-            coordinate of the crossing and ``sc`` is the slope at this point.
-            """
-            x = np.asarray(x)
-            y = np.asarray(y)
+        Creates a Markov model from a component, using the following rules:
 
-            # Get array of places where v exceeds the threshold (1s and 0s)
-            h = (y > t) * 1
+          1. Every state in the component is a state in the Markov model
+          2. Every unnested constant in the component is a parameter
+          3. The component should contain exactly one unnested intermediary
+             variable whose value depends on the model states, this will be
+             used as the current variable.
+          4. The model contains a variable labeled "membrane_potential".
 
-            # Get array of indices just before a crossing
-            c = np.argwhere(h[1:] - h[:-1])
+        Any of the automatically set variables can be overridden using the
+        keyword arguments ``states``, ``parameters``, ``current`` and ``vm``.
 
-            # Gather crossing times
-            crossings = []
-            for i in c:
-                i = i[0]
-                sc = (y[i + 1] - y[i]) / (x[i + 1] - x[i])
-                if y[i] == t:
-                    xc = x[i]
-                else:
-                    xc = x[i] + (t - y[i]) / sc
-                crossings.append((xc, sc))
-            return crossings
+        The parameters, if determined automatically, will be specified in
+        alphabetical order (using a natural sort).
+        """
+        model = component.model()
 
-        # Check time variable
-        t = np.asarray(self.time())
+        # Get or check states
+        if states is None:
 
-        # Check voltage variable
-        v = np.asarray(self[v])
+            # Get state variables
+            states = [x for x in component.variables(state=True)]
 
-        # Check threshold
-        threshold = float(threshold)
+            # Sort by state index
+            states.sort(key=lambda x: x.index())
 
-        # Initial status: check if already in AP
-        apds = myokit.DataLog()
-        apds['start'] = []
-        apds['duration'] = []
-        last = t[0]
+        else:
 
-        # Evaluate crossings
-        for time, slope in crossings(t, v, threshold):
-            if slope < 0:
-                # End of AP
-                if last != t[0]:    # Don't inlcude AP started before t[0]
-                    apds['start'].append(last)
-                    apds['duration'].append(time - last)
-            last = time
-        return apds
+            # Make sure states are variables. This is required to automatically
+            # find a current variable.
+            states_in = states
+            states = []
+            for state in states_in:
+                if isinstance(state, myokit.Variable):
+                    state = state.qname()
+                states.append(model.get(state))
+
+        # Get parameters
+        if parameters is None:
+
+            # Get parameters
+            parameters = [
+                x for x in component.variables(const=True) if x.is_literal()]
+            # Sort by qname, using natural sort
+            parameters.sort(
+                key=lambda x: myokit.tools.natural_sort_key(x.qname()))
+
+        # Get current
+        if current is None:
+            currents = []
+            for x in component.variables(inter=True):
+                for y in x.refs_to(state_refs=True):
+                    if y in states:
+                        # Found a candidate!
+                        currents.append(x)
+                        break
+            if len(currents) > 1:
+                raise LinearModelError(
+                    'The given component has more than one variable that could'
+                    ' be a current: '
+                    + ', '.join(['<' + x.qname() + '>' for x in currents])
+                    + '.')
+            try:
+                current = currents[0]
+            except IndexError:
+                pass
+
+        # Get membrane potential
+        if vm is None:
+            vm = model.label('membrane_potential')
+            if vm is None:
+                raise LinearModelError(
+                    'The model must define a variable labeled as'
+                    ' "membrane_potential".')
+
+        # Create and return LinearModel
+        return LinearModel(model, states, parameters, current, vm)
+
+    def matrices(self, membrane_potential=None, parameters=None):
+        """
+        For a given value of the ``membrane_potential`` and a list of values
+        for the ``parameters``, this method calculates and returns the matrices
+        ``A`` and ``B`` such that::
+
+            dot(x) = A * x
+            I = B * x
+
+        where ``x`` is the state vector and ``I`` is the current.
+
+        Arguments:
+
+        ``membrane_potential``
+            The value to use for the membrane potential, or ``None`` to use the
+            value from the original :class:`myokit.Model`.
+        ``parameters``
+            The values to use for the parameters, given in the order they were
+            originally specified in (if the model was created using
+            :meth:`from_component()`, this will be alphabetical order).
 
-    def block1d(self):
-        """
-        Returns a copy of this log as a :class:`DataBlock1d`.
         """
-        return myokit.DataBlock1d.from_log(self)
+        inputs = list(self._default_inputs)
+        if membrane_potential is not None:
+            inputs[-1] = float(membrane_potential)
+        if parameters is not None:
+            if len(parameters) != len(self._parameters):
+                raise ValueError(
+                    'Illegal parameter vector size: '
+                    + str(len(self._parameters)) + ' required, '
+                    + str(len(parameters)) + ' provided.')
+            inputs[:-1] = [float(x) for x in parameters]
+        return self._matrix_function(*inputs)
 
-    def block2d(self):
+    def membrane_potential(self):
         """
-        Returns a copy of this log as a :class:`DataBlock2d`.
+        Returns the name of the membrane potential variable used by this model.
         """
-        return myokit.DataBlock2d.from_log(self)
+        return self._membrane_potential.qname()
 
-    def clone(self, numpy=False):
+    def parameters(self):
         """
-        Returns a deep clone of this log.
-
-        All lists in the log will be duplicated, but the list contents are
-        assumed to be numerical (and thereby immutable) and won't be cloned.
+        Returns the names of the parameter variables used by this model.
+        """
+        return [v.qname() for v in self._parameters]
 
-        A log with numpy arrays instead of lists can be created by setting
-        ``numpy=True``.
+    def rates(self, membrane_potential=None, parameters=None):
         """
-        log = DataLog()
-        log._time = self._time
-        if numpy:
-            for k, v in self.items():
-                log[str(k)] = np.array(v, copy=True, dtype=float)
-        else:
-            for k, v in self.items():
-                log[str(k)] = list(v)
-        return log
+        For a given value of the ``membrane_potential`` and a list of values
+        for the ``parameters``, this method calculates and returns an ordered
+        list of tuples ``(i, j, rij)`` such that ``rij`` is a non-zero
+        transition rate from the ``i``-th state to the ``j``-th state.
 
-    def __contains__(self, key):
-        return super().__contains__(self._parse_key(key))
+        Arguments:
 
-    def __delitem__(self, key):
-        return super().__delitem__(self._parse_key(key))
+        ``membrane_potential``
+            The value to use for the membrane potential, or ``None`` to use the
+            value from the original :class:`myokit.Model`.
+        ``parameters``
+            The values to use for the parameters, given in the order they were
+            originally specified in (if the model was created using
+            :meth:`from_component()`, this will be alphabetical order).
 
-    def extend(self, other):
         """
-        Returns a copy of this log, extended with the data of another.
+        inputs = list(self._default_inputs)
+        if membrane_potential is not None:
+            inputs[-1] = float(membrane_potential)
+        if parameters is not None:
+            if len(parameters) != len(self._parameters):
+                raise ValueError(
+                    'Illegal parameter vector size: '
+                    + str(len(self._parameters)) + ' required, '
+                    + str(len(parameters)) + ' provided.')
+            inputs[:-1] = [float(x) for x in parameters]
+        return self._rate_list_function(*inputs)
 
-        Both logs must have the same keys and the same time key. The added data
-        must be from later time points than in the log being extended.
+    def states(self):
         """
-        if other._time != self._time:
-            raise ValueError('Both logs must have the same time key.')
-        if other[self._time][0] < self[self._time][-1]:
-            raise ValueError(
-                'Cannot extend DataLog with data from an earlier time.')
-        if set(self.keys()) != set(other.keys()):
-            raise ValueError('Both logs must have the same keys.')
-
-        # Create new log
-        log = DataLog()
-        log._time = self._time
-
-        # Add data
-        for k, v1 in self.items():
-            v2 = other[k]
-            if isinstance(v1, np.ndarray) or isinstance(v2, np.ndarray):
-                # Concatenation copies data
-                log[k] = np.concatenate((np.asarray(v1), np.asarray(v2)))
-            else:
-                log[k] = list(v1)   # Copies v1 data
-                log[k].extend(v2)   # Copies v2 data
-
-        # Return
-        return log
-
-    def find(self, time):
+        Returns the names of the state variables used by this model.
         """
-        Deprecated alias of :meth:`find_after()`.
+        return [v.qname() for v in self._states]
+
+    def steady_state(self, membrane_potential=None, parameters=None):
         """
-        # Deprecated since 2019-08-16
-        import warnings
-        warnings.warn(
-            'The method `find` is deprecated. Please use `find_after`'
-            ' instead.')
+        Analytically determines a steady state solution for this Markov model.
 
-        return self.find_after(time)
+        ``membrane_potential``
+            The value to use for the membrane potential, or ``None`` to use the
+            value from the original :class:`myokit.Model`.
+        ``parameters``
+            The values to use for the parameters, given in the order they were
+            originally specified in (if the model was created using
+            :meth:`from_component()`, this will be alphabetical order).
 
-    def find_after(self, time):
         """
-        Returns the lowest index ``i`` such that
+        # Calculate Jacobian and derivatives
+        A, _ = self.matrices(membrane_potential, parameters)
 
-            times[i] >= time
+        # Set up reduced system with full rank: dot(x) = Ay + B
+        B = A[:-1, -1:]
+        A = A[:-1, :-1] - B
 
-        where ``times`` are the times stored in this ``DataLog``.
+        # Check eigenvalues
+        if np.max(np.linalg.eigvals(A) >= 0):
+            raise LinearModelError(
+                'System has positive eigenvalues: won\'t converge to steady'
+                ' state!')
 
-        If no such value exists in the log, ``len(time)`` is returned.
-        """
-        times = self[self._time]
+        # Solve system Ax + B = 0 --> Ax = -B
+        x = np.linalg.solve(A, -B)
 
-        # Border cases
-        n = len(times)
-        if n == 0 or time <= times[0]:
-            return 0
-        if time > times[-1]:
-            return n
+        # Recreate full state vector and return
+        x = np.array(x).reshape((len(x),))
+        x = np.concatenate((x, [1 - np.sum(x)]))
+        return x
 
-        # Find t
-        def find(lo, hi):
-            # lo = first index, hi = last index + 1
-            if (lo + 1 == hi):
-                return lo + 1
-            m = int((lo + hi) / 2)
-            if time > times[m]:
-                return find(m, hi)
-            else:
-                return find(lo, m)
 
-        return find(0, n)
+class AnalyticalSimulation:
+    """
+    Analytically evaluates a :class:`LinearModel`'s state over a given set of
+    points in time.
 
-    def fold(self, period, discard_remainder=True):
-        """
-        Creates a copy of the log, split with the given period. Split signals
-        are given indexes so that "current" becomes "0.current", "1.current"
-        "2.current", etc.
-
-        If the logs entries do not divide well by 'period', the remainder will
-        be ignored. This happens commonly due to rounding point errors (in
-        which case the remainder is a single entry). To disable this behavior,
-        set ``discard_remainder=False``.
-        """
-        # Note: Using closed intervals can lead to logs of unequal length, so
-        # it should be disabled here to ensure a valid log
-        logs = self.split_periodic(period, adjust=True, closed_intervals=False)
-        # Discard remainder if present
-        if discard_remainder:
-            if len(logs) > 1:
-                n = logs[0].length()
-                if logs[-1].length() < n:
-                    logs = logs[:-1]
-        # Create new log with folded data
-        out = myokit.DataLog()
-        out._time = self._time
-        out[self._time] = logs[0][self._time]
-        for i, log in enumerate(logs):
-            for k, v in log.items():
-                if k != self._time:
-                    out[k, i] = v
-        return out
-
-    def __getitem__(self, key):
-        return super().__getitem__(self._parse_key(key))
-
-    def has_nan(self):
-        """
-        Returns True if one of the variables in this DataLog has a ``NaN`` as
-        its final logged value.
-        """
-        for k, d in self.items():
-            if len(d) > 0 and np.isnan(d[-1]):
-                return True
-        return False
-
-    def integrate(self, name, *cell):
-        """
-        Integrates a field from this log and returns it::
-
-            # Run a simulation and calculate the total current carried by INa
-            s = myokit.Simulation(m, p)
-            d = s.run(1000)
-            q = d.integrate('ina.INa')
+    Solutions are calculated for the "law of large numbers" case, i.e. without
+    stochastic behavior. The solution algorithm is based on eigenvalue
+    decomposition.
+
+    Each simulation object maintains an internal state consisting of
+
+    * The current simulation time
+    * The current state
+    * The default state
+
+    When a simulation is created, the simulation time is set to zero and both
+    the current and default state are initialized using the ``LinearModel``.
+    After each call to :meth:`run()` the time and current state are updated,
+    so that each successive call to run continues where the previous simulation
+    left off.
+
+    A :class:`protocol <myokit.Protocol>` can be used to set the membrane
+    potential during the simulation, or the membrane potential can be adjusted
+    manually between runs.
+
+    Example::
+
+        import myokit
+        import myokit.lib.markov as markov
+
+        # Create a linear markov model
+        m = myokit.load_model('clancy-1999.mmt')
+        m = markov.LinearModel.from_component(m.get('ina'))
+
+        # Create an analytical simulation object
+        s = markov.AnalyticalSimulation(m)
+
+        # Run a simulation
+        s.set_membrane_potential(-30)
+        d = s.run(10)
+
+        # Show the results
+        import matplotlib.pyplot as plt
+        plt.figure()
+        plt.subplot(211)
+        for state in m.states():
+            plt.plot(d.time(), d[state], label=state)
+        plt.legend(loc='center right')
+        plt.subplot(212)
+        plt.plot(d.time(), d[m.current()])
+        plt.show()
 
-        Arguments:
+    """
+    def __init__(self, model, protocol=None):
+        super().__init__()
+        # Check model
+        if not isinstance(model, LinearModel):
+            raise ValueError('First parameter must be a `LinearModel`.')
+        self._model = model
+
+        # Check protocol
+        if protocol is None:
+            self._protocol = None
+        elif not isinstance(protocol, myokit.Protocol):
+            raise ValueError('Protocol must be a myokit.Protocol object')
+        else:
+            self._protocol = protocol.clone()
 
-        ``name``
-            The name of the variable to return, for example 'ik1.IK1' or
-            '2.1.membrane.V'.
-        ``*cell``
-            An optional cell index, for easy access to multi-cellular data, for
-            example ``log.integrate('membrane.V', 2, 1)``.
-
-        """
-        # Get data to integrate
-        key = [str(x) for x in cell]
-        key.append(str(name))
-        key = '.'.join(key)
-        data = np.array(self[key], copy=True)
-        time = np.asarray(self.time())
-
-        # Integration using the midpoint Riemann sum:
-        #  At point i=0, the value is 0
-        #  At each point i>0, the value increases by step[i, i-1]*mean[i, i-1]
-        #data[1:] = 0.5 * (data[1:] + data[:-1]) * (time[1:] - time[:-1])
-        #data[0]  = 0
-
-        # For discontinuities (esp. with CVODES), it makes more sense to treat
-        # the signal as a zero-order hold, IE use the left-point integration
-        # rule:
-        data[1:] = data[:-1] * (time[1:] - time[:-1])
-        data[0] = 0
-        return data.cumsum()
-
-    def interpolate_at(self, name, time):
-        """
-        Returns the value for variable ``name`` at a given ``time``, determined
-        using linear interpolation between the nearest matching times.
-        """
-        t = self[self._time]
-        v = self[name]
+        # Time variable
+        self._time = 0
 
-        # Don't extrapolate
-        if time < t[0] or time > t[-1]:
-            raise ValueError(
-                'Requested time is outside of logged range, would require'
-                ' extrapolation.')
+        # Check if we have a current variable
+        self._has_current = self._model.current() is not None
 
-        # Get first time *after or at* requested time
-        i1 = self.find_after(time)
+        # Set state
+        self._state = np.array(
+            self._model.default_state(), copy=True, dtype=float)
 
-        # Return directly, if possible
-        if t[i1] == time:
-            return v[i1]
-
-        # Interpolate
-        i0 = i1 - 1
-        return v[i0] + (time - t[i0]) * (v[i1] - v[i0]) / (t[i1] - t[i0])
-
-    def isplit(self, i):
-        """
-        Returns two logs, where the first contains all this log's entries up to
-        index ``i``, and the second contains all entries starting from ``i``
-        and higher.
-        """
-        log1 = DataLog()
-        log2 = DataLog()
-        log1._time = self._time
-        log2._time = self._time
-        for k, v in self.items():
-            if isinstance(v, np.ndarray):
-                log1[k] = np.array(v[:i], copy=True, dtype=float)
-                log2[k] = np.array(v[i:], copy=True, dtype=float)
-            else:
-                log1[k] = v[:i]
-                log2[k] = v[i:]
-        return log1, log2
-
-    def itrim(self, a, b):
-        """
-        Returns a copy of this log, with all entries trimmed to the region
-        between indices ``a`` and ``b`` (similar to performing ``x = x[a:b]``
-        on a list).
-        """
-        log = DataLog()
-        log._time = self._time
-        for k, v in self.items():
-            if isinstance(v, np.ndarray):
-                log[k] = np.array(v[a:b], copy=True, dtype=float)
-            else:
-                log[k] = v[a:b]
-        return log
+        # Set default state
+        self._default_state = np.array(self._state, copy=True)
+
+        # Get membrane potential
+        self._membrane_potential = self._model.default_membrane_potential()
+
+        # Get parameters
+        self._parameters = np.array(
+            self._model.default_parameters(), copy=True, dtype=float)
 
-    def itrim_left(self, i):
+        # Mapping from parameter names to index in parameter array
+        self._parameter_map = {}
+        for i, p in enumerate(self._model.parameters()):
+            self._parameter_map[p] = i
+
+        # Cached matrices and partial solution (eigenvalue decomposition etc.)
+        # Both stored per voltage, but will become invalidated if parameters
+        # change
+        self._cached_matrices = {}
+        self._cached_solution = {}
+
+        # If protocol was given, create pacing system, update vm
+        self._pacing = None
+        if self._protocol:
+            self._pacing = myokit.PacingSystem(self._protocol)
+            self._membrane_potential = self._pacing.advance(self._time)
+
+        # Keys for logging
+        self._time_key = self._model._model.time().qname()
+        self._vm_key = self._model._membrane_potential
+        self._log_keys = [self._time_key, self._vm_key] + self._model.states()
+        if self._has_current:
+            self._log_keys.append(self._model.current())
+
+    def current(self, state):
         """
-        Returns a copy of this log, with all entries before index ``i``
-        removed (similar to performing ``x = x[i:]`` on a list).
+        Calculates the current for a given state.
         """
-        log = DataLog()
-        log._time = self._time
-        for k, v in self.items():
-            if isinstance(v, np.ndarray):
-                log[k] = np.array(v[i:], copy=True, dtype=float)
-            else:
-                log[k] = v[i:]
-        return log
+        if not self._has_current:
+            raise Exception(
+                'The used model did not specify a current variable.')
+        A, B = self._matrices()
+        return B.dot(state)
 
-    def itrim_right(self, i):
+    def default_state(self):
         """
-        Returns a copy of this log, with all entries starting from index ``i``
-        removed (similar to performing ``x = x[:i]`` on a list).
+        Returns the default state used by this simulation.
         """
-        log = DataLog()
-        log._time = self._time
-        for k, v in self.items():
-            if isinstance(v, np.ndarray):
-                log[k] = np.array(v[:i], copy=True, dtype=float)
-            else:
-                log[k] = v[:i]
-        return log
+        return list(self._default_state)
 
-    def keys_like(self, query):
+    def _matrices(self):
         """
-        Returns all keys that match the pattern ``*.query``, sorted
-        alphabetically.
+        Returns the (cached or re-generated) matrices.
 
-        For example, ``log.keys_like('membrane.V')`` could return a list
-        ``['0.membrane.V', '1.membrane.V', '2.membrane,V', ...]``, or
-        ``['0.0.membrane.V', '0.1.membrane.V', '1.0.membrane,V', ...]``.
+        Returns ``(A, B)`` if this simulation's model has a current variable,
+        or just ``B`` if it doesn't.
         """
-        keys = [x for x in self.keys() if x.endswith('.' + str(query))]
-        keys.sort()
-        return keys
+        try:
+            return self._cached_matrices[self._membrane_potential]
+        except KeyError:
+            matrices = self._model.matrices(
+                self._membrane_potential, self._parameters)
+            self._cached_matrices[self._membrane_potential] = matrices
+            return matrices
 
-    def length(self):
+    def membrane_potential(self):
         """
-        Returns the length of the entries in this log. If the log is empty,
-        zero is returned.
+        Returns the currently set membrane potential.
         """
-        if len(self) == 0:
-            return 0
-        return len(next(iter(self.values())))
+        return self._membrane_potential
 
-    @staticmethod
-    def load(filename, progress=None, msg='Loading DataLog'):
+    def parameters(self):
         """
-        Loads a :class:`DataLog` from the binary format used by myokit.
-
-        The values in the log will be stored in an :class:`array.array`. The
-        data type used by the array will be the one specified in the binary
-        file. Notice that an `array.array` storing single precision floats will
-        make conversions to ``Float`` objects when items are accessed.
-
-        To obtain feedback on the simulation progress, an object implementing
-        the :class:`myokit.ProgressReporter` interface can be passed in.
-        passed in as ``progress``. An optional description of the current
-        simulation to use in the ProgressReporter can be passed in as `msg`.
+        Returns the currently set parameter values.
         """
-        # Check filename
-        filename = os.path.expanduser(filename)
-
-        # Load compression modules
-        import zipfile
-        try:
-            # Ensure zlib is available
-            import zlib
-            del zlib
-        except ImportError:
-            raise Exception(
-                'This method requires the ``zlib`` module to be installed.')
+        return list(self._parameters)
 
-        # Get size of single and double types on this machine
-        dsize = {
-            'd': len(array.array('d', [1]).tobytes()),
-            'f': len(array.array('f', [1]).tobytes()),
-        }
+    def pre(self, duration):
+        """
+        Performs an unlogged simulation for ``duration`` time units and uses
+        the final state as the new default state.
 
-        # Read data
-        try:
-            f = None
-            f = zipfile.ZipFile(filename, 'r')
-            # Get ZipInfo objects
-            try:
-                body = f.getinfo('data.bin')
-            except KeyError:
-                raise myokit.DataLogReadError('Invalid log file format.')
-            try:
-                head = f.getinfo('structure.txt')
-            except KeyError:
-                raise myokit.DataLogReadError('Invalid log file format.')
-            # Read file contents
-            head = f.read(head).decode(ENC)
-            body = f.read(body)
-        except zipfile.BadZipfile:
-            raise myokit.DataLogReadError('Unable to read log: bad zip file.')
-        except zipfile.LargeZipFile:    # pragma: no cover
-            raise myokit.DataLogReadError(
-                'Unable to read log: zip file requires zip64 support and this'
-                ' has not been enabled on this system.')
-        finally:
-            if f:
-                f.close()
-
-        # Create empty log
-        log = DataLog()
-
-        # Parse header
-        # Number of fields, length of data arrays, data type, time, fields
-        head = iter(head.splitlines())
-        n = int(next(head))
-        data_size = int(next(head))
-        data_type = next(head)
-        time = next(head)
-        if time:
-            # Note, this field doesn't have to be present in the log!
-            log._time = time
-        fields = [x for x in head]
-        if len(fields) != n:
-            raise myokit.DataLogReadError(
-                'Invalid number of fields specified.')
-
-        # Get size of each entry on disk
-        if data_size < 0:
-            raise myokit.DataLogReadError(
-                'Invalid data size: ' + str(data_size) + '.')
-        try:
-            data_size *= dsize[data_type]
-        except KeyError:
-            raise myokit.DataLogReadError(
-                'Invalid data type: "' + data_type + '".')
+        After the simulation:
 
-        # Parse read data
-        fraction = 1.0 / len(fields)
-        start, end = 0, 0
-        nbody = len(body)
-        try:
-            if progress:
-                progress.enter(msg)
-            for k, field in enumerate(fields):
-                if progress and not progress.update(k * fraction):
-                    return
-
-                # Get new data position
-                start = end
-                end += data_size
-                if end > nbody:
-                    raise myokit.DataLogReadError(
-                        'Header indicates larger data size than found in body.'
-                    )
-
-                # Read data
-                ar = array.array(data_type)
-                ar.frombytes(body[start:end])
-                if sys.byteorder == 'big':  # pragma: no cover
-                    ar.byteswap()
-                log[field] = ar
-        finally:
-            if progress:
-                progress.exit()
-        return log
+        - The simulation time is **not** affected
+        - The current state and the default state are updated to the final
+          state reached in the simulation.
 
-    @staticmethod
-    def load_csv(filename, precision=myokit.DOUBLE_PRECISION):
+        Calls to :meth:`reset` after using :meth:`pre` will set the current
+        state to this new default state.
         """
-        Loads a CSV file from disk and returns it as a :class:`DataLog`.
+        # Check arguments
+        duration = float(duration)
+        if duration < 0:
+            raise ValueError('Duration must be non-negative.')
 
-        The CSV file must start with a header line indicating the variable
-        names, separated by commas. Each subsequent row should contain the
-        values at a single point in time for all logged variables.
+        # Run
+        # This isn't much faster, but this way the simulation's interface is
+        # similar to the standard simulation one.
+        old_time = self._time
+        self.run(duration, log_interval=2 * duration)
 
-        The ``DataLog`` is created using the data type specified by the
-        argument ``precision``, regardless of the data type of the stored data.
+        # Update default state
+        self._default_state = np.array(self._state, copy=True)
 
-        The log attempts to set a time variable by searching for a strictly
-        increasing variable. In the case of a tie the first strictly increasing
-        variable is used. This means logs stored with :meth:`save_csv` can
-        safely be read.
+        # Reset time, reset protocol
+        self._time = old_time
+        if self._protocol:
+            self._pacing = myokit.PacingSystem(self._protocol)
+            self._membrane_potential = self._pacing.advance(self._time)
+
+    def reset(self):
         """
-        log = DataLog()
-        # Check filename
-        filename = os.path.expanduser(filename)
+        Resets the simulation:
+
+        - The time variable is set to zero.
+        - The state is set to the default state.
 
-        # Typecode dependent on precision
-        typecode = 'd' if precision == myokit.DOUBLE_PRECISION else 'f'
+        """
+        self._time = 0
+        self._state = np.array(self._default_state, copy=True)
+        if self._protocol:
+            self._pacing = myokit.PacingSystem(self._protocol)
+            self._membrane_potential = self._pacing.advance(self._time)
 
-        # Error raising function
-        def e(line, char, msg):
-            raise myokit.DataLogReadError(
-                'Syntax error on line ' + str(line) + ', character '
-                + str(1 + char) + ': ' + msg)
+    def run(self, duration, log=None, log_interval=0.01, log_times=None):
+        """
+        Runs a simulation for ``duration`` time units.
 
-        quote = '"'
-        delim = ','
-        with open(filename, 'r', newline=None) as f:
-            # Read header
-            keys = []   # The log keys, in order of appearance
+        After the simulation:
 
-            # Read first line
-            line = f.readline()
+        - The simulation time will be increased by ``duration`` time units.
+        - The simulation state will be updated to the last reached state.
 
-            # Ignore comments
-            while line.lstrip()[:1] == '#':
-                line = f.readline()
+        Arguments:
 
-            # Stop on EOF (indicated by blank line without line ending)
-            if line == '':
-                return log
+        ``duration``
+            The number of time units to simulate.
+        ``log``
+            A log from a previous run can be passed in, in which case the
+            results will be appended to this one.
+        ``log_interval``
+            The time between logged points.
+        ``log_times``
+            A pre-defined sequence of times to log at. If set, ``log_interval``
+            will be ignored.
+
+        Returns a :class:`myokit.DataLog` with the simulation results.
+        """
+        # Check arguments
+        duration = float(duration)
+        if duration < 0:
+            raise ValueError('Duration must be non-negative.')
+        log_interval = float(log_interval)
+        if log_interval <= 0:
+            raise ValueError('Log interval must be greater than zero.')
+
+        # Check log_times
+        if log_times is None:
+            log_times = self._time + np.arange(0, duration, log_interval)
+
+        # Set up logging
+        if log is None:
+
+            # Create new log
+            log = myokit.DataLog()
+            log.set_time_key(self._time_key)
+            for key in self._log_keys:
+                log[key] = np.zeros(log_times.shape)
+            offset = 0
 
-            # Trim end of line
-            line = line.rstrip(' \r\n\f;')
+        else:
 
-            # Get enumerated iterator over characters
-            line = enumerate(line)
+            # Check existing log
+            if len(log.keys()) > len(self._log_keys):
+                raise ValueError('Invalid log: contains extra keys.')
             try:
-                i, c = next(line)
-            except StopIteration:
-                # Empty line
-                return log
-
-            # Whitespace characters to ignore
-            whitespace = ' \f\t'
-
-            # Start parsing header fields
-            run1 = True
-            while run1:
-                text = []
-
-                # Skip whitespace
-                # (Note: rtrim above and check below mean this will never
-                #  raise a StopIteration)
-                while c in whitespace:
-                    i, c = next(line)
-
-                # Read!
-                if c == quote:
-
-                    # Read quoted field + delimiter
-                    run2 = True
-                    while run2:
-                        try:
-                            i, c = next(line)
-                        except StopIteration:
-                            e(1, i, 'Unexpected end-of-line inside quoted'
-                                ' string.')
-
-                        if c == quote:
-                            try:
-                                i, c = next(line)
-                                if c == quote:
-                                    text.append(quote)
-                                elif c == delim or c in whitespace:
-                                    run2 = False
-                                else:
-                                    e(1, i, 'Expecting double quote, delimiter'
-                                        ' or end-of-line. Found "' + c + '".')
-                            except StopIteration:
-                                run1 = run2 = False
-                        else:
-                            text.append(c)
-                else:
-
-                    # Read unquoted field + delimiter
-                    while run1 and c != delim:
-                        try:
-                            text.append(c)
-                            i, c = next(line)
-                        except StopIteration:
-                            run1 = False
-
-                # Append new field to list
-                key = ''.join(text)
-                if key == '':
-                    e(1, i, 'Empty field in header.')
-                keys.append(key)
-
-                # Read next character
-                try:
-                    i, c = next(line)
-                except StopIteration:
-                    run1 = False
-
-            if c == delim:
-                e(1, i, 'Empty field in header.')
-
-            # Create data structure
-            m = len(keys)
-            lists = []
-            for key in keys:
-                x = array.array(typecode)
-                lists.append(x)
-                log[key] = x
-
-            # Read remaining data
-            n = 0
-            while True:
-                row = f.readline()
-
-                # Stop if a blank line is returned: indicates EOF!
-                # (Empty line in file still has line ending)
-                if row == '':
-                    break
+                key = self._time_key    # Note: error msg below uses `key`
+                offset = len(log[key])
+                for key in self._log_keys:
+                    log[key] = np.concatenate((
+                        log[key], np.zeros(log_times.shape)))
+            except KeyError:
+                raise ValueError(
+                    'Invalid log: missing entry for <' + str(key) + '>.')
 
-                # Strip leading and/or trailing whitespace
-                row = row.lstrip().rstrip(' \r\n\f;')
+        # Run simulation
+        if self._protocol is None:
 
-                # Skip blank lines
-                if row == '':
-                    continue
+            # User defined membrane potential
+            self._run(log, log_times, self._time + duration, offset)
 
-                # Ignore lines commented with #
-                if row[:1] == '#':
-                    continue
+        else:
 
-                # Split row into cells
-                row = row.split(delim)
-                n += 1
-                if len(row) != m:
-                    e(
-                        n, 0, 'Wrong number of columns found in row '
-                        + str(n) + '. Expecting ' + str(m) + ', found '
-                        + str(len(row)) + '.')
-                try:
-                    for k, v in enumerate(row):
-                        lists[k].append(float(v))
-                except ValueError:
-                    e(n, 0, 'Unable to convert found data to floats.')
-
-            # Guess time variable
-            for key in keys:
-                x = np.array(log[key], copy=False)
-                y = x[1:] - x[:-1]
-                if np.all(y > 0):
-                    log.set_time_key(key)
-                    break
+            # Voltage clamp
+            tfinal = self._time + duration
+            while self._time < tfinal:
+                # Run simulation
+                tnext = min(tfinal, self._pacing.next_time())
+                times = log_times[np.logical_and(
+                    log_times >= self._time, log_times < tnext)]
+                self._run(log, times, tnext, offset)
+                offset += len(times)
 
-            # Return log
-            return log
+                # Update pacing
+                self._membrane_potential = self._pacing.advance(tnext)
 
-    def npview(self):
-        """
-        Returns a ``DataLog`` with numpy array views of this log's data.
-        """
-        log = DataLog()
-        log._time = self._time
-        for k, v in self.items():
-            log[k] = np.asarray(v)
+        # Return
         return log
 
-    def _parse_key(self, key):
-        """
-        Parses a key used for __getitem__, __setitem__, __delitem__ and
-        __contains__.
+    def _run(self, log, times, tnext, offset):
         """
-        if type(key) == tuple:
-            name = str(key[0])
-            if len(key) == 2 and type(key[1]) not in [int, float]:
-                parts = [str(x) for x in key[1]]
-            else:
-                parts = [str(x) for x in key[1:]]
-            parts.append(str(name))
-            key = '.'.join(parts)
-        return str(key)
-
-    def regularize(self, dt, tmin=None, tmax=None):  # pragma: no cover
-        """
-        Returns a copy of this DataLog with data points at regularly spaced
-        times.
-
-        This method is deprecated and will be removed in future versions of
-        Myokit.
-
-        This method requires ``SciPy`` to be installed.
-
-        *Note: While regularize() can be used post-simulation to create fixed
-        time-step data from variable time-step data, it is usually better to
-        re-run a simulation with fixed time step logging. See*
-        :meth:`Simulation.run()` *for details.*
-
-        The first point will be at ``tmin`` if specified or otherwise the first
-        time present in the log. All following points will be spaced ``dt``
-        time units apart and the final point will be less than or equal to
-        ``tmax``. If no value for ``tmax`` is given the final value in the log
-        is used.
-
-        This method works by
-
-          1. Finding the indices corresponding to ``tmin`` and ``tmax``.
-          2. Creating a spline interpolant with all the data from ``tmin`` to
-             ``tmax``. If possible, two points to the left and right of
-             ``tmin`` and ``tmax`` will be included in the interpolated data
-             set (so *only* if there are at least two values before ``tmin`` or
-             two values after ``tmax`` in the data respectively).
-          3. Evaluating the interpolant at the regularly spaced points.
+        Runs a simulation with the current membrane potential.
+
+        Arguments:
+
+        ``log``
+            The log to append to.
+        ``times``
+            The times to evaluate at.
+        ``tnext``
+            The final time to move to.
+        ``offset``
+            The offset in the ``times`` array to log in
 
-        As a result of the cubic spline interpolation, the function may perform
-        poorly on large data sets.
         """
-        # Deprecated since 2023-06-06
-        import warnings
-        warnings.warn(
-            'The method `regularize` is deprecated and will be removed in'
-            ' future versions of Myokit.')
+        # Simulate with fixed V
+        if self._has_current:
+            states, currents = self.solve(times - self._time)
+        else:
+            states = self.solve(times - self._time)
 
-        from scipy.interpolate import UnivariateSpline as Spline
-        self.validate()
+        # Log results
+        lo = offset
+        hi = lo + len(times)
+        key = log.time_key()
+        log[key][lo:hi] = times
+        for i, key in enumerate(self._model.states()):
+            log[key][lo:hi] = states[i]
+        if self._has_current:
+            key = self._model.current()
+            log[key][lo:hi] = currents
+        key = self._model._membrane_potential
+        log[key][lo:hi] = self._membrane_potential
+
+        # Now run simulation for final time (which might not be included in the
+        # list of logged times, and should not, if you want to be able to
+        # append logs without creating duplicate points).
+        times = np.array([tnext - self._time])
+        if self._has_current:
+            states, currents = self.solve(times)
+        else:
+            states = self.solve(times)
 
-        # Check time variable
-        time = self.time()
-        n = len(time)
-
-        # Get left index for splines
-        imin = 0
-        if tmin is None:
-            tmin = time[0]
-        elif tmin > time[0]:
-            # Find position of tmin in time list, then add two points to the
-            # left so that the spline has 4 points
-            imin = max(0, np.searchsorted(time, tmin) - 2)
-
-        # Get right index for splines
-        imax = n
-        if tmax is None:
-            tmax = time[-1]
-        elif tmax < time[-1]:
-            imax = min(n, np.searchsorted(time, tmax) + 2)
-
-        # Get time steps
-        steps = 1 + np.floor((tmax - tmin) / dt)
-        rtime = tmin + dt * np.arange(0, steps)
-
-        # Create output and return
-        out = DataLog()
-        out._time = self._time
-        out[self._time] = rtime
-        time_part = time[imin:imax]
-        for key, data in self.items():
-            if key != self._time:
-                s = Spline(time_part, data[imin:imax], k=1, s=0)
-                out[key] = s(rtime)
-        return out
-
-    def save(self, filename, precision=myokit.DOUBLE_PRECISION):
-        """
-        Writes this ``DataLog`` to a binary file.
-
-        The resulting file will be a zip file with the following entries:
-
-        ``header.txt``
-            A csv file with the fields ``name, dtype, len`` for each variable.
-        ``data.bin``
-            The binary data in the order specified by the header.
-        ``readme.txt``
-            A text file explaining the file format.
-
-        The optional argument ``precision`` allows logs to be stored in single
-        precision format, which saves space.
+        # Update simulation state
+        self._state = np.array(states[:, -1], copy=True)
+        self._time = tnext
+
+    def set_constant(self, variable, value):
+        """
+        Updates a single parameter to a new value.
         """
-        self.validate()
+        self._parameters[self._parameter_map[variable]] = float(value)
 
-        # Check filename
-        filename = os.path.expanduser(filename)
+    def set_default_state(self, state):
+        """
+        Changes this simulation's default state.
+        """
+        state = np.array(state, copy=True, dtype=float)
+        if len(state) != len(self._state):
+            raise ValueError(
+                'Wrong size state vector, expecing (' + str(len(self._state))
+                + ') values.')
+        if np.any(state < 0):
+            raise ValueError(
+                'The fraction of channels in a state cannot be negative.')
+        if np.abs(np.sum(state) - 1) > 1e-6:
+            raise ValueError('The values in `state` must sum to 1.')
+        self._default_state = state
 
-        # Load compression modules
-        import zipfile
-        try:
-            # Make sure zlib is available
-            import zlib
-            del zlib
-        except ImportError:
+    def set_membrane_potential(self, v):
+        """
+        Changes the membrane potential used in this simulation.
+        """
+        if self._protocol:
             raise Exception(
-                'This method requires the `zlib` module to be installed.')
+                'Membrane potential cannot be set if a protocol is used.')
+        self._membrane_potential = float(v)
+
+    def set_parameters(self, parameters):
+        """
+        Changes the parameter values used in this simulation.
+        """
+        if len(parameters) != len(self._parameters):
+            raise ValueError(
+                'Wrong size parameter vector, expecting ('
+                + str(len(self._parameters)) + ') values.')
+        self._parameters = np.array(parameters, copy=True, dtype=float)
 
-        # Data type
-        dtype = 'd' if precision == myokit.DOUBLE_PRECISION else 'f'
+        # Invalidate cache
+        self._cached_matrices = {}
+        self._cached_solution = {}
 
-        # Create data strings
-        head_str = []
-        body_str = []   # Will be filled with bytes
-
-        # Number of fields, length of data arrays, data type, time, fields
-        head_str.append(str(len(self)))
-        head_str.append(str(len(next(iter(self.values())))))
-        head_str.append(dtype)
-
-        # Note: the time field might not be present in the log!
-        head_str.append(self._time if self._time else '')
-
-        # Write field names and data
-        enc = 'utf8'
-        for k, v in self.items():
-            head_str.append(k)
-            # Create array, ensure it's litte-endian
-            ar = array.array(dtype, v)
-            if sys.byteorder == 'big':  # pragma: no cover
-                ar.byteswap()
-            body_str.append(ar.tobytes())
-        head_str = '\n'.join(head_str)
-        body_str = b''.join(body_str)
-
-        # 2018-07-15: Wondering why I chose body-head-readme ordering now...
-
-        # Write
-        head = zipfile.ZipInfo('structure.txt')
-        head.compress_type = zipfile.ZIP_DEFLATED
-        body = zipfile.ZipInfo('data.bin')
-        body.compress_type = zipfile.ZIP_DEFLATED
-        read = zipfile.ZipInfo('readme.txt')
-        read.compress_type = zipfile.ZIP_DEFLATED
-        with zipfile.ZipFile(filename, 'w') as f:
-            f.writestr(body, body_str)
-            f.writestr(head, head_str.encode(enc))
-            f.writestr(read, README_SAVE_BIN.encode(enc))
-
-    def save_csv(
-            self, filename, precision=myokit.DOUBLE_PRECISION, order=None,
-            delimiter=',', header=True):
-        """
-        Writes this ``DataLog`` to a CSV file, following the syntax
-        outlined in RFC 4180 and with a header indicating the field names.
-
-        The resulting file will consist of:
-
-          - A header line containing the names of all logged variables,
-            separated by commas. If present, the time variable will be the
-            first entry on the line. The remaining keys are ordered using a
-            natural sort order.
-          - Each following line will be a comma separated list of values in the
-            same order as the header line. A line is added for each time point
-            logged.
+    def set_state(self, state):
+        """
+        Changes the initial state used by in this simulation.
+        """
+        state = np.array(state, copy=True, dtype=float)
+        if len(state) != len(self._state):
+            raise ValueError(
+                'Wrong size state vector, expecing (' + str(len(self._state))
+                + ') values.')
+        if np.any(state < 0):
+            raise ValueError(
+                'The fraction of channels in a state cannot be negative.')
+        if np.abs(np.sum(state) - 1) > 1e-6:
+            raise ValueError('The values in `state` must sum to 1.')
+        self._state = state
+
+    def solve(self, times):
+        """
+        Evaluates and returns the states at the given times.
+
+        In contrast to :meth:`run()`, this method simply evaluates the states
+        (and current) at the given times, using the last known settings for
+        the state and membrane potential. It does not use a protocol and does
+        not take into account the simulation time. After running this method,
+        the state and simulation time are *not* updated.
 
         Arguments:
 
-        ``filename``
-            The file to write (existing files will be overwritten without
-            warning.
-        ``precision``
-            If a precision argument (for example ``myokit.DOUBLE_PRECISION``)
-            is given, the output will be stored in such a way that this amount
-            of precision is guaranteed to be present in the string. If the
-            precision argument is set to ``None`` Python's default formatting
-            is used, which may lead to smaller files.
-        ``order``
-            To specify the ordering of the log's arguments, pass in a sequence
-            ``order`` with the log's keys.
-        ``delimiter``
-            This field can be used to set an alternative delimiter. To use
-            spaces set ``delimiter=' '``, for tabs: ``delimiter='\\t'``. Note
-            that some delimiters (for example '\\n' or '1234') will produce an
-            unreadable or invalid csv file.
-        ``header``
-            Set this to ``False`` to avoid adding a header to the file. Note
-            that Myokit will no longer be able to read the written csv file
-            without this header.
-
-        *A note about locale settings*: On Windows systems with a locale
-        setting that uses the comma as a decimal separator, importing CSV files
-        into Microsoft Excel can be troublesome. To correctly import a CSV,
-        either (1) Change your locale settings to use "." as a decimal
-        separator or (2) Use the import wizard under Data > Get External Data
-        to manually specify the correct separator and delimiter.
-        """
-        self.validate()
-
-        # Check filename
-        filename = os.path.expanduser(filename)
-
-        # Set precision
-        if precision is None:
-            fmat = lambda x: str(x)
-        elif precision == myokit.DOUBLE_PRECISION:
-            fmat = lambda x: myokit.SFDOUBLE.format(x)
-        elif precision == myokit.SINGLE_PRECISION:
-            fmat = lambda x: myokit.SFSINGLE.format(x)
-        else:
-            raise ValueError('Precision level not supported.')
+        ``times``
+            A series of times, where each time must be some ``t >= 0``.
 
-        # Write file
-        # EOL: CSV files have DOS line endings by convention. On windows,
-        # writing '\n' to a file opened in mode 'w' will actually write '\r\n'
-        # which means writing '\r\n' writes '\r\r\n'. To prevent this, open the
-        # file in mode 'wb'.
-        eol = '\r\n'
-        quote = '"'
-        escape = '""'
-        with open(filename, 'wb') as f:
-            # Convert dict structure to ordered sequences
-            if order:
-                order = [str(x) for x in order]
-                if set(order) != set(self.keys()):
-                    raise ValueError(
-                        'The given `order` sequence must contain all the same'
-                        ' keys present in the log.')
-                keys = order
-                data = [self[x] for x in keys]
-            else:
-                keys = []
-                data = []
-                if self._time and self._time in self.keys():
-                    # Save time as first variable
-                    dat = self[self._time]
-                    keys.append(self._time)
-                    data.append(dat)
-                for key, dat in sorted(
-                        self.items(),
-                        key=lambda i: myokit.tools.natural_sort_key(i[0])):
-                    if key != self._time:
-                        keys.append(key)
-                        data.append(dat)
-
-            # Number of entries
-            m = len(keys)
-            if m == 0:
-                return
-
-            # Get length of entries
-            n = self.length()
-
-            # Write header
-            if header:
-                line = []
-                for key in keys:
-                    # Escape quotes within strings
-                    line.append(quote + key.replace(quote, escape) + quote)
-                f.write((delimiter.join(line) + eol).encode('ascii'))
-
-            # Write data
-            data = [iter(x) for x in data]
-            for i in range(0, n):
-                line = []
-                for d in data:
-                    line.append(fmat(next(d)))
-                f.write((delimiter.join(line) + eol).encode('ascii'))
-
-    def set_time_key(self, key):
-        """
-        Sets the key under which the time data is stored.
-        """
-        self._time = None if key is None else str(key)
-
-    def __setitem__(self, key, value):
-        return super().__setitem__(
-            self._parse_key(key), value)
-
-    def split(self, value):
-        """
-        Splits the log into a part before and after the time ``value``::
-
-            s = myokit.Simulation(m, p)
-            d = s.run(1000)
-            d1, d2 = d.split(100)
-
-        In this example, d1 will contain all values up to, but not including,
-        t=100. While d2 will contain the values from t=100 and upwards.
-        """
-        return self.isplit(self.find_after(value))
-
-    def split_periodic(self, period, adjust=False, closed_intervals=True):
-        """
-        Splits this log into multiple logs, each covering an equal period of
-        time. For example a log covering the time span ``[0, 10000]`` can be
-        split with period ``1000`` to obtain ten logs covering ``[0, 1000]``,
-        ``[1000, 2000]`` etc.
-
-        The split log files can be returned as-is, or with the time variable's
-        value adjusted so that all logs appear to cover the same span. To
-        enable this option, set ``adjust`` to ``True``.
-
-        By default, the returned intervals are *closed*, so both the left and
-        right endpoint are included (if present in the data). This may involve
-        the duplication of some data points. To disable this behavior and
-        return half-closed endpoints (containing only the left point), set
-        ``closed_intervals`` to ``False``.
-        """
-        # Validate log before starting
-        self.validate()
-
-        # Check time variable
-        time = self.time()
-        if len(time) < 1:
-            raise RuntimeError('DataLog entries have zero length.')
-
-        # Check period
-        period = float(period)
-        if period <= 0:
-            raise ValueError('Period must be greater than zero')
-
-        # Get start, end, etc
-        tmin = 0    # time[0]
-        tmax = time[len(time) - 1]
-        nlogs = int(np.ceil((tmax - tmin) / period))
-
-        # No splitting needed? Return clone!
-        if nlogs < 2:
-            return self.clone()
-
-        # Find split points
-        tstarts = tmin + np.arange(nlogs) * period
-        istarts = [0] * nlogs
-        k = 0
-        for i, t in enumerate(time):
-            while k < nlogs and t >= tstarts[k]:
-                istarts[k] = i
-                k += 1
-
-        # Create logs
-        logs = []
-        for i in range(0, nlogs - 1):
-            log = DataLog()
-            log._time = self._time
-
-            # Get indices
-            imin = istarts[i]
-            imax = istarts[i + 1]
-
-            # Include right point endpoint if needed
-            if closed_intervals and time[imax] == tstarts[i + 1]:
-                imax += 1
-
-            # Select sections of log and append
-            for k, v in self.items():
-                d = self[k][imin:imax]
-                # NumPy? Then copy data
-                if isinstance(d, np.ndarray):
-                    d = np.array(d, copy=True, dtype=float)
-                log[k] = d
-            logs.append(log)
-
-        # Last log
-        log = DataLog()
-        log._time = self._time
-        imin = istarts[-1]
-        imax = len(time)
-
-        # Not including right endpoints? Then may be required to omit last pt
-        if not closed_intervals and time[-1] >= tmin + nlogs * period:
-            imax -= 1
-
-        # Select sections of log and append
-        for k, v in self.items():
-            d = self[k][imin:imax]
-            # NumPy? Then copy data
-            if isinstance(d, np.ndarray):
-                d = np.array(d, copy=True, dtype=float)
-            log[k] = d
-        logs.append(log)
-
-        # Adjust
-        if adjust:
-            if isinstance(time, np.ndarray):
-                # Fast method for numpy arrays
-                for k, log in enumerate(logs):
-                    log[self._time] -= k * period
-            else:
-                for k, log in enumerate(logs):
-                    tlist = log[self._time]
-                    tdiff = k * period
-                    for i in range(len(tlist)):
-                        tlist[i] -= tdiff
-
-        # Return
-        return logs
+        For models with a current variable, this method returns a tuple
+        ``(state, current)`` where ``state`` is a matrix of shape
+        ``(len(states), len(times))`` and ``current`` is a vector
+        of length ``len(times)``.
 
-    def time(self):
+        For models without a current variable, only ``state`` is returned.
         """
-        Returns this log's time array.
+        n = len(self._state)
 
-        Raises a :class:`myokit.InvalidDataLogError` if the time variable for
-        this log has not been specified or an invalid key was given for the
-        time variable.
-        """
+        # Solve system, or get cached solution
         try:
-            return self[self._time]
+            E, P, PI, B = self._cached_solution[self._membrane_potential]
         except KeyError:
-            if self._time is None:
-                raise myokit.InvalidDataLogError('No time variable set.')
-            else:
-                raise myokit.InvalidDataLogError(
-                    'Invalid key <' + str(self._time)
-                    + '> set for time variable.')
+            # Get matrices
+            A, B = self._matrices()
 
-    def time_key(self):
-        """
-        Returns the name of the time variable stored in this log, or ``None``
-        if no time variable was set.
-        """
-        return self._time
+            # Get eigenvalues, matrix of eigenvectors
+            E, P = np.linalg.eig(A)
+            E = E.reshape((n, 1))
+            PI = np.linalg.inv(P)
 
-    def trim(self, a, b, adjust=False):
-        """
-        Returns a copy of this log, with all data before time ``a`` and after
-        (and including) time ``b`` removed.
+            # Cache results
+            self._cached_solution[self._membrane_potential] = (E, P, PI, B)
 
-        If ``adjust`` is set to ``True``, all logged times will be lowered by
-        ``a``.
-        """
-        self.validate()
-        log = self.itrim(self.find_after(a), self.find_after(b))
-        if adjust and self._time in log:
-            if isinstance(log[self._time], np.ndarray):
-                log[self._time] -= a
-            else:
-                log[self._time] = [x - a for x in log[self._time]]
-        return log
+        # Calculate transform of initial state
+        y0 = PI.dot(self._state.reshape((n, 1)))
 
-    def trim_left(self, value, adjust=False):
-        """
-        Returns a copy of this log, with all data before time ``value``
-        removed.
+        # Reshape times array
+        times = np.array(times, copy=False).reshape((len(times),))
 
-        If ``adjust`` is set to ``True``, all logged times will be lowered by
-        ``value``.
-        """
-        self.validate()
-        log = self.itrim_left(self.find_after(value))
-        if adjust and self._time in log:
-            if isinstance(log[self._time], np.ndarray):
-                log[self._time] -= value
-            else:
-                log[self._time] = [x - value for x in log[self._time]]
-        return log
+        # Calculate state
+        x = P.dot(y0 * np.exp(times * E))
+
+        # Calculate current and/or return
+        if self._has_current:
+            return x, B.dot(x)
+        else:
+            return x
 
-    def trim_right(self, value):
+    def state(self):
         """
-        Returns a copy of this log, with all data at times after and including
-        ``value`` removed.
+        Returns the initial state used by this simulation.
         """
-        return self.itrim_right(self.find_after(value))
+        return list(self._state)
 
-    def validate(self):
-        """
-        Validates this ``DataLog``. Raises a
-        :class:`myokit.InvalidDataLogError` if the log has inconsistencies.
-        """
-        if self._time:
-            if self._time not in self:
-                raise myokit.InvalidDataLogError(
-                    'Time variable <' + str(self._time)
-                    + '> specified but not found in log.')
-            dt = np.asarray(self[self._time])
-            if np.any(dt[1:] - dt[:-1] < 0):
-                raise myokit.InvalidDataLogError(
-                    'Time must be non-decreasing.')
-        if len(self) > 0:
-            n = set([len(v) for v in self.values()])
-            if len(n) > 1:
-                raise myokit.InvalidDataLogError(
-                    'All entries in a data log must have the same length.')
-
-    def variable_info(self):
-        """
-        Returns a dictionary mapping fully qualified variable names to
-        :class:`LoggedvariableInfo` instances, providing information about the
-        logged data.
-
-        Comes with the following constraints:
-
-        - Per variable, the data must have a consistent dimensionality. For
-          example having a key ``0.membrane.V`` and a key ``1.1.membrane.V``
-          would violate this constraint.
-        - Per variable, the data must be regular accross dimensions. For
-          example if there are ``n`` entries ``0.x.membrane.V``, and there are
-          also entries of the form ``1.x.membrane.V`` then the values of ``x``
-          must be the same for both cases.
-
-        An example of a dataset that violates the second constraint is::
-
-            0.0.membrane.V
-            0.1.membrane.V
-            0.2.membrane.V
-            1.0.membrane.V
-            1.1.membrane.V
-
-        If either of the constraints is violated a ``ValueError`` is raised.
-        """
-        # The algorithm for condition 2 works by creating a set of the unique
-        # entries in each column. The product of the sizes of these sets should
-        # equal the total number of entries for a variable.
-        # For example:
-        #   0 1
-        #   0 2     Results in id_sets [(0,1), (1,2,3,4)]
-        #   0 3     2 * 4 = 8 != len(id_list)
-        #   1 1     So this data must be irregular.
-        #   1 2
-        #   1 4
-        #
-        id_lists = {}
-        id_sets = {}
-        for key in self:
-            # Split key into id / name parts
-            idx, name = split_key(key)
-
-            # Create tuple version of id
-            idx = idx.split('.')
-            idx = idx[:-1]
-            idx = tuple([int(i) for i in idx])
 
-            # Find or create entry in dict of id lists
-            try:
-                id_list = id_lists[name]
-                id_set = id_sets[name]
-            except KeyError:
-                # Create entry in id lists dict
-                id_lists[name] = id_list = []
+class DiscreteSimulation:
+    """
+    Performs stochastic simulations of a :class:`LinearModel`'s behavior for a
+    finite number of channels.
 
-                # Create entry in id sets dict (one set for every dimension)
-                id_sets[name] = id_set = [set() for x in idx]
+    Simulations are run using the "Direct method" proposed by Gillespie [1].
 
-            # Check if the dimensions are the same each time a name occurs.
-            if id_list and len(id_list[0]) != len(idx):
-                key1 = '.'.join([str(x) for x in id_list[0]]) + '.' + name
-                key2 = '.'.join([str(x) for x in idx]) + '.' + name
-                raise RuntimeError(
-                    'Different dimensions used for the same variable. Found: <'
-                    + key1 + '> and <' + key2 + '>.')
+    Each simulation object maintains an internal state consisting of
 
-            # Update the id list
-            id_list.append(idx)
+    * The current simulation time
+    * The current state
+    * The default state
 
-            # Update the id set
-            for k, i in enumerate(idx):
-                id_set[k].add(i)
+    When a simulation is created, the simulation time is set to zero and both
+    the current and default state are initialized using the ``LinearModel``.
+    After each call to :meth:`run()` the time and current state are updated,
+    so that each successive call to run continues where the previous simulation
+    left off.
 
-        # Create variable info objects
-        infos = {}
-        for name, id_list in id_lists.items():
-            id_set = id_sets[name]
+    A :class:`protocol <myokit.Protocol>` can be used to set the membrane
+    potential during the simulation, or the membrane potential can be adjusted
+    manually between runs.
 
-            # Check if the data is regular.
-            n = len(id_list)
-            m = 1
-            for x in id_set:
-                m *= len(x)
+    Example::
 
-            if n != m:
-                raise RuntimeError(
-                    'Irregular data used for variable <' + str(name) + '>')
+        import myokit
+        import myokit.lib.markov as markov
 
-            # Create variable info object
-            infos[name] = info = LoggedVariableInfo()
-            info._name = name
-            info._dimension = len(id_set)
-            info._size = tuple([len(x) for x in id_set])
+        # Create linear markov model
+        m = myokit.load_model('clancy-1999.mmt')
+        m = markov.LinearModel.from_component(m.get('ina'))
 
-            # Add sorted ids
-            if id_list[0]:
-                id_list.sort()
-            info._ids = id_list
+        # Run discrete simulation
+        s = markov.DiscreteSimulation(m, nchannels=1000)
+        s.set_membrane_potential(-30)
+        d = s.run(10)
 
-            # Add sorted keys
-            s = '.' + name if id_list[0] else name
-            info._keys = ['.'.join([str(x) for x in y]) + s for y in id_list]
+        import matplotlib.pyplot as plt
+        plt.figure()
+        for state in m.states():
+            plt.step(d.time(), d[state], label=state)
+        plt.legend()
+        plt.show()
 
-        return infos
+    References
 
+    [1] Gillespie (1976) A General Method for Numerically Simulating the
+        stochastic time evolution of coupled chemical reactions
+        The Journal of Computational Physics, 22, 403-434.
+
+    Arguments:
+
+    ``model``
+        A :class:`LinearModel`.
+    ``nchannels``
+        The number of channels to simulate.
 
-class LoggedVariableInfo:
-    """
-    Contains information about the log entries for each variable. These objects
-    should only be created by :meth:`DataLog.variable_info()`.
     """
-    def __init__(self):
-        self._dimension = None
-        self._ids = None
-        self._keys = None
-        self._size = None
-        self._name = None
 
-    def dimension(self):
+    def __init__(self, model, protocol=None, nchannels=100):
+        # Check model
+        if not isinstance(model, LinearModel):
+            raise ValueError('First parameter must be a `LinearModel`.')
+        self._model = model
+
+        # Check protocol
+        if protocol is None:
+            self._protocol = None
+        elif not isinstance(protocol, myokit.Protocol):
+            raise ValueError('Protocol must be a myokit.Protocol object')
+        else:
+            self._protocol = protocol.clone()
+
+        # Get state and discretize
+        nchannels = int(nchannels)
+        if nchannels < 1:
+            raise ValueError('The number of channels must be at least 1.')
+        self._nchannels = nchannels
+
+        # Set state
+        self._state = self.discretize_state(self._model.default_state())
+
+        # Set default state
+        self._default_state = list(self._state)
+
+        # Set membrane potential
+        self._membrane_potential = self._model.default_membrane_potential()
+
+        # Set parameters
+        self._parameters = np.array(
+            self._model.default_parameters(), copy=True, dtype=float)
+
+        # Mapping from parameter names to index in parameter array
+        self._parameter_map = {}
+        for i, p in enumerate(self._model.parameters()):
+            self._parameter_map[p] = i
+
+        # Cached transition rate list & current matrix
+        self._cached_rates = None
+        self._cached_matrix = None
+
+        # Set simulation time
+        self._time = 0
+
+        # If protocol was given, create pacing system, update vm
+        self._pacing = None
+        if self._protocol:
+            self._pacing = myokit.PacingSystem(self._protocol)
+            self._membrane_potential = self._pacing.advance(self._time)
+
+    def default_state(self):
         """
-        Returns the dimensions of the logged data for this variable, as an
-        integer.
+        Returns the default simulation state.
         """
-        return self._dimension
+        return list(self._default_state)
 
-    def ids(self):
+    def discretize_state(self, x):
         """
-        Returns an iterator over all available ids for this variable, such
-        that the second index (y in the simulation) changes fastest. For
-        example, for log entries::
+        Converts a list of fractional state occupancies to a list of channel
+        counts.
 
-            0.0.membrane.V
-            0.1.membrane.V
-            0.2.membrane.V
-            1.0.membrane.V
-            1.1.membrane.V
-            1.2.membrane.V
+        Arguments:
 
-        the returned result would iterate over::
+        ``x``
+            A fractional state where ``sum(x) == 1``.
 
-            [(0, 0), (0, 1), (0, 2), (1, 0), (1, 1), (1, 2)]
+        Returns a discretized state ``y`` where ``sum(y) = nchannels``.
+        """
+        x = np.array(x, copy=False, dtype=float)
+        if (np.abs(1 - np.sum(x))) > 1e-6:
+            raise ValueError(
+                'The sum of fractions in the state to be discretized must'
+                ' equal 1.')
+        y = np.round(x * self._nchannels)
+        # To make sure it always sums to 1, correct the value found at the
+        # index with the biggest rounding error.
+        i = np.argmax(np.abs(x - y))
+        y[i] = 0
+        y[i] = self._nchannels - np.sum(y)
+        return list(y)
 
-        The keys are returned in the same order as the ids.
+    def membrane_potential(self):
+        """
+        Returns the current membrane potential.
         """
-        return iter(self._ids)
+        return self._membrane_potential
 
-    def is_regular_grid(self):
+    def number_of_channels(self):
+        """
+        Returns the number of channels used in this simulation.
         """
-        Returns True if the following conditions are met:
+        return self._nchannels
 
-        - The data 2 dimensional
-        - The data is continuous: along each dimension the first data point is
-          indexed as ``0`` and the last as ``Ni-1``, where ``Ni`` is the size
-          in that dimension.
+    def parameters(self):
+        """
+        Returns the current parameter values.
+        """
+        return list(self._parameters)
 
+    def pre(self, duration):
         """
-        nx, ny = self._size
-        return (
-            self._dimension == 2
-            and self._ids[0][0] == 0
-            and self._ids[0][1] == 0
-            and self._ids[-1][0] == nx - 1
-            and self._ids[-1][1] == ny - 1
-        )
+        Performs an unlogged simulation for ``duration`` time units and uses
+        the final state as the new default state.
 
-    def keys(self):
+        After the simulation:
+
+        - The simulation time is **not** affected
+        - The current state and the default state are updated to the final
+          state reached in the simulation.
+
+        Calls to :meth:`reset` after using :meth:`pre` will set the current
+        state to this new default state.
         """
-        Returns an iterator over all available keys for this variable, such
-        that the second index (y in the simulation) changes fastest. For
-        example, for log entries::
+        # Check arguments
+        duration = float(duration)
+        if duration < 0:
+            raise ValueError('Duration must be non-negative.')
+
+        # Run
+        # This isn't much faster, but this way the simulation's interface is
+        # similar to the standard simulation one.
+        old_time = self._time
+        self.run(duration)
 
-            0.0.membrane.V
-            1.0.membrane.V
-            0.1.membrane.V
-            1.1.membrane.V
-            0.2.membrane.V
-            1.2.membrane.V
+        # Update default state
+        self._default_state = list(self._state)
 
-        the returned iterator would produce ``"0.0.membrane.V"``, then
-        ``"0.1.membrane.V"`` etc.
+        # Reset time, reset protocol
+        self._time = old_time
+        if self._protocol:
+            self._pacing = myokit.PacingSystem(self._protocol)
+            self._membrane_potential = self._pacing.advance(self._time)
 
-        The ids are returned in the same order as the keys.
+    def _current_matrix(self):
         """
-        return iter(self._keys)
+        Returns the (cached or regenerated) current matrix B.
+        """
+        if self._cached_matrix is None:
+            self._cached_matrix = self._model.matrices(
+                self._membrane_potential, self._parameters)[1]
+        return self._cached_matrix
 
-    def size(self):
+    def _rates(self):
+        """
+        Returns the (cached or regenerated) transition rate list.
         """
-        Returns a tuple containing the size i.e. the number of entries for
-        the corresponding variable in each dimension.
+        if self._cached_rates is None:
+            self._cached_rates = self._model.rates(
+                self._membrane_potential, self._parameters)
+        return self._cached_rates
 
-        For example, with the following log entries for `membrane.V`::
+    def reset(self):
+        """
+        Resets the simulation:
 
-            0.membrane.V
-            1.membrane.V
-            2.membrane.V
+        - The time variable is set to zero.
+        - The state is set to the default state.
 
-        the corresponding size would be ``(3)``.
+        """
+        self._time = 0
+        self._state = list(self._default_state)
+        if self._protocol:
+            self._pacing = myokit.PacingSystem(self._protocol)
+            self._membrane_potential = self._pacing.advance(self._time)
 
-        A size of ``3`` doesn't guarantee the final entry is for cell number
-        ``2``. For example::
+    def run(self, duration, log=None):
+        """
+        Runs a simulation for ``duration`` time units.
 
-            0.membrane.V
-            10.membrane.V
-            20.membrane.V
+        After the simulation:
 
-        would also return size ``(3)``
+        - The simulation time will be increased by ``duration`` time units.
+        - The simulation state will be updated to the last reached state.
 
-        In higher dimensions::
+        Arguments:
 
-            0.0.membrane.V
-            0.1.membrane.V
-            0.2.membrane.V
-            1.0.membrane.V
-            1.1.membrane.V
-            1.2.membrane.V
+        ``duration``
+            The number of time units to simulate.
+        ``log``
+            A log from a previous run can be passed in, in which case the
+            results will be appended to this one.
+
+        Returns a :class:`myokit.DataLog` with the simulation results.
+        """
+        # Check arguments
+        duration = float(duration)
+        if duration < 0:
+            raise ValueError('Duration must be non-negative.')
+
+        # Set up logging
+        time_key = self._model._model.time().qname()
+        log_vars = [time_key, self._model._membrane_potential]
+        log_vars.extend(self._model.states())
+        cur_key = self._model.current()
+        if cur_key is not None:
+            log_vars.append(cur_key)
+
+        if log is None:
+            # Create new log
+            log = myokit.DataLog()
+            log.set_time_key(time_key)
+            for var in log_vars:
+                log[var] = []
 
-        This would return ``(2,3)``.
+        else:
 
-        Similarly, in a single cell scenario or for global variables, for
-        exmaple::
+            # Check existing log
+            if len(log.keys()) > len(log_vars):
+                raise ValueError('Invalid log: contains extra keys.')
+            try:
+                for key in log_vars:
+                    log[key]
+            except KeyError:
+                raise ValueError(
+                    'Invalid log: missing entry for <' + str(key) + '>.')
+
+        if self._protocol is None:
+            # Simulate with fixed V
+            self._run(duration, log)
+
+        else:
+
+            # Voltage clamp
+            tfinal = self._time + duration
+            while self._time < tfinal:
+                # Run simulation
+                tnext = min(tfinal, self._pacing.next_time())
+                self._run(tnext - self._time, log)
+                # Update pacing
+                self._membrane_potential = self._pacing.advance(tnext)
+                self._cached_rates = None
+                self._cached_matrix = None
+
+        # Return
+        return log
+
+    def _run(self, duration, log):
+        """
+        Runs a simulation with the current membrane potential.
+        """
+        # Get logging lists
+        log_time = log.time()
+        log_states = []
+        for key in self._model.states():
+            log_states.append(log[key])
+
+        # Get current, time and state
+        t = self._time
+        state = np.array(self._state, copy=True, dtype=int)
+
+        # Get list of transitions
+        R = []      # Transition rates
+        SI = []     # From state
+        SJ = []     # To state
+        for i, j, rij in self._rates():
+            SI.append(i)
+            SJ.append(j)
+            R.append(rij)
+        R = np.array(R)
+        SI = np.array(SI)
+        SJ = np.array(SJ)
+
+        # Run
+        n_steps = 0
+        t_stop = self._time + duration
+
+        # Request for a short time can result in duration=0 at this point,
+        # Must set variables otherwise set in loop below here
+        if t >= t_stop:
+            lambdas = R * state[SI]
+
+        while t < t_stop:
+            # Log
+            log_time.append(t)
+            for i, x in enumerate(state):
+                log_states[i].append(x)
+            n_steps += 1
+
+            # Get lambdas
+            lambdas = R * state[SI]
+
+            # Get sum of lambdas
+            lsum = np.sum(lambdas)
+
+            # Sample time until next transition from an exponential
+            # distribution with mean 1 / lsum
+            tau = np.random.exponential(1 / lsum)
+
+            # Don't step beyond the stopping time!
+            if t + tau > t_stop:
+                break
+
+            # Get type of transition
+            transition = np.random.uniform(0, lsum)
+            rsum = 0
+            for i, r in enumerate(lambdas):
+                rsum += r
+                if rsum > transition:
+                    break
+
+            # Perform transition
+            state[SI[i]] -= 1
+            state[SJ[i]] += 1
+            t += tau
+
+        # Perform final step using the "brute-force" approach, ensuring we
+        # reach self._time + duration exactly.
+        # Note that for large tau, the estimates of the probability that
+        # something changes may become inaccurate (and > 1)
+        # I didn't see this in testing...
+        tau = (self._time + duration) - t
+        lambdas *= tau
+        for i, r in enumerate(lambdas):
+            if np.random.uniform(0, 1) < r:
+                # Perform transition
+                state[SI[i]] -= 1
+                state[SJ[i]] += 1
+
+        # Add vm to log
+        vm_key = self._model._membrane_potential
+        log[vm_key].extend([self._membrane_potential] * n_steps)
+
+        # Add current to log
+        c = self._model.current()
+        if c is not None:
+            B = self._current_matrix()
+            x = np.vstack([
+                np.array(log_states[i][-n_steps:], dtype=float)
+                for i in range(len(state))])
+            x /= self._nchannels
+            log[c].extend(B.dot(x))
+
+        # Update current state and time
+        self._state = list(state)
+        self._time += duration
+
+    def set_constant(self, variable, value):
+        """
+        Updates a single parameter to a new value.
+        """
+        self._parameters[self._parameter_map[variable]] = float(value)
+
+    def set_default_state(self, state):
+        """
+        Changes the default state used in the simulation.
+        """
+        state = np.asarray(state, dtype=int)
+        if len(state) != len(self._state):
+            raise ValueError(
+                'Wrong size state vector, expecing (' + str(len(self._state))
+                + ') values.')
+        if np.min(state) < 0:
+            raise ValueError(
+                'The number of channels in a markov model state can not be'
+                ' negative.')
+        if np.sum(state) != self._nchannels:
+            raise ValueError(
+                'The number of channels in the default state vector must'
+                ' equal ' + str(self._nchannels) + '.')
+        self._default_state = list(state)
 
-            engine.time
+    def set_membrane_potential(self, v):
+        """
+        Changes the membrane potential used in this simulation.
+        """
+        if self._protocol:
+            raise Exception(
+                'Membrane potential cannot be set if a protocol is used.')
+        self._membrane_potential = float(v)
+        self._cached_rates = None
+        self._cached_matrix = None
 
-        Would have size ``()``.
+    def set_parameters(self, parameters):
         """
-        return self._size
+        Changes the parameter values used in this simulation.
+        """
+        if len(parameters) != len(self._parameters):
+            raise ValueError(
+                'Wrong size parameter vector, expecting ('
+                + str(len(self._parameters)) + ') values.')
+        self._parameters = np.array(parameters, copy=True, dtype=float)
+        self._cached_rates = None
+        self._cached_matrix = None
 
-    def name(self):
+    def set_state(self, state):
         """
-        Returns the variable name.
+        Changes the current state used in the simulation (i.e. the number of
+        channels in every markov model state).
         """
-        return self._name
+        state = np.asarray(state, dtype=int)
+        if len(state) != len(self._state):
+            raise ValueError(
+                'Wrong size state vector, expecing (' + str(len(self._state))
+                + ') values.')
+        if np.min(state) < 0:
+            raise ValueError(
+                'The state must be given as a list of non-negative integers.')
+        if np.sum(state) != self._nchannels:
+            raise ValueError(
+                'The number of channels in the state vector must equal '
+                + str(self._nchannels) + '.')
+        self._state = list(state)
 
-    def to_long_string(self):   # pragma: no cover (debug function)
-        out = [self._name]
-        out.append('  dimension: ' + str(self._dimension))
-        out.append('  size: ' + ', '.join([str(x) for x in self._size]))
-        out.append('  keys:')
-        out.extend(['    ' + x for x in self._keys])
-        return '\n'.join(out)
+    def state(self):
+        """
+        Returns the current simulation state.
+        """
+        return list(self._state)
 
 
-def prepare_log(
-        log, model, dims=None, global_vars=None, if_empty=myokit.LOG_NONE,
-        allowed_classes=myokit.LOG_ALL, precision=myokit.DOUBLE_PRECISION):
+class MarkovModel:
+    """
+    **Deprecated**: This class has been replaced by the classes
+    :class:`LinearModel` and :class:`AnalyticalSimulation`. Please update your
+    code to use these classes instead. This class will be removed in
+    future versions of Myokit.
     """
-    Returns a :class:`DataLog` for simulation classes based on a ``log``
-    argument passed in by the user. The model the simulations will be based on
-    should be passed in as ``model``.
 
-    The ``log`` argument can take on one of four forms:
+    @staticmethod
+    def from_component(
+            component, states=None, parameters=None, current=None, vm=None):
+        """
+        Creates and returns an :class:`AnalyticalSimulation` using a
+        :class:`LinearModel` based on a Myokit model component.
+        """
+        # Deprecated since 2016-01-25
+        import warnings
+        warnings.warn(
+            'The method `MarkovModel.from_component` is deprecated.'
+            ' Please use `LinearModel.from_component` instead.')
+        return AnalyticalSimulation(LinearModel.from_component(
+            component, states, parameters, current, vm))
 
-    An existing simulation log
-        In this case, the log is tested for compatibility with the given model
-        and simulation dimensions. For single-cell simulations all keys in the
-        log must correspond to the qname of a loggable variable (IE not a
-        constant). For multi-cellular simulations this means all keys in the
-        log must have the form "x.component.variable" where "x" is the cell
-        index (for example "1" or "0.3").
-    A list (or other sequence) of variable names to log.
-        In this case, the list is converted to a DataLog object. All
-        arguments in the list must be either strings corresponding to the
-        variables' qnames (so "membrane.V") or variable objects from the given
-        model.
-        In multi-cell scenarios, passing in the qname of a variable (for
-        example "membrane.V") will cause every cell's instance of this variable
-        to be logged. To log only specific cells' values, pass in the indexed
-        name (for example "1.2.membrane.V").
-    An integer flag
-        One of the following integer flags:
+    def __new__(self, model, states, parameters=None, current=None, vm=None):
+        # Deprecated since 2016-01-25
+        import warnings
+        warnings.warn(
+            'The `MarkovModel` class is deprecated.'
+            ' Please use the `LinearModel` class instead.')
+        return AnalyticalSimulation(LinearModel(
+            model, states, parameters, current, vm))
 
-        ``myokit.LOG_NONE``
-            Don't log any variables.
-        ``myokit.LOG_STATE``
-            Log all state variables.
-        ``myokit.LOG_BOUND``
-            Log all variables bound to an external value. The method will
-            assume any bound variables still present in the model will be
-            provided by the simulation engine.
-        ``myokit.LOG_INTER``
-            Log all intermediary variables.
-        ``myokit.LOG_DERIV``
-            Log the derivatives of the state variables.
-        ``myokit.LOG_ALL``
-            Combines all the previous flags.
 
-        Flags can be chained together, for example
-        ``log=myokit.LOG_STATE+myokit.LOG_BOUND`` will log all bound variables
-        and all states.
-    ``None``
-        In this case the value from ``if_empty`` will be copied into log before
-        the function proceeds to build a log.
+class LinearModelError(myokit.MyokitError):
+    """
+    Raised for issues with constructing or using a :class:`LinearModel`.
+    """
 
-    For multi-dimensional logs the simulation dimensions can be passed in as a
-    tuple of dimension sizes, for example (10,) for a cable of 10 cells and
-    (30,20) for a 30 by 20 piece of tissue.
 
-    Simulations can define variables to be either `per-cell` or `global`. Time,
-    for example, is typically a global variable while membrane potential will
-    be stored per cell. To indicate which is which, a list of global variables
-    can be passed in as ``global_vars``.
+def _linear_combination(expression, variables):
+    """
+    Checks if ``expression`` is a linear combination of the given ``variables``
+    and returns the multiplier for each variable.
 
-    The argument ``if_empty`` is used to set a default argument if ``log`` is
-    is given as ``None``.
+    See :meth:`_linear_combination_terms` for details.
+    """
+    return _linear_combination_terms(_split_terms(expression), variables)
 
-    The argument ``allowed_classes`` is an integer flag that determines which
-    type of variables are allowed in this log.
 
-    When a new DataLog is created by this method, the internal storage
-    uses arrays from the array module. The data type for these new arrays can
-    be specified using the ``precision`` argument.
+def _linear_combination_terms(terms, variables):
     """
-    # Typecode dependent on precision
-    typecode = 'd' if precision == myokit.DOUBLE_PRECISION else 'f'
+    Checks if a list of terms forms linear combination of the given
+    ``variables`` and returns the multiplier for each variable.
 
-    # Get all options for dimensionality
-    if dims is None:
-        dims = ()
-    ndims = len(dims)
-    if ndims == 0:
-        dcombos = ['']
-    else:
-        dcombos = ['.'.join([str(y) for y in x]) + '.' for x in _dimco(*dims)]
+    If ``expression`` is a linear combination ``a1*v1 + a2*v2 + ...`` where
+    ``vi`` is a variable in ``variables``, this method returns a list of
+    expressions ``[a1, a2, ...]``. The expressions ``ai`` are not guaranteed to
+    be constants, but won't contain any references to the variables in
+    ``variables``.
 
-    # Check given list of global variables
-    if global_vars is None:
-        global_vars = []
-    else:
-        for var in global_vars:
-            try:
-                v = model.get(var)
-            except KeyError:
-                raise ValueError(
-                    'Unknown variable specified in global_vars <'
-                    + str(var) + '>.')
-            if v.is_state():
-                raise ValueError('State cannot be global variable.')
-
-    # Function to check if variable is allowed (doesn't handle derivatives)
-    def check_if_allowed_class(var):
-        if var.is_constant():
-            raise ValueError(
-                'This log does not support constants, got <'
-                + str(var) + '>.')
-        elif var.is_state():
-            if not myokit.LOG_STATE & allowed_classes:
-                raise ValueError(
-                    'This log does not support state variables, got <'
-                    + str(var) + '>.')
-        elif var.is_bound():
-            if not myokit.LOG_BOUND & allowed_classes:
-                raise ValueError(
-                    'This log does not support bound variables, got <'
-                    + str(var) + '>.')
-        elif not myokit.LOG_INTER & allowed_classes:
-            raise ValueError(
-                'This log does not support intermediary variables, got <'
-                + str(var) + '>.')
+    If the expression cannot be written as a linear combination a
+    ``ValueError`` is raised.
+    """
+    # Multiplier for each variable
+    multipliers = [None] * len(variables)
 
-    #
-    # First option, no log argument given, use the "if_empty" option
-    #
-
-    if log is None:
-        # Check if if_empty matches allowed_classes
-        # (AKA test if ``if_empty`` is contained in ``allowed_classes``)
-        if if_empty & allowed_classes == if_empty:
-            log = if_empty
+    # Check each term multiplies one of the variables
+    for term in terms:
+        # Split into name and multiplier
+        name, multiplier = _split_factor(term, variables)
+
+        # Update the variable's multiplier
+        var = name.var()
+        i = variables.index(var)
+        if multipliers[i] is None:
+            multipliers[i] = multiplier
         else:
-            # This one's only for programmers :-)
-            raise ValueError(
-                'The option given for `if_empty` should be an allowed class.')
+            multipliers[i] = myokit.Plus(multipliers[i], multiplier)
 
-    #
-    # Second option, log given as integer flag: create a simulation log and
-    # return it.
-    #
-
-    if type(log) == int:
-
-        # Log argument given as flag
-        flag = log
-        log = myokit.DataLog()
-        if flag == myokit.LOG_ALL:
-            flag = allowed_classes
-
-        if myokit.LOG_STATE & flag:
-
-            # Check if allowed
-            if not (myokit.LOG_STATE & allowed_classes):
-                raise ValueError('This log does not support state variables.')
-
-            # Add states
-            for s in model.states():
-                name = s.qname()
-                for c in dcombos:
-                    log[c + name] = array.array(typecode)
-            flag -= myokit.LOG_STATE
-
-        if myokit.LOG_BOUND & flag:
-
-            # Check if allowed
-            if not (myokit.LOG_BOUND & allowed_classes):
-                raise ValueError('This log does not support bound variables.')
-
-            # Add bound variables
-            for label, var in model.bindings():
-                name = var.qname()
-                if name in global_vars:
-                    log[name] = array.array(typecode)
-                else:
-                    for c in dcombos:
-                        log[c + name] = array.array(typecode)
-            flag -= myokit.LOG_BOUND
+    # Return obtained multipliers
+    return multipliers
 
-        if myokit.LOG_INTER & flag:
 
-            # Check if allowed
-            if not (myokit.LOG_INTER & allowed_classes):
-                raise ValueError(
-                    'This log does not support intermediary variables.')
-
-            # Add intermediary variables
-            for var in model.variables(inter=True, deep=True):
-                name = var.qname()
-                if name in global_vars:
-                    log[name] = array.array(typecode)
-                else:
-                    for c in dcombos:
-                        log[c + name] = array.array(typecode)
-            flag -= myokit.LOG_INTER
-
-        if myokit.LOG_DERIV & flag:
-
-            # Check if allowed
-            if not (myokit.LOG_DERIV & allowed_classes):
-                raise ValueError('This log does not support time-derivatives.')
-
-            # Add state derivatives
-            for var in model.states():
-                name = var.qname()
-                for c in dcombos:
-                    log['dot(' + c + name + ')'] = array.array(typecode)
-            flag -= myokit.LOG_DERIV
-
-        if flag != 0:
-            raise ValueError('One or more unknown flags given as log.')
-
-        # Set time variable
-        time = model.time().qname()
-        if time in log:
-            log.set_time_key(time)
+def _split_factor(term, variables):
+    """
+    Splits ``term`` into two parts that can be multiplied together, so that one
+    part is a reference to a variable in ``variables``, and the other part has
+    no references to variables in ``variables``.
+
+    Returns a tuple ``(name, multiplier)`` where ``name`` is a
+    :class:`myokit.Name` referencing a variable in the list ``variables``, and
+    where ``multiplier`` is some other expression such that ``name*multiplier``
+    is equivalent to the original term.
 
-        # Return
-        return log
+    If the term can't be split this way, a ``ValueError`` is raised.
+    """
 
-    #
-    # Third option, a dict or DataLog is given. Test if it's suitable for this
-    # simulation.
-    #
-
-    if isinstance(log, dict):
-
-        # Ensure it's a DataLog
-        if not isinstance(log, myokit.DataLog):
-            log = myokit.DataLog(log)
-
-        # Set time variable
-        time = model.time().qname()
-        if time in log:
-            log.set_time_key(time)
-
-        # Ensure the log is valid
-        log.validate()
-
-        # Check dict keys
-        keys = set(log.keys())
-        if len(keys) == 0:
-            return log
-
-        for key in keys:
-            # Handle derivatives
-            deriv = key[0:4] == 'dot(' and key[-1:] == ')'
-            if deriv:
-                key = key[4:-1]
+    # Check that the term references exactly one variable from ``variables``
+    names = set([myokit.Name(var) for var in variables])
+    refs = set(term.references())
+    n_refs = len(names & refs)
+    if n_refs != 1:
+        raise ValueError(
+            'The expression `term` must reference exactly one variable from'
+            ' the list `variables` (found ' + str(n_refs) + ').')
 
-            # Split of index / name
-            kdims, kname = split_key(key)
+    # Get Name of variable referenced in this term
+    name = (names & refs).pop()
 
-            # Test name-key
-            try:
-                var = model.get(kname)
-            except KeyError:
+    # Split
+    m = None
+    positive = True
+    while term != name:
+        t = type(term)
+        if t == myokit.PrefixPlus:
+            term = term[0]
+        elif t == myokit.PrefixMinus:
+            positive = not positive
+            term = term[0]
+        elif t == myokit.Multiply:
+            a, b = term
+            if name in b.references():
+                a, b = b, a
+            term = a
+            m = b if m is None else myokit.Multiply(m, b)
+        elif t == myokit.Divide:
+            a, b = term
+            if name in b.references():
                 raise ValueError(
-                    'Unknown variable <' + str(kname) + '> in log.')
+                    'Non-linear function (division) of ' + str(name)
+                    + ' found in ' + str(term) + '.')
+            term = a
+            m = myokit.Divide(myokit.Number(1) if m is None else m, b)
+        elif t in (myokit.Plus, myokit.Minus):
+            raise ValueError(
+                'Expression passed to _split_factor must be a single term.')
+        else:
+            raise ValueError(
+                'Non-linear function of ' + str(name) + ' found in '
+                + str(term) + '.')
 
-            # Check if in class of allowed variables
-            if deriv:
-                if not myokit.LOG_DERIV & allowed_classes:
-                    raise ValueError(
-                        'This log does not support derivatives, got <'
-                        + key + '>.')
-                if not var.is_state():
-                    raise ValueError(
-                        'Cannot log time derivative of non-state <'
-                        + var.qname() + '>.')
-            else:
-                check_if_allowed_class(var)
+    # Finalize multiplier
+    if m is None:
+        m = myokit.Number(1)
+    if not positive:
+        m = myokit.PrefixMinus(m)
 
-            # Check dimensions
-            if kdims:
+    # Return
+    return name, m
 
-                # Raise error if global
-                if kname in global_vars:
-                    raise ValueError(
-                        'Cannot specify a cell index for global logging'
-                        ' variable <' + str(kname) + '>.')
-
-                # Test dim key
-                if kdims not in dcombos:
-                    raise ValueError(
-                        'Invalid index <' + str(kdims) + '> in log.')
-
-            elif dims:
-
-                # Raise error if non-global variable is used in multi-cell log
-                if kname not in global_vars:
-                    raise ValueError(
-                        'DataLog contains non-indexed entry for'
-                        ' cell-specific variable <' + str(kname) + '>.')
-
-        # Check dict values can be appended to
-        m = 'append'
-        for v in log.values():
-            if not (hasattr(v, m) and callable(getattr(v, m))):
-                raise ValueError(
-                    'Logging dict must map qnames to objects'
-                    ' that support the append() method.')
 
-        # Return
-        return log
+def _split_terms(expression, terms=None, positive=True):
+    """
+    Takes an expression tree of :class:`myokit.Plus` and/or
+    :class:`myokit.Minus` objects and splits it into terms.
 
-    #
-    # Fourth option, a sequence of variable names, either global or local.
-    #
-
-    # Check if list interface works
-    # If not, then raise exception
-    try:
-        if len(log) > 0:
-            log[0]
-    except Exception:
-        raise ValueError(
-            'Argument `log` has unexpected type. Expecting None, integer flag,'
-            ' sequence of names, dict or DataLog.')
+    Arguments:
 
-    if isinstance(log, str):
-        raise ValueError(
-            'String passed in as `log` argument, should be list'
-            ' or other sequence containing strings.')
+    ``expression``
+        The expression to split.
+    ``terms``
+        Used internally: A list of terms to append to.
+    ``positive``
+        Used internally: If false, the terms will be multiplied by -1
+        before adding.
+
+    """
+    if terms is None:
+        terms = []
+    if type(expression) == myokit.Plus:
+        a, b = expression
+        _split_terms(a, terms, positive)
+        _split_terms(b, terms, positive)
+    elif type(expression) == myokit.Minus:
+        a, b = expression
+        _split_terms(a, terms, positive)
+        _split_terms(b, terms, not positive)
+    elif type(expression) == myokit.PrefixPlus:
+        _split_terms(expression[0], terms, positive)
+    elif type(expression) == myokit.PrefixMinus:
+        _split_terms(expression[0], terms, not positive)
+    else:
+        if positive:
+            terms.append(expression)
+        else:
+            terms.append(myokit.PrefixMinus(expression))
+    return terms
 
-    # Parse log argument as list
-    lst = log
-    log = myokit.DataLog()
-    checked_knames = set()
-    for key in lst:
-
-        # Allow variable objects and LhsExpressions
-        if isinstance(key, myokit.Variable):
-            key = key.qname()
-        elif isinstance(key, myokit.LhsExpression):
-            key = str(key)
-
-        # Handle derivatives
-        deriv = key[0:4] == 'dot(' and key[-1:] == ')'
-        if deriv:
-            key = key[4:-1]
 
-        # Split off cell indexes
-        kdims, kname = split_key(key)
+def find_markov_models(model):
+    """
+    Searches a :class:`myokit.Model` for groups of states that constitute a
+    Markov model.
 
-        # Don't re-test multi-dim vars
-        if kname not in checked_knames:
+    Returns a list of lists, where the inner lists are groups of variables that
+    form a Markov model together.
 
-            # Test if name key points to valid variable
-            try:
-                var = model.get(kname)
-            except KeyError:
-                raise ValueError(
-                    'Unknown variable <' + str(kname) + '> in list.')
+    Note that this method performs a shallow check of the equation shapes,
+    and does not perform any simplification or rewriting to see if the
+    expressions can be made to fit a Markov form.
 
-            # Check if in class of allowed variables
-            if deriv:
-                if not myokit.LOG_DERIV & allowed_classes:
-                    raise ValueError(
-                        'This log does not support derivatives, got <'
-                        + key + '>.')
-
-                if not var.is_state():
-                    raise ValueError(
-                        'Cannot log time derivative of non-state <'
-                        + var.qname() + '>.')
-            else:
-                check_if_allowed_class(var)
-            checked_knames.add(kname)
+    Arguments:
 
-        # Add key to log
-        if kdims:
+    ``model``
+        The :class:`myokit.Model` to search.
 
-            # Raise error if global
-            if kname in global_vars:
-                raise ValueError(
-                    'Cannot specify a cell index for global logging variable'
-                    ' <' + str(kname) + '>.')
+    """
 
-            # Test dim key
-            if kdims not in dcombos:
-                raise ValueError(
-                    'Invalid index <' + str(kdims) + '> in list.')
+    # Models
+    models = []
+
+    # Scan model for clusters of states that depend on each other
+    seen = set()
+    for var in model.states():
+        if var in seen:
+            continue
+
+        # Get references to other states, made by this state
+        group = set(var.refs_to(True))
+
+        # Find group of connected states
+        todo = collections.deque(group)
+        while todo:
+            var = todo.popleft()
+            for ref in set(var.refs_to(True)) - group:
+                group.add(ref)
+                todo.append(ref)
+
+        # All these states now count as 'seen'
+        seen |= group
+
+        # Now check if there's a (1 - x1 - x2 - ...) variable:
+        # First check if there's a non-state variable that depends on all of
+        # these states.
+        candidates = set()
+        for var in group:
+            for ref in var.refs_by(True):
+                if set(ref.refs_to(True)) == group:
+                    candidates.add(ref)
+        candidates -= group
+
+        # Now test the candidates for the correct form
+        extra = set()
+        for candidate in candidates:
+            # Split into terms
+            terms = _split_terms(candidate.rhs())
+
+            # Find and remove the '1' term
+            i_one = None
+            for i, term in enumerate(terms):
+                if term.is_constant() and term.eval() == 1:
+                    i_one = i
+                    break
+            if i_one is None:
+                continue
+            del terms[i_one]
 
-            key = kdims + kname if not deriv else 'dot(' + kdims + kname + ')'
-            log[key] = array.array(typecode)
+            # Remaining terms must be linear combination of the states in
+            # group...
+            try:
+                factors = _linear_combination_terms(terms, list(group))
+            except ValueError:
+                continue
+
+            # And each factor must be -1
+            ok = True
+            for factor in factors:
+                if not (factor.is_constant() and factor.eval() == -1):
+                    ok = False
+                    break
+            if not ok:
+                continue
 
-        else:
+            # Passed all tests!
+            extra.add(candidate)
+        del candidates
+
+        # At this point `extra` should be empty or a single variable, if not,
+        # it's not a (normal) Markov model
+        if len(extra) > 1:
+            continue
+
+        # Must have at least 2 states in total
+        states = group | extra
+        if len(states) < 2:
+            continue
+
+        # Get sorted list of states for output
+        states = list(states)
+        states.sort(key=lambda x: myokit.tools.natural_sort_key(x.qname()))
 
-            if kname in global_vars:
-                key = kname if not deriv else 'dot(' + kname + ')'
-                log[key] = array.array(typecode)
-            else:
-                for c in dcombos:
-                    key = c + kname if not deriv else 'dot(' + c + kname + ')'
-                    log[key] = array.array(typecode)
-
-    # Set time variable
-    time = model.time().qname()
-    if time in log:
-        log.set_time_key(time)
+        # Check all members of `group` are a linear combination of states
+        try:
+            for state in group:
+                _linear_combination(state.rhs(), states)
+        except ValueError:
+            continue
 
-    # Return
-    return log
+        # This looks like a Markov model!
+        models.append(states)
+
+    return models
 
 
-def _dimco(*dims):
+def convert_markov_models_to_compact_form(model):
     """
-    Generates all the combinations of a certain set of integer dimensions. For
-    example given ``dims=(2, 3)`` it returns::
+    Scans a :class:`myokit.Model` for Markov models, and ensures they contain
+    one state that's not evaluated as an ODE, but as ``1 - sum(x[i])``, where
+    the sum is over all other states ``x[i]``.
 
-        (0, 0), (1, 0), (0, 1), (1, 1), (0, 2), (1, 2)
+    Arguments:
 
+    ``model``
+        The :class:`myokit.Model` to scan.
+
+    Returns an updated :class:`myokit.Model`.
     """
-    n = len(dims) - 1
-    """
-    def inner(dims, index, prefix):
-        if index == n:
-            for i in range(0,dims[index]):
-                yield prefix + (i,)
-        else:
-            for i in range(0,dims[index]):
-                prefix2 = prefix + (i, )
-                for y in inner(dims, index + 1, prefix2):
-                    yield y
-    return inner(dims, 0, ())
-    """
-    def inner(dims, index, postfix):
-        if index == 0:
-            for i in range(0, dims[index]):
-                yield (i,) + postfix
-        else:
-            for i in range(0, dims[index]):
-                postfix2 = (i, ) + postfix
-                for y in inner(dims, index - 1, postfix2):
-                    yield y
-    return inner(dims, n, ())
+    # Clone model
+    model = model.clone()
+
+    # Find markov models and convert
+    for states in find_markov_models(model):
+
+        # Check if a non-ODE state is already present
+        if sum([1 for x in states if not x.is_state()]):
+            continue
 
+        # Update final state
+        state = states[-1]
+        state.demote()
+        state.set_rhs('1 - ' + '-'.join([x.qname() for x in states[:-1]]))
 
-def split_key(key):
+    return model
+
+
+def convert_markov_models_to_full_ode_form(model):
     """
-    Splits a log entry name into a cell index part and a variable name part.
+    Scans a :class:`myokit.Model` for Markov models, and ensures they are
+    written in a form where every Markov state is evaluated as an ODE.
 
-    The cell index will be an empty string for 0d entries or global variables.
-    For higher dimensional cases it will be the cell index in each dimension,
-    followed by a period, for example: ``15.2.``.
+    Arguments:
 
-    The two parts returned by split_key may always be concatenated to obtain
-    the original entry.
+    ``model``
+        The :class:`myokit.Model` to scan.
+
+    Returns an updated :class:`myokit.Model`.
     """
-    m = ID_NAME_PATTERN.match(key, 0)
-    if m:
-        return key[:m.end()], key[m.end():]
-    else:
-        return '', key
+    # Clone model
+    model = model.clone()
+
+    # Find markov models and convert
+    for states in find_markov_models(model):
+
+        # Find 1-sum() state
+        special = None
+        i_special = None
+        for i, state in enumerate(states):
+            if not state.is_state():
+                special = state
+                i_special = i
+                break
+
+        # No special state: then no need to convert
+        if special is None:
+            continue
+
+        # Get initial value for special state
+        initial_value = special.eval()
+
+        # Gather terms for existing states, see which ones don't cancel out
+        sum_of_terms = [[] for _ in states]
+        for state in states:
+            if state is special:
+                continue
+
+            factors = _linear_combination(state.rhs(), states)
+            for i, factor in enumerate(factors):
+                if factor is None:
+                    continue
+
+                # Split terms in factor, add each to sum_of_terms
+                for term in _split_terms(factor):
+
+                    # Get negative term
+                    if isinstance(term, myokit.PrefixMinus):
+                        negative = term[0]
+                    else:
+                        negative = myokit.PrefixMinus(term)
+
+                    # If negative term is in list, then these cancel out and
+                    # should be removed
+                    try:
+                        sum_of_terms[i].remove(negative)
+                    except ValueError:
+                        # Negative term isn't in the list, so add this factor
+                        # to the list.
+                        sum_of_terms[i].append(term)
+
+        # Create RHS from remaining terms
+        terms = []
+        for i, sums in enumerate(sum_of_terms):
+            if not sums:
+                continue
+
+            # Combine terms
+            term = sums[0]
+            for t in sums[1:]:
+                term = myokit.Plus(term, t)
+
+            # Negate
+            if isinstance(term, myokit.PrefixMinus):
+                term = term[0]
+            else:
+                term = myokit.PrefixMinus(term)
+
+            # Multiply with state and store
+            terms.append(myokit.Multiply(term, myokit.Name(states[i])))
+
+        # Combine terms (should always be 2 or more).
+        rhs = terms[0]
+        for term in terms[1:]:
+            rhs = myokit.Plus(rhs, term)
+
+        # Update special state
+        special.promote(initial_value)
+        special.set_rhs(rhs)
+
+    # Return cloned & updated model
+    return model
+
```

### Comparing `myokit-1.35.0/myokit/_err.py` & `myokit-1.35.1/myokit/_err.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_expressions.py` & `myokit-1.35.1/myokit/_expressions.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_io.py` & `myokit-1.35.1/myokit/_io.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_model_api.py` & `myokit-1.35.1/myokit/_model_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1381,17 +1381,15 @@
 
         # Return calculated state
         return [values[state.lhs()] for state in self._state_vars]
 
     def eval_state_derivatives(
             self, state=None, inputs=None, precision=myokit.DOUBLE_PRECISION,
             ignore_errors=False):
-        """
-        Deprecated alias of :meth:`evaluate_derivatives()`.
-        """
+        """ Deprecated alias of :meth:`evaluate_derivatives()`. """
         # Deprecated since 2021-08-03
         import warnings
         warnings.warn(
             'The method `eval_state_derivatives` is deprecated. Please use'
             ' `evaluate_derivatives()` instead.')
         return self.evaluate_derivatives(
             state, inputs, precision, ignore_errors)
```

### Comparing `myokit-1.35.0/myokit/_myokit_version.py` & `myokit-1.35.1/myokit/_myokit_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Version as a tuple (major, minor, revision)
 #  - Changes to major are rare
 #  - Changes to minor indicate new features, possible slight backwards
 #    incompatibility
 #  - Changes to revision indicate bugfixes, tiny new features
 #  - There is no significance to odd/even numbers
-__version_tuple__ = 1, 35, 0
+__version_tuple__ = 1, 35, 1
 
 # String version of the version number
 __version__ = '.'.join([str(x) for x in __version_tuple__])
 if not __release__:  # pragma: no cover
     __version_tuple__ += ('dev', )
     __version__ += '.dev'
```

### Comparing `myokit-1.35.0/myokit/_parsing.py` & `myokit-1.35.1/myokit/_parsing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_progress.py` & `myokit-1.35.1/myokit/_progress.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_protocol.py` & `myokit-1.35.1/myokit/_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -742,35 +742,36 @@
     >>> p = myokit.load_protocol('example')
     >>> s = myokit.PacingSystem(p)
     >>> import numpy as np
     >>> time = np.linspace(0, 1000, 10001)
     >>> pace = np.array([s.advance(t) for t in time])
 
     """
-    def __init__(self, protocol):
-        # The current time and pacing level
-        self._time = 0
+    def __init__(self, protocol, initial_time=0):
+        # The initial and current time and pacing level
+        self._initial_time = initial_time  # Needed if we add a reset()
+        self._time = initial_time
         self._pace = 0
 
         # Currently active event
         self._fire = None
 
         # Time the currently active event is over
         self._tdown = None
 
         # The next time the pacing variable changes
-        self._tnext = 0
+        self._tnext = initial_time
 
         # Create a copy of the protocol
         self._protocol = protocol.clone()
         #TODO: For periodic events, set an _t0, and a _i, use them to calculate
         #      the next occurence
 
-        # Advance to time zero
-        self.advance(0)
+        # Advance to initial time
+        self.advance(initial_time)
 
     def advance(self, new_time):
         """
         Advances the time in the pacing system to ``new_time``.
 
         Returns the current value of the pacing variable.
         """
@@ -818,29 +819,23 @@
                 self._tnext = self._tdown
             if e and self._tnext > e._start:
                 self._tnext = e._start
 
         return self._pace
 
     def next_time(self):
-        """
-        Returns the next time the pacing system will halt at.
-        """
+        """ Returns the next time the pacing system will halt at. """
         return self._tnext
 
     def pace(self):
-        """
-        Returns the current value of the pacing variable.
-        """
+        """ Returns the current value of the pacing variable. """
         return self._pace
 
     def time(self):
-        """
-        Returns the current time in the pacing system.
-        """
+        """ Returns the current time in the pacing system. """
         return self._time
 
 
 class NotASequenceError(myokit.MyokitError):
     """ Error raised exclusively by is_sequence_exception(). """
     pass
 
@@ -859,15 +854,14 @@
     of the pacing variable will be determined by interpolating between the two
     nearest points in the series. If the simulation time is outside the bounds
     of the time-series, the first or last value in the series will be used.
 
     Protocols can be compared with ``==``, which will check if the sequence of
     time value pairs is the same, and the interpolation method is the same.
     Protocols can be serialized with ``pickle``.
-
     """
 
     def __init__(self, times, values, method=None):
         super().__init__()
 
         if len(times) != len(values):
             raise ValueError('Times and values array must have same size.')
@@ -905,38 +899,30 @@
 
     def __setstate__(self, values):
         self._times = values['times']
         self._values = values['values']
         self._method = values['method']
 
     def clone(self):
-        """
-        Returns a clone of this protocol.
-        """
+        """ Returns a clone of this protocol. """
         return TimeSeriesProtocol(self._times, self._values, self._method)
 
     def pace(self, t):
-        """
-        Returns the value of the pacing variable at time ``t``.
-        """
+        """ Returns the value of the pacing variable at time ``t``. """
         if t < self._times[0]:
             return self._values[0]
         if t > self._times[-1]:
             return self._values[-1]
         i = bisect_right(self._times, t) - 1
         if i == len(self._times) - 1:
             return self._values[i]
         return self._values[i] + (t - self._times[i]) * (
             self._values[i + 1] - self._values[i]
         ) / (self._times[i + 1] - self._times[i])
 
     def times(self):
-        """
-        Returns a list of the times in this protocol.
-        """
+        """ Returns a list of the times in this protocol. """
         return self._times
 
     def values(self):
-        """
-        Returns a list of the values in this protocol.
-        """
+        """ Returns a list of the values in this protocol. """
         return self._values
```

### Comparing `myokit-1.35.0/myokit/_sim/__init__.py` & `myokit-1.35.1/myokit/_sim/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/cable.c` & `myokit-1.35.1/myokit/_sim/cable.c`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
     /* Check if log contained extra variables */
     if (ivars != nvars) {
         PyErr_SetString(PyExc_Exception, "Unknown variables found in logging dictionary.");
         return sim_clean();
     }
 
     /* Set up pacing */
-    pacing = ESys_Create(&flag_pacing);
+    pacing = ESys_Create(tmin, &flag_pacing);
     if (flag_pacing!=ESys_OK) { ESys_SetPyErr(flag_pacing); return sim_clean(); }
     flag_pacing = ESys_Populate(pacing, protocol);
     if (flag_pacing!=ESys_OK) { ESys_SetPyErr(flag_pacing); return sim_clean(); }
     flag_pacing = ESys_AdvanceTime(pacing, tmin);
     if (flag_pacing!=ESys_OK) { ESys_SetPyErr(flag_pacing); return sim_clean(); }
     tpace = ESys_GetNextTime(pacing, &flag_pacing);
     engine_pace = ESys_GetLevel(pacing, &flag_pacing);
```

### Comparing `myokit-1.35.0/myokit/_sim/cable.py` & `myokit-1.35.1/myokit/_sim/cable.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,20 @@
         gating variables (default=False).
 
     This simulation provides the following inputs variables can bind to:
 
     ``time``
         The simulation time
     ``pace``
-        The pacing level, this is set if a protocol was passed in.
+        The pacing level, this is set if a protocol was passed in. Will be set
+        to 0 if no protocol is provided.
     ``diffusion_current``
         The current flowing from the cell to its neighbors. This will be
         positive when the cell is acting as a source, negative when it is
-        acting as a sink.
+        acting as a sink. Will be set to 0 if no connections are made.
 
     The variable ``time`` is set globally, meaning each cell uses the same
     value. The variables ``pace`` and ``diffusion_current`` have different
     values per cell. The number of paced cell can be set with
     :meth:`set_paced_cells`.
 
     A single labeled variable is required for this simulation to work:
```

### Comparing `myokit-1.35.0/myokit/_sim/cmodel.h` & `myokit-1.35.1/myokit/_sim/cmodel.h`

 * *Files 0% similar despite different names*

```diff
@@ -478,14 +478,15 @@
     if (model->pace_values == NULL) {
         return Model_OUT_OF_MEMORY;
     }
 
     /* Clear values */
     for (int i = 0; i < n_pace; i++) {
         model->pace_values[i] = 0;
+        /* Note: This will be overruled by the first call to SetBoundVariables */
     }
 
     return Model_OK;
 }
 
 /*
  * (Re)calculates the values of all constants that are derived from other
```

### Comparing `myokit-1.35.0/myokit/_sim/cmodel.py` & `myokit-1.35.1/myokit/_sim/cmodel.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/compiler.c` & `myokit-1.35.1/myokit/_sim/compiler.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/compiler.py` & `myokit-1.35.1/myokit/_sim/compiler.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/cvodessim.c` & `myokit-1.35.1/myokit/_sim/cvodessim.c`

 * *Files 2% similar despite different names*

```diff
@@ -188,23 +188,15 @@
  * Model
  */
 Model model;        /* A model object */
 
 /*
  * Pacing
  */
-union PSys {
-    ESys event;
-    FSys fixed;
-};
-enum PSysType {
-    EVENT,
-    FIXED
-};
-union PSys *pacing_systems;   /* Array of pacing system (event or fixed) */
+union PSys *pacing_systems;   /* Array of pacing systems (event based or time series) */
 enum PSysType *pacing_types;  /* Array of pacing system types */
 PyObject *protocols;          /* The protocols used to generate the pacing systems */
 double* pacing;               /* Pacing values, same size as pacing_systems and pacing_types */
 int n_pace;                   /* The number of pacing systems */
 
 /*
  * CVODE Memory
@@ -347,24 +339,24 @@
  *  N_Vector ydot   Space to store the calculated derivatives in
  *  void* user_data Extra data (contains the sensitivity parameter values)
  *
  */
 int
 rhs(realtype t, N_Vector y, N_Vector ydot, void *user_data)
 {
-    FSys_Flag flag_fpacing;
+    TSys_Flag flag_fpacing;
     UserData fdata;
     int i;
 
-    /* Fixed-form pacing? Then look-up correct value of pacing variable */
+    /* Time-series pacing? Then look-up correct value of pacing variable */
     for (int i = 0; i < n_pace; i++) {
-        if (pacing_types[i] == FIXED) {
-            pacing[i] = FSys_GetLevel(pacing_systems[i].fixed, t, &flag_fpacing);
-            if (flag_fpacing != FSys_OK) { /* This should never happen */
-                FSys_SetPyErr(flag_fpacing);
+        if (pacing_types[i] == TSys_TYPE) {
+            pacing[i] = TSys_GetLevel(pacing_systems[i].tsys, t, &flag_fpacing);
+            if (flag_fpacing != TSys_OK) { /* This should never happen */
+                TSys_SetPyErr(flag_fpacing);
                 return -1;  /* Negative value signals irrecoverable error to CVODE */
             }
         }
     }
 
     /* Update model state */
 
@@ -437,55 +429,74 @@
         #ifdef MYOKIT_DEBUG_PROFILING
         benchmarker_print("CP Entered sim_clean.");
         #elif defined MYOKIT_DEBUG_MESSAGES
         printf("CM Cleaning up.\n");
         #endif
 
         /* CVode arrays */
+        #ifdef MYOKIT_DEBUG_MESSAGES
+        printf("CM ..Sundials vectors.\n");
+        #endif
         if (y != NULL) { N_VDestroy_Serial(y); y = NULL; }
         if (ylast != NULL) { N_VDestroy_Serial(ylast); ylast = NULL; }
         if (sy != NULL) { N_VDestroyVectorArray(sy, model->ns_independents); sy = NULL; }
         if (model != NULL && model->is_ode && !dynamic_logging) {
             if (z != NULL) { N_VDestroy_Serial(z); z = NULL; }
             if (sz != NULL) { N_VDestroyVectorArray(sz, model->ns_independents); sz = NULL; }
         }
 
         /* Root finding results */
+        #ifdef MYOKIT_DEBUG_MESSAGES
+        printf("CM ..Root-finding results.\n");
+        #endif
         free(rf_direction); rf_direction = NULL;
 
         /* Sundials objects */
+        #ifdef MYOKIT_DEBUG_MESSAGES
+        printf("CM ..Sundials objects.\n");
+        #endif
         CVodeFree(&cvode_mem); cvode_mem = NULL;
         #if SUNDIALS_VERSION_MAJOR >= 3
         SUNLinSolFree(sundense_solver); sundense_solver = NULL;
         SUNMatDestroy(sundense_matrix); sundense_matrix = NULL;
         #endif
         #if SUNDIALS_VERSION_MAJOR >= 6
         SUNContext_Free(&sundials_context); sundials_context = NULL;
         #endif
 
         /* User data and parameter scale array*/
+        #ifdef MYOKIT_DEBUG_MESSAGES
+        printf("CM ..Sundials user-data.\n");
+        #endif
         free(pbar);
         if (udata != NULL) {
             free(udata->p);
             free(udata); udata = NULL;
         }
 
         /* Pacing systems */
+        #ifdef MYOKIT_DEBUG_MESSAGES
+        printf("CM ..Pacing systems.\n");
+        #endif
         for (int i = 0; i < n_pace; i++) {
-            if (pacing_types[i] == FIXED) {
-                FSys_Destroy(pacing_systems[i].fixed);
-            } else if (pacing_types[i] == EVENT) {
-                ESys_Destroy(pacing_systems[i].event);
+            // Note: Type is ESys, TSys, or not set!
+            if (pacing_types[i] == ESys_TYPE) {
+                ESys_Destroy(pacing_systems[i].esys);
+            } else if (pacing_types[i] == TSys_TYPE) {
+                TSys_Destroy(pacing_systems[i].tsys);
             }
         }
         free(pacing_systems); pacing_systems = NULL;
         free(pacing_types); pacing_types = NULL;
         free(pacing); pacing = NULL;
 
         /* CModel */
+        #ifdef MYOKIT_DEBUG_MESSAGES
+        printf("CM ..CModel.\n");
+        #endif
         Model_Destroy(model); model = NULL;
 
         /* Benchmarking and profiling */
         #ifdef MYOKIT_DEBUG_PROFILING
         benchmarker_print("CP Completed sim_clean.");
         Py_XDECREF(benchmarker_print_str); benchmarker_print_str = NULL;
         #endif
@@ -504,14 +515,18 @@
 
 /*
  * Version of sim_clean that sets a python exception.
  */
 PyObject*
 sim_cleanx(PyObject* ex_type, const char* msg, ...)
 {
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("CM Entering sim_cleanx.\n");
+    #endif
+
     va_list argptr;
     char errstr[1024];
 
     va_start(argptr, msg);
     vsprintf(errstr, msg, argptr);
     va_end(argptr);
 
@@ -540,19 +555,19 @@
     printf("CM Entering sim_init.\n");
     #endif
 
     /* Error checking flags */
     int flag_cvode;
     Model_Flag flag_model;
     ESys_Flag flag_epacing;
-    FSys_Flag flag_fpacing;
+    TSys_Flag flag_fpacing;
 
     /* Pacing systems */
     ESys epacing;
-    FSys fpacing;
+    TSys fpacing;
 
     /* General purpose ints for iterating */
     int i, j;
 
     /* Log the first point? Only happens if not continuing from a log */
     int log_first_point;
 
@@ -614,15 +629,15 @@
             &tmin,              /*  0. Float: initial time */
             &tmax,              /*  1. Float: final time */
             &state_py,          /*  2. List: initial and final state */
             &s_state_py,        /*  3. List of lists: state sensitivities */
             &bound_py,          /*  4. List: store final bound variables here */
             &literals,          /*  5. List: literal constant values */
             &parameters,        /*  6. List: parameter values */
-            &protocols,         /*   7. Event-based or fixed protocols */
+            &protocols,         /*  7. Event-based or time series protocols */
             &log_dict,          /*  8. DataLog */
             &log_interval,      /*  9. Float: log interval, or 0 */
             &log_times,         /* 10. List of logging times, or None */
             &sens_list,         /* 11. List to store sensitivities in */
             &rf_index,          /* 12. Int: root-finding state variable */
             &rf_threshold,      /* 13. Float: root-finding threshold */
             &rf_list,           /* 14. List to store roots in or None */
@@ -951,14 +966,17 @@
     }
 
     /*
      * Set up pacing systems
      */
     n_pace = 0;
     if (protocols != Py_None) {
+        #ifdef MYOKIT_DEBUG_MESSAGES
+        printf("CM Initialising pacing systems\n");
+        #endif
         if (!PyList_Check(protocols)) {
             return sim_cleanx(PyExc_TypeError, "'protocols' must be a list.");
         }
         n_pace = (int)PyList_Size(protocols);
     }
     pacing_systems = (union PSys*)malloc((size_t)n_pace * sizeof(union PSys));
     if (pacing_systems == NULL) {
@@ -976,51 +994,69 @@
 
     /*
      *  Unless set by pacing, tnext is set to tmax
      */
     tnext = tmax;
 
     /*
-     * Set up event-based and/or fixed pacing.
+     * Set up event-based and/or time-series pacing.
      */
     if (protocols != Py_None) {
         for (int i = 0; i < PyList_Size(protocols); i++) {
             PyObject *protocol = PyList_GetItem(protocols, i);
             const char* protocol_type_name = Py_TYPE(protocol)->tp_name;
             if (strcmp(protocol_type_name, "Protocol") == 0) {
-                pacing_systems[i].event = ESys_Create(&flag_epacing);
-                pacing_types[i] = EVENT;
-                epacing = pacing_systems[i].event;
+
+                epacing = ESys_Create(tmin, &flag_epacing);
                 if (flag_epacing != ESys_OK) { ESys_SetPyErr(flag_epacing); return sim_clean(); }
+                pacing_systems[i].esys = epacing;
+                pacing_types[i] = ESys_TYPE;
+
                 flag_epacing = ESys_Populate(epacing, protocol);
                 if (flag_epacing != ESys_OK) { ESys_SetPyErr(flag_epacing); return sim_clean(); }
+
                 flag_epacing = ESys_AdvanceTime(epacing, tmin);
                 if (flag_epacing != ESys_OK) { ESys_SetPyErr(flag_epacing); return sim_clean(); }
+
                 t_proposed = ESys_GetNextTime(epacing, &flag_epacing);
                 pacing[i] = ESys_GetLevel(epacing, &flag_epacing);
                 tnext = fmin(t_proposed, tnext);
 
-                #ifdef MYOKIT_DEBUG_PROFILING
+                #if defined(MYOKIT_DEBUG_PROFILING)
                 benchmarker_print("CP Created event-based pacing system.");
+                #elif defined(MYOKIT_DEBUG_MESSAGES)
+                printf("CM Created an event-based pacing system\n");
                 #endif
-            } else if (strcmp(protocol_type_name, "TimeSeriesProtocol") == 0) {
-                pacing_systems[i].fixed = FSys_Create(&flag_fpacing);
-                pacing_types[i] = FIXED;
-                fpacing = pacing_systems[i].fixed;
-                if (flag_fpacing != FSys_OK) { FSys_SetPyErr(flag_fpacing); return sim_clean(); }
-                flag_fpacing = FSys_Populate(fpacing, protocol);
-                if (flag_fpacing != FSys_OK) { FSys_SetPyErr(flag_fpacing); return sim_clean(); }
 
+            } else if (strcmp(protocol_type_name, "TimeSeriesProtocol") == 0) {
 
-                #ifdef MYOKIT_DEBUG_PROFILING
-                benchmarker_print("CP Created fixed-form pacing system.");
+                fpacing = TSys_Create(&flag_fpacing);
+                pacing_systems[i].tsys = fpacing;
+                pacing_types[i] = TSys_TYPE;
+
+                if (flag_fpacing != TSys_OK) { TSys_SetPyErr(flag_fpacing); return sim_clean(); }
+                flag_fpacing = TSys_Populate(fpacing, protocol);
+                if (flag_fpacing != TSys_OK) { TSys_SetPyErr(flag_fpacing); return sim_clean(); }
+                pacing[i] = 0;
+
+                #if defined(MYOKIT_DEBUG_PROFILING)
+                benchmarker_print("CP Created time-series pacing system.");
+                #elif defined(MYOKIT_DEBUG_MESSAGES)
+                printf("CM Added a time-series pacing system\n");
                 #endif
+
             } else {
-                printf("protocol_type_name: %s", protocol_type_name);
-                return sim_cleanx(PyExc_TypeError, "Item %d in 'protocols' is not a myokit.Protocol or myokit.TimeSeriesProtocol object.", i);
+
+                /* Pacing label defined but no protocol set. Usually happens through set_protocol(None). */
+                #if defined(MYOKIT_DEBUG_MESSAGES)
+                printf("CM Unsetting previously set protocol\n");
+                #endif
+
+                pacing_types[i] = PSys_NOT_SET;
+                pacing[i] = 0;  /* See #320 and technical note on pacing */
             }
         }
     }
 
     /*
      * Create solver
      */
@@ -1280,14 +1316,17 @@
     /* Error flags */
     Model_Flag flag_model;
     ESys_Flag flag_epacing;
     int flag_cvode;         /* CVode flag */
     int flag_root;          /* Root finding flag */
     int flag_reinit = 0;    /* Set if CVODE needs to be reset during a simulation step */
 
+    /* Pacing */
+    ESys epacing;
+
     /* Multi-purpose ints for iterating */
     int i, j;
 
     /* Number of integration steps taken in this call */
     int steps_taken = 0;
 
     /* Proposed next logging or pacing point */
@@ -1517,20 +1556,18 @@
              * Event-based pacing
              *
              * At this point we have logged everything _before_ time t, so it
              * is safe to update the pacing mechanism to time t.
              */
             tnext = tmax;
             for (int i = 0; i < n_pace; i++) {
-                if (pacing_types[i] == EVENT) {
-                    ESys epacing = pacing_systems[i].event;
+                if (pacing_types[i] == ESys_TYPE) {
+                    epacing = pacing_systems[i].esys;
                     flag_epacing = ESys_AdvanceTime(epacing, t);
-                    if (flag_epacing != ESys_OK) {
-                        ESys_SetPyErr(flag_epacing); return sim_clean();
-                    }
+                    if (flag_epacing != ESys_OK) { ESys_SetPyErr(flag_epacing); return sim_clean(); }
                     t_proposed = ESys_GetNextTime(epacing, NULL);
                     tnext = fmin(tnext, t_proposed);
                     pacing[i] = ESys_GetLevel(epacing, NULL);
                 }
             }
 
             /* Dynamic logging: Log every visited point */
```

### Comparing `myokit-1.35.0/myokit/_sim/cvodessim.py` & `myokit-1.35.1/myokit/_sim/cvodessim.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,27 @@
         This input provides the number of rhs evaluations used at each point in
         time and can be used to gain some insight into the solver's behavior.
     ``realtime``
         This input provides the elapsed system time at each logged point.
 
     No variable labels are required for this simulation type.
 
+    **Multiple protocols or no protocol**
+
+    This simulation supports pacing with more than one protocol. To this end,
+    pass in a dictionary mapping pacing labels (bindings) to :class:`Protocol`
+    or :class:`TimeSeriesProtocol` objects, e.g.
+    ``protocol={'pace_1': protocol_1, 'pace_2': protocol_2}``.
+
+    For backwards compatibility, if no protocol is set and ``protocol=None``,
+    then the pacing label ``pace`` is still registered (allowing later calls to
+    add a protocol with ``set_protocol``. Alternatively, if ``protocol={}``
+    then no pacing labels will be registered, and any subsequent calls to
+    ``set_protocol`` will fail.
+
     **Storing and loading simulation objects**
 
     There are two ways to store Simulation objects to the file system: 1.
     using serialisation (the ``pickle`` module), and 2. using the ``path``
     constructor argument.
 
     Each time a simulation is created, a C module is compiled, imported, and
@@ -159,19 +172,21 @@
 
         # Set protocol
         self._protocols = []
         self._pacing_labels = []
         if isinstance(protocol, (myokit.Protocol, myokit.TimeSeriesProtocol)):
             protocol = {'pace': protocol}
         elif protocol is None:
-            # TODO: This can be an empty dict once #320 is resolved
+            # For backwards compatibility, we still register 'pace'. This
+            # means users can call `set_protocol` at a later time to set a
+            # protocol.
             protocol = {'pace': None}
         for label, protocol in protocol.items():
+            self._protocols.append(None)
             self._pacing_labels.append(label)
-            self._protocols.append(myokit.Protocol())
             self.set_protocol(protocol, label)
 
         # Generate C Model code, get sensitivity and constants info
         cmodel = myokit.CModel(self._model, self._pacing_labels, sensitivities)
         if cmodel.has_sensitivities:
             self._sensitivities = (cmodel.dependents, cmodel.independents)
 
@@ -1004,33 +1019,30 @@
         if values is None:
             raise ValueError('No values given.')
 
         self.set_protocol(myokit.TimeSeriesProtocol(times, values))
 
     def set_protocol(self, protocol, label='pace'):
         """
-        Set an event-based pacing :class:`Protocol` or a :class:`FixedProtocol`
-        for the given ``label``.
+        Set an event-based pacing :class:`Protocol` or a
+        :class:`TimeSeriesProtocol` for the given ``label``.
 
         To remove a previously set binding call this method with ``protocol =
         None``. In this case, the value of any variables bound to ``label``
         will be set to 0.
 
         The label must be one of the pacing labels set in the constructor.
         """
         try:
             index = self._pacing_labels.index(label)
         except ValueError:
             raise ValueError('Unknown pacing label: ' + str(label))
 
         # Set new protocol
-        if protocol is None:
-            self._protocols[index] = myokit.Protocol()
-        else:
-            self._protocols[index] = protocol.clone()
+        self._protocols[index] = None if protocol is None else protocol.clone()
 
     def __setstate__(self, state):
         """
         Called after unpickling, to set any variables not set by the
         constructor.
 
         See: https://docs.python.org/3/library/pickle.html#object.__setstate__
```

### Comparing `myokit-1.35.0/myokit/_sim/differential.hpp` & `myokit-1.35.1/myokit/_sim/differential.hpp`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/fiber_tissue.c` & `myokit-1.35.1/myokit/_sim/fiber_tissue.c`

 * *Files 0% similar despite different names*

```diff
@@ -496,15 +496,15 @@
     #ifdef MYOKIT_DEBUG_MESSAGES
     printf("Checked input and output states.\n");
     #endif
 
     //
     // Set up pacing system
     //
-    pacing = ESys_Create(&flag_pacing);
+    pacing = ESys_Create(tmin, &flag_pacing);
     if(flag_pacing!=ESys_OK) { ESys_SetPyErr(flag_pacing); return sim_clean(); }
     flag_pacing = ESys_Populate(pacing, protocol);
     if(flag_pacing!=ESys_OK) { ESys_SetPyErr(flag_pacing); return sim_clean(); }
     flag_pacing = ESys_AdvanceTime(pacing, tmin);
     if(flag_pacing!=ESys_OK) { ESys_SetPyErr(flag_pacing); return sim_clean(); }
     tnext_pace = ESys_GetNextTime(pacing, NULL);
     engine_pace = ESys_GetLevel(pacing, NULL);
```

### Comparing `myokit-1.35.0/myokit/_sim/fiber_tissue.py` & `myokit-1.35.1/myokit/_sim/fiber_tissue.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,19 +52,20 @@
         faster (but possibly less accurately) by setting ``native_maths=True``.
 
     The simulation provides the following inputs variables can bind to:
 
     ``time`` (global)
         The simulation time
     ``pace`` (per-cell)
-        The pacing level, this is set if a protocol was passed in.
+        The pacing level, this is set if a protocol was passed in. Will be set
+        to 0 if no protocol is provided.
     ``diffusion_current`` (per-cell)
         The current flowing from the cell to its neighbors. This will be
         positive when the cell is acting as a source, negative when it is
-        acting as a sink.
+        acting as a sink. Will be set to 0 if no connections are made.
 
     The variable ``time`` is set globally, meaning each cell uses the same
     value. The variables ``pace`` and ``diffusion_current`` have different
     values per cell.
 
     The following labeled variables are required for this simulation to work:
```

### Comparing `myokit-1.35.0/myokit/_sim/jacobian.cpp` & `myokit-1.35.1/myokit/_sim/jacobian.cpp`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/jacobian.py` & `myokit-1.35.1/myokit/_sim/jacobian.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/mcl.h` & `myokit-1.35.1/myokit/_sim/mcl.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/opencl.c` & `myokit-1.35.1/myokit/_sim/opencl.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/opencl.py` & `myokit-1.35.1/myokit/_sim/opencl.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/openclsim.c` & `myokit-1.35.1/myokit/_sim/openclsim.c`

 * *Files 0% similar despite different names*

```diff
@@ -481,15 +481,15 @@
         PyErr_SetString(PyExc_Exception, "Connections and conductance fields cannot be used together.");
         return sim_clean();
     }
 
     //
     // Set up pacing system
     //
-    pacing = ESys_Create(&flag_pacing);
+    pacing = ESys_Create(tmin, &flag_pacing);
     if(flag_pacing != ESys_OK) { ESys_SetPyErr(flag_pacing); return sim_clean(); }
     flag_pacing = ESys_Populate(pacing, protocol);
     if(flag_pacing != ESys_OK) { ESys_SetPyErr(flag_pacing); return sim_clean(); }
     flag_pacing = ESys_AdvanceTime(pacing, tmin);
     if(flag_pacing != ESys_OK) { ESys_SetPyErr(flag_pacing); return sim_clean(); }
     tnext_pace = ESys_GetNextTime(pacing, NULL);
     engine_pace = ESys_GetLevel(pacing, NULL);
```

### Comparing `myokit-1.35.0/myokit/_sim/openclsim.cl` & `myokit-1.35.1/myokit/_sim/openclsim.cl`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/openclsim.py` & `myokit-1.35.1/myokit/_sim/openclsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,16 @@
         gating variables (default=``False``).
 
     The simulation provides the following inputs variables can bind to:
 
     ``time``
         The simulation time
     ``pace``
-        The pacing level, this is set if a protocol was passed in.
+        The pacing level, this is set if a protocol was passed in. Will be set
+        to 0 if no protocol is provided.
     ``diffusion_current`` (if enabled)
         The current flowing from the cell to its neighbors. This will be
         positive when the cell is acting as a source, negative when it is
         acting as a sink.
 
     The input ``time`` is set globally: Any variable bound to ``time`` will
     appear in the logs as single, global variable (for example ``engine.time``
@@ -776,32 +777,32 @@
         area is defined as::
 
             i_diff = -(1 / chi) (k / (k + 1)) ∇ * (D∇V)
 
         (see the argument list below for the meaning of the variables).
 
         This can be equated to Myokit's diffusion current, but only if we
-        assume **zero-flux boundary conditions**, a **regularly spaced grid**,
-        and **no spatial heterogeneity in D** (or g).
+        assume *zero-flux boundary conditions*, a *regularly spaced grid*,
+        and *no spatial heterogeneity in D* (or g).
 
         With these assumptions, we can use finite differences to find::
 
             g_bar = (1 / chi) * (k / (k + 1)) * D * (1 / dx^2)
 
         where ``g_bar`` is the cell-to-cell conductance, but normalized with
         respect to unit membrane area.
         For models with currents normalized to area this is unproblematic, but
         to convert to models with unnormalized currents this means we have
-        added the further assumption that **each node contains some fixed
-        amount of membrane**, determined by an area A::
+        added the further assumption that *each node contains some fixed
+        amount of membrane*, determined by an area A::
 
             g = (1 / chi) * (k / (k + 1)) * D * (1 / dx^2) * A
 
         This equation can also be applied in two dimensions, but only if
-        **we assume that the conductivity matrix is diagonal**, in which case::
+        *we assume that the conductivity matrix is diagonal*, in which case::
 
             gx = (1 / chi) * (k / (k + 1)) * Dx * (1 / dx^2) * A
             gy = (1 / chi) * (k / (k + 1)) * Dy * (1 / dy^2) * A
 
         This method uses the above equation to calculate and return a
         conductance value from the parameters used in monodomain simulations.
 
@@ -1704,19 +1705,15 @@
         """
         step_size = float(step_size)
         if step_size <= 0:
             raise ValueError('Step size must be greater than zero.')
         self._step_size = step_size
 
     def set_time(self, time=0):
-        """
-        Sets the current simulation time.
-        """
-        if time < 0:
-            raise ValueError('Simulation time cannot be negative')
+        """ Sets the current simulation time. """
         self._time = float(time)
 
     def shape(self):
         """
         Returns the shape of this simulation's grid of cells as a tuple
         ``(ny, nx)`` for 2d simulations, or a single value ``nx`` for 1d
         simulations.
```

### Comparing `myokit-1.35.0/myokit/_sim/pacing.h` & `myokit-1.35.1/myokit/_sim/pacing.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 /*
  * pacing.h
  *
- * Ansi-C implementation for event-based pacing (using a Myokit Protocol
- * object) and fixed-form pacing (using a time-series).
+ * Ansi-C implementation for event-based pacing (using a myokit.Protocol) and
+ * time series pacing (using a myokit.TimeSeriesProtocol).
  *
  * How to use event-based pacing:
  *
  *  1. Create a pacing system using ESys_Create
  *  2. Populate it with events using ESys_Populate
  *  3. Set the time in the pacing system with ESys_AdvanceTime.
  *  4. Get the time of the first event with ESys_GetNextTime
@@ -18,21 +18,20 @@
  *  7. Tidy up using ESys_Destroy
  *
  * Events must always start at t>=0, negative times are not supported.
  *
  * Flags are used to indicate errors. If a flag other than ESys_OK is set, a
  * call to ESys_SetPyErr(flag) can be made to set a Python exception.
  *
+ * How to use time series pacing:
  *
- * How to use fixed-form pacing:
- *
- *  1. Create a pacing system using FSys_Create
- *  2. Populate it using two Python lists via FSys_Populate
- *  3. Obtain the pacing value for any time using FSys_GetLevel
- *  4. Tidy up using FSys_Destroy
+ *  1. Create a pacing system using TSys_Create
+ *  2. Populate it using two Python lists via TSys_Populate
+ *  3. Obtain the pacing value for any time using TSys_GetLevel
+ *  4. Tidy up using TSys_Destroy
  *
  * This file is part of Myokit.
  * See http://myokit.org for copyright, sharing, and licensing details.
  *
  */
 #ifndef MyokitPacing
 #define MyokitPacing
@@ -213,19 +212,20 @@
     return head;
 }
 
 /*
  * Pacing system
  */
 struct ESys_Mem {
-    Py_ssize_t n_events;   // The number of events in this system
-    double time;    // The current time
-    ESys_Event events;   // The events, stored as an array
-    ESys_Event head;     // The head of the event queue
-    ESys_Event fire;     // The currently active event
+    Py_ssize_t n_events;    // The number of events in this system
+    double time;            // The current time
+    double initial_time;    // The initial time (used by reset)
+    ESys_Event events;      // The events, stored as an array
+    ESys_Event head;        // The head of the event queue
+    ESys_Event fire;        // The currently active event
     double tnext;   // The time of the next event start or finish
     double tdown;   // The time the active event is over
     double level;   // The current output value
 };
 typedef struct ESys_Mem* ESys;
 
 /*
@@ -233,29 +233,30 @@
  *
  * Arguments
  *  flag : The address of an event-based pacing error flag or NULL
  *
  * Returns the newly created pacing system
  */
 ESys
-ESys_Create(ESys_Flag* flag)
+ESys_Create(double initial_time, ESys_Flag* flag)
 {
     ESys sys = (ESys)malloc(sizeof(struct ESys_Mem));
     if (sys == 0) {
         if(flag != 0) *flag = ESys_OUT_OF_MEMORY;
         return 0;
     }
 
-    sys->time = 0;
+    sys->time = initial_time;
+    sys->initial_time = initial_time;
     sys->n_events = -1; // Used to indicate unpopulated system
     sys->events = NULL;
     sys->head = NULL;
     sys->fire = NULL;
-    sys->tnext = 0;
-    sys->tdown = 0;
+    sys->tnext = initial_time;
+    sys->tdown = initial_time;
     sys->level = 0;
 
     if(flag != 0) *flag = ESys_OK;
     return sys;
 }
 
 /*
@@ -311,19 +312,19 @@
     next = head + 1;
     for(i=1; i<sys->n_events; i++) {
         head = ESys_ScheduleEvent(head, next++, &flag);
         if (flag != ESys_OK) { return flag; }
     }
 
     // Reset the properties of the event system
-    sys->time = 0;
+    sys->time = sys->initial_time;
     sys->head = head;
     sys->fire = 0;
-    sys->tnext = 0;
-    sys->tdown = 0;
+    sys->tnext = sys->initial_time;
+    sys->tdown = sys->initial_time;
     sys->level = 0;
 
     return ESys_OK;
 }
 
 /*
  * Populates an event system using the events from a myokit.Protocol
@@ -592,237 +593,237 @@
     }
     if(flag != 0) *flag = ESys_OK;
     return sys->level;
 }
 
 /*
  *
- * Fixed-form code starts here
+ * Time-series code starts here
  *
  */
 
 /*
- * Fixed-form pacing error flags
+ * Time series pacing error flags
  */
-typedef int FSys_Flag;
-#define FSys_OK                             0
-#define FSys_OUT_OF_MEMORY                  -1
+typedef int TSys_Flag;
+#define TSys_OK                             0
+#define TSys_OUT_OF_MEMORY                  -1
 // General
-#define FSys_INVALID_SYSTEM                 -10
-#define FSys_POPULATED_SYSTEM               -11
-#define FSys_UNPOPULATED_SYSTEM             -12
+#define TSys_INVALID_SYSTEM                 -10
+#define TSys_POPULATED_SYSTEM               -11
+#define TSys_UNPOPULATED_SYSTEM             -12
 // Populating the system
-#define FSys_POPULATE_INVALID_TIMES         -20
-#define FSys_POPULATE_INVALID_VALUES        -21
-#define FSys_POPULATE_SIZE_MISMATCH         -22
-#define FSys_POPULATE_NOT_ENOUGH_DATA       -23
-#define FSys_POPULATE_INVALID_TIMES_DATA    -24
-#define FSys_POPULATE_INVALID_VALUES_DATA   -25
-#define FSys_POPULATE_DECREASING_TIMES_DATA -26
-#define FSys_POPULATE_INVALID_PROTOCOL      -27
+#define TSys_POPULATE_INVALID_TIMES         -20
+#define TSys_POPULATE_INVALID_VALUES        -21
+#define TSys_POPULATE_SIZE_MISMATCH         -22
+#define TSys_POPULATE_NOT_ENOUGH_DATA       -23
+#define TSys_POPULATE_INVALID_TIMES_DATA    -24
+#define TSys_POPULATE_INVALID_VALUES_DATA   -25
+#define TSys_POPULATE_DECREASING_TIMES_DATA -26
+#define TSys_POPULATE_INVALID_PROTOCOL      -27
 
 /*
- * Sets a python exception based on a fixed-form pacing error flag.
+ * Sets a python exception based on a time-series pacing error flag.
  *
  * Arguments
  *  flag : The python error flag to base the message on.
  */
 void
-FSys_SetPyErr(FSys_Flag flag)
+TSys_SetPyErr(TSys_Flag flag)
 {
     switch(flag) {
-    case FSys_OK:
+    case TSys_OK:
         break;
-    case FSys_OUT_OF_MEMORY:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Memory allocation failed.");
+    case TSys_OUT_OF_MEMORY:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Memory allocation failed.");
         break;
     // General
-    case FSys_INVALID_SYSTEM:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Invalid pacing system provided.");
+    case TSys_INVALID_SYSTEM:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Invalid pacing system provided.");
         break;
-    case FSys_POPULATED_SYSTEM:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Pacing system already populated.");
+    case TSys_POPULATED_SYSTEM:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Pacing system already populated.");
         break;
-    case FSys_UNPOPULATED_SYSTEM:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Pacing system not populated.");
+    case TSys_UNPOPULATED_SYSTEM:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Pacing system not populated.");
         break;
     // Populate
-    case FSys_POPULATE_INVALID_PROTOCOL:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Invalid protocol python object passed.");
+    case TSys_POPULATE_INVALID_PROTOCOL:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Invalid protocol python object passed.");
         break;
-    case FSys_POPULATE_INVALID_TIMES:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Invalid times array passed.");
+    case TSys_POPULATE_INVALID_TIMES:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Invalid times array passed.");
         break;
-    case FSys_POPULATE_INVALID_VALUES:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Invalid values array passed.");
+    case TSys_POPULATE_INVALID_VALUES:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Invalid values array passed.");
         break;
-    case FSys_POPULATE_SIZE_MISMATCH:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Sizes of times and values arrays don't match.");
+    case TSys_POPULATE_SIZE_MISMATCH:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Sizes of times and values arrays don't match.");
         break;
-    case FSys_POPULATE_NOT_ENOUGH_DATA:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Time-series must contain at least two data points.");
+    case TSys_POPULATE_NOT_ENOUGH_DATA:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Time-series must contain at least two data points.");
         break;
-    case FSys_POPULATE_INVALID_TIMES_DATA:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Times array must contain only floats.");
+    case TSys_POPULATE_INVALID_TIMES_DATA:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Times array must contain only floats.");
         break;
-    case FSys_POPULATE_INVALID_VALUES_DATA:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Values array must contain only floats.");
+    case TSys_POPULATE_INVALID_VALUES_DATA:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Values array must contain only floats.");
         break;
-    case FSys_POPULATE_DECREASING_TIMES_DATA:
-        PyErr_SetString(PyExc_Exception, "F-Pacing error: Times array must be non-decreasing.");
+    case TSys_POPULATE_DECREASING_TIMES_DATA:
+        PyErr_SetString(PyExc_Exception, "T-Pacing error: Times array must be non-decreasing.");
         break;
     // Unknown
     default:
-        PyErr_Format(PyExc_Exception, "F-Pacing error: Unlisted error %d", (int)flag);
+        PyErr_Format(PyExc_Exception, "T-Pacing error: Unlisted error %d", (int)flag);
         break;
     };
 }
 
 /*
- * Fixed-form pacing system
+ * Time series pacing system
  */
-struct FSys_Mem {
+struct TSys_Mem {
     Py_ssize_t n_points;   // The number of entries in the time and pace arrays
     double* times;  // The time array
     double* values; // The values array
     Py_ssize_t last_index; // The index of the most recently returned value
     //double level;   // The current output value
 };
-typedef struct FSys_Mem* FSys;
+typedef struct TSys_Mem* TSys;
 
 /*
- * Creates a fixed-form pacing system
+ * Creates a time series pacing system
  *
  * Arguments
- *  flag : The address of a fixed-form pacing error flag or NULL
+ *  flag : The address of a time series pacing error flag or NULL
  *
- * Returns the newly created fixed-form pacing system
+ * Returns the newly created time series pacing system
  */
-FSys
-FSys_Create(FSys_Flag* flag)
+TSys
+TSys_Create(TSys_Flag* flag)
 {
-    FSys sys = (FSys)malloc(sizeof(struct FSys_Mem));
+    TSys sys = (TSys)malloc(sizeof(struct TSys_Mem));
     if (sys == 0) {
-        if(flag != 0) *flag = FSys_OUT_OF_MEMORY;
+        if(flag != 0) *flag = TSys_OUT_OF_MEMORY;
         return 0;
     }
 
     sys->n_points = -1;
     sys->times = NULL;
     sys->values = NULL;
     sys->last_index = 0;
 
-    if(flag != 0) *flag = FSys_OK;
+    if(flag != 0) *flag = TSys_OK;
     return sys;
 }
 
 /*
- * Destroys a fixed-form pacing system and frees the memory it occupies.
+ * Destroys a time series pacing system and frees the memory it occupies.
  *
  * Arguments
- *  sys : The fixed-form pacing system to destroy
+ *  sys : The time series pacing system to destroy
  *
- * Returns a fixed-form pacing error flag.
+ * Returns a time series pacing error flag.
  */
-FSys_Flag
-FSys_Destroy(FSys sys)
+TSys_Flag
+TSys_Destroy(TSys sys)
 {
-    if(sys == 0) return FSys_INVALID_SYSTEM;
+    if(sys == 0) return TSys_INVALID_SYSTEM;
     if(sys->times != NULL) {
         free(sys->times);
         sys->times = NULL;
     }
     if(sys->values != NULL) {
         free(sys->values);
         sys->values = NULL;
     }
     free(sys);
-    return FSys_OK;
+    return TSys_OK;
 }
 
 /*
- * Populates a fixed-form pacing system using two Python list objects
+ * Populates a time series pacing system using two Python list objects
  * containing an equal number of floating point numbers.
  * Returns an error if the system already has data.
  *
  * Arguments
- *  sys    : The fixed-form pacing system to add the data to.
+ *  sys    : The time series pacing system to add the data to.
  *  times  : A Python list of (non-decreasing) floats.
  *  values : An equally sized Python list of floats.
  *
- * Returns a fixed-form pacing error flag.
+ * Returns a time series pacing error flag.
  */
-FSys_Flag
-FSys_Populate(FSys sys, PyObject* protocol)
+TSys_Flag
+TSys_Populate(TSys sys, PyObject* protocol)
 {
     int i;
     Py_ssize_t n;
     PyObject *times_list, *values_list;
 
     // Check ESys
-    if(sys == 0) return FSys_INVALID_SYSTEM;
-    if (sys->n_points != -1) return FSys_POPULATED_SYSTEM;
-    if (protocol == Py_None) return FSys_POPULATE_INVALID_PROTOCOL;
+    if(sys == 0) return TSys_INVALID_SYSTEM;
+    if (sys->n_points != -1) return TSys_POPULATED_SYSTEM;
+    if (protocol == Py_None) return TSys_POPULATE_INVALID_PROTOCOL;
 
     // Get PyList from protocol (will need to decref!)
     times_list = PyObject_CallMethod(protocol, "times", NULL); // Returns a new reference
-    if(times_list == NULL) return FSys_POPULATE_INVALID_PROTOCOL;
+    if(times_list == NULL) return TSys_POPULATE_INVALID_PROTOCOL;
     if(!PyList_Check(times_list)) {
         Py_DECREF(times_list);
-        return FSys_POPULATE_INVALID_TIMES;
+        return TSys_POPULATE_INVALID_TIMES;
     }
 
     // Check and convert times list
     n = PyList_Size(times_list);
     sys->times = (double*)malloc((size_t)n * sizeof(double));
     for(i=0; i<n; i++) {
         // GetItem and convert --> Borrowed reference so ok not to decref!
         sys->times[i] = PyFloat_AsDouble(PyList_GetItem(times_list, i));
     }
     Py_DECREF(times_list);  // Finished with the times_list
 
     if (PyErr_Occurred()) {
         free(sys->times); sys->times = NULL;
-        return FSys_POPULATE_INVALID_TIMES_DATA;
+        return TSys_POPULATE_INVALID_TIMES_DATA;
     }
     for(i=1; i<n; i++) {
         if(sys->times[i] < sys->times[i-1]) {
             free(sys->times); sys->times = NULL;
-            return FSys_POPULATE_DECREASING_TIMES_DATA;
+            return TSys_POPULATE_DECREASING_TIMES_DATA;
         }
     }
 
     // Check and convert values list
     values_list = PyObject_CallMethod(protocol, (char*)"values", NULL); // Returns a new reference
     if(values_list == NULL) {
         free(sys->times); sys->times = NULL;
-        return FSys_POPULATE_INVALID_PROTOCOL;
+        return TSys_POPULATE_INVALID_PROTOCOL;
     }
     if(!PyList_Check(values_list) || PyList_Size(values_list) != n) {
         free(sys->times); sys->times = NULL;
         Py_DECREF(values_list);
-        return FSys_POPULATE_INVALID_VALUES;
+        return TSys_POPULATE_INVALID_VALUES;
     }
     sys->values = (double*)malloc((size_t)n * sizeof(double));
     for(i=0; i<n; i++) {
         // GetItem and convert --> Borrowed reference so ok not to decref!
         sys->values[i] = PyFloat_AsDouble(PyList_GetItem(values_list, i));
     }
     Py_DECREF(values_list); // Finished with the values list
 
     if (PyErr_Occurred()) {
         free(sys->times); sys->times = NULL;
         free(sys->values); sys->values = NULL;
-        return FSys_POPULATE_INVALID_VALUES_DATA;
+        return TSys_POPULATE_INVALID_VALUES_DATA;
     }
 
     // Update pacing system and return
     sys->n_points = n;
     sys->last_index = 0;
-    return FSys_OK;
+    return TSys_OK;
 }
 
 /*
  * Returns the pacing level at the given time.
  *
  * Arguments
  *  sys : The pacing system to query for a value.
@@ -830,50 +831,50 @@
  *  flag : The address of a pacing error flag or NULL.
  *
  * Returns the value of the pacing level at the given time.
  * Will return -1 if an error occurs, so errors should always be checked for
  * using the flag argument!
  */
 double
-FSys_GetLevel(FSys sys, double time, FSys_Flag* flag)
+TSys_GetLevel(TSys sys, double time, TSys_Flag* flag)
 {
     // Index and time at left, mid and right point, plus guessed point
     Py_ssize_t ileft, imid, iright, iguess;
     double tleft, tmid, tright, tguess;
     double vleft;
 
     // Check system
     if(sys == 0) {
-        if(flag != 0) *flag = FSys_INVALID_SYSTEM;
+        if(flag != 0) *flag = TSys_INVALID_SYSTEM;
         return -1;
     }
     if(sys->n_points < 0) {
-        if(flag != 0) *flag = FSys_UNPOPULATED_SYSTEM;
+        if(flag != 0) *flag = TSys_UNPOPULATED_SYSTEM;
         return -1;
     }
 
     // Find the highest index `i` of sorted array `times` such that
     // `times[i] <= time`, or `-1` if no such index can be found.
     // A guess can be given, which will be used to speed things up
 
     // Get left point, check value
     ileft = 0;
     tleft = sys->times[ileft];
     if (tleft > time) {
         // Out-of-bounds on the left, return left-most value
-        if(flag != 0) *flag = FSys_OK;
+        if(flag != 0) *flag = TSys_OK;
         return sys->values[ileft];
     }
 
     // Get right point, check value
     iright = sys->n_points - 1;
     tright = sys->times[iright];
     if (tright <= time) {
         // Out-of-bounds on the right, return right-most value
-        if(flag != 0) *flag = FSys_OK;
+        if(flag != 0) *flag = TSys_OK;
         return sys->values[iright];
     }
 
     // Have a quick guess at better boundaries, using last
     iguess = sys->last_index - 1; // -1 is heuristic! Could be smaller
     if (iguess > ileft) {
         tguess = sys->times[iguess];
@@ -905,22 +906,36 @@
         imid = ileft + (iright - ileft) / 2;
     }
 
     // At this stage, tleft < time <= tright
 
     // Handle special case of time == tright
     // (Because otherwise it can happen that tleft == tright, which would give
-    //  a divide-by-zero in the interpolateion)
+    //  a divide-by-zero in the interpolation)
     if (time == tright) {
-        if(flag != 0) *flag = FSys_OK;
+        if(flag != 0) *flag = TSys_OK;
         sys->last_index = iright;
         return sys->values[iright];
     }
 
     // Find the correct value using linear interpolation
-    if(flag != 0) *flag = FSys_OK;
+    if(flag != 0) *flag = TSys_OK;
     sys->last_index = ileft;
     vleft = sys->values[ileft];
     return vleft + (sys->values[iright] - vleft) * (time - tleft) / (tright - tleft);
 }
 
+/*
+ * Pacing types
+ */
+union PSys {
+    ESys esys;
+    TSys tsys;
+};
+
+enum PSysType {
+    PSys_NOT_SET,
+    ESys_TYPE,
+    TSys_TYPE
+};
+
 #endif
```

### Comparing `myokit-1.35.0/myokit/_sim/rhs.c` & `myokit-1.35.1/myokit/_sim/rhs.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/rhs.py` & `myokit-1.35.1/myokit/_sim/rhs.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/sundials.c` & `myokit-1.35.1/myokit/_sim/sundials.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_sim/sundials.py` & `myokit-1.35.1/myokit/_sim/sundials.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_system.py` & `myokit-1.35.1/myokit/_system.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/_unit.py` & `myokit-1.35.1/myokit/_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
             attempt to use if the new and old units are incompatible. Each
             factor should be specified as a :class:`myokit.Quantity` or
             something that can be converted to a Quantity e.g. a string
             ``1 [uF/cm^2]``.
 
         Returns a :class:`myokit.Quantity`.
 
-        Raises a :class:`myokit.IncompatibleUnitError` if the units cannot be
+        Raises an :class:`myokit.IncompatibleUnitError` if the units cannot be
         converted.'
         """
         # Check unit1
         if not isinstance(unit1, myokit.Unit):
             if unit1 is None:
                 unit1 = myokit.units.dimensionless
             else:
```

### Comparing `myokit-1.35.0/myokit/float.py` & `myokit-1.35.1/myokit/float.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/__init__.py` & `myokit-1.35.1/myokit/formats/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -660,7 +660,185 @@
         if _EWRITERS is not None and name in _EWRITERS:
             del _EWRITERS[name]
     else:
         if _EWRITERS is None:  # pragma: no cover
             _scan_for_internal_formats()
         _EWRITERS[name] = ewriter_class
 
+
+class SweepSource:
+    """
+    Interface for classes that provide time-series data organised into *sweeps*
+    (or *records* or *episodes*) and *channels* (or *traces*).
+
+    The :class:`SweepSource` interface defines methods to get the number of
+    sweeps and channels, the names and units of the channels, and the data
+    stored in channels either as numpy arrays or in a :class:`myokit.DataLog`.
+
+    Each sweep contains the same number of channels, and each channel is
+    represented as a 1d array. In most cases these arrays have the same length
+    for every sweep, but whether this is the case for the current source can be
+    tested with :meth:`equal_length_sweeps`.
+
+    Data can be retrieved sweep by sweep::
+
+        (time[0], sweep[0]),        n_t data points, n_c channels of n_t points
+        (time[1], sweep[1]),
+        (time[2], sweep[2]),
+        ...
+        (time[n_s], sweep[n_s])
+
+    This allows plotting in the common "overlaid" fashion, i.e. plotting every
+    ``sweep[i] against ``time[0]``.
+
+    For other types of analysis (e.g. parameter estimation) the data can also
+    be returned as single time series::
+
+        time                            sum(n_t[i]) data points
+        sweep[0] + sweep[1] + ...       n_c channels, with sum(n_t[i]) points
+
+    Some formats can also contain information from which D/A output signals can
+    be reconstructed. These can be accessed using the :meth:`da`.
+
+    """
+    def channel(self, channel_id, join_sweeps=False):
+        """
+        Returns the data for a single channel, identified by integer or string
+        ``channel_id``.
+
+        With ``join_sweeps=False``, the data is returned as a tuple
+        ``(times, sweeps)`` where ``times`` and ``sweeps`` are 2d numpy arrays
+        indexed so that ``times[i][j]`` is the ``j``-th time point for sweep
+        ``i``.
+
+        If ``join_sweeps=True`` the sweeps are joined together, and a tuple
+        ``(times, values)`` is returned ``times`` and ``values`` are 1d arrays.
+        """
+        raise NotImplementedError
+
+    def channel_count(self):
+        """ Returns the number of channels. """
+        raise NotImplementedError
+
+    def channel_names(self, index=None):
+        """
+        Returns the names of all channels or the name of a specific channel
+        ``index``.
+        """
+        raise NotImplementedError
+
+    def channel_units(self, index=None):
+        """
+        Returns the units (as :class:`myokit.Unit`) of all channels or the
+        units of a specific channel ``index``.
+        """
+        raise NotImplementedError
+
+    def da(self, output_id, join_sweeps=False):
+        """ Like :meth:`channel`, but returns reconstructed D/A signals. """
+        raise NotImplementedError
+
+    def da_count(self):
+        """
+        Returns the available number of reconstructed D/A output channels.
+
+        This should return 0 if D/A channels are not supported.
+        """
+        raise NotImplementedError
+
+    def da_names(self, index=None):
+        """
+        Returns the names of all reconstructed D/A output channels or the name
+        of a specific output channel ``index``.
+
+        This will raise a ``NotImplementedError`` if D/A channels are not
+        supported.
+        """
+        raise NotImplementedError
+
+    def da_protocol(self, output_id=None, tu='ms', vu='mV', cu='pA',
+                    n_digits=9):
+        """
+        Returns a :class:`myokit.Protocol` representation of the D/A output
+        channel specified by name or integer ``output_id``.
+
+        If no explicit output channel is set, a guess will be made.
+
+        Time units will be converted to ``tu``, voltage units to ``vu``, and
+        current units to ``cu``. Other unit types will be left unchanged. Units
+        may be specified as :class:`myokit.Unit` objects or strings.
+
+        By default, floating point numbers in the protocol will be rounded to
+        9 digits after the decimal point. This can be customised using the
+        argument ``n_digits``.
+
+        If a D/A output cannot be converted to a :class:`myokit.Protocol`, a
+        ``ValueError`` is raised. A ``NotImplementedError`` is raised if D/A
+        channels are not supported at all.
+        """
+        raise NotImplementedError
+
+    def da_units(self, index=None):
+        """
+        Returns the units (as :class:`myokit.Unit`) of all reconstructed D/A
+        output channels or the units of a specific output channel ``index``.
+
+        This will raise a ``NotImplementedError`` if D/A channels are not
+        supported.
+        """
+        raise NotImplementedError
+
+    def equal_length_sweeps(self):
+        """
+        Returns ``True`` only if each sweep in this source has the same length.
+        """
+        raise NotImplementedError
+
+    def log(self, join_sweeps=False, use_names=False, include_da=True):
+        """
+        Returns a :class:`myokit.DataLog` containing the data from all
+        channels.
+
+        The log will have a single entry ``time`` corresponding to the time of
+        the first sweep if ``join_sweeps`` is ``False``, or the time of all
+        points when ``join_sweeps`` is ``True``.
+
+        Names will have a systematic form ``i_sweep.i_channel.label``, for
+        example ``0.1.channel`` for sweep 0 of recorded channel 1, or
+        ``3.0.da`` for sweep 3 of reconstructed D/A output 0. These can also be
+        accessed using the syntax ``log['channel', 1, 0]`` and
+        ``log['da', 0, 3]``.
+
+        To obtain a log with the user-specified names from the source instead,
+        set ``use_names`` to ``True``. This will result in names such as
+        ``0.IN 1`` or ``3.Cmd 0``.
+
+        To exclude D/A signal reconstructions, set ``include_da`` to ``False``.
+
+        A call with ``join_sweeps=False`` on a source where
+        :meth:`equal_length_sweeps()` returns ``False`` will raise a
+        ``ValueError``.
+        """
+        raise NotImplementedError
+
+    def meta_str(self, verbose=False):
+        """
+        Optional method that returns a multi-line string with unstructured meta
+        data about the source and its contents.
+
+        Will return ``None`` if no such string is available.
+        """
+        return None  # pragma: no cover
+
+    def sweep_count(self):
+        """
+        Returns the number of sweeps.
+
+        Note that a source with zero recorded channels may still report a
+        non-zero number of sweeps if it can provide D/A outputs.
+        """
+        raise NotImplementedError
+
+    def time_unit(self):
+        """ Returns the time unit used in this source. """
+        raise NotImplementedError
+
```

### Comparing `myokit-1.35.0/myokit/formats/ansic/__init__.py` & `myokit-1.35.1/myokit/formats/ansic/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/ansic/_ewriter.py` & `myokit-1.35.1/myokit/formats/ansic/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/ansic/_exporter.py` & `myokit-1.35.1/myokit/formats/ansic/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/ansic/template/cable.c` & `myokit-1.35.1/myokit/formats/ansic/template/cable.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/ansic/template/euler.c` & `myokit-1.35.1/myokit/formats/ansic/template/euler.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/ansic/template/sim.c` & `myokit-1.35.1/myokit/formats/ansic/template/sim.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/axon/__init__.py` & `myokit-1.35.1/myokit/formats/axon/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/axon/_abf.py` & `myokit-1.35.1/myokit/formats/axon/_abf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This module reads files in Axon Binary File format v1 or v2 used by Axon
 # Technologies and Molecular Devices.
-# The v1 format was used until Clampex version 9. Clampex 10 and onwards use
-# the v2 format.
+# The v1 format was used until Clampex version 9.
+# Clampex 10 and onwards use the v2 format.
 #
 # WARNING: This file hasn't been extensively tested.
 #
 # About ABF
 # ---------
 # pClamp version 10 introduced a new .abf file format ABF2, with format version
 #  numbers 2.0 and up. Older version are referred to a version 1 (even though
@@ -53,34 +53,33 @@
 # Stimulus waveforms
 # ------------------
 # A stimulus signal in pClamp is termed a 'waveform'. Each waveform is divided
 #  into a series of steps, ramps or pulse trains. Such a subsection is called
 #  an 'epoch'. The protocol section of a file defines one or more stimuli, each
 #  containing a list of epochs.
 #
-# Conversion to myokit formats
-# ----------------------------
-# There is no problem-free mapping of ABF data onto myokit structures, such as
-# the simulation log. A fundamental difference is that "sampling" during a
-# simulation happens at the same time for every signal. Channels in an ABF file
-# each have their own sampling rate.
-#
 #---------------------------------  license  ----------------------------------
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 #---------------------------------  credits  ----------------------------------
 #
-# This module is derived in part from code found in the Neo package for
-# representing electrophysiology data, specifically from a python module
-# authored by sgarcia and jnowacki.
+# A lot of this code uses the (sadly somewhat outdated) information made public
+# by Axon, e.g. at https://support.moleculardevices.com/s/article/
+#                               Axon-pCLAMP-ABF-File-Support-Pack-Download-Page
+# This information comes without a specific license, but states that
+# "Permission is granted to freely use, modify and copy the code in this file."
+#
+# In addition, this module was in part derived from an early version of the
+# Neo package for representing electrophysiology data, specifically from a
+# Python module authored by sgarcia and jnowacki.
 # Neo can be found at: http://neuralensemble.org/trac/neo
 #
-# The Neo package is licensed using the following BSD License:
+# The Neo package used was licensed using the following BSD License:
 #
 #----------------------------------  start  -----------------------------------
 # Copyright (c) 2010-2012, Neo authors and contributors
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
@@ -136,574 +135,186 @@
 # The abf2load script is available from:
 #  http://www.mathworks.com/matlabcentral/fileexchange/22114-abf2load
 #------------------------------------------------------------------------------
 # Information - but no direct code - from the matlab script get_abf_header.m
 # was also used: http://neurodata.hg.sourceforge.net/hgweb/neurodata/neurodata/
 #------------------------------------------------------------------------------
 import datetime
-import logging
 import os
 import struct
-import traceback
+import warnings
 
 import numpy as np
 
-from collections import OrderedDict
+import myokit
+import myokit.formats
 
 
 # Encoding for text parts of files
 _ENC = 'latin-1'
 
 
-class AbfFile:
+class AbfFile(myokit.formats.SweepSource):
     """
     Represents a read-only Axon Binary Format file (``.abf``), stored at the
     location pointed to by ``filepath``.
 
     Files in the "ABF" format and the newer "ABF2" format can be read. If the
     given ``filepath`` ends in ``.pro`` a protocol file is assumed. This
     assumption can be overruled by setting the ``is_protocol_file`` argument
     to either ``True`` or ``False``.
 
-    The "data" in an AbfFile is recorded (analog-to-digital) data. Any output
-    signals from the amplifier to the cell (digital-to-analog) are termed the
-    "protocol".
-
-    Data in AbfFiles is recorded in episodes called "sweeps". Each sweep
-    contains the data from all recorded channels. The number of channels is
-    constant: channel 1 in sweep 1 contains data recorded from the same source
-    as channel 1 in sweep 10.
+    Data in ABF files is recorded in *sweeps*, where each sweep contains one or
+    more *channels* with recorded (A/D) data. In addition, zero or more output
+    waveforms may be defined (also called "protocol" or D/A channels). Where
+    possible, the :class`AbfFile` class will convert these embedded protocols
+    to time series and include them as additional channels.
 
-    The data in an ``AbfFile`` can be read by iterating over it::
+    For example::
 
-        f = AbfFile('some_file.abf')
-        for sweep in f:
+        abf = AbfFile('some_file.abf')
+        for sweep in abf:
             for channel in sweep:
-                plt.plot(channel.times(), channel.values())
+                print(channel.name())
+            break
 
-    Similarly, protocol data can be accessed using::
+    might show
 
-        for sweep in f.protocol():
-            for channel in sweep:
-                plt.plot(channel.times(), channel.values())
+        IN 0
+        10xVm
+        Cmd 0
+
+    where the first two channels are recorded A/D channels and the final one is
+    a reconstructed D/A output channel.
 
-    Note that the number of output ("protocol") channels need not equal the
-    number of input ("data") channels.
+    Sweeps and channels are represented by :class:`Sweep` and :class:`Channel`
+    objects respectively, and these can be used to obtain the data from a
+    file::
 
-    Because each channel can have a different sampling rate, AbfFile data is
-    not one-on-one compatible with myokit Simulation logs. To obtain a
-    :class:`myokit.DataLog` version of the file's data, use:meth:`myokit_log`.
+        abf = AbfFile('some_file.abf')
+        for sweep in abf:
+            for channel in sweep:
+                plot(channel.times(), channel.values())
+
+    In addition the ``AbfFile`` class implements the
+    :class`myokit.formats.SweepSource` interface. Note that this interface
+    treats A/D and D/A as separate things, so :meth:`channel_count` returns the
+    number of A/D channels, not the total number of channels in a
+    :class:`Sweep` object (which can include D/A channels).
+
+    Support notes:
+
+    - Protocol (D/A) conversion is only supported for "episodic stimulation"
+      with constant valued steps (so e.g. no ramps) and without "user lists".
+    - Protocols with more than one sampling rate are not supported.
+    - The publicly available information on the ABF format is not great, so
+      there will be several other issues and shortcomings.
+
+    Arguments:
+
+    ``filepath``
+        The path to load the data from. Data will be read into memory
+        immediately upon construction.
+    ``is_protocol_file``
+        If set to ``True``, no attempt to read A/D data will be made and only
+        D/A "protocol" information will be read. If left at its default value
+        of ``None`` files with the extension ``.pro`` will be recognized as
+        protocol files.
 
-    In some cases, a myokit protocol can be created from a stored stimulus
-    protocol. To do this, use the method:meth:`myokit_protocol`.
     """
     def __init__(self, filepath, is_protocol_file=None):
         # The path to the file and its basename
         filepath = str(filepath)
         self._filepath = os.path.abspath(filepath)
         self._filename = os.path.basename(filepath)
 
-        # Abf format version
-        self._version = None
-
-        # Protocol info
-        self._epoch_functions = None
-        self._numberOfTrials = None
-        self._trialStartToStart = None
-        self._runsPerTrial = None
-        self._runStartToStart = None
-        self._sweepsPerRun = None
-        self._sweepStartToStart = None
-
         # Read as protocol file yes?
         if is_protocol_file is None:
             self._is_protocol_file = os.path.splitext(filepath)[1] == '.pro'
         else:
             self._is_protocol_file = bool(is_protocol_file)
 
-        # The file header (an ordered dictionary)
-        self._header = self._read_header()
-
-        # Date/time of recording
-        self._datetime = self._read_datetime()
-
-        # Number of channels, sampling rate (Hz) and acquisition mode
-        if self._version < 2:
-            self._nc = self._header['nADCNumChannels']
-            self._rate = 1e6 / (self._header['fADCSampleInterval'] * self._nc)
-            self._mode = self._header['nOperationMode']
-        else:
-            self._nc = self._header['sections']['ADC']['length']
-            self._rate = 1e6 / self._header['protocol']['fADCSequenceInterval']
-            self._mode = self._header['protocol']['nOperationMode']
-        if self._mode not in acquisition_modes:
-            raise NotImplementedError(
-                'Unknown acquisition mode: ' + str(mode))
+        # Cached string-to-unit conversions
+        self._unit_cache = {}
 
-        # Conversion factors for integer data in the channels
-        self._adc_factors = None
-        self._adc_offsets = None
-        self._set_conversion_factors()
-
-        # The protocol used (a list of sweeps)
-        try:
-            self._protocol = self._read_protocol()
-        except Exception:   # pragma: no cover
-            # This is not something we _want_ to happen, so if we have test
-            # cases that trigger this error they should be resolved. At the
-            # same time, if it happens to a user we want it to "sort-of work"
-            # (an experimental rather than a production setting)
-            log = logging.getLogger(__name__)
-            log.warning('Unable to read protocol from ' + self._filepath)
-            log.warning(traceback.format_exc())
-            self._protocol = []
+        # Read the file header as an ordered dictionary
+        self._header = None
+        self._strings = None
+        self._version = None
+        self._version_str = None
+        self._read_1_header()
 
-        # The measured data as a list of sweeps
-        if self._is_protocol_file:
-            self._sweeps = []
-        else:
-            self._sweeps = self._read_sweeps()
+        # Read the time of recording
+        self._datetime = None
+        self._read_2_time_of_recording()
+
+        # Read the protocol information
+        self._n_adc = None
+        self._n_dac = None
 
-    def data_channels(self):
-        """
-        Returns the number of channels in this file's sweeps.
-        """
-        if len(self._sweeps) == 0:  # pragma: no cover
-            return 0
-        return len(self._sweeps[0])
+        self._rate = None
+        self._mode = None
 
-    def extract_channel(self, channel=0, join=False):
-        """
-        Extracts a selected data ``channel`` and returns its data in a tuple
-        containing::
+        self._number_of_trials = None
+        self._trial_start_to_start = None
+        self._runs_per_trial = None
+        self._run_start_to_start = None
+        self._sweeps_per_run = None
+        self._sweep_start_to_start = None
+        self._samples_per_channel = None
 
-             A numpy array representing time
-             A numpy array representing the first sweep
-             A numpy array representing the second sweep
-             ...
+        # To be able to treat v1 and v2 slightly more easily, we define 3
+        # functions read epoch info from episodic stimulation protocols
+        self._epoch_functions = None
 
-        An optional argument ``join=True`` can be set to join all sweeps
-        together and return just two arrays, one for time and one for data.
+        # Not all D/A channels can be converted, so we maintain an array with
+        # the original indices of the channels in the da_sweeps. (Note that
+        # this differs again from the "index" labels for user display, which
+        # are stored in the channels themselves).
+        self._dac_indices = []
+
+        # Read protocol information and create empty sweep objects
+        # Sweeps contain both A/D channels and D/A reconstructions. Some files
+        # will have A/D but no (or no supported) D/A. Conversely protocol files
+        # will have D/A only. So all in one sweep is easiest.
+        self._sweeps = None
 
-        If no data is available, ``None`` is returned.
-        """
-        if len(self._sweeps) == 0:  # pragma: no cover
-            return None
+        self._read_3_protocol_information()
 
-        # Join all sweeps
-        if join:
-            time, data = [], []
-            t = np.array(self._sweeps[0][channel].times())
-            for i, sweep in enumerate(self._sweeps):
-                time.append(t + i * self._sweepStartToStart)
-                data.append(np.array(sweep[channel].values()))
-            return (np.concatenate(time), np.concatenate(data))
+        # Read and calculate conversion factors for integer data in ADC
+        self._adc_factors = None
+        self._adc_offsets = None
+        self._read_4_ad_conversion_factors()
 
-        # Standard reading
-        data = []
-        data.append(np.array(self._sweeps[0][channel].times()))
+        # Read the A/D channel data and add it to the sweeps
+        if self._n_adc:
+            self._read_5_ad_data()
+
+        # Reconstruct D/A signals as additional channels and add to the sweeps
+        self._read_6_da_reconstructions()
+
+        # Copy channel names and units, for easier SweepSource implementation
+        self._ad_names = {}
+        self._da_names = {}
+        self._ad_units = []
+        self._da_units = []
         for sweep in self._sweeps:
-            data.append(np.array(sweep[channel].values()))
-        return tuple(data)
-
-    def extract_channel_as_myokit_log(self, channel=0):
-        """
-        Extracts the given data channel and returns it as a myokit
-        DataLog.
-
-        The log will contain an entry "time" that contains the time vector.
-        Each sweep will be in an entry "0.sweep", "1.sweep", "2.sweep" etc.
-        """
-        import myokit
-        log = myokit.DataLog()
-        if len(self._sweeps) == 0:  # pragma: no cover
-            return log
-        log.set_time_key('time')
-        log['time'] = np.array(self._sweeps[0][channel].times())
-        for k, sweep in enumerate(self._sweeps):
-            log['sweep', k] = np.array(sweep[channel].values())
-        return log
-
-    def filename(self):
-        """
-        Returns this AbfFile's filename.
-        """
-        return self._filepath
-
-    def __getitem__(self, key):
-        return self._sweeps.__getitem__(key)
-
-    def _get_conversion_factors(self, channel):
-        """
-        Returns the conversion factor and shift for the selected channel as a
-        tuple of floats ``(factor, shift)``.
-        """
-        return self._adc_factors[channel], self._adc_offsets[channel]
-
-    def info(self, show_header=False):
-        """
-        Returns a string with lots of info on this file.
-
-        The optional argument ``show_header`` can be used to add the full
-        header contents to the output.
-        """
-        out = []
-
-        # Show file info
-        if self._is_protocol_file:
-            out.append('Axon Protocol File: ' + self._filename)
-        else:
-            out.append('Axon Binary File: ' + self._filename)
-        out.append('ABF Format version ' + str(self._version))
-        out.append('Recorded on: ' + str(self._datetime))
-
-        # Show protocol info
-        out.append(
-            'Acquisition mode: ' + str(self._mode) + ': '
-            + acquisition_modes[self._mode])
-        if self._numberOfTrials:
-            out.append(
-                'Protocol set for ' + str(self._numberOfTrials)
-                + ' trials, spaced ' + str(self._trialStartToStart)
-                + 's apart.')
-            out.append(
-                '    with ' + str(self._runsPerTrial)
-                + ' runs per trial, spaced ' + str(self._runStartToStart)
-                + 's apart.')
-            out.append(
-                '     and ' + str(self._sweepsPerRun)
-                + ' sweeps per run, spaced ' + str(self._sweepStartToStart)
-                + 's apart.')
-        else:   # pragma: no cover
-            out.append('Protocol data could not be determined.')
-        out.append('Sampling rate: ' + str(self._rate) + ' Hz')
-
-        # Show channel info
-        if self._sweeps:
-            for i, c in enumerate(self._sweeps[0]._channels):
-                out.append('Channel ' + str(i) + ': "' + c._name + '"')
-                if c._type:  # pragma: no cover
-                    # Cover pragma: Don't have appropriate test file
-                    out.append('  Type: ' + type_mode_names[c._type])
-                out.append('  Unit: ' + c._unit.strip())
-                if c._lopass:
-                    out.append('  Low-pass filter: ' + str(c._lopass) + ' Hz')
-                if c._cm:
-                    out.append('  Cm (telegraphed): ' + str(c._cm) + ' pF')
-                if c._rs:   # pragma: no cover
-                    # Cover pragma: Don't have appropriate test file
-                    out.append('  Rs (telegraphed): ' + str(c._rs))
-
-        # Methods
-        def show_dict(name, d, tab=''):
-            m = max(0, 38 - len(tab) - int(0.1 + len(name) / 2))
-            out.append(tab + '-' * m + '  ' + name + '  ' + '-' * m)
-            for n, v in d.items():
-                n = str(n)
-                if type(v) == OrderedDict:
-                    show_dict(n, v, tab + '  ')
-                elif type(v) == list:
-                    show_list(n, v, tab)
-                else:
-                    out.append(tab + n + ': ' + str(v))
-            m = max(0, 80 - 2 * len(tab))
-            out.append(tab + m * '-')
-
-        def show_list(name, d, tab=''):
-            for index, item in enumerate(d):
-                n = name + '[' + str(index) + ']'
-                if type(item) == OrderedDict:
-                    show_dict(n, item, tab)
-                elif type(item) == list:    # pragma: no cover
-                    # Cover pragma: Don't have appropriate test file
-                    show_list(n, item, tab)
-                else:
-                    out.append(tab + n + ': ' + str(item))
-
-        # Show full header info
-        if show_header:
-            if self.strings:
-                show_dict('Strings', {'strings': self.strings})
-            show_dict('file header', self._header)
-        return '\n'.join(out)
-
-    def matplotlib_figure(self):
-        """
-        Creates and returns a matplotlib figure of this abf file's contents.
-        """
-        import matplotlib.pyplot as plt
-        f = plt.figure()
-        plt.suptitle(self.filename())
-
-        # Show data channel
-        ax = plt.subplot(2, 1, 1)
-        ax.set_title('Measured data')
-        times = None
-        for sweep in self:
-            for channel in sweep:
-                if times is None:
-                    times = channel.times()
-                plt.plot(times, channel.values())
-
-        # Show protocol channels
-        n = self.protocol_channels()
-        ax = [plt.subplot(2, n, n + 1 + i) for i in range(n)]
+            for i, channel in enumerate(sweep[:self._n_adc]):
+                self._ad_names[channel.name()] = i
+                self._ad_units.append(channel.unit())
+            for i, channel in enumerate(sweep[self._n_adc:]):
+                self._da_names[channel.name()] = i
+                self._da_units.append(channel.unit())
+            break
 
-        for sweep in self.protocol():
-            times = None
-            for i, channel in enumerate(sweep):
-                if times is None:
-                    times = channel.times()
-                ax[i].set_title(channel.name())
-                ax[i].plot(times, channel.values())
-        return f
-
-    def myokit_log(self):
-        """
-        Converts the data in this ABF file to a:class:`myokit.DataLog` with an
-        entry for every channel. All sweeps will be joined together into a
-        single time series.
-
-        The log will contain an entry "time" that contains the time vector.
-        Channels will be stored using "0.ad", "1.ad" etc. for the recorded
-        (analog-to-digital) channels and "0.da", "1.da" etc. for the output
-        (digital-to-analog) channels.
-        """
-        import myokit
-        log = myokit.DataLog()
-        if self._sweeps:
-            # Gather parts of time and channel vectors
-            time = []
-            ad_channels = []
-            da_channels = []
-            for i in range(self.data_channels()):
-                ad_channels.append([])
-            for i in range(self.protocol_channels()):
-                da_channels.append([])
-
-            # Add ad channels
-            for sweep in self:
-                for channel in sweep:
-                    time.append(channel.times())
-                    break
-                for i, channel in enumerate(sweep):
-                    ad_channels[i].append(channel.values())
-
-            # Add da channels
-            for sweep in self.protocol():
-                for i, channel in enumerate(sweep):
-                    da_channels[i].append(channel.values())
-
-            # Combine into time series, store in log
-            log['time'] = np.concatenate(time)
-            log.set_time_key('time')
-            for i, channel in enumerate(ad_channels):
-                log['ad', i] = np.concatenate(channel)
-            for i, channel in enumerate(da_channels):
-                log['da', i] = np.concatenate(channel)
-
-        return log
-
-    def myokit_protocol(self, channel=None, ms=True):
-        """
-        Returns a single channel from an embedded protocol as a
-        :class:`myokit.Protocol`. The channel to return is specified by setting
-        ``channel`` to the correct index.
-
-        Only works for episodic stimulation, without user lists.
-
-        By default, all times are converted to milliseconds. To disable this
-        function, set ``ms=False``.
-        """
-        import myokit
-
-        # Only episodic stimulation is supported.
-        if self._mode != ACMODE_EPISODIC_STIMULATION:  # pragma: no cover
-            return myokit.Protocol()
-
-        # Check channel
-        if channel is None:
-            channel = 0
-        else:
-            channel = int(channel)
-
-        # User lists are not supported
-        if self._version < 2:  # pragma: no cover
-            if self._header['nULEnable'][channel]:
-                raise NotImplementedError('User lists are not supported.')
-        else:   # pragma: no cover
-            for userlist in self._header['listUserListInfo']:
-                en1 = 'nULEnable' in userlist and userlist['nULEnable']
-                en2 = 'nConditEnable' in userlist and userlist['nConditEnable']
-                if en1 or en2:
-                    raise NotImplementedError('User lists are not supported.')
-
-        # Create protocol
-        p = myokit.Protocol()
-
-        # Get epoch functions set by _read_protocol
-        dinfo, einfo_exists, einfo = self._epoch_functions
-        start = 0
-        next_start = 0
-        f = 1e3 if ms else 1
-        for iSweep in range(self._sweepsPerRun):
-
-            if not einfo_exists(channel):   # pragma: no cover
-                # Not sure if this can happen, if so, would need to update code
-                raise Exception('Missing protocol data')
-
-            for e in einfo(channel):
-                kind = e['type']
-
-                if kind not in epoch_types:
-                    raise NotImplementedError(
-                        'Unknown epoch type: ' + str(kind))
-
-                if kind == EPOCH_DISABLED:
-                    continue
-
-                elif kind == EPOCH_STEPPED:
-                    # Event at step
-                    dur = f * e['init_duration'] / self._rate
-                    inc = f * e['duration_inc'] / self._rate
-                    e_level = e['init_level'] + e['level_inc'] * iSweep
-                    e_start = start
-                    e_length = dur + iSweep * inc
-                    p.schedule(e_level, e_start, e_length)
-                    start += e_length
-
-                else:   # pragma: no cover
-                    raise NotImplementedError(
-                        'Usupported epoch type: ' + epoch_types(kind))
-
-            # Event at holding potential
-            next_start += f * self._sweepStartToStart
-            e_level = dinfo(channel, 'fDACHoldingLevel')
-            e_start = start
-            e_length = next_start - start
-            p.schedule(e_level, e_start, e_length)
-            start = next_start
-
-        return p
-
-    def protocol_channels(self):
-        """
-        Returns the number of channels in this file's protocol.
-        """
-        if self._version < 2:
-            return len(self._header['sDACChannelName'])
-        else:
-            return int(self._header['sections']['DAC']['length'])
-
-    def protocol_holding_level(self, channel=0):
-        """
-        Returns the holding level used by the requested output channel of the
-        embedded protocol.
-        """
-        dinfo, einfo_exists, einfo = self._epoch_functions
-        return dinfo(channel, 'fDACHoldingLevel')
-
-    def protocol_steps(self, channel=0):
-        """
-        For a stepped protocol, this function returns a tuple of lists of the
-        successive values (not including the holding value).
-
-        For example, for a protocol that has holding value ``-120mV`` and
-        performs steps to ``-100mV``, ``-80mV``, and ``-40mV`` the returned
-        output will be::
-
-            ([-100, -80, -40])
-
-        For a more complicated protocol, where each step is followed by a step
-        down to ``-140mV``, the output would be::
-
-            ([-100, -80, -40], [-140, -140, -140])
-
-
-        """
-        # Get epoch functions set by _read_protocol
-        dinfo, einfo_exists, einfo = self._epoch_functions
-        if not einfo_exists(channel):  # pragma: no cover
-            # Not sure if this can happen, if so need to update code.
-            raise Exception('Missing protocol data')
-
-        # Create list of step lists
-        levels = []
-        for e in einfo(channel):
-            kind = e['type']
-            if kind not in epoch_types:
-                raise NotImplementedError('Unknown epoch type: ' + str(kind))
-            if kind == EPOCH_DISABLED:
-                continue
-            elif kind == EPOCH_STEPPED:
-                levels.append([])
-            else:
-                raise NotImplementedError(
-                    'Unsupported epoch type: ' + epoch_types(kind))
-
-        # Gather steps
-        levels = tuple(levels)
-        for i in range(self._sweepsPerRun):
-            j = 0
-            for e in einfo(channel):
-                if e['type'] == EPOCH_STEPPED:
-                    levels[j].append(e['init_level'] + e['level_inc'] * i)
-                    j += 1
-        return levels
-
-    def __iter__(self):
-        """
-        Returns an iterator over all sweeps
-        """
-        return iter(self._sweeps)
-
-    def __len__(self):
-        """
-        Returns the number of sweeps in this file.
-        """
-        return len(self._sweeps)
-
-    def protocol(self):
-        """
-        Returns an interator over the protocol data.
-        """
-        return iter(self._protocol)
-
-    def _read_datetime(self):
-        """
-        Reads the date/time this file was recorded
-        """
-        # Get date and time
-        if self._version < 2:
-            t1 = str(self._header['lFileStartDate'])
-            t2 = float(self._header['lFileStartTime'])
-        else:
-            t1 = str(self._header['uFileStartDate'])
-            t2 = float(self._header['uFileStartTimeMS']) / 1000
-
-        YY = int(t1[0:4])
-        MM = int(t1[4:6])
-        DD = int(t1[6:8])
-        hh = int(t2 / 3600)
-        mm = int((t2 - hh * 3600) / 60)
-        ss = t2 - hh * 3600 - mm * 60
-        ms = int((ss % 1) * 1e6)
-        ss = int(ss)
-
-        return datetime.datetime(YY, MM, DD, hh, mm, ss, ms)
-
-    def _read_header(self):
-        """
-        Reads the file's header.
-        """
+    def _read_1_header(self):
+        """ Read the file header. """
 
         def read_f(f, form, offset=None):
-            """
-            Read and unpack a file section using the given format ``form``.
-            """
+            """ Read and unpack a file section in the format ``form``. """
             form = str(form)
             if offset is not None:
                 f.seek(offset)
             return struct.unpack(form, f.read(struct.calcsize(form)))
 
         def ups(val):
             """
@@ -715,15 +326,15 @@
             3. Strings containing only \\x00 are replaced by ``None``
 
             """
             # Convert bytes
             values = [0] * len(val)
             for i, v in enumerate(val):
                 if isinstance(v, bytes):
-                    v = v.decode(_ENC)
+                    v = v.decode(_ENC).strip()
                     # Handle long \x00 lists
                     if v and ord(v[0]) == 0:
                         return None
                 values[i] = v
             del val
 
             # Unpack single
@@ -737,29 +348,29 @@
             # version 2)
             sig = f.read(4).decode(_ENC)
             if sig == 'ABF ':
                 version = 1
             elif sig == 'ABF2':
                 version = 2
             else:
-                raise NotImplementedError(
-                    'Unknown ABF Format "' + str(sig) + '".')
+                raise NotImplementedError('Unknown ABF Format "{sig}".')
 
             # Gather header fields
-            header = OrderedDict()
-            for key, offset, form in headerFields[version]:
+            header = {}
+            for key, offset, form in HEADER_FIELDS[version]:
                 header[key] = ups(read_f(f, form, offset))
 
             # Get uniform file version number
             if version < 2:
-                self._version = (
-                    np.round(header['fFileVersionNumber'] * 100) / 100)
+                self._version = np.round(header['fFileVersionNumber'], 5)
+                self._version_str = str(self._version)
             else:
-                n = header['fFileVersionNumber']
-                self._version = n[3] + 0.1 * n[2] + 0.01 * n[1] + 0.001 * n[0]
+                v = header['fFileVersionNumber']
+                self._version = v[3]
+                self._version_str = '.'.join([str(v) for v in reversed(v)])
 
             # Get file start time in seconds
             if version < 2:
                 header['lFileStartTime'] += (
                     header['nFileStartMillisecs'] / 1000)
             else:
                 header['lFileStartTime'] = header['uFileStartTimeMS'] / 1000
@@ -767,29 +378,29 @@
             if version < 2:
 
                 # Version 1: Only read tags
                 tags = []
                 for i in range(header['lNumTagEntries']):  # pragma: no cover
                     # Cover pragma: Don't have appropriate test file
                     f.seek(header['lTagSectionPtr'] + i * 64)
-                    tag = OrderedDict()
-                    for key, form in TagInfoDescription:
+                    tag = {}
+                    for key, form in ABF2_TAG_INFO_DESCRIPTION:
                         tag[key] = ups(read_f(f, form))
                     tags.append(tag)
                 header['tags'] = tags
-                self.strings = []
+                self._strings = []
 
             else:
 
                 # Version 2
                 # Find location of file sections
-                sections = OrderedDict()
-                for i, s in enumerate(abf2FileSections):
+                sections = {}
+                for i, s in enumerate(ABF2_FILE_SECTIONS):
                     index, data, length = read_f(f, 'IIl', 76 + i * 16)
-                    sections[s] = OrderedDict()
+                    sections[s] = {}
                     sections[s]['index'] = index
                     sections[s]['data'] = data
                     sections[s]['length'] = length
                 header['sections'] = sections
 
                 # String section contains channel names and units
                 f.seek(sections['Strings']['index'] * BLOCKSIZE)
@@ -803,146 +414,206 @@
                 # ABFLONG  lTotalBytes; 4 bytes
                 # UINT  uUnused[6];     24 bytes
                 # Total: 44 bytes
                 strings = strings[44:]
 
                 # C-style string termination
                 strings = strings.split(b'\x00')
-                strings = [s.decode(_ENC) for s in strings]
-                self.strings = strings
+                strings = [s.decode(_ENC).strip() for s in strings]
+                self._strings = strings
 
                 # Read tag section
                 tags = []
                 offs = sections['Tag']['index'] * BLOCKSIZE
                 size = sections['Tag']['data']
                 for i in range(sections['Tag']['length']):  # pragma: no cover
                     # Cover pragma: Don't have appropriate test file
                     f.seek(offs + i * size)
-                    tag = OrderedDict()
-                    for key, form in TagInfoDescription:
+                    tag = {}
+                    for key, form in ABF2_TAG_INFO_DESCRIPTION:
                         tag[key] = ups(read_f(f, form))
                     tags.append(tag)
                 header['tags'] = tags
 
                 # Read protocol section
-                protocol = OrderedDict()
+                protocol = {}
                 offs = sections['Protocol']['index'] * BLOCKSIZE
                 f.seek(offs)
-                for key, form in protocolFields:
+                for key, form in ABF2_PROTOCOL_FIELDS:
                     protocol[key] = ups(read_f(f, form))
                 header['protocol'] = protocol
 
                 # Read analog-digital conversion sections
                 adc = []
                 offs = sections['ADC']['index'] * BLOCKSIZE
                 size = sections['ADC']['data']
                 for i in range(sections['ADC']['length']):
-                    ADC = OrderedDict()
+                    ADC = {}
                     f.seek(offs + i * size)
-                    for key, form in ADCFields:
+                    for key, form in ABF2_ADC_FIELDS:
                         ADC[key] = ups(read_f(f, form))
                     # Get channel name and unit
                     ADC['ADCChNames'] = (
                         strings[ADC['lADCChannelNameIndex'] - 1])
                     ADC['ADCChUnits'] = strings[ADC['lADCUnitsIndex'] - 1]
                     adc.append(ADC)
                 header['listADCInfo'] = adc
 
                 # Read DAC section
                 dac = []
                 offs = sections['DAC']['index'] * BLOCKSIZE
                 size = sections['DAC']['data']
                 for i in range(sections['DAC']['length']):
                     f.seek(offs + size * i)
-                    DAC = OrderedDict()
-                    for key, form in DACFields:
+                    DAC = {}
+                    for key, form in ABF2_DAC_FIELDS:
                         DAC[key] = ups(read_f(f, form))
                     DAC['sDACChannelName'] = \
                         strings[DAC['lDACChannelNameIndex'] - 1]
                     DAC['sDACChannelUnits'] = \
                         strings[DAC['lDACChannelUnitsIndex'] - 1]
                     dac.append(DAC)
                 header['listDACInfo'] = dac
 
                 # Read UserList section
-                userlists = []
+                user_lists = []
+                offs = sections['UserList']['index'] * BLOCKSIZE
+                size = sections['UserList']['data']
                 r = range(sections['UserList']['length'])
                 for i in r:  # pragma: no cover
                     # Cover pragma: User lists are not supported
                     f.seek(offs + size * i)
-                    UserList = OrderedDict()
-                    for key, form in UserListFields:
-                        UserList[key] = ups(read_f(f, form))
-                    userlists.append(DAC)
-                header['listUserListInfo'] = userlists
+                    user_list = {}
+                    for key, form in ABF2_USER_LIST_FIELDS:
+                        user_list[key] = ups(read_f(f, form))
+                    user_lists.append(user_list)
+                header['listUserListInfo'] = user_lists
 
                 # Read epoch-per-DAC section
                 # The resulting OrderedDict has the following structure:
                 #  - the first index is the DAC number
                 #  - the second index is the epoch number
-                header['epochInfoPerDAC'] = OrderedDict()
+                header['epochInfoPerDAC'] = {}
                 offs = sections['EpochPerDAC']['index'] * BLOCKSIZE
                 size = sections['EpochPerDAC']['data']
-                info = OrderedDict()
+                info = {}
                 for i in range(sections['EpochPerDAC']['length']):
                     f.seek(offs + size * i)
-                    einf = OrderedDict()
-                    for key, form in EpochInfoPerDACFields:
+                    einf = {}
+                    for key, form in ABF2_EPOCH_INFO_PER_DAC_FIELD:
                         einf[key] = ups(read_f(f, form))
                     DACNum = einf['nDACNum']
                     EpochNum = einf['nEpochNum']
                     if DACNum not in info:
-                        info[DACNum] = OrderedDict()
+                        info[DACNum] = {}
                     info[DACNum][EpochNum] = einf
                 header['epochInfoPerDAC'] = info
 
-        return header
+        self._header = header
 
-    def _read_protocol(self):
-        """
-        Reads the protocol stored in the ABF file and converts it to an analog
-        signal.
+    def _read_2_time_of_recording(self):
+        """ Read and process the time when this file was recorded. """
 
-        Only works for episodic stimulation, without any user lists.
+        if self._version < 2:
+            t1 = str(self._header['lFileStartDate'])
+            t2 = float(self._header['lFileStartTime'])
+        else:
+            t1 = str(self._header['uFileStartDate'])
+            t2 = float(self._header['uFileStartTimeMS']) / 1000
 
-        The resulting analog signal has the same size as the recorded signals,
-        so not the full length of the protocol! This is different from the
-        values returned by the Myokit
+        YY = int(t1[0:4])
+        MM = int(t1[4:6])
+        DD = int(t1[6:8])
+        hh = int(t2 / 3600)
+        mm = int((t2 - hh * 3600) / 60)
+        ss = t2 - hh * 3600 - mm * 60
+        ms = int((ss % 1) * 1e6)
+        ss = int(ss)
+
+        self._datetime = datetime.datetime(YY, MM, DD, hh, mm, ss, ms)
+
+    def _read_3_protocol_information(self):
+        """
+        Reads the header fields detailing the number of runs, sweeps, and the
+        type of protocol used. Create empty sweeps.
         """
+        h = self._header
+
+        # Number of channels, sampling rate (Hz) and acquisition mode
+        # Note: Number of A/D channels will be set to 0 if this is a
+        #       protocol-only file
+        # Note: Number of D/A channels will be adjusted after checking support
+        if self._version < 2:
+            # In (newer versions of) version 1.x, only 2 D/A channels have
+            # full "waveform" support. There are still 4 D/A channels but I
+            # don't understand what the other 2 do.
+            # 1.x versions only seem to have 1 DAC channel, but this is not
+            # supported here.
+            self._n_adc = int(h['nADCNumChannels'])
+            self._n_dac = min(len(h['sDACChannelName']), 2)
+            self._rate = 1e6 / (h['fADCSampleInterval'] * self._n_adc)
+            self._mode = h['nOperationMode']
+        else:
+            # In version 2, there are up to 8 "waveform" D/A channels
+
+            self._n_adc = int(h['sections']['ADC']['length'])
+            self._n_dac = int(h['sections']['DAC']['length'])
+            self._rate = 1e6 / h['protocol']['fADCSequenceInterval']
+            self._mode = h['protocol']['nOperationMode']
+
+        if self._mode not in acquisition_modes:  # pragma: no cover
+            raise NotImplementedError(f'Unknown acquisition mode: {mode}')
+
+        # Protocol files don't have A/D channels by definition
+        if self._is_protocol_file:
+            self._n_adc = 0
+
         # Only episodic stimulation is supported.
         if self._mode != ACMODE_EPISODIC_STIMULATION:  # pragma: no cover
-            return []
-
-        # Start reading
-        h = self._header
+            warnings.warn(
+                'Unsupported acquisition method '
+                + acquisition_modes[self._mode] + '; unable to read D/A'
+                ' channels.')
+
+            # Remaining code is all about reading D/A info for episodic
+            # stimulation, so return
+            self._n_dac = 0
+            return
 
-        # Step 1: Gather information about the protocol
+        # Gather protocol information
         if self._version < 2:
 
             # Before version 2: Sections are fixed length, locations absolute
-            self._numberOfTrials = h['lNumberOfTrials']
-            self._trialStartToStart = h['fTrialStartToStart']
-            self._runsPerTrial = h['lRunsPerTrial']
-            self._runStartToStart = h['fRunStartToStart']
-            self._sweepsPerRun = h['lSweepsPerRun']
-            self._sweepStartToStart = h['fEpisodeStartToStart']
+            self._number_of_trials = h['lNumberOfTrials']
+            self._trial_start_to_start = h['fTrialStartToStart']
+            self._runs_per_trial = h['lRunsPerTrial']
+            self._run_start_to_start = h['fRunStartToStart']
+            self._sweeps_per_run = h['lSweepsPerRun']
+            self._sweep_start_to_start = h['fEpisodeStartToStart']
 
             # Number of samples in a channel for each sweep
             # (Only works for fixed-length, high-speed-osc or episodic)
-            nSam = h['lNumSamplesPerEpisode'] // h['nADCNumChannels']
+            self._samples_per_channel = \
+                h['lNumSamplesPerEpisode'] // h['nADCNumChannels']
 
             def dinfo(index, name):
+                """ Return DAC channel info, ABF1 version. """
                 return h[name][index]
 
             def einfo_exists(index):
-                return True
+                """ Check that epoch info exists for a DAC, ABF1 version. """
+                # Fields always exist for 2 channels, not always set.
+                # But not useful to look at unset ones, so using n_dac instead
+                # of hardcoded 2!
+                return 0 <= index < self._n_dac
 
             def einfo(index):
+                """ Return epoch info for a DAC, ABF1 version. """
                 lo = index * 8
-                hi = index + 8
+                hi = lo + 8
                 for i in range(lo, hi):
                     yield {
                         'type': h['nEpochType'][i],
                         'init_duration': h['lEpochInitDuration'][i],
                         'duration_inc': h['lEpochDurationInc'][i],
                         'init_level': h['fEpochInitLevel'][i],
                         'level_inc': h['fEpochLevelInc'][i],
@@ -952,407 +623,772 @@
         else:
 
             # Version 2 uses variable length sections
             p = h['protocol']
 
             # Trials, runs, sweeps
             # (According to the manual, there should only be 1 trial!)
-            self._numberOfTrials = p['lNumberOfTrials']
-            self._trialStartToStart = p['fTrialStartToStart']
-            self._runsPerTrial = p['lRunsPerTrial']
-            self._runStartToStart = p['fRunStartToStart']
-            self._sweepsPerRun = p['lSweepsPerRun']
-            self._sweepStartToStart = p['fSweepStartToStart']
+            self._number_of_trials = p['lNumberOfTrials']
+            self._trial_start_to_start = p['fTrialStartToStart']
+            self._runs_per_trial = p['lRunsPerTrial']
+            self._run_start_to_start = p['fRunStartToStart']
+            self._sweeps_per_run = p['lSweepsPerRun']
+            self._sweep_start_to_start = p['fSweepStartToStart']
 
             # Number of samples in a channel in a single sweep
-            nSam = p['lNumSamplesPerEpisode'] // h['sections']['ADC']['length']
+            self._samples_per_channel = \
+                p['lNumSamplesPerEpisode'] // h['sections']['ADC']['length']
 
             # Compatibility functions
             def dinfo(index, name):
+                """ Return DAC info, ABF2 version. """
                 return h['listDACInfo'][index][name]
 
             def einfo_exists(index):
+                """ Check that epoch info exists for a DAC, ABF2 version. """
                 return index in h['epochInfoPerDAC']
 
             def einfo(index):
+                """ Return epoch info for a DAC, ABF2 version. """
                 for e in h['epochInfoPerDAC'][index].values():
                     yield {
                         'type': e['nEpochType'],
                         'init_duration': e['lEpochInitDuration'],
                         'duration_inc': e['lEpochDurationInc'],
                         'init_level': e['fEpochInitLevel'],
                         'level_inc': e['fEpochLevelInc'],
                     }
             self._epoch_functions = (dinfo, einfo_exists, einfo)
 
         # If sweepStartToStart == 0, we set it to the duration of a sweep
-        if self._sweepStartToStart == 0:    # pragma: no cover
-            self._sweepStartToStart = nSam / self._rate
+        if self._sweep_start_to_start == 0:    # pragma: no cover
+            self._sweep_start_to_start = self._samples_per_channel / self._rate
 
-        # Step 2: Generate analog signals corresponding to the waveforms
-        # suggested by the 'epochs' in the protocol
-        # User lists are not supported
-        if self._version < 2:   # pragma: no cover
-            if any(self._header['nULEnable']):
-                return []
-        else:   # pragma: no cover
-            for userlist in self._header['listUserListInfo']:
-                if 'nULEnable' in userlist and userlist['nULEnable']:
-                    return []
-                if 'nConditEnable' in userlist and userlist['nConditEnable']:
-                    return []
-        sweeps = []
-
-        # Number of DAC channels = number of channels that can be used
-        #  to output a stimulation
-        nDac = self.protocol_channels()
-        start = 0
-        for iSweep in range(h['lActualSweeps']):
-            sweep = Sweep(nDac)
+        # Create empty sweeps
+        n = h['lActualSweeps']
+        if self._is_protocol_file:
+            n = self._sweeps_per_run
+        self._sweeps = [Sweep() for i in range(n)]
 
-            # Create channels for this sweep
-            for iDac in range(nDac):
-                c = Channel(self)
-                c._name = dinfo(iDac, 'sDACChannelName').strip()
-                c._unit = dinfo(iDac, 'sDACChannelUnits').strip()
-                if self._version < 2:
-                    c._numb = iDac
+        # User lists are not supported for D/A reconstruction
+        # I haven't been able to figure out how you see if a user list is
+        # being used, or which channel is using it. There is an 'enable' field
+        # but that's been 0 in files that definitely used a UserList...
+        # So for now not reading ANY DAC if a userlist even exists.
+        user_lists = False
+        if self._version < 2:   # pragma: no cover
+            user_lists = any(self._header['nULEnable'])
+        else:                   # pragma: no cover
+            user_lists = len(self._header['listUserListInfo']) > 0
+        if user_lists:          # pragma: no cover
+            warnings.warn(
+                'Unsupported acquisition method: episodic with user lists;'
+                ' unable to read D/A channels.')
+            self._n_dac = 0
+            return
+
+        # Get indices of enabled and supported DAC reconstructions
+        supported = {EPOCH_DISABLED, EPOCH_STEPPED}
+        for i_dac in range(self._n_dac):
+            if einfo_exists(i_dac):
+                i = einfo(i_dac)
+                use = False
+
+                # Check for unsupported features (or disabled waveforms/epochs)
+                # Version 1 files can only have two waveform channels
+                if self._version < 2 and i_dac > 1:  # pragma: no cover
+                    source = DAC_DISABLED
                 else:
-                    c._numb = int(dinfo(iDac, 'lDACChannelNameIndex'))
-                c._data = np.ones(nSam) * dinfo(iDac, 'fDACHoldingLevel')
-                c._rate = self._rate
-                c._start = start
-                sweep[iDac] = c
+                    source = dinfo(i_dac, 'nWaveformSource')
+                if source == DAC_EPOCHTABLEWAVEFORM:
+                    # Any epoch types besides disabled/stepped? Then don't use
+                    # Also don't use if exclusively disabled
+                    for e in i:
+                        t = e['type']
+                        if t == EPOCH_STEPPED:
+                            use = True
+                        elif t != EPOCH_DISABLED:  # pragma: no cover
+                            use = False
+                            warnings.warn(
+                                f'Unsupported epoch type: {epoch_types(t)}')
+                            break
+                elif source == DAC_DACFILEWAVEFORM:  # pragma: no cover
+                    # Stimulus file? Then don't use
+                    warnings.warn('Stimulus file D/A channel not supported.')
 
-                # No stimulation info for this channel? Then continue
-                if not einfo_exists(iDac):
-                    continue
+                if use:
+                    self._dac_indices.append(i_dac)
 
-                # Save last sample index
-                i_last = int(nSam * 15625 / 1e6)  # TODO: What's this?
+        # Set true number of D/A outputs
+        self._n_dac = len(self._dac_indices)
 
-                # For each 'epoch' in the stimulation signal
-                for e in einfo(iDac):
-                    kind = e['type']
-                    if kind not in epoch_types:
-                        raise NotImplementedError(
-                            'Unknown epoch type: ' + str(kind))
+    def _read_4_ad_conversion_factors(self):
+        """ Calculate the factors to convert any integer data to float. """
+        self._adc_factors = []
+        self._adc_offsets = []
+        h = self._header
+        if self._version < 2:
+            for i in range(self._n_adc):
+                j = h['nADCSamplingSeq'][i]
+
+                # Multiplier
+                f = (
+                    h['fInstrumentScaleFactor'][j]
+                    * h['fADCProgrammableGain'][j]
+                    * h['lADCResolution']
+                    / h['fADCRange'])
+
+                # Signal conditioner used?
+                if h['nSignalType'] != 0:   # pragma: no cover
+                    # Cover pragma: Don't have appropriate test file
+                    f *= h['fSignalGain'][j]
 
-                    if kind == EPOCH_DISABLED:
+                # Additional gain?
+                if h['nTelegraphEnable'][j]:
+                    f *= h['fTelegraphAdditGain'][j]
 
-                        continue
+                # Set final gain factor
+                self._adc_factors.append(1 / f)
 
-                    elif kind == EPOCH_STEPPED:
+                # Shift
+                s = h['fInstrumentOffset'][j]
 
-                        dur = e['init_duration']
-                        inc = e['duration_inc']
-                        i1 = i_last
-                        i2 = i_last + dur + iSweep * inc
-                        if i2 > nSam:
-                            # The protocol may extend beyond the number of
-                            # samples in the recording
-                            i2 = nSam
-                        level = e['init_level'] + e['level_inc'] * iSweep
-                        c._data[i1:i2] = level * np.ones(len(range(i2 - i1)))
-                        i_last += dur
-                        if i_last > nSam:
-                            # The protocol may extend beyond the number of
-                            # samples in the recording
-                            break
+                # Signal conditioner used?
+                if h['nSignalType'] != 0:   # pragma: no cover
+                    # Cover pragma: Don't have appropriate test file
+                    s -= h['fSignalOffset'][j]
 
-                    else:  # pragma: no cover
+                # Set final offset
+                self._adc_offsets.append(s)
 
-                        log = logging.getLogger(__name__)
-                        log.warning(
-                            'Unsupported epoch type: ' + epoch_types(kind))
-                        continue
-
-            sweeps.append(sweep)
-            start += self._sweepStartToStart
-        return sweeps
+        else:
 
-    def _read_sweeps(self):
-        """
-        Reads the data from an ABF file and returns a list of sweeps
-        """
-        header = self._header
-        version = self._version
-        nc = self._nc
+            a = h['listADCInfo']
+            p = h['protocol']
+            for i in range(self._n_adc):
+                # Multiplier
+                f = (
+                    a[i]['fInstrumentScaleFactor']
+                    * a[i]['fADCProgrammableGain']
+                    * p['lADCResolution']
+                    / p['fADCRange'])
+
+                # Signal conditioner used?
+                if h.get('nSignalType', 0) != 0:  # pragma: no cover
+                    # Cover pragma: Don't have appropriate test file
+                    f *= a[i]['fSignalGain']
+
+                # Additional gain?
+                if a[i]['nTelegraphEnable']:
+                    f *= a[i]['fTelegraphAdditGain']
+
+                # Set final gain factor
+                self._adc_factors.append(1 / f)
+
+                # Shift
+                s = a[i]['fInstrumentOffset']
+
+                # Signal conditioner used?
+                if h.get('nSignalType', 0) != 0:  # pragma: no cover
+                    # Cover pragma: Don't have appropriate test file
+                    s -= a[i]['fSignalOffset']
+
+                # Set final offset
+                self._adc_offsets.append(s)
+
+    def _read_5_ad_data(self):
+        """ Reads the A/D data and appends it to the list of sweeps. """
+
+        h = self._header
 
         # Sampling rate is constant for all sweeps and channels
         # TODO: This won't work for 2-rate protocols
         rate = self._rate
 
         # Get binary integer format
-        dt = np.dtype('i2') if header['nDataFormat'] == 0 else np.dtype('f4')
+        dt = np.dtype('i2') if h['nDataFormat'] == 0 else np.dtype('f4')
 
         # Get number of channels, create a numpy memory map
-        if version < 2:
+        if self._version < 2:
             # Old files, get info from fields stored directly in header
-            o = header['lDataSectionPtr'] * BLOCKSIZE \
-                + header['nNumPointsIgnored'] * dt.itemsize
-            n = header['lActualAcqLength']
+            o = h['lDataSectionPtr'] * BLOCKSIZE \
+                + h['nNumPointsIgnored'] * dt.itemsize
+            n = h['lActualAcqLength']
         else:
             # New files, get info from appropriate header section
-            o = header['sections']['Data']['index'] * BLOCKSIZE
-            n = header['sections']['Data']['length']
+            o = h['sections']['Data']['index'] * BLOCKSIZE
+            n = h['sections']['Data']['length']
         data = np.memmap(self._filepath, dt, 'r', shape=(n,), offset=o)
 
         # Load list of sweeps (Sweeps are called 'episodes' in ABF < 2)
-        if version < 2:
-            n = header['lSynchArraySize']
-            o = header['lSynchArrayPtr'] * BLOCKSIZE
+        if self._version < 2:
+            n = h['lSynchArraySize']
+            o = h['lSynchArrayPtr'] * BLOCKSIZE
         else:
-            n = header['sections']['SynchArray']['length']
-            o = header['sections']['SynchArray']['index'] * BLOCKSIZE
+            n = h['sections']['SynchArray']['length']
+            o = h['sections']['SynchArray']['index'] * BLOCKSIZE
         if n > 0:
             dt = [(str('offset'), str('i4')), (str('len'), str('i4'))]
-            sdata = np.memmap(self._filepath, dt, 'r', shape=(n), offset=o)
+            sweep_data = np.memmap(
+                self._filepath, dt, 'r', shape=(n,), offset=o)
         else:   # pragma: no cover
             # Cover pragma: Don't have appropriate test file
-            sdata = np.empty((1), dt)
-            sdata[0]['len'] = data.size
-            sdata[0]['offset'] = 0
+            sweep_data = np.empty((1), dt)
+            sweep_data[0]['len'] = data.size
+            sweep_data[0]['offset'] = 0
 
-        # Get data
-        pos = 0
-
-        # Data structure
-        sweeps = []
+        # Number of sweeps must equal n
+        if n != h['lActualSweeps']:
+            raise NotImplementedError(
+                'Unable to read file with different sizes per sweep.')
 
-        # Time-offset at start of sweep
-        start = sdata[0]['offset'] / rate
-        for j in range(sdata.size):
+        # Time-offset at start of first sweep
+        start = sweep_data[0]['offset'] / rate
 
-            # Create a new sweep
-            sweep = Sweep(nc)
+        # Get data
+        pos = 0
+        for i_sweep, sdat in enumerate(sweep_data):
 
             # Get the number of data points
-            size = sdata[j]['len']
+            size = sdat['len']
 
             # Calculate the correct size for variable-length event mode
             if self._mode == ACMODE_VARIABLE_LENGTH_EVENTS:  # pragma: no cover
                 # Cover pragma: Only episodic stimulus is supported.
-                if version < 2:
-                    f = float(header['fSynchTimeUnit'])
+                if self._version < 2:
+                    f = float(h['fSynchTimeUnit'])
                 else:
-                    f = float(header['protocol']['fSynchTimeUnit'])
+                    f = float(h['protocol']['fSynchTimeUnit'])
                 if f != 0:
                     size /= f
 
             # Get a memory map to the relevant part of the data
             part = data[pos: pos + size]
             pos += size
-            part = part.reshape((part.size // nc, nc)).astype('f')
+            part = part.reshape(
+                (part.size // self._n_adc, self._n_adc)).astype('f')
 
             # If needed, reformat the integers
-            if header['nDataFormat'] == 0:
+            if h['nDataFormat'] == 0:
                 # Data given as integers? Convert to floating point
-                for i in range(nc):
-                    factor, offset = self._get_conversion_factors(i)
-                    part[:, i] *= factor
-                    part[:, i] += offset
 
-            # Create channel
+                for i in range(self._n_adc):
+                    part[:, i] *= self._adc_factors[i]
+                    part[:, i] += self._adc_offsets[i]
+
+            # Get start in other modes
             if self._mode != ACMODE_EPISODIC_STIMULATION:  # pragma: no cover
                 # All modes except episodic stimulation
-                start = sdata[j]['offset'] / rate
+                start = data['offset'] / rate
 
-            for i in range(nc):
+            # Create and populate sweep
+            sweep = self._sweeps[i_sweep]
+            for i in range(self._n_adc):
                 c = Channel(self)
-                c._data = part[:, i]
-                if version < 2:
-                    c._name = str(header['sADCChannelName'][i])
-                    c._unit = str(header['sADCUnits'][i])
-                    c._numb = int(header['nADCPtoLChannelMap'][i])
+                c._data = part[:, i]    # Actually store the data
+                c._rate = rate
+                c._start = start
+
+                if self._version < 2:
+                    j = h['nADCSamplingSeq'][i]
+
+                    c._name = h['sADCChannelName'][j]
+                    c._index = int(h['nADCPtoLChannelMap'][j])
+                    c._unit = self._unit(h['sADCUnits'][j])
 
                     # Get telegraphed info
                     def get(field):
                         try:
-                            return float(header[field][i])
+                            return float(h[field][j])
                         except KeyError:
                             return None
 
                     if get('nTelegraphEnable'):
                         c._type = int(get('nTelegraphMode') or 0)
                         c._cm = get('fTelegraphMembraneCap')
                         c._rs = get('fTelegraphAccessResistance')
                         c._lopass = get('fTelegraphFilter')
 
                     # Updated low-pass cutoff
-                    if header['nSignalType'] != 0:  # pragma: no cover
+                    if h['nSignalType'] != 0:  # pragma: no cover
                         # Cover pragma: Don't have appropriate test file
                         # If a signal conditioner is used, the cutoff frequency
                         # is an undescribed "complex function" of both low-pass
                         # settings...
                         c._lopass = None
 
                 else:
-
-                    c._name = str(header['listADCInfo'][i]['ADCChNames'])
-                    c._unit = str(header['listADCInfo'][i]['ADCChUnits'])
-                    c._numb = int(header['listADCInfo'][i]['nADCNum'])
+                    c._name = h['listADCInfo'][i]['ADCChNames']
+                    c._index = int(h['listADCInfo'][i]['nADCNum'])
+                    c._unit = self._unit(h['listADCInfo'][i]['ADCChUnits'])
 
                     # Get telegraphed info
-                    if header['listADCInfo'][i]['nTelegraphEnable']:
-                        c._type = int(
-                            header['listADCInfo'][i]['nTelegraphMode'])
+                    if h['listADCInfo'][i]['nTelegraphEnable']:
+                        c._type = int(h['listADCInfo'][i]['nTelegraphMode'])
                         c._cm = float(
-                            header['listADCInfo'][i]['fTelegraphMembraneCap'])
+                            h['listADCInfo'][i]['fTelegraphMembraneCap'])
                         c._rs = float(
-                            header['listADCInfo'][i][
-                                'fTelegraphAccessResistance'])
+                            h['listADCInfo'][i]['fTelegraphAccessResistance'])
                         c._lopass = float(
-                            header['listADCInfo'][i]['fTelegraphFilter'])
+                            h['listADCInfo'][i]['fTelegraphFilter'])
 
                     # Updated low-pass cutoff
-                    if 'nSignalType' in header['protocol']:  # pragma: no cover
+                    if 'nSignalType' in h['protocol']:  # pragma: no cover
                         # Cover pragma: Don't have appropriate test file
-                        if header['protocol']['nSignalType'] != 0:
+                        if h['protocol']['nSignalType'] != 0:
                             # If a signal conditioner is used, the cutoff
                             # frequency is an undescribed "complex function" of
                             # both low-pass settings...
                             c._lopass = None
-                c._rate = rate
-                c._start = start
-                sweep[i] = c
+
+                sweep._channels.append(c)
 
             if self._mode == ACMODE_EPISODIC_STIMULATION:
                 # Increase time according to sweeps in episodic stim. mode
-                start += self._sweepStartToStart
+                start += self._sweep_start_to_start
+
+    def _read_6_da_reconstructions(self):
+        """
+        Convert supported D/A waveforms to channels.
+
+        Only works for episodic stimulation, with step protocols and no
+        user lists.
+
+        The resulting analog signal has the same size as the recorded
+        signals, so not always the full length of the protocol!
+
+        """
+        dinfo, einfo_exists, einfo = self._epoch_functions
+
+        ns = self._samples_per_channel
+        start = 0
+        for i_sweep, sweep in enumerate(self._sweeps):
+            for i_dac in self._dac_indices:
+
+                # Create a channel
+                c = Channel(self)
+                c._name = dinfo(i_dac, 'sDACChannelName')
+                if self._version < 2:
+                    c._index = i_dac
+                else:
+                    c._index = int(dinfo(i_dac, 'lDACChannelNameIndex'))
+                c._data = np.ones(ns) * dinfo(i_dac, 'fDACHoldingLevel')
+                c._rate = self._rate
+                c._start = start
+                c._unit = self._unit(dinfo(i_dac, 'sDACChannelUnits'))
+
+                # Find start of first epoch. This is defined as being at t=0
+                # but axon likes to add some samples before the first and after
+                # the last epoch. We can find out the number of samples using
+                # a procedure found in ABF v1's _GetHoldingLength()
+                if self._is_protocol_file:
+                    i2 = 0
+                else:
+                    i2 = ns // 64  # ABFH_HOLDINGFRACTION = 64
+                    i2 -= i2 % self._n_adc
+                    if (i2 < self._n_adc):  # pragma: no cover
+                        i2 = self._n_adc
+
+                # For each 'epoch' in the stimulation signal
+                for e in einfo(i_dac):
+                    if e['type'] == EPOCH_STEPPED:
+                        dur = e['init_duration']
+                        inc = e['duration_inc']
+                        i1 = i2
+                        i2 += dur + i_sweep * inc
+                        level = e['init_level'] + e['level_inc'] * i_sweep
+                        c._data[i1:i2] = level * np.ones(len(range(i2 - i1)))
+
+                # Store channel
+                sweep._channels.append(c)
+
+            # Update start for next sweep
+            start += self._sweep_start_to_start
+
+    def __getitem__(self, key):
+        return self._sweeps[key]
+
+    def __iter__(self):
+        return iter(self._sweeps)
 
-            # Store sweep
-            sweeps.append(sweep)
+    def __len__(self):
+        return len(self._sweeps)
+
+    def _channel_id(self, channel_id):
+        """ Checks an int or str channel id and returns a valid int. """
+        if len(self._sweeps) == 0:  # pragma: no cover
+            raise KeyError(f'Channel {channel_id} not found (empty file).')
 
-        return sweeps
+        # Handle string
+        if isinstance(channel_id, str):
+            int_id = self._ad_names[channel_id]  # Bubble KeyError to user
+        else:
+            int_id = int(channel_id)    # Propagate TypeError
+            if int_id < 0 or int_id >= self._n_adc:
+                raise IndexError(f'channel_id out of range: {channel_id}')
+
+        return int_id
+
+    def channel(self, channel_id, join_sweeps=False):
+        # Docstring in SweepSource
+        channel_id = self._channel_id(channel_id)
+        time, data = [], []
+        for i, sweep in enumerate(self._sweeps):
+            time.append(sweep[channel_id].times())
+            data.append(sweep[channel_id].values())
+        if join_sweeps:
+            return (np.concatenate(time), np.concatenate(data))
+        return time, data
 
-    def _set_conversion_factors(self):
+    def channel_count(self):
+        # Docstring in SweepSource
+        return self._n_adc
+
+    def channel_names(self, index=None):
+        # Docstring in SweepSource
+        if index is None:
+            return list(self._ad_names.keys())
+        return list(self._ad_names.keys())[index]
+
+    def channel_units(self, index=None):
+        # Docstring in SweepSource
+        if index is None:
+            return list(self._ad_units)
+        return self._ad_units[index]
+
+    def _da_id(self, output_id):
         """
-        Calculates the conversion factors to convert integer data from the ABF
-        file to floats.
+        Checks an int or str D/A channel id and returns a valid int.
+
+        Note: The integer here is from 0 to da_count(), so not equal to the
+        channel :meth:`index()` shown in pclamp.
         """
-        self._adc_factors = []
-        self._adc_offsets = []
-        h = self._header
-        if self._version < 2:
-            for i in range(self._nc):
-                # Multiplier
-                f = (
-                    h['fInstrumentScaleFactor'][i]
-                    * h['fADCProgrammableGain'][i]
-                    * h['lADCResolution']
-                    / h['fADCRange'])
+        if len(self._sweeps) == 0:  # pragma: no cover
+            raise KeyError(f'D/A output {output_id} not found (empty file).')
 
-                # Signal conditioner used?
-                if h['nSignalType'] != 0:   # pragma: no cover
-                    # Cover pragma: Don't have appropriate test file
-                    f *= h['fSignalGain'][i]
+        # Handle string
+        if isinstance(output_id, str):
+            int_id = self._da_names[output_id]  # Propagate KeyError to user
+        else:
+            int_id = int(output_id)  # Propagate TypeError
+            if int_id < 0 or int_id >= self._n_dac:
+                raise IndexError(f'output_id out of range: {output_id}')
+
+        return int_id
+
+    def da(self, output_id, join_sweeps=False):
+        # Docstring in SweepSource
+        channel_id = self._n_adc + self._da_id(output_id)
+        time, data = [], []
+        for i, sweep in enumerate(self._sweeps):
+            time.append(sweep[channel_id].times())
+            data.append(sweep[channel_id].values())
+        if join_sweeps:
+            return (np.concatenate(time), np.concatenate(data))
+        return time, data
 
-                # Additional gain?
-                if h['nTelegraphEnable'][i]:
-                    f *= h['fTelegraphAdditGain'][i]
+    def da_count(self):
+        # Docstring in SweepSource
+        return self._n_dac
 
-                # Set fina gain factor
-                self._adc_factors.append(1.0 / f)
+    def da_names(self, index=None):
+        # Docstring in SweepSource
+        if index is None:
+            return list(self._da_names.keys())
+        return list(self._da_names.keys())[index]
 
-                # Shift
-                s = h['fInstrumentOffset'][i]
+    def da_protocol(self, output_id=None, tu='ms', vu='mV', cu='pA',
+                    n_digits=9, include_initial_holding=False):
+        """
+        See :meth:`myokit.formats.SweepSource.da_protocol()`.
 
-                # Signal conditioner used?
-                if h['nSignalType'] != 0:   # pragma: no cover
-                    # Cover pragma: Don't have appropriate test file
-                    s -= h['fSignalOffset'][i]
+        This implementation adds a keyword argument ``include_initial_holding``
+        that lets you switch between the declared protocol (``False``) and the
+        protocol as actually implemented (``True``). In the latter case, a
+        short holding time is added before the first epoch in every sweep.
+        """
 
-                # Set final offset
-                self._adc_offsets.append(s)
+        # Check the output id. This also raises an error if no supported D/A
+        # channels are present.
+        output_id = self._da_id(output_id or 0)
 
+        # Get the index in dinfo
+        i_dac = self._dac_indices[output_id]
+        dinfo, einfo_exists, einfo = self._epoch_functions
+
+        # Get the time and data conversion factors
+        units = myokit.units
+        tf = myokit.Unit.conversion_factor(units.s, tu)
+        if myokit.Unit.can_convert(self._da_units[output_id], units.V):
+            df = myokit.Unit.conversion_factor(self._da_units[output_id], vu)
+        elif myokit.Unit.can_convert(
+                self._da_units[output_id], units.A):  # pragma: no cover
+            df = myokit.Unit.conversion_factor(self._da_units[output_id], cu)
+        else:  # pragma: no cover
+            # Not a voltage or current? Then don't convert
+            df = 1
+        tf, df = float(tf), float(df)
+
+        # Axon has the annoying habit of adding some extra holding at the start
+        # We can include this if we want. See _read_6 for details.
+        if self._is_protocol_file:
+            offset = 0
         else:
+            offset = self._samples_per_channel // 64
+            offset -= offset % self._n_adc
+            if (offset < self._n_adc):  # pragma: no cover
+                # Don't have a test for this, but this is part of the
+                # established procedure.
+                offset = self._n_adc
+            offset /= self._rate
 
-            a = h['listADCInfo']
-            p = h['protocol']
-            for i in range(self._nc):
-                # Multiplier
-                f = (
-                    a[i]['fInstrumentScaleFactor']
-                    * a[i]['fADCProgrammableGain']
-                    * p['lADCResolution']
-                    / p['fADCRange'])
+        # Holding level (converted and rounded)
+        holding = round(df * dinfo(i_dac, 'fDACHoldingLevel'), n_digits)
 
-                # Signal conditioner used?
-                if 'nSignalType' in h:  # pragma: no cover
-                    # Cover pragma: Don't have appropriate test file
-                    if h['nSignalType'] != 0:
-                        f *= a[i]['fSignalGain']
+        # Create protocol
+        p = myokit.Protocol()
+        start = 0
+        next_start = self._sweep_start_to_start
+        for i_sweep in range(self._sweeps_per_run):
+            # Start of sweep: secret event at holding potential
+            if include_initial_holding:
+                e_start = round(tf * start, n_digits)
+                e_length = round(tf * offset, n_digits)
+                p.schedule(holding, e_start, e_length)
+                start += offset
 
-                # Additional gain?
-                if a[i]['nTelegraphEnable']:
-                    f *= a[i]['fTelegraphAdditGain']
+            for e in einfo(i_dac):
+                if e['type'] == EPOCH_STEPPED:
+                    dur = e['init_duration'] / self._rate
+                    inc = e['duration_inc'] / self._rate
+                    duration = dur + i_sweep * inc
+                    level = e['init_level'] + e['level_inc'] * i_sweep
+
+                    e_level = round(df * level, n_digits)
+                    e_start = round(tf * start, n_digits)
+                    e_length = round(tf * duration, n_digits)
+                    p.schedule(e_level, e_start, e_length)
 
-                # Set final gain factor
-                self._adc_factors.append(1.0 / f)
+                    start += duration
+                # Note: Only other type can be EPOCH_DISABLED at this point
 
-                # Shift
-                s = a[i]['fInstrumentOffset']
+            # End of sweep: event at holding potential
+            e_start = round(tf * start, n_digits)
+            e_length = round(tf * (next_start - start), n_digits)
+            p.schedule(holding, e_start, e_length)
+            start = next_start
+            next_start += self._sweep_start_to_start
 
-                # Signal conditioner used?
-                if 'nSignalType' in h:  # pragma: no cover
+        return p
+
+    def da_units(self, index=None):
+        # Docstring in SweepSource
+        if index is None:
+            return list(self._da_units)
+        return self._da_units[index]
+
+    def equal_length_sweeps(self):
+        # Always true for ABF
+        return True
+
+    def filename(self):
+        """ Returns this ABF file's filename. """
+        return self._filename
+
+    def log(self, join_sweeps=False, use_names=False, include_da=True):
+        # Docstring in SweepSource
+
+        # Create log, return if no sweeps or channels
+        log = myokit.DataLog()
+        ns = len(self._sweeps)
+        if ns == 0 or (self._n_adc + self._n_dac) == 0:  # pragma: no cover
+            return log
+
+        # Get channel names
+        if use_names:
+            nc = self._n_adc + (self._n_dac if include_da else 0)
+            names = [c.name() for c in self._sweeps[0][:nc]]
+        else:
+            names = [f'{i}.channel' for i in range(self._n_adc)]
+            if include_da:
+                names += [f'{i}.da' for i in range(self._n_dac)]
+
+        # Gather data and return
+        t = self._sweeps[0][0].times()
+        if not join_sweeps:
+            log['time'] = t
+            for i_sweep, sweep in enumerate(self._sweeps):
+                for channel, name in zip(sweep, names):
+                    log[name, i_sweep] = channel.values()
+        else:
+            log['time'] = np.concatenate(
+                [t + i * self._sweep_start_to_start for i in range(ns)])
+            for i_channel, name in enumerate(names):
+                log[name] = np.concatenate(
+                    [sweep[i_channel].values() for sweep in self._sweeps])
+        log.set_time_key('time')
+        return log
+
+    def matplotlib_figure(self):
+        """ Creates and returns a matplotlib figure with this file's data. """
+        import matplotlib.pyplot as plt
+        f = plt.figure()
+        plt.suptitle(self.filename())
+
+        # Plot AD channels
+        ax = plt.subplot(2, 1, 1)
+        ax.set_title('Measured data')
+        times = None
+        for sweep in self._sweeps:
+            for channel in sweep[:self._n_adc]:
+                if times is None:
+                    times = channel.times()
+                plt.plot(times, channel.values())
+
+        # Plot DA channels
+        n = self._n_dac
+        ax = [plt.subplot(2, n, n + 1 + i) for i in range(n)]
+        for sweep in self._sweeps:
+            for i, channel in enumerate(sweep[self._n_adc:]):
+                ax[i].set_title(channel.name())
+                ax[i].plot(times, channel.values())
+
+        return f
+
+    def meta_str(self, show_header=False):
+        """
+        Returns a multi-line string with meta data about this file.
+
+        The optional argument ``show_header`` can be used to add the full
+        header contents to the output.
+        """
+        out = []
+
+        # File info
+        if self._is_protocol_file:
+            out.append(f'Axon Protocol File: {self._filename}')
+        else:
+            out.append(f'Axon Binary File: {self._filename}')
+        out.append(f'ABF Format version {self._version_str}')
+        out.append(f'Recorded on: {self._datetime}')
+
+        # AProtocol info
+        out.append(
+            f'Acquisition mode: {self._mode}: {acquisition_modes[self._mode]}')
+        if self._number_of_trials:
+            out.append(
+                f'Protocol set for {self._number_of_trials} trials,'
+                f' spaced {self._trial_start_to_start}s apart.')
+            out.append(
+                f'    with {self._runs_per_trial} runs per trial,'
+                f' spaced {self._run_start_to_start}s apart.')
+            out.append(
+                f'     and {self._sweeps_per_run} sweeps per run,'
+                f' spaced {self._sweep_start_to_start}s apart.')
+        else:   # pragma: no cover
+            out.append('Protocol data could not be determined.')
+        out.append(f'Sampling rate: {self._rate} Hz')
+
+        # Channel info
+        if len(self._sweeps) > 0:
+
+            # A/D recordings
+            for i, c in enumerate(self._sweeps[0][:self._n_adc]):
+                out.append(f'A/D Channel {i}: "{c._name}"')
+                if c._type:  # pragma: no cover
+                    # Cover pragma: Don't have appropriate test file
+                    out.append(f'  Type: {type_mode_names[c._type]}')
+                out.append(f'  Unit: {c._unit}')
+                if c._lopass:
+                    out.append(f'  Low-pass filter: {c._lopass} Hz')
+                if c._cm:
+                    out.append(f'  Cm (telegraphed): {c._cm} pF')
+                if c._rs:   # pragma: no cover
                     # Cover pragma: Don't have appropriate test file
-                    if h['nSignalType'] != 0:
-                        s -= a[i]['fSignalOffset']
+                    out.append(f'  Rs (telegraphed): {c._rs}')
 
-                # Set final offset
-                self._adc_offsets.append(s)
+            # Reconstructed D/A outputs
+            for i, c in enumerate(self._sweeps[0][self._n_adc:]):
+                out.append(f'D/A Channel {i}: "{c._name}"')
+                if c._type:  # pragma: no cover
+                    # Cover pragma: Don't have appropriate test file
+                    out.append('  Type: {type_mode_names[c._type]}')
+                out.append(f'  Unit: {c._unit}')
+
+        # Add full header info
+        if show_header:
+            if self._strings:
+                dict_to_string(out, 'Strings', {'strings': self._strings})
+            dict_to_string(out, 'file header', self._header)
+
+        return '\n'.join(out)
+
+    def path(self):
+        """ Returns the path to the underlying ABF file. """
+        return self._filepath
+
+    def sweep_count(self):
+        # Docstring in SweepSource
+        return len(self._sweeps)
+
+    def time_unit(self):
+        # Docstring in SweepSource
+        # For ABF, this is always seconds
+        return myokit.units.s
+
+    def _unit(self, unit_string):
+        """ Parses a unit string and returns a :class:`myokit.Unit`. """
+        try:
+            return self._unit_cache[unit_string]
+        except KeyError:
+            unit = myokit.parse_unit(unit_string.replace(MU, 'u'))
+            self._unit_cache[unit_string] = unit
+            return unit
+
+    def version(self):
+        """ Returns a string representation of this file's version number. """
+        return self._version_str
 
 
 class Sweep:
     """
-    Represents a single sweep (also called an 'episode')
+    Represents a single sweep (also called an *episode*).
 
-    A sweep is represented as a fixed-size list of channels.
+    Each sweep contains a fixed number of :class:`channels<Channel>`.
     """
-    def __init__(self, n):
-        super().__init__()
-        n = int(n)
-        if n < 0:   # pragma: no cover
-            raise ValueError('Number channels cannot be negative.')
-        self._nc = n    # Number of channels
-        self._channels = [None] * n
+    def __init__(self):
+        self._channels = []
 
     def __getitem__(self, key):
         return self._channels[key]  # Handles slices etc.
 
     def __iter__(self):
         return iter(self._channels)
 
     def __len__(self):
-        return self._nc
-
-    def __setitem__(self, key, value):
-        if type(key) == slice:
-            raise NotImplementedError(
-                'Assignment with slices is not supported.')
-        self._channels[key] = value
+        return len(self._channels)
 
 
 class Channel:
     """
-    Represents an analog signal for a single channel.
+    Represents a signal for a single channel.
 
-    To obtain this channel's formatted data, use times() and trace()
+    To obtain its data, use :meth:`times` and :meth:`values`.
     """
     def __init__(self, parent_file):
-        super().__init__()
         self._parent_file = parent_file  # The abf file this channel is from
         self._type = TYPE_UNKNOWN   # Type of recording
 
         # This channel's name
         self._name = None
 
-        # This channel's index (see note below)
-        self._numb = None
+        # This channel's index in the file. This is basically a name, and does
+        # not correspond to e.g. its index in the ADC/DAC info or its index in
+        # the sweep's list of channels.
+        self._index = None
 
         # The units this channel's data is in
         self._unit = None
 
         # The raw data points
         self._data = None
 
@@ -1367,64 +1403,91 @@
 
         # The reported access resistance
         self._rs = None
 
         # The reported low-pass filter cut-off frequency
         self._lopass = None
 
-        # Note that the channel indices are not necessarily sequential! So a
-        # file with 2 channels can have indices 0 and 3.
+    def index(self):
+        """ Returns the index set for this channel. """
+        return self._index
 
     def name(self):
-        """
-        Returns the name set for this channel.
-        """
+        """ Returns the name set for this channel. """
         return self._name
 
-    def number(self):
-        """
-        Returns the channel index used by pClamp. Note that this does not
-        necessarily equal its index in the Python sweep data!
-        """
-        return self._numb
-
     def __str__(self):
-        return 'Channel(' + str(self._numb) + ' "' + str(self._name) \
-            + '"); ' + str(len(self._data)) + ' points sampled at ' \
-            + str(self._rate) + 'Hz, starts at t=' + str(self._start)
+        return (
+            f'Channel({self._index} "{self._name}"); {len(self._data)} points'
+            f' sampled at {self._rate}Hz, starts at t={self._start}.')
 
     def times(self):
-        """
-        Returns a copy of the values on the time axis.
-        """
+        """ Returns a copy of the values on the time axis. """
         n = len(self._data)
-        f = 1.0 / self._rate
+        f = 1 / self._rate
         return np.arange(self._start, self._start + n * f, f)[0:n]
 
+    def unit(self):
+        """ Returns the units this channel is in. """
+        return self._unit
+
     def values(self):
-        """
-        Returns a copy of the values on the data axis.
-        """
-        return np.array(self._data, copy=True)
+        """ Returns a copy of the values on the data axis. """
+        return np.copy(self._data)
+
+
+def dict_to_string(out, name, d, tab=''):
+    """ Used by AbfFile.info(). """
+    m = max(0, 38 - len(tab) - int(0.1 + len(name) / 2))
+    out.append(f'{tab}{"-" * m}  {name}  {"-" * m}')
+    for n, v in d.items():
+        n = str(n)
+        if type(v) == dict:
+            dict_to_string(out, n, v, f'{tab}  ')
+        elif type(v) == list:
+            list_to_string(out, n, v, tab)
+        else:
+            out.append(f'{tab}{n}: {v}')
+    m = max(0, 80 - 2 * len(tab))
+    out.append(f'{tab}{m * "-"}')
+
+
+def list_to_string(out, name, d, tab=''):
+    """ Used by AbfFile.info(). """
+    for index, item in enumerate(d):
+        n = f'{name}[{index}]'
+        if type(item) == dict:
+            dict_to_string(out, n, item, tab)
+        elif type(item) == list:    # pragma: no cover
+            # Cover pragma: Don't have appropriate test file
+            list_to_string(out, n, item, tab)
+        else:
+            out.append(f'{tab}{n}: {item}')
 
 
 # Some python struct types:
 #   f   float
 #   h   short
 #   i   int
 #   s   string
 # Size of block alignment in ABF Files
 BLOCKSIZE = 512
 
 
+# A mu, sometimes found in unit strings
+MU = '\u00b5'
+
+
 # Header fields for versions 1 and 2
 # Stored as (key, offset, format) where format corresponds to a struct
 #  unpacking format as documented in:
 #  http://docs.python.org/library/struct.html#format-characters
-headerFields = {
+HEADER_FIELDS = {
+    # Note that a lot of the groups in the version 1 header start with obsolete
+    # fields, followed later by their newer equivalents.
     1: [
         ('fFileSignature', 0, '4s'),       # Coarse file version indication
         # Group 1, File info and sizes
         ('fFileVersionNumber', 4, 'f'),    # Version number as float
         ('nOperationMode', 8, 'h'),        # Acquisition mode
         ('lActualAcqLength', 10, 'i'),
         ('nNumPointsIgnored', 14, 'h'),
@@ -1513,33 +1576,32 @@
         ('x_fEpochInitLevel', 1464, '10f'),
         ('x_fEpochLevelInc', 1504, '10f'),
         ('x_nEpochInitDuration', 1544, '10h'),
         ('x_nEpochDurationInc', 1564, '10h'),
         ('nDigitalHolding', 1584, 'h'),
         ('nDigitalInterEpisode', 1586, 'h'),
         ('nDigitalValue', 2588, '10h'),
-        ('lDACFilePtr', 2048, '2i'),            # Pointer to protocol?
+        ('lDACFilePtr', 2048, '2i'),
         ('lDACFileNumEpisodes', 2056, '2i'),
         ('fDACCalibrationFactor', 2074, '4f'),
         ('fDACCalibrationOffset', 2090, '4f'),
         ('nWaveformEnable', 2296, '2h'),
         ('nWaveformSource', 2300, '2h'),
         ('nInterEpisodeLevel', 2304, '2h'),
         ('nEpochType', 2308, '20h'),       # 2 CMD channels with 10 values each
         ('fEpochInitLevel', 2348, '20f'),
         ('fEpochLevelInc', 2428, '20f'),
         ('lEpochInitDuration', 2508, '20i'),
         ('lEpochDurationInc', 2588, '20i'),
-        # Group 10, DAC Output file
+        # Group 10, DAC Output file (Stimulus file)
         ('fDACFileScale', 2708, 'd'),
         ('fDACFileOffset', 2716, 'd'),
         ('lDACFileEpisodeNum', 2724, 'i'),
         ('nDACFileADCNum', 2732, '2h'),
-        # 256 * 2char = utf8? or 2 strings?
-        ('sDACFilePath', 2736, '256s' * 2),
+        ('sDACFilePath', 2736, '256s' * 2),     # Two strings
         # Group 11,
         # Group 12, User list parameters
         ('nULEnable', 3360, '4h'),
         ('nULParamToVary', 3368, '4h'),
         ('nULParamValueList0', 3376, '256s' * 4),
         ('nULRepeat', 4400, '4h'),
         # Group 13,
@@ -1550,15 +1612,15 @@
         # Group 18, Application version data
         # Group 19
         # Group 20
         # Group 21 Skipped
         # Group 22
         # Group 23 Post-processing
         # Group 24 Legacy stuff
-        # Group 6 again?
+        # Group 6 extended
         ('nTelegraphEnable', 4512, '16h'),
         ('fTelegraphAdditGain', 4576, '16f'),
     ],
     2: [
         ('fFileSignature', 0, '4s'),       # Coarse file version indication
         ('fFileVersionNumber', 4, '4b'),   # Version number as 4 signed chars
         ('uFileInfoSize', 8, 'I'),
@@ -1578,15 +1640,15 @@
         ('uModifierNameIndex', 68, 'I'),
         ('uProtocolPathIndex', 72, 'I')
     ]
 }
 
 
 # ABF2 File sections
-abf2FileSections = [
+ABF2_FILE_SECTIONS = [
     'Protocol',
     'ADC',
     'DAC',
     'Epoch',
     'ADCPerDAC',
     'EpochPerDAC',
     'UserList',
@@ -1601,24 +1663,24 @@
     'SynchArray',
     'Annotation',
     'Stats',
 ]
 
 
 # ABF2 Fields in the tag section
-TagInfoDescription = [
+ABF2_TAG_INFO_DESCRIPTION = [
     ('lTagTime', 'i'),
     ('sComment', '56s'),
     ('nTagType', 'h'),
     ('nVoiceTagNumber_or_AnnotationIndex', 'h'),
 ]
 
 
 # ABF2 Fields in the protocol section
-protocolFields = [
+ABF2_PROTOCOL_FIELDS = [
     ('nOperationMode', 'h'),                # 0
     ('fADCSequenceInterval', 'f'),          # 2
     ('bEnableFileCompression', 'b'),        # 6
     ('sUnused1', '3s'),                     # 7
     ('uFileCompressionRatio', 'I'),         # 10
     ('fSynchTimeUnit', 'f'),                # 14
     ('fSecondsPerRun', 'f'),                # 18
@@ -1686,15 +1748,15 @@
     ('nDigitizerTotalDigitalOuts', 'h'),
     ('nDigitizerSynchDigitalOuts', 'h'),
     ('nDigitizerType', 'h'),
 ]
 
 
 # ABF2 Fields in the ADC section
-ADCFields = [
+ABF2_ADC_FIELDS = [
     ('nADCNum', 'h'),
     ('nTelegraphEnable', 'h'),
     ('nTelegraphInstrument', 'h'),
     ('fTelegraphAdditGain', 'f'),
     ('fTelegraphFilter', 'f'),
     ('fTelegraphMembraneCap', 'f'),
     ('nTelegraphMode', 'h'),
@@ -1718,15 +1780,15 @@
     ('nStatsChannelPolarity', 'h'),
     ('lADCChannelNameIndex', 'i'),
     ('lADCUnitsIndex', 'i'),
 ]
 
 
 # ABF2 Fields in the DAC section
-DACFields = [
+ABF2_DAC_FIELDS = [
     ('nDACNum', 'h'),
     ('nTelegraphDACScaleFactorEnable', 'h'),
     ('fInstrumentHoldingLevel', 'f'),
     ('fDACScaleFactor', 'f'),
     ('fDACHoldingLevel', 'f'),
     ('fDACCalibrationFactor', 'f'),
     ('fDACCalibrationOffset', 'f'),
@@ -1765,27 +1827,29 @@
     ('fMembTestPostSettlingTimeMS', 'f'),
     ('nLeakSubtractADCIndex', 'h'),
     ('sUnused', '124s'),
 ]
 
 
 # ABF2 Fields in the DAC-Epoch section
-EpochInfoPerDACFields = [
+ABF2_EPOCH_INFO_PER_DAC_FIELD = [
     ('nEpochNum', 'h'),
     ('nDACNum', 'h'),
     ('nEpochType', 'h'),
     ('fEpochInitLevel', 'f'),
     ('fEpochLevelInc', 'f'),
     ('lEpochInitDuration', 'i'),
     ('lEpochDurationInc', 'i'),
     ('lEpochPulsePeriod', 'i'),
     ('lEpochPulseWidth', 'i'),
     ('sUnused', '18s'),
 ]
-UserListFields = [
+
+# ABF2 User list fields
+ABF2_USER_LIST_FIELDS = [
     ('nListNum', 'h'),
     ('nULEnable', 'h'),
     ('nULParamToVary', 'h'),
     ('nULRepeat', 'h'),
     ('lULParamValueListIndex', 'i'),
     ('sUnused', '52s'),
 ]
@@ -1856,14 +1920,20 @@
     0: 'Unknown',
     1: 'Voltage clamp',
     2: 'Current clamp',
     4: 'Current clamp zero',
 }
 
 
+# DAC waveform types
+DAC_DISABLED = 0
+DAC_EPOCHTABLEWAVEFORM = 1  # Epochs
+DAC_DACFILEWAVEFORM = 2     # Stimulus file
+
+
 # User list parameter to vary
 '''
 CONDITNUMPULSES 0
 CONDITBASELINEDURATION 1
 CONDITBASELINELEVEL 2
 CONDITSTEPDURATION 3
 CONDITSTEPLEVEL 4
```

### Comparing `myokit-1.35.0/myokit/formats/axon/_atf.py` & `myokit-1.35.1/myokit/formats/axon/_atf.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import re
 
 import numpy as np
 
 from collections import OrderedDict
 
+import myokit
 
 # Format used for any text
 _ENC = 'ascii'
 
 
 class AtfFile:
     """
@@ -26,97 +27,99 @@
     Access to the data is provided using a dict-like interface: to iterate over
     the file's keys use :meth:`iterkeys`, to select a value use
     ``atf_file['key']``. All iterators return the keys stored in the order they
     were listed in the ATF file.
     """
     def __init__(self, filename):
         # The path to the file and its basename
-        self._file = os.path.abspath(filename)
+        self._path = os.path.abspath(filename)
         self._filename = os.path.basename(filename)
 
         # A version string
-        self._version = None
+        self._version_str = None
 
         # A (multi-line) string containing meta-data found in this file
         self._meta = None
 
         # An ordered dict with key-value pairs. The first key is time.
         self._data = None
 
         # Read data
         self._read()
 
-    def filename(self):
-        """
-        Returns this ATF's filename.
-        """
-        return self._file
-
     def __getitem__(self, key):
         return self._data.__getitem__(key)
 
     def __iter__(self):
-        """
-        Iterates over all data arrays in this ATF file.
-        """
         return iter(self._data)
 
+    def __len__(self):
+        return len(self._data)
+
+    def filename(self):
+        """ Returns this ATF's filename. """
+        return self._filename
+
+    def info(self):
+        """ Returns this ATF's header/meta data. """
+        # Deprecated since 2023-07-12
+        import warnings
+        warnings.warn(
+            'The method `info` is deprecated. Please use `meta_str` instead.')
+        return self.meta_str()
+
     def items(self):
-        """
-        Iterates over all key-value pairs in this ATF file's data.
-        """
+        """ Returns an iterator over all ``(key, value)`` pairs. """
         return iter(self._data.items())
 
     def keys(self):
-        """
-        Iterates over all keys in this ATF file's data.
-        """
+        """ Returns an iterator over all keys in this ATF. """
         return iter(self._data.keys())
 
-    def values(self):
-        """
-        Iterates over all values in this ATF file's data.
-        """
-        return iter(self._data.values())
-
-    def __len__(self):
-        """
-        Returns the number of records in this file.
-        """
-        return len(self._data)
-
-    def info(self):
-        """
-        Returns the header/meta data found in this file.
-        """
-        return self._meta
-
-    def myokit_log(self):
+    def log(self):
         """
         Returns this file's time series data as a :class:`myokit.DataLog`.
         """
-        import myokit
         log = myokit.DataLog()
         if len(self._data) > 0:
             log.set_time_key(next(iter(self._data.keys())))
         for k, v in self._data.items():
             log[k] = v
         return log
 
-    def _read(self):
+    def meta_str(self, verbose=True):
         """
-        Reads the data in the file.
+        Returns this ATF's header data as an unstructured multi-line string.
+
+        Note that the ``verbose`` argument doesn't do anything, but provides
+        compatibility with similar methods in other files.
         """
-        with open(self._file, 'rb') as f:
+        return self._meta
+
+    def myokit_log(self):
+        """ Deprecated alias of :meth:`log`. """
+        # Deprecated since 2023-06-22
+        import warnings
+        warnings.warn(
+            'The method `myokit_log` is deprecated. Please use `log` instead.')
+        return self.log()
+
+    def path(self):
+        """ Returns the path to this ATF file. """
+        return self._path
+
+    def _read(self):
+        """ Reads the data in this file. """
+        with open(self._path, 'rb') as f:
             # Check version
             line = f.readline().decode(_ENC)
             line_index = 1
             if line[:3] != 'ATF':
                 raise Exception('Unrecognised file type.')
-            self._version = line[3:].strip()
+            self._version_str = line[3:].strip()
 
             # Read number of header lines, number of fields
             line = f.readline().decode(_ENC)
             line_index += 1
             nh, nf = [int(x) for x in line.split()]
 
             # Read header data
@@ -127,17 +130,16 @@
             raw = []    # Fallback
             key_value_pairs = True
             for i in range(nh):
                 line = f.readline().decode(_ENC).strip()
                 line_index += 1
                 if line[0] != '"' or line[-1] != '"':
                     raise Exception(
-                        'Invalid header on line ' + str(line_index)
-                        + ': expecting lines wrapped in double quotation'
-                        ' marks "like this".')
+                        f'Invalid header on line f{line_index}: expecting '
+                        f' lines wrapped in double quotes ("like this").')
                 line = line[1:-1].strip()
                 raw.append(line)
                 if key_value_pairs:
                     try:
                         k, v = line.split('=')
                         key.append(k.strip())
                         val.append(v.strip())
@@ -166,16 +168,16 @@
             # First and last delim must be empty (i.e. line starts and ends
             # with '"')
             if delims[0] != '' or delims[-1] != '':
                 raise Exception('Unable to parse column headers.')
             delims = delims[1:-1]
             if len(delims) + 1 != nf:
                 raise Exception(
-                    'Unable to parse column headers: Expected ' + str(nf)
-                    + ' headers, found ' + str(len(delims) + 1) + '.')
+                    f'Unable to parse column headers: Expected {nf} headers,'
+                    f' found {len(delims) + 1}.')
             commas = ',' in delims[0]
             for delim in delims:
                 if commas != (',' in delim):
                     raise Exception('Mixed delimiters are not supported.')
 
             # Read column headers
             keys = []
@@ -189,50 +191,51 @@
                     keys.append(line[a + 1:b])
                     a = line.index('"', b + 1)
             except ValueError:
                 pass
             if len(keys) != nf:     # pragma: no cover
                 # This should have been picked up above
                 raise Exception(
-                    'Unable to parse column headers: Expected ' + str(nf)
-                    + ' headers, found ' + str(len(keys)) + '.')
+                    f'Unable to parse column headers: Expected {nf} headers,'
+                    f' found {len(keys)}.')
 
             # Read data
             data = []
             for key in keys:
                 col = []
                 data.append(col)
                 self._data[key] = col
             sep = ',' if commas else None
             for line in f:
                 line_index += 1
                 line = line.decode(_ENC).strip()
                 vals = line.split(sep)
                 if len(vals) != nf:
                     raise Exception(
-                        'Invalid data on line ' + str(line_index)
-                        + ': expecting ' + str(nf) + ' fields, found'
-                        + ' ' + str(len(vals)) + '.')
+                        f'Invalid data on line f{line_index}: expecting {nf}'
+                        f' fields, found {len(vals)}.')
                 vals = [float(x) for x in vals]
                 for k, d in enumerate(vals):
                     data[k].append(d)
 
+    def values(self):
+        """ Returns an iterator over all values in this ATF. """
+        return iter(self._data.values())
+
     def version(self):
-        """
-        Returns the file type version of this ATF file (as a string).
-        """
-        return self._version
+        """ Returns a string representation of this file's version number. """
+        return self._version_str
 
 
 def load_atf(filename):
     """
     Reads an ATF file and returns its data as a :class:`myokit.DataLog`.
     """
     filename = os.path.expanduser(filename)
-    return AtfFile(filename).myokit_log()
+    return AtfFile(filename).log()
 
 
 def save_atf(log, filename, fields=None):
     """
     Saves the :class:`myokit.DataLog` ``log`` to ``filename`` in ATF format.
 
     ATF requires that the times in the log be regularly spaced.
@@ -302,20 +305,20 @@
 
     # Write file
     with open(filename, 'wb') as f:
         # Write version number
         f.write(('ATF 1.0' + eol).encode(_ENC))
 
         # Write number of header lines, number of fields
-        f.write((str(nh) + delim + str(nf) + eol).encode(_ENC))
+        f.write(f'{nh}{delim}{nf}{eol}'.encode(_ENC))
         for k, v in header:
-            f.write(('"' + str(k) + '=' + str(v) + '"' + eol).encode(_ENC))
+            f.write(f'"{k}={v}"{eol}'.encode(_ENC))
 
         # Write field names
-        f.write((delim.join(['"' + k + '"' for k in keys]) + eol).encode(_ENC))
+        f.write((delim.join([f'"{k}"' for k in keys]) + eol).encode(_ENC))
 
         # Write data
         for i in range(nd):
             f.write((
                 delim.join([myokit.float.str(next(d)) for d in data]) + eol
             ).encode(_ENC))
```

### Comparing `myokit-1.35.0/myokit/formats/axon/_importer.py` & `myokit-1.35.1/myokit/formats/axon/_importer.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     This :class:`Importer <myokit.formats.Importer>` can import protocols from
     files in Axon Binary Format.
     """
 
     def supports_protocol(self):
         return True
 
-    def protocol(self, filename, channel=None):
+    def protocol(self, filename, channel=0):
         """
         Attempts to load the protocol from the file at ``filename``.
 
         If specified, the channel index ``channel`` will be used to select
         which channel in the AbfFile to convert to a protocol
         """
         from myokit.formats.axon import AbfFile
         abf = AbfFile(filename)
-        return abf.myokit_protocol(channel)
+        return abf.da_protocol(channel)
```

### Comparing `myokit-1.35.0/myokit/formats/cellml/__init__.py` & `myokit-1.35.1/myokit/formats/cellml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cellml/_ewriter.py` & `myokit-1.35.1/myokit/formats/cellml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cellml/_exporter.py` & `myokit-1.35.1/myokit/formats/cellml/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cellml/_importer.py` & `myokit-1.35.1/myokit/formats/cellml/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cellml/v1/__init__.py` & `myokit-1.35.1/myokit/formats/cellml/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cellml/v1/_api.py` & `myokit-1.35.1/myokit/formats/cellml/v1/_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cellml/v1/_parser.py` & `myokit-1.35.1/myokit/formats/cellml/v1/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cellml/v1/_writer.py` & `myokit-1.35.1/myokit/formats/cellml/v1/_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cellml/v2/__init__.py` & `myokit-1.35.1/myokit/formats/cellml/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cellml/v2/_api.py` & `myokit-1.35.1/myokit/formats/cellml/v2/_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cellml/v2/_parser.py` & `myokit-1.35.1/myokit/formats/cellml/v2/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cellml/v2/_writer.py` & `myokit-1.35.1/myokit/formats/cellml/v2/_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/channelml/_importer.py` & `myokit-1.35.1/myokit/formats/channelml/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cpp/__init__.py` & `myokit-1.35.1/myokit/formats/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cuda/__init__.py` & `myokit-1.35.1/myokit/formats/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cuda/_ewriter.py` & `myokit-1.35.1/myokit/formats/cuda/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cuda/_exporter.py` & `myokit-1.35.1/myokit/formats/cuda/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/cuda/template/kernel.cu` & `myokit-1.35.1/myokit/formats/cuda/template/kernel.cu`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/easyml/__init__.py` & `myokit-1.35.1/myokit/formats/easyml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/easyml/_ewriter.py` & `myokit-1.35.1/myokit/formats/easyml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/easyml/_exporter.py` & `myokit-1.35.1/myokit/formats/easyml/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/html/_exporter.py` & `myokit-1.35.1/myokit/formats/html/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/html/_flatten.py` & `myokit-1.35.1/myokit/formats/html/_flatten.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/latex/__init__.py` & `myokit-1.35.1/myokit/formats/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/latex/_ewriter.py` & `myokit-1.35.1/myokit/formats/latex/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/latex/_exporter.py` & `myokit-1.35.1/myokit/formats/latex/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/mathml/__init__.py` & `myokit-1.35.1/myokit/formats/mathml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/mathml/_ewriter.py` & `myokit-1.35.1/myokit/formats/mathml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/mathml/_parser.py` & `myokit-1.35.1/myokit/formats/mathml/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/matlab/__init__.py` & `myokit-1.35.1/myokit/formats/matlab/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/matlab/_ewriter.py` & `myokit-1.35.1/myokit/formats/matlab/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/matlab/_exporter.py` & `myokit-1.35.1/myokit/formats/matlab/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/matlab/template/constants.m` & `myokit-1.35.1/myokit/formats/matlab/template/constants.m`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/matlab/template/main.m` & `myokit-1.35.1/myokit/formats/matlab/template/main.m`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/matlab/template/model.m` & `myokit-1.35.1/myokit/formats/matlab/template/model.m`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/opencl/__init__.py` & `myokit-1.35.1/myokit/formats/opencl/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/opencl/_ewriter.py` & `myokit-1.35.1/myokit/formats/opencl/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/opencl/_exporter.py` & `myokit-1.35.1/myokit/formats/opencl/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/opencl/template/cable.c` & `myokit-1.35.1/myokit/formats/opencl/template/cable.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/opencl/template/kernel.cl` & `myokit-1.35.1/myokit/formats/opencl/template/kernel.cl`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/opencl/template/minilog.py` & `myokit-1.35.1/myokit/formats/opencl/template/minilog.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/opencl/template/plot.py` & `myokit-1.35.1/myokit/formats/opencl/template/plot.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/python/__init__.py` & `myokit-1.35.1/myokit/formats/python/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/python/_ewriter.py` & `myokit-1.35.1/myokit/formats/python/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/python/_exporter.py` & `myokit-1.35.1/myokit/formats/python/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/python/template/sim.py` & `myokit-1.35.1/myokit/formats/python/template/sim.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/sbml/__init__.py` & `myokit-1.35.1/myokit/formats/sbml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/sbml/_api.py` & `myokit-1.35.1/myokit/formats/sbml/_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/sbml/_importer.py` & `myokit-1.35.1/myokit/formats/sbml/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/sbml/_parser.py` & `myokit-1.35.1/myokit/formats/sbml/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/stan/__init__.py` & `myokit-1.35.1/myokit/formats/stan/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/stan/_ewriter.py` & `myokit-1.35.1/myokit/formats/stan/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/stan/_exporter.py` & `myokit-1.35.1/myokit/formats/stan/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/stan/template/cell.stan` & `myokit-1.35.1/myokit/formats/stan/template/cell.stan`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/sympy/__init__.py` & `myokit-1.35.1/myokit/formats/sympy/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/sympy/_ereader.py` & `myokit-1.35.1/myokit/formats/sympy/_ereader.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/sympy/_ewriter.py` & `myokit-1.35.1/myokit/formats/sympy/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/formats/xml/_exporter.py` & `myokit-1.35.1/myokit/formats/xml/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/gui/__init__.py` & `myokit-1.35.1/myokit/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/gui/datablock_viewer.py` & `myokit-1.35.1/myokit/gui/datablock_viewer.py`

 * *Files 7% similar despite different names*

```diff
@@ -190,36 +190,60 @@
         # Graph controls
         self._graph_clear_button = QtWidgets.QPushButton('Clear graphs')
         self._graph_clear_button.pressed.connect(self.action_clear_graphs)
 
         # Variable selection
         self._variable_select = QtWidgets.QComboBox()
         self._variable_select.activated.connect(self.event_variable_selected)
-        self._variable_select.setMinimumWidth(120)
+        self._variable_select.setMinimumWidth(160)
 
         # Colormap selection
         self._colormap = next(iter(myokit.ColorMap.names()))
         self._colormap_select = QtWidgets.QComboBox()
         for cmap in myokit.ColorMap.names():
             self._colormap_select.addItem(cmap)
         self._colormap_select.activated.connect(self.event_colormap_selected)
         self._colormap_select.setMinimumWidth(120)
 
+        self._colormap_lower_label = QtWidgets.QLabel('Range')
+        self._colormap_lower_label.setMaximumWidth(50)
+        self._colormap_lower_label.setAlignment(
+            Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignVCenter)
+        self._colormap_lower_field = AutoFloatField()
+        self._colormap_lower_field.setMaxLength(6)
+        self._colormap_lower_field.setMaximumWidth(80)
+        self._colormap_lower_field.editingFinished.connect(
+            self.event_variable_selected)
+
+        self._colormap_upper_label = QtWidgets.QLabel('to')
+        self._colormap_upper_label.setMaximumWidth(20)
+        self._colormap_upper_label.setAlignment(
+            Qt.AlignmentFlag.AlignHCenter | Qt.AlignmentFlag.AlignVCenter)
+        self._colormap_upper_field = AutoFloatField()
+        self._colormap_upper_field.setMaxLength(6)
+        self._colormap_upper_field.setMaximumWidth(80)
+        self._colormap_upper_field.editingFinished.connect(
+            self.event_variable_selected)
+
         # Control layout
         self._control_layout = QtWidgets.QHBoxLayout()
         self._control_layout.addWidget(self._play_button)
         self._control_layout.addWidget(self._frame_label)
         self._control_layout.addWidget(self._frame_field)
         self._control_layout.addWidget(self._time_label)
         self._control_layout.addWidget(self._time_field)
         self._control_layout.addWidget(self._rate_label)
         self._control_layout.addWidget(self._rate_field)
         self._control_layout.addWidget(self._graph_clear_button)
         self._control_layout.addWidget(self._variable_select)
         self._control_layout.addWidget(self._colormap_select)
+        self._control_layout.addWidget(self._colormap_lower_label)
+        self._control_layout.addWidget(self._colormap_lower_field)
+        self._control_layout.addWidget(self._colormap_upper_label)
+        self._control_layout.addWidget(self._colormap_upper_field)
 
         # Graph area
         self._graph_area = GraphArea()
         self._graph_area.mouse_moved.connect(self.event_graph_mouse_move)
         self._graph_area.setMouseTracking(True)
         self._graph_area.setCursor(Qt.CursorShape.CrossCursor)
 
@@ -470,14 +494,17 @@
             self.action_stop_timer()
         else:
             self.action_start_timer()
 
     def action_set_colormap(self, name):
         """
         Loads the ColorMap specified by ``name``.
+
+        If data is loaded, this will also call :meth:`action_set_variable` to
+        update the video frames.
         """
         name = str(name)
         if not myokit.ColorMap.exists(name):
             return  # Silent return?
         # Set colormap
         self._colormap = name
         # Update colormap controls
@@ -493,29 +520,39 @@
             self._colorbar_pixmap.convertFromImage(image)
             self._colorbar_item.setPixmap(self._colorbar_pixmap)  # qt5
             self.action_set_variable(self._variable)
 
     def action_set_variable(self, var):
         """
         Loads the variable specified by the name ``var`` into the main display.
+
+        This method is also responsible for converting the data into frames to
+        be displayed on the video widget.
         """
         if self._data is None:
             return
         self._variable = str(var)
-        self._variable_select.setCurrentIndex(self._variable_select.findText(
-            self._variable))
+        self._variable_select.setCurrentIndex(
+            self._variable_select.findText(self._variable))
         self.action_pause_timer()
         self._video_frames = self._data.images(
-            self._variable, colormap=self._colormap)
+            self._variable,
+            self._colormap,
+            self._colormap_lower_field.value(),
+            self._colormap_upper_field.value()
+        )
         self.action_set_frame(self._video_iframe)
         self.action_depause_timer()
 
     def action_set_frame(self, frame):
         """
         Move to a specific frame.
+
+        This method updates the display to show a video frame created by an
+        earlier call to :meth:`action_set_variable`.
         """
         # Check frame index
         nt, ny, nx = self._data.shape()
         frame = int(frame)
         if frame < 0 or frame >= nt:
             frame = 0
         # Update
@@ -547,17 +584,15 @@
 
     def action_stop_timer(self):
         self._timer_paused = False
         self._timer.stop()
         self._play_button.setIcon(self._play_icon_play)
 
     def closeEvent(self, event=None):
-        """
-        Called when window is closed.)
-        """
+        # Called when window is closed.
         self.save_config()
         if event:
             event.accept()
 
     def create_menu(self):
         """
         Creates this widget's menu.
@@ -695,17 +730,16 @@
                 z = F.format(z)
             except IndexError:
                 z = '?'
             x, y = F.format(x), F.format(y)
             self._label_cursor.setText('(' + x + ', ' + y + ', ' + z + ')')
 
     def keyPressEvent(self, e):
-        """
-        Catch key presses?
-        """
+        # A key has been pressed
+
         if e.key() == Qt.Key.Key_Space:
             self.action_start_stop()
 
     def load_config(self):
         """
         Loads the user configuration from an ini file.
         """
@@ -849,16 +883,15 @@
         self._video_scene.clear()
         self._video_scene.resize(nx, ny)
         self._video_view.resizeEvent()
         self._video_iframe = 0
 
         # Add empty video item to video scene
         self._video_pixmap = QtGui.QPixmap(nx, ny)
-        self._video_item = QtWidgets.QGraphicsPixmapItem(
-            self._video_pixmap)
+        self._video_item = QtWidgets.QGraphicsPixmapItem(self._video_pixmap)
         self._video_scene.addItem(self._video_item)
 
         # Update colormap scene
         nx, ny = self._colorbar_width, self._colorbar_height
         self._colorbar_scene.clear()
         self._colorbar_scene.resize(nx, ny)
         self._colorbar_view.resizeEvent()
@@ -959,14 +992,21 @@
             title = os.path.basename(self._file) + ' - ' + title
         self.setWindowTitle(title)
 
 
 class VideoScene(QtWidgets.QGraphicsScene):
     """
     Color data display scene.
+
+    Note that, despite the name, this item does not manage the conversion from
+    data to the image. The actual drawing happens by calling ``setPixmap`` on a
+    ``QGraphicsPixmapItem`` that gets added to this scene.
+
+    See :meth:`DataBlockViewer.action_set_variable()` and
+    :meth:`DataBlockViewer.action_set_frame()`.
     """
     # Signals
     # Somebody moved the mouse
     # Attributes: cell x, cell y
     mouse_moved = QtCore.Signal(int, int)
     # Single click
     # Attributes: cell x, cell y
@@ -980,49 +1020,41 @@
         self.setBackgroundBrush(QtGui.QColor(192, 192, 192))
         self._w = None
         self._h = None
         self._p = None
         self.resize(1, 1)
 
     def mousePressEvent(self, event):
-        """
-        Single-click
-        """
+        # Single-click event
         if event.button() == Qt.MouseButton.LeftButton:
-            if event.modifiers() == Qt.KeyBoardModifier.NoModifier:
+            if event.modifiers() == Qt.KeyboardModifier.NoModifier:
                 p = event.scenePos()
                 x, y = int(p.x()), int(p.y())
                 if x >= 0 and x < self._w and y >= 0 and y < self._h:
                     self.single_click.emit(x, y)
                     return
 
     def mouseDoubleClickEvent(self, event):
-        """
-        Double-click
-        """
+        # Double-click event
         if event.button() == Qt.MouseButton.LeftButton:
-            if event.modifiers() == Qt.KeyBoardModifier.NoModifier:
+            if event.modifiers() == Qt.KeyboardModifier.NoModifier:
                 p = event.scenePos()
                 x, y = int(p.x()), int(p.y())
                 if x >= 0 and x < self._w and y >= 0 and y < self._h:
                     self.double_click.emit(x, y)
                     return
 
     def mouseMoveEvent(self, event):
-        """
-        Show mouse position in status bar
-        """
+        # The mouse has moved!
         p = event.scenePos()
         x, y = int(p.x()), int(p.y())
         self.mouse_moved.emit(x, y)
 
     def resize(self, w, h):
-        """
-        Resizes the scene to match the given dimensions.
-        """
+        """ Resize the scene to match the given dimensions. """
         self._w = float(w)
         self._h = float(h)
         self.setSceneRect(0, 0, self._w, self._h)
 
 
 class VideoView(QtWidgets.QGraphicsView):
     """
@@ -1077,17 +1109,16 @@
             xr = min(xr, yr)
 
         # Scale and center
         self.scale(xr, yr)
         self.centerOn(rect.center())
 
     def resizeEvent(self, event=None):
-        """
-        Called when the view is resized.
-        """
+        # Called when the view is resized.
+
         # Tell others a resize is happening
         # (This is used to pause the video playback)
         self.resize_event.emit()
         # Schedule delayed (and grouped) resize action
         self._resize_timer.start(100)
 
     def _resize_timeout(self, event=None):
@@ -1361,7 +1392,45 @@
         return QtCore.QSize(250, 250)
 
     def sizePolicy(self):
         """
         Tells Qt that this widget shout expand.
         """
         return QtCore.QSizePolicy.Expanding
+
+
+class AutoFloatField(QtWidgets.QLineEdit):
+    """
+    A QLineEdit that requires floats as input, but will show "(Auto)" when a
+    non-float is entered and return ``None`` as its value.
+    """
+    def __init__(self, parent=None):
+        super().__init__(parent)
+
+        # Colors
+        self._color_ok = QtGui.QTextCharFormat().foreground().color().getRgb()
+        self._color_auto = (127, 127, 127)
+        self._auto_text = '(Auto)'
+
+        # Show text
+        self.editingFinished.connect(self._autofy)
+        self._autofy()
+
+    def _autofy(self):
+        """ Put (Auto) if not valid """
+        if self.value() is None:
+            self.setText(self._auto_text)
+            c = self._color_auto
+        else:
+            c = self._color_ok
+        self.setStyleSheet(f'color: rgb({c[0]}, {c[1]}, {c[2]})')
+
+    def focusInEvent(self, event):
+        super().focusInEvent(event)
+        QtCore.QTimer.singleShot(0, self.selectAll)
+
+    def value(self):
+        try:
+            return float(super().text())
+        except ValueError:
+            return None
+
```

### Comparing `myokit-1.35.0/myokit/gui/datalog_viewer.py` & `myokit-1.35.1/myokit/gui/datalog_viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import sys
 import traceback
 
 from myokit.gui import QtWidgets, QtGui, QtCore, Qt
 
 import myokit
 import myokit.gui
+import myokit.gui.progress
 import myokit.formats.axon
 import myokit.formats.wcp
 
 # Matplotlib (must be imported _after_ gui has had chance to set backend)
 import matplotlib
 import matplotlib.figure
 from myokit.gui import matplotlib_backend as backend
@@ -75,24 +76,26 @@
 # License
 LICENSE = myokit.LICENSE_HTML
 
 # File filters
 FILTER_ABF = 'ABF files (*.abf *.pro)'
 FILTER_ATF = 'ATF files (*.atf)'
 FILTER_CSV = 'CSV files (*.csv)'
-FILTER_MAT = 'MAT files (*.mat)'
-FILTER_TXT = 'TXT files (*.txt)'
+FILTER_MAT = 'Matlab files (*.mat)'
+FILTER_DAT = 'PatchMaster files (*.dat)'
+FILTER_TXT = 'Text files (*.txt)'
 FILTER_WCP = 'WCP files (*.wcp)'
 FILTER_ZIP = 'Zipped DataLog files (*.zip)'
 FILTER_ANY = 'All files (*.*)'
-FILTER_ALL = 'Data files (*.abf *.csv *.mat *.pro *.txt *.wcp *.zip)'
+FILTER_ALL = 'Data files (*.abf *.csv *.dat *.mat *.pro *.txt *.wcp *.zip)'
 FILTER_LIST = ';;'.join([
     FILTER_ALL,
     FILTER_ABF,
     FILTER_CSV,
+    FILTER_DAT,
     FILTER_MAT,
     FILTER_TXT,
     FILTER_WCP,
     FILTER_ZIP,
     FILTER_ANY,
 ])
 
@@ -137,14 +140,15 @@
         self.load_config()
 
         # File-loading methods
         self._load_actions = {
             '.abf': self.load_abf_file,
             '.atf': self.load_atf_file,
             '.csv': self.load_datalog,
+            '.dat': self.load_dat_file,
             '.pro': self.load_abf_file,
             '.txt': self.load_txt_file,
             '.wcp': self.load_wcp_file,
             '.zip': self.load_datalog,
         }
         if has_scipy:
             self._load_actions['.mat'] = self.load_mat_file
@@ -180,14 +184,26 @@
 
         # Delete tab
         if tab is not None:
             tab.deleteLater()
         gc.collect()
         del tab
 
+    def action_first_var(self):
+        """ Select the first variable in the current file. """
+        tab = self._tabs.currentWidget()
+        if tab:
+            tab.first()
+
+    def action_last_var(self):
+        """ Select the last variable in the current file. """
+        tab = self._tabs.currentWidget()
+        if tab:
+            tab.last()
+
     def action_license(self):
         """
         Displays this program's licensing information.
         """
         QtWidgets.QMessageBox.about(self, TITLE, LICENSE)
 
     def action_open(self):
@@ -291,28 +307,44 @@
         self._menu_view.addAction(self._tool_next_file)
         self._tool_prev_file = QtGui.QAction('Previous file', self)
         self._tool_prev_file.setShortcut('Ctrl+PgUp')
         self._tool_prev_file.setStatusTip('Select the previous open file')
         self._tool_prev_file.triggered.connect(self.action_prev_file)
         self._tool_prev_file.setEnabled(False)
         self._menu_view.addAction(self._tool_prev_file)
+        # View > ----
+        self._menu_view.addSeparator()
         # View > Next variable
         self._tool_next_var = QtGui.QAction('Next variable', self)
         self._tool_next_var.setShortcut('PgDown')
         self._tool_next_var.setStatusTip('Show the next variable')
         self._tool_next_var.triggered.connect(self.action_next_var)
         self._tool_next_var.setEnabled(False)
         self._menu_view.addAction(self._tool_next_var)
         # View > Previous var
         self._tool_prev_var = QtGui.QAction('Previous variable', self)
         self._tool_prev_var.setShortcut('PgUp')
         self._tool_prev_var.setStatusTip('Show the previous variable')
         self._tool_prev_var.triggered.connect(self.action_prev_var)
         self._tool_prev_var.setEnabled(False)
         self._menu_view.addAction(self._tool_prev_var)
+        # View > First variable
+        self._tool_first_var = QtGui.QAction('First variable', self)
+        self._tool_first_var.setShortcut('Home')
+        self._tool_first_var.setStatusTip('Show the first variable')
+        self._tool_first_var.triggered.connect(self.action_first_var)
+        self._tool_first_var.setEnabled(False)
+        self._menu_view.addAction(self._tool_first_var)
+        # View > Last var
+        self._tool_last_var = QtGui.QAction('Last variable', self)
+        self._tool_last_var.setShortcut('End')
+        self._tool_last_var.setStatusTip('Show the last variable')
+        self._tool_last_var.triggered.connect(self.action_last_var)
+        self._tool_last_var.setEnabled(False)
+        self._menu_view.addAction(self._tool_last_var)
         # Help menu
         self._menu_help = self._menu.addMenu('&Help')
         # Help > About
         self._tool_about = QtGui.QAction('&About', self)
         self._tool_about.setStatusTip('View information about this program.')
         self._tool_about.triggered.connect(self.action_about)
         self._menu_help.addAction(self._tool_about)
@@ -378,43 +410,76 @@
         except KeyError:
             QtWidgets.QMessageBox.critical(
                 self, TITLE, 'File format not recognized: ' + ext)
             return
         action(filename)
 
     def load_abf_file(self, filename):
-        """
-        Loads an abf file.
-        """
+        """ Loads an ABF file. """
         try:
             abf = myokit.formats.axon.AbfFile(filename)
         except Exception:
             e = traceback.format_exc()
             QtWidgets.QMessageBox.critical(self, TITLE, e)
             return
         self._path = os.path.dirname(filename)
         self._tabs.addTab(AbfTab(self, abf), os.path.basename(filename))
 
     def load_atf_file(self, filename):
-        """
-        Loads an ATF file.
-        """
+        """ Loads an ATF file. """
         try:
             atf = myokit.formats.axon.AtfFile(filename)
         except Exception:
             e = traceback.format_exc()
             QtWidgets.QMessageBox.critical(self, TITLE, e)
             return
         self._path = os.path.dirname(filename)
         self._tabs.addTab(AtfTab(self, atf), os.path.basename(filename))
 
+    def load_dat_file(self, filename):
+        """ Loads a PatchMaster dat file. """
+
+        pbar = myokit.gui.progress.ProgressBar(
+            self, 'Loading groups and series')
+        pbar.show()
+        reporter = pbar.reporter()
+        reporter.enter()
+
+        flag = QtCore.QEventLoop.ProcessEventsFlag.ExcludeUserInputEvents
+        QtWidgets.QApplication.processEvents(flag)
+
+        try:
+            with myokit.formats.heka.PatchMasterFile(filename) as f:
+                n = sum([len(list(g.complete_series())) for g in f])
+                i = 0
+                stop = False
+                for group in f:
+                    for series in group.complete_series():
+                        self._tabs.addTab(
+                            PatchMasterTab(self, series),
+                            f'{group.label()} {series.label()}')
+                        i += 1
+                        if not reporter.update(i / n):
+                            stop = True
+                            break
+                        QtWidgets.QApplication.processEvents(flag)
+                    if stop:
+                        break
+                self._path = os.path.dirname(filename)
+        except Exception:
+            e = traceback.format_exc()
+            QtWidgets.QMessageBox.critical(self, TITLE, e)
+            return
+        finally:
+            reporter.exit()
+            pbar.close()
+            pbar.deleteLater()
+
     def load_datalog(self, filename):
-        """
-        Loads a DataLog from csv or zip file.
-        """
+        """ Loads a DataLog from csv or zip file. """
         try:
             if filename[-4:].lower() == '.csv':
                 log = myokit.DataLog.load_csv(filename)
             else:
                 log = myokit.DataLog.load(filename)
             if log.time_key is None:
                 raise Exception('Log must contain a suitable time variable.')
@@ -439,31 +504,27 @@
             QtWidgets.QMessageBox.critical(self, TITLE, e)
             return
         self._path = os.path.dirname(filename)
         name = os.path.basename(filename)
         self._tabs.addTab(MatTab(self, mat, name), name)
 
     def load_txt_file(self, filename):
-        """
-        Loads a csv file.
-        """
+        """ Loads a text file. """
         try:
             data = np.loadtxt(filename)
         except Exception:
             e = traceback.format_exc()
             QtWidgets.QMessageBox.critical(self, TITLE, e)
             return
         self._path = os.path.dirname(filename)
         name = os.path.basename(filename)
         self._tabs.addTab(TxtTab(self, data, name), name)
 
     def load_wcp_file(self, filename):
-        """
-        Loads a wcp file.
-        """
+        """ Loads a WinWCP file. """
         try:
             wcp = myokit.formats.wcp.WcpFile(filename)
         except Exception:
             e = traceback.format_exc()
             QtWidgets.QMessageBox.critical(self, TITLE, e)
             return
         self._path = os.path.dirname(filename)
@@ -502,161 +563,191 @@
     def fileTabChangeEvent(self, index):
         """
         Different file tab selected.
         """
         if index >= 0:
             tab = self._tabs.widget(index)
             if tab.count() > 1:
-                self._tool_prev_var.setEnabled(True)
+                self._tool_first_var.setEnabled(True)
+                self._tool_last_var.setEnabled(True)
                 self._tool_next_var.setEnabled(True)
+                self._tool_prev_var.setEnabled(True)
                 return
+        self._tool_first_var.setEnabled(False)
+        self._tool_last_var.setEnabled(False)
         self._tool_prev_var.setEnabled(False)
         self._tool_next_var.setEnabled(False)
 
 
 class TabWidget(QtWidgets.QTabWidget):
-    """
-    Tab widget that can move up and down when asked.
-    """
+    """ Generic tab widget with first/last next/previous methods. """
+
+    def first(self):
+        """ Select the first widget. """
+        self.setCurrentIndex(0)
+
+    def last(self):
+        """ Select the last widget. """
+        self.setCurrentIndex(self.count() - 1)
+
     def next(self):
-        """
-        Select the next widget.
-        """
+        """ Select the next widget. """
         n = self.count()
         if n < 2:
             return
         i = self.currentIndex() + 1
         self.setCurrentIndex(0 if i >= n else i)
 
     def previous(self):
-        """
-        Select the previous widget.
-        """
+        """ Select the previous widget. """
         n = self.count()
         if n < 2:
             return
         i = self.currentIndex() - 1
         self.setCurrentIndex(n - 1 if i < 0 else i)
 
 
-class AbfTab(TabWidget):
-    """
-    A widget displaying an ABF file.
-    """
-    def __init__(self, parent, abf):
+class GraphTabWidget(TabWidget):
+    """ Tab widget to graph a data source. """
+
+    def __init__(self, parent):
         super().__init__(parent)
+
         self.setTabsClosable(False)
         self.setTabPosition(self.TabPosition.East)
-        self._abf = abf
+
         self._figures = []
         self._axes = []
-        for i in range(self._abf.data_channels()):
-            tab, name = self.create_graph_tab(i)
-            self.addTab(tab, name)
-        for i in range(self._abf.protocol_channels()):
-            tab, name = self.create_protocol_tab(i)
-            self.addTab(tab, name)
-        self.addTab(self.create_info_tab(), 'Info')
-        del self._abf
 
-    def create_graph_tab(self, channel):
-        """
-        Creates a widget displaying the main data.
-        """
+    def deleteLater(self):
+        """ Deletes this tab (later). """
+        for figure in self._figures:
+            figure.clear()
+        for axes in self._axes:
+            axes.cla()
+        del self._figures, self._axes
+        gc.collect()
+        super().deleteLater()
+
+
+class SweepSourceTab(GraphTabWidget):
+    """ A tab widget for sources implementing the SweepSource interface. """
+
+    def __init__(self, parent, source):
+        super().__init__(parent)
+
+        # Add A/D
+        for i in range(source.channel_count()):
+            self._add_graph_tab(source, i)
+
+        # Add D/A
+        for i in range(source.da_count()):
+            self._add_graph_tab(source, i, True)
+
+        # Add meta data
+        self._add_meta_tab(source)
+
+    def _add_graph_tab(self, source, index, da=False):
+        """ Adds a tab for a graph. """
+
+        # Create widget
         widget = QtWidgets.QWidget(self)
+
         # Create figure
         figure = matplotlib.figure.Figure()
-        figure.suptitle(self._abf.filename())
         canvas = backend.FigureCanvasQTAgg(figure)
         canvas.setParent(widget)
-        axes = figure.add_subplot(1, 1, 1)
         toolbar = backend.NavigationToolbar2QT(canvas, widget)
-        # Draw lines
-        name = 'AD(' + str(channel) + ')'   # Default if no data is present
-        times = None
-        for i, sweep in enumerate(self._abf):
-            if times is None:
-                name = 'AD' + str(sweep[channel].number()) + ': ' \
-                    + sweep[channel].name()
-                times = sweep[channel].times()
-            axes.plot(times, sweep[channel].values())
+
+        # Draw signal
+        join_sweeps = not source.equal_length_sweeps()
+        if da:
+            name = source.da_names(index)
+            units = source.da_units(index)
+            times, values = source.da(index, join_sweeps)
+        else:
+            name = source.channel_names(index)
+            units = source.channel_units(index)
+            times, values = source.channel(index, join_sweeps)
+
+        axes = figure.add_subplot(1, 1, 1)
+        axes.set_xlabel(f'Time {source.time_unit()}')
+        axes.set_ylabel(f'{name} {units}')
+        if join_sweeps:
+            axes.plot(times, values)
+        else:
+            for v in values:
+                axes.plot(times[0], v)
+
+        # Store for later deletion
+        self._figures.append(figure)
+        self._axes.append(axes)
+
         # Create a layout
         vbox = QtWidgets.QVBoxLayout()
         vbox.addWidget(canvas)
         vbox.addWidget(toolbar)
         widget.setLayout(vbox)
-        self._figures.append(figure)
-        self._axes.append(axes)
-        return widget, name
 
-    def create_protocol_tab(self, channel):
-        """
-        Creates a widget displaying a stored D/A signal.
-        """
+        # Add tab
+        self.addTab(widget, name)
+
+    '''
+    def debug_tab(self, channel_index, da=True):
+        """ Add a tab graphing data using the DataLog method. """
+        widget = QtWidgets.QWidget(self)
+
+        # Create widget
         widget = QtWidgets.QWidget(self)
+
         # Create figure
         figure = matplotlib.figure.Figure()
         figure.suptitle(self._abf.filename())
         canvas = backend.FigureCanvasQTAgg(figure)
         canvas.setParent(widget)
-        axes = figure.add_subplot(1, 1, 1)
         toolbar = backend.NavigationToolbar2QT(canvas, widget)
+
         # Draw lines
-        name = 'DA(' + str(channel) + ')'   # Default if no data is present
-        times = None
-        for i, sweep in enumerate(self._abf.protocol()):
-            if times is None:
-                name = 'DA' + str(sweep[channel].number()) + ': ' \
-                    + sweep[channel].name()
-                times = sweep[channel].times()
-            axes.plot(times, sweep[channel].values())
+        p = self._abf.da_protocol(channel_index, tu='s', vu='V')
+        times, _ = self._abf.da(channel_index)
+        for t in times:
+            d = p.log_for_interval(t[0], t[-1], for_drawing=True).npview()
+            axes.plot(d['time'] - t[0], d['pace'])
+
         # Create a layout
         vbox = QtWidgets.QVBoxLayout()
         vbox.addWidget(canvas)
         vbox.addWidget(toolbar)
         widget.setLayout(vbox)
-        self._figures.append(figure)
-        self._axes.append(axes)
-        return widget, name
 
-    def create_info_tab(self):
-        """
-        Creates a tab displaying information about the file.
-        """
-        widget = QtWidgets.QTextEdit(self)
-        widget.setText(self._abf.info(show_header=True))
-        widget.setReadOnly(True)
-        return widget
+        # Add tab
+        self.addTab(widget, name)
+'''
 
-    def deleteLater(self):
-        """
-        Deletes this tab (later).
-        """
-        for figure in self._figures:
-            figure.clear()
-        for axes in self._axes:
-            axes.cla()
-        del self._figures, self._axes
-        gc.collect()
-        super().deleteLater()
+    def _add_meta_tab(self, source):
 
+        meta = source.meta_str(True)
+        if meta:
+            widget = QtWidgets.QTextEdit(self)
+            widget.setText(meta)
+            widget.setReadOnly(True)
+            self.addTab(widget, 'info')
 
-class AtfTab(TabWidget):
-    """
-    A widget displaying an AGF file.
-    """
+
+class AbfTab(SweepSourceTab):
+    """ A widget displaying an ABF file. """
+    pass
+
+
+class AtfTab(GraphTabWidget):
+    """ A widget displaying an ATF file. """
     def __init__(self, parent, atf):
         super().__init__(parent)
         self._atf = atf
 
-        self.setTabsClosable(False)
-        self.setTabPosition(self.TabPosition.East)
-
-        self._figures = []
-        self._axes = []
         keys = list(self._atf.keys())
         if len(keys) > 1:
             time = keys[0]  # Time is always first (and regularly sampled)
             for key in keys[1:]:
                 self.addTab(self.create_graph_tab(time, key), key)
         self.addTab(self.create_info_tab(), 'Info')
         del self._atf
@@ -686,49 +777,32 @@
         self._figures.append(figure)
         self._axes.append(axes)
 
         # Return widget
         return widget
 
     def create_info_tab(self):
-        """
-        Creates a tab displaying information about the file.
-        """
+        """ Creates a tab displaying information about the file. """
         widget = QtWidgets.QTextEdit(self)
         widget.setText(self._atf.info())
         widget.setReadOnly(True)
         return widget
 
-    def deleteLater(self):
-        """
-        Deletes this tab (later).
-        """
-        for figure in self._figures:
-            figure.clear()
-        for axes in self._axes:
-            axes.cla()
-        del self._figures, self._axes
-        gc.collect()
-        super().deleteLater()
-
 
-class CsvTab(TabWidget):
+class CsvTab(GraphTabWidget):
     """
     A widget displaying a CSV file.
 
     The given log must have a time variable set.
     """
     def __init__(self, parent, log, filename):
         super().__init__(parent)
-        self.setTabsClosable(False)
-        self.setTabPosition(self.TabPosition.East)
+
         self._log = log.npview()
         self._filename = filename
-        self._figures = []
-        self._axes = []
 
         # Check time key was found
         time = log.time_key()
         try:
             self._time = log.time()
         except myokit.InvalidDataLogError:
             if time is None:
@@ -763,17 +837,15 @@
                 keys.append(var)
 
         # Add tab for each column
         for k in keys:
             self.addTab(self.create_graph_tab(k, groups.get(k)), k)
 
     def create_graph_tab(self, key, indices=None):
-        """
-        Creates a widget displaying the data stored under ``key``.
-        """
+        """ Creates a widget displaying the data stored under ``key``. """
         widget = QtWidgets.QWidget(self)
 
         # Create figure
         figure = matplotlib.figure.Figure()
         figure.suptitle(self._filename)
         canvas = backend.FigureCanvasQTAgg(figure)
         canvas.setParent(widget)
@@ -793,38 +865,21 @@
         vbox.addWidget(canvas)
         vbox.addWidget(toolbar)
         widget.setLayout(vbox)
         self._figures.append(figure)
         self._axes.append(axes)
         return widget
 
-    def deleteLater(self):
-        """
-        Deletes this tab (later).
-        """
-        for figure in self._figures:
-            figure.clear()
-        for axes in self._axes:
-            axes.cla()
-        del self._figures, self._axes
-        gc.collect()
-        super().deleteLater()
-
 
-class MatTab(TabWidget):
-    """
-    A widget displaying a MAT file.
-    """
+class MatTab(GraphTabWidget):
+    """ A widget displaying a .mat file. """
     def __init__(self, parent, mat, filename):
         super().__init__(parent)
-        self.setTabsClosable(False)
-        self.setTabPosition(self.TabPosition.East)
-        self._figures = []
+
         self._filename = filename
-        self._axes = []
 
         # Find usable data
         for key in mat.keys():
             if key[:1] == '_':
                 continue
             time, data = None, None
             data = mat[key]
@@ -881,38 +936,27 @@
         vbox.addWidget(canvas)
         vbox.addWidget(toolbar)
         widget.setLayout(vbox)
         self._figures.append(figure)
         self._axes.append(axes)
         return widget
 
-    def deleteLater(self):
-        """
-        Deletes this tab (later).
-        """
-        for figure in self._figures:
-            figure.clear()
-        for axes in self._axes:
-            axes.cla()
-        del self._figures, self._axes
-        gc.collect()
-        super().deleteLater()
 
+class PatchMasterTab(SweepSourceTab):
+    """ A widget displaying a PatchMaster series. """
+    pass
+
+
+class TxtTab(GraphTabWidget):
+    """ A widget displaying a .txt file (with lots of heuristics!). """
 
-class TxtTab(TabWidget):
-    """
-    A widget displaying a TXT file (with lots of heuristics!).
-    """
     def __init__(self, parent, data, filename):
         super().__init__(parent)
-        self.setTabsClosable(False)
-        self.setTabPosition(self.TabPosition.East)
-        self._figures = []
+
         self._filename = filename
-        self._axes = []
 
         # Find usable data
         if np.prod(data.shape) == np.max(data.shape):
             # 1d data
             data = data.reshape((np.max(data.shape),))
             # Create tab
             tab = self.create_graph_tab(None, data)
@@ -963,74 +1007,11 @@
         vbox.addWidget(canvas)
         vbox.addWidget(toolbar)
         widget.setLayout(vbox)
         self._figures.append(figure)
         self._axes.append(axes)
         return widget
 
-    def deleteLater(self):
-        """
-        Deletes this tab (later).
-        """
-        for figure in self._figures:
-            figure.clear()
-        for axes in self._axes:
-            axes.cla()
-        del self._figures, self._axes
-        gc.collect()
-        super().deleteLater()
-
-
-class WcpTab(TabWidget):
-    """
-    A widget displaying a WCP file.
-    """
-    def __init__(self, parent, wcp):
-        super().__init__(parent)
-        self.setTabsClosable(False)
-        self.setTabPosition(self.TabPosition.East)
-        self._wcp = wcp
-        self._figures = []
-        self._axes = []
-        for i in range(self._wcp.records()):
-            self.addTab(self.create_graph_tab(i), 'Record ' + str(i))
-        del self._wcp
-
-    def create_graph_tab(self, record):
-        """
-        Creates a widget displaying the data in record i
-        """
-        widget = QtWidgets.QWidget(self)
-        # Create figure
-        figure = matplotlib.figure.Figure()
-        figure.suptitle(self._wcp.filename())
-        canvas = backend.FigureCanvasQTAgg(figure)
-        canvas.setParent(widget)
-        axes = figure.add_subplot(1, 1, 1)
-        toolbar = backend.NavigationToolbar2QT(canvas, widget)
-        # Draw lines
-        for i in range(self._wcp.channels()):
-            axes.plot(
-                np.array(self._wcp.times(), copy=True),
-                np.array(self._wcp.values(record, i), copy=True),
-            )
-        # Create a layout
-        vbox = QtWidgets.QVBoxLayout()
-        vbox.addWidget(canvas)
-        vbox.addWidget(toolbar)
-        widget.setLayout(vbox)
-        self._figures.append(figure)
-        self._axes.append(axes)
-        return widget
 
-    def deleteLater(self):
-        """
-        Deletes this tab (later).
-        """
-        for figure in self._figures:
-            figure.clear()
-        for axes in self._axes:
-            axes.cla()
-        del self._figures, self._axes
-        gc.collect()
-        super().deleteLater()
+class WcpTab(SweepSourceTab):
+    pass
```

### Comparing `myokit-1.35.0/myokit/gui/explorer.py` & `myokit-1.35.1/myokit/gui/explorer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/gui/ide.py` & `myokit-1.35.1/myokit/gui/ide.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/gui/progress.py` & `myokit-1.35.1/myokit/gui/progress.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/gui/source.py` & `myokit-1.35.1/myokit/gui/source.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/gui/vargrapher.py` & `myokit-1.35.1/myokit/gui/vargrapher.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/lib/deps.py` & `myokit-1.35.1/myokit/lib/deps.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/lib/guess.py` & `myokit-1.35.1/myokit/lib/guess.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/lib/hh.py` & `myokit-1.35.1/myokit/lib/hh.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/lib/multi.py` & `myokit-1.35.1/myokit/lib/multi.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/lib/plots.py` & `myokit-1.35.1/myokit/lib/plots.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/pacing.py` & `myokit-1.35.1/myokit/pacing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/pype.py` & `myokit-1.35.1/myokit/pype.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/__init__.py` & `myokit-1.35.1/myokit/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/ansic_event_based_pacing.py` & `myokit-1.35.1/myokit/tests/ansic_event_based_pacing.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class AnsicEventBasedPacing(myokit.CModule):
     """
     Class for testing the event-based pacing system.
     """
     _index = 0
 
-    def __init__(self, protocol):
+    def __init__(self, protocol, initial_time=0):
         super().__init__()
 
         # Unique id
         AnsicEventBasedPacing._index += 1
         module_name = 'myokit_ansic_pacing_' \
             + str(AnsicEventBasedPacing._index)
 
@@ -38,16 +38,16 @@
         libs = []
         libd = []
         incd = [DIR_TEST, myokit.DIR_CFUNC]
         self._sys = None
         self._sys = self._compile(module_name, fname, args, libs, libd, incd)
 
         # Initialize
-        self._sys.init(protocol.clone())
-        self.advance(0)
+        self._sys.init(protocol.clone(), initial_time)
+        self.advance(initial_time)
 
     def __del__(self):
         # Free the memory used by the pacing system
         if self._sys is not None:
             self._sys.clean()
 
     def advance(self, new_time):
```

### Comparing `myokit-1.35.0/myokit/tests/ansic_fixed_form_pacing.py` & `myokit-1.35.1/myokit/tests/ansic_time_series_pacing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #!/usr/bin/env python3
 #
-# Class for testing the fixed-form pacing system.
+# Class for testing the time-series pacing system.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 import os
 
 import myokit
 
 from myokit.tests import DIR_TEST
 
 # Location of C template
-SOURCE_FILE = 'ansic_fixed_form_pacing.c'
+SOURCE_FILE = 'ansic_time_series_pacing.c'
 
 
-class AnsicFixedFormPacing(myokit.CModule):
+class AnsicTimeSeriesPacing(myokit.CModule):
     """
-    Class for testing the fixed-form pacing system.
+    Class for testing the time-series pacing system.
     """
     _index = 0
 
     def __init__(self, protocol):
         super().__init__()
 
         # Unique id
-        AnsicFixedFormPacing._index += 1
+        AnsicTimeSeriesPacing._index += 1
         module_name = \
-            'myokit_ansic_fpacing_' + str(AnsicFixedFormPacing._index)
+            'myokit_ansic_fpacing_' + str(AnsicTimeSeriesPacing._index)
 
         # Arguments
         fname = os.path.join(DIR_TEST, SOURCE_FILE)
 
         # Create back-end
         args = {'module_name': module_name}
         libs = []
```

### Comparing `myokit-1.35.0/myokit/tests/data/beeler-1977-model-compare-a.mmt` & `myokit-1.35.1/myokit/tests/data/beeler-1977-model-compare-a.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/beeler-1977-model-compare-b.mmt` & `myokit-1.35.1/myokit/tests/data/beeler-1977-model-compare-b.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/beeler-1977-model.mmt` & `myokit-1.35.1/myokit/tests/data/beeler-1977-model.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/beeler-1977-units.mmt` & `myokit-1.35.1/myokit/tests/data/beeler-1977-units.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/clancy-1999-fitting.mmt` & `myokit-1.35.1/myokit/tests/data/clancy-1999-fitting.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/conditional.mmt` & `myokit-1.35.1/myokit/tests/data/conditional.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/cv1d.mmt` & `myokit-1.35.1/myokit/tests/data/cv1d.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/cv1d.zip` & `myokit-1.35.1/myokit/tests/data/cv1d.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/decker-2009.mmt` & `myokit-1.35.1/myokit/tests/data/decker-2009.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/decker.model` & `myokit-1.35.1/myokit/tests/data/decker.model`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/dn-1985-normalised.mmt` & `myokit-1.35.1/myokit/tests/data/dn-1985-normalised.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/dom-markov.mmt` & `myokit-1.35.1/myokit/tests/data/dom-markov.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/abf-protocol.pro` & `myokit-1.35.1/myokit/tests/data/formats/abf-protocol.pro`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/abf-v1.abf` & `myokit-1.35.1/myokit/tests/data/formats/abf-v1.abf`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/cellml/br-1977-dot.cellml` & `myokit-1.35.1/myokit/tests/data/formats/cellml/br-1977-dot.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/cellml/br-1977.cellml` & `myokit-1.35.1/myokit/tests/data/formats/cellml/br-1977.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/cellml/corrias.cellml` & `myokit-1.35.1/myokit/tests/data/formats/cellml/corrias.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/cellml/decker-2009.cellml` & `myokit-1.35.1/myokit/tests/data/formats/cellml/decker-2009.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/cellml/documentation.cellml` & `myokit-1.35.1/myokit/tests/data/formats/cellml/documentation.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml` & `myokit-1.35.1/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml` & `myokit-1.35.1/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml` & `myokit-1.35.1/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml` & `myokit-1.35.1/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml` & `myokit-1.35.1/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/sbml/HodgkinHuxley.xml` & `myokit-1.35.1/myokit/tests/data/formats/sbml/HodgkinHuxley.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml` & `myokit-1.35.1/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml` & `myokit-1.35.1/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml` & `myokit-1.35.1/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/sbml/result/00001-results.csv` & `myokit-1.35.1/myokit/tests/data/formats/sbml/result/00001-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/sbml/result/00004-results.csv` & `myokit-1.35.1/myokit/tests/data/formats/sbml/result/00004-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/sbml/result/01103-results.csv` & `myokit-1.35.1/myokit/tests/data/formats/sbml/result/01103-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/formats/wcp-file.wcp` & `myokit-1.35.1/myokit/tests/data/formats/wcp-file.wcp`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad1d-1-not-enough-files.zip` & `myokit-1.35.1/myokit/tests/data/io/bad1d-1-not-enough-files.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad1d-2-no-header.zip` & `myokit-1.35.1/myokit/tests/data/io/bad1d-2-no-header.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad1d-3-no-data.zip` & `myokit-1.35.1/myokit/tests/data/io/bad1d-3-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad1d-4-not-a-zip.zip` & `myokit-1.35.1/myokit/tests/data/io/bad1d-4-not-a-zip.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad1d-5-bad-data-type.zip` & `myokit-1.35.1/myokit/tests/data/io/bad1d-5-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad1d-6-time-too-short.zip` & `myokit-1.35.1/myokit/tests/data/io/bad1d-6-time-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad1d-7-0d-too-short.zip` & `myokit-1.35.1/myokit/tests/data/io/bad1d-7-0d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad1d-8-1d-too-short.zip` & `myokit-1.35.1/myokit/tests/data/io/bad1d-8-1d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad2d-1-not-enough-files.zip` & `myokit-1.35.1/myokit/tests/data/io/bad2d-1-not-enough-files.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad2d-2-no-header.zip` & `myokit-1.35.1/myokit/tests/data/io/bad2d-2-no-header.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad2d-3-no-data.zip` & `myokit-1.35.1/myokit/tests/data/io/bad2d-3-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad2d-4-not-a-zip.zip` & `myokit-1.35.1/myokit/tests/data/io/bad2d-4-not-a-zip.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad2d-5-bad-data-type.zip` & `myokit-1.35.1/myokit/tests/data/io/bad2d-5-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad2d-6-time-too-short.zip` & `myokit-1.35.1/myokit/tests/data/io/bad2d-6-time-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad2d-7-0d-too-short.zip` & `myokit-1.35.1/myokit/tests/data/io/bad2d-7-0d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/bad2d-8-2d-too-short.zip` & `myokit-1.35.1/myokit/tests/data/io/bad2d-8-2d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/badlog-1-no-data.zip` & `myokit-1.35.1/myokit/tests/data/io/badlog-1-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/badlog-2-no-structure.zip` & `myokit-1.35.1/myokit/tests/data/io/badlog-2-no-structure.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/badlog-4-invalid-n-fields.zip` & `myokit-1.35.1/myokit/tests/data/io/badlog-4-invalid-n-fields.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/badlog-5-invalid-data-size.zip` & `myokit-1.35.1/myokit/tests/data/io/badlog-5-invalid-data-size.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/badlog-6-bad-data-type.zip` & `myokit-1.35.1/myokit/tests/data/io/badlog-6-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/badlog-7-not-enough-data.zip` & `myokit-1.35.1/myokit/tests/data/io/badlog-7-not-enough-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/block2d.mmt` & `myokit-1.35.1/myokit/tests/data/io/block2d.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/block2d.zip` & `myokit-1.35.1/myokit/tests/data/io/block2d.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/io/goodlog.zip` & `myokit-1.35.1/myokit/tests/data/io/goodlog.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/lr-1991-dep.mmt` & `myokit-1.35.1/myokit/tests/data/lr-1991-dep.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/lr-1991-fitting.mmt` & `myokit-1.35.1/myokit/tests/data/lr-1991-fitting.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/lr-1991-testing.mmt` & `myokit-1.35.1/myokit/tests/data/lr-1991-testing.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/lr-1991.mmt` & `myokit-1.35.1/myokit/tests/data/lr-1991.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/multi/beeler-no-name.mmt` & `myokit-1.35.1/myokit/tests/data/multi/beeler-no-name.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/multi/lr-1991.mmt` & `myokit-1.35.1/myokit/tests/data/multi/lr-1991.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/multi/subdir/beeler-no-name.mmt` & `myokit-1.35.1/myokit/tests/data/multi/subdir/beeler-no-name.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/data/noble-1962.mmt` & `myokit-1.35.1/myokit/tests/data/noble-1962.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_aux.py` & `myokit-1.35.1/myokit/tests/test_aux.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_cellml_v1_api.py` & `myokit-1.35.1/myokit/tests/test_cellml_v1_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_cellml_v1_parser.py` & `myokit-1.35.1/myokit/tests/test_cellml_v1_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_cellml_v1_writer.py` & `myokit-1.35.1/myokit/tests/test_cellml_v1_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_cellml_v2_api.py` & `myokit-1.35.1/myokit/tests/test_cellml_v2_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_cellml_v2_parser.py` & `myokit-1.35.1/myokit/tests/test_cellml_v2_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_cellml_v2_writer.py` & `myokit-1.35.1/myokit/tests/test_cellml_v2_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_cmodel.py` & `myokit-1.35.1/myokit/tests/test_cmodel.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_component.py` & `myokit-1.35.1/myokit/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_config.py` & `myokit-1.35.1/myokit/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_datablock.py` & `myokit-1.35.1/myokit/tests/test_datablock.py`

 * *Files 8% similar despite different names*

```diff
@@ -696,14 +696,98 @@
             [[153, 61, 143], [153, 61, 143]],
         ])
         c = b.colors('x', colormap='traditional')
         self.assertTrue(np.all(c[0] == t0))
         self.assertTrue(np.all(c[1] == t1))
         self.assertTrue(np.all(c[2] == t2))
 
+        # Gray colormap
+        t0 = np.array([  # Deepest array is a pixel
+            [[0] * 3, [51] * 3],
+            [[102] * 3, [153] * 3],
+            [[204] * 3, [255] * 3],
+        ])
+        t1 = np.array([
+            [[255] * 3, [204] * 3],
+            [[153] * 3, [102] * 3],
+            [[51] * 3, [0] * 3],
+        ])
+        t2 = np.array([
+            [[0] * 3, [0] * 3],
+            [[0] * 3, [0] * 3],
+            [[0] * 3, [0] * 3],
+        ])
+        c = b.colors('x', colormap='gray')
+        self.assertTrue(np.all(c[0] == t0))
+        self.assertTrue(np.all(c[1] == t1))
+        self.assertTrue(np.all(c[2] == t2))
+
+        # Cividis colormap
+        t0 = np.array([  # Deepest array is a pixel
+            [[0, 32, 76], [49, 68, 107]],
+            [[102, 104, 112], [150, 143, 119]],
+            [[203, 186, 104], [255, 233, 69]],
+        ])
+        t1 = np.array([
+            [[255, 233, 69], [203, 186, 104]],
+            [[150, 143, 119], [102, 104, 112]],
+            [[49, 68, 107], [0, 32, 76]],
+        ])
+        t2 = np.array([
+            [[0, 32, 76], [0, 32, 76]],
+            [[0, 32, 76], [0, 32, 76]],
+            [[0, 32, 76], [0, 32, 76]],
+        ])
+        c = b.colors('x', colormap='cividis')
+        self.assertTrue(np.all(c[0] == t0))
+        self.assertTrue(np.all(c[1] == t1))
+        self.assertTrue(np.all(c[2] == t2))
+
+        # Inferno colormap
+        t0 = np.array([  # Deepest array is a pixel
+            [[0, 0, 4], [66, 10, 104]],
+            [[148, 38, 104], [223, 82, 57]],
+            [[253, 167, 12], [253, 255, 165]],
+        ])
+        t1 = np.array([
+            [[253, 255, 165], [253, 167, 12]],
+            [[223, 82, 57], [148, 38, 104]],
+            [[66, 10, 104], [0, 0, 4]],
+        ])
+        t2 = np.array([
+            [[0, 0, 4], [0, 0, 4]],
+            [[0, 0, 4], [0, 0, 4]],
+            [[0, 0, 4], [0, 0, 4]],
+        ])
+        c = b.colors('x', colormap='inferno')
+        self.assertTrue(np.all(c[0] == t0))
+        self.assertTrue(np.all(c[1] == t1))
+        self.assertTrue(np.all(c[2] == t2))
+
+        # Viridis colormap
+        t0 = np.array([  # Deepest array is a pixel
+            [[68, 1, 84], [65, 68, 136]],
+            [[42, 121, 143], [35, 170, 132]],
+            [[125, 211, 80], [254, 232, 37]],
+        ])
+        t1 = np.array([
+            [[254, 232, 37], [125, 211, 80]],
+            [[35, 170, 132], [42, 121, 143]],
+            [[65, 68, 136], [68, 1, 84]],
+        ])
+        t2 = np.array([
+            [[68, 1, 84], [68, 1, 84]],
+            [[68, 1, 84], [68, 1, 84]],
+            [[68, 1, 84], [68, 1, 84]],
+        ])
+        c = b.colors('x', colormap='viridis')
+        self.assertTrue(np.all(c[0] == t0))
+        self.assertTrue(np.all(c[1] == t1))
+        self.assertTrue(np.all(c[2] == t2))
+
     def test_colors_multiplier(self):
         # Test using the multiplier argument in colors
 
         w, h = 2, 3
         time = [1, 2, 3]
         b = myokit.DataBlock2d(w, h, time)
         x = np.array([  # Each 3 by 2 array is a point in time
```

### Comparing `myokit-1.35.0/myokit/tests/test_datalog.py` & `myokit-1.35.1/myokit/tests/test_datalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -2185,15 +2185,16 @@
         self.assertEqual(len(e['time']), 7)
         x = np.array([0, 0.5, 1, 1.5, 2, 2.5, 3])
         self.assertTrue(np.all(e['time'] == x))
         for i, y in enumerate(x):
             self.assertTrue(np.abs(np.exp(y) - e['values'][i]) < 0.02)
 
         # test setting tmin and tmax
-        e = d.regularize(dt=0.5, tmin=0.4, tmax=2.6)
+        with WarningCollector() as w:
+            e = d.regularize(dt=0.5, tmin=0.4, tmax=2.6)
         self.assertEqual(len(e['time']), 5)
         x = np.array([0.4, 0.9, 1.4, 1.9, 2.4])
         self.assertTrue(np.all(e['time'] == x))
         for i, y in enumerate(x):
             self.assertTrue(np.abs(np.exp(y) - e['values'][i]) < 0.02)
 
     def test_time(self):
```

### Comparing `myokit-1.35.0/myokit/tests/test_dependency_checking.py` & `myokit-1.35.1/myokit/tests/test_dependency_checking.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_expressions.py` & `myokit-1.35.1/myokit/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_float.py` & `myokit-1.35.1/myokit/tests/test_float.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats.py` & `myokit-1.35.1/myokit/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_axon.py` & `myokit-1.35.1/myokit/tests/test_simulation_log_interval.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,404 +1,420 @@
 #!/usr/bin/env python3
 #
-# Tests the Axon format module.
+# Tests the simulation classes' interpretation of log_interval
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
 import os
 import unittest
 
 import numpy as np
 
 import myokit
-import myokit.formats.axon as axon
 
-from myokit.tests import TemporaryDirectory, DIR_FORMATS
+from myokit.tests import DIR_DATA
 
+# Extra output
+debug = False
 
-class AbfTest(unittest.TestCase):
+
+class PeriodicTest(unittest.TestCase):
     """
-    Tests the ABF format support.
+    Tests a simulation class for consistent log entry timing.
     """
-
-    def test_read_v1(self):
-        # Test reading a version 1 file.
-
-        # Load file
-        path = os.path.join(DIR_FORMATS, 'abf-v1.abf')
-        abf = axon.AbfFile(path)
-        self.assertEqual(abf.filename(), path)
-
-        # Check version info
-        self.assertIn('version 1.65', abf.info())
-        self.assertEqual(
-            abf.info(),
-            'Axon Binary File: abf-v1.abf\n'
-            'ABF Format version 1.65\n'
-            'Recorded on: 2014-11-14 12:52:29.389999\n'
-            'Acquisition mode: 5: Episodic stimulation mode\n'
-            'Protocol set for 1 trials, spaced 0.0s apart.\n'
-            '    with 1 runs per trial, spaced 0.0s apart.\n'
-            '     and 9 sweeps per run, spaced 0.5s apart.\n'
-            'Sampling rate: 10000.0 Hz\n'
-            'Channel 0: "IN 0      "\n'
-            '  Unit: pA'
-        )
-        # Test getting full header runs without crashing
-        abf.info(True)
-
-        # Test len returns number of sweeps
-        self.assertEqual(len(abf), 9)
-
-        # Test data access
-        self.assertEqual(abf.data_channels(), 1)    # 1 data channel
-        x = abf.extract_channel(0)
-        self.assertEqual(len(x), 1 + len(abf))      # sweeps + time
-        self.assertEqual(len(x[0]), len(x[1]))
-        self.assertEqual(len(x[0]), len(x[2]))
-        self.assertEqual(len(x[0]), len(x[3]))
-        self.assertEqual(len(x[0]), len(x[4]))
-        self.assertEqual(len(x[0]), len(x[5]))
-        self.assertEqual(len(x[0]), len(x[6]))
-        self.assertEqual(len(x[0]), len(x[7]))
-        self.assertEqual(len(x[0]), len(x[8]))
-        self.assertEqual(len(x[0]), len(x[9]))
-        y = abf.extract_channel_as_myokit_log(0)
-        self.assertEqual(len(y), 1 + len(abf))      # sweeps + time
-        z = abf.myokit_log()
-        self.assertEqual(len(z), 6)     # time + channel + 4 protocol channels
-        sweep = abf[0]
-        self.assertEqual(len(sweep), 1)     # 1 channel in sweep
-        channel = sweep[0]
-        self.assertIsInstance(channel.number(), int)
-        self.assertIn('Channel', str(channel))
-        self.assertEqual(len(abf) * len(channel.times()), len(z.time()))
-        self.assertEqual(len(abf) * len(channel.values()), len(z.time()))
-
-        # Test reading of sweeps as one long array
-        x, y = abf.extract_channel(0, join=True)
-        z = abf.extract_channel(0)
-        self.assertEqual(len(x), len(y))
-        self.assertEqual(len(x), len(abf) * len(z[0]))
-        self.assertTrue(np.all(x[1:] > x[:-1]))
-
-        # Test protocol extraction
-        self.assertEqual(abf.protocol_channels(), 4)    # 4 protocol channels
-        p = abf.myokit_protocol()
-        self.assertEqual(len(p), 18)    # 18 steps in this protocol
-        self.assertEqual(abf.protocol_holding_level(0), 0)
-        p = abf.myokit_protocol(0)
-        self.assertEqual(len(p), 18)
-
-    def test_read_v2(self):
-        # Test reading a version 2 file.
-
-        # Load file
-        path = os.path.join(DIR_FORMATS, 'abf-v2.abf')
-        abf = axon.AbfFile(path)
-
-        # Check version info
-        self.assertIn('version 2.0', abf.info())
-        self.assertEqual(
-            abf.info(),
-            'Axon Binary File: abf-v2.abf\n'
-            'ABF Format version 2.0\n'
-            'Recorded on: 2014-10-01 14:03:55.980999\n'
-            'Acquisition mode: 5: Episodic stimulation mode\n'
-            'Protocol set for 1 trials, spaced 0.0s apart.\n'
-            '    with 1 runs per trial, spaced 0.0s apart.\n'
-            '     and 1 sweeps per run, spaced 5.0s apart.\n'
-            'Sampling rate: 10000.0 Hz\n'
-            'Channel 0: "IN 0"\n'
-            '  Unit: pA\n'
-            '  Low-pass filter: 10000.0 Hz\n'
-            '  Cm (telegraphed): 6.34765625 pF')
-        # Test getting full header runs without crashing
-        abf.info(True)
-
-        # Test len returns number of sweeps
-        self.assertEqual(len(abf), 1)
-
-        # Test data access
-        self.assertEqual(abf.data_channels(), 1)    # 1 data channel
-        x = abf.extract_channel(0)
-        self.assertEqual(len(x), 1 + len(abf))      # sweeps + time
-        self.assertEqual(len(x[0]), len(x[1]))
-        y = abf.extract_channel_as_myokit_log(0)
-        self.assertEqual(len(y), 1 + len(abf))      # sweeps + time
-        z = abf.myokit_log()
-        self.assertEqual(len(z), 6)     # time + channel + 4 protocol channels
-        sweep = abf[0]
-        self.assertEqual(len(sweep), 1)     # 1 channel in sweep
-        channel = sweep[0]
-        self.assertEqual(len(abf) * len(channel.times()), len(z.time()))
-        self.assertEqual(len(abf) * len(channel.values()), len(z.time()))
-
-        # Test protocol extraction
-        self.assertEqual(abf.protocol_channels(), 4)    # 4 protocol channels
-        p = abf.myokit_protocol()
-        self.assertEqual(len(p), 2)     # 2 steps in this protocol
-        self.assertEqual(abf.protocol_holding_level(0), -120)
-        p = abf.myokit_protocol(0)
-        self.assertEqual(len(p), 2)
-
-    def test_read_protocol_v1(self):
-        # Test reading a v1 protocol file.
-
-        # Load file
-        path = os.path.join(DIR_FORMATS, 'abf-protocol.pro')
-        abf = axon.AbfFile(path)
-
-        # Check version info
-        self.assertIn('version 1.65', abf.info())
-        self.assertEqual(
-            abf.info(),
-            'Axon Protocol File: abf-protocol.pro\n'
-            'ABF Format version 1.65\n'
-            'Recorded on: 2005-06-17 14:33:02.160000\n'
-            'Acquisition mode: 5: Episodic stimulation mode\n'
-            'Protocol set for 1 trials, spaced 0.0s apart.\n'
-            '    with 1 runs per trial, spaced 0.0s apart.\n'
-            '     and 30 sweeps per run, spaced 5.0s apart.\n'
-            'Sampling rate: 20000.0 Hz'
-        )
-        # Test getting full header runs without crashing
-        abf.info(True)
-
-        # Load, force as protocol
-        path = os.path.join(DIR_FORMATS, 'abf-protocol.pro')
-        abf = axon.AbfFile(path, is_protocol_file=True)
-
-        # Check version info
-        self.assertIn('version 1.65', abf.info())
-        self.assertIn('Axon Protocol File', abf.info())
-
-        # Test protocol extraction
-        p = abf.myokit_protocol()
-        self.assertEqual(len(p), 60)
-
-        # Test step extraction
-        p = abf.protocol_steps()
-        self.assertEqual(len(p), 1)
-        self.assertEqual(len(p[0]), 30)
-
-    def test_matplotlib_figure(self):
-        # Test figure drawing method (doesn't inspect output).
-        # Select matplotlib backend that doesn't require a screen
-        import matplotlib
-        matplotlib.use('template')
-        path = os.path.join(DIR_FORMATS, 'abf-v1.abf')
-        abf = axon.AbfFile(path)
-        abf.matplotlib_figure()
+    def periodic(self, s):
+        # Test periodic logging.
+        # Set tolerance for equality testing
+        emax = 1e-2     # Time steps for logging are approximate
+        # Test 1: Simple 5 ms simulation, log_interval 0.5 ms
+        d = s.run(5, log=['engine.time'], log_interval=0.5).npview()
+        t = d['engine.time']
+        q = np.arange(0, 5, 0.5)
+        if debug:
+            print(t)
+            print(q)
+            print('- ' * 10)
+        self.assertEqual(len(t), len(q))
+        self.assertTrue(np.max(np.abs(t - q)) < emax)
+        # Test 2: Very short simulation
+        s.reset()
+        d = s.run(1, log=['engine.time'], log_interval=0.5).npview()
+        t = d['engine.time']
+        q = np.arange(0, 1, 0.5)
+        if debug:
+            print(t)
+            print(q)
+            print('- ' * 10)
+        self.assertEqual(len(t), len(q))
+        self.assertTrue(np.max(np.abs(t - q)) < emax)
+        # Test 3: Stop and start a simulation
+        s.reset()
+        d = s.run(1, log=['engine.time'], log_interval=0.5)
+        d = s.run(2, log=d, log_interval=0.5)
+        d = s.run(2, log=d, log_interval=0.5).npview()
+        t = d['engine.time']
+        q = np.arange(0, 5, 0.5)
+        if debug:
+            print(t)
+            print(q)
+            print('- ' * 10)
+        self.assertEqual(len(t), len(q))
+        self.assertTrue(np.max(np.abs(t - q)) < emax)
 
 
-class AtfTest(unittest.TestCase):
+class SimulationTest(PeriodicTest):
     """
-    Tests the ATF format support.
+    Tests myokit.Simulation (which has dynamic, periodic and point-list
+    logging) for consistent log entry timing.
     """
+    def test_dynamic(self):
+        # Test dynamic logging.
 
-    def test_write_read(self):
-        # Test writing and reading an ATF file.
+        emax = 1e-6     # Used for equality testing
+        if debug:
+            print('= Simulation :: Dynamic logging =')
+        # Load model & protocol
+        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+        # Define sensitivities
+        sens = (['ik1.gK1', 'ikp.IKp'], ['cell.K_o', 'ikp.gKp'])
+        # Create simulation
+        s = myokit.Simulation(m, p, sens)
+
+        #
+        # Test 1: Simple 5 ms simulation, log_interval 0.5 ms
+        #
+        d, e = s.run(50, log=['engine.time', 'ik1.gK1', 'ikp.IKp'])
+        t = d['engine.time']
+        if debug:
+            print(t[:2])
+            print(t[-2:])
+            print('- ' * 10)
+        # Test first point not double
+        self.assertGreater(t[1], t[0])
+        # Test last point not double
+        self.assertGreater(t[-1], t[-2])
+        # Test first point is 0
+        self.assertTrue(np.abs(t[0] - 0) < emax)
+        # Test last point is 50
+        self.assertTrue(np.abs(t[-1] - 50) < emax)
+        # Test shape of sensitivities
+        n_states = 2
+        n_times = len(t)
+        n_sens = 2
+        self.assertTrue(np.array(e).shape, (n_times, n_states, n_sens))
+
+        #
+        # Test 2: Very short simulation
+        #
+        s.reset()
+        d, e = s.run(1, log=['engine.time', 'ik1.gK1', 'ikp.IKp'])
+        t = d['engine.time']
+        if debug:
+            print(t[:2])
+            print(t[-2:])
+            print('- ' * 10)
+        # Test first point not double
+        self.assertGreater(t[1], t[0])
+        # Test last point not double
+        self.assertGreater(t[-1], t[-2])
+        # Test first point is 0
+        self.assertTrue(np.abs(t[0] - 0) < emax)
+        # Test last point is 50
+        self.assertTrue(np.abs(t[-1] - 1) < emax)
+        # Test shape of sensitivities
+        n_states = 2
+        n_times = len(t)
+        n_sens = 2
+        self.assertTrue(np.array(e).shape, (n_times, n_states, n_sens))
+
+        #
+        # Test 3: Stop and start a simulation
+        #
+        s.reset()
+        d, e = s.run(2, log=['engine.time', 'ik1.gK1', 'ikp.IKp'])
+        t = d['engine.time']
+        n = len(d['engine.time'])
+        if debug:
+            print(d['engine.time'][:2])
+        # Test first point not double
+        self.assertGreater(t[1], t[0])
+        # Test last point not double
+        self.assertGreater(t[-1], t[-2])
+        # Test first point is 0
+        self.assertTrue(np.abs(t[0] - 0) < emax)
+        # Test last point is 2
+        self.assertTrue(np.abs(t[-1] - 2) < emax)
+        # Test shape of sensitivities
+        n_states = 2
+        n_times = len(t)
+        n_sens = 2
+        self.assertTrue(np.array(e).shape, (n_times, n_states, n_sens))
+        d, e = s.run(13, log=d)
+        t = d['engine.time']
+        if debug:
+            print(t[n - 2:n + 2])
+        # Test last point not double
+        self.assertGreater(t[-1], t[-2])
+        # Test last point is 2+13
+        self.assertTrue(np.abs(t[-1] - 15) < emax)
+        # Test intermediary points are different
+        self.assertGreater(t[n], t[n - 1])
+        # Test shape of sensitivities
+        n_states = 2
+        n_times = len(t)
+        n_sens = 2
+        self.assertTrue(np.array(e).shape, (n_times, n_states, n_sens))
+        n = len(d['engine.time'])
+        d, e = s.run(15, log=d)
+        t = d['engine.time']
+        if debug:
+            print(t[n - 2:n + 2])
+        # Test last point not double
+        self.assertGreater(t[-1], t[-2])
+        # Test last point is 2 + 13 + 15
+        self.assertTrue(np.abs(t[-1] - 30) < emax)
+        # Test intermediary points are different
+        self.assertGreater(t[n], t[n - 1])
+        # Test shape of sensitivities
+        n_states = 2
+        n_times = len(t)
+        n_sens = 2
+        self.assertTrue(np.array(e).shape, (n_times, n_states, n_sens))
+        n = len(d['engine.time'])
+        d, e = s.run(20, log=d)
+        t = d['engine.time']
+        if debug:
+            print(t[n - 2:n + 2])
+            print(t[-2:])
+            print('- ' * 10)
+        # Test last point not double
+        self.assertGreater(t[-1], t[-2])
+        # Test last point is 2 + 13 + 15 + 20
+        self.assertTrue(np.abs(t[-1] - 50) < emax)
+        # Test intermediary points are different
+        self.assertGreater(t[n], t[n - 1])
+        # Test shape of sensitivities
+        n_states = 2
+        n_times = len(t)
+        n_sens = 2
+        self.assertTrue(np.array(e).shape, (n_times, n_states, n_sens))
+
+    def test_periodic(self):
+        # Test periodic logging
+
+        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+        s = myokit.Simulation(m, p)
+        self.periodic(s)
+
+    def test_interpolation_and_pacing(self):
+        # Test if interpolation results in correct pacing values.
+
+        # When logging with discontinuous steps, in the adaptive time
+        # CVODE sim, the value of pace must be
+        #  1. The old value *before* the time of the event
+        #  2. The new value *at and after* the time of the event
+        #  3. Back to zero *at and after* the end of the event
+        #     (Unless it ends sooner due to a new event arriving)
+        # Load model
+        m = myokit.load_model('example')
+
+        # Voltage-clamp V (but don't bind it directly)
+        v = m.label('membrane_potential')
+        v.demote()
+        v.set_rhs('-80 + 10 * engine.pace')
+
+        # Create protocol
+        p = myokit.Protocol()
+        p.schedule(level=1, start=0, duration=5, period=10)
+
+        # Create simulation
+        s = myokit.Simulation(m, p)
+
+        # Test if this would result in multiple interpolation steps for logging
+        # i.e. test if the step before each transition was at least 2 log steps
+        # long
+        e = s.run(30).npview()
+        t = e.time()
+        for x in [5, 10, 15, 20, 25]:
+            i = e.find_after(x)
+            if not t[i] - t[i - 1] > 0.2:
+                raise Exception('Issue with test: use longer intervals!')
+        del e, t, x, i
+
+        # Now test if correct interpolated values are returned by periodic
+        # logging.
+        d = s.run(30, log_interval=0.1).npview()
+
+        # Test bound variable
+        p = d['engine.pace']
+        self.assertTrue(np.all(p[0:50] == 1))
+        self.assertTrue(np.all(p[50:100] == 0))
+        self.assertTrue(np.all(p[100:150] == 1))
+        self.assertTrue(np.all(p[150:200] == 0))
+        self.assertTrue(np.all(p[200:250] == 1))
+        self.assertTrue(np.all(p[250:300] == 0))
+
+        # Test variable dependent on bound variable
+        p = d['membrane.V']
+        self.assertTrue(np.all(p[0:50] == -70))
+        self.assertTrue(np.all(p[50:100] == -80))
+        self.assertTrue(np.all(p[100:150] == -70))
+        self.assertTrue(np.all(p[150:200] == -80))
+        self.assertTrue(np.all(p[200:250] == -70))
+        self.assertTrue(np.all(p[250:300] == -80))
+
+    def test_point_list(self):
+        # Test logging with a preset list of points.
+
+        # Load model
+        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+        # Create simulation
+        s = myokit.Simulation(m, p)
+
+        # Don't allow decreasing values
+        times = [1, 2, 1]
+        self.assertRaisesRegex(
+            ValueError, 'non-decreasing', s.run, 5, log_times=times)
+
+        # Can't use together with a log interval
+        self.assertRaisesRegex(
+            ValueError, 'simultaneously', s.run, 5, log_interval=1,
+            log_times=[1, 2, 3])
+
+        # Get some odd times
+        times = np.linspace(0, 90, 999)
+
+        # Test!
+        s.reset()
+        d = s.run(100, log_times=times).npview()
+        self.assertTrue(np.all(d.time() == times))
+
+        # Reset and run again
+        s.reset()
+        d = s.run(100, log_times=times).npview()
+        self.assertTrue(np.all(d.time() == times))
+
+        # Run in parts
+        s.reset()
+        d = s.run(50, log_times=times)
+        self.assertEqual(len(d.time()), np.where(times >= 50)[0][0])
+        d = s.run(50, log=d, log_times=times).npview()
+        self.assertTrue(np.all(d.time() == times))
+
+        # Pre-pacing
+        s.reset()
+        s.pre(50)
+        s.run(100, log_times=times)
+        self.assertTrue(np.all(d.time() == times))
+
+        # Partial logging
+        s.reset()
+        s.run(10)
+        d = s.run(10, log_times=times)
+        imin = np.where(times >= 10)[0][0]
+        imax = np.where(times >= 20)[0][0]
+        self.assertEqual(len(d.time()), imax - imin)
+        self.assertTrue(np.all(d.time() == times[imin:imax]))
+        s.run(20)
+        d = s.run(15, log_times=times)
+        imin = np.where(times >= 40)[0][0]
+        imax = np.where(times >= 55)[0][0]
+        self.assertEqual(len(d.time()), imax - imin)
+        self.assertTrue(np.all(d.time() == times[imin:imax]))
+
+        # Get some regular times
+        times = [0, 1, 2, 3, 4, 5]
+        s.reset()
+        d = s.run(6, log_times=times).npview()
+        self.assertEqual(len(d.time()), len(times))
+        self.assertTrue(np.all(d.time() == times))
+
+        # Repeated points
+        times = [0, 0, 0, 5, 5, 5]
+        s.reset()
+        d = s.run(6, log_times=times).npview()
+        self.assertEqual(len(d.time()), len(times))
+        self.assertTrue(np.all(d.time() == times))
+
+        # End points not included, unless also visited!
+        s.reset()
+        s.run(5)
+        d = s.run(5, log_times=times).npview()
+        self.assertEqual(len(d.time()), 3)
+        self.assertTrue(np.all(d.time() == times[3:]))
+        d = s.run(5, log_times=times).npview()
+        self.assertEqual(len(d.time()), 0)
+
+        # Empty list is same as none
+        s.reset()
+        d = s.run(1, log_times=[])
+        self.assertNotEqual(len(d.time()), 0)
+
+    def test_point_list_2(self):
+        # Test how the point-list logging performs when some of the logging
+        # points overlap with protocol change points.
+
+        # Load model
+        m = myokit.load_model(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+        # Voltage clamp
+        m.binding('pace').set_binding(None)
+        v = m.get('membrane.V')
+        v.demote()
+        v.set_rhs(0)
+        v.set_binding('pace')
+        #TODO: Implement chaining like this?
+        #m.get('membrane.V').demote().set_rhs(0).set_binding('pace')
+        # Create step protocol
+        dt = 0.1
+        steps = [
+            [-80, 250.1],
+            [-120, 50],
+            [-80, 200],
+            [40, 1000],
+            [-120, 500],
+            [-80, 1000],
+            [-30, 3500],
+            [-120, 500],
+            [-80, 1000],
+        ]
+        p = myokit.Protocol()
+        for f, t in steps:
+            p.add_step(f, t)
+        # Create set of times that overlap with change points
+        times = np.arange(80000) * dt
+        # Create simulation
+        s = myokit.Simulation(m, p)
+        # Run
+        d = s.run(8000, log_times=times).npview()
+        # Check if logging points show correct pacing value
+        # In an earlier implementation, rounding errors and a difference in the
+        # implementation of passing logpoints and passing protocol points could
+        # cause the log point to be just before the protocol change.
+        # In this case, a change at t=120.0 would only be picked up at t=120.1
+        # (but not consistently!)
+        # The below code checks for this
+        offset = 0
+        for v, t in steps[:-1]:
+            offset += t
+            e = d.trim(offset - dt, offset + 2 * dt)
+            self.assertNotEqual(e['membrane.V'][0], e['membrane.V'][1])
 
-        with TemporaryDirectory() as d:
-            # Create data log
-            log = myokit.DataLog()
-            log.set_time_key('time')
-            log['time'] = np.arange(100)
-            log['sint'] = np.sin(log['time'])
-            log['cost'] = np.cos(log['time'])
-
-            # Write atf file
-            path = d.path('test.atf')
-            axon.save_atf(log, path)
-
-            # Read atf file
-            log2 = axon.load_atf(path)
-            self.assertEqual(len(log), len(log2))
-            self.assertEqual(set(log.keys()), set(log2.keys()))
-            for k, v in log.items():
-                self.assertTrue(np.all(v == log2[k]))
-
-            # Write selected fields
-            axon.save_atf(log, path, fields=['time', 'sint'])
-            log2 = axon.load_atf(path)
-            self.assertEqual(set(log2.keys()), set(['time', 'sint']))
-
-            # Time must be regularly spaced
-            log['time'][-1] *= 2
-            self.assertRaisesRegex(
-                ValueError, 'regularly spaced', axon.save_atf, log, path)
-
-            # Field names can't contain quotes
-            log['time'] = np.arange(100)
-            log['si"nt'] = log['sint']
-            self.assertRaisesRegex(
-                ValueError, 'double quotes', axon.save_atf, log, path)
-
-            # Field names can't have newlines
-            del log['si"nt']
-            log['si\nnt'] = log['sint']
-            self.assertRaisesRegex(
-                ValueError, 'newlines', axon.save_atf, log, path)
-
-            # Fields in `fields` must exist
-            del log['si\nnt']
-            self.assertRaisesRegex(
-                ValueError, 'not found', axon.save_atf, log, path,
-                fields=['time', 'sint', 'hi'])
-
-            # Try using on other formats
-            log.save_csv(path)
-            self.assertRaisesRegex(Exception, 'file type', axon.load_atf, path)
-
-            # Try reading raw meta data (no key-value pairs)
-            with open(path, 'w') as f:
-                f.write('ATF\t1.0\n')
-                f.write('1\t3\n')
-                f.write('"Hello! This is raw meta data"\n')
-                f.write('"time"\t"sint"\t"cost"\n')
-                f.write('0\t0.0\t1.0\n')
-                f.write('1\t10\t20\n')
-                f.write('2\t30\t40\n')
-            log2 = axon.load_atf(path)
-
-            # Test invalid header detection
-            with open(path, 'w') as f:
-                f.write('ATF\t1.0\n')
-                f.write('1\t3\n')
-                f.write('Hello! This is raw meta data\n')
-                f.write('"time"\t"sint"\t"cost"\n')
-                f.write('0\t0.0\t1.0\n')
-                f.write('1\t10\t20\n')
-                f.write('2\t30\t40\n')
-            self.assertRaisesRegex(
-                Exception, 'double quotation', axon.load_atf, path)
-
-            # Bad column headers
-            with open(path, 'w') as f:
-                f.write('ATF\t1.0\n')
-                f.write('1\t3\n')
-                f.write('"Hello! This is raw meta data"\n')
-                f.write('Bonjou\t"time"\t"sint"\t"cost"\n')
-                f.write('0\t0.0\t1.0\n')
-                f.write('1\t10\t20\n')
-                f.write('2\t30\t40\n')
-            self.assertRaisesRegex(
-                Exception, 'column headers', axon.load_atf, path)
-
-            # Bad column headers
-            with open(path, 'w') as f:
-                f.write('ATF\t1.0\n')
-                f.write('1\t3\n')
-                f.write('"Hello! This is raw meta data"\n')
-                f.write('time"\t"sint"\t"cost"\n')
-                f.write('0\t0.0\t1.0\n')
-                f.write('1\t10\t20\n')
-                f.write('2\t30\t40\n')
-            self.assertRaisesRegex(
-                Exception, 'column headers', axon.load_atf, path)
-
-            # Too many headers
-            with open(path, 'w') as f:
-                f.write('ATF\t1.0\n')
-                f.write('1\t3\n')
-                f.write('"Hello! This is raw meta data"\n')
-                f.write('"Bonjour"\t"time"\t"sint"\t"cost"\n')
-                f.write('0\t0.0\t1.0\n')
-                f.write('1\t10\t20\n')
-                f.write('2\t30\t40\n')
-            self.assertRaisesRegex(
-                Exception, 'found 4', axon.load_atf, path)
-
-            # Commas as delimiter are ok
-            with open(path, 'w') as f:
-                f.write('ATF\t1.0\n')
-                f.write('1\t3\n')
-                f.write('"Hello! This is raw meta data"\n')
-                f.write('"time","sint","cost"\n')
-                f.write('0,0.0,1.0\n')
-                f.write('1,10,20\n')
-                f.write('2,30,40\n')
-            axon.load_atf(path)
-
-            # But can't mix them
-            with open(path, 'w') as f:
-                f.write('ATF\t1.0\n')
-                f.write('1\t3\n')
-                f.write('"Hello! This is raw meta data"\n')
-                f.write('"time"\t"sint","cost"\n')
-                f.write('0,0.0,1.0\n')
-                f.write('1,10,20\n')
-                f.write('2,30,40\n')
-            self.assertRaisesRegex(
-                Exception, 'Mixed delimiters', axon.load_atf, path)
-
-            # Too many columns
-            with open(path, 'w') as f:
-                f.write('ATF\t1.0\n')
-                f.write('1\t3\n')
-                f.write('"Hello! This is raw meta data"\n')
-                f.write('"time"\t"sint"\t"cost"\n')
-                f.write('0\t0.0\t1.0\n')
-                f.write('1\t10\t20\t100\n')
-                f.write('2\t30\t40\n')
-            self.assertRaisesRegex(
-                Exception, 'Invalid data', axon.load_atf, path)
-
-    def test_accessors(self):
-        # Test various accessor methods of :class:`AtfFile`.
-
-        with TemporaryDirectory() as d:
-            # Create data log
-            log = myokit.DataLog()
-            log.set_time_key('time')
-            log['time'] = np.arange(10)
-            log['sint'] = np.sin(log['time'])
-            log['cost'] = np.cos(log['time'])
-
-            # Write atf file
-            path = d.path('test.atf')
-            axon.save_atf(log, path)
-
-            # Read atf file
-            atf = myokit.formats.axon.AtfFile(path)
-
-            # Test filename()
-            self.assertEqual(atf.filename(), path)
-
-            # Test iter and getitem
-            self.assertEqual(len(list(iter(atf))), 3)
-            self.assertTrue(np.all(atf['time'] == log['time']))
-            self.assertTrue(np.all(atf['sint'] == log['sint']))
-            self.assertTrue(np.all(atf['cost'] == log['cost']))
-
-            # Test items()
-            items = list(atf.items())
-            self.assertEqual(items[0][0], 'time')
-            self.assertEqual(items[1][0], 'sint')
-            self.assertEqual(items[2][0], 'cost')
-            self.assertTrue(np.all(items[0][1] == log['time']))
-            self.assertTrue(np.all(items[1][1] == log['sint']))
-            self.assertTrue(np.all(items[2][1] == log['cost']))
-
-            # Test keys()
-            self.assertEqual(list(atf.keys()), ['time', 'sint', 'cost'])
-
-            # Test values()
-            values = list(atf.values())
-            self.assertTrue(np.all(values[0] == log['time']))
-            self.assertTrue(np.all(values[1] == log['sint']))
-            self.assertTrue(np.all(values[2] == log['cost']))
 
-            # Test len
-            self.assertEqual(len(atf), 3)
-
-            # Test info
-            self.assertIn('myokit', atf.info())
+class Simulation1dTest(PeriodicTest):
+    """
+    Tests myokit.Simulation1d for consistent log entry timing.
+    """
+    def test_periodic(self):
+        # Test periodic logging.
 
-            # Test version
-            self.assertEqual(atf.version(), '1.0')
+        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+        s = myokit.Simulation1d(m, p, ncells=1)
+        self.periodic(s)
 
 
 if __name__ == '__main__':
+    print('Add -v for more debug output')
+    import sys
+    if '-v' in sys.argv:
+        debug = True
     unittest.main()
```

### Comparing `myokit-1.35.0/myokit/tests/test_formats_cellml.py` & `myokit-1.35.1/myokit/tests/test_formats_cellml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_channelml.py` & `myokit-1.35.1/myokit/tests/test_formats_channelml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_easyml.py` & `myokit-1.35.1/myokit/tests/test_formats_easyml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_exporters.py` & `myokit-1.35.1/myokit/tests/test_formats_exporters.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_expression_writers.py` & `myokit-1.35.1/myokit/tests/test_formats_expression_writers.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_html.py` & `myokit-1.35.1/myokit/tests/test_formats_html.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_importers.py` & `myokit-1.35.1/myokit/tests/test_formats_importers.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_mathml_content.py` & `myokit-1.35.1/myokit/tests/test_formats_mathml_content.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_mathml_presentation.py` & `myokit-1.35.1/myokit/tests/test_formats_mathml_presentation.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_opencl.py` & `myokit-1.35.1/myokit/tests/test_formats_opencl.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_sbml.py` & `myokit-1.35.1/myokit/tests/test_formats_sbml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_formats_sympy.py` & `myokit-1.35.1/myokit/tests/test_formats_sympy.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_io.py` & `myokit-1.35.1/myokit/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_jacobian_calculator.py` & `myokit-1.35.1/myokit/tests/test_jacobian_calculator.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_jacobian_tracer.py` & `myokit-1.35.1/myokit/tests/test_jacobian_tracer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_lib_deps.py` & `myokit-1.35.1/myokit/tests/test_lib_deps.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_lib_guess.py` & `myokit-1.35.1/myokit/tests/test_lib_guess.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_lib_hh.py` & `myokit-1.35.1/myokit/tests/test_lib_hh.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_lib_markov.py` & `myokit-1.35.1/myokit/tests/test_lib_markov.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_lib_multi.py` & `myokit-1.35.1/myokit/tests/test_lib_multi.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_lib_plots.py` & `myokit-1.35.1/myokit/tests/test_lib_plots.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_meta.py` & `myokit-1.35.1/myokit/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_model.py` & `myokit-1.35.1/myokit/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_model_building.py` & `myokit-1.35.1/myokit/tests/test_model_building.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_opencl_info.py` & `myokit-1.35.1/myokit/tests/test_opencl_info.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_pacing_factory.py` & `myokit-1.35.1/myokit/tests/test_pacing_factory.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_pacing_system_py.py` & `myokit-1.35.1/myokit/tests/test_pacing_system_py.py`

 * *Files 12% similar despite different names*

```diff
@@ -85,10 +85,28 @@
         t = s.next_time()
         self.assertEqual(t, 2000)
         with self.assertRaises(myokit.SimultaneousProtocolEventError) as e:
             s.advance(t)
         m = str(e.exception)
         self.assertEqual(float(m[2 + m.index('t='):-1]), 3000)
 
+    def test_negative_time(self):
+        # Test starting from a negative time
+
+        p = myokit.pacing.blocktrain(level=1, duration=1, period=2)
+        s = myokit.PacingSystem(p, initial_time=-100)
+        self.assertEqual(s.time(), -100)
+        self.assertEqual(s.next_time(), 0)
+        self.assertEqual(s.pace(), 0)
+
+        p = myokit.pacing.blocktrain(level=1, duration=1, period=2, offset=1)
+        s = myokit.PacingSystem(p, initial_time=-100)
+        self.assertEqual(s.time(), -100)
+        self.assertEqual(s.next_time(), 1)
+        self.assertEqual(s.pace(), 0)
+        s.advance(s.next_time())
+        self.assertEqual(s.time(), 1)
+        self.assertEqual(s.pace(), 1)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `myokit-1.35.0/myokit/tests/test_parsing.py` & `myokit-1.35.1/myokit/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_progress_reporters.py` & `myokit-1.35.1/myokit/tests/test_progress_reporters.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_protocol.py` & `myokit-1.35.1/myokit/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_protocol_floating_point.py` & `myokit-1.35.1/myokit/tests/test_protocol_floating_point.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_protocol_time_series.py` & `myokit-1.35.1/myokit/tests/test_protocol_time_series.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_pype.py` & `myokit-1.35.1/myokit/tests/test_pype.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_quantity.py` & `myokit-1.35.1/myokit/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_rhs_benchmarker.py` & `myokit-1.35.1/myokit/tests/test_rhs_benchmarker.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_sbml_api.py` & `myokit-1.35.1/myokit/tests/test_sbml_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_sbml_parser.py` & `myokit-1.35.1/myokit/tests/test_sbml_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_simulation_1d.py` & `myokit-1.35.1/myokit/tests/test_simulation_1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,18 +49,14 @@
         s.reset()
         self.assertEqual(s.state(), s.default_state())
 
         # Test pre updates the default state.
         s.pre(1)
         self.assertNotEqual(s.default_state(0), x0)
 
-        # Test running without a protocol
-        s.set_protocol(None)
-        s.run(1)
-
         # Simulation time can't be negative
         self.assertRaises(ValueError, s.run, -1)
 
         # Number of cells must be >0
         self.assertRaisesRegex(
             ValueError, 'number of cells', myokit.Simulation1d, m, p, 0)
 
@@ -117,34 +113,57 @@
         self.assertIsInstance(x[0], float)
         self.assertIsInstance(x[1], float)
         self.assertIsInstance(x[2], float)
         self.assertEqual(x[:3], x[3:])
         self.assertEqual(x, m.initial_values(True) * 2)
         self.assertEqual(x, s.default_state())
 
-    def test_with_progress_reporter(self):
-        # Test running with a progress reporter.
-        m, p, _ = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+    def test_negative_time(self):
+        # Test starting at a negative time
 
-        # Test using a progress reporter
-        s = myokit.Simulation1d(m, p, ncells=5)
-        s.set_step_size(0.05)
-        with myokit.tools.capture() as c:
-            s.run(110, progress=myokit.ProgressPrinter())
-        c = c.text().splitlines()
-        self.assertTrue(len(c) > 0)
+        m = myokit.load_model(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+        p = myokit.pacing.blocktrain(duration=1, level=1, period=2)
+        n = 4
+        s = myokit.Simulation1d(m, p, ncells=n)
 
-        # Not a progress reporter
-        self.assertRaisesRegex(
-            ValueError, 'ProgressReporter', s.run, 5, progress=12)
+        s.set_time(-10)
+        self.assertEqual(s.time(), -10)
+        d = s.run(5, log=['engine.pace']).npview()
+        self.assertEqual(s.time(), -5)
+        self.assertTrue(np.all(d['engine.pace'] == 0))
+        d = s.run(6, log=['engine.time', 'engine.pace']).npview()
+        #print(d['engine.time'])
+        #print(d['engine.pace'])
+        self.assertEqual(s.time(), 1)
+        self.assertTrue(np.all(d['engine.pace'][:-1] == 0))
+        self.assertEqual(d['engine.pace'][-1], 1)
 
-        # Cancel from reporter
-        self.assertRaises(
-            myokit.SimulationCancelledError, s.run, 1,
-            progress=CancellingReporter(0))
+    def test_no_protocol(self):
+        # Test running without a protocol
+        m = myokit.load_model(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+        x = 0.123
+        m.get('engine.pace').set_rhs(x)
+        n = 4
+
+        # Create without a protocol
+        s = myokit.Simulation1d(m, ncells=n)
+        d = s.run(10, log=['engine.pace']).npview()
+        self.assertIn('engine.pace', d.keys())
+        self.assertTrue(np.all(d['engine.pace'] == 0))
+
+        # Set, then unset
+        y = 0.101
+        p = myokit.pacing.blocktrain(level=y, duration=100, period=100)
+        s.set_protocol(p)
+        d = s.run(5, log=['engine.pace']).npview()
+        self.assertTrue(np.all(d['engine.pace'] == y))
+        self.assertGreater(len(d['engine.pace']), 1)
+        s.set_protocol(None)
+        d = s.run(5, log=['engine.pace']).npview()
+        self.assertTrue(np.all(d['engine.pace'] == 0))
 
     def test_set_state(self):
         # Test :meth:`Simulation1d.set_state()`.
         m, p, _ = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
         n = 4
 
         s = myokit.Simulation1d(m, p, n)
@@ -214,14 +233,35 @@
         # Invalid cell index
         s.set_default_state(sx, 0)
         self.assertRaises(ValueError, s.set_default_state, sx, -1)
         self.assertRaises(ValueError, s.set_default_state, sx, n)
         self.assertRaises(ValueError, s.default_state, -1)
         self.assertRaises(ValueError, s.default_state, n)
 
+    def test_with_progress_reporter(self):
+        # Test running with a progress reporter.
+        m, p, _ = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+
+        # Test using a progress reporter
+        s = myokit.Simulation1d(m, p, ncells=5)
+        s.set_step_size(0.05)
+        with myokit.tools.capture() as c:
+            s.run(110, progress=myokit.ProgressPrinter())
+        c = c.text().splitlines()
+        self.assertTrue(len(c) > 0)
+
+        # Not a progress reporter
+        self.assertRaisesRegex(
+            ValueError, 'ProgressReporter', s.run, 5, progress=12)
+
+        # Cancel from reporter
+        self.assertRaises(
+            myokit.SimulationCancelledError, s.run, 1,
+            progress=CancellingReporter(0))
+
     def test_against_cvode(self):
         # Compare the Simulation1d output with CVODE output
 
         # Load model and event with appropriate level/duration
         m, p, _ = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
         e = p.head()
```

### Comparing `myokit-1.35.0/myokit/tests/test_simulation_cvodes.py` & `myokit-1.35.1/myokit/tests/test_simulation_cvodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,24 +223,73 @@
         # Test b
         b_e = 0.1 + 0.2 * np.sin(t)
         b_e[t > 10] = y[-1]
         # Note: We don't expect a super good match here, as b_e is an exact
         #       sine value, while the solver will be interpolating y
         np.testing.assert_array_almost_equal(d[b], b_e, decimal=3)
 
+    def test_negative_time(self):
+        # Test starting at a negative time
+
+        self.sim.reset()
+        self.sim.set_protocol(
+            myokit.pacing.blocktrain(duration=1, level=1, period=2))
+        self.sim.set_time(-10)
+        self.assertEqual(self.sim.time(), -10)
+        d = self.sim.run(5, log=['engine.pace']).npview()
+        self.assertEqual(self.sim.time(), -5)
+        self.assertTrue(np.all(d['engine.pace'] == 0))
+        d = self.sim.run(5, log=['engine.pace']).npview()
+        self.assertEqual(self.sim.time(), 0)
+        self.assertTrue(np.all(d['engine.pace'][:-1] == 0))
+        self.assertEqual(d['engine.pace'][-1], 1)
+        self.sim.set_protocol(self.protocol)
+
     def test_no_protocol(self):
         # Test running without a protocol.
 
+        # Check if pace was set to zero (see technical notes).
         self.sim.reset()
         self.sim.pre(50)
         self.sim.set_protocol(None)
-        d = self.sim.run(50).npview()
+        d = self.sim.run(50, log=['engine.pace']).npview()
+        self.assertTrue(np.all(d['engine.pace'] == 0))
+
+        # Defined at the start? Then still counts as bound
+        self.assertRaisesRegex(
+            ValueError, 'not a literal',
+            self.sim.set_constant, 'engine.pace', 1)
+
+        # Check that pace is reset to zero when protocol is removed
+        x = 0.01    # Note: Must be low to stop sim crashing :D
+        self.sim.set_protocol(
+            myokit.pacing.blocktrain(duration=1000, level=x, period=1000))
+        d = self.sim.run(5, log=['engine.pace']).npview()
+        self.assertTrue(np.all(d['engine.pace'] == x))
+        self.sim.set_protocol(None)
+        d = self.sim.run(5, log=['engine.pace']).npview()
+        self.assertTrue(np.all(d['engine.pace'] == 0))
+        self.sim.set_protocol(self.protocol)
+
+        # No protocol set from the start? Then "pace" is set anyway for
+        # backwards compatibility
+        m = self.model.clone()
+        m.get('engine.pace').set_rhs(x)
+        s = myokit.Simulation(m)
+        d = s.run(50).npview()
+        self.assertIn('engine.pace', d.keys())
+        self.assertTrue(np.all(d['engine.pace'] == 0))
 
-        # Check if pace was set to zero (see prop 651 / technical docs).
-        self.assertTrue(np.all(d['engine.pace'] == 0.0))
+        # But if user explicitly says no labels, then pace isn't treated in a
+        # special way.
+        s = myokit.Simulation(m, {})
+        self.assertRaises(ValueError, s.set_protocol, self.protocol)
+        d = s.run(50).npview()
+        self.assertNotIn('engine.pace', d.keys())
+        #self.assertTrue(np.all(d['engine.pace'] == x))  constant is not logged
 
     def test_wrong_label_set_pacing(self):
         # Test set_pacing with incorrect label
         self.sim.reset()
         self.sim.pre(50)
         with self.assertRaisesRegex(ValueError, 'Unknown pacing label'):
             self.sim.set_protocol(None, label='does not exist')
```

### Comparing `myokit-1.35.0/myokit/tests/test_simulation_cvodes_from_disk.py` & `myokit-1.35.1/myokit/tests/test_simulation_cvodes_from_disk.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_simulation_fiber_tissue.py` & `myokit-1.35.1/myokit/tests/test_simulation_fiber_tissue.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,14 +379,35 @@
             ValueError, 'tissue model must specify a unit for the diffusion',
             FT, mf, m2)
         m2.binding('diffusion_current').set_unit(myokit.units.pF)
         self.assertRaisesRegex(
             ValueError, 'diffusion current must have the same unit',
             FT, mf, m2)
 
+    def test_negative_time(self):
+        # Test starting at a negative time
+
+        p = myokit.pacing.blocktrain(duration=1, level=1, period=2)
+        self.s0.reset()
+        self.s0.set_protocol(p)
+        self.s0.set_time(-10)
+        self.assertEqual(self.s0.time(), -10)
+        df, dt = self.s0.run(5, logf=['engine.pace'], logt=myokit.LOG_NONE)
+        df = df.npview()
+        self.assertEqual(self.s0.time(), -5)
+        self.assertTrue(np.all(df['engine.pace'] == 0))
+        df, dt = self.s0.run(
+            6, logf=['engine.time', 'engine.pace'], logt=myokit.LOG_NONE)
+        df = df.npview()
+        #print(d['engine.time'])
+        #print(d['engine.pace'])
+        self.assertEqual(self.s0.time(), 1)
+        self.assertTrue(np.all(df['engine.pace'][:-1] == 0))
+        self.assertEqual(df['engine.pace'][-1], 1)
+
     def test_pre_reset(self):
         # Tests getting/setting of states and time, and use of pre() and run()
         try:
             # Check setting of time
             self.assertEqual(self.s1.time(), 0)
             self.s1.set_time(10)
             self.assertEqual(self.s1.time(), 10)
@@ -464,23 +485,33 @@
         try:
             # Run, check Vm is raised
             df, dt = self.s0.run(
                 5, logf=['membrane.V'], logt=myokit.LOG_NONE, log_interval=1)
             self.assertGreater(df['membrane.V', 0, 0][-1], 0)
             self.s0.reset()
 
-            # Unset protocol, check Vm stays low
+            # Run with constant proto
+            x = 0.0123
+            self.s0.set_protocol(
+                myokit.pacing.blocktrain(level=x, duration=1000, period=1000))
+            self.s0.reset()
+            df, dt = self.s0.run(3, logf=['engine.pace'])
+            df = df.npview()
+            self.assertTrue(np.all(df['engine.pace'] == x))
+
+            # Unset: Must now be zero
             self.s0.set_protocol(None)
-            df, dt = self.s0.run(
-                5, logf=['membrane.V'], logt=myokit.LOG_NONE, log_interval=1)
-            self.assertLess(df['membrane.V', 0, 0][-1], 0)
             self.s0.reset()
+            df, dt = self.s0.run(3, logf=['engine.pace'])
+            df = df.npview()
+            self.assertTrue(np.all(df['engine.pace'] == 0))
 
             # Reset protocol, check Vm goes high
             self.s0.set_protocol(self.p)
+            self.s0.reset()
             df, dt = self.s0.run(
                 5, logf=['membrane.V'], logt=myokit.LOG_NONE, log_interval=1)
             self.assertGreater(df['membrane.V', 0, 0][-1], 0)
         finally:
             self.s0.reset()
 
     def test_run_errors(self):
```

### Comparing `myokit-1.35.0/myokit/tests/test_simulation_opencl.py` & `myokit-1.35.1/myokit/tests/test_simulation_opencl.py`

 * *Files 1% similar despite different names*

```diff
@@ -678,14 +678,32 @@
         self.assertIsInstance(x[0], float)
         self.assertIsInstance(x[1], float)
         self.assertIsInstance(x[2], float)
         self.assertEqual(x[:3], x[3:])
         self.assertEqual(x, m.initial_values(True) * 2)
         self.assertEqual(x, s.default_state())
 
+    def test_negative_time(self):
+        # Test starting at a negative time
+
+        p = myokit.pacing.blocktrain(duration=1, level=1, period=2)
+        self.s0.reset()
+        self.s0.set_protocol(p)
+        self.s0.set_time(-10)
+        self.assertEqual(self.s0.time(), -10)
+        d = self.s0.run(5, log=['engine.pace']).npview()
+        self.assertEqual(self.s0.time(), -5)
+        self.assertTrue(np.all(d['engine.pace'] == 0))
+        d = self.s0.run(6, log=['engine.time', 'engine.pace']).npview()
+        #print(d['engine.time'])
+        #print(d['engine.pace'])
+        self.assertEqual(self.s0.time(), 1)
+        self.assertTrue(np.all(d['engine.pace'][:-1] == 0))
+        self.assertEqual(d['engine.pace'][-1], 1)
+
     def test_neighbors_0d(self):
         # Test listing neighbors in a 0d simulation
 
         x = self.s0.neighbors(0)
         self.assertEqual(len(x), 0)
         self.assertRaisesRegex(
             IndexError, 'out of range', self.s0.neighbors, -1)
@@ -809,19 +827,27 @@
 
         # Run with protocol, check for depolarisation
         self.s0.reset()
         d0 = self.s0.run(3, log=['engine.pace']).npview()
         self.assertEqual(np.max(d0['engine.pace']), 1)
 
         try:
-            # Unset protocol
+            # Make pace high
+            x = 0.0123
+            self.s0.set_protocol(
+                myokit.pacing.blocktrain(level=x, duration=1000, period=1000))
+            self.s0.reset()
+            d0 = self.s0.run(3, log=['engine.pace']).npview()
+            self.assertTrue(np.all(d0['engine.pace'] == x))
+
+            # Unset protocol: pace must now be 0
             self.s0.reset()
             self.s0.set_protocol(None)
             d0 = self.s0.run(3, log=['engine.pace']).npview()
-            self.assertEqual(np.max(d0['engine.pace']), 0)
+            self.assertTrue(np.all(d0['engine.pace'] == 0))
 
             # Add new protocol
             p = myokit.pacing.blocktrain(period=1000, duration=2, offset=3)
             self.s0.reset()
             self.s0.set_protocol(p)
             d0 = self.s0.run(3, log=['engine.pace']).npview()
             self.assertEqual(np.max(d0['engine.pace']), 0)
@@ -870,16 +896,14 @@
             self.assertEqual(0, self.s0.time())
 
             # Test setting time
             self.s0.set_time(10)
             self.assertEqual(self.s0.time(), 10)
             self.s0.run(1)
             self.assertEqual(self.s0.time(), 11)
-            self.assertRaisesRegex(
-                ValueError, 'negative', self.s0.set_time, -1)
 
             # Test running for a negative amount of time
             self.assertRaisesRegex(
                 ValueError, 'negative', self.s0.run, -1)
 
         finally:
             self.s0.set_default_state(x0)
```

### Comparing `myokit-1.35.0/myokit/tests/test_simulation_opencl_log_interval.py` & `myokit-1.35.1/myokit/tests/test_simulation_opencl_log_interval.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_simulation_opencl_vs_cvode.py` & `myokit-1.35.1/myokit/tests/test_simulation_opencl_vs_cvode.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_simulation_opencl_vs_sim1d.py` & `myokit-1.35.1/myokit/tests/test_simulation_opencl_vs_sim1d.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_system_info.py` & `myokit-1.35.1/myokit/tests/test_system_info.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_tools.py` & `myokit-1.35.1/myokit/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_unit.py` & `myokit-1.35.1/myokit/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_user_functions.py` & `myokit-1.35.1/myokit/tests/test_user_functions.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tests/test_variable.py` & `myokit-1.35.1/myokit/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/tools.py` & `myokit-1.35.1/myokit/tools.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit/units.py` & `myokit-1.35.1/myokit/units.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.0/myokit.egg-info/PKG-INFO` & `myokit-1.35.1/myokit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myokit
-Version: 1.35.0
+Version: 1.35.1
 Summary: A simple interface to cardiac cellular electrophysiology
 Home-page: http://myokit.org
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/MichaelClerx/myokit/issues
 Project-URL: Documentation, http://docs.myokit.org
```

### Comparing `myokit-1.35.0/myokit.egg-info/SOURCES.txt` & `myokit-1.35.1/myokit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,17 @@
 myokit/formats/cuda/__init__.py
 myokit/formats/cuda/_ewriter.py
 myokit/formats/cuda/_exporter.py
 myokit/formats/cuda/template/kernel.cu
 myokit/formats/easyml/__init__.py
 myokit/formats/easyml/_ewriter.py
 myokit/formats/easyml/_exporter.py
+myokit/formats/heka/__init__.py
+myokit/formats/heka/_importer.py
+myokit/formats/heka/_patchmaster.py
 myokit/formats/html/__init__.py
 myokit/formats/html/_exporter.py
 myokit/formats/html/_flatten.py
 myokit/formats/latex/__init__.py
 myokit/formats/latex/_ewriter.py
 myokit/formats/latex/_exporter.py
 myokit/formats/mathml/__init__.py
@@ -207,15 +210,15 @@
 myokit/lib/guess.py
 myokit/lib/hh.py
 myokit/lib/markov.py
 myokit/lib/multi.py
 myokit/lib/plots.py
 myokit/tests/__init__.py
 myokit/tests/ansic_event_based_pacing.py
-myokit/tests/ansic_fixed_form_pacing.py
+myokit/tests/ansic_time_series_pacing.py
 myokit/tests/test_aux.py
 myokit/tests/test_cellml_v1_api.py
 myokit/tests/test_cellml_v1_parser.py
 myokit/tests/test_cellml_v1_writer.py
 myokit/tests/test_cellml_v2_api.py
 myokit/tests/test_cellml_v2_parser.py
 myokit/tests/test_cellml_v2_writer.py
```

### Comparing `myokit-1.35.0/setup.py` & `myokit-1.35.1/setup.py`

 * *Files identical despite different names*

