# Comparing `tmp/whoisit-2.7.4.tar.gz` & `tmp/whoisit-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whoisit-2.7.4.tar", last modified: Sat Apr 20 06:10:52 2024, max compression
+gzip compressed data, was "whoisit-2.7.5.tar", last modified: Tue Apr 30 08:53:57 2024, max compression
```

## Comparing `whoisit-2.7.4.tar` & `whoisit-2.7.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-20 06:10:52.156591 whoisit-2.7.4/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1528 2021-06-06 06:10:53.000000 whoisit-2.7.4/LICENSE
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2021-06-10 06:05:53.000000 whoisit-2.7.4/MANIFEST.in
--rw-r--r--   0 meeb      (1000) meeb      (1000)    21721 2024-04-20 06:10:52.156591 whoisit-2.7.4/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    20802 2022-07-08 03:09:28.000000 whoisit-2.7.4/README.md
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2022-12-06 10:28:45.000000 whoisit-2.7.4/requirements.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2024-04-20 06:10:52.156591 whoisit-2.7.4/setup.cfg
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1359 2024-04-20 06:08:12.000000 whoisit-2.7.4/setup.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-20 06:10:52.152591 whoisit-2.7.4/tests/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-06-06 06:14:06.000000 whoisit-2.7.4/tests/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    11786 2022-12-06 10:28:45.000000 whoisit-2.7.4/tests/test_bootstrap.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21934 2022-12-06 10:28:45.000000 whoisit-2.7.4/tests/test_parser.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5150 2021-11-18 03:52:35.000000 whoisit-2.7.4/tests/test_query.py
--rw-r--r--   0 meeb      (1000) meeb      (1000)     2070 2023-06-03 08:56:21.000000 whoisit-2.7.4/tests/test_ssl.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-20 06:10:52.156591 whoisit-2.7.4/whoisit/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     3009 2024-04-20 06:05:08.000000 whoisit-2.7.4/whoisit/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    17741 2023-06-03 08:55:54.000000 whoisit-2.7.4/whoisit/bootstrap.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      937 2022-12-06 10:28:45.000000 whoisit-2.7.4/whoisit/errors.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      522 2021-06-08 06:47:34.000000 whoisit-2.7.4/whoisit/logger.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1897 2024-03-23 08:51:07.000000 whoisit-2.7.4/whoisit/overrides.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    16104 2024-04-20 06:03:35.000000 whoisit-2.7.4/whoisit/parser.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     8965 2023-06-03 07:58:57.000000 whoisit-2.7.4/whoisit/query.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     3940 2023-07-10 18:02:01.000000 whoisit-2.7.4/whoisit/utils.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       18 2024-04-20 06:08:20.000000 whoisit-2.7.4/whoisit/version.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-20 06:10:52.156591 whoisit-2.7.4/whoisit.egg-info/
--rw-r--r--   0 meeb      (1000) meeb      (1000)    21721 2024-04-20 06:10:52.000000 whoisit-2.7.4/whoisit.egg-info/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      489 2024-04-20 06:10:52.000000 whoisit-2.7.4/whoisit.egg-info/SOURCES.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2024-04-20 06:10:52.000000 whoisit-2.7.4/whoisit.egg-info/dependency_links.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2024-04-20 06:10:52.000000 whoisit-2.7.4/whoisit.egg-info/requires.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2024-04-20 06:10:52.000000 whoisit-2.7.4/whoisit.egg-info/top_level.txt
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-30 08:53:57.627621 whoisit-2.7.5/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1528 2021-06-06 06:10:53.000000 whoisit-2.7.5/LICENSE
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2021-06-10 06:05:53.000000 whoisit-2.7.5/MANIFEST.in
+-rw-r--r--   0 meeb      (1000) meeb      (1000)    21788 2024-04-30 08:53:57.627621 whoisit-2.7.5/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    20869 2024-04-30 08:32:40.000000 whoisit-2.7.5/README.md
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2022-12-06 10:28:45.000000 whoisit-2.7.5/requirements.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2024-04-30 08:53:57.627621 whoisit-2.7.5/setup.cfg
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1359 2024-04-30 08:52:25.000000 whoisit-2.7.5/setup.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-30 08:53:57.627621 whoisit-2.7.5/tests/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-06-06 06:14:06.000000 whoisit-2.7.5/tests/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    11786 2022-12-06 10:28:45.000000 whoisit-2.7.5/tests/test_bootstrap.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    21934 2022-12-06 10:28:45.000000 whoisit-2.7.5/tests/test_parser.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5150 2021-11-18 03:52:35.000000 whoisit-2.7.5/tests/test_query.py
+-rw-r--r--   0 meeb      (1000) meeb      (1000)     2070 2023-06-03 08:56:21.000000 whoisit-2.7.5/tests/test_ssl.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-30 08:53:57.627621 whoisit-2.7.5/whoisit/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     3000 2024-04-30 08:46:41.000000 whoisit-2.7.5/whoisit/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    17741 2023-06-03 08:55:54.000000 whoisit-2.7.5/whoisit/bootstrap.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      937 2022-12-06 10:28:45.000000 whoisit-2.7.5/whoisit/errors.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      522 2021-06-08 06:47:34.000000 whoisit-2.7.5/whoisit/logger.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1897 2024-03-23 08:51:07.000000 whoisit-2.7.5/whoisit/overrides.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    16222 2024-04-30 08:49:55.000000 whoisit-2.7.5/whoisit/parser.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     8965 2023-06-03 07:58:57.000000 whoisit-2.7.5/whoisit/query.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     4147 2024-04-30 08:46:33.000000 whoisit-2.7.5/whoisit/utils.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       18 2024-04-30 08:52:38.000000 whoisit-2.7.5/whoisit/version.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-30 08:53:57.627621 whoisit-2.7.5/whoisit.egg-info/
+-rw-r--r--   0 meeb      (1000) meeb      (1000)    21788 2024-04-30 08:53:57.000000 whoisit-2.7.5/whoisit.egg-info/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      489 2024-04-30 08:53:57.000000 whoisit-2.7.5/whoisit.egg-info/SOURCES.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2024-04-30 08:53:57.000000 whoisit-2.7.5/whoisit.egg-info/dependency_links.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2024-04-30 08:53:57.000000 whoisit-2.7.5/whoisit.egg-info/requires.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2024-04-30 08:53:57.000000 whoisit-2.7.5/whoisit.egg-info/top_level.txt
```

### Comparing `whoisit-2.7.4/LICENSE` & `whoisit-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.4/PKG-INFO` & `whoisit-2.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisit
-Version: 2.7.4
+Version: 2.7.5
 Summary: A Python client to RDAP WHOIS-like services for internet resources.
 Home-page: https://github.com/meeb/whoisit
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: BSD
 Keywords: whoisit,whois,rdap,ip,network,cidr,prefix,domain,asn,autnum,tld,entity,handle,arin,afrinic,apnic,ripe,lacnic
 Classifier: Development Status :: 5 - Production/Stable
