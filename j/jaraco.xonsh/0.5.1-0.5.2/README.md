# Comparing `tmp/jaraco_xonsh-0.5.1.tar.gz` & `tmp/jaraco_xonsh-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco_xonsh-0.5.1.tar", last modified: Sat Apr 20 13:50:29 2024, max compression
+gzip compressed data, was "jaraco_xonsh-0.5.2.tar", last modified: Tue Apr 30 13:42:46 2024, max compression
```

## Comparing `jaraco_xonsh-0.5.1.tar` & `jaraco_xonsh-0.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.605560 jaraco_xonsh-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.601560 jaraco_xonsh-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.601560 jaraco_xonsh-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-20 13:50:29.605560 jaraco_xonsh-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.601560 jaraco_xonsh-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.601560 jaraco_xonsh-0.5.1/jaraco/
--rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/jaraco/xonsh.xsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:50:29.605560 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 13:50:29.000000 jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:50:29.605560 jaraco_xonsh-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-20 13:50:08.000000 jaraco_xonsh-0.5.1/tox.ini
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.778018 jaraco_xonsh-0.5.2/
+-rw-r--r--   0 jaraco     (501) staff       (20)      200 2024-02-10 03:17:09.000000 jaraco_xonsh-0.5.2/.coveragerc
+-rw-r--r--   0 jaraco     (501) staff       (20)      246 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/.editorconfig
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.774630 jaraco_xonsh-0.5.2/.github/
+-rw-r--r--   0 jaraco     (501) staff       (20)      148 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/.github/dependabot.yml
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.774730 jaraco_xonsh-0.5.2/.github/workflows/
+-rw-r--r--   0 jaraco     (501) staff       (20)     3051 2024-04-30 13:42:36.000000 jaraco_xonsh-0.5.2/.github/workflows/main.yml
+-rw-r--r--   0 jaraco     (501) staff       (20)      116 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 jaraco     (501) staff       (20)      335 2024-03-24 16:04:55.000000 jaraco_xonsh-0.5.2/.readthedocs.yaml
+-rw-r--r--   0 jaraco     (501) staff       (20)     1023 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/LICENSE
+-rw-r--r--   0 jaraco     (501) staff       (20)      954 2024-04-28 19:37:03.000000 jaraco_xonsh-0.5.2/NEWS.rst
+-rw-r--r--   0 jaraco     (501) staff       (20)     2041 2024-04-30 13:42:46.777767 jaraco_xonsh-0.5.2/PKG-INFO
+-rw-r--r--   0 jaraco     (501) staff       (20)      826 2024-02-10 03:17:09.000000 jaraco_xonsh-0.5.2/README.rst
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.775029 jaraco_xonsh-0.5.2/docs/
+-rw-r--r--   0 jaraco     (501) staff       (20)     1122 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/docs/conf.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/docs/history.rst
+-rw-r--r--   0 jaraco     (501) staff       (20)      248 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/docs/index.rst
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.775141 jaraco_xonsh-0.5.2/jaraco/
+-rw-r--r--   0 jaraco     (501) staff       (20)    12620 2024-04-28 19:34:55.000000 jaraco_xonsh-0.5.2/jaraco/xonsh.xsh
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-30 13:42:46.776660 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/
+-rw-r--r--   0 jaraco     (501) staff       (20)     2041 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/PKG-INFO
+-rw-r--r--   0 jaraco     (501) staff       (20)      493 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/SOURCES.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)        1 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/dependency_links.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)       45 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/entry_points.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)      225 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/requires.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)        7 2024-04-30 13:42:46.000000 jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/top_level.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)      154 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/mypy.ini
+-rw-r--r--   0 jaraco     (501) staff       (20)     1143 2024-04-30 07:01:07.000000 jaraco_xonsh-0.5.2/pyproject.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)      584 2024-04-02 14:34:12.000000 jaraco_xonsh-0.5.2/pytest.ini
+-rw-r--r--   0 jaraco     (501) staff       (20)      419 2024-03-24 16:04:55.000000 jaraco_xonsh-0.5.2/ruff.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)       38 2024-04-30 13:42:46.778204 jaraco_xonsh-0.5.2/setup.cfg
+-rw-r--r--   0 jaraco     (501) staff       (20)       44 2024-02-02 02:03:10.000000 jaraco_xonsh-0.5.2/towncrier.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)     1364 2024-02-19 08:35:02.000000 jaraco_xonsh-0.5.2/tox.ini
```

### Comparing `jaraco_xonsh-0.5.1/.github/workflows/main.yml` & `jaraco_xonsh-0.5.2/.github/workflows/main.yml`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
           platform: ubuntu-latest
         - python: "3.11"
           platform: ubuntu-latest
         # disable PyPy as it breaks CI
         # - python: pypy3.10
         #  platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.python == '3.13' }}
+    continue-on-error: ${{ matrix.python == '3.13' || (matrix.python == '3.8' || matrix.python == '3.9') && matrix.platform == 'macos-latest' }}
     steps:
       - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
```

### Comparing `jaraco_xonsh-0.5.1/LICENSE` & `jaraco_xonsh-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.5.1/NEWS.rst` & `jaraco_xonsh-0.5.2/NEWS.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v0.5.2
+======
+
+Bugfixes
+--------
+
+- Ensure at least the PATH is retained for shutil.which/subprocess.
+
+
 v0.5.1
 ======
 
 No significant changes.
 
 
 v0.5.0
```

### Comparing `jaraco_xonsh-0.5.1/PKG-INFO` & `jaraco_xonsh-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.xonsh
-Version: 0.5.1
+Version: 0.5.2
 Summary: Xonsh facilities used by jaraco
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/jaraco.xonsh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jaraco_xonsh-0.5.1/README.rst` & `jaraco_xonsh-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.5.1/docs/conf.py` & `jaraco_xonsh-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.5.1/jaraco/xonsh.xsh` & `jaraco_xonsh-0.5.2/jaraco/xonsh.xsh`

 * *Files 2% similar despite different names*

```diff
@@ -431,7 +431,12 @@
 	except AttributeError:
 		number = '+'
 	towncrier create -c @(descr.strip().rstrip('.') + '.') @(number).@(type).rst
 	git add newsfragments
 	git commit --amend --no-edit
 
 aliases['re-log'] = re_log
+
+
+# workaround for https://github.com/xonsh/xonsh/issues/3207
+if '/.local/bin' not in os.environ['PATH']:
+	os.environ['PATH'] = os.pathsep.join($PATH)
```

### Comparing `jaraco_xonsh-0.5.1/jaraco.xonsh.egg-info/PKG-INFO` & `jaraco_xonsh-0.5.2/jaraco.xonsh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.xonsh
-Version: 0.5.1
+Version: 0.5.2
 Summary: Xonsh facilities used by jaraco
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/jaraco.xonsh
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jaraco_xonsh-0.5.1/pyproject.toml` & `jaraco_xonsh-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.5.1/pytest.ini` & `jaraco_xonsh-0.5.2/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco_xonsh-0.5.1/tox.ini` & `jaraco_xonsh-0.5.2/tox.ini`

 * *Files identical despite different names*

