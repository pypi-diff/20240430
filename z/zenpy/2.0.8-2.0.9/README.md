# Comparing `tmp/zenpy-2.0.8.tar.gz` & `tmp/zenpy-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zenpy-2.0.8.tar", last modified: Mon Jan 21 09:28:05 2019, max compression
+gzip compressed data, was "dist/zenpy-2.0.9.tar", last modified: Tue Mar 12 10:18:04 2019, max compression
```

## Comparing `zenpy-2.0.8.tar` & `zenpy-2.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 facetoe   (1000) facetoe   (1000)        0 2019-01-21 09:28:05.000000 zenpy-2.0.8/
--rwxr-xr-x   0 facetoe   (1000) facetoe   (1000)      899 2019-01-21 09:15:19.000000 zenpy-2.0.8/setup.py
-drwxr-xr-x   0 facetoe   (1000) facetoe   (1000)        0 2019-01-21 09:28:05.000000 zenpy-2.0.8/zenpy.egg-info/
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)      572 2019-01-21 09:28:05.000000 zenpy-2.0.8/zenpy.egg-info/SOURCES.txt
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)        6 2019-01-21 09:28:05.000000 zenpy-2.0.8/zenpy.egg-info/top_level.txt
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)      614 2019-01-21 09:28:05.000000 zenpy-2.0.8/zenpy.egg-info/PKG-INFO
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)       85 2019-01-21 09:28:05.000000 zenpy-2.0.8/zenpy.egg-info/requires.txt
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)        1 2019-01-21 09:28:05.000000 zenpy-2.0.8/zenpy.egg-info/dependency_links.txt
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)       79 2019-01-21 09:28:05.000000 zenpy-2.0.8/setup.cfg
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)      614 2019-01-21 09:28:05.000000 zenpy-2.0.8/PKG-INFO
-drwxr-xr-x   0 facetoe   (1000) facetoe   (1000)        0 2019-01-21 09:28:05.000000 zenpy-2.0.8/zenpy/
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)     9153 2019-01-21 09:14:56.000000 zenpy-2.0.8/zenpy/__init__.py
-drwxr-xr-x   0 facetoe   (1000) facetoe   (1000)        0 2019-01-21 09:28:05.000000 zenpy-2.0.8/zenpy/lib/
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)     9132 2018-07-17 11:56:56.000000 zenpy-2.0.8/zenpy/lib/generator.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)    31605 2019-01-21 09:14:56.000000 zenpy-2.0.8/zenpy/lib/endpoint.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)       23 2016-08-16 09:46:16.000000 zenpy-2.0.8/zenpy/lib/__init__.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)    71714 2019-01-21 09:14:56.000000 zenpy-2.0.8/zenpy/lib/api.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)     4106 2018-07-17 11:56:56.000000 zenpy-2.0.8/zenpy/lib/util.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)    15602 2018-07-08 02:41:27.000000 zenpy-2.0.8/zenpy/lib/response.py
-drwxr-xr-x   0 facetoe   (1000) facetoe   (1000)        0 2019-01-21 09:28:05.000000 zenpy-2.0.8/zenpy/lib/api_objects/
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)   180711 2019-01-21 09:14:56.000000 zenpy-2.0.8/zenpy/lib/api_objects/__init__.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)    33758 2019-01-21 09:14:56.000000 zenpy-2.0.8/zenpy/lib/api_objects/chat_objects.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)    49522 2019-01-21 09:14:56.000000 zenpy-2.0.8/zenpy/lib/api_objects/help_centre_objects.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)    14931 2019-01-21 09:14:56.000000 zenpy-2.0.8/zenpy/lib/api_objects/talk_objects.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)     5308 2018-04-29 04:41:21.000000 zenpy-2.0.8/zenpy/lib/proxy.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)     7153 2018-09-15 13:59:41.000000 zenpy-2.0.8/zenpy/lib/cache.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)     9067 2019-01-21 09:14:56.000000 zenpy-2.0.8/zenpy/lib/mapping.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)    19974 2018-09-15 13:59:41.000000 zenpy-2.0.8/zenpy/lib/request.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)      927 2017-09-08 07:15:59.000000 zenpy-2.0.8/zenpy/lib/exception.py
--rw-r--r--   0 facetoe   (1000) facetoe   (1000)     5160 2019-01-21 09:14:56.000000 zenpy-2.0.8/README.md
+drwxr-xr-x   0 facetoe   (1000) facetoe   (1000)        0 2019-03-12 10:18:04.000000 zenpy-2.0.9/
+-rwxr-xr-x   0 facetoe   (1000) facetoe   (1000)     1296 2019-03-12 10:13:46.000000 zenpy-2.0.9/setup.py
+drwxr-xr-x   0 facetoe   (1000) facetoe   (1000)        0 2019-03-12 10:18:04.000000 zenpy-2.0.9/zenpy.egg-info/
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)      572 2019-03-12 10:18:04.000000 zenpy-2.0.9/zenpy.egg-info/SOURCES.txt
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)        6 2019-03-12 10:18:04.000000 zenpy-2.0.9/zenpy.egg-info/top_level.txt
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)      965 2019-03-12 10:18:04.000000 zenpy-2.0.9/zenpy.egg-info/PKG-INFO
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)       86 2019-03-12 10:18:04.000000 zenpy-2.0.9/zenpy.egg-info/requires.txt
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)        1 2019-03-12 10:18:04.000000 zenpy-2.0.9/zenpy.egg-info/dependency_links.txt
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)       79 2019-03-12 10:18:04.000000 zenpy-2.0.9/setup.cfg
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)      965 2019-03-12 10:18:04.000000 zenpy-2.0.9/PKG-INFO
+drwxr-xr-x   0 facetoe   (1000) facetoe   (1000)        0 2019-03-12 10:18:04.000000 zenpy-2.0.9/zenpy/
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)     9446 2019-03-12 10:16:24.000000 zenpy-2.0.9/zenpy/__init__.py
+drwxr-xr-x   0 facetoe   (1000) facetoe   (1000)        0 2019-03-12 10:18:04.000000 zenpy-2.0.9/zenpy/lib/
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)     9132 2018-07-17 11:56:56.000000 zenpy-2.0.9/zenpy/lib/generator.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)    32014 2019-03-12 10:13:46.000000 zenpy-2.0.9/zenpy/lib/endpoint.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)       23 2016-08-16 09:46:16.000000 zenpy-2.0.9/zenpy/lib/__init__.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)    79052 2019-03-12 10:13:46.000000 zenpy-2.0.9/zenpy/lib/api.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)     4106 2018-07-17 11:56:56.000000 zenpy-2.0.9/zenpy/lib/util.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)    15602 2018-07-08 02:41:27.000000 zenpy-2.0.9/zenpy/lib/response.py
+drwxr-xr-x   0 facetoe   (1000) facetoe   (1000)        0 2019-03-12 10:18:04.000000 zenpy-2.0.9/zenpy/lib/api_objects/
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)   181250 2019-03-12 10:13:46.000000 zenpy-2.0.9/zenpy/lib/api_objects/__init__.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)    33758 2019-01-21 09:14:56.000000 zenpy-2.0.9/zenpy/lib/api_objects/chat_objects.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)    50899 2019-03-12 10:13:46.000000 zenpy-2.0.9/zenpy/lib/api_objects/help_centre_objects.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)    14931 2019-01-21 09:14:56.000000 zenpy-2.0.9/zenpy/lib/api_objects/talk_objects.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)     5308 2018-04-29 04:41:21.000000 zenpy-2.0.9/zenpy/lib/proxy.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)     7486 2019-03-12 10:13:46.000000 zenpy-2.0.9/zenpy/lib/cache.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)     9376 2019-03-12 10:13:46.000000 zenpy-2.0.9/zenpy/lib/mapping.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)    21553 2019-03-12 10:13:46.000000 zenpy-2.0.9/zenpy/lib/request.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)      990 2019-03-12 10:13:46.000000 zenpy-2.0.9/zenpy/lib/exception.py
+-rw-r--r--   0 facetoe   (1000) facetoe   (1000)     5160 2019-01-21 09:14:56.000000 zenpy-2.0.9/README.md
```

### Comparing `zenpy-2.0.8/setup.py` & `zenpy-2.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from setuptools import setup
 import setuptools
