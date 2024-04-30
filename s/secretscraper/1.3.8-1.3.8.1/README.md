# Comparing `tmp/secretscraper-1.3.8.tar.gz` & `tmp/secretscraper-1.3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.8.tar", max compression
+gzip compressed data, was "secretscraper-1.3.8.1.tar", max compression
```

## Comparing `secretscraper-1.3.8.tar` & `secretscraper-1.3.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.8/LICENSE
--rw-r--r--   0        0        0     7904 2024-04-29 11:46:22.977178 secretscraper-1.3.8/README.md
--rw-r--r--   0        0        0     1865 2024-04-29 11:45:35.229587 secretscraper-1.3.8/pyproject.toml
--rw-r--r--   0        0        0       43 2024-04-29 11:45:35.226567 secretscraper-1.3.8/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7415 2024-04-29 11:35:42.170573 secretscraper-1.3.8/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.8/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2506 2024-04-28 14:43:59.561661 secretscraper-1.3.8/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.8/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    13941 2024-04-29 07:58:22.443148 secretscraper-1.3.8/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.8/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.8/src/secretscraper/exception.py
--rw-r--r--   0        0        0    14069 2024-04-29 11:41:55.192819 secretscraper-1.3.8/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.8/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6527 2024-04-29 07:58:22.528282 secretscraper-1.3.8/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1893 2024-04-29 11:33:44.901874 secretscraper-1.3.8/src/secretscraper/log.py
--rw-r--r--   0        0        0     8429 2024-04-29 07:58:22.445776 secretscraper-1.3.8/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.8/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4538 2024-04-29 07:57:20.130291 secretscraper-1.3.8/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     2264 2024-04-29 08:04:46.278752 secretscraper-1.3.8/src/secretscraper/util.py
--rw-r--r--   0        0        0     9300 1970-01-01 00:00:00.000000 secretscraper-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.8.1/LICENSE
+-rw-r--r--   0        0        0     7904 2024-04-29 11:46:22.977178 secretscraper-1.3.8.1/README.md
+-rw-r--r--   0        0        0     1867 2024-04-29 11:51:48.238995 secretscraper-1.3.8.1/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-29 11:51:48.242544 secretscraper-1.3.8.1/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7415 2024-04-29 11:35:42.170573 secretscraper-1.3.8.1/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.8.1/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2505 2024-04-29 11:47:07.757622 secretscraper-1.3.8.1/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.8.1/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    13941 2024-04-29 07:58:22.443148 secretscraper-1.3.8.1/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.8.1/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.8.1/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    14069 2024-04-29 11:41:55.192819 secretscraper-1.3.8.1/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.8.1/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6527 2024-04-29 07:58:22.528282 secretscraper-1.3.8.1/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1910 2024-04-29 11:50:54.116272 secretscraper-1.3.8.1/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8429 2024-04-29 07:58:22.445776 secretscraper-1.3.8.1/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.8.1/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4538 2024-04-29 07:57:20.130291 secretscraper-1.3.8.1/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     2264 2024-04-29 08:04:46.278752 secretscraper-1.3.8.1/src/secretscraper/util.py
+-rw-r--r--   0        0        0     9302 1970-01-01 00:00:00.000000 secretscraper-1.3.8.1/PKG-INFO
```

### Comparing `secretscraper-1.3.8/LICENSE` & `secretscraper-1.3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/README.md` & `secretscraper-1.3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/pyproject.toml` & `secretscraper-1.3.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.8"
+version = "1.3.8.1"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3.8/src/secretscraper/cmdline.py` & `secretscraper-1.3.8.1/src/secretscraper/cmdline.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/config/__init__.py` & `secretscraper-1.3.8.1/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/config/settings.yml` & `secretscraper-1.3.8.1/src/secretscraper/config/settings.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 loglevel: warning
 logpath: log
 
 proxy: "" # http://127.0.0.1:7890
 max_depth: 1 # 0 for no limit
 max_page_num: 1000 # 0 for no limit
 timeout: 5
-follow_redirects: false
+follow_redirects: true
 workers_num: 1000
 headers:
   Accept: "*/*"
   Cookie: ""
   User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.87 Safari/537.36 SE 2.X MetaSr 1.0
 
 urlFind:
```

### Comparing `secretscraper-1.3.8/src/secretscraper/coroutinue.py` & `secretscraper-1.3.8.1/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/crawler.py` & `secretscraper-1.3.8.1/src/secretscraper/crawler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/entity.py` & `secretscraper-1.3.8.1/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/exception.py` & `secretscraper-1.3.8.1/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/facade.py` & `secretscraper-1.3.8.1/src/secretscraper/facade.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/filter.py` & `secretscraper-1.3.8.1/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/handler.py` & `secretscraper-1.3.8.1/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/log.py` & `secretscraper-1.3.8.1/src/secretscraper/log.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,24 +43,24 @@
             },
         },
         "handlers": {
             "console": {
                 "formatter": verbose_formatter(settings.VERBOSE),
                 "level": log_level,
                 "class": "logging.StreamHandler",
-            },
-            "file": {
-                "class": "logging.handlers.RotatingFileHandler",
-                "level": "INFO",
-                "formatter": verbose_formatter(settings.VERBOSE),
-                "filename": os.path.join(settings.LOGPATH, "all.log"),
-                "maxBytes": 1024 * 1024 * 1024 * 200,  # 200M
-                "backupCount": "5",
-                "encoding": "utf-8",
-            },
+            }
+            # "file": {
+            #     "class": "logging.handlers.RotatingFileHandler",
+            #     "level": "INFO",
+            #     "formatter": verbose_formatter(settings.VERBOSE),
+            #     "filename": os.path.join(settings.LOGPATH, "all.log"),
+            #     "maxBytes": 1024 * 1024 * 1024 * 200,  # 200M
+            #     "backupCount": "5",
+            #     "encoding": "utf-8",
+            # },
         },
         "loggers": {
             "": {"level": log_level, "handlers": ["console"]},
         },
     }
 
     dictConfig(log_config)
```

### Comparing `secretscraper-1.3.8/src/secretscraper/output_formatter.py` & `secretscraper-1.3.8.1/src/secretscraper/output_formatter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/scanner.py` & `secretscraper-1.3.8.1/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/urlparser.py` & `secretscraper-1.3.8.1/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/src/secretscraper/util.py` & `secretscraper-1.3.8.1/src/secretscraper/util.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8/PKG-INFO` & `secretscraper-1.3.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.8
+Version: 1.3.8.1
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

