# Comparing `tmp/zfx-20240430a0.tar.gz` & `tmp/zfx-20240430b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zfx-20240430a0.tar", last modified: Tue Apr 30 03:20:54 2024, max compression
+gzip compressed data, was "zfx-20240430b0.tar", last modified: Tue Apr 30 03:32:54 2024, max compression
```

## Comparing `zfx-20240430a0.tar` & `zfx-20240430b0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 03:20:54.135158 zfx-20240430a0/
--rw-rw-rw-   0        0        0      191 2024-04-30 03:20:54.133160 zfx-20240430a0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-30 03:20:54.135656 zfx-20240430a0/setup.cfg
--rw-rw-rw-   0        0        0      472 2024-04-30 03:20:14.000000 zfx-20240430a0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:20:54.116192 zfx-20240430a0/zfx/
--rw-rw-rw-   0        0        0     1789 2024-04-30 03:15:29.000000 zfx-20240430a0/zfx/__init__.py
--rw-rw-rw-   0        0        0     1703 2024-04-26 10:03:45.000000 zfx-20240430a0/zfx/g2g_account_list.py
--rw-rw-rw-   0        0        0     2097 2024-04-26 10:03:45.000000 zfx-20240430a0/zfx/g2g_account_list_s.py
--rw-rw-rw-   0        0        0    10990 2024-04-23 06:27:52.000000 zfx-20240430a0/zfx/zmodule_240414A.py
--rw-rw-rw-   0        0        0      291 2024-04-23 06:36:54.000000 zfx-20240430a0/zfx/zprint.py
--rw-rw-rw-   0        0        0      273 2024-04-30 03:09:39.000000 zfx-20240430a0/zfx/系统_取CPU型号.py
--rw-rw-rw-   0        0        0      225 2024-04-30 03:04:34.000000 zfx-20240430a0/zfx/系统_取剪辑版内容.py
--rw-rw-rw-   0        0        0      263 2024-04-30 03:13:42.000000 zfx-20240430a0/zfx/系统_取系统现行时间.py
--rw-rw-rw-   0        0        0      175 2024-04-30 03:04:01.000000 zfx-20240430a0/zfx/系统_置剪辑版内容.py
--rw-rw-rw-   0        0        0     3299 2024-04-25 02:56:01.000000 zfx-20240430a0/zfx/系统任务计划_创建.py
--rw-rw-rw-   0        0        0      267 2024-04-25 02:26:25.000000 zfx-20240430a0/zfx/系统任务计划_删除.py
--rw-rw-rw-   0        0        0      665 2024-04-25 02:26:25.000000 zfx-20240430a0/zfx/系统任务计划_遍历名称.py
-drwxrwxrwx   0        0        0        0 2024-04-30 03:20:54.131163 zfx-20240430a0/zfx.egg-info/
--rw-rw-rw-   0        0        0      191 2024-04-30 03:20:53.000000 zfx-20240430a0/zfx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2024-04-30 03:20:53.000000 zfx-20240430a0/zfx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 03:20:53.000000 zfx-20240430a0/zfx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-30 03:20:53.000000 zfx-20240430a0/zfx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-30 03:20:53.000000 zfx-20240430a0/zfx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:54.310767 zfx-20240430b0/
+-rw-rw-rw-   0        0        0      191 2024-04-30 03:32:54.309768 zfx-20240430b0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-30 03:32:54.311265 zfx-20240430b0/setup.cfg
+-rw-rw-rw-   0        0        0      472 2024-04-30 03:32:45.000000 zfx-20240430b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:54.295295 zfx-20240430b0/zfx/
+-rw-rw-rw-   0        0        0     1789 2024-04-30 03:15:29.000000 zfx-20240430b0/zfx/__init__.py
+-rw-rw-rw-   0        0        0     1711 2024-04-30 03:32:01.000000 zfx-20240430b0/zfx/g2g_account_list.py
+-rw-rw-rw-   0        0        0     2105 2024-04-30 03:32:10.000000 zfx-20240430b0/zfx/g2g_account_list_s.py
+-rw-rw-rw-   0        0        0    10990 2024-04-23 06:27:52.000000 zfx-20240430b0/zfx/zmodule_240414A.py
+-rw-rw-rw-   0        0        0      291 2024-04-23 06:36:54.000000 zfx-20240430b0/zfx/zprint.py
+-rw-rw-rw-   0        0        0      273 2024-04-30 03:09:39.000000 zfx-20240430b0/zfx/系统_取CPU型号.py
+-rw-rw-rw-   0        0        0      225 2024-04-30 03:04:34.000000 zfx-20240430b0/zfx/系统_取剪辑版内容.py
+-rw-rw-rw-   0        0        0      263 2024-04-30 03:13:42.000000 zfx-20240430b0/zfx/系统_取系统现行时间.py
+-rw-rw-rw-   0        0        0      175 2024-04-30 03:04:01.000000 zfx-20240430b0/zfx/系统_置剪辑版内容.py
+-rw-rw-rw-   0        0        0     3299 2024-04-25 02:56:01.000000 zfx-20240430b0/zfx/系统任务计划_创建.py
+-rw-rw-rw-   0        0        0      267 2024-04-25 02:26:25.000000 zfx-20240430b0/zfx/系统任务计划_删除.py
+-rw-rw-rw-   0        0        0      665 2024-04-25 02:26:25.000000 zfx-20240430b0/zfx/系统任务计划_遍历名称.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:32:54.308271 zfx-20240430b0/zfx.egg-info/
+-rw-rw-rw-   0        0        0      191 2024-04-30 03:32:54.000000 zfx-20240430b0/zfx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2024-04-30 03:32:54.000000 zfx-20240430b0/zfx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 03:32:54.000000 zfx-20240430b0/zfx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-30 03:32:54.000000 zfx-20240430b0/zfx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-30 03:32:54.000000 zfx-20240430b0/zfx.egg-info/top_level.txt
```

### Comparing `zfx-20240430a0/zfx/__init__.py` & `zfx-20240430b0/zfx/__init__.py`

 * *Files identical despite different names*

### Comparing `zfx-20240430a0/zfx/g2g_account_list.py` & `zfx-20240430b0/zfx/g2g_account_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,13 +41,13 @@
                 products_list.append(product_dict)
     except requests.exceptions.RequestException as e:
         print("网络请求错误:", e)
 
     return products_list
 
 
