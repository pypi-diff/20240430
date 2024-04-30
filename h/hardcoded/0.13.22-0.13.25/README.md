# Comparing `tmp/hardcoded-0.13.22.tar.gz` & `tmp/hardcoded-0.13.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardcoded-0.13.22.tar", last modified: Wed Sep 27 09:15:04 2023, max compression
+gzip compressed data, was "hardcoded-0.13.25.tar", max compression
```

## Comparing `hardcoded-0.13.22.tar` & `hardcoded-0.13.25.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxr-xr-x   0 daanvellinga   (501) staff       (20)        0 2023-09-27 09:15:04.769799 hardcoded-0.13.22/
--rw-r--r--   0 daanvellinga   (501) staff       (20)     2475 2023-09-27 09:15:04.769047 hardcoded-0.13.22/PKG-INFO
--rw-r--r--   0 daanvellinga   (501) staff       (20)     1871 2023-09-27 09:14:40.000000 hardcoded-0.13.22/README.md
-drwxr-xr-x   0 daanvellinga   (501) staff       (20)        0 2023-09-27 09:15:04.764690 hardcoded-0.13.22/hardcoded/
--rw-r--r--   0 daanvellinga   (501) staff       (20)     1112 2023-02-20 12:55:16.000000 hardcoded-0.13.22/hardcoded/__init__.py
--rw-r--r--   0 daanvellinga   (501) staff       (20)     2477 2023-06-14 06:25:33.000000 hardcoded-0.13.22/hardcoded/cli.py
--rw-r--r--   0 daanvellinga   (501) staff       (20)     1396 2023-02-20 12:55:16.000000 hardcoded-0.13.22/hardcoded/git.py
--rw-r--r--   0 daanvellinga   (501) staff       (20)    19759 2023-09-11 11:55:40.000000 hardcoded-0.13.22/hardcoded/logic.py
-drwxr-xr-x   0 daanvellinga   (501) staff       (20)        0 2023-09-27 09:15:04.767595 hardcoded-0.13.22/hardcoded.egg-info/
--rw-r--r--   0 daanvellinga   (501) staff       (20)     2475 2023-09-27 09:15:04.000000 hardcoded-0.13.22/hardcoded.egg-info/PKG-INFO
--rw-r--r--   0 daanvellinga   (501) staff       (20)      325 2023-09-27 09:15:04.000000 hardcoded-0.13.22/hardcoded.egg-info/SOURCES.txt
--rw-r--r--   0 daanvellinga   (501) staff       (20)        1 2023-09-27 09:15:04.000000 hardcoded-0.13.22/hardcoded.egg-info/dependency_links.txt
--rw-r--r--   0 daanvellinga   (501) staff       (20)       44 2023-09-27 09:15:04.000000 hardcoded-0.13.22/hardcoded.egg-info/entry_points.txt
--rw-r--r--   0 daanvellinga   (501) staff       (20)        1 2023-03-13 14:51:34.000000 hardcoded-0.13.22/hardcoded.egg-info/not-zip-safe
--rw-r--r--   0 daanvellinga   (501) staff       (20)       93 2023-09-27 09:15:04.000000 hardcoded-0.13.22/hardcoded.egg-info/requires.txt
--rw-r--r--   0 daanvellinga   (501) staff       (20)       10 2023-09-27 09:15:04.000000 hardcoded-0.13.22/hardcoded.egg-info/top_level.txt
--rw-r--r--   0 daanvellinga   (501) staff       (20)       38 2023-09-27 09:15:04.769956 hardcoded-0.13.22/setup.cfg
--rwxr-xr-x   0 daanvellinga   (501) staff       (20)     1103 2023-09-27 09:06:24.000000 hardcoded-0.13.22/setup.py
+-rw-r--r--   0        0        0     1871 2023-09-27 09:14:40.293985 hardcoded-0.13.25/README.md
+-rw-r--r--   0        0        0     1112 2023-02-20 12:55:16.346319 hardcoded-0.13.25/hardcoded/__init__.py
+-rw-r--r--   0        0        0     2477 2023-06-14 06:25:33.929564 hardcoded-0.13.25/hardcoded/cli.py
+-rw-r--r--   0        0        0     1396 2024-02-19 13:26:48.977256 hardcoded-0.13.25/hardcoded/git.py
+-rw-r--r--   0        0        0    22844 2024-04-30 13:46:06.767741 hardcoded-0.13.25/hardcoded/logic.py
+-rw-r--r--   0        0        0      687 2024-04-30 07:21:02.525528 hardcoded-0.13.25/pyproject.toml
+-rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 hardcoded-0.13.25/PKG-INFO
```

### Comparing `hardcoded-0.13.22/PKG-INFO` & `hardcoded-0.13.25/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: hardcoded
-Version: 0.13.22
+Version: 0.13.25
 Summary: For everything that you really should not be hardcoding.
