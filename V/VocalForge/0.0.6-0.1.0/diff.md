# Comparing `tmp/VocalForge-0.0.6.tar.gz` & `tmp/VocalForge-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VocalForge-0.0.6.tar", last modified: Sun Jun 11 01:36:04 2023, max compression
+gzip compressed data, was "VocalForge-0.1.0.tar", last modified: Wed Jul 19 04:13:02 2023, max compression
```

## Comparing `VocalForge-0.0.6.tar` & `VocalForge-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/
--rw-rw-r--   0 rio       (1000) rio       (1000)     1067 2023-05-21 03:39:13.000000 VocalForge-0.0.6/LICENSE.md
--rw-rw-r--   0 rio       (1000) rio       (1000)     6156 2023-06-11 01:36:04.149953 VocalForge-0.0.6/PKG-INFO
--rw-rw-r--   0 rio       (1000) rio       (1000)     5774 2023-05-21 03:39:13.000000 VocalForge-0.0.6/README.md
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/VocalForge/
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/VocalForge/VocalForge/
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/VocalForge/VocalForge/audio/
--rw-rw-r--   0 rio       (1000) rio       (1000)      204 2023-05-31 00:06:05.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/__init__.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    11150 2023-06-06 03:10:36.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/audio_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     4439 2023-06-04 02:30:09.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/export_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     9966 2023-06-04 02:30:19.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/isolate.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2706 2023-06-10 23:55:14.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/overlap.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2386 2023-05-31 00:06:30.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/refine_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     3825 2023-06-10 23:51:14.000000 VocalForge-0.0.6/VocalForge/VocalForge/audio/voice_detection.py
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/VocalForge/VocalForge/text/
--rw-rw-r--   0 rio       (1000) rio       (1000)      250 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/__init__.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     3555 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/create_dataset.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2211 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/ctc.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    26284 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/ctc_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     1666 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/normalization_helpers.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     4247 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/normalize_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    10460 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/process_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2442 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/refine_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2277 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/segment.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     1759 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/split_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     5407 2023-05-31 04:31:49.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/text_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2330 2023-05-21 03:39:13.000000 VocalForge-0.0.6/VocalForge/VocalForge/text/transcribe.py
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-11 01:36:04.149953 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/
--rw-rw-r--   0 rio       (1000) rio       (1000)     6156 2023-06-11 01:36:04.000000 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/PKG-INFO
--rw-rw-r--   0 rio       (1000) rio       (1000)     1057 2023-06-11 01:36:04.000000 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/SOURCES.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)        1 2023-06-11 01:36:04.000000 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/dependency_links.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)      279 2023-06-11 01:36:04.000000 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/requires.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)       11 2023-06-11 01:36:04.000000 VocalForge-0.0.6/VocalForge/VocalForge.egg-info/top_level.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)     1078 2023-06-11 01:35:43.000000 VocalForge-0.0.6/pyproject.toml
--rw-rw-r--   0 rio       (1000) rio       (1000)       38 2023-06-11 01:36:04.149953 VocalForge-0.0.6/setup.cfg
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-07-19 04:13:02.659455 VocalForge-0.1.0/
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1067 2023-07-19 04:08:57.000000 VocalForge-0.1.0/LICENSE.md
+-rw-rw-r--   0 rio       (1000) rio       (1000)     4561 2023-07-19 04:13:02.659455 VocalForge-0.1.0/PKG-INFO
+-rw-rw-r--   0 rio       (1000) rio       (1000)     4179 2023-07-19 04:08:57.000000 VocalForge-0.1.0/README.md
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-07-19 04:13:02.659455 VocalForge-0.1.0/VocalForge/
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-07-19 04:13:02.659455 VocalForge-0.1.0/VocalForge/VocalForge/
+-rw-rw-r--   0 rio       (1000) rio       (1000)       40 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/__init__.py
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-07-19 04:13:02.659455 VocalForge-0.1.0/VocalForge/VocalForge/audio/
+-rw-rw-r--   0 rio       (1000) rio       (1000)      204 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/audio/__init__.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    11150 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/audio/audio_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     4439 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/audio/export_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     9966 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/audio/isolate.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2706 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/audio/overlap.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2386 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/audio/refine_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     3825 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/audio/voice_detection.py
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-07-19 04:13:02.659455 VocalForge-0.1.0/VocalForge/VocalForge/text/
+-rw-rw-r--   0 rio       (1000) rio       (1000)      250 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/text/__init__.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     3687 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/text/create_dataset.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2211 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/text/ctc.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    26284 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/text/ctc_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1666 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/text/normalization_helpers.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     4686 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/text/normalize_text.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    10460 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/text/process_text.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2516 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/text/segment.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1885 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/text/split_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     5407 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/text/text_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     3567 2023-07-19 04:08:57.000000 VocalForge-0.1.0/VocalForge/VocalForge/text/transcribe.py
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-07-19 04:13:02.659455 VocalForge-0.1.0/VocalForge/VocalForge.egg-info/
+-rw-rw-r--   0 rio       (1000) rio       (1000)     4561 2023-07-19 04:13:02.000000 VocalForge-0.1.0/VocalForge/VocalForge.egg-info/PKG-INFO
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1049 2023-07-19 04:13:02.000000 VocalForge-0.1.0/VocalForge/VocalForge.egg-info/SOURCES.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)        1 2023-07-19 04:13:02.000000 VocalForge-0.1.0/VocalForge/VocalForge.egg-info/dependency_links.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)      279 2023-07-19 04:13:02.000000 VocalForge-0.1.0/VocalForge/VocalForge.egg-info/requires.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)       11 2023-07-19 04:13:02.000000 VocalForge-0.1.0/VocalForge/VocalForge.egg-info/top_level.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1079 2023-07-19 04:12:54.000000 VocalForge-0.1.0/pyproject.toml
+-rw-rw-r--   0 rio       (1000) rio       (1000)       38 2023-07-19 04:13:02.659455 VocalForge-0.1.0/setup.cfg
```

### Comparing `VocalForge-0.0.6/LICENSE.md` & `VocalForge-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/audio/audio_utils.py` & `VocalForge-0.1.0/VocalForge/VocalForge/audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/audio/export_audio.py` & `VocalForge-0.1.0/VocalForge/VocalForge/audio/export_audio.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/audio/isolate.py` & `VocalForge-0.1.0/VocalForge/VocalForge/audio/isolate.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/audio/overlap.py` & `VocalForge-0.1.0/VocalForge/VocalForge/audio/overlap.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/audio/refine_audio.py` & `VocalForge-0.1.0/VocalForge/VocalForge/audio/refine_audio.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/audio/voice_detection.py` & `VocalForge-0.1.0/VocalForge/VocalForge/audio/voice_detection.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/text/create_dataset.py` & `VocalForge-0.1.0/VocalForge/VocalForge/text/create_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 import os
 import pandas as pd
 from .text_utils import get_files
 import shutil
 
