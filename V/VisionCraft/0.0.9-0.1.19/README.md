# Comparing `tmp/VisionCraft-0.0.9.tar.gz` & `tmp/VisionCraft-0.1.19-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionCraft-0.0.9.tar", last modified: Tue Mar 12 14:11:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

