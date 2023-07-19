# Comparing `tmp/mdigest-0.1.1.tar.gz` & `tmp/mdigest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdigest-0.1.1.tar", last modified: Mon May 15 17:31:06 2023, max compression
+gzip compressed data, was "mdigest-0.1.3.tar", last modified: Wed Jul 19 15:00:58 2023, max compression
```

## Comparing `mdigest-0.1.1.tar` & `mdigest-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-05-15 17:31:06.253410 mdigest-0.1.1/
--rw-r--r--   0 federica   (501) staff       (20)    35128 2023-01-24 23:12:45.000000 mdigest-0.1.1/LICENSE
--rw-r--r--   0 federica   (501) staff       (20)       73 2023-01-24 23:12:45.000000 mdigest-0.1.1/MANIFEST.in
--rw-r--r--   0 federica   (501) staff       (20)      833 2023-05-15 17:31:06.253103 mdigest-0.1.1/PKG-INFO
--rw-r--r--   0 federica   (501) staff       (20)     9616 2023-05-15 17:09:02.000000 mdigest-0.1.1/README.md
-drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-05-15 17:31:06.234305 mdigest-0.1.1/mdigest/
--rw-r--r--   0 federica   (501) staff       (20)     6148 2023-02-15 22:22:17.000000 mdigest-0.1.1/mdigest/.DS_Store
--rw-r--r--   0 federica   (501) staff       (20)      149 2023-01-24 23:12:45.000000 mdigest-0.1.1/mdigest/__init__.py
-drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-05-15 17:31:06.246838 mdigest-0.1.1/mdigest/core/
--rw-r--r--   0 federica   (501) staff       (20)     1319 2023-02-22 16:43:10.000000 mdigest-0.1.1/mdigest/core/__init__.py
--rw-r--r--   0 federica   (501) staff       (20)    22903 2023-02-22 01:43:12.000000 mdigest-0.1.1/mdigest/core/analysis.py
--rw-r--r--   0 federica   (501) staff       (20)    25737 2023-02-22 00:32:22.000000 mdigest-0.1.1/mdigest/core/auxiliary.py
--rw-r--r--   0 federica   (501) staff       (20)    23976 2023-02-22 00:32:22.000000 mdigest-0.1.1/mdigest/core/correlation.py
--rw-r--r--   0 federica   (501) staff       (20)    15546 2023-05-15 16:49:54.000000 mdigest-0.1.1/mdigest/core/dcorrelation.py
--rw-r--r--   0 federica   (501) staff       (20)    16982 2023-02-22 01:43:12.000000 mdigest-0.1.1/mdigest/core/dimreduction.py
--rw-r--r--   0 federica   (501) staff       (20)     1114 2023-03-03 06:04:18.000000 mdigest-0.1.1/mdigest/core/imports.py
--rw-r--r--   0 federica   (501) staff       (20)    27091 2023-02-22 00:32:22.000000 mdigest-0.1.1/mdigest/core/kscorrelation.py
--rw-r--r--   0 federica   (501) staff       (20)    38393 2023-04-12 23:19:30.000000 mdigest-0.1.1/mdigest/core/networkcanvas.py
--rw-r--r--   0 federica   (501) staff       (20)    39594 2023-05-10 18:35:53.000000 mdigest-0.1.1/mdigest/core/networkcommunities.py
--rw-r--r--   0 federica   (501) staff       (20)     8340 2023-02-22 00:32:22.000000 mdigest-0.1.1/mdigest/core/parsetrajectory.py
-drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-05-15 17:31:06.249232 mdigest-0.1.1/mdigest/core/plots/
--rw-r--r--   0 federica   (501) staff       (20)      451 2023-01-24 23:12:45.000000 mdigest-0.1.1/mdigest/core/plots/__init__.py
--rw-r--r--   0 federica   (501) staff       (20)     2356 2023-01-24 23:12:45.000000 mdigest-0.1.1/mdigest/core/plots/dim_reduction_plots.py
--rw-r--r--   0 federica   (501) staff       (20)     2257 2023-01-24 23:12:45.000000 mdigest-0.1.1/mdigest/core/plots/general_plots.py
--rw-r--r--   0 federica   (501) staff       (20)    12459 2023-01-24 23:12:45.000000 mdigest-0.1.1/mdigest/core/plots/plot_correlation.py
--rw-r--r--   0 federica   (501) staff       (20)    27318 2023-02-22 00:32:22.000000 mdigest-0.1.1/mdigest/core/savedata.py
--rw-r--r--   0 federica   (501) staff       (20)     8878 2023-02-22 00:32:22.000000 mdigest-0.1.1/mdigest/core/toolkit.py
-drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-05-15 17:31:06.252407 mdigest-0.1.1/mdigest/utils/
--rw-r--r--   0 federica   (501) staff       (20)      100 2023-01-24 23:12:45.000000 mdigest-0.1.1/mdigest/utils/__init__.py
--rw-r--r--   0 federica   (501) staff       (20)       63 2023-01-24 23:12:45.000000 mdigest-0.1.1/mdigest/utils/imports.py
--rw-r--r--   0 federica   (501) staff       (20)     9920 2023-01-24 23:12:45.000000 mdigest-0.1.1/mdigest/utils/pdbhandler.py
--rw-r--r--   0 federica   (501) staff       (20)    16191 2023-02-22 01:43:12.000000 mdigest-0.1.1/mdigest/utils/simulation.py
--rw-r--r--   0 federica   (501) staff       (20)     3276 2023-01-24 23:12:45.000000 mdigest-0.1.1/mdigest/utils/toolkit.py
-drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-05-15 17:31:06.236560 mdigest-0.1.1/mdigest.egg-info/
--rw-r--r--   0 federica   (501) staff       (20)      833 2023-05-15 17:31:06.000000 mdigest-0.1.1/mdigest.egg-info/PKG-INFO
--rw-r--r--   0 federica   (501) staff       (20)      872 2023-05-15 17:31:06.000000 mdigest-0.1.1/mdigest.egg-info/SOURCES.txt
--rw-r--r--   0 federica   (501) staff       (20)        1 2023-05-15 17:31:06.000000 mdigest-0.1.1/mdigest.egg-info/dependency_links.txt
--rw-r--r--   0 federica   (501) staff       (20)      165 2023-05-15 17:31:06.000000 mdigest-0.1.1/mdigest.egg-info/requires.txt
--rw-r--r--   0 federica   (501) staff       (20)        8 2023-05-15 17:31:06.000000 mdigest-0.1.1/mdigest.egg-info/top_level.txt
--rw-r--r--   0 federica   (501) staff       (20)       38 2023-05-15 17:31:06.253490 mdigest-0.1.1/setup.cfg
--rw-r--r--   0 federica   (501) staff       (20)     1455 2023-05-15 17:25:02.000000 mdigest-0.1.1/setup.py
+drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-07-19 15:00:58.215595 mdigest-0.1.3/
+-rw-r--r--   0 federica   (501) staff       (20)    35128 2023-01-24 23:12:45.000000 mdigest-0.1.3/LICENSE
+-rw-r--r--   0 federica   (501) staff       (20)       73 2023-01-24 23:12:45.000000 mdigest-0.1.3/MANIFEST.in
+-rw-r--r--   0 federica   (501) staff       (20)      833 2023-07-19 15:00:58.215294 mdigest-0.1.3/PKG-INFO
+-rw-r--r--   0 federica   (501) staff       (20)     9616 2023-05-15 17:09:02.000000 mdigest-0.1.3/README.md
+drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-07-19 15:00:58.159865 mdigest-0.1.3/mdigest/
+-rw-r--r--   0 federica   (501) staff       (20)    10244 2023-06-28 20:20:43.000000 mdigest-0.1.3/mdigest/.DS_Store
+-rw-r--r--   0 federica   (501) staff       (20)      149 2023-01-24 23:12:45.000000 mdigest-0.1.3/mdigest/__init__.py
+drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-07-19 15:00:58.209687 mdigest-0.1.3/mdigest/core/
+-rw-r--r--   0 federica   (501) staff       (20)     1319 2023-02-22 16:43:10.000000 mdigest-0.1.3/mdigest/core/__init__.py
+-rw-r--r--   0 federica   (501) staff       (20)    22903 2023-02-22 01:43:12.000000 mdigest-0.1.3/mdigest/core/analysis.py
+-rw-r--r--   0 federica   (501) staff       (20)    25737 2023-02-22 00:32:22.000000 mdigest-0.1.3/mdigest/core/auxiliary.py
+-rw-r--r--   0 federica   (501) staff       (20)    24941 2023-06-28 20:14:17.000000 mdigest-0.1.3/mdigest/core/correlation.py
+-rw-r--r--   0 federica   (501) staff       (20)    16062 2023-06-28 20:14:17.000000 mdigest-0.1.3/mdigest/core/dcorrelation.py
+-rw-r--r--   0 federica   (501) staff       (20)    16982 2023-02-22 01:43:12.000000 mdigest-0.1.3/mdigest/core/dimreduction.py
+-rw-r--r--   0 federica   (501) staff       (20)     1114 2023-03-03 06:04:18.000000 mdigest-0.1.3/mdigest/core/imports.py
+-rw-r--r--   0 federica   (501) staff       (20)    29680 2023-06-28 19:31:49.000000 mdigest-0.1.3/mdigest/core/kscorrelation.py
+-rw-r--r--   0 federica   (501) staff       (20)    38393 2023-04-12 23:19:30.000000 mdigest-0.1.3/mdigest/core/networkcanvas.py
+-rw-r--r--   0 federica   (501) staff       (20)    39594 2023-05-10 18:35:53.000000 mdigest-0.1.3/mdigest/core/networkcommunities.py
+-rw-r--r--   0 federica   (501) staff       (20)     8432 2023-06-28 19:31:49.000000 mdigest-0.1.3/mdigest/core/parsetrajectory.py
+drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-07-19 15:00:58.211947 mdigest-0.1.3/mdigest/core/plots/
+-rw-r--r--   0 federica   (501) staff       (20)      451 2023-01-24 23:12:45.000000 mdigest-0.1.3/mdigest/core/plots/__init__.py
+-rw-r--r--   0 federica   (501) staff       (20)     2356 2023-01-24 23:12:45.000000 mdigest-0.1.3/mdigest/core/plots/dim_reduction_plots.py
+-rw-r--r--   0 federica   (501) staff       (20)     2257 2023-01-24 23:12:45.000000 mdigest-0.1.3/mdigest/core/plots/general_plots.py
+-rw-r--r--   0 federica   (501) staff       (20)    12459 2023-01-24 23:12:45.000000 mdigest-0.1.3/mdigest/core/plots/plot_correlation.py
+-rw-r--r--   0 federica   (501) staff       (20)    27314 2023-06-28 23:02:13.000000 mdigest-0.1.3/mdigest/core/savedata.py
+-rw-r--r--   0 federica   (501) staff       (20)     8878 2023-02-22 00:32:22.000000 mdigest-0.1.3/mdigest/core/toolkit.py
+drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-07-19 15:00:58.214504 mdigest-0.1.3/mdigest/utils/
+-rw-r--r--   0 federica   (501) staff       (20)      100 2023-01-24 23:12:45.000000 mdigest-0.1.3/mdigest/utils/__init__.py
+-rw-r--r--   0 federica   (501) staff       (20)       63 2023-01-24 23:12:45.000000 mdigest-0.1.3/mdigest/utils/imports.py
+-rw-r--r--   0 federica   (501) staff       (20)     9920 2023-01-24 23:12:45.000000 mdigest-0.1.3/mdigest/utils/pdbhandler.py
+-rw-r--r--   0 federica   (501) staff       (20)    16191 2023-02-22 01:43:12.000000 mdigest-0.1.3/mdigest/utils/simulation.py
+-rw-r--r--   0 federica   (501) staff       (20)     3276 2023-01-24 23:12:45.000000 mdigest-0.1.3/mdigest/utils/toolkit.py
+drwxr-xr-x   0 federica   (501) staff       (20)        0 2023-07-19 15:00:58.179275 mdigest-0.1.3/mdigest.egg-info/
+-rw-r--r--   0 federica   (501) staff       (20)      833 2023-07-19 15:00:57.000000 mdigest-0.1.3/mdigest.egg-info/PKG-INFO
+-rw-r--r--   0 federica   (501) staff       (20)      872 2023-07-19 15:00:58.000000 mdigest-0.1.3/mdigest.egg-info/SOURCES.txt
+-rw-r--r--   0 federica   (501) staff       (20)        1 2023-07-19 15:00:57.000000 mdigest-0.1.3/mdigest.egg-info/dependency_links.txt
+-rw-r--r--   0 federica   (501) staff       (20)      143 2023-07-19 15:00:57.000000 mdigest-0.1.3/mdigest.egg-info/requires.txt
+-rw-r--r--   0 federica   (501) staff       (20)        8 2023-07-19 15:00:57.000000 mdigest-0.1.3/mdigest.egg-info/top_level.txt
+-rw-r--r--   0 federica   (501) staff       (20)       38 2023-07-19 15:00:58.215692 mdigest-0.1.3/setup.cfg
+-rw-r--r--   0 federica   (501) staff       (20)     1527 2023-07-19 14:47:52.000000 mdigest-0.1.3/setup.py
```

### Comparing `mdigest-0.1.1/LICENSE` & `mdigest-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/PKG-INFO` & `mdigest-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdigest
-Version: 0.1.1
+Version: 0.1.3
 Summary: Best practices made easy for analysis of correlated motions from molecular dynamics simulations.
 Home-page: https://github.com/fmaschietto/MDiGest
 Author: Federica Maschietto, Brandon Allen
 Author-email: <federica.maschietto@gmail.com>, <brandon.allen@yale.edu>
 Keywords: python,correlation,molecular dynamics,MD trajectory analysis,correlated motions,network analysis,community network
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `mdigest-0.1.1/README.md` & `mdigest-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/core/__init__.py` & `mdigest-0.1.3/mdigest/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/core/analysis.py` & `mdigest-0.1.3/mdigest/core/analysis.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/core/auxiliary.py` & `mdigest-0.1.3/mdigest/core/auxiliary.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/core/correlation.py` & `mdigest-0.1.3/mdigest/core/correlation.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,30 +294,38 @@
             print("@>: found ", (nres * nres) - np.sum(excl_mat), 'nonzero elements in the exclusion matrix')
             print("---------------------------------------------------------------")
             return excl_mat
 
         exclusion_matrix_allreplicas = {}
 
         for win_idx in tk.log_progress(range(self.num_replicas), every=1, size=self.num_replicas, name="Window"):
-            beg = int(self.final / self.num_replicas) * win_idx
-            end = int(self.final / self.num_replicas) * (win_idx + 1)
+            #beg = int(self.final / self.num_replicas) * win_idx
+            #end = int(self.final / self.num_replicas) * (win_idx + 1)
+
+            offset =  (self.final - self.initial)// self.num_replicas
+            if self.window_span != offset/self.step:
+                print("@>: WARNING: the offset is not equal to the window span")
+
+            beg = self.initial + offset * win_idx
+            end = self.initial + offset * (win_idx + 1)
 
             print('@>: using frames %d to %d with step %s' % (beg, end, self.step))
 
             name = save_name + "_%d" % win_idx
 
             exclusion_matrix_allreplicas['rep_%d' %win_idx] = _compute_exclusion_matrix(self.mda_u, self.system_selstr,
                                                                               self.nresidues,
                                                                               beg, end, self.step, spatial_cutoff,
                                                                               contact_cutoff, name)
 
         self.exclusion_matrix_allreplicas = exclusion_matrix_allreplicas
 
 
-    def parse_dynamics(self, scale=False, normalize=True, LMI='gaussian', MI='knn_5_1', DCC=False, PCC=False, COV_DISP=False, VERBOSE=False, **kwargs):
+    def parse_dynamics(self, scale=False, normalize=True, LMI='gaussian', MI='knn_5_1', DCC=False, PCC=False, COV_DISP=False,
+                       CENTRALITY=True, VERBOSE=False, **kwargs):
         """
         Parse molecular dynamics trajectory and compute different correlation metrices
 
         Parameters
         ----------
         scale: bool,
             whether to remove mean from coordinates using StandardScaler
@@ -338,14 +346,17 @@
 
         PCC: bool,
             whether to compute Pearson correlation matrix of atomic displacements. Default is False
 
         COV_DISP: bool,
             whether to compute the covariance of atomic displacements. Default is False
 
+        CENTRALITY: bool,
+            whether to compute centrality of atomic displacements. Default is True
+
         VERBOSE: bool,
             whether to set verbose printing
 
         """
 
         # Assign stride variable
         stride = self.step
@@ -399,16 +410,23 @@
             solvers.append(MI)
         if LMI is not None:
             solvers.append(LMI)
 
 
         for win_idx in tk.log_progress(range(num_replicas), every=1, size=num_replicas, name="Window"):
 
-            beg = int(self.final / self.num_replicas) * win_idx
-            end = int(self.final / self.num_replicas) * (win_idx + 1)
+            #beg = int(self.final / self.num_replicas) * win_idx
+            #end = int(self.final / self.num_replicas) * (win_idx + 1)
+            offset =  (self.final - self.initial)// self.num_replicas
+            if self.window_span != offset/self.step:
+                print("@>: WARNING: the offset is not equal to the window span")
+
+            beg = self.initial + offset * win_idx
+            end = self.initial + offset * (win_idx + 1)
+
 
             print("@>: LMI/MI calculation ...")
             print("@>: begin frame: %d" % beg)
             print("@>: end   frame: %d" % end)
             print("@>: step:        %d" % self.step)
 
             counter = 0
@@ -451,26 +469,29 @@
             MIdict = {}
             ECdict = {}
             if solvers is not []:
                 for solver in solvers:
                     if solver == 'gaussian':
                         MIdict.update({'gcc_lmi': aux.compute_generalized_correlation_coefficients(displacements_allreplicas[win_idx].reshape((self.window_span, nr, feat_dimension)),
                                                                                          features_dimension=feat_dimension, solver=solver, correction=False)})
-                        _, ec = aux.compute_eigenvector_centrality(MIdict['gcc_lmi'], weight='weight')
-                        ECdict.update({'gcc_lmi': ec})
+                        if CENTRALITY:
+                            print("@>: computing eigenvector centrality from lmi matrix")
+                            _, ec = aux.compute_eigenvector_centrality(MIdict['gcc_lmi'], weight='weight')
+                            ECdict.update({'gcc_lmi': ec})
+
 
-                        print("@>: computing eigenvector centrality from lmi matrix")
 
 
                     elif 'knn' in solver:
                         MIdict.update({'gcc_mi': aux.compute_generalized_correlation_coefficients(displacements_allreplicas[win_idx].reshape((self.window_span, nr, feat_dimension)),
                                                                          features_dimension=feat_dimension, solver=solver, correction=True, subset=subset)})
-                        _, ec = aux.compute_eigenvector_centrality(MIdict['gcc_mi'], weight='weight')
-
-                        ECdict.update({'gcc_mi': ec})
+                        if CENTRALITY:
+                            print("@>: computing eigenvector centrality from mi matrix")
+                            _, ec = aux.compute_eigenvector_centrality(MIdict['gcc_mi'], weight='weight')
+                            ECdict.update({'gcc_mi': ec})
 
             self.gcc_allreplicas['rep_%d' % win_idx] = MIdict
             self.eigenvector_centrality_allreplicas['rep_%d' % win_idx] = ECdict
 
             print("@>: computing and storing distances...")
             distances_allreplicas[win_idx] = aux.compute_distance_matrix(coordinates_allreplicas[win_idx, :, :], feat_dimension)
```

