# Comparing `tmp/across_burstcube-0.0.8.tar.gz` & `tmp/across_burstcube-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "across_burstcube-0.0.8.tar", last modified: Mon Apr 29 21:39:55 2024, max compression
+gzip compressed data, was "across_burstcube-0.4.tar", last modified: Fri Apr 19 18:58:37 2024, max compression
```

## Comparing `across_burstcube-0.0.8.tar` & `across_burstcube-0.4.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:55.321914 across_burstcube-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:55.317914 across_burstcube-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:55.317914 across_burstcube-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-29 21:39:55.321914 across_burstcube-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:55.321914 across_burstcube-0.0.8/across_burstcube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-29 21:39:55.000000 across_burstcube-0.0.8/across_burstcube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-29 21:39:55.000000 across_burstcube-0.0.8/across_burstcube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:39:55.000000 across_burstcube-0.0.8/across_burstcube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-29 21:39:55.000000 across_burstcube-0.0.8/across_burstcube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 21:39:55.000000 across_burstcube-0.0.8/across_burstcube.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:55.321914 across_burstcube-0.0.8/across_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:55.321914 across_burstcube-0.0.8/across_client/across/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/across/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/across/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/across/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:55.321914 across_burstcube-0.0.8/across_client/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/base/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/base/coords.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/base/daterange.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/base/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/base/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:55.321914 across_burstcube-0.0.8/across_client/burstcube/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/burstcube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/burstcube/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/burstcube/toorequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/across_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-29 21:39:50.000000 across_burstcube-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 21:39:55.321914 across_burstcube-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.469876 across_burstcube-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.461876 across_burstcube-0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.461876 across_burstcube-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 18:58:32.000000 across_burstcube-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 18:58:32.000000 across_burstcube-0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 18:58:37.469876 across_burstcube-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-19 18:58:32.000000 across_burstcube-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_burstcube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/across/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/daterange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/burstcube/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/fov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/toorequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-19 18:58:32.000000 across_burstcube-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:58:37.469876 across_burstcube-0.4/setup.cfg
```

### Comparing `across_burstcube-0.0.8/.github/ISSUE_TEMPLATE.md` & `across_burstcube-0.4/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.8/.github/PULL_REQUEST_TEMPLATE.md` & `across_burstcube-0.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.8/.github/workflows/deploy.yml` & `across_burstcube-0.4/.github/workflows/deploy.yml`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
       - name: Checkout the repository
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Set up Python
-        uses: actions/setup-python@v5
+        uses: actions/setup-python@v4
         with:
           python-version: "3.11"
 
       - name: Git describe
         id: ghd
         uses: proudust/gh-describe@v2
 
@@ -30,15 +30,15 @@
           build
           --user
 
       - name: Build a binary wheel and a source tarball
         run: python3 -m build
 
       - name: Store the distribution packages
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
 
   publish-to-pypi:
     name: >-
       Publish Python 🐍 distribution 📦 to PyPI
@@ -49,13 +49,13 @@
     environment:
       name: pypi
       url: https://pypi.org/p/across-burstcube  # Replace <package-name> with your PyPI project name
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
     steps:
       - name: Download all the dists
-        uses: actions/download-artifact@v4
+        uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
       - name: Publish distribution 📦 to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `across_burstcube-0.0.8/.github/workflows/pylint.yml` & `across_burstcube-0.4/.github/workflows/pylint.yml`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 on: [push]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.9", "3.10", "3.11"]
     steps:
-    - uses: actions/checkout@v4
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v5
+      uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install flake8 mypy
     - name: Lint with flake8
```

### Comparing `across_burstcube-0.0.8/across_burstcube.egg-info/SOURCES.txt` & `across_burstcube-0.4/across_burstcube.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,9 +21,11 @@
 across_client/base/__init__.py
 across_client/base/common.py
 across_client/base/coords.py
 across_client/base/daterange.py
 across_client/base/schema.py
 across_client/base/user.py
 across_client/burstcube/__init__.py
+across_client/burstcube/constants.py
+across_client/burstcube/fov.py
 across_client/burstcube/schema.py
 across_client/burstcube/toorequest.py
```

### Comparing `across_burstcube-0.0.8/across_client/base/common.py` & `across_burstcube-0.4/across_client/base/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,120 +1,36 @@
 import json
 import warnings
-from typing import Type
+from pathlib import PosixPath
+from typing import Any, Dict, Optional, Tuple, Type
 
 import requests
 
 from ..constants import API_URL
-from ..functions import _tablefy
-from .schema import BaseSchema, FileHolder
+from ..functions import tablefy
+from .schema import BaseSchema
 
 
 class ACROSSBase:
     """
-    Mixin class for ACROSS API classes that provides a representation
-    of the API data. Includes support for Jupyter notebooks.
+    Base class for ACROSS API Classes including common methods for all API classes.
     """
 
