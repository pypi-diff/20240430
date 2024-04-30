# Comparing `tmp/pyshared-1.5.5-py3-none-any.whl.zip` & `tmp/pyshared-1.5.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 12251 bytes, number of entries: 16
--rw-r--r--  2.0 unx      781 b- defN 24-Apr-12 00:41 pyshared/__init__.py
+Zip file size: 12623 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      921 b- defN 24-Apr-30 16:46 pyshared/__init__.py
 -rw-r--r--  2.0 unx      124 b- defN 24-Jan-11 01:53 pyshared/consts.py
 -rw-r--r--  2.0 unx     1293 b- defN 24-Jan-12 03:28 pyshared/crypto.py
 -rw-r--r--  2.0 unx     2029 b- defN 24-Apr-03 16:31 pyshared/env.py
 -rw-r--r--  2.0 unx      943 b- defN 24-Mar-31 21:02 pyshared/exceptions.py
 -rw-r--r--  2.0 unx      936 b- defN 24-Apr-12 00:40 pyshared/pytest.py
--rw-r--r--  2.0 unx     4929 b- defN 24-Apr-03 16:29 pyshared/python.py
+-rw-r--r--  2.0 unx     5650 b- defN 24-Apr-21 08:20 pyshared/python.py
 -rw-r--r--  2.0 unx      790 b- defN 24-Jan-11 05:57 pyshared/shell.py
 -rw-r--r--  2.0 unx     2083 b- defN 24-Jan-12 03:45 pyshared/terminal.py
 -rw-r--r--  2.0 unx     2792 b- defN 24-Apr-18 06:32 pyshared/test.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-18 06:34 pyshared/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-18 06:36 pyshared-1.5.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     6829 b- defN 24-Apr-18 06:36 pyshared-1.5.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 06:36 pyshared-1.5.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-18 06:36 pyshared-1.5.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1211 b- defN 24-Apr-18 06:36 pyshared-1.5.5.dist-info/RECORD
-16 files, 25931 bytes uncompressed, 10283 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-30 16:44 pyshared/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-30 16:46 pyshared-1.5.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6929 b- defN 24-Apr-30 16:46 pyshared-1.5.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 16:46 pyshared-1.5.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-30 16:46 pyshared-1.5.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1211 b- defN 24-Apr-30 16:46 pyshared-1.5.7.dist-info/RECORD
+16 files, 26892 bytes uncompressed, 10655 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: pyshared/test.py
 Comment: 
 
 Filename: pyshared/version.py
 Comment: 
 
-Filename: pyshared-1.5.5.dist-info/LICENSE
+Filename: pyshared-1.5.7.dist-info/LICENSE
 Comment: 
 
-Filename: pyshared-1.5.5.dist-info/METADATA
+Filename: pyshared-1.5.7.dist-info/METADATA
 Comment: 
 
-Filename: pyshared-1.5.5.dist-info/WHEEL
+Filename: pyshared-1.5.7.dist-info/WHEEL
 Comment: 
 
-Filename: pyshared-1.5.5.dist-info/top_level.txt
+Filename: pyshared-1.5.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pyshared-1.5.5.dist-info/RECORD
+Filename: pyshared-1.5.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyshared/__init__.py

```diff
@@ -18,16 +18,21 @@
     TypeVar as TypeV,
     Sequence as Seq,
     Iterable as Iter,
 )
 
 # custom imports
 from .version import __version__
+
 from .consts import ALPHANUMERIC_CHARS, ALPHANUMERIC_EXT_CHARS
 from .crypto import is_jwt
 from .env import typed_evar
 from .exceptions import NotPrintableError
-from .python import default_repr, ranstr, safe_repr, truncstr
+from .python import default_repr, ranstr, safe_repr, truncstr, tmp_pythonpath
 from .shell import runcmd
 from .terminal import get_terminal_width, print_columns, print_middle
-from .pytest import multiscope_fixture
 from .test import RanData
+
+try:
+    from .pytest import multiscope_fixture
+except (ImportError, ModuleNotFoundError):
+    print("pytest not installed, skipping multiscope_fixture import")
```

## pyshared/python.py

```diff
@@ -1,20 +1,47 @@
+import os
+import os.path as op
+import sys
+from contextlib import contextmanager
+from importlib import import_module, reload
+from pathlib import Path
+from random import choice, randint
 from typing import (
+    Generator as Gen,
+    Iterable,
+    Iterator,
     Optional as Opt,
     Union,
     Any,
-    Generator as Gen,
-    Iterable,
-    Union as U,
 )
-from random import choice, randint
-from pathlib import Path
-from importlib import reload, import_module
-from .exceptions import NotPrintableError
+
 from .consts import ALPHANUMERIC_CHARS, ALPHANUMERIC_EXT_CHARS
+from .exceptions import NotPrintableError
+
+
+@contextmanager
+def tmp_pythonpath(path: Union[str, Path], strict: bool = False):
+    """Temporarily add a path to the Python path for this context.
+    ~path: The path to add to the Python path.
+    ~strict: If True, only the path will be in the Python path.
+    """
+    og_paths = sys.path.copy()
+    if strict:
+        sys.path = [str(path)]
+    else:
+        sys.path.insert(0, str(path))
+    try:
+        yield
+    finally:
+        sys.path.remove(str(path))
+        curpaths = sys.path.copy()
+        sys.path = og_paths
+        for i, p in enumerate(curpaths):
+            if p not in sys.path:
+                sys.path.insert(i, p)
 
 
 def ranstr(
     min_len: int = 16,
     max_len: Opt[int] = None,
     chars: Iterable = ALPHANUMERIC_CHARS,
     as_generator: bool = False,
```

