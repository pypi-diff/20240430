# Comparing `tmp/machineroom-0.47.2.tar.gz` & `tmp/machineroom-0.47.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.47.2.tar", last modified: Fri Apr 26 17:11:31 2024, max compression
+gzip compressed data, was "machineroom-0.47.3.tar", last modified: Tue Apr 30 03:59:29 2024, max compression
```

## Comparing `machineroom-0.47.2.tar` & `machineroom-0.47.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 17:11:31.047301 machineroom-0.47.2/
--rw-r--r--   0 root         (0) staff       (20)     2370 2024-04-26 06:25:54.000000 machineroom-0.47.2/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.47.2/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-26 17:11:31.047101 machineroom-0.47.2/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3754 2024-04-26 03:38:34.000000 machineroom-0.47.2/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 17:11:31.033483 machineroom-0.47.2/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.47.2/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 17:11:31.040509 machineroom-0.47.2/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-26 17:11:30.000000 machineroom-0.47.2/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    10297 2024-04-26 07:21:15.000000 machineroom-0.47.2/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      286 2024-04-26 04:12:22.000000 machineroom-0.47.2/machineroom/errs.py
--rw-r--r--   0 root         (0) staff       (20)     3535 2024-04-26 17:11:01.000000 machineroom-0.47.2/machineroom/infra.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.47.2/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    14128 2024-04-26 07:27:26.000000 machineroom-0.47.2/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    29559 2024-04-26 07:16:26.000000 machineroom-0.47.2/machineroom/taskbase.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 17:11:31.045409 machineroom-0.47.2/machineroom/tunnels/
--rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.47.2/machineroom/tunnels/__init__.py
--rwxr-xr-x   0 root         (0) staff       (20)     8068 2024-04-26 03:02:40.000000 machineroom-0.47.2/machineroom/tunnels/conn.py
--rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.47.2/machineroom/tunnels/fork.py
--rw-r--r--   0 root         (0) staff       (20)    17471 2024-04-26 17:09:46.000000 machineroom-0.47.2/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     7702 2024-04-26 07:27:26.000000 machineroom-0.47.2/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-26 17:11:31.046383 machineroom-0.47.2/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-26 17:11:30.000000 machineroom-0.47.2/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      534 2024-04-26 17:11:30.000000 machineroom-0.47.2/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-26 17:11:30.000000 machineroom-0.47.2/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       28 2024-04-26 17:11:30.000000 machineroom-0.47.2/machineroom.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-26 17:11:30.000000 machineroom-0.47.2/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-26 17:11:31.047942 machineroom-0.47.2/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.47.2/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1534 2024-04-26 07:28:38.000000 machineroom-0.47.2/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-26 17:11:23.000000 machineroom-0.47.2/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-30 03:59:29.746780 machineroom-0.47.3/
+-rw-r--r--   0 root         (0) staff       (20)     2370 2024-04-26 06:25:54.000000 machineroom-0.47.3/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.47.3/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-30 03:59:29.746580 machineroom-0.47.3/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3754 2024-04-26 03:38:34.000000 machineroom-0.47.3/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-30 03:59:29.734803 machineroom-0.47.3/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.47.3/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-30 03:59:29.741349 machineroom-0.47.3/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-30 03:59:29.000000 machineroom-0.47.3/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    10297 2024-04-26 07:21:15.000000 machineroom-0.47.3/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      286 2024-04-26 04:12:22.000000 machineroom-0.47.3/machineroom/errs.py
+-rw-r--r--   0 root         (0) staff       (20)     3682 2024-04-30 03:59:14.000000 machineroom-0.47.3/machineroom/infra.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.47.3/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    14128 2024-04-26 07:27:26.000000 machineroom-0.47.3/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    30284 2024-04-30 03:53:47.000000 machineroom-0.47.3/machineroom/taskbase.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-30 03:59:29.745205 machineroom-0.47.3/machineroom/tunnels/
+-rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.47.3/machineroom/tunnels/__init__.py
+-rwxr-xr-x   0 root         (0) staff       (20)     8068 2024-04-26 03:02:40.000000 machineroom-0.47.3/machineroom/tunnels/conn.py
+-rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.47.3/machineroom/tunnels/fork.py
+-rw-r--r--   0 root         (0) staff       (20)    17469 2024-04-30 03:53:47.000000 machineroom-0.47.3/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     7702 2024-04-26 07:27:26.000000 machineroom-0.47.3/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-30 03:59:29.746007 machineroom-0.47.3/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4856 2024-04-30 03:59:29.000000 machineroom-0.47.3/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      534 2024-04-30 03:59:29.000000 machineroom-0.47.3/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-30 03:59:29.000000 machineroom-0.47.3/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       28 2024-04-30 03:59:29.000000 machineroom-0.47.3/machineroom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-30 03:59:29.000000 machineroom-0.47.3/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-30 03:59:29.747373 machineroom-0.47.3/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.47.3/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1534 2024-04-26 07:28:38.000000 machineroom-0.47.3/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-30 03:59:22.000000 machineroom-0.47.3/version
```

### Comparing `machineroom-0.47.2/.gitignore` & `machineroom-0.47.3/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.2/LICENSE` & `machineroom-0.47.3/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.2/PKG-INFO` & `machineroom-0.47.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.47.2
+Version: 0.47.3
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.47.2/README.md` & `machineroom-0.47.3/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.2/cmdbin/connect` & `machineroom-0.47.3/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.2/machineroom/__init__.py` & `machineroom-0.47.3/machineroom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.47.2'
+__version__ = '0.47.3'
```

### Comparing `machineroom-0.47.2/machineroom/const.py` & `machineroom-0.47.3/machineroom/const.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.2/machineroom/infra.py` & `machineroom-0.47.3/machineroom/infra.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,34 +41,38 @@
                 raise Exception("logic error, start should be smaller than stop")
             self.running_arr = self.running_arr[self.start_server_from:self.stop_server_at]
         if len(self.running_arr) == 0:
             raise Exception("logic error, no server to start")
 
     def run_conn_looper(self, callback_x=None):
         self.serialize_checking()