### Comparing `mdigest-0.1.1/mdigest/core/dcorrelation.py` & `mdigest-0.1.3/mdigest/core/dcorrelation.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,16 +116,15 @@
         self.mds_data.dih_gcc_allreplicas = self.dih_gcc_allreplicas
         self.mds_data.dih_dcc_allreplicas = self.dih_dcc_allreplicas
         self.mds_data.dih_pcc_allreplicas = self.dih_pcc_allreplicas
         self.mds_data.dih_eigen_centrality_allreplicas = self.dih_eigen_centrality_allreplicas
         self.mds_data.save_to_file(file_name_root)
 
 
-    def parse_dih_dynamics(self, mean_center=False, LMI='gaussian', MI='knn_5_1', DCC=False, PCC=False, COV_DISP=True,
-                           **kwargs):
+    def parse_dih_dynamics(self, mean_center=False, LMI='gaussian', MI='knn_5_1', DCC=False, PCC=False, COV_DISP=True, CENTRALITY=True, **kwargs):
         """
         General purpose class handling computation of different correlation metrics from $\phi$, \$psi$ backbone dihedrals fluctuations sampled over MD trajectories.
         Diedrals are transformed using $\phi$ --> {$sin(\phi)$, $cos(\phi)$} and $\psi$ --> {$sin(\psi)$, $cos(\psi)$} such that each residue
         (temimal residues excluded) is described by an array of four entries [$sin(\phi)$, $cos(\phi)$, $sin(\psi)$, $cos(\psi)$].
 
         Parameters
         ----------
@@ -140,14 +139,16 @@
             5 specifies number of nearest neighbours, 1 specifies estimate to use (options are 1 or 2)
         DCC: bool,
             whether to compute dynamical cross correltaion
         PCC: bool,
             whether to compute Pearson's cross correlation
         COV_DISP: bool,
             whether to compute covariance of dihedrals displacements
+        CENTRALITY: bool,
+            whether to compute eigen centrality of dihedrals fluctuations. Default is True
         kwargs:
             - normalized: bool
                 whether to normalize DCC matrix
             - subset: list,
                 list of indices specifying the nodes for which to compute MI
             - center: str or None
                 How to compute the covariance matrix; possible values are 'mean' or 'square_disp'
@@ -205,16 +206,23 @@
         if LMI is not None:
             solvers.append(LMI)
 
         num_replicas = self.num_replicas
 
         for win_idx in tk.log_progress(range(self.num_replicas), 1, size=num_replicas, name="Window"):
 
-            beg = int(self.final / self.num_replicas) * win_idx
-            end = int(self.final / self.num_replicas) * (win_idx + 1)
+            #beg = int(self.final / self.num_replicas) * win_idx
+            #end = int(self.final / self.num_replicas) * (win_idx + 1)
+            offset =  (self.final - self.initial)// self.num_replicas
+            if self.window_span != offset/self.step:
+                print("@>: WARNING: the offset is not equal to the window span")
+
+            beg = self.initial + offset * win_idx
+            end = self.initial + offset * (win_idx + 1)
+
             stride = self.step
             print("@>: start, end frames:", beg, end)
 
             print("@>: Dihedrals calculation ...")
             self.ramachandran = Ramachandran(self.mda_u.universe.select_atoms(self.system_selstr)).run()
             r = self.ramachandran
 
@@ -277,31 +285,30 @@
                     if solver == 'gaussian':
                         print("@>: computing lmi correlation matrix")
                         MIdict.update({'gcc_lmi': aux.compute_generalized_correlation_coefficients(values,
                                                                                                    features_dimension=len(
                                                                                                        self.dih_labels),
                                                                                                    solver=solver,
                                                                                                    correction=False)})
-
-                        print("@>: computing eigenvector centrality from lmi matrix")
-                        _, ec = aux.compute_eigenvector_centrality(MIdict['gcc_lmi'], weight='weight')
-
-                        ECdict.update({'gcc_lmi': ec})
+                        if CENTRALITY:
+                            print("@>: computing eigenvector centrality from lmi matrix")
+                            _, ec = aux.compute_eigenvector_centrality(MIdict['gcc_lmi'], weight='weight')
+                            ECdict.update({'gcc_lmi': ec})
 
                     elif 'knn' in solver:
                         print("@>: computing mi correlation matrix")
                         MIdict.update({'gcc_mi': aux.compute_generalized_correlation_coefficients(values,
                                                                                                   features_dimension=len(
                                                                                                       self.dih_labels),
                                                                                                   solver=solver,
-                                                                                                  correction=True)})
-                        print("@>: computing eigenvector centrality from mi matrix")
-                        _, ec = aux.compute_eigenvector_centrality(MIdict['gcc_mi'], weight='weight')
-
-                        ECdict.update({'gcc_mi': ec})
+                                                                                              correction=True)})
+                        if CENTRALITY:
+                            print("@>: computing eigenvector centrality from mi matrix")
+                            _, ec = aux.compute_eigenvector_centrality(MIdict['gcc_mi'], weight='weight')
+                            ECdict.update({'gcc_mi': ec})
 
                 self.dih_gcc_allreplicas['rep_%d' % win_idx] = MIdict
                 self.dih_eigen_centrality_allreplicas['rep_%d' % win_idx] = ECdict
 
             if COV_DISP:
                 print("@>: computing covariance of dihedral fluctuations")
                 self.covar_dih_allreplicas['rep_%d' % win_idx] = aux.evaluate_covariance_matrix(values, center=center)
```

### Comparing `mdigest-0.1.1/mdigest/core/dimreduction.py` & `mdigest-0.1.3/mdigest/core/dimreduction.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/core/imports.py` & `mdigest-0.1.3/mdigest/core/imports.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/core/kscorrelation.py` & `mdigest-0.1.3/mdigest/core/kscorrelation.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,21 +250,81 @@
             if not remap:
                 d[count][:, np.where(self.is_protein == 0)[0]] = 0.
 
             count += 1
         return d
 
 
+    # def compute_distances_parallel(self, beg, end, stride, remap=False):
+    #     """
+    #     Compute distances in parallel
+    #
+    #     Parameters
+    #     ----------
+    #
+    #     beg: int,
+    #         initial frame
+    #     end: int,
+    #         end frame
+    #     stride: int,
+    #         step
+    #     remap: bool,
+    #         if True assumes remapping is unneeded (all distance matrices have the same dimension)
+    #
+    #     Returns
+    #     -------
+    #     bb_dist_dict: dict
+    #         dictionary with CN, CH, OH, ON as keys and np.ndarrays with the corresponding distance arrays as values
+    #     """
+    #
+    #     print('@>: computing distances in parallel')
+    #
+    #     C = self.indices['C-Backbone']
+    #     N = self.indices['N-Backbone']
+    #     O = self.indices['O-Backbone']
+    #     H = self.indices['H-Backbone']
+    #
+    #     func = self._distances
+    #     calls = { 'CN': func(C, N, beg, end, stride, remap=True),
+    #               'CH': func(C, H, beg, end, stride, remap=remap),
+    #               'OH': func(O, H, beg, end, stride, remap=remap),
+    #               'ON': func(O, N, beg, end, stride, remap=True)}
+    #
+    #     processes = []
+    #     results = {}
+    #     with ThreadPoolExecutor(MAX_WORKERS) as executor:
+    #         for key, obj_ in calls.items():
+    #             processes.append(executor.submit(obj_))
+    #             results.update({key:obj_})
+    #
+    #     bb_dist_dict = {}
+    #
+    #     bb_dist_dict.update({'CH': results['CH']})
+    #     bb_dist_dict.update({'ON': results['ON']})
+    #     bb_dist_dict.update({'OH': results['OH']})
+    #     bb_dist_dict.update({'CN': results['CN']})
+    #     return bb_dist_dict
+
+    ############# NOTES #########################
+
+    # The processes list is created to store the references to the executor.submit objects returned by the ThreadPoolExecutor.
+    # However, these references are not used later in the code. As a result, the garbage collector may not be able to release the memory
+    # associated with these objects. To address this issue, we can remove the processes list,
+    # allowing the objects to be automatically garbage collected.
+    #
+    # To fix these issues, you can modify the compute_distances_parallel method as follows:
+    # TEST IT !
+
+
     def compute_distances_parallel(self, beg, end, stride, remap=False):
         """
         Compute distances in parallel
 
         Parameters
         ----------
-
         beg: int,
             initial frame
         end: int,
             end frame
         stride: int,
             step
         remap: bool,
@@ -280,35 +340,32 @@
 
         C = self.indices['C-Backbone']
         N = self.indices['N-Backbone']
         O = self.indices['O-Backbone']
         H = self.indices['H-Backbone']
 
         func = self._distances
-        calls = { 'CN': func(C, N, beg, end, stride, remap=True),
-                  'CH': func(C, H, beg, end, stride, remap=remap),
-                  'OH': func(O, H, beg, end, stride, remap=remap),
-                  'ON': func(O, N, beg, end, stride, remap=True)}
 
-        processes = []
         results = {}
         with ThreadPoolExecutor(MAX_WORKERS) as executor:
-            for key, obj_ in calls.items():
-                processes.append(executor.submit(obj_))
-                results.update({key:obj_})
+            results['CN'] = executor.submit(func, C, N, beg, end, stride, remap=True)
+            results['CH'] = executor.submit(func, C, H, beg, end, stride, remap=remap)
+            results['OH'] = executor.submit(func, O, H, beg, end, stride, remap=remap)
+            results['ON'] = executor.submit(func, O, N, beg, end, stride, remap=True)
 
         bb_dist_dict = {}
 
-        bb_dist_dict.update({'CH': results['CH']})
-        bb_dist_dict.update({'ON': results['ON']})
-        bb_dist_dict.update({'OH': results['OH']})
-        bb_dist_dict.update({'CN': results['CN']})
+        bb_dist_dict.update({'CH': results['CH'].result()})
+        bb_dist_dict.update({'ON': results['ON'].result()})
+        bb_dist_dict.update({'OH': results['OH'].result()})
+        bb_dist_dict.update({'CN': results['CN'].result()})
         return bb_dist_dict
 
 
+
     def compute_KS_energy(self, dist_dict, topology_charges=False):
         """
         Perform KS calculation
 
         Parameters
         ----------
         dist_dict: dict,
