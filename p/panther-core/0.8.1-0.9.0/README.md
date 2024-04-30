# Comparing `tmp/panther_core-0.8.1.tar.gz` & `tmp/panther_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther_core-0.8.1.tar", last modified: Thu Feb 29 20:34:03 2024, max compression
+gzip compressed data, was "panther_core-0.9.0.tar", last modified: Tue Apr 23 17:06:16 2024, max compression
```

## Comparing `panther_core-0.8.1.tar` & `panther_core-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 20:34:03.215434 panther_core-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-02-29 20:33:21.000000 panther_core-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-29 20:33:21.000000 panther_core-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-29 20:34:03.215434 panther_core-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-02-29 20:33:21.000000 panther_core-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 20:34:03.215434 panther_core-0.8.1/panther_core/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/enriched_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 20:34:03.215434 panther_core-0.8.1/panther_core/exec/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/exec/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/exec/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/exec/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    18869 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/immutable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    31265 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 20:34:03.215434 panther_core-0.8.1/panther_core/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/snapshots/_func.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/testing_exec_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-02-29 20:33:21.000000 panther_core-0.8.1/panther_core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 20:34:03.215434 panther_core-0.8.1/panther_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-29 20:34:03.000000 panther_core-0.8.1/panther_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-29 20:34:03.000000 panther_core-0.8.1/panther_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 20:34:03.000000 panther_core-0.8.1/panther_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 20:34:03.000000 panther_core-0.8.1/panther_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 20:34:03.000000 panther_core-0.8.1/panther_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-29 20:33:48.000000 panther_core-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-29 20:34:03.215434 panther_core-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-02-29 20:33:21.000000 panther_core-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:06:16.589376 panther_core-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-23 17:05:12.000000 panther_core-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-23 17:05:12.000000 panther_core-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-23 17:06:16.589376 panther_core-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-23 17:05:12.000000 panther_core-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:06:16.589376 panther_core-0.9.0/panther_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/enriched_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:06:16.589376 panther_core-0.9.0/panther_core/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/exec/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/exec/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/exec/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18869 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31266 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:06:16.589376 panther_core-0.9.0/panther_core/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/snapshots/_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12390 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/testing_exec_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-23 17:05:12.000000 panther_core-0.9.0/panther_core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:06:16.589376 panther_core-0.9.0/panther_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-23 17:06:16.000000 panther_core-0.9.0/panther_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-23 17:06:16.000000 panther_core-0.9.0/panther_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:06:16.000000 panther_core-0.9.0/panther_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 17:06:16.000000 panther_core-0.9.0/panther_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 17:06:16.000000 panther_core-0.9.0/panther_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-23 17:06:02.000000 panther_core-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 17:06:16.589376 panther_core-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-23 17:05:12.000000 panther_core-0.9.0/setup.py
```

### Comparing `panther_core-0.8.1/LICENSE.txt` & `panther_core-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/PKG-INFO` & `panther_core-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: panther_core
-Version: 0.8.1
+Version: 0.9.0
 Summary: Panther core library
 Home-page: https://github.com/panther-labs/panther_core
-Download-URL: https://github.com/panther-labs/panther_core/archive/refs/tags/v0.8.1.tar.gz
+Download-URL: https://github.com/panther-labs/panther_core/archive/refs/tags/v0.9.0.tar.gz
 Author: Panther Labs Inc
 Author-email: pypi@runpanther.io
 License: AGPL-3.0
 Keywords: Security,CLI
 Classifier: Topic :: Security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `panther_core-0.8.1/README.md` & `panther_core-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -11,57 +11,72 @@
 
 <p align="center">
   <a href="https://circleci.com/gh/panther-labs/panther_core"><img src="https://circleci.com/gh/panther-labs/panther_core.svg?style=svg" alt="CircleCI"/></a>
 </p>
 
 ---
 
-`panther_core` is a Python library for Panther Detections. See the [Panther documentation](https://docs.runpanther.io/quick-start) for more details on Panther.
+`panther_core` is a Python library for Panther Detections. See the
+[Panther documentation](https://docs.runpanther.io/quick-start) for more details
+on Panther.
 
 # Installation
 
 Install simply with pip:
 
 ```shell