+from zenpy import __version__
 
 setup(
     name='zenpy',
     packages=setuptools.find_packages(),
-    version='2.0.8',
+    version=__version__,
     description='Python wrapper for the Zendesk API',
     license='GPLv3',
     author='Face Toe',
     author_email='facetoe@facetoe.com.au',
     url='https://github.com/facetoe/zenpy',
-    download_url='https://github.com/facetoe/zenpy/releases/tag/2.0.8',
+    download_url='https://github.com/facetoe/zenpy/releases/tag/{}'.format(__version__),
     install_requires=[
-        'requests>=2.7.0',
-        'python-dateutil>=2.4.0',
-        'cachetools>=1.0.3',
-        'pytz>=2017.3',
-        'future>=0.16.0'
+        'requests>=2.14.2',
+        'python-dateutil>=2.7.5',
+        'cachetools>=3.1.0',
+        'pytz>=2018.9',
+        'future>=0.17.1'
     ],
     keywords=['zendesk', 'api', 'wrapper'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
+        'Intended Audience :: Information Technology',
+        'Intended Audience :: System Administrators',
         'Programming Language :: Python :: 2',
+        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)'
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+        'Natural Language :: English',
     ],
 )
```

### Comparing `zenpy-2.0.8/zenpy.egg-info/SOURCES.txt` & `zenpy-2.0.9/zenpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zenpy-2.0.8/zenpy.egg-info/PKG-INFO` & `zenpy-2.0.9/zenpy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 1.1
 Name: zenpy
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python wrapper for the Zendesk API
 Home-page: https://github.com/facetoe/zenpy
 Author: Face Toe
 Author-email: facetoe@facetoe.com.au
 License: GPLv3
-Download-URL: https://github.com/facetoe/zenpy/releases/tag/2.0.8
+Download-URL: https://github.com/facetoe/zenpy/releases/tag/2.0.9
 Description: UNKNOWN
 Keywords: zendesk,api,wrapper
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
```

### Comparing `zenpy-2.0.8/PKG-INFO` & `zenpy-2.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 1.1
 Name: zenpy
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python wrapper for the Zendesk API
 Home-page: https://github.com/facetoe/zenpy
 Author: Face Toe
 Author-email: facetoe@facetoe.com.au
 License: GPLv3
