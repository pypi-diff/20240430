# Comparing `tmp/tgwrap-0.9.1.tar.gz` & `tmp/tgwrap-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.9.1.tar", max compression
+gzip compressed data, was "tgwrap-0.9.2.tar", max compression
```

## Comparing `tgwrap-0.9.1.tar` & `tgwrap-0.9.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.9.1/LICENSE
--rw-r--r--   0        0        0    12159 2024-04-24 11:33:21.171629 tgwrap-0.9.1/README.md
--rw-r--r--   0        0        0      922 2024-04-29 11:10:57.134281 tgwrap-0.9.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.9.1/tgwrap/__init__.py
--rw-r--r--   0        0        0     8726 2023-10-20 14:35:12.875311 tgwrap-0.9.1/tgwrap/analyze.py
--rwxr-xr-x   0        0        0    29727 2024-04-24 07:14:54.956803 tgwrap-0.9.1/tgwrap/cli.py
--rw-r--r--   0        0        0    10243 2024-04-29 11:10:37.178306 tgwrap-0.9.1/tgwrap/deploy.py
--rwxr-xr-x   0        0        0    80691 2024-04-24 11:32:17.978883 tgwrap-0.9.1/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.9.1/tgwrap/printer.py
--rw-r--r--   0        0        0    13334 1970-01-01 00:00:00.000000 tgwrap-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.9.2/LICENSE
+-rw-r--r--   0        0        0    12159 2024-04-24 11:33:21.171629 tgwrap-0.9.2/README.md
+-rw-r--r--   0        0        0      922 2024-04-30 12:18:23.521352 tgwrap-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.9.2/tgwrap/__init__.py
+-rw-r--r--   0        0        0     8726 2023-10-20 14:35:12.875311 tgwrap-0.9.2/tgwrap/analyze.py
+-rwxr-xr-x   0        0        0    29727 2024-04-24 07:14:54.956803 tgwrap-0.9.2/tgwrap/cli.py
+-rw-r--r--   0        0        0    10243 2024-04-29 11:10:37.178306 tgwrap-0.9.2/tgwrap/deploy.py
+-rwxr-xr-x   0        0        0    81157 2024-04-30 12:17:52.165017 tgwrap-0.9.2/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.9.2/tgwrap/printer.py
+-rw-r--r--   0        0        0    13334 1970-01-01 00:00:00.000000 tgwrap-0.9.2/PKG-INFO
```

### Comparing `tgwrap-0.9.1/LICENSE` & `tgwrap-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.1/README.md` & `tgwrap-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.1/pyproject.toml` & `tgwrap-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.9.1"
+version = "0.9.2"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
```

### Comparing `tgwrap-0.9.1/tgwrap/analyze.py` & `tgwrap-0.9.2/tgwrap/analyze.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.1/tgwrap/cli.py` & `tgwrap-0.9.2/tgwrap/cli.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.1/tgwrap/deploy.py` & `tgwrap-0.9.2/tgwrap/deploy.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.1/tgwrap/main.py` & `tgwrap-0.9.2/tgwrap/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -777,14 +777,20 @@
             self.printer.verbose(f'Executed {group_nbr} groups and {total_items} steps')
 
     def _post_analyze_results_to_dce(self, data_collection_endpoint:str, payload:object):
         """
         Posts the payload to the given (Azure) data collection endpoint
         """
 
+        def mask_basic_auth(url):
+            # Regular expression to match basic authentication credentials in URL
+            auth_pattern = re.compile(r"(https?://)([^:@]+):([^:@]+)@(.+)")
+            # Return the url without the basic auth part
+            return auth_pattern.sub(r"\1\4", url)
+
         #
         # Everything we do here, can be done using native python. And probably this is preferable as well.
         # But I have decided to follow (at least for now) the overall approach of the app and that is
         # executing systems commands.
         # This does require the az cli to be installed, but that is a fair assumption if you are working
         # with terragrunt/terraform and want to post the analyze results to a Data Collection Endpoint.
         # However, not ruling out this will change, but then the change should be transparant.
@@ -850,14 +856,17 @@
             raise Exception(f'Could not get git repo info')
         
         # Get the ouptut
         repo = rc.stdout.decode().rstrip('\n')
         if not repo:
             raise Exception(f'Could not get git repo info: {repo}')
 
+        # Remove the basic auth info if it is part of the url
+        repo = mask_basic_auth(repo)
+
         # Get the current path in the repo
         rc = subprocess.run(
             shlex.split('git rev-parse --show-prefix'),
             check=True,
             stdout=subprocess.PIPE,
             stderr=sys.stderr,
         )
@@ -904,14 +913,15 @@
             resp = requests.post(
                 url=data_collection_endpoint,
                 headers=headers,
                 json=dce_payload,
             )
 
             resp.raise_for_status()
+            self.printer.success('Analyze results logged to DCE')
 
         except requests.exceptions.RequestException as e:
             # we warn but continue
             self.printer.warning(f'Error while posting the analyze results ({type(e)}): {e}')
         except Exception as e:
             self.printer.error(f'Unexpected error: {e}')
             if self.printer.print_verbose:
```

### Comparing `tgwrap-0.9.1/tgwrap/printer.py` & `tgwrap-0.9.2/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.1/PKG-INFO` & `tgwrap-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgwrap
-Version: 0.9.1
+Version: 0.9.2
 Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
 Home-page: https://gitlab.com/lunadata/tgwrap
 License: MIT
 Keywords: terraform,terragrunt,terrasafe,python
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.8,<4.0
```

