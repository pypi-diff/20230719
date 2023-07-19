# Comparing `tmp/nisnap-0.4.post0.tar.gz` & `tmp/nisnap-0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nisnap-0.4.post0.tar", last modified: Fri Dec 17 11:02:42 2021, max compression
+gzip compressed data, was "nisnap-0.4a0.tar", last modified: Fri Nov 26 14:46:44 2021, max compression
```

## Comparing `nisnap-0.4.post0.tar` & `nisnap-0.4a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 grg       (1000) grg       (1000)        0 2021-12-17 11:02:42.412030 nisnap-0.4.post0/
--rw-rw-r--   0 grg       (1000) grg       (1000)    13080 2021-12-17 11:02:42.412030 nisnap-0.4.post0/PKG-INFO
--rw-rw-r--   0 grg       (1000) grg       (1000)    10235 2021-12-17 10:54:44.000000 nisnap-0.4.post0/README.md
-drwxrwxr-x   0 grg       (1000) grg       (1000)        0 2021-12-17 11:02:42.412030 nisnap-0.4.post0/bin/
--rwxrwxr-x   0 grg       (1000) grg       (1000)      270 2021-09-06 15:02:15.000000 nisnap-0.4.post0/bin/nisnap
-drwxrwxr-x   0 grg       (1000) grg       (1000)        0 2021-12-17 11:02:42.412030 nisnap-0.4.post0/nisnap/
--rw-rw-r--   0 grg       (1000) grg       (1000)      139 2021-12-17 11:02:34.000000 nisnap-0.4.post0/nisnap/__init__.py
--rw-rw-r--   0 grg       (1000) grg       (1000)    13455 2021-12-17 11:00:17.000000 nisnap-0.4.post0/nisnap/snap.py
-drwxrwxr-x   0 grg       (1000) grg       (1000)        0 2021-12-17 11:02:42.412030 nisnap-0.4.post0/nisnap/utils/
--rw-rw-r--   0 grg       (1000) grg       (1000)        0 2021-09-06 15:02:15.000000 nisnap-0.4.post0/nisnap/utils/__init__.py
--rw-rw-r--   0 grg       (1000) grg       (1000)     4087 2021-12-17 10:54:44.000000 nisnap-0.4.post0/nisnap/utils/aseg.py
--rw-rw-r--   0 grg       (1000) grg       (1000)    33378 2021-12-17 10:54:44.000000 nisnap-0.4.post0/nisnap/utils/colormap.json
--rw-rw-r--   0 grg       (1000) grg       (1000)     4907 2021-12-17 10:54:44.000000 nisnap-0.4.post0/nisnap/utils/montage.py
--rw-rw-r--   0 grg       (1000) grg       (1000)     6468 2021-09-16 08:22:13.000000 nisnap-0.4.post0/nisnap/utils/parse.py
--rw-rw-r--   0 grg       (1000) grg       (1000)     4856 2021-12-17 10:54:44.000000 nisnap-0.4.post0/nisnap/utils/slices.py
--rw-rw-r--   0 grg       (1000) grg       (1000)    16670 2021-12-17 10:54:44.000000 nisnap-0.4.post0/nisnap/xnat.py
-drwxrwxr-x   0 grg       (1000) grg       (1000)        0 2021-12-17 11:02:42.412030 nisnap-0.4.post0/nisnap.egg-info/
--rw-rw-r--   0 grg       (1000) grg       (1000)    13080 2021-12-17 11:02:42.000000 nisnap-0.4.post0/nisnap.egg-info/PKG-INFO
--rw-rw-r--   0 grg       (1000) grg       (1000)      369 2021-12-17 11:02:42.000000 nisnap-0.4.post0/nisnap.egg-info/SOURCES.txt
--rw-rw-r--   0 grg       (1000) grg       (1000)        1 2021-12-17 11:02:42.000000 nisnap-0.4.post0/nisnap.egg-info/dependency_links.txt
--rw-rw-r--   0 grg       (1000) grg       (1000)      140 2021-12-17 11:02:42.000000 nisnap-0.4.post0/nisnap.egg-info/requires.txt
--rw-rw-r--   0 grg       (1000) grg       (1000)        7 2021-12-17 11:02:42.000000 nisnap-0.4.post0/nisnap.egg-info/top_level.txt
--rw-rw-r--   0 grg       (1000) grg       (1000)       38 2021-12-17 11:02:42.412030 nisnap-0.4.post0/setup.cfg
--rw-rw-r--   0 grg       (1000) grg       (1000)     1446 2021-12-17 10:54:44.000000 nisnap-0.4.post0/setup.py
+drwxrwxr-x   0 grg       (1000) grg       (1000)        0 2021-11-26 14:46:44.542422 nisnap-0.4a0/
+-rw-rw-r--   0 grg       (1000) grg       (1000)    13076 2021-11-26 14:46:44.542422 nisnap-0.4a0/PKG-INFO
+-rw-rw-r--   0 grg       (1000) grg       (1000)    10235 2021-11-25 18:58:50.000000 nisnap-0.4a0/README.md
+drwxrwxr-x   0 grg       (1000) grg       (1000)        0 2021-11-26 14:46:44.542422 nisnap-0.4a0/bin/
+-rwxrwxr-x   0 grg       (1000) grg       (1000)      270 2021-09-06 15:02:15.000000 nisnap-0.4a0/bin/nisnap
+drwxrwxr-x   0 grg       (1000) grg       (1000)        0 2021-11-26 14:46:44.542422 nisnap-0.4a0/nisnap/
+-rw-rw-r--   0 grg       (1000) grg       (1000)      136 2021-11-26 14:31:16.000000 nisnap-0.4a0/nisnap/__init__.py
+-rw-rw-r--   0 grg       (1000) grg       (1000)    13390 2021-11-26 13:56:15.000000 nisnap-0.4a0/nisnap/snap.py
+drwxrwxr-x   0 grg       (1000) grg       (1000)        0 2021-11-26 14:46:44.542422 nisnap-0.4a0/nisnap/utils/
+-rw-rw-r--   0 grg       (1000) grg       (1000)        0 2021-09-06 15:02:15.000000 nisnap-0.4a0/nisnap/utils/__init__.py
+-rw-rw-r--   0 grg       (1000) grg       (1000)     4087 2021-09-16 08:23:01.000000 nisnap-0.4a0/nisnap/utils/aseg.py
+-rw-rw-r--   0 grg       (1000) grg       (1000)    33378 2021-09-16 08:22:57.000000 nisnap-0.4a0/nisnap/utils/colormap.json
+-rw-rw-r--   0 grg       (1000) grg       (1000)     4907 2021-09-16 08:44:43.000000 nisnap-0.4a0/nisnap/utils/montage.py
+-rw-rw-r--   0 grg       (1000) grg       (1000)     6468 2021-09-16 08:22:13.000000 nisnap-0.4a0/nisnap/utils/parse.py
+-rw-rw-r--   0 grg       (1000) grg       (1000)     4856 2021-09-16 08:44:43.000000 nisnap-0.4a0/nisnap/utils/slices.py
+-rw-rw-r--   0 grg       (1000) grg       (1000)    17113 2021-11-26 13:56:15.000000 nisnap-0.4a0/nisnap/xnat.py
+drwxrwxr-x   0 grg       (1000) grg       (1000)        0 2021-11-26 14:46:44.542422 nisnap-0.4a0/nisnap.egg-info/
+-rw-rw-r--   0 grg       (1000) grg       (1000)    13076 2021-11-26 14:46:44.000000 nisnap-0.4a0/nisnap.egg-info/PKG-INFO
+-rw-rw-r--   0 grg       (1000) grg       (1000)      369 2021-11-26 14:46:44.000000 nisnap-0.4a0/nisnap.egg-info/SOURCES.txt
+-rw-rw-r--   0 grg       (1000) grg       (1000)        1 2021-11-26 14:46:44.000000 nisnap-0.4a0/nisnap.egg-info/dependency_links.txt
+-rw-rw-r--   0 grg       (1000) grg       (1000)      140 2021-11-26 14:46:44.000000 nisnap-0.4a0/nisnap.egg-info/requires.txt
+-rw-rw-r--   0 grg       (1000) grg       (1000)        7 2021-11-26 14:46:44.000000 nisnap-0.4a0/nisnap.egg-info/top_level.txt
+-rw-rw-r--   0 grg       (1000) grg       (1000)       38 2021-11-26 14:46:44.542422 nisnap-0.4a0/setup.cfg
+-rw-rw-r--   0 grg       (1000) grg       (1000)     1446 2021-11-26 14:27:51.000000 nisnap-0.4a0/setup.py
```

### Comparing `nisnap-0.4.post0/PKG-INFO` & `nisnap-0.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nisnap
-Version: 0.4.post0
+Version: 0.4a0
 Summary: nisnap
 Home-page: https://github.com/xgrg/nisnap
 Author: Greg Operto
 Author-email: goperto@barcelonabeta.org
 License: UNKNOWN
 Download-URL: https://github.com/xgrg/nisnap/-/archive/v0.4/nisnap-v0.4.tar.gz
 Description: # nisnap