-Download-URL: https://github.com/facetoe/zenpy/releases/tag/2.0.8
+Download-URL: https://github.com/facetoe/zenpy/releases/tag/2.0.9
 Description: UNKNOWN
 Keywords: zendesk,api,wrapper
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
```

### Comparing `zenpy-2.0.8/zenpy/__init__.py` & `zenpy-2.0.9/zenpy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3 import Retry
 
 from zenpy.lib.api import (
     UserApi,
     Api,
@@ -38,14 +37,15 @@
 from zenpy.lib.endpoint import EndpointFactory
 from zenpy.lib.exception import ZenpyException
 from zenpy.lib.mapping import ZendeskObjectMapping
 
 log = logging.getLogger()
 
 __author__ = 'facetoe'
+__version__ = '2.0.9'
 
 
 class Zenpy(object):
     """"""
 
     DEFAULT_TIMEOUT = 60.0
 
@@ -172,15 +172,15 @@
             elif token:
                 session.auth = ('%s/token' % email, token)
             elif oath_token:
                 session.headers.update({'Authorization': 'Bearer %s' % oath_token})
             else:
                 raise ZenpyException("Invalid arguments to _init_session()!")
 
-        headers = {'User-Agent': 'Zenpy/1.2'}
+        headers = {'User-Agent': 'Zenpy/{}'.format(__version__)}
         session.headers.update(headers)
         return session
 
     def get_cache_names(self):
         """
         Returns a list of current caches
         """
@@ -239,12 +239,24 @@
 
     def enable_caching(self):
         """
         Enable caching of objects.
         """
         self.cache.enable()
 
+    def caching_status(self):
+        """
+        Returns caching status.
+        """
+        self.cache.status()
+
+    def caching_engines(self):
+        """
+        Returns available caching engines.
+        """
+        self.cache.get_cache_engines()
+
     def _get_cache(self, cache_name):
         if cache_name not in self.cache.mapping:
             raise ZenpyException("No such cache - %s" % cache_name)
         else:
             return self.cache.mapping[cache_name]
```

### Comparing `zenpy-2.0.8/zenpy/lib/generator.py` & `zenpy-2.0.9/zenpy/lib/generator.py`

 * *Files identical despite different names*

### Comparing `zenpy-2.0.8/zenpy/lib/endpoint.py` & `zenpy-2.0.9/zenpy/lib/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,16 @@
             # this is a bit of a hack
             elif key == 'role':
                 if isinstance(value, basestring) or len(value) == 1:
                     parameters['role[]'] = value
                 else:
                     parameters['role[]'] = value[0] + '&' + "&".join(('role[]={}'.format(role) for role in value[1:]))
             elif key.endswith('ids'):
-                parameters[key] = ",".join(map(str, value)) #if it looks like a type of unknown id, send it through as such
+                # if it looks like a type of unknown id, send it through as such
+                parameters[key] = ",".join(map(str, value))
 
         if path == self.endpoint and not path.endswith('.json'):
             path += '.json'
         return Url(path=path, params=parameters)
 
 
 class SecondaryEndpoint(BaseEndpoint):
@@ -182,15 +183,16 @@
 class AttachmentEndpoint(BaseEndpoint):
     def __call__(self, **kwargs):
         return Url(self.endpoint, params={k: v for k, v in kwargs.items() if v is not None})
 
 
 class SearchEndpoint(BaseEndpoint):
     """
-    The search endpoint accepts all the parameters defined in the Zendesk `Search Documentation <https://developer.zendesk.com/rest_api/docs/core/search>`_.
+    The search endpoint accepts all the parameters defined in the Zendesk
+    `Search Documentation <https://developer.zendesk.com/rest_api/docs/core/search>`_.
     Zenpy defines several keywords that are mapped to the Zendesk comparison operators:
 
     +-----------------+------------------+
     | **Keyword**     | **Operator**     |
     +-----------------+------------------+
     | keyword         | : (equality)     |
     +-----------------+------------------+
@@ -248,15 +250,17 @@
                 if is_iterable_but_not_string(value):
                     [modifiers.append("-%s" % v) for v in value]
                 else:
                     modifiers.append("-%s" % value)
             elif is_iterable_but_not_string(value):
                 modifiers.append(self.format_or(key, value))
             else:
-                renamed_kwargs.update({key + ':': '"%s"' % value})
+                if isinstance(value, str) and value.count(' ') > 0:
+                    value = '"{}"'.format(value)
+                renamed_kwargs.update({key + ':': '%s' % value})
 
         search_query = ['%s%s' % (key, value) for (key, value) in renamed_kwargs.items()]
         search_query.extend(modifiers)
         if query is not None:
             search_query.insert(0, quote(query))
         params['query'] = ' '.join(search_query)
 
@@ -470,14 +474,15 @@
     ticket_forms = PrimaryEndpoint('ticket_forms')
     ticket_import = PrimaryEndpoint('imports/tickets')
     ticket_metrics = PrimaryEndpoint('ticket_metrics')
     tickets = PrimaryEndpoint('tickets')
     tickets.audits = SecondaryEndpoint('tickets/%(id)s/audits.json')
     tickets.audits.cursor = PrimaryEndpoint('ticket_audits')
     tickets.comments = SecondaryEndpoint('tickets/%(id)s/comments.json')
+    tickets.deleted = PrimaryEndpoint('deleted_tickets')
     tickets.events = IncrementalEndpoint('incremental/ticket_events.json')
     tickets.incremental = IncrementalEndpoint('incremental/tickets.json')
     tickets.metrics = SecondaryEndpoint('tickets/%(id)s/metrics.json')
     tickets.metrics.incremental = IncrementalEndpoint('incremental/ticket_metric_events.json')
     tickets.organizations = SecondaryEndpoint('organizations/%(id)s/tickets.json')
     tickets.recent = SecondaryEndpoint('tickets/recent.json')
     tickets.tags = SecondaryEndpoint('tickets/%(id)s/tags.json')
@@ -549,15 +554,15 @@
         'help_center/articles/%(id)s/translations/missing.json')
     help_centre.articles.update_translation = MultipleIDEndpoint('help_center/articles/{}/translations/{}.json')
     help_centre.articles.show_translation = MultipleIDEndpoint('help_center/articles/{}/translations/{}.json')
     help_centre.articles.delete_translation = SecondaryEndpoint('help_center/translations/%(id)s.json')
     help_centre.articles.search = HelpDeskSearchEndpoint('help_center/articles/search.json')
     help_centre.articles.subscriptions = SecondaryEndpoint('help_center/articles/%(id)s/subscriptions.json')
     help_centre.articles.subscriptions_delete = MultipleIDEndpoint('help_center/articles/{}/subscriptions/{}.json')
-    help_centre.articles.votes = SecondaryEndpoint('help_center//articles/%(id)s/votes.json')
+    help_centre.articles.votes = SecondaryEndpoint('help_center/articles/%(id)s/votes.json')
     help_centre.articles.votes.up = SecondaryEndpoint('help_center/articles/%(id)s/up.json')
     help_centre.articles.votes.down = SecondaryEndpoint('help_center/articles/%(id)s/down.json')
     help_centre.articles.comment_votes = MultipleIDEndpoint('help_center/articles/{}/comments/{}/votes.json')
     help_centre.articles.comment_votes.up = MultipleIDEndpoint('help_center/articles/{}/comments/{}/up.json')
     help_centre.articles.comment_votes.down = MultipleIDEndpoint('help_center/articles/{}/comments/{}/down.json')
 
     help_centre.labels = PrimaryEndpoint('help_center/articles/labels')
@@ -566,26 +571,28 @@
 
     help_centre.attachments = SecondaryEndpoint('help_center/articles/%(id)s/attachments.json')
     help_centre.attachments.inline = SecondaryEndpoint('help_center/articles/%(id)s/attachments/inline.json')
     help_centre.attachments.block = SecondaryEndpoint('help_center/articles/%(id)s/attachments/block.json')
     help_centre.attachments.create = SecondaryEndpoint('help_center/articles/%(id)s/attachments.json')
     help_centre.attachments.create_unassociated = PrimaryEndpoint('help_center/articles/attachments')
     help_centre.attachments.delete = SecondaryEndpoint('help_center/articles/attachments/%(id)s.json')
+    help_centre.attachments.bulk_attachments = SecondaryEndpoint('help_center/articles/%(id)s/bulk_attachments.json')
 
     help_centre.categories = PrimaryEndpoint('help_center/categories')
     help_centre.categories.articles = SecondaryEndpoint('help_center/categories/%(id)s/articles.json')
     help_centre.categories.sections = SecondaryEndpoint('help_center/categories/%(id)s/sections.json')
     help_centre.categories.translations = SecondaryEndpoint('help_center/categories/%(id)s/translations.json')
     help_centre.categories.create_translation = SecondaryEndpoint('help_center/categories/%(id)s/translations.json')
     help_centre.categories.missing_translations = SecondaryEndpoint(
         'help_center/categories/%(id)s/translations/missing.json')
     help_centre.categories.update_translation = MultipleIDEndpoint('help_center/categories/{}/translations/{}.json')
     help_centre.categories.delete_translation = SecondaryEndpoint('help_center/translations/%(id)s.json')
 
     help_centre.sections = PrimaryEndpoint('help_center/sections')
+    help_centre.sections.create = SecondaryEndpoint('help_center/categories/%(id)s/sections.json')
     help_centre.sections.articles = SecondaryEndpoint('help_center/sections/%(id)s/articles.json')
     help_centre.sections.translations = SecondaryEndpoint('help_center/sections/%(id)s/translations.json')
     help_centre.sections.create_translation = SecondaryEndpoint('help_center/sections/%(id)s/translations.json')
     help_centre.sections.missing_translations = SecondaryEndpoint(
         'help_center/sections/%(id)s/translations/missing.json')
     help_centre.sections.update_translation = MultipleIDEndpoint('help_center/sections/{}/translations/{}.json')
     help_centre.sections.delete_translation = SecondaryEndpoint('help_center/translations/%(id)s.json')
```

### Comparing `zenpy-2.0.8/zenpy/lib/api.py` & `zenpy-2.0.9/zenpy/lib/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         else:
             response = http_method(url, **kwargs)
 
         # If we are being rate-limited, wait the required period before trying again.
         if response.status_code == 429:
             while 'retry-after' in response.headers and int(response.headers['retry-after']) > 0:
                 retry_after_seconds = int(response.headers['retry-after'])
-                log.warn(
+                log.warning(
                     "Waiting for requested retry-after period: %s seconds" % retry_after_seconds
                 )
                 while retry_after_seconds > 0:
                     retry_after_seconds -= 1
                     self.check_ratelimit_budget(1)
                     log.debug("    -> sleeping: %s more seconds" % retry_after_seconds)
                     sleep(1)
@@ -169,15 +169,15 @@
         lastlimitremaining = self.callsafety['lastlimitremaining']
 
         if time_since_last_call() is None or time_since_last_call() >= self.ratelimit_request_interval or \
                 lastlimitremaining >= self.ratelimit:
             response = http_method(url, **kwargs)
         else:
             # We hit our limit floor and aren't quite at ratelimit_request_interval value in seconds yet..
-            log.warn(
+            log.warning(
                 "Safety Limit Reached of %s remaining calls and time since last call is under %s seconds"
                 % (self.ratelimit, self.ratelimit_request_interval)
             )
             while time_since_last_call() < self.ratelimit_request_interval:
                 remaining_sleep = int(self.ratelimit_request_interval - time_since_last_call())
                 log.debug("  -> sleeping: %s more seconds" % remaining_sleep)
                 self.check_ratelimit_budget(1)
@@ -269,14 +269,15 @@
             return cached_objects
         else:
             return self._get(self._build_url(endpoint=endpoint(*endpoint_args, **endpoint_kwargs)))
 
     def _check_response(self, response):
         """
         Check the response code returned by Zendesk. If it is outside the 200 range, raise an exception of the correct type.
+
         :param response: requests Response object.
         """
         if response.status_code > 299 or response.status_code < 200:
             log.debug("Received response code [%s] - headers: %s" % (response.status_code, str(response.headers)))
             try:
                 _json = response.json()
                 err_type = _json.get("error", '')
@@ -511,24 +512,24 @@
         """
         return TagRequest(self).put(tags, id)
 
     def set_tags(self, id, tags):
         """
         Set (POST) one or more tags.
 
-        :param _id: the id of the object to tag
+        :param id: the id of the object to tag
         :param tags: array of tags to apply to object
         """
         return TagRequest(self).post(tags, id)
 
     def delete_tags(self, id, tags):
         """
         Delete (DELETE) one or more tags.
 
-        :param _id: the id of the object to delete tag from
+        :param id: the id of the object to delete tag from
         :param tags: array of tags to delete from object
         """
         return TagRequest(self).delete(tags, id)
 
     def tags(self, ticket_id):
         """
         Lists the most popular recent tags in decreasing popularity from a specific ticket.
@@ -556,15 +557,17 @@
     """
     IncrementalApi supports the incremental endpoint.
     """
 
     def incremental(self, start_time, include=None):
         """
         Retrieve bulk data from the incremental API.
-        :param include: list of objects to sideload
+
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param start_time: The time of the oldest object you are interested in.
         """
         return self._query_zendesk(self.endpoint.incremental, self.object_type, start_time=start_time, include=include)
 
 
 class UserIdentityApi(Api):
     def __init__(self, config):
@@ -660,65 +663,71 @@
         self.identities = UserIdentityApi(config)
 
     @extract_id(User)
     def groups(self, user, include=None):
         """
         Retrieve the groups for this user.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param user: User object or id
         """
         return self._query_zendesk(self.endpoint.groups, 'group', id=user, include=include)
 
     @extract_id(User)
     def organizations(self, user, include=None):
         """
         Retrieve the organizations for this user.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param user: User object or id
         """
         return self._query_zendesk(self.endpoint.organizations, 'organization', id=user, include=include)
 
     @extract_id(User)
     def requested(self, user, include=None):
         """
         Retrieve the requested tickets for this user.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param user: User object or id
         """
         return self._query_zendesk(self.endpoint.requested, 'ticket', id=user, include=include)
 
     @extract_id(User)
     def cced(self, user, include=None):
         """
         Retrieve the tickets this user is cc'd into.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param user: User object or id
         """
         return self._query_zendesk(self.endpoint.cced, 'ticket', id=user, include=include)
 
     @extract_id(User)
     def assigned(self, user, include=None):
         """
         Retrieve the assigned tickets for this user.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param user: User object or id
         """
         return self._query_zendesk(self.endpoint.assigned, 'ticket', id=user, include=include)
 
     @extract_id(User)
     def group_memberships(self, user, include=None):
         """
         Retrieve the group memberships for this user.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param user: User object or id
         """
         return self._query_zendesk(self.endpoint.group_memberships, 'group_membership', id=user, include=include)
 
     def requests(self, **kwargs):
         return self._query_zendesk(self.endpoint.requests, 'request', **kwargs)
 
@@ -732,15 +741,16 @@
         """
         return self._query_zendesk(self.endpoint.related, 'user_related', id=user)
 
     def me(self, include=None):
         """
         Return the logged in user
 
-        :param include: abilities - https://developer.zendesk.com/rest_api/docs/core/side_loading#abilities
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading#abilities>`__.
         """
         return self._query_zendesk(self.endpoint.me, 'user', include=include)
 
     @extract_id(User)
     def merge(self, source_user, dest_user):
         """
         Merge the user provided in source_user into dest_user
@@ -779,43 +789,51 @@
         """
 
         return CRUDRequest(self).post(users, create_or_update=True)
 
     @extract_id(User)
     def permanently_delete(self, user):
         """
-        Permanently delete user - https://developer.zendesk.com/rest_api/docs/core/users#permanently-delete-user
+        Permanently delete user. User should be softly deleted first.
+        Zendesk API `Reference <https://developer.zendesk.com/rest_api/docs/core/users#permanently-delete-user>`__.
 
-        :param user: User object or id
+        Note: This endpoint does not support multiple ids or list of `User` objects.
+
+        :param user: User object or id.
+        :return: User object with `permanently_deleted` status
         """
         url = self._build_url(self.endpoint.deleted(id=user))
         deleted_user = self._delete(url)
         self.cache.delete(deleted_user)
         return deleted_user
 
     def deleted(self):
         """
         List Deleted Users.
 
         These are users that have been deleted but not permanently yet.
-        See Permanently delete user - https://developer.zendesk.com/rest_api/docs/core/users#permanently-delete-user
+        Zendesk API `Reference <https://developer.zendesk.com/rest_api/docs/core/users#permanently-delete-user>`__.
+
+        :return:
         """
         return self._get(self._build_url(self.endpoint.deleted()))
 
     @extract_id(User)
     def skips(self, user):
         """
-        Skips for user (https://developer.zendesk.com/rest_api/docs/core/ticket_skips)
+        Skips for user. Zendesk API `Reference <https://developer.zendesk.com/rest_api/docs/core/ticket_skips>`__.
         """
         return self._get(self._build_url(self.endpoint.skips(id=user)))
 
     @extract_id(User)
     def set_password(self, user, password):
         """
-        Sets the password for the passed user - https://developer.zendesk.com/rest_api/docs/support/users#set-a-users-password
+        Sets the password for the passed user.
+        Zendesk API `Reference <https://developer.zendesk.com/rest_api/docs/support/users#set-a-users-password>`__.
+
         :param user: User object or id
         :param password: new password
         """
         url = self._build_url(self.endpoint.set_password(id=user))
         return self._post(url, payload=dict(password=password))
 
 
@@ -831,28 +849,27 @@
     def upload(self, fp, token=None, target_name=None, content_type=None):
         """
         Upload a file to Zendesk.
 
         :param fp: file object, StringIO instance, content, or file path to be
                    uploaded
         :param token: upload token for uploading multiple files
-        :param target_name: name of the file inside¡ Zendesk
-        :return: :class:`Upload` object containing a token and other information
-                    (see https://developer.zendesk.com/rest_api/docs/core/attachments#uploading-files)
+        :param target_name: name of the file inside Zendesk
+        :return: :class:`Upload` object containing a token and other information see
+            Zendesk API `Reference <https://developer.zendesk.com/rest_api/docs/core/attachments#uploading-files>`__.
         """
         return UploadRequest(self).post(fp, token=token, target_name=target_name, content_type=content_type)
 
     def download(self, attachment_id, destination):
         """
         Download an attachment from Zendesk.
 
-
         :param attachment_id: id of the attachment to download
         :param destination: destination path. If a directory, the file will be placed in the directory with
-                            the filename from the Atttachment object.
+                            the filename from the Attachment object.
         :return: the path the file was written to
         """
         attachment = self(id=attachment_id)
         if os.path.isdir(destination):
             destination = os.path.join(destination, attachment.file_name)
         return self._download_file(attachment.content_url, destination)
 
@@ -914,15 +931,16 @@
         """
         return self._query_zendesk(self.endpoint.organization_memberships, 'organization_membership', id=organization)
 
     def external(self, external_id, include=None):
         """
         Locate an Organization by it's external_id attribute.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param external_id: external id of organization
         """
         return self._query_zendesk(self.endpoint.external, 'organization', id=external_id, include=include)
 
     def requests(self, **kwargs):
         return self._query_zendesk(self.endpoint.requests, 'request', **kwargs)
 
@@ -954,14 +972,15 @@
     def __init__(self, config):
         super(OrganizationFieldsApi, self).__init__(config, object_type='organization_field')
 
     @extract_id(OrganizationField)
     def reorder(self, organization_fields):
         """
         Reorder organization fields.
+
         :param organization_fields: list of OrganizationField objects or ids in the desired order.
         """
         return OrganizationFieldReorderRequest(self).put(organization_fields)
 
 
 class SatisfactionRatingApi(Api):
     def __init__(self, config):
@@ -981,15 +1000,16 @@
 class MacroApi(CRUDApi):
     def __init__(self, config):
         super(MacroApi, self).__init__(config, object_type='macro')
 
     @extract_id(Macro)
     def apply(self, macro):
         """
-        Show what a macro would do - https://developer.zendesk.com/rest_api/docs/core/macros#show-changes-to-ticket
+        Show what a macro would do
+        Zendesk API `Reference <https://developer.zendesk.com/rest_api/docs/core/macros#show-changes-to-ticket>`__.
 
         :param macro: Macro object or id.
         """
 
         return self._query_zendesk(self.endpoint.apply, 'result', id=macro)
 
 
@@ -1002,15 +1022,16 @@
         super(TicketApi, self).__init__(config, object_type='ticket')
 
     @extract_id(Organization)
     def organizations(self, organization, include=None):
         """
         Retrieve the tickets for this organization.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param organization: Organization object or id
         """
         return self._query_zendesk(self.endpoint.organizations, 'ticket', id=organization, include=include)
 
     def recent(self, include=None):
         """
         Retrieve the most recent tickets
@@ -1022,19 +1043,50 @@
         """
         Retrieve the comments for a ticket.
 
         :param ticket: Ticket object or id
         """
         return self._query_zendesk(self.endpoint.comments, 'comment', id=ticket)
 
+    def permanently_delete(self, tickets):
+        """
+        Permanently delete ticket. `See Zendesk API docs <https://developer.zendesk.com/rest_api/docs/support/tickets#delete-ticket-permanently>`_
+
+        Ticket should be softly deleted first with regular `delete` method.
+
+        :param tickets: Ticket object or list of tickets objects
+        :return: JobStatus object
+        """
+        endpoint_kwargs = dict()
+        if isinstance(tickets, collections.Iterable):
+            endpoint_kwargs['destroy_ids'] = [i.id for i in tickets]
+        else:
+            endpoint_kwargs['id'] = tickets.id
+        url = self._build_url(self.endpoint.deleted(**endpoint_kwargs))
+        deleted_ticket_job_id = self._delete(url)
+        self.cache.delete(tickets)
+        return deleted_ticket_job_id
+
+    def deleted(self):
+        """
+        List Deleted Tickets.
+
+        These are tickets that have been deleted but not permanently yet.
+        See Permanently delete ticket in `Zendesk API docs <https://developer.zendesk.com/rest_api/docs/support/tickets#delete-ticket-permanently>`_
+
+        :return: ResultGenerator with Tickets objects with length 0 of no deleted tickets exist.
+        """
+        return self._get(self._build_url(self.endpoint.deleted()))
+
     def events(self, start_time, include=None):
         """
         Retrieve TicketEvents
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param start_time: time to retrieve events from.
         """
         return self._query_zendesk(self.endpoint.events, 'ticket_event', start_time=start_time, include=include)
 
     @extract_id(Ticket)
     def audits(self, ticket=None, include=None, **kwargs):
         """
@@ -1047,35 +1099,39 @@
         For example:
 
         .. code-block:: python
 
             for audit in reversed(zenpy_client.tickets.audits()):
                 print(audit)
 
-        See the Zendesk docs for information on additional parameters - https://developer.zendesk.com/rest_api/docs/core/ticket_audits#pagination
+        See the `Zendesk docs <https://developer.zendesk.com/rest_api/docs/core/ticket_audits#pagination>`__ for
+        information on additional parameters.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param ticket: Ticket object or id
         """
         if ticket is not None:
             return self._query_zendesk(self.endpoint.audits, 'ticket_audit', id=ticket, include=include)
         else:
             return self._query_zendesk(self.endpoint.audits.cursor, 'ticket_audit', include=include, **kwargs)
 
     @extract_id(Ticket)
     def metrics(self, ticket):
         """
         Retrieve TicketMetric.
+
         :param ticket: Ticket object or id
         """
         return self._query_zendesk(self.endpoint.metrics, 'ticket_metric', id=ticket)
 
     def metrics_incremental(self, start_time):
         """
         Retrieve TicketMetric incremental
+
         :param start_time: time to retrieve events from.
         """
         return self._query_zendesk(self.endpoint.metrics.incremental, 'ticket_metric_events', start_time=start_time)
 
     @extract_id(Ticket, Macro)
     def show_macro_effect(self, ticket, macro):
         """
@@ -1106,15 +1162,15 @@
         return TicketMergeRequest(self).post(target, source,
                                              target_comment=target_comment,
                                              source_comment=source_comment)
 
     @extract_id(Ticket)
     def skips(self, ticket):
         """
-        Skips for ticket (https://developer.zendesk.com/rest_api/docs/core/ticket_skips)
+        Skips for ticket See Zendesk API `Reference <https://developer.zendesk.com/rest_api/docs/core/ticket_skips>`__.
         """
 
         return self._get(self._build_url(self.endpoint.skips(id=ticket)))
 
 
 class SkipApi(CRUDApi):
     def __init__(self, config):
@@ -1162,15 +1218,16 @@
         """
         return self._query_zendesk(self.endpoint.show, 'custom_field_option', ticket_field, custom_field_option)
 
     @extract_id(TicketField)
     def create_or_update(self, ticket_field, custom_field_option):
         """
         Create or update a CustomFieldOption for a TicketField. If passed CustomFieldOption has no id, a new option
-        will be created, otherwise it is updated - https://developer.zendesk.com/rest_api/docs/core/ticket_fields#create-or-update-a-ticket-field-option.
+        will be created, otherwise it is updated - See: Zendesk API `Reference
+        <https://developer.zendesk.com/rest_api/docs/core/ticket_fields#create-or-update-a-ticket-field-option>`__.
 
         :param ticket_field: TicketField object or id
         :param custom_field_option: CustomFieldOption object
         """
         return TicketFieldOptionRequest(self).post(ticket_field, custom_field_option)
 
     @extract_id(TicketField, CustomFieldOption)
@@ -1297,16 +1354,17 @@
         return self._query_zendesk(self.endpoint.comments, 'comment', id=request_id)
 
     def delete(self, api_objects, **kwargs):
         raise ZenpyException("You cannot delete requests!")
 
     def search(self, *args, **kwargs):
         """
-        Search for requests. See the Zendesk docs for more information on the syntax
-         https://developer.zendesk.com/rest_api/docs/core/requests#searching-requests
+        Search for requests. See the `Zendesk docs
+        <https://developer.zendesk.com/rest_api/docs/core/requests#searching-requests>`__ for more information on the
+        syntax.
         """
         return self._query_zendesk(self.endpoint.search, 'request', *args, **kwargs)
 
 
 class SharingAgreementAPI(CRUDApi):
     def __init__(self, config):
         super(SharingAgreementAPI, self).__init__(config, object_type='sharing_agreement')
@@ -1319,27 +1377,29 @@
     @extract_id(Group)
     def users(self, group, include=None):
         return self._get(self._build_url(self.endpoint.users(id=group, include=include)))
 
     @extract_id(Group)
     def memberships(self, group, include=None):
         """
-        Return the GroupMemberships for this group
+        Return the GroupMemberships for this group.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param group: Group object or id
         """
         return self._get(self._build_url(self.endpoint.memberships(id=group, include=include)))
 
     @extract_id(Group)
     def memberships_assignable(self, group, include=None):
         """
         Return memberships that are assignable for this group.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param group: Group object or id
         """
         return self._get(self._build_url(self.endpoint.memberships_assignable(id=group, include=include)))
 
 
 class ViewApi(CRUDApi):
     def __init__(self, config):
@@ -1349,72 +1409,78 @@
         """
         Return all active views.
         """
         return self._get(self._build_url(self.endpoint.active(include=include)))
 
     def compact(self, include=None):
         """
-        Return compact views - https://developer.zendesk.com/rest_api/docs/core/views#list-views---compact
+        Return compact views - See: Zendesk API `Reference
+        <https://developer.zendesk.com/rest_api/docs/core/views#list-views---compact>`__
         """
         return self._get(self._build_url(self.endpoint.compact(include=include)))
 
     @extract_id(View)
     def execute(self, view, include=None):
         """
         Execute a view.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param view: View or view id
         """
         return self._get(self._build_url(self.endpoint.execute(id=view, include=include)))
 
     @extract_id(View)
     def tickets(self, view, include=None):
         """
         Return the tickets in a view.
 
-        :param include: Optionally include more data. See https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param view: View or view id
         """
         return self._get(self._build_url(self.endpoint.tickets(id=view, include=include)))
 
     @extract_id(View)
     def count(self, view, include=None):
         """
         Return a ViewCount for a view.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param view: View or view id
         """
         return self._get(self._build_url(self.endpoint.count(id=view, include=include)))
 
     @extract_id(View)
     def count_many(self, views, include=None):
         """
         Return many ViewCounts.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+            <https://developer.zendesk.com/rest_api/docs/core/side_loading>`__.
         :param views: iterable of View or view ids
         """
         return self._get(self._build_url(self.endpoint(count_many=views, include=include)))
 
     @extract_id(View)
     def export(self, view, include=None):
         """
         Export a view. Returns an Export object.
 
-        :param include: https://developer.zendesk.com/rest_api/docs/core/side_loading
+        :param include: list of objects to sideload. `Side-loading API Docs 
+
         :param view: View or view id
         :return:
         """
         return self._get(self._build_url(self.endpoint.export(id=view, include=include)))
 
     def search(self, *args, **kwargs):
         """
-        Search views. See - https://developer.zendesk.com/rest_api/docs/core/views#search-views.
+        Search views. See Zendesk API `Reference <https://developer.zendesk.com/rest_api/docs/core/views#search-views>`__.
 
         :param args: query is the only accepted arg.
         :param kwargs: search parameters
         """
         return self._get(self._build_url(self.endpoint.search(*args, **kwargs)))
 
     # TODO: https://github.com/facetoe/zenpy/issues/123
@@ -1555,15 +1621,15 @@
         super(HelpCentreApiBase, self).__init__(config, object_type=object_type, endpoint=endpoint)
 
         self._response_handlers = (MissingTranslationHandler,) + self._response_handlers
 
         self._object_mapping = HelpCentreObjectMapping(self)
         self.locale = ''
 
-    def _process_response(self, response):
+    def _process_response(self, response, object_mapping=None):
         endpoint_path = get_endpoint_path(self, response)
         if endpoint_path.startswith('/help_center') or endpoint_path.startswith('/community'):
             object_mapping = self._object_mapping
         else:
             object_mapping = ZendeskObjectMapping(self)
         return super(HelpCentreApiBase, self)._process_response(response, object_mapping)
 
@@ -1641,32 +1707,35 @@
         return self._post(url, payload={})
 
 
 class ArticleApi(HelpCentreApiBase, TranslationApi, SubscriptionApi, VoteApi, VoteCommentApi):
     @extract_id(Section)
     def create(self, section, article):
         """
-        Create (POST) an Article - https://developer.zendesk.com/rest_api/docs/help_center/articles#create-article
+        Create (POST) an Article - See: Zendesk API `Reference
+        <https://developer.zendesk.com/rest_api/docs/help_center/articles#create-article>`__.
 
         :param section: Section ID or object
         :param article: Article to create
         """
         return CRUDRequest(self).post(article, create=True, id=section)
 
     def update(self, article):
         """
-        Update (PUT) and Article - https://developer.zendesk.com/rest_api/docs/help_center/articles#update-article
+        Update (PUT) and Article - See: Zendesk API `Reference
+        <https://developer.zendesk.com/rest_api/docs/help_center/articles#update-article>`__.
 
         :param article: Article to update
         """
         return CRUDRequest(self).put(article)
 
     def archive(self, article):
         """
-        Archive (DELETE) an Article - https://developer.zendesk.com/rest_api/docs/help_center/articles#archive-article
+        Archive (DELETE) an Article - See: Zendesk API `Reference
+        <https://developer.zendesk.com/rest_api/docs/help_center/articles#archive-article>`__.
 
         :param article: Article to archive
         """
         return CRUDRequest(self).delete(article)
 
     @extract_id(Article)
     def comments(self, article):
@@ -1741,48 +1810,125 @@
 
 
 class SectionApi(HelpCentreApiBase, CRUDApi, TranslationApi, SubscriptionApi, AccessPolicyApi):
     @extract_id(Section)
     def articles(self, section):
         return self._query_zendesk(self.endpoint.articles, 'article', id=section)
 
+    def create(self, section):
+        return CRUDRequest(self).post(section, create=True, id=section.category_id)
+
 
 class ArticleAttachmentApi(HelpCentreApiBase, SubscriptionApi):
     @extract_id(Article)
     def __call__(self, article):
+        """
+        Returns all attachments associated with article_id either ``inline=True`` or ``inline=False``.
+
+        :param article: Numeric article id or :class:`Article` object.
+        :return: Generator with all associated articles attachments.
+        """
         return self._query_zendesk(self.endpoint, 'article_attachment', id=article)
 
     @extract_id(Article)
     def inline(self, article):
+        """
+        Returns all inline attachments associated with article_id where (Such attachments has ``inline=True`` flag).
+
+        Inline attachments and its url can be referenced in the HTML body of the article.
+
+        :param article: Numeric article id or :class:`Article` object.
+        :return: Generator with all associated inline attachments.
+        """
         return self._query_zendesk(self.endpoint.inline, 'article_attachment', id=article)
 
     @extract_id(Article)
     def block(self, article):
+        """
+        Returns all block attachments associated with article_id (Such attachments has ``inline=False``).
+
+        Block attachments are displayed as separated files attached to Article.
+
+        :param article: Numeric article id or :class:`Article` object.
+        :return: Generator with all associated block attachments.
+        """
         return self._query_zendesk(self.endpoint.block, 'article_attachment', id=article)
 
     @extract_id(ArticleAttachment)
     def show(self, attachment):
         return self._query_zendesk(self.endpoint, 'article_attachment', id=attachment)
 
     @extract_id(Article)
-    def create(self, article, attachment, inline=False):
+    def create(self, article, attachment, inline=False, file_name=None, content_type=None):
+        """
+        This function creates attachment attached to article.
+
+        :param article: Numeric article id or :class:`Article` object.
+        :param attachment: File object or os path to file
+        :param inline: If true, the attached file is shown in the dedicated admin UI
+            for inline attachments and its url can be referenced in the HTML body of
+            the article. If false, the attachment is listed in the list of attachments.
+            Default is `false`
+        :param file_name: you can set filename on file upload.
+        :param content_type: The content type of the file. `Example: image/png`, Zendesk can ignore it.
+        :return: :class:`ArticleAttachment` object
+        """
         return HelpdeskAttachmentRequest(self).post(self.endpoint.create,
                                                     article=article,
-                                                    attachment=attachment,
-                                                    inline=inline)
-
-    def create_unassociated(self, attachment, inline=False):
+                                                    attachments=attachment,
+                                                    inline=inline,
+                                                    file_name=file_name,
+                                                    content_type=content_type)
+
+    def create_unassociated(self, attachment, inline=False, file_name=None, content_type=None):
+        """
+        You can use this endpoint for bulk imports.
+        It lets you upload a file without associating it to an article until later.
+        Check Zendesk documentation `important notes
+        <https://developer.zendesk.com/rest_api/docs/help_center/article_attachments#create-unassociated-attachment>
+
+        :param attachment: File object or os path to file
+        :param inline: If true, the attached file is shown in the dedicated admin UI
+            for inline attachments and its url can be referenced in the HTML body of
+            the article. If false, the attachment is listed in the list of attachments.
+            Default is `false`
+        :param file_name: you can set filename on file upload.
+        :param content_type: The content type of the file. `Example: image/png`, Zendesk can ignore it.
+        :return: :class:`ArticleAttachment` object
+        """
         return HelpdeskAttachmentRequest(self).post(self.endpoint.create_unassociated,
-                                                    attachment=attachment,
-                                                    inline=inline)
+                                                    attachments=attachment,
+                                                    inline=inline,
+                                                    file_name=file_name,
+                                                    content_type=content_type)
 
     @extract_id(ArticleAttachment)
     def delete(self, article_attachment):
