# Comparing `tmp/trackplot-0.2.8.tar.gz` & `tmp/trackplot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackplot-0.2.8.tar", max compression
+gzip compressed data, was "trackplot-0.3.0.tar", max compression
```

## Comparing `trackplot-0.2.8.tar` & `trackplot-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1558 2022-12-13 02:20:58.685741 trackplot-0.2.8/LICENSE
--rw-r--r--   0        0        0    12590 2023-07-18 09:32:04.382841 trackplot-0.2.8/README.md
--rw-r--r--   0        0        0     1136 2023-07-19 02:21:44.030808 trackplot-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       38 2023-02-25 03:47:37.462308 trackplot-0.2.8/trackplot/__init__.py
--rw-r--r--   0        0        0      371 2023-02-25 03:47:37.462598 trackplot-0.2.8/trackplot/anno/AxLabel.py
--rw-r--r--   0        0        0        0 2023-02-25 03:47:37.462676 trackplot-0.2.8/trackplot/anno/__init__.py
--rw-r--r--   0        0        0     1545 2023-02-25 03:47:37.462914 trackplot-0.2.8/trackplot/anno/theme.py
--rw-r--r--   0        0        0     7428 2023-02-25 03:47:37.463212 trackplot-0.2.8/trackplot/base/CoordinateMap.py
--rw-r--r--   0        0        0     4425 2023-07-12 04:37:03.080978 trackplot-0.2.8/trackplot/base/GenomicLoci.py
--rw-r--r--   0        0        0     3546 2023-02-25 03:47:37.463862 trackplot-0.2.8/trackplot/base/Junction.py
--rw-r--r--   0        0        0     8881 2023-06-30 06:55:19.943274 trackplot-0.2.8/trackplot/base/Protein.py
--rw-r--r--   0        0        0     8580 2023-06-12 01:40:46.369104 trackplot-0.2.8/trackplot/base/ReadDepth.py
--rw-r--r--   0        0        0     8933 2023-07-17 11:32:19.681424 trackplot-0.2.8/trackplot/base/Readder.py
--rw-r--r--   0        0        0     1368 2023-07-12 04:37:03.081411 trackplot-0.2.8/trackplot/base/Stroke.py
--rw-r--r--   0        0        0     4254 2023-07-18 09:19:31.032157 trackplot-0.2.8/trackplot/base/Transcript.py
--rw-r--r--   0        0        0        0 2023-02-25 03:47:37.465222 trackplot-0.2.8/trackplot/base/__init__.py
--rw-r--r--   0        0        0     7991 2023-06-30 06:55:19.957076 trackplot-0.2.8/trackplot/base/pyUniprot.py
--rw-r--r--   0        0        0    43223 2023-07-18 08:24:36.433824 trackplot-0.2.8/trackplot/cli.py
--rw-r--r--   0        0        0     4745 2023-02-25 03:47:37.466182 trackplot-0.2.8/trackplot/conf/DomainSetting.py
--rw-r--r--   0        0        0        0 2023-02-25 03:47:37.466260 trackplot-0.2.8/trackplot/conf/__init__.py
--rw-r--r--   0        0        0     1342 2023-07-18 07:13:43.301559 trackplot-0.2.8/trackplot/conf/config.py
--rw-r--r--   0        0        0     3803 2023-02-25 03:47:37.466652 trackplot-0.2.8/trackplot/conf/drawing.py
--rw-r--r--   0        0        0     6341 2023-02-26 15:22:54.255231 trackplot-0.2.8/trackplot/file/ATAC.py
--rw-r--r--   0        0        0    21613 2023-07-18 08:59:50.143765 trackplot-0.2.8/trackplot/file/Annotation.py
--rw-r--r--   0        0        0    12907 2023-06-30 06:55:19.953467 trackplot-0.2.8/trackplot/file/Bam.py
--rw-r--r--   0        0        0     1481 2023-02-25 03:47:37.467519 trackplot-0.2.8/trackplot/file/BedGraph.py
--rw-r--r--   0        0        0     1515 2023-02-25 03:47:37.467778 trackplot-0.2.8/trackplot/file/Bigwig.py
--rw-r--r--   0        0        0     2779 2023-02-25 03:47:37.468030 trackplot-0.2.8/trackplot/file/Depth.py
--rw-r--r--   0        0        0     1233 2023-06-30 06:55:19.939595 trackplot-0.2.8/trackplot/file/Fasta.py
--rw-r--r--   0        0        0     3539 2023-07-14 02:17:54.487679 trackplot-0.2.8/trackplot/file/File.py
--rw-r--r--   0        0        0     6413 2023-06-30 06:55:19.949884 trackplot-0.2.8/trackplot/file/HiCMatrixTrack.py
--rw-r--r--   0        0        0      966 2023-02-25 03:47:37.469300 trackplot-0.2.8/trackplot/file/Junction.py
--rw-r--r--   0        0        0     1020 2023-02-25 15:59:51.023722 trackplot-0.2.8/trackplot/file/Motif.py
--rw-r--r--   0        0        0    20423 2023-07-17 11:32:19.682598 trackplot-0.2.8/trackplot/file/ReadSegments.py
--rw-r--r--   0        0        0        0 2023-02-25 03:47:37.470458 trackplot-0.2.8/trackplot/file/__init__.py
--rw-r--r--   0        0        0    48112 2023-07-19 02:21:44.038340 trackplot-0.2.8/trackplot/plot.py
--rw-r--r--   0        0        0    52220 2023-07-18 09:30:06.412792 trackplot-0.2.8/trackplot/plot_func.py
--rw-r--r--   0        0        0     6403 2023-02-25 03:47:37.471775 trackplot-0.2.8/trackplot/plot_tests.py
--rw-r--r--   0        0        0    13947 1970-01-01 00:00:00.000000 trackplot-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1558 2022-12-13 02:20:58.685741 trackplot-0.3.0/LICENSE
+-rw-r--r--   0        0        0    13104 2023-07-19 08:48:46.403424 trackplot-0.3.0/README.md
+-rw-r--r--   0        0        0     1136 2023-07-19 08:18:41.634320 trackplot-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-02-25 03:47:37.462308 trackplot-0.3.0/trackplot/__init__.py
+-rw-r--r--   0        0        0      371 2023-02-25 03:47:37.462598 trackplot-0.3.0/trackplot/anno/AxLabel.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.462676 trackplot-0.3.0/trackplot/anno/__init__.py
+-rw-r--r--   0        0        0     1545 2023-02-25 03:47:37.462914 trackplot-0.3.0/trackplot/anno/theme.py
+-rw-r--r--   0        0        0     7428 2023-02-25 03:47:37.463212 trackplot-0.3.0/trackplot/base/CoordinateMap.py
+-rw-r--r--   0        0        0     4425 2023-07-12 04:37:03.080978 trackplot-0.3.0/trackplot/base/GenomicLoci.py
+-rw-r--r--   0        0        0     3546 2023-02-25 03:47:37.463862 trackplot-0.3.0/trackplot/base/Junction.py
+-rw-r--r--   0        0        0     8881 2023-06-30 06:55:19.943274 trackplot-0.3.0/trackplot/base/Protein.py
+-rw-r--r--   0        0        0     8580 2023-06-12 01:40:46.369104 trackplot-0.3.0/trackplot/base/ReadDepth.py
+-rw-r--r--   0        0        0     8933 2023-07-17 11:32:19.681424 trackplot-0.3.0/trackplot/base/Readder.py
+-rw-r--r--   0        0        0     1368 2023-07-12 04:37:03.081411 trackplot-0.3.0/trackplot/base/Stroke.py
+-rw-r--r--   0        0        0     4254 2023-07-18 09:19:31.032157 trackplot-0.3.0/trackplot/base/Transcript.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.465222 trackplot-0.3.0/trackplot/base/__init__.py
+-rw-r--r--   0        0        0     7991 2023-06-30 06:55:19.957076 trackplot-0.3.0/trackplot/base/pyUniprot.py
+-rw-r--r--   0        0        0    43183 2023-07-19 07:55:15.270105 trackplot-0.3.0/trackplot/cli.py
+-rw-r--r--   0        0        0     4745 2023-02-25 03:47:37.466182 trackplot-0.3.0/trackplot/conf/DomainSetting.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.466260 trackplot-0.3.0/trackplot/conf/__init__.py
+-rw-r--r--   0        0        0     1342 2023-07-18 07:13:43.301559 trackplot-0.3.0/trackplot/conf/config.py
+-rw-r--r--   0        0        0     3803 2023-02-25 03:47:37.466652 trackplot-0.3.0/trackplot/conf/drawing.py
+-rw-r--r--   0        0        0     6341 2023-02-26 15:22:54.255231 trackplot-0.3.0/trackplot/file/ATAC.py
+-rw-r--r--   0        0        0    23346 2023-07-19 08:14:18.002701 trackplot-0.3.0/trackplot/file/Annotation.py
+-rw-r--r--   0        0        0    12907 2023-06-30 06:55:19.953467 trackplot-0.3.0/trackplot/file/Bam.py
+-rw-r--r--   0        0        0     1481 2023-02-25 03:47:37.467519 trackplot-0.3.0/trackplot/file/BedGraph.py
+-rw-r--r--   0        0        0     1515 2023-02-25 03:47:37.467778 trackplot-0.3.0/trackplot/file/Bigwig.py
+-rw-r--r--   0        0        0     2779 2023-02-25 03:47:37.468030 trackplot-0.3.0/trackplot/file/Depth.py
+-rw-r--r--   0        0        0     1233 2023-06-30 06:55:19.939595 trackplot-0.3.0/trackplot/file/Fasta.py
+-rw-r--r--   0        0        0     3539 2023-07-14 02:17:54.487679 trackplot-0.3.0/trackplot/file/File.py
+-rw-r--r--   0        0        0     6413 2023-06-30 06:55:19.949884 trackplot-0.3.0/trackplot/file/HiCMatrixTrack.py
+-rw-r--r--   0        0        0      966 2023-02-25 03:47:37.469300 trackplot-0.3.0/trackplot/file/Junction.py
+-rw-r--r--   0        0        0     1020 2023-02-25 15:59:51.023722 trackplot-0.3.0/trackplot/file/Motif.py
+-rw-r--r--   0        0        0    20423 2023-07-17 11:32:19.682598 trackplot-0.3.0/trackplot/file/ReadSegments.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.470458 trackplot-0.3.0/trackplot/file/__init__.py
+-rw-r--r--   0        0        0    48131 2023-07-19 08:18:31.127302 trackplot-0.3.0/trackplot/plot.py
+-rw-r--r--   0        0        0    51055 2023-07-19 08:16:55.995028 trackplot-0.3.0/trackplot/plot_func.py
+-rw-r--r--   0        0        0     6403 2023-02-25 03:47:37.471775 trackplot-0.3.0/trackplot/plot_tests.py
+-rw-r--r--   0        0        0    14461 1970-01-01 00:00:00.000000 trackplot-0.3.0/PKG-INFO
```

### Comparing `trackplot-0.2.8/LICENSE` & `trackplot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/README.md` & `trackplot-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 Prior to installing the tool from the source code, users should verify their Python version (>=3.8).
 
 ```bash
 python --version
 # Python 3.10.8
 ```
 
