# Comparing `tmp/dash_websocket_component-0.0.3.tar.gz` & `tmp/dash_websocket_component-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_websocket_component-0.0.3.tar", last modified: Sun Mar 10 23:03:31 2024, max compression
+gzip compressed data, was "dash_websocket_component-0.0.4.tar", last modified: Tue Apr 30 11:20:55 2024, max compression
```

## Comparing `dash_websocket_component-0.0.3.tar` & `dash_websocket_component-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 23:03:31.176498 dash_websocket_component-0.0.3/
--rw-rw-rw-   0        0        0        0 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      484 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4094 2024-03-10 23:03:31.174447 dash_websocket_component-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3837 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-10 23:03:31.159866 dash_websocket_component-0.0.3/dash_websocket_component/
--rw-rw-rw-   0        0        0     2109 2024-03-10 23:00:25.000000 dash_websocket_component-0.0.3/dash_websocket_component/DashWebsocketComponent.py
--rw-rw-rw-   0        0        0     2389 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.3/dash_websocket_component/__init__.py
--rw-rw-rw-   0        0        0      106 2024-03-10 23:00:25.000000 dash_websocket_component-0.0.3/dash_websocket_component/_imports_.py
--rw-rw-rw-   0        0        0     4756 2024-03-10 23:00:23.000000 dash_websocket_component-0.0.3/dash_websocket_component/async-DashWebsocketComponent.js
--rw-rw-rw-   0        0        0     7177 2024-03-10 23:00:23.000000 dash_websocket_component-0.0.3/dash_websocket_component/async-DashWebsocketComponent.js.map
--rw-rw-rw-   0        0        0     4113 2024-03-10 23:00:23.000000 dash_websocket_component-0.0.3/dash_websocket_component/dash_websocket_component.min.js
--rw-rw-rw-   0        0        0    20188 2024-03-10 23:00:23.000000 dash_websocket_component-0.0.3/dash_websocket_component/dash_websocket_component.min.js.map
--rw-rw-rw-   0        0        0     2747 2024-03-10 23:00:25.000000 dash_websocket_component-0.0.3/dash_websocket_component/metadata.json
--rw-rw-rw-   0        0        0     2118 2024-03-10 23:00:24.000000 dash_websocket_component-0.0.3/dash_websocket_component/package-info.json
-drwxrwxrwx   0        0        0        0 2024-03-10 23:03:31.166023 dash_websocket_component-0.0.3/dash_websocket_component.egg-info/
--rw-rw-rw-   0        0        0     4094 2024-03-10 23:03:31.000000 dash_websocket_component-0.0.3/dash_websocket_component.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2024-03-10 23:03:31.000000 dash_websocket_component-0.0.3/dash_websocket_component.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 23:03:31.000000 dash_websocket_component-0.0.3/dash_websocket_component.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-03-10 23:03:31.000000 dash_websocket_component-0.0.3/dash_websocket_component.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2118 2024-03-10 21:31:39.000000 dash_websocket_component-0.0.3/package.json
--rw-rw-rw-   0        0        0       42 2024-03-10 23:03:31.176498 dash_websocket_component-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      721 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-10 23:03:31.166023 dash_websocket_component-0.0.3/tests/
--rw-rw-rw-   0        0        0      945 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.3/tests/test_usage.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:20:55.074930 dash_websocket_component-0.0.4/
+-rw-rw-rw-   0        0        0        0 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      484 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4137 2024-04-30 11:20:55.074930 dash_websocket_component-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3837 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 11:20:55.059924 dash_websocket_component-0.0.4/dash_websocket_component/
+-rw-rw-rw-   0        0        0     2109 2024-04-30 11:11:09.000000 dash_websocket_component-0.0.4/dash_websocket_component/DashWebsocketComponent.py
+-rw-rw-rw-   0        0        0     2389 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.4/dash_websocket_component/__init__.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 11:11:09.000000 dash_websocket_component-0.0.4/dash_websocket_component/_imports_.py
+-rw-rw-rw-   0        0        0     4921 2024-04-30 10:55:39.000000 dash_websocket_component-0.0.4/dash_websocket_component/async-DashWebsocketComponent.js
+-rw-rw-rw-   0        0        0     7336 2024-04-30 10:55:39.000000 dash_websocket_component-0.0.4/dash_websocket_component/async-DashWebsocketComponent.js.map
+-rw-rw-rw-   0        0        0     4113 2024-04-30 10:55:39.000000 dash_websocket_component-0.0.4/dash_websocket_component/dash_websocket_component.min.js
+-rw-rw-rw-   0        0        0    20188 2024-04-30 10:55:39.000000 dash_websocket_component-0.0.4/dash_websocket_component/dash_websocket_component.min.js.map
+-rw-rw-rw-   0        0        0     2747 2024-04-30 11:11:09.000000 dash_websocket_component-0.0.4/dash_websocket_component/metadata.json
+-rw-rw-rw-   0        0        0     2117 2024-04-30 11:11:09.000000 dash_websocket_component-0.0.4/dash_websocket_component/package-info.json
+drwxrwxrwx   0        0        0        0 2024-04-30 11:20:55.071020 dash_websocket_component-0.0.4/dash_websocket_component.egg-info/
+-rw-rw-rw-   0        0        0     4137 2024-04-30 11:20:55.000000 dash_websocket_component-0.0.4/dash_websocket_component.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2024-04-30 11:20:55.000000 dash_websocket_component-0.0.4/dash_websocket_component.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 11:20:55.000000 dash_websocket_component-0.0.4/dash_websocket_component.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-30 11:20:55.000000 dash_websocket_component-0.0.4/dash_websocket_component.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2118 2024-04-30 11:20:46.000000 dash_websocket_component-0.0.4/package.json
+-rw-rw-rw-   0        0        0       42 2024-04-30 11:20:55.075928 dash_websocket_component-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      721 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:20:55.071927 dash_websocket_component-0.0.4/tests/
+-rw-rw-rw-   0        0        0      945 2024-02-23 09:35:19.000000 dash_websocket_component-0.0.4/tests/test_usage.py
```

### Comparing `dash_websocket_component-0.0.3/PKG-INFO` & `dash_websocket_component-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: dash_websocket_component
-Version: 0.0.3
+Version: 0.0.4
 Summary: Project Description
