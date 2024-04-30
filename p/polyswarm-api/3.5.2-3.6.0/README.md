# Comparing `tmp/polyswarm-api-3.5.2.tar.gz` & `tmp/polyswarm-api-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyswarm-api-3.5.2.tar", last modified: Wed Feb 21 21:51:20 2024, max compression
+gzip compressed data, was "polyswarm-api-3.6.0.tar", last modified: Tue Apr 30 21:23:23 2024, max compression
```

## Comparing `polyswarm-api-3.5.2.tar` & `polyswarm-api-3.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 21:51:20.032128 polyswarm-api-3.5.2/
--rw-rw-rw-   0 root         (0) root         (0)     1064 2024-02-21 21:50:54.000000 polyswarm-api-3.5.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-02-21 21:50:54.000000 polyswarm-api-3.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1615 2024-02-21 21:51:20.032128 polyswarm-api-3.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      951 2024-02-21 21:50:54.000000 polyswarm-api-3.5.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-02-21 21:50:54.000000 polyswarm-api-3.5.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-21 21:51:20.032128 polyswarm-api-3.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1292 2024-02-21 21:50:54.000000 polyswarm-api-3.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 21:51:20.028128 polyswarm-api-3.5.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 21:51:20.032128 polyswarm-api-3.5.2/src/polyswarm_api/
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-02-21 21:50:54.000000 polyswarm-api-3.5.2/src/polyswarm_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    37806 2024-02-21 21:50:54.000000 polyswarm-api-3.5.2/src/polyswarm_api/api.py
--rw-rw-rw-   0 root         (0) root         (0)    20066 2024-02-21 21:50:54.000000 polyswarm-api-3.5.2/src/polyswarm_api/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2024-02-21 21:50:54.000000 polyswarm-api-3.5.2/src/polyswarm_api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    41397 2024-02-21 21:50:54.000000 polyswarm-api-3.5.2/src/polyswarm_api/resources.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2024-02-21 21:50:54.000000 polyswarm-api-3.5.2/src/polyswarm_api/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 21:51:20.032128 polyswarm-api-3.5.2/src/polyswarm_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1615 2024-02-21 21:51:19.000000 polyswarm-api-3.5.2/src/polyswarm_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2024-02-21 21:51:20.000000 polyswarm-api-3.5.2/src/polyswarm_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 21:51:19.000000 polyswarm-api-3.5.2/src/polyswarm_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2024-02-21 21:51:19.000000 polyswarm-api-3.5.2/src/polyswarm_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-02-21 21:51:20.000000 polyswarm-api-3.5.2/src/polyswarm_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:23:23.441932 polyswarm-api-3.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2024-04-30 21:23:06.000000 polyswarm-api-3.6.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-30 21:23:06.000000 polyswarm-api-3.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-30 21:23:23.441932 polyswarm-api-3.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      951 2024-04-30 21:23:06.000000 polyswarm-api-3.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-04-30 21:23:06.000000 polyswarm-api-3.6.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 21:23:23.441932 polyswarm-api-3.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2024-04-30 21:23:06.000000 polyswarm-api-3.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:23:23.437932 polyswarm-api-3.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:23:23.437932 polyswarm-api-3.6.0/src/polyswarm_api/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-04-30 21:23:06.000000 polyswarm-api-3.6.0/src/polyswarm_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37884 2024-04-30 21:23:06.000000 polyswarm-api-3.6.0/src/polyswarm_api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20066 2024-04-30 21:23:06.000000 polyswarm-api-3.6.0/src/polyswarm_api/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2024-04-30 21:23:06.000000 polyswarm-api-3.6.0/src/polyswarm_api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    41506 2024-04-30 21:23:06.000000 polyswarm-api-3.6.0/src/polyswarm_api/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2024-04-30 21:23:06.000000 polyswarm-api-3.6.0/src/polyswarm_api/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 21:23:23.441932 polyswarm-api-3.6.0/src/polyswarm_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-30 21:23:23.000000 polyswarm-api-3.6.0/src/polyswarm_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-30 21:23:23.000000 polyswarm-api-3.6.0/src/polyswarm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 21:23:23.000000 polyswarm-api-3.6.0/src/polyswarm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-30 21:23:23.000000 polyswarm-api-3.6.0/src/polyswarm_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-30 21:23:23.000000 polyswarm-api-3.6.0/src/polyswarm_api.egg-info/top_level.txt
```

### Comparing `polyswarm-api-3.5.2/LICENSE` & `polyswarm-api-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.5.2/PKG-INFO` & `polyswarm-api-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm-api
-Version: 3.5.2
+Version: 3.6.0
 Summary: Client library to simplify interacting with the PolySwarm consumer API
 Home-page: https://github.com/polyswarm/polyswarm-api
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `polyswarm-api-3.5.2/README.md` & `polyswarm-api-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.5.2/setup.py` & `polyswarm-api-3.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # The README.md will be used as the content for the PyPi package details page on the Python Package Index.
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 
 setup(
     name='polyswarm-api',
-    version='3.5.2',
+    version='3.6.0',
     description='Client library to simplify interacting with the PolySwarm consumer API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='PolySwarm Developers',
     author_email='info@polyswarm.io',
     url='https://github.com/polyswarm/polyswarm-api',
     license='MIT',
```

