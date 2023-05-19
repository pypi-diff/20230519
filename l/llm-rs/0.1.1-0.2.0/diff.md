# Comparing `tmp/llm_rs-0.1.1.tar.gz` & `tmp/llm_rs-0.2.0.tar.gz`

## Comparing `llm_rs-0.1.1.tar` & `llm_rs-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
--rw-r--r--   0        0        0      409 1970-01-01 00:00:00.000000 llm_rs-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123     2810 2023-05-08 14:10:49.000000 llm_rs-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3455 2023-05-08 14:10:49.000000 llm_rs-0.1.1/.gitignore
--rw-r--r--   0     1001      123       72 2023-05-08 14:10:49.000000 llm_rs-0.1.1/.vscode/settings.json
--rw-r--r--   0     1001      123     1071 2023-05-08 14:10:49.000000 llm_rs-0.1.1/LICENSE
--rw-r--r--   0     1001      123     1913 2023-05-08 14:10:49.000000 llm_rs-0.1.1/README.md
--rw-r--r--   0     1001      123      221 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/__init__.py
--rw-r--r--   0     1001      123     1201 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/config.pyi
--rw-r--r--   0     1001      123        0 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/llm_rs.pyi
--rw-r--r--   0     1001      123     1528 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/models.pyi
--rw-r--r--   0     1001      123        0 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/py.typed
--rw-r--r--   0     1001      123      697 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/results.pyi
--rw-r--r--   0     1001      123      709 2023-05-08 14:10:49.000000 llm_rs-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123     4127 2023-05-08 14:10:49.000000 llm_rs-0.1.1/src/configs.rs
--rw-r--r--   0     1001      123     1502 2023-05-08 14:10:49.000000 llm_rs-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123     8693 2023-05-08 14:10:49.000000 llm_rs-0.1.1/src/model_base.rs
--rw-r--r--   0     1001      123      253 2023-05-08 14:10:49.000000 llm_rs-0.1.1/src/models.rs
--rw-r--r--   0     1001      123     1263 2023-05-08 14:10:49.000000 llm_rs-0.1.1/src/results.rs
--rw-r--r--   0     1001      123    20390 2023-05-08 14:11:58.000000 llm_rs-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 llm_rs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      410 1970-01-01 00:00:00.000000 llm_rs-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123      610 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.github/workflows/BuildDoc.yml
+-rw-r--r--   0     1001      123     2796 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      564 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.github/workflows/Clippy.yml
+-rw-r--r--   0     1001      123      602 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.github/workflows/PublishDocs.yml
+-rw-r--r--   0     1001      123     3455 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.gitignore
+-rw-r--r--   0     1001      123       72 2023-05-19 09:40:45.000000 llm_rs-0.2.0/.vscode/settings.json
+-rw-r--r--   0     1001      123     1071 2023-05-19 09:40:45.000000 llm_rs-0.2.0/LICENSE
+-rw-r--r--   0     1001      123     1134 2023-05-19 09:40:45.000000 llm_rs-0.2.0/README.md
+-rw-r--r--   0     1001      123     8622 2023-05-19 09:40:45.000000 llm_rs-0.2.0/docs/docs/index.md
+-rw-r--r--   0     1001      123     1181 2023-05-19 09:40:45.000000 llm_rs-0.2.0/docs/mkdocs.yml
+-rw-r--r--   0     1001      123       31 2023-05-19 09:40:45.000000 llm_rs-0.2.0/docs/requirements.txt
+-rw-r--r--   0     1001      123      229 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/__init__.py
+-rw-r--r--   0     1001      123     1201 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/config.pyi
+-rw-r--r--   0     1001      123        0 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/llm_rs.pyi
+-rw-r--r--   0     1001      123     1772 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/models.pyi
+-rw-r--r--   0     1001      123        0 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/py.typed
+-rw-r--r--   0     1001      123      697 2023-05-19 09:40:45.000000 llm_rs-0.2.0/llm_rs/results.pyi
+-rw-r--r--   0     1001      123      737 2023-05-19 09:40:45.000000 llm_rs-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123     4274 2023-05-19 09:40:45.000000 llm_rs-0.2.0/src/configs.rs
+-rw-r--r--   0     1001      123     1550 2023-05-19 09:40:45.000000 llm_rs-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     8937 2023-05-19 09:40:45.000000 llm_rs-0.2.0/src/model_base.rs
+-rw-r--r--   0     1001      123      300 2023-05-19 09:40:45.000000 llm_rs-0.2.0/src/models.rs
+-rw-r--r--   0     1001      123     1352 2023-05-19 09:40:45.000000 llm_rs-0.2.0/src/results.rs
+-rw-r--r--   0     1001      123    20580 2023-05-19 09:42:28.000000 llm_rs-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 llm_rs-0.2.0/PKG-INFO
```

### Comparing `llm_rs-0.1.1/.github/workflows/CI.yml` & `llm_rs-0.2.0/.github/workflows/CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   contents: read
 
 jobs:
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        target: [x86_64, x86] #aarch64, armv7, s390x, ppc64le]
+        target: [x86_64, x86] #, s390x, ppc64le]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
```

### Comparing `llm_rs-0.1.1/.gitignore` & `llm_rs-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.1/LICENSE` & `llm_rs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.1/llm_rs/config.pyi` & `llm_rs-0.2.0/llm_rs/config.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,31 +9,31 @@
     """
     Configuration parameters for the generation process.
     """
     top_k:int
     top_p:float
     temperature:float
     repetition_penalty:float
