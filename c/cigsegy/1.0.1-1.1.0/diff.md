# Comparing `tmp/cigsegy-1.0.1.tar.gz` & `tmp/cigsegy-1.1.0-cp39-cp39-manylinux_2_24_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cigsegy-1.0.1.tar", last modified: Thu Feb 16 11:03:14 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

