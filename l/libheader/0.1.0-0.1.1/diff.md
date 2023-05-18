# Comparing `tmp/libheader-0.1.0.tar.gz` & `tmp/libheader-0.1.1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libheader-0.1.0.tar", last modified: Thu May 18 21:46:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

