# Comparing `tmp/finitelycomputable-idtrust-app-flask-24.3.tar.gz` & `tmp/finitelycomputable_idtrust_app_flask-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable-idtrust-app-flask-24.3.tar", last modified: Mon Apr  1 03:34:59 2024, max compression
+gzip compressed data, was "finitelycomputable_idtrust_app_flask-24.4.tar", last modified: Tue Apr 30 04:47:17 2024, max compression
```

## Comparing `finitelycomputable-idtrust-app-flask-24.3.tar` & `finitelycomputable_idtrust_app_flask-24.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:59.157023 finitelycomputable-idtrust-app-flask-24.3/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2227 2024-04-01 03:34:59.157023 finitelycomputable-idtrust-app-flask-24.3/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      197 2023-09-12 03:23:48.000000 finitelycomputable-idtrust-app-flask-24.3/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:59.153023 finitelycomputable-idtrust-app-flask-24.3/finitelycomputable/
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)     2972 2024-03-25 18:32:32.000000 finitelycomputable-idtrust-app-flask-24.3/finitelycomputable/idtrust_app_flask.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-01 03:34:59.157023 finitelycomputable-idtrust-app-flask-24.3/finitelycomputable_idtrust_app_flask.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2227 2024-04-01 03:34:59.000000 finitelycomputable-idtrust-app-flask-24.3/finitelycomputable_idtrust_app_flask.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      427 2024-04-01 03:34:59.000000 finitelycomputable-idtrust-app-flask-24.3/finitelycomputable_idtrust_app_flask.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-01 03:34:59.000000 finitelycomputable-idtrust-app-flask-24.3/finitelycomputable_idtrust_app_flask.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       94 2024-04-01 03:34:59.000000 finitelycomputable-idtrust-app-flask-24.3/finitelycomputable_idtrust_app_flask.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      198 2024-04-01 03:34:59.000000 finitelycomputable-idtrust-app-flask-24.3/finitelycomputable_idtrust_app_flask.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-01 03:34:59.000000 finitelycomputable-idtrust-app-flask-24.3/finitelycomputable_idtrust_app_flask.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1828 2024-03-16 18:34:55.000000 finitelycomputable-idtrust-app-flask-24.3/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-01 03:34:59.157023 finitelycomputable-idtrust-app-flask-24.3/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:17.311846 finitelycomputable_idtrust_app_flask-24.4/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2285 2024-04-30 04:47:17.307846 finitelycomputable_idtrust_app_flask-24.4/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      197 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_app_flask-24.4/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:17.307846 finitelycomputable_idtrust_app_flask-24.4/finitelycomputable/
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)     3127 2024-04-25 18:30:53.000000 finitelycomputable_idtrust_app_flask-24.4/finitelycomputable/idtrust_app_flask.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:17.307846 finitelycomputable_idtrust_app_flask-24.4/finitelycomputable/tests/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     8678 2024-04-30 04:36:59.000000 finitelycomputable_idtrust_app_flask-24.4/finitelycomputable/tests/test_idtrust_flask.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:17.307846 finitelycomputable_idtrust_app_flask-24.4/finitelycomputable_idtrust_app_flask.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2285 2024-04-30 04:47:17.000000 finitelycomputable_idtrust_app_flask-24.4/finitelycomputable_idtrust_app_flask.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      474 2024-04-30 04:47:17.000000 finitelycomputable_idtrust_app_flask-24.4/finitelycomputable_idtrust_app_flask.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:47:17.000000 finitelycomputable_idtrust_app_flask-24.4/finitelycomputable_idtrust_app_flask.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       98 2024-04-30 04:47:17.000000 finitelycomputable_idtrust_app_flask-24.4/finitelycomputable_idtrust_app_flask.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      223 2024-04-30 04:47:17.000000 finitelycomputable_idtrust_app_flask-24.4/finitelycomputable_idtrust_app_flask.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:47:17.000000 finitelycomputable_idtrust_app_flask-24.4/finitelycomputable_idtrust_app_flask.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1860 2024-04-28 21:51:18.000000 finitelycomputable_idtrust_app_flask-24.4/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:47:17.311846 finitelycomputable_idtrust_app_flask-24.4/setup.cfg
```

### Comparing `finitelycomputable-idtrust-app-flask-24.3/PKG-INFO` & `finitelycomputable_idtrust_app_flask-24.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-app-flask
-Version: 24.3
+Version: 24.4
 Summary: The Flask-dependent code for a microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -28,14 +28,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: finitelycomputable-idtrust-common
 Requires-Dist: Flask~=3.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
+Requires-Dist: finitelycomputable-tests; extra == "tests"
 Provides-Extra: waitress
 Requires-Dist: waitress~=2.1; extra == "waitress"
 Provides-Extra: cherrypy
 Requires-Dist: cherrypy~=18.0; extra == "cherrypy"
 Provides-Extra: cheroot
 Requires-Dist: cheroot~=9.0; extra == "cheroot"
 Provides-Extra: bjoern
