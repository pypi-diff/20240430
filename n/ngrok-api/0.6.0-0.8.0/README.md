# Comparing `tmp/ngrok-api-0.6.0.tar.gz` & `tmp/ngrok-api-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngrok-api-0.6.0.tar", last modified: Thu Mar 10 19:38:37 2022, max compression
+gzip compressed data, was "ngrok-api-0.8.0.tar", last modified: Mon Apr 11 19:33:00 2022, max compression
```

## Comparing `ngrok-api-0.6.0.tar` & `ngrok-api-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 ngrok     (1000) ngrok     (1000)        0 2022-03-10 19:38:37.884343 ngrok-api-0.6.0/
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)     1051 2022-03-10 19:37:51.000000 ngrok-api-0.6.0/LICENSE
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)     1425 2022-03-10 19:38:37.884343 ngrok-api-0.6.0/PKG-INFO
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)      922 2022-03-10 19:37:51.000000 ngrok-api-0.6.0/README.md
-drwxr-xr-x   0 ngrok     (1000) ngrok     (1000)        0 2022-03-10 19:38:37.884343 ngrok-api-0.6.0/ngrok/
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)       90 2022-03-10 19:38:22.000000 ngrok-api-0.6.0/ngrok/__init__.py
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)    10335 2022-03-10 19:38:06.000000 ngrok-api-0.6.0/ngrok/client.py
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)   158385 2022-03-10 19:38:10.000000 ngrok-api-0.6.0/ngrok/datatypes.py
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)     1244 2022-03-10 19:38:06.000000 ngrok-api-0.6.0/ngrok/error.py
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)     4474 2022-03-10 19:38:06.000000 ngrok-api-0.6.0/ngrok/http_client.py
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)      699 2022-03-10 19:37:51.000000 ngrok-api-0.6.0/ngrok/iterator.py
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)   146029 2022-03-10 19:38:08.000000 ngrok-api-0.6.0/ngrok/services.py
-drwxr-xr-x   0 ngrok     (1000) ngrok     (1000)        0 2022-03-10 19:38:37.884343 ngrok-api-0.6.0/ngrok_api.egg-info/
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)     1425 2022-03-10 19:38:37.000000 ngrok-api-0.6.0/ngrok_api.egg-info/PKG-INFO
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)      330 2022-03-10 19:38:37.000000 ngrok-api-0.6.0/ngrok_api.egg-info/SOURCES.txt
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)        1 2022-03-10 19:38:37.000000 ngrok-api-0.6.0/ngrok_api.egg-info/dependency_links.txt
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)      152 2022-03-10 19:38:37.000000 ngrok-api-0.6.0/ngrok_api.egg-info/requires.txt
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)        6 2022-03-10 19:38:37.000000 ngrok-api-0.6.0/ngrok_api.egg-info/top_level.txt
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)      104 2022-03-10 19:37:51.000000 ngrok-api-0.6.0/pyproject.toml
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)       38 2022-03-10 19:38:37.884343 ngrok-api-0.6.0/setup.cfg
--rw-r--r--   0 ngrok     (1000) ngrok     (1000)     1083 2022-03-10 19:38:22.000000 ngrok-api-0.6.0/setup.py
+drwxr-xr-x   0 ngrok     (1000) ngrok     (1000)        0 2022-04-11 19:33:00.875235 ngrok-api-0.8.0/
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)     1051 2022-04-11 19:32:09.000000 ngrok-api-0.8.0/LICENSE
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)     1661 2022-04-11 19:33:00.875235 ngrok-api-0.8.0/PKG-INFO
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)     1158 2022-04-11 19:32:09.000000 ngrok-api-0.8.0/README.md
+drwxr-xr-x   0 ngrok     (1000) ngrok     (1000)        0 2022-04-11 19:33:00.875235 ngrok-api-0.8.0/ngrok/
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)       90 2022-04-11 19:32:42.000000 ngrok-api-0.8.0/ngrok/__init__.py
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)    10530 2022-04-11 19:32:26.000000 ngrok-api-0.8.0/ngrok/client.py
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)   158760 2022-04-11 19:32:29.000000 ngrok-api-0.8.0/ngrok/datatypes.py
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)     1244 2022-04-11 19:32:26.000000 ngrok-api-0.8.0/ngrok/error.py
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)     4474 2022-04-11 19:32:26.000000 ngrok-api-0.8.0/ngrok/http_client.py
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)      699 2022-04-11 19:32:09.000000 ngrok-api-0.8.0/ngrok/iterator.py
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)   146720 2022-04-11 19:32:28.000000 ngrok-api-0.8.0/ngrok/services.py
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)      141 2022-04-11 19:32:26.000000 ngrok-api-0.8.0/ngrok/utils.py
+drwxr-xr-x   0 ngrok     (1000) ngrok     (1000)        0 2022-04-11 19:33:00.875235 ngrok-api-0.8.0/ngrok_api.egg-info/
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)     1661 2022-04-11 19:33:00.000000 ngrok-api-0.8.0/ngrok_api.egg-info/PKG-INFO
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)      345 2022-04-11 19:33:00.000000 ngrok-api-0.8.0/ngrok_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)        1 2022-04-11 19:33:00.000000 ngrok-api-0.8.0/ngrok_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)      179 2022-04-11 19:33:00.000000 ngrok-api-0.8.0/ngrok_api.egg-info/requires.txt
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)        6 2022-04-11 19:33:00.000000 ngrok-api-0.8.0/ngrok_api.egg-info/top_level.txt
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)      104 2022-04-11 19:32:09.000000 ngrok-api-0.8.0/pyproject.toml
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)       38 2022-04-11 19:33:00.875235 ngrok-api-0.8.0/setup.cfg
+-rw-r--r--   0 ngrok     (1000) ngrok     (1000)     1294 2022-04-11 19:32:42.000000 ngrok-api-0.8.0/setup.py
```

### Comparing `ngrok-api-0.6.0/LICENSE` & `ngrok-api-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ngrok-api-0.6.0/PKG-INFO` & `ngrok-api-0.8.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngrok-api
-Version: 0.6.0
+Version: 0.8.0
 Summary: ngrok HTTP API client library
 Home-page: https://github.com/ngrok/ngrok-api-python
 Author: Alan Shreve
 Author-email: alan@ngrok.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,21 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tox
 Provides-Extra: doc
 License-File: LICENSE
 
