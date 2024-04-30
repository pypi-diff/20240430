# Comparing `tmp/VisionCraft-0.1.19.tar.gz` & `tmp/VisionCraft-0.1.20-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionCraft-0.1.19.tar", last modified: Tue Apr 30 04:19:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