-    @property
-    def parameters(self) -> dict:
-        """
-        Return parameters as dict
-
-        Returns
-        -------
-        dict
-            Dictionary of parameters
-        """
-        if hasattr(self, "model_dump"):
-            return {k: v for k, v in self.model_dump().items() if v is not None}
-        else:
-            return {k: v for k, v in self.__dict__.items() if v is not None}
-
-    @property
-    def _table(self) -> tuple:
-        """
-        Table with head showing results of the API query. Default table is to
-        show all fields and values, in a vertical two column table format.
-
-        Returns
-        -------
-        tuple
-            Tuple containing two lists, the header and the table data
-        """
-        entries = []
-        if hasattr(self, "model_dump"):
-            entries = [
-                [key, value]
-                for key, value in self.model_dump(
-                    mode="json", exclude_none=True
-                ).items()
-            ]
-        else:
-            entries = [[key, value] for key, value in self.__dict__.items()]
-        return ["Field", "Value"], entries
-
-    def _repr_html_(self) -> str:
-        """Return a HTML summary of the API data, for e.g. Jupyter.
-
-        Returns
-        -------
-        str
-            HTML summary of data
-        """
-        header, table = self._table
-
-        if len(table) > 0:
-            return _tablefy(table, header)
-        else:
-            return "No data"
-
-    def __repr__(self) -> str:
-        # print a string showing the API call and arguments with their values
-        # in a way that can be copied and pasted into a script
-        args = ",".join([f"{k}={v}" for k, v in self.parameters.items()])
-        return f"{self.__class__.__name__}({args})"
-
-
-class ACROSSEndPoint(ACROSSBase):
-    """
-    Base class for ACROSS API Classes including common methods for all API
-    endpoint classes.
-
-    Methods
-    -------
-    api_url(argdict)
-        URL for this API call.
-    get()
-        Perform a 'GET' submission to ACROSS API.
-    put()
-        Perform a 'PUT' submission to ACROSS API.
-    post()
-        Perform a 'POST' submission to ACROSS API.
-    delete()
-        Perform a 'DELETE' submission to ACROSS API.
-    validate_get()
-        Validate arguments for GET
-    validate_put()
-        Validate arguments for PUT
-    validate_post()
-        Validate arguments for POST
-    validate_del()
-        Validate arguments for DELETE
-
-    """
+    # Type hints
+    entries: list
 
     # API descriptors type hints
+    _schema: Type[BaseSchema]
     _get_schema: Type[BaseSchema]
     _put_schema: Type[BaseSchema]
     _post_schema: Type[BaseSchema]
     _del_schema: Type[BaseSchema]
 
     _mission: str
-    _api_name: str
+    _api_name: str = __name__
 
     def __getitem__(self, i):
         return self.entries[i]
 
     def api_url(self, argdict) -> str:
         """
         URL for this API call.
@@ -126,14 +42,51 @@
         """
         # If arguments has `id` in it, then put this in the path
         if "id" in argdict.keys() and argdict["id"] is not None:
             return f"{API_URL}{self._mission.lower()}/{self._api_name.lower()}/{argdict['id']}"
         return f"{API_URL}{self._mission.lower()}/{self._api_name.lower()}"
 
     @property
+    def schema(self) -> Any:
+        """Return pydantic schema for this API class
+
+        Returns
+        -------
+        object
+            Pydantic Schema
+        """
+        return self._schema.model_validate(self)
+
+    @property
+    def parameters(self) -> dict:
+        """
+        Return parameters as dict
+
+        Returns
+        -------
+        dict
+            Dictionary of parameters
+        """
+        return {k: v for k, v in self._schema.model_validate(self) if v is not None}
+
+    @parameters.setter
+    def parameters(self, params: dict):
+        """
+        Set API parameters from a given dict which is validated from self._schema
+
+        Parameters
+        ----------
+        params : dict
+            Dictionary of class parameters
+        """
+        for k, v in self._schema(**params):
+            if hasattr(self, k) and v is not None:
+                setattr(self, k, v)
+
+    @property
     def headers(self) -> dict:
         # If we have a api_token, then use this to authenticate
         if hasattr(self, "api_token"):
             headers = {"Authorization": f"Bearer {self.api_token}"}
         else:
             headers = {}
         return headers
@@ -152,31 +105,26 @@
         ------
         HTTPError
             Raised if GET doesn't return a 200 response.
         """
         if self.validate_get():
             # Create an array of parameters from the schema
             get_params = {
-                key: value
-                for key, value in self._get_schema.model_validate(self)
-                if key in self._get_schema.model_fields
+                key: value for key, value in self._get_schema.model_validate(self)
             }
-
             # Do the GET request
             req = requests.get(
                 self.api_url(get_params),
                 params=get_params,
                 headers=self.headers,
                 timeout=60,
             )
-
             if req.status_code == 200:
                 # Parse, validate and record values from returned API JSON
-                assert hasattr(self, "model_validate")
-                for k, v in self.model_validate(req.json()):
+                for k, v in self._schema.model_validate(req.json()):
                     setattr(self, k, v)
                 return True
             elif req.status_code == 404:
                 """Handle 404 errors gracefully, by issuing a warning"""
                 warnings.warn(req.json()["detail"])
             else:
                 # Raise an exception if the HTML response was not 200
@@ -208,24 +156,23 @@
                 self.api_url(del_params),
                 params=del_params,
                 headers=self.headers,
                 timeout=60,
             )
             if req.status_code == 200:
                 # Parse, validate and record values from returned API JSON
-                assert hasattr(self, "model_validate")
-                for k, v in self.model_validate(req.json()):
+                for k, v in self._schema.model_validate(req.json()):
                     setattr(self, k, v)
                 return True
             else:
                 # Raise an exception if the HTML response was not 200
                 req.raise_for_status()
         return False
 
-    def put(self) -> bool:
+    def put(self, payload={}) -> bool:
         """
         Perform a 'PUT' submission to ACROSS API. Used for pushing/replacing
         information.
 
         Returns
         -------
         bool