+# Unstable
+
+This library is currently unstable. We know of rough edges
+and are working to bring it to parity with our other API client
+libraries. Please feel free to try it out and let us know if you find
+it useful!
+
 # ngrok API client library for Python
 
 This library wraps the [ngrok HTTP API](https://ngrok.com/docs/api) to make it
 easier to consume in Python.
 
 ## Installation
 
@@ -34,19 +41,19 @@
 ## Quickstart
 
 Please consult the [documentation](https://python-api.docs.ngrok.com) for additional examples.
 
     import ngrok
 
     # construct the api client
-    ng = ngrok.Client("<API KEY>")
+    client = ngrok.Client("<API KEY>")
 
     # list all online tunnels
-    for t in ng.tunnels.list():
+    for t in client.tunnels.list():
         print(t)
 
-    # create an ip policy the allows traffic from some subnets
-    policy = ng.ip_policies.create(action="allow")
+    # create an ip policy that allows traffic from some subnets
+    policy = client.ip_policies.create()
     for cidr in ["24.0.0.0/8", "12.0.0.0/8"]:
-        ng.ip_policy_rules.create(cidr=cidr, ip_policy_id=policy.id)
+        client.ip_policy_rules.create(cidr=cidr, ip_policy_id=policy.id, action="allow")
```

### Comparing `ngrok-api-0.6.0/README.md` & `ngrok-api-0.8.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# Unstable
+
+This library is currently unstable. We know of rough edges
+and are working to bring it to parity with our other API client
+libraries. Please feel free to try it out and let us know if you find
+it useful!
+
 # ngrok API client library for Python
 
 This library wraps the [ngrok HTTP API](https://ngrok.com/docs/api) to make it
 easier to consume in Python.
 
 ## Installation
 
@@ -16,17 +23,17 @@
 ## Quickstart
 
 Please consult the [documentation](https://python-api.docs.ngrok.com) for additional examples.
 
     import ngrok
 
     # construct the api client
-    ng = ngrok.Client("<API KEY>")
+    client = ngrok.Client("<API KEY>")
 
     # list all online tunnels
-    for t in ng.tunnels.list():
+    for t in client.tunnels.list():
         print(t)
 
-    # create an ip policy the allows traffic from some subnets
-    policy = ng.ip_policies.create(action="allow")
+    # create an ip policy that allows traffic from some subnets
+    policy = client.ip_policies.create()
     for cidr in ["24.0.0.0/8", "12.0.0.0/8"]:
-        ng.ip_policy_rules.create(cidr=cidr, ip_policy_id=policy.id)
+        client.ip_policy_rules.create(cidr=cidr, ip_policy_id=policy.id, action="allow")
```

### Comparing `ngrok-api-0.6.0/ngrok/client.py` & `ngrok-api-0.8.0/ngrok/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,65 +150,71 @@
         agent tunnel session or an SSH reverse tunnel session."""
         return TunnelsClient(self)
 
     @property
     def backends(self):
         ns = collections.namedtuple(
             "Namespace",
-            "failover",
-            "http_response",
-            "tunnel_group",
-            "weighted",
+            [
+                "failover",
+                "http_response",
+                "tunnel_group",
+                "weighted",
+            ],
         )
         return ns(
             failover=FailoverBackendsClient(self),
             http_response=HTTPResponseBackendsClient(self),
             tunnel_group=TunnelGroupBackendsClient(self),
             weighted=WeightedBackendsClient(self),
         )
 
     @property
     def edges(self):
         ns = collections.namedtuple(
             "Namespace",
-            "https_routes",
-            "https",
-            "tcp",
-            "tls",
+            [
+                "https_routes",
+                "https",
+                "tcp",
+                "tls",
+            ],
         )
         return ns(
             https_routes=EdgesHTTPSRoutesClient(self),
             https=EdgesHTTPSClient(self),
             tcp=EdgesTCPClient(self),
             tls=EdgesTLSClient(self),
         )
 
     @property
     def edge_modules(self):
         ns = collections.namedtuple(
             "Namespace",
-            "https_edge_mutual_tls",
-            "https_edge_tls_termination",
-            "https_edge_route_backend",
-            "https_edge_route_ip_restriction",
-            "https_edge_route_request_headers",
-            "https_edge_route_response_headers",
-            "https_edge_route_compression",
-            "https_edge_route_circuit_breaker",
-            "https_edge_route_webhook_verification",
-            "https_edge_route_oauth",
-            "https_edge_route_saml",
-            "https_edge_route_oidc",
-            "https_edge_route_websocket_tcp_converter",
-            "tcp_edge_backend",
-            "tcp_edge_ip_restriction",
-            "tls_edge_backend",
-            "tls_edge_ip_restriction",
-            "tls_edge_mutual_tls",
-            "tls_edge_tls_termination",
+            [
+                "https_edge_mutual_tls",
+                "https_edge_tls_termination",
+                "https_edge_route_backend",
+                "https_edge_route_ip_restriction",
+                "https_edge_route_request_headers",
+                "https_edge_route_response_headers",
+                "https_edge_route_compression",
+                "https_edge_route_circuit_breaker",
+                "https_edge_route_webhook_verification",
+                "https_edge_route_oauth",
+                "https_edge_route_saml",
+                "https_edge_route_oidc",
+                "https_edge_route_websocket_tcp_converter",
+                "tcp_edge_backend",
+                "tcp_edge_ip_restriction",
+                "tls_edge_backend",
+                "tls_edge_ip_restriction",
+                "tls_edge_mutual_tls",
+                "tls_edge_tls_termination",
+            ],
         )
         return ns(
             https_edge_mutual_tls=HTTPSEdgeMutualTLSModuleClient(self),
             https_edge_tls_termination=HTTPSEdgeTLSTerminationModuleClient(self),
             https_edge_route_backend=EdgeRouteBackendModuleClient(self),
             https_edge_route_ip_restriction=EdgeRouteIPRestrictionModuleClient(self),
             https_edge_route_request_headers=EdgeRouteRequestHeadersModuleClient(self),
```

### Comparing `ngrok-api-0.6.0/ngrok/datatypes.py` & `ngrok-api-0.8.0/ngrok/datatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
 class AbuseReport(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["hostnames"] = (
             [AbuseReportHostname(client, x) for x in props["hostnames"]]
-            if props["hostnames"] is not None
-            else None
+            if props.get("hostnames") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -183,16 +183,16 @@
 
 class AgentIngressList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["ingresses"] = (
             [AgentIngress(client, x) for x in props["ingresses"]]
-            if props["ingresses"] is not None
-            else None
+            if props.get("ingresses") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -284,16 +284,16 @@
 
 class APIKeyList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["keys"] = (
             [APIKey(client, x) for x in props["keys"]]
-            if props["keys"] is not None
-            else None
+            if props.get("keys") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -333,25 +333,25 @@
             return "<FailoverBackend {} {}>".format(self.id, repr(self._props))
         else:
             return "<FailoverBackend {}>".format(repr(self._props))
 
     def delete(
         self,
     ):
-        self._client.failover_backends.delete(
+        self._client.backends.failover.delete(
             id=self.id,
         )
 
     def update(
         self,
         description: str = None,
         metadata: str = None,
         backends: Sequence[str] = [],
     ):
-        self._client.failover_backends.update(
+        self._client.backends.failover.update(
             id=self.id,
             description=description,
             metadata=metadata,
             backends=backends,
         )
 
     @property
@@ -387,16 +387,16 @@
 
 class FailoverBackendList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["backends"] = (
             [FailoverBackend(client, x) for x in props["backends"]]
-            if props["backends"] is not None
-            else None
+            if props.get("backends") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -436,27 +436,27 @@
             return "<HTTPResponseBackend {} {}>".format(self.id, repr(self._props))
         else:
             return "<HTTPResponseBackend {}>".format(repr(self._props))
 
     def delete(
         self,
     ):
-        self._client.http_response_backends.delete(
+        self._client.backends.http_response.delete(
             id=self.id,
         )
 
     def update(
         self,
         description: str = None,
         metadata: str = None,
         body: str = None,
         headers: Mapping[str, str] = None,
         status_code: int = None,
     ):
-        self._client.http_response_backends.update(
+        self._client.backends.http_response.update(
             id=self.id,
             description=description,
             metadata=metadata,
             body=body,
             headers=headers,
             status_code=status_code,
         )
@@ -503,16 +503,16 @@
 
 class HTTPResponseBackendList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["backends"] = (
             [HTTPResponseBackend(client, x) for x in props["backends"]]
-            if props["backends"] is not None
-            else None
+            if props.get("backends") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -538,41 +538,41 @@
 
 class TunnelGroupBackend(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["tunnels"] = (
             [Ref(client, x) for x in props["tunnels"]]
-            if props["tunnels"] is not None
-            else None
+            if props.get("tunnels") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
             return "<TunnelGroupBackend {} {}>".format(self.id, repr(self._props))
         else:
             return "<TunnelGroupBackend {}>".format(repr(self._props))
 
     def delete(
         self,
     ):
-        self._client.tunnel_group_backends.delete(
+        self._client.backends.tunnel_group.delete(
             id=self.id,
         )
 
     def update(
         self,
         description: str = None,
         metadata: str = None,
         labels: Mapping[str, str] = {},
     ):
-        self._client.tunnel_group_backends.update(
+        self._client.backends.tunnel_group.update(
             id=self.id,
             description=description,
             metadata=metadata,
             labels=labels,
         )
 
     @property
@@ -613,16 +613,16 @@
 
 class TunnelGroupBackendList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["backends"] = (
             [TunnelGroupBackend(client, x) for x in props["backends"]]
-            if props["backends"] is not None
-            else None
+            if props.get("backends") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -662,25 +662,25 @@
             return "<WeightedBackend {} {}>".format(self.id, repr(self._props))
         else:
             return "<WeightedBackend {}>".format(repr(self._props))
 
     def delete(
         self,
     ):
-        self._client.weighted_backends.delete(
+        self._client.backends.weighted.delete(
             id=self.id,
         )
 
     def update(
         self,
         description: str = None,
         metadata: str = None,
         backends: Mapping[str, int] = {},
     ):
-        self._client.weighted_backends.update(
+        self._client.backends.weighted.update(
             id=self.id,
             description=description,
             metadata=metadata,
             backends=backends,
         )
 
     @property
@@ -706,26 +706,26 @@
     @property
     def metadata(self) -> str:
         """arbitrary user-defined machine-readable data of this backend. Optional"""
         return self._props["metadata"]
 
     @property
     def backends(self) -> Mapping[str, int]:
-        """the ids of the child backends to their weights (0-10000)"""
+        """the ids of the child backends to their weights [0-10000]"""
         return self._props["backends"]
 
 
 class WeightedBackendList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["backends"] = (
             [WeightedBackend(client, x) for x in props["backends"]]
-            if props["backends"] is not None
-            else None
+            if props.get("backends") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -842,16 +842,16 @@
 
 class CertificateAuthorityList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["certificate_authorities"] = (
             [CertificateAuthority(client, x) for x in props["certificate_authorities"]]
-            if props["certificate_authorities"] is not None
-            else None
+            if props.get("certificate_authorities") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -935,31 +935,31 @@
     @property
     def metadata(self) -> str:
         """arbitrary user-defined machine-readable data of this credential. Optional, max 4096 bytes."""
         return self._props["metadata"]
 
     @property
     def token(self) -> str:
-        """the credential's authtoken that can be used to authenticate an ngrok client. **This value is only available one time, on the API response from credential creation, otherwise it is null.**"""
+        """the credential's authtoken that can be used to authenticate an ngrok agent. **This value is only available one time, on the API response from credential creation, otherwise it is null.**"""
         return self._props["token"]
 
     @property
     def acl(self) -> Sequence[str]:
         """optional list of ACL rules. If unspecified, the credential will have no restrictions. The only allowed ACL rule at this time is the ``bind`` rule. The ``bind`` rule allows the caller to restrict what domains and addresses the token is allowed to bind. For example, to allow the token to open a tunnel on example.ngrok.io your ACL would include the rule ``bind:example.ngrok.io``. Bind rules may specify a leading wildcard to match multiple domains with a common suffix. For example, you may specify a rule of ``bind:*.example.com`` which will allow ``x.example.com``, ``y.example.com``, ``*.example.com``, etc. A rule of ``'*'`` is equivalent to no acl at all and will explicitly permit all actions."""
         return self._props["acl"]
 
 
 class CredentialList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["credentials"] = (
             [Credential(client, x) for x in props["credentials"]]
-            if props["credentials"] is not None
-            else None
+            if props.get("credentials") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -1040,16 +1040,16 @@
 
 class EndpointMutualTLS(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["certificate_authorities"] = (
             [Ref(client, x) for x in props["certificate_authorities"]]
-            if props["certificate_authorities"] is not None
-            else None
+            if props.get("certificate_authorities") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -1085,15 +1085,15 @@
     @property
     def enabled(self) -> bool:
         """``true`` if the module will be applied to traffic, ``false`` to disable. default ``true`` if unspecified"""
         return self._props["enabled"]
 
     @property
     def certificate_authority_ids(self) -> Sequence[str]:
-        """list of certificate authorities that will be used to validate the TLS client certificate presnted by the initiatiator of the TLS connection"""
+        """list of certificate authorities that will be used to validate the TLS client certificate presented by the initiator of the TLS connection"""
         return self._props["certificate_authority_ids"]
 
 
 class EndpointTLSTermination(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
@@ -1212,16 +1212,16 @@
 
 class EndpointIPPolicy(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["ip_policies"] = (
             [Ref(client, x) for x in props["ip_policies"]]
-            if props["ip_policies"] is not None
-            else None
+            if props.get("ip_policies") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -1311,15 +1311,15 @@
 
 class EndpointOAuth(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["provider"] = (
             EndpointOAuthProvider(client, props["provider"])
-            if props["provider"] is not None
+            if props.get("provider") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -1366,30 +1366,30 @@
 
 class EndpointOAuthProvider(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["github"] = (
             EndpointOAuthGitHub(client, props["github"])
-            if props["github"] is not None
+            if props.get("github") is not None
             else None
         )
         self._props["facebook"] = (
             EndpointOAuthFacebook(client, props["facebook"])
-            if props["facebook"] is not None
+            if props.get("facebook") is not None
             else None
         )
         self._props["microsoft"] = (
             EndpointOAuthMicrosoft(client, props["microsoft"])
-            if props["microsoft"] is not None
+            if props.get("microsoft") is not None
             else None
         )
         self._props["google"] = (
             EndpointOAuthGoogle(client, props["google"])
-            if props["google"] is not None
+            if props.get("google") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -1805,15 +1805,15 @@
 
 
 class EndpointBackend(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["backend"] = (
-            Ref(client, props["backend"]) if props["backend"] is not None else None
+            Ref(client, props["backend"]) if props.get("backend") is not None else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -1881,61 +1881,65 @@
 
 class HTTPSEdgeRoute(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["backend"] = (
             EndpointBackend(client, props["backend"])
-            if props["backend"] is not None
+            if props.get("backend") is not None
             else None
         )
         self._props["ip_restriction"] = (
             EndpointIPPolicy(client, props["ip_restriction"])
-            if props["ip_restriction"] is not None
+            if props.get("ip_restriction") is not None
             else None
         )
         self._props["circuit_breaker"] = (
             EndpointCircuitBreaker(client, props["circuit_breaker"])
-            if props["circuit_breaker"] is not None
+            if props.get("circuit_breaker") is not None
             else None
         )
         self._props["compression"] = (
             EndpointCompression(client, props["compression"])
-            if props["compression"] is not None
+            if props.get("compression") is not None
             else None
         )
         self._props["request_headers"] = (
             EndpointRequestHeaders(client, props["request_headers"])
-            if props["request_headers"] is not None
+            if props.get("request_headers") is not None
             else None
         )
         self._props["response_headers"] = (
             EndpointResponseHeaders(client, props["response_headers"])
-            if props["response_headers"] is not None
+            if props.get("response_headers") is not None
             else None
         )
         self._props["webhook_verification"] = (
             EndpointWebhookValidation(client, props["webhook_verification"])
-            if props["webhook_verification"] is not None
+            if props.get("webhook_verification") is not None
             else None
         )
         self._props["oauth"] = (
             EndpointOAuth(client, props["oauth"])
-            if props["oauth"] is not None
+            if props.get("oauth") is not None
             else None
         )
         self._props["saml"] = (
-            EndpointSAML(client, props["saml"]) if props["saml"] is not None else None
+            EndpointSAML(client, props["saml"])
+            if props.get("saml") is not None
+            else None
         )
         self._props["oidc"] = (
-            EndpointOIDC(client, props["oidc"]) if props["oidc"] is not None else None
+            EndpointOIDC(client, props["oidc"])
+            if props.get("oidc") is not None
+            else None
         )
         self._props["websocket_tcp_converter"] = (
             EndpointWebsocketTCPConverter(client, props["websocket_tcp_converter"])
-            if props["websocket_tcp_converter"] is not None
+            if props.get("websocket_tcp_converter") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -1958,15 +1962,15 @@
         response_headers: EndpointResponseHeaders = None,
         webhook_verification: EndpointWebhookValidation = None,
         oauth: EndpointOAuth = None,
         saml: EndpointSAMLMutate = None,
         oidc: EndpointOIDC = None,
         websocket_tcp_converter: EndpointWebsocketTCPConverter = None,
     ):
-        self._client.edges_https_routes.update(
+        self._client.edges.https_routes.update(
             edge_id=self.edge_id,
             id=self.id,
             match_type=match_type,
             match=match,
             description=description,
             metadata=metadata,
             backend=backend,
@@ -1981,15 +1985,15 @@
             oidc=oidc,
             websocket_tcp_converter=websocket_tcp_converter,
         )
 
     def delete(
         self,
     ):
-        self._client.edges_https_routes.delete(
+        self._client.edges.https_routes.delete(
             edge_id=self.edge_id,
             id=self.id,
         )
 
     @property
     def edge_id(self) -> str:
         """unique identifier of this edge"""
@@ -2088,16 +2092,16 @@
 
 class HTTPSEdgeList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["https_edges"] = (
             [HTTPSEdge(client, x) for x in props["https_edges"]]
-            if props["https_edges"] is not None
-            else None
+            if props.get("https_edges") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -2126,26 +2130,26 @@
 
 class HTTPSEdge(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["mutual_tls"] = (
             EndpointMutualTLS(client, props["mutual_tls"])
-            if props["mutual_tls"] is not None
+            if props.get("mutual_tls") is not None
             else None
         )
         self._props["tls_termination"] = (
             EndpointTLSTermination(client, props["tls_termination"])
-            if props["tls_termination"] is not None
+            if props.get("tls_termination") is not None
             else None
         )
         self._props["routes"] = (
             [HTTPSEdgeRoute(client, x) for x in props["routes"]]
-            if props["routes"] is not None
-            else None
+            if props.get("routes") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -2157,27 +2161,27 @@
         self,
         description: str = None,
         metadata: str = None,
         hostports: Sequence[str] = None,
         mutual_tls: EndpointMutualTLSMutate = None,
         tls_termination: EndpointTLSTerminationAtEdge = None,
     ):
-        self._client.edges_https.update(
+        self._client.edges.https.update(
             id=self.id,
             description=description,
             metadata=metadata,
             hostports=hostports,
             mutual_tls=mutual_tls,
             tls_termination=tls_termination,
         )
 
     def delete(
         self,
     ):
-        self._client.edges_https.delete(
+        self._client.edges.https.delete(
             id=self.id,
         )
 
     @property
     def id(self) -> str:
         """unique identifier of this edge"""
         return self._props["id"]
@@ -2224,16 +2228,16 @@
 
 class TCPEdgeList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["tcp_edges"] = (
             [TCPEdge(client, x) for x in props["tcp_edges"]]
-            if props["tcp_edges"] is not None
-            else None
+            if props.get("tcp_edges") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -2262,20 +2266,20 @@
 
 class TCPEdge(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["backend"] = (
             EndpointBackend(client, props["backend"])
-            if props["backend"] is not None
+            if props.get("backend") is not None
             else None
         )
         self._props["ip_restriction"] = (
             EndpointIPPolicy(client, props["ip_restriction"])
-            if props["ip_restriction"] is not None
+            if props.get("ip_restriction") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -2288,27 +2292,27 @@
         self,
         description: str = None,
         metadata: str = None,
         hostports: Sequence[str] = None,
         backend: EndpointBackendMutate = None,
         ip_restriction: EndpointIPPolicyMutate = None,
     ):
-        self._client.edges_tcp.update(
+        self._client.edges.tcp.update(
             id=self.id,
             description=description,
             metadata=metadata,
             hostports=hostports,
             backend=backend,
             ip_restriction=ip_restriction,
         )
 
     def delete(
         self,
     ):
-        self._client.edges_tcp.delete(
+        self._client.edges.tcp.delete(
             id=self.id,
         )
 
     @property
     def id(self) -> str:
         """unique identifier of this edge"""
         return self._props["id"]
@@ -2350,16 +2354,16 @@
 
 class TLSEdgeList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["tls_edges"] = (
             [TLSEdge(client, x) for x in props["tls_edges"]]
-            if props["tls_edges"] is not None
-            else None
+            if props.get("tls_edges") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -2388,30 +2392,30 @@
 
 class TLSEdge(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["backend"] = (
             EndpointBackend(client, props["backend"])
-            if props["backend"] is not None
+            if props.get("backend") is not None
             else None
         )
         self._props["ip_restriction"] = (
             EndpointIPPolicy(client, props["ip_restriction"])
-            if props["ip_restriction"] is not None
+            if props.get("ip_restriction") is not None
             else None
         )
         self._props["mutual_tls"] = (
             EndpointMutualTLS(client, props["mutual_tls"])
-            if props["mutual_tls"] is not None
+            if props.get("mutual_tls") is not None
             else None
         )
         self._props["tls_termination"] = (
             EndpointTLSTermination(client, props["tls_termination"])
-            if props["tls_termination"] is not None
+            if props.get("tls_termination") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -2426,29 +2430,29 @@
         metadata: str = None,
         hostports: Sequence[str] = None,
         backend: EndpointBackendMutate = None,
         ip_restriction: EndpointIPPolicyMutate = None,
         mutual_tls: EndpointMutualTLSMutate = None,
         tls_termination: EndpointTLSTermination = None,
     ):
-        self._client.edges_tls.update(
+        self._client.edges.tls.update(
             id=self.id,
             description=description,
             metadata=metadata,
             hostports=hostports,
             backend=backend,
             ip_restriction=ip_restriction,
             mutual_tls=mutual_tls,
             tls_termination=tls_termination,
         )
 
     def delete(
         self,
     ):
-        self._client.edges_tls.delete(
+        self._client.edges.tls.delete(
             id=self.id,
         )
 
     @property
     def id(self) -> str:
         """unique identifier of this edge"""
         return self._props["id"]
@@ -2497,24 +2501,26 @@
 
 
 class Endpoint(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["domain"] = (
-            Ref(client, props["domain"]) if props["domain"] is not None else None
+            Ref(client, props["domain"]) if props.get("domain") is not None else None
         )
         self._props["tcp_addr"] = (
-            Ref(client, props["tcp_addr"]) if props["tcp_addr"] is not None else None
+            Ref(client, props["tcp_addr"])
+            if props.get("tcp_addr") is not None
+            else None
         )
         self._props["tunnel"] = (
-            Ref(client, props["tunnel"]) if props["tunnel"] is not None else None
+            Ref(client, props["tunnel"]) if props.get("tunnel") is not None else None
         )
         self._props["edge"] = (
-            Ref(client, props["edge"]) if props["edge"] is not None else None
+            Ref(client, props["edge"]) if props.get("edge") is not None else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -2590,16 +2596,16 @@
 
 class EndpointList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["endpoints"] = (
             [Endpoint(client, x) for x in props["endpoints"]]
-            if props["endpoints"] is not None
-            else None
+            if props.get("endpoints") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -2628,15 +2634,15 @@
 
 class EventDestination(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["target"] = (
             EventTarget(client, props["target"])
-            if props["target"] is not None
+            if props.get("target") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -2690,16 +2696,16 @@
 
 class EventDestinationList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["event_destinations"] = (
             [EventDestination(client, x) for x in props["event_destinations"]]
-            if props["event_destinations"] is not None
-            else None
+            if props.get("event_destinations") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -2728,25 +2734,25 @@
 
 class EventTarget(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["firehose"] = (
             EventTargetFirehose(client, props["firehose"])
-            if props["firehose"] is not None
+            if props.get("firehose") is not None
             else None
         )
         self._props["kinesis"] = (
             EventTargetKinesis(client, props["kinesis"])
-            if props["kinesis"] is not None
+            if props.get("kinesis") is not None
             else None
         )
         self._props["cloudwatch_logs"] = (
             EventTargetCloudwatchLogs(client, props["cloudwatch_logs"])
-            if props["cloudwatch_logs"] is not None
+            if props.get("cloudwatch_logs") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -2772,15 +2778,15 @@
 
 
 class EventTargetFirehose(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["auth"] = (
-            AWSAuth(client, props["auth"]) if props["auth"] is not None else None
+            AWSAuth(client, props["auth"]) if props.get("auth") is not None else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -2800,15 +2806,15 @@
 
 
 class EventTargetKinesis(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["auth"] = (
-            AWSAuth(client, props["auth"]) if props["auth"] is not None else None
+            AWSAuth(client, props["auth"]) if props.get("auth") is not None else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -2828,15 +2834,15 @@
 
 
 class EventTargetCloudwatchLogs(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["auth"] = (
-            AWSAuth(client, props["auth"]) if props["auth"] is not None else None
+            AWSAuth(client, props["auth"]) if props.get("auth") is not None else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -2858,19 +2864,19 @@
 
 
 class AWSAuth(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["role"] = (
-            AWSRole(client, props["role"]) if props["role"] is not None else None
+            AWSRole(client, props["role"]) if props.get("role") is not None else None
         )
         self._props["creds"] = (
             AWSCredentials(client, props["creds"])
-            if props["creds"] is not None
+            if props.get("creds") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -2937,16 +2943,16 @@
 
 class EventSubscriptionList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["event_subscriptions"] = (
             [EventSubscription(client, x) for x in props["event_subscriptions"]]
-            if props["event_subscriptions"] is not None
-            else None
+            if props.get("event_subscriptions") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -2975,21 +2981,21 @@
 
 class EventSubscription(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["sources"] = (
             [EventSource(client, x) for x in props["sources"]]
-            if props["sources"] is not None
-            else None
+            if props.get("sources") is not None
+            else []
         )
         self._props["destinations"] = (
             [Ref(client, x) for x in props["destinations"]]
-            if props["destinations"] is not None
-            else None
+            if props.get("destinations") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -3087,16 +3093,16 @@
 
 class EventSourceList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["sources"] = (
             [EventSource(client, x) for x in props["sources"]]
-            if props["sources"] is not None
-            else None
+            if props.get("sources") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -3175,16 +3181,16 @@
 
 class IPPolicyList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["ip_policies"] = (
             [IPPolicy(client, x) for x in props["ip_policies"]]
-            if props["ip_policies"] is not None
-            else None
+            if props.get("ip_policies") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -3212,15 +3218,17 @@
 
 
 class IPPolicyRule(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["ip_policy"] = (
-            Ref(client, props["ip_policy"]) if props["ip_policy"] is not None else None
+            Ref(client, props["ip_policy"])
+            if props.get("ip_policy") is not None
+            else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -3291,16 +3299,16 @@
 
 class IPPolicyRuleList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["ip_policy_rules"] = (
             [IPPolicyRule(client, x) for x in props["ip_policy_rules"]]
-            if props["ip_policy_rules"] is not None
-            else None
+            if props.get("ip_policy_rules") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -3329,16 +3337,16 @@
 
 class IPRestriction(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["ip_policies"] = (
             [Ref(client, x) for x in props["ip_policies"]]
-            if props["ip_policies"] is not None
-            else None
+            if props.get("ip_policies") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -3396,16 +3404,16 @@
 
 class IPRestrictionList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["ip_restrictions"] = (
             [IPRestriction(client, x) for x in props["ip_restrictions"]]
-            if props["ip_restrictions"] is not None
-            else None
+            if props.get("ip_restrictions") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -3419,15 +3427,15 @@
     @property
     def ip_restrictions(self) -> Sequence[IPRestriction]:
         """the list of all IP restrictions on this account"""
         return self._props["ip_restrictions"]
 
     @property
     def uri(self) -> str:
-        """URI of the IP resrtrictions list API resource"""
+        """URI of the IP restrictions list API resource"""
         return self._props["uri"]
 
     @property
     def next_page_uri(self) -> str:
         """URI of the next page, or null if there is no next page"""
         return self._props["next_page_uri"]
 
@@ -3491,16 +3499,16 @@
 
 class ReservedAddrList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["reserved_addrs"] = (
             [ReservedAddr(client, x) for x in props["reserved_addrs"]]
-            if props["reserved_addrs"] is not None
-            else None
+            if props.get("reserved_addrs") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -3529,25 +3537,25 @@
 
 class ReservedDomain(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["certificate"] = (
             Ref(client, props["certificate"])
-            if props["certificate"] is not None
+            if props.get("certificate") is not None
             else None
         )
         self._props["certificate_management_policy"] = (
             ReservedDomainCertPolicy(client, props["certificate_management_policy"])
-            if props["certificate_management_policy"] is not None
+            if props.get("certificate_management_policy") is not None
             else None
         )
         self._props["certificate_management_status"] = (
             ReservedDomainCertStatus(client, props["certificate_management_status"])
-            if props["certificate_management_status"] is not None
+            if props.get("certificate_management_status") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -3626,16 +3634,16 @@
 
 class ReservedDomainList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["reserved_domains"] = (
             [ReservedDomain(client, x) for x in props["reserved_domains"]]
-            if props["reserved_domains"] is not None
-            else None
+            if props.get("reserved_domains") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -3689,15 +3697,15 @@
 
 class ReservedDomainCertStatus(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["provisioning_job"] = (
             ReservedDomainCertJob(client, props["provisioning_job"])
-            if props["provisioning_job"] is not None
+            if props.get("provisioning_job") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -3825,16 +3833,16 @@
         self._client = client
         self._props = props
         self._props["ssh_certificate_authorities"] = (
             [
                 SSHCertificateAuthority(client, x)
                 for x in props["ssh_certificate_authorities"]
             ]
-            if props["ssh_certificate_authorities"] is not None
-            else None
+            if props.get("ssh_certificate_authorities") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -3935,16 +3943,16 @@
 
 class SSHCredentialList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["ssh_credentials"] = (
             [SSHCredential(client, x) for x in props["ssh_credentials"]]
-            if props["ssh_credentials"] is not None
-            else None
+            if props.get("ssh_credentials") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -4066,16 +4074,16 @@
 
 class SSHHostCertificateList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["ssh_host_certificates"] = (
             [SSHHostCertificate(client, x) for x in props["ssh_host_certificates"]]
-            if props["ssh_host_certificates"] is not None
-            else None
+            if props.get("ssh_host_certificates") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -4172,15 +4180,15 @@
     @property
     def ssh_certificate_authority_id(self) -> str:
         """the ssh certificate authority that is used to sign this ssh user certificate"""
         return self._props["ssh_certificate_authority_id"]
 
     @property
     def principals(self) -> Sequence[str]:
-        """the list of principals included in the ssh user certificate. This is the list of usernames that the certificate holder may sign in as on a machine authorizinig the signing certificate authority. Dangerously, if no principals are specified, this certificate may be used to log in as any user."""
+        """the list of principals included in the ssh user certificate. This is the list of usernames that the certificate holder may sign in as on a machine authorizing the signing certificate authority. Dangerously, if no principals are specified, this certificate may be used to log in as any user."""
         return self._props["principals"]
 
     @property
     def critical_options(self) -> Mapping[str, str]:
         """A map of critical options included in the certificate. Only two critical options are currently defined by OpenSSH: ``force-command`` and ``source-address``. See `the OpenSSH certificate protocol spec` <https://github.com/openssh/openssh-portable/blob/master/PROTOCOL.certkeys>`_ for additional details."""
         return self._props["critical_options"]
 
@@ -4207,16 +4215,16 @@
 
 class SSHUserCertificateList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["ssh_user_certificates"] = (
             [SSHUserCertificate(client, x) for x in props["ssh_user_certificates"]]
-            if props["ssh_user_certificates"] is not None
-            else None
+            if props.get("ssh_user_certificates") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -4245,15 +4253,15 @@
 
 class TLSCertificate(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["subject_alternative_names"] = (
             TLSCertificateSANs(client, props["subject_alternative_names"])
-            if props["subject_alternative_names"] is not None
+            if props.get("subject_alternative_names") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -4388,16 +4396,16 @@
 
 class TLSCertificateList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["tls_certificates"] = (
             [TLSCertificate(client, x) for x in props["tls_certificates"]]
-            if props["tls_certificates"] is not None
-            else None
+            if props.get("tls_certificates") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -4451,15 +4459,15 @@
 
 class TunnelSession(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["credential"] = (
             Ref(client, props["credential"])
-            if props["credential"] is not None
+            if props.get("credential") is not None
             else None
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
@@ -4521,16 +4529,16 @@
 
 class TunnelSessionList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["tunnel_sessions"] = (
             [TunnelSession(client, x) for x in props["tunnel_sessions"]]
-            if props["tunnel_sessions"] is not None
-            else None
+            if props.get("tunnel_sessions") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -4559,24 +4567,26 @@
 
 class Tunnel(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["tunnel_session"] = (
             Ref(client, props["tunnel_session"])
-            if props["tunnel_session"] is not None
+            if props.get("tunnel_session") is not None
             else None
         )
         self._props["endpoint"] = (
-            Ref(client, props["endpoint"]) if props["endpoint"] is not None else None
+            Ref(client, props["endpoint"])
+            if props.get("endpoint") is not None
+            else None
         )
         self._props["backends"] = (
             [Ref(client, x) for x in props["backends"]]
-            if props["backends"] is not None
-            else None
+            if props.get("backends") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
@@ -4642,16 +4652,16 @@
 
 class TunnelList(object):
     def __init__(self, client, props):
         self._client = client
         self._props = props
         self._props["tunnels"] = (
             [Tunnel(client, x) for x in props["tunnels"]]
-            if props["tunnels"] is not None
-            else None
+            if props.get("tunnels") is not None
+            else []
         )
 
     def __eq__(self, other):
         return self._props == other._props
 
     def __str__(self):
         if "id" in self._props:
```

### Comparing `ngrok-api-0.6.0/ngrok/error.py` & `ngrok-api-0.8.0/ngrok/error.py`

 * *Files identical despite different names*

### Comparing `ngrok-api-0.6.0/ngrok/http_client.py` & `ngrok-api-0.8.0/ngrok/http_client.py`

 * *Files identical despite different names*

### Comparing `ngrok-api-0.6.0/ngrok/iterator.py` & `ngrok-api-0.8.0/ngrok/iterator.py`

 * *Files identical despite different names*

### Comparing `ngrok-api-0.6.0/ngrok/services.py` & `ngrok-api-0.8.0/ngrok/services.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 from collections.abc import Iterator
 from typing import Any, Mapping, Sequence
 
 from .http_client import HTTPClient
 from .datatypes import *
+from .utils import *
 
 
 class AbuseReportsClient(object):
     """Abuse Reports allow you to submit take-down requests for URLs hosted by
     ngrok that violate ngrok's terms of service."""
 
     def __init__(self, client):
@@ -22,21 +23,19 @@
 
         :param urls: a list of URLs containing suspected abusive content
         :param metadata: arbitrary user-defined data about this abuse report. Optional, max 4096 bytes.
 
         https://ngrok.com/docs/api#api-abuse-reports-create
         """
         path = "/abuse_reports"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                urls=urls,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            urls=urls,
+            metadata=metadata,
         )
+        result = self._client.http_client.post(path, body_arg)
         return AbuseReport(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> AbuseReport:
         """Get the detailed status of abuse report by ID.
@@ -45,15 +44,16 @@
 
         https://ngrok.com/docs/api#api-abuse-reports-get
         """
         path = "/abuse_reports/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return AbuseReport(self._client, result)
 
 
 class AgentIngressesClient(object):
     def __init__(self, client):
         self._client = client
 
@@ -68,22 +68,20 @@
         :param description: human-readable description of the use of this Agent Ingress. optional, max 255 bytes.
         :param metadata: arbitrary user-defined machine-readable data of this Agent Ingress. optional, max 4096 bytes
         :param domain: the domain that you own to be used as the base domain name to generate regional agent ingress domains.
 
         https://ngrok.com/docs/api#api-agent-ingresses-create
         """
         path = "/agent_ingresses"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                domain=domain,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            domain=domain,
         )
+        result = self._client.http_client.post(path, body_arg)
         return AgentIngress(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an Agent Ingress by ID
@@ -92,15 +90,16 @@
 
         https://ngrok.com/docs/api#api-agent-ingresses-delete
         """
         path = "/agent_ingresses/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> AgentIngress:
         """Get the details of an Agent Ingress by ID.
 
@@ -108,15 +107,16 @@
 
         https://ngrok.com/docs/api#api-agent-ingresses-get
         """
         path = "/agent_ingresses/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return AgentIngress(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> AgentIngressList:
@@ -124,21 +124,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-agent-ingresses-list
         """
         path = "/agent_ingresses"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return AgentIngressList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -151,21 +149,19 @@
 
         https://ngrok.com/docs/api#api-agent-ingresses-update
         """
         path = "/agent_ingresses/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return AgentIngress(self._client, result)
 
 
 class APIKeysClient(object):
     """API Keys are used to authenticate to the `ngrok
     API` <https://ngrok.com/docs/api#authentication>`_. You may use the API itself
     to provision and manage API Keys but you'll need to provision your first API
@@ -184,21 +180,19 @@
 
         :param description: human-readable description of what uses the API key to authenticate. optional, max 255 bytes.
         :param metadata: arbitrary user-defined data of this API key. optional, max 4096 bytes
 
         https://ngrok.com/docs/api#api-api-keys-create
         """
         path = "/api_keys"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.post(path, body_arg)
         return APIKey(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an API key by ID
@@ -207,15 +201,16 @@
 
         https://ngrok.com/docs/api#api-api-keys-delete
         """
         path = "/api_keys/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> APIKey:
         """Get the details of an API key by ID.
 
@@ -223,15 +218,16 @@
 
         https://ngrok.com/docs/api#api-api-keys-get
         """
         path = "/api_keys/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return APIKey(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> APIKeyList:
@@ -239,21 +235,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-api-keys-list
         """
         path = "/api_keys"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return APIKeyList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -266,21 +260,19 @@
 
         https://ngrok.com/docs/api#api-api-keys-update
         """
         path = "/api_keys/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return APIKey(self._client, result)
 
 
 class FailoverBackendsClient(object):
     """A Failover backend defines failover behavior within a list of referenced
     backends. Traffic is sent to the first backend in the list. If that backend
     is offline or no connection can be established, ngrok attempts to connect to
@@ -300,39 +292,38 @@
         :param description: human-readable description of this backend. Optional
         :param metadata: arbitrary user-defined machine-readable data of this backend. Optional
         :param backends: the ids of the child backends in order
 
         https://ngrok.com/docs/api#api-failover-backends-create
         """
         path = "/backends/failover"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                backends=backends,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            backends=backends,
         )
+        result = self._client.http_client.post(path, body_arg)
         return FailoverBackend(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
-        """Delete a Failover backend by ID. TODO what if used?
+        """Delete a Failover backend by ID.
 
         :param id: a resource identifier
 
         https://ngrok.com/docs/api#api-failover-backends-delete
         """
         path = "/backends/failover/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> FailoverBackend:
         """Get detailed information about a Failover backend by ID
 
@@ -340,15 +331,16 @@
 
         https://ngrok.com/docs/api#api-failover-backends-get
         """
         path = "/backends/failover/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return FailoverBackend(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> FailoverBackendList:
@@ -356,21 +348,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-failover-backends-list
         """
         path = "/backends/failover"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return FailoverBackendList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -385,22 +375,20 @@
 
         https://ngrok.com/docs/api#api-failover-backends-update
         """
         path = "/backends/failover/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                backends=backends,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            backends=backends,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return FailoverBackend(self._client, result)
 
 
 class HTTPResponseBackendsClient(object):
     def __init__(self, client):
         self._client = client
 
@@ -419,24 +407,22 @@
         :param body: body to return as fixed content
         :param headers: headers to return
         :param status_code: status code to return
 
         https://ngrok.com/docs/api#api-http-response-backends-create
         """
         path = "/backends/http_response"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                body=body,
-                headers=headers,
-                status_code=status_code,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            body=body,
+            headers=headers,
+            status_code=status_code,
         )
+        result = self._client.http_client.post(path, body_arg)
         return HTTPResponseBackend(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """
@@ -445,15 +431,16 @@
 
         https://ngrok.com/docs/api#api-http-response-backends-delete
         """
         path = "/backends/http_response/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> HTTPResponseBackend:
         """
 
@@ -461,15 +448,16 @@
 
         https://ngrok.com/docs/api#api-http-response-backends-get
         """
         path = "/backends/http_response/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return HTTPResponseBackend(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> HTTPResponseBackendList:
@@ -477,21 +465,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-http-response-backends-list
         """
         path = "/backends/http_response"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return HTTPResponseBackendList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -510,24 +496,22 @@
 
         https://ngrok.com/docs/api#api-http-response-backends-update
         """
         path = "/backends/http_response/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                body=body,
-                headers=headers,
-                status_code=status_code,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            body=body,
+            headers=headers,
+            status_code=status_code,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return HTTPResponseBackend(self._client, result)
 
 
 class TunnelGroupBackendsClient(object):
     """A Tunnel Group Backend balances traffic among all online tunnels that match
     a label selector."""
 
@@ -545,39 +529,38 @@
         :param description: human-readable description of this backend. Optional
         :param metadata: arbitrary user-defined machine-readable data of this backend. Optional
         :param labels: labels to watch for tunnels on, e.g. app->foo, dc->bar
 
         https://ngrok.com/docs/api#api-tunnel-group-backends-create
         """
         path = "/backends/tunnel_group"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                labels=labels,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            labels=labels,
         )
+        result = self._client.http_client.post(path, body_arg)
         return TunnelGroupBackend(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
-        """Delete a TunnelGroup backend by ID. TODO what if used?
+        """Delete a TunnelGroup backend by ID.
 
         :param id: a resource identifier
 
         https://ngrok.com/docs/api#api-tunnel-group-backends-delete
         """
         path = "/backends/tunnel_group/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> TunnelGroupBackend:
         """Get detailed information about a TunnelGroup backend by ID
 
@@ -585,15 +568,16 @@
 
         https://ngrok.com/docs/api#api-tunnel-group-backends-get
         """
         path = "/backends/tunnel_group/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return TunnelGroupBackend(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> TunnelGroupBackendList:
@@ -601,21 +585,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-tunnel-group-backends-list
         """
         path = "/backends/tunnel_group"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return TunnelGroupBackendList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -630,22 +612,20 @@
 
         https://ngrok.com/docs/api#api-tunnel-group-backends-update
         """
         path = "/backends/tunnel_group/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                labels=labels,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            labels=labels,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return TunnelGroupBackend(self._client, result)
 
 
 class WeightedBackendsClient(object):
     """A Weighted Backend balances traffic among the referenced backends. Traffic
     is assigned proportionally to each based on its weight. The percentage of
     traffic is calculated by dividing a backend's weight by the sum of all
@@ -660,44 +640,43 @@
         metadata: str = "",
         backends: Mapping[str, int] = {},
     ) -> WeightedBackend:
         """Create a new Weighted backend
 
         :param description: human-readable description of this backend. Optional
         :param metadata: arbitrary user-defined machine-readable data of this backend. Optional
-        :param backends: the ids of the child backends to their weights (0-10000)
+        :param backends: the ids of the child backends to their weights [0-10000]
 
         https://ngrok.com/docs/api#api-weighted-backends-create
         """
         path = "/backends/weighted"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                backends=backends,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            backends=backends,
         )
+        result = self._client.http_client.post(path, body_arg)
         return WeightedBackend(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
-        """Delete a Weighted backend by ID. TODO what if used?
+        """Delete a Weighted backend by ID.
 
         :param id: a resource identifier
 
         https://ngrok.com/docs/api#api-weighted-backends-delete
         """
         path = "/backends/weighted/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> WeightedBackend:
         """Get detailed information about a Weighted backend by ID
 
@@ -705,15 +684,16 @@
 
         https://ngrok.com/docs/api#api-weighted-backends-get
         """
         path = "/backends/weighted/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return WeightedBackend(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> WeightedBackendList:
@@ -721,51 +701,47 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-weighted-backends-list
         """
         path = "/backends/weighted"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return WeightedBackendList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
         backends: Mapping[str, int] = {},
     ) -> WeightedBackend:
         """Update Weighted backend by ID
 
         :param id:
         :param description: human-readable description of this backend. Optional
         :param metadata: arbitrary user-defined machine-readable data of this backend. Optional
-        :param backends: the ids of the child backends to their weights (0-10000)
+        :param backends: the ids of the child backends to their weights [0-10000]
 
         https://ngrok.com/docs/api#api-weighted-backends-update
         """
         path = "/backends/weighted/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                backends=backends,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            backends=backends,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return WeightedBackend(self._client, result)
 
 
 class CertificateAuthoritiesClient(object):
     """Certificate Authorities are x509 certificates that are used to sign other
     x509 certificates. Attach a Certificate Authority to the Mutual TLS module
     to verify that the TLS certificate presented by a client has been signed by
@@ -786,22 +762,20 @@
         :param description: human-readable description of this Certificate Authority. optional, max 255 bytes.
         :param metadata: arbitrary user-defined machine-readable data of this Certificate Authority. optional, max 4096 bytes.
         :param ca_pem: raw PEM of the Certificate Authority
 
         https://ngrok.com/docs/api#api-certificate-authorities-create
         """
         path = "/certificate_authorities"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                ca_pem=ca_pem,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            ca_pem=ca_pem,
         )
+        result = self._client.http_client.post(path, body_arg)
         return CertificateAuthority(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete a Certificate Authority
@@ -810,15 +784,16 @@
 
         https://ngrok.com/docs/api#api-certificate-authorities-delete
         """
         path = "/certificate_authorities/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> CertificateAuthority:
         """Get detailed information about a certficate authority
 
@@ -826,15 +801,16 @@
 
         https://ngrok.com/docs/api#api-certificate-authorities-get
         """
         path = "/certificate_authorities/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return CertificateAuthority(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> CertificateAuthorityList:
@@ -842,21 +818,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-certificate-authorities-list
         """
         path = "/certificate_authorities"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return CertificateAuthorityList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -869,21 +843,19 @@
 
         https://ngrok.com/docs/api#api-certificate-authorities-update
         """
         path = "/certificate_authorities/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return CertificateAuthority(self._client, result)
 
 
 class CredentialsClient(object):
     """Tunnel Credentials are ngrok agent authtokens. They authorize the ngrok
     agent to connect the ngrok service as your account. They are installed with
     the ``ngrok authtoken`` command or by specifying it in the ``ngrok.yml``
@@ -903,22 +875,20 @@
         :param description: human-readable description of who or what will use the credential to authenticate. Optional, max 255 bytes.
         :param metadata: arbitrary user-defined machine-readable data of this credential. Optional, max 4096 bytes.
         :param acl: optional list of ACL rules. If unspecified, the credential will have no restrictions. The only allowed ACL rule at this time is the ``bind`` rule. The ``bind`` rule allows the caller to restrict what domains and addresses the token is allowed to bind. For example, to allow the token to open a tunnel on example.ngrok.io your ACL would include the rule ``bind:example.ngrok.io``. Bind rules may specify a leading wildcard to match multiple domains with a common suffix. For example, you may specify a rule of ``bind:*.example.com`` which will allow ``x.example.com``, ``y.example.com``, ``*.example.com``, etc. A rule of ``'*'`` is equivalent to no acl at all and will explicitly permit all actions.
 
         https://ngrok.com/docs/api#api-credentials-create
         """
         path = "/credentials"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                acl=acl,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            acl=acl,
         )
+        result = self._client.http_client.post(path, body_arg)
         return Credential(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete a tunnel authtoken credential by ID
@@ -927,15 +897,16 @@
 
         https://ngrok.com/docs/api#api-credentials-delete
         """
         path = "/credentials/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> Credential:
         """Get detailed information about a tunnel authtoken credential
 
@@ -943,15 +914,16 @@
 
         https://ngrok.com/docs/api#api-credentials-get
         """
         path = "/credentials/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return Credential(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> CredentialList:
@@ -959,21 +931,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-credentials-list
         """
         path = "/credentials"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return CredentialList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -988,22 +958,20 @@
 
         https://ngrok.com/docs/api#api-credentials-update
         """
         path = "/credentials/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                acl=acl,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            acl=acl,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return Credential(self._client, result)
 
 
 class EdgesHTTPSRoutesClient(object):
     def __init__(self, client):
         self._client = client
 
@@ -1047,34 +1015,32 @@
 
         https://ngrok.com/docs/api#api-edges-https-routes-create
         """
         path = "/edges/https/{edge_id}/routes"
         path = path.format(
             edge_id=edge_id,
         )
-        result = self._client.http_client.post(
-            path,
-            dict(
-                match_type=match_type,
-                match=match,
-                description=description,
-                metadata=metadata,
-                backend=backend,
-                ip_restriction=ip_restriction,
-                circuit_breaker=circuit_breaker,
-                compression=compression,
-                request_headers=request_headers,
-                response_headers=response_headers,
-                webhook_verification=webhook_verification,
-                oauth=oauth,
-                saml=saml,
-                oidc=oidc,
-                websocket_tcp_converter=websocket_tcp_converter,
-            ),
+        body_arg = dict(
+            match_type=match_type,
+            match=match,
+            description=description,
+            metadata=metadata,
+            backend=extract_props(backend),
+            ip_restriction=extract_props(ip_restriction),
+            circuit_breaker=extract_props(circuit_breaker),
+            compression=extract_props(compression),
+            request_headers=extract_props(request_headers),
+            response_headers=extract_props(response_headers),
+            webhook_verification=extract_props(webhook_verification),
+            oauth=extract_props(oauth),
+            saml=extract_props(saml),
+            oidc=extract_props(oidc),
+            websocket_tcp_converter=extract_props(websocket_tcp_converter),
         )
+        result = self._client.http_client.post(path, body_arg)
         return HTTPSEdgeRoute(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> HTTPSEdgeRoute:
@@ -1086,15 +1052,16 @@
         https://ngrok.com/docs/api#api-edges-https-routes-get
         """
         path = "/edges/https/{edge_id}/routes/{id}"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return HTTPSEdgeRoute(self._client, result)
 
     def update(
         self,
         edge_id: str,
         id: str,
         match_type: str = "",
@@ -1136,34 +1103,32 @@
         https://ngrok.com/docs/api#api-edges-https-routes-update
         """
         path = "/edges/https/{edge_id}/routes/{id}"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                match_type=match_type,
-                match=match,
-                description=description,
-                metadata=metadata,
-                backend=backend,
-                ip_restriction=ip_restriction,
-                circuit_breaker=circuit_breaker,
-                compression=compression,
-                request_headers=request_headers,
-                response_headers=response_headers,
-                webhook_verification=webhook_verification,
-                oauth=oauth,
-                saml=saml,
-                oidc=oidc,
-                websocket_tcp_converter=websocket_tcp_converter,
-            ),
+        body_arg = dict(
+            match_type=match_type,
+            match=match,
+            description=description,
+            metadata=metadata,
+            backend=extract_props(backend),
+            ip_restriction=extract_props(ip_restriction),
+            circuit_breaker=extract_props(circuit_breaker),
+            compression=extract_props(compression),
+            request_headers=extract_props(request_headers),
+            response_headers=extract_props(response_headers),
+            webhook_verification=extract_props(webhook_verification),
+            oauth=extract_props(oauth),
+            saml=extract_props(saml),
+            oidc=extract_props(oidc),
+            websocket_tcp_converter=extract_props(websocket_tcp_converter),
         )
+        result = self._client.http_client.patch(path, body_arg)
         return HTTPSEdgeRoute(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -1175,15 +1140,16 @@
         https://ngrok.com/docs/api#api-edges-https-routes-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgesHTTPSClient(object):
     def __init__(self, client):
         self._client = client
 
     def create(
@@ -1201,24 +1167,22 @@
         :param hostports: hostports served by this edge
         :param mutual_tls: edge modules
         :param tls_termination:
 
         https://ngrok.com/docs/api#api-edges-https-create
         """
         path = "/edges/https"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                hostports=hostports,
-                mutual_tls=mutual_tls,
-                tls_termination=tls_termination,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            hostports=hostports,
+            mutual_tls=extract_props(mutual_tls),
+            tls_termination=extract_props(tls_termination),
         )
+        result = self._client.http_client.post(path, body_arg)
         return HTTPSEdge(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> HTTPSEdge:
         """Get an HTTPS Edge by ID
@@ -1227,15 +1191,16 @@
 
         https://ngrok.com/docs/api#api-edges-https-get
         """
         path = "/edges/https/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return HTTPSEdge(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> HTTPSEdgeList:
@@ -1243,21 +1208,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-edges-https-list
         """
         path = "/edges/https"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return HTTPSEdgeList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -1276,24 +1239,22 @@
 
         https://ngrok.com/docs/api#api-edges-https-update
         """
         path = "/edges/https/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                hostports=hostports,
-                mutual_tls=mutual_tls,
-                tls_termination=tls_termination,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            hostports=hostports,
+            mutual_tls=extract_props(mutual_tls),
+            tls_termination=extract_props(tls_termination),
         )
+        result = self._client.http_client.patch(path, body_arg)
         return HTTPSEdge(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an HTTPS Edge by ID
@@ -1302,15 +1263,16 @@
 
         https://ngrok.com/docs/api#api-edges-https-delete
         """
         path = "/edges/https/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class HTTPSEdgeMutualTLSModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -1325,20 +1287,16 @@
 
         https://ngrok.com/docs/api#api-https-edge-mutual-tls-module-replace
         """
         path = "/edges/https/{id}/mutual_tls"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointMutualTLS(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> EndpointMutualTLS:
         """
@@ -1347,15 +1305,16 @@
 
         https://ngrok.com/docs/api#api-https-edge-mutual-tls-module-get
         """
         path = "/edges/https/{id}/mutual_tls"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointMutualTLS(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """
@@ -1364,15 +1323,16 @@
 
         https://ngrok.com/docs/api#api-https-edge-mutual-tls-module-delete
         """
         path = "/edges/https/{id}/mutual_tls"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class HTTPSEdgeTLSTerminationModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -1387,20 +1347,16 @@
 
         https://ngrok.com/docs/api#api-https-edge-tls-termination-module-replace
         """
         path = "/edges/https/{id}/tls_termination"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointTLSTermination(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> EndpointTLSTermination:
         """
@@ -1409,15 +1365,16 @@
 
         https://ngrok.com/docs/api#api-https-edge-tls-termination-module-get
         """
         path = "/edges/https/{id}/tls_termination"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointTLSTermination(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """
@@ -1426,15 +1383,16 @@
 
         https://ngrok.com/docs/api#api-https-edge-tls-termination-module-delete
         """
         path = "/edges/https/{id}/tls_termination"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgeRouteBackendModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -1452,20 +1410,16 @@
         https://ngrok.com/docs/api#api-edge-route-backend-module-replace
         """
         path = "/edges/https/{edge_id}/routes/{id}/backend"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointBackend(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> EndpointBackend:
@@ -1477,15 +1431,16 @@
         https://ngrok.com/docs/api#api-edge-route-backend-module-get
         """
         path = "/edges/https/{edge_id}/routes/{id}/backend"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointBackend(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -1497,15 +1452,16 @@
         https://ngrok.com/docs/api#api-edge-route-backend-module-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}/backend"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgeRouteIPRestrictionModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -1523,20 +1479,16 @@
         https://ngrok.com/docs/api#api-edge-route-ip-restriction-module-replace
         """
         path = "/edges/https/{edge_id}/routes/{id}/ip_restriction"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointIPPolicy(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> EndpointIPPolicy:
@@ -1548,15 +1500,16 @@
         https://ngrok.com/docs/api#api-edge-route-ip-restriction-module-get
         """
         path = "/edges/https/{edge_id}/routes/{id}/ip_restriction"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointIPPolicy(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -1568,15 +1521,16 @@
         https://ngrok.com/docs/api#api-edge-route-ip-restriction-module-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}/ip_restriction"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgeRouteRequestHeadersModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -1594,20 +1548,16 @@
         https://ngrok.com/docs/api#api-edge-route-request-headers-module-replace
         """
         path = "/edges/https/{edge_id}/routes/{id}/request_headers"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointRequestHeaders(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> EndpointRequestHeaders:
@@ -1619,15 +1569,16 @@
         https://ngrok.com/docs/api#api-edge-route-request-headers-module-get
         """
         path = "/edges/https/{edge_id}/routes/{id}/request_headers"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointRequestHeaders(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -1639,15 +1590,16 @@
         https://ngrok.com/docs/api#api-edge-route-request-headers-module-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}/request_headers"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgeRouteResponseHeadersModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -1665,20 +1617,16 @@
         https://ngrok.com/docs/api#api-edge-route-response-headers-module-replace
         """
         path = "/edges/https/{edge_id}/routes/{id}/response_headers"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointResponseHeaders(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> EndpointResponseHeaders:
@@ -1690,15 +1638,16 @@
         https://ngrok.com/docs/api#api-edge-route-response-headers-module-get
         """
         path = "/edges/https/{edge_id}/routes/{id}/response_headers"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointResponseHeaders(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -1710,15 +1659,16 @@
         https://ngrok.com/docs/api#api-edge-route-response-headers-module-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}/response_headers"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgeRouteCompressionModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -1736,20 +1686,16 @@
         https://ngrok.com/docs/api#api-edge-route-compression-module-replace
         """
         path = "/edges/https/{edge_id}/routes/{id}/compression"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointCompression(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> EndpointCompression:
@@ -1761,15 +1707,16 @@
         https://ngrok.com/docs/api#api-edge-route-compression-module-get
         """
         path = "/edges/https/{edge_id}/routes/{id}/compression"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointCompression(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -1781,15 +1728,16 @@
         https://ngrok.com/docs/api#api-edge-route-compression-module-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}/compression"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgeRouteCircuitBreakerModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -1807,20 +1755,16 @@
         https://ngrok.com/docs/api#api-edge-route-circuit-breaker-module-replace
         """
         path = "/edges/https/{edge_id}/routes/{id}/circuit_breaker"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointCircuitBreaker(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> EndpointCircuitBreaker:
@@ -1832,15 +1776,16 @@
         https://ngrok.com/docs/api#api-edge-route-circuit-breaker-module-get
         """
         path = "/edges/https/{edge_id}/routes/{id}/circuit_breaker"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointCircuitBreaker(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -1852,15 +1797,16 @@
         https://ngrok.com/docs/api#api-edge-route-circuit-breaker-module-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}/circuit_breaker"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgeRouteWebhookVerificationModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -1878,20 +1824,16 @@
         https://ngrok.com/docs/api#api-edge-route-webhook-verification-module-replace
         """
         path = "/edges/https/{edge_id}/routes/{id}/webhook_verification"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointWebhookValidation(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> EndpointWebhookValidation:
@@ -1903,15 +1845,16 @@
         https://ngrok.com/docs/api#api-edge-route-webhook-verification-module-get
         """
         path = "/edges/https/{edge_id}/routes/{id}/webhook_verification"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointWebhookValidation(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -1923,15 +1866,16 @@
         https://ngrok.com/docs/api#api-edge-route-webhook-verification-module-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}/webhook_verification"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgeRouteOAuthModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -1949,20 +1893,16 @@
         https://ngrok.com/docs/api#api-edge-route-o-auth-module-replace
         """
         path = "/edges/https/{edge_id}/routes/{id}/oauth"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointOAuth(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> EndpointOAuth:
@@ -1974,15 +1914,16 @@
         https://ngrok.com/docs/api#api-edge-route-o-auth-module-get
         """
         path = "/edges/https/{edge_id}/routes/{id}/oauth"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointOAuth(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -1994,15 +1935,16 @@
         https://ngrok.com/docs/api#api-edge-route-o-auth-module-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}/oauth"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgeRouteSAMLModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -2020,20 +1962,16 @@
         https://ngrok.com/docs/api#api-edge-route-saml-module-replace
         """
         path = "/edges/https/{edge_id}/routes/{id}/saml"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointSAML(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> EndpointSAML:
@@ -2045,15 +1983,16 @@
         https://ngrok.com/docs/api#api-edge-route-saml-module-get
         """
         path = "/edges/https/{edge_id}/routes/{id}/saml"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointSAML(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -2065,15 +2004,16 @@
         https://ngrok.com/docs/api#api-edge-route-saml-module-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}/saml"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgeRouteOIDCModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -2091,20 +2031,16 @@
         https://ngrok.com/docs/api#api-edge-route-oidc-module-replace
         """
         path = "/edges/https/{edge_id}/routes/{id}/oidc"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointOIDC(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> EndpointOIDC:
@@ -2116,15 +2052,16 @@
         https://ngrok.com/docs/api#api-edge-route-oidc-module-get
         """
         path = "/edges/https/{edge_id}/routes/{id}/oidc"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointOIDC(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -2136,15 +2073,16 @@
         https://ngrok.com/docs/api#api-edge-route-oidc-module-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}/oidc"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgeRouteWebsocketTCPConverterModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -2162,20 +2100,16 @@
         https://ngrok.com/docs/api#api-edge-route-websocket-tcp-converter-module-replace
         """
         path = "/edges/https/{edge_id}/routes/{id}/websocket_tcp_converter"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointWebsocketTCPConverter(self._client, result)
 
     def get(
         self,
         edge_id: str,
         id: str,
     ) -> EndpointWebsocketTCPConverter:
@@ -2187,15 +2121,16 @@
         https://ngrok.com/docs/api#api-edge-route-websocket-tcp-converter-module-get
         """
         path = "/edges/https/{edge_id}/routes/{id}/websocket_tcp_converter"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointWebsocketTCPConverter(self._client, result)
 
     def delete(
         self,
         edge_id: str,
         id: str,
     ):
@@ -2207,15 +2142,16 @@
         https://ngrok.com/docs/api#api-edge-route-websocket-tcp-converter-module-delete
         """
         path = "/edges/https/{edge_id}/routes/{id}/websocket_tcp_converter"
         path = path.format(
             edge_id=edge_id,
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgesTCPClient(object):
     def __init__(self, client):
         self._client = client
 
     def create(
@@ -2233,24 +2169,22 @@
         :param hostports: hostports served by this edge
         :param backend: edge modules
         :param ip_restriction:
 
         https://ngrok.com/docs/api#api-edges-tcp-create
         """
         path = "/edges/tcp"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                hostports=hostports,
-                backend=backend,
-                ip_restriction=ip_restriction,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            hostports=hostports,
+            backend=extract_props(backend),
+            ip_restriction=extract_props(ip_restriction),
         )
+        result = self._client.http_client.post(path, body_arg)
         return TCPEdge(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> TCPEdge:
         """Get a TCP Edge by ID
@@ -2259,15 +2193,16 @@
 
         https://ngrok.com/docs/api#api-edges-tcp-get
         """
         path = "/edges/tcp/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return TCPEdge(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> TCPEdgeList:
@@ -2275,21 +2210,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-edges-tcp-list
         """
         path = "/edges/tcp"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return TCPEdgeList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -2308,24 +2241,22 @@
 
         https://ngrok.com/docs/api#api-edges-tcp-update
         """
         path = "/edges/tcp/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                hostports=hostports,
-                backend=backend,
-                ip_restriction=ip_restriction,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            hostports=hostports,
+            backend=extract_props(backend),
+            ip_restriction=extract_props(ip_restriction),
         )
+        result = self._client.http_client.patch(path, body_arg)
         return TCPEdge(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete a TCP Edge by ID
@@ -2334,15 +2265,16 @@
 
         https://ngrok.com/docs/api#api-edges-tcp-delete
         """
         path = "/edges/tcp/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class TCPEdgeBackendModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -2357,20 +2289,16 @@
 
         https://ngrok.com/docs/api#api-tcp-edge-backend-module-replace
         """
         path = "/edges/tcp/{id}/backend"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointBackend(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> EndpointBackend:
         """
@@ -2379,15 +2307,16 @@
 
         https://ngrok.com/docs/api#api-tcp-edge-backend-module-get
         """
         path = "/edges/tcp/{id}/backend"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointBackend(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """
@@ -2396,15 +2325,16 @@
 
         https://ngrok.com/docs/api#api-tcp-edge-backend-module-delete
         """
         path = "/edges/tcp/{id}/backend"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class TCPEdgeIPRestrictionModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -2419,20 +2349,16 @@
 
         https://ngrok.com/docs/api#api-tcp-edge-ip-restriction-module-replace
         """
         path = "/edges/tcp/{id}/ip_restriction"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointIPPolicy(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> EndpointIPPolicy:
         """
@@ -2441,15 +2367,16 @@
 
         https://ngrok.com/docs/api#api-tcp-edge-ip-restriction-module-get
         """
         path = "/edges/tcp/{id}/ip_restriction"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointIPPolicy(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """
@@ -2458,15 +2385,16 @@
 
         https://ngrok.com/docs/api#api-tcp-edge-ip-restriction-module-delete
         """
         path = "/edges/tcp/{id}/ip_restriction"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EdgesTLSClient(object):
     def __init__(self, client):
         self._client = client
 
     def create(
@@ -2488,26 +2416,24 @@
         :param ip_restriction:
         :param mutual_tls:
         :param tls_termination:
 
         https://ngrok.com/docs/api#api-edges-tls-create
         """
         path = "/edges/tls"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                hostports=hostports,
-                backend=backend,
-                ip_restriction=ip_restriction,
-                mutual_tls=mutual_tls,
-                tls_termination=tls_termination,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            hostports=hostports,
+            backend=extract_props(backend),
+            ip_restriction=extract_props(ip_restriction),
+            mutual_tls=extract_props(mutual_tls),
+            tls_termination=extract_props(tls_termination),
         )
+        result = self._client.http_client.post(path, body_arg)
         return TLSEdge(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> TLSEdge:
         """Get a TLS Edge by ID
@@ -2516,15 +2442,16 @@
 
         https://ngrok.com/docs/api#api-edges-tls-get
         """
         path = "/edges/tls/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return TLSEdge(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> TLSEdgeList:
@@ -2532,21 +2459,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-edges-tls-list
         """
         path = "/edges/tls"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return TLSEdgeList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -2569,26 +2494,24 @@
 
         https://ngrok.com/docs/api#api-edges-tls-update
         """
         path = "/edges/tls/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                hostports=hostports,
-                backend=backend,
-                ip_restriction=ip_restriction,
-                mutual_tls=mutual_tls,
-                tls_termination=tls_termination,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            hostports=hostports,
+            backend=extract_props(backend),
+            ip_restriction=extract_props(ip_restriction),
+            mutual_tls=extract_props(mutual_tls),
+            tls_termination=extract_props(tls_termination),
         )
+        result = self._client.http_client.patch(path, body_arg)
         return TLSEdge(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete a TLS Edge by ID
@@ -2597,15 +2520,16 @@
 
         https://ngrok.com/docs/api#api-edges-tls-delete
         """
         path = "/edges/tls/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class TLSEdgeBackendModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -2620,20 +2544,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-backend-module-replace
         """
         path = "/edges/tls/{id}/backend"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointBackend(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> EndpointBackend:
         """
@@ -2642,15 +2562,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-backend-module-get
         """
         path = "/edges/tls/{id}/backend"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointBackend(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """
@@ -2659,15 +2580,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-backend-module-delete
         """
         path = "/edges/tls/{id}/backend"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class TLSEdgeIPRestrictionModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -2682,20 +2604,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-ip-restriction-module-replace
         """
         path = "/edges/tls/{id}/ip_restriction"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointIPPolicy(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> EndpointIPPolicy:
         """
@@ -2704,15 +2622,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-ip-restriction-module-get
         """
         path = "/edges/tls/{id}/ip_restriction"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointIPPolicy(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """
@@ -2721,15 +2640,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-ip-restriction-module-delete
         """
         path = "/edges/tls/{id}/ip_restriction"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class TLSEdgeMutualTLSModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -2744,20 +2664,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-mutual-tls-module-replace
         """
         path = "/edges/tls/{id}/mutual_tls"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointMutualTLS(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> EndpointMutualTLS:
         """
@@ -2766,15 +2682,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-mutual-tls-module-get
         """
         path = "/edges/tls/{id}/mutual_tls"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointMutualTLS(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """
@@ -2783,15 +2700,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-mutual-tls-module-delete
         """
         path = "/edges/tls/{id}/mutual_tls"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class TLSEdgeTLSTerminationModuleClient(object):
     def __init__(self, client):
         self._client = client
 
     def replace(
@@ -2806,20 +2724,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-tls-termination-module-replace
         """
         path = "/edges/tls/{id}/tls_termination"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.put(
-            path,
-            dict(
-                module=module,
-            ),
-        )
+        body_arg = extract_props(module)
+        result = self._client.http_client.put(path, body_arg)
         return EndpointTLSTermination(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> EndpointTLSTermination:
         """
@@ -2828,15 +2742,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-tls-termination-module-get
         """
         path = "/edges/tls/{id}/tls_termination"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EndpointTLSTermination(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """
@@ -2845,15 +2760,16 @@
 
         https://ngrok.com/docs/api#api-tls-edge-tls-termination-module-delete
         """
         path = "/edges/tls/{id}/tls_termination"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class EndpointsClient(object):
     """Endpoints provides an API for querying the endpoint objects
     which define what tunnel or edge is used to serve a hostport.
     Only active endpoints associated with a tunnel or backend are returned."""
 
@@ -2869,21 +2785,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-endpoints-list
         """
         path = "/endpoints"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return EndpointList(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> Endpoint:
         """Get the status of an endpoint by ID
@@ -2892,15 +2806,16 @@
 
         https://ngrok.com/docs/api#api-endpoints-get
         """
         path = "/endpoints/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return Endpoint(self._client, result)
 
 
 class EventDestinationsClient(object):
     def __init__(self, client):
         self._client = client
 
@@ -2917,23 +2832,21 @@
         :param description: Human-readable description of the Event Destination. Optional, max 255 bytes.
         :param format: The output format you would like to serialize events into when sending to their target. Currently the only accepted value is ``JSON``.
         :param target: An object that encapsulates where and how to send your events. An event destination must contain exactly one of the following objects, leaving the rest null: ``kinesis``, ``firehose``, ``cloudwatch_logs``, or ``s3``.
 
         https://ngrok.com/docs/api#api-event-destinations-create
         """
         path = "/event_destinations"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                metadata=metadata,
-                description=description,
-                format=format,
-                target=target,
-            ),
+        body_arg = dict(
+            metadata=metadata,
+            description=description,
+            format=format,
+            target=extract_props(target),
         )
+        result = self._client.http_client.post(path, body_arg)
         return EventDestination(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an Event Destination. If the Event Destination is still referenced by an Event Subscription.
@@ -2942,15 +2855,16 @@
 
         https://ngrok.com/docs/api#api-event-destinations-delete
         """
         path = "/event_destinations/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> EventDestination:
         """Get detailed information about an Event Destination by ID.
 
@@ -2958,15 +2872,16 @@
 
         https://ngrok.com/docs/api#api-event-destinations-get
         """
         path = "/event_destinations/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EventDestination(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> EventDestinationList:
@@ -2974,21 +2889,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-event-destinations-list
         """
         path = "/event_destinations"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return EventDestinationList(self._client, result)
 
     def update(
         self,
         id: str,
         metadata: str = None,
         description: str = None,
@@ -3005,23 +2918,21 @@
 
         https://ngrok.com/docs/api#api-event-destinations-update
         """
         path = "/event_destinations/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                metadata=metadata,
-                description=description,
-                format=format,
-                target=target,
-            ),
+        body_arg = dict(
+            metadata=metadata,
+            description=description,
+            format=format,
+            target=extract_props(target),
         )
+        result = self._client.http_client.patch(path, body_arg)
         return EventDestination(self._client, result)
 
 
 class EventSubscriptionsClient(object):
     def __init__(self, client):
         self._client = client
 
@@ -3038,23 +2949,21 @@
         :param description: Arbitrary customer supplied information intended to be human readable. Optional, max 255 chars.
         :param sources: Sources containing the types for which this event subscription will trigger
         :param destination_ids: A list of Event Destination IDs which should be used for this Event Subscription.
 
         https://ngrok.com/docs/api#api-event-subscriptions-create
         """
         path = "/event_subscriptions"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                metadata=metadata,
-                description=description,
-                sources=sources,
-                destination_ids=destination_ids,
-            ),
+        body_arg = dict(
+            metadata=metadata,
+            description=description,
+            sources=[extract_props(item) for item in sources or []],
+            destination_ids=destination_ids,
         )
+        result = self._client.http_client.post(path, body_arg)
         return EventSubscription(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an Event Subscription.
@@ -3063,15 +2972,16 @@
 
         https://ngrok.com/docs/api#api-event-subscriptions-delete
         """
         path = "/event_subscriptions/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> EventSubscription:
         """Get an Event Subscription by ID.
 
@@ -3079,15 +2989,16 @@
 
         https://ngrok.com/docs/api#api-event-subscriptions-get
         """
         path = "/event_subscriptions/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EventSubscription(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> EventSubscriptionList:
@@ -3095,21 +3006,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-event-subscriptions-list
         """
         path = "/event_subscriptions"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return EventSubscriptionList(self._client, result)
 
     def update(
         self,
         id: str,
         metadata: str = None,
         description: str = None,
@@ -3126,23 +3035,21 @@
 
         https://ngrok.com/docs/api#api-event-subscriptions-update
         """
         path = "/event_subscriptions/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                metadata=metadata,
-                description=description,
-                sources=sources,
-                destination_ids=destination_ids,
-            ),
+        body_arg = dict(
+            metadata=metadata,
+            description=description,
+            sources=[extract_props(item) for item in sources or []],
+            destination_ids=destination_ids,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return EventSubscription(self._client, result)
 
 
 class EventSourcesClient(object):
     def __init__(self, client):
         self._client = client
 
@@ -3158,20 +3065,18 @@
 
         https://ngrok.com/docs/api#api-event-sources-create
         """
         path = "/event_subscriptions/{subscription_id}/sources"
         path = path.format(
             subscription_id=subscription_id,
         )
-        result = self._client.http_client.post(
-            path,
-            dict(
-                type=type,
-            ),
+        body_arg = dict(
+            type=type,
         )
+        result = self._client.http_client.post(path, body_arg)
         return EventSource(self._client, result)
 
     def delete(
         self,
         subscription_id: str,
         type: str,
     ):
@@ -3183,15 +3088,16 @@
         https://ngrok.com/docs/api#api-event-sources-delete
         """
         path = "/event_subscriptions/{subscription_id}/sources/{type}"
         path = path.format(
             subscription_id=subscription_id,
             type=type,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         subscription_id: str,
         type: str,
     ) -> EventSource:
         """Get the details for a given type that triggers for the given event subscription
@@ -3202,15 +3108,16 @@
         https://ngrok.com/docs/api#api-event-sources-get
         """
         path = "/event_subscriptions/{subscription_id}/sources/{type}"
         path = path.format(
             subscription_id=subscription_id,
             type=type,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EventSource(self._client, result)
 
     def list(
         self,
         subscription_id: str,
     ) -> EventSourceList:
         """List the types for which this event subscription will trigger
@@ -3219,15 +3126,16 @@
 
         https://ngrok.com/docs/api#api-event-sources-list
         """
         path = "/event_subscriptions/{subscription_id}/sources"
         path = path.format(
             subscription_id=subscription_id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return EventSourceList(self._client, result)
 
     def update(
         self,
         subscription_id: str,
         type: str,
     ) -> EventSource:
@@ -3239,15 +3147,16 @@
         https://ngrok.com/docs/api#api-event-sources-update
         """
         path = "/event_subscriptions/{subscription_id}/sources/{type}"
         path = path.format(
             subscription_id=subscription_id,
             type=type,
         )
-        result = self._client.http_client.patch(path, dict())
+        body_arg = None
+        result = self._client.http_client.patch(path, body_arg)
         return EventSource(self._client, result)
 
 
 class IPPoliciesClient(object):
     """IP Policies are reusable groups of CIDR ranges with an ``allow`` or ``deny``
     action. They can be attached to endpoints via the Endpoint Configuration IP
     Policy module. They can also be used with IP Restrictions to control source
@@ -3265,21 +3174,19 @@
 
         :param description: human-readable description of the source IPs of this IP policy. optional, max 255 bytes.
         :param metadata: arbitrary user-defined machine-readable data of this IP policy. optional, max 4096 bytes.
 
         https://ngrok.com/docs/api#api-ip-policies-create
         """
         path = "/ip_policies"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.post(path, body_arg)
         return IPPolicy(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an IP policy. If the IP policy is referenced by another object for the purposes of traffic restriction it will be treated as if the IP policy remains but has zero rules.
@@ -3288,15 +3195,16 @@
 
         https://ngrok.com/docs/api#api-ip-policies-delete
         """
         path = "/ip_policies/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> IPPolicy:
         """Get detailed information about an IP policy by ID.
 
@@ -3304,15 +3212,16 @@
 
         https://ngrok.com/docs/api#api-ip-policies-get
         """
         path = "/ip_policies/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return IPPolicy(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> IPPolicyList:
@@ -3320,21 +3229,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-ip-policies-list
         """
         path = "/ip_policies"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return IPPolicyList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -3347,21 +3254,19 @@
 
         https://ngrok.com/docs/api#api-ip-policies-update
         """
         path = "/ip_policies/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return IPPolicy(self._client, result)
 
 
 class IPPolicyRulesClient(object):
     """IP Policy Rules are the IPv4 or IPv6 CIDRs entries that
     make up an IP Policy."""
 
@@ -3383,24 +3288,22 @@
         :param cidr: an IP or IP range specified in CIDR notation. IPv4 and IPv6 are both supported.
         :param ip_policy_id: ID of the IP policy this IP policy rule will be attached to
         :param action: the action to apply to the policy rule, either ``allow`` or ``deny``
 
         https://ngrok.com/docs/api#api-ip-policy-rules-create
         """
         path = "/ip_policy_rules"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                cidr=cidr,
-                ip_policy_id=ip_policy_id,
-                action=action,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            cidr=cidr,
+            ip_policy_id=ip_policy_id,
+            action=action,
         )
+        result = self._client.http_client.post(path, body_arg)
         return IPPolicyRule(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an IP policy rule.
@@ -3409,15 +3312,16 @@
 
         https://ngrok.com/docs/api#api-ip-policy-rules-delete
         """
         path = "/ip_policy_rules/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> IPPolicyRule:
         """Get detailed information about an IP policy rule by ID.
 
@@ -3425,15 +3329,16 @@
 
         https://ngrok.com/docs/api#api-ip-policy-rules-get
         """
         path = "/ip_policy_rules/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return IPPolicyRule(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> IPPolicyRuleList:
@@ -3441,21 +3346,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-ip-policy-rules-list
         """
         path = "/ip_policy_rules"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return IPPolicyRuleList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -3470,22 +3373,20 @@
 
         https://ngrok.com/docs/api#api-ip-policy-rules-update
         """
         path = "/ip_policy_rules/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                cidr=cidr,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            cidr=cidr,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return IPPolicyRule(self._client, result)
 
 
 class IPRestrictionsClient(object):
     """An IP restriction is a restriction placed on the CIDRs that are allowed to
     initiate traffic to a specific aspect of your ngrok account. An IP
     restriction has a type which defines the ingress it applies to. IP
@@ -3511,24 +3412,22 @@
         :param enforced: true if the IP restriction will be enforced. if false, only warnings will be issued
         :param type: the type of IP restriction. this defines what traffic will be restricted with the attached policies. four values are currently supported: ``dashboard``, ``api``, ``agent``, and ``endpoints``
         :param ip_policy_ids: the set of IP policy identifiers that are used to enforce the restriction
 
         https://ngrok.com/docs/api#api-ip-restrictions-create
         """
         path = "/ip_restrictions"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                enforced=enforced,
-                type=type,
-                ip_policy_ids=ip_policy_ids,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            enforced=enforced,
+            type=type,
+            ip_policy_ids=ip_policy_ids,
         )
+        result = self._client.http_client.post(path, body_arg)
         return IPRestriction(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an IP restriction
@@ -3537,15 +3436,16 @@
 
         https://ngrok.com/docs/api#api-ip-restrictions-delete
         """
         path = "/ip_restrictions/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> IPRestriction:
         """Get detailed information about an IP restriction
 
@@ -3553,15 +3453,16 @@
 
         https://ngrok.com/docs/api#api-ip-restrictions-get
         """
         path = "/ip_restrictions/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return IPRestriction(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> IPRestrictionList:
@@ -3569,21 +3470,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-ip-restrictions-list
         """
         path = "/ip_restrictions"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return IPRestrictionList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -3600,23 +3499,21 @@
 
         https://ngrok.com/docs/api#api-ip-restrictions-update
         """
         path = "/ip_restrictions/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                enforced=enforced,
-                ip_policy_ids=ip_policy_ids,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            enforced=enforced,
+            ip_policy_ids=ip_policy_ids,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return IPRestriction(self._client, result)
 
 
 class ReservedAddrsClient(object):
     """Reserved Addresses are TCP addresses that can be used to listen for traffic.
     TCP address hostnames and ports are assigned by ngrok, they cannot be
     chosen."""
@@ -3635,22 +3532,20 @@
         :param description: human-readable description of what this reserved address will be used for
         :param metadata: arbitrary user-defined machine-readable data of this reserved address. Optional, max 4096 bytes.
         :param region: reserve the address in this geographic ngrok datacenter. Optional, default is us. (au, eu, ap, us, jp, in, sa)
 
         https://ngrok.com/docs/api#api-reserved-addrs-create
         """
         path = "/reserved_addrs"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                region=region,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            region=region,
         )
+        result = self._client.http_client.post(path, body_arg)
         return ReservedAddr(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete a reserved address.
@@ -3659,15 +3554,16 @@
 
         https://ngrok.com/docs/api#api-reserved-addrs-delete
         """
         path = "/reserved_addrs/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> ReservedAddr:
         """Get the details of a reserved address.
 
@@ -3675,15 +3571,16 @@
 
         https://ngrok.com/docs/api#api-reserved-addrs-get
         """
         path = "/reserved_addrs/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return ReservedAddr(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> ReservedAddrList:
@@ -3691,21 +3588,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-reserved-addrs-list
         """
         path = "/reserved_addrs"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return ReservedAddrList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -3718,21 +3613,19 @@
 
         https://ngrok.com/docs/api#api-reserved-addrs-update
         """
         path = "/reserved_addrs/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return ReservedAddr(self._client, result)
 
 
 class ReservedDomainsClient(object):
     """Reserved Domains are hostnames that you can listen for traffic on. Domains
     can be used to listen for http, https or tls traffic. You may use a domain
     that you own by creating a CNAME record specified in the returned resource.
@@ -3758,25 +3651,23 @@
         :param metadata: arbitrary user-defined machine-readable data of this reserved domain. Optional, max 4096 bytes.
         :param certificate_id: ID of a user-uploaded TLS certificate to use for connections to targeting this domain. Optional, mutually exclusive with ``certificate_management_policy``.
         :param certificate_management_policy: configuration for automatic management of TLS certificates for this domain, or null if automatic management is disabled. Optional, mutually exclusive with ``certificate_id``.
 
         https://ngrok.com/docs/api#api-reserved-domains-create
         """
         path = "/reserved_domains"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                name=name,
-                region=region,
-                description=description,
-                metadata=metadata,
-                certificate_id=certificate_id,
-                certificate_management_policy=certificate_management_policy,
-            ),
+        body_arg = dict(
+            name=name,
+            region=region,
+            description=description,
+            metadata=metadata,
+            certificate_id=certificate_id,
+            certificate_management_policy=extract_props(certificate_management_policy),
         )
+        result = self._client.http_client.post(path, body_arg)
         return ReservedDomain(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete a reserved domain.
@@ -3785,15 +3676,16 @@
 
         https://ngrok.com/docs/api#api-reserved-domains-delete
         """
         path = "/reserved_domains/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> ReservedDomain:
         """Get the details of a reserved domain.
 
@@ -3801,15 +3693,16 @@
 
         https://ngrok.com/docs/api#api-reserved-domains-get
         """
         path = "/reserved_domains/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return ReservedDomain(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> ReservedDomainList:
@@ -3817,21 +3710,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-reserved-domains-list
         """
         path = "/reserved_domains"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return ReservedDomainList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -3848,23 +3739,21 @@
 
         https://ngrok.com/docs/api#api-reserved-domains-update
         """
         path = "/reserved_domains/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                certificate_id=certificate_id,
-                certificate_management_policy=certificate_management_policy,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            certificate_id=certificate_id,
+            certificate_management_policy=extract_props(certificate_management_policy),
         )
+        result = self._client.http_client.patch(path, body_arg)
         return ReservedDomain(self._client, result)
 
     def delete_certificate_management_policy(
         self,
         id: str,
     ):
         """Detach the certificate management policy attached to a reserved domain.
@@ -3873,15 +3762,16 @@
 
         https://ngrok.com/docs/api#api-reserved-domains-delete-certificate-management-policy
         """
         path = "/reserved_domains/{id}/certificate_management_policy"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def delete_certificate(
         self,
         id: str,
     ):
         """Detach the certificate attached to a reserved domain.
 
@@ -3889,15 +3779,16 @@
 
         https://ngrok.com/docs/api#api-reserved-domains-delete-certificate
         """
         path = "/reserved_domains/{id}/certificate"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
 
 class SSHCertificateAuthoritiesClient(object):
     """An SSH Certificate Authority is a pair of an SSH Certificate and its private
     key that can be used to sign other SSH host and user certificates."""
 
     def __init__(self, client):
@@ -3918,24 +3809,22 @@
         :param private_key_type: the type of private key to generate. one of ``rsa``, ``ecdsa``, ``ed25519``
         :param elliptic_curve: the type of elliptic curve to use when creating an ECDSA key
         :param key_size: the key size to use when creating an RSA key. one of ``2048`` or ``4096``
 
         https://ngrok.com/docs/api#api-ssh-certificate-authorities-create
         """
         path = "/ssh_certificate_authorities"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                private_key_type=private_key_type,
-                elliptic_curve=elliptic_curve,
-                key_size=key_size,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            private_key_type=private_key_type,
+            elliptic_curve=elliptic_curve,
+            key_size=key_size,
         )
+        result = self._client.http_client.post(path, body_arg)
         return SSHCertificateAuthority(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an SSH Certificate Authority
@@ -3944,15 +3833,16 @@
 
         https://ngrok.com/docs/api#api-ssh-certificate-authorities-delete
         """
         path = "/ssh_certificate_authorities/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> SSHCertificateAuthority:
         """Get detailed information about an SSH Certficate Authority
 
@@ -3960,15 +3850,16 @@
 
         https://ngrok.com/docs/api#api-ssh-certificate-authorities-get
         """
         path = "/ssh_certificate_authorities/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return SSHCertificateAuthority(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> SSHCertificateAuthorityList:
@@ -3976,21 +3867,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-ssh-certificate-authorities-list
         """
         path = "/ssh_certificate_authorities"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return SSHCertificateAuthorityList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -4003,21 +3892,19 @@
 
         https://ngrok.com/docs/api#api-ssh-certificate-authorities-update
         """
         path = "/ssh_certificate_authorities/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return SSHCertificateAuthority(self._client, result)
 
 
 class SSHCredentialsClient(object):
     """SSH Credentials are SSH public keys that can be used to start SSH tunnels
     via the ngrok SSH tunnel gateway."""
 
@@ -4037,23 +3924,21 @@
         :param metadata: arbitrary user-defined machine-readable data of this ssh credential. Optional, max 4096 bytes.
         :param acl: optional list of ACL rules. If unspecified, the credential will have no restrictions. The only allowed ACL rule at this time is the ``bind`` rule. The ``bind`` rule allows the caller to restrict what domains and addresses the token is allowed to bind. For example, to allow the token to open a tunnel on example.ngrok.io your ACL would include the rule ``bind:example.ngrok.io``. Bind rules may specify a leading wildcard to match multiple domains with a common suffix. For example, you may specify a rule of ``bind:*.example.com`` which will allow ``x.example.com``, ``y.example.com``, ``*.example.com``, etc. A rule of ``'*'`` is equivalent to no acl at all and will explicitly permit all actions.
         :param public_key: the PEM-encoded public key of the SSH keypair that will be used to authenticate
 
         https://ngrok.com/docs/api#api-ssh-credentials-create
         """
         path = "/ssh_credentials"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                acl=acl,
-                public_key=public_key,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            acl=acl,
+            public_key=public_key,
         )
+        result = self._client.http_client.post(path, body_arg)
         return SSHCredential(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an ssh_credential by ID
@@ -4062,15 +3947,16 @@
 
         https://ngrok.com/docs/api#api-ssh-credentials-delete
         """
         path = "/ssh_credentials/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> SSHCredential:
         """Get detailed information about an ssh_credential
 
@@ -4078,15 +3964,16 @@
 
         https://ngrok.com/docs/api#api-ssh-credentials-get
         """
         path = "/ssh_credentials/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return SSHCredential(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> SSHCredentialList:
@@ -4094,21 +3981,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-ssh-credentials-list
         """
         path = "/ssh_credentials"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return SSHCredentialList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -4123,22 +4008,20 @@
 
         https://ngrok.com/docs/api#api-ssh-credentials-update
         """
         path = "/ssh_credentials/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                acl=acl,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            acl=acl,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return SSHCredential(self._client, result)
 
 
 class SSHHostCertificatesClient(object):
     """SSH Host Certificates along with the corresponding private key allows an SSH
     server to assert its authenticity to connecting SSH clients who trust the
     SSH Certificate Authority that was used to sign the certificate."""
@@ -4165,26 +4048,24 @@
         :param valid_until: The time when this host certificate becomes invalid, in RFC 3339 format. If unspecified, a default value of one year in the future will be used. The OpenSSH certificates RFC calls this ``valid_before``.
         :param description: human-readable description of this SSH Host Certificate. optional, max 255 bytes.
         :param metadata: arbitrary user-defined machine-readable data of this SSH Host Certificate. optional, max 4096 bytes.
 
         https://ngrok.com/docs/api#api-ssh-host-certificates-create
         """
         path = "/ssh_host_certificates"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                ssh_certificate_authority_id=ssh_certificate_authority_id,
-                public_key=public_key,
-                principals=principals,
-                valid_after=valid_after,
-                valid_until=valid_until,
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            ssh_certificate_authority_id=ssh_certificate_authority_id,
+            public_key=public_key,
+            principals=principals,
+            valid_after=valid_after,
+            valid_until=valid_until,
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.post(path, body_arg)
         return SSHHostCertificate(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an SSH Host Certificate
@@ -4193,15 +4074,16 @@
 
         https://ngrok.com/docs/api#api-ssh-host-certificates-delete
         """
         path = "/ssh_host_certificates/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> SSHHostCertificate:
         """Get detailed information about an SSH Host Certficate
 
@@ -4209,15 +4091,16 @@
 
         https://ngrok.com/docs/api#api-ssh-host-certificates-get
         """
         path = "/ssh_host_certificates/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return SSHHostCertificate(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> SSHHostCertificateList:
@@ -4225,21 +4108,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-ssh-host-certificates-list
         """
         path = "/ssh_host_certificates"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return SSHHostCertificateList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -4252,21 +4133,19 @@
 
         https://ngrok.com/docs/api#api-ssh-host-certificates-update
         """
         path = "/ssh_host_certificates/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return SSHHostCertificate(self._client, result)
 
 
 class SSHUserCertificatesClient(object):
     """SSH User Certificates are presented by SSH clients when connecting to an SSH
     server to authenticate their connection. The SSH server must trust the SSH
     Certificate Authority used to sign the certificate."""
@@ -4286,39 +4165,37 @@
         description: str = "",
         metadata: str = "",
     ) -> SSHUserCertificate:
         """Create a new SSH User Certificate
 
         :param ssh_certificate_authority_id: the ssh certificate authority that is used to sign this ssh user certificate
         :param public_key: a public key in OpenSSH Authorized Keys format that this certificate signs
-        :param principals: the list of principals included in the ssh user certificate. This is the list of usernames that the certificate holder may sign in as on a machine authorizinig the signing certificate authority. Dangerously, if no principals are specified, this certificate may be used to log in as any user.
+        :param principals: the list of principals included in the ssh user certificate. This is the list of usernames that the certificate holder may sign in as on a machine authorizing the signing certificate authority. Dangerously, if no principals are specified, this certificate may be used to log in as any user.
         :param critical_options: A map of critical options included in the certificate. Only two critical options are currently defined by OpenSSH: ``force-command`` and ``source-address``. See `the OpenSSH certificate protocol spec` <https://github.com/openssh/openssh-portable/blob/master/PROTOCOL.certkeys>`_ for additional details.
         :param extensions: A map of extensions included in the certificate. Extensions are additional metadata that can be interpreted by the SSH server for any purpose. These can be used to permit or deny the ability to open a terminal, do port forwarding, x11 forwarding, and more. If unspecified, the certificate will include limited permissions with the following extension map: ``{"permit-pty": "", "permit-user-rc": ""}`` OpenSSH understands a number of predefined extensions. See `the OpenSSH certificate protocol spec` <https://github.com/openssh/openssh-portable/blob/master/PROTOCOL.certkeys>`_ for additional details.
         :param valid_after: The time when the user certificate becomes valid, in RFC 3339 format. Defaults to the current time if unspecified.
         :param valid_until: The time when this host certificate becomes invalid, in RFC 3339 format. If unspecified, a default value of 24 hours will be used. The OpenSSH certificates RFC calls this ``valid_before``.
         :param description: human-readable description of this SSH User Certificate. optional, max 255 bytes.
         :param metadata: arbitrary user-defined machine-readable data of this SSH User Certificate. optional, max 4096 bytes.
 
         https://ngrok.com/docs/api#api-ssh-user-certificates-create
         """
         path = "/ssh_user_certificates"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                ssh_certificate_authority_id=ssh_certificate_authority_id,
-                public_key=public_key,
-                principals=principals,
-                critical_options=critical_options,
-                extensions=extensions,
-                valid_after=valid_after,
-                valid_until=valid_until,
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            ssh_certificate_authority_id=ssh_certificate_authority_id,
+            public_key=public_key,
+            principals=principals,
+            critical_options=critical_options,
+            extensions=extensions,
+            valid_after=valid_after,
+            valid_until=valid_until,
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.post(path, body_arg)
         return SSHUserCertificate(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete an SSH User Certificate
@@ -4327,15 +4204,16 @@
 
         https://ngrok.com/docs/api#api-ssh-user-certificates-delete
         """
         path = "/ssh_user_certificates/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> SSHUserCertificate:
         """Get detailed information about an SSH User Certficate
 
@@ -4343,15 +4221,16 @@
 
         https://ngrok.com/docs/api#api-ssh-user-certificates-get
         """
         path = "/ssh_user_certificates/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return SSHUserCertificate(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> SSHUserCertificateList:
@@ -4359,21 +4238,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-ssh-user-certificates-list
         """
         path = "/ssh_user_certificates"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return SSHUserCertificateList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -4386,21 +4263,19 @@
 
         https://ngrok.com/docs/api#api-ssh-user-certificates-update
         """
         path = "/ssh_user_certificates/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return SSHUserCertificate(self._client, result)
 
 
 class TLSCertificatesClient(object):
     """TLS Certificates are pairs of x509 certificates and their matching private
     key that can be used to terminate TLS traffic. TLS certificates are unused
     until they are attached to a Domain. TLS Certificates may also be
@@ -4423,23 +4298,21 @@
         :param metadata: arbitrary user-defined machine-readable data of this TLS certificate. optional, max 4096 bytes.
         :param certificate_pem: chain of PEM-encoded certificates, leaf first. See `Certificate Bundles` <https://ngrok.com/docs/api#tls-certificates-pem>`_.
         :param private_key_pem: private key for the TLS certificate, PEM-encoded. See `Private Keys` <https://ngrok.com/docs/ngrok-link#tls-certificates-key>`_.
 
         https://ngrok.com/docs/api#api-tls-certificates-create
         """
         path = "/tls_certificates"
-        result = self._client.http_client.post(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-                certificate_pem=certificate_pem,
-                private_key_pem=private_key_pem,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
+            certificate_pem=certificate_pem,
+            private_key_pem=private_key_pem,
         )
+        result = self._client.http_client.post(path, body_arg)
         return TLSCertificate(self._client, result)
 
     def delete(
         self,
         id: str,
     ):
         """Delete a TLS certificate
@@ -4448,15 +4321,16 @@
 
         https://ngrok.com/docs/api#api-tls-certificates-delete
         """
         path = "/tls_certificates/{id}"
         path = path.format(
             id=id,
         )
-        self._client.http_client.delete(path, dict())
+        body_arg = None
+        self._client.http_client.delete(path, body_arg)
 
     def get(
         self,
         id: str,
     ) -> TLSCertificate:
         """Get detailed information about a TLS certificate
 
@@ -4464,15 +4338,16 @@
 
         https://ngrok.com/docs/api#api-tls-certificates-get
         """
         path = "/tls_certificates/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return TLSCertificate(self._client, result)
 
     def list(
         self,
         before_id: str = None,
         limit: str = None,
     ) -> TLSCertificateList:
@@ -4480,21 +4355,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-tls-certificates-list
         """
         path = "/tls_certificates"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return TLSCertificateList(self._client, result)
 
     def update(
         self,
         id: str,
         description: str = None,
         metadata: str = None,
@@ -4507,21 +4380,19 @@
 
         https://ngrok.com/docs/api#api-tls-certificates-update
         """
         path = "/tls_certificates/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.patch(
-            path,
-            dict(
-                description=description,
-                metadata=metadata,
-            ),
+        body_arg = dict(
+            description=description,
+            metadata=metadata,
         )
+        result = self._client.http_client.patch(path, body_arg)
         return TLSCertificate(self._client, result)
 
 
 class TunnelSessionsClient(object):
     """Tunnel Sessions represent instances of ngrok agents or SSH reverse tunnel
     sessions that are running and connected to the ngrok service. Each tunnel
     session can include one or more Tunnels."""
@@ -4538,21 +4409,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-tunnel-sessions-list
         """
         path = "/tunnel_sessions"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return TunnelSessionList(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> TunnelSession:
         """Get the detailed status of a tunnel session by ID
@@ -4561,15 +4430,16 @@
 
         https://ngrok.com/docs/api#api-tunnel-sessions-get
         """
         path = "/tunnel_sessions/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return TunnelSession(self._client, result)
 
     def restart(
         self,
         id: str,
     ):
         """Issues a command instructing the ngrok agent to restart. The agent restarts itself by calling exec() on platforms that support it. This operation is notably not supported on Windows. When an agent restarts, it reconnects with a new tunnel session ID.
@@ -4578,15 +4448,16 @@
 
         https://ngrok.com/docs/api#api-tunnel-sessions-restart
         """
         path = "/tunnel_sessions/{id}/restart"
         path = path.format(
             id=id,
         )
-        self._client.http_client.post(path, dict())
+        body_arg = None
+        self._client.http_client.post(path, body_arg)
 
     def stop(
         self,
         id: str,
     ):
         """Issues a command instructing the ngrok agent that started this tunnel session to exit.
 
@@ -4594,15 +4465,16 @@
 
         https://ngrok.com/docs/api#api-tunnel-sessions-stop
         """
         path = "/tunnel_sessions/{id}/stop"
         path = path.format(
             id=id,
         )
-        self._client.http_client.post(path, dict())
+        body_arg = None
+        self._client.http_client.post(path, body_arg)
 
     def update(
         self,
         id: str,
     ):
         """Issues a command instructing the ngrok agent to update itself to the latest version. After this call completes successfully, the ngrok agent will be in the update process. A caller should wait some amount of time to allow the update to complete (at least 10 seconds) before making a call to the Restart endpoint to request that the agent restart itself to start using the new code. This call will never update an ngrok agent to a new major version which could cause breaking compatibility issues. If you wish to update to a new major version, that must be done manually. Still, please be aware that updating your ngrok agent could break your integration. This call will fail in any of the following circumstances: there is no update available the ngrok agent's configuration disabled update checks the agent is currently in process of updating the agent has already successfully updated but has not yet been restarted
 
@@ -4610,15 +4482,16 @@
 
         https://ngrok.com/docs/api#api-tunnel-sessions-update
         """
         path = "/tunnel_sessions/{id}/update"
         path = path.format(
             id=id,
         )
-        self._client.http_client.post(path, dict())
+        body_arg = None
+        self._client.http_client.post(path, body_arg)
 
 
 class TunnelsClient(object):
     """Tunnels provide endpoints to access services exposed by a running ngrok
     agent tunnel session or an SSH reverse tunnel session."""
 
     def __init__(self, client):
@@ -4633,21 +4506,19 @@
 
         :param before_id:
         :param limit:
 
         https://ngrok.com/docs/api#api-tunnels-list
         """
         path = "/tunnels"
-        result = self._client.http_client.get(
-            path,
-            dict(
-                before_id=before_id,
-                limit=limit,
-            ),
+        body_arg = dict(
+            before_id=before_id,
+            limit=limit,
         )
+        result = self._client.http_client.get(path, body_arg)
         return TunnelList(self._client, result)
 
     def get(
         self,
         id: str,
     ) -> Tunnel:
         """Get the status of a tunnel by ID
@@ -4656,9 +4527,10 @@
 
         https://ngrok.com/docs/api#api-tunnels-get
         """
         path = "/tunnels/{id}"
         path = path.format(
             id=id,
         )
-        result = self._client.http_client.get(path, dict())
+        body_arg = None
+        result = self._client.http_client.get(path, body_arg)
         return Tunnel(self._client, result)
```

### Comparing `ngrok-api-0.6.0/ngrok_api.egg-info/PKG-INFO` & `ngrok-api-0.8.0/ngrok_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngrok-api
-Version: 0.6.0
+Version: 0.8.0
 Summary: ngrok HTTP API client library
 Home-page: https://github.com/ngrok/ngrok-api-python
 Author: Alan Shreve
 Author-email: alan@ngrok.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,21 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tox
 Provides-Extra: doc
 License-File: LICENSE
 
+# Unstable
+
+This library is currently unstable. We know of rough edges
+and are working to bring it to parity with our other API client
+libraries. Please feel free to try it out and let us know if you find
+it useful!
+
 # ngrok API client library for Python
 
 This library wraps the [ngrok HTTP API](https://ngrok.com/docs/api) to make it
 easier to consume in Python.
 
 ## Installation
 
@@ -34,19 +41,19 @@
 ## Quickstart
 
 Please consult the [documentation](https://python-api.docs.ngrok.com) for additional examples.
 
     import ngrok
 
     # construct the api client
-    ng = ngrok.Client("<API KEY>")
+    client = ngrok.Client("<API KEY>")
 
     # list all online tunnels
-    for t in ng.tunnels.list():
+    for t in client.tunnels.list():
         print(t)
 
-    # create an ip policy the allows traffic from some subnets
-    policy = ng.ip_policies.create(action="allow")
+    # create an ip policy that allows traffic from some subnets
+    policy = client.ip_policies.create()
     for cidr in ["24.0.0.0/8", "12.0.0.0/8"]:
-        ng.ip_policy_rules.create(cidr=cidr, ip_policy_id=policy.id)
+        client.ip_policy_rules.create(cidr=cidr, ip_policy_id=policy.id, action="allow")
```

### Comparing `ngrok-api-0.6.0/setup.py` & `ngrok-api-0.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_file(filename):
     path = os.path.join(os.path.dirname(__file__), filename)
     with open(path) as f:
         return f.read()
 
 setup(
     name="ngrok-api",
-    version="0.6.0",
+    version="0.8.0",
     description="ngrok HTTP API client library",
     long_description=read_file("README.md"),
     long_description_content_type="text/markdown",
     author="Alan Shreve",
     author_email="alan@ngrok.com",
     packages=find_packages(exclude=['tests']),
     package_data={"ngrok": ["py.typed"]},
@@ -25,10 +25,19 @@
     ],
     python_requires=">=3.7",
     install_requires=[
         "requests==2.25.1",
     ],
     extras_require={
         "tox": ["tox==3.23.0"],
-        "doc": ["black==21.5b1", "furo==2021.4.11b34", "sphinx==3.5.4", "sphinx-autodoc-typehints==1.12.0", "sphinx-readable-theme==1.3.0"],
+        "doc": [
+            "black==21.5b1",
+            "click==8.0.4",
+            "furo==2021.4.11b34",
+            "sphinx==3.5.4",
+            "sphinx-autodoc-typehints==1.12.0",
+            "sphinx-readable-theme==1.3.0",
+            # Pin separately for https://github.com/sphinx-doc/sphinx/issues/10291
+            "Jinja2==3.0.3",
+        ],
     }
 )
```

