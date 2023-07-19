# Comparing `tmp/SiPMai-0.0.1.tar.gz` & `tmp/SiPMai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SiPMai-0.0.1.tar", last modified: Wed Jul 19 05:22:40 2023, max compression
+gzip compressed data, was "dist\SiPMai-0.0.2.tar", last modified: Wed Jul 19 15:14:42 2023, max compression
```

## Comparing `SiPMai-0.0.1.tar` & `SiPMai-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 05:22:40.752032 SiPMai-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-07-18 06:39:47.000000 SiPMai-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     4026 2023-07-19 05:22:40.750032 SiPMai-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3512 2023-07-19 03:28:17.000000 SiPMai-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 05:22:40.701080 SiPMai-0.0.1/SiPMai/
--rw-rw-rw-   0        0        0      107 2023-07-19 05:22:36.000000 SiPMai-0.0.1/SiPMai/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:22:40.719026 SiPMai-0.0.1/SiPMai/gen_data/
--rw-rw-rw-   0        0        0       53 2023-07-19 03:54:35.000000 SiPMai-0.0.1/SiPMai/gen_data/__init__.py
--rw-rw-rw-   0        0        0     4112 2023-07-18 05:43:11.000000 SiPMai-0.0.1/SiPMai/gen_data/compute_img.py
--rw-rw-rw-   0        0        0     6922 2023-07-19 05:15:03.000000 SiPMai-0.0.1/SiPMai/gen_data/gen_all_data_pipeline.py
--rw-rw-rw-   0        0        0     3498 2023-07-17 15:04:41.000000 SiPMai-0.0.1/SiPMai/gen_data/prepare_dataset.py
--rw-rw-rw-   0        0        0    10810 2023-07-19 02:41:42.000000 SiPMai-0.0.1/SiPMai/gen_data/ray_generation.py
--rw-rw-rw-   0        0        0    11749 2023-07-19 02:41:42.000000 SiPMai-0.0.1/SiPMai/gen_data/smi_molecule_simulation.py
--rw-rw-rw-   0        0        0     2896 2023-07-19 03:08:31.000000 SiPMai-0.0.1/SiPMai/gen_data/smile_generation.py
--rw-rw-rw-   0        0        0     2190 2023-07-18 03:59:34.000000 SiPMai-0.0.1/SiPMai/gen_data/util_fn.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:22:40.720032 SiPMai-0.0.1/SiPMai/smiles/
--rw-rw-rw-   0        0        0        0 2023-07-19 05:06:31.000000 SiPMai-0.0.1/SiPMai/smiles/__init__.py
--rw-rw-rw-   0        0        0 41963544 2023-07-17 10:17:15.000000 SiPMai-0.0.1/SiPMai/smiles/pubchem_39_200_100k.json
-drwxrwxrwx   0        0        0        0 2023-07-19 05:22:40.747030 SiPMai-0.0.1/SiPMai/unittest/
--rw-rw-rw-   0        0        0        0 2023-07-19 03:45:56.000000 SiPMai-0.0.1/SiPMai/unittest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:22:40.749030 SiPMai-0.0.1/SiPMai/utils/
--rw-rw-rw-   0        0        0        0 2023-07-18 03:21:53.000000 SiPMai-0.0.1/SiPMai/utils/__init__.py
--rw-rw-rw-   0        0        0     6543 2023-07-18 08:26:05.000000 SiPMai-0.0.1/SiPMai/utils/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:22:40.712194 SiPMai-0.0.1/SiPMai.egg-info/
--rw-rw-rw-   0        0        0     4026 2023-07-19 05:22:40.000000 SiPMai-0.0.1/SiPMai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      650 2023-07-19 05:22:40.000000 SiPMai-0.0.1/SiPMai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 05:22:40.000000 SiPMai-0.0.1/SiPMai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-07-19 05:22:40.000000 SiPMai-0.0.1/SiPMai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      150 2023-07-19 05:22:40.000000 SiPMai-0.0.1/SiPMai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-19 05:22:40.000000 SiPMai-0.0.1/SiPMai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 05:22:40.752032 SiPMai-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1815 2023-07-19 05:12:14.000000 SiPMai-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:14:42.010576 SiPMai-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-07-18 06:39:47.000000 SiPMai-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0     4026 2023-07-19 15:14:42.009593 SiPMai-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3512 2023-07-19 03:28:17.000000 SiPMai-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 15:14:41.920583 SiPMai-0.0.2/SiPMai/
+-rw-rw-rw-   0        0        0      107 2023-07-19 15:14:37.000000 SiPMai-0.0.2/SiPMai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:14:41.976795 SiPMai-0.0.2/SiPMai/gen_data/
+-rw-rw-rw-   0        0        0       53 2023-07-19 03:54:35.000000 SiPMai-0.0.2/SiPMai/gen_data/__init__.py
+-rw-rw-rw-   0        0        0     4633 2023-07-19 14:17:34.000000 SiPMai-0.0.2/SiPMai/gen_data/compute_img.py
+-rw-rw-rw-   0        0        0     7267 2023-07-19 15:13:17.000000 SiPMai-0.0.2/SiPMai/gen_data/gen_all_data_pipeline.py
+-rw-rw-rw-   0        0        0     3498 2023-07-17 15:04:41.000000 SiPMai-0.0.2/SiPMai/gen_data/prepare_dataset.py
+-rw-rw-rw-   0        0        0    10648 2023-07-19 14:45:55.000000 SiPMai-0.0.2/SiPMai/gen_data/ray_generation.py
+-rw-rw-rw-   0        0        0    11369 2023-07-19 10:21:20.000000 SiPMai-0.0.2/SiPMai/gen_data/smi_molecule_simulation.py
+-rw-rw-rw-   0        0        0     2896 2023-07-19 03:08:31.000000 SiPMai-0.0.2/SiPMai/gen_data/smile_generation.py
+-rw-rw-rw-   0        0        0     2190 2023-07-18 03:59:34.000000 SiPMai-0.0.2/SiPMai/gen_data/util_fn.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:14:41.977795 SiPMai-0.0.2/SiPMai/smiles/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:06:31.000000 SiPMai-0.0.2/SiPMai/smiles/__init__.py
+-rw-rw-rw-   0        0        0 41963544 2023-07-17 10:17:15.000000 SiPMai-0.0.2/SiPMai/smiles/pubchem_39_200_100k.json
+drwxrwxrwx   0        0        0        0 2023-07-19 15:14:42.006545 SiPMai-0.0.2/SiPMai/unittest/
+-rw-rw-rw-   0        0        0        0 2023-07-19 03:45:56.000000 SiPMai-0.0.2/SiPMai/unittest/__init__.py
+-rw-rw-rw-   0        0        0     2538 2023-07-19 07:42:46.000000 SiPMai-0.0.2/SiPMai/unittest/test_gen_data.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:14:42.008502 SiPMai-0.0.2/SiPMai/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-18 03:21:53.000000 SiPMai-0.0.2/SiPMai/utils/__init__.py
+-rw-rw-rw-   0        0        0     6543 2023-07-18 08:26:05.000000 SiPMai-0.0.2/SiPMai/utils/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:14:41.969889 SiPMai-0.0.2/SiPMai.egg-info/
+-rw-rw-rw-   0        0        0     4026 2023-07-19 15:14:41.000000 SiPMai-0.0.2/SiPMai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2023-07-19 15:14:41.000000 SiPMai-0.0.2/SiPMai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 15:14:41.000000 SiPMai-0.0.2/SiPMai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-07-19 15:14:41.000000 SiPMai-0.0.2/SiPMai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      150 2023-07-19 15:14:41.000000 SiPMai-0.0.2/SiPMai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-19 15:14:41.000000 SiPMai-0.0.2/SiPMai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 15:14:42.010576 SiPMai-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1815 2023-07-19 05:12:14.000000 SiPMai-0.0.2/setup.py
```

### Comparing `SiPMai-0.0.1/LICENSE.md` & `SiPMai-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.1/PKG-INFO` & `SiPMai-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiPMai
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Simple Yet Effective Scanning Tunnel Microscope Image Simulator
 Home-page: http://github.com/GilesLuo/SiPMai
 Author: Zhiyao Luo, Yaotian Yang, Jiali Li
 Author-email: zhiyao.luo@eng.ox.ac.uk
 License: MIT
 Project-URL: Source Code, https://github.com/my_username/my_package
 Keywords: Chemistry Simulation,STM Image Synthesis
