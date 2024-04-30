# Comparing `tmp/pydanja-0.1.8.tar.gz` & `tmp/pydanja-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydanja-0.1.8.tar", last modified: Sat Aug 12 12:21:52 2023, max compression
+gzip compressed data, was "pydanja-0.1.9.tar", last modified: Sat Aug 12 13:03:28 2023, max compression
```

## Comparing `pydanja-0.1.8.tar` & `pydanja-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-08-12 06:24:35.361339 pydanja-0.1.8/LICENSE
--rw-r--r--   0        0        0     4864 2023-08-12 12:19:33.640700 pydanja-0.1.8/README.md
--rw-r--r--   0        0        0     1507 2023-08-12 12:21:52.192382 pydanja-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6305 2023-08-12 12:20:47.252528 pydanja-0.1.8/src/pydanja/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 04:57:14.398442 pydanja-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     5842 2023-08-12 05:09:54.860767 pydanja-0.1.8/tests/fixtures/multiple_resource_with_id.json
--rw-r--r--   0        0        0     4848 2023-08-12 04:08:57.658463 pydanja-0.1.8/tests/fixtures/single_resource_with_id.json
--rw-r--r--   0        0        0     4848 2023-08-12 04:12:55.354347 pydanja-0.1.8/tests/fixtures/single_resource_without_id.json
--rw-r--r--   0        0        0     3282 2023-08-12 05:29:35.569454 pydanja-0.1.8/tests/test_resource_creation.py
--rw-r--r--   0        0        0     5888 1970-01-01 00:00:00.000000 pydanja-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-12 06:24:35.361339 pydanja-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4864 2023-08-12 12:19:33.640700 pydanja-0.1.9/README.md
+-rw-r--r--   0        0        0     1507 2023-08-12 13:03:28.789887 pydanja-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7021 2023-08-12 12:59:26.934128 pydanja-0.1.9/src/pydanja/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 04:57:14.398442 pydanja-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     5842 2023-08-12 05:09:54.860767 pydanja-0.1.9/tests/fixtures/multiple_resource_with_id.json
+-rw-r--r--   0        0        0     4848 2023-08-12 04:08:57.658463 pydanja-0.1.9/tests/fixtures/single_resource_with_id.json
+-rw-r--r--   0        0        0     4848 2023-08-12 04:12:55.354347 pydanja-0.1.9/tests/fixtures/single_resource_without_id.json
+-rw-r--r--   0        0        0     3282 2023-08-12 05:29:35.569454 pydanja-0.1.9/tests/test_resource_creation.py
+-rw-r--r--   0        0        0     5888 1970-01-01 00:00:00.000000 pydanja-0.1.9/PKG-INFO
```

### Comparing `pydanja-0.1.8/LICENSE` & `pydanja-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydanja-0.1.8/README.md` & `pydanja-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pydanja-0.1.8/pyproject.toml` & `pydanja-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydanja"
-version = "0.1.8"
+version = "0.1.9"
 description = "JSON:API Support for Pydantic"
 authors = [
     { name = "Chris Read", email = "centurix@gmail.com" },
 ]
 dependencies = [
     "pydantic>=2.1.1",
 ]
```

### Comparing `pydanja-0.1.8/src/pydanja/__init__.py` & `pydanja-0.1.9/src/pydanja/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,29 +11,78 @@
     "DANJAErrorList"
 ]
 
 
 ResourceType = TypeVar("ResourceType", bound=BaseModel)
 
 
+class DANJALink(BaseModel):
+    """JSON:API Link"""
+    href: str
+    rel: Optional[str] = None
+    describedby: Optional[str] = None
+    title: Optional[str] = None
+    type: Optional[str] = None
+    hreflang: Optional[str] = None
+    meta: Optional[Dict[str, Any]] = None
+
+
+class DANJASource(BaseModel):
+    """JSON:API Source"""
+    pointer: str
+    parameter: str
+    header: str
+
+
+class DANJAResourceIdentifier(BaseModel):
+    """JSON:API Resource Identifier"""
+    type: str
+    id: str
+    lid: Optional[str] = None
+
+
+class DANJARelationship(BaseModel):
+    """JSON:API Relationship"""
+    links: Optional[Dict[str, Union[str, DANJALink, None]]] = None
+    data: Optional[Dict[str, Union[DANJAResourceIdentifier, List[DANJAResourceIdentifier], None]]] = None  # noqa: E501
+    meta: Optional[Dict[str, Any]] = None
+
+
+class DANJAError(BaseModel):
+    """JSON:API Error object"""
+    id: Optional[str] = None
+    links: Optional[Dict[str, Union[str, DANJALink, None]]] = None
+    status: Optional[str] = None
+    code: Optional[str] = None
+    title: Optional[str] = None
+    detail: Optional[str] = None
+    source: Optional[Dict[str, DANJASource]] = None
+    meta: Optional[Dict[str, Any]] = None
+
+
+class DANJAErrorList(BaseModel):
+    """JSON:API Error list"""
+    errors: List[DANJAError]
+
+
 class DANJASingleResource(BaseModel, Generic[ResourceType]):
     """A single resource. The only JSON:API required field is type"""
     id: Optional[str] = None
     type: str
     lid: Optional[str] = None
     attributes: ResourceType
