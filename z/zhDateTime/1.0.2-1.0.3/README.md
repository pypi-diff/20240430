# Comparing `tmp/zhdatetime-1.0.2.tar.gz` & `tmp/zhdatetime-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhdatetime-1.0.2.tar", last modified: Sun Apr 21 15:51:05 2024, max compression
+gzip compressed data, was "zhdatetime-1.0.3.tar", last modified: Tue Apr 30 13:32:42 2024, max compression
```

## Comparing `zhdatetime-1.0.2.tar` & `zhdatetime-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 15:51:05.275787 zhdatetime-1.0.2/
--rw-rw-rw-   0        0        0    17098 2024-04-04 07:00:32.000000 zhdatetime-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       41 2023-11-18 16:11:48.000000 zhdatetime-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5773 2024-04-21 15:51:05.271783 zhdatetime-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5255 2024-04-21 07:38:14.000000 zhdatetime-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 15:51:05.275787 zhdatetime-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      764 2024-04-21 06:37:26.000000 zhdatetime-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:51:05.243849 zhdatetime-1.0.2/zhDateTime/
--rw-rw-rw-   0        0        0     1737 2024-04-21 15:49:10.000000 zhdatetime-1.0.2/zhDateTime/__init__.py
--rw-rw-rw-   0        0        0     4455 2024-04-21 05:23:15.000000 zhdatetime-1.0.2/zhDateTime/constants.py
--rw-rw-rw-   0        0        0    23682 2024-04-21 15:49:41.000000 zhdatetime-1.0.2/zhDateTime/main.py
--rw-rw-rw-   0        0        0     1664 2024-04-20 17:40:06.000000 zhdatetime-1.0.2/zhDateTime/types.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:51:05.267778 zhdatetime-1.0.2/zhDateTime.egg-info/
--rw-rw-rw-   0        0        0     5773 2024-04-21 15:51:04.000000 zhdatetime-1.0.2/zhDateTime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-04-21 15:51:05.000000 zhdatetime-1.0.2/zhDateTime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 15:51:04.000000 zhdatetime-1.0.2/zhDateTime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-21 15:51:04.000000 zhdatetime-1.0.2/zhDateTime.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 13:32:42.682824 zhdatetime-1.0.3/
+-rw-rw-rw-   0        0        0    17098 2024-04-04 07:00:32.000000 zhdatetime-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       60 2024-04-30 13:32:25.000000 zhdatetime-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5773 2024-04-30 13:32:42.679800 zhdatetime-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5255 2024-04-21 07:38:14.000000 zhdatetime-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 13:32:42.682824 zhdatetime-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      764 2024-04-21 06:37:26.000000 zhdatetime-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:32:42.659985 zhdatetime-1.0.3/zhDateTime/
+-rw-rw-rw-   0        0        0     1737 2024-04-30 13:28:56.000000 zhdatetime-1.0.3/zhDateTime/__init__.py
+-rw-rw-rw-   0        0        0     4455 2024-04-21 05:23:15.000000 zhdatetime-1.0.3/zhDateTime/constants.py
+-rw-rw-rw-   0        0        0    23692 2024-04-30 13:22:57.000000 zhdatetime-1.0.3/zhDateTime/main.py
+-rw-rw-rw-   0        0        0     1664 2024-04-20 17:40:06.000000 zhdatetime-1.0.3/zhDateTime/types.py
+drwxrwxrwx   0        0        0        0 2024-04-30 13:32:42.676822 zhdatetime-1.0.3/zhDateTime.egg-info/
+-rw-rw-rw-   0        0        0     5773 2024-04-30 13:32:42.000000 zhdatetime-1.0.3/zhDateTime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-30 13:32:42.000000 zhdatetime-1.0.3/zhDateTime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 13:32:42.000000 zhdatetime-1.0.3/zhDateTime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-30 13:32:42.000000 zhdatetime-1.0.3/zhDateTime.egg-info/top_level.txt
```

### Comparing `zhdatetime-1.0.2/LICENSE` & `zhdatetime-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zhdatetime-1.0.2/PKG-INFO` & `zhdatetime-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhDateTime
-Version: 1.0.2
+Version: 1.0.3
 Summary: 一个简单的小巧的中式日期时间库，附带数字汉字化操作。
 Home-page: https://gitee.com/EillesWan/zhDateTime
 Author: Eilles Wan
 Author-email: EillesWan@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `zhdatetime-1.0.2/README.md` & `zhdatetime-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zhdatetime-1.0.2/setup.py` & `zhdatetime-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `zhdatetime-1.0.2/zhDateTime/__init__.py` & `zhdatetime-1.0.3/zhDateTime/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Copyright (R) 2024 Eilles Wan
 
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at http://mozilla.org/MPL/2.0/.
 """
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __all__ = [
     # 所用之函数
     "shichen_ke_2_hour_minute",
     "hour_minute_2_shichen_ke",
     "get_lunar_month_list",
     "get_lunar_new_year",
     "verify_lunar_date",
```

### Comparing `zhdatetime-1.0.2/zhDateTime/constants.py` & `zhdatetime-1.0.3/zhDateTime/constants.py`

 * *Files identical despite different names*

### Comparing `zhdatetime-1.0.2/zhDateTime/main.py` & `zhdatetime-1.0.3/zhDateTime/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,19 +113,19 @@
 
     返回值
     ------
         Tuple(List[int当月天数, ]当年每月天数, int闰月之月份, )当年每月天数列表及闰月月份
     """
     leap_month = (month_code & 0b1111000000000000) >> 12
     return (
-        [month_days_pusher(month_code, i) for i in range(leap_month)][::-1]
+        [month_days_pusher(month_code, i) for i in range(11, 11 - leap_month, -1)]
         + [
             leap_days,
         ]
-        + [month_days_pusher(month_code, i) for i in range(leap_month, 12)][::-1]
+        + [month_days_pusher(month_code, i) for i in range(11 - leap_month, -1, -1)]
         if leap_month
         else [month_days_pusher(month_code, i) for i in range(12)][::-1]
     ), leap_month
 
 
 get_lunar_month_code: Callable[[int], int] = lambda solar_year: int.from_bytes(
     LUNAR_MONTH_PER_YEAR[(solar_year - 1900) * 2 : (solar_year - 1899) * 2],
```

### Comparing `zhdatetime-1.0.2/zhDateTime/types.py` & `zhdatetime-1.0.3/zhDateTime/types.py`

 * *Files identical despite different names*

### Comparing `zhdatetime-1.0.2/zhDateTime.egg-info/PKG-INFO` & `zhdatetime-1.0.3/zhDateTime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhDateTime
-Version: 1.0.2
+Version: 1.0.3
 Summary: 一个简单的小巧的中式日期时间库，附带数字汉字化操作。
 Home-page: https://gitee.com/EillesWan/zhDateTime
 Author: Eilles Wan
 Author-email: EillesWan@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

