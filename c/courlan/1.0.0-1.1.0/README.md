# Comparing `tmp/courlan-1.0.0.tar.gz` & `tmp/courlan-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "courlan-1.0.0.tar", last modified: Thu Feb  1 14:51:52 2024, max compression
+gzip compressed data, was "courlan-1.1.0.tar", last modified: Tue Apr 30 11:17:34 2024, max compression
```

## Comparing `courlan-1.0.0.tar` & `courlan-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-02-01 14:51:52.850477 courlan-1.0.0/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1131 2020-08-31 17:20:52.000000 courlan-1.0.0/CONTRIBUTING.md
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4095 2024-02-01 14:51:33.000000 courlan-1.0.0/HISTORY.md
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    10173 2024-02-01 12:57:53.000000 courlan-1.0.0/LICENSE
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      160 2022-07-18 17:01:18.000000 courlan-1.0.0/MANIFEST.in
--rw-r--r--   0 adbar     (1000) adbar     (1000)    18619 2024-02-01 14:51:52.850477 courlan-1.0.0/PKG-INFO
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    16686 2024-02-01 14:51:33.000000 courlan-1.0.0/README.rst
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-02-01 14:51:52.846477 courlan-1.0.0/courlan/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      687 2024-02-01 14:51:33.000000 courlan-1.0.0/courlan/__init__.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     7613 2024-02-01 12:57:53.000000 courlan-1.0.0/courlan/clean.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     5673 2024-02-01 12:57:53.000000 courlan-1.0.0/courlan/cli.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     8171 2024-02-01 14:51:33.000000 courlan-1.0.0/courlan/core.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     9043 2024-02-01 12:57:53.000000 courlan-1.0.0/courlan/filters.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     7223 2023-03-07 12:06:22.000000 courlan-1.0.0/courlan/langinfo.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      360 2023-05-17 11:43:25.000000 courlan-1.0.0/courlan/meta.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1572 2024-02-01 12:57:53.000000 courlan-1.0.0/courlan/network.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2022-07-18 15:53:08.000000 courlan-1.0.0/courlan/py.typed
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     2091 2024-01-29 17:09:04.000000 courlan-1.0.0/courlan/sampling.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1692 2024-02-01 12:57:53.000000 courlan-1.0.0/courlan/settings.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    19038 2024-02-01 12:41:44.000000 courlan-1.0.0/courlan/urlstore.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     5841 2024-01-29 17:08:01.000000 courlan-1.0.0/courlan/urlutils.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-02-01 14:51:52.850477 courlan-1.0.0/courlan.egg-info/
--rw-r--r--   0 adbar     (1000) adbar     (1000)    18619 2024-02-01 14:51:52.000000 courlan-1.0.0/courlan.egg-info/PKG-INFO
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      641 2024-02-01 14:51:52.000000 courlan-1.0.0/courlan.egg-info/SOURCES.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2024-02-01 14:51:52.000000 courlan-1.0.0/courlan.egg-info/dependency_links.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       45 2024-02-01 14:51:52.000000 courlan-1.0.0/courlan.egg-info/entry_points.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-11-07 16:48:28.000000 courlan-1.0.0/courlan.egg-info/not-zip-safe
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      128 2024-02-01 14:51:52.000000 courlan-1.0.0/courlan.egg-info/requires.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        8 2024-02-01 14:51:52.000000 courlan-1.0.0/courlan.egg-info/top_level.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)   151953 2020-08-31 17:20:52.000000 courlan-1.0.0/courlan_harns-march.jpg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       40 2021-12-07 18:31:00.000000 courlan-1.0.0/pytest.ini
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       38 2024-02-01 14:51:52.850477 courlan-1.0.0/setup.cfg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     3951 2024-02-01 12:57:53.000000 courlan-1.0.0/setup.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-02-01 14:51:52.846477 courlan-1.0.0/tests/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2020-08-31 17:20:52.000000 courlan-1.0.0/tests/__init__.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-02-01 14:51:52.846477 courlan-1.0.0/tests/data/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      324 2021-12-07 18:52:06.000000 courlan-1.0.0/tests/data/input.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    44509 2024-02-01 12:57:53.000000 courlan-1.0.0/tests/unit_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    18251 2024-02-01 12:41:44.000000 courlan-1.0.0/tests/urlstore_tests.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-30 11:17:34.212750 courlan-1.1.0/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1131 2020-08-31 17:20:52.000000 courlan-1.1.0/CONTRIBUTING.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4434 2024-04-30 11:13:20.000000 courlan-1.1.0/HISTORY.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    10173 2024-02-01 12:57:53.000000 courlan-1.1.0/LICENSE
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      160 2022-07-18 17:01:18.000000 courlan-1.1.0/MANIFEST.in
+-rw-r--r--   0 adbar     (1000) adbar     (1000)    18616 2024-04-30 11:17:34.212750 courlan-1.1.0/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16686 2024-04-30 11:09:14.000000 courlan-1.1.0/README.rst
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-30 11:17:34.212750 courlan-1.1.0/courlan/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      687 2024-04-30 11:13:38.000000 courlan-1.1.0/courlan/__init__.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     6908 2024-04-26 11:42:09.000000 courlan-1.1.0/courlan/clean.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5673 2024-02-01 12:57:53.000000 courlan-1.1.0/courlan/cli.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     8171 2024-02-01 14:51:33.000000 courlan-1.1.0/courlan/core.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     8177 2024-04-26 12:14:25.000000 courlan-1.1.0/courlan/filters.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      367 2024-04-26 11:42:09.000000 courlan-1.1.0/courlan/meta.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1572 2024-02-01 12:57:53.000000 courlan-1.1.0/courlan/network.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2022-07-18 15:53:08.000000 courlan-1.1.0/courlan/py.typed
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2091 2024-04-23 14:53:23.000000 courlan-1.1.0/courlan/sampling.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1636 2024-04-26 11:42:09.000000 courlan-1.1.0/courlan/settings.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    19037 2024-04-30 10:28:32.000000 courlan-1.1.0/courlan/urlstore.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5683 2024-04-26 11:42:09.000000 courlan-1.1.0/courlan/urlutils.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-30 11:17:34.212750 courlan-1.1.0/courlan.egg-info/
+-rw-r--r--   0 adbar     (1000) adbar     (1000)    18616 2024-04-30 11:17:34.000000 courlan-1.1.0/courlan.egg-info/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      621 2024-04-30 11:17:34.000000 courlan-1.1.0/courlan.egg-info/SOURCES.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2024-04-30 11:17:34.000000 courlan-1.1.0/courlan.egg-info/dependency_links.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       45 2024-04-30 11:17:34.000000 courlan-1.1.0/courlan.egg-info/entry_points.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2024-04-30 11:17:34.000000 courlan-1.1.0/courlan.egg-info/not-zip-safe
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      125 2024-04-30 11:17:34.000000 courlan-1.1.0/courlan.egg-info/requires.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        8 2024-04-30 11:17:34.000000 courlan-1.1.0/courlan.egg-info/top_level.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   151953 2020-08-31 17:20:52.000000 courlan-1.1.0/courlan_harns-march.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       40 2021-12-07 18:31:00.000000 courlan-1.1.0/pytest.ini
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       38 2024-04-30 11:17:34.212750 courlan-1.1.0/setup.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3948 2024-04-30 11:09:14.000000 courlan-1.1.0/setup.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-30 11:17:34.212750 courlan-1.1.0/tests/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2020-08-31 17:20:52.000000 courlan-1.1.0/tests/__init__.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-30 11:17:34.212750 courlan-1.1.0/tests/data/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      324 2021-12-07 18:52:06.000000 courlan-1.1.0/tests/data/input.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    45007 2024-04-26 12:14:25.000000 courlan-1.1.0/tests/unit_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    18690 2024-04-30 10:28:32.000000 courlan-1.1.0/tests/urlstore_tests.py
```

### Comparing `courlan-1.0.0/CONTRIBUTING.md` & `courlan-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `courlan-1.0.0/HISTORY.md` & `courlan-1.1.0/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 ## History / Changelog
 
 
+### 1.1.0
+
+- replace `langcodes` by `babel` and use its information on locales (#89, #92)
+- simplified and faster code: domain extraction, cleaning, filters and UrlStore (#90, #93, #94, #95)
+- UrlStore: better url batches, replace `timelimit` parameter by `time_limit` (#91)
+- maintenance: update readme and convert it to markdown (#97)
+
+
 ### 1.0.0
 
 - license change from GPLv3+ to Apache 2.0 (#81)
 - UrlStore: `write()` method and `load_store()` function added (#83)
 - add parameter `trailing_slash` to keep of discard slashes at the end of URLs (#52)
 - maintenance: fix whitespace in `clean_url()` (#77), simplify code (#79)
```

