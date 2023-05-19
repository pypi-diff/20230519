# Comparing `tmp/vectordb2-0.1.2.tar.gz` & `tmp/vectordb2-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectordb2-0.1.2.tar", last modified: Tue Apr 25 23:51:06 2023, max compression
+gzip compressed data, was "vectordb2-0.1.3.tar", last modified: Fri May 19 02:30:53 2023, max compression
```

## Comparing `vectordb2-0.1.2.tar` & `vectordb2-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 23:51:06.460070 vectordb2-0.1.2/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-25 04:13:48.000000 vectordb2-0.1.2/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)      831 2023-04-25 23:51:06.459824 vectordb2-0.1.2/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)     9470 2023-04-25 23:50:42.000000 vectordb2-0.1.2/README.md
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-25 23:51:06.460140 vectordb2-0.1.2/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1147 2023-04-25 23:38:12.000000 vectordb2-0.1.2/setup.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 23:51:06.458254 vectordb2-0.1.2/vectordb/
--rw-r--r--   0 prelovac   (502) staff       (20)       27 2023-04-25 04:10:57.000000 vectordb2-0.1.2/vectordb/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2666 2023-04-25 23:50:42.000000 vectordb2-0.1.2/vectordb/chunking.py
--rw-r--r--   0 prelovac   (502) staff       (20)      822 2023-04-25 04:00:36.000000 vectordb2-0.1.2/vectordb/embedding.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3703 2023-04-25 04:10:33.000000 vectordb2-0.1.2/vectordb/memory.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1047 2023-04-25 04:00:36.000000 vectordb2-0.1.2/vectordb/storage.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2028 2023-04-25 23:49:46.000000 vectordb2-0.1.2/vectordb/vector_search.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 23:51:06.459518 vectordb2-0.1.2/vectordb2.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)      831 2023-04-25 23:51:06.000000 vectordb2-0.1.2/vectordb2.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      319 2023-04-25 23:51:06.000000 vectordb2-0.1.2/vectordb2.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-25 23:51:06.000000 vectordb2-0.1.2/vectordb2.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)      114 2023-04-25 23:51:06.000000 vectordb2-0.1.2/vectordb2.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        9 2023-04-25 23:51:06.000000 vectordb2-0.1.2/vectordb2.egg-info/top_level.txt
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-19 02:30:53.786134 vectordb2-0.1.3/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-25 04:13:48.000000 vectordb2-0.1.3/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)      831 2023-05-19 02:30:53.785898 vectordb2-0.1.3/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    10172 2023-05-19 01:49:20.000000 vectordb2-0.1.3/README.md
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-05-19 02:30:53.786199 vectordb2-0.1.3/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1173 2023-05-19 00:51:02.000000 vectordb2-0.1.3/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-19 02:30:53.784374 vectordb2-0.1.3/vectordb/
+-rw-r--r--   0 prelovac   (502) staff       (20)       27 2023-04-25 04:10:57.000000 vectordb2-0.1.3/vectordb/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2837 2023-05-19 02:29:35.000000 vectordb2-0.1.3/vectordb/chunking.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1669 2023-05-19 02:29:35.000000 vectordb2-0.1.3/vectordb/embedding.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     4455 2023-05-19 02:29:54.000000 vectordb2-0.1.3/vectordb/memory.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1181 2023-05-01 23:45:05.000000 vectordb2-0.1.3/vectordb/storage.py
+-rw-r--r--   0 prelovac   (502) staff       (20)   318355 2023-05-19 02:29:35.000000 vectordb2-0.1.3/vectordb/test.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2407 2023-05-01 23:49:13.000000 vectordb2-0.1.3/vectordb/vector_search.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-19 02:30:53.785595 vectordb2-0.1.3/vectordb2.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)      831 2023-05-19 02:30:53.000000 vectordb2-0.1.3/vectordb2.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      336 2023-05-19 02:30:53.000000 vectordb2-0.1.3/vectordb2.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-05-19 02:30:53.000000 vectordb2-0.1.3/vectordb2.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)      130 2023-05-19 02:30:53.000000 vectordb2-0.1.3/vectordb2.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        9 2023-05-19 02:30:53.000000 vectordb2-0.1.3/vectordb2.egg-info/top_level.txt
```

### Comparing `vectordb2-0.1.2/LICENSE` & `vectordb2-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vectordb2-0.1.2/PKG-INFO` & `vectordb2-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectordb2
-Version: 0.1.2
+Version: 0.1.3
 Summary: A lightweight Python package for storing and retrieving text using chunking, embedding, and vector search
 Home-page: https://github.com/kagisearch/vectordb
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Keywords: text chunking embedding vector search
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `vectordb2-0.1.2/README.md` & `vectordb2-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # VectorDB
 
 [![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
 
-VectorDB is a lightweight Python package for storing and retrieving text using chunking, embedding, and vector search techniques. It provides an easy-to-use interface for saving, searching, and managing textual data with associated metadata.
+VectorDB is a lightweight, low-latency Python package for storing and retrieving text using chunking, embedding, and vector search techniques. It provides an easy-to-use interface for saving, searching, and managing textual data with associated metadata and is designed for use cases where low latency is essential.
 
 ## Installation
 
-To install VectorDB, use pip:
+To install VectorDB, use pip (note vectordb2 package name):
 
 ```
 pip install vectordb2
 ```
 
 ## Usage
 
@@ -21,41 +21,43 @@
 
 memory = Memory()
 
 # text = "..."
 # metadata = {...}
 
 # Save text with metadata
+# This will automatically embed content
 memory.save(text, metadata)
 
-# Search for relevant chunks
+# Search for top n relevant chunks
+# We will automatically use the fastest vector search backend
 results = memory.search(query, top_n=3)
 ```
 
 ## Methods
 Memory provides the following methods:
 
 
