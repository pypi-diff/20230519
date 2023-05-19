# Comparing `tmp/parse_broken_json-0.1.tar.gz` & `tmp/parse_broken_json-0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse_broken_json-0.1.tar", last modified: Sun May  7 21:29:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

