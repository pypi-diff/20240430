# Comparing `tmp/esanalyzer-1.0.5.tar.gz` & `tmp/esanalyzer-1.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esanalyzer-1.0.5.tar", last modified: Mon Apr 29 10:20:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