+import os
+import pandas as pd
+from .text_utils import get_files
+import shutil
+
 class GenerateDataset():
     """
     Generates a dataset by processing audio files and corresponding metadata.
 
+    Parameters:
+        segment_dir (str): Directory path of the segmented audio files.
+        sliced_aud_dir (str): Directory path of the sliced audio files.
+        output_dir (str): Directory path of the dataset.
+        threshold (float): Threshold value of confidence from CTC segmentation. The closer to 0, the more selective the clips will be. (cannot be > 0)
+
+    Generates:
+        Dataset (list): List of metadata for each audio file.
+        
     TODO: 
         Add the ability for user to delete unwanted files, and have an autoupdating metadata when called
         List the dataset length (in seconds)
-
-    Parameters:
-        threshold (float): Threshold value used to filter audio data.
-
-    Returns:
-        None
     """
     def __init__(self, segment_dir, sliced_aud_dir, output_dir, threshold=2.5):
         self.Segment_Dir = segment_dir
         self.Sliced_Aud_Dir = sliced_aud_dir
-        self.Out_Dir = output_dir
+        self.Output_Dir = output_dir
         self.Threshold = threshold
         self.Dataset = []
 
-
-    # Create directories for storing processed data
-
-    
     def create_metadata(self, file_path: str, thres: float):
         """
         Creates metadata for the audio data.
 
         Parameters:
             file_path (str): Path to audio file.
             thres (float): Threshold value used to filter audio data.
@@ -66,36 +70,31 @@
 
     def create_dataset(self, metadata: pd.DataFrame):
         """
         Creates a dataset by copying audio files and saving metadata.
 
         Parameters:
             metadata (pd.DataFrame): Metadata for the audio data.