```

### Comparing `nisnap-0.4.post0/README.md` & `nisnap-0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `nisnap-0.4.post0/nisnap/snap.py` & `nisnap-0.4a0/nisnap/snap.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,21 +70,19 @@
     return
 
 
 def _snap_contours_(data, slices, axis, bg, figsize=None, bb=None, pbar=None):
     from matplotlib import pyplot as plt
     import numpy as np
     import tempfile
-    import os
 
     plt.style.use('dark_background')
 
     paths = []
-    fd, path = tempfile.mkstemp(suffix='_%s%s' % (axis, __format__))
-    os.close(fd)
+    _, path = tempfile.mkstemp(suffix='_%s%s' % (axis, __format__))
     paths.append(path)
 
     same_box = bb is not None
     if not same_box:
         bb = {}
 
     lambdas = {'x': lambda y, x: y[:, :, x],
@@ -146,34 +144,32 @@
     return paths, bb
 
 
 def _snap_slices_(data, slices, axis, bb=None, figsize=None, pbar=None):
     from matplotlib import pyplot as plt
     import numpy as np
     import tempfile
-    import os
 
     labels = list(np.unique(data))
     has_bb = bb is not None
     d = data.ravel()
-    ratio = len(d[d <= 10]) / len(d)
+    ratio = len(d[d == 0]) / len(d)
     # has_orig = len(labels) > 50  # not bb is None
-    is_raw = ratio < 0.80
+    is_raw = ratio < 0.90
 
     paths = []
     if not has_bb:
         bb = {}
 
     fig = plt.figure(dpi=300, figsize=figsize)
 
     from nisnap.utils.slices import __get_lambdas__
     lambdas = __get_lambdas__(data)
 
-    fd, path = tempfile.mkstemp(suffix='_%s%s' % (axis, __format__))
-    os.close(fd)
+    _, path = tempfile.mkstemp(suffix='_%s%s' % (axis, __format__))
     paths.append(path)
 
     abs_index = 0
     for a, chunk in enumerate(slices):
 
         if not has_bb:
             bb[a] = []
```