@@ -336,14 +336,15 @@
 ```
 
 ### Additional domain response data
 
 ```python
 # Domain response data includes all shared general response fields above and also:
 response = {
+    'unicode_name': str,     # Domain name in unicode if available
     'nameservers': list,     # List of name servers for the domain as strings
     'status': list,          # List of the domain states as strings
 }
 ```
 
 ### Additional IP response data
```

### Comparing `whoisit-2.7.4/README.md` & `whoisit-2.7.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -313,14 +313,15 @@
 ```
 
 ### Additional domain response data
 
 ```python
 # Domain response data includes all shared general response fields above and also:
 response = {
+    'unicode_name': str,     # Domain name in unicode if available
     'nameservers': list,     # List of name servers for the domain as strings
     'status': list,          # List of the domain states as strings
 }
 ```
 
 ### Additional IP response data
```

### Comparing `whoisit-2.7.4/setup.py` & `whoisit-2.7.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 
-version = '2.7.4'
+version = '2.7.5'
 
 
 with open('README.md', 'rt') as f:
     long_description = f.read()
 
 
 with open('requirements.txt', 'rt') as f:
```

### Comparing `whoisit-2.7.4/tests/test_bootstrap.py` & `whoisit-2.7.5/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.4/tests/test_parser.py` & `whoisit-2.7.5/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.4/tests/test_query.py` & `whoisit-2.7.5/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.4/tests/test_ssl.py` & `whoisit-2.7.5/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.4/whoisit/__init__.py` & `whoisit-2.7.5/whoisit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from .bootstrap import Bootstrap
 from .query import QueryBuilder, Query
 from .parser import parse
 from .logger import get_logger
-from .utils import create_session, get_session
+from .utils import create_session, get_session, recursive_merge
 from .version import version
 
 
 # Private methods
 
 
 _bootstrap = Bootstrap()
@@ -50,22 +50,22 @@
     # an upstream RDAP endpoint that may have more information
     relresponse = None
     for link in response.get('links', []):
         rel = link.get('rel', '')
         if rel in ('related', 'registration'):
             relhref = link.get('href', '')
             if relhref:
-                print(f'MAKING SUBREQUEST TO {relhref}')
                 relq = Query(session, method, relhref)
                 relresponse = relq.request()
                 break
     if relresponse:
