# Comparing `tmp/aedev_git_repo_manager-0.3.75.tar.gz` & `tmp/aedev_git_repo_manager-0.3.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aedev_git_repo_manager-0.3.75.tar", last modified: Sun Apr 14 19:38:23 2024, max compression
+gzip compressed data, was "aedev_git_repo_manager-0.3.76.tar", last modified: Tue Apr 30 12:49:45 2024, max compression
```

## Comparing `aedev_git_repo_manager-0.3.75.tar` & `aedev_git_repo_manager-0.3.76.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:38:23.711288 aedev_git_repo_manager-0.3.75/
--rw-rw-rw-   0 root         (0) root         (0)    35002 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     6549 2024-04-14 19:38:23.711288 aedev_git_repo_manager-0.3.75/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3543 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:38:23.703964 aedev_git_repo_manager-0.3.75/aedev/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:38:23.705795 aedev_git_repo_manager-0.3.75/aedev/git_repo_manager/
--rw-rw-rw-   0 root         (0) root         (0)     1879 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/aedev/git_repo_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   186882 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/aedev/git_repo_manager/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:38:23.707626 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6549 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      449 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      117 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      543 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 19:38:23.000000 aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 19:38:23.711288 aedev_git_repo_manager-0.3.75/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 19:38:23.707626 aedev_git_repo_manager-0.3.75/tests/
--rw-rw-rw-   0 root         (0) root         (0)   157998 2024-04-14 19:38:12.000000 aedev_git_repo_manager-0.3.75/tests/test_git_repo_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:49:45.639560 aedev_git_repo_manager-0.3.76/
+-rw-rw-rw-   0 root         (0) root         (0)    35002 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     6549 2024-04-30 12:49:45.639560 aedev_git_repo_manager-0.3.76/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:49:45.632560 aedev_git_repo_manager-0.3.76/aedev/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:49:45.633560 aedev_git_repo_manager-0.3.76/aedev/git_repo_manager/
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/aedev/git_repo_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   187688 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/aedev/git_repo_manager/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:49:45.636560 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6549 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      449 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      543 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 12:49:45.000000 aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 12:49:45.639560 aedev_git_repo_manager-0.3.76/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 12:49:45.635560 aedev_git_repo_manager-0.3.76/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   157998 2024-04-30 12:49:33.000000 aedev_git_repo_manager-0.3.76/tests/test_git_repo_manager.py
```

### Comparing `aedev_git_repo_manager-0.3.75/LICENSE.md` & `aedev_git_repo_manager-0.3.76/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aedev_git_repo_manager-0.3.75/PKG-INFO` & `aedev_git_repo_manager-0.3.76/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev_git_repo_manager
-Version: 0.3.75
+Version: 0.3.76
 Summary: aedev namespace package portion git_repo_manager: create and maintain local/remote git repositories of Python projects
 Home-page: https://gitlab.com/aedev-group/aedev_git_repo_manager
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://aedev.readthedocs.io/en/latest/_autosummary/aedev.git_repo_manager.html
 Project-URL: Repository, https://gitlab.com/aedev-group/aedev_git_repo_manager
