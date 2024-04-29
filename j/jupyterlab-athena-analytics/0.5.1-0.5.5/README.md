# Comparing `tmp/jupyterlab_athena_analytics-0.5.1.tar.gz` & `tmp/jupyterlab_athena_analytics-0.5.5.tar.gz`

## Comparing `jupyterlab_athena_analytics-0.5.1.tar` & `jupyterlab_athena_analytics-0.5.5.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/babel.config.js
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/jest.config.js
--rw-r--r--   0        0        0   356405 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/package-lock.json
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/tsconfig.test.json
--rw-r--r--   0        0        0   369604 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/yarn.lock
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/_version.py
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/labextension/package.json
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/labextension/static/496.0fc234152a8e8b8f31ed.js
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/labextension/static/736.1c2d46418a08bbb03c03.js
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/labextension/static/remoteEntry.b1df3a258d734729eff5.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json
--rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/scripts/build.sh
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/src/.gitignore
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/src/.yarnrc.yml
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/src/index.ts
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/src/__tests__/jupyterlab_athena_analytics.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/style/index.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/ui-tests/yarn.lock
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/ui-tests/tests/jupyterlab_athena_analytics.spec.ts
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/LICENSE
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/README.md
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/CHANGELOG.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/babel.config.js
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/build.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jest.config.js
+-rw-r--r--   0        0        0   357048 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/package-lock.json
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/setup.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/test.ipynb
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/tsconfig.test.json
+-rw-r--r--   0        0        0   374390 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/yarn.lock
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/_version.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/package.json
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/509.68053d43f01f7d268d38.js
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/728.c9fba78fc7d4a52b2765.js
+-rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/remoteEntry.d43dde86f53fb87db6c8.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json
+-rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/scripts/build.sh
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/src/.gitignore
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/src/.yarnrc.yml
+-rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/src/index.ts
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/src/__tests__/jupyterlab_athena_analytics.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/style/index.js
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/ui-tests/tests/jupyterlab_athena_analytics.spec.ts
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/LICENSE
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/README.md
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 jupyterlab_athena_analytics-0.5.5/PKG-INFO
```

### Comparing `jupyterlab_athena_analytics-0.5.1/RELEASE.md` & `jupyterlab_athena_analytics-0.5.5/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.1/jest.config.js` & `jupyterlab_athena_analytics-0.5.5/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.1/package-lock.json` & `jupyterlab_athena_analytics-0.5.5/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8997601141078839%*

 * *Differences: {"'packages'": "{'': {'version': '0.5.1', 'dependencies': {'hatch': '^1.1.0'}}, "*

 * *               "'node_modules/debug': {delete: ['dev']}, 'node_modules/ms': {delete: ['dev']}, "*

 * *               "'node_modules/eve': OrderedDict([('version', '0.5.4'), ('resolved', "*

 * *               "'https://registry.npmjs.org/eve/-/eve-0.5.4.tgz'), ('integrity', "*

 * *               "'sha512-aqprQ9MAOh1t66PrHxDFmMXPlgNO6Uv1uqvxmwjprQV50jaQ2RqO7O1neY4PJwC+hMnkyMDphu2AQPOPZdjQog==')]), "*

 * *               "'node_modules/hatch': Ordere […]*

```diff
@@ -1,14 +1,15 @@
 {
     "lockfileVersion": 3,
     "name": "jupyterlab_athena_analytics",
     "packages": {
         "": {
             "dependencies": {
-                "@jupyterlab/application": "^4.0.0"
+                "@jupyterlab/application": "^4.0.0",
+                "hatch": "^1.1.0"
             },
             "devDependencies": {
                 "@jupyterlab/builder": "^4.0.0",
                 "@jupyterlab/testutils": "^4.0.0",
                 "@types/jest": "^29.2.0",
                 "@types/json-schema": "^7.0.11",
                 "@types/react": "^18.0.26",
@@ -30,15 +31,15 @@
                 "stylelint-config-standard": "^26.0.0",
                 "stylelint-prettier": "^2.0.0",
                 "typescript": "~5.0.2",
                 "yjs": "^13.5.0"
             },
             "license": "BSD-3-Clause",
             "name": "jupyterlab_athena_analytics",
-            "version": "0.4.2",
+            "version": "0.5.1",
             "workspaces": [
                 "workspace/athena-notebooks/jupyterlab_athena_analytics"
             ]
         },
         "node_modules/@aashutoshrathi/word-wrap": {
             "dev": true,
             "engines": {
@@ -5122,15 +5123,14 @@
             "license": "MIT",
             "version": "8.7.0"
         },
         "node_modules/debug": {
             "dependencies": {
                 "ms": "2.1.2"
             },
-            "dev": true,
             "engines": {
                 "node": ">=6.0"
             },
             "license": "MIT",
             "peerDependenciesMeta": {
                 "supports-color": {
                     "optional": true
@@ -5893,14 +5893,19 @@
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "license": "BSD-2-Clause",
             "version": "2.0.3"
         },
+        "node_modules/eve": {
+            "integrity": "sha512-aqprQ9MAOh1t66PrHxDFmMXPlgNO6Uv1uqvxmwjprQV50jaQ2RqO7O1neY4PJwC+hMnkyMDphu2AQPOPZdjQog==",
+            "resolved": "https://registry.npmjs.org/eve/-/eve-0.5.4.tgz",
+            "version": "0.5.4"
+        },
         "node_modules/events": {
             "dev": true,
             "engines": {
                 "node": ">=0.8.x"
             },
             "license": "MIT",
             "version": "3.3.0"
@@ -6467,14 +6472,23 @@
             "dev": true,
             "engines": {
                 "node": ">= 0.4"
             },
             "license": "MIT",
             "version": "2.0.0"
         },
+        "node_modules/hatch": {
+            "dependencies": {
+                "debug": "^4.1.0",
+                "eve": "^0.5.4"
+            },
+            "integrity": "sha512-F+DZQshKh1r05q6Jo/KsqinJIDv4nqCdI/qcjZyqjnIGE9+uBEFknJ6k98v9xl0XDveeWyvU4PoHnhF1VglXnQ==",
+            "resolved": "https://registry.npmjs.org/hatch/-/hatch-1.1.0.tgz",
+            "version": "1.1.0"
+        },
         "node_modules/hosted-git-info": {
             "dev": true,
             "license": "ISC",
             "version": "2.8.9"
         },
         "node_modules/html-encoding-sniffer": {
             "dependencies": {
@@ -8328,15 +8342,14 @@
             "engines": {
                 "node": ">=10"
             },
             "license": "MIT",
             "version": "1.0.4"
         },
         "node_modules/ms": {
-            "dev": true,
             "license": "MIT",
             "version": "2.1.2"
         },
         "node_modules/nanoid": {
             "bin": {
                 "nanoid": "bin/nanoid.cjs"
             },
@@ -11213,9 +11226,9 @@
                 "url": "https://github.com/sponsors/sindresorhus"
             },
             "license": "MIT",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "0.4.2"
+    "version": "0.5.1"
 }
```

### Comparing `jupyterlab_athena_analytics-0.5.1/package.json` & `jupyterlab_athena_analytics-0.5.5/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9711538461538461%*

 * *Differences: {"'dependencies'": "{'hatch': '^1.1.0'}", "'version'": "'0.5.5'"}*

```diff
@@ -3,15 +3,16 @@
         "email": "team@athenaintelligence.ai",
         "name": "Athena Intelligence"
     },
     "bugs": {
         "url": "https://github.com/github_username/jupyterlab_athena_analytics/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^4.0.0"
+        "@jupyterlab/application": "^4.0.0",
+        "hatch": "^1.1.0"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
@@ -172,12 +173,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.5.1",
+    "version": "0.5.5",
     "workspaces": [
         "workspace/athena-notebooks/jupyterlab_athena_analytics"
     ]
 }
```

### Comparing `jupyterlab_athena_analytics-0.5.1/tsconfig.json` & `jupyterlab_athena_analytics-0.5.5/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.1/yarn.lock` & `jupyterlab_athena_analytics-0.5.5/yarn.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,73 @@
 # This file is generated by running "yarn install" inside your project.
 # Manual changes might be lost - proceed with caution!
 
 __metadata:
   version: 6
   cacheKey: 8
 
-"@aashutoshrathi/word-wrap@npm:^1.2.3":
-  version: 1.2.6
-  resolution: "@aashutoshrathi/word-wrap@npm:1.2.6"
-  checksum: ada901b9e7c680d190f1d012c84217ce0063d8f5c5a7725bb91ec3c5ed99bb7572680eb2d2938a531ccbaec39a95422fcd8a6b4a13110c7d98dd75402f66a0cd
-  languageName: node
-  linkType: hard
-
 "@ampproject/remapping@npm:^2.2.0":
-  version: 2.2.1
-  resolution: "@ampproject/remapping@npm:2.2.1"
+  version: 2.3.0
+  resolution: "@ampproject/remapping@npm:2.3.0"
   dependencies:
-    "@jridgewell/gen-mapping": ^0.3.0
-    "@jridgewell/trace-mapping": ^0.3.9
-  checksum: 03c04fd526acc64a1f4df22651186f3e5ef0a9d6d6530ce4482ec9841269cf7a11dbb8af79237c282d721c5312024ff17529cd72cc4768c11e999b58e2302079
+    "@jridgewell/gen-mapping": ^0.3.5
+    "@jridgewell/trace-mapping": ^0.3.24
+  checksum: d3ad7b89d973df059c4e8e6d7c972cbeb1bb2f18f002a3bd04ae0707da214cb06cc06929b65aa2313b9347463df2914772298bae8b1d7973f246bb3f2ab3e8f0
   languageName: node
   linkType: hard
 
-"@babel/code-frame@npm:^7.0.0, @babel/code-frame@npm:^7.12.13, @babel/code-frame@npm:^7.23.5":
-  version: 7.23.5
-  resolution: "@babel/code-frame@npm:7.23.5"
+"@babel/code-frame@npm:^7.0.0, @babel/code-frame@npm:^7.12.13, @babel/code-frame@npm:^7.23.5, @babel/code-frame@npm:^7.24.2":
+  version: 7.24.2
+  resolution: "@babel/code-frame@npm:7.24.2"
   dependencies:
-    "@babel/highlight": ^7.23.4
-    chalk: ^2.4.2
-  checksum: d90981fdf56a2824a9b14d19a4c0e8db93633fd488c772624b4e83e0ceac6039a27cd298a247c3214faa952bf803ba23696172ae7e7235f3b97f43ba278c569a
+    "@babel/highlight": ^7.24.2
+    picocolors: ^1.0.0
+  checksum: 70e867340cfe09ca5488b2f36372c45cabf43c79a5b6426e6df5ef0611ff5dfa75a57dda841895693de6008f32c21a7c97027a8c7bcabd63a7d17416cbead6f8
   languageName: node
   linkType: hard
 
-"@babel/compat-data@npm:^7.22.6, @babel/compat-data@npm:^7.23.3, @babel/compat-data@npm:^7.23.5":
-  version: 7.23.5
-  resolution: "@babel/compat-data@npm:7.23.5"
-  checksum: 06ce244cda5763295a0ea924728c09bae57d35713b675175227278896946f922a63edf803c322f855a3878323d48d0255a2a3023409d2a123483c8a69ebb4744
+"@babel/compat-data@npm:^7.22.6, @babel/compat-data@npm:^7.23.5, @babel/compat-data@npm:^7.24.4":
+  version: 7.24.4
+  resolution: "@babel/compat-data@npm:7.24.4"
+  checksum: 52ce371658dc7796c9447c9cb3b9c0659370d141b76997f21c5e0028cca4d026ca546b84bc8d157ce7ca30bd353d89f9238504eb8b7aefa9b1f178b4c100c2d4
   languageName: node
   linkType: hard
 
-"@babel/core@npm:^7.10.2, @babel/core@npm:^7.11.6, @babel/core@npm:^7.12.3":
-  version: 7.23.9
-  resolution: "@babel/core@npm:7.23.9"
+"@babel/core@npm:^7.10.2, @babel/core@npm:^7.11.6, @babel/core@npm:^7.12.3, @babel/core@npm:^7.23.9":
+  version: 7.24.5
+  resolution: "@babel/core@npm:7.24.5"
   dependencies:
     "@ampproject/remapping": ^2.2.0
-    "@babel/code-frame": ^7.23.5
-    "@babel/generator": ^7.23.6
+    "@babel/code-frame": ^7.24.2
+    "@babel/generator": ^7.24.5
     "@babel/helper-compilation-targets": ^7.23.6
-    "@babel/helper-module-transforms": ^7.23.3
-    "@babel/helpers": ^7.23.9
-    "@babel/parser": ^7.23.9
-    "@babel/template": ^7.23.9
-    "@babel/traverse": ^7.23.9
-    "@babel/types": ^7.23.9
+    "@babel/helper-module-transforms": ^7.24.5
+    "@babel/helpers": ^7.24.5
+    "@babel/parser": ^7.24.5
+    "@babel/template": ^7.24.0
+    "@babel/traverse": ^7.24.5
+    "@babel/types": ^7.24.5
     convert-source-map: ^2.0.0
     debug: ^4.1.0
     gensync: ^1.0.0-beta.2
     json5: ^2.2.3
     semver: ^6.3.1
-  checksum: 634a511f74db52a5f5a283c1121f25e2227b006c095b84a02a40a9213842489cd82dc7d61cdc74e10b5bcd9bb0a4e28bab47635b54c7e2256d47ab57356e2a76
+  checksum: f4f0eafde12b145f2cb9cc893085e5f1436e1ef265bb3b7d8aa6282515c9b4e740bbd5e2cbc32114adb9afed2dd62c2336758b9fabb7e46e8ba542f76d4f3f80
   languageName: node
   linkType: hard
 
-"@babel/generator@npm:^7.23.6, @babel/generator@npm:^7.7.2":
-  version: 7.23.6
-  resolution: "@babel/generator@npm:7.23.6"
+"@babel/generator@npm:^7.24.5, @babel/generator@npm:^7.7.2":
+  version: 7.24.5
+  resolution: "@babel/generator@npm:7.24.5"
   dependencies:
-    "@babel/types": ^7.23.6
-    "@jridgewell/gen-mapping": ^0.3.2
-    "@jridgewell/trace-mapping": ^0.3.17
+    "@babel/types": ^7.24.5
+    "@jridgewell/gen-mapping": ^0.3.5
+    "@jridgewell/trace-mapping": ^0.3.25
     jsesc: ^2.5.1
-  checksum: 1a1a1c4eac210f174cd108d479464d053930a812798e09fee069377de39a893422df5b5b146199ead7239ae6d3a04697b45fc9ac6e38e0f6b76374390f91fc6c
+  checksum: a08c0ab900b36e1a17863e18e3216153322ea993246fd7a358ba38a31cfb15bab2af1dc178b2adafe4cb8a9f3ab0e0ceafd3fe6e8ca870dffb435b53b2b2a803
   languageName: node
   linkType: hard
 
 "@babel/helper-annotate-as-pure@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-annotate-as-pure@npm:7.22.5"
   dependencies:
@@ -88,43 +81,43 @@
   resolution: "@babel/helper-builder-binary-assignment-operator-visitor@npm:7.22.15"
   dependencies:
     "@babel/types": ^7.22.15
   checksum: 639c697a1c729f9fafa2dd4c9af2e18568190299b5907bd4c2d0bc818fcbd1e83ffeecc2af24327a7faa7ac4c34edd9d7940510a5e66296c19bad17001cf5c7a
   languageName: node
   linkType: hard
 
-"@babel/helper-compilation-targets@npm:^7.22.15, @babel/helper-compilation-targets@npm:^7.22.6, @babel/helper-compilation-targets@npm:^7.23.6":
+"@babel/helper-compilation-targets@npm:^7.22.6, @babel/helper-compilation-targets@npm:^7.23.6":
   version: 7.23.6
   resolution: "@babel/helper-compilation-targets@npm:7.23.6"
   dependencies:
     "@babel/compat-data": ^7.23.5
     "@babel/helper-validator-option": ^7.23.5
     browserslist: ^4.22.2
     lru-cache: ^5.1.1
     semver: ^6.3.1
   checksum: c630b98d4527ac8fe2c58d9a06e785dfb2b73ec71b7c4f2ddf90f814b5f75b547f3c015f110a010fd31f76e3864daaf09f3adcd2f6acdbfb18a8de3a48717590
   languageName: node
   linkType: hard
 
-"@babel/helper-create-class-features-plugin@npm:^7.22.15":
-  version: 7.23.10
-  resolution: "@babel/helper-create-class-features-plugin@npm:7.23.10"
+"@babel/helper-create-class-features-plugin@npm:^7.24.1, @babel/helper-create-class-features-plugin@npm:^7.24.4, @babel/helper-create-class-features-plugin@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-create-class-features-plugin@npm:7.24.5"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
     "@babel/helper-environment-visitor": ^7.22.20
     "@babel/helper-function-name": ^7.23.0
-    "@babel/helper-member-expression-to-functions": ^7.23.0
+    "@babel/helper-member-expression-to-functions": ^7.24.5
     "@babel/helper-optimise-call-expression": ^7.22.5
-    "@babel/helper-replace-supers": ^7.22.20
+    "@babel/helper-replace-supers": ^7.24.1
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
-    "@babel/helper-split-export-declaration": ^7.22.6
+    "@babel/helper-split-export-declaration": ^7.24.5
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: ff0730c21f0e73b9e314701bca6568bb5885dff2aa3c32b1e2e3d18ed2818f56851b9ffdbe2e8008c9bb94b265a1443883ae4c1ca5dde278ce71ac4218006d68
+  checksum: ea761c1155442620ee02920ec7c3190f869ff4d4fcab48a021a11fd8a46c046ed1facb070e5c76539c2b7efc2c8338f50f08a5e49d0ebf12e48743570e92247b
   languageName: node
   linkType: hard
 
 "@babel/helper-create-regexp-features-plugin@npm:^7.18.6, @babel/helper-create-regexp-features-plugin@npm:^7.22.15, @babel/helper-create-regexp-features-plugin@npm:^7.22.5":
   version: 7.22.15
   resolution: "@babel/helper-create-regexp-features-plugin@npm:7.22.15"
   dependencies:
@@ -133,37 +126,37 @@
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: 0243b8d4854f1dc8861b1029a46d3f6393ad72f366a5a08e36a4648aa682044f06da4c6e87a456260e1e1b33c999f898ba591a0760842c1387bcc93fbf2151a6
   languageName: node
   linkType: hard
 
-"@babel/helper-define-polyfill-provider@npm:^0.5.0":
-  version: 0.5.0
-  resolution: "@babel/helper-define-polyfill-provider@npm:0.5.0"
+"@babel/helper-define-polyfill-provider@npm:^0.6.1, @babel/helper-define-polyfill-provider@npm:^0.6.2":
+  version: 0.6.2
+  resolution: "@babel/helper-define-polyfill-provider@npm:0.6.2"
   dependencies:
     "@babel/helper-compilation-targets": ^7.22.6
     "@babel/helper-plugin-utils": ^7.22.5
     debug: ^4.1.1
     lodash.debounce: ^4.0.8
     resolve: ^1.14.2
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: d24626b819d3875cb65189d761004e9230f2b3fb60542525c4785616f4b2366741369235a864b744f54beb26d625ae4b0af0c9bb3306b61bf4fccb61e0620020
+  checksum: 2bba965ea9a4887ddf9c11d51d740ab473bd7597b787d042c325f6a45912dfe908c2d6bb1d837bf82f7e9fa51e6ad5150563c58131d2bb85515e63d971414a9c
   languageName: node
   linkType: hard
 
 "@babel/helper-environment-visitor@npm:^7.22.20":
   version: 7.22.20
   resolution: "@babel/helper-environment-visitor@npm:7.22.20"
   checksum: d80ee98ff66f41e233f36ca1921774c37e88a803b2f7dca3db7c057a5fea0473804db9fb6729e5dbfd07f4bed722d60f7852035c2c739382e84c335661590b69
   languageName: node
   linkType: hard
 
-"@babel/helper-function-name@npm:^7.22.5, @babel/helper-function-name@npm:^7.23.0":
+"@babel/helper-function-name@npm:^7.23.0":
   version: 7.23.0
   resolution: "@babel/helper-function-name@npm:7.23.0"
   dependencies:
     "@babel/template": ^7.22.15
     "@babel/types": ^7.23.0
   checksum: e44542257b2d4634a1f979244eb2a4ad8e6d75eb6761b4cfceb56b562f7db150d134bc538c8e6adca3783e3bc31be949071527aa8e3aab7867d1ad2d84a26e10
   languageName: node
@@ -174,60 +167,60 @@
   resolution: "@babel/helper-hoist-variables@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: 394ca191b4ac908a76e7c50ab52102669efe3a1c277033e49467913c7ed6f7c64d7eacbeabf3bed39ea1f41731e22993f763b1edce0f74ff8563fd1f380d92cc
   languageName: node
   linkType: hard
 
-"@babel/helper-member-expression-to-functions@npm:^7.22.15, @babel/helper-member-expression-to-functions@npm:^7.23.0":
-  version: 7.23.0
-  resolution: "@babel/helper-member-expression-to-functions@npm:7.23.0"
+"@babel/helper-member-expression-to-functions@npm:^7.23.0, @babel/helper-member-expression-to-functions@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-member-expression-to-functions@npm:7.24.5"
   dependencies:
-    "@babel/types": ^7.23.0
-  checksum: 494659361370c979ada711ca685e2efe9460683c36db1b283b446122596602c901e291e09f2f980ecedfe6e0f2bd5386cb59768285446530df10c14df1024e75
+    "@babel/types": ^7.24.5
+  checksum: d3ad681655128463aa5c2a239345687345f044542563506ee53c9636d147e97f93a470be320950a8ba5f497ade6b27a8136a3a681794867ff94b90060a6e427c
   languageName: node
   linkType: hard
 
-"@babel/helper-module-imports@npm:^7.22.15":
-  version: 7.22.15
-  resolution: "@babel/helper-module-imports@npm:7.22.15"
+"@babel/helper-module-imports@npm:^7.24.1, @babel/helper-module-imports@npm:^7.24.3":
+  version: 7.24.3
+  resolution: "@babel/helper-module-imports@npm:7.24.3"
   dependencies:
-    "@babel/types": ^7.22.15
-  checksum: ecd7e457df0a46f889228f943ef9b4a47d485d82e030676767e6a2fdcbdaa63594d8124d4b55fd160b41c201025aec01fc27580352b1c87a37c9c6f33d116702
+    "@babel/types": ^7.24.0
+  checksum: c23492189ba97a1ec7d37012336a5661174e8b88194836b6bbf90d13c3b72c1db4626263c654454986f924c6da8be7ba7f9447876d709cd00bd6ffde6ec00796
   languageName: node
   linkType: hard
 
-"@babel/helper-module-transforms@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/helper-module-transforms@npm:7.23.3"
+"@babel/helper-module-transforms@npm:^7.23.3, @babel/helper-module-transforms@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-module-transforms@npm:7.24.5"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.20
-    "@babel/helper-module-imports": ^7.22.15
-    "@babel/helper-simple-access": ^7.22.5
-    "@babel/helper-split-export-declaration": ^7.22.6
-    "@babel/helper-validator-identifier": ^7.22.20
+    "@babel/helper-module-imports": ^7.24.3
+    "@babel/helper-simple-access": ^7.24.5
+    "@babel/helper-split-export-declaration": ^7.24.5
+    "@babel/helper-validator-identifier": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 5d0895cfba0e16ae16f3aa92fee108517023ad89a855289c4eb1d46f7aef4519adf8e6f971e1d55ac20c5461610e17213f1144097a8f932e768a9132e2278d71
+  checksum: 208c2e3877536c367ae3f39345bb5c5954ad481fdb2204d4d1906063e53ae564e5b7b846951b1aa96ee716ec24ec3b6db01b41d128884c27315b415f62db9fd2
   languageName: node
   linkType: hard
 
 "@babel/helper-optimise-call-expression@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-optimise-call-expression@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: c70ef6cc6b6ed32eeeec4482127e8be5451d0e5282d5495d5d569d39eb04d7f1d66ec99b327f45d1d5842a9ad8c22d48567e93fc502003a47de78d122e355f7c
   languageName: node
   linkType: hard
 
-"@babel/helper-plugin-utils@npm:^7.0.0, @babel/helper-plugin-utils@npm:^7.10.4, @babel/helper-plugin-utils@npm:^7.12.13, @babel/helper-plugin-utils@npm:^7.14.5, @babel/helper-plugin-utils@npm:^7.18.6, @babel/helper-plugin-utils@npm:^7.22.5, @babel/helper-plugin-utils@npm:^7.8.0, @babel/helper-plugin-utils@npm:^7.8.3":
-  version: 7.22.5
-  resolution: "@babel/helper-plugin-utils@npm:7.22.5"
-  checksum: c0fc7227076b6041acd2f0e818145d2e8c41968cc52fb5ca70eed48e21b8fe6dd88a0a91cbddf4951e33647336eb5ae184747ca706817ca3bef5e9e905151ff5
+"@babel/helper-plugin-utils@npm:^7.0.0, @babel/helper-plugin-utils@npm:^7.10.4, @babel/helper-plugin-utils@npm:^7.12.13, @babel/helper-plugin-utils@npm:^7.14.5, @babel/helper-plugin-utils@npm:^7.18.6, @babel/helper-plugin-utils@npm:^7.22.5, @babel/helper-plugin-utils@npm:^7.24.0, @babel/helper-plugin-utils@npm:^7.24.5, @babel/helper-plugin-utils@npm:^7.8.0, @babel/helper-plugin-utils@npm:^7.8.3":
+  version: 7.24.5
+  resolution: "@babel/helper-plugin-utils@npm:7.24.5"
+  checksum: fa1450c92541b32fe18a6ae85e5c989296a284838fa0a282a2138732cae6f173f36d39dc724890c1740ae72d6d6fbca0b009916b168d4bc874bacc7e5c2fdce0
   languageName: node
   linkType: hard
 
 "@babel/helper-remap-async-to-generator@npm:^7.22.20":
   version: 7.22.20
   resolution: "@babel/helper-remap-async-to-generator@npm:7.22.20"
   dependencies:
@@ -236,150 +229,163 @@
     "@babel/helper-wrap-function": ^7.22.20
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: 2fe6300a6f1b58211dffa0aed1b45d4958506d096543663dba83bd9251fe8d670fa909143a65b45e72acb49e7e20fbdb73eae315d9ddaced467948c3329986e7
   languageName: node
   linkType: hard
 
-"@babel/helper-replace-supers@npm:^7.22.20":
-  version: 7.22.20
-  resolution: "@babel/helper-replace-supers@npm:7.22.20"
+"@babel/helper-replace-supers@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/helper-replace-supers@npm:7.24.1"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.20
-    "@babel/helper-member-expression-to-functions": ^7.22.15
+    "@babel/helper-member-expression-to-functions": ^7.23.0
     "@babel/helper-optimise-call-expression": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: a0008332e24daedea2e9498733e3c39b389d6d4512637e000f96f62b797e702ee24a407ccbcd7a236a551590a38f31282829a8ef35c50a3c0457d88218cae639
+  checksum: c04182c34a3195c6396de2f2945f86cb60daa94ca7392db09bd8b0d4e7a15b02fbe1947c70f6062c87eadaea6d7135207129efa35cf458ea0987bab8c0f02d5a
   languageName: node
   linkType: hard
 
-"@babel/helper-simple-access@npm:^7.22.5":
-  version: 7.22.5
-  resolution: "@babel/helper-simple-access@npm:7.22.5"
+"@babel/helper-simple-access@npm:^7.22.5, @babel/helper-simple-access@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-simple-access@npm:7.24.5"
   dependencies:
-    "@babel/types": ^7.22.5
-  checksum: fe9686714caf7d70aedb46c3cce090f8b915b206e09225f1e4dbc416786c2fdbbee40b38b23c268b7ccef749dd2db35f255338fb4f2444429874d900dede5ad2
+    "@babel/types": ^7.24.5
+  checksum: 5616044603c98434342f09b056c869394acdeba7cd9ec29e6a9abb0dae1922f779d364aaba74dc2ae4facf85945c6156295adbe0511a8aaecaa8a1559d14757a
   languageName: node
   linkType: hard
 
 "@babel/helper-skip-transparent-expression-wrappers@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/helper-skip-transparent-expression-wrappers@npm:7.22.5"
   dependencies:
     "@babel/types": ^7.22.5
   checksum: 1012ef2295eb12dc073f2b9edf3425661e9b8432a3387e62a8bc27c42963f1f216ab3124228015c748770b2257b4f1fda882ca8fa34c0bf485e929ae5bc45244
   languageName: node
   linkType: hard
 
-"@babel/helper-split-export-declaration@npm:^7.22.6":
-  version: 7.22.6
-  resolution: "@babel/helper-split-export-declaration@npm:7.22.6"
+"@babel/helper-split-export-declaration@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-split-export-declaration@npm:7.24.5"
   dependencies:
-    "@babel/types": ^7.22.5
-  checksum: e141cace583b19d9195f9c2b8e17a3ae913b7ee9b8120246d0f9ca349ca6f03cb2c001fd5ec57488c544347c0bb584afec66c936511e447fd20a360e591ac921
+    "@babel/types": ^7.24.5
+  checksum: f23ab6942568084a57789462ce55dc9631aef1d2142ffa2ee28fc411ab55ed3ca65adf109e48655aa349bf8df7ca6dd81fd91c8c229fee1dc77e283189dc83c2
   languageName: node
   linkType: hard
 
-"@babel/helper-string-parser@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/helper-string-parser@npm:7.23.4"
-  checksum: c0641144cf1a7e7dc93f3d5f16d5327465b6cf5d036b48be61ecba41e1eece161b48f46b7f960951b67f8c3533ce506b16dece576baef4d8b3b49f8c65410f90
+"@babel/helper-string-parser@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/helper-string-parser@npm:7.24.1"
+  checksum: 8404e865b06013979a12406aab4c0e8d2e377199deec09dfe9f57b833b0c9ce7b6e8c1c553f2da8d0bcd240c5005bd7a269f4fef0d628aeb7d5fe035c436fb67
   languageName: node
   linkType: hard
 
-"@babel/helper-validator-identifier@npm:^7.22.20":
-  version: 7.22.20
-  resolution: "@babel/helper-validator-identifier@npm:7.22.20"
-  checksum: 136412784d9428266bcdd4d91c32bcf9ff0e8d25534a9d94b044f77fe76bc50f941a90319b05aafd1ec04f7d127cd57a179a3716009ff7f3412ef835ada95bdc
+"@babel/helper-validator-identifier@npm:^7.22.20, @babel/helper-validator-identifier@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helper-validator-identifier@npm:7.24.5"
+  checksum: 75d6f9f475c08f3be87bae4953e9b8d8c72983e16ed2860870b328d048cb20dccb4fcbf85eacbdd817ea1efbb38552a6db9046e2e37bfe13bdec44ac8939024c
   languageName: node
   linkType: hard
 
 "@babel/helper-validator-option@npm:^7.23.5":
   version: 7.23.5
   resolution: "@babel/helper-validator-option@npm:7.23.5"
   checksum: 537cde2330a8aede223552510e8a13e9c1c8798afee3757995a7d4acae564124fe2bf7e7c3d90d62d3657434a74340a274b3b3b1c6f17e9a2be1f48af29cb09e
   languageName: node
   linkType: hard
 
 "@babel/helper-wrap-function@npm:^7.22.20":
-  version: 7.22.20
-  resolution: "@babel/helper-wrap-function@npm:7.22.20"
+  version: 7.24.5
+  resolution: "@babel/helper-wrap-function@npm:7.24.5"
   dependencies:
-    "@babel/helper-function-name": ^7.22.5
-    "@babel/template": ^7.22.15
-    "@babel/types": ^7.22.19
-  checksum: 221ed9b5572612aeb571e4ce6a256f2dee85b3c9536f1dd5e611b0255e5f59a3d0ec392d8d46d4152149156a8109f92f20379b1d6d36abb613176e0e33f05fca
+    "@babel/helper-function-name": ^7.23.0
+    "@babel/template": ^7.24.0
+    "@babel/types": ^7.24.5
+  checksum: c895b95f0fd5e070ced93f315f85e3b63a7236dc9c302bbdce87c699e599d3fd6ad6e44cc820ec7df2d60fadbc922b3b59a0318b708fe69e3d01e5ed15687876
   languageName: node
   linkType: hard
 
-"@babel/helpers@npm:^7.23.9":
-  version: 7.23.9
-  resolution: "@babel/helpers@npm:7.23.9"
+"@babel/helpers@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/helpers@npm:7.24.5"
   dependencies:
-    "@babel/template": ^7.23.9
-    "@babel/traverse": ^7.23.9
-    "@babel/types": ^7.23.9
-  checksum: 2678231192c0471dbc2fc403fb19456cc46b1afefcfebf6bc0f48b2e938fdb0fef2e0fe90c8c8ae1f021dae5012b700372e4b5d15867f1d7764616532e4a6324
+    "@babel/template": ^7.24.0
+    "@babel/traverse": ^7.24.5
+    "@babel/types": ^7.24.5
+  checksum: 941937456ca50ef44dbc5cdcb9a74c6ce18ce38971663acd80b622e7ecf1cc4fa034597de3ccccc37939d324139f159709f493fd8e7c385adbc162cb0888cfee
   languageName: node
   linkType: hard
 
-"@babel/highlight@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/highlight@npm:7.23.4"
+"@babel/highlight@npm:^7.24.2":
+  version: 7.24.5
+  resolution: "@babel/highlight@npm:7.24.5"
   dependencies:
-    "@babel/helper-validator-identifier": ^7.22.20
+    "@babel/helper-validator-identifier": ^7.24.5
     chalk: ^2.4.2
     js-tokens: ^4.0.0
-  checksum: 643acecdc235f87d925979a979b539a5d7d1f31ae7db8d89047269082694122d11aa85351304c9c978ceeb6d250591ccadb06c366f358ccee08bb9c122476b89
+    picocolors: ^1.0.0
+  checksum: eece0e63e9210e902f1ee88f15cabfa31d2693bd2e56806eb849478b859d274c24477081c649cee6a241c4aed7da6f3e05c7afa5c3cd70094006ed095292b0d0
   languageName: node
   linkType: hard
 
-"@babel/parser@npm:^7.1.0, @babel/parser@npm:^7.14.7, @babel/parser@npm:^7.20.7, @babel/parser@npm:^7.23.9":
-  version: 7.23.9
-  resolution: "@babel/parser@npm:7.23.9"
+"@babel/parser@npm:^7.1.0, @babel/parser@npm:^7.14.7, @babel/parser@npm:^7.20.7, @babel/parser@npm:^7.23.9, @babel/parser@npm:^7.24.0, @babel/parser@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/parser@npm:7.24.5"
   bin:
     parser: ./bin/babel-parser.js
-  checksum: e7cd4960ac8671774e13803349da88d512f9292d7baa952173260d3e8f15620a28a3701f14f709d769209022f9e7b79965256b8be204fc550cfe783cdcabe7c7
+  checksum: a251ea41bf8b5f61048beb320d43017aff68af5a3506bd2ef392180f5fa32c1061513171d582bb3d46ea48e3659dece8b3ba52511a2566066e58abee300ce2a0
   languageName: node
   linkType: hard
 
-"@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:7.23.3"
+"@babel/plugin-bugfix-firefox-class-in-computed-class-key@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-bugfix-firefox-class-in-computed-class-key@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-environment-visitor": ^7.22.20
+    "@babel/helper-plugin-utils": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: ddbaf2c396b7780f15e80ee01d6dd790db076985f3dfeb6527d1a8d4cacf370e49250396a3aa005b2c40233cac214a106232f83703d5e8491848bde273938232
+  checksum: d9921b3561762b8c7227cfbf1591436d2a12b99472993a7ce382123e88d98cb359952fbc64d66b1a492187d283d02f51e707f524b708c91b9ab82fb2659eae13
   languageName: node
   linkType: hard
 
-"@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:7.23.3"
+"@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
+  peerDependencies:
+    "@babel/core": ^7.0.0
+  checksum: ec5fddc8db6de0e0082a883f21141d6f4f9f9f0bc190d662a732b5e9a506aae5d7d2337049a1bf055d7cb7add6f128036db6d4f47de5e9ac1be29e043c8b7ca8
+  languageName: node
+  linkType: hard
+
+"@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:7.24.1"
+  dependencies:
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
-    "@babel/plugin-transform-optional-chaining": ^7.23.3
+    "@babel/plugin-transform-optional-chaining": ^7.24.1
   peerDependencies:
     "@babel/core": ^7.13.0
-  checksum: 434b9d710ae856fa1a456678cc304fbc93915af86d581ee316e077af746a709a741ea39d7e1d4f5b98861b629cc7e87f002d3138f5e836775632466d4c74aef2
+  checksum: e18235463e716ac2443938aaec3c18b40c417a1746fba0fa4c26cf4d71326b76ef26c002081ab1b445abfae98e063d561519aa55672dddc1ef80b3940211ffbb
   languageName: node
   linkType: hard
 
-"@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly@npm:^7.23.7":
-  version: 7.23.7
-  resolution: "@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly@npm:7.23.7"
+"@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly@npm:7.24.1"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.20
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: f88e400b548202a6f8c5dfd25bc4949a13ea1ccb64a170d7dea4deaa655a0fcb001d3fd61c35e1ad9c09a3d5f0d43f783400425471fe6d660ccaf33dabea9aba
+  checksum: b5e5889ce5ef51e813e3063cd548f55eb3c88e925c3c08913f334e15d62496861e538ae52a3974e0c56a3044ed8fd5033faea67a64814324af56edc9865b7359
   languageName: node
   linkType: hard
 
 "@babel/plugin-proposal-private-property-in-object@npm:7.21.0-placeholder-for-preset-env.2":
   version: 7.21.0-placeholder-for-preset-env.2
   resolution: "@babel/plugin-proposal-private-property-in-object@npm:7.21.0-placeholder-for-preset-env.2"
   peerDependencies:
@@ -450,33 +456,33 @@
     "@babel/helper-plugin-utils": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: 85740478be5b0de185228e7814451d74ab8ce0a26fcca7613955262a26e99e8e15e9da58f60c754b84515d4c679b590dbd3f2148f0f58025f4ae706f1c5a5d4a
   languageName: node
   linkType: hard
 
-"@babel/plugin-syntax-import-assertions@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-syntax-import-assertions@npm:7.23.3"
+"@babel/plugin-syntax-import-assertions@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-syntax-import-assertions@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 883e6b35b2da205138caab832d54505271a3fee3fc1e8dc0894502434fc2b5d517cbe93bbfbfef8068a0fb6ec48ebc9eef3f605200a489065ba43d8cddc1c9a7
+  checksum: 2a463928a63b62052e9fb8f8b0018aa11a926e94f32c168260ae012afe864875c6176c6eb361e13f300542c31316dad791b08a5b8ed92436a3095c7a0e4fce65
   languageName: node
   linkType: hard
 
-"@babel/plugin-syntax-import-attributes@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-syntax-import-attributes@npm:7.23.3"
+"@babel/plugin-syntax-import-attributes@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-syntax-import-attributes@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 9aed7661ffb920ca75df9f494757466ca92744e43072e0848d87fa4aa61a3f2ee5a22198ac1959856c036434b5614a8f46f1fb70298835dbe28220cdd1d4c11e
+  checksum: 87c8aa4a5ef931313f956871b27f2c051556f627b97ed21e9a5890ca4906b222d89062a956cde459816f5e0dec185ff128d7243d3fdc389504522acb88f0464e
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-import-meta@npm:^7.10.4, @babel/plugin-syntax-import-meta@npm:^7.8.3":
   version: 7.10.4
   resolution: "@babel/plugin-syntax-import-meta@npm:7.10.4"
   dependencies:
@@ -495,21 +501,21 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: bf5aea1f3188c9a507e16efe030efb996853ca3cadd6512c51db7233cc58f3ac89ff8c6bdfb01d30843b161cfe7d321e1bf28da82f7ab8d7e6bc5464666f354a
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-jsx@npm:^7.7.2":
-  version: 7.23.3
-  resolution: "@babel/plugin-syntax-jsx@npm:7.23.3"
+  version: 7.24.1
+  resolution: "@babel/plugin-syntax-jsx@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 89037694314a74e7f0e7a9c8d3793af5bf6b23d80950c29b360db1c66859d67f60711ea437e70ad6b5b4b29affe17eababda841b6c01107c2b638e0493bafb4e
+  checksum: 712f7e7918cb679f106769f57cfab0bc99b311032665c428b98f4c3e2e6d567601d45386a4f246df6a80d741e1f94192b3f008800d66c4f1daae3ad825c243f0
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-logical-assignment-operators@npm:^7.10.4, @babel/plugin-syntax-logical-assignment-operators@npm:^7.8.3":
   version: 7.10.4
   resolution: "@babel/plugin-syntax-logical-assignment-operators@npm:7.10.4"
   dependencies:
@@ -594,21 +600,21 @@
   peerDependencies:
     "@babel/core": ^7.0.0-0
   checksum: bbd1a56b095be7820029b209677b194db9b1d26691fe999856462e66b25b281f031f3dfd91b1619e9dcf95bebe336211833b854d0fb8780d618e35667c2d0d7e
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-typescript@npm:^7.7.2":
-  version: 7.23.3
-  resolution: "@babel/plugin-syntax-typescript@npm:7.23.3"
+  version: 7.24.1
+  resolution: "@babel/plugin-syntax-typescript@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: abfad3a19290d258b028e285a1f34c9b8a0cbe46ef79eafed4ed7ffce11b5d0720b5e536c82f91cbd8442cde35a3dd8e861fa70366d87ff06fdc0d4756e30876
+  checksum: bf4bd70788d5456b5f75572e47a2e31435c7c4e43609bd4dffd2cc0c7a6cf90aabcf6cd389e351854de9a64412a07d30effef5373251fe8f6a4c9db0c0163bda
   languageName: node
   linkType: hard
 
 "@babel/plugin-syntax-unicode-sets-regex@npm:^7.18.6":
   version: 7.18.6
   resolution: "@babel/plugin-syntax-unicode-sets-regex@npm:7.18.6"
   dependencies:
@@ -616,318 +622,318 @@
     "@babel/helper-plugin-utils": ^7.18.6
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: a651d700fe63ff0ddfd7186f4ebc24447ca734f114433139e3c027bc94a900d013cf1ef2e2db8430425ba542e39ae160c3b05f06b59fd4656273a3df97679e9c
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-arrow-functions@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-arrow-functions@npm:7.23.3"
+"@babel/plugin-transform-arrow-functions@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-arrow-functions@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 1e99118176e5366c2636064d09477016ab5272b2a92e78b8edb571d20bc3eaa881789a905b20042942c3c2d04efc530726cf703f937226db5ebc495f5d067e66
+  checksum: 58f9aa9b0de8382f8cfa3f1f1d40b69d98cd2f52340e2391733d0af745fdddda650ba392e509bc056157c880a2f52834a38ab2c5aa5569af8c61bb6ecbf45f34
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-async-generator-functions@npm:^7.23.9":
-  version: 7.23.9
-  resolution: "@babel/plugin-transform-async-generator-functions@npm:7.23.9"
+"@babel/plugin-transform-async-generator-functions@npm:^7.24.3":
+  version: 7.24.3
+  resolution: "@babel/plugin-transform-async-generator-functions@npm:7.24.3"
   dependencies:
     "@babel/helper-environment-visitor": ^7.22.20
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-remap-async-to-generator": ^7.22.20
     "@babel/plugin-syntax-async-generators": ^7.8.4
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: d402494087a6b803803eb5ab46b837aab100a04c4c5148e38bfa943ea1bbfc1ecfb340f1ced68972564312d3580f550c125f452372e77607a558fbbaf98c31c0
+  checksum: 309af02610be65d937664435adb432a32d9b6eb42bb3d3232c377d27fbc57014774d931665a5bfdaff3d1841b72659e0ad7adcef84b709f251cb0b8444f19214
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-async-to-generator@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-async-to-generator@npm:7.23.3"
+"@babel/plugin-transform-async-to-generator@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-async-to-generator@npm:7.24.1"
   dependencies:
-    "@babel/helper-module-imports": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-module-imports": ^7.24.1
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-remap-async-to-generator": ^7.22.20
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 2e9d9795d4b3b3d8090332104e37061c677f29a1ce65bcbda4099a32d243e5d9520270a44bbabf0fb1fb40d463bd937685b1a1042e646979086c546d55319c3c
+  checksum: 429004a6596aa5c9e707b604156f49a146f8d029e31a3152b1649c0b56425264fda5fd38e5db1ddaeb33c3fe45c97dc8078d7abfafe3542a979b49f229801135
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-block-scoped-functions@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-block-scoped-functions@npm:7.23.3"
+"@babel/plugin-transform-block-scoped-functions@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-block-scoped-functions@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: e63b16d94ee5f4d917e669da3db5ea53d1e7e79141a2ec873c1e644678cdafe98daa556d0d359963c827863d6b3665d23d4938a94a4c5053a1619c4ebd01d020
+  checksum: d8e18bd57b156da1cd4d3c1780ab9ea03afed56c6824ca8e6e74f67959d7989a0e953ec370fe9b417759314f2eef30c8c437395ce63ada2e26c2f469e4704f82
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-block-scoping@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-block-scoping@npm:7.23.4"
+"@babel/plugin-transform-block-scoping@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-block-scoping@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: fc4b2100dd9f2c47d694b4b35ae8153214ccb4e24ef545c259a9db17211b18b6a430f22799b56db8f6844deaeaa201af45a03331d0c80cc28b0c4e3c814570e4
+  checksum: 898c91efc0f8ac8e2a8d3ece36edf0001963bcf5bbeefe9bf798ac36318a33f366e88a24a90bf7c39a7aeb1593846b720ed9a9ba56709d27279f7ba61c5e43c4
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-class-properties@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-class-properties@npm:7.23.3"
+"@babel/plugin-transform-class-properties@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-class-properties@npm:7.24.1"
   dependencies:
-    "@babel/helper-create-class-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-create-class-features-plugin": ^7.24.1
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 9c6f8366f667897541d360246de176dd29efc7a13d80a5b48361882f7173d9173be4646c3b7d9b003ccc0e01e25df122330308f33db921fa553aa17ad544b3fc
+  checksum: 95779e9eef0c0638b9631c297d48aee53ffdbb2b1b5221bf40d7eccd566a8e34f859ff3571f8f20b9159b67f1bff7d7dc81da191c15d69fbae5a645197eae7e0
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-class-static-block@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-class-static-block@npm:7.23.4"
+"@babel/plugin-transform-class-static-block@npm:^7.24.4":
+  version: 7.24.4
+  resolution: "@babel/plugin-transform-class-static-block@npm:7.24.4"
   dependencies:
-    "@babel/helper-create-class-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-create-class-features-plugin": ^7.24.4
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-class-static-block": ^7.14.5
   peerDependencies:
     "@babel/core": ^7.12.0
-  checksum: c8bfaba19a674fc2eb54edad71e958647360474e3163e8226f1acd63e4e2dbec32a171a0af596c1dc5359aee402cc120fea7abd1fb0e0354b6527f0fc9e8aa1e
+  checksum: 3b1db3308b57ba21d47772a9f183804234c23fd64c9ca40915d2d65c5dc7a48b49a6de16b8b90b7a354eacbb51232a862f0fca3dbd23e27d34641f511decddab
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-classes@npm:^7.23.8":
-  version: 7.23.8
-  resolution: "@babel/plugin-transform-classes@npm:7.23.8"
+"@babel/plugin-transform-classes@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-classes@npm:7.24.5"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
     "@babel/helper-compilation-targets": ^7.23.6
     "@babel/helper-environment-visitor": ^7.22.20
     "@babel/helper-function-name": ^7.23.0
-    "@babel/helper-plugin-utils": ^7.22.5
-    "@babel/helper-replace-supers": ^7.22.20
-    "@babel/helper-split-export-declaration": ^7.22.6
+    "@babel/helper-plugin-utils": ^7.24.5
+    "@babel/helper-replace-supers": ^7.24.1
+    "@babel/helper-split-export-declaration": ^7.24.5
     globals: ^11.1.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 7dee6cebe52131d2d16944f36e1fdb9d4b24f44d0e7e450f93a44435d001f17cc0789a4cb6b15ec67c8e484581b8a730b5c3ec374470f29ff0133086955b8c58
+  checksum: 797bf2bda770148d3ee43e305e1aea26fa16ca78eb81eaaeb95b441428f52e0d12dd98e93f00bda3b65bbfde3001006995725ce911587efdef0465c41bd0a3f3
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-computed-properties@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-computed-properties@npm:7.23.3"
+"@babel/plugin-transform-computed-properties@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-computed-properties@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
-    "@babel/template": ^7.22.15
+    "@babel/helper-plugin-utils": ^7.24.0
+    "@babel/template": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 80452661dc25a0956f89fe98cb562e8637a9556fb6c00d312c57653ce7df8798f58d138603c7e1aad96614ee9ccd10c47e50ab9ded6b6eded5adeb230d2a982e
+  checksum: f2832bcf100a70f348facbb395873318ef5b9ee4b0fb4104a420d9daaeb6003cc2ecc12fd8083dd2e4a7c2da873272ad73ff94de4497125a0cf473294ef9664e
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-destructuring@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-destructuring@npm:7.23.3"
+"@babel/plugin-transform-destructuring@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-destructuring@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 9e015099877272501162419bfe781689aec5c462cd2aec752ee22288f209eec65969ff11b8fdadca2eaddea71d705d3bba5b9c60752fcc1be67874fcec687105
+  checksum: c5def67de09315cd38895c021ee7d02fd53fed596924512c33196ceed143b88f1ea76e4ac777a55bbb9db49be8b63aafb22b12e7d5c7f3051f14caa07e8d4023
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-dotall-regex@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-dotall-regex@npm:7.23.3"
+"@babel/plugin-transform-dotall-regex@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-dotall-regex@npm:7.24.1"
   dependencies:
     "@babel/helper-create-regexp-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: a2dbbf7f1ea16a97948c37df925cb364337668c41a3948b8d91453f140507bd8a3429030c7ce66d09c299987b27746c19a2dd18b6f17dcb474854b14fd9159a3
+  checksum: 7f623d25b6f213b94ebc1754e9e31c1077c8e288626d8b7bfa76a97b067ce80ddcd0ede402a546706c65002c0ccf45cd5ec621511c2668eed31ebcabe8391d35
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-duplicate-keys@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-duplicate-keys@npm:7.23.3"
+"@babel/plugin-transform-duplicate-keys@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-duplicate-keys@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: c2a21c34dc0839590cd945192cbc46fde541a27e140c48fe1808315934664cdbf18db64889e23c4eeb6bad9d3e049482efdca91d29de5734ffc887c4fbabaa16
+  checksum: a3b07c07cee441e185858a9bb9739bb72643173c18bf5f9f949dd2d4784ca124e56b01d0a270790fb1ff0cf75d436075db0a2b643fb4285ff9a21df9e8dc6284
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-dynamic-import@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-dynamic-import@npm:7.23.4"
+"@babel/plugin-transform-dynamic-import@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-dynamic-import@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-dynamic-import": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 57a722604c430d9f3dacff22001a5f31250e34785d4969527a2ae9160fa86858d0892c5b9ff7a06a04076f8c76c9e6862e0541aadca9c057849961343aab0845
+  checksum: 59fc561ee40b1a69f969c12c6c5fac206226d6642213985a569dd0f99f8e41c0f4eaedebd36936c255444a8335079842274c42a975a433beadb436d4c5abb79b
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-exponentiation-operator@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-exponentiation-operator@npm:7.23.3"
+"@babel/plugin-transform-exponentiation-operator@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-exponentiation-operator@npm:7.24.1"
   dependencies:
     "@babel/helper-builder-binary-assignment-operator-visitor": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 00d05ab14ad0f299160fcf9d8f55a1cc1b740e012ab0b5ce30207d2365f091665115557af7d989cd6260d075a252d9e4283de5f2b247dfbbe0e42ae586e6bf66
+  checksum: f90841fe1a1e9f680b4209121d3e2992f923e85efcd322b26e5901c180ef44ff727fb89790803a23fac49af34c1ce2e480018027c22b4573b615512ac5b6fc50
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-export-namespace-from@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-export-namespace-from@npm:7.23.4"
+"@babel/plugin-transform-export-namespace-from@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-export-namespace-from@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-export-namespace-from": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 9f770a81bfd03b48d6ba155d452946fd56d6ffe5b7d871e9ec2a0b15e0f424273b632f3ed61838b90015b25bbda988896b7a46c7d964fbf8f6feb5820b309f93
+  checksum: bc710ac231919df9555331885748385c11c5e695d7271824fe56fba51dd637d48d3e5cd52e1c69f2b1a384fbbb41552572bc1ca3a2285ee29571f002e9bb2421
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-for-of@npm:^7.23.6":
-  version: 7.23.6
-  resolution: "@babel/plugin-transform-for-of@npm:7.23.6"
+"@babel/plugin-transform-for-of@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-for-of@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 228c060aa61f6aa89dc447170075f8214863b94f830624e74ade99c1a09316897c12d76e848460b0b506593e58dbc42739af6dc4cb0fe9b84dffe4a596050a36
+  checksum: 990adde96ea1766ed6008c006c7040127bef59066533bb2977b246ea4a596fe450a528d1881a0db5f894deaf1b81654dfb494b19ad405b369be942738aa9c364
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-function-name@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-function-name@npm:7.23.3"
+"@babel/plugin-transform-function-name@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-function-name@npm:7.24.1"
   dependencies:
-    "@babel/helper-compilation-targets": ^7.22.15
+    "@babel/helper-compilation-targets": ^7.23.6
     "@babel/helper-function-name": ^7.23.0
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 355c6dbe07c919575ad42b2f7e020f320866d72f8b79181a16f8e0cd424a2c761d979f03f47d583d9471b55dcd68a8a9d829b58e1eebcd572145b934b48975a6
+  checksum: 31eb3c75297dda7265f78eba627c446f2324e30ec0124a645ccc3e9f341254aaa40d6787bd62b2280d77c0a5c9fbfce1da2c200ef7c7f8e0a1b16a8eb3644c6f
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-json-strings@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-json-strings@npm:7.23.4"
+"@babel/plugin-transform-json-strings@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-json-strings@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-json-strings": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: f9019820233cf8955d8ba346df709a0683c120fe86a24ed1c9f003f2db51197b979efc88f010d558a12e1491210fc195a43cd1c7fee5e23b92da38f793a875de
+  checksum: f42302d42fc81ac00d14e9e5d80405eb80477d7f9039d7208e712d6bcd486a4e3b32fdfa07b5f027d6c773723d8168193ee880f93b0e430c828e45f104fb82a4
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-literals@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-literals@npm:7.23.3"
+"@babel/plugin-transform-literals@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-literals@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 519a544cd58586b9001c4c9b18da25a62f17d23c48600ff7a685d75ca9eb18d2c5e8f5476f067f0a8f1fea2a31107eff950b9864833061e6076dcc4bdc3e71ed
+  checksum: 2df94e9478571852483aca7588419e574d76bde97583e78551c286f498e01321e7dbb1d0ef67bee16e8f950688f79688809cfde370c5c4b84c14d841a3ef217a
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-logical-assignment-operators@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-logical-assignment-operators@npm:7.23.4"
+"@babel/plugin-transform-logical-assignment-operators@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-logical-assignment-operators@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-logical-assignment-operators": ^7.10.4
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 2ae1dc9b4ff3bf61a990ff3accdecb2afe3a0ca649b3e74c010078d1cdf29ea490f50ac0a905306a2bcf9ac177889a39ac79bdcc3a0fdf220b3b75fac18d39b5
+  checksum: 895f2290adf457cbf327428bdb4fb90882a38a22f729bcf0629e8ad66b9b616d2721fbef488ac00411b647489d1dda1d20171bb3772d0796bb7ef5ecf057808a
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-member-expression-literals@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-member-expression-literals@npm:7.23.3"
+"@babel/plugin-transform-member-expression-literals@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-member-expression-literals@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 95cec13c36d447c5aa6b8e4c778b897eeba66dcb675edef01e0d2afcec9e8cb9726baf4f81b4bbae7a782595aed72e6a0d44ffb773272c3ca180fada99bf92db
+  checksum: 4ea641cc14a615f9084e45ad2319f95e2fee01c77ec9789685e7e11a6c286238a426a98f9c1ed91568a047d8ac834393e06e8c82d1ff01764b7aa61bee8e9023
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-amd@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-modules-amd@npm:7.23.3"
+"@babel/plugin-transform-modules-amd@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-modules-amd@npm:7.24.1"
   dependencies:
     "@babel/helper-module-transforms": ^7.23.3
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: d163737b6a3d67ea579c9aa3b83d4df4b5c34d9dcdf25f415f027c0aa8cded7bac2750d2de5464081f67a042ad9e1c03930c2fab42acd79f9e57c00cf969ddff
+  checksum: 3d777c262f257e93f0405b13e178f9c4a0f31855b409f0191a76bb562a28c541326a027bfe6467fcb74752f3488c0333b5ff2de64feec1b3c4c6ace1747afa03
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-commonjs@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-modules-commonjs@npm:7.23.3"
+"@babel/plugin-transform-modules-commonjs@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-modules-commonjs@npm:7.24.1"
   dependencies:
     "@babel/helper-module-transforms": ^7.23.3
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-simple-access": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 720a231ceade4ae4d2632478db4e7fecf21987d444942b72d523487ac8d715ca97de6c8f415c71e939595e1a4776403e7dc24ed68fe9125ad4acf57753c9bff7
+  checksum: 11402b34c49f76aa921b43c2d76f3f129a32544a1dc4f0d1e48b310f9036ab75269a6d8684ed0198b7a0b07bd7898b12f0cacceb26fbb167999fd2a819aa0802
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-systemjs@npm:^7.23.9":
-  version: 7.23.9
-  resolution: "@babel/plugin-transform-modules-systemjs@npm:7.23.9"
+"@babel/plugin-transform-modules-systemjs@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-modules-systemjs@npm:7.24.1"
   dependencies:
     "@babel/helper-hoist-variables": ^7.22.5
     "@babel/helper-module-transforms": ^7.23.3
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-validator-identifier": ^7.22.20
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: cec6abeae6be66fd1a5940c482fe9ff94b689c71fcf4147e179119e4accd09d17d476e36528bc9cb4ab0ec6728fedf48b1c49d0551ea707fb192575d8eac9167
+  checksum: 903766f6808f04278e887e4adec9b1efa741726279652dad255eaad0f5701df8f8ff0af25eb8541a00eb3c9eae2dccf337b085cfa011426ca33ed1f95d70bf75
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-modules-umd@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-modules-umd@npm:7.23.3"
+"@babel/plugin-transform-modules-umd@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-modules-umd@npm:7.24.1"
   dependencies:
     "@babel/helper-module-transforms": ^7.23.3
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 586a7a2241e8b4e753a37af9466a9ffa8a67b4ba9aa756ad7500712c05d8fa9a8c1ed4f7bd25fae2a8265e6cf8fe781ec85a8ee885dd34cf50d8955ee65f12dc
+  checksum: 4922f5056d34de6fd59a1ab1c85bc3472afa706c776aceeb886289c9ac9117e6eb8e22d06c537eb5bc0ede6c30f6bd85210bdcc150dc0ae2d2373f8252df9364
   languageName: node
   linkType: hard
 
 "@babel/plugin-transform-named-capturing-groups-regex@npm:^7.22.5":
   version: 7.22.5
   resolution: "@babel/plugin-transform-named-capturing-groups-regex@npm:7.22.5"
   dependencies:
@@ -935,362 +941,362 @@
     "@babel/helper-plugin-utils": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0
   checksum: 3ee564ddee620c035b928fdc942c5d17e9c4b98329b76f9cefac65c111135d925eb94ed324064cd7556d4f5123beec79abea1d4b97d1c8a2a5c748887a2eb623
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-new-target@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-new-target@npm:7.23.3"
+"@babel/plugin-transform-new-target@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-new-target@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: e5053389316fce73ad5201b7777437164f333e24787fbcda4ae489cd2580dbbbdfb5694a7237bad91fabb46b591d771975d69beb1c740b82cb4761625379f00b
+  checksum: f56159ba56e8824840b8073f65073434e4bc4ef20e366bc03aa6cae9a4389365574fa72390e48aed76049edbc6eba1181eb810e58fae22c25946c62f9da13db4
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-nullish-coalescing-operator@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-nullish-coalescing-operator@npm:7.23.4"
+"@babel/plugin-transform-nullish-coalescing-operator@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-nullish-coalescing-operator@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-nullish-coalescing-operator": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: a27d73ea134d3d9560a6b2e26ab60012fba15f1db95865aa0153c18f5ec82cfef6a7b3d8df74e3c2fca81534fa5efeb6cacaf7b08bdb7d123e3dafdd079886a3
+  checksum: 74025e191ceb7cefc619c15d33753aab81300a03d81b96ae249d9b599bc65878f962d608f452462d3aad5d6e334b7ab2b09a6bdcfe8d101fe77ac7aacca4261e
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-numeric-separator@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-numeric-separator@npm:7.23.4"
+"@babel/plugin-transform-numeric-separator@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-numeric-separator@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-numeric-separator": ^7.10.4
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 6ba0e5db3c620a3ec81f9e94507c821f483c15f196868df13fa454cbac719a5449baf73840f5b6eb7d77311b24a2cf8e45db53700d41727f693d46f7caf3eec3
+  checksum: 3247bd7d409574fc06c59e0eb573ae7470d6d61ecf780df40b550102bb4406747d8f39dcbec57eb59406df6c565a86edd3b429e396ad02e4ce201ad92050832e
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-object-rest-spread@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-object-rest-spread@npm:7.23.4"
+"@babel/plugin-transform-object-rest-spread@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-object-rest-spread@npm:7.24.5"
   dependencies:
-    "@babel/compat-data": ^7.23.3
-    "@babel/helper-compilation-targets": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-compilation-targets": ^7.23.6
+    "@babel/helper-plugin-utils": ^7.24.5
     "@babel/plugin-syntax-object-rest-spread": ^7.8.3
-    "@babel/plugin-transform-parameters": ^7.23.3
+    "@babel/plugin-transform-parameters": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 73fec495e327ca3959c1c03d07a621be09df00036c69fff0455af9a008291677ee9d368eec48adacdc6feac703269a649747568b4af4c4e9f134aa71cc5b378d
+  checksum: 427705fe1358ca4862e6cfbfc174dc0fbfdd640b786cfe759dd4881cfb2fd51723e8432ecd89f07a60444e555a9c19e0e7bf4c657b91844994b39a53a602eb16
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-object-super@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-object-super@npm:7.23.3"
+"@babel/plugin-transform-object-super@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-object-super@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
-    "@babel/helper-replace-supers": ^7.22.20
+    "@babel/helper-plugin-utils": ^7.24.0
+    "@babel/helper-replace-supers": ^7.24.1
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: e495497186f621fa79026e183b4f1fbb172fd9df812cbd2d7f02c05b08adbe58012b1a6eb6dd58d11a30343f6ec80d0f4074f9b501d70aa1c94df76d59164c53
+  checksum: d34d437456a54e2a5dcb26e9cf09ed4c55528f2a327c5edca92c93e9483c37176e228d00d6e0cf767f3d6fdbef45ae3a5d034a7c59337a009e20ae541c8220fa
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-optional-catch-binding@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-optional-catch-binding@npm:7.23.4"
+"@babel/plugin-transform-optional-catch-binding@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-optional-catch-binding@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/plugin-syntax-optional-catch-binding": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: d50b5ee142cdb088d8b5de1ccf7cea85b18b85d85b52f86618f6e45226372f01ad4cdb29abd4fd35ea99a71fefb37009e0107db7a787dcc21d4d402f97470faf
+  checksum: ff7c02449d32a6de41e003abb38537b4a1ad90b1eaa4c0b578cb1b55548201a677588a8c47f3e161c72738400ae811a6673ea7b8a734344755016ca0ac445dac
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-optional-chaining@npm:^7.23.3, @babel/plugin-transform-optional-chaining@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-optional-chaining@npm:7.23.4"
+"@babel/plugin-transform-optional-chaining@npm:^7.24.1, @babel/plugin-transform-optional-chaining@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-optional-chaining@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
     "@babel/plugin-syntax-optional-chaining": ^7.8.3
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: e7a4c08038288057b7a08d68c4d55396ada9278095509ca51ed8dfb72a7f13f26bdd7c5185de21079fe0a9d60d22c227cb32e300d266c1bda40f70eee9f4bc1e
+  checksum: 233934463ef1f9a02a9fda96c722e9c162477fd94816a58413f0d4165cc536c7af0482b46fe066e754748a20bbabec255b4bbde194a7fd20b32280e526e1bfec
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-parameters@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-parameters@npm:7.23.3"
+"@babel/plugin-transform-parameters@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-parameters@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: a735b3e85316d17ec102e3d3d1b6993b429bdb3b494651c9d754e3b7d270462ee1f1a126ccd5e3d871af5e683727e9ef98c9d34d4a42204fffaabff91052ed16
+  checksum: b052e1cf43b1ea571fc0867baa01041ce32f46576b711c6331f03263ae479a582f81a6039287535cd90ee46d2977e2f3c66f5bdbf454a9f8cdc7c5c6c67b50be
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-private-methods@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-private-methods@npm:7.23.3"
+"@babel/plugin-transform-private-methods@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-private-methods@npm:7.24.1"
   dependencies:
-    "@babel/helper-create-class-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-create-class-features-plugin": ^7.24.1
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: cedc1285c49b5a6d9a3d0e5e413b756ac40b3ac2f8f68bdfc3ae268bc8d27b00abd8bb0861c72756ff5dd8bf1eb77211b7feb5baf4fdae2ebbaabe49b9adc1d0
+  checksum: 7208c30bb3f3fbc73fb3a88bdcb78cd5cddaf6d523eb9d67c0c04e78f6fc6319ece89f4a5abc41777ceab16df55b3a13a4120e0efc9275ca6d2d89beaba80aa0
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-private-property-in-object@npm:^7.23.4":
-  version: 7.23.4
-  resolution: "@babel/plugin-transform-private-property-in-object@npm:7.23.4"
+"@babel/plugin-transform-private-property-in-object@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-private-property-in-object@npm:7.24.5"
   dependencies:
     "@babel/helper-annotate-as-pure": ^7.22.5
-    "@babel/helper-create-class-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-create-class-features-plugin": ^7.24.5
+    "@babel/helper-plugin-utils": ^7.24.5
     "@babel/plugin-syntax-private-property-in-object": ^7.14.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: fb7adfe94ea97542f250a70de32bddbc3e0b802381c92be947fec83ebffda57e68533c4d0697152719a3496fdd3ebf3798d451c024cd4ac848fc15ac26b70aa7
+  checksum: 59f9007671f50ef8f9eff33bb2dc3de22a2849612d4b64fc9e4ba502466ddbaf3f94774011695dde5128c4ca2009e241babe928ac63f71a29f27c1cc7ce01e5f
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-property-literals@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-property-literals@npm:7.23.3"
+"@babel/plugin-transform-property-literals@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-property-literals@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 16b048c8e87f25095f6d53634ab7912992f78e6997a6ff549edc3cf519db4fca01c7b4e0798530d7f6a05228ceee479251245cdd850a5531c6e6f404104d6cc9
+  checksum: a73646d7ecd95b3931a3ead82c7d5efeb46e68ba362de63eb437d33531f294ec18bd31b6d24238cd3b6a3b919a6310c4a0ba4a2629927721d4d10b0518eb7715
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-regenerator@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-regenerator@npm:7.23.3"
+"@babel/plugin-transform-regenerator@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-regenerator@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     regenerator-transform: ^0.15.2
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 7fdacc7b40008883871b519c9e5cdea493f75495118ccc56ac104b874983569a24edd024f0f5894ba1875c54ee2b442f295d6241c3280e61c725d0dd3317c8e6
+  checksum: a04319388a0a7931c3f8e15715d01444c32519692178b70deccc86d53304e74c0f589a4268f6c68578d86f75e934dd1fe6e6ed9071f54ee8379f356f88ef6e42
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-reserved-words@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-reserved-words@npm:7.23.3"
+"@babel/plugin-transform-reserved-words@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-reserved-words@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 298c4440ddc136784ff920127cea137168e068404e635dc946ddb5d7b2a27b66f1dd4c4acb01f7184478ff7d5c3e7177a127279479926519042948fb7fa0fa48
+  checksum: 132c6040c65aabae2d98a39289efb5c51a8632546dc50d2ad032c8660aec307fbed74ef499856ea4f881fc8505905f49b48e0270585da2ea3d50b75e962afd89
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-shorthand-properties@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-shorthand-properties@npm:7.23.3"
+"@babel/plugin-transform-shorthand-properties@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-shorthand-properties@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 5d677a03676f9fff969b0246c423d64d77502e90a832665dc872a5a5e05e5708161ce1effd56bb3c0f2c20a1112fca874be57c8a759d8b08152755519281f326
+  checksum: 006a2032d1c57dca76579ce6598c679c2f20525afef0a36e9d42affe3c8cf33c1427581ad696b519cc75dfee46c5e8ecdf0c6a29ffb14250caa3e16dd68cb424
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-spread@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-spread@npm:7.23.3"
+"@babel/plugin-transform-spread@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-spread@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
     "@babel/helper-skip-transparent-expression-wrappers": ^7.22.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 8fd5cac201e77a0b4825745f4e07a25f923842f282f006b3a79223c00f61075c8868d12eafec86b2642cd0b32077cdd32314e27bcb75ee5e6a68c0144140dcf2
+  checksum: 622ef507e2b5120a9010b25d3df5186c06102ecad8751724a38ec924df8d3527688198fa490c47064eabba14ef2f961b3069855bd22a8c0a1e51a23eed348d02
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-sticky-regex@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-sticky-regex@npm:7.23.3"
+"@babel/plugin-transform-sticky-regex@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-sticky-regex@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 53e55eb2575b7abfdb4af7e503a2bf7ef5faf8bf6b92d2cd2de0700bdd19e934e5517b23e6dfed94ba50ae516b62f3f916773ef7d9bc81f01503f585051e2949
+  checksum: e326e96a9eeb6bb01dbc4d3362f989411490671b97f62edf378b8fb102c463a018b777f28da65344d41b22aa6efcdfa01ed43d2b11fdcf202046d3174be137c5
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-template-literals@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-template-literals@npm:7.23.3"
+"@babel/plugin-transform-template-literals@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-template-literals@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: b16c5cb0b8796be0118e9c144d15bdc0d20a7f3f59009c6303a6e9a8b74c146eceb3f05186f5b97afcba7cfa87e34c1585a22186e3d5b22f2fd3d27d959d92b2
+  checksum: 4c9009c72321caf20e3b6328bbe9d7057006c5ae57b794cf247a37ca34d87dfec5e27284169a16df5a6235a083bf0f3ab9e1bfcb005d1c8b75b04aed75652621
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-typeof-symbol@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-typeof-symbol@npm:7.23.3"
+"@babel/plugin-transform-typeof-symbol@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/plugin-transform-typeof-symbol@npm:7.24.5"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 0af7184379d43afac7614fc89b1bdecce4e174d52f4efaeee8ec1a4f2c764356c6dba3525c0685231f1cbf435b6dd4ee9e738d7417f3b10ce8bbe869c32f4384
+  checksum: 35504219e4e8b361dbd285400c846f154754e591e931cd30dbe1426a619e41ed0c410b26dd173824ed3a2ff0371d64213ae2304b6f169b32e78b004114f5acd5
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-escapes@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-unicode-escapes@npm:7.23.3"
+"@babel/plugin-transform-unicode-escapes@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-unicode-escapes@npm:7.24.1"
   dependencies:
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 561c429183a54b9e4751519a3dfba6014431e9cdc1484fad03bdaf96582dfc72c76a4f8661df2aeeae7c34efd0fa4d02d3b83a2f63763ecf71ecc925f9cc1f60
+  checksum: d4d7cfea91af7be2768fb6bed902e00d6e3190bda738b5149c3a788d570e6cf48b974ec9548442850308ecd8fc9a67681f4ea8403129e7867bcb85adaf6ec238
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-property-regex@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-unicode-property-regex@npm:7.23.3"
+"@babel/plugin-transform-unicode-property-regex@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-unicode-property-regex@npm:7.24.1"
   dependencies:
     "@babel/helper-create-regexp-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 2298461a194758086d17c23c26c7de37aa533af910f9ebf31ebd0893d4aa317468043d23f73edc782ec21151d3c46cf0ff8098a83b725c49a59de28a1d4d6225
+  checksum: 276099b4483e707f80b054e2d29bc519158bfe52461ef5ff76f70727d592df17e30b1597ef4d8a0f04d810f6cb5a8dd887bdc1d0540af3744751710ef280090f
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-regex@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-unicode-regex@npm:7.23.3"
+"@babel/plugin-transform-unicode-regex@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-unicode-regex@npm:7.24.1"
   dependencies:
     "@babel/helper-create-regexp-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: c5f835d17483ba899787f92e313dfa5b0055e3deab332f1d254078a2bba27ede47574b6599fcf34d3763f0c048ae0779dc21d2d8db09295edb4057478dc80a9a
+  checksum: 400a0927bdb1425b4c0dc68a61b5b2d7d17c7d9f0e07317a1a6a373c080ef94be1dd65fdc4ac9a78fcdb58f89fd128450c7bc0d5b8ca0ae7eca3fbd98e50acba
   languageName: node
   linkType: hard
 
-"@babel/plugin-transform-unicode-sets-regex@npm:^7.23.3":
-  version: 7.23.3
-  resolution: "@babel/plugin-transform-unicode-sets-regex@npm:7.23.3"
+"@babel/plugin-transform-unicode-sets-regex@npm:^7.24.1":
+  version: 7.24.1
+  resolution: "@babel/plugin-transform-unicode-sets-regex@npm:7.24.1"
   dependencies:
     "@babel/helper-create-regexp-features-plugin": ^7.22.15
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.0
   peerDependencies:
     "@babel/core": ^7.0.0
-  checksum: 79d0b4c951955ca68235c87b91ab2b393c96285f8aeaa34d6db416d2ddac90000c9bd6e8c4d82b60a2b484da69930507245035f28ba63c6cae341cf3ba68fdef
+  checksum: 364342fb8e382dfaa23628b88e6484dc1097e53fb7199f4d338f1e2cd71d839bb0a35a9b1380074f6a10adb2e98b79d53ca3ec78c0b8c557ca895ffff42180df
   languageName: node
   linkType: hard
 
 "@babel/preset-env@npm:^7.10.2":
-  version: 7.23.9
-  resolution: "@babel/preset-env@npm:7.23.9"
+  version: 7.24.5
+  resolution: "@babel/preset-env@npm:7.24.5"
   dependencies:
-    "@babel/compat-data": ^7.23.5
+    "@babel/compat-data": ^7.24.4
     "@babel/helper-compilation-targets": ^7.23.6
-    "@babel/helper-plugin-utils": ^7.22.5
+    "@babel/helper-plugin-utils": ^7.24.5
     "@babel/helper-validator-option": ^7.23.5
-    "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression": ^7.23.3
-    "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining": ^7.23.3
-    "@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly": ^7.23.7
+    "@babel/plugin-bugfix-firefox-class-in-computed-class-key": ^7.24.5
+    "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression": ^7.24.1
+    "@babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining": ^7.24.1
+    "@babel/plugin-bugfix-v8-static-class-fields-redefine-readonly": ^7.24.1
     "@babel/plugin-proposal-private-property-in-object": 7.21.0-placeholder-for-preset-env.2
     "@babel/plugin-syntax-async-generators": ^7.8.4
     "@babel/plugin-syntax-class-properties": ^7.12.13
     "@babel/plugin-syntax-class-static-block": ^7.14.5
     "@babel/plugin-syntax-dynamic-import": ^7.8.3
     "@babel/plugin-syntax-export-namespace-from": ^7.8.3
-    "@babel/plugin-syntax-import-assertions": ^7.23.3
-    "@babel/plugin-syntax-import-attributes": ^7.23.3
+    "@babel/plugin-syntax-import-assertions": ^7.24.1
+    "@babel/plugin-syntax-import-attributes": ^7.24.1
     "@babel/plugin-syntax-import-meta": ^7.10.4
     "@babel/plugin-syntax-json-strings": ^7.8.3
     "@babel/plugin-syntax-logical-assignment-operators": ^7.10.4
     "@babel/plugin-syntax-nullish-coalescing-operator": ^7.8.3
     "@babel/plugin-syntax-numeric-separator": ^7.10.4
     "@babel/plugin-syntax-object-rest-spread": ^7.8.3
     "@babel/plugin-syntax-optional-catch-binding": ^7.8.3
     "@babel/plugin-syntax-optional-chaining": ^7.8.3
     "@babel/plugin-syntax-private-property-in-object": ^7.14.5
     "@babel/plugin-syntax-top-level-await": ^7.14.5
     "@babel/plugin-syntax-unicode-sets-regex": ^7.18.6
-    "@babel/plugin-transform-arrow-functions": ^7.23.3
-    "@babel/plugin-transform-async-generator-functions": ^7.23.9
-    "@babel/plugin-transform-async-to-generator": ^7.23.3
-    "@babel/plugin-transform-block-scoped-functions": ^7.23.3
-    "@babel/plugin-transform-block-scoping": ^7.23.4
-    "@babel/plugin-transform-class-properties": ^7.23.3
-    "@babel/plugin-transform-class-static-block": ^7.23.4
-    "@babel/plugin-transform-classes": ^7.23.8
-    "@babel/plugin-transform-computed-properties": ^7.23.3
-    "@babel/plugin-transform-destructuring": ^7.23.3
-    "@babel/plugin-transform-dotall-regex": ^7.23.3
-    "@babel/plugin-transform-duplicate-keys": ^7.23.3
-    "@babel/plugin-transform-dynamic-import": ^7.23.4
-    "@babel/plugin-transform-exponentiation-operator": ^7.23.3
-    "@babel/plugin-transform-export-namespace-from": ^7.23.4
-    "@babel/plugin-transform-for-of": ^7.23.6
-    "@babel/plugin-transform-function-name": ^7.23.3
-    "@babel/plugin-transform-json-strings": ^7.23.4
-    "@babel/plugin-transform-literals": ^7.23.3
-    "@babel/plugin-transform-logical-assignment-operators": ^7.23.4
-    "@babel/plugin-transform-member-expression-literals": ^7.23.3
-    "@babel/plugin-transform-modules-amd": ^7.23.3
-    "@babel/plugin-transform-modules-commonjs": ^7.23.3
-    "@babel/plugin-transform-modules-systemjs": ^7.23.9
-    "@babel/plugin-transform-modules-umd": ^7.23.3
+    "@babel/plugin-transform-arrow-functions": ^7.24.1
+    "@babel/plugin-transform-async-generator-functions": ^7.24.3
+    "@babel/plugin-transform-async-to-generator": ^7.24.1
+    "@babel/plugin-transform-block-scoped-functions": ^7.24.1
+    "@babel/plugin-transform-block-scoping": ^7.24.5
+    "@babel/plugin-transform-class-properties": ^7.24.1
+    "@babel/plugin-transform-class-static-block": ^7.24.4
+    "@babel/plugin-transform-classes": ^7.24.5
+    "@babel/plugin-transform-computed-properties": ^7.24.1
+    "@babel/plugin-transform-destructuring": ^7.24.5
+    "@babel/plugin-transform-dotall-regex": ^7.24.1
+    "@babel/plugin-transform-duplicate-keys": ^7.24.1
+    "@babel/plugin-transform-dynamic-import": ^7.24.1
+    "@babel/plugin-transform-exponentiation-operator": ^7.24.1
+    "@babel/plugin-transform-export-namespace-from": ^7.24.1
+    "@babel/plugin-transform-for-of": ^7.24.1
+    "@babel/plugin-transform-function-name": ^7.24.1
+    "@babel/plugin-transform-json-strings": ^7.24.1
+    "@babel/plugin-transform-literals": ^7.24.1
+    "@babel/plugin-transform-logical-assignment-operators": ^7.24.1
+    "@babel/plugin-transform-member-expression-literals": ^7.24.1
+    "@babel/plugin-transform-modules-amd": ^7.24.1
+    "@babel/plugin-transform-modules-commonjs": ^7.24.1
+    "@babel/plugin-transform-modules-systemjs": ^7.24.1
+    "@babel/plugin-transform-modules-umd": ^7.24.1
     "@babel/plugin-transform-named-capturing-groups-regex": ^7.22.5
-    "@babel/plugin-transform-new-target": ^7.23.3
-    "@babel/plugin-transform-nullish-coalescing-operator": ^7.23.4
-    "@babel/plugin-transform-numeric-separator": ^7.23.4
-    "@babel/plugin-transform-object-rest-spread": ^7.23.4
-    "@babel/plugin-transform-object-super": ^7.23.3
-    "@babel/plugin-transform-optional-catch-binding": ^7.23.4
-    "@babel/plugin-transform-optional-chaining": ^7.23.4
-    "@babel/plugin-transform-parameters": ^7.23.3
-    "@babel/plugin-transform-private-methods": ^7.23.3
-    "@babel/plugin-transform-private-property-in-object": ^7.23.4
-    "@babel/plugin-transform-property-literals": ^7.23.3
-    "@babel/plugin-transform-regenerator": ^7.23.3
-    "@babel/plugin-transform-reserved-words": ^7.23.3
-    "@babel/plugin-transform-shorthand-properties": ^7.23.3
-    "@babel/plugin-transform-spread": ^7.23.3
-    "@babel/plugin-transform-sticky-regex": ^7.23.3
-    "@babel/plugin-transform-template-literals": ^7.23.3
-    "@babel/plugin-transform-typeof-symbol": ^7.23.3
-    "@babel/plugin-transform-unicode-escapes": ^7.23.3
-    "@babel/plugin-transform-unicode-property-regex": ^7.23.3
-    "@babel/plugin-transform-unicode-regex": ^7.23.3
-    "@babel/plugin-transform-unicode-sets-regex": ^7.23.3
+    "@babel/plugin-transform-new-target": ^7.24.1
+    "@babel/plugin-transform-nullish-coalescing-operator": ^7.24.1
+    "@babel/plugin-transform-numeric-separator": ^7.24.1
+    "@babel/plugin-transform-object-rest-spread": ^7.24.5
+    "@babel/plugin-transform-object-super": ^7.24.1
+    "@babel/plugin-transform-optional-catch-binding": ^7.24.1
+    "@babel/plugin-transform-optional-chaining": ^7.24.5
+    "@babel/plugin-transform-parameters": ^7.24.5
+    "@babel/plugin-transform-private-methods": ^7.24.1
+    "@babel/plugin-transform-private-property-in-object": ^7.24.5
+    "@babel/plugin-transform-property-literals": ^7.24.1
+    "@babel/plugin-transform-regenerator": ^7.24.1
+    "@babel/plugin-transform-reserved-words": ^7.24.1
+    "@babel/plugin-transform-shorthand-properties": ^7.24.1
+    "@babel/plugin-transform-spread": ^7.24.1
+    "@babel/plugin-transform-sticky-regex": ^7.24.1
+    "@babel/plugin-transform-template-literals": ^7.24.1
+    "@babel/plugin-transform-typeof-symbol": ^7.24.5
+    "@babel/plugin-transform-unicode-escapes": ^7.24.1
+    "@babel/plugin-transform-unicode-property-regex": ^7.24.1
+    "@babel/plugin-transform-unicode-regex": ^7.24.1
+    "@babel/plugin-transform-unicode-sets-regex": ^7.24.1
     "@babel/preset-modules": 0.1.6-no-external-plugins
-    babel-plugin-polyfill-corejs2: ^0.4.8
-    babel-plugin-polyfill-corejs3: ^0.9.0
-    babel-plugin-polyfill-regenerator: ^0.5.5
+    babel-plugin-polyfill-corejs2: ^0.4.10
+    babel-plugin-polyfill-corejs3: ^0.10.4
+    babel-plugin-polyfill-regenerator: ^0.6.1
     core-js-compat: ^3.31.0
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.0.0-0
-  checksum: 23a48468ba820c68ba34ea2c1dbc62fd2ff9cf858cfb69e159cabb0c85c72dc4c2266ce20ca84318d8742de050cb061e7c66902fbfddbcb09246afd248847933
+  checksum: cced4e5331231158e02ba5903c4de12ef0aa2d2266ebb07fa80a85045b1fe2c63410d7558b702f1916d9d038531f3d79ab31007762188de5f712b16f7a66bb74
   languageName: node
   linkType: hard
 
 "@babel/preset-modules@npm:0.1.6-no-external-plugins":
   version: 0.1.6-no-external-plugins
   resolution: "@babel/preset-modules@npm:0.1.6-no-external-plugins"
   dependencies:
@@ -1307,95 +1313,95 @@
   version: 0.8.0
   resolution: "@babel/regjsgen@npm:0.8.0"
   checksum: 89c338fee774770e5a487382170711014d49a68eb281e74f2b5eac88f38300a4ad545516a7786a8dd5702e9cf009c94c2f582d200f077ac5decd74c56b973730
   languageName: node
   linkType: hard
 
 "@babel/runtime@npm:^7.8.4":
-  version: 7.23.9
-  resolution: "@babel/runtime@npm:7.23.9"
+  version: 7.24.5
+  resolution: "@babel/runtime@npm:7.24.5"
   dependencies:
     regenerator-runtime: ^0.14.0
-  checksum: 6bbebe8d27c0c2dd275d1ac197fc1a6c00e18dab68cc7aaff0adc3195b45862bae9c4cc58975629004b0213955b2ed91e99eccb3d9b39cabea246c657323d667
+  checksum: 755383192f3ac32ba4c62bd4f1ae92aed5b82d2c6665f39eb28fa94546777cf5c63493ea92dd03f1c2e621b17e860f190c056684b7f234270fdc91e29beda063
   languageName: node
   linkType: hard
 
-"@babel/template@npm:^7.22.15, @babel/template@npm:^7.23.9, @babel/template@npm:^7.3.3":
-  version: 7.23.9
-  resolution: "@babel/template@npm:7.23.9"
+"@babel/template@npm:^7.22.15, @babel/template@npm:^7.24.0, @babel/template@npm:^7.3.3":
+  version: 7.24.0
+  resolution: "@babel/template@npm:7.24.0"
   dependencies:
     "@babel/code-frame": ^7.23.5
-    "@babel/parser": ^7.23.9
-    "@babel/types": ^7.23.9
-  checksum: 6e67414c0f7125d7ecaf20c11fab88085fa98a96c3ef10da0a61e962e04fdf3a18a496a66047005ddd1bb682a7cc7842d556d1db2f3f3f6ccfca97d5e445d342
+    "@babel/parser": ^7.24.0
+    "@babel/types": ^7.24.0
+  checksum: f257b003c071a0cecdbfceca74185f18fe62c055469ab5c1d481aab12abeebed328e67e0a19fd978a2a8de97b28953fa4bc3da6d038a7345fdf37923b9fcdec8
   languageName: node
   linkType: hard
 
-"@babel/traverse@npm:^7.23.9":
-  version: 7.23.9
-  resolution: "@babel/traverse@npm:7.23.9"
+"@babel/traverse@npm:^7.24.5":
+  version: 7.24.5
+  resolution: "@babel/traverse@npm:7.24.5"
   dependencies:
-    "@babel/code-frame": ^7.23.5
-    "@babel/generator": ^7.23.6
+    "@babel/code-frame": ^7.24.2
+    "@babel/generator": ^7.24.5
     "@babel/helper-environment-visitor": ^7.22.20
     "@babel/helper-function-name": ^7.23.0
     "@babel/helper-hoist-variables": ^7.22.5
-    "@babel/helper-split-export-declaration": ^7.22.6
-    "@babel/parser": ^7.23.9
-    "@babel/types": ^7.23.9
+    "@babel/helper-split-export-declaration": ^7.24.5
+    "@babel/parser": ^7.24.5
+    "@babel/types": ^7.24.5
     debug: ^4.3.1
     globals: ^11.1.0
-  checksum: a932f7aa850e158c00c97aad22f639d48c72805c687290f6a73e30c5c4957c07f5d28310c9bf59648e2980fe6c9d16adeb2ff92a9ca0f97fa75739c1328fc6c3
+  checksum: a313fbf4a06946cc4b74b06e9846d7393a9ca1e8b6df6da60c669cff0a9426d6198c21a478041c60807b62b48f980473d4afbd3768764b0d9741ac80f5dfa04f
   languageName: node
   linkType: hard
 
-"@babel/types@npm:^7.0.0, @babel/types@npm:^7.20.7, @babel/types@npm:^7.22.15, @babel/types@npm:^7.22.19, @babel/types@npm:^7.22.5, @babel/types@npm:^7.23.0, @babel/types@npm:^7.23.6, @babel/types@npm:^7.23.9, @babel/types@npm:^7.3.3, @babel/types@npm:^7.4.4, @babel/types@npm:^7.8.3":
-  version: 7.23.9
-  resolution: "@babel/types@npm:7.23.9"
+"@babel/types@npm:^7.0.0, @babel/types@npm:^7.20.7, @babel/types@npm:^7.22.15, @babel/types@npm:^7.22.5, @babel/types@npm:^7.23.0, @babel/types@npm:^7.24.0, @babel/types@npm:^7.24.5, @babel/types@npm:^7.3.3, @babel/types@npm:^7.4.4, @babel/types@npm:^7.8.3":
+  version: 7.24.5
+  resolution: "@babel/types@npm:7.24.5"
   dependencies:
-    "@babel/helper-string-parser": ^7.23.4
-    "@babel/helper-validator-identifier": ^7.22.20
+    "@babel/helper-string-parser": ^7.24.1
+    "@babel/helper-validator-identifier": ^7.24.5
     to-fast-properties: ^2.0.0
-  checksum: 0a9b008e9bfc89beb8c185e620fa0f8ed6c771f1e1b2e01e1596870969096fec7793898a1d64a035176abf1dd13e2668ee30bf699f2d92c210a8128f4b151e65
+  checksum: 8eeeacd996593b176e649ee49d8dc3f26f9bb6aa1e3b592030e61a0e58ea010fb018dccc51e5314c8139409ea6cbab02e29b33e674e1f6962d8e24c52da6375b
   languageName: node
   linkType: hard
 
 "@bcoe/v8-coverage@npm:^0.2.3":
   version: 0.2.3
   resolution: "@bcoe/v8-coverage@npm:0.2.3"
   checksum: 850f9305536d0f2bd13e9e0881cb5f02e4f93fad1189f7b2d4bebf694e3206924eadee1068130d43c11b750efcc9405f88a8e42ef098b6d75239c0f047de1a27
   languageName: node
   linkType: hard
 
 "@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.5.1, @codemirror/autocomplete@npm:^6.7.1":
-  version: 6.12.0
-  resolution: "@codemirror/autocomplete@npm:6.12.0"
+  version: 6.16.0
+  resolution: "@codemirror/autocomplete@npm:6.16.0"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
   peerDependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: 1d4da6ccc12f5a67053a76b361f2683b5af031dd405a0bd2a261a265eb8cb7dfb115343a3291260d1ba31ce7ccb5427208ebe50f50f6747fcf27a50b62c87f7e
+  checksum: e33d3d8c961c03dc4a70d1ac6f01aee5362d778da9d873a8335aed47f7de9430eab083589736e7922464b941d5da23c51ab6af05400413a8d1a07604ffcb99f7
   languageName: node
   linkType: hard
 
 "@codemirror/commands@npm:^6.2.3":
-  version: 6.3.3
-  resolution: "@codemirror/commands@npm:6.3.3"
+  version: 6.5.0
+  resolution: "@codemirror/commands@npm:6.5.0"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.4.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.1.0
-  checksum: 7d23aecc973823969434b839aefa9a98bb47212d2ce0e6869ae903adbb5233aad22a760788fb7bb6eb45b00b01a4932fb93ad43bacdcbc0215e7500cf54b17bb
+  checksum: 27e49c5e0cb918b95d6a9f741bcc0e72cb76f963b0c829308edfb4491a37d8b12ae6fb96f9f1886b3189a22c82fec4434fbe65547dc3cd3e8dfb5222dfead2e7
   languageName: node
   linkType: hard
 
 "@codemirror/lang-cpp@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-cpp@npm:6.0.2"
   dependencies:
@@ -1415,77 +1421,77 @@
     "@lezer/common": ^1.0.2
     "@lezer/css": ^1.0.0
   checksum: 5a8457ee8a4310030a969f2d3128429f549c4dc9b7907ee8888b42119c80b65af99093801432efdf659b8ec36a147d2a947bc1ecbbf69a759395214e3f4834a8
   languageName: node
   linkType: hard
 
 "@codemirror/lang-html@npm:^6.0.0, @codemirror/lang-html@npm:^6.4.3":
-  version: 6.4.8
-  resolution: "@codemirror/lang-html@npm:6.4.8"
+  version: 6.4.9
+  resolution: "@codemirror/lang-html@npm:6.4.9"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/lang-css": ^6.0.0
     "@codemirror/lang-javascript": ^6.0.0
     "@codemirror/language": ^6.4.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
     "@lezer/css": ^1.1.0
     "@lezer/html": ^1.3.0
-  checksum: 9aec56c333cc06f9e4bb6d09806ae83e4a7f235a26b3244010e2dcea83a923cfcd7bec84904b8a59bc81256b0bb579a52bf5614962dad031d7577db1c49a216a
+  checksum: ac8c3ceb0396f2e032752c5079bd950124dca708bc64e96fc147dc5fe7133e5cee0814fe951abdb953ec1d11fa540e4b30a712b5149d9a36016a197a28de45d7
   languageName: node
   linkType: hard
 
 "@codemirror/lang-java@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-java@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/java": ^1.0.0
   checksum: 4679104683cbffcd224ac04c7e5d144b787494697b26470b07017259035b7bb3fa62609d9a61bfbc566f1756d9f972f9f26d96a3c1362dd48881c1172f9a914d
   languageName: node
   linkType: hard
 
 "@codemirror/lang-javascript@npm:^6.0.0, @codemirror/lang-javascript@npm:^6.1.7":
-  version: 6.2.1
-  resolution: "@codemirror/lang-javascript@npm:6.2.1"
+  version: 6.2.2
+  resolution: "@codemirror/lang-javascript@npm:6.2.2"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.6.0
     "@codemirror/lint": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
     "@lezer/javascript": ^1.0.0
-  checksum: 3df38c4cced06195283a9a2a9365aaa7c8c1b157852b331bc3a118403f774bbba57d2a392de52f5e28d2b344a323bc0146bcf7c8ef8be2473f167d815e4a37cd
+  checksum: 66379942a8347dff2bd76d10ed7cf313bca83872f8336fdd3e14accfef23e7b690cd913c9d11a3854fba2b32299da07fc3275995327642c9ee43c2a8e538c19d
   languageName: node
   linkType: hard
 
 "@codemirror/lang-json@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-json@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/json": ^1.0.0
   checksum: e9e87d50ff7b81bd56a6ab50740b1dd54e9a93f1be585e1d59d0642e2148842ea1528ac7b7221eb4ddc7fe84bbc28065144cc3ab86f6e06c6aeb2d4b4e62acf1
   languageName: node
   linkType: hard
 
 "@codemirror/lang-markdown@npm:^6.1.1":
-  version: 6.2.4
-  resolution: "@codemirror/lang-markdown@npm:6.2.4"
+  version: 6.2.5
+  resolution: "@codemirror/lang-markdown@npm:6.2.5"
   dependencies:
     "@codemirror/autocomplete": ^6.7.1
     "@codemirror/lang-html": ^6.0.0
     "@codemirror/language": ^6.3.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.2.1
     "@lezer/markdown": ^1.0.0
-  checksum: fbdf1388a9fd08b4e6fc9950ac57fc59ef02bb0bd3e76654158ce1494b101356ded049b65dcf6da457e7e302cb178bf30852fd152680f3a8679be3c3884c0bc2
+  checksum: 3d9e0817f888eddcb6d05ec8f0d8dacbde7b9ef7650303bc4ab8b08a550a986c60c65b1565212e06af389c31590330f1f5ed65e619a9446dc2979ff3dac0e874
   languageName: node
   linkType: hard
 
 "@codemirror/lang-php@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-php@npm:6.0.1"
   dependencies:
@@ -1495,47 +1501,47 @@
     "@lezer/common": ^1.0.0
     "@lezer/php": ^1.0.0
   checksum: c003a29a426486453fdfddbf7302982fa2aa7f059bf6f1ce4cbf08341b0162eee5e2f50e0d71c418dcd358491631780156d846fe352754d042576172c5d86721
   languageName: node
   linkType: hard
 
 "@codemirror/lang-python@npm:^6.1.3":
-  version: 6.1.4
-  resolution: "@codemirror/lang-python@npm:6.1.4"
+  version: 6.1.6
+  resolution: "@codemirror/lang-python@npm:6.1.6"
   dependencies:
     "@codemirror/autocomplete": ^6.3.2
     "@codemirror/language": ^6.8.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.2.1
     "@lezer/python": ^1.1.4
-  checksum: 94d0126bc5da4878eb3cc4da5afae4dc2ca7bb1c4c1f483e786ec0fed439490bb6ed8cad0a6090e2638e6b3453a6f4225bfaa3b49aac5cfb3e466556d0aaae1e
+  checksum: eb1faabd332bb95d0f3e227eb19ac5a31140cf238905bbe73e061040999f5680a012f9145fb3688bc2fcbb1908c957511edc8eeb8a9aa88d27d4fa55ad451e95
   languageName: node
   linkType: hard
 
 "@codemirror/lang-rust@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-rust@npm:6.0.1"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@lezer/rust": ^1.0.0
   checksum: 8a439944cb22159b0b3465ca4fa4294c69843219d5d30e278ae6df8e48f30a7a9256129723c025ec9b5e694d31a3560fb004300b125ffcd81c22d13825845170
   languageName: node
   linkType: hard
 
 "@codemirror/lang-sql@npm:^6.4.1":
-  version: 6.5.5
-  resolution: "@codemirror/lang-sql@npm:6.5.5"
+  version: 6.6.3
+  resolution: "@codemirror/lang-sql@npm:6.6.3"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 404003ae73b986bd7a00f6924db78b7ffb28fdc38d689fdc11416aaafe2d5c6dc37cc18972530f82e940acb61e18ac74a1cf7712beef448c145344ff93970dc3
+  checksum: b8e554bda9107107283674a6397cdb4816ad8bb429afd739fdc5e0339ef60170f09bdd93e7dc3eaf7f24ffaec5c7477ee42af7c05cb471990657014fac2fea1e
   languageName: node
   linkType: hard
 
 "@codemirror/lang-wast@npm:^6.0.1":
   version: 6.0.2
   resolution: "@codemirror/lang-wast@npm:6.0.2"
   dependencies:
@@ -1544,23 +1550,24 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: 72119d4a7d726c54167aa227c982ae9fa785c8ad97a158d8350ae95eecfbd8028a803eef939f7e6c5c6e626fcecda1dc37e9dffc6d5d6ec105f686aeda6b2c24
   languageName: node
   linkType: hard
 
 "@codemirror/lang-xml@npm:^6.0.2":
-  version: 6.0.2
-  resolution: "@codemirror/lang-xml@npm:6.0.2"
+  version: 6.1.0
+  resolution: "@codemirror/lang-xml@npm:6.1.0"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.4.0
     "@codemirror/state": ^6.0.0
+    "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
     "@lezer/xml": ^1.0.0
-  checksum: e156ecafaa87e9b6ef4ab6812ccd00d8f3c6cb81f232837636b36336d80513b61936dfee6f4f6800574f236208b61e95a2abcb997cdcd7366585a6b796e0e13b
+  checksum: 3a1b7af07b29ad7e53b77bf584245580b613bc92256059f175f2b1d7c28c4e39b75654fe169b9a8a330a60164b53ff5254bdb5b8ee8c6e6766427ee115c4e229
   languageName: node
   linkType: hard
 
 "@codemirror/language@npm:^6.0.0, @codemirror/language@npm:^6.3.0, @codemirror/language@npm:^6.4.0, @codemirror/language@npm:^6.6.0, @codemirror/language@npm:^6.8.0":
   version: 6.10.1
   resolution: "@codemirror/language@npm:6.10.1"
   dependencies:
@@ -1571,30 +1578,30 @@
     "@lezer/lr": ^1.0.0
     style-mod: ^4.0.0
   checksum: 453bbe122a84795752f29261412b69a8dcfdd7e4369eb7e112bffba36b9e527ad21adff1d3845e0dc44c9ab44eb0c6f823eb6ba790ddd00cc749847574eda779
   languageName: node
   linkType: hard
 
 "@codemirror/legacy-modes@npm:^6.3.2":
-  version: 6.3.3
-  resolution: "@codemirror/legacy-modes@npm:6.3.3"
+  version: 6.4.0
+  resolution: "@codemirror/legacy-modes@npm:6.4.0"
   dependencies:
     "@codemirror/language": ^6.0.0
-  checksum: 3cd32b0f011b0a193e0948e5901b625f38aa6d9a8b24344531d6e142eb6fbb3e6cb5969429102044f3d04fbe53c4deaebd9f659c05067a0b18d17766290c9e05
+  checksum: d382aa6f640a67418bd209e1e4b395340f96aac1b0cf185927fc2c7f98b62cfd0c59ef0f7048148ce8771622003ca844c78c2d18548235ecc57d0bcbfbbfe091
   languageName: node
   linkType: hard
 
 "@codemirror/lint@npm:^6.0.0":
-  version: 6.5.0
-  resolution: "@codemirror/lint@npm:6.5.0"
+  version: 6.6.0
+  resolution: "@codemirror/lint@npm:6.6.0"
   dependencies:
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
-  checksum: b4f3899d0f73e5a2b5e9bc1df8e13ecb9324b94c7d384e7c8dde794109dee051461fc86658338f41652b44879b2ccc12cdd51a8ac0bb16a5b18aafa8e57a843c
+  checksum: e68b53b051742143b50067663af8b0fe88615d5cdaa18497f888b3ea0e130c1af47525821a5a81efc45f828dbf15bb56348de1ec329f411bdd0ba3b000846555
   languageName: node
   linkType: hard
 
 "@codemirror/search@npm:^6.3.0":
   version: 6.5.6
   resolution: "@codemirror/search@npm:6.5.6"
   dependencies:
@@ -1602,28 +1609,28 @@
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
   checksum: 19dc88d09fc750563347001e83c6194bbb2a25c874bd919d2d81809e1f98d6330222ddbd284aa9758a09eeb41fd153ec7c2cf810b2ee51452c25963d7f5833d5
   languageName: node
   linkType: hard
 
 "@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.2.0, @codemirror/state@npm:^6.4.0":
-  version: 6.4.0
-  resolution: "@codemirror/state@npm:6.4.0"
-  checksum: c5236fe5786f1b85d17273a5c17fa8aeb063658c1404ab18caeb6e7591663ec96b65d453ab8162f75839c3801b04cd55ba4bc48f44cb61ebfeeee383f89553c7
+  version: 6.4.1
+  resolution: "@codemirror/state@npm:6.4.1"
+  checksum: b81b55574091349eed4d32fc0eadb0c9688f1f7c98b681318f59138ee0f527cb4c4a97831b70547c0640f02f3127647838ae6730782de4a3dd2cc58836125d01
   languageName: node
   linkType: hard
 
 "@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.23.0, @codemirror/view@npm:^6.9.6":
-  version: 6.23.1
-  resolution: "@codemirror/view@npm:6.23.1"
+  version: 6.26.3
+  resolution: "@codemirror/view@npm:6.26.3"
   dependencies:
     "@codemirror/state": ^6.4.0
     style-mod: ^4.1.0
     w3c-keyname: ^2.2.4
-  checksum: 5ea3ba5761c574e1f6e1f1058cb452189c890982a77991606d0ae40da3c6fff77f7c7fc3c43fa78d62677ccdfa65dbc56175706b793e34ad4ec7a63b21e8c18e
+  checksum: fdee35fb5e0bbba7b6f1a9b43a865880911bbfafd30360da5dda21b35f81ba2d080ff66b6c3d94dbe946b6b7ec98a76208786360b8f030ef10bcb054b816de05
   languageName: node
   linkType: hard
 
 "@csstools/selector-specificity@npm:^2.0.2":
   version: 2.2.0
   resolution: "@csstools/selector-specificity@npm:2.2.0"
   peerDependencies:
@@ -1670,29 +1677,29 @@
     js-yaml: ^4.1.0
     minimatch: ^3.1.2
     strip-json-comments: ^3.1.1
   checksum: 10957c7592b20ca0089262d8c2a8accbad14b4f6507e35416c32ee6b4dbf9cad67dfb77096bbd405405e9ada2b107f3797fe94362e1c55e0b09d6e90dd149127
   languageName: node
   linkType: hard
 
-"@eslint/js@npm:8.56.0":
-  version: 8.56.0
-  resolution: "@eslint/js@npm:8.56.0"
-  checksum: 5804130574ef810207bdf321c265437814e7a26f4e6fac9b496de3206afd52f533e09ec002a3be06cd9adcc9da63e727f1883938e663c4e4751c007d5b58e539
+"@eslint/js@npm:8.57.0":
+  version: 8.57.0
+  resolution: "@eslint/js@npm:8.57.0"
+  checksum: 315dc65b0e9893e2bff139bddace7ea601ad77ed47b4550e73da8c9c2d2766c7a575c3cddf17ef85b8fd6a36ff34f91729d0dcca56e73ca887c10df91a41b0bb
   languageName: node
   linkType: hard
 
 "@fortawesome/fontawesome-free@npm:^5.12.0":
   version: 5.15.4
   resolution: "@fortawesome/fontawesome-free@npm:5.15.4"
   checksum: 32281c3df4075290d9a96dfc22f72fadb3da7055d4117e48d34046b8c98032a55fa260ae351b0af5d6f6fb57a2f5d79a4abe52af456da35195f7cb7dda27b4a2
   languageName: node
   linkType: hard
 
-"@humanwhocodes/config-array@npm:^0.11.13":
+"@humanwhocodes/config-array@npm:^0.11.14":
   version: 0.11.14
   resolution: "@humanwhocodes/config-array@npm:0.11.14"
   dependencies:
     "@humanwhocodes/object-schema": ^2.0.2
     debug: ^4.3.1
     minimatch: ^3.0.5
   checksum: 861ccce9eaea5de19546653bccf75bf09fe878bc39c3aab00aeee2d2a0e654516adad38dd1098aab5e3af0145bbcbf3f309bdf4d964f8dab9dcd5834ae4c02f2
@@ -1703,17 +1710,17 @@
   version: 1.0.1
   resolution: "@humanwhocodes/module-importer@npm:1.0.1"
   checksum: 0fd22007db8034a2cdf2c764b140d37d9020bbfce8a49d3ec5c05290e77d4b0263b1b972b752df8c89e5eaa94073408f2b7d977aed131faf6cf396ebb5d7fb61
   languageName: node
   linkType: hard
 
 "@humanwhocodes/object-schema@npm:^2.0.2":
-  version: 2.0.2
-  resolution: "@humanwhocodes/object-schema@npm:2.0.2"
-  checksum: 2fc11503361b5fb4f14714c700c02a3f4c7c93e9acd6b87a29f62c522d90470f364d6161b03d1cc618b979f2ae02aed1106fd29d302695d8927e2fc8165ba8ee
+  version: 2.0.3
+  resolution: "@humanwhocodes/object-schema@npm:2.0.3"
+  checksum: d3b78f6c5831888c6ecc899df0d03bcc25d46f3ad26a11d7ea52944dc36a35ef543fad965322174238d677a43d5c694434f6607532cff7077062513ad7022631
   languageName: node
   linkType: hard
 
 "@isaacs/cliui@npm:^8.0.2":
   version: 8.0.2
   resolution: "@isaacs/cliui@npm:8.0.2"
   dependencies:
@@ -1736,15 +1743,15 @@
     get-package-type: ^0.1.0
     js-yaml: ^3.13.1
     resolve-from: ^5.0.0
   checksum: d578da5e2e804d5c93228450a1380e1a3c691de4953acc162f387b717258512a3e07b83510a936d9fab03eac90817473917e24f5d16297af3867f59328d58568
   languageName: node
   linkType: hard
 
-"@istanbuljs/schema@npm:^0.1.2":
+"@istanbuljs/schema@npm:^0.1.2, @istanbuljs/schema@npm:^0.1.3":
   version: 0.1.3
   resolution: "@istanbuljs/schema@npm:0.1.3"
   checksum: 5282759d961d61350f33d9118d16bcaed914ebf8061a52f4fa474b2cb08720c9c81d165e13b82f2e5a8a212cc5af482f0c6fc1ac27b9e067e5394c9a6ed186c9
   languageName: node
   linkType: hard
 
 "@jest/console@npm:^29.7.0":
@@ -1973,86 +1980,86 @@
     "@types/node": "*"
     "@types/yargs": ^17.0.8
     chalk: ^4.0.0
   checksum: a0bcf15dbb0eca6bdd8ce61a3fb055349d40268622a7670a3b2eb3c3dbafe9eb26af59938366d520b86907b9505b0f9b29b85cec11579a9e580694b87cd90fcc
   languageName: node
   linkType: hard
 
-"@jridgewell/gen-mapping@npm:^0.3.0, @jridgewell/gen-mapping@npm:^0.3.2":
-  version: 0.3.3
-  resolution: "@jridgewell/gen-mapping@npm:0.3.3"
+"@jridgewell/gen-mapping@npm:^0.3.5":
+  version: 0.3.5
+  resolution: "@jridgewell/gen-mapping@npm:0.3.5"
   dependencies:
-    "@jridgewell/set-array": ^1.0.1
+    "@jridgewell/set-array": ^1.2.1
     "@jridgewell/sourcemap-codec": ^1.4.10
-    "@jridgewell/trace-mapping": ^0.3.9
-  checksum: 4a74944bd31f22354fc01c3da32e83c19e519e3bbadafa114f6da4522ea77dd0c2842607e923a591d60a76699d819a2fbb6f3552e277efdb9b58b081390b60ab
+    "@jridgewell/trace-mapping": ^0.3.24
+  checksum: ff7a1764ebd76a5e129c8890aa3e2f46045109dabde62b0b6c6a250152227647178ff2069ea234753a690d8f3c4ac8b5e7b267bbee272bffb7f3b0a370ab6e52
   languageName: node
   linkType: hard
 
 "@jridgewell/resolve-uri@npm:^3.1.0":
-  version: 3.1.1
-  resolution: "@jridgewell/resolve-uri@npm:3.1.1"
-  checksum: f5b441fe7900eab4f9155b3b93f9800a916257f4e8563afbcd3b5a5337b55e52bd8ae6735453b1b745457d9f6cdb16d74cd6220bbdd98cf153239e13f6cbb653
+  version: 3.1.2
+  resolution: "@jridgewell/resolve-uri@npm:3.1.2"
+  checksum: 83b85f72c59d1c080b4cbec0fef84528963a1b5db34e4370fa4bd1e3ff64a0d80e0cee7369d11d73c704e0286fb2865b530acac7a871088fbe92b5edf1000870
   languageName: node
   linkType: hard
 
-"@jridgewell/set-array@npm:^1.0.1":
-  version: 1.1.2
-  resolution: "@jridgewell/set-array@npm:1.1.2"
-  checksum: 69a84d5980385f396ff60a175f7177af0b8da4ddb81824cb7016a9ef914eee9806c72b6b65942003c63f7983d4f39a5c6c27185bbca88eb4690b62075602e28e
+"@jridgewell/set-array@npm:^1.2.1":
+  version: 1.2.1
+  resolution: "@jridgewell/set-array@npm:1.2.1"
+  checksum: 832e513a85a588f8ed4f27d1279420d8547743cc37fcad5a5a76fc74bb895b013dfe614d0eed9cb860048e6546b798f8f2652020b4b2ba0561b05caa8c654b10
   languageName: node
   linkType: hard
 
 "@jridgewell/source-map@npm:^0.3.3":
-  version: 0.3.5
-  resolution: "@jridgewell/source-map@npm:0.3.5"
+  version: 0.3.6
+  resolution: "@jridgewell/source-map@npm:0.3.6"
   dependencies:
-    "@jridgewell/gen-mapping": ^0.3.0
-    "@jridgewell/trace-mapping": ^0.3.9
-  checksum: 1ad4dec0bdafbade57920a50acec6634f88a0eb735851e0dda906fa9894e7f0549c492678aad1a10f8e144bfe87f238307bf2a914a1bc85b7781d345417e9f6f
+    "@jridgewell/gen-mapping": ^0.3.5
+    "@jridgewell/trace-mapping": ^0.3.25
+  checksum: c9dc7d899397df95e3c9ec287b93c0b56f8e4453cd20743e2b9c8e779b1949bc3cccf6c01bb302779e46560eb45f62ea38d19fedd25370d814734268450a9f30
   languageName: node
   linkType: hard
 
 "@jridgewell/sourcemap-codec@npm:^1.4.10, @jridgewell/sourcemap-codec@npm:^1.4.14":
   version: 1.4.15
   resolution: "@jridgewell/sourcemap-codec@npm:1.4.15"
   checksum: b881c7e503db3fc7f3c1f35a1dd2655a188cc51a3612d76efc8a6eb74728bef5606e6758ee77423e564092b4a518aba569bbb21c9bac5ab7a35b0c6ae7e344c8
   languageName: node
   linkType: hard
 
-"@jridgewell/trace-mapping@npm:^0.3.12, @jridgewell/trace-mapping@npm:^0.3.17, @jridgewell/trace-mapping@npm:^0.3.18, @jridgewell/trace-mapping@npm:^0.3.20, @jridgewell/trace-mapping@npm:^0.3.9":
-  version: 0.3.22
-  resolution: "@jridgewell/trace-mapping@npm:0.3.22"
+"@jridgewell/trace-mapping@npm:^0.3.12, @jridgewell/trace-mapping@npm:^0.3.18, @jridgewell/trace-mapping@npm:^0.3.20, @jridgewell/trace-mapping@npm:^0.3.24, @jridgewell/trace-mapping@npm:^0.3.25":
+  version: 0.3.25
+  resolution: "@jridgewell/trace-mapping@npm:0.3.25"
   dependencies:
     "@jridgewell/resolve-uri": ^3.1.0
     "@jridgewell/sourcemap-codec": ^1.4.14
-  checksum: ac7dd2cfe0b479aa1b81776d40d789243131cc792dc8b6b6a028c70fcd6171958ae1a71bf67b618ffe3c0c3feead9870c095ee46a5e30319410d92976b28f498
+  checksum: 9d3c40d225e139987b50c48988f8717a54a8c994d8a948ee42e1412e08988761d0754d7d10b803061cc3aebf35f92a5dbbab493bd0e1a9ef9e89a2130e83ba34
   languageName: node
   linkType: hard
 
 "@jupyter/react-components@npm:^0.15.2":
-  version: 0.15.2
-  resolution: "@jupyter/react-components@npm:0.15.2"
+  version: 0.15.3
+  resolution: "@jupyter/react-components@npm:0.15.3"
   dependencies:
-    "@jupyter/web-components": ^0.15.2
+    "@jupyter/web-components": ^0.15.3
     "@microsoft/fast-react-wrapper": ^0.3.22
     react: ">=17.0.0 <19.0.0"
-  checksum: d6d339ff9c2fed1fd5afda612be500d73c4a83eee5470d50e94020dadd1e389a3bf745c7240b0a48edbc6d3fdacec93367b7b5e40588f2df588419caada705be
+  checksum: 1a6b256314259c6465c4b6d958575710536b82234a7bf0fba3e889a07e1f19ff8ab321450be354359876f92c45dbcc9d21a840237ff4a619806d9de696f55496
   languageName: node
   linkType: hard
 
-"@jupyter/web-components@npm:^0.15.2":
-  version: 0.15.2
-  resolution: "@jupyter/web-components@npm:0.15.2"
+"@jupyter/web-components@npm:^0.15.2, @jupyter/web-components@npm:^0.15.3":
+  version: 0.15.3
+  resolution: "@jupyter/web-components@npm:0.15.3"
   dependencies:
     "@microsoft/fast-colors": ^5.3.1
     "@microsoft/fast-element": ^1.12.0
     "@microsoft/fast-foundation": ^2.49.4
     "@microsoft/fast-web-utilities": ^5.4.1
-  checksum: f272ef91de08e28f9414a26dbd2388e1a8985c90f4ab00231978cee49bd5212f812411397a9038d298c8c0c4b41eb28cc86f1127bc7ace309bda8df60c4a87c8
+  checksum: a0980af934157bfdbdb6cc169c0816c1b2e57602d524c56bdcef746a4c25dfeb8f505150d83207c8695ed89b5486cf53d35a3382584d25ef64db666e4e16e45b
   languageName: node
   linkType: hard
 
 "@jupyter/ydoc@npm:^1.1.1":
   version: 1.1.1
   resolution: "@jupyter/ydoc@npm:1.1.1"
   dependencies:
@@ -2062,88 +2069,88 @@
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   checksum: a239b1dd57cfc9ba36c06ac5032a1b6388849ae01a1d0db0d45094f71fdadf4d473b4bf8becbef0cfcdc85cae505361fbec0822b02da5aa48e06b66f742dd7a0
   languageName: node
   linkType: hard
 
-"@jupyterlab/application@npm:^4.0.0, @jupyterlab/application@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/application@npm:4.1.0"
+"@jupyterlab/application@npm:^4.0.0, @jupyterlab/application@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/application@npm:4.1.8"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/docregistry": ^4.1.0
-    "@jupyterlab/rendermime": ^4.1.0
-    "@jupyterlab/rendermime-interfaces": ^3.9.0
-    "@jupyterlab/services": ^7.1.0
-    "@jupyterlab/statedb": ^4.1.0
-    "@jupyterlab/translation": ^4.1.0
-    "@jupyterlab/ui-components": ^4.1.0
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/docregistry": ^4.1.8
+    "@jupyterlab/rendermime": ^4.1.8
+    "@jupyterlab/rendermime-interfaces": ^3.9.8
+    "@jupyterlab/services": ^7.1.8
+    "@jupyterlab/statedb": ^4.1.8
+    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/ui-components": ^4.1.8
     "@lumino/algorithm": ^2.0.1
     "@lumino/application": ^2.3.0
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
-  checksum: 1ca13156bee6e07850c008b1c8c510073bfd74c1c5056014313bfda1503db0b19472e727d549bb8461f17fdb6cd10fb3db854aa9f4cefb5599a4fc73017d46e7
+  checksum: 33c57c7e825f72f8aca146bfb2ade9c91e55ac5218410ff4472b0e4cf0de0305ec34f94a9ff3ab5e8982c37a170225dbfe47b4ac900980837ecaf00b7effb0fc
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.2.0":
-  version: 4.2.0
-  resolution: "@jupyterlab/apputils@npm:4.2.0"
+"@jupyterlab/apputils@npm:^4.2.8":
+  version: 4.2.8
+  resolution: "@jupyterlab/apputils@npm:4.2.8"
   dependencies:
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/observables": ^5.1.0
-    "@jupyterlab/rendermime-interfaces": ^3.9.0
-    "@jupyterlab/services": ^7.1.0
-    "@jupyterlab/settingregistry": ^4.1.0
-    "@jupyterlab/statedb": ^4.1.0
-    "@jupyterlab/statusbar": ^4.1.0
-    "@jupyterlab/translation": ^4.1.0
-    "@jupyterlab/ui-components": ^4.1.0
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/observables": ^5.1.8
+    "@jupyterlab/rendermime-interfaces": ^3.9.8
+    "@jupyterlab/services": ^7.1.8
+    "@jupyterlab/settingregistry": ^4.1.8
+    "@jupyterlab/statedb": ^4.1.8
+    "@jupyterlab/statusbar": ^4.1.8
+    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/ui-components": ^4.1.8
     "@lumino/algorithm": ^2.0.1
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.1
     "@types/react": ^18.0.26
     react: ^18.2.0
     sanitize-html: ~2.7.3
-  checksum: aec06e0e1403850676e766061d847e7cefa7225cdf48bbd2f3ab3f8356cb306646bf57dc15bcda149aa700e87850425ab8b79299d3414751a1753747ef9f15ba
+  checksum: 253b3a21f292b19791e149926014e90eb0e6e074b86422a63ce2fbfaebc53c6e16c6cd628f79d91eb7e66b60357df79b9dc6de683b5293562f9fcbe39bcd0522
   languageName: node
   linkType: hard
 
-"@jupyterlab/attachments@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/attachments@npm:4.1.0"
+"@jupyterlab/attachments@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/attachments@npm:4.1.8"
   dependencies:
-    "@jupyterlab/nbformat": ^4.1.0
-    "@jupyterlab/observables": ^5.1.0
-    "@jupyterlab/rendermime": ^4.1.0
-    "@jupyterlab/rendermime-interfaces": ^3.9.0
+    "@jupyterlab/nbformat": ^4.1.8
+    "@jupyterlab/observables": ^5.1.8
+    "@jupyterlab/rendermime": ^4.1.8
+    "@jupyterlab/rendermime-interfaces": ^3.9.8
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
-  checksum: ddb1716f7e9d0a7272979dc82109c17069b2b618142e289e2127a1b59eecf3ddc02cf8665b1f1ae42a3c8fbbc90f2d6ba270455381cdeec3d5d1be7488ca8a5c
+  checksum: 496eb41e8335d237f7c88b5ce7d1194292d4e6ab8952a3a62883bf4daea36dc6e426ce97b039583ea0e9b9a3ec72e755b2d842e3fc562747efe517e34930f25e
   languageName: node
   linkType: hard
 
 "@jupyterlab/builder@npm:^4.0.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/builder@npm:4.1.0"
+  version: 4.1.8
+  resolution: "@jupyterlab/builder@npm:4.1.8"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/application": ^2.3.0
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
@@ -2170,81 +2177,81 @@
     terser-webpack-plugin: ^5.3.7
     webpack: ^5.76.1
     webpack-cli: ^5.0.1
     webpack-merge: ^5.8.0
     worker-loader: ^3.0.2
   bin:
     build-labextension: lib/build-labextension.js
-  checksum: 1a8f684fbf31fef2bae93b84e79af12bd0e70cedc5546f7501a17147425616ffd7ec42586ba23e9d6eb6a79e40d651f6f87d9c1c496ed26f84a2990da8631958
+  checksum: e727e4fddbfd4e8f7d4c83e5c5aaf9be41b67771f6a4ef10b44bbc0e51bb21966b2fa1ad33eacf58420ca3a2cda2ab410331a1543e6f945b9ca0a59e109f240b
   languageName: node
   linkType: hard
 
-"@jupyterlab/cells@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/cells@npm:4.1.0"
+"@jupyterlab/cells@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/cells@npm:4.1.8"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/attachments": ^4.1.0
-    "@jupyterlab/codeeditor": ^4.1.0
-    "@jupyterlab/codemirror": ^4.1.0
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/documentsearch": ^4.1.0
-    "@jupyterlab/filebrowser": ^4.1.0
-    "@jupyterlab/nbformat": ^4.1.0
-    "@jupyterlab/observables": ^5.1.0
-    "@jupyterlab/outputarea": ^4.1.0
-    "@jupyterlab/rendermime": ^4.1.0
-    "@jupyterlab/services": ^7.1.0
-    "@jupyterlab/toc": ^6.1.0
-    "@jupyterlab/translation": ^4.1.0
-    "@jupyterlab/ui-components": ^4.1.0
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/attachments": ^4.1.8
+    "@jupyterlab/codeeditor": ^4.1.8
+    "@jupyterlab/codemirror": ^4.1.8
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/documentsearch": ^4.1.8
+    "@jupyterlab/filebrowser": ^4.1.8
+    "@jupyterlab/nbformat": ^4.1.8
+    "@jupyterlab/observables": ^5.1.8
+    "@jupyterlab/outputarea": ^4.1.8
+    "@jupyterlab/rendermime": ^4.1.8
+    "@jupyterlab/services": ^7.1.8
+    "@jupyterlab/toc": ^6.1.8
+    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/ui-components": ^4.1.8
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 41fb5dddda54ff53d828eff9f142092966214dadff7d93d6d91777746a36fcd192bc5a4055e364185fb367f6d3ed462946d214a33ba0ed63037b83b683958c44
+  checksum: feb2aa9b681acaae78aadffce6d9c61c6b7d4c15da23f11accf98a5d36891918a7304260f73e6b39512fadb8cc31b433bf8619cbb8d7c5c410d5c14b78558364
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/codeeditor@npm:4.1.0"
+"@jupyterlab/codeeditor@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/codeeditor@npm:4.1.8"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/nbformat": ^4.1.0
-    "@jupyterlab/observables": ^5.1.0
-    "@jupyterlab/statusbar": ^4.1.0
-    "@jupyterlab/translation": ^4.1.0
-    "@jupyterlab/ui-components": ^4.1.0
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/nbformat": ^4.1.8
+    "@jupyterlab/observables": ^5.1.8
+    "@jupyterlab/statusbar": ^4.1.8
+    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/ui-components": ^4.1.8
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: ae58f6cb446f98b781a956986fcb497b53f380ed86510d67b13e3086cee434423d5a03c26a130ea8d02c762cd6a6cbc62fd088c6f60f78d4bb558102e4c80ad8
+  checksum: e5d3b0f5c94775017b044528843596ce7f5616cede5555a6a32b3a8e9ae583775f83a6448717fd15e2cf254ef50209861da06821f67267ebe2ef67b34860f7d6
   languageName: node
   linkType: hard
 
-"@jupyterlab/codemirror@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/codemirror@npm:4.1.0"
+"@jupyterlab/codemirror@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/codemirror@npm:4.1.8"
   dependencies:
     "@codemirror/autocomplete": ^6.5.1
     "@codemirror/commands": ^6.2.3
     "@codemirror/lang-cpp": ^6.0.2
     "@codemirror/lang-css": ^6.1.1
     "@codemirror/lang-html": ^6.4.3
     "@codemirror/lang-java": ^6.0.1
@@ -2259,425 +2266,425 @@
     "@codemirror/lang-xml": ^6.0.2
     "@codemirror/language": ^6.6.0
     "@codemirror/legacy-modes": ^6.3.2
     "@codemirror/search": ^6.3.0
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/codeeditor": ^4.1.0
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/documentsearch": ^4.1.0
-    "@jupyterlab/nbformat": ^4.1.0
-    "@jupyterlab/translation": ^4.1.0
+    "@jupyterlab/codeeditor": ^4.1.8
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/documentsearch": ^4.1.8
+    "@jupyterlab/nbformat": ^4.1.8
+    "@jupyterlab/translation": ^4.1.8
     "@lezer/common": ^1.0.2
     "@lezer/generator": ^1.2.2
     "@lezer/highlight": ^1.1.4
     "@lezer/markdown": ^1.0.2
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     yjs: ^13.5.40
-  checksum: 92fb4ebebe4b5926fbf5ba2a99f845e8879918b3a095adf99de5f8385b3168412db38ebe2f1ae1eff8f29304d2c8c1b31c3cc1ba66a9c2d16e7a69dced20a768
+  checksum: 0a56b6855b6dd4999e9816938f7546c2f1c46c629f05cf246813d58700f3c283e068b9c86dba275374756536472b598a19a0e5e12cfffd365817fbcc8333c795
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.1.0":
-  version: 6.1.0
-  resolution: "@jupyterlab/coreutils@npm:6.1.0"
+"@jupyterlab/coreutils@npm:^6.1.8":
+  version: 6.1.8
+  resolution: "@jupyterlab/coreutils@npm:6.1.8"
   dependencies:
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: d1fdeb3fa28af76cab52c04c82b51a1f02f9cd7779dc1eecbd1177bf246d0213c4e7234bf74eb1bd1d909123988e40addbec8fd7a027c4f5448f3c968b27642c
+  checksum: 1049c78bdbffb247fe7e7be4e082fe15711ca0d8da997d6da7042e0299d7ebbf1d0341d830ae0ab451bf8dfbfc30027bf3f063fc7e35210409a7aa56fe94cee9
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/docmanager@npm:4.1.0"
+"@jupyterlab/docmanager@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/docmanager@npm:4.1.8"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/docregistry": ^4.1.0
-    "@jupyterlab/services": ^7.1.0
-    "@jupyterlab/statusbar": ^4.1.0
-    "@jupyterlab/translation": ^4.1.0
-    "@jupyterlab/ui-components": ^4.1.0
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/docregistry": ^4.1.8
+    "@jupyterlab/services": ^7.1.8
+    "@jupyterlab/statusbar": ^4.1.8
+    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/ui-components": ^4.1.8
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 64f63512a862c2539f3eb1eb255ad6d1c3d5380519079b745503b38eebba255af4d12688b57d42c83a0220758b5cd8304012044cab18433f1c35ca6e49356719
+  checksum: d0d1316a885d1e72891d9b9cd61c36c7f8db4a4e53ae4cc8f105931e0dcdc262ebd5e76d3a145517bcc009cb3f8ab23e4e4ce84191f2f09c5df3d2a3294cfe9a
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/docregistry@npm:4.1.0"
+"@jupyterlab/docregistry@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/docregistry@npm:4.1.8"
   dependencies:
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/codeeditor": ^4.1.0
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/observables": ^5.1.0
-    "@jupyterlab/rendermime": ^4.1.0
-    "@jupyterlab/rendermime-interfaces": ^3.9.0
-    "@jupyterlab/services": ^7.1.0
-    "@jupyterlab/translation": ^4.1.0
-    "@jupyterlab/ui-components": ^4.1.0
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/codeeditor": ^4.1.8
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/observables": ^5.1.8
+    "@jupyterlab/rendermime": ^4.1.8
+    "@jupyterlab/rendermime-interfaces": ^3.9.8
+    "@jupyterlab/services": ^7.1.8
+    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/ui-components": ^4.1.8
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 8407ea92d2f7a094ea47313917b7d32ce6a9e7dd79ab595eeef4064d805f818720210cde3c949b517ba98bae52980ab373df42082ca654f0f483935e104f0335
+  checksum: d65aef500ab8d9d761490cf2a6902e897475173727cd3676691789e6d2609aefc8c98c0a4d4e57c670721409cb58925eeb162dbd101c9b6a473ecd20cf7efe78
   languageName: node
   linkType: hard
 
-"@jupyterlab/documentsearch@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/documentsearch@npm:4.1.0"
+"@jupyterlab/documentsearch@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/documentsearch@npm:4.1.8"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/translation": ^4.1.0
-    "@jupyterlab/ui-components": ^4.1.0
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/ui-components": ^4.1.8
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 768b02f07c892622b126d8b8f59e4559003f3900f2cb588fba27aa87ebb1eb9a703fe99ebccc9bd8ccba2f8859ba157060b0bb5e5c5572fe9906fd7152caf536
+  checksum: c8f05403435c8613c599ea54512f4a8bb865e3836f336e2258cba60291b101f35515eb6e8a33d88973d22fffe2b9772d1b0d9d177a5b7a396ff64b046b211580
   languageName: node
   linkType: hard
 
-"@jupyterlab/filebrowser@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/filebrowser@npm:4.1.0"
-  dependencies:
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/docmanager": ^4.1.0
-    "@jupyterlab/docregistry": ^4.1.0
-    "@jupyterlab/services": ^7.1.0
-    "@jupyterlab/statedb": ^4.1.0
-    "@jupyterlab/statusbar": ^4.1.0
-    "@jupyterlab/translation": ^4.1.0
-    "@jupyterlab/ui-components": ^4.1.0
+"@jupyterlab/filebrowser@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/filebrowser@npm:4.1.8"
+  dependencies:
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/docmanager": ^4.1.8
+    "@jupyterlab/docregistry": ^4.1.8
+    "@jupyterlab/services": ^7.1.8
+    "@jupyterlab/statedb": ^4.1.8
+    "@jupyterlab/statusbar": ^4.1.8
+    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/ui-components": ^4.1.8
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: ee29ad3a5ca3d9477a760179ff8b520cb88b8fd08f62ecd872d0cc0c5e1cc397349b020ba8c24f9b543b9cd5513c3b9da813d41bc5a63464aa3321a31b613115
+  checksum: 51ae88c5fabb2fad341cd3ea7b94750c373d5b3d251287f0bcbc7f1357b11f7a4e9ec08ee92512a46435fccee0c7c647cdf2185db9459a55845d15410f0dcf1c
   languageName: node
   linkType: hard
 
-"@jupyterlab/lsp@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/lsp@npm:4.1.0"
+"@jupyterlab/lsp@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/lsp@npm:4.1.8"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/codeeditor": ^4.1.0
-    "@jupyterlab/codemirror": ^4.1.0
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/docregistry": ^4.1.0
-    "@jupyterlab/services": ^7.1.0
-    "@jupyterlab/translation": ^4.1.0
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/codeeditor": ^4.1.8
+    "@jupyterlab/codemirror": ^4.1.8
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/docregistry": ^4.1.8
+    "@jupyterlab/services": ^7.1.8
+    "@jupyterlab/translation": ^4.1.8
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     lodash.mergewith: ^4.6.1
     vscode-jsonrpc: ^6.0.0
     vscode-languageserver-protocol: ^3.17.0
     vscode-ws-jsonrpc: ~1.0.2
-  checksum: 487e4d2609ed4212be79c00f45f445ebb252d3a37a537adc421d1cc7824a45c782578cbf5876b75e1a184a2d4a0cc9ec232494e4440b082062a63278ede502d3
+  checksum: 535786735c28c8cd6b3a39c2ae0d8e7b4d7b39c96346595fea6c39f4c81b55c986025e27b6a5f874d16319eab09022eb3d9ae7114ecbdcf688712838858f1590
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/nbformat@npm:4.1.0"
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/nbformat@npm:4.1.8"
   dependencies:
     "@lumino/coreutils": ^2.1.2
-  checksum: 0f10f53d312e1ad386be0cd1db3ea8d76ac5e169a1c470465179b35c7d7bd0e55b9d450b64abe38f447dcbec71224bfe8d4115a1cdb433f986d3a91234ffd391
+  checksum: 11d89ae6fb2385a00e60ab84defc61e3cf28510b029ffbe9ffe27a75bc84f85e64a0d0d16b6deb7b57256fdd651d842a0626128def511e7755121a5a0a71f078
   languageName: node
   linkType: hard
 
-"@jupyterlab/notebook@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/notebook@npm:4.1.0"
+"@jupyterlab/notebook@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/notebook@npm:4.1.8"
   dependencies:
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/cells": ^4.1.0
-    "@jupyterlab/codeeditor": ^4.1.0
-    "@jupyterlab/codemirror": ^4.1.0
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/docregistry": ^4.1.0
-    "@jupyterlab/documentsearch": ^4.1.0
-    "@jupyterlab/lsp": ^4.1.0
-    "@jupyterlab/nbformat": ^4.1.0
-    "@jupyterlab/observables": ^5.1.0
-    "@jupyterlab/rendermime": ^4.1.0
-    "@jupyterlab/services": ^7.1.0
-    "@jupyterlab/settingregistry": ^4.1.0
-    "@jupyterlab/statusbar": ^4.1.0
-    "@jupyterlab/toc": ^6.1.0
-    "@jupyterlab/translation": ^4.1.0
-    "@jupyterlab/ui-components": ^4.1.0
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/cells": ^4.1.8
+    "@jupyterlab/codeeditor": ^4.1.8
+    "@jupyterlab/codemirror": ^4.1.8
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/docregistry": ^4.1.8
+    "@jupyterlab/documentsearch": ^4.1.8
+    "@jupyterlab/lsp": ^4.1.8
+    "@jupyterlab/nbformat": ^4.1.8
+    "@jupyterlab/observables": ^5.1.8
+    "@jupyterlab/rendermime": ^4.1.8
+    "@jupyterlab/services": ^7.1.8
+    "@jupyterlab/settingregistry": ^4.1.8
+    "@jupyterlab/statusbar": ^4.1.8
+    "@jupyterlab/toc": ^6.1.8
+    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/ui-components": ^4.1.8
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 0083ef437c3db33d5fdbb72e176f4aa74e3f07a9bdd7868dc72deef65ee50de75156c92c9e9be4464d498225867488e7b177668579a3996869819d1e1e14bf53
+  checksum: ec1044f23cbbcaa5a6d1057f2f26640630a3c31f4d2fc9930da5dc6665fcf041ab4472952f13dd863eb29a91ed3af2e8a4eee5eff2d329b381b8f0a5865f52ef
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.1.0":
-  version: 5.1.0
-  resolution: "@jupyterlab/observables@npm:5.1.0"
+"@jupyterlab/observables@npm:^5.1.8":
+  version: 5.1.8
+  resolution: "@jupyterlab/observables@npm:5.1.8"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: 38ee528b244b06a2813874e11d2c3aa8b576f98ffdf9f77fc6c9ddf49de296b4067b4ad7f41f5eaab1de50d16fc79a31d26a34963e09c259e4332cf15c0c7bd5
+  checksum: c349b4fea92ef28019c0b3f5a100abdd4384554188d6741234e90e03f3f18b343a22ea8560f9d2eea1a00d4cd9514074d195ec850e930785f28a2f8a624a0f4d
   languageName: node
   linkType: hard
 
-"@jupyterlab/outputarea@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/outputarea@npm:4.1.0"
+"@jupyterlab/outputarea@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/outputarea@npm:4.1.8"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/nbformat": ^4.1.0
-    "@jupyterlab/observables": ^5.1.0
-    "@jupyterlab/rendermime": ^4.1.0
-    "@jupyterlab/rendermime-interfaces": ^3.9.0
-    "@jupyterlab/services": ^7.1.0
-    "@jupyterlab/translation": ^4.1.0
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/nbformat": ^4.1.8
+    "@jupyterlab/observables": ^5.1.8
+    "@jupyterlab/rendermime": ^4.1.8
+    "@jupyterlab/rendermime-interfaces": ^3.9.8
+    "@jupyterlab/services": ^7.1.8
+    "@jupyterlab/translation": ^4.1.8
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
-  checksum: 069d5d5fa1e75f5a09421e22fbaa15729f8bbc93c3915f9c0a8bee404a663b8def6c0c0d82a85d84cc6c4e3bdda87eb3d7820eb74e1cf1b99b834ee49ccf572f
+  checksum: deb86addc7c43794442cdec2097946be949accd081aec51029cf0c6b53e4a950be1cfd9d9621059e580b9e45255a8bf971966ae8ecebec2358579462f7396b8b
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime-interfaces@npm:^3.9.0":
-  version: 3.9.0
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.9.0"
+"@jupyterlab/rendermime-interfaces@npm:^3.9.8":
+  version: 3.9.8
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.9.8"
   dependencies:
     "@lumino/coreutils": ^1.11.0 || ^2.1.2
     "@lumino/widgets": ^1.37.2 || ^2.3.1
-  checksum: 462f5d034cd636caf9322245a50045ddaac55e05e056e7c6579e2db55088e724c8054a51a959aa284c44b108a9e0f0053707b50d6d8a9caed5825eeaf715b245
+  checksum: d08bcecdf37a48de5c22bbb5b62a4ebe756408aaa27ae18b3a99d13863e5776c861db69ee1066b2262a1a93ce59f475b549a8d56fe5bc087d4a6ba27afbc168a
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/rendermime@npm:4.1.0"
+"@jupyterlab/rendermime@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/rendermime@npm:4.1.8"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/nbformat": ^4.1.0
-    "@jupyterlab/observables": ^5.1.0
-    "@jupyterlab/rendermime-interfaces": ^3.9.0
-    "@jupyterlab/services": ^7.1.0
-    "@jupyterlab/translation": ^4.1.0
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/nbformat": ^4.1.8
+    "@jupyterlab/observables": ^5.1.8
+    "@jupyterlab/rendermime-interfaces": ^3.9.8
+    "@jupyterlab/services": ^7.1.8
+    "@jupyterlab/translation": ^4.1.8
     "@lumino/coreutils": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     lodash.escape: ^4.0.1
-  checksum: 52323a1d907b29f5b60c237b6e1c3085c667f9fd59e76c6dcab29076a50eb4bd39efe5f6e3e49e3dbabb6dc1f5f7820f09af74f211a76e7e7db6c7c0be8d5715
+  checksum: 3c750598c212e2df43f45c32deba9d4b96dd676781e348771dd7d18c4c23e64e9bf3d25906a68be5368d898a4c81e48ff4215607c46df7934b17dc1ba672a697
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.1.0":
-  version: 7.1.0
-  resolution: "@jupyterlab/services@npm:7.1.0"
+"@jupyterlab/services@npm:^7.1.8":
+  version: 7.1.8
+  resolution: "@jupyterlab/services@npm:7.1.8"
   dependencies:
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/nbformat": ^4.1.0
-    "@jupyterlab/settingregistry": ^4.1.0
-    "@jupyterlab/statedb": ^4.1.0
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/nbformat": ^4.1.8
+    "@jupyterlab/settingregistry": ^4.1.8
+    "@jupyterlab/statedb": ^4.1.8
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     ws: ^8.11.0
-  checksum: 4a4797746c708551a7647c43ecc4dce20dc12ea043bb2bd43ec0c20966825a5e14742258d3bcee9ae832c91030132db895dc9a81bf1596d59c08066c4fecfba5
+  checksum: 56143631829ee1081f6ad2f03343a47d83549d2463f9c4bfddb34e4770c74cf78cbcc5f54aca5338a0d5ce4d28e9b8d8301e6e04b4fb7f66570c49d1ceaf19e5
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/settingregistry@npm:4.1.0"
+"@jupyterlab/settingregistry@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/settingregistry@npm:4.1.8"
   dependencies:
-    "@jupyterlab/nbformat": ^4.1.0
-    "@jupyterlab/statedb": ^4.1.0
+    "@jupyterlab/nbformat": ^4.1.8
+    "@jupyterlab/statedb": ^4.1.8
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@rjsf/utils": ^5.13.4
     ajv: ^8.12.0
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
-  checksum: 1a0c52016806ceda150168cdeae966b15afce454fe24acfd68939f3f380eaf2d4390c40e27c1475877c8e8da6b3f15a952999ebcc9d3838d5306bd24ad5b4b51
+  checksum: 90067142211fdaf6e9a6e0029fe1bc4c9ae05fa8e88e37f912373a0365bc8d507ef44e0bf83deb1e0bd0855a2cf05b0f541db38fafe3bc37d83422df8671e56a
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/statedb@npm:4.1.0"
+"@jupyterlab/statedb@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/statedb@npm:4.1.8"
   dependencies:
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: 693d40ba6ce67b41aae2acbae027a5c637c2bfa51d7085b6faecdb1877a5e3bd43ca70f3670f88f038c49bef80e0e09899b05d330dd9010b1d578ca73b13ea17
+  checksum: 28983e98affec8b8d6bb8e0cbacfe2c74d1ae48af8e69fddc7f457dcd87210adf5e39dafd21bcad24cfe572f45758c7531cd8d991e9eda894e63392b544bf09d
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/statusbar@npm:4.1.0"
+"@jupyterlab/statusbar@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/statusbar@npm:4.1.8"
   dependencies:
-    "@jupyterlab/ui-components": ^4.1.0
+    "@jupyterlab/ui-components": ^4.1.8
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 309d3cb98c924c23dfef2ad91862dfa56ea133d8ae08aa7bc743c4000f15584841b39712bc8829eb09d7382d5c9e0e7b3e85c3ae1165c01597ade96702bcc055
+  checksum: eb3094b9511334a82b92686ad7010763fc8c101a9631ee558462cc71d6ca3e7ad485a927e777da1f2c1aba8398c5c2d1ec65c48daae69317267944255197dbe7
   languageName: node
   linkType: hard
 
-"@jupyterlab/testing@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/testing@npm:4.1.0"
+"@jupyterlab/testing@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/testing@npm:4.1.8"
   dependencies:
     "@babel/core": ^7.10.2
     "@babel/preset-env": ^7.10.2
-    "@jupyterlab/coreutils": ^6.1.0
+    "@jupyterlab/coreutils": ^6.1.8
     "@lumino/coreutils": ^2.1.2
     "@lumino/signaling": ^2.1.2
     child_process: ~1.0.2
     deepmerge: ^4.2.2
     fs-extra: ^10.1.0
     identity-obj-proxy: ^3.0.0
     jest: ^29.2.0
     jest-environment-jsdom: ^29.3.0
     jest-junit: ^15.0.0
     node-fetch: ^2.6.0
     simulate-event: ~1.4.0
     ts-jest: ^29.1.0
   peerDependencies:
     typescript: ">=4.3"
-  checksum: ea44aa152e005302b10725401c0116ce250498168bd829553feec39564bde03d1c92c357dbe6ca55396e5bd66b82c77da2de0bcbdb8acb92371d37b7fe3c998b
+  checksum: 8bb3e0e3ee9722fc36993fbba5252627ff9080045d1ddecc196a5df13e84b64cb1d65ded0cf567bcf275207c014a812cca4910be88f2f35fc52d91c45123d5be
   languageName: node
   linkType: hard
 
 "@jupyterlab/testutils@npm:^4.0.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/testutils@npm:4.1.0"
+  version: 4.1.8
+  resolution: "@jupyterlab/testutils@npm:4.1.8"
   dependencies:
-    "@jupyterlab/application": ^4.1.0
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/notebook": ^4.1.0
-    "@jupyterlab/rendermime": ^4.1.0
-    "@jupyterlab/testing": ^4.1.0
-  checksum: 0ed195b52cec7639358c8694ed99b8106aeb58d2b9afa51da3c564f8d4530c089a7d72d8fb503ca7de40ca0aec26e28b7d6fc551fae235027111b9b66eba80eb
+    "@jupyterlab/application": ^4.1.8
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/notebook": ^4.1.8
+    "@jupyterlab/rendermime": ^4.1.8
+    "@jupyterlab/testing": ^4.1.8
+  checksum: efabbdd60565a76cf7c17ef05ae73956f5955bbe943430c64ff9985677cadbfdc35eb79f20ea5e4ae5227fdcb397e8920a71e8b0f9b60a5c31dc6a9a4815fa11
   languageName: node
   linkType: hard
 
-"@jupyterlab/toc@npm:^6.1.0":
-  version: 6.1.0
-  resolution: "@jupyterlab/toc@npm:6.1.0"
-  dependencies:
-    "@jupyterlab/apputils": ^4.2.0
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/docregistry": ^4.1.0
-    "@jupyterlab/observables": ^5.1.0
-    "@jupyterlab/rendermime": ^4.1.0
-    "@jupyterlab/rendermime-interfaces": ^3.9.0
-    "@jupyterlab/translation": ^4.1.0
-    "@jupyterlab/ui-components": ^4.1.0
+"@jupyterlab/toc@npm:^6.1.8":
+  version: 6.1.8
+  resolution: "@jupyterlab/toc@npm:6.1.8"
+  dependencies:
+    "@jupyterlab/apputils": ^4.2.8
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/docregistry": ^4.1.8
+    "@jupyterlab/observables": ^5.1.8
+    "@jupyterlab/rendermime": ^4.1.8
+    "@jupyterlab/rendermime-interfaces": ^3.9.8
+    "@jupyterlab/translation": ^4.1.8
+    "@jupyterlab/ui-components": ^4.1.8
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 051f960311e0f9dfba2668411c32480376d04cd05a023e69d25818ca6b7ca9fdc16f5c3ffc966a519cb2653a26e03cb14f2c267a2e40cffd4d06c31c7db138d8
+  checksum: 6dadf19c32fadeccc19df6ba31287c929a7a09ac41ecaf53fbc88471d4c62a16193555c3fb391ecc4e495c9f6cdde7d0519c77ed0b69fbc90da9e5b16bb924d3
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/translation@npm:4.1.0"
+"@jupyterlab/translation@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/translation@npm:4.1.8"
   dependencies:
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/rendermime-interfaces": ^3.9.0
-    "@jupyterlab/services": ^7.1.0
-    "@jupyterlab/statedb": ^4.1.0
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/rendermime-interfaces": ^3.9.8
+    "@jupyterlab/services": ^7.1.8
+    "@jupyterlab/statedb": ^4.1.8
     "@lumino/coreutils": ^2.1.2
-  checksum: 88b7422697c1795dfcb85870cb8642cd10be6ae27a61dd1ca9f1304f06460f859202bfb6733cb744e2b4c448e8bfbf7a4793c6626cb4a18a59c80999cf1c5050
+  checksum: 7de872e52ffa0d2e4579c26b906ae7f98fcab6767ff85a4ce157f70be26d9edcf3410e94931ea9c8c1a1c48f4fc5f5e410b396761164dc8314ec1157314bcb9e
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "@jupyterlab/ui-components@npm:4.1.0"
+"@jupyterlab/ui-components@npm:^4.1.8":
+  version: 4.1.8
+  resolution: "@jupyterlab/ui-components@npm:4.1.8"
   dependencies:
     "@jupyter/react-components": ^0.15.2
     "@jupyter/web-components": ^0.15.2
-    "@jupyterlab/coreutils": ^6.1.0
-    "@jupyterlab/observables": ^5.1.0
-    "@jupyterlab/rendermime-interfaces": ^3.9.0
-    "@jupyterlab/translation": ^4.1.0
+    "@jupyterlab/coreutils": ^6.1.8
+    "@jupyterlab/observables": ^5.1.8
+    "@jupyterlab/rendermime-interfaces": ^3.9.8
+    "@jupyterlab/translation": ^4.1.8
     "@lumino/algorithm": ^2.0.1
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
@@ -2687,15 +2694,15 @@
     "@rjsf/core": ^5.13.4
     "@rjsf/utils": ^5.13.4
     react: ^18.2.0
     react-dom: ^18.2.0
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
-  checksum: 53f8eb432d7ff8890ec748c3b43fbcb67fe6cd218b771c4c334e1ddd80a13b570071f171eca4c15feebc4715427e422f833d7b8e2084bcd2605979a444e1536d
+  checksum: 6a95597b8c71cd31b3f7a39cc61dc094fc6fede5b0b6bac61ff9df0a5757542d419e653f3a2527a15cb0dc9e7b7fcd2568101e9063878ce260f6adb486787e69
   languageName: node
   linkType: hard
 
 "@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2, @lezer/common@npm:^1.1.0, @lezer/common@npm:^1.2.0, @lezer/common@npm:^1.2.1":
   version: 1.2.1
   resolution: "@lezer/common@npm:1.2.1"
   checksum: 0bd092e293a509ce334f4aaf9a4d4a25528f743cd9d7e7948c697e34ac703b805b288b62ad01563488fb206fc34ff05084f7fc5d864be775924b3d0d53ea5dd2
@@ -2710,75 +2717,75 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: a319cd46fd32affc07c9432e9b2b9954becf7766be0361176c525d03474bb794cc051aad9932f48c9df33833eee1d6bfdccab12e571f2b137b4ca765c60c75de
   languageName: node
   linkType: hard
 
 "@lezer/css@npm:^1.0.0, @lezer/css@npm:^1.1.0":
-  version: 1.1.7
-  resolution: "@lezer/css@npm:1.1.7"
+  version: 1.1.8
+  resolution: "@lezer/css@npm:1.1.8"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 7760d294fd0b1ac6db319c4990517c1ed9027d6757de537553624238056df6e1ef1b6a571a023a4bce3d7a2b891036d9f85f76f2109f503bea94837f90c64bc2
+  checksum: 1f5968360dbac7ba27f0c2a194143769f7b01824715274dd8507dacf13cc790bb8c48ce95de355e9c58be93bb3e271bf98b9fc51213f79e4ce918e7c7ebbef04
   languageName: node
   linkType: hard
 
 "@lezer/generator@npm:^1.2.2":
-  version: 1.6.0
-  resolution: "@lezer/generator@npm:1.6.0"
+  version: 1.7.0
+  resolution: "@lezer/generator@npm:1.7.0"
   dependencies:
     "@lezer/common": ^1.1.0
     "@lezer/lr": ^1.3.0
   bin:
     lezer-generator: src/lezer-generator.cjs
-  checksum: dfbf19d0533922272ac00c4b7884e1df88e2a35dd758e4544ceb5d784aa38d5751add03ca87f35d14cc39416e0dbc06ccaf2a211a6ae982e00daaaffe9c9320c
+  checksum: 69f4c6625446cb65adaa509480ec67502f27651707a8e45e99373e682d7f66f8842205669f174bcb138eade72c64ded0b54d6de6aa5af995ac1f1e805ef021fd
   languageName: node
   linkType: hard
 
 "@lezer/highlight@npm:^1.0.0, @lezer/highlight@npm:^1.1.3, @lezer/highlight@npm:^1.1.4":
   version: 1.2.0
   resolution: "@lezer/highlight@npm:1.2.0"
   dependencies:
     "@lezer/common": ^1.0.0
   checksum: 5b9dfe741f95db13f6124cb9556a43011cb8041ecf490be98d44a86b04d926a66e912bcd3a766f6a3d79e064410f1a2f60ab240b50b645a12c56987bf4870086
   languageName: node
   linkType: hard
 
 "@lezer/html@npm:^1.3.0":
-  version: 1.3.8
-  resolution: "@lezer/html@npm:1.3.8"
+  version: 1.3.9
+  resolution: "@lezer/html@npm:1.3.9"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 06bce804487435ea6ccb39595176bb65d68691f082b0b68fb7d22d90d4de9798a8202f16e9aefe22865db15257a37f6fca93275d660715eea98f7578579e7135
+  checksum: 40d89b0af4379768ce7d3e7162988e9ec73b42984e333e877c7451f7e2c10131e39e4b50150bc334093cbd84a3b34f9fc1a6ac62cbba51f503a495ad243e880b
   languageName: node
   linkType: hard
 
 "@lezer/java@npm:^1.0.0":
-  version: 1.1.1
-  resolution: "@lezer/java@npm:1.1.1"
+  version: 1.1.2
+  resolution: "@lezer/java@npm:1.1.2"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 8a071aca6b5e1ed1d22bffed22bbd29f21b102b7337a7ea5c956eb259e6ff20eee2d6e85b7dadff69859cb6615d6b1a3f0ba109673e87ce5a1f6cabdeee626fd
+  checksum: 752e8c9b99cccf022669a702016e0c3a793d8326e043b1d053159f5de4d222cd188e8e31e1427cbe6a8ed8e53de3977ab551c64cbd5a76a12eb3a1da5e18b6a5
   languageName: node
   linkType: hard
 
 "@lezer/javascript@npm:^1.0.0":
-  version: 1.4.13
-  resolution: "@lezer/javascript@npm:1.4.13"
+  version: 1.4.15
+  resolution: "@lezer/javascript@npm:1.4.15"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.1.3
     "@lezer/lr": ^1.3.0
-  checksum: a5e4607fec7671dff66d1f3bfee5a5da7395982f1867e17ac4d8f2d8f223451fb18516ef2699340b148af112176a07e1fcba9e63c5f8397c12895dd0509113d6
+  checksum: e0322ec70231a1beb6652f0883d62371297f37783a774ad011a3c7d4acaf066f4bcd6c0b83b34cef0893766ae730ab29efee7a11d67d66e8c5f8d4dea3c46172
   languageName: node
   linkType: hard
 
 "@lezer/json@npm:^1.0.0":
   version: 1.0.2
   resolution: "@lezer/json@npm:1.0.2"
   dependencies:
@@ -2795,20 +2802,20 @@
   dependencies:
     "@lezer/common": ^1.0.0
   checksum: 4c8517017e9803415c6c5cb8230d8764107eafd7d0b847676cd1023abb863a4b268d0d01c7ce3cf1702c4749527c68f0a26b07c329cb7b68c36ed88362d7b193
   languageName: node
   linkType: hard
 
 "@lezer/markdown@npm:^1.0.0, @lezer/markdown@npm:^1.0.2":
-  version: 1.2.0
-  resolution: "@lezer/markdown@npm:1.2.0"
+  version: 1.3.0
+  resolution: "@lezer/markdown@npm:1.3.0"
   dependencies:
     "@lezer/common": ^1.0.0
     "@lezer/highlight": ^1.0.0
-  checksum: e6355272ad98c97b339dd42d8d9b78fa4f48fdcc5c9c408720936cacb7d2bcd47b0cedf8e0997ef93539c2b03a65326fc59372e54f0b24acd98630e06869a350
+  checksum: 13eb2720e4cb84278349bad8af116f748813094f99fad02680010c3a8c5985e0358c344487990f87a31ef0d6c1a2be582301f914c0e4a6e9cfa22647b6cd6545
   languageName: node
   linkType: hard
 
 "@lezer/php@npm:^1.0.0":
   version: 1.0.2
   resolution: "@lezer/php@npm:1.0.2"
   dependencies:
@@ -2816,21 +2823,21 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.1.0
   checksum: c85ef18571d37826b687dd141a0fe110f5814adaf9d1a391e7e482020d7f81df189ca89ec0dd141c1433d48eff4c6e53648b46f008dea8ad2dc574f35f1d4d79
   languageName: node
   linkType: hard
 
 "@lezer/python@npm:^1.1.4":
-  version: 1.1.11
-  resolution: "@lezer/python@npm:1.1.11"
+  version: 1.1.13
+  resolution: "@lezer/python@npm:1.1.13"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: ed0e58317716967644f57bf29eb902c0c205b909bc035c0960520222a79bd6525468c8adfb7d824787a8a29ec7a1c7d2da5fd59f912cdeff2830c71958b9576d
+  checksum: 43465f3289063e16caac9a109f61b8f810dd6a0e1043874df1b4d0f1cee5fba39cfd8c78fa2e507c0aa8f50cee8c48fe36df549ac1f959dae8d51c06e8ec0d0b
   languageName: node
   linkType: hard
 
 "@lezer/rust@npm:^1.0.0":
   version: 1.0.2
   resolution: "@lezer/rust@npm:1.0.2"
   dependencies:
@@ -2838,63 +2845,63 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: fc5e97852b42beeb44a0ebe316dc64e3cc49ff481c22e3e67d6003fc4a5c257fcd94959cfcc76cd154fa172db9b3b4b28de5c09f10550d6e5f14869ddc274e5b
   languageName: node
   linkType: hard
 
 "@lezer/xml@npm:^1.0.0":
-  version: 1.0.4
-  resolution: "@lezer/xml@npm:1.0.4"
+  version: 1.0.5
+  resolution: "@lezer/xml@npm:1.0.5"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 68a82085bff6c1525f4ef03cd9f9dac0132b3e03fe574e0289700dd4475056e40e8744cde15cf5ad6d3760d0d584ff85ce707e26a7c938d0c5fe2e325c1c336e
+  checksum: a0a077b9e455b03593b93a7fdff2a4eab2cb7b230c8e1b878a8bebe80184632b9cc75ca018f1f9e2acb3a26e1386f4777385ab6e87aea70ccf479cde5ca268ee
   languageName: node
   linkType: hard
 
 "@lumino/algorithm@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/algorithm@npm:2.0.1"
   checksum: cbf7fcf6ee6b785ea502cdfddc53d61f9d353dcb9659343511d5cd4b4030be2ff2ca4c08daec42f84417ab0318a3d9972a17319fa5231693e109ab112dcf8000
   languageName: node
   linkType: hard
 
 "@lumino/application@npm:^2.3.0":
-  version: 2.3.0
-  resolution: "@lumino/application@npm:2.3.0"
+  version: 2.3.1
+  resolution: "@lumino/application@npm:2.3.1"
   dependencies:
-    "@lumino/commands": ^2.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
-    "@lumino/widgets": ^2.3.1
-  checksum: 9d1eb5bc972ed158bf219604a53bbac1262059bc5b0123d3e041974486b9cbb8288abeeec916f3b62f62d7c32e716cccf8b73e4832ae927e4f9dd4e4b0cd37ed
+    "@lumino/widgets": ^2.3.2
+  checksum: c112789d99baf62e5c2cee98834bc3efb5027bbca1aac81f10ea8855c0cd2538ec0a7c56c3f5dd42dce244e6892ef5bf8ef356f97e1cd4c161b99eb2068c195c
   languageName: node
   linkType: hard
 
 "@lumino/collections@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/collections@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: 8a29b7973a388a33c5beda0819dcd2dc2aad51a8406dcfd4581b055a9f77a39dc5800f7a8b4ae3c0bb97ae7b56a7a869e2560ffb7a920a28e93b477ba05907d6
   languageName: node
   linkType: hard
 
-"@lumino/commands@npm:^2.2.0":
-  version: 2.2.0
-  resolution: "@lumino/commands@npm:2.2.0"
+"@lumino/commands@npm:^2.2.0, @lumino/commands@npm:^2.3.0":
+  version: 2.3.0
+  resolution: "@lumino/commands@npm:2.3.0"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/keyboard": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-  checksum: 093e9715491e5cef24bc80665d64841417b400f2fa595f9b60832a3b6340c405c94a6aa276911944a2c46d79a6229f3cc087b73f50852bba25ece805abd0fae9
+  checksum: a9b83bbfcc0421ff501e818dd234c65db438a8abb450628db0dea9ee05e8077d10b2275e7e2289f6df9c20dc26d2af458b1db88ccf43ec69f185eb207dbad419
   languageName: node
   linkType: hard
 
 "@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.1.2, @lumino/coreutils@npm:^2.1.2":
   version: 2.1.2
   resolution: "@lumino/coreutils@npm:2.1.2"
   checksum: 7865317ac0676b448d108eb57ab5d8b2a17c101995c0f7a7106662d9fe6c859570104525f83ee3cda12ae2e326803372206d6f4c1f415a5b59e4158a7b81066f
@@ -2977,68 +2984,68 @@
   resolution: "@lumino/virtualdom@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: cf59b6f15b430e13e9e657b7a0619b9056cd9ea7b2a87f407391d071c501b77403c302b6a66dca510382045e75b2e3fe551630bb391f1c6b33678057d4bec164
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^1.37.2 || ^2.3.1, @lumino/widgets@npm:^2.3.1":
-  version: 2.3.1
-  resolution: "@lumino/widgets@npm:2.3.1"
+"@lumino/widgets@npm:^1.37.2 || ^2.3.1, @lumino/widgets@npm:^2.3.1, @lumino/widgets@npm:^2.3.2":
+  version: 2.3.2
+  resolution: "@lumino/widgets@npm:2.3.2"
   dependencies:
     "@lumino/algorithm": ^2.0.1
-    "@lumino/commands": ^2.2.0
+    "@lumino/commands": ^2.3.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/keyboard": ^2.0.1
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
-  checksum: ba7b8f8839c1cd2a41dbda13281094eb6981a270cccf4f25a0cf83686dcc526a2d8044a20204317630bb7dd4a04d65361408c7623a921549c781afca84b91c67
+  checksum: 954fe066b0826cf00c019731bb3f70e635c63be4a0ce27f7573dbe6bd59e2154f511594b50e8f58f44877cf514084128c1e894ecbbbfd6e20d937e5cfb69ca8b
   languageName: node
   linkType: hard
 
 "@microsoft/fast-colors@npm:^5.3.1":
   version: 5.3.1
   resolution: "@microsoft/fast-colors@npm:5.3.1"
   checksum: ff87f402faadb4b5aeee3d27762566c11807f927cd4012b8bbc7f073ca68de0e2197f95330ff5dfd7038f4b4f0e2f51b11feb64c5d570f5c598d37850a5daf60
   languageName: node
   linkType: hard
 
-"@microsoft/fast-element@npm:^1.12.0":
-  version: 1.12.0
-  resolution: "@microsoft/fast-element@npm:1.12.0"
-  checksum: bbff4e9c83106d1d74f3eeedc87bf84832429e78fee59c6a4ae8164ee4f42667503f586896bea72341b4d2c76c244a3cb0d4fd0d5d3732755f00357714dd609e
+"@microsoft/fast-element@npm:^1.12.0, @microsoft/fast-element@npm:^1.13.0":
+  version: 1.13.0
+  resolution: "@microsoft/fast-element@npm:1.13.0"
+  checksum: 1cb7b4cfb7531116a3542d3f59bf1dd35106194f5764205403590250aaff744de79e35a5a1f36b4941c4eda9edc088148d4d629fb80be15fdf25f6be01770f3a
   languageName: node
   linkType: hard
 
-"@microsoft/fast-foundation@npm:^2.49.4, @microsoft/fast-foundation@npm:^2.49.5":
-  version: 2.49.5
-  resolution: "@microsoft/fast-foundation@npm:2.49.5"
+"@microsoft/fast-foundation@npm:^2.49.4, @microsoft/fast-foundation@npm:^2.49.6":
+  version: 2.49.6
+  resolution: "@microsoft/fast-foundation@npm:2.49.6"
   dependencies:
-    "@microsoft/fast-element": ^1.12.0
+    "@microsoft/fast-element": ^1.13.0
     "@microsoft/fast-web-utilities": ^5.4.1
     tabbable: ^5.2.0
     tslib: ^1.13.0
-  checksum: 8a4729e8193ee93f780dc88fac26561b42f2636e3f0a8e89bb1dfe256f50a01a21ed1d8e4d31ce40678807dc833e25f31ba735cb5d3c247b65219aeb2560c82c
+  checksum: 15fdf9dd0b910a72a9cff140f765d522304df11f8a78d5a97a815e2bbae25027c2b336e94f89ca31e650d6aabe17b590b7453acc0d2cb7340c219eb76350a942
   languageName: node
   linkType: hard
 
 "@microsoft/fast-react-wrapper@npm:^0.3.22":
-  version: 0.3.23
-  resolution: "@microsoft/fast-react-wrapper@npm:0.3.23"
+  version: 0.3.24
+  resolution: "@microsoft/fast-react-wrapper@npm:0.3.24"
   dependencies:
-    "@microsoft/fast-element": ^1.12.0
-    "@microsoft/fast-foundation": ^2.49.5
+    "@microsoft/fast-element": ^1.13.0
+    "@microsoft/fast-foundation": ^2.49.6
   peerDependencies:
     react: ">=16.9.0"
-  checksum: 45885e1868916d2aa9059e99c341c97da434331d9340a57128d4218081df68b5e1107031c608db9a550d6d1c3b010d516ed4f8dc5a8a2470058da6750dcd204a
+  checksum: 1d7a87509c22872bafc9b5c64f66659e52ba0cfdff484d7204125e503dafdea143f5e1bd2a643e2f3fbba6cc7567d916393369433f19dab9f0adcbe7a88b7d98
   languageName: node
   linkType: hard
 
 "@microsoft/fast-web-utilities@npm:^5.4.1":
   version: 5.4.1
   resolution: "@microsoft/fast-web-utilities@npm:5.4.1"
   dependencies:
@@ -3071,23 +3078,23 @@
     "@nodelib/fs.scandir": 2.1.5
     fastq: ^1.6.0
   checksum: 190c643f156d8f8f277bf2a6078af1ffde1fd43f498f187c2db24d35b4b4b5785c02c7dc52e356497b9a1b65b13edc996de08de0b961c32844364da02986dc53
   languageName: node
   linkType: hard
 
 "@npmcli/agent@npm:^2.0.0":
-  version: 2.2.1
-  resolution: "@npmcli/agent@npm:2.2.1"
+  version: 2.2.2
+  resolution: "@npmcli/agent@npm:2.2.2"
   dependencies:
     agent-base: ^7.1.0
     http-proxy-agent: ^7.0.0
     https-proxy-agent: ^7.0.1
     lru-cache: ^10.0.1
-    socks-proxy-agent: ^8.0.1
-  checksum: c69aca42dbba393f517bc5777ee872d38dc98ea0e5e93c1f6d62b82b8fecdc177a57ea045f07dda1a770c592384b2dd92a5e79e21e2a7cf51c9159466a8f9c9b
+    socks-proxy-agent: ^8.0.3
+  checksum: 67de7b88cc627a79743c88bab35e023e23daf13831a8aa4e15f998b92f5507b644d8ffc3788afc8e64423c612e0785a6a92b74782ce368f49a6746084b50d874
   languageName: node
   linkType: hard
 
 "@npmcli/fs@npm:^3.1.0":
   version: 3.1.0
   resolution: "@npmcli/fs@npm:3.1.0"
   dependencies:
@@ -3100,41 +3107,41 @@
   version: 0.11.0
   resolution: "@pkgjs/parseargs@npm:0.11.0"
   checksum: 6ad6a00fc4f2f2cfc6bff76fb1d88b8ee20bc0601e18ebb01b6d4be583733a860239a521a7fbca73b612e66705078809483549d2b18f370eb346c5155c8e4a0f
   languageName: node
   linkType: hard
 
 "@rjsf/core@npm:^5.13.4":
-  version: 5.17.0
-  resolution: "@rjsf/core@npm:5.17.0"
+  version: 5.18.3
+  resolution: "@rjsf/core@npm:5.18.3"
   dependencies:
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     markdown-to-jsx: ^7.4.1
     nanoid: ^3.3.7
     prop-types: ^15.8.1
   peerDependencies:
-    "@rjsf/utils": ^5.16.x
+    "@rjsf/utils": ^5.18.x
     react: ^16.14.0 || >=17
-  checksum: adfcbd1d44cef5f9e5de2873096085abd03b146dcef2c9c226060341ce2c935b5399e4ad5f00ad5091394224f5859bd6ac9bac533537dc5c8e2edb16b52b67cf
+  checksum: 370586a38e6557367281cd3e6292abf4391a24ed3d7c19b02478a45ca5aeb337363f54d841a7077b1403a24014bb1969d568976f12220b3ccd1a076ed4875397
   languageName: node
   linkType: hard
 
 "@rjsf/utils@npm:^5.13.4":
-  version: 5.17.0
-  resolution: "@rjsf/utils@npm:5.17.0"
+  version: 5.18.3
+  resolution: "@rjsf/utils@npm:5.18.3"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: 01d0001f83083764a8552e009aa7df084621df9d1fc6ccdfad9d534513084421b1ad7494cab77b9b8205d680fd915f612d87800e20ab242e7066f33184c73d4f
+  checksum: 36f6574836e8ccad27b8215f940cb86b1a02939d325e0223a8d8e70b9ae65245e6649dd4835a40e628153f26d961a5cfbdd6c0bdd7b70a80f7cb1911357f78ff
   languageName: node
   linkType: hard
 
 "@sinclair/typebox@npm:^0.27.8":
   version: 0.27.8
   resolution: "@sinclair/typebox@npm:0.27.8"
   checksum: 00bd7362a3439021aa1ea51b0e0d0a0e8ca1351a3d54c606b115fdcc49b51b16db6e5f43b4fe7a28c38688523e22a94d49dd31168868b655f0d4d50f032d07a1
@@ -3214,20 +3221,20 @@
     "@types/eslint": "*"
     "@types/estree": "*"
   checksum: e2889a124aaab0b89af1bab5959847c5bec09809209255de0e63b9f54c629a94781daa04adb66bffcdd742f5e25a17614fb933965093c0eea64aacda4309380e
   languageName: node
   linkType: hard
 
 "@types/eslint@npm:*":
-  version: 8.56.2
-  resolution: "@types/eslint@npm:8.56.2"
+  version: 8.56.10
+  resolution: "@types/eslint@npm:8.56.10"
   dependencies:
     "@types/estree": "*"
     "@types/json-schema": "*"
-  checksum: 38e054971596f5c0413f66a62dc26b10e0a21ac46ceacb06fbf8cfb838d20820787209b17218b3916e4c23d990ff77cfdb482d655cac0e0d2b837d430fcc5db8
+  checksum: fb7137dd263ce1130b42d14452bdd0266ef81f52cb55ba1a5e9750e65da1f0596dc598c88bffc7e415458b6cb611a876dcc132bcf40ea48701c6d05b40c57be5
   languageName: node
   linkType: hard
 
 "@types/estree@npm:*, @types/estree@npm:^1.0.5":
   version: 1.0.5
   resolution: "@types/estree@npm:1.0.5"
   checksum: dd8b5bed28e6213b7acd0fb665a84e693554d850b0df423ac8076cc3ad5823a6bc26b0251d080bdc545af83179ede51dd3f6fa78cad2c46ed1f29624ddf3e41a
@@ -3300,19 +3307,19 @@
   version: 1.2.5
   resolution: "@types/minimist@npm:1.2.5"
   checksum: 477047b606005058ab0263c4f58097136268007f320003c348794f74adedc3166ffc47c80ec3e94687787f2ab7f4e72c468223946e79892cf0fd9e25e9970a90
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 20.11.16
-  resolution: "@types/node@npm:20.11.16"
+  version: 20.12.7
+  resolution: "@types/node@npm:20.12.7"
   dependencies:
     undici-types: ~5.26.4
-  checksum: 51f0831c1219bf4698e7430aeb9892237bd851deeb25ce23c5bb0ceefcc77c3b114e48f4e98d9fc26def5a87ba9d8079f0281dd37bee691140a93f133812c152
+  checksum: 7cc979f7e2ca9a339ec71318c3901b9978555257929ef3666987f3e447123bc6dc92afcc89f6347e09e07d602fde7d51bcddea626c23aa2bb74aeaacfd1e1686
   languageName: node
   linkType: hard
 
 "@types/normalize-package-data@npm:^2.4.0":
   version: 2.4.4
   resolution: "@types/normalize-package-data@npm:2.4.4"
   checksum: 65dff72b543997b7be8b0265eca7ace0e34b75c3e5fee31de11179d08fa7124a7a5587265d53d0409532ecb7f7fba662c2012807963e1f9b059653ec2c83ee05
@@ -3323,42 +3330,34 @@
   version: 4.0.2
   resolution: "@types/parse-json@npm:4.0.2"
   checksum: 5bf62eec37c332ad10059252fc0dab7e7da730764869c980b0714777ad3d065e490627be9f40fc52f238ffa3ac4199b19de4127196910576c2fe34dd47c7a470
   languageName: node
   linkType: hard
 
 "@types/prop-types@npm:*":
-  version: 15.7.11
-  resolution: "@types/prop-types@npm:15.7.11"
-  checksum: 7519ff11d06fbf6b275029fe03fff9ec377b4cb6e864cac34d87d7146c7f5a7560fd164bdc1d2dbe00b60c43713631251af1fd3d34d46c69cd354602bc0c7c54
+  version: 15.7.12
+  resolution: "@types/prop-types@npm:15.7.12"
+  checksum: ac16cc3d0a84431ffa5cfdf89579ad1e2269549f32ce0c769321fdd078f84db4fbe1b461ed5a1a496caf09e637c0e367d600c541435716a55b1d9713f5035dfe
   languageName: node
   linkType: hard
 
 "@types/react@npm:^18.0.26":
-  version: 18.2.55
-  resolution: "@types/react@npm:18.2.55"
+  version: 18.3.1
+  resolution: "@types/react@npm:18.3.1"
   dependencies:
     "@types/prop-types": "*"
-    "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: a8eb4fa77f73831b9112d4f11a7006217dc0740361649b9b0da3fd441d151a9cd415d5d68b91c0af4e430e063424d301c77489e5edaddc9f711c4e46cf9818a5
-  languageName: node
-  linkType: hard
-
-"@types/scheduler@npm:*":
-  version: 0.16.8
-  resolution: "@types/scheduler@npm:0.16.8"
-  checksum: 6c091b096daa490093bf30dd7947cd28e5b2cd612ec93448432b33f724b162587fed9309a0acc104d97b69b1d49a0f3fc755a62282054d62975d53d7fd13472d
+  checksum: 9224ef319a0c2b7f66e7e7f06012aa5eb638a6c76c9742843eab1a5d243f2bed5ff829ddbb41efd60d33a266420528adfcb84cb93f238b00e905f98c3a355768
   languageName: node
   linkType: hard
 
 "@types/semver@npm:^7.3.12":
-  version: 7.5.6
-  resolution: "@types/semver@npm:7.5.6"
-  checksum: 563a0120ec0efcc326567db2ed920d5d98346f3638b6324ea6b50222b96f02a8add3c51a916b6897b51523aad8ac227d21d3dcf8913559f1bfc6c15b14d23037
+  version: 7.5.8
+  resolution: "@types/semver@npm:7.5.8"
+  checksum: ea6f5276f5b84c55921785a3a27a3cd37afee0111dfe2bcb3e03c31819c197c782598f17f0b150a69d453c9584cd14c4c4d7b9a55d2c5e6cacd4d66fdb3b3663
   languageName: node
   linkType: hard
 
 "@types/source-list-map@npm:*":
   version: 0.1.6
   resolution: "@types/source-list-map@npm:0.1.6"
   checksum: 9cd294c121f1562062de5d241fe4d10780b1131b01c57434845fe50968e9dcf67ede444591c2b1ad6d3f9b6bc646ac02cc8f51a3577c795f9c64cf4573dcc6b1
@@ -3530,21 +3529,21 @@
 "@ungap/structured-clone@npm:^1.2.0":
   version: 1.2.0
   resolution: "@ungap/structured-clone@npm:1.2.0"
   checksum: 4f656b7b4672f2ce6e272f2427d8b0824ed11546a601d8d5412b9d7704e83db38a8d9f402ecdf2b9063fc164af842ad0ec4a55819f621ed7e7ea4d1efcc74524
   languageName: node
   linkType: hard
 
-"@webassemblyjs/ast@npm:1.11.6, @webassemblyjs/ast@npm:^1.11.5":
-  version: 1.11.6
-  resolution: "@webassemblyjs/ast@npm:1.11.6"
+"@webassemblyjs/ast@npm:1.12.1, @webassemblyjs/ast@npm:^1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/ast@npm:1.12.1"
   dependencies:
     "@webassemblyjs/helper-numbers": 1.11.6
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
-  checksum: 38ef1b526ca47c210f30975b06df2faf1a8170b1636ce239fc5738fc231ce28389dd61ecedd1bacfc03cbe95b16d1af848c805652080cb60982836eb4ed2c6cf
+  checksum: 31bcc64147236bd7b1b6d29d1f419c1f5845c785e1e42dc9e3f8ca2e05a029e9393a271b84f3a5bff2a32d35f51ff59e2181a6e5f953fe88576acd6750506202
   languageName: node
   linkType: hard
 
 "@webassemblyjs/floating-point-hex-parser@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/floating-point-hex-parser@npm:1.11.6"
   checksum: 29b08758841fd8b299c7152eda36b9eb4921e9c584eb4594437b5cd90ed6b920523606eae7316175f89c20628da14326801090167cc7fbffc77af448ac84b7e2
@@ -3554,18 +3553,18 @@
 "@webassemblyjs/helper-api-error@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-api-error@npm:1.11.6"
   checksum: e8563df85161096343008f9161adb138a6e8f3c2cc338d6a36011aa55eabb32f2fd138ffe63bc278d009ada001cc41d263dadd1c0be01be6c2ed99076103689f
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-buffer@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/helper-buffer@npm:1.11.6"
-  checksum: b14d0573bf680d22b2522e8a341ec451fddd645d1f9c6bd9012ccb7e587a2973b86ab7b89fe91e1c79939ba96095f503af04369a3b356c8023c13a5893221644
+"@webassemblyjs/helper-buffer@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/helper-buffer@npm:1.12.1"
+  checksum: c3ffb723024130308db608e86e2bdccd4868bbb62dffb0a9a1530606496f79c87f8565bd8e02805ce64912b71f1a70ee5fb00307258b0c082c3abf961d097eca
   languageName: node
   linkType: hard
 
 "@webassemblyjs/helper-numbers@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-numbers@npm:1.11.6"
   dependencies:
@@ -3579,23 +3578,23 @@
 "@webassemblyjs/helper-wasm-bytecode@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-wasm-bytecode@npm:1.11.6"
   checksum: 3535ef4f1fba38de3475e383b3980f4bbf3de72bbb631c2b6584c7df45be4eccd62c6ff48b5edd3f1bcff275cfd605a37679ec199fc91fd0a7705d7f1e3972dc
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-wasm-section@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/helper-wasm-section@npm:1.11.6"
+"@webassemblyjs/helper-wasm-section@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/helper-wasm-section@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
-    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
+    "@webassemblyjs/helper-buffer": 1.12.1
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
-    "@webassemblyjs/wasm-gen": 1.11.6
-  checksum: b2cf751bf4552b5b9999d27bbb7692d0aca75260140195cb58ea6374d7b9c2dc69b61e10b211a0e773f66209c3ddd612137ed66097e3684d7816f854997682e9
+    "@webassemblyjs/wasm-gen": 1.12.1
+  checksum: c19810cdd2c90ff574139b6d8c0dda254d42d168a9e5b3d353d1bc085f1d7164ccd1b3c05592a45a939c47f7e403dc8d03572bb686642f06a3d02932f6f0bc8f
   languageName: node
   linkType: hard
 
 "@webassemblyjs/ieee754@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/ieee754@npm:1.11.6"
   dependencies:
@@ -3616,76 +3615,76 @@
 "@webassemblyjs/utf8@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/utf8@npm:1.11.6"
   checksum: 807fe5b5ce10c390cfdd93e0fb92abda8aebabb5199980681e7c3743ee3306a75729bcd1e56a3903980e96c885ee53ef901fcbaac8efdfa480f9c0dae1d08713
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-edit@npm:^1.11.5":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-edit@npm:1.11.6"
+"@webassemblyjs/wasm-edit@npm:^1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-edit@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
-    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
+    "@webassemblyjs/helper-buffer": 1.12.1
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
-    "@webassemblyjs/helper-wasm-section": 1.11.6
-    "@webassemblyjs/wasm-gen": 1.11.6
-    "@webassemblyjs/wasm-opt": 1.11.6
-    "@webassemblyjs/wasm-parser": 1.11.6
-    "@webassemblyjs/wast-printer": 1.11.6
-  checksum: 29ce75870496d6fad864d815ebb072395a8a3a04dc9c3f4e1ffdc63fc5fa58b1f34304a1117296d8240054cfdbc38aca88e71fb51483cf29ffab0a61ef27b481
+    "@webassemblyjs/helper-wasm-section": 1.12.1
+    "@webassemblyjs/wasm-gen": 1.12.1
+    "@webassemblyjs/wasm-opt": 1.12.1
+    "@webassemblyjs/wasm-parser": 1.12.1
+    "@webassemblyjs/wast-printer": 1.12.1
+  checksum: ae23642303f030af888d30c4ef37b08dfec7eab6851a9575a616e65d1219f880d9223913a39056dd654e49049d76e97555b285d1f7e56935047abf578cce0692
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-gen@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-gen@npm:1.11.6"
+"@webassemblyjs/wasm-gen@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-gen@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
     "@webassemblyjs/ieee754": 1.11.6
     "@webassemblyjs/leb128": 1.11.6
     "@webassemblyjs/utf8": 1.11.6
-  checksum: a645a2eecbea24833c3260a249704a7f554ef4a94c6000984728e94bb2bc9140a68dfd6fd21d5e0bbb09f6dfc98e083a45760a83ae0417b41a0196ff6d45a23a
+  checksum: 5787626bb7f0b033044471ddd00ce0c9fe1ee4584e8b73e232051e3a4c99ba1a102700d75337151c8b6055bae77eefa4548960c610a5e4a504e356bd872138ff
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-opt@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-opt@npm:1.11.6"
+"@webassemblyjs/wasm-opt@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-opt@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
-    "@webassemblyjs/helper-buffer": 1.11.6
-    "@webassemblyjs/wasm-gen": 1.11.6
-    "@webassemblyjs/wasm-parser": 1.11.6
-  checksum: b4557f195487f8e97336ddf79f7bef40d788239169aac707f6eaa2fa5fe243557c2d74e550a8e57f2788e70c7ae4e7d32f7be16101afe183d597b747a3bdd528
+    "@webassemblyjs/ast": 1.12.1
+    "@webassemblyjs/helper-buffer": 1.12.1
+    "@webassemblyjs/wasm-gen": 1.12.1
+    "@webassemblyjs/wasm-parser": 1.12.1
+  checksum: 0e8fa8a0645304a1e18ff40d3db5a2e9233ebaa169b19fcc651d6fc9fe2cac0ce092ddee927318015ae735d9cd9c5d97c0cafb6a51dcd2932ac73587b62df991
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-parser@npm:1.11.6, @webassemblyjs/wasm-parser@npm:^1.11.5":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wasm-parser@npm:1.11.6"
+"@webassemblyjs/wasm-parser@npm:1.12.1, @webassemblyjs/wasm-parser@npm:^1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wasm-parser@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
     "@webassemblyjs/helper-api-error": 1.11.6
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
     "@webassemblyjs/ieee754": 1.11.6
     "@webassemblyjs/leb128": 1.11.6
     "@webassemblyjs/utf8": 1.11.6
-  checksum: 8200a8d77c15621724a23fdabe58d5571415cda98a7058f542e670ea965dd75499f5e34a48675184947c66f3df23adf55df060312e6d72d57908e3f049620d8a
+  checksum: 176015de3551ac068cd4505d837414f258d9ade7442bd71efb1232fa26c9f6d7d4e11a5c816caeed389943f409af7ebff6899289a992d7a70343cb47009d21a8
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wast-printer@npm:1.11.6":
-  version: 1.11.6
-  resolution: "@webassemblyjs/wast-printer@npm:1.11.6"
+"@webassemblyjs/wast-printer@npm:1.12.1":
+  version: 1.12.1
+  resolution: "@webassemblyjs/wast-printer@npm:1.12.1"
   dependencies:
-    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/ast": 1.12.1
     "@xtuc/long": 4.2.2
-  checksum: d2fa6a4c427325ec81463e9c809aa6572af6d47f619f3091bf4c4a6fc34f1da3df7caddaac50b8e7a457f8784c62cd58c6311b6cb69b0162ccd8d4c072f79cf8
+  checksum: 2974b5dda8d769145ba0efd886ea94a601e61fb37114c14f9a9a7606afc23456799af652ac3052f284909bd42edc3665a76bc9b50f95f0794c053a8a1757b713
   languageName: node
   linkType: hard
 
 "@webpack-cli/configtest@npm:^2.1.1":
   version: 2.1.1
   resolution: "@webpack-cli/configtest@npm:2.1.1"
   peerDependencies:
@@ -3795,20 +3794,20 @@
   resolution: "agent-base@npm:6.0.2"
   dependencies:
     debug: 4
   checksum: f52b6872cc96fd5f622071b71ef200e01c7c4c454ee68bc9accca90c98cfb39f2810e3e9aa330435835eedc8c23f4f8a15267f67c6e245d2b33757575bdac49d
   languageName: node
   linkType: hard
 
-"agent-base@npm:^7.0.2, agent-base@npm:^7.1.0":
-  version: 7.1.0
-  resolution: "agent-base@npm:7.1.0"
+"agent-base@npm:^7.0.2, agent-base@npm:^7.1.0, agent-base@npm:^7.1.1":
+  version: 7.1.1
+  resolution: "agent-base@npm:7.1.1"
   dependencies:
     debug: ^4.3.4
-  checksum: f7828f991470a0cc22cb579c86a18cbae83d8a3cbed39992ab34fc7217c4d126017f1c74d0ab66be87f71455318a8ea3e757d6a37881b8d0f2a2c6aa55e5418f
+  checksum: 51c158769c5c051482f9ca2e6e1ec085ac72b5a418a9b31b4e82fe6c0a6699adb94c1c42d246699a587b3335215037091c79e0de512c516f73b6ea844202f037
   languageName: node
   linkType: hard
 
 "aggregate-error@npm:^3.0.0":
   version: 3.1.0
   resolution: "aggregate-error@npm:3.1.0"
   dependencies:
@@ -3953,15 +3952,15 @@
 "argparse@npm:^2.0.1":
   version: 2.0.1
   resolution: "argparse@npm:2.0.1"
   checksum: 83644b56493e89a254bae05702abf3a1101b4fa4d0ca31df1c9985275a5a5bd47b3c27b7fa0b71098d41114d8ca000e6ed90cad764b306f8a503665e4d517ced
   languageName: node
   linkType: hard
 
-"array-buffer-byte-length@npm:^1.0.0, array-buffer-byte-length@npm:^1.0.1":
+"array-buffer-byte-length@npm:^1.0.1":
   version: 1.0.1
   resolution: "array-buffer-byte-length@npm:1.0.1"
   dependencies:
     call-bind: ^1.0.5
     is-array-buffer: ^3.0.4
   checksum: 53524e08f40867f6a9f35318fafe467c32e45e9c682ba67b11943e167344d2febc0f6977a17e699b05699e805c3e8f073d876f8bbf1b559ed494ad2cd0fae09e
   languageName: node
@@ -3970,15 +3969,15 @@
 "array-union@npm:^2.1.0":
   version: 2.1.0
   resolution: "array-union@npm:2.1.0"
   checksum: 5bee12395cba82da674931df6d0fea23c4aa4660cb3b338ced9f828782a65caa232573e6bf3968f23e0c5eb301764a382cef2f128b170a9dc59de0e36c39f98d
   languageName: node
   linkType: hard
 
-"arraybuffer.prototype.slice@npm:^1.0.2":
+"arraybuffer.prototype.slice@npm:^1.0.3":
   version: 1.0.3
   resolution: "arraybuffer.prototype.slice@npm:1.0.3"
   dependencies:
     array-buffer-byte-length: ^1.0.1
     call-bind: ^1.0.5
     define-properties: ^1.2.1
     es-abstract: ^1.22.3
@@ -4007,18 +4006,20 @@
 "asynckit@npm:^0.4.0":
   version: 0.4.0
   resolution: "asynckit@npm:0.4.0"
   checksum: 7b78c451df768adba04e2d02e63e2d0bf3b07adcd6e42b4cf665cb7ce899bedd344c69a1dcbce355b5f972d597b25aaa1c1742b52cffd9caccb22f348114f6be
   languageName: node
   linkType: hard
 
-"available-typed-arrays@npm:^1.0.5, available-typed-arrays@npm:^1.0.6":
-  version: 1.0.6
-  resolution: "available-typed-arrays@npm:1.0.6"
-  checksum: 8295571eb86447138adf64a0df0c08ae61250b17190bba30e1fae8c80a816077a6d028e5506f602c382c0197d3080bae131e92e331139d55460989580eeae659
+"available-typed-arrays@npm:^1.0.7":
+  version: 1.0.7
+  resolution: "available-typed-arrays@npm:1.0.7"
+  dependencies:
+    possible-typed-array-names: ^1.0.0
+  checksum: 1aa3ffbfe6578276996de660848b6e95669d9a95ad149e3dd0c0cda77db6ee1dbd9d1dd723b65b6d277b882dd0c4b91a654ae9d3cf9e1254b7e93e4908d78fd3
   languageName: node
   linkType: hard
 
 "babel-jest@npm:^29.7.0":
   version: 29.7.0
   resolution: "babel-jest@npm:29.7.0"
   dependencies:
@@ -4056,47 +4057,47 @@
     "@babel/types": ^7.3.3
     "@types/babel__core": ^7.1.14
     "@types/babel__traverse": ^7.0.6
   checksum: 51250f22815a7318f17214a9d44650ba89551e6d4f47a2dc259128428324b52f5a73979d010cefd921fd5a720d8c1d55ad74ff601cd94c7bd44d5f6292fde2d1
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-corejs2@npm:^0.4.8":
-  version: 0.4.8
-  resolution: "babel-plugin-polyfill-corejs2@npm:0.4.8"
+"babel-plugin-polyfill-corejs2@npm:^0.4.10":
+  version: 0.4.11
+  resolution: "babel-plugin-polyfill-corejs2@npm:0.4.11"
   dependencies:
     "@babel/compat-data": ^7.22.6
-    "@babel/helper-define-polyfill-provider": ^0.5.0
+    "@babel/helper-define-polyfill-provider": ^0.6.2
     semver: ^6.3.1
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: 22857b87268b354e095452199464accba5fd8f690558a2f24b0954807ca2494b96da8d5c13507955802427582015160bce26a66893acf6da5dafbed8b336cf79
+  checksum: f098353ce7c7dde1a1d2710858e01b471e85689110c9e37813e009072347eb8c55d5f84d20d3bf1cab31755f20078ba90f8855fdc4686a9daa826a95ff280bd7
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-corejs3@npm:^0.9.0":
-  version: 0.9.0
-  resolution: "babel-plugin-polyfill-corejs3@npm:0.9.0"
+"babel-plugin-polyfill-corejs3@npm:^0.10.4":
+  version: 0.10.4
+  resolution: "babel-plugin-polyfill-corejs3@npm:0.10.4"
   dependencies:
-    "@babel/helper-define-polyfill-provider": ^0.5.0
-    core-js-compat: ^3.34.0
+    "@babel/helper-define-polyfill-provider": ^0.6.1
+    core-js-compat: ^3.36.1
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: 65bbf59fc0145c7a264822777403632008dce00015b4b5c7ec359125ef4faf9e8f494ae5123d2992104feb6f19a3cff85631992862e48b6d7bd64eb7e755ee1f
+  checksum: b96a54495f7cc8b3797251c8c15f5ed015edddc3110fc122f6b32c94bec33af1e8bc56fa99091808f500bde0cccaaa266889cdc5935d9e6e9cf09898214f02dd
   languageName: node
   linkType: hard
 
-"babel-plugin-polyfill-regenerator@npm:^0.5.5":
-  version: 0.5.5
-  resolution: "babel-plugin-polyfill-regenerator@npm:0.5.5"
+"babel-plugin-polyfill-regenerator@npm:^0.6.1":
+  version: 0.6.2
+  resolution: "babel-plugin-polyfill-regenerator@npm:0.6.2"
   dependencies:
-    "@babel/helper-define-polyfill-provider": ^0.5.0
+    "@babel/helper-define-polyfill-provider": ^0.6.2
   peerDependencies:
     "@babel/core": ^7.4.0 || ^8.0.0-0 <8.0.0
-  checksum: 3a9b4828673b23cd648dcfb571eadcd9d3fadfca0361d0a7c6feeb5a30474e92faaa49f067a6e1c05e49b6a09812879992028ff3ef3446229ff132d6e1de7eb6
+  checksum: 150233571072b6b3dfe946242da39cba8587b7f908d1c006f7545fc88b0e3c3018d445739beb61e7a75835f0c2751dbe884a94ff9b245ec42369d9267e0e1b3f
   languageName: node
   linkType: hard
 
 "babel-preset-current-node-syntax@npm:^1.0.0":
   version: 1.0.1
   resolution: "babel-preset-current-node-syntax@npm:1.0.1"
   dependencies:
@@ -4175,25 +4176,25 @@
   resolution: "braces@npm:3.0.2"
   dependencies:
     fill-range: ^7.0.1
   checksum: e2a8e769a863f3d4ee887b5fe21f63193a891c68b612ddb4b68d82d1b5f3ff9073af066c343e9867a393fe4c2555dcb33e89b937195feb9c1613d259edfcd459
   languageName: node
   linkType: hard
 
-"browserslist@npm:^4.21.10, browserslist@npm:^4.22.2":
-  version: 4.22.3
-  resolution: "browserslist@npm:4.22.3"
+"browserslist@npm:^4.21.10, browserslist@npm:^4.22.2, browserslist@npm:^4.23.0":
+  version: 4.23.0
+  resolution: "browserslist@npm:4.23.0"
   dependencies:
-    caniuse-lite: ^1.0.30001580
-    electron-to-chromium: ^1.4.648
+    caniuse-lite: ^1.0.30001587
+    electron-to-chromium: ^1.4.668
     node-releases: ^2.0.14
     update-browserslist-db: ^1.0.13
   bin:
     browserslist: cli.js
-  checksum: e62b17348e92143fe58181b02a6a97c4a98bd812d1dc9274673a54f73eec53dbed1c855ebf73e318ee00ee039f23c9a6d0e7629d24f3baef08c7a5b469742d57
+  checksum: 436f49e796782ca751ebab7edc010cfc9c29f68536f387666cd70ea22f7105563f04dd62c6ff89cb24cc3254d17cba385f979eeeb3484d43e012412ff7e75def
   languageName: node
   linkType: hard
 
 "bs-logger@npm:0.x":
   version: 0.2.6
   resolution: "bs-logger@npm:0.2.6"
   dependencies:
@@ -4234,23 +4235,24 @@
     ssri: ^10.0.0
     tar: ^6.1.11
     unique-filename: ^3.0.0
   checksum: 0250df80e1ad0c828c956744850c5f742c24244e9deb5b7dc81bca90f8c10e011e132ecc58b64497cc1cad9a98968676147fb6575f4f94722f7619757b17a11b
   languageName: node
   linkType: hard
 
-"call-bind@npm:^1.0.2, call-bind@npm:^1.0.5, call-bind@npm:^1.0.6":
-  version: 1.0.6
-  resolution: "call-bind@npm:1.0.6"
+"call-bind@npm:^1.0.2, call-bind@npm:^1.0.5, call-bind@npm:^1.0.6, call-bind@npm:^1.0.7":
+  version: 1.0.7
+  resolution: "call-bind@npm:1.0.7"
   dependencies:
+    es-define-property: ^1.0.0
     es-errors: ^1.3.0
     function-bind: ^1.1.2
-    get-intrinsic: ^1.2.3
-    set-function-length: ^1.2.0
-  checksum: 9e75989b60124df0fee40c129b2f8f401efb54e40451e18f112b64654c7d6d0dd7b6195e990edaeb3fdb447911926a19ffe1635858de00d68826ced6eeab24a9
+    get-intrinsic: ^1.2.4
+    set-function-length: ^1.2.1
+  checksum: 295c0c62b90dd6522e6db3b0ab1ce26bdf9e7404215bda13cfee25b626b5ff1a7761324d58d38b1ef1607fc65aca2d06e44d2e18d0dfc6c14b465b00d8660029
   languageName: node
   linkType: hard
 
 "callsites@npm:^3.0.0":
   version: 3.1.0
   resolution: "callsites@npm:3.1.0"
   checksum: 072d17b6abb459c2ba96598918b55868af677154bec7e73d222ef95a8fdb9bbf7dae96a8421085cdad8cd190d86653b5b6dc55a4484f2e5b2e27d5e0c3fc15b3
@@ -4278,18 +4280,18 @@
 "camelcase@npm:^6.2.0":
   version: 6.3.0
   resolution: "camelcase@npm:6.3.0"
   checksum: 8c96818a9076434998511251dcb2761a94817ea17dbdc37f47ac080bd088fc62c7369429a19e2178b993497132c8cbcf5cc1f44ba963e76782ba469c0474938d
   languageName: node
   linkType: hard
 
-"caniuse-lite@npm:^1.0.30001580":
-  version: 1.0.30001585
-  resolution: "caniuse-lite@npm:1.0.30001585"
-  checksum: c5994f0b5de857349ae0c157a3c61883e800ed154bbeab339aecf01a0a0fd24f67d23ebb48bc995c4c9cde2a281a51b682d1b14bbf2f832f6b2261119f450af4
+"caniuse-lite@npm:^1.0.30001587":
+  version: 1.0.30001614
+  resolution: "caniuse-lite@npm:1.0.30001614"
+  checksum: 1b695625f9a1b08584c3c229d4b8deaebb89e7901a2a2ffe599a6250c0a79fc61afc49c374c32a76dbf593a5dedac3229bb0140bbacd438276211bdd1d7c4958
   languageName: node
   linkType: hard
 
 "chalk@npm:^2.3.0, chalk@npm:^2.4.1, chalk@npm:^2.4.2":
   version: 2.4.2
   resolution: "chalk@npm:2.4.2"
   dependencies:
@@ -4342,17 +4344,17 @@
   version: 3.9.0
   resolution: "ci-info@npm:3.9.0"
   checksum: 6b19dc9b2966d1f8c2041a838217299718f15d6c4b63ae36e4674edd2bee48f780e94761286a56aa59eb305a85fbea4ddffb7630ec063e7ec7e7e5ad42549a87
   languageName: node
   linkType: hard
 
 "cjs-module-lexer@npm:^1.0.0":
-  version: 1.2.3
-  resolution: "cjs-module-lexer@npm:1.2.3"
-  checksum: 5ea3cb867a9bb609b6d476cd86590d105f3cfd6514db38ff71f63992ab40939c2feb68967faa15a6d2b1f90daa6416b79ea2de486e9e2485a6f8b66a21b4fb0a
+  version: 1.3.1
+  resolution: "cjs-module-lexer@npm:1.3.1"
+  checksum: 75f20ac264a397ea5c63f9c2343a51ab878043666468f275e94862f7180ec1d764a400ec0c09085dcf0db3193c74a8b571519abd2bf4be0d2be510d1377c8d4b
   languageName: node
   linkType: hard
 
 "clean-stack@npm:^2.0.0":
   version: 2.2.0
   resolution: "clean-stack@npm:2.2.0"
   checksum: 2ac8cd2b2f5ec986a3c743935ec85b07bc174d5421a5efc8017e1f146a1cf5f781ae962618f416352103b32c9cd7e203276e8c28241bbe946160cab16149fb68
@@ -4504,20 +4506,20 @@
 "convert-source-map@npm:^2.0.0":
   version: 2.0.0
   resolution: "convert-source-map@npm:2.0.0"
   checksum: 63ae9933be5a2b8d4509daca5124e20c14d023c820258e484e32dc324d34c2754e71297c94a05784064ad27615037ef677e3f0c00469fb55f409d2bb21261035
   languageName: node
   linkType: hard
 
-"core-js-compat@npm:^3.31.0, core-js-compat@npm:^3.34.0":
-  version: 3.35.1
-  resolution: "core-js-compat@npm:3.35.1"
+"core-js-compat@npm:^3.31.0, core-js-compat@npm:^3.36.1":
+  version: 3.37.0
+  resolution: "core-js-compat@npm:3.37.0"
   dependencies:
-    browserslist: ^4.22.2
-  checksum: 4c1a7076d31fa489eec5c46eb11c7127703f9756b5fed1eab9bf27b7f0f151247886d3fa488911078bd2801a5dfa12a9ea2ecb7a4e61dfa460b2c291805f503b
+    browserslist: ^4.23.0
+  checksum: cab5078e98625f889fd9bbbb19e84cb408f31c87e68302d380db0d26ae8e35c1b38cde084358ff345d4aa461af5f3c60d8a913a5b30bff3a83b4b7859374db36
   languageName: node
   linkType: hard
 
 "cosmiconfig@npm:^7.1.0":
   version: 7.1.0
   resolution: "cosmiconfig@npm:7.1.0"
   dependencies:
@@ -4575,41 +4577,41 @@
     shebang-command: ^2.0.0
     which: ^2.0.1
   checksum: 671cc7c7288c3a8406f3c69a3ae2fc85555c04169e9d611def9a675635472614f1c0ed0ef80955d5b6d4e724f6ced67f0ad1bb006c2ea643488fcfef994d7f52
   languageName: node
   linkType: hard
 
 "css-functions-list@npm:^3.1.0":
-  version: 3.2.1
-  resolution: "css-functions-list@npm:3.2.1"
-  checksum: 57d7deb3b05e84d95b88ba9b3244cf60d33b40652b3357f084c805b24a9febda5987ade44ef25a56be41e73249a7dcc157abd704d8a0e998b2c1c2e2d5de6461
+  version: 3.2.2
+  resolution: "css-functions-list@npm:3.2.2"
+  checksum: b8a564118b93b87b63236a57132a3ef581416896a70c1d0df73360a9ec43dc582f7c2a586b578feb8476179518e557c6657570a8b6185b16300c7232a84d43e3
   languageName: node
   linkType: hard
 
 "css-loader@npm:^6.7.1":
-  version: 6.10.0
-  resolution: "css-loader@npm:6.10.0"
+  version: 6.11.0
+  resolution: "css-loader@npm:6.11.0"
   dependencies:
     icss-utils: ^5.1.0
     postcss: ^8.4.33
-    postcss-modules-extract-imports: ^3.0.0
-    postcss-modules-local-by-default: ^4.0.4
-    postcss-modules-scope: ^3.1.1
+    postcss-modules-extract-imports: ^3.1.0
+    postcss-modules-local-by-default: ^4.0.5
+    postcss-modules-scope: ^3.2.0
     postcss-modules-values: ^4.0.0
     postcss-value-parser: ^4.2.0
     semver: ^7.5.4
   peerDependencies:
     "@rspack/core": 0.x || 1.x
     webpack: ^5.0.0
   peerDependenciesMeta:
     "@rspack/core":
       optional: true
     webpack:
       optional: true
-  checksum: ee3d62b5f7e4eb24281a22506431e920d07a45bd6ea627731ce583f3c6a846ab8b8b703bace599b9b35256b9e762f9f326d969abb72b69c7e6055eacf39074fd
+  checksum: 5c8d35975a7121334905394e88e28f05df72f037dbed2fb8fec4be5f0b313ae73a13894ba791867d4a4190c35896da84a7fd0c54fb426db55d85ba5e714edbe3
   languageName: node
   linkType: hard
 
 "cssesc@npm:^3.0.0":
   version: 3.0.0
   resolution: "cssesc@npm:3.0.0"
   bin:
@@ -4673,14 +4675,47 @@
     abab: ^2.0.6
     whatwg-mimetype: ^3.0.0
     whatwg-url: ^11.0.0
   checksum: 033fc3dd0fba6d24bc9a024ddcf9923691dd24f90a3d26f6545d6a2f71ec6956f93462f2cdf2183cc46f10dc01ed3bcb36731a8208456eb1a08147e571fe2a76
   languageName: node
   linkType: hard
 
+"data-view-buffer@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "data-view-buffer@npm:1.0.1"
+  dependencies:
+    call-bind: ^1.0.6
+    es-errors: ^1.3.0
+    is-data-view: ^1.0.1
+  checksum: ce24348f3c6231223b216da92e7e6a57a12b4af81a23f27eff8feabdf06acfb16c00639c8b705ca4d167f761cfc756e27e5f065d0a1f840c10b907fdaf8b988c
+  languageName: node
+  linkType: hard
+
+"data-view-byte-length@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "data-view-byte-length@npm:1.0.1"
+  dependencies:
+    call-bind: ^1.0.7
+    es-errors: ^1.3.0
+    is-data-view: ^1.0.1
+  checksum: dbb3200edcb7c1ef0d68979834f81d64fd8cab2f7691b3a4c6b97e67f22182f3ec2c8602efd7b76997b55af6ff8bce485829c1feda4fa2165a6b71fb7baa4269
+  languageName: node
+  linkType: hard
+
+"data-view-byte-offset@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "data-view-byte-offset@npm:1.0.0"
+  dependencies:
+    call-bind: ^1.0.6
+    es-errors: ^1.3.0
+    is-data-view: ^1.0.1
+  checksum: 7f0bf8720b7414ca719eedf1846aeec392f2054d7af707c5dc9a753cc77eb8625f067fa901e0b5127e831f9da9056138d894b9c2be79c27a21f6db5824f009c2
+  languageName: node
+  linkType: hard
+
 "debug@npm:4, debug@npm:^4.1.0, debug@npm:^4.1.1, debug@npm:^4.3.1, debug@npm:^4.3.2, debug@npm:^4.3.4":
   version: 4.3.4
   resolution: "debug@npm:4.3.4"
   dependencies:
     ms: 2.1.2
   peerDependenciesMeta:
     supports-color:
@@ -4710,22 +4745,22 @@
   version: 10.4.3
   resolution: "decimal.js@npm:10.4.3"
   checksum: 796404dcfa9d1dbfdc48870229d57f788b48c21c603c3f6554a1c17c10195fc1024de338b0cf9e1efe0c7c167eeb18f04548979bcc5fdfabebb7cc0ae3287bae
   languageName: node
   linkType: hard
 
 "dedent@npm:^1.0.0":
-  version: 1.5.1
-  resolution: "dedent@npm:1.5.1"
+  version: 1.5.3
+  resolution: "dedent@npm:1.5.3"
   peerDependencies:
     babel-plugin-macros: ^3.1.0
   peerDependenciesMeta:
     babel-plugin-macros:
       optional: true
-  checksum: c3c300a14edf1bdf5a873f9e4b22e839d62490bc5c8d6169c1f15858a1a76733d06a9a56930e963d677a2ceeca4b6b0894cc5ea2f501aa382ca5b92af3413c2a
+  checksum: 045b595557b2a8ea2eb9b0b4623d764e9a87326486fe2b61191b4342ed93dc01245644d8a09f3108a50c0ee7965f1eedd92e4a3a503ed89ea8e810566ea27f9a
   languageName: node
   linkType: hard
 
 "deep-is@npm:^0.1.3":
   version: 0.1.4
   resolution: "deep-is@npm:0.1.4"
   checksum: edb65dd0d7d1b9c40b2f50219aef30e116cedd6fc79290e740972c132c09106d2e80aa0bc8826673dd5a00222d4179c84b36a790eef63a4c4bca75a37ef90804
@@ -4735,23 +4770,22 @@
 "deepmerge@npm:^4.2.2":
   version: 4.3.1
   resolution: "deepmerge@npm:4.3.1"
   checksum: 2024c6a980a1b7128084170c4cf56b0fd58a63f2da1660dcfe977415f27b17dbe5888668b59d0b063753f3220719d5e400b7f113609489c90160bb9a5518d052
   languageName: node
   linkType: hard
 
-"define-data-property@npm:^1.0.1, define-data-property@npm:^1.1.2":
-  version: 1.1.2
-  resolution: "define-data-property@npm:1.1.2"
+"define-data-property@npm:^1.0.1, define-data-property@npm:^1.1.4":
+  version: 1.1.4
+  resolution: "define-data-property@npm:1.1.4"
   dependencies:
+    es-define-property: ^1.0.0
     es-errors: ^1.3.0
-    get-intrinsic: ^1.2.2
     gopd: ^1.0.1
-    has-property-descriptors: ^1.0.1
-  checksum: a903d932c83ede85d47d7764fff23435e038e8d7c2ed09a5461d59a0279bf590ed7459ac9ab468e550e24d81aa91e4de1714df155ecce4c925e94bc5ea94f9f3
+  checksum: 8068ee6cab694d409ac25936eb861eea704b7763f7f342adbdfe337fc27c78d7ae0eff2364b2917b58c508d723c7a074326d068eef2e45c4edcd85cf94d0313b
   languageName: node
   linkType: hard
 
 "define-properties@npm:^1.1.3, define-properties@npm:^1.2.0, define-properties@npm:^1.2.1":
   version: 1.2.1
   resolution: "define-properties@npm:1.2.1"
   dependencies:
@@ -4863,18 +4897,18 @@
 "eastasianwidth@npm:^0.2.0":
   version: 0.2.0
   resolution: "eastasianwidth@npm:0.2.0"
   checksum: 7d00d7cd8e49b9afa762a813faac332dee781932d6f2c848dc348939c4253f1d4564341b7af1d041853bc3f32c2ef141b58e0a4d9862c17a7f08f68df1e0f1ed
   languageName: node
   linkType: hard
 
-"electron-to-chromium@npm:^1.4.648":
-  version: 1.4.661
-  resolution: "electron-to-chromium@npm:1.4.661"
-  checksum: 7d89d8e60496ee2b713b79e266ec71972a0c0c2adc8e4c3a3753e24faf5ece173c89a7063d5a438e8a83532c2461f1c1e35b0b7897f471ea8c2f99590aa14672
+"electron-to-chromium@npm:^1.4.668":
+  version: 1.4.751
+  resolution: "electron-to-chromium@npm:1.4.751"
+  checksum: 7d8fce48b7b9997eee6bbef136044702f3fcf959a05a143e8818e4f36106024df86ed6e3aaaf83455cd1d83f5f180c8281c7cef645b798cd7a9424b2847ca15d
   languageName: node
   linkType: hard
 
 "emittery@npm:^0.13.1":
   version: 0.13.1
   resolution: "emittery@npm:0.13.1"
   checksum: 2b089ab6306f38feaabf4f6f02792f9ec85fc054fda79f44f6790e61bbf6bc4e1616afb9b232e0c5ec5289a8a452f79bfa6d905a6fd64e94b49981f0934001c6
@@ -4907,21 +4941,21 @@
   resolution: "encoding@npm:0.1.13"
   dependencies:
     iconv-lite: ^0.6.2
   checksum: bb98632f8ffa823996e508ce6a58ffcf5856330fde839ae42c9e1f436cc3b5cc651d4aeae72222916545428e54fd0f6aa8862fd8d25bdbcc4589f1e3f3715e7f
   languageName: node
   linkType: hard
 
-"enhanced-resolve@npm:^5.15.0":
-  version: 5.15.0
-  resolution: "enhanced-resolve@npm:5.15.0"
+"enhanced-resolve@npm:^5.16.0":
+  version: 5.16.0
+  resolution: "enhanced-resolve@npm:5.16.0"
   dependencies:
     graceful-fs: ^4.2.4
     tapable: ^2.2.0
-  checksum: fbd8cdc9263be71cc737aa8a7d6c57b43d6aa38f6cc75dde6fcd3598a130cc465f979d2f4d01bb3bf475acb43817749c79f8eef9be048683602ca91ab52e4f11
+  checksum: ccfd01850ecf2aa51e8554d539973319ff7d8a539ef1e0ba3460a0ccad6223c4ef6e19165ee64161b459cd8a48df10f52af4434c60023c65fde6afa32d475f7e
   languageName: node
   linkType: hard
 
 "entities@npm:^2.0.0":
   version: 2.2.0
   resolution: "entities@npm:2.2.0"
   checksum: 19010dacaf0912c895ea262b4f6128574f9ccf8d4b3b65c7e8334ad0079b3706376360e28d8843ff50a78aabcb8f08f0a32dbfacdc77e47ed77ca08b713669b3
@@ -4939,19 +4973,19 @@
   version: 2.2.1
   resolution: "env-paths@npm:2.2.1"
   checksum: 65b5df55a8bab92229ab2b40dad3b387fad24613263d103a97f91c9fe43ceb21965cd3392b1ccb5d77088021e525c4e0481adb309625d0cb94ade1d1fb8dc17e
   languageName: node
   linkType: hard
 
 "envinfo@npm:^7.7.3":
-  version: 7.11.1
-  resolution: "envinfo@npm:7.11.1"
+  version: 7.13.0
+  resolution: "envinfo@npm:7.13.0"
   bin:
     envinfo: dist/cli.js
-  checksum: f3d38ab6bc62388466e86e2f5665f90f238ca349c81bb36b311d908cb5ca96650569b43b308c9dcb6725a222693f6c43a704794e74a68fb445ec5575a90ca05e
+  checksum: 822fc30f53bd0be67f0e25be96eb6a2562b8062f3058846bbd7ec471bd4b7835fca6436ee72c4029c8ae4a3d8f8cddbe2ee725b22291f015232d20a682bee732
   languageName: node
   linkType: hard
 
 "err-code@npm:^2.0.2":
   version: 2.0.3
   resolution: "err-code@npm:2.0.3"
   checksum: 8b7b1be20d2de12d2255c0bc2ca638b7af5171142693299416e6a9339bd7d88fc8d7707d913d78e0993176005405a236b066b45666b27b797252c771156ace54
@@ -4963,83 +4997,108 @@
   resolution: "error-ex@npm:1.3.2"
   dependencies:
     is-arrayish: ^0.2.1
   checksum: c1c2b8b65f9c91b0f9d75f0debaa7ec5b35c266c2cac5de412c1a6de86d4cbae04ae44e510378cb14d032d0645a36925d0186f8bb7367bcc629db256b743a001
   languageName: node
   linkType: hard
 
-"es-abstract@npm:^1.22.1, es-abstract@npm:^1.22.3":
-  version: 1.22.3
-  resolution: "es-abstract@npm:1.22.3"
-  dependencies:
-    array-buffer-byte-length: ^1.0.0
-    arraybuffer.prototype.slice: ^1.0.2
-    available-typed-arrays: ^1.0.5
-    call-bind: ^1.0.5
-    es-set-tostringtag: ^2.0.1
+"es-abstract@npm:^1.22.1, es-abstract@npm:^1.22.3, es-abstract@npm:^1.23.0, es-abstract@npm:^1.23.2":
+  version: 1.23.3
+  resolution: "es-abstract@npm:1.23.3"
+  dependencies:
+    array-buffer-byte-length: ^1.0.1
+    arraybuffer.prototype.slice: ^1.0.3
+    available-typed-arrays: ^1.0.7
+    call-bind: ^1.0.7
+    data-view-buffer: ^1.0.1
+    data-view-byte-length: ^1.0.1
+    data-view-byte-offset: ^1.0.0
+    es-define-property: ^1.0.0
+    es-errors: ^1.3.0
+    es-object-atoms: ^1.0.0
+    es-set-tostringtag: ^2.0.3
     es-to-primitive: ^1.2.1
     function.prototype.name: ^1.1.6
-    get-intrinsic: ^1.2.2
-    get-symbol-description: ^1.0.0
+    get-intrinsic: ^1.2.4
+    get-symbol-description: ^1.0.2
     globalthis: ^1.0.3
     gopd: ^1.0.1
-    has-property-descriptors: ^1.0.0
-    has-proto: ^1.0.1
+    has-property-descriptors: ^1.0.2
+    has-proto: ^1.0.3
     has-symbols: ^1.0.3
-    hasown: ^2.0.0
-    internal-slot: ^1.0.5
-    is-array-buffer: ^3.0.2
+    hasown: ^2.0.2
+    internal-slot: ^1.0.7
+    is-array-buffer: ^3.0.4
     is-callable: ^1.2.7
-    is-negative-zero: ^2.0.2
+    is-data-view: ^1.0.1
+    is-negative-zero: ^2.0.3
     is-regex: ^1.1.4
-    is-shared-array-buffer: ^1.0.2
+    is-shared-array-buffer: ^1.0.3
     is-string: ^1.0.7
-    is-typed-array: ^1.1.12
+    is-typed-array: ^1.1.13
     is-weakref: ^1.0.2
     object-inspect: ^1.13.1
     object-keys: ^1.1.1
-    object.assign: ^4.1.4
-    regexp.prototype.flags: ^1.5.1
-    safe-array-concat: ^1.0.1
-    safe-regex-test: ^1.0.0
-    string.prototype.trim: ^1.2.8
-    string.prototype.trimend: ^1.0.7
-    string.prototype.trimstart: ^1.0.7
-    typed-array-buffer: ^1.0.0
-    typed-array-byte-length: ^1.0.0
-    typed-array-byte-offset: ^1.0.0
-    typed-array-length: ^1.0.4
+    object.assign: ^4.1.5
+    regexp.prototype.flags: ^1.5.2
+    safe-array-concat: ^1.1.2
+    safe-regex-test: ^1.0.3
+    string.prototype.trim: ^1.2.9
+    string.prototype.trimend: ^1.0.8
+    string.prototype.trimstart: ^1.0.8
+    typed-array-buffer: ^1.0.2
+    typed-array-byte-length: ^1.0.1
+    typed-array-byte-offset: ^1.0.2
+    typed-array-length: ^1.0.6
     unbox-primitive: ^1.0.2
-    which-typed-array: ^1.1.13
-  checksum: b1bdc962856836f6e72be10b58dc128282bdf33771c7a38ae90419d920fc3b36cc5d2b70a222ad8016e3fc322c367bf4e9e89fc2bc79b7e933c05b218e83d79a
+    which-typed-array: ^1.1.15
+  checksum: f840cf161224252512f9527306b57117192696571e07920f777cb893454e32999206198b4f075516112af6459daca282826d1735c450528470356d09eff3a9ae
+  languageName: node
+  linkType: hard
+
+"es-define-property@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "es-define-property@npm:1.0.0"
+  dependencies:
+    get-intrinsic: ^1.2.4
+  checksum: f66ece0a887b6dca71848fa71f70461357c0e4e7249696f81bad0a1f347eed7b31262af4a29f5d726dc026426f085483b6b90301855e647aa8e21936f07293c6
   languageName: node
   linkType: hard
 
 "es-errors@npm:^1.2.1, es-errors@npm:^1.3.0":
   version: 1.3.0
   resolution: "es-errors@npm:1.3.0"
   checksum: ec1414527a0ccacd7f15f4a3bc66e215f04f595ba23ca75cdae0927af099b5ec865f9f4d33e9d7e86f512f252876ac77d4281a7871531a50678132429b1271b5
   languageName: node
   linkType: hard
 
 "es-module-lexer@npm:^1.2.1":
-  version: 1.4.1
-  resolution: "es-module-lexer@npm:1.4.1"
-  checksum: a11b5a256d4e8e9c7d94c2fd87415ccd1591617b6edd847e064503f8eaece2d25e2e9078a02c5ce3ed5e83bb748f5b4820efbe78072c8beb07ac619c2edec35d
+  version: 1.5.2
+  resolution: "es-module-lexer@npm:1.5.2"
+  checksum: 59c47109eca80b93dda2418337b4308c194c578704dc57d5aa54973b196e378d31e92f258e5525655b99b3de8a84dda2debb9646cddf6fe8830f1bfca95ee060
   languageName: node
   linkType: hard
 
-"es-set-tostringtag@npm:^2.0.1":
-  version: 2.0.2
-  resolution: "es-set-tostringtag@npm:2.0.2"
+"es-object-atoms@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "es-object-atoms@npm:1.0.0"
   dependencies:
-    get-intrinsic: ^1.2.2
-    has-tostringtag: ^1.0.0
-    hasown: ^2.0.0
-  checksum: afcec3a4c9890ae14d7ec606204858441c801ff84f312538e1d1ccf1e5493c8b17bd672235df785f803756472cb4f2d49b87bde5237aef33411e74c22f194e07
+    es-errors: ^1.3.0
+  checksum: 26f0ff78ab93b63394e8403c353842b2272836968de4eafe97656adfb8a7c84b9099bf0fe96ed58f4a4cddc860f6e34c77f91649a58a5daa4a9c40b902744e3c
+  languageName: node
+  linkType: hard
+
+"es-set-tostringtag@npm:^2.0.3":
+  version: 2.0.3
+  resolution: "es-set-tostringtag@npm:2.0.3"
+  dependencies:
+    get-intrinsic: ^1.2.4
+    has-tostringtag: ^1.0.2
+    hasown: ^2.0.1
+  checksum: 7227fa48a41c0ce83e0377b11130d324ac797390688135b8da5c28994c0165be8b252e15cd1de41e1325e5a5412511586960213e88f9ab4a5e7d028895db5129
   languageName: node
   linkType: hard
 
 "es-to-primitive@npm:^1.2.1":
   version: 1.2.1
   resolution: "es-to-primitive@npm:1.2.1"
   dependencies:
@@ -5146,22 +5205,22 @@
   version: 3.4.3
   resolution: "eslint-visitor-keys@npm:3.4.3"
   checksum: 36e9ef87fca698b6fd7ca5ca35d7b2b6eeaaf106572e2f7fd31c12d3bfdaccdb587bba6d3621067e5aece31c8c3a348b93922ab8f7b2cbc6aaab5e1d89040c60
   languageName: node
   linkType: hard
 
 "eslint@npm:^8.36.0":
-  version: 8.56.0
-  resolution: "eslint@npm:8.56.0"
+  version: 8.57.0
+  resolution: "eslint@npm:8.57.0"
   dependencies:
     "@eslint-community/eslint-utils": ^4.2.0
     "@eslint-community/regexpp": ^4.6.1
     "@eslint/eslintrc": ^2.1.4
-    "@eslint/js": 8.56.0
-    "@humanwhocodes/config-array": ^0.11.13
+    "@eslint/js": 8.57.0
+    "@humanwhocodes/config-array": ^0.11.14
     "@humanwhocodes/module-importer": ^1.0.1
     "@nodelib/fs.walk": ^1.2.8
     "@ungap/structured-clone": ^1.2.0
     ajv: ^6.12.4
     chalk: ^4.0.0
     cross-spawn: ^7.0.2
     debug: ^4.3.2
@@ -5189,15 +5248,15 @@
     minimatch: ^3.1.2
     natural-compare: ^1.4.0
     optionator: ^0.9.3
     strip-ansi: ^6.0.1
     text-table: ^0.2.0
   bin:
     eslint: bin/eslint.js
-  checksum: 883436d1e809b4a25d9eb03d42f584b84c408dbac28b0019f6ea07b5177940bf3cca86208f749a6a1e0039b63e085ee47aca1236c30721e91f0deef5cc5a5136
+  checksum: 3a48d7ff85ab420a8447e9810d8087aea5b1df9ef68c9151732b478de698389ee656fd895635b5f2871c89ee5a2652b3f343d11e9db6f8486880374ebc74a2d9
   languageName: node
   linkType: hard
 
 "espree@npm:^9.6.0, espree@npm:^9.6.1":
   version: 9.6.1
   resolution: "espree@npm:9.6.1"
   dependencies:
@@ -5253,14 +5312,21 @@
 "esutils@npm:^2.0.2":
   version: 2.0.3
   resolution: "esutils@npm:2.0.3"
   checksum: 22b5b08f74737379a840b8ed2036a5fb35826c709ab000683b092d9054e5c2a82c27818f12604bfc2a9a76b90b6834ef081edbc1c7ae30d1627012e067c6ec87
   languageName: node
   linkType: hard
 
+"eve@npm:^0.5.4":
+  version: 0.5.4
+  resolution: "eve@npm:0.5.4"
+  checksum: 217ebf167cabaed9056733044a34809e483a58d96a1c1f925e3de99e60f501701622f359f17e5d68fbba0e4fd39391cc62ad284bffcf714efba32b2eee1f5899
+  languageName: node
+  linkType: hard
+
 "events@npm:^3.2.0":
   version: 3.3.0
   resolution: "events@npm:3.3.0"
   checksum: f6f487ad2198aa41d878fa31452f1a3c00958f46e9019286ff4787c84aac329332ab45c9cdc8c445928fc6d7ded294b9e005a7fce9426488518017831b272780
   languageName: node
   linkType: hard
 
@@ -5443,17 +5509,17 @@
   bin:
     flat: cli.js
   checksum: 12a1536ac746db74881316a181499a78ef953632ddd28050b7a3a43c62ef5462e3357c8c29d76072bb635f147f7a9a1f0c02efef6b4be28f8db62ceb3d5c7f5d
   languageName: node
   linkType: hard
 
 "flatted@npm:^3.2.9":
-  version: 3.2.9
-  resolution: "flatted@npm:3.2.9"
-  checksum: f14167fbe26a9d20f6fca8d998e8f1f41df72c8e81f9f2c9d61ed2bea058248f5e1cbd05e7f88c0e5087a6a0b822a1e5e2b446e879f3cfbe0b07ba2d7f80b026
+  version: 3.3.1
+  resolution: "flatted@npm:3.3.1"
+  checksum: 85ae7181650bb728c221e7644cbc9f4bf28bc556f2fc89bb21266962bdf0ce1029cc7acc44bb646cd469d9baac7c317f64e841c4c4c00516afa97320cdac7f94
   languageName: node
   linkType: hard
 
 "for-each@npm:^0.3.3":
   version: 0.3.3
   resolution: "for-each@npm:0.3.3"
   dependencies:
@@ -5581,15 +5647,15 @@
 "get-caller-file@npm:^2.0.5":
   version: 2.0.5
   resolution: "get-caller-file@npm:2.0.5"
   checksum: b9769a836d2a98c3ee734a88ba712e62703f1df31b94b784762c433c27a386dd6029ff55c2a920c392e33657d80191edbf18c61487e198844844516f843496b9
   languageName: node
   linkType: hard
 
-"get-intrinsic@npm:^1.1.3, get-intrinsic@npm:^1.2.1, get-intrinsic@npm:^1.2.2, get-intrinsic@npm:^1.2.3, get-intrinsic@npm:^1.2.4":
+"get-intrinsic@npm:^1.1.3, get-intrinsic@npm:^1.2.1, get-intrinsic@npm:^1.2.3, get-intrinsic@npm:^1.2.4":
   version: 1.2.4
   resolution: "get-intrinsic@npm:1.2.4"
   dependencies:
     es-errors: ^1.3.0
     function-bind: ^1.1.2
     has-proto: ^1.0.1
     has-symbols: ^1.0.3
@@ -5608,15 +5674,15 @@
 "get-stream@npm:^6.0.0":
   version: 6.0.1
   resolution: "get-stream@npm:6.0.1"
   checksum: e04ecece32c92eebf5b8c940f51468cd53554dcbb0ea725b2748be583c9523d00128137966afce410b9b051eb2ef16d657cd2b120ca8edafcf5a65e81af63cad
   languageName: node
   linkType: hard
 
-"get-symbol-description@npm:^1.0.0":
+"get-symbol-description@npm:^1.0.2":
   version: 1.0.2
   resolution: "get-symbol-description@npm:1.0.2"
   dependencies:
     call-bind: ^1.0.5
     es-errors: ^1.3.0
     get-intrinsic: ^1.2.4
   checksum: e1cb53bc211f9dbe9691a4f97a46837a553c4e7caadd0488dc24ac694db8a390b93edd412b48dcdd0b4bbb4c595de1709effc75fc87c0839deedc6968f5bd973
@@ -5645,25 +5711,25 @@
   version: 0.4.1
   resolution: "glob-to-regexp@npm:0.4.1"
   checksum: e795f4e8f06d2a15e86f76e4d92751cf8bbfcf0157cea5c2f0f35678a8195a750b34096b1256e436f0cebc1883b5ff0888c47348443e69546a5a87f9e1eb1167
   languageName: node
   linkType: hard
 
 "glob@npm:^10.2.2, glob@npm:^10.3.10":
-  version: 10.3.10
-  resolution: "glob@npm:10.3.10"
+  version: 10.3.12
+  resolution: "glob@npm:10.3.12"
   dependencies:
     foreground-child: ^3.1.0
-    jackspeak: ^2.3.5
+    jackspeak: ^2.3.6
     minimatch: ^9.0.1
-    minipass: ^5.0.0 || ^6.0.2 || ^7.0.0
-    path-scurry: ^1.10.1
+    minipass: ^7.0.4
+    path-scurry: ^1.10.2
   bin:
     glob: dist/esm/bin.mjs
-  checksum: 4f2fe2511e157b5a3f525a54092169a5f92405f24d2aed3142f4411df328baca13059f4182f1db1bf933e2c69c0bd89e57ae87edd8950cba8c7ccbe84f721cf3
+  checksum: 2b0949d6363021aaa561b108ac317bf5a97271b8a5d7a5fac1a176e40e8068ecdcccc992f8a7e958593d501103ac06d673de92adc1efcbdab45edefe35f8d7c6
   languageName: node
   linkType: hard
 
 "glob@npm:^7.1.3, glob@npm:^7.1.4":
   version: 7.2.3
   resolution: "glob@npm:7.2.3"
   dependencies:
@@ -5774,15 +5840,15 @@
   resolution: "gopd@npm:1.0.1"
   dependencies:
     get-intrinsic: ^1.1.3
   checksum: a5ccfb8806e0917a94e0b3de2af2ea4979c1da920bc381667c260e00e7cafdbe844e2cb9c5bcfef4e5412e8bf73bab837285bc35c7ba73aaaf0134d4583393a6
   languageName: node
   linkType: hard
 
-"graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.6, graceful-fs@npm:^4.2.9":
+"graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.11, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.6, graceful-fs@npm:^4.2.9":
   version: 4.2.11
   resolution: "graceful-fs@npm:4.2.11"
   checksum: ac85f94da92d8eb6b7f5a8b20ce65e43d66761c55ce85ac96df6865308390da45a8d3f0296dd3a663de65d30ba497bd46c696cc1e248c72b13d6d567138a4fc7
   languageName: node
   linkType: hard
 
 "graphemer@npm:^1.4.0":
@@ -5823,52 +5889,62 @@
 "has-flag@npm:^4.0.0":
   version: 4.0.0
   resolution: "has-flag@npm:4.0.0"
   checksum: 261a1357037ead75e338156b1f9452c016a37dcd3283a972a30d9e4a87441ba372c8b81f818cd0fbcd9c0354b4ae7e18b9e1afa1971164aef6d18c2b6095a8ad
   languageName: node
   linkType: hard
 
-"has-property-descriptors@npm:^1.0.0, has-property-descriptors@npm:^1.0.1":
-  version: 1.0.1
-  resolution: "has-property-descriptors@npm:1.0.1"
+"has-property-descriptors@npm:^1.0.0, has-property-descriptors@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "has-property-descriptors@npm:1.0.2"
   dependencies:
-    get-intrinsic: ^1.2.2
-  checksum: 2bcc6bf6ec6af375add4e4b4ef586e43674850a91ad4d46666d0b28ba8e1fd69e424c7677d24d60f69470ad0afaa2f3197f508b20b0bb7dd99a8ab77ffc4b7c4
+    es-define-property: ^1.0.0
+  checksum: fcbb246ea2838058be39887935231c6d5788babed499d0e9d0cc5737494c48aba4fe17ba1449e0d0fbbb1e36175442faa37f9c427ae357d6ccb1d895fbcd3de3
   languageName: node
   linkType: hard
 
-"has-proto@npm:^1.0.1":
-  version: 1.0.1
-  resolution: "has-proto@npm:1.0.1"
-  checksum: febc5b5b531de8022806ad7407935e2135f1cc9e64636c3916c6842bd7995994ca3b29871ecd7954bd35f9e2986c17b3b227880484d22259e2f8e6ce63fd383e
+"has-proto@npm:^1.0.1, has-proto@npm:^1.0.3":
+  version: 1.0.3
+  resolution: "has-proto@npm:1.0.3"
+  checksum: fe7c3d50b33f50f3933a04413ed1f69441d21d2d2944f81036276d30635cad9279f6b43bc8f32036c31ebdfcf6e731150f46c1907ad90c669ffe9b066c3ba5c4
   languageName: node
   linkType: hard
 
 "has-symbols@npm:^1.0.2, has-symbols@npm:^1.0.3":
   version: 1.0.3
   resolution: "has-symbols@npm:1.0.3"
   checksum: a054c40c631c0d5741a8285010a0777ea0c068f99ed43e5d6eb12972da223f8af553a455132fdb0801bdcfa0e0f443c0c03a68d8555aa529b3144b446c3f2410
   languageName: node
   linkType: hard
 
-"has-tostringtag@npm:^1.0.0, has-tostringtag@npm:^1.0.1":
+"has-tostringtag@npm:^1.0.0, has-tostringtag@npm:^1.0.2":
   version: 1.0.2
   resolution: "has-tostringtag@npm:1.0.2"
   dependencies:
     has-symbols: ^1.0.3
   checksum: 999d60bb753ad714356b2c6c87b7fb74f32463b8426e159397da4bde5bca7e598ab1073f4d8d4deafac297f2eb311484cd177af242776bf05f0d11565680468d
   languageName: node
   linkType: hard
 
-"hasown@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "hasown@npm:2.0.0"
+"hasown@npm:^2.0.0, hasown@npm:^2.0.1, hasown@npm:^2.0.2":
+  version: 2.0.2
+  resolution: "hasown@npm:2.0.2"
   dependencies:
     function-bind: ^1.1.2
-  checksum: 6151c75ca12554565098641c98a40f4cc86b85b0fd5b6fe92360967e4605a4f9610f7757260b4e8098dd1c2ce7f4b095f2006fe72a570e3b6d2d28de0298c176
+  checksum: e8516f776a15149ca6c6ed2ae3110c417a00b62260e222590e54aa367cbcd6ed99122020b37b7fbdf05748df57b265e70095d7bf35a47660587619b15ffb93db
+  languageName: node
+  linkType: hard
+
+"hatch@npm:^1.1.0":
+  version: 1.1.0
+  resolution: "hatch@npm:1.1.0"
+  dependencies:
+    debug: ^4.1.0
+    eve: ^0.5.4
+  checksum: eaf26b57f6ee4a1b4789d247cfaba71e3a602c6fafbbd6ae9dbc9543715582b634880c0027c635d0ca5c5893d76e2f3aa57244b607cf207bbe5441952f5243b4
   languageName: node
   linkType: hard
 
 "hosted-git-info@npm:^2.1.4":
   version: 2.8.9
   resolution: "hosted-git-info@npm:2.8.9"
   checksum: c955394bdab888a1e9bb10eb33029e0f7ce5a2ac7b3f158099dc8c486c99e73809dca609f5694b223920ca2174db33d32b12f9a2a47141dc59607c29da5a62dd
@@ -5934,40 +6010,40 @@
     agent-base: 6
     debug: 4
   checksum: e2ee1ff1656a131953839b2a19cd1f3a52d97c25ba87bd2559af6ae87114abf60971e498021f9b73f9fd78aea8876d1fb0d4656aac8a03c6caa9fc175f22b786
   languageName: node
   linkType: hard
 
 "http-proxy-agent@npm:^7.0.0":
-  version: 7.0.0
-  resolution: "http-proxy-agent@npm:7.0.0"
+  version: 7.0.2
+  resolution: "http-proxy-agent@npm:7.0.2"
   dependencies:
     agent-base: ^7.1.0
     debug: ^4.3.4
-  checksum: 48d4fac997917e15f45094852b63b62a46d0c8a4f0b9c6c23ca26d27b8df8d178bed88389e604745e748bd9a01f5023e25093722777f0593c3f052009ff438b6
+  checksum: 670858c8f8f3146db5889e1fa117630910101db601fff7d5a8aa637da0abedf68c899f03d3451cac2f83bcc4c3d2dabf339b3aa00ff8080571cceb02c3ce02f3
   languageName: node
   linkType: hard
 
 "https-proxy-agent@npm:^5.0.1":
   version: 5.0.1
   resolution: "https-proxy-agent@npm:5.0.1"
   dependencies:
     agent-base: 6
     debug: 4
   checksum: 571fccdf38184f05943e12d37d6ce38197becdd69e58d03f43637f7fa1269cf303a7d228aa27e5b27bbd3af8f09fd938e1c91dcfefff2df7ba77c20ed8dfc765
   languageName: node
   linkType: hard
 
 "https-proxy-agent@npm:^7.0.1":
-  version: 7.0.2
-  resolution: "https-proxy-agent@npm:7.0.2"
+  version: 7.0.4
+  resolution: "https-proxy-agent@npm:7.0.4"
   dependencies:
     agent-base: ^7.0.2
     debug: 4
-  checksum: 088969a0dd476ea7a0ed0a2cf1283013682b08f874c3bc6696c83fa061d2c157d29ef0ad3eb70a2046010bb7665573b2388d10fdcb3e410a66995e5248444292
+  checksum: daaab857a967a2519ddc724f91edbbd388d766ff141b9025b629f92b9408fc83cee8a27e11a907aede392938e9c398e240d643e178408a59e4073539cde8cfe9
   languageName: node
   linkType: hard
 
 "human-signals@npm:^2.1.0":
   version: 2.1.0
   resolution: "human-signals@npm:2.1.0"
   checksum: b87fd89fce72391625271454e70f67fe405277415b48bcc0117ca73d31fa23a4241787afdc8d67f5a116cf37258c052f59ea82daffa72364d61351423848e3b8
@@ -6071,15 +6147,15 @@
 "ini@npm:^1.3.5":
   version: 1.3.8
   resolution: "ini@npm:1.3.8"
   checksum: dfd98b0ca3a4fc1e323e38a6c8eb8936e31a97a918d3b377649ea15bdb15d481207a0dda1021efbd86b464cae29a0d33c1d7dcaf6c5672bee17fa849bc50a1b3
   languageName: node
   linkType: hard
 
-"internal-slot@npm:^1.0.5":
+"internal-slot@npm:^1.0.7":
   version: 1.0.7
   resolution: "internal-slot@npm:1.0.7"
   dependencies:
     es-errors: ^1.3.0
     hasown: ^2.0.0
     side-channel: ^1.0.4
   checksum: cadc5eea5d7d9bc2342e93aae9f31f04c196afebb11bde97448327049f492cd7081e18623ae71388aac9cd237b692ca3a105be9c68ac39c1dec679d7409e33eb
@@ -6089,22 +6165,25 @@
 "interpret@npm:^3.1.1":
   version: 3.1.1
   resolution: "interpret@npm:3.1.1"
   checksum: 35cebcf48c7351130437596d9ab8c8fe131ce4038da4561e6d665f25640e0034702a031cf7e3a5cea60ac7ac548bf17465e0571ede126f3d3a6933152171ac82
   languageName: node
   linkType: hard
 
-"ip@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "ip@npm:2.0.0"
-  checksum: cfcfac6b873b701996d71ec82a7dd27ba92450afdb421e356f44044ed688df04567344c36cbacea7d01b1c39a4c732dc012570ebe9bebfb06f27314bca625349
+"ip-address@npm:^9.0.5":
+  version: 9.0.5
+  resolution: "ip-address@npm:9.0.5"
+  dependencies:
+    jsbn: 1.1.0
+    sprintf-js: ^1.1.3
+  checksum: aa15f12cfd0ef5e38349744e3654bae649a34c3b10c77a674a167e99925d1549486c5b14730eebce9fea26f6db9d5e42097b00aa4f9f612e68c79121c71652dc
   languageName: node
   linkType: hard
 
-"is-array-buffer@npm:^3.0.2, is-array-buffer@npm:^3.0.4":
+"is-array-buffer@npm:^3.0.4":
   version: 3.0.4
   resolution: "is-array-buffer@npm:3.0.4"
   dependencies:
     call-bind: ^1.0.2
     get-intrinsic: ^1.2.1
   checksum: e4e3e6ef0ff2239e75371d221f74bc3c26a03564a22efb39f6bb02609b598917ddeecef4e8c877df2a25888f247a98198959842a5e73236bc7f22cabdf6351a7
   languageName: node
@@ -6148,14 +6227,23 @@
   resolution: "is-core-module@npm:2.13.1"
   dependencies:
     hasown: ^2.0.0
   checksum: 256559ee8a9488af90e4bad16f5583c6d59e92f0742e9e8bb4331e758521ee86b810b93bae44f390766ffbc518a0488b18d9dab7da9a5ff997d499efc9403f7c
   languageName: node
   linkType: hard
 
+"is-data-view@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "is-data-view@npm:1.0.1"
+  dependencies:
+    is-typed-array: ^1.1.13
+  checksum: 4ba4562ac2b2ec005fefe48269d6bd0152785458cd253c746154ffb8a8ab506a29d0cfb3b74af87513843776a88e4981ae25c89457bf640a33748eab1a7216b5
+  languageName: node
+  linkType: hard
+
 "is-date-object@npm:^1.0.1":
   version: 1.0.5
   resolution: "is-date-object@npm:1.0.5"
   dependencies:
     has-tostringtag: ^1.0.0
   checksum: baa9077cdf15eb7b58c79398604ca57379b2fc4cf9aa7a9b9e295278648f628c9b201400c01c5e0f7afae56507d741185730307cbe7cad3b9f90a77e5ee342fc
   languageName: node
@@ -6194,18 +6282,18 @@
 "is-lambda@npm:^1.0.1":
   version: 1.0.1
   resolution: "is-lambda@npm:1.0.1"
   checksum: 93a32f01940220532e5948538699ad610d5924ac86093fcee83022252b363eb0cc99ba53ab084a04e4fb62bf7b5731f55496257a4c38adf87af9c4d352c71c35
   languageName: node
   linkType: hard
 
-"is-negative-zero@npm:^2.0.2":
-  version: 2.0.2
-  resolution: "is-negative-zero@npm:2.0.2"
-  checksum: f3232194c47a549da60c3d509c9a09be442507616b69454716692e37ae9f37c4dea264fb208ad0c9f3efd15a796a46b79df07c7e53c6227c32170608b809149a
+"is-negative-zero@npm:^2.0.3":
+  version: 2.0.3
+  resolution: "is-negative-zero@npm:2.0.3"
+  checksum: c1e6b23d2070c0539d7b36022d5a94407132411d01aba39ec549af824231f3804b1aea90b5e4e58e807a65d23ceb538ed6e355ce76b267bdd86edb757ffcbdcd
   languageName: node
   linkType: hard
 
 "is-number-object@npm:^1.0.4":
   version: 1.0.7
   resolution: "is-number-object@npm:1.0.7"
   dependencies:
@@ -6264,20 +6352,20 @@
   dependencies:
     call-bind: ^1.0.2
     has-tostringtag: ^1.0.0
   checksum: 362399b33535bc8f386d96c45c9feb04cf7f8b41c182f54174c1a45c9abbbe5e31290bbad09a458583ff6bf3b2048672cdb1881b13289569a7c548370856a652
   languageName: node
   linkType: hard
 
-"is-shared-array-buffer@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "is-shared-array-buffer@npm:1.0.2"
+"is-shared-array-buffer@npm:^1.0.2, is-shared-array-buffer@npm:^1.0.3":
+  version: 1.0.3
+  resolution: "is-shared-array-buffer@npm:1.0.3"
   dependencies:
-    call-bind: ^1.0.2
-  checksum: 9508929cf14fdc1afc9d61d723c6e8d34f5e117f0bffda4d97e7a5d88c3a8681f633a74f8e3ad1fe92d5113f9b921dc5ca44356492079612f9a247efbce7032a
+    call-bind: ^1.0.7
+  checksum: a4fff602c309e64ccaa83b859255a43bb011145a42d3f56f67d9268b55bc7e6d98a5981a1d834186ad3105d6739d21547083fe7259c76c0468483fc538e716d8
   languageName: node
   linkType: hard
 
 "is-stream@npm:^2.0.0":
   version: 2.0.1
   resolution: "is-stream@npm:2.0.1"
   checksum: b8e05ccdf96ac330ea83c12450304d4a591f9958c11fd17bed240af8d5ffe08aedafa4c0f4cfccd4d28dc9d4d129daca1023633d5c11601a6cbc77521f6fae66
@@ -6298,15 +6386,15 @@
   resolution: "is-symbol@npm:1.0.4"
   dependencies:
     has-symbols: ^1.0.2
   checksum: 92805812ef590738d9de49d677cd17dfd486794773fb6fa0032d16452af46e9b91bb43ffe82c983570f015b37136f4b53b28b8523bfb10b0ece7a66c31a54510
   languageName: node
   linkType: hard
 
-"is-typed-array@npm:^1.1.10, is-typed-array@npm:^1.1.12, is-typed-array@npm:^1.1.13, is-typed-array@npm:^1.1.9":
+"is-typed-array@npm:^1.1.13":
   version: 1.1.13
   resolution: "is-typed-array@npm:1.1.13"
   dependencies:
     which-typed-array: ^1.1.14
   checksum: 150f9ada183a61554c91e1c4290086d2c100b0dff45f60b028519be72a8db964da403c48760723bf5253979b8dffe7b544246e0e5351dcd05c5fdb1dcc1dc0f0
   languageName: node
   linkType: hard
@@ -6372,23 +6460,23 @@
     istanbul-lib-coverage: ^3.2.0
     semver: ^6.3.0
   checksum: bf16f1803ba5e51b28bbd49ed955a736488381e09375d830e42ddeb403855b2006f850711d95ad726f2ba3f1ae8e7366de7e51d2b9ac67dc4d80191ef7ddf272
   languageName: node
   linkType: hard
 
 "istanbul-lib-instrument@npm:^6.0.0":
-  version: 6.0.1
-  resolution: "istanbul-lib-instrument@npm:6.0.1"
+  version: 6.0.2
+  resolution: "istanbul-lib-instrument@npm:6.0.2"
   dependencies:
-    "@babel/core": ^7.12.3
-    "@babel/parser": ^7.14.7
-    "@istanbuljs/schema": ^0.1.2
+    "@babel/core": ^7.23.9
+    "@babel/parser": ^7.23.9
+    "@istanbuljs/schema": ^0.1.3
     istanbul-lib-coverage: ^3.2.0
     semver: ^7.5.4
-  checksum: fb23472e739cfc9b027cefcd7d551d5e7ca7ff2817ae5150fab99fe42786a7f7b56a29a2aa8309c37092e18297b8003f9c274f50ca4360949094d17fbac81472
+  checksum: c10aa1e93a022f9767d7f41e6c07d244cc0a5c090fbb5522d70a5f21fcb98c52b7038850276c6fd1a7a17d1868c14a9d4eb8a24efe58a0ebb9a06f3da68131fe
   languageName: node
   linkType: hard
 
 "istanbul-lib-report@npm:^3.0.0":
   version: 3.0.1
   resolution: "istanbul-lib-report@npm:3.0.1"
   dependencies:
@@ -6407,24 +6495,24 @@
     istanbul-lib-coverage: ^3.0.0
     source-map: ^0.6.1
   checksum: 21ad3df45db4b81852b662b8d4161f6446cd250c1ddc70ef96a585e2e85c26ed7cd9c2a396a71533cfb981d1a645508bc9618cae431e55d01a0628e7dec62ef2
   languageName: node
   linkType: hard
 
 "istanbul-reports@npm:^3.1.3":
-  version: 3.1.6
-  resolution: "istanbul-reports@npm:3.1.6"
+  version: 3.1.7
+  resolution: "istanbul-reports@npm:3.1.7"
   dependencies:
     html-escaper: ^2.0.0
     istanbul-lib-report: ^3.0.0
-  checksum: 44c4c0582f287f02341e9720997f9e82c071627e1e862895745d5f52ec72c9b9f38e1d12370015d2a71dcead794f34c7732aaef3fab80a24bc617a21c3d911d6
+  checksum: 2072db6e07bfbb4d0eb30e2700250636182398c1af811aea5032acb219d2080f7586923c09fa194029efd6b92361afb3dcbe1ebcc3ee6651d13340f7c6c4ed95
   languageName: node
   linkType: hard
 
-"jackspeak@npm:^2.3.5":
+"jackspeak@npm:^2.3.6":
   version: 2.3.6
   resolution: "jackspeak@npm:2.3.6"
   dependencies:
     "@isaacs/cliui": ^8.0.2
     "@pkgjs/parseargs": ^0.11.0
   dependenciesMeta:
     "@pkgjs/parseargs":
@@ -6942,14 +7030,21 @@
     argparse: ^2.0.1
   bin:
     js-yaml: bin/js-yaml.js
   checksum: c7830dfd456c3ef2c6e355cc5a92e6700ceafa1d14bba54497b34a99f0376cecbb3e9ac14d3e5849b426d5a5140709a66237a8c991c675431271c4ce5504151a
   languageName: node
   linkType: hard
 
+"jsbn@npm:1.1.0":
+  version: 1.1.0
+  resolution: "jsbn@npm:1.1.0"
+  checksum: 944f924f2bd67ad533b3850eee47603eed0f6ae425fd1ee8c760f477e8c34a05f144c1bd4f5a5dd1963141dc79a2c55f89ccc5ab77d039e7077f3ad196b64965
+  languageName: node
+  linkType: hard
+
 "jsdom@npm:^20.0.0":
   version: 20.0.3
   resolution: "jsdom@npm:20.0.3"
   dependencies:
     abab: ^2.0.6
     acorn: ^8.8.1
     acorn-globals: ^7.0.0
@@ -7106,14 +7201,15 @@
     "@types/react": ^18.0.26
     "@typescript-eslint/eslint-plugin": ^5.55.0
     "@typescript-eslint/parser": ^5.55.0
     css-loader: ^6.7.1
     eslint: ^8.36.0
     eslint-config-prettier: ^8.7.0
     eslint-plugin-prettier: ^4.2.1
+    hatch: ^1.1.0
     jest: ^29.2.0
     npm-run-all: ^4.1.5
     prettier: ^2.8.7
     rimraf: ^4.4.1
     source-map-loader: ^1.0.2
     style-loader: ^3.3.1
     stylelint: ^14.9.1
@@ -7170,22 +7266,23 @@
     prelude-ls: ^1.2.1
     type-check: ~0.4.0
   checksum: 12c5021c859bd0f5248561bf139121f0358285ec545ebf48bb3d346820d5c61a4309535c7f387ed7d84361cf821e124ce346c6b7cef8ee09a67c1473b46d0fc4
   languageName: node
   linkType: hard
 
 "lib0@npm:^0.2.85, lib0@npm:^0.2.86":
-  version: 0.2.88
-  resolution: "lib0@npm:0.2.88"
+  version: 0.2.93
+  resolution: "lib0@npm:0.2.93"
   dependencies:
     isomorphic.js: ^0.2.4
   bin:
+    0ecdsa-generate-keypair: bin/0ecdsa-generate-keypair.js
     0gentesthtml: bin/gentesthtml.js
     0serve: bin/0serve.js
-  checksum: 1ac13d6781f4d29aa317ad9fb9b6c41e8bed52b096a369f54d10d9b8651ceb4a0a63b06c01c2e1c7319d3bb74668afb6cac3735161b32031f185cec024bbba37
+  checksum: 4c482aba249c471316fdec360ee4ace2a70ae42faad5fb6862aebb6786e187de9470eb082a5675489c59ffe54b005a15711a3d7dba33764bcab56349e61a1520
   languageName: node
   linkType: hard
 
 "license-webpack-plugin@npm:^2.3.14":
   version: 2.3.21
   resolution: "license-webpack-plugin@npm:2.3.21"
   dependencies:
@@ -7316,18 +7413,18 @@
     js-tokens: ^3.0.0 || ^4.0.0
   bin:
     loose-envify: cli.js
   checksum: 6517e24e0cad87ec9888f500c5b5947032cdfe6ef65e1c1936a0c48a524b81e65542c9c3edc91c97d5bddc806ee2a985dbc79be89215d613b1de5db6d1cfe6f4
   languageName: node
   linkType: hard
 
-"lru-cache@npm:^10.0.1, lru-cache@npm:^9.1.1 || ^10.0.0":
-  version: 10.2.0
-  resolution: "lru-cache@npm:10.2.0"
-  checksum: eee7ddda4a7475deac51ac81d7dd78709095c6fa46e8350dc2d22462559a1faa3b81ed931d5464b13d48cbd7e08b46100b6f768c76833912bc444b99c37e25db
+"lru-cache@npm:^10.0.1, lru-cache@npm:^10.2.0":
+  version: 10.2.2
+  resolution: "lru-cache@npm:10.2.2"
+  checksum: 98e8fc93691c546f719a76103ef2bee5a3ac823955c755a47641ec41f8c7fafa1baeaba466937cc1cbfa9cfd47e03536d10e2db3158a64ad91ff3a58a32c893e
   languageName: node
   linkType: hard
 
 "lru-cache@npm:^5.1.1":
   version: 5.1.1
   resolution: "lru-cache@npm:5.1.1"
   dependencies:
@@ -7400,19 +7497,19 @@
   version: 4.3.0
   resolution: "map-obj@npm:4.3.0"
   checksum: fbc554934d1a27a1910e842bc87b177b1a556609dd803747c85ece420692380827c6ae94a95cce4407c054fa0964be3bf8226f7f2cb2e9eeee432c7c1985684e
   languageName: node
   linkType: hard
 
 "markdown-to-jsx@npm:^7.4.1":
-  version: 7.4.1
-  resolution: "markdown-to-jsx@npm:7.4.1"
+  version: 7.4.7
+  resolution: "markdown-to-jsx@npm:7.4.7"
   peerDependencies:
     react: ">= 0.14.0"
-  checksum: 2888cb2389cb810ab35454a59d0623474a60a78e28f281ae0081f87053f6c59b033232a2cd269cc383a5edcaa1eab8ca4b3cf639fe4e1aa3fb418648d14bcc7d
+  checksum: bb8a696c8a95dd67ac1eb44255f31cf17e60b6c2ff03bfcd51b5e28da17856c57d7a16da59fda7f3a4eedb01d7e92eeef57a10ff3abd5431e5c80059d4565016
   languageName: node
   linkType: hard
 
 "mathml-tag-names@npm:^2.1.3":
   version: 2.1.3
   resolution: "mathml-tag-names@npm:2.1.3"
   checksum: 1201a25a137d6b9e328facd67912058b8b45b19a6c4cc62641c9476195da28a275ca6e0eca070af5378b905c2b11abc1114676ba703411db0b9ce007de921ad0
@@ -7497,22 +7594,22 @@
   version: 1.0.1
   resolution: "min-indent@npm:1.0.1"
   checksum: bfc6dd03c5eaf623a4963ebd94d087f6f4bbbfd8c41329a7f09706b0cb66969c4ddd336abeb587bc44bc6f08e13bf90f0b374f9d71f9f01e04adc2cd6f083ef1
   languageName: node
   linkType: hard
 
 "mini-css-extract-plugin@npm:^2.7.0":
-  version: 2.8.0
-  resolution: "mini-css-extract-plugin@npm:2.8.0"
+  version: 2.9.0
+  resolution: "mini-css-extract-plugin@npm:2.9.0"
   dependencies:
     schema-utils: ^4.0.0
     tapable: ^2.2.1
   peerDependencies:
     webpack: ^5.0.0
-  checksum: c1edc3ee0e1b3514c3323fa72ad38e993f357964e76737f1d7bb6cf50a0af1ac071080ec16b4e1a94688d23f78533944badad50cd0f00d2ae176f9c58c1f2029
+  checksum: ae192c67ba85ac8bffeab66774635bf90181f00d5dd6cf95412426192599ddf5506fb4b1550acbd7a5476476e39db53c770dd40f8378f7baf5de96e3fec4e6e9
   languageName: node
   linkType: hard
 
 "mini-svg-data-uri@npm:^1.4.4":
   version: 1.4.4
   resolution: "mini-svg-data-uri@npm:1.4.4"
   bin:
@@ -7536,19 +7633,19 @@
   dependencies:
     brace-expansion: ^2.0.1
   checksum: 2e46cffb86bacbc524ad45a6426f338920c529dd13f3a732cc2cf7618988ee1aae88df4ca28983285aca9e0f45222019ac2d14ebd17c1edadd2ee12221ab801a
   languageName: node
   linkType: hard
 
 "minimatch@npm:^9.0.1":
-  version: 9.0.3
-  resolution: "minimatch@npm:9.0.3"
+  version: 9.0.4
+  resolution: "minimatch@npm:9.0.4"
   dependencies:
     brace-expansion: ^2.0.1
-  checksum: 253487976bf485b612f16bf57463520a14f512662e592e95c571afdab1442a6a6864b6c88f248ce6fc4ff0b6de04ac7aa6c8bb51e868e99d1d65eb0658a708b5
+  checksum: cf717f597ec3eed7dabc33153482a2e8d49f4fd3c26e58fd9c71a94c5029a0838728841b93f46bf1263b65a8010e2ee800d0dc9b004ab8ba8b6d1ec07cc115b5
   languageName: node
   linkType: hard
 
 "minimist-options@npm:4.1.0":
   version: 4.1.0
   resolution: "minimist-options@npm:4.1.0"
   dependencies:
@@ -7636,15 +7733,15 @@
 "minipass@npm:^5.0.0":
   version: 5.0.0
   resolution: "minipass@npm:5.0.0"
   checksum: 425dab288738853fded43da3314a0b5c035844d6f3097a8e3b5b29b328da8f3c1af6fc70618b32c29ff906284cf6406b6841376f21caaadd0793c1d5a6a620ea
   languageName: node
   linkType: hard
 
-"minipass@npm:^5.0.0 || ^6.0.2 || ^7.0.0, minipass@npm:^7.0.2, minipass@npm:^7.0.3":
+"minipass@npm:^5.0.0 || ^6.0.2 || ^7.0.0, minipass@npm:^7.0.2, minipass@npm:^7.0.3, minipass@npm:^7.0.4":
   version: 7.0.4
   resolution: "minipass@npm:7.0.4"
   checksum: 87585e258b9488caf2e7acea242fd7856bbe9a2c84a7807643513a338d66f368c7d518200ad7b70a508664d408aa000517647b2930c259a8b1f9f0984f344a21
   languageName: node
   linkType: hard
 
 "minizlib@npm:^2.1.1, minizlib@npm:^2.1.2":
@@ -7728,30 +7825,30 @@
     encoding:
       optional: true
   checksum: d76d2f5edb451a3f05b15115ec89fc6be39de37c6089f1b6368df03b91e1633fd379a7e01b7ab05089a25034b2023d959b47e59759cb38d88341b2459e89d6e5
   languageName: node
   linkType: hard
 
 "node-gyp@npm:latest":
-  version: 10.0.1
-  resolution: "node-gyp@npm:10.0.1"
+  version: 10.1.0
+  resolution: "node-gyp@npm:10.1.0"
   dependencies:
     env-paths: ^2.2.0
     exponential-backoff: ^3.1.1
     glob: ^10.3.10
     graceful-fs: ^4.2.6
     make-fetch-happen: ^13.0.0
     nopt: ^7.0.0
     proc-log: ^3.0.0
     semver: ^7.3.5
     tar: ^6.1.2
     which: ^4.0.0
   bin:
     node-gyp: bin/node-gyp.js
-  checksum: 60a74e66d364903ce02049966303a57f898521d139860ac82744a5fdd9f7b7b3b61f75f284f3bfe6e6add3b8f1871ce305a1d41f775c7482de837b50c792223f
+  checksum: 72e2ab4b23fc32007a763da94018f58069fc0694bf36115d49a2b195c8831e12cf5dd1e7a3718fa85c06969aedf8fc126722d3b672ec1cb27e06ed33caee3c60
   languageName: node
   linkType: hard
 
 "node-int64@npm:^0.4.0":
   version: 0.4.0
   resolution: "node-int64@npm:0.4.0"
   checksum: d0b30b1ee6d961851c60d5eaa745d30b5c95d94bc0e74b81e5292f7c42a49e3af87f1eb9e89f59456f80645d679202537de751b7d72e9e40ceea40c5e449057e
@@ -7834,17 +7931,17 @@
   dependencies:
     path-key: ^3.0.0
   checksum: 5374c0cea4b0bbfdfae62da7bbdf1e1558d338335f4cacf2515c282ff358ff27b2ecb91ffa5330a8b14390ac66a1e146e10700440c1ab868208430f56b5f4d23
   languageName: node
   linkType: hard
 
 "nwsapi@npm:^2.2.2":
-  version: 2.2.7
-  resolution: "nwsapi@npm:2.2.7"
-  checksum: cab25f7983acec7e23490fec3ef7be608041b460504229770e3bfcf9977c41d6fe58f518994d3bd9aa3a101f501089a3d4a63536f4ff8ae4b8c4ca23bdbfda4e
+  version: 2.2.9
+  resolution: "nwsapi@npm:2.2.9"
+  checksum: 3ab2bc47d5507a76e2fdee5aae7ea2875c6def912d0401126cad3e39825a7decb7a02622810c855a7902bd31e917e606b37882dca12b0ae54b4d3b70275de927
   languageName: node
   linkType: hard
 
 "object-assign@npm:^4.1.1":
   version: 4.1.1
   resolution: "object-assign@npm:4.1.1"
   checksum: fcc6e4ea8c7fe48abfbb552578b1c53e0d194086e2e6bbbf59e0a536381a292f39943c6e9628af05b5528aa5e3318bb30d6b2e53cadaf5b8fe9e12c4b69af23f
@@ -7861,15 +7958,15 @@
 "object-keys@npm:^1.1.1":
   version: 1.1.1
   resolution: "object-keys@npm:1.1.1"
   checksum: b363c5e7644b1e1b04aa507e88dcb8e3a2f52b6ffd0ea801e4c7a62d5aa559affe21c55a07fd4b1fd55fc03a33c610d73426664b20032405d7b92a1414c34d6a
   languageName: node
   linkType: hard
 
-"object.assign@npm:^4.1.4":
+"object.assign@npm:^4.1.5":
   version: 4.1.5
   resolution: "object.assign@npm:4.1.5"
   dependencies:
     call-bind: ^1.0.5
     define-properties: ^1.2.1
     has-symbols: ^1.0.3
     object-keys: ^1.1.1
@@ -7892,24 +7989,24 @@
   dependencies:
     mimic-fn: ^2.1.0
   checksum: 2478859ef817fc5d4e9c2f9e5728512ddd1dbc9fb7829ad263765bb6d3b91ce699d6e2332eef6b7dff183c2f490bd3349f1666427eaba4469fba0ac38dfd0d34
   languageName: node
   linkType: hard
 
 "optionator@npm:^0.9.3":
-  version: 0.9.3
-  resolution: "optionator@npm:0.9.3"
+  version: 0.9.4
+  resolution: "optionator@npm:0.9.4"
   dependencies:
-    "@aashutoshrathi/word-wrap": ^1.2.3
     deep-is: ^0.1.3
     fast-levenshtein: ^2.0.6
     levn: ^0.4.1
     prelude-ls: ^1.2.1
     type-check: ^0.4.0
-  checksum: 09281999441f2fe9c33a5eeab76700795365a061563d66b098923eb719251a42bdbe432790d35064d0816ead9296dbeb1ad51a733edf4167c96bd5d0882e428a
+    word-wrap: ^1.2.5
+  checksum: ecbd010e3dc73e05d239976422d9ef54a82a13f37c11ca5911dff41c98a6c7f0f163b27f922c37e7f8340af9d36febd3b6e9cef508f3339d4c393d7276d716bb
   languageName: node
   linkType: hard
 
 "p-limit@npm:^2.2.0":
   version: 2.3.0
   resolution: "p-limit@npm:2.3.0"
   dependencies:
@@ -8046,21 +8143,21 @@
 "path-parse@npm:^1.0.7":
   version: 1.0.7
   resolution: "path-parse@npm:1.0.7"
   checksum: 49abf3d81115642938a8700ec580da6e830dde670be21893c62f4e10bd7dd4c3742ddc603fe24f898cba7eb0c6bc1777f8d9ac14185d34540c6d4d80cd9cae8a
   languageName: node
   linkType: hard
 
-"path-scurry@npm:^1.10.1, path-scurry@npm:^1.6.1":
-  version: 1.10.1
-  resolution: "path-scurry@npm:1.10.1"
+"path-scurry@npm:^1.10.2, path-scurry@npm:^1.6.1":
+  version: 1.10.2
+  resolution: "path-scurry@npm:1.10.2"
   dependencies:
-    lru-cache: ^9.1.1 || ^10.0.0
+    lru-cache: ^10.2.0
     minipass: ^5.0.0 || ^6.0.2 || ^7.0.0
-  checksum: e2557cff3a8fb8bc07afdd6ab163a92587884f9969b05bbbaf6fe7379348bfb09af9ed292af12ed32398b15fb443e81692047b786d1eeb6d898a51eb17ed7d90
+  checksum: 6739b4290f7d1a949c61c758b481c07ac7d1a841964c68cf5e1fa153d7e18cbde4872b37aadf9c5173c800d627f219c47945859159de36c977dd82419997b9b8
   languageName: node
   linkType: hard
 
 "path-type@npm:^3.0.0":
   version: 3.0.0
   resolution: "path-type@npm:3.0.0"
   dependencies:
@@ -8118,51 +8215,58 @@
   resolution: "pkg-dir@npm:4.2.0"
   dependencies:
     find-up: ^4.0.0
   checksum: 9863e3f35132bf99ae1636d31ff1e1e3501251d480336edb1c211133c8d58906bed80f154a1d723652df1fda91e01c7442c2eeaf9dc83157c7ae89087e43c8d6
   languageName: node
   linkType: hard
 
+"possible-typed-array-names@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "possible-typed-array-names@npm:1.0.0"
+  checksum: b32d403ece71e042385cc7856385cecf1cd8e144fa74d2f1de40d1e16035dba097bc189715925e79b67bdd1472796ff168d3a90d296356c9c94d272d5b95f3ae
+  languageName: node
+  linkType: hard
+
 "postcss-media-query-parser@npm:^0.2.3":
   version: 0.2.3
   resolution: "postcss-media-query-parser@npm:0.2.3"
   checksum: 8000d4d95b912994928ff86137f5ab0ed4c4ee1498af2336e93d708ae8827a690cd7acbaed55d14684cf44d82c8d44b031c1c69ae6bcd2f9620ea67573888090
   languageName: node
   linkType: hard
 
-"postcss-modules-extract-imports@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "postcss-modules-extract-imports@npm:3.0.0"
+"postcss-modules-extract-imports@npm:^3.1.0":
+  version: 3.1.0
+  resolution: "postcss-modules-extract-imports@npm:3.1.0"
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 4b65f2f1382d89c4bc3c0a1bdc5942f52f3cb19c110c57bd591ffab3a5fee03fcf831604168205b0c1b631a3dce2255c70b61aaae3ef39d69cd7eb450c2552d2
+  checksum: b9192e0f4fb3d19431558be6f8af7ca45fc92baaad9b2778d1732a5880cd25c3df2074ce5484ae491e224f0d21345ffc2d419bd51c25b019af76d7a7af88c17f
   languageName: node
   linkType: hard
 
-"postcss-modules-local-by-default@npm:^4.0.4":
-  version: 4.0.4
-  resolution: "postcss-modules-local-by-default@npm:4.0.4"
+"postcss-modules-local-by-default@npm:^4.0.5":
+  version: 4.0.5
+  resolution: "postcss-modules-local-by-default@npm:4.0.5"
   dependencies:
     icss-utils: ^5.0.0
     postcss-selector-parser: ^6.0.2
     postcss-value-parser: ^4.1.0
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 578b955b0773147890caa88c30b10dfc849c5b1412a47ad51751890dba16fca9528c3ab00a19b186a8c2c150c2d08e2ce64d3d907800afee1f37c6d38252e365
+  checksum: ca9b01f4a0a3dfb33e016299e2dfb7e85c3123292f7aec2efc0c6771b9955648598bfb4c1561f7ee9732fb27fb073681233661b32eef98baab43743f96735452
   languageName: node
   linkType: hard
 
-"postcss-modules-scope@npm:^3.1.1":
-  version: 3.1.1
-  resolution: "postcss-modules-scope@npm:3.1.1"
+"postcss-modules-scope@npm:^3.2.0":
+  version: 3.2.0
+  resolution: "postcss-modules-scope@npm:3.2.0"
   dependencies:
     postcss-selector-parser: ^6.0.4
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 9e9d23abb0babc7fa243be65704d72a5a9ceb2bded4dbaef96a88210d468b03c8c3158c197f4e22300c851f08c6fdddd6ebe65f44e4c34448b45b8a2e063a16d
+  checksum: 2ffe7e98c1fa993192a39c8dd8ade93fc4f59fbd1336ce34fcedaee0ee3bafb29e2e23fb49189256895b30e4f21af661c6a6a16ef7b17ae2c859301e4a4459ae
   languageName: node
   linkType: hard
 
 "postcss-modules-values@npm:^4.0.0":
   version: 4.0.0
   resolution: "postcss-modules-values@npm:4.0.0"
   dependencies:
@@ -8186,38 +8290,38 @@
   peerDependencies:
     postcss: ^8.3.3
   checksum: 06c733eaad83a3954367e7ee02ddfe3796e7a44d4299ccf9239f40964a4daac153c7d77613f32964b5a86c0c6c2f6167738f31d578b73b17cb69d0c4446f0ebe
   languageName: node
   linkType: hard
 
 "postcss-selector-parser@npm:^6.0.11, postcss-selector-parser@npm:^6.0.2, postcss-selector-parser@npm:^6.0.4":
-  version: 6.0.15
-  resolution: "postcss-selector-parser@npm:6.0.15"
+  version: 6.0.16
+  resolution: "postcss-selector-parser@npm:6.0.16"
   dependencies:
     cssesc: ^3.0.0
     util-deprecate: ^1.0.2
-  checksum: 57decb94152111004f15e27b9c61131eb50ee10a3288e7fcf424cebbb4aba82c2817517ae718f8b5d704ee9e02a638d4a2acff8f47685c295a33ecee4fd31055
+  checksum: e1cd68e33a39e3dc1e1e5bd8717be5bbe3cc23a4cecb466c3acb2f3a77daad7a47df4d6137a76f8db74cf160d2fb16b2cfdb4ccbebdfda844690f8d545fe281d
   languageName: node
   linkType: hard
 
 "postcss-value-parser@npm:^4.1.0, postcss-value-parser@npm:^4.2.0":
   version: 4.2.0
   resolution: "postcss-value-parser@npm:4.2.0"
   checksum: 819ffab0c9d51cf0acbabf8996dffbfafbafa57afc0e4c98db88b67f2094cb44488758f06e5da95d7036f19556a4a732525e84289a425f4f6fd8e412a9d7442f
   languageName: node
   linkType: hard
 
 "postcss@npm:^8.3.11, postcss@npm:^8.4.19, postcss@npm:^8.4.33":
-  version: 8.4.35
-  resolution: "postcss@npm:8.4.35"
+  version: 8.4.38
+  resolution: "postcss@npm:8.4.38"
   dependencies:
     nanoid: ^3.3.7
     picocolors: ^1.0.0
-    source-map-js: ^1.0.2
-  checksum: cf3c3124d3912a507603f6d9a49b3783f741075e9aa73eb592a6dd9194f9edab9d20a8875d16d137d4f779fe7b6fbd1f5727e39bfd1c3003724980ee4995e1da
+    source-map-js: ^1.2.0
+  checksum: 649f9e60a763ca4b5a7bbec446a069edf07f057f6d780a5a0070576b841538d1ecf7dd888f2fbfd1f76200e26c969e405aeeae66332e6927dbdc8bdcb90b9451
   languageName: node
   linkType: hard
 
 "prelude-ls@npm:^1.2.1":
   version: 1.2.1
   resolution: "prelude-ls@npm:1.2.1"
   checksum: cd192ec0d0a8e4c6da3bb80e4f62afe336df3f76271ac6deb0e6a36187133b6073a19e9727a1ff108cd8b9982e4768850d413baa71214dd80c7979617dca827a
@@ -8309,17 +8413,17 @@
   version: 2.3.1
   resolution: "punycode@npm:2.3.1"
   checksum: bb0a0ceedca4c3c57a9b981b90601579058903c62be23c5e8e843d2c2d4148a3ecf029d5133486fb0e1822b098ba8bba09e89d6b21742d02fa26bda6441a6fb2
   languageName: node
   linkType: hard
 
 "pure-rand@npm:^6.0.0":
-  version: 6.0.4
-  resolution: "pure-rand@npm:6.0.4"
-  checksum: e1c4e69f8bf7303e5252756d67c3c7551385cd34d94a1f511fe099727ccbab74c898c03a06d4c4a24a89b51858781057b83ebbfe740d984240cdc04fead36068
+  version: 6.1.0
+  resolution: "pure-rand@npm:6.1.0"
+  checksum: 8d53bc02bed99eca0b65b505090152ee7e9bd67dd74f8ff32ba1c883b87234067c5bf68d2614759fb217d82594d7a92919e6df80f97885e7b12b42af4bd3316a
   languageName: node
   linkType: hard
 
 "querystringify@npm:^2.1.1":
   version: 2.2.0
   resolution: "querystringify@npm:2.2.0"
   checksum: 5641ea231bad7ef6d64d9998faca95611ed4b11c2591a8cae741e178a974f6a8e0ebde008475259abe1621cb15e692404e6b6626e927f7b849d5c09392604b15
@@ -8346,45 +8450,45 @@
   dependencies:
     safe-buffer: ^5.1.0
   checksum: d779499376bd4cbb435ef3ab9a957006c8682f343f14089ed5f27764e4645114196e75b7f6abf1cbd84fd247c0cb0651698444df8c9bf30e62120fbbc52269d6
   languageName: node
   linkType: hard
 
 "react-dom@npm:^18.2.0":
-  version: 18.2.0
-  resolution: "react-dom@npm:18.2.0"
+  version: 18.3.1
+  resolution: "react-dom@npm:18.3.1"
   dependencies:
     loose-envify: ^1.1.0
-    scheduler: ^0.23.0
+    scheduler: ^0.23.2
   peerDependencies:
-    react: ^18.2.0
-  checksum: 7d323310bea3a91be2965f9468d552f201b1c27891e45ddc2d6b8f717680c95a75ae0bc1e3f5cf41472446a2589a75aed4483aee8169287909fcd59ad149e8cc
+    react: ^18.3.1
+  checksum: 298954ecd8f78288dcaece05e88b570014d8f6dce5db6f66e6ee91448debeb59dcd31561dddb354eee47e6c1bb234669459060deb238ed0213497146e555a0b9
   languageName: node
   linkType: hard
 
 "react-is@npm:^16.13.1":
   version: 16.13.1
   resolution: "react-is@npm:16.13.1"
   checksum: f7a19ac3496de32ca9ae12aa030f00f14a3d45374f1ceca0af707c831b2a6098ef0d6bdae51bd437b0a306d7f01d4677fcc8de7c0d331eb47ad0f46130e53c5f
   languageName: node
   linkType: hard
 
 "react-is@npm:^18.0.0, react-is@npm:^18.2.0":
-  version: 18.2.0
-  resolution: "react-is@npm:18.2.0"
-  checksum: e72d0ba81b5922759e4aff17e0252bd29988f9642ed817f56b25a3e217e13eea8a7f2322af99a06edb779da12d5d636e9fda473d620df9a3da0df2a74141d53e
+  version: 18.3.1
+  resolution: "react-is@npm:18.3.1"
+  checksum: e20fe84c86ff172fc8d898251b7cc2c43645d108bf96d0b8edf39b98f9a2cae97b40520ee7ed8ee0085ccc94736c4886294456033304151c3f94978cec03df21
   languageName: node
   linkType: hard
 
 "react@npm:>=17.0.0 <19.0.0, react@npm:^18.2.0":
-  version: 18.2.0
-  resolution: "react@npm:18.2.0"
+  version: 18.3.1
+  resolution: "react@npm:18.3.1"
   dependencies:
     loose-envify: ^1.1.0
-  checksum: 88e38092da8839b830cda6feef2e8505dec8ace60579e46aa5490fc3dc9bba0bd50336507dc166f43e3afc1c42939c09fe33b25fae889d6f402721dcd78fca1b
+  checksum: a27bcfa8ff7c15a1e50244ad0d0c1cb2ad4375eeffefd266a64889beea6f6b64c4966c9b37d14ee32d6c9fcd5aa6ba183b6988167ab4d127d13e7cb5b386a376
   languageName: node
   linkType: hard
 
 "read-pkg-up@npm:^7.0.1":
   version: 7.0.1
   resolution: "read-pkg-up@npm:7.0.1"
   dependencies:
@@ -8465,22 +8569,23 @@
   resolution: "regenerator-transform@npm:0.15.2"
   dependencies:
     "@babel/runtime": ^7.8.4
   checksum: 20b6f9377d65954980fe044cfdd160de98df415b4bff38fbade67b3337efaf078308c4fed943067cd759827cc8cfeca9cb28ccda1f08333b85d6a2acbd022c27
   languageName: node
   linkType: hard
 
-"regexp.prototype.flags@npm:^1.5.1":
-  version: 1.5.1
-  resolution: "regexp.prototype.flags@npm:1.5.1"
+"regexp.prototype.flags@npm:^1.5.2":
+  version: 1.5.2
+  resolution: "regexp.prototype.flags@npm:1.5.2"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.2.0
-    set-function-name: ^2.0.0
-  checksum: 869edff00288442f8d7fa4c9327f91d85f3b3acf8cbbef9ea7a220345cf23e9241b6def9263d2c1ebcf3a316b0aa52ad26a43a84aa02baca3381717b3e307f47
+    call-bind: ^1.0.6
+    define-properties: ^1.2.1
+    es-errors: ^1.3.0
+    set-function-name: ^2.0.1
+  checksum: d7f333667d5c564e2d7a97c56c3075d64c722c9bb51b2b4df6822b2e8096d623a5e63088fb4c83df919b6951ef8113841de8b47de7224872fa6838bc5d8a7d64
   languageName: node
   linkType: hard
 
 "regexpu-core@npm:^5.3.1":
   version: 5.3.2
   resolution: "regexpu-core@npm:5.3.2"
   dependencies:
@@ -8623,34 +8728,34 @@
   resolution: "run-parallel@npm:1.2.0"
   dependencies:
     queue-microtask: ^1.2.2
   checksum: cb4f97ad25a75ebc11a8ef4e33bb962f8af8516bb2001082ceabd8902e15b98f4b84b4f8a9b222e5d57fc3bd1379c483886ed4619367a7680dad65316993021d
   languageName: node
   linkType: hard
 
-"safe-array-concat@npm:^1.0.1":
-  version: 1.1.0
-  resolution: "safe-array-concat@npm:1.1.0"
+"safe-array-concat@npm:^1.1.2":
+  version: 1.1.2
+  resolution: "safe-array-concat@npm:1.1.2"
   dependencies:
-    call-bind: ^1.0.5
-    get-intrinsic: ^1.2.2
+    call-bind: ^1.0.7
+    get-intrinsic: ^1.2.4
     has-symbols: ^1.0.3
     isarray: ^2.0.5
-  checksum: 5c71eaa999168ee7474929f1cd3aae80f486353a651a094d9968936692cf90aa065224929a6486dcda66334a27dce4250a83612f9e0fef6dced1a925d3ac7296
+  checksum: a3b259694754ddfb73ae0663829e396977b99ff21cbe8607f35a469655656da8e271753497e59da8a7575baa94d2e684bea3e10ddd74ba046c0c9b4418ffa0c4
   languageName: node
   linkType: hard
 
 "safe-buffer@npm:^5.1.0":
   version: 5.2.1
   resolution: "safe-buffer@npm:5.2.1"
   checksum: b99c4b41fdd67a6aaf280fcd05e9ffb0813654894223afb78a31f14a19ad220bba8aba1cb14eddce1fcfb037155fe6de4e861784eb434f7d11ed58d1e70dd491
   languageName: node
   linkType: hard
 
-"safe-regex-test@npm:^1.0.0":
+"safe-regex-test@npm:^1.0.3":
   version: 1.0.3
   resolution: "safe-regex-test@npm:1.0.3"
   dependencies:
     call-bind: ^1.0.6
     es-errors: ^1.3.0
     is-regex: ^1.1.4
   checksum: 6c7d392ff1ae7a3ae85273450ed02d1d131f1d2c76e177d6b03eb88e6df8fa062639070e7d311802c1615f351f18dc58f9454501c58e28d5ffd9b8f502ba6489
@@ -8683,20 +8788,20 @@
   resolution: "saxes@npm:6.0.0"
   dependencies:
     xmlchars: ^2.2.0
   checksum: d3fa3e2aaf6c65ed52ee993aff1891fc47d5e47d515164b5449cbf5da2cbdc396137e55590472e64c5c436c14ae64a8a03c29b9e7389fc6f14035cf4e982ef3b
   languageName: node
   linkType: hard
 
-"scheduler@npm:^0.23.0":
-  version: 0.23.0
-  resolution: "scheduler@npm:0.23.0"
+"scheduler@npm:^0.23.2":
+  version: 0.23.2
+  resolution: "scheduler@npm:0.23.2"
   dependencies:
     loose-envify: ^1.1.0
-  checksum: d79192eeaa12abef860c195ea45d37cbf2bbf5f66e3c4dcd16f54a7da53b17788a70d109ee3d3dde1a0fd50e6a8fc171f4300356c5aee4fc0171de526bf35f8a
+  checksum: 3e82d1f419e240ef6219d794ff29c7ee415fbdc19e038f680a10c067108e06284f1847450a210b29bbaf97b9d8a97ced5f624c31c681248ac84c80d56ad5a2c4
   languageName: node
   linkType: hard
 
 "schema-utils@npm:^2.7.0":
   version: 2.7.1
   resolution: "schema-utils@npm:2.7.1"
   dependencies:
@@ -8764,36 +8869,37 @@
   resolution: "serialize-javascript@npm:6.0.2"
   dependencies:
     randombytes: ^2.1.0
   checksum: c4839c6206c1d143c0f80763997a361310305751171dd95e4b57efee69b8f6edd8960a0b7fbfc45042aadff98b206d55428aee0dc276efe54f100899c7fa8ab7
   languageName: node
   linkType: hard
 
-"set-function-length@npm:^1.2.0":
-  version: 1.2.1
-  resolution: "set-function-length@npm:1.2.1"
+"set-function-length@npm:^1.2.1":
+  version: 1.2.2
+  resolution: "set-function-length@npm:1.2.2"
   dependencies:
-    define-data-property: ^1.1.2
+    define-data-property: ^1.1.4
     es-errors: ^1.3.0
     function-bind: ^1.1.2
-    get-intrinsic: ^1.2.3
+    get-intrinsic: ^1.2.4
     gopd: ^1.0.1
-    has-property-descriptors: ^1.0.1
-  checksum: 23742476d695f2eae86348c069bd164d4f25fa7c26546a46a2b5f370f1f84b98ec64366d2cd17785d5b41bbf16b95855da4b7eb188e7056fe3b0248d61f6afda
+    has-property-descriptors: ^1.0.2
+  checksum: a8248bdacdf84cb0fab4637774d9fb3c7a8e6089866d04c817583ff48e14149c87044ce683d7f50759a8c50fb87c7a7e173535b06169c87ef76f5fb276dfff72
   languageName: node
   linkType: hard
 
-"set-function-name@npm:^2.0.0":
-  version: 2.0.1
-  resolution: "set-function-name@npm:2.0.1"
+"set-function-name@npm:^2.0.1":
+  version: 2.0.2
+  resolution: "set-function-name@npm:2.0.2"
   dependencies:
-    define-data-property: ^1.0.1
+    define-data-property: ^1.1.4
+    es-errors: ^1.3.0
     functions-have-names: ^1.2.3
-    has-property-descriptors: ^1.0.0
-  checksum: 4975d17d90c40168eee2c7c9c59d023429f0a1690a89d75656306481ece0c3c1fb1ebcc0150ea546d1913e35fbd037bace91372c69e543e51fc5d1f31a9fa126
+    has-property-descriptors: ^1.0.2
+  checksum: d6229a71527fd0404399fc6227e0ff0652800362510822a291925c9d7b48a1ca1a468b11b281471c34cd5a2da0db4f5d7ff315a61d26655e77f6e971e6d0c80f
   languageName: node
   linkType: hard
 
 "shallow-clone@npm:^3.0.0":
   version: 3.0.1
   resolution: "shallow-clone@npm:3.0.1"
   dependencies:
@@ -8838,22 +8944,22 @@
   version: 1.8.1
   resolution: "shell-quote@npm:1.8.1"
   checksum: 5f01201f4ef504d4c6a9d0d283fa17075f6770bfbe4c5850b074974c68062f37929ca61700d95ad2ac8822e14e8c4b990ca0e6e9272e64befd74ce5e19f0736b
   languageName: node
   linkType: hard
 
 "side-channel@npm:^1.0.4":
-  version: 1.0.5
-  resolution: "side-channel@npm:1.0.5"
+  version: 1.0.6
+  resolution: "side-channel@npm:1.0.6"
   dependencies:
-    call-bind: ^1.0.6
+    call-bind: ^1.0.7
     es-errors: ^1.3.0
     get-intrinsic: ^1.2.4
     object-inspect: ^1.13.1
-  checksum: 640446b4e5a9554116ed6f5bec17c6740fa8da2c1a19e4d69c1202191185d4cc24f21ba0dd3ccca140eb6a8ee978d0b5bc5132f09b7962db7f9c4bc7872494ac
+  checksum: bfc1afc1827d712271453e91b7cd3878ac0efd767495fd4e594c4c2afaa7963b7b510e249572bfd54b0527e66e4a12b61b80c061389e129755f34c493aad9b97
   languageName: node
   linkType: hard
 
 "signal-exit@npm:^3.0.3, signal-exit@npm:^3.0.7":
   version: 3.0.7
   resolution: "signal-exit@npm:3.0.7"
   checksum: a2f098f247adc367dffc27845853e9959b9e88b01cb301658cfe4194352d8d2bb32e18467c786a7fe15f1d44b233ea35633d076d5e737870b7139949d1ab6318
@@ -8904,46 +9010,46 @@
 "smart-buffer@npm:^4.2.0":
   version: 4.2.0
   resolution: "smart-buffer@npm:4.2.0"
   checksum: b5167a7142c1da704c0e3af85c402002b597081dd9575031a90b4f229ca5678e9a36e8a374f1814c8156a725d17008ae3bde63b92f9cfd132526379e580bec8b
   languageName: node
   linkType: hard
 
-"socks-proxy-agent@npm:^8.0.1":
-  version: 8.0.2
-  resolution: "socks-proxy-agent@npm:8.0.2"
+"socks-proxy-agent@npm:^8.0.3":
+  version: 8.0.3
+  resolution: "socks-proxy-agent@npm:8.0.3"
   dependencies:
-    agent-base: ^7.0.2
+    agent-base: ^7.1.1
     debug: ^4.3.4
     socks: ^2.7.1
-  checksum: 4fb165df08f1f380881dcd887b3cdfdc1aba3797c76c1e9f51d29048be6e494c5b06d68e7aea2e23df4572428f27a3ec22b3d7c75c570c5346507433899a4b6d
+  checksum: 8fab38821c327c190c28f1658087bc520eb065d55bc07b4a0fdf8d1e0e7ad5d115abbb22a95f94f944723ea969dd771ad6416b1e3cde9060c4c71f705c8b85c5
   languageName: node
   linkType: hard
 
 "socks@npm:^2.7.1":
-  version: 2.7.1
-  resolution: "socks@npm:2.7.1"
+  version: 2.8.3
+  resolution: "socks@npm:2.8.3"
   dependencies:
-    ip: ^2.0.0
+    ip-address: ^9.0.5
     smart-buffer: ^4.2.0
-  checksum: 259d9e3e8e1c9809a7f5c32238c3d4d2a36b39b83851d0f573bfde5f21c4b1288417ce1af06af1452569cd1eb0841169afd4998f0e04ba04656f6b7f0e46d748
+  checksum: 7a6b7f6eedf7482b9e4597d9a20e09505824208006ea8f2c49b71657427f3c137ca2ae662089baa73e1971c62322d535d9d0cf1c9235cf6f55e315c18203eadd
   languageName: node
   linkType: hard
 
 "source-list-map@npm:^2.0.0":
   version: 2.0.1
   resolution: "source-list-map@npm:2.0.1"
   checksum: 806efc6f75e7cd31e4815e7a3aaf75a45c704871ea4075cb2eb49882c6fca28998f44fc5ac91adb6de03b2882ee6fb02f951fdc85e6a22b338c32bfe19557938
   languageName: node
   linkType: hard
 
-"source-map-js@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "source-map-js@npm:1.0.2"
-  checksum: c049a7fc4deb9a7e9b481ae3d424cc793cb4845daa690bc5a05d428bf41bf231ced49b4cf0c9e77f9d42fdb3d20d6187619fc586605f5eabe995a316da8d377c
+"source-map-js@npm:^1.2.0":
+  version: 1.2.0
+  resolution: "source-map-js@npm:1.2.0"
+  checksum: 791a43306d9223792e84293b00458bf102a8946e7188f3db0e4e22d8d530b5f80a4ce468eb5ec0bf585443ad55ebbd630bf379c98db0b1f317fd902500217f97
   languageName: node
   linkType: hard
 
 "source-map-loader@npm:^1.0.2":
   version: 1.1.3
   resolution: "source-map-loader@npm:1.1.3"
   dependencies:
@@ -9008,34 +9114,41 @@
     spdx-expression-parse: ^3.0.0
     spdx-license-ids: ^3.0.0
   checksum: e9ae98d22f69c88e7aff5b8778dc01c361ef635580e82d29e5c60a6533cc8f4d820803e67d7432581af0cc4fb49973125076ee3b90df191d153e223c004193b2
   languageName: node
   linkType: hard
 
 "spdx-exceptions@npm:^2.1.0":
-  version: 2.4.0
-  resolution: "spdx-exceptions@npm:2.4.0"
-  checksum: b1b650a8d94424473bf9629cf972c86a91c03cccc260f5c901bce0e4b92d831627fec28c9e0a1e9c34c5ebad0a12cf2eab887bec088e0a862abb9d720c2fd0a1
+  version: 2.5.0
+  resolution: "spdx-exceptions@npm:2.5.0"
+  checksum: bb127d6e2532de65b912f7c99fc66097cdea7d64c10d3ec9b5e96524dbbd7d20e01cba818a6ddb2ae75e62bb0c63d5e277a7e555a85cbc8ab40044984fa4ae15
   languageName: node
   linkType: hard
 
 "spdx-expression-parse@npm:^3.0.0":
   version: 3.0.1
   resolution: "spdx-expression-parse@npm:3.0.1"
   dependencies:
     spdx-exceptions: ^2.1.0
     spdx-license-ids: ^3.0.0
   checksum: a1c6e104a2cbada7a593eaa9f430bd5e148ef5290d4c0409899855ce8b1c39652bcc88a725259491a82601159d6dc790bedefc9016c7472f7de8de7361f8ccde
   languageName: node
   linkType: hard
 
 "spdx-license-ids@npm:^3.0.0":
-  version: 3.0.16
-  resolution: "spdx-license-ids@npm:3.0.16"
-  checksum: 5cdaa85aaa24bd02f9353a2e357b4df0a4f205cb35655f3fd0a5674a4fb77081f28ffd425379214bc3be2c2b7593ce1215df6bcc75884aeee0a9811207feabe2
+  version: 3.0.17
+  resolution: "spdx-license-ids@npm:3.0.17"
+  checksum: 0aba5d16292ff604dd20982200e23b4d425f6ba364765039bdbde2f6c956b9909fce1ad040a897916a5f87388e85e001f90cb64bf706b6e319f3908cfc445a59
+  languageName: node
+  linkType: hard
+
+"sprintf-js@npm:^1.1.3":
+  version: 1.1.3
+  resolution: "sprintf-js@npm:1.1.3"
+  checksum: a3fdac7b49643875b70864a9d9b469d87a40dfeaf5d34d9d0c5b1cda5fd7d065531fcb43c76357d62254c57184a7b151954156563a4d6a747015cfb41021cad0
   languageName: node
   linkType: hard
 
 "sprintf-js@npm:~1.0.2":
   version: 1.0.3
   resolution: "sprintf-js@npm:1.0.3"
   checksum: 19d79aec211f09b99ec3099b5b2ae2f6e9cdefe50bc91ac4c69144b6d3928a640bb6ae5b3def70c2e85a2c3d9f5ec2719921e3a59d3ca3ef4b2fd1a4656a0df3
@@ -9089,54 +9202,56 @@
     emoji-regex: ^9.2.2
     strip-ansi: ^7.0.1
   checksum: 7369deaa29f21dda9a438686154b62c2c5f661f8dda60449088f9f980196f7908fc39fdd1803e3e01541970287cf5deae336798337e9319a7055af89dafa7193
   languageName: node
   linkType: hard
 
 "string.prototype.padend@npm:^3.0.0":
-  version: 3.1.5
-  resolution: "string.prototype.padend@npm:3.1.5"
+  version: 3.1.6
+  resolution: "string.prototype.padend@npm:3.1.6"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.2.0
-    es-abstract: ^1.22.1
-  checksum: fc915e0b6ae1dce07a9f5088429d84fda2c1c0ac9a05bc14a602f173cc2fdef32e4893dfba5656f8f955450c9c16deebdb8d303d27613a367bc6d8508a94cd5e
+    call-bind: ^1.0.7
+    define-properties: ^1.2.1
+    es-abstract: ^1.23.2
+    es-object-atoms: ^1.0.0
+  checksum: d9fc23c21bdfb6850756002ef09cebc420882003f29eafbd8322df77a90726bc2a64892d01f94f1fc9fc6f809414fbcbd8615610bb3cddd33512c12b6b3643a2
   languageName: node
   linkType: hard
 
-"string.prototype.trim@npm:^1.2.8":
-  version: 1.2.8
-  resolution: "string.prototype.trim@npm:1.2.8"
+"string.prototype.trim@npm:^1.2.9":
+  version: 1.2.9
+  resolution: "string.prototype.trim@npm:1.2.9"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.2.0
-    es-abstract: ^1.22.1
-  checksum: 49eb1a862a53aba73c3fb6c2a53f5463173cb1f4512374b623bcd6b43ad49dd559a06fb5789bdec771a40fc4d2a564411c0a75d35fb27e76bbe738c211ecff07
+    call-bind: ^1.0.7
+    define-properties: ^1.2.1
+    es-abstract: ^1.23.0
+    es-object-atoms: ^1.0.0
+  checksum: ea2df6ec1e914c9d4e2dc856fa08228e8b1be59b59e50b17578c94a66a176888f417264bb763d4aac638ad3b3dad56e7a03d9317086a178078d131aa293ba193
   languageName: node
   linkType: hard
 
-"string.prototype.trimend@npm:^1.0.7":
-  version: 1.0.7
-  resolution: "string.prototype.trimend@npm:1.0.7"
+"string.prototype.trimend@npm:^1.0.8":
+  version: 1.0.8
+  resolution: "string.prototype.trimend@npm:1.0.8"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.2.0
-    es-abstract: ^1.22.1
-  checksum: 2375516272fd1ba75992f4c4aa88a7b5f3c7a9ca308d963bcd5645adf689eba6f8a04ebab80c33e30ec0aefc6554181a3a8416015c38da0aa118e60ec896310c
+    call-bind: ^1.0.7
+    define-properties: ^1.2.1
+    es-object-atoms: ^1.0.0
+  checksum: cc3bd2de08d8968a28787deba9a3cb3f17ca5f9f770c91e7e8fa3e7d47f079bad70fadce16f05dda9f261788be2c6e84a942f618c3bed31e42abc5c1084f8dfd
   languageName: node
   linkType: hard
 
-"string.prototype.trimstart@npm:^1.0.7":
-  version: 1.0.7
-  resolution: "string.prototype.trimstart@npm:1.0.7"
+"string.prototype.trimstart@npm:^1.0.8":
+  version: 1.0.8
+  resolution: "string.prototype.trimstart@npm:1.0.8"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.2.0
-    es-abstract: ^1.22.1
-  checksum: 13d0c2cb0d5ff9e926fa0bec559158b062eed2b68cd5be777ffba782c96b2b492944e47057274e064549b94dd27cf81f48b27a31fee8af5b574cff253e7eb613
+    call-bind: ^1.0.7
+    define-properties: ^1.2.1
+    es-object-atoms: ^1.0.0
+  checksum: df1007a7f580a49d692375d996521dc14fd103acda7f3034b3c558a60b82beeed3a64fa91e494e164581793a8ab0ae2f59578a49896a7af6583c1f20472bce96
   languageName: node
   linkType: hard
 
 "strip-ansi-cjs@npm:strip-ansi@^6.0.1, strip-ansi@npm:^6.0.0, strip-ansi@npm:^6.0.1":
   version: 6.0.1
   resolution: "strip-ansi@npm:6.0.1"
   dependencies:
@@ -9197,17 +9312,17 @@
   peerDependencies:
     webpack: ^5.0.0
   checksum: caac3f2fe2c3c89e49b7a2a9329e1cfa515ecf5f36b9c4885f9b218019fda207a9029939b2c35821dec177a264a007e7c391ccdd3ff7401881ce6287b9c8f38b
   languageName: node
   linkType: hard
 
 "style-mod@npm:^4.0.0, style-mod@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "style-mod@npm:4.1.0"
-  checksum: 8402b14ca11113a3640d46b3cf7ba49f05452df7846bc5185a3535d9b6a64a3019e7fb636b59ccbb7816aeb0725b24723e77a85b05612a9360e419958e13b4e6
+  version: 4.1.2
+  resolution: "style-mod@npm:4.1.2"
+  checksum: 7c5c3e82747f9bcf5f288d8d07f50848e4630fe5ff7bfe4d94cc87d6b6a2588227cbf21b4c792ac6406e5852293300a75e710714479a5c59a06af677f0825ef8
   languageName: node
   linkType: hard
 
 "style-search@npm:^0.1.0":
   version: 0.1.0
   resolution: "style-search@npm:0.1.0"
   checksum: 3cfefe335033aad6d47da0725cb48f5db91a73935954c77eab77d9e415e6668cdb406da4a4f7ef9f1aca77853cf5ba7952c45e869caa5bd6439691d88098d468
@@ -9368,44 +9483,44 @@
   version: 5.3.3
   resolution: "tabbable@npm:5.3.3"
   checksum: 1aa56e1bb617cc10616c407f4e756f0607f3e2d30f9803664d70b85db037ca27e75918ed1c71443f3dc902e21dc9f991ce4b52d63a538c9b69b3218d3babcd70
   languageName: node
   linkType: hard
 
 "table@npm:^6.8.1":
-  version: 6.8.1
-  resolution: "table@npm:6.8.1"
+  version: 6.8.2
+  resolution: "table@npm:6.8.2"
   dependencies:
     ajv: ^8.0.1
     lodash.truncate: ^4.4.2
     slice-ansi: ^4.0.0
     string-width: ^4.2.3
     strip-ansi: ^6.0.1
-  checksum: 08249c7046125d9d0a944a6e96cfe9ec66908d6b8a9db125531be6eb05fa0de047fd5542e9d43b4f987057f00a093b276b8d3e19af162a9c40db2681058fd306
+  checksum: 61188652f53a980d1759ca460ca8dea5c5322aece3210457e7084882f053c2b6a870041295e08a82cb1d676e31b056406845d94b0abf3c79a4b104777bec413b
   languageName: node
   linkType: hard
 
 "tapable@npm:^2.1.1, tapable@npm:^2.2.0, tapable@npm:^2.2.1":
   version: 2.2.1
   resolution: "tapable@npm:2.2.1"
   checksum: 3b7a1b4d86fa940aad46d9e73d1e8739335efd4c48322cb37d073eb6f80f5281889bf0320c6d8ffcfa1a0dd5bfdbd0f9d037e252ef972aca595330538aac4d51
   languageName: node
   linkType: hard
 
 "tar@npm:^6.1.11, tar@npm:^6.1.2":
-  version: 6.2.0
-  resolution: "tar@npm:6.2.0"
+  version: 6.2.1
+  resolution: "tar@npm:6.2.1"
   dependencies:
     chownr: ^2.0.0
     fs-minipass: ^2.0.0
     minipass: ^5.0.0
     minizlib: ^2.1.1
     mkdirp: ^1.0.3
     yallist: ^4.0.0
-  checksum: db4d9fe74a2082c3a5016630092c54c8375ff3b280186938cfd104f2e089c4fd9bad58688ef6be9cf186a889671bf355c7cda38f09bbf60604b281715ca57f5c
+  checksum: f1322768c9741a25356c11373bce918483f40fa9a25c69c59410c8a1247632487edef5fe76c5f12ac51a6356d2f1829e96d2bc34098668a2fc34d76050ac2b6c
   languageName: node
   linkType: hard
 
 "terser-webpack-plugin@npm:^5.3.10, terser-webpack-plugin@npm:^5.3.7":
   version: 5.3.10
   resolution: "terser-webpack-plugin@npm:5.3.10"
   dependencies:
@@ -9424,24 +9539,24 @@
     uglify-js:
       optional: true
   checksum: bd6e7596cf815f3353e2a53e79cbdec959a1b0276f5e5d4e63e9d7c3c5bb5306df567729da287d1c7b39d79093e56863c569c42c6c24cc34c76aa313bd2cbcea
   languageName: node
   linkType: hard
 
 "terser@npm:^5.26.0":
-  version: 5.27.0
-  resolution: "terser@npm:5.27.0"
+  version: 5.31.0
+  resolution: "terser@npm:5.31.0"
   dependencies:
     "@jridgewell/source-map": ^0.3.3
     acorn: ^8.8.2
     commander: ^2.20.0
     source-map-support: ~0.5.20
   bin:
     terser: bin/terser
-  checksum: c165052cfea061e8512e9b9ba42a098c2ff6382886ae122b040fd5b6153443070cc2dcb4862269f1669c09c716763e856125a355ff984aa72be525d6fffd8729
+  checksum: 48f14229618866bba8a9464e9d0e7fdcb6b6488b3a6c4690fcf4d48df65bf45959d5ae8c02f1a0b3f3dd035a9ae340b715e1e547645b112dc3963daa3564699a
   languageName: node
   linkType: hard
 
 "test-exclude@npm:^6.0.0":
   version: 6.0.0
   resolution: "test-exclude@npm:6.0.0"
   dependencies:
@@ -9479,22 +9594,22 @@
   dependencies:
     is-number: ^7.0.0
   checksum: f76fa01b3d5be85db6a2a143e24df9f60dd047d151062d0ba3df62953f2f697b16fe5dad9b0ac6191c7efc7b1d9dcaa4b768174b7b29da89d4428e64bc0a20ed
   languageName: node
   linkType: hard
 
 "tough-cookie@npm:^4.1.2":
-  version: 4.1.3
-  resolution: "tough-cookie@npm:4.1.3"
+  version: 4.1.4
+  resolution: "tough-cookie@npm:4.1.4"
   dependencies:
     psl: ^1.1.33
     punycode: ^2.1.1
     universalify: ^0.2.0
     url-parse: ^1.5.3
-  checksum: c9226afff36492a52118432611af083d1d8493a53ff41ec4ea48e5b583aec744b989e4280bcf476c910ec1525a89a4a0f1cae81c08b18fb2ec3a9b3a72b91dcc
+  checksum: 5815059f014c31179a303c673f753f7899a6fce94ac93712c88ea5f3c26e0c042b5f0c7a599a00f8e0feeca4615dba75c3dffc54f3c1a489978aa8205e09307c
   languageName: node
   linkType: hard
 
 "tr46@npm:^2.1.0":
   version: 2.1.0
   resolution: "tr46@npm:2.1.0"
   dependencies:
@@ -9624,58 +9739,63 @@
 "type-fest@npm:^0.8.1":
   version: 0.8.1
   resolution: "type-fest@npm:0.8.1"
   checksum: d61c4b2eba24009033ae4500d7d818a94fd6d1b481a8111612ee141400d5f1db46f199c014766b9fa9b31a6a7374d96fc748c6d688a78a3ce5a33123839becb7
   languageName: node
   linkType: hard
 
-"typed-array-buffer@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "typed-array-buffer@npm:1.0.1"
+"typed-array-buffer@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "typed-array-buffer@npm:1.0.2"
   dependencies:
-    call-bind: ^1.0.6
+    call-bind: ^1.0.7
     es-errors: ^1.3.0
     is-typed-array: ^1.1.13
-  checksum: 1d65e46b2b9b7ec2a30df39b9ddf32e55ad08d6119aec33975506a3dba56057796bdc3c64dbeb7fdb61bf340a75e279dfd55b48ce8f3b874f01731e1da6833d2
+  checksum: 02ffc185d29c6df07968272b15d5319a1610817916ec8d4cd670ded5d1efe72901541ff2202fcc622730d8a549c76e198a2f74e312eabbfb712ed907d45cbb0b
   languageName: node
   linkType: hard
 
-"typed-array-byte-length@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "typed-array-byte-length@npm:1.0.0"
+"typed-array-byte-length@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "typed-array-byte-length@npm:1.0.1"
   dependencies:
-    call-bind: ^1.0.2
+    call-bind: ^1.0.7
     for-each: ^0.3.3
-    has-proto: ^1.0.1
-    is-typed-array: ^1.1.10
-  checksum: b03db16458322b263d87a702ff25388293f1356326c8a678d7515767ef563ef80e1e67ce648b821ec13178dd628eb2afdc19f97001ceae7a31acf674c849af94
+    gopd: ^1.0.1
+    has-proto: ^1.0.3
+    is-typed-array: ^1.1.13
+  checksum: f65e5ecd1cf76b1a2d0d6f631f3ea3cdb5e08da106c6703ffe687d583e49954d570cc80434816d3746e18be889ffe53c58bf3e538081ea4077c26a41055b216d
   languageName: node
   linkType: hard
 
-"typed-array-byte-offset@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "typed-array-byte-offset@npm:1.0.0"
+"typed-array-byte-offset@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "typed-array-byte-offset@npm:1.0.2"
   dependencies:
-    available-typed-arrays: ^1.0.5
-    call-bind: ^1.0.2
+    available-typed-arrays: ^1.0.7
+    call-bind: ^1.0.7
     for-each: ^0.3.3
-    has-proto: ^1.0.1
-    is-typed-array: ^1.1.10
-  checksum: 04f6f02d0e9a948a95fbfe0d5a70b002191fae0b8fe0fe3130a9b2336f043daf7a3dda56a31333c35a067a97e13f539949ab261ca0f3692c41603a46a94e960b
+    gopd: ^1.0.1
+    has-proto: ^1.0.3
+    is-typed-array: ^1.1.13
+  checksum: c8645c8794a621a0adcc142e0e2c57b1823bbfa4d590ad2c76b266aa3823895cf7afb9a893bf6685e18454ab1b0241e1a8d885a2d1340948efa4b56add4b5f67
   languageName: node
   linkType: hard
 
-"typed-array-length@npm:^1.0.4":
-  version: 1.0.4
-  resolution: "typed-array-length@npm:1.0.4"
+"typed-array-length@npm:^1.0.6":
+  version: 1.0.6
+  resolution: "typed-array-length@npm:1.0.6"
   dependencies:
-    call-bind: ^1.0.2
+    call-bind: ^1.0.7
     for-each: ^0.3.3
-    is-typed-array: ^1.1.9
-  checksum: 2228febc93c7feff142b8c96a58d4a0d7623ecde6c7a24b2b98eb3170e99f7c7eff8c114f9b283085cd59dcd2bd43aadf20e25bba4b034a53c5bb292f71f8956
+    gopd: ^1.0.1
+    has-proto: ^1.0.3
+    is-typed-array: ^1.1.13
+    possible-typed-array-names: ^1.0.0
+  checksum: f0315e5b8f0168c29d390ff410ad13e4d511c78e6006df4a104576844812ee447fcc32daab1f3a76c9ef4f64eff808e134528b5b2439de335586b392e9750e5c
   languageName: node
   linkType: hard
 
 "typescript@npm:~5.0.2":
   version: 5.0.4
   resolution: "typescript@npm:5.0.4"
   bin:
@@ -9965,21 +10085,21 @@
   resolution: "walker@npm:1.0.8"
   dependencies:
     makeerror: 1.0.12
   checksum: ad7a257ea1e662e57ef2e018f97b3c02a7240ad5093c392186ce0bcf1f1a60bbadd520d073b9beb921ed99f64f065efb63dfc8eec689a80e569f93c1c5d5e16c
   languageName: node
   linkType: hard
 
-"watchpack@npm:^2.4.0":
-  version: 2.4.0
-  resolution: "watchpack@npm:2.4.0"
+"watchpack@npm:^2.4.1":
+  version: 2.4.1
+  resolution: "watchpack@npm:2.4.1"
   dependencies:
     glob-to-regexp: ^0.4.1
     graceful-fs: ^4.1.2
-  checksum: 23d4bc58634dbe13b86093e01c6a68d8096028b664ab7139d58f0c37d962d549a940e98f2f201cecdabd6f9c340338dc73ef8bf094a2249ef582f35183d1a131
+  checksum: 5b0179348655dcdf19cac7cb4ff923fdc024d630650c0bf6bec8899cf47c60e19d4f810a88dba692ed0e7f684cf0fcffea86efdbf6c35d81f031e328043b7fab
   languageName: node
   linkType: hard
 
 "webidl-conversions@npm:^3.0.0":
   version: 3.0.1
   resolution: "webidl-conversions@npm:3.0.1"
   checksum: c92a0a6ab95314bde9c32e1d0a6dfac83b578f8fa5f21e675bc2706ed6981bc26b7eb7e6a1fab158e5ce4adf9caa4a0aee49a52505d4d13c7be545f15021b17c
@@ -10057,47 +10177,47 @@
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
 "webpack@npm:^5.76.1":
-  version: 5.90.1
-  resolution: "webpack@npm:5.90.1"
+  version: 5.91.0
+  resolution: "webpack@npm:5.91.0"
   dependencies:
     "@types/eslint-scope": ^3.7.3
     "@types/estree": ^1.0.5
-    "@webassemblyjs/ast": ^1.11.5
-    "@webassemblyjs/wasm-edit": ^1.11.5
-    "@webassemblyjs/wasm-parser": ^1.11.5
+    "@webassemblyjs/ast": ^1.12.1
+    "@webassemblyjs/wasm-edit": ^1.12.1
+    "@webassemblyjs/wasm-parser": ^1.12.1
     acorn: ^8.7.1
     acorn-import-assertions: ^1.9.0
     browserslist: ^4.21.10
     chrome-trace-event: ^1.0.2
-    enhanced-resolve: ^5.15.0
+    enhanced-resolve: ^5.16.0
     es-module-lexer: ^1.2.1
     eslint-scope: 5.1.1
     events: ^3.2.0
     glob-to-regexp: ^0.4.1
-    graceful-fs: ^4.2.9
+    graceful-fs: ^4.2.11
     json-parse-even-better-errors: ^2.3.1
     loader-runner: ^4.2.0
     mime-types: ^2.1.27
     neo-async: ^2.6.2
     schema-utils: ^3.2.0
     tapable: ^2.1.1
     terser-webpack-plugin: ^5.3.10
-    watchpack: ^2.4.0
+    watchpack: ^2.4.1
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: a7be844d5720a0c6282fec012e6fa34b1137dff953c5d48bf2ef066a6c27c1dbc92a9b9effc05ee61c9fe269499266db9782073f2d82a589d3c5c966ffc56584
+  checksum: f1073715dbb1ed5c070affef293d800a867708bcbc5aba4d8baee87660e0cf53c55966a6f36fab078d1d6c9567cdcd0a9086bdfb607cab87ea68c6449791b9a3
   languageName: node
   linkType: hard
 
 "whatwg-encoding@npm:^2.0.0":
   version: 2.0.0
   resolution: "whatwg-encoding@npm:2.0.0"
   dependencies:
@@ -10160,24 +10280,24 @@
     is-number-object: ^1.0.4
     is-string: ^1.0.5
     is-symbol: ^1.0.3
   checksum: 53ce774c7379071729533922adcca47220228405e1895f26673bbd71bdf7fb09bee38c1d6399395927c6289476b5ae0629863427fd151491b71c4b6cb04f3a5e
   languageName: node
   linkType: hard
 
-"which-typed-array@npm:^1.1.13, which-typed-array@npm:^1.1.14":
-  version: 1.1.14
-  resolution: "which-typed-array@npm:1.1.14"
+"which-typed-array@npm:^1.1.14, which-typed-array@npm:^1.1.15":
+  version: 1.1.15
+  resolution: "which-typed-array@npm:1.1.15"
   dependencies:
-    available-typed-arrays: ^1.0.6
-    call-bind: ^1.0.5
+    available-typed-arrays: ^1.0.7
+    call-bind: ^1.0.7
     for-each: ^0.3.3
     gopd: ^1.0.1
-    has-tostringtag: ^1.0.1
-  checksum: efe30c143c58630dde8ab96f9330e20165bacd77ca843c602b510120a415415573bcdef3ccbc30a0e5aaf20f257360cfe24712aea0008f149ce5bb99834c0c0b
+    has-tostringtag: ^1.0.2
+  checksum: 65227dcbfadf5677aacc43ec84356d17b5500cb8b8753059bb4397de5cd0c2de681d24e1a7bd575633f976a95f88233abfd6549c2105ef4ebd58af8aa1807c75
   languageName: node
   linkType: hard
 
 "which@npm:^1.2.9, which@npm:^1.3.1":
   version: 1.3.1
   resolution: "which@npm:1.3.1"
   dependencies:
@@ -10213,14 +10333,21 @@
 "wildcard@npm:^2.0.0":
   version: 2.0.1
   resolution: "wildcard@npm:2.0.1"
   checksum: e0c60a12a219e4b12065d1199802d81c27b841ed6ad6d9d28240980c73ceec6f856771d575af367cbec2982d9ae7838759168b551776577f155044f5a5ba843c
   languageName: node
   linkType: hard
 
+"word-wrap@npm:^1.2.5":
+  version: 1.2.5
+  resolution: "word-wrap@npm:1.2.5"
+  checksum: f93ba3586fc181f94afdaff3a6fef27920b4b6d9eaefed0f428f8e07adea2a7f54a5f2830ce59406c8416f033f86902b91eb824072354645eea687dff3691ccb
+  languageName: node
+  linkType: hard
+
 "worker-loader@npm:^3.0.2":
   version: 3.0.8
   resolution: "worker-loader@npm:3.0.8"
   dependencies:
     loader-utils: ^2.0.0
     schema-utils: ^3.0.0
   peerDependencies:
@@ -10265,25 +10392,25 @@
     imurmurhash: ^0.1.4
     signal-exit: ^3.0.7
   checksum: 5da60bd4eeeb935eec97ead3df6e28e5917a6bd317478e4a85a5285e8480b8ed96032bbcc6ecd07b236142a24f3ca871c924ec4a6575e623ec1b11bf8c1c253c
   languageName: node
   linkType: hard
 
 "ws@npm:^8.11.0":
-  version: 8.16.0
-  resolution: "ws@npm:8.16.0"
+  version: 8.17.0
+  resolution: "ws@npm:8.17.0"
   peerDependencies:
     bufferutil: ^4.0.1
     utf-8-validate: ">=5.0.2"
   peerDependenciesMeta:
     bufferutil:
       optional: true
     utf-8-validate:
       optional: true
-  checksum: feb3eecd2bae82fa8a8beef800290ce437d8b8063bdc69712725f21aef77c49cb2ff45c6e5e7fce622248f9c7abaee506bae0a9064067ffd6935460c7357321b
+  checksum: 147ef9eab0251364e1d2c55338ad0efb15e6913923ccbfdf20f7a8a6cb8f88432bcd7f4d8f66977135bfad35575644f9983201c1a361019594a4e53977bf6d4e
   languageName: node
   linkType: hard
 
 "xml-name-validator@npm:^4.0.0":
   version: 4.0.0
   resolution: "xml-name-validator@npm:4.0.0"
   checksum: af100b79c29804f05fa35aa3683e29a321db9b9685d5e5febda3fa1e40f13f85abc40f45a6b2bf7bee33f68a1dc5e8eaef4cec100a304a9db565e6061d4cb5ad
@@ -10376,19 +10503,19 @@
     y18n: ^5.0.5
     yargs-parser: ^21.1.1
   checksum: 73b572e863aa4a8cbef323dd911d79d193b772defd5a51aab0aca2d446655216f5002c42c5306033968193bdbf892a7a4c110b0d77954a7fdf563e653967b56a
   languageName: node
   linkType: hard
 
 "yjs@npm:^13.5.0, yjs@npm:^13.5.40":
-  version: 13.6.11
-  resolution: "yjs@npm:13.6.11"
+  version: 13.6.15
+  resolution: "yjs@npm:13.6.15"
   dependencies:
     lib0: ^0.2.86
-  checksum: fb2993b12c6d13caf52d41af747991fa0be0a7e560ad2de84a736b4b7fa085d8327ff7254238840c407fa0671ca8c8e5917baea32f6d6686923c602134045b94
+  checksum: a0cdb323f9cd40de37c9cd0a9a4613e35d8365488ed6078ec632f0ec1853de4d16e46d435dc97e4029c0e70666e24d02c7240a71e84f7b1f15ff18670d715483
   languageName: node
   linkType: hard
 
 "yocto-queue@npm:^0.1.0":
   version: 0.1.0
   resolution: "yocto-queue@npm:0.1.0"
   checksum: f77b3d8d00310def622123df93d4ee654fc6a0096182af8bd60679ddcdfb3474c56c6c7190817c84a2785648cdee9d721c0154eb45698c62176c322fb46fc700
```

### Comparing `jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/labextension/package.json` & `jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9706196581196581%*

 * *Differences: {"'dependencies'": "{'hatch': '^1.1.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.d43dde86f53fb87db6c8.js'}}",*

 * * "'version'": "'0.5.5'"}*

```diff
@@ -3,15 +3,16 @@
         "email": "team@athenaintelligence.ai",
         "name": "Athena Intelligence"
     },
     "bugs": {
         "url": "https://github.com/github_username/jupyterlab_athena_analytics/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^4.0.0"
+        "@jupyterlab/application": "^4.0.0",
+        "hatch": "^1.1.0"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
@@ -103,15 +104,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/github_username/jupyterlab_athena_analytics",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b1df3a258d734729eff5.js",
+            "load": "static/remoteEntry.d43dde86f53fb87db6c8.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_athena_analytics/labextension"
     },
     "keywords": [
         "jupyter",
@@ -177,12 +178,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.5.1",
+    "version": "0.5.5",
     "workspaces": [
         "workspace/athena-notebooks/jupyterlab_athena_analytics"
     ]
 }
```

### Comparing `jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/labextension/static/736.1c2d46418a08bbb03c03.js` & `jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/728.c9fba78fc7d4a52b2765.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,66 +1,66 @@
 "use strict";
 (self.webpackChunkjupyterlab_athena_analytics = self.webpackChunkjupyterlab_athena_analytics || []).push([
-    [736], {
-        795: (e, t, n) => {
+    [728], {
+        475: (e, t, n) => {
             n.d(t, {
-                c: () => s
+                A: () => c
             });
-            var r = n(500),
+            var r = n(601),
                 a = n.n(r),
-                o = n(312),
-                c = n.n(o)()(a());
-            c.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n", ""]);
-            const s = c
+                o = n(314),
+                s = n.n(o)()(a());
+            s.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n", ""]);
+            const c = s
         },
-        312: e => {
+        314: e => {
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
                         var n = "",
                             r = void 0 !== t[5];
                         return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), r && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), r && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
                     })).join("")
                 }, t.i = function(e, n, r, a, o) {
                     "string" == typeof e && (e = [
                         [null, e, void 0]
                     ]);
-                    var c = {};
+                    var s = {};
                     if (r)
-                        for (var s = 0; s < this.length; s++) {
-                            var i = this[s][0];
-                            null != i && (c[i] = !0)
+                        for (var c = 0; c < this.length; c++) {
+                            var i = this[c][0];
+                            null != i && (s[i] = !0)
                         }
                     for (var u = 0; u < e.length; u++) {
                         var l = [].concat(e[u]);
-                        r && c[l[0]] || (void 0 !== o && (void 0 === l[5] || (l[1] = "@layer".concat(l[5].length > 0 ? " ".concat(l[5]) : "", " {").concat(l[1], "}")), l[5] = o), n && (l[2] ? (l[1] = "@media ".concat(l[2], " {").concat(l[1], "}"), l[2] = n) : l[2] = n), a && (l[4] ? (l[1] = "@supports (".concat(l[4], ") {").concat(l[1], "}"), l[4] = a) : l[4] = "".concat(a)), t.push(l))
+                        r && s[l[0]] || (void 0 !== o && (void 0 === l[5] || (l[1] = "@layer".concat(l[5].length > 0 ? " ".concat(l[5]) : "", " {").concat(l[1], "}")), l[5] = o), n && (l[2] ? (l[1] = "@media ".concat(l[2], " {").concat(l[1], "}"), l[2] = n) : l[2] = n), a && (l[4] ? (l[1] = "@supports (".concat(l[4], ") {").concat(l[1], "}"), l[4] = a) : l[4] = "".concat(a)), t.push(l))
                     }
                 }, t
             }
         },
-        500: e => {
+        601: e => {
             e.exports = function(e) {
                 return e[1]
             }
         },
-        596: e => {
+        72: e => {
             var t = [];
 
             function n(e) {
                 for (var n = -1, r = 0; r < t.length; r++)
                     if (t[r].identifier === e) {
                         n = r;
                         break
                     } return n
             }
 
             function r(e, r) {
-                for (var o = {}, c = [], s = 0; s < e.length; s++) {
-                    var i = e[s],
+                for (var o = {}, s = [], c = 0; c < e.length; c++) {
+                    var i = e[c],
                         u = r.base ? i[0] + r.base : i[0],
                         l = o[u] || 0,
                         p = "".concat(u, " ").concat(l);
                     o[u] = l + 1;
                     var f = n(p),
                         d = {
                             css: i[1],
@@ -68,23 +68,23 @@
                             sourceMap: i[3],
                             supports: i[4],
                             layer: i[5]
                         };
                     if (-1 !== f) t[f].references++, t[f].updater(d);
                     else {
                         var v = a(d, r);
-                        r.byIndex = s, t.splice(s, 0, {
+                        r.byIndex = c, t.splice(c, 0, {
                             identifier: p,
                             updater: v,
                             references: 1
                         })
                     }
-                    c.push(p)
+                    s.push(p)
                 }
-                return c
+                return s
             }
 
             function a(e, t) {
                 var n = t.domAPI(t);
                 return n.update(e),
                     function(t) {
                         if (t) {
@@ -93,27 +93,27 @@
                         } else n.remove()
                     }
             }
             e.exports = function(e, a) {
                 var o = r(e = e || [], a = a || {});
                 return function(e) {
                     e = e || [];
-                    for (var c = 0; c < o.length; c++) {
-                        var s = n(o[c]);
-                        t[s].references--
+                    for (var s = 0; s < o.length; s++) {
+                        var c = n(o[s]);
+                        t[c].references--
                     }
                     for (var i = r(e, a), u = 0; u < o.length; u++) {
                         var l = n(o[u]);
                         0 === t[l].references && (t[l].updater(), t.splice(l, 1))
                     }
                     o = i
                 }
             }
         },
-        176: e => {
+        659: e => {
             var t = {};
             e.exports = function(e, n) {
                 var r = function(e) {
                     if (void 0 === t[e]) {
                         var n = document.querySelector(e);
                         if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                             n = n.contentDocument.head
@@ -124,27 +124,27 @@
                     }
                     return t[e]
                 }(e);
                 if (!r) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                 r.appendChild(n)
             }
         },
-        808: e => {
+        540: e => {
             e.exports = function(e) {
                 var t = document.createElement("style");
                 return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
             }
         },
-        120: (e, t, n) => {
+        56: (e, t, n) => {
             e.exports = function(e) {
                 var t = n.nc;
                 t && e.setAttribute("nonce", t)
             }
         },
-        520: e => {
+        825: e => {
             e.exports = function(e) {
                 if ("undefined" == typeof document) return {
                     update: function() {},
                     remove: function() {}
                 };
                 var t = e.insertStyleElement(e);
                 return {
@@ -163,36 +163,36 @@
                             if (null === e.parentNode) return !1;
                             e.parentNode.removeChild(e)
                         }(t)
                     }
                 }
             }
         },
-        936: e => {
+        113: e => {
             e.exports = function(e, t) {
                 if (t.styleSheet) t.styleSheet.cssText = e;
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
-        736: (e, t, n) => {
+        728: (e, t, n) => {
             n.r(t);
-            var r = n(596),
+            var r = n(72),
                 a = n.n(r),
-                o = n(520),
-                c = n.n(o),
-                s = n(176),
-                i = n.n(s),
-                u = n(120),
+                o = n(825),
+                s = n.n(o),
+                c = n(659),
+                i = n.n(c),
+                u = n(56),
                 l = n.n(u),
-                p = n(808),
+                p = n(540),
                 f = n.n(p),
-                d = n(936),
+                d = n(113),
                 v = n.n(d),
-                h = n(795),
+                h = n(475),
                 m = {};
-            m.styleTagTransform = v(), m.setAttributes = l(), m.insert = i().bind(null, "head"), m.domAPI = c(), m.insertStyleElement = f(), a()(h.c, m), h.c && h.c.locals && h.c.locals
+            m.styleTagTransform = v(), m.setAttributes = l(), m.insert = i().bind(null, "head"), m.domAPI = s(), m.insertStyleElement = f(), a()(h.A, m), h.A && h.A.locals && h.A.locals
         }
     }
 ]);
```

### Comparing `jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/labextension/static/remoteEntry.b1df3a258d734729eff5.js` & `jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/remoteEntry.d43dde86f53fb87db6c8.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, f, d, p, c, h, v, y, b = {
-            280: (e, r, t) => {
+    var e, r, t, n, a, o, i, u, l, s, f, c, d, p, h, v, b, y = {
+            98: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(496).then((() => () => t(496))),
-                        "./extension": () => t.e(496).then((() => () => t(496))),
-                        "./style": () => t.e(736).then((() => () => t(736)))
+                        "./index": () => t.e(509).then((() => () => t(509))),
+                        "./extension": () => t.e(509).then((() => () => t(509))),
+                        "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -30,32 +30,32 @@
     function m(e) {
         var r = g[e];
         if (void 0 !== r) return r.exports;
         var t = g[e] = {
             id: e,
             exports: {}
         };
-        return b[e](t, t.exports, m), t.exports
+        return y[e](t, t.exports, m), t.exports
     }
-    m.m = b, m.c = g, m.n = e => {
+    m.m = y, m.c = g, m.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return m.d(r, {
             a: r
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        496: "0fc234152a8e8b8f31ed",
-        736: "1c2d46418a08bbb03c03"
+        509: "68053d43f01f7d268d38",
+        728: "c9fba78fc7d4a52b2765"
     } [e] + ".js?v=" + {
-        496: "0fc234152a8e8b8f31ed",
-        736: "1c2d46418a08bbb03c03"
+        509: "68053d43f01f7d268d38",
+        728: "c9fba78fc7d4a52b2765"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -68,24 +68,24 @@
                     var f = l[s];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
                         i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            var c = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(d);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                d = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -102,29 +102,29 @@
                 var o = m.S[t],
                     i = "jupyterlab_athena_analytics",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
-                        get: () => m.e(496).then((() => () => m(496))),
+                        get: () => m.e(509).then((() => () => m(509))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab_athena_analytics", "0.5.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab_athena_analytics", "0.5.5"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
-                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
+                for (var n = t.length - 1; n > -1 && (!e || !/^http(s?):/.test(e));) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
@@ -164,87 +164,88 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !a : "" == d != a);
+                var s, f, c = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == c ? u > n && !a : "" == c != a);
                 if ("u" == f) {
-                    if (!l || "u" != d) return !1
+                    if (!l || "u" != c) return !1
                 } else if (l)
-                    if (d == f)
+                    if (c == f)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
                             if (a ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != c && "n" != c) {
                     if (a || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < d != a) return !1;
+                    if (u <= n || f < c != a) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != c && "n" != c && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var d = [],
+            p = d.pop.bind(d);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+            d.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
         var a = u(e, t);
-        return o(n, a) || f(l(e, t, a, n)), d(e[t][a])
+        return o(n, a) || f(l(e, t, a, n)), c(e[t][a])
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, a) {
+    }, c = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, a) {
         var o = m.I(r);
         return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, a)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
-        628: () => p("default", "@jupyterlab/notebook", [1, 4, 1, 8])
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), p = {}, h = {
+        242: () => d("default", "@jupyterlab/docmanager", [1, 4, 1, 8]),
+        506: () => d("default", "@jupyterlab/notebook", [1, 4, 1, 8])
     }, v = {
-        496: [628]
-    }, y = {}, m.f.consumes = (e, r) => {
+        509: [242, 506]
+    }, b = {}, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
-            if (m.o(c, e)) return r.push(c[e]);
-            if (!y[e]) {
+            if (m.o(p, e)) return r.push(p[e]);
+            if (!b[e]) {
                 var t = r => {
-                    c[e] = 0, m.m[e] = t => {
+                    p[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
                 };
-                y[e] = !0;
+                b[e] = !0;
                 var n = r => {
-                    delete c[e], m.m[e] = t => {
+                    delete p[e], m.m[e] = t => {
                         throw delete m.c[e], r
                     }
                 };
                 try {
                     var a = h[e]();
-                    a.then ? r.push(c[e] = a.then(t).catch(n)) : t(a)
+                    a.then ? r.push(p[e] = a.then(t).catch(n)) : t(a)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
-            248: 0
+            642: 0
         };
         m.f.j = (r, t) => {
             var n = m.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var a = new Promise(((t, a) => n = e[r] = [t, a]));
@@ -268,10 +269,10 @@
                     u && u(m)
                 }
                 for (r && r(t); l < o.length; l++) a = o[l], m.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunkjupyterlab_athena_analytics = self.webpackChunkjupyterlab_athena_analytics || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), m.nc = void 0;
-    var w = m(280);
+    var w = m(98);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).jupyterlab_athena_analytics = w
 })();
```

### Comparing `jupyterlab_athena_analytics-0.5.1/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json` & `jupyterlab_athena_analytics-0.5.5/jupyterlab_athena_analytics/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.11.0'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "6.10.0"
+            "versionInfo": "6.11.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
             "versionInfo": "3.3.4"
         }
```

### Comparing `jupyterlab_athena_analytics-0.5.1/ui-tests/README.md` & `jupyterlab_athena_analytics-0.5.5/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.1/ui-tests/tests/jupyterlab_athena_analytics.spec.ts` & `jupyterlab_athena_analytics-0.5.5/ui-tests/tests/jupyterlab_athena_analytics.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.1/.gitignore` & `jupyterlab_athena_analytics-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.1/LICENSE` & `jupyterlab_athena_analytics-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.1/README.md` & `jupyterlab_athena_analytics-0.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # DEVELOP
 
+cd jupyterlab_athena_analytics
+
+### install
+npm install
+
+
+
 ### Build Extension
 ```
-cd jupyterlab_athena_analytics
 pip install -e .
 ```
 
 
 ### Serve to view in jupyter
 ```
 cd ~/workspace/notebooks
```

### Comparing `jupyterlab_athena_analytics-0.5.1/pyproject.toml` & `jupyterlab_athena_analytics-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_athena_analytics-0.5.1/PKG-INFO` & `jupyterlab_athena_analytics-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab_athena_analytics
-Version: 0.5.1
+Version: 0.5.5
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/github_username/jupyterlab_athena_analytics
 Project-URL: Bug Tracker, https://github.com/github_username/jupyterlab_athena_analytics/issues
 Project-URL: Repository, https://github.com/github_username/jupyterlab_athena_analytics.git
 Author-email: Athena Intelligence <team@athenaintelligence.ai>
 License: BSD 3-Clause License
         
@@ -49,17 +49,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # DEVELOP
 
+cd jupyterlab_athena_analytics
+
+### install
+npm install
+
+
+
 ### Build Extension
 ```
-cd jupyterlab_athena_analytics
 pip install -e .
 ```
 
 
 ### Serve to view in jupyter
 ```
 cd ~/workspace/notebooks
```

