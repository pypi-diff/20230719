# Comparing `tmp/ephysio-1.0.6.tar.gz` & `tmp/ephysio-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysio-1.0.6.tar", last modified: Tue Jul 11 20:58:21 2023, max compression
+gzip compressed data, was "ephysio-1.0.7.tar", last modified: Tue Jul 18 22:51:54 2023, max compression
```

## Comparing `ephysio-1.0.6.tar` & `ephysio-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-11 20:58:21.292050 ephysio-1.0.6/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    35149 2023-01-11 21:50:43.000000 ephysio-1.0.6/LICENSE
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-11 20:58:21.292050 ephysio-1.0.6/PKG-INFO
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1203 2023-01-11 21:50:43.000000 ephysio-1.0.6/README.md
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-11 20:58:21.288050 ephysio-1.0.6/ephysio/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        3 2023-07-07 19:58:47.000000 ephysio-1.0.6/ephysio/__init__.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    12774 2023-07-09 17:40:03.000000 ephysio-1.0.6/ephysio/kilosortIO.py
--rw-------   0 wagenaar  (1000) wagenaar  (1000)    58904 2023-07-10 01:01:39.000000 ephysio-1.0.6/ephysio/openEphysIO.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6370 2023-07-10 01:06:33.000000 ephysio-1.0.6/ephysio/spikestats.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17733 2023-07-09 15:35:19.000000 ephysio-1.0.6/ephysio/vizio.py
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6897 2023-07-10 20:43:28.000000 ephysio-1.0.6/ephysio/vizly.py
-drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-11 20:58:21.292050 ephysio-1.0.6/ephysio.egg-info/
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-11 20:58:21.000000 ephysio-1.0.6/ephysio.egg-info/PKG-INFO
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      307 2023-07-11 20:58:21.000000 ephysio-1.0.6/ephysio.egg-info/SOURCES.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-07-11 20:58:21.000000 ephysio-1.0.6/ephysio.egg-info/dependency_links.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        6 2023-07-11 20:58:21.000000 ephysio-1.0.6/ephysio.egg-info/requires.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-07-11 20:58:21.000000 ephysio-1.0.6/ephysio.egg-info/top_level.txt
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      297 2023-07-11 20:58:13.000000 ephysio-1.0.6/pyproject.toml
--rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-07-11 20:58:21.292050 ephysio-1.0.6/setup.cfg
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-18 22:51:54.627983 ephysio-1.0.7/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    35149 2023-01-11 21:50:43.000000 ephysio-1.0.7/LICENSE
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-18 22:51:54.627983 ephysio-1.0.7/PKG-INFO
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1203 2023-01-11 21:50:43.000000 ephysio-1.0.7/README.md
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-18 22:51:54.623983 ephysio-1.0.7/ephysio/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        3 2023-07-18 20:27:55.000000 ephysio-1.0.7/ephysio/__init__.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    12870 2023-07-18 22:50:35.000000 ephysio-1.0.7/ephysio/kilosortIO.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    58904 2023-07-18 22:50:45.000000 ephysio-1.0.7/ephysio/openEphysIO.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6400 2023-07-18 22:48:44.000000 ephysio-1.0.7/ephysio/spikestats.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)    17733 2023-07-18 20:27:55.000000 ephysio-1.0.7/ephysio/vizio.py
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     6897 2023-07-18 20:27:55.000000 ephysio-1.0.7/ephysio/vizly.py
+drwxrwxr-x   0 wagenaar  (1000) wagenaar  (1000)        0 2023-07-18 22:51:54.627983 ephysio-1.0.7/ephysio.egg-info/
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)     1403 2023-07-18 22:51:54.000000 ephysio-1.0.7/ephysio.egg-info/PKG-INFO
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      307 2023-07-18 22:51:54.000000 ephysio-1.0.7/ephysio.egg-info/SOURCES.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        1 2023-07-18 22:51:54.000000 ephysio-1.0.7/ephysio.egg-info/dependency_links.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        6 2023-07-18 22:51:54.000000 ephysio-1.0.7/ephysio.egg-info/requires.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)        8 2023-07-18 22:51:54.000000 ephysio-1.0.7/ephysio.egg-info/top_level.txt
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)      297 2023-07-18 22:49:05.000000 ephysio-1.0.7/pyproject.toml
+-rw-rw-r--   0 wagenaar  (1000) wagenaar  (1000)       38 2023-07-18 22:51:54.627983 ephysio-1.0.7/setup.cfg
```

### Comparing `ephysio-1.0.6/LICENSE` & `ephysio-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.6/PKG-INFO` & `ephysio-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysio
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tools for reading ephys data
 Author-email: Daniel Wagenaar <daw@caltech.edu>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ephysio
 Python code for reading ephys files