### Comparing `polyswarm-api-3.5.2/src/polyswarm_api/api.py` & `polyswarm-api-3.6.0/src/polyswarm_api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         if isinstance(artifact, resources.LocalArtifact):
             instance = resources.ArtifactInstance.create(self,
                                                          artifact_name=artifact.artifact_name,
                                                          artifact_type=artifact.artifact_type.name,
                                                          scan_config=scan_config,
                                                          community=self.community).result()
             instance.upload_file(artifact)
-            return resources.ArtifactInstance.update(self, id=instance.id).result()
+            return resources.ArtifactInstance.update(self, id=instance.id, community=self.community).result()
         else:
             raise exceptions.InvalidValueException('Artifacts should be a path to a file or a LocalArtifact instance')
 
     def lookup(self, scan):
         """
         Lookup a scan by Scan id.
 
@@ -712,15 +712,15 @@
                                                      artifact_name=artifact.artifact_name,
                                                      artifact_type=artifact.artifact_type.name,
                                                      community=self.community,
                                                      provider_slug=provider_slug,
                                                      vm_slug=vm_slug,
                                                      network_enabled=network_enabled).result()
             task.upload_file(artifact)
-            return resources.SandboxTask.update_file(self, id=task.id).result()
+            return resources.SandboxTask.update_file(self, id=task.id, community=self.community).result()
         else:
             raise exceptions.InvalidValueException(
                 'Artifacts should be a path to a file or a LocalArtifact instance')
 
     def sandbox_url(self, url, provider_slug, vm_slug, browser=None):
         logger.info('Sandboxing url in provider %s vm %s', provider_slug, vm_slug)
         artifact = resources.LocalArtifact.from_content(self, url, artifact_name=url, artifact_type='URL')
@@ -729,15 +729,15 @@
                                                  artifact_type="URL",
                                                  community=self.community,
                                                  provider_slug=provider_slug,
                                                  vm_slug=vm_slug,
                                                  browser=browser,
                                                  network_enabled=True).result()
         task.upload_file(artifact)
-        return resources.SandboxTask.update_file(self, id=task.id).result()
+        return resources.SandboxTask.update_file(self, id=task.id, community=self.community).result()
 
     def sandbox_providers(self):
         """
         List sandboxes available in polyswarm.
         """
         logger.info('Listing sandbox names')
         return resources.SandboxProvider.list(self)
```

### Comparing `polyswarm-api-3.5.2/src/polyswarm_api/core.py` & `polyswarm-api-3.6.0/src/polyswarm_api/core.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.5.2/src/polyswarm_api/exceptions.py` & `polyswarm-api-3.6.0/src/polyswarm_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.5.2/src/polyswarm_api/resources.py` & `polyswarm-api-3.6.0/src/polyswarm_api/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,18 @@
         self.failed = content.get('failed')
         self.filename = content.get('filename')
         self.result = content.get('result')
         self.type = content.get('type')
         self.votes = [Vote(v, api=api, scanfile=self) for v in content.get('votes', [])]
         self.window_closed = content.get('window_closed')
         self.polyscore = float(content['polyscore']) if content.get('polyscore') is not None else None
-        self.permalink = settings.DEFAULT_PERMALINK_BASE + '/' + str(self.hash) + '/' + str(self.id)
+        if content.get('permalink'):
+            self.permalink = content.get('permalink')
+        else:
+            self.permalink = settings.DEFAULT_PERMALINK_BASE + '/' + str(self.hash) + '/' + str(self.id)
 
         self._malicious_assertions = None
         self._benign_assertions = None
         self._valid_assertions = None
 
     def upload_file(self, artifact, attempts=3, **kwargs):
         if not self.upload_url:
```

### Comparing `polyswarm-api-3.5.2/src/polyswarm_api/settings.py` & `polyswarm-api-3.6.0/src/polyswarm_api/settings.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.5.2/src/polyswarm_api.egg-info/PKG-INFO` & `polyswarm-api-3.6.0/src/polyswarm_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm-api
-Version: 3.5.2
+Version: 3.6.0
 Summary: Client library to simplify interacting with the PolySwarm consumer API
 Home-page: https://github.com/polyswarm/polyswarm-api
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