+    repetition_penalty_last_n:int
     seed:int
     max_new_tokens:Optional[int]
     stop_words:Optional[List[str]]
     
-    def  __init__(self,top_k:int=40,top_p:float=0.95,temperature:float=0.8,repetition_penalty:float=1.3,seed:int=42,max_new_tokens:Optional[int]=None,stop_words:Optional[List[str]]=None) -> None: ...
+    def  __init__(self,top_k:int=40,top_p:float=0.95,temperature:float=0.8,repetition_penalty:float=1.3,repetition_penalty_last_n:int=512,seed:int=42,max_new_tokens:Optional[int]=None,stop_words:Optional[List[str]]=None) -> None: ...
     
 class SessionConfig():
     """
     Configure the generation session that will be used for all generations.
     """
     threads:int
     batch_size:int
-    repetition_penalty_last_n:int
     keys_memory_type:Precision
     values_memory_type:Precision
     
     
     @property
     def context_length(self)->int: ...
     
     @property
     def prefer_mmap(self)->bool:...
     
-    def  __init__(self,threads:int=8,batch_size:int=8,context_length:int=2048,repetition_penalty_last_n:int=512,keys_memory_type:Precision=Precision.FP32,values_memory_type:Precision=values_memory_type.FP32,prefer_mmap:bool=True) -> None: ...
+    def  __init__(self,threads:int=8,batch_size:int=8,context_length:int=2048,keys_memory_type:Precision=Precision.FP32,values_memory_type:Precision=values_memory_type.FP32,prefer_mmap:bool=True) -> None: ...
```

### Comparing `llm_rs-0.1.1/llm_rs/models.pyi` & `llm_rs-0.2.0/llm_rs/models.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, Callable, List
-from abc import ABC, abstractmethod
+from abc import ABC
 
 from .config import GenerationConfig, SessionConfig
 from .results import GenerationResult
 
 #Theoretically this is incorrect as the 'model' doesnt actually exist, but it is a good enough approximation for now. 
 class Model(ABC):
     """
@@ -12,16 +12,23 @@
     config:SessionConfig
     
     @property
     def path(self)->str: ...
     
     @property
     def verbose(self)->bool: ...
-    
-    def  __init__(self,path:str,session_config:SessionConfig=SessionConfig(), verbose:bool=False) -> None: ...
+
+    @property
+    def lora_paths(self)->Optional[List[str]]: ...
+
+    def  __init__(self,
+                  path:str,
+                  session_config:SessionConfig=SessionConfig(),
+                  lora_paths:Optional[List[str]]=None,
+                  verbose:bool=False) -> None: ...
     
     def generate(self,prompt:str,
                  generation_config:Optional[GenerationConfig]=None,
                  callback:Callable[[str],Optional[bool]]=None) -> GenerationResult: ...
     
     def tokenize(self,text:str) -> List[int]:
         """
@@ -39,30 +46,36 @@
 class Llama(Model):
     """
     Wrapper around all Llama based models.
     """
     ...
     
     
-class GPTJ(Model):
+class GptJ(Model):
     """
     Wrapper around all GPTJ based models.
     """
     ...
     
-class GPT2(Model):
+class Gpt2(Model):
     """
     Wrapper around all GPT2 based models.
     """
     ...
     
 class Bloom(Model):
     """
     Wrapper around all Bloom based models.
     """
     ...
     
-class NeoX(Model):
+class GptNeoX(Model):
     """
     Wrapper around all GPT-NeoX based models.
     """
+    ...
+
+class Mpt(Model):
+    """
+    Wrapper around all Mpt based models.
+    """
     ...
```

### Comparing `llm_rs-0.1.1/llm_rs/results.pyi` & `llm_rs-0.2.0/llm_rs/results.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.1/pyproject.toml` & `llm_rs-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
+keywords = ["LLM","Transformers"]
 
 [project.urls]
-"Homepage" = "https://github.com/LLukas22/llm-rs-python"
-"Bug Tracker" = "https://github.com/LLukas22/llm-rs-python/issues"
+repository = "https://github.com/LLukas22/llm-rs-python"
+documentation  = "https://llukas22.github.io/llm-rs-python/"
 
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
```

### Comparing `llm_rs-0.1.1/src/configs.rs` & `llm_rs-0.2.0/src/configs.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,155 +1,157 @@
+use llm::{InferenceParameters, InferenceSessionConfig, ModelKVMemoryType, TokenBias};
 use pyo3::prelude::*;
