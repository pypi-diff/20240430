# Comparing `tmp/cobweb-launcher-0.1.8.tar.gz` & `tmp/cobweb-launcher-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobweb-launcher-0.1.8.tar", last modified: Tue Mar 19 05:20:03 2024, max compression
+gzip compressed data, was "cobweb-launcher-0.1.9.tar", last modified: Sat Mar 23 10:01:45 2024, max compression
```

## Comparing `cobweb-launcher-0.1.8.tar` & `cobweb-launcher-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-19 05:20:03.851508 cobweb-launcher-0.1.8/
--rw-r--r--   0 jyni       (501) staff       (20)     1063 2024-03-02 08:41:06.000000 cobweb-launcher-0.1.8/LICENSE
--rw-r--r--   0 jyni       (501) staff       (20)     1091 2024-03-19 05:20:03.851361 cobweb-launcher-0.1.8/PKG-INFO
--rw-r--r--   0 jyni       (501) staff       (20)      731 2023-12-28 13:30:05.000000 cobweb-launcher-0.1.8/README.md
-drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-19 05:20:03.848870 cobweb-launcher-0.1.8/cobweb/
--rw-r--r--   0 jyni       (501) staff       (20)      326 2024-03-19 03:02:01.000000 cobweb-launcher-0.1.8/cobweb/__init__.py
--rw-r--r--   0 jyni       (501) staff       (20)     5684 2024-03-06 12:47:48.000000 cobweb-launcher-0.1.8/cobweb/bbb.py
-drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-19 05:20:03.849239 cobweb-launcher-0.1.8/cobweb/db/
--rw-r--r--   0 jyni       (501) staff       (20)       63 2024-03-02 13:30:50.000000 cobweb-launcher-0.1.8/cobweb/db/__init__.py
--rw-r--r--   0 jyni       (501) staff       (20)     4221 2024-03-07 03:46:26.000000 cobweb-launcher-0.1.8/cobweb/db/oss_db.py
--rw-r--r--   0 jyni       (501) staff       (20)     8202 2024-03-19 03:00:32.000000 cobweb-launcher-0.1.8/cobweb/db/redis_db.py
-drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-19 05:20:03.849595 cobweb-launcher-0.1.8/cobweb/db/scheduler/
--rw-r--r--   0 jyni       (501) staff       (20)        0 2024-03-02 10:49:53.000000 cobweb-launcher-0.1.8/cobweb/db/scheduler/__init__.py
--rw-r--r--   0 jyni       (501) staff       (20)      114 2024-03-02 13:56:38.000000 cobweb-launcher-0.1.8/cobweb/db/scheduler/default.py
--rw-r--r--   0 jyni       (501) staff       (20)      821 2024-03-02 13:56:38.000000 cobweb-launcher-0.1.8/cobweb/db/scheduler/textfile.py
-drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-19 05:20:03.850142 cobweb-launcher-0.1.8/cobweb/db/storer/
--rw-r--r--   0 jyni       (501) staff       (20)        0 2024-03-02 12:45:22.000000 cobweb-launcher-0.1.8/cobweb/db/storer/__init__.py
--rw-r--r--   0 jyni       (501) staff       (20)      182 2024-03-02 13:56:38.000000 cobweb-launcher-0.1.8/cobweb/db/storer/console.py
--rw-r--r--   0 jyni       (501) staff       (20)     1731 2024-03-02 15:12:51.000000 cobweb-launcher-0.1.8/cobweb/db/storer/loghub.py
--rw-r--r--   0 jyni       (501) staff       (20)      412 2024-03-02 13:56:38.000000 cobweb-launcher-0.1.8/cobweb/db/storer/redis.py
--rw-r--r--   0 jyni       (501) staff       (20)      415 2024-03-02 13:56:38.000000 cobweb-launcher-0.1.8/cobweb/db/storer/textfile.py
--rw-r--r--   0 jyni       (501) staff       (20)      320 2024-03-06 09:11:57.000000 cobweb-launcher-0.1.8/cobweb/decorators.py
-drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-19 05:20:03.850439 cobweb-launcher-0.1.8/cobweb/distributed/
--rw-r--r--   0 jyni       (501) staff       (20)        0 2024-03-18 15:34:54.000000 cobweb-launcher-0.1.8/cobweb/distributed/__init__.py
--rw-r--r--   0 jyni       (501) staff       (20)     7998 2024-03-18 15:43:42.000000 cobweb-launcher-0.1.8/cobweb/distributed/launcher.py
--rw-r--r--   0 jyni       (501) staff       (20)     4568 2024-03-19 05:19:41.000000 cobweb-launcher-0.1.8/cobweb/distributed/models.py
--rw-r--r--   0 jyni       (501) staff       (20)      802 2024-03-02 14:41:45.000000 cobweb-launcher-0.1.8/cobweb/interface.py
--rw-r--r--   0 jyni       (501) staff       (20)     2384 2024-03-02 10:49:53.000000 cobweb-launcher-0.1.8/cobweb/log.py
--rw-r--r--   0 jyni       (501) staff       (20)      288 2024-03-18 06:24:00.000000 cobweb-launcher-0.1.8/cobweb/setting.py
-drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-19 05:20:03.850727 cobweb-launcher-0.1.8/cobweb/single/
--rw-r--r--   0 jyni       (501) staff       (20)        0 2024-03-02 10:49:53.000000 cobweb-launcher-0.1.8/cobweb/single/__init__.py
--rw-r--r--   0 jyni       (501) staff       (20)     7302 2024-03-19 03:09:28.000000 cobweb-launcher-0.1.8/cobweb/single/launcher.py
--rw-r--r--   0 jyni       (501) staff       (20)     4247 2024-03-19 05:19:41.000000 cobweb-launcher-0.1.8/cobweb/single/models.py
--rw-r--r--   0 jyni       (501) staff       (20)     1405 2024-03-18 06:24:00.000000 cobweb-launcher-0.1.8/cobweb/task.py
--rw-r--r--   0 jyni       (501) staff       (20)     2651 2024-03-19 04:43:18.000000 cobweb-launcher-0.1.8/cobweb/utils.py
-drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-19 05:20:03.851216 cobweb-launcher-0.1.8/cobweb_launcher.egg-info/
--rw-r--r--   0 jyni       (501) staff       (20)     1091 2024-03-19 05:20:03.000000 cobweb-launcher-0.1.8/cobweb_launcher.egg-info/PKG-INFO
--rw-r--r--   0 jyni       (501) staff       (20)      822 2024-03-19 05:20:03.000000 cobweb-launcher-0.1.8/cobweb_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 jyni       (501) staff       (20)        1 2024-03-19 05:20:03.000000 cobweb-launcher-0.1.8/cobweb_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 jyni       (501) staff       (20)       65 2024-03-19 05:20:03.000000 cobweb-launcher-0.1.8/cobweb_launcher.egg-info/requires.txt
--rw-r--r--   0 jyni       (501) staff       (20)        7 2024-03-19 05:20:03.000000 cobweb-launcher-0.1.8/cobweb_launcher.egg-info/top_level.txt
--rw-r--r--   0 jyni       (501) staff       (20)       38 2024-03-19 05:20:03.851543 cobweb-launcher-0.1.8/setup.cfg
--rw-r--r--   0 jyni       (501) staff       (20)      728 2024-03-19 05:20:01.000000 cobweb-launcher-0.1.8/setup.py
+drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-23 10:01:45.443875 cobweb-launcher-0.1.9/
+-rw-r--r--   0 jyni       (501) staff       (20)     1063 2024-03-02 08:41:06.000000 cobweb-launcher-0.1.9/LICENSE
+-rw-r--r--   0 jyni       (501) staff       (20)     1216 2024-03-23 10:01:45.443657 cobweb-launcher-0.1.9/PKG-INFO
+-rw-r--r--   0 jyni       (501) staff       (20)      731 2023-12-28 13:30:05.000000 cobweb-launcher-0.1.9/README.md
+drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-23 10:01:45.438096 cobweb-launcher-0.1.9/cobweb/
+-rw-r--r--   0 jyni       (501) staff       (20)      227 2024-03-23 09:07:49.000000 cobweb-launcher-0.1.9/cobweb/__init__.py
+-rw-r--r--   0 jyni       (501) staff       (20)     5684 2024-03-06 12:47:48.000000 cobweb-launcher-0.1.9/cobweb/bbb.py
+-rw-r--r--   0 jyni       (501) staff       (20)      462 2024-03-22 16:48:49.000000 cobweb-launcher-0.1.9/cobweb/constant.py
+drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-23 10:01:45.438851 cobweb-launcher-0.1.9/cobweb/db/
+-rw-r--r--   0 jyni       (501) staff       (20)      139 2024-03-22 16:40:13.000000 cobweb-launcher-0.1.9/cobweb/db/__init__.py
+-rw-r--r--   0 jyni       (501) staff       (20)     4221 2024-03-07 03:46:26.000000 cobweb-launcher-0.1.9/cobweb/db/oss_db.py
+-rw-r--r--   0 jyni       (501) staff       (20)     8179 2024-03-22 16:40:13.000000 cobweb-launcher-0.1.9/cobweb/db/redis_db.py
+drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-23 10:01:45.439633 cobweb-launcher-0.1.9/cobweb/db/scheduler/
+-rw-r--r--   0 jyni       (501) staff       (20)       51 2024-03-22 16:40:13.000000 cobweb-launcher-0.1.9/cobweb/db/scheduler/__init__.py
+-rw-r--r--   0 jyni       (501) staff       (20)       79 2024-03-22 16:40:13.000000 cobweb-launcher-0.1.9/cobweb/db/scheduler/default.py
+-rw-r--r--   0 jyni       (501) staff       (20)      786 2024-03-22 16:40:13.000000 cobweb-launcher-0.1.9/cobweb/db/scheduler/textfile.py
+drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-23 10:01:45.440744 cobweb-launcher-0.1.9/cobweb/db/storer/
+-rw-r--r--   0 jyni       (501) staff       (20)       49 2024-03-22 16:40:13.000000 cobweb-launcher-0.1.9/cobweb/db/storer/__init__.py
+-rw-r--r--   0 jyni       (501) staff       (20)      153 2024-03-22 16:40:13.000000 cobweb-launcher-0.1.9/cobweb/db/storer/console.py
+-rw-r--r--   0 jyni       (501) staff       (20)     1702 2024-03-22 16:40:13.000000 cobweb-launcher-0.1.9/cobweb/db/storer/loghub.py
+-rw-r--r--   0 jyni       (501) staff       (20)      386 2024-03-22 16:40:12.000000 cobweb-launcher-0.1.9/cobweb/db/storer/textfile.py
+-rw-r--r--   0 jyni       (501) staff       (20)      318 2024-03-22 16:48:49.000000 cobweb-launcher-0.1.9/cobweb/decorators.py
+drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-23 10:01:45.441023 cobweb-launcher-0.1.9/cobweb/equip/
+-rw-r--r--   0 jyni       (501) staff       (20)      238 2024-03-22 16:48:49.000000 cobweb-launcher-0.1.9/cobweb/equip/__init__.py
+drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-23 10:01:45.441644 cobweb-launcher-0.1.9/cobweb/equip/distributed/
+-rw-r--r--   0 jyni       (501) staff       (20)        0 2024-03-22 16:48:49.000000 cobweb-launcher-0.1.9/cobweb/equip/distributed/__init__.py
+-rw-r--r--   0 jyni       (501) staff       (20)     7475 2024-03-22 16:48:49.000000 cobweb-launcher-0.1.9/cobweb/equip/distributed/launcher.py
+-rw-r--r--   0 jyni       (501) staff       (20)     4815 2024-03-22 16:48:49.000000 cobweb-launcher-0.1.9/cobweb/equip/distributed/models.py
+drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-23 10:01:45.442429 cobweb-launcher-0.1.9/cobweb/equip/single/
+-rw-r--r--   0 jyni       (501) staff       (20)        0 2024-03-02 10:49:53.000000 cobweb-launcher-0.1.9/cobweb/equip/single/__init__.py
+-rw-r--r--   0 jyni       (501) staff       (20)     6702 2024-03-23 09:27:35.000000 cobweb-launcher-0.1.9/cobweb/equip/single/launcher.py
+-rw-r--r--   0 jyni       (501) staff       (20)     4447 2024-03-22 16:48:49.000000 cobweb-launcher-0.1.9/cobweb/equip/single/models.py
+-rw-r--r--   0 jyni       (501) staff       (20)      802 2024-03-02 14:41:45.000000 cobweb-launcher-0.1.9/cobweb/interface.py
+-rw-r--r--   0 jyni       (501) staff       (20)     2384 2024-03-02 10:49:53.000000 cobweb-launcher-0.1.9/cobweb/log.py
+-rw-r--r--   0 jyni       (501) staff       (20)     1704 2024-03-22 15:42:17.000000 cobweb-launcher-0.1.9/cobweb/task.py
+-rw-r--r--   0 jyni       (501) staff       (20)     2651 2024-03-19 04:43:18.000000 cobweb-launcher-0.1.9/cobweb/utils.py
+drwxr-xr-x   0 jyni       (501) staff       (20)        0 2024-03-23 10:01:45.443419 cobweb-launcher-0.1.9/cobweb_launcher.egg-info/
+-rw-r--r--   0 jyni       (501) staff       (20)     1216 2024-03-23 10:01:45.000000 cobweb-launcher-0.1.9/cobweb_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 jyni       (501) staff       (20)      858 2024-03-23 10:01:45.000000 cobweb-launcher-0.1.9/cobweb_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 jyni       (501) staff       (20)        1 2024-03-23 10:01:45.000000 cobweb-launcher-0.1.9/cobweb_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 jyni       (501) staff       (20)       65 2024-03-23 10:01:45.000000 cobweb-launcher-0.1.9/cobweb_launcher.egg-info/requires.txt
+-rw-r--r--   0 jyni       (501) staff       (20)        7 2024-03-23 10:01:45.000000 cobweb-launcher-0.1.9/cobweb_launcher.egg-info/top_level.txt
+-rw-r--r--   0 jyni       (501) staff       (20)       38 2024-03-23 10:01:45.443920 cobweb-launcher-0.1.9/setup.cfg
+-rw-r--r--   0 jyni       (501) staff       (20)      728 2024-03-23 09:28:24.000000 cobweb-launcher-0.1.9/setup.py
```

### Comparing `cobweb-launcher-0.1.8/LICENSE` & `cobweb-launcher-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cobweb-launcher-0.1.8/PKG-INFO` & `cobweb-launcher-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: cobweb-launcher
-Version: 0.1.8
+Version: 0.1.9
 Summary: spider_hole
 Home-page: https://github.com/Juannie-PP/cobweb
 Author: Juannie-PP
 Author-email: 2604868278@qq.com
 License: MIT
 Keywords: cobweb-launcher, cobweb
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.19.1
+Requires-Dist: oss2>=2.18.1
+Requires-Dist: redis>=4.4.4
+Requires-Dist: aliyun-log-python-sdk
 
 # cobweb
 
 > 通用爬虫框架： 1.单机模式采集框架；2.分布式采集框架
 > 
 >  5部分
 >
