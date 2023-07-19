# Comparing `tmp/pyfem-0.1.1.tar.gz` & `tmp/pyfem-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.1.1.tar", last modified: Tue Jul  4 03:24:57 2023, max compression
+gzip compressed data, was "pyfem-0.1.2.tar", last modified: Wed Jul 19 05:49:14 2023, max compression
```

## Comparing `pyfem-0.1.1.tar` & `pyfem-0.1.2.tar`

### file list

```diff
@@ -1,88 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.895680 pyfem-0.1.1/
--rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4373 2023-07-04 03:24:57.895680 pyfem-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3848 2023-06-15 07:05:17.000000 pyfem-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 03:24:57.895680 pyfem-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-07-04 03:24:27.000000 pyfem-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.813681 pyfem-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.824681 pyfem-0.1.1/src/pyfem/
--rw-rw-rw-   0        0        0     1025 2023-06-30 04:12:57.000000 pyfem-0.1.1/src/pyfem/Job.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0      277 2023-05-22 03:59:51.000000 pyfem-0.1.1/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.834681 pyfem-0.1.1/src/pyfem/amplitude/
--rw-rw-rw-   0        0        0      924 2023-06-09 08:03:09.000000 pyfem-0.1.1/src/pyfem/amplitude/BaseAmplitude.py
--rw-rw-rw-   0        0        0     1357 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/amplitude/TabularAmplitude.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/amplitude/__init__.py
--rw-rw-rw-   0        0        0      818 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/amplitude/get_amplitude_data.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.836681 pyfem-0.1.1/src/pyfem/assembly/
--rw-rw-rw-   0        0        0    10194 2023-07-03 09:00:51.000000 pyfem-0.1.1/src/pyfem/assembly/Assembly.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.844679 pyfem-0.1.1/src/pyfem/bc/
--rw-rw-rw-   0        0        0     1672 2023-06-30 06:18:06.000000 pyfem-0.1.1/src/pyfem/bc/BaseBC.py
--rw-rw-rw-   0        0        0     2406 2023-06-29 04:23:17.000000 pyfem-0.1.1/src/pyfem/bc/DirichletBC.py
--rw-rw-rw-   0        0        0     3706 2023-06-09 08:02:51.000000 pyfem-0.1.1/src/pyfem/bc/NeumannBC.py
--rw-rw-rw-   0        0        0     2844 2023-07-03 03:24:41.000000 pyfem-0.1.1/src/pyfem/bc/NeumannBCConcentrated.py
--rw-rw-rw-   0        0        0     8757 2023-06-30 10:22:55.000000 pyfem-0.1.1/src/pyfem/bc/NeumannBCDistributed.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/bc/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-07-03 03:24:41.000000 pyfem-0.1.1/src/pyfem/bc/get_bc_data.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.854680 pyfem-0.1.1/src/pyfem/elements/
--rw-rw-rw-   0        0        0     9323 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0     2315 2023-05-30 06:11:08.000000 pyfem-0.1.1/src/pyfem/elements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    37158 2023-06-30 07:52:18.000000 pyfem-0.1.1/src/pyfem/elements/IsoElementShape.py
--rw-rw-rw-   0        0        0     9927 2023-07-03 08:49:00.000000 pyfem-0.1.1/src/pyfem/elements/SolidPlaneSmallStrain.py
--rw-rw-rw-   0        0        0    13761 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/elements/SolidThermalPlaneSmallStrain.py
--rw-rw-rw-   0        0        0    10693 2023-07-03 08:47:31.000000 pyfem-0.1.1/src/pyfem/elements/SolidVolumeSmallStrain.py
--rw-rw-rw-   0        0        0     7580 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/elements/ThermalStatic.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/elements/__init__.py
--rw-rw-rw-   0        0        0     2515 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/elements/get_element_data.py
--rw-rw-rw-   0        0        0     1842 2023-06-08 06:40:10.000000 pyfem-0.1.1/src/pyfem/elements/get_iso_element_type.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.857680 pyfem-0.1.1/src/pyfem/fem/
--rw-rw-rw-   0        0        0      897 2023-06-01 03:56:06.000000 pyfem-0.1.1/src/pyfem/fem/Timer.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/fem/__init__.py
--rw-rw-rw-   0        0        0       68 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/fem/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.870678 pyfem-0.1.1/src/pyfem/io/
--rw-rw-rw-   0        0        0      592 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/io/Amplitude.py
--rw-rw-rw-   0        0        0      888 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0      614 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/io/Dof.py
--rw-rw-rw-   0        0        0     2449 2023-06-19 04:15:35.000000 pyfem-0.1.1/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      538 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0      612 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0    10307 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0      859 2023-07-03 03:48:49.000000 pyfem-0.1.1/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0      821 2023-06-01 09:39:23.000000 pyfem-0.1.1/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1741 2023-07-04 03:24:43.000000 pyfem-0.1.1/src/pyfem/io/arguments.py
--rw-rw-rw-   0        0        0     4622 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/io/write_vtk.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.878680 pyfem-0.1.1/src/pyfem/materials/
--rw-rw-rw-   0        0        0     1293 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     7014 2023-07-03 08:58:44.000000 pyfem-0.1.1/src/pyfem/materials/ElasticIsotropic.py
--rw-rw-rw-   0        0        0     6871 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/materials/PlasticKinematicHardening.py
--rw-rw-rw-   0        0        0     2061 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/materials/ThermalIsotropic.py
--rw-rw-rw-   0        0        0     5711 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/materials/ViscoElasticMaxwell.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/materials/__init__.py
--rw-rw-rw-   0        0        0     1551 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/materials/get_material_data.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.882681 pyfem-0.1.1/src/pyfem/mesh/
--rw-rw-rw-   0        0        0     4977 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/mesh/ElementSet.py
--rw-rw-rw-   0        0        0     6572 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/mesh/MeshData.py
--rw-rw-rw-   0        0        0     5036 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/mesh/NodeSet.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.887680 pyfem-0.1.1/src/pyfem/solvers/
--rw-rw-rw-   0        0        0      700 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/solvers/BaseSolver.py
--rw-rw-rw-   0        0        0     1603 2023-07-03 03:24:41.000000 pyfem-0.1.1/src/pyfem/solvers/LinearSolver.py
--rw-rw-rw-   0        0        0     8733 2023-07-03 03:24:41.000000 pyfem-0.1.1/src/pyfem/solvers/NonlinearSolver.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/solvers/__init__.py
--rw-rw-rw-   0        0        0      991 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/solvers/get_solver_data.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.893680 pyfem-0.1.1/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2350 2023-06-02 03:00:28.000000 pyfem-0.1.1/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      795 2023-05-30 02:50:20.000000 pyfem-0.1.1/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0     1518 2023-05-30 02:23:43.000000 pyfem-0.1.1/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0     2352 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/utils/visualization.py
--rw-rw-rw-   0        0        0     1046 2023-05-30 02:47:20.000000 pyfem-0.1.1/src/pyfem/utils/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.830680 pyfem-0.1.1/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0     4373 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.262223 pyfem-0.1.2/
+-rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4520 2023-07-19 05:49:14.262223 pyfem-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3997 2023-07-07 05:28:59.000000 pyfem-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-19 05:49:14.262223 pyfem-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-07-19 05:46:31.000000 pyfem-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.179223 pyfem-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.189223 pyfem-0.1.2/src/pyfem/
+-rw-rw-rw-   0        0        0     1407 2023-07-13 07:39:17.000000 pyfem-0.1.2/src/pyfem/Job.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0      277 2023-05-22 03:59:51.000000 pyfem-0.1.2/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.199223 pyfem-0.1.2/src/pyfem/amplitude/
+-rw-rw-rw-   0        0        0      988 2023-07-13 06:20:15.000000 pyfem-0.1.2/src/pyfem/amplitude/BaseAmplitude.py
+-rw-rw-rw-   0        0        0     1525 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/amplitude/TabularAmplitude.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/amplitude/__init__.py
+-rw-rw-rw-   0        0        0      818 2023-06-09 03:34:39.000000 pyfem-0.1.2/src/pyfem/amplitude/get_amplitude_data.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.202223 pyfem-0.1.2/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0    11052 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.208223 pyfem-0.1.2/src/pyfem/bc/
+-rw-rw-rw-   0        0        0     2168 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     2200 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0     2648 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/bc/NeumannBCConcentrated.py
+-rw-rw-rw-   0        0        0     8922 2023-07-14 04:08:19.000000 pyfem-0.1.2/src/pyfem/bc/NeumannBCDistributed.py
+-rw-rw-rw-   0        0        0     9036 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/bc/NeumannBCPressure.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0     1484 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.220223 pyfem-0.1.2/src/pyfem/elements/
+-rw-rw-rw-   0        0        0    14002 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0     2311 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    40943 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/elements/IsoElementShape.py
+-rw-rw-rw-   0        0        0    10577 2023-07-19 03:59:10.000000 pyfem-0.1.2/src/pyfem/elements/SolidPhaseFieldDamagePlaneSmallStrain.py
+-rw-rw-rw-   0        0        0     9927 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/SolidPlaneSmallStrain.py
+-rw-rw-rw-   0        0        0    12780 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/SolidThermalPlaneSmallStrain.py
+-rw-rw-rw-   0        0        0    10689 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/SolidVolumeSmallStrain.py
+-rw-rw-rw-   0        0        0     7570 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/Thermal.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0      939 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/elements/derive.py
+-rw-rw-rw-   0        0        0     2829 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/get_element_data.py
+-rw-rw-rw-   0        0        0     1842 2023-06-08 06:40:10.000000 pyfem-0.1.2/src/pyfem/elements/get_iso_element_type.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.223223 pyfem-0.1.2/src/pyfem/fem/
+-rw-rw-rw-   0        0        0     1148 2023-07-13 07:26:47.000000 pyfem-0.1.2/src/pyfem/fem/Timer.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/fem/__init__.py
+-rw-rw-rw-   0        0        0       68 2023-06-08 03:23:23.000000 pyfem-0.1.2/src/pyfem/fem/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.236225 pyfem-0.1.2/src/pyfem/io/
+-rw-rw-rw-   0        0        0      596 2023-07-13 09:14:21.000000 pyfem-0.1.2/src/pyfem/io/Amplitude.py
+-rw-rw-rw-   0        0        0     1077 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0     1584 2023-07-13 09:07:55.000000 pyfem-0.1.2/src/pyfem/io/BaseIO.py
+-rw-rw-rw-   0        0        0      511 2023-07-13 08:44:15.000000 pyfem-0.1.2/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     2586 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      417 2023-07-13 08:45:45.000000 pyfem-0.1.2/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0      534 2023-07-13 08:46:22.000000 pyfem-0.1.2/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0     7966 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0      900 2023-07-13 08:42:59.000000 pyfem-0.1.2/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0      999 2023-07-14 02:39:28.000000 pyfem-0.1.2/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1741 2023-07-19 05:46:59.000000 pyfem-0.1.2/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     5160 2023-07-19 03:59:10.000000 pyfem-0.1.2/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.246223 pyfem-0.1.2/src/pyfem/materials/
+-rw-rw-rw-   0        0        0     2290 2023-07-13 06:56:12.000000 pyfem-0.1.2/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     7243 2023-07-14 03:34:03.000000 pyfem-0.1.2/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0     2699 2023-07-13 05:52:00.000000 pyfem-0.1.2/src/pyfem/materials/MechanicalThermalExpansion.py
+-rw-rw-rw-   0        0        0     1509 2023-07-13 05:49:56.000000 pyfem-0.1.2/src/pyfem/materials/PhaseFieldDamage.py
+-rw-rw-rw-   0        0        0     7668 2023-07-13 05:54:25.000000 pyfem-0.1.2/src/pyfem/materials/PlasticKinematicHardening.py
+-rw-rw-rw-   0        0        0     2297 2023-07-13 05:55:59.000000 pyfem-0.1.2/src/pyfem/materials/ThermalIsotropic.py
+-rw-rw-rw-   0        0        0     6221 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/materials/ViscoElasticMaxwell.py
+-rw-rw-rw-   0        0        0     6248 2023-07-13 05:58:59.000000 pyfem-0.1.2/src/pyfem/materials/ViscoElasticMaxwellUMAT.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0     1801 2023-07-06 05:22:46.000000 pyfem-0.1.2/src/pyfem/materials/get_material_data.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.248223 pyfem-0.1.2/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     6852 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/mesh/MeshData.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.252223 pyfem-0.1.2/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0      930 2023-07-13 06:55:29.000000 pyfem-0.1.2/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0     1838 2023-07-13 06:57:34.000000 pyfem-0.1.2/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0     9277 2023-07-13 06:58:09.000000 pyfem-0.1.2/src/pyfem/solvers/NonlinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0      991 2023-06-09 03:34:39.000000 pyfem-0.1.2/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.261223 pyfem-0.1.2/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2443 2023-07-14 02:39:28.000000 pyfem-0.1.2/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      795 2023-05-30 02:50:20.000000 pyfem-0.1.2/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0      769 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/utils/data_types.py
+-rw-rw-rw-   0        0        0     1814 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/utils/derive.py
+-rw-rw-rw-   0        0        0     1518 2023-05-30 02:23:43.000000 pyfem-0.1.2/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0     5032 2023-07-14 05:55:14.000000 pyfem-0.1.2/src/pyfem/utils/mechanics.py
+-rw-rw-rw-   0        0        0     3722 2023-07-13 07:29:45.000000 pyfem-0.1.2/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0     1046 2023-05-30 02:47:20.000000 pyfem-0.1.2/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.195222 pyfem-0.1.2/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0     4520 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2479 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.1.1/LICENSE` & `pyfem-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.1/PKG-INFO` & `pyfem-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.1.1
+Version: 0.1.2
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,47 +27,47 @@
 pip install pyfem
 ```
 
 ## Development
 
 ### ToDo list
 
-- [ ] 增加Neumann边界条件，支持concentrated force，pressure，traction和函数定义方式
+- [x] 增加Neumann边界条件，支持concentrated force，distributed和pressure定义方式
 - [ ] 增加hdf5计算结果输出格式
 - [ ] 完善帮助文档
 - [ ] 完善输入文件的校检
-- [ ] 增加测试模块
+- [x] 增加测试模块
 - [ ] 增加日志模块
 - [ ] 增加后台运行模式
 - [ ] 处理平面应力状态的面外应力平衡
 - [x] 增加粘弹性力学本构模型
 - [ ] 增加晶体塑性力学本构模型
-- [ ] 增加温度场求解单元
-- [ ] 增加温度场-位移场耦合求解单元
-- [ ] 增加相场-位移场耦合求解单元
+- [x] 增加温度场求解单元
+- [x] 增加温度场-位移场耦合求解单元
+- [x] 增加相场-位移场耦合求解单元
 - [ ] 增加内聚区单元
 - [ ] 增加动力学求解器
 - [ ] 建立前处理界面
 
 ## Tutorial
 
 #### Run in command line:
 
 ```bash
 pyfem -i Job-1.toml
 ```
 
-#### Example with geometry file:
+#### Job file Job-1.toml:
 
 ```toml
 title = "Job-1"
 
 [mesh]
 type = "abaqus"
-file = "Job-1.inp"
+file = "hex8.inp"
 
 [dof]
 names = ["u1", "u2", "u3"]
 order = 1
 family = "LAGRANGE"
 
 [[bcs]]
@@ -95,27 +95,27 @@
 dof = ["u3"]
 node_sets = ['Set-Z0']
 element_sets = []
 value = 0.0
 
 [[bcs]]
 name = "BC-4"
-category = "DirichletBC"
-type = ""
+category = "NeumannBC"
+type = "Distributed"
 dof = ["u1"]
 node_sets = ['Set-X1']
-element_sets = []
+element_sets = ['Set-X1']
 value = 1.0
 
 [solver]
 type = "NonlinearSolver"
 option = "NewtonRaphson"
