# Comparing `tmp/news_fetcher-0.3.0.tar.gz` & `tmp/news_fetcher-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news_fetcher-0.3.0.tar", max compression
+gzip compressed data, was "news_fetcher-0.3.1.tar", max compression
```

## Comparing `news_fetcher-0.3.0.tar` & `news_fetcher-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2022-10-19 18:47:08.791350 news_fetcher-0.3.0/LICENSE
--rw-r--r--   0        0        0     8386 2023-11-21 05:45:31.662096 news_fetcher-0.3.0/README.md
--rw-r--r--   0        0        0      325 2022-10-19 18:47:08.755381 news_fetcher-0.3.0/news_fetcher/db.py
--rw-r--r--   0        0        0     1735 2022-10-19 18:47:08.751385 news_fetcher-0.3.0/news_fetcher/models.py
--rw-r--r--   0        0        0     3651 2022-10-19 18:47:08.759378 news_fetcher-0.3.0/news_fetcher/module.py
--rw-r--r--   0        0        0     7860 2023-11-21 05:45:31.662096 news_fetcher-0.3.0/news_fetcher/news_fetcher.py
--rw-r--r--   0        0        0    12449 2023-11-21 05:45:31.662096 news_fetcher-0.3.0/news_fetcher/prostoprosport.py
--rw-r--r--   0        0        0     8126 2023-11-21 05:45:31.666096 news_fetcher-0.3.0/news_fetcher/rss.py
--rw-r--r--   0        0        0     5140 2022-10-19 18:47:08.767371 news_fetcher-0.3.0/news_fetcher/test.py
--rw-r--r--   0        0        0     1911 2022-10-19 18:47:08.763374 news_fetcher-0.3.0/news_fetcher/utils.py
--rw-r--r--   0        0        0     1210 2023-11-21 05:45:31.666096 news_fetcher-0.3.0/news_fetcher/wikitext.py
--rw-r--r--   0        0        0     1070 2023-11-21 05:45:52.686431 news_fetcher-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9446 1970-01-01 00:00:00.000000 news_fetcher-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-10-19 18:47:08.791350 news_fetcher-0.3.1/LICENSE
+-rw-r--r--   0        0        0     8386 2023-11-21 05:45:31.662096 news_fetcher-0.3.1/README.md
+-rw-r--r--   0        0        0      325 2022-10-19 18:47:08.755381 news_fetcher-0.3.1/news_fetcher/db.py
+-rw-r--r--   0        0        0     1735 2022-10-19 18:47:08.751385 news_fetcher-0.3.1/news_fetcher/models.py
+-rw-r--r--   0        0        0     3651 2022-10-19 18:47:08.759378 news_fetcher-0.3.1/news_fetcher/module.py
+-rw-r--r--   0        0        0     7860 2023-11-21 05:45:31.662096 news_fetcher-0.3.1/news_fetcher/news_fetcher.py
+-rw-r--r--   0        0        0    12449 2023-11-21 05:45:31.662096 news_fetcher-0.3.1/news_fetcher/prostoprosport.py
+-rw-r--r--   0        0        0     8126 2023-11-21 05:45:31.666096 news_fetcher-0.3.1/news_fetcher/rss.py
+-rw-r--r--   0        0        0     5140 2022-10-19 18:47:08.767371 news_fetcher-0.3.1/news_fetcher/test.py
+-rw-r--r--   0        0        0     1911 2022-10-19 18:47:08.763374 news_fetcher-0.3.1/news_fetcher/utils.py
+-rw-r--r--   0        0        0     1210 2023-11-21 05:45:31.666096 news_fetcher-0.3.1/news_fetcher/wikitext.py
+-rw-r--r--   0        0        0     1070 2024-04-30 13:01:41.154285 news_fetcher-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     9446 1970-01-01 00:00:00.000000 news_fetcher-0.3.1/PKG-INFO
```

### Comparing `news_fetcher-0.3.0/LICENSE` & `news_fetcher-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `news_fetcher-0.3.0/README.md` & `news_fetcher-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `news_fetcher-0.3.0/news_fetcher/models.py` & `news_fetcher-0.3.1/news_fetcher/models.py`

 * *Files identical despite different names*

### Comparing `news_fetcher-0.3.0/news_fetcher/module.py` & `news_fetcher-0.3.1/news_fetcher/module.py`

 * *Files identical despite different names*

### Comparing `news_fetcher-0.3.0/news_fetcher/news_fetcher.py` & `news_fetcher-0.3.1/news_fetcher/news_fetcher.py`

 * *Files identical despite different names*

### Comparing `news_fetcher-0.3.0/news_fetcher/prostoprosport.py` & `news_fetcher-0.3.1/news_fetcher/prostoprosport.py`

 * *Files identical despite different names*

### Comparing `news_fetcher-0.3.0/news_fetcher/rss.py` & `news_fetcher-0.3.1/news_fetcher/rss.py`

 * *Files identical despite different names*

### Comparing `news_fetcher-0.3.0/news_fetcher/test.py` & `news_fetcher-0.3.1/news_fetcher/test.py`

 * *Files identical despite different names*

### Comparing `news_fetcher-0.3.0/news_fetcher/utils.py` & `news_fetcher-0.3.1/news_fetcher/utils.py`

 * *Files identical despite different names*

### Comparing `news_fetcher-0.3.0/news_fetcher/wikitext.py` & `news_fetcher-0.3.1/news_fetcher/wikitext.py`

 * *Files identical despite different names*

### Comparing `news_fetcher-0.3.0/pyproject.toml` & `news_fetcher-0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "news_fetcher"
-version = "0.3.0"
+version = "0.3.1"
 description = "Script to fetch news using API and convert to wiki-text"
 authors = ["Artiom Khandamirov <t9max@yandex.ru>"]
 license = "MIT"
 repository = "https://github.com/ArtUshak/prostoprosport_news_fetcher/"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `news_fetcher-0.3.0/PKG-INFO` & `news_fetcher-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news_fetcher
-Version: 0.3.0
+Version: 0.3.1
 Summary: Script to fetch news using API and convert to wiki-text
 Home-page: https://github.com/ArtUshak/prostoprosport_news_fetcher/
 License: MIT
 Author: Artiom Khandamirov
 Author-email: t9max@yandex.ru
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

