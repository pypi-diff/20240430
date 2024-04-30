# Comparing `tmp/mypy-boto3-omics-1.34.83.tar.gz` & `tmp/mypy_boto3_omics-1.34.95-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-omics-1.34.83.tar", last modified: Thu Apr 11 19:18:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