```

### Comparing `cobweb-launcher-0.1.8/README.md` & `cobweb-launcher-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cobweb-launcher-0.1.8/cobweb/bbb.py` & `cobweb-launcher-0.1.9/cobweb/bbb.py`

 * *Files identical despite different names*

### Comparing `cobweb-launcher-0.1.8/cobweb/db/oss_db.py` & `cobweb-launcher-0.1.9/cobweb/db/oss_db.py`

 * *Files identical despite different names*

### Comparing `cobweb-launcher-0.1.8/cobweb/db/redis_db.py` & `cobweb-launcher-0.1.9/cobweb/db/redis_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 import time
 import redis
-from cobweb import Seed, log
-from cobweb.decorators import check_redis_status
+from . import log, decorators, Seed, Setting, DealModel
+# from cobweb.decorators import decorators.check_redis_status
+# from cobweb.constant import Setting, DealModel
 
 
 class RedisDB:
 
     def __init__(
             self,
             project: str,
             task_name: str,
             config: dict,
-            model: int,
-            cs_lct: int,
-            rs_time: int,
     ):
         pool = redis.ConnectionPool(**config)
         self.heartbeat_key = f"{project}:{task_name}:heartbeat"  # redis type string
         self.spider_key = f"{project}:{task_name}:seed_info:spider"  # redis type zset, .format(priority)
         self.storer_key = f"{project}:{task_name}:seed_info:storer:%s"  # redis type set,
         self.failed_key = f"{project}:{task_name}:seed_info:failed"  # redis type set, .format(priority)
         self.succeed_key = f"{project}:{task_name}:seed_info:succeed"  # redis type set, .format(priority)
         self.update_lock = f"{project}:{task_name}:update_seed_lock"  # redis type string
         self.check_lock = f"{project}:{task_name}:check_seed_lock"  # redis type string
         self.scheduler_lock = f"{project}:{task_name}:scheduler_lock"  # redis type string
         self.client = redis.Redis(connection_pool=pool)
