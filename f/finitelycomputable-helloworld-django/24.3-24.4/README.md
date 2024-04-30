# Comparing `tmp/finitelycomputable-helloworld-django-24.3.tar.gz` & `tmp/finitelycomputable_helloworld_django-24.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable-helloworld-django-24.3.tar", last modified: Mon Apr  1 03:33:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
