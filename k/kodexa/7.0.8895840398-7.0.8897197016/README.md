# Comparing `tmp/kodexa-7.0.8895840398.tar.gz` & `tmp/kodexa-7.0.8897197016.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.8895840398.tar", max compression
+gzip compressed data, was "kodexa-7.0.8897197016.tar", max compression
```

## Comparing `kodexa-7.0.8895840398.tar` & `kodexa-7.0.8897197016.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0    11357 2024-04-30 13:41:16.794320 kodexa-7.0.8895840398/LICENSE
--rw-r--r--   0        0        0     2178 2024-04-30 13:41:16.794320 kodexa-7.0.8895840398/README.md
--rw-r--r--   0        0        0      957 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/base.py
--rw-r--r--   0        0        0     3592 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/entities/product.py
--rw-r--r--   0        0        0     3873 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/entities/product_subscription.py
--rw-r--r--   0        0        0   115561 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/model.py
--rw-r--r--   0        0        0   175470 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/objects.py
--rw-r--r--   0        0        0    62032 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   214979 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    34024 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-04-30 13:41:16.802320 kodexa-7.0.8895840398/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 13:41:16.806320 kodexa-7.0.8895840398/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1389 2024-04-30 13:41:34.238227 kodexa-7.0.8895840398/pyproject.toml
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8895840398/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 15:09:26.303766 kodexa-7.0.8897197016/LICENSE
+-rw-r--r--   0        0        0     2178 2024-04-30 15:09:26.303766 kodexa-7.0.8897197016/README.md
+-rw-r--r--   0        0        0      957 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/base.py
+-rw-r--r--   0        0        0        0 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/entities/__init__.py
+-rw-r--r--   0        0        0     3526 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/entities/product.py
+-rw-r--r--   0        0        0     3814 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/entities/product_subscription.py
+-rw-r--r--   0        0        0   115561 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/model.py
+-rw-r--r--   0        0        0   174318 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/objects.py
+-rw-r--r--   0        0        0    62032 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   216867 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    34024 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1389 2024-04-30 15:09:40.991799 kodexa-7.0.8897197016/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8897197016/PKG-INFO
```

### Comparing `kodexa-7.0.8895840398/LICENSE` & `kodexa-7.0.8897197016/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/README.md` & `kodexa-7.0.8897197016/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/__init__.py` & `kodexa-7.0.8897197016/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/assistant/assistant.py` & `kodexa-7.0.8897197016/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/connectors/connectors.py` & `kodexa-7.0.8897197016/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/model/__init__.py` & `kodexa-7.0.8897197016/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/model/base.py` & `kodexa-7.0.8897197016/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/model/entities/product.py` & `kodexa-7.0.8897197016/kodexa/model/entities/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from dataclasses import Field
 from typing import Optional, List
 