-        self.model = model
-        self.cs_lct = cs_lct
-        self.rs_time = rs_time
 
-    @check_redis_status
+    @decorators.check_redis_status
     def _get_lock(self, key, t=15, timeout=3, sleep_time=0.1):
         begin_time = int(time.time())
         while True:
             if self.client.setnx(key, ""):
                 self.client.expire(key, t)
                 return True
             if int(time.time()) - begin_time > timeout:
@@ -51,15 +46,15 @@
                 self.client.expire(key, t)
             return False
         else:
             ttl = self.client.ttl(key)
             log.info("ttl: " + str(ttl))
             return False
 
-    @check_redis_status
+    @decorators.check_redis_status
     def _deal_seed(self, seeds, is_add: bool):
         if not seeds:
             return None
 
         if not isinstance(seeds, list):
             seeds = [seeds]
 
@@ -69,45 +64,43 @@
             if not isinstance(seed, Seed):
                 seed = Seed(seed)
             item_info[seed.format_seed] = seed._priority
 
         if item_info:
             self.client.zadd(self.spider_key, mapping=item_info, nx=is_add, xx=not is_add)
 
-    @check_redis_status
+    @decorators.check_redis_status
     def add_seed(self, seeds):
         self._deal_seed(seeds, is_add=True)
 
-    @check_redis_status
+    @decorators.check_redis_status
     def reset_seed(self, seeds):
         self._deal_seed(seeds, is_add=False)
 
