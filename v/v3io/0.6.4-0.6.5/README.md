# Comparing `tmp/v3io-0.6.4.tar.gz` & `tmp/v3io-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v3io-0.6.4.tar", last modified: Sun Mar 31 12:55:35 2024, max compression
+gzip compressed data, was "v3io-0.6.5.tar", last modified: Tue Apr 30 05:55:42 2024, max compression
```

## Comparing `v3io-0.6.4.tar` & `v3io-0.6.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 12:55:35.291281 v3io-0.6.4/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-01-04 08:51:26.000000 v3io-0.6.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       30 2024-01-04 08:51:26.000000 v3io-0.6.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    14514 2024-03-31 12:55:35.291281 v3io-0.6.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13310 2024-01-04 12:11:45.000000 v3io-0.6.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-31 12:55:35.291281 v3io-0.6.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2825 2024-01-04 08:51:26.000000 v3io-0.6.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 12:55:35.284281 v3io-0.6.4/tests/
--rw-r--r--   0 root         (0) root         (0)    29372 2024-02-07 12:34:16.000000 v3io-0.6.4/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)    22000 2024-01-04 08:51:26.000000 v3io-0.6.4/tests/test_client_aio.py
--rw-r--r--   0 root         (0) root         (0)     6104 2024-03-31 07:34:43.000000 v3io-0.6.4/tests/test_client_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 12:55:35.285281 v3io-0.6.4/v3io/
--rw-r--r--   0 root         (0) root         (0)      595 2024-03-31 12:55:32.000000 v3io-0.6.4/v3io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 12:55:35.282281 v3io-0.6.4/v3io/aio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 12:55:35.287281 v3io-0.6.4/v3io/aio/dataplane/
--rw-r--r--   0 root         (0) root         (0)      681 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/aio/dataplane/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4257 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/aio/dataplane/client.py
--rw-r--r--   0 root         (0) root         (0)     2740 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/aio/dataplane/container.py
--rw-r--r--   0 root         (0) root         (0)    15316 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/aio/dataplane/kv.py
--rw-r--r--   0 root         (0) root         (0)     3869 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/aio/dataplane/kv_cursor.py
--rw-r--r--   0 root         (0) root         (0)     4637 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/aio/dataplane/object.py
--rw-r--r--   0 root         (0) root         (0)    15134 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/aio/dataplane/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 12:55:35.287281 v3io-0.6.4/v3io/aio/dataplane/transport/
--rw-r--r--   0 root         (0) root         (0)      573 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/aio/dataplane/transport/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4139 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/aio/dataplane/transport/aiohttp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 12:55:35.288281 v3io-0.6.4/v3io/common/
--rw-r--r--   0 root         (0) root         (0)      573 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      817 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/common/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 12:55:35.290281 v3io-0.6.4/v3io/dataplane/
--rw-r--r--   0 root         (0) root         (0)      666 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4487 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/batch.py
--rw-r--r--   0 root         (0) root         (0)    42124 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/client.py
--rw-r--r--   0 root         (0) root         (0)     2791 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/container.py
--rw-r--r--   0 root         (0) root         (0)    15754 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/kv.py
--rw-r--r--   0 root         (0) root         (0)     2144 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/kv_array.py
--rw-r--r--   0 root         (0) root         (0)     4039 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/kv_cursor.py
--rw-r--r--   0 root         (0) root         (0)     1608 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/kv_timestamp.py
--rw-r--r--   0 root         (0) root         (0)      742 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/model.py
--rw-r--r--   0 root         (0) root         (0)     4894 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/object.py
--rw-r--r--   0 root         (0) root         (0)     7887 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/output.py
--rw-r--r--   0 root         (0) root         (0)    12123 2024-02-12 11:42:26.000000 v3io-0.6.4/v3io/dataplane/request.py
--rw-r--r--   0 root         (0) root         (0)     3471 2024-03-31 12:33:23.000000 v3io-0.6.4/v3io/dataplane/response.py
--rw-r--r--   0 root         (0) root         (0)    15526 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 12:55:35.290281 v3io-0.6.4/v3io/dataplane/transport/
--rw-r--r--   0 root         (0) root         (0)      787 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/transport/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2815 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/transport/abstract.py
--rw-r--r--   0 root         (0) root         (0)     8558 2024-03-31 07:26:31.000000 v3io-0.6.4/v3io/dataplane/transport/httpclient.py
--rw-r--r--   0 root         (0) root         (0)     2337 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/transport/requests.py
--rw-r--r--   0 root         (0) root         (0)     1385 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/dataplane/transport/verifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 12:55:35.291281 v3io-0.6.4/v3io/logger/
--rw-r--r--   0 root         (0) root         (0)      649 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2619 2024-01-04 08:51:26.000000 v3io-0.6.4/v3io/logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 12:55:35.291281 v3io-0.6.4/v3io.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14514 2024-03-31 12:55:35.000000 v3io-0.6.4/v3io.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1199 2024-03-31 12:55:35.000000 v3io-0.6.4/v3io.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 12:55:35.000000 v3io-0.6.4/v3io.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-31 12:55:35.000000 v3io-0.6.4/v3io.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-31 12:55:35.000000 v3io-0.6.4/v3io.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:55:42.649643 v3io-0.6.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-01-04 08:51:26.000000 v3io-0.6.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       30 2024-01-04 08:51:26.000000 v3io-0.6.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14514 2024-04-30 05:55:42.649643 v3io-0.6.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13310 2024-01-04 12:11:45.000000 v3io-0.6.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 05:55:42.649643 v3io-0.6.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2825 2024-01-04 08:51:26.000000 v3io-0.6.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:55:42.644643 v3io-0.6.5/tests/
+-rw-r--r--   0 root         (0) root         (0)    29372 2024-02-07 12:34:16.000000 v3io-0.6.5/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)    22000 2024-01-04 08:51:26.000000 v3io-0.6.5/tests/test_client_aio.py
+-rw-r--r--   0 root         (0) root         (0)     6104 2024-03-31 07:34:43.000000 v3io-0.6.5/tests/test_client_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:55:42.644643 v3io-0.6.5/v3io/
+-rw-r--r--   0 root         (0) root         (0)      656 2024-04-30 05:55:39.000000 v3io-0.6.5/v3io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:55:42.642643 v3io-0.6.5/v3io/aio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:55:42.645643 v3io-0.6.5/v3io/aio/dataplane/
+-rw-r--r--   0 root         (0) root         (0)      681 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/aio/dataplane/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/aio/dataplane/client.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/aio/dataplane/container.py
+-rw-r--r--   0 root         (0) root         (0)    15316 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/aio/dataplane/kv.py
+-rw-r--r--   0 root         (0) root         (0)     3869 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/aio/dataplane/kv_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     4637 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/aio/dataplane/object.py
+-rw-r--r--   0 root         (0) root         (0)    15134 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/aio/dataplane/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:55:42.646643 v3io-0.6.5/v3io/aio/dataplane/transport/
+-rw-r--r--   0 root         (0) root         (0)      573 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/aio/dataplane/transport/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4139 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/aio/dataplane/transport/aiohttp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:55:42.646643 v3io-0.6.5/v3io/common/
+-rw-r--r--   0 root         (0) root         (0)      573 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      817 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/common/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:55:42.648643 v3io-0.6.5/v3io/dataplane/
+-rw-r--r--   0 root         (0) root         (0)      666 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4487 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/batch.py
+-rw-r--r--   0 root         (0) root         (0)    42124 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/client.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/container.py
+-rw-r--r--   0 root         (0) root         (0)    15754 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/kv.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/kv_array.py
+-rw-r--r--   0 root         (0) root         (0)     4039 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/kv_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/kv_timestamp.py
+-rw-r--r--   0 root         (0) root         (0)      742 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/model.py
+-rw-r--r--   0 root         (0) root         (0)     4894 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/object.py
+-rw-r--r--   0 root         (0) root         (0)     7887 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/output.py
+-rw-r--r--   0 root         (0) root         (0)    12123 2024-02-12 11:42:26.000000 v3io-0.6.5/v3io/dataplane/request.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-03-31 12:33:23.000000 v3io-0.6.5/v3io/dataplane/response.py
+-rw-r--r--   0 root         (0) root         (0)    15526 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:55:42.648643 v3io-0.6.5/v3io/dataplane/transport/
+-rw-r--r--   0 root         (0) root         (0)      787 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/transport/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/transport/abstract.py
+-rw-r--r--   0 root         (0) root         (0)     8558 2024-03-31 07:26:31.000000 v3io-0.6.5/v3io/dataplane/transport/httpclient.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/transport/requests.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/dataplane/transport/verifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:55:42.649643 v3io-0.6.5/v3io/logger/
+-rw-r--r--   0 root         (0) root         (0)      649 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2024-01-04 08:51:26.000000 v3io-0.6.5/v3io/logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:55:42.649643 v3io-0.6.5/v3io.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14514 2024-04-30 05:55:42.000000 v3io-0.6.5/v3io.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-04-30 05:55:42.000000 v3io-0.6.5/v3io.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 05:55:42.000000 v3io-0.6.5/v3io.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-30 05:55:42.000000 v3io-0.6.5/v3io.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-30 05:55:42.000000 v3io-0.6.5/v3io.egg-info/top_level.txt
```

### Comparing `v3io-0.6.4/LICENSE` & `v3io-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/PKG-INFO` & `v3io-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v3io
-Version: 0.6.4
+Version: 0.6.5
 Summary: SDK for v3io
 Home-page: https://github.com/v3io/v3io-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `v3io-0.6.4/README.md` & `v3io-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/setup.py` & `v3io-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/tests/test_client.py` & `v3io-0.6.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/tests/test_client_aio.py` & `v3io-0.6.5/tests/test_client_aio.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/tests/test_client_errors.py` & `v3io-0.6.5/tests/test_client_errors.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/__init__.py` & `v3io-0.6.5/v3io/aio/dataplane/transport/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.6.4"