-$ pip3 install panther_core
+pip3 install panther_core
 ```
 
 ## Build From Source
 
-If you'd prefer instead to run from source for development reasons, first setup your environment:
+If you'd prefer instead to run from source for development reasons, first setup
+your environment:
 
 ```shell
-$ make install-pipenv
-$ make install
-$ pipenv run -- pip3 install -e .
+make install-pipenv
+make install
+pipenv run -- pip3 install -e .
 ```
 
-If you would rather use the `panther_core` outside of the virtual environment, install it  directly:
+If you would rather use the `panther_core` outside of the virtual environment,
+install it directly:
 
 ```shell
-$ make deps
-$ pip3 install -e .
+make deps
+pip3 install -e .
 ```
 
 ## Testing
 
 Follow the build steps above, then run:
 
 ```shell
-$ make test
+make test
 ```
 
 ## Publishing
 
-1. Bump the minor or patch version in `setup.py` in a pull request and merge. Minor versions for weekly releases, patch versions for updates to that release.
-2. Pull and checkout the latest main branch locally and tag it with the version `git tag vX.X.X`, and `git push --tags` 
-3. Create a GitHub release in the UI with the appropriate tag. 
+1. Bump the minor or patch version in `setup.py` in a pull request and merge.
+   Minor versions for weekly releases, patch versions for updates to that
+   release.
+2. Pull and checkout the latest main branch locally and tag it with the version
+   `git tag vX.X.X`, and `git push --tags`
+3. Create a GitHub release in the UI with the appropriate tag.
 4. If not installed, download twine `pip3 install twine`
-5. With main still checked out, run `make publish`. Use [these](https://start.1password.com/open/i?a=MQH6SE7BG5BQRKT3KEXZS537RU&v=bkez2qslmvtjp5hpy3et7pquhy&i=3ijfwjsdolp6wltzikfpzyts3i&h=panther-labs.1password.com) PyPi credentials in 1Password, username: `__token__`, password is the api token.
+5. With main still checked out, run `make publish`. Use
+   [these](https://start.1password.com/open/i?a=MQH6SE7BG5BQRKT3KEXZS537RU&v=bkez2qslmvtjp5hpy3et7pquhy&i=3ijfwjsdolp6wltzikfpzyts3i&h=panther-labs.1password.com)
+   PyPi credentials in 1Password, username: `__token__`, password is the api
+   token.
 
 # Contributing
 
-We welcome all contributions! Please read the [contributing guidelines](https://github.com/panther-labs/panther_core/blob/master/CONTRIBUTING.md) before submitting pull requests. [Instructions for opening a pull request](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) from your fork of the repo can be found on Github.
+We welcome all contributions! Please read the
+[contributing guidelines](https://github.com/panther-labs/panther_core/blob/master/CONTRIBUTING.md)
+before submitting pull requests.
+[Instructions for opening a pull request](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
+from your fork of the repo can be found on Github.
 
 ## License
 
-This repository is licensed under the AGPL-3.0 [license](https://github.com/panther-labs/panther_core/blob/master/LICENSE).
+This repository is licensed under the AGPL-3.0
+[license](https://github.com/panther-labs/panther_core/blob/master/LICENSE).
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
                           ************ PPaanntthheerr CCoorree ************
                       Python core for Panther detections
                           _D_o_c_u_m_e_n_t_a_t_i_o_n | _Q_u_i_c_k_ _S_t_a_r_t
                                   _[_C_i_r_c_l_e_C_I_]
 --- `panther_core` is a Python library for Panther Detections. See the [Panther
 documentation](https://docs.runpanther.io/quick-start) for more details on
-Panther. # Installation Install simply with pip: ```shell $ pip3 install
+Panther. # Installation Install simply with pip: ```shell pip3 install
 panther_core ``` ## Build From Source If you'd prefer instead to run from
-source for development reasons, first setup your environment: ```shell $ make
-install-pipenv $ make install $ pipenv run -- pip3 install -e . ``` If you
-would rather use the `panther_core` outside of the virtual environment, install
-it directly: ```shell $ make deps $ pip3 install -e . ``` ## Testing Follow the
-build steps above, then run: ```shell $ make test ``` ## Publishing 1. Bump the
-minor or patch version in `setup.py` in a pull request and merge. Minor
-versions for weekly releases, patch versions for updates to that release. 2.
-Pull and checkout the latest main branch locally and tag it with the version
-`git tag vX.X.X`, and `git push --tags` 3. Create a GitHub release in the UI
-with the appropriate tag. 4. If not installed, download twine `pip3 install
-twine` 5. With main still checked out, run `make publish`. Use [these](https://
+source for development reasons, first setup your environment: ```shell make
+install-pipenv make install pipenv run -- pip3 install -e . ``` If you would
+rather use the `panther_core` outside of the virtual environment, install it
+directly: ```shell make deps pip3 install -e . ``` ## Testing Follow the build
+steps above, then run: ```shell make test ``` ## Publishing 1. Bump the minor
+or patch version in `setup.py` in a pull request and merge. Minor versions for
+weekly releases, patch versions for updates to that release. 2. Pull and
+checkout the latest main branch locally and tag it with the version `git tag
+vX.X.X`, and `git push --tags` 3. Create a GitHub release in the UI with the
+appropriate tag. 4. If not installed, download twine `pip3 install twine` 5.
+With main still checked out, run `make publish`. Use [these](https://
 start.1password.com/open/
 i?a=MQH6SE7BG5BQRKT3KEXZS537RU&v=bkez2qslmvtjp5hpy3et7pquhy&i=3ijfwjsdolp6wltzikfpzyts3i&h=panther-
 labs.1password.com) PyPi credentials in 1Password, username: `__token__`,
 password is the api token. # Contributing We welcome all contributions! Please
 read the [contributing guidelines](https://github.com/panther-labs/
 panther_core/blob/master/CONTRIBUTING.md) before submitting pull requests.
 [Instructions for opening a pull request](https://docs.github.com/en/github/
```

