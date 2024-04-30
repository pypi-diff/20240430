# Comparing `tmp/zfx-1.0.6.tar.gz` & `tmp/zfx-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zfx-1.0.6.tar", last modified: Tue Apr 30 06:40:36 2024, max compression
+gzip compressed data, was "zfx-1.0.7.tar", last modified: Tue Apr 30 07:40:54 2024, max compression
```

## Comparing `zfx-1.0.6.tar` & `zfx-1.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 06:40:36.654571 zfx-1.0.6/
--rw-rw-rw-   0        0        0      233 2024-04-30 06:40:36.653080 zfx-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-30 06:40:36.655074 zfx-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      511 2024-04-30 06:40:31.000000 zfx-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:40:36.639068 zfx-1.0.6/zfx/
--rw-rw-rw-   0        0        0     2691 2024-04-30 06:40:31.000000 zfx-1.0.6/zfx/__init__.py
--rw-rw-rw-   0        0        0     1711 2024-04-30 03:32:01.000000 zfx-1.0.6/zfx/g2g_account_list.py
--rw-rw-rw-   0        0        0     2105 2024-04-30 03:32:10.000000 zfx-1.0.6/zfx/g2g_account_list_s.py
--rw-rw-rw-   0        0        0    10990 2024-04-23 06:27:52.000000 zfx-1.0.6/zfx/zmodule_240414A.py
--rw-rw-rw-   0        0        0      291 2024-04-23 06:36:54.000000 zfx-1.0.6/zfx/zprint.py
--rw-rw-rw-   0        0        0      364 2024-04-30 05:26:52.000000 zfx-1.0.6/zfx/目录_创建.py
--rw-rw-rw-   0        0        0      273 2024-04-30 03:09:39.000000 zfx-1.0.6/zfx/系统_取CPU型号.py
--rw-rw-rw-   0        0        0      225 2024-04-30 03:04:34.000000 zfx-1.0.6/zfx/系统_取剪辑版内容.py
--rw-rw-rw-   0        0        0     1316 2024-04-30 04:11:09.000000 zfx-1.0.6/zfx/系统_取操作系统类别.py
--rw-rw-rw-   0        0        0      588 2024-04-30 04:17:38.000000 zfx-1.0.6/zfx/系统_取时区.py
--rw-rw-rw-   0        0        0      433 2024-04-30 04:34:35.000000 zfx-1.0.6/zfx/系统_取用户名.py
--rw-rw-rw-   0        0        0      787 2024-04-30 04:25:33.000000 zfx-1.0.6/zfx/系统_取硬盘特征字.py
--rw-rw-rw-   0        0        0      263 2024-04-30 03:13:42.000000 zfx-1.0.6/zfx/系统_取系统现行时间.py
--rw-rw-rw-   0        0        0      154 2024-04-30 03:44:02.000000 zfx-1.0.6/zfx/系统_强制关机.py
--rw-rw-rw-   0        0        0      240 2024-04-30 03:48:40.000000 zfx-1.0.6/zfx/系统_强制注销.py
--rw-rw-rw-   0        0        0      240 2024-04-30 03:47:12.000000 zfx-1.0.6/zfx/系统_强制重启.py
--rw-rw-rw-   0        0        0      454 2024-04-30 04:38:22.000000 zfx-1.0.6/zfx/系统_是否为管理员.py
--rw-rw-rw-   0        0        0      697 2024-04-30 04:43:28.000000 zfx-1.0.6/zfx/系统_是否已联网.py
--rw-rw-rw-   0        0        0      487 2024-04-30 04:04:45.000000 zfx-1.0.6/zfx/系统_清空回收站.py
--rw-rw-rw-   0        0        0      175 2024-04-30 03:04:01.000000 zfx-1.0.6/zfx/系统_置剪辑版内容.py
--rw-rw-rw-   0        0        0     3299 2024-04-25 02:56:01.000000 zfx-1.0.6/zfx/系统任务计划_创建.py
--rw-rw-rw-   0        0        0      267 2024-04-25 02:26:25.000000 zfx-1.0.6/zfx/系统任务计划_删除.py
--rw-rw-rw-   0        0        0      665 2024-04-25 02:26:25.000000 zfx-1.0.6/zfx/系统任务计划_遍历名称.py
--rw-rw-rw-   0        0        0      384 2024-04-30 06:40:31.000000 zfx-1.0.6/zfx/编码_十六进制文本到字符串.py
--rw-rw-rw-   0        0        0      375 2024-04-30 06:40:31.000000 zfx-1.0.6/zfx/编码_字符串到十六进制文本.py
--rw-rw-rw-   0        0        0      494 2024-04-30 05:31:14.000000 zfx-1.0.6/zfx/进程_名取ID.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:40:36.651577 zfx-1.0.6/zfx.egg-info/
--rw-rw-rw-   0        0        0      233 2024-04-30 06:40:36.000000 zfx-1.0.6/zfx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      907 2024-04-30 06:40:36.000000 zfx-1.0.6/zfx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 06:40:36.000000 zfx-1.0.6/zfx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-30 06:40:36.000000 zfx-1.0.6/zfx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-30 06:40:36.000000 zfx-1.0.6/zfx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 07:40:54.332756 zfx-1.0.7/
+-rw-rw-rw-   0        0        0      233 2024-04-30 07:40:54.329762 zfx-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-30 07:40:54.332756 zfx-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      511 2024-04-30 07:40:50.000000 zfx-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:40:54.316786 zfx-1.0.7/zfx/
+-rw-rw-rw-   0        0        0     2726 2024-04-30 07:40:50.000000 zfx-1.0.7/zfx/__init__.py
+-rw-rw-rw-   0        0        0     1711 2024-04-30 03:32:01.000000 zfx-1.0.7/zfx/g2g_account_list.py
+-rw-rw-rw-   0        0        0     2105 2024-04-30 03:32:10.000000 zfx-1.0.7/zfx/g2g_account_list_s.py
+-rw-rw-rw-   0        0        0    10990 2024-04-23 06:27:52.000000 zfx-1.0.7/zfx/zmodule_240414A.py
+-rw-rw-rw-   0        0        0      905 2024-04-30 07:38:51.000000 zfx-1.0.7/zfx/zprint.py
+-rw-rw-rw-   0        0        0      364 2024-04-30 05:26:52.000000 zfx-1.0.7/zfx/目录_创建.py
+-rw-rw-rw-   0        0        0      273 2024-04-30 03:09:39.000000 zfx-1.0.7/zfx/系统_取CPU型号.py
+-rw-rw-rw-   0        0        0      225 2024-04-30 03:04:34.000000 zfx-1.0.7/zfx/系统_取剪辑版内容.py
+-rw-rw-rw-   0        0        0     1316 2024-04-30 04:11:09.000000 zfx-1.0.7/zfx/系统_取操作系统类别.py
+-rw-rw-rw-   0        0        0      588 2024-04-30 04:17:38.000000 zfx-1.0.7/zfx/系统_取时区.py
+-rw-rw-rw-   0        0        0      433 2024-04-30 04:34:35.000000 zfx-1.0.7/zfx/系统_取用户名.py
+-rw-rw-rw-   0        0        0      787 2024-04-30 04:25:33.000000 zfx-1.0.7/zfx/系统_取硬盘特征字.py
+-rw-rw-rw-   0        0        0      263 2024-04-30 03:13:42.000000 zfx-1.0.7/zfx/系统_取系统现行时间.py
+-rw-rw-rw-   0        0        0      154 2024-04-30 03:44:02.000000 zfx-1.0.7/zfx/系统_强制关机.py
+-rw-rw-rw-   0        0        0      240 2024-04-30 03:48:40.000000 zfx-1.0.7/zfx/系统_强制注销.py
+-rw-rw-rw-   0        0        0      240 2024-04-30 03:47:12.000000 zfx-1.0.7/zfx/系统_强制重启.py
+-rw-rw-rw-   0        0        0      454 2024-04-30 04:38:22.000000 zfx-1.0.7/zfx/系统_是否为管理员.py
+-rw-rw-rw-   0        0        0      697 2024-04-30 04:43:28.000000 zfx-1.0.7/zfx/系统_是否已联网.py
+-rw-rw-rw-   0        0        0      487 2024-04-30 04:04:45.000000 zfx-1.0.7/zfx/系统_清空回收站.py
+-rw-rw-rw-   0        0        0      175 2024-04-30 03:04:01.000000 zfx-1.0.7/zfx/系统_置剪辑版内容.py
+-rw-rw-rw-   0        0        0     3299 2024-04-25 02:56:01.000000 zfx-1.0.7/zfx/系统任务计划_创建.py
+-rw-rw-rw-   0        0        0      267 2024-04-25 02:26:25.000000 zfx-1.0.7/zfx/系统任务计划_删除.py
+-rw-rw-rw-   0        0        0      665 2024-04-25 02:26:25.000000 zfx-1.0.7/zfx/系统任务计划_遍历名称.py
+-rw-rw-rw-   0        0        0      384 2024-04-30 06:40:31.000000 zfx-1.0.7/zfx/编码_十六进制文本到字符串.py
+-rw-rw-rw-   0        0        0      375 2024-04-30 06:40:31.000000 zfx-1.0.7/zfx/编码_字符串到十六进制文本.py
+-rw-rw-rw-   0        0        0      494 2024-04-30 05:31:14.000000 zfx-1.0.7/zfx/进程_名取ID.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:40:54.328764 zfx-1.0.7/zfx.egg-info/
+-rw-rw-rw-   0        0        0      233 2024-04-30 07:40:54.000000 zfx-1.0.7/zfx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      907 2024-04-30 07:40:54.000000 zfx-1.0.7/zfx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 07:40:54.000000 zfx-1.0.7/zfx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-30 07:40:54.000000 zfx-1.0.7/zfx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-30 07:40:54.000000 zfx-1.0.7/zfx.egg-info/top_level.txt
```

### Comparing `zfx-1.0.6/zfx/__init__.py` & `zfx-1.0.7/zfx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from zfx.g2g_account_list import g2g_account_list
 from zfx.g2g_account_list_s import g2g_account_list_s