@@ -234,59 +181,66 @@
         Raises
         ------
         HTTPError
             Raised if PUT doesn't return a 201 response.
         """
 
         if self.validate_put():
-            # Make an object from this object, validated through the PUT Schema
-            put_object = self._put_schema.model_validate(self)
+            # Extract any files out of the arguments
+            files: Dict[str, Tuple[Optional[str], Any, str]] = {
+                key.replace("filename", "file"): (
+                    # Return either the existing filelike object, or open the file
+                    value.name,
+                    (
+                        getattr(self, key.replace("filename", "file"))
+                        if hasattr(self, key.replace("filename", "file"))
+                        else value.open("rb")
+                    ),
+                    "application/octet-stream",
+                )
+                for key, value in self._put_schema.model_validate(self)
+                if type(value) is PosixPath
+            }
 
-            # Extract all PUT parameters from this object
-            all_params = put_object.model_dump(mode="json", exclude_none=True)
+            # Extract all POST parameters from the schema
+            all_params = self._put_schema.model_validate(self).model_dump(
+                mode="json", exclude_none=True
+            )
 
-            # Extract query parameters, everything that isn't a dict or file
+            # Extract query parameters
             put_params = {
                 k: all_params[k]
                 for k in all_params
                 if not isinstance(all_params[k], dict)
             }
 
             # URL for this API call
             api_url = self.api_url(put_params)
             if "id" in put_params.keys():
                 put_params.pop("id")  # Remove id from query parameters
 
-            # Add any files and json data to files
-            files = dict()
+            # Add any json data to files
             for k in all_params:
-                if isinstance(getattr(put_object, k), FileHolder):
-                    files[k] = getattr(put_object, k).upload_file_tuple
-                elif isinstance(all_params[k], dict):
+                if isinstance(all_params[k], dict):
                     files[k] = (None, json.dumps(all_params[k]), "application/json")
 
             # Submit request
             req = requests.put(
                 api_url,
                 params=put_params,
                 headers=self.headers,
                 files=files,
                 timeout=60,
             )
 
             if req.status_code == 201:
                 # Parse, validate and record values from returned API JSON
-                assert hasattr(self, "model_validate")
-                for k, v in self.model_validate(req.json()):
+                for k, v in self._schema.model_validate(req.json()):
                     setattr(self, k, v)
                 return True
-            elif req.status_code == 304:
-                # No changes made
-                warnings.warn("Update identical to values on server. No changes made.")
-                return False
             else:
                 print("ERROR: ", req.status_code, req.json())
                 req.raise_for_status()
         return False
 
     def post(self) -> bool:
         """
@@ -300,57 +254,88 @@
 
         Raises
         ------
         HTTPError
             Raised if POST doesn't return a 201 response.
         """
         if self.validate_post():
-            # Make an object from this object, validated through the PUT Schema
-            post_object = self._post_schema.model_validate(self)
+            # Extract any files out of the arguments
+            files: Dict[str, Tuple[Optional[str], Any, str]] = {
+                key: (
+                    PosixPath(getattr(self, key + "name")).name
+                    if getattr(self, key) is not None
+                    else "healpix_file.fits",
+                    open(getattr(self, key + "name"), "rb"),
+                    "application/octet-stream",
+                )
+                if getattr(self, key) is None
+                and getattr(self, key + "name") is not None
+                else (
+                    PosixPath(getattr(self, key).name).name
+                    if getattr(self, key) is not None
+                    else None,
+                    getattr(self, key),
+                    "application/octet-stream",
+                )
+                for key, value in self._post_schema.model_validate(self)
+                if "_file" in key
+            }
 
-            # Extract all PUT parameters from this object
-            all_params = post_object.model_dump(mode="json", exclude_none=True)
+            # If files are gzipped, then set the content type to
+            # application/x-gzip
+            for key in files:
+                filename = files[key][0]
+                if isinstance(filename, str):
+                    if ".gz" in filename:
+                        files[key] = (
+                            files[key][0],
+                            files[key][1],
+                            "application/x-gzip",
+                        )
+
+            # Extract all POST parameters from the schema
+            all_params = self._post_schema.model_validate(self).model_dump(
+                mode="json", exclude_none=True
+            )
 
-            # Extract query parameters, everything that isn't a dict or file
+            # Extract query parameters
             post_params = {
                 k: all_params[k]
                 for k in all_params
                 if not isinstance(all_params[k], dict)
             }
 
-            # Add any files and json data to files
-            files = dict()
+            # Add any json data to files
             for k in all_params:
-                if isinstance(getattr(post_object, k), FileHolder):
-                    files[k] = getattr(post_object, k).upload_file_tuple
-                elif isinstance(all_params[k], dict):
+                if isinstance(all_params[k], dict):
                     files[k] = (None, json.dumps(all_params[k]), "application/json")
-
             # Submit request
             req = requests.post(
                 self.api_url(post_params),
                 params=post_params,
                 headers=self.headers,
                 files=files,
                 timeout=60,
             )
 
             if req.status_code == 201:
                 # Parse, validate and record values from returned API JSON
-                assert hasattr(self, "model_validate")
-                for k, v in self.model_validate(req.json()):
+                print(req.json())
+                for k, v in self._schema.model_validate(req.json()):
                     setattr(self, k, v)
                 return True
             elif req.status_code == 200:
                 warnings.warn(req.json()["detail"])
                 return False
             else:
-                print(f"{req.status_code}: {req.text}")
                 # Raise an exception if the HTML response was not 200
-                req.raise_for_status()
+                try:
+                    req.raise_for_status()
+                except requests.HTTPError as exc:
+                    print(f"HTTP Exception: {exc}: {req.json()['detail']}.")
 
         return False
 
     def validate_get(self) -> bool:
         """Validate arguments for GET
 
         Returns
