# Comparing `tmp/freqtrade-client-2024.3.dev1.tar.gz` & `tmp/freqtrade_client-2024.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freqtrade-client-2024.3.dev1.tar", last modified: Fri Mar 29 08:00:36 2024, max compression
+gzip compressed data, was "freqtrade_client-2024.4.tar", last modified: Tue Apr 30 12:41:58 2024, max compression
```

## Comparing `freqtrade-client-2024.3.dev1.tar` & `freqtrade_client-2024.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 xmatt     (1000) xmatt     (1000)        0 2024-03-29 08:00:36.274244 freqtrade-client-2024.3.dev1/
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)     1320 2024-03-29 08:00:36.274244 freqtrade-client-2024.3.dev1/PKG-INFO
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)      304 2024-03-29 07:59:45.000000 freqtrade-client-2024.3.dev1/README.md
-drwxr-xr-x   0 xmatt     (1000) xmatt     (1000)        0 2024-03-29 08:00:36.274244 freqtrade-client-2024.3.dev1/freqtrade_client/
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)      881 2024-03-29 08:00:28.000000 freqtrade-client-2024.3.dev1/freqtrade_client/__init__.py
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)     3282 2024-03-29 07:33:22.000000 freqtrade-client-2024.3.dev1/freqtrade_client/ft_client.py
--rwxr-xr-x   0 xmatt     (1000) xmatt     (1000)    12407 2024-03-29 07:38:32.000000 freqtrade-client-2024.3.dev1/freqtrade_client/ft_rest_client.py
-drwxr-xr-x   0 xmatt     (1000) xmatt     (1000)        0 2024-03-29 08:00:36.274244 freqtrade-client-2024.3.dev1/freqtrade_client.egg-info/
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)     1320 2024-03-29 08:00:36.000000 freqtrade-client-2024.3.dev1/freqtrade_client.egg-info/PKG-INFO
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)      360 2024-03-29 08:00:36.000000 freqtrade-client-2024.3.dev1/freqtrade_client.egg-info/SOURCES.txt
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)        1 2024-03-29 08:00:36.000000 freqtrade-client-2024.3.dev1/freqtrade_client.egg-info/dependency_links.txt
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)       60 2024-03-29 08:00:36.000000 freqtrade-client-2024.3.dev1/freqtrade_client.egg-info/entry_points.txt
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)       39 2024-03-29 08:00:36.000000 freqtrade-client-2024.3.dev1/freqtrade_client.egg-info/requires.txt
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)       17 2024-03-29 08:00:36.000000 freqtrade-client-2024.3.dev1/freqtrade_client.egg-info/top_level.txt
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)     1392 2024-03-29 08:00:00.000000 freqtrade-client-2024.3.dev1/pyproject.toml
--rw-r--r--   0 xmatt     (1000) xmatt     (1000)       38 2024-03-29 08:00:36.274244 freqtrade-client-2024.3.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:41:58.578423 freqtrade_client-2024.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 12:41:58.578423 freqtrade_client-2024.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:41:58.578423 freqtrade_client-2024.4/freqtrade_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/freqtrade_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/freqtrade_client/ft_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13616 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/freqtrade_client/ft_rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:41:58.578423 freqtrade_client-2024.4/freqtrade_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:41:58.578423 freqtrade_client-2024.4/setup.cfg
```

### Comparing `freqtrade-client-2024.3.dev1/PKG-INFO` & `freqtrade_client-2024.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freqtrade-client
-Version: 2024.3.dev1
+Version: 2024.4
 Summary: Freqtrade - Client scripts
 Author: Freqtrade Team
 Author-email: Freqtrade Team <freqtrade@protonmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/freqtrade/freqtrade
 Project-URL: Documentation, https://freqtrade.io
 Project-URL: Bug Tracker, https://github.com/freqtrade/freqtrade/issues
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests>=2.26.0
 Requires-Dist: python-rapidjson>=1.0
 
 # Freqtrade Client
 
 # ![freqtrade](https://raw.githubusercontent.com/freqtrade/freqtrade/develop/docs/assets/freqtrade_poweredby.svg)
```

### Comparing `freqtrade-client-2024.3.dev1/freqtrade_client/__init__.py` & `freqtrade_client-2024.4/freqtrade_client/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from freqtrade_client.ft_rest_client import FtRestClient
 
 
-__all__ = ['FtRestClient']
-
-
-__version__ = '2024.3-dev1'
+__version__ = '2024.4'
 
 if 'dev' in __version__:
     from pathlib import Path
     try:
         import subprocess
         freqtrade_basedir = Path(__file__).parent
 
