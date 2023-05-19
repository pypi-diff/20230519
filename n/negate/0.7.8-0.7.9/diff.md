# Comparing `tmp/negate-0.7.8.tar.gz` & `tmp/negate-0.7.9.tar.gz`

## Comparing `negate-0.7.8.tar` & `negate-0.7.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 negate-0.7.8/.deepsource.toml
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 negate-0.7.8/.pylintrc
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 negate-0.7.8/test.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 negate-0.7.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 negate-0.7.8/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 negate-0.7.8/negate/__init__.py
--rw-r--r--   0        0        0    22336 2020-02-02 00:00:00.000000 negate-0.7.8/negate/negate.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 negate-0.7.8/negate/py.typed
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 negate-0.7.8/negate/tokens.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 negate-0.7.8/tests/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 negate-0.7.8/tests/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 negate-0.7.8/tests/conftest.py
--rw-r--r--   0        0        0    17999 2020-02-02 00:00:00.000000 negate-0.7.8/tests/data.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 negate-0.7.8/tests/requirements.txt
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 negate-0.7.8/tests/test_negate.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 negate-0.7.8/.gitignore
--rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 negate-0.7.8/LICENSE
--rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 negate-0.7.8/README.md
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 negate-0.7.8/pyproject.toml
--rw-r--r--   0        0        0    22083 2020-02-02 00:00:00.000000 negate-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 negate-0.7.9/.deepsource.toml
+-rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 negate-0.7.9/.pylintrc
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 negate-0.7.9/test.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 negate-0.7.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 negate-0.7.9/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 negate-0.7.9/negate/__init__.py
+-rw-r--r--   0        0        0    23002 2020-02-02 00:00:00.000000 negate-0.7.9/negate/negate.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 negate-0.7.9/negate/py.typed
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 negate-0.7.9/negate/tokens.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 negate-0.7.9/tests/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 negate-0.7.9/tests/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 negate-0.7.9/tests/conftest.py
+-rw-r--r--   0        0        0    17999 2020-02-02 00:00:00.000000 negate-0.7.9/tests/data.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 negate-0.7.9/tests/requirements.txt
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 negate-0.7.9/tests/test_negate.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 negate-0.7.9/.gitignore
+-rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 negate-0.7.9/LICENSE
+-rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 negate-0.7.9/README.md
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 negate-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0    22083 2020-02-02 00:00:00.000000 negate-0.7.9/PKG-INFO
```

### Comparing `negate-0.7.8/.pylintrc` & `negate-0.7.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `negate-0.7.8/.github/workflows/run-tests.yml` & `negate-0.7.9/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `negate-0.7.8/negate/negate.py` & `negate-0.7.9/negate/negate.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,28 +181,25 @@
         # AUX as ROOT (e.g.: "I'm excited.") or ROOT children e.g.,
         # "I do think...".
         if (self._is_aux(root) or self._is_verb_to_be(root)
                 or any(self._is_aux(child) for child in root.children)):
             # If the AUX has AUX children, negate them instead. E.g.: "I will
             # be there." or "They have been moody lately."
             aux_child = self._get_aux_child(root)
-            prev_fail_on_unsupported = self.fail_on_unsupported
-            if aux_child:
-                # Handle cases such as "I expect everything to be ready."
-                self.fail_on_unsupported = True
             try:
                 return self._negate_aux_in_doc(
                     aux=root if not aux_child else aux_child,
                     doc=doc,
-                    prefer_contractions=prefer_contractions
+                    prefer_contractions=prefer_contractions,
+                    fail_on_unsupported=True
                 )
             except RuntimeError:
-                pass  # Continue trying to negate the root verb instead.
-            finally:
-                self.fail_on_unsupported = prev_fail_on_unsupported
+                # In cases such as "I expect everything to be ready.", continue
+                # trying to negate the root verb instead.
+                pass
 
         # General verb non-negated.
         negated_aux = self.negate_aux(self.conjugate_verb('do', root.tag_),
                                       prefer_contractions)
         return self._compile_sentence(
             doc,
             remove_tokens=[root.i],
@@ -238,29 +235,41 @@
     def get_base_verb(self, verb: str) -> str:
         base_verb: Tuple[str] = getLemma(verb, upos="VERB")
         return base_verb[0] if base_verb else verb
 
     def negate_aux(
         self,
         auxiliary_verb: str,
-        prefer_contractions: bool = True
+        prefer_contractions: Optional[bool] = None,
+        fail_on_unsupported: Optional[bool] = None
     ) -> Optional[str]:
+        if prefer_contractions is None:
+            prefer_contractions = True
+        if fail_on_unsupported is None:
+            fail_on_unsupported = self.fail_on_unsupported
+
         negated_aux = self._aux_negations[prefer_contractions].get(
             auxiliary_verb
         )
         if negated_aux is None:
-            self._handle_unsupported()
+            self._handle_unsupported(fail_on_unsupported)
         return negated_aux
 
     def _negate_aux_in_doc(
         self,
         aux: Union[Token, SpacyToken],
         doc: SpacyDoc,
-        prefer_contractions: bool = True
+        prefer_contractions: Optional[bool] = None,
+        fail_on_unsupported: Optional[bool] = None
     ) -> str:
+        if prefer_contractions is None:
+            prefer_contractions = True
+        if fail_on_unsupported is None:
+            fail_on_unsupported = self.fail_on_unsupported
+
         negation = self._get_negated_child(aux)
         # If AUX negated -> Remove negation.
         if negation:
             # Special case AUX "won't" -> Remove negation and replace
             # "wo" -> "will".
             if aux.text.lower() == "wo":
                 replace_aux = Token(
@@ -296,15 +305,19 @@
             if parent and (parent.tag_ == "VBN"
                     or any(child.tag_ == "VBN" for child in parent.children)):
                 # "'s" is "to have"
                 aux_text = f"{aux.text}_"
         remove = [aux.i]
         add = {
             aux.i: Token(
-                text=self.negate_aux(aux_text, prefer_contractions),
+                text=self.negate_aux(
+                    aux_text,
+                    prefer_contractions,
+                    fail_on_unsupported=fail_on_unsupported
+                ),
                 has_space_after=aux._.has_space_after
             )
         }
         # Handle e.g., "should've" -> "shouldn't have"
         if aux.i+1 < len(doc) and doc[aux.i+1].text.lower() == "'ve":
             remove.append(aux.i+1)
             add[aux.i+1] = Token(
@@ -501,22 +514,27 @@
             self.logger.info("Downloading model. This only needs to happen "
                              "once. Please, be patient...")
             with suppress_stdout():
                 spacy.cli.download(model_name, False, False, "-q")
             model_module = importlib.import_module(model_name)
         return model_module.load(**kwargs)
 
-    def _handle_unsupported(self):
+    def _handle_unsupported(self, fail: Optional[bool] = None):
         """Handle behavior upon unsupported sentences.
 
+        Args:
+            fail (:obj:`Optional[bool]`):
+                Whether to raise an exception with unsupported sentences of not.
         Raises:
             :obj:`RuntimeError`: If :arg:`fail_on_unsupported` is set to
             :obj:`True`.
         """
-        if self.fail_on_unsupported:
+        if fail is None:
+            fail = self.fail_on_unsupported
+        if fail:
             raise RuntimeError("Sentence not supported.")
         else:
             self.logger.warning("Sentence not supported. Output might be "
                                 "arbitrary.")
 
     def _initialize_aux_negations(self):
         self._aux_negations = {
```

### Comparing `negate-0.7.8/negate/tokens.py` & `negate-0.7.9/negate/tokens.py`

 * *Files identical despite different names*

### Comparing `negate-0.7.8/tests/README.md` & `negate-0.7.9/tests/README.md`

 * *Files identical despite different names*

### Comparing `negate-0.7.8/tests/conftest.py` & `negate-0.7.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `negate-0.7.8/tests/data.py` & `negate-0.7.9/tests/data.py`

 * *Files identical despite different names*

### Comparing `negate-0.7.8/tests/test_negate.py` & `negate-0.7.9/tests/test_negate.py`

 * *Files identical despite different names*

### Comparing `negate-0.7.8/.gitignore` & `negate-0.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `negate-0.7.8/LICENSE` & `negate-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `negate-0.7.8/README.md` & `negate-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `negate-0.7.8/pyproject.toml` & `negate-0.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 dependencies = [
-    "spacy[transformers]>=3.4.1,<3.6.0",
+    "spacy[transformers]>=3.4.1,<3.5.0",
     "lemminflect>=0.2.3,<0.3.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/dmlls/negate"
 "GitHub Issues" = "https://github.com/dmlls/negate/issues"
 "GitHub Repo" = "https://github.com/dmlls/negate"
```

### Comparing `negate-0.7.8/PKG-INFO` & `negate-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negate
-Version: 0.7.8
+Version: 0.7.9
 Summary: A Python module that negates sentences.
 Project-URL: Homepage, https://github.com/dmlls/negate
 Project-URL: GitHub Issues, https://github.com/dmlls/negate/issues
 Project-URL: GitHub Repo, https://github.com/dmlls/negate
 Author-email: Diego Miguel Lozano <hello@diegomiguel.me>
 Maintainer-email: Diego Miguel Lozano <hello@diegomiguel.me>
 License: 
@@ -220,15 +220,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Requires-Dist: lemminflect<0.3.0,>=0.2.3
-Requires-Dist: spacy[transformers]<3.6.0,>=3.4.1
+Requires-Dist: spacy[transformers]<3.5.0,>=3.4.1
 Description-Content-Type: text/markdown
 
 <p align="center"><img width="666" src="https://user-images.githubusercontent.com/22967053/208313993-b873be19-8648-4edd-b4ee-e5283c19ad8f.png" alt="Negate: A Python module to negate sentences."></p>
 <p align="center" display="inline-block">
   <a href="https://pypi.org/project/negate/">
     <img src="https://img.shields.io/pypi/v/negate">
   </a>
```

