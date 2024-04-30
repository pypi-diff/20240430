# Comparing `tmp/dknovautils-0.2.8.tar.gz` & `tmp/dknovautils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dknovautils-0.2.8.tar", last modified: Mon Apr 29 12:34:18 2024, max compression
+gzip compressed data, was "dknovautils-0.2.9.tar", last modified: Mon Apr 29 14:12:00 2024, max compression
```

## Comparing `dknovautils-0.2.8.tar` & `dknovautils-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 12:34:18.831507 dknovautils-0.2.8/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1091 2023-05-19 02:33:35.000000 dknovautils-0.2.8/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      914 2024-04-29 12:34:18.829337 dknovautils-0.2.8/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      169 2024-02-02 04:40:13.000000 dknovautils-0.2.8/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2398 2024-04-29 12:34:04.000000 dknovautils-0.2.8/pyproject.toml
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2024-04-29 12:34:18.831507 dknovautils-0.2.8/setup.cfg
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 12:34:18.785828 dknovautils-0.2.8/src/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 12:34:18.813326 dknovautils-0.2.8/src/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      326 2024-01-25 15:30:10.000000 dknovautils-0.2.8/src/dknovautils/__init__.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      134 2024-01-25 15:30:06.000000 dknovautils-0.2.8/src/dknovautils/__main__.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2907 2024-02-01 04:42:06.000000 dknovautils-0.2.8/src/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1229 2024-04-29 12:34:04.000000 dknovautils-0.2.8/src/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     6828 2024-01-25 19:13:32.000000 dknovautils-0.2.8/src/dknovautils/dk_lang_etc_util.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)    17331 2024-04-29 12:34:04.000000 dknovautils-0.2.8/src/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     4856 2024-04-29 12:30:42.000000 dknovautils-0.2.8/src/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1447 2024-04-19 11:27:14.000000 dknovautils-0.2.8/src/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     4035 2024-04-29 03:22:31.000000 dknovautils-0.2.8/src/dknovautils/dkprocess.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      618 2024-01-25 09:56:51.000000 dknovautils-0.2.8/src/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      282 2024-01-25 09:56:22.000000 dknovautils-0.2.8/src/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      314 2024-01-25 15:05:17.000000 dknovautils-0.2.8/src/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-01-25 17:59:24.000000 dknovautils-0.2.8/src/dknovautils/py.typed
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 12:34:18.828326 dknovautils-0.2.8/src/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      914 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      677 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       43 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/entry_points.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       14 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/top_level.txt
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 12:34:18.827325 dknovautils-0.2.8/tests/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      172 2024-01-26 10:01:40.000000 dknovautils-0.2.8/tests/test_b.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      220 2024-01-26 10:01:52.000000 dknovautils-0.2.8/tests/test_c.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     3700 2024-04-29 03:16:44.000000 dknovautils-0.2.8/tests/test_d.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 14:12:00.970541 dknovautils-0.2.9/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1091 2023-05-19 02:33:35.000000 dknovautils-0.2.9/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      914 2024-04-29 14:12:00.969544 dknovautils-0.2.9/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      169 2024-02-02 04:40:13.000000 dknovautils-0.2.9/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2398 2024-04-29 14:11:50.000000 dknovautils-0.2.9/pyproject.toml
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2024-04-29 14:12:00.970541 dknovautils-0.2.9/setup.cfg
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 14:12:00.929027 dknovautils-0.2.9/src/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 14:12:00.953025 dknovautils-0.2.9/src/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      326 2024-01-25 15:30:10.000000 dknovautils-0.2.9/src/dknovautils/__init__.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      134 2024-01-25 15:30:06.000000 dknovautils-0.2.9/src/dknovautils/__main__.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2907 2024-02-01 04:42:06.000000 dknovautils-0.2.9/src/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1229 2024-04-29 14:11:50.000000 dknovautils-0.2.9/src/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     6828 2024-01-25 19:13:32.000000 dknovautils-0.2.9/src/dknovautils/dk_lang_etc_util.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)    17331 2024-04-29 14:11:50.000000 dknovautils-0.2.9/src/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     5589 2024-04-29 14:09:47.000000 dknovautils-0.2.9/src/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1447 2024-04-19 11:27:14.000000 dknovautils-0.2.9/src/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      571 2024-04-29 12:59:03.000000 dknovautils-0.2.9/src/dknovautils/dknetwork.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     4035 2024-04-29 03:22:31.000000 dknovautils-0.2.9/src/dknovautils/dkprocess.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      618 2024-01-25 09:56:51.000000 dknovautils-0.2.9/src/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      282 2024-01-25 09:56:22.000000 dknovautils-0.2.9/src/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      314 2024-01-25 15:05:17.000000 dknovautils-0.2.9/src/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-01-25 17:59:24.000000 dknovautils-0.2.9/src/dknovautils/py.typed
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 14:12:00.968540 dknovautils-0.2.9/src/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      914 2024-04-29 14:12:00.000000 dknovautils-0.2.9/src/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      706 2024-04-29 14:12:00.000000 dknovautils-0.2.9/src/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2024-04-29 14:12:00.000000 dknovautils-0.2.9/src/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       43 2024-04-29 14:12:00.000000 dknovautils-0.2.9/src/dknovautils.egg-info/entry_points.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       14 2024-04-29 14:12:00.000000 dknovautils-0.2.9/src/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2024-04-29 14:12:00.000000 dknovautils-0.2.9/src/dknovautils.egg-info/top_level.txt
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 14:12:00.966540 dknovautils-0.2.9/tests/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      172 2024-01-26 10:01:40.000000 dknovautils-0.2.9/tests/test_b.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      220 2024-01-26 10:01:52.000000 dknovautils-0.2.9/tests/test_c.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     3700 2024-04-29 03:16:44.000000 dknovautils-0.2.9/tests/test_d.py
```

### Comparing `dknovautils-0.2.8/LICENSE` & `dknovautils-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.8/PKG-INFO` & `dknovautils-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.2.8
+Version: 0.2.9
 Summary: A small example package
 Author-email: dknova <dikisite@outlook.com>, dknova2 <dikisite2@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://example.com/xxx
 Project-URL: Documentation, https://readthedocs.org/xxx
 Project-URL: Repository, https://github.com/me/xxx.git
 Project-URL: Issues, https://github.com/me/xxx/issues