-total_time = 0.01
+total_time = 1.0
 max_increment = 1000000
-initial_dtime = 0.001
+initial_dtime = 0.1
 max_dtime = 1.0
 min_dtime = 0.001
 
 [[materials]]
 name = "Material-1"
 category = "Plastic"
 type = "KinematicHardening"
@@ -131,24 +131,24 @@
 
 [[sections]]
 name = "Section-1"
 category = "Solid"
 type = "Volume"
 option = "SmallStrain"
 element_sets = ["Set-All"]
-material_name = "Material-1"
+material_names = ["Material-1"]
 data = []
 
 [[outputs]]
 type = "vtk"
 field_outputs = ['S11', 'S22', 'S33', 'S12', 'S13', 'S23', 'E11', 'E22', 'E33', 'E12', 'E13', 'E23']
 on_screen = false
 ```
 
-### geometry file in abaqus formate:
+#### abaqus geometry file hex8.inp:
 
 ```abaqus
 *Heading
 *Preprint, echo=NO, model=NO, history=NO, contact=NO
 **
 ** PARTS
 **
@@ -200,7 +200,11 @@
 *Assembly, name=Assembly
 **  
 *Instance, name=Part-1-1, part=Part-1
 *End Instance
 **  
 *End Assembly
 ```
+
+### Bug list
+
+- [ ] 采用abaqus网格文件时，如果存在node不属于任何element则在计算时会导致全局刚度矩阵奇异。
```

### Comparing `pyfem-0.1.1/README.md` & `pyfem-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -12,47 +12,47 @@
 pip install pyfem
 ```
 
 ## Development
 
 ### ToDo list
 
-- [ ] 增加Neumann边界条件，支持concentrated force，pressure，traction和函数定义方式
+- [x] 增加Neumann边界条件，支持concentrated force，distributed和pressure定义方式
 - [ ] 增加hdf5计算结果输出格式
 - [ ] 完善帮助文档
 - [ ] 完善输入文件的校检
-- [ ] 增加测试模块
+- [x] 增加测试模块
 - [ ] 增加日志模块
 - [ ] 增加后台运行模式
 - [ ] 处理平面应力状态的面外应力平衡
 - [x] 增加粘弹性力学本构模型
 - [ ] 增加晶体塑性力学本构模型
-- [ ] 增加温度场求解单元
-- [ ] 增加温度场-位移场耦合求解单元
-- [ ] 增加相场-位移场耦合求解单元
+- [x] 增加温度场求解单元
+- [x] 增加温度场-位移场耦合求解单元
+- [x] 增加相场-位移场耦合求解单元
 - [ ] 增加内聚区单元
 - [ ] 增加动力学求解器
 - [ ] 建立前处理界面
 
 ## Tutorial
 
 #### Run in command line:
 
 ```bash
 pyfem -i Job-1.toml
 ```
 
-#### Example with geometry file:
+#### Job file Job-1.toml:
 
 ```toml
 title = "Job-1"
 
 [mesh]
 type = "abaqus"
-file = "Job-1.inp"
+file = "hex8.inp"
 
 [dof]
 names = ["u1", "u2", "u3"]
 order = 1
 family = "LAGRANGE"
 
 [[bcs]]
@@ -80,27 +80,27 @@
 dof = ["u3"]
 node_sets = ['Set-Z0']
 element_sets = []
 value = 0.0
 
 [[bcs]]
 name = "BC-4"
-category = "DirichletBC"
-type = ""
+category = "NeumannBC"
+type = "Distributed"
 dof = ["u1"]
 node_sets = ['Set-X1']
-element_sets = []
+element_sets = ['Set-X1']
 value = 1.0
 
 [solver]
 type = "NonlinearSolver"
 option = "NewtonRaphson"
-total_time = 0.01
+total_time = 1.0
 max_increment = 1000000
-initial_dtime = 0.001
+initial_dtime = 0.1
 max_dtime = 1.0
 min_dtime = 0.001
 
 [[materials]]
 name = "Material-1"
 category = "Plastic"
 type = "KinematicHardening"
@@ -116,24 +116,24 @@
 
 [[sections]]
 name = "Section-1"
 category = "Solid"
 type = "Volume"
 option = "SmallStrain"
 element_sets = ["Set-All"]
-material_name = "Material-1"
+material_names = ["Material-1"]
 data = []
 
 [[outputs]]
 type = "vtk"
 field_outputs = ['S11', 'S22', 'S33', 'S12', 'S13', 'S23', 'E11', 'E22', 'E33', 'E12', 'E13', 'E23']
 on_screen = false
 ```
 
-### geometry file in abaqus formate:
+#### abaqus geometry file hex8.inp:
 
 ```abaqus
 *Heading
 *Preprint, echo=NO, model=NO, history=NO, contact=NO
 **
 ** PARTS
 **
@@ -184,8 +184,12 @@
 **
 *Assembly, name=Assembly
 **  
 *Instance, name=Part-1-1, part=Part-1
 *End Instance
 **  
 *End Assembly
-```
+```
+
+### Bug list
+
+- [ ] 采用abaqus网格文件时，如果存在node不属于任何element则在计算时会导致全局刚度矩阵奇异。
```

### Comparing `pyfem-0.1.1/setup.py` & `pyfem-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfem",
-    version="0.1.1",
+    version="0.1.2",
     author="Jingyu Sun",
     author_email="sun.jingyu@outlook.com",
     description="A finite element package for learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sunwhale/pyfem",
     project_urls={
```

### Comparing `pyfem-0.1.1/src/pyfem/Job.py` & `pyfem-0.1.2/src/pyfem/Job.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from pathlib import Path
-from typing import Union
+from typing import Tuple, Union
 
 from pyfem.assembly.Assembly import Assembly
 from pyfem.io.Properties import Properties
 from pyfem.solvers.get_solver_data import get_solver_data
-from pyfem.utils.visualization import object_dict_to_string
+from pyfem.utils.visualization import object_slots_to_string
 
 
 class Job:
+    __slots__: Tuple = ('input_file', 'work_directory', 'abs_input_file', 'props', 'assembly', 'solver_data')
+
     def __init__(self, filename: Union[Path, str]) -> None:
         input_file = Path(filename)
         if input_file.is_absolute():
             abs_input_file = input_file
         else:
-            abs_input_file = Path.cwd().joinpath(input_file)
+            abs_input_file = Path.cwd().joinpath(input_file).resolve()
+        self.input_file = input_file
+        self.work_directory = Path.cwd()
+        self.abs_input_file = abs_input_file
         self.props = Properties()
         self.props.read_file(abs_input_file)
         # self.props.show()
         self.assembly = Assembly(self.props)
         self.solver_data = get_solver_data(self.assembly, self.props.solver)
 
-    def run(self):
-        self.solver_data.run()
+    def run(self) -> int:
+        return self.solver_data.run()
 
     def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string(self, level)
+        return object_slots_to_string(self, level)
 
     def show(self) -> None:
         print(self.to_string())
+
+
+if __name__ == '__main__':
+    job = Job(r'..\..\examples\mechanical\plane\Job-1.toml')
+    job.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/amplitude/TabularAmplitude.py` & `pyfem-0.1.2/src/pyfem/amplitude/TabularAmplitude.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 from pyfem.amplitude.BaseAmplitude import BaseAmplitude
 from pyfem.io.Amplitude import Amplitude
 from pyfem.utils.colors import error_style
 
 
 class TabularAmplitude(BaseAmplitude):
+    __slots__ = BaseAmplitude.__slots__ + ('table',)
+
     def __init__(self, amplitude: Amplitude) -> None:
         super().__init__()
         self.start = amplitude.start
         self.table: ndarray = array(amplitude.data)
         if self.table.ndim != 2:
             raise NotImplementedError(error_style('dimension of amplitude table must be 2'))
         elif self.table.shape[1] != 2:
@@ -27,13 +29,13 @@
                                               fill_value='extrapolate')
 
     def get_amplitude(self, time: float) -> float:
         return self.f_amplitude(time) + self.start
 
 
 if __name__ == "__main__":
-    time_table = [
-        [0.0, 0.0],
-        [1.0, 1.0],
-        [10.0, 2.0]
-    ]
-    pass
+    from pyfem.io.Properties import Properties
+
+    props = Properties()
+    props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
+    amp = TabularAmplitude(props.amplitudes[0])
+    amp.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/amplitude/get_amplitude_data.py` & `pyfem-0.1.2/src/pyfem/amplitude/get_amplitude_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.1/src/pyfem/assembly/Assembly.py` & `pyfem-0.1.2/src/pyfem/assembly/Assembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import List, Dict
+from typing import List, Dict, Tuple
 
 from numpy import repeat, array, ndarray, empty, zeros
 from scipy.sparse import coo_matrix, csc_matrix  # type: ignore
 
 from pyfem.bc.BaseBC import BaseBC
 from pyfem.bc.get_bc_data import get_bc_data
 from pyfem.elements.BaseElement import BaseElement
@@ -14,15 +14,15 @@
 from pyfem.elements.get_element_data import get_element_data
 from pyfem.elements.get_iso_element_type import get_iso_element_type
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Properties import Properties
 from pyfem.materials.get_material_data import get_material_data
 from pyfem.utils.colors import error_style
-from pyfem.utils.visualization import object_dict_to_string_assembly
+from pyfem.utils.visualization import object_slots_to_string_assembly
 from pyfem.utils.wrappers import show_running_time
 
 iso_element_shape_dict = {
     'line2': IsoElementShape('line2'),
     'line3': IsoElementShape('line3'),
     'tria3': IsoElementShape('tria3'),
     'tria6': IsoElementShape('tria6'),
@@ -31,14 +31,31 @@
     'tetra4': IsoElementShape('tetra4'),
     'hex8': IsoElementShape('hex8'),
     'hex20': IsoElementShape('hex20')
 }
 
 
 class Assembly:
+    __slots__: Tuple = ('total_dof_number',
+                        'props',
+                        'timer',
+                        'materials_dict',
+                        'sections_dict',
+                        'amplitudes_dict',
+                        'section_of_element_set',
+                        'element_data_list',
+                        'bc_data_list',
+                        'global_stiffness',
+                        'fext',
+                        'fint',
+                        'dof_solution',
+                        'ddof_solution',
+                        'bc_dof_ids',
+                        'field_variables')
+
     def __init__(self, props: Properties) -> None:
         self.total_dof_number: int = -1
         self.props: Properties = props
         self.timer: Timer = Timer()
         self.materials_dict: Dict = {}
         self.sections_dict: Dict = {}
         self.amplitudes_dict: Dict = {}
@@ -53,15 +70,15 @@
         self.bc_dof_ids = empty(0)
         self.field_variables: Dict[str, ndarray] = {}
         self.init()
         self.update_element_data()
         self.assembly_global_stiffness()
 
     def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string_assembly(self, level)
