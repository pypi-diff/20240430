# Comparing `tmp/excel2db-0.0.2.tar.gz` & `tmp/excel2db-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\excel2db-0.0.2.tar", last modified: Tue Apr 30 02:23:11 2024, max compression
+gzip compressed data, was "dist\excel2db-0.0.3.tar", last modified: Tue Apr 30 03:32:56 2024, max compression
```

## Comparing `excel2db-0.0.2.tar` & `excel2db-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/
--rw-rw-rw-   0        0        0      171 2024-04-30 02:23:11.000000 excel2db-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/
--rw-rw-rw-   0        0        0        0 2024-04-24 13:59:30.000000 excel2db-0.0.2/excel2db/__init__.py
--rw-rw-rw-   0        0        0    19636 2024-04-25 02:26:33.000000 excel2db-0.0.2/excel2db/cheakConf.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/com/
--rw-rw-rw-   0        0        0        0 2024-04-25 02:12:38.000000 excel2db-0.0.2/excel2db/com/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/com/util/
--rw-rw-rw-   0        0        0        0 2024-04-25 02:12:38.000000 excel2db-0.0.2/excel2db/com/util/__init__.py
--rw-rw-rw-   0        0        0     8036 2023-06-28 01:48:10.000000 excel2db-0.0.2/excel2db/com/util/coordinate.py
--rw-rw-rw-   0        0        0     1637 2024-04-25 02:08:40.000000 excel2db-0.0.2/excel2db/com/util/dbconnect.py
--rw-rw-rw-   0        0        0     6194 2023-10-17 13:38:33.000000 excel2db-0.0.2/excel2db/com/util/fileTool.py
--rw-rw-rw-   0        0        0     8842 2024-04-25 02:39:56.000000 excel2db-0.0.2/excel2db/com/util/timeTool.py
--rw-rw-rw-   0        0        0     5072 2024-04-29 09:11:27.000000 excel2db-0.0.2/excel2db/defaultConf.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/demo/
--rw-rw-rw-   0        0        0        0 2024-04-25 03:02:41.000000 excel2db-0.0.2/excel2db/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/demo/demo1/
--rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo1/__init__.py
--rw-rw-rw-   0        0        0      173 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo1/demo1.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/demo/demo2/
--rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo2/__init__.py
--rw-rw-rw-   0        0        0      190 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo2/demo2.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/demo/demo3/
--rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo3/__init__.py
--rw-rw-rw-   0        0        0      190 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo3/demo3.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db/demo/demo4/
--rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.2/excel2db/demo/demo4/__init__.py
--rw-rw-rw-   0        0        0      175 2024-04-30 02:21:22.000000 excel2db-0.0.2/excel2db/demo/demo4/demo4.py
--rw-rw-rw-   0        0        0     3807 2024-04-30 02:21:22.000000 excel2db-0.0.2/excel2db/demo/generalDemoFile.py
--rw-rw-rw-   0        0        0     2629 2024-04-25 02:28:07.000000 excel2db-0.0.2/excel2db/detailData.py
--rw-rw-rw-   0        0        0     2636 2024-04-25 02:28:07.000000 excel2db-0.0.2/excel2db/detailTitle.py
--rw-rw-rw-   0        0        0     2534 2024-04-25 02:37:46.000000 excel2db-0.0.2/excel2db/excel.py
--rw-rw-rw-   0        0        0      719 2024-04-25 02:26:33.000000 excel2db-0.0.2/excel2db/excel2db.py
--rw-rw-rw-   0        0        0     2058 2024-04-25 02:37:46.000000 excel2db-0.0.2/excel2db/extraFuction.py
--rw-rw-rw-   0        0        0     5897 2024-04-30 02:03:04.000000 excel2db-0.0.2/excel2db/insert2sqlite.py
--rw-rw-rw-   0        0        0     3063 2024-04-25 02:42:06.000000 excel2db-0.0.2/excel2db/mainData.py
--rw-rw-rw-   0        0        0     3411 2024-04-25 02:42:06.000000 excel2db-0.0.2/excel2db/mainTitle.py
--rw-rw-rw-   0        0        0     6949 2024-04-25 02:42:06.000000 excel2db-0.0.2/excel2db/scale.py
--rw-rw-rw-   0        0        0     5200 2024-04-25 02:42:06.000000 excel2db-0.0.2/excel2db/sheet.py
--rw-rw-rw-   0        0        0     9711 2024-04-25 02:39:56.000000 excel2db-0.0.2/excel2db/value.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db.egg-info/
--rw-rw-rw-   0        0        0      171 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 02:23:11.000000 excel2db-0.0.2/excel2db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 02:23:11.000000 excel2db-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-04-30 02:23:10.000000 excel2db-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:56.000000 excel2db-0.0.3/
+-rw-rw-rw-   0        0        0      171 2024-04-30 03:32:56.000000 excel2db-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db/
+-rw-rw-rw-   0        0        0        0 2024-04-24 13:59:30.000000 excel2db-0.0.3/excel2db/__init__.py
+-rw-rw-rw-   0        0        0    19621 2024-04-30 03:24:30.000000 excel2db-0.0.3/excel2db/cheakConf.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db/com/
+-rw-rw-rw-   0        0        0        0 2024-04-25 02:12:38.000000 excel2db-0.0.3/excel2db/com/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db/com/util/
+-rw-rw-rw-   0        0        0        0 2024-04-25 02:12:38.000000 excel2db-0.0.3/excel2db/com/util/__init__.py
+-rw-rw-rw-   0        0        0     8036 2023-06-28 01:48:10.000000 excel2db-0.0.3/excel2db/com/util/coordinate.py
+-rw-rw-rw-   0        0        0     1633 2024-04-30 03:24:30.000000 excel2db-0.0.3/excel2db/com/util/dbconnect.py
+-rw-rw-rw-   0        0        0     6194 2023-10-17 13:38:33.000000 excel2db-0.0.3/excel2db/com/util/fileTool.py
+-rw-rw-rw-   0        0        0     8838 2024-04-30 03:24:30.000000 excel2db-0.0.3/excel2db/com/util/timeTool.py
+-rw-rw-rw-   0        0        0     5072 2024-04-29 09:11:27.000000 excel2db-0.0.3/excel2db/defaultConf.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db/demo/
+-rw-rw-rw-   0        0        0        0 2024-04-25 03:02:41.000000 excel2db-0.0.3/excel2db/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db/demo/demo1/
+-rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.3/excel2db/demo/demo1/__init__.py
+-rw-rw-rw-   0        0        0      173 2024-04-30 02:19:13.000000 excel2db-0.0.3/excel2db/demo/demo1/demo1.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db/demo/demo2/
+-rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.3/excel2db/demo/demo2/__init__.py
+-rw-rw-rw-   0        0        0      190 2024-04-30 02:19:13.000000 excel2db-0.0.3/excel2db/demo/demo2/demo2.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db/demo/demo3/
+-rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.3/excel2db/demo/demo3/__init__.py
+-rw-rw-rw-   0        0        0      190 2024-04-30 02:19:13.000000 excel2db-0.0.3/excel2db/demo/demo3/demo3.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db/demo/demo4/
+-rw-rw-rw-   0        0        0        0 2024-04-30 02:19:13.000000 excel2db-0.0.3/excel2db/demo/demo4/__init__.py
+-rw-rw-rw-   0        0        0      175 2024-04-30 02:21:22.000000 excel2db-0.0.3/excel2db/demo/demo4/demo4.py
+-rw-rw-rw-   0        0        0     3807 2024-04-30 02:21:22.000000 excel2db-0.0.3/excel2db/demo/generalDemoFile.py
+-rw-rw-rw-   0        0        0     2614 2024-04-30 03:24:30.000000 excel2db-0.0.3/excel2db/detailData.py
+-rw-rw-rw-   0        0        0     2621 2024-04-30 03:24:30.000000 excel2db-0.0.3/excel2db/detailTitle.py
+-rw-rw-rw-   0        0        0     2527 2024-04-30 03:24:30.000000 excel2db-0.0.3/excel2db/excel.py
+-rw-rw-rw-   0        0        0      712 2024-04-30 03:24:30.000000 excel2db-0.0.3/excel2db/excel2db.py
+-rw-rw-rw-   0        0        0     2050 2024-04-30 03:24:30.000000 excel2db-0.0.3/excel2db/extraFuction.py
+-rw-rw-rw-   0        0        0     5891 2024-04-30 03:27:24.000000 excel2db-0.0.3/excel2db/insert2sqlite.py
+-rw-rw-rw-   0        0        0     3057 2024-04-30 03:27:24.000000 excel2db-0.0.3/excel2db/mainData.py
+-rw-rw-rw-   0        0        0     3405 2024-04-30 03:27:24.000000 excel2db-0.0.3/excel2db/mainTitle.py
+-rw-rw-rw-   0        0        0     6943 2024-04-30 03:27:24.000000 excel2db-0.0.3/excel2db/scale.py
+-rw-rw-rw-   0        0        0     5193 2024-04-30 03:27:24.000000 excel2db-0.0.3/excel2db/sheet.py
+-rw-rw-rw-   0        0        0     9704 2024-04-30 03:27:24.000000 excel2db-0.0.3/excel2db/value.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db.egg-info/
+-rw-rw-rw-   0        0        0      171 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      949 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 03:32:56.000000 excel2db-0.0.3/excel2db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 03:32:56.000000 excel2db-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      514 2024-04-30 03:32:52.000000 excel2db-0.0.3/setup.py
```

### Comparing `excel2db-0.0.2/excel2db/cheakConf.py` & `excel2db-0.0.3/excel2db/cheakConf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf8 -*-
 """
 生成对应级别配置文件
 """
 from json import loads