@@ -417,7 +402,65 @@
         """
         if hasattr(self, "_del_schema"):
             self._del_schema.model_validate(self.__dict__)
         else:
             warnings.warn("DELETE not allowed for this class.")
             return False
         return True
+
+    @property
+    def _table(self) -> tuple:
+        """
+        Table with head showing results of the API query.
+
+        Returns
+        -------
+        tuple
+            Tuple containing two lists, the header and the table data
+        """
+        if hasattr(self, "entries") and len(self.entries) > 0:
+            header = self.entries[0]._table[0]
+            table = [t._table[1][0] for t in self.entries]
+        else:
+            # Start with arguments
+            if hasattr(self, "_get_schema"):
+                _parameters = list(self.parameters.keys())
+            else:
+                _parameters = []
+            _parameters += list(self.parameters.keys())
+            # Don't include client_id/client_secret in table
+            try:
+                _parameters.pop(_parameters.index("client_id"))
+                _parameters.pop(_parameters.index("client_secret"))
+            except ValueError:
+                pass
+
+            # Removed repeated values
+            _parameters = list(set(_parameters))
+
+            header = [par for par in _parameters]
+            table = []
+            for row in _parameters:
+                value = getattr(self, row)
+                table.append(value)
+            table = [table]
+        return header, table
+
+    def _repr_html_(self) -> str:
+        """Return a HTML summary of the API data, for e.g. Jupyter.
+
+        Returns
+        -------
+        str
+            HTML summary of data
+        """
+        header, table = self._table
+        if len(table) > 0:
+            return tablefy(table, header)
+        else:
+            return "No data"
+
+    def __repr__(self) -> str:
+        # print a string showing the API call and arguments with their values
+        # in a way that can be copied and pasted into a script
+        args = ",".join([f"{k}={v}" for k, v in self.parameters.items()])
+        return f"{self.__class__.__name__}({args})"
```

### Comparing `across_burstcube-0.0.8/across_client/base/coords.py` & `across_burstcube-0.4/across_client/base/coords.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     if type(coord) is Longitude or type(coord) is Latitude:
         return coord.value
     # Universal translator
     return float(coord)
 
 
 class ACROSSSkyCoord:
+    ra: float
+    dec: float
+
     @property
     def skycoord(self) -> SkyCoord:
         """Returns a string representation of the skycoord."""
         if self.ra is None or self.dec is None:
             return None
         else:
             return SkyCoord(self.ra, self.dec, unit="deg")
```

### Comparing `across_burstcube-0.0.8/across_client/base/daterange.py` & `across_burstcube-0.4/across_client/base/daterange.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.8/across_client/burstcube/schema.py` & `across_burstcube-0.4/across_client/burstcube/schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from datetime import datetime
 from enum import Enum
-from typing import Optional
+from io import IOBase
+from typing import List, Optional
 
-from pydantic import ConfigDict
+from pydantic import ConfigDict  # type: ignore
 
-from ..base.common import ACROSSBase
-from ..base.schema import (
-    BaseSchema,
-    FileHolder,
-    OptionalDateRangeSchema,
-    OptionalPositionSchema,
-)
+from ..base.schema import BaseSchema, OptionalDateRangeSchema, OptionalPositionSchema
 
 
 class TOOReason(str, Enum):
     """
     Reasons for rejecting TOO observations
 
     Attributes
@@ -68,49 +63,51 @@
     declined = "Declined"
     approved = "Approved"
     executed = "Executed"
     deleted = "Deleted"
     other = "Other"
 
 