+        return object_slots_to_string_assembly(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
     @show_running_time
     def init(self) -> None:
         # 初始化 self.element_data_list
@@ -223,8 +240,13 @@
                         self.field_variables[field_name][assembly_conn] += \
                             element_data.element_average_field_variables[field_name]
                         nodes_count[assembly_conn] += 1.0
                     self.field_variables[field_name] = self.field_variables[field_name] / nodes_count
 
 
 if __name__ == "__main__":
-    pass
+    from pyfem.io.Properties import Properties
+
+    props = Properties()
+    props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
+    assembly = Assembly(props)
+    assembly.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/bc/BaseBC.py` & `pyfem-0.1.2/src/pyfem/bc/BaseBC.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,32 @@
 from pyfem.amplitude.BaseAmplitude import BaseAmplitude
 from pyfem.amplitude.get_amplitude_data import get_amplitude_data
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
 from pyfem.io.Solver import Solver
 from pyfem.mesh.MeshData import MeshData
-from pyfem.utils.visualization import object_dict_to_string_ndarray
+from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
 class BaseBC:
+    __slots__: Tuple = ('bc',
+                        'dof',
+                        'mesh_data',
+                        'solver',
+                        'amplitude',
+                        'amplitude_data',
+                        'get_amplitude',
+                        'bc_node_ids',
+                        'bc_element_ids',
+                        'dof_ids',
+                        'dof_values',
+                        'bc_fext',
+                        'bc_surface')
+
     def __init__(self, bc: BC, dof: Dof, mesh_data: MeshData, solver: Solver, amplitude: Optional[Amplitude]) -> None:
         self.bc: BC = bc
         self.dof: Dof = dof
         self.mesh_data: MeshData = mesh_data
         self.solver: Solver = solver
         self.amplitude: Optional[Amplitude] = amplitude
         if self.amplitude is not None:
@@ -33,15 +47,15 @@
         self.bc_element_ids: ndarray = empty(0)
         self.dof_ids: ndarray = empty(0)
         self.dof_values: ndarray = empty(0)
         self.bc_fext: ndarray = empty(0)
         self.bc_surface: List[Tuple[int, str]] = []
 
     def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string_ndarray(self, level)
+        return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `pyfem-0.1.1/src/pyfem/bc/DirichletBC.py` & `pyfem-0.1.2/src/pyfem/bc/DirichletBC.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,28 +9,23 @@
 from pyfem.bc.BaseBC import BaseBC
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
 from pyfem.io.Solver import Solver
 from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import error_style
-from pyfem.utils.visualization import object_dict_to_string_ndarray
 
 
 class DirichletBC(BaseBC):
+    __slots__ = BaseBC.__slots__ + ()
+
     def __init__(self, bc: BC, dof: Dof, mesh_data: MeshData, solver: Solver, amplitude: Optional[Amplitude]) -> None:
         super().__init__(bc, dof, mesh_data, solver, amplitude)
         self.create_dof_values()
 
-    def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string_ndarray(self, level)
-
-    def show(self) -> None:
-        print(self.to_string())
-
     def create_dof_values(self) -> None:
         bc_node_sets = self.bc.node_sets
         bc_node_ids = []
         for bc_node_set in bc_node_sets:
             bc_node_ids += list(self.mesh_data.node_sets[bc_node_set])
 
         # 如果发现施加当前边界条件的点集中有重复的点则抛出异常
@@ -55,13 +50,13 @@
             self.dof_values = array([bc_value for _ in self.dof_ids])
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
     props = Properties()
-    props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
+    props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
     props.verify()
 
     bc_data = DirichletBC(props.bcs[1], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
     bc_data.create_dof_values()
     bc_data.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/bc/NeumannBCConcentrated.py` & `pyfem-0.1.2/src/pyfem/bc/NeumannBCConcentrated.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     'tetra4': IsoElementShape('tetra4'),
     'hex8': IsoElementShape('hex8'),
     'hex20': IsoElementShape('hex20')
 }
 
 
 class NeumannBCConcentrated(BaseBC):
+    __slots__ = BaseBC.__slots__ + ()
+
     def __init__(self, bc: BC, dof: Dof, mesh_data: MeshData, solver: Solver, amplitude: Optional[Amplitude]) -> None:
         super().__init__(bc, dof, mesh_data, solver, amplitude)
         self.create_dof_values()
 
     def create_dof_values(self) -> None:
         bc_node_sets = self.bc.node_sets
         bc_node_ids = []
@@ -60,16 +62,11 @@
         if isinstance(bc_value, float):
             self.bc_fext = array([bc_value for _ in self.dof_ids])
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
-    # props = Properties()
-    # props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
-    # bc_data = NeumannBCPressure(props.bcs[3], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
-    # bc_data.show()
-
     props = Properties()
-    props.read_file(r'F:\Github\pyfem\examples\quad8\quad8.toml')
+    props.read_file(r'..\..\..\examples\mechanical\quad8\Job-1.toml')
     bc_data = NeumannBCConcentrated(props.bcs[2], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
     bc_data.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/bc/NeumannBCDistributed.py` & `pyfem-0.1.2/src/pyfem/bc/NeumannBCPressure.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     'quad8': IsoElementShape('quad8'),
     'tetra4': IsoElementShape('tetra4'),
     'hex8': IsoElementShape('hex8'),
     'hex20': IsoElementShape('hex20')
 }
 
 
-class NeumannBCDistributed(BaseBC):
+class NeumannBCPressure(BaseBC):
+    __slots__ = BaseBC.__slots__ + ()
+
     def __init__(self, bc: BC, dof: Dof, mesh_data: MeshData, solver: Solver, amplitude: Optional[Amplitude]) -> None:
         super().__init__(bc, dof, mesh_data, solver, amplitude)
         self.create_dof_values()
 
     def get_surface_from_bc_element(self, bc_element_id: int, bc_element: ndarray) -> List[Tuple[int, str]]:
         nodes = self.mesh_data.nodes
         elements = self.mesh_data.elements
@@ -136,51 +138,57 @@
             for node_index in surface_nodes:
                 for _, bc_dof_name in enumerate(bc_dof_names):
                     surface_dof_id = node_index * len(dof_names) + dof_names.index(bc_dof_name)
                     surface_dof_ids.append(surface_dof_id)
 
             dof_ids += surface_dof_ids
 
-            element_fext = zeros(nodes_number)
+            element_fext = zeros(nodes_number * len(self.bc.dof))
 
             for i in range(bc_gp_number):
                 bc_gp_jacobi = dot(bc_gp_shape_gradients[i], node_coords).transpose()
                 bc_gp_jacobi_sub = delete(bc_gp_jacobi, bc_surface_coord[0], axis=1)
                 if dimension == 2:
-                    s = sum(bc_gp_jacobi_sub ** 2)
-                    element_fext += bc_gp_shape_values[i].transpose() * bc_gp_weights[i] * bc_value * sqrt(s) * \
-                                    bc_surface_coord[2]
+                    pressure = -array([[0, bc_value], [-bc_value, 0]])
+                    pressure_times_jacobi = (dot(pressure, bc_gp_jacobi_sub)).transpose()
+                    element_fext += (dot(bc_gp_shape_values[i].transpose().reshape(4, -1), pressure_times_jacobi) *
+                                     bc_gp_weights[i] * bc_surface_coord[2]).reshape(-1)
+
                 elif dimension == 3:
                     s = 0
                     for row in range(bc_gp_jacobi_sub.shape[0]):
                         s += det(delete(bc_gp_jacobi_sub, row, axis=0)) ** 2
                     element_fext += bc_gp_shape_values[i].transpose() * bc_gp_weights[i] * bc_value * sqrt(s) * \
                                     bc_surface_coord[2]
 
+            print(element_fext)
+
             surface_fext = []
             for fext in element_fext[surface_local_nodes]:
                 for _ in range(len(bc_dof_names)):
                     surface_fext.append(fext)
 
             bc_fext += list(surface_fext)
 
         self.dof_ids = array(dof_ids)
         self.bc_fext = array(bc_fext)
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
-    # props = Properties()
-    # props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
-    # bc_data = NeumannBCDistributed(props.bcs[3], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
-    # bc_data.show()
+    props = Properties()
+    props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
+    bc_data = NeumannBCPressure(props.bcs[3], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
+    bc_data.show()
+
+    print(props.mesh_data.bc_element_sets)
 
     # props = Properties()
     # props.read_file(r'F:\Github\pyfem\examples\hex\hex.toml')
     # bc_data = NeumannBCDistributed(props.bcs[4], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
     # bc_data.show()
 
-    props = Properties()
-    props.read_file(r'F:\Github\pyfem\examples\quad8\quad8.toml')
-    bc_data = NeumannBCDistributed(props.bcs[2], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
-    bc_data.show()
+    # props = Properties()
+    # props.read_file(r'F:\Github\pyfem\examples\quad8\quad8.toml')
+    # bc_data = NeumannBCDistributed(props.bcs[2], props.dof, props.mesh_data, props.solver, props.amplitudes[0])
+    # bc_data.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/bc/get_bc_data.py` & `pyfem-0.1.2/src/pyfem/bc/get_bc_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 """
 
 """
 from typing import Optional
 
 from pyfem.bc.BaseBC import BaseBC
 from pyfem.bc.DirichletBC import DirichletBC
-from pyfem.bc.NeumannBC import NeumannBC
 from pyfem.bc.NeumannBCConcentrated import NeumannBCConcentrated
 from pyfem.bc.NeumannBCDistributed import NeumannBCDistributed
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
 from pyfem.io.Solver import Solver
 from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import error_style
 
 bc_data_dict = {
     'DirichletBC': DirichletBC,
-    'NeumannBC': NeumannBC,
     'NeumannBCConcentrated': NeumannBCConcentrated,
     'NeumannBCDistributed': NeumannBCDistributed
 }
 
 
 def get_bc_data(bc: BC,
                 dof: Dof,
```

### Comparing `pyfem-0.1.1/src/pyfem/elements/IsoElementDiagram.py` & `pyfem-0.1.2/src/pyfem/elements/IsoElementDiagram.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,20 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
+
+
 class IsoElementDiagram:
     """
     等参元的形状示意图
     """
 
+    __slots__ = ()
+
     line2 = r"""
     0---------------1
             +-->x0"""
 
     line3 = r"""
     0-------1-------2
             +-->x0"""
@@ -52,28 +60,28 @@
     |       x1      |
     |       |       |
     7       9--x0   5
     |               |
     |               |
     0-------4-------1"""
 
-    # tetra4 = r"""
-    # 3
-    # * * *
-    # *   *   *
-    # *     *     *
-    # *       *       2
-    # *         *    * *
-    # *           **    *
-    # *          *  *    *
-    # *        *      *   *
-    # *      *          *  *
-    # x2   x1             * *
-    # |  *                  **
-    # 0--x0 * * * * * * * * * 1"""
+    tetra4_zoom = r"""
+    3
+    * * *
+    *   *   *
+    *     *     *
+    *       *       2
+    *         *    * *
+    *           **    *
+    *          *  *    *
+    *        *      *   *
+    *      *          *  *
+    x2   x1             * *
+    |  *                  **
+    0--x0 * * * * * * * * * 1"""
 
     tetra4 = r"""
     3
     * **
     *   * *
     *     *  *
     *       *   2
@@ -92,24 +100,24 @@
     |   3-----------+---2
     |  /            |  /
     | /             | /
     |/              |/
     0---------------1"""
 
     hex20 = r"""
-            7-------14------6
-           /|              /|
-         15 |     x2 x1  13 |
-         /  19    | /    /  18
-        4---+---12|/----5   |
-        |   |     +--x0 |   |
-        |   3-------10--+---2
-        16 /            17 /
-        |11             | 9
-        |/              |/
-        0-------8-------1"""
+        7-------14------6
+       /|              /|
+     15 |     x2 x1  13 |
+     /  19    | /    /  18
+    4---+---12|/----5   |
+    |   |     +--x0 |   |
+    |   3-------10--+---2
+    16 /            17 /
+    |11             | 9
+    |/              |/
+    0-------8-------1"""
 
 
 if __name__ == "__main__":
     print(IsoElementDiagram.quad4)
     print(IsoElementDiagram.tetra4)
     print(IsoElementDiagram.hex8)
```

### Comparing `pyfem-0.1.1/src/pyfem/elements/IsoElementShape.py` & `pyfem-0.1.2/src/pyfem/elements/IsoElementShape.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,120 @@
-from typing import Tuple, Callable, Dict
+from typing import Callable, Dict, Tuple
 
-from numpy import (empty, meshgrid, outer, column_stack, array, ndarray, insert, in1d)
+from numpy import empty, meshgrid, outer, column_stack, array, ndarray, insert, in1d
 from numpy.polynomial.legendre import leggauss
 
 from pyfem.elements.IsoElementDiagram import IsoElementDiagram
 from pyfem.fem.constants import DTYPE
 from pyfem.utils.colors import error_style
-from pyfem.utils.visualization import object_dict_to_string_ndarray
+from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
 class IsoElementShape:
     """
     等参单元类，设置等参单元的形函数和积分点等信息
+
+    当前支持的单元类型 ['empty', 'line2', 'line3', 'tria3', 'tria6', 'quad4', 'quad8', 'tetra4', 'hex8', 'hex20']
+
+    :ivar element_type: 等参单元类型
+    :vartype element_type: str
+
+    :ivar diagram: 等参单元示意图（字符串形式）
+    :vartype diagram: str
+
+    :ivar dimension: 等参单元空间维度
+    :vartype dimension: int
+
+    :ivar nodes_number: 等参单元节点数目
+    :vartype nodes_number: int
+
+    :ivar order: 等参单元插值阶次
+    :vartype order: int
+
+    :ivar shape_function: 等参单元形函数
+    :vartype shape_function: Callable
+
+    :ivar gp_number: 等参单元积分点数量
+    :vartype gp_number: int
+
+    :ivar gp_coords: 等参单元积分点坐标
+    :vartype gp_coords: ndarray
+
+    :ivar gp_weights: 等参单元积分点权重
+    :vartype gp_weights: ndarray
+
+    :ivar gp_shape_values: 等参单元积分点处形函数的值
+    :vartype gp_shape_values: ndarray
+
+    :ivar gp_shape_gradients: 等参单元积分点处形函数对局部坐标梯度的值
+    :vartype gp_shape_gradients: ndarray
+
+    :ivar bc_surface_number: 等参单元边界面数量
+    :vartype bc_surface_number: int
+
+    :ivar bc_surface_nodes_dict: 等参单元边界面节点编号
+    :vartype bc_surface_nodes_dict: Dict[str, Tuple]
+
+    :ivar bc_surface_coord_dict: 等参单元边界面节点坐标
+    :vartype bc_surface_coord_dict: Dict[str, Tuple]
+
+    :ivar bc_gp_coords_dict: 等参单元边界面积分点坐标
+    :vartype bc_gp_coords_dict: Dict[str, ndarray]
+
+    :ivar bc_gp_weights: 等参单元边界面积分点权重
+    :vartype bc_gp_weights: ndarray
+
+    :ivar bc_gp_shape_values_dict: 等参单元边界面积分点处形函数的值
+    :vartype bc_gp_shape_values_dict: Dict[str, ndarray]
+
+    :ivar bc_gp_shape_gradients_dict: 等参单元边界面积分点处形函数对局部坐标梯度的值
+    :vartype bc_gp_shape_gradients_dict: Dict[str, ndarray]
+
+    :ivar nodes_to_surface_dict: 单元节点与等参单元边界面的映射字典
+    :vartype nodes_to_surface_dict: Dict[str, ndarray]
     """
+
+    __slots_dir__ = {
+        'element_type': ('str', '等参单元类型'),
+        'diagram': ('str', '等参单元示意图（字符串形式）'),
+        'dimension': ('int', '等参单元空间维度'),
+        'nodes_number': ('int', '等参单元节点数目'),
+        'order': ('int', '等参单元插值阶次'),
+        'shape_function': ('Callable', '等参单元形函数'),
+        'gp_number': ('int', '等参单元积分点数量'),
+        'gp_coords': ('ndarray', '等参单元积分点坐标'),
+        'gp_weights': ('ndarray', '等参单元积分点权重'),
+        'gp_shape_values': ('ndarray', '等参单元积分点处形函数的值'),
+        'gp_shape_gradients': ('ndarray', '等参单元积分点处形函数对局部坐标梯度的值'),
+        'bc_surface_number': ('int', '等参单元边界面数量'),
+        'bc_surface_nodes_dict': ('Dict[str, Tuple]', '等参单元边界面节点编号'),
+        'bc_surface_coord_dict': ('Dict[str, Tuple]', '等参单元边界面节点坐标'),
+        'bc_gp_coords_dict': ('Dict[str, ndarray]', '等参单元边界面积分点坐标'),
+        'bc_gp_weights': ('ndarray', '等参单元边界面积分点权重'),
+        'bc_gp_shape_values_dict': ('Dict[str, ndarray]', '等参单元边界面积分点处形函数的值'),
+        'bc_gp_shape_gradients_dict': ('Dict[str, ndarray]', '等参单元边界面积分点处形函数对局部坐标梯度的值'),
+        'nodes_to_surface_dict': ('Dict[str, ndarray]', '单元节点与等参单元边界面的映射字典')
+    }
+
+    # for key, item in __slots_dir__.items():
+    #     print(f'    :ivar {key}: {item[1]}')
+    #     print(f'    :vartype {key}: {item[0]}\n')
+
+    __slots__ = (slot for slot in __slots_dir__.keys())
+
     allowed_element_type = ['empty', 'line2', 'line3', 'tria3', 'tria6', 'quad4', 'quad8', 'tetra4', 'hex8', 'hex20']
 
     def __init__(self, element_type: str) -> None:
-        """
-        当前支持的单元类型 ['empty', 'line2', 'line3', 'tria3', 'tria6', 'quad4', 'quad8', 'tetra4', 'hex8', 'hex20']
-        """
         self.element_type: str = ''
         self.diagram: str = ''
         self.dimension: int = 0
         self.nodes_number: int = 0
         self.order: int = 0
         self.shape_function: Callable = get_shape_empty
-        self.gp_number = 0
+        self.gp_number: int = 0
         self.gp_coords: ndarray = empty(0)
         self.gp_weights: ndarray = empty(0)
         self.gp_shape_values: ndarray = empty(0)
         self.gp_shape_gradients: ndarray = empty(0)
         self.bc_surface_number: int = 0
         self.bc_surface_nodes_dict: Dict[str, Tuple] = {}
         self.bc_surface_coord_dict: Dict[str, Tuple] = {}
@@ -69,15 +154,15 @@
             self.element_type = element_type
             self.set_hex20()
         else:
             error_msg = f'Unsupported element type {element_type}'
             raise NotImplementedError(error_style(error_msg))
 
     def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string_ndarray(self, level)
+        return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
     def set_line2(self) -> None:
         self.dimension = 1
         self.nodes_number = 2
@@ -128,18 +213,18 @@
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
         self.bc_surface_number = 4
         self.bc_surface_nodes_dict = {'s1': (3, 0),
                                       's2': (1, 2),
                                       's3': (0, 1),
                                       's4': (2, 3)}
-        self.bc_surface_coord_dict = {'s1': (0, -1, 1),
-                                      's2': (0, 1, 1),
-                                      's3': (1, -1, 1),
-                                      's4': (1, 1, 1)}
+        self.bc_surface_coord_dict = {'s1': (0, -1, -1, 1),
+                                      's2': (0, 1, 1, 1),
+                                      's3': (1, -1, 1, 1),
+                                      's4': (1, 1, -1, 1)}
         for surface_name, surface_conn in self.bc_surface_nodes_dict.items():
             self.nodes_to_surface_dict[surface_name] = in1d(range(self.nodes_number), surface_conn)
         bc_gp_coords, self.bc_gp_weights = get_gauss_points(dimension=self.dimension - 1, order=self.order)
         self.bc_gp_coords_dict = {'s1': insert(bc_gp_coords, 0, -1, axis=1),
                                   's2': insert(bc_gp_coords, 0, 1, axis=1),
                                   's3': insert(bc_gp_coords, 1, -1, axis=1),
                                   's4': insert(bc_gp_coords, 1, 1, axis=1)}
@@ -172,18 +257,18 @@
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
         self.bc_surface_number = 4
         self.bc_surface_nodes_dict = {'s1': (3, 0, 7),
                                       's2': (1, 2, 5),
                                       's3': (0, 1, 4),
                                       's4': (2, 3, 6)}
-        self.bc_surface_coord_dict = {'s1': (0, -1, 1),
-                                      's2': (0, 1, 1),
-                                      's3': (1, -1, 1),
-                                      's4': (1, 1, 1)}
+        self.bc_surface_coord_dict = {'s1': (0, -1, -1, 1),
+                                      's2': (0, 1, 1, 1),
+                                      's3': (1, -1, 1, 1),
+                                      's4': (1, 1, -1, 1)}
         for surface_name, surface_conn in self.bc_surface_nodes_dict.items():
             self.nodes_to_surface_dict[surface_name] = in1d(range(self.nodes_number), surface_conn)
         bc_gp_coords, self.bc_gp_weights = get_gauss_points(dimension=self.dimension - 1, order=self.order)
         self.bc_gp_coords_dict = {'s1': insert(bc_gp_coords, 0, -1, axis=1),
                                   's2': insert(bc_gp_coords, 0, 1, axis=1),
                                   's3': insert(bc_gp_coords, 1, -1, axis=1),
                                   's4': insert(bc_gp_coords, 1, 1, axis=1)}
@@ -269,20 +354,20 @@
         self.bc_surface_number = 6
         self.bc_surface_nodes_dict = {'s1': (0, 3, 7, 4),
                                       's2': (1, 2, 6, 5),
                                       's3': (0, 1, 5, 4),
                                       's4': (2, 3, 6, 7),
                                       's5': (0, 1, 2, 3),
                                       's6': (4, 5, 6, 7)}
-        self.bc_surface_coord_dict = {'s1': (0, -1, 1),
-                                      's2': (0, 1, 1),
-                                      's3': (1, -1, 1),
-                                      's4': (1, 1, 1),
-                                      's5': (2, -1, 1),
-                                      's6': (2, 1, 1)}
+        self.bc_surface_coord_dict = {'s1': (0, -1, 1, 1),
+                                      's2': (0, 1, 1, 1),
+                                      's3': (1, -1, 1, 1),
+                                      's4': (1, 1, 1, 1),
+                                      's5': (2, -1, 1, 1),
+                                      's6': (2, 1, 1, 1)}
         for surface_name, surface_conn in self.bc_surface_nodes_dict.items():
             self.nodes_to_surface_dict[surface_name] = in1d(range(self.nodes_number), surface_conn)
         bc_gp_coords, self.bc_gp_weights = get_gauss_points(dimension=self.dimension - 1, order=self.order)
         self.bc_gp_coords_dict = {'s1': insert(bc_gp_coords, 0, -1, axis=1),
                                   's2': insert(bc_gp_coords, 0, 1, axis=1),
                                   's3': insert(bc_gp_coords, 1, -1, axis=1),
                                   's4': insert(bc_gp_coords, 1, 1, axis=1),
@@ -900,10 +985,8 @@
     # iso_element_shape = IsoElementShape('empty')
 
     # print(iso_element_shape.bc_gp_coords_dict['s1'])
     # print(iso_element_shape.bc_gp_weights)
     # print(iso_element_shape.bc_gp_shape_values_dict['s1'])
     # print(iso_element_shape.bc_gp_shape_gradients_dict['s1'])
 
-    iso_element_shape.show()
-
-    # print(iso_element_shape.gp_weights.dtype)
+    # iso_element_shape.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/elements/SolidPlaneSmallStrain.py` & `pyfem-0.1.2/src/pyfem/elements/SolidPlaneSmallStrain.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 from pyfem.elements.BaseElement import BaseElement
 from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
-from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
+from pyfem.utils.data_types import MaterialData
 
 
 class SolidPlaneSmallStrain(BaseElement):
     __slots__ = BaseElement.__slots__ + ('gp_b_matrices', 'gp_b_matrices_transpose', 'gp_strains', 'gp_stresses')
 
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
                  materials: List[Material],
                  section: Section,
-                 material_data_list: List[BaseMaterial],
+                 material_data_list: List[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = ('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell')
+        self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell')]
         self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
@@ -204,10 +204,10 @@
         self.element_average_field_variables['S22'] = average_stress[1]
         self.element_average_field_variables['S12'] = average_stress[2]
 
 
 if __name__ == "__main__":
     from pyfem.Job import Job
 
-    job = Job(r'F:\Github\pyfem\examples\1element\hex8\Job-1.toml')
+    job = Job(r'..\..\..\examples\mechanical\1element\hex8\Job-1.toml')
 
     job.assembly.element_data_list[0].show()
```

### Comparing `pyfem-0.1.1/src/pyfem/elements/SolidThermalPlaneSmallStrain.py` & `pyfem-0.1.2/src/pyfem/elements/SolidVolumeSmallStrain.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from typing import List
 
-from numpy import array, zeros, dot, ndarray, average, ix_
+from numpy import array, zeros, dot, ndarray, average
 
 from pyfem.elements.BaseElement import BaseElement
 from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
-from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
+from pyfem.utils.data_types import MaterialData
 
 
-class SolidThermalPlaneSmallStrain(BaseElement):
-    __slots__ = BaseElement.__slots__ + ('gp_b_matrices', 'gp_b_matrices_transpose', 'gp_strains', 'gp_stresses',
-                                         'gp_temperatures', 'gp_heat_fluxes', 'dof_u', 'dof_T')
+class SolidVolumeSmallStrain(BaseElement):
+    __slots__ = BaseElement.__slots__ + ('gp_b_matrices', 'gp_b_matrices_transpose', 'gp_strains', 'gp_stresses')
 
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
                  materials: List[Material],
                  section: Section,
-                 material_data_list: List[BaseMaterial],
+                 material_data_list: List[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = ('ElasticIsotropic', 'PlasticKinematicHardening',
-                                           'ViscoElasticMaxwell', 'ThermalIsotropic')
-        self.allowed_material_number = 2
+        self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell')]
+        self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
         self.timer = timer
 
-        self.dof_names = ['u1', 'u2', 'T']
+        self.dof_names = ['u1', 'u2', 'u3']
         if dof.names != self.dof_names:
             error_msg = f'{dof.names} is not the supported dof of {type(self).__name__} element'
             raise NotImplementedError(error_style(error_msg))
 
         element_dof_number = len(self.dof_names) * self.iso_element_shape.nodes_number
         self.element_dof_number = element_dof_number
         self.element_dof_values = zeros(element_dof_number, dtype=DTYPE)
@@ -57,33 +55,32 @@
         self.element_stiffness = None  # type: ignore
 
         self.gp_b_matrices: ndarray = None  # type: ignore
         self.gp_b_matrices_transpose: ndarray = None  # type: ignore
         self.gp_strains: List[ndarray] = []
         self.gp_stresses: List[ndarray] = []
 
-        self.dof_u = []
-        self.dof_T = []
-        for i in range(self.iso_element_shape.nodes_number):
-            self.dof_u += [len(self.dof_names) * i + 0, len(self.dof_names) * i + 1]
-            self.dof_T += [len(self.dof_names) * i + 2]
-
         self.create_gp_b_matrices()
 
     def create_gp_b_matrices(self) -> None:
-        self.gp_b_matrices = zeros(shape=(self.gp_number, 3, len(self.dof_u)), dtype=DTYPE)
+        self.gp_b_matrices = zeros(shape=(self.iso_element_shape.gp_number, 6, self.element_dof_number))
 
         for igp, (gp_shape_gradient, gp_jacobi_inv) in \
                 enumerate(zip(self.iso_element_shape.gp_shape_gradients, self.gp_jacobi_invs)):
             gp_dhdx = dot(gp_shape_gradient.transpose(), gp_jacobi_inv)
             for i, val in enumerate(gp_dhdx):
-                self.gp_b_matrices[igp, 0, i * 2] = val[0]
-                self.gp_b_matrices[igp, 1, i * 2 + 1] = val[1]
-                self.gp_b_matrices[igp, 2, i * 2] = val[1]
-                self.gp_b_matrices[igp, 2, i * 2 + 1] = val[0]
+                self.gp_b_matrices[igp, 0, i * 3] = val[0]
+                self.gp_b_matrices[igp, 1, i * 3 + 1] = val[1]
+                self.gp_b_matrices[igp, 2, i * 3 + 2] = val[2]
+                self.gp_b_matrices[igp, 3, i * 3] = val[1]
+                self.gp_b_matrices[igp, 3, i * 3 + 1] = val[0]
+                self.gp_b_matrices[igp, 4, i * 3] = val[2]
+                self.gp_b_matrices[igp, 4, i * 3 + 2] = val[0]
+                self.gp_b_matrices[igp, 5, i * 3 + 1] = val[2]
+                self.gp_b_matrices[igp, 5, i * 3 + 2] = val[1]
 
         self.gp_b_matrices_transpose = array([gp_b_matrix.transpose() for gp_b_matrix in self.gp_b_matrices])
 
     def update_material_state(self) -> None:
         gp_number = self.iso_element_shape.gp_number
         gp_b_matrices = self.gp_b_matrices
         gp_state_variables = self.gp_state_variables
@@ -102,17 +99,17 @@
             gp_dstrain = dot(gp_b_matrices[i], element_ddof_values)
             variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
             gp_ddsdde, gp_output = self.material_data_list[0].get_tangent(variable=variable,
                                                                           state_variable=gp_state_variables[i],
                                                                           state_variable_new=gp_state_variables_new[i],
                                                                           element_id=element_id,
                                                                           igp=i,
-                                                                          ntens=4,
+                                                                          ntens=6,
                                                                           ndi=3,
-                                                                          nshr=1,
+                                                                          nshr=3,
                                                                           timer=timer)
             gp_stress = gp_output['stress']
             gp_ddsddes.append(gp_ddsdde)
             gp_strains.append(gp_strain)
             gp_stresses.append(gp_stress)
 
         self.gp_ddsddes = gp_ddsddes
@@ -123,114 +120,58 @@
         element_id = self.element_id
         timer = self.timer
 
         gp_number = self.gp_number
         gp_b_matrices = self.gp_b_matrices
         gp_b_matrices_transpose = self.gp_b_matrices_transpose
         gp_weight_times_jacobi_dets = self.gp_weight_times_jacobi_dets
-        gp_shape_values = self.iso_element_shape.gp_shape_values
-        gp_shape_gradients = self.iso_element_shape.gp_shape_gradients
 
         gp_state_variables = self.gp_state_variables
         gp_state_variables_new = self.gp_state_variables_new
 
         element_dof_values = self.element_dof_values
         element_ddof_values = self.element_ddof_values
 
-        u = element_dof_values[self.dof_u]
-        T = element_dof_values[self.dof_T]
-
-        du = element_ddof_values[self.dof_u]
-        dT = element_ddof_values[self.dof_T]
-
         self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
         self.element_fint = zeros(self.element_dof_number, dtype=DTYPE)
 
-        for material_data in self.material_data_list:
-            if 'Thermal' not in type(material_data).__name__:
-                gp_ddsddes = []
-                gp_strains = []
-                gp_stresses = []
-
-                for i in range(gp_number):
-                    gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
-                    gp_b_matrix_transpose = gp_b_matrices_transpose[i]
-                    gp_b_matrix = gp_b_matrices[i]
-                    gp_strain = dot(gp_b_matrix, u)
-                    gp_dstrain = dot(gp_b_matrix, du)
-                    variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
-                    gp_ddsdde, gp_output = material_data.get_tangent(variable=variable,
-                                                                     state_variable=gp_state_variables[i],
-                                                                     state_variable_new=gp_state_variables_new[i],
-                                                                     element_id=element_id,
-                                                                     igp=i,
-                                                                     ntens=4,
-                                                                     ndi=3,
-                                                                     nshr=1,
-                                                                     timer=timer)
-                    gp_stress = gp_output['stress']
-
-                    self.element_stiffness[ix_(self.dof_u, self.dof_u)] += dot(gp_b_matrix_transpose,
-                                                                               dot(gp_ddsdde,
-                                                                                   gp_b_matrix)) * gp_weight_times_jacobi_det
-
-                    self.element_fint[self.dof_u] += dot(gp_b_matrix_transpose, gp_stress) * gp_weight_times_jacobi_det
-
-                    gp_ddsddes.append(gp_ddsdde)
-                    gp_strains.append(gp_strain)
-                    gp_stresses.append(gp_stress)
-
-                self.gp_ddsddes = gp_ddsddes
-                self.gp_strains = gp_strains
-                self.gp_stresses = gp_stresses
-
-            else:
-                gp_ddsddes = []
-                gp_temperatures = []
-                gp_heat_fluxes = []
-
-                for i in range(gp_number):
-                    gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
-                    gp_shape_value = gp_shape_values[i]
-                    gp_shape_gradient = gp_shape_gradients[i]
-                    gp_temperature = dot(gp_shape_value, T)
-                    gp_dtemperature = dot(gp_shape_value, dT)
-                    gp_temperature_gradient = dot(gp_shape_gradient, T)
-                    gp_dtemperature_gradient = dot(gp_shape_gradient, dT)
-
-                    variable = {'temperature': gp_temperature,
-                                'dtemperature': gp_dtemperature,
-                                'temperature_gradient': gp_temperature_gradient,
-                                'dtemperature_gradient': gp_dtemperature_gradient}
-                    gp_ddsdde, gp_output = material_data.get_tangent(variable=variable,
-                                                                     state_variable=gp_state_variables[i],
-                                                                     state_variable_new=
-                                                                     gp_state_variables_new[i],
-                                                                     element_id=element_id,
-                                                                     igp=i,
-                                                                     ntens=4,
-                                                                     ndi=3,
-                                                                     nshr=1,
-                                                                     timer=timer)
-                    gp_heat_flux = gp_output['heat_flux']
-
-                    self.element_stiffness[ix_(self.dof_T, self.dof_T)] += dot(gp_shape_gradient.transpose(),
-                                                                               dot(gp_ddsdde, gp_shape_gradient)) * \
-                                                                           gp_weight_times_jacobi_det
-
-                    self.element_fint[self.dof_T] += dot(gp_shape_gradient.transpose(),
-                                                         gp_heat_flux) * gp_weight_times_jacobi_det
-
-                    gp_ddsddes.append(gp_ddsdde)
-                    gp_temperatures.append(gp_temperature)
-                    gp_heat_fluxes.append(gp_heat_flux)
-
-                self.gp_ddsddes = gp_ddsddes
-                self.gp_temperatures = gp_temperatures
-                self.gp_heat_fluxes = gp_heat_fluxes
+        gp_ddsddes = []
+        gp_strains = []
+        gp_stresses = []
+
+        for i in range(gp_number):
+            gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
+            gp_b_matrix_transpose = gp_b_matrices_transpose[i]
+            gp_b_matrix = gp_b_matrices[i]
+            gp_strain = dot(gp_b_matrix, element_dof_values)
+            gp_dstrain = dot(gp_b_matrix, element_ddof_values)
+            variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
+            gp_ddsdde, gp_output = self.material_data_list[0].get_tangent(variable=variable,
+                                                                          state_variable=gp_state_variables[i],
+                                                                          state_variable_new=gp_state_variables_new[i],
+                                                                          element_id=element_id,
+                                                                          igp=i,
+                                                                          ntens=6,
+                                                                          ndi=3,
+                                                                          nshr=3,
+                                                                          timer=timer)
+            gp_stress = gp_output['stress']
+
+            self.element_stiffness += dot(gp_b_matrix_transpose, dot(gp_ddsdde, gp_b_matrix)) * \
+                                      gp_weight_times_jacobi_det
+
+            self.element_fint += dot(gp_b_matrix_transpose, gp_stress) * gp_weight_times_jacobi_det
+
+            gp_ddsddes.append(gp_ddsdde)
+            gp_strains.append(gp_strain)
+            gp_stresses.append(gp_stress)
+
+        self.gp_ddsddes = gp_ddsddes
+        self.gp_strains = gp_strains
+        self.gp_stresses = gp_stresses
 
     def update_element_stiffness(self) -> None:
         self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
 
         gp_weight_times_jacobi_dets = self.gp_weight_times_jacobi_dets
         gp_b_matrices = self.gp_b_matrices
         gp_b_matrices_transpose = self.gp_b_matrices_transpose
@@ -259,18 +200,24 @@
         average_stress = average(gp_stresses, axis=0)
 
         self.gp_field_variables['strain'] = array(gp_strains, dtype=DTYPE)
         self.gp_field_variables['stress'] = array(gp_stresses, dtype=DTYPE)
 
         self.element_average_field_variables['E11'] = average_strain[0]
         self.element_average_field_variables['E22'] = average_strain[1]
-        self.element_average_field_variables['E12'] = average_strain[2]
+        self.element_average_field_variables['E33'] = average_strain[2]
+        self.element_average_field_variables['E12'] = average_strain[3]
+        self.element_average_field_variables['E13'] = average_strain[4]
+        self.element_average_field_variables['E23'] = average_strain[5]
         self.element_average_field_variables['S11'] = average_stress[0]
         self.element_average_field_variables['S22'] = average_stress[1]
-        self.element_average_field_variables['S12'] = average_stress[2]
+        self.element_average_field_variables['S33'] = average_stress[2]
+        self.element_average_field_variables['S12'] = average_stress[3]
+        self.element_average_field_variables['S13'] = average_stress[4]
+        self.element_average_field_variables['S23'] = average_stress[5]
 
 
 if __name__ == "__main__":
     from pyfem.Job import Job
 
     job = Job(r'F:\Github\pyfem\examples\1element\hex8\Job-1.toml')
```

### Comparing `pyfem-0.1.1/src/pyfem/elements/ThermalStatic.py` & `pyfem-0.1.2/src/pyfem/elements/Thermal.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 from pyfem.elements.BaseElement import BaseElement
 from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
-from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
+from pyfem.utils.data_types import MaterialData
 
 
-class ThermalStatic(BaseElement):
+class Thermal(BaseElement):
     __slots__ = BaseElement.__slots__ + ('gp_temperatures', 'gp_heat_fluxes')
 
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
                  materials: List[Material],
                  section: Section,
-                 material_data_list: List[BaseMaterial],
+                 material_data_list: List[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = ('ThermalIsotropic',)
+        self.allowed_material_data_list = [('ThermalIsotropic',)]
         self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
```

### Comparing `pyfem-0.1.1/src/pyfem/elements/get_element_data.py` & `pyfem-0.1.2/src/pyfem/elements/get_element_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,43 +4,46 @@
 """
 from typing import List
 
 from numpy import ndarray
 
 from pyfem.elements.BaseElement import BaseElement
 from pyfem.elements.IsoElementShape import IsoElementShape
+from pyfem.elements.SolidPhaseFieldDamagePlaneSmallStrain import SolidPhaseFieldDamagePlaneSmallStrain
 from pyfem.elements.SolidPlaneSmallStrain import SolidPlaneSmallStrain
-from pyfem.elements.SolidVolumeSmallStrain import SolidVolumeSmallStrain
-from pyfem.elements.ThermalStatic import ThermalStatic
 from pyfem.elements.SolidThermalPlaneSmallStrain import SolidThermalPlaneSmallStrain
+from pyfem.elements.SolidVolumeSmallStrain import SolidVolumeSmallStrain
+from pyfem.elements.Thermal import Thermal
 from pyfem.fem.Timer import Timer
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
-from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
+from pyfem.utils.data_types import MaterialData
 
 element_data_dict = {
-    'SolidPlaneStressSmallStrain': SolidPlaneSmallStrain,
     'SolidPlaneStrainSmallStrain': SolidPlaneSmallStrain,
+    'SolidPlaneStressSmallStrain': SolidPlaneSmallStrain,
     'SolidVolumeSmallStrain': SolidVolumeSmallStrain,
     'SolidThermalPlaneStrainSmallStrain': SolidThermalPlaneSmallStrain,
-    'ThermalStatic': ThermalStatic
+    'SolidThermalPlaneStressSmallStrain': SolidThermalPlaneSmallStrain,
+    'SolidPhaseFieldDamagePlaneStrainSmallStrain': SolidPhaseFieldDamagePlaneSmallStrain,
+    'SolidPhaseFieldDamagePlaneStressSmallStrain': SolidPhaseFieldDamagePlaneSmallStrain,
+    'Thermal': Thermal,
 }
 
 
-# @trace_calls
 def get_element_data(element_id: int,
                      iso_element_shape: IsoElementShape,
                      connectivity: ndarray,
                      node_coords: ndarray,
                      dof: Dof,
                      materials: List[Material],
                      section: Section,
-                     material_data_list: List[BaseMaterial],
+                     material_data_list: List[MaterialData],
                      timer: Timer) -> BaseElement:
     class_name = f'{section.category}{section.type}{section.option}'.strip().replace(' ', '')
 
     if class_name in element_data_dict:
         return element_data_dict[class_name](element_id=element_id,
                                              iso_element_shape=iso_element_shape,
                                              connectivity=connectivity,
```

### Comparing `pyfem-0.1.1/src/pyfem/elements/get_iso_element_type.py` & `pyfem-0.1.2/src/pyfem/elements/get_iso_element_type.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.1/src/pyfem/fem/Timer.py` & `pyfem-0.1.2/src/pyfem/fem/Timer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import List
+from typing import List, Tuple
 
-from pyfem.utils.visualization import object_dict_to_string
+from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
 class Timer:
     """
     计时器类，用于存储求解过程中的时间信息。
     """
-    TOL_TIME = 1e-6
+    __slots__: Tuple = ('total_time',
+                        'time0',
+                        'time1',
+                        'dtime',
+                        'increment',
+                        'frame_ids')
+
+    TOL_TIME: float = 1e-6
 
     def __init__(self) -> None:
         self.total_time: float = 1.0
         self.time0: float = 0.0
         self.time1: float = 0.0
         self.dtime: float = 1.0
         self.increment: int = 0
         self.frame_ids: List[int] = []
 
     def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string(self, level)
+        return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
     def is_done(self) -> bool:
         if self.time1 * (1.0 + self.TOL_TIME) >= self.total_time:
             return True
```

### Comparing `pyfem-0.1.1/src/pyfem/io/BC.py` & `pyfem-0.1.2/src/pyfem/io/BC.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import List
+from typing import List, Tuple
 
-from pyfem.utils.visualization import object_dict_to_string
+from pyfem.io.BaseIO import BaseIO
 
 
-class BC:
+class BC(BaseIO):
+    __slots__: Tuple = ('name',
+                        'category',
+                        'type',
+                        'dof',
+                        'node_sets',
+                        'element_sets',
+                        'bc_element_sets',
+                        'value',
+                        'amplitude_name')
+
     def __init__(self) -> None:
+        super().__init__()
         self.name: str = None  # type: ignore
         self.category: str = None  # type: ignore
         self.type: str = None  # type: ignore
         self.dof: List[str] = None  # type: ignore
         self.node_sets: List[str] = None  # type: ignore
         self.element_sets: List[str] = None  # type: ignore
         self.bc_element_sets: List[str] = None  # type: ignore
         self.value: float = None  # type: ignore
         self.amplitude_name: str = None  # type: ignore
 
-    def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string(self, level)
-
-    def show(self) -> None:
-        print(self.to_string())
-
 
 if __name__ == "__main__":
     bc = BC()
     bc.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/io/Material.py` & `pyfem-0.1.2/src/pyfem/materials/MechanicalThermalExpansion.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import List, Tuple, Dict
+from typing import Tuple, Dict
 
+from numpy import ones, ndarray
+
+from pyfem.fem.Timer import Timer
+from pyfem.io.Material import Material
+from pyfem.io.Section import Section
+from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
-from pyfem.utils.visualization import object_dict_to_string
 
 
-class Material:
-    """
-    Material类用于存储配置文件中定义的材料属性。
-
-    当 self.is_read_only = True 时：
-        1. Material 类的所有属性在首次被赋非None值后不能再被修改和删除，
-        2. 此时许可的属性关键字存储在self.slots中。
-    """
-    is_read_only: bool = True
-    slots: Tuple = ('name', 'category', 'type', 'data')
-    allowed_keys_values: Dict = {
-        'category': [None, 'Elastic', 'Plastic', 'ViscoElastic', 'Thermal'],
-        'type': [None, 'Isotropic', 'IsotropicHardening', 'KinematicHardening', 'Maxwell']
-    }
-
-    def __init__(self) -> None:
-        self.name: str = None  # type: ignore
-        self.category: str = None  # type: ignore
-        self.type: str = None  # type: ignore
-        self.data: List[float] = None  # type: ignore
-
-    def __setattr__(self, key, value) -> None:
-        if self.is_read_only:
-            if key not in self.slots:
-                error_msg = f'{key} is not an allowable attribute keyword of {type(self).__name__}'
-                raise AttributeError(error_style(error_msg))
-
-            elif hasattr(self, key) and self.__getattribute__(key) is not None:
-                error_msg = f'attribute {type(self).__name__}.{key} is READ ONLY'
-                raise PermissionError(error_style(error_msg))
-
-            else:
-                for allowed_key, allowed_values in self.allowed_keys_values.items():
-                    if key == allowed_key and value not in allowed_values:
-                        error_msg = f'{value} is unsupported for {type(self).__name__}.{key}\n'
-                        error_msg += f'The allowed values of {type(self).__name__}.{key} are {self.allowed_keys_values[key]}'
-                        raise AttributeError(error_style(error_msg))
+class MechanicalThermalExpansion(BaseMaterial):
+    __slots__ = BaseMaterial.__slots__ + ('alpha',)
+
+    def __init__(self, material: Material, dimension: int, section: Section) -> None:
+        super().__init__(material, dimension, section)
+        self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
 
-                super().__setattr__(key, value)
+        self.data_keys = ['Coefficient of thermal expansion alpha']
+
+        if len(self.material.data) != len(self.data_keys):
+            raise NotImplementedError(error_style(self.get_data_length_error_msg()))
         else:
-            super().__setattr__(key, value)
+            for i, key in enumerate(self.data_keys):
+                self.data_dict[key] = material.data[i]
 
-    def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string(self, level)
+        self.alpha: float = self.data_dict['Coefficient of thermal expansion alpha']
 
-    def show(self) -> None:
-        print(self.to_string())
+        self.create_tangent()
+
+    def create_tangent(self):
+        if self.section.type in self.allowed_section_types:
+            if self.dimension == 2:
+                self.tangent = ones(3) * self.alpha
+                self.tangent[self.dimension:] = 0.0
+            elif self.dimension == 3:
+                self.tangent = ones(6) * self.alpha
+                self.tangent[self.dimension:] = 0.0
+        else:
+            error_msg = f'{self.section.type} is not the allowed section types {self.allowed_section_types} of the material {type(self).__name__}, please check the definition of the section {self.section.name}'
+            raise NotImplementedError(error_style(error_msg))
+
+    def get_tangent(self, variable: Dict[str, ndarray],
+                    state_variable: Dict[str, ndarray],
+                    state_variable_new: Dict[str, ndarray],
+                    element_id: int,
+                    igp: int,
+                    ntens: int,
+                    ndi: int,
+                    nshr: int,
+                    timer: Timer) -> Tuple[ndarray, Dict[str, ndarray]]:
+        temperature = variable['temperature']
+        thermal_strain = -self.tangent * temperature
+        output = {'thermal_strain': thermal_strain}
+        return self.tangent, output
 
 
 if __name__ == "__main__":
-    material = Material()
-    print(material.__dict__.keys())
-    print(material)
-    print(material.to_string())
+    from pyfem.io.Properties import Properties
+
+    props = Properties()
+    props.read_file(r'..\..\..\examples\mechanical_thermal\rectangle\Job-1.toml')
+    material_data = MechanicalThermalExpansion(props.materials[2], 3, props.sections[0])
+    material_data.show()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyfem-0.1.1/src/pyfem/io/Output.py` & `pyfem-0.1.2/src/pyfem/io/Output.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from pyfem.utils.visualization import object_dict_to_string
+from typing import Tuple
 
+from pyfem.io.BaseIO import BaseIO
+
+
+class Output(BaseIO):
+    __slots__: Tuple = ('type',
+                        'field_outputs',
+                        'on_screen')
 
-class Output:
     def __init__(self) -> None:
+        super().__init__()
         self.type: str = None  # type: ignore
         self.field_outputs: str = None  # type: ignore
         self.on_screen: bool = None  # type: ignore
 
-    def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string(self, level)
-
-    def show(self) -> None:
-        print(self.to_string())
-
 
 if __name__ == "__main__":
     output = Output()
-    print(output.__dict__.keys())
-    print(output)
-    print(output.to_string())
+    output.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/io/Properties.py` & `pyfem-0.1.2/src/pyfem/io/Properties.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from pathlib import Path
-from typing import Dict, List, Any, Tuple, Union
+from typing import Dict, List, Tuple, Union
 
 try:
     import tomllib  # type: ignore
 except ModuleNotFoundError:
     import tomli as tomllib
 
 from pyfem.io.Dof import Dof
@@ -16,80 +16,74 @@
 from pyfem.io.Mesh import Mesh
 from pyfem.io.BC import BC
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.Solver import Solver
 from pyfem.io.Output import Output
 from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import CYAN, MAGENTA, BLUE, END, error_style, info_style
+from pyfem.io.BaseIO import BaseIO
 
 
-class Properties:
+class Properties(BaseIO):
     """
     Properties类用于解析配置文件中定义的属性。
     当 self.is_read_only = True 时：
 
     1. Properties 类的所有属性在首次被赋非None值后不能再被修改和删除，
 
     2. 此时许可的属性关键字存储在self.slots中。
     """
-    is_read_only: bool = True
-    slots: Tuple = (
-        'work_path', 'input_file', 'toml', 'title', 'mesh', 'dof', 'materials', 'sections', 'amplitudes',
-        'bcs', 'solver', 'outputs', 'mesh_data')
+    __slots__: Tuple = ('work_path',
+                        'input_file',
+                        'abs_input_file',
+                        'toml',
+                        'title',
+                        'mesh',
+                        'dof',
+                        'materials',
+                        'sections',
+                        'amplitudes',
+                        'bcs',
+                        'solver',
+                        'outputs',
+                        'mesh_data')
 
     def __init__(self) -> None:
+        super().__init__()
         self.work_path: Path = None  # type: ignore
         self.input_file: Path = None  # type: ignore
+        self.abs_input_file: Path = None  # type: ignore
         self.toml: Dict = None  # type: ignore
         self.title: str = None  # type: ignore
         self.mesh: Mesh = None  # type: ignore
         self.dof: Dof = None  # type: ignore
         self.materials: List[Material] = None  # type: ignore
         self.sections: List[Section] = None  # type: ignore
         self.amplitudes: List[Amplitude] = None  # type: ignore
         self.bcs: List[BC] = None  # type: ignore
         self.solver: Solver = None  # type: ignore
         self.outputs: List[Output] = None  # type: ignore
         self.mesh_data: MeshData = None  # type: ignore
 
-    def __setattr__(self, key, value):
-        if self.is_read_only:
-            if key not in self.slots:
-                error_msg = f'{key} is not an allowable attribute keyword of {type(self).__name__}'
-                raise AttributeError(error_style(error_msg))
-            elif hasattr(self, key) and self.__getattribute__(key) is not None:
-                error_msg = f'attribute {type(self).__name__}.{key} is READ ONLY'
-                raise PermissionError(error_style(error_msg))
-            else:
-                super().__setattr__(key, value)
-        else:
-            super().__setattr__(key, value)
-
-    def __delattr__(self, key):
-        if self.is_read_only:
-            error_msg = f'attribute {type(self).__name__}.{key} is READ ONLY'
-            raise PermissionError(error_style(error_msg))
-        else:
-            super().__delattr__(key)
-
     def verify(self) -> None:
         print(info_style('Verifying the input ...'))
         is_error = False
         error_msg = '\nInput error:\n'
-        for key in self.slots[2:]:  # 忽略这2个关键字：'work_path', 'input_file'，它们不是在.toml中定义的
+        for key in self.__slots__[3:]:  # 忽略这3个关键字：'work_path', 'input_file', 'abs_input_file'，它们不是在.toml中定义的
             if self.__getattribute__(key) is None:
                 is_error = True
                 error_msg += f'  - {key} is missing\n'
 
         if is_error:
             error_msg += f'Please check the input file {self.input_file}'
             raise NotImplementedError(error_style(error_msg))
 
     def show(self) -> None:
-        for key, item in self.__dict__.items():
+        for key in self.__slots__:
+            item = self.__getattribute__(key)
             print()
             print(CYAN + f'+-{key}' + END)
             print(MAGENTA + f'  |- {type(item)}' + END)
             if hasattr(item, 'to_string'):
                 print(f'  |- {item.to_string()}')
             else:
                 print(f'  |- {item}')
@@ -101,129 +95,89 @@
         self.toml = toml
 
     def set_title(self, title: str) -> None:
         self.title = title
 
     def set_mesh(self, mesh_dict: Dict) -> None:
         self.mesh = Mesh()
-        allowed_keys = self.mesh.__dict__.keys()
-        for key, item in mesh_dict.items():
-            if key in allowed_keys:
-                self.mesh.__setattr__(key, item)
-            else:
-                raise AttributeError(self.key_error_message(key, self.mesh))
+        self.mesh.set_io_values(mesh_dict)
 
         mesh_path = Path(self.mesh.file)
         if mesh_path.is_absolute():  # 判断 self.mesh.file 是不是绝对路径
             abs_mesh_path = mesh_path
         else:  # 如果 self.mesh.file 不是绝对路径，则用工作目录 self.work_path 补全为绝对路径
             abs_mesh_path = self.work_path.joinpath(mesh_path)
         self.mesh_data = MeshData()
         self.mesh_data.read_file(abs_mesh_path, self.mesh.type)
 
     def set_dofs(self, dofs_dict: Dict) -> None:
         self.dof = Dof()
-        allowed_keys = self.dof.__dict__.keys()
-        for key, item in dofs_dict.items():
-            if key in allowed_keys:
-                self.dof.__setattr__(key, item)
-            else:
-                raise AttributeError(self.key_error_message(key, self.dof))
+        self.dof.set_io_values(dofs_dict)
 
     def set_solver(self, solver_dict: Dict) -> None:
         self.solver = Solver()
-        allowed_keys = self.solver.__dict__.keys()
-        for key, item in solver_dict.items():
-            if key in allowed_keys:
-                self.solver.__setattr__(key, item)
-            else:
-                raise AttributeError(self.key_error_message(key, self.solver))
+        self.solver.set_io_values(solver_dict)
 
     def set_materials(self, materials_list: List) -> None:
         self.materials = []
         for material_dict in materials_list:
             material = Material()
-            allowed_keys = material.__dict__.keys()
-            for key, item in material_dict.items():
-                if key in allowed_keys:
-                    material.__setattr__(key, item)
-                else:
-                    raise AttributeError(self.key_error_message(key, material))
+            material.set_io_values(material_dict)
             self.materials.append(material)
 
     def set_sections(self, sections_list: List) -> None:
         self.sections = []
         for section_dict in sections_list:
             section = Section()
-            allowed_keys = section.__dict__.keys()
-            for key, item in section_dict.items():
-                if key in allowed_keys:
-                    section.__setattr__(key, item)
-                else:
-                    raise AttributeError(self.key_error_message(key, section))
+            section.set_io_values(section_dict)
             self.sections.append(section)
 
     def set_amplitudes(self, amplitudes_list: List) -> None:
         self.amplitudes = []
         for amplitude_dict in amplitudes_list:
             amplitude = Amplitude()
-            allowed_keys = amplitude.__dict__.keys()
-            for key, item in amplitude_dict.items():
-                if key in allowed_keys:
-                    amplitude.__setattr__(key, item)
-                else:
-                    raise AttributeError(self.key_error_message(key, amplitude))
+            amplitude.set_io_values(amplitude_dict)
             self.amplitudes.append(amplitude)
 
     def set_bcs(self, bcs_list: List) -> None:
         self.bcs = []
         for bc_dict in bcs_list:
             bc = BC()
-            allowed_keys = bc.__dict__.keys()
-            for key, item in bc_dict.items():
-                if key in allowed_keys:
-                    bc.__setattr__(key, item)
-                else:
-                    raise AttributeError(self.key_error_message(key, bc))
+            bc.set_io_values(bc_dict)
             self.bcs.append(bc)
 
     def set_outputs(self, outputs_list: List) -> None:
         self.outputs = []
         for output_dict in outputs_list:
             output = Output()
-            allowed_keys = output.__dict__.keys()
-            for key, item in output_dict.items():
-                if key in allowed_keys:
-                    output.__setattr__(key, item)
-                else:
-                    raise AttributeError(self.key_error_message(key, output))
+            output.set_io_values(output_dict)
             self.outputs.append(output)
 
-    @staticmethod
-    def key_error_message(key: Any, obj: Any) -> str:
-        return error_style(f'{key} is not an allowable attribute keyword of {type(obj).__name__}')
-
     def read_file(self, filename: Union[Path, str]) -> None:
         """
         读取 .toml 格式的配置文件。
         """
         self.input_file = Path(filename)
         self.work_path = self.input_file.parent
+        if self.input_file.is_absolute():
+            self.abs_input_file = self.input_file
+        else:
+            self.abs_input_file = Path.cwd().joinpath(self.input_file).resolve()
 
         with open(self.input_file, "rb") as f:
             toml = tomllib.load(f)
             self.set_toml(toml)
 
         toml_keys = self.toml.keys()
-        allowed_keys = self.__dict__.keys()
+        allowed_keys = self.__slots__
 
         for key in toml_keys:
             if key not in allowed_keys:
                 error_msg = f'{key} is not an allowable attribute keyword of {type(self).__name__}\n'
-                error_msg += f'Please check the file {self.input_file}'
+                error_msg += f'please check the file {self.abs_input_file}'
                 raise AttributeError(error_style(error_msg))
 
         if 'title' in toml_keys:
             title = self.toml['title']
             self.set_title(title)
 
         if 'sections' in toml_keys:
@@ -259,10 +213,11 @@
             self.set_outputs(outputs_dict)
 
         self.verify()
 
 
 if __name__ == "__main__":
     props = Properties()
-    # props.show()
-    props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
+    props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
     props.show()
+
+    # props.outputs[0].type = 1
```

### Comparing `pyfem-0.1.1/src/pyfem/io/Section.py` & `pyfem-0.1.2/src/pyfem/io/Section.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Optional, List
+from typing import Optional, List, Tuple
 
-from pyfem.utils.visualization import object_dict_to_string
+from pyfem.io.BaseIO import BaseIO
 
 
-class Section:
+class Section(BaseIO):
+    __slots__: Tuple = ('name',
+                        'category',
+                        'type',
+                        'option',
+                        'element_sets',
+                        'material_names',
+                        'data')
+
     def __init__(self) -> None:
+        super().__init__()
         self.name: str = None  # type: ignore
         self.category: str = None  # type: ignore
         self.type: str = None  # type: ignore
         self.option: Optional[str] = None
         self.element_sets: List[str] = None  # type: ignore
         self.material_names: List[str] = None  # type: ignore
         self.data: List = None  # type: ignore
 
-    def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string(self, level)
-
-    def show(self) -> None:
-        print(self.to_string())
-
 
 if __name__ == "__main__":
     section = Section()
-    print(section.__dict__.keys())
-    print(section)
-    print(section.to_string())
+    section.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/io/arguments.py` & `pyfem-0.1.2/src/pyfem/io/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     # 添加帮助选项
     parser.add_argument('-h', '--help', action='help', default=SUPPRESS,
                         help='Show this help message and exit.')
 
     # 添加版本选项
     parser.add_argument('-v', '--version', action='version', help='Show program\'s version number and exit.',
-                        version='pyfem 0.1.1')
+                        version='pyfem 0.1.2')
 
     # 解析命令行参数
     args = parser.parse_args()
 
     # 如果未指定程序输入文件，则打印帮助并退出
     if not args.i:
         print('--------------------------------------')
```

### Comparing `pyfem-0.1.1/src/pyfem/io/write_vtk.py` & `pyfem-0.1.2/src/pyfem/io/write_vtk.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from xml.etree.ElementTree import ElementTree, Element, SubElement
 
 from pyfem.assembly.Assembly import Assembly
+from pyfem.utils.wrappers import show_running_time
 
 
+@show_running_time
 def write_vtk(assembly: Assembly):
     props = assembly.props
     timer = assembly.timer
     dimension = props.mesh_data.dimension
 
     root = Element("VTKFile", {
         "type": "UnstructuredGrid",
@@ -36,14 +38,27 @@
         })
         temp.text = ""
         col_T = props.dof.names.index("T")
         dof_T = assembly.dof_solution.reshape(-1, len(props.dof.names))[:, col_T]
         for T in dof_T:
             temp.text += f"{T} \n"
 
+    if "phi" in props.dof.names:
+        temp = SubElement(point_data, "DataArray", {
+            "type": "Float64",
+            "Name": "PhaseField",
+            "NumberOfComponents": "1",
+            "format": "ascii"
+        })
+        temp.text = ""
+        col_phi = props.dof.names.index("phi")
+        dof_phi = assembly.dof_solution.reshape(-1, len(props.dof.names))[:, col_phi]
+        for phi in dof_phi:
+            temp.text += f"{phi} \n"
+
     if "u1" in props.dof.names:
         disp = SubElement(point_data, "DataArray", {
             "type": "Float64",
             "Name": "Displacement",
             "NumberOfComponents": "3",
             "format": "ascii"
         })
```

### Comparing `pyfem-0.1.1/src/pyfem/materials/BaseMaterial.py` & `pyfem-0.1.2/src/pyfem/solvers/BaseSolver.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Tuple, Dict
+from typing import Tuple
 
 from numpy import ndarray, empty
 
-from pyfem.fem.Timer import Timer
-from pyfem.io.Material import Material
-from pyfem.io.Section import Section
-from pyfem.utils.visualization import object_dict_to_string_ndarray
+from pyfem.assembly.Assembly import Assembly
+from pyfem.io.Solver import Solver
+from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
-class BaseMaterial:
-    def __init__(self, material: Material, dimension: int, section: Section) -> None:
-        self.material: Material = material
-        self.dimension: int = dimension
-        self.section: Section = section
-        self.allowed_section_types: Tuple = ()
-        self.ddsdde: ndarray = empty(0)
-        self.output: Dict[str, ndarray] = {}
+class BaseSolver:
+    __slots__: Tuple = ('assembly',
+                        'solver',
+                        'dof_solution')
+
+    def __init__(self) -> None:
+        self.assembly: Assembly = None  # type: ignore
+        self.solver: Solver = None  # type: ignore
+        self.dof_solution: ndarray = empty(0)
 
     def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string_ndarray(self, level)
+        return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
-    def get_tangent(self, variable: Dict[str, ndarray],
-                    state_variable: Dict[str, ndarray],
-                    state_variable_new: Dict[str, ndarray],
-                    element_id: int,
-                    igp: int,
-                    ntens: int,
-                    ndi: int,
-                    nshr: int,
-                    timer: Timer) -> Tuple[ndarray, Dict[str, ndarray]]:
-        return self.ddsdde, self.output
+    def run(self) -> int:
+        return -1
+
+    def solve(self) -> int:
+        return -1
+
+
+if __name__ == "__main__":
+    solver = BaseSolver()
+    solver.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/materials/ElasticIsotropic.py` & `pyfem-0.1.2/src/pyfem/materials/ElasticIsotropic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Optional, Tuple, Dict
+from typing import Tuple, Dict
 
 from numpy import array, outer, diag, ndarray, dot
 
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 
 class ElasticIsotropic(BaseMaterial):
+    __slots__ = BaseMaterial.__slots__ + ('E', 'nu')
 
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
-        self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain', None)
+        self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
+
+        self.data_keys = ['Young\'s modulus E', 'Poisson\'s ratio nu']
+
+        if len(self.material.data) != len(self.data_keys):
+            raise NotImplementedError(error_style(self.get_data_length_error_msg()))
+        else:
+            for i, key in enumerate(self.data_keys):
+                self.data_dict[key] = material.data[i]
+
+        self.E: float = self.data_dict['Young\'s modulus E']
+        self.nu: float = self.data_dict['Poisson\'s ratio nu']
+
         self.create_tangent()
 
     def create_tangent(self):
-        young = self.material.data[0]
-        poisson = self.material.data[1]
-
         if self.section.type in self.allowed_section_types:
-            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.section.type)
+            self.tangent = get_stiffness_from_young_poisson(self.dimension, self.E, self.nu, self.section.type)
         else:
