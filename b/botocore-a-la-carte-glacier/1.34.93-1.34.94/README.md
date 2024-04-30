# Comparing `tmp/botocore-a-la-carte-glacier-1.34.93.tar.gz` & `tmp/botocore_a_la_carte_glacier-1.34.94-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-glacier-1.34.93.tar", last modified: Sat Apr 27 01:00:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