@@ -536,16 +593,24 @@
 
         print('@>: prepare kabsch sanders calculation')
         self.prepare_kabsch_sander_arrays()
         print('@>: run KS calculation')
 
 
         for win_idx in tk.log_progress(range(self.num_replicas), every=1, size=self.num_replicas, name="Window"):
-            beg =  int(self.final/self.num_replicas)* win_idx
-            end =  int(self.final/self.num_replicas)* (win_idx + 1)
+            #beg =  int(self.final/self.num_replicas)* win_idx
+            #end =  int(self.final/self.num_replicas)* (win_idx + 1)
+
+            offset =  (self.final - self.initial)// self.num_replicas
+            if self.window_span != offset/self.step:
+                print("@>: WARNING: the offset is not equal to the window span")
+
+            beg = self.initial + offset * win_idx
+            end = self.initial + offset * (win_idx + 1)
+
             print("@>: KS energy calculation ...")
             print("@>: begin frame: %d" % beg)
             print("@>: end   frame: %d" % end)
             print("@>: step:        %d" % self.step)
             stride = self.step
             bb_distances_dict = self.compute_distances_parallel(beg, end, stride)
             KS_energies = self.compute_KS_energy(bb_distances_dict, topology_charges=topology_charges)
```

### Comparing `mdigest-0.1.1/mdigest/core/networkcanvas.py` & `mdigest-0.1.3/mdigest/core/networkcanvas.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/core/networkcommunities.py` & `mdigest-0.1.3/mdigest/core/networkcommunities.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/core/parsetrajectory.py` & `mdigest-0.1.3/mdigest/core/parsetrajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,16 @@
         # Final frame
         self.final = final
 
         # Step
         self.step =  step
 
         # Window span defines the lenght of each simulation block (replica)
