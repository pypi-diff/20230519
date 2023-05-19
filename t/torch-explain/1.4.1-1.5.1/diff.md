# Comparing `tmp/torch_explain-1.4.1.tar.gz` & `tmp/torch_explain-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_explain-1.4.1.tar", last modified: Mon Apr 17 06:22:30 2023, max compression
+gzip compressed data, was "torch_explain-1.5.1.tar", last modified: Fri May 19 08:16:40 2023, max compression
```

## Comparing `torch_explain-1.4.1.tar` & `torch_explain-1.5.1.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.189907 torch_explain-1.4.1/
--rwxrwxrwx   0 root         (0) root         (0)    11558 2021-04-10 16:35:22.000000 torch_explain-1.4.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       26 2021-04-10 16:35:22.000000 torch_explain-1.4.1/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)    12554 2023-04-17 06:22:30.190182 torch_explain-1.4.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    11497 2023-03-13 17:45:04.000000 torch_explain-1.4.1/README.rst
--rwxrwxrwx   0 root         (0) root         (0)       48 2022-06-28 14:29:09.000000 torch_explain-1.4.1/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      148 2023-04-17 06:22:30.190884 torch_explain-1.4.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2236 2023-03-13 18:00:22.000000 torch_explain-1.4.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.176680 torch_explain-1.4.1/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-06-28 14:16:39.000000 torch_explain-1.4.1/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4737 2023-03-13 15:43:46.000000 torch_explain-1.4.1/tests/test_cem.py
--rwxrwxrwx   0 root         (0) root         (0)    11806 2023-03-13 16:15:13.000000 torch_explain-1.4.1/tests/test_logic_layer.py
--rwxrwxrwx   0 root         (0) root         (0)     1016 2023-03-13 15:55:57.000000 torch_explain-1.4.1/tests/test_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.177728 torch_explain-1.4.1/torch_explain/
--rwxrwxrwx   0 root         (0) root         (0)      179 2023-03-13 15:56:23.000000 torch_explain-1.4.1/torch_explain/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-17 06:22:07.000000 torch_explain-1.4.1/torch_explain/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.181007 torch_explain-1.4.1/torch_explain/datasets/
--rwxrwxrwx   0 root         (0) root         (0)      104 2023-03-13 14:44:06.000000 torch_explain-1.4.1/torch_explain/datasets/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1712 2023-03-13 15:20:42.000000 torch_explain-1.4.1/torch_explain/datasets/benchmarks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.182666 torch_explain-1.4.1/torch_explain/logic/
--rwxrwxrwx   0 root         (0) root         (0)      370 2023-03-13 16:08:55.000000 torch_explain-1.4.1/torch_explain/logic/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6048 2023-03-13 16:11:08.000000 torch_explain-1.4.1/torch_explain/logic/metrics.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.185199 torch_explain-1.4.1/torch_explain/logic/nn/
--rwxrwxrwx   0 root         (0) root         (0)        0 2021-06-23 07:06:23.000000 torch_explain-1.4.1/torch_explain/logic/nn/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    21093 2023-04-17 06:20:19.000000 torch_explain-1.4.1/torch_explain/logic/nn/entropy.py
--rwxrwxrwx   0 root         (0) root         (0)    11038 2021-06-23 07:41:49.000000 torch_explain-1.4.1/torch_explain/logic/nn/psi.py
--rwxrwxrwx   0 root         (0) root         (0)     1052 2023-03-13 16:06:44.000000 torch_explain-1.4.1/torch_explain/logic/nn/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     3251 2023-03-13 15:54:45.000000 torch_explain-1.4.1/torch_explain/logic/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.187107 torch_explain-1.4.1/torch_explain/nn/
--rwxrwxrwx   0 root         (0) root         (0)      184 2023-03-13 15:26:10.000000 torch_explain-1.4.1/torch_explain/nn/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3669 2023-03-13 15:36:41.000000 torch_explain-1.4.1/torch_explain/nn/concepts.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.189300 torch_explain-1.4.1/torch_explain/nn/functional/
--rwxrwxrwx   0 root         (0) root         (0)      172 2021-06-23 07:23:21.000000 torch_explain-1.4.1/torch_explain/nn/functional/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      848 2022-05-31 08:15:20.000000 torch_explain-1.4.1/torch_explain/nn/functional/loss.py
--rwxrwxrwx   0 root         (0) root         (0)     1356 2021-06-23 07:26:08.000000 torch_explain-1.4.1/torch_explain/nn/functional/prune.py
--rwxrwxrwx   0 root         (0) root         (0)     2351 2023-03-13 15:50:39.000000 torch_explain-1.4.1/torch_explain/nn/logic.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 06:22:30.180154 torch_explain-1.4.1/torch_explain.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)    12554 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      912 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)      138 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       20 2023-04-17 06:22:30.000000 torch_explain-1.4.1/torch_explain.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 08:16:40.109130 torch_explain-1.5.1/
+-rwxrwxrwx   0 root         (0) root         (0)    11558 2021-04-10 16:35:22.000000 torch_explain-1.5.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       26 2021-04-10 16:35:22.000000 torch_explain-1.5.1/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)    15543 2023-05-19 08:16:40.109301 torch_explain-1.5.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    14486 2023-05-19 08:10:44.000000 torch_explain-1.5.1/README.rst
+-rwxrwxrwx   0 root         (0) root         (0)       48 2022-06-28 14:29:09.000000 torch_explain-1.5.1/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      148 2023-05-19 08:16:40.109685 torch_explain-1.5.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2236 2023-03-13 18:00:22.000000 torch_explain-1.5.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 08:16:40.101405 torch_explain-1.5.1/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-06-28 14:16:39.000000 torch_explain-1.5.1/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4737 2023-03-13 15:43:46.000000 torch_explain-1.5.1/tests/test_cem.py
+-rwxrwxrwx   0 root         (0) root         (0)     3047 2023-05-19 08:10:44.000000 torch_explain-1.5.1/tests/test_dcr.py
+-rwxrwxrwx   0 root         (0) root         (0)    11806 2023-03-13 16:15:13.000000 torch_explain-1.5.1/tests/test_logic_layer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1016 2023-03-13 15:55:57.000000 torch_explain-1.5.1/tests/test_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 08:16:40.102086 torch_explain-1.5.1/torch_explain/
+-rwxrwxrwx   0 root         (0) root         (0)      179 2023-03-13 15:56:23.000000 torch_explain-1.5.1/torch_explain/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-05-19 08:10:44.000000 torch_explain-1.5.1/torch_explain/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 08:16:40.104720 torch_explain-1.5.1/torch_explain/datasets/
+-rwxrwxrwx   0 root         (0) root         (0)      104 2023-03-13 14:44:06.000000 torch_explain-1.5.1/torch_explain/datasets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1712 2023-03-13 15:20:42.000000 torch_explain-1.5.1/torch_explain/datasets/benchmarks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 08:16:40.105571 torch_explain-1.5.1/torch_explain/logic/
+-rwxrwxrwx   0 root         (0) root         (0)      370 2023-03-13 16:08:55.000000 torch_explain-1.5.1/torch_explain/logic/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5963 2023-05-19 08:10:38.000000 torch_explain-1.5.1/torch_explain/logic/metrics.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 08:16:40.106990 torch_explain-1.5.1/torch_explain/logic/nn/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2021-06-23 07:06:23.000000 torch_explain-1.5.1/torch_explain/logic/nn/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    21093 2023-04-17 06:20:19.000000 torch_explain-1.5.1/torch_explain/logic/nn/entropy.py
+-rwxrwxrwx   0 root         (0) root         (0)    11038 2021-06-23 07:41:49.000000 torch_explain-1.5.1/torch_explain/logic/nn/psi.py
+-rwxrwxrwx   0 root         (0) root         (0)     1052 2023-03-13 16:06:44.000000 torch_explain-1.5.1/torch_explain/logic/nn/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     3251 2023-03-13 15:54:45.000000 torch_explain-1.5.1/torch_explain/logic/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 08:16:40.108050 torch_explain-1.5.1/torch_explain/nn/
+-rwxrwxrwx   0 root         (0) root         (0)      184 2023-03-13 15:26:10.000000 torch_explain-1.5.1/torch_explain/nn/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9891 2023-05-19 08:10:44.000000 torch_explain-1.5.1/torch_explain/nn/concepts.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 08:16:40.108827 torch_explain-1.5.1/torch_explain/nn/functional/
+-rwxrwxrwx   0 root         (0) root         (0)      172 2021-06-23 07:23:21.000000 torch_explain-1.5.1/torch_explain/nn/functional/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      848 2022-05-31 08:15:20.000000 torch_explain-1.5.1/torch_explain/nn/functional/loss.py
+-rwxrwxrwx   0 root         (0) root         (0)     1356 2021-06-23 07:26:08.000000 torch_explain-1.5.1/torch_explain/nn/functional/prune.py
+-rwxrwxrwx   0 root         (0) root         (0)     2351 2023-03-13 15:50:39.000000 torch_explain-1.5.1/torch_explain/nn/logic.py
+-rwxrwxrwx   0 root         (0) root         (0)     2081 2023-05-19 08:10:44.000000 torch_explain-1.5.1/torch_explain/nn/semantics.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-19 08:16:40.104125 torch_explain-1.5.1/torch_explain.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    15543 2023-05-19 08:16:40.000000 torch_explain-1.5.1/torch_explain.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      960 2023-05-19 08:16:40.000000 torch_explain-1.5.1/torch_explain.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-19 08:16:40.000000 torch_explain-1.5.1/torch_explain.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-19 08:16:40.000000 torch_explain-1.5.1/torch_explain.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)      138 2023-05-19 08:16:40.000000 torch_explain-1.5.1/torch_explain.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       20 2023-05-19 08:16:40.000000 torch_explain-1.5.1/torch_explain.egg-info/top_level.txt
```

### Comparing `torch_explain-1.4.1/LICENSE` & `torch_explain-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/PKG-INFO` & `torch_explain-1.5.1/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: torch_explain
-Version: 1.4.1
-Summary: PyTorch Explain: Explainable Deep Learning in Python.
-Home-page: https://github.com/pietrobarbiero/pytorch_explain
-Download-URL: https://github.com/pietrobarbiero/pytorch_explain
-Maintainer: P. Barbiero
-Maintainer-email: barbiero@tutanota.com
-License: Apache 2.0
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
 .. image:: https://raw.githubusercontent.com/pietrobarbiero/pytorch_explain/master/doc/_static/img/pye_logo_text_dark.svg
     :align: center
     :height: 100px
     :scale: 50 %
 
 
 
