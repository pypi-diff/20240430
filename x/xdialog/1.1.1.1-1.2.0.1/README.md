# Comparing `tmp/xdialog-1.1.1.1.tar.gz` & `tmp/xdialog-1.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdialog-1.1.1.1.tar", last modified: Sun Mar 19 01:19:20 2023, max compression
+gzip compressed data, was "xdialog-1.2.0.1.tar", last modified: Tue Apr 30 06:20:58 2024, max compression
```

## Comparing `xdialog-1.1.1.1.tar` & `xdialog-1.2.0.1.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 mgz       (1000) mgz       (1000)        0 2023-03-19 01:19:20.898579 xdialog-1.1.1.1/
--rw-r--r--   0 mgz       (1000) mgz       (1000)     1063 2022-09-10 05:53:09.000000 xdialog-1.1.1.1/LICENSE
--rw-r--r--   0 mgz       (1000) mgz       (1000)      411 2023-03-19 01:19:20.898579 xdialog-1.1.1.1/PKG-INFO
--rw-r--r--   0 mgz       (1000) mgz       (1000)     2376 2023-03-19 00:21:00.000000 xdialog-1.1.1.1/README.md
--rw-r--r--   0 mgz       (1000) mgz       (1000)       38 2023-03-19 01:19:20.898579 xdialog-1.1.1.1/setup.cfg
--rwxrwxrwx   0 mgz       (1000) mgz       (1000)      816 2023-03-19 01:19:17.000000 xdialog-1.1.1.1/setup.py
-drwxr-xr-x   0 mgz       (1000) mgz       (1000)        0 2023-03-19 01:19:20.898579 xdialog-1.1.1.1/xdialog/
--rw-r--r--   0 mgz       (1000) mgz       (1000)     7477 2023-03-19 00:13:16.000000 xdialog-1.1.1.1/xdialog/__init__.py
--rw-r--r--   0 mgz       (1000) mgz       (1000)       42 2022-09-10 05:53:09.000000 xdialog-1.1.1.1/xdialog/constants.py
--rw-r--r--   0 mgz       (1000) mgz       (1000)     3407 2023-03-19 01:09:51.000000 xdialog-1.1.1.1/xdialog/mac_dialogs.py
--rw-r--r--   0 mgz       (1000) mgz       (1000)     2452 2022-09-10 05:53:09.000000 xdialog-1.1.1.1/xdialog/test.py
--rw-r--r--   0 mgz       (1000) mgz       (1000)     1154 2022-09-10 05:53:09.000000 xdialog-1.1.1.1/xdialog/tk_dialogs.py
--rw-r--r--   0 mgz       (1000) mgz       (1000)     5420 2023-03-18 07:59:59.000000 xdialog-1.1.1.1/xdialog/windows_dialogs.py
--rw-r--r--   0 mgz       (1000) mgz       (1000)     8698 2022-10-28 17:15:19.000000 xdialog-1.1.1.1/xdialog/windows_structs.py
--rw-r--r--   0 mgz       (1000) mgz       (1000)     3140 2023-03-18 07:40:42.000000 xdialog-1.1.1.1/xdialog/zenity_dialogs.py
-drwxr-xr-x   0 mgz       (1000) mgz       (1000)        0 2023-03-19 01:19:20.898579 xdialog-1.1.1.1/xdialog.egg-info/
--rw-r--r--   0 mgz       (1000) mgz       (1000)      411 2023-03-19 01:19:20.000000 xdialog-1.1.1.1/xdialog.egg-info/PKG-INFO
--rw-r--r--   0 mgz       (1000) mgz       (1000)      332 2023-03-19 01:19:20.000000 xdialog-1.1.1.1/xdialog.egg-info/SOURCES.txt
--rw-r--r--   0 mgz       (1000) mgz       (1000)        1 2023-03-19 01:19:20.000000 xdialog-1.1.1.1/xdialog.egg-info/dependency_links.txt
--rw-r--r--   0 mgz       (1000) mgz       (1000)        8 2023-03-19 01:19:20.000000 xdialog-1.1.1.1/xdialog.egg-info/top_level.txt
+drwxr-xr-x   0 mgz       (1000) mgz       (1000)        0 2024-04-30 06:20:58.112790 xdialog-1.2.0.1/
+-rw-r--r--   0 mgz       (1000) mgz       (1000)       66 2022-09-10 05:53:09.000000 xdialog-1.2.0.1/.gitattributes
+-rw-r--r--   0 mgz       (1000) mgz       (1000)       40 2024-04-30 06:19:21.000000 xdialog-1.2.0.1/.gitignore
+-rw-r--r--   0 mgz       (1000) mgz       (1000)     1063 2022-09-10 05:53:09.000000 xdialog-1.2.0.1/LICENSE
+-rw-r--r--   0 mgz       (1000) mgz       (1000)      411 2024-04-30 06:20:58.112790 xdialog-1.2.0.1/PKG-INFO
+-rw-r--r--   0 mgz       (1000) mgz       (1000)     2524 2024-04-30 03:08:02.000000 xdialog-1.2.0.1/README.md
+-rw-r--r--   0 mgz       (1000) mgz       (1000)       38 2024-04-30 06:20:58.112790 xdialog-1.2.0.1/setup.cfg
+-rwxrwxrwx   0 mgz       (1000) mgz       (1000)      805 2024-04-30 06:20:50.000000 xdialog-1.2.0.1/setup.py
+-rwxrwxrwx   0 mgz       (1000) mgz       (1000)      140 2022-08-31 03:16:14.000000 xdialog-1.2.0.1/upload
+drwxr-xr-x   0 mgz       (1000) mgz       (1000)        0 2024-04-30 06:20:58.112790 xdialog-1.2.0.1/xdialog/
+-rw-r--r--   0 mgz       (1000) mgz       (1000)     7496 2024-04-30 03:28:16.000000 xdialog-1.2.0.1/xdialog/__init__.py
+-rw-r--r--   0 mgz       (1000) mgz       (1000)       42 2024-04-30 02:55:02.000000 xdialog-1.2.0.1/xdialog/constants.py
+-rw-r--r--   0 mgz       (1000) mgz       (1000)     3407 2023-03-19 01:09:51.000000 xdialog-1.2.0.1/xdialog/mac_dialogs.py
+-rw-r--r--   0 mgz       (1000) mgz       (1000)     2452 2022-09-10 05:53:09.000000 xdialog-1.2.0.1/xdialog/test.py
+-rw-r--r--   0 mgz       (1000) mgz       (1000)     1154 2022-09-10 05:53:09.000000 xdialog-1.2.0.1/xdialog/tk_dialogs.py
+-rw-r--r--   0 mgz       (1000) mgz       (1000)     5420 2023-03-18 07:59:59.000000 xdialog-1.2.0.1/xdialog/windows_dialogs.py
+-rw-r--r--   0 mgz       (1000) mgz       (1000)     8698 2022-10-28 17:15:19.000000 xdialog-1.2.0.1/xdialog/windows_structs.py
+-rw-r--r--   0 mgz       (1000) mgz       (1000)     4442 2024-04-30 06:05:53.000000 xdialog-1.2.0.1/xdialog/yad_dialogs.py
+-rw-r--r--   0 mgz       (1000) mgz       (1000)     3306 2024-04-30 05:55:05.000000 xdialog-1.2.0.1/xdialog/zenity_dialogs.py
+drwxr-xr-x   0 mgz       (1000) mgz       (1000)        0 2024-04-30 06:20:58.112790 xdialog-1.2.0.1/xdialog.egg-info/
+-rw-r--r--   0 mgz       (1000) mgz       (1000)      411 2024-04-30 06:20:58.000000 xdialog-1.2.0.1/xdialog.egg-info/PKG-INFO
+-rw-r--r--   0 mgz       (1000) mgz       (1000)      388 2024-04-30 06:20:58.000000 xdialog-1.2.0.1/xdialog.egg-info/SOURCES.txt
+-rw-r--r--   0 mgz       (1000) mgz       (1000)        1 2024-04-30 06:20:58.000000 xdialog-1.2.0.1/xdialog.egg-info/dependency_links.txt
+-rw-r--r--   0 mgz       (1000) mgz       (1000)        8 2024-04-30 06:20:58.000000 xdialog-1.2.0.1/xdialog.egg-info/top_level.txt
```

### Comparing `xdialog-1.1.1.1/LICENSE` & `xdialog-1.2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xdialog-1.1.1.1/README.md` & `xdialog-1.2.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 Or you can copy and paste the xdialog folder into the root of your project if pip isn't available; this is possible because xdialog only uses modules in the standard library.
 
 Here's how xdialog determines what dialogs to use:
 
 - On Windows, xdialog uses the built-in ctypes module to interface directly with system dialogs.
 - On MacOS, it uses AppleScript to interface directly with system dialogs.
