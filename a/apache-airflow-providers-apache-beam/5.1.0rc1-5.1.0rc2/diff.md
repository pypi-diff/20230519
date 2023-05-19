# Comparing `tmp/apache-airflow-providers-apache-beam-5.1.0rc1.tar.gz` & `tmp/apache_airflow_providers_apache_beam-5.1.0rc2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-beam-5.1.0rc1.tar", last modified: Tue May 16 15:52:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

