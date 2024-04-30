# Comparing `tmp/gardener_cicd_cli-1.2389.0.tar.gz` & `tmp/gardener_cicd_cli-1.2390.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener_cicd_cli-1.2389.0.tar", last modified: Tue Apr 30 09:51:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

