# Comparing `tmp/spike2loader-0.1.tar.gz` & `tmp/spike2loader-0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spike2loader-0.1.tar", last modified: Tue Mar  7 10:51:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