-    @check_redis_status
+    @decorators.check_redis_status
     def del_seed(self, seeds, spider_status: bool = True):
         if not seeds:
             return None
 
         if not isinstance(seeds, list):
             seeds = [seeds]
 
         seeds = [seed if isinstance(seed, Seed) else Seed(seed) for seed in seeds]
 
         if seeds:
-            # redis_key = self.succeed_key if spider_status else self.failed_key
             redis_key = None
-            if spider_status:
-                if isinstance(self.model, int) and self.model == 2:
-                    redis_key = self.succeed_key
-            else:
+            if spider_status and Setting.DEAL_MODEL in [DealModel.success, DealModel.polling]:
+                redis_key = self.succeed_key
+            elif not spider_status:
                 redis_key = self.failed_key
             if redis_key:
                 self.client.sadd(redis_key, *(str(seed) for seed in seeds))
             self.client.zrem(self.spider_key, *(seed.format_seed for seed in seeds))
 
-    @check_redis_status
+    @decorators.check_redis_status
     def set_storer(self, key, seeds):
         if not seeds:
             return None
 
         if not isinstance(seeds, list):
             seeds = [seeds]
 
@@ -118,15 +111,15 @@
                 seed = Seed(seed)
             item_info[seed.format_seed] = score
 
         if item_info:
             self.client.zadd(self.storer_key % key, mapping=item_info)
             log.info(f"zadd storer key: length {len(item_info.keys())}")
 
-    @check_redis_status
+    @decorators.check_redis_status
     def get_seed(self, length: int = 200):
         cs = time.time()
 
         if self._get_lock(key=self.update_lock):
 
             update_item, result = {}, []
 
@@ -144,37 +137,37 @@
             if result:
                 self.client.zadd(self.spider_key, mapping=update_item, xx=True)
 
             self.client.delete(self.update_lock)
             log.info("push seeds into queue time: " + str(time.time() - cs))
             return result
 
-    @check_redis_status
+    @decorators.check_redis_status
     def check_spider_queue(self, stop, storer_num):
         while not stop.is_set():
             # 每15s获取check锁,等待600s后仍获取不到锁则重试;获取到锁后，设置锁的存活时间为${cs_lct}s
-            if self._get_lock(key=self.check_lock, t=self.cs_lct, timeout=600, sleep_time=3):
+            if self._get_lock(key=self.check_lock, t=Setting.CHECK_LOCK_TIME, timeout=600, sleep_time=3):
                 heartbeat = True if self.client.exists(self.heartbeat_key) else False
                 # 重启重制score值，否则获取${rs_time}分钟前的分数值
-                score = -int(time.time()) + self.rs_time if heartbeat else "-inf"
+                score = -int(time.time()) + Setting.RESET_SCORE if heartbeat else "-inf"
 
                 keys = self.client.keys(self.storer_key % "*")
 
                 if keys and len(keys) >= storer_num:
                     intersection_key = self.storer_key % "intersection"
                     self.client.delete(intersection_key)
                     self.client.zinterstore(intersection_key, keys)
 
                     while True:
                         members = self.client.zrange(intersection_key, 0, 1999)
                         if not members:
                             break
                         for key in keys:
                             self.client.zrem(key, *members)
-                        if self.model == 2:
+                        if Setting.DEAL_MODEL in [DealModel.success, DealModel.polling]:
                             self.client.sadd(self.succeed_key, *members)
                         self.client.zrem(self.spider_key, *members)
                         self.client.zrem(intersection_key, *members)
                         log.info("succeed spider data ...")
 
                 for key in keys:
                     self.client.zremrangebyscore(key, min=score, max="(0")
@@ -189,35 +182,32 @@
                         reset_items[value] = int(reset_score)
                     if reset_items:
                         self.client.zadd(self.spider_key, mapping=reset_items, xx=True)
 
                 if not heartbeat:
                     self.client.setex(self.heartbeat_key, 15, "")
 
-                # self.client.delete(self.check_lock)
-                # time.sleep(3)
-
-    @check_redis_status
+    @decorators.check_redis_status
     def set_heartbeat(self, stop):
         time.sleep(5)
         while not stop.is_set():
             self.client.setex(self.heartbeat_key, 5, "")
             time.sleep(3)
 
-    # @check_redis_status
+    # @decorators.check_redis_status
     # def heartbeat(self):
     #     """
     #     返回心跳key剩余存活时间
     #     """
     #     return self.client.ttl(self.heartbeat_key)
 
-    @check_redis_status
+    @decorators.check_redis_status
     def spider_queue_length(self):
         return self.client.zcard(self.spider_key)
 
-    @check_redis_status
+    @decorators.check_redis_status
     def ready_seed_length(self):
         return self.client.zcount(self.spider_key, min=0, max="+inf")
 
-    @check_redis_status
+    @decorators.check_redis_status
     def get_scheduler_lock(self):
         return self._get_lock(self.scheduler_lock)
```

### Comparing `cobweb-launcher-0.1.8/cobweb/db/storer/loghub.py` & `cobweb-launcher-0.1.9/cobweb/db/storer/loghub.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
+from . import Inf, log
 from aliyun.log import LogClient, LogItem, PutLogsRequest
-from cobweb import log, StorerInterface
 
 
-class Loghub(StorerInterface):
+class Loghub(Inf):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.client = None
 
     def init_loghub_clint(self):
         try:
```

### Comparing `cobweb-launcher-0.1.8/cobweb/distributed/launcher.py` & `cobweb-launcher-0.1.9/cobweb/equip/distributed/launcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import time
 import threading
-from threading import Thread
 
+from .. import log, sqn, rtn, pim
+from .. import Queue, DBItem, RedisDB, Setting
 from .models import Scheduler, Spider, Storer