```

### Comparing `SiPMai-0.0.1/README.md` & `SiPMai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.1/SiPMai/gen_data/gen_all_data_pipeline.py` & `SiPMai-0.0.2/SiPMai/gen_data/gen_all_data_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import json
 from typing import Dict
 
 
 def gen_all_data(smiles_file: str, num_mol: int, csv_file: str, min_atom: int, max_atom: int, num_cpus: int,
                  mol_save_dir: str,
                  resolution: int, blur_sigma: int, use_motion_blur: bool, use_gaussian_noise: bool,
-                 gen_original_img: bool, img_show: bool,
+                 gen_original_img: bool, gen_mol_drawing:bool, img_show: bool,
                  train_ratio: float, val_ratio: float, test_ratio: float, split_seed: int,
                  development: bool = False) -> None:
     """
     Generate all data required for the molecular images.
 
     Args:
         smiles_file (str): The path to the file containing SMILES strings.
@@ -43,76 +43,81 @@
         print("smiles generated")
 
     if not os.path.exists(smiles_file):
         raise FileNotFoundError(f"smiles file {smiles_file} not found, please generate smiles first.")
     else:
         with open(smiles_file, 'r') as f:
             smiles_dict: Dict = json.load(f)
-            num_mol = len(smiles_dict)
-            print(f"Found {num_mol} molecules!")
-            if num_mol > num_mol:
+            num_mol_ = len(smiles_dict)
+            print(f"Found {num_mol_} molecules!")
+            if num_mol_ > num_mol:
                 print(f"use the first {num_mol} molecules for later steps")
                 smiles_dict = {k: smiles_dict[k] for k in list(smiles_dict)[:num_mol]}
     if num_cpus == 0:
         num_cpus = os.cpu_count()
 
     ray_gen_main(smiles_dict, mol_save_dir,
-                 resolution, blur_sigma, use_motion_blur, use_gaussian_noise, gen_original_img,
-                 num_cpus, img_show)
+                 resolution, blur_sigma, use_motion_blur, use_gaussian_noise, gen_original_img, gen_mol_drawing,
+                 num_cpus, img_show, development)
     gen_index_main(mol_save_dir, train_ratio, val_ratio, test_ratio, split_seed)
 
 
 def main() -> None:
     """
     Main function that parses command line arguments and calls the gen_all function.
     """
     print("Start generating data with preset parameters (100k dataset with 39 <= num_atom <= 200)... ")
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--development", type=bool, default=False,
-                        help="Whether to run in development mode. Defaults to False.")
+                        help="Whether to run in development mode. Development mode will run ray locally with serial output."
+                             "Defaults to False.")
     # gen smiles args
     parser.add_argument("--smiles_file", type=str, default="pubchem_39_200_100k.json",
                         help="The path to the file containing SMILES strings.")
-    parser.add_argument("--num_mol", type=int, default=100000, help="The number of molecules to be generated.")
+    parser.add_argument("--num_mol", type=int, default=4, help="The number of molecules to be generated.")
     parser.add_argument("--csv_file", type=str, default="../CID-SMILES2.csv",
                         help="The path to the CSV file containing molecular data.")
     parser.add_argument("--min_atom", type=int, default=39, help="The minimum number of atoms for a molecule.")
     parser.add_argument("--max_atom", type=int, default=200, help="The maximum number of atoms for a molecule.")
 
     # gen ray args
-    cmd_dir = os.getcwd()
-    mol_save_dir = os.path.join(cmd_dir, "pubchem_39_200_100k")
-    print("mol_save_dir set to command execution dir: ", mol_save_dir)
-    parser.add_argument("--mol_save_dir", type=str, default=mol_save_dir,
+
+    parser.add_argument("--mol_save_dir", type=str, default="pubchem_39_200_100k",
                         help="The directory where the generated data should be saved.")
-    parser.add_argument("--resolution", type=int, default=256, help="The resolution of the generated images.")
-    parser.add_argument("--blur_sigma", type=int, default=24,
+
+    parser.add_argument("--resolution", type=int, default=512, help="The resolution of the generated images.")
+    parser.add_argument("--blur_sigma", type=int, default=34,
                         help="The sigma value for the Gaussian blur applied to the images.")
     parser.add_argument("--use_motion_blur", type=bool, default=False, help="Whether to use motion blur in the images.")
     parser.add_argument("--use_gaussian_noise", type=bool, default=False,
                         help="Whether to add Gaussian noise to the images.")
     parser.add_argument("--gen_original_img", type=bool, default=True, help="Whether to generate original images.")
+    parser.add_argument("--gen_mol_drawing", type=bool, default=True, help="Whether to generate mol images for eye inspection.")
     parser.add_argument("--num_cpus", type=int, default=4, help="The number of CPUs to be used for data generation.")
     parser.add_argument("--show", type=bool, default=False, help="Whether to display the generated images.")
 
     # data indices args
     parser.add_argument("--split_seed", type=int, default=1, help="The seed for the random splitting of data.")
     parser.add_argument("--train_ratio", type=float, default=0.8, help="The ratio of data to be used for training.")
     parser.add_argument("--val_ratio", type=float, default=0.1, help="The ratio of data to be used for validation.")
     parser.add_argument("--test_ratio", type=float, default=0.1, help="The ratio of data to be used for testing.")
     args = parser.parse_args()
 
     from pkg_resources import resource_filename
     args.smiles_file = resource_filename('SiPMai', f'smiles/{args.smiles_file}')
+    cmd_dir = os.getcwd()
+    args.mol_save_dir = os.path.join(cmd_dir, args.mol_save_dir)
+    print("mol_save_dir set to command execution dir: ", args.mol_save_dir)
     gen_all_data(smiles_file=args.smiles_file, num_mol=args.num_mol, csv_file=args.csv_file, min_atom=args.min_atom,
                  max_atom=args.max_atom, num_cpus=args.num_cpus, mol_save_dir=args.mol_save_dir,
                  resolution=args.resolution, blur_sigma=args.blur_sigma, use_motion_blur=args.use_motion_blur,
-                 use_gaussian_noise=args.use_gaussian_noise, gen_original_img=args.gen_original_img, img_show=False,
+                 use_gaussian_noise=args.use_gaussian_noise, gen_original_img=args.gen_original_img, gen_mol_drawing=args.gen_mol_drawing,
+                 img_show=False,
                  train_ratio=args.train_ratio, val_ratio=args.val_ratio, test_ratio=args.test_ratio,
                  split_seed=args.split_seed,
                  development=args.development)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `SiPMai-0.0.1/SiPMai/gen_data/prepare_dataset.py` & `SiPMai-0.0.2/SiPMai/gen_data/prepare_dataset.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.1/SiPMai/gen_data/ray_generation.py` & `SiPMai-0.0.2/SiPMai/gen_data/smi_molecule_simulation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+import warnings
 import os
 import json
-
-import ray
 from tqdm import tqdm
-import time
 from rdkit import Chem
 from rdkit.Chem import Draw
-from SiPMai.gen_data.util_fn import uniform_noise, motion_blur, compress_binary_arr
+from SiPMai.gen_data.util_fn import uniform_noise, motion_blur, compress_binary_arr, decompress_binary_arr
 from matplotlib import pyplot as plt
 from PIL import Image
 import numpy as np
-from SiPMai.gen_data.compute_img import cal_atom_projection, bond_location_cal
 from scipy.ndimage import gaussian_filter
+from SiPMai.gen_data.compute_img import cal_atom_projection, bond_location_cal
+if not "ENABLE_MAYAVI" in globals():
+    try:
+        from mayavi import mlab
+
+        ENABLE_MAYAVI = True
+    except ImportError as e:
+        ENABLE_MAYAVI = False
+        warnings.warn("mayavi not found, this will not hinder data generation. "
+                      "If img_show is needed, please install mayavi")
 
-ENABLE_MAYAVI = False
-
-
-@ray.remote
 def points_height_matrix(smi: str, molecule_name: int, resolution: int, info_dir, json_dir, img_dir,
-                         blur_sigma, use_motion_blur, use_gaussian_noise, gen_original_img=True,
+                         blur_sigma, use_motion_blur, use_gaussian_noise,
                          show=False):
     """
     generate 5 files for each molecule:
     1. img_dir/img.png:                 the image of the molecule with gaussian noise (for simulating electron cloud)
     2. img_dir/orig_img.png:            the image of the molecule without noise, calculated from the 2D coordinates
     3. info_dir/points_info.npz:   -- atom instance binary array, shape: (num_atom, resolution, resolution)
                                          -- bond instance binary array, shape: (num_bond, resolution, resolution)
