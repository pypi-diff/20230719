# Comparing `tmp/trackplot-0.2.7.tar.gz` & `tmp/trackplot-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackplot-0.2.7.tar", max compression
+gzip compressed data, was "trackplot-0.2.8.tar", max compression
```

## Comparing `trackplot-0.2.7.tar` & `trackplot-0.2.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1558 2022-12-13 02:20:58.685741 trackplot-0.2.7/LICENSE
--rw-r--r--   0        0        0    12535 2023-07-17 11:41:19.355720 trackplot-0.2.7/README.md
--rw-r--r--   0        0        0     1136 2023-07-17 09:57:45.537804 trackplot-0.2.7/pyproject.toml
--rw-r--r--   0        0        0       38 2023-02-25 03:47:37.462308 trackplot-0.2.7/trackplot/__init__.py
--rw-r--r--   0        0        0      371 2023-02-25 03:47:37.462598 trackplot-0.2.7/trackplot/anno/AxLabel.py
--rw-r--r--   0        0        0        0 2023-02-25 03:47:37.462676 trackplot-0.2.7/trackplot/anno/__init__.py
--rw-r--r--   0        0        0     1545 2023-02-25 03:47:37.462914 trackplot-0.2.7/trackplot/anno/theme.py
--rw-r--r--   0        0        0     7428 2023-02-25 03:47:37.463212 trackplot-0.2.7/trackplot/base/CoordinateMap.py
--rw-r--r--   0        0        0     4425 2023-07-12 04:37:03.080978 trackplot-0.2.7/trackplot/base/GenomicLoci.py
--rw-r--r--   0        0        0     3546 2023-02-25 03:47:37.463862 trackplot-0.2.7/trackplot/base/Junction.py
--rw-r--r--   0        0        0     8881 2023-06-30 06:55:19.943274 trackplot-0.2.7/trackplot/base/Protein.py
--rw-r--r--   0        0        0     8580 2023-06-12 01:40:46.369104 trackplot-0.2.7/trackplot/base/ReadDepth.py
--rw-r--r--   0        0        0     8933 2023-07-17 11:32:19.681424 trackplot-0.2.7/trackplot/base/Readder.py
--rw-r--r--   0        0        0     1368 2023-07-12 04:37:03.081411 trackplot-0.2.7/trackplot/base/Stroke.py
--rw-r--r--   0        0        0     3572 2023-02-25 03:47:37.465151 trackplot-0.2.7/trackplot/base/Transcript.py
--rw-r--r--   0        0        0        0 2023-02-25 03:47:37.465222 trackplot-0.2.7/trackplot/base/__init__.py
--rw-r--r--   0        0        0     7991 2023-06-30 06:55:19.957076 trackplot-0.2.7/trackplot/base/pyUniprot.py
--rw-r--r--   0        0        0    43297 2023-07-17 11:32:19.682002 trackplot-0.2.7/trackplot/cli.py
--rw-r--r--   0        0        0     4745 2023-02-25 03:47:37.466182 trackplot-0.2.7/trackplot/conf/DomainSetting.py
--rw-r--r--   0        0        0        0 2023-02-25 03:47:37.466260 trackplot-0.2.7/trackplot/conf/__init__.py
--rw-r--r--   0        0        0     1330 2023-07-17 11:32:19.682283 trackplot-0.2.7/trackplot/conf/config.py
--rw-r--r--   0        0        0     3803 2023-02-25 03:47:37.466652 trackplot-0.2.7/trackplot/conf/drawing.py
--rw-r--r--   0        0        0     6341 2023-02-26 15:22:54.255231 trackplot-0.2.7/trackplot/file/ATAC.py
--rw-r--r--   0        0        0    21597 2023-07-17 12:26:02.906206 trackplot-0.2.7/trackplot/file/Annotation.py
--rw-r--r--   0        0        0    12907 2023-06-30 06:55:19.953467 trackplot-0.2.7/trackplot/file/Bam.py
--rw-r--r--   0        0        0     1481 2023-02-25 03:47:37.467519 trackplot-0.2.7/trackplot/file/BedGraph.py
--rw-r--r--   0        0        0     1515 2023-02-25 03:47:37.467778 trackplot-0.2.7/trackplot/file/Bigwig.py
--rw-r--r--   0        0        0     2779 2023-02-25 03:47:37.468030 trackplot-0.2.7/trackplot/file/Depth.py
--rw-r--r--   0        0        0     1233 2023-06-30 06:55:19.939595 trackplot-0.2.7/trackplot/file/Fasta.py
--rw-r--r--   0        0        0     3539 2023-07-14 02:17:54.487679 trackplot-0.2.7/trackplot/file/File.py
--rw-r--r--   0        0        0     6413 2023-06-30 06:55:19.949884 trackplot-0.2.7/trackplot/file/HiCMatrixTrack.py
--rw-r--r--   0        0        0      966 2023-02-25 03:47:37.469300 trackplot-0.2.7/trackplot/file/Junction.py
--rw-r--r--   0        0        0     1020 2023-02-25 15:59:51.023722 trackplot-0.2.7/trackplot/file/Motif.py
--rw-r--r--   0        0        0    20423 2023-07-17 11:32:19.682598 trackplot-0.2.7/trackplot/file/ReadSegments.py
--rw-r--r--   0        0        0        0 2023-02-25 03:47:37.470458 trackplot-0.2.7/trackplot/file/__init__.py
--rw-r--r--   0        0        0    47253 2023-07-17 12:28:36.876308 trackplot-0.2.7/trackplot/plot.py
--rw-r--r--   0        0        0    52344 2023-07-17 12:28:14.643398 trackplot-0.2.7/trackplot/plot_func.py
--rw-r--r--   0        0        0     6403 2023-02-25 03:47:37.471775 trackplot-0.2.7/trackplot/plot_tests.py
--rw-r--r--   0        0        0    13892 1970-01-01 00:00:00.000000 trackplot-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1558 2022-12-13 02:20:58.685741 trackplot-0.2.8/LICENSE
+-rw-r--r--   0        0        0    12590 2023-07-18 09:32:04.382841 trackplot-0.2.8/README.md
+-rw-r--r--   0        0        0     1136 2023-07-19 02:21:44.030808 trackplot-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-02-25 03:47:37.462308 trackplot-0.2.8/trackplot/__init__.py
+-rw-r--r--   0        0        0      371 2023-02-25 03:47:37.462598 trackplot-0.2.8/trackplot/anno/AxLabel.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.462676 trackplot-0.2.8/trackplot/anno/__init__.py
+-rw-r--r--   0        0        0     1545 2023-02-25 03:47:37.462914 trackplot-0.2.8/trackplot/anno/theme.py
+-rw-r--r--   0        0        0     7428 2023-02-25 03:47:37.463212 trackplot-0.2.8/trackplot/base/CoordinateMap.py
+-rw-r--r--   0        0        0     4425 2023-07-12 04:37:03.080978 trackplot-0.2.8/trackplot/base/GenomicLoci.py
+-rw-r--r--   0        0        0     3546 2023-02-25 03:47:37.463862 trackplot-0.2.8/trackplot/base/Junction.py
+-rw-r--r--   0        0        0     8881 2023-06-30 06:55:19.943274 trackplot-0.2.8/trackplot/base/Protein.py
+-rw-r--r--   0        0        0     8580 2023-06-12 01:40:46.369104 trackplot-0.2.8/trackplot/base/ReadDepth.py
+-rw-r--r--   0        0        0     8933 2023-07-17 11:32:19.681424 trackplot-0.2.8/trackplot/base/Readder.py
+-rw-r--r--   0        0        0     1368 2023-07-12 04:37:03.081411 trackplot-0.2.8/trackplot/base/Stroke.py
+-rw-r--r--   0        0        0     4254 2023-07-18 09:19:31.032157 trackplot-0.2.8/trackplot/base/Transcript.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.465222 trackplot-0.2.8/trackplot/base/__init__.py
+-rw-r--r--   0        0        0     7991 2023-06-30 06:55:19.957076 trackplot-0.2.8/trackplot/base/pyUniprot.py
+-rw-r--r--   0        0        0    43223 2023-07-18 08:24:36.433824 trackplot-0.2.8/trackplot/cli.py
+-rw-r--r--   0        0        0     4745 2023-02-25 03:47:37.466182 trackplot-0.2.8/trackplot/conf/DomainSetting.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.466260 trackplot-0.2.8/trackplot/conf/__init__.py
+-rw-r--r--   0        0        0     1342 2023-07-18 07:13:43.301559 trackplot-0.2.8/trackplot/conf/config.py
+-rw-r--r--   0        0        0     3803 2023-02-25 03:47:37.466652 trackplot-0.2.8/trackplot/conf/drawing.py
+-rw-r--r--   0        0        0     6341 2023-02-26 15:22:54.255231 trackplot-0.2.8/trackplot/file/ATAC.py
+-rw-r--r--   0        0        0    21613 2023-07-18 08:59:50.143765 trackplot-0.2.8/trackplot/file/Annotation.py
+-rw-r--r--   0        0        0    12907 2023-06-30 06:55:19.953467 trackplot-0.2.8/trackplot/file/Bam.py
+-rw-r--r--   0        0        0     1481 2023-02-25 03:47:37.467519 trackplot-0.2.8/trackplot/file/BedGraph.py
+-rw-r--r--   0        0        0     1515 2023-02-25 03:47:37.467778 trackplot-0.2.8/trackplot/file/Bigwig.py
+-rw-r--r--   0        0        0     2779 2023-02-25 03:47:37.468030 trackplot-0.2.8/trackplot/file/Depth.py
+-rw-r--r--   0        0        0     1233 2023-06-30 06:55:19.939595 trackplot-0.2.8/trackplot/file/Fasta.py
+-rw-r--r--   0        0        0     3539 2023-07-14 02:17:54.487679 trackplot-0.2.8/trackplot/file/File.py
+-rw-r--r--   0        0        0     6413 2023-06-30 06:55:19.949884 trackplot-0.2.8/trackplot/file/HiCMatrixTrack.py
+-rw-r--r--   0        0        0      966 2023-02-25 03:47:37.469300 trackplot-0.2.8/trackplot/file/Junction.py
+-rw-r--r--   0        0        0     1020 2023-02-25 15:59:51.023722 trackplot-0.2.8/trackplot/file/Motif.py
+-rw-r--r--   0        0        0    20423 2023-07-17 11:32:19.682598 trackplot-0.2.8/trackplot/file/ReadSegments.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.470458 trackplot-0.2.8/trackplot/file/__init__.py
+-rw-r--r--   0        0        0    48112 2023-07-19 02:21:44.038340 trackplot-0.2.8/trackplot/plot.py
+-rw-r--r--   0        0        0    52220 2023-07-18 09:30:06.412792 trackplot-0.2.8/trackplot/plot_func.py
+-rw-r--r--   0        0        0     6403 2023-02-25 03:47:37.471775 trackplot-0.2.8/trackplot/plot_tests.py
+-rw-r--r--   0        0        0    13947 1970-01-01 00:00:00.000000 trackplot-0.2.8/PKG-INFO
```

### Comparing `trackplot-0.2.7/LICENSE` & `trackplot-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/README.md` & `trackplot-0.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
 ## Example
 
 The `example` folder is downloaded from [here.](https://github.com/ygidtu/trackplot/archive/refs/heads/main.zip) 
 And a more detailed tutorial could be found at [here.](https://trackplot.readthedocs.io/en/latest/)  
 
 ```bash
 # example of basic plot types
-python main.py \
+python ../main.py \
   -e chr1:1270656-1284730:+ \
   -r example/example.sorted.gtf.gz \
   --interval example/interval_list.tsv \
   --density example/density_list.tsv \
   --show-junction-num \
   --igv example/igv.tsv \
   --heatmap example/heatmap_list.tsv \
@@ -341,14 +341,15 @@
   -o example.png \
   --dpi 300 \
   --width 10 \
   --height 1 \
   --barcode example/barcode_list.tsv \
   --domain --remove-duplicate-umi \
   --normalize-format cpm \
+  --annotation-scale .3 \
   -p 4
 ```
 
 if trackplot was installed by docker, here is the cmd
 
 ```bash
 ## The absolute path is required in Docker env.
@@ -373,14 +374,15 @@
   -o example.png \
   --dpi 300 \
   --width 10 \
   --height 1 \
   --barcode $PWD/example/barcode_list.tsv \
   --domain --remove-duplicate-umi \
   --normalize-format cpm \
+  --annotation-scale .3 \
   -p 4
 
 ```
 
 here is the [output file](https://raw.githubusercontent.com/ygidtu/trackplot/main/example/example.png).
```

### Comparing `trackplot-0.2.7/pyproject.toml` & `trackplot-0.2.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trackplot"
-version = "0.2.7"
+version = "0.2.8"
 description = "The trackplot is a tool for visualizing various next-generation sequencing (NGS) data, including DNA-seq, RNA-seq, single-cell RNA-seq and full-length sequencing datasets. https://sashimi.readthedocs.io/"
 authors = ["ygidtu <ygidtu@gmail.com>"]
 license = "BSD-3"
 readme = "README.md"
 packages = [{include = "trackplot"}]
 
 [tool.poetry.dependencies]
```

### Comparing `trackplot-0.2.7/trackplot/anno/theme.py` & `trackplot-0.2.8/trackplot/anno/theme.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/base/CoordinateMap.py` & `trackplot-0.2.8/trackplot/base/CoordinateMap.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/base/GenomicLoci.py` & `trackplot-0.2.8/trackplot/base/GenomicLoci.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/base/Junction.py` & `trackplot-0.2.8/trackplot/base/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/base/Protein.py` & `trackplot-0.2.8/trackplot/base/Protein.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/base/ReadDepth.py` & `trackplot-0.2.8/trackplot/base/ReadDepth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/base/Readder.py` & `trackplot-0.2.8/trackplot/base/Readder.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/base/Stroke.py` & `trackplot-0.2.8/trackplot/base/Stroke.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/base/Transcript.py` & `trackplot-0.2.8/trackplot/base/Transcript.py`

 * *Files 24% similar despite different names*

```diff
@@ -112,13 +112,37 @@
     def __len__(self):
         return sum(map(lambda x: x[1] - x[0] + 1, self.exon_list))
 
     def __hash__(self):
         exons = sorted([str(x.__hash__()) for x in self.exons])
         return hash((self.chromosome, self.start, self.end, self.strand, " ".join(exons)))
 
+    def __lt__(self, other):
+        if self.chromosome != other.chromosome:
+            return self.chromosome < other.chromosome
+
+        if self.start != other.start:
+            return self.start < other.start
+
+        if self.end != other.end:
+            return self.end < other.end
+
+        return len(self.exons) < len(other.exons)
+
+    def __gt__(self, other):
+        if self.chromosome != other.chromosome:
+            return self.chromosome > other.chromosome
+
+        if self.start != other.start:
+            return self.start > other.start
+
+        if self.end != other.end:
+            return self.end > other.end
+
+        return len(self.exons) > len(other.exons)
+
     def ids(self) -> List[str]:
         return [self.transcript, self.transcript_id, self.gene, self.gene_id]
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `trackplot-0.2.7/trackplot/base/pyUniprot.py` & `trackplot-0.2.8/trackplot/base/pyUniprot.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/cli.py` & `trackplot-0.2.8/trackplot/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,15 @@
 import click
 from click_option_group import optgroup
 from loguru import logger
 
 from trackplot.base.GenomicLoci import GenomicLoci
 from trackplot.conf.config import CLUSTERING_METHOD, COLORS, COLORMAP, DISTANCE_METRIC, IMAGE_TYPE, NORMALIZATION
 from trackplot.file.ATAC import ATAC
-from trackplot.plot import Plot
-
-__version__ = "0.2.7"
-__author__ = "ygidtu & Ran Zhou"
-__email__ = "ygidtu@gmail.com"
+from trackplot.plot import Plot, __version__
 
 
 def decode_region(region: str):
     regions = region.split(":")
 
     if len(regions) < 3:
         strand = "+"
```

### Comparing `trackplot-0.2.7/trackplot/conf/DomainSetting.py` & `trackplot-0.2.8/trackplot/conf/DomainSetting.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/conf/config.py` & `trackplot-0.2.8/trackplot/conf/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'YlOrBr', 'YlOrRd', 'OrRd', 'PuRd', 'RdPu', 'BuPu',
     'GnBu', 'PuBu', 'YlGnBu', 'PuBuGn', 'BuGn', 'YlGn',
     'binary', 'gist_yarg', 'gist_gray', 'gray', 'bone',
     'viridis', 'plasma', 'inferno', 'magma', 'cividis',
     'pink', 'spring', 'summer', 'autumn', 'winter',
     'cool', 'Wistia', 'hot', 'afmhot', 'gist_heat',
     'copper', 'PiYG', 'PRGn', 'BrBG', 'PuOr', 'RdGy', 'RdBu', 'RdYlBu',
-    'RdYlGn', 'Spectral', 'coolwarm', 'bwr', 'seismic'
+    'RdYlGn', 'Spectral', 'coolwarm', 'bwr', 'seismic', "RdYlBu_r"
 ]
 
 DISTANCE_METRIC = [
     "braycurtis", "canberra", "chebyshev",
     "cityblock", "correlation", "cosine",
     "dice", "euclidean", "hamming",
     "jaccard", "jensenshannon", "kulsinski",
```

### Comparing `trackplot-0.2.7/trackplot/conf/drawing.py` & `trackplot-0.2.8/trackplot/conf/drawing.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/file/ATAC.py` & `trackplot-0.2.8/trackplot/file/ATAC.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/file/Annotation.py` & `trackplot-0.2.8/trackplot/file/Annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,26 +60,26 @@
         self.proxy = proxy
         self.timeout = timeout
 
         if proxy:
             logger.info(f"Using proxy: {proxy}")
 
     def __add__(self, other):
-        assert isinstance(other, Reference), "only Reference and Reference could be added"
-        new_ref = Reference(self.path, category=self.category)
+        assert isinstance(other, Annotation), "only Annotation and Annotation could be added"
+        new_ref = Annotation(self.path, category=self.category)
         new_ref.data += self.data
         new_ref.data += other.data
         new_ref.data = sorted(new_ref.data)
 
         new_ref.interval_file.update(other.interval_file)
 
         if self.domain:
             new_ref.__add_domain__()
         if self.add_local_domain:
-            new_ref.__load_local_domain__()
+            new_ref.__load_local_domain__(self.region)
         return new_ref
 
     def len(self, scale: Union[int, float] = .25) -> int:
         u"""
         the length of reference to draw in final plots, default using the quarter of number of transcripts
         """
         size = len(self.data)
@@ -108,15 +108,15 @@
         create reference file object
         :param path: path to input file
         :param add_domain: whether plot domain
         :param add_local_domain: fetch domain information from local file, which download from ucsc
         :param domain_exclude: the domain will be included in reference plot
         :param domain_include: the domain will be excluded in reference plot
         :param category: the type of reference file, include gtf and bam: customized reads as references
-        :return: Reference obj
+        :return: Annotation obj
         """
         assert os.path.exists(path), f"{path} not exists"
 
         if add_local_domain:
             assert os.path.isdir(add_local_domain), f"{add_local_domain} not exists"
 
         return cls(
```

### Comparing `trackplot-0.2.7/trackplot/file/Bam.py` & `trackplot-0.2.8/trackplot/file/Bam.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/file/BedGraph.py` & `trackplot-0.2.8/trackplot/file/BedGraph.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/file/Bigwig.py` & `trackplot-0.2.8/trackplot/file/Bigwig.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/file/Depth.py` & `trackplot-0.2.8/trackplot/file/Depth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/file/Fasta.py` & `trackplot-0.2.8/trackplot/file/Fasta.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/file/File.py` & `trackplot-0.2.8/trackplot/file/File.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/file/HiCMatrixTrack.py` & `trackplot-0.2.8/trackplot/file/HiCMatrixTrack.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/file/Junction.py` & `trackplot-0.2.8/trackplot/file/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/file/Motif.py` & `trackplot-0.2.8/trackplot/file/Motif.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/file/ReadSegments.py` & `trackplot-0.2.8/trackplot/file/ReadSegments.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/trackplot/plot.py` & `trackplot-0.2.8/trackplot/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 from trackplot.plot_func import *
 
 logging.getLogger('matplotlib.font_manager').setLevel(logging.ERROR)
 
 faulthandler.enable()
 
 
+__version__ = "0.2.8"
+__author__ = "ygidtu & Ran Zhou"
+__email__ = "ygidtu@gmail.com"
+
+
 def __load__(args):
     p, args, kwargs = args
     p.load(*args, **kwargs)
     return p
 
 
 class PlotInfo(object):
@@ -140,14 +145,26 @@
 
                 for obj in self.obj:
                     obj.data = data
 
         return self
 
 
+def add_object_error(func):
+    def inner(*args, **kwargs):
+        # calling the actual function now
+        # inside the wrapper function.
+        try:
+            func(*args, **kwargs)
+        except Exception as err:
+            logger.error(f"trackplot will ignore this object, {err}")
+
+    return inner
+
+
 class Plot(object):
     u"""
     this class is the main framework of sashimi
     """
 
     __slots__ = [
         "__n_objs__", "region", "sites",
@@ -174,15 +191,17 @@
         self.graph_coords = None
         self.plots = []
         self.params = {}
         self.junctions = {}
         self.link = []
 
         if logfile:
-            logger.add(logfile, level="TRACE")
+            logger.add(logfile, level="DEBUG")
+
+        logger.info(f"Create trackplot version: {__version__}")
 
         # print warning info about backend
         if backend:
             try:
                 plt.switch_backend(backend)
             except ImportError as err:
                 if backend.lower() == "cairo":
@@ -217,14 +236,15 @@
             return self.region.strand
 
     @property
     def exons(self) -> Optional[List[List[int]]]:
         if self.annotation:
             return self.annotation.exons
 
+    @add_object_error
     def set_region(self, chromosome: str = "",
                    start: int = 0, end: int = 0,
                    strand: str = "+",
                    region: Optional[GenomicLoci] = None):
         u"""
         change the plot region
         """
@@ -232,23 +252,25 @@
         if region:
             self.region = region
         elif chromosome and start and end:
             self.region = GenomicLoci(chromosome, start=start, end=end, strand=strand)
         logger.info(f"set region to {self.region}")
         return self
 
+    @add_object_error
     def add_sites(self, sites):
         u"""
         highlight specific sites
         :param sites: string in 100,200 format or int
         :return:
         """
         assert self.region is not None, f"please set plot region first."
-        logger.info(f"add sites: {sites}")
+
         if sites is not None:
+            logger.info(f"add sites: {sites}")
             if isinstance(sites, str):
                 sites = [int(x) for x in sites.split(",")]
 
                 for s in sites:
                     s = s - self.start
                     if s not in self.sites.keys():
                         self.sites[s] = "blue"
@@ -258,14 +280,15 @@
                 sites = sites - self.start
                 if sites not in self.sites.keys():
                     self.sites[sites] = "blue"
                 else:
                     self.sites[sites] = "red"
         return self
 
+    @add_object_error
     def add_focus(self, focus: Optional[str] = None, start: int = 0, end: int = 0):
         u"""
         set focus region
         :param focus: string in 100-200:300-400
         :param start: start site
         :param end: end site
         :return:
@@ -284,14 +307,15 @@
                 self.focus[site[0]] = max(site[1], self.focus.get(site[0], -1))
 
         if 0 < start < end:
             logger.info(f"add focus: {start}-{end}")
             self.focus[start] = max(end, self.focus.get(start, -1))
         return self
 
+    @add_object_error
     def add_stroke(
             self,
             stroke: Optional[str] = None,
             start: int = 0,
             end: int = 0,
             label: str = "",
             color: str = "black"
@@ -311,14 +335,15 @@
             self.stroke += Stroke.create(stroke, self.region)
 
         if 0 < start < end:
             logger.info(f"add stroke: {start}-{end}")
             self.stroke.append(Stroke(start - self.start, end - self.end, color, label))
         return self
 
+    @add_object_error
     def add_links(
             self,
             link: Optional[str] = None,
             start: int = 0,
             end: int = 0,
             label: str = "",
             color: str = "blue"
@@ -339,24 +364,26 @@
             self.link.append(Stroke.create(link, self.region, default_color=color))
 
         if 0 < start < end:
             logger.info(f"add link: {start}-{end}")
             self.link.append([Stroke(start - self.start, end - self.end, color, label)])
         return self
 
+    @add_object_error
     def set_sequence(self, fasta: str):
         u"""
         set sequence info for
         :param fasta: path to indexed fasta file
         :return:
         """
         logger.info(f"fetch sequence from {fasta}")
         self.sequence = Fasta.create(fasta)
         return self
 
+    @add_object_error
     def set_annotation(self, gtf: str,
                        add_domain: bool = False,
                        local_domain: Optional[str] = False,
                        domain_include: Optional[str] = False,
                        domain_exclude: Optional[str] = False,
                        interval: Optional[str] = None,
                        interval_label: Optional[str] = None,
@@ -418,14 +445,15 @@
             "exon_width": exon_width,
             "show_exon_id": show_exon_id,
             "theme": theme
         }
 
         return self
 
+    @add_object_error
     def add_interval(self, interval: str, interval_label: str):
         assert self.annotation is not None, "please set_annotation first."
         logger.info(f"add interval: {interval} - {interval_label}")
         self.annotation.add_interval(interval, interval_label)
         return self
 
     def __init_input_file__(self, path: str,
@@ -482,15 +510,15 @@
                 label=label,
                 library=library,
                 features=features,
                 deletion_ignore=deletion_ignore,
                 del_ratio_ignore=del_ratio_ignore,
                 exon_focus=exon_focus
             )
-        elif category == "hic":
+        elif category == "hic" or category == "h5":
             obj = HiCTrack.create(
                 path=path,
                 label=label,
                 log_trans=log_trans,
                 depth=depth,
                 tad=tad
             )
@@ -500,23 +528,25 @@
         elif category == "bedgraph" or category == "bg":
             category = "bg"
             obj = Bedgraph.create(path=path, label=label, title=title)
         elif category == "depth":
             obj = Depth.create(path, label=label, title=title)
         else:
             raise ValueError(
-                f"the category should be one of [bam, bigwig, bw, depth, bedgraph, bg], instead of {category}")
+                f"the category should be one of [bam, bigwig, bw, depth, bedgraph, bg, h5], instead of {category}")
 
         obj.log_trans = log_trans
         return obj, category
 
+    @add_object_error
     def add_customized_junctions(self, path: str):
         if path and os.path.exists(path) and os.path.isfile(path):
             self.junctions = load_custom_junction(path)
 
+    @add_object_error
     def add_density(self,
                     path: str,
                     category: str = "bam",
                     size_factor=None,
 
                     # file loading parameters
                     label: Union[str, List[str]] = "",
@@ -586,15 +616,16 @@
             log_trans=log_trans
         )
 
         type_ = "density"
         if show_site_plot and category == "bam":
             type_ = "site-plot"
         elif show_site_plot:
-            logger.debug("show_site_plot only works with bam files")
+            if category != "bam":
+                raise ValueError("show_site_plot only works with bam files")
 
         info = PlotInfo(obj=obj, type_=type_, category=category)
 
         new_obj = True
         for p in self.plots:
             if p.category == info.category:
                 for obj_ in p.obj:
@@ -620,14 +651,15 @@
                 "theme": theme,
                 "strand_choice": strand_choice,
                 "density_by_strand": density_by_strand,
                 "only_customized_junction": only_customized_junction
             }
         return self
 
+    @add_object_error
     def add_heatmap(self,
                     path: str,
                     group: str = "",
                     category: str = "bam",
                     size_factor=None,
 
                     # file loading parameters
@@ -719,14 +751,15 @@
                 "distance_metric": distance_metric,
                 "show_row_names": show_row_names,
                 "vmin": vmin, "vmax": vmax
             }
 
         return self
 
+    @add_object_error
     def add_line(self,
                  path: str,
                  group: str = "",
                  category: str = "bam",
 
                  # file loading parameters
                  label: Union[str, List[str]] = "",
@@ -811,14 +844,15 @@
                 "theme": theme,
                 "legend_position": legend_position,
                 "legend_ncol": legend_ncol
             }
 
         return self
 
+    @add_object_error
     def add_hic(
             self,
             path: str,
             category: str = "hic",
             label: str = "",
             color: str = "RdYlBu_r",
             log_trans: Optional[str] = None,
@@ -846,17 +880,17 @@
             "color": color,
             "y_label": label,
             "font_size": font_size,
             "n_y_ticks": n_y_ticks,
             "show_y_label": show_y_label,
             "theme": theme
         }
-
         return self
 
+    @add_object_error
     def add_igv(
             self,
             path: str,
             category: str = "igv",
             label: str = "",
             exon_focus: Optional[str] = None,
 
@@ -918,14 +952,15 @@
             "n_y_ticks": n_y_ticks,
             "show_y_label": show_y_label,
             "theme": theme
         }
 
         return self
 
+    @add_object_error
     def add_motif(self,
                   path: str,
                   category: str = "motif",
                   motif_region: GenomicLoci = None,
                   width: float = 0.8,
                   theme: str = "blank",
                   **kwargs):
@@ -940,14 +975,15 @@
 
         info = PlotInfo(obj=obj, category=category, type_="motif")
 
         self.plots.append(info)
         self.params[info] = {"width": width, "theme": theme}
         return self
 
+    @add_object_error
     def add_manual(self,
                    data: np.array,
                    image_type: str = "line",
                    label: str = "",
                    group: str = "",
                    color: str = "blue",
                    font_size: int = 8,
@@ -1250,19 +1286,20 @@
             *args, **kwargs
         )
         curr_idx += 1
 
         if self.annotation is not None:
             logger.info(f"plotting annotation at idx: {curr_idx} with height_ratio: {height_ratio[curr_idx]}")
             ax_var = plt.subplot(gs[curr_idx:curr_idx + self.annotation.len(scale=annotation_scale), 0])
-            plot_annotation(ax=ax_var, obj=self.annotation,
-                           graph_coords=self.graph_coords,
-                           plot_domain=self.annotation.add_domain,
-                           distance_between_label_axis=distance_between_label_axis,
-                           **self.params["annotation"])
+            plot_annotation(
+                ax=ax_var, obj=self.annotation,
+                graph_coords=self.graph_coords,
+                plot_domain=self.annotation.add_domain,
+                distance_between_label_axis=distance_between_label_axis,
+                **self.params["annotation"])
 
             # adjust indicator lines and focus background
             set_indicator_lines(ax=ax_var, sites=self.sites, graph_coords=self.graph_coords)
             set_focus(ax=ax_var, focus=self.focus, graph_coords=self.graph_coords)
             curr_idx += self.annotation.len(scale=annotation_scale)
 
         if self.stroke:
```

### Comparing `trackplot-0.2.7/trackplot/plot_func.py` & `trackplot-0.2.8/trackplot/plot_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
         pass
 
     """
     @2018.12.26
     Maybe I'm too stupid for this, using 30% of total length of x axis as the gap between text with axis
     """
 
-    for transcript in obj.data:
+    for transcript in data:
         # ignore the unwanted transcript
         if transcripts and not (set(transcripts) & set(transcript.ids())):
             continue
 
         # ignore transcripts without any exons
         if remove_empty_transcripts and not transcript.exons:
             continue
@@ -490,15 +490,14 @@
                         x = [loc - spread, loc, loc - spread]
                     else:
                         x = [loc + spread, loc, loc + spread]
                     y = [y_loc - exon_width / 5, y_loc, y_loc + exon_width / 5]
                     ax.plot(x, y, lw=.5, color=color, rasterized=raster)
 
         y_loc += 1  # if transcript.transcript else .5
-
         if plot_domain and obj.domain and transcript.transcript_id in obj.domain.pep:
             current_domains = obj.domain.pep[transcript.transcript_id]
 
             for sub_current_domain in current_domains:
                 if not (sub_current_domain.start <= region.end and
                         sub_current_domain.end >= region.start):
                     continue
@@ -517,16 +516,15 @@
                             graph_coords[s], graph_coords[e],
                             graph_coords[e], graph_coords[s]
                         ]
                         y = [
                             y_loc - exon_width / 4, y_loc - exon_width / 4,
                             y_loc + exon_width / 4, y_loc + exon_width / 4
                         ]
-                        ax.fill(x, y, color, lw=.5,
-                                zorder=20, rasterized=raster)
+                        ax.fill(x, y, color, lw=.5, zorder=20, rasterized=raster)
 
                     # @2022.05.13
                     intron_relative_s = region.relative(
                         min(map(lambda x_: x_.end, sub_exon)))
                     intron_relative_s = intron_relative_s if intron_relative_s >= 0 else 0
                     if intron_relative_s > len(region):
                         continue
@@ -537,27 +535,25 @@
                         region) - 1 if intron_relative_e > len(region) else intron_relative_e
                     if intron_relative_e <= 0:
                         continue
 
                     intron_sites = [graph_coords[intron_relative_s],
                                     graph_coords[intron_relative_e]]
                     if len(sub_exon) != 1:
-                        ax.plot(intron_sites, [y_loc, y_loc],
-                                color=color, lw=0.2, rasterized=raster)
+                        ax.plot(intron_sites, [y_loc, y_loc], color=color, lw=0.2, rasterized=raster)
+
                 if show_id:
                     ax.text(x=-1, y=y_loc - 0.125, s=f"{sub_current_domain.gene}|{transcript.transcript_id}",
                             fontsize=font_size / 2, ha="right")
                 else:
                     ax.text(x=-1, y=y_loc - 0.125, s=f"{sub_current_domain.gene}|{transcript.transcript}",
                             fontsize=font_size / 2, ha="right")
 
-                y_loc += 0.25
+                y_loc += .5
 
-        # offset for next term.
-        y_loc += 0.75
     if obj.local_domain:
         for base_name, current_domain in obj.local_domain.items():
             for sub_current_domain in current_domain:
                 if not (sub_current_domain.start <= region.end and
                         sub_current_domain.end >= region.start):
                     continue
```

### Comparing `trackplot-0.2.7/trackplot/plot_tests.py` & `trackplot-0.2.8/trackplot/plot_tests.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.7/PKG-INFO` & `trackplot-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackplot
-Version: 0.2.7
+Version: 0.2.8
 Summary: The trackplot is a tool for visualizing various next-generation sequencing (NGS) data, including DNA-seq, RNA-seq, single-cell RNA-seq and full-length sequencing datasets. https://sashimi.readthedocs.io/
 License: BSD-3
 Author: ygidtu
 Author-email: ygidtu@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -354,15 +354,15 @@
 ## Example
 
 The `example` folder is downloaded from [here.](https://github.com/ygidtu/trackplot/archive/refs/heads/main.zip) 
 And a more detailed tutorial could be found at [here.](https://trackplot.readthedocs.io/en/latest/)  
 
 ```bash
 # example of basic plot types
-python main.py \
+python ../main.py \
   -e chr1:1270656-1284730:+ \
   -r example/example.sorted.gtf.gz \
   --interval example/interval_list.tsv \
   --density example/density_list.tsv \
   --show-junction-num \
   --igv example/igv.tsv \
   --heatmap example/heatmap_list.tsv \
@@ -373,14 +373,15 @@
   -o example.png \
   --dpi 300 \
   --width 10 \
   --height 1 \
   --barcode example/barcode_list.tsv \
   --domain --remove-duplicate-umi \
   --normalize-format cpm \
+  --annotation-scale .3 \
   -p 4
 ```
 
 if trackplot was installed by docker, here is the cmd
 
 ```bash
 ## The absolute path is required in Docker env.
@@ -405,14 +406,15 @@
   -o example.png \
   --dpi 300 \
   --width 10 \
   --height 1 \
   --barcode $PWD/example/barcode_list.tsv \
   --domain --remove-duplicate-umi \
   --normalize-format cpm \
+  --annotation-scale .3 \
   -p 4
 
 ```
 
 here is the [output file](https://raw.githubusercontent.com/ygidtu/trackplot/main/example/example.png).
```