-# 调用函数并打印结果
-结果 = g2g_account_list(1)
-for product in 结果:
-    print(product)
+# # 调用函数并打印结果
+# 结果 = g2g_account_list(1)
+# for product in 结果:
+#     print(product)
```

### Comparing `zfx-20240430a0/zfx/g2g_account_list_s.py` & `zfx-20240430b0/zfx/g2g_account_list_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,11 +48,11 @@
                 break
     except requests.exceptions.RequestException as e:
         print("网络请求错误:", e)
 
     return products_list
 
 
-# 调用函数并打印结果
-结果 = g2g_account_list_s()
-for product in 结果:
-    print(product)
+# # 调用函数并打印结果
+# 结果 = g2g_account_list_s()
+# for product in 结果:
+#     print(product)
```

### Comparing `zfx-20240430a0/zfx/zmodule_240414A.py` & `zfx-20240430b0/zfx/zmodule_240414A.py`

 * *Files identical despite different names*

### Comparing `zfx-20240430a0/zfx/系统任务计划_创建.py` & `zfx-20240430b0/zfx/系统任务计划_创建.py`

 * *Files identical despite different names*

### Comparing `zfx-20240430a0/zfx/系统任务计划_遍历名称.py` & `zfx-20240430b0/zfx/系统任务计划_遍历名称.py`

 * *Files identical despite different names*