-Home-page: https://pypi.org/project/hardcoded/
+Home-page: https://pypi.org/project/hardcoded
+License: LGPL-3.0-or-later
 Author: moizuo
 Author-email: no_spam@example.com
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Description-Content-Type: text/markdown
-Requires-Dist: Click>=8.0.1
-Requires-Dist: pyyaml
-Requires-Dist: python-gnupg
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: encryption-without-pgp
-Requires-Dist: cryptography>=39.0.0; extra == "encryption-without-pgp"
-Requires-Dist: cffi>=1.15.1; extra == "encryption-without-pgp"
+Requires-Dist: Click (>=8.0.1,<9.0.0)
+Requires-Dist: cffi (>=1.15.1,<2.0.0) ; extra == "encryption-without-pgp"
+Requires-Dist: cryptography (>=39.0.0,<40.0.0) ; extra == "encryption-without-pgp"
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
+Requires-Dist: python-gnupg
+Requires-Dist: pyyaml
+Description-Content-Type: text/markdown
 
 This package wants to replace your hardcoded.password, your hardcoded.api\_key, actually  hardcoded("Everything you really shouldn't be hardcoding").
 
 To move a hardcoded value from your code to an external file, use hardcoded.foo as if it was holding your value already. On running the code, this will happen:
 - if an environment variable exist with exactly the same name ("foo" in our example), the value of that environment variable is returned
 - otherwise, hardcoded will find a file holding your data
     - if you initialised hardcoded as hardcoded.File(path='secrets.yml'), secrets.yml is used
@@ -34,7 +42,8 @@
     - if not running interactively (stdin is not an open TTY), a KeyError is raised
     - if running interactively, you are asked to input the value
         - if encryption is requested with hardcoded.File(secret=True), the YAML is encrypted:
             - if GPG is available, the YAML is GPG encrypted with a key of your choosing
             - if Apple Keychain is available, a random password is generated and stored in the keychain
             - otherwise, you are asked for a new password
 - the value of foo is returned to your code
+
```

### Comparing `hardcoded-0.13.22/README.md` & `hardcoded-0.13.25/README.md`

 * *Files identical despite different names*

### Comparing `hardcoded-0.13.22/hardcoded/__init__.py` & `hardcoded-0.13.25/hardcoded/__init__.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.13.22/hardcoded/cli.py` & `hardcoded-0.13.25/hardcoded/cli.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.13.22/hardcoded/git.py` & `hardcoded-0.13.25/hardcoded/git.py`

 * *Files identical despite different names*

### Comparing `hardcoded-0.13.22/hardcoded/logic.py` & `hardcoded-0.13.25/hardcoded/logic.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import shutil
 import string
 import base64
 import secrets
 import inspect
 import subprocess
 from pathlib import Path
+from collections import defaultdict
 from functools import lru_cache, cached_property
 
 import yaml
 import click
 try:
     from cryptography.fernet import Fernet, InvalidToken
     from cryptography.hazmat.primitives import hashes
@@ -31,14 +32,83 @@
             env['GPG_TTY'] = tty_name
     except:
         pass
     _gpg = gnupg.GPG(use_agent=True, env=env)
 except:
     _gpg = None
 
+try:
+    import psutil
+    possible_mounted_secrets = []
+
+    class MountedFile:
+        def __init__(self, path):
+            self.path = path
+
+        def match_name(self, search_string):
+            # Full path match
+            if str(self.path) == search_string:
+                return 5
+            score = 0
+            # /data/.shhh
+            if self.path.stem.strip('.') == search_string:
+                score = 1
+            # /data/shhh.txt
+            elif self.path.stem == search_string:
+                score = 2
+            # /data/shhh
+            elif self.path.name == search_string:
+                score = 3
+            # /var/secrets/shhh
+            if score > 0 and re.search(r'secret', str(self.path)):
+                score += 1
+            return score
+
+        def __repr__(self):
+            return str(self)
+        def __str__(self):
+            return str(self.path)
+
+        @property
+        def value(self):
+            with self.path.open('r') as f:
+                return f.read()
+
+    for part in psutil.disk_partitions(all=True):
+        if part.fstype in ('proc', 'devpts', 'mqueue', 'sysfs', 'cgroup2'):
+            continue
+        mountpoint = Path(part.mountpoint)
+        if mountpoint.is_file():
+            possible_mounted_secrets.append(MountedFile(mountpoint))
+        elif mountpoint.is_dir():
+            for path in mountpoint.iterdir():
+                if path.is_file():
+                    possible_mounted_secrets.append(MountedFile(path))
+
+    def get_secret_from_mounted_file(name):
+        possible_matches = defaultdict(list)
+        for possible_mounted_secret in possible_mounted_secrets:
+            possible_matches[possible_mounted_secret.match_name(name)].append(possible_mounted_secret)
+        try:
+            highest_score = max(possible_matches.keys())
+        except:
+            raise KeyError(
+                    f'Found no mounted secrets')
+        if highest_score == 0:
+            num_non_matching = possible_matches[0]
+            raise KeyError(
+                    f'Found {num_non_matching} mounted files, but none matching the name "{name}"')
+        best_matches = possible_matches[highest_score]
+        if len(best_matches) > 1:
+            raise KeyError(
+                    f'Could not decide which mounted file to use for "{name}": {best_matches}')
+        return best_matches[0].value
+except:
+    pass
+
 from . import git
 
 DEFAULT_FILE_NAME = '.hardcoded.yml'
 CONFIG_HOME = Path(os.environ.get('XDG_CONFIG_HOME', Path.home()/'.config'))
 DEFAULT_FILE_PATH = CONFIG_HOME / DEFAULT_FILE_NAME.strip('.')
 NOT_GIVEN = object()
 
