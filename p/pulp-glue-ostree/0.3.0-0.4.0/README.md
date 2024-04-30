# Comparing `tmp/pulp-glue-ostree-0.3.0.tar.gz` & `tmp/pulp-glue-ostree-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-ostree-0.3.0.tar", last modified: Tue Apr 23 17:35:29 2024, max compression
+gzip compressed data, was "pulp-glue-ostree-0.4.0.tar", last modified: Tue Apr 30 13:13:54 2024, max compression
```

## Comparing `pulp-glue-ostree-0.3.0.tar` & `pulp-glue-ostree-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 17:35:17.000000 pulp-glue-ostree-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/pulp_glue/ostree/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 17:35:17.000000 pulp-glue-ostree-0.3.0/pulp_glue/ostree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-23 17:35:17.000000 pulp-glue-ostree-0.3.0/pulp_glue/ostree/context.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:17.000000 pulp-glue-ostree-0.3.0/pulp_glue/ostree/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-23 17:35:29.000000 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-23 17:35:29.000000 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:35:29.000000 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 17:35:29.000000 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 17:35:29.000000 pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-23 17:35:17.000000 pulp-glue-ostree-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:35:29.827659 pulp-glue-ostree-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:13:54.212092 pulp-glue-ostree-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 13:13:54.212092 pulp-glue-ostree-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 13:13:45.000000 pulp-glue-ostree-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:13:54.212092 pulp-glue-ostree-0.4.0/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:13:54.212092 pulp-glue-ostree-0.4.0/pulp_glue/ostree/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 13:13:45.000000 pulp-glue-ostree-0.4.0/pulp_glue/ostree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-30 13:13:45.000000 pulp-glue-ostree-0.4.0/pulp_glue/ostree/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:13:45.000000 pulp-glue-ostree-0.4.0/pulp_glue/ostree/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:13:54.212092 pulp-glue-ostree-0.4.0/pulp_glue_ostree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 13:13:54.000000 pulp-glue-ostree-0.4.0/pulp_glue_ostree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-30 13:13:54.000000 pulp-glue-ostree-0.4.0/pulp_glue_ostree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:13:54.000000 pulp-glue-ostree-0.4.0/pulp_glue_ostree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 13:13:54.000000 pulp-glue-ostree-0.4.0/pulp_glue_ostree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 13:13:54.000000 pulp-glue-ostree-0.4.0/pulp_glue_ostree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-30 13:13:45.000000 pulp-glue-ostree-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:13:54.212092 pulp-glue-ostree-0.4.0/setup.cfg
```

### Comparing `pulp-glue-ostree-0.3.0/PKG-INFO` & `pulp-glue-ostree-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue-ostree
-Version: 0.3.0
+Version: 0.4.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API. (OSTree plugin)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-ostree
 Project-URL: changelog, https://github.com/pulp/pulp-cli-ostree/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-ostree-0.3.0/pulp_glue/ostree/context.py` & `pulp-glue-ostree-0.4.0/pulp_glue/ostree/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,82 +5,95 @@
     EntityDefinition,
     PluginRequirement,
     PulpContentContext,
     PulpEntityContext,
     PulpRemoteContext,
     PulpRepositoryContext,
     PulpRepositoryVersionContext,
-    registered_repository_contexts,
 )
 
 
 class PulpOstreeCommitContentContext(PulpContentContext):
+    PLUGIN = "ostree"
+    RESOURCE_TYPE = "commit"
     ENTITY = _("commit content")
     ENTITIES = _("commit content")
     HREF = "ostree_ostree_commit_href"
     ID_PREFIX = "content_ostree_commits"
-    NEEDS_PLUGINS = [PluginRequirement("ostree", min="2.0.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ostree", specifier=">=2.0.0")]
 
 
 class PulpOstreeRefContentContext(PulpContentContext):
+    PLUGIN = "ostree"
+    RESOURCE_TYPE = "ref"
     ENTITY = _("ref content")
     ENTITIES = _("ref content")
     HREF = "ostree_ostree_ref_href"
     ID_PREFIX = "content_ostree_refs"
-    NEEDS_PLUGINS = [PluginRequirement("ostree", min="2.0.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ostree", specifier=">=2.0.0")]
 
 
 class PulpOstreeConfigContentContext(PulpContentContext):
+    PLUGIN = "ostree"
+    RESOURCE_TYPE = "config"
     ENTITY = _("config content")
     ENTITIES = _("config content")
     HREF = "ostree_ostree_config_href"
     ID_PREFIX = "content_ostree_configs"
-    NEEDS_PLUGINS = [PluginRequirement("ostree", min="2.0.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ostree", specifier=">=2.0.0")]
 
 
 class PulpOstreeDistributionContext(PulpEntityContext):
