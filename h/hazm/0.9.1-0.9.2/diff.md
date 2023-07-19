# Comparing `tmp/hazm-0.9.1.tar.gz` & `tmp/hazm-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazm-0.9.1.tar", max compression
+gzip compressed data, was "hazm-0.9.2.tar", max compression
```

## Comparing `hazm-0.9.1.tar` & `hazm-0.9.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     2556 2023-06-29 06:34:44.278743 hazm-0.9.1/hazm/__init__.py
--rw-r--r--   0        0        0    12199 2023-06-29 06:34:44.278743 hazm-0.9.1/hazm/chunker.py
--rw-r--r--   0        0        0      600 2023-06-29 06:34:44.279745 hazm-0.9.1/hazm/corpus_readers/__init__.py
--rw-r--r--   0        0        0     4603 2023-06-29 06:34:44.280743 hazm-0.9.1/hazm/corpus_readers/bijankhan_reader.py
--rw-r--r--   0        0        0    17393 2023-06-29 06:34:44.281745 hazm-0.9.1/hazm/corpus_readers/dadegan_reader.py
--rw-r--r--   0        0        0     6504 2023-06-29 06:34:44.281745 hazm-0.9.1/hazm/corpus_readers/degarbayan_reader.py
--rw-r--r--   0        0        0     6302 2023-06-29 06:34:44.282742 hazm-0.9.1/hazm/corpus_readers/hamshahri_reader.py
--rw-r--r--   0        0        0     1910 2023-05-19 17:02:23.654234 hazm-0.9.1/hazm/corpus_readers/mirastext_reader.py
--rw-r--r--   0        0        0     1307 2023-05-20 09:29:17.536041 hazm-0.9.1/hazm/corpus_readers/persian_plain_text_reader.py
--rw-r--r--   0        0        0     3419 2023-05-19 17:02:23.657234 hazm-0.9.1/hazm/corpus_readers/persica_reader.py
--rw-r--r--   0        0        0    11969 2023-06-29 06:34:44.282742 hazm-0.9.1/hazm/corpus_readers/peykare_reader.py
--rw-r--r--   0        0        0     4495 2023-06-29 06:34:44.283743 hazm-0.9.1/hazm/corpus_readers/quran_reader.py
--rw-r--r--   0        0        0     4861 2023-06-29 06:34:44.283743 hazm-0.9.1/hazm/corpus_readers/sentipers_reader.py
--rw-r--r--   0        0        0     4731 2023-05-19 17:02:23.659233 hazm-0.9.1/hazm/corpus_readers/tnews_reader.py
--rw-r--r--   0        0        0    14949 2023-06-29 06:34:44.284743 hazm-0.9.1/hazm/corpus_readers/treebank_reader.py
--rw-r--r--   0        0        0     2799 2023-05-19 17:02:23.653233 hazm-0.9.1/hazm/corpus_readers/verbvalency_reader.py
--rw-r--r--   0        0        0    66091 2023-05-20 08:47:35.344846 hazm-0.9.1/hazm/corpus_readers/wiki_extractor.py
--rw-r--r--   0        0        0     3579 2023-05-19 17:02:23.651232 hazm-0.9.1/hazm/corpus_readers/wikipedia_reader.py
--rw-r--r--   0        0        0      682 2023-06-29 06:34:30.160053 hazm-0.9.1/hazm/data/iverbs.dat
--rw-r--r--   0        0        0     5415 2023-06-29 06:34:30.161054 hazm-0.9.1/hazm/data/iwords.dat
--rw-r--r--   0        0        0     4053 2023-04-21 06:10:37.576573 hazm-0.9.1/hazm/data/stopwords.dat
--rw-r--r--   0        0        0     3259 2023-06-29 07:11:56.484742 hazm-0.9.1/hazm/data/verbs.dat
--rw-r--r--   0        0        0   886268 2023-06-29 06:40:36.368810 hazm-0.9.1/hazm/data/words.dat
--rw-r--r--   0        0        0     8805 2023-06-29 06:34:44.285743 hazm-0.9.1/hazm/dependency_parser.py
--rw-r--r--   0        0        0    15980 2023-06-29 06:34:44.286745 hazm-0.9.1/hazm/embedding.py
--rw-r--r--   0        0        0    36919 2023-06-29 07:20:53.180758 hazm-0.9.1/hazm/informal_normalizer.py
--rw-r--r--   0        0        0   110303 2023-06-29 06:34:44.287745 hazm-0.9.1/hazm/lemmatizer.py
--rw-r--r--   0        0        0    25042 2023-06-29 06:34:44.288745 hazm-0.9.1/hazm/normalizer.py
--rw-r--r--   0        0        0    10216 2023-06-29 06:34:44.289742 hazm-0.9.1/hazm/pos_tagger.py
--rw-r--r--   0        0        0     1388 2023-05-19 10:59:52.643719 hazm-0.9.1/hazm/sentence_tokenizer.py
--rw-r--r--   0        0        0    17569 2023-05-24 17:29:45.481776 hazm-0.9.1/hazm/sequence_tagger.py
--rw-r--r--   0        0        0     2570 2023-05-24 10:34:28.735473 hazm-0.9.1/hazm/stemmer.py
--rw-r--r--   0        0        0     2659 2023-05-20 09:04:50.521923 hazm-0.9.1/hazm/token_splitter.py
--rw-r--r--   0        0        0     3133 2023-05-20 09:38:21.938503 hazm-0.9.1/hazm/utils.py
--rw-r--r--   0        0        0    14149 2023-05-20 09:01:45.137870 hazm-0.9.1/hazm/word_tokenizer.py
--rw-r--r--   0        0        0     1103 2023-05-05 07:10:08.350612 hazm-0.9.1/LICENSE
--rw-r--r--   0        0        0     4261 2023-06-29 07:35:28.487269 hazm-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4558 2023-06-29 06:34:44.270745 hazm-0.9.1/README.md
--rw-r--r--   0        0        0     5905 1970-01-01 00:00:00.000000 hazm-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-08 12:36:36.591071 hazm-0.9.2/LICENSE
+-rw-r--r--   0        0        0     6363 2023-07-08 12:36:36.591071 hazm-0.9.2/README.md
+-rw-r--r--   0        0        0     2500 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/__init__.py
+-rwxr-xr-x   0        0        0    11972 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/chunker.py
+-rw-r--r--   0        0        0      661 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/__init__.py
+-rw-r--r--   0        0        0     4501 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/bijankhan_reader.py
+-rw-r--r--   0        0        0    16978 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/dadegan_reader.py
+-rw-r--r--   0        0        0     6330 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/degarbayan_reader.py
+-rw-r--r--   0        0        0     6143 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/hamshahri_reader.py
+-rw-r--r--   0        0        0     1850 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/mirastext_reader.py
+-rw-r--r--   0        0        0     1267 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/persian_plain_text_reader.py
+-rw-r--r--   0        0        0     3316 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/persica_reader.py
+-rw-r--r--   0        0        0    11635 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/peykare_reader.py
+-rw-r--r--   0        0        0     4391 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/quran_reader.py
+-rw-r--r--   0        0        0     4738 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/sentipers_reader.py
+-rw-r--r--   0        0        0     4593 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/tnews_reader.py
+-rw-r--r--   0        0        0    15018 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/treebank_reader.py
+-rw-r--r--   0        0        0     2020 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/universal_dadegan_reader.py
+-rw-r--r--   0        0        0     2725 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/verbvalency_reader.py
+-rw-r--r--   0        0        0    64231 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/wiki_extractor.py
+-rw-r--r--   0        0        0     3479 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/corpus_readers/wikipedia_reader.py
+-rw-r--r--   0        0        0     2131 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/data/iverbs.dat
+-rw-r--r--   0        0        0     7613 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/data/iwords.dat
+-rw-r--r--   0        0        0     3664 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/data/stopwords.dat
+-rw-r--r--   0        0        0     9720 2023-07-08 12:36:36.663098 hazm-0.9.2/hazm/data/verbs.dat
+-rw-r--r--   0        0        0   850552 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/data/words.dat
+-rw-r--r--   0        0        0     8724 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/dependency_parser.py
+-rw-r--r--   0        0        0    19629 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/embedding.py
+-rw-r--r--   0        0        0    36078 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/informal_normalizer.py
+-rw-r--r--   0        0        0   107981 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/lemmatizer.py
+-rw-r--r--   0        0        0    24507 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/normalizer.py
+-rw-r--r--   0        0        0     9971 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/pos_tagger.py
+-rw-r--r--   0        0        0     1348 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/sentence_tokenizer.py
+-rw-r--r--   0        0        0    17158 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/sequence_tagger.py
+-rw-r--r--   0        0        0     2495 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/stemmer.py
+-rw-r--r--   0        0        0     2593 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/token_splitter.py
+-rw-r--r--   0        0        0     3027 2023-07-08 12:36:36.667100 hazm-0.9.2/hazm/utils.py
+-rw-r--r--   0        0        0    13819 2023-07-08 12:36:36.671101 hazm-0.9.2/hazm/word_tokenizer.py
+-rw-r--r--   0        0        0     4419 2023-07-08 12:36:36.671101 hazm-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     7860 1970-01-01 00:00:00.000000 hazm-0.9.2/PKG-INFO
```

### Comparing `hazm-0.9.1/hazm/__init__.py` & `hazm-0.9.2/hazm/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,77 @@
-"""entry point for the package."""
-
-from typing import List
-
-from hazm.utils import default_verbs
-from hazm.utils import default_words
-from hazm.utils import stopwords_list
-from hazm.utils import words_list
-from hazm.utils import maketrans
-from hazm.utils import regex_replace
-from hazm.utils import words_list
-from hazm.utils import NUMBERS
-from hazm.utils import informal_verbs
-from hazm.utils import informal_words
-
-from hazm.sequence_tagger import IOBTagger
-from hazm.sequence_tagger import SequenceTagger
-
-from hazm.pos_tagger import POSTagger
-from hazm.pos_tagger import StanfordPOSTagger
-
-from hazm.stemmer import Stemmer
-from hazm.word_tokenizer import WordTokenizer
-
-from hazm.lemmatizer import Conjugation
-from hazm.lemmatizer import Lemmatizer
-
-from hazm.normalizer import Normalizer
-
-from hazm.chunker import Chunker
-from hazm.chunker import RuleBasedChunker
-from hazm.chunker import tree2brackets
-
-from hazm.sentence_tokenizer import SentenceTokenizer
-
-def sent_tokenize(text: str) -> List[str]:
-    """Sentence Tokenizer."""
-    if not hasattr(sent_tokenize, "tokenizer"):
-        sent_tokenize.tokenizer = SentenceTokenizer()
-    return sent_tokenize.tokenizer.tokenize(text)
-
-
-def word_tokenize(sentence: str) -> List[str]:
-    """Word Tokenizer."""
-    if not hasattr(word_tokenize, "tokenizer"):
-        word_tokenize.tokenizer = WordTokenizer()
-    return word_tokenize.tokenizer.tokenize(sentence)
-
-from hazm.corpus_readers import PeykareReader
-from hazm.corpus_readers import BijankhanReader
-from hazm.corpus_readers import DadeganReader
-from hazm.corpus_readers import DegarbayanReader
-from hazm.corpus_readers import HamshahriReader
-from hazm.corpus_readers import MirasTextReader
-from hazm.corpus_readers import PersicaReader
-from hazm.corpus_readers import QuranReader
-from hazm.corpus_readers import SentiPersReader
-from hazm.corpus_readers import TNewsReader
-from hazm.corpus_readers import TreebankReader
-from hazm.corpus_readers import VerbValencyReader
-from hazm.corpus_readers import WikipediaReader
-from hazm.corpus_readers import persian_plain_text_reader
-
-from hazm.dependency_parser import DependencyParser
-from hazm.dependency_parser import MaltParser
-from hazm.dependency_parser import TurboParser
-
-from hazm.embedding import SentEmbedding
-from hazm.embedding import WordEmbedding
-
-from hazm.informal_normalizer import InformalLemmatizer
-from hazm.informal_normalizer import InformalNormalizer
-
-from hazm.token_splitter import TokenSplitter
-
-
+# ruff: noqa
+"""entry point for the package."""
+
+from typing import List
+
+from hazm.utils import default_verbs
+from hazm.utils import default_words
+from hazm.utils import stopwords_list
+from hazm.utils import words_list
+from hazm.utils import maketrans
+from hazm.utils import regex_replace
+from hazm.utils import words_list
+from hazm.utils import NUMBERS
+from hazm.utils import informal_verbs
+from hazm.utils import informal_words
+
+from hazm.sequence_tagger import IOBTagger
+from hazm.sequence_tagger import SequenceTagger
+
+from hazm.pos_tagger import POSTagger
+from hazm.pos_tagger import StanfordPOSTagger
+
+from hazm.stemmer import Stemmer
+from hazm.word_tokenizer import WordTokenizer
+
+from hazm.lemmatizer import Conjugation
+from hazm.lemmatizer import Lemmatizer
+
+from hazm.normalizer import Normalizer
+
+from hazm.chunker import Chunker
+from hazm.chunker import RuleBasedChunker
+from hazm.chunker import tree2brackets
+
+from hazm.sentence_tokenizer import SentenceTokenizer
+
+def sent_tokenize(text: str) -> List[str]:
+    """Sentence Tokenizer."""
+    if not hasattr(sent_tokenize, "tokenizer"):
+        sent_tokenize.tokenizer = SentenceTokenizer()
+    return sent_tokenize.tokenizer.tokenize(text)
+
+
+def word_tokenize(sentence: str) -> List[str]:
+    """Word Tokenizer."""
+    if not hasattr(word_tokenize, "tokenizer"):
+        word_tokenize.tokenizer = WordTokenizer()
+    return word_tokenize.tokenizer.tokenize(sentence)
+
+from hazm.corpus_readers import PeykareReader
+from hazm.corpus_readers import BijankhanReader
+from hazm.corpus_readers import DadeganReader
+from hazm.corpus_readers import UniversalDadeganReader
+from hazm.corpus_readers import DegarbayanReader
+from hazm.corpus_readers import HamshahriReader
+from hazm.corpus_readers import MirasTextReader
+from hazm.corpus_readers import PersicaReader
+from hazm.corpus_readers import QuranReader
+from hazm.corpus_readers import SentiPersReader
+from hazm.corpus_readers import TNewsReader
+from hazm.corpus_readers import TreebankReader
+from hazm.corpus_readers import VerbValencyReader
+from hazm.corpus_readers import persian_plain_text_reader
+
+from hazm.dependency_parser import DependencyParser
+from hazm.dependency_parser import MaltParser
+from hazm.dependency_parser import TurboParser
+
+from hazm.embedding import SentEmbedding
+from hazm.embedding import WordEmbedding
+
+from hazm.informal_normalizer import InformalLemmatizer
+from hazm.informal_normalizer import InformalNormalizer
+
+from hazm.token_splitter import TokenSplitter
+
+
```

### Comparing `hazm-0.9.1/hazm/chunker.py` & `hazm-0.9.2/hazm/chunker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,256 +1,258 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای تجزیهٔ متن به عبارات اسمی، فعلی و حرف
-اضافه‌ای است. **میزان دقت تجزیه‌گر سطحی در نسخهٔ حاضر ۹۳.۴ درصد [^1] است.**
-[^1]:
-این عدد با انتشار هر نسخه بروزرسانی می‌شود.
-
-"""
-
-from typing import Dict
-from typing import Iterator
-from typing import List
-from typing import Tuple
-from typing import Union
-
-from nltk.chunk import RegexpParser
-from nltk.chunk import conlltags2tree
-from nltk.chunk import tree2conlltags
-
-from hazm import POSTagger
-from hazm import IOBTagger
-
-
-def tree2brackets(tree: str) -> str:
-    """خروجی درختی تابع [parse()][hazm.chunker.Chunker.parse] را به یک ساختار
-    کروشه‌ای تبدیل می‌کند.
-
-    Examples:
-        >>> chunker = Chunker(model='resources/chunker.model')
-        >>> tree=chunker.parse([('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')])
-        >>> print(tree)
-        (S
-          (NP نامه/NOUN,EZ ایشان/PRON)
-          (POSTP را/ADP)
-          (VP دریافت/NOUN داشتم/VERB)
-          ./PUNCT)
-
-        >>> tree2brackets(tree)
-        '[نامه ایشان NP] [را POSTP] [دریافت داشتم VP] .'
-
-    Args:
-        tree: ساختار درختی حاصل از پردزاش تابع parse()
-
-    Returns:
-        رشته‌ای از کروشه‌ها که در هر کروشه جزئی از متن به همراه نوع آن جای گرفته است.
-
-    """
-    s, tag = "", ""
-    for item in tree2conlltags(tree):
-        if item[2][0] in {"B", "O"} and tag:
-            s += tag + "] "
-            tag = ""
-
-        if item[2][0] == "B":
-            tag = item[2].split("-")[1]
-            s += "["
-        s += item[0] + " "
-
-    if tag:
-        s += tag + "] "
-
-    return s.strip()
-
-
-class Chunker(IOBTagger):
-    """این کلاس شامل توابعی برای تقطیع متن، آموزش و ارزیابی مدل است."""
-
-    def __init__(
-        self: "Chunker",
-        model: str = None,
-        data_maker: List[List[Dict]] = None,
-    ) -> None:
-        """constructor."""
-        data_maker = self.data_maker if data_maker is None else data_maker
-        self.posTagger = POSTagger()
-        super().__init__(model, data_maker)
-
-    def data_maker(
-        self: "Chunker",
-        tokens: List[List[Tuple[str, str]]],
-    ) -> List[List[Dict]]:
-        """تابعی که لیستی دو بعدی از کلمات به همراه لیبل را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
-
-        Examples:
-            >>> chunker = Chunker(model = 'resources/chunker.model')
-            >>> chunker.data_maker(tokens = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]])
-            [[{'word': 'من', 'is_first': True, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'من', 'prefix-3': 'من', 'suffix-1': 'ن', 'suffix-2': 'من', 'suffix-3': 'من', 'prev_word': '', 'two_prev_word': '', 'next_word': 'به', 'two_next_word': 'مدرسه', 'is_numeric': False, 'prev_is_numeric': '', 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': '', 'next_is_punc': False, 'pos': 'PRON', 'prev_pos': '', 'next_pos': 'ADP'}, {'word': 'به', 'is_first': False, 'is_last': False, 'prefix-1': 'ب', 'prefix-2': 'به', 'prefix-3': 'به', 'suffix-1': 'ه', 'suffix-2': 'به', 'suffix-3': 'به', 'prev_word': 'من', 'two_prev_word': '.', 'next_word': 'مدرسه', 'two_next_word': 'ایران', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'ADP', 'prev_pos': 'PRON', 'next_pos': 'NOUN,EZ'}, {'word': 'مدرسه', 'is_first': False, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'مد', 'prefix-3': 'مدر', 'suffix-1': 'ه', 'suffix-2': 'سه', 'suffix-3': 'رسه', 'prev_word': 'به', 'two_prev_word': 'من', 'next_word': 'ایران', 'two_next_word': 'رفته_بودم', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'NOUN,EZ', 'prev_pos': 'ADP', 'next_pos': 'NOUN'}, {'word': 'ایران', 'is_first': False, 'is_last': False, 'prefix-1': 'ا', 'prefix-2': 'ای', 'prefix-3': 'ایر', 'suffix-1': 'ن', 'suffix-2': 'ان', 'suffix-3': 'ران', 'prev_word': 'مدرسه', 'two_prev_word': 'به', 'next_word': 'رفته_بودم', 'two_next_word': '.', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'NOUN', 'prev_pos': 'NOUN,EZ', 'next_pos': 'VERB'}, {'word': 'رفته_بودم', 'is_first': False, 'is_last': False, 'prefix-1': 'ر', 'prefix-2': 'رف', 'prefix-3': 'رفت', 'suffix-1': 'م', 'suffix-2': 'دم', 'suffix-3': 'ودم', 'prev_word': 'ایران', 'two_prev_word': 'مدرسه', 'next_word': '.', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': True, 'pos': 'VERB', 'prev_pos': 'NOUN', 'next_pos': 'PUNCT'}, {'word': '.', 'is_first': False, 'is_last': True, 'prefix-1': '.', 'prefix-2': '.', 'prefix-3': '.', 'suffix-1': '.', 'suffix-2': '.', 'suffix-3': '.', 'prev_word': 'رفته_بودم', 'two_prev_word': 'ایران', 'next_word': '', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': '', 'is_punc': True, 'prev_is_punc': False, 'next_is_punc': '', 'pos': 'PUNCT', 'prev_pos': 'VERB', 'next_pos': ''}]]
-
-        Args:
-            tokens: جملاتی که نیاز به تبدیل آن به برداری از ویژگی‌ها است.
-
-        Returns:
-            لیستی از لیستی از دیکشنری‌های بیان‌کننده ویژگی‌های یک کلمه.
-
-        """
-        words = [[word for word, _ in token] for token in tokens]
-        tags = [[tag for _, tag in token] for token in tokens]
-        return [
-            [
-                self.features(words=word_tokens, pos_tags=tag_tokens, index=index)
-                for index in range(len(word_tokens))
-            ]
-            for word_tokens, tag_tokens in zip(words, tags)
-        ]
-
-    def features(
-        self: "Chunker",
-        words: List[str],
-        pos_tags: List[str],
-        index: int,
-    ) -> Dict[str, Union[str, bool]]:
-        """ویژگی‌های کلمه را برمی‌گرداند."""
-        word_features = self.posTagger.features(words, index)
-        word_features.update(
-            {
-                "pos": pos_tags[index],
-                "prev_pos": "" if index == 0 else pos_tags[index - 1],
-                "next_pos": "" if index == len(pos_tags) - 1 else pos_tags[index + 1],
-            },
-        )
-        return word_features
-
-    def train(
-        self: "Chunker",
-        trees: List[str],
-        c1: float = 0.4,
-        c2: float = 0.04,
-        max_iteration: int = 400,
-        verbose: bool = True,
-        file_name: str = "chunker_crf.model",
-        report_duration: bool = True,
-    ) -> None:
-        """از روی درخت ورودی، مدل را آموزش می‌دهد.
-
-        Args:
-            trees: لیستی از درخت‌ها برای آموزش مدل.
-            c1: مقدار L1 regularization.
-            c2: مقدار L2 regularization.
-            max_iteration: تعداد تکرار آموزش بر کل دیتا.
-            verbose: نمایش اطلاعات مربوط به آموزش.
-            file_name: نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
-            report_duration: نمایش گزارشات مربوط به زمان.
-
-        """
-        return super().train(
-            [tree2conlltags(tree) for tree in trees],
-            c1,
-            c2,
-            max_iteration,
-            verbose,
-            file_name,
-            report_duration,
-        )
-
-    def parse(self: "Chunker", sentence: List[Tuple[str, str]]) -> str:
-        """جمله‌ای را در قالب لیستی از تاپل‌های دوتایی [(توکن, نوع), (توکن, نوع), ...]
-        دریافت می‌کند و درخت تقطع‌شدهٔ آن را بر می‌گرداند.
-
-        Examples:
-            >>> chunker = Chunker(model = 'resources/chunker.model')
-            >>> tree = chunker.parse(sentence = [('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')])
-            >>> print(tree)
-            (S
-              (NP نامه/NOUN,EZ ایشان/PRON)
-              (POSTP را/ADP)
-              (VP دریافت/NOUN داشتم/VERB)
-              ./PUNCT)
-
-        Args:
-            sentence: جمله‌ای که باید درخت تقطیع‌شدهٔ آن تولید شود.
-
-        Returns:
-            ساختار درختی حاصل از تقطیع.
-            برای تبدیل این ساختار درختی به یک ساختار کروشه‌ای و قابل‌درک‌تر
-            می‌توانید از تابع `tree2brackets()` استفاده کنید.
-
-        """
-        return conlltags2tree(super().tag(sentence))
-
-    def parse_sents(
-        self: "Chunker",
-        sentences: List[List[Tuple[str, str]]],
-    ) -> Iterator[str]:
-        """جملات ورودی را به‌شکل تقطیع‌شده و در قالب یک برمی‌گرداند.
-
-        Args:
-            sentences: جملات ورودی.
-
-        Yields:
-            یک `Iterator` از جملات تقطیع شده.
-
-        """
-        for conlltagged in super().tag_sents(sentences):
-            yield conlltags2tree(conlltagged)
-
-    def evaluate(self: "Chunker", trees: List[str]) -> float:
-        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
-
-        Examples:
-            >>> chunker = Chunker(model = 'resources/chunker.model')
-            >>> trees = list(chunker.parse_sents([[('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')]]))
-            >>> chunker.evaluate(trees)
-            1.0
-
-        Args:
-            trees: لیست درختانی که با استفاده از آن مدل را ارزیابی می‌کنیم.
-
-        Returns:
-            دقت مدل
-
-        """
-        return super().evaluate([tree2conlltags(tree) for tree in trees])
-
-
-class RuleBasedChunker(RegexpParser):
-    """کلاس RuleBasedChunker.
-
-
-    Examples:
-    >>> chunker = RuleBasedChunker()
-    >>> tree2brackets(chunker.parse([('نامه', 'Ne'), ('۱۰', 'NUMe'), ('فوریه', 'Ne'), ('شما', 'PRO'), ('را', 'POSTP'), ('دریافت', 'N'), ('داشتم', 'V'), ('.', 'PUNC')]))
-    '[نامه ۱۰ فوریه شما NP] [را POSTP] [دریافت داشتم VP] .'
-
-    """
-
-    def __init__(self: "RuleBasedChunker") -> None:
-        """Init."""
-        grammar = r"""
-
-            NP:
-                <P>{<N>}<V>
-
-            VP:
-                <.*[^e]>{<N>?<V>}
-                {<V>}
-
-            ADVP:
-                {<ADVe?><AJ>?}
-
-            ADJP:
-                <.*[^e]>{<AJe?>}
-
-            NP:
-                {<DETe?|Ne?|NUMe?|AJe|PRO|CL|RESe?><DETe?|Ne?|NUMe?|AJe?|PRO|CL|RESe?>*}
-                <N>}{<.*e?>
-
-            ADJP:
-                {<AJe?>}
-
-            POSTP:
-                {<POSTP>}
-
-            PP:
-                {<Pe?>+}
-
-        """
-
-        super().__init__(grammar=grammar)
+# ruff: noqa: EXE002
+"""این ماژول شامل کلاس‌ها و توابعی برای تجزیهٔ متن به عبارات اسمی، فعلی و حرف
+اضافه‌ای است. **میزان دقت تجزیه‌گر سطحی در نسخهٔ حاضر ۹۳.۴ درصد [^1] است.**
+[^1]:
+این عدد با انتشار هر نسخه بروزرسانی می‌شود.
+
+"""
+
+from typing import Dict
+from typing import Iterator
+from typing import List
+from typing import Optional
+from typing import Tuple
+from typing import Union
+
+from nltk.chunk import RegexpParser
+from nltk.chunk import conlltags2tree
+from nltk.chunk import tree2conlltags
+
+from hazm import IOBTagger
+from hazm import POSTagger
+
+
+def tree2brackets(tree: str) -> str:
+    """خروجی درختی تابع [parse()][hazm.chunker.Chunker.parse] را به یک ساختار
+    کروشه‌ای تبدیل می‌کند.
+
+    Examples:
+        >>> chunker = Chunker(model='chunker.model')
+        >>> tree=chunker.parse([('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')])
+        >>> print(tree)
+        (S
+          (NP نامه/NOUN,EZ ایشان/PRON)
+          (POSTP را/ADP)
+          (VP دریافت/NOUN داشتم/VERB)
+          ./PUNCT)
+
+        >>> tree2brackets(tree)
+        '[نامه ایشان NP] [را POSTP] [دریافت داشتم VP] .'
+
+    Args:
+        tree: ساختار درختی حاصل از پردزاش تابع parse()
+
+    Returns:
+        رشته‌ای از کروشه‌ها که در هر کروشه جزئی از متن به همراه نوع آن جای گرفته است.
+
+    """
+    s, tag = "", ""
+    for item in tree2conlltags(tree):
+        if item[2][0] in {"B", "O"} and tag:
+            s += tag + "] "
+            tag = ""
+
+        if item[2][0] == "B":
+            tag = item[2].split("-")[1]
+            s += "["
+        s += item[0] + " "
+
+    if tag:
+        s += tag + "] "
+
+    return s.strip()
+
+
+class Chunker(IOBTagger):
+    """این کلاس شامل توابعی برای تقطیع متن، آموزش و ارزیابی مدل است."""
+
+    def __init__(
+        self: "Chunker",
+        model: Optional[str] = None,
+        data_maker: Optional[List[List[Dict]]] = None,
+    ) -> None:
+        """constructor."""
+        data_maker = self.data_maker if data_maker is None else data_maker
+        self.posTagger = POSTagger()
+        super().__init__(model, data_maker)
+
+    def data_maker(
+        self: "Chunker",
+        tokens: List[List[Tuple[str, str]]],
+    ) -> List[List[Dict]]:
+        """تابعی که لیستی دو بعدی از کلمات به همراه لیبل را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
+
+        Examples:
+            >>> chunker = Chunker(model = 'chunker.model')
+            >>> chunker.data_maker(tokens = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]])
+            [[{'word': 'من', 'is_first': True, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'من', 'prefix-3': 'من', 'suffix-1': 'ن', 'suffix-2': 'من', 'suffix-3': 'من', 'prev_word': '', 'two_prev_word': '', 'next_word': 'به', 'two_next_word': 'مدرسه', 'is_numeric': False, 'prev_is_numeric': '', 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': '', 'next_is_punc': False, 'pos': 'PRON', 'prev_pos': '', 'next_pos': 'ADP'}, {'word': 'به', 'is_first': False, 'is_last': False, 'prefix-1': 'ب', 'prefix-2': 'به', 'prefix-3': 'به', 'suffix-1': 'ه', 'suffix-2': 'به', 'suffix-3': 'به', 'prev_word': 'من', 'two_prev_word': '.', 'next_word': 'مدرسه', 'two_next_word': 'ایران', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'ADP', 'prev_pos': 'PRON', 'next_pos': 'NOUN,EZ'}, {'word': 'مدرسه', 'is_first': False, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'مد', 'prefix-3': 'مدر', 'suffix-1': 'ه', 'suffix-2': 'سه', 'suffix-3': 'رسه', 'prev_word': 'به', 'two_prev_word': 'من', 'next_word': 'ایران', 'two_next_word': 'رفته_بودم', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'NOUN,EZ', 'prev_pos': 'ADP', 'next_pos': 'NOUN'}, {'word': 'ایران', 'is_first': False, 'is_last': False, 'prefix-1': 'ا', 'prefix-2': 'ای', 'prefix-3': 'ایر', 'suffix-1': 'ن', 'suffix-2': 'ان', 'suffix-3': 'ران', 'prev_word': 'مدرسه', 'two_prev_word': 'به', 'next_word': 'رفته_بودم', 'two_next_word': '.', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False, 'pos': 'NOUN', 'prev_pos': 'NOUN,EZ', 'next_pos': 'VERB'}, {'word': 'رفته_بودم', 'is_first': False, 'is_last': False, 'prefix-1': 'ر', 'prefix-2': 'رف', 'prefix-3': 'رفت', 'suffix-1': 'م', 'suffix-2': 'دم', 'suffix-3': 'ودم', 'prev_word': 'ایران', 'two_prev_word': 'مدرسه', 'next_word': '.', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': True, 'pos': 'VERB', 'prev_pos': 'NOUN', 'next_pos': 'PUNCT'}, {'word': '.', 'is_first': False, 'is_last': True, 'prefix-1': '.', 'prefix-2': '.', 'prefix-3': '.', 'suffix-1': '.', 'suffix-2': '.', 'suffix-3': '.', 'prev_word': 'رفته_بودم', 'two_prev_word': 'ایران', 'next_word': '', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': '', 'is_punc': True, 'prev_is_punc': False, 'next_is_punc': '', 'pos': 'PUNCT', 'prev_pos': 'VERB', 'next_pos': ''}]]
+
+        Args:
+            tokens: جملاتی که نیاز به تبدیل آن به برداری از ویژگی‌ها است.
+
+        Returns:
+            لیستی از لیستی از دیکشنری‌های بیان‌کننده ویژگی‌های یک کلمه.
+
+        """
+        words = [[word for word, _ in token] for token in tokens]
+        tags = [[tag for _, tag in token] for token in tokens]
+        return [
+            [
+                self.features(words=word_tokens, pos_tags=tag_tokens, index=index)
+                for index in range(len(word_tokens))
+            ]
+            for word_tokens, tag_tokens in zip(words, tags)
+        ]
+
+    def features(
+        self: "Chunker",
+        words: List[str],
+        pos_tags: List[str],
+        index: int,
+    ) -> Dict[str, Union[str, bool]]:
+        """ویژگی‌های کلمه را برمی‌گرداند."""
+        word_features = self.posTagger.features(words, index)
+        word_features.update(
+            {
+                "pos": pos_tags[index],
+                "prev_pos": "" if index == 0 else pos_tags[index - 1],
+                "next_pos": "" if index == len(pos_tags) - 1 else pos_tags[index + 1],
+            },
+        )
+        return word_features
+
+    def train(
+        self: "Chunker",
+        trees: List[str],
+        c1: float = 0.4,
+        c2: float = 0.04,
+        max_iteration: int = 400,
+        verbose: bool = True,
+        file_name: str = "chunker_crf.model",
+        report_duration: bool = True,
+    ) -> None:
+        """از روی درخت ورودی، مدل را آموزش می‌دهد.
+
+        Args:
+            trees: لیستی از درخت‌ها برای آموزش مدل.
+            c1: مقدار L1 regularization.
+            c2: مقدار L2 regularization.
+            max_iteration: تعداد تکرار آموزش بر کل دیتا.
+            verbose: نمایش اطلاعات مربوط به آموزش.
+            file_name: نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
+            report_duration: نمایش گزارشات مربوط به زمان.
+
+        """
+        return super().train(
+            [tree2conlltags(tree) for tree in trees],
+            c1,
+            c2,
+            max_iteration,
+            verbose,
+            file_name,
+            report_duration,
+        )
+
+    def parse(self: "Chunker", sentence: List[Tuple[str, str]]) -> str:
+        """جمله‌ای را در قالب لیستی از تاپل‌های دوتایی [(توکن, نوع), (توکن, نوع), ...]
+        دریافت می‌کند و درخت تقطع‌شدهٔ آن را بر می‌گرداند.
+
+        Examples:
+            >>> chunker = Chunker(model = 'chunker.model')
+            >>> tree = chunker.parse(sentence = [('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')])
+            >>> print(tree)
+            (S
+              (NP نامه/NOUN,EZ ایشان/PRON)
+              (POSTP را/ADP)
+              (VP دریافت/NOUN داشتم/VERB)
+              ./PUNCT)
+
+        Args:
+            sentence: جمله‌ای که باید درخت تقطیع‌شدهٔ آن تولید شود.
+
+        Returns:
+            ساختار درختی حاصل از تقطیع.
+            برای تبدیل این ساختار درختی به یک ساختار کروشه‌ای و قابل‌درک‌تر
+            می‌توانید از تابع `tree2brackets()` استفاده کنید.
+
+        """
+        return conlltags2tree(super().tag(sentence))
+
+    def parse_sents(
+        self: "Chunker",
+        sentences: List[List[Tuple[str, str]]],
+    ) -> Iterator[str]:
+        """جملات ورودی را به‌شکل تقطیع‌شده و در قالب یک برمی‌گرداند.
+
+        Args:
+            sentences: جملات ورودی.
+
+        Yields:
+            یک `Iterator` از جملات تقطیع شده.
+
+        """
+        for conlltagged in super().tag_sents(sentences):
+            yield conlltags2tree(conlltagged)
+
+    def evaluate(self: "Chunker", trees: List[str]) -> float:
+        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
+
+        Examples:
+            >>> chunker = Chunker(model = 'chunker.model')
+            >>> trees = list(chunker.parse_sents([[('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')]]))
+            >>> chunker.evaluate(trees)
+            1.0
+
+        Args:
+            trees: لیست درختانی که با استفاده از آن مدل را ارزیابی می‌کنیم.
+
+        Returns:
+            دقت مدل
+
+        """
+        return super().evaluate([tree2conlltags(tree) for tree in trees])
+
+
+class RuleBasedChunker(RegexpParser):
+    """کلاس RuleBasedChunker.
+
+
+    Examples:
+    >>> chunker = RuleBasedChunker()
+    >>> tree2brackets(chunker.parse([('نامه', 'Ne'), ('۱۰', 'NUMe'), ('فوریه', 'Ne'), ('شما', 'PRO'), ('را', 'POSTP'), ('دریافت', 'N'), ('داشتم', 'V'), ('.', 'PUNC')]))
+    '[نامه ۱۰ فوریه شما NP] [را POSTP] [دریافت داشتم VP] .'
+
+    """
+
+    def __init__(self: "RuleBasedChunker") -> None:
+        """Init."""
+        grammar = r"""
+
+            NP:
+                <P>{<N>}<V>
+
+            VP:
+                <.*[^e]>{<N>?<V>}
+                {<V>}
+
+            ADVP:
+                {<ADVe?><AJ>?}
+
+            ADJP:
+                <.*[^e]>{<AJe?>}
+
+            NP:
+                {<DETe?|Ne?|NUMe?|AJe|PRO|CL|RESe?><DETe?|Ne?|NUMe?|AJe?|PRO|CL|RESe?>*}
+                <N>}{<.*e?>
+
+            ADJP:
+                {<AJe?>}
+
+            POSTP:
+                {<POSTP>}
+
+            PP:
+                {<Pe?>+}
+
+        """
+
+        super().__init__(grammar=grammar)
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/__init__.py` & `hazm-0.9.2/hazm/corpus_readers/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-"""init."""
-from .bijankhan_reader import BijankhanReader
-from .dadegan_reader import DadeganReader
-from .degarbayan_reader import DegarbayanReader
-from .hamshahri_reader import HamshahriReader
-from .mirastext_reader import MirasTextReader
-from .persica_reader import PersicaReader
-from .peykare_reader import PeykareReader
-from .quran_reader import QuranReader
-from .sentipers_reader import SentiPersReader
-from .tnews_reader import TNewsReader
-from .treebank_reader import TreebankReader
-from .verbvalency_reader import VerbValencyReader
-from .wikipedia_reader import WikipediaReader
+# ruff: noqa
+
+"""init."""
+from .bijankhan_reader import BijankhanReader
+from .dadegan_reader import DadeganReader
+from .universal_dadegan_reader import UniversalDadeganReader
+from .degarbayan_reader import DegarbayanReader
+from .hamshahri_reader import HamshahriReader
+from .mirastext_reader import MirasTextReader
+from .persica_reader import PersicaReader
+from .peykare_reader import PeykareReader
+from .quran_reader import QuranReader
+from .sentipers_reader import SentiPersReader
+from .tnews_reader import TNewsReader
+from .treebank_reader import TreebankReader
+from .verbvalency_reader import VerbValencyReader
+from .wikipedia_reader import WikipediaReader
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/bijankhan_reader.py` & `hazm-0.9.2/hazm/corpus_readers/bijankhan_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,135 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ بی‌جن‌خان است.
-
-[پیکرهٔ
-بی‌جن‌خان](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-
-%D8%A8%DB%8C%E2%80%8C%D8%AC%D9%86%E2%80%8C%D8%AE%D8%A7%D9%86) مجموعه‌ای
-است از متون فارسی شامل بیش از ۲ میلیون و ۶۰۰ هزار کلمه که با ۵۵۰ نوع برچسب POS
-برچسب‌گذاری شده‌اند. این پیکره که در پژوهشکدهٔ پردازش هوشمند علائم تهیه شده است
-همچنین شامل بیش از ۴۳۰۰ تگ موضوعی چون سیاسی، تاریخی و ... برای متون است.
-
-"""
-
-import re
-from pathlib import Path
-from typing import Iterator
-from typing import List
-from typing import Tuple
-
-from hazm import Normalizer
-from .peykare_reader import join_verb_parts
-
-default_pos_map = {
-    "ADJ": "ADJ",
-    "ADJ_CMPR": "ADJ",
-    "ADJ_INO": "ADJ",
-    "ADJ_ORD": "ADJ",
-    "ADJ_SIM": "ADJ",
-    "ADJ_SUP": "ADJ",
-    "ADV": "ADV",
-    "ADV_EXM": "ADV",
-    "ADV_I": "ADV",
-    "ADV_NEGG": "ADV",
-    "ADV_NI": "ADV",
-    "ADV_TIME": "ADV",
-    "AR": "AR",
-    "CON": "CONJ",
-    "DEFAULT": "DEFAULT",
-    "DELM": "PUNC",
-    "DET": "PREP",
-    "IF": "IF",
-    "INT": "INT",
-    "MORP": "MORP",
-    "MQUA": "MQUA",
-    "MS": "MS",
-    "N_PL": "N",
-    "N_SING": "N",
-    "NN": "NN",
-    "NP": "NP",
-    "OH": "OH",
-    "OHH": "OHH",
-    "P": "PREP",
-    "PP": "PP",
-    "PRO": "PR",
-    "PS": "PS",
-    "QUA": "QUA",
-    "SPEC": "SPEC",
-    "V_AUX": "V",
-    "V_IMP": "V",
-    "V_PA": "V",
-    "V_PRE": "V",
-    "V_PRS": "V",
-    "V_SUB": "V",
-}
-
-
-class BijankhanReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ بی‌جن‌خان است.
-
-    Args:
-        bijankhan_file: مسیر فایلِ پیکره.
-        joined_verb_parts: اگر `True‍` باشد افعال چندبخشی را با _ به‌هم می‌چسباند.
-        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
-
-    """
-
-    def __init__(
-        self: "BijankhanReader",
-        bijankhan_file: str,
-        joined_verb_parts: bool = True,
-        pos_map: str = None,
-    ) -> None:
-        """Init."""
-        if pos_map is None:
-            pos_map = default_pos_map
-        self._bijankhan_file = bijankhan_file
-        self._joined_verb_parts = joined_verb_parts
-        self._pos_map = pos_map
-        self._normalizer = Normalizer(correct_spacing=False)
-
-    def _sentences(self: "BijankhanReader") -> Iterator[List[Tuple[str, str]]]:
-        """جملات پیکره را به شکل متن خام برمی‌گرداند.
-
-        Yields:
-            جملهٔ بعدی.
-
-        """
-        sentence = []
-        with Path(self._bijankhan_file).open(encoding="utf-8") as f:
-            length = 2
-            for line in f:
-                parts = re.split("  +", line.strip())
-                if len(parts) == length:
-                    word, tag = parts
-                    if word not in ("#", "*"):
-                        word = self._normalizer.normalize(word)
-                        sentence.append((word if word else "_", tag))
-                    if (
-                        tag == "DELM"
-                        and word in ("#", "*", ".", "؟", "!")
-                        and len(sentence)
-                    ):
-                        yield sentence
-                        sentence = []
-
-    def sents(self: "BijankhanReader") -> Iterator[List[Tuple[str, str]]]:
-        """جملات پیکره را به شکل لیستی از `(توکن،برچسب)`ها برمی‌گرداند..
-
-        Examples:
-            >>> bijankhan = BijankhanReader(bijankhan_file='corpora/bijankhan.txt')
-            >>> next(bijankhan.sents())
-            [('اولین', 'ADJ'), ('سیاره', 'N'), ('خارج', 'ADJ'), ('از', 'PREP'), ('منظومه', 'N'), ('شمسی', 'ADJ'), ('دیده_شد', 'V'), ('.', 'PUNC')]
-
-        Yields:
-            جملهٔ بعدی در قالب لیستی از `(توکن،برچسب)`ها.
-
-        """
-
-        def map_poses(item: Tuple[str, str]) -> Tuple[str, str]:
-            return (item[0], self._pos_map.get(item[1], item[1]))
-
-        for sentence in self._sentences():
-            if self._joined_verb_parts:
-                sentence = join_verb_parts(sentence)
-            yield list(map(map_poses, sentence))
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ بی‌جن‌خان است.
+
+[پیکرهٔ
+بی‌جن‌خان](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-
+%D8%A8%DB%8C%E2%80%8C%D8%AC%D9%86%E2%80%8C%D8%AE%D8%A7%D9%86) مجموعه‌ای
+است از متون فارسی شامل بیش از ۲ میلیون و ۶۰۰ هزار کلمه که با ۵۵۰ نوع برچسب POS
+برچسب‌گذاری شده‌اند. این پیکره که در پژوهشکدهٔ پردازش هوشمند علائم تهیه شده است
+همچنین شامل بیش از ۴۳۰۰ تگ موضوعی چون سیاسی، تاریخی و ... برای متون است.
+
+"""
+
+import re
+from pathlib import Path
+from typing import Iterator
+from typing import List
+from typing import Optional
+from typing import Tuple
+
+from hazm import Normalizer
+
+from .peykare_reader import join_verb_parts
+
+default_pos_map = {
+    "ADJ": "ADJ",
+    "ADJ_CMPR": "ADJ",
+    "ADJ_INO": "ADJ",
+    "ADJ_ORD": "ADJ",
+    "ADJ_SIM": "ADJ",
+    "ADJ_SUP": "ADJ",
+    "ADV": "ADV",
+    "ADV_EXM": "ADV",
+    "ADV_I": "ADV",
+    "ADV_NEGG": "ADV",
+    "ADV_NI": "ADV",
+    "ADV_TIME": "ADV",
+    "AR": "AR",
+    "CON": "CONJ",
+    "DEFAULT": "DEFAULT",
+    "DELM": "PUNC",
+    "DET": "PREP",
+    "IF": "IF",
+    "INT": "INT",
+    "MORP": "MORP",
+    "MQUA": "MQUA",
+    "MS": "MS",
+    "N_PL": "N",
+    "N_SING": "N",
+    "NN": "NN",
+    "NP": "NP",
+    "OH": "OH",
+    "OHH": "OHH",
+    "P": "PREP",
+    "PP": "PP",
+    "PRO": "PR",
+    "PS": "PS",
+    "QUA": "QUA",
+    "SPEC": "SPEC",
+    "V_AUX": "V",
+    "V_IMP": "V",
+    "V_PA": "V",
+    "V_PRE": "V",
+    "V_PRS": "V",
+    "V_SUB": "V",
+}
+
+
+class BijankhanReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ بی‌جن‌خان است.
+
+    Args:
+        bijankhan_file: مسیر فایلِ پیکره.
+        joined_verb_parts: اگر `True‍` باشد افعال چندبخشی را با _ به‌هم می‌چسباند.
+        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
+
+    """
+
+    def __init__(
+        self: "BijankhanReader",
+        bijankhan_file: str,
+        joined_verb_parts: bool = True,
+        pos_map: Optional[str] = None,
+    ) -> None:
+        """Init."""
+        if pos_map is None:
+            pos_map = default_pos_map
+        self._bijankhan_file = bijankhan_file
+        self._joined_verb_parts = joined_verb_parts
+        self._pos_map = pos_map
+        self._normalizer = Normalizer(correct_spacing=False)
+
+    def _sentences(self: "BijankhanReader") -> Iterator[List[Tuple[str, str]]]:
+        """جملات پیکره را به شکل متن خام برمی‌گرداند.
+
+        Yields:
+            جملهٔ بعدی.
+
+        """
+        sentence = []
+        with Path(self._bijankhan_file).open(encoding="utf-8") as f:
+            length = 2
+            for line in f:
+                parts = re.split("  +", line.strip())
+                if len(parts) == length:
+                    word, tag = parts
+                    if word not in ("#", "*"):
+                        word = self._normalizer.normalize(word)
+                        sentence.append((word if word else "_", tag))
+                    if (
+                        tag == "DELM"
+                        and word in ("#", "*", ".", "؟", "!")
+                        and len(sentence)
+                    ):
+                        yield sentence
+                        sentence = []
+
+    def sents(self: "BijankhanReader") -> Iterator[List[Tuple[str, str]]]:
+        """جملات پیکره را به شکل لیستی از `(توکن،برچسب)`ها برمی‌گرداند..
+
+        Examples:
+            >>> bijankhan = BijankhanReader(bijankhan_file='bijankhan.txt')
+            >>> next(bijankhan.sents())
+            [('اولین', 'ADJ'), ('سیاره', 'N'), ('خارج', 'ADJ'), ('از', 'PREP'), ('منظومه', 'N'), ('شمسی', 'ADJ'), ('دیده_شد', 'V'), ('.', 'PUNC')]
+
+        Yields:
+            جملهٔ بعدی در قالب لیستی از `(توکن،برچسب)`ها.
+
+        """
+
+        def map_poses(item: Tuple[str, str]) -> Tuple[str, str]:
+            return (item[0], self._pos_map.get(item[1], item[1]))
+
+        for sentence in self._sentences():
+            if self._joined_verb_parts:
+                sentence = join_verb_parts(sentence)
+            yield list(map(map_poses, sentence))
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/dadegan_reader.py` & `hazm-0.9.2/hazm/corpus_readers/dadegan_reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,414 +1,414 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ PerDT است.
-
-PerDT حاوی تعداد قابل‌توجهی جملۀ برچسب‌خورده با اطلاعات نحوی و ساخت‌واژی است.
-
-"""
-from pathlib import Path
-from typing import Any
-from typing import Dict
-from typing import Iterator
-from typing import List
-from typing import Tuple
-from typing import Type
-
-from nltk.parse import DependencyGraph
-from nltk.tree import Tree
-
-
-def coarse_pos_u(tags: List[str], word: str) -> str:
-    """برچسب‌های ریز را به برچسب‌های درشت منطبق با استاندارد جهانی (coarse-grained
-    universal pos tags) تبدیل می‌کند.
-
-    Examples:
-        >>> coarse_pos_e(['N', 'IANM'], 'امروز')
-        'N'
-
-    """
-    mapping = {
-        "N": "NOUN",
-        "V": "VERB",
-        "ADJ": "ADJ",
-        "ADV": "ADV",
-        "PR": "PRON",
-        "PREM": "DET",
-        "PREP": "ADP",
-        "POSTP": "ADP",
-        "PRENUM": "NUM",
-        "CONJ": "CCONJ",
-        "PUNC": "PUNCT",
-        "SUBR": "SCONJ",
-        "IDEN": "PROPN",
-        "POSTNUM": "NUM",
-        "PSUS": "INTJ",
-        "PART": "PART",
-        "ADR": "INTJ",
-    }
-    pos_mapped = mapping.get(tags[0], "X")
-    if pos_mapped == "PART" and word == "را":
-        return "ADP"
-    if pos_mapped == "PART" and word in ["خوب", "آخر"]:
-        return "ADP"
-    return pos_mapped
-
-
-def coarse_pos_e(tags: List[str], word) -> str:
-    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
-
-    Examples:
-        >>> coarse_pos_e(['N', 'IANM'],'امروز')
-        'N'
-
-    """
-    mapping = {
-        "N": "N",
-        "V": "V",
-        "ADJ": "AJ",
-        "ADV": "ADV",
-        "PR": "PRO",
-        "PREM": "DET",
-        "PREP": "P",
-        "POSTP": "POSTP",
-        "PRENUM": "NUM",
-        "CONJ": "CONJ",
-        "PUNC": "PUNC",
-        "SUBR": "CONJ",
-    }
-    return mapping.get(tags[0], "X") + ("e" if "EZ" in tags else "")
-
-
-def word_nodes(tree: Type[Tree]) -> List[Dict[str, Any]]:
-    """نودها را به صورت مرتب‌شده برمی‌گرداند."""
-    return sorted(tree.nodes.values(), key=lambda node: node["address"])[1:]
-
-
-def node_deps(node: List[Dict[str, Any]]) -> List[Any]:
-    """مقادیر موجود در فیلد deps نود ورودی را برمی‌گرداند."""
-    return sum(list(node["deps"].values()), [])
-
-
-class DadeganReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ PerDT است.
-
-    Args:
-        conll_file: مسیر فایلِ پیکره.
-        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
-
-    """
-
-    def __init__(
-        self: "DadeganReader",
-        conll_file: str,
-        pos_map: str = coarse_pos_e,
-        universal_pos: bool = False,
-    ) -> None:
-        self._conll_file = conll_file
-        if pos_map is None:
-            self._pos_map = lambda tags: ",".join(tags)
-        elif universal_pos:
-            self._pos_map = coarse_pos_u
-        else:
-            self._pos_map = coarse_pos_e
-
-    def _sentences(self: "DadeganReader") -> Iterator[str]:
-        """جملات پیکره را به شکل متن خام برمی‌گرداند.
-
-        Yields:
-            جملهٔ بعدی.
-
-        """
-        with Path(self._conll_file).open(encoding="utf8") as conll_file:
-            text = conll_file.read()
-
-            # refine text
-            text = (
-                text.replace("‌‌", "‌")
-                .replace("\t‌", "\t")
-                .replace("‌\t", "\t")
-                .replace("\t ", "\t")
-                .replace(" \t", "\t")
-                .replace("\r", "")
-                .replace("\u2029", "‌")
-            )
-
-            for item in text.replace(" ", "_").split("\n\n"):
-                if item.strip():
-                    yield item
-
-    def trees(self: "DadeganReader") -> Iterator[Type[Tree]]:
-        """ساختار درختی جملات را برمی‌گرداند.
-
-        Yields:
-            ساختار درختی جملهٔ بعدی.
-
-        """
-        for sentence in self._sentences():
-            tree = DependencyGraph(sentence)
-
-            for node in word_nodes(tree):
-                node["mtag"] = [node["ctag"], node["tag"]]
-
-                if "ezafe" in node["feats"]:
-                    node["mtag"].append("EZ")
-
-                node["mtag"] = self._pos_map(node["mtag"], node["word"])
-
-            yield tree
-
-    def sents(self: "DadeganReader") -> Iterator[List[Tuple[str, str]]]:
-        """لیستی از جملات را برمی‌گرداند.
-
-        هر جمله لیستی از `(توکن، برچسب)`ها است.
-
-        Examples:
-            >>> dadegan = DadeganReader(conll_file='corpora/dadegan.conll')
-            >>> next(dadegan.sents())
-            [('این', 'DET'), ('میهمانی', 'N'), ('به', 'P'), ('منظور', 'Ne'), ('آشنایی', 'Ne'), ('هم‌تیمی‌های', 'Ne'), ('او', 'PRO'), ('با', 'P'), ('غذاهای', 'Ne'), ('ایرانی', 'AJ'), ('ترتیب', 'N'), ('داده_شد', 'V'), ('.', 'PUNC')]
-
-        Yields:
-            جملهٔ بعدی.
-
-        """
-        for tree in self.trees():
-            yield [(node["word"], node["mtag"]) for node in word_nodes(tree)]
-
-    def chunked_trees(self: "DadeganReader") -> Iterator[Type[Tree]]:
-        """درخت وابستگی‌های جملات را برمی‌گرداند.
-
-        Examples:
-            >>> from hazm.chunker import tree2brackets
-            >>> dadegan = DadeganReader(conll_file='corpora/dadegan.conll')
-            >>> tree2brackets(next(dadegan.chunked_trees()))
-            '[این میهمانی NP] [به PP] [منظور آشنایی هم‌تیمی‌های او NP] [با PP] [غذاهای ایرانی NP] [ترتیب داده_شد VP] .'
-
-        Yields:
-            درخت وابستگی‌های جملهٔ بعدی.
-
-        """
-        for tree in self.trees():
-            chunks = []
-            for node in word_nodes(tree):
-                n = node["address"]
-                item = (node["word"], node["mtag"])
-                appended = False
-                if node["ctag"] in {"PREP", "POSTP"}:
-                    for d in node_deps(node):
-                        label = "PP"
-                        if node["ctag"] == "POSTP":
-                            label = "POSTP"
-                        if (
-                            d == n - 1
-                            and type(chunks[-1]) == Tree
-                            and chunks[-1].label() == label
-                        ):
-                            chunks[-1].append(item)
-                            appended = True
-                    if (
-                        node["head"] == n - 1
-                        and len(chunks) > 0
-                        and type(chunks[-1]) == Tree
-                        and chunks[-1].label() == label
-                    ):
-                        chunks[-1].append(item)
-                        appended = True
-                    if not appended:
-                        chunks.append(Tree(label, [item]))
-                elif node["ctag"] in {"PUNC", "CONJ", "SUBR", "PART"}:
-                    if (
-                        item[0]
-                        in {"'", '"', "(", ")", "{", "}", "[", "]", "-", "#", "«", "»"}
-                        and len(chunks) > 0
-                        and type(chunks[-1]) == Tree
-                    ):
-                        for leaf in chunks[-1].leaves():
-                            if leaf[1] == item[1]:
-                                chunks[-1].append(item)
-                                appended = True
-                                break
-                    if appended is not True:
-                        chunks.append(item)
-                elif node["ctag"] in {
-                    "N",
-                    "PREM",
-                    "ADJ",
-                    "PR",
-                    "ADR",
-                    "PRENUM",
-                    "IDEN",
-                    "POSNUM",
-                    "SADV",
-                }:
-                    if node["rel"] in {"MOZ", "NPOSTMOD"}:
-                        if len(chunks) > 0:
-                            if type(chunks[-1]) == Tree:
-                                j = n - len(chunks[-1].leaves())
-                                chunks[-1].append(item)
-                            else:
-                                j = n - 1
-                                treenode = Tree("NP", [chunks.pop(), item])
-                                chunks.append(treenode)
-                            while j > node["head"]:
-                                leaves = chunks.pop().leaves()
-                                if len(chunks) < 1:
-                                    chunks.append(Tree("NP", leaves))
-                                    j -= 1
-                                elif type(chunks[-1]) == Tree:
-                                    j -= len(chunks[-1])
-                                    for leaf in leaves:
-                                        chunks[-1].append(leaf)
-                                else:
-                                    leaves.insert(0, chunks.pop())
-                                    chunks.append(Tree("NP", leaves))
-                                    j -= 1
-                            continue
-                    elif node["rel"] == "POSDEP" and tree.nodes[node["head"]][
-                        "rel"
-                    ] in {"NCONJ", "AJCONJ"}:
-                        conj = tree.nodes[node["head"]]
-                        if tree.nodes[conj["head"]]["rel"] in {
-                            "MOZ",
-                            "NPOSTMOD",
-                            "AJCONJ",
-                            "POSDEP",
-                        }:
-                            label = "NP"
-                            leaves = [item]
-                            j = n - 1
-                            while j >= conj["head"]:
-                                if type(chunks[-1]) is Tree:
-                                    j -= len(chunks[-1].leaves())
-                                    label = chunks[-1].label()
-                                    leaves = chunks.pop().leaves() + leaves
-                                else:
-                                    leaves.insert(0, chunks.pop())
-                                    j -= 1
-                            chunks.append(Tree(label, leaves))
-                            appended = True
-                    elif (
-                        node["head"] == n - 1
-                        and len(chunks) > 0
-                        and type(chunks[-1]) == Tree
-                        and chunks[-1].label() != "PP"
-                    ):
-                        chunks[-1].append(item)
-                        appended = True
-                    elif node["rel"] == "AJCONJ" and tree.nodes[node["head"]][
-                        "rel"
-                    ] in {"NPOSTMOD", "AJCONJ"}:
-                        np_nodes = [item]
-                        label = "ADJP"
-                        i = n - node["head"]
-                        while i > 0:
-                            if type(chunks[-1]) == Tree:
-                                label = chunks[-1].label()
-                                leaves = chunks.pop().leaves()
-                                i -= len(leaves)
-                                np_nodes = leaves + np_nodes
-                            else:
-                                i -= 1
-                                np_nodes.insert(0, chunks.pop())
-                        chunks.append(Tree(label, np_nodes))
-                        appended = True
-                    elif (
-                        node["ctag"] == "ADJ"
-                        and node["rel"] == "POSDEP"
-                        and tree.nodes[node["head"]]["ctag"] != "CONJ"
-                    ):
-                        np_nodes = [item]
-                        i = n - node["head"]
-                        while i > 0:
-                            label = "ADJP"
-                            if type(chunks[-1]) == Tree:
-                                label = chunks[-1].label()
-                                leaves = chunks.pop().leaves()
-                                i -= len(leaves)
-                                np_nodes = leaves + np_nodes
-                            else:
-                                i -= 1
-                                np_nodes.insert(0, chunks.pop())
-                        chunks.append(Tree(label, np_nodes))
-                        appended = True
-                    for d in node_deps(node):
-                        if (
-                            d == n - 1
-                            and type(chunks[-1]) == Tree
-                            and chunks[-1].label() != "PP"
-                            and appended is not True
-                        ):
-                            label = chunks[-1].label()
-                            if node["rel"] == "ADV":
-                                label = "ADVP"
-                            elif label in {"ADJP", "ADVP"}:
-                                if node["ctag"] == "N":
-                                    label = "NP"
-                                elif node["ctag"] == "ADJ":
-                                    label = "ADJP"
-                            leaves = chunks.pop().leaves()
-                            leaves.append(item)
-                            chunks.append(Tree(label, leaves))
-                            appended = True
-                        elif tree.nodes[d]["rel"] == "NPREMOD" and appended is not True:
-                            np_nodes = [item]
-                            i = n - d
-                            while i > 0:
-                                if type(chunks[-1]) == Tree:
-                                    leaves = chunks.pop().leaves()
-                                    i -= len(leaves)
-                                    np_nodes = leaves + np_nodes
-                                else:
-                                    i -= 1
-                                    np_nodes.insert(0, chunks.pop())
-                            chunks.append(Tree("NP", np_nodes))
-                            appended = True
-                    if not appended:
-                        label = "NP"
-                        if node["ctag"] == "ADJ":
-                            label = "ADJP"
-                        elif node["rel"] == "ADV":
-                            label = "ADVP"
-                        chunks.append(Tree(label, [item]))
-                elif node["ctag"] in {"V"}:
-                    appended = False
-                    for d in node_deps(node):
-                        if (
-                            d == n - 1
-                            and type(chunks[-1]) == Tree
-                            and tree.nodes[d]["rel"] in {"NVE", "ENC"}
-                            and appended is not True
-                        ):
-                            leaves = chunks.pop().leaves()
-                            leaves.append(item)
-                            chunks.append(Tree("VP", leaves))
-                            appended = True
-                        elif tree.nodes[d]["rel"] in {"VPRT", "NVE"}:
-                            vp_nodes = [item]
-                            i = n - d
-                            while i > 0:
-                                if type(chunks[-1]) == Tree:
-                                    leaves = chunks.pop().leaves()
-                                    i -= len(leaves)
-                                    vp_nodes = leaves + vp_nodes
-                                else:
-                                    i -= 1
-                                    vp_nodes.insert(0, chunks.pop())
-                            chunks.append(Tree("VP", vp_nodes))
-                            appended = True
-                            break
-                    if not appended:
-                        chunks.append(Tree("VP", [item]))
-                elif node["ctag"] in {"PSUS"}:
-                    if node["rel"] == "ADV":
-                        chunks.append(Tree("ADVP", [item]))
-                    else:
-                        chunks.append(Tree("VP", [item]))
-                elif node["ctag"] in {"ADV", "SADV"}:
-                    appended = False
-                    for d in node_deps(node):
-                        if d == n - 1 and type(chunks[-1]) == Tree:
-                            leaves = chunks.pop().leaves()
-                            leaves.append(item)
-                            chunks.append(Tree("ADVP", leaves))
-                            appended = True
-                    if not appended:
-                        chunks.append(Tree("ADVP", [item]))
-
-            yield Tree("S", chunks)
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ PerDT است.
+
+PerDT حاوی تعداد قابل‌توجهی جملۀ برچسب‌خورده با اطلاعات نحوی و ساخت‌واژی است.
+
+"""
+from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import Iterator
+from typing import List
+from typing import Tuple
+from typing import Type
+
+from nltk.parse import DependencyGraph
+from nltk.tree import Tree
+
+
+def coarse_pos_u(tags: List[str], word: str) -> str:
+    """برچسب‌های ریز را به برچسب‌های درشت منطبق با استاندارد جهانی (coarse-grained
+    universal pos tags) تبدیل می‌کند.
+
+    Examples:
+        >>> coarse_pos_e(['N', 'IANM'], 'امروز')
+        'N'
+
+    """
+    mapping = {
+        "N": "NOUN",
+        "V": "VERB",
+        "ADJ": "ADJ",
+        "ADV": "ADV",
+        "PR": "PRON",
+        "PREM": "DET",
+        "PREP": "ADP",
+        "POSTP": "ADP",
+        "PRENUM": "NUM",
+        "CONJ": "CCONJ",
+        "PUNC": "PUNCT",
+        "SUBR": "SCONJ",
+        "IDEN": "PROPN",
+        "POSTNUM": "NUM",
+        "PSUS": "INTJ",
+        "PART": "PART",
+        "ADR": "INTJ",
+    }
+    pos_mapped = mapping.get(tags[0], "X")
+    if pos_mapped == "PART" and word == "را":
+        return "ADP"
+    if pos_mapped == "PART" and word in ["خوب", "آخر"]:
+        return "ADP"
+    return pos_mapped
+
+
+def coarse_pos_e(tags: List[str], word) -> str: # noqa: ARG001
+    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
+
+    Examples:
+        >>> coarse_pos_e(['N', 'IANM'],'امروز')
+        'N'
+
+    """
+    mapping = {
+        "N": "N",
+        "V": "V",
+        "ADJ": "AJ",
+        "ADV": "ADV",
+        "PR": "PRO",
+        "PREM": "DET",
+        "PREP": "P",
+        "POSTP": "POSTP",
+        "PRENUM": "NUM",
+        "CONJ": "CONJ",
+        "PUNC": "PUNC",
+        "SUBR": "CONJ",
+    }
+    return mapping.get(tags[0], "X") + ("e" if "EZ" in tags else "")
+
+
+def word_nodes(tree: Type[Tree]) -> List[Dict[str, Any]]:
+    """نودها را به صورت مرتب‌شده برمی‌گرداند."""
+    return sorted(tree.nodes.values(), key=lambda node: node["address"])[1:]
+
+
+def node_deps(node: List[Dict[str, Any]]) -> List[Any]:
+    """مقادیر موجود در فیلد deps نود ورودی را برمی‌گرداند."""
+    return sum(list(node["deps"].values()), [])
+
+
+class DadeganReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ PerDT است.
+
+    Args:
+        conll_file: مسیر فایلِ پیکره.
+        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
+
+    """
+
+    def __init__(
+        self: "DadeganReader",
+        conll_file: str,
+        pos_map: str = coarse_pos_e,
+        universal_pos: bool = False,
+    ) -> None:
+        self._conll_file = conll_file
+        if pos_map is None:
+            self._pos_map = lambda tags: ",".join(tags)
+        elif universal_pos:
+            self._pos_map = coarse_pos_u
+        else:
+            self._pos_map = coarse_pos_e
+
+    def _sentences(self: "DadeganReader") -> Iterator[str]:
+        """جملات پیکره را به شکل متن خام برمی‌گرداند.
+
+        Yields:
+            جملهٔ بعدی.
+
+        """
+        with Path(self._conll_file).open(encoding="utf8") as conll_file:
+            text = conll_file.read()
+
+            # refine text
+            text = (
+                text.replace("‌‌", "‌")
+                .replace("\t‌", "\t")
+                .replace("‌\t", "\t")
+                .replace("\t ", "\t")
+                .replace(" \t", "\t")
+                .replace("\r", "")
+                .replace("\u2029", "‌")
+            )
+
+            for item in text.replace(" ", "_").split("\n\n"):
+                if item.strip():
+                    yield item
+
+    def trees(self: "DadeganReader") -> Iterator[Type[Tree]]:
+        """ساختار درختی جملات را برمی‌گرداند.
+
+        Yields:
+            ساختار درختی جملهٔ بعدی.
+
+        """
+        for sentence in self._sentences():
+            tree = DependencyGraph(sentence)
+
+            for node in word_nodes(tree):
+                node["mtag"] = [node["ctag"], node["tag"]]
+
+                if "ezafe" in node["feats"]:
+                    node["mtag"].append("EZ")
+
+                node["mtag"] = self._pos_map(node["mtag"], node["word"])
+
+            yield tree
+
+    def sents(self: "DadeganReader") -> Iterator[List[Tuple[str, str]]]:
+        """لیستی از جملات را برمی‌گرداند.
+
+        هر جمله لیستی از `(توکن، برچسب)`ها است.
+
+        Examples:
+            >>> dadegan = DadeganReader(conll_file='dadegan.conll')
+            >>> next(dadegan.sents())
+            [('این', 'DET'), ('میهمانی', 'N'), ('به', 'P'), ('منظور', 'Ne'), ('آشنایی', 'Ne'), ('هم‌تیمی‌های', 'Ne'), ('او', 'PRO'), ('با', 'P'), ('غذاهای', 'Ne'), ('ایرانی', 'AJ'), ('ترتیب', 'N'), ('داده_شد', 'V'), ('.', 'PUNC')]
+
+        Yields:
+            جملهٔ بعدی.
+
+        """
+        for tree in self.trees():
+            yield [(node["word"], node["mtag"]) for node in word_nodes(tree)]
+
+    def chunked_trees(self: "DadeganReader") -> Iterator[Type[Tree]]:
+        """درخت وابستگی‌های جملات را برمی‌گرداند.
+
+        Examples:
+            >>> from hazm.chunker import tree2brackets
+            >>> dadegan = DadeganReader(conll_file='dadegan.conll')
+            >>> tree2brackets(next(dadegan.chunked_trees()))
+            '[این میهمانی NP] [به PP] [منظور آشنایی هم‌تیمی‌های او NP] [با PP] [غذاهای ایرانی NP] [ترتیب داده_شد VP] .'
+
+        Yields:
+            درخت وابستگی‌های جملهٔ بعدی.
+
+        """
+        for tree in self.trees():
+            chunks = []
+            for node in word_nodes(tree):
+                n = node["address"]
+                item = (node["word"], node["mtag"])
+                appended = False
+                if node["ctag"] in {"PREP", "POSTP"}:
+                    for d in node_deps(node):
+                        label = "PP"
+                        if node["ctag"] == "POSTP":
+                            label = "POSTP"
+                        if (
+                            d == n - 1
+                            and type(chunks[-1]) == Tree
+                            and chunks[-1].label() == label
+                        ):
+                            chunks[-1].append(item)
+                            appended = True
+                    if (
+                        node["head"] == n - 1
+                        and len(chunks) > 0
+                        and type(chunks[-1]) == Tree
+                        and chunks[-1].label() == label
+                    ):
+                        chunks[-1].append(item)
+                        appended = True
+                    if not appended:
+                        chunks.append(Tree(label, [item]))
+                elif node["ctag"] in {"PUNC", "CONJ", "SUBR", "PART"}:
+                    if (
+                        item[0]
+                        in {"'", '"', "(", ")", "{", "}", "[", "]", "-", "#", "«", "»"}
+                        and len(chunks) > 0
+                        and type(chunks[-1]) == Tree
+                    ):
+                        for leaf in chunks[-1].leaves():
+                            if leaf[1] == item[1]:
+                                chunks[-1].append(item)
+                                appended = True
+                                break
+                    if appended is not True:
+                        chunks.append(item)
+                elif node["ctag"] in {
+                    "N",
+                    "PREM",
+                    "ADJ",
+                    "PR",
+                    "ADR",
+                    "PRENUM",
+                    "IDEN",
+                    "POSNUM",
+                    "SADV",
+                }:
+                    if node["rel"] in {"MOZ", "NPOSTMOD"}:
+                        if len(chunks) > 0:
+                            if type(chunks[-1]) == Tree:
+                                j = n - len(chunks[-1].leaves())
+                                chunks[-1].append(item)
+                            else:
+                                j = n - 1
+                                treenode = Tree("NP", [chunks.pop(), item])
+                                chunks.append(treenode)
+                            while j > node["head"]:
+                                leaves = chunks.pop().leaves()
+                                if len(chunks) < 1:
+                                    chunks.append(Tree("NP", leaves))
+                                    j -= 1
+                                elif type(chunks[-1]) == Tree:
+                                    j -= len(chunks[-1])
+                                    for leaf in leaves:
+                                        chunks[-1].append(leaf)
+                                else:
+                                    leaves.insert(0, chunks.pop())
+                                    chunks.append(Tree("NP", leaves))
+                                    j -= 1
+                            continue
+                    elif node["rel"] == "POSDEP" and tree.nodes[node["head"]][
+                        "rel"
+                    ] in {"NCONJ", "AJCONJ"}:
+                        conj = tree.nodes[node["head"]]
+                        if tree.nodes[conj["head"]]["rel"] in {
+                            "MOZ",
+                            "NPOSTMOD",
+                            "AJCONJ",
+                            "POSDEP",
+                        }:
+                            label = "NP"
+                            leaves = [item]
+                            j = n - 1
+                            while j >= conj["head"]:
+                                if type(chunks[-1]) is Tree:
+                                    j -= len(chunks[-1].leaves())
+                                    label = chunks[-1].label()
+                                    leaves = chunks.pop().leaves() + leaves
+                                else:
+                                    leaves.insert(0, chunks.pop())
+                                    j -= 1
+                            chunks.append(Tree(label, leaves))
+                            appended = True
+                    elif (
+                        node["head"] == n - 1
+                        and len(chunks) > 0
+                        and type(chunks[-1]) == Tree
+                        and chunks[-1].label() != "PP"
+                    ):
+                        chunks[-1].append(item)
+                        appended = True
+                    elif node["rel"] == "AJCONJ" and tree.nodes[node["head"]][
+                        "rel"
+                    ] in {"NPOSTMOD", "AJCONJ"}:
+                        np_nodes = [item]
+                        label = "ADJP"
+                        i = n - node["head"]
+                        while i > 0:
+                            if type(chunks[-1]) == Tree:
+                                label = chunks[-1].label()
+                                leaves = chunks.pop().leaves()
+                                i -= len(leaves)
+                                np_nodes = leaves + np_nodes
+                            else:
+                                i -= 1
+                                np_nodes.insert(0, chunks.pop())
+                        chunks.append(Tree(label, np_nodes))
+                        appended = True
+                    elif (
+                        node["ctag"] == "ADJ"
+                        and node["rel"] == "POSDEP"
+                        and tree.nodes[node["head"]]["ctag"] != "CONJ"
+                    ):
+                        np_nodes = [item]
+                        i = n - node["head"]
+                        while i > 0:
+                            label = "ADJP"
+                            if type(chunks[-1]) == Tree:
+                                label = chunks[-1].label()
+                                leaves = chunks.pop().leaves()
+                                i -= len(leaves)
+                                np_nodes = leaves + np_nodes
+                            else:
+                                i -= 1
+                                np_nodes.insert(0, chunks.pop())
+                        chunks.append(Tree(label, np_nodes))
+                        appended = True
+                    for d in node_deps(node):
+                        if (
+                            d == n - 1
+                            and type(chunks[-1]) == Tree
+                            and chunks[-1].label() != "PP"
+                            and appended is not True
+                        ):
+                            label = chunks[-1].label()
+                            if node["rel"] == "ADV":
+                                label = "ADVP"
+                            elif label in {"ADJP", "ADVP"}:
+                                if node["ctag"] == "N":
+                                    label = "NP"
+                                elif node["ctag"] == "ADJ":
+                                    label = "ADJP"
+                            leaves = chunks.pop().leaves()
+                            leaves.append(item)
+                            chunks.append(Tree(label, leaves))
+                            appended = True
+                        elif tree.nodes[d]["rel"] == "NPREMOD" and appended is not True:
+                            np_nodes = [item]
+                            i = n - d
+                            while i > 0:
+                                if type(chunks[-1]) == Tree:
+                                    leaves = chunks.pop().leaves()
+                                    i -= len(leaves)
+                                    np_nodes = leaves + np_nodes
+                                else:
+                                    i -= 1
+                                    np_nodes.insert(0, chunks.pop())
+                            chunks.append(Tree("NP", np_nodes))
+                            appended = True
+                    if not appended:
+                        label = "NP"
+                        if node["ctag"] == "ADJ":
+                            label = "ADJP"
+                        elif node["rel"] == "ADV":
+                            label = "ADVP"
+                        chunks.append(Tree(label, [item]))
+                elif node["ctag"] in {"V"}:
+                    appended = False
+                    for d in node_deps(node):
+                        if (
+                            d == n - 1
+                            and type(chunks[-1]) == Tree
+                            and tree.nodes[d]["rel"] in {"NVE", "ENC"}
+                            and appended is not True
+                        ):
+                            leaves = chunks.pop().leaves()
+                            leaves.append(item)
+                            chunks.append(Tree("VP", leaves))
+                            appended = True
+                        elif tree.nodes[d]["rel"] in {"VPRT", "NVE"}:
+                            vp_nodes = [item]
+                            i = n - d
+                            while i > 0:
+                                if type(chunks[-1]) == Tree:
+                                    leaves = chunks.pop().leaves()
+                                    i -= len(leaves)
+                                    vp_nodes = leaves + vp_nodes
+                                else:
+                                    i -= 1
+                                    vp_nodes.insert(0, chunks.pop())
+                            chunks.append(Tree("VP", vp_nodes))
+                            appended = True
+                            break
+                    if not appended:
+                        chunks.append(Tree("VP", [item]))
+                elif node["ctag"] in {"PSUS"}:
+                    if node["rel"] == "ADV":
+                        chunks.append(Tree("ADVP", [item]))
+                    else:
+                        chunks.append(Tree("VP", [item]))
+                elif node["ctag"] in {"ADV", "SADV"}:
+                    appended = False
+                    for d in node_deps(node):
+                        if d == n - 1 and type(chunks[-1]) == Tree:
+                            leaves = chunks.pop().leaves()
+                            leaves.append(item)
+                            chunks.append(Tree("ADVP", leaves))
+                            appended = True
+                    if not appended:
+                        chunks.append(Tree("ADVP", [item]))
+
+            yield Tree("S", chunks)
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/degarbayan_reader.py` & `hazm-0.9.2/hazm/corpus_readers/degarbayan_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,144 +1,143 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ دِگَربیان است.
-
-[پیکرهٔ
-دگربیان](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-
-%D8%AF%DA%AF%D8%B1%D8%A8%DB%8C%D8%A7%D9%86) حاوی
-۱۵۲۳ نمونه است که به عنوان نمونه‌های دگربیان نشانه‌گذاری شده‌اند. جملات و
-عبارات
-دگربیان، بیانی متفاوت از مفهومی یکسان هستند. داده‌های این پیکره از خبرگزاری‌ها
-جمع‌آورده شده و در سه دسته‌بندی «دگربیان»، «تقریباً دگربیان» و «نامرتبط» ارائه
-می‌شوند. این داده‌ها با استفاده از همکاری جمعی در پیام‌رسان تلگرام نشانه‌گذاری
-شده است.
-
-"""
-
-
-import os
-import sys
-from pathlib import Path
-from typing import Any
-from typing import Dict
-from typing import Iterator
-from typing import Tuple
-from xml.dom import minidom
-
-
-class DegarbayanReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ دگربیان است.
-
-    Args:
-        root: مسیر فولدر حاوی فایل‌های پیکره
-        corpus_file: فایل اطلاعات پیکره.
-            در صورتی که بخواهید از حالت استاندارد پیکره استفاده کنید نیازی به تغییرِ این فایل نیست.
-        judge_type: این پارامتر دارای دو مقدار `three_class` و `two_class` است.
-            در حالت `three_class` جملات سه برچسب می‌خورند: ۱. `Paraphrase`(دگربیان)
-            ۲. `SemiParaphrase`(تقریباً دگربیان) ۳. `NotParaphrase`(غیر دگربیان). در حالت
-            `two_class` حالت دوم یعنی `SemiParaphrase` هم برچسب `Paraphrase` می‌خورَد.
-        version: شمارهٔ نسخهٔ پیکره
-
-    """
-
-    def __init__(
-        self: "DegarbayanReader",
-        root: str,
-        corpus_file: str = "corpus_pair.xml",
-        judge_type: str = "three_class",
-    ) -> None:
-        self._root = root
-        self._corpus_file = corpus_file
-        self._judge_type = judge_type
-        if judge_type != "three_class" and judge_type != "two_class":
-            self._judge_type = "three_class"
-
-    def docs(self: "DegarbayanReader") -> Iterator[Dict[str, Any]]:
-        """اسناد موجود در پیکره را برمی‌گرداند.
-
-        Yields:
-            سند بعدی.
-
-        """
-
-        def judge_number_to_text(judge: str) -> str:
-            if judge == "1" or (self._judge_type == "two_class" and judge == "0"):
-                return "Paraphrase"
-
-            if judge == "0":
-                return "SemiParaphrase"
-
-            return "NotParaphrase"
-
-        filename = os.path.join(self._root, self._corpus_file)
-        if os.path.exists(filename):
-            try:
-                elements = minidom.parse(filename)
-                for element in elements.getElementsByTagName("Pair"):
-                    pair = {
-                        "id": (
-                            element.getElementsByTagName("PairId")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "news_source1": (
-                            element.getElementsByTagName("NewsSource1")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "news_source2": (
-                            element.getElementsByTagName("NewsSource2")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "news_id1": (
-                            element.getElementsByTagName("NewsId1")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "news_id2": (
-                            element.getElementsByTagName("NewsId2")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "sentence1": (
-                            element.getElementsByTagName("Sentence1")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "sentence2": (
-                            element.getElementsByTagName("Sentence2")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "method_type": (
-                            element.getElementsByTagName("MethodType")[0]
-                            .childNodes[0]
-                            .data.strip()
-                        ),
-                        "judge": judge_number_to_text(
-                            element.getElementsByTagName("judge")[0]
-                            .childNodes[0]
-                            .data.strip(),
-                        ),
-                    }
-                    yield pair
-
-            except Exception as e:
-                print("error in reading", filename, e, file=sys.stderr)
-        else:
-            print("error in reading file", filename, e, file=sys.stderr)  # noqa: F821
-            msg = "error in reading file"
-            raise FileNotFoundError(msg, filename)
-
-    def pairs(self: "DegarbayanReader") -> Iterator[Tuple[str, str, str]]:
-        """متن‌های دگربیان را در قالب یک `(متن اصلی، شکل دگربیان، برچسب)` برمی‌گرداند.
-
-        Examples:
-            >>> degarbayan = DegarbayanReader(root='corpora/degarbayan')
-            >>> next(degarbayan.pairs())
-            ('24 نفر نهایی تیم ملی بدون تغییری خاص معرفی شد', 'کی روش 24 بازیکن را به تیم ملی فوتبال دعوت کرد', 'Paraphrase')
-
-        Yields:
-            `متن دگربیان بعدی در قالب یک `(متن اصلی، شکل دگربیان، برچسب).
-
-        """
-        for pair in self.docs():
-            yield pair["sentence1"], pair["sentence2"], pair["judge"]
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ دِگَربیان است.
+
+[پیکرهٔ
+دگربیان](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-
+%D8%AF%DA%AF%D8%B1%D8%A8%DB%8C%D8%A7%D9%86) حاوی
+۱۵۲۳ نمونه است که به عنوان نمونه‌های دگربیان نشانه‌گذاری شده‌اند. جملات و
+عبارات
+دگربیان، بیانی متفاوت از مفهومی یکسان هستند. داده‌های این پیکره از خبرگزاری‌ها
+جمع‌آورده شده و در سه دسته‌بندی «دگربیان»، «تقریباً دگربیان» و «نامرتبط» ارائه
+می‌شوند. این داده‌ها با استفاده از همکاری جمعی در پیام‌رسان تلگرام نشانه‌گذاری
+شده است.
+
+"""
+
+
+import os
+import sys
+from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import Iterator
+from typing import Tuple
+from xml.dom import minidom
+
+
+class DegarbayanReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ دگربیان است.
+
+    Args:
+        root: مسیر فولدر حاوی فایل‌های پیکره
+        corpus_file: فایل اطلاعات پیکره.
+            در صورتی که بخواهید از حالت استاندارد پیکره استفاده کنید نیازی به تغییرِ این فایل نیست.
+        judge_type: این پارامتر دارای دو مقدار `three_class` و `two_class` است.
+            در حالت `three_class` جملات سه برچسب می‌خورند: ۱. `Paraphrase`(دگربیان)
+            ۲. `SemiParaphrase`(تقریباً دگربیان) ۳. `NotParaphrase`(غیر دگربیان). در حالت
+            `two_class` حالت دوم یعنی `SemiParaphrase` هم برچسب `Paraphrase` می‌خورَد.
+
+    """
+
+    def __init__(
+        self: "DegarbayanReader",
+        root: str,
+        corpus_file: str = "corpus_pair.xml",
+        judge_type: str = "three_class",
+    ) -> None:
+        self._root = root
+        self._corpus_file = corpus_file
+        self._judge_type = judge_type
+        if judge_type != "three_class" and judge_type != "two_class":
+            self._judge_type = "three_class"
+
+    def docs(self: "DegarbayanReader") -> Iterator[Dict[str, Any]]:
+        """اسناد موجود در پیکره را برمی‌گرداند.
+
+        Yields:
+            سند بعدی.
+
+        """
+
+        def judge_number_to_text(judge: str) -> str:
+            if judge == "1" or (self._judge_type == "two_class" and judge == "0"):
+                return "Paraphrase"
+
+            if judge == "0":
+                return "SemiParaphrase"
+
+            return "NotParaphrase"
+
+        filename = os.path.join(self._root, self._corpus_file) # noqa: PTH118
+        if os.path.exists(filename): # noqa: PTH110
+            try:
+                elements = minidom.parse(filename)
+                for element in elements.getElementsByTagName("Pair"):
+                    pair = {
+                        "id": (
+                            element.getElementsByTagName("PairId")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "news_source1": (
+                            element.getElementsByTagName("NewsSource1")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "news_source2": (
+                            element.getElementsByTagName("NewsSource2")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "news_id1": (
+                            element.getElementsByTagName("NewsId1")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "news_id2": (
+                            element.getElementsByTagName("NewsId2")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "sentence1": (
+                            element.getElementsByTagName("Sentence1")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "sentence2": (
+                            element.getElementsByTagName("Sentence2")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "method_type": (
+                            element.getElementsByTagName("MethodType")[0]
+                            .childNodes[0]
+                            .data.strip()
+                        ),
+                        "judge": judge_number_to_text(
+                            element.getElementsByTagName("judge")[0]
+                            .childNodes[0]
+                            .data.strip(),
+                        ),
+                    }
+                    yield pair
+
+            except Exception as e:
+                print("error in reading", filename, e, file=sys.stderr)
+        else:
+            print("error in reading file", filename, e, file=sys.stderr)  # noqa: F821
+            msg = "error in reading file"
+            raise FileNotFoundError(msg, filename)
+
+    def pairs(self: "DegarbayanReader") -> Iterator[Tuple[str, str, str]]:
+        """متن‌های دگربیان را در قالب یک `(متن اصلی، شکل دگربیان، برچسب)` برمی‌گرداند.
+
+        Examples:
+            >>> degarbayan = DegarbayanReader(root='degarbayan')
+            >>> next(degarbayan.pairs())
+            ('24 نفر نهایی تیم ملی بدون تغییری خاص معرفی شد', 'کی روش 24 بازیکن را به تیم ملی فوتبال دعوت کرد', 'Paraphrase')
+
+        Yields:
+            `متن دگربیان بعدی در قالب یک `(متن اصلی، شکل دگربیان، برچسب).
+
+        """
+        for pair in self.docs():
+            yield pair["sentence1"], pair["sentence2"], pair["judge"]
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/mirastext_reader.py` & `hazm-0.9.2/hazm/corpus_readers/mirastext_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ میراث است.
-
-[پیکرهٔ میراث](https://github.com/miras-tech/MirasText) حاوی ۲,۸۳۵,۴۱۴ خبر از
-۲۵۰ خبرگزاری فارسی است.
-
-"""
-from pathlib import Path
-from typing import Dict
-from typing import Iterator
-
-
-class MirasTextReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ میراث است.
-
-    Args:
-        filename: مسیر فایلِ پیکره.
-
-    """
-
-    def __init__(self: "MirasTextReader", filename: str) -> None:
-        self._filename = filename
-
-    def docs(self: "MirasTextReader") -> Iterator[Dict[str, str]]:
-        """خبرها را برمی‌گرداند.
-
-        Yields:
-            خبر بعدی.
-
-        """
-        for line in Path(self._filename).open(encoding="utf-8"):
-            parts = line.split("***")
-            # todo: extract link, tags, ...
-            yield {"text": parts[0].strip()}
-
-    def texts(self: "MirasTextReader") -> Iterator[str]:
-        """فقط متن خبرها را برمی‌گرداند.
-
-        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با تابع
-        ‍[docs()][hazm.corpus_readers.mirastext_reader.MirasTextReader.docs] و دریافت مقدار
-        پراپرتی `text` نیز می‌توانید همین کار را انجام دهید.
-
-        Examples:
-            >>> mirastext = MirasTextReader(filename='corpora/mirastext.txt')
-            >>> next(mirastext.texts())[:42]  # first 42 characters of fitst text
-            'ایرانی‌ها چقدر از اینترنت استفاده می‌کنند؟'
-
-        Yields:
-            : متنِ خبر بعدی.
-
-        """
-        for doc in self.docs():
-            yield doc["text"]
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ میراث است.
+
+[پیکرهٔ میراث](https://github.com/miras-tech/MirasText) حاوی ۲,۸۳۵,۴۱۴ خبر از
+۲۵۰ خبرگزاری فارسی است.
+
+"""
+from pathlib import Path
+from typing import Dict
+from typing import Iterator
+
+
+class MirasTextReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ میراث است.
+
+    Args:
+        filename: مسیر فایلِ پیکره.
+
+    """
+
+    def __init__(self: "MirasTextReader", filename: str) -> None:
+        self._filename = filename
+
+    def docs(self: "MirasTextReader") -> Iterator[Dict[str, str]]:
+        """خبرها را برمی‌گرداند.
+
+        Yields:
+            خبر بعدی.
+
+        """
+        for line in Path(self._filename).open(encoding="utf-8"):
+            parts = line.split("***")
+            # todo: extract link, tags, ...
+            yield {"text": parts[0].strip()}
+
+    def texts(self: "MirasTextReader") -> Iterator[str]:
+        """فقط متن خبرها را برمی‌گرداند.
+
+        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با تابع
+        ‍[docs()][hazm.corpus_readers.mirastext_reader.MirasTextReader.docs] و دریافت مقدار
+        پراپرتی `text` نیز می‌توانید همین کار را انجام دهید.
+
+        Examples:
+            >>> mirastext = MirasTextReader(filename='mirastext.txt')
+            >>> next(mirastext.texts())[:42]  # first 42 characters of fitst text
+            'ایرانی‌ها چقدر از اینترنت استفاده می‌کنند؟'
+
+        Yields:
+            : متنِ خبر بعدی.
+
+        """
+        for doc in self.docs():
+            yield doc["text"]
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/persian_plain_text_reader.py` & `hazm-0.9.2/hazm/corpus_readers/persian_plain_text_reader.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""این ماژول، پیکره‌های متنی خام را می‌خواند."""
-from typing import Any
-from typing import Callable
-from typing import List
-
-from nltk.corpus import PlaintextCorpusReader
-from nltk.corpus.reader import StreamBackedCorpusView
-from nltk.corpus.reader import read_blankline_block
-
-from hazm import SentenceTokenizer
-from hazm import WordTokenizer
-
-
-class PersianPlainTextReader(PlaintextCorpusReader):
-    """Reader for corpora that consist of plaintext documents.  Paragraphs
-    are assumed to be split using blank lines.  Sentences and words can
-    be tokenized using the default tokenizers, or by custom tokenizers
-    specificed as parameters to the constructor.
-
-    """
-
-    CorpusView = StreamBackedCorpusView
-
-    def __init__(
-        self: "PersianPlainTextReader",
-        root: str,
-        fileids: List,
-        word_tokenizer: Callable = WordTokenizer.tokenize,
-        sent_tokenizer: Callable = SentenceTokenizer.tokenize,
-        para_block_reader: Callable = read_blankline_block,
-        encoding: str = "utf8",
-    ) -> None:
-        super().__init__(
-            root,
-            fileids,
-            word_tokenizer,
-            sent_tokenizer,
-            para_block_reader,
-            encoding,
-        )
+"""این ماژول، پیکره‌های متنی خام را می‌خواند."""
+from typing import Any
+from typing import Callable
+from typing import List
+
+from nltk.corpus import PlaintextCorpusReader
+from nltk.corpus.reader import StreamBackedCorpusView
+from nltk.corpus.reader import read_blankline_block
+
+from hazm import SentenceTokenizer
+from hazm import WordTokenizer
+
+
+class PersianPlainTextReader(PlaintextCorpusReader):
+    """Reader for corpora that consist of plaintext documents.  Paragraphs
+    are assumed to be split using blank lines.  Sentences and words can
+    be tokenized using the default tokenizers, or by custom tokenizers
+    specificed as parameters to the constructor.
+
+    """
+
+    CorpusView = StreamBackedCorpusView
+
+    def __init__(
+        self: "PersianPlainTextReader",
+        root: str,
+        fileids: List,
+        word_tokenizer: Callable = WordTokenizer.tokenize,
+        sent_tokenizer: Callable = SentenceTokenizer.tokenize,
+        para_block_reader: Callable = read_blankline_block,
+        encoding: str = "utf8",
+    ) -> None:
+        super().__init__(
+            root,
+            fileids,
+            word_tokenizer,
+            sent_tokenizer,
+            para_block_reader,
+            encoding,
+        )
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/persica_reader.py` & `hazm-0.9.2/hazm/corpus_readers/persica_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ پرسیکا است.
-
-[پیکرهٔ پرسیکا](https://www.peykaregan.ir/dataset/%D9%BE%D8%B1%D8%B3%DB%8C%DA%A
-9%D8%A7-%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-%D9%85%D8%AA%D9%88%D9%86-
-%D8%AE%D8%A8%D8%B1%DB%8C) حاوی
-خبرهای برگرفته از خبرگزاری ایسنا در یازده دستهٔ ورزشی، اقتصادی، فرهنگی، مذهبی،
-تاریخی، سیاسی، علمی، اجتماعی، آموزشی، حقوق قضایی و بهداشت است. روی این داده‌ها
-پیش‌پردازش‌هایی صورت شده و آمادهٔ استفاده در کاربردهای مختلف پردازش زبان طبیعی
-و
-داده‌کاوی است.
-
-"""
-from pathlib import Path
-from typing import Dict
-from typing import Iterator
-
-
-class PersicaReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ پرسیکا است.
-
-    Args:
-        csv_file: مسیر فایلِ پیکره با پسوند csv.
-
-    """
-
-    def __init__(self: "PersicaReader", csv_file: str) -> None:
-        self._csv_file = csv_file
-
-    def docs(self: "PersicaReader") -> Iterator[Dict[str, str]]:
-        """خبرها را برمی‌گرداند.
-
-        هر خبر، شی‌ای متشکل از این پارامتر است:
-
-        - شناسه (`id`)
-        - عنوان (`title`)
-        - متن (`text`)
-        - تاریخ (`date`)
-        - زمان (`time`)
-        - دستهٔ اصلی (`category`)
-        - دستهٔ فرعی (`category2`)
-
-        Examples:
-            >>> persica = PersicaReader('corpora/persica.csv')
-            >>> next(persica.docs())['id']
-            843656
-
-        Yields:
-            خبر بعدی.
-
-        """
-        lines = []
-        for current_line in Path(self._csv_file).open(encoding="utf-8-sig"):
-            current_line = current_line.strip()
-            if current_line:
-                if current_line.endswith(","):
-                    lines.append(current_line[:-1])
-                else:
-                    lines.append(current_line)
-                    yield {
-                        "id": int(lines[0]),
-                        "title": lines[1],
-                        "text": lines[2],
-                        "date": lines[3],
-                        "time": lines[4],
-                        "category": lines[5],
-                        "category2": lines[6],
-                    }
-                    lines = []
-
-    def texts(self: "PersicaReader") -> Iterator[str]:
-        """فقط متن خبرها را برمی‌گرداند.
-
-        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با همان تابع
-        ‍[docs()][hazm.corpus_readers.persica_reader.PersicaReader.docs] و دریافت مقدار پراپرتی
-        `text` نیز می‌توانید همین کار را انجام دهید.
-
-        Examples:
-            >>> persica = PersicaReader('corpora/persica.csv')
-            >>> next(persica.texts()).startswith('وزير علوم در جمع استادان نمونه كشور گفت')
-            True
-
-        Yields:
-            متنِ خبر بعدی.
-
-        """
-        for doc in self.docs():
-            yield doc["text"]
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ پرسیکا است.
+
+[پیکرهٔ پرسیکا](https://www.peykaregan.ir/dataset/%D9%BE%D8%B1%D8%B3%DB%8C%DA%A
+9%D8%A7-%D9%BE%DB%8C%DA%A9%D8%B1%D9%87-%D9%85%D8%AA%D9%88%D9%86-
+%D8%AE%D8%A8%D8%B1%DB%8C) حاوی
+خبرهای برگرفته از خبرگزاری ایسنا در یازده دستهٔ ورزشی، اقتصادی، فرهنگی، مذهبی،
+تاریخی، سیاسی، علمی، اجتماعی، آموزشی، حقوق قضایی و بهداشت است. روی این داده‌ها
+پیش‌پردازش‌هایی صورت شده و آمادهٔ استفاده در کاربردهای مختلف پردازش زبان طبیعی
+و
+داده‌کاوی است.
+
+"""
+from pathlib import Path
+from typing import Dict
+from typing import Iterator
+
+
+class PersicaReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ پرسیکا است.
+
+    Args:
+        csv_file: مسیر فایلِ پیکره با پسوند csv.
+
+    """
+
+    def __init__(self: "PersicaReader", csv_file: str) -> None:
+        self._csv_file = csv_file
+
+    def docs(self: "PersicaReader") -> Iterator[Dict[str, str]]:
+        """خبرها را برمی‌گرداند.
+
+        هر خبر، شی‌ای متشکل از این پارامتر است:
+
+        - شناسه (`id`)
+        - عنوان (`title`)
+        - متن (`text`)
+        - تاریخ (`date`)
+        - زمان (`time`)
+        - دستهٔ اصلی (`category`)
+        - دستهٔ فرعی (`category2`)
+
+        Examples:
+            >>> persica = PersicaReader('persica.csv')
+            >>> next(persica.docs())['id']
+            843656
+
+        Yields:
+            خبر بعدی.
+
+        """
+        lines = []
+        for current_line in Path(self._csv_file).open(encoding="utf-8-sig"):
+            current_line = current_line.strip()
+            if current_line:
+                if current_line.endswith(","):
+                    lines.append(current_line[:-1])
+                else:
+                    lines.append(current_line)
+                    yield {
+                        "id": int(lines[0]),
+                        "title": lines[1],
+                        "text": lines[2],
+                        "date": lines[3],
+                        "time": lines[4],
+                        "category": lines[5],
+                        "category2": lines[6],
+                    }
+                    lines = []
+
+    def texts(self: "PersicaReader") -> Iterator[str]:
+        """فقط متن خبرها را برمی‌گرداند.
+
+        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با همان تابع
+        ‍[docs()][hazm.corpus_readers.persica_reader.PersicaReader.docs] و دریافت مقدار پراپرتی
+        `text` نیز می‌توانید همین کار را انجام دهید.
+
+        Examples:
+            >>> persica = PersicaReader('persica.csv')
+            >>> next(persica.texts()).startswith('وزير علوم در جمع استادان نمونه كشور گفت')
+            True
+
+        Yields:
+            متنِ خبر بعدی.
+
+        """
+        for doc in self.docs():
+            yield doc["text"]
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/peykare_reader.py` & `hazm-0.9.2/hazm/corpus_readers/peykare_reader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ Peykare است.
-
-[peykare پیکرهٔ](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%
-87-%D9%85%D8%AA%D9%86%DB%8C-%D8%B2%D8%A8%D8%A7%D9%86-
-%D9%81%D8%A7%D8%B1%D8%B3%DB%8C)
-جموعه‌ای از متون نوشتاری و گفتاری رسمی زبان فارسی است که از منابع واقعی همچون
-روزنامه‌ها، سایت‌ها و مستنداتِ از قبل تایپ‌شده، جمع‌آوری شده، تصحیح گردیده و
-برچسب خورده است. حجم این دادگان حدوداً ۱۰۰ میلیون کلمه است و از منابع مختلف
-تهیه
-گردیده و دارای تنوع بسیار زیادی است. ۱۰ میلیون کلمه از این پیکره با استفاده از
-۸۸۲ برچسب نحوی-معنایی به صورت دستی توسط دانشجویان رشتهٔ زبان‌شناسی برچسب‌دهی
-شده‌اند و هر پرونده بر حسب موضوع و منبع آن طبقه‌بندی شده است. این پیکره که توسط
-پژوهشکده پردازش هوشمند علائم تهیه شده است، برای استفاده در آموزش مدل زبانی و
-سایر پروژه‌های مربوط به پردازش زبان طبیعی مناسب است.
-
-"""
-
-
-import codecs
-import os
-from pathlib import Path
-from typing import Any
-from typing import Iterator
-from typing import List
-from typing import Tuple
-
-from hazm.normalizer import Normalizer
-from hazm.word_tokenizer import WordTokenizer
-
-
-def coarse_pos_u(tags: List[str], word: str) -> List[str]:
-    """برچسب‌های ریز را به برچسب‌های درشت منطبق با استاندارد جهانی (coarse-grained
-    universal pos tags) تبدیل می‌کند.
-
-    Examples:
-        >>> coarse_pos_u(['N','COM','SING'], 'الجزیره')
-        'NOUN'
-
-    Args:
-        tags: لیست برچسب‌های ریز.
-        word: برچسبی که می‌خواهید به برچسب جهانی تبدیل شود.
-
-    Returns:
-        لیست برچسب‌های درشت جهانی.
-
-    """
-    map_pos_to_upos = {
-        "N": "NOUN",
-        "V": "VERB",
-        "AJ": "ADJ",
-        "ADV": "ADV",
-        "PRO": "PRON",
-        "DET": "DET",
-        "P": "ADP",
-        "POSTP": "ADP",
-        "NUM": "NUM",
-        "CONJ": "CCONJ",
-        "PUNC": "PUNCT",
-        "CL": "NOUN",
-        "INT": "INTJ",
-        "RES": "NOUN",
-    }
-    sconj_list = {
-        "که",
-        "تا",
-        "گرچه",
-        "اگرچه",
-        "چرا",
-        "زیرا",
-        "اگر",
-        "چون",
-        "چراکه",
-        "هرچند",
-        "وگرنه",
-        "چنانچه",
-        "والا",
-        "هرچه",
-        "ولو",
-        "مگر",
-        "پس",
-        "چو",
-        "چه",
-        "بنابراین",
-        "وقتی",
-        "والّا",
-        "انگاری",
-        "هرچندكه",
-        "درنتيجه",
-        "اگه",
-        "ازآنجاكه",
-        "گر",
-        "وگر",
-        "وقتيكه",
-        "تااينكه",
-        "زمانيكه",
-    }
-    num_adj_list = {
-        "نخست",
-        "دوم",
-        "اول",
-        "پنجم",
-        "آخر",
-        "يازدهم",
-        "نهم",
-        "چهارم",
-        "ششم",
-        "پانزدهم",
-        "دوازدهم",
-        "هشتم",
-        "صدم",
-        "هفتم",
-        "هفدهم",
-        "آخرين",
-        "سيزدهم",
-        "يكم",
-        "بيستم",
-        "ويكم",
-        "دوسوم",
-        "شانزدهم",
-        "هجدهم",
-        "چهاردهم",
-        "ششصدم",
-        "ميليونيم",
-        "وهفتم",
-        "يازدهمين",
-        "هيجدهمين",
-        "واپسين",
-        "چهلم",
-        "هزارم",
-        "وپنجم",
-        "هيجدهم",
-        "ميلياردم",
-        "ميليونيوم",
-        "تريليونيوم",
-        "چهارپنجم",
-        "دهگانه",
-        "ميليونم",
-        "اوّل",
-        "سوّم",
-    }
-    try:
-        old_pos = list(
-            set(tags)
-            & {
-                "N",
-                "V",
-                "AJ",
-                "ADV",
-                "PRO",
-                "DET",
-                "P",
-                "POSTP",
-                "NUM",
-                "CONJ",
-                "PUNC",
-                "CL",
-                "INT",
-                "RES",
-            },
-        )[0]
-        if old_pos == "CONJ" and word in sconj_list:
-            return "SCONJ"
-        if old_pos == "NUM" and word in num_adj_list:
-            return "ADJ" + (",EZ" if "EZ" in tags else "")
-        return map_pos_to_upos[old_pos] + (",EZ" if "EZ" in tags else "")
-    except:
-        return "NOUN"
-
-
-def coarse_pos_e(tags: List[str], word) -> List[str]:
-    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
-
-    Examples:
-        >>> coarse_pos_e(['N','COM','SING'],'الجزیره')
-        'N'
-
-    Args:
-        tags: لیست برچسب‌های ریز.
-
-    Returns:
-        لیست برچسب‌های درشت.
-
-    """
-    try:
-        return list(
-            set(tags)
-            & {
-                "N",
-                "V",
-                "AJ",
-                "ADV",
-                "PRO",
-                "DET",
-                "P",
-                "POSTP",
-                "NUM",
-                "CONJ",
-                "PUNC",
-                "CL",
-                "INT",
-                "RES",
-            },
-        )[0] + (",EZ" if "EZ" in tags else "")
-    except:
-        return "N"
-
-
-def join_verb_parts(sentence: List[Tuple[str, str]]) -> List[Tuple[str, str]]:
-    """جمله را در قالب لیستی از `(توکن، برچسب)‌`ها می‌گیرد و توکن‌های مربوط به
-    افعال چندبخشی را با کاراکتر زیرخط (_) به هم می‌چسباند.
-
-    Examples:
-        >>> join_verb_parts([('اولین', 'AJ'), ('سیاره', 'Ne'), ('خارج', 'AJ'), ('از', 'P'), ('منظومه', 'Ne'), ('شمسی', 'AJ'), ('دیده', 'AJ'), ('شد', 'V'), ('.', 'PUNC')])
-        [('اولین', 'AJ'), ('سیاره', 'Ne'), ('خارج', 'AJ'), ('از', 'P'), ('منظومه', 'Ne'), ('شمسی', 'AJ'), ('دیده_شد', 'V'), ('.', 'PUNC')]
-
-    Args:
-        sentence: جمله در قالب لیستی از `(توکن، برچسب)`ها.
-
-    Returns:
-        لیستی از `(توکن، برچسب)`ها که در آن افعال چندبخشی در قالب یک توکن با کاراکتر زیرخط به هم چسبانده شده‌اند.
-
-    """
-    if not hasattr(join_verb_parts, "tokenizer"):
-        join_verb_parts.tokenizer = WordTokenizer()
-    before_verbs, after_verbs, verbe = (
-        join_verb_parts.tokenizer.before_verbs,
-        join_verb_parts.tokenizer.after_verbs,
-        join_verb_parts.tokenizer.verbe,
-    )
-
-    result = [("", "")]
-    for word in reversed(sentence):
-        if word[0] in before_verbs or (
-            result[-1][0] in after_verbs and word[0] in verbe
-        ):
-            result[-1] = (word[0] + "_" + result[-1][0], result[-1][1])
-        else:
-            result.append(word)
-    return list(reversed(result[1:]))
-
-
-class PeykareReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ Peykare است.
-
-    Args:
-        root: آدرس فولدر حاوی فایل‌های پیکره.
-        joined_verb_parts: اگر `True‍` باشد افعال چندقسمتی به‌شکل چسبیده‌به‌هم برگردانده_می‌شود.
-        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
-
-    """
-
-    def __init__(
-        self: "PeykareReader",
-        root: str,
-        joined_verb_parts: bool = True,
-        pos_map: str = coarse_pos_e,
-        universal_pos: bool = False,
-    ) -> None:
-        self._root = root
-        if pos_map is None:
-            self._pos_map = lambda tags: ",".join(tags)
-        elif universal_pos:
-            self._pos_map = coarse_pos_u
-        else:
-            self._pos_map = coarse_pos_e
-        self._joined_verb_parts = joined_verb_parts
-        self._normalizer = Normalizer(correct_spacing=False)
-
-    def docs(self: "PeykareReader") -> Iterator[str]:
-        """اسناد را به شکل متن خام برمی‌گرداند.
-
-        Yields:
-            متن خام سند بعدی.
-
-        """
-        for root, _, files in os.walk(self._root):
-            for name in sorted(files):
-                with codecs.open(
-                    Path(root) / name,
-                    encoding="windows-1256",
-                ) as peykare_file:
-                    text = peykare_file.read()
-                    if text:
-                        yield text
-
-    def doc_to_sents(
-        self: "PeykareReader", document: str,
-    ) -> Iterator[List[Tuple[str, str]]]:
-        """سند ورودی را به لیستی از جملات تبدیل می‌کند.
-
-        هر جمله لیستی از `(کلمه, برچسب)`ها است.
-
-        Args:
-            document: سندی که باید تبدیل شود.
-
-        Yields:
-            `ها جملهٔ بعدی در قالب لیستی از `(کلمه، برچسب).
-
-        """
-        sentence = []
-        for line in document.split("\r\n"):
-            if not line:
-                continue
-
-            parts = line.split(" ")
-            tags, word = parts[3], self._normalizer.normalize("‌".join(parts[4:]))
-
-            if word and word != "#":
-                sentence.append((word, tags))
-
-            if parts[2] == "PUNC" and word in {"#", ".", "؟", "!"}:
-                if len(sentence) > 1:
-                    yield sentence
-                sentence = []
-
-    def sents(self: "PeykareReader") -> Iterator[List[Tuple[str, str]]]:
-        """جملات پیکره را در قالب لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
-
-        Examples:
-            >>> peykare = PeykareReader(root='corpora/peykare')
-            >>> next(peykare.sents())
-            [('دیرزمانی', 'N'), ('از', 'P'), ('راه\u200cاندازی', 'N,EZ'), ('شبکه\u200cی', 'N,EZ'), ('خبر', 'N,EZ'), ('الجزیره', 'N'), ('نمی\u200cگذرد', 'V'), ('،', 'PUNC'), ('اما', 'CONJ'), ('این', 'DET'), ('شبکه\u200cی', 'N,EZ'), ('خبری', 'AJ,EZ'), ('عربی', 'N'), ('بسیار', 'ADV'), ('سریع', 'ADV'), ('توانسته', 'V'), ('در', 'P'), ('میان', 'N,EZ'), ('شبکه\u200cهای', 'N,EZ'), ('عظیم', 'AJ,EZ'), ('خبری', 'AJ'), ('و', 'CONJ'), ('بنگاه\u200cهای', 'N,EZ'), ('چندرسانه\u200cای', 'AJ,EZ'), ('دنیا', 'N'), ('خودی', 'N'), ('نشان', 'N'), ('دهد', 'V'), ('.', 'PUNC')]
-
-        Yields:
-            جملهٔ بعدی در قالب لیستی از `(توکن، برچسب)`ها.
-
-        """
-
-        # >>> peykare = PeykareReader(root='corpora/peykare', joined_verb_parts=False, pos_map=None)
-        # >>> next(peykare.sents())
-        def map_pos(item: str) -> Tuple:
-            return (item[0], self._pos_map(item[1].split(","), item[0]))
-
-        for document in self.docs():
-            for sentence in self.doc_to_sents(document):
-                if self._joined_verb_parts:
-                    sentence = join_verb_parts(sentence)
-
-                yield list(map(map_pos, sentence))
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ Peykare است.
+
+[peykare پیکرهٔ](https://www.peykaregan.ir/dataset/%D9%BE%DB%8C%DA%A9%D8%B1%D9%
+87-%D9%85%D8%AA%D9%86%DB%8C-%D8%B2%D8%A8%D8%A7%D9%86-
+%D9%81%D8%A7%D8%B1%D8%B3%DB%8C)
+جموعه‌ای از متون نوشتاری و گفتاری رسمی زبان فارسی است که از منابع واقعی همچون
+روزنامه‌ها، سایت‌ها و مستنداتِ از قبل تایپ‌شده، جمع‌آوری شده، تصحیح گردیده و
+برچسب خورده است. حجم این دادگان حدوداً ۱۰۰ میلیون کلمه است و از منابع مختلف
+تهیه
+گردیده و دارای تنوع بسیار زیادی است. ۱۰ میلیون کلمه از این پیکره با استفاده از
+۸۸۲ برچسب نحوی-معنایی به صورت دستی توسط دانشجویان رشتهٔ زبان‌شناسی برچسب‌دهی
+شده‌اند و هر پرونده بر حسب موضوع و منبع آن طبقه‌بندی شده است. این پیکره که توسط
+پژوهشکده پردازش هوشمند علائم تهیه شده است، برای استفاده در آموزش مدل زبانی و
+سایر پروژه‌های مربوط به پردازش زبان طبیعی مناسب است.
+
+"""
+
+
+import codecs
+import os
+from pathlib import Path
+from typing import Any
+from typing import Iterator
+from typing import List
+from typing import Tuple
+
+from hazm.normalizer import Normalizer
+from hazm.word_tokenizer import WordTokenizer
+
+
+def coarse_pos_u(tags: List[str], word: str) -> List[str]:
+    """برچسب‌های ریز را به برچسب‌های درشت منطبق با استاندارد جهانی (coarse-grained
+    universal pos tags) تبدیل می‌کند.
+
+    Examples:
+        >>> coarse_pos_u(['N','COM','SING'], 'الجزیره')
+        'NOUN'
+
+    Args:
+        tags: لیست برچسب‌های ریز.
+        word: برچسبی که می‌خواهید به برچسب جهانی تبدیل شود.
+
+    Returns:
+        لیست برچسب‌های درشت جهانی.
+
+    """
+    map_pos_to_upos = {
+        "N": "NOUN",
+        "V": "VERB",
+        "AJ": "ADJ",
+        "ADV": "ADV",
+        "PRO": "PRON",
+        "DET": "DET",
+        "P": "ADP",
+        "POSTP": "ADP",
+        "NUM": "NUM",
+        "CONJ": "CCONJ",
+        "PUNC": "PUNCT",
+        "CL": "NOUN",
+        "INT": "INTJ",
+        "RES": "NOUN",
+    }
+    sconj_list = {
+        "که",
+        "تا",
+        "گرچه",
+        "اگرچه",
+        "چرا",
+        "زیرا",
+        "اگر",
+        "چون",
+        "چراکه",
+        "هرچند",
+        "وگرنه",
+        "چنانچه",
+        "والا",
+        "هرچه",
+        "ولو",
+        "مگر",
+        "پس",
+        "چو",
+        "چه",
+        "بنابراین",
+        "وقتی",
+        "والّا",
+        "انگاری",
+        "هرچندكه",
+        "درنتيجه",
+        "اگه",
+        "ازآنجاكه",
+        "گر",
+        "وگر",
+        "وقتيكه",
+        "تااينكه",
+        "زمانيكه",
+    }
+    num_adj_list = {
+        "نخست",
+        "دوم",
+        "اول",
+        "پنجم",
+        "آخر",
+        "يازدهم",
+        "نهم",
+        "چهارم",
+        "ششم",
+        "پانزدهم",
+        "دوازدهم",
+        "هشتم",
+        "صدم",
+        "هفتم",
+        "هفدهم",
+        "آخرين",
+        "سيزدهم",
+        "يكم",
+        "بيستم",
+        "ويكم",
+        "دوسوم",
+        "شانزدهم",
+        "هجدهم",
+        "چهاردهم",
+        "ششصدم",
+        "ميليونيم",
+        "وهفتم",
+        "يازدهمين",
+        "هيجدهمين",
+        "واپسين",
+        "چهلم",
+        "هزارم",
+        "وپنجم",
+        "هيجدهم",
+        "ميلياردم",
+        "ميليونيوم",
+        "تريليونيوم",
+        "چهارپنجم",
+        "دهگانه",
+        "ميليونم",
+        "اوّل",
+        "سوّم",
+    }
+    try:
+        old_pos = list(
+            set(tags)
+            & {
+                "N",
+                "V",
+                "AJ",
+                "ADV",
+                "PRO",
+                "DET",
+                "P",
+                "POSTP",
+                "NUM",
+                "CONJ",
+                "PUNC",
+                "CL",
+                "INT",
+                "RES",
+            },
+        )[0]
+        if old_pos == "CONJ" and word in sconj_list:
+            return "SCONJ"
+        if old_pos == "NUM" and word in num_adj_list:
+            return "ADJ" + (",EZ" if "EZ" in tags else "")
+        return map_pos_to_upos[old_pos] + (",EZ" if "EZ" in tags else "")
+    except:
+        return "NOUN"
+
+
+def coarse_pos_e(tags: List[str], word) -> List[str]: # noqa: D417, ARG001
+    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
+
+    Examples:
+        >>> coarse_pos_e(['N','COM','SING'],'الجزیره')
+        'N'
+
+    Args:
+        tags: لیست برچسب‌های ریز.
+
+    Returns:
+        لیست برچسب‌های درشت.
+
+    """
+    try:
+        return list(
+            set(tags)
+            & {
+                "N",
+                "V",
+                "AJ",
+                "ADV",
+                "PRO",
+                "DET",
+                "P",
+                "POSTP",
+                "NUM",
+                "CONJ",
+                "PUNC",
+                "CL",
+                "INT",
+                "RES",
+            },
+        )[0] + (",EZ" if "EZ" in tags else "")
+    except:
+        return "N"
+
+
+def join_verb_parts(sentence: List[Tuple[str, str]]) -> List[Tuple[str, str]]:
+    """جمله را در قالب لیستی از `(توکن، برچسب)‌`ها می‌گیرد و توکن‌های مربوط به
+    افعال چندبخشی را با کاراکتر زیرخط (_) به هم می‌چسباند.
+
+    Examples:
+        >>> join_verb_parts([('اولین', 'AJ'), ('سیاره', 'Ne'), ('خارج', 'AJ'), ('از', 'P'), ('منظومه', 'Ne'), ('شمسی', 'AJ'), ('دیده', 'AJ'), ('شد', 'V'), ('.', 'PUNC')])
+        [('اولین', 'AJ'), ('سیاره', 'Ne'), ('خارج', 'AJ'), ('از', 'P'), ('منظومه', 'Ne'), ('شمسی', 'AJ'), ('دیده_شد', 'V'), ('.', 'PUNC')]
+
+    Args:
+        sentence: جمله در قالب لیستی از `(توکن، برچسب)`ها.
+
+    Returns:
+        لیستی از `(توکن، برچسب)`ها که در آن افعال چندبخشی در قالب یک توکن با کاراکتر زیرخط به هم چسبانده شده‌اند.
+
+    """
+    if not hasattr(join_verb_parts, "tokenizer"):
+        join_verb_parts.tokenizer = WordTokenizer()
+    before_verbs, after_verbs, verbe = (
+        join_verb_parts.tokenizer.before_verbs,
+        join_verb_parts.tokenizer.after_verbs,
+        join_verb_parts.tokenizer.verbe,
+    )
+
+    result = [("", "")]
+    for word in reversed(sentence):
+        if word[0] in before_verbs or (
+            result[-1][0] in after_verbs and word[0] in verbe
+        ):
+            result[-1] = (word[0] + "_" + result[-1][0], result[-1][1])
+        else:
+            result.append(word)
+    return list(reversed(result[1:]))
+
+
+class PeykareReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ Peykare است.
+
+    Args:
+        root: آدرس فولدر حاوی فایل‌های پیکره.
+        joined_verb_parts: اگر `True‍` باشد افعال چندقسمتی به‌شکل چسبیده‌به‌هم برگردانده_می‌شود.
+        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
+
+    """
+
+    def __init__(
+        self: "PeykareReader",
+        root: str,
+        joined_verb_parts: bool = True,
+        pos_map: str = coarse_pos_e,
+        universal_pos: bool = False,
+    ) -> None:
+        self._root = root
+        if pos_map is None:
+            self._pos_map = lambda tags: ",".join(tags)
+        elif universal_pos:
+            self._pos_map = coarse_pos_u
+        else:
+            self._pos_map = coarse_pos_e
+        self._joined_verb_parts = joined_verb_parts
+        self._normalizer = Normalizer(correct_spacing=False)
+
+    def docs(self: "PeykareReader") -> Iterator[str]:
+        """اسناد را به شکل متن خام برمی‌گرداند.
+
+        Yields:
+            متن خام سند بعدی.
+
+        """
+        for root, _, files in os.walk(self._root):
+            for name in sorted(files):
+                with codecs.open(
+                    Path(root) / name,
+                    encoding="windows-1256",
+                ) as peykare_file:
+                    text = peykare_file.read()
+                    if text:
+                        yield text
+
+    def doc_to_sents(
+        self: "PeykareReader", document: str,
+    ) -> Iterator[List[Tuple[str, str]]]:
+        """سند ورودی را به لیستی از جملات تبدیل می‌کند.
+
+        هر جمله لیستی از `(کلمه, برچسب)`ها است.
+
+        Args:
+            document: سندی که باید تبدیل شود.
+
+        Yields:
+            `ها جملهٔ بعدی در قالب لیستی از `(کلمه، برچسب).
+
+        """
+        sentence = []
+        for line in document.split("\r\n"):
+            if not line:
+                continue
+
+            parts = line.split(" ")
+            tags, word = parts[3], self._normalizer.normalize("‌".join(parts[4:]))
+
+            if word and word != "#":
+                sentence.append((word, tags))
+
+            if parts[2] == "PUNC" and word in {"#", ".", "؟", "!"}:
+                if len(sentence) > 1:
+                    yield sentence
+                sentence = []
+
+    def sents(self: "PeykareReader") -> Iterator[List[Tuple[str, str]]]:
+        """جملات پیکره را در قالب لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
+
+        Examples:
+            >>> peykare = PeykareReader(root='peykare')
+            >>> next(peykare.sents())
+            [('دیرزمانی', 'N'), ('از', 'P'), ('راه\u200cاندازی', 'N,EZ'), ('شبکه\u200cی', 'N,EZ'), ('خبر', 'N,EZ'), ('الجزیره', 'N'), ('نمی\u200cگذرد', 'V'), ('،', 'PUNC'), ('اما', 'CONJ'), ('این', 'DET'), ('شبکه\u200cی', 'N,EZ'), ('خبری', 'AJ,EZ'), ('عربی', 'N'), ('بسیار', 'ADV'), ('سریع', 'ADV'), ('توانسته', 'V'), ('در', 'P'), ('میان', 'N,EZ'), ('شبکه\u200cهای', 'N,EZ'), ('عظیم', 'AJ,EZ'), ('خبری', 'AJ'), ('و', 'CONJ'), ('بنگاه\u200cهای', 'N,EZ'), ('چندرسانه\u200cای', 'AJ,EZ'), ('دنیا', 'N'), ('خودی', 'N'), ('نشان', 'N'), ('دهد', 'V'), ('.', 'PUNC')]
+
+        Yields:
+            جملهٔ بعدی در قالب لیستی از `(توکن، برچسب)`ها.
+
+        """
+
+        # >>> peykare = PeykareReader(root='peykare', joined_verb_parts=False, pos_map=None)
+        # >>> next(peykare.sents())
+        def map_pos(item: str) -> Tuple:
+            return (item[0], self._pos_map(item[1].split(","), item[0]))
+
+        for document in self.docs():
+            for sentence in self.doc_to_sents(document):
+                if self._joined_verb_parts:
+                    sentence = join_verb_parts(sentence)
+
+                yield list(map(map_pos, sentence))
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/quran_reader.py` & `hazm-0.9.2/hazm/corpus_readers/quran_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ Quranic Arabic است.
-
-پیکرهٔ [Quranic Arabic](https://corpus.quran.com/) شامل قواعد نحوی و اطلاعات
-ریخت‌شناسی تک‌تک کلمات قرآن کریم است.
-
-"""
-from pathlib import Path
-from typing import Dict
-from typing import Iterator
-from typing import List
-from typing import Tuple
-
-from hazm.utils import maketrans
-
-buckwalter_transliteration = maketrans(
-    "'>&<}AbptvjHxd*rzs$SDTZEg_fqklmnhwYyFNKaui~o^#`{:@\"[;,.!-+%]",
-    "\u0621\u0623\u0624\u0625\u0626\u0627\u0628\u0629\u062a\u062b\u062c\u062d\u062e\u062f\u0630\u0631\u0632\u0633\u0634\u0635\u0636\u0637\u0638\u0639\u063a\u0640\u0641\u0642\u0643\u0644\u0645\u0646\u0647\u0648\u0649\u064a\u064b\u064c\u064d\u064e\u064f\u0650\u0651\u0652\u0653\u0654\u0670\u0671\u06dc\u06df\u06e0\u06e2\u06e3\u06e5\u06e6\u06e8\u06ea\u06eb\u06ec\u06ed",
-)
-
-
-class QuranReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ Quranic Arabic است.
-
-    Args:
-        quran_file: مسیر فایلِ پیکره
-
-    """
-
-    def __init__(self: "QuranReader", quran_file: str) -> None:
-        self._quran_file = quran_file
-
-    def parts(self: "QuranReader") -> Iterator[Dict[str, str]]:
-        """اجزای متن قرآن را به‌همراه اطلاعات نحوی‌شان برمی‌گرداند.
-
-        یک جزء لزوماً یک کلمه نیست؛ مثلاً واژهٔ «الرحمن» از دو جزء «ال» و «رحمن» تشکیل
-        شده است.
-
-        Examples:
-            >>> parts=QuranReader(quran_file='corpora/quranic_corpus_morphology.txt').parts()
-            >>> print(next(parts))
-            {'loc': (1, 1, 1, 1), 'text': 'بِ', 'tag': 'P'}
-            >>> print(next(parts))
-            {'loc': (1, 1, 1, 2), 'text': 'سْمِ', 'tag': 'N', 'lem': 'ٱسْم', 'root': 'سمو'}
-            >>> print(next(parts))
-            {'loc': (1, 1, 2, 1), 'text': 'ٱللَّهِ', 'tag': 'PN', 'lem': 'ٱللَّه', 'root': 'اله'}
-
-        Yields:
-            جزء بعدی متن قرآن.
-
-        """
-        for line in Path(self._quran_file).open(encoding="utf8"):
-            if not line.startswith("("):
-                continue
-            parts = line.strip().split("\t")
-
-            part = {
-                "loc": eval(parts[0].replace(":", ",")),
-                "text": parts[1].translate(buckwalter_transliteration),
-                "tag": parts[2],
-            }
-
-            features = parts[3].split("|")
-            for feature in features:
-                if feature.startswith("LEM:"):
-                    part["lem"] = feature[4:].translate(buckwalter_transliteration)
-                elif feature.startswith("ROOT:"):
-                    part["root"] = feature[5:].translate(buckwalter_transliteration)
-            yield part
-
-    def words(
-        self: "QuranReader",
-    ) -> Iterator[Tuple[str, str, str, str, str, List[Dict[str, str]]]]:
-        """اطلاعات صرفی کلمات قرآن را برمی‌گرداند.
-
-        Examples:
-            >>> words=QuranReader(quran_file='corpora/quranic_corpus_morphology.txt').words()
-            >>> print(next(words))
-            ('1.1.1', 'بِسْمِ', 'ٱسْم', 'سمو', 'P-N', [{'text': 'بِ', 'tag': 'P'}, {'text': 'سْمِ', 'tag': 'N', 'lem': 'ٱسْم', 'root': 'سمو'}])
-
-        Yields:
-            اطلاعات صرفی کلمهٔ بعدی قرآن.
-
-        """
-
-        def word_item(location: Tuple[int], parts: List[Dict]) -> str:
-            text = "".join([part["text"] for part in parts])
-            tag = "-".join([part["tag"] for part in parts])
-            lem = "-".join([part["lem"] for part in parts if "lem" in part])
-            root = "-".join([part["root"] for part in parts if "root" in part])
-            return ".".join(map(str, location)), text, lem, root, tag, parts
-
-        last_location = (0, 0, 0, 0)
-        items = []
-        for part in self.parts():
-            if last_location[:3] == part["loc"][:3]:
-                items.append(part)
-            else:
-                if items:
-                    yield word_item(last_location[:3], items)
-                items = [part]
-            last_location = part["loc"]
-            del part["loc"]
-        yield word_item(last_location[:3], items)
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ Quranic Arabic است.
+
+پیکرهٔ [Quranic Arabic](https://corpus.quran.com/) شامل قواعد نحوی و اطلاعات
+ریخت‌شناسی تک‌تک کلمات قرآن کریم است.
+
+"""
+from pathlib import Path
+from typing import Dict
+from typing import Iterator
+from typing import List
+from typing import Tuple
+
+from hazm.utils import maketrans
+
+buckwalter_transliteration = maketrans(
+    "'>&<}AbptvjHxd*rzs$SDTZEg_fqklmnhwYyFNKaui~o^#`{:@\"[;,.!-+%]",
+    "\u0621\u0623\u0624\u0625\u0626\u0627\u0628\u0629\u062a\u062b\u062c\u062d\u062e\u062f\u0630\u0631\u0632\u0633\u0634\u0635\u0636\u0637\u0638\u0639\u063a\u0640\u0641\u0642\u0643\u0644\u0645\u0646\u0647\u0648\u0649\u064a\u064b\u064c\u064d\u064e\u064f\u0650\u0651\u0652\u0653\u0654\u0670\u0671\u06dc\u06df\u06e0\u06e2\u06e3\u06e5\u06e6\u06e8\u06ea\u06eb\u06ec\u06ed",
+)
+
+
+class QuranReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ Quranic Arabic است.
+
+    Args:
+        quran_file: مسیر فایلِ پیکره
+
+    """
+
+    def __init__(self: "QuranReader", quran_file: str) -> None:
+        self._quran_file = quran_file
+
+    def parts(self: "QuranReader") -> Iterator[Dict[str, str]]:
+        """اجزای متن قرآن را به‌همراه اطلاعات نحوی‌شان برمی‌گرداند.
+
+        یک جزء لزوماً یک کلمه نیست؛ مثلاً واژهٔ «الرحمن» از دو جزء «ال» و «رحمن» تشکیل
+        شده است.
+
+        Examples:
+            >>> parts=QuranReader(quran_file='quranic_corpus_morphology.txt').parts()
+            >>> print(next(parts))
+            {'loc': (1, 1, 1, 1), 'text': 'بِ', 'tag': 'P'}
+            >>> print(next(parts))
+            {'loc': (1, 1, 1, 2), 'text': 'سْمِ', 'tag': 'N', 'lem': 'ٱسْم', 'root': 'سمو'}
+            >>> print(next(parts))
+            {'loc': (1, 1, 2, 1), 'text': 'ٱللَّهِ', 'tag': 'PN', 'lem': 'ٱللَّه', 'root': 'اله'}
+
+        Yields:
+            جزء بعدی متن قرآن.
+
+        """
+        for line in Path(self._quran_file).open(encoding="utf8"):
+            if not line.startswith("("):
+                continue
+            parts = line.strip().split("\t")
+
+            part = {
+                "loc": eval(parts[0].replace(":", ",")), # noqa: PGH001
+                "text": parts[1].translate(buckwalter_transliteration),
+                "tag": parts[2],
+            }
+
+            features = parts[3].split("|")
+            for feature in features:
+                if feature.startswith("LEM:"):
+                    part["lem"] = feature[4:].translate(buckwalter_transliteration)
+                elif feature.startswith("ROOT:"):
+                    part["root"] = feature[5:].translate(buckwalter_transliteration)
+            yield part
+
+    def words(
+        self: "QuranReader",
+    ) -> Iterator[Tuple[str, str, str, str, str, List[Dict[str, str]]]]:
+        """اطلاعات صرفی کلمات قرآن را برمی‌گرداند.
+
+        Examples:
+            >>> words=QuranReader(quran_file='quranic_corpus_morphology.txt').words()
+            >>> print(next(words))
+            ('1.1.1', 'بِسْمِ', 'ٱسْم', 'سمو', 'P-N', [{'text': 'بِ', 'tag': 'P'}, {'text': 'سْمِ', 'tag': 'N', 'lem': 'ٱسْم', 'root': 'سمو'}])
+
+        Yields:
+            اطلاعات صرفی کلمهٔ بعدی قرآن.
+
+        """
+
+        def word_item(location: Tuple[int], parts: List[Dict]) -> str:
+            text = "".join([part["text"] for part in parts])
+            tag = "-".join([part["tag"] for part in parts])
+            lem = "-".join([part["lem"] for part in parts if "lem" in part])
+            root = "-".join([part["root"] for part in parts if "root" in part])
+            return ".".join(map(str, location)), text, lem, root, tag, parts
+
+        last_location = (0, 0, 0, 0)
+        items = []
+        for part in self.parts():
+            if last_location[:3] == part["loc"][:3]:
+                items.append(part)
+            else:
+                if items:
+                    yield word_item(last_location[:3], items)
+                items = [part]
+            last_location = part["loc"]
+            del part["loc"]
+        yield word_item(last_location[:3], items)
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/sentipers_reader.py` & `hazm-0.9.2/hazm/corpus_readers/sentipers_reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ سِنتی‌پِرِس است.
-
-سِنتی‌پرس شامل مجموعه‌ای از متون فارسی با برچسب‌های معنایی است.
-
-"""
-
-
-import itertools
-import os
-import sys
-from pathlib import Path
-from typing import Any
-from typing import Dict
-from typing import Iterator
-from xml.dom import minidom
-
-
-class SentiPersReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ سِنتی‌پِرِس است.
-
-    Args:
-        root: مسیر فولدر حاوی فایل‌های پیکره
-
-    """
-
-    def __init__(self: "SentiPersReader", root: str) -> None:
-        self._root = root
-
-    def docs(self: "SentiPersReader") -> Iterator[Dict[str, Any]]:
-        """متن‌های فارسی را در قالب یک برمی‌گرداند.
-
-        هر متن شامل این فیلدهاست:
-
-        - عنوان (Title)
-        - نوع (Type)
-        - نظرات (comments)
-
-        فیلد `comments `خودش شامل این فیلدهاست:
-
-        - شناسه (id)
-        - نوع (type)
-        - نویسنده (author)
-        - ارزش (value)
-        - جملات (sentences)
-
-        Yields:
-            متن بعدی.
-
-        """
-
-        def element_sentences(element: str) -> Iterator[Dict]:
-            for sentence in element.getElementsByTagName("Sentence"):
-                yield {
-                    "text": sentence.childNodes[0].data,
-                    "id": sentence.getAttribute("ID"),
-                    "value": (
-                        int(sentence.getAttribute("Value"))
-                        if comment.getAttribute("Value")
-                        else None
-                    ),
-                }
-
-        for root, _dirs, files in os.walk(self._root):
-            for filename in sorted(files):
-                try:
-                    elements = minidom.parse(os.path.join(root, filename))
-
-                    product = elements.getElementsByTagName("Product")[0]
-                    doc = {
-                        "Title": product.getAttribute("Title"),
-                        "Type": product.getAttribute("Type"),
-                        "comments": [],
-                    }
-
-                    for child in product.childNodes:
-                        if child.nodeName in {
-                            "Voters",
-                            "Performance",
-                            "Capability",
-                            "Production_Quality",
-                            "Ergonomics",
-                            "Purchase_Value",
-                        }:
-                            value = child.getAttribute("Value")
-                            doc[child.nodeName] = (
-                                float(value) if "." in value else int(value)
-                            )
-
-                    for comment in itertools.chain(
-                        elements.getElementsByTagName("Opinion"),
-                        elements.getElementsByTagName("Criticism"),
-                    ):
-                        doc["comments"].append(
-                            {
-                                "id": comment.getAttribute("ID"),
-                                "type": comment.nodeName,
-                                "author": comment.getAttribute("Holder").strip(),
-                                "value": (
-                                    int(comment.getAttribute("Value"))
-                                    if comment.getAttribute("Value")
-                                    else None
-                                ),
-                                "sentences": list(element_sentences(comment)),
-                            },
-                        )
-
-                    # todo: Accessories, Features, Review, Advantages, Tags, Keywords, Index
-
-                    yield doc
-
-                except Exception as e:
-                    print("error in reading", filename, e, file=sys.stderr)
-
-    def comments(self: "SentiPersReader") -> Iterator[str]:
-        """نظرات مربوط به متن را برمی‌گرداند.
-
-        Examples:
-            >>> sentipers = SentiPersReader(root='corpora/sentipers')
-            >>> next(sentipers.comments())[0][1]
-            'بيشتر مناسب است براي کساني که به دنبال تنوع هستند و در همه چيز نو گرايي دارند .'
-
-        Yields:
-            نظر بعدی.
-
-        """
-        for doc in self.docs():
-            yield [
-                [sentence["text"] for sentence in text]
-                for text in [comment["sentences"] for comment in doc["comments"]]
-            ]
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ سِنتی‌پِرِس است.
+
+سِنتی‌پرس شامل مجموعه‌ای از متون فارسی با برچسب‌های معنایی است.
+
+"""
+
+
+import itertools
+import os
+import sys
+from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import Iterator
+from xml.dom import minidom
+
+
+class SentiPersReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ سِنتی‌پِرِس است.
+
+    Args:
+        root: مسیر فولدر حاوی فایل‌های پیکره
+
+    """
+
+    def __init__(self: "SentiPersReader", root: str) -> None:
+        self._root = root
+
+    def docs(self: "SentiPersReader") -> Iterator[Dict[str, Any]]:
+        """متن‌های فارسی را در قالب یک برمی‌گرداند.
+
+        هر متن شامل این فیلدهاست:
+
+        - عنوان (Title)
+        - نوع (Type)
+        - نظرات (comments)
+
+        فیلد `comments `خودش شامل این فیلدهاست:
+
+        - شناسه (id)
+        - نوع (type)
+        - نویسنده (author)
+        - ارزش (value)
+        - جملات (sentences)
+
+        Yields:
+            متن بعدی.
+
+        """
+
+        def element_sentences(element: str) -> Iterator[Dict]:
+            for sentence in element.getElementsByTagName("Sentence"):
+                yield {
+                    "text": sentence.childNodes[0].data,
+                    "id": sentence.getAttribute("ID"),
+                    "value": (
+                        int(sentence.getAttribute("Value"))
+                        if comment.getAttribute("Value")
+                        else None
+                    ),
+                }
+
+        for root, _dirs, files in os.walk(self._root):
+            for filename in sorted(files):
+                try:
+                    elements = minidom.parse(os.path.join(root, filename)) # noqa: PTH118
+
+                    product = elements.getElementsByTagName("Product")[0]
+                    doc = {
+                        "Title": product.getAttribute("Title"),
+                        "Type": product.getAttribute("Type"),
+                        "comments": [],
+                    }
+
+                    for child in product.childNodes:
+                        if child.nodeName in {
+                            "Voters",
+                            "Performance",
+                            "Capability",
+                            "Production_Quality",
+                            "Ergonomics",
+                            "Purchase_Value",
+                        }:
+                            value = child.getAttribute("Value")
+                            doc[child.nodeName] = (
+                                float(value) if "." in value else int(value)
+                            )
+
+                    for comment in itertools.chain(
+                        elements.getElementsByTagName("Opinion"),
+                        elements.getElementsByTagName("Criticism"),
+                    ):
+                        doc["comments"].append(
+                            {
+                                "id": comment.getAttribute("ID"),
+                                "type": comment.nodeName,
+                                "author": comment.getAttribute("Holder").strip(),
+                                "value": (
+                                    int(comment.getAttribute("Value"))
+                                    if comment.getAttribute("Value")
+                                    else None
+                                ),
+                                "sentences": list(element_sentences(comment)),
+                            },
+                        )
+
+                    # todo: Accessories, Features, Review, Advantages, Tags, Keywords, Index
+
+                    yield doc
+
+                except Exception as e:
+                    print("error in reading", filename, e, file=sys.stderr)
+
+    def comments(self: "SentiPersReader") -> Iterator[str]:
+        """نظرات مربوط به متن را برمی‌گرداند.
+
+        Examples:
+            >>> sentipers = SentiPersReader(root='sentipers')
+            >>> next(sentipers.comments())[0][1]
+            'بيشتر مناسب است براي کساني که به دنبال تنوع هستند و در همه چيز نو گرايي دارند .'
+
+        Yields:
+            نظر بعدی.
+
+        """
+        for doc in self.docs():
+            yield [
+                [sentence["text"] for sentence in text]
+                for text in [comment["sentences"] for comment in doc["comments"]]
+            ]
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/tnews_reader.py` & `hazm-0.9.2/hazm/corpus_readers/tnews_reader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,296 +1,288 @@
 00000000: 2222 22d8 a7db 8cd9 8620 d985 d8a7 da98  """...... ......
 00000010: d988 d984 20d8 b4d8 a7d9 85d9 8420 daa9  .... ........ ..
 00000020: d984 d8a7 d8b3 e280 8cd9 87d8 a720 d988  ............. ..
 00000030: 20d8 aad9 88d8 a7d8 a8d8 b9db 8c20 d8a8   ............ ..
 00000040: d8b1 d8a7 db8c 20d8 aed9 88d8 a7d9 86d8  ...... .........
 00000050: afd9 8620 d9be db8c daa9 d8b1 d987 d994  ... ............
 00000060: 20d8 aadb 8ce2 808c d986 db8c d988 d8b2   ...............
-00000070: 20d8 a7d8 b3d8 aa2e 2222 220d 0a0d 0a0d   .......""".....
-00000080: 0a69 6d70 6f72 7420 6f73 0d0a 696d 706f  .import os..impo
-00000090: 7274 2072 650d 0a69 6d70 6f72 7420 7379  rt re..import sy
-000000a0: 730d 0a66 726f 6d20 7061 7468 6c69 6220  s..from pathlib 
-000000b0: 696d 706f 7274 2050 6174 680d 0a66 726f  import Path..fro
-000000c0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-000000d0: 416e 790d 0a66 726f 6d20 7479 7069 6e67  Any..from typing
-000000e0: 2069 6d70 6f72 7420 4469 6374 0d0a 6672   import Dict..fr
-000000f0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00000100: 2049 7465 7261 746f 720d 0a66 726f 6d20   Iterator..from 
-00000110: 786d 6c2e 646f 6d20 696d 706f 7274 206d  xml.dom import m
-00000120: 696e 6964 6f6d 0d0a 0d0a 0d0a 636c 6173  inidom......clas
-00000130: 7320 544e 6577 7352 6561 6465 723a 0d0a  s TNewsReader:..
-00000140: 2020 2020 2222 22d8 a7db 8cd9 8620 daa9      """...... ..
-00000150: d984 d8a7 d8b3 20d8 b4d8 a7d9 85d9 8420  ...... ........ 
-00000160: d8aa d988 d8a7 d8a8 d8b9 db8c 20d8 a8d8  ............ ...
-00000170: b1d8 a7db 8c20 d8ae d988 d8a7 d986 d8af  ..... ..........
-00000180: d986 20d9 bedb 8cda a9d8 b1d9 87d9 9420  .. ............ 
-00000190: d8aa db8c e280 8cd9 86db 8cd9 88d8 b220  ............... 
-000001a0: d8a7 d8b3 d8aa 2e0d 0a0d 0a20 2020 2041  ...........    A
-000001b0: 7267 733a 0d0a 2020 2020 2020 2020 726f  rgs:..        ro
-000001c0: 6f74 3a20 d985 d8b3 db8c d8b1 20d9 81d9  ot: ........ ...
-000001d0: 88d9 84d8 afd8 b120 d8ad d8a7 d988 db8c  ....... ........
-000001e0: 20d9 81d8 a7db 8cd9 84e2 808c d987 d8a7   ...............
-000001f0: db8c 20d9 bedb 8cda a9d8 b1d9 872e 0d0a  .. .............
-00000200: 0d0a 2020 2020 2222 220d 0a0d 0a20 2020  ..    """....   
-00000210: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00000220: 6c66 3a20 2254 4e65 7773 5265 6164 6572  lf: "TNewsReader
-00000230: 222c 2072 6f6f 743a 2073 7472 2920 2d3e  ", root: str) ->
-00000240: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00000250: 7365 6c66 2e5f 726f 6f74 203d 2072 6f6f  self._root = roo
-00000260: 740d 0a20 2020 2020 2020 2073 656c 662e  t..        self.
-00000270: 636c 6561 6e65 7220 3d20 7265 2e63 6f6d  cleaner = re.com
-00000280: 7069 6c65 2872 223c 5b5e 3c3e 5d2b 3e22  pile(r"<[^<>]+>"
-00000290: 290d 0a0d 0a20 2020 2064 6566 2064 6f63  )....    def doc
-000002a0: 7328 7365 6c66 3a20 2254 4e65 7773 5265  s(self: "TNewsRe
-000002b0: 6164 6572 2229 202d 3e20 4974 6572 6174  ader") -> Iterat
-000002c0: 6f72 5b44 6963 745b 7374 722c 2073 7472  or[Dict[str, str
-000002d0: 5d5d 3a0d 0a20 2020 2020 2020 2022 2222  ]]:..        """
-000002e0: d8ae d8a8 d8b1 d987 d8a7 20d8 b1d8 a720  .......... .... 
-000002f0: d8af d8b1 20d9 82d8 a7d9 84d8 a820 db8c  .... ........ ..
-00000300: daa9 2060 6974 6572 6174 6f72 6020 d8a8  .. `iterator` ..
-00000310: d8b1 d985 db8c e280 8cda afd8 b1d8 afd8  ................
-00000320: a7d9 86d8 af2e 0d0a 0d0a 2020 2020 2020  ..........      
-00000330: 2020 d987 d8b1 20d8 aed8 a8d8 b1d8 8c20    .... ........ 
-00000340: d8b4 db8c e280 8cd8 a7db 8c20 d985 d8aa  ........... ....
-00000350: d8b4 daa9 d984 20d8 a7d8 b220 da86 d986  ...... .... ....
-00000360: d8af 20d9 bed8 a7d8 b1d8 a7d9 85d8 aad8  .. .............
-00000370: b120 d8a7 d8b3 d8aa 3a0d 0a0d 0a20 2020  . ......:....   
-00000380: 2020 2020 202d 20d8 b4d9 86d8 a7d8 b3d9       - .........
-00000390: 8720 2869 6429 d88c 0d0a 2020 2020 2020  . (id)....      
-000003a0: 2020 2d20 d8b9 d986 d988 d8a7 d986 2028    - .......... (
-000003b0: 7469 746c 6529 d88c 0d0a 2020 2020 2020  title)....      
-000003c0: 2020 2d20 d9be db8c d8b4 20d8 a7d8 b220    - ...... .... 
-000003d0: d8b9 d986 d988 d8a7 d986 2028 7072 652d  .......... (pre-
-000003e0: 7469 746c 6529 d88c 0d0a 2020 2020 2020  title)....      
-000003f0: 2020 2d20 d9be d8b3 20d8 a7d8 b220 d8b9    - .... .... ..
-00000400: d986 d988 d8a7 d986 2028 706f 7374 2d74  ........ (post-t
-00000410: 6974 6c65 29d8 8c0d 0a20 2020 2020 2020  itle)....       
-00000420: 202d 20d9 85d8 aad9 8620 2874 6578 7429   - ...... (text)
-00000430: d88c 0d0a 2020 2020 2020 2020 2d20 d8ae  ....        - ..
-00000440: d984 d8a7 d8b5 d987 2028 6272 6965 6629  ........ (brief)
-00000450: d88c 0d0a 2020 2020 2020 2020 2d20 d8a2  ....        - ..
-00000460: d8af d8b1 d8b3 2028 7572 6c29 d88c 0d0a  ...... (url)....
-00000470: 2020 2020 2020 2020 2d20 d985 d988 d8b6          - ......
-00000480: d988 d8b9 2028 6361 7465 676f 7279 29d8  .... (category).
-00000490: 8c0d 0a20 2020 2020 2020 202d 20d8 aad8  ...        - ...
-000004a0: a7d8 b1db 8cd8 ae20 d988 20d8 b2d9 85d8  ....... .. .....
-000004b0: a7d9 8620 d8a7 d986 d8aa d8b4 d8a7 d8b1  ... ............
-000004c0: 2028 6461 7465 7469 6d65 292e 0d0a 0d0a   (datetime).....
-000004d0: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
-000004e0: 3a0d 0a20 2020 2020 2020 2020 2020 203e  :..            >
-000004f0: 3e3e 2074 6e65 7773 203d 2054 4e65 7773  >> tnews = TNews
-00000500: 5265 6164 6572 2872 6f6f 743d 2763 6f72  Reader(root='cor
-00000510: 706f 7261 2f74 6e65 7773 2729 0d0a 2020  pora/tnews')..  
-00000520: 2020 2020 2020 2020 2020 3e3e 3e20 6e65            >>> ne
-00000530: 7874 2874 6e65 7773 2e64 6f63 7328 2929  xt(tnews.docs())
-00000540: 5b27 6964 275d 0d0a 2020 2020 2020 2020  ['id']..        
-00000550: 2020 2020 2731 3430 3932 3330 3334 3832      '14092303482
-00000560: 3330 3030 3133 3635 3327 0d0a 0d0a 2020  300013653'....  
-00000570: 2020 2020 2020 5969 656c 6473 3a0d 0a20        Yields:.. 
-00000580: 2020 2020 2020 2020 2020 2028 4469 6374             (Dict
-00000590: 293a 20d8 aed8 a8d8 b120 d8a8 d8b9 d8af  ): ...... ......
-000005a0: db8c 2e0d 0a0d 0a20 2020 2020 2020 2022  .......        "
-000005b0: 2222 0d0a 0d0a 2020 2020 2020 2020 6465  ""....        de
-000005c0: 6620 6765 745f 7465 7874 2865 6c65 6d65  f get_text(eleme
-000005d0: 6e74 3a20 7374 7229 202d 3e20 7374 723a  nt: str) -> str:
-000005e0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-000005f0: 775f 6874 6d6c 203d 2065 6c65 6d65 6e74  w_html = element
-00000600: 2e63 6869 6c64 4e6f 6465 735b 305d 2e64  .childNodes[0].d
-00000610: 6174 6120 6966 2065 6c65 6d65 6e74 2e63  ata if element.c
-00000620: 6869 6c64 4e6f 6465 7320 656c 7365 2022  hildNodes else "
-00000630: 220d 0a20 2020 2020 2020 2020 2020 2072  "..            r
-00000640: 6574 7572 6e20 7265 2e73 7562 2873 656c  eturn re.sub(sel
-00000650: 662e 636c 6561 6e65 722c 2022 222c 2072  f.cleaner, "", r
-00000660: 6177 5f68 746d 6c29 0d0a 0d0a 2020 2020  aw_html)....    
-00000670: 2020 2020 666f 7220 726f 6f74 2c20 5f64      for root, _d
-00000680: 6972 732c 2066 696c 6573 2069 6e20 6f73  irs, files in os
-00000690: 2e77 616c 6b28 7365 6c66 2e5f 726f 6f74  .walk(self._root
-000006a0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000006b0: 666f 7220 6e61 6d65 2069 6e20 736f 7274  for name in sort
-000006c0: 6564 2866 696c 6573 293a 0d0a 2020 2020  ed(files):..    
-000006d0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000006e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000006f0: 2020 2020 2020 7061 7468 203d 2050 6174        path = Pat
-00000700: 6828 726f 6f74 2920 2f20 6e61 6d65 0d0a  h(root) / name..
+00000070: 20d8 a7d8 b3d8 aa2e 2222 220a 0a0a 696d   ......."""...im
+00000080: 706f 7274 206f 730a 696d 706f 7274 2072  port os.import r
+00000090: 650a 696d 706f 7274 2073 7973 0a66 726f  e.import sys.fro
+000000a0: 6d20 7061 7468 6c69 6220 696d 706f 7274  m pathlib import
+000000b0: 2050 6174 680a 6672 6f6d 2074 7970 696e   Path.from typin
+000000c0: 6720 696d 706f 7274 2041 6e79 0a66 726f  g import Any.fro
+000000d0: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+000000e0: 4469 6374 0a66 726f 6d20 7479 7069 6e67  Dict.from typing
+000000f0: 2069 6d70 6f72 7420 4974 6572 6174 6f72   import Iterator
+00000100: 0a66 726f 6d20 786d 6c2e 646f 6d20 696d  .from xml.dom im
+00000110: 706f 7274 206d 696e 6964 6f6d 0a0a 0a63  port minidom...c
+00000120: 6c61 7373 2054 4e65 7773 5265 6164 6572  lass TNewsReader
+00000130: 3a0a 2020 2020 2222 22d8 a7db 8cd9 8620  :.    """...... 
+00000140: daa9 d984 d8a7 d8b3 20d8 b4d8 a7d9 85d9  ........ .......
+00000150: 8420 d8aa d988 d8a7 d8a8 d8b9 db8c 20d8  . ............ .
+00000160: a8d8 b1d8 a7db 8c20 d8ae d988 d8a7 d986  ....... ........
+00000170: d8af d986 20d9 bedb 8cda a9d8 b1d9 87d9  .... ...........
+00000180: 9420 d8aa db8c e280 8cd9 86db 8cd9 88d8  . ..............
+00000190: b220 d8a7 d8b3 d8aa 2e0a 0a20 2020 2041  . .........    A
+000001a0: 7267 733a 0a20 2020 2020 2020 2072 6f6f  rgs:.        roo
+000001b0: 743a 20d9 85d8 b3db 8cd8 b120 d981 d988  t: ........ ....
+000001c0: d984 d8af d8b1 20d8 add8 a7d9 88db 8c20  ...... ........ 
+000001d0: d981 d8a7 db8c d984 e280 8cd9 87d8 a7db  ................
+000001e0: 8c20 d9be db8c daa9 d8b1 d987 2e0a 0a20  . ............. 
+000001f0: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
+00000200: 5f5f 696e 6974 5f5f 2873 656c 663a 2022  __init__(self: "
+00000210: 544e 6577 7352 6561 6465 7222 2c20 726f  TNewsReader", ro
+00000220: 6f74 3a20 7374 7229 202d 3e20 4e6f 6e65  ot: str) -> None
+00000230: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00000240: 726f 6f74 203d 2072 6f6f 740a 2020 2020  root = root.    
+00000250: 2020 2020 7365 6c66 2e63 6c65 616e 6572      self.cleaner
+00000260: 203d 2072 652e 636f 6d70 696c 6528 7222   = re.compile(r"
+00000270: 3c5b 5e3c 3e5d 2b3e 2229 0a0a 2020 2020  <[^<>]+>")..    
+00000280: 6465 6620 646f 6373 2873 656c 663a 2022  def docs(self: "
+00000290: 544e 6577 7352 6561 6465 7222 2920 2d3e  TNewsReader") ->
+000002a0: 2049 7465 7261 746f 725b 4469 6374 5b73   Iterator[Dict[s
+000002b0: 7472 2c20 7374 725d 5d3a 0a20 2020 2020  tr, str]]:.     
+000002c0: 2020 2022 2222 d8ae d8a8 d8b1 d987 d8a7     """..........
+000002d0: 20d8 b1d8 a720 d8af d8b1 20d9 82d8 a7d9   .... .... .....
+000002e0: 84d8 a820 db8c daa9 2060 6974 6572 6174  ... .... `iterat
+000002f0: 6f72 6020 d8a8 d8b1 d985 db8c e280 8cda  or` ............
+00000300: afd8 b1d8 afd8 a7d9 86d8 af2e 0a0a 2020  ..............  
+00000310: 2020 2020 2020 d987 d8b1 20d8 aed8 a8d8        .... .....
+00000320: b1d8 8c20 d8b4 db8c e280 8cd8 a7db 8c20  ... ........... 
+00000330: d985 d8aa d8b4 daa9 d984 20d8 a7d8 b220  .......... .... 
+00000340: da86 d986 d8af 20d9 bed8 a7d8 b1d8 a7d9  ...... .........
+00000350: 85d8 aad8 b120 d8a7 d8b3 d8aa 3a0a 0a20  ..... ......:.. 
+00000360: 2020 2020 2020 202d 20d8 b4d9 86d8 a7d8         - .......
+00000370: b3d9 8720 2869 6429 d88c 0a20 2020 2020  ... (id)...     
+00000380: 2020 202d 20d8 b9d9 86d9 88d8 a7d9 8620     - .......... 
+00000390: 2874 6974 6c65 29d8 8c0a 2020 2020 2020  (title)...      
+000003a0: 2020 2d20 d9be db8c d8b4 20d8 a7d8 b220    - ...... .... 
+000003b0: d8b9 d986 d988 d8a7 d986 2028 7072 652d  .......... (pre-
+000003c0: 7469 746c 6529 d88c 0a20 2020 2020 2020  title)...       
+000003d0: 202d 20d9 bed8 b320 d8a7 d8b2 20d8 b9d9   - .... .... ...
+000003e0: 86d9 88d8 a7d9 8620 2870 6f73 742d 7469  ....... (post-ti
+000003f0: 746c 6529 d88c 0a20 2020 2020 2020 202d  tle)...        -
+00000400: 20d9 85d8 aad9 8620 2874 6578 7429 d88c   ...... (text)..
+00000410: 0a20 2020 2020 2020 202d 20d8 aed9 84d8  .        - .....
+00000420: a7d8 b5d9 8720 2862 7269 6566 29d8 8c0a  ..... (brief)...
+00000430: 2020 2020 2020 2020 2d20 d8a2 d8af d8b1          - ......
+00000440: d8b3 2028 7572 6c29 d88c 0a20 2020 2020  .. (url)...     
+00000450: 2020 202d 20d9 85d9 88d8 b6d9 88d8 b920     - .......... 
+00000460: 2863 6174 6567 6f72 7929 d88c 0a20 2020  (category)...   
+00000470: 2020 2020 202d 20d8 aad8 a7d8 b1db 8cd8       - .........
+00000480: ae20 d988 20d8 b2d9 85d8 a7d9 8620 d8a7  . .. ........ ..
+00000490: d986 d8aa d8b4 d8a7 d8b1 2028 6461 7465  .......... (date
+000004a0: 7469 6d65 292e 0a0a 2020 2020 2020 2020  time)...        
+000004b0: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
+000004c0: 2020 2020 2020 3e3e 3e20 746e 6577 7320        >>> tnews 
+000004d0: 3d20 544e 6577 7352 6561 6465 7228 726f  = TNewsReader(ro
+000004e0: 6f74 3d27 746e 6577 7327 290a 2020 2020  ot='tnews').    
+000004f0: 2020 2020 2020 2020 3e3e 3e20 6e65 7874          >>> next
+00000500: 2874 6e65 7773 2e64 6f63 7328 2929 5b27  (tnews.docs())['
+00000510: 6964 275d 0a20 2020 2020 2020 2020 2020  id'].           
+00000520: 2027 3134 3039 3233 3033 3438 3233 3030   '14092303482300
+00000530: 3031 3336 3533 270a 0a20 2020 2020 2020  013653'..       
+00000540: 2059 6965 6c64 733a 0a20 2020 2020 2020   Yields:.       
+00000550: 2020 2020 2028 4469 6374 293a 20d8 aed8       (Dict): ...
+00000560: a8d8 b120 d8a8 d8b9 d8af db8c 2e0a 0a20  ... ........... 
+00000570: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00000580: 2020 2020 6465 6620 6765 745f 7465 7874      def get_text
+00000590: 2865 6c65 6d65 6e74 3a20 7374 7229 202d  (element: str) -
+000005a0: 3e20 7374 723a 0a20 2020 2020 2020 2020  > str:.         
+000005b0: 2020 2072 6177 5f68 746d 6c20 3d20 656c     raw_html = el
+000005c0: 656d 656e 742e 6368 696c 644e 6f64 6573  ement.childNodes
+000005d0: 5b30 5d2e 6461 7461 2069 6620 656c 656d  [0].data if elem
+000005e0: 656e 742e 6368 696c 644e 6f64 6573 2065  ent.childNodes e
+000005f0: 6c73 6520 2222 0a20 2020 2020 2020 2020  lse "".         
+00000600: 2020 2072 6574 7572 6e20 7265 2e73 7562     return re.sub
+00000610: 2873 656c 662e 636c 6561 6e65 722c 2022  (self.cleaner, "
+00000620: 222c 2072 6177 5f68 746d 6c29 0a0a 2020  ", raw_html)..  
+00000630: 2020 2020 2020 666f 7220 726f 6f74 2c20        for root, 
+00000640: 5f64 6972 732c 2066 696c 6573 2069 6e20  _dirs, files in 
+00000650: 6f73 2e77 616c 6b28 7365 6c66 2e5f 726f  os.walk(self._ro
+00000660: 6f74 293a 0a20 2020 2020 2020 2020 2020  ot):.           
+00000670: 2066 6f72 206e 616d 6520 696e 2073 6f72   for name in sor
+00000680: 7465 6428 6669 6c65 7329 3a0a 2020 2020  ted(files):.    
+00000690: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+000006a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000006b0: 2020 2020 2070 6174 6820 3d20 5061 7468       path = Path
+000006c0: 2872 6f6f 7429 202f 206e 616d 650a 2020  (root) / name.  
+000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006e0: 2020 636f 6e74 656e 7420 3d20 7061 7468    content = path
+000006f0: 2e72 6561 645f 7465 7874 2865 6e63 6f64  .read_text(encod
+00000700: 696e 673d 2275 7466 3822 290a 0a20 2020  ing="utf8")..   
 00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 2020 636f 6e74 656e 7420 3d20 7061      content = pa
-00000730: 7468 2e72 6561 645f 7465 7874 2865 6e63  th.read_text(enc
-00000740: 6f64 696e 673d 2275 7466 3822 290d 0a0d  oding="utf8")...
-00000750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000760: 2020 2020 2023 2066 6978 2078 6d6c 2066       # fix xml f
-00000770: 6f72 6d61 7469 6e67 2069 7373 7565 0d0a  ormating issue..
+00000720: 2023 2066 6978 2078 6d6c 2066 6f72 6d61   # fix xml forma
+00000730: 7469 6e67 2069 7373 7565 0a20 2020 2020  ting issue.     
+00000740: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00000750: 6f6e 7465 6e74 203d 2028 0a20 2020 2020  ontent = (.     
+00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000770: 2020 2072 652e 7375 6228 0a20 2020 2020     re.sub(.     
 00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 2020 2020 636f 6e74 656e 7420 3d20 280d      content = (.
-000007a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007b0: 2020 2020 2020 2020 2072 652e 7375 6228           re.sub(
-000007c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000007d0: 2020 2020 2020 2020 2020 2020 2020 7222                r"
-000007e0: 5b5c 7831 425c 620b 0f01 1112 145c 7831  [\x1B\b......\x1
-000007f0: 4116 071f 0e10 0615 1d18 0c1e 0302 0405  A...............
-00000800: 5d22 2c0d 0a20 2020 2020 2020 2020 2020  ]",..           
-00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 2022 222c 0d0a 2020 2020 2020 2020 2020   "",..          
+00000790: 2020 2020 2020 2072 225b 5c78 3142 5c62         r"[\x1B\b
+000007a0: 0b0f 0111 1214 5c78 3141 1607 1f0e 1006  ......\x1A......
+000007b0: 151d 180c 1e03 0204 055d 222c 0a20 2020  .........]",.   
+000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007d0: 2020 2020 2020 2020 2022 222c 0a20 2020           "",.   
+000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007f0: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
+00000800: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000810: 2020 2020 2020 2020 2020 292e 7265 706c            ).repl
+00000820: 6163 6528 0a20 2020 2020 2020 2020 2020  ace(.           
 00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000840: 2020 636f 6e74 656e 742c 0d0a 2020 2020    content,..    
+00000840: 2022 3c2f 544e 6577 733e 222c 0a20 2020   "</TNews>",.   
 00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 2020 2020 292e 7265 706c 6163 6528 0d0a      ).replace(..
+00000860: 2020 2020 2020 2020 2022 222c 0a20 2020           "",.   
 00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000880: 2020 2020 2020 2020 2020 2020 223c 2f54              "</T
-00000890: 4e65 7773 3e22 2c0d 0a20 2020 2020 2020  News>",..       
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 2020 2020 2022 222c 0d0a 2020 2020 2020       "",..      
-000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008d0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-000008e0: 2020 2020 2020 2020 2020 2020 202b 2022               + "
-000008f0: 3c2f 544e 6577 733e 220d 0a20 2020 2020  </TNews>"..     
-00000900: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00000910: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00000920: 2020 2020 2020 2020 656c 656d 656e 7473          elements
-00000930: 203d 206d 696e 6964 6f6d 2e70 6172 7365   = minidom.parse
-00000940: 5374 7269 6e67 2863 6f6e 7465 6e74 290d  String(content).
-00000950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000960: 2020 2020 2066 6f72 2065 6c65 6d65 6e74       for element
-00000970: 2069 6e20 656c 656d 656e 7473 2e67 6574   in elements.get
-00000980: 456c 656d 656e 7473 4279 5461 674e 616d  ElementsByTagNam
-00000990: 6528 224e 4557 5322 293a 0d0a 2020 2020  e("NEWS"):..    
-000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009b0: 2020 2020 646f 6320 3d20 7b7d 0d0a 2020      doc = {}..  
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2020 2020 2020 646f 635b 2269 6422 5d20        doc["id"] 
-000009e0: 3d20 6765 745f 7465 7874 2865 6c65 6d65  = get_text(eleme
-000009f0: 6e74 2e67 6574 456c 656d 656e 7473 4279  nt.getElementsBy
-00000a00: 5461 674e 616d 6528 224e 4557 5349 4422  TagName("NEWSID"
-00000a10: 295b 305d 290d 0a20 2020 2020 2020 2020  )[0])..         
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00000a30: 6f63 5b22 7572 6c22 5d20 3d20 6765 745f  oc["url"] = get_
-00000a40: 7465 7874 2865 6c65 6d65 6e74 2e67 6574  text(element.get
-00000a50: 456c 656d 656e 7473 4279 5461 674e 616d  ElementsByTagNam
-00000a60: 6528 2255 524c 2229 5b30 5d29 0d0a 2020  e("URL")[0])..  
-00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a80: 2020 2020 2020 646f 635b 2264 6174 6574        doc["datet
-00000a90: 696d 6522 5d20 3d20 6765 745f 7465 7874  ime"] = get_text
-00000aa0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00000ac0: 6c65 6d65 6e74 2e67 6574 456c 656d 656e  lement.getElemen
-00000ad0: 7473 4279 5461 674e 616d 6528 2255 5443  tsByTagName("UTC
-00000ae0: 4441 5445 2229 5b30 5d2c 0d0a 2020 2020  DATE")[0],..    
-00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b00: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00000b10: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00000b20: 6f63 5b22 6361 7465 676f 7279 225d 203d  oc["category"] =
-00000b30: 2067 6574 5f74 6578 7428 0d0a 2020 2020   get_text(..    
-00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b50: 2020 2020 2020 2020 656c 656d 656e 742e          element.
-00000b60: 6765 7445 6c65 6d65 6e74 7342 7954 6167  getElementsByTag
-00000b70: 4e61 6d65 2822 4341 5445 474f 5259 2229  Name("CATEGORY")
-00000b80: 5b30 5d2c 0d0a 2020 2020 2020 2020 2020  [0],..          
-00000b90: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00000ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000bb0: 2020 2020 2020 2020 2064 6f63 5b22 7072           doc["pr
-00000bc0: 652d 7469 746c 6522 5d20 3d20 6765 745f  e-title"] = get_
-00000bd0: 7465 7874 280d 0a20 2020 2020 2020 2020  text(..         
+00000880: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00000890: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+000008a0: 2022 3c2f 544e 6577 733e 220a 2020 2020   "</TNews>".    
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008c0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+000008d0: 2020 2020 2020 2065 6c65 6d65 6e74 7320         elements 
+000008e0: 3d20 6d69 6e69 646f 6d2e 7061 7273 6553  = minidom.parseS
+000008f0: 7472 696e 6728 636f 6e74 656e 7429 0a20  tring(content). 
+00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000910: 2020 2066 6f72 2065 6c65 6d65 6e74 2069     for element i
+00000920: 6e20 656c 656d 656e 7473 2e67 6574 456c  n elements.getEl
+00000930: 656d 656e 7473 4279 5461 674e 616d 6528  ementsByTagName(
+00000940: 224e 4557 5322 293a 0a20 2020 2020 2020  "NEWS"):.       
+00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000960: 2064 6f63 203d 207b 7d0a 2020 2020 2020   doc = {}.      
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 2020 646f 635b 2269 6422 5d20 3d20 6765    doc["id"] = ge
+00000990: 745f 7465 7874 2865 6c65 6d65 6e74 2e67  t_text(element.g
+000009a0: 6574 456c 656d 656e 7473 4279 5461 674e  etElementsByTagN
+000009b0: 616d 6528 224e 4557 5349 4422 295b 305d  ame("NEWSID")[0]
+000009c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000009d0: 2020 2020 2020 2020 2020 646f 635b 2275            doc["u
+000009e0: 726c 225d 203d 2067 6574 5f74 6578 7428  rl"] = get_text(
+000009f0: 656c 656d 656e 742e 6765 7445 6c65 6d65  element.getEleme
+00000a00: 6e74 7342 7954 6167 4e61 6d65 2822 5552  ntsByTagName("UR
+00000a10: 4c22 295b 305d 290a 2020 2020 2020 2020  L")[0]).        
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a30: 646f 635b 2264 6174 6574 696d 6522 5d20  doc["datetime"] 
+00000a40: 3d20 6765 745f 7465 7874 280a 2020 2020  = get_text(.    
+00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a60: 2020 2020 2020 2020 656c 656d 656e 742e          element.
+00000a70: 6765 7445 6c65 6d65 6e74 7342 7954 6167  getElementsByTag
+00000a80: 4e61 6d65 2822 5554 4344 4154 4522 295b  Name("UTCDATE")[
+00000a90: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+00000aa0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00000ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ac0: 2020 2020 2020 646f 635b 2263 6174 6567        doc["categ
+00000ad0: 6f72 7922 5d20 3d20 6765 745f 7465 7874  ory"] = get_text
+00000ae0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00000af0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00000b00: 656d 656e 742e 6765 7445 6c65 6d65 6e74  ement.getElement
+00000b10: 7342 7954 6167 4e61 6d65 2822 4341 5445  sByTagName("CATE
+00000b20: 474f 5259 2229 5b30 5d2c 0a20 2020 2020  GORY")[0],.     
+00000b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b40: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00000b50: 2020 2020 2020 2020 2020 2020 2064 6f63               doc
+00000b60: 5b22 7072 652d 7469 746c 6522 5d20 3d20  ["pre-title"] = 
+00000b70: 6765 745f 7465 7874 280a 2020 2020 2020  get_text(.      
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 2020 2020 2020 656c 656d 656e 742e 6765        element.ge
+00000ba0: 7445 6c65 6d65 6e74 7342 7954 6167 4e61  tElementsByTagNa
+00000bb0: 6d65 2822 5052 4554 4954 4c45 2229 5b30  me("PRETITLE")[0
+00000bc0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00000bd0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
 00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bf0: 2020 2065 6c65 6d65 6e74 2e67 6574 456c     element.getEl
-00000c00: 656d 656e 7473 4279 5461 674e 616d 6528  ementsByTagName(
-00000c10: 2250 5245 5449 544c 4522 295b 305d 2c0d  "PRETITLE")[0],.
-00000c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c30: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c50: 2020 2020 646f 635b 2274 6974 6c65 225d      doc["title"]
-00000c60: 203d 2067 6574 5f74 6578 7428 0d0a 2020   = get_text(..  
+00000bf0: 2020 2020 2064 6f63 5b22 7469 746c 6522       doc["title"
+00000c00: 5d20 3d20 6765 745f 7465 7874 280a 2020  ] = get_text(.  
+00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c20: 2020 2020 2020 2020 2020 656c 656d 656e            elemen
+00000c30: 742e 6765 7445 6c65 6d65 6e74 7342 7954  t.getElementsByT
+00000c40: 6167 4e61 6d65 2822 5449 544c 4522 295b  agName("TITLE")[
+00000c50: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+00000c60: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
 00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2020 2020 2020 2020 2020 656c 656d 656e            elemen
-00000c90: 742e 6765 7445 6c65 6d65 6e74 7342 7954  t.getElementsByT
-00000ca0: 6167 4e61 6d65 2822 5449 544c 4522 295b  agName("TITLE")[
-00000cb0: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
-00000cc0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 2020 2020 2020 2020 646f 635b 2270 6f73          doc["pos
-00000cf0: 742d 7469 746c 6522 5d20 3d20 6765 745f  t-title"] = get_
-00000d00: 7465 7874 280d 0a20 2020 2020 2020 2020  text(..         
+00000c80: 2020 2020 2020 646f 635b 2270 6f73 742d        doc["post-
+00000c90: 7469 746c 6522 5d20 3d20 6765 745f 7465  title"] = get_te
+00000ca0: 7874 280a 2020 2020 2020 2020 2020 2020  xt(.            
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 656c 656d 656e 742e 6765 7445 6c65 6d65  element.getEleme
+00000cd0: 6e74 7342 7954 6167 4e61 6d65 2822 504f  ntsByTagName("PO
+00000ce0: 5354 5449 544c 4522 295b 305d 2c0a 2020  STTITLE")[0],.  
+00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
 00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d20: 2020 2065 6c65 6d65 6e74 2e67 6574 456c     element.getEl
-00000d30: 656d 656e 7473 4279 5461 674e 616d 6528  ementsByTagName(
-00000d40: 2250 4f53 5454 4954 4c45 2229 5b30 5d2c  "POSTTITLE")[0],
-00000d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000d60: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2020 2064 6f63 5b22 6272 6965 6622       doc["brief"
-00000d90: 5d20 3d20 6765 745f 7465 7874 280d 0a20  ] = get_text(.. 
+00000d20: 646f 635b 2262 7269 6566 225d 203d 2067  doc["brief"] = g
+00000d30: 6574 5f74 6578 7428 0a20 2020 2020 2020  et_text(.       
+00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d50: 2020 2020 2065 6c65 6d65 6e74 2e67 6574       element.get
+00000d60: 456c 656d 656e 7473 4279 5461 674e 616d  ElementsByTagNam
+00000d70: 6528 2242 5249 4546 2229 5b30 5d2c 0a20  e("BRIEF")[0],. 
+00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d90: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
 00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000db0: 2020 2020 2020 2020 2020 2065 6c65 6d65             eleme
-00000dc0: 6e74 2e67 6574 456c 656d 656e 7473 4279  nt.getElementsBy
-00000dd0: 5461 674e 616d 6528 2242 5249 4546 2229  TagName("BRIEF")
-00000de0: 5b30 5d2c 0d0a 2020 2020 2020 2020 2020  [0],..          
-00000df0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00000e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e10: 2020 2020 2020 2020 2064 6f63 5b22 7465           doc["te
-00000e20: 7874 225d 203d 2067 6574 5f74 6578 7428  xt"] = get_text(
-00000e30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000e40: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00000e50: 656d 656e 742e 6765 7445 6c65 6d65 6e74  ement.getElement
-00000e60: 7342 7954 6167 4e61 6d65 2822 4445 5343  sByTagName("DESC
-00000e70: 5249 5054 494f 4e22 295b 305d 2c0d 0a20  RIPTION")[0],.. 
-00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e90: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 2020 7969 656c 6420 646f 630d 0a0d 0a20    yield doc.... 
-00000ec0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00000ed0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00000ee0: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
-00000ef0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00000f00: 2822 6572 726f 7220 696e 2072 6561 6469  ("error in readi
-00000f10: 6e67 222c 206e 616d 652c 2065 2c20 6669  ng", name, e, fi
-00000f20: 6c65 3d73 7973 2e73 7464 6572 7229 0d0a  le=sys.stderr)..
-00000f30: 0d0a 2020 2020 6465 6620 7465 7874 7328  ..    def texts(
-00000f40: 7365 6c66 3a20 2254 4e65 7773 5265 6164  self: "TNewsRead
-00000f50: 6572 2229 202d 3e20 4974 6572 6174 6f72  er") -> Iterator
-00000f60: 5b73 7472 5d3a 0d0a 2020 2020 2020 2020  [str]:..        
-00000f70: 2222 22d9 81d9 82d8 b720 d985 d8aa d986  """...... ......
-00000f80: 20d8 aed8 a8d8 b1d9 87d8 a720 d8b1 d8a7   .......... ....
-00000f90: 20d8 a8d8 b1d9 85db 8ce2 808c daaf d8b1   ...............
-00000fa0: d8af d8a7 d986 d8af 2e0d 0a0d 0a20 2020  .............   
-00000fb0: 2020 2020 20d8 a7db 8cd9 8620 d8aa d8a7       ...... ....
-00000fc0: d8a8 d8b9 20d8 b5d8 b1d9 81d8 a7d9 8b20  .... .......... 
-00000fd0: d8a8 d8b1 d8a7 db8c 20d8 b1d8 a7d8 add8  ........ .......
-00000fe0: aadb 8c20 d8a8 db8c d8b4 d8aa d8b1 20d8  ... .......... .
-00000ff0: aad9 87db 8cd9 8720 d8b4 d8af d987 20d9  ....... ...... .
-00001000: 88da afd8 b1d9 86d9 8720 d8a8 d8a7 20d9  ......... .... .
-00001010: 87d9 85d8 a7d9 8620 d8aa d8a7 d8a8 d8b9  ....... ........
-00001020: 0d0a 2020 2020 2020 2020 e280 8d5b 646f  ..        ...[do
-00001030: 6373 2829 5d5b 6861 7a6d 2e63 6f72 7075  cs()][hazm.corpu
-00001040: 735f 7265 6164 6572 732e 746e 6577 735f  s_readers.tnews_
-00001050: 7265 6164 6572 2e54 4e65 7773 5265 6164  reader.TNewsRead
-00001060: 6572 2e64 6f63 735d 20d9 8820 d8af d8b1  er.docs] .. ....
-00001070: db8c d8a7 d981 d8aa 20d9 85d9 82d8 afd8  ........ .......
-00001080: a7d8 b120 d9be d8b1 d8a7 d9be d8b1 d8aa  ... ............
-00001090: db8c 0d0a 2020 2020 2020 2020 6074 6578  ....        `tex
-000010a0: 7460 20d9 86db 8cd8 b220 d985 db8c e280  t` ...... ......
-000010b0: 8cd8 aad9 88d8 a7d9 86db 8cd8 af20 d987  ............. ..
-000010c0: d985 db8c d986 20da a9d8 a7d8 b120 d8b1  ...... ...... ..
-000010d0: d8a7 20d8 a7d9 86d8 acd8 a7d9 8520 d8af  .. .......... ..
-000010e0: d987 db8c d8af 2e0d 0a0d 0a20 2020 2020  ...........     
-000010f0: 2020 2045 7861 6d70 6c65 733a 0d0a 2020     Examples:..  
-00001100: 2020 2020 2020 2020 2020 3e3e 3e20 746e            >>> tn
-00001110: 6577 7320 3d20 544e 6577 7352 6561 6465  ews = TNewsReade
-00001120: 7228 726f 6f74 3d27 636f 7270 6f72 612f  r(root='corpora/
-00001130: 746e 6577 7327 290d 0a20 2020 2020 2020  tnews')..       
-00001140: 2020 2020 203e 3e3e 206e 6578 7428 746e       >>> next(tn
-00001150: 6577 732e 7465 7874 7328 2929 2e73 7461  ews.texts()).sta
-00001160: 7274 7377 6974 6828 27d8 a8d9 8720 daaf  rtswith('.... ..
-00001170: d8b2 d8a7 d8b1 d8b4 20e2 809d 2020 d8b4  ........ ...  ..
-00001180: d8a8 daa9 d987 20d8 a7d8 b7d9 84d8 a7d8  ...... .........
-00001190: b920 d8b1 d8b3 d8a7 d986 db8c 20d8 a7db  . .......... ...
-000011a0: 8cd9 86d8 aad8 b1d9 86d8 aadb 8c20 d8a8  ............. ..
-000011b0: d988 d8aa db8c d8a7 2020 e280 9d20 d8a8  ........  ... ..
-000011c0: d987 20d9 86d9 82d9 8420 d8a7 d8b2 20d8  .. ...... .... .
-000011d0: a7d8 b1da af20 d986 db8c d988 d8b2 2729  ..... ........')
-000011e0: 0d0a 2020 2020 2020 2020 2020 2020 5472  ..            Tr
-000011f0: 7565 0d0a 0d0a 2020 2020 2020 2020 5969  ue....        Yi
-00001200: 656c 6473 3a0d 0a20 2020 2020 2020 2020  elds:..         
-00001210: 2020 20d9 85d8 aad9 8620 d8ae d8a8 d8b1     ...... ......
-00001220: 20d8 a8d8 b9d8 afdb 8c2e 0d0a 0d0a 2020   .............  
-00001230: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00001240: 2020 2066 6f72 2064 6f63 2069 6e20 7365     for doc in se
-00001250: 6c66 2e64 6f63 7328 293a 0d0a 2020 2020  lf.docs():..    
-00001260: 2020 2020 2020 2020 7969 656c 6420 646f          yield do
-00001270: 635b 2274 6578 7422 5d0d 0a              c["text"]..
+00000db0: 2064 6f63 5b22 7465 7874 225d 203d 2067   doc["text"] = g
+00000dc0: 6574 5f74 6578 7428 0a20 2020 2020 2020  et_text(.       
+00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000de0: 2020 2020 2065 6c65 6d65 6e74 2e67 6574       element.get
+00000df0: 456c 656d 656e 7473 4279 5461 674e 616d  ElementsByTagNam
+00000e00: 6528 2244 4553 4352 4950 5449 4f4e 2229  e("DESCRIPTION")
+00000e10: 5b30 5d2c 0a20 2020 2020 2020 2020 2020  [0],.           
+00000e20: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e40: 2020 2020 2020 2079 6965 6c64 2064 6f63         yield doc
+00000e50: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000e60: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00000e70: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
+00000e80: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00000e90: 6e74 2822 6572 726f 7220 696e 2072 6561  nt("error in rea
+00000ea0: 6469 6e67 222c 206e 616d 652c 2065 2c20  ding", name, e, 
+00000eb0: 6669 6c65 3d73 7973 2e73 7464 6572 7229  file=sys.stderr)
+00000ec0: 0a0a 2020 2020 6465 6620 7465 7874 7328  ..    def texts(
+00000ed0: 7365 6c66 3a20 2254 4e65 7773 5265 6164  self: "TNewsRead
+00000ee0: 6572 2229 202d 3e20 4974 6572 6174 6f72  er") -> Iterator
+00000ef0: 5b73 7472 5d3a 0a20 2020 2020 2020 2022  [str]:.        "
+00000f00: 2222 d981 d982 d8b7 20d9 85d8 aad9 8620  ""...... ...... 
+00000f10: d8ae d8a8 d8b1 d987 d8a7 20d8 b1d8 a720  .......... .... 
+00000f20: d8a8 d8b1 d985 db8c e280 8cda afd8 b1d8  ................
+00000f30: afd8 a7d9 86d8 af2e 0a0a 2020 2020 2020  ..........      
+00000f40: 2020 d8a7 db8c d986 20d8 aad8 a7d8 a8d8    ...... .......
+00000f50: b920 d8b5 d8b1 d981 d8a7 d98b 20d8 a8d8  . .......... ...
+00000f60: b1d8 a7db 8c20 d8b1 d8a7 d8ad d8aa db8c  ..... ..........
+00000f70: 20d8 a8db 8cd8 b4d8 aad8 b120 d8aa d987   .......... ....
+00000f80: db8c d987 20d8 b4d8 afd9 8720 d988 daaf  .... ...... ....
+00000f90: d8b1 d986 d987 20d8 a8d8 a720 d987 d985  ...... .... ....
+00000fa0: d8a7 d986 20d8 aad8 a7d8 a8d8 b90a 2020  .... .........  
+00000fb0: 2020 2020 2020 e280 8d5b 646f 6373 2829        ...[docs()
+00000fc0: 5d5b 6861 7a6d 2e63 6f72 7075 735f 7265  ][hazm.corpus_re
+00000fd0: 6164 6572 732e 746e 6577 735f 7265 6164  aders.tnews_read
+00000fe0: 6572 2e54 4e65 7773 5265 6164 6572 2e64  er.TNewsReader.d
+00000ff0: 6f63 735d 20d9 8820 d8af d8b1 db8c d8a7  ocs] .. ........
+00001000: d981 d8aa 20d9 85d9 82d8 afd8 a7d8 b120  .... .......... 
+00001010: d9be d8b1 d8a7 d9be d8b1 d8aa db8c 0a20  ............... 
+00001020: 2020 2020 2020 2060 7465 7874 6020 d986         `text` ..
+00001030: db8c d8b2 20d9 85db 8ce2 808c d8aa d988  .... ...........
+00001040: d8a7 d986 db8c d8af 20d9 87d9 85db 8cd9  ........ .......
+00001050: 8620 daa9 d8a7 d8b1 20d8 b1d8 a720 d8a7  . ...... .... ..
+00001060: d986 d8ac d8a7 d985 20d8 afd9 87db 8cd8  ........ .......
+00001070: af2e 0a0a 2020 2020 2020 2020 4578 616d  ....        Exam
+00001080: 706c 6573 3a0a 2020 2020 2020 2020 2020  ples:.          
+00001090: 2020 3e3e 3e20 746e 6577 7320 3d20 544e    >>> tnews = TN
+000010a0: 6577 7352 6561 6465 7228 726f 6f74 3d27  ewsReader(root='
+000010b0: 746e 6577 7327 290a 2020 2020 2020 2020  tnews').        
+000010c0: 2020 2020 3e3e 3e20 6e65 7874 2874 6e65      >>> next(tne
+000010d0: 7773 2e74 6578 7473 2829 292e 7374 6172  ws.texts()).star
+000010e0: 7473 7769 7468 2827 d8a8 d987 20da afd8  tswith('.... ...
+000010f0: b2d8 a7d8 b1d8 b420 e280 9d20 20d8 b4d8  ....... ...  ...
+00001100: a8da a9d9 8720 d8a7 d8b7 d984 d8a7 d8b9  ..... ..........
+00001110: 20d8 b1d8 b3d8 a7d9 86db 8c20 d8a7 db8c   .......... ....
+00001120: d986 d8aa d8b1 d986 d8aa db8c 20d8 a8d9  ............ ...
+00001130: 88d8 aadb 8cd8 a720 20e2 809d 20d8 a8d9  .......  ... ...
+00001140: 8720 d986 d982 d984 20d8 a7d8 b220 d8a7  . ...... .... ..
+00001150: d8b1 daaf 20d9 86db 8cd9 88d8 b227 290a  .... ........').
+00001160: 2020 2020 2020 2020 2020 2020 5472 7565              True
+00001170: 0a0a 2020 2020 2020 2020 5969 656c 6473  ..        Yields
+00001180: 3a0a 2020 2020 2020 2020 2020 2020 d985  :.            ..
+00001190: d8aa d986 20d8 aed8 a8d8 b120 d8a8 d8b9  .... ...... ....
+000011a0: d8af db8c 2e0a 0a20 2020 2020 2020 2022  .......        "
+000011b0: 2222 0a20 2020 2020 2020 2066 6f72 2064  "".        for d
+000011c0: 6f63 2069 6e20 7365 6c66 2e64 6f63 7328  oc in self.docs(
+000011d0: 293a 0a20 2020 2020 2020 2020 2020 2079  ):.            y
+000011e0: 6965 6c64 2064 6f63 5b22 7465 7874 225d  ield doc["text"]
+000011f0: 0a                                       .
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/treebank_reader.py` & `hazm-0.9.2/hazm/corpus_readers/treebank_reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,410 +1,423 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ تری‌بانک است.
-
-پیکرهٔ تری‌بانک حاوی هزاران جملهٔ برچسب‌خورده با اطلاعات نحوی و ساخت‌واژی است.
-
-"""
-
-
-import os
-import re
-import sys
-from pathlib import Path
-from typing import Any
-from typing import Dict
-from typing import Iterator
-from typing import List
-from typing import Tuple
-from xml.dom import minidom
-
-from nltk.tree import Tree
-
-from ..word_tokenizer import WordTokenizer
-
-
-def coarse_pos_e(tags: List[str]) -> List[str]:
-    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
-
-    Examples:
-        >>> coarse_pos_e(['Nasp---', 'pers', 'prop'])
-        'N'
-
-    Args:
-        tags: لیست برچسب‌های ریز.
-
-    Returns:
-        لیست برچسب‌های درشت.
-
-    """
-    mapping = {
-        "N": "N",
-        "V": "V",
-        "A": "AJ",
-        "D": "ADV",
-        "Z": "PRO",
-        "T": "DET",
-        "E": "P",
-        "P": "POSTP",
-        "U": "NUM",
-        "J": "CONJ",
-        "O": "PUNC",
-        "R": "RES",
-        "L": "CL",
-        "I": "INT",
-    }
-    try:
-        if tags[0][0] == "C":
-            if "pronominal" in tags:
-                tags[0] = "Z"
-            elif "verb" in tags:
-                tags[0] = "V"
-            elif "prep" in tags:
-                tags[0] = "E"
-            elif "adv" in tags:
-                tags[0] = "D"
-            elif "det" in tags:
-                tags[0] = "T"
-        return mapping[tags[0][0]] + ("e" if "ezafe" in tags else "")
-    except Exception:
-        return ""
-
-
-class TreebankReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ تری‌بانک است.
-
-    Args:
-        root: مسیر فولدر حاوی فایل‌های پیکره
-        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
-        join_clitics: اگر `True‍` باشد واژه‌بست‌ها را به کلمهٔ مادر می‌چسباند.
-        join_verb_parts: اگر `True` باشد افعال چندبخشی را با _ به هم می‌چسباند.
-
-    """
-
-    def __init__(
-        self: "TreebankReader",
-        root: str,
-        pos_map: str = coarse_pos_e,
-        join_clitics: bool = False,
-        join_verb_parts: bool = False,
-    ) -> None:
-        self._root = root
-        self._pos_map = pos_map if pos_map else lambda tags: ",".join(tags)
-        self._join_clitics = join_clitics
-        self._join_verb_parts = join_verb_parts
-        self._tokenizer = WordTokenizer()
-
-    def docs(self: "TreebankReader") -> Iterator[Any]:
-        """اسناد موجود در پیکره را برمی‌گرداند.
-
-        Yields:
-            سند بعدی.
-
-        """
-        for root, _dirs, files in os.walk(self._root):
-            for name in sorted(files):
-                try:
-                    with Path.open(
-                        Path(root) / name,
-                        encoding="utf8",
-                    ) as treebank_file:
-                        raw = re.sub(r"\n *", "", treebank_file.read())
-                        yield minidom.parseString(raw.encode("utf8"))
-                except Exception as e:
-                    print("error in reading", name, e, file=sys.stderr)
-
-    def trees(self: "TreebankReader") -> Iterator[str]:
-        """ساختارهای درختی موجود در پیکره را برمی‌گرداند.
-
-        Examples:
-            >>> treebank = TreebankReader(root='corpora/treebank')
-            >>> print(next(treebank.trees()))
-            (S
-            (VPS
-                    (NPC (N دنیای/Ne) (MN (N آدولف/N) (N بورن/N)))
-                    (VPC
-                    (NPC (N دنیای/Ne) (NPA (N اتفاقات/Ne) (ADJ رویایی/AJ)))
-                    (V است/V)))
-            (PUNC ./PUNC))
-
-        Yields:
-            ساختار درختی بعدی.
-
-        """
-
-        def traverse(node: str) -> Tree:
-            def extract_tags(w: str):
-                pos = [w.getAttribute("lc") if w.getAttribute("lc") else None]
-                if w.getAttribute("clitic") in {
-                    "ezafe",
-                    "pronominal",
-                    "verb",
-                    "prep",
-                    "adv",
-                    "det",
-                }:
-                    pos.append(w.getAttribute("clitic"))
-                if w.getAttribute("ne_sort"):
-                    pos.append(w.getAttribute("ne_sort"))
-                if w.getAttribute("n_type"):
-                    pos.append(w.getAttribute("n_type"))
-                if w.getAttribute("ya_type"):
-                    pos.append(w.getAttribute("ya_type"))
-                if w.getAttribute("ke_type"):
-                    pos.append(w.getAttribute("ke_type"))
-                if w.getAttribute("type"):
-                    pos.append(w.getAttribute("type"))
-                if w.getAttribute("kind"):
-                    pos.append(w.getAttribute("kind"))
-                return pos
-
-            def clitic_join(tree: Tree, clitic: Dict):
-                if type(tree[-1]) == Tree:
-                    return clitic_join(tree[-1], clitic)
-
-                if clitic[0][0][0] == "ا":
-                    clitic[0] = ("‌" + clitic[0][0], clitic[0][1])
-                tree[-1] = (tree[-1][0] + clitic[0][0], clitic[0][1])
-                tree.set_label("CLITICS")
-                return None
-
-            if not len(node.childNodes):
-                return None
-            first = node.childNodes[0]
-
-            if first.nodeName == "w":
-                pos = extract_tags(first)
-                return Tree(
-                    node.nodeName,
-                    [
-                        (self._pos_map(pos),),
-                    ],
-                )
-            childs = node.childNodes[2:] if node.tagName == "S" else node.childNodes
-            for child in childs:
-                if not len(child.childNodes):
-                    childs.remove(child)
-            tree = Tree(node.tagName, list(map(traverse, childs)))
-            if (
-                self._join_clitics
-                and len(tree) > 1
-                and type(tree[1]) == Tree
-                and tree[1].label() == "CLITIC"
-                and tree[1][0][1] not in {"P", "V"}
-            ):
-                clitic = tree[-1]
-                tree = Tree(tree.label(), list(tree[0]))
-                clitic_join(tree, clitic)
-            if (
-                self._join_verb_parts
-                and len(tree) > 1
-                and type(tree[1]) == Tree
-                and type(tree[0]) == Tree
-                and tree[0].label() == "AUX"
-                and tree[0][0][0] in self._tokenizer.before_verbs
-            ):
-                tree[1][0] = (tree[0][0][0] + " " + tree[1][0][0], tree[1][0][1])
-                tree.remove(tree[0])
-            if (
-                self._join_verb_parts
-                and len(tree.leaves()) > 1
-                and tree.leaves()[-1][0] in self._tokenizer.after_verbs
-                and tree.leaves()[-2][0] in self._tokenizer.verbe
-            ):
-                tree[1][0] = (
-                    tree[0].leaves()[-1][0] + " " + tree[1][0][0],
-                    tree[1][0][1],
-                )
-                path = tree.leaf_treeposition(len(tree.leaves()) - 2)
-                removingtree = tree
-                while len(path) > 2:
-                    removingtree = removingtree[path[0]]
-                    path = path[1:]
-                removingtree.remove(Tree(tree.pos()[-2][1], [tree.pos()[-2][0]]))
-            if (
-                self._join_verb_parts
-                and len(tree.leaves()) > 1
-                and tree.leaves()[-1][0] in self._tokenizer.after_verbs
-                and tree.leaves()[-2][0] in self._tokenizer.verbe
-            ):
-                tree[1][0] = (
-                    tree[0].leaves()[-1][0] + " " + tree[1][0][0],
-                    tree[1][0][1],
-                )
-                path = tree.leaf_treeposition(len(tree.leaves()) - 2)
-                removingtree = tree
-                while len(path) > 2:
-                    removingtree = removingtree[path[0]]
-                    path = path[1:]
-                removingtree.remove(Tree(tree.pos()[-2][1], [tree.pos()[-2][0]]))
-            return tree
-
-        for doc in self.docs():
-            for s in doc.getElementsByTagName("S"):
-                traverse(s)
-                yield traverse(s)
-
-    def sents(self: "TreebankReader") -> Iterator[List[Tuple[str, str]]]:
-        """جملات را به شکل مجموعه‌ای از `(توکن،برچسب)`ها برمی‌گرداند.
-
-        Examples:
-            >>> treebank = TreebankReader(root='corpora/treebank')
-            >>> next(treebank.sents())
-            [('دنیای', 'Ne'), ('آدولف', 'N'), ('بورن', 'N'), ('دنیای', 'Ne'), ('اتفاقات', 'Ne'), ('رویایی', 'AJ'), ('است', 'V'), ('.', 'PUNC')]
-
-        Yields:
-            جملهٔ بعدی.
-
-        """
-        for tree in self.trees():
-            yield tree.leaves()
-
-    def chunked_trees(self: "TreebankReader") -> Iterator[str]:
-        """ساختار درختی را به شکل تقطیع شده برمی‌گرداند.
-
-        Examples:
-            >>> from .Chunker import tree2brackets
-            >>> treebank = TreebankReader(root='corpora/treebank')
-            >>> tree2brackets(next(treebank.chunked_trees()))
-            '[دنیای آدولف بورن NP] [دنیای اتفاقات رویایی NP] [است VP] .'
-
-        Yields:
-            درخت تقطیع شدهٔ بعدی.
-
-        """
-
-        def collapse(node, label):
-            return Tree(label, [Tree(pos[1], [pos[0]]) for pos in node.pos()])
-
-        def traverse(node, parent, chunks):
-            label = node.label()
-
-            if label.count("-nid") > 0:
-                label = label.replace("-nid", "")
-            if label.count("-nid") > 0:
-                label = label.replace("-nid", "")
-            if label.count("-DiscA") > 0:
-                label = label.replace("-DiscA", "")
-
-            if label in {"CLITIC", "CLITICS"}:
-                if node[0][1] == "V":
-                    label = "V"
-                elif node[0][1] == "P":
-                    label = "PREP"
-                elif node[0][1] == "DET":
-                    label = "DET"
-                elif node[0][1] == "ADV":
-                    label = "ADV"
-                elif node[0][1] == "PRO":
-                    label = "PRON"
-
-            if label in {"CONJ", "PUNC"} and len(node) == 1:
-                chunks.append(node)
-                return
-
-            if label == "PPC" and len(node) == 1:
-                chunks.append(Tree("PP", [node[0]]))
-                return
-
-            if label == "PREP":
-                chunks.append(Tree("PP", [node]))
-                return
-
-            if label == "PostP":
-                chunks.append(Tree("POSTP", [node]))
-                return
-
-            for leaf in node.pos():
-                if leaf[1] in {"PUNC", "CONJ", "PREP", "PostP"}:
-                    for i in range(len(node)):
-                        traverse(node[i], node, chunks)
-                    return
-
-            if label == "NPA" and parent.label() in {"CPC", "PPC"}:
-                chunks.append(collapse(node, "NP"))
-                return
-
-            if label == "NPA" and len(node) >= 1 and node[0].label() == "ADV":
-                chunks.append(collapse(node, "NP"))
-                return
-
-            if label in {
-                "NPC",
-                "N",
-                "INFV",
-                "DPA",
-                "CLASS",
-                "DPC",
-                "DEM",
-                "INTJ",
-                "MN",
-                "PRON",
-                "DET",
-                "NUM",
-                "RES",
-            }:
-                chunks.append(collapse(node, "NP"))
-                return
-
-            if (
-                label == "NPA"
-                and len(node) >= 2
-                and (
-                    node[0].label() == "ADJ"
-                    and node[1].label() == "NPC"
-                    or node[0].label() in {"N", "PRON"}
-                    and node[1].label() in {"ADJ", "ADJPA", "N"}
-                    or node[0].label() == "NUM"
-                    and node[1].label() in {"N", "NPC", "MN", "NUM"}
-                    or node[0].label() in {"N", "NPC", "MN"}
-                    and node[1].label() == "NUM"
-                    or node[0].label() == "NPC"
-                    and node[1].label() == "ADJ"
-                    or node[0].label() == "NPA"
-                    and node[1].label() != "NPC"
-                    or node[1].label() == "NPA"
-                    and node[0].label() != "NPC"
-                )
-            ):
-                chunks.append(collapse(node, "NP"))
-                return
-
-            if label == "DPC" and len(node) >= 2:
-                chunkable = True
-                for leaf in node[1].pos():
-                    if leaf[1] in {"PUNC", "CONJ", "PREP", "PostP"}:
-                        chunkable = False
-                if node[1].label() in {"N", "NPA", "NPC"} and chunkable:
-                    chunks.append(collapse(node, "NP"))
-                    return
-
-            if label == "DPA" and len(node) >= 2 and node[1].label() == "ADV":
-                chunks.append(collapse(node, "ADVP"))
-                return
-
-            if label in {"MV", "V", "AUX", "PPARV"}:
-                chunks.append(Tree("VP", [node]))
-                return
-
-            if label in {"ADJ", "ADJPC", "MADJ", "ADVPA"}:
-                chunks.append(Tree("ADJP", [node]))
-                return
-
-            if label in {"ADV", "MADV", "ADVPC"}:
-                chunks.append(Tree("ADVP", [node]))
-                return
-
-            if type(node[0]) != Tree:
-                chunks.append(node)
-                return
-
-            for i in range(len(node)):
-                traverse(node[i], node, chunks)
-
-        for tree in self.trees():
-            chunks = []
-            traverse(tree, None, chunks)
-            for i in range(len(chunks)):
-                if chunks[i].label() in {"PUNC", "CONJ"}:
-                    chunks[i] = chunks[i][0]
-                else:
-                    chunks[i] = Tree(chunks[i].label(), chunks[i].leaves())
-            yield Tree("S", chunks)
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ تری‌بانک است.
+
+پیکرهٔ تری‌بانک حاوی هزاران جملهٔ برچسب‌خورده با اطلاعات نحوی و ساخت‌واژی است.
+
+"""
+
+
+import os
+import sys
+from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import Iterator
+from typing import List
+from typing import Tuple
+from xml.dom import minidom
+from xml.dom.minidom import Node
+
+from nltk.tree import Tree
+
+from hazm import WordTokenizer
+
+
+def coarse_pos_e(tags: List[str]) -> List[str]:
+    """برچسب‌های ریز را به برچسب‌های درشت (coarse-grained pos tags) تبدیل می‌کند.
+
+    Examples:
+        >>> coarse_pos_e(['Nasp---', 'pers', 'prop'])
+        'N'
+
+    Args:
+        tags: لیست برچسب‌های ریز.
+
+    Returns:
+        لیست برچسب‌های درشت.
+
+    """
+    mapping = {
+        "N": "N",
+        "V": "V",
+        "A": "AJ",
+        "D": "ADV",
+        "Z": "PRO",
+        "T": "DET",
+        "E": "P",
+        "P": "POSTP",
+        "U": "NUM",
+        "J": "CONJ",
+        "O": "PUNC",
+        "R": "RES",
+        "L": "CL",
+        "I": "INT",
+    }
+    try:
+        if tags[0][0] == "C":
+            if "pronominal" in tags:
+                tags[0] = "Z"
+            elif "verb" in tags:
+                tags[0] = "V"
+            elif "prep" in tags:
+                tags[0] = "E"
+            elif "adv" in tags:
+                tags[0] = "D"
+            elif "det" in tags:
+                tags[0] = "T"
+        return mapping[tags[0][0]] + ("e" if "ezafe" in tags else "")
+    except Exception:
+        return ""
+
+
+class TreebankReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ تری‌بانک است.
+
+    Args:
+        root: مسیر فولدر حاوی فایل‌های پیکره
+        pos_map: دیکشنری مبدل برچسب‌های ریز به درشت.
+        join_clitics: اگر `True‍` باشد واژه‌بست‌ها را به کلمهٔ مادر می‌چسباند.
+        join_verb_parts: اگر `True` باشد افعال چندبخشی را با _ به هم می‌چسباند.
+
+    """
+
+    def __init__(
+        self: "TreebankReader",
+        root: str,
+        pos_map: str = coarse_pos_e,
+        join_clitics: bool = False,
+        join_verb_parts: bool = False,
+    ) -> None:
+        self._root = root
+        self._pos_map = pos_map if pos_map else lambda tags: ",".join(tags)
+        self._join_clitics = join_clitics
+        self._join_verb_parts = join_verb_parts
+        self._tokenizer = WordTokenizer()
+
+    def docs(self: "TreebankReader") -> Iterator[Any]:
+        """اسناد موجود در پیکره را برمی‌گرداند.
+
+        Yields:
+            سند بعدی.
+
+        """
+        def remove_blanks(node):
+            for x in node.childNodes:
+                if x.nodeType == Node.TEXT_NODE:
+                    if x.nodeValue:
+                        x.nodeValue = x.nodeValue.strip()
+                elif x.nodeType == Node.ELEMENT_NODE:
+                    remove_blanks(x)
+
+        for root, _dirs, files in os.walk(self._root):
+            for name in sorted(files):
+                try:
+                    with Path.open(
+                        Path(root) / name,
+                        encoding="utf8",
+                    ) as treebank_file:
+                        xml = minidom.parseString(treebank_file.read().encode("utf8"))
+                        remove_blanks(xml)
+                        xml.normalize()
+                        yield xml
+                except Exception as e:
+                    print("error in reading", name, e, file=sys.stderr)
+
+    def trees(self: "TreebankReader") -> Iterator[str]:
+        """ساختارهای درختی موجود در پیکره را برمی‌گرداند.
+
+        Examples:
+            >>> treebank = TreebankReader(root='treebank')
+            >>> print(next(treebank.trees()))
+            (S
+              (VPS
+                (NPC (N دنیای/Ne) (MN (N آدولف/N) (N بورن/N)))
+                (VPC
+                  (NPC (N دنیای/Ne) (NPA (N اتفاقات/Ne) (ADJ رویایی/AJ)))
+                  (V است/V)))
+              (PUNC ./PUNC))
+
+
+        Yields:
+            ساختار درختی بعدی.
+
+        """
+
+        def traverse(node: str) -> Tree:
+            def extract_tags(w: str):
+                pos = [w.getAttribute("lc") if w.getAttribute("lc") else None]
+                if w.getAttribute("clitic") in {
+                    "ezafe",
+                    "pronominal",
+                    "verb",
+                    "prep",
+                    "adv",
+                    "det",
+                }:
+                    pos.append(w.getAttribute("clitic"))
+                if w.getAttribute("ne_sort"):
+                    pos.append(w.getAttribute("ne_sort"))
+                if w.getAttribute("n_type"):
+                    pos.append(w.getAttribute("n_type"))
+                if w.getAttribute("ya_type"):
+                    pos.append(w.getAttribute("ya_type"))
+                if w.getAttribute("ke_type"):
+                    pos.append(w.getAttribute("ke_type"))
+                if w.getAttribute("type"):
+                    pos.append(w.getAttribute("type"))
+                if w.getAttribute("kind"):
+                    pos.append(w.getAttribute("kind"))
+                return pos
+
+            def clitic_join(tree: Tree, clitic: Dict):
+                if type(tree[-1]) == Tree:
+                    return clitic_join(tree[-1], clitic)
+
+                if clitic[0][0][0] == "ا":
+                    clitic[0] = ("‌" + clitic[0][0], clitic[0][1])
+                tree[-1] = (tree[-1][0] + clitic[0][0], clitic[0][1])
+                tree.set_label("CLITICS")
+                return None
+
+            if not len(node.childNodes):
+                return None
+            first = node.childNodes[0]
+            if first.tagName == "w":
+                pos = extract_tags(first)
+                return Tree(
+                    node.tagName,
+                    [
+                        (
+                            first.childNodes[0].data.replace("می ", "می‌"),
+                            self._pos_map(pos),
+                        ),
+                    ],
+                )
+            childs = node.childNodes[2:] if node.tagName == "S" else node.childNodes
+            for child in childs:
+                if not len(child.childNodes):
+                    childs.remove(child)
+            tree = Tree(node.tagName, map(traverse, childs))
+            if (
+                self._join_clitics
+                and len(tree) > 1
+                and type(tree[1]) == Tree
+                and tree[1].label() == "CLITIC"
+                and tree[1][0][1] not in {"P", "V"}
+            ):
+                clitic = tree[-1]
+                tree = Tree(tree.label(), list(tree[0]))
+                clitic_join(tree, clitic)
+            if (
+                self._join_verb_parts
+                and len(tree) > 1
+                and type(tree[1]) == Tree
+                and type(tree[0]) == Tree
+                and tree[0].label() == "AUX"
+                and tree[0][0][0] in self._tokenizer.before_verbs
+            ):
+                tree[1][0] = (tree[0][0][0] + " " + tree[1][0][0], tree[1][0][1])
+                tree.remove(tree[0])
+            if (
+                self._join_verb_parts
+                and len(tree.leaves()) > 1
+                and tree.leaves()[-1][0] in self._tokenizer.after_verbs
+                and tree.leaves()[-2][0] in self._tokenizer.verbe
+            ):
+                tree[1][0] = (
+                    tree[0].leaves()[-1][0] + " " + tree[1][0][0],
+                    tree[1][0][1],
+                )
+                path = tree.leaf_treeposition(len(tree.leaves()) - 2)
+                removingtree = tree
+                while len(path) > 2:
+                    removingtree = removingtree[path[0]]
+                    path = path[1:]
+                removingtree.remove(Tree(tree.pos()[-2][1], [tree.pos()[-2][0]]))
+            if (
+                self._join_verb_parts
+                and len(tree.leaves()) > 1
+                and tree.leaves()[-1][0] in self._tokenizer.after_verbs
+                and tree.leaves()[-2][0] in self._tokenizer.verbe
+            ):
+                tree[1][0] = (
+                    tree[0].leaves()[-1][0] + " " + tree[1][0][0],
+                    tree[1][0][1],
+                )
+                path = tree.leaf_treeposition(len(tree.leaves()) - 2)
+                removingtree = tree
+                while len(path) > 2:
+                    removingtree = removingtree[path[0]]
+                    path = path[1:]
+                removingtree.remove(Tree(tree.pos()[-2][1], [tree.pos()[-2][0]]))
+            return tree
+
+        for doc in self.docs():
+            for s in doc.getElementsByTagName("S"):
+                traverse(s)
+                yield traverse(s)
+
+    def sents(self: "TreebankReader") -> Iterator[List[Tuple[str, str]]]:
+        """جملات را به شکل مجموعه‌ای از `(توکن،برچسب)`ها برمی‌گرداند.
+
+        Examples:
+            >>> treebank = TreebankReader(root='treebank')
+            >>> next(treebank.sents())
+            [('دنیای', 'Ne'), ('آدولف', 'N'), ('بورن', 'N'), ('دنیای', 'Ne'), ('اتفاقات', 'Ne'), ('رویایی', 'AJ'), ('است', 'V'), ('.', 'PUNC')]
+
+        Yields:
+            جملهٔ بعدی.
+
+        """
+        for tree in self.trees():
+            yield tree.leaves()
+
+    def chunked_trees(self: "TreebankReader") -> Iterator[str]:
+        """ساختار درختی را به شکل تقطیع شده برمی‌گرداند.
+
+        Examples:
+            >>> from hazm.chunker import tree2brackets
+            >>> treebank = TreebankReader(root='treebank')
+            >>> tree2brackets(next(treebank.chunked_trees()))
+            '[دنیای آدولف بورن NP] [دنیای اتفاقات رویایی NP] [است VP] .'
+
+        Yields:
+            درخت تقطیع شدهٔ بعدی.
+
+        """
+
+        def collapse(node, label):
+            return Tree(label, [Tree(pos[1], [pos[0]]) for pos in node.pos()])
+
+        def traverse(node, parent, chunks):
+            label = node.label()
+
+            if label.count("-nid") > 0:
+                label = label.replace("-nid", "")
+            if label.count("-nid") > 0:
+                label = label.replace("-nid", "")
+            if label.count("-DiscA") > 0:
+                label = label.replace("-DiscA", "")
+
+            if label in {"CLITIC", "CLITICS"}:
+                if node[0][1] == "V":
+                    label = "V"
+                elif node[0][1] == "P":
+                    label = "PREP"
+                elif node[0][1] == "DET":
+                    label = "DET"
+                elif node[0][1] == "ADV":
+                    label = "ADV"
+                elif node[0][1] == "PRO":
+                    label = "PRON"
+
+            if label in {"CONJ", "PUNC"} and len(node) == 1:
+                chunks.append(node)
+                return
+
+            if label == "PPC" and len(node) == 1:
+                chunks.append(Tree("PP", [node[0]]))
+                return
+
+            if label == "PREP":
+                chunks.append(Tree("PP", [node]))
+                return
+
+            if label == "PostP":
+                chunks.append(Tree("POSTP", [node]))
+                return
+
+            for leaf in node.pos():
+                if leaf[1] in {"PUNC", "CONJ", "PREP", "PostP"}:
+                    for i in range(len(node)):
+                        traverse(node[i], node, chunks)
+                    return
+
+            if label == "NPA" and parent.label() in {"CPC", "PPC"}:
+                chunks.append(collapse(node, "NP"))
+                return
+
+            if label == "NPA" and len(node) >= 1 and node[0].label() == "ADV":
+                chunks.append(collapse(node, "NP"))
+                return
+
+            if label in {
+                "NPC",
+                "N",
+                "INFV",
+                "DPA",
+                "CLASS",
+                "DPC",
+                "DEM",
+                "INTJ",
+                "MN",
+                "PRON",
+                "DET",
+                "NUM",
+                "RES",
+            }:
+                chunks.append(collapse(node, "NP"))
+                return
+
+            if (
+                label == "NPA"
+                and len(node) >= 2
+                and (
+                    node[0].label() == "ADJ"
+                    and node[1].label() == "NPC"
+                    or node[0].label() in {"N", "PRON"}
+                    and node[1].label() in {"ADJ", "ADJPA", "N"}
+                    or node[0].label() == "NUM"
+                    and node[1].label() in {"N", "NPC", "MN", "NUM"}
+                    or node[0].label() in {"N", "NPC", "MN"}
+                    and node[1].label() == "NUM"
+                    or node[0].label() == "NPC"
+                    and node[1].label() == "ADJ"
+                    or node[0].label() == "NPA"
+                    and node[1].label() != "NPC"
+                    or node[1].label() == "NPA"
+                    and node[0].label() != "NPC"
+                )
+            ):
+                chunks.append(collapse(node, "NP"))
+                return
+
+            if label == "DPC" and len(node) >= 2:
+                chunkable = True
+                for leaf in node[1].pos():
+                    if leaf[1] in {"PUNC", "CONJ", "PREP", "PostP"}:
+                        chunkable = False
+                if node[1].label() in {"N", "NPA", "NPC"} and chunkable:
+                    chunks.append(collapse(node, "NP"))
+                    return
+
+            if label == "DPA" and len(node) >= 2 and node[1].label() == "ADV":
+                chunks.append(collapse(node, "ADVP"))
+                return
+
+            if label in {"MV", "V", "AUX", "PPARV"}:
+                chunks.append(Tree("VP", [node]))
+                return
+
+            if label in {"ADJ", "ADJPC", "MADJ", "ADVPA"}:
+                chunks.append(Tree("ADJP", [node]))
+                return
+
+            if label in {"ADV", "MADV", "ADVPC"}:
+                chunks.append(Tree("ADVP", [node]))
+                return
+
+            if type(node[0]) != Tree:
+                chunks.append(node)
+                return
+
+            for i in range(len(node)):
+                traverse(node[i], node, chunks)
+
+        for tree in self.trees():
+            chunks = []
+            traverse(tree, None, chunks)
+            for i in range(len(chunks)):
+                if chunks[i].label() in {"PUNC", "CONJ"}:
+                    chunks[i] = chunks[i][0]
+                else:
+                    chunks[i] = Tree(chunks[i].label(), chunks[i].leaves())
+            yield Tree("S", chunks)
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/verbvalency_reader.py` & `hazm-0.9.2/hazm/corpus_readers/verbvalency_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ ظرفیت نحوی افعال فارسی
-است.
-
-پیکرهٔ ظرفیت نحوی افعال فارسی مجموعه‌ای است حاوی اطلاعات مربوط به ظرفیت نحوی
-بیش
-از ۴۵۰۰ فعل در زبان فارسی. در این فرهنگ، متمم‌های اجباری و اختیاری انواع
-فعل‌های
-ساده، مرکب، پیشوندی و عبارات فعلی مشخص شده است. فراوانی فعل‌های مرکب در زبان
-فارسی، نیاز به فرهنگ ظرفیت فعل را در این زبان دوچندان می‌نماید. چرا که شناخت
-فعل‌های مرکب چه از لحاظ انسانی و چه از لحاظ پردازشی کاری دشوار‌تر از شناخت
-فعل‌های ساده است و به همین خاطر فراهم آوردن فهرستی از فعل‌های زبان (که شامل
-فعل‌های مرکب نیز می‌شود) به همراه ساخت‌های ظرفیتی افعال، کمکی شایان برای کارهای
-پردازشی است. از سوی دیگر، بر اساس نظریه وابستگی، ساخت بنیادین جمله را می‌توان
-از
-روی ساخت ظرفیتی فعل جمله به دست آورد و به همین دلیل بر اهمیت دانستن ساخت‌های
-ظرفیتی فعل در متن‌های زبانی افزوده می‌شود.
-
-"""
-
-
-from collections import namedtuple
-from pathlib import Path
-from typing import Iterator
-
-Verb = namedtuple(
-    "Verb",
-    (
-        "past_light_verb",
-        "present_light_verb",
-        "prefix",
-        "nonverbal_element",
-        "preposition",
-        "valency",
-    ),
-)
-
-
-class VerbValencyReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ ظرفیت نحوی افعال فارسی است.
-
-    Args:
-        valency_file: مسیر فایلِ پیکره.
-
-    """
-
-    def __init__(
-        self: "VerbValencyReader", valency_file: str = "corpora/valency.txt",
-    ) -> None:
-        self._valency_file = valency_file
-
-    def verbs(self: "VerbValencyReader") -> Iterator[Verb]:
-        """افعال پیکره را برمی‌گرداند.
-
-        Yields:
-            فعل بعدی.
-
-        """
-        with Path.open(self._valency_file, encoding="utf-8") as valency_file:
-            for line in valency_file:
-                if "بن ماضی" in line:
-                    continue
-
-                line = line.strip().replace("-\t", "\t")
-                parts = line.split("\t")
-                if len(parts) == 6:
-                    yield Verb(*parts)
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ ظرفیت نحوی افعال فارسی
+است.
+
+پیکرهٔ ظرفیت نحوی افعال فارسی مجموعه‌ای است حاوی اطلاعات مربوط به ظرفیت نحوی
+بیش
+از ۴۵۰۰ فعل در زبان فارسی. در این فرهنگ، متمم‌های اجباری و اختیاری انواع
+فعل‌های
+ساده، مرکب، پیشوندی و عبارات فعلی مشخص شده است. فراوانی فعل‌های مرکب در زبان
+فارسی، نیاز به فرهنگ ظرفیت فعل را در این زبان دوچندان می‌نماید. چرا که شناخت
+فعل‌های مرکب چه از لحاظ انسانی و چه از لحاظ پردازشی کاری دشوار‌تر از شناخت
+فعل‌های ساده است و به همین خاطر فراهم آوردن فهرستی از فعل‌های زبان (که شامل
+فعل‌های مرکب نیز می‌شود) به همراه ساخت‌های ظرفیتی افعال، کمکی شایان برای کارهای
+پردازشی است. از سوی دیگر، بر اساس نظریه وابستگی، ساخت بنیادین جمله را می‌توان
+از
+روی ساخت ظرفیتی فعل جمله به دست آورد و به همین دلیل بر اهمیت دانستن ساخت‌های
+ظرفیتی فعل در متن‌های زبانی افزوده می‌شود.
+
+"""
+
+
+from collections import namedtuple
+from pathlib import Path
+from typing import Iterator
+
+Verb = namedtuple(
+    "Verb",
+    (
+        "past_light_verb",
+        "present_light_verb",
+        "prefix",
+        "nonverbal_element",
+        "preposition",
+        "valency",
+    ),
+)
+
+
+class VerbValencyReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ ظرفیت نحوی افعال فارسی است.
+
+    Args:
+        valency_file: مسیر فایلِ پیکره.
+
+    """
+
+    def __init__(
+        self: "VerbValencyReader", valency_file: str = "valency.txt",
+    ) -> None:
+        self._valency_file = valency_file
+
+    def verbs(self: "VerbValencyReader") -> Iterator[Verb]:
+        """افعال پیکره را برمی‌گرداند.
+
+        Yields:
+            فعل بعدی.
+
+        """
+        with Path.open(self._valency_file, encoding="utf-8") as valency_file:
+            for line in valency_file:
+                if "بن ماضی" in line:
+                    continue
+
+                line = line.strip().replace("-\t", "\t")
+                parts = line.split("\t")
+                if len(parts) == 6:
+                    yield Verb(*parts)
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/wiki_extractor.py` & `hazm-0.9.2/hazm/corpus_readers/wiki_extractor.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,1859 +1,1859 @@
-# -*- coding: utf-8 -*-
-
-# =============================================================================
-#  Copyright (c) 2020. Giuseppe Attardi (attardi@di.unipi.it).
-# =============================================================================
-#  This file is part of Tanl.
-#
-#  Tanl is free software; you can redistribute it and/or modify it
-#  under the terms of the GNU Affero General Public License, version 3,
-#  as published by the Free Software Foundation.
-#
-#  Tanl is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Affero General Public License for more details.
-#
-#  You should have received a copy of the GNU Affero General Public License
-#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-# =============================================================================
-
-import re
-import html
-import json
-from itertools import zip_longest
-from urllib.parse import quote as urlencode
-from html.entities import name2codepoint
-import logging
-import time
-
-# ----------------------------------------------------------------------
-
-# match tail after wikilink
-tailRE = re.compile('\w+')
-syntaxhighlight = re.compile('&lt;syntaxhighlight .*?&gt;(.*?)&lt;/syntaxhighlight&gt;', re.DOTALL)
-
-## PARAMS ####################################################################
-
-##
-# Defined in <siteinfo>
-# We include as default Template, when loading external template file.
-knownNamespaces = set(['Template'])
-
-##
-# Drop these elements from article text
-#
-discardElements = [
-    'gallery', 'timeline', 'noinclude', 'pre',
-    'table', 'tr', 'td', 'th', 'caption', 'div',
-    'form', 'input', 'select', 'option', 'textarea',
-    'ul', 'li', 'ol', 'dl', 'dt', 'dd', 'menu', 'dir',
-    'ref', 'references', 'img', 'imagemap', 'source', 'small'
-]
-
-##
-# Recognize only these namespaces
-# w: Internal links to the Wikipedia
-# wiktionary: Wiki dictionary
-# wikt: shortcut for Wiktionary
-#
-acceptedNamespaces = ['w', 'wiktionary', 'wikt']
-
-
-def get_url(urlbase, uid):
-    return "%s?curid=%s" % (urlbase, uid)
-
-
-# ======================================================================
-
-
-def clean(extractor, text, expand_templates=False, html_safe=True):
-    """
-    Transforms wiki markup. If the command line flag --escapedoc is set then the text is also escaped
-    @see https://www.mediawiki.org/wiki/Help:Formatting
-    :param extractor: the Extractor t use.
-    :param text: the text to clean.
-    :param expand_templates: whether to perform template expansion.
-    :param html_safe: whether to convert reserved HTML characters to entities.
-    @return: the cleaned text.
-    """
-
-    if expand_templates:
-        # expand templates
-        # See: http://www.mediawiki.org/wiki/Help:Templates
-        text = extractor.expandTemplates(text)
-    else:
-        # Drop transclusions (template, parser functions)
-        text = dropNested(text, r'{{', r'}}')
-
-    # Drop tables
-    text = dropNested(text, r'{\|', r'\|}')
-
-    # replace external links
-    text = replaceExternalLinks(text)
-
-    # replace internal links
-    text = replaceInternalLinks(text)
-
-    # drop MagicWords behavioral switches
-    text = magicWordsRE.sub('', text)
-
-    # ############### Process HTML ###############
-
-    # turn into HTML, except for the content of <syntaxhighlight>
-    res = ''
-    cur = 0
-    for m in syntaxhighlight.finditer(text):
-        end = m.end()
-        res += unescape(text[cur:m.start()]) + m.group(1)
-        cur = end
-    text = res + unescape(text[cur:])
-
-    # Handle bold/italic/quote
-    if extractor.HtmlFormatting:
-        text = bold_italic.sub(r'<b>\1</b>', text)
-        text = bold.sub(r'<b>\1</b>', text)
-        text = italic.sub(r'<i>\1</i>', text)
-    else:
-        text = bold_italic.sub(r'\1', text)
-        text = bold.sub(r'\1', text)
-        text = italic_quote.sub(r'"\1"', text)
-        text = italic.sub(r'"\1"', text)
-        text = quote_quote.sub(r'"\1"', text)
-    # residuals of unbalanced quotes
-    text = text.replace("'''", '').replace("''", '"')
-
-    # Collect spans
-
-    spans = []
-    # Drop HTML comments
-    for m in comment.finditer(text):
-        spans.append((m.start(), m.end()))
-
-    # Drop self-closing tags
-    for pattern in selfClosing_tag_patterns:
-        for m in pattern.finditer(text):
-            spans.append((m.start(), m.end()))
-
-    # Drop ignored tags
-    for left, right in ignored_tag_patterns:
-        for m in left.finditer(text):
-            spans.append((m.start(), m.end()))
-        for m in right.finditer(text):
-            spans.append((m.start(), m.end()))
-
-    # Bulk remove all spans
-    text = dropSpans(spans, text)
-
-    # Drop discarded elements
-    for tag in discardElements:
-        text = dropNested(text, r'<\s*%s\b[^>/]*>' % tag, r'<\s*/\s*%s>' % tag)
-
-    if not extractor.HtmlFormatting:
-        # Turn into text what is left (&amp;nbsp;) and <syntaxhighlight>
-        text = unescape(text)
-
-    # Expand placeholders
-    for pattern, placeholder in placeholder_tag_patterns:
-        index = 1
-        for match in pattern.finditer(text):
-            text = text.replace(match.group(), '%s_%d' % (placeholder, index))
-            index += 1
-
-    text = text.replace('<<', u'«').replace('>>', u'»')
-
-    #############################################
-
-    # Cleanup text
-    text = text.replace('\t', ' ')
-    text = spaces.sub(' ', text)
-    text = dots.sub('...', text)
-    text = re.sub(u' (,:\.\)\]»)', r'\1', text)
-    text = re.sub(u'(\[\(«) ', r'\1', text)
-    text = re.sub(r'\n\W+?\n', '\n', text, flags=re.U)  # lines with only punctuations
-    text = text.replace(',,', ',').replace(',.', '.')
-    if html_safe:
-        text = html.escape(text, quote=False)
-    return text
-
-
-# skip level 1, it is page name level
-section = re.compile(r'(==+)\s*(.*?)\s*\1')
-
-listOpen = {'*': '<ul>', '#': '<ol>', ';': '<dl>', ':': '<dl>'}
-listClose = {'*': '</ul>', '#': '</ol>', ';': '</dl>', ':': '</dl>'}
-listItem = {'*': '<li>%s</li>', '#': '<li>%s</<li>', ';': '<dt>%s</dt>',
-            ':': '<dd>%s</dd>'}
-
-
-def compact(text, mark_headers=False):
-    """Deal with headers, lists, empty sections, residuals of tables.
-    :param text: convert to HTML
-    """
-
-    page = []  # list of paragraph
-    headers = {}  # Headers for unfilled sections
-    emptySection = False  # empty sections are discarded
-    listLevel = ''  # nesting of lists
-
-    for line in text.split('\n'):
-
-        if not line:
-            if len(listLevel):    # implies Extractor.HtmlFormatting
-                for c in reversed(listLevel):
-                    page.append(listClose[c])
-                    listLevel = ''
-            continue
-
-        # Handle section titles
-        m = section.match(line)
-        if m:
-            title = m.group(2)
-            lev = len(m.group(1))
-            if Extractor.HtmlFormatting:
-                page.append("<h%d>%s</h%d>" % (lev, title, lev))
-            if title and title[-1] not in '!?':
-                title += '.'
-
-            if mark_headers:
-                title = "## " + title
-
-            headers[lev] = title
-            # drop previous headers
-            headers = { k:v for k,v in headers.items() if k <= lev }
-            emptySection = True
-            continue
-        # Handle page title
-        if line.startswith('++'):
-            title = line[2:-2]
-            if title:
-                if title[-1] not in '!?':
-                    title += '.'
-                page.append(title)
-        # handle indents
-        elif line[0] == ':':
-            page.append(line.lstrip(':'))
-        # handle lists
-        # @see https://www.mediawiki.org/wiki/Help:Formatting
-        elif line[0] in '*#;':
-            if Extractor.HtmlFormatting:
-                # close extra levels
-                l = 0
-                for c in listLevel:
-                    if l < len(line) and c != line[l]:
-                        for extra in reversed(listLevel[l:]):
-                            page.append(listClose[extra])
-                        listLevel = listLevel[:l]
-                        break
-                    l += 1
-                if l < len(line) and line[l] in '*#;:':
-                    # add new level (only one, no jumps)
-                    # FIXME: handle jumping levels
-                    type = line[l]
-                    page.append(listOpen[type])
-                    listLevel += type
-                    line = line[l+1:].strip()
-                else:
-                    # continue on same level
-                    type = line[l-1]
-                    line = line[l:].strip()
-                page.append(listItem[type] % line)
-            else:
-                continue
-        elif len(listLevel):    # implies Extractor.HtmlFormatting
-            for c in reversed(listLevel):
-                page.append(listClose[c])
-            listLevel = []
-
-        # Drop residuals of lists
-        elif line[0] in '{|' or line[-1] == '}':
-            continue
-        # Drop irrelevant lines
-        elif (line[0] == '(' and line[-1] == ')') or line.strip('.-') == '':
-            continue
-        elif len(headers):
-            if Extractor.keepSections:
-                items = sorted(headers.items())
-                for (i, v) in items:
-                    page.append(v)
-            headers.clear()
-            page.append(line)  # first line
-            emptySection = False
-        elif not emptySection:
-            page.append(line)
-            # dangerous
-            # # Drop preformatted
-            # elif line[0] == ' ':
-            #     continue
-
-    return page
-
-
-# ----------------------------------------------------------------------
-
-def dropNested(text, openDelim, closeDelim):
-    """
-    A matching function for nested expressions, e.g. namespaces and tables.
-    """
-    openRE = re.compile(openDelim, re.IGNORECASE)
-    closeRE = re.compile(closeDelim, re.IGNORECASE)
-    # partition text in separate blocks { } { }
-    spans = []  # pairs (s, e) for each partition
-    nest = 0  # nesting level
-    start = openRE.search(text, 0)
-    if not start:
-        return text
-    end = closeRE.search(text, start.end())
-    next = start
-    while end:
-        next = openRE.search(text, next.end())
-        if not next:  # termination
-            while nest:  # close all pending
-                nest -= 1
-                end0 = closeRE.search(text, end.end())
-                if end0:
-                    end = end0
-                else:
-                    break
-            spans.append((start.start(), end.end()))
-            break
-        while end.end() < next.start():
-            # { } {
-            if nest:
-                nest -= 1
-                # try closing more
-                last = end.end()
-                end = closeRE.search(text, end.end())
-                if not end:  # unbalanced
-                    if spans:
-                        span = (spans[0][0], last)
-                    else:
-                        span = (start.start(), last)
-                    spans = [span]
-                    break
-            else:
-                spans.append((start.start(), end.end()))
-                # advance start, find next close
-                start = next
-                end = closeRE.search(text, next.end())
-                break  # { }
-        if next != start:
-            # { { }
-            nest += 1
-    # collect text outside partitions
-    return dropSpans(spans, text)
-
-
-def dropSpans(spans, text):
-    """
-    Drop from text the blocks identified in :param spans:, possibly nested.
-    """
-    spans.sort()
-    res = ''
-    offset = 0
-    for s, e in spans:
-        if offset <= s:  # handle nesting
-            if offset < s:
-                res += text[offset:s]
-            offset = e
-    res += text[offset:]
-    return res
-
-
-# ----------------------------------------------------------------------
-# External links
-
-# from: https://doc.wikimedia.org/mediawiki-core/master/php/DefaultSettings_8php_source.html
-
-wgUrlProtocols = [
-    'bitcoin:', 'ftp://', 'ftps://', 'geo:', 'git://', 'gopher://', 'http://',
-    'https://', 'irc://', 'ircs://', 'magnet:', 'mailto:', 'mms://', 'news:',
-    'nntp://', 'redis://', 'sftp://', 'sip:', 'sips:', 'sms:', 'ssh://',
-    'svn://', 'tel:', 'telnet://', 'urn:', 'worldwind://', 'xmpp:', '//'
-]
-
-# from: https://doc.wikimedia.org/mediawiki-core/master/php/Parser_8php_source.html
-
-# Constants needed for external link processing
-# Everything except bracket, space, or control characters
-# \p{Zs} is unicode 'separator, space' category. It covers the space 0x20
-# as well as U+3000 is IDEOGRAPHIC SPACE for bug 19052
-EXT_LINK_URL_CLASS = r'[^][<>"\x00-\x20\x7F\s]'
-ExtLinkBracketedRegex = re.compile(
-    '(?i)\[((' + '|'.join(wgUrlProtocols) + ')' + EXT_LINK_URL_CLASS + r'+)\s*([^\]\x00-\x08\x0a-\x1F]*?)\]',
-    re.S | re.U)
-EXT_IMAGE_REGEX = re.compile(
-    r"""(?i)^(http://|https://)([^][<>"\x00-\x20\x7F\s]+)
-    /([A-Za-z0-9_.,~%\-+&;#*?!=()@\x80-\xFF]+)\.(gif|png|jpg|jpeg)$""",
-    re.X | re.S | re.U)
-
-
-def replaceExternalLinks(text):
-    s = ''
-    cur = 0
-    for m in ExtLinkBracketedRegex.finditer(text):
-        s += text[cur:m.start()]
-        cur = m.end()
-
-        url = m.group(1)
-        label = m.group(3)
-
-        # # The characters '<' and '>' (which were escaped by
-        # # removeHTMLtags()) should not be included in
-        # # URLs, per RFC 2396.
-        # m2 = re.search('&(lt|gt);', url)
-        # if m2:
-        #     link = url[m2.end():] + ' ' + link
-        #     url = url[0:m2.end()]
-
-        # If the link text is an image URL, replace it with an <img> tag
-        # This happened by accident in the original parser, but some people used it extensively
-        m = EXT_IMAGE_REGEX.match(label)
-        if m:
-            label = makeExternalImage(label)
-
-        # Use the encoded URL
-        # This means that users can paste URLs directly into the text
-        # Funny characters like ö aren't valid in URLs anyway
-        # This was changed in August 2004
-        s += makeExternalLink(url, label)  # + trail
-
-    return s + text[cur:]
-
-
-def makeExternalLink(url, anchor):
-    """Function applied to wikiLinks"""
-    if Extractor.keepLinks:
-        return '<a href="%s">%s</a>' % (urlencode(url), anchor)
-    else:
-        return anchor
-
-
-def makeExternalImage(url, alt=''):
-    if Extractor.keepLinks:
-        return '<img src="%s" alt="%s">' % (url, alt)
-    else:
-        return alt
-
-
-# ----------------------------------------------------------------------
-# WikiLinks
-# See https://www.mediawiki.org/wiki/Help:Links#Internal_links
-
-# Can be nested [[File:..|..[[..]]..|..]], [[Category:...]], etc.
-# Also: [[Help:IPA for Catalan|[andora]]]
-
-
-def replaceInternalLinks(text):
-    """
-    Replaces external links of the form:
-    [[title |...|label]]trail
-
-    with title concatenated with trail, when present, e.g. 's' for plural.
-    """
-    # call this after removal of external links, so we need not worry about
-    # triple closing ]]].
-    cur = 0
-    res = ''
-    for s, e in findBalanced(text, ['[['], [']]']):
-        m = tailRE.match(text, e)
-        if m:
-            trail = m.group(0)
-            end = m.end()
-        else:
-            trail = ''
-            end = e
-        inner = text[s + 2:e - 2]
-        # find first |
-        pipe = inner.find('|')
-        if pipe < 0:
-            title = inner
-            label = title
-        else:
-            title = inner[:pipe].rstrip()
-            # find last |
-            curp = pipe + 1
-            for s1, e1 in findBalanced(inner, ['[['], [']]']):
-                last = inner.rfind('|', curp, s1)
-                if last >= 0:
-                    pipe = last  # advance
-                curp = e1
-            label = inner[pipe + 1:].strip()
-        res += text[cur:s] + makeInternalLink(title, label) + trail
-        cur = end
-    return res + text[cur:]
-
-
-def makeInternalLink(title, label):
-    colon = title.find(':')
-    if colon > 0 and title[:colon] not in acceptedNamespaces:
-        return ''
-    if colon == 0:
-        # drop also :File:
-        colon2 = title.find(':', colon + 1)
-        if colon2 > 1 and title[colon + 1:colon2] not in acceptedNamespaces:
-            return ''
-    if Extractor.keepLinks:
-        return '<a href="%s">%s</a>' % (urlencode(title), label)
-    else:
-        return label
-
-
-# ----------------------------------------------------------------------
-# variables
-
-
-class MagicWords():
-
-    """
-    One copy in each Extractor.
-
-    @see https://doc.wikimedia.org/mediawiki-core/master/php/MagicWord_8php_source.html
-    """
-    names = [
-        '!',
-        'currentmonth',
-        'currentmonth1',
-        'currentmonthname',
-        'currentmonthnamegen',
-        'currentmonthabbrev',
-        'currentday',
-        'currentday2',
-        'currentdayname',
-        'currentyear',
-        'currenttime',
-        'currenthour',
-        'localmonth',
-        'localmonth1',
-        'localmonthname',
-        'localmonthnamegen',
-        'localmonthabbrev',
-        'localday',
-        'localday2',
-        'localdayname',
-        'localyear',
-        'localtime',
-        'localhour',
-        'numberofarticles',
-        'numberoffiles',
-        'numberofedits',
-        'articlepath',
-        'pageid',
-        'sitename',
-        'server',
-        'servername',
-        'scriptpath',
-        'stylepath',
-        'pagename',
-        'pagenamee',
-        'fullpagename',
-        'fullpagenamee',
-        'namespace',
-        'namespacee',
-        'namespacenumber',
-        'currentweek',
-        'currentdow',
-        'localweek',
-        'localdow',
-        'revisionid',
-        'revisionday',
-        'revisionday2',
-        'revisionmonth',
-        'revisionmonth1',
-        'revisionyear',
-        'revisiontimestamp',
-        'revisionuser',
-        'revisionsize',
-        'subpagename',
-        'subpagenamee',
-        'talkspace',
-        'talkspacee',
-        'subjectspace',
-        'subjectspacee',
-        'talkpagename',
-        'talkpagenamee',
-        'subjectpagename',
-        'subjectpagenamee',
-        'numberofusers',
-        'numberofactiveusers',
-        'numberofpages',
-        'currentversion',
-        'rootpagename',
-        'rootpagenamee',
-        'basepagename',
-        'basepagenamee',
-        'currenttimestamp',
-        'localtimestamp',
-        'directionmark',
-        'contentlanguage',
-        'numberofadmins',
-        'cascadingsources',
-    ]
-
-    def __init__(self):
-        self.values = {'!': '|'}
-
-    def __getitem__(self, name):
-        return self.values.get(name)
-
-    def __setitem__(self, name, value):
-        self.values[name] = value
-
-    switches = (
-        '__NOTOC__',
-        '__FORCETOC__',
-        '__TOC__',
-        '__TOC__',
-        '__NEWSECTIONLINK__',
-        '__NONEWSECTIONLINK__',
-        '__NOGALLERY__',
-        '__HIDDENCAT__',
-        '__NOCONTENTCONVERT__',
-        '__NOCC__',
-        '__NOTITLECONVERT__',
-        '__NOTC__',
-        '__START__',
-        '__END__',
-        '__INDEX__',
-        '__NOINDEX__',
-        '__STATICREDIRECT__',
-        '__DISAMBIG__'
-    )
-
-
-magicWordsRE = re.compile('|'.join(MagicWords.switches))
-
-
-# =========================================================================
-#
-# MediaWiki Markup Grammar
-# https://www.mediawiki.org/wiki/Preprocessor_ABNF
-
-# xml-char = %x9 / %xA / %xD / %x20-D7FF / %xE000-FFFD / %x10000-10FFFF
-# sptab = SP / HTAB
-
-# ; everything except ">" (%x3E)
-# attr-char = %x9 / %xA / %xD / %x20-3D / %x3F-D7FF / %xE000-FFFD / %x10000-10FFFF
-
-# literal         = *xml-char
-# title           = wikitext-L3
-# part-name       = wikitext-L3
-# part-value      = wikitext-L3
-# part            = ( part-name "=" part-value ) / ( part-value )
-# parts           = [ title *( "|" part ) ]
-# tplarg          = "{{{" parts "}}}"
-# template        = "{{" parts "}}"
-# link            = "[[" wikitext-L3 "]]"
-
-# comment         = "<!--" literal "-->"
-# unclosed-comment = "<!--" literal END
-# ; the + in the line-eating-comment rule was absent between MW 1.12 and MW 1.22
-# line-eating-comment = LF LINE-START *SP +( comment *SP ) LINE-END
-
-# attr            = *attr-char
-# nowiki-element  = "<nowiki" attr ( "/>" / ( ">" literal ( "</nowiki>" / END ) ) )
-
-# wikitext-L2     = heading / wikitext-L3 / *wikitext-L2
-# wikitext-L3     = literal / template / tplarg / link / comment /
-#                   line-eating-comment / unclosed-comment / xmlish-element /
-#                   *wikitext-L3
-
-# ------------------------------------------------------------------------------
-
-selfClosingTags = ('br', 'hr', 'nobr', 'ref', 'references', 'nowiki')
-
-# These tags are dropped, keeping their content.
-# handle 'a' separately, depending on keepLinks
-ignoredTags = (
-    'abbr', 'b', 'big', 'blockquote', 'center', 'cite', 'div', 'em',
-    'font', 'h1', 'h2', 'h3', 'h4', 'hiero', 'i', 'kbd', 'nowiki',
-    'p', 'plaintext', 's', 'span', 'strike', 'strong',
-    'sub', 'sup', 'tt', 'u', 'var'
-)
-
-placeholder_tags = {'math': 'formula', 'code': 'codice'}
-
-
-def normalizeTitle(title):
-    """Normalize title"""
-    # remove leading/trailing whitespace and underscores
-    title = title.strip(' _')
-    # replace sequences of whitespace and underscore chars with a single space
-    title = re.sub(r'[\s_]+', ' ', title)
-
-    m = re.match(r'([^:]*):(\s*)(\S(?:.*))', title)
-    if m:
-        prefix = m.group(1)
-        if m.group(2):
-            optionalWhitespace = ' '
-        else:
-            optionalWhitespace = ''
-        rest = m.group(3)
-
-        ns = normalizeNamespace(prefix)
-        if ns in knownNamespaces:
-            # If the prefix designates a known namespace, then it might be
-            # followed by optional whitespace that should be removed to get
-            # the canonical page name
-            # (e.g., "Category:  Births" should become "Category:Births").
-            title = ns + ":" + ucfirst(rest)
-        else:
-            # No namespace, just capitalize first letter.
-            # If the part before the colon is not a known namespace, then we
-            # must not remove the space after the colon (if any), e.g.,
-            # "3001: The_Final_Odyssey" != "3001:The_Final_Odyssey".
-            # However, to get the canonical page name we must contract multiple
-            # spaces into one, because
-            # "3001:   The_Final_Odyssey" != "3001: The_Final_Odyssey".
-            title = ucfirst(prefix) + ":" + optionalWhitespace + ucfirst(rest)
-    else:
-        # no namespace, just capitalize first letter
-        title = ucfirst(title)
-    return title
-
-
-def unescape(text):
-    """
-    Removes HTML or XML character references and entities from a text string.
-
-    :param text The HTML (or XML) source text.
-    :return The plain text, as a Unicode string, if necessary.
-    """
-
-    def fixup(m):
-        text = m.group(0)
-        code = m.group(1)
-        try:
-            if text[1] == "#":  # character reference
-                if text[2] == "x":
-                    return chr(int(code[1:], 16))
-                else:
-                    return chr(int(code))
-            else:  # named entity
-                return chr(name2codepoint[code])
-        except:
-            return text  # leave as is
-
-    return re.sub("&#?(\w+);", fixup, text)
-
-
-# Match HTML comments
-# The buggy template {{Template:T}} has a comment terminating with just "->"
-comment = re.compile(r'<!--.*?-->', re.DOTALL)
-
-# Match ignored tags
-ignored_tag_patterns = []
-
-
-def ignoreTag(tag):
-    left = re.compile(r'<%s\b.*?>' % tag, re.IGNORECASE | re.DOTALL)  # both <ref> and <reference>
-    right = re.compile(r'</\s*%s>' % tag, re.IGNORECASE)
-    ignored_tag_patterns.append((left, right))
-
-
-def resetIgnoredTags():
-    global ignored_tag_patterns
-    ignored_tag_patterns = []
-
-
-for tag in ignoredTags:
-    ignoreTag(tag)
-
-# Match selfClosing HTML tags
-selfClosing_tag_patterns = [
-    re.compile(r'<\s*%s\b[^>]*/\s*>' % tag, re.DOTALL | re.IGNORECASE) for tag in selfClosingTags
-]
-
-# Match HTML placeholder tags
-placeholder_tag_patterns = [
-    (re.compile(r'<\s*%s(\s*| [^>]+?)>.*?<\s*/\s*%s\s*>' % (tag, tag), re.DOTALL | re.IGNORECASE),
-     repl) for tag, repl in placeholder_tags.items()
-]
-
-# Match preformatted lines
-preformatted = re.compile(r'^ .*?$')
-
-# Match external links (space separates second optional parameter)
-externalLink = re.compile(r'\[\w+[^ ]*? (.*?)]')
-externalLinkNoAnchor = re.compile(r'\[\w+[&\]]*\]')
-
-# Matches bold/italic
-bold_italic = re.compile(r"'''''(.*?)'''''")
-bold = re.compile(r"'''(.*?)'''")
-italic_quote = re.compile(r"''\"([^\"]*?)\"''")
-italic = re.compile(r"''(.*?)''")
-quote_quote = re.compile(r'""([^"]*?)""')
-
-# Matches space
-spaces = re.compile(r' {2,}')
-
-# Matches dots
-dots = re.compile(r'\.{4,}')
-
-# ======================================================================
-
-class Template(list):
-    """
-    A Template is a list of TemplateText or TemplateArgs
-    """
-
-    @classmethod
-    def parse(cls, body):
-        tpl = Template()
-        # we must handle nesting, s.a.
-        # {{{1|{{PAGENAME}}}
-        # {{{italics|{{{italic|}}}
-        # {{#if:{{{{{#if:{{{nominee|}}}|nominee|candidate}}|}}}|
-        #
-        start = 0
-        for s,e in findMatchingBraces(body, 3):
-            tpl.append(TemplateText(body[start:s]))
-            tpl.append(TemplateArg(body[s+3:e-3]))
-            start = e
-        tpl.append(TemplateText(body[start:])) # leftover
-        return tpl
-
-    def subst(self, params, extractor, depth=0):
-        # We perform parameter substitutions recursively.
-        # We also limit the maximum number of iterations to avoid too long or
-        # even endless loops (in case of malformed input).
-
-        # :see: http://meta.wikimedia.org/wiki/Help:Expansion#Distinction_between_variables.2C_parser_functions.2C_and_templates
-        #
-        # Parameter values are assigned to parameters in two (?) passes.
-        # Therefore a parameter name in a template can depend on the value of
-        # another parameter of the same template, regardless of the order in
-        # which they are specified in the template call, for example, using
-        # Template:ppp containing "{{{{{{p}}}}}}", {{ppp|p=q|q=r}} and even
-        # {{ppp|q=r|p=q}} gives r, but using Template:tvvv containing
-        # "{{{{{{{{{p}}}}}}}}}", {{tvvv|p=q|q=r|r=s}} gives s.
-
-        logging.debug('subst tpl (%d, %d) %s', len(extractor.frame), depth, self)
-
-        if depth > extractor.maxParameterRecursionLevels:
-            extractor.recursion_exceeded_3_errs += 1
-            return ''
-
-        return ''.join([tpl.subst(params, extractor, depth) for tpl in self])
-
-    def __str__(self):
-        return ''.join([str(x) for x in self])
-
-
-class TemplateText(str):
-    """Fixed text of template"""
-
-    def subst(self, params, extractor, depth):
-        return self
-
-
-class TemplateArg():
-    """
-    parameter to a template.
-    Has a name and a default value, both of which are Templates.
-    """
-    def __init__(self, parameter):
-        """
-        :param parameter: the parts of a tplarg.
-        """
-        # the parameter name itself might contain templates, e.g.:
-        #   appointe{{#if:{{{appointer14|}}}|r|d}}14|
-        #   4|{{{{{subst|}}}CURRENTYEAR}}
-
-        # any parts in a tplarg after the first (the parameter default) are
-        # ignored, and an equals sign in the first part is treated as plain text.
-        #logging.debug('TemplateArg %s', parameter)
-
-        parts = splitParts(parameter)
-        self.name = Template.parse(parts[0])
-        if len(parts) > 1:
-            # This parameter has a default value
-            self.default = Template.parse(parts[1])
-        else:
-            self.default = None
-
-    def __str__(self):
-        if self.default:
-            return '{{{%s|%s}}}' % (self.name, self.default)
-        else:
-            return '{{{%s}}}' % self.name
-
-    def subst(self, params, extractor, depth):
-        """
-        Substitute value for this argument from dict :param params:
-        Use :param extractor: to evaluate expressions for name and default.
-        Limit substitution to the maximun :param depth:.
-        """
-        # the parameter name itself might contain templates, e.g.:
-        # appointe{{#if:{{{appointer14|}}}|r|d}}14|
-        paramName = self.name.subst(params, extractor, depth+1)
-        paramName = extractor.expandTemplates(paramName)
-        res = ''
-        if paramName in params:
-            res = params[paramName]  # use parameter value specified in template invocation
-        elif self.default:            # use the default value
-            defaultValue = self.default.subst(params, extractor, depth+1)
-            res =  extractor.expandTemplates(defaultValue)
-        #logging.debug('subst arg %d %s -> %s' % (depth, paramName, res))
-        return res
-
-
-# ======================================================================
-
-substWords = 'subst:|safesubst:'
-
-
-class Extractor():
-    """
-    An extraction task on a article.
-    """
-    ##
-    # Whether to preserve links in output
-    keepLinks = False
-
-    ##
-    # Whether to preserve section titles
-    keepSections = True
-
-    ##
-    # Whether to output text with HTML formatting elements in <doc> files.
-    HtmlFormatting = False
-
-    ##
-    # Whether to produce json instead of the default <doc> output format.
-    toJson = False
-
-    ##
-    # Obtained from TemplateNamespace
-    templatePrefix = ''
-
-    def __init__(self, id, revid, urlbase, title, page):
-        """
-        :param page: a list of lines.
-        """
-        self.id = id
-        self.revid = revid
-        self.url = get_url(urlbase, id)
-        self.title = title
-        self.page = page
-        self.magicWords = MagicWords()
-        self.frame = []
-        self.recursion_exceeded_1_errs = 0  # template recursion within expandTemplates()
-        self.recursion_exceeded_2_errs = 0  # template recursion within expandTemplate()
-        self.recursion_exceeded_3_errs = 0  # parameter recursion
-        self.template_title_errs = 0
-
-    def clean_text(self, text, mark_headers=False, expand_templates=True,
-                   html_safe=True):
-        """
-        :param mark_headers: True to distinguish headers from paragraphs
-          e.g. "## Section 1"
-        """
-        self.magicWords['namespace'] = self.title[:max(0, self.title.find(":"))]
-        #self.magicWords['namespacenumber'] = '0' # for article,
-        self.magicWords['pagename'] = self.title
-        self.magicWords['fullpagename'] = self.title
-        self.magicWords['currentyear'] = time.strftime('%Y')
-        self.magicWords['currentmonth'] = time.strftime('%m')
-        self.magicWords['currentday'] = time.strftime('%d')
-        self.magicWords['currenthour'] = time.strftime('%H')
-        self.magicWords['currenttime'] = time.strftime('%H:%M:%S')
-
-        text = clean(self, text, expand_templates=expand_templates,
-                     html_safe=html_safe)
-
-        text = compact(text, mark_headers=mark_headers)
-        return text
-
-    def extract(self, out, html_safe=True):
-        """
-        :param out: a memory file.
-        :param html_safe: whether to escape HTML entities.
-        """
-        logging.debug("%s\t%s", self.id, self.title)
-        text = ''.join(self.page)
-        text = self.clean_text(text, html_safe=html_safe)
-
-        if self.to_json:
-            json_data = {
-		'id': self.id,
-                'revid': self.revid,
-                'url': self.url,
-                'title': self.title,
-                'text': "\n".join(text)
-            }
-            out_str = json.dumps(json_data)
-            out.write(out_str)
-            out.write('\n')
-        else:
-            header = '<doc id="%s" url="%s" title="%s">\n' % (self.id, self.url, self.title)
-            # Separate header from text with a newline.
-            header += self.title + '\n\n'
-            footer = "\n</doc>\n"
-            out.write(header)
-            out.write('\n'.join(text))
-            out.write('\n')
-            out.write(footer)
-
-        errs = (self.template_title_errs,
-                self.recursion_exceeded_1_errs,
-                self.recursion_exceeded_2_errs,
-                self.recursion_exceeded_3_errs)
-        if any(errs):
-            logging.warn("Template errors in article '%s' (%s): title(%d) recursion(%d, %d, %d)",
-                         self.title, self.id, *errs)
-
-    # ----------------------------------------------------------------------
-    # Expand templates
-
-    maxTemplateRecursionLevels = 30
-    maxParameterRecursionLevels = 16
-
-    # check for template beginning
-    reOpen = re.compile('(?<!{){{(?!{)', re.DOTALL)
-
-    def expandTemplates(self, wikitext):
-        """
-        :param wikitext: the text to be expanded.
-
-        Templates are frequently nested. Occasionally, parsing mistakes may
-        cause template insertion to enter an infinite loop, for instance when
-        trying to instantiate Template:Country
-
-        {{country_{{{1}}}|{{{2}}}|{{{2}}}|size={{{size|}}}|name={{{name|}}}}}
-
-        which is repeatedly trying to insert template 'country_', which is
-        again resolved to Template:Country. The straightforward solution of
-        keeping track of templates that were already inserted for the current
-        article would not work, because the same template may legally be used
-        more than once, with different parameters in different parts of the
-        article.  Therefore, we limit the number of iterations of nested
-        template inclusion.
-
-        """
-        # Test template expansion at:
-        # https://en.wikipedia.org/wiki/Special:ExpandTemplates
-
-        res = ''
-        if len(self.frame) >= self.maxTemplateRecursionLevels:
-            self.recursion_exceeded_1_errs += 1
-            return res
-
-        # logging.debug('<expandTemplates ' + str(len(self.frame)))
-
-        cur = 0
-        # look for matching {{...}}
-        for s, e in findMatchingBraces(wikitext, 2):
-            res += wikitext[cur:s] + self.expandTemplate(wikitext[s + 2:e - 2])
-            cur = e
-        # leftover
-        res += wikitext[cur:]
-        # logging.debug('   expandTemplates> %d %s', len(self.frame), res)
-        return res
-
-    def templateParams(self, parameters):
-        """
-        Build a dictionary with positional or name key to expanded parameters.
-        :param parameters: the parts[1:] of a template, i.e. all except the title.
-        """
-        templateParams = {}
-
-        if not parameters:
-            return templateParams
-        logging.debug('<templateParams: %s', '|'.join(parameters))
-
-        # Parameters can be either named or unnamed. In the latter case, their
-        # name is defined by their ordinal position (1, 2, 3, ...).
-
-        unnamedParameterCounter = 0
-
-        # It's legal for unnamed parameters to be skipped, in which case they
-        # will get default values (if available) during actual instantiation.
-        # That is {{template_name|a||c}} means parameter 1 gets
-        # the value 'a', parameter 2 value is not defined, and parameter 3 gets
-        # the value 'c'.  This case is correctly handled by function 'split',
-        # and does not require any special handling.
-        for param in parameters:
-            # Spaces before or after a parameter value are normally ignored,
-            # UNLESS the parameter contains a link (to prevent possible gluing
-            # the link to the following text after template substitution)
-
-            # Parameter values may contain "=" symbols, hence the parameter
-            # name extends up to the first such symbol.
-
-            # It is legal for a parameter to be specified several times, in
-            # which case the last assignment takes precedence. Example:
-            # "{{t|a|b|c|2=B}}" is equivalent to "{{t|a|B|c}}".
-            # Therefore, we don't check if the parameter has been assigned a
-            # value before, because anyway the last assignment should override
-            # any previous ones.
-            # FIXME: Don't use DOTALL here since parameters may be tags with
-            # attributes, e.g. <div class="templatequotecite">
-            # Parameters may span several lines, like:
-            # {{Reflist|colwidth=30em|refs=
-            # &lt;ref name=&quot;Goode&quot;&gt;Title&lt;/ref&gt;
-
-            # The '=' might occurr within an HTML attribute:
-            #   "&lt;ref name=value"
-            # but we stop at first.
-
-            # The '=' might occurr within quotes:
-            # ''''<span lang="pt-pt" xml:lang="pt-pt">cénicas</span>'''
-
-            m = re.match(" *([^=']*?) *=(.*)", param, re.DOTALL)
-            if m:
-                # This is a named parameter.  This case also handles parameter
-                # assignments like "2=xxx", where the number of an unnamed
-                # parameter ("2") is specified explicitly - this is handled
-                # transparently.
-
-                parameterName = m.group(1).strip()
-                parameterValue = m.group(2)
-
-                if ']]' not in parameterValue:  # if the value does not contain a link, trim whitespace
-                    parameterValue = parameterValue.strip()
-                templateParams[parameterName] = parameterValue
-            else:
-                # this is an unnamed parameter
-                unnamedParameterCounter += 1
-
-                if ']]' not in param:  # if the value does not contain a link, trim whitespace
-                    param = param.strip()
-                templateParams[str(unnamedParameterCounter)] = param
-        logging.debug('   templateParams> %s', '|'.join(templateParams.values()))
-        return templateParams
-
-    def expandTemplate(self, body):
-        """Expands template invocation.
-        :param body: the parts of a template.
-
-        :see http://meta.wikimedia.org/wiki/Help:Expansion for an explanation
-        of the process.
-
-        See in particular: Expansion of names and values
-        http://meta.wikimedia.org/wiki/Help:Expansion#Expansion_of_names_and_values
-
-        For most parser functions all names and values are expanded,
-        regardless of what is relevant for the result. The branching functions
-        (#if, #ifeq, #iferror, #ifexist, #ifexpr, #switch) are exceptions.
-
-        All names in a template call are expanded, and the titles of the
-        tplargs in the template body, after which it is determined which
-        values must be expanded, and for which tplargs in the template body
-        the first part (default).
-
-        In the case of a tplarg, any parts beyond the first are never
-        expanded.  The possible name and the value of the first part is
-        expanded if the title does not match a name in the template call.
-
-        :see code for braceSubstitution at
-        https://doc.wikimedia.org/mediawiki-core/master/php/html/Parser_8php_source.html#3397:
-
-        """
-
-        # template        = "{{" parts "}}"
-
-        # Templates and tplargs are decomposed in the same way, with pipes as
-        # separator, even though eventually any parts in a tplarg after the first
-        # (the parameter default) are ignored, and an equals sign in the first
-        # part is treated as plain text.
-        # Pipes inside inner templates and tplargs, or inside double rectangular
-        # brackets within the template or tplargs are not taken into account in
-        # this decomposition.
-        # The first part is called title, the other parts are simply called parts.
-
-        # If a part has one or more equals signs in it, the first equals sign
-        # determines the division into name = value. Equals signs inside inner
-        # templates and tplargs, or inside double rectangular brackets within the
-        # part are not taken into account in this decomposition. Parts without
-        # equals sign are indexed 1, 2, .., given as attribute in the <name> tag.
-
-        if len(self.frame) >= self.maxTemplateRecursionLevels:
-            self.recursion_exceeded_2_errs += 1
-            # logging.debug('   INVOCATION> %d %s', len(self.frame), body)
-            return ''
-
-        logging.debug('INVOCATION %d %s', len(self.frame), body)
-
-        parts = splitParts(body)
-        # title is the portion before the first |
-        logging.debug('TITLE %s', parts[0].strip())
-        title = self.expandTemplates(parts[0].strip())
-
-        # SUBST
-        # Apply the template tag to parameters without
-        # substituting into them, e.g.
-        # {{subst:t|a{{{p|q}}}b}} gives the wikitext start-a{{{p|q}}}b-end
-        # @see https://www.mediawiki.org/wiki/Manual:Substitution#Partial_substitution
-        subst = False
-        if re.match(substWords, title, re.IGNORECASE):
-            title = re.sub(substWords, '', title, 1, re.IGNORECASE)
-            subst = True
-
-        if title.lower() in self.magicWords.values:
-            return self.magicWords[title.lower()]
-
-        # Parser functions
-        # The first argument is everything after the first colon.
-        # It has been evaluated above.
-        colon = title.find(':')
-        if colon > 1:
-            funct = title[:colon]
-            parts[0] = title[colon + 1:].strip()  # side-effect (parts[0] not used later)
-            # arguments after first are not evaluated
-            ret = callParserFunction(funct, parts, self.frame)
-            return self.expandTemplates(ret)
-
-        title = fullyQualifiedTemplateTitle(title)
-        if not title:
-            self.template_title_errs += 1
-            return ''
-
-        redirected = redirects.get(title)
-        if redirected:
-            title = redirected
-
-        # get the template
-        if title in templateCache:
-            template = templateCache[title]
-        elif title in templates:
-            template = Template.parse(templates[title])
-            # add it to cache
-            templateCache[title] = template
-            del templates[title]
-        else:
-            # The page being included could not be identified
-            return ''
-
-        # logging.debug('TEMPLATE %s: %s', title, template)
-
-        # tplarg          = "{{{" parts "}}}"
-        # parts           = [ title *( "|" part ) ]
-        # part            = ( part-name "=" part-value ) / ( part-value )
-        # part-name       = wikitext-L3
-        # part-value      = wikitext-L3
-        # wikitext-L3     = literal / template / tplarg / link / comment /
-        #                   line-eating-comment / unclosed-comment /
-        #           	    xmlish-element / *wikitext-L3
-
-        # A tplarg may contain other parameters as well as templates, e.g.:
-        #   {{{text|{{{quote|{{{1|{{error|Error: No text given}}}}}}}}}}}
-        # hence no simple RE like this would work:
-        #   '{{{((?:(?!{{{).)*?)}}}'
-        # We must use full CF parsing.
-
-        # the parameter name itself might be computed, e.g.:
-        #   {{{appointe{{#if:{{{appointer14|}}}|r|d}}14|}}}
-
-        # Because of the multiple uses of double-brace and triple-brace
-        # syntax, expressions can sometimes be ambiguous.
-        # Precedence rules specifed here:
-        # http://www.mediawiki.org/wiki/Preprocessor_ABNF#Ideal_precedence
-        # resolve ambiguities like this:
-        #   {{{{ }}}} -> { {{{ }}} }
-        #   {{{{{ }}}}} -> {{ {{{ }}} }}
-        #
-        # :see: https://en.wikipedia.org/wiki/Help:Template#Handling_parameters
-
-        params = parts[1:]
-
-        if not subst:
-            # Evaluate parameters, since they may contain templates, including
-            # the symbol "=".
-            # {{#ifexpr: {{{1}}} = 1 }}
-            params = [self.expandTemplates(p) for p in params]
-
-        # build a dict of name-values for the parameter values
-        params = self.templateParams(params)
-
-        # Perform parameter substitution
-        # extend frame before subst, since there may be recursion in default
-        # parameter value, e.g. {{OTRS|celebrative|date=April 2015}} in article
-        # 21637542 in enwiki.
-        self.frame.append((title, params))
-        instantiated = template.subst(params, self)
-        # logging.debug('instantiated %d %s', len(self.frame), instantiated)
-        value = self.expandTemplates(instantiated)
-        self.frame.pop()
-        # logging.debug('   INVOCATION> %s %d %s', title, len(self.frame), value)
-        return value
-
-
-# ----------------------------------------------------------------------
-# parameter handling
-
-
-def splitParts(paramsList):
-    """
-    :param paramsList: the parts of a template or tplarg.
-
-    Split template parameters at the separator "|".
-    separator "=".
-
-    Template parameters often contain URLs, internal links, text or even
-    template expressions, since we evaluate templates outside in.
-    This is required for cases like:
-      {{#if: {{{1}}} | {{lc:{{{1}}} | "parameter missing"}}
-    Parameters are separated by "|" symbols. However, we
-    cannot simply split the string on "|" symbols, since these
-    also appear inside templates and internal links, e.g.
-
-     {{if:|
-      |{{#if:the president|
-           |{{#if:|
-               [[Category:Hatnote templates|A{{PAGENAME}}]]
-            }}
-       }}
-     }}
-
-    We split parts at the "|" symbols that are not inside any pair
-    {{{...}}}, {{...}}, [[...]], {|...|}.
-    """
-
-    # Must consider '[' as normal in expansion of Template:EMedicine2:
-    # #ifeq: ped|article|[http://emedicine.medscape.com/article/180-overview|[http://www.emedicine.com/ped/topic180.htm#{{#if: |section~}}
-    # as part of:
-    # {{#ifeq: ped|article|[http://emedicine.medscape.com/article/180-overview|[http://www.emedicine.com/ped/topic180.htm#{{#if: |section~}}}} ped/180{{#if: |~}}]
-
-    # should handle both tpl arg like:
-    #    4|{{{{{subst|}}}CURRENTYEAR}}
-    # and tpl parameters like:
-    #    ||[[Category:People|{{#if:A|A|{{PAGENAME}}}}]]
-
-    sep = '|'
-    parameters = []
-    cur = 0
-    for s, e in findMatchingBraces(paramsList):
-        par = paramsList[cur:s].split(sep)
-        if par:
-            if parameters:
-                # portion before | belongs to previous parameter
-                parameters[-1] += par[0]
-                if len(par) > 1:
-                    # rest are new parameters
-                    parameters.extend(par[1:])
-            else:
-                parameters = par
-        elif not parameters:
-            parameters = ['']  # create first param
-        # add span to last previous parameter
-        parameters[-1] += paramsList[s:e]
-        cur = e
-    # leftover
-    par = paramsList[cur:].split(sep)
-    if par:
-        if parameters:
-            # portion before | belongs to previous parameter
-            parameters[-1] += par[0]
-            if len(par) > 1:
-                # rest are new parameters
-                parameters.extend(par[1:])
-        else:
-            parameters = par
-
-    # logging.debug('splitParts %s %s\nparams: %s', sep, paramsList, str(parameters))
-    return parameters
-
-
-def findMatchingBraces(text, ldelim=0):
-    """
-    :param ldelim: number of braces to match. 0 means match [[]], {{}} and {{{}}}.
-    """
-    # Parsing is done with respect to pairs of double braces {{..}} delimiting
-    # a template, and pairs of triple braces {{{..}}} delimiting a tplarg.
-    # If double opening braces are followed by triple closing braces or
-    # conversely, this is taken as delimiting a template, with one left-over
-    # brace outside it, taken as plain text. For any pattern of braces this
-    # defines a set of templates and tplargs such that any two are either
-    # separate or nested (not overlapping).
-
-    # Unmatched double rectangular closing brackets can be in a template or
-    # tplarg, but unmatched double rectangular opening brackets cannot.
-    # Unmatched double or triple closing braces inside a pair of
-    # double rectangular brackets are treated as plain text.
-    # Other formulation: in ambiguity between template or tplarg on one hand,
-    # and a link on the other hand, the structure with the rightmost opening
-    # takes precedence, even if this is the opening of a link without any
-    # closing, so not producing an actual link.
-
-    # In the case of more than three opening braces the last three are assumed
-    # to belong to a tplarg, unless there is no matching triple of closing
-    # braces, in which case the last two opening braces are are assumed to
-    # belong to a template.
-
-    # We must skip individual { like in:
-    #   {{#ifeq: {{padleft:|1|}} | { | | &nbsp;}}
-    # We must resolve ambiguities like this:
-    #   {{{{ }}}} -> { {{{ }}} }
-    #   {{{{{ }}}}} -> {{ {{{ }}} }}
-    #   {{#if:{{{{{#if:{{{nominee|}}}|nominee|candidate}}|}}}|...}}
-
-    # Handle:
-    #   {{{{{|safesubst:}}}#Invoke:String|replace|{{{1|{{{{{|safesubst:}}}PAGENAME}}}}}|%s+%([^%(]-%)$||plain=false}}
-    # as well as expressions with stray }:
-    #   {{{link|{{ucfirst:{{{1}}}}}} interchange}}}
-
-    if ldelim:  # 2-3
-        reOpen = re.compile('[{]{%d,}' % ldelim)  # at least ldelim
-        reNext = re.compile('[{]{2,}|}{2,}')  # at least 2 open or close bracces
-    else:
-        reOpen = re.compile('{{2,}|\[{2,}')
-        reNext = re.compile('{{2,}|}{2,}|\[{2,}|]{2,}')  # at least 2
-
-    cur = 0
-    while True:
-        m1 = reOpen.search(text, cur)
-        if not m1:
-            return
-        lmatch = m1.end() - m1.start()
-        if m1.group()[0] == '{':
-            stack = [lmatch]  # stack of opening braces lengths
-        else:
-            stack = [-lmatch]  # negative means [
-        end = m1.end()
-        while True:
-            m2 = reNext.search(text, end)
-            if not m2:
-                return  # unbalanced
-            end = m2.end()
-            brac = m2.group()[0]
-            lmatch = m2.end() - m2.start()
-
-            if brac == '{':
-                stack.append(lmatch)
-            elif brac == '}':
-                while stack:
-                    openCount = stack.pop()  # opening span
-                    if openCount == 0:  # illegal unmatched [[
-                        continue
-                    if lmatch >= openCount:
-                        lmatch -= openCount
-                        if lmatch <= 1:  # either close or stray }
-                            break
-                    else:
-                        # put back unmatched
-                        stack.append(openCount - lmatch)
-                        break
-                if not stack:
-                    yield m1.start(), end - lmatch
-                    cur = end
-                    break
-                elif len(stack) == 1 and 0 < stack[0] < ldelim:
-                    # ambiguous {{{{{ }}} }}
-                    yield m1.start() + stack[0], end
-                    cur = end
-                    break
-            elif brac == '[':  # [[
-                stack.append(-lmatch)
-            else:  # ]]
-                while stack and stack[-1] < 0:  # matching [[
-                    openCount = -stack.pop()
-                    if lmatch >= openCount:
-                        lmatch -= openCount
-                        if lmatch <= 1:  # either close or stray ]
-                            break
-                    else:
-                        # put back unmatched (negative)
-                        stack.append(lmatch - openCount)
-                        break
-                if not stack:
-                    yield m1.start(), end - lmatch
-                    cur = end
-                    break
-                # unmatched ]] are discarded
-                cur = end
-
-
-def findBalanced(text, openDelim, closeDelim):
-    """
-    Assuming that text contains a properly balanced expression using
-    :param openDelim: as opening delimiters and
-    :param closeDelim: as closing delimiters.
-    :return: an iterator producing pairs (start, end) of start and end
-    positions in text containing a balanced expression.
-    """
-    openPat = '|'.join([re.escape(x) for x in openDelim])
-    # patter for delimiters expected after each opening delimiter
-    afterPat = {o: re.compile(openPat + '|' + c, re.DOTALL) for o, c in zip(openDelim, closeDelim)}
-    stack = []
-    start = 0
-    cur = 0
-    # end = len(text)
-    startSet = False
-    startPat = re.compile(openPat)
-    nextPat = startPat
-    while True:
-        next = nextPat.search(text, cur)
-        if not next:
-            return
-        if not startSet:
-            start = next.start()
-            startSet = True
-        delim = next.group(0)
-        if delim in openDelim:
-            stack.append(delim)
-            nextPat = afterPat[delim]
-        else:
-            opening = stack.pop()
-            # assert opening == openDelim[closeDelim.index(next.group(0))]
-            if stack:
-                nextPat = afterPat[stack[-1]]
-            else:
-                yield start, next.end()
-                nextPat = startPat
-                start = next.end()
-                startSet = False
-        cur = next.end()
-
-# ----------------------------------------------------------------------
-# parser functions utilities
-
-
-def ucfirst(string):
-    """:return: a string with just its first character uppercase
-    We can't use title() since it coverts all words.
-    """
-    if string:
-        if len(string) > 1:
-            return string[0].upper() + string[1:]
-        else:
-            return string.upper()
-    else:
-        return ''
-
-
-def lcfirst(string):
-    """:return: a string with its first character lowercase"""
-    if string:
-        if len(string) > 1:
-            return string[0].lower() + string[1:]
-        else:
-            return string.lower()
-    else:
-        return ''
-
-
-def fullyQualifiedTemplateTitle(templateTitle):
-    """
-    Determine the namespace of the page being included through the template
-    mechanism
-    """
-    if templateTitle.startswith(':'):
-        # Leading colon by itself implies main namespace, so strip this colon
-        return ucfirst(templateTitle[1:])
-    else:
-        m = re.match('([^:]*)(:.*)', templateTitle)
-        if m:
-            # colon found but not in the first position - check if it
-            # designates a known namespace
-            prefix = normalizeNamespace(m.group(1))
-            if prefix in knownNamespaces:
-                return prefix + ucfirst(m.group(2))
-    # The title of the page being included is NOT in the main namespace and
-    # lacks any other explicit designation of the namespace - therefore, it
-    # is resolved to the Template namespace (that's the default for the
-    # template inclusion mechanism).
-
-    # This is a defense against pages whose title only contains UTF-8 chars
-    # that are reduced to an empty string. Right now I can think of one such
-    # case - <C2><A0> which represents the non-breaking space.
-    # In this particular case, this page is a redirect to [[Non-nreaking
-    # space]], but having in the system a redirect page with an empty title
-    # causes numerous problems, so we'll live happier without it.
-    if templateTitle:
-        return Extractor.templatePrefix + ucfirst(templateTitle)
-    else:
-        return ''  # caller may log as error
-
-
-def normalizeNamespace(ns):
-    return ucfirst(ns)
-
-
-# ----------------------------------------------------------------------
-# Parser functions
-# see http://www.mediawiki.org/wiki/Help:Extension:ParserFunctions
-# https://github.com/Wikia/app/blob/dev/extensions/ParserFunctions/ParserFunctions_body.php
-
-
-class Infix():
-
-    """Infix operators.
-    The calling sequence for the infix is:
-      x |op| y
-    """
-
-    def __init__(self, function):
-        self.function = function
-
-    def __ror__(self, other):
-        return Infix(lambda x, self=self, other=other: self.function(other, x))
-
-    def __or__(self, other):
-        return self.function(other)
-
-    def __rlshift__(self, other):
-        return Infix(lambda x, self=self, other=other: self.function(other, x))
-
-    def __rshift__(self, other):
-        return self.function(other)
-
-    def __call__(self, value1, value2):
-        return self.function(value1, value2)
-
-
-ROUND = Infix(lambda x, y: round(x, y))
-
-
-def sharp_expr(expr):
-    try:
-        expr = re.sub('=', '==', expr)
-        expr = re.sub('mod', '%', expr)
-        expr = re.sub('\bdiv\b', '/', expr)
-        expr = re.sub('\bround\b', '|ROUND|', expr)
-        return str(eval(expr))
-    except:
-        return '<span class="error"></span>'
-
-
-def sharp_if(testValue, valueIfTrue, valueIfFalse=None, *args):
-    # In theory, we should evaluate the first argument here,
-    # but it was evaluated while evaluating part[0] in expandTemplate().
-    if testValue.strip():
-        # The {{#if:}} function is an if-then-else construct.
-        # The applied condition is: "The condition string is non-empty".
-        valueIfTrue = valueIfTrue.strip()
-        if valueIfTrue:
-            return valueIfTrue
-    elif valueIfFalse:
-        return valueIfFalse.strip()
-    return ""
-
-
-def sharp_ifeq(lvalue, rvalue, valueIfTrue, valueIfFalse=None, *args):
-    rvalue = rvalue.strip()
-    if rvalue:
-        # lvalue is always defined
-        if lvalue.strip() == rvalue:
-            # The {{#ifeq:}} function is an if-then-else construct. The
-            # applied condition is "is rvalue equal to lvalue". Note that this
-            # does only string comparison while MediaWiki implementation also
-            # supports numerical comparissons.
-
-            if valueIfTrue:
-                return valueIfTrue.strip()
-        else:
-            if valueIfFalse:
-                return valueIfFalse.strip()
-    return ""
-
-
-def sharp_iferror(test, then='', Else=None, *args):
-    if re.match('<(?:strong|span|p|div)\s(?:[^\s>]*\s+)*?class="(?:[^"\s>]*\s+)*?error(?:\s[^">]*)?"', test):
-        return then
-    elif Else is None:
-        return test.strip()
-    else:
-        return Else.strip()
-
-
-def sharp_switch(primary, *params):
-    # FIXME: we don't support numeric expressions in primary
-
-    # {{#switch: comparison string
-    #  | case1 = result1
-    #  | case2
-    #  | case4 = result2
-    #  | 1 | case5 = result3
-    #  | #default = result4
-    # }}
-
-    primary = primary.strip()
-    found = False  # for fall through cases
-    default = None
-    rvalue = None
-    lvalue = ''
-    for param in params:
-        # handle cases like:
-        #  #default = [http://www.perseus.tufts.edu/hopper/text?doc=Perseus...]
-        pair = param.split('=', 1)
-        lvalue = pair[0].strip()
-        rvalue = None
-        if len(pair) > 1:
-            # got "="
-            rvalue = pair[1].strip()
-            # check for any of multiple values pipe separated
-            if found or primary in [v.strip() for v in lvalue.split('|')]:
-                # Found a match, return now
-                return rvalue
-            elif lvalue == '#default':
-                default = rvalue
-            rvalue = None  # avoid defaulting to last case
-        elif lvalue == primary:
-            # If the value matches, set a flag and continue
-            found = True
-    # Default case
-    # Check if the last item had no = sign, thus specifying the default case
-    if rvalue is not None:
-        return lvalue
-    elif default is not None:
-        return default
-    return ''
-
-
-# Extension Scribuntu
-def sharp_invoke(module, function, frame):
-    functions = modules.get(module)
-    if functions:
-        funct = functions.get(function)
-        if funct:
-            # find parameters in frame whose title is the one of the original
-            # template invocation
-            templateTitle = fullyQualifiedTemplateTitle(function)
-            if not templateTitle:
-                logging.warn("Template with empty title")
-            pair = next((x for x in frame if x[0] == templateTitle), None)
-            if pair:
-                params = pair[1]
-                # extract positional args
-                params = [params.get(str(i + 1)) for i in range(len(params))]
-                return funct(*params)
-            else:
-                return funct()
-    return ''
-
-
-parserFunctions = {
-
-    '#expr': sharp_expr,
-
-    '#if': sharp_if,
-
-    '#ifeq': sharp_ifeq,
-
-    '#iferror': sharp_iferror,
-
-    '#ifexpr': lambda *args: '',  # not supported
-
-    '#ifexist': lambda *args: '',  # not supported
-
-    '#rel2abs': lambda *args: '',  # not supported
-
-    '#switch': sharp_switch,
-
-    '# language': lambda *args: '',  # not supported
-
-    '#time': lambda *args: '',  # not supported
-
-    '#timel': lambda *args: '',  # not supported
-
-    '#titleparts': lambda *args: '',  # not supported
-
-    # This function is used in some pages to construct links
-    # http://meta.wikimedia.org/wiki/Help:URL
-    'urlencode': lambda string, *rest: urlencode(string),
-
-    'lc': lambda string, *rest: string.lower() if string else '',
-
-    'lcfirst': lambda string, *rest: lcfirst(string),
-
-    'uc': lambda string, *rest: string.upper() if string else '',
-
-    'ucfirst': lambda string, *rest: ucfirst(string),
-
-    'int': lambda string, *rest: str(int(string)),
-
-    'padleft': lambda char, width, string: string.ljust(char, int(pad)), # CHECK_ME
-
-}
-
-
-def callParserFunction(functionName, args, frame):
-    """
-    Parser functions have similar syntax as templates, except that
-    the first argument is everything after the first colon.
-    :param functionName: nameof the parser function
-    :param args: the arguments to the function
-    :return: the result of the invocation, None in case of failure.
-
-    http://meta.wikimedia.org/wiki/Help:ParserFunctions
-    """
-
-    try:
-        if functionName == '#invoke':
-            # special handling of frame
-            ret = sharp_invoke(args[0].strip(), args[1].strip(), frame)
-            # logging.debug('parserFunction> %s %s', args[1], ret)
-            return ret
-        if functionName in parserFunctions:
-            ret = parserFunctions[functionName](*args)
-            # logging.debug('parserFunction> %s(%s) %s', functionName, args, ret)
-            return ret
-    except:
-        return ""  # FIXME: fix errors
-
-    return ""
-
-
-# ----------------------------------------------------------------------
-# Extract Template definition
-
-reNoinclude = re.compile(r'<noinclude>(?:.*?)</noinclude>', re.DOTALL)
-reIncludeonly = re.compile(r'<includeonly>|</includeonly>', re.DOTALL)
-
-# These are built before spawning processes, hence they are shared.
-templates = {}
-redirects = {}
-# cache of parser templates
-# FIXME: sharing this with a Manager slows down.
-templateCache = {}
-
-
-def define_template(title, page):
-    """
-    Adds a template defined in the :param page:.
-    @see https://en.wikipedia.org/wiki/Help:Template#Noinclude.2C_includeonly.2C_and_onlyinclude
-    """
-    global templates
-    global redirects
-
-    # title = normalizeTitle(title)
-
-    # check for redirects
-    m = re.match('#REDIRECT.*?\[\[([^\]]*)]]', page[0], re.IGNORECASE)
-    if m:
-        redirects[title] = m.group(1)  # normalizeTitle(m.group(1))
-        return
-
-    text = unescape(''.join(page))
-
-    # We're storing template text for future inclusion, therefore,
-    # remove all <noinclude> text and keep all <includeonly> text
-    # (but eliminate <includeonly> tags per se).
-    # However, if <onlyinclude> ... </onlyinclude> parts are present,
-    # then only keep them and discard the rest of the template body.
-    # This is because using <onlyinclude> on a text fragment is
-    # equivalent to enclosing it in <includeonly> tags **AND**
-    # enclosing all the rest of the template body in <noinclude> tags.
-
-    # remove comments
-    text = comment.sub('', text)
-
-    # eliminate <noinclude> fragments
-    text = reNoinclude.sub('', text)
-    # eliminate unterminated <noinclude> elements
-    text = re.sub(r'<noinclude\s*>.*$', '', text, flags=re.DOTALL)
-    text = re.sub(r'<noinclude/>', '', text)
-
-    onlyincludeAccumulator = ''
-    for m in re.finditer('<onlyinclude>(.*?)</onlyinclude>', text, re.DOTALL):
-        onlyincludeAccumulator += m.group(1)
-    if onlyincludeAccumulator:
-        text = onlyincludeAccumulator
-    else:
-        text = reIncludeonly.sub('', text)
-
-    if text:
-        if title in templates and templates[title] != text:
-            logging.warn('Redefining: %s', title)
-        templates[title] = text
+# -*- coding: utf-8 -*-
+
+# =============================================================================
+#  Copyright (c) 2020. Giuseppe Attardi (attardi@di.unipi.it).
+# =============================================================================
+#  This file is part of Tanl.
+#
+#  Tanl is free software; you can redistribute it and/or modify it
+#  under the terms of the GNU Affero General Public License, version 3,
+#  as published by the Free Software Foundation.
+#
+#  Tanl is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Affero General Public License for more details.
+#
+#  You should have received a copy of the GNU Affero General Public License
+#  along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# =============================================================================
+
+import re
+import html
+import json
+from itertools import zip_longest
+from urllib.parse import quote as urlencode
+from html.entities import name2codepoint
+import logging
+import time
+
+# ----------------------------------------------------------------------
+
+# match tail after wikilink
+tailRE = re.compile('\w+')
+syntaxhighlight = re.compile('&lt;syntaxhighlight .*?&gt;(.*?)&lt;/syntaxhighlight&gt;', re.DOTALL)
+
+## PARAMS ####################################################################
+
+##
+# Defined in <siteinfo>
+# We include as default Template, when loading external template file.
+knownNamespaces = set(['Template'])
+
+##
+# Drop these elements from article text
+#
+discardElements = [
+    'gallery', 'timeline', 'noinclude', 'pre',
+    'table', 'tr', 'td', 'th', 'caption', 'div',
+    'form', 'input', 'select', 'option', 'textarea',
+    'ul', 'li', 'ol', 'dl', 'dt', 'dd', 'menu', 'dir',
+    'ref', 'references', 'img', 'imagemap', 'source', 'small'
+]
+
+##
+# Recognize only these namespaces
+# w: Internal links to the Wikipedia
+# wiktionary: Wiki dictionary
+# wikt: shortcut for Wiktionary
+#
+acceptedNamespaces = ['w', 'wiktionary', 'wikt']
+
+
+def get_url(urlbase, uid):
+    return "%s?curid=%s" % (urlbase, uid)
+
+
+# ======================================================================
+
+
+def clean(extractor, text, expand_templates=False, html_safe=True):
+    """
+    Transforms wiki markup. If the command line flag --escapedoc is set then the text is also escaped
+    @see https://www.mediawiki.org/wiki/Help:Formatting
+    :param extractor: the Extractor t use.
+    :param text: the text to clean.
+    :param expand_templates: whether to perform template expansion.
+    :param html_safe: whether to convert reserved HTML characters to entities.
+    @return: the cleaned text.
+    """
+
+    if expand_templates:
+        # expand templates
+        # See: http://www.mediawiki.org/wiki/Help:Templates
+        text = extractor.expandTemplates(text)
+    else:
+        # Drop transclusions (template, parser functions)
+        text = dropNested(text, r'{{', r'}}')
+
+    # Drop tables
+    text = dropNested(text, r'{\|', r'\|}')
+
+    # replace external links
+    text = replaceExternalLinks(text)
+
+    # replace internal links
+    text = replaceInternalLinks(text)
+
+    # drop MagicWords behavioral switches
+    text = magicWordsRE.sub('', text)
+
+    # ############### Process HTML ###############
+
+    # turn into HTML, except for the content of <syntaxhighlight>
+    res = ''
+    cur = 0
+    for m in syntaxhighlight.finditer(text):
+        end = m.end()
+        res += unescape(text[cur:m.start()]) + m.group(1)
+        cur = end
+    text = res + unescape(text[cur:])
+
+    # Handle bold/italic/quote
+    if extractor.HtmlFormatting:
+        text = bold_italic.sub(r'<b>\1</b>', text)
+        text = bold.sub(r'<b>\1</b>', text)
+        text = italic.sub(r'<i>\1</i>', text)
+    else:
+        text = bold_italic.sub(r'\1', text)
+        text = bold.sub(r'\1', text)
+        text = italic_quote.sub(r'"\1"', text)
+        text = italic.sub(r'"\1"', text)
+        text = quote_quote.sub(r'"\1"', text)
+    # residuals of unbalanced quotes
+    text = text.replace("'''", '').replace("''", '"')
+
+    # Collect spans
+
+    spans = []
+    # Drop HTML comments
+    for m in comment.finditer(text):
+        spans.append((m.start(), m.end()))
+
+    # Drop self-closing tags
+    for pattern in selfClosing_tag_patterns:
+        for m in pattern.finditer(text):
+            spans.append((m.start(), m.end()))
+
+    # Drop ignored tags
+    for left, right in ignored_tag_patterns:
+        for m in left.finditer(text):
+            spans.append((m.start(), m.end()))
+        for m in right.finditer(text):
+            spans.append((m.start(), m.end()))
+
+    # Bulk remove all spans
+    text = dropSpans(spans, text)
+
+    # Drop discarded elements
+    for tag in discardElements:
+        text = dropNested(text, r'<\s*%s\b[^>/]*>' % tag, r'<\s*/\s*%s>' % tag)
+
+    if not extractor.HtmlFormatting:
+        # Turn into text what is left (&amp;nbsp;) and <syntaxhighlight>
+        text = unescape(text)
+
+    # Expand placeholders
+    for pattern, placeholder in placeholder_tag_patterns:
+        index = 1
+        for match in pattern.finditer(text):
+            text = text.replace(match.group(), '%s_%d' % (placeholder, index))
+            index += 1
+
+    text = text.replace('<<', u'«').replace('>>', u'»')
+
+    #############################################
+
+    # Cleanup text
+    text = text.replace('\t', ' ')
+    text = spaces.sub(' ', text)
+    text = dots.sub('...', text)
+    text = re.sub(u' (,:\.\)\]»)', r'\1', text)
+    text = re.sub(u'(\[\(«) ', r'\1', text)
+    text = re.sub(r'\n\W+?\n', '\n', text, flags=re.U)  # lines with only punctuations
+    text = text.replace(',,', ',').replace(',.', '.')
+    if html_safe:
+        text = html.escape(text, quote=False)
+    return text
+
+
+# skip level 1, it is page name level
+section = re.compile(r'(==+)\s*(.*?)\s*\1')
+
+listOpen = {'*': '<ul>', '#': '<ol>', ';': '<dl>', ':': '<dl>'}
+listClose = {'*': '</ul>', '#': '</ol>', ';': '</dl>', ':': '</dl>'}
+listItem = {'*': '<li>%s</li>', '#': '<li>%s</<li>', ';': '<dt>%s</dt>',
+            ':': '<dd>%s</dd>'}
+
+
+def compact(text, mark_headers=False):
+    """Deal with headers, lists, empty sections, residuals of tables.
+    :param text: convert to HTML
+    """
+
+    page = []  # list of paragraph
+    headers = {}  # Headers for unfilled sections
+    emptySection = False  # empty sections are discarded
+    listLevel = ''  # nesting of lists
+
+    for line in text.split('\n'):
+
+        if not line:
+            if len(listLevel):    # implies Extractor.HtmlFormatting
+                for c in reversed(listLevel):
+                    page.append(listClose[c])
+                    listLevel = ''
+            continue
+
+        # Handle section titles
+        m = section.match(line)
+        if m:
+            title = m.group(2)
+            lev = len(m.group(1))
+            if Extractor.HtmlFormatting:
+                page.append("<h%d>%s</h%d>" % (lev, title, lev))
+            if title and title[-1] not in '!?':
+                title += '.'
+
+            if mark_headers:
+                title = "## " + title
+
+            headers[lev] = title
+            # drop previous headers
+            headers = { k:v for k,v in headers.items() if k <= lev }
+            emptySection = True
+            continue
+        # Handle page title
+        if line.startswith('++'):
+            title = line[2:-2]
+            if title:
+                if title[-1] not in '!?':
+                    title += '.'
+                page.append(title)
+        # handle indents
+        elif line[0] == ':':
+            page.append(line.lstrip(':'))
+        # handle lists
+        # @see https://www.mediawiki.org/wiki/Help:Formatting
+        elif line[0] in '*#;':
+            if Extractor.HtmlFormatting:
+                # close extra levels
+                l = 0
+                for c in listLevel:
+                    if l < len(line) and c != line[l]:
+                        for extra in reversed(listLevel[l:]):
+                            page.append(listClose[extra])
+                        listLevel = listLevel[:l]
+                        break
+                    l += 1
+                if l < len(line) and line[l] in '*#;:':
+                    # add new level (only one, no jumps)
+                    # FIXME: handle jumping levels
+                    type = line[l]
+                    page.append(listOpen[type])
+                    listLevel += type
+                    line = line[l+1:].strip()
+                else:
+                    # continue on same level
+                    type = line[l-1]
+                    line = line[l:].strip()
+                page.append(listItem[type] % line)
+            else:
+                continue
+        elif len(listLevel):    # implies Extractor.HtmlFormatting
+            for c in reversed(listLevel):
+                page.append(listClose[c])
+            listLevel = []
+
+        # Drop residuals of lists
+        elif line[0] in '{|' or line[-1] == '}':
+            continue
+        # Drop irrelevant lines
+        elif (line[0] == '(' and line[-1] == ')') or line.strip('.-') == '':
+            continue
+        elif len(headers):
+            if Extractor.keepSections:
+                items = sorted(headers.items())
+                for (i, v) in items:
+                    page.append(v)
+            headers.clear()
+            page.append(line)  # first line
+            emptySection = False
+        elif not emptySection:
+            page.append(line)
+            # dangerous
+            # # Drop preformatted
+            # elif line[0] == ' ':
+            #     continue
+
+    return page
+
+
+# ----------------------------------------------------------------------
+
+def dropNested(text, openDelim, closeDelim):
+    """
+    A matching function for nested expressions, e.g. namespaces and tables.
+    """
+    openRE = re.compile(openDelim, re.IGNORECASE)
+    closeRE = re.compile(closeDelim, re.IGNORECASE)
+    # partition text in separate blocks { } { }
+    spans = []  # pairs (s, e) for each partition
+    nest = 0  # nesting level
+    start = openRE.search(text, 0)
+    if not start:
+        return text
+    end = closeRE.search(text, start.end())
+    next = start
+    while end:
+        next = openRE.search(text, next.end())
+        if not next:  # termination
+            while nest:  # close all pending
+                nest -= 1
+                end0 = closeRE.search(text, end.end())
+                if end0:
+                    end = end0
+                else:
+                    break
+            spans.append((start.start(), end.end()))
+            break
+        while end.end() < next.start():
+            # { } {
+            if nest:
+                nest -= 1
+                # try closing more
+                last = end.end()
+                end = closeRE.search(text, end.end())
+                if not end:  # unbalanced
+                    if spans:
+                        span = (spans[0][0], last)
+                    else:
+                        span = (start.start(), last)
+                    spans = [span]
+                    break
+            else:
+                spans.append((start.start(), end.end()))
+                # advance start, find next close
+                start = next
+                end = closeRE.search(text, next.end())
+                break  # { }
+        if next != start:
+            # { { }
+            nest += 1
+    # collect text outside partitions
+    return dropSpans(spans, text)
+
+
+def dropSpans(spans, text):
+    """
+    Drop from text the blocks identified in :param spans:, possibly nested.
+    """
+    spans.sort()
+    res = ''
+    offset = 0
+    for s, e in spans:
+        if offset <= s:  # handle nesting
+            if offset < s:
+                res += text[offset:s]
+            offset = e
+    res += text[offset:]
+    return res
+
+
+# ----------------------------------------------------------------------
+# External links
+
+# from: https://doc.wikimedia.org/mediawiki-core/master/php/DefaultSettings_8php_source.html
+
+wgUrlProtocols = [
+    'bitcoin:', 'ftp://', 'ftps://', 'geo:', 'git://', 'gopher://', 'http://',
+    'https://', 'irc://', 'ircs://', 'magnet:', 'mailto:', 'mms://', 'news:',
+    'nntp://', 'redis://', 'sftp://', 'sip:', 'sips:', 'sms:', 'ssh://',
+    'svn://', 'tel:', 'telnet://', 'urn:', 'worldwind://', 'xmpp:', '//'
+]
+
+# from: https://doc.wikimedia.org/mediawiki-core/master/php/Parser_8php_source.html
+
+# Constants needed for external link processing
+# Everything except bracket, space, or control characters
+# \p{Zs} is unicode 'separator, space' category. It covers the space 0x20
+# as well as U+3000 is IDEOGRAPHIC SPACE for bug 19052
+EXT_LINK_URL_CLASS = r'[^][<>"\x00-\x20\x7F\s]'
+ExtLinkBracketedRegex = re.compile(
+    '(?i)\[((' + '|'.join(wgUrlProtocols) + ')' + EXT_LINK_URL_CLASS + r'+)\s*([^\]\x00-\x08\x0a-\x1F]*?)\]',
+    re.S | re.U)
+EXT_IMAGE_REGEX = re.compile(
+    r"""(?i)^(http://|https://)([^][<>"\x00-\x20\x7F\s]+)
+    /([A-Za-z0-9_.,~%\-+&;#*?!=()@\x80-\xFF]+)\.(gif|png|jpg|jpeg)$""",
+    re.X | re.S | re.U)
+
+
+def replaceExternalLinks(text):
+    s = ''
+    cur = 0
+    for m in ExtLinkBracketedRegex.finditer(text):
+        s += text[cur:m.start()]
+        cur = m.end()
+
+        url = m.group(1)
+        label = m.group(3)
+
+        # # The characters '<' and '>' (which were escaped by
+        # # removeHTMLtags()) should not be included in
+        # # URLs, per RFC 2396.
+        # m2 = re.search('&(lt|gt);', url)
+        # if m2:
+        #     link = url[m2.end():] + ' ' + link
+        #     url = url[0:m2.end()]
+
+        # If the link text is an image URL, replace it with an <img> tag
+        # This happened by accident in the original parser, but some people used it extensively
+        m = EXT_IMAGE_REGEX.match(label)
+        if m:
+            label = makeExternalImage(label)
+
+        # Use the encoded URL
+        # This means that users can paste URLs directly into the text
+        # Funny characters like ö aren't valid in URLs anyway
+        # This was changed in August 2004
+        s += makeExternalLink(url, label)  # + trail
+
+    return s + text[cur:]
+
+
+def makeExternalLink(url, anchor):
+    """Function applied to wikiLinks"""
+    if Extractor.keepLinks:
+        return '<a href="%s">%s</a>' % (urlencode(url), anchor)
+    else:
+        return anchor
+
+
+def makeExternalImage(url, alt=''):
+    if Extractor.keepLinks:
+        return '<img src="%s" alt="%s">' % (url, alt)
+    else:
+        return alt
+
+
+# ----------------------------------------------------------------------
+# WikiLinks
+# See https://www.mediawiki.org/wiki/Help:Links#Internal_links
+
+# Can be nested [[File:..|..[[..]]..|..]], [[Category:...]], etc.
+# Also: [[Help:IPA for Catalan|[andora]]]
+
+
+def replaceInternalLinks(text):
+    """
+    Replaces external links of the form:
+    [[title |...|label]]trail
+
+    with title concatenated with trail, when present, e.g. 's' for plural.
+    """
+    # call this after removal of external links, so we need not worry about
+    # triple closing ]]].
+    cur = 0
+    res = ''
+    for s, e in findBalanced(text, ['[['], [']]']):
+        m = tailRE.match(text, e)
+        if m:
+            trail = m.group(0)
+            end = m.end()
+        else:
+            trail = ''
+            end = e
+        inner = text[s + 2:e - 2]
+        # find first |
+        pipe = inner.find('|')
+        if pipe < 0:
+            title = inner
+            label = title
+        else:
+            title = inner[:pipe].rstrip()
+            # find last |
+            curp = pipe + 1
+            for s1, e1 in findBalanced(inner, ['[['], [']]']):
+                last = inner.rfind('|', curp, s1)
+                if last >= 0:
+                    pipe = last  # advance
+                curp = e1
+            label = inner[pipe + 1:].strip()
+        res += text[cur:s] + makeInternalLink(title, label) + trail
+        cur = end
+    return res + text[cur:]
+
+
+def makeInternalLink(title, label):
+    colon = title.find(':')
+    if colon > 0 and title[:colon] not in acceptedNamespaces:
+        return ''
+    if colon == 0:
+        # drop also :File:
+        colon2 = title.find(':', colon + 1)
+        if colon2 > 1 and title[colon + 1:colon2] not in acceptedNamespaces:
+            return ''
+    if Extractor.keepLinks:
+        return '<a href="%s">%s</a>' % (urlencode(title), label)
+    else:
+        return label
+
+
+# ----------------------------------------------------------------------
+# variables
+
+
+class MagicWords():
+
+    """
+    One copy in each Extractor.
+
+    @see https://doc.wikimedia.org/mediawiki-core/master/php/MagicWord_8php_source.html
+    """
+    names = [
+        '!',
+        'currentmonth',
+        'currentmonth1',
+        'currentmonthname',
+        'currentmonthnamegen',
+        'currentmonthabbrev',
+        'currentday',
+        'currentday2',
+        'currentdayname',
+        'currentyear',
+        'currenttime',
+        'currenthour',
+        'localmonth',
+        'localmonth1',
+        'localmonthname',
+        'localmonthnamegen',
+        'localmonthabbrev',
+        'localday',
+        'localday2',
+        'localdayname',
+        'localyear',
+        'localtime',
+        'localhour',
+        'numberofarticles',
+        'numberoffiles',
+        'numberofedits',
+        'articlepath',
+        'pageid',
+        'sitename',
+        'server',
+        'servername',
+        'scriptpath',
+        'stylepath',
+        'pagename',
+        'pagenamee',
+        'fullpagename',
+        'fullpagenamee',
+        'namespace',
+        'namespacee',
+        'namespacenumber',
+        'currentweek',
+        'currentdow',
+        'localweek',
+        'localdow',
+        'revisionid',
+        'revisionday',
+        'revisionday2',
+        'revisionmonth',
+        'revisionmonth1',
+        'revisionyear',
+        'revisiontimestamp',
+        'revisionuser',
+        'revisionsize',
+        'subpagename',
+        'subpagenamee',
+        'talkspace',
+        'talkspacee',
+        'subjectspace',
+        'subjectspacee',
+        'talkpagename',
+        'talkpagenamee',
+        'subjectpagename',
+        'subjectpagenamee',
+        'numberofusers',
+        'numberofactiveusers',
+        'numberofpages',
+        'currentversion',
+        'rootpagename',
+        'rootpagenamee',
+        'basepagename',
+        'basepagenamee',
+        'currenttimestamp',
+        'localtimestamp',
+        'directionmark',
+        'contentlanguage',
+        'numberofadmins',
+        'cascadingsources',
+    ]
+
+    def __init__(self):
+        self.values = {'!': '|'}
+
+    def __getitem__(self, name):
+        return self.values.get(name)
+
+    def __setitem__(self, name, value):
+        self.values[name] = value
+
+    switches = (
+        '__NOTOC__',
+        '__FORCETOC__',
+        '__TOC__',
+        '__TOC__',
+        '__NEWSECTIONLINK__',
+        '__NONEWSECTIONLINK__',
+        '__NOGALLERY__',
+        '__HIDDENCAT__',
+        '__NOCONTENTCONVERT__',
+        '__NOCC__',
+        '__NOTITLECONVERT__',
+        '__NOTC__',
+        '__START__',
+        '__END__',
+        '__INDEX__',
+        '__NOINDEX__',
+        '__STATICREDIRECT__',
+        '__DISAMBIG__'
+    )
+
+
+magicWordsRE = re.compile('|'.join(MagicWords.switches))
+
+
+# =========================================================================
+#
+# MediaWiki Markup Grammar
+# https://www.mediawiki.org/wiki/Preprocessor_ABNF
+
+# xml-char = %x9 / %xA / %xD / %x20-D7FF / %xE000-FFFD / %x10000-10FFFF
+# sptab = SP / HTAB
+
+# ; everything except ">" (%x3E)
+# attr-char = %x9 / %xA / %xD / %x20-3D / %x3F-D7FF / %xE000-FFFD / %x10000-10FFFF
+
+# literal         = *xml-char
+# title           = wikitext-L3
+# part-name       = wikitext-L3
+# part-value      = wikitext-L3
+# part            = ( part-name "=" part-value ) / ( part-value )
+# parts           = [ title *( "|" part ) ]
+# tplarg          = "{{{" parts "}}}"
+# template        = "{{" parts "}}"
+# link            = "[[" wikitext-L3 "]]"
+
+# comment         = "<!--" literal "-->"
+# unclosed-comment = "<!--" literal END
+# ; the + in the line-eating-comment rule was absent between MW 1.12 and MW 1.22
+# line-eating-comment = LF LINE-START *SP +( comment *SP ) LINE-END
+
+# attr            = *attr-char
+# nowiki-element  = "<nowiki" attr ( "/>" / ( ">" literal ( "</nowiki>" / END ) ) )
+
+# wikitext-L2     = heading / wikitext-L3 / *wikitext-L2
+# wikitext-L3     = literal / template / tplarg / link / comment /
+#                   line-eating-comment / unclosed-comment / xmlish-element /
+#                   *wikitext-L3
+
+# ------------------------------------------------------------------------------
+
+selfClosingTags = ('br', 'hr', 'nobr', 'ref', 'references', 'nowiki')
+
+# These tags are dropped, keeping their content.
+# handle 'a' separately, depending on keepLinks
+ignoredTags = (
+    'abbr', 'b', 'big', 'blockquote', 'center', 'cite', 'div', 'em',
+    'font', 'h1', 'h2', 'h3', 'h4', 'hiero', 'i', 'kbd', 'nowiki',
+    'p', 'plaintext', 's', 'span', 'strike', 'strong',
+    'sub', 'sup', 'tt', 'u', 'var'
+)
+
+placeholder_tags = {'math': 'formula', 'code': 'codice'}
+
+
+def normalizeTitle(title):
+    """Normalize title"""
+    # remove leading/trailing whitespace and underscores
+    title = title.strip(' _')
+    # replace sequences of whitespace and underscore chars with a single space
+    title = re.sub(r'[\s_]+', ' ', title)
+
+    m = re.match(r'([^:]*):(\s*)(\S(?:.*))', title)
+    if m:
+        prefix = m.group(1)
+        if m.group(2):
+            optionalWhitespace = ' '
+        else:
+            optionalWhitespace = ''
+        rest = m.group(3)
+
+        ns = normalizeNamespace(prefix)
+        if ns in knownNamespaces:
+            # If the prefix designates a known namespace, then it might be
+            # followed by optional whitespace that should be removed to get
+            # the canonical page name
+            # (e.g., "Category:  Births" should become "Category:Births").
+            title = ns + ":" + ucfirst(rest)
+        else:
+            # No namespace, just capitalize first letter.
+            # If the part before the colon is not a known namespace, then we
+            # must not remove the space after the colon (if any), e.g.,
+            # "3001: The_Final_Odyssey" != "3001:The_Final_Odyssey".
+            # However, to get the canonical page name we must contract multiple
+            # spaces into one, because
+            # "3001:   The_Final_Odyssey" != "3001: The_Final_Odyssey".
+            title = ucfirst(prefix) + ":" + optionalWhitespace + ucfirst(rest)
+    else:
+        # no namespace, just capitalize first letter
+        title = ucfirst(title)
+    return title
+
+
+def unescape(text):
+    """
+    Removes HTML or XML character references and entities from a text string.
+
+    :param text The HTML (or XML) source text.
+    :return The plain text, as a Unicode string, if necessary.
+    """
+
+    def fixup(m):
+        text = m.group(0)
+        code = m.group(1)
+        try:
+            if text[1] == "#":  # character reference
+                if text[2] == "x":
+                    return chr(int(code[1:], 16))
+                else:
+                    return chr(int(code))
+            else:  # named entity
+                return chr(name2codepoint[code])
+        except:
+            return text  # leave as is
+
+    return re.sub("&#?(\w+);", fixup, text)
+
+
+# Match HTML comments
+# The buggy template {{Template:T}} has a comment terminating with just "->"
+comment = re.compile(r'<!--.*?-->', re.DOTALL)
+
+# Match ignored tags
+ignored_tag_patterns = []
+
+
+def ignoreTag(tag):
+    left = re.compile(r'<%s\b.*?>' % tag, re.IGNORECASE | re.DOTALL)  # both <ref> and <reference>
+    right = re.compile(r'</\s*%s>' % tag, re.IGNORECASE)
+    ignored_tag_patterns.append((left, right))
+
+
+def resetIgnoredTags():
+    global ignored_tag_patterns
+    ignored_tag_patterns = []
+
+
+for tag in ignoredTags:
+    ignoreTag(tag)
+
+# Match selfClosing HTML tags
+selfClosing_tag_patterns = [
+    re.compile(r'<\s*%s\b[^>]*/\s*>' % tag, re.DOTALL | re.IGNORECASE) for tag in selfClosingTags
+]
+
+# Match HTML placeholder tags
+placeholder_tag_patterns = [
+    (re.compile(r'<\s*%s(\s*| [^>]+?)>.*?<\s*/\s*%s\s*>' % (tag, tag), re.DOTALL | re.IGNORECASE),
+     repl) for tag, repl in placeholder_tags.items()
+]
+
+# Match preformatted lines
+preformatted = re.compile(r'^ .*?$')
+
+# Match external links (space separates second optional parameter)
+externalLink = re.compile(r'\[\w+[^ ]*? (.*?)]')
+externalLinkNoAnchor = re.compile(r'\[\w+[&\]]*\]')
+
+# Matches bold/italic
+bold_italic = re.compile(r"'''''(.*?)'''''")
+bold = re.compile(r"'''(.*?)'''")
+italic_quote = re.compile(r"''\"([^\"]*?)\"''")
+italic = re.compile(r"''(.*?)''")
+quote_quote = re.compile(r'""([^"]*?)""')
+
+# Matches space
+spaces = re.compile(r' {2,}')
+
+# Matches dots
+dots = re.compile(r'\.{4,}')
+
+# ======================================================================
+
+class Template(list):
+    """
+    A Template is a list of TemplateText or TemplateArgs
+    """
+
+    @classmethod
+    def parse(cls, body):
+        tpl = Template()
+        # we must handle nesting, s.a.
+        # {{{1|{{PAGENAME}}}
+        # {{{italics|{{{italic|}}}
+        # {{#if:{{{{{#if:{{{nominee|}}}|nominee|candidate}}|}}}|
+        #
+        start = 0
+        for s,e in findMatchingBraces(body, 3):
+            tpl.append(TemplateText(body[start:s]))
+            tpl.append(TemplateArg(body[s+3:e-3]))
+            start = e
+        tpl.append(TemplateText(body[start:])) # leftover
+        return tpl
+
+    def subst(self, params, extractor, depth=0):
+        # We perform parameter substitutions recursively.
+        # We also limit the maximum number of iterations to avoid too long or
+        # even endless loops (in case of malformed input).
+
+        # :see: http://meta.wikimedia.org/wiki/Help:Expansion#Distinction_between_variables.2C_parser_functions.2C_and_templates
+        #
+        # Parameter values are assigned to parameters in two (?) passes.
+        # Therefore a parameter name in a template can depend on the value of
+        # another parameter of the same template, regardless of the order in
+        # which they are specified in the template call, for example, using
+        # Template:ppp containing "{{{{{{p}}}}}}", {{ppp|p=q|q=r}} and even
+        # {{ppp|q=r|p=q}} gives r, but using Template:tvvv containing
+        # "{{{{{{{{{p}}}}}}}}}", {{tvvv|p=q|q=r|r=s}} gives s.
+
+        logging.debug('subst tpl (%d, %d) %s', len(extractor.frame), depth, self)
+
+        if depth > extractor.maxParameterRecursionLevels:
+            extractor.recursion_exceeded_3_errs += 1
+            return ''
+
+        return ''.join([tpl.subst(params, extractor, depth) for tpl in self])
+
+    def __str__(self):
+        return ''.join([str(x) for x in self])
+
+
+class TemplateText(str):
+    """Fixed text of template"""
+
+    def subst(self, params, extractor, depth):
+        return self
+
+
+class TemplateArg():
+    """
+    parameter to a template.
+    Has a name and a default value, both of which are Templates.
+    """
+    def __init__(self, parameter):
+        """
+        :param parameter: the parts of a tplarg.
+        """
+        # the parameter name itself might contain templates, e.g.:
+        #   appointe{{#if:{{{appointer14|}}}|r|d}}14|
+        #   4|{{{{{subst|}}}CURRENTYEAR}}
+
+        # any parts in a tplarg after the first (the parameter default) are
+        # ignored, and an equals sign in the first part is treated as plain text.
+        #logging.debug('TemplateArg %s', parameter)
+
+        parts = splitParts(parameter)
+        self.name = Template.parse(parts[0])
+        if len(parts) > 1:
+            # This parameter has a default value
+            self.default = Template.parse(parts[1])
+        else:
+            self.default = None
+
+    def __str__(self):
+        if self.default:
+            return '{{{%s|%s}}}' % (self.name, self.default)
+        else:
+            return '{{{%s}}}' % self.name
+
+    def subst(self, params, extractor, depth):
+        """
+        Substitute value for this argument from dict :param params:
+        Use :param extractor: to evaluate expressions for name and default.
+        Limit substitution to the maximun :param depth:.
+        """
+        # the parameter name itself might contain templates, e.g.:
+        # appointe{{#if:{{{appointer14|}}}|r|d}}14|
+        paramName = self.name.subst(params, extractor, depth+1)
+        paramName = extractor.expandTemplates(paramName)
+        res = ''
+        if paramName in params:
+            res = params[paramName]  # use parameter value specified in template invocation
+        elif self.default:            # use the default value
+            defaultValue = self.default.subst(params, extractor, depth+1)
+            res =  extractor.expandTemplates(defaultValue)
+        #logging.debug('subst arg %d %s -> %s' % (depth, paramName, res))
+        return res
+
+
+# ======================================================================
+
+substWords = 'subst:|safesubst:'
+
+
+class Extractor():
+    """
+    An extraction task on a article.
+    """
+    ##
+    # Whether to preserve links in output
+    keepLinks = False
+
+    ##
+    # Whether to preserve section titles
+    keepSections = True
+
+    ##
+    # Whether to output text with HTML formatting elements in <doc> files.
+    HtmlFormatting = False
+
+    ##
+    # Whether to produce json instead of the default <doc> output format.
+    toJson = False
+
+    ##
+    # Obtained from TemplateNamespace
+    templatePrefix = ''
+
+    def __init__(self, id, revid, urlbase, title, page):
+        """
+        :param page: a list of lines.
+        """
+        self.id = id
+        self.revid = revid
+        self.url = get_url(urlbase, id)
+        self.title = title
+        self.page = page
+        self.magicWords = MagicWords()
+        self.frame = []
+        self.recursion_exceeded_1_errs = 0  # template recursion within expandTemplates()
+        self.recursion_exceeded_2_errs = 0  # template recursion within expandTemplate()
+        self.recursion_exceeded_3_errs = 0  # parameter recursion
+        self.template_title_errs = 0
+
+    def clean_text(self, text, mark_headers=False, expand_templates=True,
+                   html_safe=True):
+        """
+        :param mark_headers: True to distinguish headers from paragraphs
+          e.g. "## Section 1"
+        """
+        self.magicWords['namespace'] = self.title[:max(0, self.title.find(":"))]
+        #self.magicWords['namespacenumber'] = '0' # for article,
+        self.magicWords['pagename'] = self.title
+        self.magicWords['fullpagename'] = self.title
+        self.magicWords['currentyear'] = time.strftime('%Y')
+        self.magicWords['currentmonth'] = time.strftime('%m')
+        self.magicWords['currentday'] = time.strftime('%d')
+        self.magicWords['currenthour'] = time.strftime('%H')
+        self.magicWords['currenttime'] = time.strftime('%H:%M:%S')
+
+        text = clean(self, text, expand_templates=expand_templates,
+                     html_safe=html_safe)
+
+        text = compact(text, mark_headers=mark_headers)
+        return text
+
+    def extract(self, out, html_safe=True):
+        """
+        :param out: a memory file.
+        :param html_safe: whether to escape HTML entities.
+        """
+        logging.debug("%s\t%s", self.id, self.title)
+        text = ''.join(self.page)
+        text = self.clean_text(text, html_safe=html_safe)
+
+        if self.to_json:
+            json_data = {
+		'id': self.id,
+                'revid': self.revid,
+                'url': self.url,
+                'title': self.title,
+                'text': "\n".join(text)
+            }
+            out_str = json.dumps(json_data)
+            out.write(out_str)
+            out.write('\n')
+        else:
+            header = '<doc id="%s" url="%s" title="%s">\n' % (self.id, self.url, self.title)
+            # Separate header from text with a newline.
+            header += self.title + '\n\n'
+            footer = "\n</doc>\n"
+            out.write(header)
+            out.write('\n'.join(text))
+            out.write('\n')
+            out.write(footer)
+
+        errs = (self.template_title_errs,
+                self.recursion_exceeded_1_errs,
+                self.recursion_exceeded_2_errs,
+                self.recursion_exceeded_3_errs)
+        if any(errs):
+            logging.warn("Template errors in article '%s' (%s): title(%d) recursion(%d, %d, %d)",
+                         self.title, self.id, *errs)
+
+    # ----------------------------------------------------------------------
+    # Expand templates
+
+    maxTemplateRecursionLevels = 30
+    maxParameterRecursionLevels = 16
+
+    # check for template beginning
+    reOpen = re.compile('(?<!{){{(?!{)', re.DOTALL)
+
+    def expandTemplates(self, wikitext):
+        """
+        :param wikitext: the text to be expanded.
+
+        Templates are frequently nested. Occasionally, parsing mistakes may
+        cause template insertion to enter an infinite loop, for instance when
+        trying to instantiate Template:Country
+
+        {{country_{{{1}}}|{{{2}}}|{{{2}}}|size={{{size|}}}|name={{{name|}}}}}
+
+        which is repeatedly trying to insert template 'country_', which is
+        again resolved to Template:Country. The straightforward solution of
+        keeping track of templates that were already inserted for the current
+        article would not work, because the same template may legally be used
+        more than once, with different parameters in different parts of the
+        article.  Therefore, we limit the number of iterations of nested
+        template inclusion.
+
+        """
+        # Test template expansion at:
+        # https://en.wikipedia.org/wiki/Special:ExpandTemplates
+
+        res = ''
+        if len(self.frame) >= self.maxTemplateRecursionLevels:
+            self.recursion_exceeded_1_errs += 1
+            return res
+
+        # logging.debug('<expandTemplates ' + str(len(self.frame)))
+
+        cur = 0
+        # look for matching {{...}}
+        for s, e in findMatchingBraces(wikitext, 2):
+            res += wikitext[cur:s] + self.expandTemplate(wikitext[s + 2:e - 2])
+            cur = e
+        # leftover
+        res += wikitext[cur:]
+        # logging.debug('   expandTemplates> %d %s', len(self.frame), res)
+        return res
+
+    def templateParams(self, parameters):
+        """
+        Build a dictionary with positional or name key to expanded parameters.
+        :param parameters: the parts[1:] of a template, i.e. all except the title.
+        """
+        templateParams = {}
+
+        if not parameters:
+            return templateParams
+        logging.debug('<templateParams: %s', '|'.join(parameters))
+
+        # Parameters can be either named or unnamed. In the latter case, their
+        # name is defined by their ordinal position (1, 2, 3, ...).
+
+        unnamedParameterCounter = 0
+
+        # It's legal for unnamed parameters to be skipped, in which case they
+        # will get default values (if available) during actual instantiation.
+        # That is {{template_name|a||c}} means parameter 1 gets
+        # the value 'a', parameter 2 value is not defined, and parameter 3 gets
+        # the value 'c'.  This case is correctly handled by function 'split',
+        # and does not require any special handling.
+        for param in parameters:
+            # Spaces before or after a parameter value are normally ignored,
+            # UNLESS the parameter contains a link (to prevent possible gluing
+            # the link to the following text after template substitution)
+
+            # Parameter values may contain "=" symbols, hence the parameter
+            # name extends up to the first such symbol.
+
+            # It is legal for a parameter to be specified several times, in
+            # which case the last assignment takes precedence. Example:
+            # "{{t|a|b|c|2=B}}" is equivalent to "{{t|a|B|c}}".
+            # Therefore, we don't check if the parameter has been assigned a
+            # value before, because anyway the last assignment should override
+            # any previous ones.
+            # FIXME: Don't use DOTALL here since parameters may be tags with
+            # attributes, e.g. <div class="templatequotecite">
+            # Parameters may span several lines, like:
+            # {{Reflist|colwidth=30em|refs=
+            # &lt;ref name=&quot;Goode&quot;&gt;Title&lt;/ref&gt;
+
+            # The '=' might occurr within an HTML attribute:
+            #   "&lt;ref name=value"
+            # but we stop at first.
+
+            # The '=' might occurr within quotes:
+            # ''''<span lang="pt-pt" xml:lang="pt-pt">cénicas</span>'''
+
+            m = re.match(" *([^=']*?) *=(.*)", param, re.DOTALL)
+            if m:
+                # This is a named parameter.  This case also handles parameter
+                # assignments like "2=xxx", where the number of an unnamed
+                # parameter ("2") is specified explicitly - this is handled
+                # transparently.
+
+                parameterName = m.group(1).strip()
+                parameterValue = m.group(2)
+
+                if ']]' not in parameterValue:  # if the value does not contain a link, trim whitespace
+                    parameterValue = parameterValue.strip()
+                templateParams[parameterName] = parameterValue
+            else:
+                # this is an unnamed parameter
+                unnamedParameterCounter += 1
+
+                if ']]' not in param:  # if the value does not contain a link, trim whitespace
+                    param = param.strip()
+                templateParams[str(unnamedParameterCounter)] = param
+        logging.debug('   templateParams> %s', '|'.join(templateParams.values()))
+        return templateParams
+
+    def expandTemplate(self, body):
+        """Expands template invocation.
+        :param body: the parts of a template.
+
+        :see http://meta.wikimedia.org/wiki/Help:Expansion for an explanation
+        of the process.
+
+        See in particular: Expansion of names and values
+        http://meta.wikimedia.org/wiki/Help:Expansion#Expansion_of_names_and_values
+
+        For most parser functions all names and values are expanded,
+        regardless of what is relevant for the result. The branching functions
+        (#if, #ifeq, #iferror, #ifexist, #ifexpr, #switch) are exceptions.
+
+        All names in a template call are expanded, and the titles of the
+        tplargs in the template body, after which it is determined which
+        values must be expanded, and for which tplargs in the template body
+        the first part (default).
+
+        In the case of a tplarg, any parts beyond the first are never
+        expanded.  The possible name and the value of the first part is
+        expanded if the title does not match a name in the template call.
+
+        :see code for braceSubstitution at
+        https://doc.wikimedia.org/mediawiki-core/master/php/html/Parser_8php_source.html#3397:
+
+        """
+
+        # template        = "{{" parts "}}"
+
+        # Templates and tplargs are decomposed in the same way, with pipes as
+        # separator, even though eventually any parts in a tplarg after the first
+        # (the parameter default) are ignored, and an equals sign in the first
+        # part is treated as plain text.
+        # Pipes inside inner templates and tplargs, or inside double rectangular
+        # brackets within the template or tplargs are not taken into account in
+        # this decomposition.
+        # The first part is called title, the other parts are simply called parts.
+
+        # If a part has one or more equals signs in it, the first equals sign
+        # determines the division into name = value. Equals signs inside inner
+        # templates and tplargs, or inside double rectangular brackets within the
+        # part are not taken into account in this decomposition. Parts without
+        # equals sign are indexed 1, 2, .., given as attribute in the <name> tag.
+
+        if len(self.frame) >= self.maxTemplateRecursionLevels:
+            self.recursion_exceeded_2_errs += 1
+            # logging.debug('   INVOCATION> %d %s', len(self.frame), body)
+            return ''
+
+        logging.debug('INVOCATION %d %s', len(self.frame), body)
+
+        parts = splitParts(body)
+        # title is the portion before the first |
+        logging.debug('TITLE %s', parts[0].strip())
+        title = self.expandTemplates(parts[0].strip())
+
+        # SUBST
+        # Apply the template tag to parameters without
+        # substituting into them, e.g.
+        # {{subst:t|a{{{p|q}}}b}} gives the wikitext start-a{{{p|q}}}b-end
+        # @see https://www.mediawiki.org/wiki/Manual:Substitution#Partial_substitution
+        subst = False
+        if re.match(substWords, title, re.IGNORECASE):
+            title = re.sub(substWords, '', title, 1, re.IGNORECASE)
+            subst = True
+
+        if title.lower() in self.magicWords.values:
+            return self.magicWords[title.lower()]
+
+        # Parser functions
+        # The first argument is everything after the first colon.
+        # It has been evaluated above.
+        colon = title.find(':')
+        if colon > 1:
+            funct = title[:colon]
+            parts[0] = title[colon + 1:].strip()  # side-effect (parts[0] not used later)
+            # arguments after first are not evaluated
+            ret = callParserFunction(funct, parts, self.frame)
+            return self.expandTemplates(ret)
+
+        title = fullyQualifiedTemplateTitle(title)
+        if not title:
+            self.template_title_errs += 1
+            return ''
+
+        redirected = redirects.get(title)
+        if redirected:
+            title = redirected
+
+        # get the template
+        if title in templateCache:
+            template = templateCache[title]
+        elif title in templates:
+            template = Template.parse(templates[title])
+            # add it to cache
+            templateCache[title] = template
+            del templates[title]
+        else:
+            # The page being included could not be identified
+            return ''
+
+        # logging.debug('TEMPLATE %s: %s', title, template)
+
+        # tplarg          = "{{{" parts "}}}"
+        # parts           = [ title *( "|" part ) ]
+        # part            = ( part-name "=" part-value ) / ( part-value )
+        # part-name       = wikitext-L3
+        # part-value      = wikitext-L3
+        # wikitext-L3     = literal / template / tplarg / link / comment /
+        #                   line-eating-comment / unclosed-comment /
+        #           	    xmlish-element / *wikitext-L3
+
+        # A tplarg may contain other parameters as well as templates, e.g.:
+        #   {{{text|{{{quote|{{{1|{{error|Error: No text given}}}}}}}}}}}
+        # hence no simple RE like this would work:
+        #   '{{{((?:(?!{{{).)*?)}}}'
+        # We must use full CF parsing.
+
+        # the parameter name itself might be computed, e.g.:
+        #   {{{appointe{{#if:{{{appointer14|}}}|r|d}}14|}}}
+
+        # Because of the multiple uses of double-brace and triple-brace
+        # syntax, expressions can sometimes be ambiguous.
+        # Precedence rules specifed here:
+        # http://www.mediawiki.org/wiki/Preprocessor_ABNF#Ideal_precedence
+        # resolve ambiguities like this:
+        #   {{{{ }}}} -> { {{{ }}} }
+        #   {{{{{ }}}}} -> {{ {{{ }}} }}
+        #
+        # :see: https://en.wikipedia.org/wiki/Help:Template#Handling_parameters
+
+        params = parts[1:]
+
+        if not subst:
+            # Evaluate parameters, since they may contain templates, including
+            # the symbol "=".
+            # {{#ifexpr: {{{1}}} = 1 }}
+            params = [self.expandTemplates(p) for p in params]
+
+        # build a dict of name-values for the parameter values
+        params = self.templateParams(params)
+
+        # Perform parameter substitution
+        # extend frame before subst, since there may be recursion in default
+        # parameter value, e.g. {{OTRS|celebrative|date=April 2015}} in article
+        # 21637542 in enwiki.
+        self.frame.append((title, params))
+        instantiated = template.subst(params, self)
+        # logging.debug('instantiated %d %s', len(self.frame), instantiated)
+        value = self.expandTemplates(instantiated)
+        self.frame.pop()
+        # logging.debug('   INVOCATION> %s %d %s', title, len(self.frame), value)
+        return value
+
+
+# ----------------------------------------------------------------------
+# parameter handling
+
+
+def splitParts(paramsList):
+    """
+    :param paramsList: the parts of a template or tplarg.
+
+    Split template parameters at the separator "|".
+    separator "=".
+
+    Template parameters often contain URLs, internal links, text or even
+    template expressions, since we evaluate templates outside in.
+    This is required for cases like:
+      {{#if: {{{1}}} | {{lc:{{{1}}} | "parameter missing"}}
+    Parameters are separated by "|" symbols. However, we
+    cannot simply split the string on "|" symbols, since these
+    also appear inside templates and internal links, e.g.
+
+     {{if:|
+      |{{#if:the president|
+           |{{#if:|
+               [[Category:Hatnote templates|A{{PAGENAME}}]]
+            }}
+       }}
+     }}
+
+    We split parts at the "|" symbols that are not inside any pair
+    {{{...}}}, {{...}}, [[...]], {|...|}.
+    """
+
+    # Must consider '[' as normal in expansion of Template:EMedicine2:
+    # #ifeq: ped|article|[http://emedicine.medscape.com/article/180-overview|[http://www.emedicine.com/ped/topic180.htm#{{#if: |section~}}
+    # as part of:
+    # {{#ifeq: ped|article|[http://emedicine.medscape.com/article/180-overview|[http://www.emedicine.com/ped/topic180.htm#{{#if: |section~}}}} ped/180{{#if: |~}}]
+
+    # should handle both tpl arg like:
+    #    4|{{{{{subst|}}}CURRENTYEAR}}
+    # and tpl parameters like:
+    #    ||[[Category:People|{{#if:A|A|{{PAGENAME}}}}]]
+
+    sep = '|'
+    parameters = []
+    cur = 0
+    for s, e in findMatchingBraces(paramsList):
+        par = paramsList[cur:s].split(sep)
+        if par:
+            if parameters:
+                # portion before | belongs to previous parameter
+                parameters[-1] += par[0]
+                if len(par) > 1:
+                    # rest are new parameters
+                    parameters.extend(par[1:])
+            else:
+                parameters = par
+        elif not parameters:
+            parameters = ['']  # create first param
+        # add span to last previous parameter
+        parameters[-1] += paramsList[s:e]
+        cur = e
+    # leftover
+    par = paramsList[cur:].split(sep)
+    if par:
+        if parameters:
+            # portion before | belongs to previous parameter
+            parameters[-1] += par[0]
+            if len(par) > 1:
+                # rest are new parameters
+                parameters.extend(par[1:])
+        else:
+            parameters = par
+
+    # logging.debug('splitParts %s %s\nparams: %s', sep, paramsList, str(parameters))
+    return parameters
+
+
+def findMatchingBraces(text, ldelim=0):
+    """
+    :param ldelim: number of braces to match. 0 means match [[]], {{}} and {{{}}}.
+    """
+    # Parsing is done with respect to pairs of double braces {{..}} delimiting
+    # a template, and pairs of triple braces {{{..}}} delimiting a tplarg.
+    # If double opening braces are followed by triple closing braces or
+    # conversely, this is taken as delimiting a template, with one left-over
+    # brace outside it, taken as plain text. For any pattern of braces this
+    # defines a set of templates and tplargs such that any two are either
+    # separate or nested (not overlapping).
+
+    # Unmatched double rectangular closing brackets can be in a template or
+    # tplarg, but unmatched double rectangular opening brackets cannot.
+    # Unmatched double or triple closing braces inside a pair of
+    # double rectangular brackets are treated as plain text.
+    # Other formulation: in ambiguity between template or tplarg on one hand,
+    # and a link on the other hand, the structure with the rightmost opening
+    # takes precedence, even if this is the opening of a link without any
+    # closing, so not producing an actual link.
+
+    # In the case of more than three opening braces the last three are assumed
+    # to belong to a tplarg, unless there is no matching triple of closing
+    # braces, in which case the last two opening braces are are assumed to
+    # belong to a template.
+
+    # We must skip individual { like in:
+    #   {{#ifeq: {{padleft:|1|}} | { | | &nbsp;}}
+    # We must resolve ambiguities like this:
+    #   {{{{ }}}} -> { {{{ }}} }
+    #   {{{{{ }}}}} -> {{ {{{ }}} }}
+    #   {{#if:{{{{{#if:{{{nominee|}}}|nominee|candidate}}|}}}|...}}
+
+    # Handle:
+    #   {{{{{|safesubst:}}}#Invoke:String|replace|{{{1|{{{{{|safesubst:}}}PAGENAME}}}}}|%s+%([^%(]-%)$||plain=false}}
+    # as well as expressions with stray }:
+    #   {{{link|{{ucfirst:{{{1}}}}}} interchange}}}
+
+    if ldelim:  # 2-3
+        reOpen = re.compile('[{]{%d,}' % ldelim)  # at least ldelim
+        reNext = re.compile('[{]{2,}|}{2,}')  # at least 2 open or close bracces
+    else:
+        reOpen = re.compile('{{2,}|\[{2,}')
+        reNext = re.compile('{{2,}|}{2,}|\[{2,}|]{2,}')  # at least 2
+
+    cur = 0
+    while True:
+        m1 = reOpen.search(text, cur)
+        if not m1:
+            return
+        lmatch = m1.end() - m1.start()
+        if m1.group()[0] == '{':
+            stack = [lmatch]  # stack of opening braces lengths
+        else:
+            stack = [-lmatch]  # negative means [
+        end = m1.end()
+        while True:
+            m2 = reNext.search(text, end)
+            if not m2:
+                return  # unbalanced
+            end = m2.end()
+            brac = m2.group()[0]
+            lmatch = m2.end() - m2.start()
+
+            if brac == '{':
+                stack.append(lmatch)
+            elif brac == '}':
+                while stack:
+                    openCount = stack.pop()  # opening span
+                    if openCount == 0:  # illegal unmatched [[
+                        continue
+                    if lmatch >= openCount:
+                        lmatch -= openCount
+                        if lmatch <= 1:  # either close or stray }
+                            break
+                    else:
+                        # put back unmatched
+                        stack.append(openCount - lmatch)
+                        break
+                if not stack:
+                    yield m1.start(), end - lmatch
+                    cur = end
+                    break
+                elif len(stack) == 1 and 0 < stack[0] < ldelim:
+                    # ambiguous {{{{{ }}} }}
+                    yield m1.start() + stack[0], end
+                    cur = end
+                    break
+            elif brac == '[':  # [[
+                stack.append(-lmatch)
+            else:  # ]]
+                while stack and stack[-1] < 0:  # matching [[
+                    openCount = -stack.pop()
+                    if lmatch >= openCount:
+                        lmatch -= openCount
+                        if lmatch <= 1:  # either close or stray ]
+                            break
+                    else:
+                        # put back unmatched (negative)
+                        stack.append(lmatch - openCount)
+                        break
+                if not stack:
+                    yield m1.start(), end - lmatch
+                    cur = end
+                    break
+                # unmatched ]] are discarded
+                cur = end
+
+
+def findBalanced(text, openDelim, closeDelim):
+    """
+    Assuming that text contains a properly balanced expression using
+    :param openDelim: as opening delimiters and
+    :param closeDelim: as closing delimiters.
+    :return: an iterator producing pairs (start, end) of start and end
+    positions in text containing a balanced expression.
+    """
+    openPat = '|'.join([re.escape(x) for x in openDelim])
+    # patter for delimiters expected after each opening delimiter
+    afterPat = {o: re.compile(openPat + '|' + c, re.DOTALL) for o, c in zip(openDelim, closeDelim)}
+    stack = []
+    start = 0
+    cur = 0
+    # end = len(text)
+    startSet = False
+    startPat = re.compile(openPat)
+    nextPat = startPat
+    while True:
+        next = nextPat.search(text, cur)
+        if not next:
+            return
+        if not startSet:
+            start = next.start()
+            startSet = True
+        delim = next.group(0)
+        if delim in openDelim:
+            stack.append(delim)
+            nextPat = afterPat[delim]
+        else:
+            opening = stack.pop()
+            # assert opening == openDelim[closeDelim.index(next.group(0))]
+            if stack:
+                nextPat = afterPat[stack[-1]]
+            else:
+                yield start, next.end()
+                nextPat = startPat
+                start = next.end()
+                startSet = False
+        cur = next.end()
+
+# ----------------------------------------------------------------------
+# parser functions utilities
+
+
+def ucfirst(string):
+    """:return: a string with just its first character uppercase
+    We can't use title() since it coverts all words.
+    """
+    if string:
+        if len(string) > 1:
+            return string[0].upper() + string[1:]
+        else:
+            return string.upper()
+    else:
+        return ''
+
+
+def lcfirst(string):
+    """:return: a string with its first character lowercase"""
+    if string:
+        if len(string) > 1:
+            return string[0].lower() + string[1:]
+        else:
+            return string.lower()
+    else:
+        return ''
+
+
+def fullyQualifiedTemplateTitle(templateTitle):
+    """
+    Determine the namespace of the page being included through the template
+    mechanism
+    """
+    if templateTitle.startswith(':'):
+        # Leading colon by itself implies main namespace, so strip this colon
+        return ucfirst(templateTitle[1:])
+    else:
+        m = re.match('([^:]*)(:.*)', templateTitle)
+        if m:
+            # colon found but not in the first position - check if it
+            # designates a known namespace
+            prefix = normalizeNamespace(m.group(1))
+            if prefix in knownNamespaces:
+                return prefix + ucfirst(m.group(2))
+    # The title of the page being included is NOT in the main namespace and
+    # lacks any other explicit designation of the namespace - therefore, it
+    # is resolved to the Template namespace (that's the default for the
+    # template inclusion mechanism).
+
+    # This is a defense against pages whose title only contains UTF-8 chars
+    # that are reduced to an empty string. Right now I can think of one such
+    # case - <C2><A0> which represents the non-breaking space.
+    # In this particular case, this page is a redirect to [[Non-nreaking
+    # space]], but having in the system a redirect page with an empty title
+    # causes numerous problems, so we'll live happier without it.
+    if templateTitle:
+        return Extractor.templatePrefix + ucfirst(templateTitle)
+    else:
+        return ''  # caller may log as error
+
+
+def normalizeNamespace(ns):
+    return ucfirst(ns)
+
+
+# ----------------------------------------------------------------------
+# Parser functions
+# see http://www.mediawiki.org/wiki/Help:Extension:ParserFunctions
+# https://github.com/Wikia/app/blob/dev/extensions/ParserFunctions/ParserFunctions_body.php
+
+
+class Infix():
+
+    """Infix operators.
+    The calling sequence for the infix is:
+      x |op| y
+    """
+
+    def __init__(self, function):
+        self.function = function
+
+    def __ror__(self, other):
+        return Infix(lambda x, self=self, other=other: self.function(other, x))
+
+    def __or__(self, other):
+        return self.function(other)
+
+    def __rlshift__(self, other):
+        return Infix(lambda x, self=self, other=other: self.function(other, x))
+
+    def __rshift__(self, other):
+        return self.function(other)
+
+    def __call__(self, value1, value2):
+        return self.function(value1, value2)
+
+
+ROUND = Infix(lambda x, y: round(x, y))
+
+
+def sharp_expr(expr):
+    try:
+        expr = re.sub('=', '==', expr)
+        expr = re.sub('mod', '%', expr)
+        expr = re.sub('\bdiv\b', '/', expr)
+        expr = re.sub('\bround\b', '|ROUND|', expr)
+        return str(eval(expr))
+    except:
+        return '<span class="error"></span>'
+
+
+def sharp_if(testValue, valueIfTrue, valueIfFalse=None, *args):
+    # In theory, we should evaluate the first argument here,
+    # but it was evaluated while evaluating part[0] in expandTemplate().
+    if testValue.strip():
+        # The {{#if:}} function is an if-then-else construct.
+        # The applied condition is: "The condition string is non-empty".
+        valueIfTrue = valueIfTrue.strip()
+        if valueIfTrue:
+            return valueIfTrue
+    elif valueIfFalse:
+        return valueIfFalse.strip()
+    return ""
+
+
+def sharp_ifeq(lvalue, rvalue, valueIfTrue, valueIfFalse=None, *args):
+    rvalue = rvalue.strip()
+    if rvalue:
+        # lvalue is always defined
+        if lvalue.strip() == rvalue:
+            # The {{#ifeq:}} function is an if-then-else construct. The
+            # applied condition is "is rvalue equal to lvalue". Note that this
+            # does only string comparison while MediaWiki implementation also
+            # supports numerical comparissons.
+
+            if valueIfTrue:
+                return valueIfTrue.strip()
+        else:
+            if valueIfFalse:
+                return valueIfFalse.strip()
+    return ""
+
+
+def sharp_iferror(test, then='', Else=None, *args):
+    if re.match('<(?:strong|span|p|div)\s(?:[^\s>]*\s+)*?class="(?:[^"\s>]*\s+)*?error(?:\s[^">]*)?"', test):
+        return then
+    elif Else is None:
+        return test.strip()
+    else:
+        return Else.strip()
+
+
+def sharp_switch(primary, *params):
+    # FIXME: we don't support numeric expressions in primary
+
+    # {{#switch: comparison string
+    #  | case1 = result1
+    #  | case2
+    #  | case4 = result2
+    #  | 1 | case5 = result3
+    #  | #default = result4
+    # }}
+
+    primary = primary.strip()
+    found = False  # for fall through cases
+    default = None
+    rvalue = None
+    lvalue = ''
+    for param in params:
+        # handle cases like:
+        #  #default = [http://www.perseus.tufts.edu/hopper/text?doc=Perseus...]
+        pair = param.split('=', 1)
+        lvalue = pair[0].strip()
+        rvalue = None
+        if len(pair) > 1:
+            # got "="
+            rvalue = pair[1].strip()
+            # check for any of multiple values pipe separated
+            if found or primary in [v.strip() for v in lvalue.split('|')]:
+                # Found a match, return now
+                return rvalue
+            elif lvalue == '#default':
+                default = rvalue
+            rvalue = None  # avoid defaulting to last case
+        elif lvalue == primary:
+            # If the value matches, set a flag and continue
+            found = True
+    # Default case
+    # Check if the last item had no = sign, thus specifying the default case
+    if rvalue is not None:
+        return lvalue
+    elif default is not None:
+        return default
+    return ''
+
+
+# Extension Scribuntu
+def sharp_invoke(module, function, frame):
+    functions = modules.get(module)
+    if functions:
+        funct = functions.get(function)
+        if funct:
+            # find parameters in frame whose title is the one of the original
+            # template invocation
+            templateTitle = fullyQualifiedTemplateTitle(function)
+            if not templateTitle:
+                logging.warn("Template with empty title")
+            pair = next((x for x in frame if x[0] == templateTitle), None)
+            if pair:
+                params = pair[1]
+                # extract positional args
+                params = [params.get(str(i + 1)) for i in range(len(params))]
+                return funct(*params)
+            else:
+                return funct()
+    return ''
+
+
+parserFunctions = {
+
+    '#expr': sharp_expr,
+
+    '#if': sharp_if,
+
+    '#ifeq': sharp_ifeq,
+
+    '#iferror': sharp_iferror,
+
+    '#ifexpr': lambda *args: '',  # not supported
+
+    '#ifexist': lambda *args: '',  # not supported
+
+    '#rel2abs': lambda *args: '',  # not supported
+
+    '#switch': sharp_switch,
+
+    '# language': lambda *args: '',  # not supported
+
+    '#time': lambda *args: '',  # not supported
+
+    '#timel': lambda *args: '',  # not supported
+
+    '#titleparts': lambda *args: '',  # not supported
+
+    # This function is used in some pages to construct links
+    # http://meta.wikimedia.org/wiki/Help:URL
+    'urlencode': lambda string, *rest: urlencode(string),
+
+    'lc': lambda string, *rest: string.lower() if string else '',
+
+    'lcfirst': lambda string, *rest: lcfirst(string),
+
+    'uc': lambda string, *rest: string.upper() if string else '',
+
+    'ucfirst': lambda string, *rest: ucfirst(string),
+
+    'int': lambda string, *rest: str(int(string)),
+
+    'padleft': lambda char, width, string: string.ljust(char, int(pad)), # CHECK_ME
+
+}
+
+
+def callParserFunction(functionName, args, frame):
+    """
+    Parser functions have similar syntax as templates, except that
+    the first argument is everything after the first colon.
+    :param functionName: nameof the parser function
+    :param args: the arguments to the function
+    :return: the result of the invocation, None in case of failure.
+
+    http://meta.wikimedia.org/wiki/Help:ParserFunctions
+    """
+
+    try:
+        if functionName == '#invoke':
+            # special handling of frame
+            ret = sharp_invoke(args[0].strip(), args[1].strip(), frame)
+            # logging.debug('parserFunction> %s %s', args[1], ret)
+            return ret
+        if functionName in parserFunctions:
+            ret = parserFunctions[functionName](*args)
+            # logging.debug('parserFunction> %s(%s) %s', functionName, args, ret)
+            return ret
+    except:
+        return ""  # FIXME: fix errors
+
+    return ""
+
+
+# ----------------------------------------------------------------------
+# Extract Template definition
+
+reNoinclude = re.compile(r'<noinclude>(?:.*?)</noinclude>', re.DOTALL)
+reIncludeonly = re.compile(r'<includeonly>|</includeonly>', re.DOTALL)
+
+# These are built before spawning processes, hence they are shared.
+templates = {}
+redirects = {}
+# cache of parser templates
+# FIXME: sharing this with a Manager slows down.
+templateCache = {}
+
+
+def define_template(title, page):
+    """
+    Adds a template defined in the :param page:.
+    @see https://en.wikipedia.org/wiki/Help:Template#Noinclude.2C_includeonly.2C_and_onlyinclude
+    """
+    global templates
+    global redirects
+
+    # title = normalizeTitle(title)
+
+    # check for redirects
+    m = re.match('#REDIRECT.*?\[\[([^\]]*)]]', page[0], re.IGNORECASE)
+    if m:
+        redirects[title] = m.group(1)  # normalizeTitle(m.group(1))
+        return
+
+    text = unescape(''.join(page))
+
+    # We're storing template text for future inclusion, therefore,
+    # remove all <noinclude> text and keep all <includeonly> text
+    # (but eliminate <includeonly> tags per se).
+    # However, if <onlyinclude> ... </onlyinclude> parts are present,
+    # then only keep them and discard the rest of the template body.
+    # This is because using <onlyinclude> on a text fragment is
+    # equivalent to enclosing it in <includeonly> tags **AND**
+    # enclosing all the rest of the template body in <noinclude> tags.
+
+    # remove comments
+    text = comment.sub('', text)
+
+    # eliminate <noinclude> fragments
+    text = reNoinclude.sub('', text)
+    # eliminate unterminated <noinclude> elements
+    text = re.sub(r'<noinclude\s*>.*$', '', text, flags=re.DOTALL)
+    text = re.sub(r'<noinclude/>', '', text)
+
+    onlyincludeAccumulator = ''
+    for m in re.finditer('<onlyinclude>(.*?)</onlyinclude>', text, re.DOTALL):
+        onlyincludeAccumulator += m.group(1)
+    if onlyincludeAccumulator:
+        text = onlyincludeAccumulator
+    else:
+        text = reIncludeonly.sub('', text)
+
+    if text:
+        if title in templates and templates[title] != text:
+            logging.warn('Redefining: %s', title)
+        templates[title] = text
```

### Comparing `hazm-0.9.1/hazm/corpus_readers/wikipedia_reader.py` & `hazm-0.9.2/hazm/corpus_readers/wikipedia_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ ویکی‌پدیا است.
-
-[پیکرهٔ ویکی‌پدیا](http://download.wikimedia.org/fawiki/latest/fawiki-latest-
-pages-articles.xml.bz2) پیکرهٔ
-عظیمی مشتمل بر تمام مقالات ویکی‌پدیای فارسی است که هر دوماه یکبار بروزرسانی
-می‌شود. برای کسب اطلاعات بیشتر دربارهٔ این پیکره می‌توانید به [صفحهٔ اصلی
-آن](https://dumps.wikimedia.org/backup-index.html) مراجعه کنید.
-
-"""
-
-
-import os
-import re
-import subprocess
-from pathlib import Path
-from typing import Dict
-from typing import Iterator
-
-
-class WikipediaReader:
-    """این کلاس شامل توابعی برای خواندن پیکرهٔ ویکی‌پدیا است.
-
-    Args:
-        fawiki_dump: مسیر فولدر حاوی فایل‌های پیکره.
-        n_jobs: تعداد هسته‌های پردازنده برای پردازش موازی.
-
-    """
-
-    def __init__(self: "WikipediaReader", fawiki_dump: str, n_jobs: int = 2) -> None:
-        self.fawiki_dump = fawiki_dump
-        self.wiki_extractor = Path(__file__).parent / "wiki_extractor.py"
-        self.n_jobs = n_jobs
-
-    def docs(self: "WikipediaReader") -> Iterator[Dict[str, str]]:
-        """مقالات را برمی‌گرداند.
-
-        هر مقاله، شی‌ای متشکل از چند پارامتر است:
-
-        - شناسه (id)،
-        - عنوان (title)،
-        - متن (text)،
-        - نسخهٔ وب (date)،
-        - آدرس صفحه (url).
-
-        Examples:
-            >>> wikipedia = WikipediaReader('corpora/wikipedia.csv')
-            >>> next(wikipedia.docs())['id']
-
-        Yields:
-            مقالهٔ بعدی.
-
-        """
-        proc = subprocess.Popen(
-            [
-                "python",
-                self.wiki_extractor,
-                "--no-templates",
-                "--processes",
-                str(self.n_jobs),
-                "--output",
-                "-",
-                self.fawiki_dump,
-            ],
-            stdout=subprocess.PIPE,
-        )
-        doc_pattern = re.compile(r'<doc id="(\d+)" url="([^\"]+)" title="([^\"]+)">')
-
-        doc = []
-        for line in iter(proc.stdout.readline, b""):
-            line = line.strip().decode("utf8")
-            if line:
-                doc.append(line)
-
-            if line == "</doc>":
-                del doc[1]
-                id, url, title = doc_pattern.match(doc[0]).groups()  # noqa: A001
-                html = "\n".join(doc[1:-1])
-
-                yield {"id": id, "url": url, "title": title, "html": html, "text": html}
-                doc = []
-
-    def texts(self: "WikipediaReader") -> Iterator[str]:
-        """فقط متن مقالات را برمی‌گرداند.
-
-        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با همان تابع
-        ‍[docs()][hazm.corpus_readers.wikipedia_reader.WikipediaReader.docs] و دریافت مقدار
-        پراپرتی `text` نیز می‌توانید همین کار را انجام دهید.
-
-        Examples:
-            >>> wikipedia = WikipediaReader('corpora/wikipedia.csv')
-            >>> next(wikipedia.texts())[:30]
-
-        Yields:
-            متنِ مقالهٔ بعدی.
-
-        """
-        for doc in self.docs():
-            yield doc["text"]
+"""این ماژول شامل کلاس‌ها و توابعی برای خواندن پیکرهٔ ویکی‌پدیا است.
+
+[پیکرهٔ ویکی‌پدیا](http://download.wikimedia.org/fawiki/latest/fawiki-latest-
+pages-articles.xml.bz2) پیکرهٔ
+عظیمی مشتمل بر تمام مقالات ویکی‌پدیای فارسی است که هر دوماه یکبار بروزرسانی
+می‌شود. برای کسب اطلاعات بیشتر دربارهٔ این پیکره می‌توانید به [صفحهٔ اصلی
+آن](https://dumps.wikimedia.org/backup-index.html) مراجعه کنید.
+
+"""
+
+
+import os
+import re
+import subprocess
+from pathlib import Path
+from typing import Dict
+from typing import Iterator
+
+
+class WikipediaReader:
+    """این کلاس شامل توابعی برای خواندن پیکرهٔ ویکی‌پدیا است.
+
+    Args:
+        fawiki_dump: مسیر فولدر حاوی فایل‌های پیکره.
+        n_jobs: تعداد هسته‌های پردازنده برای پردازش موازی.
+
+    """
+
+    def __init__(self: "WikipediaReader", fawiki_dump: str, n_jobs: int = 2) -> None:
+        self.fawiki_dump = fawiki_dump
+        self.wiki_extractor = Path(__file__).parent / "wiki_extractor.py"
+        self.n_jobs = n_jobs
+
+    def docs(self: "WikipediaReader") -> Iterator[Dict[str, str]]:
+        """مقالات را برمی‌گرداند.
+
+        هر مقاله، شی‌ای متشکل از چند پارامتر است:
+
+        - شناسه (id)،
+        - عنوان (title)،
+        - متن (text)،
+        - نسخهٔ وب (date)،
+        - آدرس صفحه (url).
+
+        Examples:
+            >>> wikipedia = WikipediaReader('corpora/wikipedia.csv')
+            >>> next(wikipedia.docs())['id']
+
+        Yields:
+            مقالهٔ بعدی.
+
+        """
+        proc = subprocess.Popen(
+            [
+                "python",
+                self.wiki_extractor,
+                "--no-templates",
+                "--processes",
+                str(self.n_jobs),
+                "--output",
+                "-",
+                self.fawiki_dump,
+            ],
+            stdout=subprocess.PIPE,
+        )
+        doc_pattern = re.compile(r'<doc id="(\d+)" url="([^\"]+)" title="([^\"]+)">')
+
+        doc = []
+        for line in iter(proc.stdout.readline, b""):
+            line = line.strip().decode("utf8")
+            if line:
+                doc.append(line)
+
+            if line == "</doc>":
+                del doc[1]
+                id, url, title = doc_pattern.match(doc[0]).groups()  # noqa: A001
+                html = "\n".join(doc[1:-1])
+
+                yield {"id": id, "url": url, "title": title, "html": html, "text": html}
+                doc = []
+
+    def texts(self: "WikipediaReader") -> Iterator[str]:
+        """فقط متن مقالات را برمی‌گرداند.
+
+        این تابع صرفاً برای راحتی بیشتر تهیه شده وگرنه با همان تابع
+        ‍[docs()][hazm.corpus_readers.wikipedia_reader.WikipediaReader.docs] و دریافت مقدار
+        پراپرتی `text` نیز می‌توانید همین کار را انجام دهید.
+
+        Examples:
+            >>> wikipedia = WikipediaReader('corpora/wikipedia.csv')
+            >>> next(wikipedia.texts())[:30]
+
+        Yields:
+            متنِ مقالهٔ بعدی.
+
+        """
+        for doc in self.docs():
+            yield doc["text"]
```

### Comparing `hazm-0.9.1/hazm/embedding.py` & `hazm-0.9.2/hazm/embedding.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,412 +1,520 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای تبدیل کلمه یا متن به برداری از اعداد است."""
-import multiprocessing
-import os
-import warnings
-from pathlib import Path
-from typing import Any
-from typing import Iterator
-from typing import List
-from typing import Tuple
-from typing import Type
-
-from gensim.models import Doc2Vec
-from gensim.models import KeyedVectors
-from gensim.models import fasttext
-from gensim.models.doc2vec import TaggedDocument
-from gensim.scripts.glove2word2vec import glove2word2vec
-from gensim.test.utils import datapath
-from numpy import ndarray
-
-from hazm import Normalizer
-
-from hazm import word_tokenize
-
-supported_embeddings = ["fasttext", "keyedvector", "glove"]
-
-
-class WordEmbedding:
-    """این کلاس شامل توابعی برای تبدیل کلمه به برداری از اعداد است.
-
-    Args:
-        model_type: نوع امبدینگ که می‌تواند یکی از مقادیر ‍`fasttext`, `keyedvector`, `glove` باشد.
-        model_path: مسیر فایل امبدینگ.
-
-    """
-
-    def __init__(
-        self: "WordEmbedding",
-        model_type: str,
-        model_path: str = None,
-    ) -> None:
-        if model_type not in supported_embeddings:
-            msg = (
-                f'Model type "{model_type}" is not supported! Please choose from'
-                f" {supported_embeddings}"
-            )
-            raise KeyError(
-                msg,
-            )
-        self.model_type = model_type
-        if model_path:
-            self.load_model(model_path)
-
-    def load_model(self: "WordEmbedding", model_path: str) -> None:
-        """فایل امبدینگ را بارگزاری می‌کند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
-            >>> wordEmbedding.load_model('resources/cc.fa.300.bin')
-
-        Args:
-            model_path: مسیر فایل امبدینگ.
-
-        """
-        if self.model_type == "fasttext":
-            self.model = fasttext.load_facebook_model(model_path).wv
-        elif self.model_type == "keyedvector":
-            if model_path.endswith("bin"):
-                self.model = KeyedVectors.load_word2vec_format(model_path, binary=True)
-            else:
-                self.model = KeyedVectors.load_word2vec_format(model_path)
-        elif self.model_type == "glove":
-            word2vec_addr = str(model_path) + "_word2vec_format.vec"
-            if not Path.exists(word2vec_addr):
-                _ = glove2word2vec(model_path, word2vec_addr)
-            self.model = KeyedVectors.load_word2vec_format(word2vec_addr)
-            self.model_type = "keyedvector"
-        else:
-            msg = (
-                f"{self.model_type} not supported! Please choose from"
-                f" {supported_embeddings}"
-            )
-            raise KeyError(
-                msg,
-            )
-
-    def train(
-        self: "WordEmbedding",
-        dataset_path: str,
-        workers: int = multiprocessing.cpu_count() - 1,  # noqa: B008
-        vector_size: int = 200,
-        epochs: int = 10,
-        fasttext_type: str = "skipgram",
-        dest_path: str = None,
-    ) -> None:
-        """یک فایل امبدینگ از نوع fasttext ترین می‌کند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
-            >>> wordEmbedding.train(dataset_path = 'dataset.txt', worker = 4, vector_size = 300, epochs = 30, fasttext_type = 'cbow', dest_path = 'fasttext_model')
-
-        Args:
-            dataset_path: مسیر فایل متنی.
-            workers: تعداد هسته درگیر برای ترین مدل.
-            vector_size: طول وکتور خروجی به ازای هر کلمه.
-            epochs: تعداد تکرار ترین بر روی کل دیتا.
-            fasttext_type: نوع fasttext مورد نظر برای ترین که میتواند یکی از مقادیر skipgram یا cbow را داشته باشد.
-            dest_path: مسیر مورد نظر برای ذخیره فایل امبدینگ.
-
-        """
-        if self.model_type != "fasttext":
-            self.model = "fasttext"
-            warnings.warn(
-                (
-                    "this function is for training fasttext models only and"
-                    f" {self.model_type} is not supported"
-                ),
-                stacklevel=2,
-            )
-
-        fasttext_model_types = ["cbow", "skipgram"]
-        if fasttext_type not in fasttext_model_types:
-            msg = (
-                f'Model type "{fasttext_type}" is not supported! Please choose from'
-                f" {fasttext_model_types}"
-            )
-            raise KeyError(
-                msg,
-            )
-
-        workers = 1 if workers == 0 else workers
-
-        model = fasttext.train_unsupervised(
-            dataset_path,
-            model=fasttext_type,
-            dim=vector_size,
-            epoch=epochs,
-            thread=workers,
-        )
-
-        self.model = model.wv
-
-        print("Model trained.")
-
-        if dest_path is not None:
-            model.save_model(dest_path)
-            print("Model saved.")
-
-    def __getitem__(self: "WordEmbedding", word: str) -> str:
-        """__getitem__."""
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return self.model[word]
-
-    def doesnt_match(self: "WordEmbedding", words: List[str]) -> str:
-        """لیستی از کلمات را دریافت می‌کند و کلمهٔ نامرتبط را برمی‌گرداند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
-            >>> wordEmbedding.doesnt_match(['سلام' ,'درود' ,'خداحافظ' ,'پنجره'])
-            'پنجره'
-            >>> wordEmbedding.doesnt_match(['ساعت' ,'پلنگ' ,'شیر'])
-            'ساعت'
-
-        Args:
-            words: لیست کلمات.
-
-        Returns:
-            کلمهٔ نامرتبط.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return self.model.doesnt_match(words)
-
-    def similarity(self: "WordEmbedding", word1: str, word2: str) -> float:
-        """میزان شباهت دو کلمه را برمی‌گرداند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
-            >>> wordEmbedding.similarity('ایران', 'آلمان')
-            0.44988164
-            >>> wordEmbedding.similarity('ایران', 'پنجره')
-            0.08837362
-
-        Args:
-            word1: کلمهٔ اول
-            word2: کلمهٔ دوم
-
-        Returns:
-            میزان شباهت دو کلمه.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return float(str(self.model.similarity(word1, word2)))
-
-    def get_vocab(self: "WordEmbedding") -> List[str]:
-        """لیستی از کلمات موجود در فایل امبدینگ را برمی‌گرداند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
-            >>> wordEmbedding.get_vocab()
-            ['،', 'در', '.', 'و', ...]
-
-        Returns:
-            لیست کلمات موجود در فایل امبدینگ.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return self.model.index_to_key
-
-    def nearest_words(
-        self: "WordEmbedding",
-        word: str,
-        topn: int = 5,
-    ) -> List[Tuple[str, str]]:
-        """کلمات مرتبط با یک واژه را به همراه میزان ارتباط آن برمی‌گرداند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
-            >>> wordEmbedding.nearest_words('ایران', topn = 5)
-            [('ايران', 0.657148540019989'), (جمهوری', 0.6470394134521484'), (آمریکا', 0.635792076587677'), (اسلامی', 0.6354473233222961'), (کشور', 0.6339613795280457')]
-
-        Args:
-            word: کلمه‌ای که می‌خواهید واژگان مرتبط با آن را بدانید.
-            topn: تعداد کلمات مرتبطی که می‌خواهید برگردانده شود.
-
-        Returns:
-            لیستی از تاپل‌های [`کلمهٔ مرتبط`, `میزان ارتباط`].
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return self.model.most_similar(word, topn=topn)
-
-    def get_normal_vector(self: "WordEmbedding", word: str) -> Type[ndarray]:
-        """بردار امبدینگ نرمالایزشدهٔ کلمه ورودی را برمی‌گرداند.
-
-        Examples:
-            >>> wordEmbedding = WordEmbedding(model_type = 'model_type', model_path = 'resources/cc.fa.300.bin')
-            >>> wordEmbedding.get_normal_vector('سرباز')
-            array([ 8.99544358e-03,  2.76231226e-02, -1.06164828e-01, ..., -9.45233554e-02, -7.59726465e-02, -8.96625668e-02], dtype=float32)
-
-        Args:
-            word: کلمه‌ای که می‌خواهید بردار متناظر با آن را بدانید.
-
-        Returns:
-            لیست بردار نرمالایزشدهٔ مرتبط با کلمهٔ ورودی.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-
-        return self.model.get_vector(word=word, norm=True)
-
-
-class SentEmbedding:
-    """این کلاس شامل توابعی برای تبدیل جمله به برداری از اعداد است.
-
-    Args:
-        model_path: مسیر فایل امبدینگ.
-
-    """
-
-    def __init__(self: "SentEmbedding", model_path: str = None) -> None:
-        if model_path:
-            self.load_model(model_path)
-
-    def load_model(self: "SentEmbedding", model_path: str) -> None:
-        """فایل امبدینگ را بارگذاری می‌کند.
-
-        Examples:
-            >>> sentEmbedding = SentEmbedding()
-            >>> sentEmbedding.load_model('sent2vec_model_path')
-
-        Args:
-            model_path: مسیر فایل امبدینگ.
-
-        """
-        self.model = Doc2Vec.load(model_path)
-
-    def train(
-        self: "SentEmbedding",
-        dataset_path: str,
-        min_count: int = 5,
-        workers: int = multiprocessing.cpu_count() - 1,  # noqa: B008
-        windows: int = 5,
-        vector_size: int = 300,
-        epochs: int = 10,
-        dest_path: str = None,
-    ) -> None:
-        """یک فایل امبدینگ doc2vec ترین می‌کند.
-
-        Examples:
-            >>> sentEmbedding = SentEmbedding()
-            >>> sentEmbedding.train(dataset_path = 'dataset.txt', min_count = 10, worker = 6, windows = 3, vector_size = 250, epochs = 35, dest_path = 'doc2vec_model')
-
-        Args:
-            dataset_path: مسیر فایل متنی.
-            min_count: مینیموم دفعات تکرار یک کلمه برای حضور آن در لیست کلمات امبدینگ.
-            workers: تعداد هسته درگیر برای ترین مدل.
-            windows: طول پنجره برای لحاظ کلمات اطراف یک کلمه در ترین آن.
-            vector_size: طول وکتور خروجی به ازای هر جمله.
-            epochs: تعداد تکرار ترین بر روی کل دیتا.
-            dest_path: مسیر مورد نظر برای ذخیره فایل امبدینگ.
-
-        """
-        workers = 1 if workers == 0 else workers
-
-        doc = SentenceEmbeddingCorpus(dataset_path)
-
-        model = Doc2Vec(
-            min_count=min_count,
-            window=windows,
-            vector_size=vector_size,
-            workers=workers,
-        )
-        model.build_vocab(doc)
-        model.train(doc, total_examples=model.corpus_count, epochs=epochs)
-
-        self.model = model
-
-        print("Model trained.")
-
-        if dest_path is not None:
-            model.save(dest_path)
-            print("Model saved.")
-
-    def __getitem__(self: "SentEmbedding", sent: str) -> Type[ndarray]:
-        """__getitem__."""
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-        return self.get_sentence_vector(sent)
-
-    def get_sentence_vector(self: "SentEmbedding", sent: str) -> str:
-        """جمله‌ای را دریافت می‌کند و بردار امبدینگ متناظر با آن را برمی‌گرداند.
-
-        Examples:
-            >>> sentEmbedding = SentEmbedding(sent_embedding_file)
-            >>> sentEmbedding.get_sentence_vector('این متن به برداری متناظر با خودش تبدیل خواهد شد')
-            array([-0.28460968,  0.04566888, -0.00979532, ..., -0.4701098 , -0.3010612 , -0.18577948], dtype=float32)
-
-        Args:
-            sent: جمله‌ای که می‌خواهید بردار امبیدنگ آن را دریافت کنید.
-
-        Returns:
-            لیست بردار مرتبط با جملهٔ ورودی.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-
-        tokenized_sent = word_tokenize(sent)
-        return self.model.infer_vector(tokenized_sent)
-
-    def similarity(self: "SentEmbedding", sent1: str, sent2: str) -> float:
-        """میزان شباهت دو جمله را برمی‌گرداند.
-
-        Examples:
-            >>> sentEmbedding = SentEmbedding(sent_embedding_file)
-            >>> sentEmbedding.similarity('شیر حیوانی وحشی است', 'پلنگ از دیگر جانوران درنده است')
-            0.8748713
-            >>> sentEmbedding.similarity('هضم یک محصول پردازش متن فارسی است', 'شیر حیوانی وحشی است')
-            0.2379288
-
-        Args:
-            sent1: جملهٔ اول.
-            sent2: جملهٔ دوم.
-
-        Returns:
-            میزان شباهت دو جمله که عددی بین `0` و`1` است.
-
-        """
-        if not self.model:
-            msg = "Model must not be None! Please load model first."
-            raise AttributeError(msg)
-
-        return float(
-            str(
-                self.model.similarity_unseen_docs(
-                    word_tokenize(sent1),
-                    word_tokenize(sent2),
-                ),
-            ),
-        )
-
-
-class SentenceEmbeddingCorpus:
-    """SentenceEmbeddingCorpus."""
-
-    def __init__(self: "SentenceEmbeddingCorpus", data_path: str) -> None:
-        """__init__."""
-        self.data_path = data_path
-
-    def __iter__(self: "SentenceEmbeddingCorpus") -> Iterator[TaggedDocument]:
-        """__iter__."""
-        corpus_path = datapath(self.data_path)
-        
-        for i, list_of_words in enumerate(Path.open(corpus_path)):
-            yield TaggedDocument(
-                word_tokenize(Normalizer().normalize(list_of_words)),
-                [i],
-            )
+"""این ماژول شامل کلاس‌ها و توابعی برای تبدیل کلمه یا متن به برداری از اعداد است."""
+import multiprocessing
+import os
+import warnings
+from pathlib import Path
+from typing import Any
+from typing import Iterator
+from typing import List
+from typing import Optional
+from typing import Tuple
+from typing import Type
+
+import fasttext as fstxt
+import numpy as np
+import smart_open
+from gensim.models import Doc2Vec
+from gensim.models import KeyedVectors
+from gensim.models import fasttext
+from gensim.models.callbacks import CallbackAny2Vec
+from gensim.models.doc2vec import TaggedDocument
+from gensim.scripts.glove2word2vec import glove2word2vec
+from gensim.test.utils import datapath
+from numpy import ndarray
+
+from hazm import Normalizer
+from hazm import word_tokenize
+
+supported_embeddings = ["fasttext", "keyedvector", "glove"]
+
+
+class WordEmbedding:
+    """این کلاس شامل توابعی برای تبدیل کلمه به برداری از اعداد است.
+
+    Args:
+        model_type: نوع امبدینگ که می‌تواند یکی از مقادیر ‍`fasttext`, `keyedvector`, `glove` باشد.
+        model_path: مسیر فایل امبدینگ.
+
+    """
+
+    def __init__(
+        self: "WordEmbedding",
+        model_type: str,
+        model_path: Optional[str] = None,
+    ) -> None:
+        if model_type not in supported_embeddings:
+            msg = (
+                f'Model type "{model_type}" is not supported! Please choose from'
+                f" {supported_embeddings}"
+            )
+            raise KeyError(
+                msg,
+            )
+        self.model_type = model_type
+        if model_path:
+            self.load_model(model_path)
+
+    def load_model(self: "WordEmbedding", model_path: str) -> None:
+        """فایل امبدینگ را بارگزاری می‌کند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.load_model('word2vec.bin') # doctest: +ELLIPSIS
+            ...
+
+        Args:
+            model_path: مسیر فایل امبدینگ.
+
+        """
+        if self.model_type == "fasttext":
+            self.model = fasttext.load_facebook_model(model_path).wv
+        elif self.model_type == "keyedvector":
+            if model_path.endswith("bin"):
+                self.model = KeyedVectors.load_word2vec_format(model_path, binary=True)
+            else:
+                self.model = KeyedVectors.load_word2vec_format(model_path)
+        elif self.model_type == "glove":
+            word2vec_addr = str(model_path) + "_word2vec_format.vec"
+            if not Path.exists(word2vec_addr):
+                _ = glove2word2vec(model_path, word2vec_addr)
+            self.model = KeyedVectors.load_word2vec_format(word2vec_addr)
+            self.model_type = "keyedvector"
+        else:
+            msg = (
+                f"{self.model_type} not supported! Please choose from"
+                f" {supported_embeddings}"
+            )
+            raise KeyError(
+                msg,
+            )
+
+    def train(
+        self: "WordEmbedding",
+        dataset_path: str,
+        workers: int = multiprocessing.cpu_count() - 1,  # noqa: B008
+        vector_size: int = 200,
+        epochs: int = 10,
+        min_count: int = 5,
+        fasttext_type: str = "skipgram",
+        dest_path: str = "fasttext_word2vec_model.bin",
+    ) -> None:
+        """یک فایل امبدینگ از نوع fasttext ترین می‌کند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.train(dataset_path = 'dataset.txt', workers = 4, vector_size = 300, epochs = 30, fasttext_type = 'cbow', dest_path = 'fasttext_model') # doctest: +ELLIPSIS
+            ...
+
+        Args:
+            dataset_path: مسیر فایل متنی.
+            workers: تعداد هسته درگیر برای ترین مدل.
+            vector_size: طول وکتور خروجی به ازای هر کلمه.
+            epochs: تعداد تکرار ترین بر روی کل دیتا.
+            min_count:  حداقل تعداد تکرار یک کلمه برای قرارگیری آن در مدل امبدینگ.
+            fasttext_type: نوع fasttext مورد نظر برای ترین که میتواند یکی از مقادیر skipgram یا cbow را داشته باشد.
+            dest_path: مسیر مورد نظر برای ذخیره فایل امبدینگ.
+
+        """
+        if self.model_type != "fasttext":
+            self.model = "fasttext"
+            warnings.warn(
+                (
+                    "this function is for training fasttext models only and"
+                    f" {self.model_type} is not supported"
+                ),
+                stacklevel=2,
+            )
+
+        fasttext_model_types = ["cbow", "skipgram"]
+        if fasttext_type not in fasttext_model_types:
+            msg = (
+                f'Model type "{fasttext_type}" is not supported! Please choose from'
+                f" {fasttext_model_types}"
+            )
+            raise KeyError(
+                msg,
+            )
+
+        workers = 1 if workers == 0 else workers
+
+        print("training model...")
+        model = fstxt.train_unsupervised(
+            dataset_path,
+            model=fasttext_type,
+            dim=vector_size,
+            epoch=epochs,
+            thread=workers,
+            min_count = min_count,
+        )
+
+        print("Model trained.")
+
+        print("saving model...")
+        model.save_model(dest_path)
+        print("Model saved.")
+
+        print("loading model...")
+        self.load_model(model_path=dest_path)
+        print("model loaded.")
+
+    def __getitem__(self: "WordEmbedding", word: str) -> Type[ndarray]:
+        """__getitem__."""
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+        return self.model[word]
+
+    def doesnt_match(self: "WordEmbedding", words: List[str]) -> str:
+        """لیستی از کلمات را دریافت می‌کند و کلمهٔ نامرتبط را برمی‌گرداند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.load_model('word2vec.bin')
+            >>> wordEmbedding.doesnt_match(['سلام' ,'درود' ,'خداحافظ' ,'پنجره'])
+            'پنجره'
+            >>> wordEmbedding.doesnt_match(['ساعت' ,'پلنگ' ,'شیر'])
+            'ساعت'
+
+        Args:
+            words: لیست کلمات.
+
+        Returns:
+            کلمهٔ نامرتبط.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+        return self.model.doesnt_match(words)
+
+    def similarity(self: "WordEmbedding", word1: str, word2: str) -> float:
+        """میزان شباهت دو کلمه را برمی‌گرداند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.load_model('word2vec.bin')
+            >>> wordEmbedding.similarity('ایران', 'آلمان')
+            0.72231203
+            >>> wordEmbedding.similarity('ایران', 'پنجره')
+            0.04535884
+
+        Args:
+            word1: کلمهٔ اول
+            word2: کلمهٔ دوم
+
+        Returns:
+            میزان شباهت دو کلمه.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+
+        return float(str(self.model.similarity(word1, word2)))
+
+    def nearest_words(
+        self: "WordEmbedding",
+        word: str,
+        topn: int = 5,
+    ) -> List[Tuple[str, str]]:
+        """کلمات مرتبط با یک واژه را به همراه میزان ارتباط آن برمی‌گرداند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.load_model('word2vec.bin')
+            >>> wordEmbedding.nearest_words('ایران', topn = 5)
+            [('ایران،', 0.8742443919181824), ('کشور', 0.8735059499740601), ('کشورمان', 0.8443885445594788), ('ایران\u200cبه', 0.8271722197532654), ('خاورمیانه', 0.8266966342926025)]
+
+
+        Args:
+                word: کلمه‌ای که می‌خواهید واژگان مرتبط با آن را بدانید.
+                topn: تعداد کلمات مرتبطی که می‌خواهید برگردانده شود.
+
+        Returns:
+            لیستی از تاپل‌های [`کلمهٔ مرتبط`, `میزان ارتباط`].
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+        return self.model.most_similar(word, topn=topn)
+
+    def get_normal_vector(self: "WordEmbedding", word: str) -> Type[ndarray]:
+        """بردار امبدینگ نرمالایزشدهٔ کلمه ورودی را برمی‌گرداند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.load_model('word2vec.bin')
+            >>> result = wordEmbedding.get_normal_vector('سرباز')
+            >>> isinstance(result, ndarray)
+            True
+
+        Args:
+            word: کلمه‌ای که می‌خواهید بردار متناظر با آن را بدانید.
+
+        Returns:
+            لیست بردار نرمالایزشدهٔ مرتبط با کلمهٔ ورودی.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+
+        return self.model.get_vector(word=word, norm=True)
+
+    def get_vocabs(self: "WordEmbedding") -> List[str]:
+        """لیستی از کلمات موجود در فایل امبدینگ را برمی‌گرداند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.load_model('word2vec.bin')
+            >>> wordEmbedding.get_vocabs() # doctest: +ELLIPSIS
+            ['و', '.', 'در', '،', ...]
+
+        Returns:
+            لیست کلمات موجود در فایل امبدینگ.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+        return self.model.index_to_key
+
+    def get_vocab_to_index(self: "WordEmbedding") -> dict:
+        """دیکشنری برمی‌گرداند که هر کلمه موجود در فایل امبدینگ را به ایندکس آن کلمه در لیست بردارها مپ می‌کند.
+
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.load_model('word2vec.bin)
+            >>> vocab_to_index = wordEmbedding.get_vocab_to_index()
+            >>> index = vocab_to_index['سلام']
+            >>> vocabs = wordEmbedding.get_vocabs()
+            >>> vocabs[index]
+            'سلام'
+
+        Returns:
+            دیکشنری که هر کلمه را به ایندکس آن مپ می‌کند.
+        """
+        return self.model.key_to_index
+
+    def get_vectors(self: "WordEmbedding") -> Type[ndarray]:
+        """وکتورهای توصیف کننده کلمات را برمیگرداند.(عناصر این وکتور با وکتور کلمات تابع  get_vocabs هم‌اندیس هستند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.load_model('resorces/word2vec.bin')
+            >>> vectors = wordEmbedding.get_vectors()
+            >>> all(vectors[wordEmbedding.get_vocab_to_index()['سلام']] == wordEmbedding['سلام'])
+            True
+
+        Returns:
+            تمامی وکتور بیان‌کننده کلمات.
+        """
+        return self.model.vectors
+
+    def get_vector_size(self: "WordEmbedding") -> int:
+        """طول وکتور بیان‌کننده هر کلمه در مدل را برمی‌گرداند.
+
+        Examples:
+            >>> wordEmbedding = WordEmbedding(model_type = 'fasttext')
+            >>> wordEmbedding.load_model('resorces/word2vec.bin')
+            >>> wordEmbedding.get_vector_size()
+            300
+
+
+        Returns:
+            طول وکتور بیان‌کننده کلمات.
+
+        """
+        return self.model.vector_size
+
+
+class SentenceEmbeddingCorpus:
+    """SentenceEmbeddingCorpus."""
+
+    def __init__(self: "SentenceEmbeddingCorpus", data_path: str) -> None:
+        """__init__."""
+        self.data_path = data_path
+
+    def __iter__(self: "SentenceEmbeddingCorpus") -> Iterator[TaggedDocument]:
+        """__iter__."""
+        for i, list_of_words in enumerate(smart_open.open(self.data_path)):
+            yield TaggedDocument(
+                word_tokenize(Normalizer().normalize(list_of_words)),
+                [i],
+            )
+
+class CallbackSentEmbedding(CallbackAny2Vec):
+    def __init__(self: "CallbackSentEmbedding") -> None:
+        self.epoch = 0
+
+    def on_epoch_end(self: "CallbackSentEmbedding", model: Doc2Vec):
+        print(f"Epoch {self.epoch+1} of {model.epochs}...")
+        self.epoch += 1
+
+
+class SentEmbedding:
+    """این کلاس شامل توابعی برای تبدیل جمله به برداری از اعداد است.
+
+    Args:
+        model_path: مسیر فایل امبدینگ.
+
+    """
+
+    def __init__(self: "SentEmbedding", model_path: Optional[str] = None) -> None:
+        if model_path:
+            self.load_model(model_path)
+            self.__load_word_embedding_model()
+
+    def __load_word_embedding_model(self: "SentEmbedding") -> None:
+        self.word_embedding = WordEmbedding(model_type="keyedvector")
+        self.word_embedding.model = self.model.wv
+
+    def load_model(self: "SentEmbedding", model_path: str) -> None:
+        """فایل امبدینگ را بارگذاری می‌کند.
+
+        Examples:
+            >>> sentEmbedding = SentEmbedding()
+            >>> sentEmbedding.load_model('sent2vec.model') # doctest: +ELLIPSIS
+            ...
+
+        Args:
+            model_path: مسیر فایل امبدینگ.
+
+        """
+        self.model = Doc2Vec.load(model_path)
+        self.__load_word_embedding_model()
+
+    def train(
+        self: "SentEmbedding",
+        dataset_path: str,
+        min_count: int = 5,
+        workers: int = multiprocessing.cpu_count() - 1,  # noqa: B008
+        windows: int = 5,
+        vector_size: int = 300,
+        epochs: int = 10,
+        dest_path: str = "gensim_sent2vec.model",
+    ) -> None:
+        """یک فایل امبدینگ doc2vec ترین می‌کند.
+
+        Examples:
+            >>> sentEmbedding = SentEmbedding()
+            >>> sentEmbedding.train(dataset_path = 'dataset.txt', min_count = 10, workers = 6, windows = 3, vector_size = 250, epochs = 35, dest_path = 'doc2vec_model') # doctest: +ELLIPSIS
+            ...
+
+        Args:
+            dataset_path: مسیر فایل متنی.
+            min_count: حداقل تعداد تکرار یک کلمه برای قرارگیری آن در مدل امبدینگ.
+            workers: تعداد هسته درگیر برای ترین مدل.
+            windows: طول پنجره برای لحاظ کلمات اطراف یک کلمه در ترین آن.
+            vector_size: طول وکتور خروجی به ازای هر جمله.
+            epochs: تعداد تکرار ترین بر روی کل دیتا.
+            dest_path: مسیر مورد نظر برای ذخیره فایل امبدینگ.
+
+        """
+        workers = 1 if workers == 0 else workers
+
+        doc = SentenceEmbeddingCorpus(dataset_path)
+
+        model = Doc2Vec(
+            min_count=min_count,
+            window=windows,
+            vector_size=vector_size,
+            workers=workers,
+        )
+        print("building vocab...")
+        model.build_vocab(doc)
+        print("training model...")
+        callbacks = [CallbackSentEmbedding()]
+        model.train(doc, total_examples=model.corpus_count, epochs=epochs, callbacks=callbacks)
+
+        model.dv.vectors = np.array([[]])
+        self.model = model
+        self.__load_word_embedding_model()
+        print("Model trained.")
+
+        print("saving model...")
+        model.save(dest_path)
+        print("Model saved.")
+
+    def __getitem__(self: "SentEmbedding", sent: str) -> Type[ndarray]:
+        """__getitem__."""
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+        return self.get_sentence_vector(sent)
+
+    def get_sentence_vector(self: "SentEmbedding", sent: str) -> ndarray:
+        """جمله‌ای را دریافت می‌کند و بردار امبدینگ متناظر با آن را برمی‌گرداند.
+
+        Examples:
+            >>> sentEmbedding = SentEmbedding()
+            >>> sentEmbedding.load_model("sent2vec.model")
+            >>> result = sentEmbedding.get_sentence_vector('این متن به برداری متناظر با خودش تبدیل خواهد شد')
+            >>> isinstance(result, ndarray)
+            True
+
+        Args:
+            sent: جمله‌ای که می‌خواهید بردار امبیدنگ آن را دریافت کنید.
+
+        Returns:
+            لیست بردار مرتبط با جملهٔ ورودی.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+
+        tokenized_sent = word_tokenize(sent)
+        return self.model.infer_vector(tokenized_sent)
+
+    def similarity(self: "SentEmbedding", sent1: str, sent2: str) -> float:
+        """میزان شباهت دو جمله را برمی‌گرداند.
+
+        Examples:
+            >>> sentEmbedding = SentEmbedding()
+            >>> sentEmbedding.load_model("sent2vec.model")
+            >>> result = sentEmbedding.similarity('شیر حیوانی وحشی است', 'پلنگ از دیگر جانوران درنده است')
+            >>> isinstance(result, float)
+            True
+            >>> result = sentEmbedding.similarity('هضم یک محصول پردازش متن فارسی است', 'شیر حیوانی وحشی است')
+            >>> isinstance(result, float)
+            True
+
+        Args:
+            sent1: جملهٔ اول.
+            sent2: جملهٔ دوم.
+
+        Returns:
+            میزان شباهت دو جمله که عددی بین `0` و`1` است.
+
+        """
+        if not self.model:
+            msg = "Model must not be None! Please load model first."
+            raise AttributeError(msg)
+
+        return float(
+            str(
+                self.model.similarity_unseen_docs(
+                    word_tokenize(sent1),
+                    word_tokenize(sent2),
+                ),
+            ),
+        )
+
+    def get_vector_size(self: "WordEmbedding") -> int:
+        """طول وکتور بیان‌کننده هر جمله در مدل را برمی‌گرداند.
+
+        Examples:
+            >>> sentEmbedding = SentEmbedding()
+            >>> sentEmbedding.load_model("sent2vec.model")
+            >>> sentEmbedding.get_vector_size()
+            300
+
+
+        Returns:
+            طول وکتور بیان‌کننده جملات.
+
+        """
+        return self.model.vector_size
```

### Comparing `hazm-0.9.1/hazm/informal_normalizer.py` & `hazm-0.9.2/hazm/informal_normalizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,856 +1,856 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای نرمال‌سازی متن‌های محاوره‌ای است."""
-
-
-import re
-from pathlib import Path
-from typing import List
-
-from hazm import Lemmatizer
-from hazm import Normalizer
-from hazm import SentenceTokenizer
-from hazm import Stemmer
-from hazm import NUMBERS
-from hazm import informal_verbs
-from hazm import informal_words
-from hazm import WordTokenizer
-from hazm import default_verbs
-
-
-class InformalNormalizer(Normalizer):
-    """این کلاس شامل توابعی برای نرمال‌سازی متن‌های محاوره‌ای است.
-
-    Args:
-        verb_file: فایل حاوی افعال محاوره‌ای.
-        word_file: فایل حاوی کلمات محاوره‌ای.
-        seperation_flag: اگر `True` باشد و در بخشی از متن به فاصله نیاز بود آن فاصله درج می‌شود.
-        **kargs: پارامترهای نامدارِ اختیاری
-
-    """
-
-    def __init__(
-        self: "InformalNormalizer",
-        verb_file: str = informal_verbs,
-        word_file: str = informal_words,
-        seperation_flag: bool = False,
-        **kargs: str,
-    ) -> None:
-        self.seperation_flag = seperation_flag
-        self.lemmatizer = Lemmatizer()
-        self.ilemmatizer = InformalLemmatizer()
-        self.stemmer = Stemmer()
-        super().__init__(**kargs)
-
-        self.sent_tokenizer = SentenceTokenizer()
-        self.word_tokenizer = WordTokenizer()
-
-        with Path.open(verb_file, encoding="utf8") as vf:
-            self.pastVerbs = {}
-            self.presentVerbs = {}
-            for f, i, _flag in [x.strip().split(" ", 2) for x in vf]:
-                splitedf = f.split("#")
-                self.presentVerbs.update({i: splitedf[1]})
-                self.pastVerbs.update({splitedf[0]: splitedf[0]})
-        with Path.open(default_verbs, encoding="utf8") as vf:
-            for f, i in [x.strip().split("#", 2) for x in vf]:
-                self.presentVerbs.update({i: i})
-                self.pastVerbs.update({f: f})
-
-        def informal_to_formal_conjucation(i, f, flag):
-            iv = self.informal_conjugations(i)
-            fv = self.lemmatizer.conjugation.get_all(f)
-            res = {}
-            if flag:
-                for i, j in zip(iv, fv[48:]):
-                    res[i] = j
-                    if "‌" in i:
-                        res[i.replace("‌", "")] = j
-                        res[i.replace("‌", " ")] = j
-                    if i.endswith("ین"):
-                        res[i[:-1] + "د"] = j
-            else:
-                for i, j in zip(iv[8:], fv[56:]):
-                    res[i] = j
-                    if "‌" in i:
-                        res[i.replace("‌", "")] = j
-                        res[i.replace("‌", " ")] = j
-                    if i.endswith("ین"):
-                        res[i[:-1] + "د"] = j
-
-            return res
-
-        with Path.open(verb_file, encoding="utf8") as vf:
-            self.iverb_map = {}
-            for f, i, flag in [x.strip().split(" ", 2) for x in vf]:
-                self.iverb_map.update(informal_to_formal_conjucation(i, f, flag))
-
-        with Path.open(word_file, encoding="utf8") as wf:
-            self.iword_map = dict([x.strip().split(" ", 1) for x in wf])
-
-        self.words = set()
-        if self.seperation_flag:
-            self.words.update(list(self.iword_map.keys()))
-            self.words.update(list(self.iword_map.values()))
-            self.words.update(list(self.iverb_map.keys()))
-            self.words.update(list(self.iverb_map.values()))
-            self.words.update(self.lemmatizer.words)
-            self.words.update(list(self.lemmatizer.verbs.keys()))
-            self.words.update(list(self.lemmatizer.verbs.values()))
-
-    def split_token_words(self: "InformalNormalizer", token: str) -> str:
-        """هرجایی در متن فاصله نیاز بود قرار می‌دهد.
-
-        متأسفانه در برخی از متن‌ها، به بهانهٔ صرفه‌جویی در زمان یا از سرِ تنبلی،
-        فاصله‌گذاری‌ها درست رعایت نمی‌شود. مثلاً جملهٔ «تو را دوست دارم.» به این
-        شکل نوشته می‌شود: «تورادوست دارم.» این تابع فواصل ضروری را در متن
-        ایجاد می‌کند و آن را به شکل صحیح برمی‌گرداند.
-
-        Args:
-            token: توکنی که باید فاصله‌گذاری شود.
-
-        Returns:
-            توکنی با فاصله‌گذاری صحیح.
-
-        """
-
-        def shekan(token):
-            res = [""]
-            for i in token:
-                res[-1] += i
-                if i in {"ا", "د", "ذ", "ر", "ز", "ژ", "و", *list(NUMBERS)}:
-                    res.append("")
-            while "" in res:
-                res.remove("")
-            return res
-
-        def perm(lst):
-            if len(lst) > 1:
-                up = perm(lst[1:])
-            else:
-                return [lst]
-            res = []
-            for i in up:
-                res.append([lst[0], *i])
-                res.append([lst[0] + i[0]] + i[1:])
-            res.sort(key=len)
-            return res
-
-        token = re.sub(r"(.)\1{2,}", r"\1", token)
-        ps = perm(shekan(token))
-        for c in ps:
-            if {self.ilemmatizer.lemmatize(x) for x in c}.issubset(self.words):
-                return " ".join(c)
-        return token
-
-    def normalized_word(self: "InformalNormalizer", word: str) -> List[str]:
-        """اشکال مختلف نرمالایزشدهٔ کلمه را برمی‌گرداند.
-
-        Examples:
-            >>> normalizer = InformalNormalizer()
-            >>> normalizer.normalized_word('می‌رم')
-            ['می‌روم']
-
-        Args:
-            word: کلمه‌ای که باید نرمال‌سازی شود.
-
-        Returns:
-            اشکال نرمالایزشدهٔ کلمه.
-
-        """
-        # >>> normalizer = InformalNormalizer(seperation_flag=True)
-        # >>> normalizer.normalized_word('صداوسیماجمهوری')
-
-        def analyze_word(word):
-            end_words_list = [
-                "هاست",
-                "هایی",
-                "هایم",
-                "ترین",
-                "ایی",
-                "انی",
-                "شان",
-                "شون",
-                "است",
-                "تان",
-                "تون",
-                "مان",
-                "مون",
-                "هام",
-                "هاش",
-                "های",
-                "طور",
-                "ها",
-                "تر",
-                "ئی",
-                "یی",
-                "یم",
-                "ام",
-                "ای",
-                "ان",
-                "هم",
-                "رو",
-                "یت",
-                "ه",
-                "ی",
-                "ش",
-                "و",
-                "ا",
-                "ت",
-                "م",
-            ]
-
-            return_list = []
-
-            collection_of_word_and_suffix = []
-
-            found_early = False
-
-            mid_word_condidate = []
-
-            if word.endswith(("\u200c", "\u200e")):
-                word = word[:-1]
-
-            if word in self.lemmatizer.words or word in self.iword_map:
-                if word in self.lemmatizer.words:
-                    collection_of_word_and_suffix.append({"word": word, "suffix": []})
-                if word in self.iword_map:
-                    collection_of_word_and_suffix.append(
-                        {"word": self.iword_map[word], "suffix": []},
-                    )
-                found_early = True
-
-            if not found_early:
-                for endword in end_words_list:
-                    if word.endswith(endword):
-                        sliceword = word[: -1 * len(endword)]
-                        if (
-                            sliceword in self.lemmatizer.words
-                            or sliceword in self.iword_map
-                        ):
-                            if sliceword in self.lemmatizer.words:
-                                collection_of_word_and_suffix.append(
-                                    {"word": sliceword, "suffix": [endword]},
-                                )
-                            if sliceword in self.iword_map:
-                                collection_of_word_and_suffix.append(
-                                    {
-                                        "word": self.iword_map[sliceword],
-                                        "suffix": [endword],
-                                    },
-                                )
-                        else:
-                            mid_word_condidate.append(sliceword)
-                            mid_word_condidate.append([endword])
-
-                for endword in end_words_list:
-                    for i in range(len(mid_word_condidate) - 1):
-                        if i % 2 == 1:
-                            continue
-                        midword = mid_word_condidate[i]
-                        mid_word_end_word_list = mid_word_condidate[i + 1]
-                        if midword.endswith(endword):
-                            sliceword = midword[: -1 * len(endword)]
-                            if (
-                                sliceword in self.lemmatizer.words
-                                or sliceword in self.iword_map
-                            ):
-                                if sliceword in self.lemmatizer.words:
-                                    collection_of_word_and_suffix.append(
-                                        {
-                                            "word": sliceword,
-                                            "suffix": [
-                                                endword,
-                                                *mid_word_end_word_list,
-                                            ],
-                                        },
-                                    )
-                                if sliceword in self.iword_map:
-                                    collection_of_word_and_suffix.append(
-                                        {
-                                            "word": self.iword_map[sliceword],
-                                            "suffix": [
-                                                endword,
-                                                *mid_word_end_word_list,
-                                            ],
-                                        },
-                                    )
-
-            for i in range(len(collection_of_word_and_suffix)):
-                new_possible_word_list = append_suffix_to_word(
-                    collection_of_word_and_suffix[i],
-                )
-                for j in range(len(new_possible_word_list)):
-                    new_possible_word = new_possible_word_list[j]
-                    if new_possible_word not in return_list:
-                        return_list.append(new_possible_word)
-
-            return return_list
-
-        def analyze_verb_word(word):
-            if word in self.pastVerbs:
-                word = self.pastVerbs[word]
-                return [word]
-
-            if word in self.iword_map:
-                return []
-
-            if word in self.lemmatizer.words:
-                if word[-1] == "ن":
-                    None  # noqa: B018
-                else:
-                    return []
-
-            return_list = []
-
-            collection_of_verb_list = []
-
-            end_verb_list = [
-                "یم",
-                "دم",
-                "دیم",
-                "ید",
-                "دی",
-                "دید",
-                "ند",
-                "دن",
-                "دند",
-                "ین",
-                "دین",
-                "ست",
-                "ستم",
-                "ستی",
-                "ستیم",
-                "ستید",
-                "ستند",
-                "ستن",
-                "م",
-                "ی",
-                "ه",
-                "د",
-                "ن",
-            ]
-
-            for endverb in end_verb_list:
-                if word.endswith(endverb):
-                    if endverb == "ین":
-                        collection_of_verb_list.append(
-                            {"word": word[:-2], "suffix": "ید"},
-                        )
-                    elif endverb == "ستن":
-                        collection_of_verb_list.append(
-                            {"word": word[:-3], "suffix": "ستند"},
-                        )
-                    elif endverb == "ن":
-                        collection_of_verb_list.append(
-                            {"word": word[:-1], "suffix": "ن"},
-                        )
-                        collection_of_verb_list.append(
-                            {"word": word[:-1], "suffix": "ند"},
-                        )
-                    elif endverb == "ه":
-                        if len(word) > 1:
-                            if word[-2] != "د":
-                                collection_of_verb_list.append(
-                                    {"word": word[:-1], "suffix": "د"},
-                                )
-                            collection_of_verb_list.append(
-                                {"word": word[:-1], "suffix": "ه"},
-                            )
-                        else:
-                            collection_of_verb_list.append(
-                                {"word": word[:-1], "suffix": "ه"},
-                            )
-                    else:
-                        collection_of_verb_list.append(
-                            {
-                                "word": word[: -1 * len(endverb)],
-                                "suffix": endverb,
-                            },
-                        )
-            collection_of_verb_list.append({"word": word, "suffix": ""})
-            collection_of_verb_list_2 = []
-            for i in range(len(collection_of_verb_list)):
-                mainword = collection_of_verb_list[i]["word"]
-                collection_of_verb_list[i]["preffix"] = ""
-                if mainword.startswith("بر"):
-                    modified_word = mainword[2:]
-                    new_main_word = ""
-                    if modified_word.startswith("نمی"):
-                        collection_of_verb_list[i]["preffix"] = "برنمی"
-                        new_main_word = modified_word[3:]
-                    elif modified_word.startswith("می"):
-                        collection_of_verb_list[i]["preffix"] = "برمی"
-                        new_main_word = modified_word[2:]
-                    elif modified_word.startswith("ن"):
-                        collection_of_verb_list[i]["preffix"] = "برن"
-                        new_main_word = modified_word[1:]
-                    elif modified_word.startswith("بی"):
-                        collection_of_verb_list[i]["preffix"] = "بربی"
-                        new_main_word = modified_word[2:]
-                    elif modified_word.startswith("ب"):
-                        collection_of_verb_list[i]["preffix"] = "برب"
-                        new_main_word = modified_word[1:]
-                    else:
-                        collection_of_verb_list[i]["preffix"] = "بر"
-                        new_main_word = modified_word
-                        collection_of_verb_list_2.append(
-                            {
-                                "word": mainword,
-                                "preffix": "",
-                                "suffix": collection_of_verb_list[i]["suffix"],
-                            },
-                        )
-
-                    if new_main_word:
-                        collection_of_verb_list[i]["word"] = new_main_word
-                elif mainword.startswith("نمی"):
-                    collection_of_verb_list[i]["preffix"] = "نمی"
-                    collection_of_verb_list[i]["word"] = mainword[3:]
-                elif mainword.startswith("می"):
-                    collection_of_verb_list[i]["preffix"] = "می"
-                    collection_of_verb_list[i]["word"] = mainword[2:]
-                elif mainword.startswith("ن"):
-                    collection_of_verb_list[i]["preffix"] = "ن"
-                    collection_of_verb_list[i]["word"] = mainword[1:]
-                    collection_of_verb_list_2.append(
-                        {
-                            "word": mainword,
-                            "preffix": "",
-                            "suffix": collection_of_verb_list[i]["suffix"],
-                        },
-                    )
-
-                elif mainword.startswith("بی"):
-                    collection_of_verb_list[i]["preffix"] = "بی"
-                    collection_of_verb_list[i]["word"] = mainword[2:]
-                elif mainword.startswith("ب"):
-                    collection_of_verb_list[i]["preffix"] = "ب"
-                    collection_of_verb_list[i]["word"] = mainword[1:]
-                    collection_of_verb_list_2.append(
-                        {
-                            "word": mainword,
-                            "preffix": "",
-                            "suffix": collection_of_verb_list[i]["suffix"],
-                        },
-                    )
-
-            for i in range(len(collection_of_verb_list_2)):
-                collection_of_verb_list.append(collection_of_verb_list_2[i])
-
-            collection_of_real_verb_list = []
-            for i in range(len(collection_of_verb_list)):
-                mainword = collection_of_verb_list[i]["word"]
-                if mainword.startswith(("\u200c", "\u200e")):
-                    mainword = mainword[1:]
-
-                mainword2 = None
-                if mainword.startswith("ا"):
-                    mainword2 = "آ" + mainword[1:]
-                if mainword in self.pastVerbs:
-                    collection_of_verb_list[i]["word"] = self.pastVerbs[mainword]
-                    collection_of_real_verb_list.append(collection_of_verb_list[i])
-                if mainword in self.presentVerbs:
-                    collection_of_verb_list[i]["word"] = self.presentVerbs[mainword]
-                    collection_of_real_verb_list.append(collection_of_verb_list[i])
-                if mainword2 is not None and not (
-                    collection_of_verb_list[i]["preffix"] == "بربی"
-                    or collection_of_verb_list[i]["preffix"] == "بی"
-                ):
-                    if mainword2 in self.pastVerbs:
-                        collection_of_verb_list[i]["word"] = self.pastVerbs[mainword2]
-                        collection_of_real_verb_list.append(collection_of_verb_list[i])
-                    if mainword2 in self.presentVerbs:
-                        collection_of_verb_list[i]["word"] = self.presentVerbs[
-                            mainword2
-                        ]
-                        collection_of_real_verb_list.append(collection_of_verb_list[i])
-
-            for i in range(len(collection_of_real_verb_list)):
-                preffix = collection_of_real_verb_list[i]["preffix"]
-                suffix = collection_of_real_verb_list[i]["suffix"]
-                mainword = collection_of_real_verb_list[i]["word"]
-                returnword = preffix
-                if preffix.endswith("می"):
-                    returnword += "‌"
-                returnword += mainword
-                returnword += suffix
-                if mainword and returnword not in return_list:
-                    return_list.append(returnword)
-
-            return return_list
-
-        def append_suffix_to_word(one_collection_of_word_and_suffix):
-            mainword = one_collection_of_word_and_suffix["word"]
-            suffix_list = one_collection_of_word_and_suffix["suffix"]
-            adhesive_alphabet = {
-                "ب": "ب",
-                "پ": "پ",
-                "ت": "ت",
-                "ث": "ث",
-                "ج": "ج",
-                "چ": "چ",
-                "ح": "ح",
-                "خ": "خ",
-                "س": "س",
-                "ش": "ش",
-                "ص": "ص",
-                "ض": "ض",
-                "ع": "ع",
-                "غ": "غ",
-                "ف": "ف",
-                "ق": "ق",
-                "ک": "ک",
-                "گ": "گ",
-                "ل": "ل",
-                "م": "م",
-                "ن": "ن",
-                "ه": "ه",
-                "ی": "ی",
-            }
-            return_list = []
-            returnword = mainword
-            return_word2 = None
-            return_word3 = None
-            if len(suffix_list) == 0:
-                return [returnword]
-            if len(suffix_list) > 1:
-                if suffix_list[0] == "ه" and suffix_list[1] == "ا":
-                    suffix_list[0] = "ها"
-                    suffix_list.remove(suffix_list[1])
-                if suffix_list[0] == "ه" and suffix_list[1] == "است":
-                    suffix_list[0] = "هاست"
-                    suffix_list.remove(suffix_list[1])
-                if suffix_list[0] == "ت" and suffix_list[1] == "ا":
-                    suffix_list[0] = "تا"
-                    suffix_list.remove(suffix_list[1])
-            for i in range(len(suffix_list)):
-                if suffix_list[i] == "شون":
-                    returnword += "شان"
-                elif suffix_list[i] == "تون":
-                    returnword += "تان"
-                elif suffix_list[i] == "مون":
-                    returnword += "مان"
-                elif suffix_list[i] == "هام":
-                    try:
-                        adhesive_alphabet[returnword[-1]]
-                        returnword += "‌"
-                    except:
-                        None  # noqa: B018
-                    returnword += "هایم"
-                elif suffix_list[i] == "ها":  # noqa: SIM114
-                    try:
-                        adhesive_alphabet[returnword[-1]]
-                        returnword += "‌"
-                    except:
-                        None  # noqa: B018
-                    returnword += "ها"
-                elif (
-                    suffix_list[i] == "ا"
-                    and suffix_list[len(suffix_list) - 1] == "ا"
-                    and not returnword.endswith("ه")
-                ):
-                    try:
-                        adhesive_alphabet[returnword[-1]]
-                        returnword += "‌"
-                    except:
-                        None  # noqa: B018
-                    returnword += "ها"
-                elif suffix_list[i] == "و" and suffix_list[len(suffix_list) - 1] == "و":
-                    return_word2 = returnword
-                    return_word2 += " و"
-                    returnword += " را"
-
-                elif (
-                    suffix_list[i] == "رو" and suffix_list[len(suffix_list) - 1] == "رو"
-                ):
-                    returnword += " را"
-
-                elif suffix_list[i] == "ه" and suffix_list[len(suffix_list) - 1] == "ه":
-                    return_word2 = returnword
-                    return_word2 += "ه"
-                    return_word3 = returnword
-                    return_word3 += " است"
-                    returnword += "ه است"
-                else:
-                    returnword += suffix_list[i]
-            return_list.append(returnword)
-            if return_word2 is not None:
-                return_list.append(return_word2)
-            if return_word3 is not None:
-                return_list.append(return_word3)
-            return return_list
-
-        def straight_forward_result(word):
-            straight_forward_dic = {
-                "ب": ["به"],
-                "ک": ["که"],
-                "آن": ["آن"],
-                "می‌آید": ["می‌آید"],
-                "میاید": ["می‌آید"],
-                "می‌آیم": ["می‌آیم"],
-                "میایم": ["می‌آیم"],
-                "نمی‌آید": ["نمی‌آید"],
-                "نمیاید": ["نمی‌آید"],
-                "نمی‌آیم": ["نمی‌آیم"],
-                "نمیایم": ["نمی‌آیم"],
-                "برمی‌آید": ["برمی‌آید"],
-                "برمیاید": ["برمی‌آید"],
-                "برمی‌آیم": ["برمی‌آیم"],
-                "برمیایم": ["برمی‌آیم"],
-                "برنمی‌آید": ["برنمی‌آید"],
-                "برنمیاید": ["برنمی‌آید"],
-                "برنمی‌آیم": ["برنمی‌آیم"],
-                "برنمیایم": ["برنمی‌آیم"],
-                "منظوره": ["منظوره"],
-                "بدن": ["بدن"],
-                "میا": ["میا"],
-                "نیس": ["نیست"],
-                "فک": ["فکر"],
-                "برام": ["برایم"],
-                "آ": ["آ"],
-                "آی": ["آی"],
-                "این": ["این"],
-                "است": ["است"],
-                "ان": ["ان"],
-                "اند": ["اند"],
-                "میان": ["میان"],
-                "گردن": ["گردن"],
-                "اینهمه": ["اینهمه"],
-                "آنهمه": ["آنهمه"],
-                "الیه": ["الیه"],
-                "غرغره": ["غرغره"],
-                "لیله": ["لیله"],
-                "بزرگانه": ["بزرگانه"],
-                "پرستانه": ["پرستانه"],
-                "ام": ["ام"],
-                "بادی": ["بادی"],
-                "نان": ["نان"],
-                "باورم": ["باورم"],
-                "اوه": ["اوه"],
-                "چقد": ["چقدر"],
-                "چو": ["چون"],
-                "هس": ["هست"],
-                "اومدند": ["آمدند"],
-                "ش": ["اش"],
-                "بش": ["بهش"],
-                "ازت": ["از تو"],
-                "رو": ["را", "رو"],
-                "پایتون": ["پایتون"],
-                "اردن": ["اردن"],
-                "دست": ["دست"],
-                "دستی": ["دستی"],
-                "دستم": ["دستم"],
-                "دین": ["دین"],
-                "شین": ["شین"],
-                "سراتو": ["سراتو"],
-                "فالو": ["فالو"],
-                "هرجا": ["هرجا"],
-                "میدان": ["میدان"],
-                "میدون": ["میدان"],
-                "کفا": ["کفا"],
-                "ویا": ["و یا"],
-                "نشد": ["نشد"],
-                "شو": ["شو"],
-                "مشیا": ["مشیا"],
-                "پلاسما": ["پلاسما"],
-                "فیلیمو": ["فیلیمو"],
-                "پاشو": ["پاشو"],
-                "میر": ["میر"],
-                "بارم": ["بار هم", "بارم"],
-                "برند": ["برند"],
-                "کنه": ["کند"],
-                "بتونه": ["بتواند"],
-                "باشه": ["باشد"],
-                "بخوان": ["بخوان"],
-                "بدم": ["بدم"],
-                "برم": ["برم"],
-                "بده": ["بده"],
-                "نده": ["نده"],
-                "شهرو": ["شهرو"],
-                "شیرو": ["شیرو"],
-                "نگذاشته": ["نگذاشته"],
-                "نگرفته": ["نگرفته"],
-                "نمیشناخته": ["نمی‌شناخته"],
-                "نمی‌شناخته": ["نمی‌شناخته"],
-                "بشین": ["بشین"],
-                "هارو": ["ها را"],
-                "مارو": ["ما را"],
-                "میاومد": ["می‌آمد"],
-                "می‌اومد": ["می‌آمد"],
-                "میخواسته": ["می‌خواسته"],
-                "می‌خواسته": ["می‌خواسته"],
-                "نمیخواسته": ["نمی‌خواسته"],
-                "نمی‌خواسته": ["نمی‌خواسته"],
-                "میتوانسته": ["می‌توانسته"],
-                "می‌توانسته": ["می‌توانسته"],
-                "میرفته": ["می‌رفته"],
-                "می‌رفته": ["می‌رفته"],
-                "نشین": ["نشین"],
-                "انا": ["انا"],
-                "خونی": ["خونی"],
-                "خون": ["خون"],
-                "یالا": ["یالا"],
-                "میخواند": ["می‌خواند"],
-                "می‌خواند": ["می‌خواند"],
-                "نمیخواند": ["نمی‌خواند"],
-                "نمی‌خواند": ["نمی‌خواند"],
-                "میده": ["می‌دهد"],
-                "می‌ده": ["می‌دهد"],
-                "میشه": ["می‌شود"],
-                "می‌شه": ["می‌شود"],
-                "میشد": ["می‌شد"],
-                "می‌شد": ["می‌شد"],
-                "میشدم": ["می‌شدم"],
-                "می‌شدم": ["می‌شدم"],
-                "نمیشد": ["نمی‌شد"],
-                "نمی‌شد": ["نمی‌شد"],
-                "بردم": ["بردم"],
-                "بره": ["بره", "برود"],
-                "شم": ["بشوم"],
-                "اوست": ["اوست"],
-                "بیا": ["بیا"],
-                "نیا": ["نیا"],
-                "میاد": ["می‌آید"],
-                "نشدی": ["نشدی"],
-                "بخواند": ["بخواند"],
-                "سیا": ["سیا"],
-                "میدید": ["می‌دید"],
-                "می‌دید": ["می‌دید"],
-                "وا": ["وا"],
-                "برگشته": ["برگشته"],
-                "میخواست": ["می‌خواست"],
-                "می‌خواست": ["می‌خواست"],
-            }
-            try:
-                return straight_forward_dic[word]
-            except:
-                return []
-
-        straight_forward_words = straight_forward_result(word)
-        if len(straight_forward_words) > 0:
-            return straight_forward_words
-
-        verb_words_list = analyze_verb_word(word)
-        if len(verb_words_list) > 0:
-            return verb_words_list
-        possible_words = analyze_word(word)
-
-        mainword = word
-        if mainword in possible_words:
-            possible_words.remove(mainword)
-            possible_words.append(mainword)
-        elif len(possible_words) == 0:
-            possible_words.append(mainword)
-
-        return possible_words
-
-    def normalize(self: "InformalNormalizer", text: str) -> List[List[List[str]]]:
-        """متن محاوره‌ای را به متن فارسی معیار تبدیل می‌کند.
-
-        Examples:
-            >>> normalizer = InformalNormalizer()
-            >>> normalizer.normalize('بابا یه شغل مناسب واسه بچه هام پیدا کردن که به جایی برنمیخوره !')
-            [[['بابا'], ['یک'], ['شغل'], ['مناسب'], ['برای'], ['بچه'], ['هایم'], ['پیدا'], ['کردن', 'کردند'], ['که'], ['به'], ['جایی'], ['برنمی\u200cخورد', 'برنمی\u200cخوره'], ['!']]]
-            >>> normalizer = InformalNormalizer()
-            >>> normalizer.normalize('اجازه بدیم همسرمون در جمع خانواده‌اش احساس آزادی کنه و فکر نکنه که ما دائم هواسمون بهش هست .')
-            [[['اجازه'], ['بدهیم'], ['همسرمان'], ['در'], ['جمع'], ['خانواده\u200cاش'], ['احساس'], ['آزادی'], ['کند'], ['و'], ['فکر'], ['نکند', 'نکنه'], ['که'], ['ما'], ['دائم'], ['حواسمان'], ['بهش'], ['هست'], ['.']]]
-
-        Args:
-            text: متن محاوره‌ای که باید تبدیل به متن فارسی معیار شود.
-
-        Returns:
-           متن فارسی معیار.
-
-        """
-        text = super().normalize(text)
-        sents = [
-            self.word_tokenizer.tokenize(sentence)
-            for sentence in self.sent_tokenizer.tokenize(text)
-        ]
-
-        return [[self.normalized_word(word) for word in sent] for sent in sents]
-
-    def informal_conjugations(self: "InformalNormalizer", verb: str) -> List[str]:
-        """صورت‌های صرفی فعل را در شکل محاوره‌ای تولید می‌کند.
-
-        Args:
-            verb: فعلی که باید صرف شود.
-
-        Returns:
-            صورت‌های صرفی فعل.
-
-        """
-        ends = ["م", "ی", "", "یم", "ین", "ن"]
-        present_simples = [verb + end for end in ends]
-        if verb.endswith("ا"):
-            present_simples[2] = verb + "د"
-        else:
-            present_simples[2] = verb + "ه"
-        present_not_simples = ["ن" + item for item in present_simples]
-        present_imperfects = ["می‌" + item for item in present_simples]
-        present_not_imperfects = ["ن" + item for item in present_imperfects]
-        present_subjunctives = [
-            item if item.startswith("ب") else "ب" + item for item in present_simples
-        ]
-        present_not_subjunctives = ["ن" + item for item in present_simples]
-        return (
-            present_simples
-            + present_not_simples
-            + present_imperfects
-            + present_not_imperfects
-            + present_subjunctives
-            + present_not_subjunctives
-        )
-
-
-class InformalLemmatizer(Lemmatizer):
-    """این کلاس شامل توابعی برای نرمال‌سازی متن‌های محاوره‌ای است."""
-
-    def __init__(self: "InformalNormalizer", **kargs: str) -> None:
-        """__init__."""
-        super().__init__(**kargs)
-
-        temp = []
-        self.words = set(self.words.keys())
-        for word in self.words:
-            if word.endswith("ً"):
-                temp.append(word[:-1])
-
-        self.words.update(temp)
-
-        temp = {}
-        for verb in self.verbs:
-            if verb.endswith("د"):
-                temp[verb[:-1] + "ن"] = self.verbs[verb]
-
-        self.verbs.update(temp)
-
-        with Path.open(informal_verbs, encoding="utf8") as vf:
-            for f, i, _flag in [x.strip().split(" ", 2) for x in vf]:
-                self.verbs.update({x: f for x in self.iconjugations(i)})
-
-        with Path.open(informal_words, encoding="utf8") as wf:
-            self.words.update([x.strip().split(" ", 1)[0] for x in wf])
-
-    def iconjugations(self: "InformalNormalizer", verb: str):
-        """iconjugations."""
-        ends = ["م", "ی", "", "یم", "ین", "ن"]
-        present_simples = [verb + end for end in ends]
-        if verb.endswith("ا"):
-            present_simples[2] = verb + "د"
-        else:
-            present_simples[2] = verb + "ه"
-        present_not_simples = ["ن" + item for item in present_simples]
-        present_imperfects = ["می‌" + item for item in present_simples]
-        present_not_imperfects = ["ن" + item for item in present_imperfects]
-        present_subjunctives = [
-            item if item.startswith("ب") else "ب" + item for item in present_simples
-        ]
-        present_not_subjunctives = ["ن" + item for item in present_simples]
-        return (
-            present_simples
-            + present_not_simples
-            + present_imperfects
-            + present_not_imperfects
-            + present_subjunctives
-            + present_not_subjunctives
-        )
+"""این ماژول شامل کلاس‌ها و توابعی برای نرمال‌سازی متن‌های محاوره‌ای است."""
+
+
+import re
+from pathlib import Path
+from typing import List
+
+from hazm import NUMBERS
+from hazm import Lemmatizer
+from hazm import Normalizer
+from hazm import SentenceTokenizer
+from hazm import Stemmer
+from hazm import WordTokenizer
+from hazm import default_verbs
+from hazm import informal_verbs
+from hazm import informal_words
+
+
+class InformalNormalizer(Normalizer):
+    """این کلاس شامل توابعی برای نرمال‌سازی متن‌های محاوره‌ای است.
+
+    Args:
+        verb_file: فایل حاوی افعال محاوره‌ای.
+        word_file: فایل حاوی کلمات محاوره‌ای.
+        seperation_flag: اگر `True` باشد و در بخشی از متن به فاصله نیاز بود آن فاصله درج می‌شود.
+        **kargs: پارامترهای نامدارِ اختیاری
+
+    """
+
+    def __init__(
+        self: "InformalNormalizer",
+        verb_file: str = informal_verbs,
+        word_file: str = informal_words,
+        seperation_flag: bool = False,
+        **kargs: str,
+    ) -> None:
+        self.seperation_flag = seperation_flag
+        self.lemmatizer = Lemmatizer()
+        self.ilemmatizer = InformalLemmatizer()
+        self.stemmer = Stemmer()
+        super().__init__(**kargs)
+
+        self.sent_tokenizer = SentenceTokenizer()
+        self.word_tokenizer = WordTokenizer()
+
+        with Path.open(verb_file, encoding="utf8") as vf:
+            self.pastVerbs = {}
+            self.presentVerbs = {}
+            for f, i, _flag in [x.strip().split(" ", 2) for x in vf]:
+                splitedf = f.split("#")
+                self.presentVerbs.update({i: splitedf[1]})
+                self.pastVerbs.update({splitedf[0]: splitedf[0]})
+        with Path.open(default_verbs, encoding="utf8") as vf:
+            for f, i in [x.strip().split("#", 2) for x in vf]:
+                self.presentVerbs.update({i: i})
+                self.pastVerbs.update({f: f})
+
+        def informal_to_formal_conjucation(i, f, flag):
+            iv = self.informal_conjugations(i)
+            fv = self.lemmatizer.conjugation.get_all(f)
+            res = {}
+            if flag:
+                for i, j in zip(iv, fv[48:]):
+                    res[i] = j
+                    if "‌" in i:
+                        res[i.replace("‌", "")] = j
+                        res[i.replace("‌", " ")] = j
+                    if i.endswith("ین"):
+                        res[i[:-1] + "د"] = j
+            else:
+                for i, j in zip(iv[8:], fv[56:]):
+                    res[i] = j
+                    if "‌" in i:
+                        res[i.replace("‌", "")] = j
+                        res[i.replace("‌", " ")] = j
+                    if i.endswith("ین"):
+                        res[i[:-1] + "د"] = j
+
+            return res
+
+        with Path.open(verb_file, encoding="utf8") as vf:
+            self.iverb_map = {}
+            for f, i, flag in [x.strip().split(" ", 2) for x in vf]:
+                self.iverb_map.update(informal_to_formal_conjucation(i, f, flag))
+
+        with Path.open(word_file, encoding="utf8") as wf:
+            self.iword_map = dict([x.strip().split(" ", 1) for x in wf])
+
+        self.words = set()
+        if self.seperation_flag:
+            self.words.update(list(self.iword_map.keys()))
+            self.words.update(list(self.iword_map.values()))
+            self.words.update(list(self.iverb_map.keys()))
+            self.words.update(list(self.iverb_map.values()))
+            self.words.update(self.lemmatizer.words)
+            self.words.update(list(self.lemmatizer.verbs.keys()))
+            self.words.update(list(self.lemmatizer.verbs.values()))
+
+    def split_token_words(self: "InformalNormalizer", token: str) -> str:
+        """هرجایی در متن فاصله نیاز بود قرار می‌دهد.
+
+        متأسفانه در برخی از متن‌ها، به بهانهٔ صرفه‌جویی در زمان یا از سرِ تنبلی،
+        فاصله‌گذاری‌ها درست رعایت نمی‌شود. مثلاً جملهٔ «تو را دوست دارم.» به این
+        شکل نوشته می‌شود: «تورادوست دارم.» این تابع فواصل ضروری را در متن
+        ایجاد می‌کند و آن را به شکل صحیح برمی‌گرداند.
+
+        Args:
+            token: توکنی که باید فاصله‌گذاری شود.
+
+        Returns:
+            توکنی با فاصله‌گذاری صحیح.
+
+        """
+
+        def shekan(token):
+            res = [""]
+            for i in token:
+                res[-1] += i
+                if i in {"ا", "د", "ذ", "ر", "ز", "ژ", "و", *list(NUMBERS)}:
+                    res.append("")
+            while "" in res:
+                res.remove("")
+            return res
+
+        def perm(lst):
+            if len(lst) > 1:
+                up = perm(lst[1:])
+            else:
+                return [lst]
+            res = []
+            for i in up:
+                res.append([lst[0], *i])
+                res.append([lst[0] + i[0]] + i[1:])
+            res.sort(key=len)
+            return res
+
+        token = re.sub(r"(.)\1{2,}", r"\1", token)
+        ps = perm(shekan(token))
+        for c in ps:
+            if {self.ilemmatizer.lemmatize(x) for x in c}.issubset(self.words):
+                return " ".join(c)
+        return token
+
+    def normalized_word(self: "InformalNormalizer", word: str) -> List[str]:
+        """اشکال مختلف نرمالایزشدهٔ کلمه را برمی‌گرداند.
+
+        Examples:
+            >>> normalizer = InformalNormalizer()
+            >>> normalizer.normalized_word('می‌رم')
+            ['می‌روم', 'می‌رم']
+
+        Args:
+            word: کلمه‌ای که باید نرمال‌سازی شود.
+
+        Returns:
+            اشکال نرمالایزشدهٔ کلمه.
+
+        """
+        # >>> normalizer = InformalNormalizer(seperation_flag=True)
+        # >>> normalizer.normalized_word('صداوسیماجمهوری')
+
+        def analyze_word(word):
+            end_words_list = [
+                "هاست",
+                "هایی",
+                "هایم",
+                "ترین",
+                "ایی",
+                "انی",
+                "شان",
+                "شون",
+                "است",
+                "تان",
+                "تون",
+                "مان",
+                "مون",
+                "هام",
+                "هاش",
+                "های",
+                "طور",
+                "ها",
+                "تر",
+                "ئی",
+                "یی",
+                "یم",
+                "ام",
+                "ای",
+                "ان",
+                "هم",
+                "رو",
+                "یت",
+                "ه",
+                "ی",
+                "ش",
+                "و",
+                "ا",
+                "ت",
+                "م",
+            ]
+
+            return_list = []
+
+            collection_of_word_and_suffix = []
+
+            found_early = False
+
+            mid_word_condidate = []
+
+            if word.endswith(("\u200c", "\u200e")):
+                word = word[:-1]
+
+            if word in self.lemmatizer.words or word in self.iword_map:
+                if word in self.lemmatizer.words:
+                    collection_of_word_and_suffix.append({"word": word, "suffix": []})
+                if word in self.iword_map:
+                    collection_of_word_and_suffix.append(
+                        {"word": self.iword_map[word], "suffix": []},
+                    )
+                found_early = True
+
+            if not found_early:
+                for endword in end_words_list:
+                    if word.endswith(endword):
+                        sliceword = word[: -1 * len(endword)]
+                        if (
+                            sliceword in self.lemmatizer.words
+                            or sliceword in self.iword_map
+                        ):
+                            if sliceword in self.lemmatizer.words:
+                                collection_of_word_and_suffix.append(
+                                    {"word": sliceword, "suffix": [endword]},
+                                )
+                            if sliceword in self.iword_map:
+                                collection_of_word_and_suffix.append(
+                                    {
+                                        "word": self.iword_map[sliceword],
+                                        "suffix": [endword],
+                                    },
+                                )
+                        else:
+                            mid_word_condidate.append(sliceword)
+                            mid_word_condidate.append([endword])
+
+                for endword in end_words_list:
+                    for i in range(len(mid_word_condidate) - 1):
+                        if i % 2 == 1:
+                            continue
+                        midword = mid_word_condidate[i]
+                        mid_word_end_word_list = mid_word_condidate[i + 1]
+                        if midword.endswith(endword):
+                            sliceword = midword[: -1 * len(endword)]
+                            if (
+                                sliceword in self.lemmatizer.words
+                                or sliceword in self.iword_map
+                            ):
+                                if sliceword in self.lemmatizer.words:
+                                    collection_of_word_and_suffix.append(
+                                        {
+                                            "word": sliceword,
+                                            "suffix": [
+                                                endword,
+                                                *mid_word_end_word_list,
+                                            ],
+                                        },
+                                    )
+                                if sliceword in self.iword_map:
+                                    collection_of_word_and_suffix.append(
+                                        {
+                                            "word": self.iword_map[sliceword],
+                                            "suffix": [
+                                                endword,
+                                                *mid_word_end_word_list,
+                                            ],
+                                        },
+                                    )
+
+            for i in range(len(collection_of_word_and_suffix)):
+                new_possible_word_list = append_suffix_to_word(
+                    collection_of_word_and_suffix[i],
+                )
+                for j in range(len(new_possible_word_list)):
+                    new_possible_word = new_possible_word_list[j]
+                    if new_possible_word not in return_list:
+                        return_list.append(new_possible_word)
+
+            return return_list
+
+        def analyze_verb_word(word):
+            if word in self.pastVerbs:
+                word = self.pastVerbs[word]
+                return [word]
+
+            if word in self.iword_map:
+                return []
+
+            if word in self.lemmatizer.words:
+                if word[-1] == "ن":
+                    None  # noqa: B018
+                else:
+                    return []
+
+            return_list = []
+
+            collection_of_verb_list = []
+
+            end_verb_list = [
+                "یم",
+                "دم",
+                "دیم",
+                "ید",
+                "دی",
+                "دید",
+                "ند",
+                "دن",
+                "دند",
+                "ین",
+                "دین",
+                "ست",
+                "ستم",
+                "ستی",
+                "ستیم",
+                "ستید",
+                "ستند",
+                "ستن",
+                "م",
+                "ی",
+                "ه",
+                "د",
+                "ن",
+            ]
+
+            for endverb in end_verb_list:
+                if word.endswith(endverb):
+                    if endverb == "ین":
+                        collection_of_verb_list.append(
+                            {"word": word[:-2], "suffix": "ید"},
+                        )
+                    elif endverb == "ستن":
+                        collection_of_verb_list.append(
+                            {"word": word[:-3], "suffix": "ستند"},
+                        )
+                    elif endverb == "ن":
+                        collection_of_verb_list.append(
+                            {"word": word[:-1], "suffix": "ن"},
+                        )
+                        collection_of_verb_list.append(
+                            {"word": word[:-1], "suffix": "ند"},
+                        )
+                    elif endverb == "ه":
+                        if len(word) > 1:
+                            if word[-2] != "د":
+                                collection_of_verb_list.append(
+                                    {"word": word[:-1], "suffix": "د"},
+                                )
+                            collection_of_verb_list.append(
+                                {"word": word[:-1], "suffix": "ه"},
+                            )
+                        else:
+                            collection_of_verb_list.append(
+                                {"word": word[:-1], "suffix": "ه"},
+                            )
+                    else:
+                        collection_of_verb_list.append(
+                            {
+                                "word": word[: -1 * len(endverb)],
+                                "suffix": endverb,
+                            },
+                        )
+            collection_of_verb_list.append({"word": word, "suffix": ""})
+            collection_of_verb_list_2 = []
+            for i in range(len(collection_of_verb_list)):
+                mainword = collection_of_verb_list[i]["word"]
+                collection_of_verb_list[i]["preffix"] = ""
+                if mainword.startswith("بر"):
+                    modified_word = mainword[2:]
+                    new_main_word = ""
+                    if modified_word.startswith("نمی"):
+                        collection_of_verb_list[i]["preffix"] = "برنمی"
+                        new_main_word = modified_word[3:]
+                    elif modified_word.startswith("می"):
+                        collection_of_verb_list[i]["preffix"] = "برمی"
+                        new_main_word = modified_word[2:]
+                    elif modified_word.startswith("ن"):
+                        collection_of_verb_list[i]["preffix"] = "برن"
+                        new_main_word = modified_word[1:]
+                    elif modified_word.startswith("بی"):
+                        collection_of_verb_list[i]["preffix"] = "بربی"
+                        new_main_word = modified_word[2:]
+                    elif modified_word.startswith("ب"):
+                        collection_of_verb_list[i]["preffix"] = "برب"
+                        new_main_word = modified_word[1:]
+                    else:
+                        collection_of_verb_list[i]["preffix"] = "بر"
+                        new_main_word = modified_word
+                        collection_of_verb_list_2.append(
+                            {
+                                "word": mainword,
+                                "preffix": "",
+                                "suffix": collection_of_verb_list[i]["suffix"],
+                            },
+                        )
+
+                    if new_main_word:
+                        collection_of_verb_list[i]["word"] = new_main_word
+                elif mainword.startswith("نمی"):
+                    collection_of_verb_list[i]["preffix"] = "نمی"
+                    collection_of_verb_list[i]["word"] = mainword[3:]
+                elif mainword.startswith("می"):
+                    collection_of_verb_list[i]["preffix"] = "می"
+                    collection_of_verb_list[i]["word"] = mainword[2:]
+                elif mainword.startswith("ن"):
+                    collection_of_verb_list[i]["preffix"] = "ن"
+                    collection_of_verb_list[i]["word"] = mainword[1:]
+                    collection_of_verb_list_2.append(
+                        {
+                            "word": mainword,
+                            "preffix": "",
+                            "suffix": collection_of_verb_list[i]["suffix"],
+                        },
+                    )
+
+                elif mainword.startswith("بی"):
+                    collection_of_verb_list[i]["preffix"] = "بی"
+                    collection_of_verb_list[i]["word"] = mainword[2:]
+                elif mainword.startswith("ب"):
+                    collection_of_verb_list[i]["preffix"] = "ب"
+                    collection_of_verb_list[i]["word"] = mainword[1:]
+                    collection_of_verb_list_2.append(
+                        {
+                            "word": mainword,
+                            "preffix": "",
+                            "suffix": collection_of_verb_list[i]["suffix"],
+                        },
+                    )
+
+            for i in range(len(collection_of_verb_list_2)):
+                collection_of_verb_list.append(collection_of_verb_list_2[i])
+
+            collection_of_real_verb_list = []
+            for i in range(len(collection_of_verb_list)):
+                mainword = collection_of_verb_list[i]["word"]
+                if mainword.startswith(("\u200c", "\u200e")):
+                    mainword = mainword[1:]
+
+                mainword2 = None
+                if mainword.startswith("ا"):
+                    mainword2 = "آ" + mainword[1:]
+                if mainword in self.pastVerbs:
+                    collection_of_verb_list[i]["word"] = self.pastVerbs[mainword]
+                    collection_of_real_verb_list.append(collection_of_verb_list[i])
+                if mainword in self.presentVerbs:
+                    collection_of_verb_list[i]["word"] = self.presentVerbs[mainword]
+                    collection_of_real_verb_list.append(collection_of_verb_list[i])
+                if mainword2 is not None and not (
+                    collection_of_verb_list[i]["preffix"] == "بربی"
+                    or collection_of_verb_list[i]["preffix"] == "بی"
+                ):
+                    if mainword2 in self.pastVerbs:
+                        collection_of_verb_list[i]["word"] = self.pastVerbs[mainword2]
+                        collection_of_real_verb_list.append(collection_of_verb_list[i])
+                    if mainword2 in self.presentVerbs:
+                        collection_of_verb_list[i]["word"] = self.presentVerbs[
+                            mainword2
+                        ]
+                        collection_of_real_verb_list.append(collection_of_verb_list[i])
+
+            for i in range(len(collection_of_real_verb_list)):
+                preffix = collection_of_real_verb_list[i]["preffix"]
+                suffix = collection_of_real_verb_list[i]["suffix"]
+                mainword = collection_of_real_verb_list[i]["word"]
+                returnword = preffix
+                if preffix.endswith("می"):
+                    returnword += "‌"
+                returnword += mainword
+                returnword += suffix
+                if mainword and returnword not in return_list:
+                    return_list.append(returnword)
+
+            return return_list
+
+        def append_suffix_to_word(one_collection_of_word_and_suffix):
+            mainword = one_collection_of_word_and_suffix["word"]
+            suffix_list = one_collection_of_word_and_suffix["suffix"]
+            adhesive_alphabet = {
+                "ب": "ب",
+                "پ": "پ",
+                "ت": "ت",
+                "ث": "ث",
+                "ج": "ج",
+                "چ": "چ",
+                "ح": "ح",
+                "خ": "خ",
+                "س": "س",
+                "ش": "ش",
+                "ص": "ص",
+                "ض": "ض",
+                "ع": "ع",
+                "غ": "غ",
+                "ف": "ف",
+                "ق": "ق",
+                "ک": "ک",
+                "گ": "گ",
+                "ل": "ل",
+                "م": "م",
+                "ن": "ن",
+                "ه": "ه",
+                "ی": "ی",
+            }
+            return_list = []
+            returnword = mainword
+            return_word2 = None
+            return_word3 = None
+            if len(suffix_list) == 0:
+                return [returnword]
+            if len(suffix_list) > 1:
+                if suffix_list[0] == "ه" and suffix_list[1] == "ا":
+                    suffix_list[0] = "ها"
+                    suffix_list.remove(suffix_list[1])
+                if suffix_list[0] == "ه" and suffix_list[1] == "است":
+                    suffix_list[0] = "هاست"
+                    suffix_list.remove(suffix_list[1])
+                if suffix_list[0] == "ت" and suffix_list[1] == "ا":
+                    suffix_list[0] = "تا"
+                    suffix_list.remove(suffix_list[1])
+            for i in range(len(suffix_list)):
+                if suffix_list[i] == "شون":
+                    returnword += "شان"
+                elif suffix_list[i] == "تون":
+                    returnword += "تان"
+                elif suffix_list[i] == "مون":
+                    returnword += "مان"
+                elif suffix_list[i] == "هام":
+                    try:
+                        adhesive_alphabet[returnword[-1]]
+                        returnword += "‌"
+                    except:
+                        None  # noqa: B018
+                    returnword += "هایم"
+                elif suffix_list[i] == "ها":  # noqa: SIM114
+                    try:
+                        adhesive_alphabet[returnword[-1]]
+                        returnword += "‌"
+                    except:
+                        None  # noqa: B018
+                    returnword += "ها"
+                elif (
+                    suffix_list[i] == "ا"
+                    and suffix_list[len(suffix_list) - 1] == "ا"
+                    and not returnword.endswith("ه")
+                ):
+                    try:
+                        adhesive_alphabet[returnword[-1]]
+                        returnword += "‌"
+                    except:
+                        None  # noqa: B018
+                    returnword += "ها"
+                elif suffix_list[i] == "و" and suffix_list[len(suffix_list) - 1] == "و":
+                    return_word2 = returnword
+                    return_word2 += " و"
+                    returnword += " را"
+
+                elif (
+                    suffix_list[i] == "رو" and suffix_list[len(suffix_list) - 1] == "رو"
+                ):
+                    returnword += " را"
+
+                elif suffix_list[i] == "ه" and suffix_list[len(suffix_list) - 1] == "ه":
+                    return_word2 = returnword
+                    return_word2 += "ه"
+                    return_word3 = returnword
+                    return_word3 += " است"
+                    returnword += "ه است"
+                else:
+                    returnword += suffix_list[i]
+            return_list.append(returnword)
+            if return_word2 is not None:
+                return_list.append(return_word2)
+            if return_word3 is not None:
+                return_list.append(return_word3)
+            return return_list
+
+        def straight_forward_result(word):
+            straight_forward_dic = {
+                "ب": ["به"],
+                "ک": ["که"],
+                "آن": ["آن"],
+                "می‌آید": ["می‌آید"],
+                "میاید": ["می‌آید"],
+                "می‌آیم": ["می‌آیم"],
+                "میایم": ["می‌آیم"],
+                "نمی‌آید": ["نمی‌آید"],
+                "نمیاید": ["نمی‌آید"],
+                "نمی‌آیم": ["نمی‌آیم"],
+                "نمیایم": ["نمی‌آیم"],
+                "برمی‌آید": ["برمی‌آید"],
+                "برمیاید": ["برمی‌آید"],
+                "برمی‌آیم": ["برمی‌آیم"],
+                "برمیایم": ["برمی‌آیم"],
+                "برنمی‌آید": ["برنمی‌آید"],
+                "برنمیاید": ["برنمی‌آید"],
+                "برنمی‌آیم": ["برنمی‌آیم"],
+                "برنمیایم": ["برنمی‌آیم"],
+                "منظوره": ["منظوره"],
+                "بدن": ["بدن"],
+                "میا": ["میا"],
+                "نیس": ["نیست"],
+                "فک": ["فکر"],
+                "برام": ["برایم"],
+                "آ": ["آ"],
+                "آی": ["آی"],
+                "این": ["این"],
+                "است": ["است"],
+                "ان": ["ان"],
+                "اند": ["اند"],
+                "میان": ["میان"],
+                "گردن": ["گردن"],
+                "اینهمه": ["اینهمه"],
+                "آنهمه": ["آنهمه"],
+                "الیه": ["الیه"],
+                "غرغره": ["غرغره"],
+                "لیله": ["لیله"],
+                "بزرگانه": ["بزرگانه"],
+                "پرستانه": ["پرستانه"],
+                "ام": ["ام"],
+                "بادی": ["بادی"],
+                "نان": ["نان"],
+                "باورم": ["باورم"],
+                "اوه": ["اوه"],
+                "چقد": ["چقدر"],
+                "چو": ["چون"],
+                "هس": ["هست"],
+                "اومدند": ["آمدند"],
+                "ش": ["اش"],
+                "بش": ["بهش"],
+                "ازت": ["از تو"],
+                "رو": ["را", "رو"],
+                "پایتون": ["پایتون"],
+                "اردن": ["اردن"],
+                "دست": ["دست"],
+                "دستی": ["دستی"],
+                "دستم": ["دستم"],
+                "دین": ["دین"],
+                "شین": ["شین"],
+                "سراتو": ["سراتو"],
+                "فالو": ["فالو"],
+                "هرجا": ["هرجا"],
+                "میدان": ["میدان"],
+                "میدون": ["میدان"],
+                "کفا": ["کفا"],
+                "ویا": ["و یا"],
+                "نشد": ["نشد"],
+                "شو": ["شو"],
+                "مشیا": ["مشیا"],
+                "پلاسما": ["پلاسما"],
+                "فیلیمو": ["فیلیمو"],
+                "پاشو": ["پاشو"],
+                "میر": ["میر"],
+                "بارم": ["بار هم", "بارم"],
+                "برند": ["برند"],
+                "کنه": ["کند"],
+                "بتونه": ["بتواند"],
+                "باشه": ["باشد"],
+                "بخوان": ["بخوان"],
+                "بدم": ["بدم"],
+                "برم": ["برم"],
+                "بده": ["بده"],
+                "نده": ["نده"],
+                "شهرو": ["شهرو"],
+                "شیرو": ["شیرو"],
+                "نگذاشته": ["نگذاشته"],
+                "نگرفته": ["نگرفته"],
+                "نمیشناخته": ["نمی‌شناخته"],
+                "نمی‌شناخته": ["نمی‌شناخته"],
+                "بشین": ["بشین"],
+                "هارو": ["ها را"],
+                "مارو": ["ما را"],
+                "میاومد": ["می‌آمد"],
+                "می‌اومد": ["می‌آمد"],
+                "میخواسته": ["می‌خواسته"],
+                "می‌خواسته": ["می‌خواسته"],
+                "نمیخواسته": ["نمی‌خواسته"],
+                "نمی‌خواسته": ["نمی‌خواسته"],
+                "میتوانسته": ["می‌توانسته"],
+                "می‌توانسته": ["می‌توانسته"],
+                "میرفته": ["می‌رفته"],
+                "می‌رفته": ["می‌رفته"],
+                "نشین": ["نشین"],
+                "انا": ["انا"],
+                "خونی": ["خونی"],
+                "خون": ["خون"],
+                "یالا": ["یالا"],
+                "میخواند": ["می‌خواند"],
+                "می‌خواند": ["می‌خواند"],
+                "نمیخواند": ["نمی‌خواند"],
+                "نمی‌خواند": ["نمی‌خواند"],
+                "میده": ["می‌دهد"],
+                "می‌ده": ["می‌دهد"],
+                "میشه": ["می‌شود"],
+                "می‌شه": ["می‌شود"],
+                "میشد": ["می‌شد"],
+                "می‌شد": ["می‌شد"],
+                "میشدم": ["می‌شدم"],
+                "می‌شدم": ["می‌شدم"],
+                "نمیشد": ["نمی‌شد"],
+                "نمی‌شد": ["نمی‌شد"],
+                "بردم": ["بردم"],
+                "بره": ["بره", "برود"],
+                "شم": ["بشوم"],
+                "اوست": ["اوست"],
+                "بیا": ["بیا"],
+                "نیا": ["نیا"],
+                "میاد": ["می‌آید"],
+                "نشدی": ["نشدی"],
+                "بخواند": ["بخواند"],
+                "سیا": ["سیا"],
+                "میدید": ["می‌دید"],
+                "می‌دید": ["می‌دید"],
+                "وا": ["وا"],
+                "برگشته": ["برگشته"],
+                "میخواست": ["می‌خواست"],
+                "می‌خواست": ["می‌خواست"],
+            }
+            try:
+                return straight_forward_dic[word]
+            except:
+                return []
+
+        straight_forward_words = straight_forward_result(word)
+        if len(straight_forward_words) > 0:
+            return straight_forward_words
+
+        verb_words_list = analyze_verb_word(word)
+        if len(verb_words_list) > 0:
+            return verb_words_list
+        possible_words = analyze_word(word)
+
+        mainword = word
+        if mainword in possible_words:
+            possible_words.remove(mainword)
+            possible_words.append(mainword)
+        elif len(possible_words) == 0:
+            possible_words.append(mainword)
+
+        return possible_words
+
+    def normalize(self: "InformalNormalizer", text: str) -> List[List[List[str]]]:
+        """متن محاوره‌ای را به متن فارسی معیار تبدیل می‌کند.
+
+        Examples:
+            >>> normalizer = InformalNormalizer()
+            >>> normalizer.normalize('بابا یه شغل مناسب واسه بچه هام پیدا کردن که به جایی برنمیخوره !')
+            [[['بابا'], ['یک'], ['شغل'], ['مناسب'], ['برای'], ['بچه'], ['هایم'], ['پیدا'], ['کردن', 'کردند'], ['که'], ['به'], ['جایی'], ['برنمی\u200cخورد', 'برنمی\u200cخوره'], ['!']]]
+            >>> normalizer = InformalNormalizer()
+            >>> normalizer.normalize('اجازه بدیم همسرمون در جمع خانواده‌اش احساس آزادی کنه و فکر نکنه که ما دائم هواسمون بهش هست .')
+            [[['اجازه'], ['بدهیم'], ['همسرمان'], ['در'], ['جمع'], ['خانواده\u200cاش'], ['احساس'], ['آزادی'], ['کند'], ['و'], ['فکر'], ['نکند', 'نکنه'], ['که'], ['ما'], ['دائم'], ['حواسمان'], ['بهش'], ['هست'], ['.']]]
+
+        Args:
+            text: متن محاوره‌ای که باید تبدیل به متن فارسی معیار شود.
+
+        Returns:
+           متن فارسی معیار.
+
+        """
+        text = super().normalize(text)
+        sents = [
+            self.word_tokenizer.tokenize(sentence)
+            for sentence in self.sent_tokenizer.tokenize(text)
+        ]
+
+        return [[self.normalized_word(word) for word in sent] for sent in sents]
+
+    def informal_conjugations(self: "InformalNormalizer", verb: str) -> List[str]:
+        """صورت‌های صرفی فعل را در شکل محاوره‌ای تولید می‌کند.
+
+        Args:
+            verb: فعلی که باید صرف شود.
+
+        Returns:
+            صورت‌های صرفی فعل.
+
+        """
+        ends = ["م", "ی", "", "یم", "ین", "ن"]
+        present_simples = [verb + end for end in ends]
+        if verb.endswith("ا"):
+            present_simples[2] = verb + "د"
+        else:
+            present_simples[2] = verb + "ه"
+        present_not_simples = ["ن" + item for item in present_simples]
+        present_imperfects = ["می‌" + item for item in present_simples]
+        present_not_imperfects = ["ن" + item for item in present_imperfects]
+        present_subjunctives = [
+            item if item.startswith("ب") else "ب" + item for item in present_simples
+        ]
+        present_not_subjunctives = ["ن" + item for item in present_simples]
+        return (
+            present_simples
+            + present_not_simples
+            + present_imperfects
+            + present_not_imperfects
+            + present_subjunctives
+            + present_not_subjunctives
+        )
+
+
+class InformalLemmatizer(Lemmatizer):
+    """این کلاس شامل توابعی برای نرمال‌سازی متن‌های محاوره‌ای است."""
+
+    def __init__(self: "InformalNormalizer", **kargs: str) -> None:
+        """__init__."""
+        super().__init__(**kargs)
+
+        temp = []
+        self.words = set(self.words.keys())
+        for word in self.words:
+            if word.endswith("ً"):
+                temp.append(word[:-1])
+
+        self.words.update(temp)
+
+        temp = {}
+        for verb in self.verbs:
+            if verb.endswith("د"):
+                temp[verb[:-1] + "ن"] = self.verbs[verb]
+
+        self.verbs.update(temp)
+
+        with Path.open(informal_verbs, encoding="utf8") as vf:
+            for f, i, _flag in [x.strip().split(" ", 2) for x in vf]:
+                self.verbs.update({x: f for x in self.iconjugations(i)})
+
+        with Path.open(informal_words, encoding="utf8") as wf:
+            self.words.update([x.strip().split(" ", 1)[0] for x in wf])
+
+    def iconjugations(self: "InformalNormalizer", verb: str):
+        """iconjugations."""
+        ends = ["م", "ی", "", "یم", "ین", "ن"]
+        present_simples = [verb + end for end in ends]
+        if verb.endswith("ا"):
+            present_simples[2] = verb + "د"
+        else:
+            present_simples[2] = verb + "ه"
+        present_not_simples = ["ن" + item for item in present_simples]
+        present_imperfects = ["می‌" + item for item in present_simples]
+        present_not_imperfects = ["ن" + item for item in present_imperfects]
+        present_subjunctives = [
+            item if item.startswith("ب") else "ب" + item for item in present_simples
+        ]
+        present_not_subjunctives = ["ن" + item for item in present_simples]
+        return (
+            present_simples
+            + present_not_simples
+            + present_imperfects
+            + present_not_imperfects
+            + present_subjunctives
+            + present_not_subjunctives
+        )
```

### Comparing `hazm-0.9.1/hazm/lemmatizer.py` & `hazm-0.9.2/hazm/lemmatizer.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,2322 +1,2322 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای ریشه‌یابی کلمات است.
-
-فرق بین [Lemmatizer](./lemmatizer.md) و [Stemmer](./stemmer.md) این است که
-اِستمر درکی از معنای کلمه ندارد و صرفاً براساس حذف برخی از پسوندهای ساده تلاش
-می‌کند ریشهٔ کلمه را بیابد؛ بنابراین ممکن است در ریشه‌یابیِ برخی از کلمات نتایج
-نادرستی ارائه دهد؛ اما لماتایزر براساس لیستی از کلمات مرجع به همراه ریشهٔ آن
-این
-کار را انجام می‌دهد و نتایج دقیق‌تری ارائه می‌دهد. البته هزینهٔ این دقت، سرعتِ
-کمتر در ریشه‌یابی است.
-
-**میزان دقت
-لماتایزر در نسخهٔ حاضر ۸۹.۹ درصد [^1] است.**
-[^1]:
-این عدد با انتشار هر نسخه بروزرسانی می‌شود
-
-"""
-
-
-from typing import List
-
-from hazm import Stemmer
-from hazm import default_verbs
-from hazm import default_words
-from hazm import WordTokenizer
-
-
-class Lemmatizer:
-    """این کلاس شامل توابعی برای ریشه‌یابی کلمات است.
-
-    Args:
-        words_file: ریشه‌یابی کلمات از روی این فایل صورت
-            می‌گیرد. هضم به صورت پیش‌فرض فایلی برای این منظور در نظر گرفته است؛ با
-            این حال شما می‌توانید فایل موردنظر خود را معرفی کنید. برای آگاهی از
-            ساختار این فایل به فایل پیش‌فرض مراجعه کنید.
-        verbs_file: اشکال صرفی فعل از روی این فایل ساخته
-            می‌شود. هضم به صورت پیش‌فرض فایلی برای این منظور در نظر گرفته است؛ با
-            این حال شما می‌توانید فایل موردنظر خود را معرفی کنید. برای آگاهی از
-            ساختار این فایل به فایل پیش‌فرض مراجعه کنید.
-        joined_verb_parts: اگر `True` باشد افعال چندبخشی را با کاراکتر زیرخط به هم می‌چسباند.
-
-    """
-
-    def __init__(
-        self: "Lemmatizer",
-        words_file: str = default_words,
-        verbs_file: str = default_verbs,
-        joined_verb_parts: bool = True,
-    ) -> None:
-        self.words_file = words_file
-        self.verbs = {}
-        self.stemmer = Stemmer()
-        self.conjugation = Conjugation()
-
-        tokenizer = WordTokenizer(words_file=default_words, verbs_file=verbs_file)
-        self.words = tokenizer.words
-
-        if verbs_file:
-            self.verbs["است"] = "#است"
-            for verb in tokenizer.verbs:
-                for tense in self.conjugation.get_all(verb):
-                    self.verbs[tense] = verb
-            if joined_verb_parts:
-                for verb in tokenizer.verbs:
-                    bon = verb.split("#")[0]
-                    for after_verb in tokenizer.after_verbs:
-                        self.verbs[bon + "ه_" + after_verb] = verb
-                        self.verbs["ن" + bon + "ه_" + after_verb] = verb
-                    for before_verb in tokenizer.before_verbs:
-                        self.verbs[before_verb + "_" + bon] = verb
-
-    def lemmatize(self: "Lemmatizer", word: str, pos: str = "") -> str:
-        """ریشهٔ کلمه را پیدا می‌کند.
-
-        پارامتر `pos` نوع کلمه است: (اسم، فعل، صفت و ...) و به این خاطر لازم
-        است که می‌تواند روی ریشه‌یابی کلمات اثر بگذارد؛ مثلاً واژهٔ «اجتماعی» در
-        جایگاه صفت (او یک فرد اجتماعی است)، ریشه‌اش همان «اجتماعی» می‌شود ولی
-        همین واژه در جایگاه اسم (اجتماعی از مردم)، ریشه‌اش می‌شود «اجتماع».
-
-        Examples:
-            >>> lemmatizer = Lemmatizer()
-            >>> lemmatizer.lemmatize('کتاب‌ها')
-            'کتاب'
-            >>> lemmatizer.lemmatize('آتشفشان')
-            'آتشفشان'
-            >>> lemmatizer.lemmatize('می‌روم')
-            'رفت#رو'
-            >>> lemmatizer.lemmatize('گفته_شده_است')
-            'گفت#گو'
-            >>> lemmatizer.lemmatize('نچشیده_است')
-            'چشید#چش'
-            >>> lemmatizer.lemmatize('مردم', pos='N')
-            'مردم'
-            >>> lemmatizer.lemmatize('اجتماعی', pos='AJ')
-            'اجتماعی'
-
-        Args:
-            word: کلمه‌ای که باید پردازش شود.
-            pos: نوع کلمه. این پارامتر سه مقدار `V` (فعل) و `AJ` (صفت) و `PRO` (ضمیر) را می‌پذیرد.
-
-        Returns:
-            ریشهٔ کلمه
-
-        """
-        if not pos and word in self.words:
-            return word
-
-        if (not pos or pos == "V") and word in self.verbs:
-            return self.verbs[word]
-
-        if pos.startswith("AJ") and word[-1] == "ی":
-            return word
-
-        if pos == "PRO":
-            return word
-
-        if word in self.words:
-            return word
-
-        stem = self.stemmer.stem(word)
-        if stem and stem in self.words:
-            return stem
-
-        return word
-
-
-class Conjugation:
-    """این کلاس دارای توابعی برای صرف‌کردن افعال است."""
-
-    def perfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ مطلق صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.perfective_past('دید')
-            ['دیدم', 'دیدی', 'دید', 'دیدیم', 'دیدید', 'دیدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-            صورت‌های صرفی فعل در زمان گذشتهٔ مطلق.
-        """
-        return [ri + x for x in ["م", "ی", "", "یم", "ید", "ند"]]
-
-    def negative_perfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ مطلق به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_perfective_past('دید')
-            ['ندیدم', 'ندیدی', 'ندید', 'ندیدیم', 'ندیدید', 'ندیدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.perfective_past(ri)]
-
-    def passive_perfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ مطلق در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_perfective_past('دید')
-            ['دیده شدم', 'دیده شدی', 'دیده شد', 'دیده شدیم', 'دیده شدید', 'دیده شدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.perfective_past("شد")]
-
-    def negative_passive_perfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_perfective_past('دید')
-            ['دیده نشدم', 'دیده نشدی', 'دیده نشد', 'دیده نشدیم', 'دیده نشدید', 'دیده نشدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_perfective_past("شد")]
-
-    def imperfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_past('دید')
-            ['می‌دیدم', 'می‌دیدی', 'می‌دید', 'می‌دیدیم', 'می‌دیدید', 'می‌دیدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پایا.
-        """
-        return ["می‌" + x for x in self.perfective_past(ri)]
-
-    def negative_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_past('دید')
-            ['نمی‌دیدم', 'نمی‌دیدی', 'نمی‌دید', 'نمی‌دیدیم', 'نمی‌دیدید', 'نمی‌دیدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_past(ri)]
-
-    def passive_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_past('دید')
-            ['دیده می‌شدم', 'دیده می‌شدی', 'دیده می‌شد', 'دیده می‌شدیم', 'دیده می‌شدید', 'دیده می‌شدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_past("شد")]
-
-    def negative_passive_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_past('دید')
-            ['دیده نمی‌شدم', 'دیده نمی‌شدی', 'دیده نمی‌شد', 'دیده نمی‌شدیم', 'دیده نمی‌شدید', 'دیده نمی‌شدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_imperfective_past("شد")]
-
-    def past_progresive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ استمراری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.past_progresive('دید')
-            ['داشتم می‌دیدم', 'داشتی می‌دیدی', 'داشت می‌دید', 'داشتیم می‌دیدیم', 'داشتید می‌دیدید', 'داشتند می‌دیدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ استمراری.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(self.perfective_past("داشت"), self.imperfective_past(ri))
-        ]
-
-    def passive_past_progresive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ استمراری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_past_progresive('دید')
-            ['داشتم دیده می‌شدم', 'داشتی دیده می‌شدی', 'داشت دیده می‌شد', 'داشتیم دیده می‌شدیم', 'داشتید دیده می‌شدید', 'داشتند دیده می‌شدند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ استمراری در حالت مجهول.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.perfective_past("داشت"),
-                self.passive_imperfective_past(ri),
-            )
-        ]
-
-    def present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.present_perfect('دید')
-            ['دیده‌ام', 'دیده‌ای', 'دیده است', 'دیده', 'دیده‌ایم', 'دیده‌اید', 'دیده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل.
-        """
-        return [ri + x for x in ["ه‌ام", "ه‌ای", "ه است", "ه", "ه‌ایم", "ه‌اید", "ه‌اند"]]
-
-    def negative_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_present_perfect('دید')
-            ['ندیده‌ام', 'ندیده‌ای', 'ندیده است', 'ندیده', 'ندیده‌ایم', 'ندیده‌اید', 'ندیده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.present_perfect(ri)]
-
-    def subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه التزامی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.subjunctive_present_perfect('دید')
-            ['دیده باشم', 'دیده باشی', 'دیده باشد', 'دیده باشیم', 'دیده باشید', 'دیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی.
-        """
-        return [ri + "ه " + x for x in self.perfective_present("باش")]
-
-    def negative_subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه التزامی به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_subjunctive_present_perfect('دید')
-            ['ندیده باشم', 'ندیده باشی', 'ندیده باشد', 'ندیده باشیم', 'ندیده باشید', 'ندیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.subjunctive_present_perfect(ri)]
-
-    def grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه دستوری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.grammatical_present_perfect('دید')
-            ['دیده باشم', 'دیده باش', 'دیده باشد', 'دیده باشیم', 'دیده باشید', 'دیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری.
-        """
-        return [
-            ri + "ه " + ("باش" if x == "باشی" else x)
-            for x in self.perfective_present("باش")
-        ]
-
-    def negative_grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه دستوری به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_grammatical_present_perfect('دید')
-            ['ندیده باشم', 'ندیده باش', 'ندیده باشد', 'ندیده باشیم', 'ندیده باشید', 'ندیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری به‌شکل منفی.
-        """
-        return [
-            "ن" + ri + "ه " + ("باش" if x == "باشی" else x)
-            for x in self.perfective_present("باش")
-        ]
-
-    def passive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_present_perfect('دید')
-            ['دیده شده‌ام', 'دیده شده‌ای', 'دیده شده است', 'دیده شده', 'دیده شده‌ایم', 'دیده شده‌اید', 'دیده شده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.present_perfect("شد")]
-
-    def negative_passive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_present_perfect('دید')
-            ['دیده نشده‌ام', 'دیده نشده‌ای', 'دیده نشده است', 'دیده نشده', 'دیده نشده‌ایم', 'دیده نشده‌اید', 'دیده نشده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_present_perfect("شد")]
-
-    def passive_subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه التزامی در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_subjunctive_present_perfect('دید')
-            ['دیده شده باشم', 'دیده شده باشی', 'دیده شده باشد', 'دیده شده باشیم', 'دیده شده باشید', 'دیده شده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.subjunctive_present_perfect("شد")]
-
-    def negative_passive_subjunctive_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_subjunctive_present_perfect('دید')
-            ['دیده نشده باشم', 'دیده نشده باشی', 'دیده نشده باشد', 'دیده نشده باشیم', 'دیده نشده باشید', 'دیده نشده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_subjunctive_present_perfect("شد")]
-
-    def passive_grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل در وجه دستوری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_grammatical_present_perfect('دید')
-            ['دیده شده باشم', 'دیده شده باش', 'دیده شده باشد', 'دیده شده باشیم', 'دیده شده باشید', 'دیده شده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری در حالت مجهول.
-        """
-        return [
-            ri + "ه شده " + ("باش" if x == "باشی" else x)
-            for x in self.perfective_present("باش")
-        ]
-
-    def negative_passive_grammatical_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_grammatical_present_perfect('دید')
-            ['دیده نشده باشم', 'دیده نشده باش', 'دیده نشده باشد', 'دیده نشده باشیم', 'دیده نشده باشید', 'دیده نشده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه نشده " + ("باش" if x == "باشی" else x)
-            for x in self.perfective_present("باش")
-        ]
-
-    def imperfective_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_present_perfect('دید')
-            ['می‌دیده‌ام', 'می‌دیده‌ای', 'می‌دیده است', 'می‌دیده', 'می‌دیده‌ایم', 'می‌دیده‌اید', 'می‌دیده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا.
-        """
-        return ["می‌" + x for x in self.present_perfect(ri)]
-
-    def negative_imperfective_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_present_perfect('دید')
-            ['نمی‌دیده‌ام', 'نمی‌دیده‌ای', 'نمی‌دیده است', 'نمی‌دیده', 'نمی‌دیده‌ایم', 'نمی‌دیده‌اید', 'نمی‌دیده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_present_perfect(ri)]
-
-    def subjunctive_imperfective_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا در وجه التزامی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.subjunctive_imperfective_present_perfect('دید')
-            ['می‌دیده باشم', 'می‌دیده باشی', 'می‌دیده باشد', 'می‌دیده باشیم', 'می‌دیده باشید', 'می‌دیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی.
-        """
-        return ["می‌" + x for x in self.subjunctive_present_perfect(ri)]
-
-    def negative_subjunctive_imperfective_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا در وجه التزامی به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_subjunctive_imperfective_present_perfect('دید')
-            ['نمی‌دیده باشم', 'نمی‌دیده باشی', 'نمی‌دیده باشد', 'نمی‌دیده باشیم', 'نمی‌دیده باشید', 'نمی‌دیده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.subjunctive_imperfective_present_perfect(ri)]
-
-    def passive_imperfective_present_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_present_perfect('دید')
-            ['دیده می‌شده‌ام', 'دیده می‌شده‌ای', 'دیده می‌شده است', 'دیده می‌شده', 'دیده می‌شده‌ایم', 'دیده می‌شده‌اید', 'دیده می‌شده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_present_perfect("شد")]
-
-    def negative_passive_imperfective_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_present_perfect('دید')
-            ['دیده نمی‌شده‌ام', 'دیده نمی‌شده‌ای', 'دیده نمی‌شده است', 'دیده نمی‌شده', 'دیده نمی‌شده‌ایم', 'دیده نمی‌شده‌اید', 'دیده نمی‌شده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_imperfective_present_perfect("شد")]
-
-    def passive_subjunctive_imperfective_present_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا در وجه التزامی در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_subjunctive_imperfective_present_perfect('دید')
-            ['دیده می‌شده باشم', 'دیده می‌شده باشی', 'دیده می‌شده باشد', 'دیده می‌شده باشیم', 'دیده می‌شده باشید', 'دیده می‌شده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی در حالت مجهول.
-        """
-        return [
-            ri + "ه " + x for x in self.subjunctive_imperfective_present_perfect("شد")
-        ]
-
-    def negative_passive_subjunctive_imperfective_present_perfect(
-        self: "Conjugation",
-        ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_subjunctive_imperfective_present_perfect('دید')
-            ['دیده نمی‌شده باشم', 'دیده نمی‌شده باشی', 'دیده نمی‌شده باشد', 'دیده نمی‌شده باشیم', 'دیده نمی‌شده باشید', 'دیده نمی‌شده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + x
-            for x in self.negative_subjunctive_imperfective_present_perfect("شد")
-        ]
-
-    def present_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل استمراری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.present_perfect_progressive('دید')
-            ['داشته‌ام می‌دیده‌ام', 'داشته‌ای می‌دیده‌ای', 'داشته است می‌دیده است', 'داشته می‌دیده', 'داشته‌ایم می‌دیده‌ایم', 'داشته‌اید می‌دیده‌اید', 'داشته‌اند می‌دیده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل استمراری.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.present_perfect("داشت"),
-                self.imperfective_present_perfect(ri),
-            )
-        ]
-
-    def passive_present_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال کامل استمراری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_present_perfect_progressive('دید')
-            ['داشته‌ام دیده می‌شده‌ام', 'داشته‌ای دیده می‌شده‌ای', 'داشته است دیده می‌شده است', 'داشته دیده می‌شده', 'داشته‌ایم دیده می‌شده‌ایم', 'داشته‌اید دیده می‌شده‌اید', 'داشته‌اند دیده می‌شده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال کامل استمراری در حالت مجهول.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.present_perfect("داشت"),
-                self.passive_imperfective_present_perfect(ri),
-            )
-        ]
-
-    def past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.past_precedent('دید')
-            ['دیده بودم', 'دیده بودی', 'دیده بود', 'دیده بودیم', 'دیده بودید', 'دیده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین.
-        """
-        return [ri + "ه " + x for x in self.perfective_past("بود")]
-
-    def negative_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_past_precedent('دید')
-            ['ندیده بودم', 'ندیده بودی', 'ندیده بود', 'ندیده بودیم', 'ندیده بودید', 'ندیده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.past_precedent(ri)]
-
-    def passive_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_past_precedent('دید')
-            ['دیده شده بودم', 'دیده شده بودی', 'دیده شده بود', 'دیده شده بودیم', 'دیده شده بودید', 'دیده شده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.past_precedent("شد")]
-
-    def negative_passive_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_past_precedent('دید')
-            ['دیده نشده بودم', 'دیده نشده بودی', 'دیده نشده بود', 'دیده نشده بودیم', 'دیده نشده بودید', 'دیده نشده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_past_precedent("شد")]
-
-    def imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_past_precedent('دید')
-            ['می‌دیده بودم', 'می‌دیده بودی', 'می‌دیده بود', 'می‌دیده بودیم', 'می‌دیده بودید', 'می‌دیده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا.
-        """
-        return ["می‌" + x for x in self.past_precedent(ri)]
-
-    def negative_imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_past_precedent('دید')
-            ['نمی‌دیده بودم', 'نمی‌دیده بودی', 'نمی‌دیده بود', 'نمی‌دیده بودیم', 'نمی‌دیده بودید', 'نمی‌دیده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_past_precedent(ri)]
-
-    def passive_imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_past_precedent('دید')
-            ['دیده می‌شده بودم', 'دیده می‌شده بودی', 'دیده می‌شده بود', 'دیده می‌شده بودیم', 'دیده می‌شده بودید', 'دیده می‌شده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_past_precedent("شد")]
-
-    def negative_passive_imperfective_past_precedent(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_past_precedent('دید')
-            ['دیده نمی‌شده بودم', 'دیده نمی‌شده بودی', 'دیده نمی‌شده بود', 'دیده نمی‌شده بودیم', 'دیده نمی‌شده بودید', 'دیده نمی‌شده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_imperfective_past_precedent("شد")]
-
-    def past_precedent_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین استمراری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.past_precedent_progressive('دید')
-            ['داشتم می‌دیده بودم', 'داشتی می‌دیده بودی', 'داشت می‌دیده بود', 'داشتیم می‌دیده بودیم', 'داشتید می‌دیده بودید', 'داشتند می‌دیده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین استمراری.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.perfective_past("داشت"),
-                self.imperfective_past_precedent(ri),
-            )
-        ]
-
-    def passive_past_precedent_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین استمراری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_past_precedent_progressive('دید')
-            ['داشتم دیده می‌شده بودم', 'داشتی دیده می‌شده بودی', 'داشت دیده می‌شده بود', 'داشتیم دیده می‌شده بودیم', 'داشتید دیده می‌شده بودید', 'داشتند دیده می‌شده بودند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین استمراری در حالت مجهول.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.perfective_past("داشت"),
-                self.passive_imperfective_past_precedent(ri),
-            )
-        ]
-
-    def past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.past_precedent_perfect('دید')
-            ['دیده بوده‌ام', 'دیده بوده‌ای', 'دیده بوده است', 'دیده بوده', 'دیده بوده‌ایم', 'دیده بوده‌اید', 'دیده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل.
-        """
-        return [ri + "ه " + x for x in self.present_perfect("بود")]
-
-    def negative_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_past_precedent_perfect('دید')
-            ['ندیده بوده‌ام', 'ندیده بوده‌ای', 'ندیده بوده است', 'ندیده بوده', 'ندیده بوده‌ایم', 'ندیده بوده‌اید', 'ندیده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.past_precedent_perfect(ri)]
-
-    def subjunctive_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.subjunctive_past_precedent_perfect('دید')
-            ['دیده بوده باشم', 'دیده بوده باشی', 'دیده بوده باشد', 'دیده بوده باشیم', 'دیده بوده باشید', 'دیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی.
-        """
-        return [ri + "ه " + x for x in self.subjunctive_present_perfect("بود")]
-
-    def negative_subjunctive_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_subjunctive_past_precedent_perfect('دید')
-            ['ندیده بوده باشم', 'ندیده بوده باشی', 'ندیده بوده باشد', 'ندیده بوده باشیم', 'ندیده بوده باشید', 'ندیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.subjunctive_past_precedent_perfect(ri)]
-
-    def grammatical_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.grammatical_past_precedent_perfect('دید')
-            ['دیده بوده باشم', 'دیده بوده باش', 'دیده بوده باشد', 'دیده بوده باشیم', 'دیده بوده باشید', 'دیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری.
-        """
-        return [
-            ri + "ه بوده " + ("باش" if x == "باشی" else x)
-            for x in self.perfective_present("باش")
-        ]
-
-    def negative_grammatical_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_grammatical_past_precedent_perfect('دید')
-            ['ندیده بوده باشم', 'ندیده بوده باش', 'ندیده بوده باشد', 'ندیده بوده باشیم', 'ندیده بوده باشید', 'ندیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.grammatical_past_precedent_perfect(ri)]
-
-    def passive_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_past_precedent_perfect('دید')
-            ['دیده شده بوده‌ام', 'دیده شده بوده‌ای', 'دیده شده بوده است', 'دیده شده بوده', 'دیده شده بوده‌ایم', 'دیده شده بوده‌اید', 'دیده شده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.past_precedent_perfect("شد")]
-
-    def negative_passive_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_past_precedent_perfect('دید')
-            ['دیده نشده بوده‌ام', 'دیده نشده بوده‌ای', 'دیده نشده بوده است', 'دیده نشده بوده', 'دیده نشده بوده‌ایم', 'دیده نشده بوده‌اید', 'دیده نشده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_past_precedent_perfect("شد")]
-
-    def passive_subjunctive_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_subjunctive_past_precedent_perfect('دید')
-            ['دیده شده بوده باشم', 'دیده شده بوده باشی', 'دیده شده بوده باشد', 'دیده شده بوده باشیم', 'دیده شده بوده باشید', 'دیده شده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.subjunctive_past_precedent_perfect("شد")]
-
-    def negative_passive_subjunctive_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_subjunctive_past_precedent_perfect('دید')
-            ['دیده نشده بوده باشم', 'دیده نشده بوده باشی', 'دیده نشده بوده باشد', 'دیده نشده بوده باشیم', 'دیده نشده بوده باشید', 'دیده نشده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + "ن" + x for x in self.subjunctive_past_precedent_perfect("شد")
-        ]
-
-    def passive_grammatical_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_grammatical_past_precedent_perfect('دید')
-            ['دیده شده بوده باشم', 'دیده شده بوده باش', 'دیده شده بوده باشد', 'دیده شده بوده باشیم', 'دیده شده بوده باشید', 'دیده شده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.grammatical_past_precedent_perfect("شد")]
-
-    def negative_passive_grammatical_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_grammatical_past_precedent_perfect('دید')
-            ['دیده نشده بوده باشم', 'دیده نشده بوده باش', 'دیده نشده بوده باشد', 'دیده نشده بوده باشیم', 'دیده نشده بوده باشید', 'دیده نشده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + x
-            for x in self.negative_grammatical_past_precedent_perfect("شد")
-        ]
-
-    def imperfective_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_past_precedent_perfect('دید')
-            ['می‌دیده بوده‌ام', 'می‌دیده بوده‌ای', 'می‌دیده بوده است', 'می‌دیده بوده', 'می‌دیده بوده‌ایم', 'می‌دیده بوده‌اید', 'می‌دیده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا.
-        """
-        return ["می‌" + x for x in self.past_precedent_perfect(ri)]
-
-    def negative_imperfective_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_past_precedent_perfect('دید')
-            ['نمی‌دیده بوده‌ام', 'نمی‌دیده بوده‌ای', 'نمی‌دیده بوده است', 'نمی‌دیده بوده', 'نمی‌دیده بوده‌ایم', 'نمی‌دیده بوده‌اید', 'نمی‌دیده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_past_precedent_perfect(ri)]
-
-    def subjunctive_imperfective_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.subjunctive_imperfective_past_precedent_perfect('دید')
-            ['می‌دیده بوده باشم', 'می‌دیده بوده باشی', 'می‌دیده بوده باشد', 'می‌دیده بوده باشیم', 'می‌دیده بوده باشید', 'می‌دیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی.
-        """
-        return ["می‌" + x for x in self.subjunctive_past_precedent_perfect(ri)]
-
-    def negative_subjunctive_imperfective_past_precedent_perfect(
-        self: "Conjugation",
-        ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_subjunctive_imperfective_past_precedent_perfect('دید')
-            ['نمی‌دیده بوده باشم', 'نمی‌دیده بوده باشی', 'نمی‌دیده بوده باشد', 'نمی‌دیده بوده باشیم', 'نمی‌دیده بوده باشید', 'نمی‌دیده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی به‌شکل منفی.
-        """
-        return [
-            "ن" + x for x in self.subjunctive_imperfective_past_precedent_perfect(ri)
-        ]
-
-    def passive_imperfective_past_precedent_perfect(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_past_precedent_perfect('دید')
-            ['دیده می‌شده بوده‌ام', 'دیده می‌شده بوده‌ای', 'دیده می‌شده بوده است', 'دیده می‌شده بوده', 'دیده می‌شده بوده‌ایم', 'دیده می‌شده بوده‌اید', 'دیده می‌شده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_past_precedent_perfect("شد")]
-
-    def negative_passive_imperfective_past_precedent_perfect(
-        self: "Conjugation",
-        ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_past_precedent_perfect('دید')
-            ['دیده نمی‌شده بوده‌ام', 'دیده نمی‌شده بوده‌ای', 'دیده نمی‌شده بوده است', 'دیده نمی‌شده بوده', 'دیده نمی‌شده بوده‌ایم', 'دیده نمی‌شده بوده‌اید', 'دیده نمی‌شده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + x
-            for x in self.negative_imperfective_past_precedent_perfect("شد")
-        ]
-
-    def passive_subjunctive_imperfective_past_precedent_perfect(
-        self: "Conjugation",
-        ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_subjunctive_imperfective_past_precedent_perfect('دید')
-            ['دیده می‌شده بوده باشم', 'دیده می‌شده بوده باشی', 'دیده می‌شده بوده باشد', 'دیده می‌شده بوده باشیم', 'دیده می‌شده بوده باشید', 'دیده می‌شده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول.
-        """
-        return [
-            ri + "ه " + x
-            for x in self.subjunctive_imperfective_past_precedent_perfect("شد")
-        ]
-
-    def negative_passive_subjunctive_imperfective_past_precedent_perfect(
-        self: "Conjugation",
-        ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_subjunctive_imperfective_past_precedent_perfect('دید')
-            ['دیده نمی‌شده بوده باشم', 'دیده نمی‌شده بوده باشی', 'دیده نمی‌شده بوده باشد', 'دیده نمی‌شده بوده باشیم', 'دیده نمی‌شده بوده باشید', 'دیده نمی‌شده بوده باشند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + "ن" + x
-            for x in self.subjunctive_imperfective_past_precedent_perfect("شد")
-        ]
-
-    def past_precedent_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل استمراری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.past_precedent_perfect_progressive('دید')
-            ['داشته‌ام می‌دیده بوده‌ام', 'داشته‌ای می‌دیده بوده‌ای', 'داشته است می‌دیده بوده است', 'داشته می‌دیده بوده', 'داشته‌ایم می‌دیده بوده‌ایم', 'داشته‌اید می‌دیده بوده‌اید', 'داشته‌اند می‌دیده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل استمراری.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.present_perfect("داشت"),
-                self.imperfective_past_precedent_perfect(ri),
-            )
-        ]
-
-    def passive_past_precedent_perfect_progressive(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان گذشتهٔ پیشین کامل استمراری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_past_precedent_perfect_progressive('دید')
-            ['داشته‌ام دیده می‌شده بوده‌ام', 'داشته‌ای دیده می‌شده بوده‌ای', 'داشته است دیده می‌شده بوده است', 'داشته دیده می‌شده بوده', 'داشته‌ایم دیده می‌شده بوده‌ایم', 'داشته‌اید دیده می‌شده بوده‌اید', 'داشته‌اند دیده می‌شده بوده‌اند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل استمراری در حالت مجهول.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.present_perfect("داشت"),
-                self.passive_imperfective_past_precedent_perfect(ri),
-            )
-        ]
-
-    def perfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال مطلق صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.perfective_present('بین')
-            ['بینم', 'بینی', 'بیند', 'بینیم', 'بینید', 'بینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق.
-        """
-        return [rii + x for x in ["م", "ی", "د", "یم", "ید", "ند"]]
-
-    def negative_perfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال مطلق به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_perfective_present('بین')
-            ['نبینم', 'نبینی', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.perfective_present(rii)]
-
-    def subjunctive_perfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه التزامی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.subjunctive_perfective_present('بین')
-            ['ببینم', 'ببینی', 'ببیند', 'ببینیم', 'ببینید', 'ببینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی.
-        """
-        return ["ب" + x for x in self.perfective_present(rii)]
-
-    def negative_subjunctive_perfective_present(
-        self: "Conjugation", rii: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه التزامی به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_subjunctive_perfective_present('بین')
-            ['نبینم', 'نبینی', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.perfective_present(rii)]
-
-    def grammatical_perfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه دستوری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.grammatical_perfective_present('بین')
-            ['ببینم', 'ببین', 'ببیند', 'ببینیم', 'ببینید', 'ببینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری.
-        """
-        return [
-            "ببین" if x == "ببینی" else x
-            for x in self.subjunctive_perfective_present(rii)
-        ]
-
-    def negative_grammatical_perfective_present(
-        self: "Conjugation", rii: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه دستوری به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_grammatical_perfective_present('بین')
-            ['نبینم', 'نبین', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری به‌شکل منفی.
-        """
-        return [
-            "ن" + ("بین" if x == "بینی" else x) for x in self.perfective_present(rii)
-        ]
-
-    def passive_perfective_present(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال مطلق در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_perfective_present('دید')
-            ['دیده شوم', 'دیده شوی', 'دیده شود', 'دیده شویم', 'دیده شوید', 'دیده شوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.perfective_present("شو")]
-
-    def negative_passive_perfective_present(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_perfective_present('دید')
-            ['دیده نشوم', 'دیده نشوی', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_perfective_present("شو")]
-
-    def passive_subjunctive_perfective_present(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه التزامی در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_subjunctive_perfective_present('دید')
-            ['دیده بشوم', 'دیده بشوی', 'دیده بشود', 'دیده بشویم', 'دیده بشوید', 'دیده بشوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.subjunctive_perfective_present("شو")]
-
-    def negative_passive_subjunctive_perfective_present(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_subjunctive_perfective_present('دید')
-            ['دیده نشوم', 'دیده نشوی', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + x for x in self.negative_subjunctive_perfective_present("شو")
-        ]
-
-    def passive_grammatical_perfective_present(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه دستوری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_grammatical_perfective_present('دید')
-            ['دیده بشوم', 'دیده بشو', 'دیده بشود', 'دیده بشویم', 'دیده بشوید', 'دیده بشوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری در حالت مجهول.
-        """
-        return [
-            ri + "ه " + ("بشو" if x == "بشوی" else x)
-            for x in self.grammatical_perfective_present("شو")
-        ]
-
-    def negative_passive_grammatical_perfective_present(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال مطلق در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_grammatical_perfective_present('دید')
-            ['دیده نشوم', 'دیده نشو', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + ("نشو" if x == "نشوی" else x)
-            for x in self.negative_grammatical_perfective_present("شو")
-        ]
-
-    def imperfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_present('بین')
-            ['می‌بینم', 'می‌بینی', 'می‌بیند', 'می‌بینیم', 'می‌بینید', 'می‌بینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال پایا.
-        """
-        return ["می‌" + x for x in self.perfective_present(rii)]
-
-    def negative_imperfective_present(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_present('بین')
-            ['نمی‌بینم', 'نمی‌بینی', 'نمی‌بیند', 'نمی‌بینیم', 'نمی‌بینید', 'نمی‌بینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_present(rii)]
-
-    def passive_imperfective_present(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_present('دید')
-            ['دیده می‌شوم', 'دیده می‌شوی', 'دیده می‌شود', 'دیده می‌شویم', 'دیده می‌شوید', 'دیده می‌شوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_present("شو")]
-
-    def negative_passive_imperfective_present(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان حال پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_present('دید')
-            ['دیده نمی‌شوم', 'دیده نمی‌شوی', 'دیده نمی‌شود', 'دیده نمی‌شویم', 'دیده نمی‌شوید', 'دیده نمی‌شوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_imperfective_present("شو")]
-
-    def present_progressive(self: "Conjugation", rii: str) -> List[str]:
-        """فعل را در زمان حال استمراری صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.present_progressive('بین')
-            ['دارم می‌بینم', 'داری می‌بینی', 'دارد می‌بیند', 'داریم می‌بینیم', 'دارید می‌بینید', 'دارند می‌بینند']
-
-        Args:
-            rii: بن مضارع فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال استمراری.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.perfective_present("دار"),
-                self.imperfective_present(rii),
-            )
-        ]
-
-    def passive_present_progressive(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان حال استمراری در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_present_progressive('دید')
-            ['دارم دیده می‌شوم', 'داری دیده می‌شوی', 'دارد دیده می‌شود', 'داریم دیده می‌شویم', 'دارید دیده می‌شوید', 'دارند دیده می‌شوند']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان حال استمراری در حالت مجهول.
-        """
-        return [
-            x + " " + y
-            for x, y in zip(
-                self.perfective_present("دار"),
-                self.passive_imperfective_present(ri),
-            )
-        ]
-
-    def perfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ مطلق صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.perfective_future('دید')
-            ['خواهم دید', 'خواهی دید', 'خواهد دید', 'خواهیم دید', 'خواهید دید', 'خواهند دید']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ مطلق.
-        """
-        return [x + " " + ri for x in self.perfective_present("خواه")]
-
-    def negative_perfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ مطلق به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_perfective_future('دید')
-            ['نخواهم دید', 'نخواهی دید', 'نخواهد دید', 'نخواهیم دید', 'نخواهید دید', 'نخواهند دید']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ مطلق به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.perfective_future(ri)]
-
-    def passive_perfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ مطلق در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_perfective_future('دید')
-            ['دیده خواهم شد', 'دیده خواهی شد', 'دیده خواهد شد', 'دیده خواهیم شد', 'دیده خواهید شد', 'دیده خواهند شد']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ مطلق در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.perfective_future("شد")]
-
-    def negative_passive_perfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_perfective_future('دید')
-            ['دیده نخواهم شد', 'دیده نخواهی شد', 'دیده نخواهد شد', 'دیده نخواهیم شد', 'دیده نخواهید شد', 'دیده نخواهند شد']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ مطلق در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_perfective_future("شد")]
-
-    def imperfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.imperfective_future('دید')
-            ['می‌خواهم دید', 'می‌خواهی دید', 'می‌خواهد دید', 'می‌خواهیم دید', 'می‌خواهید دید', 'می‌خواهند دید']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پایا.
-        """
-        return ["می‌" + x for x in self.perfective_future(ri)]
-
-    def negative_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_imperfective_future('دید')
-            ['نمی‌خواهم دید', 'نمی‌خواهی دید', 'نمی‌خواهد دید', 'نمی‌خواهیم دید', 'نمی‌خواهید دید', 'نمی‌خواهند دید']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.imperfective_future(ri)]
-
-    def passive_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_imperfective_future('دید')
-            ['دیده می‌خواهم شد', 'دیده می‌خواهی شد', 'دیده می‌خواهد شد', 'دیده می‌خواهیم شد', 'دیده می‌خواهید شد', 'دیده می‌خواهند شد']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.imperfective_future("شد")]
-
-    def negative_passive_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_imperfective_future('دید')
-            ['دیده نمی‌خواهم شد', 'دیده نمی‌خواهی شد', 'دیده نمی‌خواهد شد', 'دیده نمی‌خواهیم شد', 'دیده نمی‌خواهید شد', 'دیده نمی‌خواهند شد']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_imperfective_future("شد")]
-
-    def future_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.future_precedent('دید')
-            ['دیده خواهم بود', 'دیده خواهی بود', 'دیده خواهد بود', 'دیده خواهیم بود', 'دیده خواهید بود', 'دیده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین.
-        """
-        return [ri + "ه " + x for x in self.perfective_future("بود")]
-
-    def negative_future_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_future_precedent('دید')
-            ['ندیده خواهم بود', 'ندیده خواهی بود', 'ندیده خواهد بود', 'ندیده خواهیم بود', 'ندیده خواهید بود', 'ندیده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.future_precedent(ri)]
-
-    def passive_future_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_future_precedent('دید')
-            ['دیده شده خواهم بود', 'دیده شده خواهی بود', 'دیده شده خواهد بود', 'دیده شده خواهیم بود', 'دیده شده خواهید بود', 'دیده شده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.future_precedent("شد")]
-
-    def negative_passive_future_precedent(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_future_precedent('دید')
-            ['دیده نشده خواهم بود', 'دیده نشده خواهی بود', 'دیده نشده خواهد بود', 'دیده نشده خواهیم بود', 'دیده نشده خواهید بود', 'دیده نشده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین در حالت مجهول به‌شکل منفی.
-        """
-        return [ri + "ه " + x for x in self.negative_future_precedent("شد")]
-
-    def future_precedent_imperfective(self: "Conjugation", ri: str) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین پایا صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.future_precedent_imperfective('دید')
-            ['می‌دیده خواهم بود', 'می‌دیده خواهی بود', 'می‌دیده خواهد بود', 'می‌دیده خواهیم بود', 'می‌دیده خواهید بود', 'می‌دیده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا.
-        """
-        return ["می‌" + x for x in self.future_precedent(ri)]
-
-    def negative_future_precedent_imperfective(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین پایا به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_future_precedent_imperfective('دید')
-            ['نمی‌دیده خواهم بود', 'نمی‌دیده خواهی بود', 'نمی‌دیده خواهد بود', 'نمی‌دیده خواهیم بود', 'نمی‌دیده خواهید بود', 'نمی‌دیده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا به‌شکل منفی.
-        """
-        return ["ن" + x for x in self.future_precedent_imperfective(ri)]
-
-    def passive_future_precedent_imperfective(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین پایا در حالت مجهول صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.passive_future_precedent_imperfective('دید')
-            ['دیده می‌شده خواهم بود', 'دیده می‌شده خواهی بود', 'دیده می‌شده خواهد بود', 'دیده می‌شده خواهیم بود', 'دیده می‌شده خواهید بود', 'دیده می‌شده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا در حالت مجهول.
-        """
-        return [ri + "ه " + x for x in self.future_precedent_imperfective("شد")]
-
-    def negative_passive_future_precedent_imperfective(
-        self: "Conjugation", ri: str,
-    ) -> List[str]:
-        """فعل را در زمان آیندهٔ پیشین پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
-
-        Examples:
-            >>> conj = Conjugation()
-            >>> conj.negative_passive_future_precedent_imperfective('دید')
-            ['دیده نمی‌شده خواهم بود', 'دیده نمی‌شده خواهی بود', 'دیده نمی‌شده خواهد بود', 'دیده نمی‌شده خواهیم بود', 'دیده نمی‌شده خواهید بود', 'دیده نمی‌شده خواهند بود']
-
-        Args:
-            ri: بن ماضی فعل.
-
-        Returns:
-             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا در حالت مجهول به‌شکل منفی.
-        """
-        return [
-            ri + "ه " + x for x in self.negative_future_precedent_imperfective("شد")
-        ]
-
-    def get(self: "Conjugation", verb, negative=False, passive=False) -> List[str]:
-        """صورت‌های صرفی فعل را برمی‌گرداند.
-
-        Args:
-            verb (str): فعلی که باید صرف شود. به‌صورت بن ماضی#بن مضارع؛ مانند: دید#بین.
-            negative (bool, optional): اگر `True` باشد صورت‌های صرفی منفی را برمی‌گرداند.
-            passive (bool, optional): اگر `True` باشد صورت‌های صرفی مجهول را برمی‌گرداند.
-
-        Returns:
-            (List(str)): صورت‌های صرفی فعل.
-        """
-        ri, rii = verb.split("#")
-        infinitive = [ri + "ن"]
-        result = [infinitive]
-
-        if negative and passive:
-            result.append(self.negative_passive_perfective_past(ri))
-            result.append(self.negative_passive_imperfective_past(ri))
-            result.append(self.negative_passive_present_perfect(ri))
-            result.append(self.negative_passive_subjunctive_present_perfect(ri))
-            result.append(self.negative_passive_grammatical_present_perfect(ri))
-            result.append(self.negative_passive_imperfective_present_perfect(ri))
-            result.append(
-                self.negative_passive_subjunctive_imperfective_present_perfect(ri),
-            )
-            result.append(self.negative_passive_past_precedent(ri))
-            result.append(self.negative_passive_imperfective_past_precedent(ri))
-            result.append(self.negative_passive_past_precedent_perfect(ri))
-            result.append(self.negative_passive_subjunctive_past_precedent_perfect(ri))
-            result.append(self.negative_passive_grammatical_past_precedent_perfect(ri))
-            result.append(self.negative_passive_imperfective_past_precedent_perfect(ri))
-            result.append(
-                self.negative_passive_subjunctive_imperfective_past_precedent_perfect(
-                    ri,
-                ),
-            )
-            result.append(self.negative_passive_perfective_present(ri))
-            result.append(self.negative_passive_subjunctive_perfective_present(ri))
-            result.append(self.negative_passive_grammatical_perfective_present(ri))
-            result.append(self.negative_passive_imperfective_present(ri))
-            result.append(self.negative_passive_perfective_future(ri))
-            result.append(self.negative_passive_imperfective_future(ri))
-            result.append(self.negative_passive_future_precedent(ri))
-            result.append(self.negative_passive_future_precedent_imperfective(ri))
-
-        elif passive and not negative:
-            result.append(self.passive_perfective_past(ri))
-            result.append(self.passive_imperfective_past(ri))
-            result.append(self.passive_past_progresive(ri))
-            result.append(self.passive_present_perfect(ri))
-            result.append(self.passive_subjunctive_present_perfect(ri))
-            result.append(self.passive_grammatical_present_perfect(ri))
-            result.append(self.passive_imperfective_present_perfect(ri))
-            result.append(self.passive_subjunctive_imperfective_present_perfect(ri))
-            result.append(self.passive_present_perfect_progressive(ri))
-            result.append(self.passive_past_precedent(ri))
-            result.append(self.passive_imperfective_past_precedent(ri))
-            result.append(self.passive_past_precedent_progressive(ri))
-            result.append(self.passive_past_precedent_perfect(ri))
-            result.append(self.passive_subjunctive_past_precedent_perfect(ri))
-            result.append(self.passive_grammatical_past_precedent_perfect(ri))
-            result.append(self.passive_imperfective_past_precedent_perfect(ri))
-            result.append(
-                self.passive_subjunctive_imperfective_past_precedent_perfect(ri),
-            )
-            result.append(self.passive_past_precedent_perfect_progressive(ri))
-            result.append(self.passive_perfective_present(ri))
-            result.append(self.passive_subjunctive_perfective_present(ri))
-            result.append(self.passive_grammatical_perfective_present(ri))
-            result.append(self.passive_imperfective_present(ri))
-            result.append(self.passive_present_progressive(ri))
-            result.append(self.passive_perfective_future(ri))
-            result.append(self.passive_imperfective_future(ri))
-            result.append(self.passive_future_precedent(ri))
-            result.append(self.passive_future_precedent_imperfective(ri))
-
-        elif negative and not passive:
-            result.append(self.negative_perfective_past(ri))
-            result.append(self.negative_imperfective_past(ri))
-            result.append(self.negative_present_perfect(ri))
-            result.append(self.negative_subjunctive_present_perfect(ri))
-            result.append(self.negative_grammatical_present_perfect(ri))
-            result.append(self.negative_imperfective_present_perfect(ri))
-            result.append(self.negative_subjunctive_imperfective_present_perfect(ri))
-            result.append(self.negative_past_precedent(ri))
-            result.append(self.negative_imperfective_past_precedent(ri))
-            result.append(self.negative_past_precedent_perfect(ri))
-            result.append(self.negative_subjunctive_past_precedent_perfect(ri))
-            result.append(self.negative_grammatical_past_precedent_perfect(ri))
-            result.append(self.negative_imperfective_past_precedent_perfect(ri))
-            result.append(
-                self.negative_subjunctive_imperfective_past_precedent_perfect(ri),
-            )
-            result.append(self.negative_perfective_present(rii))
-            result.append(self.negative_subjunctive_perfective_present(rii))
-            result.append(self.negative_grammatical_perfective_present(rii))
-            result.append(self.negative_imperfective_present(rii))
-            result.append(self.negative_perfective_future(ri))
-            result.append(self.negative_imperfective_future(ri))
-            result.append(self.negative_future_precedent(ri))
-            result.append(self.negative_future_precedent_imperfective(ri))
-
-        elif not negative and not passive:
-            result.append(self.perfective_past(ri))
-            result.append(self.imperfective_past(ri))
-            result.append(self.past_progresive(ri))
-            result.append(self.present_perfect(ri))
-            result.append(self.subjunctive_present_perfect(ri))
-            result.append(self.grammatical_present_perfect(ri))
-            result.append(self.imperfective_present_perfect(ri))
-            result.append(self.subjunctive_imperfective_present_perfect(ri))
-            result.append(self.present_perfect_progressive(ri))
-            result.append(self.past_precedent(ri))
-            result.append(self.imperfective_past_precedent(ri))
-            result.append(self.past_precedent_progressive(ri))
-            result.append(self.past_precedent_perfect(ri))
-            result.append(self.subjunctive_past_precedent_perfect(ri))
-            result.append(self.grammatical_past_precedent_perfect(ri))
-            result.append(self.imperfective_past_precedent_perfect(ri))
-            result.append(self.subjunctive_imperfective_past_precedent_perfect(ri))
-            result.append(self.past_precedent_perfect_progressive(ri))
-            result.append(self.perfective_present(rii))
-            result.append(self.subjunctive_perfective_present(rii))
-            result.append(self.grammatical_perfective_present(rii))
-            result.append(self.imperfective_present(rii))
-            result.append(self.present_progressive(rii))
-            result.append(self.perfective_future(ri))
-            result.append(self.imperfective_future(ri))
-            result.append(self.future_precedent(ri))
-            result.append(self.future_precedent_imperfective(ri))
-
-        return sum(result, [])
-
-    def get_all(self: "Conjugation", verb: str) -> List[str]:
-        """تمام صورت‌های صرفی فعل را در وجوه اخباری، التزامی، دستوری و در اشکال منفی و مثبت و مجهول برمی‌گرداند.
-
-        Args:
-            verb (str): فعلی که باید صرف شود. به‌صورت بن ماضی#بن مضارع؛ مانند: دید#بین.
-
-        Returns:
-             لیست تمام صورت‌های صرفی فعل.
-        """
-        ri, rii = verb.split("#")
-        infinitive = [ri + "ن"]
-        result = [infinitive]
-
-        # گذشتهٔ مطلق
-        result.append(self.perfective_past(ri))
-
-        # گذشتهٔ مطلق منفی
-        result.append(self.negative_perfective_past(ri))
-
-        # گذشتهٔ مطلق مجهول
-        result.append(self.passive_perfective_past(ri))
-
-        # گذشتهٔ مطلق مجهول منفی
-        result.append(self.negative_passive_perfective_past(ri))
-
-        # گذشتهٔ پایا
-        result.append(self.imperfective_past(ri))
-
-        # گذشتهٔ پایای منفی
-        result.append(self.negative_imperfective_past(ri))
-
-        # گذشتهٔ پایای مجهول
-        result.append(self.passive_imperfective_past(ri))
-
-        # گذشتهٔ پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_past(ri))
-
-        # گذشتهٔ استمراری
-        result.append(self.past_progresive(ri))
-
-        # گذشتهٔ استمراری مجهول
-        result.append(self.passive_past_progresive(ri))
-
-        # حال کامل
-        result.append(self.present_perfect(ri))
-
-        # حال کامل منفی
-        result.append(self.negative_present_perfect(ri))
-
-        # حال کامل التزامی
-        result.append(self.subjunctive_present_perfect(ri))
-
-        # حال کامل التزامی منفی
-        result.append(self.negative_subjunctive_present_perfect(ri))
-
-        # حال کامل دستوری
-        result.append(self.grammatical_present_perfect(ri))
-
-        # حال کامل دستوری منفی
-        result.append(self.negative_grammatical_present_perfect(ri))
-
-        # حال کامل مجهول
-        result.append(self.passive_present_perfect(ri))
-
-        # حال کامل مجهول منفی
-        result.append(self.negative_passive_present_perfect(ri))
-
-        # حال کامل التزامی مجهول
-        result.append(self.passive_subjunctive_present_perfect(ri))
-
-        # حال کامل التزامی مجهول منفی
-        result.append(self.negative_passive_subjunctive_present_perfect(ri))
-
-        # حال کامل دستوری مجهول
-        result.append(self.passive_grammatical_present_perfect(ri))
-
-        # حال کامل دستوری مجهول منفی
-        result.append(self.negative_passive_grammatical_present_perfect(ri))
-
-        # حال کامل پایا
-        result.append(self.imperfective_present_perfect(ri))
-
-        # حال کامل پایای منفی
-        result.append(self.negative_imperfective_present_perfect(ri))
-
-        # حال کامل پایای التزامی
-        result.append(self.subjunctive_imperfective_present_perfect(ri))
-
-        # حال کامل پایای التزامی منفی
-        result.append(self.negative_subjunctive_imperfective_present_perfect(ri))
-
-        # حال کامل پایای مجهول
-        result.append(self.passive_imperfective_present_perfect(ri))
-
-        # حال کامل پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_present_perfect(ri))
-
-        # حال کامل پایای التزامی مجهول
-        result.append(self.passive_subjunctive_imperfective_present_perfect(ri))
-
-        # حال کامل پایای التزامی مجهول منفی
-        result.append(
-            self.negative_passive_subjunctive_imperfective_present_perfect(ri),
-        )
-
-        # حال کامل استمراری
-        result.append(self.present_perfect_progressive(ri))
-
-        # حال کامل استمراری مجهول
-        result.append(self.passive_present_perfect_progressive(ri))
-
-        # گذشتهٔ پیشین
-        result.append(self.past_precedent(ri))
-
-        # گذشتهٔ پیشین منفی
-        result.append(self.negative_past_precedent(ri))
-
-        # گذشتهٔ پیشین مجهول
-        result.append(self.passive_past_precedent(ri))
-
-        # گذشتهٔ پیشین مجهول منفی
-        result.append(self.negative_passive_past_precedent(ri))
-
-        # گذشتهٔ پیشین پایا
-        result.append(self.imperfective_past_precedent(ri))
-
-        # گذشتهٔ پیشین پایای منفی
-        result.append(self.negative_imperfective_past_precedent(ri))
-
-        # گذشتهٔ پیشین پایای مجهول
-        result.append(self.passive_imperfective_past_precedent(ri))
-
-        # گذشتهٔ پیشین پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_past_precedent(ri))
-
-        # گذشتهٔ پیشین استمراری
-        result.append(self.past_precedent_progressive(ri))
-
-        # گذشتهٔ پیشین استمراری مجهول
-        result.append(self.passive_past_precedent_progressive(ri))
-
-        # گذشتهٔ پیشین کامل
-        result.append(self.past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل منفی
-        result.append(self.negative_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل التزامی
-        result.append(self.subjunctive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل التزامی منفی
-        result.append(self.negative_subjunctive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل دستوری
-        result.append(self.grammatical_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل دستوری منفی
-        result.append(self.negative_grammatical_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل مجهول
-        result.append(self.passive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل مجهول منفی
-        result.append(self.negative_passive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل التزامی مجهول
-        result.append(self.passive_subjunctive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل التزامی مجهول منفی
-        result.append(self.negative_passive_subjunctive_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشن کامل دستوری مجهول
-        result.append(self.passive_grammatical_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل دستوری مجهول منفی
-        result.append(self.negative_passive_grammatical_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایا
-        result.append(self.imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای منفی
-        result.append(self.negative_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای التزامی
-        result.append(self.subjunctive_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای التزامی منفی
-        result.append(self.negative_subjunctive_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای مجهول
-        result.append(self.passive_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای التزامی مجهول
-        result.append(self.passive_subjunctive_imperfective_past_precedent_perfect(ri))
-
-        # گذشتهٔ پیشین کامل پایای التزامی مجهول منفی
-        result.append(
-            self.negative_passive_subjunctive_imperfective_past_precedent_perfect(ri),
-        )
-
-        # گذشتهٔ پیشین کامل استمراری
-        result.append(self.past_precedent_perfect_progressive(ri))
-
-        # گذشتهٔ پیشین کامل استمراری مجهول
-        result.append(self.passive_past_precedent_perfect_progressive(ri))
-
-        # حال مطلق
-        result.append(self.perfective_present(rii))
-
-        # حال مطلق منفی
-        result.append(self.negative_perfective_present(rii))
-
-        # حال مطلق التزامی
-        result.append(self.subjunctive_perfective_present(rii))
-
-        # حال مطلق التزامی منفی
-        result.append(self.negative_subjunctive_perfective_present(rii))
-
-        # حال مطلق دستوری
-        result.append(self.grammatical_perfective_present(rii))
-
-        # حال مطلق دستوری منفی
-        result.append(self.negative_grammatical_perfective_present(rii))
-
-        # حال مطلق مجهول
-        result.append(self.passive_perfective_present(ri))
-
-        # حال مطلق مجهول منفی
-        result.append(self.negative_passive_perfective_present(ri))
-
-        # حال مطلق التزامی مجهول
-        result.append(self.passive_subjunctive_perfective_present(ri))
-
-        # حال مطلق التزامی مجهول منفی
-        result.append(self.negative_passive_subjunctive_perfective_present(ri))
-
-        # حال مطلق دستوری مجهول
-        result.append(self.passive_grammatical_perfective_present(ri))
-
-        # حال مطلق دستوری مجهول منفی
-        result.append(self.negative_passive_grammatical_perfective_present(ri))
-
-        # حال پایا
-        result.append(self.imperfective_present(rii))
-
-        # حال پایای منفی
-        result.append(self.negative_imperfective_present(rii))
-
-        # حال پایای مجهول
-        result.append(self.passive_imperfective_present(ri))
-
-        # حال پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_present(ri))
-
-        # حال استمراری
-        result.append(self.present_progressive(rii))
-
-        # حال استمراری مجهول
-        result.append(self.passive_present_progressive(ri))
-
-        # آیندهٔ مطلق
-        result.append(self.perfective_future(ri))
-
-        # آیندهٔ مطلق منفی
-        result.append(self.negative_perfective_future(ri))
-
-        # آیندهٔ مطلق مجهول
-        result.append(self.passive_perfective_future(ri))
-
-        # آیندهٔ مطلق مجهول منفی
-        result.append(self.negative_passive_perfective_future(ri))
-
-        # آیندهٔ پایا
-        result.append(self.imperfective_future(ri))
-
-        # آیندهٔ پایای منفی
-        result.append(self.negative_imperfective_future(ri))
-
-        # آیندهٔ پایای مجهول
-        result.append(self.passive_imperfective_future(ri))
-
-        # آیندهٔ پایای مجهول منفی
-        result.append(self.negative_passive_imperfective_future(ri))
-
-        # آیندهٔ پیشین
-        result.append(self.future_precedent(ri))
-
-        # آیندهٔ پیشین منفی
-        result.append(self.negative_future_precedent(ri))
-
-        # آیندهٔ پیشین مجهول
-        result.append(self.passive_future_precedent(ri))
-
-        # آیندهٔ پیشین مجهول منفی
-        result.append(self.negative_passive_future_precedent(ri))
-
-        # آیندهٔ پیشین پایا
-        result.append(self.future_precedent_imperfective(ri))
-
-        # آیندهٔ پیشین پایای منفی
-        result.append(self.negative_future_precedent_imperfective(ri))
-
-        # آیندهٔ پیشین پایای مجهول
-        result.append(self.passive_future_precedent_imperfective(ri))
-
-        # آیندهٔ پیشین پایای مجهول منفی
-        result.append(self.negative_passive_future_precedent_imperfective(ri))
-
-        return sum(result, [])
+"""این ماژول شامل کلاس‌ها و توابعی برای ریشه‌یابی کلمات است.
+
+فرق بین [Lemmatizer](./lemmatizer.md) و [Stemmer](./stemmer.md) این است که
+اِستمر درکی از معنای کلمه ندارد و صرفاً براساس حذف برخی از پسوندهای ساده تلاش
+می‌کند ریشهٔ کلمه را بیابد؛ بنابراین ممکن است در ریشه‌یابیِ برخی از کلمات نتایج
+نادرستی ارائه دهد؛ اما لماتایزر براساس لیستی از کلمات مرجع به همراه ریشهٔ آن
+این
+کار را انجام می‌دهد و نتایج دقیق‌تری ارائه می‌دهد. البته هزینهٔ این دقت، سرعتِ
+کمتر در ریشه‌یابی است.
+
+**میزان دقت
+لماتایزر در نسخهٔ حاضر ۸۹.۹ درصد [^1] است.**
+[^1]:
+این عدد با انتشار هر نسخه بروزرسانی می‌شود
+
+"""
+
+
+from typing import List
+
+from hazm import Stemmer
+from hazm import WordTokenizer
+from hazm import default_verbs
+from hazm import default_words
+
+
+class Lemmatizer:
+    """این کلاس شامل توابعی برای ریشه‌یابی کلمات است.
+
+    Args:
+        words_file: ریشه‌یابی کلمات از روی این فایل صورت
+            می‌گیرد. هضم به صورت پیش‌فرض فایلی برای این منظور در نظر گرفته است؛ با
+            این حال شما می‌توانید فایل موردنظر خود را معرفی کنید. برای آگاهی از
+            ساختار این فایل به فایل پیش‌فرض مراجعه کنید.
+        verbs_file: اشکال صرفی فعل از روی این فایل ساخته
+            می‌شود. هضم به صورت پیش‌فرض فایلی برای این منظور در نظر گرفته است؛ با
+            این حال شما می‌توانید فایل موردنظر خود را معرفی کنید. برای آگاهی از
+            ساختار این فایل به فایل پیش‌فرض مراجعه کنید.
+        joined_verb_parts: اگر `True` باشد افعال چندبخشی را با کاراکتر زیرخط به هم می‌چسباند.
+
+    """
+
+    def __init__(
+        self: "Lemmatizer",
+        words_file: str = default_words,
+        verbs_file: str = default_verbs,
+        joined_verb_parts: bool = True,
+    ) -> None:
+        self.words_file = words_file
+        self.verbs = {}
+        self.stemmer = Stemmer()
+        self.conjugation = Conjugation()
+
+        tokenizer = WordTokenizer(words_file=default_words, verbs_file=verbs_file)
+        self.words = tokenizer.words
+
+        if verbs_file:
+            self.verbs["است"] = "#است"
+            for verb in tokenizer.verbs:
+                for tense in self.conjugation.get_all(verb):
+                    self.verbs[tense] = verb
+            if joined_verb_parts:
+                for verb in tokenizer.verbs:
+                    bon = verb.split("#")[0]
+                    for after_verb in tokenizer.after_verbs:
+                        self.verbs[bon + "ه_" + after_verb] = verb
+                        self.verbs["ن" + bon + "ه_" + after_verb] = verb
+                    for before_verb in tokenizer.before_verbs:
+                        self.verbs[before_verb + "_" + bon] = verb
+
+    def lemmatize(self: "Lemmatizer", word: str, pos: str = "") -> str:
+        """ریشهٔ کلمه را پیدا می‌کند.
+
+        پارامتر `pos` نوع کلمه است: (اسم، فعل، صفت و ...) و به این خاطر لازم
+        است که می‌تواند روی ریشه‌یابی کلمات اثر بگذارد؛ مثلاً واژهٔ «اجتماعی» در
+        جایگاه صفت (او یک فرد اجتماعی است)، ریشه‌اش همان «اجتماعی» می‌شود ولی
+        همین واژه در جایگاه اسم (اجتماعی از مردم)، ریشه‌اش می‌شود «اجتماع».
+
+        Examples:
+            >>> lemmatizer = Lemmatizer()
+            >>> lemmatizer.lemmatize('کتاب‌ها')
+            'کتاب'
+            >>> lemmatizer.lemmatize('آتشفشان')
+            'آتشفشان'
+            >>> lemmatizer.lemmatize('می‌روم')
+            'رفت#رو'
+            >>> lemmatizer.lemmatize('گفته_شده_است')
+            'گفت#گو'
+            >>> lemmatizer.lemmatize('نچشیده_است')
+            'چشید#چش'
+            >>> lemmatizer.lemmatize('مردم', pos='N')
+            'مردم'
+            >>> lemmatizer.lemmatize('اجتماعی', pos='AJ')
+            'اجتماعی'
+
+        Args:
+            word: کلمه‌ای که باید پردازش شود.
+            pos: نوع کلمه. این پارامتر سه مقدار `V` (فعل) و `AJ` (صفت) و `PRO` (ضمیر) را می‌پذیرد.
+
+        Returns:
+            ریشهٔ کلمه
+
+        """
+        if not pos and word in self.words:
+            return word
+
+        if (not pos or pos == "V") and word in self.verbs:
+            return self.verbs[word]
+
+        if pos.startswith("AJ") and word[-1] == "ی":
+            return word
+
+        if pos == "PRO":
+            return word
+
+        if word in self.words:
+            return word
+
+        stem = self.stemmer.stem(word)
+        if stem and stem in self.words:
+            return stem
+
+        return word
+
+
+class Conjugation:
+    """این کلاس دارای توابعی برای صرف‌کردن افعال است."""
+
+    def perfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ مطلق صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.perfective_past('دید')
+            ['دیدم', 'دیدی', 'دید', 'دیدیم', 'دیدید', 'دیدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+            صورت‌های صرفی فعل در زمان گذشتهٔ مطلق.
+        """
+        return [ri + x for x in ["م", "ی", "", "یم", "ید", "ند"]]
+
+    def negative_perfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ مطلق به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_perfective_past('دید')
+            ['ندیدم', 'ندیدی', 'ندید', 'ندیدیم', 'ندیدید', 'ندیدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.perfective_past(ri)]
+
+    def passive_perfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ مطلق در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_perfective_past('دید')
+            ['دیده شدم', 'دیده شدی', 'دیده شد', 'دیده شدیم', 'دیده شدید', 'دیده شدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.perfective_past("شد")]
+
+    def negative_passive_perfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_perfective_past('دید')
+            ['دیده نشدم', 'دیده نشدی', 'دیده نشد', 'دیده نشدیم', 'دیده نشدید', 'دیده نشدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ مطلق در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_perfective_past("شد")]
+
+    def imperfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_past('دید')
+            ['می‌دیدم', 'می‌دیدی', 'می‌دید', 'می‌دیدیم', 'می‌دیدید', 'می‌دیدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پایا.
+        """
+        return ["می‌" + x for x in self.perfective_past(ri)]
+
+    def negative_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_past('دید')
+            ['نمی‌دیدم', 'نمی‌دیدی', 'نمی‌دید', 'نمی‌دیدیم', 'نمی‌دیدید', 'نمی‌دیدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_past(ri)]
+
+    def passive_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_past('دید')
+            ['دیده می‌شدم', 'دیده می‌شدی', 'دیده می‌شد', 'دیده می‌شدیم', 'دیده می‌شدید', 'دیده می‌شدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_past("شد")]
+
+    def negative_passive_imperfective_past(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_past('دید')
+            ['دیده نمی‌شدم', 'دیده نمی‌شدی', 'دیده نمی‌شد', 'دیده نمی‌شدیم', 'دیده نمی‌شدید', 'دیده نمی‌شدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_imperfective_past("شد")]
+
+    def past_progresive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ استمراری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.past_progresive('دید')
+            ['داشتم می‌دیدم', 'داشتی می‌دیدی', 'داشت می‌دید', 'داشتیم می‌دیدیم', 'داشتید می‌دیدید', 'داشتند می‌دیدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ استمراری.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(self.perfective_past("داشت"), self.imperfective_past(ri))
+        ]
+
+    def passive_past_progresive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ استمراری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_past_progresive('دید')
+            ['داشتم دیده می‌شدم', 'داشتی دیده می‌شدی', 'داشت دیده می‌شد', 'داشتیم دیده می‌شدیم', 'داشتید دیده می‌شدید', 'داشتند دیده می‌شدند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ استمراری در حالت مجهول.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.perfective_past("داشت"),
+                self.passive_imperfective_past(ri),
+            )
+        ]
+
+    def present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.present_perfect('دید')
+            ['دیده‌ام', 'دیده‌ای', 'دیده است', 'دیده', 'دیده‌ایم', 'دیده‌اید', 'دیده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل.
+        """
+        return [ri + x for x in ["ه‌ام", "ه‌ای", "ه است", "ه", "ه‌ایم", "ه‌اید", "ه‌اند"]]
+
+    def negative_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_present_perfect('دید')
+            ['ندیده‌ام', 'ندیده‌ای', 'ندیده است', 'ندیده', 'ندیده‌ایم', 'ندیده‌اید', 'ندیده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.present_perfect(ri)]
+
+    def subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه التزامی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.subjunctive_present_perfect('دید')
+            ['دیده باشم', 'دیده باشی', 'دیده باشد', 'دیده باشیم', 'دیده باشید', 'دیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی.
+        """
+        return [ri + "ه " + x for x in self.perfective_present("باش")]
+
+    def negative_subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه التزامی به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_subjunctive_present_perfect('دید')
+            ['ندیده باشم', 'ندیده باشی', 'ندیده باشد', 'ندیده باشیم', 'ندیده باشید', 'ندیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.subjunctive_present_perfect(ri)]
+
+    def grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه دستوری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.grammatical_present_perfect('دید')
+            ['دیده باشم', 'دیده باش', 'دیده باشد', 'دیده باشیم', 'دیده باشید', 'دیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری.
+        """
+        return [
+            ri + "ه " + ("باش" if x == "باشی" else x)
+            for x in self.perfective_present("باش")
+        ]
+
+    def negative_grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه دستوری به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_grammatical_present_perfect('دید')
+            ['ندیده باشم', 'ندیده باش', 'ندیده باشد', 'ندیده باشیم', 'ندیده باشید', 'ندیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری به‌شکل منفی.
+        """
+        return [
+            "ن" + ri + "ه " + ("باش" if x == "باشی" else x)
+            for x in self.perfective_present("باش")
+        ]
+
+    def passive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_present_perfect('دید')
+            ['دیده شده‌ام', 'دیده شده‌ای', 'دیده شده است', 'دیده شده', 'دیده شده‌ایم', 'دیده شده‌اید', 'دیده شده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.present_perfect("شد")]
+
+    def negative_passive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_present_perfect('دید')
+            ['دیده نشده‌ام', 'دیده نشده‌ای', 'دیده نشده است', 'دیده نشده', 'دیده نشده‌ایم', 'دیده نشده‌اید', 'دیده نشده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_present_perfect("شد")]
+
+    def passive_subjunctive_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه التزامی در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_subjunctive_present_perfect('دید')
+            ['دیده شده باشم', 'دیده شده باشی', 'دیده شده باشد', 'دیده شده باشیم', 'دیده شده باشید', 'دیده شده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.subjunctive_present_perfect("شد")]
+
+    def negative_passive_subjunctive_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_subjunctive_present_perfect('دید')
+            ['دیده نشده باشم', 'دیده نشده باشی', 'دیده نشده باشد', 'دیده نشده باشیم', 'دیده نشده باشید', 'دیده نشده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه التزامی در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_subjunctive_present_perfect("شد")]
+
+    def passive_grammatical_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل در وجه دستوری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_grammatical_present_perfect('دید')
+            ['دیده شده باشم', 'دیده شده باش', 'دیده شده باشد', 'دیده شده باشیم', 'دیده شده باشید', 'دیده شده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری در حالت مجهول.
+        """
+        return [
+            ri + "ه شده " + ("باش" if x == "باشی" else x)
+            for x in self.perfective_present("باش")
+        ]
+
+    def negative_passive_grammatical_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_grammatical_present_perfect('دید')
+            ['دیده نشده باشم', 'دیده نشده باش', 'دیده نشده باشد', 'دیده نشده باشیم', 'دیده نشده باشید', 'دیده نشده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل در وجه دستوری در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه نشده " + ("باش" if x == "باشی" else x)
+            for x in self.perfective_present("باش")
+        ]
+
+    def imperfective_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_present_perfect('دید')
+            ['می‌دیده‌ام', 'می‌دیده‌ای', 'می‌دیده است', 'می‌دیده', 'می‌دیده‌ایم', 'می‌دیده‌اید', 'می‌دیده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا.
+        """
+        return ["می‌" + x for x in self.present_perfect(ri)]
+
+    def negative_imperfective_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_present_perfect('دید')
+            ['نمی‌دیده‌ام', 'نمی‌دیده‌ای', 'نمی‌دیده است', 'نمی‌دیده', 'نمی‌دیده‌ایم', 'نمی‌دیده‌اید', 'نمی‌دیده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_present_perfect(ri)]
+
+    def subjunctive_imperfective_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا در وجه التزامی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.subjunctive_imperfective_present_perfect('دید')
+            ['می‌دیده باشم', 'می‌دیده باشی', 'می‌دیده باشد', 'می‌دیده باشیم', 'می‌دیده باشید', 'می‌دیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی.
+        """
+        return ["می‌" + x for x in self.subjunctive_present_perfect(ri)]
+
+    def negative_subjunctive_imperfective_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا در وجه التزامی به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_subjunctive_imperfective_present_perfect('دید')
+            ['نمی‌دیده باشم', 'نمی‌دیده باشی', 'نمی‌دیده باشد', 'نمی‌دیده باشیم', 'نمی‌دیده باشید', 'نمی‌دیده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.subjunctive_imperfective_present_perfect(ri)]
+
+    def passive_imperfective_present_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_present_perfect('دید')
+            ['دیده می‌شده‌ام', 'دیده می‌شده‌ای', 'دیده می‌شده است', 'دیده می‌شده', 'دیده می‌شده‌ایم', 'دیده می‌شده‌اید', 'دیده می‌شده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_present_perfect("شد")]
+
+    def negative_passive_imperfective_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_present_perfect('دید')
+            ['دیده نمی‌شده‌ام', 'دیده نمی‌شده‌ای', 'دیده نمی‌شده است', 'دیده نمی‌شده', 'دیده نمی‌شده‌ایم', 'دیده نمی‌شده‌اید', 'دیده نمی‌شده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_imperfective_present_perfect("شد")]
+
+    def passive_subjunctive_imperfective_present_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا در وجه التزامی در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_subjunctive_imperfective_present_perfect('دید')
+            ['دیده می‌شده باشم', 'دیده می‌شده باشی', 'دیده می‌شده باشد', 'دیده می‌شده باشیم', 'دیده می‌شده باشید', 'دیده می‌شده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی در حالت مجهول.
+        """
+        return [
+            ri + "ه " + x for x in self.subjunctive_imperfective_present_perfect("شد")
+        ]
+
+    def negative_passive_subjunctive_imperfective_present_perfect(
+        self: "Conjugation",
+        ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_subjunctive_imperfective_present_perfect('دید')
+            ['دیده نمی‌شده باشم', 'دیده نمی‌شده باشی', 'دیده نمی‌شده باشد', 'دیده نمی‌شده باشیم', 'دیده نمی‌شده باشید', 'دیده نمی‌شده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + x
+            for x in self.negative_subjunctive_imperfective_present_perfect("شد")
+        ]
+
+    def present_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل استمراری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.present_perfect_progressive('دید')
+            ['داشته‌ام می‌دیده‌ام', 'داشته‌ای می‌دیده‌ای', 'داشته است می‌دیده است', 'داشته می‌دیده', 'داشته‌ایم می‌دیده‌ایم', 'داشته‌اید می‌دیده‌اید', 'داشته‌اند می‌دیده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل استمراری.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.present_perfect("داشت"),
+                self.imperfective_present_perfect(ri),
+            )
+        ]
+
+    def passive_present_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال کامل استمراری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_present_perfect_progressive('دید')
+            ['داشته‌ام دیده می‌شده‌ام', 'داشته‌ای دیده می‌شده‌ای', 'داشته است دیده می‌شده است', 'داشته دیده می‌شده', 'داشته‌ایم دیده می‌شده‌ایم', 'داشته‌اید دیده می‌شده‌اید', 'داشته‌اند دیده می‌شده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال کامل استمراری در حالت مجهول.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.present_perfect("داشت"),
+                self.passive_imperfective_present_perfect(ri),
+            )
+        ]
+
+    def past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.past_precedent('دید')
+            ['دیده بودم', 'دیده بودی', 'دیده بود', 'دیده بودیم', 'دیده بودید', 'دیده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین.
+        """
+        return [ri + "ه " + x for x in self.perfective_past("بود")]
+
+    def negative_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_past_precedent('دید')
+            ['ندیده بودم', 'ندیده بودی', 'ندیده بود', 'ندیده بودیم', 'ندیده بودید', 'ندیده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.past_precedent(ri)]
+
+    def passive_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_past_precedent('دید')
+            ['دیده شده بودم', 'دیده شده بودی', 'دیده شده بود', 'دیده شده بودیم', 'دیده شده بودید', 'دیده شده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.past_precedent("شد")]
+
+    def negative_passive_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_past_precedent('دید')
+            ['دیده نشده بودم', 'دیده نشده بودی', 'دیده نشده بود', 'دیده نشده بودیم', 'دیده نشده بودید', 'دیده نشده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_past_precedent("شد")]
+
+    def imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_past_precedent('دید')
+            ['می‌دیده بودم', 'می‌دیده بودی', 'می‌دیده بود', 'می‌دیده بودیم', 'می‌دیده بودید', 'می‌دیده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا.
+        """
+        return ["می‌" + x for x in self.past_precedent(ri)]
+
+    def negative_imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_past_precedent('دید')
+            ['نمی‌دیده بودم', 'نمی‌دیده بودی', 'نمی‌دیده بود', 'نمی‌دیده بودیم', 'نمی‌دیده بودید', 'نمی‌دیده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_past_precedent(ri)]
+
+    def passive_imperfective_past_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_past_precedent('دید')
+            ['دیده می‌شده بودم', 'دیده می‌شده بودی', 'دیده می‌شده بود', 'دیده می‌شده بودیم', 'دیده می‌شده بودید', 'دیده می‌شده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_past_precedent("شد")]
+
+    def negative_passive_imperfective_past_precedent(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_past_precedent('دید')
+            ['دیده نمی‌شده بودم', 'دیده نمی‌شده بودی', 'دیده نمی‌شده بود', 'دیده نمی‌شده بودیم', 'دیده نمی‌شده بودید', 'دیده نمی‌شده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_imperfective_past_precedent("شد")]
+
+    def past_precedent_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین استمراری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.past_precedent_progressive('دید')
+            ['داشتم می‌دیده بودم', 'داشتی می‌دیده بودی', 'داشت می‌دیده بود', 'داشتیم می‌دیده بودیم', 'داشتید می‌دیده بودید', 'داشتند می‌دیده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین استمراری.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.perfective_past("داشت"),
+                self.imperfective_past_precedent(ri),
+            )
+        ]
+
+    def passive_past_precedent_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین استمراری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_past_precedent_progressive('دید')
+            ['داشتم دیده می‌شده بودم', 'داشتی دیده می‌شده بودی', 'داشت دیده می‌شده بود', 'داشتیم دیده می‌شده بودیم', 'داشتید دیده می‌شده بودید', 'داشتند دیده می‌شده بودند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین استمراری در حالت مجهول.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.perfective_past("داشت"),
+                self.passive_imperfective_past_precedent(ri),
+            )
+        ]
+
+    def past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.past_precedent_perfect('دید')
+            ['دیده بوده‌ام', 'دیده بوده‌ای', 'دیده بوده است', 'دیده بوده', 'دیده بوده‌ایم', 'دیده بوده‌اید', 'دیده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل.
+        """
+        return [ri + "ه " + x for x in self.present_perfect("بود")]
+
+    def negative_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_past_precedent_perfect('دید')
+            ['ندیده بوده‌ام', 'ندیده بوده‌ای', 'ندیده بوده است', 'ندیده بوده', 'ندیده بوده‌ایم', 'ندیده بوده‌اید', 'ندیده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.past_precedent_perfect(ri)]
+
+    def subjunctive_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.subjunctive_past_precedent_perfect('دید')
+            ['دیده بوده باشم', 'دیده بوده باشی', 'دیده بوده باشد', 'دیده بوده باشیم', 'دیده بوده باشید', 'دیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی.
+        """
+        return [ri + "ه " + x for x in self.subjunctive_present_perfect("بود")]
+
+    def negative_subjunctive_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_subjunctive_past_precedent_perfect('دید')
+            ['ندیده بوده باشم', 'ندیده بوده باشی', 'ندیده بوده باشد', 'ندیده بوده باشیم', 'ندیده بوده باشید', 'ندیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.subjunctive_past_precedent_perfect(ri)]
+
+    def grammatical_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.grammatical_past_precedent_perfect('دید')
+            ['دیده بوده باشم', 'دیده بوده باش', 'دیده بوده باشد', 'دیده بوده باشیم', 'دیده بوده باشید', 'دیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری.
+        """
+        return [
+            ri + "ه بوده " + ("باش" if x == "باشی" else x)
+            for x in self.perfective_present("باش")
+        ]
+
+    def negative_grammatical_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_grammatical_past_precedent_perfect('دید')
+            ['ندیده بوده باشم', 'ندیده بوده باش', 'ندیده بوده باشد', 'ندیده بوده باشیم', 'ندیده بوده باشید', 'ندیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.grammatical_past_precedent_perfect(ri)]
+
+    def passive_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_past_precedent_perfect('دید')
+            ['دیده شده بوده‌ام', 'دیده شده بوده‌ای', 'دیده شده بوده است', 'دیده شده بوده', 'دیده شده بوده‌ایم', 'دیده شده بوده‌اید', 'دیده شده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.past_precedent_perfect("شد")]
+
+    def negative_passive_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_past_precedent_perfect('دید')
+            ['دیده نشده بوده‌ام', 'دیده نشده بوده‌ای', 'دیده نشده بوده است', 'دیده نشده بوده', 'دیده نشده بوده‌ایم', 'دیده نشده بوده‌اید', 'دیده نشده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_past_precedent_perfect("شد")]
+
+    def passive_subjunctive_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_subjunctive_past_precedent_perfect('دید')
+            ['دیده شده بوده باشم', 'دیده شده بوده باشی', 'دیده شده بوده باشد', 'دیده شده بوده باشیم', 'دیده شده بوده باشید', 'دیده شده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.subjunctive_past_precedent_perfect("شد")]
+
+    def negative_passive_subjunctive_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_subjunctive_past_precedent_perfect('دید')
+            ['دیده نشده بوده باشم', 'دیده نشده بوده باشی', 'دیده نشده بوده باشد', 'دیده نشده بوده باشیم', 'دیده نشده بوده باشید', 'دیده نشده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه التزامی در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + "ن" + x for x in self.subjunctive_past_precedent_perfect("شد")
+        ]
+
+    def passive_grammatical_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_grammatical_past_precedent_perfect('دید')
+            ['دیده شده بوده باشم', 'دیده شده بوده باش', 'دیده شده بوده باشد', 'دیده شده بوده باشیم', 'دیده شده بوده باشید', 'دیده شده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.grammatical_past_precedent_perfect("شد")]
+
+    def negative_passive_grammatical_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_grammatical_past_precedent_perfect('دید')
+            ['دیده نشده بوده باشم', 'دیده نشده بوده باش', 'دیده نشده بوده باشد', 'دیده نشده بوده باشیم', 'دیده نشده بوده باشید', 'دیده نشده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل در وجه دستوری در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + x
+            for x in self.negative_grammatical_past_precedent_perfect("شد")
+        ]
+
+    def imperfective_past_precedent_perfect(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_past_precedent_perfect('دید')
+            ['می‌دیده بوده‌ام', 'می‌دیده بوده‌ای', 'می‌دیده بوده است', 'می‌دیده بوده', 'می‌دیده بوده‌ایم', 'می‌دیده بوده‌اید', 'می‌دیده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا.
+        """
+        return ["می‌" + x for x in self.past_precedent_perfect(ri)]
+
+    def negative_imperfective_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_past_precedent_perfect('دید')
+            ['نمی‌دیده بوده‌ام', 'نمی‌دیده بوده‌ای', 'نمی‌دیده بوده است', 'نمی‌دیده بوده', 'نمی‌دیده بوده‌ایم', 'نمی‌دیده بوده‌اید', 'نمی‌دیده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_past_precedent_perfect(ri)]
+
+    def subjunctive_imperfective_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.subjunctive_imperfective_past_precedent_perfect('دید')
+            ['می‌دیده بوده باشم', 'می‌دیده بوده باشی', 'می‌دیده بوده باشد', 'می‌دیده بوده باشیم', 'می‌دیده بوده باشید', 'می‌دیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی.
+        """
+        return ["می‌" + x for x in self.subjunctive_past_precedent_perfect(ri)]
+
+    def negative_subjunctive_imperfective_past_precedent_perfect(
+        self: "Conjugation",
+        ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_subjunctive_imperfective_past_precedent_perfect('دید')
+            ['نمی‌دیده بوده باشم', 'نمی‌دیده بوده باشی', 'نمی‌دیده بوده باشد', 'نمی‌دیده بوده باشیم', 'نمی‌دیده بوده باشید', 'نمی‌دیده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی به‌شکل منفی.
+        """
+        return [
+            "ن" + x for x in self.subjunctive_imperfective_past_precedent_perfect(ri)
+        ]
+
+    def passive_imperfective_past_precedent_perfect(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_past_precedent_perfect('دید')
+            ['دیده می‌شده بوده‌ام', 'دیده می‌شده بوده‌ای', 'دیده می‌شده بوده است', 'دیده می‌شده بوده', 'دیده می‌شده بوده‌ایم', 'دیده می‌شده بوده‌اید', 'دیده می‌شده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_past_precedent_perfect("شد")]
+
+    def negative_passive_imperfective_past_precedent_perfect(
+        self: "Conjugation",
+        ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_past_precedent_perfect('دید')
+            ['دیده نمی‌شده بوده‌ام', 'دیده نمی‌شده بوده‌ای', 'دیده نمی‌شده بوده است', 'دیده نمی‌شده بوده', 'دیده نمی‌شده بوده‌ایم', 'دیده نمی‌شده بوده‌اید', 'دیده نمی‌شده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + x
+            for x in self.negative_imperfective_past_precedent_perfect("شد")
+        ]
+
+    def passive_subjunctive_imperfective_past_precedent_perfect(
+        self: "Conjugation",
+        ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_subjunctive_imperfective_past_precedent_perfect('دید')
+            ['دیده می‌شده بوده باشم', 'دیده می‌شده بوده باشی', 'دیده می‌شده بوده باشد', 'دیده می‌شده بوده باشیم', 'دیده می‌شده بوده باشید', 'دیده می‌شده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول.
+        """
+        return [
+            ri + "ه " + x
+            for x in self.subjunctive_imperfective_past_precedent_perfect("شد")
+        ]
+
+    def negative_passive_subjunctive_imperfective_past_precedent_perfect(
+        self: "Conjugation",
+        ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_subjunctive_imperfective_past_precedent_perfect('دید')
+            ['دیده نمی‌شده بوده باشم', 'دیده نمی‌شده بوده باشی', 'دیده نمی‌شده بوده باشد', 'دیده نمی‌شده بوده باشیم', 'دیده نمی‌شده بوده باشید', 'دیده نمی‌شده بوده باشند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل پایا در وجه التزامی در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + "ن" + x
+            for x in self.subjunctive_imperfective_past_precedent_perfect("شد")
+        ]
+
+    def past_precedent_perfect_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل استمراری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.past_precedent_perfect_progressive('دید')
+            ['داشته‌ام می‌دیده بوده‌ام', 'داشته‌ای می‌دیده بوده‌ای', 'داشته است می‌دیده بوده است', 'داشته می‌دیده بوده', 'داشته‌ایم می‌دیده بوده‌ایم', 'داشته‌اید می‌دیده بوده‌اید', 'داشته‌اند می‌دیده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل استمراری.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.present_perfect("داشت"),
+                self.imperfective_past_precedent_perfect(ri),
+            )
+        ]
+
+    def passive_past_precedent_perfect_progressive(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان گذشتهٔ پیشین کامل استمراری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_past_precedent_perfect_progressive('دید')
+            ['داشته‌ام دیده می‌شده بوده‌ام', 'داشته‌ای دیده می‌شده بوده‌ای', 'داشته است دیده می‌شده بوده است', 'داشته دیده می‌شده بوده', 'داشته‌ایم دیده می‌شده بوده‌ایم', 'داشته‌اید دیده می‌شده بوده‌اید', 'داشته‌اند دیده می‌شده بوده‌اند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان گذشتهٔ پیشین کامل استمراری در حالت مجهول.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.present_perfect("داشت"),
+                self.passive_imperfective_past_precedent_perfect(ri),
+            )
+        ]
+
+    def perfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال مطلق صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.perfective_present('بین')
+            ['بینم', 'بینی', 'بیند', 'بینیم', 'بینید', 'بینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق.
+        """
+        return [rii + x for x in ["م", "ی", "د", "یم", "ید", "ند"]]
+
+    def negative_perfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال مطلق به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_perfective_present('بین')
+            ['نبینم', 'نبینی', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.perfective_present(rii)]
+
+    def subjunctive_perfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه التزامی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.subjunctive_perfective_present('بین')
+            ['ببینم', 'ببینی', 'ببیند', 'ببینیم', 'ببینید', 'ببینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی.
+        """
+        return ["ب" + x for x in self.perfective_present(rii)]
+
+    def negative_subjunctive_perfective_present(
+        self: "Conjugation", rii: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه التزامی به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_subjunctive_perfective_present('بین')
+            ['نبینم', 'نبینی', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.perfective_present(rii)]
+
+    def grammatical_perfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه دستوری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.grammatical_perfective_present('بین')
+            ['ببینم', 'ببین', 'ببیند', 'ببینیم', 'ببینید', 'ببینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری.
+        """
+        return [
+            "ببین" if x == "ببینی" else x
+            for x in self.subjunctive_perfective_present(rii)
+        ]
+
+    def negative_grammatical_perfective_present(
+        self: "Conjugation", rii: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه دستوری به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_grammatical_perfective_present('بین')
+            ['نبینم', 'نبین', 'نبیند', 'نبینیم', 'نبینید', 'نبینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری به‌شکل منفی.
+        """
+        return [
+            "ن" + ("بین" if x == "بینی" else x) for x in self.perfective_present(rii)
+        ]
+
+    def passive_perfective_present(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال مطلق در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_perfective_present('دید')
+            ['دیده شوم', 'دیده شوی', 'دیده شود', 'دیده شویم', 'دیده شوید', 'دیده شوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.perfective_present("شو")]
+
+    def negative_passive_perfective_present(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_perfective_present('دید')
+            ['دیده نشوم', 'دیده نشوی', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_perfective_present("شو")]
+
+    def passive_subjunctive_perfective_present(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه التزامی در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_subjunctive_perfective_present('دید')
+            ['دیده بشوم', 'دیده بشوی', 'دیده بشود', 'دیده بشویم', 'دیده بشوید', 'دیده بشوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.subjunctive_perfective_present("شو")]
+
+    def negative_passive_subjunctive_perfective_present(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه التزامی در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_subjunctive_perfective_present('دید')
+            ['دیده نشوم', 'دیده نشوی', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه التزامی در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + x for x in self.negative_subjunctive_perfective_present("شو")
+        ]
+
+    def passive_grammatical_perfective_present(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه دستوری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_grammatical_perfective_present('دید')
+            ['دیده بشوم', 'دیده بشو', 'دیده بشود', 'دیده بشویم', 'دیده بشوید', 'دیده بشوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری در حالت مجهول.
+        """
+        return [
+            ri + "ه " + ("بشو" if x == "بشوی" else x)
+            for x in self.grammatical_perfective_present("شو")
+        ]
+
+    def negative_passive_grammatical_perfective_present(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال مطلق در وجه دستوری در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_grammatical_perfective_present('دید')
+            ['دیده نشوم', 'دیده نشو', 'دیده نشود', 'دیده نشویم', 'دیده نشوید', 'دیده نشوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال مطلق در وجه دستوری در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + ("نشو" if x == "نشوی" else x)
+            for x in self.negative_grammatical_perfective_present("شو")
+        ]
+
+    def imperfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_present('بین')
+            ['می‌بینم', 'می‌بینی', 'می‌بیند', 'می‌بینیم', 'می‌بینید', 'می‌بینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال پایا.
+        """
+        return ["می‌" + x for x in self.perfective_present(rii)]
+
+    def negative_imperfective_present(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_present('بین')
+            ['نمی‌بینم', 'نمی‌بینی', 'نمی‌بیند', 'نمی‌بینیم', 'نمی‌بینید', 'نمی‌بینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_present(rii)]
+
+    def passive_imperfective_present(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_present('دید')
+            ['دیده می‌شوم', 'دیده می‌شوی', 'دیده می‌شود', 'دیده می‌شویم', 'دیده می‌شوید', 'دیده می‌شوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_present("شو")]
+
+    def negative_passive_imperfective_present(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان حال پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_present('دید')
+            ['دیده نمی‌شوم', 'دیده نمی‌شوی', 'دیده نمی‌شود', 'دیده نمی‌شویم', 'دیده نمی‌شوید', 'دیده نمی‌شوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_imperfective_present("شو")]
+
+    def present_progressive(self: "Conjugation", rii: str) -> List[str]:
+        """فعل را در زمان حال استمراری صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.present_progressive('بین')
+            ['دارم می‌بینم', 'داری می‌بینی', 'دارد می‌بیند', 'داریم می‌بینیم', 'دارید می‌بینید', 'دارند می‌بینند']
+
+        Args:
+            rii: بن مضارع فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال استمراری.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.perfective_present("دار"),
+                self.imperfective_present(rii),
+            )
+        ]
+
+    def passive_present_progressive(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان حال استمراری در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_present_progressive('دید')
+            ['دارم دیده می‌شوم', 'داری دیده می‌شوی', 'دارد دیده می‌شود', 'داریم دیده می‌شویم', 'دارید دیده می‌شوید', 'دارند دیده می‌شوند']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان حال استمراری در حالت مجهول.
+        """
+        return [
+            x + " " + y
+            for x, y in zip(
+                self.perfective_present("دار"),
+                self.passive_imperfective_present(ri),
+            )
+        ]
+
+    def perfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ مطلق صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.perfective_future('دید')
+            ['خواهم دید', 'خواهی دید', 'خواهد دید', 'خواهیم دید', 'خواهید دید', 'خواهند دید']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ مطلق.
+        """
+        return [x + " " + ri for x in self.perfective_present("خواه")]
+
+    def negative_perfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ مطلق به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_perfective_future('دید')
+            ['نخواهم دید', 'نخواهی دید', 'نخواهد دید', 'نخواهیم دید', 'نخواهید دید', 'نخواهند دید']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ مطلق به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.perfective_future(ri)]
+
+    def passive_perfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ مطلق در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_perfective_future('دید')
+            ['دیده خواهم شد', 'دیده خواهی شد', 'دیده خواهد شد', 'دیده خواهیم شد', 'دیده خواهید شد', 'دیده خواهند شد']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ مطلق در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.perfective_future("شد")]
+
+    def negative_passive_perfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ مطلق در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_perfective_future('دید')
+            ['دیده نخواهم شد', 'دیده نخواهی شد', 'دیده نخواهد شد', 'دیده نخواهیم شد', 'دیده نخواهید شد', 'دیده نخواهند شد']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ مطلق در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_perfective_future("شد")]
+
+    def imperfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.imperfective_future('دید')
+            ['می‌خواهم دید', 'می‌خواهی دید', 'می‌خواهد دید', 'می‌خواهیم دید', 'می‌خواهید دید', 'می‌خواهند دید']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پایا.
+        """
+        return ["می‌" + x for x in self.perfective_future(ri)]
+
+    def negative_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_imperfective_future('دید')
+            ['نمی‌خواهم دید', 'نمی‌خواهی دید', 'نمی‌خواهد دید', 'نمی‌خواهیم دید', 'نمی‌خواهید دید', 'نمی‌خواهند دید']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.imperfective_future(ri)]
+
+    def passive_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_imperfective_future('دید')
+            ['دیده می‌خواهم شد', 'دیده می‌خواهی شد', 'دیده می‌خواهد شد', 'دیده می‌خواهیم شد', 'دیده می‌خواهید شد', 'دیده می‌خواهند شد']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.imperfective_future("شد")]
+
+    def negative_passive_imperfective_future(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_imperfective_future('دید')
+            ['دیده نمی‌خواهم شد', 'دیده نمی‌خواهی شد', 'دیده نمی‌خواهد شد', 'دیده نمی‌خواهیم شد', 'دیده نمی‌خواهید شد', 'دیده نمی‌خواهند شد']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_imperfective_future("شد")]
+
+    def future_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.future_precedent('دید')
+            ['دیده خواهم بود', 'دیده خواهی بود', 'دیده خواهد بود', 'دیده خواهیم بود', 'دیده خواهید بود', 'دیده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین.
+        """
+        return [ri + "ه " + x for x in self.perfective_future("بود")]
+
+    def negative_future_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_future_precedent('دید')
+            ['ندیده خواهم بود', 'ندیده خواهی بود', 'ندیده خواهد بود', 'ندیده خواهیم بود', 'ندیده خواهید بود', 'ندیده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.future_precedent(ri)]
+
+    def passive_future_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_future_precedent('دید')
+            ['دیده شده خواهم بود', 'دیده شده خواهی بود', 'دیده شده خواهد بود', 'دیده شده خواهیم بود', 'دیده شده خواهید بود', 'دیده شده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.future_precedent("شد")]
+
+    def negative_passive_future_precedent(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_future_precedent('دید')
+            ['دیده نشده خواهم بود', 'دیده نشده خواهی بود', 'دیده نشده خواهد بود', 'دیده نشده خواهیم بود', 'دیده نشده خواهید بود', 'دیده نشده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین در حالت مجهول به‌شکل منفی.
+        """
+        return [ri + "ه " + x for x in self.negative_future_precedent("شد")]
+
+    def future_precedent_imperfective(self: "Conjugation", ri: str) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین پایا صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.future_precedent_imperfective('دید')
+            ['می‌دیده خواهم بود', 'می‌دیده خواهی بود', 'می‌دیده خواهد بود', 'می‌دیده خواهیم بود', 'می‌دیده خواهید بود', 'می‌دیده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا.
+        """
+        return ["می‌" + x for x in self.future_precedent(ri)]
+
+    def negative_future_precedent_imperfective(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین پایا به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_future_precedent_imperfective('دید')
+            ['نمی‌دیده خواهم بود', 'نمی‌دیده خواهی بود', 'نمی‌دیده خواهد بود', 'نمی‌دیده خواهیم بود', 'نمی‌دیده خواهید بود', 'نمی‌دیده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا به‌شکل منفی.
+        """
+        return ["ن" + x for x in self.future_precedent_imperfective(ri)]
+
+    def passive_future_precedent_imperfective(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین پایا در حالت مجهول صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.passive_future_precedent_imperfective('دید')
+            ['دیده می‌شده خواهم بود', 'دیده می‌شده خواهی بود', 'دیده می‌شده خواهد بود', 'دیده می‌شده خواهیم بود', 'دیده می‌شده خواهید بود', 'دیده می‌شده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا در حالت مجهول.
+        """
+        return [ri + "ه " + x for x in self.future_precedent_imperfective("شد")]
+
+    def negative_passive_future_precedent_imperfective(
+        self: "Conjugation", ri: str,
+    ) -> List[str]:
+        """فعل را در زمان آیندهٔ پیشین پایا در حالت مجهول به‌شکل منفی صرف می‌کند.
+
+        Examples:
+            >>> conj = Conjugation()
+            >>> conj.negative_passive_future_precedent_imperfective('دید')
+            ['دیده نمی‌شده خواهم بود', 'دیده نمی‌شده خواهی بود', 'دیده نمی‌شده خواهد بود', 'دیده نمی‌شده خواهیم بود', 'دیده نمی‌شده خواهید بود', 'دیده نمی‌شده خواهند بود']
+
+        Args:
+            ri: بن ماضی فعل.
+
+        Returns:
+             صورت‌های صرفی فعل در زمان آیندهٔ پیشین پایا در حالت مجهول به‌شکل منفی.
+        """
+        return [
+            ri + "ه " + x for x in self.negative_future_precedent_imperfective("شد")
+        ]
+
+    def get(self: "Conjugation", verb, negative=False, passive=False) -> List[str]:
+        """صورت‌های صرفی فعل را برمی‌گرداند.
+
+        Args:
+            verb (str): فعلی که باید صرف شود. به‌صورت بن ماضی#بن مضارع؛ مانند: دید#بین.
+            negative (bool, optional): اگر `True` باشد صورت‌های صرفی منفی را برمی‌گرداند.
+            passive (bool, optional): اگر `True` باشد صورت‌های صرفی مجهول را برمی‌گرداند.
+
+        Returns:
+            (List(str)): صورت‌های صرفی فعل.
+        """
+        ri, rii = verb.split("#")
+        infinitive = [ri + "ن"]
+        result = [infinitive]
+
+        if negative and passive:
+            result.append(self.negative_passive_perfective_past(ri))
+            result.append(self.negative_passive_imperfective_past(ri))
+            result.append(self.negative_passive_present_perfect(ri))
+            result.append(self.negative_passive_subjunctive_present_perfect(ri))
+            result.append(self.negative_passive_grammatical_present_perfect(ri))
+            result.append(self.negative_passive_imperfective_present_perfect(ri))
+            result.append(
+                self.negative_passive_subjunctive_imperfective_present_perfect(ri),
+            )
+            result.append(self.negative_passive_past_precedent(ri))
+            result.append(self.negative_passive_imperfective_past_precedent(ri))
+            result.append(self.negative_passive_past_precedent_perfect(ri))
+            result.append(self.negative_passive_subjunctive_past_precedent_perfect(ri))
+            result.append(self.negative_passive_grammatical_past_precedent_perfect(ri))
+            result.append(self.negative_passive_imperfective_past_precedent_perfect(ri))
+            result.append(
+                self.negative_passive_subjunctive_imperfective_past_precedent_perfect(
+                    ri,
+                ),
+            )
+            result.append(self.negative_passive_perfective_present(ri))
+            result.append(self.negative_passive_subjunctive_perfective_present(ri))
+            result.append(self.negative_passive_grammatical_perfective_present(ri))
+            result.append(self.negative_passive_imperfective_present(ri))
+            result.append(self.negative_passive_perfective_future(ri))
+            result.append(self.negative_passive_imperfective_future(ri))
+            result.append(self.negative_passive_future_precedent(ri))
+            result.append(self.negative_passive_future_precedent_imperfective(ri))
+
+        elif passive and not negative:
+            result.append(self.passive_perfective_past(ri))
+            result.append(self.passive_imperfective_past(ri))
+            result.append(self.passive_past_progresive(ri))
+            result.append(self.passive_present_perfect(ri))
+            result.append(self.passive_subjunctive_present_perfect(ri))
+            result.append(self.passive_grammatical_present_perfect(ri))
+            result.append(self.passive_imperfective_present_perfect(ri))
+            result.append(self.passive_subjunctive_imperfective_present_perfect(ri))
+            result.append(self.passive_present_perfect_progressive(ri))
+            result.append(self.passive_past_precedent(ri))
+            result.append(self.passive_imperfective_past_precedent(ri))
+            result.append(self.passive_past_precedent_progressive(ri))
+            result.append(self.passive_past_precedent_perfect(ri))
+            result.append(self.passive_subjunctive_past_precedent_perfect(ri))
+            result.append(self.passive_grammatical_past_precedent_perfect(ri))
+            result.append(self.passive_imperfective_past_precedent_perfect(ri))
+            result.append(
+                self.passive_subjunctive_imperfective_past_precedent_perfect(ri),
+            )
+            result.append(self.passive_past_precedent_perfect_progressive(ri))
+            result.append(self.passive_perfective_present(ri))
+            result.append(self.passive_subjunctive_perfective_present(ri))
+            result.append(self.passive_grammatical_perfective_present(ri))
+            result.append(self.passive_imperfective_present(ri))
+            result.append(self.passive_present_progressive(ri))
+            result.append(self.passive_perfective_future(ri))
+            result.append(self.passive_imperfective_future(ri))
+            result.append(self.passive_future_precedent(ri))
+            result.append(self.passive_future_precedent_imperfective(ri))
+
+        elif negative and not passive:
+            result.append(self.negative_perfective_past(ri))
+            result.append(self.negative_imperfective_past(ri))
+            result.append(self.negative_present_perfect(ri))
+            result.append(self.negative_subjunctive_present_perfect(ri))
+            result.append(self.negative_grammatical_present_perfect(ri))
+            result.append(self.negative_imperfective_present_perfect(ri))
+            result.append(self.negative_subjunctive_imperfective_present_perfect(ri))
+            result.append(self.negative_past_precedent(ri))
+            result.append(self.negative_imperfective_past_precedent(ri))
+            result.append(self.negative_past_precedent_perfect(ri))
+            result.append(self.negative_subjunctive_past_precedent_perfect(ri))
+            result.append(self.negative_grammatical_past_precedent_perfect(ri))
+            result.append(self.negative_imperfective_past_precedent_perfect(ri))
+            result.append(
+                self.negative_subjunctive_imperfective_past_precedent_perfect(ri),
+            )
+            result.append(self.negative_perfective_present(rii))
+            result.append(self.negative_subjunctive_perfective_present(rii))
+            result.append(self.negative_grammatical_perfective_present(rii))
+            result.append(self.negative_imperfective_present(rii))
+            result.append(self.negative_perfective_future(ri))
+            result.append(self.negative_imperfective_future(ri))
+            result.append(self.negative_future_precedent(ri))
+            result.append(self.negative_future_precedent_imperfective(ri))
+
+        elif not negative and not passive:
+            result.append(self.perfective_past(ri))
+            result.append(self.imperfective_past(ri))
+            result.append(self.past_progresive(ri))
+            result.append(self.present_perfect(ri))
+            result.append(self.subjunctive_present_perfect(ri))
+            result.append(self.grammatical_present_perfect(ri))
+            result.append(self.imperfective_present_perfect(ri))
+            result.append(self.subjunctive_imperfective_present_perfect(ri))
+            result.append(self.present_perfect_progressive(ri))
+            result.append(self.past_precedent(ri))
+            result.append(self.imperfective_past_precedent(ri))
+            result.append(self.past_precedent_progressive(ri))
+            result.append(self.past_precedent_perfect(ri))
+            result.append(self.subjunctive_past_precedent_perfect(ri))
+            result.append(self.grammatical_past_precedent_perfect(ri))
+            result.append(self.imperfective_past_precedent_perfect(ri))
+            result.append(self.subjunctive_imperfective_past_precedent_perfect(ri))
+            result.append(self.past_precedent_perfect_progressive(ri))
+            result.append(self.perfective_present(rii))
+            result.append(self.subjunctive_perfective_present(rii))
+            result.append(self.grammatical_perfective_present(rii))
+            result.append(self.imperfective_present(rii))
+            result.append(self.present_progressive(rii))
+            result.append(self.perfective_future(ri))
+            result.append(self.imperfective_future(ri))
+            result.append(self.future_precedent(ri))
+            result.append(self.future_precedent_imperfective(ri))
+
+        return sum(result, [])
+
+    def get_all(self: "Conjugation", verb: str) -> List[str]:
+        """تمام صورت‌های صرفی فعل را در وجوه اخباری، التزامی، دستوری و در اشکال منفی و مثبت و مجهول برمی‌گرداند.
+
+        Args:
+            verb (str): فعلی که باید صرف شود. به‌صورت بن ماضی#بن مضارع؛ مانند: دید#بین.
+
+        Returns:
+             لیست تمام صورت‌های صرفی فعل.
+        """
+        ri, rii = verb.split("#")
+        infinitive = [ri + "ن"]
+        result = [infinitive]
+
+        # گذشتهٔ مطلق
+        result.append(self.perfective_past(ri))
+
+        # گذشتهٔ مطلق منفی
+        result.append(self.negative_perfective_past(ri))
+
+        # گذشتهٔ مطلق مجهول
+        result.append(self.passive_perfective_past(ri))
+
+        # گذشتهٔ مطلق مجهول منفی
+        result.append(self.negative_passive_perfective_past(ri))
+
+        # گذشتهٔ پایا
+        result.append(self.imperfective_past(ri))
+
+        # گذشتهٔ پایای منفی
+        result.append(self.negative_imperfective_past(ri))
+
+        # گذشتهٔ پایای مجهول
+        result.append(self.passive_imperfective_past(ri))
+
+        # گذشتهٔ پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_past(ri))
+
+        # گذشتهٔ استمراری
+        result.append(self.past_progresive(ri))
+
+        # گذشتهٔ استمراری مجهول
+        result.append(self.passive_past_progresive(ri))
+
+        # حال کامل
+        result.append(self.present_perfect(ri))
+
+        # حال کامل منفی
+        result.append(self.negative_present_perfect(ri))
+
+        # حال کامل التزامی
+        result.append(self.subjunctive_present_perfect(ri))
+
+        # حال کامل التزامی منفی
+        result.append(self.negative_subjunctive_present_perfect(ri))
+
+        # حال کامل دستوری
+        result.append(self.grammatical_present_perfect(ri))
+
+        # حال کامل دستوری منفی
+        result.append(self.negative_grammatical_present_perfect(ri))
+
+        # حال کامل مجهول
+        result.append(self.passive_present_perfect(ri))
+
+        # حال کامل مجهول منفی
+        result.append(self.negative_passive_present_perfect(ri))
+
+        # حال کامل التزامی مجهول
+        result.append(self.passive_subjunctive_present_perfect(ri))
+
+        # حال کامل التزامی مجهول منفی
+        result.append(self.negative_passive_subjunctive_present_perfect(ri))
+
+        # حال کامل دستوری مجهول
+        result.append(self.passive_grammatical_present_perfect(ri))
+
+        # حال کامل دستوری مجهول منفی
+        result.append(self.negative_passive_grammatical_present_perfect(ri))
+
+        # حال کامل پایا
+        result.append(self.imperfective_present_perfect(ri))
+
+        # حال کامل پایای منفی
+        result.append(self.negative_imperfective_present_perfect(ri))
+
+        # حال کامل پایای التزامی
+        result.append(self.subjunctive_imperfective_present_perfect(ri))
+
+        # حال کامل پایای التزامی منفی
+        result.append(self.negative_subjunctive_imperfective_present_perfect(ri))
+
+        # حال کامل پایای مجهول
+        result.append(self.passive_imperfective_present_perfect(ri))
+
+        # حال کامل پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_present_perfect(ri))
+
+        # حال کامل پایای التزامی مجهول
+        result.append(self.passive_subjunctive_imperfective_present_perfect(ri))
+
+        # حال کامل پایای التزامی مجهول منفی
+        result.append(
+            self.negative_passive_subjunctive_imperfective_present_perfect(ri),
+        )
+
+        # حال کامل استمراری
+        result.append(self.present_perfect_progressive(ri))
+
+        # حال کامل استمراری مجهول
+        result.append(self.passive_present_perfect_progressive(ri))
+
+        # گذشتهٔ پیشین
+        result.append(self.past_precedent(ri))
+
+        # گذشتهٔ پیشین منفی
+        result.append(self.negative_past_precedent(ri))
+
+        # گذشتهٔ پیشین مجهول
+        result.append(self.passive_past_precedent(ri))
+
+        # گذشتهٔ پیشین مجهول منفی
+        result.append(self.negative_passive_past_precedent(ri))
+
+        # گذشتهٔ پیشین پایا
+        result.append(self.imperfective_past_precedent(ri))
+
+        # گذشتهٔ پیشین پایای منفی
+        result.append(self.negative_imperfective_past_precedent(ri))
+
+        # گذشتهٔ پیشین پایای مجهول
+        result.append(self.passive_imperfective_past_precedent(ri))
+
+        # گذشتهٔ پیشین پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_past_precedent(ri))
+
+        # گذشتهٔ پیشین استمراری
+        result.append(self.past_precedent_progressive(ri))
+
+        # گذشتهٔ پیشین استمراری مجهول
+        result.append(self.passive_past_precedent_progressive(ri))
+
+        # گذشتهٔ پیشین کامل
+        result.append(self.past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل منفی
+        result.append(self.negative_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل التزامی
+        result.append(self.subjunctive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل التزامی منفی
+        result.append(self.negative_subjunctive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل دستوری
+        result.append(self.grammatical_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل دستوری منفی
+        result.append(self.negative_grammatical_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل مجهول
+        result.append(self.passive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل مجهول منفی
+        result.append(self.negative_passive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل التزامی مجهول
+        result.append(self.passive_subjunctive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل التزامی مجهول منفی
+        result.append(self.negative_passive_subjunctive_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشن کامل دستوری مجهول
+        result.append(self.passive_grammatical_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل دستوری مجهول منفی
+        result.append(self.negative_passive_grammatical_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایا
+        result.append(self.imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای منفی
+        result.append(self.negative_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای التزامی
+        result.append(self.subjunctive_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای التزامی منفی
+        result.append(self.negative_subjunctive_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای مجهول
+        result.append(self.passive_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای التزامی مجهول
+        result.append(self.passive_subjunctive_imperfective_past_precedent_perfect(ri))
+
+        # گذشتهٔ پیشین کامل پایای التزامی مجهول منفی
+        result.append(
+            self.negative_passive_subjunctive_imperfective_past_precedent_perfect(ri),
+        )
+
+        # گذشتهٔ پیشین کامل استمراری
+        result.append(self.past_precedent_perfect_progressive(ri))
+
+        # گذشتهٔ پیشین کامل استمراری مجهول
+        result.append(self.passive_past_precedent_perfect_progressive(ri))
+
+        # حال مطلق
+        result.append(self.perfective_present(rii))
+
+        # حال مطلق منفی
+        result.append(self.negative_perfective_present(rii))
+
+        # حال مطلق التزامی
+        result.append(self.subjunctive_perfective_present(rii))
+
+        # حال مطلق التزامی منفی
+        result.append(self.negative_subjunctive_perfective_present(rii))
+
+        # حال مطلق دستوری
+        result.append(self.grammatical_perfective_present(rii))
+
+        # حال مطلق دستوری منفی
+        result.append(self.negative_grammatical_perfective_present(rii))
+
+        # حال مطلق مجهول
+        result.append(self.passive_perfective_present(ri))
+
+        # حال مطلق مجهول منفی
+        result.append(self.negative_passive_perfective_present(ri))
+
+        # حال مطلق التزامی مجهول
+        result.append(self.passive_subjunctive_perfective_present(ri))
+
+        # حال مطلق التزامی مجهول منفی
+        result.append(self.negative_passive_subjunctive_perfective_present(ri))
+
+        # حال مطلق دستوری مجهول
+        result.append(self.passive_grammatical_perfective_present(ri))
+
+        # حال مطلق دستوری مجهول منفی
+        result.append(self.negative_passive_grammatical_perfective_present(ri))
+
+        # حال پایا
+        result.append(self.imperfective_present(rii))
+
+        # حال پایای منفی
+        result.append(self.negative_imperfective_present(rii))
+
+        # حال پایای مجهول
+        result.append(self.passive_imperfective_present(ri))
+
+        # حال پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_present(ri))
+
+        # حال استمراری
+        result.append(self.present_progressive(rii))
+
+        # حال استمراری مجهول
+        result.append(self.passive_present_progressive(ri))
+
+        # آیندهٔ مطلق
+        result.append(self.perfective_future(ri))
+
+        # آیندهٔ مطلق منفی
+        result.append(self.negative_perfective_future(ri))
+
+        # آیندهٔ مطلق مجهول
+        result.append(self.passive_perfective_future(ri))
+
+        # آیندهٔ مطلق مجهول منفی
+        result.append(self.negative_passive_perfective_future(ri))
+
+        # آیندهٔ پایا
+        result.append(self.imperfective_future(ri))
+
+        # آیندهٔ پایای منفی
+        result.append(self.negative_imperfective_future(ri))
+
+        # آیندهٔ پایای مجهول
+        result.append(self.passive_imperfective_future(ri))
+
+        # آیندهٔ پایای مجهول منفی
+        result.append(self.negative_passive_imperfective_future(ri))
+
+        # آیندهٔ پیشین
+        result.append(self.future_precedent(ri))
+
+        # آیندهٔ پیشین منفی
+        result.append(self.negative_future_precedent(ri))
+
+        # آیندهٔ پیشین مجهول
+        result.append(self.passive_future_precedent(ri))
+
+        # آیندهٔ پیشین مجهول منفی
+        result.append(self.negative_passive_future_precedent(ri))
+
+        # آیندهٔ پیشین پایا
+        result.append(self.future_precedent_imperfective(ri))
+
+        # آیندهٔ پیشین پایای منفی
+        result.append(self.negative_future_precedent_imperfective(ri))
+
+        # آیندهٔ پیشین پایای مجهول
+        result.append(self.passive_future_precedent_imperfective(ri))
+
+        # آیندهٔ پیشین پایای مجهول منفی
+        result.append(self.negative_passive_future_precedent_imperfective(ri))
+
+        return sum(result, [])
```

### Comparing `hazm-0.9.1/hazm/normalizer.py` & `hazm-0.9.2/hazm/normalizer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,535 +1,535 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای نرمال‌سازی متن است."""
-
-
-import re
-from typing import List
-
-from hazm import Lemmatizer
-from hazm import maketrans
-from hazm import regex_replace
-from hazm import WordTokenizer
-
-
-class Normalizer:
-    """این کلاس شامل توابعی برای نرمال‌سازی متن است.
-
-    Args:
-        correct_spacing: اگر `True‍` فاصله‌گذاری‌ها را در متن، نشانه‌های سجاوندی و پیشوندها و پسوندها اصلاح می‌کند.
-        remove_diacritics: اگر `True` باشد اعرابِ حروف را حذف می‌کند.
-        remove_specials_chars: اگر `True` باشد برخی از کاراکترها و نشانه‌های خاص را که کاربردی در پردازش متن ندارند حذف می‌کند.
-        decrease_repeated_chars: اگر `True` باشد تکرارهای بیش از ۲ بار را به ۲ بار کاهش می‌دهد. مثلاً «سلاممم» را به «سلامم» تبدیل می‌کند.
-        persian_style: اگر `True` باشد اصلاحات مخصوص زبان فارسی را انجام می‌دهد؛ مثلاً جایگزین‌کردن کوتیشن با گیومه.
-        persian_numbers: اگر `True` باشد ارقام انگلیسی را با فارسی جایگزین می‌کند.
-        unicodes_replacement: اگر `True` باشد برخی از کاراکترهای یونیکد را با معادل نرمال‌شدهٔ آن جایگزین می‌کند.
-        seperate_mi: اگر `True` باشد پیشوند «می» و «نمی» را در افعال جدا می‌کند.
-
-    """
-
-    def __init__(
-        self: "Normalizer",
-        correct_spacing: bool = True,
-        remove_diacritics: bool = True,
-        remove_specials_chars: bool = True,
-        decrease_repeated_chars: bool = True,
-        persian_style: bool = True,
-        persian_numbers: bool = True,
-        unicodes_replacement: bool = True,
-        seperate_mi: bool = True,
-    ) -> None:
-        self._correct_spacing = correct_spacing
-        self._remove_diacritics = remove_diacritics
-        self._remove_specials_chars = remove_specials_chars
-        self._decrease_repeated_chars = decrease_repeated_chars
-        self._persian_style = persian_style
-        self._persian_number = persian_numbers
-        self._unicodes_replacement = unicodes_replacement
-        self._seperate_mi = seperate_mi
-
-        self.translation_src = "ؠػػؽؾؿكيٮٯٷٸٹٺٻټٽٿڀځٵٶٷٸٹٺٻټٽٿڀځڂڅڇڈډڊڋڌڍڎڏڐڑڒړڔڕږڗڙښڛڜڝڞڟڠڡڢڣڤڥڦڧڨڪګڬڭڮڰڱڲڳڴڵڶڷڸڹںڻڼڽھڿہۂۃۄۅۆۇۈۉۊۋۏۍێېۑےۓەۮۯۺۻۼۿݐݑݒݓݔݕݖݗݘݙݚݛݜݝݞݟݠݡݢݣݤݥݦݧݨݩݪݫݬݭݮݯݰݱݲݳݴݵݶݷݸݹݺݻݼݽݾݿࢠࢡࢢࢣࢤࢥࢦࢧࢨࢩࢪࢫࢮࢯࢰࢱࢬࢲࢳࢴࢶࢷࢸࢹࢺࢻࢼࢽﭐﭑﭒﭓﭔﭕﭖﭗﭘﭙﭚﭛﭜﭝﭞﭟﭠﭡﭢﭣﭤﭥﭦﭧﭨﭩﭮﭯﭰﭱﭲﭳﭴﭵﭶﭷﭸﭹﭺﭻﭼﭽﭾﭿﮀﮁﮂﮃﮄﮅﮆﮇﮈﮉﮊﮋﮌﮍﮎﮏﮐﮑﮒﮓﮔﮕﮖﮗﮘﮙﮚﮛﮜﮝﮞﮟﮠﮡﮢﮣﮤﮥﮦﮧﮨﮩﮪﮫﮬﮭﮮﮯﮰﮱﺀﺁﺃﺄﺅﺆﺇﺈﺉﺊﺋﺌﺍﺎﺏﺐﺑﺒﺕﺖﺗﺘﺙﺚﺛﺜﺝﺞﺟﺠﺡﺢﺣﺤﺥﺦﺧﺨﺩﺪﺫﺬﺭﺮﺯﺰﺱﺲﺳﺴﺵﺶﺷﺸﺹﺺﺻﺼﺽﺾﺿﻀﻁﻂﻃﻄﻅﻆﻇﻈﻉﻊﻋﻌﻍﻎﻏﻐﻑﻒﻓﻔﻕﻖﻗﻘﻙﻚﻛﻜﻝﻞﻟﻠﻡﻢﻣﻤﻥﻦﻧﻨﻩﻪﻫﻬﻭﻮﻯﻰﻱﻲﻳﻴىكي“” "
-        self.translation_dst = (
-            'یککیییکیبقویتتبتتتبحاوویتتبتتتبحححچدددددددددررررررررسسسصصطعففففففققکککککگگگگگللللنننننهچهههوووووووووییییییهدرشضغهبببببببححددرسعععففکککممنننلررسححسرحاایییووییحسسکببجطفقلمییرودصگویزعکبپتریفقنااببببپپپپببببتتتتتتتتتتتتففففححححححححچچچچچچچچددددددددژژررککککگگگگگگگگگگگگننننننههههههههههییییءاااووااییییااببببتتتتثثثثججججححححخخخخددذذررززسسسسششششصصصصضضضضططططظظظظععععغغغغففففققققککککللللممممننننههههوویییییییکی"" '
-        )
-
-        if self._correct_spacing or self._decrease_repeated_chars:
-            self.tokenizer = WordTokenizer(join_verb_parts=False)
-            self.words = self.tokenizer.words
-
-        if self._persian_number:
-            self.number_translation_src = "0123456789%٠١٢٣٤٥٦٧٨٩"
-            self.number_translation_dst = "۰۱۲۳۴۵۶۷۸۹٪۰۱۲۳۴۵۶۷۸۹"
-
-        if self._correct_spacing:
-            self.suffixes = {
-                "ی",
-                "ای",
-                "ها",
-                "های",
-                "تر",
-                "تری",
-                "ترین",
-                "گر",
-                "گری",
-                "ام",
-                "ات",
-                "اش",
-            }
-
-            self.extra_space_patterns = [
-                (r" {2,}", " "),  # remove extra spaces
-                (r"\n{3,}", "\n\n"),  # remove extra newlines
-                (r"\u200c{2,}", "\u200c"),  # remove extra ZWNJs
-                (r"\u200c{1,} ", " "),  # remove unneded ZWNJs before space
-                (r" \u200c{1,}", " "),  # remove unneded ZWNJs after space
-                (r"\b\u200c*\B", ""),  # remove unneded ZWNJs at the beginning of words
-                (r"\B\u200c*\b", ""),  # remove unneded ZWNJs at the end of words
-                (r"[ـ\r]", ""),  # remove keshide, carriage returns
-            ]
-
-            punc_after, punc_before = r"\.:!،؛؟»\]\)\}", r"«\[\(\{"
-
-            self.punctuation_spacing_patterns = [
-                # remove space before and after quotation
-                ('" ([^\n"]+) "', r'"\1"'),
-                (" ([" + punc_after + "])", r"\1"),  # remove space before
-                ("([" + punc_before + "]) ", r"\1"),  # remove space after
-                # put space after . and :
-                (
-                    "([" + punc_after[:3] + "])([^ " + punc_after + r"\d۰۱۲۳۴۵۶۷۸۹])",
-                    r"\1 \2",
-                ),
-                (
-                    "([" + punc_after[3:] + "])([^ " + punc_after + "])",
-                    r"\1 \2",
-                ),  # put space after
-                (
-                    "([^ " + punc_before + "])([" + punc_before + "])",
-                    r"\1 \2",
-                ),  # put space before
-                # put space after number; e.g., به طول ۹متر -> به طول ۹ متر
-                (r"(\d)([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])", r"\1 \2"),
-                # put space after number; e.g., به طول۹ -> به طول ۹
-                (r"([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])(\d)", r"\1 \2"),
-            ]
-
-            self.affix_spacing_patterns = [
-                (r"([^ ]ه) ی ", r"\1‌ی "),  # fix ی space
-                (r"(^| )(ن?می) ", r"\1\2‌"),  # put zwnj after می, نمی
-                # put zwnj before تر, تری, ترین, گر, گری, ها, های
-                (
-                    r"(?<=[^\n\d "
-                    + punc_after
-                    + punc_before
-                    + "]{2}) (تر(ین?)?|گری?|های?)(?=[ \n"
-                    + punc_after
-                    + punc_before
-                    + "]|$)",
-                    r"‌\1",
-                ),
-                # join ام, ایم, اش, اند, ای, اید, ات
-                (
-                    r"([^ ]ه) (ا(م|یم|ش|ند|ی|ید|ت))(?=[ \n" + punc_after + "]|$)",
-                    r"\1‌\2",
-                ),
-                # شنبهها => شنبه‌ها
-                ("(ه)(ها)", r"\1‌\2"),
-            ]
-
-        if self._persian_style:
-            self.persian_style_patterns = [
-                ('"([^\n"]+)"', r"«\1»"),  # replace quotation with gyoome
-                (r"([\d+])\.([\d+])", r"\1٫\2"),  # replace dot with momayez
-                (r" ?\.\.\.", " …"),  # replace 3 dots
-            ]
-
-        if self._decrease_repeated_chars:
-            self.more_than_two_repeat_pattern = (
-                r"([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])\1{2,}"
-            )
-            self.repeated_chars_pattern = (
-                r"[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]*"
-                + self.more_than_two_repeat_pattern
-                + "[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]*"
-            )
-
-        if self._remove_diacritics:
-            self.diacritics_patterns = [
-                # remove FATHATAN, DAMMATAN, KASRATAN, FATHA, DAMMA, KASRA, SHADDA, SUKUN
-                ("[\u064b\u064c\u064d\u064e\u064f\u0650\u0651\u0652]", ""),
-            ]
-
-        if self._remove_specials_chars:
-            self.specials_chars_patterns = [
-                # Remove almoast all arabic unicode superscript and subscript characters in the ranges of 00600-06FF, 08A0-08FF, FB50-FDFF, and FE70-FEFF
-                (
-                    "[\u0605\u0653\u0654\u0655\u0656\u0657\u0658\u0659\u065a\u065b\u065c\u065d\u065e\u065f\u0670\u0610\u0611\u0612\u0613\u0614\u0615\u0616\u0618\u0619\u061a\u061e\u06d4\u06d6\u06d7\u06d8\u06d9\u06da\u06db\u06dc\u06dd\u06de\u06df\u06e0\u06e1\u06e2\u06e3\u06e4\u06e5\u06e6\u06e7\u06e8\u06e9\u06ea\u06eb\u06ec\u06ed\u06fd\u06fe\u08ad\u08d4\u08d5\u08d6\u08d7\u08d8\u08d9\u08da\u08db\u08dc\u08dd\u08de\u08df\u08e0\u08e1\u08e2\u08e3\u08e4\u08e5\u08e6\u08e7\u08e8\u08e9\u08ea\u08eb\u08ec\u08ed\u08ee\u08ef\u08f0\u08f1\u08f2\u08f3\u08f4\u08f5\u08f6\u08f7\u08f8\u08f9\u08fa\u08fb\u08fc\u08fd\u08fe\u08ff\ufbb2\ufbb3\ufbb4\ufbb5\ufbb6\ufbb7\ufbb8\ufbb9\ufbba\ufbbb\ufbbc\ufbbd\ufbbe\ufbbf\ufbc0\ufbc1\ufc5e\ufc5f\ufc60\ufc61\ufc62\ufc63\ufcf2\ufcf3\ufcf4\ufd3e\ufd3f\ufe70\ufe71\ufe72\ufe76\ufe77\ufe78\ufe79\ufe7a\ufe7b\ufe7c\ufe7d\ufe7e\ufe7f\ufdfa\ufdfb]",
-                    "",
-                ),
-            ]
-
-        if self._seperate_mi:
-            self.verbs = Lemmatizer(joined_verb_parts=False).verbs
-            self.joint_mi_patterns = r"\bن?می[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]+"
-
-        if self._unicodes_replacement:
-            self.replacements = [
-                ("﷽", "بسم الله الرحمن الرحیم"),
-                ("﷼", "ریال"),
-                ("(ﷰ|ﷹ)", "صلی"),
-                ("ﷲ", "الله"),
-                ("ﷳ", "اکبر"),
-                ("ﷴ", "محمد"),
-                ("ﷵ", "صلعم"),
-                ("ﷶ", "رسول"),
-                ("ﷷ", "علیه"),
-                ("ﷸ", "وسلم"),
-                ("ﻵ|ﻶ|ﻷ|ﻸ|ﻹ|ﻺ|ﻻ|ﻼ", "لا"),
-            ]
-
-    def normalize(self: "Normalizer", text: str) -> str:
-        """متن را نرمال‌سازی می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.normalize('اِعلاممممم کَرد : « زمین لرزه ای به بُزرگیِ 6 دهم ریشتر ...»')
-            'اعلام کرد: «زمین‌لرزه‌ای به بزرگی ۶ دهم ریشتر …»'
-            >>> normalizer.normalize('')
-            ''
-
-        Args:
-            text: متنی که باید نرمال‌سازی شود.
-
-        Returns:
-            متنِ نرمال‌سازی‌شده.
-
-        """
-        translations = maketrans(self.translation_src, self.translation_dst)
-        text = text.translate(translations)
-
-        if self._persian_style:
-            text = self.persian_style(text)
-
-        if self._persian_number:
-            text = self.persian_number(text)
-
-        if self._remove_diacritics:
-            text = self.remove_diacritics(text)
-
-        if self._correct_spacing:
-            text = self.correct_spacing(text)
-
-        if self._unicodes_replacement:
-            text = self.unicodes_replacement(text)
-
-        if self._remove_specials_chars:
-            text = self.remove_specials_chars(text)
-
-        if self._decrease_repeated_chars:
-            text = self.decrease_repeated_chars(text)
-
-        if self._seperate_mi:
-            text = self.seperate_mi(text)
-
-        return text
-
-    def correct_spacing(self: "Normalizer", text: str) -> str:
-        """فاصله‌گذاری‌ها را در پیشوندها و پسوندها اصلاح می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.correct_spacing("سلام   دنیا")
-            'سلام دنیا'
-            >>> normalizer.correct_spacing("به طول ۹متر و عرض۶")
-            'به طول ۹ متر و عرض ۶'
-            >>> normalizer.correct_spacing("کاروان‌‌سرا")
-            'کاروان‌سرا'
-            >>> normalizer.correct_spacing("‌سلام‌ به ‌همه‌")
-            'سلام به همه'
-            >>> normalizer.correct_spacing("سلام دنیـــا")
-            'سلام دنیا'
-            >>> normalizer.correct_spacing("جمعهها که کار نمی کنم مطالعه می کنم")
-            'جمعه‌ها که کار نمی‌کنم مطالعه می‌کنم'
-            >>> normalizer.correct_spacing(' "سلام به همه"   ')
-            '"سلام به همه"'
-            >>> normalizer.correct_spacing('')
-            ''
-
-        Args:
-            text (str): متنی که باید فاصله‌گذاری‌های آن اصلاح شود.
-
-        Returns:
-            (str): متنی با فاصله‌گذاری‌های اصلاح‌شده.
-
-
-        """
-        text = regex_replace(self.extra_space_patterns, text)
-
-        lines = text.split("\n")
-        result = []
-        for line in lines:
-            tokens = self.tokenizer.tokenize(line)
-            spaced_tokens = self.token_spacing(tokens)
-            line = " ".join(spaced_tokens)
-            result.append(line)
-
-        text = "\n".join(result)
-
-        text = regex_replace(self.affix_spacing_patterns, text)
-        text = regex_replace(self.punctuation_spacing_patterns, text)
-
-        return text
-
-    def remove_diacritics(self: "Normalizer", text: str) -> str:
-        """اِعراب را از متن حذف می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.remove_diacritics('حَذفِ اِعراب')
-            'حذف اعراب'
-            >>> normalizer.remove_diacritics('آمدند')
-            'آمدند'
-            >>> normalizer.remove_diacritics('متن بدون اعراب')
-            'متن بدون اعراب'
-            >>> normalizer.remove_diacritics('')
-            ''
-
-        Args:
-            text: متنی که باید اعراب آن حذف شود.
-
-        Returns:
-            متنی بدون اعراب.
-
-        """
-        return regex_replace(self.diacritics_patterns, text)
-
-    def remove_specials_chars(self: "Normalizer", text: str) -> str:
-        """برخی از کاراکترها و نشانه‌های خاص را که کاربردی در پردازش متن ندارند حذف
-        می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.remove_specials_chars('پیامبر اکرم ﷺ')
-            'پیامبر اکرم '
-
-        Args:
-            text: متنی که باید کاراکترها و نشانه‌های اضافهٔ آن حذف شود.
-
-        Returns:
-            متنی بدون کاراکترها و نشانه‌های اضافه.
-
-        """
-        return regex_replace(self.specials_chars_patterns, text)
-
-    def decrease_repeated_chars(self: "Normalizer", text: str) -> str:
-        """تکرارهای زائد حروف را در کلماتی مثل سلامممممم حذف می‌کند و در مواردی که
-        نمی‌تواند تشخیص دهد دست کم به دو تکرار کاهش می‌دهد.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.decrease_repeated_chars('سلامممم به همه')
-            'سلام به همه'
-            >>> normalizer.decrease_repeated_chars('سلامم به همه')
-            'سلامم به همه'
-            >>> normalizer.decrease_repeated_chars('سلامم را برسان')
-            'سلامم را برسان'
-            >>> normalizer.decrease_repeated_chars('سلاممم را برسان')
-            'سلام را برسان'
-            >>> normalizer.decrease_repeated_chars('')
-            ''
-
-        Args:
-            text: متنی که باید تکرارهای زائد آن حذف شود.
-
-        Returns:
-            متنی بدون کاراکترهای زائد یا حداقل با دو تکرار.
-
-        """
-        matches = re.finditer(self.repeated_chars_pattern, text)
-
-        for m in matches:
-            word = m.group()
-            if word not in self.words:
-                no_repeat = re.sub(self.more_than_two_repeat_pattern, r"\1", word)
-                two_repeat = re.sub(self.more_than_two_repeat_pattern, r"\1\1", word)
-
-                if (no_repeat in self.words) != (two_repeat in self.words):
-                    r = no_repeat if no_repeat in self.words else two_repeat
-                    text = text.replace(word, r)
-                else:
-                    text = text.replace(word, two_repeat)
-
-        return text
-
-    def persian_style(self: "Normalizer", text: str) -> str:
-        """برخی از حروف و نشانه‌ها را با حروف و نشانه‌های فارسی جایگزین می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.persian_style('"نرمال‌سازی"')
-            '«نرمال‌سازی»'
-            >>> normalizer.persian_style('و ...')
-            'و …'
-            >>> normalizer.persian_style('10.450')
-            '10٫450'
-            >>> normalizer.persian_style('')
-            ''
-
-        Args:
-            text: متنی که باید حروف و نشانه‌های آن با حروف و نشانه‌های فارسی جایگزین شود.
-
-        Returns:
-            متنی با حروف و نشانه‌های فارسی‌سازی شده.
-
-        """
-        return regex_replace(self.persian_style_patterns, text)
-
-    def persian_number(self: "Normalizer", text: str) -> str:
-        """اعداد لاتین و علامت % را با معادل فارسی آن جایگزین می‌کند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.persian_number('5 درصد')
-            '۵ درصد'
-            >>> normalizer.persian_number('۵ درصد')
-            '۵ درصد'
-            >>> normalizer.persian_number('')
-            ''
-
-        Args:
-            text: متنی که باید اعداد لاتین و علامت % آن با معادل فارسی جایگزین شود.
-
-        Returns:
-            متنی با اعداد و علامت ٪ فارسی.
-
-        """
-        translations = maketrans(
-            self.number_translation_src,
-            self.number_translation_dst,
-        )
-        return text.translate(translations)
-
-    def unicodes_replacement(self: "Normalizer", text: str) -> str:
-        """برخی از کاراکترهای خاص یونیکد را با معادلِ نرمال آن جایگزین می‌کند. غالباً
-        این کار فقط در مواردی صورت می‌گیرد که یک کلمه در قالب یک کاراکتر یونیکد تعریف
-        شده است.
-
-        **فهرست این کاراکترها و نسخهٔ جایگزین آن:**
-
-        |کاراکتر|نسخهٔ جایگزین|
-        |--------|------------------|
-        |﷽|بسم الله الرحمن الرحیم|
-        |﷼|ریال|
-        |ﷰ، ﷹ|صلی|
-        |ﷲ|الله|
-        |ﷳ|اکبر|
-        |ﷴ|محمد|
-        |ﷵ|صلعم|
-        |ﷶ|رسول|
-        |ﷷ|علیه|
-        |ﷸ|وسلم|
-        |ﻵ، ﻶ، ﻷ، ﻸ، ﻹ، ﻺ، ﻻ، ﻼ|لا|
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.remove_specials_chars('پیامبر اکرم ﷺ')
-            'پیامبر اکرم '
-            >>> normalizer.remove_specials_chars('')
-            ''
-
-        Args:
-            text: متنی که باید برخی از کاراکترهای یونیکد آن (جدول بالا)، با شکل استاندارد، جایگزین شود.
-
-        Returns:
-            متنی که برخی از کاراکترهای یونیکد آن با شکل استاندارد جایگزین شده است.
-
-        """
-        for old, new in self.replacements:
-            text = re.sub(old, new, text)
-
-        return text
-
-    def seperate_mi(self: "Normalizer", text: str) -> str:
-        """پیشوند «می» و «نمی» را در افعال جدا کرده و با نیم‌فاصله می‌چسباند.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.seperate_mi('نمیدانم چه میگفت')
-            'نمی‌دانم چه می‌گفت'
-            >>> normalizer.seperate_mi('میز')
-            'میز'
-            >>> normalizer.seperate_mi('')
-            ''
-
-
-        Args:
-            text: متنی که باید پیشوند «می» و «نمی» در آن جدا شود.
-
-        Returns:
-            متنی با «می» و «نمی» جدا شده.
-
-        """
-        matches = re.findall(r"\bن?می[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]+", text)
-        for m in matches:
-            r = re.sub("^(ن?می)", r"\1‌", m)
-            if r in self.verbs:
-                text = text.replace(m, r)
-
-        return text
-
-    def token_spacing(self: "Normalizer", tokens: List[str]) -> List[str]:
-        """توکن‌های ورودی را به فهرستی از توکن‌های نرمال‌سازی شده تبدیل می‌کند.
-        در این فرایند ممکن است برخی از توکن‌ها به یکدیگر بچسبند؛
-        برای مثال: `['زمین', 'لرزه', 'ای']` تبدیل می‌شود به: `['زمین‌لرزه‌ای']`.
-
-        Examples:
-            >>> normalizer = Normalizer()
-            >>> normalizer.token_spacing(['کتاب', 'ها'])
-            ['کتاب‌ها']
-            >>> normalizer.token_spacing(['او', 'می', 'رود'])
-            ['او', 'می‌رود']
-            >>> normalizer.token_spacing(['ماه', 'می', 'سال', 'جدید'])
-            ['ماه', 'می', 'سال', 'جدید']
-            >>> normalizer.token_spacing(['اخلال', 'گر'])
-            ['اخلال‌گر']
-            >>> normalizer.token_spacing(['زمین', 'لرزه', 'ای'])
-            ['زمین‌لرزه‌ای']
-            >>> normalizer.token_spacing([])
-            []
-
-        Args:
-            tokens: توکن‌هایی که باید نرمال‌سازی شود.
-
-        Returns:
-            لیستی از توکن‌های نرمال‌سازی شده به شکل `[token1, token2, ...]`.
-
-        """
-        # >>> normalizer.token_spacing(['پرداخت', 'شده', 'است'])
-
-        result = []
-        for t, token in enumerate(tokens):
-            joined = False
-
-            if result:
-                token_pair = result[-1] + "‌" + token
-                if (
-                    token_pair in self.verbs
-                    or token_pair in self.words
-                    and self.words[token_pair][0] > 0
-                ):
-                    joined = True
-
-                    if (
-                        t < len(tokens) - 1
-                        and token + "_" + tokens[t + 1] in self.verbs
-                    ):
-                        joined = False
-
-                elif token in self.suffixes and result[-1] in self.words:
-                    joined = True
-
-            if joined:
-                result.pop()
-                result.append(token_pair)
-            else:
-                result.append(token)
-
-        return result
+"""این ماژول شامل کلاس‌ها و توابعی برای نرمال‌سازی متن است."""
+
+
+import re
+from typing import List
+
+from hazm import Lemmatizer
+from hazm import WordTokenizer
+from hazm import maketrans
+from hazm import regex_replace
+
+
+class Normalizer:
+    """این کلاس شامل توابعی برای نرمال‌سازی متن است.
+
+    Args:
+        correct_spacing: اگر `True‍` فاصله‌گذاری‌ها را در متن، نشانه‌های سجاوندی و پیشوندها و پسوندها اصلاح می‌کند.
+        remove_diacritics: اگر `True` باشد اعرابِ حروف را حذف می‌کند.
+        remove_specials_chars: اگر `True` باشد برخی از کاراکترها و نشانه‌های خاص را که کاربردی در پردازش متن ندارند حذف می‌کند.
+        decrease_repeated_chars: اگر `True` باشد تکرارهای بیش از ۲ بار را به ۲ بار کاهش می‌دهد. مثلاً «سلاممم» را به «سلامم» تبدیل می‌کند.
+        persian_style: اگر `True` باشد اصلاحات مخصوص زبان فارسی را انجام می‌دهد؛ مثلاً جایگزین‌کردن کوتیشن با گیومه.
+        persian_numbers: اگر `True` باشد ارقام انگلیسی را با فارسی جایگزین می‌کند.
+        unicodes_replacement: اگر `True` باشد برخی از کاراکترهای یونیکد را با معادل نرمال‌شدهٔ آن جایگزین می‌کند.
+        seperate_mi: اگر `True` باشد پیشوند «می» و «نمی» را در افعال جدا می‌کند.
+
+    """
+
+    def __init__(
+        self: "Normalizer",
+        correct_spacing: bool = True,
+        remove_diacritics: bool = True,
+        remove_specials_chars: bool = True,
+        decrease_repeated_chars: bool = True,
+        persian_style: bool = True,
+        persian_numbers: bool = True,
+        unicodes_replacement: bool = True,
+        seperate_mi: bool = True,
+    ) -> None:
+        self._correct_spacing = correct_spacing
+        self._remove_diacritics = remove_diacritics
+        self._remove_specials_chars = remove_specials_chars
+        self._decrease_repeated_chars = decrease_repeated_chars
+        self._persian_style = persian_style
+        self._persian_number = persian_numbers
+        self._unicodes_replacement = unicodes_replacement
+        self._seperate_mi = seperate_mi
+
+        self.translation_src = "ؠػػؽؾؿكيٮٯٷٸٹٺٻټٽٿڀځٵٶٷٸٹٺٻټٽٿڀځڂڅڇڈډڊڋڌڍڎڏڐڑڒړڔڕږڗڙښڛڜڝڞڟڠڡڢڣڤڥڦڧڨڪګڬڭڮڰڱڲڳڴڵڶڷڸڹںڻڼڽھڿہۂۃۄۅۆۇۈۉۊۋۏۍێېۑےۓەۮۯۺۻۼۿݐݑݒݓݔݕݖݗݘݙݚݛݜݝݞݟݠݡݢݣݤݥݦݧݨݩݪݫݬݭݮݯݰݱݲݳݴݵݶݷݸݹݺݻݼݽݾݿࢠࢡࢢࢣࢤࢥࢦࢧࢨࢩࢪࢫࢮࢯࢰࢱࢬࢲࢳࢴࢶࢷࢸࢹࢺࢻࢼࢽﭐﭑﭒﭓﭔﭕﭖﭗﭘﭙﭚﭛﭜﭝﭞﭟﭠﭡﭢﭣﭤﭥﭦﭧﭨﭩﭮﭯﭰﭱﭲﭳﭴﭵﭶﭷﭸﭹﭺﭻﭼﭽﭾﭿﮀﮁﮂﮃﮄﮅﮆﮇﮈﮉﮊﮋﮌﮍﮎﮏﮐﮑﮒﮓﮔﮕﮖﮗﮘﮙﮚﮛﮜﮝﮞﮟﮠﮡﮢﮣﮤﮥﮦﮧﮨﮩﮪﮫﮬﮭﮮﮯﮰﮱﺀﺁﺃﺄﺅﺆﺇﺈﺉﺊﺋﺌﺍﺎﺏﺐﺑﺒﺕﺖﺗﺘﺙﺚﺛﺜﺝﺞﺟﺠﺡﺢﺣﺤﺥﺦﺧﺨﺩﺪﺫﺬﺭﺮﺯﺰﺱﺲﺳﺴﺵﺶﺷﺸﺹﺺﺻﺼﺽﺾﺿﻀﻁﻂﻃﻄﻅﻆﻇﻈﻉﻊﻋﻌﻍﻎﻏﻐﻑﻒﻓﻔﻕﻖﻗﻘﻙﻚﻛﻜﻝﻞﻟﻠﻡﻢﻣﻤﻥﻦﻧﻨﻩﻪﻫﻬﻭﻮﻯﻰﻱﻲﻳﻴىكي“” "
+        self.translation_dst = (
+            'یککیییکیبقویتتبتتتبحاوویتتبتتتبحححچدددددددددررررررررسسسصصطعففففففققکککککگگگگگللللنننننهچهههوووووووووییییییهدرشضغهبببببببححددرسعععففکککممنننلررسححسرحاایییووییحسسکببجطفقلمییرودصگویزعکبپتریفقنااببببپپپپببببتتتتتتتتتتتتففففححححححححچچچچچچچچددددددددژژررککککگگگگگگگگگگگگننننننههههههههههییییءاااووااییییااببببتتتتثثثثججججححححخخخخددذذررززسسسسششششصصصصضضضضططططظظظظععععغغغغففففققققککککللللممممننننههههوویییییییکی"" '
+        )
+
+        if self._correct_spacing or self._decrease_repeated_chars:
+            self.tokenizer = WordTokenizer(join_verb_parts=False)
+            self.words = self.tokenizer.words
+
+        if self._persian_number:
+            self.number_translation_src = "0123456789%٠١٢٣٤٥٦٧٨٩"
+            self.number_translation_dst = "۰۱۲۳۴۵۶۷۸۹٪۰۱۲۳۴۵۶۷۸۹"
+
+        if self._correct_spacing:
+            self.suffixes = {
+                "ی",
+                "ای",
+                "ها",
+                "های",
+                "تر",
+                "تری",
+                "ترین",
+                "گر",
+                "گری",
+                "ام",
+                "ات",
+                "اش",
+            }
+
+            self.extra_space_patterns = [
+                (r" {2,}", " "),  # remove extra spaces
+                (r"\n{3,}", "\n\n"),  # remove extra newlines
+                (r"\u200c{2,}", "\u200c"),  # remove extra ZWNJs
+                (r"\u200c{1,} ", " "),  # remove unneded ZWNJs before space
+                (r" \u200c{1,}", " "),  # remove unneded ZWNJs after space
+                (r"\b\u200c*\B", ""),  # remove unneded ZWNJs at the beginning of words
+                (r"\B\u200c*\b", ""),  # remove unneded ZWNJs at the end of words
+                (r"[ـ\r]", ""),  # remove keshide, carriage returns
+            ]
+
+            punc_after, punc_before = r"\.:!،؛؟»\]\)\}", r"«\[\(\{"
+
+            self.punctuation_spacing_patterns = [
+                # remove space before and after quotation
+                ('" ([^\n"]+) "', r'"\1"'),
+                (" ([" + punc_after + "])", r"\1"),  # remove space before
+                ("([" + punc_before + "]) ", r"\1"),  # remove space after
+                # put space after . and :
+                (
+                    "([" + punc_after[:3] + "])([^ " + punc_after + r"\d۰۱۲۳۴۵۶۷۸۹])",
+                    r"\1 \2",
+                ),
+                (
+                    "([" + punc_after[3:] + "])([^ " + punc_after + "])",
+                    r"\1 \2",
+                ),  # put space after
+                (
+                    "([^ " + punc_before + "])([" + punc_before + "])",
+                    r"\1 \2",
+                ),  # put space before
+                # put space after number; e.g., به طول ۹متر -> به طول ۹ متر
+                (r"(\d)([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])", r"\1 \2"),
+                # put space after number; e.g., به طول۹ -> به طول ۹
+                (r"([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])(\d)", r"\1 \2"),
+            ]
+
+            self.affix_spacing_patterns = [
+                (r"([^ ]ه) ی ", r"\1‌ی "),  # fix ی space
+                (r"(^| )(ن?می) ", r"\1\2‌"),  # put zwnj after می, نمی
+                # put zwnj before تر, تری, ترین, گر, گری, ها, های
+                (
+                    r"(?<=[^\n\d "
+                    + punc_after
+                    + punc_before
+                    + "]{2}) (تر(ین?)?|گری?|های?)(?=[ \n"
+                    + punc_after
+                    + punc_before
+                    + "]|$)",
+                    r"‌\1",
+                ),
+                # join ام, ایم, اش, اند, ای, اید, ات
+                (
+                    r"([^ ]ه) (ا(م|یم|ش|ند|ی|ید|ت))(?=[ \n" + punc_after + "]|$)",
+                    r"\1‌\2",
+                ),
+                # شنبهها => شنبه‌ها
+                ("(ه)(ها)", r"\1‌\2"),
+            ]
+
+        if self._persian_style:
+            self.persian_style_patterns = [
+                ('"([^\n"]+)"', r"«\1»"),  # replace quotation with gyoome
+                (r"([\d+])\.([\d+])", r"\1٫\2"),  # replace dot with momayez
+                (r" ?\.\.\.", " …"),  # replace 3 dots
+            ]
+
+        if self._decrease_repeated_chars:
+            self.more_than_two_repeat_pattern = (
+                r"([آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی])\1{2,}"
+            )
+            self.repeated_chars_pattern = (
+                r"[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]*"
+                + self.more_than_two_repeat_pattern
+                + "[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]*"
+            )
+
+        if self._remove_diacritics:
+            self.diacritics_patterns = [
+                # remove FATHATAN, DAMMATAN, KASRATAN, FATHA, DAMMA, KASRA, SHADDA, SUKUN
+                ("[\u064b\u064c\u064d\u064e\u064f\u0650\u0651\u0652]", ""),
+            ]
+
+        if self._remove_specials_chars:
+            self.specials_chars_patterns = [
+                # Remove almoast all arabic unicode superscript and subscript characters in the ranges of 00600-06FF, 08A0-08FF, FB50-FDFF, and FE70-FEFF
+                (
+                    "[\u0605\u0653\u0654\u0655\u0656\u0657\u0658\u0659\u065a\u065b\u065c\u065d\u065e\u065f\u0670\u0610\u0611\u0612\u0613\u0614\u0615\u0616\u0618\u0619\u061a\u061e\u06d4\u06d6\u06d7\u06d8\u06d9\u06da\u06db\u06dc\u06dd\u06de\u06df\u06e0\u06e1\u06e2\u06e3\u06e4\u06e5\u06e6\u06e7\u06e8\u06e9\u06ea\u06eb\u06ec\u06ed\u06fd\u06fe\u08ad\u08d4\u08d5\u08d6\u08d7\u08d8\u08d9\u08da\u08db\u08dc\u08dd\u08de\u08df\u08e0\u08e1\u08e2\u08e3\u08e4\u08e5\u08e6\u08e7\u08e8\u08e9\u08ea\u08eb\u08ec\u08ed\u08ee\u08ef\u08f0\u08f1\u08f2\u08f3\u08f4\u08f5\u08f6\u08f7\u08f8\u08f9\u08fa\u08fb\u08fc\u08fd\u08fe\u08ff\ufbb2\ufbb3\ufbb4\ufbb5\ufbb6\ufbb7\ufbb8\ufbb9\ufbba\ufbbb\ufbbc\ufbbd\ufbbe\ufbbf\ufbc0\ufbc1\ufc5e\ufc5f\ufc60\ufc61\ufc62\ufc63\ufcf2\ufcf3\ufcf4\ufd3e\ufd3f\ufe70\ufe71\ufe72\ufe76\ufe77\ufe78\ufe79\ufe7a\ufe7b\ufe7c\ufe7d\ufe7e\ufe7f\ufdfa\ufdfb]",
+                    "",
+                ),
+            ]
+
+        if self._seperate_mi:
+            self.verbs = Lemmatizer(joined_verb_parts=False).verbs
+            self.joint_mi_patterns = r"\bن?می[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]+"
+
+        if self._unicodes_replacement:
+            self.replacements = [
+                ("﷽", "بسم الله الرحمن الرحیم"),
+                ("﷼", "ریال"),
+                ("(ﷰ|ﷹ)", "صلی"),
+                ("ﷲ", "الله"),
+                ("ﷳ", "اکبر"),
+                ("ﷴ", "محمد"),
+                ("ﷵ", "صلعم"),
+                ("ﷶ", "رسول"),
+                ("ﷷ", "علیه"),
+                ("ﷸ", "وسلم"),
+                ("ﻵ|ﻶ|ﻷ|ﻸ|ﻹ|ﻺ|ﻻ|ﻼ", "لا"),
+            ]
+
+    def normalize(self: "Normalizer", text: str) -> str:
+        """متن را نرمال‌سازی می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.normalize('اِعلاممممم کَرد : « زمین لرزه ای به بُزرگیِ 6 دهم ریشتر ...»')
+            'اعلام کرد: «زمین‌لرزه‌ای به بزرگی ۶ دهم ریشتر …»'
+            >>> normalizer.normalize('')
+            ''
+
+        Args:
+            text: متنی که باید نرمال‌سازی شود.
+
+        Returns:
+            متنِ نرمال‌سازی‌شده.
+
+        """
+        translations = maketrans(self.translation_src, self.translation_dst)
+        text = text.translate(translations)
+
+        if self._persian_style:
+            text = self.persian_style(text)
+
+        if self._persian_number:
+            text = self.persian_number(text)
+
+        if self._remove_diacritics:
+            text = self.remove_diacritics(text)
+
+        if self._correct_spacing:
+            text = self.correct_spacing(text)
+
+        if self._unicodes_replacement:
+            text = self.unicodes_replacement(text)
+
+        if self._remove_specials_chars:
+            text = self.remove_specials_chars(text)
+
+        if self._decrease_repeated_chars:
+            text = self.decrease_repeated_chars(text)
+
+        if self._seperate_mi:
+            text = self.seperate_mi(text)
+
+        return text
+
+    def correct_spacing(self: "Normalizer", text: str) -> str:
+        """فاصله‌گذاری‌ها را در پیشوندها و پسوندها اصلاح می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.correct_spacing("سلام   دنیا")
+            'سلام دنیا'
+            >>> normalizer.correct_spacing("به طول ۹متر و عرض۶")
+            'به طول ۹ متر و عرض ۶'
+            >>> normalizer.correct_spacing("کاروان‌‌سرا")
+            'کاروان‌سرا'
+            >>> normalizer.correct_spacing("‌سلام‌ به ‌همه‌")
+            'سلام به همه'
+            >>> normalizer.correct_spacing("سلام دنیـــا")
+            'سلام دنیا'
+            >>> normalizer.correct_spacing("جمعهها که کار نمی کنم مطالعه می کنم")
+            'جمعه‌ها که کار نمی‌کنم مطالعه می‌کنم'
+            >>> normalizer.correct_spacing(' "سلام به همه"   ')
+            '"سلام به همه"'
+            >>> normalizer.correct_spacing('')
+            ''
+
+        Args:
+            text (str): متنی که باید فاصله‌گذاری‌های آن اصلاح شود.
+
+        Returns:
+            (str): متنی با فاصله‌گذاری‌های اصلاح‌شده.
+
+
+        """
+        text = regex_replace(self.extra_space_patterns, text)
+
+        lines = text.split("\n")
+        result = []
+        for line in lines:
+            tokens = self.tokenizer.tokenize(line)
+            spaced_tokens = self.token_spacing(tokens)
+            line = " ".join(spaced_tokens)
+            result.append(line)
+
+        text = "\n".join(result)
+
+        text = regex_replace(self.affix_spacing_patterns, text)
+        text = regex_replace(self.punctuation_spacing_patterns, text)
+
+        return text
+
+    def remove_diacritics(self: "Normalizer", text: str) -> str:
+        """اِعراب را از متن حذف می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.remove_diacritics('حَذفِ اِعراب')
+            'حذف اعراب'
+            >>> normalizer.remove_diacritics('آمدند')
+            'آمدند'
+            >>> normalizer.remove_diacritics('متن بدون اعراب')
+            'متن بدون اعراب'
+            >>> normalizer.remove_diacritics('')
+            ''
+
+        Args:
+            text: متنی که باید اعراب آن حذف شود.
+
+        Returns:
+            متنی بدون اعراب.
+
+        """
+        return regex_replace(self.diacritics_patterns, text)
+
+    def remove_specials_chars(self: "Normalizer", text: str) -> str:
+        """برخی از کاراکترها و نشانه‌های خاص را که کاربردی در پردازش متن ندارند حذف
+        می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.remove_specials_chars('پیامبر اکرم ﷺ')
+            'پیامبر اکرم '
+
+        Args:
+            text: متنی که باید کاراکترها و نشانه‌های اضافهٔ آن حذف شود.
+
+        Returns:
+            متنی بدون کاراکترها و نشانه‌های اضافه.
+
+        """
+        return regex_replace(self.specials_chars_patterns, text)
+
+    def decrease_repeated_chars(self: "Normalizer", text: str) -> str:
+        """تکرارهای زائد حروف را در کلماتی مثل سلامممممم حذف می‌کند و در مواردی که
+        نمی‌تواند تشخیص دهد دست کم به دو تکرار کاهش می‌دهد.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.decrease_repeated_chars('سلامممم به همه')
+            'سلام به همه'
+            >>> normalizer.decrease_repeated_chars('سلامم به همه')
+            'سلامم به همه'
+            >>> normalizer.decrease_repeated_chars('سلامم را برسان')
+            'سلامم را برسان'
+            >>> normalizer.decrease_repeated_chars('سلاممم را برسان')
+            'سلام را برسان'
+            >>> normalizer.decrease_repeated_chars('')
+            ''
+
+        Args:
+            text: متنی که باید تکرارهای زائد آن حذف شود.
+
+        Returns:
+            متنی بدون کاراکترهای زائد یا حداقل با دو تکرار.
+
+        """
+        matches = re.finditer(self.repeated_chars_pattern, text)
+
+        for m in matches:
+            word = m.group()
+            if word not in self.words:
+                no_repeat = re.sub(self.more_than_two_repeat_pattern, r"\1", word)
+                two_repeat = re.sub(self.more_than_two_repeat_pattern, r"\1\1", word)
+
+                if (no_repeat in self.words) != (two_repeat in self.words):
+                    r = no_repeat if no_repeat in self.words else two_repeat
+                    text = text.replace(word, r)
+                else:
+                    text = text.replace(word, two_repeat)
+
+        return text
+
+    def persian_style(self: "Normalizer", text: str) -> str:
+        """برخی از حروف و نشانه‌ها را با حروف و نشانه‌های فارسی جایگزین می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.persian_style('"نرمال‌سازی"')
+            '«نرمال‌سازی»'
+            >>> normalizer.persian_style('و ...')
+            'و …'
+            >>> normalizer.persian_style('10.450')
+            '10٫450'
+            >>> normalizer.persian_style('')
+            ''
+
+        Args:
+            text: متنی که باید حروف و نشانه‌های آن با حروف و نشانه‌های فارسی جایگزین شود.
+
+        Returns:
+            متنی با حروف و نشانه‌های فارسی‌سازی شده.
+
+        """
+        return regex_replace(self.persian_style_patterns, text)
+
+    def persian_number(self: "Normalizer", text: str) -> str:
+        """اعداد لاتین و علامت % را با معادل فارسی آن جایگزین می‌کند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.persian_number('5 درصد')
+            '۵ درصد'
+            >>> normalizer.persian_number('۵ درصد')
+            '۵ درصد'
+            >>> normalizer.persian_number('')
+            ''
+
+        Args:
+            text: متنی که باید اعداد لاتین و علامت % آن با معادل فارسی جایگزین شود.
+
+        Returns:
+            متنی با اعداد و علامت ٪ فارسی.
+
+        """
+        translations = maketrans(
+            self.number_translation_src,
+            self.number_translation_dst,
+        )
+        return text.translate(translations)
+
+    def unicodes_replacement(self: "Normalizer", text: str) -> str:
+        """برخی از کاراکترهای خاص یونیکد را با معادلِ نرمال آن جایگزین می‌کند. غالباً
+        این کار فقط در مواردی صورت می‌گیرد که یک کلمه در قالب یک کاراکتر یونیکد تعریف
+        شده است.
+
+        **فهرست این کاراکترها و نسخهٔ جایگزین آن:**
+
+        |کاراکتر|نسخهٔ جایگزین|
+        |--------|------------------|
+        |﷽|بسم الله الرحمن الرحیم|
+        |﷼|ریال|
+        |ﷰ، ﷹ|صلی|
+        |ﷲ|الله|
+        |ﷳ|اکبر|
+        |ﷴ|محمد|
+        |ﷵ|صلعم|
+        |ﷶ|رسول|
+        |ﷷ|علیه|
+        |ﷸ|وسلم|
+        |ﻵ، ﻶ، ﻷ، ﻸ، ﻹ، ﻺ، ﻻ، ﻼ|لا|
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.remove_specials_chars('پیامبر اکرم ﷺ')
+            'پیامبر اکرم '
+            >>> normalizer.remove_specials_chars('')
+            ''
+
+        Args:
+            text: متنی که باید برخی از کاراکترهای یونیکد آن (جدول بالا)، با شکل استاندارد، جایگزین شود.
+
+        Returns:
+            متنی که برخی از کاراکترهای یونیکد آن با شکل استاندارد جایگزین شده است.
+
+        """
+        for old, new in self.replacements:
+            text = re.sub(old, new, text)
+
+        return text
+
+    def seperate_mi(self: "Normalizer", text: str) -> str:
+        """پیشوند «می» و «نمی» را در افعال جدا کرده و با نیم‌فاصله می‌چسباند.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.seperate_mi('نمیدانم چه میگفت')
+            'نمی‌دانم چه می‌گفت'
+            >>> normalizer.seperate_mi('میز')
+            'میز'
+            >>> normalizer.seperate_mi('')
+            ''
+
+
+        Args:
+            text: متنی که باید پیشوند «می» و «نمی» در آن جدا شود.
+
+        Returns:
+            متنی با «می» و «نمی» جدا شده.
+
+        """
+        matches = re.findall(r"\bن?می[آابپتثجچحخدذرزژسشصضطظعغفقکگلمنوهی]+", text)
+        for m in matches:
+            r = re.sub("^(ن?می)", r"\1‌", m)
+            if r in self.verbs:
+                text = text.replace(m, r)
+
+        return text
+
+    def token_spacing(self: "Normalizer", tokens: List[str]) -> List[str]:
+        """توکن‌های ورودی را به فهرستی از توکن‌های نرمال‌سازی شده تبدیل می‌کند.
+        در این فرایند ممکن است برخی از توکن‌ها به یکدیگر بچسبند؛
+        برای مثال: `['زمین', 'لرزه', 'ای']` تبدیل می‌شود به: `['زمین‌لرزه‌ای']`.
+
+        Examples:
+            >>> normalizer = Normalizer()
+            >>> normalizer.token_spacing(['کتاب', 'ها'])
+            ['کتاب‌ها']
+            >>> normalizer.token_spacing(['او', 'می', 'رود'])
+            ['او', 'می‌رود']
+            >>> normalizer.token_spacing(['ماه', 'می', 'سال', 'جدید'])
+            ['ماه', 'می', 'سال', 'جدید']
+            >>> normalizer.token_spacing(['اخلال', 'گر'])
+            ['اخلال‌گر']
+            >>> normalizer.token_spacing(['زمین', 'لرزه', 'ای'])
+            ['زمین‌لرزه‌ای']
+            >>> normalizer.token_spacing([])
+            []
+
+        Args:
+            tokens: توکن‌هایی که باید نرمال‌سازی شود.
+
+        Returns:
+            لیستی از توکن‌های نرمال‌سازی شده به شکل `[token1, token2, ...]`.
+
+        """
+        # >>> normalizer.token_spacing(['پرداخت', 'شده', 'است'])
+
+        result = []
+        for t, token in enumerate(tokens):
+            joined = False
+
+            if result:
+                token_pair = result[-1] + "‌" + token
+                if (
+                    token_pair in self.verbs
+                    or token_pair in self.words
+                    and self.words[token_pair][0] > 0
+                ):
+                    joined = True
+
+                    if (
+                        t < len(tokens) - 1
+                        and token + "_" + tokens[t + 1] in self.verbs
+                    ):
+                        joined = False
+
+                elif token in self.suffixes and result[-1] in self.words:
+                    joined = True
+
+            if joined:
+                result.pop()
+                result.append(token_pair)
+            else:
+                result.append(token)
+
+        return result
```

### Comparing `hazm-0.9.1/hazm/pos_tagger.py` & `hazm-0.9.2/hazm/pos_tagger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای برچسب‌گذاری توکن‌هاست.
-
- **میزان دقت
-برچسب‌زنی در نسخهٔ حاضر ۹۷.۲ درصد [^1] است.**
-[^1]:
-این عدد با انتشار هر نسخه بروزرسانی می‌شود.
-
-"""
-
-from nltk.tag import stanford
-
-from hazm import SequenceTagger
-
-punctuation_list = [
-    '"',
-    "#",
-    "(",
-    ")",
-    "*",
-    ",",
-    "-",
-    ".",
-    "/",
-    ":",
-    "[",
-    "]",
-    "«",
-    "»",
-    "،",
-    ";",
-    "?",
-    "!",
-]
-
-
-class POSTagger(SequenceTagger):
-    """این کلاس‌ها شامل توابعی برای برچسب‌گذاری توکن‌هاست. **میزان دقت برچسب‌زنی در
-    نسخهٔ حاضر ۹۷.۲ درصد [^1] است.** این کلاس تمام توابع خود را از کلاس
-    [SequenceTagger][hazm.sequence_tagger.SequenceTagger] به ارث می‌برد.
-    [^1]:
-    این عدد با انتشار هر نسخه بروزرسانی می‌شود.
-
-    """
-
-    def __init__(
-        self: "POSTagger", model=None, data_maker=None, universal_tag=False,
-    ) -> None:
-        data_maker = self.data_maker if data_maker is None else data_maker
-        self.__is_universal = universal_tag
-        super().__init__(model, data_maker)
-
-    def __universal_converter(self: "POSTagger", tagged_list):
-        return [(word, tag.split(",")[0]) for word, tag in tagged_list]
-
-    def __is_punc(self: "POSTagger", word):
-        return word in punctuation_list
-
-    def data_maker(self: "POSTagger", tokens):
-        """تابعی که لیستی از لیستی از کلمات توکنایز شده را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
-
-        Examples:
-            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model')
-            >>> posTagger.data_maker(tokens = [['دلم', 'اینجا', 'مانده‌است', '.']])
-            [[{'word': 'دلم', 'is_first': True, 'is_last': False, 'prefix-1': 'د', 'prefix-2': 'دل', 'prefix-3': 'دلم', 'suffix-1': 'م', 'suffix-2': 'لم', 'suffix-3': 'دلم', 'prev_word': '', 'two_prev_word': '', 'next_word': 'اینجا', 'two_next_word': 'مانده\u200cاست', 'is_numeric': False, 'prev_is_numeric': '', 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': '', 'next_is_punc': False}, {'word': 'اینجا', 'is_first': False, 'is_last': False, 'prefix-1': 'ا', 'prefix-2': 'ای', 'prefix-3': 'این', 'suffix-1': 'ا', 'suffix-2': 'جا', 'suffix-3': 'نجا', 'prev_word': 'دلم', 'two_prev_word': '.', 'next_word': 'مانده\u200cاست', 'two_next_word': '.', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False}, {'word': 'مانده\u200cاست', 'is_first': False, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'ما', 'prefix-3': 'مان', 'suffix-1': 'ت', 'suffix-2': 'ست', 'suffix-3': 'است', 'prev_word': 'اینجا', 'two_prev_word': 'دلم', 'next_word': '.', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': True}, {'word': '.', 'is_first': False, 'is_last': True, 'prefix-1': '.', 'prefix-2': '.', 'prefix-3': '.', 'suffix-1': '.', 'suffix-2': '.', 'suffix-3': '.', 'prev_word': 'مانده\u200cاست', 'two_prev_word': 'اینجا', 'next_word': '', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': '', 'is_punc': True, 'prev_is_punc': False, 'next_is_punc': ''}]]
-
-        Args:
-            tokens (List[List[str]]): جملاتی که نیاز به تبدیل آن به برداری از ویژگی‌ها است.
-
-        Returns:
-            List(List(Dict())): لیستی از لیستی از دیکشنری‌های بیان‌کننده ویژگی‌های یک کلمه.
-        """
-        return [
-            [self.features(token, index) for index in range(len(token))]
-            for token in tokens
-        ]
-
-    def features(self: "POSTagger", sentence, index):
-        """features."""
-        return {
-            "word": sentence[index],
-            "is_first": index == 0,
-            "is_last": index == len(sentence) - 1,
-            # *ix
-            "prefix-1": sentence[index][0],
-            "prefix-2": sentence[index][:2],
-            "prefix-3": sentence[index][:3],
-            "suffix-1": sentence[index][-1],
-            "suffix-2": sentence[index][-2:],
-            "suffix-3": sentence[index][-3:],
-            # word
-            "prev_word": "" if index == 0 else sentence[index - 1],
-            "two_prev_word": "" if index == 0 else sentence[index - 2],
-            "next_word": "" if index == len(sentence) - 1 else sentence[index + 1],
-            "two_next_word": (
-                ""
-                if (index == len(sentence) - 1 or index == len(sentence) - 2)
-                else sentence[index + 2]
-            ),
-            # digit
-            "is_numeric": sentence[index].isdigit(),
-            "prev_is_numeric": "" if index == 0 else sentence[index - 1].isdigit(),
-            "next_is_numeric": (
-                "" if index == len(sentence) - 1 else sentence[index + 1].isdigit()
-            ),
-            # punc
-            "is_punc": self.__is_punc(sentence[index]),
-            "prev_is_punc": "" if index == 0 else self.__is_punc(sentence[index - 1]),
-            "next_is_punc": (
-                ""
-                if index == len(sentence) - 1
-                else self.__is_punc(sentence[index + 1])
-            ),
-        }
-
-    def tag(self: "POSTagger", tokens):
-        """یک جمله را در قالب لیستی از توکن‌ها دریافت می‌کند و در خروجی لیستی از
-        `(توکن، برچسب)`ها برمی‌گرداند.
-
-        Examples:
-            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model')
-            >>> posTagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
-            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
-
-            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model', universal_tag = True)
-            >>> posTagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
-            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
-
-        Args:
-            tokens (List[str]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[Tuple[str,str]]): ‌لیستی از `(توکن، برچسب)`ها.
-
-        """
-        tagged_token = super().tag(tokens)
-        return (
-            self.__universal_converter(tagged_token)
-            if self.__is_universal
-            else tagged_token
-        )
-
-    def tag_sents(self: "POSTagger", sentences):
-        """جملات را در قالب لیستی از توکن‌ها دریافت می‌کند
-        و در خروجی، لیستی از لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
-
-        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
-
-        Examples:
-            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model')
-            >>> posTagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
-            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
-
-            >>> posTagger = POSTagger(model = 'resources/pos_tagger.model', universal_tag = True)
-            >>> posTagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
-            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
-
-        Args:
-            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، برچسب)`ها.
-                    هر لیست از `(توکن،برچسب)`ها مربوط به یک جمله است.
-
-        """
-        tagged_sents = super().tag_sents(sentences)
-        return (
-            [self.__universal_converter(tagged_sent) for tagged_sent in tagged_sents]
-            if self.__is_universal
-            else tagged_sents
-        )
-
-
-class StanfordPOSTagger(stanford.StanfordPOSTagger):
-    """StanfordPOSTagger."""
-
-    def __init__(
-        self: "StanfordPOSTagger",
-        model_filename: "str",
-        path_to_jar: str,
-        *args,
-        **kwargs,
-    ) -> None:
-        self._SEPARATOR = "/"
-        super(stanford.StanfordPOSTagger, self).__init__(
-            model_filename=model_filename,
-            path_to_jar=path_to_jar,
-            *args,  # noqa: B026
-            **kwargs,
-        )
-
-    def tag(self: "StanfordPOSTagger", tokens):
-        """tag.
-
-        Examples:
-            >>> tagger = StanfordPOSTagger(model_filename='resources/persian.tagger', path_to_jar='resources/stanford_postagger.jar')
-            >>> tagger.tag(['من', 'به', 'مدرسه', 'رفته_بودم', '.'])
-            [('من', 'PRO'), ('به', 'P'), ('مدرسه', 'N'), ('رفته_بودم', 'V'), ('.', 'PUNC')]
-
-        """
-        return self.tag_sents([tokens])[0]
-
-    def tag_sents(self: "StanfordPOSTagger", sentences):
-        """tag_sents."""
-        refined = ([w.replace(" ", "_") for w in s] for s in sentences)
-        return super(stanford.StanfordPOSTagger, self).tag_sents(refined)
+"""این ماژول شامل کلاس‌ها و توابعی برای برچسب‌گذاری توکن‌هاست.
+
+ **میزان دقت
+برچسب‌زنی در نسخهٔ حاضر ۹۷.۲ درصد [^1] است.**
+[^1]:
+این عدد با انتشار هر نسخه بروزرسانی می‌شود.
+
+"""
+
+from nltk.tag import stanford
+
+from hazm import SequenceTagger
+
+punctuation_list = [
+    '"',
+    "#",
+    "(",
+    ")",
+    "*",
+    ",",
+    "-",
+    ".",
+    "/",
+    ":",
+    "[",
+    "]",
+    "«",
+    "»",
+    "،",
+    ";",
+    "?",
+    "!",
+]
+
+
+class POSTagger(SequenceTagger):
+    """این کلاس‌ها شامل توابعی برای برچسب‌گذاری توکن‌هاست. **میزان دقت برچسب‌زنی در
+    نسخهٔ حاضر ۹۷.۲ درصد [^1] است.** این کلاس تمام توابع خود را از کلاس
+    [SequenceTagger][hazm.sequence_tagger.SequenceTagger] به ارث می‌برد.
+    [^1]:
+    این عدد با انتشار هر نسخه بروزرسانی می‌شود.
+
+    """
+
+    def __init__(
+        self: "POSTagger", model=None, data_maker=None, universal_tag=False,
+    ) -> None:
+        data_maker = self.data_maker if data_maker is None else data_maker
+        self.__is_universal = universal_tag
+        super().__init__(model, data_maker)
+
+    def __universal_converter(self: "POSTagger", tagged_list):
+        return [(word, tag.split(",")[0]) for word, tag in tagged_list]
+
+    def __is_punc(self: "POSTagger", word):
+        return word in punctuation_list
+
+    def data_maker(self: "POSTagger", tokens):
+        """تابعی که لیستی از لیستی از کلمات توکنایز شده را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
+
+        Examples:
+            >>> posTagger = POSTagger(model = 'pos_tagger.model')
+            >>> posTagger.data_maker(tokens = [['دلم', 'اینجا', 'مانده‌است', '.']])
+            [[{'word': 'دلم', 'is_first': True, 'is_last': False, 'prefix-1': 'د', 'prefix-2': 'دل', 'prefix-3': 'دلم', 'suffix-1': 'م', 'suffix-2': 'لم', 'suffix-3': 'دلم', 'prev_word': '', 'two_prev_word': '', 'next_word': 'اینجا', 'two_next_word': 'مانده\u200cاست', 'is_numeric': False, 'prev_is_numeric': '', 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': '', 'next_is_punc': False}, {'word': 'اینجا', 'is_first': False, 'is_last': False, 'prefix-1': 'ا', 'prefix-2': 'ای', 'prefix-3': 'این', 'suffix-1': 'ا', 'suffix-2': 'جا', 'suffix-3': 'نجا', 'prev_word': 'دلم', 'two_prev_word': '.', 'next_word': 'مانده\u200cاست', 'two_next_word': '.', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': False}, {'word': 'مانده\u200cاست', 'is_first': False, 'is_last': False, 'prefix-1': 'م', 'prefix-2': 'ما', 'prefix-3': 'مان', 'suffix-1': 'ت', 'suffix-2': 'ست', 'suffix-3': 'است', 'prev_word': 'اینجا', 'two_prev_word': 'دلم', 'next_word': '.', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': False, 'is_punc': False, 'prev_is_punc': False, 'next_is_punc': True}, {'word': '.', 'is_first': False, 'is_last': True, 'prefix-1': '.', 'prefix-2': '.', 'prefix-3': '.', 'suffix-1': '.', 'suffix-2': '.', 'suffix-3': '.', 'prev_word': 'مانده\u200cاست', 'two_prev_word': 'اینجا', 'next_word': '', 'two_next_word': '', 'is_numeric': False, 'prev_is_numeric': False, 'next_is_numeric': '', 'is_punc': True, 'prev_is_punc': False, 'next_is_punc': ''}]]
+
+        Args:
+            tokens (List[List[str]]): جملاتی که نیاز به تبدیل آن به برداری از ویژگی‌ها است.
+
+        Returns:
+            List(List(Dict())): لیستی از لیستی از دیکشنری‌های بیان‌کننده ویژگی‌های یک کلمه.
+        """
+        return [
+            [self.features(token, index) for index in range(len(token))]
+            for token in tokens
+        ]
+
+    def features(self: "POSTagger", sentence, index):
+        """features."""
+        return {
+            "word": sentence[index],
+            "is_first": index == 0,
+            "is_last": index == len(sentence) - 1,
+            # *ix
+            "prefix-1": sentence[index][0],
+            "prefix-2": sentence[index][:2],
+            "prefix-3": sentence[index][:3],
+            "suffix-1": sentence[index][-1],
+            "suffix-2": sentence[index][-2:],
+            "suffix-3": sentence[index][-3:],
+            # word
+            "prev_word": "" if index == 0 else sentence[index - 1],
+            "two_prev_word": "" if index == 0 else sentence[index - 2],
+            "next_word": "" if index == len(sentence) - 1 else sentence[index + 1],
+            "two_next_word": (
+                ""
+                if (index == len(sentence) - 1 or index == len(sentence) - 2)
+                else sentence[index + 2]
+            ),
+            # digit
+            "is_numeric": sentence[index].isdigit(),
+            "prev_is_numeric": "" if index == 0 else sentence[index - 1].isdigit(),
+            "next_is_numeric": (
+                "" if index == len(sentence) - 1 else sentence[index + 1].isdigit()
+            ),
+            # punc
+            "is_punc": self.__is_punc(sentence[index]),
+            "prev_is_punc": "" if index == 0 else self.__is_punc(sentence[index - 1]),
+            "next_is_punc": (
+                ""
+                if index == len(sentence) - 1
+                else self.__is_punc(sentence[index + 1])
+            ),
+        }
+
+    def tag(self: "POSTagger", tokens):
+        """یک جمله را در قالب لیستی از توکن‌ها دریافت می‌کند و در خروجی لیستی از
+        `(توکن، برچسب)`ها برمی‌گرداند.
+
+        Examples:
+            >>> posTagger = POSTagger(model = 'pos_tagger.model')
+            >>> posTagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
+            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
+
+            >>> posTagger = POSTagger(model = 'pos_tagger.model', universal_tag = True)
+            >>> posTagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
+            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
+
+        Args:
+            tokens (List[str]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[Tuple[str,str]]): ‌لیستی از `(توکن، برچسب)`ها.
+
+        """
+        tagged_token = super().tag(tokens)
+        return (
+            self.__universal_converter(tagged_token)
+            if self.__is_universal
+            else tagged_token
+        )
+
+    def tag_sents(self: "POSTagger", sentences):
+        """جملات را در قالب لیستی از توکن‌ها دریافت می‌کند
+        و در خروجی، لیستی از لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
+
+        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
+
+        Examples:
+            >>> posTagger = POSTagger(model = 'pos_tagger.model')
+            >>> posTagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
+            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
+
+            >>> posTagger = POSTagger(model = 'pos_tagger.model', universal_tag = True)
+            >>> posTagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
+            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
+
+        Args:
+            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، برچسب)`ها.
+                    هر لیست از `(توکن،برچسب)`ها مربوط به یک جمله است.
+
+        """
+        tagged_sents = super().tag_sents(sentences)
+        return (
+            [self.__universal_converter(tagged_sent) for tagged_sent in tagged_sents]
+            if self.__is_universal
+            else tagged_sents
+        )
+
+
+class StanfordPOSTagger(stanford.StanfordPOSTagger):
+    """StanfordPOSTagger."""
+
+    def __init__(
+        self: "StanfordPOSTagger",
+        model_filename: "str",
+        path_to_jar: str,
+        *args, # noqa: ANN002
+        **kwargs, # noqa: ANN003
+    ) -> None:
+        self._SEPARATOR = "/"
+        super(stanford.StanfordPOSTagger, self).__init__(
+            model_filename=model_filename,
+            path_to_jar=path_to_jar,
+            *args,  # noqa: B026
+            **kwargs,
+        )
+
+    def tag(self: "StanfordPOSTagger", tokens):
+        """tag.
+
+        Examples:
+            >>> tagger = StanfordPOSTagger(model_filename='persian.tagger', path_to_jar='stanford_postagger.jar')
+            >>> tagger.tag(['من', 'به', 'مدرسه', 'رفته_بودم', '.'])
+            [('من', 'PRO'), ('به', 'P'), ('مدرسه', 'N'), ('رفته_بودم', 'V'), ('.', 'PUNC')]
+
+        """
+        return self.tag_sents([tokens])[0]
+
+    def tag_sents(self: "StanfordPOSTagger", sentences):
+        """tag_sents."""
+        refined = ([w.replace(" ", "_") for w in s] for s in sentences)
+        return super(stanford.StanfordPOSTagger, self).tag_sents(refined)
```

### Comparing `hazm-0.9.1/hazm/sentence_tokenizer.py` & `hazm-0.9.2/hazm/sentence_tokenizer.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای استخراج جملاتِ متن است.
-
-برای استخراج کلمات از تابع [WordTokenizer()][hazm.WordTokenizer] استفاده کنید.
-
-"""
-
-
-import re
-from typing import List
-
-from nltk.tokenize.api import TokenizerI
-
-
-class SentenceTokenizer(TokenizerI):
-    """این کلاس شامل توابعی برای استخراج جملاتِ متن است."""
-
-    def __init__(self: "SentenceTokenizer") -> None:
-        self.pattern = re.compile(r"([!.?⸮؟]+)[ \n]+")
-
-    def tokenize(self: "SentenceTokenizer", text: str) -> List[str]:
-        """متن ورودی را به جملات سازندهٔ آن می‌شِکند.
-
-        Examples:
-            >>> tokenizer = SentenceTokenizer()
-            >>> tokenizer.tokenize('جدا کردن ساده است. تقریبا البته!')
-            ['جدا کردن ساده است.', 'تقریبا البته!']
-
-        Args:
-            text: متنی که باید جملات آن استخراج شود.
-
-        Returns:
-            فهرست جملات استخراج‌شده.
-
-        """
-        text = self.pattern.sub(r"\1\n\n", text)
-        return [
-            sentence.replace("\n", " ").strip()
-            for sentence in text.split("\n\n")
-            if sentence.strip()
-        ]
+"""این ماژول شامل کلاس‌ها و توابعی برای استخراج جملاتِ متن است.
+
+برای استخراج کلمات از تابع [WordTokenizer()][hazm.WordTokenizer] استفاده کنید.
+
+"""
+
+
+import re
+from typing import List
+
+from nltk.tokenize.api import TokenizerI
+
+
+class SentenceTokenizer(TokenizerI):
+    """این کلاس شامل توابعی برای استخراج جملاتِ متن است."""
+
+    def __init__(self: "SentenceTokenizer") -> None:
+        self.pattern = re.compile(r"([!.?⸮؟]+)[ \n]+")
+
+    def tokenize(self: "SentenceTokenizer", text: str) -> List[str]:
+        """متن ورودی را به جملات سازندهٔ آن می‌شِکند.
+
+        Examples:
+            >>> tokenizer = SentenceTokenizer()
+            >>> tokenizer.tokenize('جدا کردن ساده است. تقریبا البته!')
+            ['جدا کردن ساده است.', 'تقریبا البته!']
+
+        Args:
+            text: متنی که باید جملات آن استخراج شود.
+
+        Returns:
+            فهرست جملات استخراج‌شده.
+
+        """
+        text = self.pattern.sub(r"\1\n\n", text)
+        return [
+            sentence.replace("\n", " ").strip()
+            for sentence in text.split("\n\n")
+            if sentence.strip()
+        ]
```

### Comparing `hazm-0.9.1/hazm/sequence_tagger.py` & `hazm-0.9.2/hazm/sequence_tagger.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,411 +1,411 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای برچسب‌گذاری توکن‌هاست."""
-
-import time
-from typing import List
-from typing import Tuple
-
-import numpy as np
-from pycrfsuite import Tagger
-from pycrfsuite import Trainer
-from sklearn.metrics import accuracy_score
-
-
-def features(sent, index):
-    """فهرست فیچرها را برمی‌گرداند."""
-    return {
-        "word": sent[index],
-        "is_first": index == 0,
-        "is_last": index == len(sent),
-        "is_num": sent[index].isdigit(),
-        "prev_word": sent[index - 1] if index != 0 else "",
-        "next_word": sent[index + 1] if index != len(sent) - 1 else "",
-    }
-
-
-def data_maker(tokens):
-    """تابع دیتا میکر."""
-    return [[features(sent, index) for index in range(len(sent))] for sent in tokens]
-
-
-def iob_features(words, pos_tags, index):
-    """تابع iob_features."""
-    word_features = features(words, index)
-    word_features.update(
-        {
-            "pos": pos_tags[index],
-            "prev_pos": "" if index == 0 else pos_tags[index - 1],
-            "next_pos": "" if index == len(pos_tags) - 1 else pos_tags[index + 1],
-        },
-    )
-    return word_features
-
-
-def iob_data_maker(tokens):
-    """تابع iob_data_maker."""
-    words = [[word for word, _ in token] for token in tokens]
-    tags = [[tag for _, tag in token] for token in tokens]
-    return [
-        [
-            iob_features(words=word_tokens, pos_taggs=tag_tokens, index=index)
-            for index in range(len(word_tokens))
-        ]
-        for word_tokens, tag_tokens in zip(words, tags)
-    ]
-
-
-class SequenceTagger:
-    """این کلاس شامل توابعی برای برچسب‌گذاری توکن‌ها است. این کلاس در نقش یک
-    wrapper برای کتابخانهٔ [python-crfsuite](https://python-crfsuite.readthedocs.io/en/latest/) است.
-
-    Args:
-        model (str, optional): مسیر فایل tagger.
-        data_maker (function, optional): تابعی که لیستی دو بعدی از کلمات توکنایز شده را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
-    """
-
-    def __init__(self: "SequenceTagger", model=None, data_maker=data_maker) -> None:
-        if model is not None:
-            self.load_model(model)
-        else:
-            self.model = None
-        self.data_maker = data_maker
-
-    def __add_label(self: "SequenceTagger", sentence, tags):
-        return [(word, tag) for word, tag in zip(sentence, tags)]
-
-    def __tag(self: "SequenceTagger", tokens):
-        return self.__add_label(tokens, self.model.tag(self.data_maker([tokens])[0]))
-
-    def __train(
-        self: "SequenceTagger", x, y, args, verbose, file_name, report_duration,
-    ):
-        trainer = Trainer(verbose=verbose)
-        trainer.set_params(args)
-
-        for xseq, yseq in zip(x, y):
-            trainer.append(xseq, yseq)
-
-        start_time = time.time()
-        trainer.train(file_name)
-        end_time = time.time()
-
-        if report_duration:
-            print(f"training time: {(end_time - start_time):.2f} sec")
-
-        self.load_model(file_name)
-
-    def __evaluate(self: "SequenceTagger", gold_labels, predicted_labels):
-        gold_labels = np.concatenate(gold_labels)
-        predicted_labels = np.concatenate(predicted_labels)
-        return float(accuracy_score(gold_labels, predicted_labels))
-
-    def load_model(self: "SequenceTagger", model):
-        """فایل تگر را بارگزاری می‌کند.
-
-        Examples:
-            >>> tagger = SequenceTagger()
-            >>> tagger.load_model(model = 'tagger.model')
-
-        Args:
-            model (str): مسیر فایل تگر.
-
-        """
-        tagger = Tagger()
-        tagger.open(model)
-        self.model = tagger
-
-    def tag(self: "SequenceTagger", tokens):
-        """یک جمله را در قالب لیستی از توکن‌ها دریافت می‌کند و در خروجی لیستی از
-        `(توکن، برچسب)`ها برمی‌گرداند.
-
-        Examples:
-            >>> tagger = SequenceTagger(model = 'tagger.model')
-            >>> tagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
-            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
-
-        Args:
-            tokens (List[str]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[Tuple[str,str]]): ‌لیستی از `(توکن، برچسب)`ها.
-
-        """
-        if self.model is None:
-            msg = "you should load model first..."
-            raise ValueError(msg)
-
-        return self.__tag(tokens)
-
-    def tag_sents(self: "SequenceTagger", sentences):
-        """جملات را در قالب لیستی از توکن‌ها دریافت می‌کند
-        و در خروجی، لیستی از لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
-
-        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
-
-        Examples:
-            >>> tagger = SequenceTagger(model = 'tagger.model')
-            >>> tagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
-            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
-
-        Args:
-            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، برچسب)`ها.
-                    هر لیست از `(توکن،برچسب)`ها مربوط به یک جمله است.
-
-        """
-        if self.model is None:
-            msg = "you should load model first..."
-            raise ValueError(msg)
-
-        return [self.__tag(tokens) for tokens in sentences]
-
-    def train(
-        self: "SequenceTagger",
-        tagged_list,
-        c1=0.4,
-        c2=0.04,
-        max_iteration=400,
-        verbose=True,
-        file_name="crf.model",
-        report_duration=True,
-    ):
-        """لیستی از جملات را می‌گیرد و بر اساس آن مدل را آموزش می‌دهد.
-
-        هر جمله، لیستی از `(توکن، برچسب)`هاست.
-
-        Examples:
-            >>> tagger = SequenceTagger()
-            >>> tagger.train(tagged_list = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'tagger.model', report_duration = True)
-            Feature generation
-            type: CRF1d
-            feature.minfreq: 0.000000
-            feature.possible_states: 0
-            feature.possible_transitions: 1
-            0....1....2....3....4....5....6....7....8....9....10
-            Number of features: 150
-            Seconds required: 0.001
-            ...
-            Writing feature references for attributes
-            Seconds required: 0.000
-
-            training time: 0.01 sec
-
-        Args:
-            tagged_list (List[{List[Tuple[str,str]]]): جملاتی که مدل از روی آن‌ها آموزش می‌بیند.
-            c1 (float): مقدار L1 regularization.
-            c2 (float): مقدار L2 regularization.
-            max_iteration (int): تعداد تکرار آموزش بر کل دیتا.
-            verbose (boolean): نمایش اطلاعات مربوط به آموزش.
-            file_name (str): نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
-            report_duration (boolean): نمایش گزارشات مربوط به زمان.
-
-        """
-        x = self.data_maker(
-            [[x for x, _ in tagged_sent] for tagged_sent in tagged_list],
-        )
-        y = [[y for _, y in tagged_sent] for tagged_sent in tagged_list]
-
-        args = {
-            "c1": c1,
-            "c2": c2,
-            "max_iterations": max_iteration,
-            "feature.possible_transitions": True,
-        }
-
-        self.__train(x, y, args, verbose, file_name, report_duration)
-
-    def save_model(self: "SequenceTagger", filename):
-        """مدل تهیه‌شده توسط تابع [train()][hazm.sequence_tagger.SequenceTagger.train]
-        را ذخیره می‌کند.
-
-        Examples:
-            >>> tagger = SequenceTagger()
-            >>> tagger.train(tagged_list = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'tagger.model', report_duration = True)
-            >>> tagger.save_model(file_name = 'new_tagger.model')
-
-        Args:
-            filename (str): نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
-
-        """
-        if self.model is None:
-            msg = "you should load model first..."
-            raise ValueError(msg)
-
-        self.model.dump(filename)
-
-    def evaluate(
-        self: "SequenceTagger", tagged_sent: List[List[Tuple[str, str]]],
-    ) -> float:
-        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
-
-        Examples:
-            >>> tagger = SequenceTagger(model = 'tagger.model')
-            >>> tagger.evaluate([[('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')]])
-            1.0
-
-
-        Args:
-            tagged_sent: جملات لیبل‌داری که با استفاده از آن مدل را ارزیابی می‌کنیم.
-
-        Returns:
-            دقت مدل
-
-        """
-        if self.model is None:
-            msg = "you should load model first..."
-            raise ValueError(msg)
-
-        def extract_labels(tagged_list):
-            return [[label for _, label in sent] for sent in tagged_list]
-
-        tokens = [[word for word, _ in sent] for sent in tagged_sent]
-        predicted_tagged_sent = self.tag_sents(tokens)
-        return self.__evaluate(
-            extract_labels(tagged_sent),
-            extract_labels(predicted_tagged_sent),
-        )
-
-
-class IOBTagger(SequenceTagger):
-    """IOBTagger."""
-
-    def __init__(self: "SequenceTagger", model=None, data_maker=iob_data_maker) -> None:
-        super().__init__(model, data_maker)
-
-    def __iob_format(self: "SequenceTagger", tagged_data, chunk_tags):
-        return [
-            (token[0], token[1], chunk_tag[1])
-            for token, chunk_tag in zip(tagged_data, chunk_tags)
-        ]
-
-    def tag(self: "SequenceTagger", tagged_data):
-        """یک جمله را در قالب لیستی از توکن‌ها و تگ‌ها دریافت می‌کند و در خروجی لیستی از
-        `(توکن، تگ، برچسب)`ها برمی‌گرداند.
-
-        Examples:
-            >>> iobTagger = IOBTagger(model = 'tagger.model')
-            >>> iobTagger.tag(tagged_data = [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')])
-            [('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]
-
-        Args:
-            tagged_data (List[Tuple[str, str]]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[Tuple[str, str, str]]): ‌لیستی از `(توکن، تگ، برچسب)`ها.
-
-        """
-        chunk_tags = super().tag(tagged_data)
-        return self.__iob_format(tagged_data, chunk_tags)
-
-    def tag_sents(self: "SequenceTagger", sentences):
-        """جملات را در قالب لیستی لیستی از توکن‌ها و تگ‌ها دریافت می‌کند
-        و در خروجی، لیستی از لیستی از `(توکن، تگ، برچسب)`ها برمی‌گرداند.
-
-        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
-
-        Examples:
-            >>> iobTagger = IOBTagger(model = 'tagger.model')
-            >>> iobTagger.tag_sents(tagged_data = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]])
-            [[('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]]
-
-        Args:
-            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
-
-        Returns:
-            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، تگ، برچسب)`ها.
-                    هر لیست از `(توکن، تگ، برچسب)`ها مربوط به یک جمله است.
-
-        """
-        chunk_tags = super().tag_sents(sentences)
-        return [
-            self.__iob_format(tagged_data, chunks)
-            for tagged_data, chunks in zip(sentences, chunk_tags)
-        ]
-
-    def train(
-        self: "SequenceTagger",
-        tagged_list: List[List[Tuple[str, str, str]]],
-        c1: float = 0.4,
-        c2: float = 0.04,
-        max_iteration: int = 400,
-        verbose: True = True,
-        file_name: str = "crf.model",
-        report_duration=True,
-    ):
-        """لیستی از جملات را می‌گیرد و بر اساس آن مدل را آموزش می‌دهد.
-
-        هر جمله، لیستی از `(توکن، تگ، برچسب)`هاست.
-
-        Examples:
-            >>> iobTagger = IOBTagger()
-            >>> iobTagger.train(tagged_list = [[('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'newIOBTagger.model', report_duration = True)
-            Feature generation
-            type: CRF1d
-            feature.minfreq: 0.000000
-            feature.possible_states: 0
-            feature.possible_transitions: 1
-            0....1....2....3....4....5....6....7....8....9....10
-            Number of features: 150
-            Seconds required: 0.001
-            ...
-            Writing feature references for attributes
-            Seconds required: 0.000
-
-            training time: 0.01 sec
-
-        Args:
-            tagged_list: جملاتی که مدل از روی آن‌ها آموزش می‌بیند.
-            c1: مقدار L1 regularization.
-            c2: مقدار L2 regularization.
-            max_iteration: تعداد تکرار آموزش بر کل دیتا.
-            verbose: نمایش اطلاعات مربوط به آموزش.
-            file_name: نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
-            report_duration: نمایش گزارشات مربوط به زمان.
-
-        """
-        tagged_list = [
-            [((word, tag), chunk) for word, tag, chunk in tagged_sent]
-            for tagged_sent in tagged_list
-        ]
-        return super().train(
-            tagged_list,
-            c1,
-            c2,
-            max_iteration,
-            verbose,
-            file_name,
-            report_duration,
-        )
-
-    def evaluate(
-        self: "SequenceTagger", tagged_sent: List[List[Tuple[str, str, str]]],
-    ) -> float:
-        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
-
-        Examples:
-            >>> iobTagger = IOBTagger(model = 'tagger.model')
-            >>> iobTagger.evaluate([[('نامه', 'NOUN,EZ', 'B-NP'), ('ایشان', 'PRON', 'I-NP'), ('را', 'ADP', 'B-POSTP'), ('دریافت', 'NOUN', 'B-VP'), ('داشتم', 'VERB', 'I-VP'), ('.', 'PUNCT', 'O')]])
-            1.0
-
-
-        Args:
-            tagged_sent: جملات لیبل‌داری که با استفاده از آن مدل را ارزیابی می‌کنیم.
-
-        Returns:
-            دقت مدل
-
-        """
-        if self.model is None:
-            msg = "you should load model first..."
-            raise ValueError(msg)
-
-        def extract_labels(tagged_list):
-            return [[token[-1] for token in sent] for sent in tagged_list]
-
-        tokens = [[token[:-1] for token in sent] for sent in tagged_sent]
-        predicted_tagged_sent = self.tag_sents(tokens)
-        return super()._SequenceTagger__evaluate(
-            extract_labels(tagged_sent),
-            extract_labels(predicted_tagged_sent),
-        )
+"""این ماژول شامل کلاس‌ها و توابعی برای برچسب‌گذاری توکن‌هاست."""
+
+import time
+from typing import List
+from typing import Tuple
+
+import numpy as np
+from pycrfsuite import Tagger
+from pycrfsuite import Trainer
+from sklearn.metrics import accuracy_score
+
+
+def features(sent, index):
+    """فهرست فیچرها را برمی‌گرداند."""
+    return {
+        "word": sent[index],
+        "is_first": index == 0,
+        "is_last": index == len(sent),
+        "is_num": sent[index].isdigit(),
+        "prev_word": sent[index - 1] if index != 0 else "",
+        "next_word": sent[index + 1] if index != len(sent) - 1 else "",
+    }
+
+
+def data_maker(tokens):
+    """تابع دیتا میکر."""
+    return [[features(sent, index) for index in range(len(sent))] for sent in tokens]
+
+
+def iob_features(words, pos_tags, index):
+    """تابع iob_features."""
+    word_features = features(words, index)
+    word_features.update(
+        {
+            "pos": pos_tags[index],
+            "prev_pos": "" if index == 0 else pos_tags[index - 1],
+            "next_pos": "" if index == len(pos_tags) - 1 else pos_tags[index + 1],
+        },
+    )
+    return word_features
+
+
+def iob_data_maker(tokens):
+    """تابع iob_data_maker."""
+    words = [[word for word, _ in token] for token in tokens]
+    tags = [[tag for _, tag in token] for token in tokens]
+    return [
+        [
+            iob_features(words=word_tokens, pos_taggs=tag_tokens, index=index)
+            for index in range(len(word_tokens))
+        ]
+        for word_tokens, tag_tokens in zip(words, tags)
+    ]
+
+
+class SequenceTagger:
+    """این کلاس شامل توابعی برای برچسب‌گذاری توکن‌ها است. این کلاس در نقش یک
+    wrapper برای کتابخانهٔ [python-crfsuite](https://python-crfsuite.readthedocs.io/en/latest/) است.
+
+    Args:
+        model (str, optional): مسیر فایل tagger.
+        data_maker (function, optional): تابعی که لیستی دو بعدی از کلمات توکنایز شده را گرفته و لیست دو بعدی از از دیکشنری‌هایی که تعیین‌کننده ویژگی‌ها هر کلمه هستند را برمی‌گرداند.
+    """
+
+    def __init__(self: "SequenceTagger", model=None, data_maker=data_maker) -> None:
+        if model is not None:
+            self.load_model(model)
+        else:
+            self.model = None
+        self.data_maker = data_maker
+
+    def __add_label(self: "SequenceTagger", sentence, tags):
+        return [(word, tag) for word, tag in zip(sentence, tags)]
+
+    def __tag(self: "SequenceTagger", tokens):
+        return self.__add_label(tokens, self.model.tag(self.data_maker([tokens])[0]))
+
+    def __train(
+        self: "SequenceTagger", x, y, args, verbose, file_name, report_duration,
+    ):
+        trainer = Trainer(verbose=verbose)
+        trainer.set_params(args)
+
+        for xseq, yseq in zip(x, y):
+            trainer.append(xseq, yseq)
+
+        start_time = time.time()
+        trainer.train(file_name)
+        end_time = time.time()
+
+        if report_duration:
+            print(f"training time: {(end_time - start_time):.2f} sec")
+
+        self.load_model(file_name)
+
+    def __evaluate(self: "SequenceTagger", gold_labels, predicted_labels):
+        gold_labels = np.concatenate(gold_labels)
+        predicted_labels = np.concatenate(predicted_labels)
+        return float(accuracy_score(gold_labels, predicted_labels))
+
+    def load_model(self: "SequenceTagger", model):
+        """فایل تگر را بارگزاری می‌کند.
+
+        Examples:
+            >>> tagger = SequenceTagger()
+            >>> tagger.load_model(model = 'tagger.model')
+
+        Args:
+            model (str): مسیر فایل تگر.
+
+        """
+        tagger = Tagger()
+        tagger.open(model)
+        self.model = tagger
+
+    def tag(self: "SequenceTagger", tokens):
+        """یک جمله را در قالب لیستی از توکن‌ها دریافت می‌کند و در خروجی لیستی از
+        `(توکن، برچسب)`ها برمی‌گرداند.
+
+        Examples:
+            >>> tagger = SequenceTagger(model = 'tagger.model')
+            >>> tagger.tag(tokens = ['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.'])
+            [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]
+
+        Args:
+            tokens (List[str]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[Tuple[str,str]]): ‌لیستی از `(توکن، برچسب)`ها.
+
+        """
+        if self.model is None:
+            msg = "you should load model first..."
+            raise ValueError(msg)
+
+        return self.__tag(tokens)
+
+    def tag_sents(self: "SequenceTagger", sentences):
+        """جملات را در قالب لیستی از توکن‌ها دریافت می‌کند
+        و در خروجی، لیستی از لیستی از `(توکن، برچسب)`ها برمی‌گرداند.
+
+        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
+
+        Examples:
+            >>> tagger = SequenceTagger(model = 'tagger.model')
+            >>> tagger.tag_sents(sentences = [['من', 'به', 'مدرسه', 'ایران', 'رفته_بودم', '.']])
+            [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]]
+
+        Args:
+            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، برچسب)`ها.
+                    هر لیست از `(توکن،برچسب)`ها مربوط به یک جمله است.
+
+        """
+        if self.model is None:
+            msg = "you should load model first..."
+            raise ValueError(msg)
+
+        return [self.__tag(tokens) for tokens in sentences]
+
+    def train(
+        self: "SequenceTagger",
+        tagged_list,
+        c1=0.4,
+        c2=0.04,
+        max_iteration=400,
+        verbose=True,
+        file_name="crf.model",
+        report_duration=True,
+    ):
+        """لیستی از جملات را می‌گیرد و بر اساس آن مدل را آموزش می‌دهد.
+
+        هر جمله، لیستی از `(توکن، برچسب)`هاست.
+
+        Examples:
+            >>> tagger = SequenceTagger()
+            >>> tagger.train(tagged_list = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'tagger.model', report_duration = True)
+            Feature generation
+            type: CRF1d
+            feature.minfreq: 0.000000
+            feature.possible_states: 0
+            feature.possible_transitions: 1
+            0....1....2....3....4....5....6....7....8....9....10
+            Number of features: 150
+            Seconds required: 0.001
+            ...
+            Writing feature references for attributes
+            Seconds required: 0.000
+
+            training time: 0.01 sec
+
+        Args:
+            tagged_list (List[{List[Tuple[str,str]]]): جملاتی که مدل از روی آن‌ها آموزش می‌بیند.
+            c1 (float): مقدار L1 regularization.
+            c2 (float): مقدار L2 regularization.
+            max_iteration (int): تعداد تکرار آموزش بر کل دیتا.
+            verbose (boolean): نمایش اطلاعات مربوط به آموزش.
+            file_name (str): نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
+            report_duration (boolean): نمایش گزارشات مربوط به زمان.
+
+        """
+        x = self.data_maker(
+            [[x for x, _ in tagged_sent] for tagged_sent in tagged_list],
+        )
+        y = [[y for _, y in tagged_sent] for tagged_sent in tagged_list]
+
+        args = {
+            "c1": c1,
+            "c2": c2,
+            "max_iterations": max_iteration,
+            "feature.possible_transitions": True,
+        }
+
+        self.__train(x, y, args, verbose, file_name, report_duration)
+
+    def save_model(self: "SequenceTagger", filename):
+        """مدل تهیه‌شده توسط تابع [train()][hazm.sequence_tagger.SequenceTagger.train]
+        را ذخیره می‌کند.
+
+        Examples:
+            >>> tagger = SequenceTagger()
+            >>> tagger.train(tagged_list = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'tagger.model', report_duration = True)
+            >>> tagger.save_model(file_name = 'new_tagger.model')
+
+        Args:
+            filename (str): نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
+
+        """
+        if self.model is None:
+            msg = "you should load model first..."
+            raise ValueError(msg)
+
+        self.model.dump(filename)
+
+    def evaluate(
+        self: "SequenceTagger", tagged_sent: List[List[Tuple[str, str]]],
+    ) -> float:
+        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
+
+        Examples:
+            >>> tagger = SequenceTagger(model = 'tagger.model')
+            >>> tagger.evaluate([[('نامه', 'NOUN,EZ'), ('ایشان', 'PRON'), ('را', 'ADP'), ('دریافت', 'NOUN'), ('داشتم', 'VERB'), ('.', 'PUNCT')]])
+            1.0
+
+
+        Args:
+            tagged_sent: جملات لیبل‌داری که با استفاده از آن مدل را ارزیابی می‌کنیم.
+
+        Returns:
+            دقت مدل
+
+        """
+        if self.model is None:
+            msg = "you should load model first..."
+            raise ValueError(msg)
+
+        def extract_labels(tagged_list):
+            return [[label for _, label in sent] for sent in tagged_list]
+
+        tokens = [[word for word, _ in sent] for sent in tagged_sent]
+        predicted_tagged_sent = self.tag_sents(tokens)
+        return self.__evaluate(
+            extract_labels(tagged_sent),
+            extract_labels(predicted_tagged_sent),
+        )
+
+
+class IOBTagger(SequenceTagger):
+    """IOBTagger."""
+
+    def __init__(self: "SequenceTagger", model=None, data_maker=iob_data_maker) -> None:
+        super().__init__(model, data_maker)
+
+    def __iob_format(self: "SequenceTagger", tagged_data, chunk_tags):
+        return [
+            (token[0], token[1], chunk_tag[1])
+            for token, chunk_tag in zip(tagged_data, chunk_tags)
+        ]
+
+    def tag(self: "SequenceTagger", tagged_data):
+        """یک جمله را در قالب لیستی از توکن‌ها و تگ‌ها دریافت می‌کند و در خروجی لیستی از
+        `(توکن، تگ، برچسب)`ها برمی‌گرداند.
+
+        Examples:
+            >>> iobTagger = IOBTagger(model = 'tagger.model')
+            >>> iobTagger.tag(tagged_data = [('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')])
+            [('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]
+
+        Args:
+            tagged_data (List[Tuple[str, str]]): لیستی از توکن‌های یک جمله که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[Tuple[str, str, str]]): ‌لیستی از `(توکن، تگ، برچسب)`ها.
+
+        """
+        chunk_tags = super().tag(tagged_data)
+        return self.__iob_format(tagged_data, chunk_tags)
+
+    def tag_sents(self: "SequenceTagger", sentences):
+        """جملات را در قالب لیستی لیستی از توکن‌ها و تگ‌ها دریافت می‌کند
+        و در خروجی، لیستی از لیستی از `(توکن، تگ، برچسب)`ها برمی‌گرداند.
+
+        هر لیست از `(توکن، برچسب)`ها مربوط به یک جمله است.
+
+        Examples:
+            >>> iobTagger = IOBTagger(model = 'tagger.model')
+            >>> iobTagger.tag_sents(tagged_data = [[('من', 'PRON'), ('به', 'ADP'), ('مدرسه', 'NOUN,EZ'), ('ایران', 'NOUN'), ('رفته_بودم', 'VERB'), ('.', 'PUNCT')]])
+            [[('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]]
+
+        Args:
+            sentences (List[List[str]]): لیستی از جملات که باید برچسب‌گذاری شود.
+
+        Returns:
+            (List[List[Tuple[str,str]]]): لیستی از لیستی از `(توکن، تگ، برچسب)`ها.
+                    هر لیست از `(توکن، تگ، برچسب)`ها مربوط به یک جمله است.
+
+        """
+        chunk_tags = super().tag_sents(sentences)
+        return [
+            self.__iob_format(tagged_data, chunks)
+            for tagged_data, chunks in zip(sentences, chunk_tags)
+        ]
+
+    def train(
+        self: "SequenceTagger",
+        tagged_list: List[List[Tuple[str, str, str]]],
+        c1: float = 0.4,
+        c2: float = 0.04,
+        max_iteration: int = 400,
+        verbose: True = True,
+        file_name: str = "crf.model",
+        report_duration=True,
+    ):
+        """لیستی از جملات را می‌گیرد و بر اساس آن مدل را آموزش می‌دهد.
+
+        هر جمله، لیستی از `(توکن، تگ، برچسب)`هاست.
+
+        Examples:
+            >>> iobTagger = IOBTagger()
+            >>> iobTagger.train(tagged_list = [[('من', 'PRON', 'B-NP'), ('به', 'ADP', 'B-PP'), ('مدرسه', 'NOUN,EZ', 'B-NP'), ('ایران', 'NOUN', 'I-NP'), ('رفته_بودم', 'VERB', 'B-VP'), ('.', 'PUNCT', 'O')]], c1 = 0.5, c2 = 0.5, max_iteration = 100, verbose = True, file_name = 'newIOBTagger.model', report_duration = True)
+            Feature generation
+            type: CRF1d
+            feature.minfreq: 0.000000
+            feature.possible_states: 0
+            feature.possible_transitions: 1
+            0....1....2....3....4....5....6....7....8....9....10
+            Number of features: 150
+            Seconds required: 0.001
+            ...
+            Writing feature references for attributes
+            Seconds required: 0.000
+
+            training time: 0.01 sec
+
+        Args:
+            tagged_list: جملاتی که مدل از روی آن‌ها آموزش می‌بیند.
+            c1: مقدار L1 regularization.
+            c2: مقدار L2 regularization.
+            max_iteration: تعداد تکرار آموزش بر کل دیتا.
+            verbose: نمایش اطلاعات مربوط به آموزش.
+            file_name: نام و مسیر فایلی که می‌خواهید مدل در آن ذخیره شود.
+            report_duration: نمایش گزارشات مربوط به زمان.
+
+        """
+        tagged_list = [
+            [((word, tag), chunk) for word, tag, chunk in tagged_sent]
+            for tagged_sent in tagged_list
+        ]
+        return super().train(
+            tagged_list,
+            c1,
+            c2,
+            max_iteration,
+            verbose,
+            file_name,
+            report_duration,
+        )
+
+    def evaluate(
+        self: "SequenceTagger", tagged_sent: List[List[Tuple[str, str, str]]],
+    ) -> float:
+        """داده صحیح دریافت شده را با استفاده از مدل لیبل می‌زند و دقت مدل را برمی‌گرداند.
+
+        Examples:
+            >>> iobTagger = IOBTagger(model = 'tagger.model')
+            >>> iobTagger.evaluate([[('نامه', 'NOUN,EZ', 'B-NP'), ('ایشان', 'PRON', 'I-NP'), ('را', 'ADP', 'B-POSTP'), ('دریافت', 'NOUN', 'B-VP'), ('داشتم', 'VERB', 'I-VP'), ('.', 'PUNCT', 'O')]])
+            1.0
+
+
+        Args:
+            tagged_sent: جملات لیبل‌داری که با استفاده از آن مدل را ارزیابی می‌کنیم.
+
+        Returns:
+            دقت مدل
+
+        """
+        if self.model is None:
+            msg = "you should load model first..."
+            raise ValueError(msg)
+
+        def extract_labels(tagged_list):
+            return [[token[-1] for token in sent] for sent in tagged_list]
+
+        tokens = [[token[:-1] for token in sent] for sent in tagged_sent]
+        predicted_tagged_sent = self.tag_sents(tokens)
+        return super()._SequenceTagger__evaluate(
+            extract_labels(tagged_sent),
+            extract_labels(predicted_tagged_sent),
+        )
```

### Comparing `hazm-0.9.1/hazm/stemmer.py` & `hazm-0.9.2/hazm/stemmer.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای ریشه‌یابی کلمات است.
-
-فرق بین [Lemmatizer](./lemmatizer.md) و [Stemmer](./stemmer.md) این است که
-اِستمر درکی از معنای کلمه ندارد و صرفاً براساس حذف برخی از پسوندهای ساده تلاش
-می‌کند ریشهٔ کلمه را بیابد؛ بنابراین ممکن است در ریشه‌یابیِ برخی از کلمات نتایج
-نادرستی ارائه دهد؛ اما لماتایزر براساس لیستی از کلمات مرجع به همراه ریشهٔ آن
-این
-کار را انجام می‌دهد و نتایج دقیق‌تری ارائه می‌دهد. البته هزینهٔ این دقت، سرعتِ
-کمتر در ریشه‌یابی است.
-
-"""
-
-
-from nltk.stem.api import StemmerI
-
-
-class Stemmer(StemmerI):
-    """این کلاس شامل توابعی برای ریشه‌یابی کلمات است."""
-
-    def __init__(self: "Stemmer") -> None:
-        self.ends = [
-            "ات",
-            "ان",
-            "ترین",
-            "تر",
-            "م",
-            "ت",
-            "ش",
-            "یی",
-            "ی",
-            "ها",
-            "ٔ",
-            "‌ا",
-            "‌",
-        ]
-
-    def stem(self: "Stemmer", word: str) -> str:
-        """ریشهٔ کلمه را پیدا می‌کند.
-
-        Examples:
-            >>> stemmer = Stemmer()
-            >>> stemmer.stem('کتابی')
-            'کتاب'
-            >>> stemmer.stem('کتاب‌ها')
-            'کتاب'
-            >>> stemmer.stem('کتاب‌هایی')
-            'کتاب'
-            >>> stemmer.stem('کتابهایشان')
-            'کتاب'
-            >>> stemmer.stem('اندیشه‌اش')
-            'اندیشه'
-            >>> stemmer.stem('خانۀ')
-            'خانه'
-            >>> stemmer.stem('محبوب‌ترین‌ها')
-            'محبوب'
-
-        Args:
-            word: کلمه‌ای که باید ریشهٔ آن پیدا شود.
-
-        Returns:
-            ریشهٔ کلمه.
-
-        """
-        if word.endswith("ۀ"):
-            word = word[:-1] + "ه"
-
-        else:
-            iteration = len(self.ends)
-            while iteration:
-                for end in self.ends:
-                    if word.endswith(end):
-                        word = word[: -len(end)]
-                iteration -= 1
-
-        return word
+"""این ماژول شامل کلاس‌ها و توابعی برای ریشه‌یابی کلمات است.
+
+فرق بین [Lemmatizer](./lemmatizer.md) و [Stemmer](./stemmer.md) این است که
+اِستمر درکی از معنای کلمه ندارد و صرفاً براساس حذف برخی از پسوندهای ساده تلاش
+می‌کند ریشهٔ کلمه را بیابد؛ بنابراین ممکن است در ریشه‌یابیِ برخی از کلمات نتایج
+نادرستی ارائه دهد؛ اما لماتایزر براساس لیستی از کلمات مرجع به همراه ریشهٔ آن
+این
+کار را انجام می‌دهد و نتایج دقیق‌تری ارائه می‌دهد. البته هزینهٔ این دقت، سرعتِ
+کمتر در ریشه‌یابی است.
+
+"""
+
+
+from nltk.stem.api import StemmerI
+
+
+class Stemmer(StemmerI):
+    """این کلاس شامل توابعی برای ریشه‌یابی کلمات است."""
+
+    def __init__(self: "Stemmer") -> None:
+        self.ends = [
+            "ات",
+            "ان",
+            "ترین",
+            "تر",
+            "م",
+            "ت",
+            "ش",
+            "یی",
+            "ی",
+            "ها",
+            "ٔ",
+            "‌ا",
+            "‌",
+        ]
+
+    def stem(self: "Stemmer", word: str) -> str:
+        """ریشهٔ کلمه را پیدا می‌کند.
+
+        Examples:
+            >>> stemmer = Stemmer()
+            >>> stemmer.stem('کتابی')
+            'کتاب'
+            >>> stemmer.stem('کتاب‌ها')
+            'کتاب'
+            >>> stemmer.stem('کتاب‌هایی')
+            'کتاب'
+            >>> stemmer.stem('کتابهایشان')
+            'کتاب'
+            >>> stemmer.stem('اندیشه‌اش')
+            'اندیشه'
+            >>> stemmer.stem('خانۀ')
+            'خانه'
+            >>> stemmer.stem('محبوب‌ترین‌ها')
+            'محبوب'
+
+        Args:
+            word: کلمه‌ای که باید ریشهٔ آن پیدا شود.
+
+        Returns:
+            ریشهٔ کلمه.
+
+        """
+        if word.endswith("ۀ"):
+            word = word[:-1] + "ه"
+
+        else:
+            iteration = len(self.ends)
+            while iteration:
+                for end in self.ends:
+                    if word.endswith(end):
+                        word = word[: -len(end)]
+                iteration -= 1
+
+        return word
```

### Comparing `hazm-0.9.1/hazm/token_splitter.py` & `hazm-0.9.2/hazm/token_splitter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-"""این ماژول شامل کلاس‌ها و توابعی برای تجزیه توکن به دو توکن کوچکتر است."""
-
-
-from typing import List
-from typing import Tuple
-
-from hazm import Lemmatizer
-
-
-class TokenSplitter:
-    """این کلاس شامل توابعی برای تجزیه توکن به دو توکن کوچکتر است."""
-
-    def __init__(self: "TokenSplitter") -> None:
-        self.lemmatizer = Lemmatizer()
-        self.lemmatize = self.lemmatizer.lemmatize
-        self.words = self.lemmatizer.words
-
-    def split_token_words(self: "TokenSplitter", token: str) -> List[Tuple[str, str]]:
-        """توکنِ ورودی را به دو توکن کوچکتر تجزیه می‌کند.
-
-        اگر توکن به بیش از یک روش قابل تجزیه باشد همهٔ حالت‌های ممکن را
-        برمی‌گرداند؛ مثلاً «داستان‌سرا» هم می‌توان به `['داستان', 'سرا']` تجزیه
-        شود و هم می‌تواند به `['داستان‌سرا',]` شکسته شود؛ پس هر دو را
-        برمی‌گرداند: `[('داستان', 'سرا'), ('داستان‌سرا',)]`.
-
-        Examples:
-            >>> splitter = TokenSplitter()
-            >>> splitter.split_token_words('صداوسیماجمهوری')
-            [('صداوسیما', 'جمهوری')]
-            >>> splitter.split_token_words('صداو')
-            [('صد', 'او'), ('صدا', 'و')]
-            >>> splitter.split_token_words('داستان‌سرا')
-            [('داستان', 'سرا'), ('داستان‌سرا',)]
-            >>> splitter.split_token_words('دستان‌سرا')
-            [('دستان', 'سرا')]
-
-        Args:
-            token: توکنی که باید پردازش شود.
-
-        Returns:
-            <dir-rtl>لیستی از `[(توکن, توکن), (توکن, توکن), …]`ها.</dir-rtl>
-
-        """
-        # >>> splitter.split_token_words('شهرموشها')
-
-        candidates = []
-        if "‌" in token:
-            candidates.append(tuple(token.split("‌")))
-
-        splits = [
-            (token[:s], token[s:])
-            for s in range(1, len(token))
-            if token[s - 1] != "‌" and token[s] != "‌"
-        ] + [(token,)]
-        candidates.extend(
-            list(
-                filter(
-                    lambda tokens: set(map(self.lemmatize, tokens)).issubset(
-                        self.words,
-                    ),
-                    splits,
-                ),
-            ),
-        )
-
-        return candidates
+"""این ماژول شامل کلاس‌ها و توابعی برای تجزیه توکن به دو توکن کوچکتر است."""
+
+
+from typing import List
+from typing import Tuple
+
+from hazm import Lemmatizer
+
+
+class TokenSplitter:
+    """این کلاس شامل توابعی برای تجزیه توکن به دو توکن کوچکتر است."""
+
+    def __init__(self: "TokenSplitter") -> None:
+        self.lemmatizer = Lemmatizer()
+        self.lemmatize = self.lemmatizer.lemmatize
+        self.words = self.lemmatizer.words
+
+    def split_token_words(self: "TokenSplitter", token: str) -> List[Tuple[str, str]]:
+        """توکنِ ورودی را به دو توکن کوچکتر تجزیه می‌کند.
+
+        اگر توکن به بیش از یک روش قابل تجزیه باشد همهٔ حالت‌های ممکن را
+        برمی‌گرداند؛ مثلاً «داستان‌سرا» هم می‌توان به `['داستان', 'سرا']` تجزیه
+        شود و هم می‌تواند به `['داستان‌سرا',]` شکسته شود؛ پس هر دو را
+        برمی‌گرداند: `[('داستان', 'سرا'), ('داستان‌سرا',)]`.
+
+        Examples:
+            >>> splitter = TokenSplitter()
+            >>> splitter.split_token_words('صداوسیماجمهوری')
+            [('صداوسیما', 'جمهوری')]
+            >>> splitter.split_token_words('صداو')
+            [('صد', 'او'), ('صدا', 'و')]
+            >>> splitter.split_token_words('داستان‌سرا')
+            [('داستان', 'سرا'), ('داستان‌سرا',)]
+            >>> splitter.split_token_words('دستان‌سرا')
+            [('دستان', 'سرا')]
+
+        Args:
+            token: توکنی که باید پردازش شود.
+
+        Returns:
+            <dir-rtl>لیستی از `[(توکن, توکن), (توکن, توکن), …]`ها.</dir-rtl>
+
+        """
+        # >>> splitter.split_token_words('شهرموشها')
+
+        candidates = []
+        if "‌" in token:
+            candidates.append(tuple(token.split("‌")))
+
+        splits = [
+            (token[:s], token[s:])
+            for s in range(1, len(token))
+            if token[s - 1] != "‌" and token[s] != "‌"
+        ] + [(token,)]
+        candidates.extend(
+            list(
+                filter(
+                    lambda tokens: set(map(self.lemmatize, tokens)).issubset(
+                        self.words,
+                    ),
+                    splits,
+                ),
+            ),
+        )
+
+        return candidates
```

### Comparing `hazm-0.9.1/hazm/utils.py` & `hazm-0.9.2/hazm/utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-"""این ماژول شامل کلاس‌ها و توابع کمکی است."""
-
-import re
-from os import path
-from pathlib import Path
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Tuple
-
-data_path = Path(__file__).parent / "data"
-
-default_words = Path(data_path) / "words.dat"
-default_stopwords = Path(data_path) / "stopwords.dat"
-default_verbs = Path(data_path) / "verbs.dat"
-informal_words = Path(data_path) / "iwords.dat"
-informal_verbs = Path(data_path) / "iverbs.dat"
-
-NUMBERS = "۰۱۲۳۴۵۶۷۸۹"
-
-
-def maketrans(a: str, b: str) -> Dict[int, Any]:
-    """هر یک از حروف رشتهٔ a را به یک حرف در رشتهٔ b مپ می‌کند."""
-    return {ord(a): b for a, b in zip(a, b)}
-
-
-def words_list(
-    words_file: str = default_words,
-) -> List[Tuple[str, int, Tuple[str]]]:
-    """لیست کلمات را برمی‌گرداند.
-
-    Examples:
-        >>> from hazm.utils import words_list
-        >>> words_list()[1]
-        ('آب', 549005877, ('N', 'AJ'))
-
-    Args:
-        words_file: مسیر فایل حاوی کلمات.
-
-    Returns:
-        فهرست کلمات.
-
-    """
-    with Path.open(words_file, encoding="utf-8") as words_file:
-        items = [line.strip().split("\t") for line in words_file]
-        return [
-            (item[0], int(item[1]), tuple(item[2].split(",")))
-            for item in items
-            if len(item) == 3
-        ]
-
-
-def stopwords_list(stopwords_file: str = default_stopwords) -> List[str]:
-    """لیست ایست‌واژه‌ها را برمی‌گرداند.
-
-    Examples:
-        >>> from hazm.utils import stopwords_list
-        >>> stopwords_list()[:4]
-        ['آخرین', 'آقای', 'آمد', 'آمده']
-
-    Args:
-        stopwords_file: مسیر فایل حاوی ایست‌واژه‌ها.
-
-    Returns:
-        فهرست ایست‌واژه‌ها.
-
-    """
-    with Path.open(stopwords_file, encoding="utf8") as stopwords_file:
-        return sorted({w.strip() for w in stopwords_file})
-
-
-def verbs_list() -> List[str]:
-    """لیست افعال را برمی‌گرداند."""
-    with Path.open(default_verbs, encoding="utf8") as verbs_file:
-        lst = []
-        for line in verbs_file:
-            lst.append(line.strip())
-        return lst
-
-
-def past_roots() -> str:
-    """لیست بن‌های گذشته را برمی‌گرداند."""
-    roots = ""
-    for verb in verbs_list():
-        split = verb.split("#")
-        roots += split[0] + "|"
-
-    return roots[:-1]
-
-
-def present_roots() -> str:
-    """لیست بن‌های مضارع را برمی‌گرداند."""
-    roots = ""
-    for verb in verbs_list():
-        split = verb.split("#")
-        roots += split[1] + "|"
-
-    return roots[:-1]
-
-
-def regex_replace(patterns: str, text: str) -> str:
-    """الگوی ریجکس را یافته و با متن داده شده جایگزین می‌کند."""
-    for pattern, repl in patterns:
-        text = re.sub(pattern, repl, text)
-    return text
-
+"""این ماژول شامل کلاس‌ها و توابع کمکی است."""
+
+import re
+from os import path
+from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Tuple
+
+data_path = Path(__file__).parent / "data"
+
+default_words = Path(data_path) / "words.dat"
+default_stopwords = Path(data_path) / "stopwords.dat"
+default_verbs = Path(data_path) / "verbs.dat"
+informal_words = Path(data_path) / "iwords.dat"
+informal_verbs = Path(data_path) / "iverbs.dat"
+
+NUMBERS = "۰۱۲۳۴۵۶۷۸۹"
+
+
+def maketrans(a: str, b: str) -> Dict[int, Any]:
+    """هر یک از حروف رشتهٔ a را به یک حرف در رشتهٔ b مپ می‌کند."""
+    return {ord(a): b for a, b in zip(a, b)}
+
+
+def words_list(
+    words_file: str = default_words,
+) -> List[Tuple[str, int, Tuple[str]]]:
+    """لیست کلمات را برمی‌گرداند.
+
+    Examples:
+        >>> from hazm.utils import words_list
+        >>> words_list()[1]
+        ('آب', 549005877, ('N', 'AJ'))
+
+    Args:
+        words_file: مسیر فایل حاوی کلمات.
+
+    Returns:
+        فهرست کلمات.
+
+    """
+    with Path.open(words_file, encoding="utf-8") as words_file:
+        items = [line.strip().split("\t") for line in words_file]
+        return [
+            (item[0], int(item[1]), tuple(item[2].split(",")))
+            for item in items
+            if len(item) == 3
+        ]
+
+
+def stopwords_list(stopwords_file: str = default_stopwords) -> List[str]:
+    """لیست ایست‌واژه‌ها را برمی‌گرداند.
+
+    Examples:
+        >>> from hazm.utils import stopwords_list
+        >>> stopwords_list()[:4]
+        ['آخرین', 'آقای', 'آمد', 'آمده']
+
+    Args:
+        stopwords_file: مسیر فایل حاوی ایست‌واژه‌ها.
+
+    Returns:
+        فهرست ایست‌واژه‌ها.
+
+    """
+    with Path.open(stopwords_file, encoding="utf8") as stopwords_file:
+        return sorted({w.strip() for w in stopwords_file})
+
+
+def verbs_list() -> List[str]:
+    """لیست افعال را برمی‌گرداند."""
+    with Path.open(default_verbs, encoding="utf8") as verbs_file:
+        lst = []
+        for line in verbs_file:
+            lst.append(line.strip())
+        return lst
+
+
+def past_roots() -> str:
+    """لیست بن‌های گذشته را برمی‌گرداند."""
+    roots = ""
+    for verb in verbs_list():
+        split = verb.split("#")
+        roots += split[0] + "|"
+
+    return roots[:-1]
+
+
+def present_roots() -> str:
+    """لیست بن‌های مضارع را برمی‌گرداند."""
+    roots = ""
+    for verb in verbs_list():
+        split = verb.split("#")
+        roots += split[1] + "|"
+
+    return roots[:-1]
+
+
+def regex_replace(patterns: str, text: str) -> str:
+    """الگوی ریجکس را یافته و با متن داده شده جایگزین می‌کند."""
+    for pattern, repl in patterns:
+        text = re.sub(pattern, repl, text)
+    return text
+
```

### Comparing `hazm-0.9.1/LICENSE` & `hazm-0.9.2/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-
-Copyright (c) 2013 Alireza Nourian
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2013 Alireza Nourian
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