-use llm::{InferenceParameters,ModelKVMemoryType,TokenBias,InferenceSessionParameters};
 
 #[pyclass]
 pub struct GenerationConfig {
     #[pyo3(get, set)]
-    pub top_k:usize,
+    pub top_k: usize,
     #[pyo3(get, set)]
-    pub top_p:f32,
+    pub top_p: f32,
     #[pyo3(get, set)]
-    pub temperature:f32,
+    pub temperature: f32,
     #[pyo3(get, set)]
-    pub repetition_penalty:f32,
+    pub repetition_penalty: f32,
     #[pyo3(get, set)]
-    pub seed:u64,
+    pub repetition_penalty_last_n: usize,
     #[pyo3(get, set)]
-    pub max_new_tokens :Option<usize>,
+    pub seed: u64,
     #[pyo3(get, set)]
-    pub stop_words :Option<Vec<String>>,
+    pub max_new_tokens: Option<usize>,
+    #[pyo3(get, set)]
+    pub stop_words: Option<Vec<String>>,
 }
 
 impl Default for GenerationConfig {
     fn default() -> Self {
         Self {
-            top_k:40,
-            top_p:0.95,
-            temperature:0.80,
-            repetition_penalty:1.30,
-            seed:42,
-            max_new_tokens :None,
-            stop_words :None,
+            top_k: 40,
+            top_p: 0.95,
+            temperature: 0.80,
+            repetition_penalty: 1.30,
+            repetition_penalty_last_n: 512,
+            seed: 42,
+            max_new_tokens: None,
+            stop_words: None,
         }
     }
 }
 
 #[pymethods]
 impl GenerationConfig {
-
     #[new]
-    fn new(top_k: Option<usize>,top_p:Option<f32>,temperature:Option<f32>,repetition_penalty:Option<f32>,seed:Option<u64>, max_new_tokens:Option<usize>,stop_words:Option<Vec<String>>) -> Self {
+    #[allow(clippy::too_many_arguments)]
+    fn new(
+        top_k: Option<usize>,
+        top_p: Option<f32>,
+        temperature: Option<f32>,
+        repetition_penalty: Option<f32>,
+        repetition_penalty_last_n: Option<usize>,
+        seed: Option<u64>,
+        max_new_tokens: Option<usize>,
+        stop_words: Option<Vec<String>>,
+    ) -> Self {
         GenerationConfig {
             top_k: top_k.unwrap_or(40),
             top_p: top_p.unwrap_or(0.95),
             temperature: temperature.unwrap_or(0.80),
             repetition_penalty: repetition_penalty.unwrap_or(1.30),
+            repetition_penalty_last_n: repetition_penalty_last_n.unwrap_or(512),
             seed: seed.unwrap_or(42),
-            max_new_tokens:max_new_tokens,
-            stop_words:stop_words,
+            max_new_tokens,
+            stop_words,
         }
     }
 }
 
-impl GenerationConfig{
-    pub fn to_llama_rs_params(&self,n_threads:usize,n_batch:usize)->InferenceParameters{
-        InferenceParameters{
+impl GenerationConfig {
+    pub fn to_llm_params(&self, n_threads: usize, n_batch: usize) -> InferenceParameters {
+        InferenceParameters {
             top_k: self.top_k,
             top_p: self.top_p,
             temperature: self.temperature,
             repeat_penalty: self.repetition_penalty,
+            repetition_penalty_last_n: self.repetition_penalty_last_n,
             bias_tokens: TokenBias::default(),
-            n_threads: n_threads,
-            n_batch: n_batch,
+            n_threads,
+            n_batch,
         }
     }
 }
 
-
-
 #[pyclass]
 #[derive(Clone, Copy, Debug, PartialEq)]
-pub enum Precision{
+pub enum Precision {
     FP32,
     FP16,
 }
 
-impl Precision{
-    pub fn to_llama_rs_memory_type(&self)->
-    ModelKVMemoryType{
-        match self{
-            Precision::FP16=>ModelKVMemoryType::Float16,
-            Precision::FP32=>ModelKVMemoryType::Float32,
+impl Precision {
+    pub fn to_llama_rs_memory_type(self) -> ModelKVMemoryType {
+        match self {
+            Precision::FP16 => ModelKVMemoryType::Float16,
+            Precision::FP32 => ModelKVMemoryType::Float32,
         }
     }
 }
 
-
 #[pyclass]
 #[derive(Clone, Copy)]
 pub struct SessionConfig {
     #[pyo3(get, set)]
-    pub threads:usize,
+    pub threads: usize,
     #[pyo3(get, set)]
-    pub batch_size:usize,
+    pub batch_size: usize,
     #[pyo3(get)]
-    pub context_length:usize,
+    pub context_length: usize,
     #[pyo3(get, set)]
-    pub repetition_penalty_last_n:usize,
+    pub keys_memory_type: Precision,
     #[pyo3(get, set)]
-    pub keys_memory_type:Precision,
-    #[pyo3(get, set)]
-    pub values_memory_type:Precision,
+    pub values_memory_type: Precision,
     #[pyo3(get)]
-    pub prefer_mmap:bool,
+    pub prefer_mmap: bool,
 }
 
 impl Default for SessionConfig {
     fn default() -> Self {
         Self {
-            threads:8,
-            batch_size:8,
-            context_length:2048,
-            repetition_penalty_last_n:512,
-            keys_memory_type:Precision::FP32,
-            values_memory_type:Precision::FP32,
-            prefer_mmap:true,
+            threads: 8,
+            batch_size: 8,
+            context_length: 2048,
+            keys_memory_type: Precision::FP32,
+            values_memory_type: Precision::FP32,
+            prefer_mmap: true,
         }
     }
 }
 
 #[pymethods]
 impl SessionConfig {
     #[new]
-    fn new(threads: Option<usize>,
-        batch_size:Option<usize>,
-        context_length:Option<usize>,
-        repetition_penalty_last_n:Option<usize>,
-        keys_memory_type:Option<Precision>,
-        values_memory_type:Option<Precision>,
-        prefer_mmap:Option<bool>
+    #[allow(clippy::too_many_arguments)]
+    fn new(
+        threads: Option<usize>,
+        batch_size: Option<usize>,
+        context_length: Option<usize>,
+        keys_memory_type: Option<Precision>,
+        values_memory_type: Option<Precision>,
+        prefer_mmap: Option<bool>,
     ) -> Self {
         SessionConfig {
-            threads:threads.unwrap_or(8),
-            batch_size:batch_size.unwrap_or(8),
-            context_length:context_length.unwrap_or(2048),
-            repetition_penalty_last_n:repetition_penalty_last_n.unwrap_or(512),
-            keys_memory_type:keys_memory_type.unwrap_or(Precision::FP32),
-            values_memory_type:values_memory_type.unwrap_or(Precision::FP32),
-            prefer_mmap:prefer_mmap.unwrap_or(true),
+            threads: threads.unwrap_or(8),
+            batch_size: batch_size.unwrap_or(8),
+            context_length: context_length.unwrap_or(2048),
+            keys_memory_type: keys_memory_type.unwrap_or(Precision::FP32),
+            values_memory_type: values_memory_type.unwrap_or(Precision::FP32),
+            prefer_mmap: prefer_mmap.unwrap_or(true),
         }
     }
 }
 
-impl SessionConfig{
-    pub fn to_llama_rs_params(&self)->InferenceSessionParameters{
-        InferenceSessionParameters{
-            repetition_penalty_last_n: self.repetition_penalty_last_n,
+impl SessionConfig {
+    pub fn to_llm_params(self) -> InferenceSessionConfig {
+        InferenceSessionConfig {
             memory_k_type: self.keys_memory_type.to_llama_rs_memory_type(),
             memory_v_type: self.values_memory_type.to_llama_rs_memory_type(),
         }
     }
 }
-
-
-
-
```

### Comparing `llm_rs-0.1.1/src/lib.rs` & `llm_rs-0.2.0/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 use pyo3::prelude::*;
 
 mod configs;
-mod results;
-mod models;
 mod model_base;
+mod models;
+mod results;
 
 #[pymodule]
 fn llm_rs(_py: Python, m: &PyModule) -> PyResult<()> {
-
     let config_module = PyModule::new(_py, "config")?;
     config_module.add_class::<configs::GenerationConfig>()?;
     config_module.add_class::<configs::Precision>()?;
     config_module.add_class::<configs::SessionConfig>()?;
     m.add_submodule(config_module)?;
 
     let results_module = PyModule::new(_py, "results")?;
     results_module.add_class::<results::GenerationTimes>()?;
     results_module.add_class::<results::StopReason>()?;
     results_module.add_class::<results::GenerationResult>()?;
     m.add_submodule(results_module)?;
 
-
     let models_module = PyModule::new(_py, "models")?;
     models_module.add_class::<models::Llama>()?;
-    models_module.add_class::<models::GPTJ>()?;
-    models_module.add_class::<models::GPT2>()?;
-    models_module.add_class::<models::NeoX>()?;
+    models_module.add_class::<models::GptJ>()?;
+    models_module.add_class::<models::Gpt2>()?;
+    models_module.add_class::<models::GptNeoX>()?;
     models_module.add_class::<models::Bloom>()?;
+    models_module.add_class::<models::Mpt>()?;
     m.add_submodule(models_module)?;
 
     //hacky but apparently the only way to get a submodule to work on all platforms with typehints
     //see https://github.com/PyO3/pyo3/issues/759
     _py.import("sys")?
         .getattr("modules")?
         .set_item("llm_rs.config", config_module)?;
```

### Comparing `llm_rs-0.1.1/src/model_base.rs` & `llm_rs-0.2.0/src/model_base.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,237 +1,260 @@
-use pyo3::prelude::*;
 use pyo3::exceptions::PyException;
-use pyo3::types::{PyTuple};
+use pyo3::prelude::*;
+use pyo3::types::PyTuple;
 
-use llm::{InferenceError, TokenUtf8Buffer,};
-use llm_base::{EvaluateOutputRequest};
+use llm::{InferenceError, TokenUtf8Buffer};
+use llm_base::{InferenceFeedback, OutputRequest};
 
-use rand_chacha::ChaCha8Rng;
 use rand::prelude::*;
+use rand_chacha::ChaCha8Rng;
+
+use std::convert::Infallible;
 
 use crate::configs;
 use crate::results;
 
-
-pub fn _tokenize(model: & dyn llm::Model,text: &str) -> Result<Vec<i32>,InferenceError>{
-    Ok(model.vocabulary()
-        .tokenize(text,false)?
+pub fn _tokenize(model: &dyn llm::Model, text: &str) -> Result<Vec<i32>, InferenceError> {
+    Ok(model
+        .vocabulary()
+        .tokenize(text, false)?
         .iter()
         .map(|(_, token)| *token)
         .collect())
 }
 
-pub fn _decode(model: & dyn llm::Model,tokens: Vec<i32>) -> Result<String,std::str::Utf8Error>{
+pub fn _decode(model: &dyn llm::Model, tokens: Vec<i32>) -> Result<String, std::str::Utf8Error> {
     let vocab = model.vocabulary();
-    let characters:Vec<u8> = tokens
-    .into_iter()
-    .map(|token| vocab.id_to_token[token as usize].to_owned())
-    .flatten()
-    .collect();
+    let characters: Vec<u8> = tokens
+        .into_iter()
+        .flat_map(|token| vocab.id_to_token[token as usize].to_owned())
+        .collect();
 
-    match std::str::from_utf8(&characters){
+    match std::str::from_utf8(&characters) {
         Ok(text) => Ok(text.to_string()),
         Err(e) => Err(e),
     }
 }
 
-
 pub fn _generate(
-        _py: Python,
-        model: & dyn llm::Model,
-        session_config: &configs::SessionConfig,
-        prompt: String,
-        generation_config: Option<&configs::GenerationConfig>,
-        callback: Option<PyObject>,)->Result<results::GenerationResult,PyErr>{
-
-            let session_params = session_config.to_llama_rs_params();
-        
-            //Build the correct generation parameters
-            let default_config = configs::GenerationConfig::default();
-            let config_to_use = generation_config.unwrap_or(&default_config);
-    
-            let generation_params = config_to_use.to_llama_rs_params(session_config.threads,  session_config.batch_size);
-    
-            let mut rng = ChaCha8Rng::seed_from_u64(config_to_use.seed);
-            let prompt = prompt.as_str();
-    
-            let mut session = model.start_session(session_params);
-    
-            //Extract the callback function from the python object
-            let mut callback_function: Option<&PyAny> = None;
-            let pytohn_object: Py<PyAny>;
-    
-            if let Some(unwrapped) = callback {
-                pytohn_object = unwrapped;
-                let python_function = pytohn_object.as_ref(_py);
-                callback_function = Some(python_function);
-                assert!(python_function.is_callable(), "Callback is not callable!");
-            }
-    
-            let feed_start_at = std::time::SystemTime::now();
-            //Feed the prompt
-            
-            
-            let mut output_request_feeding = EvaluateOutputRequest::default();
-            _py.allow_threads(||session.feed_prompt(model, &generation_params, &prompt, &mut output_request_feeding,|_| {
-                Ok::<(),InferenceError>(())
-            }).unwrap());
-            let feed_prompt_duration = feed_start_at.elapsed().unwrap();
-    
-    
-            //Start the inference loop
-            let mut tokens_processed = 0;
-            let mut token_utf8_buf = TokenUtf8Buffer::new();
-    
-            let mut total_generated_text = String::new();
-            let stop_reason ;
-    
-            let generation_start_at = std::time::SystemTime::now();
-
-       
-            let mut output_request_generation = EvaluateOutputRequest::default();   
-            let mut _generate_next_tokens= ||-> Result<Option<String>, PyErr>{
-                
-                let token = match session.infer_next_token(model, &generation_params, &mut output_request_generation,&mut rng) {
-                    Ok(token) => token,
-                    Err(InferenceError::EndOfText) => return Ok(None),
-                    Err(e) => return Err(PyException::new_err(e.to_string())),
-                };
-                Ok(token_utf8_buf.push(token))
+    _py: Python,
+    model: &dyn llm::Model,
+    session_config: &configs::SessionConfig,
+    prompt: String,
+    generation_config: Option<&configs::GenerationConfig>,
+    callback: Option<PyObject>,
+) -> Result<results::GenerationResult, PyErr> {
+    let session_params = session_config.to_llm_params();
+
+    //Build the correct generation parameters
+    let default_config = configs::GenerationConfig::default();
+    let config_to_use = generation_config.unwrap_or(&default_config);
+
+    let generation_params =
+        config_to_use.to_llm_params(session_config.threads, session_config.batch_size);
+
+    let mut rng = ChaCha8Rng::seed_from_u64(config_to_use.seed);
+    let prompt = prompt.as_str();
+
+    let mut session = model.start_session(session_params);
+
+    //Extract the callback function from the python object
+    let mut callback_function: Option<&PyAny> = None;
+    let pytohn_object: Py<PyAny>;
+
+    if let Some(unwrapped) = callback {
+        pytohn_object = unwrapped;
+        let python_function = pytohn_object.as_ref(_py);
+        callback_function = Some(python_function);
+        assert!(python_function.is_callable(), "Callback is not callable!");
+    }
 
-            };
+    let feed_start_at = std::time::SystemTime::now();
+    //Feed the prompt
 
-            loop {
-                //Check if we have reached the maximum token count
-                if config_to_use.max_new_tokens.is_some() && tokens_processed >= config_to_use.max_new_tokens.unwrap() {
-                    stop_reason=results::StopReason::MaxLength;
-                    break;
-                }
-    
-                //Infere the next token and break if the END_OF_TEXT token is reached
-                
-                let mut token:Option<String> = None;
-                _py.allow_threads(|| token=_generate_next_tokens().unwrap());
-               
+    let mut output_request_feeding = OutputRequest::default();
+    _py.allow_threads(|| {
+        session
+            .feed_prompt::<Infallible>(
+                model,
+                &generation_params,
+                prompt,
+                &mut output_request_feeding,
+                |_| Ok(InferenceFeedback::Continue),
+            )
+            .unwrap()
+    });
+    let feed_prompt_duration = feed_start_at.elapsed().unwrap();
+
+    //Start the inference loop
+    let mut tokens_processed = 0;
+    let mut token_utf8_buf = TokenUtf8Buffer::new();
+
+    let mut total_generated_text = String::new();
+    let stop_reason;
+
+    let generation_start_at = std::time::SystemTime::now();
+
+    let mut output_request_generation = OutputRequest::default();
+    let mut _generate_next_tokens = || -> Result<Option<String>, PyErr> {
+        let token = match session.infer_next_token(
+            model,
+            &generation_params,
+            &mut output_request_generation,
+            &mut rng,
+        ) {
+            Ok(token) => token,
+            Err(InferenceError::EndOfText) => return Ok(None),
+            Err(e) => return Err(PyException::new_err(e.to_string())),
+        };
+        Ok(token_utf8_buf.push(token))
+    };
+
+    loop {
+        //Check if we have reached the maximum token count
+        if config_to_use.max_new_tokens.is_some()
+            && tokens_processed >= config_to_use.max_new_tokens.unwrap()
+        {
+            stop_reason = results::StopReason::MaxLength;
+            break;
+        }
 
-                if token.is_none() {
-                    stop_reason=results::StopReason::EndToken;
+        //Infere the next token and break if the END_OF_TEXT token is reached
+
+        let mut token: Option<String> = None;
+        _py.allow_threads(|| token = _generate_next_tokens().unwrap());
+
+        if token.is_none() {
+            stop_reason = results::StopReason::EndToken;
+            break;
+        }
+        //Buffer until a valid utf8 sequence is found
+        if let Some(tokens) = token {
+            total_generated_text.push_str(&tokens);
+            //Check if the callback function is set and call it
+            if let Some(function) = callback_function {
+                let args = PyTuple::new(_py, &[tokens]);
+                let result = function.call1(args)?;
+                //Check if the callback function returned true
+                if !result.is_none() && result.is_true()? {
+                    //If the callback function returned true, stop the generation
+                    stop_reason = results::StopReason::UserCancelled;
                     break;
                 }
-                //Buffer until a valid utf8 sequence is found
-                if let Some(tokens) = token {
-    
-                    total_generated_text.push_str(&tokens);
-                    //Check if the callback function is set and call it
-                    if let Some(function) = callback_function {
-                        let args = PyTuple::new(_py, &[tokens]);
-                        let result = function.call1(args)?;
-                        //Check if the callback function returned true
-                        if !result.is_none() {
-                            if result.is_true()? {
-                                //If the callback function returned true, stop the generation
-                                stop_reason=results::StopReason::UserCancelled;
-                                break;
-                            }
-                        }
-                    }
-                }
-    
-                tokens_processed += 1;
             }
-            
-           
+        }
 
-            let generation_duration = generation_start_at.elapsed().unwrap();
-    
-            let result = results::GenerationResult{
-                text:total_generated_text,
-                times: results::GenerationTimes{
-                    total:generation_duration.as_millis()+feed_prompt_duration.as_millis(),
-                    generation:generation_duration.as_millis(),
-                    prompt_feeding:feed_prompt_duration.as_millis()},
-                stop_reason:stop_reason
-                };
-    
-            Ok(result)
-}
+        tokens_processed += 1;
+    }
 
-   
+    let generation_duration = generation_start_at.elapsed().unwrap();
 
+    let result = results::GenerationResult {
+        text: total_generated_text,
+        times: results::GenerationTimes {
+            total: generation_duration.as_millis() + feed_prompt_duration.as_millis(),
+            generation: generation_duration.as_millis(),
+            prompt_feeding: feed_prompt_duration.as_millis(),
+        },
+        stop_reason,
+    };
 
+    Ok(result)
+}
 
 macro_rules! wrap_model {
     ($name:ident,$llm_model:ty) => {
         #[pyclass]
+        #[allow(clippy::upper_case_acronyms)]
         pub struct $name {
-
-            #[pyo3(get,set)]
+            #[pyo3(get, set)]
             pub config: crate::configs::SessionConfig,
             #[pyo3(get)]
             pub verbose: bool,
             #[pyo3(get)]
             pub path: String,
-            pub llm_model: Box<dyn llm::Model>
+            #[pyo3(get)]
+            pub lora_paths: Option<Vec<String>>,
+            pub llm_model: Box<dyn llm::Model>,
         }
 
         #[pymethods]
         impl $name {
-            
             #[new]
-            fn new(path: String, session_config:Option<crate::configs::SessionConfig>,verbose:Option<bool>) -> Self {                
+            fn new(
+                path: String,
+                session_config: Option<crate::configs::SessionConfig>,
+                lora_paths: Option<Vec<String>>,
+                verbose: Option<bool>,
+            ) -> Self {
                 let should_log = verbose.unwrap_or(false);
 
                 //Build the correct session parameters
                 let default_config = crate::configs::SessionConfig::default();
                 let config_to_use = session_config.unwrap_or(default_config);
-            
+
                 let path = std::path::Path::new(&path);
-                let model_params =  llm_base::ModelParameters{
+                let lora_paths = lora_paths
+                    .map(|strings| strings.into_iter().map(std::path::PathBuf::from).collect());
+                let model_params = llm_base::ModelParameters {
                     n_context_tokens: config_to_use.context_length,
                     prefer_mmap: config_to_use.prefer_mmap,
+                    lora_adapters: lora_paths.clone(),
                     ..Default::default()
                 };
-                let llm_model: $llm_model = llm_base::load(
-                    &path,
-                    model_params,
-                    |load_progress| {
-                    if should_log{
-                        llm_base::load_progress_callback_stdout(load_progress)
-                    }
-                }).unwrap();
-
-                
-                $name { config: config_to_use,verbose: should_log,path: path.to_str().unwrap().to_string(),llm_model:Box::new(llm_model) }
-            } 
+                let llm_model: $llm_model =
+                    llm_base::load(&path, model_params, None, |load_progress| {
+                        if should_log {
+                            llm_base::load_progress_callback_stdout(load_progress)
+                        }
+                    })
+                    .unwrap();
+
+                $name {
+                    config: config_to_use,
+                    verbose: should_log,
+                    path: path.to_str().unwrap().to_string(),
+                    llm_model: Box::new(llm_model),
+                    lora_paths: lora_paths.map(|paths| {
+                        paths
+                            .into_iter()
+                            .map(|p| p.to_str().unwrap().to_string())
+                            .collect()
+                    }),
+                }
+            }
 
             fn generate(
                 &self,
                 _py: Python,
                 prompt: String,
                 generation_config: Option<&crate::configs::GenerationConfig>,
                 callback: Option<PyObject>,
             ) -> PyResult<crate::results::GenerationResult> {
-
-                return crate::model_base::_generate(_py,self.llm_model.as_ref(),&self.config,prompt, generation_config, callback);
+                return crate::model_base::_generate(
+                    _py,
+                    self.llm_model.as_ref(),
+                    &self.config,
+                    prompt,
+                    generation_config,
+                    callback,
+                );
             }
 
-            fn tokenize(&self,text:String)-> PyResult<Vec<i32>>{
-                match crate::model_base::_tokenize(self.llm_model.as_ref(),&text){
+            fn tokenize(&self, text: String) -> PyResult<Vec<i32>> {
+                match crate::model_base::_tokenize(self.llm_model.as_ref(), &text) {
                     Ok(tokens) => Ok(tokens),
-                    Err(e) => Err(pyo3::exceptions::PyException::new_err(e.to_string()))
+                    Err(e) => Err(pyo3::exceptions::PyException::new_err(e.to_string())),
                 }
             }
 
-            fn decode(&self,tokens:Vec<i32>)-> PyResult<String>{
-                match crate::model_base::_decode(self.llm_model.as_ref(),tokens){
+            fn decode(&self, tokens: Vec<i32>) -> PyResult<String> {
+                match crate::model_base::_decode(self.llm_model.as_ref(), tokens) {
                     Ok(tokens) => Ok(tokens),
-                    Err(e) => Err(pyo3::exceptions::PyException::new_err(e.to_string()))
+                    Err(e) => Err(pyo3::exceptions::PyException::new_err(e.to_string())),
                 }
             }
         }
-
-
-        };
+    };
 }
 
-
-pub(crate) use wrap_model;
+pub(crate) use wrap_model;
```

### Comparing `llm_rs-0.1.1/src/results.rs` & `llm_rs-0.2.0/src/results.rs`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,25 @@
     pub generation: u128,
     #[pyo3(get)]
     pub prompt_feeding: u128,
 }
 
 impl fmt::Display for GenerationTimes {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        write!(f, "(Total: {} ms, Feeding: {} ms, Generation: {} ms)", self.total, self.prompt_feeding, self.generation)
+        write!(
+            f,
+            "(Total: {} ms, Feeding: {} ms, Generation: {} ms)",
+            self.total, self.prompt_feeding, self.generation
+        )
     }
 }
 
 #[pyclass]
 #[derive(Clone)]
-pub enum StopReason{
+pub enum StopReason {
     EndToken,
     MaxLength,
     UserCancelled,
 }
 
 impl fmt::Display for StopReason {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
@@ -32,24 +36,26 @@
             StopReason::EndToken => write!(f, "EndToken"),
             StopReason::MaxLength => write!(f, "MaxLength"),
             StopReason::UserCancelled => write!(f, "UserCancelled"),
         }
     }
 }
 
-
 #[pyclass]
 pub struct GenerationResult {
     #[pyo3(get)]
     pub text: String,
     #[pyo3(get)]
     pub times: GenerationTimes,
     #[pyo3(get)]
     pub stop_reason: StopReason,
 }
 
 #[pymethods]
 impl GenerationResult {
-   fn __repr__(&self)->PyResult<String>{
-       Ok(format!("GenerationResult(text='{}', times={}, stop_reason={})",self.text,self.times,self.stop_reason))
+    fn __repr__(&self) -> PyResult<String> {
+        Ok(format!(
+            "GenerationResult(text='{}', times={}, stop_reason={})",
+            self.text, self.times, self.stop_reason
+        ))
     }
-}
+}
```

### Comparing `llm_rs-0.1.1/Cargo.lock` & `llm_rs-0.2.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -132,25 +132,25 @@
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "ggml"
-version = "0.1.0-rc3"
-source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
+version = "0.1.1"
+source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
 dependencies = [
  "ggml-sys",
  "thiserror",
 ]
 
 [[package]]
 name = "ggml-sys"
-version = "0.1.0-rc3"
-source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
+version = "0.1.1"
+source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "half"
 version = "2.2.1"
@@ -210,95 +210,107 @@
 name = "libc"
 version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "llm"
-version = "0.1.0-rc3"
-source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
+version = "0.1.1"
+source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
 dependencies = [
  "llm-base",
  "llm-bloom",
  "llm-gpt2",
  "llm-gptj",
+ "llm-gptneox",
  "llm-llama",
- "llm-neox",
+ "llm-mpt",
+ "serde",
 ]
 
 [[package]]
 name = "llm-base"
-version = "0.1.0-rc3"
-source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
+version = "0.1.1"
+source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
 dependencies = [
  "bytemuck",
  "ggml",
  "half",
  "memmap2",
  "partial_sort",
  "rand",
  "serde",
  "serde_bytes",
  "thiserror",
 ]
 
 [[package]]
 name = "llm-bloom"
-version = "0.1.0-rc3"
-source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
+version = "0.1.1"
+source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gpt2"
-version = "0.1.0-rc3"
-source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
+version = "0.1.1"
+source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gptj"
-version = "0.1.0-rc3"
-source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
+version = "0.1.1"
+source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
+dependencies = [
+ "bytemuck",
+ "llm-base",
+]
+
+[[package]]
+name = "llm-gptneox"
+version = "0.1.1"
+source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
 dependencies = [
  "bytemuck",
  "llm-base",
+ "serde",
 ]
 
 [[package]]
 name = "llm-llama"
-version = "0.1.0-rc3"
-source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
+version = "0.1.1"
+source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
 dependencies = [
  "bytemuck",
  "llm-base",
  "protobuf",
  "rand",
  "rust_tokenizers",
  "serde",
  "serde_json",
  "thiserror",
 ]
 
 [[package]]
-name = "llm-neox"
-version = "0.1.0-rc3"
-source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
+name = "llm-mpt"
+version = "0.1.1"
+source = "git+https://github.com/rustformers/llm.git#99adc84d2b4cbda400ff26bde187dd5c73b3b120"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-rs"
-version = "0.1.1"
+version = "0.2.0"
 dependencies = [
  "llm",
  "llm-base",
  "log",
  "pyo3",
  "rand",
  "rand_chacha",
@@ -396,17 +408,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "protobuf"
 version = "2.14.0"
@@ -471,17 +483,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -589,17 +601,17 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.162"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71b2f6e1ab5c2b98c05f0f35b236b22e8df7ead6ffbf51d7808da7f8817e7ab6"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
 version = "0.11.9"
@@ -607,21 +619,21 @@
 checksum = "416bda436f9aab92e02c8e10d49a15ddd339cea90b6e340fe51ed97abb548294"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.162"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2a0814352fd64b58489904a44ea8d90cb1a91dcb6b4f5ebabc32c8318e93cb6"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -646,17 +658,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -678,15 +690,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
```

