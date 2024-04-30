# Comparing `tmp/rdeploy-0.1.7.tar.gz` & `tmp/rdeploy-0.1.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rdeploy-0.1.7.tar", last modified: Mon Oct 31 17:42:18 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