-from pydantic import BaseModel, ConfigDict
-
+from pydantic import BaseModel, ConfigDict, Field
 from kodexa.model.base import StandardDateTime
 from kodexa.platform.client import EntityEndpoint, PageEndpoint, EntitiesEndpoint
 
 
 class Product(BaseModel):
     """
 
@@ -17,15 +15,16 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     A product
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+
+    id: Optional[str] = None
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     name: str
     description: Optional[str] = None
     overview_markdown: Optional[str] = Field(None, alias="overviewMarkdown")
```

### Comparing `kodexa-7.0.8895840398/kodexa/model/entities/product_subscription.py` & `kodexa-7.0.8897197016/kodexa/model/entities/product_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from dataclasses import Field
 from typing import Optional, List
 
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, Field
 
 from kodexa.model.base import StandardDateTime
 from kodexa.model.entities.product import Product
 from kodexa.model.objects import Organization
 from kodexa.platform.client import EntityEndpoint, PageEndpoint, EntitiesEndpoint
 
 
@@ -16,15 +15,15 @@
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     product: Optional[Product] = None
     organization: Optional[Organization] = None
```

### Comparing `kodexa-7.0.8895840398/kodexa/model/model.py` & `kodexa-7.0.8897197016/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/model/objects.py` & `kodexa-7.0.8897197016/kodexa/model/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     name: str
     slug: str = Field(pattern=r"^[a-zA-Z0-9\-_]{0,100}$")
     public_access: Optional[bool] = Field(None, alias="publicAccess")
@@ -236,15 +236,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     name: Optional[str] = None
     description: Optional[str] = None
     organization: Optional[Organization] = None
@@ -1111,15 +1111,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     color: Optional[str] = None
     icon: Optional[str] = None
     status: Optional[str] = None
     status_type: Optional[StatusType1] = Field(None, alias="statusType")
@@ -1198,15 +1198,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     color: Optional[str] = None
     icon: Optional[str] = None
     status: str
@@ -1233,15 +1233,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     Provides the definition of a transition for a document, where a change was applied by an assistant, user or external process
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     unknown_fields: Optional[Dict[str, str]] = Field(None, alias="unknownFields")
     transition_type: Optional[TransitionType] = Field(
         None, alias="transitionType", description="The type of transition"
@@ -1413,15 +1413,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     The labels from the latest content object in the family
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     name: str
     color: Optional[str] = None
     label: str
@@ -1437,15 +1437,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     A project tag
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     name: str
     color: Optional[str] = None
 
 
 class PathExtractedData(BaseModel):
     """
 
@@ -1515,15 +1515,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     token: Optional[str] = None
     last_accessed: Optional[StandardDateTime] = Field(None, alias="lastAccessed")
 
@@ -1574,15 +1574,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     message: Optional[str] = None
     option: Optional[str] = None
     description: Optional[str] = None
 
@@ -1668,15 +1668,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     A data exception
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     message: str
     exception_details: Optional[str] = Field(None, alias="exceptionDetails")
     severity: Optional[str] = None
@@ -1818,15 +1818,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     welcome_markdown: Optional[str] = Field(None, alias="welcomeMarkdown")
     news_markdown: Optional[str] = Field(None, alias="newsMarkdown")
     about_markdown: Optional[str] = Field(None, alias="aboutMarkdown")
@@ -1870,15 +1870,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     name: Optional[str] = None
     state: Optional[str] = None
     training_materials_generated: Optional[bool] = Field(
         None, alias="trainingMaterialsGenerated"
     )
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
@@ -1963,15 +1963,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     log_date: Optional[StandardDateTime] = Field(None, alias="logDate")
     entry: Optional[str] = None
 
@@ -2190,15 +2190,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     A user within the Kodexa platform
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     email: Optional[str] = None
     first_name: Optional[str] = Field(None, alias="firstName")
     last_name: Optional[str] = Field(None, alias="lastName")
@@ -2680,15 +2680,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     content_type: ContentType = Field(
         ..., alias="contentType", description="The type of content"
     )
@@ -2714,15 +2714,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     A list of the assignments to users for this document
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     user: User
 
 
@@ -2791,15 +2791,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     status: Optional[str] = Field(None, description="The status of the project")
     color: Optional[str] = None
     organization: Organization
@@ -2821,15 +2821,15 @@
 class Project(BaseModel):
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     organization: Optional[Organization] = None
     name: Optional[str] = None
     description: Optional[str] = None