-class BurstCubeTriggerInfo(BaseSchema, ACROSSBase):
+class BurstCubeTriggerInfo(BaseSchema):
     """
     Metadata schema for the BurstCube Target of Opportunity (TOO) request. Note
     that this schema is not strictly defined, keys are only suggested, and
     additional keys can be added as needed.
-
-    Attributes
-    ----------
-    trigger_name : Optional[str]
-        The name of the trigger.
-    trigger_mission : Optional[str]
-        The mission that triggered the TOO request.
-    trigger_instrument : Optional[str]
-        The instrument that triggered the TOO request.
-    trigger_id : Optional[str]
-        The ID of the trigger.
-    trigger_duration : Optional[float]
-        The duration of the trigger.
-    classification : Optional[str]
-        The classification of the trigger.
-    justification : Optional[str]
-        Textual justification for the TOO request.
     """
 
     trigger_name: Optional[str] = None
     trigger_mission: Optional[str] = None
     trigger_instrument: Optional[str] = None
     trigger_id: Optional[str] = None
     trigger_duration: Optional[float] = None
     classification: Optional[str] = None
     justification: Optional[str] = None
 
     model_config = ConfigDict(extra="allow")
 
 
+class BurstCubeTOOSchema(OptionalPositionSchema):
+    """
+    Schema describing a BurstCube TOO Request.
+    """
+
+    id: Optional[int] = None
+    created_by: str
+    created_on: datetime
+    modified_by: Optional[str] = None
+    modified_on: Optional[datetime] = None
+    trigger_time: datetime
+    trigger_info: BurstCubeTriggerInfo
+    exposure: int
+    offset: int
+    reject_reason: TOOReason = TOOReason.none
+    status: TOOStatus = TOOStatus.requested
+    too_info: str = ""
+
+
 class BurstCubeTOODelSchema(BaseSchema):
     """
     Schema for BurstCubeTOO DELETE API call.
 
     Attributes
     ----------
     id
@@ -125,15 +122,15 @@
     Schema to submit a TOO request for BurstCube.
     """
 
     trigger_time: datetime
     trigger_info: BurstCubeTriggerInfo
     exposure: int = 200
     offset: int = -50
-    healpix_file: Optional[FileHolder] = None
+    healpix_file: Optional[IOBase] = None
 
 
 class BurstCubeTOOGetSchema(BaseSchema):
     """
     Schema for BurstCubeTOO GET request.
     """
 
@@ -142,18 +139,31 @@
 
 class BurstCubeTOOPutSchema(BurstCubeTOOPostSchema):
     """
     Schema for BurstCubeTOO PUT request.
     """
 
     id: int
+    trigger_time: datetime
+    trigger_info: BurstCubeTriggerInfo
+    exposure: int = 200
+    offset: int = -50
     status: TOOStatus
+    healpix_file: Optional[IOBase] = None
 
 
 class BurstCubeTOORequestsGetSchema(OptionalDateRangeSchema):
     """
     Schema for GET requests to retrieve BurstCube Target of Opportunity (TOO) requests.
     """
 
     duration: Optional[float] = None
     limit: Optional[int] = None
     offset: Optional[int] = None
+
+
+class BurstCubeTOORequestsSchema(BaseSchema):
+    """
+    Schema for BurstCube TOO requests.
+    """
+
+    entries: List[BurstCubeTOOSchema]
```

### Comparing `across_burstcube-0.0.8/across_client/burstcube/toorequest.py` & `across_burstcube-0.4/across_client/burstcube/toorequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,212 +1,207 @@
+import io
+from dataclasses import dataclass, field
 from datetime import datetime
-from typing import Any, List, Optional
+from typing import Optional, Union
 
-from pydantic import Field, model_validator
+from pydantic import FilePath
 
-from across_client.base.coords import ACROSSSkyCoord
-
-from ..base.common import ACROSSEndPoint
-from ..base.schema import BaseSchema, FileHolder
+from ..across.resolve import ACROSSResolveName
+from ..base.common import ACROSSBase
+from .constants import MISSION
 from .schema import (
     BurstCubeTOOGetSchema,
     BurstCubeTOOPostSchema,
     BurstCubeTOOPutSchema,
     BurstCubeTOORequestsGetSchema,
+    BurstCubeTOORequestsSchema,
+    BurstCubeTOOSchema,
     BurstCubeTriggerInfo,
     TOOReason,
     TOOStatus,
 )
 
-MISSION = "BurstCube"
-
 
