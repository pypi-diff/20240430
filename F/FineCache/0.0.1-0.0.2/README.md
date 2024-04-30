# Comparing `tmp/FineCache-0.0.1.tar.gz` & `tmp/finecache-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FineCache-0.0.1.tar", last modified: Mon Feb 19 11:07:52 2024, max compression
+gzip compressed data, was "finecache-0.0.2.tar", last modified: Tue Apr 30 15:49:13 2024, max compression
```

## Comparing `FineCache-0.0.1.tar` & `finecache-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:07:52.104392 FineCache-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:07:52.104392 FineCache-0.0.1/FineCache/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-19 11:07:43.000000 FineCache-0.0.1/FineCache/CachedCall.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-19 11:07:43.000000 FineCache-0.0.1/FineCache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-02-19 11:07:43.000000 FineCache-0.0.1/FineCache/cachelib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:07:52.104392 FineCache-0.0.1/FineCache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-19 11:07:52.000000 FineCache-0.0.1/FineCache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-19 11:07:52.000000 FineCache-0.0.1/FineCache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 11:07:52.000000 FineCache-0.0.1/FineCache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-19 11:07:52.000000 FineCache-0.0.1/FineCache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-19 11:07:43.000000 FineCache-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-19 11:07:52.104392 FineCache-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-02-19 11:07:43.000000 FineCache-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 11:07:52.108392 FineCache-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-19 11:07:43.000000 FineCache-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:07:52.104392 FineCache-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-02-19 11:07:43.000000 FineCache-0.0.1/tests/test_cachelib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:49:13.090517 finecache-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:49:13.090517 finecache-0.0.2/FineCache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-30 15:49:09.000000 finecache-0.0.2/FineCache/CachedCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 15:49:09.000000 finecache-0.0.2/FineCache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-04-30 15:49:09.000000 finecache-0.0.2/FineCache/cachelib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:49:13.090517 finecache-0.0.2/FineCache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-30 15:49:13.000000 finecache-0.0.2/FineCache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-30 15:49:13.000000 finecache-0.0.2/FineCache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:49:13.000000 finecache-0.0.2/FineCache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 15:49:13.000000 finecache-0.0.2/FineCache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 15:49:09.000000 finecache-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-30 15:49:13.090517 finecache-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-30 15:49:09.000000 finecache-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:49:13.090517 finecache-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-30 15:49:09.000000 finecache-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:49:13.090517 finecache-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-30 15:49:09.000000 finecache-0.0.2/tests/test_cachelib.py
```

### Comparing `FineCache-0.0.1/FineCache/cachelib.py` & `finecache-0.0.2/FineCache/cachelib.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,265 +1,230 @@
 import inspect
 import pickle
 from dataclasses import dataclass
 from datetime import datetime
 from functools import wraps
-from typing import Tuple, Callable, Dict, Any
+from typing import Tuple, Callable, Dict, Any, List
 from zipfile import ZipFile, ZIP_DEFLATED
 
-from .CachedCall import CachedCall
+from .CachedCall import CachedCall, FilenameConfig, DefaultOptions
 import os
 import json
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
                     datefmt='%m-%d %H:%M:%S')
 logger = logging.getLogger(__name__)
 
 
-@dataclass
 class BaseCache:
     """
     缓存基础类。
     """
-    args_hash: Tuple[Callable] = None
-    kwargs_hash: Dict[str, Callable] = None
 
-    def cache(self, func: Callable) -> Callable:
-        @wraps(func)
-        def _get_result(*args, **kwargs):
-            call = CachedCall(func, args, kwargs, args_hash=self.args_hash, kwargs_hash=self.kwargs_hash)
-            if self.exists(call):
-                return self.get(call)
-            else:
-                self.set(call)
-                return call.result
+    def __init__(self, base_path=None):
+        """
+        :param base_path: 保存的文件夹，默认为当前文件夹。
+        """
+        super().__init__()
+        self.base_path = base_path if base_path else os.path.abspath(os.getcwd())
+        os.makedirs(self.base_path, exist_ok=True)
 
