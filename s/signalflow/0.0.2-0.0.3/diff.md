# Comparing `tmp/signalflow-0.0.2.tar.gz` & `tmp/signalflow-0.0.3-cp39-cp39-macosx_12_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signalflow-0.0.2.tar", last modified: Wed Jan  4 00:06:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