-from zfx.zprint import en_print
-from zfx.zprint import dis_print
-from zfx.zprint import zprint
-from zfx.zprint import zdebug
+from zfx.zprint import 打印_开启
+from zfx.zprint import 打印_关闭
+from zfx.zprint import 打印_普通打印
+from zfx.zprint import 打印_强制打印
 from zfx.zmodule_240414A import 延迟
 from zfx.zmodule_240414A import 文本_到大写
 from zfx.zmodule_240414A import 文本_到小写
 from zfx.zmodule_240414A import 文本_颠倒
 from zfx.zmodule_240414A import 文本_分割文本
 from zfx.zmodule_240414A import 文本_加密
 from zfx.zmodule_240414A import 文本_解密
```

### Comparing `zfx-1.0.6/zfx/g2g_account_list.py` & `zfx-1.0.7/zfx/g2g_account_list.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.6/zfx/g2g_account_list_s.py` & `zfx-1.0.7/zfx/g2g_account_list_s.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.6/zfx/zmodule_240414A.py` & `zfx-1.0.7/zfx/zmodule_240414A.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.6/zfx/系统_取操作系统类别.py` & `zfx-1.0.7/zfx/系统_取操作系统类别.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.6/zfx/系统_取时区.py` & `zfx-1.0.7/zfx/系统_取时区.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.6/zfx/系统_取硬盘特征字.py` & `zfx-1.0.7/zfx/系统_取硬盘特征字.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.6/zfx/系统_是否已联网.py` & `zfx-1.0.7/zfx/系统_是否已联网.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.6/zfx/系统任务计划_创建.py` & `zfx-1.0.7/zfx/系统任务计划_创建.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.6/zfx/系统任务计划_遍历名称.py` & `zfx-1.0.7/zfx/系统任务计划_遍历名称.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.6/zfx.egg-info/SOURCES.txt` & `zfx-1.0.7/zfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