### Comparing `panther_core-0.8.1/panther_core/data_model.py` & `panther_core-0.9.0/panther_core/data_model.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/detection.py` & `panther_core-0.9.0/panther_core/detection.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/enriched_event.py` & `panther_core-0.9.0/panther_core/enriched_event.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
+
 from collections import OrderedDict
 from collections.abc import Mapping
 from functools import reduce
 from typing import Any, List, Optional, Sequence, Union
 
 from dateutil import parser as dateparser
 
@@ -38,26 +39,45 @@
         Args:
             event: Dictionary representing the event.
             data_model: the data model used for the LogType associated with this event
         """
         super().__init__(event)
         self.data_model = data_model
 
-    def udm(self, key: str) -> Any:
-        """Converts standard data model field to logtype field"""
-        self._validate()
-        # access values via standardized fields
-        match = self._get_json_path(key)
-        if match:
-            return self._ensure_immutable(match.value)
-        method = self._get_method(key)
-        if method:
-            return self._ensure_immutable(method(self._ensure_immutable(self._container)))
-        # no matches, return None by default
-        return None
+    def udm(self, *key: str, default: Any = None) -> Any:
+        """
+        udm operates in two modes
+
+        Mode 1: Data Model Access
+        If a single key is provided it will check to see if it exists on the data
+        model mapping. If a mapping is not found it operates in Mode 2.
+
+        Mode 2: p_udm access
+        If there was no match against the data model it checks against the p_udm field.
+        If there was no match against the p_udm field it will check on the event itself.
+        If all other conditions are exhausted the default value is utilized as the return value
+        """
+        if len(key) == 1 and self.data_model:
+            match = self._get_json_path(key[0])
+            if match:
+                return self._ensure_immutable(match.value)
+            method = self._get_method(key[0])
+            if method:
+                return self._ensure_immutable(method(self._ensure_immutable(self._container)))
+
+        pieces = list(key)
+        if len(pieces) > 0:
+            pieces.insert(0, "p_udm")
+            result = self.deep_get(*tuple(pieces))
+            if not result:
+                result = self.deep_get(*list(key))
+            if result:
+                return result
+        # no matches, return default
+        return default
 
     def udm_path(self, key: str) -> Optional[str]:
         """Returns the JSON path or method name for the mapped field"""
         self._validate()
         # access values via standardized fields
         match = self._get_json_path(key)
         if match:
```

### Comparing `panther_core-0.8.1/panther_core/exceptions.py` & `panther_core-0.9.0/panther_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/exec/__init__.py` & `panther_core-0.9.0/panther_core/exec/__init__.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/exec/common.py` & `panther_core-0.9.0/panther_core/exec/common.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/exec/results.py` & `panther_core-0.9.0/panther_core/exec/results.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/exec/task.py` & `panther_core-0.9.0/panther_core/exec/task.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/filter.py` & `panther_core-0.9.0/panther_core/filter.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/immutable.py` & `panther_core-0.9.0/panther_core/immutable.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/policy.py` & `panther_core-0.9.0/panther_core/policy.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/rule.py` & `panther_core-0.9.0/panther_core/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
+
 import contextlib
 import json
 import logging
 import os
 import tempfile
 from abc import ABC, abstractmethod
 from collections.abc import Mapping
```

### Comparing `panther_core-0.8.1/panther_core/snapshots/_func.py` & `panther_core-0.9.0/panther_core/snapshots/_func.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/testing.py` & `panther_core-0.9.0/panther_core/testing.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/testing_exec_output.py` & `panther_core-0.9.0/panther_core/testing_exec_output.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core/util.py` & `panther_core-0.9.0/panther_core/util.py`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/panther_core.egg-info/PKG-INFO` & `panther_core-0.9.0/panther_core.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: panther_core
-Version: 0.8.1
+Version: 0.9.0
 Summary: Panther core library
 Home-page: https://github.com/panther-labs/panther_core
-Download-URL: https://github.com/panther-labs/panther_core/archive/refs/tags/v0.8.1.tar.gz
+Download-URL: https://github.com/panther-labs/panther_core/archive/refs/tags/v0.9.0.tar.gz
 Author: Panther Labs Inc
 Author-email: pypi@runpanther.io
 License: AGPL-3.0
 Keywords: Security,CLI
 Classifier: Topic :: Security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `panther_core-0.8.1/panther_core.egg-info/SOURCES.txt` & `panther_core-0.9.0/panther_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panther_core-0.8.1/requirements.txt` & `panther_core-0.9.0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 -i https://pypi.org/simple
-botocore==1.31.61; python_version >= '3.7'
-certifi==2021.10.8
+botocore==1.34.78; python_version >= '3.8'
+certifi==2023.7.22; python_version >= '3.6'
 chardet==4.0.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
 contextlib2==0.6.0.post1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 decorator==5.1.1; python_version >= '3.5'
 idna==3.3; python_version >= '3.5'
 jmespath==1.0.0; python_version >= '3.7'
 jsonpath-ng==1.5.3
 ply==3.11
 python-dateutil==2.8.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 s3transfer==0.5.2; python_version >= '3.6'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 types-python-dateutil==2.8.19
-urllib3==1.26.9; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'
+urllib3==1.26.18; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
```

### Comparing `panther_core-0.8.1/setup.py` & `panther_core-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from distutils.core import setup
 
-VERSION = "0.8.1"
+VERSION = "0.9.0"
 
 install_requires = [
     'jsonpath-ng',
 ]
 
 with open('requirements.txt') as f:
     dependencies_with_versions = []
```

