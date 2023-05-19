# Comparing `tmp/tests4py-0.0.1a0.tar.gz` & `tmp/tests4py-0.0.1b0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tests4py-0.0.1a0.tar", last modified: Tue Mar 28 11:11:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