-            error_msg = f'{self.section.type} is not the allowed section types {self.allowed_section_types} of the material {type(self).__name__}, please check the definition of the section {self.section.name}'
-            raise NotImplementedError(error_style(error_msg))
+            raise NotImplementedError(error_style(self.get_section_type_error_msg()))
 
     def get_tangent(self, variable: Dict[str, ndarray],
                     state_variable: Dict[str, ndarray],
                     state_variable_new: Dict[str, ndarray],
                     element_id: int,
                     igp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
                     timer: Timer) -> Tuple[ndarray, Dict[str, ndarray]]:
         strain = variable['strain']
-        stress = dot(self.ddsdde, strain)
+        dstrain = variable['dstrain']
+        stress = dot(self.tangent, strain + dstrain)
         output = {'stress': stress}
-        return self.ddsdde, output
+        return self.tangent, output
 
 
-def get_lame_from_young_poisson(young: float, poisson: float, plane: Optional[str]) -> Tuple[float, float]:
+def get_lame_from_young_poisson(young: float, poisson: float, plane: str) -> Tuple[float, float]:
     r"""
     Compute Lamé parameters from Young's modulus and Poisson's ratio.
 
     The relationship between Lamé parameters and Young's modulus, Poisson's
     ratio (see [1],[2]):
 
     .. math::
@@ -95,15 +105,15 @@
     do1 = diag(o + 1.0)
 
     lam_array = array(lam, dtype=DTYPE)[..., None, None]
     mu_array = array(mu, dtype=DTYPE)[..., None, None]
     return lam_array * oot + mu_array * do1
 
 
-def get_stiffness_from_young_poisson(dim: int, young: float, poisson: float, plane: Optional[str]) -> ndarray:
+def get_stiffness_from_young_poisson(dim: int, young: float, poisson: float, plane: str) -> ndarray:
     """
     Compute stiffness tensor corresponding to Young's modulus and Poisson's
     ratio.
     """
 
     lam, mu = get_lame_from_young_poisson(young, poisson, plane)
 
@@ -154,36 +164,36 @@
 
     .. math::
         \gamma = \lambda + {2 \over 3} \mu
     """
     return lam + 2.0 * mu / 3.0
 
 