-
         for ser_i in self.running_arr:
             self.srv.read_serv_at(ser_i)
             self.stage_0()
             c = self._est_connection()
             try:
                 self.stage_1(c)
                 if callable(callback_x):
                     callback_x(c)
             except Exception as e:
                 if self.handle_exceptions(e, False):
                     pass
                 raise e
-
         self.run_tunnel_detection_off()
 
 
 class Infra1(tb.DeploymentBotFoundation):
+    server_name: str
+
     def __init__(self, x):
         super().__init__(x)
+        self.server_name = x
+
+    def match_prefix_or_subfix(self, what: str) -> bool:
+        return what in self.server_name
 
     def run_conn(self, callback_x=None):
         k = self.start_server_from
         if self.srv.serv_count < k:
             print("cannot start from out of range server number")
             return
         if self.run_tunnel_detection():
```

### Comparing `machineroom-0.47.2/machineroom/schema.json` & `machineroom-0.47.3/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.2/machineroom/sql.py` & `machineroom-0.47.3/machineroom/sql.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.2/machineroom/taskbase.py` & `machineroom-0.47.3/machineroom/taskbase.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,28 +52,28 @@
     if exists(c, path) is False:
         print(f"make path for {path}")
         c.run(f"mkdir -p {path}", warn=True, pty=True)
         return False
     return True
 
 
-def upload_cache_file(c: Connection, cache_file_name: str, if_not_exist: bool = False):
-    remote_path = os.path.join(Config.REMOTE_WS, "cache", cache_file_name)
-    local_path = os.path.join(Config.WS_LOCAL, "cache", cache_file_name)
+def upload_what_file(c: Connection, folder_name: str, cache_file_name: str, if_not_exist: bool):
+    remote_path = os.path.join(Config.REMOTE_WS, folder_name, cache_file_name)
+    local_path = os.path.join(Config.WS_LOCAL, folder_name, cache_file_name)
     if if_not_exist is True:
         if exists(c, remote_path) is False:
             c.put(local_path, remote_path)
     else:
         c.put(local_path, remote_path)
 
 