@@ -21,7 +18,9 @@
         try:
             # Try Fallback to freqtrade_commit file (created by CI while building docker image)
             versionfile = Path('./freqtrade_commit')
             if versionfile.is_file():
                 __version__ = f"docker-{__version__}-{versionfile.read_text()[:8]}"
         except Exception:
             pass
+
+__all__ = ['FtRestClient']
```

### Comparing `freqtrade-client-2024.3.dev1/freqtrade_client/ft_client.py` & `freqtrade_client-2024.4/freqtrade_client/ft_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 logging.basicConfig(
     level=logging.INFO,
     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
 )
 logger = logging.getLogger("ft_rest_client")
 
 
-def add_arguments():
-    parser = argparse.ArgumentParser()
+def add_arguments(args: Any = None):
+    parser = argparse.ArgumentParser(
+            prog="freqtrade-client",
+            description="Client for the freqtrade REST API",
+    )
     parser.add_argument("command",
                         help="Positional argument defining the command to execute.",
                         nargs="?"
                         )
     parser.add_argument('-V', '--version', action='version', version=f'%(prog)s {__version__}')
     parser.add_argument('--show',
                         help='Show possible methods with this client',
@@ -43,16 +46,16 @@
 
     parser.add_argument("command_arguments",
                         help="Positional arguments for the parameters for [command]",
                         nargs="*",
                         default=[]
                         )
 
-    args = parser.parse_args()
-    return vars(args)
+    pargs = parser.parse_args(args)
+    return vars(pargs)
 
 
 def load_config(configfile):
     file = Path(configfile)
     if file.is_file():
         with file.open("r") as f:
             config = rapidjson.load(f, parse_mode=rapidjson.PM_COMMENTS |
@@ -63,15 +66,15 @@
         sys.exit(1)
 
 
 def print_commands():
     # Print dynamic help for the different commands using the commands doc-strings
     client = FtRestClient(None)
     print("Possible commands:\n")
-    for x, y in inspect.getmembers(client):
+    for x, _ in inspect.getmembers(client):
         if not x.startswith('_'):
             doc = re.sub(':return:.*', '', getattr(client, x).__doc__, flags=re.MULTILINE).rstrip()
             print(f"{x}\n\t{doc}\n")
 
 
 def main_exec(args: Dict[str, Any]):
```

### Comparing `freqtrade-client-2024.3.dev1/freqtrade_client/ft_rest_client.py` & `freqtrade_client-2024.4/freqtrade_client/ft_rest_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,44 @@
-#!/usr/bin/env python3
 """
-Simple command line client into RPC commands
-Can be used as an alternate to Telegram
+A Rest Client for Freqtrade bot
 
 Should not import anything from freqtrade,
-so it can be used as a standalone script.
+so it can be used as a standalone script, and can be installed independently.
 """
 
 import json
 import logging
-from typing import Optional
+from typing import Any, Dict, List, Optional, Union
 from urllib.parse import urlencode, urlparse, urlunparse
 
 import requests
 from requests.exceptions import ConnectionError
 
 
 logger = logging.getLogger("ft_rest_client")
 
+ParamsT = Optional[Dict[str, Any]]
+PostDataT = Optional[Union[Dict[str, Any], List[Dict[str, Any]]]]
+
 
 class FtRestClient:
 
-    def __init__(self, serverurl, username=None, password=None):
+    def __init__(self, serverurl, username=None, password=None, *,
+                 pool_connections=10, pool_maxsize=10):
 
         self._serverurl = serverurl
         self._session = requests.Session()
+
+        # allow configuration of pool
+        adapter = requests.adapters.HTTPAdapter(
+            pool_connections=pool_connections,
+            pool_maxsize=pool_maxsize
+        )
+        self._session.mount('http://', adapter)
+
         self._session.auth = (username, password)
 
     def _call(self, method, apipath, params: Optional[dict] = None, data=None, files=None):
 
         if str(method).upper() not in ('GET', 'POST', 'PUT', 'DELETE'):
             raise ValueError(f'invalid method <{method}>')
         basepath = f"{self._serverurl}/api/v1/{apipath}"
@@ -47,21 +57,21 @@
         try:
             resp = self._session.request(method, url, headers=hd, data=json.dumps(data))
             # return resp.text
             return resp.json()
         except ConnectionError:
             logger.warning("Connection error")
 
-    def _get(self, apipath, params: Optional[dict] = None):
+    def _get(self, apipath, params: ParamsT = None):
         return self._call("GET", apipath, params=params)
 
-    def _delete(self, apipath, params: Optional[dict] = None):
+    def _delete(self, apipath, params: ParamsT = None):
         return self._call("DELETE", apipath, params=params)
 
-    def _post(self, apipath, params: Optional[dict] = None, data: Optional[dict] = None):
+    def _post(self, apipath, params: ParamsT = None, data: PostDataT = None):
         return self._call("POST", apipath, params=params, data=data)
 
     def start(self):
         """Start the bot if it's in the stopped state.
 
         :return: json object
         """
@@ -137,14 +147,33 @@
         """Delete (disable) lock from the database.
 
         :param lock_id: ID for the lock to delete
         :return: json object
         """
         return self._delete(f"locks/{lock_id}")
 
+    def lock_add(self, pair: str, until: str, side: str = '*', reason: str = ''):
+        """Lock pair
+
+        :param pair: Pair to lock
+        :param until: Lock until this date (format "2024-03-30 16:00:00Z")
+        :param side: Side to lock (long, short, *)
+        :param reason: Reason for the lock
+        :return: json object
+        """
+        data = [
+            {
+                "pair": pair,
+                "until": until,
+                "side": side,
+                "reason": reason
+            }
+        ]
+        return self._post("locks", data=data)
+
     def daily(self, days=None):
         """Return the profits for each day, and amount of trades.
 
         :return: json object
         """
         return self._get("daily", params={"timescale": days} if days else None)
 
@@ -364,28 +393,37 @@
         :return: json object
         """
         return self._get("available_pairs", params={
             "stake_currency": stake_currency if timeframe else '',
             "timeframe": timeframe if timeframe else '',
         })
 
-    def pair_candles(self, pair, timeframe, limit=None):
+    def pair_candles(self, pair, timeframe, limit=None, columns=None):
         """Return live dataframe for <pair><timeframe>.
 
         :param pair: Pair to get data for
         :param timeframe: Only pairs with this timeframe available.
         :param limit: Limit result to the last n candles.
+        :param columns: List of dataframe columns to return. Empty list will return OHLCV.
         :return: json object
         """
         params = {
             "pair": pair,
             "timeframe": timeframe,
         }
         if limit:
             params['limit'] = limit
+
+        if columns is not None:
+            params['columns'] = columns
+            return self._post(
+                "pair_candles",
+                data=params
+            )
+
         return self._get("pair_candles", params=params)
 
     def pair_history(self, pair, timeframe, strategy, timerange=None, freqaimodel=None):
         """Return historic, analyzed dataframe
 
         :param pair: Pair to get data for
         :param timeframe: Only pairs with this timeframe available.
```

### Comparing `freqtrade-client-2024.3.dev1/freqtrade_client.egg-info/PKG-INFO` & `freqtrade_client-2024.4/freqtrade_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freqtrade-client
-Version: 2024.3.dev1
+Version: 2024.4
 Summary: Freqtrade - Client scripts
 Author: Freqtrade Team
 Author-email: Freqtrade Team <freqtrade@protonmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/freqtrade/freqtrade
 Project-URL: Documentation, https://freqtrade.io
 Project-URL: Bug Tracker, https://github.com/freqtrade/freqtrade/issues
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests>=2.26.0
 Requires-Dist: python-rapidjson>=1.0
 
 # Freqtrade Client
 
 # ![freqtrade](https://raw.githubusercontent.com/freqtrade/freqtrade/develop/docs/assets/freqtrade_poweredby.svg)
```

### Comparing `freqtrade-client-2024.3.dev1/pyproject.toml` & `freqtrade_client-2024.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 [project.urls]
 Homepage = "https://github.com/freqtrade/freqtrade"
 Documentation = "https://freqtrade.io"
 "Bug Tracker" = "https://github.com/freqtrade/freqtrade/issues"
 
 
 [project.scripts]
-ft_rest = "freqtrade_client.ft_client:main"
+freqtrade-client = "freqtrade_client.ft_client:main"
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["freqtrade_client*"]
 exclude = ["tests", "tests.*"]
 namespaces = true
```