-def get_bulk_from_young_poisson(young: float, poisson: float, plane: Optional[str]) -> float:
+def get_bulk_from_young_poisson(young: float, poisson: float, plane: str) -> float:
     """
     Compute bulk modulus corresponding to Young's modulus and Poisson's ratio.
     """
     lam, mu = get_lame_from_young_poisson(young, poisson, plane)
 
     return get_bulk_from_lame(lam, mu)
 
 
-def get_lame_from_stiffness(stiffness: ndarray, plane: Optional[str]) -> Tuple[float, float]:
+def get_lame_from_stiffness(stiffness: ndarray, plane: str) -> Tuple[float, float]:
     """
     Compute Lamé parameters from an isotropic stiffness tensor.
     """
     lam = float(stiffness[..., 0, 1])
     mu = float(stiffness[..., -1, -1])
     if plane == 'PlaneStress':
         lam = - 2.0 * mu * lam / (lam - 2.0 * mu)
 
     return lam, mu
 
 
-def get_young_poisson_from_stiffness(stiffness: ndarray, plane: Optional[str]) -> Tuple[float, float]:
+def get_young_poisson_from_stiffness(stiffness: ndarray, plane: str) -> Tuple[float, float]:
     """
     Compute Young's modulus and Poisson's ratio from an isotropic stiffness
     tensor.
     """
     lam, mu = get_lame_from_stiffness(stiffness, plane)
     young = (3 * lam * mu + 2 * mu ** 2) / (lam + mu)
     poisson = lam / (2 * lam + 2 * mu)