-- On Linux and other systems, it uses the `zenity` command, or defaults to Tkinter if `zenity` is not available.
+- On Linux and other systems, it uses the `yad` command, the `zenity` command, or defaults to Tkinter if neither are available.
 
 ## Notes
 
-Both `zenity` and AppleScript provide easy access to password/input prompts, color pickers, and a few more useful things from the command line, while Windows makes it more difficult to access these (it requires using ctypes to mimic C++ code). It could be possible to rebind tk's dialogs on Windows into python, but for now these functions will not be implemented.
+`yad`, `zenity`, and AppleScript provide easy access to password/input prompts, color pickers, and a few more useful things from the command line, while Windows makes it more difficult to access these (it requires using ctypes to mimic C++ code). It could be possible to rebind tk's dialogs on Windows into python, but for now these functions will not be implemented.
 
 ## Usage
 
 ```python
 import xdialog
 
 # For opening files (returns either Iterable[str], or str, which is empty on failure)
@@ -43,8 +43,12 @@
 
 # Other dialogs are also available:
 # They can return xdialog.YES, xdialog.NO, xdialog.CANCEL, xdialog.RETRY, or xdialog.OK.
 xdialog.yesno("Title Here", "Yes, or No?")
 xdialog.yesnocancel("Title Here", "Do you want to read from this file?")
 xdialog.retrycancel("Title Here", "Failure, do you want to retry?")
 xdialog.okcancel("Title Here", "Someone did something bad on social media.")
-```
+```
+
+## Contact
+
+Contact me on [Discord](https://discord.gg/pBFqEcXvW5) and support me on [Ko-Fi](https://ko-fi.com/mathgeniuszach)!
```

