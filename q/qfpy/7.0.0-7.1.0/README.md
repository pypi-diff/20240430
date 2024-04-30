# Comparing `tmp/qfpy-7.0.0.tar.gz` & `tmp/qfpy-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfpy-7.0.0.tar", last modified: Mon Apr 29 17:02:35 2024, max compression
+gzip compressed data, was "qfpy-7.1.0.tar", last modified: Tue Apr 30 16:32:30 2024, max compression
```

## Comparing `qfpy-7.0.0.tar` & `qfpy-7.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:02:35.722128 qfpy-7.0.0/
--rw-rw-rw-   0        0        0      159 2024-04-29 17:02:35.721150 qfpy-7.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-29 17:02:17.000000 qfpy-7.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 17:02:35.722128 qfpy-7.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 17:02:35.691856 qfpy-7.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 17:02:35.712364 qfpy-7.0.0/src/qfpy/
--rw-rw-rw-   0        0        0       80 2024-04-29 17:01:22.000000 qfpy-7.0.0/src/qfpy/__init__.py
--rw-rw-rw-   0        0        0      210 2024-04-29 16:48:36.000000 qfpy-7.0.0/src/qfpy/character.py
--rw-rw-rw-   0        0        0      131 2024-04-29 17:01:55.000000 qfpy-7.0.0/src/qfpy/crypto.py
--rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-7.0.0/src/qfpy/exif.py
--rw-rw-rw-   0        0        0     3067 2024-04-29 16:52:59.000000 qfpy-7.0.0/src/qfpy/ffmpeg.py
--rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-7.0.0/src/qfpy/folder.py
--rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-7.0.0/src/qfpy/function.py
--rw-rw-rw-   0        0        0      854 2024-04-29 16:55:44.000000 qfpy-7.0.0/src/qfpy/process.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:02:35.720174 qfpy-7.0.0/src/qfpy.egg-info/
--rw-rw-rw-   0        0        0      159 2024-04-29 17:02:35.000000 qfpy-7.0.0/src/qfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-04-29 17:02:35.000000 qfpy-7.0.0/src/qfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:02:35.000000 qfpy-7.0.0/src/qfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-29 17:02:35.000000 qfpy-7.0.0/src/qfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 16:32:30.353092 qfpy-7.1.0/
+-rw-rw-rw-   0        0        0      159 2024-04-30 16:32:30.352096 qfpy-7.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-30 16:32:15.000000 qfpy-7.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:32:30.353092 qfpy-7.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 16:32:30.329090 qfpy-7.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 16:32:30.346096 qfpy-7.1.0/src/qfpy/
+-rw-rw-rw-   0        0        0       80 2024-04-29 17:01:22.000000 qfpy-7.1.0/src/qfpy/__init__.py
+-rw-rw-rw-   0        0        0      210 2024-04-29 16:48:36.000000 qfpy-7.1.0/src/qfpy/character.py
+-rw-rw-rw-   0        0        0      131 2024-04-29 17:01:55.000000 qfpy-7.1.0/src/qfpy/crypto.py
+-rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-7.1.0/src/qfpy/exif.py
+-rw-rw-rw-   0        0        0     3067 2024-04-29 16:52:59.000000 qfpy-7.1.0/src/qfpy/ffmpeg.py
+-rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-7.1.0/src/qfpy/folder.py
+-rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-7.1.0/src/qfpy/function.py
+-rw-rw-rw-   0        0        0     1127 2024-04-30 16:31:47.000000 qfpy-7.1.0/src/qfpy/process.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:32:30.351095 qfpy-7.1.0/src/qfpy.egg-info/
+-rw-rw-rw-   0        0        0      159 2024-04-30 16:32:30.000000 qfpy-7.1.0/src/qfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-04-30 16:32:30.000000 qfpy-7.1.0/src/qfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:32:30.000000 qfpy-7.1.0/src/qfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-30 16:32:30.000000 qfpy-7.1.0/src/qfpy.egg-info/top_level.txt
```

### Comparing `qfpy-7.0.0/src/qfpy/exif.py` & `qfpy-7.1.0/src/qfpy/exif.py`

 * *Files identical despite different names*

### Comparing `qfpy-7.0.0/src/qfpy/ffmpeg.py` & `qfpy-7.1.0/src/qfpy/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `qfpy-7.0.0/src/qfpy/folder.py` & `qfpy-7.1.0/src/qfpy/folder.py`

 * *Files identical despite different names*

### Comparing `qfpy-7.0.0/src/qfpy/function.py` & `qfpy-7.1.0/src/qfpy/function.py`

 * *Files identical despite different names*

### Comparing `qfpy-7.0.0/src/qfpy/process.py` & `qfpy-7.1.0/src/qfpy/process.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import psutil
 
 
 def exist(process_name: str) -> bool:
     """
-    检查指定的进程是否在运行
+    检查指定的进程是否 存在
     
     参数:
     - process_name: str，要检查的进程名称（不包含扩展名）
     
     返回值:
     - bool，如果进程正在运行，则返回True；否则返回False
     """
@@ -22,10 +22,22 @@
     # 遍历所有运行的进程，忽略大小写比较进程名
     for p in psutil.process_iter():
         if process_name in p.name().lower():
             return True  # 找到匹配的进程，返回True
     
     return False  # 未找到匹配的进程，返回False
 
+def not_exit(process_name: str) -> bool:
+    """
+    描述：检查指定的进程是否 不存在
+    
+    参数
+    - process_name：str，要检查的进程名称（不包含扩展名）
+    
+    返回
+    - bool
+    """
+    return not exist(process_name)
+
 
 if __name__ == "__main__":
     print(exist("edge"))
```

