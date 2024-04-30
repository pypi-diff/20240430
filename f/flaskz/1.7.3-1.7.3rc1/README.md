# Comparing `tmp/flaskz-1.7.3.tar.gz` & `tmp/flaskz-1.7.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskz-1.7.3.tar", last modified: Tue Apr 30 16:00:41 2024, max compression
+gzip compressed data, was "flaskz-1.7.3rc1.tar", last modified: Tue Apr 16 02:00:09 2024, max compression
```

## Comparing `flaskz-1.7.3.tar` & `flaskz-1.7.3rc1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-30 16:00:41.741317 flaskz-1.7.3/
--rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2023-12-29 07:22:00.000000 flaskz-1.7.3/LICENSE
--rw-r--r--   0 taozh      (501) staff       (20)     9712 2024-04-30 16:00:41.740800 flaskz-1.7.3/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)     9106 2024-04-30 15:53:38.000000 flaskz-1.7.3/README.md
--rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.7.3/pyproject.toml
--rwxrwxrwx   0 taozh      (501) staff       (20)      775 2024-04-30 16:00:41.742976 flaskz-1.7.3/setup.cfg
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-30 16:00:41.692472 flaskz-1.7.3/src/
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-30 16:00:41.698404 flaskz-1.7.3/src/flaskz/
--rwxrwxrwx   0 taozh      (501) staff       (20)       22 2024-04-29 08:33:26.000000 flaskz-1.7.3/src/flaskz/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-30 16:00:41.703133 flaskz-1.7.3/src/flaskz/auth/
--rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.7.3/src/flaskz/auth/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8563 2023-11-06 11:28:38.000000 flaskz-1.7.3/src/flaskz/auth/_jws.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-30 16:00:41.708428 flaskz-1.7.3/src/flaskz/ext/
--rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.7.3/src/flaskz/ext/__init__.py
--rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-12-11 08:39:54.000000 flaskz-1.7.3/src/flaskz/ext/cypher.py
--rw-r--r--   0 taozh      (501) staff       (20)    22539 2024-04-26 11:27:26.000000 flaskz-1.7.3/src/flaskz/ext/ssh.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-30 16:00:41.710420 flaskz-1.7.3/src/flaskz/log/
--rwxrwxrwx   0 taozh      (501) staff       (20)     2395 2023-07-06 02:14:56.000000 flaskz-1.7.3/src/flaskz/log/__init__.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-30 16:00:41.718069 flaskz-1.7.3/src/flaskz/models/
--rwxrwxrwx   0 taozh      (501) staff       (20)     6102 2024-02-02 04:22:48.000000 flaskz-1.7.3/src/flaskz/models/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    31531 2024-04-14 10:04:24.000000 flaskz-1.7.3/src/flaskz/models/_base.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    11055 2024-01-22 02:47:13.000000 flaskz-1.7.3/src/flaskz/models/_model.py
--rw-r--r--   0 taozh      (501) staff       (20)    20087 2024-04-07 02:45:01.000000 flaskz-1.7.3/src/flaskz/models/_query_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    11212 2024-04-14 09:19:30.000000 flaskz-1.7.3/src/flaskz/models/_util.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.7.3/src/flaskz/res_status_codes.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-30 16:00:41.721590 flaskz-1.7.3/src/flaskz/rest/
--rwxrwxrwx   0 taozh      (501) staff       (20)    21363 2024-01-01 06:50:15.000000 flaskz-1.7.3/src/flaskz/rest/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.7.3/src/flaskz/rest/_mgmt.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     4173 2023-12-30 16:50:29.000000 flaskz-1.7.3/src/flaskz/rest/_util.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-30 16:00:41.736145 flaskz-1.7.3/src/flaskz/utils/
--rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.7.3/src/flaskz/utils/__init__.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2502 2023-12-30 16:37:35.000000 flaskz-1.7.3/src/flaskz/utils/_app.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2848 2023-12-30 16:37:56.000000 flaskz-1.7.3/src/flaskz/utils/_cache.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     7248 2024-04-14 10:55:34.000000 flaskz-1.7.3/src/flaskz/utils/_cls.py
--rwxrwxrwx   0 taozh      (501) staff       (20)    13669 2024-01-17 09:40:36.000000 flaskz-1.7.3/src/flaskz/utils/_common.py
--rw-r--r--   0 taozh      (501) staff       (20)      860 2023-12-30 16:48:17.000000 flaskz-1.7.3/src/flaskz/utils/_func.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.7.3/src/flaskz/utils/_magic.py
--rw-r--r--   0 taozh      (501) staff       (20)     1020 2023-12-30 16:50:25.000000 flaskz-1.7.3/src/flaskz/utils/_private.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     7933 2024-01-30 02:20:56.000000 flaskz-1.7.3/src/flaskz/utils/_request_api.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     1201 2023-12-30 16:50:25.000000 flaskz-1.7.3/src/flaskz/utils/_request_args.py
--rwxrwxrwx   0 taozh      (501) staff       (20)     3045 2024-01-30 02:31:20.000000 flaskz-1.7.3/src/flaskz/utils/_response.py
--rw-r--r--   0 taozh      (501) staff       (20)     4322 2023-12-30 13:56:42.000000 flaskz-1.7.3/src/flaskz/utils/_timer.py
-drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-30 16:00:41.738688 flaskz-1.7.3/src/flaskz.egg-info/
--rw-r--r--   0 taozh      (501) staff       (20)     9712 2024-04-30 16:00:41.000000 flaskz-1.7.3/src/flaskz.egg-info/PKG-INFO
--rwxrwxrwx   0 taozh      (501) staff       (20)      981 2024-04-30 16:00:41.000000 flaskz-1.7.3/src/flaskz.egg-info/SOURCES.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        1 2024-04-30 16:00:41.000000 flaskz-1.7.3/src/flaskz.egg-info/dependency_links.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)       87 2024-04-30 16:00:41.000000 flaskz-1.7.3/src/flaskz.egg-info/requires.txt
--rwxrwxrwx   0 taozh      (501) staff       (20)        7 2024-04-30 16:00:41.000000 flaskz-1.7.3/src/flaskz.egg-info/top_level.txt
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.550594 flaskz-1.7.3rc1/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1070 2023-12-29 07:22:00.000000 flaskz-1.7.3rc1/LICENSE
+-rw-r--r--   0 taozh      (501) staff       (20)     9710 2024-04-16 02:00:09.550215 flaskz-1.7.3rc1/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)     9102 2024-04-15 11:36:23.000000 flaskz-1.7.3rc1/README.md
+-rwxrwxrwx   0 taozh      (501) staff       (20)      108 2021-10-20 06:20:46.000000 flaskz-1.7.3rc1/pyproject.toml
+-rwxrwxrwx   0 taozh      (501) staff       (20)      778 2024-04-16 02:00:09.551653 flaskz-1.7.3rc1/setup.cfg
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.506875 flaskz-1.7.3rc1/src/
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.512737 flaskz-1.7.3rc1/src/flaskz/
+-rwxrwxrwx   0 taozh      (501) staff       (20)       25 2024-04-14 04:30:05.000000 flaskz-1.7.3rc1/src/flaskz/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.516736 flaskz-1.7.3rc1/src/flaskz/auth/
+-rw-r--r--   0 taozh      (501) staff       (20)       20 2022-09-19 02:49:18.000000 flaskz-1.7.3rc1/src/flaskz/auth/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8563 2023-11-06 11:28:38.000000 flaskz-1.7.3rc1/src/flaskz/auth/_jws.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.520306 flaskz-1.7.3rc1/src/flaskz/ext/
+-rw-r--r--   0 taozh      (501) staff       (20)      117 2023-04-27 10:17:39.000000 flaskz-1.7.3rc1/src/flaskz/ext/__init__.py
+-rw-r--r--   0 taozh      (501) staff       (20)     8661 2023-12-11 08:39:54.000000 flaskz-1.7.3rc1/src/flaskz/ext/cypher.py
+-rw-r--r--   0 taozh      (501) staff       (20)    22378 2024-04-15 12:15:00.000000 flaskz-1.7.3rc1/src/flaskz/ext/ssh.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.520831 flaskz-1.7.3rc1/src/flaskz/log/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2395 2023-07-06 02:14:56.000000 flaskz-1.7.3rc1/src/flaskz/log/__init__.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.527060 flaskz-1.7.3rc1/src/flaskz/models/
+-rwxrwxrwx   0 taozh      (501) staff       (20)     6102 2024-02-02 04:22:48.000000 flaskz-1.7.3rc1/src/flaskz/models/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    31531 2024-04-14 10:04:24.000000 flaskz-1.7.3rc1/src/flaskz/models/_base.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    11055 2024-01-22 02:47:13.000000 flaskz-1.7.3rc1/src/flaskz/models/_model.py
+-rw-r--r--   0 taozh      (501) staff       (20)    20087 2024-04-07 02:45:01.000000 flaskz-1.7.3rc1/src/flaskz/models/_query_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    11212 2024-04-14 09:19:30.000000 flaskz-1.7.3rc1/src/flaskz/models/_util.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1316 2021-10-25 05:47:22.000000 flaskz-1.7.3rc1/src/flaskz/res_status_codes.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.531391 flaskz-1.7.3rc1/src/flaskz/rest/
+-rwxrwxrwx   0 taozh      (501) staff       (20)    21363 2024-01-01 06:50:15.000000 flaskz-1.7.3rc1/src/flaskz/rest/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)      960 2023-04-26 02:54:40.000000 flaskz-1.7.3rc1/src/flaskz/rest/_mgmt.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     4173 2023-12-30 16:50:29.000000 flaskz-1.7.3rc1/src/flaskz/rest/_util.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.547250 flaskz-1.7.3rc1/src/flaskz/utils/
+-rwxrwxrwx   0 taozh      (501) staff       (20)      251 2023-06-21 05:37:43.000000 flaskz-1.7.3rc1/src/flaskz/utils/__init__.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2502 2023-12-30 16:37:35.000000 flaskz-1.7.3rc1/src/flaskz/utils/_app.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2848 2023-12-30 16:37:56.000000 flaskz-1.7.3rc1/src/flaskz/utils/_cache.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7248 2024-04-14 10:55:34.000000 flaskz-1.7.3rc1/src/flaskz/utils/_cls.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)    13669 2024-01-17 09:40:36.000000 flaskz-1.7.3rc1/src/flaskz/utils/_common.py
+-rw-r--r--   0 taozh      (501) staff       (20)      860 2023-12-30 16:48:17.000000 flaskz-1.7.3rc1/src/flaskz/utils/_func.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     2785 2023-04-26 10:28:36.000000 flaskz-1.7.3rc1/src/flaskz/utils/_magic.py
+-rw-r--r--   0 taozh      (501) staff       (20)     1020 2023-12-30 16:50:25.000000 flaskz-1.7.3rc1/src/flaskz/utils/_private.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     7933 2024-01-30 02:20:56.000000 flaskz-1.7.3rc1/src/flaskz/utils/_request_api.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     1201 2023-12-30 16:50:25.000000 flaskz-1.7.3rc1/src/flaskz/utils/_request_args.py
+-rwxrwxrwx   0 taozh      (501) staff       (20)     3045 2024-01-30 02:31:20.000000 flaskz-1.7.3rc1/src/flaskz/utils/_response.py
+-rw-r--r--   0 taozh      (501) staff       (20)     4322 2023-12-30 13:56:42.000000 flaskz-1.7.3rc1/src/flaskz/utils/_timer.py
+drwxr-xr-x   0 taozh      (501) staff       (20)        0 2024-04-16 02:00:09.548505 flaskz-1.7.3rc1/src/flaskz.egg-info/
+-rw-r--r--   0 taozh      (501) staff       (20)     9710 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/PKG-INFO
+-rwxrwxrwx   0 taozh      (501) staff       (20)      981 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        1 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)       87 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/requires.txt
+-rwxrwxrwx   0 taozh      (501) staff       (20)        7 2024-04-16 02:00:09.000000 flaskz-1.7.3rc1/src/flaskz.egg-info/top_level.txt
```

### Comparing `flaskz-1.7.3/LICENSE` & `flaskz-1.7.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/PKG-INFO` & `flaskz-1.7.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.7.3
+Version: 1.7.3rc1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,33 +17,34 @@
 Requires-Dist: requests>=2
 Provides-Extra: ext
 Requires-Dist: pycryptodome>=3.15.0; extra == "ext"
 Requires-Dist: paramiko>=3.0.0; extra == "ext"
 
 ## 关于
 
