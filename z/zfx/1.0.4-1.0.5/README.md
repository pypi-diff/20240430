# Comparing `tmp/zfx-1.0.4.tar.gz` & `tmp/zfx-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zfx-1.0.4.tar", last modified: Tue Apr 30 05:45:18 2024, max compression
+gzip compressed data, was "zfx-1.0.5.tar", last modified: Tue Apr 30 06:37:35 2024, max compression
```

## Comparing `zfx-1.0.4.tar` & `zfx-1.0.5.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 05:45:18.407423 zfx-1.0.4/
--rw-rw-rw-   0        0        0      233 2024-04-30 05:45:18.405956 zfx-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-30 05:45:18.407423 zfx-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      507 2024-04-30 05:44:50.000000 zfx-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 05:45:18.388456 zfx-1.0.4/zfx/
--rw-rw-rw-   0        0        0     2505 2024-04-30 05:32:34.000000 zfx-1.0.4/zfx/__init__.py
--rw-rw-rw-   0        0        0     1711 2024-04-30 03:32:01.000000 zfx-1.0.4/zfx/g2g_account_list.py
--rw-rw-rw-   0        0        0     2105 2024-04-30 03:32:10.000000 zfx-1.0.4/zfx/g2g_account_list_s.py
--rw-rw-rw-   0        0        0    10990 2024-04-23 06:27:52.000000 zfx-1.0.4/zfx/zmodule_240414A.py
--rw-rw-rw-   0        0        0      291 2024-04-23 06:36:54.000000 zfx-1.0.4/zfx/zprint.py
--rw-rw-rw-   0        0        0      364 2024-04-30 05:26:52.000000 zfx-1.0.4/zfx/目录_创建.py
--rw-rw-rw-   0        0        0      273 2024-04-30 03:09:39.000000 zfx-1.0.4/zfx/系统_取CPU型号.py
--rw-rw-rw-   0        0        0      225 2024-04-30 03:04:34.000000 zfx-1.0.4/zfx/系统_取剪辑版内容.py
--rw-rw-rw-   0        0        0     1316 2024-04-30 04:11:09.000000 zfx-1.0.4/zfx/系统_取操作系统类别.py
--rw-rw-rw-   0        0        0      588 2024-04-30 04:17:38.000000 zfx-1.0.4/zfx/系统_取时区.py
--rw-rw-rw-   0        0        0      433 2024-04-30 04:34:35.000000 zfx-1.0.4/zfx/系统_取用户名.py
--rw-rw-rw-   0        0        0      787 2024-04-30 04:25:33.000000 zfx-1.0.4/zfx/系统_取硬盘特征字.py
--rw-rw-rw-   0        0        0      263 2024-04-30 03:13:42.000000 zfx-1.0.4/zfx/系统_取系统现行时间.py
--rw-rw-rw-   0        0        0      154 2024-04-30 03:44:02.000000 zfx-1.0.4/zfx/系统_强制关机.py
--rw-rw-rw-   0        0        0      240 2024-04-30 03:48:40.000000 zfx-1.0.4/zfx/系统_强制注销.py
--rw-rw-rw-   0        0        0      240 2024-04-30 03:47:12.000000 zfx-1.0.4/zfx/系统_强制重启.py
--rw-rw-rw-   0        0        0      454 2024-04-30 04:38:22.000000 zfx-1.0.4/zfx/系统_是否为管理员.py
--rw-rw-rw-   0        0        0      697 2024-04-30 04:43:28.000000 zfx-1.0.4/zfx/系统_是否已联网.py
--rw-rw-rw-   0        0        0      487 2024-04-30 04:04:45.000000 zfx-1.0.4/zfx/系统_清空回收站.py
--rw-rw-rw-   0        0        0      175 2024-04-30 03:04:01.000000 zfx-1.0.4/zfx/系统_置剪辑版内容.py
--rw-rw-rw-   0        0        0     3299 2024-04-25 02:56:01.000000 zfx-1.0.4/zfx/系统任务计划_创建.py
--rw-rw-rw-   0        0        0      267 2024-04-25 02:26:25.000000 zfx-1.0.4/zfx/系统任务计划_删除.py
--rw-rw-rw-   0        0        0      665 2024-04-25 02:26:25.000000 zfx-1.0.4/zfx/系统任务计划_遍历名称.py
--rw-rw-rw-   0        0        0      494 2024-04-30 05:31:14.000000 zfx-1.0.4/zfx/进程_名取ID.py
-drwxrwxrwx   0        0        0        0 2024-04-30 05:45:18.404966 zfx-1.0.4/zfx.egg-info/
--rw-rw-rw-   0        0        0      233 2024-04-30 05:45:18.000000 zfx-1.0.4/zfx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2024-04-30 05:45:18.000000 zfx-1.0.4/zfx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 05:45:18.000000 zfx-1.0.4/zfx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-30 05:45:18.000000 zfx-1.0.4/zfx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-30 05:45:18.000000 zfx-1.0.4/zfx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 06:37:35.292810 zfx-1.0.5/
+-rw-rw-rw-   0        0        0      233 2024-04-30 06:37:35.287819 zfx-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-30 06:37:35.293310 zfx-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      511 2024-04-30 06:37:31.000000 zfx-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:37:35.271848 zfx-1.0.5/zfx/
+-rw-rw-rw-   0        0        0     2663 2024-04-30 06:36:20.000000 zfx-1.0.5/zfx/__init__.py
+-rw-rw-rw-   0        0        0     1711 2024-04-30 03:32:01.000000 zfx-1.0.5/zfx/g2g_account_list.py
+-rw-rw-rw-   0        0        0     2105 2024-04-30 03:32:10.000000 zfx-1.0.5/zfx/g2g_account_list_s.py
+-rw-rw-rw-   0        0        0    10990 2024-04-23 06:27:52.000000 zfx-1.0.5/zfx/zmodule_240414A.py
+-rw-rw-rw-   0        0        0      291 2024-04-23 06:36:54.000000 zfx-1.0.5/zfx/zprint.py
+-rw-rw-rw-   0        0        0      364 2024-04-30 05:26:52.000000 zfx-1.0.5/zfx/目录_创建.py
+-rw-rw-rw-   0        0        0      273 2024-04-30 03:09:39.000000 zfx-1.0.5/zfx/系统_取CPU型号.py
+-rw-rw-rw-   0        0        0      225 2024-04-30 03:04:34.000000 zfx-1.0.5/zfx/系统_取剪辑版内容.py
+-rw-rw-rw-   0        0        0     1316 2024-04-30 04:11:09.000000 zfx-1.0.5/zfx/系统_取操作系统类别.py
+-rw-rw-rw-   0        0        0      588 2024-04-30 04:17:38.000000 zfx-1.0.5/zfx/系统_取时区.py
+-rw-rw-rw-   0        0        0      433 2024-04-30 04:34:35.000000 zfx-1.0.5/zfx/系统_取用户名.py
+-rw-rw-rw-   0        0        0      787 2024-04-30 04:25:33.000000 zfx-1.0.5/zfx/系统_取硬盘特征字.py
+-rw-rw-rw-   0        0        0      263 2024-04-30 03:13:42.000000 zfx-1.0.5/zfx/系统_取系统现行时间.py
+-rw-rw-rw-   0        0        0      154 2024-04-30 03:44:02.000000 zfx-1.0.5/zfx/系统_强制关机.py
+-rw-rw-rw-   0        0        0      240 2024-04-30 03:48:40.000000 zfx-1.0.5/zfx/系统_强制注销.py
+-rw-rw-rw-   0        0        0      240 2024-04-30 03:47:12.000000 zfx-1.0.5/zfx/系统_强制重启.py
+-rw-rw-rw-   0        0        0      454 2024-04-30 04:38:22.000000 zfx-1.0.5/zfx/系统_是否为管理员.py
+-rw-rw-rw-   0        0        0      697 2024-04-30 04:43:28.000000 zfx-1.0.5/zfx/系统_是否已联网.py
+-rw-rw-rw-   0        0        0      487 2024-04-30 04:04:45.000000 zfx-1.0.5/zfx/系统_清空回收站.py
+-rw-rw-rw-   0        0        0      175 2024-04-30 03:04:01.000000 zfx-1.0.5/zfx/系统_置剪辑版内容.py
+-rw-rw-rw-   0        0        0     3299 2024-04-25 02:56:01.000000 zfx-1.0.5/zfx/系统任务计划_创建.py
+-rw-rw-rw-   0        0        0      267 2024-04-25 02:26:25.000000 zfx-1.0.5/zfx/系统任务计划_删除.py
+-rw-rw-rw-   0        0        0      665 2024-04-25 02:26:25.000000 zfx-1.0.5/zfx/系统任务计划_遍历名称.py
+-rw-rw-rw-   0        0        0      377 2024-04-30 06:36:20.000000 zfx-1.0.5/zfx/编码_十六进制文本到字符串.py
+-rw-rw-rw-   0        0        0      368 2024-04-30 06:36:20.000000 zfx-1.0.5/zfx/编码_字符串到十六进制文本.py
+-rw-rw-rw-   0        0        0      494 2024-04-30 05:31:14.000000 zfx-1.0.5/zfx/进程_名取ID.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:37:35.286820 zfx-1.0.5/zfx.egg-info/
+-rw-rw-rw-   0        0        0      233 2024-04-30 06:37:35.000000 zfx-1.0.5/zfx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      907 2024-04-30 06:37:35.000000 zfx-1.0.5/zfx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 06:37:35.000000 zfx-1.0.5/zfx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-30 06:37:35.000000 zfx-1.0.5/zfx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-30 06:37:35.000000 zfx-1.0.5/zfx.egg-info/top_level.txt
```

### Comparing `zfx-1.0.4/zfx/__init__.py` & `zfx-1.0.5/zfx/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,9 +39,11 @@
 from zfx.系统_强制重启 import 系统_强制重启
 from zfx.系统_是否为管理员 import 系统_是否为管理员
 from zfx.系统_是否已联网 import 系统_是否已联网
 from zfx.系统_清空回收站 import 系统_清空回收站
 from zfx.系统_置剪辑版内容 import 系统_置剪辑版内容
 from zfx.系统任务计划_删除 import 系统任务计划_删除
 from zfx.系统任务计划_遍历名称 import 系统任务计划_遍历名称