-from cobweb import log, Queue, DBItem, RedisDB
-from cobweb.setting import MODEL, RESET_SCORE, CHECK_LOCK_TIME
-from cobweb.utils import (
-    struct_queue_name as sqn,
-    restore_table_name as rtn,
-    parse_import_model as pim,
-)
 
 
 def check(stop, last, spider, scheduler, storer_list, ready_seed_length, spider_queue_length):
     log.info("run check thread after 30 seconds...")
     time.sleep(30)
     spider_info = """
 ------------------- check: {0} ------------------
@@ -33,19 +27,18 @@
         storer_upload_queue_list = []
         for storer in storer_list:
             storer_upload_queue_list.append(
                 f"{storer.__class__.__name__} storer queue length: {storer.queue.length}"
             )
         if (
                 scheduler.stop and
-                # not redis_ready_seed_length and
                 not memory_seed_queue_length and
                 not running_spider_thread_num
         ):
-            if not MODEL:
+            if not Setting.LAUNCHER_MODEL:
                 log.info("spider is done?")
             last.set()
             time.sleep(3)
             storer_queue_empty = True
             storer_upload_queue_list = []
             for storer in storer_list:
                 if storer.queue.length:
@@ -54,15 +47,15 @@
                     f"{storer.__class__.__name__} storer queue length: {storer.queue.length}"
                 )
             if (
                     storer_queue_empty and
                     not redis_ready_seed_length and
                     not redis_spider_seed_length
             ):
-                if MODEL:
+                if Setting.LAUNCHER_MODEL:
                     log.info("waiting for push seeds...")
                     status = "waiting"
                     time.sleep(30)
                 else:
                     log.info("spider done!")
                     break
 
@@ -85,40 +78,23 @@
 
 def launcher(task):
     """
     任务启动装饰器
     :param task: 任务配置信息
     """
     def decorator(func):
-        """
-        Item:
-            Textfile()
-            Loghub()
-            Console()
-        e.g.
-        task.fields = "a,b"
-        func(item, seed)
-            a = "a"
-            b = "b"
-            data = {"a": "a", "b": "b"}
-            yield item.Loghub(**data)
-            yield item.Loghub(a=a, b=b)
-        """
         storer_list = []
 
         # 程序结束事件
         last = threading.Event()
         # 停止采集事件
         stop = threading.Event()
 
         # 初始化redis信息
-        redis_db = RedisDB(
-            task.project, task.task_name, task.redis_info,
-            model=MODEL, cs_lct=CHECK_LOCK_TIME, rs_time=RESET_SCORE
-        )
+        redis_db = RedisDB(task.project, task.task_name, task.redis_info)
 
         log.info("初始化cobweb!")
 
         seed_queue = Queue()
 
         if task.scheduler_info is None:
             task.scheduler_info = dict()
@@ -135,17 +111,14 @@
 
         # 初始化调度器
         scheduler = SchedulerTmp(
             table=table, sql=sql, size=size, queue=seed_queue,
             length=task.scheduler_queue_length, config=scheduler_config
         )
 
-        # 初始化采集器
-        spider = Spider(seed_queue, task.max_retries)
-
         # 解析存储器信息
         storer_info_list = task.storer_info or []
         if not isinstance(storer_info_list, list):
             storer_info_list = [storer_info_list]
 
         # new item
         item = type("Item", (object,), {"redis_client": redis_db.client})()
@@ -174,65 +147,68 @@
             storer = StorerTmp(
                 table=table_name, fields=fields,
                 length=task.storer_queue_length,
                 queue=queue, config=storer_config
             )
             storer_list.append(storer)
 
-        Thread(target=redis_db.check_spider_queue, args=(stop, len(storer_list))).start()
-        Thread(target=redis_db.set_heartbeat, args=(stop,)).start()
+        # 初始化采集器
+        spider = Spider(seed_queue, storer_list and True, task.max_retries)
+
+        threading.Thread(target=redis_db.check_spider_queue, args=(stop, len(storer_list))).start()
+        threading.Thread(target=redis_db.set_heartbeat, args=(stop,)).start()
 
         # 推送初始种子
         # seeds = start_seeds(task.start_seed)
         redis_db.add_seed(task.seeds)
         # 启动调度器, 调度至redis队列
-        Thread(
+        threading.Thread(
             # name="xxxx_schedule_seeds",
             target=scheduler.schedule_seed,
             args=(
                 redis_db.ready_seed_length,
                 redis_db.get_scheduler_lock,
                 redis_db.add_seed
             )
         ).start()
 
         # 启动调度器, 调度任务队列
-        Thread(
+        threading.Thread(
             # name="xxxx_schedule_task",
             target=scheduler.schedule_task,
             args=(
                 stop, redis_db.get_seed,
                 redis_db.ready_seed_length
             )
         ).start()
 
         # 启动采集器
         for index in range(task.spider_num):
-            Thread(
+            threading.Thread(
                 # name=f"xxxx_spider_task:{index}",
                 target=spider.spider_task,
                 args=(
                     stop, func, item,
                     redis_db.del_seed
                 )
             ).start()
 
         # 启动存储器
         for storer in storer_list:
-            Thread(
+            threading.Thread(
                 # name=f"xxxx_store_task:{storer.table}",
                 target=storer.store_task,
                 args=(
                     stop, last,
                     redis_db.reset_seed,
                     redis_db.set_storer
                 )
             ).start()
 
-        Thread(
+        threading.Thread(
             # name="check_spider",
             target=check,
             args=(
                 stop, last, spider,
                 scheduler, storer_list,
                 redis_db.ready_seed_length,
                 redis_db.spider_queue_length,
```

### Comparing `cobweb-launcher-0.1.8/cobweb/distributed/models.py` & `cobweb-launcher-0.1.9/cobweb/equip/distributed/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import time
 from hashlib import md5
-from cobweb import log, Queue, Seed
-from cobweb.utils import issubclass_cobweb_inf
+from inspect import isgenerator
 
+from .. import log, ici
+from .. import DealModel, Queue, Seed
 # from pympler import asizeof
 
 
 class Scheduler:
 
     def schedule_seed(self, ready_seed_length, get_scheduler_lock, add_seed):
 
         inf_name = "SchedulerInterface"
-        if not issubclass_cobweb_inf(self.__class__, inf_name):
+        if not ici(self.__class__, inf_name):
             raise Exception("not have schedule function!")
 
         if self.__class__.__name__ == "Default":
             self.stop = True
             return None
 
         while not self.stop:
@@ -44,73 +45,83 @@
             seeds = get_seed(self.length)
             self.queue.push(seeds)
         log.info(f"close thread: schedule_task")
 
 
 class Spider:
 
-    def __init__(self, queue, max_retries=5):
+    def __init__(self, queue, storage, max_retries=5):
         self.spider_in_progress = Queue()
         self.max_retries = max_retries
+        self.storage = storage
         self.queue = queue
 
     def spider_task(self, stop, func, item, del_seed):
         while not stop.is_set():
             seed = self.queue.pop()
             if not seed:
                 time.sleep(3)
                 continue
             elif seed._retry >= self.max_retries:
                 del_seed(seed, spider_status=False)
                 continue
             try:
                 self.spider_in_progress.push(1, direct_insertion=True)
                 # log.info("spider seed: " + str(seed))
-                ret_count = 0
-                status = None
+
                 store_queue = None
                 store_data = list()
-                for it in func(item, seed):
-                    ret_count += 1
+
+                iterators = func(item, seed)
+
+                if not isgenerator(iterators):
+                    if not self.storage:
+                        del_seed(seed, spider_status=True)
+                        continue
+                    raise TypeError(f"{func.__name__} isn't a generator")
+
+                for it in iterators:
                     if getattr(it, "table_name", None):
                         if not store_queue:
                             store_queue = it.queue()
                         store_data.append(it.struct_data)
                     elif isinstance(it, Seed):
                         self.queue.push(it)
-                    elif any(isinstance(it, t) for t in (list, tuple)):
-                        self.queue.push([s if isinstance(s, Seed) else Seed(s) for s in it])
-                    elif isinstance(it, bool):
-                        status = it
+
+                    elif isinstance(it, str) and it == DealModel.polling:
+                        self.queue.push(seed)
+                        break
+                    elif isinstance(it, str) and it == DealModel.success:
+                        del_seed(seed, spider_status=True)
+                        break
+                    elif isinstance(it, str) and it == DealModel.failure:
+                        del_seed(seed, spider_status=False)
+                        break
+                    else:
+                        raise TypeError("yield value type error!")
 
                 if store_queue and store_data:
                     store_data.append(seed)
                     store_queue.push(store_data)
 
-                if status:
-                    del_seed(seed, spider_status=True)
-                elif not ret_count or status is False:
-                    seed._retry += 1
-                    self.queue.push(seed)
-
             except Exception as e:
                 seed._retry += 1
                 self.queue.push(seed)
                 log.info(f"{str(seed)} -> {str(e)}")
             finally:
                 self.spider_in_progress.pop()
         log.info(f"close thread: spider")
 
 
 class Storer:
 
     def store_task(self, stop, last, reset_seed, set_storer):
 
         inf_name = "StorerInterface"
-        if not issubclass_cobweb_inf(self.__class__, inf_name):
+        if not ici(self.__class__, inf_name):
             return None
 
         if not getattr(self, "store", None):
             raise Exception("not have store function!")
 
         storer_name = self.__class__.__name__ + self.table
         store_key_id = md5(storer_name.encode()).hexdigest()
@@ -127,17 +138,15 @@
                     if isinstance(data, Seed):
                         seeds.append(data)
                         if len(data_list) >= self.length:
                             break
                         continue
                     data_list.append(data)
 
-                if data_list:
-                    if self.store(data_list):
-                        set_storer(store_key_id, seeds)
-                    else:
-                        reset_seed(seeds)
-                    continue
+                if self.store(data_list):
+                    set_storer(store_key_id, seeds)
+                else:
+                    reset_seed(seeds)
 
             time.sleep(3)
 
         log.info(f"close thread: {storer_name}")
```

### Comparing `cobweb-launcher-0.1.8/cobweb/interface.py` & `cobweb-launcher-0.1.9/cobweb/interface.py`

 * *Files identical despite different names*

### Comparing `cobweb-launcher-0.1.8/cobweb/log.py` & `cobweb-launcher-0.1.9/cobweb/log.py`

 * *Files identical despite different names*

### Comparing `cobweb-launcher-0.1.8/cobweb/single/launcher.py` & `cobweb-launcher-0.1.9/cobweb/equip/single/launcher.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import time
 import threading
-from threading import Thread
 
+from .. import log, sqn, rtn, pim
+from .. import Queue, DBItem, RedisDB, Setting
 from .models import Scheduler, Spider, Storer
-from cobweb import log, Queue, DBItem, RedisDB
-from cobweb.setting import MODEL, RESET_SCORE, CHECK_LOCK_TIME
-from cobweb.utils import (
-    struct_queue_name as sqn,
-    restore_table_name as rtn,
-    parse_import_model as pim,
-)
 
 
 def check(stop, last, spider, scheduler, storer, ready_seed_length, spider_queue_length):
     log.info("run check thread after 30 seconds...")
     time.sleep(30)
     spider_info = """
 ------------------- check: {0} ------------------
