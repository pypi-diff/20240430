# Comparing `tmp/mlswarm-0.31.tar.gz` & `tmp/mlswarm-0.32-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlswarm-0.31.tar", last modified: Sun Aug 11 14:41:17 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