```

### Comparing `ephysio-1.0.6/README.md` & `ephysio-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.6/ephysio/kilosortIO.py` & `ephysio-1.0.7/ephysio/kilosortIO.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,30 +142,31 @@
             return dd[0]
         else:
             return np.nan
 
     def allspikes(self):
         '''ALLSPIKES - Times and cluster numbers for all spikes
         tms, cls = ALLSPIKES() returns time stamps in samples and cluster 
-        numbers (counted from 0) as two numpy vectors.'''
+        numbers (counted from 0) as two numpy vectors.
+        Caution: Results are not necessarily in cluster or time order.'''
         return self.spk_tms, self.spk_cls
 
     def nclusters(self):
         '''NCLUSTERS - Return number of clusters'''
         return self.tmpls.shape[0]
 
     def nchannels(self):
         '''NCHANELS - Return number of channels'''
         return len(self.chan2elc)
 
     def spikesforcluster(self, k):
         '''SPIKESFORCLUSTER - Times of spikes for given cluster
         tms = SPIKESFORCLUSTER(k) returns the spike times (in samples) 
-        for cluster k.'''
-        return self.spk_tms[self.spk_cls==k]
+        for cluster k, sorted by time.'''
+        return np.sort(self.spk_tms[self.spk_cls==k])
 
     def spikesbycluster(self, label=None):
         '''SPIKESBYCLUSTER - Map of spike times for all clusters
         SPIKEBYCLUSTER() returns a dict of cluster number to vector of 
         spike times.
         Optional argument LABEL specifies that clusters must have the given 
         label to be included in the dict.'''
```

### Comparing `ephysio-1.0.6/ephysio/openEphysIO.py` & `ephysio-1.0.7/ephysio/openEphysIO.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,15 +520,15 @@
         if len(ss) == 18 and ud[0] == 1 and not np.any(np.diff(ud) == 0):
             # Potential barcode
             s0 = ss[0]
             dss = np.diff(ss)
             code = 0
             onems = dss[0] / 10
             thr = dss[0] * 3 // 4
-            if np.any(dss < 3 * onems) or np.any(dss > 12 * onems):
+            if np.any(dss < 3 * onems) or np.any(dss > 14 * onems):
                 noth += 1
             else:
                 nbar += 1
                 for ds in dss[1:]:
                     code *= 2
                     if ds > thr:
                         code += 1
```

### Comparing `ephysio-1.0.6/ephysio/spikestats.py` & `ephysio-1.0.7/ephysio/spikestats.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,18 @@
         if stim_idx is not None:
             if selector is not None:
                 self.stim_s = np.array([t for t,idx in zip(stim_s, stim_idx) if selector(idx)])
                 self.stim_idx = [idx for idx in stim_idx if selector(idx)]
             ndims = 0
             for idx in stim_idx:
                 if idx is not None:
-                    if type(idx)==list or type(idx)==tuple:
+                    if type(idx)==list or type(idx)==tuple or type(idx)==np.ndarray:
                         ndims = len(idx)
                         break
-            shape = np.zeros(ndims, np.int)
+            shape = np.zeros(ndims, int)
             for idx in stim_idx:
                 if idx is not None:
                     for dim in range(ndims):
                         if idx[dim] >= shape[dim]:
                             shape[dim] = idx[dim] + 1
             self.idx_shape = shape
         else:
@@ -101,25 +101,25 @@
     def trialcounts(self):
         '''TRIALCOUNTS - Count trials by type
         nnn = TRIALCOUNTS() returns a tensor of occurrences of each trial type, or None if no trial
         types were passed into the constructor.
         '''
         if self.stim_idx is None:
             raise Exception("Calculating trial counts by type requires knowing a trial type (idx)")
-        nnn = np.zeros(self.idx_shape, np.int)
+        nnn = np.zeros(self.idx_shape, int)
         for idx in self.stim_idx:
             if idx is not None:
-                nnn[idx] += 1
+                nnn[tuple(idx)] += 1
         return nnn
 
     def totalspikecountsbytrialtype(self, celid, dt_start_ms=-50, dt_end_ms=150):
         '''TOTALSPIKECOUNTSBYTRIALTYPE - As SPIKECOUNTS, but accumulates over trials of the same type.
         Use TRIALCOUNTS to find out how many trials of the type there are, if you need to get
         averagecounts.'''
         if self.stim_idx is None:
             raise Exception("Calculating spike counts by trial type requires knowing a trial type (idx)")
         nn = self.spikecounts(celid, dt_start_ms, dt_end_ms)
-        nnn = np.zeros(self.idx_shape, np.int)
+        nnn = np.zeros(self.idx_shape, int)
         for n, idx in zip(nn, self.stim_idx):
             if idx is not None:
-                nnn[idx] += n
+                nnn[tuple(idx)] += n
         return nnn
```

### Comparing `ephysio-1.0.6/ephysio/vizio.py` & `ephysio-1.0.7/ephysio/vizio.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.6/ephysio/vizly.py` & `ephysio-1.0.7/ephysio/vizly.py`

 * *Files identical despite different names*

### Comparing `ephysio-1.0.6/ephysio.egg-info/PKG-INFO` & `ephysio-1.0.7/ephysio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysio
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tools for reading ephys data
 Author-email: Daniel Wagenaar <daw@caltech.edu>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ephysio
 Python code for reading ephys files
```

