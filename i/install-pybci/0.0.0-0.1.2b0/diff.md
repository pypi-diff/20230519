# Comparing `tmp/install-pybci-0.0.0.tar.gz` & `tmp/install_pybci-0.1.2b0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.0.0.tar", last modified: Thu May 18 23:57:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

