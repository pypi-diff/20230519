# Comparing `tmp/pycommremover-0.1.tar.gz` & `tmp/pycommremover-0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycommremover-0.1.tar", last modified: Tue May 10 23:51:04 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