@@ -72,25 +72,25 @@
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.75
+# git_repo_manager 0.3.76
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.72?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.72)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.75?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.75)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.75.
+>aedev_git_repo_manager package 0.3.76.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.75/README.md` & `aedev_git_repo_manager-0.3.76/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.75
+# git_repo_manager 0.3.76
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.72?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.72)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.75?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.75)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.75.
+>aedev_git_repo_manager package 0.3.76.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.75/aedev/git_repo_manager/__init__.py` & `aedev_git_repo_manager-0.3.76/aedev/git_repo_manager/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 
 in conjunction with the template projects of the `aedev` namespace (like e.g. :mod:`aedev.tpl_project`) any common
 portions file (even the ``setup.py`` file) can be created/maintained as a template in a single place, and then
 requested and updated individually for each portion project.
 """
 
 
-__version__ = '0.3.75'
+__version__ = '0.3.76'
```

### Comparing `aedev_git_repo_manager-0.3.75/aedev/git_repo_manager/__main__.py` & `aedev_git_repo_manager-0.3.76/aedev/git_repo_manager/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Sequence, Set, Tuple, Union, cast)
 
 from dotenv import find_dotenv, load_dotenv
 
 from github import Github
 from gitlab import Gitlab, GitlabCreateError, GitlabError, GitlabHttpError
 from gitlab.const import MAINTAINER_ACCESS
-from gitlab.v4.objects import Group, Project
+from gitlab.v4.objects import Group, Project, User
 
 from packaging.version import Version
 from PIL import Image
 
 import ae.base                                                                          # type: ignore # for patching
 from ae.base import (
     PY_EXT, PY_INIT, TEMPLATES_FOLDER, UNSET, UnsetType,
@@ -2457,36 +2457,51 @@
                 self.connection.enable_debug()
             self.connection.auth()          # authenticate and create user attribute
         except (Exception, ) as ex:
             cae.po(f"****  Gitlab connection exception: {ex}")
             return False
         return True
 
-    def group_from_name(self, group_name: str) -> Optional[Group]:
-        """ convert group/username string to remote repo user/group instance.
+    def owner_from_pdv(self, ini_pdv: PdvType) -> Union[Group, User]:
+        """ convert group/user specified in pdv to remote repo group/user object instance.
 
-        :param group_name:      group name to search.
-        :return:                gitlab group object/instance or None if not found.
+        :param ini_pdv:         project dev vars.
+        :return:                gitlab owner object/instance (group or user) or quit with error if not found.
         """
+        domain = _get_host_domain(ini_pdv)
+
+        group_name = _get_host_group(ini_pdv, domain)
         try:
             return self.connection.groups.get(group_name)
         except GitlabError:
             groups = self.connection.groups.list(search=group_name)
-        return groups[0] if groups else None                        # type: ignore
+            if groups:
+                return groups[0]                                    # type: ignore
+
+        user_name = _get_host_user_name(ini_pdv, domain)
+        try:
+            return self.connection.users.get(user_name)
+        except GitlabError:
+            users = self.connection.users.list(search=user_name)
+            if users:
+                return users[0]                                     # type: ignore
+
+        _exit_error(37, f"neither group '{group_name}' nor user '{user_name}' found on repository host '{domain}'")
+        return                                                      # type: ignore
 
     def project_from_name(self, err_code: int, err_msg: str, project_name: str, owned: bool = True) -> Project:
         """ convert group/project_name or an endswith-fragment of it to a Project instance of the remote repo api.
 
         :param err_code:        error code, pass 0 to not exit on error.
         :param err_msg:         error message to display on error with optional {name} to be automatically substituted
                                 with the project name from the :paramref:`~project_from_name.project_name` argument.
         :param project_name:    package-name, group/package-name or group/package-endswith-fragment to search for.
         :param owned:           if True then the 2nd/fallback fragment/list search is limited to owned repos (quicker).
                                 pass False to search in all repos for the specified group/project-name fragment.
-        :return:                python-gitlab project instance if found, else return None if err_code is zero else exit.
+        :return:                python-gitlab project instance if found, else return None if err_code is zero else quit.
         """
         try:
             # Projects.get() raises GitLabError (404 project not found) on an exact project name if there are other
             # project names starting with the same string. Projects.list() will then return the project as last item.
             return self.connection.projects.get(project_name)
         except GitlabError:     # e.g. GitlabGetError: 404: 404 Project Not Found
             projects = cast(List[Project], self.connection.projects.list(search=project_name, owned=owned))
@@ -2618,26 +2633,26 @@
         project_name = _get_prj_name(ini_pdv)
 
         changed = _git_uncommitted(ini_pdv)
         _chk_if(76, not changed, f"{project_name} has {len(changed)} uncommitted files: {changed}")
 
         push_refs = []
         if not self.project_from_name(0, "", project_name):
