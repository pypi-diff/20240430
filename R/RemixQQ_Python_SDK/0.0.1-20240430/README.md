# Comparing `tmp/remixqq_python_sdk-0.0.1.tar.gz` & `tmp/remixqq_python_sdk-20240430.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remixqq_python_sdk-0.0.1.tar", last modified: Sun Apr 28 03:00:23 2024, max compression
+gzip compressed data, was "remixqq_python_sdk-20240430.tar", last modified: Tue Apr 30 16:21:02 2024, max compression
```

## Comparing `remixqq_python_sdk-0.0.1.tar` & `remixqq_python_sdk-20240430.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 03:00:23.333227 remixqq_python_sdk-0.0.1/
--rw-rw-rw-   0        0        0     1090 2024-04-23 08:40:39.000000 remixqq_python_sdk-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2091 2024-04-28 03:00:23.333227 remixqq_python_sdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1624 2024-04-09 00:50:29.000000 remixqq_python_sdk-0.0.1/README.md
--rw-rw-rw-   0        0        0      731 2024-04-28 02:21:41.000000 remixqq_python_sdk-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 03:00:23.333227 remixqq_python_sdk-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-28 03:00:23.275653 remixqq_python_sdk-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-28 03:00:23.332220 remixqq_python_sdk-0.0.1/src/RemixQQ_Python_SDK.egg-info/
--rw-rw-rw-   0        0        0     2091 2024-04-28 03:00:23.000000 remixqq_python_sdk-0.0.1/src/RemixQQ_Python_SDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2024-04-28 03:00:23.000000 remixqq_python_sdk-0.0.1/src/RemixQQ_Python_SDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 03:00:23.000000 remixqq_python_sdk-0.0.1/src/RemixQQ_Python_SDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-28 03:00:23.000000 remixqq_python_sdk-0.0.1/src/RemixQQ_Python_SDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-28 03:00:23.000000 remixqq_python_sdk-0.0.1/src/RemixQQ_Python_SDK.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-28 03:00:23.331220 remixqq_python_sdk-0.0.1/src/remixqq_python_sdk/
--rw-rw-rw-   0        0        0        0 2024-04-09 00:50:29.000000 remixqq_python_sdk-0.0.1/src/remixqq_python_sdk/__init__.py
--rw-rw-rw-   0        0        0     9447 2024-04-23 09:02:19.000000 remixqq_python_sdk-0.0.1/src/remixqq_python_sdk/app.py
-drwxrwxrwx   0        0        0        0 2024-04-28 03:00:23.332220 remixqq_python_sdk-0.0.1/test/
--rw-rw-rw-   0        0        0      141 2024-04-28 02:26:07.000000 remixqq_python_sdk-0.0.1/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:21:02.619431 remixqq_python_sdk-20240430/
+-rw-rw-rw-   0        0        0     1090 2024-04-10 11:58:02.000000 remixqq_python_sdk-20240430/LICENSE
+-rw-rw-rw-   0        0        0     2362 2024-04-30 16:21:02.618432 remixqq_python_sdk-20240430/PKG-INFO
+-rw-rw-rw-   0        0        0     1892 2024-04-30 15:37:51.000000 remixqq_python_sdk-20240430/README.md
+-rw-rw-rw-   0        0        0      736 2024-04-30 16:20:57.000000 remixqq_python_sdk-20240430/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:21:02.619431 remixqq_python_sdk-20240430/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 16:21:02.613431 remixqq_python_sdk-20240430/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 16:21:02.618432 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/
+-rw-rw-rw-   0        0        0     2362 2024-04-30 16:21:02.000000 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2024-04-30 16:21:02.000000 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:21:02.000000 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-30 16:21:02.000000 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-30 16:21:02.000000 remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 16:21:02.617431 remixqq_python_sdk-20240430/src/remixqq_python_sdk/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:16:24.000000 remixqq_python_sdk-20240430/src/remixqq_python_sdk/__init__.py
+-rw-rw-rw-   0        0        0    12210 2024-04-30 14:48:27.000000 remixqq_python_sdk-20240430/src/remixqq_python_sdk/app.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:21:02.617431 remixqq_python_sdk-20240430/tests/
+-rw-rw-rw-   0        0        0      162 2024-04-10 13:30:43.000000 remixqq_python_sdk-20240430/tests/test.py
```

### Comparing `remixqq_python_sdk-0.0.1/LICENSE` & `remixqq_python_sdk-20240430/LICENSE`

 * *Files identical despite different names*

### Comparing `remixqq_python_sdk-0.0.1/PKG-INFO` & `remixqq_python_sdk-20240430/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RemixQQ_Python_SDK
-Version: 0.0.1
+Version: 20240430
 Summary: A python SDK for RemixQQ connected by httpapi
 Author-email: 404_NOT_FOUND <1127738407@qq.com>
 License: MIT
 Project-URL: Homepage, https://github.com/willyautoman/RemixQQ_Python_SDK
 Project-URL: Bug Tracker, https://github.com/willyautoman/RemixQQ_Python_SDK/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -23,39 +23,48 @@
 
 1. MyQQ_Httpapi的配置方法
    1. 在主界面配置端口号及Token（用于发送消息）
    ![](https://image-bed.ityun.tech/1.png)
    2. 在“回调”界面配置接收消息用的地址（重要！！！）
    ![](https://image-bed.ityun.tech/2.png)
 
-2. 使用pip安装（开发中，暂无法安装）
+2. 使用pip安装
 ```shell
 pip install RemixQQ_Python_SDK
 ```
 
 1. 使用以下代码进行初始化
 ```python
 from http.server import HTTPServer, BaseHTTPRequestHandler
+from remixqq_python_sdk.app import App
 import json
 import urllib.parse
 import random
 import requests
 host = ('localhost', 8082) #接收消息地址（需与上方配置界面一致）
-url = 'http://localhost:8081/MyQQHTTPAPI'  #发送消息地址
+app = App('http://localhost:8081/MyQQHTTPAPI', "Token", "QQ")
 class Resquest(BaseHTTPRequestHandler):
     def do_POST(self):
         datas = self.rfile.read(int(self.headers['content-length'])).decode()
         datas = json.loads(datas)
         from_qun = urllib.parse.unquote(datas['MQ_fromID']) #获取消息来源群号
         msg = urllib.parse.unquote(datas['MQ_msg']) #获取消息内容
         # do something
-        print(datas)
+        response = app.send_group_message("123",0,0,"test")
+        print(response)
 
 if __name__ == '__main__':
     server = HTTPServer(host, Resquest)
     print("Starting server, listen at: %s:%s" % host)
     server.serve_forever()
 ```
-TODO:
-1.将API完整复刻至Python
-2.实现一个包即可完成消息收发
-
+## TODO:
+1. 将API完整复刻至Python
+2. 实现一个包即可完成消息收发
+3. 建立API文档
+
+## Release Note
+### 0.0.1（发布日期：2024年4月26日）
+1. 已完成基础功能
+2. 发布包至PYPI，可使用pip安装
+3. 新增代办：建立API文档
+4.
```

### Comparing `remixqq_python_sdk-0.0.1/README.md` & `remixqq_python_sdk-20240430/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -10,39 +10,48 @@
 
 1. MyQQ_Httpapi的配置方法
    1. 在主界面配置端口号及Token（用于发送消息）
    ![](https://image-bed.ityun.tech/1.png)
    2. 在“回调”界面配置接收消息用的地址（重要！！！）
    ![](https://image-bed.ityun.tech/2.png)
 
-2. 使用pip安装（开发中，暂无法安装）
+2. 使用pip安装
 ```shell
 pip install RemixQQ_Python_SDK
 ```
 
 1. 使用以下代码进行初始化
 ```python
 from http.server import HTTPServer, BaseHTTPRequestHandler
+from remixqq_python_sdk.app import App
 import json
 import urllib.parse
 import random
 import requests
 host = ('localhost', 8082) #接收消息地址（需与上方配置界面一致）
-url = 'http://localhost:8081/MyQQHTTPAPI'  #发送消息地址
+app = App('http://localhost:8081/MyQQHTTPAPI', "Token", "QQ")
 class Resquest(BaseHTTPRequestHandler):
     def do_POST(self):
         datas = self.rfile.read(int(self.headers['content-length'])).decode()
         datas = json.loads(datas)
         from_qun = urllib.parse.unquote(datas['MQ_fromID']) #获取消息来源群号
         msg = urllib.parse.unquote(datas['MQ_msg']) #获取消息内容
         # do something
-        print(datas)
+        response = app.send_group_message("123",0,0,"test")
+        print(response)
 
 if __name__ == '__main__':
     server = HTTPServer(host, Resquest)
     print("Starting server, listen at: %s:%s" % host)
     server.serve_forever()
 ```
-TODO:
-1.将API完整复刻至Python
-2.实现一个包即可完成消息收发
+## TODO:
+1. 将API完整复刻至Python
+2. 实现一个包即可完成消息收发
+3. 建立API文档
 
+## Release Note
+### 0.0.1（发布日期：2024年4月26日）
+1. 已完成基础功能
+2. 发布包至PYPI，可使用pip安装
+3. 新增代办：建立API文档
+4.
```

### Comparing `remixqq_python_sdk-0.0.1/pyproject.toml` & `remixqq_python_sdk-20240430/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [project]
 name = "RemixQQ_Python_SDK"
-version = "0.0.1"
+version = "20240430"
 description = "A python SDK for RemixQQ connected by httpapi"
 authors = [
     {name = "404_NOT_FOUND", email = "1127738407@qq.com"},
 ]
 dependencies = [
     "requests>=2.31.0",
 ]
+
 requires-python = ">=3.8"
 readme = "README.md"
 license = {text = "MIT"}
 
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `remixqq_python_sdk-0.0.1/src/RemixQQ_Python_SDK.egg-info/PKG-INFO` & `remixqq_python_sdk-20240430/src/RemixQQ_Python_SDK.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RemixQQ_Python_SDK
-Version: 0.0.1
+Version: 20240430
 Summary: A python SDK for RemixQQ connected by httpapi
 Author-email: 404_NOT_FOUND <1127738407@qq.com>
 License: MIT
 Project-URL: Homepage, https://github.com/willyautoman/RemixQQ_Python_SDK
 Project-URL: Bug Tracker, https://github.com/willyautoman/RemixQQ_Python_SDK/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -23,39 +23,48 @@
 
 1. MyQQ_Httpapi的配置方法
    1. 在主界面配置端口号及Token（用于发送消息）
    ![](https://image-bed.ityun.tech/1.png)
    2. 在“回调”界面配置接收消息用的地址（重要！！！）
    ![](https://image-bed.ityun.tech/2.png)
 
-2. 使用pip安装（开发中，暂无法安装）
+2. 使用pip安装
 ```shell
 pip install RemixQQ_Python_SDK
 ```
 
 1. 使用以下代码进行初始化
 ```python
 from http.server import HTTPServer, BaseHTTPRequestHandler
+from remixqq_python_sdk.app import App
 import json
 import urllib.parse
 import random
 import requests
 host = ('localhost', 8082) #接收消息地址（需与上方配置界面一致）
-url = 'http://localhost:8081/MyQQHTTPAPI'  #发送消息地址
+app = App('http://localhost:8081/MyQQHTTPAPI', "Token", "QQ")
 class Resquest(BaseHTTPRequestHandler):
     def do_POST(self):
         datas = self.rfile.read(int(self.headers['content-length'])).decode()
         datas = json.loads(datas)
         from_qun = urllib.parse.unquote(datas['MQ_fromID']) #获取消息来源群号
         msg = urllib.parse.unquote(datas['MQ_msg']) #获取消息内容
         # do something
-        print(datas)
+        response = app.send_group_message("123",0,0,"test")
+        print(response)
 
 if __name__ == '__main__':
     server = HTTPServer(host, Resquest)
     print("Starting server, listen at: %s:%s" % host)
     server.serve_forever()
 ```
-TODO:
-1.将API完整复刻至Python
-2.实现一个包即可完成消息收发
-
+## TODO:
+1. 将API完整复刻至Python
+2. 实现一个包即可完成消息收发
+3. 建立API文档
+
+## Release Note
+### 0.0.1（发布日期：2024年4月26日）
+1. 已完成基础功能
+2. 发布包至PYPI，可使用pip安装
+3. 新增代办：建立API文档
+4.
```

### Comparing `remixqq_python_sdk-0.0.1/src/remixqq_python_sdk/app.py` & `remixqq_python_sdk-20240430/src/remixqq_python_sdk/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -323,9 +323,111 @@
             "params": {
                 'c1': self.qq,
             }
         }
 
         return self.__send_request(params)
 
+    def get_blog_pskey(self) -> dict:
+        """
+        取得腾讯微博页面操作用参数P_skey
+        """
+        params = {
+            "function": "Api_GetBlogPsKey",
+            "token": self.token,
+            "params": {
+                'c1': self.qq,
+            }
+        }
+        return self.__send_request(params)
+
+    def get_zone_pskey(self) -> dict:
+        """
+        取得QQ空间页面操作用参数P_skey
+        """
+        params = {
+            "function": "Api_GetZonePsKey",
+            "token": self.token,
+            "params": {
+                'c1': self.qq,
+            }
+        }
+        return self.__send_request(params)
+
+    def get_group_pskey(self) -> dict:
+        """
+        取得QQ群页面操作用参数P_skey
+        """
+        params = {
+            "function": "Api_GetGroupPsKey",
+            "token": self.token,
+            "params": {
+                'c1': self.qq,
+            }
+        }
+        return self.__send_request(params)
+
+    def get_classroom_pskey(self) -> dict:
+        """
+        取得QQ教室页面操作用参数P_skey
+        """
+        params = {
+            "function": "Api_GetClassRoomPsKey",
+            "token": self.token,
+            "params": {
+                'c1': self.qq,
+            }
+        }
+        return self.__send_request(params)
 
+    def get_ten_pay_pskey(self) -> dict:
+        """
+        取得QQ钱包页面操作用参数P_skey
+        """
+        params = {
+            "function": "Api_GetTenPayPsKey",
+            "token": self.token,
+            "params": {
+                'c1': self.qq,
+            }
+        }
+        return self.__send_request(params)
+
+    def get_jubao_pskey(self) -> dict:
+        """
+        取得QQ举报页面操作用参数P_skey
+        """
+        params = {
+            "function": "Api_GetJuBaoPsKey",
+            "token": self.token,
+            "params": {
+                'c1': self.qq,
+            }
+        }
+
+        return self.__send_request(params)
 
+    def get_bkn(self) -> dict:
+        """
+        取得机器人网页操作用参数Bkn或G_tk
+        """
+        params = {
+            "function": "Api_GetBkn",
+            "token": self.token,
+            "params": {
+                'c1': self.qq,
+            }
+        }
+        return self.__send_request(params)
+
+    def get_bkn_32(self) -> dict:
+        """
+        取得机器人网页操作用参数长Bkn或长G_tk
+        """
+        params = {
+            "function": "Api_GetBkn32",
+            "token": self.token,
+            "params": {
+                'c1': self.qq,
+            }
+        }
+        return self.__send_request(params)
```

