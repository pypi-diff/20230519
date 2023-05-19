# Comparing `tmp/logrouter-0.0.1.tar.gz` & `tmp/logrouter-0.0.2.tar.gz`

## Comparing `logrouter-0.0.1.tar` & `logrouter-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,20 @@
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 logrouter-0.0.1/examples/log_by_thread/log_by_thread.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 logrouter-0.0.1/examples/log_by_thread/logging_conf.yaml
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 logrouter-0.0.1/examples/simple_usage/logging_conf.yaml
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 logrouter-0.0.1/examples/simple_usage/simple_usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logrouter-0.0.1/logrouter/__init__.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 logrouter-0.0.1/logrouter/default_logging_conf.yaml
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 logrouter-0.0.1/logrouter/logrouter.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 logrouter-0.0.1/logrouter/setup_logging.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 logrouter-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 logrouter-0.0.1/LICENSE
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 logrouter-0.0.1/README.md
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 logrouter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 logrouter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 logrouter-0.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 logrouter-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 logrouter-0.0.2/MAINTAINERS.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 logrouter-0.0.2/.github/dco.yml
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 logrouter-0.0.2/examples/handlers_by_discriminant_value/custom_handlers.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 logrouter-0.0.2/examples/handlers_by_discriminant_value/handlers_by_discriminant_value.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 logrouter-0.0.2/examples/handlers_by_discriminant_value/logging_conf.yaml
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 logrouter-0.0.2/examples/log_by_thread/log_by_thread.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 logrouter-0.0.2/examples/log_by_thread/logging_conf.yaml
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 logrouter-0.0.2/examples/simple_usage/logging_conf.yaml
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 logrouter-0.0.2/examples/simple_usage/simple_usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logrouter-0.0.2/logrouter/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 logrouter-0.0.2/logrouter/default_logging_conf.yaml
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 logrouter-0.0.2/logrouter/logrouter.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 logrouter-0.0.2/logrouter/setup_logging.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 logrouter-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 logrouter-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 logrouter-0.0.2/README.md
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 logrouter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 logrouter-0.0.2/PKG-INFO
```

### Comparing `logrouter-0.0.1/examples/log_by_thread/log_by_thread.py` & `logrouter-0.0.2/examples/log_by_thread/log_by_thread.py`

 * *Files identical despite different names*

### Comparing `logrouter-0.0.1/examples/log_by_thread/logging_conf.yaml` & `logrouter-0.0.2/examples/log_by_thread/logging_conf.yaml`

 * *Files identical despite different names*

### Comparing `logrouter-0.0.1/examples/simple_usage/simple_usage.py` & `logrouter-0.0.2/examples/simple_usage/simple_usage.py`

 * *Files identical despite different names*

### Comparing `logrouter-0.0.1/logrouter/default_logging_conf.yaml` & `logrouter-0.0.2/logrouter/default_logging_conf.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,11 +13,11 @@
   logrouter:
     class: logrouter.logrouter.LogRouter
     level: DEBUG
     formatter: simple
     discriminator: discriminator
     # filters: [discriminator-filter]
     single_handler_class: logrouter.logrouter.DefaultHandler
-
+    
 root:
   level: DEBUG
   handlers: [console, logrouter]
```

### Comparing `logrouter-0.0.1/logrouter/setup_logging.py` & `logrouter-0.0.2/logrouter/setup_logging.py`

 * *Files identical despite different names*

### Comparing `logrouter-0.0.1/LICENSE` & `logrouter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logrouter-0.0.1/pyproject.toml` & `logrouter-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logrouter"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Martín Santillán Cooper", email="msantillancooper@ibm.com" },
 ]
 description = "A package that allows logs to be routed to different handlers based on a discriminant"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["pyyaml"]
```

### Comparing `logrouter-0.0.1/PKG-INFO` & `logrouter-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,23 @@
-Metadata-Version: 2.1
-Name: logrouter
-Version: 0.0.1
-Summary: A package that allows logs to be routed to different handlers based on a discriminant
-Author-email: Martín Santillán Cooper <msantillancooper@ibm.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: pyyaml
-Description-Content-Type: text/markdown
-
 # python-log-router
 
-A package that allows logs to be routed to different handlers based on a discriminant.
+A package that allows logs to be routed to different log handlers based on a discriminant. Each unique value of the discriminant is managed by a distinct handler.
 
 ## Installation
 
 `pip install logrouter`
 
 ## Usage
 
-Call `logrouter.setup_logging()` to setup the logging configuration by providing the configuration yaml absolute file path. You can also set the configuration file using an environment variable. Specify the `env_path` parameter.
+Call `logrouter.setup_logging()` to setup the logging configuration by providing the configuration yaml absolute file path. You can also set the configuration path using an environment variable. Specify the name of the env variable by setting the `env_path` parameter.
+
+For an example of a configuration file, refer to the [default configuration file](https://github.com/IBM/python-log-router/blob/main/logrouter/default_logging_conf.yaml). You can specify the log handler to be used by replacing `handlers.single_handler_class` with the name of the handler. The default one is `logrouter.logrouter.DefaultHandler`, which inherits from `logging.FileHandler`.
+
+The default logging configuration will route all the logs based on the `discriminator` field of the LogRecord object. To use the default configuration, call `logrouter.setup_logging(use_default_config=True)`.
 
-For an example of a configuration file, refer to the [default configuration file](https://github.com/IBM/python-log-router/blob/main/logrouter/default_logging_conf.yaml). You can specify the handler by replacing `handlers.single_handler_class` with the name of your handler. Default is `logrouter.logrouter.DefaultHandler`.
+## Examples
 
-The default logging configuration will route the logs based on the `discriminator` field of the LogRecord object.
-To use the default configuration, call `logrouter.setup_logging(use_default_config=True)`.
+Run and look at the code and logs produced of the examples located at [`/examples`](https://github.com/IBM/python-log-router/blob/main/examples/) to experience what you can achieve with `logrouter`.
 
+## Using different types of handlers
 
+A new instance of `single_handler_class` handler class is used for each discriminator unique value. This instance receives the log level and the discriminator value when created. If you want to use a differnet handler class for some discriminant values, specify them in `handlers.handlers_dict` in the logging configuration file. See [this example](https://github.com/IBM/python-log-router/tree/main/examples/handlers_by_discriminant_value).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

