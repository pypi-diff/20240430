# Comparing `tmp/recoverable_async_task-0.1.1.tar.gz` & `tmp/recoverable_async_task-0.1.3.tar.gz`

## Comparing `recoverable_async_task-0.1.1.tar` & `recoverable_async_task-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10600 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.1/recoverable_async_task.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.1/.gitignore
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.1/README.md
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10600 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.3/recoverable_async_task.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.3/.gitignore
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.3/README.md
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.3/PKG-INFO
```

### Comparing `recoverable_async_task-0.1.1/recoverable_async_task.py` & `recoverable_async_task-0.1.3/recoverable_async_task.py`

 * *Files identical despite different names*

### Comparing `recoverable_async_task-0.1.1/README.md` & `recoverable_async_task-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -8,18 +8,52 @@
 
 To install the library, use the following command:
 
 ```bash
 pip install recoverable-async-task
 ```
 
-The `example.py` file provides a simple illustration of how to utilize the `RecoverableAsyncTask` library to manage concurrent tasks and enable checkpointing and resumption:
+The following is a simple illustration of how to utilize the `RecoverableAsyncTask` library to manage concurrent tasks and enable checkpointing and resumption:
 
-```bash
-python3 example.py
+```python
+import asyncio
+
+from recoverable_async_task import RecoverableAsyncTask
+
+
+async def main():
+    async def task(id: int | str):
+        import random
+
+        await asyncio.sleep(0.1)
+
+        if random.randint(1, 2) == 1:
+            raise Exception(f"Task {id=} failed!")
+
+        return {"id": id, "data": f"Task {id=} finished!"}
+
+    # 创建 RecoverableAsyncTask 实例
+    re_async_task = RecoverableAsyncTask(
+        task,
+        max_workers=10,
+        max_qps=10,
+        retry_n=3,
+        checkpoint_path_name="save-dir/my-example-task",
+    )
+
+    # 推送任务以并发处理
+    for i in range(100):
+        re_async_task.push(i)
+
+    # 收集并打印结果
+    async for result in re_async_task.collect_results():
+        print(result)
+
+
+asyncio.run(main())
 ```
 
 You may notice that even with `retry_n=3` set, some tasks may still fail due to random issues. In such cases, you can simply execute the tasks again, and they will automatically read the checkpoint file and resume from where they were interrupted. You can repeat this process manually or programmatically until all tasks are successfully completed.
 
 ## Contributing Guidelines
 
 If you wish to contribute to the `recoverable-async-task` library, please follow the setup instructions below to prepare your development environment:
```

### Comparing `recoverable_async_task-0.1.1/pyproject.toml` & `recoverable_async_task-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `recoverable_async_task-0.1.1/PKG-INFO` & `recoverable_async_task-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: recoverable-async-task
-Version: 0.1.1
+Version: 0.1.3
 Summary: `recoverable-async-task` is a Python library that streamlines the handling of asynchronous tasks through its `RecoverableAsyncTask` class, with the added benefit of **supporting task checkpointing and resumption**. This feature ensures that tasks can pick up from where they left off in the event of unexpected failures.
 Project-URL: Homepage, https://github.com/Haskely/recoverable-async-task
 Project-URL: Bug Reports, https://github.com/Haskely/recoverable-async-task/issues
 Project-URL: Source, https://github.com/Haskely/recoverable-async-task
 Author-email: Haskely <Haskely@live.com>
 Requires-Python: >=3.8
 Requires-Dist: loguru>=0.7.2
@@ -21,18 +21,52 @@
 
 To install the library, use the following command:
 
 ```bash
 pip install recoverable-async-task
 ```
 
-The `example.py` file provides a simple illustration of how to utilize the `RecoverableAsyncTask` library to manage concurrent tasks and enable checkpointing and resumption:
+The following is a simple illustration of how to utilize the `RecoverableAsyncTask` library to manage concurrent tasks and enable checkpointing and resumption:
 
-```bash
-python3 example.py
+```python
+import asyncio
+
+from recoverable_async_task import RecoverableAsyncTask
+
+
+async def main():
+    async def task(id: int | str):
+        import random
+
+        await asyncio.sleep(0.1)
+
+        if random.randint(1, 2) == 1:
+            raise Exception(f"Task {id=} failed!")
+
+        return {"id": id, "data": f"Task {id=} finished!"}
+
+    # 创建 RecoverableAsyncTask 实例
+    re_async_task = RecoverableAsyncTask(
+        task,
+        max_workers=10,
+        max_qps=10,
+        retry_n=3,
+        checkpoint_path_name="save-dir/my-example-task",
+    )
+
+    # 推送任务以并发处理
+    for i in range(100):
+        re_async_task.push(i)
+
+    # 收集并打印结果
+    async for result in re_async_task.collect_results():
+        print(result)
+
+
+asyncio.run(main())
 ```
 
 You may notice that even with `retry_n=3` set, some tasks may still fail due to random issues. In such cases, you can simply execute the tasks again, and they will automatically read the checkpoint file and resume from where they were interrupted. You can repeat this process manually or programmatically until all tasks are successfully completed.
 
 ## Contributing Guidelines
 
 If you wish to contribute to the `recoverable-async-task` library, please follow the setup instructions below to prepare your development environment:
```

