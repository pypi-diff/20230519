# Comparing `tmp/reactpy_jupyter-0.8.1.tar.gz` & `tmp/reactpy_jupyter-0.9.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactpy_jupyter-0.8.1.tar", last modified: Sat Apr 15 01:57:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

