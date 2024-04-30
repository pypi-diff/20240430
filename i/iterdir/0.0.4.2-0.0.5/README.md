# Comparing `tmp/iterdir-0.0.4.2.tar.gz` & `tmp/iterdir-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterdir-0.0.4.2.tar", max compression
+gzip compressed data, was "iterdir-0.0.5.tar", max compression
```

## Comparing `iterdir-0.0.4.2.tar` & `iterdir-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.4.2/LICENSE
--rwxr-xr-x   0        0        0    10835 2024-04-26 15:41:56.804325 iterdir-0.0.4.2/iterdir/__init__.py
--rwxr-xr-x   0        0        0     9620 2024-04-26 15:42:48.292258 iterdir-0.0.4.2/iterdir/__main__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iterdir-0.0.4.2/iterdir/py.typed
--rw-r--r--   0        0        0     1115 2024-04-26 15:43:01.027269 iterdir-0.0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3704 2024-04-19 12:19:41.653359 iterdir-0.0.4.2/readme.md
--rw-r--r--   0        0        0     4801 1970-01-01 00:00:00.000000 iterdir-0.0.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 iterdir-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0     9421 2024-04-30 05:54:47.336601 iterdir-0.0.5/iterdir/__init__.py
+-rwxr-xr-x   0        0        0    10105 2024-04-30 06:01:32.882677 iterdir-0.0.5/iterdir/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 iterdir-0.0.5/iterdir/py.typed
+-rw-r--r--   0        0        0     1135 2024-04-30 06:02:20.639422 iterdir-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5348 2024-04-30 06:04:55.686039 iterdir-0.0.5/readme.md
+-rw-r--r--   0        0        0     6465 1970-01-01 00:00:00.000000 iterdir-0.0.5/PKG-INFO
```

### Comparing `iterdir-0.0.4.2/LICENSE` & `iterdir-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iterdir-0.0.4.2/iterdir/__init__.py` & `iterdir-0.0.5/iterdir/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 4)
-__all__ = ["DirEntry", "iterdir", "statsdir"]
+__version__ = (0, 0, 5)
+__all__ = ["DirEntry", "iterdir"]
 
 from collections import deque
 from collections.abc import Callable, Iterable, Iterator
 from os import (
     fspath, listdir, lstat, scandir, stat, stat_result, 
     DirEntry as _DirEntry, PathLike, 
 )
@@ -84,15 +84,14 @@
     /, 
     is_dir: Callable[[PathType], bool], 
     iter_dir: Callable[[PathType], Iterable[PathType]], 
     min_depth: int = 1, 
     max_depth: int = 1, 
     predicate: Optional[Callable[[PathType], Optional[bool]]] = None, 
     onerror: bool | Callable[[OSError], bool] = False, 
-    follow_symlinks: bool = False, 
 ) -> Iterator[PathType]:
     dq: deque[tuple[int, PathType]] = deque()
     push, pop = dq.append, dq.popleft
     push((0, top))
     while dq:
         depth, path = pop()
         if min_depth <= 0:
@@ -127,15 +126,14 @@
     is_dir: Callable[[PathType], bool], 
     iter_dir: Callable[[PathType], Iterable[PathType]], 
     topdown: bool = True, 
     min_depth: int = 1, 
     max_depth: int = 1, 
     predicate: Optional[Callable[[PathType], Optional[bool]]] = None, 
     onerror: bool | Callable[[OSError], bool] = False, 
-    follow_symlinks: bool = False, 
 ) -> Iterator[PathType]:
     if not max_depth:
         return
     global_yield_me = True
     if min_depth > 1:
         global_yield_me = False
         min_depth -= 1
@@ -166,15 +164,14 @@
                     is_dir=is_dir, 
                     iter_dir=iter_dir, 
                     topdown=topdown, 
                     min_depth=min_depth, 
                     max_depth=max_depth, 
                     predicate=predicate, 
                     onerror=onerror, 