### Comparing `courlan-1.0.0/LICENSE` & `courlan-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `courlan-1.0.0/PKG-INFO` & `courlan-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: courlan
-Version: 1.0.0
+Version: 1.1.0
 Summary: Clean, filter and sample URLs to optimize data collection – includes spam, content type and language filters.
 Home-page: https://github.com/adbar/courlan
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: Apache-2.0
 Project-URL: Blog, https://adrien.barbaresi.eu/blog/
 Project-URL: Tracker, https://github.com/adbar/courlan/issues
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: langcodes>=3.3.0
+Requires-Dist: babel>=2.11.0
 Requires-Dist: tld==0.12.6; python_version < "3.7"
 Requires-Dist: tld>=0.13; python_version >= "3.7"
 Requires-Dist: urllib3<2,>=1.26; python_version < "3.7"
 Requires-Dist: urllib3<3,>=1.26; python_version >= "3.7"
 
 coURLan: Clean, filter, normalize, and sample URLs
 ==================================================
```

### Comparing `courlan-1.0.0/README.rst` & `courlan-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `courlan-1.0.0/courlan/__init__.py` & `courlan-1.1.0/courlan/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # meta
 __title__ = "courlan"
 __author__ = "Adrien Barbaresi"
 __license__ = "Apache-2.0"
 __copyright__ = "Copyright 2020-2024, Adrien Barbaresi"
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 
 # imports
 from .clean import clean_url, normalize_url, scrub_url
 from .core import check_url, extract_links
 from .filters import (
     is_navigation_page,
```

### Comparing `courlan-1.0.0/courlan/clean.py` & `courlan-1.1.0/courlan/clean.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import re
 
 from typing import Optional, Union
 from urllib.parse import parse_qs, quote, urlencode, urlunsplit, SplitResult
 
 from .filters import is_valid_url
-from .settings import ALLOWED_PARAMS, CONTROL_PARAMS, TARGET_LANG_DE, TARGET_LANG_EN
+from .settings import ALLOWED_PARAMS, LANG_PARAMS, TARGET_LANGS
 from .urlutils import _parse
 
 
 LOGGER = logging.getLogger(__name__)
 
 # parsing
 PROTOCOLS = re.compile(r"https?://")
@@ -36,47 +36,48 @@
 # https://github.com/AdguardTeam/AdguardFilters/blob/master/TrackParamFilter/sections/general_url.txt
 # https://gitlab.com/ClearURLs/rules/-/blob/master/data.min.json
 # https://firefox.settings.services.mozilla.com/v1/buckets/main/collections/query-stripping/records
 TRACKERS_RE = re.compile(
     r"^(?:dc|fbc|gc|twc|yc|ysc)lid|"
     r"^(?:click|gbra|msclk|igsh|partner|wbra)id|"
     r"^(?:ads?|mc|ga|gs|itm|mc|mkt|ml|mtm|oly|pk|utm|vero)_|"
-    r"(?:\b|_)(?:aff|affi|affiliate|campaign|cl?id|eid|ga|gl|kwd|keyword|medium|ref|referr?er|session|source|uid|xtor)"
+    r"(?:\b|_)(?:aff|affi|affiliate|campaign|cl?id|eid|ga|gl|"
+    r"kwd|keyword|medium|ref|referr?er|session|source|uid|xtor)"
 )
 
 
 def clean_url(url: str, language: Optional[str] = None) -> Optional[str]:
     "Helper function: chained scrubbing and normalization"
     try:
         return normalize_url(scrub_url(url), False, language)
     except (AttributeError, ValueError):
         return None
 
 
 def scrub_url(url: str) -> str:
     "Strip unnecessary parts and make sure only one URL is considered"
