# Comparing `tmp/relatio-0.2.1.tar.gz` & `tmp/relatio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/andrei/Documents/SIS-CDSS/Projects/D-GESS/Ash/Narrative NLP/relatio/dist/tmp6uu_332q/relatio-0.2.1.tar", last modified: Mon Nov 15 13:39:59 2021, max compression
+gzip compressed data, was "relatio-0.3.0.tar", last modified: Fri Apr 14 15:39:20 2023, max compression
```

## Comparing `relatio-0.2.1.tar` & `relatio-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2021-11-15 13:39:59.000000 relatio-0.2.1/
--rw-r--r--   0 andrei     (501) staff       (20)     1265 2021-11-05 12:23:56.000000 relatio-0.2.1/LICENSE
--rw-r--r--   0 andrei     (501) staff       (20)     2083 2021-11-15 13:39:59.000000 relatio-0.2.1/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1507 2021-11-15 13:34:06.000000 relatio-0.2.1/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      291 2021-08-17 07:22:29.000000 relatio-0.2.1/pyproject.toml
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2021-11-15 13:39:59.000000 relatio-0.2.1/relatio/
--rw-r--r--   0 andrei     (501) staff       (20)       35 2021-11-15 13:38:38.000000 relatio-0.2.1/relatio/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)    10303 2021-11-05 12:31:55.000000 relatio-0.2.1/relatio/clustering.py
--rw-r--r--   0 andrei     (501) staff       (20)     1631 2021-11-05 12:31:57.000000 relatio-0.2.1/relatio/datasets.py
--rw-r--r--   0 andrei     (501) staff       (20)     4671 2021-11-05 12:32:00.000000 relatio-0.2.1/relatio/graphs.py
--rw-r--r--   0 andrei     (501) staff       (20)     4429 2021-11-05 12:32:02.000000 relatio-0.2.1/relatio/named_entity_recognition.py
--rw-r--r--   0 andrei     (501) staff       (20)     9965 2021-11-05 12:32:06.000000 relatio-0.2.1/relatio/semantic_role_labeling.py
--rw-r--r--   0 andrei     (501) staff       (20)    15303 2021-11-05 12:32:08.000000 relatio-0.2.1/relatio/utils.py
--rw-r--r--   0 andrei     (501) staff       (20)     4737 2021-11-05 12:32:11.000000 relatio-0.2.1/relatio/verbs.py
--rw-r--r--   0 andrei     (501) staff       (20)    19859 2021-11-05 12:32:14.000000 relatio-0.2.1/relatio/wrappers.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2021-11-15 13:39:59.000000 relatio-0.2.1/relatio.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     2083 2021-11-15 13:39:59.000000 relatio-0.2.1/relatio.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      409 2021-11-15 13:39:59.000000 relatio-0.2.1/relatio.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2021-11-15 13:39:59.000000 relatio-0.2.1/relatio.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)      162 2021-11-15 13:39:59.000000 relatio-0.2.1/relatio.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)        8 2021-11-15 13:39:59.000000 relatio-0.2.1/relatio.egg-info/top_level.txt
--rw-r--r--   0 andrei     (501) staff       (20)      827 2021-11-15 13:39:59.000000 relatio-0.2.1/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)       38 2021-11-15 13:02:57.000000 relatio-0.2.1/setup.py
+drwxrwxr-x   0 germain   (1000) germain   (1000)        0 2023-04-14 15:39:20.974664 relatio-0.3.0/
+-rw-rw-r--   0 germain   (1000) germain   (1000)     1265 2023-04-13 15:13:37.000000 relatio-0.3.0/LICENSE
+-rw-rw-r--   0 germain   (1000) germain   (1000)     3530 2023-04-14 15:39:20.974664 relatio-0.3.0/PKG-INFO
+-rw-rw-r--   0 germain   (1000) germain   (1000)     2973 2023-04-14 13:02:43.000000 relatio-0.3.0/README.md
+-rw-rw-r--   0 germain   (1000) germain   (1000)      358 2023-04-13 15:09:48.000000 relatio-0.3.0/pyproject.toml
+drwxrwxr-x   0 germain   (1000) germain   (1000)        0 2023-04-14 15:39:20.974664 relatio-0.3.0/relatio/
+-rw-rw-r--   0 germain   (1000) germain   (1000)      448 2023-04-14 13:20:56.000000 relatio-0.3.0/relatio/__init__.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     1627 2023-04-13 15:09:48.000000 relatio-0.3.0/relatio/datasets.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     8351 2023-04-13 15:09:48.000000 relatio-0.3.0/relatio/dependency_parsing.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)    10651 2023-04-14 12:58:48.000000 relatio-0.3.0/relatio/embeddings.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     3488 2023-04-13 15:09:48.000000 relatio-0.3.0/relatio/graphs.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     2657 2023-04-13 15:09:48.000000 relatio-0.3.0/relatio/logging.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)    32455 2023-04-13 15:09:48.000000 relatio-0.3.0/relatio/narrative_models.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)    11222 2023-04-13 15:09:48.000000 relatio-0.3.0/relatio/preprocessing.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     8085 2023-04-13 15:09:48.000000 relatio-0.3.0/relatio/semantic_role_labeling.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     1628 2023-04-13 15:09:48.000000 relatio-0.3.0/relatio/supported_models.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)    10198 2023-04-13 15:09:48.000000 relatio-0.3.0/relatio/utils.py
+-rw-rw-r--   0 germain   (1000) germain   (1000)     4232 2023-04-13 15:09:48.000000 relatio-0.3.0/relatio/verbs.py
+drwxrwxr-x   0 germain   (1000) germain   (1000)        0 2023-04-14 15:39:20.974664 relatio-0.3.0/relatio.egg-info/
+-rw-rw-r--   0 germain   (1000) germain   (1000)     3530 2023-04-14 15:39:20.000000 relatio-0.3.0/relatio.egg-info/PKG-INFO
+-rw-rw-r--   0 germain   (1000) germain   (1000)      508 2023-04-14 15:39:20.000000 relatio-0.3.0/relatio.egg-info/SOURCES.txt
+-rw-rw-r--   0 germain   (1000) germain   (1000)        1 2023-04-14 15:39:20.000000 relatio-0.3.0/relatio.egg-info/dependency_links.txt
+-rw-rw-r--   0 germain   (1000) germain   (1000)      224 2023-04-14 15:39:20.000000 relatio-0.3.0/relatio.egg-info/requires.txt
+-rw-rw-r--   0 germain   (1000) germain   (1000)        8 2023-04-14 15:39:20.000000 relatio-0.3.0/relatio.egg-info/top_level.txt
+-rw-rw-r--   0 germain   (1000) germain   (1000)      892 2023-04-14 15:39:20.974664 relatio-0.3.0/setup.cfg
+-rw-rw-r--   0 germain   (1000) germain   (1000)       38 2023-03-02 10:18:47.000000 relatio-0.3.0/setup.py
+drwxrwxr-x   0 germain   (1000) germain   (1000)        0 2023-04-14 15:39:20.974664 relatio-0.3.0/tests/
+-rw-rw-r--   0 germain   (1000) germain   (1000)      716 2023-04-13 15:09:48.000000 relatio-0.3.0/tests/test_embeddings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `relatio-0.2.1/LICENSE` & `relatio-0.3.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 MIT License
 
-Copyright (c) 2020-2021 ETH Zurich, Andrei V. Plamada
-Copyright (c) 2020-2021 ETH Zurich, Elliott Ash
-Copyright (c) 2020-2021 University of St.Gallen, Philine Widmer
-Copyright (c) 2020-2021 Ecole Polytechnique, Germain Gauthier
+Copyright (c) 2023-2024 ETH Zurich, Andrei V. Plamada
+Copyright (c) 2023-2024 ETH Zurich, Elliott Ash
+Copyright (c) 2023-2024 University of St.Gallen, Philine Widmer
+Copyright (c) 2023-2024 Ecole Polytechnique, Germain Gauthier
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `relatio-0.2.1/relatio/semantic_role_labeling.py` & `relatio-0.3.0/relatio/preprocessing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,313 +1,342 @@
-# MIT License
-
-# Copyright (c) 2020-2021 ETH Zurich, Andrei V. Plamada
-# Copyright (c) 2020-2021 ETH Zurich, Elliott Ash
-# Copyright (c) 2020-2021 University of St.Gallen, Philine Widmer
-# Copyright (c) 2020-2021 Ecole Polytechnique, Germain Gauthier
-
-# Semantic Role Labeling
-# ..................................................................................................................
-# ..................................................................................................................
+import csv
+import time
+from collections import Counter
+from typing import Dict, List, Optional, Tuple
 
