# Comparing `tmp/apache-airflow-providers-cncf-kubernetes-6.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-cncf-kubernetes-7.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-cncf-kubernetes-6.2.0rc1.tar", last modified: Tue May 16 15:53:29 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-cncf-kubernetes-7.0.0rc2.tar", last modified: Fri May 19 17:52:06 2023, max compression
```

## Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1.tar` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1156 2023-05-16 15:53:28.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    34370 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    32816 2023-05-16 15:53:28.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/
--rw-r--r--   0 root         (0) root         (0)     1398 2023-05-16 15:39:21.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6178 2023-05-12 08:38:07.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     4383 2023-05-16 15:53:28.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24886 2023-05-16 07:40:59.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-05-03 19:47:07.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    40094 2023-05-16 07:40:59.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0 root         (0) root         (0)     4860 2023-03-15 08:58:48.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0 root         (0) root         (0)     3343 2023-03-27 08:32:49.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-05-03 19:47:07.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    10367 2023-04-24 21:04:25.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/
--rw-r--r--   0 root         (0) root         (0)      863 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23045 2023-05-16 07:40:59.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)    34370 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1782 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1976 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-05-16 15:53:28.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-05-19 17:52:04.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    34812 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    33258 2023-05-19 17:52:04.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-05-19 17:37:00.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/backcompat/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-05-19 11:18:18.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2023-05-12 08:38:07.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     4383 2023-05-19 17:52:04.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23078 2023-05-19 11:18:18.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-05-03 19:47:07.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    38841 2023-05-19 11:18:18.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2023-03-15 08:58:48.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3343 2023-03-27 08:32:49.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-05-03 19:47:07.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    10367 2023-04-24 21:04:25.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/pod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22634 2023-05-19 11:18:18.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    34812 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-05-19 17:52:04.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/setup.py
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/LICENSE` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/MANIFEST.in` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 6.2.0rc1
+Version: 7.0.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``6.2.0rc1``
+Release: ``7.0.0rc2``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -112,21 +112,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-6.2.0
+
+
+7.0.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. note::
+  Return None when namespace is not defined in the Kubernetes connection
+
+* ``Remove deprecated features from KubernetesHook (#31402)``
+
 Features
 ~~~~~~~~
 
 .. note::
   If ``kubernetes_default`` connection is not defined, then KubernetesHook / KubernetesPodOperator will behave as though given ``conn_id=None``.
   This should make it easier to mitigate breaking change introduced in 6.0.0
 
@@ -150,14 +160,18 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Upgrade ruff to 0.0.262 (#30809)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
    * ``Fix pod describing on system test failure (#31191)``
+   * ``Docstring improvements (#31375)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
 
 6.1.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/README.rst` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``6.2.0rc1``
+Release: ``7.0.0rc2``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,21 +79,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-6.2.0
+
+
+7.0.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. note::
+  Return None when namespace is not defined in the Kubernetes connection
+
+* ``Remove deprecated features from KubernetesHook (#31402)``
+
 Features
 ~~~~~~~~
 
 .. note::
   If ``kubernetes_default`` connection is not defined, then KubernetesHook / KubernetesPodOperator will behave as though given ``conn_id=None``.
   This should make it easier to mitigate breaking change introduced in 6.0.0
 
@@ -117,14 +127,18 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Upgrade ruff to 0.0.262 (#30809)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
    * ``Fix pod describing on system test failure (#31191)``
+   * ``Docstring improvements (#31375)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
 
 6.1.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,91 +39,77 @@
         api_client = ApiClient()
         return api_client._ApiClient__deserialize_model(obj, new_class)
     else:
         raise AirflowException(f"Expected dict or {new_class}, got {type(obj)}")
 
 
 def convert_volume(volume) -> k8s.V1Volume:
-    """
-    Converts an airflow Volume object into a k8s.V1Volume
+    """Converts an airflow Volume object into a k8s.V1Volume
 
     :param volume:
-    :return: k8s.V1Volume
     """
     return _convert_kube_model_object(volume, k8s.V1Volume)
 
 
 def convert_volume_mount(volume_mount) -> k8s.V1VolumeMount:
-    """
-    Converts an airflow VolumeMount object into a k8s.V1VolumeMount
+    """Converts an airflow VolumeMount object into a k8s.V1VolumeMount
 
     :param volume_mount:
-    :return: k8s.V1VolumeMount
     """
     return _convert_kube_model_object(volume_mount, k8s.V1VolumeMount)
 
 
 def convert_port(port) -> k8s.V1ContainerPort:
-    """
-    Converts an airflow Port object into a k8s.V1ContainerPort
+    """Converts an airflow Port object into a k8s.V1ContainerPort
 
     :param port:
-    :return: k8s.V1ContainerPort
     """
     return _convert_kube_model_object(port, k8s.V1ContainerPort)
 
 
 def convert_env_vars(env_vars) -> list[k8s.V1EnvVar]:
-    """
-    Converts a dictionary into a list of env_vars
+    """Converts a dictionary into a list of env_vars
 
     :param env_vars:
-    :return:
     """
     if isinstance(env_vars, dict):
         res = []
         for k, v in env_vars.items():
             res.append(k8s.V1EnvVar(name=k, value=v))
         return res
     elif isinstance(env_vars, list):
         return env_vars
     else:
         raise AirflowException(f"Expected dict or list, got {type(env_vars)}")
 
 
 def convert_pod_runtime_info_env(pod_runtime_info_envs) -> k8s.V1EnvVar:
-    """
-    Converts a PodRuntimeInfoEnv into an k8s.V1EnvVar
+    """Converts a PodRuntimeInfoEnv into an k8s.V1EnvVar
 
     :param pod_runtime_info_envs:
-    :return:
     """
     return _convert_kube_model_object(pod_runtime_info_envs, k8s.V1EnvVar)
 
 
 def convert_image_pull_secrets(image_pull_secrets) -> list[k8s.V1LocalObjectReference]:
-    """
-    Converts a PodRuntimeInfoEnv into an k8s.V1EnvVar
+    """Converts a PodRuntimeInfoEnv into an k8s.V1EnvVar
 
     :param image_pull_secrets:
-    :return:
     """
     if isinstance(image_pull_secrets, str):
         secrets = image_pull_secrets.split(",")
         return [k8s.V1LocalObjectReference(name=secret) for secret in secrets]
     else:
         return image_pull_secrets
 
 
 def convert_configmap(configmaps) -> k8s.V1EnvFromSource:
-    """
-    Converts a str into an k8s.V1EnvFromSource
+    """Converts a str into an k8s.V1EnvFromSource
 
     :param configmaps:
-    :return:
     """
     return k8s.V1EnvFromSource(config_map_ref=k8s.V1ConfigMapEnvSource(name=configmaps))
 
 
 def convert_affinity(affinity) -> k8s.V1Affinity:
     """Converts a dict into an k8s.V1Affinity"""
     return _convert_from_dict(affinity, k8s.V1Affinity)
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-cncf-kubernetes",
         "name": "Kubernetes",
         "description": "`Kubernetes <https://kubernetes.io/>`__\n",
         "suspended": False,
         "versions": [
-            "6.2.0",
+            "7.0.0",
             "6.1.0",
             "6.0.0",
             "5.3.0",
             "5.2.2",
             "5.2.1",
             "5.2.0",
             "5.1.1",
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,26 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import contextlib
-import json
 import tempfile
-import warnings
 from typing import TYPE_CHECKING, Any, Generator
 
 from asgiref.sync import sync_to_async
 from kubernetes import client, config, watch
 from kubernetes.client.models import V1Pod
 from kubernetes.config import ConfigException
 from kubernetes_asyncio import client as async_client, config as async_config
 from urllib3.exceptions import HTTPError
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException, AirflowNotFoundException, AirflowProviderDeprecationWarning
+from airflow.exceptions import AirflowException, AirflowNotFoundException
 from airflow.hooks.base import BaseHook
 from airflow.kubernetes.kube_client import _disable_verify_ssl, _enable_tcp_keepalive
 from airflow.models import Connection
 from airflow.providers.cncf.kubernetes.utils.pod_manager import PodOperatorHookProtocol
 from airflow.utils import yaml
 
 LOADING_KUBE_CONFIG_FILE_RESOURCE = "Loading Kubernetes configuration file kube_config from {}..."
@@ -97,20 +95,14 @@
             "kube_config": StringField(
                 lazy_gettext("Kube config (JSON format)"), widget=BS3TextFieldWidget()
             ),
             "namespace": StringField(lazy_gettext("Namespace"), widget=BS3TextFieldWidget()),
             "cluster_context": StringField(lazy_gettext("Cluster context"), widget=BS3TextFieldWidget()),
             "disable_verify_ssl": BooleanField(lazy_gettext("Disable SSL")),
             "disable_tcp_keepalive": BooleanField(lazy_gettext("Disable TCP keepalive")),
-            "xcom_sidecar_container_image": StringField(
-                lazy_gettext("XCom sidecar image"), widget=BS3TextFieldWidget()
-            ),
-            "xcom_sidecar_container_resources": StringField(
-                lazy_gettext("XCom sidecar resources (JSON format)"), widget=BS3TextFieldWidget()
-            ),
         }
 
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
         """Returns custom field behaviour"""
         return {
             "hidden_fields": ["host", "schema", "login", "password", "port", "extra"],
@@ -299,15 +291,15 @@
             body_dict = _load_body_to_dict(body)
         else:
             body_dict = body
 
         response = api.create_namespaced_custom_object(
             group=group,
             version=version,
-            namespace=namespace or self.get_namespace(),
+            namespace=namespace or self.get_namespace() or self.DEFAULT_NAMESPACE,
             plural=plural,
             body=body_dict,
         )
 
         self.log.debug("Response: %s", response)
         return response
 
@@ -323,15 +315,15 @@
         :param name: crd object name
         :param namespace: kubernetes namespace
         """
         api = client.CustomObjectsApi(self.api_client)
         response = api.get_namespaced_custom_object(
             group=group,
             version=version,
-            namespace=namespace or self.get_namespace(),
+            namespace=namespace or self.get_namespace() or self.DEFAULT_NAMESPACE,
             plural=plural,
             name=name,
         )
         return response
 
     def delete_custom_object(
         self, group: str, version: str, plural: str, name: str, namespace: str | None = None, **kwargs
@@ -345,60 +337,26 @@
         :param name: crd object name
         :param namespace: kubernetes namespace
         """
         api = client.CustomObjectsApi(self.api_client)
         return api.delete_namespaced_custom_object(
             group=group,
             version=version,
-            namespace=namespace or self.get_namespace(),
+            namespace=namespace or self.get_namespace() or self.DEFAULT_NAMESPACE,
             plural=plural,
             name=name,
             **kwargs,
         )
 
     def get_namespace(self) -> str | None:
-        """
-        Returns the namespace defined in the connection or 'default'.
-
-        TODO: in provider version 6.0, return None when namespace not defined in connection
-        """
-        namespace = self._get_namespace()
-        if self.conn_id and not namespace:
-            warnings.warn(
-                "Airflow connection defined but namespace is not set; returning 'default'.  In "
-                "cncf.kubernetes provider version 6.0 we will return None when namespace is "
-                "not defined in the connection so that it's clear whether user intends 'default' or "
-                "whether namespace is unset (which is required in order to apply precedence logic in "
-                "KubernetesPodOperator).",
-                AirflowProviderDeprecationWarning,
-            )
-            return "default"
-        return namespace
-
-    def _get_namespace(self) -> str | None:
-        """
-        Returns the namespace that defined in the connection
-
-        TODO: in provider version 6.0, get rid of this method and make it the behavior of get_namespace.
-        """
+        """Returns the namespace that defined in the connection"""
         if self.conn_id:
             return self._get_field("namespace")
         return None
 
-    def get_xcom_sidecar_container_image(self):
-        """Returns the xcom sidecar image that defined in the connection"""
-        return self._get_field("xcom_sidecar_container_image")
-
-    def get_xcom_sidecar_container_resources(self):
-        """Returns the xcom sidecar resources that defined in the connection"""
-        field = self._get_field("xcom_sidecar_container_resources")
-        if not field:
-            return None
-        return json.loads(field)
-
     def get_pod_log_stream(
         self,
         pod_name: str,
         container: str | None = "",
         namespace: str | None = None,
     ) -> tuple[watch.Watch, Generator[str, None, None]]:
         """
@@ -411,15 +369,15 @@
         watcher = watch.Watch()
         return (
             watcher,
             watcher.stream(
                 self.core_v1_client.read_namespaced_pod_log,
                 name=pod_name,
                 container=container,
-                namespace=namespace or self._get_namespace() or self.DEFAULT_NAMESPACE,
+                namespace=namespace or self.get_namespace() or self.DEFAULT_NAMESPACE,
             ),
         )
 
     def get_pod_logs(
         self,
         pod_name: str,
         container: str | None = "",
@@ -432,15 +390,15 @@
         :param container: container name
         :param namespace: kubernetes namespace
         """
         return self.core_v1_client.read_namespaced_pod_log(
             name=pod_name,
             container=container,
             _preload_content=False,
-            namespace=namespace or self._get_namespace() or self.DEFAULT_NAMESPACE,
+            namespace=namespace or self.get_namespace() or self.DEFAULT_NAMESPACE,
         )
 
     def get_pod(self, name: str, namespace: str) -> V1Pod:
         """Read pod object from kubernetes API."""
         return self.core_v1_client.read_namespaced_pod(
             name=name,
             namespace=namespace,
@@ -456,15 +414,15 @@
         """
         Retrieves a list of Kind pod which belong default kubernetes namespace
         :param label_selector: A selector to restrict the list of returned objects by their labels
         :param namespace: kubernetes namespace
         :param watch: Watch for changes to the described resources and return them as a stream
         """
         return self.core_v1_client.list_namespaced_pod(
-            namespace=namespace or self._get_namespace() or self.DEFAULT_NAMESPACE,
+            namespace=namespace or self.get_namespace() or self.DEFAULT_NAMESPACE,
             watch=watch,
             label_selector=label_selector,
             _preload_content=False,
             **kwargs,
         )
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,29 +16,27 @@
 # under the License.
 """Executes task in a Kubernetes POD"""
 
 from __future__ import annotations
 
 import json
 import logging
-import os
 import re
 import secrets
 import string
-import warnings
 from collections.abc import Container
 from contextlib import AbstractContextManager
 from typing import TYPE_CHECKING, Any, Sequence
 
 from kubernetes.client import CoreV1Api, models as k8s
 from slugify import slugify
 from urllib3.exceptions import HTTPError
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning, AirflowSkipException
+from airflow.exceptions import AirflowException, AirflowSkipException
 from airflow.kubernetes import pod_generator
 from airflow.kubernetes.pod_generator import PodGenerator
 from airflow.kubernetes.secret import Secret
 from airflow.models import BaseOperator
 from airflow.providers.cncf.kubernetes.backcompat.backwards_compat_converters import (
     convert_affinity,
     convert_configmap,
@@ -469,22 +467,14 @@
             conn_id=self.kubernetes_conn_id,
             in_cluster=self.in_cluster,
             config_file=self.config_file,
             cluster_context=self.cluster_context,
         )
         return hook
 
-    def get_hook(self):
-        warnings.warn(
-            "get_hook is deprecated. Please use hook instead.",
-            AirflowProviderDeprecationWarning,
-            stacklevel=2,
-        )
-        return self.hook
-
     @cached_property
     def client(self) -> CoreV1Api:
         return self.hook.core_v1_client
 
     def find_pod(self, namespace: str, context: Context, *, exclude_checked: bool = True) -> k8s.V1Pod | None:
         """Returns an already-running pod for this task instance if one exists."""
         label_selector = self._build_find_pod_label_selector(context, exclude_checked=exclude_checked)
@@ -585,28 +575,14 @@
         self.pod_request_obj = self.build_pod_request_obj(context)
         self.pod = self.get_or_create_pod(  # must set `self.pod` for `on_kill`
             pod_request_obj=self.pod_request_obj,
             context=context,
         )
         self.invoke_defer_method()
 
-    def convert_config_file_to_dict(self):
-        """Converts passed config_file to dict format."""
-        warnings.warn(
-            "This method is deprecated and will be removed in a future version.",
-            AirflowProviderDeprecationWarning,
-            stacklevel=2,
-        )
-        config_file = self.config_file if self.config_file else os.environ.get(KUBE_CONFIG_ENV_VAR)
-        if config_file:
-            with open(config_file) as f:
-                self._config_dict = yaml.safe_load(f)
-        else:
-            self._config_dict = None
-
     def invoke_defer_method(self):
         """Method to easily redefine triggers which are being used in child classes."""
         trigger_start_time = utcnow()
         self.defer(
             trigger=KubernetesPodTrigger(
                 pod_name=self.pod.metadata.name,
                 pod_namespace=self.pod.metadata.namespace,
@@ -847,30 +823,24 @@
                 task_id=self.task_id, unique=self.random_name_suffix, max_length=80
             )
         elif self.random_name_suffix:
             # user has supplied pod name, we're just adding suffix
             pod.metadata.name = _add_pod_suffix(pod_name=pod.metadata.name)
 
         if not pod.metadata.namespace:
-            # todo: replace with call to `hook.get_namespace` in 6.0, when it doesn't default to `default`.
-            # if namespace not actually defined in hook, we want to check k8s if in cluster
-            hook_namespace = self.hook._get_namespace()
+            hook_namespace = self.hook.get_namespace()
             pod_namespace = self.namespace or hook_namespace or self._incluster_namespace or "default"
             pod.metadata.namespace = pod_namespace
 
         for secret in self.secrets:
             self.log.debug("Adding secret to task %s", self.task_id)
             pod = secret.attach_to_pod(pod)
         if self.do_xcom_push:
             self.log.debug("Adding xcom sidecar to task %s", self.task_id)
-            pod = xcom_sidecar.add_xcom_sidecar(
-                pod,
-                sidecar_container_image=self.hook.get_xcom_sidecar_container_image(),
-                sidecar_container_resources=self.hook.get_xcom_sidecar_container_resources(),
-            )
+            pod = xcom_sidecar.add_xcom_sidecar(pod)
 
         labels = self._get_ti_pod_labels(context)
         self.log.info("Building pod %s with labels: %s", pod.metadata.name, labels)
 
         # Merge Pod Identifying labels with labels passed to operator
         pod.metadata.labels.update(labels)
         # Add Airflow Version to the label
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,26 +89,16 @@
     @property
     def is_in_cluster(self) -> bool:
         """Expose whether the hook is configured with ``load_incluster_config`` or not"""
 
     def get_pod(self, name: str, namespace: str) -> V1Pod:
         """Read pod object from kubernetes API."""
 
-    def _get_namespace(self) -> str | None:
-        """
-        Returns the namespace that defined in the connection
-
-        TODO: in provider version 6.0, get rid of this method and make it the behavior of get_namespace.
-        """
-
-    def get_xcom_sidecar_container_image(self) -> str | None:
-        """Returns the xcom sidecar image that defined in the connection"""
-
-    def get_xcom_sidecar_container_resources(self) -> str | None:
-        """Returns the xcom sidecar resources that defined in the connection"""
+    def get_namespace(self) -> str | None:
+        """Returns the namespace that defined in the connection"""
 
 
 def get_container_status(pod: V1Pod, container_name: str) -> V1ContainerStatus | None:
     """Retrieves container status"""
     container_statuses = pod.status.container_statuses if pod and pod.status else None
     if container_statuses:
         # In general the variable container_statuses can store multiple items matching different containers.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 6.2.0rc1
+Version: 7.0.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``6.2.0rc1``
+Release: ``7.0.0rc2``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -112,21 +112,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-6.2.0
+
+
+7.0.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+.. note::
+  Return None when namespace is not defined in the Kubernetes connection
+
+* ``Remove deprecated features from KubernetesHook (#31402)``
+
 Features
 ~~~~~~~~
 
 .. note::
   If ``kubernetes_default`` connection is not defined, then KubernetesHook / KubernetesPodOperator will behave as though given ``conn_id=None``.
   This should make it easier to mitigate breaking change introduced in 6.0.0
 
@@ -150,14 +160,18 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Upgrade ruff to 0.0.262 (#30809)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
    * ``Fix pod describing on system test failure (#31191)``
+   * ``Docstring improvements (#31375)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
 
 6.1.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/pyproject.toml` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     # implicit single-line string concatenation
     "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
+    # "D400", WIP: see #31135
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
     "D403",
     "D412",
     "D419"
 ]
 extend-ignore = [
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/setup.cfg` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -56,10 +56,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.cncf.kubernetes.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.cncf.kubernetes
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/setup.py` & `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-cncf-kubernetes package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "6.2.0"
+version = "7.0.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-cncf-kubernetes setup."""
     setup(
         version=version,
         extras_require={},
```

