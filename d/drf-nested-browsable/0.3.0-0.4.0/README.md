# Comparing `tmp/drf_nested_browsable-0.3.0.tar.gz` & `tmp/drf_nested_browsable-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_nested_browsable-0.3.0.tar", max compression
+gzip compressed data, was "drf_nested_browsable-0.4.0.tar", max compression
```

## Comparing `drf_nested_browsable-0.3.0.tar` & `drf_nested_browsable-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1783 2024-04-29 08:01:11.719321 drf_nested_browsable-0.3.0/README.md
--rw-r--r--   0        0        0      213 2024-02-08 16:17:25.775220 drf_nested_browsable-0.3.0/drf_nested_browsable/__init__.py
--rw-r--r--   0        0        0     7010 2024-04-29 07:57:24.554538 drf_nested_browsable-0.3.0/drf_nested_browsable/serializers.py
--rw-r--r--   0        0        0     3419 2024-02-08 16:17:25.775220 drf_nested_browsable-0.3.0/drf_nested_browsable/templates/writable_list.html
--rw-r--r--   0        0        0        0 2024-02-08 16:17:25.775220 drf_nested_browsable-0.3.0/drf_nested_browsable/templatetags/__init__.py
--rw-r--r--   0        0        0     4200 2024-02-08 16:17:25.775220 drf_nested_browsable-0.3.0/drf_nested_browsable/templatetags/drf_nested_browsable.py
--rw-r--r--   0        0        0     1193 2024-04-29 08:02:55.806714 drf_nested_browsable-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2795 1970-01-01 00:00:00.000000 drf_nested_browsable-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1783 2024-04-29 08:01:11.719321 drf_nested_browsable-0.4.0/README.md
+-rw-r--r--   0        0        0      213 2024-02-08 16:17:25.775220 drf_nested_browsable-0.4.0/drf_nested_browsable/__init__.py
+-rw-r--r--   0        0        0     7254 2024-04-30 10:53:41.469399 drf_nested_browsable-0.4.0/drf_nested_browsable/serializers.py
+-rw-r--r--   0        0        0     3419 2024-02-08 16:17:25.775220 drf_nested_browsable-0.4.0/drf_nested_browsable/templates/writable_list.html
+-rw-r--r--   0        0        0        0 2024-02-08 16:17:25.775220 drf_nested_browsable-0.4.0/drf_nested_browsable/templatetags/__init__.py
+-rw-r--r--   0        0        0     4200 2024-02-08 16:17:25.775220 drf_nested_browsable-0.4.0/drf_nested_browsable/templatetags/drf_nested_browsable.py
+-rw-r--r--   0        0        0     1193 2024-04-30 11:05:16.483683 drf_nested_browsable-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2795 1970-01-01 00:00:00.000000 drf_nested_browsable-0.4.0/PKG-INFO
```

### Comparing `drf_nested_browsable-0.3.0/README.md` & `drf_nested_browsable-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.3.0/drf_nested_browsable/serializers.py` & `drf_nested_browsable-0.4.0/drf_nested_browsable/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,24 +95,29 @@
 
         updated_ids = []
 
         if not (partial and validated_data is None):
             for new_elem in validated_data:
                 full_elem = {**new_elem, **self.parent_data}
 
-                try:
-                    elem = instance.get(
-                        **{
-                            key: new_elem[key] for key in keys if key in new_elem.keys()
-                        },
-                        **self.parent_data,
-                    )
-                    elem = self.child.update(elem, full_elem)
-                except instance.model.DoesNotExist:
+                if not set(new_elem).intersection(set(keys)):
                     elem = self.child.create(full_elem)
+                else:
+                    try:
+                        elem = instance.get(
+                            **{
+                                key: new_elem[key]
+                                for key in keys
+                                if key in new_elem.keys()
+                            },
+                            **self.parent_data,
+                        )
+                        elem = self.child.update(elem, full_elem)
+                    except instance.model.DoesNotExist:
+                        elem = self.child.create(full_elem)
                 updated_ids.append(elem.id)
 
             instance.exclude(id__in=updated_ids).delete()
 
 
 class WritableNestedModelSerializer(ModelSerializer):
     """
```

### Comparing `drf_nested_browsable-0.3.0/drf_nested_browsable/templates/writable_list.html` & `drf_nested_browsable-0.4.0/drf_nested_browsable/templates/writable_list.html`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.3.0/drf_nested_browsable/templatetags/drf_nested_browsable.py` & `drf_nested_browsable-0.4.0/drf_nested_browsable/templatetags/drf_nested_browsable.py`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.3.0/pyproject.toml` & `drf_nested_browsable-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-nested-browsable"
-version = "0.3.0"
+version = "0.4.0"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Framework :: Django",
     "Intended Audience :: Developers"
 ]
 description = "Writable nested serializers with forms for the Browsable API"
 keywords = ["django", "rest framework", "drf", "browsable api", "nested serializers"]
```

### Comparing `drf_nested_browsable-0.3.0/PKG-INFO` & `drf_nested_browsable-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-nested-browsable
-Version: 0.3.0
+Version: 0.4.0
 Summary: Writable nested serializers with forms for the Browsable API
 Home-page: https://pierre-couy.dev/projects/drf-nested-browsable.html
 License: MIT
 Keywords: django,rest framework,drf,browsable api,nested serializers
 Author: Pierre Couy
 Author-email: contact@pierre-couy.dev
 Requires-Python: >=3.10,<4.0
```