```

### Comparing `dknovautils-0.2.8/pyproject.toml` & `dknovautils-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 之所以改成setuptools build 是因为要配置 py.typed参数 而如果用hatch工具不知道如何配置
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dknovautils"
-version = '0.2.8'
+version = '0.2.9'
 dependencies = [
     "numpy",
     "ipython"
 ]
 authors = [
   { name="dknova", email="dikisite@outlook.com" },
   { name="dknova2", email="dikisite2@outlook.com" },
```

### Comparing `dknovautils-0.2.8/src/dknovautils/commons.py` & `dknovautils-0.2.9/src/dknovautils/commons.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.8/src/dknovautils/dk_imports.py` & `dknovautils-0.2.9/src/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.8/src/dknovautils/dk_lang_etc_util.py` & `dknovautils-0.2.9/src/dknovautils/dk_lang_etc_util.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.8/src/dknovautils/dkat.py` & `dknovautils-0.2.9/src/dknovautils/dkat.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import dknovautils
 
 # from dknovautils.dk_imports import *
 from dknovautils.commons import *
 
 
-DkAppVer = '0.2.8'
+DkAppVer = '0.2.9'
 
 _unknown_err = "_unknown_err4035"
 
 T = TypeVar("T")
 
 
 class staticproperty(property):
```

### Comparing `dknovautils-0.2.8/src/dknovautils/dkfiles.py` & `dknovautils-0.2.9/src/dknovautils/dkfiles.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,51 +121,77 @@
 
     @staticmethod
     def fill_disk_simple(
         dir: str = ".",
         *,
         size: int = 1024 * 1024 * 100,
         pre: str = "tmp",
-        verbose: bool = True,
+        verbose: bool = False,
     ) -> None:
         import numpy as np
 
         """
-        在目录下创建文件. 文件大小约为10M. 创建之后马上读出检查内容是否正确.
+        在目录下创建文件. 文件大小约为10M. 创建之后马上读出检查内容是否正确. 用来对硬盘进行简单的检查.
         直到写满磁盘为止, [Errno 28] No space left on device 最后退出.
+        
+        mkdir tmp
+        python3.10 -c "from dknovautils import *; DkFile.fill_disk_simple(dir='./tmp')"
 
         """
-        assert size >= 1024 * 1024 * 10
-        fid = 1
+        if isinstance(size, int):
+            assert size >= 1024 * 1024 * 10
+            N = size // len(bs)
+        else:
+            raise Exception("unimplemented")
+
         pre = "tmp"
         bse = b"a"
         bs = np.frombuffer(bse * (1024 * 1024), dtype=np.uint8)
-        N = size // len(bs)
+
+        def fpath(fid: int) -> Path:
+            return Path(f"{dir}/{pre}{fid:08d}")
+
+        print("begin write file")
+        fid = 1
         while True:
-            file = Path(f"{dir}/{pre}{fid:08d}")
+            file = fpath(fid)
             if verbose:
                 print(f"write file {file}")
             try:
                 with file.open(mode="wb") as f:
                     for i in range(N):
                         f.write(bs)
                     f.flush()
-                time.sleep(0.2)
+                fid += 1
+            except Exception as e:
+                print(e)
+                break
+
+        print("begin verify")
+        fid, maxfid = 1, fid
+        while True:
+            if fid >= maxfid:
+                break
+            file = fpath(fid)
+            if verbose:
+                print(f"verify file {file}")
+            try:
                 with file.open(mode="rb") as f:
                     r = f.read(len(bs))
                     bs2 = np.frombuffer(r, dtype=np.uint8)
                     if len(bs2) == len(bs):
-                        assert np.all(bs == bs2), "err56373 verify error"
+                        assert np.all(bs2 == bs), "err56373 verify error"
                     else:
                         condition = bs2 == bs[0]
                         assert np.all(condition), "err56374 verify error"
                 fid += 1
             except Exception as e:
                 print(e)
                 break
+        print("all end")
 
 
 class DkPyFiles(object):
     pass
 
 
 if __name__ == "__main__":
```

### Comparing `dknovautils-0.2.8/src/dknovautils/dkipy.py` & `dknovautils-0.2.9/src/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.8/src/dknovautils/dkprocess.py` & `dknovautils-0.2.9/src/dknovautils/dkprocess.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.8/src/dknovautils/example.py` & `dknovautils-0.2.9/src/dknovautils/example.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.8/src/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.2.9/src/dknovautils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.2.8
+Version: 0.2.9
 Summary: A small example package
 Author-email: dknova <dikisite@outlook.com>, dknova2 <dikisite2@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://example.com/xxx
 Project-URL: Documentation, https://readthedocs.org/xxx
 Project-URL: Repository, https://github.com/me/xxx.git
 Project-URL: Issues, https://github.com/me/xxx/issues
```

### Comparing `dknovautils-0.2.8/src/dknovautils.egg-info/SOURCES.txt` & `dknovautils-0.2.9/src/dknovautils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/dknovautils/__main__.py
 src/dknovautils/commons.py
 src/dknovautils/dk_imports.py
 src/dknovautils/dk_lang_etc_util.py
 src/dknovautils/dkat.py
 src/dknovautils/dkfiles.py
 src/dknovautils/dkipy.py
+src/dknovautils/dknetwork.py
 src/dknovautils/dkprocess.py
 src/dknovautils/example.py
 src/dknovautils/myadd.py
 src/dknovautils/mysubtract.py
 src/dknovautils/py.typed
 src/dknovautils.egg-info/PKG-INFO
 src/dknovautils.egg-info/SOURCES.txt
```

### Comparing `dknovautils-0.2.8/tests/test_d.py` & `dknovautils-0.2.9/tests/test_d.py`

 * *Files identical despite different names*

