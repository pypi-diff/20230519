# Comparing `tmp/negate-0.7.6.tar.gz` & `tmp/negate-0.7.7.tar.gz`

## Comparing `negate-0.7.6.tar` & `negate-0.7.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 negate-0.7.6/.deepsource.toml
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 negate-0.7.6/.pylintrc
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 negate-0.7.6/test.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 negate-0.7.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 negate-0.7.6/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 negate-0.7.6/negate/__init__.py
--rw-r--r--   0        0        0    21828 2020-02-02 00:00:00.000000 negate-0.7.6/negate/negate.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 negate-0.7.6/negate/py.typed
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 negate-0.7.6/negate/tokens.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 negate-0.7.6/tests/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 negate-0.7.6/tests/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 negate-0.7.6/tests/conftest.py
--rw-r--r--   0        0        0    17819 2020-02-02 00:00:00.000000 negate-0.7.6/tests/data.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 negate-0.7.6/tests/requirements.txt
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 negate-0.7.6/tests/test_negate.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 negate-0.7.6/.gitignore
--rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 negate-0.7.6/LICENSE
--rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 negate-0.7.6/README.md
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 negate-0.7.6/pyproject.toml
--rw-r--r--   0        0        0    22117 2020-02-02 00:00:00.000000 negate-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 negate-0.7.7/.deepsource.toml
+-rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 negate-0.7.7/.pylintrc
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 negate-0.7.7/test.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 negate-0.7.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 negate-0.7.7/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 negate-0.7.7/negate/__init__.py
+-rw-r--r--   0        0        0    22309 2020-02-02 00:00:00.000000 negate-0.7.7/negate/negate.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 negate-0.7.7/negate/py.typed
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 negate-0.7.7/negate/tokens.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 negate-0.7.7/tests/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 negate-0.7.7/tests/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 negate-0.7.7/tests/conftest.py
+-rw-r--r--   0        0        0    17999 2020-02-02 00:00:00.000000 negate-0.7.7/tests/data.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 negate-0.7.7/tests/requirements.txt
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 negate-0.7.7/tests/test_negate.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 negate-0.7.7/.gitignore
+-rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 negate-0.7.7/LICENSE
+-rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 negate-0.7.7/README.md
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 negate-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0    22083 2020-02-02 00:00:00.000000 negate-0.7.7/PKG-INFO
```

### Comparing `negate-0.7.6/.pylintrc` & `negate-0.7.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `negate-0.7.6/.github/workflows/run-tests.yml` & `negate-0.7.7/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `negate-0.7.6/negate/negate.py` & `negate-0.7.7/negate/negate.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,16 @@
         )
         self.logger = logging.getLogger(__class__.__name__)
         self.fail_on_unsupported = fail_on_unsupported
         # Load spaCy model. If not available locally, the model will be first
         # installed.
         if use_transformers and use_gpu:
             spacy.require_gpu()
+        else:
+            spacy.require_cpu()
         self.spacy_model = self._initialize_spacy_model(use_transformers)
         # Initialize AUX negation dictionary.
         self._initialize_aux_negations()
         # Store whether tokens have a whitespace after them. This is used later
         # on for detokenization.
         SpacyToken.set_extension("has_space_after", default=True, force=True)
 
@@ -179,19 +181,27 @@
         # AUX as ROOT (e.g.: "I'm excited.") or ROOT children e.g.,
         # "I do think...".
         if (self._is_aux(root) or self._is_verb_to_be(root)
                 or any(self._is_aux(child) for child in root.children)):
             # If the AUX has AUX children, negate them instead. E.g.: "I will
             # be there." or "They have been moody lately."
             aux_child = self._get_aux_child(root)