-def upload_cache_file_modify(c: Connection, cache_file_name: str, modifier, if_not_exist: bool = False):
-    remote_path = os.path.join(Config.REMOTE_WS, "cache", cache_file_name)
-    local_path = os.path.join(Config.WS_LOCAL, "cache", cache_file_name)
-    local_mod_path = os.path.join(Config.WS_LOCAL, "cache", "mod_" + cache_file_name)
+def upload_what_file_modify(c: Connection, folder_name: str, cache_file_name: str, modifier, if_not_exist: bool):
+    remote_path = os.path.join(Config.REMOTE_WS, folder_name, cache_file_name)
+    local_path = os.path.join(Config.WS_LOCAL, folder_name, cache_file_name)
+    local_mod_path = os.path.join(Config.WS_LOCAL, folder_name, "mod_" + cache_file_name)
 
     if callable(modifier):
         io = open(local_path, "r")
         content = io.read()
         io.close()
         new_content = modifier(content)
 
@@ -86,14 +86,30 @@
             if exists(c, remote_path) is False:
                 c.put(local_mod_path, remote_path)
         else:
             c.put(local_mod_path, remote_path)
         os.remove(local_mod_path)
 
 
+def upload_cache_file(c: Connection, cache_file_name: str, if_not_exist: bool = False):
+    upload_what_file(c, "cache", cache_file_name, if_not_exist)
+
+
+def upload_cache_file_modify(c: Connection, cache_file_name: str, modifier, if_not_exist: bool = False):
+    upload_what_file_modify(c, "cache", cache_file_name, modifier, if_not_exist)
+
+
+def upload_asset_file(c: Connection, cache_file_name: str, if_not_exist: bool = False):
+    upload_what_file(c, "assets", cache_file_name, if_not_exist)
+
+
+def upload_asset_file_modify(c: Connection, cache_file_name: str, modifier, if_not_exist: bool = False):
+    upload_what_file_modify(c, "assets", cache_file_name, modifier, if_not_exist)
+
+
 # https://fabric-zh.readthedocs.io/_/downloads/zh-cn/latest/pdf/
 def detect_cert(c: Connection) -> bool:
     r = c.run("cat ~/.ssh/authorized_keys", warn=True)
     line = str(r.stdout.strip().replace("\n", ""))
     t = True if Config.MY_KEY_FEATURE in line else False
     if t is True:
         print(f"certification found {Config.MY_KEY_FEATURE}")
@@ -712,14 +728,15 @@
             return False
         else:
             self.connection_err(e, fail_exit)
             return True
 
     def stage_0(self):
         ...
+
     def maybe_upgrade_docker(self):
         ...
 
     def stage_1(self, c: Connection):
         for key in Config.STAGE1:
             self._stage_loop(c, key)
```

### Comparing `machineroom-0.47.2/machineroom/tunnels/conn.py` & `machineroom-0.47.3/machineroom/tunnels/conn.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.2/machineroom/util.py` & `machineroom-0.47.3/machineroom/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,17 +481,15 @@
         n = index % self.serv_count
         line = read_file_at_line(self.path_file, n)
         line = reader_split_recognition(line)
         configuration = reader_profile_0(line)
         self._srv_index = n
         ID = configuration.get("id")
         check_for_bad_ids(ID)
-
         IP = configuration.get("host")
-
         if index == 0 and "#" in configuration.get("id"):
             TUNNEL_TYPE = IP
             print(f"Detected tunnel for machine group {ID} using {TUNNEL_TYPE}")
             self._tunnel_type = TunnelType.Recongize(TUNNEL_TYPE)
             self.profile_name = line[0].replace("#", "")
             raise FoundVPNTunnel()
```

### Comparing `machineroom-0.47.2/machineroom/worker.py` & `machineroom-0.47.3/machineroom/worker.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.2/machineroom.egg-info/PKG-INFO` & `machineroom-0.47.3/machineroom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.47.2
+Version: 0.47.3
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.47.2/machineroom.egg-info/SOURCES.txt` & `machineroom-0.47.3/machineroom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.2/setup.py` & `machineroom-0.47.3/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.47.2/update` & `machineroom-0.47.3/update`

 * *Files identical despite different names*