-            group_name = _get_host_group(ini_pdv, _get_host_domain(ini_pdv))
+            owner_obj = self.owner_from_pdv(ini_pdv)                # get group/user object or quit
             project_properties = {
                 'name': project_name,
-                'namespace_id': self.group_from_name(group_name).id,        # type: ignore
+                'namespace_id': owner_obj.id,
                 'description': pdv_str(ini_pdv, 'project_desc'),
                 'default_branch': MAIN_BRANCH,
                 'visibility': 'public',
             }
             cae.vpo(f"    - remote project properties of new package {project_name}: {PPF(project_properties)}")
             project = cast(Project, self.connection.projects.create(project_properties))
 
-            cae.po(f"   == created new project {PPF(project.attributes)} under remote user/group {group_name}")
+            cae.po(f"   == created new project {PPF(project.attributes)} under remote user/group {owner_obj.name}")
             _wait()
 
             for branch_mask in (MAIN_BRANCH, 'release*'):
                 protected_branch_properties = {'name': branch_mask,
                                                'merge_access_level': MAINTAINER_ACCESS,
                                                'push_access_level': MAINTAINER_ACCESS}
                 cae.vpo(f"    - {branch_mask} protected branch properties: {protected_branch_properties}")
@@ -2831,34 +2846,37 @@
                                             pdv_val(ini_pdv, 'project_name'))
         return not self.connection.error_message
 
     deploy_flags = {'ALL': False, 'CLEANUP': False, 'LEAN': False, 'MASKS': []}
     """ optional flag names and default values for the actions :meth:`check_deploy` and :meth:`deploy_project` """
 
     def deploy_differences(self, ini_pdv: PdvType, action: str, version_tag: str, **optional_flags
-                           ) -> tuple[str, set[str], set[str]]:
+                           ) -> tuple[str, str, set[str], set[str]]:
         """ determine differences between the specified repository and web host/server (deployable and deletable files).
 
         :param ini_pdv:         project dev vars.
         :param action:          pass 'check' to only check the differences between the specified repository and
                                 the web server/host, or 'deploy' to prepare the deployment of these differences.
         :param version_tag:     project package version to deploy. pass ``LATEST`` to use the version tag
                                 of the latest repository version (PyPI release), or ``WORKTREE`` to deploy
                                 the actual working tree package version (including unstaged/untracked files).
         :param optional_flags:  optional command line arguments, documented in detail in the declaration of
                                 the action method parameter :paramref:`check_deploy.optional_flags`.
-        :return:                tuple of string and 2 sets. both sets containing file paths, relative to the
-                                local/temporary project root folder, which gets returned as the first item of the tuple.
-                                the first set contains the deployable files, and the 2nd one the files that got removed
-                                from the repository or that could be cleaned-up on the server.
+        :return:                tuple of 2 strings and 2 sets. the first string contains a description of the project
+                                and the server to check/deploy-to, and the second the path to the project root folder.
+                                the two sets containing project file paths, relative to the
+                                local/temporary project root folder, the first one with the deployable files,
+                                and the 2nd one with the removable files.
         """
+        prj_desc = f"{pdv_str(ini_pdv, 'web_user')}@{pdv_str(ini_pdv, 'web_domain')}/{pdv_str(ini_pdv, 'project_desc')}"
         func = self.check_deploy if action == 'check' else self.deploy_project
         lean_msg = ' lean' if optional_flags['LEAN'] else ''
         verbose = _debug_or_verbose()
         deployed_ver = self.connection.deployed_version()
+        cae.po(f" ---- {action} {version_tag}{lean_msg} against host/project {prj_desc} {deployed_ver}")
 
         if version_tag == 'WORKTREE':
             include_untracked = True
             branch_or_tag = f"v{deployed_ver}" if deployed_ver else MAIN_BRANCH     # from this to HEAD
             prj_root_path = pdv_str(ini_pdv, 'project_path')
             version_tag = f"v{_git_project_version(ini_pdv, increment_part=0)}w"    # w suffix only visible in logs
         else:
@@ -2874,14 +2892,15 @@
             prj_root_path = _git_clone(pdv_str(ini_pdv, 'repo_root'), pdv_str(ini_pdv, 'project_name'),
                                        branch_or_tag=version_tag, extra_args=("--filter=blob:none", ))
             _chk_if(85, bool(prj_root_path), "git clone tmp cleanup error, to check run again with the -D 1 option")
             branch_or_tag = f"v{deployed_ver}...{version_tag}"
 
         path_masks = optional_flags['MASKS'] + ['manage.py'] + root_packages_masks(ini_pdv)
         cae.vpo(f"  --- {len(path_masks)} deploy file path masks found: {_pp(sorted(path_masks))}")
+
         skip_func = skip_files_lean_web if lean_msg else skip_py_cache_files
         skipped = set()
 
         def _track_skipped(file_path: str) -> bool:
             if skip_func(file_path):
                 if skip_py_cache_files(file_path):
                     return True
@@ -2942,15 +2961,15 @@
 
         verbose = action == 'check' or verbose
         cae.po(f" ===  {len(to_deploy)} {which_files} files found to migrate server to {version_tag} version"
                f"{'; from v' + deployed_ver if deployed_ver else ''}{':' + _pp(sorted(to_deploy)) if verbose else ''}")
         cae.po(f" ===  {len(to_delete) + len(to_cleanup)} deletable (repo={len(to_delete)} cleanup={len(to_cleanup)})"
                f" files found{':' + _pp(sorted(to_delete | to_cleanup)) if verbose else ''}")
 
-        return prj_root_path, to_deploy, to_delete | to_cleanup
+        return prj_desc, prj_root_path, to_deploy, to_delete | to_cleanup
 
     # ----------- remote action methods ----------------------------------------------------------------------------
 
     @_action(APP_PRJ, DJANGO_PRJ, arg_names=(("version-tag", ), ('LATEST', ), ('WORKTREE', ), ), flags=deploy_flags)
     def check_deploy(self, ini_pdv: PdvType, version_tag: str, **optional_flags):
         """ check all project package files at the app/web server against the specified package version.
 
@@ -2974,46 +2993,44 @@
                                   repository files to check/deploy. to include e.g. the files of the static root folder
                                   specify this argument as ``MASKS="['static/**/*']"``. single files can be included
                                   too, by adding their possible file names to the list - only the found ones will be
                                   included. for example to include the django database you could add some possible DB
                                   file names to the list like in ``"MASKS=['static/**/*', 'db.sqlite', 'project.db']"``
 
         """
-        root, to_deploy, to_delete = self.deploy_differences(ini_pdv, 'check', version_tag, **optional_flags)
+        prj_desc, _, to_deploy, to_delete = self.deploy_differences(ini_pdv, 'check', version_tag, **optional_flags)
 
-        cae.po(f" ==== {len(to_deploy)} files outdated and {len(to_delete)} could be deleted on server"
-               f" {pdv_str(ini_pdv, 'web_user')}@{pdv_str(ini_pdv, 'web_domain')} / {pdv_str(ini_pdv, 'project_desc')}")
+        cae.po(f" ==== found {len(to_deploy)} outdated and {len(to_delete)} deletable files on host/project {prj_desc}")
 
     @_action(APP_PRJ, DJANGO_PRJ, arg_names=(("version-tag", ), ('LATEST', ), ('WORKTREE', ), ), flags=deploy_flags,
              shortcut='deploy')
     def deploy_project(self, ini_pdv: PdvType, version_tag: str, **optional_flags):
         """ deploy code files of django/app project version to the web-/app-server.
 
         :param ini_pdv:         project dev vars.
         :param version_tag:     version tag in the format ``v<version-number>`` to deploy or ``LATEST`` to use
                                 the tag of the latest repository version or ``WORKTREE`` to deploy directly
                                 from the local work tree (including locally added, unstaged and changed files).
         :param optional_flags:  optional command line arguments, documented in the :meth:`.check_deploy` action.
         """