-        self.window_span = int(np.ceil(np.ceil((self.final - self.initial) / self.step)/ self.num_replicas))
+        #self.window_span = int(np.ceil(np.ceil((self.final - self.initial) / self.step)/ self.num_replicas))
+        self.window_span = ((self.final - self.initial) // self.step) // self.num_replicas
 
         # Number of frames per replica
         self.nframes_per_replica = int(len(self.mda_u.trajectory[initial:final:step])/self.num_replicas)
 
 
         print('@>: number of frames:      %d' % self.total_nframes)
         print('@>: number of replicas:    %d' % self.num_replicas)
```

### Comparing `mdigest-0.1.1/mdigest/core/plots/dim_reduction_plots.py` & `mdigest-0.1.3/mdigest/core/plots/dim_reduction_plots.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/core/plots/general_plots.py` & `mdigest-0.1.3/mdigest/core/plots/general_plots.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/core/plots/plot_correlation.py` & `mdigest-0.1.3/mdigest/core/plots/plot_correlation.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/core/savedata.py` & `mdigest-0.1.3/mdigest/core/savedata.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,26 +492,26 @@
         if file_exists(file_name_root + "_nxGraphs_dict.pickle"):
             print('@>: load %s' % file_name_root + '_nxGraphs_dict.pickle')
             with open(file_name_root + "_nxGraphs_dict.pickle", 'rb') as infile:
                 self.nxGraphs_dict = pickle.load(infile)
 
         # load other attributes
         try:
-            if self.nodes_to_res_dictionary is not None:
-                self.nresidues = len(np.unique(np.asarray(list(self.nodes_to_res_dictionary.values()))))
+            #if self.nodes_to_res_dictionary is not None:
+            self.nresidues = len(np.unique(np.asarray(list(self.nodes_to_res_dictionary.values()))))
         except AttributeError:
             self.nresidues = np.asarray([len(v) for k, v in
-                                         self.nodes_communities_collect[0]['comm_nodes'].items()]).sum()
+                                         self.nodes_communities_collect['0']['comm_nodes'].items()]).sum()
 
         if self.nnodes is not None:
             self.nnodes = len(np.unique(np.asarray(list(self.nodes_to_res_dictionary.values()))))
 
         try:
