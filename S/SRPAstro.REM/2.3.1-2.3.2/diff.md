# Comparing `tmp/SRPAstro.REM-2.3.1.tar.gz` & `tmp/SRPAstro.REM-2.3.2-py3.9.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SRPAstro.REM-2.3.1.tar", last modified: Thu Mar 10 16:38:59 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

