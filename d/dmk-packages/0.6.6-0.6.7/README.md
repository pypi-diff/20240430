# Comparing `tmp/dmk_packages-0.6.6.tar.gz` & `tmp/dmk_packages-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmk_packages-0.6.6.tar", last modified: Wed Apr 24 08:56:46 2024, max compression
+gzip compressed data, was "dmk_packages-0.6.7.tar", last modified: Tue Apr 30 07:14:08 2024, max compression
```

## Comparing `dmk_packages-0.6.6.tar` & `dmk_packages-0.6.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:46.002235 dmk_packages-0.6.6/
--rw-r--r--   0 tommie     (501) staff       (20)    11347 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/LICENSE
--rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-24 08:56:46.002006 dmk_packages-0.6.6/PKG-INFO
--rw-r--r--   0 tommie     (501) staff       (20)     1365 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/README.md
--rw-r--r--   0 tommie     (501) staff       (20)      584 2024-04-24 08:53:14.000000 dmk_packages-0.6.6/pyproject.toml
--rw-r--r--   0 tommie     (501) staff       (20)       38 2024-04-24 08:56:46.002282 dmk_packages-0.6.6/setup.cfg
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:45.996546 dmk_packages-0.6.6/src/
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:45.997665 dmk_packages-0.6.6/src/dmk_packages/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/__init__.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:46.000952 dmk_packages-0.6.6/src/dmk_packages/crawler/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/__init__.py
--rw-r--r--   0 tommie     (501) staff       (20)     3534 2024-04-24 08:52:39.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/bigkinds.py
--rw-r--r--   0 tommie     (501) staff       (20)     6580 2024-04-24 08:53:08.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/clien.py
--rw-r--r--   0 tommie     (501) staff       (20)     6600 2024-04-24 08:52:39.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/fnguide.py
--rw-r--r--   0 tommie     (501) staff       (20)     2321 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/naver_blog.py
--rw-r--r--   0 tommie     (501) staff       (20)    15349 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/naver_search_volume.py
--rw-r--r--   0 tommie     (501) staff       (20)     1382 2024-04-24 08:52:39.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/pdf_to_text.py
--rw-r--r--   0 tommie     (501) staff       (20)    13362 2024-04-23 05:01:14.000000 dmk_packages-0.6.6/src/dmk_packages/crawler/youtube.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:46.001451 dmk_packages-0.6.6/src/dmk_packages/database/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/database/__init__.py
--rw-r--r--   0 tommie     (501) staff       (20)     3057 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/database/database.py
--rw-r--r--   0 tommie     (501) staff       (20)     1895 2024-04-04 04:45:57.000000 dmk_packages-0.6.6/src/dmk_packages/naver_datalab.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-24 08:56:46.001745 dmk_packages-0.6.6/src/dmk_packages.egg-info/
--rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-24 08:56:45.000000 dmk_packages-0.6.6/src/dmk_packages.egg-info/PKG-INFO
--rw-r--r--   0 tommie     (501) staff       (20)      677 2024-04-24 08:56:45.000000 dmk_packages-0.6.6/src/dmk_packages.egg-info/SOURCES.txt
--rw-r--r--   0 tommie     (501) staff       (20)        1 2024-04-24 08:56:45.000000 dmk_packages-0.6.6/src/dmk_packages.egg-info/dependency_links.txt
--rw-r--r--   0 tommie     (501) staff       (20)       41 2024-04-24 08:56:45.000000 dmk_packages-0.6.6/src/dmk_packages.egg-info/requires.txt
--rw-r--r--   0 tommie     (501) staff       (20)       13 2024-04-24 08:56:45.000000 dmk_packages-0.6.6/src/dmk_packages.egg-info/top_level.txt
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-30 07:14:08.725010 dmk_packages-0.6.7/
+-rw-r--r--   0 tommie     (501) staff       (20)    11347 2024-04-04 04:45:57.000000 dmk_packages-0.6.7/LICENSE
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-30 07:14:08.724765 dmk_packages-0.6.7/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)     1365 2024-04-04 04:45:57.000000 dmk_packages-0.6.7/README.md
+-rw-r--r--   0 tommie     (501) staff       (20)      584 2024-04-30 07:06:31.000000 dmk_packages-0.6.7/pyproject.toml
+-rw-r--r--   0 tommie     (501) staff       (20)       38 2024-04-30 07:14:08.725067 dmk_packages-0.6.7/setup.cfg
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-30 07:14:08.719097 dmk_packages-0.6.7/src/
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-30 07:14:08.720363 dmk_packages-0.6.7/src/dmk_packages/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.7/src/dmk_packages/__init__.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-30 07:14:08.723677 dmk_packages-0.6.7/src/dmk_packages/crawler/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.7/src/dmk_packages/crawler/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     3534 2024-04-30 04:52:14.000000 dmk_packages-0.6.7/src/dmk_packages/crawler/bigkinds.py
+-rw-r--r--   0 tommie     (501) staff       (20)     6580 2024-04-30 04:52:14.000000 dmk_packages-0.6.7/src/dmk_packages/crawler/clien.py
+-rw-r--r--   0 tommie     (501) staff       (20)     6631 2024-04-30 06:18:13.000000 dmk_packages-0.6.7/src/dmk_packages/crawler/fnguide.py
+-rw-r--r--   0 tommie     (501) staff       (20)     2321 2024-04-04 04:45:57.000000 dmk_packages-0.6.7/src/dmk_packages/crawler/naver_blog.py
+-rw-r--r--   0 tommie     (501) staff       (20)    15349 2024-04-04 04:45:57.000000 dmk_packages-0.6.7/src/dmk_packages/crawler/naver_search_volume.py
+-rw-r--r--   0 tommie     (501) staff       (20)     1382 2024-04-24 08:52:39.000000 dmk_packages-0.6.7/src/dmk_packages/crawler/pdf_to_text.py
+-rw-r--r--   0 tommie     (501) staff       (20)    13362 2024-04-23 05:01:14.000000 dmk_packages-0.6.7/src/dmk_packages/crawler/youtube.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-30 07:14:08.724192 dmk_packages-0.6.7/src/dmk_packages/database/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.7/src/dmk_packages/database/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     3057 2024-04-04 04:45:57.000000 dmk_packages-0.6.7/src/dmk_packages/database/database.py
+-rw-r--r--   0 tommie     (501) staff       (20)     1895 2024-04-04 04:45:57.000000 dmk_packages-0.6.7/src/dmk_packages/naver_datalab.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-04-30 07:14:08.724473 dmk_packages-0.6.7/src/dmk_packages.egg-info/
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-04-30 07:14:08.000000 dmk_packages-0.6.7/src/dmk_packages.egg-info/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)      677 2024-04-30 07:14:08.000000 dmk_packages-0.6.7/src/dmk_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 tommie     (501) staff       (20)        1 2024-04-30 07:14:08.000000 dmk_packages-0.6.7/src/dmk_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       41 2024-04-30 07:14:08.000000 dmk_packages-0.6.7/src/dmk_packages.egg-info/requires.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       13 2024-04-30 07:14:08.000000 dmk_packages-0.6.7/src/dmk_packages.egg-info/top_level.txt
```

### Comparing `dmk_packages-0.6.6/LICENSE` & `dmk_packages-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.6/PKG-INFO` & `dmk_packages-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.6
+Version: 0.6.7
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.6/README.md` & `dmk_packages-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.6/pyproject.toml` & `dmk_packages-0.6.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmk_packages"
-version = "0.6.6"
+version = "0.6.7"
 authors = [{ name = "DataMarketingKorea", email = "infra@datamarketing.co.kr" }]
 description = "Common packages for DataMKTKorea"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["SQLAlchemy", "python-dotenv", "psycopg2-binary"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `dmk_packages-0.6.6/src/dmk_packages/crawler/bigkinds.py` & `dmk_packages-0.6.7/src/dmk_packages/crawler/bigkinds.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.6/src/dmk_packages/crawler/clien.py` & `dmk_packages-0.6.7/src/dmk_packages/crawler/clien.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.6/src/dmk_packages/crawler/fnguide.py` & `dmk_packages-0.6.7/src/dmk_packages/crawler/fnguide.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import random
 import asyncio
 import pendulum
 from loguru import logger
 from playwright.async_api import (
     async_playwright,
     TimeoutError as PlaywrightTimeoutError,
 )
@@ -135,15 +136,15 @@
                             timeout=15000
                         ) as download_info:
                             pdf = await row.query_selector(".btn--get")
                             await pdf.click()
 
                         download = await download_info.value
                         await download.save_as(download_path + filename)
-                        await asyncio.sleep(0.5)
+                        await asyncio.sleep(random.uniform(1,10))
 
                 except PlaywrightTimeoutError:
                     # 오류난 파일의 url_tag 추가
                     logger.error(f"[{cat}][{regist_date}][{title}] download error")
                     self.url_e.append(url_tag)
 
                     # 다시 실행
```

### Comparing `dmk_packages-0.6.6/src/dmk_packages/crawler/naver_blog.py` & `dmk_packages-0.6.7/src/dmk_packages/crawler/naver_blog.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.6/src/dmk_packages/crawler/naver_search_volume.py` & `dmk_packages-0.6.7/src/dmk_packages/crawler/naver_search_volume.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.6/src/dmk_packages/crawler/pdf_to_text.py` & `dmk_packages-0.6.7/src/dmk_packages/crawler/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.6/src/dmk_packages/crawler/youtube.py` & `dmk_packages-0.6.7/src/dmk_packages/crawler/youtube.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.6/src/dmk_packages/database/database.py` & `dmk_packages-0.6.7/src/dmk_packages/database/database.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.6/src/dmk_packages/naver_datalab.py` & `dmk_packages-0.6.7/src/dmk_packages/naver_datalab.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.6/src/dmk_packages.egg-info/PKG-INFO` & `dmk_packages-0.6.7/src/dmk_packages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.6
+Version: 0.6.7
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.6/src/dmk_packages.egg-info/SOURCES.txt` & `dmk_packages-0.6.7/src/dmk_packages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

