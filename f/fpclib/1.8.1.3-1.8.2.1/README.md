# Comparing `tmp/fpclib-1.8.1.3.tar.gz` & `tmp/fpclib-1.8.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpclib-1.8.1.3.tar", max compression
+gzip compressed data, was "fpclib-1.8.2.1.tar", max compression
```

## Comparing `fpclib-1.8.1.3.tar` & `fpclib-1.8.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0    20849 2024-04-29 21:20:39.702437 fpclib-1.8.1.3/LICENSE
--rw-r--r--   0        0        0     3919 2024-04-29 21:42:01.307544 fpclib-1.8.1.3/README.md
--rw-r--r--   0        0        0    96248 2024-04-29 21:32:57.112825 fpclib-1.8.1.3/fpclib/__init__.py
--rw-r--r--   0        0        0     1053 2024-04-29 21:42:47.631574 fpclib-1.8.1.3/pyproject.toml
--rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 fpclib-1.8.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0    20849 2024-04-29 21:20:39.702437 fpclib-1.8.2.1/LICENSE
+-rw-r--r--   0        0        0     3915 2024-04-30 00:44:21.863274 fpclib-1.8.2.1/README.md
+-rw-r--r--   0        0        0    96905 2024-04-30 00:45:48.688030 fpclib-1.8.2.1/fpclib/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-30 00:55:58.075789 fpclib-1.8.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4828 1970-01-01 00:00:00.000000 fpclib-1.8.2.1/PKG-INFO
```

### Comparing `fpclib-1.8.1.3/LICENSE` & `fpclib-1.8.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fpclib-1.8.1.3/README.md` & `fpclib-1.8.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ## General Overview
-"fpclib" stands for "Flashpoint Curation Library" and is a powerful collection of functions and classes you can use and extend to hopefully curate any game/animation in existence through python3. If you're not familiar with curating for Flashpoint and would like to know how to curate, first follow the [Curation Tutorial](https://bluemaxima.org/flashpoint/datahub/Curation_Tutorial) page on the Flashpoint wiki. If you're not familiar with using python or coding, you should read the [official python tutorial](https://docs.python.org/3/tutorial/index.html) before using this library.
+"fpclib" stands for "Flashpoint Curation Library" and is a powerful collection of functions and classes you can use and extend to hopefully curate any game/animation in existence through python3. If you're not familiar with curating for Flashpoint and would like to know how to curate, first follow the [Curation Tutorial](https://flashpointarchive.org/datahub/Curation_Tutorial) page on the Flashpoint wiki. If you're not familiar with using python or coding, you should read the [official python tutorial](https://docs.python.org/3/tutorial/index.html) before using this library.
 
 Although there are already several useful tools you can use for manually curating games/animations for Flashpoint and downloading assets easily, such as Flashpoint Core, cURLsDownloader, and MAD4FP, none of these tools offer the ability to curate through code or automate the process; fpclib was created to fix that. [fpcurator](https://github.com/FlashpointProject/fpcurator) uses fpclib to automatically generate curations. Of course, you should still always manually check any curation you make with fpclib in Flashpoint Core to make sure it works properly.
 
 There are numerous benefits of using fpclib/fpcurator to help you curate:
 
 * By default, fpclib downloads main game/animation files and puts them in the right file format based upon your launch commands.
 * Logos and screenshots can be automatically downloaded from online and converted to PNG files.
```

### Comparing `fpclib-1.8.1.3/fpclib/__init__.py` & `fpclib-1.8.2.1/fpclib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import copy
 import os
 import re
 import uuid
 import pickle
 import stat
 import shutil
+import datetime
 
 INVALID_CHARS = re.compile(r'(?<!^\w)[/<>:\"\\\|\?\*\x00-\x1F]')
 """A compiled pattern that matches invalid charaters to be in a folder name.
 
 :code:`re.compile(r'(?<!^\\w)[/<>:\\"\\\\\\|\\?\\*\\x00-\\x1F]')`
 """
 INVALID_CHARS_NO_SLASH = re.compile(r'(?<!^\w)[<>:\"\|\?\*\x00-\x1F]')
@@ -710,40 +711,52 @@
     if not url:
         return None
     global TABULATION
     TABULATION += 1
     try:
         rurl = normalize(url, True, True, True)
         with requests.get(rurl, **kwargs) as response:
+            if response.status_code >= 400: raise ValueError("Bad response code")
             # Screw weird ascii pages
             soup = BeautifulSoup(response.content.decode("utf-8"), parser)
         return soup
     except Exception as e:
         if ignore_errs:
             return None
         raise e
     finally:
         TABULATION -= 1
 
 def get_fpdata(page, ignore_errs=True):
-    """Reads the Flashpoint online datahub at :code:`https://bluemaxima.org/flashpoint/datahub/{page}` and returns a list of possible values; you can use this to get the most up-to-date tags, platforms, games, or animations.
+    """Reads the Flashpoint online datahub at :code:`https://flashpointarchive.org/datahub/{page}` and returns a list of possible values; you can use this to get the most up-to-date tags and platforms. It will automatically check the web archive if the given wiki page is down.
 
-    :param str page: Can be "Platforms", "Tags", "Game_Master_List", "Animation_Master_List", or any other page on the datahub with tables in it.
+    :param str page: Can be "Platforms", "Tags", or any other page on the datahub with tables in it.
     :param bool ignore_errs: If False, instead of returning None on any errors, those errors will be raised.
 
-    :returns: A list of all Platforms, Tags, Games, Animations, etc. depending on each page.
+    :returns: A list of all Platforms, Tags, etc. depending on each page, or an empty list on failure.
 
     :since 1.3:
     """
     debug('Getting "{}" from Flashpoint datahub', 2, page, pre='[FUNC] ')
     global TABULATION
     TABULATION += 1
     try:
-        soup = get_soup('https://bluemaxima.org/flashpoint/datahub/' + page, ignore_errs=False)
-
+        soup = None
+        url = 'https://flashpointarchive.org/datahub/' + page
+        rurl = url
+        timestamp = None
+        for i in range(4): # Try up to 4 times
+            try:
+                soup = get_soup(rurl, ignore_errs=False, timeout=5)
+                if soup and not soup.select_one("#cf-error-details"): break
+            except (ValueError, requests.ReadTimeout):
+                if timestamp: timestamp -= datetime.timedelta(days=2)
+                else: timestamp = datetime.datetime.now()
+                rurl = f'https://web.archive.org/web/{timestamp.year}{timestamp.month:02}{timestamp.day:02}id_/' + url
+        print(rurl)
         items = []
         i = 0
         if page == "Platforms": i = 1
 
         for table in soup.find_all('table', class_='wikitable'):
             for row in table.find_all('tr')[1:]:
                 try:
@@ -759,15 +772,15 @@
             last = soup.find('div', class_='mw-parser-output').find_all('h2')[-1].next_sibling
             if last is not None and last.name == 'ul':
                 for item in last.find_all('li'):
                     items.append(STARTING_PARENTHESES.sub('', item.text))
         return items
     except Exception as e:
         if ignore_errs:
-            return None
+            return []
         else:
             raise e
     finally:
         TABULATION -= 1
 
 def read(file_name):
     """Reads the contents of the file :code:`file_name` into a string.
@@ -1532,15 +1545,15 @@
     Application Path     applicationPath, appPath, app
     Launch Command       launchCommand, launch, cmd
     Game Notes           gameNotes, notes
     Original Description originalDescription, description, desc
     Curation Notes       curationNotes, cnotes
     ==================== ======================================
 
-    You can find the description of each of these tags on the `Curation Format <https://bluemaxima.org/flashpoint/datahub/Curation_Format#Metadata>`_ page on the Flashpoint wiki.
+    You can find the description of each of these tags on the `Curation Format <https://flashpointarchive.org/datahub/Curation_Format#Metadata>`_ page on the Flashpoint wiki.
     """
 
     def __init__(self, curation=None, **kwargs):
         if not curation:
             self.meta = {
                 'Title': None,
                 'Alternate Titles': None,
@@ -1653,15 +1666,15 @@
     def add_app(self, heading, launch, path=FLASH):
         """Add an additional application. To add extras or a message, use :func:`Curation.add_ext()` and :func:`Curation.add_msg()` respectively.
 
         :param str heading: The name of the additional application.
         :param str launch: The name of the launch command for the additional application.
         :param str path: The application path for the additional application. Defaults to :data:`FLASH`.
 
-        :seealso: The `Additional Applications <https://bluemaxima.org/flashpoint/datahub/Curation_Format#Appendix_II:_Additional_Applications>`_ section of the Curation Format page.
+        :seealso: The `Additional Applications <https://flashpointarchive.org/datahub/Curation_Format#Appendix_II:_Additional_Applications>`_ section of the Curation Format page.
 
         :note: Trying to add an additional app with a heading that already exists will result in replacing it.
 
         :raises ValueError: If :code:`heading` is in :attr:`Curation.RESERVED_APPS`.
         """
         debug('Adding app "{}" to curation {}', 2, heading, str(self), pre='[FUNC] ')
         if heading.lower() in Curation.RESERVED_APPS:
@@ -1672,26 +1685,26 @@
         }
 
     def add_ext(self, folder):
         """Add extras from folder.
 
         :param str folder: The name of the folder the extras are located in.
 
-        :seealso: The `Extras <https://bluemaxima.org/flashpoint/datahub/Curation_Format#Extras>`_ section of the Curation Format page.
+        :seealso: The `Extras <https://flashpointarchive.org/datahub/Curation_Format#Extras>`_ section of the Curation Format page.
 
         :note: Calling this method more than once will replace the current extras."""
         debug('Adding extras folder "{}" to curation {}', 2, folder, str(self), pre='[FUNC] ')
         self.meta['Additional Applications']['Extras'] = folder
 
     def add_msg(self, message):
         """Add message.
 
         :param str message: The message to add to this curation.
 
-        :seealso: The `Messages <https://bluemaxima.org/flashpoint/datahub/Curation_Format#Messages>`_ section of the Curation Format page.
+        :seealso: The `Messages <https://flashpointarchive.org/datahub/Curation_Format#Messages>`_ section of the Curation Format page.
 
         :note: Calling this method more than once will replace the current message.
         """
         debug('Adding message to curation {}', 2, str(self), pre='[FUNC] ')
         self.meta['Additional Applications']['Message'] = message
 
     def del_app(self, heading):
```

### Comparing `fpclib-1.8.1.3/pyproject.toml` & `fpclib-1.8.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fpclib"
-version = "1.8.1.3"
+version = "1.8.2.1"
 description = "A powerful library for curating games for Flashpoint."
 authors = ["mathgeniuszach <huntingmanzach@gmail.com>"]
 license = "CC BY-NC-SA 4.0"
 readme = "README.md"
 repository = "https://github.com/xMGZx/fpclib"
 homepage = "https://www.mathgeniuszach.com/"
 documentation = "https://www.mathgeniuszach.com/bin/fpclib/"
```

### Comparing `fpclib-1.8.1.3/PKG-INFO` & `fpclib-1.8.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpclib
-Version: 1.8.1.3
+Version: 1.8.2.1
 Summary: A powerful library for curating games for Flashpoint.
 Home-page: https://www.mathgeniuszach.com/
 License: CC BY-NC-SA 4.0
 Author: mathgeniuszach
 Author-email: huntingmanzach@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -18,15 +18,15 @@
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ruamel-yaml (==0.16.13)
 Project-URL: Documentation, https://www.mathgeniuszach.com/bin/fpclib/
 Project-URL: Repository, https://github.com/xMGZx/fpclib
 Description-Content-Type: text/markdown
 
 ## General Overview
-"fpclib" stands for "Flashpoint Curation Library" and is a powerful collection of functions and classes you can use and extend to hopefully curate any game/animation in existence through python3. If you're not familiar with curating for Flashpoint and would like to know how to curate, first follow the [Curation Tutorial](https://bluemaxima.org/flashpoint/datahub/Curation_Tutorial) page on the Flashpoint wiki. If you're not familiar with using python or coding, you should read the [official python tutorial](https://docs.python.org/3/tutorial/index.html) before using this library.
+"fpclib" stands for "Flashpoint Curation Library" and is a powerful collection of functions and classes you can use and extend to hopefully curate any game/animation in existence through python3. If you're not familiar with curating for Flashpoint and would like to know how to curate, first follow the [Curation Tutorial](https://flashpointarchive.org/datahub/Curation_Tutorial) page on the Flashpoint wiki. If you're not familiar with using python or coding, you should read the [official python tutorial](https://docs.python.org/3/tutorial/index.html) before using this library.
 
 Although there are already several useful tools you can use for manually curating games/animations for Flashpoint and downloading assets easily, such as Flashpoint Core, cURLsDownloader, and MAD4FP, none of these tools offer the ability to curate through code or automate the process; fpclib was created to fix that. [fpcurator](https://github.com/FlashpointProject/fpcurator) uses fpclib to automatically generate curations. Of course, you should still always manually check any curation you make with fpclib in Flashpoint Core to make sure it works properly.
 
 There are numerous benefits of using fpclib/fpcurator to help you curate:
 
 * By default, fpclib downloads main game/animation files and puts them in the right file format based upon your launch commands.
 * Logos and screenshots can be automatically downloaded from online and converted to PNG files.
```

