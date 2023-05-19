# Comparing `tmp/llm_rs-0.2.0.tar.gz` & `tmp/llm_rs-0.2.1.tar.gz`

## Comparing `llm_rs-0.2.0.tar` & `llm_rs-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,29 @@
--rw-r--r--   0        0        0      410 1970-01-01 00:00:00.000000 llm_rs-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123      610 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.github/workflows/BuildDoc.yml
--rw-r--r--   0     1001      123     2796 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      564 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.github/workflows/Clippy.yml
--rw-r--r--   0     1001      123      602 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.github/workflows/PublishDocs.yml
--rw-r--r--   0     1001      123     3455 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.gitignore
--rw-r--r--   0     1001      123       72 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.vscode/settings.json
--rw-r--r--   0     1001      123     1071 2023-05-19 09:40:45.000000 llm_rs-0.2.0/LICENSE
--rw-r--r--   0     1001      123     1134 2023-05-19 09:40:45.000000 llm_rs-0.2.0/README.md
--rw-r--r--   0     1001      123     8622 2023-05-19 09:40:45.000000 llm_rs-0.2.0/docs/docs/index.md
--rw-r--r--   0     1001      123     1181 2023-05-19 09:40:45.000000 llm_rs-0.2.0/docs/mkdocs.yml
--rw-r--r--   0     1001      123       31 2023-05-19 09:40:45.000000 llm_rs-0.2.0/docs/requirements.txt
--rw-r--r--   0     1001      123      229 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/__init__.py
--rw-r--r--   0     1001      123     1201 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/config.pyi
--rw-r--r--   0     1001      123        0 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/llm_rs.pyi
--rw-r--r--   0     1001      123     1772 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/models.pyi
--rw-r--r--   0     1001      123        0 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/py.typed
--rw-r--r--   0     1001      123      697 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/results.pyi
--rw-r--r--   0     1001      123      737 2023-05-19 09:40:45.000000 llm_rs-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123     4274 2023-05-19 09:40:45.000000 llm_rs-0.2.0/src/configs.rs
--rw-r--r--   0     1001      123     1550 2023-05-19 09:40:45.000000 llm_rs-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123     8937 2023-05-19 09:40:45.000000 llm_rs-0.2.0/src/model_base.rs
--rw-r--r--   0     1001      123      300 2023-05-19 09:40:45.000000 llm_rs-0.2.0/src/models.rs
--rw-r--r--   0     1001      123     1352 2023-05-19 09:40:45.000000 llm_rs-0.2.0/src/results.rs
--rw-r--r--   0     1001      123    20580 2023-05-19 09:42:28.000000 llm_rs-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 llm_rs-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 llm_rs-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123      610 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.github/workflows/BuildDoc.yml
+-rw-r--r--   0     1001      123     2796 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      564 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.github/workflows/Clippy.yml
+-rw-r--r--   0     1001      123      602 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.github/workflows/PublishDocs.yml
+-rw-r--r--   0     1001      123     3455 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.gitignore
+-rw-r--r--   0     1001      123       72 2023-05-19 16:34:02.000000 llm_rs-0.2.1/.vscode/settings.json
+-rw-r--r--   0     1001      123     1071 2023-05-19 16:34:02.000000 llm_rs-0.2.1/LICENSE
+-rw-r--r--   0     1001      123     1134 2023-05-19 16:34:02.000000 llm_rs-0.2.1/README.md
+-rw-r--r--   0     1001      123     1909 2023-05-19 16:34:02.000000 llm_rs-0.2.1/docs/docs/conversion.md
+-rw-r--r--   0     1001      123     8622 2023-05-19 16:34:02.000000 llm_rs-0.2.1/docs/docs/index.md
+-rw-r--r--   0     1001      123     1181 2023-05-19 16:34:02.000000 llm_rs-0.2.1/docs/mkdocs.yml
+-rw-r--r--   0     1001      123       31 2023-05-19 16:34:02.000000 llm_rs-0.2.1/docs/requirements.txt
+-rw-r--r--   0     1001      123      263 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/__init__.py
+-rw-r--r--   0     1001      123     1299 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/config.pyi
+-rw-r--r--   0     1001      123        0 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/llm_rs.pyi
+-rw-r--r--   0     1001      123     2108 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/models.pyi
+-rw-r--r--   0     1001      123        0 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/py.typed
+-rw-r--r--   0     1001      123      697 2023-05-19 16:34:02.000000 llm_rs-0.2.1/llm_rs/results.pyi
+-rw-r--r--   0     1001      123      925 2023-05-19 16:34:02.000000 llm_rs-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123     1274 2023-05-19 16:34:02.000000 llm_rs-0.2.1/quantize.py
+-rw-r--r--   0     1001      123     4274 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/configs.rs
+-rw-r--r--   0     1001      123     1685 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123     9645 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/model_base.rs
+-rw-r--r--   0     1001      123      300 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/models.rs
+-rw-r--r--   0     1001      123     2426 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/quantize.rs
+-rw-r--r--   0     1001      123     1352 2023-05-19 16:34:02.000000 llm_rs-0.2.1/src/results.rs
+-rw-r--r--   0     1001      123    20589 2023-05-19 16:35:27.000000 llm_rs-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     2178 1970-01-01 00:00:00.000000 llm_rs-0.2.1/PKG-INFO
```

### Comparing `llm_rs-0.2.0/.github/workflows/BuildDoc.yml` & `llm_rs-0.2.1/.github/workflows/BuildDoc.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/.github/workflows/CI.yml` & `llm_rs-0.2.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/.github/workflows/Clippy.yml` & `llm_rs-0.2.1/.github/workflows/Clippy.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/.github/workflows/PublishDocs.yml` & `llm_rs-0.2.1/.github/workflows/PublishDocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/.gitignore` & `llm_rs-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/LICENSE` & `llm_rs-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/README.md` & `llm_rs-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/docs/docs/index.md` & `llm_rs-0.2.1/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/docs/mkdocs.yml` & `llm_rs-0.2.1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/llm_rs/models.pyi` & `llm_rs-0.2.1/llm_rs/models.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Callable, List
 from abc import ABC
 