```

### Comparing `v3io-0.6.4/v3io/aio/dataplane/__init__.py` & `v3io-0.6.5/v3io/aio/dataplane/__init__.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/aio/dataplane/client.py` & `v3io-0.6.5/v3io/aio/dataplane/client.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/aio/dataplane/container.py` & `v3io-0.6.5/v3io/aio/dataplane/container.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/aio/dataplane/kv.py` & `v3io-0.6.5/v3io/aio/dataplane/kv.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/aio/dataplane/kv_cursor.py` & `v3io-0.6.5/v3io/aio/dataplane/kv_cursor.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/aio/dataplane/object.py` & `v3io-0.6.5/v3io/aio/dataplane/object.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/aio/dataplane/stream.py` & `v3io-0.6.5/v3io/aio/dataplane/stream.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/aio/dataplane/transport/__init__.py` & `v3io-0.6.5/v3io/common/__init__.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/aio/dataplane/transport/aiohttp.py` & `v3io-0.6.5/v3io/aio/dataplane/transport/aiohttp.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/common/__init__.py` & `v3io-0.6.5/v3io/dataplane/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,7 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+class Model(object):
+    @staticmethod
+    def _ensure_path_ends_with_slash(path):
+        if not path.endswith("/"):
+            return path + "/"
+
+        return path
```

### Comparing `v3io-0.6.4/v3io/common/helpers.py` & `v3io-0.6.5/v3io/common/helpers.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/__init__.py` & `v3io-0.6.5/v3io/dataplane/__init__.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/batch.py` & `v3io-0.6.5/v3io/dataplane/batch.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/client.py` & `v3io-0.6.5/v3io/dataplane/client.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/container.py` & `v3io-0.6.5/v3io/dataplane/container.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/kv.py` & `v3io-0.6.5/v3io/dataplane/kv.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/kv_array.py` & `v3io-0.6.5/v3io/dataplane/kv_array.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/kv_cursor.py` & `v3io-0.6.5/v3io/dataplane/kv_cursor.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/kv_timestamp.py` & `v3io-0.6.5/v3io/dataplane/kv_timestamp.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/model.py` & `v3io-0.6.5/v3io/dataplane/transport/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-class Model(object):
-    @staticmethod
-    def _ensure_path_ends_with_slash(path):
-        if not path.endswith("/"):
-            return path + "/"
+from .verifier import Transport  # noqa: F401
 
