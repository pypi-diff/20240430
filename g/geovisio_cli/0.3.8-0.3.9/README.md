# Comparing `tmp/geovisio_cli-0.3.8.tar.gz` & `tmp/geovisio_cli-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovisio_cli-0.3.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geovisio_cli-0.3.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geovisio_cli-0.3.8.tar` & `geovisio_cli-0.3.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0       56 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/.gitignore
--rw-r--r--   0        0        0     4857 2023-12-20 15:13:39.166384 geovisio_cli-0.3.8/.gitlab-ci.yml
--rw-r--r--   0        0        0       91 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6581 2023-12-20 15:56:46.804033 geovisio_cli-0.3.8/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/LICENSE
--rw-r--r--   0        0        0      590 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/Makefile
--rw-r--r--   0        0        0    11187 2023-12-20 15:13:39.166384 geovisio_cli-0.3.8/README.md
--rw-r--r--   0        0        0     5096 2023-12-20 15:56:46.804033 geovisio_cli-0.3.8/USAGE.md
--rw-r--r--   0        0        0       53 2023-12-20 15:56:46.804033 geovisio_cli-0.3.8/geovisio_cli/__init__.py
--rw-r--r--   0        0        0       41 2023-12-20 15:13:39.166384 geovisio_cli-0.3.8/geovisio_cli/__main__.py
--rw-r--r--   0        0        0     6477 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/auth.py
--rw-r--r--   0        0        0      284 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/exception.py
--rw-r--r--   0        0        0     9997 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/main.py
--rw-r--r--   0        0        0     9792 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/model.py
--rw-r--r--   0        0        0        0 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/sequences/__init__.py
--rw-r--r--   0        0        0     1391 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/sequences/external_metadata/__init__.py
--rw-r--r--   0        0        0     2402 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/sequences/external_metadata/csv_metadata.py
--rw-r--r--   0        0        0     2225 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/sequences/external_metadata/utils.py
--rw-r--r--   0        0        0        0 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/sequences/process/__init__.py
--rw-r--r--   0        0        0    11798 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/sequences/process/standard.py
--rw-r--r--   0        0        0     5369 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/sequences/status.py
--rw-r--r--   0        0        0    11377 2023-11-23 08:15:32.626055 geovisio_cli-0.3.8/geovisio_cli/sequences/upload.py
--rw-r--r--   0        0        0     2763 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/geovisio_cli/utils.py
--rw-r--r--   0        0        0      324 2023-12-20 15:13:39.166384 geovisio_cli-0.3.8/pyinstaller/hooks/hook-pyexiv2.py
--rw-r--r--   0        0        0     1361 2023-12-20 15:26:43.546259 geovisio_cli-0.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0      234 2023-11-02 10:57:34.878890 geovisio_cli-0.3.8/tests/conftest.py
--rw-r--r--   0        0        0   523332 2023-11-02 10:57:34.882890 geovisio_cli-0.3.8/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0   484422 2023-11-02 10:57:34.882890 geovisio_cli-0.3.8/tests/fixtures/e1_without_exif.jpg
--rw-r--r--   0        0        0   483454 2023-11-02 10:57:34.882890 geovisio_cli-0.3.8/tests/fixtures/e2.jpg
--rw-r--r--   0        0        0   483375 2023-11-02 10:57:34.882890 geovisio_cli-0.3.8/tests/fixtures/e2_without_coord.jpg
--rw-r--r--   0        0        0   529344 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/fixtures/e3.jpg
--rw-r--r--   0        0        0   489922 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/fixtures/e3_without_exif.jpg
--rw-r--r--   0        0        0       16 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/fixtures/invalid_pic.jpg
--rw-r--r--   0        0        0      165 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/fixtures/metadata.csv
--rw-r--r--   0        0        0      215 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/fixtures/metadata_exif.csv
--rw-r--r--   0        0        0       27 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/fixtures/not_a_pic.md
--rw-r--r--   0        0        0        0 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/integration/__init__.py
--rw-r--r--   0        0        0     3327 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/integration/conftest.py
--rw-r--r--   0        0        0     2189 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/integration/docker-compose-geovisio.yml
--rw-r--r--   0        0        0      541 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/integration/docker-compose-gitlab-override.yml
--rw-r--r--   0        0        0    76457 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/integration/keycloak-realm.json
--rw-r--r--   0        0        0     3490 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/integration/test_auth.py
--rw-r--r--   0        0        0      563 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/integration/test_status.py
--rw-r--r--   0        0        0    13047 2023-11-02 11:51:59.727685 geovisio_cli-0.3.8/tests/integration/test_upload.py
--rw-r--r--   0        0        0     2765 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/integration/test_upload_csv_metadata.py
--rw-r--r--   0        0        0     3624 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/test_csv_metadata_reader.py
--rw-r--r--   0        0        0      805 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/test_external_metadata_utils.py
--rw-r--r--   0        0        0     9830 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/test_model.py
--rw-r--r--   0        0        0     8961 2023-11-14 07:46:31.345004 geovisio_cli-0.3.8/tests/test_process.py
--rw-r--r--   0        0        0    12923 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/test_sequence_standard.py
--rw-r--r--   0        0        0     5689 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/test_sequence_upload.py
--rw-r--r--   0        0        0      902 2023-11-02 10:57:34.886890 geovisio_cli-0.3.8/tests/test_utils.py
--rw-r--r--   0        0        0    12510 1970-01-01 00:00:00.000000 geovisio_cli-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/.gitignore
+-rw-r--r--   0        0        0     4857 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/.gitlab-ci.yml
+-rw-r--r--   0        0        0       91 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6858 2024-03-15 11:24:23.261630 geovisio_cli-0.3.9/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/LICENSE
+-rw-r--r--   0        0        0      590 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/Makefile
+-rw-r--r--   0        0        0    11187 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/README.md
+-rw-r--r--   0        0        0     5096 2024-03-15 11:24:23.261630 geovisio_cli-0.3.9/USAGE.md
+-rw-r--r--   0        0        0       53 2024-03-15 11:24:23.261630 geovisio_cli-0.3.9/geovisio_cli/__init__.py
+-rw-r--r--   0        0        0       41 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/__main__.py
+-rw-r--r--   0        0        0     6477 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/auth.py
+-rw-r--r--   0        0        0      284 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/exception.py
+-rw-r--r--   0        0        0     9997 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/main.py
+-rw-r--r--   0        0        0     9792 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/model.py
+-rw-r--r--   0        0        0        0 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/sequences/__init__.py
+-rw-r--r--   0        0        0     1391 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/sequences/external_metadata/__init__.py
+-rw-r--r--   0        0        0     2402 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/sequences/external_metadata/csv_metadata.py
+-rw-r--r--   0        0        0     2225 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/sequences/external_metadata/utils.py
+-rw-r--r--   0        0        0        0 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/sequences/process/__init__.py
+-rw-r--r--   0        0        0    11798 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/sequences/process/standard.py
+-rw-r--r--   0        0        0     5369 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/sequences/status.py
+-rw-r--r--   0        0        0    11377 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/sequences/upload.py
+-rw-r--r--   0        0        0     2763 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/geovisio_cli/utils.py
+-rw-r--r--   0        0        0      324 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/pyinstaller/hooks/hook-pyexiv2.py
+-rw-r--r--   0        0        0     1361 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/tests/__init__.py
+-rw-r--r--   0        0        0      234 2024-03-06 15:24:06.225327 geovisio_cli-0.3.9/tests/conftest.py
+-rw-r--r--   0        0        0   523332 2024-03-06 15:24:06.229327 geovisio_cli-0.3.9/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0   484422 2024-03-06 15:24:06.229327 geovisio_cli-0.3.9/tests/fixtures/e1_without_exif.jpg
+-rw-r--r--   0        0        0   483454 2024-03-06 15:24:06.229327 geovisio_cli-0.3.9/tests/fixtures/e2.jpg
+-rw-r--r--   0        0        0   483375 2024-03-06 15:24:06.229327 geovisio_cli-0.3.9/tests/fixtures/e2_without_coord.jpg
+-rw-r--r--   0        0        0   529344 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/fixtures/e3.jpg
+-rw-r--r--   0        0        0   489922 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/fixtures/e3_without_exif.jpg
+-rw-r--r--   0        0        0       16 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/fixtures/invalid_pic.jpg
+-rw-r--r--   0        0        0      165 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/fixtures/metadata.csv
+-rw-r--r--   0        0        0      215 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/fixtures/metadata_exif.csv
+-rw-r--r--   0        0        0       27 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/fixtures/not_a_pic.md
+-rw-r--r--   0        0        0        0 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3327 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2189 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/integration/docker-compose-geovisio.yml
+-rw-r--r--   0        0        0      541 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/integration/docker-compose-gitlab-override.yml
+-rw-r--r--   0        0        0    76457 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/integration/keycloak-realm.json
+-rw-r--r--   0        0        0     3490 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/integration/test_auth.py
+-rw-r--r--   0        0        0      563 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/integration/test_status.py
+-rw-r--r--   0        0        0    13047 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/integration/test_upload.py
+-rw-r--r--   0        0        0     2765 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/integration/test_upload_csv_metadata.py
+-rw-r--r--   0        0        0     3624 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/test_csv_metadata_reader.py
+-rw-r--r--   0        0        0      805 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/test_external_metadata_utils.py
+-rw-r--r--   0        0        0     9830 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/test_model.py
+-rw-r--r--   0        0        0     8961 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/test_process.py
+-rw-r--r--   0        0        0    12923 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/test_sequence_standard.py
+-rw-r--r--   0        0        0     5689 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/test_sequence_upload.py
+-rw-r--r--   0        0        0      902 2024-03-06 15:24:06.233327 geovisio_cli-0.3.9/tests/test_utils.py
+-rw-r--r--   0        0        0    12510 1970-01-01 00:00:00.000000 geovisio_cli-0.3.9/PKG-INFO
```

### Comparing `geovisio_cli-0.3.8/.gitlab-ci.yml` & `geovisio_cli-0.3.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/CHANGELOG.md` & `geovisio_cli-0.3.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+
+## [0.3.9] - 2024-03-15
+
+### Changed
+
+- Update [geo-picture-tag-reader](https://gitlab.com/geovisio/geo-picture-tag-reader) to [1.0.5 version](https://gitlab.com/geovisio/geo-picture-tag-reader/-/tags/1.0.5).
+
+
 ## [0.3.8] - 2023-12-20
 
 ### Changed
 
 - Update [geo-picture-tag-reader](https://gitlab.com/geovisio/geo-picture-tag-reader) to [1.0.3 version](https://gitlab.com/geovisio/geo-picture-tag-reader/-/tags/1.0.3).
 
 ## [0.3.7] - 2023-11-24
@@ -141,15 +149,16 @@
 
 ## [0.0.1] - 2023-03-14
 
 ### Added
 - Basic scripts for uploading pictures to a GeoVisio API
 
 
-[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.3.8...main
+[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.3.9...main
+[0.3.9]: https://gitlab.com/geovisio/cli/-/compare/0.3.8...0.3.9
 [0.3.8]: https://gitlab.com/geovisio/cli/-/compare/0.3.7...0.3.8
 [0.3.7]: https://gitlab.com/geovisio/cli/-/compare/0.3.6...0.3.7
 [0.3.6]: https://gitlab.com/geovisio/cli/-/compare/0.3.5...0.3.6
 [0.3.5]: https://gitlab.com/geovisio/cli/-/compare/0.3.4...0.3.5
 [0.3.4]: https://gitlab.com/geovisio/cli/-/compare/0.3.3...0.3.4
 [0.3.3]: https://gitlab.com/geovisio/cli/-/compare/0.3.2...0.3.3
 [0.3.2]: https://gitlab.com/geovisio/cli/-/compare/0.3.1...0.3.2
```

### Comparing `geovisio_cli-0.3.8/CODE_OF_CONDUCT.md` & `geovisio_cli-0.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/LICENSE` & `geovisio_cli-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/Makefile` & `geovisio_cli-0.3.9/Makefile`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/README.md` & `geovisio_cli-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/USAGE.md` & `geovisio_cli-0.3.9/USAGE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # `geovisio`
 
-GeoVisio command-line client (v0.3.8)
+GeoVisio command-line client (v0.3.9)
 
 **Usage**:
 
 ```console
 $ geovisio [OPTIONS] COMMAND [ARGS]...
 ```
```

### Comparing `geovisio_cli-0.3.8/geovisio_cli/auth.py` & `geovisio_cli-0.3.9/geovisio_cli/auth.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/geovisio_cli/main.py` & `geovisio_cli-0.3.9/geovisio_cli/main.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/geovisio_cli/model.py` & `geovisio_cli-0.3.9/geovisio_cli/model.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/geovisio_cli/sequences/external_metadata/__init__.py` & `geovisio_cli-0.3.9/geovisio_cli/sequences/external_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/geovisio_cli/sequences/external_metadata/csv_metadata.py` & `geovisio_cli-0.3.9/geovisio_cli/sequences/external_metadata/csv_metadata.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/geovisio_cli/sequences/external_metadata/utils.py` & `geovisio_cli-0.3.9/geovisio_cli/sequences/external_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/geovisio_cli/sequences/process/standard.py` & `geovisio_cli-0.3.9/geovisio_cli/sequences/process/standard.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/geovisio_cli/sequences/status.py` & `geovisio_cli-0.3.9/geovisio_cli/sequences/status.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/geovisio_cli/sequences/upload.py` & `geovisio_cli-0.3.9/geovisio_cli/sequences/upload.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/geovisio_cli/utils.py` & `geovisio_cli-0.3.9/geovisio_cli/utils.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/pyproject.toml` & `geovisio_cli-0.3.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 dependencies = [
     "requests ~= 2.28",
     "typer ~= 0.9",
     "rich ~= 13.4",
     "tomli ~= 2.0.1",
     "tomli-w ~= 1.0.0",
     "qrcode ~= 7.4",
-    "geopic-tag-reader ~= 1.0.3",
+    "geopic-tag-reader ~= 1.0.5",
     "packaging ~= 23.1",
     "haversine ~= 2.8",
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Home = "https://gitlab.com/geovisio/cli"
```

### Comparing `geovisio_cli-0.3.8/tests/fixtures/e1.jpg` & `geovisio_cli-0.3.9/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/fixtures/e1_without_exif.jpg` & `geovisio_cli-0.3.9/tests/fixtures/e1_without_exif.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/fixtures/e2.jpg` & `geovisio_cli-0.3.9/tests/fixtures/e2.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/fixtures/e2_without_coord.jpg` & `geovisio_cli-0.3.9/tests/fixtures/e2_without_coord.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/fixtures/e3.jpg` & `geovisio_cli-0.3.9/tests/fixtures/e3.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/fixtures/e3_without_exif.jpg` & `geovisio_cli-0.3.9/tests/fixtures/e3_without_exif.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/integration/conftest.py` & `geovisio_cli-0.3.9/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/integration/docker-compose-geovisio.yml` & `geovisio_cli-0.3.9/tests/integration/docker-compose-geovisio.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/integration/docker-compose-gitlab-override.yml` & `geovisio_cli-0.3.9/tests/integration/docker-compose-gitlab-override.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/integration/keycloak-realm.json` & `geovisio_cli-0.3.9/tests/integration/keycloak-realm.json`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/integration/test_auth.py` & `geovisio_cli-0.3.9/tests/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/integration/test_status.py` & `geovisio_cli-0.3.9/tests/integration/test_status.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/integration/test_upload.py` & `geovisio_cli-0.3.9/tests/integration/test_upload.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/integration/test_upload_csv_metadata.py` & `geovisio_cli-0.3.9/tests/integration/test_upload_csv_metadata.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/test_csv_metadata_reader.py` & `geovisio_cli-0.3.9/tests/test_csv_metadata_reader.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/test_external_metadata_utils.py` & `geovisio_cli-0.3.9/tests/test_external_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/test_model.py` & `geovisio_cli-0.3.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/test_process.py` & `geovisio_cli-0.3.9/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/test_sequence_standard.py` & `geovisio_cli-0.3.9/tests/test_sequence_standard.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/test_sequence_upload.py` & `geovisio_cli-0.3.9/tests/test_sequence_upload.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/tests/test_utils.py` & `geovisio_cli-0.3.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.3.8/PKG-INFO` & `geovisio_cli-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: geovisio_cli
-Version: 0.3.8
+Version: 0.3.9
 Summary: Geovio client cli tool
 Author-email: Antoine Desbordes <antoine.desbordes@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests ~= 2.28
 Requires-Dist: typer ~= 0.9
 Requires-Dist: rich ~= 13.4
 Requires-Dist: tomli ~= 2.0.1
 Requires-Dist: tomli-w ~= 1.0.0
 Requires-Dist: qrcode ~= 7.4
-Requires-Dist: geopic-tag-reader ~= 1.0.3
+Requires-Dist: geopic-tag-reader ~= 1.0.5
 Requires-Dist: packaging ~= 23.1
 Requires-Dist: haversine ~= 2.8
 Requires-Dist: flit ~= 3.8.0 ; extra == "build"
 Requires-Dist: pyinstaller ~= 6.3.0 ; extra == "build-binary"
 Requires-Dist: black ~= 22.8.0 ; extra == "dev"
 Requires-Dist: mypy ~= 1.0.0 ; extra == "dev"
 Requires-Dist: types-requests ~= 2.28.0 ; extra == "dev"
```

