# Comparing `tmp/gitblog2-2.1.3.tar.gz` & `tmp/gitblog2-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitblog2-2.1.3.tar", max compression
+gzip compressed data, was "gitblog2-2.1.4.tar", max compression
```

## Comparing `gitblog2-2.1.3.tar` & `gitblog2-2.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-02-18 16:19:17.029548 gitblog2-2.1.3/LICENSE
--rw-r--r--   0        0        0      261 2023-04-08 12:33:53.131324 gitblog2-2.1.3/build.py
--rw-r--r--   0        0        0     3230 2024-01-21 12:38:57.005522 gitblog2-2.1.3/docs/index.md
--rw-r--r--   0        0        0       25 2023-02-18 16:19:17.029548 gitblog2-2.1.3/gitblog2/__init__.py
--rw-r--r--   0        0        0     2766 2024-01-21 12:53:51.615585 gitblog2-2.1.3/gitblog2/blog_posts.py
--rwxr-xr-x   0        0        0     1918 2023-09-25 10:56:07.538590 gitblog2-2.1.3/gitblog2/cli.py
--rw-r--r--   0        0        0    15850 2024-01-21 13:01:17.531760 gitblog2-2.1.3/gitblog2/lib.py
--rw-r--r--   0        0        0      362 2023-04-22 16:58:21.192330 gitblog2-2.1.3/gitblog2/media/favicon.svg
--rw-r--r--   0        0        0     7951 2023-09-27 15:11:44.319193 gitblog2-2.1.3/gitblog2/media/icons.svg
--rw-r--r--   0        0        0      541 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/repo_utils.py
--rw-r--r--   0        0        0     6749 2024-01-21 12:57:11.805293 gitblog2-2.1.3/gitblog2/style.css
--rw-r--r--   0        0        0     1004 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/templates/article.html.j2
--rw-r--r--   0        0        0      650 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/templates/footer.html.j2
--rw-r--r--   0        0        0      327 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/templates/head_common.html.j2
--rw-r--r--   0        0        0      867 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/templates/index.html.j2
--rw-r--r--   0        0        0      360 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/templates/navbar.html.j2
--rw-r--r--   0        0        0     1184 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/tests/example_output/index.html
--rw-r--r--   0        0        0      362 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/tests/example_output/media/favicon.svg
--rw-r--r--   0        0        0     7951 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/tests/example_output/media/icons.svg
--rw-r--r--   0        0        0     6749 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/tests/example_output/style.css
--rw-r--r--   0        0        0     3398 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/tests/example_output/tech/example.html
--rw-r--r--   0        0        0     1184 2024-01-21 12:38:57.005522 gitblog2-2.1.3/gitblog2/tests/example_output/tech/index.html
--rw-r--r--   0        0        0      976 2024-01-21 13:00:58.435560 gitblog2-2.1.3/gitblog2/tests/test_e2e.py
--rw-r--r--   0        0        0      757 2024-01-21 13:17:40.020137 gitblog2-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     3987 1970-01-01 00:00:00.000000 gitblog2-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-18 16:19:17.029548 gitblog2-2.1.4/LICENSE
+-rw-r--r--   0        0        0      261 2023-04-08 12:33:53.131324 gitblog2-2.1.4/build.py
+-rw-r--r--   0        0        0     5724 2024-04-30 20:29:05.248299 gitblog2-2.1.4/docs/index.md
+-rw-r--r--   0        0        0       25 2023-02-18 16:19:17.029548 gitblog2-2.1.4/gitblog2/__init__.py
+-rw-r--r--   0        0        0     2766 2024-01-21 12:53:51.615585 gitblog2-2.1.4/gitblog2/blog_posts.py
+-rwxr-xr-x   0        0        0     1918 2024-04-30 20:42:27.991108 gitblog2-2.1.4/gitblog2/cli.py
+-rw-r--r--   0        0        0    15850 2024-01-21 13:01:17.531760 gitblog2-2.1.4/gitblog2/lib.py
+-rw-r--r--   0        0        0      362 2023-04-22 16:58:21.192330 gitblog2-2.1.4/gitblog2/media/favicon.svg
+-rw-r--r--   0        0        0     7951 2023-09-27 15:11:44.319193 gitblog2-2.1.4/gitblog2/media/icons.svg
+-rw-r--r--   0        0        0      541 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/repo_utils.py
+-rw-r--r--   0        0        0     6749 2024-01-21 13:21:02.245051 gitblog2-2.1.4/gitblog2/style.css
+-rw-r--r--   0        0        0     1004 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/templates/article.html.j2
+-rw-r--r--   0        0        0      650 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/templates/footer.html.j2
+-rw-r--r--   0        0        0      327 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/templates/head_common.html.j2
+-rw-r--r--   0        0        0      867 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/templates/index.html.j2
+-rw-r--r--   0        0        0      360 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/templates/navbar.html.j2
+-rw-r--r--   0        0        0     1184 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/tests/example_output/index.html
+-rw-r--r--   0        0        0      362 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/tests/example_output/media/favicon.svg
+-rw-r--r--   0        0        0     7951 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/tests/example_output/media/icons.svg
+-rw-r--r--   0        0        0     6749 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/tests/example_output/style.css
+-rw-r--r--   0        0        0     3398 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/tests/example_output/tech/example.html
+-rw-r--r--   0        0        0     1184 2024-01-21 12:38:57.005522 gitblog2-2.1.4/gitblog2/tests/example_output/tech/index.html
+-rw-r--r--   0        0        0      951 2024-04-30 20:54:51.750226 gitblog2-2.1.4/gitblog2/tests/test_e2e.py
+-rw-r--r--   0        0        0      758 2024-04-30 20:29:15.816360 gitblog2-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6481 1970-01-01 00:00:00.000000 gitblog2-2.1.4/PKG-INFO
```

### Comparing `gitblog2-2.1.3/LICENSE` & `gitblog2-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/blog_posts.py` & `gitblog2-2.1.4/gitblog2/blog_posts.py`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/cli.py` & `gitblog2-2.1.4/gitblog2/cli.py`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/lib.py` & `gitblog2-2.1.4/gitblog2/lib.py`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/media/icons.svg` & `gitblog2-2.1.4/gitblog2/media/icons.svg`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/repo_utils.py` & `gitblog2-2.1.4/gitblog2/repo_utils.py`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/style.css` & `gitblog2-2.1.4/gitblog2/style.css`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/templates/article.html.j2` & `gitblog2-2.1.4/gitblog2/templates/article.html.j2`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/templates/footer.html.j2` & `gitblog2-2.1.4/gitblog2/templates/footer.html.j2`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/templates/index.html.j2` & `gitblog2-2.1.4/gitblog2/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/tests/example_output/index.html` & `gitblog2-2.1.4/gitblog2/tests/example_output/index.html`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/tests/example_output/media/icons.svg` & `gitblog2-2.1.4/gitblog2/tests/example_output/media/icons.svg`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/tests/example_output/style.css` & `gitblog2-2.1.4/gitblog2/tests/example_output/style.css`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/tests/example_output/tech/example.html` & `gitblog2-2.1.4/gitblog2/tests/example_output/tech/example.html`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/gitblog2/tests/example_output/tech/index.html` & `gitblog2-2.1.4/gitblog2/tests/example_output/tech/index.html`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.3/pyproject.toml` & `gitblog2-2.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitblog2"
-version = "2.1.3"
+version = "2.1.4"
 description = "Git + Markdown = blog"
 authors = ["Henri Hannetel <henri.hannetel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "gitblog2" }]
 include = ["gitblog2/*"]
 exclude = ["gitblog2/tests"]
@@ -30,8 +30,8 @@
 script = "build.py"
 
 [tool.pyright]
 include = ["gitblog2"]
 stubPath = "typings"
 
 [tool.poetry.group.test.dependencies]
-pytest = ">=7.4.4"
+pytest = ">=7.4.4"
```