@@ -33,21 +36,18 @@
     """
     img_name = os.path.join(img_dir, str(molecule_name) + '_img.png')
     orig_img_name = os.path.join(img_dir, str(molecule_name) + '_orig_img.png')
     points_info_name = os.path.join(info_dir, str(molecule_name) + '_points_info.npz')
     drawing_name = os.path.join(info_dir, str(molecule_name) + '_mol_drawing.png')
     json_name = os.path.join(json_dir, str(molecule_name) + '.json')
 
-    if show:
-        raise NotImplementedError("show is not implemented for ray version")
-
     # check done
     if os.path.exists(points_info_name) and os.path.exists(img_name) and os.path.exists(
             orig_img_name) and os.path.exists(
-        drawing_name) and os.path.exists(json_name):
+            drawing_name) and os.path.exists(json_name):
         print(f"molecule {molecule_name} exists, skip")
         return True
 
     #         2D molecules were converted into 3D structures,
     #         and mechanical functions were used for Angle correction and optimization
     smile_dict = {}
     mol_2D = Chem.MolFromSmiles(smi)
@@ -74,50 +74,67 @@
         if atom_symbol in atom_radius.keys():
             x.append(atom_radius[atom_symbol])
         else:
             raise NotImplementedError("only support C, H, O, S, N, P, Cl")
         x.append(mol_2D_H.GetAtomWithIdx(s).GetIdx())
         atom_position.append(x)
     Draw.MolToFile(mol_2D_H, drawing_name, size=(600, 600))
+    # 在三维坐标系绘制得到的原子坐标，可通过原子坐标调整三维坐标轴大小
+    if show and ENABLE_MAYAVI:
+        plt.figure()  # 得到画面
+        ax1 = plt.axes(projection='3d')
+        ax1.set_xlim(0, 10)  # X轴，横向向右方向
+        ax1.set_ylim(10, 0)  # Y轴,左向与X,Z轴互为垂直
+        ax1.set_zlim(0, 10)  # 竖向为Z轴
+        # color1 = ['r', 'g', 'b', 'k', 'm']
+        # marker1 = ['o', 'v', '1', 's', 'H']
+        for x in atom_position:
+            ax1.scatter(x[0], x[1], x[2], c='r', marker='o', linewidths=4)
+        plt.show()
 
     points = np.array(atom_position)
+
+    # 计算基平面上的投影的x，y的坐标范围，确定生成的坐标点阵的区域
     x, y, z, r = points[:, 0], points[:, 1], points[:, 2], points[:, 3]
     r_max = max(r)
     x_max, x_min, y_max, y_min = int(max(x) + r_max) + 1, int(min(x) - r_max) - 1, int(max(y) + r_max) + 1, int(
         min(y) - r_max) - 1
-    z_min = int(min(z) - r_max) - 1
+    z_min = int(min(z) - r_max) - 1  # 方便后续对基平面进行平移操作
+
+    # Draw a scale model of a 3D molecule (stacked ball model)
+    if show and ENABLE_MAYAVI:
+        mlab.points3d(x, y, z, r * 2, scale_factor=1, resolution=30, mode="sphere")
+        mlab.outline()
+        mlab.axes()
+        mlab.show()
+
 
-    # Build the matrix to start recording the height
-    points_initial = np.zeros([resolution, resolution])  # initialize
-    points_class = np.zeros([resolution, resolution])
     # Initializes the bool matrix that stores the atoms
-    points_bool = np.zeros([atom_num, resolution, resolution])
     points_bond_bool = np.zeros([bond_num, resolution, resolution])
+
+    # create coordinate mesh
     x_axes = np.linspace(x_min, x_max, resolution)
     y_axes = np.linspace(y_min, y_max, resolution)
     X, Y = np.meshgrid(x_axes, y_axes)
     coordinate_points = np.array([X.ravel(), Y.ravel()])
     coordinate_points_array = coordinate_points.T
     coordinate_points_array = np.array(coordinate_points_array).reshape((resolution, resolution, 2))
 
     '''
     Start to calculate the height of each atom in the molecule from the base plane. At this time, 
     the base plane is set as the xoy plane, and the virtual projection is made from top to bottom through 
     the point light source cluster, that is, the height of the highest atom contacted is taken as the height recorded
     '''
-    points_initial, points_bool, points_class = cal_atom_projection(atom_position, coordinate_points_array,
-                                                                    resolution,
-                                                                    points_bool,
-                                                                    points_initial, points_class, atom_class, z_min)
+    points_initial, points_bool, points_class = cal_atom_projection(np.array(atom_position), coordinate_points_array,
+                                                                    resolution,  atom_class, z_min)
     points_class = np.where(points_class == 0, 255, points_class)
-
-    if gen_original_img:
-        im = Image.fromarray(points_class[::-1, :])
-        im = im.convert('L')
-        im.save(orig_img_name)
+    # attention! 图像坐标系的原点通常是左上角，而数组的索引是从左到右、从上到下的。因此，在将 NumPy 数组转换为 Pillow 图像对象时，需要将数组进行翻转，使其与图像坐标系保持一致。可以使用以下代码进行翻转：
+    im = Image.fromarray(points_class[::-1, :])
+    im = im.convert('L')
+    im.save(orig_img_name)
 
     # get blurred image
     points_initial = gaussian_filter(points_initial, sigma=blur_sigma)
     if use_motion_blur:
         points_initial = motion_blur(points_initial)
     if use_gaussian_noise:
         points_initial = uniform_noise(points_initial)
@@ -128,14 +145,15 @@
     plt.gca().xaxis.set_major_locator(plt.NullLocator())
     plt.gca().yaxis.set_major_locator(plt.NullLocator())
     plt.subplots_adjust(top=1, bottom=0, right=1, left=0, hspace=0, wspace=0)
     plt.margins(0, 0)
     fig.savefig(img_name, format='png')
     plt.close()
 
+    # todo: calculate per pixel label of each bond in the image
     bond_list = [[] for i in range(bond_num)]
     molecule_adjacent_matrix = np.zeros((atom_num, atom_num), dtype=np.bool_)
     bond_record_dic = {}
     bonds = mol_2D_H.GetBonds()  # To traverse the key
     for bond_i in range(bond_num):
         bond_list[bond_i].append(bonds[bond_i].GetIdx())
         atom_begin_index = bonds[bond_i].GetBeginAtomIdx()
@@ -162,65 +180,50 @@
 
     np.savez_compressed(points_info_name,
                         arr_atom=arr_atom_compressed, arr_bond=arr_bond_compressed, adj_matrix=adj_matrix_compressed,
                         arr_atom_shape=arr_atom.shape, arr_bond_shape=arr_bond.shape,
                         adj_shape=molecule_adjacent_matrix.shape,
                         molecule_points_height=points_initial)
 
+    # turn on debug mode to check compression
+    arr_atom_, arr_bond_, adj, points_initial_ = decompress_binary_arr(points_info_name)
+    assert np.array_equal(arr_atom, arr_atom_)
+    assert np.array_equal(arr_bond, arr_bond_)
+    assert np.array_equal(adj, molecule_adjacent_matrix)
+    assert np.array_equal(points_initial, points_initial_)
+
     json_information = [bond_record_dic, smile_dict]
     with open(json_name, 'w', encoding='utf-8') as f:
         json.dump(json_information, f)
     return True
 
 
-def ray_gen_main(mol_dict, save_dir, resolution, blur_sigma, use_motion_blur, use_gaussian_noise, gen_original_img,
-                 num_cpu=None, show=False):
-    ray.init(num_cpus=num_cpu)
-
-    # prepare folders
-    info_dir = os.path.join(save_dir, "info")
-    json_dir = os.path.join(save_dir, "json")
-    img_dir = os.path.join(save_dir, "img")
-    os.makedirs(info_dir, exist_ok=True)
-    os.makedirs(json_dir, exist_ok=True)
-    os.makedirs(img_dir, exist_ok=True)
-
-    tasks = {}
-    for mol, smiles in mol_dict.items():
-        task_id = points_height_matrix.remote(smiles, mol, resolution, info_dir, json_dir, img_dir,
-                                              blur_sigma, use_motion_blur, use_gaussian_noise, gen_original_img, show)
-        tasks[task_id] = mol
-
-    pbar = tqdm(total=len(tasks), desc="Processing tasks")
-    while len(tasks):
-        done_ids, _ = ray.wait(list(tasks.keys()), num_returns=1)
-        for ready_id in done_ids:
-            try:
-                result = ray.get(ready_id)
-                molecule_name = tasks.pop(ready_id)
-                pbar.set_description(molecule_name)
-                pbar.update()
-            except ray.exceptions.RayTaskError as ex:
-                print(f"Task failed for molecule {tasks[ready_id]} with error: {ex}")
-        time.sleep(0.5)  # To avoid busy waiting
-
-    pbar.close()
-    ray.shutdown()
-
-
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--smiles_file", type=str, default="../data/pubchem_smiles.json")
     parser.add_argument("--save_dir", type=str, default="../data")
     parser.add_argument("--resolution", type=int, default=256)
     parser.add_argument("--blur_sigma", type=int, default=24)
     parser.add_argument("--use_motion_blur", type=bool, default=False)
     parser.add_argument("--use_gaussian_noise", type=bool, default=False)
     parser.add_argument("--show", type=bool, default=False)
     args = parser.parse_args()
+
+    # start generation
     with open(args.smiles_file, 'r') as f:
         mol_dict = json.load(f)
-    # start generation
-    ray_gen_main(mol_dict, args.save_dir,
-                 args.resolution, args.blur_sigma, args.use_motion_blur, args.use_gaussian_noise, args.show)
+
+    # prepare folders
+    info_dir = os.path.join(args.save_dir, "info")
+    json_dir = os.path.join(args.save_dir, "json")
+    img_dir = os.path.join(args.save_dir, "img")
+    os.makedirs(info_dir, exist_ok=True)
+    os.makedirs(json_dir, exist_ok=True)
+    os.makedirs(img_dir, exist_ok=True)
+
+    pbar = tqdm(total=len(mol_dict), desc="Generating molecules")
+    for mol, smiles in mol_dict.items():
+        task_id = points_height_matrix(smiles, mol, args.resolution, info_dir, json_dir, img_dir,
+                                       args.blur_sigma, args.use_motion_blur, args.use_gaussian_noise, args.show)
+        pbar.update()
```

### Comparing `SiPMai-0.0.1/SiPMai/gen_data/smi_molecule_simulation.py` & `SiPMai-0.0.2/SiPMai/gen_data/ray_generation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,232 +1,228 @@
-import warnings
 import os
 import json
+
+import ray
 from tqdm import tqdm
+import time
 from rdkit import Chem
 from rdkit.Chem import Draw
-from SiPMai.gen_data.util_fn import uniform_noise, motion_blur, compress_binary_arr, decompress_binary_arr
+from SiPMai.gen_data.util_fn import uniform_noise, motion_blur, compress_binary_arr
 from matplotlib import pyplot as plt
 from PIL import Image
 import numpy as np
-from scipy.ndimage import gaussian_filter
 from SiPMai.gen_data.compute_img import cal_atom_projection, bond_location_cal
-if not "ENABLE_MAYAVI" in globals():
-    try:
-        from mayavi import mlab
+from scipy.ndimage import gaussian_filter
+
+ENABLE_MAYAVI = False
 
-        ENABLE_MAYAVI = True
-    except ImportError as e:
-        ENABLE_MAYAVI = False
-        warnings.warn("mayavi not found, this will not hinder data generation. "
-                      "If img_show is needed, please install mayavi")
 
+@ray.remote
 def points_height_matrix(smi: str, molecule_name: int, resolution: int, info_dir, json_dir, img_dir,
                          blur_sigma, use_motion_blur, use_gaussian_noise,
+                         gen_original_img, gen_mol_drawing,
                          show=False):
     """
     generate 5 files for each molecule:
     1. img_dir/img.png:                 the image of the molecule with gaussian noise (for simulating electron cloud)