-*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展工具集, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
+*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
 
 ## 使用
 
 1. [☞数据库初始化&常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_model_init.html)
 2. [☞数据模型扩展类](http://zhangyiheng.com/blog/articles/py_flaskz_model_mixin.html)
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.7.3** `2024/05/01`
+- **1.7.3rc1** `2024/04/16`
     - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
     - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
-    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认复用)
+    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认启用)
     - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
     - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
+
 - **1.7.2** `2024/02/01`
     - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
     - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
 - **1.7.1** `2024/01/05`
     - [F] 修复SQLAlchemy<2.0.0版本时, `flaskz.models._util.py`中`BinaryExpression`类的导入问题
 - **1.7.0** `2024/01/01`
     - [C] `SQLAlchemy`依赖的版本从`>=1.3.13(EOL)`升级到`>=1.4.0(Maintenance)`
```

### Comparing `flaskz-1.7.3/README.md` & `flaskz-1.7.3rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 ## 关于
 
-*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展工具集, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
+*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
 
 ## 使用
 
 1. [☞数据库初始化&常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_model_init.html)
 2. [☞数据模型扩展类](http://zhangyiheng.com/blog/articles/py_flaskz_model_mixin.html)
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.7.3** `2024/05/01`
+- **1.7.3rc1** `2024/04/16`
     - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
     - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
-    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认复用)
+    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认启用)
     - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
     - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