+        """
+        This function completely wipes attachment from Zendesk Helpdesk article.
+
+        :param article_attachment: :class:`ArticleAttachment` object or numeric article attachment id.
+        :return: status_code == 204 on success
+        """
         return HelpdeskAttachmentRequest(self).delete(self.endpoint.delete, article_attachment)
 
+    @extract_id(Article)
+    def bulk_attachments(self, article, attachments):
+        """
+        This function implements associating attachments to an article after article creation (for
+        unassociated attachments).
+
+        :param article: Article id or :class:`Article` object
+        :param attachments: :class:`ArticleAttachment` object, or list of :class:`ArticleAttachment` objects,
+        up to 20 supported. `Zendesk documentation.
+        <https://developer.zendesk.com/rest_api/docs/help_center/articles#associate-attachments-in-bulk-to-article>`__
+        :return:
+        """
+        return HelpdeskAttachmentRequest(self).post(self.endpoint.bulk_attachments, article=article,
+                                                    attachments=attachments)
 
 class LabelApi(HelpCentreApiBase):
     @extract_id(Article)
     def create(self, article, label):
         return HelpCentreRequest(self).post(self.endpoint.create, article, label)
 
     @extract_id(Article, Label)
@@ -1858,21 +2004,23 @@
 
     def __call__(self, *args, **kwargs):
         raise ZenpyException("You cannot call this endpoint directly!")
 
     def recipients_incremental(self, start_time):
         """
         Retrieve NPS Recipients incremental
+
         :param start_time: time to retrieve events from.
         """
         return self._query_zendesk(self.endpoint.recipients_incremental, 'recipients', start_time=start_time)
 
     def responses_incremental(self, start_time):
         """
         Retrieve NPS Responses incremental
+
         :param start_time: time to retrieve events from.
         """
         return self._query_zendesk(self.endpoint.responses_incremental, 'responses', start_time=start_time)
 
 class TalkApiBase(Api):
     def __init__(self, config, endpoint, object_type):
         super(TalkApiBase, self).__init__(config, object_type=object_type, endpoint=endpoint)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `zenpy-2.0.8/zenpy/lib/util.py` & `zenpy-2.0.9/zenpy/lib/util.py`

 * *Files identical despite different names*