@@ -234,18 +304,24 @@
                         click.echo(completed_process.stderr.decode(), err=True)
                         exit(completed_process.returncode)
                 except Exception as ex:
                     click.echo(ex, err=True)
                     pass
 
         if not password:
-            if sys.stdin.isatty():
+            if not sys.stdin.isatty():
+                raise RuntimeError(
+                        f'We need an encryption password for {self.path}, but stdin is not a TTY (so we cannot expect input).')
+            try:
                 password = click.prompt(f'Please enter the encryption password for {self.path}', hide_input=True, err=True)
-            else:
-                raise RuntimeError(f'We need an encryption password for {self.path}, but stdin is not a TTY (so we cannot expect input).')
+            except ValueError as ex:
+                if 'closed file' in str(ex):
+                    raise RuntimeError(
+                            f'We need an encryption password for {self.path}, but stdin is closed (so we cannot expect input).')
+                raise
         if save_to_keychain:
             completed_process = subprocess.run(['security', 'add-internet-password', '-U', '-a', account, '-s', 'hardcoded', '-l', f'hardcoded {account}', '-T', '', '-w', password,], capture_output=True)
         return password
 
 
     def fernet(self, password_policy=None):
         if not self._fernet:
@@ -421,45 +497,55 @@
             return None
         elif name == '__origin__':
             return File
 
         if environment_variable := os.environ.get(name):
             return type(environment_variable)
 
+        try:
+            return type(get_secret_from_mounted_file(name))
+        except:
+            pass
+
         data = self._x.data
         if name in data:
             return data.get(name)
 
         if (not self._x.ask_if_not_found) and default != None:
             return default
 
         # Don't try to ask for input if stdin is not a TTY.
         if self._x.ask_if_not_found:
-            if sys.stdin.isatty():
-                if not text:
-                    text = f'Please enter {name} (will be saved in {self._x.path})'
+            if not sys.stdin.isatty():
+                click.echo(f'We need input ({name}), but stdin is not interactive and environment variable ${name} is empty!', err=True)
+                raise KeyError(
+                        f'Missing hardcoded.{name}')
+            if not text:
+                text = f'Please enter {name} (will be saved in {self._x.path})'
+            try:
                 if type == bool or default in (True, False):
                     # Boolean return value expected. Ask a boolean question.
                     click.echo(text, nl=False, err=True)
                     value = click.getchar(echo=True)
                     while not value in 'yn':
                         click.echo(f'\r{text} [yn]', nl=False, err=True)
                         value = click.getchar(echo=True)
                     click.echo(err=True)
                     value = (value.lower() == 'y')
                 else:
                     value = click.prompt(text=text, type=type, default=default, err=True)
-                data = self._x.data
-                data[name] = value
-                self._x.data = data
-                return value
-            else:
-                click.echo(f'We need input ({name}), but stdin is not interactive and environment variable ${name} is empty!', err=True)
-                raise KeyError(
-                        f'Missing hardcoded.{name}')
+            except ValueError as ex:
+                if 'closed file' in str(ex):
+                    raise RuntimeError(
+                            f'We need input ({name}), but stdin is closed and environment variable ${name} is empty!')
+                raise
+            data = self._x.data
+            data[name] = value
+            self._x.data = data
+            return value
         else:
             raise KeyError(
                     f'Missing hardcoded.{name}')
 
 
     def dict(self):
         '''Return a dict containing all the keys and values from this file.'''
```

