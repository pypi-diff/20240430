# Comparing `tmp/trytoncommunity-setuptools-0.3.tar.gz` & `tmp/trytoncommunity_setuptools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytoncommunity-setuptools-0.3.tar", last modified: Tue Nov  7 11:05:44 2023, max compression
+gzip compressed data, was "trytoncommunity_setuptools-0.4.0.tar", last modified: Tue Apr 30 12:56:21 2024, max compression
```

## Comparing `trytoncommunity-setuptools-0.3.tar` & `trytoncommunity_setuptools-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 hartmut   (1000) hartmut   (1000)        0 2023-11-07 11:05:44.550646 trytoncommunity-setuptools-0.3/
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)      394 2023-11-07 11:05:43.000000 trytoncommunity-setuptools-0.3/CHANGES
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)    35149 2023-11-07 11:05:43.000000 trytoncommunity-setuptools-0.3/LICENSE-GPL-3.0.txt
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)       26 2023-11-07 11:05:43.000000 trytoncommunity-setuptools-0.3/MANIFEST.in
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)     3493 2023-11-07 11:05:44.550646 trytoncommunity-setuptools-0.3/PKG-INFO
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)     2451 2023-11-07 11:05:43.000000 trytoncommunity-setuptools-0.3/README.rst
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)     1303 2023-11-07 11:05:44.550646 trytoncommunity-setuptools-0.3/setup.cfg
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)       38 2023-11-07 11:05:43.000000 trytoncommunity-setuptools-0.3/setup.py
-drwxrwxr-x   0 hartmut   (1000) hartmut   (1000)        0 2023-11-07 11:05:44.549646 trytoncommunity-setuptools-0.3/src/
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)     9499 2023-11-07 11:05:43.000000 trytoncommunity-setuptools-0.3/src/__init__.py
-drwxrwxr-x   0 hartmut   (1000) hartmut   (1000)        0 2023-11-07 11:05:44.550646 trytoncommunity-setuptools-0.3/trytoncommunity_setuptools.egg-info/
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)     3493 2023-11-07 11:05:44.000000 trytoncommunity-setuptools-0.3/trytoncommunity_setuptools.egg-info/PKG-INFO
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)      334 2023-11-07 11:05:44.000000 trytoncommunity-setuptools-0.3/trytoncommunity_setuptools.egg-info/SOURCES.txt
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)        1 2023-11-07 11:05:44.000000 trytoncommunity-setuptools-0.3/trytoncommunity_setuptools.egg-info/dependency_links.txt
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)       11 2023-11-07 11:05:44.000000 trytoncommunity-setuptools-0.3/trytoncommunity_setuptools.egg-info/requires.txt
--rw-rw-r--   0 hartmut   (1000) hartmut   (1000)       27 2023-11-07 11:05:44.000000 trytoncommunity-setuptools-0.3/trytoncommunity_setuptools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:56:21.341857 trytoncommunity_setuptools-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-11-07 11:07:46.000000 trytoncommunity_setuptools-0.4.0/CHANGES
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-11-02 10:53:21.000000 trytoncommunity_setuptools-0.4.0/LICENSE-GPL-3.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-11-02 10:53:21.000000 trytoncommunity_setuptools-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3521 2024-04-30 12:56:21.341857 trytoncommunity_setuptools-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-11-07 11:07:46.000000 trytoncommunity_setuptools-0.4.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-04-30 12:51:16.000000 trytoncommunity_setuptools-0.4.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2024-04-30 12:56:21.345857 trytoncommunity_setuptools-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-11-02 10:53:21.000000 trytoncommunity_setuptools-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:56:21.341857 trytoncommunity_setuptools-0.4.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)     9952 2024-04-30 08:44:50.000000 trytoncommunity_setuptools-0.4.0/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:56:21.341857 trytoncommunity_setuptools-0.4.0/trytoncommunity_setuptools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3521 2024-04-30 12:56:21.000000 trytoncommunity_setuptools-0.4.0/trytoncommunity_setuptools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      349 2024-04-30 12:56:21.000000 trytoncommunity_setuptools-0.4.0/trytoncommunity_setuptools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 12:56:21.000000 trytoncommunity_setuptools-0.4.0/trytoncommunity_setuptools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-30 12:56:21.000000 trytoncommunity_setuptools-0.4.0/trytoncommunity_setuptools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-30 12:56:21.000000 trytoncommunity_setuptools-0.4.0/trytoncommunity_setuptools.egg-info/top_level.txt
```

### Comparing `trytoncommunity-setuptools-0.3/LICENSE-GPL-3.0.txt` & `trytoncommunity_setuptools-0.4.0/LICENSE-GPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `trytoncommunity-setuptools-0.3/PKG-INFO` & `trytoncommunity_setuptools-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytoncommunity-setuptools
-Version: 0.3
+Version: 0.4.0
 Summary: Shortening the boilerplate in Tryton modules
 Home-page: https://tryton.community
 Author: Hartmut Goebel
 Author-email: h.goebel@crazy-compilers.com
 License: GPL-3.0-or-later
 Project-URL: Source Code, https://foss.heptapod.net/tryton-community/setuptools
 Keywords: tryton,setuptools,package management
@@ -18,14 +18,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE-GPL-3.0.txt
+Requires-Dist: setuptools
 
 ============================
 trytoncommunity-setuptools
 ============================
 
 **Shortening the boilerplate in Tryton modules**
```

