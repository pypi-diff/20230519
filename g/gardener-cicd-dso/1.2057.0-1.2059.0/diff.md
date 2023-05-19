# Comparing `tmp/gardener-cicd-dso-1.2057.0.tar.gz` & `tmp/gardener_cicd_dso-1.2059.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-dso-1.2057.0.tar", last modified: Wed May 17 13:36:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

