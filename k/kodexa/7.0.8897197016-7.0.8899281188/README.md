# Comparing `tmp/kodexa-7.0.8897197016.tar.gz` & `tmp/kodexa-7.0.8899281188.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.8897197016.tar", max compression
+gzip compressed data, was "kodexa-7.0.8899281188.tar", max compression
```

## Comparing `kodexa-7.0.8897197016.tar` & `kodexa-7.0.8899281188.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2024-04-30 15:09:26.303766 kodexa-7.0.8897197016/LICENSE
--rw-r--r--   0        0        0     2178 2024-04-30 15:09:26.303766 kodexa-7.0.8897197016/README.md
--rw-r--r--   0        0        0      957 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/base.py
--rw-r--r--   0        0        0        0 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/entities/__init__.py
--rw-r--r--   0        0        0     3526 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/entities/product.py
--rw-r--r--   0        0        0     3814 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/entities/product_subscription.py
--rw-r--r--   0        0        0   115561 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/model.py
--rw-r--r--   0        0        0   174318 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/objects.py
--rw-r--r--   0        0        0    62032 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   216867 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    34024 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-04-30 15:09:26.311766 kodexa-7.0.8897197016/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 15:09:26.315766 kodexa-7.0.8897197016/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1389 2024-04-30 15:09:40.991799 kodexa-7.0.8897197016/pyproject.toml
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8897197016/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 17:43:38.743521 kodexa-7.0.8899281188/LICENSE
+-rw-r--r--   0        0        0     2178 2024-04-30 17:43:38.743521 kodexa-7.0.8899281188/README.md
+-rw-r--r--   0        0        0      957 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/model/base.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/model/entities/__init__.py
+-rw-r--r--   0        0        0     3526 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/model/entities/product.py
+-rw-r--r--   0        0        0     3814 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/model/entities/product_subscription.py
+-rw-r--r--   0        0        0   115561 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/model/model.py
+-rw-r--r--   0        0        0   174318 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/model/objects.py
+-rw-r--r--   0        0        0    62032 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-04-30 17:43:38.747521 kodexa-7.0.8899281188/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   217016 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    34024 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 17:43:38.751521 kodexa-7.0.8899281188/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1389 2024-04-30 17:43:52.495581 kodexa-7.0.8899281188/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8899281188/PKG-INFO
```

### Comparing `kodexa-7.0.8897197016/LICENSE` & `kodexa-7.0.8899281188/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/README.md` & `kodexa-7.0.8899281188/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/__init__.py` & `kodexa-7.0.8899281188/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/assistant/assistant.py` & `kodexa-7.0.8899281188/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/connectors/connectors.py` & `kodexa-7.0.8899281188/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/model/__init__.py` & `kodexa-7.0.8899281188/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/model/base.py` & `kodexa-7.0.8899281188/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/model/entities/product.py` & `kodexa-7.0.8899281188/kodexa/model/entities/product.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/model/entities/product_subscription.py` & `kodexa-7.0.8899281188/kodexa/model/entities/product_subscription.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/model/model.py` & `kodexa-7.0.8899281188/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/model/objects.py` & `kodexa-7.0.8899281188/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/model/persistence.py` & `kodexa-7.0.8899281188/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/pipeline/pipeline.py` & `kodexa-7.0.8899281188/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/platform/client.py` & `kodexa-7.0.8899281188/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -884,52 +884,14 @@
             Optional[OrganizationEndpoint]: The organization with the given slug, or None if no such organization exists.
         """
         organizations = self.list(filters=["slug: '" + slug + "'"])
         if organizations.number_of_elements == 0:
             return None
         return organizations.content[0]
 
-    def get_subscriptions(self, page: int = 1, page_size: int = 10) -> "PageProductSubscriptionEndpoint":
-        """
-        Get the subscriptions of the organization.
-
-        Returns:
-            The subscriptions of the organization.
-        """
-        url = f"/api/productSubscriptions"
-        params = {
-            filter: f"organization.id: '{self.organization.id}'",
-        }
-        response = self.client.get(url, params=params)
-
-        from kodexa.model.entities.product_subscription import PageProductSubscriptionEndpoint
-        return PageProductSubscriptionEndpoint.model_validate(response.json()).set_client(self.client)
-
-    def remove_subscription(self, subscription_id: str) -> None:
-        """
-        Remove a subscription from the organization.
-
-        Args:
-            subscription_id (str): The id of the subscription to remove.
-        """
-        url = f"/api/productSubscriptions/{subscription_id}"
-        self.client.delete(url)
-
-    def add_subscription(self, product: "Product") -> None:
-        """
-        Add a subscription to the organization.
-
-        Args:
-            product (Product): The product to subscribe to.
-        """
-        url = f"/api/productSubscriptions"
-        from kodexa.model.entities.product_subscription import ProductSubscription
-        new_product_subscription = ProductSubscription(organization=self.organization, product=product)
-        self.client.post(url, body=new_product_subscription.model_dump_json(by_alias=True))
-
 
 class PageEndpoint(ClientEndpoint):
     """
     Represents a page endpoint.
     """
 
     """
