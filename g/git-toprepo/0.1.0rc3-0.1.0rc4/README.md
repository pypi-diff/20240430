# Comparing `tmp/git_toprepo-0.1.0rc3.tar.gz` & `tmp/git_toprepo-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_toprepo-0.1.0rc3.tar", max compression
+gzip compressed data, was "git_toprepo-0.1.0rc4.tar", max compression
```

## Comparing `git_toprepo-0.1.0rc3.tar` & `git_toprepo-0.1.0rc4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2024-04-19 07:12:26.634820 git_toprepo-0.1.0rc3/LICENSE
--rw-r--r--   0        0        0     8855 2024-04-19 07:12:26.634820 git_toprepo-0.1.0rc3/README.md
--rwxr-xr-x   0        0        0    96764 2024-04-19 07:12:26.634820 git_toprepo-0.1.0rc3/git_toprepo.py
--rw-r--r--   0        0        0      621 2024-04-19 07:12:32.826889 git_toprepo-0.1.0rc3/pyproject.toml
--rw-r--r--   0        0        0     9590 1970-01-01 00:00:00.000000 git_toprepo-0.1.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 09:09:20.840105 git_toprepo-0.1.0rc4/LICENSE
+-rw-r--r--   0        0        0     8855 2024-04-30 09:09:20.844105 git_toprepo-0.1.0rc4/README.md
+-rwxr-xr-x   0        0        0    98319 2024-04-30 09:09:20.844105 git_toprepo-0.1.0rc4/git_toprepo.py
+-rw-r--r--   0        0        0      621 2024-04-30 09:09:28.332152 git_toprepo-0.1.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     9590 1970-01-01 00:00:00.000000 git_toprepo-0.1.0rc4/PKG-INFO
```

### Comparing `git_toprepo-0.1.0rc3/LICENSE` & `git_toprepo-0.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `git_toprepo-0.1.0rc3/README.md` & `git_toprepo-0.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `git_toprepo-0.1.0rc3/git_toprepo.py` & `git_toprepo-0.1.0rc4/git_toprepo.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,24 +85,45 @@
                 text=True,
             ).rstrip("\n")
         )
         super().__init__(toplevel_repo_dir)
 
     @lru_cache
     def get_toprepo_fetch_url(self) -> Url:
-        toprepo_fetchurl_key = "toprepo.top.fetchUrl"
+        fetch_url = self.get_toprepo_fetch_url_impl("remote.origin.url", False)
+        if fetch_url is None or fetch_url == "file:///dev/null":
+            # TODO: 2024-04-29 Remove after migration.
+            fetch_url = self.get_toprepo_fetch_url_impl("toprepo.top.fetchUrl", True)
+            subprocess.check_output(
+                ["git", "-C", str(self.path), "config", "remote.origin.url", fetch_url],
+                text=True,
+            ).rstrip()
+        # TODO: 2024-04-29 Remove after migration.
+        push_url = self.get_toprepo_fetch_url_impl("remote.top.pushUrl", False)
+        if push_url is None:
+            push_url = self.get_toprepo_fetch_url_impl("toprepo.top.pushUrl", True)
+            subprocess.check_output(
+                ["git", "-C", str(self.path), "config", "remote.top.pushUrl", push_url],
+                text=True,
+            ).rstrip()
+        return fetch_url
+
+    def get_toprepo_fetch_url_impl(self, toprepo_fetchurl_key, throw) -> Optional[Url]:
         try:
             fetch_url = subprocess.check_output(
                 ["git", "-C", str(self.path), "config", toprepo_fetchurl_key], text=True
             ).rstrip()
         except subprocess.CalledProcessError as err:
             if err.returncode == 1:
-                raise ValueError(
-                    f"git-config {toprepo_fetchurl_key} is missing in {self.path}"
-                )
+                if throw:
+                    raise ValueError(
+                        f"git-config {toprepo_fetchurl_key} is missing in {self.path}"
+                    )
+                else:
+                    return None
             raise
         return fetch_url
 
     def get_toprepo_dir(self) -> Path:
         return self.get_subrepo_dir(TopRepo.name)
 
     def get_subrepo_dir(self, name: RepoName):
