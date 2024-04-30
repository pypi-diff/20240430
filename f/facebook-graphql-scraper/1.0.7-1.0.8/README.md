# Comparing `tmp/facebook-graphql-scraper-1.0.7.tar.gz` & `tmp/facebook-graphql-scraper-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook-graphql-scraper-1.0.7.tar", last modified: Fri Apr 26 08:57:21 2024, max compression
+gzip compressed data, was "facebook-graphql-scraper-1.0.8.tar", last modified: Tue Apr 30 07:27:06 2024, max compression
```

## Comparing `facebook-graphql-scraper-1.0.7.tar` & `facebook-graphql-scraper-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.108841 facebook-graphql-scraper-1.0.7/
--rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.7/LICENSE
--rw-r--r--   0 renren     (501) staff       (20)     7036 2024-04-26 08:57:21.108485 facebook-graphql-scraper-1.0.7/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)     6548 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/README.md
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.103835 facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/
--rw-r--r--   0 renren     (501) staff       (20)     7036 2024-04-26 08:57:21.000000 facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/PKG-INFO
--rw-r--r--   0 renren     (501) staff       (20)      657 2024-04-26 08:57:21.000000 facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-26 08:57:21.000000 facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-26 08:57:21.000000 facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.104665 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.105337 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/base/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/base/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/base/base_page.py
--rw-r--r--   0 renren     (501) staff       (20)     1367 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/example.py
--rw-r--r--   0 renren     (501) staff       (20)     9668 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/facebook_graphql_scraper.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.106037 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/pages/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/pages/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     4746 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/pages/page_optional.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.106520 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/tests/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/tests/__init__.py
-drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-26 08:57:21.107733 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/
--rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/__init__.py
--rw-r--r--   0 renren     (501) staff       (20)     2883 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/locator.py
--rw-r--r--   0 renren     (501) staff       (20)     3813 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/parser.py
--rw-r--r--   0 renren     (501) staff       (20)     6324 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/utils.py
--rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-26 08:57:21.108959 facebook-graphql-scraper-1.0.7/setup.cfg
--rw-r--r--   0 renren     (501) staff       (20)      863 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.7/setup.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.139473 facebook-graphql-scraper-1.0.8/
+-rw-r--r--   0 renren     (501) staff       (20)     1055 2024-04-02 15:04:14.000000 facebook-graphql-scraper-1.0.8/LICENSE
+-rw-r--r--   0 renren     (501) staff       (20)     7036 2024-04-30 07:27:06.139157 facebook-graphql-scraper-1.0.8/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)     6548 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/README.md
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.134889 facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/
+-rw-r--r--   0 renren     (501) staff       (20)     7036 2024-04-30 07:27:06.000000 facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 renren     (501) staff       (20)      657 2024-04-30 07:27:06.000000 facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 renren     (501) staff       (20)        1 2024-04-30 07:27:06.000000 facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 renren     (501) staff       (20)       19 2024-04-30 07:27:06.000000 facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.135604 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.136175 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/base/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 07:27:32.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/base/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)      822 2024-04-03 07:55:30.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/base/base_page.py
+-rw-r--r--   0 renren     (501) staff       (20)     1367 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/example.py
+-rw-r--r--   0 renren     (501) staff       (20)     9759 2024-04-30 07:26:22.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/facebook_graphql_scraper.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.136927 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/pages/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:07.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/pages/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     4746 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/pages/page_optional.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.137334 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/tests/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/tests/__init__.py
+drwxr-xr-x   0 renren     (501) staff       (20)        0 2024-04-30 07:27:06.138419 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/
+-rw-r--r--   0 renren     (501) staff       (20)        0 2024-04-03 06:55:08.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/__init__.py
+-rw-r--r--   0 renren     (501) staff       (20)     2883 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/locator.py
+-rw-r--r--   0 renren     (501) staff       (20)     3813 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/parser.py
+-rw-r--r--   0 renren     (501) staff       (20)     6324 2024-04-26 08:56:24.000000 facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/utils.py
+-rw-r--r--   0 renren     (501) staff       (20)       38 2024-04-30 07:27:06.139548 facebook-graphql-scraper-1.0.8/setup.cfg
+-rw-r--r--   0 renren     (501) staff       (20)      863 2024-04-30 07:26:22.000000 facebook-graphql-scraper-1.0.8/setup.py
```

### Comparing `facebook-graphql-scraper-1.0.7/LICENSE` & `facebook-graphql-scraper-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.7/PKG-INFO` & `facebook-graphql-scraper-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 1.0.7
+Version: 1.0.8
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/FB_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-1.0.7/README.md` & `facebook-graphql-scraper-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/PKG-INFO` & `facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-graphql-scraper
-Version: 1.0.7
+Version: 1.0.8
 Summary: Implement Facebook scraper for post data retrieval
 Home-page: https://github.com/FaustRen/FB_graphql_scraper
 Author: FaustRen
 Author-email: faustren1z@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `facebook-graphql-scraper-1.0.7/facebook_graphql_scraper.egg-info/SOURCES.txt` & `facebook-graphql-scraper-1.0.8/facebook_graphql_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/base/base_page.py` & `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/base/base_page.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/example.py` & `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/example.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/facebook_graphql_scraper.py` & `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/facebook_graphql_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,15 @@
                 reactions_in=each_reactions)
             reactions_out.append(processed_reactions)
         return reactions_out
 
     def get_user_posts(self, fb_username_or_userid: str, days_limit: int = 61, display_progress:bool=True) -> dict:
         url = "https://www.facebook.com/"+fb_username_or_userid # 建立完整user連結
         self.move_to_next_kol(url=url)# driver 跳至該連結
+        self.move_to_next_kol(url=url)# 徹底清除requests避免參雜上一用戶資料
         self.requests_parser.clean_res() # 清空所有用於儲存結果的array
         self.set_container() # 清空用於儲存貼文資訊的array
         self.set_stop_point() # 設置/重置停止條件 | 停止條件: 瀏覽器無法往下取得更多貼文(n次) or 已取得目標天數內貼文
 
         # If you did not login, click X button
         if self.fb_account == None: self.page_optional.click_reject_login_button()
```

### Comparing `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/pages/page_optional.py` & `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/pages/page_optional.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/locator.py` & `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/locator.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/parser.py` & `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/parser.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.7/fb_graphql_scraper/utils/utils.py` & `facebook-graphql-scraper-1.0.8/fb_graphql_scraper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `facebook-graphql-scraper-1.0.7/setup.py` & `facebook-graphql-scraper-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import setuptools
 from setuptools import setup, find_packages
 
 setup(
     name='facebook-graphql-scraper',
-    version='1.0.7',
+    version='1.0.8',
     packages=[
         "fb_graphql_scraper",
         "fb_graphql_scraper.pages",
         "fb_graphql_scraper.base",
         "fb_graphql_scraper.tests", 
         "fb_graphql_scraper.utils",
         ],
```

