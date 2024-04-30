# Comparing `tmp/python_dupan-0.0.1.3.6.tar.gz` & `tmp/python_dupan-0.0.1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dupan-0.0.1.3.6.tar", max compression
+gzip compressed data, was "python_dupan-0.0.1.3.7.tar", max compression
```

## Comparing `python_dupan-0.0.1.3.6.tar` & `python_dupan-0.0.1.3.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1100 2023-12-31 13:16:43.902936 python_dupan-0.0.1.3.6/LICENSE
--rw-r--r--   0        0        0    96106 2024-04-20 12:24:08.768698 python_dupan-0.0.1.3.6/dupan/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_dupan-0.0.1.3.6/dupan/py.typed
--rw-r--r--   0        0        0       61 2024-01-01 10:28:23.372962 python_dupan-0.0.1.3.6/dupan/util/__init__.py
--rw-r--r--   0        0        0    13103 2024-01-19 04:25:53.949786 python_dupan-0.0.1.3.6/dupan/util/file.py
--rw-r--r--   0        0        0     1795 2023-12-14 11:01:07.350145 python_dupan-0.0.1.3.6/dupan/util/property.py
--rw-r--r--   0        0        0     2751 2023-12-29 05:26:01.836028 python_dupan-0.0.1.3.6/dupan/util/response.py
--rw-r--r--   0        0        0     6295 2024-01-16 04:33:26.963104 python_dupan-0.0.1.3.6/dupan/util/text.py
--rw-r--r--   0        0        0     2114 2023-12-10 10:45:36.285664 python_dupan-0.0.1.3.6/dupan/util/urlopen.py
--rw-r--r--   0        0        0     1249 2024-04-20 12:25:13.879064 python_dupan-0.0.1.3.6/pyproject.toml
--rw-r--r--   0        0        0    10836 2024-01-17 04:31:26.628554 python_dupan-0.0.1.3.6/readme.md
--rw-r--r--   0        0        0    12069 1970-01-01 00:00:00.000000 python_dupan-0.0.1.3.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-12-31 13:16:43.902936 python_dupan-0.0.1.3.7/LICENSE
+-rw-r--r--   0        0        0    97454 2024-04-30 15:58:43.872254 python_dupan-0.0.1.3.7/dupan/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_dupan-0.0.1.3.7/dupan/py.typed
+-rw-r--r--   0        0        0       61 2024-01-01 10:28:23.372962 python_dupan-0.0.1.3.7/dupan/util/__init__.py
+-rw-r--r--   0        0        0    13103 2024-01-19 04:25:53.949786 python_dupan-0.0.1.3.7/dupan/util/file.py
+-rw-r--r--   0        0        0     1795 2023-12-14 11:01:07.350145 python_dupan-0.0.1.3.7/dupan/util/property.py
+-rw-r--r--   0        0        0     2751 2023-12-29 05:26:01.836028 python_dupan-0.0.1.3.7/dupan/util/response.py
+-rw-r--r--   0        0        0     6295 2024-01-16 04:33:26.963104 python_dupan-0.0.1.3.7/dupan/util/text.py
+-rw-r--r--   0        0        0     2114 2023-12-10 10:45:36.285664 python_dupan-0.0.1.3.7/dupan/util/urlopen.py
+-rw-r--r--   0        0        0     1249 2024-04-30 15:59:15.383122 python_dupan-0.0.1.3.7/pyproject.toml
+-rw-r--r--   0        0        0    10836 2024-01-17 04:31:26.628554 python_dupan-0.0.1.3.7/readme.md
+-rw-r--r--   0        0        0    12069 1970-01-01 00:00:00.000000 python_dupan-0.0.1.3.7/PKG-INFO
```

### Comparing `python_dupan-0.0.1.3.6/LICENSE` & `python_dupan-0.0.1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.6/dupan/__init__.py` & `python_dupan-0.0.1.3.7/dupan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2255,17 +2255,24 @@
         if isinstance(path, DuPanPath):
             path = path.path
         elif _check:
             path = self.abspath(path)
         path = cast(str, path)
         if path == "/":
             return "/"