-                    follow_symlinks=follow_symlinks, 
                 )
             if yield_me and not topdown:
                 yield path
     except OSError as e:
         if callable(onerror):
             onerror(e)
         elif onerror:
@@ -289,60 +286,7 @@
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
             predicate=predicate, 
             onerror=onerror, 
         )
 
-
-def format_bytes(
-    n: int, 
-    /, 
-    unit: str = "", 
-    precision: int = 6, 
-) -> str:
-    "scale bytes to its proper byte format"
-    if unit == "B" or not unit and n < 1024:
-        return f"{n} B"
-    b = 1
-    b2 = 1024
-    for u in ["K", "M", "G", "T", "P", "E", "Z", "Y"]:
-        b, b2 = b2, b2 << 10
-        if u == unit if unit else n < b2:
-            break
-    return f"%.{precision}f {u}B" % (n / b)
-
-
-def statsdir(
-    top=None, 
-    /, 
-    min_depth: int = 0, 
-    max_depth: int = -1, 
-    predicate: Optional[Callable[..., Optional[bool]]] = None, 
-    onerror: bool | Callable[[OSError], bool] = False, 
-    follow_symlinks: bool = False, 
-) -> dict:
-    files = 0
-    dirs = 0
-    size = 0
-    for path in iterdir(
-        top, 
-        min_depth=min_depth, 
-        max_depth=max_depth, 
-        predicate=predicate, 
-        onerror=onerror, 
-        follow_symlinks=follow_symlinks, 
-    ):
-        if isdir(path) and not islink(path):
-            dirs += 1
-        else:
-            files += 1
-            size += lstat(path).st_size
-    return {
-        "path": abspath(DirEntry(top or ".")), 
-        "total": files + dirs, 
-        "files": files, 
-        "dirs": dirs, 
-        "size": size, 
-        "fmt_size": format_bytes(size)
-    }
-
```

### Comparing `iterdir-0.0.4.2/iterdir/__main__.py` & `iterdir-0.0.5/iterdir/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,190 +1,265 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
+__doc__ = "目录树信息遍历导出"
 
 from argparse import ArgumentParser, RawTextHelpFormatter
+from hashlib import algorithms_available
 
-parser = ArgumentParser(description="目录树工具集", formatter_class=RawTextHelpFormatter)
-parser.set_defaults(func=None)
+KEYS = ["inode", "name", "path", "relpath", "isdir", "islink", "stat"]
 
-subparsers = parser.add_subparsers()
+parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
 