-            dataset_dir (str): Directory where the dataset is to be saved.
-
-        Returns:
-            None
         """
         wav_dir = os.path.join(self.Out_Dir, 'wavs')
         try:
             os.mkdir(wav_dir)
         except:
             pass
         metadata.to_csv(os.path.join(self.Out_Dir, "metadata.csv"),
                         index=False, header=False, sep='|', encoding='utf-8-sig')
         
         for folder in get_files(self.Sliced_Aud_Dir):
             #TODO: check if file is entered on metadata.csv, currently copies regardless of validity
             aud_clips_dir = os.path.join(self.Sliced_Aud_Dir, folder)
             destination = shutil.copytree(aud_clips_dir, wav_dir, dirs_exist_ok=True)
     
-    def run_dataset_generation(self):
-        if os.listdir(self.Out_Dir) != []:
-            print("Dataset has already been created! Skipping...")
-            return
+    def run(self):
+        """
+        Runs the dataset generation process.
+        """
         for file in get_files(self.Segment_Dir, '.txt'):
             file_dir = os.path.join(self.Segment_Dir, file)
             self.Dataset.append(self.create_metadata(file_dir, self.Threshold))
         metadata = pd.concat(self.Dataset)
         self.create_dataset(metadata)
-        self.Dataset = []
-        print("Dataset has been created!")
+        self.Dataset = []
```

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/text/ctc.py` & `VocalForge-0.1.0/VocalForge/VocalForge/text/ctc.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/text/ctc_utils.py` & `VocalForge-0.1.0/VocalForge/VocalForge/text/ctc_utils.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/text/normalization_helpers.py` & `VocalForge-0.1.0/VocalForge/VocalForge/text/normalization_helpers.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/text/normalize_text.py` & `VocalForge-0.1.0/VocalForge/VocalForge/text/normalize_text.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,48 +4,48 @@
 from .text_utils import get_files
 
 class NormalizeText():
     """
     This function prepares the audio and text files for language modeling.
     
     Args:
-    1. model (str): Model name to be used for processing the text.
-    2. length (int): The max length of each sentence in the output file.
-    3. lang (str): Language of the input audio and text files.
-    
-    Returns:
-    None
+    1. input_dir (str): Directory path of the raw text files.
+    2. output_dir (str): Directory path of the processed text files.
+    3. audio_dir (str): Directory path of the raw audio files.
+    4. model (str): Nvidia Model to use for language modeling.
+    5. max_length (int): max length of the text sentences.
+    7. min_length (int): min length of the text sentences.
+    6. lang (str): Language of the text, i.e 'en' or 'ru'
+
     """
     def __init__(
         self, 
         input_dir: str, 
-        out_dir: str, 
+        output_dir: str, 
         audio_dir: str, 
         model='nvidia/stt_en_citrinet_1024_gamma_0_25', 
-        length=25, 
-        lang='en',
-        min_length=0
+        max_length=25, 
+        min_length=0,
+        lang='en'
     ):
         self.Model = model
-        self.Length = length
+        self.Max_Length = max_length
         self.Min_Length = min_length
         self.Lang = lang
         self.Input_Dir = input_dir
-        self.Out_Dir = out_dir
+        self.Output_Dir = output_dir
         self.Audio_Dir = audio_dir
         from nemo.collections.asr.models import ASRModel
         self.Cfg = ASRModel.from_pretrained(model_name=self.Model, return_config=True)  
-
-    # Check if the folders have already been processed
     
     
 
     def prepare_audio_file(self, aud_dir, out_dir):
         """