-        return _get_result
+    def cache(self, args_hash: List[Callable[[Any], str]] = None,
+              kwargs_hash: List[Callable[[str, Any], Tuple[str, str]]] = None,
+              config: FilenameConfig = None):
+        def _cache(func: Callable) -> Callable:
+            @wraps(func)
+            def _get_result(*args, **kwargs):
+                call = CachedCall(func, args, kwargs, args_hash=args_hash, kwargs_hash=kwargs_hash, config=config)
+                if self.exists(call):
+                    return self.get(call)
+                else:
+                    result = call.result
+                    self.set(call)
+                    return result
 
-    def exists(self, call: CachedCall):
-        pass
+            return _get_result
 
-    def get(self, call: CachedCall):
-        pass
+        return _cache
 
-    def set(self, call):
+    def exists(self, call: CachedCall) -> bool:
+        """
+        检查缓存文件是否存在
+        :param call:
+        :return:
+        """
         pass
 
-
-@dataclass
-class FilenameConfig:
-    join_args: str = ';'
-    join_dict: str = ';'
-    join_key_value: str = '-'
-    template_string: str = "{func_name}@[{args}]@{kwargs}"
-    config_path: str = None
-
-    def set_path(self, base_path=None, cfg_path=None):
-        cfg_path = cfg_path if cfg_path else '.cache_config.json'
-        # Load setting
-        if cfg_path and os.path.exists(cfg_path):
-            self.config_path = cfg_path
-        elif cfg_path and base_path and os.path.exists(os.path.join(base_path, cfg_path)):
-            self.config_path = os.path.join(base_path, cfg_path)
-        if self.config_path:
-            with open(self.config_path) as config_fp:
-                cfg = json.load(config_fp)
-            self.load(cfg)
-
-    def load(self, cfg: Dict[str, str]):
-        if 'join_args' in cfg:
-            self.join_args = cfg['join_args']
-        if 'join_dict' in cfg:
-            self.join_dict = cfg['join_dict']
-        if 'join_key_value' in cfg:
-            self.join_key_value = cfg['join_key_value']
-        if 'template_string' in cfg:
-            self.template_string = cfg['template_string']
-
-    def get_id(self, call: CachedCall):
+    def get(self, call: CachedCall):
         """
-        获取缓存的文件名
+        从缓存文件获取结果
         :param call:
         :return:
         """
-        arg_list = [call.get_args_hash(i) if PickleCache.is_picklable(a) else 'None' for i, a in enumerate(call.args)]
-        kwarg_list = {k: call.get_kwargs_hash(k) if PickleCache.is_picklable(v) else 'None' for k, v in
-                      call.kwargs.items()}
-        args_string = self.join_args.join(arg_list)
-        kwargs_string = self.join_dict.join([k + self.join_key_value + v for k, v in kwarg_list.items()])
-        return self.template_string.format(func_name=call.func.__name__, args=args_string, kwargs=kwargs_string)
-
+        pass
 
-class PickleCache(BaseCache):
-    def __init__(self, base_path=None, cfg_path=None, args_hash=None, kwargs_hash=None):
+    def set(self, call) -> None:
         """
-
-        :param base_path: 保存的文件夹，默认为当前文件夹。
-        :param cfg_path: 配置文件的路径，主要用于指定保存文件的路径格式。
+        将运行结果缓存到缓存文件中
+        :param call:
+        :return:
         """
-        super().__init__(args_hash, kwargs_hash)
-        self.base_path = base_path if base_path else os.path.abspath(os.getcwd())
-        os.makedirs(self.base_path, exist_ok=True)
-        self.config = FilenameConfig()
-        self.config.set_path(base_path, cfg_path)
+        pass
 