-class BurstCubeTOO(ACROSSEndPoint, ACROSSSkyCoord, BaseSchema):
+@dataclass
+class TOO(ACROSSBase, ACROSSResolveName):
     """
     Class representing a Target of Opportunity (TOO) request.
 
-    Parameters
+    Parameters:
     ----------
     api_token: str
         The api_token for login (optional).
-    trigger_time : Optional[datetime]
-        The time at which the BurstCube TOO request was triggered.
-    trigger_info : BurstCubeTriggerInfo
-        Metadata about the BurstCube TOO request.
-    exposure : int
-        The exposure time for the BurstCube TOO request.
-    offset : int
-        The offset from `trigger_time` that indicates when the BurstCube TOO
-        request dump time should begin. E.g. if offset is -50, the dump time
-        will begin 50 seconds before `trigger_time`.
-    healpix_filename : Optional[str]
-        The filename of the healpix file that represents the object localization
-        for the BurstCube TOO request.
+    trigger_time : datetime
+        The time of the trigger.
+    ra : Optional[float]
+        The right ascension of the target (optional).
+    dec : Optional[float]
+        The declination of the target (optional).
+    begin : datetime
+        The start time of the TOO observation.
+    end : datetime
+        The end time of the TOO observation.
+    exposure : float
+        The exposure time for the TOO observation.
+    offset : float
+        The offset for the TOO observation.
+    healpix_filename : Optional[FilePath]
+        The healpix filename that represents the object localization for the TOO. This should be a file
+        on disk.
     healpix_file : Union[io.BytesIO, io.BufferedReader, None]
-        The healpix file handle for the TOO observation, takes a file like
-        object.
-    name : str
-        The name of the celestial object. If given, the `ra` and `dec` values
-        will be set using the `Resolve` API end point.
+        The healpix file handle for the TOO observation, takes a file like object.
+    trigger_info : BurstCubeTriggerInfo
+        The trigger information for the TOO observation.
+    too_info : str
+        The information about the TOO observation.
+    status : str
+        The status of the TOO request.
+    id : id
+        The ID of the TOO request.
 
-    Attributes
+
+    Attributes:
     ----------
-    id : int
-        The ID of the TOO request.
     created_on : datetime
         The time at which the TOO request was made.
     created_by : str
         The user who made the TOO request.
     modified_on : datetime
         The time at which the TOO request was last modified.
     modified_by : str
         The user who modified the TOO request.
-    reject_reason : TOOReason
-        The reason for rejecting the BurstCube TOO request. Default is `none`.
-        Options are:
-            - saa
-            - earth_occult
-            - moon_occult
-            - sun_occult
-            - too_old
-            - other
-            - none
-    status : TOOStatus
-        The status of the BurstCube TOO request. Default is `requested`.
-        Options are:
-            - requested
-            - rejected
-            - declined
-            - approved
-            - executed
-            - other
+    reject_reason : str
+        The reason for the TOO request being rejected.
+    status : str
+        The status of the TOO request.
     too_info : str
-        Additional textual information about the BurstCube TOO request.
-    version : int
-        The version of the TOO request.
-    skycoord : SkyCoord
-        An astropy SkyCoord object representing the RA/Dec of the TOO.
+        The information about the TOO request.
+    id : str
+        The ID of the TOO request.
     """
 
-    # API definitions
-    _mission = MISSION
-    _api_name = "TOO"
-    _put_schema = BurstCubeTOOPutSchema
-    _post_schema = BurstCubeTOOPostSchema
-    _get_schema = BurstCubeTOOGetSchema
-    _del_schema = BurstCubeTOOGetSchema
-
-    # Schema parameters
+    api_token: Optional[str] = None
     id: Optional[int] = None
-    ra: Optional[float] = None
-    dec: Optional[float] = None
-    error_radius: Optional[float] = None
+    trigger_time: Optional[datetime] = None
     created_by: Optional[str] = None
     created_on: Optional[datetime] = None
     modified_by: Optional[str] = None
     modified_on: Optional[datetime] = None
-    trigger_time: Optional[datetime] = None
-    trigger_info: BurstCubeTriggerInfo = BurstCubeTriggerInfo()
-    exposure: int = 200
-    offset: int = -50
+    trigger_info: BurstCubeTriggerInfo = field(default_factory=BurstCubeTriggerInfo)
+    exposure: float = 200
+    offset: float = -50
+    too_info: str = ""
+    ra: Optional[float] = None
+    dec: Optional[float] = None
+    error_radius: Optional[float] = None
+    healpix_filename: Optional[FilePath] = None
+    healpix_file: Union[io.BytesIO, io.BufferedReader, None] = None
     reject_reason: TOOReason = TOOReason.none
     status: TOOStatus = TOOStatus.requested
-    too_info: str = ""
-    healpix_filename: Optional[str] = None
-    version: Optional[int] = None
 
-    # Local parameters
-    healpix_file: Optional[FileHolder] = Field(exclude=True, default=None)
-    api_token: Optional[str] = Field(exclude=True, default=None)
+    # API definitions
+    _mission = MISSION
+    _api_name = "TOO"
+    _schema = BurstCubeTOOSchema
+    _put_schema = BurstCubeTOOPutSchema
+    _post_schema = BurstCubeTOOPostSchema
+    _get_schema = BurstCubeTOOGetSchema
+    _del_schema = BurstCubeTOOGetSchema
 
-    # Aliases
-    def submit(self) -> bool:
-        return self.post()
+    @classmethod
+    def submit_too(cls, **kwargs):
+        """
+        Submit a TOO request.
+        """
+        for k, a in kwargs.items():
+            if k in cls._post_schema.model_fields.keys():
+                setattr(cls, k, a)
 