-        This function prepares the audio file for language modeling.
+        This function prepares the audio file for language modeling. Currently it only moves the file to the output directory.
         
         Args:
         1. audio_dir (str): Directory path of the raw audio file.
         2. new_dir (str): Directory path of the processed audio file.
         
         Returns:
         None
@@ -68,53 +68,58 @@
         lang = self.Lang
         cfg = self.Cfg
         transcript = format_text(textfile_dir, lang)
         sentences = split_text(
             transcript, 
             lang, 
             cfg.decoder.vocabulary, 
-            self.Length, 
+            self.Max_Length, 
             additional_split_symbols=None,
             min_length=self.Min_Length
         )
         return normalize_text(sentences, lang, cfg.decoder.vocabulary)
 
     def write_file(self, file_num:str, text_type:str, sentences:str, outdir:str):
         """
         This function writes the processed text to a file.
         
         Args:
         1. file_num (str): File number to be used in the file name.
         2. text_type (str): Type of text to be written to the file.
         3. sentences (str): Processed text sentences to be written to the file.
-        
-        Returns:
-        None
+        4. outdir (str): Directory path of the processed text files.
         """
         file_name = f"{file_num}{text_type}"
         file_dir = os.path.join(outdir, file_num, file_name)
         print(file_dir)
         with open(file_dir+'.txt', 'w', encoding='UTF-8') as f:
             for sentence in sentences:
                 sentence = sentence.strip()
                 f.write(sentence+"\n")
 
     def prepare_file(self, text_dir, aud_dir, out_dir):
-        #folder_dir = os.path.join(processed_dir, file.replace('.txt',''))
+        """
+        This function prepares the text and audio files for language modeling.
+        
+        Args:
+        1. text_dir (str): Directory path of the raw text file.
+        2. aud_dir (str): Directory path of the raw audio file.
+        3. out_dir (str): Directory path of the processed text and audio files.
+        """
         base_name = os.path.basename(text_dir)
         sentence_types = self.prepare_text(text_dir)
         folder_dir = os.path.join(out_dir, base_name.replace('.txt', ''))
         try: os.mkdir(folder_dir)
         except: pass
         for name, sentences in sentence_types.items():
             self.write_file(base_name.replace('.txt', ''), name, sentences.splitlines(), out_dir)
         self.prepare_audio_file(aud_dir, os.path.join(folder_dir, base_name.replace('.txt', '.wav')))
     
-    def run_processing(self):
-        print(self.Out_Dir)
-        if os.listdir(self.Out_Dir) != []:
-            print("folder(s) have already been processed! Skipping...")
-            return
+    
+    def run(self):
+        """
+        This function runs the text normalization pipeline.
+        """
         for file in get_files(self.Input_Dir, '.txt'):
             text_dir = os.path.join(self.Input_Dir, file)
             audfile_dir = os.path.join(self.Audio_Dir, file.replace('.txt', '.wav'))
