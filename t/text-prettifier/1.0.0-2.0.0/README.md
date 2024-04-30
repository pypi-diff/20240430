# Comparing `tmp/text_prettifier-1.0.0.tar.gz` & `tmp/text_prettifier-2.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_prettifier-1.0.0.tar", last modified: Tue Apr 30 10:48:17 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

