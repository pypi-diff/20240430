# Comparing `tmp/japr-1.0.1.tar.gz` & `tmp/japr-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "japr-1.0.1.tar", max compression
+gzip compressed data, was "japr-1.1.0.tar", max compression
```

## Comparing `japr-1.0.1.tar` & `japr-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-01-21 19:39:00.706060 japr-1.0.1/LICENSE.md
--rw-r--r--   0        0        0    17910 2024-01-21 19:39:00.706060 japr-1.0.1/README.md
--rw-r--r--   0        0        0      679 2024-01-21 19:39:00.710060 japr-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1148 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check.py
--rw-r--r--   0        0        0     1049 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check_providers/__init__.py
--rw-r--r--   0        0        0     1661 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check_providers/ci_check_provider.py
--rw-r--r--   0        0        0     2458 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check_providers/contributing_check_provider.py
--rw-r--r--   0        0        0     5517 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check_providers/csharp_check_provider.py
--rw-r--r--   0        0        0     6529 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check_providers/git_check_provider.py
--rw-r--r--   0        0        0     6645 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check_providers/github_check_provider.py
--rw-r--r--   0        0        0     4323 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check_providers/javascript_check_provider.py
--rw-r--r--   0        0        0     1324 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check_providers/license_check_provider.py
--rw-r--r--   0        0        0     7931 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check_providers/python_check_provider.py
--rw-r--r--   0        0        0     4937 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check_providers/readme_check_provider.py
--rw-r--r--   0        0        0     2118 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/check_providers/rust_check_provider.py
--rw-r--r--   0        0        0    11543 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/japr.py
--rw-r--r--   0        0        0      968 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/template_util.py
--rw-r--r--   0        0        0     9470 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/templates/CONTRIBUTING.md
--rw-r--r--   0        0        0     1093 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/templates/README.md
--rw-r--r--   0        0        0      826 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/templates/bug_report_issue_template.md
--rw-r--r--   0        0        0      601 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/templates/feature_request_issue_template.md
--rw-r--r--   0        0        0      915 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/templates/pull_request_template.md
--rw-r--r--   0        0        0      953 2024-01-21 19:39:00.710060 japr-1.0.1/src/japr/util.py
--rw-r--r--   0        0        0    18647 1970-01-01 00:00:00.000000 japr-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-30 11:34:37.985451 japr-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0    20994 2024-04-30 11:34:37.985451 japr-1.1.0/README.md
+-rw-r--r--   0        0        0      680 2024-04-30 11:34:37.989451 japr-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1148 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check.py
+-rw-r--r--   0        0        0     1160 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/__init__.py
+-rw-r--r--   0        0        0     1661 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/ci_check_provider.py
+-rw-r--r--   0        0        0     2526 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/contributing_check_provider.py
+-rw-r--r--   0        0        0     5633 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/csharp_check_provider.py
+-rw-r--r--   0        0        0     6577 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/git_check_provider.py
+-rw-r--r--   0        0        0     6645 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/github_check_provider.py
+-rw-r--r--   0        0        0     4379 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/javascript_check_provider.py
+-rw-r--r--   0        0        0     1392 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/license_check_provider.py
+-rw-r--r--   0        0        0     8043 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/python_check_provider.py
+-rw-r--r--   0        0        0     5201 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/readme_check_provider.py
+-rw-r--r--   0        0        0     2118 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/rust_check_provider.py
+-rw-r--r--   0        0        0     8449 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/terraform_check_provider.py
+-rw-r--r--   0        0        0    11543 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/japr.py
+-rw-r--r--   0        0        0      968 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/template_util.py
+-rw-r--r--   0        0        0     9470 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/templates/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1093 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/templates/README.md
+-rw-r--r--   0        0        0      826 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/templates/bug_report_issue_template.md
+-rw-r--r--   0        0        0      601 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/templates/feature_request_issue_template.md
+-rw-r--r--   0        0        0      915 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/templates/pull_request_template.md
+-rw-r--r--   0        0        0     1042 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/util.py
+-rw-r--r--   0        0        0    21696 1970-01-01 00:00:00.000000 japr-1.1.0/PKG-INFO
```

### Comparing `japr-1.0.1/LICENSE.md` & `japr-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `japr-1.0.1/README.md` & `japr-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -70,19 +70,19 @@
 ## Supported Languages
 Japr will work for projects of all languages however there are additional checks for the following:
 - Python
 - C#
 - Javascript
 
 The following table tracks the level of support for each language. Many languages also have additional checks not listed.
-|                       | Python         | C# | JS        | Rust  |
-|-----------------------|----------------|----|-----------|-------|
-| Linter setup          | ✅             | ✅ | ✅        |       |
-| Lock files in Git     | ✅             | ❌ | ✅        | ✅    |
-| Dependency Managers   | Poetry, Pipenv |    | NPM, Yarn | Cargo |
+|                       | Python         | C# | JS        | Rust  | Terraform |
+|-----------------------|----------------|----|-----------|-------|-----------|
+| Linter setup          | ✅             | ✅ | ✅        |       | ❌        |
+| Lock files in Git     | ✅             | ❌ | ✅        | ✅    | ✅        |
+| Dependency Managers   | Poetry, Pipenv |    | NPM, Yarn | Cargo |           |
 
 ## Experimental Automatic Fixes
 Japr can automatically fix some issues when supplied the `--fix` flag. **This functionality is highly expermental**
 
 ## Development
 Pull requsts are welcome. Please read [the contributing guide first](./CONTRIBUTING.md).
 
@@ -197,7 +197,21 @@
 
 ### Javascript
 | ID | Severity | Enabled for Project Types | Description | Advice |
 |----|----------|---------------------------|-------------|--------|
 | JS002 | Medium | open-source, inner-source, team | Javascript projects should have a linter configured | Javascript projects should have a comprehensive linter configured such as ESLint in order to ensure a consistent code style is used across all files and by all contributors.</br></br>Having a consistent style helps ensure readability and ease of understanding for any outsider looking into the project's code. Linters can also improve the stability of the code by catching mistakes before the code is published. |
 | JS004 | Medium | open-source, inner-source, team, personal | Javascript projects should have their lock files committed into Git | When using a dependency manager for Javascript such as npm, the lock files should be comitted into Git. This ensures that all dependencies of packages are installed at the same version no matter when and on what machine the project is installed. |
 
+### Rust
+| ID | Severity | Enabled for Project Types | Description | Advice |
+|----|----------|---------------------------|-------------|--------|
+| RS004 | Medium | open-source, inner-source, team, personal | Rust projects should have their Cargo lock files committed into Git | When using Cargo for Rust, the lock files should be comitted into Git. This ensures that all dependencies of packages are installed at the same version no matter when and on what machine the project is installed. |
+
+### Terraform
+| ID | Severity | Enabled for Project Types | Description | Advice |
+|----|----------|---------------------------|-------------|--------|
+| TF004 | Medium | open-source, inner-source, team, personal | Terraform projects should have their Terraform lock files committed into Git | When using Terraform, the lock files should be comitted into Git. This ensures that all dependencies of packages are installed at the same version no matter when and on what machine the project is installed. |
+| TF005 | Medium | open-source, inner-source, team, personal | Terraform projects should not have their .terraform directory committed into Git | The .terraform directory contains binaries, thrid party modules and other things that are generated during a terraform init. This folder should not be committed into git. |
+| TF006 | High | open-source, inner-source, team, personal | Terraform state files should not be committed into git | Terraform state files can contain secrets and are stored unencrypted. These secrets can be easily leaked when stored in git. Additionally, terraform state in git does not provide a single source of truth nor state locking and so can cause major issues when used in teams.</br></br>Instead of storing state in git, use another terraform backend</br></br>See https://developer.hashicorp.com/terraform/language/settings/backends/configuration |
+| TF007 | Low | open-source, inner-source, team, personal | Terraform modules should contain a main.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
+| TF008 | Low | open-source, inner-source, team, personal | Terraform modules should contain an outputs.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
+| TF009 | Low | open-source, inner-source, team, personal | Terraform modules should contain a variables.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
```