+
 - **1.7.2** `2024/02/01`
     - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
     - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
 - **1.7.1** `2024/01/05`
     - [F] 修复SQLAlchemy<2.0.0版本时, `flaskz.models._util.py`中`BinaryExpression`类的导入问题
 - **1.7.0** `2024/01/01`
     - [C] `SQLAlchemy`依赖的版本从`>=1.3.13(EOL)`升级到`>=1.4.0(Maintenance)`
```

### Comparing `flaskz-1.7.3/setup.cfg` & `flaskz-1.7.3rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flaskz
-version = 1.7.3
+version = 1.7.3rc1
 author = Zhang Tao
 author_email = taozh1982@gmail.com
 description = Flask and SQLAlchemy extensions for web applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/taozh1982/flaskz
 project_urls =
```

### Comparing `flaskz-1.7.3/src/flaskz/auth/_jws.py` & `flaskz-1.7.3rc1/src/flaskz/auth/_jws.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/ext/cypher.py` & `flaskz-1.7.3rc1/src/flaskz/ext/cypher.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/ext/ssh.py` & `flaskz-1.7.3rc1/src/flaskz/ext/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,19 +226,18 @@
          :param recv: wait for the result or not.
          :param clean: clean output info or not, default True(clean)
          :param prompt: the prompt of the command line
 
          :return: the output of the command
         """
 
-        if self._pre_commands_run is False and self._pre_commands:
-            self._run_command('', False)
-            pre_command_len = len(self._pre_commands)
-            for index, pre_command in enumerate(self._pre_commands):
-                self._run_command(pre_command, index == pre_command_len - 1)
+        if self._pre_commands and self._pre_commands_run is False:
+            # self._run_command('', False)
+            for pre_command in self._pre_commands:
+                self._run_command(pre_command, False)
             self._pre_commands_run = True
 
         if prompt is None:  # prompt is False for config
             prompt = self.get_prompt()  # 1.get prompt 2.remove welcome
 
         command, recv, clean = _get_command_arg(command, recv, clean)
         output = self._run_command(command, recv, prompt)
@@ -447,15 +446,15 @@
                 continue
             else:
                 recv_start = None
                 if count == 0:  # Solve the problem of incomplete data
                     time.sleep(recv_start_delay)
             count += 1
             data = self.channel.recv(recv_max_bytes)
-            info = data.decode('utf-8', 'backslashreplace')  # @2024-04-18 data.decode() --> current
+            info = data.decode()
             res = info.replace(' \r', '')
             res_list.append(res)
             if len(info) < recv_max_bytes:  # read speed > write speed
                 if (prompt is not None and info.endswith(prompt)) or info.endswith(self.recv_endswith):
                     time.sleep(0.02)  # Make sure recv is finished, info.endswith(self.recv_endswith) Not 100% sure
                     if not self.channel.recv_ready():
                         break
```

### Comparing `flaskz-1.7.3/src/flaskz/log/__init__.py` & `flaskz-1.7.3rc1/src/flaskz/log/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/models/__init__.py` & `flaskz-1.7.3rc1/src/flaskz/models/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/models/_base.py` & `flaskz-1.7.3rc1/src/flaskz/models/_base.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/models/_model.py` & `flaskz-1.7.3rc1/src/flaskz/models/_model.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/models/_query_util.py` & `flaskz-1.7.3rc1/src/flaskz/models/_query_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/models/_util.py` & `flaskz-1.7.3rc1/src/flaskz/models/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/res_status_codes.py` & `flaskz-1.7.3rc1/src/flaskz/res_status_codes.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/rest/__init__.py` & `flaskz-1.7.3rc1/src/flaskz/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/rest/_mgmt.py` & `flaskz-1.7.3rc1/src/flaskz/rest/_mgmt.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/rest/_util.py` & `flaskz-1.7.3rc1/src/flaskz/rest/_util.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/utils/_app.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_app.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/utils/_cache.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_cache.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/utils/_cls.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_cls.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/utils/_common.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_common.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/utils/_func.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_func.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/utils/_magic.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_magic.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/utils/_private.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_private.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/utils/_request_api.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_request_api.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/utils/_request_args.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_request_args.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/utils/_response.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_response.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz/utils/_timer.py` & `flaskz-1.7.3rc1/src/flaskz/utils/_timer.py`

 * *Files identical despite different names*

### Comparing `flaskz-1.7.3/src/flaskz.egg-info/PKG-INFO` & `flaskz-1.7.3rc1/src/flaskz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskz
-Version: 1.7.3
+Version: 1.7.3rc1
 Summary: Flask and SQLAlchemy extensions for web applications
 Home-page: https://github.com/taozh1982/flaskz
 Author: Zhang Tao
 Author-email: taozh1982@gmail.com
 Project-URL: Bug Tracker, https://github.com/taozh1982/flaskz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,33 +17,34 @@
 Requires-Dist: requests>=2
 Provides-Extra: ext
 Requires-Dist: pycryptodome>=3.15.0; extra == "ext"
 Requires-Dist: paramiko>=3.0.0; extra == "ext"
 
 ## 关于
 
-*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展工具集, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
+*Flaskz*是*Flask*和*SQLAlchemy ORM*的扩展, 主要用于web应用的开发, 可以快速灵活的实现各种业务场景并提供API。
 
 ## 使用
 
 1. [☞数据库初始化&常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_model_init.html)
 2. [☞数据模型扩展类](http://zhangyiheng.com/blog/articles/py_flaskz_model_mixin.html)
 3. [☞API封装、访问权限控制和系统日志](http://zhangyiheng.com/blog/articles/py_flaskz_api.html)
 4. [☞常用函数](http://zhangyiheng.com/blog/articles/py_flaskz_utils.html)
 5. [☞基于Flaskz的管理系统开发模板 Flaskz-admin](http://zhangyiheng.com/blog/articles/py_flaskz_admin.html)
 6. [☞使用手册](http://zhangyiheng.com/blog/articles/py_flaskz_manual.html)
 
 ## 版本
 
-- **1.7.3** `2024/05/01`
+- **1.7.3rc1** `2024/04/16`
     - [C] `flaskz.utils.ins_to_dict`函数返回的dict中包含值为`None`的键值
     - [A] `BaseModelMixin.to_dict`方法的`option`参数添加`relationships`选项，用于自定义是否查询关联关系
-    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认复用)
+    - [A] `FLASKZ_DATABASE_SESSION_KWARGS`配置参数添加`reusable_in_flask_g`选项, 用于设置是否在`flask.g`中缓存&复用`session`对象(默认启用)
     - [C] `flaskz.ext.ssh`返回值保留文本两侧的空格
     - [A] `flaskz.ext.ssh.SSH`添加`pre_commands`参数, 用于在命令执行之前预先执行控制相关命令
+
 - **1.7.2** `2024/02/01`
     - [A] `flaskz.models.parse_pss`函数支持`like_columns`参数, 用于定义模糊查询列(默认使用模型类的like_columns)
     - [A] `flaskz.utils.api_request`函数添加`http_kwargs`参数，用于设置http请求参数
 - **1.7.1** `2024/01/05`
     - [F] 修复SQLAlchemy<2.0.0版本时, `flaskz.models._util.py`中`BinaryExpression`类的导入问题
 - **1.7.0** `2024/01/01`
     - [C] `SQLAlchemy`依赖的版本从`>=1.3.13(EOL)`升级到`>=1.4.0(Maintenance)`
```

### Comparing `flaskz-1.7.3/src/flaskz.egg-info/SOURCES.txt` & `flaskz-1.7.3rc1/src/flaskz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