```

### Comparing `finitelycomputable-idtrust-app-flask-24.3/finitelycomputable/idtrust_app_flask.py` & `finitelycomputable_idtrust_app_flask-24.4/finitelycomputable/idtrust_app_flask.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,26 +12,30 @@
 blueprint = Blueprint('idtrust', __name__)
 base_path = join('/', environ.get('BASE_PATH', ''))
 
 
 @blueprint.route('interact/<int:pk>', defaults={'blind': True},
         methods=('GET', 'POST'))
 @blueprint.route('interact/<int:pk>/reveal_miscommunication',
-        methods=('GET', 'POST'))
-def interact(pk, blind=False):
+        defaults={'blind': False}, methods=('GET', 'POST'))
+def interact(pk, blind):
     try:
         interaction = dialog_from_id(pk)
     except:
         flask.abort(flask.Response(f"Dialog {pk} not found.", 404))
     return flask.render_template('interaction.html',
         new_partner_url=flask.url_for(
                 'idtrust.new_dialogue',
                 journey_id=interaction.journey_id,
                 blind=blind),
         new_journey_url=flask.url_for('idtrust.new_dialogue', blind=blind),
+        blind_toggle_url=flask.url_for(
+                'idtrust.interact',
+                pk=pk,
+                blind=not blind),
         **interact_core(
             interaction,
             blind,
             flask.request.form.get('user_intent'),
             flask.request.form.get('user_guess'),
     ))
 
@@ -62,15 +66,15 @@
     obj = create_dialog(
             journey,
             flask.request.form.get('user_miscommunication'),
             flask.request.form.get('foil_miscommunication'),
     )
     interact_core(obj, not blind, flask.request.form.get('user_intent'))
     return flask.redirect(
-            flask.url_for( 'idtrust.interact', pk=obj.id, blind=True)
+            flask.url_for( 'idtrust.interact', pk=obj.id, blind=blind)
     )
 
 application.register_blueprint(blueprint, url_prefix = base_path)
 
 def run():
     from sys import argv, exit, stderr
     if len(argv) < 2 or argv[1] != 'run':
```

### Comparing `finitelycomputable-idtrust-app-flask-24.3/finitelycomputable_idtrust_app_flask.egg-info/PKG-INFO` & `finitelycomputable_idtrust_app_flask-24.4/finitelycomputable_idtrust_app_flask.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-app-flask
-Version: 24.3
+Version: 24.4
 Summary: The Flask-dependent code for a microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
@@ -28,14 +28,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: finitelycomputable-idtrust-common
 Requires-Dist: Flask~=3.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
+Requires-Dist: finitelycomputable-tests; extra == "tests"
 Provides-Extra: waitress
 Requires-Dist: waitress~=2.1; extra == "waitress"
 Provides-Extra: cherrypy
 Requires-Dist: cherrypy~=18.0; extra == "cherrypy"
 Provides-Extra: cheroot
 Requires-Dist: cheroot~=9.0; extra == "cheroot"
 Provides-Extra: bjoern
```

### Comparing `finitelycomputable-idtrust-app-flask-24.3/pyproject.toml` & `finitelycomputable_idtrust_app_flask-24.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 authors = [{name = "Samuel Newbold", email = "sam@rwsh.org"}]
 license = {text = "AGPL-3.0-only"}
 readme = "README.rst"
-version = "24.3"
+version = "24.4"
 name = "finitelycomputable-idtrust-app-flask"
 requires-python = ">=3.8"
 description = "The Flask-dependent code for a microsite to explore identifying game-theory strategies"
 dependencies = [
   "finitelycomputable-idtrust-common",
   "Flask~=3.0",
 ]
@@ -29,23 +29,23 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 
 [project.optional-dependencies]
-tests = ["pytest", "pytest-env"]
+tests = ["pytest", "pytest-env", "finitelycomputable-tests"]
 waitress = ["waitress~=2.1"]
 cherrypy = ["cherrypy~=18.0"]
 cheroot = ["cheroot~=9.0"]
 bjoern = ["bjoern~=3.0"]
 gunicorn = ["gunicorn~=21.2"]
 
 [project.scripts]
-finitelycomputable-idtrust-app-flask = "finitelycomputable.idtrust_flask:run"
+finitelycomputable-idtrust-app-flask = "finitelycomputable.idtrust_app_flask:run"
 
 [project.urls]
 Homepage = "https://www.finitelycomputable.net/identification_of_trust"
 Documentation = "https://github.com/thrasymache/microsites"
 Source = "https://github.com/thrasymache/microsites"
 Gitlab = "https://gitlab.com/thrasymache/microsites"
 sourcehut = "https://git.sr.ht/~thrasymache/finitelycomputable-microsites"
```