-    2. img_dir/orig_img.png:            the image of the molecule without noise, calculated from the 2D coordinates
+    2. img_dir/orig_img.png:            binary image of the molecule (only for human inspection)
     3. info_dir/points_info.npz:   -- atom instance binary array, shape: (num_atom, resolution, resolution)
                                          -- bond instance binary array, shape: (num_bond, resolution, resolution)
                                          -- adjacency matrix, shape: (num_atom, num_atom)
                                          -- point height array, shape: (resolution, resolution)
     4. info_dir/mol_drawing.png   a molecule image (only for human inspection)
     5. json_dir/.json                   json file containing the SMILES string and other useful information
     """
     img_name = os.path.join(img_dir, str(molecule_name) + '_img.png')
     orig_img_name = os.path.join(img_dir, str(molecule_name) + '_orig_img.png')
     points_info_name = os.path.join(info_dir, str(molecule_name) + '_points_info.npz')
     drawing_name = os.path.join(info_dir, str(molecule_name) + '_mol_drawing.png')
     json_name = os.path.join(json_dir, str(molecule_name) + '.json')
 
+    if show:
+        raise NotImplementedError("show is not implemented for ray version")
+
     # check done
     if os.path.exists(points_info_name) and os.path.exists(img_name) and os.path.exists(
             orig_img_name) and os.path.exists(
-            drawing_name) and os.path.exists(json_name):
+        drawing_name) and os.path.exists(json_name):
         print(f"molecule {molecule_name} exists, skip")
         return True
 
     #         2D molecules were converted into 3D structures,
     #         and mechanical functions were used for Angle correction and optimization
-    smile_dict = {}
     mol_2D = Chem.MolFromSmiles(smi)
-    smile_dict['smile'] = smi
     mol_2D_H = Chem.AddHs(mol_2D)
     atom_num = mol_2D_H.GetNumAtoms()
     bond_num = mol_2D_H.GetNumBonds()
 
     moleblock_2D = Chem.MolToMolBlock(mol_2D_H)  # Returns the two-dimensional coordinates of the atoms in the molecule
     if show:
         mol_3D = Chem.MolFromSmiles(smi)
         Draw.ShowMol(mol_3D, size=(550, 550), kekulize=False)
         Draw.ShowMol(mol_2D_H, size=(550, 550), kekulize=False)
     mol_2D_H = Chem.MolFromMolBlock(moleblock_2D, removeHs=False)
     conf = mol_2D_H.GetConformer()
 
-    atom_position = []
+    atom_position = np.zeros((atom_num, 5), dtype=np.float32)
     atom_radius = {'C': 0.77, 'H': 0.37, 'O': 0.73, 'S': 1.02, 'N': 0.75, 'P': 1.06, 'Cl': 0.99}
-    atom_class = {'0.77': 1, '0.37': 2, '0.73': 3, '1.02': 4, '0.75': 5, '1.06': 6, '0.99': 7}
     for s in range(atom_num):
-        x = list(conf.GetAtomPosition(s))
-        mol_2D_H.GetAtomWithIdx(s).SetProp('molAtomMapNumber', str(mol_2D_H.GetAtomWithIdx(s).GetIdx()))  # 对原子进行索引
+        mol_2D_H.GetAtomWithIdx(s).SetProp('molAtomMapNumber', str(mol_2D_H.GetAtomWithIdx(s).GetIdx()))
         atom_symbol = mol_2D_H.GetAtoms()[s].GetSymbol()
+        # get x, y, z, r
         if atom_symbol in atom_radius.keys():
-            x.append(atom_radius[atom_symbol])
+            atom_position[s, 3] = atom_radius[atom_symbol]
         else:
             raise NotImplementedError("only support C, H, O, S, N, P, Cl")
-        x.append(mol_2D_H.GetAtomWithIdx(s).GetIdx())
-        atom_position.append(x)
-    Draw.MolToFile(mol_2D_H, drawing_name, size=(600, 600))
-    # 在三维坐标系绘制得到的原子坐标，可通过原子坐标调整三维坐标轴大小
-    if show and ENABLE_MAYAVI:
-        plt.figure()  # 得到画面
-        ax1 = plt.axes(projection='3d')
-        ax1.set_xlim(0, 10)  # X轴，横向向右方向
-        ax1.set_ylim(10, 0)  # Y轴,左向与X,Z轴互为垂直
-        ax1.set_zlim(0, 10)  # 竖向为Z轴
-        # color1 = ['r', 'g', 'b', 'k', 'm']
-        # marker1 = ['o', 'v', '1', 's', 'H']
-        for x in atom_position:
-            ax1.scatter(x[0], x[1], x[2], c='r', marker='o', linewidths=4)
-        plt.show()
-
-    points = np.array(atom_position)
-
-    # 计算基平面上的投影的x，y的坐标范围，确定生成的坐标点阵的区域
-    x, y, z, r = points[:, 0], points[:, 1], points[:, 2], points[:, 3]
-    r_max = max(r)
-    x_max, x_min, y_max, y_min = int(max(x) + r_max) + 1, int(min(x) - r_max) - 1, int(max(y) + r_max) + 1, int(
-        min(y) - r_max) - 1
-    z_min = int(min(z) - r_max) - 1  # 方便后续对基平面进行平移操作
-
-    # Draw a scale model of a 3D molecule (stacked ball model)
-    if show and ENABLE_MAYAVI:
-        mlab.points3d(x, y, z, r * 2, scale_factor=1, resolution=30, mode="sphere")
-        mlab.outline()
-        mlab.axes()
-        mlab.show()
-
-    # Build the matrix to start recording the height
-    points_initial = np.zeros([resolution, resolution])  # initialize
-    points_class = np.zeros([resolution, resolution])
-    # Initializes the bool matrix that stores the atoms
-    points_bool = np.zeros([atom_num, resolution, resolution])
-    points_bond_bool = np.zeros([bond_num, resolution, resolution])
+        atom_position[s, :3] = list(conf.GetAtomPosition(s))
+        atom_position[s, 4] = mol_2D_H.GetAtomWithIdx(s).GetIdx()  # atom index
+
+    # save drawing
+    if gen_mol_drawing:
+        Draw.MolToFile(mol_2D_H, drawing_name, size=(600, 600))
+
+    # get image boundaries
+    x, y, z, r = atom_position[:, 0], atom_position[:, 1], atom_position[:, 2], atom_position[:, 3]
+    r_max = r.max()
+    x_max, x_min, y_max, y_min = int(x.max() + r_max) + 1, int(x.min() - r_max) - 1, int(y.max() + r_max) + 1, int(
+        y.min() - r_max) - 1
+    z_min = int(z.min() - r_max) - 1  # doesn't really matter
+
+    # get x, y mesh
+    points_bond_bool = np.zeros([bond_num, resolution, resolution], dtype=bool)
     x_axes = np.linspace(x_min, x_max, resolution)
     y_axes = np.linspace(y_min, y_max, resolution)
     X, Y = np.meshgrid(x_axes, y_axes)
     coordinate_points = np.array([X.ravel(), Y.ravel()])
-    coordinate_points_array = coordinate_points.T
-    coordinate_points_array = np.array(coordinate_points_array).reshape((resolution, resolution, 2))
+    mesh = coordinate_points.T
+    mesh = np.array(mesh).reshape((resolution, resolution, 2))
 
     '''
     Start to calculate the height of each atom in the molecule from the base plane. At this time, 
     the base plane is set as the xoy plane, and the virtual projection is made from top to bottom through 
     the point light source cluster, that is, the height of the highest atom contacted is taken as the height recorded
     '''
-    points_initial, points_bool, points_class = cal_atom_projection(atom_position, coordinate_points_array,
-                                                                    resolution,
-                                                                    points_bool,
-                                                                    points_initial, points_class, atom_class, z_min)
-    points_class = np.where(points_class == 0, 255, points_class)
-    # attention! 图像坐标系的原点通常是左上角，而数组的索引是从左到右、从上到下的。因此，在将 NumPy 数组转换为 Pillow 图像对象时，需要将数组进行翻转，使其与图像坐标系保持一致。可以使用以下代码进行翻转：
-    im = Image.fromarray(points_class[::-1, :])
-    im = im.convert('L')
-    im.save(orig_img_name)
+    height_mesh, atom_mask, is_coincide = cal_atom_projection(atom_position, mesh, z_min)
+    # if is_coincide.any():
+    #     raise ValueError("atom coincide")
+    if gen_original_img:
+        orig_arr = atom_mask.sum(axis=0)
+        orig_arr[orig_arr > 0] = 255
+        im = Image.fromarray(orig_arr[::-1, :])
+        im = im.convert('L')
+        im.save(orig_img_name)
 
     # get blurred image
-    points_initial = gaussian_filter(points_initial, sigma=blur_sigma)
+    height_mesh = gaussian_filter(height_mesh, sigma=blur_sigma)
     if use_motion_blur:
-        points_initial = motion_blur(points_initial)
+        height_mesh = motion_blur(height_mesh)
     if use_gaussian_noise:
-        points_initial = uniform_noise(points_initial)
+        height_mesh = uniform_noise(height_mesh)
     plt.figure(figsize=(resolution, resolution), dpi=1)
-    plt.imshow(points_initial, cmap='gray', origin='lower')
+    plt.imshow(height_mesh, cmap='gray', origin='lower')
     plt.axis('off')
     fig = plt.gcf()
     plt.gca().xaxis.set_major_locator(plt.NullLocator())
     plt.gca().yaxis.set_major_locator(plt.NullLocator())
     plt.subplots_adjust(top=1, bottom=0, right=1, left=0, hspace=0, wspace=0)
     plt.margins(0, 0)
     fig.savefig(img_name, format='png')
     plt.close()
 
-    # todo: calculate per pixel label of each bond in the image
-    bond_list = [[] for i in range(bond_num)]
+    # get adjacent matrix
+    bonds = mol_2D_H.GetBonds()  # To traverse the key
     molecule_adjacent_matrix = np.zeros((atom_num, atom_num), dtype=np.bool_)
     bond_record_dic = {}
-    bonds = mol_2D_H.GetBonds()  # To traverse the key
-    for bond_i in range(bond_num):
-        bond_list[bond_i].append(bonds[bond_i].GetIdx())
-        atom_begin_index = bonds[bond_i].GetBeginAtomIdx()
-        atom_end_index = bonds[bond_i].GetEndAtomIdx()
-        bond_record_dic[f'bond-{bond_i}'] = str(atom_begin_index) + str(atom_end_index)
-        molecule_adjacent_matrix[atom_begin_index][atom_end_index] = 1
-        molecule_adjacent_matrix[atom_end_index][atom_begin_index] = 1
-        for t in atom_position:
-            if t[4] == atom_begin_index or t[4] == atom_end_index:
-                bond_list[bond_i].append(t[0])
-                bond_list[bond_i].append(t[1])
-                bond_list[bond_i].append(t[3])
+    bond_list = [[bond.GetIdx()] for bond in bonds]
 
-    points_bond_bool = bond_location_cal(bond_list, coordinate_points_array, points_bond_bool, resolution)
+    for bond_i, bond in enumerate(bonds):
+        atom_begin_index = bond.GetBeginAtomIdx()
+        atom_end_index = bond.GetEndAtomIdx()
+        bond_key = f"{atom_begin_index}-{atom_end_index}"
+        bond_record_dic[bond_key] = bond_i
+        molecule_adjacent_matrix[atom_begin_index, atom_end_index] = 1
+        molecule_adjacent_matrix[atom_end_index, atom_begin_index] = 1
+
+        matching_positions = atom_position[
+            (atom_position[:, 4] == atom_begin_index) | (atom_position[:, 4] == atom_end_index)]
+        bond_list[bond_i].extend(matching_positions[:, [0, 1, 3]].ravel().tolist())
+
+    # get bond mask in the image
+    points_bond_bool = bond_location_cal(bond_list, mesh, points_bond_bool, resolution)
 
     # save np.array
 
-    arr_atom = np.array(points_bool, dtype=bool)
+    arr_atom = np.array(atom_mask, dtype=bool)
     arr_bond = np.array(points_bond_bool, dtype=bool)
 
     arr_atom_compressed = compress_binary_arr(arr_atom)
     arr_bond_compressed = compress_binary_arr(arr_bond)
     adj_matrix_compressed = compress_binary_arr(molecule_adjacent_matrix)
 
     np.savez_compressed(points_info_name,
                         arr_atom=arr_atom_compressed, arr_bond=arr_bond_compressed, adj_matrix=adj_matrix_compressed,
                         arr_atom_shape=arr_atom.shape, arr_bond_shape=arr_bond.shape,
                         adj_shape=molecule_adjacent_matrix.shape,
-                        molecule_points_height=points_initial)
-
-    # turn on debug mode to check compression
-    arr_atom_, arr_bond_, adj, points_initial_ = decompress_binary_arr(points_info_name)
-    assert np.array_equal(arr_atom, arr_atom_)
-    assert np.array_equal(arr_bond, arr_bond_)
-    assert np.array_equal(adj, molecule_adjacent_matrix)
-    assert np.array_equal(points_initial, points_initial_)
-
-    json_information = [bond_record_dic, smile_dict]
-    with open(json_name, 'w', encoding='utf-8') as f:
-        json.dump(json_information, f)
+                        molecule_points_height=height_mesh)
+    try:
+        with open(json_name, 'w', encoding='utf-8') as f:
+            json.dump({"bond_dict": bond_record_dic, "smiles": smi}, f)
+    except Exception as e:
+        # to avoid the error of json.dump, remove the file if an exception occurs
+        os.remove(json_name)
+        raise ValueError("something wrong with json.dump. Json file removed to avoid saving broken files")
     return True
 
 
+def ray_gen_main(mol_dict, save_dir, resolution, blur_sigma, use_motion_blur, use_gaussian_noise, gen_original_img=False, gen_mol_drawing=False,
+                 num_cpu=None, show=False, debug_mode=False):
+    ray.init(num_cpus=num_cpu, local_mode=debug_mode)
+
+    # prepare folders
+    info_dir = os.path.join(save_dir, "info")
+    json_dir = os.path.join(save_dir, "json")
+    img_dir = os.path.join(save_dir, "img")
+    os.makedirs(info_dir, exist_ok=True)
+    os.makedirs(json_dir, exist_ok=True)
+    os.makedirs(img_dir, exist_ok=True)
+
+    tasks = {}
+    for mol, smiles in mol_dict.items():
+        task_id = points_height_matrix.remote(smiles, mol, resolution, info_dir, json_dir, img_dir,
+                                              blur_sigma, use_motion_blur, use_gaussian_noise,
+                                              gen_original_img, gen_mol_drawing, show)
+        tasks[task_id] = mol
+
+    pbar = tqdm(total=len(tasks), desc="Processing tasks")
+    while len(tasks):
+        done_ids, _ = ray.wait(list(tasks.keys()), num_returns=1)
+        for ready_id in done_ids:
+            try:
+                result = ray.get(ready_id)
+                molecule_name = tasks.pop(ready_id)
+                pbar.set_description(molecule_name)
+                pbar.update()
+            except ray.exceptions.RayTaskError as ex:
+                print(f"Task failed for molecule {tasks[ready_id]} with error: {ex}")
+        time.sleep(0.5)  # To avoid busy waiting
+
+    pbar.close()
+    ray.shutdown()
+
+
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser()
-    parser.add_argument("--smiles_file", type=str, default="../data/pubchem_smiles.json")
+    parser.add_argument("--smiles_file", type=str, default="../smiles/pubchem_39_200_100k.json")
     parser.add_argument("--save_dir", type=str, default="../data")
     parser.add_argument("--resolution", type=int, default=256)
     parser.add_argument("--blur_sigma", type=int, default=24)
     parser.add_argument("--use_motion_blur", type=bool, default=False)
     parser.add_argument("--use_gaussian_noise", type=bool, default=False)
     parser.add_argument("--show", type=bool, default=False)
     args = parser.parse_args()
-
-    # start generation
     with open(args.smiles_file, 'r') as f:
         mol_dict = json.load(f)
-
-    # prepare folders
-    info_dir = os.path.join(args.save_dir, "info")
-    json_dir = os.path.join(args.save_dir, "json")
-    img_dir = os.path.join(args.save_dir, "img")
-    os.makedirs(info_dir, exist_ok=True)
-    os.makedirs(json_dir, exist_ok=True)
-    os.makedirs(img_dir, exist_ok=True)
-
-    pbar = tqdm(total=len(mol_dict), desc="Generating molecules")
-    for mol, smiles in mol_dict.items():
-        task_id = points_height_matrix(smiles, mol, args.resolution, info_dir, json_dir, img_dir,
-                                       args.blur_sigma, args.use_motion_blur, args.use_gaussian_noise, args.show)
-        pbar.update()
+    # start generation
+    ray_gen_main(mol_dict, args.save_dir,
+                 args.resolution, args.blur_sigma, args.use_motion_blur, args.use_gaussian_noise, args.show, num_cpu=2)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SiPMai-0.0.1/SiPMai/gen_data/smile_generation.py` & `SiPMai-0.0.2/SiPMai/gen_data/smile_generation.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.1/SiPMai/gen_data/util_fn.py` & `SiPMai-0.0.2/SiPMai/gen_data/util_fn.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.1/SiPMai/smiles/pubchem_39_200_100k.json` & `SiPMai-0.0.2/SiPMai/smiles/pubchem_39_200_100k.json`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.1/SiPMai/utils/dataloader.py` & `SiPMai-0.0.2/SiPMai/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.1/SiPMai.egg-info/PKG-INFO` & `SiPMai-0.0.2/SiPMai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiPMai
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Simple Yet Effective Scanning Tunnel Microscope Image Simulator
 Home-page: http://github.com/GilesLuo/SiPMai
 Author: Zhiyao Luo, Yaotian Yang, Jiali Li
 Author-email: zhiyao.luo@eng.ox.ac.uk
 License: MIT
 Project-URL: Source Code, https://github.com/my_username/my_package
 Keywords: Chemistry Simulation,STM Image Synthesis
```

### Comparing `SiPMai-0.0.1/SiPMai.egg-info/SOURCES.txt` & `SiPMai-0.0.2/SiPMai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 SiPMai/gen_data/ray_generation.py
 SiPMai/gen_data/smi_molecule_simulation.py
 SiPMai/gen_data/smile_generation.py
 SiPMai/gen_data/util_fn.py
 SiPMai/smiles/__init__.py
 SiPMai/smiles/pubchem_39_200_100k.json
 SiPMai/unittest/__init__.py
+SiPMai/unittest/test_gen_data.py
 SiPMai/utils/__init__.py
 SiPMai/utils/dataloader.py
```

### Comparing `SiPMai-0.0.1/setup.py` & `SiPMai-0.0.2/setup.py`

 * *Files identical despite different names*

