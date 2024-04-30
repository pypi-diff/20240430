# Comparing `tmp/tailucas_pylib-0.3.2.tar.gz` & `tmp/tailucas_pylib-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailucas_pylib-0.3.2.tar", max compression
+gzip compressed data, was "tailucas_pylib-0.3.3.tar", max compression
```

## Comparing `tailucas_pylib-0.3.2.tar` & `tailucas_pylib-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.3.2/LICENSE
--rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.3.2/README.md
--rw-r--r--   0        0        0      537 2024-04-28 11:52:28.561594 tailucas_pylib-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5982 2024-04-28 11:52:17.451594 tailucas_pylib-0.3.2/tailucas_pylib/__init__.py
--rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.3.2/tailucas_pylib/app.py
--rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.3.2/tailucas_pylib/aws/__init__.py
--rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.3.2/tailucas_pylib/aws/metrics.py
--rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.3.2/tailucas_pylib/aws/swf.py
--rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.2/tailucas_pylib/bluetooth.py
--rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.3.2/tailucas_pylib/data.py
--rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.2/tailucas_pylib/datetime.py
--rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.3.2/tailucas_pylib/handler.py
--rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.2/tailucas_pylib/process.py
--rw-r--r--   0        0        0     9521 2023-09-03 07:12:39.509088 tailucas_pylib-0.3.2/tailucas_pylib/rabbit.py
--rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.3.2/tailucas_pylib/threads.py
--rw-r--r--   0        0        0     3387 2024-04-21 11:13:24.751872 tailucas_pylib-0.3.2/tailucas_pylib/zmq.py
--rw-r--r--   0        0        0    12289 1970-01-01 00:00:00.000000 tailucas_pylib-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-31 19:44:41.375775 tailucas_pylib-0.3.3/LICENSE
+-rw-r--r--   0        0        0    11403 2023-11-25 09:06:51.036540 tailucas_pylib-0.3.3/README.md
+-rw-r--r--   0        0        0      537 2024-04-29 20:24:46.456999 tailucas_pylib-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5982 2024-04-29 15:31:10.287006 tailucas_pylib-0.3.3/tailucas_pylib/__init__.py
+-rw-r--r--   0        0        0     2148 2023-09-10 09:39:25.219973 tailucas_pylib-0.3.3/tailucas_pylib/app.py
+-rw-r--r--   0        0        0     1218 2023-09-10 09:33:16.369962 tailucas_pylib-0.3.3/tailucas_pylib/aws/__init__.py
+-rw-r--r--   0        0        0     1455 2023-09-10 09:49:11.549965 tailucas_pylib-0.3.3/tailucas_pylib/aws/metrics.py
+-rw-r--r--   0        0        0     8727 2024-02-25 13:23:22.241361 tailucas_pylib-0.3.3/tailucas_pylib/aws/swf.py
+-rw-r--r--   0        0        0     2427 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.3/tailucas_pylib/bluetooth.py
+-rw-r--r--   0        0        0      725 2023-12-29 14:58:54.907113 tailucas_pylib-0.3.3/tailucas_pylib/data.py
+-rw-r--r--   0        0        0     3147 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.3/tailucas_pylib/datetime.py
+-rw-r--r--   0        0        0     3112 2023-09-10 09:47:03.819967 tailucas_pylib-0.3.3/tailucas_pylib/handler.py
+-rw-r--r--   0        0        0     1009 2023-08-31 19:44:41.385775 tailucas_pylib-0.3.3/tailucas_pylib/process.py
+-rw-r--r--   0        0        0     9796 2024-04-29 20:28:04.457000 tailucas_pylib-0.3.3/tailucas_pylib/rabbit.py
+-rw-r--r--   0        0        0     5398 2024-04-28 08:25:39.491596 tailucas_pylib-0.3.3/tailucas_pylib/threads.py
+-rw-r--r--   0        0        0     3387 2024-04-21 11:13:24.751872 tailucas_pylib-0.3.3/tailucas_pylib/zmq.py
+-rw-r--r--   0        0        0    12289 1970-01-01 00:00:00.000000 tailucas_pylib-0.3.3/PKG-INFO
```

### Comparing `tailucas_pylib-0.3.2/LICENSE` & `tailucas_pylib-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/README.md` & `tailucas_pylib-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/pyproject.toml` & `tailucas_pylib-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tailucas-pylib"
-version = "0.3.2"
+version = "0.3.3"
 description = "Common Python utility modules"
 authors = ["Tai Lucas <tglucas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/__init__.py` & `tailucas_pylib-0.3.3/tailucas_pylib/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/app.py` & `tailucas_pylib-0.3.3/tailucas_pylib/app.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/aws/__init__.py` & `tailucas_pylib-0.3.3/tailucas_pylib/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/aws/metrics.py` & `tailucas_pylib-0.3.3/tailucas_pylib/aws/metrics.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/aws/swf.py` & `tailucas_pylib-0.3.3/tailucas_pylib/aws/swf.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/bluetooth.py` & `tailucas_pylib-0.3.3/tailucas_pylib/bluetooth.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/data.py` & `tailucas_pylib-0.3.3/tailucas_pylib/data.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/datetime.py` & `tailucas_pylib-0.3.3/tailucas_pylib/datetime.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/handler.py` & `tailucas_pylib-0.3.3/tailucas_pylib/handler.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/process.py` & `tailucas_pylib-0.3.3/tailucas_pylib/process.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/rabbit.py` & `tailucas_pylib-0.3.3/tailucas_pylib/rabbit.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ignore_logger('pika.connection')
 
 
 log = logging.getLogger(APP_NAME)  # type: ignore
 
 
 BLOCKED_CONNECTION_TIMEOUT = 5
-PUBLISH_RETRIES = 2
+PUBLISH_RETRIES = 3
 
 
 class MQConnection(AppThread):
     def __init__(self, mq_server_address, mq_exchange_name, mq_topic_filter='#', mq_exchange_type='topic', mq_arguments=None):
         AppThread.__init__(self, name=self.__class__.__name__)
 
         if isinstance(mq_server_address, str):
@@ -78,56 +78,60 @@
                 success = True
                 # exit loop
                 break
             except StreamLostError as e:
                 # try again
                 if tries < PUBLISH_RETRIES:
                     log.warning(f'Retrying on lost stream during publish: {e!s}')
-                    continue
                 else:
                     raise RuntimeWarning('Publish failure after retry.') from e
             except ConnectionClosedByBroker as e:
                 raise ResourceWarning() from e
             finally:
-                tries += 1
                 if close_channel or not success:
                     log.debug(f'Closing potentially stale channel (successful attempt? {success})...')
                     self._close_channel()
-                    if close_connection or not success:
-                        log.debug(f'Closing potentially stale connection (successful attempt? {success})...')
-                        self._close_connection()
+                    if tries > 1:
+                        if close_connection or not success:
+                            log.debug(f'Closing potentially stale connection (successful attempt? {success})...')
+                            self._close_connection()
+                tries += 1
         if not success:
             raise AssertionError('No success after publish attempt.')
 
     def _setup_connection(self):
         if self._mq_connection is None or self._mq_connection.is_closed:
+            if self._mq_connection:
+                log.info(f'Recreating RabbitMQ connection...')
             self._mq_connection = pika.BlockingConnection(parameters=self._pika_parameters)
 
     def _setup_channel(self):
         self._setup_connection()
         if self._mq_channel is None or self._mq_channel.is_closed:
+            if self._mq_channel:
+                log.info(f'Recreating RabbitMQ channel...')
             self._mq_channel = self._mq_connection.channel()
             self._mq_channel.exchange_declare(exchange=self._mq_exchange_name, exchange_type=self._mq_exchange_type, arguments=self._mq_arguments)
             mq_result = self._mq_channel.queue_declare('', exclusive=True)
             self._mq_queue_name = mq_result.method.queue
             log.info(f'Using RabbitMQ server(s) {self._mq_server_list} using {self._mq_exchange_type} exchange {self._mq_exchange_name} and queue {self._mq_queue_name}.')
 
     def _close_connection(self):
-        if self._mq_connection:
-            log.info(f'Closing RabbitMQ connection for {self.name}...')
+        if self._mq_connection and self._mq_connection.is_open:
+            log.info(f'Closing RabbitMQ connection...')
             try:
                 self._mq_connection.close()
             except Exception:
                 log.debug(self.__class__.__name__, exc_info=True)
 
     def _close_channel(self):
-        if self._mq_channel:
-            log.info(f'Stopping RabbitMQ channel for {self.name}...')
+        if self._mq_channel and self._mq_channel.is_open:
+            log.info(f'Closing RabbitMQ channel...')
             try:
-                self._mq_channel.stop_consuming()
+                self._mq_channel.close()
             except Exception:
                 log.debug(self.__class__.__name__, exc_info=True)
 
     def stop(self):
         self._close_channel()
         self._close_connection()
 
@@ -138,14 +142,15 @@
         MQConnection.__init__(
             self,
             mq_server_address=mq_server_address,
             mq_exchange_name=mq_exchange_name,
             mq_topic_filter=mq_topic_filter,
             mq_exchange_type=mq_exchange_type)
         self._zmq_url = zmq_url
+        self.name = f'{self.__class__.__name__} ({zmq_url})'
 
     def _setup_channel(self):
         MQConnection._setup_channel(self)
         self._mq_channel.queue_bind(
             exchange=self._mq_exchange_name,
             queue=self._mq_queue_name,
             routing_key=self._mq_topic_filter)
@@ -156,21 +161,21 @@
 
     # noinspection PyBroadException
     def run(self):
         with exception_handler(connect_url=self._zmq_url, and_raise=False, shutdown_on_error=True) as zmq_socket:
             self.processor = zmq_socket
             try:
                 self._setup_channel()
-                log.info(f'Ready for RabbitMQ messages in {self.name}.')
+                log.info(f'Ready for RabbitMQ messages.')
                 self._mq_channel.start_consuming()
             except (AMQPConnectionError, ConnectionClosedByBroker, StreamLostError) as e:
                 # handled error due to already shutting down
                 raise ResourceWarning('Consumer interrupted.') from e
             finally:
-                log.info(f'RabbitMQ listener for {self.name} has finished.')
+                log.info(f'RabbitMQ listener has finished.')
 
     def callback(self, ch, method, properties, body):
         topic = method.routing_key
         log.debug(f'[{topic}]: {body}')
         topic_parts = topic.split('.')
         if len(topic_parts) < 3:
             log.warning(f'Ignoring non-routable message from topic [{topic}] due to unsufficient topic parts.')
@@ -190,15 +195,15 @@
             if not threads.shutting_down:
                 raise e
 
 
 class RabbitMQRelay(AppThread):
 
     def __init__(self, zmq_url, mq_server_address, mq_exchange_name, mq_topic_filter, mq_exchange_type):
-        AppThread.__init__(self, name=self.__class__.__name__)
+        AppThread.__init__(self, name=f'{self.__class__.__name__} ({zmq_url})')
         self._source_zmq_url = zmq_url
         self._source_socket_type = zmq.PULL
 
         self._mq_config_server = mq_server_address
         self._mq_connection = pika.BlockingConnection(
             pika.ConnectionParameters(
                 host=self._mq_config_server,
```

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/threads.py` & `tailucas_pylib-0.3.3/tailucas_pylib/threads.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/tailucas_pylib/zmq.py` & `tailucas_pylib-0.3.3/tailucas_pylib/zmq.py`

 * *Files identical despite different names*

### Comparing `tailucas_pylib-0.3.2/PKG-INFO` & `tailucas_pylib-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailucas-pylib
-Version: 0.3.2
+Version: 0.3.3
 Summary: Common Python utility modules
 License: MIT
 Author: Tai Lucas
 Author-email: tglucas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

