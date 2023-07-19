# Comparing `tmp/bert-for-sequence-classification-0.0.5a0.tar.gz` & `tmp/bert-for-sequence-classification-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert-for-sequence-classification-0.0.5a0.tar", last modified: Mon Jul 10 13:42:44 2023, max compression
+gzip compressed data, was "bert-for-sequence-classification-0.0.6a0.tar", last modified: Wed Jul 19 12:30:14 2023, max compression
```

## Comparing `bert-for-sequence-classification-0.0.5a0.tar` & `bert-for-sequence-classification-0.0.6a0.tar`

### file list

```diff
@@ -1,29 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/bert_clf/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/bert_clf/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/BertCLF.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/early_stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/BaseDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/PandasDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/SimpleDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/preparing_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-10 13:42:33.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/src/training_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-10 13:42:34.000000 bert-for-sequence-classification-0.0.5a0/bert_clf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 13:42:44.000000 bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 13:42:44.370093 bert-for-sequence-classification-0.0.5a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-10 13:42:34.000000 bert-for-sequence-classification-0.0.5a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.101203 bert-for-sequence-classification-0.0.6a0/bert_clf/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.101203 bert-for-sequence-classification-0.0.6a0/bert_clf/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/BaseDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/BaseModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/CLFFabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/early_stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/bert_clf/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/models/BertCLF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/models/EncoderCLF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/PandasDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/SimpleDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/preparing_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/src/training_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/bert_clf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 12:30:14.000000 bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-19 12:30:14.105203 bert-for-sequence-classification-0.0.6a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-19 12:30:00.000000 bert-for-sequence-classification-0.0.6a0/setup.py
```

### Comparing `bert-for-sequence-classification-0.0.5a0/LICENSE` & `bert-for-sequence-classification-0.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5a0/PKG-INFO` & `bert-for-sequence-classification-0.0.6a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.0.5a0
+Version: 0.0.6a0
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -74,42 +74,42 @@
 Otherwise:
 
 ```python
 
 import torch
 import json
 import pandas as pd
-from bert_clf.src.BertCLF import BertCLF
+from bert_clf.src.models.BertCLF import BertCLF
 from transformers import AutoModel, AutoTokenizer
 
-device = torch.device("cuda" if  torch.cuda.is_available() else "cpu")
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 tokenizer = AutoTokenizer.from_pretrained(
-        pretrained_model_name_or_path="pretrained_model_name_or_path"
-    )
+    pretrained_model_name_or_path="pretrained_model_name_or_path"
+)
 model_bert = AutoModel.from_pretrained(
     pretrained_model_name_or_path="pretrained_model_name_or_path"
 ).to(device)
 
-id2label = json.load(open("path/to/saved/mapper")) # mapper is saved with the state dict
+id2label = json.load(open("path/to/saved/mapper"))  # mapper is saved with the state dict
 
 model = BertCLF(
     pretrained_model=model_bert,
     tokenizer=tokenizer,
     id2label=id2label,
     dropout="some number",
     device=device
 )
 
 model.load_state_dict(
     torch.load(
-    "path_to_state_dict", map_location=device
+        "path_to_state_dict", map_location=device
     ),
     strict=False
 )
 
 model.eval()
-    
+
 df = pd.read_csv("path_to_some_df")
 
 df["target_column"] = df["text_column"].apply(model.predict)
 ```
```

### Comparing `bert-for-sequence-classification-0.0.5a0/README.md` & `bert-for-sequence-classification-0.0.6a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,42 +60,42 @@
 Otherwise:
 
 ```python
 
 import torch
 import json
 import pandas as pd
-from bert_clf.src.BertCLF import BertCLF
+from bert_clf.src.models.BertCLF import BertCLF
 from transformers import AutoModel, AutoTokenizer
 
-device = torch.device("cuda" if  torch.cuda.is_available() else "cpu")
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 tokenizer = AutoTokenizer.from_pretrained(
-        pretrained_model_name_or_path="pretrained_model_name_or_path"
-    )
+    pretrained_model_name_or_path="pretrained_model_name_or_path"
+)
 model_bert = AutoModel.from_pretrained(
     pretrained_model_name_or_path="pretrained_model_name_or_path"
 ).to(device)
 
-id2label = json.load(open("path/to/saved/mapper")) # mapper is saved with the state dict
+id2label = json.load(open("path/to/saved/mapper"))  # mapper is saved with the state dict
 
 model = BertCLF(
     pretrained_model=model_bert,
     tokenizer=tokenizer,
     id2label=id2label,
     dropout="some number",
     device=device
 )
 
 model.load_state_dict(
     torch.load(
-    "path_to_state_dict", map_location=device
+        "path_to_state_dict", map_location=device
     ),
     strict=False
 )
 
 model.eval()
-    
+
 df = pd.read_csv("path_to_some_df")
 
 df["target_column"] = df["text_column"].apply(model.predict)
 ```
