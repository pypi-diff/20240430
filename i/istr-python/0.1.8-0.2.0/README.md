# Comparing `tmp/istr_python-0.1.8.tar.gz` & `tmp/istr_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.1.8.tar", last modified: Sun Apr 28 13:16:40 2024, max compression
+gzip compressed data, was "istr_python-0.2.0.tar", last modified: Tue Apr 30 11:49:06 2024, max compression
```

## Comparing `istr_python-0.1.8.tar` & `istr_python-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 13:16:40.905445 istr_python-0.1.8/
--rw-rw-rw-   0        0        0    10790 2024-04-28 13:16:40.903427 istr_python-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     9869 2024-04-28 13:15:20.000000 istr_python-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 13:16:40.859642 istr_python-0.1.8/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.1.8/istr/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.1.8/istr/install istr.py
--rw-rw-rw-   0        0        0    18187 2024-04-28 09:43:05.000000 istr_python-0.1.8/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-04-28 13:16:40.900414 istr_python-0.1.8/istr_python.egg-info/
--rw-rw-rw-   0        0        0    10790 2024-04-28 13:16:40.000000 istr_python-0.1.8/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-28 13:16:40.000000 istr_python-0.1.8/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 13:16:40.000000 istr_python-0.1.8/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-28 13:16:40.000000 istr_python-0.1.8/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      658 2024-04-28 13:16:35.000000 istr_python-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 13:16:40.905445 istr_python-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-28 13:16:40.894785 istr_python-0.1.8/tests/
--rw-rw-rw-   0        0        0    12707 2024-04-26 18:39:45.000000 istr_python-0.1.8/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:49:06.470996 istr_python-0.2.0/
+-rw-rw-rw-   0        0        0    11703 2024-04-30 11:49:06.468918 istr_python-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10764 2024-04-30 07:19:54.000000 istr_python-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 11:49:06.437441 istr_python-0.2.0/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.2.0/istr/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.2.0/istr/install istr.py
+-rw-rw-rw-   0        0        0    20662 2024-04-30 11:44:48.000000 istr_python-0.2.0/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:49:06.465304 istr_python-0.2.0/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    11703 2024-04-30 11:49:06.000000 istr_python-0.2.0/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-30 11:49:06.000000 istr_python-0.2.0/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 11:49:06.000000 istr_python-0.2.0/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-30 11:49:06.000000 istr_python-0.2.0/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      658 2024-04-30 11:48:59.000000 istr_python-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 11:49:06.471994 istr_python-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 11:49:06.463308 istr_python-0.2.0/tests/
+-rw-rw-rw-   0        0        0    13111 2024-04-30 11:45:24.000000 istr_python-0.2.0/tests/test_istr.py
```

### Comparing `istr_python-0.1.8/PKG-INFO` & `istr_python-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.8
+Version: 0.2.0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -252,15 +252,15 @@
 istr('0') a
 istr('1') b
 istr('2') c
 ```
 
 ## concatenate an iterable
 
-The `istr.concat1 method can be useful to map all items of an iterable
+The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
 `list(istr.concat(((1,2),(3,4)))` ==> `istr([12,34])`
 
 `list(istr.concat(itertools.permutations(range(3),2)))` ==> `[istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')]` 
 
 ## Subclassing istr
@@ -411,14 +411,33 @@
 with istr.format("03"):
     print(repr(istr("  12 ")))
 ```
 will result in `istr('0012')`
 
 Remark: For bases other than 10, the string will never be reformatted!
 
+## Operations
+----------------------------
+operator/function   int  str  Example
+----------------------------
++                    x        istr(20) + 3 ==> istr('23')
+_                    x        istr(20) - 3 ==> istr('17')
+*                    x        istr(20) * 3 ==> istr('60')
+/                    x        istr(20) / 3 ==> istr('6')
+//                   x        istr(20) // 3 ==> istr('6')
+%                    x        istr(20) % 3 ==> istr('2')
+**                   x        istr(2) ** 3 ==> istr('8')
+@                         x   istr(20) @ 3 ==> istr('202020')
+==                   x    x   istr(20) == 20 ==> True | istr(20) == '20' ==> True
+|                         x   istr(20) | 5 ==> istr('205')
+abs                  x
+<=, <, >, >=         x        istr('100') > istr('2') ==> True
+slicing              x        istr(12345)[1:3] ==> istr('23')
+----------------------------
+
 ## Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used.
 
 ## Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
```

### Comparing `istr_python-0.1.8/README.md` & `istr_python-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 istr('0') a
 istr('1') b
 istr('2') c
 ```
 
 ## concatenate an iterable
 
-The `istr.concat1 method can be useful to map all items of an iterable
+The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
 `list(istr.concat(((1,2),(3,4)))` ==> `istr([12,34])`
 
 `list(istr.concat(itertools.permutations(range(3),2)))` ==> `[istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')]` 
 
 ## Subclassing istr