-from excel2db.com.util import fileTool, coordinate
-from excel2db import defaultConf
+from .com.util import fileTool, coordinate
+from . import defaultConf
 
 def combinExcelConf(*configFileUrl):
     """
     校验配置文件，并合并excel级别配置文件，后面的配置文件覆盖前面的
     :param conf: 配置文件元组
     """
     filetool = fileTool.fileTool()
```

### Comparing `excel2db-0.0.2/excel2db/com/util/coordinate.py` & `excel2db-0.0.3/excel2db/com/util/coordinate.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.2/excel2db/com/util/dbconnect.py` & `excel2db-0.0.3/excel2db/com/util/dbconnect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 数据库连接
 在实例化类后，使用时应判断STATUS参数，若参数为0表示连接成功，可以调用
 可以使用close方法关闭，也可以等待程序结束后自动关闭
 """
-import threading, re
+import threading
 
 ###sqlite
 class sqliteCon:
     def __init__(self, dbname):
         """
         :param dbname: 数据库文件路径
         """
```

### Comparing `excel2db-0.0.2/excel2db/com/util/fileTool.py` & `excel2db-0.0.3/excel2db/com/util/fileTool.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.2/excel2db/com/util/timeTool.py` & `excel2db-0.0.3/excel2db/com/util/timeTool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 """时间工具
 Author: endlessdesert
 """
-import datetime, time, os
+import datetime, time
 
 def verityFormat(date, format='%Y-%m-%d %H:%M:%S'):
     """
     校验字符串日期格式
     :param date:
     :param format:
     :return:
```

### Comparing `excel2db-0.0.2/excel2db/defaultConf.py` & `excel2db-0.0.3/excel2db/defaultConf.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.2/excel2db/demo/generalDemoFile.py` & `excel2db-0.0.3/excel2db/demo/generalDemoFile.py`

 * *Files identical despite different names*

### Comparing `excel2db-0.0.2/excel2db/detailData.py` & `excel2db-0.0.3/excel2db/detailData.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf8 -*-
 """
 ##执行detailData级别转换
 """
-from excel2db import cheakConf, scale
-from excel2db.com.util.coordinate import coordinate
+from . import cheakConf, scale
+from .com.util.coordinate import coordinate
 
 class detailData:
     def __init__(self, value, conf):
 
         """
         detailData级别操作
         :param value: 变量文件
```

### Comparing `excel2db-0.0.2/excel2db/detailTitle.py` & `excel2db-0.0.3/excel2db/detailTitle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf8 -*-
 """
 ##执行detailTitle级别转换
 """
-from excel2db import cheakConf, scale
-from excel2db.com.util.coordinate import coordinate
+from . import cheakConf, scale
+from .com.util.coordinate import coordinate
 
 class detailTitle:
     def __init__(self, value, conf):
 
         """
         detailTitle级别操作
         :param value: 变量文件
```

### Comparing `excel2db-0.0.2/excel2db/excel.py` & `excel2db-0.0.3/excel2db/excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf8 -*-
 """
 ##执行excel级别转换
 """
 import os, xlrd
 from pandas import read_excel
 from openpyxl import load_workbook