### Comparing `zenpy-2.0.8/zenpy/lib/response.py` & `zenpy-2.0.9/zenpy/lib/response.py`

 * *Files identical despite different names*

### Comparing `zenpy-2.0.8/zenpy/lib/api_objects/__init__.py` & `zenpy-2.0.9/zenpy/lib/api_objects/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 ######################################################################
 #  Do not modify, these classes are autogenerated by gen_classes.py  #
 ######################################################################
 
 import json
 import dateutil.parser
-from zenpy.lib.util import json_encode_for_printing
+from zenpy.lib.util import json_encode_for_printing, json_encode_for_zendesk
 
 
 class BaseObject(object):
     """
     Base for all Zenpy objects. Keeps track of which attributes have been modified.
     """
 
@@ -51,14 +51,27 @@
 
     def to_json(self, indent=2):
         """ Return self formatted as JSON. """
         return json.dumps(self, default=json_encode_for_printing, indent=indent)
 
     def to_dict(self, serialize=False):
         """
+        This method returns the object as a Python dict. If serialize is passed, only those attributes
+        that have been modified will be included in the result.
+        :param serialize:
+        :return:
+        """
+        if serialize:
+            encode_method = json_encode_for_zendesk
+        else:
+            encode_method = json_encode_for_printing
+        return json.loads(json.dumps(self._to_dict(serialize=serialize), default=encode_method))
+
+    def _to_dict(self, serialize=False):
+        """
         This method works by copying self.__dict__, and removing everything that should not be serialized.
         """
         copy_dict = self.__dict__.copy()
         for key, value in vars(self).items():
             # We want to send all ids to Zendesk always
             if serialize and key == 'id':
                 continue
