# Comparing `tmp/django-stubs-ext-4.2.7.tar.gz` & `tmp/django_stubs_ext-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-stubs-ext-4.2.7.tar", last modified: Tue Dec  5 19:01:55 2023, max compression
+gzip compressed data, was "django_stubs_ext-5.0.0.tar", last modified: Tue Apr 30 10:02:55 2024, max compression
```

## Comparing `django-stubs-ext-4.2.7.tar` & `django_stubs_ext-5.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:01:55.208542 django-stubs-ext-4.2.7/
--rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-10-18 16:47:22.000000 django-stubs-ext-4.2.7/LICENSE.md
--rw-r--r--   0 marti     (1000) marti      (121)     3554 2023-12-05 19:01:55.208542 django-stubs-ext-4.2.7/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)     2496 2023-10-18 16:47:22.000000 django-stubs-ext-4.2.7/README.md
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:01:55.205209 django-stubs-ext-4.2.7/django_stubs_ext/
--rw-r--r--   0 marti     (1000) marti      (121)      535 2023-10-18 16:47:22.000000 django-stubs-ext-4.2.7/django_stubs_ext/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)      620 2023-10-18 16:47:22.000000 django-stubs-ext-4.2.7/django_stubs_ext/aliases.py
--rw-r--r--   0 marti     (1000) marti      (121)      693 2023-10-18 16:47:22.000000 django-stubs-ext-4.2.7/django_stubs_ext/annotations.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:01:55.208542 django-stubs-ext-4.2.7/django_stubs_ext/db/
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-10-18 16:47:22.000000 django-stubs-ext-4.2.7/django_stubs_ext/db/__init__.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:01:55.208542 django-stubs-ext-4.2.7/django_stubs_ext/db/models/
--rw-r--r--   0 marti     (1000) marti      (121)     1911 2023-12-05 19:01:16.000000 django-stubs-ext-4.2.7/django_stubs_ext/db/models/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)      769 2023-12-05 19:01:16.000000 django-stubs-ext-4.2.7/django_stubs_ext/db/models/manager.py
--rw-r--r--   0 marti     (1000) marti      (121)      978 2023-10-18 16:47:22.000000 django-stubs-ext-4.2.7/django_stubs_ext/db/router.py
--rw-r--r--   0 marti     (1000) marti      (121)     3851 2023-12-05 19:01:16.000000 django-stubs-ext-4.2.7/django_stubs_ext/patch.py
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-10-18 16:47:22.000000 django-stubs-ext-4.2.7/django_stubs_ext/py.typed
--rw-r--r--   0 marti     (1000) marti      (121)      236 2023-10-18 16:47:22.000000 django-stubs-ext-4.2.7/django_stubs_ext/types.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:01:55.208542 django-stubs-ext-4.2.7/django_stubs_ext.egg-info/
--rw-r--r--   0 marti     (1000) marti      (121)     3554 2023-12-05 19:01:55.000000 django-stubs-ext-4.2.7/django_stubs_ext.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)      585 2023-12-05 19:01:55.000000 django-stubs-ext-4.2.7/django_stubs_ext.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti      (121)        1 2023-12-05 19:01:55.000000 django-stubs-ext-4.2.7/django_stubs_ext.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti      (121)       25 2023-12-05 19:01:55.000000 django-stubs-ext-4.2.7/django_stubs_ext.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti      (121)       17 2023-12-05 19:01:55.000000 django-stubs-ext-4.2.7/django_stubs_ext.egg-info/top_level.txt
--rw-r--r--   0 marti     (1000) marti      (121)       38 2023-12-05 19:01:55.208542 django-stubs-ext-4.2.7/setup.cfg
--rwxr-xr-x   0 marti     (1000) marti      (121)     1713 2023-12-05 19:01:16.000000 django-stubs-ext-4.2.7/setup.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-12-05 19:01:55.208542 django-stubs-ext-4.2.7/tests/
--rw-r--r--   0 marti     (1000) marti      (121)      169 2023-10-18 16:47:22.000000 django-stubs-ext-4.2.7/tests/test_aliases.py
--rw-r--r--   0 marti     (1000) marti      (121)     3936 2023-10-18 16:47:22.000000 django-stubs-ext-4.2.7/tests/test_monkeypatching.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1075 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/LICENSE.md
+-rw-r--r--   0 marti     (1000) marti     (1000)     3578 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti     (1000)     2496 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/README.md
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/django_stubs_ext/
+-rw-r--r--   0 marti     (1000) marti     (1000)      535 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/django_stubs_ext/__init__.py
+-rw-r--r--   0 marti     (1000) marti     (1000)      620 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/django_stubs_ext/aliases.py
+-rw-r--r--   0 marti     (1000) marti     (1000)      693 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/django_stubs_ext/annotations.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/django_stubs_ext/db/
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/django_stubs_ext/db/__init__.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/django_stubs_ext/db/models/
+-rw-r--r--   0 marti     (1000) marti     (1000)     1911 2023-12-05 19:01:16.000000 django_stubs_ext-5.0.0/django_stubs_ext/db/models/__init__.py
+-rw-r--r--   0 marti     (1000) marti     (1000)      814 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/django_stubs_ext/db/models/manager.py
+-rw-r--r--   0 marti     (1000) marti     (1000)      930 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/django_stubs_ext/db/router.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     3902 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/django_stubs_ext/patch.py
+-rw-r--r--   0 marti     (1000) marti     (1000)        0 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/django_stubs_ext/py.typed
+-rw-r--r--   0 marti     (1000) marti     (1000)      220 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/django_stubs_ext/types.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/
+-rw-r--r--   0 marti     (1000) marti     (1000)     3578 2024-04-30 10:02:55.000000 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti     (1000)      585 2024-04-30 10:02:55.000000 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)        1 2024-04-30 10:02:55.000000 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)       25 2024-04-30 10:02:55.000000 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)       17 2024-04-30 10:02:55.000000 django_stubs_ext-5.0.0/django_stubs_ext.egg-info/top_level.txt
+-rw-r--r--   0 marti     (1000) marti     (1000)       38 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/setup.cfg
+-rwxr-xr-x   0 marti     (1000) marti     (1000)     1736 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/setup.py
+drwxr-xr-x   0 marti     (1000) marti     (1000)        0 2024-04-30 10:02:55.564887 django_stubs_ext-5.0.0/tests/
+-rw-r--r--   0 marti     (1000) marti     (1000)      169 2023-10-18 16:47:22.000000 django_stubs_ext-5.0.0/tests/test_aliases.py
+-rw-r--r--   0 marti     (1000) marti     (1000)     3928 2024-04-30 10:01:49.000000 django_stubs_ext-5.0.0/tests/test_monkeypatching.py
```

### Comparing `django-stubs-ext-4.2.7/LICENSE.md` & `django_stubs_ext-5.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.7/PKG-INFO` & `django_stubs_ext-5.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: django-stubs-ext
-Version: 4.2.7
+Version: 5.0.0
 Summary: Monkey-patching and extensions for django-stubs
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Simula Proxy
-Author-email: 3nki.nam.shub@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
+Project-URL: Funding, https://github.com/sponsors/typeddjango
 Project-URL: Release notes, https://github.com/typeddjango/django-stubs/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
 Requires-Dist: typing-extensions
 
 # Extensions and monkey-patching for django-stubs