### Comparing `xdialog-1.1.1.1/setup.py` & `xdialog-1.2.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-#!/usr/bin/env python3
-
-import setuptools
-
-from pathlib import Path
-
-build = Path("build.txt")
-def get_build():
-    if build.is_file():
-        num = int(build.read_text())
-        build.write_text(str(num+1))
-        return num+1
-    else:
-        build.write_text("0")
-        return 0
-
-setuptools.setup(
-    name='xdialog',
-    version=f'1.1.1.{get_build()}',
-    author='mathgeniuszach',
-    author_email='huntingmanzach@gmail.com',
-    description='A cross-platform python wrapper for native dialogs.',
-    long_description='A cross-platform python wrapper for native dialogs. Portable as it only uses the standard library.',
-    url='https://github.com/xMGZx/xdialog',
-    packages=['xdialog'],
-    license='MIT License',
-    classifiers=['Programming Language :: Python :: 3']
-)
-
+#!/usr/bin/env python3
+
+import setuptools
+
+from pathlib import Path
+
+build = Path(__file__).parent / "build.txt"
+def get_build():
+    if build.is_file():
+        num = int(build.read_text())
+        build.write_text(str(num+1))
+        return num+1
+    else:
+        build.write_text("0")
+        return 0
+
+setuptools.setup(
+    name='xdialog',
+    version=f'1.2.0.{get_build()}',
+    author='mathgeniuszach',
+    author_email='huntingmanzach@gmail.com',
+    description='A cross-platform python wrapper for native dialogs.',
+    long_description='A cross-platform python wrapper for native dialogs. Portable as it only uses the standard library.',
+    url='https://github.com/xMGZx/xdialog',
+    packages=['xdialog'],
+    license='MIT License',
+    classifiers=['Programming Language :: Python :: 3']
+)
+
```

### Comparing `xdialog-1.1.1.1/xdialog/__init__.py` & `xdialog-1.2.0.1/xdialog/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,27 @@
         from . import mac_dialogs
         return mac_dialogs
     else:
         def cmd_exists(cmd):
             proc = subprocess.Popen(('which', cmd), stdout=subprocess.PIPE, stderr=subprocess.DEVNULL, shell=False)
             proc.communicate()
             return not proc.returncode
-        
+
+        if cmd_exists('yad'):
+            from . import yad_dialogs
+            return yad_dialogs
         if cmd_exists('zenity'):
             from . import zenity_dialogs
             return zenity_dialogs
-    
+
     try:
         from . import tk_dialogs
         return tk_dialogs
     except ModuleNotFoundError: pass
-    
+
     raise ModuleNotFoundError('No dialog type is supported on this machine. Install tkinter to guarantee dialogs.')
 
 
 
 dialogs = get_dialogs()
 
 @overload