@@ -398,17 +398,36 @@
 with istr.format("03"):
     print(repr(istr("  12 ")))
 ```
 will result in `istr('0012')`
 
 Remark: For bases other than 10, the string will never be reformatted!
 
+## Operations
+----------------------------
+operator/function   int  str  Example
+----------------------------
++                    x        istr(20) + 3 ==> istr('23')
+_                    x        istr(20) - 3 ==> istr('17')
+*                    x        istr(20) * 3 ==> istr('60')
+/                    x        istr(20) / 3 ==> istr('6')
+//                   x        istr(20) // 3 ==> istr('6')
+%                    x        istr(20) % 3 ==> istr('2')
+**                   x        istr(2) ** 3 ==> istr('8')
+@                         x   istr(20) @ 3 ==> istr('202020')
+==                   x    x   istr(20) == 20 ==> True | istr(20) == '20' ==> True
+|                         x   istr(20) | 5 ==> istr('205')
+abs                  x
+<=, <, >, >=         x        istr('100') > istr('2') ==> True
+slicing              x        istr(12345)[1:3] ==> istr('23')
+----------------------------
+
 ## Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used.
 
 ## Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
 
 ![PyPI - License](https://img.shields.io/pypi/l/istr-python) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
- ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
+ ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
```

### Comparing `istr_python-0.1.8/istr/install istr.py` & `istr_python-0.2.0/istr/install istr.py`

 * *Files identical despite different names*

### Comparing `istr_python-0.1.8/istr/istr.py` & `istr_python-0.2.0/istr/istr.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,40 @@
 #     _       _
 #    (_) ___ | |_  _ __
 #    | |/ __|| __|| '__|
 #    | |\__ \| |_ | |
 #    |_||___/ \__||_|
 # strings you can count on
 