-4.1 python3 is not available 
+    4.1 python3 is not available 
 
 If your Python version does not match the requirements of Trackplot, 
 users could follow the cmd to install and 
 more detailed instruction for different system please refer to [here](https://realpython.com/installing-python/).  
 
 ```bash
 # If the default Python version does not meet the requirements of Trackplot, 
@@ -163,15 +163,15 @@
 $PWD/Python-3.10.12/python -m pip install -e trackplot/
 
 # 3. check trackplot
 $PWD/Python-3.10.12/Python-3.10.12/Python/bin/trackplot --help
 
 ```
 
-4.2 python3 is available
+    4.2 python3 is available
 
 ```bash
 # 1. download the trackplot
 git clone https://github.com/ygidtu/trackplot trackplot
 cd trackplot
 
 # 2. install the trackplot and it's requirements to python env
@@ -254,19 +254,19 @@
 
 # or just run with poetry
 poetry run python main.py --help
 ```
 
 ### Using trackplot by a local webserver
 
-1. using AppImage (Linux x86_64 only)
+1. [AppImage](https://github.com/ygidtu/trackplot/releases) (Linux x86_64 only)
 
 ```bash
-# example with version v0.2.6, please using your interested version according to your needs
-export VERSION=0.2.6
+# example with version v0.3.0, please using your interested version according to your needs
+export VERSION=0.3.0
 gunzip trackplotweb-${VERSION}-x86_64.AppImage
 chmod +x trackplotweb-${VERSION}-x86_64.AppImage
 ./trackplotweb-${VERSION}-x86_64.AppImage --help
 
 # startup webserver
 ./trackplotweb-${VERSION}-x86_64.AppImage --host 127.0.0.1 --port 5000 --plots ./plots
 ```
@@ -280,24 +280,33 @@
    
 ```bash
 docker pull ygidtu/trackplotweb
 
 # -v map the current working directory into docker containers
 # -p map the outer port to inner port of docker container
 docker run --name trackplotweb \
- --rm -v $PWD:$PWD \
- -p 5000:5000 \
- ygidtu/trackplotweb
+  --rm \
+  -v $PWD/data:/data \
+  -v $PWD/plots/:/plots
+  -p 5000:5000 \
+  --data /data \
+  --plots /plots \
+  ygidtu/trackplotweb 
 ```
 
+`-p`: public and private port for the server, default:5000(public):5000(private)
+- `-v`, `--volume`: mount the working directory to docker container, for example, the `$PWD/data` could replace by the path to your directory contains all necessary data
+- `--user`: prevent docker read and write file using root privileges
+- the rest usage please check [Command line usage](./command.md)
+
 ---
 
 3. Install from source code
 
-Before this, please make sure that trackplot has been properly installed in your env.  
+Before this, please make sure that trackplot has been properly installed in the same env.  
 
 
 ```bash
 git clone https://github.com/ygidtu/trackplot trackplot
 cd trackplot/web
 
 # build the frontend static files; If npm was not found, please install nodejs(https://nodejs.org).
```

### Comparing `trackplot-0.2.8/pyproject.toml` & `trackplot-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trackplot"
-version = "0.2.8"
+version = "0.3.0"
 description = "The trackplot is a tool for visualizing various next-generation sequencing (NGS) data, including DNA-seq, RNA-seq, single-cell RNA-seq and full-length sequencing datasets. https://sashimi.readthedocs.io/"
 authors = ["ygidtu <ygidtu@gmail.com>"]
 license = "BSD-3"
 readme = "README.md"
 packages = [{include = "trackplot"}]
 
 [tool.poetry.dependencies]
```

### Comparing `trackplot-0.2.8/trackplot/anno/theme.py` & `trackplot-0.3.0/trackplot/anno/theme.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/base/CoordinateMap.py` & `trackplot-0.3.0/trackplot/base/CoordinateMap.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/base/GenomicLoci.py` & `trackplot-0.3.0/trackplot/base/GenomicLoci.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/base/Junction.py` & `trackplot-0.3.0/trackplot/base/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/base/Protein.py` & `trackplot-0.3.0/trackplot/base/Protein.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/base/ReadDepth.py` & `trackplot-0.3.0/trackplot/base/ReadDepth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/base/Readder.py` & `trackplot-0.3.0/trackplot/base/Readder.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/base/Stroke.py` & `trackplot-0.3.0/trackplot/base/Stroke.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/base/Transcript.py` & `trackplot-0.3.0/trackplot/base/Transcript.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/base/pyUniprot.py` & `trackplot-0.3.0/trackplot/base/pyUniprot.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/cli.py` & `trackplot-0.3.0/trackplot/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,14 @@
     size_factors = {}
 
     # add annotation
     # print(kwargs.keys())
     for key in kwargs.keys():
         if key in IMAGE_TYPE and kwargs[key] and os.path.exists(kwargs[key]):
             if key == "annotation":
-                print("set_annotation")
                 p.set_annotation(kwargs["annotation"],
                                  show_gene=not kwargs["no_gene"],
                                  color=kwargs["ref_color"],
                                  remove_empty_transcripts=kwargs["remove_empty"],
                                  choose_primary=kwargs["choose_primary"],
                                  font_size=kwargs["font_size"],
                                  show_id=kwargs["show_id"],
```

### Comparing `trackplot-0.2.8/trackplot/conf/DomainSetting.py` & `trackplot-0.3.0/trackplot/conf/DomainSetting.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/conf/config.py` & `trackplot-0.3.0/trackplot/conf/config.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/conf/drawing.py` & `trackplot-0.3.0/trackplot/conf/drawing.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/file/ATAC.py` & `trackplot-0.3.0/trackplot/file/ATAC.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/file/Annotation.py` & `trackplot-0.3.0/trackplot/file/Annotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -345,31 +345,31 @@
                 pysam.tabix_index(sorted_gtf, preset="gff", force=True, keep_original=True)
                 return sorted_gtf
         elif os.path.getctime(output_gtf) < os.path.getctime(output_gtf):
             logger.info("the tbi index is older than the gtf file")
 
         return output_gtf
 
-    def __load_gtf__(self, region: GenomicLoci) -> List[Transcript]:
+    def __load_gtf__(self):
 
         u"""
         Load transcripts inside of region from gtf file
         :param region: target region
         :return: list of Transcript
         """
         transcripts = {}
         exons = {}
 
-        for rec in Reader.read_gtf(self.path, region):
-            start = max(rec.start, region.start)
-            end = min(rec.end, region.end)
+        for rec in Reader.read_gtf(self.path, self.region):
+            start = max(rec.start, self.region.start)
+            end = min(rec.end, self.region.end)
 
-            if end + 1 <= region.start:
+            if end + 1 <= self.region.start:
                 continue
-            if start + 1 >= region.end:
+            if start + 1 >= self.region.end:
                 break
 
             if re.search(r"(rna|transcript|cds)", rec.feature, re.I):
                 if rec.transcript_id not in transcripts.keys():
                     transcripts[rec.transcript_id] = Transcript(
                         chromosome=rec.contig,
                         start=start,
@@ -384,74 +384,72 @@
             elif re.search(r"(exon)", rec.feature, re.I):
                 if rec.transcript_id not in exons.keys():
                     exons[rec.transcript_id] = []
 
                 exons[rec.transcript_id].append(
                     GenomicLoci(
                         chromosome=rec.contig,
-                        start=start,
-                        end=end,
-                        strand=rec.strand
+                        start=start, end=end,
+                        strand=rec.strand,
+                        name=rec.exon_id
                     )
                 )
 
         for key, trans in transcripts.items():
             if key in exons.keys():
                 trans.exons += exons[key]
 
-        return sorted(transcripts.values())
+        self.data += sorted(transcripts.values())
 
-    def __load_bam__(self, region: GenomicLoci, threshold_of_reads: int = 0) -> List[Transcript]:
+    def __load_bam__(self, threshold_of_reads: int = 0):
         u"""
         Load transcripts inside of region from bam file
-        :param region: target region
         :param threshold_of_reads: only kept reads with minimum frequency
         :return: list of Transcript
         """
         transcripts = {}
         try:
-            for read, strand in Reader.read_bam(self.path, region):
+            for read, strand in Reader.read_bam(self.path, self.region):
                 start = read.reference_start
 
                 exons_in_read = []
                 for cigar, length in read.cigartuples:
                     cur_start = start + 1
                     cur_end = start + length + 1
 
                     if cigar == 0:  # M
-                        if cur_start < region.end < cur_end:
+                        if cur_start < self.region.end < cur_end:
                             exons_in_read.append(GenomicLoci(
                                 chromosome=read.reference_name,
-                                start=cur_start if cur_start > region.start else region.start,
-                                end=cur_end if cur_end <= region.end else region.end,
+                                start=cur_start if cur_start > self.region.start else self.region.start,
+                                end=cur_end if cur_end <= self.region.end else self.region.end,
                                 strand="+",
                             ))
 
                     elif cigar not in (1, 2, 4, 5):  # I, D, S, H
                         start += length
 
                 t = Transcript(
                     chromosome=read.reference_name,
-                    start=read.reference_start + 1 if read.reference_start + 1 > region.start else region.start,
-                    end=read.reference_end + 1 if read.reference_end + 1 < region.end else region.end,
+                    start=read.reference_start + 1 if read.reference_start + 1 > self.region.start else self.region.start,
+                    end=read.reference_end + 1 if read.reference_end + 1 < self.region.end else self.region.end,
                     strand=strand,
                     exons=exons_in_read
                 )
                 transcripts[t] = transcripts.get(t, 0) + 1
         except IOError as err:
             logger.debug(f"There is no .bam file at {self.path}: {err}")
         except ValueError as err:
             logger.debug(f"{self.path}: {err}")
 
-        return sorted([x for x, y in transcripts.items() if y > threshold_of_reads])
+        self.data += sorted([x for x, y in transcripts.items() if y > threshold_of_reads])
 
-    def __load_bed__(self, region: GenomicLoci) -> List[Transcript]:
-        transcripts = []
+    def __load_bed__(self):
         try:
-            for rec in Reader.read_gtf(self.path, region=region, bed=True):
+            for rec in Reader.read_gtf(self.path, region=self.region, bed=True):
                 exon_bound = []
                 current_start = int(rec[1])
                 current_end = int(rec[2])
                 if len(rec) > 3:
                     current_id = rec[3]
                 else:
                     current_id = "NoID"
@@ -489,56 +487,36 @@
                     strand=self.region.strand,
                     transcript_id=current_id,
                     exons=exon_bound,
                 )
                 if read.start < self.region.start or read.end > self.region.end:
                     continue
 
-                transcripts.append(read)
+                self.data.append(read)
 
         except IOError as err:
             logger.debug(f"There is no .bed file at {self.path}: {err}")
         except ValueError as err:
             logger.debug(f"{self.path}: {err}")
-        return transcripts
-
-    def load(self, region: GenomicLoci, threshold_of_reads: int = 0, **kwargs):
-        u"""
-        Load transcripts inside of region
-        :param region: target region
-        :param threshold_of_reads: used for bam file, only kept reads with minimum frequency
-        :return:
-        """
-        assert isinstance(region, GenomicLoci), "region should be a GenomicLoci object"
-        self.region = region
-        if self.category == "gtf":
-            self.data = self.__load_gtf__(region)
-            if self.add_local_domain:
-                self.__load_local_domain__(region)
-
-            if self.add_domain:
-                self.__add_domain__()
-        elif self.category == "bam":
-            self.data = self.__load_bam__(region, threshold_of_reads)
-        elif self.category == "bed":
-            self.data = self.__load_bed__(region)
 
+    def __load_interval(self):
         rec, start, end, strand = None, None, None, None
         for interval_file, interval_label in self.interval_file.items():
             try:
                 if not os.path.exists(interval_file + ".tbi"):
                     interval_file = pysam.tabix_index(
                         interval_file,
                         preset="bed",
                         force=True,
                         keep_original=True
                     )
 
                 interval_target = []
                 for rec in Reader.read_gtf(interval_file, region=self.region, bed=True):
+                    print(rec.start, rec.end, rec.name)
                     start = max(rec.start, self.region.start)
                     end = min(rec.end, self.region.end)
 
                     if end + 1 <= self.region.start:
                         continue
                     if start + 1 >= self.region.end:
                         break
@@ -576,10 +554,74 @@
 
             except NameError:
                 raise "Target region was not found, run load before add_bed."
 
             except OSError:
                 raise f"Error found when build index for {interval_file}, please sort file manually"
 
+    def load(self,
+             region: GenomicLoci,
+             threshold_of_reads: int = 0,
+             transcripts: Optional[List[str]] = None,
+             remove_empty_transcripts: bool = False,
+             choose_primary: bool = False,
+             **kwargs):
+        u"""
+        Load transcripts inside of region
+        :param region: target region
+        :param threshold_of_reads: used for bam file, only kept reads with minimum frequency
+        :param transcripts: list of ids or names contains the transcripts to show
+        :param remove_empty_transcripts: ignore transcripts with any exons in this region
+        :param choose_primary: only show the primary transcripts in final track
+        :return:
+        """
+        assert isinstance(region, GenomicLoci), "region should be a GenomicLoci object"
+        if transcripts is None:
+            transcripts = []
+        self.region = region
+        if self.category == "gtf":
+            self.__load_gtf__()
+            if self.add_local_domain:
+                self.__load_local_domain__(region)
+
+            if self.add_domain:
+                self.__add_domain__()
+        elif self.category == "bam":
+            self.__load_bam__(threshold_of_reads)
+        elif self.category == "bed":
+            self.__load_bed__()
+
+        self.__load_interval()
+
+        if choose_primary and len(transcripts) == 0:
+            transcripts = []
+            # For each gene, you can choose only one transcript to plot.
+            genes = defaultdict(list)
+            for transcript in self.data:
+                if transcript.category == 'interval':
+                    continue
+                genes[transcript.gene_id].append(transcript)
+
+            for _, transcripts_list in genes.items():
+                primary_transcripts = sorted(
+                    transcripts_list, key=lambda i_: len(i_), reverse=True)[0]
+                transcripts.append(primary_transcripts.transcript_id)
+        elif choose_primary and len(transcripts) != 0:
+            logger.debug(
+                "--transcripts-to-show is prior to --choose-primary, and primary transcript won't be presented.")
+        else:
+            pass
+
+        if remove_empty_transcripts or len(transcripts) > 0:
+            data = []
+            for i in self.data:
+                if len(transcripts) > 0 and i.transcript not in transcripts and i.transcript_id not in transcripts:
+                    continue
+
+                if remove_empty_transcripts and len(i.exons) < 1:
+                    continue
+                data.append(i)
+            self.data = data
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `trackplot-0.2.8/trackplot/file/Bam.py` & `trackplot-0.3.0/trackplot/file/Bam.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/file/BedGraph.py` & `trackplot-0.3.0/trackplot/file/BedGraph.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/file/Bigwig.py` & `trackplot-0.3.0/trackplot/file/Bigwig.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/file/Depth.py` & `trackplot-0.3.0/trackplot/file/Depth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/file/Fasta.py` & `trackplot-0.3.0/trackplot/file/Fasta.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/file/File.py` & `trackplot-0.3.0/trackplot/file/File.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/file/HiCMatrixTrack.py` & `trackplot-0.3.0/trackplot/file/HiCMatrixTrack.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/file/Junction.py` & `trackplot-0.3.0/trackplot/file/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/file/Motif.py` & `trackplot-0.3.0/trackplot/file/Motif.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/file/ReadSegments.py` & `trackplot-0.3.0/trackplot/file/ReadSegments.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/trackplot/plot.py` & `trackplot-0.3.0/trackplot/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from trackplot.plot_func import *
 
 logging.getLogger('matplotlib.font_manager').setLevel(logging.ERROR)
 
 faulthandler.enable()
 
 
-__version__ = "0.2.8"
+__version__ = "0.3.0"
 __author__ = "ygidtu & Ran Zhou"
 __email__ = "ygidtu@gmail.com"
 
 
 def __load__(args):
     p, args, kwargs = args
     p.load(*args, **kwargs)
@@ -1078,15 +1078,15 @@
         assert self.region is not None, f"please set the plotting region first."
 
         plots_n_rows, plots_n_cols = 1, 1
 
         height_ratio = []
         if self.annotation is not None:
             logger.info("load annotation")
-            self.annotation.load(self.region, *args, **kwargs)
+            self.annotation.load(self.region, *args, **self.params["annotation"])
             plots_n_rows += self.annotation.len(scale=annotation_scale)
 
         if self.stroke:
             plots_n_rows += int(max(len(self.stroke) * stroke_scale, 1))
 
         if self.link:
             plots_n_rows += len(self.link)
```

### Comparing `trackplot-0.2.8/trackplot/plot_func.py` & `trackplot-0.3.0/trackplot/plot_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,17 +360,14 @@
 def plot_annotation(
         ax: mpl.axes.Axes,
         obj: Annotation,
         graph_coords: Optional[Union[Dict, np.ndarray]] = None,
         font_size: int = 5,
         show_gene: bool = False,
         show_id: bool = False,
-        transcripts: Optional[List[str]] = None,
-        remove_empty_transcripts: bool = False,
-        choose_primary: bool = False,
         color: Optional[str] = None,
         theme: str = "blank",
         y_loc: int = 0,
         exon_width: float = .3,
         plot_domain: bool = False,
         show_exon_id: bool = False,
         raster: bool = True,
@@ -389,47 +386,19 @@
         return
 
     if graph_coords is None:
         graph_coords = init_graph_coords(region)
 
     color = "k" if not color else color
 
-    if choose_primary and (len(transcripts) == 0 or transcripts is None):
-        transcripts = []
-        # For each gene, you can choose only one transcript to plot.
-        genes = defaultdict(list)
-        for transcript in data:
-            if transcript.category == 'interval':
-                continue
-            genes[transcript.gene_id].append(transcript)
-
-        for _, transcripts_list in genes.items():
-            primary_transcripts = sorted(
-                transcripts_list, key=lambda i_: len(i_), reverse=True)[0]
-            transcripts.append(primary_transcripts.transcript_id)
-    elif choose_primary and (len(transcripts) != 0 or transcripts is not None):
-        logger.debug(
-            "--transcripts-to-show is prior to --choose-primary, and primary transcript won't be presented.")
-    else:
-        pass
-
     """
     @2018.12.26
     Maybe I'm too stupid for this, using 30% of total length of x axis as the gap between text with axis
     """
-
     for transcript in data:
-        # ignore the unwanted transcript
-        if transcripts and not (set(transcripts) & set(transcript.ids())):
-            continue
-
-        # ignore transcripts without any exons
-        if remove_empty_transcripts and not transcript.exons:
-            continue
-
         strand = transcript.strand
         # @2018.12.20 add transcript id, based on fixed coordinates
         if transcript.transcript:
             if show_gene and transcript.gene and transcript.gene_id != transcript.transcript_id:
                 if show_id:
                     ax.text(x=-.01 * max(graph_coords), y=y_loc + 0.25,
                             s=transcript.gene_id, fontsize=font_size, ha="right")
@@ -454,18 +423,20 @@
             ]
             y = [
                 y_loc - exon_width / 2, y_loc - exon_width / 2,
                 y_loc + exon_width / 2, y_loc + exon_width / 2
             ]
             ax.fill(x, y, color, lw=.5, zorder=20)
 
-            if show_exon_id:
+            if show_exon_id and exon.name:
                 y_loc_offset = 0.1 if ind % 2 == 0 else - 0.2
-                ax.text(x=(graph_coords[s] + graph_coords[s]) / 2, y=y_loc + y_loc_offset,
-                        s=exon.name, fontsize=font_size / 2, ha="right")
+                ax.text(x=(graph_coords[s] + graph_coords[e]) / 2,
+                        y=y_loc + y_loc_offset,
+                        s=exon.name, fontsize=font_size / 2,
+                        ha="center", color="red")
 
         # @2018.12.21
         # change the intron range
         # Draw intron.
         # if transcript's category is interval, then don't plot the intron.
         if transcript.category != "interval":
             intron_sites = [
```

### Comparing `trackplot-0.2.8/trackplot/plot_tests.py` & `trackplot-0.3.0/trackplot/plot_tests.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.8/PKG-INFO` & `trackplot-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackplot
-Version: 0.2.8
+Version: 0.3.0
 Summary: The trackplot is a tool for visualizing various next-generation sequencing (NGS) data, including DNA-seq, RNA-seq, single-cell RNA-seq and full-length sequencing datasets. https://sashimi.readthedocs.io/
 License: BSD-3
 Author: ygidtu
 Author-email: ygidtu@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -163,15 +163,15 @@
 Prior to installing the tool from the source code, users should verify their Python version (>=3.8).
 
 ```bash
 python --version
 # Python 3.10.8
 ```
 
-4.1 python3 is not available 
+    4.1 python3 is not available 
 
 If your Python version does not match the requirements of Trackplot, 
 users could follow the cmd to install and 
 more detailed instruction for different system please refer to [here](https://realpython.com/installing-python/).  
 
 ```bash
 # If the default Python version does not meet the requirements of Trackplot, 
@@ -195,15 +195,15 @@
 $PWD/Python-3.10.12/python -m pip install -e trackplot/
 
 # 3. check trackplot
 $PWD/Python-3.10.12/Python-3.10.12/Python/bin/trackplot --help
 
 ```
 
-4.2 python3 is available
+    4.2 python3 is available
 
 ```bash
 # 1. download the trackplot
 git clone https://github.com/ygidtu/trackplot trackplot
 cd trackplot
 
 # 2. install the trackplot and it's requirements to python env
@@ -286,19 +286,19 @@
 
 # or just run with poetry
 poetry run python main.py --help
 ```
 
 ### Using trackplot by a local webserver
 
-1. using AppImage (Linux x86_64 only)
+1. [AppImage](https://github.com/ygidtu/trackplot/releases) (Linux x86_64 only)
 
 ```bash
-# example with version v0.2.6, please using your interested version according to your needs
-export VERSION=0.2.6
+# example with version v0.3.0, please using your interested version according to your needs
+export VERSION=0.3.0
 gunzip trackplotweb-${VERSION}-x86_64.AppImage
 chmod +x trackplotweb-${VERSION}-x86_64.AppImage
 ./trackplotweb-${VERSION}-x86_64.AppImage --help
 
 # startup webserver
 ./trackplotweb-${VERSION}-x86_64.AppImage --host 127.0.0.1 --port 5000 --plots ./plots
 ```
@@ -312,24 +312,33 @@
    
 ```bash
 docker pull ygidtu/trackplotweb
 
 # -v map the current working directory into docker containers
 # -p map the outer port to inner port of docker container
 docker run --name trackplotweb \
- --rm -v $PWD:$PWD \
- -p 5000:5000 \
- ygidtu/trackplotweb
+  --rm \
+  -v $PWD/data:/data \
+  -v $PWD/plots/:/plots
+  -p 5000:5000 \
+  --data /data \
+  --plots /plots \
+  ygidtu/trackplotweb 
 ```
 
+`-p`: public and private port for the server, default:5000(public):5000(private)
+- `-v`, `--volume`: mount the working directory to docker container, for example, the `$PWD/data` could replace by the path to your directory contains all necessary data
+- `--user`: prevent docker read and write file using root privileges
+- the rest usage please check [Command line usage](./command.md)
+
 ---
 
 3. Install from source code
 
-Before this, please make sure that trackplot has been properly installed in your env.  
+Before this, please make sure that trackplot has been properly installed in the same env.  
 
 
 ```bash
 git clone https://github.com/ygidtu/trackplot trackplot
 cd trackplot/web
 
 # build the frontend static files; If npm was not found, please install nodejs(https://nodejs.org).
```