-    # trim
-    # https://github.com/cocrawler/cocrawler/blob/main/cocrawler/urls.py
-    # remove leading and trailing white space and unescaped control chars
-    url = url.strip(
+    # remove leading/trailing space and unescaped control chars
+    # strip space in input string
+    url = "".join(url.split()).strip(
         "\x00\x01\x02\x03\x04\x05\x06\x07\x08\x09\x0a\x0b\x0c\x0d\x0e\x0f"
-        "\x10\x11\x12\x13\x14\x15\x16\x17\x18\x19\x1a\x1b\x1c\x1d\x1e\x1f \r\n"
+        "\x10\x11\x12\x13\x14\x15\x16\x17\x18\x19\x1a\x1b\x1c\x1d\x1e\x1f"
     )
-    # strip space in input string
-    url = "".join(url.split())
-    # <![CDATA[http://www.urbanlife.de/item/260-bmw-i8-hybrid-revolution-unter-den-sportwagen.html]]>
+
+    # <![CDATA[http://...]]>
     if url.startswith("<![CDATA["):
-        url = url.replace("<![CDATA[", "")  # url = re.sub(r'^<!\[CDATA\[', '', url)
-        url = url.replace("]]>", "")  # url = re.sub(r'\]\]>$', '', url)
+        url = url.replace("<![CDATA[", "").replace("]]>", "")
+
     # markup rests
     url = REMAINING_MARKUP.sub("", url)
+
     # & and &amp;
     if "&amp;" in url:
         url = url.replace("&amp;", "&")
     url = TRAILING_AMP.sub("", url)
+
     # if '"' in link:
     #    link = link.split('"')[0]
     # double/faulty URLs
     protocols = PROTOCOLS.findall(url)
     if len(protocols) > 1 and "web.archive.org" not in url:
         LOGGER.debug("double url: %s %s", len(protocols), url)
         match = SELECTION.match(url)
@@ -84,61 +85,60 @@
             url = match[1]
             LOGGER.debug("taking url: %s", url)
         else:
             match = MIDDLE_URL.match(url)
             if match and is_valid_url(match[1]):
                 url = match[1]
                 LOGGER.debug("taking url: %s", url)
+
     # too long and garbled URLs e.g. due to quotes URLs
-    # https://github.com/cocrawler/cocrawler/blob/main/cocrawler/urls.py
-    # if len(url) > 500:  # arbitrary choice
     match = TRAILING_PARTS.match(url)
     if match:
         url = match[1]
-    if len(url) > 500:
+    if len(url) > 500:  # arbitrary choice
         LOGGER.debug("invalid-looking link %s of length %d", url[:50] + "…", len(url))
 
     # trailing slashes in URLs without path or in embedded URLs
     if url.count("/") == 3 or url.count("://") > 1:
         url = url.rstrip("/")
-    # lower
-    # url = url.lower()
+
     return url
 
 
 def clean_query(
     querystring: str, strict: bool = False, language: Optional[str] = None
 ) -> str:
     "Strip unwanted query elements"
-    if querystring:
-        qdict = parse_qs(querystring)
-        newqdict = {}
-        for qelem in sorted(qdict):
-            teststr = qelem.lower()
-            # control param
-            if strict:
-                if teststr not in ALLOWED_PARAMS and teststr not in CONTROL_PARAMS:
-                    continue
-            # get rid of trackers
-            elif TRACKERS_RE.search(teststr):
+    if not querystring:
+        return ""
+
+    qdict = parse_qs(querystring)
+    newqdict = {}
+
+    for qelem in sorted(qdict):
+        teststr = qelem.lower()
+        # control param
+        if strict:
+            if teststr not in ALLOWED_PARAMS and teststr not in LANG_PARAMS:
                 continue
-            # control language
-            if language is not None and teststr in CONTROL_PARAMS:
-                found_lang = str(qdict[qelem][0])
-                if (
-                    (language == "de" and found_lang not in TARGET_LANG_DE)
-                    or (language == "en" and found_lang not in TARGET_LANG_EN)
-                    or found_lang != language
-                ):
-                    LOGGER.info("bad lang: %s %s %s", language, qelem, found_lang)
-                    raise ValueError
-            # insert
-            newqdict[qelem] = qdict[qelem]
-        return urlencode(newqdict, doseq=True)
-    return querystring
+        # get rid of trackers
+        elif TRACKERS_RE.search(teststr):
+            continue
+        # control language
+        if (
+            language in TARGET_LANGS
+            and teststr in LANG_PARAMS
+            and str(qdict[qelem][0]) not in TARGET_LANGS[language]
+        ):
+            LOGGER.debug("bad lang: %s %s", language, qelem)
+            raise ValueError
+        # insert
+        newqdict[qelem] = qdict[qelem]
+
+    return urlencode(newqdict, doseq=True)
 
 
 def decode_punycode(string: str) -> str:
     "Probe for punycode in lower-cased hostname and try to decode it."
     if "xn--" not in string:
         return string
 
@@ -204,8 +204,8 @@
         and len(newpath) > 1
         and newpath.endswith("/")
     ):
         newpath = newpath.rstrip("/")
     # fragment
     newfragment = "" if strict else normalize_fragment(parsed_url.fragment, language)
     # rebuild