-            self.prepare_file(text_dir, audfile_dir, self.Out_Dir)
+            self.prepare_file(text_dir, audfile_dir, self.Output_Dir)
```

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/text/process_text.py` & `VocalForge-0.1.0/VocalForge/VocalForge/text/process_text.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/text/segment.py` & `VocalForge-0.1.0/VocalForge/VocalForge/text/segment.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,36 +6,40 @@
 class Segment():
     """
     This function segments audio files into multiple parts based on the timestamps obtained
     using a model. The timestamps are used to split the audio file into smaller parts and
     are saved in a text file.
 
     Parameters:
-    model (str): Pretrained model name.
-    window_size (int): Size of the window for the model.
-
-    Returns:
-    None
+    input_dir (str): Directory path of the audio files.
+    output_dir (str): Directory path of the segmented audio files.
+    model (str): Nvidia Model to use for segmentation.
+    window_size (int): The amount (in ms) of audio to process at a time. May have to increase if files are too large. 
+
+    Generates:
+    Median_Loss (float): Median loss obtained from the model timing for all audio files.
+    Loss (list): List of losses obtained from the model timing for each audio file.
     """
     def __init__(self, input_dir, output_dir, model='nvidia/stt_en_citrinet_1024_gamma_0_25', window_size=8000):
         self.Input_Dir = input_dir
-        self.Out_Dir = output_dir
+        self.Output_Dir = output_dir
         self.Window_Size = window_size
         import nemo.collections.asr as nemo_asr
         self.Model = nemo_asr.models.EncDecCTCModelBPE.from_pretrained(model)
         self.Loss = []
         self.Median_Loss = None
 
     def segment_folder(self, folder_dir, out_dir):
         """
         This function segments audio files in a folder into multiple parts based on
         the timestamps obtained using a model.
 
         Parameters:
-        folder (str): Folder containing audio files.
+        folder_dir (str): Directory path of the audio files.
+        out_dir (str): Directory path of the segmented audio files.
 
         Returns:
         float: Mean loss obtained from the model.
         """
         loss_folder = []
         for aud_file in get_files(folder_dir, '.wav'):
             aud_path = os.path.join(folder_dir, aud_file)
@@ -45,18 +49,14 @@
         try:
             return statistics.mean(loss_folder)
         except: return None
 
     def find_median_loss(self):
         self.Median_Loss = statistics.median(self.Loss)
 
-    def run_segmentation(self):
-        if os.listdir(self.Out_Dir) != []:
-            print("folder(s) have already found its split timestamps! Skipping...")
-            return
+    def run(self):
         for folder in get_files(self.Input_Dir):
             folder_dir = os.path.join(self.Input_Dir, folder)
-            value = self.segment_folder(folder_dir, self.Out_Dir)
+            value = self.segment_folder(folder_dir, self.Output_Dir)
             if value != None: self.Loss.append(value)
         self.Median_Loss = statistics.median(self.Loss)
-        self.find_median_loss()
-        print(f"median loss: {self.Median_Loss}")
+        self.find_median_loss()
```

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/text/split_audio.py` & `VocalForge-0.1.0/VocalForge/VocalForge/text/split_audio.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,46 +4,41 @@
 
 class SplitAudio():
     """
     This function splits the audio into clips using the timestamps in the
     segmented audio folder.
 
     Args:
-    - offset: The number of seconds to add or subtract from the timestamps.
-    - max_duration: The maximum duration of each clip.
-    - threshold: The threshold to use for processing the alignment.
-
-    Returns:
-    None
-
+    1. input_dir (str): Directory path of the segmented audio files.
+    2. output_dir (str): Directory path of the clips.
+    3. offsets (list): List of offsets for each file, i.e [0, 0.5, 1.0] for 3 files.
+    4. paddings (list): List of paddings for each file, i.e [0, 0.5, 1.0] for 3 files.
+    5. max_duration (int): Max duration of the clips in seconds.
+    6. threshold (float): Confidence threshold for the timing of the clips. The closer to 0, the more selective the clips will be. (cannot be > 0)
     """
     def __init__(self, input_dir, output_dir, offsets=[0], paddings=[0], max_duration=40, threshold=2.5):
         self.Input_Dir = input_dir
-        print(self.Input_Dir)
-        self.Out_Dir = output_dir
+        self.Output_Dir = output_dir
         self.Offset = offsets
         self.Padding = paddings
         self.Max_Duration = max_duration
         self.Threshold = -threshold
         
 