### Comparing `nisnap-0.4.post0/nisnap/utils/aseg.py` & `nisnap-0.4a0/nisnap/utils/aseg.py`

 * *Files identical despite different names*

### Comparing `nisnap-0.4.post0/nisnap/utils/colormap.json` & `nisnap-0.4a0/nisnap/utils/colormap.json`

 * *Files identical despite different names*

### Comparing `nisnap-0.4.post0/nisnap/utils/montage.py` & `nisnap-0.4a0/nisnap/utils/montage.py`

 * *Files identical despite different names*

### Comparing `nisnap-0.4.post0/nisnap/utils/parse.py` & `nisnap-0.4a0/nisnap/utils/parse.py`

 * *Files identical despite different names*

### Comparing `nisnap-0.4.post0/nisnap/utils/slices.py` & `nisnap-0.4a0/nisnap/utils/slices.py`

 * *Files identical despite different names*

### Comparing `nisnap-0.4.post0/nisnap/xnat.py` & `nisnap-0.4a0/nisnap/xnat.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,54 +60,37 @@
     t2_t1space = list(e.resource('ANTS').files('*%s*T1space.nii.gz'
                                                % t2_scans[0]))[0]
     return t2_t1space
 
 
 def __download_freesurfer__(x, experiment_id, destination,
                             resource_name='FREESURFER7',
-                            raw=True, cache=False, fn='aparc+aseg.mgz'):
+                            raw=True, cache=False):
     import os.path as op
     filepaths = []
     e = x.select.experiment(experiment_id)
     r = e.resource(resource_name)
