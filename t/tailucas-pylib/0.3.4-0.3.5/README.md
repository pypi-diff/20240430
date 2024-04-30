# Comparing `tmp/tailucas_pylib-0.3.4.tar.gz` & `tmp/tailucas_pylib-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailucas_pylib-0.3.4.tar", max compression
+gzip compressed data, was "tailucas_pylib-0.3.5.tar", max compression
```

## Comparing `tailucas_pylib-0.3.4.tar` & `tailucas_pylib-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.3.4/LICENSE
--rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.3.4/README.md
--rw-r--r--   0        0        0      537 2024-04-30 05:19:18.522011 tailucas_pylib-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     5982 2024-04-29 15:31:10.287006 tailucas_pylib-0.3.4/tailucas_pylib/__init__.py
--rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.3.4/tailucas_pylib/app.py
--rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.3.4/tailucas_pylib/aws/__init__.py
--rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.3.4/tailucas_pylib/aws/metrics.py
--rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.3.4/tailucas_pylib/aws/swf.py
--rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.4/tailucas_pylib/bluetooth.py
--rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.3.4/tailucas_pylib/data.py
--rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.4/tailucas_pylib/datetime.py
--rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.3.4/tailucas_pylib/handler.py
--rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.4/tailucas_pylib/process.py
--rw-r--r--   0        0        0     9802 2024-04-30 05:19:04.362011 tailucas_pylib-0.3.4/tailucas_pylib/rabbit.py
--rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.3.4/tailucas_pylib/threads.py
--rw-r--r--   0        0        0     3387 2024-04-30 05:12:18.922012 tailucas_pylib-0.3.4/tailucas_pylib/zmq.py
--rw-r--r--   0        0        0    12289 1970-01-01 00:00:00.000000 tailucas_pylib-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.3.5/LICENSE
+-rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.3.5/README.md
+-rw-r--r--   0        0        0      537 2024-04-30 05:24:47.912012 tailucas_pylib-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     5982 2024-04-29 15:31:10.287006 tailucas_pylib-0.3.5/tailucas_pylib/__init__.py
+-rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.3.5/tailucas_pylib/app.py
+-rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.3.5/tailucas_pylib/aws/__init__.py
+-rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.3.5/tailucas_pylib/aws/metrics.py
+-rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.3.5/tailucas_pylib/aws/swf.py
+-rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.5/tailucas_pylib/bluetooth.py
+-rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.3.5/tailucas_pylib/data.py
+-rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.5/tailucas_pylib/datetime.py
+-rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.3.5/tailucas_pylib/handler.py
+-rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.5/tailucas_pylib/process.py
+-rw-r--r--   0        0        0     9781 2024-04-30 05:24:41.782012 tailucas_pylib-0.3.5/tailucas_pylib/rabbit.py
+-rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.3.5/tailucas_pylib/threads.py
+-rw-r--r--   0        0        0     3387 2024-04-30 05:12:18.922012 tailucas_pylib-0.3.5/tailucas_pylib/zmq.py
+-rw-r--r--   0        0        0    12289 1970-01-01 00:00:00.000000 tailucas_pylib-0.3.5/PKG-INFO
```

### Comparing `tailucas_pylib-0.3.4/LICENSE` & `tailucas_pylib-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/README.md` & `tailucas_pylib-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/pyproject.toml` & `tailucas_pylib-0.3.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tailucas-pylib"
-version = "0.3.4"
+version = "0.3.5"
 description = "Common Python utility modules"
 authors = ["Tai Lucas <tglucas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/__init__.py` & `tailucas_pylib-0.3.5/tailucas_pylib/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/app.py` & `tailucas_pylib-0.3.5/tailucas_pylib/app.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/aws/__init__.py` & `tailucas_pylib-0.3.5/tailucas_pylib/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/aws/metrics.py` & `tailucas_pylib-0.3.5/tailucas_pylib/aws/metrics.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/aws/swf.py` & `tailucas_pylib-0.3.5/tailucas_pylib/aws/swf.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/bluetooth.py` & `tailucas_pylib-0.3.5/tailucas_pylib/bluetooth.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/data.py` & `tailucas_pylib-0.3.5/tailucas_pylib/data.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/datetime.py` & `tailucas_pylib-0.3.5/tailucas_pylib/datetime.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/handler.py` & `tailucas_pylib-0.3.5/tailucas_pylib/handler.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/process.py` & `tailucas_pylib-0.3.5/tailucas_pylib/process.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/rabbit.py` & `tailucas_pylib-0.3.5/tailucas_pylib/rabbit.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 
 
 BLOCKED_CONNECTION_TIMEOUT = 5
 PUBLISH_RETRIES = 3
 
 
 class MQConnection(AppThread):
-    def __init__(self, mq_server_address, mq_exchange_name, mq_topic_filter='#', mq_exchange_type='topic', mq_arguments=None):
-        AppThread.__init__(self, name=self.__class__.__name__)
+    def __init__(self, name, mq_server_address, mq_exchange_name, mq_topic_filter='#', mq_exchange_type='topic', mq_arguments=None):
+        AppThread.__init__(self, name=name)
 
         if isinstance(mq_server_address, str):
             self._mq_server_list = [mq_server_address]
         elif isinstance(mq_server_address, list):
             self._mq_server_list = mq_server_address
         else:
             raise AssertionError(f'Unsupported argument type: {mq_server_address}')
@@ -137,14 +137,15 @@
 
 
 class ZMQListener(MQConnection):
 
     def __init__(self, zmq_url, mq_server_address, mq_exchange_name, mq_topic_filter, mq_exchange_type):
         MQConnection.__init__(
             self,
+            name=f'{self.__class__.__name__} ({zmq_url})',
             mq_server_address=mq_server_address,
             mq_exchange_name=mq_exchange_name,
             mq_topic_filter=mq_topic_filter,
             mq_exchange_type=mq_exchange_type)
         self._zmq_url = zmq_url
 
     def _setup_channel(self):
@@ -156,15 +157,14 @@
         self._mq_channel.basic_consume(
             queue=self._mq_queue_name,
             on_message_callback=self.callback,
             auto_ack=True)
 
     # noinspection PyBroadException
     def run(self):
-        self.name = f'{self.__class__.__name__} ({self._zmq_url})'
         with exception_handler(connect_url=self._zmq_url, and_raise=False, shutdown_on_error=True) as zmq_socket:
             self.processor = zmq_socket
             try:
                 self._setup_channel()
                 log.info(f'Ready for RabbitMQ messages.')
                 self._mq_channel.start_consuming()
             except (AMQPConnectionError, ConnectionClosedByBroker, StreamLostError) as e:
```

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/threads.py` & `tailucas_pylib-0.3.5/tailucas_pylib/threads.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/tailucas_pylib/zmq.py` & `tailucas_pylib-0.3.5/tailucas_pylib/zmq.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.4/PKG-INFO` & `tailucas_pylib-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailucas-pylib
-Version: 0.3.4
+Version: 0.3.5
 Summary: Common Python utility modules
 License: MIT
 Author: Tai Lucas
 Author-email: tglucas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