```

### Comparing `zenpy-2.0.8/zenpy/lib/api_objects/chat_objects.py` & `zenpy-2.0.9/zenpy/lib/api_objects/chat_objects.py`

 * *Files identical despite different names*

### Comparing `zenpy-2.0.8/zenpy/lib/api_objects/help_centre_objects.py` & `zenpy-2.0.9/zenpy/lib/api_objects/help_centre_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,18 +292,24 @@
     """
 
     def __init__(self,
                  api=None,
                  article_id=None,
                  content_type=None,
                  content_url=None,
+                 created_at=None,
+                 display_file_name=None,
                  file_name=None,
                  id=None,
                  inline=None,
+                 legacy=None,
+                 relative_path=None,
                  size=None,
+                 updated_at=None,
+                 url=None,
                  **kwargs):
 
         self.api = api
 
         # Comment: Id of the associated article, if present
         # Type: integer
         self.article_id = article_id
@@ -312,30 +318,45 @@
         # Type: string
         self.content_type = content_type
 
         # Comment: A full URL where the attachment file can be downloaded
         # Type: string
         self.content_url = content_url
 
+        # Comment: The time at which the article attachment was created
+        # Type: timestamp
+        self.created_at = created_at
+        self.display_file_name = display_file_name
+
         # Comment: The name of the file
         # Type: string
         self.file_name = file_name
 
         # Comment: Automatically assigned when the article attachment is created
         # Type: integer
         self.id = id
 
         # Comment: If true, the attached file is shown in the dedicated admin UI for inline attachments and its url can be referenced in the HTML body of the article. If false, the attachment is listed in the list of attachments. Default is false
         # Type: boolean
         self.inline = inline
+        self.legacy = legacy
+        self.relative_path = relative_path
 
         # Comment: The size of the attachment file in bytes
         # Type: integer
         self.size = size
 
+        # Comment: The time at which the article attachment was last updated
+        # Type: timestamp
+        self.updated_at = updated_at
+
+        # Comment: The API url of this article attachment
+        # Type: string
+        self.url = url
+
         for key, value in kwargs.items():
             setattr(self, key, value)
 
         for key in self.to_dict():
             if getattr(self, key) is None:
                 try:
                     self._dirty_attributes.remove(key)
@@ -352,14 +373,40 @@
 
     @article.setter
     def article(self, article):
         if article:
             self.article_id = article.id
             self._article = article
 
+    @property
+    def created(self):
+        """
+        |  Comment: The time at which the article attachment was created
+        """
+        if self.created_at:
+            return dateutil.parser.parse(self.created_at)
+
+    @created.setter
+    def created(self, created):
+        if created:
+            self.created_at = created
+
+    @property
+    def updated(self):
+        """
+        |  Comment: The time at which the article attachment was last updated
+        """
+        if self.updated_at:
+            return dateutil.parser.parse(self.updated_at)
+
+    @updated.setter
+    def updated(self, updated):
+        if updated:
+            self.updated_at = updated
+
 
 class Category(BaseObject):
     """
     ######################################################################
     #    Do not modify, this class is autogenerated by gen_classes.py    #
     ######################################################################
     """
```

### Comparing `zenpy-2.0.8/zenpy/lib/api_objects/talk_objects.py` & `zenpy-2.0.9/zenpy/lib/api_objects/talk_objects.py`

 * *Files identical despite different names*

### Comparing `zenpy-2.0.8/zenpy/lib/proxy.py` & `zenpy-2.0.9/zenpy/lib/proxy.py`

 * *Files identical despite different names*

### Comparing `zenpy-2.0.8/zenpy/lib/cache.py` & `zenpy-2.0.9/zenpy/lib/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 
 
 class ZenpyCache(object):
     """
     Wrapper class for the various cachetools caches. Adds ability to change cache implementations
     on the fly and change the maxsize setting.
     """
+
     AVAILABLE_CACHES = [c for c in dir(cachetools) if c.endswith('Cache') and c != 'Cache']
 
     def __init__(self, cache_impl, maxsize, **kwargs):
         self.cache = self._get_cache_impl(cache_impl, maxsize, **kwargs)
         self.purge_lock = RLock()
 
     def set_cache_impl(self, cache_impl, maxsize, **kwargs):
         """
         Change cache implementation. The contents of the old cache will
         be transferred to the new one.
