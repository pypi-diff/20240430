# Comparing `tmp/pulp-cli-ostree-0.3.0.tar.gz` & `tmp/pulp-cli-ostree-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-cli-ostree-0.3.0.tar", last modified: Tue Apr 23 17:35:30 2024, max compression
+gzip compressed data, was "pulp-cli-ostree-0.4.0.tar", last modified: Tue Apr 30 13:13:55 2024, max compression
```

## Comparing `pulp-cli-ostree-0.3.0.tar` & `pulp-cli-ostree-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 17:35:30.000000 pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/pulpcore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/pulpcore/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-23 17:35:17.000000 pulp-cli-ostree-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:35:30.979662 pulp-cli-ostree-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:13:55.344095 pulp-cli-ostree-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-30 13:13:55.344095 pulp-cli-ostree-0.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:13:55.344095 pulp-cli-ostree-0.4.0/pulp_cli_ostree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-30 13:13:55.000000 pulp-cli-ostree-0.4.0/pulp_cli_ostree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 13:13:55.000000 pulp-cli-ostree-0.4.0/pulp_cli_ostree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:13:55.000000 pulp-cli-ostree-0.4.0/pulp_cli_ostree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 13:13:55.000000 pulp-cli-ostree-0.4.0/pulp_cli_ostree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 13:13:55.000000 pulp-cli-ostree-0.4.0/pulp_cli_ostree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 13:13:55.000000 pulp-cli-ostree-0.4.0/pulp_cli_ostree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:13:55.344095 pulp-cli-ostree-0.4.0/pulpcore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:13:55.344095 pulp-cli-ostree-0.4.0/pulpcore/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:13:55.344095 pulp-cli-ostree-0.4.0/pulpcore/cli/ostree/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 13:13:45.000000 pulp-cli-ostree-0.4.0/pulpcore/cli/ostree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-30 13:13:45.000000 pulp-cli-ostree-0.4.0/pulpcore/cli/ostree/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:13:45.000000 pulp-cli-ostree-0.4.0/pulpcore/cli/ostree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-30 13:13:45.000000 pulp-cli-ostree-0.4.0/pulpcore/cli/ostree/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-04-30 13:13:45.000000 pulp-cli-ostree-0.4.0/pulpcore/cli/ostree/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-30 13:13:45.000000 pulp-cli-ostree-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:13:55.344095 pulp-cli-ostree-0.4.0/setup.cfg
```

### Comparing `pulp-cli-ostree-0.3.0/PKG-INFO` & `pulp-cli-ostree-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-cli-ostree
-Version: 0.3.0
+Version: 0.4.0
 Summary: Command line interface to talk to pulpcore's REST API. (OSTree plugin commands)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-ostree
 Project-URL: changelog, https://github.com/pulp/pulp-cli-ostree/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pulp-cli-ostree-0.3.0/pulp_cli_ostree.egg-info/PKG-INFO` & `pulp-cli-ostree-0.4.0/pulp_cli_ostree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-cli-ostree
-Version: 0.3.0
+Version: 0.4.0
 Summary: Command line interface to talk to pulpcore's REST API. (OSTree plugin commands)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-ostree
 Project-URL: changelog, https://github.com/pulp/pulp-cli-ostree/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/__init__.py` & `pulp-cli-ostree-0.4.0/pulpcore/cli/ostree/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from typing import Any
 
 import click
+from pulp_glue.common.i18n import get_translation
 from pulpcore.cli.common.generic import pulp_group
 
 from pulpcore.cli.ostree.distribution import distribution
 from pulpcore.cli.ostree.remote import remote
 from pulpcore.cli.ostree.repository import repository
 
-__version__ = "0.3.0"
+translation = get_translation(__package__)
+_ = translation.gettext
+
+__version__ = "0.4.0"
 
 
 @pulp_group("ostree")
 def ostree_group() -> None:
     pass
```

### Comparing `pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/distribution.py` & `pulp-cli-ostree-0.4.0/pulpcore/cli/ostree/distribution.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from gettext import gettext as _
 from typing import Optional, Union, cast
 
 import click
 from pulp_glue.common.context import EntityDefinition, PluginRequirement, PulpEntityContext