-**__init__(self, memory_file=None, chunking_strategy={"mode":"sliding_window"},
+**__init__(memory_file=None, chunking_strategy={"mode":"sliding_window"},
 embedding_model="sentence-transformers/all-MiniLM-L6-v2")**
 
 
 - Initializes the Memory class.
-- **memory_file** (str): Path to the memory file (default: None). If provided, memory will persist to disk.
-- **chunking_strategy** (dict): Dictionary containing the chunking mode (default: {"mode": "sliding_window"})
-   Options::
-	{'mode':'sliding_window', 'window_size': 256, 'overlap': 32}
+- **memory_file** (str): Path to the memory file (default: None). If provided, memory will persist to disk and loaded/saved to this file. save() will automatically use the provided memory_file.
+- **chunking_strategy** (dict): Dictionary containing the chunking mode (default: {"mode": "sliding_window"})\
+   Options:\
+	{'mode':'sliding_window', 'window_size': 240, 'overlap': 8}\
 	{'mode':'paragraph'}
-- **embedding_model** (str): Name of the pre-trained model to be used for embeddings (default: "sentence-transformers/all-MiniLM-L6-v2"). See [Pretrained models](https://www.sbert.net/docs/pretrained_models.html) and [MTEB](https://huggingface.co/spaces/mteb/leaderboard).
+- **embeddings** (str): can be 'fast', 'normal' or 'best' or the name of the pre-trained embeddings model from HuggingFace to be used for embeddings (default: "sentence-transformers/all-MiniLM-L6-v2"). See [Pretrained models](https://www.sbert.net/docs/pretrained_models.html) and [MTEB](https://huggingface.co/spaces/mteb/leaderboard).
 
-**save(self, texts, metadata_list, memory_file=None)**
+**save(texts, metadata, memory_file=None)**
 
 - Saves the given texts and metadata to memory.
 - **texts** (str or list of str): Text or list of texts to be saved.
-- **metadata_list** (dict or list of dict): Metadata or list of metadata associated with the texts.
+- **metdata** (dict or list of dict): Metadata or list of metadata associated with the texts.
 - **memory_file** (str): Path to the memory file (default: None).
 
 **search(self, query, top_n=5)**
 
 - Searches for the most similar chunks to the given query in memory.
 - **query** (str): Query text.
 - **top_n** (int): Number of most similar chunks to return (default: 5).
@@ -171,11 +173,16 @@
       'title': 'Introduction to Artificial Intelligence', 
       'url': 'https://example.com/introduction-to-artificial-intelligence'
     }
   }
 ]
 ```
 
+## Vector search performance
+
+VectorDB is optimized for speed of retrieval and uses [Faiss](https://github.com/facebookresearch/faiss) for low number of chunks (<4000) and [mrpt](https://github.com/vioshyvo/mrpt) for high number of chunks to ensure maximum performance across the spectrum of use cases.
+
+![Vector search engine comparison](images/comparison.png)
 
 ## License
 
 MIT License.
```

### Comparing `vectordb2-0.1.2/setup.py` & `vectordb2-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vectordb2",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         "torch>=1.9.0",
         "transformers>=4.10.0",
         "numpy>=1.21.0",
         "scikit-learn>=0.24.0",
         "scipy>=1.7.0",
         "sentence_transformers",
         "faiss-cpu",
