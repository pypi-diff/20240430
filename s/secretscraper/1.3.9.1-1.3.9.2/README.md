# Comparing `tmp/secretscraper-1.3.9.1.tar.gz` & `tmp/secretscraper-1.3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.9.1.tar", max compression
+gzip compressed data, was "secretscraper-1.3.9.2.tar", max compression
```

## Comparing `secretscraper-1.3.9.1.tar` & `secretscraper-1.3.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9.1/LICENSE
--rw-r--r--   0        0        0     8116 2024-04-30 07:35:25.305186 secretscraper-1.3.9.1/README.md
--rw-r--r--   0        0        0     1889 2024-04-30 07:40:32.160253 secretscraper-1.3.9.1/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-30 07:40:32.163504 secretscraper-1.3.9.1/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7499 2024-04-30 07:22:49.760009 secretscraper-1.3.9.1/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9.1/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2533 2024-04-30 07:33:09.625864 secretscraper-1.3.9.1/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9.1/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    16556 2024-04-30 07:29:51.633036 secretscraper-1.3.9.1/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.9.1/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9.1/src/secretscraper/exception.py
--rw-r--r--   0        0        0    14257 2024-04-30 07:22:49.748124 secretscraper-1.3.9.1/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9.1/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6527 2024-04-29 07:58:22.528282 secretscraper-1.3.9.1/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9.1/src/secretscraper/log.py
--rw-r--r--   0        0        0     8822 2024-04-30 07:39:46.452140 secretscraper-1.3.9.1/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9.1/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9.1/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     2862 2024-04-30 06:43:03.216699 secretscraper-1.3.9.1/src/secretscraper/util.py
--rw-r--r--   0        0        0     9557 1970-01-01 00:00:00.000000 secretscraper-1.3.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9.2/LICENSE
+-rw-r--r--   0        0        0     8116 2024-04-30 07:35:25.305186 secretscraper-1.3.9.2/README.md
+-rw-r--r--   0        0        0     1910 2024-04-30 08:10:59.606747 secretscraper-1.3.9.2/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-30 07:52:30.278200 secretscraper-1.3.9.2/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7499 2024-04-30 07:22:49.760009 secretscraper-1.3.9.2/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9.2/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2533 2024-04-30 07:33:09.625864 secretscraper-1.3.9.2/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9.2/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    17214 2024-04-30 08:49:48.323754 secretscraper-1.3.9.2/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.9.2/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9.2/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    14303 2024-04-30 08:50:24.645938 secretscraper-1.3.9.2/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9.2/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6527 2024-04-29 07:58:22.528282 secretscraper-1.3.9.2/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9.2/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8822 2024-04-30 07:39:46.452140 secretscraper-1.3.9.2/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9.2/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9.2/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     2862 2024-04-30 06:43:03.216699 secretscraper-1.3.9.2/src/secretscraper/util.py
+-rw-r--r--   0        0        0     9600 1970-01-01 00:00:00.000000 secretscraper-1.3.9.2/PKG-INFO
```

### Comparing `secretscraper-1.3.9.1/LICENSE` & `secretscraper-1.3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/README.md` & `secretscraper-1.3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/pyproject.toml` & `secretscraper-1.3.9.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.9.1"
+version = "1.3.9.2"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
@@ -22,14 +22,15 @@
     { version = "^0.7.0", platform = "linux", python = "^3.10" },
     { version = "^0.7.7", platform = "linux", python = "^3.11" }
 ]
 bs4 = "^0.0.2"
 aiohttp = "^3.9.4"
 httpx = { extras = ["socks"], version = "^0.27.0" }
 tldextract = "^5.1.2"
+aiocache = "^0.12.2"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.4"
 isort = "^5.12.0"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.23.6"
 pytest-benchmark = "^4.0.0"
```

### Comparing `secretscraper-1.3.9.1/src/secretscraper/cmdline.py` & `secretscraper-1.3.9.2/src/secretscraper/cmdline.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/config/__init__.py` & `secretscraper-1.3.9.2/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/config/settings.yml` & `secretscraper-1.3.9.2/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/coroutinue.py` & `secretscraper-1.3.9.2/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/crawler.py` & `secretscraper-1.3.9.2/src/secretscraper/crawler.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 import re
 import threading
 import traceback
 import typing
 from typing import Set
 from urllib.parse import urlparse
 
+import aiocache
 import aiohttp