@@ -25,35 +19,34 @@
 -----------------------  end  -----------------------"""
     while True:
         status = "running"
         running_spider_thread_num = spider.spider_in_progress.length
         redis_ready_seed_length = ready_seed_length()
         redis_spider_seed_length = spider_queue_length()
         memory_seed_queue_length = scheduler.queue.length
-        storer_upload_queue_length = storer.queue.length
+        storer_upload_queue_length = storer.queue.length if storer else None
         if (
                 scheduler.stop and
-                # not redis_ready_seed_length and
                 not memory_seed_queue_length and
                 not running_spider_thread_num
         ):
-            if not MODEL:
+            if not Setting.LAUNCHER_MODEL:
                 log.info("spider is done?")
             last.set()
             time.sleep(3)
             storer_queue_empty = True
-            if storer.queue.length:
+            if storer and storer.queue.length:
                 storer_queue_empty = False
-            storer_upload_queue_length = storer.queue.length
+            storer_upload_queue_length = storer.queue.length if storer else None
             if (
                     storer_queue_empty and
                     not redis_ready_seed_length and
                     not redis_spider_seed_length
             ):
-                if MODEL:
+                if Setting.LAUNCHER_MODEL:
                     log.info("waiting for push seeds...")
                     status = "waiting"
                     time.sleep(30)
                 else:
                     log.info("spider done!")
                     break
 
@@ -74,75 +67,48 @@
 
 def launcher(task):
     """
     任务启动装饰器
     :param task: 任务配置信息
     """
     def decorator(func):
-        """
-        Item:
-            Textfile()
-            Loghub()
-            Console()
-        e.g.
-        task.fields = "a,b"
-        func(item, seed)
-            a = "a"
-            b = "b"
-            data = {"a": "a", "b": "b"}
-            yield item.Loghub(**data)
-            yield item.Loghub(a=a, b=b)
-        """
-        storer_list = []
-
         # 程序结束事件
         last = threading.Event()
         # 停止采集事件
         stop = threading.Event()
 
         # 初始化redis信息
-        redis_db = RedisDB(
-            task.project, task.task_name, task.redis_info,
-            model=MODEL, cs_lct=CHECK_LOCK_TIME, rs_time=RESET_SCORE
-        )
+        redis_db = RedisDB(task.project, task.task_name, task.redis_info)
 
         # new item
         item = type("Item", (object,), {"redis_client": redis_db.client})()
 
         log.info("初始化cobweb!")
 
         seed_queue = Queue()
 
         scheduler_info = task.scheduler_info or dict()
-
         # 调度器动态继承
         sql = scheduler_info.get("sql")
         table = scheduler_info.get("table")
         size = scheduler_info.get("size")
         scheduler_config = scheduler_info.get("config")
         scheduler_db = scheduler_info.get("db", "default")
         DB, class_name = pim(scheduler_db, "scheduler")
         # SchedulerDB, table, sql, length, size, config = task.scheduler_info
         SchedulerTmp = type(class_name, (Scheduler, DB), {})
-
         # 初始化调度器
         scheduler = SchedulerTmp(
             table=table, sql=sql, size=size, queue=seed_queue,
             length=task.scheduler_queue_length, config=scheduler_config
         )
 
-        # 初始化采集器
-        spider = Spider(seed_queue, task.max_retries)
-
         storer = None
-
-        # 解析存储器信息
         storer_info = task.storer_info or dict()
 
-        # for storer_info in storer_info_list:
         if storer_info:
             storer_db = storer_info["db"]
             fields = storer_info["fields"]
             storer_table = storer_info.get("table", "console")
             storer_config = storer_info.get("config")
 
             StorerDB, class_name = pim(storer_db, "storer")
@@ -162,65 +128,68 @@
             table_name = rtn(table_name=storer_table)
             storer = StorerTmp(
                 table=table_name, fields=fields,
                 length=task.storer_queue_length,
                 queue=queue, config=storer_config
             )
 
-        Thread(target=redis_db.check_spider_queue, args=(stop, len(storer_list))).start()
-        Thread(target=redis_db.set_heartbeat, args=(stop,)).start()
+        # 初始化采集器
+        spider = Spider(seed_queue, storer and True, task.max_retries)
+
+        threading.Thread(target=redis_db.check_spider_queue, args=(stop, 0)).start()
+        threading.Thread(target=redis_db.set_heartbeat, args=(stop,)).start()
 
         # 推送初始种子
         # seeds = start_seeds(task.start_seed)
         redis_db.add_seed(task.seeds)
         # 启动调度器, 调度至redis队列
-        Thread(
+        threading.Thread(
             # name="xxxx_schedule_seeds",
             target=scheduler.schedule_seed,
             args=(
                 redis_db.ready_seed_length,
                 redis_db.get_scheduler_lock,
                 redis_db.add_seed
             )
         ).start()
 
         # 启动调度器, 调度任务队列
-        Thread(
+        threading.Thread(
             # name="xxxx_schedule_task",
             target=scheduler.schedule_task,
             args=(
                 stop, redis_db.get_seed,
                 redis_db.ready_seed_length
             )
         ).start()
 
         # 启动采集器
         for index in range(task.spider_num):
-            Thread(
+            threading.Thread(
                 # name=f"xxxx_spider_task:{index}",
                 target=spider.spider_task,
                 args=(
                     stop, func, item,
                     redis_db.del_seed
                 )
             ).start()
 
         # 启动存储器
         if storer:
-            Thread(
+            threading.Thread(
                 # name=f"xxxx_store_task:{storer.table}",
                 target=storer.store_task,
                 args=(
                     stop, last,
                     redis_db.reset_seed,
                     redis_db.del_seed
                 )
             ).start()
 
-        Thread(
+        threading.Thread(
             # name="check_spider",
             target=check,
             args=(
                 stop, last, spider,
                 scheduler, storer,
                 redis_db.ready_seed_length,
                 redis_db.spider_queue_length,
```

### Comparing `cobweb-launcher-0.1.8/cobweb/single/models.py` & `cobweb-launcher-0.1.9/cobweb/equip/single/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import time
-from cobweb import log, Queue, Seed
-from cobweb.utils import issubclass_cobweb_inf
+from inspect import isgenerator
 # from pympler import asizeof
+from .. import log, ici
+from .. import DealModel, Queue, Seed
 
 
 class Scheduler:
 
     def schedule_seed(self, ready_seed_length, get_scheduler_lock, add_seed):
 
         inf_name = "SchedulerInterface"
-        if not issubclass_cobweb_inf(self.__class__, inf_name):
+        if not ici(self.__class__, inf_name):
             raise Exception("not have schedule function!")
 
         if self.__class__.__name__ == "Default":
             self.stop = True
             return None
 
         while not self.stop:
@@ -42,53 +43,65 @@
             seeds = get_seed(self.length)
             self.queue.push(seeds)
         log.info(f"close thread: schedule_task")
 
 
 class Spider:
 
-    def __init__(self, queue, max_retries=5):
+    def __init__(self, queue, storage, max_retries=5):
         self.spider_in_progress = Queue()
         self.max_retries = max_retries
+        self.storage = storage
         self.queue = queue
 
     def spider_task(self, stop, func, item, del_seed):
         while not stop.is_set():
+
             seed = self.queue.pop()
+
             if not seed:
                 time.sleep(3)
                 continue
+
             elif seed._retry >= self.max_retries:
                 del_seed(seed, spider_status=False)
                 continue
+
             try:
                 self.spider_in_progress.push(1, direct_insertion=True)
                 # log.info("spider seed: " + str(seed))
-                ret_count = 0
-                status = None
-                for it in func(item, seed):
-                    ret_count += 1
+                iterators = func(item, seed)
+
+                if not isgenerator(iterators):
+                    if not self.storage:
+                        del_seed(seed, spider_status=True)
+                        continue
+                    raise TypeError(f"{func.__name__} isn't a generator")
+
+                for it in iterators:
                     if getattr(it, "table_name", None):
                         store_queue = it.queue()
                         store_queue.push(
                             [seed, it.struct_data],
                             direct_insertion=True
                         )
                     elif isinstance(it, Seed):
                         self.queue.push(it)
-                    elif any(isinstance(it, t) for t in (list, tuple)):
-                        self.queue.push([s if isinstance(s, Seed) else Seed(s) for s in it])
-                    elif isinstance(it, bool):
-                        status = it
-
-                if status:
-                    del_seed(seed, spider_status=True)
-                elif not ret_count or status is False:
-                    seed._retry += 1
-                    self.queue.push(seed)
+
+                    elif isinstance(it, str) and it == DealModel.polling:
+                        self.queue.push(seed)
+                        break
+                    elif isinstance(it, str) and it == DealModel.success:
+                        del_seed(seed, spider_status=True)
+                        break
+                    elif isinstance(it, str) and it == DealModel.failure:
+                        del_seed(seed, spider_status=False)
+                        break
+                    else:
+                        raise TypeError("yield value type error!")
 
             except Exception as e:
                 seed._retry += 1
                 self.queue.push(seed)
                 log.info(f"{str(seed)} -> {str(e)}")
             finally:
                 self.spider_in_progress.pop()
@@ -96,15 +109,15 @@
 
 
 class Storer:
 
     def store_task(self, stop, last, reset_seed, del_seed):
 
         inf_name = "StorerInterface"
-        if not issubclass_cobweb_inf(self.__class__, inf_name):
+        if not ici(self.__class__, inf_name):
             return None
 
         if not getattr(self, "store", None):
             raise Exception("not have store function!")
 
         storer_name = self.__class__.__name__ + self.table
 
@@ -117,18 +130,15 @@
                     items = self.queue.pop()
                     if not items:
                         break
                     seed, data = items
                     seeds.append(seed)
                     data_list.append(data)
 
-                if data_list:
-                    if self.store(data_list):
-                        del_seed(seeds)
-                    else:
-                        reset_seed(seeds)
-                        log.info("reset seeds!")
-                    continue
+                if self.store(data_list):
+                    del_seed(seeds)
+                else:
+                    reset_seed(seeds)
 
             time.sleep(3)
 
         log.info(f"close thread: {storer_name}")
```

### Comparing `cobweb-launcher-0.1.8/cobweb/task.py` & `cobweb-launcher-0.1.9/cobweb/task.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,23 @@
+import os
+from .constant import *
 from .utils import parse_info, struct_start_seeds
 
 
+def init_task_env():
+    Setting.RESET_SCORE = int(os.getenv("RESET_SCORE", 600))
+    Setting.CHECK_LOCK_TIME = int(os.getenv("CHECK_LOCK_TIME", 30))
+    Setting.DEAL_MODEL = os.getenv("DEAL_MODEL", DealModel.failure)
+    Setting.LAUNCHER_MODEL = os.getenv("LAUNCHER_MODEL", LauncherModel.task)
+
+
 class Task:
 
     def __init__(
             self,
-            # model=None,
             seeds=None,
             project=None,
             task_name=None,
             oss_config=None,
             redis_info=None,
             storer_info=None,
             scheduler_info=None,
@@ -27,16 +35,15 @@
         :param storer_info:
         :param scheduler_info: dict(DB="", table="", size="", config="")
         :param spider_num:
         :param max_retries:
         :param storer_queue_length:
         :param scheduler_queue_length:
         """