```

### Comparing `bert-for-sequence-classification-0.0.5a0/bert_clf/src/BertCLF.py` & `bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/BaseModel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,34 @@
 from typing import Dict
 
 import torch
 import torch.nn as nn
-from transformers.modeling_utils import PreTrainedModel
-from transformers.tokenization_utils_base import PreTrainedTokenizerBase
+from transformers import AutoTokenizer, AutoModel
+from abc import abstractmethod
 
 
-class BertCLF(nn.Module):
+class BaseCLF(nn.Module):
 
     def __init__(
             self,
-            pretrained_model: PreTrainedModel,
-            tokenizer: PreTrainedTokenizerBase,
+            pretrained_model_name: str,
             id2label: Dict[int, str],
             dropout: float,
-            device: torch.device = torch.device('cpu')
     ):
         super().__init__()
-        self.tokenizer = tokenizer
-        self.pretrained_model = pretrained_model
+        self.tokenizer = AutoTokenizer.from_pretrained(pretrained_model_name_or_path=pretrained_model_name)
+        self.pretrained_model = AutoModel.from_pretrained(pretrained_model_name_or_path=pretrained_model_name)
         self.drop = nn.Dropout(dropout)
         self.act = nn.LogSoftmax(1)
         self.mapper = id2label
-        self.device = device
 
-        out_bert = self.pretrained_model.config.hidden_size
-        self.fc = nn.Linear(out_bert, len(self.mapper))
 
+    @abstractmethod
     def forward(self, texts: torch.Tensor) -> torch.Tensor:
-        mask = (texts != self.tokenizer.pad_token_id).long()
-
-        hidden = self.pretrained_model(texts, attention_mask=mask)[0]
-
-        dense_outputs = self.fc(self.drop(hidden[:, 0]))
-        outputs = self.act(dense_outputs)
-
-        return outputs
+        raise NotImplementedError
 
     def _predict(self, text: str) -> torch.Tensor:
         inputs = self.tokenizer.encode(text, return_tensors="pt", truncation=True)
         outputs = self(inputs.to(self.pretrained_model.device))
         return outputs
 
     def predict(self, text: str) -> str:
```

### Comparing `bert-for-sequence-classification-0.0.5a0/bert_clf/src/dataset.py` & `bert-for-sequence-classification-0.0.6a0/bert_clf/src/dataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5a0/bert_clf/src/early_stopping.py` & `bert-for-sequence-classification-0.0.6a0/bert_clf/src/early_stopping.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/BaseDataset.py` & `bert-for-sequence-classification-0.0.6a0/bert_clf/src/core/BaseDataset.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/PandasDataset.py` & `bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/PandasDataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import pandas as pd
 
-from bert_clf.src.pandas_dataset.BaseDataset import BaseDataset
+from bert_clf.src.core.BaseDataset import BaseDataset
 
 
 class PandasDataset(BaseDataset):
     """
     Dataset class for datasets that have simple structure
     """
```

### Comparing `bert-for-sequence-classification-0.0.5a0/bert_clf/src/pandas_dataset/SimpleDataFrame.py` & `bert-for-sequence-classification-0.0.6a0/bert_clf/src/pandas_dataset/SimpleDataFrame.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5a0/bert_clf/src/preparing_data_utils.py` & `bert-for-sequence-classification-0.0.6a0/bert_clf/src/preparing_data_utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5a0/bert_clf/src/training_utils.py` & `bert-for-sequence-classification-0.0.6a0/bert_clf/src/training_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 import torch
 from sklearn.metrics import classification_report
-from bert_clf.src.BertCLF import BertCLF
+
+from bert_clf.src.core import BaseCLF
 from bert_clf.src.early_stopping import EarlyStopping
 import numpy as np
 from sklearn.metrics import f1_score
 from tqdm import tqdm
 from typing import Dict, Any, Optional, Union, List, Tuple
 
 
 def predict_metrics(
-        model: BertCLF,
+        model: BaseCLF,
         iterator: torch.utils.data.DataLoader,
 ):
 
     """
     :param model: model architecture that you want to fine-tune
     :param iterator: iterator with data reserved for evaluating
     """
 
     true = []
     pred = []
 
     model.eval()
     with torch.no_grad():
         for texts, ys in tqdm(iterator, total=len(iterator), desc="Computing final metrics..."):
