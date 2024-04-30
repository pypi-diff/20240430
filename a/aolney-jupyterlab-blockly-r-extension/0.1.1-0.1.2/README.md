# Comparing `tmp/aolney_jupyterlab_blockly_r_extension-0.1.1.tar.gz` & `tmp/aolney_jupyterlab_blockly_r_extension-0.1.2.tar.gz`

## Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1.tar` & `aolney_jupyterlab_blockly_r_extension-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/.copier-answers.yml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/babel.config.js
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/environment.yml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/jest.config.js
--rw-r--r--   0        0        0     6751 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/package.json
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/python-testing.ipynb
--rw-r--r--   0        0        0    21365 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/r-test.ipynb
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/tsconfig.test.json
--rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/watch.sh
--rw-r--r--   0        0        0   378784 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/yarn.lock
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/_version.py
--rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/package.json
--rw-r--r--   0        0        0   140516 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/369.02184f958ba98de69fb9.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/369.02184f958ba98de69fb9.js.LICENSE.txt
--rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/728.fab96543eb438ca8425a.js
--rw-r--r--   0        0        0    65063 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/978.4bc44e871dcb20252e08.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/978.4bc44e871dcb20252e08.js.LICENSE.txt
--rw-r--r--   0        0        0   558336 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/983.e6daa4ad1ba05ddae851.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/983.e6daa4ad1ba05ddae851.js.LICENSE.txt
--rw-r--r--   0        0        0     7857 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/remoteEntry.b9292539421da221e3e6.js
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    57673 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/src/RGenerator.ts
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/src/SearchDropdown.ts
--rw-r--r--   0        0        0    50672 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/src/Toolbox.ts
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/src/field_minus.ts
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/src/field_plus.ts
--rw-r--r--   0        0        0    20978 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/src/index.ts
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/src/logging.ts
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/src/__tests__/aolney_jupyterlab_blockly_r_extension.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/style/base.css
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/style/index.js
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/ui-tests/package.json
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/ui-tests/yarn.lock
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/ui-tests/tests/aolney_jupyterlab_blockly_r_extension.spec.ts
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/LICENSE
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/README.md
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    18798 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/.copier-answers.yml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/babel.config.js
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/environment.yml
+-rw-r--r--   0        0        0    30613 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/fable-to-typescript-conversion-source.7z
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/jest.config.js
+-rw-r--r--   0        0        0     6751 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/package.json
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/python-testing.ipynb
+-rw-r--r--   0        0        0    25872 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/r-test.ipynb
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/tsconfig.test.json
+-rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/watch.sh
+-rw-r--r--   0        0        0   378784 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/yarn.lock
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/_version.py
+-rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/package.json
+-rw-r--r--   0        0        0   140516 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/369.33cb3b39acb33feedba2.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/369.33cb3b39acb33feedba2.js.LICENSE.txt
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/728.fab96543eb438ca8425a.js
+-rw-r--r--   0        0        0    65465 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/978.503c08dddbdbe0d6b639.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/978.503c08dddbdbe0d6b639.js.LICENSE.txt
+-rw-r--r--   0        0        0   558336 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/983.e6daa4ad1ba05ddae851.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/983.e6daa4ad1ba05ddae851.js.LICENSE.txt
+-rw-r--r--   0        0        0     7857 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/remoteEntry.ea69d1a6ef05a0944e0d.js
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    57673 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/src/RGenerator.ts
+-rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/src/SearchDropdown.ts
+-rw-r--r--   0        0        0    53649 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/src/Toolbox.ts
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/src/field_minus.ts
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/src/field_plus.ts
+-rw-r--r--   0        0        0    20978 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/src/index.ts
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/src/logging.ts
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/src/__tests__/aolney_jupyterlab_blockly_r_extension.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/style/base.css
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/style/index.js
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/ui-tests/package.json
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/ui-tests/tests/aolney_jupyterlab_blockly_r_extension.spec.ts
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/README.md
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    18798 2020-02-02 00:00:00.000000 aolney_jupyterlab_blockly_r_extension-0.1.2/PKG-INFO
```

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/.copier-answers.yml` & `aolney_jupyterlab_blockly_r_extension-0.1.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/RELEASE.md` & `aolney_jupyterlab_blockly_r_extension-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/jest.config.js` & `aolney_jupyterlab_blockly_r_extension-0.1.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/package.json` & `aolney_jupyterlab_blockly_r_extension-0.1.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -189,9 +189,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/python-testing.ipynb` & `aolney_jupyterlab_blockly_r_extension-0.1.2/python-testing.ipynb`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/tsconfig.json` & `aolney_jupyterlab_blockly_r_extension-0.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/yarn.lock` & `aolney_jupyterlab_blockly_r_extension-0.1.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/__init__.py` & `aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/package.json` & `aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ea69d1a6ef05a0944e0d.js'}}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -108,15 +108,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/aolney/jupyterlab-blockly-r-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b9292539421da221e3e6.js",
+            "load": "static/remoteEntry.ea69d1a6ef05a0944e0d.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "aolney_jupyterlab_blockly_r_extension/labextension"
     },
     "keywords": [
         "jupyter",
@@ -194,9 +194,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/369.02184f958ba98de69fb9.js` & `aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/369.33cb3b39acb33feedba2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 369.02184f958ba98de69fb9.js.LICENSE.txt */
+/*! For license information please see 369.33cb3b39acb33feedba2.js.LICENSE.txt */
 (self.webpackChunk_aolney_jupyterlab_blockly_r_extension = self.webpackChunk_aolney_jupyterlab_blockly_r_extension || []).push([
     [369], {
         499: function(e, t, s) {
             var n, o, i;
             o = [s(791)], void 0 === (i = "function" == typeof(n = function(e) {
                 return e
             }) ? n.apply(t, o) : n) || (e.exports = i)
@@ -2351,19 +2351,19 @@
             var n, o, i;
             o = [s(225)], void 0 === (i = "function" == typeof(n = function(e) {
                 return e
             }) ? n.apply(t, o) : n) || (e.exports = i)
         },
         986: function(e, t, s) {
             var n, o, i;
-            o = [s(983), s(824)], void 0 === (i = "function" == typeof(n = function(e, t) {
+            o = [s(983), s(443)], void 0 === (i = "function" == typeof(n = function(e, t) {
                 return t
             }) ? n.apply(t, o) : n) || (e.exports = i)
         },
-        824: function(e, t, s) {
+        443: function(e, t, s) {
             var n, o, i;
             o = [s(731)], void 0 === (i = "function" == typeof(n = function(e) {
                 var t, s, n = e.__namespace__,
                     o = function(e, s) {
                         var n = 0;
                         let o = "";
                         s.STATEMENT_PREFIX && (o += s.injectId(s.STATEMENT_PREFIX, e));
```

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/728.fab96543eb438ca8425a.js` & `aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/728.fab96543eb438ca8425a.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/978.4bc44e871dcb20252e08.js` & `aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/978.503c08dddbdbe0d6b639.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,45 +1,45 @@
-/*! For license information please see 978.4bc44e871dcb20252e08.js.LICENSE.txt */
+/*! For license information please see 978.503c08dddbdbe0d6b639.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_aolney_jupyterlab_blockly_r_extension = self.webpackChunk_aolney_jupyterlab_blockly_r_extension || []).push([
     [978], {
         978: (e, t, n) => {
             n.r(t), n.d(t, {
-                BlocklyWidget: () => P,
-                BlocklyWidget__ActiveCellSerializedBlocksWorkspaceOption: () => ee,
-                BlocklyWidget__RenderBlocks: () => ne,
-                BlocklyWidget__RenderCode: () => te,
-                BlocklyWidget__RenderCodeToLastCell: () => oe,
-                BlocklyWidget__clearBlocks: () => le,
-                BlocklyWidget__get_Notebooks: () => X,
-                BlocklyWidget__get_blocksRendered: () => q,
-                BlocklyWidget__get_lastCell: () => Q,
-                BlocklyWidget__get_notHooked: () => z,
-                BlocklyWidget__get_onActiveCellChanged: () => J,
-                BlocklyWidget__get_onKernelExecuted: () => $,
-                BlocklyWidget__get_workspace: () => j,
-                BlocklyWidget__set_blocksRendered: () => Y,
-                BlocklyWidget__set_lastCell: () => Z,
-                BlocklyWidget__set_notHooked: () => K,
+                BlocklyWidget: () => j,
+                BlocklyWidget__ActiveCellSerializedBlocksWorkspaceOption: () => te,
+                BlocklyWidget__RenderBlocks: () => oe,
+                BlocklyWidget__RenderCode: () => ne,
+                BlocklyWidget__RenderCodeToLastCell: () => le,
+                BlocklyWidget__clearBlocks: () => ie,
+                BlocklyWidget__get_Notebooks: () => H,
+                BlocklyWidget__get_blocksRendered: () => z,
+                BlocklyWidget__get_lastCell: () => Z,
+                BlocklyWidget__get_notHooked: () => K,
+                BlocklyWidget__get_onActiveCellChanged: () => ee,
+                BlocklyWidget__get_onKernelExecuted: () => J,
+                BlocklyWidget__get_workspace: () => X,
+                BlocklyWidget__set_blocksRendered: () => q,
+                BlocklyWidget__set_lastCell: () => $,
+                BlocklyWidget__set_notHooked: () => Q,
                 BlocklyWidget__set_workspace: () => G,
-                BlocklyWidget_factor: () => H,
-                attachWidget: () => ae,
-                createMainAreaWidget: () => ie,
-                default: () => ue,
-                onKernelChanged: () => re,
-                onNotebookChanged: () => ce,
-                runCommandOnNotebookChanged: () => se
+                BlocklyWidget_factor: () => Y,
+                attachWidget: () => se,
+                createMainAreaWidget: () => ae,
+                default: () => de,
+                onKernelChanged: () => ce,
+                onNotebookChanged: () => ue,
+                runCommandOnNotebookChanged: () => re
             });
-            var o = n(465),
+            var o = n(371),
                 l = n(256),
                 i = n(983),
-                a = n(638),
-                s = n(750),
-                r = n(372),
-                c = n(315);
+                a = n(440),
+                s = n(824),
+                r = n(506),
+                c = n(385);
             const u = new i.Generator("R");
             u.addReservedWords("Blockly,if,else,repeat,while,function,for,in,next,break,TRUE,FALSE,NULL,Inf,NaN,NA,NA_integer_,NA_real_,NA_complex_,NA_character_,...,..1,..2,..3,..4,..5,..6,..7,..8,..9"), u.ORDER_ATOMIC = 0, u.ORDER_NEW = 1.1, u.ORDER_MEMBER = 1.2, u.ORDER_FUNCTION_CALL = 2, u.ORDER_INCREMENT = 3, u.ORDER_DECREMENT = 3, u.ORDER_BITWISE_NOT = 4.1, u.ORDER_UNARY_PLUS = 4.2, u.ORDER_UNARY_NEGATION = 4.3, u.ORDER_LOGICAL_NOT = 4.4, u.ORDER_TYPEOF = 4.5, u.ORDER_VOID = 4.6, u.ORDER_DELETE = 4.7, u.ORDER_AWAIT = 4.8, u.ORDER_EXPONENTIATION = 5, u.ORDER_DIVISION = 5.1, u.ORDER_MULTIPLICATION = 5.2, u.ORDER_MODULUS = 5.3, u.ORDER_ADDITION = 6.1, u.ORDER_SUBTRACTION = 6.2, u.ORDER_BITWISE_SHIFT = 7, u.ORDER_RELATIONAL = 8, u.ORDER_IN = 8, u.ORDER_INSTANCEOF = 8, u.ORDER_EQUALITY = 9, u.ORDER_BITWISE_AND = 10, u.ORDER_BITWISE_XOR = 11, u.ORDER_BITWISE_OR = 12, u.ORDER_LOGICAL_AND = 13, u.ORDER_LOGICAL_OR = 14, u.ORDER_CONDITIONAL = 15, u.ORDER_ASSIGNMENT = 16, u.ORDER_YIELD = 17, u.ORDER_COMMA = 18, u.ORDER_NONE = 99, u.ORDER_OVERRIDES = [
                 [u.ORDER_FUNCTION_CALL, u.ORDER_MEMBER],
                 [u.ORDER_FUNCTION_CALL, u.ORDER_FUNCTION_CALL],
                 [u.ORDER_MEMBER, u.ORDER_MEMBER],
                 [u.ORDER_MEMBER, u.ORDER_FUNCTION_CALL],
                 [u.ORDER_LOGICAL_NOT, u.ORDER_LOGICAL_NOT],
@@ -732,15 +732,15 @@
                     o = n && i.Xml.domToText(n);
                 t.plus(e.args_);
                 const l = t.mutationToDom(),
                     a = l && i.Xml.domToText(l);
                 o != a && i.Events.fire(new i.Events.BlockChange(t, "mutation", null, o, a)), i.Events.setGroup(!1)
             }
             const O = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZlcnNpb249IjEuMSIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0Ij48cGF0aCBkPSJNMTggMTBoLTR2LTRjMC0xLjEwNC0uODk2LTItMi0ycy0yIC44OTYtMiAybC4wNzEgNGgtNC4wNzFjLTEuMTA0IDAtMiAuODk2LTIgMnMuODk2IDIgMiAybDQuMDcxLS4wNzEtLjA3MSA0LjA3MWMwIDEuMTA0Ljg5NiAyIDIgMnMyLS44OTYgMi0ydi00LjA3MWw0IC4wNzFjMS4xMDQgMCAyLS44OTYgMi0ycy0uODk2LTItMi0yeiIgZmlsbD0id2hpdGUiIC8+PC9zdmc+Cg==";
-            var T = n(723);
+            var T = n(574);
             const b = E;
 
             function g() {
                 const e = d.Xml.workspaceToDom(d.getMainWorkspace());
                 return d.Xml.domToText(e)
             }
 
@@ -752,17 +752,17 @@
                     }
                 }, u[e] = e => {
                     const o = e.getFieldValue("CODE").toString();
                     let l;
                     return l = t ? (o + " " + u.valueToCode(e, "INPUT", u.ORDER_ATOMIC)).trim() : o.trim(), n ? [l, u.ORDER_ATOMIC] : l + "\n"
                 }
             }
-            var D;
+            var f;
 
-            function f(e, t, n, o, l, i) {
+            function D(e, t, n, o, l, i) {
                 d.Blocks[e] = {
                     init: function() {
                         console.log(e + " init"), this.appendValueInput("x").setCheck(void 0).appendField(t), this.setInputsInline(!0), this.setOutput(!0, n), this.setColour(230), this.setTooltip(o), this.setHelpUrl(l)
                     }
                 }, u[e] = e => {
                     const t = u.valueToCode(e, "x", u.ORDER_MEMBER).replace(/^\[|\]$/g, "");
                     return [`${i}(${t})`, u.ORDER_FUNCTION_CALL]
@@ -823,27 +823,27 @@
             }, u.textFromFile_R = e => {
                 const t = u.valueToCode(e, "FILENAME", u.ORDER_ATOMIC);
                 return ["readChar(" + t + ", file.info(" + t + ")$size)", u.ORDER_FUNCTION_CALL]
             }, d.Blocks.readFile_R = {
                 init: function() {
                     console.log("readFile_R init"), this.appendValueInput("FILENAME").setCheck("String").appendField("read file"), this.setOutput(!0, void 0), this.setColour(230), this.setTooltip("Use this to read a file. It will output a file, not a string."), this.setHelpUrl("https://stat.ethz.ch/R-manual/R-devel/library/base/html/connections.html")
                 }
-            }, u.readFile_R = e => ["file(" + u.valueToCode(e, "FILENAME", u.ORDER_ATOMIC) + ", 'rt')", u.ORDER_FUNCTION_CALL], N("dummyOutputCodeBlock_R", !1, !0), N("dummyNoOutputCodeBlock_R", !1, !1), N("valueOutputCodeBlock_R", !0, !0), N("valueNoOutputCodeBlock_R", !0, !1), D = "import_R", d.Blocks[D] = {
+            }, u.readFile_R = e => ["file(" + u.valueToCode(e, "FILENAME", u.ORDER_ATOMIC) + ", 'rt')", u.ORDER_FUNCTION_CALL], N("dummyOutputCodeBlock_R", !1, !0), N("dummyNoOutputCodeBlock_R", !1, !1), N("valueOutputCodeBlock_R", !0, !0), N("valueNoOutputCodeBlock_R", !0, !1), f = "import_R", d.Blocks[f] = {
                 init: function() {
                     this.appendDummyInput().appendField("library").appendField(new d.FieldVariable("some library"), "libraryName"), this.setNextStatement(!0), this.setPreviousStatement(!0), this.setColour(230), this.setTooltip("Load an R package to access functions in that package"), this.setHelpUrl("https://stat.ethz.ch/R-manual/R-devel/library/base/html/library.html")
                 }
-            }, u[D] = e => "library(" + u.getVariableName(e.getFieldValue("libraryName")) + ")\n", d.Blocks.indexer_R = {
+            }, u[f] = e => "library(" + u.getVariableName(e.getFieldValue("libraryName")) + ")\n", d.Blocks.indexer_R = {
                 init: function() {
                     this.appendValueInput("INDEX").appendField(new d.FieldVariable("{dictVariable}"), "VAR").appendField("["), this.appendDummyInput().appendField("]"), this.setInputsInline(!0), this.setOutput(!0), this.setColour(230), this.setTooltip("Gets a list from the variable at a given indices. Not supported for all variables."), this.setHelpUrl("https://cran.r-project.org/doc/manuals/R-lang.html#Indexing")
                 }
             }, u.indexer_R = e => [e.getFieldValue("VAR").toString() + "[" + u.valueToCode(e, "INDEX", u.ORDER_ATOMIC) + "]", u.ORDER_ATOMIC], d.Blocks.doubleIndexer_R = {
                 init: function() {
                     this.appendValueInput("INDEX").appendField(new d.FieldVariable("{dictVariable}"), "VAR").appendField("[["), this.appendDummyInput().appendField("]]"), this.setInputsInline(!0), this.setOutput(!0), this.setColour(230), this.setTooltip("Gets an item from the variable at a given index. Not supported for all variables."), this.setHelpUrl("https://cran.r-project.org/doc/manuals/R-lang.html#Indexing")
                 }
-            }, u.doubleIndexer_R = e => [e.getFieldValue("VAR").toString() + "[[" + u.valueToCode(e, "INDEX", u.ORDER_ATOMIC) + "]]", u.ORDER_ATOMIC], f("reversedBlock_R", "reversed", "None", "Provides a reversed version of its argument.", "https://stat.ethz.ch/R-manual/R-devel/library/base/html/rev.html", "rev"), f("boolConversion_R", "as bool", "Boolean", "Convert something to Boolean.", "https://stat.ethz.ch/R-manual/R-devel/library/base/html/logical.html", "as.logical"), f("strConversion_R", "as str", "String", "Convert something to String.", "https://stat.ethz.ch/R-manual/R-patched/library/base/html/toString.html", "toString"), f("floatConversion_R", "as float", "Number", "Convert something to Float.", "https://stat.ethz.ch/R-manual/R-devel/library/base/html/numeric.html", "as.numeric"), f("intConversion_R", "as int", "Number", "Convert something to Int.", "https://stat.ethz.ch/R-manual/R-devel/library/base/html/integer.html", "as.integer"), d.Blocks.unlistBlock_R = {
+            }, u.doubleIndexer_R = e => [e.getFieldValue("VAR").toString() + "[[" + u.valueToCode(e, "INDEX", u.ORDER_ATOMIC) + "]]", u.ORDER_ATOMIC], D("reversedBlock_R", "reversed", "None", "Provides a reversed version of its argument.", "https://stat.ethz.ch/R-manual/R-devel/library/base/html/rev.html", "rev"), D("boolConversion_R", "as bool", "Boolean", "Convert something to Boolean.", "https://stat.ethz.ch/R-manual/R-devel/library/base/html/logical.html", "as.logical"), D("strConversion_R", "as str", "String", "Convert something to String.", "https://stat.ethz.ch/R-manual/R-patched/library/base/html/toString.html", "toString"), D("floatConversion_R", "as float", "Number", "Convert something to Float.", "https://stat.ethz.ch/R-manual/R-devel/library/base/html/numeric.html", "as.numeric"), D("intConversion_R", "as int", "Number", "Convert something to Int.", "https://stat.ethz.ch/R-manual/R-devel/library/base/html/integer.html", "as.integer"), d.Blocks.unlistBlock_R = {
                 init: function() {
                     this.appendValueInput("LIST").setCheck("Array").appendField("vector"), this.setInputsInline(!0), this.setOutput(!0, "Array"), this.setColour(230), this.setTooltip("Use this to convert a list to a vector"), this.setHelpUrl("https://www.rdocumentation.org/packages/base/versions/3.6.2/topics/unlist")
                 }
             }, u.unlistBlock_R = e => ["unlist(" + u.valueToCode(e, "LIST", u.ORDER_MEMBER) + ", use.names = FALSE)", u.ORDER_FUNCTION_CALL], d.Blocks.uniqueBlock_R = {
                 init: function() {
                     this.appendValueInput("LIST").setCheck("Array").appendField("unique"), this.setInputsInline(!0), this.setOutput(!0, "Array"), this.setColour(230), this.setTooltip("Use this to get the unique elements of a list"), this.setHelpUrl("https://stackoverflow.com/questions/3879522/finding-unique-values-from-a-list")
                 }
@@ -932,109 +932,123 @@
                         }))
                     }))
                 }
             }
             const L = new Map([]);
 
             function y(e, t) {
-                return 0 === e.indexOf("`") || t.indexOf("Class attribute:\n'function'") >= 0 || t.indexOf("Usage") >= 0 && t.indexOf("Arguments") >= 0
+                return !!(e.startsWith("`") || t.includes(e + "(") || t.includes("Class attribute:\n'function'") || t.includes("Usage") && t.includes("Arguments") || t.includes("function") || t.includes("Function") || t.includes("object") || t.includes("Object"))
             }
 
             function S(e) {
                 return !y("", e)
             }
 
-            function F(e, t) {
+            function F(e) {
+                try {
+                    const t = new d.Events.BlockChange(e, "field", "VAR", 0, 1);
+                    t.group = "INTELLISENSE", console.log("event status is " + d.Events.disabled_), d.Events.disabled_ = 0, d.Events.fire(t)
+                } catch (e) {
+                    e instanceof Error && console.log("Intellisense event failed to fire; " + e.message)
+                }
+            }
+
+            function x(e, t) {
                 return "" === t || e.isInFlyout || function(e, t) {
                     M(t).then((n => {
                         const o = new C(t, n, y(t, n), S(n));
-                        let l, i = new v(o, []);
-                        const a = [L.has(o.Name), i];
-                        if (a[0]) {
-                            const e = a[1];
-                            l = e.VariableEntry.Info !== o.Info || 0 === e.ChildEntries.length
-                        } else l = !0;
-                        l ? function(e) {
+                        let l = !0,
+                            i = L.get(o.Name);
+                        i && (l = i.VariableEntry.Info !== o.Info || i.ChildEntries.length <= 1), l ? function(e) {
                             const t = A();
                             if (null == t) return Promise.reject((() => {
                                 throw 1
                             })());
                             {
                                 const n = t[1];
                                 return new Promise(((t, o) => {
-                                    setTimeout((() => {
-                                        n.requestComplete({
-                                            code: e,
-                                            cursor_pos: e.length
-                                        }).then((e => {
-                                            const n = e.content;
-                                            "matches" in n && t(n.matches.slice())
-                                        })).catch((t => {
-                                            o([e + " is unavailable"])
-                                        }))
-                                    }), 100)
+                                    n.requestComplete({
+                                        code: e,
+                                        cursor_pos: e.length
+                                    }).then((e => {
+                                        const n = e.content;
+                                        "matches" in n && t(n.matches.slice())
+                                    })).catch((t => {
+                                        o([e + " is unavailable"])
+                                    }))
                                 }))
                             }
                         }(t + "::").then((n => {
-                            const l = n.map((e => M(e)));
-                            return Promise.all(l).then((l => {
-                                const i = new v(o, n.map(((e, n) => {
-                                    const o = e.replace(new RegExp(t + "::"), "");
-                                    return new C(o, l[n], y(o, l[n]), S(l[n]))
-                                })));
-                                L.has(t) ? L.set(t, i) : function(e, t, n) {
-                                    if (e.has(t)) throw new Error("An item with the same key has already been added. Key: " + t);
-                                    e.set(t, n)
-                                }(L, t, i);
-                                const a = new d.Events.BlockChange(e, "field", "VAR", 0, 1);
-                                a.group = "INTELLISENSE", console.log("event status is " + d.Events.disabled_), d.Events.disabled_ = 0, d.Events.fire(a)
+                            const l = n.map(((e, t) => {
+                                return n = 100 * (t + 1), o = M(e), new Promise(((e, t) => {
+                                    const l = setTimeout((() => {
+                                        t(new Error("promise timeout"))
+                                    }), n);
+                                    o.then((t => {
+                                        clearTimeout(l), e(t)
+                                    }), (e => {
+                                        clearTimeout(l), t(e)
+                                    }))
+                                }));
+                                var n, o
+                            }));
+                            Promise.allSettled(l).then((l => {
+                                let i = n.map(((e, n) => {
+                                        const o = e.replace(new RegExp(t + "::"), "");
+                                        let i = "",
+                                            a = !0,
+                                            s = !1;
+                                        return "fulfilled" === l[n].status && (i = l[n].value, a = y(o, i), s = S(i)), new C(o, i, a, s)
+                                    })).sort(((e, t) => e.Name < t.Name ? -1 : 1)),
+                                    a = new v(o, i);
+                                L.set(t, a), F(e)
                             })).catch((e => {
-                                console.log("Error resolving promises:", e)
+                                console.log("Intellisense error getting inspections for children of " + t, e)
                             }))
                         })).catch((e => {
-                            console.log("Error getting completions:", e)
-                        })) : console.log("Not refreshing intellisense for " + o.Name)
+                            console.log("Intellisense error getting child completions of " + t, e)
+                        })) : (console.log("Not refreshing intellisense for " + o.Name), F(e))
                     })).catch((e => {
-                        console.log("Intellisense event failed to fire; " + e.message)
+                        console.log("Intellisense error getting inspection of intellisense variable candidate (parent) " + t, e)
                     }))
                 }(e, t), e.isInFlyout ? [
                     [" ", " "]
                 ] : "" !== t && L.has(t) ? [
                     ["!Waiting for kernel to respond with options.", "!Waiting for kernel to respond with options."]
                 ] : [
                     ["!Not defined until you execute code.", "!Not defined until you execute code."]
                 ]
             }
 
-            function x(e, t) {
+            function U(e, t) {
                 var n;
                 const o = (i = e, null, (l = L).has(i) ? [!0, l.get(i)] : [!1, null]);
                 var l, i;
                 if (o[0]) {
                     const e = null === (n = o[1]) || void 0 === n ? void 0 : n.ChildEntries.find((e => e.Name === t));
                     return null == e ? "!Not defined until you execute code." : e.Info
                 }
                 return "!Not defined until you execute code."
             }
 
-            function U() {
+            function w() {
                 const e = d.getMainWorkspace(),
                     t = e.getBlocksByType("varGetProperty_R", !1);
                 e.getBlocksByType("varDoMethod_R", !1).forEach((e => t.push(e))), t.forEach((e => {
-                    e.updateIntellisense(e, null, (t => F(e, t)))
-                })), e.registerToolboxCategoryCallback("VARIABLE", V)
+                    e.updateIntellisense(e, null, (t => x(e, t)))
+                })), e.registerToolboxCategoryCallback("VARIABLE", W)
             }
 
-            function w(e, t, n) {
+            function B(e, t, n) {
                 const o = e.getField(t),
                     l = e.getInput(n);
                 o && (l ? l.removeField(t) : console.log("error removing (" + t + ") from block; input (" + n + ") does not exist"))
             }
 
-            function B(e, t, n, o, l, i) {
+            function V(e, t, n, o, l, i) {
                 d.Blocks[e] = {
                     varSelectionUserName(e, t) {
                         const n = e.getField("VAR"),
                             o = e.workspace.getAllVariables().slice(-1)[0],
                             l = e.data,
                             i = l && l.indexOf(":") >= 0 ? l.split(":") : [""];
                         if (null == t) {
@@ -1046,32 +1060,32 @@
                             const e = n.getOptions().find((e => e[1] === t));
                             return e && "string" == typeof e[0] ? e[0] : ""
                         }
                     },
                     selectedMember: "",
                     updateIntellisense(e, t, n) {
                         const o = e.getInput("INPUT");
-                        w(e, "MEMBER", "INPUT"), w(e, "USING", "INPUT");
+                        B(e, "MEMBER", "INPUT"), B(e, "USING", "INPUT");
                         const l = e.varSelectionUserName(e, t),
                             i = n(l).map((e => e[0])),
                             a = e.data ? e.data : "";
                         if (o) {
                             let t = new b.FieldFilter(a, i, (function(t) {
                                 const n = "" === t ? a : this.WORDS[t];
                                 let o;
-                                return this.setTooltip(x(l, n)), e.selectedMember = (o = [0 === n.indexOf("!"), this.selectedMember], "" === o[1] ? n : o[0] ? this.selectedMember : n), "" !== l && "" !== e.selectedMember && (e.data = e.selectedMember), n
+                                return this.setTooltip(U(l, n)), e.selectedMember = (o = [0 === n.indexOf("!"), this.selectedMember], "" === o[1] ? n : o[0] ? this.selectedMember : n), "" !== l && "" !== e.selectedMember && (e.data = e.selectedMember), n
                             }));
                             o.appendField(t, "MEMBER")
                         }
                         void 0 !== e.data && null !== e.data || (e.data = e.selectedMember);
                         const s = e.getField("MEMBER");
-                        s && s.setTooltip(x(l, s.getText()))
+                        s && s.setTooltip(U(l, s.getText()))
                     },
                     init: function() {
-                        console.log(e + " init"), this.appendDummyInput("INPUT").appendField(t).appendField(new d.FieldVariable("variable name", (e => (this.updateIntellisense(this, e, (e => F(this, e))), e))), "VAR").appendField(n), this.updateIntellisense(this, null, (e => F(this, e))), this.setOutput(!0), this.setColour(230), this.setTooltip("!Not defined until you execute code."), this.setHelpUrl(""), l && (this.appendDummyInput("EMPTY"), d.Extensions.apply("intelliblockMutator", this, !0))
+                        console.log(e + " init"), this.appendDummyInput("INPUT").appendField(t).appendField(new d.FieldVariable("variable name", (e => (this.updateIntellisense(this, e, (e => x(this, e))), e))), "VAR").appendField(n), this.updateIntellisense(this, null, (e => x(this, e))), this.setOutput(!0), this.setColour(230), this.setTooltip("!Not defined until you execute code."), this.setHelpUrl(""), l && (this.appendDummyInput("EMPTY"), d.Extensions.apply("intelliblockMutator", this, !0))
                     },
                     onchange: function(e) {
                         if (this.workspace && !this.isInFlyout && "INTELLISENSE" === e.group) {
                             const e = this.data ? this.data.toString() : "";
                             this.updateIntellisense(this, null, (e => function(e, t) {
                                 const n = L.get(t);
                                 return n ? !n.VariableEntry.isFunction && n.ChildEntries.length > 0 ? n.ChildEntries.filter(e).map((e => [e.Name, e.Name])) : "UNDEFINED" === n.VariableEntry.Info ? [
@@ -1102,15 +1116,15 @@
                         }, ((t, n) => u.valueToCode(e, "ADD" + n.toString(), u.ORDER_COMMA))).join(",");
                         o = t + (i ? "::" : "") + n + "(" + l + ")"
                     } else o = t + (i ? "::" : "") + n;
                     return [o, u.ORDER_FUNCTION_CALL]
                 }
             }
 
-            function V(e) {
+            function W(e) {
                 const t = e.getVariablesOfType(""),
                     n = [],
                     o = document.createElement("button");
                 if (o.setAttribute("text", "%{BKY_NEW_VARIABLE}"), o.setAttribute("callbackKey", "CREATE_VARIABLE"), e.registerButtonCallback("CREATE_VARIABLE", (function(e) {
                         d.Variables.createVariableButtonHandler(e.getTargetWorkspace())
                     })), n.push(o), t.length > 0) {
                     const e = t[t.length - 1];
@@ -1140,49 +1154,49 @@
                         for (const e of t) {
                             const t = d.utils.xml.createElement("block");
                             t.setAttribute("type", "variables_get"), t.setAttribute("gap", "8"), t.appendChild(d.Variables.generateVariableFieldDom(e)), n.push(t)
                         }
                 }
                 return n
             }
-            I("intelliblockMutator", 1, "add argument", "using", "and"), B("varGetProperty_R", "from", "get", (e => !e.isFunction), !1, !0), B("varDoMethod_R", "with", "do", (e => e.isFunction), !0, !0), d.Variables.flyoutCategoryBlocks = e => {
-                if (W) {
+            I("intelliblockMutator", 1, "add argument", "using", "and"), V("varGetProperty_R", "from", "get", (e => !e.isFunction), !1, !0), V("varDoMethod_R", "with", "do", (e => e.isFunction), !0, !0), d.Variables.flyoutCategoryBlocks = e => {
+                if (P) {
                     const t = A();
                     if (t) {
                         const n = t[1],
-                            o = W.find((e => e.KernelCheckFunction(n.name)));
+                            o = P.find((e => e.KernelCheckFunction(n.name)));
                         return o ? o.FlyoutFunction(e) : []
                     }
                     return []
                 }
                 return []
             };
-            const W = [];
-            W.push(new class {
+            const P = [];
+            P.push(new class {
                 constructor(e, t, n) {
                     this.LanguageName = e, this.KernelCheckFunction = t, this.FlyoutFunction = n
                 }
-            }("R", (e => "ir" === e), V));
-            class P extends l.Widget {
+            }("R", (e => "ir" === e), W));
+            class j extends l.Widget {
                 constructor(e) {
-                    super(), this.notebooks = e, this.generator = u, this.notebooks.activeCellChanged.connect(J(this), this),
+                    super(), this.notebooks = e, this.generator = u, this.notebooks.activeCellChanged.connect(ee(this), this),
                         function(e) {
                             k = e
                         }(this.notebooks);
                     const t = document.createElement("div");
                     t.setAttribute("style", "height: 480px; width: 600px;"), t.id = "blocklyDivR", this.node.appendChild(t);
                     const n = document.createElement("div");
                     n.id = "buttonDivR";
                     const o = document.createElement("button");
                     o.innerText = "Blocks to Code", o.addEventListener("click", (e => {
-                        te(this)
+                        ne(this)
                     })), n.appendChild(o);
                     const l = document.createElement("button");
                     l.innerText = "Code to Blocks", l.addEventListener("click", (e => {
-                        ne(this)
+                        oe(this)
                     })), n.appendChild(l);
                     const i = document.createElement("button");
                     i.innerText = "Report Bug", i.addEventListener("click", (e => {
                         window.open("https://github.com/aolney/jupyterlab-blockly-r-extension/issues", "_blank").focus()
                     })), n.appendChild(i);
                     const a = document.createElement("input");
                     a.setAttribute("type", "checkbox"), a.checked = !0, a.id = "syncCheckboxR";
@@ -1207,17 +1221,17 @@
                 }
                 onAfterAttach() {
                     const e = this;
                     G(e, i.inject("blocklyDivR", {
                         toolbox: '<xml xmlns="https://developers.google.com/blockly/xml" id="toolbox" style="display: none">\n    <category name="IMPORT" colour="255">\n      <block type="import_R"></block>\n    </category>\n    <category name="FREESTYLE" colour="290">\n      <block type="dummyOutputCodeBlock_R"></block>\n      <block type="dummyNoOutputCodeBlock_R"></block>\n      <block type="valueOutputCodeBlock_R"></block>\n      <block type="valueNoOutputCodeBlock_R"></block>\n    </category>\n    <category name="LOGIC" colour="%{BKY_LOGIC_HUE}">\n      <block type="controls_if"></block>\n      <block type="logic_compare"></block>\n      <block type="logic_operation"></block>\n      <block type="logic_negate"></block>\n      <block type="logic_boolean"></block>\n      <block type="logic_null"></block>\n      <block type="logic_ternary"></block>\n    </category>\n    <category name="LOOPS" colour="%{BKY_LOOPS_HUE}">\n      <block type="controls_repeat_ext">\n        <value name="TIMES">\n          <shadow type="math_number">\n            <field name="NUM">10</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="controls_whileUntil"></block>\n      <block type="controls_for">\n        <value name="FROM">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="TO">\n          <shadow type="math_number">\n            <field name="NUM">10</field>\n          </shadow>\n        </value>\n        <value name="BY">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="controls_forEach"></block>\n      <block type="controls_flow_statements"></block>\n    </category>\n    <category name="MATH" colour="%{BKY_MATH_HUE}">\n      <block type="math_number">\n        <field name="NUM">123</field>\n      </block>\n      <block type="math_arithmetic">\n        <value name="A">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="B">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_single">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">9</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_trig">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">45</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_constant"></block>\n      <block type="math_number_property">\n        <value name="NUMBER_TO_CHECK">\n          <shadow type="math_number">\n            <field name="NUM">0</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_round">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">3.1</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_on_list"></block>\n      <block type="math_modulo">\n        <value name="DIVIDEND">\n          <shadow type="math_number">\n            <field name="NUM">64</field>\n          </shadow>\n        </value>\n        <value name="DIVISOR">\n          <shadow type="math_number">\n            <field name="NUM">10</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_constrain">\n        <value name="VALUE">\n          <shadow type="math_number">\n            <field name="NUM">50</field>\n          </shadow>\n        </value>\n        <value name="LOW">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="HIGH">\n          <shadow type="math_number">\n            <field name="NUM">100</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_random_int">\n        <value name="FROM">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="TO">\n          <shadow type="math_number">\n            <field name="NUM">100</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="math_random_float"></block>\n      <block type="math_atan2">\n        <value name="X">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n        <value name="Y">\n          <shadow type="math_number">\n            <field name="NUM">1</field>\n          </shadow>\n        </value>\n      </block>\n    </category>\n    <category name="TEXT" colour="%{BKY_TEXTS_HUE}">\n      <block type="text"></block>\n      <block type="text_join"></block>\n      <block type="text_append">\n        <value name="TEXT">\n          <shadow type="text"></shadow>\n        </value>\n      </block>\n      <block type="text_length">\n        <value name="VALUE">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_isEmpty">\n        <value name="VALUE">\n          <shadow type="text">\n            <field name="TEXT"></field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_indexOf">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{textVariable}</field>\n          </block>\n        </value>\n        <value name="FIND">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_charAt">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{textVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="text_getSubstring">\n        <value name="STRING">\n          <block type="variables_get">\n            <field name="VAR">{textVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="text_changeCase">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_trim">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_print">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="text_prompt_ext">\n        <value name="TEXT">\n          <shadow type="text">\n            <field name="TEXT">abc</field>\n          </shadow>\n        </value>\n      </block>\n    </category>\n    <category name="LISTS" colour="%{BKY_LISTS_HUE}">\n      <block type="lists_create_with">\n        <mutation items="0"></mutation>\n      </block>\n      <block type="lists_create_with"></block>\n      <block type="lists_repeat">\n        <value name="NUM">\n          <shadow type="math_number">\n            <field name="NUM">5</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="lists_length"></block>\n      <block type="lists_isEmpty"></block>\n      <block type="lists_indexOf">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="lists_getIndex">\n        <value name="VALUE">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="lists_setIndex">\n        <value name="LIST">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="lists_getSublist">\n        <value name="LIST">\n          <block type="variables_get">\n            <field name="VAR">{listVariable}</field>\n          </block>\n        </value>\n      </block>\n      <block type="indexer_R"></block>\n      <block type="doubleIndexer_R"></block>\n      <block type="lists_split">\n        <value name="DELIM">\n          <shadow type="text">\n            <field name="TEXT">,</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="lists_sort"></block>\n      <block type="uniqueBlock_R"></block>\n      <block type="reversedBlock_R"></block>\n      <block type="unlistBlock_R"></block>\n    </category>\n    <category name="COLOUR" colour="%{BKY_COLOUR_HUE}">\n      <block type="colour_picker"></block>\n      <block type="colour_random"></block>\n      <block type="colour_rgb">\n        <value name="RED">\n          <shadow type="math_number">\n            <field name="NUM">100</field>\n          </shadow>\n        </value>\n        <value name="GREEN">\n          <shadow type="math_number">\n            <field name="NUM">50</field>\n          </shadow>\n        </value>\n        <value name="BLUE">\n          <shadow type="math_number">\n            <field name="NUM">0</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="colour_blend">\n        <value name="COLOUR1">\n          <shadow type="colour_picker">\n            <field name="COLOUR">#ff0000</field>\n          </shadow>\n        </value>\n        <value name="COLOUR2">\n          <shadow type="colour_picker">\n            <field name="COLOUR">#3333ff</field>\n          </shadow>\n        </value>\n        <value name="RATIO">\n          <shadow type="math_number">\n            <field name="NUM">0.5</field>\n          </shadow>\n        </value>\n      </block>\n    </category>\n    <category name="CONVERSION" colour="120">\n      <block type="boolConversion_R">\n      </block>\n      <block type="intConversion_R">\n      </block>\n      <block type="floatConversion_R">\n      </block>\n      <block type="strConversion_R">\n      </block>\n    </category>\n    <category name="I/O" colour="190">\n      <block type="textFromFile_R">\n        <value name="FILENAME">\n          <shadow type="text">\n            <field name="TEXT">name of file</field>\n          </shadow>\n        </value>\n      </block>\n      <block type="readFile_R">\n        <value name="FILENAME">\n          <shadow type="text">\n            <field name="TEXT">name of file</field>\n          </shadow>\n        </value>\n      </block>\n    </category>\n    <sep></sep>\n    <category name="VARIABLES" colour="%{BKY_VARIABLES_HUE}" custom="VARIABLE"></category>\n    \x3c!-- TEMPORARILY DISABLED B/C OF PLUS/MINUS INCOMPATIBILITY <category name="FUNCTIONS" colour="%{BKY_PROCEDURES_HUE}" custom="PROCEDURE"></category> --\x3e\n    <category name="SPECIAL" colour="270" custom="SPECIAL"></category>\n  </xml>'
                     })), console.log("jupyterlab_blockly_extension_r: blockly palette initialized");
                     const t = t => {
-                        "create" === t.type && Y(e, !1), "finished_loading" === t.type && Y(e, !0)
+                        "create" === t.type && q(e, !1), "finished_loading" === t.type && q(e, !0)
                     };
-                    j(e).removeChangeListener(t), j(e).addChangeListener(t), j(e).registerToolboxCategoryCallback("SPECIAL", (e => {
+                    X(e).removeChangeListener(t), X(e).addChangeListener(t), X(e).registerToolboxCategoryCallback("SPECIAL", (e => {
                         const t = [],
                             n = document.createElement("label");
                         if (n.setAttribute("text", "Occassionally blocks appear here as you load libraries (e.g. %>%). See VARIABLES for most cases."), t.push(n), L.has("dplyr")) {
                             const e = document.createElement("block");
                             e.setAttribute("type", "pipe_R"), t.push(e)
                         }
                         if (L.has("ggplot2")) {
@@ -1228,193 +1242,193 @@
                     }))
                 }
                 onResize(e) {
                     let t, n;
                     const o = document.getElementById("blocklyDivR"),
                         l = document.getElementById("buttonDivR"),
                         a = e.height - 30;
-                    o.setAttribute("style", "position: absolute; top: 0px; left: 0px; width: " + (t = e.width, t.toString() + "px; height: ") + a.toString() + "px"), l.setAttribute("style", "position: absolute; top: " + a.toString() + "px; left: 0px; width: " + (n = e.width, n.toString() + "px; height: 30px")), i.svgResize(j(this))
+                    o.setAttribute("style", "position: absolute; top: 0px; left: 0px; width: " + (t = e.width, t.toString() + "px; height: ") + a.toString() + "px"), l.setAttribute("style", "position: absolute; top: " + a.toString() + "px; left: 0px; width: " + (n = e.width, n.toString() + "px; height: 30px")), i.svgResize(X(this))
                 }
             }
 
             function G(e, t) {
                 e["workspace@"] = t
             }
 
-            function j(e) {
+            function X(e) {
                 return e["workspace@"]
             }
 
-            function X(e) {
+            function H(e) {
                 return e.notebooks
             }
 
-            function H(e) {
-                return new P(e)
+            function Y(e) {
+                return new j(e)
             }
 
-            function Y(e, t) {
+            function q(e, t) {
                 e["blocksRendered@"] = t
             }
 
-            function q(e) {
+            function z(e) {
                 return e["blocksRendered@"]
             }
 
-            function z(e) {
+            function K(e) {
                 return e["notHooked@"]
             }
 
-            function K(e, t) {
+            function Q(e, t) {
                 e["notHooked@"] = t
             }
 
-            function Q(e) {
+            function Z(e) {
                 return e["lastCell@"]
             }
 
-            function Z(e, t) {
+            function $(e, t) {
                 e["lastCell@"] = t
             }
 
-            function $(e) {
-                return (e, t) => ("ir" === e.name && "execute_input" === t.header.msg_type.toString() && (console.log("jupyterlab_blockly_extension_r: kernel executed code, updating intellisense"), U()), !0)
+            function J(e) {
+                return (e, t) => ("ir" === e.name && "execute_input" === t.header.msg_type.toString() && (console.log("jupyterlab_blockly_extension_r: kernel executed code, updating intellisense"), w()), !0)
             }
 
-            function J(e) {
+            function ee(e) {
                 return (t, n) => {
                     if (n) {
                         const t = document.getElementById("syncCheckboxR"),
                             o = document.getElementById("autosaveCheckbox"),
                             l = e => !!e && e.checked;
-                        l(t) && e.notebooks.activeCell && (q(e) && null == ee(e) ? le() : ne(e), U()), l(o) && e.notebooks.activeCell && (oe(e), Z(e, n))
+                        l(t) && e.notebooks.activeCell && (z(e) && null == te(e) ? ie() : oe(e), w()), l(o) && e.notebooks.activeCell && (le(e), $(e, n))
                     }
                     return !0
                 }
             }
 
-            function ee(e) {
+            function te(e) {
                 if (e.notebooks.activeCell) {
                     const t = e.notebooks.activeCell.model.sharedModel.getSource();
                     if (!(t.indexOf("xmlns") >= 0)) return null;
                     {
                         const e = /(<xml[\s\S]+<\/xml>)/;
                         let n = t.match(e);
                         if (n && n[0]) return n[0]
                     }
                 }
                 return null
             }
 
-            function te(e) {
+            function ne(e) {
                 let t;
-                const n = e.generator.workspaceToCode(j(e));
-                e.notebooks.activeCell ? (t = e.notebooks.activeCell.model, c.isMarkdownCellModel(t) ? window.alert("You are calling 'Blocks to Code' on a MARKDOWN cell. Select an empty CODE cell and try again.") : (e.notebooks.activeCell.model.sharedModel.setSource(n + "\n#" + g()), console.log("jupyterlab_blockly_extension_r: wrote to active cell\n" + n + "\n"), Y(e, !0))) : console.log("jupyterlab_blockly_extension_r: no cell active, flushed\n" + n + "\n")
+                const n = e.generator.workspaceToCode(X(e));
+                e.notebooks.activeCell ? (t = e.notebooks.activeCell.model, c.isMarkdownCellModel(t) ? window.alert("You are calling 'Blocks to Code' on a MARKDOWN cell. Select an empty CODE cell and try again.") : (e.notebooks.activeCell.model.sharedModel.setSource(n + "\n#" + g()), console.log("jupyterlab_blockly_extension_r: wrote to active cell\n" + n + "\n"), q(e, !0))) : console.log("jupyterlab_blockly_extension_r: no cell active, flushed\n" + n + "\n")
             }
 
-            function ne(e) {
+            function oe(e) {
                 if (e.notebooks.activeCell) {
                     const t = /(<xml[\s\S]+<\/xml>)/;
                     let n = e.notebooks.activeCell.model.sharedModel.getSource().match(t);
                     try {
                         if (n && n[1]) {
                             const e = n[1];
-                            le(),
+                            ie(),
                                 function(e) {
                                     const t = (new DOMParser).parseFromString(e, "application/xml").documentElement;
                                     d.Xml.domToWorkspace(t, d.getMainWorkspace())
                                 }(e)
                         }
                     } catch (e) {
                         window.alert("Unable to perform 'Code to Blocks': XML is either invald or renames existing variables. Specific error message is: " + e.message), console.log("jupyterlab_blockly_extension_r: unable to decode blocks, last line is invald xml")
                     }
                 } else console.log("jupyterlab_blockly_extension_r: unable to decode blocks, active cell is null")
             }
 
-            function oe(e) {
+            function le(e) {
                 let t;
-                const n = e.generator.workspaceToCode(j(e));
-                Q(e) ? Q(e).model && (t = Q(e).model, c.isCodeCellModel(t) && (() => {
+                const n = e.generator.workspaceToCode(X(e));
+                Z(e) ? Z(e).model && (t = Z(e).model, c.isCodeCellModel(t) && (() => {
                     try {
-                        const t = Q(e).model.sharedModel.getSource();
+                        const t = Z(e).model.sharedModel.getSource();
                         if (t.indexOf("xmlns") >= 0) {
                             const e = /(<xml[\s\S]+<\/xml>)/;
                             let n = t.match(e);
                             if (n && n[0]) return n[0]
                         }
                     } catch (e) {
                         return !1
                     }
-                })()) && j(e).getAllBlocks(!1).length > 0 && (Q(e).model.sharedModel.setSource(n + "\n#" + g()), console.log("jupyterlab_blockly_extension_r: wrote to active cell\n" + n + "\n")) : console.log("jupyterlab_blockly_extension_r: no cell active, flushed instead of autosave\n" + n + "\n")
+                })()) && X(e).getAllBlocks(!1).length > 0 && (Z(e).model.sharedModel.setSource(n + "\n#" + g()), console.log("jupyterlab_blockly_extension_r: wrote to active cell\n" + n + "\n")) : console.log("jupyterlab_blockly_extension_r: no cell active, flushed instead of autosave\n" + n + "\n")
             }
 
-            function le(e) {
+            function ie(e) {
                 const t = i.getMainWorkspace().getAllBlocks(!1);
                 for (let e = 0; e < t.length; e++) t[e].dispose(!1)
             }
 
-            function ie(e) {
+            function ae(e) {
                 const t = new a.MainAreaWidget({
                     content: e
                 });
                 return t.id = "blockly-jupyterlab-r", t.title.label = "Blockly R", t.title.closable = !0, t
             }
 
-            function ae(e, t, n) {
+            function se(e, t, n) {
                 if (!n.isAttached) {
                     const o = t.currentWidget;
                     if (null == o) e.shell.add(n, "main");
                     else {
                         const e = o,
                             t = {
                                 ref: e.id,
                                 mode: "split-left"
                             };
                         e.context.addSibling(n, t)
                     }
                 }
                 e.shell.activateById(n.id)
             }
-            const se = function(e, t) {
+            const re = function(e, t) {
                 return null == e.currentWidget || (console.log("jupyterlab_blockly_extension_r: notebook changed, autorunning blockly r command"), this.commands.execute("blockly_r:open")), !0
             };
 
-            function re(e, t) {
+            function ce(e, t) {
                 var n;
                 const o = this;
-                if (z(o)) {
+                if (K(o)) {
                     const t = null === (n = e.session) || void 0 === n ? void 0 : n.kernel;
                     if (null == t || null == t);
                     else {
                         const e = t;
-                        "ir" === e.name && (e.iopubMessage.connect($(), o), console.log("jupyterlab_blockly_extension_r: Listening for kernel messages"), K(o, !1))
+                        "ir" === e.name && (e.iopubMessage.connect(J(), o), console.log("jupyterlab_blockly_extension_r: Listening for kernel messages"), Q(o, !1))
                     }
                     return !0
                 }
                 return !1
             }
 
-            function ce(e, t) {
+            function ue(e, t) {
                 const n = this,
                     o = e.currentWidget;
                 if (null == o);
                 else {
                     const e = o;
-                    console.log("jupyterlab_blockly_extension_r: notebook changed to " + e.context.path), e.sessionContext.kernelChanged.connect(re, n)
+                    console.log("jupyterlab_blockly_extension_r: notebook changed to " + e.context.path), e.sessionContext.kernelChanged.connect(ce, n)
                 }
                 return !0
             }
-            const ue = {
+            const de = {
                 id: "jupyterlab_blockly_extension_r",
                 autoStart: !0,
                 requires: [a.ICommandPalette, r.INotebookTracker, o.ILayoutRestorer, s.IStateDB],
                 activate: (e, t, n, o, l) => {
                     console.log("jupyterlab_blockly_extension_r: activated");
-                    const i = H(n);
-                    let s = ie(i);
+                    const i = Y(n);
+                    let s = ae(i);
                     const r = new a.WidgetTracker({
                         namespace: "blockly_r"
                     });
                     o && o.restore(r, {
                         command: "blockly_r:open",
                         name: () => "blockly_r"
                     }), e.restored.then((() => l.fetch("jupyterlab_blockly_extension_r:intellisense-cache").then((e => {
@@ -1425,28 +1439,28 @@
                             const n = Object.keys(t);
                             for (let e = 0; e <= n.length - 1; e++) {
                                 const t = n[e];
                                 console.log(t)
                             }
                             n.length, console.log("...done")
                         }
-                    })))), n.currentChanged.connect(ce, i), e.commands.addCommand("blockly_r:open", {
+                    })))), n.currentChanged.connect(ue, i), e.commands.addCommand("blockly_r:open", {
                         label: "Blockly R",
                         execute: () => {
-                            s && !s.isDisposed || (s = ie(i)), ae(e, n, s), r.has(s) || r.add(s)
+                            s && !s.isDisposed || (s = ae(i)), se(e, n, s), r.has(s) || r.add(s)
                         }
                     }), t.addItem({
                         command: "blockly_r:open",
                         category: "Blockly"
                     });
                     const c = new URLSearchParams(window.location.search),
                         u = c.get("bl");
                     let d;
                     d = u && "r" === u ? 0 : 1, 0 === d && (console.log("jupyterlab_blockly_extension_r: triggering open command based on query string input"), e.restored.then((() => {
-                        n.currentChanged.connect(se, e), s.title.closable = !1
+                        n.currentChanged.connect(re, e), s.title.closable = !1
                     })));
                     const _ = c.get("log"),
                         E = c.get("logr");
                     let R;
                     R = _ && E && "1" === E ? 0 : 1
                 }
             }
```

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/983.e6daa4ad1ba05ddae851.js` & `aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/983.e6daa4ad1ba05ddae851.js`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/remoteEntry.b9292539421da221e3e6.js` & `aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/remoteEntry.ea69d1a6ef05a0944e0d.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, f, s, d, p, c, h, v, b, y, m, g, j, w, k, S, x = {
+    var e, r, t, n, o, a, i, l, u, s, f, d, p, c, h, v, b, y, m, g, j, w, k, S, x = {
             193: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(983), t.e(978)]).then((() => () => t(978))),
                         "./extension": () => Promise.all([t.e(983), t.e(978)]).then((() => () => t(978))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -43,39 +43,39 @@
         }), r
     }, P.d = (e, r) => {
         for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
-        369: "02184f958ba98de69fb9",
+        369: "33cb3b39acb33feedba2",
         728: "fab96543eb438ca8425a",
-        978: "4bc44e871dcb20252e08",
+        978: "503c08dddbdbe0d6b639",
         983: "e6daa4ad1ba05ddae851"
     } [e] + ".js?v=" + {
-        369: "02184f958ba98de69fb9",
+        369: "33cb3b39acb33feedba2",
         728: "fab96543eb438ca8425a",
-        978: "4bc44e871dcb20252e08",
+        978: "503c08dddbdbe0d6b639",
         983: "e6daa4ad1ba05ddae851"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@aolney/jupyterlab-blockly-r-extension:", P.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
+                    var f = u[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
@@ -111,15 +111,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@aolney/jupyterlab-blockly-r-extension", "0.1.1", (() => Promise.all([P.e(983), P.e(978)]).then((() => () => P(978))))), l("blockly", "10.4.3", (() => Promise.all([P.e(983), P.e(369)]).then((() => () => P(369)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@aolney/jupyterlab-blockly-r-extension", "0.1.2", (() => Promise.all([P.e(983), P.e(978)]).then((() => () => P(978))))), l("blockly", "10.4.3", (() => Promise.all([P.e(983), P.e(369)]).then((() => () => P(369)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -169,31 +169,31 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > n && !o : "" == d != o);
-                if ("u" == s) {
+                var s, f, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !u || ("u" == d ? l > n && !o : "" == d != o);
+                if ("u" == f) {
                     if (!u || "u" != d) return !1
                 } else if (u)
-                    if (d == s)
+                    if (d == f)
                         if (l <= n) {
-                            if (f != e[l]) return !1
+                            if (s != e[l]) return !1
                         } else {
-                            if (o ? f > e[l] : f < e[l]) return !1;
-                            f != e[l] && (u = !1)
+                            if (o ? s > e[l] : s < e[l]) return !1;
+                            s != e[l] && (u = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < d != o) return !1;
+                    if (l <= n || f < d != o) return !1;
                     u = !1
                 } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
@@ -207,44 +207,44 @@
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || c(f(e, t, o, n)), v(e[t][o])
+        return a(n, o) || c(s(e, t, o, n)), v(e[t][o])
     }, d = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, p = (e, r, t, n) => {
         var a = e[t];
         return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = (e, r, t, n) => {
         c(p(e, r, t, n))
     }, v = e => (e.loaded = 1, e.get()), y = (b = e => function(r, t, n, o) {
         var a = P.I(r);
         return a && a.then ? a.then(e.bind(e, r, P.S[r], t, n, o)) : e(r, P.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), v(d(r, t, n) || h(r, e, t, n) || l(r, t))))), m = b(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (i(e, t), v(d(r, t, n) || h(r, e, t, n) || l(r, t))))), m = b(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
         var a = r && P.o(r, t) && d(r, t, n);
         return a ? v(a) : o()
     })), j = {}, w = {
         256: () => m("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        315: () => y("default", "@jupyterlab/cells", [1, 4, 1, 6]),
-        372: () => m("default", "@jupyterlab/notebook", [1, 4, 1, 6]),
-        465: () => m("default", "@jupyterlab/application", [1, 4, 1, 6]),
+        371: () => m("default", "@jupyterlab/application", [1, 4, 1, 8]),
+        385: () => y("default", "@jupyterlab/cells", [1, 4, 1, 8]),
+        440: () => m("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
+        506: () => m("default", "@jupyterlab/notebook", [1, 4, 1, 8]),
         569: () => g("default", "blockly", [1, 10, 4, 3], (() => P.e(369).then((() => () => P(369))))),
-        638: () => m("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
-        723: () => m("default", "@jupyterlab/rendermime", [1, 4, 1, 6]),
-        750: () => m("default", "@jupyterlab/statedb", [1, 4, 1, 6])
+        574: () => m("default", "@jupyterlab/rendermime", [1, 4, 1, 8]),
+        824: () => m("default", "@jupyterlab/statedb", [1, 4, 1, 8])
     }, k = {
-        978: [256, 315, 372, 465, 569, 638, 723, 750]
+        978: [256, 371, 385, 440, 506, 569, 574, 824]
     }, S = {}, P.f.consumes = (e, r) => {
         P.o(k, e) && k[e].forEach((e => {
             if (P.o(j, e)) return r.push(j[e]);
             if (!S[e]) {
                 var t = r => {
                     j[e] = 0, P.m[e] = t => {
                         delete P.c[e], t.exports = r()
```

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/aolney_jupyterlab_blockly_r_extension/labextension/static/third-party-licenses.json` & `aolney_jupyterlab_blockly_r_extension-0.1.2/aolney_jupyterlab_blockly_r_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/src/RGenerator.ts` & `aolney_jupyterlab_blockly_r_extension-0.1.2/src/RGenerator.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/src/SearchDropdown.ts` & `aolney_jupyterlab_blockly_r_extension-0.1.2/src/SearchDropdown.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/src/Toolbox.ts` & `aolney_jupyterlab_blockly_r_extension-0.1.2/src/Toolbox.ts`

 * *Files 2% similar despite different names*

```diff
@@ -427,27 +427,27 @@
     return Promise.reject((() => {
       throw 1;
     })());
   }
   else {
     const kernel: Kernel.IKernelConnection = matchValue[1];
     return new Promise<string[]>((resolve, reject) => {
-      setTimeout(() => {
+      // setTimeout(() => {
         kernel.requestComplete({
           code: queryString,
           cursor_pos: queryString.length,
         }).then((_arg: KernelMessage.ICompleteReplyMsg) => {
           const content = _arg.content;
           if ('matches' in content) {
             resolve(content.matches.slice());
           }
         }).catch((_arg_1: Error) => {
           reject([queryString + " is unavailable"]);
         });
-      }, 100);
+      // }, 100);
     });
   }
 }
 
 // requestInspectTimeout, not used
 
 
@@ -474,14 +474,15 @@
           const payload = content.data;
           const model: MimeModel = new rendermime.MimeModel({
             data: payload,
           });
           if(mimeType){
             const renderer: IRenderMime.IRenderer = widget.content.rendermime.createRenderer(mimeType);
             renderer.renderModel(model).then(() => {
+              // console.log("debug: kernel inspected " + queryString) //for debug only
               resolve(renderer.node.innerText);
             }).catch((error: any) => {
               console.log(queryString + ":RENDER_ERROR");
               reject(error);
             });
           }
         } else {
@@ -516,22 +517,35 @@
 
 /**
  * Determine if an entry is a function. We have separate blocks for properties and functions because only function blocks need parameters
  * This is a bit weird for R; not sure about standardization of this information
  * We need some special handling for cases like dplyr %>%, which is surrounded in backticks
  */
 export function isFunction_R(query: string, info: string): boolean {
-  if (query.indexOf("`") === 0) {
+  // for %>% and other backticked functions
+  if (query.startsWith("`")) {
       return true;
   }
-  else if (info.indexOf("Class attribute:\n\'function\'") >= 0) {
+  // indicates it takes parameters
+  else if (info.includes( query + "(") ) {
+    return true;
+  }
+  // explicit marking of function in documentation
+  else if (info.includes("Class attribute:\n\'function\'") ) {
+      return true;
+  }
+  else if (info.includes("Usage") && info.includes("Arguments")) {
       return true;
   }
-  else if (info.indexOf("Usage") >= 0) {
-      return info.indexOf("Arguments") >= 0;
+  // look for words that otherwise indicate functionhood. These matchers might be too aggressive; hard to say since R is mostly functions
+  else if (info.includes("function") || info.includes("Function")) {
+    return true;
+  }
+  else if (info.includes("object") || info.includes("Object")) {
+    return true;
   }
   else {
       return false;
   }
 }
 
 /**
@@ -546,74 +560,129 @@
   if (dict.has(k)) {
     throw new Error("An item with the same key has already been added. Key: " + k);
   }
   dict.set(k, v);
 }
 
 /**
+ * Fire intellisense event that causes Blockly to refresh intellisense-driven options
+ * Typically called by RequestIntellisenseVariable 
+ * @param block 
+ */
+export function fireIntellisenseEvent(block: Blockly.Block) {
+  try {
+  // Create event on this block
+  const intellisenseUpdateEvent = new Blockly.Events.BlockChange(block, "field", "VAR", 0, 1);
+  // Set the event group; this allows event listners to focus on only relevant messages
+  intellisenseUpdateEvent.group = "INTELLISENSE";
+  // Do some state tracking; this helps with debugging events
+  // @ts-ignore
+  console.log("event status is " + Blockly.Events.disabled_); //disabled_ existed in old version but not new version?
+  // @ts-ignore
+  Blockly.Events.disabled_ = 0;
+  Blockly.Events.fire(intellisenseUpdateEvent);
+  } 
+  catch(e){
+    if (e instanceof Error) {
+      console.log("Intellisense event failed to fire; " + e.message);
+    }
+  }
+}
+
+/**
+ * Wrap a promise inside another with a timeout in milliseconds
+ * https://github.com/JakeChampion/fetch/issues/175#issuecomment-216791333
+ * @param ms 
+ * @param promise 
+ * @returns 
+ */
+export function timeoutPromise<T>(ms: number, promise: Promise<T>) {
+  return new Promise<T>((resolve, reject) => {
+    const timeoutId = setTimeout(() => {
+      reject(new Error("promise timeout"))
+    }, ms);
+    promise.then(
+      (res) => {
+        clearTimeout(timeoutId);
+        resolve(res);
+      },
+      (err) => {
+        clearTimeout(timeoutId);
+        reject(err);
+      }
+    );
+  })
+}
+
+/**
  * Request an IntellisenseVariable. If the type does not descend from object, the children will be empty.
  * Sometimes we will create a variable but it will have no type until we make an assignment.
  * We might also create a variable and then change its type.
  * So we need to check for introspections/completions repeatedly (no caching right now).
  */
 export function RequestIntellisenseVariable_R(block: Blockly.Block, parentName: string): void {
   GetKernalInspection(parentName).then((parentInspection: string) => {
+    // Package the parent inspection 
     const parent: IntellisenseEntry = new IntellisenseEntry(parentName, parentInspection, isFunction_R(parentName, parentInspection), isClass_R(parentInspection));
-    let shouldGetChildren: boolean;
-    let outArg: IntellisenseVariable = new IntellisenseVariable(parent, []);
-    const matchValue: [boolean, IntellisenseVariable] = [
-      intellisenseLookup.has(parent.Name),
-      outArg
-    ];
-    if (matchValue[0]) {
-      const cached: IntellisenseVariable = matchValue[1];
-      if (cached.VariableEntry.Info !== parent.Info || cached.ChildEntries.length === 0) {
+    // Assume we need to get children
+    let shouldGetChildren: boolean = true;
+    // Check the cache to see if we have found children before
+    let cached: IntellisenseVariable | undefined = intellisenseLookup.get(parent.Name);
+    if( cached ) {
+      // Even if we have a cached variable, update it if the parent Info does not match or if child entries is short
+      if (cached.VariableEntry.Info !== parent.Info || cached.ChildEntries.length <= 1) {
         shouldGetChildren = true;
+      // Only avoid getting children if the cached variable looks good
       } else {
         shouldGetChildren = false;
       }
-    } else {
-      shouldGetChildren = true;
     }
-    if (shouldGetChildren) {
-      GetKernelCompletion(parentName + "::").then((completions: string[]) => {
-        const pr: Promise<string>[] = completions.map((completion: string) => GetKernalInspection(completion));
-        return Promise.all(pr).then((inspections: string[]) => {
-          const intellisenseVariable: IntellisenseVariable = new IntellisenseVariable(parent, completions.map((completion: string, index: number) => {
-            const childName: string = completion.replace(new RegExp(parentName + "::"), "");
-            return new IntellisenseEntry(childName, inspections[index], isFunction_R(childName, inspections[index]), isClass_R(inspections[index]));
-          }));
-          if (intellisenseLookup.has(parentName)) {
-            intellisenseLookup.set(parentName, intellisenseVariable);
-          } else {
-            addToDict(intellisenseLookup, parentName, intellisenseVariable);
-          }
-          const intellisenseUpdateEvent = new Blockly.Events.BlockChange(block, "field", "VAR", 0, 1);
-          intellisenseUpdateEvent.group = "INTELLISENSE";
-          // @ts-ignore
-          console.log("event status is " + Blockly.Events.disabled_); //disabled_ existed in old version but not new version?
-          // @ts-ignore
-          Blockly.Events.disabled_ = 0;
-          Blockly.Events.fire(intellisenseUpdateEvent);
+    
+    if (!shouldGetChildren) {
+      console.log("Not refreshing intellisense for " + parent.Name);
+      // Trigger update intellisense even if we are cached (this could be reconsidered, but original code does this)
+      fireIntellisenseEvent(block)
+    } else {
+      // Get children by prefixing on parent's name (package completions)
+      GetKernelCompletion(parentName + "::").then((childCompletions: string[]) => {
+        // Set up inspections for all children; use a timeout promise so we don't wait forever; make timeout dynamic based on which child this is (assumes serial bottleneck at kernel)
+        const pr: Promise<string>[] = childCompletions.map((childCompletion: string, index: number) => timeoutPromise<string>( 100 * (index+1) , GetKernalInspection(childCompletion)) );
+        // Synchronize on inspections to yield the final result
+        Promise.allSettled(pr).then((results : PromiseSettledResult<string>[]) => {
+          // Create an intellisense entries for children, sorted alphabetically
+          let children: IntellisenseEntry[] = childCompletions.map((childCompletion: string, index: number) => {
+            const childName: string = childCompletion.replace(new RegExp(parentName + "::"), "");
+            let info = "";
+            let isFunction = true;
+            let isClass = false;
+            if( results[index].status === "fulfilled") {
+              info = (results[index] as PromiseFulfilledResult<string>).value;
+              isFunction = isFunction_R(childName, info);
+              isClass = isClass_R(info);
+            } 
+            return new IntellisenseEntry(childName, info, isFunction, isClass)}).sort((a, b) => (a.Name < b.Name ? -1 : 1));
+          // Package up IntellisenseVariable (parent + children)
+          let intellisenseVariable: IntellisenseVariable = new IntellisenseVariable(parent, children);
+          // Add to cache
+          intellisenseLookup.set(parentName, intellisenseVariable);
+
+          // Fire event; this causes Blockly to refresh
+          fireIntellisenseEvent(block);
         }).catch(error => {
-          console.log("Error resolving promises:", error);
+          console.log("Intellisense error getting inspections for children of " + parentName, error);
         });
       }).catch(error => {
-        console.log("Error getting completions:", error);
+        console.log("Intellisense error getting child completions of " + parentName, error);
       });
-    } else {
-      console.log("Not refreshing intellisense for " + parent.Name);
     }
-  }).catch((error: Error) => {
-    console.log("Intellisense event failed to fire; " + error.message);
+  }).catch((error) => {
+    console.log("Intellisense error getting inspection of intellisense variable candidate (parent) " + parentName, error);
   });
 }
 
-
-
 export function requestAndStubOptions_R(block: Blockly.Block, varName: string): string[][] {
   if ((varName !== "") && !block.isInFlyout) {
     RequestIntellisenseVariable_R(block, varName);
   }
   if (block.isInFlyout) {
     return [[" ", " "]];
   }
```

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/src/field_minus.ts` & `aolney_jupyterlab_blockly_r_extension-0.1.2/src/field_minus.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/src/field_plus.ts` & `aolney_jupyterlab_blockly_r_extension-0.1.2/src/field_plus.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/src/index.ts` & `aolney_jupyterlab_blockly_r_extension-0.1.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/src/logging.ts` & `aolney_jupyterlab_blockly_r_extension-0.1.2/src/logging.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/ui-tests/README.md` & `aolney_jupyterlab_blockly_r_extension-0.1.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/ui-tests/tests/aolney_jupyterlab_blockly_r_extension.spec.ts` & `aolney_jupyterlab_blockly_r_extension-0.1.2/ui-tests/tests/aolney_jupyterlab_blockly_r_extension.spec.ts`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/.gitignore` & `aolney_jupyterlab_blockly_r_extension-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/LICENSE` & `aolney_jupyterlab_blockly_r_extension-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/README.md` & `aolney_jupyterlab_blockly_r_extension-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/pyproject.toml` & `aolney_jupyterlab_blockly_r_extension-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aolney_jupyterlab_blockly_r_extension-0.1.1/PKG-INFO` & `aolney_jupyterlab_blockly_r_extension-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aolney_jupyterlab_blockly_r_extension
-Version: 0.1.1
+Version: 0.1.2
 Dynamic: Keywords
 Summary: A JupyterLab extension that creates a Blockly palette for R.
 Project-URL: Homepage, https://github.com/aolney/jupyterlab-blockly-r-extension
 Project-URL: Bug Tracker, https://github.com/aolney/jupyterlab-blockly-r-extension/issues
 Project-URL: Repository, https://github.com/aolney/jupyterlab-blockly-r-extension.git
 Author-email: "Andrew M. Olney" <aolney@memphis.edu>
 License:                                  Apache License
```

