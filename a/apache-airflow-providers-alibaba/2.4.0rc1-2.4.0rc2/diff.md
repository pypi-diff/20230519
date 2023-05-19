# Comparing `tmp/apache-airflow-providers-alibaba-2.4.0rc1.tar.gz` & `tmp/apache_airflow_providers_alibaba-2.4.0rc2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-alibaba-2.4.0rc1.tar", last modified: Tue May 16 15:52:47 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