-            predictions = model(texts.to(model.device)).squeeze()
+            predictions = model(texts.to(model.pretrained_model.device)).squeeze()
             preds = predictions.detach().to('cpu').numpy().argmax(1).tolist()
             y_true = ys.tolist()
             true.extend(y_true)
             pred.extend(preds)
 
     true = [model.mapper[x] for x in true]
     pred = [model.mapper[x] for x in pred]
 
     print(classification_report(true, pred, zero_division=0))
 
 
 def train(
-        model: BertCLF,
+        model: BaseCLF,
         iterator: torch.utils.data.DataLoader,
         optimizer: torch.optim,
         criterion: torch.nn,
         average: str = 'macro',
         other_metrics: Optional[Union[str, List[str]]] = None
-) -> Tuple[float, Optional[Dict[str, float]]]:
+) -> Tuple[np.ndarray, Optional[Dict[str, float]]]:
     """
     :param model: model architecture that you want to fine-tune
     :param iterator: iterator with data reserved for bert_clf
     :param optimizer: torch optimizer
     :param criterion: instance of torch-like loses
     :param average: type of averaging for f1 sklearn metric. Possible types are: 'micro', 'macro', 'weighted'
+    :param other_metrics: other metrics of your choice
     :return: mean metric for the bert_clf loop
     """
 
     epoch_loss = []
     epoch_f1 = []
     metrics = None
     if other_metrics is not None:
@@ -67,16 +69,16 @@
             raise ValueError("Other metrics can be only in list or str format")
 
     model.train()
 
     for texts, ys in tqdm(iterator, total=len(iterator), desc='Training loop'):
 
         optimizer.zero_grad()
-        predictions = model(texts.to(model.device))
-        loss = criterion(predictions, ys.to(model.device))
+        predictions = model(texts.to(model.pretrained_model.device))
+        loss = criterion(predictions, ys.to(model.pretrained_model.device))
 
         loss.backward()
         optimizer.step()
         preds = predictions.detach().to('cpu').numpy().argmax(1).tolist()
         y_true = ys.tolist()
 
         epoch_loss.append(loss.item())
@@ -88,26 +90,26 @@
     if metrics is not None:
         for k, v in metrics.items():
             metrics[k] = np.mean(v)
     return np.mean(epoch_f1), metrics
 
 
 def evaluate(
-        model: BertCLF,
+        model: BaseCLF,
         iterator: torch.utils.data.DataLoader,
         criterion: torch.nn,
         average: str = 'macro',
         other_metrics: Optional[Union[str, List[str]]] = None
 ) -> Tuple[np.ndarray, Optional[Dict[str, float]]]:
     """
     :param model: trained model (instance of class model.CLF)
     :param iterator: instance of torch.utils.data.DataLoader
     :param criterion: instance of torch-like loses
     :param average: type of averaging for f1 sklearn metric. Possible types are: 'micro', 'macro', 'weighted'
-    :param other_metrics: other metrics you would like to track. NOTE: they wouldn't affect the training provess
+    :param other_metrics: other metrics you would like to track. NOTE: they wouldn't affect the training process
     :return: mean metric for the evaluating loop
     """
 
     epoch_loss = []
     epoch_f1 = []
     metrics = None
 
@@ -129,16 +131,16 @@
                 metrics[m] = []
         else:
             raise ValueError("Other metrics can be only in list or str format")
 
     model.eval()
     with torch.no_grad():
         for texts, ys in tqdm(iterator, total=len(iterator), desc='Evaluating loop'):
-            predictions = model(texts.to(model.device))
-            loss = criterion(predictions, ys.to(model.device))
+            predictions = model(texts.to(model.pretrained_model.device))
+            loss = criterion(predictions, ys.to(model.pretrained_model.device))
             preds = predictions.detach().to('cpu').numpy().argmax(1).tolist()
             y_true = ys.tolist()
 
             epoch_loss.append(loss.item())
             epoch_f1.append(f1_score(y_true, preds, average=average))
             if metrics is not None:
                 for k in metrics:
