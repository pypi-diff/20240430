# Comparing `tmp/vlt-sphere-1.6.1.tar.gz` & `tmp/vlt_sphere-1.7-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlt-sphere-1.6.1.tar", last modified: Tue Jun 14 14:42:12 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