-        return path
+
+class RaiseForStatus(object):
+    never = "never"
+    always = "always"
+
+
+class Actions(object):
+    encode_only = 1
+    encode_and_send = 2
+    send_and_receive = 3
```

### Comparing `v3io-0.6.4/v3io/dataplane/object.py` & `v3io-0.6.5/v3io/dataplane/object.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/output.py` & `v3io-0.6.5/v3io/dataplane/output.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/request.py` & `v3io-0.6.5/v3io/dataplane/request.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/response.py` & `v3io-0.6.5/v3io/dataplane/response.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/stream.py` & `v3io-0.6.5/v3io/dataplane/stream.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/transport/__init__.py` & `v3io-0.6.5/v3io/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,19 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .verifier import Transport  # noqa: F401
+__version__ = "0.6.5"
 
-
-class RaiseForStatus(object):
-    never = "never"
-    always = "always"
-
-
-class Actions(object):
-    encode_only = 1
-    encode_and_send = 2
-    send_and_receive = 3
+from .dataplane import Client, RaiseForStatus  # noqa: F401
```

### Comparing `v3io-0.6.4/v3io/dataplane/transport/abstract.py` & `v3io-0.6.5/v3io/dataplane/transport/abstract.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/transport/httpclient.py` & `v3io-0.6.5/v3io/dataplane/transport/httpclient.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/transport/requests.py` & `v3io-0.6.5/v3io/dataplane/transport/requests.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/dataplane/transport/verifier.py` & `v3io-0.6.5/v3io/dataplane/transport/verifier.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/logger/__init__.py` & `v3io-0.6.5/v3io/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io/logger/logger.py` & `v3io-0.6.5/v3io/logger/logger.py`

 * *Files identical despite different names*

### Comparing `v3io-0.6.4/v3io.egg-info/PKG-INFO` & `v3io-0.6.5/v3io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v3io
-Version: 0.6.4
+Version: 0.6.5
 Summary: SDK for v3io
 Home-page: https://github.com/v3io/v3io-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `v3io-0.6.4/v3io.egg-info/SOURCES.txt` & `v3io-0.6.5/v3io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

