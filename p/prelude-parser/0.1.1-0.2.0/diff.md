# Comparing `tmp/prelude_parser-0.1.1.tar.gz` & `tmp/prelude_parser-0.2.0.tar.gz`

## Comparing `prelude_parser-0.1.1.tar` & `prelude_parser-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,31 @@
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 prelude_parser-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123      539 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.github/release-draft-template.yml
--rw-r--r--   0     1001      123     2599 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.github/workflows/pypi_publish.yml
--rw-r--r--   0     1001      123      309 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.github/workflows/release-drafter.yml
--rw-r--r--   0     1001      123     1884 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.github/workflows/testing.yml
--rw-r--r--   0     1001      123      686 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.gitignore
--rw-r--r--   0     1001      123      640 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     7942 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1080 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/LICENSE
--rw-r--r--   0     1001      123     1162 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/README.md
--rw-r--r--   0     1001      123       81 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/prelude_parser/__init__.py
--rw-r--r--   0     1001      123      293 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/prelude_parser/_prelude_parser.pyi
--rw-r--r--   0     1001      123     1966 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/prelude_parser/parser.py
--rw-r--r--   0     1001      123        0 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/prelude_parser/py.typed
--rw-r--r--   0     1001      123     1609 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123       89 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/requirements-dev.txt
--rw-r--r--   0     1001      123     3469 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/__init__.py
--rw-r--r--   0     1001      123     1304 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/assets/test1.xml
--rw-r--r--   0     1001      123     1839 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/assets/test2.xml
--rw-r--r--   0     1001      123     2122 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/assets/test3.xml
--rw-r--r--   0     1001      123      312 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/conftest.py
--rw-r--r--   0     1001      123     2474 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/test_parser.py
--rw-r--r--   0     1001      123     8093 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     2011 1970-01-01 00:00:00.000000 prelude_parser-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 prelude_parser-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123      439 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.github/dependabot.yml
+-rw-r--r--   0     1001      123      539 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.github/release-draft-template.yml
+-rw-r--r--   0     1001      123     2599 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.github/workflows/pypi_publish.yml
+-rw-r--r--   0     1001      123      309 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0     1001      123     1884 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.github/workflows/testing.yml
+-rw-r--r--   0     1001      123      686 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.gitignore
+-rw-r--r--   0     1001      123      640 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     7889 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1080 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/LICENSE
+-rw-r--r--   0     1001      123     1499 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/README.md
+-rw-r--r--   0     1001      123      585 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/justfile
+-rw-r--r--   0     1001      123      115 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/__init__.py
+-rw-r--r--   0     1001      123      399 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/_prelude_parser.pyi
+-rw-r--r--   0     1001      123      911 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/pandas.py
+-rw-r--r--   0     1001      123     2325 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/parser.py
+-rw-r--r--   0     1001      123      901 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/polars.py
+-rw-r--r--   0     1001      123        0 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/prelude_parser/py.typed
+-rw-r--r--   0     1001      123     1845 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      147 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/requirements-dev.txt
+-rw-r--r--   0     1001      123     6082 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/__init__.py
+-rw-r--r--   0     1001      123     1304 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/assets/test1.xml
+-rw-r--r--   0     1001      123     1839 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/assets/test2.xml
+-rw-r--r--   0     1001      123     2122 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/assets/test3.xml
+-rw-r--r--   0     1001      123      312 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/conftest.py
+-rw-r--r--   0     1001      123      942 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/test_pandas.py
+-rw-r--r--   0     1001      123     8042 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/test_parser.py
+-rw-r--r--   0     1001      123     1004 2023-05-19 16:41:18.000000 prelude_parser-0.2.0/tests/test_polars.py
+-rw-r--r--   0     1001      123     8093 2023-05-19 16:42:55.000000 prelude_parser-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     2710 1970-01-01 00:00:00.000000 prelude_parser-0.2.0/PKG-INFO
```

### Comparing `prelude_parser-0.1.1/.github/release-draft-template.yml` & `prelude_parser-0.2.0/.github/release-draft-template.yml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.1/.github/workflows/pypi_publish.yml` & `prelude_parser-0.2.0/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.1/.github/workflows/testing.yml` & `prelude_parser-0.2.0/.github/workflows/testing.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     - uses: actions-rs/toolchain@v1
       with:
         profile: minimal
         toolchain: stable
         override: true
         components: clippy
     - name: Cache dependencies