+from pulp_glue.common.i18n import get_translation
 from pulp_glue.ostree.context import PulpOstreeDistributionContext, PulpOstreeRepositoryContext
 from pulpcore.cli.common.generic import (
     PulpCLIContext,
     base_path_contains_option,
     base_path_option,
     create_command,
     destroy_command,
@@ -17,14 +17,18 @@
     name_option,
     pass_entity_context,
     pass_pulp_context,
     resource_option,
     show_command,
 )
 
+translation = get_translation(__package__)
+_ = translation.gettext
+
+
 repository_option = resource_option(
     "--repository",
     default_plugin="ostree",
     default_type="ostree",
     context_table={"ostree:ostree": PulpOstreeRepositoryContext},
 )
 
@@ -78,15 +82,14 @@
     base_path: Optional[str],
     repository: Optional[Union[str, PulpEntityContext]],
     version: Optional[int],
 ) -> None:
     assert isinstance(distribution_ctx, PulpOstreeDistributionContext)
 
     distribution: EntityDefinition = distribution_ctx.entity
-    href: str = distribution_ctx.pulp_href
     body: EntityDefinition = {}
 
     if base_path is not None:
         body["base_path"] = base_path
     if repository is not None:
         if repository == "":
             # unset repository or repository version
@@ -94,42 +97,40 @@
                 body["repository"] = ""
             elif distribution["repository_version"]:
                 body["repository_version"] = ""
         else:
             repository = cast(PulpEntityContext, repository)
             if version is not None:
                 if distribution["repository"]:
-                    if pulp_ctx.has_plugin(PluginRequirement("ostree", min="2.0.0")):
+                    if pulp_ctx.has_plugin(PluginRequirement("ostree", specifier=">=2.0.0")):
                         body["repository"] = ""
                     else:
-                        distribution_ctx.update(href, body={"repository": ""}, non_blocking=True)
+                        distribution_ctx.update(body={"repository": ""}, non_blocking=True)
 
                 body["repository_version"] = f"{repository.pulp_href}versions/{version}/"
             else:
                 if distribution["repository_version"]:
-                    if pulp_ctx.has_plugin(PluginRequirement("ostree", min="2.0.0")):
+                    if pulp_ctx.has_plugin(PluginRequirement("ostree", specifier=">=2.0.0")):
                         body["repository_version"] = ""
                     else:
-                        distribution_ctx.update(
-                            href, body={"repository_version": ""}, non_blocking=True
-                        )
+                        distribution_ctx.update(body={"repository_version": ""}, non_blocking=True)
                 body["repository"] = repository.pulp_href
     elif version is not None:
         # keep current repository, change version
         if distribution["repository"]:
-            if pulp_ctx.has_plugin(PluginRequirement("ostree", min="2.0.0")):
+            if pulp_ctx.has_plugin(PluginRequirement("ostree", specifier=">=2.0.0")):
                 body["repository"] = ""
             else:
-                distribution_ctx.update(href, body={"repository": ""}, non_blocking=True)
+                distribution_ctx.update(body={"repository": ""}, non_blocking=True)
 
             body["repository_version"] = f'{distribution["repository"]}versions/{version}/'
         elif distribution["repository_version"]:
             repository_href = distribution["repository_version"].partition("versions")[0]
             body["repository_version"] = f"{repository_href}versions/{version}/"
         else:
             raise click.ClickException(
                 _(
                     "Distribution {distribution} doesn't have a repository set, "
                     "please specify the repository to use  with --repository"
                 ).format(distribution=distribution["name"])
             )
-    distribution_ctx.update(href, body=body)
+    distribution_ctx.update(body=body)
```

### Comparing `pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/remote.py` & `pulp-cli-ostree-0.4.0/pulpcore/cli/ostree/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from typing import Any
 
 import click
+from pulp_glue.common.i18n import get_translation
 from pulp_glue.ostree.context import PulpOstreeRemoteContext
 from pulpcore.cli.common.generic import (
     PulpCLIContext,
     common_remote_create_options,
     common_remote_update_options,
     create_command,
     destroy_command,
@@ -15,14 +16,17 @@
     list_command,
     name_option,
     pass_pulp_context,
     show_command,
     update_command,
 )
 
