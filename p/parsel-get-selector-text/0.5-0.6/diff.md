# Comparing `tmp/parsel_get_selector_text-0.5.tar.gz` & `tmp/parsel_get_selector_text-0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsel_get_selector_text-0.5.tar", last modified: Sun May  7 21:18:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