@@ -767,20 +788,26 @@
                 _, _, repo_id, subkey = key.split(".", 3)
                 repo_config_dicts[repo_id][subkey].extend(values)
 
         # Resolve the role.
         config_dict.setdefault("toprepo.role.default.repos", ["+.*"])
         role = config_dict.get("toprepo.role", ["default"])[-1]
         wanted_repos_patterns = config_dict.setdefault(f"toprepo.role.{role}.repos", [])
-        top_fetch_url = config_dict.get("toprepo.top.fetchurl", [None])[-1]
-        if top_fetch_url is None:
-            raise ConfigParsingError("Config toprepo.top.fetchUrl is not set")
-        top_push_url = config_dict.get("toprepo.top.pushurl", [None])[-1]
+        top_fetch_url = config_dict.get("remote.origin.url", [None])[-1]
+        if top_fetch_url is None or top_fetch_url == "file:///dev/null":
+            # TODO: 2024-04-29 Remove after migration.
+            top_fetch_url = config_dict.get("toprepo.top.fetchurl", [None])[-1]
+            if top_fetch_url is None:
+                raise ConfigParsingError("Config remote.origin.url is not set")
+        top_push_url = config_dict.get("remote.top.pushurl", [None])[-1]
         if top_push_url is None:
-            raise ConfigParsingError("Config toprepo.top.pushUrl is not set")
+            # TODO: 2024-04-29 Remove after migration.
+            top_push_url = config_dict.get("toprepo.top.pushurl", [None])[-1]
+            if top_push_url is None:
+                raise ConfigParsingError("Config remote.top.pushUrl is not set")
         repo_configs = Config.parse_repo_configs(
             repo_config_dicts,
             wanted_repos_patterns,
             top_fetch_url,
             top_push_url,
         )
 
@@ -2190,27 +2217,29 @@
         return 1
     if not monorepo_dir.parent.exists():
         print(f"ERROR: The directory {monorepo_dir.parent} is missing")
         return 1
     monorepo_dir.mkdir()
     try:
         log_run_git(monorepo_dir, ["init", "--quiet"])
+        # git-submodule and git-filter-repo fail if remote.origin.url is missing.
         log_run_git(
             monorepo_dir,
-            ["config", "toprepo.top.fetchUrl", args.repository],
+            ["config", "remote.origin.url", args.repository],
         )
+        # Avoid accidental `git push origin`, use `git-toprepo push`.
         log_run_git(
             monorepo_dir,
-            ["config", "toprepo.top.pushUrl", args.repository],
+            ["config", "remote.origin.pushUrl", "file:///dev/null"],
+            log_command=False,
         )
-        # git-filter-repo fails if remote.origin.url is missing.
+        # Power users can push to the "top" remote.
         log_run_git(
             monorepo_dir,
-            ["config", "remote.origin.url", "file:///dev/null"],
-            log_command=False,
+            ["config", "remote.top.pushUrl", args.repository],
         )
         monorepo = MonoRepo(monorepo_dir)
         toprepo_dir = monorepo.get_toprepo_dir()
         toprepo_dir.mkdir(parents=True)
         log_run_git(
             toprepo_dir,
             ["init", "--quiet", "--bare"],
```

### Comparing `git_toprepo-0.1.0rc3/pyproject.toml` & `git_toprepo-0.1.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-toprepo"
-version = "0.1.0rc3"
+version = "0.1.0rc4"
 description = "git-submodule made easy with git-toprepo"
 keywords = ["git", "submodule", "monorepo", "toprepo", "superrepo"]
 authors = ["Fredrik Medley <fredrik@meroton.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `git_toprepo-0.1.0rc3/PKG-INFO` & `git_toprepo-0.1.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-toprepo
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: git-submodule made easy with git-toprepo
 License: GPL-3.0-only
 Keywords: git,submodule,monorepo,toprepo,superrepo
 Author: Fredrik Medley
 Author-email: fredrik@meroton.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

