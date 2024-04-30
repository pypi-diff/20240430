# Comparing `tmp/backend.ai-kernel-24.3.3rc2.tar.gz` & `tmp/backend.ai_kernel-24.3.3rc3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-kernel-24.3.3rc2.tar", last modified: Tue Apr 30 06:26:17 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