-# link to choose the SRL model
-# https://storage.googleapis.com/allennlp-public-models/YOUR-PREFERRED-MODEL
+import pandas as pd
+import spacy
+from spacy.cli import download as spacy_download
+from spacy.tokens import Doc, Token
+from tqdm import tqdm
 
-import time
-import warnings
-from copy import deepcopy
-from typing import Any, Dict, List, Optional, Tuple, Union
-
-import numpy as np
-import torch
-from allennlp_models.structured_prediction.predictors import (
-    SemanticRoleLabelerPredictor as Predictor,
+from relatio.dependency_parsing import (
+    extract_svos_en,
+    extract_svos_fr,
+    from_svos_to_srl_res,
 )
-from tqdm import tqdm
+from relatio.supported_models import LANGUAGE_MODELS
+from relatio.utils import make_list_from_key, save_entities, save_roles
+
+Token.set_extension("noun_chunk", default=None)
 
-from .utils import clean_text, group_sentences_in_batches, replace_sentences
 
+class Preprocessor:
+    """
+    A class to preprocess a given corpus
+    (e.g., split it into sentences, annotate semantic roles, clean the text, mine named entities)
+
+    Args:
+        spacy_model: One of the available spacy models for the English language (default: en_core_web_sm). For a complete list, see: https://spacy.io/models/en
+        remove_punctuation: whether to remove string.punctuation
+        remove_digits: whether to remove string.digits
+        stop_words: list of stopwords to remove
+        lowercase: whether to lower the case
+        lemmatize: whether to lemmatize
+        n_process: Number of processes to user in nlp.pipe() for parallel computing (default: -1). Set to -1 to use all cores on the machine.
+        batch_size: Size of the batches for parallel computing (default: 1000)
+    """
 
-class SRL:
     def __init__(
         self,
-        path: str,
-        cuda_device: int = -1,
-        max_batch_char_length: Optional[int] = None,
-        batch_size: Optional[int] = None,
-        max_sentence_length: Optional[int] = None,
-        max_number_words: Optional[int] = None,
-        cuda_empty_cache: bool = True,
-        cuda_sleep: float = 0.0,
+        spacy_model="en_core_web_sm",
+        remove_punctuation: bool = True,
+        remove_digits: bool = True,
+        stop_words: List[str] = [],
+        lowercase: bool = True,
+        lemmatize: bool = True,
+        remove_chars: Optional[List[str]] = None,
+        n_process: int = -1,
+        batch_size: int = 1000,
     ):
-        self._predictor = Predictor.from_path(path, cuda_device=cuda_device)
-        self._max_batch_char_length = max_batch_char_length
-        self._batch_size = batch_size
-        self._max_sentence_length = max_sentence_length
-        self._max_number_words = max_number_words
-        self._cuda_empty_cache = cuda_empty_cache
-        self._cuda_device = cuda_device
-        self._cuda_sleep = cuda_sleep
-
-    def _clean_cache(self, cuda_sleep, cuda_empty_cache):
-        if self._cuda_device > -1 and cuda_empty_cache:
-            with torch.cuda.device(self._cuda_device):
-                torch.cuda.empty_cache()
-                time.sleep(cuda_sleep)
+        if not spacy.util.is_package(spacy_model):
+            spacy_download(spacy_model)
 
-    def __call__(
+        self.spacy_model = spacy_model
+        self.nlp = spacy.load(spacy_model)
+        self.language = LANGUAGE_MODELS[spacy_model].get("language", "unknown")
+        self.nlp.add_pipe("sentencizer")
+        self.n_process = n_process
+        self.batch_size = batch_size
+        self.remove_punctuation = remove_punctuation
+        self.remove_digits = remove_digits
+        self.stop_words = stop_words
+        self.lowercase = lowercase
+        self.lemmatize = lemmatize
+        self.remove_chars = remove_chars
+
+    def split_into_sentences(
         self,
-        sentences: List[str],
-        max_batch_char_length: Optional[int] = None,
-        batch_size: Optional[int] = None,
-        max_sentence_length: Optional[int] = None,
-        max_number_words: Optional[int] = None,
-        cuda_empty_cache: bool = None,
-        cuda_sleep: float = None,
+        dataframe: pd.DataFrame,
+        output_path: Optional[str] = None,
         progress_bar: bool = False,
-    ):
-        max_batch_char_length = (
-            max_batch_char_length
-            if max_batch_char_length is not None
-            else self._max_batch_char_length
-        )
+    ) -> Tuple[List[str], List[str]]:
+        """
 
-        batch_size = batch_size if batch_size is not None else self._batch_size
+        Split a list of documents into sentences (using the SpaCy sentence splitter).
 
-        max_sentence_length = (
-            max_sentence_length
-            if max_sentence_length is not None
-            else self._max_sentence_length
-        )
+        Args:
+            dataframe: a pandas dataframe with one column "id" and one column "doc"
+            output_path: path to save the pandas DataFrame in a .csv format (default is None). NB: Specifying output_path is much faster than output_path = None for large datasets.
+            progress_bar: print a progress bar (default is False)
 
-        max_number_words = (
-            max_number_words if max_number_words is not None else self._max_number_words
-        )
+        Returns:
+            Pandas DataFrame with  one column "id" and one column "sentence"
 
-        cuda_empty_cache = (
-            cuda_empty_cache if cuda_empty_cache is not None else self._cuda_empty_cache
-        )
+        """
 
-        cuda_sleep = cuda_sleep if cuda_sleep is not None else self._cuda_sleep
+        sentences: List[str] = []
+        doc_ids: List[str] = []
 
-        sentences = replace_sentences(
-            sentences,
-            max_sentence_length=max_sentence_length,
-            max_number_words=max_number_words,
+        length = len(dataframe["doc"])
+
+        spacy_docs = self.nlp.pipe(
+            dataframe["doc"],
+            disable=["tagger", "ner", "parser", "lemmatizer"],
+            batch_size=self.batch_size,
+            n_process=self.n_process,
         )
 
-        batches = group_sentences_in_batches(
+        if progress_bar:
+            print("Splitting into sentences...")
+            time.sleep(1)
+            spacy_docs = tqdm(spacy_docs, total=length)
+
+        if output_path is None:
+            for i, doc in enumerate(spacy_docs):
+                for sent in doc.sents:
+                    sentences.append(str(sent))
+                    doc_ids = doc_ids + [dataframe["id"].iloc[i]]
+
+            df = pd.DataFrame({"id": doc_ids, "sentence": sentences}, index=None)
+
+        else:
+            with open(output_path, "w", newline="") as csvfile:
+                fieldnames = ["id", "sentence"]
+                writer = csv.writer(csvfile)
+                writer.writerow(fieldnames)
+                for i, doc in enumerate(spacy_docs):
+                    for sent in doc.sents:
+                        doc_id = dataframe["id"].iloc[i]
+                        sentence = str(sent)
+                        writer.writerow([doc_id, sentence])
+
+            df = pd.read_csv(output_path)
+
+        return df
+
+    def extract_svos(
+        self,
+        sentences: List[str],
+        expand_nouns: bool = True,
+        only_triplets: bool = True,
+        custom_extraction_function=None,
+        progress_bar: bool = False,
+    ):
+        length = len(sentences)
+
+        spacy_docs = self.nlp.pipe(
             sentences,
-            max_batch_char_length=max_batch_char_length,
-            batch_size=batch_size,
+            disable=["ner", "lemmatizer"],
+            batch_size=self.batch_size,
+            n_process=self.n_process,
         )
 
-        res: List[Dict[str, List]] = []
-
         if progress_bar:
-            print("Running SRL...")
+            print("Extracting SVOs...")
             time.sleep(1)
-            batches = tqdm(batches)
+            spacy_docs = tqdm(spacy_docs, total=length)
 
-        for batch in batches:
-            sentences_json = [{"sentence": sent} for sent in batch]
-            try:
-                res_batch = self._predictor.predict_batch_json(sentences_json)
-            except RuntimeError as err:
-                warnings.warn(f"empty result {err}", RuntimeWarning)
-                res = [{"words": [], "verbs": []}] * len(batch)
-                break
-            except:
-                raise
-            finally:
-                self._clean_cache(cuda_sleep, cuda_empty_cache)
-
-            res.extend(res_batch)
-        return res
-
-
-def extract_roles(
-    srl: List[Dict[str, Any]], used_roles: List[str], progress_bar: bool = False
-) -> Tuple[List[Dict[str, Union[str, bool]]], List[int]]:
+        all_svos = []
+        sentence_index = []
 
-    """
+        for i, sent in enumerate(spacy_docs):
+            if expand_nouns:
+                for noun_chunk in sent.noun_chunks:
+                    for token in noun_chunk:
+                        token._.noun_chunk = noun_chunk
+
+            if custom_extraction_function:
+                svos = custom_extraction_function(sent)
+            elif self.language == "french":
+                svos = extract_svos_fr(sent, expand_nouns, only_triplets)
+            elif self.language == "english":
+                svos = extract_svos_en(sent, expand_nouns, only_triplets)
+            else:
+                raise ValueError(
+                    "No Subject-Verb-Object (SVO) extraction function pre-coded for this language. Please provide a custom extraction function."
+                )
+            sentence_index.extend([i] * len(svos))
+            all_svos.extend(svos)
 
-    A function that extracts semantic roles from the SRL output.
+        all_svos = from_svos_to_srl_res(all_svos)
 
-    Args:
-        srl: srl output
-        used_roles: list of semantic roles to extract
-        progress_bar: print a progress bar (default is False)
+        return sentence_index, all_svos
 
-    Returns:
-        List of statements and numpy array of sentence indices (to keep track of sentences)
+    def clean_text(self, s, pos_tags_to_keep: Optional[List[str]] = None) -> List[str]:
+        """
 
-    """
+        Clean a string of text.
 
-    statements_role_list: List[Dict[str, Union[str, bool]]] = []
-    sentence_index: List[int] = []
+        """
 
-    if progress_bar:
-        print("Processing SRL...")
-        time.sleep(1)
-        srl = tqdm(srl)
+        if self.remove_punctuation:
+            s = [t for t in s if t.is_punct is False]
 
-    for i, sentence_dict in enumerate(srl):
-        role_per_sentence = extract_role_per_sentence(sentence_dict, used_roles)
-        sentence_index.extend([i] * len(role_per_sentence))
-        statements_role_list.extend(role_per_sentence)
+        if self.remove_digits:
+            s = [t for t in s if t.is_digit is False]
 
-    return statements_role_list, np.asarray(sentence_index, dtype=np.uint32)
+        if pos_tags_to_keep:
+            s = [t for t in s if t.pos_ in pos_tags_to_keep]
 
+        if self.lowercase and not self.lemmatize:
+            s = [t.lower_ for t in s]
 
-def extract_role_per_sentence(
-    sentence_dict: dict, used_roles: List[str]
-) -> List[Dict[str, Union[str, bool]]]:
+        if self.lowercase and self.lemmatize:
+            s = [t.lemma_.lower() for t in s]
 
-    """
+        if not self.lowercase and not self.lemmatize:
+            s = [t.text for t in s]
 
-    A function that extracts the semantic roles for a given sentence.
+        if self.remove_chars is not None:
+            for char in self.remove_chars:
+                s = [t.replace(char, " ") for t in s]
 
-    Args:
-        srl: srl output
-        used_roles: list of semantic roles to extract
+        s = [t for t in s if t not in self.stop_words]
 
-    Returns:
-        List of statements with their associated roles for a given sentence
+        s = [t.strip() for t in s if t.strip() not in self.stop_words]
 
-    """
+        s = " ".join(s)
 
-    word_list = sentence_dict["words"]
-    sentence_role_list = []
+        s = s.strip()
 
-    for statement_dict in sentence_dict["verbs"]:
-        tag_list = statement_dict["tags"]
+        return s
 
-        statement_role_dict: Dict[str, Union[str, bool]] = {}
-        for role in ["ARG0", "ARG1", "ARG2", "B-V", "B-ARGM-MOD"]:
-            if role in used_roles:
-                indices_role = [i for i, tok in enumerate(tag_list) if role in tok]
-                toks_role = [
-                    tok for i, tok in enumerate(word_list) if i in indices_role
-                ]
-                statement_role_dict[role] = " ".join(toks_role)
-
-        if "B-ARGM-NEG" in used_roles:
-            role_negation_value = any("B-ARGM-NEG" in tag for tag in tag_list)
-            statement_role_dict["B-ARGM-NEG"] = role_negation_value
-
-        key_to_delete = []
-        for key, value in statement_role_dict.items():
-            if not value:
-                key_to_delete.append(key)
-        for key in key_to_delete:
-            del statement_role_dict[key]
-        sentence_role_list.append(statement_role_dict)
-
-    if not sentence_role_list:
-        sentence_role_list = [{}]
-
-    return sentence_role_list
-
-
-def process_roles(
-    statements: List[Dict[str, List]],
-    max_length: Optional[int] = None,
-    remove_punctuation: bool = True,
-    remove_digits: bool = True,
-    remove_chars: str = "",
-    stop_words: Optional[List[str]] = None,
-    lowercase: bool = True,
-    strip: bool = True,
-    remove_whitespaces: bool = True,
-    lemmatize: bool = False,
-    stem: bool = False,
-    tags_to_keep: Optional[List[str]] = None,
-    remove_n_letter_words: Optional[int] = None,
-    progress_bar: bool = False,
-) -> List[Dict[str, List]]:
+    def mine_entities(
+        self,
+        sentences: List[str],
+        ent_labels: List[str] = ["PERSON", "NORP", "ORG", "GPE", "EVENT"],
+        clean_entities: bool = True,
+        output_path: Optional[str] = None,
+        progress_bar: bool = False,
+    ) -> Counter:
+        """
 
-    """
+        Go through sentences and counts named entities found in the corpus.
 
-    Takes a list of raw extracted semantic roles and cleans the text.
+        Args:
+            sentences: list of sentences
+            ent_labels: list of entity labels to be considered (see SpaCy documentation)
+            progress_bar: print a progress bar (default is False)
+            For other arguments see utils.clean_text.
 
-    Args:
-        max_length = remove roles of more than n characters (NB: very long roles tend to be uninformative)
-        progress_bar: print a progress bar (default is False)
-        For other arguments see utils.clean_text.
+        Returns:
+            Counter with the named entity and its associated frequency on the corpus
 
-    Returns:
-        List of processed statements
+        """
 
-    """
+        entities_all = []
+
+        spacy_sentences = self.nlp.pipe(
+            sentences, batch_size=self.batch_size, n_process=self.n_process
+        )
+
+        length = len(sentences)
 
-    roles_copy = deepcopy(statements)
+        if progress_bar:
+            print("Mining named entities...")
+            time.sleep(1)
+            spacy_sentences = tqdm(spacy_sentences, total=length)
 
-    if progress_bar:
-        print("Cleaning SRL...")
-        time.sleep(1)
-        statements = tqdm(statements)
-
-    for i, statement in enumerate(statements):
-        for role, role_content in roles_copy[i].items():
-            if isinstance(role_content, str):
-                res = clean_text(
-                    [role_content],
-                    remove_punctuation=remove_punctuation,
-                    remove_digits=remove_digits,
-                    remove_chars=remove_chars,
-                    stop_words=stop_words,
-                    lowercase=lowercase,
-                    strip=strip,
-                    remove_whitespaces=remove_whitespaces,
-                    lemmatize=lemmatize,
-                    stem=stem,
-                    tags_to_keep=tags_to_keep,
-                    remove_n_letter_words=remove_n_letter_words,
-                )[0]
-                if max_length is not None:
-                    if len(res) <= max_length:
-                        roles_copy[i][role] = res
+        for sentence in spacy_sentences:
+            for ent in sentence.ents:
+                if ent.label_ in ent_labels:
+                    if clean_entities:
+                        entity = self.clean_text(ent)
                     else:
-                        roles_copy[i][role] = ""
-                else:
-                    roles_copy[i][role] = res
-            elif isinstance(role_content, bool):
-                pass
-            else:
-                raise ValueError(f"{role_content}")
+                        entity = ent.text
+                    entities_all.append(entity)
 
-    return roles_copy
+        entity_counts = Counter(entities_all)
 
+        if output_path is not None:
+            save_entities(entity_counts, output_path)
 
-def rename_arguments(
-    statements: List[dict], progress_bar: bool = False, suffix: str = "_highdim"
-):
+        return entity_counts
 
-    """
+    def clean_roles(self, roles, max_length, pos_tags_to_keep, progress_bar):
+        spacy_roles = self.nlp.pipe(
+            roles, batch_size=self.batch_size, n_process=self.n_process
+        )
 
-    Takes a list of dictionaries and renames the keys of the dictionary with an extra user-specified suffix.
+        length = len(roles)
 
-    Args:
-        statements: list of statements
-        progress_bar: print a progress bar (default is False)
-        suffix: extra suffix to add to the keys of the dictionaries
+        if progress_bar:
+            spacy_roles = tqdm(spacy_roles, total=length)
 
-    Returns:
-        List of dictionaries with renamed keys.
+        clean_roles = []
 
-    """
+        for phrase in spacy_roles:
+            clean_phrase = self.clean_text(phrase, pos_tags_to_keep=pos_tags_to_keep)
+            if max_length is not None:
+                if len(clean_phrase) > max_length:
+                    clean_phrase = ""
+            clean_roles.append(clean_phrase)
+
+        return clean_roles
+
+    def process_roles(
+        self,
+        statements: List[Dict[str, List]],
+        max_length: Optional[int] = None,
+        dict_of_pos_tags_to_keep: Optional[dict] = None,
+        output_path: Optional[str] = None,
+        progress_bar: bool = False,
+    ) -> List[Dict[str, List]]:
+        """
+
+        Takes a list of raw extracted semantic roles and cleans the text.
 
-    roles_copy = deepcopy(statements)
+        Args:
+            max_length = remove roles of more than n characters (NB: very long roles tend to be uninformative)
+            progress_bar: print a progress bar (default is False)
+            For other arguments see utils.clean_text.
+
+        Returns:
+            List of processed statements
+
+        """
+
+        pos_tags_to_keep = {
+            "ARG0": None,
+            "ARG1": None,
+            "ARG2": None,
+            "B-ARGM-MOD": None,
+            "B-V": None,
+        }
+        if dict_of_pos_tags_to_keep is not None:
+            for role in dict_of_pos_tags_to_keep.keys():
+                pos_tags_to_keep[role] = dict_of_pos_tags_to_keep[role]
+
+        length = len(statements)
+        clean_statements: List[dict] = [{} for i in range(length)]
+
+        for role in ["ARG0", "B-V", "B-ARGM-NEG", "B-ARGM-MOD", "ARG1", "ARG2"]:
+            indices, roles = make_list_from_key(role, statements)
+
+            if role != "B-ARGM-NEG":
+                print("Cleaning phrases for role %s..." % role)
+                roles = self.clean_roles(
+                    roles,
+                    max_length=max_length,
+                    pos_tags_to_keep=pos_tags_to_keep[role],
+                    progress_bar=progress_bar,
+                )
+
+            for i, role_content in enumerate(roles):
+                if role_content != "":
+                    clean_statements[indices[i]][role] = role_content
 
-    if progress_bar:
-        print("Processing raw arguments...")
-        time.sleep(1)
-        statements = tqdm(statements)
-
-    for i, statement in enumerate(statements):
-        for role, role_content in statement.items():
-            name = role + suffix
-            roles_copy[i][name] = roles_copy[i].pop(role)
-            roles_copy[i][name] = role_content
+        if output_path is not None:
+            save_roles(clean_statements, output_path)
 
-    return roles_copy
+        return clean_statements
```

### Comparing `relatio-0.2.1/relatio/utils.py` & `relatio-0.3.0/relatio/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,19 @@
-# MIT License
-
-# Copyright (c) 2020-2021 ETH Zurich, Andrei V. Plamada
-# Copyright (c) 2020-2021 ETH Zurich, Elliott Ash
-# Copyright (c) 2020-2021 University of St.Gallen, Philine Widmer
-# Copyright (c) 2020-2021 Ecole Polytechnique, Germain Gauthier
-
-# Utils
-# ..................................................................................................................
-# ..................................................................................................................
-
 import json
-import re
-import string
+import pickle as pk
 import time
 from collections import Counter
-from typing import Dict, List, Optional, Tuple
-
-import pandas as pd
-import spacy
-from nltk import pos_tag
-from nltk.corpus import wordnet
-from nltk.stem import SnowballStemmer, WordNetLemmatizer
-from tqdm import tqdm
-
-nlp = spacy.load("en_core_web_sm", disable=["tagger", "ner", "lemmatizer"])
-
-
-def split_into_sentences(
-    dataframe: pd.DataFrame,
-    output_path: Optional[str] = None,
-    progress_bar: bool = False,
-) -> Tuple[List[str], List[str]]:
-
-    """
-
-    A function that splits a list of documents into sentences (using the SpaCy sentence splitter).
-
-    Args:
-        dataframe: a pandas dataframe with one column "id" and one column "doc"
-        output_path: path to save the output
-        progress_bar: print a progress bar (default is False)
-
-    Returns:
-        Tuple with the list of document indices and list of sentences
-
-    """
-
-    docs = dataframe.to_dict(orient="records")
-
-    sentences: List[str] = []
-    doc_indices: List[str] = []
-
-    if progress_bar:
-        print("Splitting into sentences...")
-        time.sleep(1)
-        docs = tqdm(docs)
-
-    for doc in docs:
-        for sent in nlp(doc["doc"], disable=["tagger", "ner"]).sents:
-            sentences.append(str(sent))
-            doc_indices = doc_indices + [doc["id"]]
-
-    if output_path is not None:
-        with open(output_path, "w") as f:
-            json.dump((doc_indices, sentences), f)
-
-    return (doc_indices, sentences)
+from typing import Dict, List, Optional
 
 
 def replace_sentences(
     sentences: List[str],
     max_sentence_length: Optional[int] = None,
     max_number_words: Optional[int] = None,
 ) -> List[str]:
-
     """
 
     Replace long sentences in list of sentences by empty strings.
 
     Args:
         sentences: list of sentences
         max_sentence_length: Keep only sentences with a a number of character lower or equal to max_sentence_length. For max_number_words = max_sentence_length = -1 all sentences are kept.
@@ -128,15 +64,14 @@
 
 
 def group_sentences_in_batches(
     sentences: List[str],
     max_batch_char_length: Optional[int] = None,
     batch_size: Optional[int] = None,
 ) -> List[List[str]]:
-
     """
 
     Group sentences in batches of given total character length or size (number of sentences).
 
     In case a sentence is longer than max_batch_char_length it is replaced with an empty string.
 
     Args:
@@ -170,15 +105,14 @@
     """
 
     batches: List[List[str]] = []
 
     if max_batch_char_length is not None and batch_size is not None:
         raise ValueError("max_batch_char_length and batch_size are mutually exclusive.")
     elif max_batch_char_length is not None:
-
         # longer sentences are replaced with an empty string
         sentences = replace_sentences(
             sentences, max_sentence_length=max_batch_char_length
         )
         batch_char_length = 0
         batch: List[str] = []
 
@@ -201,173 +135,15 @@
         ]
     else:
         batches = [sentences]
 
     return batches
 
 
-def _get_wordnet_pos(word):
-    """Get POS tag"""
-    tag = pos_tag([word])[0][1][0].upper()
-
-    return tag
-
-
-wnl = WordNetLemmatizer()
-f_lemmatize = wnl.lemmatize
-
-
-def clean_text(
-    sentences: List[str],
-    remove_punctuation: bool = True,
-    remove_digits: bool = True,
-    remove_chars: str = "",
-    stop_words: Optional[List[str]] = None,
-    lowercase: bool = True,
-    strip: bool = True,
-    remove_whitespaces: bool = True,
-    lemmatize: bool = False,
-    stem: bool = False,
-    tags_to_keep: Optional[List[str]] = None,
-    remove_n_letter_words: Optional[int] = None,
-) -> List[str]:
-
-    """
-
-    Clean a list of sentences.
-
-    Args:
-        sentences: list of sentences
-        remove_punctuation: whether to remove string.punctuation
-        remove_digits: whether to remove string.digits
-        remove_chars: remove the given characters
-        stop_words: list of stopwords to remove
-        lowercase: whether to lower the case
-        strip: whether to strip
-        remove_whitespaces: whether to remove superfluous whitespaceing by " ".join(str.split(())
-        lemmatize: whether to lemmatize using nltk.WordNetLemmatizer
-        stem: whether to stem using nltk.SnowballStemmer("english")
-        tags_to_keep: list of grammatical tags to keep (common tags: ['V', 'N', 'J'])
-        remove_n_letter_words: drop words lesser or equal to n letters (default is None)
-
-    Returns:
-        Processed list of sentences
-
-    Examples:
-        >>> clean_text([' Return the factorial of n, an  exact integer >= 0.'])
-        ['return the factorial of n an exact integer']
-        >>> clean_text(['Learning is usefull.'])
-        ['learning is usefull']
-        >>> clean_text([' Return the factorial of n, an  exact integer >= 0.'], stop_words=['factorial'])
-        ['return the of n an exact integer']
-        >>> clean_text([' Return the factorial of n, an  exact integer >= 0.'], lemmatize=True)
-        ['return the factorial of n an exact integer']
-        >>> clean_text(['Learning is usefull.'],lemmatize=True)
-        ['learn be usefull']
-        >>> clean_text([' Return the factorial of n, an  exact integer >= 0.'], stem=True)
-        ['return the factori of n an exact integ']
-        >>> clean_text(['Learning is usefull.'],stem=True)
-        ['learn is useful']
-        >>> clean_text(['A1b c\\n\\nde \\t fg\\rkl\\r\\n m+n'])
-        ['ab c de fg kl mn']
-        >>> clean_text(['This is a sentence with verbs and nice adjectives.'], tags_to_keep = ['V', 'J'])
-        ['is nice']
-        >>> clean_text(['This is a sentence with one and two letter words.'], remove_n_letter_words = 2)
-        ['this sentence with one and two letter words']
-
-    """
-
-    if lemmatize is True and stem is True:
-        raise ValueError("lemmatize and stemming cannot be both True")
-    if stop_words is not None and lowercase is False:
-        raise ValueError("remove stop words make sense only for lowercase")
-
-    # remove chars
-    if remove_punctuation:
-        remove_chars += string.punctuation
-    if remove_digits:
-        remove_chars += string.digits
-    if remove_chars:
-        sentences = [re.sub(f"[{remove_chars}]", "", str(sent)) for sent in sentences]
-
-    # lowercase, strip and remove superfluous white spaces
-    if lowercase:
-        sentences = [sent.lower() for sent in sentences]
-    if strip:
-        sentences = [sent.strip() for sent in sentences]
-    if remove_whitespaces:
-        sentences = [" ".join(sent.split()) for sent in sentences]
-
-    # lemmatize
-    if lemmatize:
-
-        tag_dict = {
-            "J": wordnet.ADJ,
-            "N": wordnet.NOUN,
-            "V": wordnet.VERB,
-            "R": wordnet.ADV,
-        }
-
-        sentences = [
-            " ".join(
-                [
-                    f_lemmatize(
-                        word, tag_dict.get(_get_wordnet_pos(word), wordnet.NOUN)
-                    )
-                    for word in sent.split()
-                ]
-            )
-            for sent in sentences
-        ]
-
-    # keep specific nltk tags
-    # this step should be performed before stemming, but may be performed after lemmatization
-    if tags_to_keep is not None:
-        sentences = [
-            " ".join(
-                [
-                    word
-                    for word in sent.split()
-                    if _get_wordnet_pos(word) in tags_to_keep
-                ]
-            )
-            for sent in sentences
-        ]
-
-    # stem
-    if stem:
-        stemmer = SnowballStemmer("english")
-        f_stem = stemmer.stem
-
-        sentences = [
-            " ".join([f_stem(word) for word in sent.split()]) for sent in sentences
-        ]
-
-    # drop stopwords
-    # stopwords are dropped after the bulk of preprocessing steps, so they should also be preprocessed with the same standards
-    if stop_words is not None:
-        sentences = [
-            " ".join([word for word in sent.split() if word not in stop_words])
-            for sent in sentences
-        ]
-
-    # remove short words < n
-    if remove_n_letter_words is not None:
-        sentences = [
-            " ".join(
-                [word for word in sent.split() if len(word) > remove_n_letter_words]
-            )
-            for sent in sentences
-        ]
-
-    return sentences
-
-
 def is_subsequence(v1: list, v2: list) -> bool:
-
     """
 
     Check whether v1 is a subset of v2.
 
     Args:
         v1: lists of elements
         v2: list of elements
@@ -385,15 +161,14 @@
     # TODO: Check whether the order of elements matter, e.g. is_subsequence(["A","B"],["B","A"])
     return set(v1).issubset(set(v2))
 
 
 def count_values(
     dicts: List[Dict], keys: Optional[list] = None, progress_bar: bool = False
 ) -> Counter:
-
     """
 
     Get a counter with the values of a list of dictionaries, with the conssidered keys given as argument.
 
     Args:
         dicts: list of dictionaries
         keys: keys to consider
@@ -411,15 +186,15 @@
     """
 
     counts: Dict[str, int] = {}
 
     if progress_bar:
         print("Computing role frequencies...")
         time.sleep(1)
-        dicts = tqdm(dicts)
+        dicts = dicts
 
     if keys is None:
         return Counter()
 
     for el in dicts:
         for key, value in el.items():
             if key in keys:
@@ -428,15 +203,14 @@
                 else:
                     counts[value] = 1
 
     return Counter(counts)
 
 
 def count_words(sentences: List[str]) -> Counter:
-
     """
 
     A function that computes word frequencies in a list of sentences.
 
     Args:
         sentences: list of sentences
 
@@ -456,7 +230,98 @@
 
     for sentence in sentences:
         words.extend(sentence.split())
 
     words_counter = Counter(words)
 
     return words_counter
+
+
+def make_list_from_key(key, list_of_dicts):
+    """
+
+    Extract the content of a specific key in a list of dictionaries.
+    Returns a list and the corresponding indices.
+
+    """
+
+    list_from_key = []
+    indices = []
+
+    for i, statement in enumerate(list_of_dicts):
+        content = statement.get(key)
+        if content is not None:
+            list_from_key.append(content)
+            indices.append(i)
+
+    return indices, list_from_key
+
+
+def get_element(narrative, role):
+    return narrative[role] if role in narrative else ""
+
+
+def prettify(narrative) -> str:
+    """
+    Takes a narrative statement dictionary and returns a pretty string.
+
+    Args:
+        narrative: a dictionary with the following keys: "ARG0", "B-V", "B-ARGM-NEG", "B-ARGM-MOD", "ARG1", "ARG2"
+
+    Returns:
+        a concatenated string of text
+    """
+
+    ARG0 = get_element(narrative, "ARG0")
+    V = get_element(narrative, "B-V")
+
+    NEG = get_element(narrative, "B-ARGM-NEG")
+    if NEG is True:
+        NEG = "!"
+    elif NEG is False:
+        NEG = ""
+
+    MOD = get_element(narrative, "B-ARGM-MOD")
+    ARG1 = get_element(narrative, "ARG1")
+    ARG2 = get_element(narrative, "ARG2")
+
+    pretty_narrative = (ARG0, MOD, NEG, V, ARG1, ARG2)
+
+    pretty_narrative = " ".join([t for t in pretty_narrative if t != ""])
+
+    return pretty_narrative
+
+
+def save_entities(entity_counts, output_path: str):
+    """
+    Save the entity counts to a pickle file.
+    """
+    with open(output_path, "wb") as f:
+        pk.dump(entity_counts, f)
+
+
+def load_entities(input_path: str):
+    """
+    Load the entity counts from a pickle file.
+    """
+    with open(input_path, "rb") as f:
+        entity_counts = pk.load(f)
+
+    return entity_counts
+
+
+def save_roles(roles, output_path):
+    """
+    Save the roles to a json file.
+    """
+    with open(output_path, "w") as f:
+        json.dump(roles, f)
+
+
+def load_roles(input_path):
+    """
+    Load the roles from a json file.
+    """
+    with open(input_path, "r") as f:
+        roles = json.load(f)
+
+    return roles
```

### Comparing `relatio-0.2.1/relatio/verbs.py` & `relatio-0.3.0/relatio/verbs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,17 @@
-# MIT License
-
-# Copyright (c) 2020-2021 ETH Zurich, Andrei V. Plamada
-# Copyright (c) 2020-2021 ETH Zurich, Elliott Ash
-# Copyright (c) 2020-2021 University of St.Gallen, Philine Widmer
-# Copyright (c) 2020-2021 Ecole Polytechnique, Germain Gauthier
-
-# Clean Verbs
-# ..................................................................................................................
-# ..................................................................................................................
-
 import time
 from collections import Counter
 from copy import deepcopy
 from typing import List, Optional
 
 from nltk.corpus import wordnet
 from tqdm import tqdm
 
 
 def find_synonyms(verb: str) -> List[str]:
-
     """
 
     Find synonyms of a given word based on wordnet.
 
     Args:
         verb: a verb
 
@@ -42,15 +30,14 @@
         for lemma in syn.lemmas():
             synonyms.append(lemma.name())
 
     return synonyms
 
 
 def find_antonyms(verb: str) -> List[str]:
-
     """
 
     Find antonyms of a given word based on wordnet.
 
     Args:
         verb: a verb
 
@@ -70,15 +57,14 @@
             if lemma.antonyms():
                 antonyms.append(lemma.antonyms()[0].name())
 
     return antonyms
 
 
 def get_most_frequent(tokens: List[str], token_counts: Counter) -> Optional[str]:
-
     """
 
     Find most frequent token in a list of tokens.
 
     Args:
         tokens: a list of tokens
         token_counts: a dictionary of token frequencies
@@ -102,15 +88,14 @@
 
 def clean_verbs(
     statements: List[dict],
     verb_counts: Counter,
     progress_bar: bool = False,
     suffix: str = "_lowdim",
 ) -> List[dict]:
-
     """
 
     Replace verbs by their most frequent synonym or antonym.
     If a verb is combined with a negation in the statement (e.g. 'not increase'),
     it is replaced by its most frequent antonym and the negation is removed (e.g. "decrease").
 
     Args:
```