@@ -191,11 +201,10 @@
     return young, poisson
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
     props = Properties()
-    props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
-
-    material_data = ElasticIsotropic(props.materials[0], 3, props.sections[0])
-    print(material_data.ddsdde.dtype)
+    props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
+    material_data = ElasticIsotropic(props.materials[1], 3, props.sections[0])
+    material_data.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/materials/PlasticKinematicHardening.py` & `pyfem-0.1.2/src/pyfem/materials/PlasticKinematicHardening.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,36 +13,56 @@
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import get_stiffness_from_young_poisson
 from pyfem.utils.colors import error_style
 
 
 class PlasticKinematicHardening(BaseMaterial):
+    __slots__ = BaseMaterial.__slots__ + ('E',
+                                          'nu',
+                                          'yield_stress',
+                                          'hard',
+                                          'EBULK3',
+                                          'EG2',
+                                          'EG',
+                                          'EG3',
+                                          'ELAM',
+                                          'tolerance')
 
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
-        self.allowed_section_types = ('PlaneStress', 'PlaneStrain', 'Volume')
-        self.young: float = self.material.data[0]
-        self.poisson: float = self.material.data[1]
-        self.yield_stress: float = self.material.data[2]
-        self.hard: float = self.material.data[3]
-        self.EBULK3: float = self.young / (1.0 - 2.0 * self.poisson)
-        self.EG2: float = self.young / (1.0 + self.poisson)
+        self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
+
+        self.data_keys = ['Young\'s modulus E', 'Poisson\'s ratio nu', 'Yield stress', 'Hardening coefficient']
+
+        if len(self.material.data) != len(self.data_keys):
+            raise NotImplementedError(error_style(self.get_data_length_error_msg()))
+        else:
+            for i, key in enumerate(self.data_keys):
+                self.data_dict[key] = material.data[i]
+
+        self.E: float = self.data_dict['Young\'s modulus E']
+        self.nu: float = self.data_dict['Poisson\'s ratio nu']
+        self.yield_stress: float = self.data_dict['Yield stress']
+        self.hard: float = self.data_dict['Hardening coefficient']
+
+        self.EBULK3: float = self.E / (1.0 - 2.0 * self.nu)
+        self.EG2: float = self.E / (1.0 + self.nu)
         self.EG: float = self.EG2 / 2.0
         self.EG3: float = 3.0 * self.EG
         self.ELAM: float = (self.EBULK3 - self.EG2) / 3.0
         self.tolerance: float = 1.0e-10