-    def update(self) -> bool:
-        return self.put()
+        if cls.validate_post():
+            cls.post()
+
+    @property
+    def _table(self):
+        return (
+            [
+                "TOO ID",
+                "Submitted",
+                "Submitter",
+                "Trigger Time",
+                "Mission",
+                "Instrument",
+                "ID",
+                "Status",
+                "Reason",
+            ],
+            [
+                [
+                    self.id,
+                    self.created_on,
+                    self.created_by,
+                    self.trigger_time,
+                    self.trigger_info.trigger_mission,
+                    self.trigger_info.trigger_instrument,
+                    self.trigger_info.trigger_id,
+                    self.status.value,
+                    self.reject_reason.value,
+                ]
+            ],
+        )
 
 
-class TOORequests(ACROSSEndPoint, BurstCubeTOORequestsGetSchema):
+class TOORequests(ACROSSBase):
     """
     Represents a Targer of Opportunity (TOO) request.
 
-    Parameters
+    Attributes
     ----------
-    trigger_time : datetime
-        Trigger time of the TOO request.
     begin : datetime
         The start time of the observation.
     end : datetime
         The end time of the observation.
     limit : int
-        The maximum number of TOOs to return.
-    offset : int
-        The limit offset for fetching TOOs.
-
-    Attributes
-    ----------
+        The maximum number of entries for the observation.
+    trigger_time : datetime
+        The time at which the observation should be triggered.
     entries : list
         The list of entries for the observation.
-
-    Methods
-    -------
-    get_toos
-        Fetch TOOs based on various criteria.
-
     """
 
-    # API definitions
     _mission = MISSION
     _api_name = "TOO"
+    _schema = BurstCubeTOORequestsSchema
     _get_schema = BurstCubeTOORequestsGetSchema
-    # Local parameters
-    trigger_time: Optional[datetime] = None
-
-    entries: List[BurstCubeTOO] = []
 
-    def __len__(self):
-        return len(self.entries)
+    def __init__(self, **kwargs):
+        self.entries = []
+        self.begin = None
+        self.end = None
+        self.limit = None
+        for k, a in kwargs.items():
+            if k in self._get_schema.model_fields.keys():
+                setattr(self, k, a)
+
+        # As this is a GET only class, we can validate and get the data
+        if self.validate_get():
+            self.get()
 
-    def __getitem__(self, i):
-        return self.entries[i]
+        # Convert the entries to a list of TOO objects
+        self.entries = [TOO(**entry.__dict__) for entry in self.entries]
 
     def by_id(self, id):
         """
-        Return a TOO from the fetched list by the ID number.
-
-        Parameters
-        ----------
-        id : int
-            The ID of the TOO request.
-
-        Returns
-        -------
-        BurstCubeTOO
-            The TOO request.
+        Get a TOO request by ID.
         """
         for entry in self.entries:
             if entry.id == id:
                 return entry
 
-    @model_validator(mode="before")
-    @classmethod
-    def _trigger_time_validator(cls, data: Any) -> Any:
-        if isinstance(data, dict):
-            if "trigger_time" in data and data["trigger_time"] is not None:
-                data["begin"] = data["trigger_time"]
-                data["end"] = data["trigger_time"]
-        return data
-
     @property
     def _table(self):
-        entries = [
-            BurstCubeTOO.model_validate_json(entry.model_dump_json())
-            for entry in self.entries
-        ]
         return (
             [
                 "TOO ID",
                 "Submitted",
                 "Submitter",
                 "Trigger Time",
                 "Mission",
@@ -223,137 +218,17 @@
                     entry.trigger_time,
                     entry.trigger_info.trigger_mission,
                     entry.trigger_info.trigger_instrument,
                     entry.trigger_info.trigger_id,
                     entry.status.value,
                     entry.reject_reason.value,
                 ]
-                for entry in entries
+                for entry in self.entries
             ],
         )
 
-    @classmethod
-    def get_too_requests(cls, *args, **kwargs):
-        """
-        Fetch TOOs based on various criteria. Passing no arguments will fetch
-        all. TOOs are returned in reverse order of receipt time.
-
-        Parameters
-        ----------
-        trigger_time : datetime
-            Trigger time of the TOO request to search for. Only returns trigger
-            with this exact trigger time.
-        begin : datetime
-            Beginning trigger time to search.
-        end : datetime
-            Ending trigger time to search.
-        limit : int
-            The maximum number of TOOs to return.
-        offset : int
-            The limit offset for fetching TOOs. Provides pagination support.
-            I.e. if limit is 10 and offset is 10, then the second page of 10
-            TOOs will be returned.
-
-        Returns
-        ----------
-        TOORequests
-            The list of entries for the observation.
-        """
-        too_requests = cls(*args, **kwargs)
-        too_requests.get()
-        return too_requests
-
-
-def get_too_by_id(id: int) -> BurstCubeTOO:
-    """
-    Get a TOO request by ID.
-
-    Parameters
-    ----------
-    id : int
-        The ID of the TOO request.
-    api_token : str
-        The API token for the user.
-
-    Returns
-    -------
-    BurstCubeTOO
-        The TOO request.
-    """
-    too = BurstCubeTOO(id=id)
-    too.get()
-    return too
-
-
-def get_too_by_trigger_time(trigger_time: datetime) -> Optional[BurstCubeTOO]:
-    """
-    Get a TOO request by timestamp.
-
-    Parameters
-    ----------
-    timestamp : str
-        The timestamp of the TOO request.
-    api_token : str
-        The API token for the user.
-
-    Returns
-    -------
-    BurstCubeTOO
-        The TOO request.
-    """
-    too = TOORequests(trigger_time=trigger_time)
-    too.get()
-    if len(too) > 0:
-        return too[0]
-    return None
-
-
-def delete_too_by_id(id: Optional[int]) -> bool:
-    """
-    Delete a TOO request by ID.
-
-    Parameters
-    ----------
-    id : int
-        The ID of the TOO request.
-    api_token : str
-        The API token for the user.
-
-    Returns
-    -------
-    bool
-        True if the request was deleted.
-    """
-    if id is None:
-        return False
-    too = BurstCubeTOO(id=id)
-    return too.delete()
-
-
-def delete_too_by_trigger_time(trigger_time: datetime) -> bool:
-    """
-    Delete a TOO request by timestamp.
-
-    Parameters
-    ----------
-    timestamp : str
-        The timestamp of the TOO request.
-    api_token : str
-        The API token for the user.
-
-    Returns
-    -------
-    bool
-        True if the request was deleted.
-    """
-    too = TOORequests(trigger_time=trigger_time)
-    too.get()
-    # There will only be 0 or 1 entries
-    for entry in too.entries:
-        return delete_too_by_id(entry.id)
-    return False
-
 
 # Alias
