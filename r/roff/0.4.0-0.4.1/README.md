# Comparing `tmp/roff-0.4.0.tar.gz` & `tmp/roff-0.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roff-0.4.0.tar", last modified: Tue Apr 30 13:55:41 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