-    return urlunsplit([scheme, netloc, newpath, newquery, newfragment])
+    return urlunsplit((scheme, netloc, newpath, newquery, newfragment))
```

### Comparing `courlan-1.0.0/courlan/cli.py` & `courlan-1.1.0/courlan/cli.py`

 * *Files identical despite different names*

### Comparing `courlan-1.0.0/courlan/core.py` & `courlan-1.1.0/courlan/core.py`

 * *Files identical despite different names*

### Comparing `courlan-1.0.0/courlan/filters.py` & `courlan-1.1.0/courlan/filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 Bundles functions needed to target text content and validate the input.
 """
 
 import logging
 import re
 
+from functools import lru_cache
 from ipaddress import ip_address
 from typing import Any, Optional, Tuple
 from urllib.parse import urlsplit
 
-from langcodes import Language, tag_is_valid
-
-from .langinfo import COUNTRY_CODES, LANGUAGE_CODES
+from babel import Locale, UnknownLocaleError  # type: ignore
 
 
 LOGGER = logging.getLogger(__name__)
 
 
+PROTOCOLS = {"http", "https"}
+
 # domain/host names
 IP_SET = {
     ".",
     ":",
     "0",
     "1",
     "2",
@@ -48,35 +49,35 @@
     # First 61 characters of the gTLD
     + r"+[A-Za-z0-9][A-Za-z0-9-_]{0,61}"
     # Last character of the gTLD
     + r"[A-Za-z]$",
     re.IGNORECASE,
 )
 
-UNSUITABLE_DOMAIN = re.compile(r"[0-9]+\.")
-
 # content filters
 SITE_STRUCTURE = re.compile(
     # wordpress
-    r"/(?:paged?|seite|search|suche|gall?er[a-z]{1,2}|labels|archives|uploads|modules|attachment|wp-admin|wp-content|wp-includes|wp-json|wp-themes|oembed)/|"
+    r"/(?:wp-(?:admin|content|includes|json|themes)|"
+    r"paged?|seite|search|suche|gall?er[a-z]{1,2}|labels|"
+    r"archives|uploads|modules|attachment|oembed)/|"
     # wordpress + short URL
     r"[/_-](?:tags?|schlagwort|[ck]ategor[a-z]{1,2}|[ck]at|auth?or|user)/[^/]+/?$|"
     # mixed/blogspot
-    r"[^0-9]/[0-9]+/[0-9]+/$|[^0-9]/[0-9]{4}/$|"
-    # blogspot
-    r"_archive\.html$",
+    r"[^0-9]/[0-9]+/[0-9]+/$|[^0-9]/[0-9]{4}/$",
     re.IGNORECASE,
 )
 FILE_TYPE = re.compile(
-    r"\.(atom|json|css|xml|js|jpg|jpeg|png|svg|gif|tiff|pdf|ogg|mp3|m4a|aac|avi|mp4|mov|web[mp]|flv|ico|pls|zip|tar|gz|iso|swf|woff|eot|ttf)\b|"
+    r"\.(atom|json|css|xml|js|jpg|jpeg|png|svg|gif|tiff|pdf|ogg|mp3|m4a|aac|"
+    r"avi|mp4|mov|web[mp]|flv|ico|pls|zip|tar|gz|iso|swf|woff|eot|ttf)\b|"
     r"[/-](img|jpg|png)(\b|_)",
     re.IGNORECASE,
 )  # (?=[&?])
 ADULT_AND_VIDEOS = re.compile(
-    r"[/_-](?:bild-?kontakte|fick|gangbang|incest|live-?cams?|live-?chat|porno?|sexcam|sexyeroti[ck]|swinger|x{3})\b",
+    r"[/_-](?:bild-?kontakte|fick|gangbang|incest|live-?cams?|live-?chat|"
+    r"porno?|sexcam|sexyeroti[ck]|swinger|x{3})\b",
     re.IGNORECASE,
 )
 
 # language filter
 PATH_LANG_FILTER = re.compile(
     r"(?:https?://[^/]+/)([a-z]{2})([_-][a-z]{2,3})?(?:/|$)", re.IGNORECASE
 )
@@ -129,90 +130,74 @@
     ".shtml",
     ".stm",
     ".txt",
     ".xhtml",
     ".xml",
 }
 
-# territories whitelist
-# see also: https://babel.pocoo.org/en/latest/api/languages.html
-# get_official_languages('ch')
-LANGUAGE_MAPPINGS = {
-    "de": {"at", "ch", "de", "li"},  # 'be', 'it'
-    "en": {"au", "ca", "en", "gb", "ie", "nz", "us"},
-    "fr": {"be", "ca", "ch", "fr", "tn"},  # , 'lu', ...
-}
-
 
 def basic_filter(url: str) -> bool:
-    """Filter URLs based on basic formal characteristics"""
+    "Filter URLs based on basic formal characteristics."
     return bool(url.startswith("http") and 10 <= len(url) < 500)
 
 
 def domain_filter(domain: str) -> bool:
-    "Find invalid domain/host names"
+    "Find invalid domain/host names."
     # IPv4 or IPv6
     if not set(domain).difference(IP_SET):
         try:
             ip_address(domain)
         except ValueError:
             return False
         return True
 
     # malformed domains
-    try:
-        if not VALID_DOMAIN.match(domain.encode("idna").decode("utf-8")):
+    if not VALID_DOMAIN.match(domain):
+        try:
+            if not VALID_DOMAIN.match(domain.encode("idna").decode("utf-8")):
+                return False
+        except UnicodeError:
             return False
-    except UnicodeError:
-        return False
 
     # unsuitable content
-    if UNSUITABLE_DOMAIN.match(domain) or FILE_TYPE.search(domain):
+    if domain.split(".")[0].isdigit() or FILE_TYPE.search(domain):
         return False
 
     # extensions
     extension_match = EXTENSION_REGEX.search(domain)
     return not extension_match or extension_match[0] not in WHITELISTED_EXTENSIONS
 
 
 def extension_filter(urlpath: str) -> bool:
-    """Filter based on file extension"""
+    "Filter based on file extension."
     extension_match = EXTENSION_REGEX.search(urlpath)
     return not extension_match or extension_match[0] in WHITELISTED_EXTENSIONS
 
 
+@lru_cache(maxsize=1024)
 def langcodes_score(language: str, segment: str, score: int) -> int:
-    """Use langcodes on selected URL segments and integrate
-    them into a score."""
-    # see also: https://babel.pocoo.org/en/latest/locale.html
-    # test if the code looks like a country or a language
-    if segment[:2] not in COUNTRY_CODES and segment[:2] not in LANGUAGE_CODES:
-        return score
-    # test if tag is valid (caution: private codes are)
-    if tag_is_valid(segment):
-        # try to identify language code
-        identified = Language.get(segment).language
-        # see if it matches
-        if identified is not None:
-            LOGGER.debug("langcode %s found in URL segment %s", identified, segment)
-            if identified != language:
-                score -= 1
-            else:
-                score += 1
+    "Use locale parser to assess the plausibility of the chosen URL segment."
+    delimiter = "_" if "_" in segment else "-"
+    try:
+        if Locale.parse(segment, sep=delimiter).language == language:
+            score += 1
+        else:
+            score -= 1
+    except (TypeError, UnknownLocaleError):
+        pass
     return score
 
 
 def lang_filter(
     url: str,
     language: Optional[str] = None,
     strict: bool = False,
     trailing_slash: bool = True,
 ) -> bool:
-    """Heuristics targeting internationalization and linguistic elements.
-    Based on a score."""
+    "Heuristics targeting internationalization and linguistic elements based on a score."
     # sanity check
     if language is None:
         return True
     # init score
     score = 0
     # first test: internationalization in URL path
     match = PATH_LANG_FILTER.match(url)
@@ -225,72 +210,68 @@
         if len(occurrences) == 1:
             score = langcodes_score(language, match[1], score)
         elif len(occurrences) == 2:
             for occurrence in occurrences:
                 score = langcodes_score(language, occurrence, score)
         # don't perform the test if there are too many candidates: > 2
     # second test: prepended language cues
-    if strict and language in LANGUAGE_MAPPINGS:
+    if strict:
         match = HOST_LANG_FILTER.match(url)
         if match:
             candidate = match[1].lower()
-            LOGGER.debug("candidate lang %s found in URL", candidate)
-            if candidate in LANGUAGE_MAPPINGS[language]:
+            if candidate == language:
                 score += 1
             else:
                 score -= 1
     # determine test result
     return score >= 0
 
 
 def path_filter(urlpath: str, query: str) -> bool:
-    """Filters based on URL path: index page, imprint, etc."""
+    "Filters based on URL path: index page, imprint, etc."
     if NOTCRAWLABLE.search(urlpath):
         return False
     return bool(not INDEX_PAGE_FILTER.match(urlpath) or query)
 
 
 def type_filter(url: str, strict: bool = False, with_nav: bool = False) -> bool:
     """Make sure the target URL is from a suitable type (HTML page with primarily text).
     Strict: Try to filter out other document types, spam, video and adult websites."""
     try:
-        # feeds
-        if url.endswith(("/feed", "/rss")):
+        # feeds + blogspot
+        if url.endswith(("/feed", "/rss", "_archive.html")):
             raise ValueError
         # website structure
         if SITE_STRUCTURE.search(url) and (not with_nav or not is_navigation_page(url)):
             raise ValueError
         # type (also hidden in parameters), videos, adult content
         if strict and (FILE_TYPE.search(url) or ADULT_AND_VIDEOS.search(url)):
             raise ValueError
     except ValueError:
         return False
     # default
     return True
 
 
 def validate_url(url: Optional[str]) -> Tuple[bool, Any]:
-    """Parse and validate the input"""
+    "Parse and validate the input."
     try:
         parsed_url = urlsplit(url)
     except ValueError:
         return False, None
-    if not bool(parsed_url.scheme) or parsed_url.scheme not in (
-        "http",
-        "https",
-    ):
+
+    if not bool(parsed_url.scheme) or parsed_url.scheme not in PROTOCOLS:
         return False, None
-    # fmt: off
+
     if len(parsed_url.netloc) < 5 or (
         parsed_url.netloc.startswith("www.")  # type: ignore
         and len(parsed_url.netloc) < 8
     ):
         return False, None
-    # fmt: on
-    # default
+
     return True, parsed_url
 
 
 def is_valid_url(url: Optional[str]) -> bool:
     "Determine if a given string is a valid URL."
     return validate_url(url)[0]
```

### Comparing `courlan-1.0.0/courlan/network.py` & `courlan-1.1.0/courlan/network.py`

 * *Files identical despite different names*

### Comparing `courlan-1.0.0/courlan/sampling.py` & `courlan-1.1.0/courlan/sampling.py`

 * *Files identical despite different names*

### Comparing `courlan-1.0.0/courlan/settings.py` & `courlan-1.1.0/courlan/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 General settings for package execution.
 """
 
