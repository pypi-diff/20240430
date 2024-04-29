# Comparing `tmp/lollms_client-0.5.0.tar.gz` & `tmp/lollms_client-0.5.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms_client-0.5.0.tar", last modified: Sun Apr 28 00:01:29 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

