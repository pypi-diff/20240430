# Comparing `tmp/mms_client-1.5.0.tar.gz` & `tmp/mms_client-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_client-1.5.0.tar", max compression
+gzip compressed data, was "mms_client-1.5.1.tar", max compression
```

## Comparing `mms_client-1.5.0.tar` & `mms_client-1.5.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1211 2024-04-23 00:20:48.431840 mms_client-1.5.0/LICENSE
--rw-r--r--   0        0        0    14703 2024-04-23 00:20:48.431840 mms_client-1.5.0/README.md
--rw-r--r--   0        0        0     2913 2024-04-23 00:20:48.431840 mms_client-1.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/__init__.py
--rw-r--r--   0        0        0      676 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/client.py
--rw-r--r--   0        0        0        0 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/py.typed
--rw-r--r--   0        0        0    10702 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
--rw-r--r--   0        0        0     9894 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl
--rw-r--r--   0        0        0   109679 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/schemas/xsd/mi-market.xsd
--rw-r--r--   0        0        0    76166 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
--rw-r--r--   0        0        0    13276 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/schemas/xsd/mi-report.xsd
--rw-r--r--   0        0        0    69149 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/schemas/xsd/mpr.xsd
--rw-r--r--   0        0        0    31524 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/schemas/xsd/omi.xsd
--rw-r--r--   0        0        0        0 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/security/__init__.py
--rw-r--r--   0        0        0     1489 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/security/certs.py
--rw-r--r--   0        0        0     2149 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/security/crypto.py
--rw-r--r--   0        0        0        0 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/__init__.py
--rw-r--r--   0        0        0    25897 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/base.py
--rw-r--r--   0        0        0     7684 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/market.py
--rw-r--r--   0        0        0      626 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/omi.py
--rw-r--r--   0        0        0     3815 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/registration.py
--rw-r--r--   0        0        0      642 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/report.py
--rw-r--r--   0        0        0        0 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/__init__.py
--rw-r--r--   0        0        0    14139 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/award.py
--rw-r--r--   0        0        0     9710 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/base.py
--rw-r--r--   0        0        0     1629 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/enums.py
--rw-r--r--   0        0        0    14785 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/fields.py
--rw-r--r--   0        0        0     2706 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/market.py
--rw-r--r--   0        0        0     6791 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/offer.py
--rw-r--r--   0        0        0     1381 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/registration.py
--rw-r--r--   0        0        0    65974 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/resource.py
--rw-r--r--   0        0        0     4399 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/transport.py
--rw-r--r--   0        0        0        0 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/utils/__init__.py
--rw-r--r--   0        0        0     1797 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/utils/auditing.py
--rw-r--r--   0        0        0     2579 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/utils/errors.py
--rw-r--r--   0        0        0    29638 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/utils/serialization.py
--rw-r--r--   0        0        0    10033 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/utils/web.py
--rw-r--r--   0        0        0    15987 1970-01-01 00:00:00.000000 mms_client-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-30 01:57:17.676666 mms_client-1.5.1/LICENSE
+-rw-r--r--   0        0        0    14703 2024-04-30 01:57:17.676666 mms_client-1.5.1/README.md
+-rw-r--r--   0        0        0     2913 2024-04-30 01:57:17.680666 mms_client-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/__init__.py
+-rw-r--r--   0        0        0      676 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/client.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/py.typed
+-rw-r--r--   0        0        0    10702 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
+-rw-r--r--   0        0        0     9894 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/wsdl/omi-web-service.wsdl
+-rw-r--r--   0        0        0   109679 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/xsd/mi-market.xsd
+-rw-r--r--   0        0        0    76166 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
+-rw-r--r--   0        0        0    13276 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/xsd/mi-report.xsd
+-rw-r--r--   0        0        0    69149 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/xsd/mpr.xsd
+-rw-r--r--   0        0        0    31524 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/xsd/omi.xsd
+-rw-r--r--   0        0        0        0 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/security/__init__.py
+-rw-r--r--   0        0        0     1489 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/security/certs.py
+-rw-r--r--   0        0        0     2149 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/security/crypto.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/__init__.py
+-rw-r--r--   0        0        0    25897 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/base.py
+-rw-r--r--   0        0        0     7684 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/market.py
+-rw-r--r--   0        0        0      626 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/omi.py
+-rw-r--r--   0        0        0     3815 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/registration.py
+-rw-r--r--   0        0        0      642 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/report.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/types/__init__.py
+-rw-r--r--   0        0        0    14139 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/types/award.py
+-rw-r--r--   0        0        0     9710 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/types/base.py
+-rw-r--r--   0        0        0     1629 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/types/enums.py
+-rw-r--r--   0        0        0    14785 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/fields.py
+-rw-r--r--   0        0        0     2706 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/market.py
+-rw-r--r--   0        0        0     6791 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/offer.py
+-rw-r--r--   0        0        0     1381 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/registration.py
+-rw-r--r--   0        0        0    65974 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/resource.py
+-rw-r--r--   0        0        0     4399 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/transport.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/utils/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/utils/auditing.py
+-rw-r--r--   0        0        0     2579 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/utils/errors.py
+-rw-r--r--   0        0        0    29638 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/utils/serialization.py
+-rw-r--r--   0        0        0    10156 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/utils/web.py
+-rw-r--r--   0        0        0    15987 1970-01-01 00:00:00.000000 mms_client-1.5.1/PKG-INFO
```

### Comparing `mms_client-1.5.0/LICENSE` & `mms_client-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/README.md` & `mms_client-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/pyproject.toml` & `mms_client-1.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mms_client"
-version = "v1.5.0"
+version = "v1.5.1"
 description = "API client for accessing the MMS"
 authors = ["Ryan Wood <ryan.wood@electroroute.co.jp>"]
 readme = "README.md"
 packages = [{ include = "mms_client", from = "src" }]
 homepage = "https://github.com/ElectroRoute-Japan/mms-client"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `mms_client-1.5.0/src/mms_client/client.py` & `mms_client-1.5.1/src/mms_client/client.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl` & `mms_client-1.5.1/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl` & `mms_client-1.5.1/src/mms_client/schemas/wsdl/omi-web-service.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/schemas/xsd/mi-market.xsd` & `mms_client-1.5.1/src/mms_client/schemas/xsd/mi-market.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd` & `mms_client-1.5.1/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/schemas/xsd/mi-report.xsd` & `mms_client-1.5.1/src/mms_client/schemas/xsd/mi-report.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/schemas/xsd/mpr.xsd` & `mms_client-1.5.1/src/mms_client/schemas/xsd/mpr.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/schemas/xsd/omi.xsd` & `mms_client-1.5.1/src/mms_client/schemas/xsd/omi.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/security/certs.py` & `mms_client-1.5.1/src/mms_client/security/certs.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/security/crypto.py` & `mms_client-1.5.1/src/mms_client/security/crypto.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/services/base.py` & `mms_client-1.5.1/src/mms_client/services/base.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/services/market.py` & `mms_client-1.5.1/src/mms_client/services/market.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/services/omi.py` & `mms_client-1.5.1/src/mms_client/services/omi.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/services/registration.py` & `mms_client-1.5.1/src/mms_client/services/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/services/report.py` & `mms_client-1.5.1/src/mms_client/services/report.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/types/award.py` & `mms_client-1.5.1/src/mms_client/types/award.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/types/base.py` & `mms_client-1.5.1/src/mms_client/types/base.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/types/enums.py` & `mms_client-1.5.1/src/mms_client/types/enums.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/types/fields.py` & `mms_client-1.5.1/src/mms_client/types/fields.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/types/market.py` & `mms_client-1.5.1/src/mms_client/types/market.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/types/offer.py` & `mms_client-1.5.1/src/mms_client/types/offer.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/types/registration.py` & `mms_client-1.5.1/src/mms_client/types/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/types/resource.py` & `mms_client-1.5.1/src/mms_client/types/resource.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/types/transport.py` & `mms_client-1.5.1/src/mms_client/types/transport.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/utils/auditing.py` & `mms_client-1.5.1/src/mms_client/utils/auditing.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,56 +3,59 @@
 from abc import ABC
 from abc import abstractmethod
 from logging import getLogger
 
 from lxml.etree import _Element as Element
 from lxml.etree import tostring
 from zeep import Plugin
+from zeep.wsdl.definitions import Operation
 
 # Set the default logger for the MMS client
 logger = getLogger(__name__)
 
 
 class AuditPlugin(ABC, Plugin):
     """Base class for audit plugins."""
 
-    def egress(self, envelope: Element, http_headers: dict, operation, binding_options):
+    def egress(self, envelope: Element, http_headers: dict, operation: Operation, binding_options):
         """Handle the MMS request before it is sent.
 
         Arguments are the same as in the egress method of the Plugin class.
 
         Returns:
         lxml.etree.Element: The XML message to send.
         dict:               The HTTP headers to send.
         """
         data = tostring(envelope, encoding="UTF-8", xml_declaration=True)
-        self.audit_request(data)
+        self.audit_request(operation.name, data)
         return envelope, http_headers
 
-    def ingress(self, envelope: Element, http_headers: dict, operation):
+    def ingress(self, envelope: Element, http_headers: dict, operation: Operation):
         """Handle the MMS response before it is processed.
 
         Arguments are the same as in the ingress method of the Plugin class.
 
         Returns:
         lxml.etree.Element: The XML message to process.
         dict:               The HTTP headers to process.
         """
         data = tostring(envelope, encoding="UTF-8", xml_declaration=True)
-        self.audit_response(data)
+        self.audit_response(operation.name, data)
         return envelope, http_headers
 
     @abstractmethod
-    def audit_request(self, mms_request: bytes) -> None:
+    def audit_request(self, operation: str, mms_request: bytes) -> None:
         """Audit an MMS request.
 
         Arguments:
+        operation (str):        The SOAP operation being called.
         mms_request (bytes):    The MMS request XML to audit.
         """
 
     @abstractmethod
-    def audit_response(self, mms_response: bytes) -> None:
+    def audit_response(self, operation: str, mms_response: bytes) -> None:
         """Audit an MMS response.
 
         Arguments:
+        operation (str):        The SOAP operation being called.
         mms_response (bytes):   The MMS response XML to audit.
         """
```

