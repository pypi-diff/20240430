# Comparing `tmp/stratigraph-0.1.1.tar.gz` & `tmp/stratigraph-0.1.1.dev0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stratigraph-0.1.1.tar", last modified: Mon Apr 29 21:45:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