-        # self.model = model
-
+        init_task_env()
         self.seeds = struct_start_seeds(seeds)
         self.project = project or "test"
         self.task_name = task_name or "spider"
 
         self.oss_config = oss_config
 
         self.redis_info = parse_info(redis_info)
```

### Comparing `cobweb-launcher-0.1.8/cobweb/utils.py` & `cobweb-launcher-0.1.9/cobweb/utils.py`

 * *Files identical despite different names*

### Comparing `cobweb-launcher-0.1.8/cobweb_launcher.egg-info/PKG-INFO` & `cobweb-launcher-0.1.9/cobweb_launcher.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: cobweb-launcher
-Version: 0.1.8
+Version: 0.1.9
 Summary: spider_hole
 Home-page: https://github.com/Juannie-PP/cobweb
 Author: Juannie-PP
 Author-email: 2604868278@qq.com
 License: MIT
 Keywords: cobweb-launcher, cobweb
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.19.1
+Requires-Dist: oss2>=2.18.1
+Requires-Dist: redis>=4.4.4
+Requires-Dist: aliyun-log-python-sdk
 
 # cobweb
 
 > 通用爬虫框架： 1.单机模式采集框架；2.分布式采集框架
 > 
 >  5部分
 >
```

### Comparing `cobweb-launcher-0.1.8/cobweb_launcher.egg-info/SOURCES.txt` & `cobweb-launcher-0.1.9/cobweb_launcher.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 LICENSE
 README.md
 setup.py
 cobweb/__init__.py
 cobweb/bbb.py