@@ -3115,15 +3115,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     value: Optional[str] = None
     truncated: Optional[bool] = None
     data_exceptions: Optional[List[DataException]] = Field(
@@ -3160,15 +3160,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     A role that can be used to manage rights
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     name: str
     users: Optional[List[User]] = Field(default_factory=list)
     teams: Optional[List[Team]] = Field(default_factory=list)
@@ -3180,15 +3180,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     role: Optional[Role1] = None
     organization: Optional[Organization] = None
     user: Optional[User] = None
@@ -3610,15 +3610,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     A list of the content exceptions from the content objects
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     tag: Optional[str] = None
     message: Optional[str] = None
     exception_type: Optional[str] = Field(None, alias="exceptionType")
@@ -3689,15 +3689,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     description: Optional[str] = None
     targets: Optional[ExecutionTargets] = None
     session: Optional[Session] = None
@@ -3724,15 +3724,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     description: Optional[str] = None
     targets: Optional[ExecutionTargets] = None
     session: Optional[Session] = None
@@ -3860,15 +3860,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     A document family is the representation of a single piece of external content (ie. a PDF) and all the related document representations of that file
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     document_status: Optional[DocumentStatus] = Field(None, alias="documentStatus")
     summary: Optional[str] = None
 
@@ -3959,15 +3959,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     subscription: Optional[str] = None
     schedules: Optional[List[AssistantSchedule]] = Field(default_factory=list)
     project: Optional[Project] = None
@@ -4006,15 +4006,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     document_family: Optional[DocumentFamily] = Field(None, alias="documentFamily")
     data_exceptions: Optional[List[DataException]] = Field(
         default_factory=list,
@@ -4038,15 +4038,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     subscription: Optional[str] = None
     schedules: Optional[List[AssistantSchedule]] = Field(default_factory=list)
     project: Optional[Project] = None
@@ -4244,15 +4244,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     type: ExecutionEventType
     status: Optional[Status6] = None
     execution: Optional[Execution] = None
@@ -4472,15 +4472,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     A document family is the representation of a single peice of external content (ie. a PDF) and all the related document representations of that file
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     store: Optional[StoreMetadata] = None
     document_family: Optional[DocumentFamily] = Field(None, alias="documentFamily")
     container_type: Optional[str] = Field(
@@ -4556,15 +4556,15 @@
     """
     model_config = ConfigDict(
         populate_by_name=True,
         use_enum_values=True,
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     date_time: Optional[StandardDateTime] = Field(None, alias="dateTime")
     assistant: Optional[Assistant] = None
     event_detail: Optional[
@@ -4613,15 +4613,15 @@
         arbitrary_types_allowed=True,
         protected_namespaces=("model_config",),
     )
     """
     An audit event captures a data to a data structure or document
     """
 
-    id: Optional[str] = Field(None, description="The ID of the object")
+    id: Optional[str] = Field(None)
     uuid: Optional[str] = None
     change_sequence: Optional[int] = Field(None, alias="changeSequence")
     created_on: Optional[StandardDateTime] = Field(None, alias="createdOn")
     updated_on: Optional[StandardDateTime] = Field(None, alias="updatedOn")
     platform_user: Optional[User] = Field(None, alias="platformUser")
     document_family: Optional[DocumentFamily] = Field(None, alias="documentFamily")
     data_object: Optional[DataObject] = Field(None, alias="dataObject")
```

### Comparing `kodexa-7.0.8895840398/kodexa/model/persistence.py` & `kodexa-7.0.8897197016/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/pipeline/pipeline.py` & `kodexa-7.0.8897197016/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/platform/client.py` & `kodexa-7.0.8897197016/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -884,14 +884,52 @@
             Optional[OrganizationEndpoint]: The organization with the given slug, or None if no such organization exists.
         """
         organizations = self.list(filters=["slug: '" + slug + "'"])
         if organizations.number_of_elements == 0:
             return None
         return organizations.content[0]
 
+    def get_subscriptions(self, page: int = 1, page_size: int = 10) -> "PageProductSubscriptionEndpoint":
+        """
+        Get the subscriptions of the organization.
+
+        Returns:
+            The subscriptions of the organization.
+        """
+        url = f"/api/productSubscriptions"
+        params = {
+            filter: f"organization.id: '{self.organization.id}'",
+        }
+        response = self.client.get(url, params=params)
+
+        from kodexa.model.entities.product_subscription import PageProductSubscriptionEndpoint
+        return PageProductSubscriptionEndpoint.model_validate(response.json()).set_client(self.client)
+
+    def remove_subscription(self, subscription_id: str) -> None:
+        """
+        Remove a subscription from the organization.
+
+        Args:
+            subscription_id (str): The id of the subscription to remove.
+        """
+        url = f"/api/productSubscriptions/{subscription_id}"
+        self.client.delete(url)
+
+    def add_subscription(self, product: "Product") -> None:
+        """
+        Add a subscription to the organization.
+
+        Args:
+            product (Product): The product to subscribe to.
+        """
+        url = f"/api/productSubscriptions"
+        from kodexa.model.entities.product_subscription import ProductSubscription
+        new_product_subscription = ProductSubscription(organization=self.organization, product=product)
+        self.client.post(url, body=new_product_subscription.model_dump_json(by_alias=True))
+
 
 class PageEndpoint(ClientEndpoint):
     """
     Represents a page endpoint.
     """
 
     """
@@ -6180,14 +6218,16 @@
         self.workspaces = WorkspacesEndpoint(self)
         self.users = UsersEndpoint(self)
         self.memberships = MembershipsEndpoint(self)
         self.executions = ExecutionsEndpoint(self)
         self.channels = ChannelsEndpoint(self)
         self.assistants = AssistantsEndpoint(self)
         self.messages = MessagesEndpoint(self)
+        from kodexa.model.entities.product import ProductsEndpoint
+        self.products = ProductsEndpoint(self)
 
     @staticmethod
     def login(url, token):
         """
         A static method to login to the Kodexa platform.
 
         Args:
@@ -6729,14 +6769,16 @@
                             component_dict
                         ).set_client(self)
 
                     raise Exception("Unknown store type: " + store_type)
 
                 raise Exception("A store must have a storeType")
 
+            from kodexa.model.entities.product import ProductEndpoint
+            from kodexa.model.entities.product_subscription import ProductSubscriptionEndpoint
             known_components = {
                 "taxonomy": TaxonomyEndpoint,
                 "pipeline": PipelineEndpoint,
                 "action": ActionEndpoint,
                 "credential": CredentialDefinitionEndpoint,
                 "projectTemplate": ProjectTemplateEndpoint,
                 "modelRuntime": ModelRuntimeEndpoint,
@@ -6752,14 +6794,16 @@
                 "assistant": AssistantDefinitionEndpoint,
                 "exception": DataExceptionEndpoint,
                 "workspace": WorkspaceEndpoint,
                 "message": MessageEndpoint,
                 "prompt": PromptEndpoint,
                 "guidance": GuidanceSetEndpoint,
                 "channel": ChannelEndpoint,
+                "product": ProductEndpoint,
+                "productSubscription": ProductSubscriptionEndpoint,
             }
 
             if component_type in known_components:
                 return (
                     known_components[component_type]
                     .model_validate(component_dict)
                     .set_client(self)
```

### Comparing `kodexa-7.0.8895840398/kodexa/platform/interaction.py` & `kodexa-7.0.8897197016/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/platform/kodexa.py` & `kodexa-7.0.8897197016/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/selectors/ast.py` & `kodexa-7.0.8897197016/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/selectors/core.py` & `kodexa-7.0.8897197016/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/selectors/lexrules.py` & `kodexa-7.0.8897197016/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/selectors/lextab.py` & `kodexa-7.0.8897197016/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/selectors/parserules.py` & `kodexa-7.0.8897197016/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/selectors/parsetab.py` & `kodexa-7.0.8897197016/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/spatial/azure_models.py` & `kodexa-7.0.8897197016/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/spatial/bbox_common.py` & `kodexa-7.0.8897197016/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/spatial/table_form_common.py` & `kodexa-7.0.8897197016/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/steps/common.py` & `kodexa-7.0.8897197016/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/testing/test_components.py` & `kodexa-7.0.8897197016/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/kodexa/testing/test_utils.py` & `kodexa-7.0.8897197016/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8895840398/pyproject.toml` & `kodexa-7.0.8897197016/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.08895840398"
+version = "7.0.08897197016"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.8895840398/PKG-INFO` & `kodexa-7.0.8897197016/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.8895840398
+Version: 7.0.8897197016
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

