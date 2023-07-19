# Comparing `tmp/upkie_description-1.3.0.tar.gz` & `tmp/upkie_description-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upkie_description-1.3.0.tar", last modified: Wed Apr  5 15:22:26 2023, max compression
+gzip compressed data, was "upkie_description-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `upkie_description-1.3.0.tar` & `upkie_description-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1350 2023-04-05 15:22:25.924849 upkie_description-1.3.0/README.md
--rw-r--r--   0        0        0     1332 2023-04-05 15:22:25.928849 upkie_description-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      892 2023-04-05 15:22:25.924849 upkie_description-1.3.0/upkie_description/__init__.py
--rw-r--r--   0        0        0     1774 2023-04-05 15:22:25.924849 upkie_description-1.3.0/upkie_description/load_in_pinocchio.py
--rw-r--r--   0        0        0   103184 2023-04-05 15:22:25.916849 upkie_description-1.3.0/upkie_description/meshes/ankle_stator.stl
--rw-r--r--   0        0        0   171484 2023-04-05 15:22:25.912850 upkie_description-1.3.0/upkie_description/meshes/handle.stl
--rw-r--r--   0        0        0   474984 2023-04-05 15:22:25.912850 upkie_description-1.3.0/upkie_description/meshes/hollow_leg/hollow_femur.stl
--rw-r--r--   0        0        0   162384 2023-04-05 15:22:25.912850 upkie_description-1.3.0/upkie_description/meshes/hollow_leg/hollow_hip.stl
--rw-r--r--   0        0        0   164484 2023-04-05 15:22:25.912850 upkie_description-1.3.0/upkie_description/meshes/hollow_leg/hollow_knee.stl
--rw-r--r--   0        0        0   185484 2023-04-05 15:22:25.916849 upkie_description-1.3.0/upkie_description/meshes/knee_stator.stl
--rw-r--r--   0        0        0      549 2023-04-05 15:22:25.912850 upkie_description-1.3.0/upkie_description/meshes/mjbots/README.md
--rw-r--r--   0        0        0  2811184 2023-04-05 15:22:25.916849 upkie_description-1.3.0/upkie_description/meshes/mjbots/mj5208_rotor.stl
--rw-r--r--   0        0        0  3597884 2023-04-05 15:22:25.916849 upkie_description-1.3.0/upkie_description/meshes/mjbots/mj5208_stator.stl
--rw-r--r--   0        0        0   134684 2023-04-05 15:22:25.916849 upkie_description-1.3.0/upkie_description/meshes/mjbots/qdd100_horn.stl
--rw-r--r--   0        0        0    51284 2023-04-05 15:22:25.912850 upkie_description-1.3.0/upkie_description/meshes/mjbots/qdd100_rotor.stl
--rw-r--r--   0        0        0   113184 2023-04-05 15:22:25.912850 upkie_description-1.3.0/upkie_description/meshes/mjbots/qdd100_stator.stl
--rw-r--r--   0        0        0    80284 2023-04-05 15:22:25.916849 upkie_description-1.3.0/upkie_description/meshes/wheel_hub.stl
--rw-r--r--   0        0        0      388 2023-04-05 15:22:25.920849 upkie_description-1.3.0/upkie_description/meshes/wheel_tire/README.md
--rw-r--r--   0        0        0  5848384 2023-04-05 15:22:25.920849 upkie_description-1.3.0/upkie_description/meshes/wheel_tire/wheel_tire.stl
--rw-r--r--   0        0        0     1003 2023-04-05 15:22:25.924849 upkie_description-1.3.0/upkie_description/paths.py
--rw-r--r--   0        0        0    43025 2023-04-05 15:22:25.924849 upkie_description-1.3.0/upkie_description/urdf/upkie.urdf
--rw-r--r--   0        0        0     2518 1970-01-01 00:00:00.000000 upkie_description-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1350 2023-07-19 08:39:33.837281 upkie_description-1.4.0/README.md
+-rw-r--r--   0        0        0     1332 2023-07-19 08:39:33.841281 upkie_description-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      892 2023-07-19 08:39:33.837281 upkie_description-1.4.0/upkie_description/__init__.py
+-rw-r--r--   0        0        0     1774 2023-07-19 08:39:33.837281 upkie_description-1.4.0/upkie_description/load_in_pinocchio.py
+-rw-r--r--   0        0        0   103184 2023-07-19 08:39:33.821282 upkie_description-1.4.0/upkie_description/meshes/ankle_stator.stl
+-rw-r--r--   0        0        0   171484 2023-07-19 08:39:33.821282 upkie_description-1.4.0/upkie_description/meshes/handle.stl
+-rw-r--r--   0        0        0   474984 2023-07-19 08:39:33.825281 upkie_description-1.4.0/upkie_description/meshes/hollow_leg/hollow_femur.stl
+-rw-r--r--   0        0        0   162384 2023-07-19 08:39:33.825281 upkie_description-1.4.0/upkie_description/meshes/hollow_leg/hollow_hip.stl
+-rw-r--r--   0        0        0   164484 2023-07-19 08:39:33.825281 upkie_description-1.4.0/upkie_description/meshes/hollow_leg/hollow_knee.stl
+-rw-r--r--   0        0        0   185484 2023-07-19 08:39:33.825281 upkie_description-1.4.0/upkie_description/meshes/knee_stator.stl
+-rw-r--r--   0        0        0      549 2023-07-19 08:39:33.825281 upkie_description-1.4.0/upkie_description/meshes/mjbots/README.md
+-rw-r--r--   0        0        0  2811184 2023-07-19 08:39:33.825281 upkie_description-1.4.0/upkie_description/meshes/mjbots/mj5208_rotor.stl
+-rw-r--r--   0        0        0  3597884 2023-07-19 08:39:33.829281 upkie_description-1.4.0/upkie_description/meshes/mjbots/mj5208_stator.stl
+-rw-r--r--   0        0        0   134684 2023-07-19 08:39:33.829281 upkie_description-1.4.0/upkie_description/meshes/mjbots/qdd100_horn.stl
+-rw-r--r--   0        0        0    51284 2023-07-19 08:39:33.829281 upkie_description-1.4.0/upkie_description/meshes/mjbots/qdd100_rotor.stl
+-rw-r--r--   0        0        0   113184 2023-07-19 08:39:33.829281 upkie_description-1.4.0/upkie_description/meshes/mjbots/qdd100_stator.stl
+-rw-r--r--   0        0        0    80284 2023-07-19 08:39:33.829281 upkie_description-1.4.0/upkie_description/meshes/wheel_hub.stl
+-rw-r--r--   0        0        0      388 2023-07-19 08:39:33.829281 upkie_description-1.4.0/upkie_description/meshes/wheel_tire/README.md
+-rw-r--r--   0        0        0  5848384 2023-07-19 08:39:33.833281 upkie_description-1.4.0/upkie_description/meshes/wheel_tire/wheel_tire.stl
+-rw-r--r--   0        0        0     1003 2023-07-19 08:39:33.837281 upkie_description-1.4.0/upkie_description/paths.py
+-rw-r--r--   0        0        0    43264 2023-07-19 08:39:33.837281 upkie_description-1.4.0/upkie_description/urdf/upkie.urdf
+-rw-r--r--   0        0        0     2518 1970-01-01 00:00:00.000000 upkie_description-1.4.0/PKG-INFO
```

### Comparing `upkie_description-1.3.0/README.md` & `upkie_description-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/pyproject.toml` & `upkie_description-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/__init__.py` & `upkie_description-1.4.0/upkie_description/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 URDF description for the Upkie wheeled biped.
 """
 
 from .load_in_pinocchio import load_in_pinocchio
 from .paths import meshes_path, path, urdf_path
 
-__version__ = "1.3.0"
+__version__ = "1.4.0"
 
 __all__ = [
     "load_in_pinocchio",
     "meshes_path",
     "path",
     "urdf_path",
 ]
```

### Comparing `upkie_description-1.3.0/upkie_description/load_in_pinocchio.py` & `upkie_description-1.4.0/upkie_description/load_in_pinocchio.py`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/ankle_stator.stl` & `upkie_description-1.4.0/upkie_description/meshes/ankle_stator.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/handle.stl` & `upkie_description-1.4.0/upkie_description/meshes/handle.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/hollow_leg/hollow_femur.stl` & `upkie_description-1.4.0/upkie_description/meshes/hollow_leg/hollow_femur.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/hollow_leg/hollow_hip.stl` & `upkie_description-1.4.0/upkie_description/meshes/hollow_leg/hollow_hip.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/hollow_leg/hollow_knee.stl` & `upkie_description-1.4.0/upkie_description/meshes/hollow_leg/hollow_knee.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/knee_stator.stl` & `upkie_description-1.4.0/upkie_description/meshes/knee_stator.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/mjbots/README.md` & `upkie_description-1.4.0/upkie_description/meshes/mjbots/README.md`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/mjbots/mj5208_rotor.stl` & `upkie_description-1.4.0/upkie_description/meshes/mjbots/mj5208_rotor.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/mjbots/mj5208_stator.stl` & `upkie_description-1.4.0/upkie_description/meshes/mjbots/mj5208_stator.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/mjbots/qdd100_horn.stl` & `upkie_description-1.4.0/upkie_description/meshes/mjbots/qdd100_horn.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/mjbots/qdd100_rotor.stl` & `upkie_description-1.4.0/upkie_description/meshes/mjbots/qdd100_rotor.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/mjbots/qdd100_stator.stl` & `upkie_description-1.4.0/upkie_description/meshes/mjbots/qdd100_stator.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/wheel_hub.stl` & `upkie_description-1.4.0/upkie_description/meshes/wheel_hub.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/meshes/wheel_tire/wheel_tire.stl` & `upkie_description-1.4.0/upkie_description/meshes/wheel_tire/wheel_tire.stl`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/paths.py` & `upkie_description-1.4.0/upkie_description/paths.py`

 * *Files identical despite different names*

### Comparing `upkie_description-1.3.0/upkie_description/urdf/upkie.urdf` & `upkie_description-1.4.0/upkie_description/urdf/upkie.urdf`

 * *Files 0% similar despite different names*

#### Comparing `upkie_description-1.3.0/upkie_description/urdf/upkie.urdf` & `upkie_description-1.4.0/upkie_description/urdf/upkie.urdf`

```diff
@@ -1,24 +1,28 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
 
 Copyright 2022 Stéphane Caron
+Copyright 2023 Inria
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
+-->
+<!--
+
 Conventions in this file:
 
 - Links and joints are grouped by "assemblies", for example "left_hip" or
   "right_knee". We can recognize assemblies in link and joint names.
 
 - A link is named "<assembly>_<identifier>", for example
   "left_hip_qdd100_stator" denotes the stator of the qdd100 of the left hip.
@@ -104,15 +108,15 @@
     <inertial>
       <mass value="0.001"/>
       <!-- ./box_inertia.py 0.001 0.01 0.01 0.01 -->
       <inertia ixx="1.6666666666666667e-08" ixy="0" ixz="0" iyx="0" iyy="1.6666666666666667e-08" iyz="0" izx="0" izy="0" izz="1.6666666666666667e-08"/>
     </inertial>
   </link>
   <joint name="imu_fix" type="fixed">
-    <origin rpy="3.141592653589793 0 0" xyz="0 0 0"/>
+    <origin rpy="3.141592653589793 0 3.141592653589793" xyz="0 0 0"/>
     <!-- no translation -->
     <parent link="base"/>
     <child link="imu"/>
   </joint>
   <!-- Torso -->
   <link name="torso">
     <visual>
@@ -241,15 +245,15 @@
   </link>
   <joint name="left_hip" type="revolute">
     <parent link="left_hip_qdd100_stator"/>
     <child link="left_hip_qdd100_rotor"/>
     <origin rpy="0 0 0" xyz="0 0 0.0292"/>
     <axis xyz="0 0 -1"/>
     <!-- search "moteus-direction-configuration" -->
-    <limit lower="-1.54" upper="1.54" velocity="12.0" effort="10.0"/>
+    <limit lower="-1.2566370614359172" upper="1.2566370614359172" velocity="12.566370614359172" effort="10.0"/>
   </joint>
   <link name="left_hip_horn">
     <visual>
       <geometry>
         <mesh filename="package://upkie_description/meshes/mjbots/qdd100_horn.stl"/>
       </geometry>
       <material name="black"/>
@@ -354,15 +358,15 @@
   </joint>
   <joint name="left_knee" type="revolute">
     <parent link="left_knee_qdd100_stator"/>
     <child link="left_knee_qdd100_rotor"/>
     <origin rpy="0 0 0" xyz="0 0 0.0292"/>
     <axis xyz="0 0 -1"/>
     <!-- search "moteus-direction-configuration" -->
-    <limit lower="-2.57" upper="2.57" velocity="12.0" effort="10.0"/>
+    <limit lower="-2.5132741228718345" upper="2.5132741228718345" velocity="12.566370614359172" effort="10.0"/>
   </joint>
   <link name="left_knee_qdd100_rotor">
     <visual>
       <geometry>
         <mesh filename="package://upkie_description/meshes/mjbots/qdd100_rotor.stl"/>
       </geometry>
       <material name="black"/>
@@ -533,15 +537,15 @@
   </link>
   <joint name="left_wheel" type="revolute">
     <parent link="left_ankle_mj5208_stator"/>
     <child link="left_ankle_mj5208_rotor"/>
     <origin rpy="0 0 0" xyz="0 0 0"/>
     <axis xyz="0 0 -1"/>
     <!-- search "moteus-direction-configuration" -->
-    <limit velocity="100.0" effort="1.0"/>
+    <limit velocity="50.26548245743669" effort="1.0"/>
   </joint>
   <!-- Left wheel -->
   <link name="left_wheel_hub">
     <visual>
       <geometry>
         <mesh filename="package://upkie_description/meshes/wheel_hub.stl"/>
       </geometry>
@@ -700,15 +704,15 @@
   </link>
   <joint name="right_hip" type="revolute">
     <parent link="right_hip_qdd100_stator"/>
     <child link="right_hip_qdd100_rotor"/>
     <origin rpy="0 0 0" xyz="0 0 0.0292"/>
     <axis xyz="0 0 -1"/>
     <!-- search "moteus-direction-configuration" -->
-    <limit lower="-1.54" upper="1.54" velocity="12.0" effort="10.0"/>
+    <limit lower="-1.2566370614359172" upper="1.2566370614359172" velocity="12.566370614359172" effort="10.0"/>
   </joint>
   <link name="right_hip_horn">
     <visual>
       <geometry>
         <mesh filename="package://upkie_description/meshes/mjbots/qdd100_horn.stl"/>
       </geometry>
       <material name="black"/>
@@ -813,15 +817,15 @@
   </joint>
   <joint name="right_knee" type="revolute">
     <parent link="right_knee_qdd100_stator"/>
     <child link="right_knee_qdd100_rotor"/>
     <origin rpy="0 0 0" xyz="0 0 0.0292"/>
     <axis xyz="0 0 -1"/>
     <!-- search "moteus-direction-configuration" -->
-    <limit lower="-2.57" upper="2.57" velocity="12.0" effort="10.0"/>
+    <limit lower="-2.5132741228718345" upper="2.5132741228718345" velocity="12.566370614359172" effort="10.0"/>
   </joint>
   <link name="right_knee_qdd100_rotor">
     <visual>
       <geometry>
         <mesh filename="package://upkie_description/meshes/mjbots/qdd100_rotor.stl"/>
       </geometry>
       <material name="black"/>
@@ -992,15 +996,15 @@
   </link>
   <joint name="right_wheel" type="revolute">
     <parent link="right_ankle_mj5208_stator"/>
     <child link="right_ankle_mj5208_rotor"/>
     <origin rpy="0 0 0" xyz="0 0 0"/>
     <axis xyz="0 0 -1"/>
     <!-- search "moteus-direction-configuration" -->
-    <limit velocity="100.0" effort="1.0"/>
+    <limit velocity="50.26548245743669" effort="1.0"/>
   </joint>
   <!-- Right wheel -->
   <link name="right_wheel_hub">
     <visual>
       <geometry>
         <mesh filename="package://upkie_description/meshes/wheel_hub.stl"/>
       </geometry>
```

### Comparing `upkie_description-1.3.0/PKG-INFO` & `upkie_description-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upkie_description
-Version: 1.3.0
+Version: 1.4.0
 Summary: URDF description for the Upkie wheeled biped.
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

