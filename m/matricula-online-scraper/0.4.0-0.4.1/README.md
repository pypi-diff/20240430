# Comparing `tmp/matricula_online_scraper-0.4.0.tar.gz` & `tmp/matricula_online_scraper-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matricula_online_scraper-0.4.0.tar", max compression
+gzip compressed data, was "matricula_online_scraper-0.4.1.tar", max compression
```

## Comparing `matricula_online_scraper-0.4.0.tar` & `matricula_online_scraper-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/LICENSE
--rw-r--r--   0        0        0     2337 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/README.md
--rw-r--r--   0        0        0        0 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/matricula_online_scraper/__init__.py
--rw-r--r--   0        0        0       65 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/matricula_online_scraper/__main__.py
--rw-r--r--   0        0        0        0 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/matricula_online_scraper/cli/__init__.py
--rw-r--r--   0        0        0     2065 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/matricula_online_scraper/cli/common.py
--rw-r--r--   0        0        0     6132 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/matricula_online_scraper/cli/fetch.py
--rw-r--r--   0        0        0      707 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/matricula_online_scraper/cli/utils.py
--rwxr-xr-x   0        0        0     1123 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/matricula_online_scraper/main.py
--rw-r--r--   0        0        0        0 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/matricula_online_scraper/spiders/__init__.py
--rw-r--r--   0        0        0     4236 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/matricula_online_scraper/spiders/locations_spider.py
--rw-r--r--   0        0        0     4000 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/matricula_online_scraper/spiders/parish_registers_spider.py
--rw-r--r--   0        0        0      746 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/matricula_online_scraper/spiders/utils.py
--rw-r--r--   0        0        0      856 2024-04-29 05:57:38.367645 matricula_online_scraper-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3157 1970-01-01 00:00:00.000000 matricula_online_scraper-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2337 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/matricula_online_scraper/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/matricula_online_scraper/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/matricula_online_scraper/cli/__init__.py
+-rw-r--r--   0        0        0     2065 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/matricula_online_scraper/cli/common.py
+-rw-r--r--   0        0        0     6132 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/matricula_online_scraper/cli/fetch.py
+-rw-r--r--   0        0        0      707 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/matricula_online_scraper/cli/utils.py
+-rwxr-xr-x   0        0        0     1123 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/matricula_online_scraper/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/matricula_online_scraper/spiders/__init__.py
+-rw-r--r--   0        0        0     4422 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/matricula_online_scraper/spiders/locations_spider.py
+-rw-r--r--   0        0        0     4000 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/matricula_online_scraper/spiders/parish_registers_spider.py
+-rw-r--r--   0        0        0      746 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/matricula_online_scraper/spiders/utils.py
+-rw-r--r--   0        0        0      856 2024-04-30 06:32:42.435947 matricula_online_scraper-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3157 1970-01-01 00:00:00.000000 matricula_online_scraper-0.4.1/PKG-INFO
```

### Comparing `matricula_online_scraper-0.4.0/LICENSE` & `matricula_online_scraper-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.4.0/README.md` & `matricula_online_scraper-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.4.0/matricula_online_scraper/cli/common.py` & `matricula_online_scraper-0.4.1/matricula_online_scraper/cli/common.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.4.0/matricula_online_scraper/cli/fetch.py` & `matricula_online_scraper-0.4.1/matricula_online_scraper/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.4.0/matricula_online_scraper/cli/utils.py` & `matricula_online_scraper-0.4.1/matricula_online_scraper/cli/utils.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.4.0/matricula_online_scraper/main.py` & `matricula_online_scraper-0.4.1/matricula_online_scraper/main.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.4.0/matricula_online_scraper/spiders/locations_spider.py` & `matricula_online_scraper-0.4.1/matricula_online_scraper/spiders/locations_spider.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,16 +75,20 @@
             # extract the location information
             country_region_str = location.css(
                 "a.list-group-item span.text-muted::text"
             ).get()
             # and split into country and region
             country, region = [item.strip() for item in country_region_str.split("•")]
             url = urljoin(HOST, location.css("a.list-group-item::attr('href')").get())
-            # BUG: if 'place' is used, the text might be highlighted and <mark> inside
-            name = location.css("a.list-group-item span.text-primary::text").get()
+            # If search parameters like 'place' are used, the DOM is changed and a <mark>
+            # is inserted to highlight text. This gets all text from childnodes and joins them.
+            name_parts = location.css(
+                "a.list-group-item span.text-primary ::text"
+            ).getall()
+            name = "".join(name_parts).strip()
 
             export = {
                 "country": country,
                 "region": region,
                 "name": name,
                 "url": url,
             }
```

### Comparing `matricula_online_scraper-0.4.0/matricula_online_scraper/spiders/parish_registers_spider.py` & `matricula_online_scraper-0.4.1/matricula_online_scraper/spiders/parish_registers_spider.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.4.0/matricula_online_scraper/spiders/utils.py` & `matricula_online_scraper-0.4.1/matricula_online_scraper/spiders/utils.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.4.0/pyproject.toml` & `matricula_online_scraper-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "matricula-online-scraper"
-version = "0.4.0"
+version = "0.4.1"
 description = "Command Line Interface tool for scraping Matricula Online https://data.matricula-online.eu."
 repository = "https://github.com/lsg551/matricula-online-scraper"
 authors = ["Luis Schulte"]
 license = "MIT"
 readme = "README.md"
 keywords = ["matricula-online", "matricula", "scraper", "parish-registers"]
 classifiers = [
```

### Comparing `matricula_online_scraper-0.4.0/PKG-INFO` & `matricula_online_scraper-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matricula-online-scraper
-Version: 0.4.0
+Version: 0.4.1
 Summary: Command Line Interface tool for scraping Matricula Online https://data.matricula-online.eu.
 Home-page: https://github.com/lsg551/matricula-online-scraper
 License: MIT
 Keywords: matricula-online,matricula,scraper,parish-registers
 Author: Luis Schulte
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 3 - Alpha
```