-            if self.eigvec_centrality_don_allrep is not None:
-                self.num_replicas = len(self.eigvec_centrality_don_allrep)
+            #if self.eigvec_centrality_don_allrep is not None:
+            self.num_replicas = len(self.eigvec_centrality_don_allrep)
         except TypeError:
             try:
                 self.num_replicas = len(self.eigenvector_centrality_allreplicas)
             except TypeError:
                 try:
                     self.num_replicas = len(self.dih_eigen_centrality_allreplicas)
                 except TypeError:
```

### Comparing `mdigest-0.1.1/mdigest/core/toolkit.py` & `mdigest-0.1.3/mdigest/core/toolkit.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/utils/pdbhandler.py` & `mdigest-0.1.3/mdigest/utils/pdbhandler.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/utils/simulation.py` & `mdigest-0.1.3/mdigest/utils/simulation.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest/utils/toolkit.py` & `mdigest-0.1.3/mdigest/utils/toolkit.py`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/mdigest.egg-info/PKG-INFO` & `mdigest-0.1.3/mdigest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdigest
-Version: 0.1.1
+Version: 0.1.3
 Summary: Best practices made easy for analysis of correlated motions from molecular dynamics simulations.
 Home-page: https://github.com/fmaschietto/MDiGest
 Author: Federica Maschietto, Brandon Allen
 Author-email: <federica.maschietto@gmail.com>, <brandon.allen@yale.edu>
 Keywords: python,correlation,molecular dynamics,MD trajectory analysis,correlated motions,network analysis,community network
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `mdigest-0.1.1/mdigest.egg-info/SOURCES.txt` & `mdigest-0.1.3/mdigest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdigest-0.1.1/setup.py` & `mdigest-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1'
+VERSION = '0.1.3'
 DESCRIPTION = 'Best practices made easy for analysis of correlated motions from molecular dynamics simulations.'
 LONG_DESCRIPTION = 'MDiGest is a best-practices-made-easy Python package that handles the most common issues in ' \
                    'the network-based analysis of correlated motions from molecular dynamics simulations.'
 
 setup(
     name="mdigest",
     version=VERSION,
     author="Federica Maschietto, Brandon Allen",
     author_email="<federica.maschietto@gmail.com>, <brandon.allen@yale.edu>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=[
-        'pandas>=1.5.3',
-        'seaborn>=0.12.2',
-        'mdtraj>=1.9.7',
-        'pyemma==2.5.12',
-        'MDAnalysis>=2.3.0',
-        'silx>=1.1.1',
-        'numba>=0.56.4',
-        'python-louvain==0.15',
-        'nglview>=3.0.3',
-        'networkx>=2.6.3',
-        'silx>=1.1'],
+    install_requires=['numpy<=1.24.3',
+                      'numba==0.56.4',
+                      'scipy>=1.10.0',
+                      'python-louvain==0.15',
+                      'pymol-open-source',
+                      'pandas', 'seaborn',
+                      'mdtraj', 'pyemma',
+                      'MDAnalysis', 'silx',
+                      'nglview', 'networkx'],
+
     keywords=[
         'python',
         'correlation',
         'molecular dynamics',
         'MD trajectory analysis',
         'correlated motions',
         'network analysis',
```