-        return parse(_bootstrap, 'domain', domain_name, relresponse)
-    else:
-        return parse(_bootstrap, 'domain', domain_name, response)
+        # Overlay the related response over the original response
+        recursive_merge(response, relresponse)
+    return parse(_bootstrap, 'domain', domain_name, response)
+
 
 def ip(ip_address_or_network, rir=None, raw=False, allow_insecure_ssl=False, session=None):
     session = get_session(session, allow_insecure_ssl=allow_insecure_ssl)
     method, url, exact_match = build_query(
         query_type='ip', query_value=ip_address_or_network, rir=rir)
     q = Query(session, method, url)
     response = q.request()
```

### Comparing `whoisit-2.7.4/whoisit/bootstrap.py` & `whoisit-2.7.5/whoisit/bootstrap.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.4/whoisit/errors.py` & `whoisit-2.7.5/whoisit/errors.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.4/whoisit/logger.py` & `whoisit-2.7.5/whoisit/logger.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.4/whoisit/overrides.py` & `whoisit-2.7.5/whoisit/overrides.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.4/whoisit/parser.py` & `whoisit-2.7.5/whoisit/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,23 +154,23 @@
         self.parsed['registration_date'] = None
         self.parsed['expiration_date'] = None
         for event in self.raw_data.get('events', []):
             action = event.get('eventAction').strip().lower()
             if action == 'last changed':
                 last_changed_date = event.get('eventDate', '')
                 if last_changed_date:
-                    self.parsed['last_changed_date'] = dateutil_parse(last_changed_date)
+                    self.parsed['last_changed_date'] = dateutil_parse(last_changed_date, fuzzy=True)
             elif action == 'registration':
                 registration_date = event.get('eventDate', '')
                 if registration_date:
-                    self.parsed['registration_date'] = dateutil_parse(registration_date)
+                    self.parsed['registration_date'] = dateutil_parse(registration_date, fuzzy=True)
             elif action == 'expiration':
                 expiration_date = event.get('eventDate', '')
                 if expiration_date:
-                    self.parsed['expiration_date'] = dateutil_parse(expiration_date)
+                    self.parsed['expiration_date'] = dateutil_parse(expiration_date, fuzzy=True)
 
     def extract_self_link(self):
         self.parsed['url'] = ''
         for link in self.raw_data.get('links', []):
             if link.get('rel', '').strip().lower() == 'self':
                 self.parsed['url'] = clean(link.get('href', ''))
         else:
@@ -272,14 +272,15 @@
         self.extract_domain_nameservers()
         self.extract_domain_status()
         self.extract_domain_dnssec()
         return self.parsed
 
     def extract_domain_name(self):
         self.parsed['name'] = clean(self.raw_data.get('ldhName', ''))
+        self.parsed['unicode_name'] = clean(self.raw_data.get('unicodeName', ''))
 
     def extract_domain_nameservers(self):
         self.parsed['nameservers'] = []
         for nameserver in self.raw_data.get('nameservers', []):
             if nameserver.get('objectClassName', '') == 'nameserver':
                 nameserver = nameserver.get('ldhName', '')
                 if nameserver:
```

### Comparing `whoisit-2.7.4/whoisit/query.py` & `whoisit-2.7.5/whoisit/query.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.4/whoisit/utils.py` & `whoisit-2.7.5/whoisit/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,7 +101,15 @@
 
 
 def contains_only_chars(s, chars=default_chars):
     for c in s:
         if c not in chars:
             return False
     return True
+
+
+def recursive_merge(d1, d2):
+    for k, v in d2.items():
+        if k in d1 and isinstance(d1[k], dict) and isinstance(v, dict):
+            recursive_merge(d1[k], v)
+        elif v:
+            d1[k] = v
```

### Comparing `whoisit-2.7.4/whoisit.egg-info/PKG-INFO` & `whoisit-2.7.5/whoisit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisit
-Version: 2.7.4
+Version: 2.7.5
 Summary: A Python client to RDAP WHOIS-like services for internet resources.
 Home-page: https://github.com/meeb/whoisit
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: BSD
 Keywords: whoisit,whois,rdap,ip,network,cidr,prefix,domain,asn,autnum,tld,entity,handle,arin,afrinic,apnic,ripe,lacnic
 Classifier: Development Status :: 5 - Production/Stable
@@ -336,14 +336,15 @@
 ```
 
 ### Additional domain response data
 
 ```python
 # Domain response data includes all shared general response fields above and also:
 response = {
+    'unicode_name': str,     # Domain name in unicode if available
     'nameservers': list,     # List of name servers for the domain as strings
     'status': list,          # List of the domain states as strings
 }
 ```
 
 ### Additional IP response data
```