-KEYS = ("inode", "name", "path", "relpath", "isdir", "islink", "stat")
-
-parser_iter = subparsers.add_parser("iter", description="目录树信息遍历导出")
-
-parser_iter.add_argument("path", nargs="?", default="", help="文件夹路径，默认为当前工作目录")
-parser_iter.add_argument("-s", "--select", help="提供一个表达式（会注入一个变量 path，类型是 pathlib.Path），用于对路径进行筛选")
-parser_iter.add_argument("-m", "--min-depth", default=0, type=int, help="最小深度，默认值 0，小于 0 时不限")
-parser_iter.add_argument("-M", "--max-depth", default=-1, type=int, help="最大深度，默认值 -1，小于 0 时不限")
-parser_iter.add_argument("-v", "--version", action="store_true", help="输出版本号")
-
-parser_iter.add_argument("-k", "--keys", nargs="*", choices=KEYS, help=f"选择输出的 key，默认输出所有可选值")
-parser_iter.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""\
+parser.add_argument("path", nargs="?", default="", help="文件夹路径，默认为当前工作目录")
+parser.add_argument("-m", "--min-depth", default=0, type=int, help="最小深度，默认值 0，小于 0 时不限")
+parser.add_argument("-M", "--max-depth", default=-1, type=int, help="最大深度，默认值 -1，小于 0 时不限")
+parser.add_argument("-k", "--keys", choices=KEYS, nargs="*", help=f"选择输出的 key，默认输出所有可选值")
+parser.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""\
 输出类型，默认为 log
 - log   每行输出一条数据，每条数据输出为一个 json 的 object
 - json  输出一个 json 的 list，每条数据输出为一个 json 的 object
 - csv   输出一个 csv，第 1 行为表头，以后每行输出一条数据
 """)
-parser_iter.add_argument("-o", "--output-file", help="保存到文件，此时命令行会输出进度条")
-parser_iter.add_argument("-dfs", "--depth-first", action="store_true", help="使用深度优先搜索，否则使用广度优先")
-parser_iter.add_argument("-fl", "--follow-symlinks", action="store_true", help="是否跟进符号连接（如果为否，则会把符号链接视为文件，即使它指向目录）")
-
-def main_iter(args):
-    from iterdir import __version__, iterdir, DirEntry
-
-    if args.version:
-        print(".".join(map(str, __version__)))
-        raise SystemExit(0)
-
-    from collections.abc import Callable, Iterator
-    from os import fsdecode, lstat, stat, stat_result, PathLike
-    from os.path import abspath, isdir, islink, relpath
-    from operator import attrgetter
-    from pathlib import Path
-    from sys import stdout
-    from typing import Optional
-
-    STAT_FIELDS = tuple(
-        f for f in dir(stat_result) 
-        if f.startswith("st_")
-    )
+parser.add_argument("-d", "--dump", default="", help="""\
+(优先级高于 -k/--keys、-hs/--hashes、-t/--output-type) 调用以导出数据，如果有返回值则再行输出，尾部会添加一个 b'\n'。
+如果结果 result 是
+    - None，跳过
+    - bytes，输出
+    - 其它，先调用 `bytes(str(result), 'utf-8')`，再输出
+提供一个表达式（会注入一个变量 path，类型是 pathlib.Path）或函数（会传入一个参数，类型是 pathlib.Path）    
+""")
+parser.add_argument("-de", "--dump-exec", action="store_true", help="对 -d/--dump 传入的代码用 exec 运行，其中必须存在名为 dump 的函数。否则，视为表达式或 lambda 函数")
+parser.add_argument("-s", "--select", help="对路径进行筛选，提供一个表达式（会注入一个变量 path，类型是 pathlib.Path）或函数（会传入一个参数，类型是 pathlib.Path）")
+parser.add_argument("-se", "--select-exec", action="store_true", help="对 -s/--select 传入的代码用 exec 运行，其中必须存在名为 select 的函数。否则，视为表达式或 lambda 函数")
+parser.add_argument("-o", "--output-file", help="保存到文件，此时命令行会输出进度条")
+parser.add_argument("-hs", "--hashes", choices=(*algorithms_available, "crc32"), nargs="*", help="计算文件的哈希值，可以选择多个算法")
+parser.add_argument("-dfs", "--depth-first", action="store_true", help="使用深度优先搜索，否则使用广度优先")
+parser.add_argument("-fl", "--follow-symlinks", action="store_true", help="跟进符号连接，否则会把符号链接视为文件，即使它指向目录")
+parser.add_argument("-v", "--version", action="store_true", help="输出版本号")
 
-    def stat_to_dict(
-        path: None | bytes | str | PathLike = None, 
-        /, 
-        follow_symlinks: bool = False, 
-    ) -> Optional[dict]:
-        getstat: Callable[[bytes | str | PathLike], stat_result]
-        if follow_symlinks:
-            getstat = stat
-        else:
-            getstat = lstat
-        try:
-            return dict(zip(
-                STAT_FIELDS, 
-                attrgetter(*STAT_FIELDS)(getstat(path or ".")), 
-            ))
-        except OSError:
-            return None
-
-    select = args.select
-    predicate: Optional[Callable[[DirEntry], Optional[bool]]]
-    if select:
-        if select.startswith("lambda "):
-            pred = eval(select)
-        else:
-            pred = eval("lambda path:" + select)
-        predicate = lambda e: pred(Path(fsdecode(e)))
+args = parser.parse_args()
+
+if args.version:
+    from iterdir import __version__
+    print(".".join(map(str, __version__)))
+    raise SystemExit(0)
+
+from binascii import crc32
+from collections.abc import Callable, Iterator, Sequence
+from functools import partial
+from hashlib import new as hashnew
+from os import fsdecode, lstat, stat, stat_result, PathLike
+from os.path import abspath, isdir, islink, relpath
+from operator import attrgetter
+from pathlib import Path
+from sys import stdout
+from textwrap import dedent
+from typing import cast, Any, Optional
+
+from iterdir import iterdir, DirEntry
+
+STAT_FIELDS = tuple(
+    f for f in dir(stat_result) 
+    if f.startswith("st_")
+)
+
+def stat_to_dict(
+    path: None | bytes | str | PathLike = None, 
+    /, 
+    follow_symlinks: bool = False, 
+) -> Optional[dict]:
+    getstat: Callable[[bytes | str | PathLike], stat_result]
+    if follow_symlinks:
+        getstat = stat
     else:
-        predicate = None
+        getstat = lstat
+    try:
+        return dict(zip(
+            STAT_FIELDS, 
+            attrgetter(*STAT_FIELDS)(getstat(path or ".")), 
+        ))
+    except OSError:
+        return None
+
+def file_multi_hashes(
+    path: bytes | str | PathLike, 
+    hashes: Sequence[str], 
+) -> Optional[dict[str, str]]:
+    try:
+        file = open(path, "rb", buffering=0)
+    except OSError:
+        return None
+    cache: dict[str, Any] = {alg: 0 if alg == "crc32" else hashnew(alg) for alg in hashes}
+    updates = tuple(
+        (lambda data: 
+            cache.__setitem__("crc32", crc32(data, cast(int, cache["crc32"])))
+        ) if alg == "crc32" else val.update 
+        for alg, val in cache.items()
+    )
+    readinto = file.readinto
+    buf = bytearray(1 << 16) # 64 KB
+    view = memoryview(buf)
+    while (size := readinto(buf)):
+        for update in updates:
+            update(view[:size])
+    return {alg: format(val, "x") if alg == "crc32" else val.hexdigest() for alg, val in cache.items()}
+
+predicate: Optional[Callable[[DirEntry], Optional[bool]]] = None
+select_code = dedent(args.select).strip()
+if select_code:
+    ns = {"re": __import__("re")}
+    if args.select_exec:
+        exec(select_code, ns)
+        select = ns.get("select")
+    elif select_code.startswith("lambda "):
+        select = eval(select_code, ns)
+    else:
+        select = eval("lambda path:" + select_code, ns)
+    if callable(select):
+        predicate = lambda e: select(Path(fsdecode(e)))
+
+dumps: Optional[Callable[[DirEntry], Any]] = None
+dump_code = dedent(args.dump).strip()
+if dump_code:
+    ns = {}
+    if args.dump_exec:
+        exec(dump_code, ns)
+        dump = ns.get("dump")
+    elif dump_code.startswith("lambda "):
+        dump = eval(dump_code, ns)
+    else:
+        dump = eval("lambda path:" + dump_code, ns)
+    if callable(dump):
+        dumps = lambda e: dump(Path(fsdecode(e)))
+
+path = args.path
+path_it: Iterator[DirEntry] = iterdir(
+    DirEntry(path), 
+    topdown=True if args.depth_first else None, 
+    min_depth=args.min_depth, 
+    max_depth=args.max_depth, 
+    predicate=predicate, 
+    follow_symlinks=args.follow_symlinks, 
+)
+
+output_file = args.output_file
+if output_file:
+    from collections import deque
+    from time import perf_counter
+
+    def format_time(t):
+        m, s = divmod(t, 60)
+        if m < 60:
+            return f"{m:02.0f}:{s:09.06f}"
+        h, m = divmod(m, 60)
+        if h < 24:
+            return f"{h:02.0f}:{m:02.0f}:{s:09.06f}"
+        d, h = divmod(h, 60)
+        return f"{d}d{h:02.0f}:{m:02.0f}:{s:09.06f}"
+
+    def progress(it):
+        write = stdout.buffer.raw.write # type: ignore
+        dq: deque[tuple[int, float]] = deque(maxlen=10*60)
+        push = dq.append
+        total = 0
+        ndirs = 0
+        nfiles = 0
+        start_t = last_t = perf_counter()
+        write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles}".encode())
+        push((total, start_t))
+        for p in it:
+            total += 1
+            if p.is_dir():
+                ndirs += 1
+            else:
+                nfiles += 1
+            cur_t = perf_counter()
+            if cur_t - last_t > 0.1:
+                speed = (total - dq[0][0]) / (cur_t - dq[0][1])
+                write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles} | 🕙 {format_time(cur_t-start_t)} | 🚀 {speed:.3f} it/s".encode())
+                push((total, cur_t))
+                last_t = cur_t
+            yield p
+        cur_t = perf_counter()
+        speed = total / (cur_t - start_t)
+        write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles} | 🕙 {format_time(cur_t-start_t)} | 🚀 {speed:.3f} it/s".encode())
+    file = open(output_file, "w")
+    path_it = iter(progress(path_it))
+    write = file.buffer.write
+else:
+    file = stdout # type: ignore
+    write = file.buffer.raw.write # type: ignore
 
-    path = args.path
+if dumps is not None:
+    try:
+        for path in path_it:
+            result = dumps(path)
+            if not (result is None or isinstance(result, bytes)):
+                result = bytes(str(result), "utf-8")
+            if result:
+                write(result)
+                write(b"\n")
+    except KeyboardInterrupt:
+        pass
+    except BrokenPipeError:
+        from sys import stderr
+        stderr.close()
+    finally:
+        file.close()
+else:
     top = abspath(path)
     fmap: dict[str, Callable] = {
         "inode": DirEntry.inode, 
         "name": lambda e: e.name, 
         "path": lambda e: e.path, 
         "relpath": lambda e: relpath(abspath(e), top), 
         "isdir": isdir, 
         "islink": islink, 
         "stat": stat_to_dict, 
     }
 
-    keys = args.keys or KEYS
+    keys: list[str] = args.keys
     if keys:
         fmap = {k: fmap[k] for k in keys if k in fmap}
-
-    path_it: Iterator[DirEntry] = iterdir(
-        DirEntry(path), 
-        topdown=True if args.depth_first else None, 
-        min_depth=args.min_depth, 
-        max_depth=args.max_depth, 
-        predicate=predicate, 
-        follow_symlinks=args.follow_symlinks, 
-    )
-
-    output_file = args.output_file
-    if output_file:
-        from collections import deque
-        from time import perf_counter
-
-        def format_time(t):
-            m, s = divmod(t, 60)
-            if m < 60:
-                return f"{m:02.0f}:{s:09.06f}"
-            h, m = divmod(m, 60)
-            if h < 24:
-                return f"{h:02.0f}:{m:02.0f}:{s:09.06f}"
-            d, h = divmod(h, 60)
-            return f"{d}d{h:02.0f}:{m:02.0f}:{s:09.06f}"
-
-        def progress(it):
-            write = stdout.buffer.raw.write # type: ignore
-            dq: deque[tuple[int, float]] = deque(maxlen=10*60)
-            push = dq.append
-            total = 0
-            ndirs = 0
-            nfiles = 0
-            start_t = last_t = perf_counter()
-            write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles}".encode())
-            push((total, start_t))
-            for p in it:
-                total += 1
-                if p.is_dir():
-                    ndirs += 1
-                else:
-                    nfiles += 1
-                cur_t = perf_counter()
-                if cur_t - last_t > 0.1:
-                    speed = (total - dq[0][0]) / (cur_t - dq[0][1])
-                    write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles} | 🕙 {format_time(cur_t-start_t)} | 🚀 {speed:.3f} it/s".encode())
-                    push((total, cur_t))
-                    last_t = cur_t
-                yield p
-            cur_t = perf_counter()
-            speed = total / (cur_t - start_t)
-            write(f"\r\x1b[K🗂️  {total} = 📂 {ndirs} + 📝 {nfiles} | 🕙 {format_time(cur_t-start_t)} | 🚀 {speed:.3f} it/s".encode())
-        file = open(output_file, "w")
-        path_it = iter(progress(path_it))
+        keys = list(fmap)
     else:
-        file = stdout # type: ignore
+        keys = KEYS
+
+    if args.hashes:
+        keys.append("hashes")
+        fmap["hashes"] = partial(file_multi_hashes, hashes=args.hashes)
 
     records = ({k: f(e) for k, f in fmap.items()} for e in path_it)
 
     output_type = args.output_type
-    dumps: Callable[..., bytes]
+    json_dumps: Callable[..., bytes]
     if output_type in ("log", "json"):
         try:
-            from orjson import dumps
+            from orjson import dumps as json_dumps
         except ImportError:
             odumps: Callable
             try:
                 from ujson import dumps as odumps
             except ImportError:
                 from json import dumps as odumps
-            dumps = lambda obj, /: bytes(odumps(obj, ensure_ascii=False), "utf-8")
-        if output_file:
-            write = file.buffer.write
-        else:
-            write = file.buffer.raw.write # type: ignore
+            json_dumps = lambda obj, /: bytes(odumps(obj, ensure_ascii=False), "utf-8")
 
     try:
         if output_type == "json":
             write(b"[")
             for i, record in enumerate(records):
                 if i:
                     write(b", ")
-                write(dumps(record))
+                write(json_dumps(record))
             write(b"]")
         elif output_type == "log":
             for record in records:
-                write(dumps(record))
+                write(json_dumps(record))
                 write(b"\n")
         else:
             from csv import DictWriter
 
             writer = DictWriter(file, fieldnames=keys)
             writer.writeheader()
             for record in records:
@@ -193,76 +268,7 @@
         pass
     except BrokenPipeError:
         from sys import stderr
         stderr.close()
     finally:
         file.close()
 
-parser_iter.set_defaults(func=main_iter)
-
-parser_stats = subparsers.add_parser("stats", description="目录树遍历统计")
-
-parser_stats.add_argument("paths", nargs="*", help="文件夹路径，多个用空格隔开，默认从 stdin 读取")
-parser_stats.add_argument("-s", "--select", help="提供一个表达式（会注入一个变量 path，类型是 pathlib.Path），用于对路径进行筛选")
-parser_stats.add_argument("-m", "--min-depth", default=0, type=int, help="最小深度，默认值 0，小于 0 时不限")
-parser_stats.add_argument("-M", "--max-depth", default=-1, type=int, help="最大深度，默认值 -1，小于 0 时不限")
-parser_stats.add_argument("-v", "--version", action="store_true", help="输出版本号")
-
-def main_stats(args):
-    from json import dumps
-    from iterdir import __version__, DirEntry, statsdir
-
-    if args.version:
-        print(".".join(map(str, __version__)))
-        raise SystemExit(0)
-
-    from collections.abc import Callable, Iterable
-    from os import fsdecode
-    from pathlib import Path
-    from typing import Optional
-
-    select = args.select
-    predicate: Optional[Callable[[DirEntry], Optional[bool]]]
-    if select:
-        if select.startswith("lambda "):
-            pred = eval(select)
-        else:
-            pred = eval("lambda path:" + select)
-        predicate = lambda e: pred(Path(fsdecode(e)))
-    else:
-        predicate = None
-
-    paths: Iterable[str]
-    if args.paths:
-        paths = args.paths
-    else:
-        from sys import stdin
-        paths = (path.removesuffix("\n") for path in stdin)
-
-    try:
-        for path in paths:
-            print(
-                dumps(
-                    statsdir(
-                        path, 
-                        min_depth=args.min_depth, 
-                        max_depth=args.max_depth, 
-                        predicate=predicate, 
-                    ), 
-                    ensure_ascii=False, 
-                ), 
-                flush=True, 
-            )
-    except BrokenPipeError:
-        from sys import stderr
-        stderr.close()
-    except (EOFError, KeyboardInterrupt):
-        pass
-
-parser_stats.set_defaults(func=main_stats)
-
-args = parser.parse_args()
-if args.func:
-    args.func(args)
-else:
-    parser.parse_args(["-h"])
-
```

### Comparing `iterdir-0.0.4.2/pyproject.toml` & `iterdir-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "iterdir"
-version = "0.0.4.2"
-description = "iterdir."
+version = "0.0.5"
+description = "python iterate over path tree."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir"
 keywords = ["iterdir", "traverse"]
 classifiers = [
```

### Comparing `iterdir-0.0.4.2/PKG-INFO` & `iterdir-0.0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: iterdir
-Version: 0.0.4.2
-Summary: iterdir.
+Version: 0.0.5
+Summary: python iterate over path tree.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir
 License: MIT
 Keywords: iterdir,traverse
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/iterdir
 Description-Content-Type: text/markdown
 
-# Python iterdir
+# Python iterate over path tree.
 
 ## 安装
 
 你可以通过 [pypi](https://pypi.org/project/iterdir/) 安装
 
 ```console
 pip install -U iterdir
@@ -42,15 +42,15 @@
 
 ```python
 >>> from iterdir import iterdir
 >>> help(iterdir)
 
 Help on function iterdir in module iterdir:
 
-iterdir(top=None, /, topdown: Optional[bool] = True, min_depth: int = 1, max_depth: int = 1, predicate: Optional[collections.abc.Callable[..., Optional[bool]]] = None, onerror: bool | collections.abc.Callable = None, follow_symlinks: bool = False) -> collections.abc.Iterator
+iterdir(top=None, /, topdown: Optional[bool] = True, min_depth: int = 1, max_depth: int = 1, predicate: Optional[collections.abc.Callable[..., Optional[bool]]] = None, onerror: bool | collections.abc.Callable[[OSError], bool] = False, follow_symlinks: bool = False) -> collections.abc.Iterator
     遍历目录树
     
     :param top: 根路径，默认为当前目录。
     :param topdown: 如果是 True，自顶向下深度优先搜索；如果是 False，自底向上深度优先搜索；如果是 None，广度优先搜索。
     :param min_depth: 最小深度，小于 0 时不限。参数 `top` 本身的深度为 0，它的直接跟随路径的深度是 1，以此类推。
     :param max_depth: 最大深度，小于 0 时不限。
     :param predicate: 调用以筛选遍历得到的路径。可接受的参数与参数 `top` 的类型一致，参见 `:return:` 部分。
@@ -65,39 +65,54 @@
 
 ### 用作命令
 
 提供一个命令行工具，用于导出目录树
 
 ```console
 $ python -m iterdir -h
-usage: __main__.py [-h] [-k [{inode,name,path,relpath,isdir,islink,stat} ...]] [-s SELECT] [-t {log,json,csv}] [-o OUTPUT_FILE] [-m MIN_DEPTH]
-                   [-M MAX_DEPTH] [-dfs] [-fl] [-v]
-                   [path]
+usage: __main__ [-h] [-m MIN_DEPTH] [-M MAX_DEPTH]
+                [-k [{inode,name,path,relpath,isdir,islink,stat} ...]]
+                [-t {log,json,csv}] [-d DUMP] [-de] [-s SELECT] [-se]
+                [-o OUTPUT_FILE]
+                [-hs [{sha256,sha3_512,sha1,sha512_256,md5,ripemd160,sha512,md5-sha1,sha3_256,sha384,sha3_384,sha512_224,sha224,sm3,shake_128,blake2s,sha3_224,blake2b,shake_256,crc32} ...]]
+                [-dfs] [-fl] [-v]
+                [path]
 
 目录树信息遍历导出
 
 positional arguments:
   path                  文件夹路径，默认为当前工作目录
 
 options:
   -h, --help            show this help message and exit
+  -m MIN_DEPTH, --min-depth MIN_DEPTH
+                        最小深度，默认值 0，小于 0 时不限
+  -M MAX_DEPTH, --max-depth MAX_DEPTH
+                        最大深度，默认值 -1，小于 0 时不限
   -k [{inode,name,path,relpath,isdir,islink,stat} ...], --keys [{inode,name,path,relpath,isdir,islink,stat} ...]
                         选择输出的 key，默认输出所有可选值
-  -s SELECT, --select SELECT
-                        提供一个表达式（会注入一个变量 path，类型是 pathlib.Path），用于对路径进行筛选
   -t {log,json,csv}, --output-type {log,json,csv}
-                        输出类型，默认为 json
+                        输出类型，默认为 log
                         - log   每行输出一条数据，每条数据输出为一个 json 的 object
                         - json  输出一个 json 的 list，每条数据输出为一个 json 的 object
                         - csv   输出一个 csv，第 1 行为表头，以后每行输出一条数据
+  -d DUMP, --dump DUMP  (优先级高于 -k/--keys、-hs/--hashes、-t/--output-type) 调用以导出数据，如果有返回值则再行输出，尾部会添加一个 b'
+                        '。
+                        如果结果 result 是
+                            - None，跳过
+                            - bytes，输出
+                            - 其它，先调用 `bytes(str(result), 'utf-8')`，再输出
+                        提供一个表达式（会注入一个变量 path，类型是 pathlib.Path）或函数（会传入一个参数，类型是 pathlib.Path）    
+  -de, --dump-exec      对 -d/--dump 传入的代码用 exec 运行，其中必须存在名为 dump 的函数。否则，视为表达式或 lambda 函数
+  -s SELECT, --select SELECT
+                        对路径进行筛选，提供一个表达式（会注入一个变量 path，类型是 pathlib.Path）或函数（会传入一个参数，类型是 pathlib.Path）
+  -se, --select-exec    对 -s/--select 传入的代码用 exec 运行，其中必须存在名为 select 的函数。否则，视为表达式或 lambda 函数
   -o OUTPUT_FILE, --output-file OUTPUT_FILE
                         保存到文件，此时命令行会输出进度条
-  -m MIN_DEPTH, --min-depth MIN_DEPTH
-                        最小深度，默认值 0，小于或等于 0 时不限
-  -M MAX_DEPTH, --max-depth MAX_DEPTH
-                        最大深度，默认值 -1，小于 0 时不限
+  -hs [{sha256,sha3_512,sha1,sha512_256,md5,ripemd160,sha512,md5-sha1,sha3_256,sha384,sha3_384,sha512_224,sha224,sm3,shake_128,blake2s,sha3_224,blake2b,shake_256,crc32} ...], --hashes [{sha256,sha3_512,sha1,sha512_256,md5,ripemd160,sha512,md5-sha1,sha3_256,sha384,sha3_384,sha512_224,sha224,sm3,shake_128,blake2s,sha3_224,blake2b,shake_256,crc32} ...]
+                        计算文件的哈希值，可以选择多个算法
   -dfs, --depth-first   使用深度优先搜索，否则使用广度优先
   -fl, --follow-symlinks
-                        是否跟进符号连接（如果为否，则会把符号链接视为文件，即使它指向目录）
-  -v, --version         输出版本号
+                        跟进符号连接，否则会把符号链接视为文件，即使它指向目录
+  -v, --version         输出版本
 ```
```