### Comparing `mms_client-1.5.0/src/mms_client/utils/errors.py` & `mms_client-1.5.1/src/mms_client/utils/errors.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/utils/serialization.py` & `mms_client-1.5.1/src/mms_client/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.0/src/mms_client/utils/web.py` & `mms_client-1.5.1/src/mms_client/utils/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,21 @@
             transport=Transport(cache=SqliteCache() if cache else None, session=sess),
             plugins=plugins,
         )
         self._create_service()
 
     @on_exception(expo, TransportError, max_tries=3, giveup=fatal_code, logger=logger)  # type: ignore[arg-type]
     def submit(self, req: MmsRequest) -> MmsResponse:
-        """Submit the given request to the MMS server and return the response."""
+        """Submit the given request to the MMS server and return the response.
+
+        Arguments:
+        req (MmsRequest):   The MMS request to submit.
+
+        Returns:    The MMS response.
+        """
         try:
             logger.debug(f"Submitting MMS request request to {self._interface.name} service")
 
             # Submit the request to the MMS server and retrieve the response
             resp: CompoundValue = self._service["submitAttachment"](**req.to_arguments())
 
             # Validate the response and return it
```

### Comparing `mms_client-1.5.0/PKG-INFO` & `mms_client-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mms-client
-Version: 1.5.0
+Version: 1.5.1
 Summary: API client for accessing the MMS
 Home-page: https://github.com/ElectroRoute-Japan/mms-client
 Author: Ryan Wood
 Author-email: ryan.wood@electroroute.co.jp
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic :: 2
```

