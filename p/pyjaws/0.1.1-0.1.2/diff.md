# Comparing `tmp/pyjaws-0.1.1.tar.gz` & `tmp/pyjaws-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjaws-0.1.1.tar", last modified: Tue May 16 11:10:34 2023, max compression
+gzip compressed data, was "pyjaws-0.1.2.tar", last modified: Fri May 19 08:09:33 2023, max compression
```

## Comparing `pyjaws-0.1.1.tar` & `pyjaws-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.388727 pyjaws-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-16 11:10:34.388727 pyjaws-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.384726 pyjaws-0.1.1/pyjaws/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.384726 pyjaws-0.1.1/pyjaws/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.384726 pyjaws-0.1.1/pyjaws/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.384726 pyjaws-0.1.1/pyjaws/api/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/templates/macros/cluster.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/templates/macros/task.j2
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/api/templates/workflow.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.388727 pyjaws-0.1.1/pyjaws/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyjaws/client/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:10:34.384726 pyjaws-0.1.1/pyjaws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 11:10:34.000000 pyjaws-0.1.1/pyjaws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-16 11:10:19.000000 pyjaws-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 11:10:34.388727 pyjaws-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-16 11:10:19.000000 pyjaws-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.412507 pyjaws-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-19 08:09:33.412507 pyjaws-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.408507 pyjaws-0.1.2/pyjaws/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.412507 pyjaws-0.1.2/pyjaws/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.412507 pyjaws-0.1.2/pyjaws/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.412507 pyjaws-0.1.2/pyjaws/api/templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/templates/macros/cluster.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/templates/macros/task.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/templates/workflow.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.412507 pyjaws-0.1.2/pyjaws/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/client/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.408507 pyjaws-0.1.2/pyjaws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 08:09:33.412507 pyjaws-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-19 08:09:24.000000 pyjaws-0.1.2/setup.py
```

### Comparing `pyjaws-0.1.1/PKG-INFO` & `pyjaws-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyjaws
-Version: 0.1.1
+Version: 0.1.2
 Author: Rafael Pierre
 Description-Content-Type: text/markdown
 
 # PyJaws: A Pythonic Way to Define Databricks Jobs and Workflows
 
 <p align="center">
         <img src="https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/pyjaws.png" class="align-center" />
     </a>
 </p>
 
 <hr />
 
-[![pypi](https://img.shields.io/badge/pypi-0.1.0-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
+[![pypi](https://img.shields.io/badge/pypi-0.1.1-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
 
 <hr />
 
 * **PyJaws** enables declaring [Databricks Jobs and Workflows](https://docs.databricks.com/workflows/index.html) as Python code, allowing for:
   * Code Linting
   * Formatting
   * Parameter Validation
```

### Comparing `pyjaws-0.1.1/pyjaws/api/base.py` & `pyjaws-0.1.2/pyjaws/api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,20 @@
             storing cluster logs.\n
         """
         super().__init__(**kwargs)
 
     def __str__(self):
         return self.job_cluster_key
 
+    def __enter__(self) -> Cluster:
+        return self
+
+    def __exit__(self, *args):
+        pass
+
     @property
     def cluster_log_conf_str(self) -> str:
         return json.dumps(self.cluster_log_conf)
 
 
 class BaseTask(BaseModel):
     """
```

### Comparing `pyjaws-0.1.1/pyjaws/api/jobs.py` & `pyjaws-0.1.2/pyjaws/api/jobs.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.1/pyjaws/api/tasks.py` & `pyjaws-0.1.2/pyjaws/api/tasks.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.1/pyjaws/api/templates/macros/cluster.j2` & `pyjaws-0.1.2/pyjaws/api/templates/macros/cluster.j2`

 * *Files 1% similar despite different names*

```diff
@@ -20,11 +20,11 @@
         {% else %}
         "runtime_engine": "STANDARD",
         {% endif %}
         {% if cluster_specs.cluster_log_conf %}
         "cluster_log_conf": {{ cluster_specs.cluster_log_conf_str }},
         {% endif %}
     }
-}
+},
 {% endfilter %}
 {% endfor %}
 {% endmacro %}
```

### Comparing `pyjaws-0.1.1/pyjaws/api/templates/macros/task.j2` & `pyjaws-0.1.2/pyjaws/api/templates/macros/task.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.1/pyjaws/api/templates/workflow.j2` & `pyjaws-0.1.2/pyjaws/api/templates/workflow.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.1/pyjaws/client/entrypoint.py` & `pyjaws-0.1.2/pyjaws/client/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.1/pyjaws.egg-info/PKG-INFO` & `pyjaws-0.1.2/pyjaws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyjaws
-Version: 0.1.1
+Version: 0.1.2
 Author: Rafael Pierre
 Description-Content-Type: text/markdown
 
 # PyJaws: A Pythonic Way to Define Databricks Jobs and Workflows
 
 <p align="center">
         <img src="https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/pyjaws.png" class="align-center" />
     </a>
 </p>
 
 <hr />
 
-[![pypi](https://img.shields.io/badge/pypi-0.1.0-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
+[![pypi](https://img.shields.io/badge/pypi-0.1.1-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
 
 <hr />
 
 * **PyJaws** enables declaring [Databricks Jobs and Workflows](https://docs.databricks.com/workflows/index.html) as Python code, allowing for:
   * Code Linting
   * Formatting
   * Parameter Validation
```

### Comparing `pyjaws-0.1.1/pyproject.toml` & `pyjaws-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.1/setup.py` & `pyjaws-0.1.2/setup.py`

 * *Files identical despite different names*