### Comparing `japr-1.0.1/pyproject.toml` & `japr-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "Japr"
-version = "1.0.1"
+version = "1.1.0"
 description = "A cross-language tool for rating the overall quality of open source, commercial and personal projects"
 authors = ["Jamie Read <hey@jread.dev>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "japr", from = "src"}]
 
 [tool.poetry.scripts]
 japr = "japr.japr:cli"
 generate_docs = "generate_ruleset_docs:generate"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-gitpython = "^3.1.30"
+gitpython = "^3.1.43"
 toml = "^0.10.2"
-pyyaml = "^6.0"
-jinja2 = "^3.1.2"
-pytest = "^7.3.1"
+pyyaml = "^6.0.1"
+jinja2 = "^3.1.3"
 
 [tool.poetry.group.dev.dependencies]
 pylama = "^8.4.1"
-black = "^22.12.0"
+black = "^24.4.2"
+pytest = "^8.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `japr-1.0.1/src/japr/check.py` & `japr-1.1.0/src/japr/check.py`

 * *Files identical despite different names*

### Comparing `japr-1.0.1/src/japr/check_providers/__init__.py` & `japr-1.1.0/src/japr/check_providers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from japr.check_providers.ci_check_provider import CiCheckProvider
 from japr.check_providers.python_check_provider import PythonCheckProvider
 from japr.check_providers.github_check_provider import GitHubCheckProvider
 from japr.check_providers.csharp_check_provider import CSharpCheckProvider
 from japr.check_providers.contributing_check_provider import ContributingCheckProvider
 from japr.check_providers.javascript_check_provider import JavascriptCheckProvider
 from japr.check_providers.rust_check_provider import RustCheckProvider
+from japr.check_providers.terraform_check_provider import TerraformCheckProvider
 
 check_providers = [
     ReadmeCheckProvider(),
     LicenseCheckProvider(),
     GitCheckProvider(),
     CiCheckProvider(),
     PythonCheckProvider(),
     GitHubCheckProvider(),
     CSharpCheckProvider(),
     ContributingCheckProvider(),
     JavascriptCheckProvider(),
     RustCheckProvider(),
+    TerraformCheckProvider(),
 ]
```

### Comparing `japr-1.0.1/src/japr/check_providers/ci_check_provider.py` & `japr-1.1.0/src/japr/check_providers/ci_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.0.1/src/japr/check_providers/contributing_check_provider.py` & `japr-1.1.0/src/japr/check_providers/contributing_check_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,24 +27,26 @@
 class ContributingCheckProvider(CheckProvider):
     def name(self):
         return "Contributing"
 
     def test(self, directory):
         yield CheckResult(
             "CT001",
-            Result.PASSED
-            if any(
-                [
-                    os.path.isfile(os.path.join(directory, "CONTRIBUTING.md")),
-                    os.path.isfile(os.path.join(directory, "CONTRIBUTING")),
-                    os.path.isfile(os.path.join(directory, "CONTRIBUTING.txt")),
-                    os.path.isfile(os.path.join(directory, "CONTRIBUTING.rst")),
-                ]
-            )
-            else Result.FAILED,
+            (
+                Result.PASSED
+                if any(
+                    [
+                        os.path.isfile(os.path.join(directory, "CONTRIBUTING.md")),
+                        os.path.isfile(os.path.join(directory, "CONTRIBUTING")),
+                        os.path.isfile(os.path.join(directory, "CONTRIBUTING.txt")),
+                        os.path.isfile(os.path.join(directory, "CONTRIBUTING.rst")),
+                    ]
+                )
+                else Result.FAILED
+            ),
             fix=AddContributorFix(),
         )
 
     def checks(self):
         return [
             Check(
                 "CT001",
```

### Comparing `japr-1.0.1/src/japr/check_providers/csharp_check_provider.py` & `japr-1.1.0/src/japr/check_providers/csharp_check_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,18 +80,20 @@
                     os.path.join(directory, cs_project)
                 )
                 has_enabled_net_analyzers = _has_enabled_net_analyzers_in_csproj(
                     os.path.join(directory, cs_project)
                 )
                 yield CheckResult(
                     "CS002",
-                    Result.PASSED
-                    if len(set(_linters).intersection(dependencies))
-                    or has_enabled_net_analyzers
-                    else Result.FAILED,
+                    (
+                        Result.PASSED
+                        if len(set(_linters).intersection(dependencies))
+                        or has_enabled_net_analyzers
+                        else Result.FAILED
+                    ),
                     cs_project,
                 )
                 has_enabled_nullable = _has_enabled_nullable_in_csproj(
                     os.path.join(directory, cs_project)
                 )
                 yield CheckResult(
                     "CS003",
@@ -101,17 +103,19 @@
                 has_enabled_treat_warnings_as_errors = (
                     _has_enabled_treat_warnings_as_errors(
                         os.path.join(directory, cs_project)
                     )
                 )
                 yield CheckResult(
                     "CS004",
-                    Result.PASSED
-                    if has_enabled_treat_warnings_as_errors
-                    else Result.FAILED,
+                    (
+                        Result.PASSED
+                        if has_enabled_treat_warnings_as_errors
+                        else Result.FAILED
+                    ),
                     cs_project,
                 )
         else:
             yield CheckResult("CS002", Result.NOT_APPLICABLE)
             yield CheckResult("CS003", Result.NOT_APPLICABLE)
             yield CheckResult("CS004", Result.NOT_APPLICABLE)
```

### Comparing `japr-1.0.1/src/japr/check_providers/git_check_provider.py` & `japr-1.1.0/src/japr/check_providers/git_check_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,17 +23,19 @@
                 "GI002", Result.PASSED if "origin" in repo.remotes else Result.FAILED
             )
             yield CheckResult(
                 "GI003", Result.PASSED if "master" not in repo.heads else Result.FAILED
             )
             yield CheckResult(
                 "GI004",
-                Result.PASSED
-                if os.path.isfile(os.path.join(directory, ".gitignore"))
-                else Result.FAILED,
+                (
+                    Result.PASSED
+                    if os.path.isfile(os.path.join(directory, ".gitignore"))
+                    else Result.FAILED
+                ),
             )
 
             ds_store_paths = [
                 f.path
                 for f in repo.tree("HEAD").list_traverse()
                 if f.type == "blob" and f.name == ".DS_Store"
             ]
```

### Comparing `japr-1.0.1/src/japr/check_providers/github_check_provider.py` & `japr-1.1.0/src/japr/check_providers/github_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.0.1/src/japr/check_providers/javascript_check_provider.py` & `japr-1.1.0/src/japr/check_providers/javascript_check_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,17 +48,19 @@
         if len(package_jsons) != 0:
             for package_json in package_jsons:
                 dependencies = _extract_dependencies_from_package_json(
                     os.path.join(directory, package_json)
                 )
                 yield CheckResult(
                     "JS002",
-                    Result.PASSED
-                    if len(set(_linters).intersection(dependencies))
-                    else Result.FAILED,
+                    (
+                        Result.PASSED
+                        if len(set(_linters).intersection(dependencies))
+                        else Result.FAILED
+                    ),
                     package_json,
                 )
 
                 # Check lock file is committed into Git
                 if repo is not None:
                     package_lock_file = os.path.join(
                         os.path.split(package_json)[0], "package-lock.json"
```

### Comparing `japr-1.0.1/src/japr/check_providers/license_check_provider.py` & `japr-1.1.0/src/japr/check_providers/license_check_provider.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 class LicenseCheckProvider(CheckProvider):
     def name(self):
         return "License"
 
     def test(self, directory):
         yield CheckResult(
             "LI001",
-            Result.PASSED
-            if any(
-                [
-                    os.path.isfile(os.path.join(directory, "LICENSE.md")),
-                    os.path.isfile(os.path.join(directory, "LICENSE")),
-                    os.path.isfile(os.path.join(directory, "LICENSE.txt")),
-                    os.path.isfile(os.path.join(directory, "LICENSE.rst")),
-                ]
-            )
-            else Result.FAILED,
+            (
+                Result.PASSED
+                if any(
+                    [
+                        os.path.isfile(os.path.join(directory, "LICENSE.md")),
+                        os.path.isfile(os.path.join(directory, "LICENSE")),
+                        os.path.isfile(os.path.join(directory, "LICENSE.txt")),
+                        os.path.isfile(os.path.join(directory, "LICENSE.rst")),
+                    ]
+                )
+                else Result.FAILED
+            ),
         )
 
     def checks(self):
         return [
             Check(
                 "LI001",
                 Severity.MEDIUM,
```

### Comparing `japr-1.0.1/src/japr/check_providers/python_check_provider.py` & `japr-1.1.0/src/japr/check_providers/python_check_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,17 +86,19 @@
         if len(pyproject_tomls) != 0 or len(pipfiles) != 0:
             for pyproject_toml in pyproject_tomls:
                 dependencies = _extract_dependencies_from_pyproject(
                     os.path.join(directory, pyproject_toml)
                 )
                 yield CheckResult(
                     "PY002",
-                    Result.PASSED
-                    if len(set(_linters).intersection(dependencies))
-                    else Result.FAILED,
+                    (
+                        Result.PASSED
+                        if len(set(_linters).intersection(dependencies))
+                        else Result.FAILED
+                    ),
                     pyproject_toml,
                 )
 
                 # Check lock file is committed into Git
                 if repo is not None:
                     lock_file = os.path.join(
                         os.path.split(pyproject_toml)[0], "poetry.lock"
@@ -120,17 +122,19 @@
 
             for pipfile in pipfiles:
                 dependencies = _extract_dependencies_from_pipfile(
                     os.path.join(directory, pipfile)
                 )
                 yield CheckResult(
                     "PY002",
-                    Result.PASSED
-                    if len(set(_linters).intersection(dependencies))
-                    else Result.FAILED,
+                    (
+                        Result.PASSED
+                        if len(set(_linters).intersection(dependencies))
+                        else Result.FAILED
+                    ),
                     pipfile,
                 )
 
                 # Check lock file is committed into Git
                 if repo is not None:
                     lock_file = pipfile + ".lock"
                     is_file_committed = any(
```

### Comparing `japr-1.0.1/src/japr/check_providers/readme_check_provider.py` & `japr-1.1.0/src/japr/check_providers/readme_check_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,46 +48,54 @@
         if readme_path is not None:
             with open(readme_path, "r") as readme_file:
                 content = readme_file.read()
 
             if readme_path.endswith(".rst"):
                 yield CheckResult(
                     "RE002",
-                    Result.PASSED
-                    if content.find("Install\n=") != -1
-                    or content.find("Setup\n=") != -1
-                    or content.find("Getting Started\n=") != -1
-                    or content.find("Quickstart\n=") != -1
-                    else Result.FAILED,
+                    (
+                        Result.PASSED
+                        if content.find("Install\n=") != -1
+                        or content.find("Setup\n=") != -1
+                        or content.find("Getting Started\n=") != -1
+                        or content.find("Quickstart\n=") != -1
+                        else Result.FAILED
+                    ),
                 )
                 yield CheckResult(
                     "RE003",
-                    Result.PASSED
-                    if content.find("Usage\n=") != -1
-                    or content.find("How-to\n=") != -1
-                    or content.find("API\n=") != -1
-                    else Result.FAILED,
+                    (
+                        Result.PASSED
+                        if content.find("Usage\n=") != -1
+                        or content.find("How-to\n=") != -1
+                        or content.find("API\n=") != -1
+                        else Result.FAILED
+                    ),
                 )
             else:
                 yield CheckResult(
                     "RE002",
-                    Result.PASSED
-                    if content.find("# Install") != -1
-                    or content.find("# Setup") != -1
-                    or content.find("# Getting Started") != -1
-                    or content.find("# Quickstart") != -1
-                    else Result.FAILED,
+                    (
+                        Result.PASSED
+                        if content.find("# Install") != -1
+                        or content.find("# Setup") != -1
+                        or content.find("# Getting Started") != -1
+                        or content.find("# Quickstart") != -1
+                        else Result.FAILED
+                    ),
                 )
                 yield CheckResult(
                     "RE003",
-                    Result.PASSED
-                    if content.find("# Usage") != -1
-                    or content.find("# How-to") != -1
-                    or content.find("# API") != -1
-                    else Result.FAILED,
+                    (
+                        Result.PASSED
+                        if content.find("# Usage") != -1
+                        or content.find("# How-to") != -1
+                        or content.find("# API") != -1
+                        else Result.FAILED
+                    ),
                 )
         else:
             yield CheckResult("RE002", Result.PRE_REQUISITE_CHECK_FAILED)
             yield CheckResult("RE003", Result.PRE_REQUISITE_CHECK_FAILED)
 
     def checks(self):
         return [
```

### Comparing `japr-1.0.1/src/japr/check_providers/rust_check_provider.py` & `japr-1.1.0/src/japr/check_providers/rust_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.0.1/src/japr/japr.py` & `japr-1.1.0/src/japr/japr.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
     def _print_result(self, result, check, profile_time, suppressed_checks):
         if (
             result.result == Result.FAILED and result.id not in suppressed_checks
         ) or self.is_profile:
             # Build up components then display for code clarity
             if result.result == Result.FAILED:
-                emoji_block = "\N{cross mark}"
+                emoji_block = "\N{CROSS MARK}"
             elif result.result == Result.PASSED:
-                emoji_block = "\N{white heavy check mark}"
+                emoji_block = "\N{WHITE HEAVY CHECK MARK}"
             elif result.result == Result.PRE_REQUISITE_CHECK_FAILED:
-                emoji_block = "\N{white question mark ornament}"
+                emoji_block = "\N{WHITE QUESTION MARK ORNAMENT}"
             else:
-                emoji_block = "\N{heavy minus sign}"
+                emoji_block = "\N{HEAVY MINUS SIGN}"
 
             if check.severity == Severity.HIGH:
                 severity_color = "\033[1;31m"
             elif check.severity == Severity.MEDIUM:
                 severity_color = "\033[1;33m"
             else:
                 severity_color = "\033[37m"
@@ -46,15 +46,15 @@
 
             if result.file_path is not None:
                 file_block = f"[{result.file_path}] "
             else:
                 file_block = ""
 
             if result.fix is not None:
-                fix_block = f" - A fix is available \N{wrench}"
+                fix_block = f" - A fix is available \N{WRENCH}"
             else:
                 fix_block = ""
 
             if self.is_summary:
                 print(
                     f"{severity_color}{check.severity.name.ljust(6)}\033[0;0m -"
                     f" \033[1m{check.id}\033[0;0m {file_block}{check.reason}"
@@ -75,17 +75,17 @@
                 print()
                 print(check.advice)
                 print()
                 print("-" * 10)
 
     def _print_fix_result(self, result):
         if result.is_fixed:
-            print(f"\N{white heavy check mark} {result.fix.success_message}")
+            print(f"\N{WHITE HEAVY CHECK MARK} {result.fix.success_message}")
         else:
-            print(f"\N{cross mark} {result.fix.failure_message}")
+            print(f"\N{CROSS MARK} {result.fix.failure_message}")
 
     def _print_json(
         self,
         issues,
         score,
         passed,
         failed,
@@ -121,16 +121,16 @@
         print(json.dumps(out, indent=2))
 
     def _print_summary(
         self, score, passed, failed, cannot_run, suppressed, fixed, failed_to_fix
     ):
         print(
             "\033[1mProject score: "
-            + "\N{glowing star}" * score
-            + "\N{heavy minus sign}" * (5 - score)
+            + "\N{GLOWING STAR}" * score
+            + "\N{HEAVY MINUS SIGN}" * (5 - score)
             + "\033[0;0m"
         )
 
         print(
             f"\033[1m\033[1;32mPassed: {passed}\033[0;0m, \033[1m\033[1;31mFailed:"
             f" {failed}\033[0;0m, \033[1m\033[1;37mCannot Run Yet: {cannot_run},"
             f" Suppressed {suppressed}\033[0;0m"
@@ -140,15 +140,15 @@
             print(
                 f"\033[1m\033[1;32mFixed: {fixed}\033[0;0m, \033[1m\033[1;31mFailed to"
                 f" Fix: {failed_to_fix}\033[0;0m"
             )
 
         if score == 5:
             print()
-            print("\033[1mCongratulations on a fantastic score \U0001F389\033[0;0m")
+            print("\033[1mCongratulations on a fantastic score \U0001f389\033[0;0m")
 
     def check_directory(
         self,
         directory,
         project_type,
     ):
         directory = os.path.abspath(directory)
```

### Comparing `japr-1.0.1/src/japr/template_util.py` & `japr-1.1.0/src/japr/template_util.py`

 * *Files identical despite different names*

### Comparing `japr-1.0.1/src/japr/templates/CONTRIBUTING.md` & `japr-1.1.0/src/japr/templates/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `japr-1.0.1/src/japr/templates/README.md` & `japr-1.1.0/src/japr/templates/README.md`

 * *Files identical despite different names*

### Comparing `japr-1.0.1/src/japr/templates/bug_report_issue_template.md` & `japr-1.1.0/src/japr/templates/bug_report_issue_template.md`

 * *Files identical despite different names*

### Comparing `japr-1.0.1/src/japr/templates/feature_request_issue_template.md` & `japr-1.1.0/src/japr/templates/feature_request_issue_template.md`

 * *Files identical despite different names*

### Comparing `japr-1.0.1/src/japr/templates/pull_request_template.md` & `japr-1.1.0/src/japr/templates/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `japr-1.0.1/src/japr/util.py` & `japr-1.1.0/src/japr/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # List of directories to immediately stop searching when looking for files
 # This is designed to be a short and non-comprehensive list mostly in the interest of search speed
 SKIP_DIRECTORIES = [
     # You know why this is skipped...
     "node_modules",
     # Stores git history as lots and lots of files we don't want to parse through
     ".git",
+    # Stores installed terraform modules and other autogenerated stuff
+    ".terraform",
 ]
 
 
 def _walk(base_path):
     with os.scandir(base_path) as scan:
         for obj in scan:
             if obj.is_dir() and obj.name not in SKIP_DIRECTORIES:
```

### Comparing `japr-1.0.1/PKG-INFO` & `japr-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: Japr
-Version: 1.0.1
+Version: 1.1.0
 Summary: A cross-language tool for rating the overall quality of open source, commercial and personal projects
 License: MIT
 Author: Jamie Read
 Author-email: hey@jread.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: gitpython (>=3.1.30,<4.0.0)
-Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: gitpython (>=3.1.43,<4.0.0)
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Jamie's Awesome Project Rater
 A cross-language tool for rating and enforcing the overall quality of projects by looking at tool & language setup
 
 It's a linter that makes sure you install linters (and some other stuff)
@@ -90,19 +89,19 @@
 ## Supported Languages
 Japr will work for projects of all languages however there are additional checks for the following:
 - Python
 - C#
 - Javascript
 
 The following table tracks the level of support for each language. Many languages also have additional checks not listed.
-|                       | Python         | C# | JS        | Rust  |
-|-----------------------|----------------|----|-----------|-------|
-| Linter setup          | ✅             | ✅ | ✅        |       |
-| Lock files in Git     | ✅             | ❌ | ✅        | ✅    |
-| Dependency Managers   | Poetry, Pipenv |    | NPM, Yarn | Cargo |
+|                       | Python         | C# | JS        | Rust  | Terraform |
+|-----------------------|----------------|----|-----------|-------|-----------|
+| Linter setup          | ✅             | ✅ | ✅        |       | ❌        |
+| Lock files in Git     | ✅             | ❌ | ✅        | ✅    | ✅        |
+| Dependency Managers   | Poetry, Pipenv |    | NPM, Yarn | Cargo |           |
 
 ## Experimental Automatic Fixes
 Japr can automatically fix some issues when supplied the `--fix` flag. **This functionality is highly expermental**
 
 ## Development
 Pull requsts are welcome. Please read [the contributing guide first](./CONTRIBUTING.md).
 
@@ -217,8 +216,22 @@
 
 ### Javascript
 | ID | Severity | Enabled for Project Types | Description | Advice |
 |----|----------|---------------------------|-------------|--------|
 | JS002 | Medium | open-source, inner-source, team | Javascript projects should have a linter configured | Javascript projects should have a comprehensive linter configured such as ESLint in order to ensure a consistent code style is used across all files and by all contributors.</br></br>Having a consistent style helps ensure readability and ease of understanding for any outsider looking into the project's code. Linters can also improve the stability of the code by catching mistakes before the code is published. |
 | JS004 | Medium | open-source, inner-source, team, personal | Javascript projects should have their lock files committed into Git | When using a dependency manager for Javascript such as npm, the lock files should be comitted into Git. This ensures that all dependencies of packages are installed at the same version no matter when and on what machine the project is installed. |
 
+### Rust
+| ID | Severity | Enabled for Project Types | Description | Advice |
+|----|----------|---------------------------|-------------|--------|
+| RS004 | Medium | open-source, inner-source, team, personal | Rust projects should have their Cargo lock files committed into Git | When using Cargo for Rust, the lock files should be comitted into Git. This ensures that all dependencies of packages are installed at the same version no matter when and on what machine the project is installed. |
+
+### Terraform
+| ID | Severity | Enabled for Project Types | Description | Advice |
+|----|----------|---------------------------|-------------|--------|
+| TF004 | Medium | open-source, inner-source, team, personal | Terraform projects should have their Terraform lock files committed into Git | When using Terraform, the lock files should be comitted into Git. This ensures that all dependencies of packages are installed at the same version no matter when and on what machine the project is installed. |
+| TF005 | Medium | open-source, inner-source, team, personal | Terraform projects should not have their .terraform directory committed into Git | The .terraform directory contains binaries, thrid party modules and other things that are generated during a terraform init. This folder should not be committed into git. |
+| TF006 | High | open-source, inner-source, team, personal | Terraform state files should not be committed into git | Terraform state files can contain secrets and are stored unencrypted. These secrets can be easily leaked when stored in git. Additionally, terraform state in git does not provide a single source of truth nor state locking and so can cause major issues when used in teams.</br></br>Instead of storing state in git, use another terraform backend</br></br>See https://developer.hashicorp.com/terraform/language/settings/backends/configuration |
+| TF007 | Low | open-source, inner-source, team, personal | Terraform modules should contain a main.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
+| TF008 | Low | open-source, inner-source, team, personal | Terraform modules should contain an outputs.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
+| TF009 | Low | open-source, inner-source, team, personal | Terraform modules should contain a variables.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
```