## pyshared/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.5.5'
+__version__ = '1.5.7'
```

## Comparing `pyshared-1.5.5.dist-info/LICENSE` & `pyshared-1.5.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyshared-1.5.5.dist-info/METADATA` & `pyshared-1.5.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshared
-Version: 1.5.5
+Version: 1.5.7
 Summary: A Python library containing common utility functions for use across multiple codebases, filling gaps not covered by the standard Python libraries.
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Cary Carter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,14 +75,18 @@
 pip install pyshared
 # To include development dependencies:
 pip install pyshared[dev]
 ```
 
 ## Feature Overview
 
+### `args.py`
+
+-
+
 ### `consts.py`
 
 - `ALPHANUMERIC_CHARS`: A string of alphanumeric characters.
 - `ALPHANUMERIC_EXT_CHARS`: Alphanumeric characters, including underscores and hyphens.
 
 ### `crypto.py`
 
@@ -153,32 +157,33 @@
 
 ### `tests.py`
 
 - `RanData`: A class for generating random data for testing purposes.
 
 ## Test Coverage
 
-100% lol
+not quite 100% lol
 
 ```
 ---------- coverage: platform darwin, python 3.9.18-final-0 ----------
 Name                     Stmts   Miss  Cover   Missing
 ------------------------------------------------------
-pyshared/__init__.py         9      0   100%
+pyshared/__init__.py        17      0   100%
 pyshared/consts.py           3      0   100%
 pyshared/crypto.py          21      0   100%
-pyshared/env.py             26      0   100%
+pyshared/env.py             34      3    91%   30, 42, 54
 pyshared/exceptions.py       8      0   100%
-pyshared/pytest.py          11      0   100%
-pyshared/python.py          45      0   100%
+pyshared/pytest.py          12      0   100%
+pyshared/python.py          69      3    96%   40, 63, 139
 pyshared/shell.py            9      0   100%
 pyshared/terminal.py        34      0   100%
+pyshared/test.py            54      0   100%
 pyshared/version.py          1      0   100%
 ------------------------------------------------------
-TOTAL                      167      0   100%
+TOTAL                      262      6    98%
 ```
 
 ## License
 
 MIT
 
 ## Contact
```

## Comparing `pyshared-1.5.5.dist-info/RECORD` & `pyshared-1.5.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-pyshared/__init__.py,sha256=8TrznKzkmm9mjpR6joySUECAwvMGDK0pjCldF9PQfWo,781
+pyshared/__init__.py,sha256=AQ6jfkVz0ti59hIna15DhjdCTN6quoEuCVzDJDXedj4,921
 pyshared/consts.py,sha256=vfUhhaxsFGp-DnTP_iJ-ZFT_w_be6frq9VabkLzejuA,124
 pyshared/crypto.py,sha256=Ww3uT2xa7g0ewgZzvJthJQ_BRPeHM0sLZPc5c3tad2E,1293
 pyshared/env.py,sha256=sJM9SVUIKVq9n7ugpC81zRhvAlNPur_Q8qUiCasglXQ,2029
 pyshared/exceptions.py,sha256=j7alpB6QyzZcCt9quCWPIKXmSsUw7dZPvs7fdqbYbO4,943
 pyshared/pytest.py,sha256=3coYUTNfSHB7-pQIPlIOWwOjbtjgBoX5uEc90DfH188,936
-pyshared/python.py,sha256=2AsqfdwMGv-ZwXvlaKvaPKmXwq69yFSwKIzQfMblD_E,4929
+pyshared/python.py,sha256=k8rBcjZpMYDmvwBydM7AGHwhYIBHLlYeF5RL4TulWRk,5650
 pyshared/shell.py,sha256=F2EJdaImnnlxeiONPlzdXcE_JZ1HUAdBWR5_i-WLfSA,790
 pyshared/terminal.py,sha256=6BjoRuUoqU7iKuXhEqU091aOiQWJUcVWXTMeUlNE3MA,2083
 pyshared/test.py,sha256=Ta4nNuYckDAtay4mltFCrXSHicQyuQvwGrkM0ypvPHQ,2792
-pyshared/version.py,sha256=Zzj2nCH-pedLXQfcBxIuFgiJXSAz9GGJSJ96GFPKLJE,22
-pyshared-1.5.5.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
-pyshared-1.5.5.dist-info/METADATA,sha256=CHBR8FbsUpN7sxO59JrQQORWyEpMP_FA7IrVxahAXdU,6829
-pyshared-1.5.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyshared-1.5.5.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
-pyshared-1.5.5.dist-info/RECORD,,
+pyshared/version.py,sha256=1EQtBGa2dlHmCdA46_Q8GSrMI6pq3EXQ8KTx-m_h-LY,22
+pyshared-1.5.7.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
+pyshared-1.5.7.dist-info/METADATA,sha256=P5Fs-mGBtVTpri5G1xxaI_ZZpIN0PCctSrdgnk0TuRw,6929
+pyshared-1.5.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyshared-1.5.7.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
+pyshared-1.5.7.dist-info/RECORD,,
```