+        "tensorflow_text"
     ],
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     description="A lightweight Python package for storing and retrieving text using chunking, embedding, and vector search",
     keywords="text chunking embedding vector search",
     url="https://github.com/kagisearch/vectordb",
     classifiers=[
```

### Comparing `vectordb2-0.1.2/vectordb/chunking.py` & `vectordb2-0.1.3/vectordb/chunking.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-from typing import List, Callable
-import spacy
+from typing import List
 import re
+import spacy
 
 nlp = spacy.load("en_core_web_sm", disable=["parser", "ner"])
 
 
 class Chunker:
+    """
+    This class provides a way to chunk a given text using different strategies.
+    """
+
     def __init__(self, strategy: dict):
         """
         Initializes the Chunker with a specified strategy.
 
         :param strategy: a dictionary containing the chunking mode (paragraph or sliding_window)
                          and optional window_size and overlap values for sliding_window mode.
         """
         if strategy["mode"] == "paragraph":
             self.strategy = self.paragraph_chunking
         elif strategy["mode"] == "sliding_window":
             self.strategy = self.sliding_window_chunking
-            self.window_size = strategy.get("window_size", 256)
-            self.overlap = strategy.get("overlap", 32)
+            self.window_size = strategy.get("window_size", 240)
+            self.overlap = strategy.get("overlap", 8)
         else:
             raise ValueError(f"Invalid chunking strategy: {strategy}")
 
-    def clean_text(self, text: str) -> str:
+    @staticmethod
+    def clean_text(text: str) -> str:
         """
         Removes extra whitespaces from the input text.
 
         :param text: a string containing the text to be cleaned.
         :return: a cleaned version of the input text.
         """
         # Remove extra whitespaces
@@ -39,18 +44,18 @@
         Splits the input text into paragraphs.
 
         :param text: a string containing the text to be chunked.
         :return: a list of paragraphs extracted from the input text.
         """
         paragraphs = text.split("\n\n")
         cleaned_paragraphs = []
-        for p in paragraphs:
-            cleaned_p = self.clean_text(p)
-            if cleaned_p:
-                cleaned_paragraphs.append(cleaned_p)
+        for paragraph in paragraphs:
+            cleaned_paragraph = self.clean_text(paragraph)
+            if cleaned_paragraph:
+                cleaned_paragraphs.append(cleaned_paragraph)
         return cleaned_paragraphs
 
     def sliding_window_chunking(self, text: str) -> List[str]:
         """
         Splits the input text into chunks using the sliding window technique.
 
         :param text: a string containing the text to be chunked.
@@ -58,15 +63,17 @@
         """
         if self.window_size is None or self.overlap is None:
             raise ValueError(
                 "Window size and overlap must be specified for sliding window chunking."
             )
 
         text = self.clean_text(text)
-        tokens = [t.text for t in nlp(text)]
+
+        tokens = text.split()
+        # tokens = [t.text for t in nlp(text)]
 
         # Use a list comprehension to create chunks from windows
         step = self.window_size - self.overlap
         # Ensure the range covers the entire length of the tokens
         chunks = [
             " ".join(tokens[i : i + self.window_size])
             for i in range(0, len(tokens) - self.window_size + step, step)
```

### Comparing `vectordb2-0.1.2/vectordb/memory.py` & `vectordb2-0.1.3/vectordb/memory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,89 @@
+"""
+This module provides the Memory class that represents a memory storage system
+for text and associated metadata, with functionality for saving, searching, and
+managing memory entries.
+"""
+
 from typing import List, Dict, Any
 from .chunking import Chunker
 from .embedding import Embedder
 from .vector_search import VectorSearch
 from .storage import Storage
+import time
+import tensorflow as tf
 
 
 class Memory:
+    """
+    Memory class represents a memory storage system for text and associated metadata.
+    It provides functionality for saving, searching, and managing memory entries.
+    """
+
     def __init__(
         self,
         memory_file: str = None,
-        chunking_strategy: dict = {"mode": "sliding_window"},
-        embedding_model: str = "sentence-transformers/all-MiniLM-L6-v2",
+        chunking_strategy: dict = None,
+        embeddings: str = "normal",
     ):
         """
         Initializes the Memory class.
 
         :param memory_file: a string containing the path to the memory file. (default: None)
         :param chunking_strategy: a dictionary containing the chunking mode (default: {"mode": "sliding_window"}).
         :param embedding_model: a string containing the name of the pre-trained model to be used for embeddings (default: "sentence-transformers/all-MiniLM-L6-v2").
         """
         self.memory_file = memory_file
         self.memory = (
             [] if memory_file is None else Storage(memory_file).load_from_disk()
         )
+        if chunking_strategy is None:
+            chunking_strategy = {"mode": "sliding_window"}
         self.chunker = Chunker(chunking_strategy)
-        self.embedder = Embedder(embedding_model)
+        self.embedder = Embedder(embeddings)
         self.vector_search = VectorSearch()
 
-    def save(self, texts, metadata_list, memory_file: str = None):
+    def save(
+        self,
+        texts,
+        metadata: list = [],
+        memory_file: str = None,
+        embed_at_search: bool = False,
+    ):
         """
         Saves the given texts and metadata to memory.
 
         :param texts: a string or a list of strings containing the texts to be saved.
-        :param metadata_list: a dictionary or a list of dictionaries containing the metadata associated with the texts.
+        :param metadata: a dictionary or a list of dictionaries containing the metadata associated with the texts.
         :param memory_file: a string containing the path to the memory file. (default: None)
         """
         if not isinstance(texts, list):
             texts = [texts]
-        if not isinstance(metadata_list, list):
-            metadata_list = [metadata_list]
+        if not isinstance(metadata, list):
+            metadata = [metadata]
+
+        # Extend metadata to be the same length as texts, if it's shorter.
+        metadata += [{}] * (len(texts) - len(metadata))
 
         if memory_file is None:
             memory_file = self.memory_file
-        for text, metadata in zip(texts, metadata_list):
+
+        for text, meta in zip(texts, metadata):
             chunks = self.chunker.strategy(text)
             embeddings = self.embedder.embed_text(chunks)
             for chunk, embedding in zip(chunks, embeddings):
                 entry = {
                     "chunk": chunk,
-                    "embedding": embedding.tolist(),
-                    "metadata": metadata,
+                    "embedding": embedding.numpy().tolist()
+                    if isinstance(embedding, tf.Tensor)
+                    else embedding.tolist(),
+                    "metadata": meta,
                 }
                 self.memory.append(entry)
+
         if memory_file is not None:
             Storage(memory_file).save_to_disk(self.memory)
 
     def search(self, query: str, top_n: int = 5) -> List[Dict[str, Any]]:
         """
         Searches for the most similar chunks to the given query in memory.
 
@@ -85,8 +113,8 @@
         Prints the contents of the memory.
         """
         for entry in self.memory:
             print("Chunk:", entry["chunk"])
             print("Embedding Length:", len(entry["embedding"]))
             print("Metadata:", entry["metadata"])
             print("-" * 40)
-        print("Total entries: ", len)
+        print("Total entries: ", len(self.memory))
```

### Comparing `vectordb2-0.1.2/vectordb/storage.py` & `vectordb2-0.1.3/vectordb/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from typing import List, Dict, Any
 import pickle
 import os
 
 
 class Storage:
+    """
+    A class to handle saving and loading data to and from a memory file.
+    """
+
     def __init__(self, memory_file: str = "long_memory.pkl"):
         """
         Initializes the Storage with a specified memory file.
 
         :param memory_file: a string containing the path to the memory file.
         """
         self.memory_file = memory_file
 
     def save_to_disk(self, data: List[Dict[str, Any]]):
         """
         Saves a list of dictionaries containing data to the memory file.
 
         :param data: a list of dictionaries to be saved.
         """
-        with open(self.memory_file, "wb") as f:
-            pickle.dump(data, f)
+        with open(self.memory_file, "wb") as file_handler:
+            pickle.dump(data, file_handler)
 
     def load_from_disk(self) -> List[Dict[str, Any]]:
         """
         Loads the data from the memory file as a list of dictionaries.
 
         :return: a list of dictionaries containing the data loaded from the memory file.
         """
         if not os.path.exists(self.memory_file):
             return []
-        with open(self.memory_file, "rb") as f:
-            data = pickle.load(f)
+        with open(self.memory_file, "rb") as file_handler:
+            data = pickle.load(file_handler)
         return data
```

### Comparing `vectordb2-0.1.2/vectordb2.egg-info/PKG-INFO` & `vectordb2-0.1.3/vectordb2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectordb2
-Version: 0.1.2
+Version: 0.1.3
 Summary: A lightweight Python package for storing and retrieving text using chunking, embedding, and vector search
 Home-page: https://github.com/kagisearch/vectordb
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Keywords: text chunking embedding vector search
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