+
+class PickleCache(BaseCache):
     @staticmethod
     def is_picklable(obj: Any) -> bool:
         """
         判断是否可以被pickle缓存
         :param obj:
         :return:
         """
         try:
             pickle.dumps(obj)
             return True
         except:
+            logger.info(f'parameters: {obj} could not be pickle')
             return False
 
     def exists(self, call: CachedCall):
-        filename = os.path.join(self.base_path, self.config.get_id(call) + '.pk')
+        filename = os.path.join(self.base_path, call.filename + '.pk')
         return os.path.exists(filename) and os.path.isfile(filename)
 
     def get(self, call: CachedCall) -> Any:
-        filename = os.path.join(self.base_path, self.config.get_id(call) + '.pk')
+        filename = os.path.join(self.base_path, call.filename + '.pk')
         with open(filename, 'rb') as fp:
             data = pickle.load(fp)
         assert call.func.__qualname__ == data['func']
         logger.debug(data)
 
-        n_call = CachedCall(data['func'], data['args'], data['kwargs'], result=data['result'],
-                            args_hash=self.args_hash, kwargs_hash=self.kwargs_hash)
-        return n_call.result
+        # 可以尝试获取更多的数据内容，但是可以直接返回 'result'
+        # n_call = CachedCall(data['func'], data['args'], data['kwargs'], result=data['result'])
+        return data['result']
 
     @staticmethod
     def _construct_content(call):
         """
         构造函数调用缓存的内容
         :param call:
         :return:
         """
         args = [a if PickleCache.is_picklable(a) else None for a in call.args]
         kwargs = {k: v if PickleCache.is_picklable(v) else None for k, v in call.kwargs.items()}
-        result = call.run()
+        result = call.result
         if not PickleCache.is_picklable(result):
+            logger.error(f"{result} isn't picklable...")
+            logger.error(f"{call.func.__qualname__}, args: {args}, kwargs: {kwargs}")
             raise pickle.PickleError("not a picklable result...")
 
         return {
             'func': call.func.__qualname__,
             'args': args,
             'kwargs': kwargs,
             'result': result,
+            'module': call.func.__module__,
+            'runtime': str(datetime.now())
         }
 
     def set(self, call: CachedCall):
-        filename = os.path.join(self.base_path, self.config.get_id(call) + '.pk')
+        filename = os.path.join(self.base_path, call.filename + '.pk')
         content = self._construct_content(call)
         logger.debug(content)
         with open(filename, 'wb') as fp:
             pickle.dump(content, fp)
 
 
-@dataclass
-class VersionConfig:
-    version: int = 1
-
-    def increment(self):
-        self.version += 1
-
-    def save_to_file(self, filename):
-        with open(filename, 'wb') as f:
-            pickle.dump(self.version, f)
-
-    @classmethod
-    def load_from_file(cls, filename):
-        with open(filename, 'rb') as f:
-            version = pickle.load(f)
-        new_instance = cls(version)
-        return new_instance
-
-
 class HistoryCache(BaseCache):
     """
     这个类只保存函数代码和运行结果，内容可以直接查看。
     """
 
-    def __init__(self, base_path=None, tracking_files=None, cfg_path=None, args_hash=None, kwargs_hash=None):
-        super().__init__(args_hash, kwargs_hash)
-        self.base_path = base_path if base_path else os.path.abspath(os.getcwd())
-        os.makedirs(self.base_path, exist_ok=True)
-        self.config = FilenameConfig()
-        self.config.set_path(base_path, cfg_path)
+    def __init__(self, base_path=None, tracking_files: List[str] = None, cache_result: bool = True):
+        super().__init__(base_path)
+        self.cache_result = cache_result
         self.tracking_files = tracking_files if tracking_files else []