### Comparing `trytoncommunity-setuptools-0.3/README.rst` & `trytoncommunity_setuptools-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `trytoncommunity-setuptools-0.3/setup.cfg` & `trytoncommunity_setuptools-0.4.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trytoncommunity-setuptools
-version = 0.3
+version = 0.4.0
 description = Shortening the boilerplate in Tryton modules
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://tryton.community
 author = Hartmut Goebel
 author_email = h.goebel@crazy-compilers.com
 license = GPL-3.0-or-later
@@ -28,20 +28,24 @@
 [options]
 python_requires = >=3.6
 install_requires = 
 	setuptools
 package_dir = 
 	trytoncommunity_setuptools=src
 
-[zest.releaser]
-history-file = CHANGES
-push-changes = no
-tag-format = v{version}
-tag-message = trytoncommunity-setuptools {version}
-tag-signing = yes
-create-wheel = yes
-development-marker = 
+[bumpversion]
+current_version = 0.4.0
+commit = True
+tag = True
+tag_message = trytoncommunity-setuptools {new_version}
+sign_tags = True
+parse = 0.(?P<major>\d+)\.(?P<minor>\d+)
+serialize = 0.{major}.{minor}
+
+[bumpversion:file:setup.cfg]
+search = version = {current_version}
+replace = version = {new_version}
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trytoncommunity-setuptools-0.3/src/__init__.py` & `trytoncommunity_setuptools-0.4.0/src/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     # keep aligned with trytoncommunity-cookiecutter-module
     "6.0": ["3.6", "3.7", "3.8", "3.9"],
     "6.2": ["3.6", "3.7", "3.8", "3.9"],
     "6.4": ["3.7", "3.8", "3.9", "3.10"],
     "6.6": ["3.7", "3.8", "3.9", "3.10"],
     "6.8": ["3.8", "3.9", "3.10", "3.11"],
     "7.0": ["3.8", "3.9", "3.10", "3.11", "3.12"],
+    "7.2": ["3.8", "3.9", "3.10", "3.11", "3.12"],
 }
 
 
 def TrytonCommunityURL(project_path):
     """
     Return a URL string pointing to the 'project_path' within the
     Tryton Community group at heptapod.
@@ -70,21 +71,25 @@
     # content = Path(__file__).with_name(fname).read_text('utf-8')
     content = Path(fname).read_text('utf-8')
     content = re.sub(
         r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
     return content
 
 
-def _get_require_version(name, module2prefix):
+def _get_require_version(name, tryton_version, **kw):
     return '%s == %s.*' % (name, tryton_version)
 
 
-def _get_prefix_require_version(name, module2prefix):
+def _get_prefix_require_version(name, tryton_version, module2prefix):
+    if '-' in name:
+        raise SystemExit("Tryton module names must not contain a dash ('-') "
+                         "to keep them aligned with the names in tryton.cfg: "
+                         "%r" % name)
     name = '%s-%s' % (module2prefix.get(name, 'trytond'), name)
-    return _get_require_version(name, module2prefix)
+    return _get_require_version(name, tryton_version=tryton_version)
 
 
 def get_require_version(name):
     """
     Return a string suitable as a requirement for setuptools with a
     version-specifier matching the Tryton version for the module.
 
@@ -106,37 +111,37 @@
       get_prefix_require_version('sale') -> 'trytond-sale == 6.8.*'
       get_prefix_require_version('country_order')
          -> 'trytoncommunity-country_order == 6.8.*'
     """
     return partial(_get_prefix_require_version, name)
 
 
-def _get_supported_python_versions():
+def _get_supported_python_versions(tryton_version):
     # if the version is not yet defined, use the latest one before
     if tryton_version in SUPPORTED_PYTHON_VERSIONS:
         tv = tryton_version
     else:
         tv = max(v for v in SUPPORTED_PYTHON_VERSIONS if v <= tryton_version)
     return SUPPORTED_PYTHON_VERSIONS[tv]
 
 
-def _get_classifiers():
+def _get_classifiers(tryton_version):
     config = ConfigParser()
     config.read('setup.cfg')  # TODO: which encoding is used for this file?
     classifiers = config.get('metadata', 'classifiers', fallback='')
     if not classifiers:
         # try alias
         classifiers = config.get('metadata', 'classifier', fallback='')
     if 'file:' in classifiers:  # TODO
         raise SystemExit(
             "Reading classifiers from 'file:' is not yet supported")
     classifiers = set(c2 for c1 in classifiers.splitlines()
                       for c2 in c1.split(',') if c2)
     classifiers.update(DEFAULT_CLASSIFIERS)
-    for pyver in _get_supported_python_versions():
+    for pyver in _get_supported_python_versions(tryton_version):
         classifiers.add('Programming Language :: Python :: ' + pyver)
     return list(sorted(classifiers))
 
 
 def __get_metadata_file_or_section(key):
     config = ConfigParser()
     config.read('setup.cfg')  # TODO: which encoding is used for this file?
@@ -166,20 +171,18 @@
     :package_data_patterns: list of file-globs to be added to the
                   package_data entry passed to setuptools.setup()
     :entry_points: (string) passed on to setuptools.setup(),
                   'trytond.modules' will be added automatically
     """
 
     def resolve_requirements(requirements):