+
         :param cache_impl: Name of cache implementation, must exist in AVAILABLE_CACHES
         """
         new_cache = self._get_cache_impl(cache_impl, maxsize, **kwargs)
         self._populate_new_cache(new_cache)
         self.cache = new_cache
 
     def pop(self, key, default=None):
@@ -173,18 +175,28 @@
         return self.get(object_type, getattr(zenpy_object, cache_key_attr)) is not None
 
     def should_cache(self, zenpy_object):
         """ Determine whether or not this object should be cached (ie, a cache exists for it's object_type) """
         return get_object_type(zenpy_object) in self.mapping
 
     def disable(self):
+        """Disables cache"""
         self.disabled = True
 
     def enable(self):
+        """Enables cache"""
         self.disabled = False
 
+    def status(self):
+        """Returns current cache status"""
+        return 'Cache disabled' if self.disabled else 'Cache enabled'
+
+    def get_cache_engines(self):
+        """Returns list of caches available in cachetools"""
+        return ZenpyCache.AVAILABLE_CACHES
+
     def _cache_key_attribute(self, object_type):
         """ Return the attribute used as the cache_key for a particular object type. """
         # This function used to return the key for objects that are not referenced by id.
         # These objects are no longer cached (UserField, OrganizationalField) and so the
         # function has no purpose anymore. I'm leaving it here in case it comes in handy again
         return 'id'
```

### Comparing `zenpy-2.0.8/zenpy/lib/mapping.py` & `zenpy-2.0.9/zenpy/lib/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 log = logging.getLogger(__name__)
 
 __author__ = 'facetoe'
 
 
 class ZendeskObjectMapping(object):
     """
-    Handle converting Zendesk JSON objects to Python ones.
+    Handle converting Zendesk Support JSON objects to Python ones.
     """
     class_mapping = {
         'ticket': Ticket,
+        'deleted_ticket': Ticket,
         'user': User,
         'deleted_user': User,
         'organization': Organization,
         'group': Group,
         'brand': Brand,
         'topic': Topic,
         'comment': Comment,
@@ -190,15 +191,15 @@
             key = '{}'.format(key)
         return key
 
 
 class ChatObjectMapping(ZendeskObjectMapping):
     """
     Handle converting Chat API objects to Python ones. This class exists
-    mainly to prevent namespace collisions between the two APIs.
+    to prevent namespace collisions between APIs.
     """
     class_mapping = {
         'chat': Chat,
         'offline_msg': OfflineMessage,
         'session': Session,
         'response_time': ResponseTime,
         'visitor': Visitor,
@@ -216,14 +217,18 @@
         'ip_address': IpAddress,
         'department': Department,
         'goal': Goal
     }
 
 
 class HelpCentreObjectMapping(ZendeskObjectMapping):
+    """
+    Handle converting Helpdesk API objects to Python ones. This class exists
+    to prevent namespace collisions between APIs.
+    """
     class_mapping = {
         'article': Article,
         'category': Category,
         'section': Section,
         'comment': zenpy.lib.api_objects.help_centre_objects.Comment,
         'article_attachment': zenpy.lib.api_objects.help_centre_objects.ArticleAttachment,
         'label': Label,
@@ -233,14 +238,18 @@
         'subscription': Subscription,
         'vote': Vote,
         'access_policy': AccessPolicy,
         'user_segment': UserSegment
     }
 
 class TalkObjectMapping(ZendeskObjectMapping):
+    """
+    Handle converting Talk API objects to Python ones. This class exists
+    to prevent namespace collisions between APIs.
+    """
     class_mapping = {
         'account_overview': AccountOverview,
         'agents_activity': AgentsActivity,
         'agents_overview': AgentsOverview,
         'current_queue_activity': CurrentQueueActivity,
         'phone_numbers': PhoneNumbers,
         'availability': ShowAvailability
```

### Comparing `zenpy-2.0.8/zenpy/lib/request.py` & `zenpy-2.0.9/zenpy/lib/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import collections
 import os
 
 from zenpy.lib.api_objects.chat_objects import Shortcut, Trigger
 from zenpy.lib.endpoint import EndpointFactory
-from zenpy.lib.exception import ZenpyException
+from zenpy.lib.exception import ZenpyException, TooManyValuesException
 from zenpy.lib.util import get_object_type, as_plural, is_iterable_but_not_string
 
 
 class RequestHandler(object):
     """
     Abstraction of a request to either the Zendesk API or the Chat API. Only POST, PUT and
     DELETE are handled. Subclasses implement the logic needed to correctly serialize the request
@@ -493,26 +493,55 @@
 
     def delete(self, endpoint, translation):
         url = self.api._build_url(endpoint(id=translation))
         return self.api._delete(url)
 
 
 class HelpdeskAttachmentRequest(BaseZendeskRequest):
+    def build_payload(self, ids):
+        return {'attachment_ids': ids}
+
     def delete(self, endpoint, article_attachment):
         url = self.api._build_url(endpoint(id=article_attachment))
         return self.api._delete(url)
 
     def put(self, api_objects, *args, **kwargs):
         raise NotImplementedError("You cannot update HelpCentre attachments!")
 
-    def post(self, endpoint, attachment, article=None, inline=False):
+    def post(self, endpoint, attachments, article=None, inline=False, file_name=None, content_type=None):
         if article:
             url = self.api._build_url(endpoint(id=article))
         else:
             url = self.api._build_url(endpoint())
 
-        if hasattr(attachment, 'read'):
-            return self.api._post(url, payload={}, files=dict(file=attachment))
-        elif os.path.isfile(attachment):
-            with open(attachment, 'rb') as fp:
-                return self.api._post(url, payload={}, files=dict(file=fp))
+        if endpoint == self.api.endpoint.bulk_attachments:
+            self.check_type(attachments)
+            if isinstance(attachments, collections.Iterable):
+                if len(attachments) > 20:
+                    raise TooManyValuesException('Maximum 20 attachments objects allowed')
+                ids = [attachment.id for attachment in attachments]
+            else:
+                ids = attachments.id
+            content_type = "application/json"
+            return self.api._post(url, payload=self.build_payload(ids), content_type=content_type)
+        else:
+            if hasattr(attachments, 'read'):
+                file = (file_name if file_name else attachments.name, attachments, content_type)
+                return self.api._post(url,
+                                          payload={},
+                                          files=dict(
+                                                     inline=(None, 'true' if inline else 'false'),
+                                                     file=file
+                                                     )
+                                          )
+            elif os.path.isfile(attachments):
+                with open(attachments, 'rb') as fp:
+                    file = (file_name if file_name else fp.name, fp, content_type)
+                    return self.api._post(url,
+                                          payload={},
+                                          files=dict(
+                                                     inline=(None, 'true' if inline else 'false'),
+                                                     file=file
+                                                     )
+                                          )
+
         raise ValueError("Attachment is not a file-like object or valid path!")
```

### Comparing `zenpy-2.0.8/README.md` & `zenpy-2.0.9/README.md`

 * *Files identical despite different names*