+Home-page: UNKNOWN
 Author: Dominik Tkacik <tkacik38@gmail.com>
 License: MIT
+Platform: UNKNOWN
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dash WebSocket Component
 
 Dash WebSocket Component is a Dash component library.
@@ -102,7 +104,9 @@
         ```
         _Publishing your component to NPM will make the JavaScript bundles available on the unpkg CDN. By default, Dash serves the component library's CSS and JS locally, but if you choose to publish the package to NPM you can set `serve_locally` to `False` and you may see faster load times._
 
 5. Share your component with the community! https://community.plotly.com/c/dash
     1. Publish this repository to GitHub
     2. Tag your GitHub repository with the plotly-dash tag so that it appears here: https://github.com/topics/plotly-dash
     3. Create a post in the Dash community forum: https://community.plotly.com/c/dash
+
+
```

### Comparing `dash_websocket_component-0.0.3/README.md` & `dash_websocket_component-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dash_websocket_component-0.0.3/dash_websocket_component/DashWebsocketComponent.py` & `dash_websocket_component-0.0.4/dash_websocket_component/DashWebsocketComponent.py`

 * *Files identical despite different names*

### Comparing `dash_websocket_component-0.0.3/dash_websocket_component/__init__.py` & `dash_websocket_component-0.0.4/dash_websocket_component/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_websocket_component-0.0.3/dash_websocket_component/async-DashWebsocketComponent.js` & `dash_websocket_component-0.0.4/dash_websocket_component/async-DashWebsocketComponent.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,208 +1,214 @@
 "use strict";
 (self.webpackChunkdash_websocket_component = self.webpackChunkdash_websocket_component || []).push([
     [12], {
         368: (t, e, n) => {
             n.r(e), n.d(e, {
-                default: () => d
+                default: () => m
             });
-            var r = n(609),
-                o = n(120),
-                i = n.n(o);
+            var o = n(609),
+                r = n(120),
+                i = n.n(r);
 
-            function s(t) {
-                return s = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+            function c(t) {
+                return c = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
                     return typeof t
                 } : function(t) {
                     return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
-                }, s(t)
+                }, c(t)
             }
 
-            function c(t, e) {
+            function s(t, e) {
                 var n = Object.keys(t);
                 if (Object.getOwnPropertySymbols) {
-                    var r = Object.getOwnPropertySymbols(t);
-                    e && (r = r.filter((function(e) {
+                    var o = Object.getOwnPropertySymbols(t);
+                    e && (o = o.filter((function(e) {
                         return Object.getOwnPropertyDescriptor(t, e).enumerable
-                    }))), n.push.apply(n, r)
+                    }))), n.push.apply(n, o)
                 }
                 return n
             }
 
             function u(t) {
                 for (var e = 1; e < arguments.length; e++) {
                     var n = null != arguments[e] ? arguments[e] : {};
-                    e % 2 ? c(Object(n), !0).forEach((function(e) {
-                        var r, o, i;
-                        r = t, o = e, i = n[e], (o = p(o)) in r ? Object.defineProperty(r, o, {
+                    e % 2 ? s(Object(n), !0).forEach((function(e) {
+                        var o, r, i;
+                        o = t, r = e, i = n[e], (r = p(r)) in o ? Object.defineProperty(o, r, {
                             value: i,
                             enumerable: !0,
                             configurable: !0,
                             writable: !0
-                        }) : r[o] = i
-                    })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(n)) : c(Object(n)).forEach((function(e) {
+                        }) : o[r] = i
+                    })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(n)) : s(Object(n)).forEach((function(e) {
                         Object.defineProperty(t, e, Object.getOwnPropertyDescriptor(n, e))
                     }))
                 }
                 return t
             }
 
             function a(t, e) {
                 for (var n = 0; n < e.length; n++) {
-                    var r = e[n];
-                    r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(t, p(r.key), r)
+                    var o = e[n];
+                    o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(t, p(o.key), o)
                 }
             }
 
             function p(t) {
                 var e = function(t, e) {
-                    if ("object" != s(t) || !t) return t;
+                    if ("object" != c(t) || !t) return t;
                     var n = t[Symbol.toPrimitive];
                     if (void 0 !== n) {
-                        var r = n.call(t, "string");
-                        if ("object" != s(r)) return r;
+                        var o = n.call(t, "string");
+                        if ("object" != c(o)) return o;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }
                     return String(t)
                 }(t);
-                return "symbol" == s(e) ? e : String(e)
+                return "symbol" == c(e) ? e : String(e)
             }
 
             function l(t, e, n) {
-                return e = b(e),
+                return e = y(e),
                     function(t, e) {
-                        if (e && ("object" === s(e) || "function" == typeof e)) return e;
+                        if (e && ("object" === c(e) || "function" == typeof e)) return e;
                         if (void 0 !== e) throw new TypeError("Derived constructors may only return object or undefined");
                         return function(t) {
                             if (void 0 === t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                             return t
                         }(t)
-                    }(t, f() ? Reflect.construct(e, n || [], b(t).constructor) : e.apply(t, n))
+                    }(t, f() ? Reflect.construct(e, n || [], y(t).constructor) : e.apply(t, n))
             }
 
             function f() {
                 try {
                     var t = !Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {})))
                 } catch (t) {}
                 return (f = function() {
                     return !!t
                 })()
             }
 
-            function b(t) {
-                return b = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(t) {
+            function y(t) {
+                return y = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(t) {
                     return t.__proto__ || Object.getPrototypeOf(t)
-                }, b(t)
+                }, y(t)
             }
 
-            function y(t, e) {
-                return y = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(t, e) {
+            function b(t, e) {
+                return b = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(t, e) {
                     return t.__proto__ = e, t
-                }, y(t, e)
+                }, b(t, e)
             }
-            var d = function(t) {
+            var m = function(t) {
                 function e() {
                     return function(t, e) {
                         if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                     }(this, e), l(this, e, arguments)
                 }
-                var n, r;
+                var n, o;
                 return function(t, e) {
                     if ("function" != typeof e && null !== e) throw new TypeError("Super expression must either be null or a function");
                     t.prototype = Object.create(e && e.prototype, {
                         constructor: {
                             value: t,
                             writable: !0,
                             configurable: !0
                         }
                     }), Object.defineProperty(t, "prototype", {
                         writable: !1
-                    }), e && y(t, e)
-                }(e, t), n = e, (r = [{
+                    }), e && b(t, e)
+                }(e, t), n = e, o = [{
                     key: "_init_client",
-                    value: function() {
+                    value: function(t) {
+                        function e() {
+                            return t.apply(this, arguments)
+                        }
+                        return e.toString = function() {
+                            return t.toString()
+                        }, e
+                    }((function() {
                         var t = this,
                             e = this.props.url,
                             n = this.props.protocols;
                         e = e || "ws://" + location.host + location.pathname + "ws", this.client = new WebSocket(e, n), this.client.onopen = function(e) {
-                            t.props.setProps(u(u({}, t.props), {}, {
+                            t.props.setProps({
                                 state: {
                                     readyState: WebSocket.OPEN,
                                     isTrusted: e.isTrusted,
                                     timeStamp: e.timeStamp,
                                     origin: e.origin,
                                     lastConnected: Number(new Date)
                                 }
-                            }))
+                            })
                         }, this.client.onmessage = function(e) {
-                            t.props.setProps(u(u({}, t.props), {}, {
+                            t.props.setProps({
                                 state: {
                                     lastConnected: Number(new Date)
                                 },
                                 message: {
                                     data: e.data,
                                     isTrusted: e.isTrusted,
                                     origin: e.origin,
                                     timeStamp: e.timeStamp
                                 }
-                            }))
+                            })
                         }, this.client.onerror = function(e) {
-                            t.props.setProps({
+                            console.log("ON ERROR ".concat(location.host)), t.props.setProps({
                                 error: JSON.stringify(e)
                             })
                         }, this.client.onclose = function(e) {
-                            t.props.setProps(u(u({}, t.props), {}, {
+                            console.log("ON CLOSE ".concat(location.host)), t.props.setProps({
                                 error: JSON.stringify(e),
                                 state: {
                                     readyState: WebSocket.CLOSED,
                                     isTrusted: e.isTrusted,
                                     timeStamp: e.timeStamp,
                                     code: e.code,
                                     reason: e.reason,
                                     wasClean: e.wasClean,
                                     lastConnected: Number(new Date)
                                 }
-                            }))
+                            }), setTimeout(_init_client, 1e3)
                         }
-                    }
+                    }))
                 }, {
                     key: "componentDidMount",
                     value: function() {
-                        this.props.setProps({
+                        console.log("Try to load web socket component"), this.props.setProps({
                             state: u(u({}, this.props.state), {}, {
                                 lastConnected: 0
                             })
                         }), this._init_client()
                     }
                 }, {
                     key: "componentDidUpdate",
                     value: function(t) {
-                        this.client.readyState === WebSocket.CLOSED && this._init_client();
                         var e = this.props.send;
-                        e && e !== t.send && this.client.readyState === WebSocket.OPEN && this.client.send(e)
+                        e && e !== t.send && this.props.state.readyState === WebSocket.OPEN && this.client.send(e)
                     }
                 }, {
                     key: "componentWillUnmount",
                     value: function() {
                         this.client.onopen = null, this.client.onclose = null, this.client.onerror = null, this.client.onmessage = null, this.client.close()
                     }
                 }, {
                     key: "render",
                     value: function() {
                         return null
                     }
-                }]) && a(n.prototype, r), Object.defineProperty(n, "prototype", {
+                }], o && a(n.prototype, o), Object.defineProperty(n, "prototype", {
                     writable: !1
                 }), e
-            }(r.Component);
-            d.defaultProps = {
+            }(o.Component);
+            m.defaultProps = {
                 state: {
                     readyState: WebSocket.CONNECTING
                 }
-            }, d.propTypes = {
+            }, m.propTypes = {
                 state: i().oneOfType([i().object, i().string]),
                 message: i().oneOfType([i().object, i().string]),
                 error: i().oneOfType([i().object, i().string]),
                 send: i().oneOfType([i().object, i().string]),
                 url: i().string,
                 protocols: i().arrayOf(i().string),
                 id: i().string,
```

### Comparing `dash_websocket_component-0.0.3/dash_websocket_component/async-DashWebsocketComponent.js.map` & `dash_websocket_component-0.0.4/dash_websocket_component/async-DashWebsocketComponent.js.map`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8444700460829493%*

 * *Differences: {"'mappings'": "'izEACmC,IAEdA,EAAsB,SAAAC,GAAA,SAAAD,IAAA,O,4FAAAE,CAAA,KAAAF,GAAAG,EAAA,KAAAH,EAAAI,UAAA,C,QAoFtC,O,qRApFsCC,CAAAL,EAAAC,G,EAAAD,E,EAAA,EAAAM,IAAA,eAAAC,MAAA,SAAAC,GAAA,SAAAC,IAAA,OAAAD,EAAAE,MAAA,KAAAN,UAAA,QAAAK,EAAAE,SAAA,kBAAAH,EAAAG,UAAA,EAAAF,CAAA,GACvC,WAAe,IAAAG,EAAA,KACNC,EAAOC,KAAKC,MAAZF,IACEG,EAAaF,KAAKC,MAAlBC,UACPH,EAAMA,GAAY,QAAUI,SAASC,KAAOD,SAASE,SAAW,KAChEL,KAAKM,OAAS,IAAIC,UAAUR,EAAKG,GAEjCF,KAAKM,OAAOE,OAAS,SAACC,GAClBX,EAAKG,MAAMS,SAAS,CAChBC,MAAO,CACHC,WAAYL,UAAUM,KAC […]*

```diff
@@ -1,55 +1,62 @@
 {
     "file": "async-DashWebsocketComponent.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "DashWebsocketComponent",
         "_Component",
         "_classCallCheck",
         "_callSuper",
         "arguments",
         "_inherits",
         "key",
         "value",
+        "_init_client2",
+        "_init_client",
+        "apply",
+        "toString",
         "_this",
         "url",
         "this",
         "props",
         "protocols",
         "location",
         "host",
         "pathname",
         "client",
         "WebSocket",
         "onopen",
         "e",
         "setProps",
-        "_objectSpread",
         "state",
         "readyState",
         "OPEN",
         "isTrusted",
         "timeStamp",
         "origin",
         "lastConnected",
         "Number",
         "Date",
         "onmessage",
         "message",
         "data",
         "onerror",
+        "console",
+        "log",
+        "concat",
         "error",
         "JSON",
         "stringify",
         "onclose",
         "CLOSED",
         "code",
         "reason",
         "wasClean",
-        "_init_client",
+        "setTimeout",
+        "_objectSpread",
         "prevProps",
         "send",
         "close",
         "Component",
         "defaultProps",
         "CONNECTING",
         "propTypes",
@@ -57,11 +64,11 @@
         "id"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///./src/lib/fragments/DashWebsocketComponent.react.js"
     ],
     "sourcesContent": [
-        "import {Component} from 'react';\r\nimport PropTypes from 'prop-types';\r\n\r\nexport default class DashWebsocketComponent extends Component {\r\n    _init_client() {\r\n        let {url} = this.props;\r\n        const {protocols} = this.props;\r\n        url = url ? url : 'ws://' + location.host + location.pathname + 'ws';\r\n        this.client = new WebSocket(url, protocols);\r\n\r\n        this.client.onopen = (e) => {\r\n            this.props.setProps({\r\n                ...this.props,\r\n                state: {\r\n                    readyState: WebSocket.OPEN,\r\n                    isTrusted: e.isTrusted,\r\n                    timeStamp: e.timeStamp,\r\n                    origin: e.origin,\r\n                    lastConnected: Number(new Date()),\r\n                },\r\n            });\r\n        };\r\n        this.client.onmessage = (e) => {\r\n            this.props.setProps({\r\n                ...this.props,\r\n                state: {\r\n                    lastConnected: Number(new Date()),\r\n                },\r\n                message: {\r\n                    data: e.data,\r\n                    isTrusted: e.isTrusted,\r\n                    origin: e.origin,\r\n                    timeStamp: e.timeStamp,\r\n                },\r\n            });\r\n        };\r\n        this.client.onerror = (e) => {\r\n            this.props.setProps({error: JSON.stringify(e)});\r\n        };\r\n        this.client.onclose = (e) => {\r\n            this.props.setProps({\r\n                ...this.props,\r\n                error: JSON.stringify(e),\r\n                state: {\r\n                    readyState: WebSocket.CLOSED,\r\n                    isTrusted: e.isTrusted,\r\n                    timeStamp: e.timeStamp,\r\n                    code: e.code,\r\n                    reason: e.reason,\r\n                    wasClean: e.wasClean,\r\n                    lastConnected: Number(new Date()),\r\n                },\r\n            });\r\n        };\r\n    }\r\n\r\n    componentDidMount() {\r\n        this.props.setProps({\r\n            state: {\r\n                ...this.props.state,\r\n                lastConnected: 0,\r\n            },\r\n        });\r\n        this._init_client();\r\n    }\r\n\r\n    componentDidUpdate(prevProps) {\r\n        if (this.client.readyState === WebSocket.CLOSED) {\r\n            this._init_client();\r\n        }\r\n\r\n        const {send} = this.props;\r\n        if (send && send !== prevProps.send) {\r\n            if (this.client.readyState === WebSocket.OPEN) {\r\n                this.client.send(send);\r\n            }\r\n            // TODO handle this\r\n        }\r\n    }\r\n\r\n    componentWillUnmount() {\r\n        this.client.onopen = null;\r\n        this.client.onclose = null;\r\n        this.client.onerror = null;\r\n        this.client.onmessage = null;\r\n        this.client.close();\r\n    }\r\n\r\n    render() {\r\n        return null;\r\n    }\r\n}\r\n\r\nDashWebsocketComponent.defaultProps = {\r\n    state: {readyState: WebSocket.CONNECTING},\r\n};\r\n\r\nDashWebsocketComponent.propTypes = {\r\n    /**\r\n     * This websocket state (in the readyState prop) and associated information.\r\n     */\r\n    state: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * When messages are received, this property is updated with the message content.\r\n     */\r\n    message: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * This property is set with the content of the onerror event.\r\n     */\r\n    error: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * When this property is set, a message is sent with its content.\r\n     */\r\n    send: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * The websocket endpoint (e.g. wss://echo.websocket.org).\r\n     */\r\n    url: PropTypes.string,\r\n\r\n    /**\r\n     * Supported websocket protocols (optional).\r\n     */\r\n    protocols: PropTypes.arrayOf(PropTypes.string),\r\n\r\n    /**\r\n     * The ID used to identify this component in Dash callbacks.\r\n     */\r\n    id: PropTypes.string,\r\n\r\n    /**\r\n     * Dash-assigned callback that should be called to report property changes\r\n     * to Dash, to make them available for callbacks.\r\n     */\r\n    setProps: PropTypes.func,\r\n};\r\n"
+        "import {Component} from 'react';\r\nimport PropTypes from 'prop-types';\r\n\r\nexport default class DashWebsocketComponent extends Component {\r\n    _init_client() {\r\n        let {url} = this.props;\r\n        const {protocols} = this.props;\r\n        url = url ? url : 'ws://' + location.host + location.pathname + 'ws';\r\n        this.client = new WebSocket(url, protocols);\r\n\r\n        this.client.onopen = (e) => {\r\n            this.props.setProps({\r\n                state: {\r\n                    readyState: WebSocket.OPEN,\r\n                    isTrusted: e.isTrusted,\r\n                    timeStamp: e.timeStamp,\r\n                    origin: e.origin,\r\n                    lastConnected: Number(new Date()),\r\n                },\r\n            });\r\n        };\r\n        this.client.onmessage = (e) => {\r\n            this.props.setProps({\r\n                state: {\r\n                    lastConnected: Number(new Date()),\r\n                },\r\n                message: {\r\n                    data: e.data,\r\n                    isTrusted: e.isTrusted,\r\n                    origin: e.origin,\r\n                    timeStamp: e.timeStamp,\r\n                },\r\n            });\r\n        };\r\n        this.client.onerror = (e) => {\r\n            console.log(`ON ERROR ${location.host}`);\r\n            this.props.setProps({error: JSON.stringify(e)});\r\n        };\r\n        this.client.onclose = (e) => {\r\n            console.log(`ON CLOSE ${location.host}`);\r\n            this.props.setProps({\r\n                error: JSON.stringify(e),\r\n                state: {\r\n                    readyState: WebSocket.CLOSED,\r\n                    isTrusted: e.isTrusted,\r\n                    timeStamp: e.timeStamp,\r\n                    code: e.code,\r\n                    reason: e.reason,\r\n                    wasClean: e.wasClean,\r\n                    lastConnected: Number(new Date()),\r\n                },\r\n            });\r\n            setTimeout(_init_client, 1000);\r\n        };\r\n    }\r\n\r\n    componentDidMount() {\r\n        console.log('Try to load web socket component');\r\n        this.props.setProps({\r\n            state: {\r\n                ...this.props.state,\r\n                lastConnected: 0,\r\n            },\r\n        });\r\n        this._init_client();\r\n    }\r\n\r\n    componentDidUpdate(prevProps) {\r\n        const {send} = this.props;\r\n        if (send && send !== prevProps.send) {\r\n            if (this.props.state.readyState === WebSocket.OPEN) {\r\n                this.client.send(send);\r\n            }\r\n            // TODO handle this\r\n        }\r\n    }\r\n\r\n    componentWillUnmount() {\r\n        this.client.onopen = null;\r\n        this.client.onclose = null;\r\n        this.client.onerror = null;\r\n        this.client.onmessage = null;\r\n        this.client.close();\r\n    }\r\n\r\n    render() {\r\n        return null;\r\n    }\r\n}\r\n\r\nDashWebsocketComponent.defaultProps = {\r\n    state: {readyState: WebSocket.CONNECTING},\r\n};\r\n\r\nDashWebsocketComponent.propTypes = {\r\n    /**\r\n     * This websocket state (in the readyState prop) and associated information.\r\n     */\r\n    state: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * When messages are received, this property is updated with the message content.\r\n     */\r\n    message: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * This property is set with the content of the onerror event.\r\n     */\r\n    error: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * When this property is set, a message is sent with its content.\r\n     */\r\n    send: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * The websocket endpoint (e.g. wss://echo.websocket.org).\r\n     */\r\n    url: PropTypes.string,\r\n\r\n    /**\r\n     * Supported websocket protocols (optional).\r\n     */\r\n    protocols: PropTypes.arrayOf(PropTypes.string),\r\n\r\n    /**\r\n     * The ID used to identify this component in Dash callbacks.\r\n     */\r\n    id: PropTypes.string,\r\n\r\n    /**\r\n     * Dash-assigned callback that should be called to report property changes\r\n     * to Dash, to make them available for callbacks.\r\n     */\r\n    setProps: PropTypes.func,\r\n};\r\n"
     ],
     "version": 3
 }
```

### Comparing `dash_websocket_component-0.0.3/dash_websocket_component/dash_websocket_component.min.js` & `dash_websocket_component-0.0.4/dash_websocket_component/dash_websocket_component.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -95,15 +95,15 @@
         var a = jsonpScriptSrc;
         jsonpScriptSrc = function(e) {
             var t, r = (t = s(), /\/_dash-component-suites\//.test(t.src)),
                 n = a(e);
             if (!r) return n;
             var o = n.split("/"),
                 i = o.slice(-1)[0].split(".");
-            return i.splice(1, 0, "v0_0_3m1710111623"), o.splice(-1, 1, i.join(".")), o.join("/")
+            return i.splice(1, 0, "v0_0_2m1714474540"), o.splice(-1, 1, i.join(".")), o.join("/")
         }
     }(() => {
         var e = {
             792: 0
         };
         o.f.j = (t, r) => {
             var n = o.o(e, t) ? e[t] : void 0;
```

### Comparing `dash_websocket_component-0.0.3/dash_websocket_component/dash_websocket_component.min.js.map` & `dash_websocket_component-0.0.4/dash_websocket_component/dash_websocket_component.min.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915966386554622%*

 * *Differences: {"'sourcesContent'": "{insert: [(12, 'var getCurrentScript = function() {\\n    var script = "*

 * *                     'document.currentScript;\\n    if (!script) {\\n        /* Shim for IE11 and '*

 * *                     'below */\\n        /* Do not take into account async scripts and inline '*

 * *                     'scripts */\\n\\n        var doc_scripts = '*

 * *                     "document.getElementsByTagName(\\'script\\');\\n        var scripts = "*

 * *                     '[];\\n\\n        for (var i = 0; i < doc […]*

```diff
@@ -171,14 +171,14 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + \"async-DashWebsocketComponent\" + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_3m1710111623\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_2m1714474540\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t792: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkdash_websocket_component\"] = self[\"webpackChunkdash_websocket_component\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "export const DashWebsocketComponent = React.lazy(() =>\r\n    import(\r\n        /* webpackChunkName: \"DashWebsocketComponent\" */ './fragments/DashWebsocketComponent.react'\r\n    )\r\n);\r\n",
         "import React from 'react';\r\nimport PropTypes from 'prop-types';\r\nimport {DashWebsocketComponent as RealComponent} from '../LazyLoader';\r\n\r\n/**\r\n * ExampleComponent is an example component.\r\n * It takes a property, `label`, and\r\n * displays it.\r\n * It renders an input with the property `value`\r\n * which is editable by the user.\r\n */\r\nconst DashWebsocketComponent = (props) => {\r\n    return (\r\n        <React.Suspense fallback={null}>\r\n            <RealComponent {...props} />\r\n        </React.Suspense>\r\n    );\r\n};\r\n\r\nDashWebsocketComponent.defaultProps = {};\r\n\r\nDashWebsocketComponent.propTypes = {\r\n    /**\r\n     * This websocket state (in the readyState prop) and associated information.\r\n     */\r\n    state: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * When messages are received, this property is updated with the message content.\r\n     */\r\n    message: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * This property is set with the content of the onerror event.\r\n     */\r\n    error: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * When this property is set, a message is sent with its content.\r\n     */\r\n    send: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\r\n\r\n    /**\r\n     * The websocket endpoint (e.g. wss://echo.websocket.org).\r\n     */\r\n    url: PropTypes.string,\r\n\r\n    /**\r\n     * Supported websocket protocols (optional).\r\n     */\r\n    protocols: PropTypes.arrayOf(PropTypes.string),\r\n\r\n    /**\r\n     * The ID used to identify this component in Dash callbacks.\r\n     */\r\n    id: PropTypes.string,\r\n\r\n    /**\r\n     * Dash-assigned callback that should be called to report property changes\r\n     * to Dash, to make them available for callbacks.\r\n     */\r\n    setProps: PropTypes.func,\r\n};\r\n\r\nexport default DashWebsocketComponent;\r\n\r\nexport const defaultProps = DashWebsocketComponent.defaultProps;\r\nexport const propTypes = DashWebsocketComponent.propTypes;\r\n"
     ],
     "version": 3
 }
```

### Comparing `dash_websocket_component-0.0.3/dash_websocket_component/metadata.json` & `dash_websocket_component-0.0.4/dash_websocket_component/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_websocket_component-0.0.3/dash_websocket_component/package-info.json` & `dash_websocket_component-0.0.4/dash_websocket_component/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9230769230769231%*

 * *Differences: {"'name'": "'dash_webocket_component'", "'version'": "'0.0.4'"}*

```diff
@@ -35,24 +35,24 @@
     "engines": {
         "node": ">=8.11.0",
         "npm": ">=6.1.0"
     },
     "homepage": "https://github.com/tkacikdominik/dash-websocket-component",
     "license": "MIT",
     "main": "build/index.js",
-    "name": "dash_websocket_component",
+    "name": "dash_webocket_component",
     "repository": {
         "type": "git",
         "url": "git://github.com/tkacikdominik/dash-websocket-component.git"
     },
     "scripts": {
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components dash_websocket_component -p package-info.json --r-prefix 'dwc' --jl-prefix 'dwc' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

### Comparing `dash_websocket_component-0.0.3/dash_websocket_component.egg-info/PKG-INFO` & `dash_websocket_component-0.0.4/dash_websocket_component.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: dash-websocket-component
-Version: 0.0.3
+Version: 0.0.4
 Summary: Project Description
+Home-page: UNKNOWN
 Author: Dominik Tkacik <tkacik38@gmail.com>
 License: MIT
+Platform: UNKNOWN
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dash WebSocket Component
 
 Dash WebSocket Component is a Dash component library.
@@ -102,7 +104,9 @@
         ```
         _Publishing your component to NPM will make the JavaScript bundles available on the unpkg CDN. By default, Dash serves the component library's CSS and JS locally, but if you choose to publish the package to NPM you can set `serve_locally` to `False` and you may see faster load times._
 
 5. Share your component with the community! https://community.plotly.com/c/dash
     1. Publish this repository to GitHub
     2. Tag your GitHub repository with the plotly-dash tag so that it appears here: https://github.com/topics/plotly-dash
     3. Create a post in the Dash community forum: https://community.plotly.com/c/dash
+
+
```

### Comparing `dash_websocket_component-0.0.3/dash_websocket_component.egg-info/SOURCES.txt` & `dash_websocket_component-0.0.4/dash_websocket_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_websocket_component-0.0.3/package.json` & `dash_websocket_component-0.0.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.0.4'"}*

```diff
@@ -50,9 +50,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_websocket_component -p package-info.json --r-prefix 'dwc' --jl-prefix 'dwc' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

### Comparing `dash_websocket_component-0.0.3/setup.py` & `dash_websocket_component-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `dash_websocket_component-0.0.3/tests/test_usage.py` & `dash_websocket_component-0.0.4/tests/test_usage.py`

 * *Files identical despite different names*

