# Comparing `tmp/secretscraper-1.3.8.1.tar.gz` & `tmp/secretscraper-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.8.1.tar", max compression
+gzip compressed data, was "secretscraper-1.3.9.tar", max compression
```

## Comparing `secretscraper-1.3.8.1.tar` & `secretscraper-1.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.8.1/LICENSE
--rw-r--r--   0        0        0     7904 2024-04-29 11:46:22.977178 secretscraper-1.3.8.1/README.md
--rw-r--r--   0        0        0     1867 2024-04-29 11:51:48.238995 secretscraper-1.3.8.1/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-29 11:51:48.242544 secretscraper-1.3.8.1/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7415 2024-04-29 11:35:42.170573 secretscraper-1.3.8.1/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.8.1/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2505 2024-04-29 11:47:07.757622 secretscraper-1.3.8.1/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.8.1/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    13941 2024-04-29 07:58:22.443148 secretscraper-1.3.8.1/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.8.1/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.8.1/src/secretscraper/exception.py
--rw-r--r--   0        0        0    14069 2024-04-29 11:41:55.192819 secretscraper-1.3.8.1/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.8.1/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6527 2024-04-29 07:58:22.528282 secretscraper-1.3.8.1/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1910 2024-04-29 11:50:54.116272 secretscraper-1.3.8.1/src/secretscraper/log.py
--rw-r--r--   0        0        0     8429 2024-04-29 07:58:22.445776 secretscraper-1.3.8.1/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.8.1/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4538 2024-04-29 07:57:20.130291 secretscraper-1.3.8.1/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     2264 2024-04-29 08:04:46.278752 secretscraper-1.3.8.1/src/secretscraper/util.py
--rw-r--r--   0        0        0     9302 1970-01-01 00:00:00.000000 secretscraper-1.3.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.9/LICENSE
+-rw-r--r--   0        0        0     8116 2024-04-30 07:35:25.305186 secretscraper-1.3.9/README.md
+-rw-r--r--   0        0        0     1887 2024-04-30 07:36:14.477936 secretscraper-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-04-30 07:36:14.480840 secretscraper-1.3.9/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7499 2024-04-30 07:22:49.760009 secretscraper-1.3.9/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.9/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2533 2024-04-30 07:33:09.625864 secretscraper-1.3.9/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.9/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    16556 2024-04-30 07:29:51.633036 secretscraper-1.3.9/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.9/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.9/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    14257 2024-04-30 07:22:49.748124 secretscraper-1.3.9/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.9/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6527 2024-04-29 07:58:22.528282 secretscraper-1.3.9/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1910 2024-04-30 07:31:20.191193 secretscraper-1.3.9/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8786 2024-04-30 06:58:22.947099 secretscraper-1.3.9/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.9/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4596 2024-04-30 03:29:52.175016 secretscraper-1.3.9/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     2862 2024-04-30 06:43:03.216699 secretscraper-1.3.9/src/secretscraper/util.py
+-rw-r--r--   0        0        0     9555 1970-01-01 00:00:00.000000 secretscraper-1.3.9/PKG-INFO
```

### Comparing `secretscraper-1.3.8.1/LICENSE` & `secretscraper-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8.1/README.md` & `secretscraper-1.3.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -197,24 +197,31 @@
 ```
 
 ---
 
 # TODO
 - [ ] Support headless browser
 - [ ] Add regex doc reference
+- [ ] Fuzz path that are 404
+- [x] Separate subdomains in the result
+- [x] Optimize url collector
+[//]: # (- [ ] Employ jsbeautifier)
 - [x] Generate configuration file
 - [x] Detect dangerous paths and avoid requesting them
 - [x] Support url-finder output format, add `--detail` option
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.4.29 Version 1.3.9
+- Add `--validate` option
+- Optimize url collector
 ## 2024.4.29 Version 1.3.8
 - Optimize log output
 - Optimize the performance of `--debug` option
 ## 2024.4.29 Version 1.3.7
 - Test on multiple python versions
 - Support python 3.9~3.11
 ## 2024.4.29 Version 1.3.6
```

### Comparing `secretscraper-1.3.8.1/pyproject.toml` & `secretscraper-1.3.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.8.1"
+version = "1.3.9"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
@@ -21,14 +21,15 @@
 #    { version = "^0.7.0", platform = "linux", python = "^3.9" },
     { version = "^0.7.0", platform = "linux", python = "^3.10" },
     { version = "^0.7.7", platform = "linux", python = "^3.11" }
 ]
 bs4 = "^0.0.2"
 aiohttp = "^3.9.4"
 httpx = { extras = ["socks"], version = "^0.27.0" }
