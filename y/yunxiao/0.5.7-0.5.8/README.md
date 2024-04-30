# Comparing `tmp/yunxiao-0.5.7.tar.gz` & `tmp/yunxiao-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.5.7.tar", last modified: Tue Apr 30 16:12:00 2024, max compression
+gzip compressed data, was "yunxiao-0.5.8.tar", last modified: Tue Apr 30 16:39:14 2024, max compression
```

## Comparing `yunxiao-0.5.7.tar` & `yunxiao-0.5.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 16:12:00.957183 yunxiao-0.5.7/
--rw-rw-rw-   0        0        0      509 2024-04-30 16:12:00.956184 yunxiao-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.7/README.md
--rw-rw-rw-   0        0        0     2443 2024-04-30 16:11:30.000000 yunxiao-0.5.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 16:12:00.957183 yunxiao-0.5.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 16:12:00.926605 yunxiao-0.5.7/yunxiao/
--rw-rw-rw-   0        0        0       87 2024-04-25 16:28:49.000000 yunxiao-0.5.7/yunxiao/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:12:00.955184 yunxiao-0.5.7/yunxiao/schemas/
--rw-rw-rw-   0        0        0      403 2024-04-30 15:15:40.000000 yunxiao-0.5.7/yunxiao/schemas/__init__.py
--rw-rw-rw-   0        0        0     2406 2024-04-30 13:07:02.000000 yunxiao-0.5.7/yunxiao/schemas/achievements.py
--rw-rw-rw-   0        0        0      346 2024-04-30 12:00:14.000000 yunxiao-0.5.7/yunxiao/schemas/page.py
--rw-rw-rw-   0        0        0     4157 2024-04-30 15:41:58.000000 yunxiao-0.5.7/yunxiao/schemas/payments.py
--rw-rw-rw-   0        0        0     2383 2024-04-30 12:00:14.000000 yunxiao-0.5.7/yunxiao/schemas/teachers.py
--rw-rw-rw-   0        0        0    33659 2024-04-30 16:11:30.000000 yunxiao-0.5.7/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:12:00.956184 yunxiao-0.5.7/yunxiao.egg-info/
--rw-rw-rw-   0        0        0      509 2024-04-30 16:12:00.000000 yunxiao-0.5.7/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-04-30 16:12:00.000000 yunxiao-0.5.7/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 16:12:00.000000 yunxiao-0.5.7/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 16:12:00.000000 yunxiao-0.5.7/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-30 16:12:00.000000 yunxiao-0.5.7/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 16:39:14.055216 yunxiao-0.5.8/
+-rw-rw-rw-   0        0        0      509 2024-04-30 16:39:14.054214 yunxiao-0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.8/README.md
+-rw-rw-rw-   0        0        0     2504 2024-04-30 16:39:03.000000 yunxiao-0.5.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:39:14.055216 yunxiao-0.5.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 16:39:14.040215 yunxiao-0.5.8/yunxiao/
+-rw-rw-rw-   0        0        0       87 2024-04-25 16:28:49.000000 yunxiao-0.5.8/yunxiao/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:39:14.052218 yunxiao-0.5.8/yunxiao/schemas/
+-rw-rw-rw-   0        0        0      403 2024-04-30 15:15:40.000000 yunxiao-0.5.8/yunxiao/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2406 2024-04-30 13:07:02.000000 yunxiao-0.5.8/yunxiao/schemas/achievements.py
+-rw-rw-rw-   0        0        0      346 2024-04-30 12:00:14.000000 yunxiao-0.5.8/yunxiao/schemas/page.py
+-rw-rw-rw-   0        0        0     4157 2024-04-30 15:41:58.000000 yunxiao-0.5.8/yunxiao/schemas/payments.py
+-rw-rw-rw-   0        0        0     2383 2024-04-30 12:00:14.000000 yunxiao-0.5.8/yunxiao/schemas/teachers.py
+-rw-rw-rw-   0        0        0    33724 2024-04-30 16:28:56.000000 yunxiao-0.5.8/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:39:14.053216 yunxiao-0.5.8/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0      509 2024-04-30 16:39:14.000000 yunxiao-0.5.8/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-04-30 16:39:14.000000 yunxiao-0.5.8/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:39:14.000000 yunxiao-0.5.8/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 16:39:14.000000 yunxiao-0.5.8/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-30 16:39:14.000000 yunxiao-0.5.8/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.5.7/pyproject.toml` & `yunxiao-0.5.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.5.7"
+version = "0.5.8"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "sqkkyzx", email = "admin@sqkkyzx.com"},
 ]
 
 dependencies = ["requests"]
@@ -15,14 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.12"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.5.8" = "新增: 对翻页的日志输出启用色彩。"
 "0.5.7" = "新增: 对 payments 引入 pydantic 做数据验证。"
 "0.5.6" = "新增: 对 achievements 引入 pydantic 做数据验证。"
 "0.5.5" = "新增: 对 teacher 引入 pydantic 做数据验证。"
 "0.5.4" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.3" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.2" = "新增（测试）: 引入pydantic做数据验证。"
 "0.5.1" = "新增: '订单组详情'端点;\n改进: '账户明细'端点更改函数名"
```

### Comparing `yunxiao-0.5.7/yunxiao/schemas/achievements.py` & `yunxiao-0.5.8/yunxiao/schemas/achievements.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.5.7/yunxiao/schemas/payments.py` & `yunxiao-0.5.8/yunxiao/schemas/payments.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.5.7/yunxiao/schemas/teachers.py` & `yunxiao-0.5.8/yunxiao/schemas/teachers.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.5.7/yunxiao/yunxiao.py` & `yunxiao-0.5.8/yunxiao/yunxiao.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,18 +117,20 @@
         while payload.page.pageNum <= response.page.totalPage:
             res = self.request(method="post", url=endpoint, json=payload.model_dump())
             try:
                 new = schemas(**res)
                 response.data.extend(new.data)
                 response.page = new.page
 
-                logging.info(f"SIZE-{payload.page.pageSize} "
-                             f"PAGE-{response.page.pageNum}/{response.page.totalPage} "
-                             f"COUNT-{response.page.pageNum * payload.page.pageSize}/{response.page.totalCount} "
-                             f"FROM-{endpoint}")  # 汇报数量
+                logging.info(
+                    f"\033[32m size \033[36m{payload.page.pageSize}"
+                    f"\033[32m page \033[36m{response.page.pageNum}/{response.page.totalPage}"
+                    f"\033[32m count \033[36m{response.page.pageNum * payload.page.pageSize}/{response.page.totalCount}"
+                    f"\033[0m\t{endpoint}"
+                )  # 汇报数量
 
                 payload.page.pageNum += 1  # 翻页
             except TypeError:
                 logging.error(res)
         response.page.pageSize = payload.page.pageSize
         return response
```

