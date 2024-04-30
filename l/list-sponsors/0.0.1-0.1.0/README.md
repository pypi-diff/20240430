# Comparing `tmp/list-sponsors-0.0.1.tar.gz` & `tmp/list_sponsors-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list-sponsors-0.0.1.tar", last modified: Sun Mar  6 09:19:13 2022, max compression
+gzip compressed data, was "list_sponsors-0.1.0.tar", last modified: Tue Apr 30 03:55:20 2024, max compression
```

## Comparing `list-sponsors-0.0.1.tar` & `list_sponsors-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,37 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-03-06 09:19:13.019161 list-sponsors-0.0.1/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2022-03-06 08:27:38.000000 list-sponsors-0.0.1/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      253 2022-03-06 07:56:47.000000 list-sponsors-0.0.1/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     3727 2022-03-06 09:19:13.019161 list-sponsors-0.0.1/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     2579 2022-03-06 08:19:51.000000 list-sponsors-0.0.1/README.md
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-03-06 09:19:13.019161 list-sponsors-0.0.1/list_sponsors/
--rw-r--r--   0 toor      (1000) toor      (1000)       88 2022-03-06 07:56:47.000000 list-sponsors-0.0.1/list_sponsors/__init__.py
--rwxr-xr-x   0 toor      (1000) toor      (1000)     3194 2022-03-06 08:34:27.000000 list-sponsors-0.0.1/list_sponsors/__main__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2022-03-06 07:56:47.000000 list-sponsors-0.0.1/list_sponsors/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      144 2022-03-06 08:16:20.000000 list-sponsors-0.0.1/list_sponsors/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5092 2022-03-06 08:17:49.000000 list-sponsors-0.0.1/list_sponsors/_gh_client.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1995 2022-03-06 07:56:47.000000 list-sponsors-0.0.1/list_sponsors/_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2691 2022-03-06 07:56:47.000000 list-sponsors-0.0.1/list_sponsors/_sponsor.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-03-06 09:19:13.019161 list-sponsors-0.0.1/list_sponsors.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     3727 2022-03-06 09:19:12.000000 list-sponsors-0.0.1/list_sponsors.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      570 2022-03-06 09:19:12.000000 list-sponsors-0.0.1/list_sponsors.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-03-06 09:19:12.000000 list-sponsors-0.0.1/list_sponsors.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       62 2022-03-06 09:19:12.000000 list-sponsors-0.0.1/list_sponsors.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-03-06 09:18:47.000000 list-sponsors-0.0.1/list_sponsors.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)       39 2022-03-06 09:19:12.000000 list-sponsors-0.0.1/list_sponsors.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       14 2022-03-06 09:19:12.000000 list-sponsors-0.0.1/list_sponsors.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      699 2022-03-06 07:56:47.000000 list-sponsors-0.0.1/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-03-06 09:19:13.019161 list-sponsors-0.0.1/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       24 2022-03-06 08:57:20.000000 list-sponsors-0.0.1/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        7 2022-03-06 07:56:47.000000 list-sponsors-0.0.1/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2022-03-06 09:19:13.019161 list-sponsors-0.0.1/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2429 2022-03-06 08:23:15.000000 list-sponsors-0.0.1/setup.py
--rw-r--r--   0 toor      (1000) toor      (1000)      863 2022-03-06 08:30:17.000000 list-sponsors-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:55:20.757188 list_sponsors-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:55:20.753188 list_sponsors-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:55:20.753188 list_sponsors-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-30 03:55:20.757188 list_sponsors-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:55:20.757188 list_sponsors-0.1.0/list_sponsors/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/list_sponsors/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3194 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/list_sponsors/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/list_sponsors/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/list_sponsors/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/list_sponsors/_gh_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/list_sponsors/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/list_sponsors/_sponsor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:55:20.757188 list_sponsors-0.1.0/list_sponsors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-30 03:55:20.000000 list_sponsors-0.1.0/list_sponsors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-30 03:55:20.000000 list_sponsors-0.1.0/list_sponsors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 03:55:20.000000 list_sponsors-0.1.0/list_sponsors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 03:55:20.000000 list_sponsors-0.1.0/list_sponsors.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 03:55:11.000000 list_sponsors-0.1.0/list_sponsors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 03:55:20.000000 list_sponsors-0.1.0/list_sponsors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 03:55:20.000000 list_sponsors-0.1.0/list_sponsors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:55:20.757188 list_sponsors-0.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 03:55:20.757188 list_sponsors-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:55:20.757188 list_sponsors-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/tests/test_sponsor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 03:54:54.000000 list_sponsors-0.1.0/tox.ini
```

### Comparing `list-sponsors-0.0.1/LICENSE` & `list_sponsors-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `list-sponsors-0.0.1/PKG-INFO` & `list_sponsors-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 Metadata-Version: 2.1
 Name: list-sponsors
-Version: 0.0.1
-Summary: A CLI tool to list GitHub sponsors of a user/organization with specified format.
+Version: 0.1.0
+Summary: A CLI tool to list GitHub sponsors of a user/organization with a specified format.
 Home-page: https://github.com/thombashi/list-sponsors
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changelog, https://github.com/thombashi/list-sponsors/releases
 Project-URL: Source, https://github.com/thombashi/list-sponsors
 Project-URL: Tracker, https://github.com/thombashi/list-sponsors/issues
 Keywords: GitHub,sponsors
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Terminals
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: loguru<1,>=0.4.1
+Requires-Dist: retryrequests<1,>=0.2.0
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # **list-sponsors**
 
 
 ## Summary
-A CLI tool to list GitHub sponsors of a user/organization with specified format.
+A CLI tool to list GitHub sponsors of a user/organization with a specified format.
 
 
 ## Installation
 
 ```
 pip install list-sponsors
 ```
@@ -70,25 +74,23 @@
 List your sponsors:
 
 ```
 export GITHUB_TOKEN=<PAT>
 list-sponsors
 ```
 
-### Output: raw
+### Output: raw markdown
 ```md
 [![onetime: Dmitry Belyaev (b4tman)](https://avatars.githubusercontent.com/u/3658062?s=48&v=4 "onetime: Dmitry Belyaev (b4tman)")](https://github.com/b4tman)
 [![Charles Becker (chasbecker)](https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4 "Charles Becker (chasbecker)")](https://github.com/chasbecker)
 [![onetime: Arturi0](https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4 "onetime: Arturi0")](https://github.com/Arturi0)
 ```
 
 ### Output: rendered
 [![onetime: Dmitry Belyaev (b4tman)](https://avatars.githubusercontent.com/u/3658062?s=48&v=4 "onetime: Dmitry Belyaev (b4tman)")](https://github.com/b4tman)
 [![Charles Becker (chasbecker)](https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4 "Charles Becker (chasbecker)")](https://github.com/chasbecker)
 [![onetime: Arturi0](https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4 "onetime: Arturi0")](https://github.com/Arturi0)
 
 
 ## Dependencies
-- Python 3.7+
+- Python 3.8+
 - [Python package dependencies (automatically installed)](https://github.com/thombashi/list-sponsors/network/dependencies)
-
-
```

### Comparing `list-sponsors-0.0.1/README.md` & `list_sponsors-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # **list-sponsors**
 
 
 ## Summary
-A CLI tool to list GitHub sponsors of a user/organization with specified format.
+A CLI tool to list GitHub sponsors of a user/organization with a specified format.
 
 
 ## Installation
 
 ```
 pip install list-sponsors
 ```
@@ -41,23 +41,23 @@
 List your sponsors:
 
 ```
 export GITHUB_TOKEN=<PAT>
 list-sponsors
 ```
 
-### Output: raw
+### Output: raw markdown
 ```md
 [![onetime: Dmitry Belyaev (b4tman)](https://avatars.githubusercontent.com/u/3658062?s=48&v=4 "onetime: Dmitry Belyaev (b4tman)")](https://github.com/b4tman)
 [![Charles Becker (chasbecker)](https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4 "Charles Becker (chasbecker)")](https://github.com/chasbecker)
 [![onetime: Arturi0](https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4 "onetime: Arturi0")](https://github.com/Arturi0)
 ```
 
 ### Output: rendered
 [![onetime: Dmitry Belyaev (b4tman)](https://avatars.githubusercontent.com/u/3658062?s=48&v=4 "onetime: Dmitry Belyaev (b4tman)")](https://github.com/b4tman)
 [![Charles Becker (chasbecker)](https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4 "Charles Becker (chasbecker)")](https://github.com/chasbecker)
 [![onetime: Arturi0](https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4 "onetime: Arturi0")](https://github.com/Arturi0)
 
 
 ## Dependencies
-- Python 3.7+
+- Python 3.8+
 - [Python package dependencies (automatically installed)](https://github.com/thombashi/list-sponsors/network/dependencies)
```

### Comparing `list-sponsors-0.0.1/list_sponsors/__main__.py` & `list_sponsors-0.1.0/list_sponsors/__main__.py`

 * *Files identical despite different names*

### Comparing `list-sponsors-0.0.1/list_sponsors/_gh_client.py` & `list_sponsors-0.1.0/list_sponsors/_gh_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,14 +61,20 @@
                                 sponsorEntity {
                                     ... on User {
                                         name
                                         login
                                         avatarUrl(size: $avatar_size)
                                         url
                                     }
+                                    ... on Organization {
+                                        name
+                                        login
+                                        avatarUrl(size: $avatar_size)
+                                        url
+                                    }
                                 }
                             }
                         }
                     }"""
         query = (
             """\
             query($login: String!, $avatar_size: Int!, $first: Int!, $after: String!) {
@@ -89,19 +95,30 @@
         variables: Dict[str, Union[str, int]] = {
             "login": login,
             "first": 100,
             "after": after,
             "avatar_size": avatar_size,
         }
         result = self.exec_query(query, variables=variables)
+        data = result.get("data", {})
+
+        if "user" in data:
+            return data["user"]["sponsorshipsAsMaintainer"]
+        elif "organization" in data:
+            return data["organization"]["sponsorshipsAsMaintainer"]
+
+        err_msg_cache = set()
+        if "errors" in result:
+            for error in result["errors"]:
+                err_msg = f"{error['type']}: {error['message']}"
+                if err_msg in err_msg_cache:
+                    continue
 
-        if result["data"]["user"]:
-            return result["data"]["user"]["sponsorshipsAsMaintainer"]
-        elif result["data"]["organization"]:
-            return result["data"]["organization"]["sponsorshipsAsMaintainer"]
+                err_msg_cache.add(err_msg)
+                logger.error(err_msg)
 
         raise RuntimeError("empty result")
 
     def fetch_sponsors(self, login: str, avatar_size: int) -> Iterator[Sponsor]:
         sponsorships = self.__fetch_sponsors(login=login, after="", avatar_size=avatar_size)
         logger.debug(f"results - totalCount: {sponsorships['totalCount']}")
 
@@ -112,22 +129,21 @@
                 continue
 
             tier = node["tier"]
             if not tier:
                 price = None
             else:
                 price = tier["monthlyPriceInDollars"] if "monthlyPriceInDollars" in tier else None
-                # print(price)
 
             yield Sponsor(
                 **entity, monthlyPriceInDollars=price, isOneTimePayment=node["isOneTimePayment"]
             )
 
         page_info = sponsorships["pageInfo"]
-        # print(page_info)
+        logger.debug(f"pageInfo: {page_info}")
 
         while page_info["hasNextPage"]:
             sponsorships = self.__fetch_sponsors(
                 login=login, after=page_info["endCursor"], avatar_size=avatar_size
             )
             for sponsor in sponsorships["edges"]:
                 node = sponsor["node"]
@@ -144,8 +160,8 @@
                     )
 
                 yield Sponsor(
                     **entity, monthlyPriceInDollars=price, isOneTimePayment=node["isOneTimePayment"]
                 )
 
             page_info = sponsorships["pageInfo"]
-            # print(page_info)
+            logger.debug(f"pageInfo: {page_info}")
```

### Comparing `list-sponsors-0.0.1/list_sponsors/_logger.py` & `list_sponsors-0.1.0/list_sponsors/_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import sys
 
+from loguru import logger
+
 from ._const import MODULE_NAME, LogLevel
 
 
+logger.disable(MODULE_NAME)
+
+
 class NullLogger:
     level_name = None
 
     def remove(self, handler_id=None):  # pragma: no cover
         pass
 
     def add(self, sink, **kwargs):  # pragma: no cover
@@ -42,23 +47,15 @@
     def trace(self, __message, *args, **kwargs):  # pragma: no cover
         pass
 
     def warning(self, __message, *args, **kwargs):  # pragma: no cover
         pass
 
 
-try:
-    from loguru import logger
-
-    logger.disable(MODULE_NAME)
-except ImportError:
-    logger = NullLogger()  # type: ignore
-
-
-def set_logger(is_enable: bool, propagation_depth: int = 1):
+def set_logger(is_enable: bool, propagation_depth: int = 1) -> None:
     if is_enable:
         logger.enable(MODULE_NAME)
     else:
         logger.disable(MODULE_NAME)
 
 
 def initialize_logger(name: str, log_level: str) -> None:
```

### Comparing `list-sponsors-0.0.1/list_sponsors/_sponsor.py` & `list_sponsors-0.1.0/list_sponsors/_sponsor.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,16 @@
     def alt(self) -> str:
         return f"onetime: {self.name_and_login}" if self.isOneTimePayment else self.name_and_login
 
 
 class SponsorRendererInterface(metaclass=abc.ABCMeta):
     REGEXP_HAS_AVATAR = re.compile(r"&u=")
 
-    @abc.abstractclassmethod
-    def render(self, sponsor: Sponsor, avatar_size: Optional[int] = None) -> str:
-        pass
+    @abc.abstractmethod
+    def render(self, sponsor: Sponsor, avatar_size: Optional[int] = None) -> str: ...
 
 
 class MarkdownSponsorRenderer(SponsorRendererInterface):
     def render(self, sponsor: Sponsor, avatar_size: Optional[int] = None) -> str:
         return '[![{alt}]({avatar} "{alt}")]({url})'.format(
             alt=sponsor.alt, avatar=sponsor.avatarUrl, url=sponsor.url
         )
```

### Comparing `list-sponsors-0.0.1/list_sponsors.egg-info/PKG-INFO` & `list_sponsors-0.1.0/list_sponsors.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 Metadata-Version: 2.1
 Name: list-sponsors
-Version: 0.0.1
-Summary: A CLI tool to list GitHub sponsors of a user/organization with specified format.
+Version: 0.1.0
+Summary: A CLI tool to list GitHub sponsors of a user/organization with a specified format.
 Home-page: https://github.com/thombashi/list-sponsors
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changelog, https://github.com/thombashi/list-sponsors/releases
 Project-URL: Source, https://github.com/thombashi/list-sponsors
 Project-URL: Tracker, https://github.com/thombashi/list-sponsors/issues
 Keywords: GitHub,sponsors
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Terminals
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: loguru<1,>=0.4.1
+Requires-Dist: retryrequests<1,>=0.2.0
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # **list-sponsors**
 
 
 ## Summary
-A CLI tool to list GitHub sponsors of a user/organization with specified format.
+A CLI tool to list GitHub sponsors of a user/organization with a specified format.
 
 
 ## Installation
 
 ```
 pip install list-sponsors
 ```
@@ -70,25 +74,23 @@
 List your sponsors:
 
 ```
 export GITHUB_TOKEN=<PAT>
 list-sponsors
 ```
 
-### Output: raw
+### Output: raw markdown
 ```md
 [![onetime: Dmitry Belyaev (b4tman)](https://avatars.githubusercontent.com/u/3658062?s=48&v=4 "onetime: Dmitry Belyaev (b4tman)")](https://github.com/b4tman)
 [![Charles Becker (chasbecker)](https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4 "Charles Becker (chasbecker)")](https://github.com/chasbecker)
 [![onetime: Arturi0](https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4 "onetime: Arturi0")](https://github.com/Arturi0)
 ```
 
 ### Output: rendered
 [![onetime: Dmitry Belyaev (b4tman)](https://avatars.githubusercontent.com/u/3658062?s=48&v=4 "onetime: Dmitry Belyaev (b4tman)")](https://github.com/b4tman)
 [![Charles Becker (chasbecker)](https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4 "Charles Becker (chasbecker)")](https://github.com/chasbecker)
 [![onetime: Arturi0](https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4 "onetime: Arturi0")](https://github.com/Arturi0)
 
 
 ## Dependencies
-- Python 3.7+
+- Python 3.8+
 - [Python package dependencies (automatically installed)](https://github.com/thombashi/list-sponsors/network/dependencies)
-
-
```

### Comparing `list-sponsors-0.0.1/setup.py` & `list_sponsors-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "list-sponsors"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -31,43 +31,44 @@
     INSTALL_REQUIRES = [line.strip() for line in f if line.strip()]
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     TESTS_REQUIRES = [line.strip() for line in f if line.strip()]
 
 setuptools.setup(
     name=MODULE_NAME,
-    version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
-    description="A CLI tool to list GitHub sponsors of a user/organization with specified format.",
+    description="A CLI tool to list GitHub sponsors of a user/organization with a specified format.",
     include_package_data=True,
     keywords=["GitHub", "sponsors"],
     license=pkg_info["__license__"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests*"]),
     project_urls={
+        "Changelog": f"{REPOSITORY_URL:s}/releases",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=INSTALL_REQUIRES,
     extras_require={"test": TESTS_REQUIRES},
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Terminals",
     ],
     cmdclass=get_release_command_class(),
     zip_safe=False,
     entry_points={
         "console_scripts": [
```

### Comparing `list-sponsors-0.0.1/tox.ini` & `list_sponsors-0.1.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 [tox]
 envlist =
-    py{37,38,39,310}
+    py{38,39,310,311,312}
     build
-    clean
     fmt
     lint
 
 [testenv]
 extras =
     test
 commands =
     pytest {posargs} tests
 
 [testenv:build]
-basepython = python3.8
 deps =
+    build>=1
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
+    python -m build
     twine check dist/*.whl dist/*.tar.gz
-    python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
-    cleanpy>=0.3.1
+    cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
 
 [testenv:fmt]
 skip_install = true
 deps =
-    autoflake>=1.4
-    black>=22.1
+    autoflake>=2
     isort>=5
+    ruff>=0.3.5
 commands =
-    autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
+    autoflake --in-place --recursive --remove-all-unused-imports .
     isort .
-    black setup.py tests list_sponsors
+    ruff format
 
 [testenv:lint]
-skip_install = true
+extras =
+    test
 deps =
-    mypy>=0.931
-    pylama>=8.3.6
-    types-requests
+    codespell>=2
+    mypy>=1
+    pyright>=1.1
+    releasecmd
+    ruff>=0.3.5
 commands =
-    python setup.py check
     mypy list_sponsors setup.py
-    pylama
+    pyright
+    codespell list_sponsors setup.py tests -q2 --check-filenames
+    ruff format --check
+    ruff check
```