-        if not exist_ok and self.exists(path, _check=False):
-            raise FileExistsError(errno.EEXIST, path)
-        Error.check(self.client.makedir(path))
+        try:
+            attr = self.attr(path, _check=False)
+        except FileNotFoundError:
+            if exist_ok:
+                if not attr["isdir"]:
+                    raise NotADirectoryError(errno.ENOTDIR, path)
+            else:
+                raise FileExistsError(errno.EEXIST, path)
+        else:
+            return Error.check(self.client.makedir(path))["path"]
         return path
 
     def mkdir(
         self, 
         /, 
         path: str | PathLike[str], 
         _check: bool = True, 
@@ -2639,14 +2646,46 @@
         if not self.exists(path, _check=False):
             dir_ = dirname(path)
             if not self.attr(dir_, _check=False)["isdir"]:
                 raise NotADirectoryError(errno.ENOTDIR, f"parent path {dir_!r} is not a directory: {path!r}")
             return self.upload(BytesIO(), path, _check=False)
         return path
 
+    # TODO: 确保转存后也保持目录结构
+    def transfer(
+        self, 
+        /, 
+        url: str, 
+        password: str = "", 
+        fsidlist: None | list[int] = None, 
+        save_dir: str = "/", 
+    ) -> dict:
+        """转存文件到百度网盘
+
+        :param url: 分享链接
+        :param password: 密码（如果链接中包含密码，可以不传）
+        :param fsidlist: 待转存的文件 id 列表
+        :param save_dir: 存储到这个文件夹，默认是 /，也就是网盘根目录（请提前建立这个文件夹）
+
+        :return: 转存接口返回到 JSON 信息
+        """
+        share_list = DuPanShareList(url, password)
+        if not fsidlist:
+            fsidlist = [f["fs_id"] for f in share_list.list_index()]
+        return self.client.transfer(
+            share_list.url, 
+            params={
+                "shareid": share_list.share_id, 
+                "from": share_list.share_uk, 
+                "sekey": share_list.randsk, 
+                "ondup": "overwrite", 
+            }, 
+            data = {"fsidlist": fsidlist, "path": save_dir}, 
+        )
+
     def upload(
         self, 
         /, 
         local_path_or_file: str | PathLike | SupportsRead[bytes] | TextIOWrapper, 
         path: str | PathLike[str] = "", 
         overwrite_or_ignore: Optional[bool] = None, 
         _check: bool = True,
```

### Comparing `python_dupan-0.0.1.3.6/dupan/util/file.py` & `python_dupan-0.0.1.3.7/dupan/util/file.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.6/dupan/util/property.py` & `python_dupan-0.0.1.3.7/dupan/util/property.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.6/dupan/util/response.py` & `python_dupan-0.0.1.3.7/dupan/util/response.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.6/dupan/util/text.py` & `python_dupan-0.0.1.3.7/dupan/util/text.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.6/dupan/util/urlopen.py` & `python_dupan-0.0.1.3.7/dupan/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.6/pyproject.toml` & `python_dupan-0.0.1.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-dupan"
-version = "0.0.1.3.6"
+version = "0.0.1.3.7"
 description = "Python wrapper for `baidu webdisk <https://pan.baidu.com>`."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-dupan-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-dupan-client"
 keywords = ["nas", "dupan", "百度网盘"]
```

### Comparing `python_dupan-0.0.1.3.6/readme.md` & `python_dupan-0.0.1.3.7/readme.md`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.6/PKG-INFO` & `python_dupan-0.0.1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dupan
-Version: 0.0.1.3.6
+Version: 0.0.1.3.7
 Summary: Python wrapper for `baidu webdisk <https://pan.baidu.com>`.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-dupan-client
 License: MIT
 Keywords: nas,dupan,百度网盘
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