-from excel2db import cheakConf, sheet, insert2sqlite
+from . import cheakConf, sheet, insert2sqlite
 
 class excel:
     def __init__(self, value, conf):
 
         """
         excel级别操作
         :param value: 变量文件
```

### Comparing `excel2db-0.0.2/excel2db/excel2db.py` & `excel2db-0.0.3/excel2db/excel2db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf8 -*-
 """
 用于excel转sqlite数据库
 注意：
 依据变量修改配置文件，应在cheakConf中进行
 依据配置文件修改变量，应在配置文件完全生成后进行
 """
-from excel2db import value, cheakConf, excel
+from . import value, cheakConf, excel
 
 class excel2db:
 
     def __init__(self, *configFileUrl):
         """
         :param *configFileUrl: 配置文件路径
         """
```

### Comparing `excel2db-0.0.2/excel2db/extraFuction.py` & `excel2db-0.0.3/excel2db/extraFuction.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 
 """
 日期格式编辑器
 定义方法，需设置两个参数：date(传入数据),targetFormat(目标格式), 并且返回处理后的数据
 """
-from excel2db.com.util import timeTool
+from .com.util import timeTool
 
 def dateFormat_1(date, targetFormat):
     print(date)
     baseDate = "2023-08-01"  ##基准日期
     baseNum = 45139  ##基准数字
     number = int(float(date))
     date = timeTool.changeTime(baseDate, "days", number - baseNum, targetFormat)
```

### Comparing `excel2db-0.0.2/excel2db/insert2sqlite.py` & `excel2db-0.0.3/excel2db/insert2sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 
 import sys, numpy
-from com.util import dbconnect, fileTool
-from excel2db import defaultConf
+from .com.util import dbconnect, fileTool
+from . import defaultConf
 
 class insert2sqlite:
     def __init__(self, value):
         """
         插入数据库操作
         :param value: 变量文件
         """
```

### Comparing `excel2db-0.0.2/excel2db/mainData.py` & `excel2db-0.0.3/excel2db/mainData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf8 -*-
 """
 ##执行mainData级别转换
 """
-from excel2db import cheakConf, scale
-from com.util.coordinate import coordinate
+from . import cheakConf, scale
+from .com.util.coordinate import coordinate
 
 class mainData:
     def __init__(self, value, conf):
 
         """
         mainData级别操作
         :param value: 变量文件
```

### Comparing `excel2db-0.0.2/excel2db/mainTitle.py` & `excel2db-0.0.3/excel2db/mainTitle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf8 -*-
 """
 ##执行mainTitle级别转换
 """
-from excel2db import cheakConf, scale
-from com.util.coordinate import coordinate
+from . import cheakConf, scale
+from .com.util.coordinate import coordinate
 
 class mainTitle:
     def __init__(self, value, conf):
 
         """
         mainTitle级别操作
         :param value: 变量文件
```

### Comparing `excel2db-0.0.2/excel2db/scale.py` & `excel2db-0.0.3/excel2db/scale.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf8 -*-
 """
 ##执行scale级别转换
 """
-from excel2db import cheakConf
-from com.util import timeTool
+from . import cheakConf
+from .com.util import timeTool
 import numpy as np
 
 class scale:
     def __init__(self, value, conf):
 
         """
         scale级别操作
```

### Comparing `excel2db-0.0.2/excel2db/sheet.py` & `excel2db-0.0.3/excel2db/sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding:utf8 -*-
 """
 ##执行sheet级别转换
 """
-from excel2db import cheakConf, mainTitle, mainData, detailTitle, detailData
+from . import cheakConf, mainTitle, mainData, detailTitle, detailData
 
 class sheet:
     def __init__(self, value, conf):
 
         """
         sheet级别操作
         :param value: 变量文件
```

### Comparing `excel2db-0.0.2/excel2db/value.py` & `excel2db-0.0.3/excel2db/value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf8 -*-
 """
 变量存放
 """
 import string, xmltodict, zipfile, shutil, os, inspect
-from excel2db import extraFuction
+from . import extraFuction
 
 class value:
     def __init__(self):
         ##excel文件相关
         self.excelFileName = "" ##excel文件名
         self.sheetList = [] ##sheet工作表列表
```

### Comparing `excel2db-0.0.2/excel2db.egg-info/SOURCES.txt` & `excel2db-0.0.3/excel2db.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 excel2db/mainTitle.py
 excel2db/scale.py
 excel2db/sheet.py
 excel2db/value.py
 excel2db.egg-info/PKG-INFO
 excel2db.egg-info/SOURCES.txt
 excel2db.egg-info/dependency_links.txt
+excel2db.egg-info/requires.txt
 excel2db.egg-info/top_level.txt
 excel2db/com/__init__.py
 excel2db/com/util/__init__.py
 excel2db/com/util/coordinate.py
 excel2db/com/util/dbconnect.py
 excel2db/com/util/fileTool.py
 excel2db/com/util/timeTool.py
```