+import anyio
 import dynaconf
 import httpx
 from aiohttp import ClientResponse
 from httpx import AsyncClient
 
 from secretscraper.coroutinue import AsyncPoolCollector, AsyncTask
 from secretscraper.entity import URL, Secret, URLNode
 from secretscraper.filter import URLFilter
 from secretscraper.handler import Handler
 from secretscraper.urlparser import URLParser
+from aiocache.serializers import PickleSerializer
 
 from .config import settings
 from .exception import CrawlerException
 from .util import Range
 
 logger = logging.getLogger(__name__)
 
@@ -84,14 +87,17 @@
         self.headers = headers
         self.debug = debug
         if self.debug:
             logger.setLevel(logging.DEBUG)
         self.follow_redirects = follow_redirects
         self._validate = validate
 
+        self.cache = aiocache.Cache(aiocache.Cache.MEMORY)
+        self.serializer = PickleSerializer()
+
         self.visited_urls: Set[URLNode] = set()
         self.found_urls: Set[URLNode] = set()  # newly found urls
         self.working_queue: queue.Queue[URLNode] = queue.Queue()  # BP queue
         self.url_dict: typing.Dict[URLNode, typing.Set[URLNode]] = (
             dict()
         )  # url and all of its children url
         self.js_dict: typing.Dict[URLNode, typing.Set[URLNode]] = (
@@ -165,61 +171,60 @@
                 if self.max_depth <= 0 or url_node.depth <= self.max_depth:
                     task = AsyncTask(self.process_one, url_node)
                     await self.pool.submit(task)
                 logger.debug(
                     f"Total:{self.total_page}, Found:{len(self.found_urls)}, Depth:{url_node.depth}, Visited:{len(self.visited_urls)}, Secrets:{sum([len(secrets) for secrets in self.url_secrets.values()])}"
                 )
             logger.debug(f"Crawler finished.")
-            if self._validate:
-                logger.debug(f"Start validate...")
-                await self.validate()
-
         except asyncio.CancelledError:
+            # raise CrawlerException(f"Crawler cancelled.")
             pass
         except Exception as e:
             raise CrawlerException("Unexpected Exception") from e
         finally:
             await self.clean()
 
+    def start_validate(self):
+        """Start validate"""
+        if not self._validate:
+            return
+        logger.debug(f"Start validate...")
+        self._event_loop = asyncio.new_event_loop()
+        self.client = AsyncClient(verify=False, proxies=self.proxy)
+        try:
+            self._event_loop.run_until_complete(self.validate())
+        except asyncio.CancelledError:
+            pass  # ignore
+
     async def validate(self):
         """Validate the status of results that are marked as unknown"""
 
-        # counter = 0
-
         async def fetch_task(url_node: URLNode) -> None:
-            # nonlocal counter
             res = await self.fetch(url_node.url)
             logger.debug(f"Validate {url_node.url}: {res.status_code if res is not None else 'Unknown'}")
             url_node.response_status = str(res.status_code) if res is not None else url_node.response_status
-            # counter -= 1
+
+        task_list: list[asyncio.Future] = list()
 
         for base, urls in self.url_dict.items():
             if not str(base.response_status).isdigit():
-                # logger.debug(f"Start to validate {base.url}")
-                # counter += 1
-                await self.pool.submit(AsyncTask(fetch_task, base))
+                task_list.append(asyncio.create_task(fetch_task(base)))
             for url in urls:
                 if not str(url.response_status).isdigit():
-                    # logger.debug(f"Start to validate {url.url}")
-                    # counter += 1
-                    await self.pool.submit(AsyncTask(fetch_task, url))
+                    task_list.append(asyncio.create_task(fetch_task(url)))
 
         for base, urls in self.js_dict.items():
             if not str(base.response_status).isdigit():
-                await self.pool.submit(AsyncTask(fetch_task, base))
+                task_list.append(asyncio.create_task(fetch_task(base)))
 
             for url in urls:
                 if not str(url.response_status).isdigit():
-                    await self.pool.submit(AsyncTask(fetch_task, url))
-        # while counter > 0:
-        while not self.pool.is_finish:
-            # if self.pool.is_finish:
-            #     logger.exception(f"Validate abnormal finish")
-            #     break
-            await asyncio.sleep(0.01)
+                    task_list.append(asyncio.create_task(fetch_task(base)))
+        for future in asyncio.as_completed(task_list):
+            await future
 
     def is_evade(self, url: URLNode) -> bool:
         """Check whether url should be evaded"""
         if self.dangerous_paths is not None:
             path = url.url_object.path
             if len(
                 [path for p in self.dangerous_paths if re.search(f"/?{p}", path.strip(), re.IGNORECASE)]
@@ -345,18 +350,23 @@
                     self.js_dict[url_node].add(child)
                 elif self.is_append_url(child):
                     if url_node not in self.url_dict:
                         self.url_dict[url_node] = set()
                     self.url_dict[url_node].add(child)
                 logger.debug(f"New link found: {child.url} from {url_node.url}")
 
+    # @aiocache.cached(ttl=5, key="http", namespace="fetch", serializer=PickleSerializer())
     async def fetch(self, url: str) -> httpx.Response:
         """Wrapper for sending http request
         If exception occurs, return None
         """
+        cached_response = await self.cache.get(url)
+        if cached_response is not None:
+            logger.debug(f"Cache Match: {url}")
+            return self.serializer.loads(cached_response)
         logger.debug(f"Fetching {url}")
         response = None
         try:
             # response = await self.client.get(
             #     url,
             #     allow_redirects=self.follow_redirects,
             #     headers=self.headers,
@@ -367,29 +377,32 @@
             response = await self.client.get(
                 url,
                 headers=self.headers,
                 follow_redirects=self.follow_redirects,
                 timeout=self.timeout,
             )
             logger.debug(f"Fetch {url}, status: {response.status_code}")
+            await self.cache.set(url, self.serializer.dumps(response), ttl=60)
 
         except TimeoutError:
             logger.error(f"Timeout while fetching {url}")
         except httpx.ConnectError as e:
             logger.error(f"Connection error for {url}: {e}")
+        except anyio.ClosedResourceError as e:
+            logger.error(f"Closing resource for {url}: {e}")
         except httpx.InvalidURL as e:
             logger.error(f"Invalid URL for {url}: {e}")
         except httpx.TimeoutException as e:
             logger.error(f"Timeout while fetching {url} ")
         except httpx.ReadError as e:
             logger.debug(f"Read error for {url}: {e}")  # trigger when keyboard interrupt
         except KeyboardInterrupt:
             pass  # ignore
         except Exception as e:
-            logger.error(f"Unexpected error: {e.__class__} while fetching {url}")
+            logger.error(f"Unexpected error: {e.__class__}:{e} while fetching {url}")
         return response
 
     async def clean(self):
         """Close pool, cancel tasks, close http client session"""
         try:
             await self.client.aclose()
         except:
```

### Comparing `secretscraper-1.3.9.1/src/secretscraper/entity.py` & `secretscraper-1.3.9.2/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/exception.py` & `secretscraper-1.3.9.2/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/facade.py` & `secretscraper-1.3.9.2/src/secretscraper/facade.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
                 print_func_colorful(f,
                                     self.print_func,
                                     f"Target URLs: {', '.join(self.crawler.start_urls)}",
                                     bold=True,
                                     blink=True,
                                     )
                 self.crawler.start()
+                self.crawler.start_validate()
                 if self.detail_output:
                     # print_func_colorful(self.print_func,f"Total page: {self.crawler.total_page}")
                     f.write(self.formatter.output_url_hierarchy(self.crawler.url_dict, True))
 
                     if not self.hide_regex:
                         print_func_colorful(f, self.print_func,
                                             f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
```

### Comparing `secretscraper-1.3.9.1/src/secretscraper/filter.py` & `secretscraper-1.3.9.2/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/handler.py` & `secretscraper-1.3.9.2/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/log.py` & `secretscraper-1.3.9.2/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/output_formatter.py` & `secretscraper-1.3.9.2/src/secretscraper/output_formatter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/scanner.py` & `secretscraper-1.3.9.2/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/urlparser.py` & `secretscraper-1.3.9.2/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/src/secretscraper/util.py` & `secretscraper-1.3.9.2/src/secretscraper/util.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.9.1/PKG-INFO` & `secretscraper-1.3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.9.1
+Version: 1.3.9.2
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiocache (>=0.12.2,<0.13.0)
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: httpx[socks] (>=0.27.0,<0.28.0)
 Requires-Dist: hyperscan (>=0.7.0,<0.8.0) ; python_version >= "3.10" and python_version < "4.0" and sys_platform == "darwin"
 Requires-Dist: hyperscan (>=0.7.0,<0.8.0) ; python_version >= "3.10" and python_version < "4.0" and sys_platform == "linux"
```

