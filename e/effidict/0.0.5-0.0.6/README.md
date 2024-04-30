# Comparing `tmp/effidict-0.0.5.tar.gz` & `tmp/effidict-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "effidict-0.0.5.tar", last modified: Mon Apr 29 10:28:18 2024, max compression
+gzip compressed data, was "effidict-0.0.6.tar", last modified: Tue Apr 30 15:30:06 2024, max compression
```

## Comparing `effidict-0.0.5.tar` & `effidict-0.0.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:18.130892 effidict-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:18.122892 effidict-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:18.122892 effidict-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-29 10:28:06.000000 effidict-0.0.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-29 10:28:06.000000 effidict-0.0.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-29 10:28:06.000000 effidict-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-29 10:28:06.000000 effidict-0.0.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-29 10:28:06.000000 effidict-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-29 10:28:18.130892 effidict-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 10:28:06.000000 effidict-0.0.5/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)    87532 2024-04-29 10:28:06.000000 effidict-0.0.5/comparative_notebook.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:18.122892 effidict-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 10:28:06.000000 effidict-0.0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:28:06.000000 effidict-0.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:18.122892 effidict-0.0.5/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:18.126892 effidict-0.0.5/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-04-29 10:28:06.000000 effidict-0.0.5/docs/source/_static/logo_effidict.png
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-29 10:28:06.000000 effidict-0.0.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-29 10:28:06.000000 effidict-0.0.5/docs/source/effidict.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-29 10:28:06.000000 effidict-0.0.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-29 10:28:06.000000 effidict-0.0.5/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:18.126892 effidict-0.0.5/effidict/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 10:28:06.000000 effidict-0.0.5/effidict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-04-29 10:28:06.000000 effidict-0.0.5/effidict/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 10:28:18.000000 effidict-0.0.5/effidict/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-29 10:28:06.000000 effidict-0.0.5/effidict/db_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-29 10:28:06.000000 effidict-0.0.5/effidict/lru_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:18.130892 effidict-0.0.5/effidict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-29 10:28:18.000000 effidict-0.0.5/effidict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-29 10:28:18.000000 effidict-0.0.5/effidict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:28:18.000000 effidict-0.0.5/effidict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 10:28:18.000000 effidict-0.0.5/effidict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 10:28:18.000000 effidict-0.0.5/effidict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:18.126892 effidict-0.0.5/images/
--rw-r--r--   0 runner    (1001) docker     (127)    59857 2024-04-29 10:28:06.000000 effidict-0.0.5/images/comparative.png
--rw-r--r--   0 runner    (1001) docker     (127)    51212 2024-04-29 10:28:06.000000 effidict-0.0.5/images/custom_100.png
--rw-r--r--   0 runner    (1001) docker     (127)    55710 2024-04-29 10:28:06.000000 effidict-0.0.5/images/custom_1000.png
--rw-r--r--   0 runner    (1001) docker     (127)    45813 2024-04-29 10:28:06.000000 effidict-0.0.5/images/custom_1000_db.png
--rw-r--r--   0 runner    (1001) docker     (127)    45280 2024-04-29 10:28:06.000000 effidict-0.0.5/images/custom_1000_db_10.png
--rw-r--r--   0 runner    (1001) docker     (127)   195221 2024-04-29 10:28:06.000000 effidict-0.0.5/images/logo_effidict.png
--rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-04-29 10:28:06.000000 effidict-0.0.5/images/logo_effidict_no_bg.png
--rw-r--r--   0 runner    (1001) docker     (127)    55050 2024-04-29 10:28:06.000000 effidict-0.0.5/images/named_tuple.png
--rw-r--r--   0 runner    (1001) docker     (127)    55777 2024-04-29 10:28:06.000000 effidict-0.0.5/images/normal_dict.png
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-29 10:28:06.000000 effidict-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:28:18.130892 effidict-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:28:18.130892 effidict-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:28:06.000000 effidict-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-29 10:28:06.000000 effidict-0.0.5/tests/test_db_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-29 10:28:06.000000 effidict-0.0.5/tests/test_lru_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-29 10:28:06.000000 effidict-0.0.5/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.269612 effidict-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.261613 effidict-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.265612 effidict-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-30 15:29:56.000000 effidict-0.0.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-30 15:29:56.000000 effidict-0.0.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-30 15:29:56.000000 effidict-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-30 15:29:56.000000 effidict-0.0.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-30 15:29:56.000000 effidict-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-30 15:30:06.269612 effidict-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-30 15:29:56.000000 effidict-0.0.6/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)    87532 2024-04-30 15:29:56.000000 effidict-0.0.6/comparative_notebook.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.265612 effidict-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.265612 effidict-0.0.6/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.265612 effidict-0.0.6/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/source/_static/logo_effidict.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/source/effidict.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 15:29:56.000000 effidict-0.0.6/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.265612 effidict-0.0.6/effidict/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 15:29:56.000000 effidict-0.0.6/effidict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-30 15:29:56.000000 effidict-0.0.6/effidict/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-30 15:29:56.000000 effidict-0.0.6/effidict/db_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-30 15:29:56.000000 effidict-0.0.6/effidict/lru_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.269612 effidict-0.0.6/effidict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 15:30:06.000000 effidict-0.0.6/effidict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.269612 effidict-0.0.6/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    59857 2024-04-30 15:29:56.000000 effidict-0.0.6/images/comparative.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51212 2024-04-30 15:29:56.000000 effidict-0.0.6/images/custom_100.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55710 2024-04-30 15:29:56.000000 effidict-0.0.6/images/custom_1000.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45813 2024-04-30 15:29:56.000000 effidict-0.0.6/images/custom_1000_db.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45280 2024-04-30 15:29:56.000000 effidict-0.0.6/images/custom_1000_db_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)   195221 2024-04-30 15:29:56.000000 effidict-0.0.6/images/logo_effidict.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-04-30 15:29:56.000000 effidict-0.0.6/images/logo_effidict_no_bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55050 2024-04-30 15:29:56.000000 effidict-0.0.6/images/named_tuple.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55777 2024-04-30 15:29:56.000000 effidict-0.0.6/images/normal_dict.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-30 15:29:56.000000 effidict-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:30:06.269612 effidict-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:30:06.269612 effidict-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:29:56.000000 effidict-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-30 15:29:56.000000 effidict-0.0.6/tests/test_db_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-30 15:29:56.000000 effidict-0.0.6/tests/test_lru_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-30 15:29:56.000000 effidict-0.0.6/utils.py
```

### Comparing `effidict-0.0.5/.github/workflows/release.yaml` & `effidict-0.0.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/.github/workflows/test.yml` & `effidict-0.0.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/.readthedocs.yaml` & `effidict-0.0.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/LICENSE` & `effidict-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/PKG-INFO` & `effidict-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effidict
-Version: 0.0.5
+Version: 0.0.6
 Summary: Fast Python package providing enhanced dictionary-like data structures with advanced caching capabilities.
 Author-email: Isra Mekki <isra.mekki@helmholtz-munich.de>, Lisa Barros de Andrade e Sousa <lisa.barros.andrade.sousa@gmail.com>, Francesco Campi <francesco.campi@helmholtz-munich.de>
 Maintainer-email: Isra Mekki <isra.mekki@helmholtz-munich.de>
 Project-URL: documentation, https://oligo-designer-toolsuite.readthedocs.io/
 Project-URL: repository, https://github.com/HelmholtzAI-Consultants-Munich/oligo-designer-toolsuite
 Keywords: data structures,efficient dictionary
 Classifier: Programming Language :: Python :: 3