@@ -71,29 +43,32 @@
     :target: https://pypi.org/project/torch-explain/
 
 .. image:: https://zenodo.org/badge/356630474.svg
    :target: https://zenodo.org/badge/latestdoi/356630474
 
 
 `PyTorch, Explain!` is an extension library for PyTorch to develop
-explainable deep learning models going beyond the current accuracy-explainability trade-off.
+explainable deep learning models going beyond the current accuracy-interpretability trade-off.
 
 The library includes a set of tools to develop:
 
 
+* Deep Concept Reasoner (Deep CoRe): an interpretable concept-based model going
+  **beyond the current accuracy-interpretability trade-off**;
 * Concept Embedding Models (CEMs): a class of concept-based models going
   **beyond the current accuracy-explainability trade-off**;
 * Logic Explained Networks (LENs): a class of concept-based models generating
   accurate compound logic explanations for their predictions
   **without the need for a post-hoc explainer**.
 
 Table of Content
 -----------------
 * `Quick start <https://github.com/pietrobarbiero/pytorch_explain#quick-start>`_
 * `Quick tutorial on Concept Embedding Models <https://github.com/pietrobarbiero/pytorch_explain#quick-tutorial-on-concept-embedding-models>`_
+* `Quick tutorial on Deep Concept Reasoning <https://github.com/pietrobarbiero/pytorch_explain#quick-tutorial-on-deep-concept-reasoning>`_
 * `Quick tutorial on Logic Explained Networks <https://github.com/pietrobarbiero/pytorch_explain#quick-tutorial-on-logic-explained-networks>`_
 * `Benchmark datasets <https://github.com/pietrobarbiero/pytorch_explain#benchmark-datasets>`_
 * `Theory <https://github.com/pietrobarbiero/pytorch_explain#theory>`_
 * `Authors <https://github.com/pietrobarbiero/pytorch_explain#authors>`_
 * `Licence <https://github.com/pietrobarbiero/pytorch_explain#licence>`_
 
 Quick start