-    def run_slicing(self):
-        if os.listdir(self.Out_Dir) != []:
-            print("audio has already been sliced! Skipping...")
-            return
+    def run(self):
         for index, file in enumerate(get_files(self.Input_Dir, '.txt')):
             try:
                 offset = self.Offset[index]
             except:
                 offset = self.Offset[0]
             try:
                 padding = self.Padding[index]
             except:
                 padding = self.Padding[0]
-            clips_folder_dir = os.path.join(self.Out_Dir, file.split('_segmented')[0])
+            clips_folder_dir = os.path.join(self.Output_Dir, file.split('_segmented')[0])
             os.mkdir(clips_folder_dir)
             file_dir = os.path.join(self.Input_Dir, file)
             process_alignment(
                 alignment_file=file_dir,
                 clips_dir=clips_folder_dir,
                 offset = offset,
                 padding = padding,
```

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/text/text_utils.py` & `VocalForge-0.1.0/VocalForge/VocalForge/text/text_utils.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge/text/transcribe.py` & `VocalForge-0.1.0/VocalForge/VocalForge/text/transcribe.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,85 @@
 from .text_utils import get_files
 import os
-
+from whisper import load_model
 class Transcribe():
     """
-    Transcribe audio files in a directory using a pre-trained ASR model.
-    
-    Returns:
-        None
-        
-    Note:
-        The function prints the names of the transcribed files and skips the ones 
-        that have already been transcribed. If a file is corrupted, the function 
-        prints "file corrupted! skipping...".
+    A class for transcribing audio files and writing the transcriptions to text files.
+
+    Attributes:
+        Input_Dir (str): The directory containing the audio files to transcribe.
+        Output_Dir (str): The directory to write the transcriptions to.
+        Prompt (str, optional): The initial prompt to use for the transcription. Defaults to None.
+        Model (object): The model to use for the transcription.
+        Texts (list): A list of the transcribed texts.
+        do_write (bool): Whether to write the transcriptions to text files.
+
+    Methods:
+        analyze(do_write=True):
+            Transcribes audio files in the input directory and writes the transcriptions to text files in the output directory.
+
+            Args:
+                do_write (bool, optional): Whether to write the transcriptions to text files. Defaults to True.
+
+        write_transcription(result, text_file_dir):
+            Writes the transcription to a text file.
+
+            Args:
+                result (dict): The transcription result.
+                text_file_dir (str): The directory to write the transcription to.
+
+        run():
+            Transcribes all audio files in the `Input_Dir` folder.
     """
-    def __init__(self, raw_dir, out_dir, prompt=None):
-        self.Raw_Dir = raw_dir
-        self.Out_Dir = out_dir
+
+    def __init__(self, input_dir, output_dir, model="large", prompt=None, do_write=True):
+        """
+        Initializes the Transcribe class.
+
+        Args:
+            input_dir (str): The directory containing the audio files to transcribe.
+            output_dir (str): The directory to write the transcriptions to.
+            model (str, optional): The model to use for the transcription. Defaults to "large".
+            prompt (str, optional): The initial prompt to use for the transcription. Defaults to None.
+            do_write (bool, optional): Whether to write the transcriptions to text files. Defaults to True.
+        """
+        self.Input_Dir = input_dir
+        self.Output_Dir = output_dir
         self.Prompt = prompt
-        from whisper import load_model
-        self.Model = load_model("large")
+        self.Model = load_model(model)
+        self.Texts = []
+        self.Do_Write = do_write
 
-    def transcribe_folder(self, input_dir, do_write=True):
+    def analyze(self):
         """
-        Transcribe all audio files in a folder.
-        
+        Transcribes audio files in the input directory and writes the transcriptions to text files in the output directory.
+
         Args:
-            folder (str): The path to the folder containing audio files.
-            
-        Returns:
-            None
-            
-        Note:
-            The function transcribes each audio file in the folder and writes the 
-            transcription to a text file with the same name. If the text file 
-            already exists, the function skips the transcription.
-        """
-
-        for file in get_files(input_dir):
-            #try:
-                text_file_dir = os.path.join(self.Out_Dir, file.split(".")[0]+".txt")
-                # check if the text file already exists
-                if not os.path.exists(text_file_dir):
-                    # transcribe the audio file
-                    aud_file_dir = os.path.join(input_dir, file)
-                    result = self.Model.transcribe(aud_file_dir, initial_prompt=self.Prompt)
-                    if do_write:
-                        self.write_transcription(result, text_file_dir)
-            # except:
-            #     # print an error message if the audio file is corrupted
-            #     print("file corrupted! skipping...")
-    
+            do_write (bool, optional): Whether to write the transcriptions to text files. Defaults to True.
+        """
+        for file in get_files(self.Input_Dir):
+            text_file_dir = os.path.join(self.Output_Dir, file.split(".")[0]+".txt")
+            # check if the text file already exists
+            if not os.path.exists(text_file_dir):
+                # transcribe the audio file
+                aud_file_dir = os.path.join(self.Input_Dir, file)
+                result = self.Model.transcribe(aud_file_dir, initial_prompt=self.Prompt)
+                self.Texts.append(result['text'].strip())
+                if self.Do_Write:
+                    self.write_transcription(result, text_file_dir)
+
     def write_transcription(self, result, text_file_dir):
+        """
+        Writes the transcription to a text file.
+
+        Args:
+            result (dict): The transcription result.
+            text_file_dir (str): The directory to write the transcription to.
+        """
         with open(text_file_dir, 'w', encoding="utf-8") as f:
             f.write(result['text'].strip())
 
-    # transcribe all audio files in the `aud_dir` folder
-    def run_trancription(self): 
-        if os.listdir(self.Out_Dir) != []:
-            print("folder(s) have already been transcribed! Skipping...")
-            return
-        self.transcribe_folder(self.Raw_Dir)
+    def run(self):
+        """
+        Transcribes all audio files in the `Input_Dir` folder.
+        """
+        self.analyze(self.Input_Dir)
```

### Comparing `VocalForge-0.0.6/VocalForge/VocalForge.egg-info/SOURCES.txt` & `VocalForge-0.1.0/VocalForge/VocalForge.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.md
 README.md
 pyproject.toml
+VocalForge/VocalForge/__init__.py
 VocalForge/VocalForge.egg-info/PKG-INFO
 VocalForge/VocalForge.egg-info/SOURCES.txt
 VocalForge/VocalForge.egg-info/dependency_links.txt
 VocalForge/VocalForge.egg-info/requires.txt
 VocalForge/VocalForge.egg-info/top_level.txt
 VocalForge/VocalForge/audio/__init__.py
 VocalForge/VocalForge/audio/audio_utils.py
@@ -16,12 +17,11 @@
 VocalForge/VocalForge/text/__init__.py
 VocalForge/VocalForge/text/create_dataset.py
 VocalForge/VocalForge/text/ctc.py
 VocalForge/VocalForge/text/ctc_utils.py
 VocalForge/VocalForge/text/normalization_helpers.py
 VocalForge/VocalForge/text/normalize_text.py
 VocalForge/VocalForge/text/process_text.py
-VocalForge/VocalForge/text/refine_text.py
 VocalForge/VocalForge/text/segment.py
 VocalForge/VocalForge/text/split_audio.py
 VocalForge/VocalForge/text/text_utils.py
 VocalForge/VocalForge/text/transcribe.py
```

### Comparing `VocalForge-0.0.6/pyproject.toml` & `VocalForge-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "VocalForge"
-version = "0.0.6"
+version = "0.1.0"
 
 authors = [
   {email="rio@rioharper.com" },
 ]
 description = "Your one-stop solution for voice dataset creation"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -49,8 +49,8 @@
         'ctc_segmentation',
         'nemo==4.5.5',
         'nemo_text_processing',
         'nemo_toolkit',
         'num2words==0.5.12',
         'openai_whisper',
         'whisper',
-]
+]
```