```

### Comparing `effidict-0.0.5/Readme.md` & `effidict-0.0.6/Readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,25 +17,31 @@
 You can install EffiDict via pip:
 
 ```
 pip install effidict
 ```
 
 ## Usage
+Importing the package
 ```
 from effidict import LRUDBDict, LRUDict, DBDict
+```
 
-# Using LRUDict
+Using `LRUDict` for persistent storage on `pickle` files
+```
 cache_dict = LRUDict(max_in_memory=100, storage_path="cache")
 cache_dict['key'] = 'value'
+```
 
-# Using LRUDBDict for persistent storage
+Using `LRUDBDict` for persistent storage on `sqlite`
+```
 db_cache_dict = LRUDBDict(max_in_memory=100, storage_path="cache.db")
 db_cache_dict['key'] = 'value'
-
-# Standard DBDict
+```
+Standard `DBDict` (`sqlite` only)
+```
 db_dict = DBDict(storage_path="cache.db")
 db_dict['key'] = 'value'
 ```
 
 ## License
 Licensed under the MIT License.
```

### Comparing `effidict-0.0.5/comparative_notebook.ipynb` & `effidict-0.0.6/comparative_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/docs/Makefile` & `effidict-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/docs/source/_static/logo_effidict.png` & `effidict-0.0.6/docs/source/_static/logo_effidict.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/docs/source/conf.py` & `effidict-0.0.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/docs/source/index.rst` & `effidict-0.0.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/effidict/_base.py` & `effidict-0.0.6/effidict/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -108,14 +108,30 @@
         """
         Remove all items from the cache.
         """
         self.memory.clear()
         for key in self.keys():
             self.__delitem__(key)
 