-            return self._negate_aux_in_doc(
-                aux=root if not aux_child else aux_child,
-                doc=doc,
-                prefer_contractions=prefer_contractions
-            )
+            prev_fail_on_unsupported = self.fail_on_unsupported
+            if aux_child:
+                # Handle cases such as "I expect everything to be ready."
+                self.fail_on_unsupported = True
+            try:
+                return self._negate_aux_in_doc(
+                    aux=root if not aux_child else aux_child,
+                    doc=doc,
+                    prefer_contractions=prefer_contractions
+                )
+            except RuntimeError:
+                # Continue trying to negate the root verb instead.
+                self.fail_on_unsupported = prev_fail_on_unsupported
 
         # General verb non-negated.
         negated_aux = self.negate_aux(self.conjugate_verb('do', root.tag_),
                                       prefer_contractions)
         return self._compile_sentence(
             doc,
             remove_tokens=[root.i],
@@ -471,15 +481,15 @@
             :obj:`spacy.language.Language`: The loaded spaCy model, ready to
             use.
         """
         # See https://stackoverflow.com/a/25061573/14683209
         # We don't want the messages coming from pip to pollute the stdout.
         @contextmanager
         def suppress_stdout():
-            with open(os.devnull, "w") as devnull:
+            with open(os.devnull, "w", encoding="utf-8") as devnull:
                 old_stdout = sys.stdout
                 sys.stdout = devnull
                 try:
                     yield
                 finally:
                     sys.stdout = old_stdout
```

### Comparing `negate-0.7.6/negate/tokens.py` & `negate-0.7.7/negate/tokens.py`

 * *Files identical despite different names*

### Comparing `negate-0.7.6/tests/README.md` & `negate-0.7.7/tests/README.md`

 * *Files identical despite different names*

### Comparing `negate-0.7.6/tests/conftest.py` & `negate-0.7.7/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,11 +18,12 @@
         global negator_model
         if negator_model is None:
             use_transformers = metafunc.config.getoption("transformers")
             try:
                 # `use_gpu` ignored if `use_transformers` is False.
                 negator_model = Negator(
                     use_transformers=use_transformers, use_gpu=True)
-            except ValueError:  # "No GPU devices detected"
+                negator_model.negate_sentence("I will now check GPU support!")
+            except (ValueError, NotImplementedError):  # GPU not supported
                 negator_model = Negator(
                     use_transformers=use_transformers, use_gpu=False)
         metafunc.parametrize("negator", [negator_model])
```

### Comparing `negate-0.7.6/tests/data.py` & `negate-0.7.7/tests/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
     ("I would have done it.", "I would not have done it.", False),
     ("I would've done it.", "I wouldn't have done it.", True),
     ("I would've done it.", "I would not have done it.", False),
     ("I should have done it.", "I shouldn't have done it.", True),
     ("I should have done it.", "I should not have done it.", False),
     ("I should've done it.", "I shouldn't have done it.", True),
     ("I should've done it.", "I should not have done it.", False),
+    ("I expect everything to be ready.", "I don't expect everything to be ready.", True),
 ]
 
 # AUX in ROOT children - Negative
 aux_root_children_negative = [
     ("I shouldn't do it.", "I should do it.", True),
     ("I shouldn't do it.", "I should do it.", False),
     ("I should not do it.", "I should do it.", True),
@@ -212,14 +213,15 @@
     ("I wouldn't have done it.", "I would have done it.", False),
     ("I would not have done it.", "I would have done it.", True),
     ("I would not have done it.", "I would have done it.", False),
     ("I shouldn't have done it.", "I should have done it.", True),
     ("I shouldn't have done it.", "I should have done it.", False),
     ("I should not have done it.", "I should have done it.", True),
     ("I should not have done it.", "I should have done it.", False),
+    ("I don't expect everything to be ready.", "I expect everything to be ready.", True),
 ]
 
 # General verbs - Affirmative
 general_verbs_affirmative = [
     ("I love hiking.", "I don't love hiking.", True),
     ("I love hiking.", "I do not love hiking.", False),
     ("He loves hiking.", "He doesn't love hiking.", True),
```

### Comparing `negate-0.7.6/tests/test_negate.py` & `negate-0.7.7/tests/test_negate.py`

 * *Files identical despite different names*

### Comparing `negate-0.7.6/.gitignore` & `negate-0.7.7/.gitignore`

 * *Files identical despite different names*

### Comparing `negate-0.7.6/LICENSE` & `negate-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `negate-0.7.6/README.md` & `negate-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `negate-0.7.6/pyproject.toml` & `negate-0.7.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 dependencies = [
-    "spacy>=3.4.1,<3.5.0",
-    "spacy-transformers>=1.1.8,<1.2.0",
+    "spacy[transformers]>=3.4.1,<3.6.0",
     "lemminflect>=0.2.3,<0.3.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/dmlls/negate"
 "GitHub Issues" = "https://github.com/dmlls/negate/issues"
 "GitHub Repo" = "https://github.com/dmlls/negate"
```

### Comparing `negate-0.7.6/PKG-INFO` & `negate-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negate
-Version: 0.7.6
+Version: 0.7.7
 Summary: A Python module that negates sentences.
 Project-URL: Homepage, https://github.com/dmlls/negate
 Project-URL: GitHub Issues, https://github.com/dmlls/negate/issues
 Project-URL: GitHub Repo, https://github.com/dmlls/negate
 Author-email: Diego Miguel Lozano <hello@diegomiguel.me>
 Maintainer-email: Diego Miguel Lozano <hello@diegomiguel.me>
 License: 
@@ -220,16 +220,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Requires-Dist: lemminflect<0.3.0,>=0.2.3
-Requires-Dist: spacy-transformers<1.2.0,>=1.1.8
-Requires-Dist: spacy<3.5.0,>=3.4.1
+Requires-Dist: spacy[transformers]<3.6.0,>=3.4.1
 Description-Content-Type: text/markdown
 
 <p align="center"><img width="666" src="https://user-images.githubusercontent.com/22967053/208313993-b873be19-8648-4edd-b4ee-e5283c19ad8f.png" alt="Negate: A Python module to negate sentences."></p>
 <p align="center" display="inline-block">
   <a href="https://pypi.org/project/negate/">
     <img src="https://img.shields.io/pypi/v/negate">
   </a>
```