-        self.filename_template = 'v{ver}.{suffix}'
-
-    def cache(self, func: Callable) -> Callable:
-        @wraps(func)
-        def _get_result(*args, **kwargs):
-            call = CachedCall(func, args, kwargs, args_hash=self.args_hash, kwargs_hash=self.kwargs_hash)
-            self.set(call)
-            return call.result
-
-        return _get_result
+        self.code_filename = 'code.py'  # 当前版本代码文件
+        self.result_filename = 'result.pk'  # 当前版本结果与参数等的保存文件 （对于不支持pickle的参数，将会跳过存储。对于不支持pickle 的函数运行结果，将会报错。）
+        self.tracking_filename = 'tracking.zip'  # 所有tracking_files的打包
 
     def exists(self, call: CachedCall):
-        path = os.path.join(self.base_path, self.config.get_id(call))
-        return os.path.exists(path) and os.path.isdir(path)
+        path = os.path.join(self.base_path, call.filename)
+        if not (os.path.exists(path) and os.path.isdir(path)):
+            return False
+        # get the latest version code
+        version_path = os.path.join(path, '.version.txt')
+        if not os.path.exists(version_path):
+            return False
+
+        with open(version_path, 'r') as f:
+            latest_version = int(f.read())
+        latest_version_folder = os.path.join(path, str(latest_version))
+        code_filename = os.path.join(latest_version_folder, self.code_filename)
+        with open(code_filename, encoding='utf-8') as fp:
+            lines = fp.readlines()
+            old_code = ''.join(lines[1:])
+        return inspect.getsource(call.func) == old_code
 
     def set(self, call):
-        path = os.path.join(self.base_path, self.config.get_id(call))
+        path = os.path.join(self.base_path, call.filename)
         os.makedirs(path, exist_ok=True)
         version_path = os.path.join(path, '.version.txt')
+        if os.path.exists(version_path):
+            with open(version_path, 'r') as f:
+                latest_version = int(f.read())
+        else:
+            latest_version = 0
+
+        now_version = latest_version + 1
+        now_version_folder = os.path.join(path, str(now_version))
+        os.makedirs(now_version_folder, exist_ok=True)
 
-        ver_conf = VersionConfig() if not os.path.exists(version_path) else VersionConfig.load_from_file(version_path)
-
-        old_filename = self.filename_template.format(ver=ver_conf.version, suffix='py')
-        old_path = os.path.join(path, old_filename)
-        # 若存在旧文件，则存在新文件，否则直接存在旧文件
-        if os.path.exists(old_path):
-            with open(old_path, encoding='utf-8') as fp:
-                lines = fp.readlines()
-                old_code = ''.join(lines[1:])
-            # 若现有代码与历史代码不一致
-            if inspect.getsource(call.func) != old_code:
-                # 保存结果到新的版本
-                ver_conf.increment()
-            else:
-                # 否则无需保存结果，只照常运行即可
-                call.run()
-                return
-        ver_conf.save_to_file(version_path)
-
-        # Save function code
-        func_code_filename = os.path.join(path, self.filename_template.format(ver=ver_conf.version, suffix='py'))
+        # 保存当前函数代码
+        func_code_filename = os.path.join(now_version_folder, self.code_filename)
         src_filename = inspect.getsourcefile(call.func)
         lines, line_num = inspect.getsourcelines(call.func)
         with open(func_code_filename, 'w', encoding='utf-8') as fp:
-            fp.write(f'# {src_filename} L{line_num} V{ver_conf.version}\n')
+            fp.write(f'# {src_filename} L{line_num} V{now_version}\n')
             fp.writelines(lines)
 
-        pickle_filename = os.path.join(path, self.filename_template.format(ver=ver_conf.version, suffix='pk'))
+        # 保存当前函数运行结果
+        pickle_filename = os.path.join(now_version_folder, self.result_filename)
         content = PickleCache._construct_content(call)
         content.update({
-            'module': call.func.__module__,
-            'version': ver_conf.version,
-            'runtime': str(datetime.now()),
+            'version': now_version
         })
         logger.debug(content)
         with open(pickle_filename, 'wb') as fp:
             pickle.dump(content, fp)
 
         if len(self.tracking_files) != 0:
-            zip_filename = os.path.join(path, self.filename_template.format(ver=ver_conf.version, suffix='zip'))
+            zip_filename = os.path.join(now_version_folder, self.tracking_filename)
             with ZipFile(zip_filename, 'w') as zip_file:
                 for f in self.tracking_files:
                     zip_file.write(f, compress_type=ZIP_DEFLATED)
 
-    def explore(self, func, args=(), kwargs=None, key=lambda x: x):
-        if kwargs is None:
-            kwargs = {}
-        call = CachedCall(func, args, kwargs)
-        path = os.path.join(self.base_path, self.config.get_id(call))
-        if not os.path.exists(path):
-            raise Exception(f"Could not explore: {func.__qualname__}(args={args}, kwargs={kwargs}), not exists {path}")
-        return [key(os.path.join(path, f[:-5])) for f in os.listdir(path) if f.endswith('json')]
+        # 重新写入 Latest version 文件
+        latest_version += 1
+        with open(version_path, 'w') as f:
+            f.write(str(latest_version))
+
+    def get(self, call: CachedCall) -> Any:
+        if self.cache_result:
+            path = os.path.join(self.base_path, call.filename)
+            version_path = os.path.join(path, '.version.txt')
+            with open(version_path, 'r') as f:
+                latest_version = int(f.read())
+            latest_version_folder = os.path.join(path, str(latest_version))
+            filename = os.path.join(latest_version_folder, self.result_filename)
+            with open(filename, 'rb') as fp:
+                data = pickle.load(fp)
+            assert call.func.__qualname__ == data['func']
+            logger.debug(data)
+
+            # 可以尝试获取更多的数据内容，但是可以直接返回 'result'
+            # n_call = CachedCall(data['func'], data['args'], data['kwargs'], result=data['result'])
+            return data['result']
+        else:
+            # 不读取Cache结果，而是直接进行计算
+            return call.result
```

### Comparing `FineCache-0.0.1/LICENSE` & `finecache-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FineCache-0.0.1/setup.py` & `finecache-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="FineCache",
-  version="0.0.1",
+  version="0.0.2",
   author="Ciaran Chen",
   author_email="ciaranchen@qq.com",
   description="A function cache for fine-tuning",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ciaranchen/FineCache",
   packages=setuptools.find_packages(),
```

### Comparing `FineCache-0.0.1/tests/test_cachelib.py` & `finecache-0.0.2/tests/test_cachelib.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,40 +14,44 @@
     # print(a1, a2, k1, k2)
     # print(a1, "+ 1 =", a1 + 1)
     return a3, a4, kr1, kr2
 
 
 class TestPickleCache(unittest.TestCase):
     def setUp(self) -> None:
-        # Clear folders...
-        rmtree('.p_cache')
         self.pc = PickleCache('.p_cache')
 
+    def tearDown(self):
+        super().tearDown()
+        # Clear folders...
+        if os.path.exists('.p_cache'):
+            rmtree('.p_cache')
+
     def test_wrapped(self):
-        wrapped = self.pc.cache(func)
+        wrapped = self.pc.cache()(func)
         self.assertEqual(wrapped.__qualname__, func.__qualname__)
         self.assertEqual(wrapped.__doc__, func.__doc__)
 
     def test_pickle_cache(self):
         args = (3,)
         kwargs = {'a2': 4, 'k1': "v3"}
-        wrapped = self.pc.cache(func)
+        wrapped = self.pc.cache()(func)
         self.assertEqual(func(*args, **kwargs), wrapped(*args, **kwargs))
         self.assertEqual(func(*args, **kwargs), wrapped(*args, **kwargs))
 
     def test_unpicklable_args(self):
         def _test_unpicklable(a1, a2, k1, k2):
             # print(a1, a2, k1, k2)
             return a1, k1
 
         args = (3, lambda x: x + 2)
         kwargs = {'k1': 4, 'k2': lambda x: x + 3}
         _test_unpicklable(*args, **kwargs)
 