-        root, to_deploy, to_delete = self.deploy_differences(ini_pdv, 'deploy', version_tag, **optional_flags)
+        prj_desc, root, to_deploy, to_delete = self.deploy_differences(ini_pdv, 'deploy', version_tag, **optional_flags)
 
         for upg_fil in to_deploy:
             err_str = self.connection.deploy_file(upg_fil, read_file(os.path.join(root, upg_fil), extra_mode='b'))
             _chk_if(96, not err_str, err_str)
 
         for del_fil in to_delete:
             err_str = self.connection.delete_file_or_folder(del_fil)
             _chk_if(96, not err_str, err_str)
 
         verbose = _debug_or_verbose()
         cae.po(f"  === {len(to_deploy)} files deployed{': ' + _pp(sorted(to_deploy)) if verbose else ''}")
         cae.po(f"  === {len(to_delete)} files removed{': ' + _pp(sorted(to_deploy)) if verbose else ''}")
         cae.po("  === check server if Django manage migration command(s) have to be run and if a restart is needed")
-        cae.po(f" ==== deployed {version_tag} to server"
-               f" {pdv_str(ini_pdv, 'web_user')}@{pdv_str(ini_pdv, 'web_domain')} / {pdv_str(ini_pdv, 'project_desc')}")
+        cae.po(f" ==== successfully deployed {version_tag} to host/project {prj_desc}")
 
 
 # --------------- local actions ---------------------------------------------------------------------------------------
 
 
 @_action(PARENT_PRJ, ROOT_PRJ, arg_names=tuple(tuple(('source-name', 'rel-path', ) + _) for _ in ARGS_CHILDREN_DEFAULT))
 def add_children_file(ini_pdv: PdvType, file_name: str, rel_path: str, *children_pdv: PdvType) -> bool:
```

### Comparing `aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/PKG-INFO` & `aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aedev_git_repo_manager
-Version: 0.3.75
+Version: 0.3.76
 Summary: aedev namespace package portion git_repo_manager: create and maintain local/remote git repositories of Python projects
 Home-page: https://gitlab.com/aedev-group/aedev_git_repo_manager
 Author: AndiEcker
 Author-email: aecker2@gmail.com
 License: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://aedev.readthedocs.io/en/latest/_autosummary/aedev.git_repo_manager.html
 Project-URL: Repository, https://gitlab.com/aedev-group/aedev_git_repo_manager
@@ -72,25 +72,25 @@
 Requires-Dist: typing; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Requires-Dist: wheel; extra == "tests"
 Requires-Dist: twine; extra == "tests"
 
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.aedev V0.3.22 -->
 <!-- THIS FILE IS EXCLUSIVELY MAINTAINED by the project aedev.tpl_namespace_root V0.3.14 -->
-# git_repo_manager 0.3.75
+# git_repo_manager 0.3.76
 
 [![GitLab develop](https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/develop?logo=python)](
     https://gitlab.com/aedev-group/aedev_git_repo_manager)
 [![LatestPyPIrelease](
-    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.72?logo=python)](
-    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.72)
+    https://img.shields.io/gitlab/pipeline/aedev-group/aedev_git_repo_manager/release0.3.75?logo=python)](
+    https://gitlab.com/aedev-group/aedev_git_repo_manager/-/tree/release0.3.75)
 [![PyPIVersions](https://img.shields.io/pypi/v/aedev_git_repo_manager)](
     https://pypi.org/project/aedev-git-repo-manager/#history)
 
->aedev_git_repo_manager package 0.3.75.
+>aedev_git_repo_manager package 0.3.76.
 
 [![Coverage](https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/coverage/index.html)
 [![MyPyPrecision](https://aedev-group.gitlab.io/aedev_git_repo_manager/mypy.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/lineprecision.txt)
 [![PyLintScore](https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.svg)](
     https://aedev-group.gitlab.io/aedev_git_repo_manager/pylint.log)
```

### Comparing `aedev_git_repo_manager-0.3.75/aedev_git_repo_manager.egg-info/requires.txt` & `aedev_git_repo_manager-0.3.76/aedev_git_repo_manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aedev_git_repo_manager-0.3.75/setup.py` & `aedev_git_repo_manager-0.3.76/setup.py`

 * *Files identical despite different names*

### Comparing `aedev_git_repo_manager-0.3.75/tests/test_git_repo_manager.py` & `aedev_git_repo_manager-0.3.76/tests/test_git_repo_manager.py`

 * *Files identical despite different names*