-    if not r.exists():
-        raise Exception('Experiment %s has no resource %s.' % (experiment_id, resource_name))
 
     if raw:
         fp1 = op.join(destination, '%s_T1.nii.gz' % experiment_id)
         filepaths.append(fp1)
         if not cache:
             t1_file = __get_T1__(x, experiment_id)
             t1_file.get(fp1)
     else:
         filepaths.append(None)
 
-    files = ['rawavg.mgz', fn] if __freesurfer_reg_to_native__\
-        else ['nu.mgz', fn]
-    for each in files:
-        c = list(r.files('*%s' % each))
-        if each in ['nu.mgz', 'rawavg.mgz']:  # should come from FREESURFER7
-            r1 = e.resource(resource_name.split('_EXTRAS')[0])
-            c = list(r1.files('*%s' % each))
+    files = ['rawavg.mgz', 'aparc+aseg.mgz'] if __freesurfer_reg_to_native__\
+        else ['nu.mgz', 'aparc+aseg.mgz']
 
+    for each in files:
+        c = list(r.files('*%s' % each))[0]
         fp = op.join(destination, '%s_%s' % (experiment_id, each))
         if not cache:
-            c[0].get(fp)
-        filepaths.append(fp)
-
-    if fn == 'hypothalamic_subunits_seg.v1.mgz':
-        # Register hypothalamus
-        import nibabel as nib
-        from nilearn.image import resample_img
-        target_affine = nib.load(filepaths[1]).affine  # thalamus
-        img = nib.load(filepaths[2])  # hypothalamus
-        resampled_nii = resample_img(img, target_affine, interpolation='nearest')
-        fp = filepaths[2].replace('.mgz', 'FSvoxelSpace.mgz')
-        resampled_nii.to_filename(fp)
-        filepaths.pop(-1)
+            c.get(fp)
         filepaths.append(fp)
 
     from nisnap.utils import aseg
     aseg_fp = filepaths[2]
     bg = filepaths[1]
 
     # Note that the filepaths for these new steps are not stored/returned
@@ -128,18 +111,98 @@
     # So we only need to fetch their names (with cache=True)
     if __freesurfer_reg_to_native__:
         aseg_fp = aseg.__preproc_aseg__(aseg_fp, bg, cache=True)
     else:
         aseg_fp = aseg.__swap_fs__(aseg_fp, cache=True)
         bg = aseg.__swap_fs__(filepaths[1], cache=True)
 
