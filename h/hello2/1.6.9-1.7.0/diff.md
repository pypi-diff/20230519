# Comparing `tmp/hello2-1.6.9.tar.gz` & `tmp/hello2-1.7.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello2-1.6.9.tar", last modified: Wed May 17 04:12:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