+
         self.create_tangent()
 
     def create_tangent(self):
         if self.section.type in self.allowed_section_types:
-            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, self.young, self.poisson, self.section.type)
+            self.tangent = get_stiffness_from_young_poisson(self.dimension, self.E, self.nu, self.section.type)
         else:
-            error_msg = f'{self.section.type} is not the allowed section types {self.allowed_section_types} of the material {type(self).__name__}, please check the definition of the section {self.section.name}'
-            raise NotImplementedError(error_style(error_msg))
+            raise NotImplementedError(error_style(self.get_section_type_error_msg()))
 
     def get_tangent(self, variable: Dict[str, ndarray],
                     state_variable: Dict[str, ndarray],
                     state_variable_new: Dict[str, ndarray],
                     element_id: int,
                     igp: int,
                     ntens: int,
@@ -59,16 +79,16 @@
         elastic_strain = deepcopy(state_variable['elastic_strain'])
         plastic_strain = deepcopy(state_variable['plastic_strain'])
         back_stress = deepcopy(state_variable['back_stress'])
         stress = deepcopy(state_variable['stress'])
 
         dstrain = variable['dstrain']
 
-        E = self.young
-        nu = self.poisson
+        E = self.E
+        nu = self.nu
 
         if self.section.type == 'PlaneStrain':
             dstrain = insert(dstrain, 2, 0)
         elif self.section.type == 'PlaneStress':
             dstrain = insert(dstrain, 2, -nu / (1 - nu) * (dstrain[0] + dstrain[1]))
 
         elastic_strain += dstrain
@@ -166,12 +186,13 @@
         smises = sqrt(0.5 * smises)
         return float(smises)
     else:
         raise NotImplementedError(error_style(f'unsupported stress dimension {len(s)}'))
 
 
 if __name__ == "__main__":
-    from pyfem.Job import Job
-
-    job = Job(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
+    from pyfem.io.Properties import Properties
 
-    material_data = PlasticKinematicHardening(job.props.materials[0], 3, job.props.sections[0])
+    props = Properties()
+    props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
+    material_data = PlasticKinematicHardening(props.materials[0], 3, props.sections[0])
+    material_data.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/materials/ThermalIsotropic.py` & `pyfem-0.1.2/src/pyfem/materials/BaseMaterial.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Tuple, Dict
+from typing import Dict, List, Tuple
 
-from numpy import eye, ndarray, dot
+from numpy import ndarray, empty
 
 from pyfem.fem.Timer import Timer
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
-from pyfem.materials.BaseMaterial import BaseMaterial
-from pyfem.utils.colors import error_style
+from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
-class ThermalIsotropic(BaseMaterial):
+class BaseMaterial:
+    __slots__: Tuple = ('material',
+                        'dimension',
+                        'section',
+                        'allowed_section_types',
+                        'tangent',
+                        'output',
+                        'data_keys',
+                        'data_dict')
 
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
-        super().__init__(material, dimension, section)
-        self.allowed_section_types = ('Static', 'PlaneStrain')
-        self.create_tangent()
-
-    def create_tangent(self):
-        conductivity = self.material.data[0]
-        capacity = self.material.data[1]
-
-        if self.section.type in self.allowed_section_types:
-            self.ddsdde = eye(self.dimension) * conductivity
-        else:
-            error_msg = f'{self.section.type} is not the allowed section types {self.allowed_section_types} of the material {type(self).__name__}, please check the definition of the section {self.section.name}'
-            raise NotImplementedError(error_style(error_msg))
+        self.material: Material = material
+        self.dimension: int = dimension
+        self.section: Section = section
+        self.allowed_section_types: Tuple = ()
+        self.tangent: ndarray = empty(0)
+        self.output: Dict[str, ndarray] = {}
+        self.data_keys: List[str] = []
+        self.data_dict: Dict[str, float] = {}
+
+    def get_section_type_error_msg(self) -> str:
+        return f'\'{self.section.type}\' is not the allowed section types {self.allowed_section_types} of the material \'{self.material.name}\' -> {type(self).__name__}, please check the definition of the section \'{self.section.name}\''
+
+    def get_data_length_error_msg(self) -> str:
+        return f'the length of \'data\' -> {self.material.data} of \'{self.material.name}\' -> {type(self).__name__} must be {len(self.data_keys)} and stored in the order of {self.data_keys}'
+
+    def to_string(self, level: int = 1) -> str:
+        return object_slots_to_string_ndarray(self, level)
+
+    def show(self) -> None:
+        print(self.to_string())
+
+    def create_tangent(self) -> None:
+        pass
 
     def get_tangent(self, variable: Dict[str, ndarray],
                     state_variable: Dict[str, ndarray],
                     state_variable_new: Dict[str, ndarray],
                     element_id: int,
                     igp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
                     timer: Timer) -> Tuple[ndarray, Dict[str, ndarray]]:
-        temperature_gradient = variable['temperature_gradient']
-        heat_flux = dot(-self.ddsdde, temperature_gradient)
-        output = {'heat_flux': heat_flux}
-        return self.ddsdde, output
-
-
-if __name__ == "__main__":
-    from pyfem.io.Properties import Properties
-
-    props = Properties()
-    props.read_file(r'F:\Github\pyfem\examples\thermal\1element\hex8\Job-1.toml')
-
-    material_data = ThermalIsotropic(props.materials[0], 3, props.sections[0])
-    material_data.show()
+        return self.tangent, self.output
```

### Comparing `pyfem-0.1.1/src/pyfem/materials/ViscoElasticMaxwell.py` & `pyfem-0.1.2/src/pyfem/materials/ViscoElasticMaxwellUMAT.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,37 +13,51 @@
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import get_stiffness_from_young_poisson
 from pyfem.utils.colors import error_style
 
 
 class ViscoElasticMaxwell(BaseMaterial):
+    __slots__ = BaseMaterial.__slots__ + ('E0',
+                                          'E1',
+                                          'E2',
+                                          'E3',
+                                          'TAU1',
+                                          'TAU2',
+                                          'TAU3',
+                                          'POISSON')
 
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
-        self.allowed_section_types = ('PlaneStress', 'PlaneStrain', 'Volume')
-        self.E0: float = self.material.data[0]
-        self.E1: float = self.material.data[1]
-        self.E2: float = self.material.data[2]
-        self.E3: float = self.material.data[3]
-        self.TAU1: float = self.material.data[4]
-        self.TAU2: float = self.material.data[5]
-        self.TAU3: float = self.material.data[6]
-        self.POISSON: float = self.material.data[7]
+        self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
+
+        self.data_keys = ['E0', 'Poisson\'s ratio nu', 'E1', 'TAU1', 'E2', 'TAU2', 'E3', 'TAU3']
+
+        if len(self.material.data) != len(self.data_keys):
+            raise NotImplementedError(error_style(self.get_data_length_error_msg()))
+        else:
+            for i, key in enumerate(self.data_keys):
+                self.data_dict[key] = material.data[i]
+
+        self.E0: float = self.data_dict['E0']
+        self.E1: float = self.data_dict['E1']
+        self.E2: float = self.data_dict['E2']
+        self.E3: float = self.data_dict['E3']
+        self.TAU1: float = self.data_dict['TAU1']
+        self.TAU2: float = self.data_dict['TAU2']
+        self.TAU3: float = self.data_dict['TAU3']
+        self.POISSON: float = self.data_dict['Poisson\'s ratio nu']
+
         self.create_tangent()
 
     def create_tangent(self):
-        young = self.material.data[0]
-        poisson = self.material.data[1]
-
         if self.section.type in self.allowed_section_types:
-            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.section.type)
+            self.tangent = get_stiffness_from_young_poisson(self.dimension, self.E0, self.POISSON, self.section.type)
         else:
-            error_msg = f'{self.section.type} is not the allowed section types {self.allowed_section_types} of the material {type(self).__name__}, please check the definition of the section {self.section.name}'
-            raise NotImplementedError(error_style(error_msg))
+            raise NotImplementedError(error_style(self.get_section_type_error_msg()))
 
     def get_tangent(self, variable: Dict[str, ndarray],
                     state_variable: Dict[str, ndarray],
                     state_variable_new: Dict[str, ndarray],
                     element_id: int,
                     igp: int,
                     ntens: int,
@@ -83,18 +97,14 @@
         m1 = (TAU1 * mu1 - TAU1 * mu1 * exp(-dtime / TAU1)) / (mu0 * dtime)
         m2 = (TAU2 * mu2 - TAU2 * mu2 * exp(-dtime / TAU2)) / (mu0 * dtime)
         m3 = (TAU3 * mu3 - TAU3 * mu3 * exp(-dtime / TAU3)) / (mu0 * dtime)
 
         term1 = BULK + (4.0 * mu0) / 3.0
         term2 = BULK - (2.0 * mu0) / 3.0
 
-        a1 = exp(-dtime / TAU1)
-        a2 = exp(-dtime / TAU2)
-        a3 = exp(-dtime / TAU3)
-
         g = zeros((ntens, ntens), dtype=DTYPE)
 
         for i in range(ndi):
             g[i, i] = term1
         for i in range(1, ndi):
             for j in range(0, i):
                 g[i, j] = term2
@@ -109,14 +119,17 @@
                         SM1OLD[i] + SM2OLD[i] + SM3OLD[i] + (1 + m1 + m2 + m3) * \
                         (g[i, 0] * dstrain[0] + g[i, 1] * dstrain[1] + g[i, 2] * dstrain[2])
 
         for i in range(ndi, ntens):
             stress[i] = g[i, i] * strain[i] + SM1OLD[i] + SM2OLD[i] + SM3OLD[i] + (1 + m1 + m2 + m3) * (
                     g[i, i] * dstrain[i])
 
+        if element_id == 0 and igp == 0:
+            print(stress)
+
         SM1 = zeros(ntens, dtype=DTYPE)
         SM2 = zeros(ntens, dtype=DTYPE)
         SM3 = zeros(ntens, dtype=DTYPE)
 
         for i in range(ndi):
             SM1[i] = SM1OLD[i] + m1 * g[i, 0] * dstrain[0] + g[i, 1] * dstrain[1] + g[i, 2] * dstrain[2]
             SM2[i] = SM2OLD[i] + m2 * g[i, 0] * dstrain[0] + g[i, 1] * dstrain[1] + g[i, 2] * dstrain[2]
@@ -140,13 +153,13 @@
 
         output = {'stress': stress}
 
         return ddsdde, output
 
 
 if __name__ == "__main__":
-    from pyfem.Job import Job
-
-    job = Job(r'F:\Github\pyfem\examples\specimen3D\Job-1.toml')
+    from pyfem.io.Properties import Properties
 
-    material_data = ViscoElasticMaxwell(job.props.materials[2], 3, job.props.sections[0])
-    print(material_data.to_string())
+    props = Properties()
+    props.read_file(r'..\..\..\examples\mechanical\1element\hex8\Job-1.toml')
+    material_data = ViscoElasticMaxwell(props.materials[2], 3, props.sections[0])
+    material_data.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/materials/get_material_data.py` & `pyfem-0.1.2/src/pyfem/materials/get_material_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 
 """
 
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import ElasticIsotropic
+from pyfem.materials.MechanicalThermalExpansion import MechanicalThermalExpansion
+from pyfem.materials.PhaseFieldDamage import PhaseFieldDamage
 from pyfem.materials.PlasticKinematicHardening import PlasticKinematicHardening
 from pyfem.materials.ThermalIsotropic import ThermalIsotropic
 from pyfem.materials.ViscoElasticMaxwell import ViscoElasticMaxwell
 from pyfem.utils.colors import error_style
 
 material_data_dict = {
     'ElasticIsotropic': ElasticIsotropic,
     'PlasticKinematicHardening': PlasticKinematicHardening,
     'ViscoElasticMaxwell': ViscoElasticMaxwell,
-    'ThermalIsotropic': ThermalIsotropic
-
+    'ThermalIsotropic': ThermalIsotropic,
+    'MechanicalThermalExpansion': MechanicalThermalExpansion,
+    'PhaseFieldDamage': PhaseFieldDamage
 }
 
 
 def get_material_data(material: Material, dimension: int, section: Section) -> BaseMaterial:
     class_name = f'{material.category}{material.type}'.strip().replace(' ', '')
 
     if class_name in material_data_dict:
```

### Comparing `pyfem-0.1.1/src/pyfem/mesh/MeshData.py` & `pyfem-0.1.2/src/pyfem/mesh/MeshData.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 from pyfem.fem.constants import DTYPE
 from pyfem.utils.colors import BLUE, END
 from pyfem.utils.colors import error_style, info_style
 from pyfem.utils.wrappers import show_running_time
 
 
 class MeshData:
+    __slots__ = ('dimension',
+                 'mesh',
+                 'nodes',
+                 'elements',
+                 'bc_elements',
+                 'node_sets',
+                 'element_sets',
+                 'bc_element_sets')
 
     def __init__(self) -> None:
         self.dimension: int = -1
         self.mesh: meshio.Mesh = None  # type: ignore
         self.nodes: ndarray = empty(0)
         self.elements: List[ndarray] = []
         self.bc_elements: List[ndarray] = []
@@ -135,10 +143,10 @@
         else:
             self.node_sets[node_set_name] += node_ids
 
 
 if __name__ == "__main__":
     mesh_data = MeshData()
     # mesh_data.read_file(r'F:\Github\pyfem\examples\rectangle\quad40000.msh', 'gmsh')
-    mesh_data.read_file(r'F:\Github\pyfem\examples\hole\hole_quad4.inp', 'abaqus')
+    mesh_data.read_file(r'F:\Github\pyfem\examples\mechanical\rectangle_hole\rectangle_hole_quad4.inp', 'abaqus')
     # mesh_data.read_file(r'F:\Github\pyfem\examples\quad_tria\Job-1.inp', 'abaqus')
     mesh_data.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/solvers/BaseSolver.py` & `pyfem-0.1.2/src/pyfem/solvers/get_solver_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-from numpy import ndarray, empty
+# -*- coding: utf-8 -*-
+"""
 
+"""
 from pyfem.assembly.Assembly import Assembly
 from pyfem.io.Solver import Solver
-from pyfem.utils.visualization import object_dict_to_string_ndarray
-
-
-class BaseSolver:
-    def __init__(self) -> None:
-        self.assembly: Assembly = None  # type: ignore
-        self.solver: Solver = None  # type: ignore
-        self.solution: ndarray = empty(0)
-
-    def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string_ndarray(self, level)
-
-    def show(self) -> None:
-        print(self.to_string())
-
-    def run(self) -> None:
-        pass
-
-    def solve(self) -> None:
-        pass
+from pyfem.solvers.BaseSolver import BaseSolver
+from pyfem.solvers.LinearSolver import LinearSolver
+from pyfem.solvers.NonlinearSolver import NonlinearSolver
+from pyfem.utils.colors import error_style
+
+solver_data_dict = {
+    'LinearSolver': LinearSolver,
+    'NonlinearSolver': NonlinearSolver
+}
+
+
+def get_solver_data(assembly: Assembly, solver: Solver) -> BaseSolver:
+    class_name = f'{solver.type}'.strip().replace(' ', '')
+
+    if class_name in solver_data_dict:
+        return solver_data_dict[class_name](assembly=assembly,
+                                            solver=solver)
+    else:
+        error_msg = f'{class_name} solver is not supported.\n'
+        error_msg += f'The allowed solver types are {list(solver_data_dict.keys())}.'
+        raise NotImplementedError(error_style(error_msg))
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `pyfem-0.1.1/src/pyfem/solvers/LinearSolver.py` & `pyfem-0.1.2/src/pyfem/solvers/LinearSolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Solver import Solver
 from pyfem.io.write_vtk import write_vtk
 from pyfem.solvers.BaseSolver import BaseSolver
 
 
 class LinearSolver(BaseSolver):
+    __slots__ = BaseSolver.__slots__ + ('PENALTY',)
+
     def __init__(self, assembly: Assembly, solver: Solver) -> None:
         super().__init__()
-        self.assembly: Assembly = assembly
-        self.solver: Solver = solver
+        self.assembly = assembly
+        self.solver = solver
         self.dof_solution = empty(0, dtype=DTYPE)
-        self.PENALTY = 1.0e16
+        self.PENALTY: float = 1.0e16
 
-    def run(self) -> None:
-        self.solve()
+    def run(self) -> int:
+        return self.solve()
 
-    def solve(self) -> None:
+    def solve(self) -> int:
         A = self.assembly.global_stiffness
         rhs = self.assembly.fext
 
         for bc_data in self.assembly.bc_data_list:
             if bc_data.bc.category == 'DirichletBC':
                 for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
                     A[dof_id, dof_id] += self.PENALTY
@@ -41,10 +43,16 @@
         self.dof_solution = x
         self.assembly.dof_solution = x
         self.assembly.update_element_data()
         self.assembly.update_element_field_variables()
         self.assembly.assembly_field_variables()
         write_vtk(self.assembly)
 
+        return 0
+
 
 if __name__ == "__main__":
-    pass
+    from pyfem.Job import Job
+
+    job = Job(r'..\..\..\examples\mechanical\plane\Job-1.toml')
+    solver = LinearSolver(job.assembly, job.props.solver)
+    solver.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/solvers/NonlinearSolver.py` & `pyfem-0.1.2/src/pyfem/solvers/NonlinearSolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,30 +14,35 @@
 from pyfem.io.write_vtk import write_vtk, write_pvd
 from pyfem.solvers.BaseSolver import BaseSolver
 from pyfem.utils.colors import error_style
 from pyfem.utils.colors import info_style
 
 
 class NonlinearSolver(BaseSolver):
+    __slots__ = BaseSolver.__slots__ + ('PENALTY', 'FORCE_TOL', 'MAX_NITER')
+
     def __init__(self, assembly: Assembly, solver: Solver) -> None:
         super().__init__()
-        self.assembly: Assembly = assembly
-        self.solver: Solver = solver
+        self.assembly = assembly
+        self.solver = solver
         self.dof_solution = zeros(self.assembly.total_dof_number)
-        self.PENALTY = 1.0e16
-        self.FORCE_TOL = 1.0e-6
-        self.MAX_NITER = 32
-
-    def run(self) -> None:
-        if self.assembly.props.solver.option in ['', 'NewtonRaphson', None]:
-            self.Newton_Raphson_solve()
-        elif self.assembly.props.solver.option == 'InitialTangent':
-            self.initial_tangent_solve()
+        self.PENALTY: float = 1.0e16
+        self.FORCE_TOL: float = 1.0e-6
+        self.MAX_NITER: int = 32
+
+    def run(self) -> int:
+        if self.assembly.props.solver.option in [None, '', 'NR', 'NewtonRaphson']:
+            return self.Newton_Raphson_solve()
+        elif self.assembly.props.solver.option in ['IT', 'InitialTangent']:
+            return self.initial_tangent_solve()
+        else:
+            raise NotImplementedError(error_style(
+                f'unsupported option \'{self.assembly.props.solver.option}\' of {self.assembly.props.solver.type}'))
 
-    def Newton_Raphson_solve(self) -> None:
+    def Newton_Raphson_solve(self) -> int:
         timer = self.assembly.timer
         timer.total_time = self.solver.total_time
         timer.dtime = self.solver.initial_dtime
         timer.time0 = self.solver.start_time
         timer.increment = 0
         timer.frame_ids.append(0)
 
@@ -109,17 +114,20 @@
             timer.frame_ids.append(increment)
 
             if timer.is_done():
                 write_pvd(self.assembly)
                 break
 
         if not timer.is_done():
-            raise NotImplementedError(error_style('maximum increment is reached'))
+            print((error_style('maximum increment is reached')))
+            return -1
+        else:
+            return 0
 
-    def initial_tangent_solve(self) -> None:
+    def initial_tangent_solve(self) -> int:
         self.MAX_NITER = 1024
         timer = self.assembly.timer
 
         timer.total_time = self.solver.total_time
         timer.dtime = self.solver.initial_dtime
         timer.time0 = self.solver.start_time
         timer.increment = 0
@@ -194,12 +202,19 @@
             timer.frame_ids.append(increment)
 
             if timer.is_done():
                 write_pvd(self.assembly)
                 break
 
         if not timer.is_done():
-            raise NotImplementedError(error_style('maximum increment is reached'))
+            print((error_style('maximum increment is reached')))
+            return -1
+        else:
+            return 0
 
 
 if __name__ == "__main__":
-    pass
+    from pyfem.Job import Job
+
+    job = Job(r'..\..\..\examples\mechanical\plane\Job-1.toml')
+    solver = NonlinearSolver(job.assembly, job.props.solver)
+    solver.show()
```

### Comparing `pyfem-0.1.1/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.1.2/src/pyfem/utils/IntKeyDict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Dict, List, Any
+from typing import Dict, List, Any, Tuple
 
 
 class IntKeyDict(dict):
     """
     关键字只能为整数（Integer）类型的字典，已经存在的键值无法通过赋值方法（__setitem__）更改。
     """
+    __slots__: Tuple = ('indices_to_ids',
+                        'ids_to_indices')
 
     def __init__(self) -> None:
         super().__init__()
         self.indices_to_ids: Dict[int, int] = {}
         self.ids_to_indices: Dict[int, int] = {}
         self.update_indices()
```

### Comparing `pyfem-0.1.1/src/pyfem/utils/colors.py` & `pyfem-0.1.2/src/pyfem/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.1/src/pyfem/utils/logger.py` & `pyfem-0.1.2/src/pyfem/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.1/src/pyfem/utils/wrappers.py` & `pyfem-0.1.2/src/pyfem/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.1/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.1.2/src/pyfem.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.1.1
+Version: 0.1.2
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,47 +27,47 @@
 pip install pyfem
 ```
 
 ## Development
 
 ### ToDo list
 
-- [ ] 增加Neumann边界条件，支持concentrated force，pressure，traction和函数定义方式
+- [x] 增加Neumann边界条件，支持concentrated force，distributed和pressure定义方式
 - [ ] 增加hdf5计算结果输出格式
 - [ ] 完善帮助文档
 - [ ] 完善输入文件的校检
-- [ ] 增加测试模块
+- [x] 增加测试模块
 - [ ] 增加日志模块
 - [ ] 增加后台运行模式
 - [ ] 处理平面应力状态的面外应力平衡
 - [x] 增加粘弹性力学本构模型
 - [ ] 增加晶体塑性力学本构模型
-- [ ] 增加温度场求解单元
-- [ ] 增加温度场-位移场耦合求解单元
-- [ ] 增加相场-位移场耦合求解单元
+- [x] 增加温度场求解单元
+- [x] 增加温度场-位移场耦合求解单元
+- [x] 增加相场-位移场耦合求解单元
 - [ ] 增加内聚区单元
 - [ ] 增加动力学求解器
 - [ ] 建立前处理界面
 
 ## Tutorial
 
 #### Run in command line:
 
 ```bash
 pyfem -i Job-1.toml
 ```
 
-#### Example with geometry file:
+#### Job file Job-1.toml:
 
 ```toml
 title = "Job-1"
 
 [mesh]
 type = "abaqus"
-file = "Job-1.inp"
+file = "hex8.inp"
 
 [dof]
 names = ["u1", "u2", "u3"]
 order = 1
 family = "LAGRANGE"
 
 [[bcs]]
@@ -95,27 +95,27 @@
 dof = ["u3"]
 node_sets = ['Set-Z0']
 element_sets = []
 value = 0.0
 
 [[bcs]]
 name = "BC-4"
-category = "DirichletBC"
-type = ""
+category = "NeumannBC"
+type = "Distributed"
 dof = ["u1"]
 node_sets = ['Set-X1']
-element_sets = []
+element_sets = ['Set-X1']
 value = 1.0
 
 [solver]
 type = "NonlinearSolver"
 option = "NewtonRaphson"
-total_time = 0.01
+total_time = 1.0
 max_increment = 1000000
-initial_dtime = 0.001
+initial_dtime = 0.1
 max_dtime = 1.0
 min_dtime = 0.001
 
 [[materials]]
 name = "Material-1"
 category = "Plastic"
 type = "KinematicHardening"
@@ -131,24 +131,24 @@
 
 [[sections]]
 name = "Section-1"
 category = "Solid"
 type = "Volume"
 option = "SmallStrain"
 element_sets = ["Set-All"]
-material_name = "Material-1"
+material_names = ["Material-1"]
 data = []
 
 [[outputs]]
 type = "vtk"
 field_outputs = ['S11', 'S22', 'S33', 'S12', 'S13', 'S23', 'E11', 'E22', 'E33', 'E12', 'E13', 'E23']
 on_screen = false
 ```
 
-### geometry file in abaqus formate:
+#### abaqus geometry file hex8.inp:
 
 ```abaqus
 *Heading
 *Preprint, echo=NO, model=NO, history=NO, contact=NO
 **
 ** PARTS
 **
@@ -200,7 +200,11 @@
 *Assembly, name=Assembly
 **  
 *Instance, name=Part-1-1, part=Part-1
 *End Instance
 **  
 *End Assembly
 ```
+
+### Bug list
+
+- [ ] 采用abaqus网格文件时，如果存在node不属于任何element则在计算时会导致全局刚度矩阵奇异。
```

### Comparing `pyfem-0.1.1/src/pyfem.egg-info/SOURCES.txt` & `pyfem-0.1.2/src/pyfem.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,59 +14,66 @@
 src/pyfem/amplitude/TabularAmplitude.py
 src/pyfem/amplitude/__init__.py
 src/pyfem/amplitude/get_amplitude_data.py
 src/pyfem/assembly/Assembly.py
 src/pyfem/assembly/__init__.py
 src/pyfem/bc/BaseBC.py
 src/pyfem/bc/DirichletBC.py
-src/pyfem/bc/NeumannBC.py
 src/pyfem/bc/NeumannBCConcentrated.py
 src/pyfem/bc/NeumannBCDistributed.py
+src/pyfem/bc/NeumannBCPressure.py
 src/pyfem/bc/__init__.py
 src/pyfem/bc/get_bc_data.py
 src/pyfem/elements/BaseElement.py
 src/pyfem/elements/IsoElementDiagram.py
 src/pyfem/elements/IsoElementShape.py
+src/pyfem/elements/SolidPhaseFieldDamagePlaneSmallStrain.py
 src/pyfem/elements/SolidPlaneSmallStrain.py
 src/pyfem/elements/SolidThermalPlaneSmallStrain.py
 src/pyfem/elements/SolidVolumeSmallStrain.py
-src/pyfem/elements/ThermalStatic.py
+src/pyfem/elements/Thermal.py
 src/pyfem/elements/__init__.py
+src/pyfem/elements/derive.py
 src/pyfem/elements/get_element_data.py
 src/pyfem/elements/get_iso_element_type.py
 src/pyfem/fem/Timer.py
 src/pyfem/fem/__init__.py
 src/pyfem/fem/constants.py
 src/pyfem/io/Amplitude.py
 src/pyfem/io/BC.py
+src/pyfem/io/BaseIO.py
 src/pyfem/io/Dof.py
 src/pyfem/io/Material.py
 src/pyfem/io/Mesh.py
 src/pyfem/io/Output.py
 src/pyfem/io/Properties.py
 src/pyfem/io/Section.py
 src/pyfem/io/Solver.py
 src/pyfem/io/__init__.py
 src/pyfem/io/arguments.py
 src/pyfem/io/write_vtk.py
 src/pyfem/materials/BaseMaterial.py
 src/pyfem/materials/ElasticIsotropic.py
+src/pyfem/materials/MechanicalThermalExpansion.py
+src/pyfem/materials/PhaseFieldDamage.py
 src/pyfem/materials/PlasticKinematicHardening.py
 src/pyfem/materials/ThermalIsotropic.py
 src/pyfem/materials/ViscoElasticMaxwell.py
+src/pyfem/materials/ViscoElasticMaxwellUMAT.py
 src/pyfem/materials/__init__.py
 src/pyfem/materials/get_material_data.py
-src/pyfem/mesh/ElementSet.py
 src/pyfem/mesh/MeshData.py
-src/pyfem/mesh/NodeSet.py
 src/pyfem/mesh/__init__.py
 src/pyfem/solvers/BaseSolver.py
 src/pyfem/solvers/LinearSolver.py
 src/pyfem/solvers/NonlinearSolver.py
 src/pyfem/solvers/__init__.py
 src/pyfem/solvers/get_solver_data.py
 src/pyfem/utils/IntKeyDict.py
 src/pyfem/utils/__init__.py
 src/pyfem/utils/colors.py
+src/pyfem/utils/data_types.py
+src/pyfem/utils/derive.py
 src/pyfem/utils/logger.py
+src/pyfem/utils/mechanics.py
 src/pyfem/utils/visualization.py
 src/pyfem/utils/wrappers.py
```