+    return [bg, aseg_fp]
+
+
+def __download_freesurfer7_extras__(x, experiment_id, destination,
+                                    resource_name='FREESURFER7_EXTRAS',
+                                    raw=True, cache=False):
+    import os.path as op
+    import logging as log
+
+    # __freesurfer_reg_to_native__ = True
+    # log.info('__freesurfer_reg_to_native__: True by default (%s)' % resource_name)
+
+    filepaths = []
+    e = x.select.experiment(experiment_id)
+    r1 = e.resource(resource_name.split('_EXTRAS')[0])
+    r2 = e.resource(resource_name)
+
+    if raw:
+        fp1 = op.join(destination, '%s_T1.nii.gz' % experiment_id)
+        filepaths.append(fp1)
+        if not cache:
+            t1_file = __get_T1__(x, experiment_id)
+            t1_file.get(fp1)
+    else:
+        filepaths.append(None)
+
+    extras_files = ['hypothalamic_subunits_seg.v1.mgz',
+                    'ThalamicNuclei.v12.T1.FSvoxelSpace.mgz',
+                    'brainstemSsLabels.v12.FSvoxelSpace.mgz']
+    files = ['rawavg.mgz'] if __freesurfer_reg_to_native__ else ['nu.mgz']
+    files.extend(extras_files)
+    r = r1
+    for each in files:
+        c = list(r.files('*%s' % each))[0]
+        r = r2
+        fp = op.join(destination, '%s_%s' % (experiment_id, each))
+        if not cache:
+            c.get(fp)
+        filepaths.append(fp)
+
+    # Register hypothalamus
+    import nibabel as nib
+    from nilearn.image import resample_img
+    target_affine = nib.load(filepaths[3]).affine  # thalamus
+    img = nib.load(filepaths[2])  # hypothalamus
+    resampled_nii = resample_img(img, target_affine, interpolation='nearest')
+    fp = filepaths[2].replace('.mgz', 'FSvoxelSpace.mgz')
+    resampled_nii.to_filename(fp)
+
+    filepaths.pop(2)
+    filepaths.insert(2, fp)
+
+    from nisnap.utils import aseg
+    for aseg_fp in filepaths[2:]:
+        bg = filepaths[1]
+
+        # Note that the filepaths for these new steps are not stored/returned
+        if __freesurfer_reg_to_native__:
+            aseg.__preproc_aseg__(aseg_fp, bg, cache=cache)
+        aseg.__swap_fs__(aseg_fp, cache=cache)
+        aseg.__swap_fs__(bg, cache=cache)
+
+    log.basicConfig(level=log.INFO)
+    log.info('__freesurfer_reg_to_native__: %s' % __freesurfer_reg_to_native__)
+
+    bg = filepaths[0]
+
+    res = []
+    for aseg_fp in filepaths[2:]:
+
+        # Files were created just before
+        # So we only need to fetch their names (with cache=True)
+        if __freesurfer_reg_to_native__:
+            aseg_fp = aseg.__preproc_aseg__(aseg_fp, bg, cache=True)
+        else:
+            aseg_fp = aseg.__swap_fs__(aseg_fp, cache=True)
+            bg = aseg.__swap_fs__(filepaths[1], cache=True)
+        res.append(aseg_fp)
+
     if raw:
-        res = [bg, aseg_fp]
+        res.insert(0, bg)
     else:
-        res = [None, aseg_fp]
+        res.insert(0, None)
+
     return res
 
 
 def __download_spm12__(x, experiment_id, destination,
                        resource_name='SPM12_SEGMENT',
                        raw=True, cache=False):
     import os.path as op
@@ -250,37 +313,20 @@
                                        resource_name, raw, cache)
 
     elif resource_name == 'ASHS':
         filepaths = __download_ashs__(x, experiment_id, destination,
                                       resource_name, raw, cache)
 
     elif 'FREESURFER' in resource_name and resource_name.endswith('_EXTRAS'):
-        files = ['hypothalamic_subunits_seg.v1.mgz',
-                 'ThalamicNuclei.v12.T1.FSvoxelSpace.mgz',
-                 'brainstemSsLabels.v12.FSvoxelSpace.mgz']
-        filepaths = []
-        for fn in files:
-            fp = __download_freesurfer__(x, experiment_id,
-                                         destination, resource_name,
-                                         raw, cache, fn=fn)
-            if len(filepaths) != 0:
-                fp = [fp[-1]]
-            filepaths.extend(fp)
-
+        filepaths = __download_freesurfer7_extras__(x, experiment_id,
+                                                    destination, resource_name,
+                                                    raw, cache)
     elif 'FREESURFER' in resource_name:
         filepaths = __download_freesurfer__(x, experiment_id, destination,
                                             resource_name, raw, cache)
-        if resource_name == 'FREESURFER7':
-            fn = '%s.hippoAmygLabels-T1.v21.%s.FSvoxelSpace.mgz'
-            for side in ['lh', 'rh']:
-                for each in ['CA', 'HBT', 'FS60']:
-                    fp = __download_freesurfer__(x, experiment_id, destination,
-                                                 resource_name, raw, cache,
-                                                 fn=fn % (side, each))
-                    filepaths.append(fp[-1])
 
     elif 'CAT12' in resource_name:
         if raw:
             fp1 = op.join(destination, '%s_T1.nii.gz' % experiment_id)
             filepaths.append(fp1)
             if not cache:
                 t2_t1space = __get_T1__(x, experiment_id)