+translation = get_translation(__package__)
+_ = translation.gettext
+
 
 @click.group()
 @click.option(
     "-t",
     "--type",
     "remote_type",
     type=click.Choice(["ostree"], case_sensitive=False),
```

### Comparing `pulp-cli-ostree-0.3.0/pulpcore/cli/ostree/repository.py` & `pulp-cli-ostree-0.4.0/pulpcore/cli/ostree/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from gettext import gettext as _
 from typing import IO, Any, Dict, Optional
 
 import click
 from pulp_glue.common.context import (
     EntityFieldDefinition,
     PluginRequirement,
     PulpEntityContext,
     PulpRemoteContext,
     PulpRepositoryContext,
 )
+from pulp_glue.common.i18n import get_translation
+from pulp_glue.core.context import PulpArtifactContext
 from pulp_glue.ostree.context import (
     PulpOstreeCommitContentContext,
     PulpOstreeConfigContentContext,
     PulpOstreeRefContentContext,
     PulpOstreeRemoteContext,
     PulpOstreeRepositoryContext,
 )
@@ -28,24 +29,26 @@
     list_command,
     name_option,
     pass_pulp_context,
     pass_repository_context,
     pulp_option,
     repository_content_command,
     repository_href_option,
-    repository_option,
+    repository_lookup_option,
     resource_option,
     retained_versions_option,
     show_command,
     update_command,
     version_command,
 )
-from pulpcore.cli.core.context import PulpArtifactContext
 from pulpcore.cli.core.generic import task_command
 
+translation = get_translation(__package__)
+_ = translation.gettext
+
 remote_option = resource_option(
     "--remote",
     default_plugin="ostree",
     default_type="ostree",
     context_table={"ostree:ostree": PulpOstreeRemoteContext},
     href_pattern=PulpRemoteContext.HREF_PATTERN,
     help=_("Remote used for syncing in the form '[[<plugin>:]<resource_type>:]<name>' or by href."),
@@ -66,15 +69,15 @@
     if repo_type == "ostree":
         ctx.obj = PulpOstreeRepositoryContext(pulp_ctx)
     else:
         raise NotImplementedError()
 
 
 lookup_options = [href_option, name_option]
-nested_lookup_options = [repository_href_option, repository_option]
+nested_lookup_options = [repository_href_option, repository_lookup_option]
 update_options = [
     click.option("--description"),
     remote_option,
     retained_versions_option,
 ]
 create_options = update_options + [click.option("--name", required=True)]
 
@@ -164,29 +167,28 @@
     repository_ctx: PulpRepositoryContext,
     remote: EntityFieldDefinition,
 ) -> None:
     if not repository_ctx.capable("sync"):
         raise click.ClickException(_("Repository type does not support sync."))
 
     repository = repository_ctx.entity
-    repository_href = repository_ctx.pulp_href
 
     body: Dict[str, Any] = {}
 
     if isinstance(remote, PulpEntityContext):
         body["remote"] = remote.pulp_href
     elif repository["remote"] is None:
         raise click.ClickException(
             _(
                 "Repository '{name}' does not have a default remote. "
                 "Please specify with '--remote'."
             ).format(name=repository["name"])
         )
 
-    repository_ctx.sync(href=repository_href, body=body)
+    repository_ctx.sync(body=body)
 
 
 @repository.command(help=_("Import all refs and commits from a tarball"))
 @click.option("--file", type=click.File("rb"), required=True)
 @chunk_size_option
 @name_option
 @click.option(
@@ -252,15 +254,15 @@
     kwargs = {
         "href": repository_href,
         "artifact": artifact_href,
         "repository_name": repository_name,
         "ref": ref,
     }
 
-    if pulp_ctx.has_plugin(PluginRequirement("ostree", max="2.0.0")):
+    if pulp_ctx.has_plugin(PluginRequirement("ostree", specifier="<2.0.0")):
         if not all((ref, parent_commit)) and any((ref, parent_commit)):
             raise click.ClickException(
                 "Please specify both the ref and parent_commit if you want to add new child "
                 "commits to the existing repository"
             )
 
         kwargs["parent_commit"] = parent_commit
```