-        return [req(module2prefix=module2prefix)
+        return [req(tryton_version=tryton_version, module2prefix=module2prefix)
                 if isinstance(req, partial) else req
                 for req in (requirements or [])]
 
-    global tryton_version
-
     module2prefix = module2prefix or {}
     extras_require = extras_require or {}
 
     config = ConfigParser()
     # config.read_file(open(Path(__file__).with_name('tryton.cfg')))
     config.read_file(open('tryton.cfg'))
     info = dict(config.items('tryton'))
@@ -192,31 +195,32 @@
     # resolve any delayed evaluation in requires and tests_require
     requires = resolve_requirements(requires)
     tests_require = resolve_requirements(tests_require)
 
     # collect dependencies from tryton.cfg
     for dep in info.get('depends', []):
         if not re.match(r'(ir|res)(\W|$)', dep):
-            requires.append(_get_prefix_require_version(dep, module2prefix))
-    requires.append(_get_require_version('trytond', module2prefix))
+            requires.append(_get_prefix_require_version(
+                dep, tryton_version, module2prefix))
+    requires.append(_get_require_version('trytond', tryton_version))
 
     package_data = (
         info.get('xml', [])
         + (package_data_patterns or [])
         + DEFAULT_PACKAGE_DATA_GLOBS)
 
     if not extras_require:
         extras_require = __get_metadata_file_or_section('extras_requires')
     if tests_require:
         if 'test' in extras_require:
             raise SystemExit(
                 """Must only pass one of 'tests_require' or """
                 """'extra_require["tests"]'.""")
         extras_require['test'] = tests_require
-        if _get_supported_python_versions() != '6.0.':
+        if _get_supported_python_versions(tryton_version) != '6.0.':
             # keep the `tests_require` keyword for 6.0 to still allow
             # running the tests using 'python setup.py test'.
             tests_require = None
 
     if not entry_points:
         entry_points = __get_metadata_file_or_section('entry_points')
     elif isinstance(entry_points, str):
@@ -234,23 +238,24 @@
     setuptools.setup(
         name='%s_%s' % (prefix, module),
         version=version,
         long_description=_read_readme('README.rst'),
         install_requires=requires,
         tests_require=tests_require,
         extras_require=extras_require,
-        python_requires='>= %s' % _get_supported_python_versions()[0],
+        python_requires='>= %s' %
+            _get_supported_python_versions(tryton_version)[0],  # noqa: E131
         package_dir={'trytond.modules.%s' % module: '.'},
         packages=(
             ['trytond.modules.%s' % module]
             + ['trytond.modules.%s.%s' % (module, p)
                for p in setuptools.find_packages()]
         ),
         package_data={
             'trytond.modules.%s' % module: package_data,
         },
         include_package_data=True,  # of course we want :-)
         zip_safe=False,  # Tryton only supports file-based access yet
         entry_points=entry_points,
-        classifiers=_get_classifiers(),
+        classifiers=_get_classifiers(tryton_version),
         **kwargs,
     )
```

### Comparing `trytoncommunity-setuptools-0.3/trytoncommunity_setuptools.egg-info/PKG-INFO` & `trytoncommunity_setuptools-0.4.0/trytoncommunity_setuptools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytoncommunity-setuptools
-Version: 0.3
+Version: 0.4.0
 Summary: Shortening the boilerplate in Tryton modules
 Home-page: https://tryton.community
 Author: Hartmut Goebel
 Author-email: h.goebel@crazy-compilers.com
 License: GPL-3.0-or-later
 Project-URL: Source Code, https://foss.heptapod.net/tryton-community/setuptools
 Keywords: tryton,setuptools,package management
@@ -18,14 +18,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE-GPL-3.0.txt
+Requires-Dist: setuptools
 
 ============================
 trytoncommunity-setuptools
 ============================
 
 **Shortening the boilerplate in Tryton modules**
```