+cobweb/constant.py
 cobweb/decorators.py
 cobweb/interface.py
 cobweb/log.py
-cobweb/setting.py
 cobweb/task.py
 cobweb/utils.py
 cobweb/db/__init__.py
 cobweb/db/oss_db.py
 cobweb/db/redis_db.py
 cobweb/db/scheduler/__init__.py
 cobweb/db/scheduler/default.py
 cobweb/db/scheduler/textfile.py
 cobweb/db/storer/__init__.py
 cobweb/db/storer/console.py
 cobweb/db/storer/loghub.py
-cobweb/db/storer/redis.py
 cobweb/db/storer/textfile.py
-cobweb/distributed/__init__.py
-cobweb/distributed/launcher.py
-cobweb/distributed/models.py
-cobweb/single/__init__.py
-cobweb/single/launcher.py
-cobweb/single/models.py
+cobweb/equip/__init__.py
+cobweb/equip/distributed/__init__.py
+cobweb/equip/distributed/launcher.py
+cobweb/equip/distributed/models.py
+cobweb/equip/single/__init__.py
+cobweb/equip/single/launcher.py
+cobweb/equip/single/models.py
 cobweb_launcher.egg-info/PKG-INFO
 cobweb_launcher.egg-info/SOURCES.txt
 cobweb_launcher.egg-info/dependency_links.txt
 cobweb_launcher.egg-info/requires.txt
 cobweb_launcher.egg-info/top_level.txt
```

### Comparing `cobweb-launcher-0.1.8/setup.py` & `cobweb-launcher-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="cobweb-launcher",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     url="https://github.com/Juannie-PP/cobweb",
     license="MIT",
     author="Juannie-PP",
     author_email="2604868278@qq.com",
     description="spider_hole",
     long_description=long_description,
```