-__version__ = "0.1" # only x.y here!
+__version__ = "0.2.0"
 import functools
 import math
 
 """
 changelog
 
+version 0.2.0 2024-04-30
+----------------------
+Added __iter__ method__ .
+    So now,
+        for c in istr('123'):
+            ...
+        results in c values that are istrs 
+
+Added istr.digits method:
+    Examples
+    --------
+    istr.digits() ==> istr('0123456789')
+    istr.digits('') ==> istr('0123456789')
+    istr.digits('1') ==> istr('1')
+    istr.digits('3-') ==> istr('3456789')
+    istr.digits('-3') ==> istr('0123')
+    istr('1-4', '6', '8-9') ==> istr('1234689')
+    istr.digits('1', '1-2', '1-3') ==> istr('11213')
+
 version 0.1.2  2024-04-26  
 -------------------------
 Added all relevant string methods to return istrs or data structures with istrs.
 Added corresponding tests.
 
 version 0.1.0  2024-04-22  
 -------------------------
@@ -282,14 +301,17 @@
         if self._mode == "istr":
             self._as_repr = f"{cls.__name__}({repr(as_str)})"
         elif self._mode == "int":
             self._as_repr = repr(as_int)
         else:
             self._as_repr = repr(as_str)
         return self
+              
+    def __iter__(self):
+        yield from self.__class__(super().__iter__())
 
     def __hash__(self):
         return hash((self.__class__, str(self)))
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self._as_int == other._as_int
@@ -489,16 +511,68 @@
 
         def __exit__(self, exc_type, exc_value, exc_tb):
             self.saved_cls._base = self.saved_base
 
     @classmethod
     def range(cls, start, stop=None, step=1):
         return _range(cls, start, stop, step)
+        
+    @classmethod
+    @functools.lru_cache
+    def digits(cls,*args):
+        '''
+        return an istr of istr'ed digits as specified with args
+        
+        if no args, 0-9 will be used
+        
+        all given args will be used
+        each arg has to be either null string, <digit>, <digit>-<digit> or -<digit>
+        
+        examples
+        --------
+        istr.digits() ==> istr('0123456789')
+        istr.digits('') ==> istr('0123456789')
+        istr.digits('1') ==> istr('1')
+        istr.digits('3-') ==> istr('3456789')
+        istr.digits('-3') ==> istr('0123')
+        istr('1-4', '6', '8-9') ==> istr('1234689')
+        istr('1', '1-2', '1-3') ==> istr('11213')
+        '''
+        result=[]
+        if not args:
+            args=['0-9']
+        for arg in args:
+            if arg.strip()=='':
+                arg='0-9'
+            pre,*post=arg.split('-')
+            if pre.strip()=='':
+                pre='0'
+            try:
+                start=int(pre)
+            except ValueError:
+                raise ValueError(f'incorrect specifier: {repr(arg)}')  
+            if not 0<=start<=9:
+                raise ValueError(f'incorrect specifier: {repr(arg)}')                
+            if len(post)>1:
+                raise ValueError(f'incorrect specifier: {repr(arg)}')
+            if post:
+                if post[0].strip()=="":
+                    post="9"
+                try:
+                    stop=int(post[0])
+                except ValueError:
+                    raise ValueError(f'incorrect specifier: {repr(arg)}')                    
+                if (not 0<=start<=9) or start>stop:
+                    raise ValueError(f'incorrect specifier: {repr(arg)}')
+            else:
+                stop=start
+            result.extend(range(start,stop+1))
+        return cls('').join(istr(result))
 
-    def capitalize1(self, *args, **kwargs):
+    def capitalize(self, *args, **kwargs):
         return self.__class__(super().capitalize(*args, **kwargs))
 
     def casefold(self, *args, **kwargs):
         return self.__class__(super().casefold(*args, **kwargs))
 
     def center(self, *args, **kwargs):
         return self.__class__(super().center(*args, **kwargs))
@@ -559,26 +633,21 @@
 
     def upper(self, *args, **kwargs):
         return self.__class__(super().upper(*args, **kwargs))
 
     def zfill(self, *args, **kwargs):
         return self.__class__(super().zfill(*args, **kwargs))
 
-    f = "capitalize"
-    exec(
-        f"""
-def {f}(self, *args, **kwargs):
-        return self.__class__(super(istr,self).{f}(*args, **kwargs)) 
-""",
-        globals(),
-        locals(),
-    )
-
 
 def main():
-    a = istr("123123")
-    print(repr(a.capitalize()))
-
+    print(repr(istr.digits()))
+    print(istr.digits('1-9'))
+    print(istr.digits('1'))
+    print(istr.digits('1-2', '6'))    
+    print(istr.digits('1-5', '7-9'))        
+    print(istr.digits('-5'))   
+    print(istr.digits('3-'))   
+    a=istr('1-4', '6', '8-9')
 
 if __name__ == "__main__":
     main()
```

### Comparing `istr_python-0.1.8/istr_python.egg-info/PKG-INFO` & `istr_python-0.2.0/istr_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.1.8
+Version: 0.2.0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -252,15 +252,15 @@
 istr('0') a
 istr('1') b
 istr('2') c
 ```
 
 ## concatenate an iterable
 
-The `istr.concat1 method can be useful to map all items of an iterable
+The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
 `list(istr.concat(((1,2),(3,4)))` ==> `istr([12,34])`
 
 `list(istr.concat(itertools.permutations(range(3),2)))` ==> `[istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')]` 
 
 ## Subclassing istr
@@ -411,14 +411,33 @@
 with istr.format("03"):
     print(repr(istr("  12 ")))
 ```
 will result in `istr('0012')`
 
 Remark: For bases other than 10, the string will never be reformatted!
 
+## Operations
+----------------------------
+operator/function   int  str  Example
+----------------------------
++                    x        istr(20) + 3 ==> istr('23')
+_                    x        istr(20) - 3 ==> istr('17')
+*                    x        istr(20) * 3 ==> istr('60')
+/                    x        istr(20) / 3 ==> istr('6')
+//                   x        istr(20) // 3 ==> istr('6')
+%                    x        istr(20) % 3 ==> istr('2')
+**                   x        istr(2) ** 3 ==> istr('8')
+@                         x   istr(20) @ 3 ==> istr('202020')
+==                   x    x   istr(20) == 20 ==> True | istr(20) == '20' ==> True
+|                         x   istr(20) | 5 ==> istr('205')
+abs                  x
+<=, <, >, >=         x        istr('100') > istr('2') ==> True
+slicing              x        istr(12345)[1:3] ==> istr('23')
+----------------------------
+
 ## Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used.
 
 ## Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
```

### Comparing `istr_python-0.1.8/pyproject.toml` & `istr_python-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "0.1.8"
+version = "0.2.0"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `istr_python-0.1.8/tests/test_istr.py` & `istr_python-0.2.0/tests/test_istr.py`

 * *Files 5% similar despite different names*

```diff
@@ -470,15 +470,22 @@
         a = istr(15)
     with istr.base(10):
         assert a * a == 225
     with pytest.raises(ValueError):
         assert a | a # FF can't be converted to base 10
         
     
-
+def test_digits():
+    assert istr.digits().equals(istr('0123456789'))
+    assert istr.digits('').equals(istr('0123456789'))
+    assert istr.digits('1').equals(istr('1'))
+    assert istr.digits('3-').equals(istr('3456789'))
+    assert istr.digits('-3').equals(istr('0123'))
+    assert istr.digits('1-4', '6', '8-9').equals(istr('1234689'))
+    assert istr.digits('1', '1-2', '1-3').equals(istr('112123'))
 
 
 def test_subclassing():
     class jstr(istr):
         ...
 
     assert jstr(5).equals(jstr(5))
```