@@ -126,78 +129,78 @@
 
 def warning(title: Optional[str] = None, message: str = '') -> None:
     '''Shows a warning dialog box.
 
     Arguments:
         title: Text to show on the header of the dialog box.
             Omitting it has system-dependent results.
-        
+
         message: Text to show in the middle of the dialog box.
     '''
     dialogs.warning(title, message)
 
 def error(title: Optional[str] = None, message: str = '') -> None:
     '''Shows an error dialog box.
 
     Arguments:
         title: Text to show on the header of the dialog box.
             Omitting it has system-dependent results.
-        
+
         message: Text to show in the middle of the dialog box.
     '''
     dialogs.error(title, message)
 
 def yesno(title: Optional[str] = None, message: str = '') -> int:
     '''Shows a question dialog box with the buttons "Yes" and "No".
 
     Arguments:
         title: Text to show on the header of the dialog box.
             Omitting it has system-dependent results.
-        
+
         message: Text to show in the middle of the dialog box.
-    
+
     Returns:
         `xdialog.YES` or `xdialog.NO`. Closing the box results in `xdialog.NO`.
     '''
     return dialogs.yesno(title, message)
 
 def yesnocancel(title: Optional[str] = None, message: str = '') -> int:
     '''Shows a question dialog box with the buttons "Yes", "No", and "Cancel".
 
     Arguments:
         title: Text to show on the header of the dialog box.
             Omitting it has system-dependent results.
-        
+
         message: Text to show in the middle of the dialog box.
-    
+
     Returns:
         `xdialog.YES`, `xdialog.NO`, or `xdialog.CANCEL`. Closing the box results in `xdialog.CANCEL`.
     '''
     return dialogs.yesnocancel(title, message)
 
 def retrycancel(title: Optional[str] = None, message: str = '') -> int:
     '''Shows a question dialog box with the buttons "Retry" and "Cancel".
 
     Arguments:
         title: Text to show on the header of the dialog box.
             Omitting it has system-dependent results.
-        
+
         message: Text to show in the middle of the dialog box.
-    
+
     Returns:
         `xdialog.RETRY` or `xdialog.CANCEL`. Closing the box results in `xdialog.CANCEL`.
     '''
     return dialogs.retrycancel(title, message)
 
 def okcancel(title: Optional[str] = None, message: str = '') -> int:
     '''Shows a question dialog box with the buttons "Ok" and "Cancel".
 
     Arguments:
         title: Text to show on the header of the dialog box.
             Omitting it has system-dependent results.
-        
+
         message: Text to show in the middle of the dialog box.
-    
+
     Returns:
         `xdialog.OK` or `xdialog.CANCEL`. Closing the box results in `xdialog.CANCEL`.
     '''
     return dialogs.okcancel(title, message)
```

### Comparing `xdialog-1.1.1.1/xdialog/mac_dialogs.py` & `xdialog-1.2.0.1/xdialog/mac_dialogs.py`

 * *Files identical despite different names*

### Comparing `xdialog-1.1.1.1/xdialog/test.py` & `xdialog-1.2.0.1/xdialog/test.py`

 * *Files identical despite different names*

### Comparing `xdialog-1.1.1.1/xdialog/tk_dialogs.py` & `xdialog-1.2.0.1/xdialog/tk_dialogs.py`

 * *Files identical despite different names*

### Comparing `xdialog-1.1.1.1/xdialog/windows_dialogs.py` & `xdialog-1.2.0.1/xdialog/windows_dialogs.py`

 * *Files identical despite different names*

### Comparing `xdialog-1.1.1.1/xdialog/windows_structs.py` & `xdialog-1.2.0.1/xdialog/windows_structs.py`

 * *Files identical despite different names*

### Comparing `xdialog-1.1.1.1/xdialog/zenity_dialogs.py` & `xdialog-1.2.0.1/xdialog/zenity_dialogs.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,38 @@
         .replace("!", "\\!")\
         .replace("*", "\\*")\
         .replace("?", "\\?")\
         .replace("&", "&amp;")\
         .replace("|", "&#124;")\
         .replace("<", "&lt;")\
         .replace(">", "&gt;")\
+        .replace("(", "\\(")\
+        .replace(")", "\\)")\
+        .replace("[", "\\[")\
+        .replace("]", "\\]")\
+        .replace("{", "\\{")\
+        .replace("}", "\\}")\
 
 def zenity(typ, filetypes=None, **kwargs) -> Tuple[int, str]:
     # Build args based on keywords
     args = ['zenity', '--'+typ]
     for k, v in kwargs.items():
         if v is True:
             args.append(f'--{k.replace("_", "-").strip("-")}')
         elif isinstance(v, str):
             cv = clean(v) if k != "title" else v
-            args.append(f'--{k.replace("_", "-").strip("-")}={cv}') 
-    
+            args.append(f'--{k.replace("_", "-").strip("-")}={cv}')
+
     # Build filetypes specially if specified
     if filetypes:
         for name, globs in filetypes:
             if name:
                 globlist = globs.split()
                 args.append(f'--file-filter={name.replace("|", "")} ({", ".join(t for t in globlist)})|{globs}')
-    
+
     proc = subprocess.Popen(
         args,
         stdout=subprocess.PIPE,
         stderr=subprocess.DEVNULL,
         shell=False
     )
     stdout, _ = proc.communicate()
@@ -89,15 +95,15 @@
         return CANCEL
     else:
         return YES
 
 def retrycancel(title, message):
     r = zenity(
         "question",
-        title=(title or "Retry"),
+        title=(title or ""),
         text=message,
         ok_label="Retry",
         cancel_label="Cancel"
     )[0]
 
     if r:
         return CANCEL
```