-# https://www.alexa.com/topsites
 # https://www.alexa.com/topsites/countries/DE
 # https://www.alexa.com/topsites/countries/US
 BLACKLIST = {
     "360",
     "akamai",
     "aliexpress",
     "amzn",
@@ -97,11 +96,14 @@
     "pagenum",
     "page_id",
     "pid",
     "post",
     "postid",
     "product_id",
 }
-CONTROL_PARAMS = {"lang", "language"}
-TARGET_LANG_DE = {"de", "deutsch", "ger", "german"}
-TARGET_LANG_EN = {"en", "english", "eng"}  # 'en_US', ''
-# accepted_lang = ('en')
+
+LANG_PARAMS = {"lang", "language"}
+
+TARGET_LANGS = {
+    "de": {"de", "deutsch", "ger", "german"},
+    "en": {"en", "english", "eng"},  # 'en_US'
+}
```

### Comparing `courlan-1.0.0/courlan/urlstore.py` & `courlan-1.1.0/courlan/urlstore.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import signal
 import sys
 import zlib
 
 from collections import defaultdict, deque
 from datetime import datetime, timedelta
 from enum import Enum
+from operator import itemgetter
 from threading import Lock
 from typing import (
     Any,
     DefaultDict,
     Deque,
     Dict,
     List,
@@ -44,18 +45,18 @@
     BUSTED = 3
 
 
 class DomainEntry:
     "Class to record host-related information and URL paths."
     __slots__ = ("count", "rules", "state", "timestamp", "total", "tuples")
 
-    def __init__(self) -> None:
+    def __init__(self, state: State = State.OPEN) -> None:
         self.count: int = 0
         self.rules: Optional[RobotFileParser] = None
-        self.state: State = State.OPEN
+        self.state: State = state
         self.timestamp: Optional[Any] = None
         self.total: int = 0
         self.tuples: Deque[UrlPathTuple] = deque()
 
 
 class UrlPathTuple:
     "Class storing information for URL paths relative to a domain/host."
@@ -145,15 +146,15 @@
         if domain in self.urldict:
             if self.compressed:
                 return pickle.loads(bz2.decompress(self.urldict[domain].tuples))  # type: ignore
             return self.urldict[domain].tuples
         return deque()
 
     def _set_done(self) -> None:
-        if not self.done and all(self.is_exhausted_domain(d) for d in self.urldict):
+        if not self.done and all(v.state != State.OPEN for v in self.urldict.values()):
             with self._lock:
                 self.done = True
 
     def _store_urls(
         self,
         domain: str,
         to_right: Optional[Deque[UrlPathTuple]] = None,
@@ -227,17 +228,14 @@
             if urlpath in known_paths and (
                 switch == 1 or (switch == 2 and known_paths[urlpath])
             ):
                 del remaining_urls[url]
         # preserve input order
         return list(remaining_urls)
 
-    def _timestamp(self, domain: str) -> Optional[datetime]:
-        return self.urldict[domain].timestamp
-
     # ADDITIONS AND DELETIONS
 
     def add_urls(
         self,
         urls: Optional[List[str]] = None,
         appendleft: Optional[List[str]] = None,
         visited: bool = False,
@@ -275,16 +273,15 @@
         )
         self.add_urls(urls=links, appendleft=links_priority)
 
     def discard(self, domains: List[str]) -> None:
         "Declare domains void and prune the store."
         with self._lock:
             for d in domains:
-                self.urldict[d] = DomainEntry()
-                self.urldict[d].state = State.BUSTED
+                self.urldict[d] = DomainEntry(state=State.BUSTED)
         self._set_done()
         num = gc.collect()
         LOGGER.debug("%s objects in GC after UrlStore.discard", num)
 
     def reset(self) -> None:
         "Re-initialize the URL store."
         with self._lock:
@@ -298,25 +295,20 @@
     def get_known_domains(self) -> List[str]:
         "Return all known domains as a list."
         return list(self.urldict)
 
     def get_unvisited_domains(self) -> List[str]:
         """Find all domains for which there are unvisited URLs
         and potentially adjust done meta-information."""
-        unvisited = []
-        if not self.done:
-            unvisited = [d for d in self.urldict if not self.is_exhausted_domain(d)]
-            if not unvisited:
-                self._set_done()
-        return unvisited
+        return [d for d, v in self.urldict.items() if v.state == State.OPEN]
 
     def is_exhausted_domain(self, domain: str) -> bool:
         "Tell if all known URLs for the website have been visited."
         if domain in self.urldict:
-            return self.urldict[domain].state in (State.ALL_VISITED, State.BUSTED)
+            return self.urldict[domain].state != State.OPEN
         return False
         # raise KeyError("website not in store")
 
     def unvisited_websites_number(self) -> int:
         "Return the number of websites for which there are still URLs to visit."
         return len(self.get_unvisited_domains())
 
@@ -371,28 +363,40 @@
                     return domain + url.urlpath
         # nothing to draw from
         with self._lock:
             self.urldict[domain].state = State.ALL_VISITED
         self._set_done()
         return None
 
-    def get_download_urls(self, timelimit: int = 10) -> Optional[List[str]]:
+    def get_download_urls(
+        self,
+        time_limit: int = 10,
+        max_urls: int = 10000,
+        timelimit: Optional[int] = None,
+    ) -> Optional[List[str]]:
         """Get a list of immediately downloadable URLs according to the given
         time limit per domain."""
-        potential = self.get_unvisited_domains()
-        targets = []
-        for domain in potential:
-            timestamp = self._timestamp(domain)
+        # TODO: deprecate in later version
+        time_limit = timelimit if timelimit is not None else time_limit
+
+        urls = []
+        for website, entry in self.urldict.items():
+            if entry.state != State.OPEN:
+                continue
             if (
-                timestamp is None
-                or (datetime.now() - timestamp).total_seconds() > timelimit
+                not entry.timestamp
+                or (datetime.now() - entry.timestamp).total_seconds() > time_limit
             ):
-                targets.append(domain)
-        # get corresponding URLs and filter out None values
-        return list(filter(None, [self.get_url(domain) for domain in targets]))
+                url = self.get_url(website)
+                if url is not None:
+                    urls.append(url)
+                    if len(urls) >= max_urls:
+                        break
+        self._set_done()
+        return urls
 
     def establish_download_schedule(
         self, max_urls: int = 100, time_limit: int = 10
     ) -> List[str]:
         """Get up to the specified number of URLs along with a suitable
         backoff schedule (in seconds)."""
         # see which domains are free
@@ -417,17 +421,17 @@
                 if not url.visited:
                     urlpaths.append(url.urlpath)
                     url.visited = True
                     with self._lock:
                         self.urldict[domain].count += 1
             # determine timestamps
             now = datetime.now()
-            original_timestamp = self._timestamp(domain)
+            original_timestamp = self.urldict[domain].timestamp
             if (
-                original_timestamp is None
+                not original_timestamp
                 or (now - original_timestamp).total_seconds() > time_limit
             ):
                 schedule_secs = 0.0
             else:
                 schedule_secs = time_limit - float(
                     f"{(now - original_timestamp).total_seconds():.2f}"
                 )
@@ -436,15 +440,15 @@
                 schedule_secs += time_limit
             # calculate difference and offset last addition
             total_diff = now + timedelta(0, schedule_secs - time_limit)
             # store new info
             self._store_urls(domain, url_tuples, timestamp=total_diff)
         # sort by first tuple element (time in secs)
         self._set_done()
-        return sorted(targets, key=lambda x: x[0])  # type: ignore[arg-type]
+        return sorted(targets, key=itemgetter(1))  # type: ignore[arg-type]
 
     # CRAWLING
 
     def store_rules(self, website: str, rules: Optional[RobotFileParser]) -> None:
         "Store crawling rules for a given website."
         if self.compressed:
             rules = zlib.compress(  # type: ignore[assignment]
@@ -471,23 +475,23 @@
         # backup
         return delay or default  # type: ignore[return-value]
 
     # GENERAL INFO
 
     def get_all_counts(self) -> List[int]:
         "Return all download counts for the hosts in store."
-        return [self.urldict[d].count for d in self.urldict]
+        return [v.count for v in self.urldict.values()]
 
     def total_url_number(self) -> int:
         "Find number of all URLs in store."
-        return sum(self.urldict[d].total for d in self.urldict)
+        return sum(v.total for v in self.urldict.values())
 
     def download_threshold_reached(self, threshold: float) -> bool:
         "Find out if the download limit (in seconds) has been reached for one of the websites in store."
-        return any(self.urldict[d].count >= threshold for d in self.urldict)
+        return any(v.count >= threshold for v in self.urldict.values())
 
     def dump_urls(self) -> List[str]:
         "Return a list of all known URLs."
         urls = []
         for domain in self.urldict:
             urls.extend(self.find_known_urls(domain))
         return urls
```

### Comparing `courlan-1.0.0/courlan/urlutils.py` & `courlan-1.1.0/courlan/urlutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Functions related to URL manipulation and extraction of URL parts.
 """
 
 import re
 
-from functools import lru_cache
 from html import unescape
 from typing import Any, List, Optional, Set, Tuple, Union
 from urllib.parse import urljoin, urlsplit, urlunsplit, SplitResult
 
 from tld import get_tld
 
 
@@ -16,36 +15,33 @@
     r"(?:(?:f|ht)tp)s?://"  # protocols
     r"(?:[^/?#]{,63}\.)?"  # subdomain, www, etc.
     r"([^/?#.]{4,63}\.[^/?#]{2,63}|"  # domain and extension
     r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}|"  # IPv4
     r"[0-9a-f:]{16,})"  # IPv6
     r"(?:/|$)"  # slash or end of string
 )
-NO_EXTENSION_REGEX = re.compile(r"(^[^.]+)")
-STRIP_DOMAIN_REGEX = re.compile(r"^.+?:.*?@|(?<=\D):\d+")
+STRIP_PORT_REGEX = re.compile(r"(?<=\D):\d+")
 CLEAN_FLD_REGEX = re.compile(r"^www[0-9]*\.")
-INNER_SLASH_REGEX = re.compile(r"(.+/)+")
 FEED_WHITELIST_REGEX = re.compile(r"(?:feed(?:burner|proxy))", re.I)
 
 
-@lru_cache(maxsize=1024)
 def get_tldinfo(
     url: str, fast: bool = False
 ) -> Union[Tuple[None, None], Tuple[str, str]]:
     """Cached function to extract top-level domain info"""
     if not url or not isinstance(url, str):
         return None, None
     if fast:
         # try with regexes
         domain_match = DOMAIN_REGEX.match(url)
         if domain_match:
-            full_domain = STRIP_DOMAIN_REGEX.sub("", domain_match[1])
-            clean_match = NO_EXTENSION_REGEX.match(full_domain)
+            full_domain = STRIP_PORT_REGEX.sub("", domain_match[1].split("@")[-1])
+            clean_match = full_domain.split(".")[0]
             if clean_match:
-                return clean_match[0], full_domain
+                return clean_match, full_domain
     # fallback
     tldinfo = get_tld(url, as_object=True, fail_silently=True)
     if tldinfo is None:
         return None, None
     # this step is necessary to standardize output
     return tldinfo.domain, CLEAN_FLD_REGEX.sub("", tldinfo.fld)  # type: ignore[union-attr]
```

### Comparing `courlan-1.0.0/courlan.egg-info/PKG-INFO` & `courlan-1.1.0/courlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: courlan
-Version: 1.0.0
+Version: 1.1.0
 Summary: Clean, filter and sample URLs to optimize data collection – includes spam, content type and language filters.
 Home-page: https://github.com/adbar/courlan
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: Apache-2.0
 Project-URL: Blog, https://adrien.barbaresi.eu/blog/
 Project-URL: Tracker, https://github.com/adbar/courlan/issues
@@ -30,15 +30,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: langcodes>=3.3.0
+Requires-Dist: babel>=2.11.0
 Requires-Dist: tld==0.12.6; python_version < "3.7"
 Requires-Dist: tld>=0.13; python_version >= "3.7"
 Requires-Dist: urllib3<2,>=1.26; python_version < "3.7"
 Requires-Dist: urllib3<3,>=1.26; python_version >= "3.7"
 
 coURLan: Clean, filter, normalize, and sample URLs
 ==================================================
```

### Comparing `courlan-1.0.0/courlan.egg-info/SOURCES.txt` & `courlan-1.1.0/courlan.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 pytest.ini
 setup.py
 courlan/__init__.py
 courlan/clean.py
 courlan/cli.py
 courlan/core.py
 courlan/filters.py
-courlan/langinfo.py
 courlan/meta.py
 courlan/network.py
 courlan/py.typed
 courlan/sampling.py
 courlan/settings.py
 courlan/urlstore.py
 courlan/urlutils.py
```

### Comparing `courlan-1.0.0/courlan_harns-march.jpg` & `courlan-1.1.0/courlan_harns-march.jpg`

 * *Files identical despite different names*

### Comparing `courlan-1.0.0/setup.py` & `courlan-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         "Blog": "https://adrien.barbaresi.eu/blog/",  # /tag/courlan.html
         "Tracker": "https://github.com/adbar/courlan/issues",
     },
     # package_data={},
     include_package_data=True,
     python_requires=">=3.6",
     install_requires=[
-        "langcodes >= 3.3.0",
+        "babel >= 2.11.0",
         "tld == 0.12.6; python_version < '3.7'",
         "tld >= 0.13; python_version >= '3.7'",
         "urllib3 >= 1.26, < 2; python_version < '3.7'",
         "urllib3 >= 1.26, < 3; python_version >= '3.7'",
     ],
     # extras_require=extras,
     entry_points={
```

### Comparing `courlan-1.0.0/tests/unit_tests.py` & `courlan-1.1.0/tests/unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,23 @@
     get_host_and_path,
     get_hostinfo,
     is_navigation_page,
     is_not_crawlable,
     lang_filter,
 )
 from courlan.core import filter_links
-from courlan.filters import domain_filter, extension_filter, path_filter, type_filter
+from courlan.filters import (
+    domain_filter,
+    extension_filter,
+    langcodes_score,
+    path_filter,
+    type_filter,
+)
 from courlan.meta import clear_caches
-from courlan.urlutils import _parse, get_tldinfo, is_known_link
+from courlan.urlutils import _parse, is_known_link
 
 
 logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
 RESOURCES_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)), "data")
 
 
 def test_baseurls():
@@ -239,14 +245,17 @@
         type_filter("http://www.example.org/livecams/test.html", strict=True) is False
     )
     assert type_filter("http://www.example.org/test.html") is True
 
 
 def test_type_filter():
     assert type_filter("http://www.example.org/feed") is False
+    # wp
+    assert type_filter("http://www.example.org/wp-admin/") is False
+    assert type_filter("http://www.example.org/wp-includes/this") is False
     # straight category
     assert type_filter("http://www.example.org/category/123") is False
     assert type_filter("http://www.example.org/product-category/123") is False
     # post simply filed under a category
     assert type_filter("http://www.example.org/category/tropes/time-travel") is True
     assert (
         type_filter("http://www.example.org/test.xml?param=test", strict=True) is False
@@ -436,14 +445,21 @@
         lang_filter("http://bz.berlin1.de/kino/050513/fans.html", "de", strict=False)
         is True
     )
     assert (
         lang_filter("http://bz.berlin1.de/kino/050513/fans.html", "de", strict=True)
         is False
     )
+    assert langcodes_score("en", "en_HK", 0) == 1
+    assert langcodes_score("en", "en-HK", 0) == 1
+    assert langcodes_score("en", "en_XY", 0) == 0
+    assert langcodes_score("en", "en-XY", 0) == 0
+    assert langcodes_score("en", "de_DE", 0) == -1
+    assert langcodes_score("en", "de-DE", 0) == -1
+
     # assert lang_filter('http://www.verfassungen.de/ch/basel/verf03.htm'. 'de') is True
     # assert lang_filter('http://www.uni-stuttgart.de/hi/fnz/lehrveranst.html', 'de') is True
     # http://www.wildwechsel.de/ww/front_content.php?idcatart=177&lang=4&client=6&a=view&eintrag=100&a=view&eintrag=0&a=view&eintrag=20&a=view&eintrag=80&a=view&eintrag=20
 
 
 def test_navigation():
     assert is_navigation_page("https://test.org/") is False
@@ -1167,20 +1183,22 @@
         )
         == "http://test.net/foo.html?page=2&post=abc"
     )
 
 
 def test_meta():
     "Test package meta functions."
-    url = "https://example.net/123/abc"
-    _ = get_tldinfo(url)
-    _ = _parse(url)
-    assert get_tldinfo.cache_info().currsize > 0
+    _ = langcodes_score("en", "en_HK", 0)
+    _ = _parse("https://example.net/123/abc")
+
+    assert langcodes_score.cache_info().currsize > 0
     try:
         urlsplit_lrucache = True
         assert urlsplit.cache_info().currsize > 0
     except AttributeError:  # newer Python versions only
         urlsplit_lrucache = False
+
     clear_caches()
-    assert get_tldinfo.cache_info().currsize == 0
+
+    assert langcodes_score.cache_info().currsize == 0
     if urlsplit_lrucache:
         assert urlsplit.cache_info().currsize == 0
```

### Comparing `courlan-1.0.0/tests/urlstore_tests.py` & `courlan-1.1.0/tests/urlstore_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 from datetime import datetime
 from time import sleep
 
 import pytest
 
 from courlan import UrlStore
-from courlan.core import filter_links
 from courlan.urlstore import State, load_store
 
 
 def test_urlstore():
     "Test all functionality related to the class."
 
     # sanity checks
@@ -283,26 +282,40 @@
     assert len(my_urls.find_unvisited_urls(example_domain)) == 10009
     assert (
         my_urls.unvisited_websites_number() == len(my_urls.get_unvisited_domains()) == 2
     )
     assert my_urls.total_url_number() == 20014
 
     # get download URLs
-    downloadable_urls = my_urls.get_download_urls(timelimit=0)
+    downloadable_urls = my_urls.get_download_urls(time_limit=0, max_urls=1)
     assert (
-        len(downloadable_urls) == 2
+        len(downloadable_urls) == 1
         and downloadable_urls[0] == "https://www.example.org/1"
     )
     assert (
         datetime.now() - my_urls.urldict["https://www.example.org"].timestamp
     ).total_seconds() < 0.25
     assert my_urls.urldict["https://www.example.org"].count == 3
-    assert my_urls.urldict["https://test.org"].count == 1
-    downloadable_urls = my_urls.get_download_urls()  # limit=10
+
+    # does not work on Windows?
+    # if os.name != "nt":
+    test_urls = UrlStore()
+    test_urls.add_urls(
+        ["https://www.example.org/1", "https://test.org/1", "https://test.org/2"]
+    )
+    downloadable_urls = test_urls.get_download_urls(timelimit=0)  # legacy
+    assert (
+        len(downloadable_urls) == 2
+        and downloadable_urls[0].startswith("https://www.example.org")
+        and downloadable_urls[1].startswith("https://test.org")
+        and test_urls.urldict["https://test.org"].count == 1
+    )
+    downloadable_urls = test_urls.get_download_urls()
     assert len(downloadable_urls) == 0
+
     other_store = UrlStore()
     downloadable_urls = other_store.get_download_urls()
     assert not downloadable_urls and other_store.done is True
 
     # schedule
     schedule = other_store.establish_download_schedule()
     assert not schedule
@@ -316,22 +329,22 @@
     schedule = other_store.establish_download_schedule()
     assert len(schedule) == 3
     # reaching buffer limit
     schedule = my_urls.establish_download_schedule(max_urls=1, time_limit=1)
     assert (
         len(schedule) == 1
         and round(schedule[0][0]) == 1
-        and schedule[0][1] == "https://www.example.org/2"
+        and schedule[0][1].startswith("https://www.example.org")
     )
     schedule = my_urls.establish_download_schedule(max_urls=6, time_limit=1)
     assert len(schedule) == 6 and round(max(s[0] for s in schedule)) == 4
     assert my_urls.urldict["https://www.example.org"].count == 7
     assert (
         my_urls.urldict["https://test.org"].count
-        == 4
+        == 3
         == sum(u.visited is True for u in my_urls.urldict["https://test.org"].tuples)
     )
     assert my_urls.download_threshold_reached(8) is False
     assert my_urls.download_threshold_reached(7) is True
 
 
 def test_dbdump(capsys):
```

