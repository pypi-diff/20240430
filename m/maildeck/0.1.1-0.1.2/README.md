# Comparing `tmp/maildeck-0.1.1.tar.gz` & `tmp/maildeck-0.1.2.tar.gz`

## Comparing `maildeck-0.1.1.tar` & `maildeck-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 maildeck-0.1.1/.python-version
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 maildeck-0.1.1/requirements-dev.lock
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 maildeck-0.1.1/requirements.lock
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 maildeck-0.1.1/src/maildeck/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 maildeck-0.1.1/src/maildeck/__main__.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 maildeck-0.1.1/src/maildeck/config.py
--rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 maildeck-0.1.1/src/maildeck/deck.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 maildeck-0.1.1/src/maildeck/imap.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 maildeck-0.1.1/src/maildeck/maildeck.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 maildeck-0.1.1/.gitignore
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 maildeck-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 maildeck-0.1.1/README.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 maildeck-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 maildeck-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 maildeck-0.1.2/.python-version
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 maildeck-0.1.2/requirements-dev.lock
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 maildeck-0.1.2/requirements.lock
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 maildeck-0.1.2/src/maildeck/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 maildeck-0.1.2/src/maildeck/__main__.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 maildeck-0.1.2/src/maildeck/config.py
+-rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 maildeck-0.1.2/src/maildeck/deck.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 maildeck-0.1.2/src/maildeck/imap.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 maildeck-0.1.2/src/maildeck/maildeck.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 maildeck-0.1.2/.gitignore
+-rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 maildeck-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 maildeck-0.1.2/README.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 maildeck-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 maildeck-0.1.2/PKG-INFO
```

### Comparing `maildeck-0.1.1/src/maildeck/__init__.py` & `maildeck-0.1.2/src/maildeck/__init__.py`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.1/src/maildeck/config.py` & `maildeck-0.1.2/src/maildeck/config.py`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.1/src/maildeck/deck.py` & `maildeck-0.1.2/src/maildeck/deck.py`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.1/src/maildeck/imap.py` & `maildeck-0.1.2/src/maildeck/imap.py`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.1/src/maildeck/maildeck.py` & `maildeck-0.1.2/src/maildeck/maildeck.py`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.1/LICENSE.txt` & `maildeck-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maildeck-0.1.1/README.md` & `maildeck-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 ### Optional Arguments
 
 - **`--imap-port`** IMAP_PORT: The IMAP server port. Default is 993.
 - **`--nextcloud-stack-id`** NEXTCLOUD_STACK_ID: The Nextcloud Deck stack ID. Default is the first stack in the board.
 
 ### Help
 
-- \*\*`-h, --help`: Show the help message and exit.
+- **`-h, --help`**: Show the help message and exit.
 
 **All arguments can also be set as environment variables** with the same name as the placeholder in this help message.
 
 ## Alternatives
 
 - You might also want to have a look at [newroco/mail2deck](https://github.com/newroco/mail2deck), which works a bit
   differently.
```

### Comparing `maildeck-0.1.1/pyproject.toml` & `maildeck-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "maildeck"
-version = "0.1.1"
+version = "0.1.2"
 description = "Import emails into Nextcloud Deck"
 authors = [
     { name = "Mathis Wiehl (@fahrradflucht)", email = "mail-pypi@mathiswiehl.de" }
 ]
 dependencies = []
 readme = "README.md"
-requires-python = ">= 3.11"
+requires-python = ">= 3.10"
 license = { text = "EUPL-1.2" }
 
 [project.scripts]
 "maildeck" = "maildeck:main"
 
 [build-system]
 requires = ["hatchling"]
```

### Comparing `maildeck-0.1.1/PKG-INFO` & `maildeck-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: maildeck
-Version: 0.1.1
+Version: 0.1.2
 Summary: Import emails into Nextcloud Deck
 Author-email: "Mathis Wiehl (@fahrradflucht)" <mail-pypi@mathiswiehl.de>
 License: EUPL-1.2
 License-File: LICENSE.txt
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # maildeck
 
 `maildeck` is a Python command-line tool designed to import emails into Nextcloud Deck. It fetches emails from an IMAP server and creates corresponding cards within a Nextcloud Deck board.
 
 The idea is that you would run this script in a cron job or a systemd-timer.
@@ -53,15 +53,15 @@
 ### Optional Arguments
 
 - **`--imap-port`** IMAP_PORT: The IMAP server port. Default is 993.
 - **`--nextcloud-stack-id`** NEXTCLOUD_STACK_ID: The Nextcloud Deck stack ID. Default is the first stack in the board.
 
 ### Help
 
-- \*\*`-h, --help`: Show the help message and exit.
+- **`-h, --help`**: Show the help message and exit.
 
 **All arguments can also be set as environment variables** with the same name as the placeholder in this help message.
 
 ## Alternatives
 
 - You might also want to have a look at [newroco/mail2deck](https://github.com/newroco/mail2deck), which works a bit
   differently.
```