-    relationships: Optional[Dict[str, Any]] = None
+    relationships: Optional[Dict[str, DANJARelationship]] = None
     links: Optional[Dict[str, Any]] = None
     meta: Optional[Dict[str, Any]] = None
 
 
 class DANJAResource(BaseModel, Generic[ResourceType]):
     """JSON:API base for a single resource"""
     data: DANJASingleResource[ResourceType]
-    links: Optional[Dict[str, Any]] = None
+    links: Optional[Dict[str, Union[str, DANJALink, None]]] = None
     meta: Optional[Dict[str, Any]] = None
     included: Optional[List[Dict[str, Any]]] = None
 
     @property
     def resource(self) -> ResourceType:
         return self.data.attributes
 
@@ -85,15 +134,15 @@
                 f"Resource ID field not found in {resource_name}: {resource_id}"
             )
 
 
 class DANJAResourceList(BaseModel, Generic[ResourceType]):
     """JSON:API base for a list of resources"""
     data: List[DANJASingleResource[ResourceType]]
-    links: Optional[Dict[str, Any]] = None
+    links: Optional[Dict[str, Union[str, DANJALink, None]]] = None
     meta: Optional[Dict[str, Any]] = None
     included: Optional[List[Dict[str, Any]]] = None
 
     @property
     def resources(self) -> List[ResourceType]:
         return [data.attributes for data in self.data]
 
@@ -156,35 +205,7 @@
                 data.append(DANJASingleResource(**values))
 
             return cls(data=data)
         except AttributeError:
             raise Exception(
                 f"Resource ID field not found in {resource_name}: {resource_id}"
             )
-
-
-class DANJALink(BaseModel):
-    """JSON:API Link"""
-    href: str
-    rel: Optional[str]
-    describedby: Optional[str]
-    title: Optional[str]
-    type: Optional[str]
-    hreflang: Optional[str]
-    meta: Optional[Dict[str, Any]]
-
-
-class DANJAError(BaseModel):
-    """JSON:API Error object"""
-    id: Optional[str]
-    links: Optional[Dict[str, Union[str, DANJALink, None]]]
-    status: Optional[str]
-    code: Optional[str]
-    title: Optional[str]
-    detail: Optional[str]
-    source: Optional[Dict[str, Any]]
-    meta: Optional[Dict[str, Any]]
-
-
-class DANJAErrorList(BaseModel):
-    """JSON:API Error list"""
-    errors: List[DANJAError]
```

### Comparing `pydanja-0.1.8/tests/fixtures/multiple_resource_with_id.json` & `pydanja-0.1.9/tests/fixtures/multiple_resource_with_id.json`

 * *Files identical despite different names*

### Comparing `pydanja-0.1.8/tests/fixtures/single_resource_with_id.json` & `pydanja-0.1.9/tests/fixtures/single_resource_with_id.json`

 * *Files identical despite different names*

### Comparing `pydanja-0.1.8/tests/fixtures/single_resource_without_id.json` & `pydanja-0.1.9/tests/fixtures/single_resource_without_id.json`

 * *Files identical despite different names*

### Comparing `pydanja-0.1.8/tests/test_resource_creation.py` & `pydanja-0.1.9/tests/test_resource_creation.py`

 * *Files identical despite different names*

### Comparing `pydanja-0.1.8/PKG-INFO` & `pydanja-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydanja
-Version: 0.1.8
+Version: 0.1.9
 Summary: JSON:API Support for Pydantic
 Keywords: pydantic jsonapi json:api openapi fastapi
 Home-page: https://github.com/Centurix/pydanja
 Author-Email: Chris Read <centurix@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