-from .config import GenerationConfig, SessionConfig
+from .config import GenerationConfig, SessionConfig, ContainerType, QuantizationType
 from .results import GenerationResult
 
 #Theoretically this is incorrect as the 'model' doesnt actually exist, but it is a good enough approximation for now. 
 class Model(ABC):
     """
     Wrapper around a llm model.
     """
@@ -24,27 +24,38 @@
                   path:str,
                   session_config:SessionConfig=SessionConfig(),
                   lora_paths:Optional[List[str]]=None,
                   verbose:bool=False) -> None: ...
     
     def generate(self,prompt:str,
                  generation_config:Optional[GenerationConfig]=None,
-                 callback:Callable[[str],Optional[bool]]=None) -> GenerationResult: ...
+                 callback:Callable[[str],Optional[bool]]=None) -> GenerationResult: 
+        """
+        Generates text from a prompt.
+        """ 
+        ...
     
     def tokenize(self,text:str) -> List[int]:
         """
         Tokenizes a string into a list of tokens.
         """
         ...
     
     def decode(self,tokens:List[int]) -> str:
         """
         Decodes a list of tokens into a string.
         """
         ...
+
+    @staticmethod
+    def quantize(source:str,destination:str,quantization:QuantizationType=QuantizationType.Q4_0,container:ContainerType=ContainerType.GGJT)->None:
+        """
+        Quantizes the model.
+        """
+        ...
     
 
 class Llama(Model):
     """
     Wrapper around all Llama based models.
     """
     ...
```

### Comparing `llm_rs-0.2.0/llm_rs/results.pyi` & `llm_rs-0.2.1/llm_rs/results.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/src/configs.rs` & `llm_rs-0.2.1/src/configs.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/src/lib.rs` & `llm_rs-0.2.1/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 use pyo3::prelude::*;
 
 mod configs;
 mod model_base;
 mod models;
+mod quantize;
 mod results;
 
 #[pymodule]
 fn llm_rs(_py: Python, m: &PyModule) -> PyResult<()> {
     let config_module = PyModule::new(_py, "config")?;
     config_module.add_class::<configs::GenerationConfig>()?;
     config_module.add_class::<configs::Precision>()?;
     config_module.add_class::<configs::SessionConfig>()?;
+    config_module.add_class::<quantize::ContainerType>()?;
+    config_module.add_class::<quantize::QuantizationType>()?;
     m.add_submodule(config_module)?;
 
     let results_module = PyModule::new(_py, "results")?;
     results_module.add_class::<results::GenerationTimes>()?;
     results_module.add_class::<results::StopReason>()?;
     results_module.add_class::<results::GenerationResult>()?;
     m.add_submodule(results_module)?;
```

### Comparing `llm_rs-0.2.0/src/model_base.rs` & `llm_rs-0.2.1/src/model_base.rs`

 * *Files 12% similar despite different names*

```diff
@@ -249,12 +249,28 @@
 
             fn decode(&self, tokens: Vec<i32>) -> PyResult<String> {
                 match crate::model_base::_decode(self.llm_model.as_ref(), tokens) {
                     Ok(tokens) => Ok(tokens),
                     Err(e) => Err(pyo3::exceptions::PyException::new_err(e.to_string())),
                 }
             }
+
+            #[staticmethod]
+            fn quantize(
+                source: String,
+                destination: String,
+                quantization: Option<crate::quantize::QuantizationType>,
+                container: Option<crate::quantize::ContainerType>,
+            ) -> PyResult<()> {
+                crate::quantize::_quantize::<$llm_model>(
+                    source.into(),
+                    destination.into(),
+                    container.unwrap_or(crate::quantize::ContainerType::GGJT),
+                    quantization.unwrap_or(crate::quantize::QuantizationType::Q4_0),
+                )
+                .map_err(|e| pyo3::exceptions::PyException::new_err(e.to_string()))
+            }
         }
     };
 }
 
 pub(crate) use wrap_model;
```

### Comparing `llm_rs-0.2.0/src/results.rs` & `llm_rs-0.2.1/src/results.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.0/Cargo.lock` & `llm_rs-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -302,16 +302,17 @@
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-rs"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
+ "ggml",
  "llm",
  "llm-base",
  "log",
  "pyo3",
  "rand",
  "rand_chacha",
 ]
```

