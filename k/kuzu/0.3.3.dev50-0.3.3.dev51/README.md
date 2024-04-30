# Comparing `tmp/kuzu-0.3.3.dev50.tar.gz` & `tmp/kuzu-0.3.3.dev51-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.3.3.dev50.tar", last modified: Mon Apr 29 08:05:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