@@ -107,35 +82,36 @@
     pip install torch-explain
 
 
 Quick tutorial on Concept Embedding Models
 -----------------------------------------------
 
 Using concept embeddings we can solve concept-based problems very efficiently!
-For this simple tutorial, let's approach the trigonometry benchmark dataset:
+For this simple tutorial, let's approach the XOR benchmark dataset:
 
 .. code:: python
 
     import torch
     import torch_explain as te
     from torch_explain import datasets
     from sklearn.metrics import accuracy_score
     from sklearn.model_selection import train_test_split
 
-    x, c, y = datasets.trigonometry(500)
+    x, c, y = datasets.xor(500)
     x_train, x_test, c_train, c_test, y_train, y_test = train_test_split(x, c, y, test_size=0.33, random_state=42)
 
 We just need to define a task predictor and a concept encoder using a
 concept embedding layer:
 
 .. code:: python
 
     import torch
     import torch_explain as te
 
+    embedding_size = 8
     concept_encoder = torch.nn.Sequential(
         torch.nn.Linear(x.shape[1], 10),
         torch.nn.LeakyReLU(),
         te.nn.ConceptEmbedding(10, c.shape[1], embedding_size),
     )
     task_predictor = torch.nn.Sequential(
         torch.nn.Linear(c.shape[1]*embedding_size, 1),
@@ -151,39 +127,100 @@
     loss_form_c = torch.nn.BCELoss()
     loss_form_y = torch.nn.BCEWithLogitsLoss()
     model.train()
     for epoch in range(501):
         optimizer.zero_grad()
 
         # generate concept and task predictions
-        c_emb, c_pred = concept_embedder(x_train)
+        c_emb, c_pred = concept_encoder(x_train)
         y_pred = task_predictor(c_emb.reshape(len(c_emb), -1))
 
         # compute loss
         concept_loss = loss_form_c(c_pred, c_train)
         task_loss = loss_form_y(y_pred, y_train)
         loss = concept_loss + 0.5*task_loss
 
         loss.backward()
         optimizer.step()
 
 Once trained we can check the performance of the model on the test set:
 
 .. code:: python
 
-    c_emb, c_pred = concept_embedder.forward(x_test)
+    c_emb, c_pred = concept_encoder.forward(x_test)
     y_pred = task_predictor(c_emb.reshape(len(c_emb), -1))
 
     task_accuracy = accuracy_score(y_test, y_pred > 0)
     concept_accuracy = accuracy_score(c_test, c_pred > 0.5)
 
 As you can see the performance of the model is now great as the task
 task accuracy is around ~100%.
 
 
+Quick tutorial on Deep Concept Reasoning
+-----------------------------------------------
+
+Using deep concept reasoning we can solve the same problem as above,
+but with an intrinsically interpretable model! In fact, Deep Concept Reasoners (Deep CoRes)
+make task predictions by means of interpretable logic rules using concept embeddings.
+
+Using the same example as before, we can just change the task predictor
+using a Deep CoRe layer:
+
+.. code:: python
+
+    from torch_explain.nn.concepts import ConceptReasoningLayer
+    import torch.nn.functional as F
+
+    y_train = F.one_hot(y_train.long().ravel()).float()
+    y_test = F.one_hot(y_test.long().ravel()).float()
+
+    task_predictor = ConceptReasoningLayer(embedding_size, y_train.shape[1])
+    model = torch.nn.Sequential(concept_encoder, task_predictor)
+
+
+We can now train the network by optimizing the cross entropy loss
+on concepts and tasks:
+
+.. code:: python
+
+    optimizer = torch.optim.AdamW(model.parameters(), lr=0.01)
+    loss_form = torch.nn.BCELoss()
+    model.train()
+    for epoch in range(501):
+        optimizer.zero_grad()
+
+        # generate concept and task predictions
+        c_emb, c_pred = concept_encoder(x_train)
+        y_pred = task_predictor(c_emb, c_pred)
+
+        # compute loss
+        concept_loss = loss_form(c_pred, c_train)
+        task_loss = loss_form(y_pred, y_train)
+        loss = concept_loss + 0.5*task_loss
+
+        loss.backward()
+        optimizer.step()
+
+Once trained the Deep CoRe layer can explain its predictions by
+providing both local and global logic rules:
+
+
+.. code:: python
+
+    local_explanations = task_predictor.explain(c_emb, c_pred, 'local')
+    global_explanations = task_predictor.explain(c_emb, c_pred, 'global')
+
+
+For global explanations, the reasoner will return a dictionary with entries such as
+``{'class': 'y_0', 'explanation': '~c_0 & ~c_1', 'count': 94}``, specifying
+for each logic rule, the task it is associated with and the number of samples
+associated with the explanation.
+
+
 Quick tutorial on Logic Explained Networks
 ---------------------------------------------
 
 For this simple experiment, let's solve the XOR problem
 (augmented with 100 dummy features):
 
 .. code:: python
@@ -263,22 +300,35 @@
 Real-world datasets can be downloaded from the links provided in the supplementary material of the paper.
 
 
 Theory
 --------
 Theoretical foundations can be found in the following papers.
 
+Deep Concept Reasoning (recently accepted at ICML-23)::
+
+    @article{barbiero2023interpretable,
+      title={Interpretable Neural-Symbolic Concept Reasoning},
+      author={Barbiero, Pietro and Ciravegna, Gabriele and Giannini, Francesco and Zarlenga, Mateo Espinosa and Magister, Lucie Charlotte and Tonda, Alberto and Lio, Pietro and Precioso, Frederic and Jamnik, Mateja and Marra, Giuseppe},
+      journal={arXiv preprint arXiv:2304.14068},
+      year={2023}
+    }
+
 Concept Embedding Models::
 
-    @inproceedings{zarlengaconcept,
+    @article{espinosa2022concept,
       title={Concept Embedding Models: Beyond the Accuracy-Explainability Trade-Off},
-      author={Zarlenga, Mateo Espinosa and Barbiero, Pietro and Ciravegna, Gabriele and Marra, Giuseppe and Giannini, Francesco and Diligenti, Michelangelo and Shams, Zohreh and Precioso, Frederic and Melacci, Stefano and Weller, Adrian and others},
-      booktitle={Advances in Neural Information Processing Systems}
+      author={Espinosa Zarlenga, Mateo and Barbiero, Pietro and Ciravegna, Gabriele and Marra, Giuseppe and Giannini, Francesco and Diligenti, Michelangelo and Shams, Zohreh and Precioso, Frederic and Melacci, Stefano and Weller, Adrian and others},
+      journal={Advances in Neural Information Processing Systems},
+      volume={35},
+      pages={21400--21413},
+      year={2022}
     }
 
+
 Logic Explained Networks::
 
     @article{ciravegna2023logic,
       title={Logic explained networks},
       author={Ciravegna, Gabriele and Barbiero, Pietro and Giannini, Francesco and Gori, Marco and Li{\'o}, Pietro and Maggini, Marco and Melacci, Stefano},
       journal={Artificial Intelligence},
       volume={314},
@@ -298,21 +348,24 @@
       pages={6046--6054},
       year={2022}
     }
 
 Psi network ("learning of constraints")::
 
     @inproceedings{ciravegna2020constraint,
-      title={A Constraint-Based Approach to Learning and Explanation.},
+      title={A constraint-based approach to learning and explanation},
       author={Ciravegna, Gabriele and Giannini, Francesco and Melacci, Stefano and Maggini, Marco and Gori, Marco},
-      booktitle={AAAI},
+      booktitle={Proceedings of the AAAI Conference on Artificial Intelligence},
+      volume={34},
+      number={04},
       pages={3658--3665},
       year={2020}
     }
 
+
 Learning with constraints::
 
     @inproceedings{marra2019lyrics,
       title={LYRICS: A General Interface Layer to Integrate Logic Inference and Deep Learning},
       author={Marra, Giuseppe and Giannini, Francesco and Diligenti, Michelangelo and Gori, Marco},
       booktitle={Joint European Conference on Machine Learning and Knowledge Discovery in Databases},
       pages={283--298},
@@ -331,24 +384,26 @@
 
 
 Authors
 -------
 
 * `Pietro Barbiero <http://www.pietrobarbiero.eu/>`__, University of Cambridge, UK.
 * Mateo Espinosa Zarlenga, University of Cambridge, UK.
+* Giuseppe Marra, Katholieke Universiteit Leuven, BE.
 * Steve Azzolin, University of Trento, IT.
 * Francesco Giannini, University of Florence, IT.
 * Gabriele Ciravegna, University of Florence, IT.
 * Dobrik Georgiev, University of Cambridge, UK.
 
 
 Licence
 -------
 
-Copyright 2020 Pietro Barbiero, Mateo Espinosa Zarlenga, Steve Azzolin, Francesco Giannini, Gabriele Ciravegna, and Dobrik Georgiev.
+Copyright 2020 Pietro Barbiero, Mateo Espinosa Zarlenga, Giuseppe Marra,
+Steve Azzolin, Francesco Giannini, Gabriele Ciravegna, and Dobrik Georgiev.
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may
 not use this file except in compliance with the License. You may obtain
 a copy of the License at: http://www.apache.org/licenses/LICENSE-2.0.
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
```

### Comparing `torch_explain-1.4.1/README.rst` & `torch_explain-1.5.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: torch_explain
+Version: 1.5.1
+Summary: PyTorch Explain: Explainable Deep Learning in Python.
+Home-page: https://github.com/pietrobarbiero/pytorch_explain
+Download-URL: https://github.com/pietrobarbiero/pytorch_explain
+Maintainer: P. Barbiero
+Maintainer-email: barbiero@tutanota.com
+License: Apache 2.0
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: tests
+Provides-Extra: docs
+License-File: LICENSE
+
 .. image:: https://raw.githubusercontent.com/pietrobarbiero/pytorch_explain/master/doc/_static/img/pye_logo_text_dark.svg
     :align: center
     :height: 100px
     :scale: 50 %
 
 
 
@@ -43,29 +71,32 @@
     :target: https://pypi.org/project/torch-explain/
 
 .. image:: https://zenodo.org/badge/356630474.svg
    :target: https://zenodo.org/badge/latestdoi/356630474
 
 
 `PyTorch, Explain!` is an extension library for PyTorch to develop
-explainable deep learning models going beyond the current accuracy-explainability trade-off.
+explainable deep learning models going beyond the current accuracy-interpretability trade-off.
 
 The library includes a set of tools to develop:
 
 
+* Deep Concept Reasoner (Deep CoRe): an interpretable concept-based model going
+  **beyond the current accuracy-interpretability trade-off**;
 * Concept Embedding Models (CEMs): a class of concept-based models going
   **beyond the current accuracy-explainability trade-off**;
 * Logic Explained Networks (LENs): a class of concept-based models generating
   accurate compound logic explanations for their predictions
   **without the need for a post-hoc explainer**.
 
 Table of Content
 -----------------
 * `Quick start <https://github.com/pietrobarbiero/pytorch_explain#quick-start>`_
 * `Quick tutorial on Concept Embedding Models <https://github.com/pietrobarbiero/pytorch_explain#quick-tutorial-on-concept-embedding-models>`_
+* `Quick tutorial on Deep Concept Reasoning <https://github.com/pietrobarbiero/pytorch_explain#quick-tutorial-on-deep-concept-reasoning>`_
 * `Quick tutorial on Logic Explained Networks <https://github.com/pietrobarbiero/pytorch_explain#quick-tutorial-on-logic-explained-networks>`_
 * `Benchmark datasets <https://github.com/pietrobarbiero/pytorch_explain#benchmark-datasets>`_
 * `Theory <https://github.com/pietrobarbiero/pytorch_explain#theory>`_
 * `Authors <https://github.com/pietrobarbiero/pytorch_explain#authors>`_
 * `Licence <https://github.com/pietrobarbiero/pytorch_explain#licence>`_
 
 Quick start
@@ -79,35 +110,36 @@
     pip install torch-explain
 
 
 Quick tutorial on Concept Embedding Models
 -----------------------------------------------
 
 Using concept embeddings we can solve concept-based problems very efficiently!
-For this simple tutorial, let's approach the trigonometry benchmark dataset:
+For this simple tutorial, let's approach the XOR benchmark dataset:
 
 .. code:: python
 
     import torch
     import torch_explain as te
     from torch_explain import datasets
     from sklearn.metrics import accuracy_score
     from sklearn.model_selection import train_test_split
 
-    x, c, y = datasets.trigonometry(500)
+    x, c, y = datasets.xor(500)
     x_train, x_test, c_train, c_test, y_train, y_test = train_test_split(x, c, y, test_size=0.33, random_state=42)
 
 We just need to define a task predictor and a concept encoder using a
 concept embedding layer:
 
 .. code:: python
 
     import torch
     import torch_explain as te
 
+    embedding_size = 8
     concept_encoder = torch.nn.Sequential(
         torch.nn.Linear(x.shape[1], 10),
         torch.nn.LeakyReLU(),
         te.nn.ConceptEmbedding(10, c.shape[1], embedding_size),
     )
     task_predictor = torch.nn.Sequential(
         torch.nn.Linear(c.shape[1]*embedding_size, 1),
@@ -123,39 +155,100 @@
     loss_form_c = torch.nn.BCELoss()
     loss_form_y = torch.nn.BCEWithLogitsLoss()
     model.train()
     for epoch in range(501):
         optimizer.zero_grad()
 
         # generate concept and task predictions
-        c_emb, c_pred = concept_embedder(x_train)
+        c_emb, c_pred = concept_encoder(x_train)
         y_pred = task_predictor(c_emb.reshape(len(c_emb), -1))
 
         # compute loss
         concept_loss = loss_form_c(c_pred, c_train)
         task_loss = loss_form_y(y_pred, y_train)
         loss = concept_loss + 0.5*task_loss
 
         loss.backward()
         optimizer.step()
 
 Once trained we can check the performance of the model on the test set:
 
 .. code:: python
 
-    c_emb, c_pred = concept_embedder.forward(x_test)
+    c_emb, c_pred = concept_encoder.forward(x_test)
     y_pred = task_predictor(c_emb.reshape(len(c_emb), -1))
 
     task_accuracy = accuracy_score(y_test, y_pred > 0)
     concept_accuracy = accuracy_score(c_test, c_pred > 0.5)
 
 As you can see the performance of the model is now great as the task
 task accuracy is around ~100%.
 
 
+Quick tutorial on Deep Concept Reasoning
+-----------------------------------------------
+
+Using deep concept reasoning we can solve the same problem as above,
+but with an intrinsically interpretable model! In fact, Deep Concept Reasoners (Deep CoRes)
+make task predictions by means of interpretable logic rules using concept embeddings.
+
+Using the same example as before, we can just change the task predictor
+using a Deep CoRe layer:
+
+.. code:: python
+
+    from torch_explain.nn.concepts import ConceptReasoningLayer
+    import torch.nn.functional as F
+
+    y_train = F.one_hot(y_train.long().ravel()).float()
+    y_test = F.one_hot(y_test.long().ravel()).float()
+
+    task_predictor = ConceptReasoningLayer(embedding_size, y_train.shape[1])
+    model = torch.nn.Sequential(concept_encoder, task_predictor)
+
+
+We can now train the network by optimizing the cross entropy loss
+on concepts and tasks:
+
+.. code:: python
+
+    optimizer = torch.optim.AdamW(model.parameters(), lr=0.01)
+    loss_form = torch.nn.BCELoss()
+    model.train()
+    for epoch in range(501):
+        optimizer.zero_grad()
+
+        # generate concept and task predictions
+        c_emb, c_pred = concept_encoder(x_train)
+        y_pred = task_predictor(c_emb, c_pred)
+
+        # compute loss
+        concept_loss = loss_form(c_pred, c_train)
+        task_loss = loss_form(y_pred, y_train)
+        loss = concept_loss + 0.5*task_loss
+
+        loss.backward()
+        optimizer.step()
+
+Once trained the Deep CoRe layer can explain its predictions by
+providing both local and global logic rules:
+
+
+.. code:: python
+
+    local_explanations = task_predictor.explain(c_emb, c_pred, 'local')
+    global_explanations = task_predictor.explain(c_emb, c_pred, 'global')
+
+
+For global explanations, the reasoner will return a dictionary with entries such as
+``{'class': 'y_0', 'explanation': '~c_0 & ~c_1', 'count': 94}``, specifying
+for each logic rule, the task it is associated with and the number of samples
+associated with the explanation.
+
+
 Quick tutorial on Logic Explained Networks
 ---------------------------------------------
 
 For this simple experiment, let's solve the XOR problem
 (augmented with 100 dummy features):
 
 .. code:: python
@@ -235,22 +328,35 @@
 Real-world datasets can be downloaded from the links provided in the supplementary material of the paper.
 
 
 Theory
 --------
 Theoretical foundations can be found in the following papers.
 
+Deep Concept Reasoning (recently accepted at ICML-23)::
+
+    @article{barbiero2023interpretable,
+      title={Interpretable Neural-Symbolic Concept Reasoning},
+      author={Barbiero, Pietro and Ciravegna, Gabriele and Giannini, Francesco and Zarlenga, Mateo Espinosa and Magister, Lucie Charlotte and Tonda, Alberto and Lio, Pietro and Precioso, Frederic and Jamnik, Mateja and Marra, Giuseppe},
+      journal={arXiv preprint arXiv:2304.14068},
+      year={2023}
+    }
+
 Concept Embedding Models::
 
-    @inproceedings{zarlengaconcept,
+    @article{espinosa2022concept,
       title={Concept Embedding Models: Beyond the Accuracy-Explainability Trade-Off},
-      author={Zarlenga, Mateo Espinosa and Barbiero, Pietro and Ciravegna, Gabriele and Marra, Giuseppe and Giannini, Francesco and Diligenti, Michelangelo and Shams, Zohreh and Precioso, Frederic and Melacci, Stefano and Weller, Adrian and others},
-      booktitle={Advances in Neural Information Processing Systems}
+      author={Espinosa Zarlenga, Mateo and Barbiero, Pietro and Ciravegna, Gabriele and Marra, Giuseppe and Giannini, Francesco and Diligenti, Michelangelo and Shams, Zohreh and Precioso, Frederic and Melacci, Stefano and Weller, Adrian and others},
+      journal={Advances in Neural Information Processing Systems},
+      volume={35},
+      pages={21400--21413},
+      year={2022}
     }
 
+
 Logic Explained Networks::
 
     @article{ciravegna2023logic,
       title={Logic explained networks},
       author={Ciravegna, Gabriele and Barbiero, Pietro and Giannini, Francesco and Gori, Marco and Li{\'o}, Pietro and Maggini, Marco and Melacci, Stefano},
       journal={Artificial Intelligence},
       volume={314},
@@ -270,21 +376,24 @@
       pages={6046--6054},
       year={2022}
     }
 
 Psi network ("learning of constraints")::
 
     @inproceedings{ciravegna2020constraint,
-      title={A Constraint-Based Approach to Learning and Explanation.},
+      title={A constraint-based approach to learning and explanation},
       author={Ciravegna, Gabriele and Giannini, Francesco and Melacci, Stefano and Maggini, Marco and Gori, Marco},
-      booktitle={AAAI},
+      booktitle={Proceedings of the AAAI Conference on Artificial Intelligence},
+      volume={34},
+      number={04},
       pages={3658--3665},
       year={2020}
     }
 
+
 Learning with constraints::
 
     @inproceedings{marra2019lyrics,
       title={LYRICS: A General Interface Layer to Integrate Logic Inference and Deep Learning},
       author={Marra, Giuseppe and Giannini, Francesco and Diligenti, Michelangelo and Gori, Marco},
       booktitle={Joint European Conference on Machine Learning and Knowledge Discovery in Databases},
       pages={283--298},
@@ -303,24 +412,26 @@
 
 
 Authors
 -------
 
 * `Pietro Barbiero <http://www.pietrobarbiero.eu/>`__, University of Cambridge, UK.
 * Mateo Espinosa Zarlenga, University of Cambridge, UK.
+* Giuseppe Marra, Katholieke Universiteit Leuven, BE.
 * Steve Azzolin, University of Trento, IT.
 * Francesco Giannini, University of Florence, IT.
 * Gabriele Ciravegna, University of Florence, IT.
 * Dobrik Georgiev, University of Cambridge, UK.
 
 
 Licence
 -------
 
-Copyright 2020 Pietro Barbiero, Mateo Espinosa Zarlenga, Steve Azzolin, Francesco Giannini, Gabriele Ciravegna, and Dobrik Georgiev.
+Copyright 2020 Pietro Barbiero, Mateo Espinosa Zarlenga, Giuseppe Marra,
+Steve Azzolin, Francesco Giannini, Gabriele Ciravegna, and Dobrik Georgiev.
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may
 not use this file except in compliance with the License. You may obtain
 a copy of the License at: http://www.apache.org/licenses/LICENSE-2.0.
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
```

### Comparing `torch_explain-1.4.1/setup.py` & `torch_explain-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/tests/test_cem.py` & `torch_explain-1.5.1/tests/test_cem.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/tests/test_logic_layer.py` & `torch_explain-1.5.1/tests/test_logic_layer.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/tests/test_utils.py` & `torch_explain-1.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/torch_explain/datasets/benchmarks.py` & `torch_explain-1.5.1/torch_explain/datasets/benchmarks.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/torch_explain/logic/metrics.py` & `torch_explain-1.5.1/torch_explain/logic/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,14 @@
     assert len(y.shape) == 2
     
     y2 = y.argmax(-1)
     x = x.cpu().detach().numpy()
     concept_list = [f"feature{i:010}" for i in range(x.shape[1])]
     
     # get predictions using sympy
-    global class_predictions  # remove
-    global class_predictions_filtered_by_pred
     class_predictions = torch.zeros(len(formulas), x.shape[0])
     for i, formula in enumerate(formulas):
         explanation = to_dnf(formula)
         fun = lambdify(concept_list, explanation, 'numpy')
         
         predictions = fun(*[x[:, i] > threshold for i in range(x.shape[1])])
         predictions = torch.LongTensor(predictions)
```

### Comparing `torch_explain-1.4.1/torch_explain/logic/nn/entropy.py` & `torch_explain-1.5.1/torch_explain/logic/nn/entropy.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/torch_explain/logic/nn/psi.py` & `torch_explain-1.5.1/torch_explain/logic/nn/psi.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/torch_explain/logic/nn/utils.py` & `torch_explain-1.5.1/torch_explain/logic/nn/utils.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/torch_explain/logic/utils.py` & `torch_explain-1.5.1/torch_explain/logic/utils.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/torch_explain/nn/functional/loss.py` & `torch_explain-1.5.1/torch_explain/nn/functional/loss.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/torch_explain/nn/functional/prune.py` & `torch_explain-1.5.1/torch_explain/nn/functional/prune.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/torch_explain/nn/logic.py` & `torch_explain-1.5.1/torch_explain/nn/logic.py`

 * *Files identical despite different names*

### Comparing `torch_explain-1.4.1/torch_explain.egg-info/PKG-INFO` & `torch_explain-1.5.1/torch_explain.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-explain
-Version: 1.4.1
+Version: 1.5.1
 Summary: PyTorch Explain: Explainable Deep Learning in Python.
 Home-page: https://github.com/pietrobarbiero/pytorch_explain
 Download-URL: https://github.com/pietrobarbiero/pytorch_explain
 Maintainer: P. Barbiero
 Maintainer-email: barbiero@tutanota.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
@@ -71,29 +71,32 @@
     :target: https://pypi.org/project/torch-explain/
 
 .. image:: https://zenodo.org/badge/356630474.svg
    :target: https://zenodo.org/badge/latestdoi/356630474
 
 
 `PyTorch, Explain!` is an extension library for PyTorch to develop
-explainable deep learning models going beyond the current accuracy-explainability trade-off.
+explainable deep learning models going beyond the current accuracy-interpretability trade-off.
 
 The library includes a set of tools to develop:
 
 
+* Deep Concept Reasoner (Deep CoRe): an interpretable concept-based model going
+  **beyond the current accuracy-interpretability trade-off**;
 * Concept Embedding Models (CEMs): a class of concept-based models going
   **beyond the current accuracy-explainability trade-off**;
 * Logic Explained Networks (LENs): a class of concept-based models generating
   accurate compound logic explanations for their predictions
   **without the need for a post-hoc explainer**.
 
 Table of Content
 -----------------
 * `Quick start <https://github.com/pietrobarbiero/pytorch_explain#quick-start>`_
 * `Quick tutorial on Concept Embedding Models <https://github.com/pietrobarbiero/pytorch_explain#quick-tutorial-on-concept-embedding-models>`_
+* `Quick tutorial on Deep Concept Reasoning <https://github.com/pietrobarbiero/pytorch_explain#quick-tutorial-on-deep-concept-reasoning>`_
 * `Quick tutorial on Logic Explained Networks <https://github.com/pietrobarbiero/pytorch_explain#quick-tutorial-on-logic-explained-networks>`_
 * `Benchmark datasets <https://github.com/pietrobarbiero/pytorch_explain#benchmark-datasets>`_
 * `Theory <https://github.com/pietrobarbiero/pytorch_explain#theory>`_
 * `Authors <https://github.com/pietrobarbiero/pytorch_explain#authors>`_
 * `Licence <https://github.com/pietrobarbiero/pytorch_explain#licence>`_
 
 Quick start
@@ -107,35 +110,36 @@
     pip install torch-explain
 
 
 Quick tutorial on Concept Embedding Models
 -----------------------------------------------
 
 Using concept embeddings we can solve concept-based problems very efficiently!
-For this simple tutorial, let's approach the trigonometry benchmark dataset:
+For this simple tutorial, let's approach the XOR benchmark dataset:
 
 .. code:: python
 
     import torch
     import torch_explain as te
     from torch_explain import datasets
     from sklearn.metrics import accuracy_score
     from sklearn.model_selection import train_test_split
 
-    x, c, y = datasets.trigonometry(500)
+    x, c, y = datasets.xor(500)
     x_train, x_test, c_train, c_test, y_train, y_test = train_test_split(x, c, y, test_size=0.33, random_state=42)
 
 We just need to define a task predictor and a concept encoder using a
 concept embedding layer:
 
 .. code:: python
 
     import torch
     import torch_explain as te
 
+    embedding_size = 8
     concept_encoder = torch.nn.Sequential(
         torch.nn.Linear(x.shape[1], 10),
         torch.nn.LeakyReLU(),
         te.nn.ConceptEmbedding(10, c.shape[1], embedding_size),
     )
     task_predictor = torch.nn.Sequential(
         torch.nn.Linear(c.shape[1]*embedding_size, 1),
@@ -151,39 +155,100 @@
     loss_form_c = torch.nn.BCELoss()
     loss_form_y = torch.nn.BCEWithLogitsLoss()
     model.train()
     for epoch in range(501):
         optimizer.zero_grad()
 
         # generate concept and task predictions
-        c_emb, c_pred = concept_embedder(x_train)
+        c_emb, c_pred = concept_encoder(x_train)
         y_pred = task_predictor(c_emb.reshape(len(c_emb), -1))
 
         # compute loss
         concept_loss = loss_form_c(c_pred, c_train)
         task_loss = loss_form_y(y_pred, y_train)
         loss = concept_loss + 0.5*task_loss
 
         loss.backward()
         optimizer.step()
 
 Once trained we can check the performance of the model on the test set:
 
 .. code:: python
 
-    c_emb, c_pred = concept_embedder.forward(x_test)
+    c_emb, c_pred = concept_encoder.forward(x_test)
     y_pred = task_predictor(c_emb.reshape(len(c_emb), -1))
 
     task_accuracy = accuracy_score(y_test, y_pred > 0)
     concept_accuracy = accuracy_score(c_test, c_pred > 0.5)
 
 As you can see the performance of the model is now great as the task
 task accuracy is around ~100%.
 
 
+Quick tutorial on Deep Concept Reasoning
+-----------------------------------------------
+
+Using deep concept reasoning we can solve the same problem as above,
+but with an intrinsically interpretable model! In fact, Deep Concept Reasoners (Deep CoRes)
+make task predictions by means of interpretable logic rules using concept embeddings.
+
+Using the same example as before, we can just change the task predictor
+using a Deep CoRe layer:
+
+.. code:: python
+
+    from torch_explain.nn.concepts import ConceptReasoningLayer
+    import torch.nn.functional as F
+
+    y_train = F.one_hot(y_train.long().ravel()).float()
+    y_test = F.one_hot(y_test.long().ravel()).float()
+
+    task_predictor = ConceptReasoningLayer(embedding_size, y_train.shape[1])
+    model = torch.nn.Sequential(concept_encoder, task_predictor)
+
+
+We can now train the network by optimizing the cross entropy loss
+on concepts and tasks:
+
+.. code:: python
+
+    optimizer = torch.optim.AdamW(model.parameters(), lr=0.01)
+    loss_form = torch.nn.BCELoss()
+    model.train()
+    for epoch in range(501):
+        optimizer.zero_grad()
+
+        # generate concept and task predictions
+        c_emb, c_pred = concept_encoder(x_train)
+        y_pred = task_predictor(c_emb, c_pred)
+
+        # compute loss
+        concept_loss = loss_form(c_pred, c_train)
+        task_loss = loss_form(y_pred, y_train)
+        loss = concept_loss + 0.5*task_loss
+
+        loss.backward()
+        optimizer.step()
+
+Once trained the Deep CoRe layer can explain its predictions by
+providing both local and global logic rules:
+
+
+.. code:: python
+
+    local_explanations = task_predictor.explain(c_emb, c_pred, 'local')
+    global_explanations = task_predictor.explain(c_emb, c_pred, 'global')
+
+
+For global explanations, the reasoner will return a dictionary with entries such as
+``{'class': 'y_0', 'explanation': '~c_0 & ~c_1', 'count': 94}``, specifying
+for each logic rule, the task it is associated with and the number of samples
+associated with the explanation.
+
+
 Quick tutorial on Logic Explained Networks
 ---------------------------------------------
 
 For this simple experiment, let's solve the XOR problem
 (augmented with 100 dummy features):
 
 .. code:: python
@@ -263,22 +328,35 @@
 Real-world datasets can be downloaded from the links provided in the supplementary material of the paper.
 
 
 Theory
 --------
 Theoretical foundations can be found in the following papers.
 
+Deep Concept Reasoning (recently accepted at ICML-23)::
+
+    @article{barbiero2023interpretable,
+      title={Interpretable Neural-Symbolic Concept Reasoning},
+      author={Barbiero, Pietro and Ciravegna, Gabriele and Giannini, Francesco and Zarlenga, Mateo Espinosa and Magister, Lucie Charlotte and Tonda, Alberto and Lio, Pietro and Precioso, Frederic and Jamnik, Mateja and Marra, Giuseppe},
+      journal={arXiv preprint arXiv:2304.14068},
+      year={2023}
+    }
+
 Concept Embedding Models::
 
-    @inproceedings{zarlengaconcept,
+    @article{espinosa2022concept,
       title={Concept Embedding Models: Beyond the Accuracy-Explainability Trade-Off},
-      author={Zarlenga, Mateo Espinosa and Barbiero, Pietro and Ciravegna, Gabriele and Marra, Giuseppe and Giannini, Francesco and Diligenti, Michelangelo and Shams, Zohreh and Precioso, Frederic and Melacci, Stefano and Weller, Adrian and others},
-      booktitle={Advances in Neural Information Processing Systems}
+      author={Espinosa Zarlenga, Mateo and Barbiero, Pietro and Ciravegna, Gabriele and Marra, Giuseppe and Giannini, Francesco and Diligenti, Michelangelo and Shams, Zohreh and Precioso, Frederic and Melacci, Stefano and Weller, Adrian and others},
+      journal={Advances in Neural Information Processing Systems},
+      volume={35},
+      pages={21400--21413},
+      year={2022}
     }
 
+
 Logic Explained Networks::
 
     @article{ciravegna2023logic,
       title={Logic explained networks},
       author={Ciravegna, Gabriele and Barbiero, Pietro and Giannini, Francesco and Gori, Marco and Li{\'o}, Pietro and Maggini, Marco and Melacci, Stefano},
       journal={Artificial Intelligence},
       volume={314},
@@ -298,21 +376,24 @@
       pages={6046--6054},
       year={2022}
     }
 
 Psi network ("learning of constraints")::
 
     @inproceedings{ciravegna2020constraint,
-      title={A Constraint-Based Approach to Learning and Explanation.},
+      title={A constraint-based approach to learning and explanation},
       author={Ciravegna, Gabriele and Giannini, Francesco and Melacci, Stefano and Maggini, Marco and Gori, Marco},
-      booktitle={AAAI},
+      booktitle={Proceedings of the AAAI Conference on Artificial Intelligence},
+      volume={34},
+      number={04},
       pages={3658--3665},
       year={2020}
     }
 
+
 Learning with constraints::
 
     @inproceedings{marra2019lyrics,
       title={LYRICS: A General Interface Layer to Integrate Logic Inference and Deep Learning},
       author={Marra, Giuseppe and Giannini, Francesco and Diligenti, Michelangelo and Gori, Marco},
       booktitle={Joint European Conference on Machine Learning and Knowledge Discovery in Databases},
       pages={283--298},
@@ -331,24 +412,26 @@
 
 
 Authors
 -------
 
 * `Pietro Barbiero <http://www.pietrobarbiero.eu/>`__, University of Cambridge, UK.
 * Mateo Espinosa Zarlenga, University of Cambridge, UK.
+* Giuseppe Marra, Katholieke Universiteit Leuven, BE.
 * Steve Azzolin, University of Trento, IT.
 * Francesco Giannini, University of Florence, IT.
 * Gabriele Ciravegna, University of Florence, IT.
 * Dobrik Georgiev, University of Cambridge, UK.
 
 
 Licence
 -------
 
-Copyright 2020 Pietro Barbiero, Mateo Espinosa Zarlenga, Steve Azzolin, Francesco Giannini, Gabriele Ciravegna, and Dobrik Georgiev.
+Copyright 2020 Pietro Barbiero, Mateo Espinosa Zarlenga, Giuseppe Marra,
+Steve Azzolin, Francesco Giannini, Gabriele Ciravegna, and Dobrik Georgiev.
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may
 not use this file except in compliance with the License. You may obtain
 a copy of the License at: http://www.apache.org/licenses/LICENSE-2.0.
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
```

### Comparing `torch_explain-1.4.1/torch_explain.egg-info/SOURCES.txt` & `torch_explain-1.5.1/torch_explain.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 tests/__init__.py
 tests/test_cem.py
+tests/test_dcr.py
 tests/test_logic_layer.py
 tests/test_utils.py
 torch_explain/__init__.py
 torch_explain/_version.py
 torch_explain.egg-info/PKG-INFO
 torch_explain.egg-info/SOURCES.txt
 torch_explain.egg-info/dependency_links.txt
@@ -24,10 +25,11 @@
 torch_explain/logic/nn/__init__.py
 torch_explain/logic/nn/entropy.py
 torch_explain/logic/nn/psi.py
 torch_explain/logic/nn/utils.py
 torch_explain/nn/__init__.py
 torch_explain/nn/concepts.py
 torch_explain/nn/logic.py
+torch_explain/nn/semantics.py
 torch_explain/nn/functional/__init__.py
 torch_explain/nn/functional/loss.py
 torch_explain/nn/functional/prune.py
```

