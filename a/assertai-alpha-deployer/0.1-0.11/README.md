# Comparing `tmp/assertai-alpha-deployer-0.1.tar.gz` & `tmp/assertai_alpha_deployer-0.11-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assertai-alpha-deployer-0.1.tar", last modified: Mon Apr 29 13:07:15 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