@@ -148,15 +150,15 @@
         for k, v in metrics.items():
             metrics[k] = np.mean(v)
 
     return np.mean(epoch_f1), metrics
 
 
 def train_evaluate(
-        model: BertCLF,
+        model: BaseCLF,
         training_generator: torch.utils.data.DataLoader,
         valid_generator: torch.utils.data.DataLoader,
         criterion: torch.optim,
         optimizer: torch.nn,
         num_epochs: int,
         average: str,
         config: Dict[str, Union[Dict[str, Any], List[str]]]
```

### Comparing `bert-for-sequence-classification-0.0.5a0/bert_clf/utils.py` & `bert-for-sequence-classification-0.0.6a0/bert_clf/utils.py`

 * *Files identical despite different names*

### Comparing `bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/PKG-INFO` & `bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-for-sequence-classification
-Version: 0.0.5a0
+Version: 0.0.6a0
 Summary: Easy fine-tuning for BERT models
 Author: Tatiana Iazykova
 Author-email: tania_yazykova@bk.ru
 Keywords: python,bert,deep learning,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -74,42 +74,42 @@
 Otherwise:
 
 ```python
 
 import torch
 import json
 import pandas as pd
-from bert_clf.src.BertCLF import BertCLF
+from bert_clf.src.models.BertCLF import BertCLF
 from transformers import AutoModel, AutoTokenizer
 
-device = torch.device("cuda" if  torch.cuda.is_available() else "cpu")
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 tokenizer = AutoTokenizer.from_pretrained(
-        pretrained_model_name_or_path="pretrained_model_name_or_path"
-    )
+    pretrained_model_name_or_path="pretrained_model_name_or_path"
+)
 model_bert = AutoModel.from_pretrained(
     pretrained_model_name_or_path="pretrained_model_name_or_path"
 ).to(device)
 
-id2label = json.load(open("path/to/saved/mapper")) # mapper is saved with the state dict
+id2label = json.load(open("path/to/saved/mapper"))  # mapper is saved with the state dict
 
 model = BertCLF(
     pretrained_model=model_bert,
     tokenizer=tokenizer,
     id2label=id2label,
     dropout="some number",
     device=device
 )
 
 model.load_state_dict(
     torch.load(
-    "path_to_state_dict", map_location=device
+        "path_to_state_dict", map_location=device
     ),
     strict=False
 )
 
 model.eval()
-    
+
 df = pd.read_csv("path_to_some_df")
 
 df["target_column"] = df["text_column"].apply(model.predict)
 ```
```

### Comparing `bert-for-sequence-classification-0.0.5a0/bert_for_sequence_classification.egg-info/SOURCES.txt` & `bert-for-sequence-classification-0.0.6a0/bert_for_sequence_classification.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 bert_clf/__init__.py
 bert_clf/pipeline.py
 bert_clf/utils.py
-bert_clf/src/BertCLF.py
 bert_clf/src/__init__.py
 bert_clf/src/dataset.py
 bert_clf/src/early_stopping.py
 bert_clf/src/preparing_data_utils.py
 bert_clf/src/training_utils.py
-bert_clf/src/pandas_dataset/BaseDataset.py
+bert_clf/src/core/BaseDataset.py
+bert_clf/src/core/BaseModel.py
+bert_clf/src/core/CLFFabric.py
+bert_clf/src/core/__init__.py
+bert_clf/src/models/BertCLF.py
+bert_clf/src/models/EncoderCLF.py
+bert_clf/src/models/__init__.py
 bert_clf/src/pandas_dataset/PandasDataset.py
 bert_clf/src/pandas_dataset/SimpleDataFrame.py
 bert_clf/src/pandas_dataset/__init__.py
 bert_for_sequence_classification.egg-info/PKG-INFO
 bert_for_sequence_classification.egg-info/SOURCES.txt
 bert_for_sequence_classification.egg-info/dependency_links.txt
 bert_for_sequence_classification.egg-info/entry_points.txt
```

### Comparing `bert-for-sequence-classification-0.0.5a0/setup.py` & `bert-for-sequence-classification-0.0.6a0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bert-for-sequence-classification",
-    version='0.0.5a',
+    version='0.0.6a',
     author="Tatiana Iazykova",
     author_email="tania_yazykova@bk.ru",
     description='Easy fine-tuning for BERT models',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'bert-clf-train = bert_clf.pipeline:main',
         ],
     },
     install_requires=[
         'transformers>=4.2.0',
-        'torch>=1.7.1, != 1.10',
+        'torch>=1.7.1',
         'numpy>=1.19.5',
         'pandas>=1.1.5',
         'scikit-learn>=1.0',
         'pyyaml>=6.0',
         'openpyxl>=3.0.9',
     ],
```