+    def __del__(self):
+        self.destroy()
+
+    def __eq__(self, other):
+        if not isinstance(other, EffiDictBase):
+            return False
+
+        if len(self) != len(other):
+            return False
+
+        for key, value in self.items():
+            if key not in other or other[key] != value:
+                return False
+
+        return True
+
     @abstractmethod
     def keys(self):
         pass
 
     @abstractmethod
     def __getitem__(self, key):
         pass
@@ -139,29 +155,7 @@
     @abstractmethod
     def load_from_dict(self, dictionary):
         pass
 
     @abstractmethod
     def destroy(self):
         pass
-
-    def __del__(self):
-        self.destroy()
-
-    def pop(self, key, default=None):
-        """
-        Remove an item from the cache and return its value.
-
-        This method attempts to use the __getitem__ and __delitem__ methods to
-        access and remove the item, respectively. If the key is not found, it
-        returns a default value if provided, or raises a KeyError.
-
-        :param key: The key of the item to remove.
-        :param default: The default value to return if the key is not found.
-        :return: The value of the removed item if the key is found or the default value if not.
-        """
-        try:
-            value = self[key]
-            del self[key]
-            return value
-        except KeyError:
-            return default
```

### Comparing `effidict-0.0.5/effidict/db_dict.py` & `effidict-0.0.6/effidict/db_dict.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/effidict/lru_dict.py` & `effidict-0.0.6/effidict/lru_dict.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/effidict.egg-info/PKG-INFO` & `effidict-0.0.6/effidict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effidict
-Version: 0.0.5
+Version: 0.0.6
 Summary: Fast Python package providing enhanced dictionary-like data structures with advanced caching capabilities.
 Author-email: Isra Mekki <isra.mekki@helmholtz-munich.de>, Lisa Barros de Andrade e Sousa <lisa.barros.andrade.sousa@gmail.com>, Francesco Campi <francesco.campi@helmholtz-munich.de>
 Maintainer-email: Isra Mekki <isra.mekki@helmholtz-munich.de>
 Project-URL: documentation, https://oligo-designer-toolsuite.readthedocs.io/
 Project-URL: repository, https://github.com/HelmholtzAI-Consultants-Munich/oligo-designer-toolsuite
 Keywords: data structures,efficient dictionary
 Classifier: Programming Language :: Python :: 3
```

### Comparing `effidict-0.0.5/effidict.egg-info/SOURCES.txt` & `effidict-0.0.6/effidict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/images/comparative.png` & `effidict-0.0.6/images/comparative.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/images/custom_100.png` & `effidict-0.0.6/images/custom_100.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/images/custom_1000.png` & `effidict-0.0.6/images/custom_1000.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/images/custom_1000_db.png` & `effidict-0.0.6/images/custom_1000_db.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/images/custom_1000_db_10.png` & `effidict-0.0.6/images/custom_1000_db_10.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/images/logo_effidict.png` & `effidict-0.0.6/images/logo_effidict.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/images/logo_effidict_no_bg.png` & `effidict-0.0.6/images/logo_effidict_no_bg.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/images/named_tuple.png` & `effidict-0.0.6/images/named_tuple.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/images/normal_dict.png` & `effidict-0.0.6/images/normal_dict.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/pyproject.toml` & `effidict-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/tests/test_db_dict.py` & `effidict-0.0.6/tests/test_db_dict.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/tests/test_lru_dict.py` & `effidict-0.0.6/tests/test_lru_dict.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.5/utils.py` & `effidict-0.0.6/utils.py`

 * *Files identical despite different names*