-      uses: Swatinem/rust-cache@v2.2.1
+      uses: Swatinem/rust-cache@v2.3.0
     - name: Run cargo clippy
       uses: actions-rs/cargo@v1
       with:
         command: clippy
         args: --all-targets -- --deny warnings
   fmt:
     name: Rustfmt
@@ -35,15 +35,15 @@
     - uses: actions-rs/toolchain@v1
       with:
         profile: minimal
         toolchain: stable
         override: true
         components: rustfmt
     - name: Cache dependencies
-      uses: Swatinem/rust-cache@v2.2.1
+      uses: Swatinem/rust-cache@v2.3.0
     - name: Run cargo fmt
       run: cargo fmt --all -- --check
   test:
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
```

### Comparing `prelude_parser-0.1.1/.gitignore` & `prelude_parser-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.1/.pre-commit-config.yaml` & `prelude_parser-0.2.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
     - id: black
       language_version: python3
       args: [--line-length=100]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
     - id: mypy
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.267
     hooks:
     - id: ruff
       args: [--fix, --exit-non-zero-on-fix]
```

### Comparing `prelude_parser-0.1.1/CONTRIBUTING.md` & `prelude_parser-0.2.0/CONTRIBUTING.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,26 @@
 
 Please include:
 
 1. A short, self-contained Python snippet reproducing the problem. You can format the code by using
 [GitHub markdown](https://docs.github.com/en/free-pro-team@latest/github/writing-on-github). For example:
 
     ```py
-    from prelude_parser import parse_flat_file
+    from prelude_parser import parse_to_classes
 
-    data = parse_flat_file("my_file.xml")
+    data = parse_to_classes("my_file.xml")
     ```
 
 2. Explain what is currently happening and what you expect instead.
 
 ## Working on the code
 
+In order to work on this project you will need to have [Rust](https://www.rust-lang.org/) and
+[just](https://github.com/casey/just) in addition to Python.
+
 ### Fork the project
 
 In order to work on the project you will need your own fork. To do this click the "Fork" button on
 this project.
 
 Once the project is forked clone it to your local machine:
 
@@ -35,37 +38,32 @@
 git clone git@github.com:your-user-name/prelude-parser
 cd prelude-parser
 git remote add upstream git@github.com:pbs-data-solutions/prelude-parser
 ```
 
 This creates the directory prelude-parser and connects your repository to the upstream (main project) repository.
 
-### Working with the code
-
-In order to work on this project you will need to have [Rust](https://www.rust-lang.org/) in
-addition to Python.
-
-Once Rust is installed you should create a vitural environment and activate it.
+Next create a vitural environment and activate it.
 
 ```sh
 python -m venv .venv
 
 . .venv/bin/activate
 ```
 
-Then install the dev requirements
+Then install the dev requirements. This will also build the Rust module in dev mode and install it.
 
 ```sh
-pip install -r requirements-dev.txt
+just install
 ```
 
-Now the Rust module can be built in dev mode.
+When changes are made to the Rust code, build and install the new module with:
 
 ```sh
-maturin develop
+just develop
 ```
 
 ### Creating a branch
 
 You want your main branch to reflect only production-ready code, so create a feature branch for
 making your changes. For example:
 
@@ -91,28 +89,15 @@
 and [mypy](https://mypy.readthedocs.io/en/stable/), [clippy](https://doc.rust-lang.org/clippy/), and
 [rustfmt](https://rust-lang.github.io/rustfmt/?version=v1.5.1&search=) to ensure consistant code
 formmating.
 
 You can run linting on your code at any time with:
 
 ```sh
-# Run ruff
-ruff check .
-
-# Run black
-black prelude_parser tests
-
-# Run mypy
-mypy .
-
-# clippy
-cargo clippy
-
-# rustfmt
-cargo fmt
+just lint
 ```
 
 It is also suggested that you setup [pre-commit](https://pre-commit.com/) in order to run linting
 when you commit changes to you branch. To setup pre-commit for this project run:
 
 ```sh
 pre-commit install
@@ -161,15 +146,15 @@
 additions/changes you make to the code have tests to go along with them. Code coverage should not
 drop blow it's current level with any pull requests you make, if it does the pull request will not
 be accepted. You can view the current coverage level in the codecov badge on the
 [main github page](https://github.com/pbs-data-solutions/prelude-parser). You can run tests and see
 the code coverage by running:
 
 ```sh
-pytest
+just test
 ```
 
 In additon to mainting the coverage percentage please ensure that all tests are passing before
 submitting a pull request.
 
 ## Committing your code
```

### Comparing `prelude_parser-0.1.1/LICENSE` & `prelude_parser-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.1/pyproject.toml` & `prelude_parser-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=0.15"]
 build-backend = "maturin"
 
 [project]
 name = "prelude-parser"
 requires-python = ">=3.8"
+description = "Parses XML files exported from Prelude EDC into formats usable by Python."
 authors = [{name = "Paul Sanders", email = "paul@pbsdatasolutions.com"}]
-keywords = ["prelude-edc", "xml", "parser"]
+keywords = ["parser", "prelude-edc", "xml", "pandas", "polars"]
 classifiers = [
   "Programming Language :: Rust",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
@@ -20,14 +21,19 @@
 license = {file = "LICENSE"}
 readme = "README.md"
 repository = "https://github.com/pbs-data-solutions/prelude-parser"
 homepage = "https://github.com/pbs-data-solutions/prelude-parser"
 documentation = "https://github.com/pbs-data-solutions/prelude-parser"
 dependencies = ["camel-converter>=3.0.0"]
 
+[project.optional-dependencies]
+pandas = ["pandas>=2.0.1"]
+polars = ["polars>=0.17.14"]
+all = ["pandas>=2.0.1", "polars>=0.17.14"]
+
 [tool.maturin]
 module-name = "prelude_parser._prelude_parser"
 binding = "pyo3"
 features = ["pyo3/extension-module"]
 
 [tool.black]
 line-length = 100
```

### Comparing `prelude_parser-0.1.1/src/lib.rs` & `prelude_parser-0.2.0/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -8,39 +8,63 @@
 use pyo3::types::{IntoPyDict, PyDict};
 use roxmltree::Document;
 
 create_exception!(_prelude_parser, FileNotFoundError, PyException);
 create_exception!(_prelude_parser, InvalidFileTypeError, PyException);
 create_exception!(_prelude_parser, ParsingError, PyException);
 
+fn to_snake(camel_string: &str) -> String {
+    let snake_string: String = camel_string
+        .chars()
+        .map(|c| {
+            if c.is_uppercase() {
+                format!("_{}", c)
+            } else {
+                c.to_string()
+            }
+        })
+        .collect();
+
+    // There is some weirdness in the Prelude XML files that can result in names like
+    // `i_communications_Details`. Because of this we can end up with values like
+    // `i_communications__details` so we need to fix double `__` values when we return the string.
+
+    snake_string
+        .trim_start_matches('_')
+        .to_lowercase()
+        .replace("__", "_")
+}
+
 fn parse_xml<'py>(py: Python<'py>, xml_file: &PathBuf) -> PyResult<&'py PyDict> {
     let reader = read_to_string(xml_file);
 
     match reader {
         Ok(r) => match Document::parse(&r) {
             Ok(doc) => {
-                let mut data: HashMap<&str, Vec<&PyDict>> = HashMap::new();
+                let mut data: HashMap<String, Vec<&PyDict>> = HashMap::new();
                 let tree = doc.root_element();
                 for form in tree.children() {
-                    let form_name = form.tag_name().name();
+                    let form_name = to_snake(form.tag_name().name());
                     if !form_name.is_empty() {
-                        if let Some(d) = data.get_mut(form_name) {
-                            let mut form_data: HashMap<&str, Option<&str>> = HashMap::new();
+                        if let Some(d) = data.get_mut(&form_name) {
+                            let mut form_data: HashMap<String, Option<&str>> = HashMap::new();
                             for child in form.children() {
                                 if child.is_element() && child.tag_name().name() != "" {
-                                    form_data.insert(child.tag_name().name(), child.text());
+                                    let key = to_snake(child.tag_name().name());
+                                    form_data.insert(key, child.text());
                                 }
                             }
                             d.push(form_data.into_py_dict(py));
                         } else {
                             let mut items: Vec<&PyDict> = Vec::new();
-                            let mut form_data: HashMap<&str, Option<&str>> = HashMap::new();
+                            let mut form_data: HashMap<String, Option<&str>> = HashMap::new();
                             for child in form.children() {
                                 if child.is_element() && child.tag_name().name() != "" {
-                                    form_data.insert(child.tag_name().name(), child.text());
+                                    let key = to_snake(child.tag_name().name());
+                                    form_data.insert(key, child.text());
                                 }
                             }
                             items.push(form_data.into_py_dict(py));
                             data.insert(form_name, items);
                         }
                     }
                 }
@@ -54,14 +78,49 @@
         Err(e) => Err(ParsingError::new_err(format!(
             "Error parsing xml file: {:?}",
             e
         ))),
     }
 }
 
+fn parse_xml_pandas<'py>(py: Python<'py>, xml_file: &PathBuf) -> PyResult<&'py PyDict> {
+    let reader = read_to_string(xml_file);
+
+    match reader {
+        Ok(r) => match Document::parse(&r) {
+            Ok(doc) => {
+                let mut data: HashMap<&str, Vec<Option<&str>>> = HashMap::new();
+                let tree = doc.root_element();
+
+                for form in tree.children() {
+                    for child in form.children() {
+                        if child.is_element() && child.tag_name().name() != "" {
+                            let column = child.tag_name().name();
+                            if let Some(d) = data.get_mut(column) {
+                                d.push(child.text());
+                            } else {
+                                data.insert(column, vec![child.text()]);
+                            }
+                        }
+                    }
+                }
+                return Ok(data.into_py_dict(py));
+            }
+            Err(e) => Err(ParsingError::new_err(format!(
+                "Error parsing xml file: {:?}",
+                e
+            ))),
+        },
+        Err(e) => Err(ParsingError::new_err(format!(
+            "Error parsing xml file: {:?}",
+            e
+        ))),
+    }
+}
+
 fn validate_file(xml_file: &PathBuf) -> PyResult<()> {
     if !xml_file.is_file() {
         return Err(FileNotFoundError::new_err(format!(
             "File not found: {:?}",
             xml_file
         )));
     } else if xml_file.extension().unwrap() != "xml" {
@@ -71,25 +130,49 @@
         )));
     }
 
     Ok(())
 }
 
 #[pyfunction]
-fn _parse_flat_file(py: Python, xml_file: PathBuf) -> PyResult<&PyDict> {
+fn _parse_flat_file_to_dict(py: Python, xml_file: PathBuf) -> PyResult<&PyDict> {
     validate_file(&xml_file)?;
     let data = parse_xml(py, &xml_file)?;
 
     Ok(data)
 }
 
+#[pyfunction]
+fn _parse_flat_file_to_pandas_dict(py: Python, xml_file: PathBuf) -> PyResult<&PyDict> {
+    validate_file(&xml_file)?;
+    let data = parse_xml_pandas(py, &xml_file)?;
+
+    Ok(data)
+}
+
 #[pymodule]
 fn _prelude_parser(py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_function(wrap_pyfunction!(_parse_flat_file, m)?)?;
+    m.add_function(wrap_pyfunction!(_parse_flat_file_to_dict, m)?)?;
+    m.add_function(wrap_pyfunction!(_parse_flat_file_to_pandas_dict, m)?)?;
     m.add("FileNotFoundError", py.get_type::<FileNotFoundError>())?;
     m.add(
         "InvalidFileTypeError",
         py.get_type::<InvalidFileTypeError>(),
     )?;
     m.add("ParsingError", py.get_type::<ParsingError>())?;
     Ok(())
 }
+
+#[cfg(test)]
+mod tests {
+    use std::assert_eq;
+
+    use super::*;
+
+    #[test]
+    fn test_to_snake() {
+        assert_eq!(
+            to_snake("i_communications_Details"),
+            String::from("i_communications_details")
+        );
+    }
+}
```

### Comparing `prelude_parser-0.1.1/tests/assets/test1.xml` & `prelude_parser-0.2.0/tests/assets/test1.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.1/tests/assets/test2.xml` & `prelude_parser-0.2.0/tests/assets/test2.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.1/tests/assets/test3.xml` & `prelude_parser-0.2.0/tests/assets/test3.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.1/Cargo.lock` & `prelude_parser-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "prelude-parser"
-version = "0.1.1"
+version = "0.2.0"
 dependencies = [
  "pyo3",
  "roxmltree",
 ]
 
 [[package]]
 name = "proc-macro2"
```

### Comparing `prelude_parser-0.1.1/PKG-INFO` & `prelude_parser-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-Metadata-Version: 2.1
-Name: prelude-parser
-Version: 0.1.1
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Typing :: Typed
-Requires-Dist: camel-converter>=3.0.0
-License-File: LICENSE
-Keywords: prelude-edc,xml,parser
-Home-Page: https://github.com/pbs-data-solutions/prelude-parser
-Author-email: Paul Sanders <paul@pbsdatasolutions.com>
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Source Code, https://github.com/pbs-data-solutions/prelude-parser
-
 # Prelude Parser
 
 [![Tests Status](https://github.com/pbs-data-solutions/prelude-parser/workflows/Testing/badge.svg?branch=main&event=push)](https://github.com/pbs-data-solutions/prelude-parser/actions?query=workflow%3ATesting+branch%3Amain+event%3Apush)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pbs-data-solutions/prelude-parser/main.svg)](https://results.pre-commit.ci/latest/github/pbs-data-solutions/prelude-parser/main)
 [![Coverage](https://codecov.io/github/pbs-data-solutions/prelude-parser/coverage.svg?branch=main)](https://codecov.io/gh/pbs-data-solutions/prelude-parser)
 [![PyPI version](https://badge.fury.io/py/prelude-parser.svg)](https://badge.fury.io/py/prelude-parser)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/prelude-parser?color=5cc141)](https://github.com/pbs-data-solutions/prelude-parser)
 
-Parses XML files exported from [Prelude EDC](https://preludeedc.com/) into Python classes.
+Parses XML files exported from [Prelude EDC](https://preludeedc.com/) into formats Python can use.
 
 ## Installation
 
 ```sh
 pip install prelude-parser
 ```
 
+Optionally the `pandas` extra can be installed to parse to a Pandas `DataFrame`
+
+```sh
+pip install prelude-parser[pandas]
+```
+
+Optionally the `polars` extra can be installed to parse to a Polars `DataFrame`
+
+```sh
+pip install prelude-parser[polars]
+```
+
+All extras can be install with
+
+```sh
+pip install prelude-parser[all]
+```
+
 ## Contributing
 
 Contributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)
-
```

