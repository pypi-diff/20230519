# Comparing `tmp/pyecsca-0.1.0.tar.gz` & `tmp/pyecsca-0.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecsca-0.1.0.tar", last modified: Sat Jan 16 17:37:05 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