-        wrapped = self.pc.cache(_test_unpicklable)
+        wrapped = self.pc.cache()(_test_unpicklable)
         wrapped(*args, **kwargs)
 
         filepaths = [file for file in os.listdir('.p_cache') if file.startswith(_test_unpicklable.__name__ + '@')]
         self.assertEqual(len(filepaths), 1)
         with open(os.path.join('.p_cache', filepaths[0]), 'rb') as fp:
             data = pickle.load(fp)
         self.assertEqual(data['func'], _test_unpicklable.__qualname__)
@@ -62,69 +66,76 @@
     def test_unpicklable_different_action(self):
         def _test_lambda(a1, func1):
             return func1(a1)
 
         args = (3, lambda x: x)
         res0 = _test_lambda(*args)
         self.assertEqual(res0, 3)
-        wrapped = self.pc.cache(_test_lambda)
+        wrapped = self.pc.cache()(_test_lambda)
         res1 = wrapped(*args)
         self.assertEqual(res1, 3)
 
         args2 = (3, lambda x: x + 1)
-        # 此处会加载同样的文件，但是不会以func1的值重新调用，而是直接使用上一个结果。
+        # 此处不会产生相同结果
         res2 = wrapped(*args2)
-        self.assertEqual(res2, 3)
-
-        args3 = (4, lambda x: x)
-        # 这里完全实现新的函数，所以会直接以args3为参数重新计算。
-        res3 = wrapped(*args3)
-        self.assertEqual(res3, 4)
+        self.assertEqual(res2, 4)
 
     def test_not_picklable_result(self):
         def _test_unpicklable_result():
             return lambda x: 0
 
-        wrapped = self.pc.cache(_test_unpicklable_result)
+        wrapped = self.pc.cache()(_test_unpicklable_result)
         try:
             wrapped()
         except pickle.PickleError as e:
             pass
 
+    def test_self_defined_hash(self):
+        def test_func(a1, a2):
+            return a1, a2
+
+        wrapped = self.pc.cache(args_hash=[lambda a1: 'x', lambda a2: 'y'])(test_func)
+        wrapped('a1', 'a2')
+        self.assertTrue(os.path.exists(os.path.join('.p_cache', "test_func@['x';'y']@.pk")))
+
 
 class TestHistoryCache(unittest.TestCase):
-    def setUp(self) -> None:
+    def tearDown(self):
+        super().tearDown()
         # Clear folders...
-        rmtree('.h_cache')
+        if os.path.exists('.h_cache'):
+            rmtree('.h_cache')
+
+    def setUp(self) -> None:
         self.hc = HistoryCache('.h_cache')
 
         def _test_func_history(a1, a2):
             """
             test function version 1
             :param a1:
             :param a2:
             :return:
             """
             return a1
 
-        self.wrapped1 = self.hc.cache(_test_func_history)
+        self.wrapped1 = self.hc.cache()(_test_func_history)
 
         def _test_func_history(a1, a2):
             """
             test function version 2
             :param a1:
             :param a2:
             :return:
             """
             return a1 + 1
 
-        self.wrapped2 = self.hc.cache(_test_func_history)
+        self.wrapped2 = self.hc.cache()(_test_func_history)
 
     def test_wrapped(self):
-        wrapped = self.hc.cache(func)
+        wrapped = self.hc.cache()(func)
         self.assertEqual(wrapped.__qualname__, func.__qualname__)
         self.assertEqual(wrapped.__doc__, func.__doc__)
 
     def test_history_cache(self):
         args = (1, 2)
         self.assertEqual(self.wrapped1(*args) + 1, self.wrapped2(*args))
```

