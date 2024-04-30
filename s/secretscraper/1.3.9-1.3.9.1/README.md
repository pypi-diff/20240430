# Comparing `tmp/secretscraper-1.3.9.tar.gz` & `tmp/secretscraper-1.3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.9.tar", max compression
+gzip compressed data, was "secretscraper-1.3.9.1.tar", max compression
```

## Comparing `secretscraper-1.3.9.tar` & `secretscraper-1.3.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9/LICENSE
--rw-r--r--   0        0        0     8116 2024-04-30 07:35:25.305186 secretscraper-1.3.9/README.md
--rw-r--r--   0        0        0     1887 2024-04-30 07:36:14.477936 secretscraper-1.3.9/pyproject.toml
--rw-r--r--   0        0        0       43 2024-04-30 07:36:14.480840 secretscraper-1.3.9/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7499 2024-04-30 07:22:49.760009 secretscraper-1.3.9/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2533 2024-04-30 07:33:09.625864 secretscraper-1.3.9/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    16556 2024-04-30 07:29:51.633036 secretscraper-1.3.9/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.9/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9/src/secretscraper/exception.py
--rw-r--r--   0        0        0    14257 2024-04-30 07:22:49.748124 secretscraper-1.3.9/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6527 2024-04-29 07:58:22.528282 secretscraper-1.3.9/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9/src/secretscraper/log.py
--rw-r--r--   0        0        0     8786 2024-04-30 06:58:22.947099 secretscraper-1.3.9/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     2862 2024-04-30 06:43:03.216699 secretscraper-1.3.9/src/secretscraper/util.py
--rw-r--r--   0        0        0     9555 1970-01-01 00:00:00.000000 secretscraper-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9.1/LICENSE
+-rw-r--r--   0        0        0     8116 2024-04-30 07:35:25.305186 secretscraper-1.3.9.1/README.md
+-rw-r--r--   0        0        0     1889 2024-04-30 07:40:32.160253 secretscraper-1.3.9.1/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-30 07:40:32.163504 secretscraper-1.3.9.1/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7499 2024-04-30 07:22:49.760009 secretscraper-1.3.9.1/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9.1/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2533 2024-04-30 07:33:09.625864 secretscraper-1.3.9.1/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9.1/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    16556 2024-04-30 07:29:51.633036 secretscraper-1.3.9.1/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.9.1/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9.1/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    14257 2024-04-30 07:22:49.748124 secretscraper-1.3.9.1/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9.1/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6527 2024-04-29 07:58:22.528282 secretscraper-1.3.9.1/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9.1/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8822 2024-04-30 07:39:46.452140 secretscraper-1.3.9.1/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9.1/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9.1/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     2862 2024-04-30 06:43:03.216699 secretscraper-1.3.9.1/src/secretscraper/util.py
+-rw-r--r--   0        0        0     9557 1970-01-01 00:00:00.000000 secretscraper-1.3.9.1/PKG-INFO
```

### Comparing `secretscraper-1.3.9/LICENSE` & `secretscraper-1.3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/README.md` & `secretscraper-1.3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/pyproject.toml` & `secretscraper-1.3.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.9"
+version = "1.3.9.1"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3.9/src/secretscraper/cmdline.py` & `secretscraper-1.3.9.1/src/secretscraper/cmdline.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/config/__init__.py` & `secretscraper-1.3.9.1/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/config/settings.yml` & `secretscraper-1.3.9.1/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/coroutinue.py` & `secretscraper-1.3.9.1/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/crawler.py` & `secretscraper-1.3.9.1/src/secretscraper/crawler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/entity.py` & `secretscraper-1.3.9.1/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/exception.py` & `secretscraper-1.3.9.1/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/facade.py` & `secretscraper-1.3.9.1/src/secretscraper/facade.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/filter.py` & `secretscraper-1.3.9.1/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/handler.py` & `secretscraper-1.3.9.1/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/log.py` & `secretscraper-1.3.9.1/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/output_formatter.py` & `secretscraper-1.3.9.1/src/secretscraper/output_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,16 +136,17 @@
                 domain = get_root_domain(domain)
                 if domain not in root_domains:
                     domain = "Other"
                 if domain not in domain_secrets:
                     domain_secrets[domain] = list()
                 domain_secrets[domain].append(url)
         keys = list(domain_secrets.keys())
-        keys.remove("Other")
-        keys.append("Other")
+        if "Other" in keys:
+            keys.remove("Other")
+            keys.append("Other")
         for domain in keys:
             urls = domain_secrets[domain]
             if urls is None or len(urls) == 0:
                 continue
             url_set = {
                 self.format_normal_result(f"{str(url.url)}")
                 + " ["
```

### Comparing `secretscraper-1.3.9/src/secretscraper/scanner.py` & `secretscraper-1.3.9.1/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/urlparser.py` & `secretscraper-1.3.9.1/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/src/secretscraper/util.py` & `secretscraper-1.3.9.1/src/secretscraper/util.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9/PKG-INFO` & `secretscraper-1.3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.9
+Version: 1.3.9.1
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```