+    PLUGIN = "ostree"
+    RESOURCE_TYPE = "ostree"
     ENTITY = _("ostree distribution")
     ENTITIES = _("ostree distributions")
     HREF = "ostree_ostree_distribution_href"
     ID_PREFIX = "distributions_ostree_ostree"
-    NEEDS_PLUGINS = [PluginRequirement("ostree", min="2.0.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ostree", specifier=">=2.0.0")]
 
-    def preprocess_body(self, body: EntityDefinition) -> EntityDefinition:
-        body = super().preprocess_body(body)
+    def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
+        body = super().preprocess_entity(body, partial)
         version = body.pop("version", None)
         if version is not None:
             repository_href = body.pop("repository")
             body["repository_version"] = f"{repository_href}versions/{version}/"
         return body
 
 
 class PulpOstreeRemoteContext(PulpRemoteContext):
+    PLUGIN = "ostree"
+    RESOURCE_TYPE = "ostree"
     ENTITY = _("ostree remote")
     ENTITIES = _("ostree remotes")
     HREF = "ostree_ostree_remote_href"
     ID_PREFIX = "remotes_ostree_ostree"
-    NEEDS_PLUGINS = [PluginRequirement("ostree", min="2.0.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ostree", specifier=">=2.0.0")]
 
 
 class PulpOstreeRepositoryVersionContext(PulpRepositoryVersionContext):
+    PLUGIN = "ostree"
+    RESOURCE_TYPE = "ostree"
     HREF = "ostree_ostree_repository_version_href"
     ID_PREFIX = "repositories_ostree_ostree_versions"
-    NEEDS_PLUGINS = [PluginRequirement("ostree", min="2.0.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ostree", specifier=">=2.0.0")]
 
 
 class PulpOstreeRepositoryContext(PulpRepositoryContext):
+    PLUGIN = "ostree"
+    RESOURCE_TYPE = "ostree"
     HREF = "ostree_ostree_repository_href"
     ID_PREFIX = "repositories_ostree_ostree"
     IMPORT_ALL_ID: ClassVar[str] = "repositories_ostree_ostree_import_all"
     IMPORT_COMMITS_ID: ClassVar[str] = "repositories_ostree_ostree_import_commits"
     VERSION_CONTEXT = PulpOstreeRepositoryVersionContext
-    NEEDS_PLUGINS = [PluginRequirement("ostree", min="2.0.0")]
+    NEEDS_PLUGINS = [PluginRequirement("ostree", specifier=">=2.0.0")]
     CAPABILITIES = {
         "sync": [PluginRequirement("ostree")],
-        "import_all": [PluginRequirement("ostree", min="2.0.0")],
+        "import_all": [PluginRequirement("ostree", specifier=">=2.0.0")],
         "import_commits": [PluginRequirement("ostree")],
     }
 
     def import_all(self, href: str, artifact: str, repository_name: str) -> Any:
         body: Dict[str, Any] = {
             "artifact": artifact,
             "repository_name": repository_name,
@@ -106,10 +119,7 @@
             body["parent_commit"] = parent_commit
 
         return self.pulp_ctx.call(
             self.IMPORT_COMMITS_ID,
             parameters={self.HREF: href},
             body=body,
         )
-
-
-registered_repository_contexts["ostree:ostree"] = PulpOstreeRepositoryContext
```

### Comparing `pulp-glue-ostree-0.3.0/pulp_glue_ostree.egg-info/PKG-INFO` & `pulp-glue-ostree-0.4.0/pulp_glue_ostree.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue-ostree
-Version: 0.3.0
+Version: 0.4.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API. (OSTree plugin)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-ostree
 Project-URL: changelog, https://github.com/pulp/pulp-cli-ostree/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-ostree-0.3.0/pyproject.toml` & `pulp-glue-ostree-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pulp-glue-ostree"
-version = "0.3.0"
+version = "0.4.0"
 description = "Version agnostic glue library to talk to pulpcore's REST API. (OSTree plugin)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "GPLv2+"}
 authors = [
   {name = "Pulp Team", email = "pulp-list@redhat.com"},
 ]
@@ -19,15 +19,15 @@
   "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Topic :: System :: Software Distribution",
   "Typing :: Typed",
 ]
 dependencies = [
-  "pulp-glue>=0.20.0,<0.26",
+  "pulp-glue>=0.23.1,<0.26",
 ]
 
 [project.urls]
 repository = "https://github.com/pulp/pulp-cli-ostree"
 changelog = "https://github.com/pulp/pulp-cli-ostree/blob/main/CHANGES.md"
 
 [tool.setuptools.packages.find]
```