@@ -1668,14 +1630,53 @@
         Returns:
             MarketplaceEndpoint: The marketplace endpoint of the organization.
         """
         url = f"/api/organizations/{self.id}/availableAssistants"
         response = self.client.get(url, params={"page": page, "pageSize": page_size, "query": query})
         return PageAssistantDefinitionEndpoint.model_validate(response.json()).set_client(self.client)
 
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
+        new_product_subscription = ProductSubscription(organization=self.detach(), product=product)
+        print(new_product_subscription.model_dump_json(by_alias=True))
+        self.client.post(url, body=json.loads(new_product_subscription.model_dump_json(by_alias=True)))
+
 
 class ComponentsEndpoint(ClientEndpoint):
     """
     Represents a components endpoint.
 
     Attributes:
         organization (OrganizationEndpoint): The organization endpoint that the components endpoint belongs to.
@@ -6123,17 +6124,18 @@
             document (Document): The document to extract data from.
 
         Returns:
             List[DataObject]: The extracted data objects.
         """
         response = self.client.post(
             "/api/extractionEngine/extract",
-            data={"taxonomyJson": taxonomy.model_dump_json()},
+            data={"taxonomyJson": taxonomy.model_dump_json(by_alias=True)},
             files={"document": document.to_kddb()},
         )
+        print(response.json())
         return [
             DataObject.model_validate(data_object) for data_object in response.json()
         ]
 
     def extract_data_objects_with_exceptions(
             self, taxonomy: Taxonomy, document: Document
     ) -> Dict:
@@ -6146,15 +6148,15 @@
 
         Returns:
             Dict: A dictionary containing the extracted data objects and any exceptions.
         """
         response = self.client.post(
             "/api/extractionEngine/extract",
             params="full",
-            data={"taxonomyJson": taxonomy.model_dump_json()},
+            data={"taxonomyJson": taxonomy.model_dump_json(by_alias=True)},
             files={"document": document.to_kddb()},
         )
         return {
             "dataObjects": [
                 DataObject.model_validate(data_object)
                 for data_object in response.json()["dataObjects"]
             ],
@@ -6177,15 +6179,15 @@
 
         Returns:
             str: The extracted data in the given format.
         """
         response = self.client.post(
             "/api/extractionEngine/extract",
             params={"format": format},
-            data={"taxonomyJson": taxonomy.model_dump_json()},
+            data={"taxonomyJson": taxonomy.model_dump_json(by_alias=True)},
             files={"document": document.to_kddb()},
         )
         return response.text
 
 
 class KodexaClient:
     """
```

### Comparing `kodexa-7.0.8897197016/kodexa/platform/interaction.py` & `kodexa-7.0.8899281188/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/platform/kodexa.py` & `kodexa-7.0.8899281188/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/selectors/ast.py` & `kodexa-7.0.8899281188/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/selectors/core.py` & `kodexa-7.0.8899281188/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/selectors/lexrules.py` & `kodexa-7.0.8899281188/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/selectors/lextab.py` & `kodexa-7.0.8899281188/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/selectors/parserules.py` & `kodexa-7.0.8899281188/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/selectors/parsetab.py` & `kodexa-7.0.8899281188/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/spatial/azure_models.py` & `kodexa-7.0.8899281188/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/spatial/bbox_common.py` & `kodexa-7.0.8899281188/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/spatial/table_form_common.py` & `kodexa-7.0.8899281188/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/steps/common.py` & `kodexa-7.0.8899281188/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/testing/test_components.py` & `kodexa-7.0.8899281188/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/kodexa/testing/test_utils.py` & `kodexa-7.0.8899281188/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8897197016/pyproject.toml` & `kodexa-7.0.8899281188/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.08897197016"
+version = "7.0.08899281188"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.8897197016/PKG-INFO` & `kodexa-7.0.8899281188/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.8897197016
+Version: 7.0.8899281188
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