+from zfx.十六进制文本转字符串 import 十六进制文本转字符串
+from zfx.字符串转十六进制文本 import 字符串转十六进制文本
 from zfx.进程_名取ID import 进程_名取ID
```

### Comparing `zfx-1.0.4/zfx/g2g_account_list.py` & `zfx-1.0.5/zfx/g2g_account_list.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.4/zfx/g2g_account_list_s.py` & `zfx-1.0.5/zfx/g2g_account_list_s.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.4/zfx/zmodule_240414A.py` & `zfx-1.0.5/zfx/zmodule_240414A.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.4/zfx/系统_取操作系统类别.py` & `zfx-1.0.5/zfx/系统_取操作系统类别.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.4/zfx/系统_取时区.py` & `zfx-1.0.5/zfx/系统_取时区.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.4/zfx/系统_取硬盘特征字.py` & `zfx-1.0.5/zfx/系统_取硬盘特征字.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.4/zfx/系统_是否已联网.py` & `zfx-1.0.5/zfx/系统_是否已联网.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.4/zfx/系统任务计划_创建.py` & `zfx-1.0.5/zfx/系统任务计划_创建.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.4/zfx/系统任务计划_遍历名称.py` & `zfx-1.0.5/zfx/系统任务计划_遍历名称.py`

 * *Files identical despite different names*