-TOO = BurstCubeTOO
+BurstCubeTOO = TOO
 BurstCubeTOORequests = TOORequests
-get_too_requests = TOORequests.get_too_requests
+submit_too = TOO.submit_too
+burstcube_submit_too = TOO.submit_too
```

### Comparing `across_burstcube-0.0.8/across_client/functions.py` & `across_burstcube-0.4/across_client/functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import re
 import warnings
-from datetime import date, datetime, timezone
+from datetime import date, datetime, timedelta, timezone
 from typing import Optional, Union
 
+import astropy.units as u  # type: ignore
 import numpy as np
-from astropy.time import Time  # type: ignore
+from astropy.time import Time, TimeDelta  # type: ignore
+from astropy.units import Quantity
 from dateutil import parser
 
 
-def _tablefy(table: list, header: Optional[list] = None) -> str:
+def tablefy(table: list, header: Optional[list] = None) -> str:
     """Simple HTML table generator
 
     Parameters
     ----------
     table : list
         Data for table
     header : list, optional
@@ -44,15 +46,58 @@
 
 # Regex for matching date, time and datetime strings
 DATE_REGEX = r"^[0-2]\d{3}-(0?[1-9]|1[012])-([0][1-9]|[1-2][0-9]|3[0-1])?$"
 ISO8601_REGEX = r"^([\+-]?\d{4}(?!\d{2}\b))((-?)((0[1-9]|1[0-2])(\3([12]\d|0[1-9]|3[01]))?|W([0-4]\d|5[0-2])(-?[1-7])?|(00[1-9]|0[1-9]\d|[12]\d{2}|3([0-5]\d|6[1-6])))([T\s]((([01]\d|2[0-3])((:?)[0-5]\d)?|24\:?00)([\.,]\d+(?!:))?)?(\17[0-5]\d([\.,]\d+)?)?([zZ]|([\+-])([01]\d|2[0-3]):?([0-5]\d)?)?)?)?$"
 DATETIME_REGEX = r"^[0-2]\d{3}-(0?[1-9]|1[012])-([0][1-9]|[1-2][0-9]|3[0-1])[\sT]([0-9]:|[0-1][0-9]:|2[0-3]:)[0-5][0-9]:[0-5][0-9]+(\.\d+)?$"
 
 
-def _convert_to_dt(value: Union[str, date, datetime, Time]) -> Optional[datetime]:
+def convert_timedelta(
+    length: Union[str, float, timedelta, TimeDelta, Quantity, None], units=u.day
+) -> timedelta:
+    """Convert various timedelta formats to swiftdatetime or datetime
+
+    Parameters
+    ----------
+    length : Union[str, float, timedelta, TimeDelta, Quantity, None]
+        Value to be converted.
+    units : astropy.units.Quantity, optional
+        Unit to use if float/int given. Default is days.
+
+    Returns
+    -------
+    datetime.timedelta
+        Returned timedelta object.
+
+    Raises
+    ------
+    TypeError
+        Raised if incorrect format is given for conversion.
+    """
+
+    if units == u.day:
+        divisor = 86400.0
+    else:
+        divisor = 1.0
+    if type(length) is Quantity:
+        length = length.to(u.day).value
+    elif type(length) is timedelta:
+        length = length.total_seconds() / divisor
+    elif type(length) is TimeDelta:
+        length = length.to_datetime().total_seconds() / divisor  # type: ignore
+    else:
+        try:
+            length = float(length)  # type: ignore
+        except ValueError:
+            raise TypeError(
+                f"Length of time should be given as a datetime.timedelta, astropy TimeDelta, astropy quantity or as a number of {units}"
+            )
+    return timedelta(days=length)  # type: ignore
+
+
+def convert_to_dt(value: Union[str, date, datetime, Time]) -> Optional[datetime]:
     """Convert various date formats to datetime
 
     Parameters
     ----------
     value : Union[str, date, datetime, Time]
         Value to be converted.
```

