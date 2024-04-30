# Comparing `tmp/llama_index_readers_github-0.1.7.tar.gz` & `tmp/llama_index_readers_github-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_github-0.1.7.tar", max compression
+gzip compressed data, was "llama_index_readers_github-0.1.8.tar", max compression
```

## Comparing `llama_index_readers_github-0.1.7.tar` & `llama_index_readers_github-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       41 2024-02-16 00:43:38.375451 llama_index_readers_github-0.1.7/README.md
--rw-r--r--   0        0        0      491 2024-02-16 00:43:38.375451 llama_index_readers_github-0.1.7/llama_index/readers/github/__init__.py
--rw-r--r--   0        0        0        0 2024-02-16 00:43:38.405451 llama_index_readers_github-0.1.7/llama_index/readers/github/collaborators/__init__.py
--rw-r--r--   0        0        0     5944 2024-02-16 00:43:38.405451 llama_index_readers_github-0.1.7/llama_index/readers/github/collaborators/base.py
--rw-r--r--   0        0        0     5917 2024-02-16 00:43:38.405451 llama_index_readers_github-0.1.7/llama_index/readers/github/collaborators/github_client.py
--rw-r--r--   0        0        0        0 2024-02-16 00:43:38.405451 llama_index_readers_github-0.1.7/llama_index/readers/github/issues/__init__.py
--rw-r--r--   0        0        0     7826 2024-02-21 23:57:36.350386 llama_index_readers_github-0.1.7/llama_index/readers/github/issues/base.py
--rw-r--r--   0        0        0     6496 2024-02-16 00:43:38.405451 llama_index_readers_github-0.1.7/llama_index/readers/github/issues/github_client.py
--rw-r--r--   0        0        0        0 2024-02-16 00:43:38.405451 llama_index_readers_github-0.1.7/llama_index/readers/github/repository/__init__.py
--rw-r--r--   0        0        0    21262 2024-02-22 22:34:52.919489 llama_index_readers_github-0.1.7/llama_index/readers/github/repository/base.py
--rw-r--r--   0        0        0    15317 2024-02-22 22:34:52.919489 llama_index_readers_github-0.1.7/llama_index/readers/github/repository/github_client.py
--rw-r--r--   0        0        0     5614 2024-02-21 23:57:36.350386 llama_index_readers_github-0.1.7/llama_index/readers/github/repository/utils.py
--rw-r--r--   0        0        0     1744 2024-02-22 22:48:55.418406 llama_index_readers_github-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 llama_index_readers_github-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2113 2024-04-30 16:55:06.385854 llama_index_readers_github-0.1.8/README.md
+-rw-r--r--   0        0        0      555 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/collaborators/__init__.py
+-rw-r--r--   0        0        0     5944 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/collaborators/base.py
+-rw-r--r--   0        0        0     5917 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/collaborators/github_client.py
+-rw-r--r--   0        0        0        0 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/issues/__init__.py
+-rw-r--r--   0        0        0     7826 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/issues/base.py
+-rw-r--r--   0        0        0     6496 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/issues/github_client.py
+-rw-r--r--   0        0        0        0 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/repository/__init__.py
+-rw-r--r--   0        0        0    21522 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/repository/base.py
+-rw-r--r--   0        0        0    15377 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/repository/github_client.py
+-rw-r--r--   0        0        0     5614 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/repository/utils.py
+-rw-r--r--   0        0        0     1744 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 llama_index_readers_github-0.1.8/PKG-INFO
```

### Comparing `llama_index_readers_github-0.1.7/llama_index/readers/github/collaborators/base.py` & `llama_index_readers_github-0.1.8/llama_index/readers/github/collaborators/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.7/llama_index/readers/github/collaborators/github_client.py` & `llama_index_readers_github-0.1.8/llama_index/readers/github/collaborators/github_client.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.7/llama_index/readers/github/issues/base.py` & `llama_index_readers_github-0.1.8/llama_index/readers/github/issues/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.7/llama_index/readers/github/issues/github_client.py` & `llama_index_readers_github-0.1.8/llama_index/readers/github/issues/github_client.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.7/llama_index/readers/github/repository/base.py` & `llama_index_readers_github-0.1.8/llama_index/readers/github/repository/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,23 @@
     Github repository reader.
 
     Retrieves the contents of a Github repository and returns a list of documents.
     The documents are either the contents of the files in the repository or the text
     extracted from the files using the parser.
 
     Examples:
-        >>> reader = GithubRepositoryReader("owner", "repo")
+        >>> client = github_client = GithubClient(
+        ...    github_token=os.environ["GITHUB_TOKEN"],
+        ...    verbose=True
+        ... )
+        >>> reader = GithubRepositoryReader(
+        ...    github_client=github_client,
+        ...    owner="run-llama",
+        ...    repo="llama_index",
+        ... )
         >>> branch_documents = reader.load_data(branch="branch")
         >>> commit_documents = reader.load_data(commit_sha="commit_sha")
 
     """
 
     class FilterType(enum.Enum):
         """
```

### Comparing `llama_index_readers_github-0.1.7/llama_index/readers/github/repository/github_client.py` & `llama_index_readers_github-0.1.8/llama_index/readers/github/repository/github_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 This module contains the Github API client for the GPT-Index library.
 It is used by the Github readers to retrieve the data from Github.
 """
 
 import os
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Protocol
 
-from dataclasses_json import DataClassJsonMixin
+from dataclasses_json import DataClassJsonMixin, config
 
 
 @dataclass
 class GitTreeResponseModel(DataClassJsonMixin):
     """
     Dataclass for the response from the Github API's getTree endpoint.
 
@@ -138,15 +138,15 @@
 
             tree: Tree
 
         commit: Commit
 
     @dataclass
     class Links(DataClassJsonMixin):
-        self: str
+        _self: str = field(metadata=config(field_name="self"))
         html: str
 
     commit: Commit
     name: str
     _links: Links
```

### Comparing `llama_index_readers_github-0.1.7/llama_index/readers/github/repository/utils.py` & `llama_index_readers_github-0.1.8/llama_index/readers/github/repository/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.7/pyproject.toml` & `llama_index_readers_github-0.1.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 description = "llama-index readers github integration"
 exclude = ["**/BUILD"]
 keywords = ["code", "collaborators", "git", "github", "issues", "placeholder", "repository", "source code"]
 license = "MIT"
 maintainers = ["ahmetkca", "moncho", "rwood-97"]
 name = "llama-index-readers-github"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-readers-file = "^0.1.1"
 httpx = ">=0.26.0"
```