```

### Comparing `django-stubs-ext-4.2.7/README.md` & `django_stubs_ext-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.7/django_stubs_ext/__init__.py` & `django_stubs_ext-5.0.0/django_stubs_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.7/django_stubs_ext/aliases.py` & `django_stubs_ext-5.0.0/django_stubs_ext/aliases.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.7/django_stubs_ext/annotations.py` & `django_stubs_ext-5.0.0/django_stubs_ext/annotations.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.7/django_stubs_ext/db/models/__init__.py` & `django_stubs_ext-5.0.0/django_stubs_ext/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.7/django_stubs_ext/db/router.py` & `django_stubs_ext-5.0.0/django_stubs_ext/db/router.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,23 +10,19 @@
         Typed base class for Django's DATABASE_ROUTERS setting. At runtime this is just an alias to `object`.
 
         All methods are optional.
 
         Django documentation: https://docs.djangoproject.com/en/stable/topics/db/multi-db/#automatic-database-routing
         """
 
-        def db_for_read(self, model: Type[Model], **hints: Any) -> Optional[str]:
-            ...
+        def db_for_read(self, model: Type[Model], **hints: Any) -> Optional[str]: ...
 
-        def db_for_write(self, model: Type[Model], **hints: Any) -> Optional[str]:
-            ...
+        def db_for_write(self, model: Type[Model], **hints: Any) -> Optional[str]: ...
 
-        def allow_relation(self, obj1: Type[Model], obj2: Type[Model], **hints: Any) -> Optional[bool]:
-            ...
+        def allow_relation(self, obj1: Type[Model], obj2: Type[Model], **hints: Any) -> Optional[bool]: ...
 
         def allow_migrate(
             self, db: str, app_label: str, model_name: Optional[str] = None, **hints: Any
-        ) -> Optional[bool]:
-            ...
+        ) -> Optional[bool]: ...
 
 else:
     TypedDatabaseRouter = object
```

### Comparing `django-stubs-ext-4.2.7/django_stubs_ext/patch.py` & `django_stubs_ext-5.0.0/django_stubs_ext/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from django.db.models.expressions import ExpressionWrapper
 from django.db.models.fields import Field
 from django.db.models.fields.related import ForeignKey
 from django.db.models.lookups import Lookup
 from django.db.models.manager import BaseManager
 from django.db.models.query import QuerySet
 from django.forms.formsets import BaseFormSet
-from django.forms.models import BaseModelForm, BaseModelFormSet
+from django.forms.models import BaseModelForm, BaseModelFormSet, ModelChoiceField
 from django.utils.connection import BaseConnectionHandler
 from django.views.generic.detail import SingleObjectMixin
 from django.views.generic.edit import DeletionMixin, FormMixin
 from django.views.generic.list import MultipleObjectMixin
 
 __all__ = ["monkeypatch"]
 
@@ -59,14 +59,15 @@
     MPGeneric(MultipleObjectMixin),
     MPGeneric(BaseModelAdmin),
     MPGeneric(Field),
     MPGeneric(Paginator),
     MPGeneric(BaseFormSet),
     MPGeneric(BaseModelForm),
     MPGeneric(BaseModelFormSet),
+    MPGeneric(ModelChoiceField),
     MPGeneric(Feed),
     MPGeneric(Sitemap),
     MPGeneric(SuccessMessageMixin),
     MPGeneric(FileProxyMixin),
     MPGeneric(Lookup),
     MPGeneric(BaseConnectionHandler),
     MPGeneric(ExpressionWrapper),
```

### Comparing `django-stubs-ext-4.2.7/django_stubs_ext.egg-info/PKG-INFO` & `django_stubs_ext-5.0.0/django_stubs_ext.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: django-stubs-ext
-Version: 4.2.7
+Version: 5.0.0
 Summary: Monkey-patching and extensions for django-stubs
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Simula Proxy
-Author-email: 3nki.nam.shub@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
+Project-URL: Funding, https://github.com/sponsors/typeddjango
 Project-URL: Release notes, https://github.com/typeddjango/django-stubs/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
 Requires-Dist: typing-extensions
 
 # Extensions and monkey-patching for django-stubs
```

### Comparing `django-stubs-ext-4.2.7/django_stubs_ext.egg-info/SOURCES.txt` & `django_stubs_ext-5.0.0/django_stubs_ext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.7/setup.py` & `django_stubs_ext-5.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 #!/usr/bin/env python
-from distutils.core import setup
-
-from setuptools import find_packages
+from setuptools import find_packages, setup  # type: ignore[import-untyped]
 
 with open("README.md") as f:
     readme = f.read()
 
 dependencies = [
     "django",
     "typing-extensions",
 ]
 
 # NB! For clarity, keep version major.minor.patch in sync with django-stubs.
 # It's fine to skip django-stubs-ext releases, but when doing a release, update this to newest django-stubs version.
 setup(
     name="django-stubs-ext",
-    version="4.2.7",
+    version="5.0.0",
     description="Monkey-patching and extensions for django-stubs",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     license_files=["LICENSE.md"],
     url="https://github.com/typeddjango/django-stubs",
     author="Simula Proxy",
-    author_email="3nki.nam.shub@gmail.com",
     maintainer="Marti Raudsepp",
     maintainer_email="marti@juffo.org",
     py_modules=[],
     python_requires=">=3.8",
     install_requires=dependencies,
     packages=["django_stubs_ext", *find_packages(exclude=["scripts"])],
     package_data={"django_stubs_ext": ["py.typed"]},
@@ -37,15 +34,16 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Typing :: Typed",
         "Framework :: Django",
-        "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
+        "Framework :: Django :: 5.0",
     ],
     project_urls={
+        "Funding": "https://github.com/sponsors/typeddjango",
         "Release notes": "https://github.com/typeddjango/django-stubs/releases",
     },
 )
```

### Comparing `django-stubs-ext-4.2.7/tests/test_monkeypatching.py` & `django_stubs_ext-5.0.0/tests/test_monkeypatching.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
     """Used to represent a type of ``make_generic_classes`` fixture."""
 
     def __call__(
         self,
         django_version: Optional[_VersionSpec] = None,
         extra_classes: Optional[Iterable[type]] = None,
         include_builtins: bool = True,
-    ) -> None:
-        ...
+    ) -> None: ...
 
 
 @pytest.fixture(scope="function")
 def make_generic_classes(
     request: FixtureRequest,
     monkeypatch: MonkeyPatch,
 ) -> _MakeGenericClasses:
```