@@ -306,15 +352,15 @@
                 msg = 'No such file: \'%s\'. Retry with cache set to False.' % f
                 raise FileNotFoundError(msg)
 
     return filepaths
 
 
 def plot_segment(config, experiment_id, savefig=None, slices=None,
-                 resource_name='SPM12_SEGMENT', fn='aparc+aseg.mgz',
+                 resource_name='SPM12_SEGMENT', extras='brainstem',
                  axes='xyz', raw=True, opacity=70, animated=False,
                  rowsize=None, figsize=None, contours=False, cache=False,
                  samebox=False):
     """Download a given experiment/resource from an XNAT instance and create
     snapshots of this resource along a selected set of slices.
 
     Parameters
@@ -335,15 +381,15 @@
         The indexes of the slices that will be rendered. If None is given, the
         slices are selected automatically.
 
     resource_name: string, optional
         Name of the resource where the segmentation maps are stored in the XNAT
         instance. Default: SPM12_SEGMENT
 
-    fn: string, optional
+    extras: string, optional
         Only for FREESURFER7_EXTRAS. Defines which segmentation should be
         rendered (among 'brainstem', 'thalamus', 'hypothalamus') Default: None
 
     axes: string, or a tuple of strings
         Choose the direction of the cuts (among 'x', 'y', or 'z')
 
     raw: boolean, optional
@@ -399,28 +445,19 @@
     if animated and not raw:
         msg = 'animated cannot be True with raw set to False. ' \
               'Switching raw to True.'
         import logging as log
         log.warning(msg)
         raw = True
 
-    options = ['aparc+aseg.mgz']
-    fn0 = '%s.hippoAmygLabels-T1.v21.%s.FSvoxelSpace.mgz'
-    for side in ['lh', 'rh']:
-        for each in ['CA', 'HBT', 'FS60']:
-            options.append(fn0 % (side, each))
+    options = ('hypothalamus', 'thalamus', 'brainstem')
+
     if resource_name == 'FREESURFER7_EXTRAS':
-        options = ['hypothalamic_subunits_seg.v1.mgz',
-                   'ThalamicNuclei.v12.T1.FSvoxelSpace.mgz',
-                   'brainstemSsLabels.v12.FSvoxelSpace.mgz']
-        if fn not in options:
-            raise Exception('`fn` should be among %s' % options)
-    elif resource_name.startswith('FREESURFER'):
-        if fn not in options:
-            raise Exception('`fn` should be among %s' % options)
+        if extras not in options:
+            raise Exception('`extras` should be among %s' % options)
 
     fp = savefig
     if savefig is None:
         if animated:
             f, fp = tempfile.mkstemp(suffix='.gif')
         else:
             from nisnap.snap import __format__
@@ -434,20 +471,15 @@
                                        dest, raw=raw, cache=cache)
     except FileNotFoundError as exc:
         msg = '{0}. Retry with cache set to False.'.format(exc)
         raise FileNotFoundError(msg)
     bg = filepaths[0]
 
     if resource_name == 'FREESURFER7_EXTRAS':
-        filepaths = [bg, filepaths[options.index(fn) + 1]]
-    elif resource_name.startswith('FREESURFER'):
-        if fn[3:].startswith('hippoAmygLabels'):
-            filepaths = [bg, filepaths[options.index(fn) + 1]]
-        else:
-            filepaths = filepaths[:2]
+        filepaths = [bg, filepaths[options.index(extras) + 1]]
 
     filepaths = filepaths[1] if len(filepaths) == 2 else filepaths[1:]
     from . import snap
     snap.plot_segment(filepaths, axes=axes, bg=bg, opacity=opacity,
                       animated=animated, savefig=fp, figsize=figsize,
                       contours=contours, rowsize=rowsize, slices=slices,
                       samebox=samebox)
```

### Comparing `nisnap-0.4.post0/nisnap.egg-info/PKG-INFO` & `nisnap-0.4a0/nisnap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nisnap
-Version: 0.4.post0
+Version: 0.4a0
 Summary: nisnap
 Home-page: https://github.com/xgrg/nisnap
 Author: Greg Operto
 Author-email: goperto@barcelonabeta.org
 License: UNKNOWN
 Download-URL: https://github.com/xgrg/nisnap/-/archive/v0.4/nisnap-v0.4.tar.gz
 Description: # nisnap
```

### Comparing `nisnap-0.4.post0/setup.py` & `nisnap-0.4a0/setup.py`

 * *Files identical despite different names*