+tldextract = "^5.1.2"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.4"
 isort = "^5.12.0"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.23.6"
 pytest-benchmark = "^4.0.0"
```

### Comparing `secretscraper-1.3.8.1/src/secretscraper/cmdline.py` & `secretscraper-1.3.9/src/secretscraper/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     type=click.STRING,
 )
 @click.option("-H", "--hide-regex", help="Hide regex search result", is_flag=True)
 @click.option("-F", "--follow-redirects", help="Follow redirects", is_flag=True,
               type=click.BOOL)
 @click.option("-u", "--url", help="Target url", type=click.STRING)
 @click.option("--detail", help="Show detailed result", is_flag=True)
+@click.option("--validate", help="Validate the status of found urls", is_flag=True)
 @click.option("-l", "--local", help="Local file or directory, scan local file/directory recursively ",
               type=click.Path(exists=True, file_okay=True, dir_okay=True, path_type=pathlib.Path))
 def main(**options):
     """Main commands"""
     if options["version"]:
         click.echo(__version__)
         exit(0)
```

### Comparing `secretscraper-1.3.8.1/src/secretscraper/config/__init__.py` & `secretscraper-1.3.9/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8.1/src/secretscraper/config/settings.yml` & `secretscraper-1.3.9/src/secretscraper/config/settings.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 verbose: false
 debug: false
-loglevel: warning
+loglevel: critical
 logpath: log
 
 proxy: "" # http://127.0.0.1:7890
 max_depth: 1 # 0 for no limit
 max_page_num: 1000 # 0 for no limit
 timeout: 5
 follow_redirects: true
 workers_num: 1000
 headers:
   Accept: "*/*"
   Cookie: ""
   User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.87 Safari/537.36 SE 2.X MetaSr 1.0
 
 urlFind:
-  - '["''‘“`]\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
-  - =\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
-  - '["''‘“`]\s{0,6}([#,.]{0,2}/[-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100}?)\s{0,6}["''‘“`]'
-  - '"([-a-zA-Z0-9()@:%_\+.~#?&//={}]+?[/]{1}[-a-zA-Z0-9()@:%_\+.~#?&//={}]+?)"'
-  - href\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})|action\s{0,6}=\s{0,6}["'‘“`]{0,1}\s{0,6}([-a-zA-Z0-9()@:%_\+.~#?&//={}]{2,100})
+  - "[\"'‘“`]\\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250}?)\\s{0,6}[\"'‘“`]"
+  - "=\\s{0,6}(https{0,1}:[-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250})"
+  - "[\"'‘“`]\\s{0,6}([#,.]{0,2}/[-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250}?)\\s{0,6}[\"'‘“`]"
+  - "\"([-a-zA-Z0-9()@:%_\\+.~#?&//={}]+?[/]{1}[-a-zA-Z0-9()@:%_\\+.~#?&//={}]+?)\""
+  - "href\\s{0,6}=\\s{0,6}[\"'‘“`]{0,1}\\s{0,6}([-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250})|action\\s{0,6}=\\s{0,6}[\"'‘“`]{0,1}\\s{0,6}([-a-zA-Z0-9()@:%_\\+.~#?&//={}]{2,250})"
 jsFind:
   - (https{0,1}:[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
   - '["''‘“`]\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)'
   - =\s{0,6}[",',’,”]{0,1}\s{0,6}(/{0,1}[-a-zA-Z0-9（）@:%_\+.~#?&//=]{2,100}?[-a-zA-Z0-9（）@:%_\+.~#?&//=]{3}[.]js)
+
 dangerousPath:
   - logout
   - update
   - remove
   - insert
   - delete
```

### Comparing `secretscraper-1.3.8.1/src/secretscraper/coroutinue.py` & `secretscraper-1.3.9/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8.1/src/secretscraper/crawler.py` & `secretscraper-1.3.9/src/secretscraper/crawler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """The facade interfaces to integrate crawler, filter, and handler"""
 
 import asyncio
+import functools
 import logging
 import queue
 import re
 import threading
 import traceback
 import typing
 from typing import Set
@@ -46,14 +47,15 @@
         proxy: str = None,
         headers: dict = None,
         verbose: bool = False,
         timeout: float = 5,
         debug: bool = False,
         follow_redirects: bool = False,
         dangerous_paths: typing.List[str] = None,
+        validate: bool = False
     ):
         """
 
         :param start_urls: urls to start crawl from
         # :param client: aiohttp client
         :param url_filter: determine whether a url should be crawled
         :param parser: extract child url nodes from html
@@ -80,14 +82,15 @@
         self.verbose = verbose
         self.timeout = timeout
         self.headers = headers
         self.debug = debug
         if self.debug:
             logger.setLevel(logging.DEBUG)
         self.follow_redirects = follow_redirects
+        self._validate = validate
 
         self.visited_urls: Set[URLNode] = set()
         self.found_urls: Set[URLNode] = set()  # newly found urls
         self.working_queue: queue.Queue[URLNode] = queue.Queue()  # BP queue
         self.url_dict: typing.Dict[URLNode, typing.Set[URLNode]] = (
             dict()
         )  # url and all of its children url
@@ -161,28 +164,69 @@
                     continue
                 if self.max_depth <= 0 or url_node.depth <= self.max_depth:
                     task = AsyncTask(self.process_one, url_node)
                     await self.pool.submit(task)
                 logger.debug(
                     f"Total:{self.total_page}, Found:{len(self.found_urls)}, Depth:{url_node.depth}, Visited:{len(self.visited_urls)}, Secrets:{sum([len(secrets) for secrets in self.url_secrets.values()])}"
                 )
-            logger.debug(f"Crawler finished")
+            logger.debug(f"Crawler finished.")
+            if self._validate:
+                logger.debug(f"Start validate...")
+                await self.validate()
+
         except asyncio.CancelledError:
             pass
         except Exception as e:
             raise CrawlerException("Unexpected Exception") from e
         finally:
             await self.clean()
 
+    async def validate(self):
+        """Validate the status of results that are marked as unknown"""
+
+        # counter = 0
+
+        async def fetch_task(url_node: URLNode) -> None:
+            # nonlocal counter
+            res = await self.fetch(url_node.url)
+            logger.debug(f"Validate {url_node.url}: {res.status_code if res is not None else 'Unknown'}")
+            url_node.response_status = str(res.status_code) if res is not None else url_node.response_status
+            # counter -= 1
+
+        for base, urls in self.url_dict.items():
+            if not str(base.response_status).isdigit():
+                # logger.debug(f"Start to validate {base.url}")
+                # counter += 1
+                await self.pool.submit(AsyncTask(fetch_task, base))
+            for url in urls:
+                if not str(url.response_status).isdigit():
+                    # logger.debug(f"Start to validate {url.url}")
+                    # counter += 1
+                    await self.pool.submit(AsyncTask(fetch_task, url))
+
+        for base, urls in self.js_dict.items():
+            if not str(base.response_status).isdigit():
+                await self.pool.submit(AsyncTask(fetch_task, base))
+
+            for url in urls:
+                if not str(url.response_status).isdigit():
+                    await self.pool.submit(AsyncTask(fetch_task, url))
+        # while counter > 0:
+        while not self.pool.is_finish:
+            # if self.pool.is_finish:
+            #     logger.exception(f"Validate abnormal finish")
+            #     break
+            await asyncio.sleep(0.01)
+
     def is_evade(self, url: URLNode) -> bool:
         """Check whether url should be evaded"""
         if self.dangerous_paths is not None:
             path = url.url_object.path
             if len(
-                [path for p in self.dangerous_paths if re.search(f"{p}", path.strip(), re.IGNORECASE)]
+                [path for p in self.dangerous_paths if re.search(f"/?{p}", path.strip(), re.IGNORECASE)]
             ) > 0:
                 return True
         return False
 
     async def process_one(self, url_node: URLNode):
         """Fetch, extract url children and execute handler on result"""
         if self.max_page_num > 0 and self.total_page >= self.max_page_num:
@@ -220,21 +264,16 @@
         logger.debug(f"Extracting secret from {url_node.url}")
 
         secrets = self.handler.handle(response_text)
         if secrets is not None:
             self.url_secrets[url_node] = set(secrets)
         logger.debug(f"Extract secret of number {len(list(secrets))} from {url_node}")
 
-    async def extract_links_and_extend(
-        self, url_node: URLNode, response: httpx.Response, response_text: str
-    ):
-        """Extract links from response and extend the task queue in demand
-        This function only works if the response is text-like, but regardless of whether it is html or not.
-        Extract and extend `url_node` only if `response` is text-like.
-        """
+    def is_extend(self, response: httpx.Response) -> bool:
+        """Determine if extract links from a url node"""
         is_text_like = False
         is_html = False
         try:
             content_type = response.headers['content-type']
         except KeyError:
             content_type = ""
         if content_type.startswith("text"):
@@ -245,48 +284,72 @@
             if content_type.endswith(
                 "octet-stream"
             ) or content_type.endswith("pdf"):
                 is_text_like = False
             else:
                 is_text_like = True
 
-        if not is_text_like or not is_html:  # or not is_html just process html
-            return
-        if response.status_code != 200:  # just process normal response
+        # if not is_text_like or not is_html:  # or not is_html just process html TODO: whether extend or not
+        #     return False
+        # if response.status_code != 200:  # just process normal response
+        #     return False
+        return True
+
+    def is_append_js(self, url_node: URLNode) -> bool:
+        """Determine whether append url to js result or not"""
+        if url_node.url_object.path.endswith(".js") or url_node.url_object.path.endswith(
+            ".js.map") or url_node.url_object.path.__contains__(".js?"):
+            return True
+        return False
+
+    def is_append_url(self, url_node: URLNode) -> bool:
+        """Determine whether append url to url result or not"""
+        return True
+
+    async def extract_links_and_extend(
+        self, url_node: URLNode, response: httpx.Response, response_text: str
+    ):
+        """Extract links from response and extend the task queue in demand
+        This function only works if the response is text-like, but regardless of whether it is html or not.
+        Extract and extend `url_node` only if `response` is text-like.
+        """
+        if not self.is_extend(response):
             return
 
         if self.max_depth <= 0 or url_node.depth + 1 <= self.max_depth:
             # avoid enqueue urls with excessive depth
             # for non-html response, just record, no visit
             is_extending = True
         else:
             is_extending = False
 
         logger.debug(f"Extracting links from {url_node.url}")
         url_children: typing.Set[URLNode] = self.parser.extract_urls(url_node, response_text)
-        if len(url_children) > 0:
-            self.url_dict[url_node] = set()
-        elif is_html and (
-            url_node not in self.url_dict.keys() or self.url_dict[url_node] is None
-        ):
-            self.url_dict[url_node] = set()
+        # self.url_dict[url_node] = set()
+
+        # if len(url_children) > 0:
+        #     self.url_dict[url_node] = set()
+        # elif is_html and (
+        #     url_node not in self.url_dict.keys() or self.url_dict[url_node] is None
+        # ):
+        #     self.url_dict[url_node] = set()
 
         for child in url_children:
             if child is not None and child not in self.visited_urls:
                 self.found_urls.add(child)
                 if is_extending and self.filter.doFilter(child.url_object):
                     self.working_queue.put(child)
                     self.visited_urls.add(child)
-                if child.url_object.path.endswith(
-                    ".js"
-                ) or child.url_object.path.endswith(".js.map"):
+                if self.is_append_js(child):
                     if url_node not in self.js_dict:
                         self.js_dict[url_node] = set()
                     self.js_dict[url_node].add(child)
-                else:
+                elif self.is_append_url(child):
+                    if url_node not in self.url_dict:
+                        self.url_dict[url_node] = set()
                     self.url_dict[url_node].add(child)
                 logger.debug(f"New link found: {child.url} from {url_node.url}")
 
     async def fetch(self, url: str) -> httpx.Response:
         """Wrapper for sending http request
         If exception occurs, return None
         """
```

### Comparing `secretscraper-1.3.8.1/src/secretscraper/entity.py` & `secretscraper-1.3.9/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8.1/src/secretscraper/exception.py` & `secretscraper-1.3.9/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8.1/src/secretscraper/facade.py` & `secretscraper-1.3.9/src/secretscraper/facade.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,19 @@
             except Exception as e:
                 self.print_func(f"Unexpected error: {e}.\nExiting...")
                 self.crawler.close_all()
                 # raise FacadeException from e
 
     def create_crawler(self) -> Crawler:
         """Create a Crawler"""
+        # No validate
+        if self.custom_settings.get("validate", False) is True:
+            validate = True
+        else:
+            validate = False
         # Follow redirects
         if self.custom_settings.get("follow_redirects", False) is True:
             self.settings["follow_redirects"] = True
         # Hide regex output
         if self.custom_settings.get("hide_regex", False) is True:
             self.hide_regex = True
         # Get url filter
@@ -282,15 +287,16 @@
             num_workers=self.settings.get("workers_num"),
             proxy=self.settings.get("proxy"),
             headers=headers,
             verbose=self.settings.get("verbose"),
             timeout=self.settings.get("timeout"),
             debug=self.debug,
             follow_redirects=self.settings["follow_redirects"],
-            dangerous_paths=dangerous_paths
+            dangerous_paths=dangerous_paths,
+            validate=validate
         )
         return crawler
 
 
 class FileScannerFacade:
     """Facade for local file scanner"""
```

### Comparing `secretscraper-1.3.8.1/src/secretscraper/filter.py` & `secretscraper-1.3.9/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8.1/src/secretscraper/handler.py` & `secretscraper-1.3.9/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8.1/src/secretscraper/log.py` & `secretscraper-1.3.9/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8.1/src/secretscraper/output_formatter.py` & `secretscraper-1.3.9/src/secretscraper/output_formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 import sys
 import typing
 
 import click
 
 from .entity import URL, Secret, URLNode
-from .util import Range, to_host_port
+from .util import Range, to_host_port, get_root_domain
 
 
 class Formatter:
     """Colorful output for terminal and non-colorful output for out-file"""
 
     def __init__(
         self,
@@ -123,22 +123,31 @@
 
     def output_url_per_domain(
         self, domains: typing.Set[str], url_dict: typing.Dict[URLNode, typing.Iterable[URLNode]], url_type: str = "URL"
     ) -> str:
         """Output the URLs for differenct domains"""
         url_hierarchy = ""
         domain_secrets: typing.Dict[str, typing.List[URLNode]] = dict()
+        root_domains = {get_root_domain(domain) for domain in domains}
         for base, urls in url_dict.items():
-            domain, _ = to_host_port(base.url_object.netloc)
-            if domain not in domains:
-                domain = "Other"
-            if domain not in domain_secrets:
-                domain_secrets[domain] = list()
-            domain_secrets[domain].extend(list(urls))
-        for domain, urls in domain_secrets.items():
+            l = list(urls)
+            l.append(base)
+            for url in l:
+                domain, _ = to_host_port(url.url_object.netloc)
+                domain = get_root_domain(domain)
+                if domain not in root_domains:
+                    domain = "Other"
+                if domain not in domain_secrets:
+                    domain_secrets[domain] = list()
+                domain_secrets[domain].append(url)
+        keys = list(domain_secrets.keys())
+        keys.remove("Other")
+        keys.append("Other")
+        for domain in keys:
+            urls = domain_secrets[domain]
             if urls is None or len(urls) == 0:
                 continue
             url_set = {
                 self.format_normal_result(f"{str(url.url)}")
                 + " ["
                 + self.format_colorful_status(url.response_status)
                 + "]"
```

### Comparing `secretscraper-1.3.8.1/src/secretscraper/scanner.py` & `secretscraper-1.3.9/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.8.1/src/secretscraper/urlparser.py` & `secretscraper-1.3.9/src/secretscraper/urlparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Extract URL nodes in HTML page."""
-
+import typing
 from typing import Set
 from urllib.parse import ParseResult, urlparse
 
 from bs4 import BeautifulSoup
 
 from .entity import URL, Secret, URLNode
 from .handler import Handler
@@ -53,17 +53,17 @@
             except KeyError:
                 pass
 
         for href in hrefs:
             if href is not None:
                 url_obj = urlparse(href)
 
-                if is_static_resource(url_obj.path):
+                if is_static_resource(url_obj.path): # remove static resource
                     continue
-                href = sanitize_url(href)
+                href = sanitize_url(href)  # remove dirty url
                 if len(href) == 0:
                     continue
                 if (
                     len(url_obj.scheme) > 0
                     and url_obj.netloc is not None
                     and len(url_obj.netloc) > 0
                 ):
```

### Comparing `secretscraper-1.3.8.1/src/secretscraper/util.py` & `secretscraper-1.3.9/src/secretscraper/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Common utility functions."""
 
 import re
 import typing
 from collections import namedtuple
 from urllib.parse import urlparse
+import tldextract
 
 # from dynaconf import LazySettings
 
 from .entity import URL
 from .exception import SecretScraperException
 
 Range = namedtuple("Range", ["start", "end"])
@@ -33,43 +34,57 @@
             f"Exception occur when reading rules from setting: {e}"
         ) from e
     return rules_dict
 
 
 def is_static_resource(path: str) -> bool:
     """Check whether a path is a static resource"""
-    exts = ['.png', '.jpg', '.jpeg', '.gif', '.css', '.ico', ".dtd", '.svg']
+    exts = {'.png', '.jpg', '.jpeg', '.gif', '.css', '.ico', ".dtd", '.svg', '.scss', '.vue', '.ts'}
     for ext in exts:
-        if path.endswith(ext):
+        if path.endswith(ext) or path.__contains__(ext + "?"):
             return True
     return False
 
 
 def to_host_port(netloc: str) -> typing.Tuple[str, str]:
     """Convert netloc to host and port"""
     r = netloc.split(":")
     if len(r) == 1:
         return r[0], ""
     if len(r) == 2:
         return r[0].strip(), r[1].strip()
     return '', ''
 
 
+def get_root_domain(host: str) -> str:
+    """Get the root domain"""
+    domain = tldextract.extract(host)
+
+    return domain.domain + "." + domain.suffix
+
+
 def sanitize_url(url: str) -> str:
     """Remove invalid characters in url
     Return emtpy string if url is invalid
     """
     url = url.replace(" ", "") \
         .replace("\\/", "/") \
         .replace("%3A", ":") \
         .replace("%2F", "/")
     # remove url that does not contain any word
     m = re.search("[a-zA-Z0-9]+", url)
     if m is None:
         return ""
+    m = re.search(
+        "\\<|\\>|\\{|\\}|\\[|\\]|\\||\\^|;|/node_modules/|www\\.w3\\.org|example\\.com|jquery[-\\.\\w]*?\\.js|\\.src|\\.replace|\\.url|\\.att|\\.href|location\\.href|javascript:|location:|application/x-www-form-urlencoded|\\.createObject|:location|\\.path|\\*#__PURE__\\*|\\*\\$0\\*|\\n",
+        url
+    )
+    if m is not None:
+        return ""
+
     if url.strip().startswith("javascript"):
         return ""
     try:
         obj = urlparse(url)
         if obj.netloc.startswith("127.0.0.1") or obj.netloc.startswith("localhost"):
             return ""
     except:
```

### Comparing `secretscraper-1.3.8.1/PKG-INFO` & `secretscraper-1.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.8.1
+Version: 1.3.9
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,15 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: httpx[socks] (>=0.27.0,<0.28.0)
 Requires-Dist: hyperscan (>=0.7.0,<0.8.0) ; python_version >= "3.10" and python_version < "4.0" and sys_platform == "darwin"
 Requires-Dist: hyperscan (>=0.7.0,<0.8.0) ; python_version >= "3.10" and python_version < "4.0" and sys_platform == "linux"
 Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; python_version >= "3.11" and python_version < "4.0" and sys_platform == "darwin"
 Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; python_version >= "3.11" and python_version < "4.0" and sys_platform == "linux"
+Requires-Dist: tldextract (>=5.1.2,<6.0.0)
 Description-Content-Type: text/markdown
 
 # SecretScraper
 
 ![Tests](https://github.com/PadishahIII/SecretScraper/actions/workflows/main.yml/badge.svg)
 ![Pypi Python Version](https://img.shields.io/pypi/pyversions/secretscraper.svg?style=plastic)
 
@@ -223,24 +224,31 @@
 ```
 
 ---
 
 # TODO
 - [ ] Support headless browser
 - [ ] Add regex doc reference
+- [ ] Fuzz path that are 404
+- [x] Separate subdomains in the result
+- [x] Optimize url collector
+[//]: # (- [ ] Employ jsbeautifier)
 - [x] Generate configuration file
 - [x] Detect dangerous paths and avoid requesting them
 - [x] Support url-finder output format, add `--detail` option
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.4.29 Version 1.3.9
+- Add `--validate` option
+- Optimize url collector
 ## 2024.4.29 Version 1.3.8
 - Optimize log output
 - Optimize the performance of `--debug` option
 ## 2024.4.29 Version 1.3.7
 - Test on multiple python versions
 - Support python 3.9~3.11
 ## 2024.4.29 Version 1.3.6
```

