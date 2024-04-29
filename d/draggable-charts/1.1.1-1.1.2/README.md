# Comparing `tmp/draggable-charts-1.1.1.tar.gz` & `tmp/draggable-charts-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draggable-charts-1.1.1.tar", last modified: Fri Apr 26 18:41:55 2024, max compression
+gzip compressed data, was "draggable-charts-1.1.2.tar", last modified: Mon Apr 29 22:15:36 2024, max compression
```

## Comparing `draggable-charts-1.1.1.tar` & `draggable-charts-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 18:41:55.243696 draggable-charts-1.1.1/
--rw-rw-rw-   0        0        0     1082 2024-04-05 22:58:34.000000 draggable-charts-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6106 2024-04-26 18:41:55.240703 draggable-charts-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5613 2024-04-24 01:12:42.000000 draggable-charts-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 18:41:55.028361 draggable-charts-1.1.1/draggable_charts/
--rw-rw-rw-   0        0        0       41 2024-04-26 18:40:29.000000 draggable-charts-1.1.1/draggable_charts/__init__.py
--rw-rw-rw-   0        0        0     2878 2024-04-26 18:05:48.000000 draggable-charts-1.1.1/draggable_charts/example.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:41:54.993439 draggable-charts-1.1.1/draggable_charts/frontend/
-drwxrwxrwx   0        0        0        0 2024-04-26 18:41:55.138261 draggable-charts-1.1.1/draggable_charts/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-04-26 18:39:58.000000 draggable-charts-1.1.1/draggable_charts/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.1.1/draggable_charts/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-04-26 18:39:58.000000 draggable-charts-1.1.1/draggable_charts/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-04-26 18:41:54.995434 draggable-charts-1.1.1/draggable_charts/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-04-26 18:41:55.166901 draggable-charts-1.1.1/draggable_charts/frontend/build/static/js/
--rw-rw-rw-   0        0        0   598781 2024-04-26 18:39:58.000000 draggable-charts-1.1.1/draggable_charts/frontend/build/static/js/main.ac399b09.js
--rw-rw-rw-   0        0        0     1831 2024-04-26 18:39:58.000000 draggable-charts-1.1.1/draggable_charts/frontend/build/static/js/main.ac399b09.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2560067 2024-04-26 18:39:58.000000 draggable-charts-1.1.1/draggable_charts/frontend/build/static/js/main.ac399b09.js.map
-drwxrwxrwx   0        0        0        0 2024-04-26 18:41:55.201806 draggable-charts-1.1.1/draggable_charts/utils/
--rw-rw-rw-   0        0        0      149 2024-04-25 23:36:44.000000 draggable-charts-1.1.1/draggable_charts/utils/__init__.py
--rw-rw-rw-   0        0        0     1797 2024-04-25 23:34:16.000000 draggable-charts-1.1.1/draggable_charts/utils/callback.py
--rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.1.1/draggable_charts/utils/component_func.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:41:55.232925 draggable-charts-1.1.1/draggable_charts/widgets/
--rw-rw-rw-   0        0        0      113 2024-04-23 23:20:49.000000 draggable-charts-1.1.1/draggable_charts/widgets/__init__.py
--rw-rw-rw-   0        0        0     4984 2024-04-26 17:59:06.000000 draggable-charts-1.1.1/draggable_charts/widgets/bezierchart.py
--rw-rw-rw-   0        0        0     4502 2024-04-26 00:23:06.000000 draggable-charts-1.1.1/draggable_charts/widgets/linechart.py
--rw-rw-rw-   0        0        0     2495 2024-04-26 00:23:32.000000 draggable-charts-1.1.1/draggable_charts/widgets/scatterchart.py
-drwxrwxrwx   0        0        0        0 2024-04-26 18:41:55.112525 draggable-charts-1.1.1/draggable_charts.egg-info/
--rw-rw-rw-   0        0        0     6106 2024-04-26 18:41:54.000000 draggable-charts-1.1.1/draggable_charts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      899 2024-04-26 18:41:54.000000 draggable-charts-1.1.1/draggable_charts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 18:41:54.000000 draggable-charts-1.1.1/draggable_charts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-26 18:41:54.000000 draggable-charts-1.1.1/draggable_charts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-26 18:41:54.000000 draggable-charts-1.1.1/draggable_charts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 18:41:55.244692 draggable-charts-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1115 2024-04-26 18:39:03.000000 draggable-charts-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.644344 draggable-charts-1.1.2/
+-rw-rw-rw-   0        0        0     1057 2024-04-29 05:02:10.000000 draggable-charts-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6106 2024-04-29 22:15:36.642326 draggable-charts-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5613 2024-04-24 01:12:42.000000 draggable-charts-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.560516 draggable-charts-1.1.2/draggable_charts/
+-rw-rw-rw-   0        0        0       41 2024-04-29 22:11:20.000000 draggable-charts-1.1.2/draggable_charts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.542557 draggable-charts-1.1.2/draggable_charts/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.589071 draggable-charts-1.1.2/draggable_charts/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-04-29 22:13:44.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2024-04-29 22:13:44.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.544553 draggable-charts-1.1.2/draggable_charts/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.602829 draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   605045 2024-04-29 22:13:44.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js
+-rw-rw-rw-   0        0        0     1831 2024-04-29 22:13:44.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2585172 2024-04-29 22:13:44.000000 draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js.map
+drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.619783 draggable-charts-1.1.2/draggable_charts/utils/
+-rw-rw-rw-   0        0        0      149 2024-04-25 23:36:44.000000 draggable-charts-1.1.2/draggable_charts/utils/__init__.py
+-rw-rw-rw-   0        0        0     1797 2024-04-25 23:34:16.000000 draggable-charts-1.1.2/draggable_charts/utils/callback.py
+-rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.1.2/draggable_charts/utils/component_func.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.637951 draggable-charts-1.1.2/draggable_charts/widgets/
+-rw-rw-rw-   0        0        0      163 2024-04-29 05:02:10.000000 draggable-charts-1.1.2/draggable_charts/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4984 2024-04-26 17:59:06.000000 draggable-charts-1.1.2/draggable_charts/widgets/bezierchart.py
+-rw-rw-rw-   0        0        0     6458 2024-04-29 15:36:39.000000 draggable-charts-1.1.2/draggable_charts/widgets/cubicbezierchart.py
+-rw-rw-rw-   0        0        0     4502 2024-04-26 00:23:06.000000 draggable-charts-1.1.2/draggable_charts/widgets/linechart.py
+-rw-rw-rw-   0        0        0     2495 2024-04-26 00:23:32.000000 draggable-charts-1.1.2/draggable_charts/widgets/scatterchart.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:15:36.578873 draggable-charts-1.1.2/draggable_charts.egg-info/
+-rw-rw-rw-   0        0        0     6106 2024-04-29 22:15:36.000000 draggable-charts-1.1.2/draggable_charts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      916 2024-04-29 22:15:36.000000 draggable-charts-1.1.2/draggable_charts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 22:15:36.000000 draggable-charts-1.1.2/draggable_charts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-29 22:15:36.000000 draggable-charts-1.1.2/draggable_charts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-29 22:15:36.000000 draggable-charts-1.1.2/draggable_charts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 22:15:36.645272 draggable-charts-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1115 2024-04-29 22:15:28.000000 draggable-charts-1.1.2/setup.py
```

### Comparing `draggable-charts-1.1.1/LICENSE` & `draggable-charts-1.1.2/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018-2021 Streamlit Inc.
+Copyright (c)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `draggable-charts-1.1.1/PKG-INFO` & `draggable-charts-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `draggable-charts-1.1.1/README.md` & `draggable-charts-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.1/draggable_charts/frontend/build/bootstrap.min.css` & `draggable-charts-1.1.2/draggable_charts/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.1/draggable_charts/frontend/build/static/js/main.ac399b09.js` & `draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.ac399b09.js.LICENSE.txt */
+/*! For license information please see main.96151505.js.LICENSE.txt */
 (() => {
     var e = {
             895: (t, e, n) => {
                 var i;
                 ! function(r, s, o, a) {
                     "use strict";
                     var l, c = ["", "webkit", "Moz", "MS", "ms", "o"],
@@ -131,21 +131,21 @@
                             if ((i = (n = c[s]) ? n + r : e) in t) return i;
                             s++
                         }
                         return a
                     }
                     var F = 1;
 
-                    function L(t) {
+                    function z(t) {
                         var e = t.ownerDocument || t;
                         return e.defaultView || e.parentWindow || r
                     }
-                    var z = "ontouchstart" in r,
+                    var L = "ontouchstart" in r,
                         N = P(r, "PointerEvent") !== a,
-                        B = z && /mobile|tablet|ip(ad|hone|od)|android/i.test(navigator.userAgent),
+                        B = L && /mobile|tablet|ip(ad|hone|od)|android/i.test(navigator.userAgent),
                         R = "touch",
                         U = "mouse",
                         V = 25,
                         j = 1,
                         W = 4,
                         H = 8,
                         Y = 1,
@@ -269,18 +269,18 @@
                         var i = e[n[0]] - t[n[0]],
                             r = e[n[1]] - t[n[1]];
                         return 180 * Math.atan2(r, i) / Math.PI
                     }
                     et.prototype = {
                         handler: function() {},
                         init: function() {
-                            this.evEl && k(this.element, this.evEl, this.domHandler), this.evTarget && k(this.target, this.evTarget, this.domHandler), this.evWin && k(L(this.element), this.evWin, this.domHandler)
+                            this.evEl && k(this.element, this.evEl, this.domHandler), this.evTarget && k(this.target, this.evTarget, this.domHandler), this.evWin && k(z(this.element), this.evWin, this.domHandler)
                         },
                         destroy: function() {
-                            this.evEl && M(this.element, this.evEl, this.domHandler), this.evTarget && M(this.target, this.evTarget, this.domHandler), this.evWin && M(L(this.element), this.evWin, this.domHandler)
+                            this.evEl && M(this.element, this.evEl, this.domHandler), this.evTarget && M(this.target, this.evTarget, this.domHandler), this.evWin && M(z(this.element), this.evWin, this.domHandler)
                         }
                     };
                     var ct = {
                             mousedown: j,
                             mousemove: 2,
                             mouseup: W
                         },
@@ -457,16 +457,16 @@
                         }
                     });
                     var Ot = P(u.style, "touchAction"),
                         Ct = Ot !== a,
                         At = "compute",
                         Pt = "auto",
                         Ft = "manipulation",
-                        Lt = "none",
-                        zt = "pan-x",
+                        zt = "none",
+                        Lt = "pan-x",
                         Nt = "pan-y",
                         Bt = function() {
                             if (!Ct) return !1;
                             var t = {},
                                 e = r.CSS && r.CSS.supports;
                             return ["auto", "manipulation", "pan-y", "pan-x", "pan-x pan-y", "none"].forEach((function(n) {
                                 t[n] = !e || r.CSS.supports("touch-action", n)
@@ -485,32 +485,32 @@
                         },
                         compute: function() {
                             var t = [];
                             return y(this.manager.recognizers, (function(e) {
                                     S(e.options.enable, [e]) && (t = t.concat(e.getTouchAction()))
                                 })),
                                 function(t) {
-                                    if (E(t, Lt)) return Lt;
-                                    var e = E(t, zt),
+                                    if (E(t, zt)) return zt;
+                                    var e = E(t, Lt),
                                         n = E(t, Nt);
-                                    if (e && n) return Lt;
-                                    if (e || n) return e ? zt : Nt;
+                                    if (e && n) return zt;
+                                    if (e || n) return e ? Lt : Nt;
                                     if (E(t, Ft)) return Ft;
                                     return Pt
                                 }(t.join(" "))
                         },
                         preventDefaults: function(t) {
                             var e = t.srcEvent,
                                 n = t.offsetDirection;
                             if (this.manager.session.prevented) e.preventDefault();
                             else {
                                 var i = this.actions,
-                                    r = E(i, Lt) && !Bt[Lt],
+                                    r = E(i, zt) && !Bt[zt],
                                     s = E(i, Nt) && !Bt[Nt],
-                                    o = E(i, zt) && !Bt[zt];
+                                    o = E(i, Lt) && !Bt[Lt];
                                 if (r) {
                                     var a = 1 === t.pointers.length,
                                         l = t.distance < 2,
                                         c = t.deltaTime < 250;
                                     if (a && l && c) return
                                 }
                                 if (!o || !s) return r || s && n & Q || o && n & G ? this.preventSrc(e) : void 0
@@ -650,15 +650,15 @@
                             threshold: 10,
                             pointers: 1,
                             direction: Z
                         },
                         getTouchAction: function() {
                             var t = this.options.direction,
                                 e = [];
-                            return t & Q && e.push(Nt), t & G && e.push(zt), e
+                            return t & Q && e.push(Nt), t & G && e.push(Lt), e
                         },
                         directionTest: function(t) {
                             var e = this.options,
                                 n = !0,
                                 i = t.distance,
                                 r = t.direction,
                                 s = t.deltaX,
@@ -676,15 +676,15 @@
                     }), _(qt, $t, {
                         defaults: {
                             event: "pinch",
                             threshold: 0,
                             pointers: 2
                         },
                         getTouchAction: function() {
-                            return [Lt]
+                            return [zt]
                         },
                         attrTest: function(t) {
                             return this._super.attrTest.call(this, t) && (Math.abs(t.scale - 1) > this.options.threshold || 2 & this.state)
                         },
                         emit: function(t) {
                             if (1 !== t.scale) {
                                 var e = t.scale < 1 ? "in" : "out";
@@ -723,15 +723,15 @@
                     }), _(Qt, $t, {
                         defaults: {
                             event: "rotate",
                             threshold: 0,
                             pointers: 2
                         },
                         getTouchAction: function() {
-                            return [Lt]
+                            return [zt]
                         },
                         attrTest: function(t) {
                             return this._super.attrTest.call(this, t) && (Math.abs(t.rotation) > this.options.threshold || 2 & this.state)
                         }
                     }), _(Gt, $t, {
                         defaults: {
                             event: "swipe",
@@ -831,15 +831,15 @@
                             userDrag: "none",
                             tapHighlightColor: "rgba(0,0,0,0)"
                         }
                     };
 
                     function te(t, e) {
                         var n;
-                        this.options = l({}, Jt.defaults, e || {}), this.options.inputTarget = this.options.inputTarget || t, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = t, this.input = new((n = this).options.inputClass || (N ? yt : B ? St : z ? Mt : dt))(n, nt), this.touchAction = new Rt(this, this.options.touchAction), ee(this, !0), y(this.options.recognizers, (function(t) {
+                        this.options = l({}, Jt.defaults, e || {}), this.options.inputTarget = this.options.inputTarget || t, this.handlers = {}, this.session = {}, this.recognizers = [], this.oldCssProps = {}, this.element = t, this.input = new((n = this).options.inputClass || (N ? yt : B ? St : L ? Mt : dt))(n, nt), this.touchAction = new Rt(this, this.options.touchAction), ee(this, !0), y(this.options.recognizers, (function(t) {
                             var e = this.add(new t[0](t[1]));
                             t[2] && e.recognizeWith(t[2]), t[3] && e.requireFailure(t[3])
                         }), this)
                     }
 
                     function ee(t, e) {
                         var n, i = t.element;
@@ -1196,25 +1196,25 @@
                     }
                 }
 
                 function F(t, e) {
                     return t(e)
                 }
 
-                function L(t, e, n, i, r) {
+                function z(t, e, n, i, r) {
                     return t(e, n, i, r)
                 }
 
-                function z() {}
+                function L() {}
                 var N = F,
                     B = !1,
                     R = !1;
 
                 function U() {
-                    null === D && null === O || (z(), P())
+                    null === D && null === O || (L(), P())
                 }
 
                 function V(t, e, n) {
                     if (R) return t(e, n);
                     R = !0;
                     try {
                         return N(t, e, n)
@@ -1560,32 +1560,32 @@
                 }
 
                 function Pt(t) {
                     var e = t.textContent;
                     e === t._wrapperState.initialValue && "" !== e && null !== e && (t.value = e)
                 }
                 var Ft = "http://www.w3.org/1999/xhtml",
-                    Lt = "http://www.w3.org/2000/svg";
+                    zt = "http://www.w3.org/2000/svg";
 
-                function zt(t) {
+                function Lt(t) {
                     switch (t) {
                         case "svg":
                             return "http://www.w3.org/2000/svg";
                         case "math":
                             return "http://www.w3.org/1998/Math/MathML";
                         default:
                             return "http://www.w3.org/1999/xhtml"
                     }
                 }
 
                 function Nt(t, e) {
-                    return null == t || "http://www.w3.org/1999/xhtml" === t ? zt(e) : "http://www.w3.org/2000/svg" === t && "foreignObject" === e ? "http://www.w3.org/1999/xhtml" : t
+                    return null == t || "http://www.w3.org/1999/xhtml" === t ? Lt(e) : "http://www.w3.org/2000/svg" === t && "foreignObject" === e ? "http://www.w3.org/1999/xhtml" : t
                 }
                 var Bt, Rt, Ut = (Rt = function(t, e) {
-                    if (t.namespaceURI !== Lt || "innerHTML" in t) t.innerHTML = e;
+                    if (t.namespaceURI !== zt || "innerHTML" in t) t.innerHTML = e;
                     else {
                         for ((Bt = Bt || document.createElement("div")).innerHTML = "<svg>" + e.valueOf().toString() + "</svg>", e = Bt.firstChild; t.firstChild;) t.removeChild(t.firstChild);
                         for (; e.firstChild;) t.appendChild(e.firstChild)
                     }
                 }, "undefined" !== typeof MSApp && MSApp.execUnsafeLocalFunction ? function(t, e, n, i) {
                     MSApp.execUnsafeLocalFunction((function() {
                         return Rt(t, e)
@@ -1920,43 +1920,43 @@
                     return !0
                 }
 
                 function Fe(t, e, n) {
                     Pe(t) && n.delete(e)
                 }
 
-                function Le() {
+                function ze() {
                     for (ve = !1; 0 < xe.length;) {
                         var t = xe[0];
                         if (null !== t.blockedOn) {
                             null !== (t = Fn(t.blockedOn)) && me(t);
                             break
                         }
                         var e = Je(t.topLevelType, t.eventSystemFlags, t.container, t.nativeEvent);
                         null !== e ? t.blockedOn = e : xe.shift()
                     }
                     null !== _e && Pe(_e) && (_e = null), null !== we && Pe(we) && (we = null), null !== Se && Pe(Se) && (Se = null), Te.forEach(Fe), ke.forEach(Fe)
                 }
 
-                function ze(t, e) {
-                    t.blockedOn === e && (t.blockedOn = null, ve || (ve = !0, s.unstable_scheduleCallback(s.unstable_NormalPriority, Le)))
+                function Le(t, e) {
+                    t.blockedOn === e && (t.blockedOn = null, ve || (ve = !0, s.unstable_scheduleCallback(s.unstable_NormalPriority, ze)))
                 }
 
                 function Ne(t) {
                     function e(e) {
-                        return ze(e, t)
+                        return Le(e, t)
                     }
                     if (0 < xe.length) {
-                        ze(xe[0], t);
+                        Le(xe[0], t);
                         for (var n = 1; n < xe.length; n++) {
                             var i = xe[n];
                             i.blockedOn === t && (i.blockedOn = null)
                         }
                     }
-                    for (null !== _e && ze(_e, t), null !== we && ze(we, t), null !== Se && ze(Se, t), Te.forEach(e), ke.forEach(e), n = 0; n < Me.length; n++)(i = Me[n]).blockedOn === t && (i.blockedOn = null);
+                    for (null !== _e && Le(_e, t), null !== we && Le(we, t), null !== Se && Le(Se, t), Te.forEach(e), ke.forEach(e), n = 0; n < Me.length; n++)(i = Me[n]).blockedOn === t && (i.blockedOn = null);
                     for (; 0 < Me.length && null === (n = Me[0]).blockedOn;) Ae(n), null === n.blockedOn && Me.shift()
                 }
                 var Be = {},
                     Re = new Map,
                     Ue = new Map,
                     Ve = ["abort", "abort", Xt, "animationEnd", qt, "animationIteration", Kt, "animationStart", "canplay", "canPlay", "canplaythrough", "canPlayThrough", "durationchange", "durationChange", "emptied", "emptied", "encrypted", "encrypted", "ended", "ended", "error", "error", "gotpointercapture", "gotPointerCapture", "load", "load", "loadeddata", "loadedData", "loadedmetadata", "loadedMetadata", "loadstart", "loadStart", "lostpointercapture", "lostPointerCapture", "playing", "playing", "progress", "progress", "seeking", "seeking", "stalled", "stalled", "suspend", "suspend", "timeupdate", "timeUpdate", Qt, "transitionEnd", "waiting", "waiting"];
 
@@ -1997,20 +1997,20 @@
                         default:
                             i = Ze.bind(null, e, 1, t)
                     }
                     n ? t.addEventListener(e, i, !0) : t.addEventListener(e, i, !1)
                 }
 
                 function Qe(t, e, n, i) {
-                    B || z();
+                    B || L();
                     var r = Ze,
                         s = B;
                     B = !0;
                     try {
-                        L(r, t, e, n, i)
+                        z(r, t, e, n, i)
                     } finally {
                         (B = s) || U()
                     }
                 }
 
                 function Ge(t, e, n, i) {
                     $e(Ye, Ze.bind(null, t, e, n, i))
@@ -2319,20 +2319,20 @@
                     return null
                 }
 
                 function Fn(t) {
                     return !(t = t[On] || t[An]) || 5 !== t.tag && 6 !== t.tag && 13 !== t.tag && 3 !== t.tag ? null : t
                 }
 
-                function Ln(t) {
+                function zn(t) {
                     if (5 === t.tag || 6 === t.tag) return t.stateNode;
                     throw Error(o(33))
                 }
 
-                function zn(t) {
+                function Ln(t) {
                     return t[Cn] || null
                 }
 
                 function Nn(t) {
                     do {
                         t = t.return
                     } while (t && 5 !== t.tag);
@@ -2630,15 +2630,15 @@
                     vi = null;
 
                 function xi(t) {
                     le(t)
                 }
 
                 function _i(t) {
-                    if (_t(Ln(t))) return t
+                    if (_t(zn(t))) return t
                 }
 
                 function wi(t, e) {
                     if ("change" === t) return e
                 }
                 var Si = !1;
 
@@ -2675,15 +2675,15 @@
                     if ("input" === t || "change" === t) return _i(e)
                 }
                 I && (Si = ue("input") && (!document.documentMode || 9 < document.documentMode));
                 var Oi = {
                         eventTypes: mi,
                         _isInputEventSupported: Si,
                         extractEvents: function(t, e, n, i) {
-                            var r = e ? Ln(e) : window,
+                            var r = e ? zn(e) : window,
                                 s = r.nodeName && r.nodeName.toLowerCase();
                             if ("select" === s || "input" === s && "file" === r.type) var o = wi;
                             else if (gi(r))
                                 if (Si) o = Di;
                                 else {
                                     o = Ii;
                                     var a = Mi
@@ -2708,16 +2708,16 @@
                     var e = this.nativeEvent;
                     return e.getModifierState ? e.getModifierState(t) : !!(t = Ai[t]) && !!e[t]
                 }
 
                 function Fi() {
                     return Pi
                 }
-                var Li = 0,
-                    zi = 0,
+                var zi = 0,
+                    Li = 0,
                     Ni = !1,
                     Bi = !1,
                     Ri = Ci.extend({
                         screenX: null,
                         screenY: null,
                         clientX: null,
                         clientY: null,
@@ -2731,21 +2731,21 @@
                         button: null,
                         buttons: null,
                         relatedTarget: function(t) {
                             return t.relatedTarget || (t.fromElement === t.srcElement ? t.toElement : t.fromElement)
                         },
                         movementX: function(t) {
                             if ("movementX" in t) return t.movementX;
-                            var e = Li;
-                            return Li = t.screenX, Ni ? "mousemove" === t.type ? t.screenX - e : 0 : (Ni = !0, 0)
+                            var e = zi;
+                            return zi = t.screenX, Ni ? "mousemove" === t.type ? t.screenX - e : 0 : (Ni = !0, 0)
                         },
                         movementY: function(t) {
                             if ("movementY" in t) return t.movementY;
-                            var e = zi;
-                            return zi = t.screenY, Bi ? "mousemove" === t.type ? t.screenY - e : 0 : (Bi = !0, 0)
+                            var e = Li;
+                            return Li = t.screenY, Bi ? "mousemove" === t.type ? t.screenY - e : 0 : (Bi = !0, 0)
                         }
                     }),
                     Ui = Ri.extend({
                         pointerId: null,
                         width: null,
                         height: null,
                         pressure: null,
@@ -2783,15 +2783,15 @@
                             (s = i.window === i ? i : (s = i.ownerDocument) ? s.defaultView || s.parentWindow : window, o) ? (o = e, null !== (e = (e = n.relatedTarget || n.toElement) ? Pn(e) : null) && (e !== te(e) || 5 !== e.tag && 6 !== e.tag) && (e = null)) : o = null;
                             if (o === e) return null;
                             if ("mouseout" === t || "mouseover" === t) var a = Ri,
                                 l = Vi.mouseLeave,
                                 c = Vi.mouseEnter,
                                 u = "mouse";
                             else "pointerout" !== t && "pointerover" !== t || (a = Ui, l = Vi.pointerLeave, c = Vi.pointerEnter, u = "pointer");
-                            if (t = null == o ? s : Ln(o), s = null == e ? s : Ln(e), (l = a.getPooled(l, o, n, i)).type = u + "leave", l.target = t, l.relatedTarget = s, (n = a.getPooled(c, e, n, i)).type = u + "enter", n.target = s, n.relatedTarget = t, u = e, (i = o) && u) t: {
+                            if (t = null == o ? s : zn(o), s = null == e ? s : zn(e), (l = a.getPooled(l, o, n, i)).type = u + "leave", l.target = t, l.relatedTarget = s, (n = a.getPooled(c, e, n, i)).type = u + "enter", n.target = s, n.relatedTarget = t, u = e, (i = o) && u) t: {
                                 for (c = u, o = 0, t = a = i; t; t = Nn(t)) o++;
                                 for (t = 0, e = c; e; e = Nn(e)) t++;
                                 for (; 0 < o - t;) a = Nn(a),
                                 o--;
                                 for (; 0 < t - o;) c = Nn(c),
                                 t--;
                                 for (; o--;) {
@@ -2862,15 +2862,15 @@
                                             r = !1;
                                             break t
                                         } r = !0
                                 }
                                 s = !r
                             }
                             if (s) return null;
-                            switch (r = e ? Ln(e) : window, t) {
+                            switch (r = e ? zn(e) : window, t) {
                                 case "focus":
                                     (gi(r) || "true" === r.contentEditable) && (qi = r, Ki = e, Qi = null);
                                     break;
                                 case "blur":
                                     Qi = Ki = qi = null;
                                     break;
                                 case "mousedown":
@@ -3089,15 +3089,15 @@
                                 default:
                                     t = Qn
                             }
                             return Wn(e = t.getPooled(r, e, n, i)), e
                         }
                     };
                 if (b) throw Error(o(101));
-                b = Array.prototype.slice.call("ResponderEventPlugin SimpleEventPlugin EnterLeaveEventPlugin ChangeEventPlugin SelectEventPlugin BeforeInputEventPlugin".split(" ")), x(), p = zn, g = Fn, m = Ln, M({
+                b = Array.prototype.slice.call("ResponderEventPlugin SimpleEventPlugin EnterLeaveEventPlugin ChangeEventPlugin SelectEventPlugin BeforeInputEventPlugin".split(" ")), x(), p = Ln, g = Fn, m = zn, M({
                     SimpleEventPlugin: hr,
                     EnterLeaveEventPlugin: ji,
                     ChangeEventPlugin: Oi,
                     SelectEventPlugin: Ji,
                     BeforeInputEventPlugin: fi
                 });
                 var dr = [],
@@ -3163,16 +3163,16 @@
                     Er = s.unstable_scheduleCallback,
                     Dr = s.unstable_cancelCallback,
                     Or = s.unstable_requestPaint,
                     Cr = s.unstable_now,
                     Ar = s.unstable_getCurrentPriorityLevel,
                     Pr = s.unstable_ImmediatePriority,
                     Fr = s.unstable_UserBlockingPriority,
-                    Lr = s.unstable_NormalPriority,
-                    zr = s.unstable_LowPriority,
+                    zr = s.unstable_NormalPriority,
+                    Lr = s.unstable_LowPriority,
                     Nr = s.unstable_IdlePriority,
                     Br = {},
                     Rr = s.unstable_shouldYield,
                     Ur = void 0 !== Or ? Or : function() {},
                     Vr = null,
                     jr = null,
                     Wr = !1,
@@ -3183,17 +3183,17 @@
 
                 function $r() {
                     switch (Ar()) {
                         case Pr:
                             return 99;
                         case Fr:
                             return 98;
-                        case Lr:
-                            return 97;
                         case zr:
+                            return 97;
+                        case Lr:
                             return 96;
                         case Nr:
                             return 95;
                         default:
                             throw Error(o(332))
                     }
                 }
@@ -3201,17 +3201,17 @@
                 function Xr(t) {
                     switch (t) {
                         case 99:
                             return Pr;
                         case 98:
                             return Fr;
                         case 97:
-                            return Lr;
-                        case 96:
                             return zr;
+                        case 96:
+                            return Lr;
                         case 95:
                             return Nr;
                         default:
                             throw Error(o(332))
                     }
                 }
 
@@ -3291,15 +3291,15 @@
                             n.childExpirationTime = e
                         }
                         t = t.return
                     }
                 }
 
                 function ls(t, e) {
-                    ns = t, rs = is = null, null !== (t = t.dependencies) && null !== t.firstContext && (t.expirationTime >= e && (zo = !0), t.firstContext = null)
+                    ns = t, rs = is = null, null !== (t = t.dependencies) && null !== t.firstContext && (t.expirationTime >= e && (Lo = !0), t.firstContext = null)
                 }
 
                 function cs(t, e) {
                     if (rs !== t && !1 !== e && 0 !== e)
                         if ("number" === typeof e && 1073741823 !== e || (rs = t, e = 1073741823), e = {
                                 context: t,
                                 observedBits: e,
@@ -3715,42 +3715,42 @@
                     As = {},
                     Ps = {
                         current: As
                     },
                     Fs = {
                         current: As
                     },
-                    Ls = {
+                    zs = {
                         current: As
                     };
 
-                function zs(t) {
+                function Ls(t) {
                     if (t === As) throw Error(o(174));
                     return t
                 }
 
                 function Ns(t, e) {
-                    switch (gr(Ls, e), gr(Fs, t), gr(Ps, As), t = e.nodeType) {
+                    switch (gr(zs, e), gr(Fs, t), gr(Ps, As), t = e.nodeType) {
                         case 9:
                         case 11:
                             e = (e = e.documentElement) ? e.namespaceURI : Nt(null, "");
                             break;
                         default:
                             e = Nt(e = (t = 8 === t ? e.parentNode : e).namespaceURI || null, t = t.tagName)
                     }
                     pr(Ps), gr(Ps, e)
                 }
 
                 function Bs() {
-                    pr(Ps), pr(Fs), pr(Ls)
+                    pr(Ps), pr(Fs), pr(zs)
                 }
 
                 function Rs(t) {
-                    zs(Ls.current);
-                    var e = zs(Ps.current),
+                    Ls(zs.current);
+                    var e = Ls(Ps.current),
                         n = Nt(e, t.type);
                     e !== n && (gr(Fs, t), gr(Ps, n))
                 }
 
                 function Us(t) {
                     Fs.current === t && (pr(Ps), pr(Fs))
                 }
@@ -3888,15 +3888,15 @@
                                 action: c.action,
                                 eagerReducer: c.eagerReducer,
                                 eagerState: c.eagerState,
                                 next: null
                             }), wl(u, c.suspenseConfig), i = c.eagerReducer === t ? c.eagerState : t(i, c.action);
                             c = c.next
                         } while (null !== c && c !== r);
-                        null === l ? s = i : l.next = a, Wi(i, e.memoizedState) || (zo = !0), e.memoizedState = i, e.baseState = s, e.baseQueue = l, n.lastRenderedState = i
+                        null === l ? s = i : l.next = a, Wi(i, e.memoizedState) || (Lo = !0), e.memoizedState = i, e.baseState = s, e.baseQueue = l, n.lastRenderedState = i
                     }
                     return [e.memoizedState, n.dispatch]
                 }
 
                 function ro(t) {
                     var e = eo(),
                         n = e.queue;
@@ -3907,15 +3907,15 @@
                         s = e.memoizedState;
                     if (null !== r) {
                         n.pending = null;
                         var a = r = r.next;
                         do {
                             s = t(s, a.action), a = a.next
                         } while (a !== r);
-                        Wi(s, e.memoizedState) || (zo = !0), e.memoizedState = s, null === e.baseQueue && (e.baseState = s), n.lastRenderedState = s
+                        Wi(s, e.memoizedState) || (Lo = !0), e.memoizedState = s, null === e.baseQueue && (e.baseState = s), n.lastRenderedState = s
                     }
                     return [s, i]
                 }
 
                 function so(t) {
                     var e = to();
                     return "function" === typeof t && (t = t()), e.memoizedState = e.baseState = t, t = (t = e.queue = {
@@ -4244,47 +4244,47 @@
                     } else Io = Mo ? In(t.stateNode.nextSibling) : null;
                     return !0
                 }
 
                 function Fo() {
                     Io = Mo = null, Eo = !1
                 }
-                var Lo = Q.ReactCurrentOwner,
-                    zo = !1;
+                var zo = Q.ReactCurrentOwner,
+                    Lo = !1;
 
                 function No(t, e, n, i) {
                     e.child = null === t ? Cs(e, null, n, i) : Os(e, t.child, n, i)
                 }
 
                 function Bo(t, e, n, i, r) {
                     n = n.render;
                     var s = e.ref;
-                    return ls(e, r), i = Js(t, e, n, i, s, r), null === t || zo ? (e.effectTag |= 1, No(t, e, i, r), e.child) : (e.updateQueue = t.updateQueue, e.effectTag &= -517, t.expirationTime <= r && (t.expirationTime = 0), ea(t, e, r))
+                    return ls(e, r), i = Js(t, e, n, i, s, r), null === t || Lo ? (e.effectTag |= 1, No(t, e, i, r), e.child) : (e.updateQueue = t.updateQueue, e.effectTag &= -517, t.expirationTime <= r && (t.expirationTime = 0), ea(t, e, r))
                 }
 
                 function Ro(t, e, n, i, r, s) {
                     if (null === t) {
                         var o = n.type;
                         return "function" !== typeof o || jl(o) || void 0 !== o.defaultProps || null !== n.compare || void 0 !== n.defaultProps ? ((t = Hl(n.type, null, i, null, e.mode, s)).ref = e.ref, t.return = e, e.child = t) : (e.tag = 15, e.type = o, Uo(t, e, o, i, r, s))
                     }
                     return o = t.child, r < s && (r = o.memoizedProps, (n = null !== (n = n.compare) ? n : Yi)(r, i) && t.ref === e.ref) ? ea(t, e, s) : (e.effectTag |= 1, (t = Wl(o, i)).ref = e.ref, t.return = e, e.child = t)
                 }
 
                 function Uo(t, e, n, i, r, s) {
-                    return null !== t && Yi(t.memoizedProps, i) && t.ref === e.ref && (zo = !1, r < s) ? (e.expirationTime = t.expirationTime, ea(t, e, s)) : jo(t, e, n, i, s)
+                    return null !== t && Yi(t.memoizedProps, i) && t.ref === e.ref && (Lo = !1, r < s) ? (e.expirationTime = t.expirationTime, ea(t, e, s)) : jo(t, e, n, i, s)
                 }
 
                 function Vo(t, e) {
                     var n = e.ref;
                     (null === t && null !== n || null !== t && t.ref !== n) && (e.effectTag |= 128)
                 }
 
                 function jo(t, e, n, i, r) {
                     var s = _r(n) ? vr : yr.current;
-                    return s = xr(e, s), ls(e, r), n = Js(t, e, n, i, s, r), null === t || zo ? (e.effectTag |= 1, No(t, e, n, r), e.child) : (e.updateQueue = t.updateQueue, e.effectTag &= -517, t.expirationTime <= r && (t.expirationTime = 0), ea(t, e, r))
+                    return s = xr(e, s), ls(e, r), n = Js(t, e, n, i, s, r), null === t || Lo ? (e.effectTag |= 1, No(t, e, n, r), e.child) : (e.updateQueue = t.updateQueue, e.effectTag &= -517, t.expirationTime <= r && (t.expirationTime = 0), ea(t, e, r))
                 }
 
                 function Wo(t, e, n, i, r) {
                     if (_r(n)) {
                         var s = !0;
                         kr(e)
                     } else s = !1;
@@ -4305,15 +4305,15 @@
                     return Ho(t, e, n, i, s, r)
                 }
 
                 function Ho(t, e, n, i, r, s) {
                     Vo(t, e);
                     var o = 0 !== (64 & e.effectTag);
                     if (!i && !o) return r && Mr(e, n, !1), ea(t, e, s);
-                    i = e.stateNode, Lo.current = e;
+                    i = e.stateNode, zo.current = e;
                     var a = o && "function" !== typeof n.getDerivedStateFromError ? null : i.render();
                     return e.effectTag |= 1, null !== t && o ? (e.child = Os(e, t.child, null, s), e.child = Os(e, null, a, s)) : No(t, e, a, s), e.memoizedState = i.state, r && Mr(e, n, !0), e.child
                 }
 
                 function Yo(t) {
                     var e = t.stateNode;
                     e.pendingContext ? Sr(0, e.pendingContext, e.pendingContext !== e.context) : e.context && Sr(0, e.context, !1), Ns(t, e.containerInfo)
@@ -4461,23 +4461,23 @@
                             return null;
                         case 1:
                         case 17:
                             return _r(e.type) && wr(), null;
                         case 3:
                             return Bs(), pr(br), pr(yr), (n = e.stateNode).pendingContext && (n.context = n.pendingContext, n.pendingContext = null), null !== t && null !== t.child || !Po(e) || (e.effectTag |= 4), Xo(e), null;
                         case 5:
-                            Us(e), n = zs(Ls.current);
+                            Us(e), n = Ls(zs.current);
                             var s = e.type;
                             if (null !== t && null != e.stateNode) qo(t, e, s, i, n), t.ref !== e.ref && (e.effectTag |= 128);
                             else {
                                 if (!i) {
                                     if (null === e.stateNode) throw Error(o(166));
                                     return null
                                 }
-                                if (t = zs(Ps.current), Po(e)) {
+                                if (t = Ls(Ps.current), Po(e)) {
                                     i = e.stateNode, s = e.type;
                                     var a = e.memoizedProps;
                                     switch (i[On] = e, i[Cn] = a, s) {
                                         case "iframe":
                                         case "object":
                                         case "embed":
                                             qe("load", i);
@@ -4526,15 +4526,15 @@
                                         case "option":
                                             break;
                                         default:
                                             "function" === typeof a.onClick && (i.onclick = un)
                                     }
                                     n = t, e.updateQueue = n, null !== n && (e.effectTag |= 4)
                                 } else {
-                                    switch (l = 9 === n.nodeType ? n : n.ownerDocument, t === ln && (t = zt(s)), t === ln ? "script" === s ? ((t = l.createElement("div")).innerHTML = "<script><\/script>", t = t.removeChild(t.firstChild)) : "string" === typeof i.is ? t = l.createElement(s, {
+                                    switch (l = 9 === n.nodeType ? n : n.ownerDocument, t === ln && (t = Lt(s)), t === ln ? "script" === s ? ((t = l.createElement("div")).innerHTML = "<script><\/script>", t = t.removeChild(t.firstChild)) : "string" === typeof i.is ? t = l.createElement(s, {
                                             is: i.is
                                         }) : (t = l.createElement(s), "select" === s && (l = t, i.multiple ? l.multiple = !0 : i.size && (l.size = i.size))) : t = l.createElementNS(t, s), t[On] = e, t[Cn] = i, $o(t, e, !1, !1), e.stateNode = t, l = an(s, i), s) {
                                         case "iframe":
                                         case "object":
                                         case "embed":
                                             qe("load", t), c = i;
                                             break;
@@ -4603,19 +4603,19 @@
                                 null !== e.ref && (e.effectTag |= 128)
                             }
                             return null;
                         case 6:
                             if (t && null != e.stateNode) Ko(t, e, t.memoizedProps, i);
                             else {
                                 if ("string" !== typeof i && null === e.stateNode) throw Error(o(166));
-                                n = zs(Ls.current), zs(Ps.current), Po(e) ? (n = e.stateNode, i = e.memoizedProps, n[On] = e, n.nodeValue !== i && (e.effectTag |= 4)) : ((n = (9 === n.nodeType ? n : n.ownerDocument).createTextNode(i))[On] = e, e.stateNode = n)
+                                n = Ls(zs.current), Ls(Ps.current), Po(e) ? (n = e.stateNode, i = e.memoizedProps, n[On] = e, n.nodeValue !== i && (e.effectTag |= 4)) : ((n = (9 === n.nodeType ? n : n.ownerDocument).createTextNode(i))[On] = e, e.stateNode = n)
                             }
                             return null;
                         case 13:
-                            return pr(Vs), i = e.memoizedState, 0 !== (64 & e.effectTag) ? (e.expirationTime = n, e) : (n = null !== i, i = !1, null === t ? void 0 !== e.memoizedProps.fallback && Po(e) : (i = null !== (s = t.memoizedState), n || null === s || null !== (s = t.child.sibling) && (null !== (a = e.firstEffect) ? (e.firstEffect = s, s.nextEffect = a) : (e.firstEffect = e.lastEffect = s, s.nextEffect = null), s.effectTag = 8)), n && !i && 0 !== (2 & e.mode) && (null === t && !0 !== e.memoizedProps.unstable_avoidThisFallback || 0 !== (1 & Vs.current) ? Wa === Pa && (Wa = za) : (Wa !== Pa && Wa !== za || (Wa = Na), 0 !== qa && null !== Ua && (Ql(Ua, ja), Gl(Ua, qa)))), (n || i) && (e.effectTag |= 4), null);
+                            return pr(Vs), i = e.memoizedState, 0 !== (64 & e.effectTag) ? (e.expirationTime = n, e) : (n = null !== i, i = !1, null === t ? void 0 !== e.memoizedProps.fallback && Po(e) : (i = null !== (s = t.memoizedState), n || null === s || null !== (s = t.child.sibling) && (null !== (a = e.firstEffect) ? (e.firstEffect = s, s.nextEffect = a) : (e.firstEffect = e.lastEffect = s, s.nextEffect = null), s.effectTag = 8)), n && !i && 0 !== (2 & e.mode) && (null === t && !0 !== e.memoizedProps.unstable_avoidThisFallback || 0 !== (1 & Vs.current) ? Wa === Pa && (Wa = La) : (Wa !== Pa && Wa !== La || (Wa = Na), 0 !== qa && null !== Ua && (Ql(Ua, ja), Gl(Ua, qa)))), (n || i) && (e.effectTag |= 4), null);
                         case 4:
                             return Bs(), Xo(e), null;
                         case 10:
                             return os(e), null;
                         case 19:
                             if (pr(Vs), null === (i = e.memoizedState)) return null;
                             if (s = 0 !== (64 & e.effectTag), null === (a = i.rendering)) {
@@ -4689,15 +4689,15 @@
                         }
                         n.sibling.return = n.return, n = n.sibling
                     }
                 }, Xo = function() {}, qo = function(t, e, n, i, s) {
                     var o = t.memoizedProps;
                     if (o !== i) {
                         var a, l, c = e.stateNode;
-                        switch (zs(Ps.current), t = null, n) {
+                        switch (Ls(Ps.current), t = null, n) {
                             case "input":
                                 o = wt(c, o), i = wt(c, i), t = [];
                                 break;
                             case "option":
                                 o = Et(c, o), i = Et(c, i), t = [];
                                 break;
                             case "select":
@@ -4750,15 +4750,15 @@
 
                 function la(t) {
                     var e = t.ref;
                     if (null !== e)
                         if ("function" === typeof e) try {
                             e(null)
                         } catch (n) {
-                            Ll(t, n)
+                            zl(t, n)
                         } else e.current = null
                 }
 
                 function ca(t, e) {
                     switch (e.tag) {
                         case 0:
                         case 11:
@@ -4861,28 +4861,28 @@
                                     do {
                                         var n = t.destroy;
                                         if (void 0 !== n) {
                                             var r = e;
                                             try {
                                                 n()
                                             } catch (s) {
-                                                Ll(r, s)
+                                                zl(r, s)
                                             }
                                         }
                                         t = t.next
                                     } while (t !== i)
                                 }))
                             }
                             break;
                         case 1:
                             la(e), "function" === typeof(n = e.stateNode).componentWillUnmount && function(t, e) {
                                 try {
                                     e.props = t.memoizedProps, e.state = t.memoizedState, e.componentWillUnmount()
                                 } catch (n) {
-                                    Ll(t, n)
+                                    zl(t, n)
                                 }
                             }(e, n);
                             break;
                         case 5:
                             la(e);
                             break;
                         case 4:
@@ -5124,16 +5124,16 @@
                     Ea = Q.ReactCurrentOwner,
                     Da = 0,
                     Oa = 8,
                     Ca = 16,
                     Aa = 32,
                     Pa = 0,
                     Fa = 1,
-                    La = 2,
-                    za = 3,
+                    za = 2,
+                    La = 3,
                     Na = 4,
                     Ba = 5,
                     Ra = Da,
                     Ua = null,
                     Va = null,
                     ja = 0,
                     Wa = Pa,
@@ -5258,18 +5258,18 @@
                                 xl(t, l)
                             }
                             if (ss(), Ra = i, Ia.current = r, Wa === Fa) throw e = Ha, vl(t, n), Ql(t, n), pl(t), e;
                             if (null === Va) switch (r = t.finishedWork = t.current.alternate, t.finishedExpirationTime = n, i = Wa, Ua = null, i) {
                                 case Pa:
                                 case Fa:
                                     throw Error(o(345));
-                                case La:
+                                case za:
                                     Zl(t, 2 < n ? 2 : n);
                                     break;
-                                case za:
+                                case La:
                                     if (Ql(t, n), n === (i = t.lastSuspendedTime) && (t.nextKnownPendingLevel = El(r)), 1073741823 === Ya && 10 < (r = Qa + Ga - Yr())) {
                                         if (Ka) {
                                             var s = t.lastPingedTime;
                                             if (0 === s || s >= n) {
                                                 t.lastPingedTime = n, vl(t, n);
                                                 break
                                             }
@@ -5437,25 +5437,25 @@
                                                     } o.expirationTime = 1073741823;
                                                 break t
                                             }
                                             a = void 0, o = e;
                                             var b = r.pingCache;
                                             if (null === b ? (b = r.pingCache = new wa, a = new Set, b.set(l, a)) : void 0 === (a = b.get(l)) && (a = new Set, b.set(l, a)), !a.has(o)) {
                                                 a.add(o);
-                                                var v = zl.bind(null, r, l, o);
+                                                var v = Ll.bind(null, r, l, o);
                                                 l.then(v, v)
                                             }
                                             h.effectTag |= 4096, h.expirationTime = e;
                                             break t
                                         }
                                         h = h.return
                                     } while (null !== h);
                                     a = Error((mt(o.type) || "A React component") + " suspended while rendering, but no fallback UI was specified.\n\nAdd a <Suspense fallback=...> component higher in the tree to provide a loading indicator or placeholder to display." + yt(o))
                                 }
-                                Wa !== Ba && (Wa = La),
+                                Wa !== Ba && (Wa = za),
                                 a = sa(a, o),
                                 h = s;do {
                                     switch (h.tag) {
                                         case 3:
                                             l = a, h.effectTag |= 4096, h.expirationTime = e, gs(h, Sa(h, l, e));
                                             break t;
                                         case 1:
@@ -5606,15 +5606,15 @@
                             selectionRange: l
                         }, Xe = !1, Za = r;
                         do {
                             try {
                                 Cl()
                             } catch (M) {
                                 if (null === Za) throw Error(o(330));
-                                Ll(Za, M), Za = Za.nextEffect
+                                zl(Za, M), Za = Za.nextEffect
                             }
                         } while (null !== Za);
                         Za = r;
                         do {
                             try {
                                 for (a = t, l = e; null !== Za;) {
                                     var x = Za.effectTag;
@@ -5644,15 +5644,15 @@
                                         case 8:
                                             va(a, u = Za, l), pa(u)
                                     }
                                     Za = Za.nextEffect
                                 }
                             } catch (M) {
                                 if (null === Za) throw Error(o(330));
-                                Ll(Za, M), Za = Za.nextEffect
+                                zl(Za, M), Za = Za.nextEffect
                             }
                         } while (null !== Za);
                         if (w = wn, _ = gn(), x = w.focusedElem, l = w.selectionRange, _ !== x && x && x.ownerDocument && pn(x.ownerDocument.documentElement, x)) {
                             null !== l && mn(x) && (_ = l.start, void 0 === (w = l.end) && (w = _), "selectionStart" in x ? (x.selectionStart = _, x.selectionEnd = Math.min(w, x.value.length)) : (w = (_ = x.ownerDocument || document) && _.defaultView || window).getSelection && (w = w.getSelection(), u = x.textContent.length, a = Math.min(l.start, u), l = void 0 === l.end ? a : Math.min(l.end, u), !w.extend && a > l && (u = l, l = a, a = u), u = fn(x, a), h = fn(x, l), u && h && (1 !== w.rangeCount || w.anchorNode !== u.node || w.anchorOffset !== u.offset || w.focusNode !== h.node || w.focusOffset !== h.offset) && ((_ = _.createRange()).setStart(u.node, u.offset), w.removeAllRanges(), a > l ? (w.addRange(_), w.extend(h.node, h.offset)) : (_.setEnd(h.node, h.offset), w.addRange(_))))), _ = [];
                             for (w = x; w = w.parentNode;) 1 === w.nodeType && _.push({
                                 element: w,
                                 left: w.scrollLeft,
@@ -5673,15 +5673,15 @@
                                             Za.tag, _ = k, "function" === typeof T ? T(_) : T.current = _
                                         }
                                     }
                                     Za = Za.nextEffect
                                 }
                             } catch (M) {
                                 if (null === Za) throw Error(o(330));
-                                Ll(Za, M), Za = Za.nextEffect
+                                zl(Za, M), Za = Za.nextEffect
                             }
                         } while (null !== Za);
                         Za = null, Ur(), Ra = s
                     } else t.current = n;
                     if (nl) nl = !1, il = t, rl = e;
                     else
                         for (Za = r; null !== Za;) e = Za.nextEffect, Za.nextEffect = null, Za = e;
@@ -5718,26 +5718,26 @@
                                 case 11:
                                 case 15:
                                 case 22:
                                     ua(5, n), ha(5, n)
                             }
                         } catch (i) {
                             if (null === t) throw Error(o(330));
-                            Ll(t, i)
+                            zl(t, i)
                         }
                         n = t.nextEffect, t.nextEffect = null, t = n
                     }
                     return Ra = e, Gr(), !0
                 }
 
                 function Fl(t, e, n) {
                     ps(t, e = Sa(t, e = sa(n, e), 1073741823)), null !== (t = dl(t, 1073741823)) && pl(t)
                 }
 
-                function Ll(t, e) {
+                function zl(t, e) {
                     if (3 === t.tag) Fl(t, t, e);
                     else
                         for (var n = t.return; null !== n;) {
                             if (3 === n.tag) {
                                 Fl(n, t, e);
                                 break
                             }
@@ -5748,31 +5748,31 @@
                                     break
                                 }
                             }
                             n = n.return
                         }
                 }
 
-                function zl(t, e, n) {
+                function Ll(t, e, n) {
                     var i = t.pingCache;
-                    null !== i && i.delete(e), Ua === t && ja === n ? Wa === Na || Wa === za && 1073741823 === Ya && Yr() - Qa < Ga ? vl(t, ja) : Ka = !0 : Kl(t, n) && (0 !== (e = t.lastPingedTime) && e < n || (t.lastPingedTime = n, pl(t)))
+                    null !== i && i.delete(e), Ua === t && ja === n ? Wa === Na || Wa === La && 1073741823 === Ya && Yr() - Qa < Ga ? vl(t, ja) : Ka = !0 : Kl(t, n) && (0 !== (e = t.lastPingedTime) && e < n || (t.lastPingedTime = n, pl(t)))
                 }
 
                 function Nl(t, e) {
                     var n = t.stateNode;
                     null !== n && n.delete(e), 0 === (e = 0) && (e = ul(e = cl(), t, null)), null !== (t = dl(t, e)) && pl(t)
                 }
                 ka = function(t, e, n) {
                     var i = e.expirationTime;
                     if (null !== t) {
                         var r = e.pendingProps;
-                        if (t.memoizedProps !== r || br.current) zo = !0;
+                        if (t.memoizedProps !== r || br.current) Lo = !0;
                         else {
                             if (i < n) {
-                                switch (zo = !1, e.tag) {
+                                switch (Lo = !1, e.tag) {
                                     case 3:
                                         Yo(e), Fo();
                                         break;
                                     case 5:
                                         if (Rs(e), 4 & e.mode && 1 !== n && r.hidden) return e.expirationTime = e.childExpirationTime = 1, null;
                                         break;
                                     case 1:
@@ -5793,17 +5793,17 @@
                                             if (i) return ta(t, e, n);
                                             e.effectTag |= 64
                                         }
                                         if (null !== (r = e.memoizedState) && (r.rendering = null, r.tail = null), gr(Vs, Vs.current), !i) return null
                                 }
                                 return ea(t, e, n)
                             }
-                            zo = !1
+                            Lo = !1
                         }
-                    } else zo = !1;
+                    } else Lo = !1;
                     switch (e.expirationTime = 0, e.tag) {
                         case 2:
                             if (i = e.type, null !== t && (t.alternate = null, e.alternate = null, e.effectTag |= 2), t = e.pendingProps, r = xr(e, yr.current), ls(e, n), r = Js(null, e, i, t, r, n), e.effectTag |= 1, "object" === typeof r && null !== r && "function" === typeof r.render && void 0 === r.$$typeof) {
                                 if (e.tag = 1, e.memoizedState = null, e.updateQueue = null, _r(i)) {
                                     var s = !0;
                                     kr(e)
                                 } else s = !1;
@@ -6185,36 +6185,36 @@
                     switch (e) {
                         case "input":
                             if (kt(t, n), e = n.name, "radio" === n.type && null != e) {
                                 for (n = t; n.parentNode;) n = n.parentNode;
                                 for (n = n.querySelectorAll("input[name=" + JSON.stringify("" + e) + '][type="radio"]'), e = 0; e < n.length; e++) {
                                     var i = n[e];
                                     if (i !== t && i.form === t.form) {
-                                        var r = zn(i);
+                                        var r = Ln(i);
                                         if (!r) throw Error(o(90));
                                         _t(i), kt(i, r)
                                     }
                                 }
                             }
                             break;
                         case "textarea":
                             At(t, n);
                             break;
                         case "select":
                             null != (e = n.value) && Dt(t, !!n.multiple, e, !1)
                     }
-                }, F = yl, L = function(t, e, n, i, r) {
+                }, F = yl, z = function(t, e, n, i, r) {
                     var s = Ra;
                     Ra |= 4;
                     try {
                         return qr(98, t.bind(null, e, n, i, r))
                     } finally {
                         (Ra = s) === Da && Gr()
                     }
-                }, z = function() {
+                }, L = function() {
                     (Ra & (1 | Ca | Aa)) === Da && (function() {
                         if (null !== sl) {
                             var t = sl;
                             sl = null, t.forEach((function(t, e) {
                                 Zl(e, t), pl(e)
                             })), Gr()
                         }
@@ -6225,15 +6225,15 @@
                     try {
                         return t(e)
                     } finally {
                         (Ra = n) === Da && Gr()
                     }
                 };
                 var ac = {
-                    Events: [Fn, Ln, zn, M, S, Wn, function(t) {
+                    Events: [Fn, zn, Ln, M, S, Wn, function(t) {
                         se(t, jn)
                     }, A, P, Ze, le, Al, {
                         current: !1
                     }]
                 };
                 ! function(t) {
                     var e = t.findFiberByHostInstance;
@@ -6568,42 +6568,42 @@
                         case "object":
                             switch (t.$$typeof) {
                                 case s:
                                 case o:
                                     a = !0
                             }
                     }
-                    if (a) return n(i, t, "" === e ? "." + L(t, 0) : e), 1;
+                    if (a) return n(i, t, "" === e ? "." + z(t, 0) : e), 1;
                     if (a = 0, e = "" === e ? "." : e + ":", Array.isArray(t))
                         for (var l = 0; l < t.length; l++) {
-                            var c = e + L(r = t[l], l);
+                            var c = e + z(r = t[l], l);
                             a += P(r, c, n, i)
                         } else if (null === t || "object" !== typeof t ? c = null : c = "function" === typeof(c = m && t[m] || t["@@iterator"]) ? c : null, "function" === typeof c)
-                            for (t = c.call(t), l = 0; !(r = t.next()).done;) a += P(r = r.value, c = e + L(r, l++), n, i);
+                            for (t = c.call(t), l = 0; !(r = t.next()).done;) a += P(r = r.value, c = e + z(r, l++), n, i);
                         else if ("object" === r) throw n = "" + t, Error(y(31, "[object Object]" === n ? "object with keys {" + Object.keys(t).join(", ") + "}" : n, ""));
                     return a
                 }
 
                 function F(t, e, n) {
                     return null == t ? 0 : P(t, "", e, n)
                 }
 
-                function L(t, e) {
+                function z(t, e) {
                     return "object" === typeof t && null !== t && null != t.key ? function(t) {
                         var e = {
                             "=": "=0",
                             ":": "=2"
                         };
                         return "$" + ("" + t).replace(/[=:]/g, (function(t) {
                             return e[t]
                         }))
                     }(t.key) : e.toString(36)
                 }
 
-                function z(t, e) {
+                function L(t, e) {
                     t.func.call(t.context, e, t.count++)
                 }
 
                 function N(t, e, n) {
                     var i = t.result,
                         r = t.keyPrefix;
                     t = t.func.call(t.context, e, t.count++), Array.isArray(t) ? B(t, i, n, (function(t) {
@@ -6648,15 +6648,15 @@
                     map: function(t, e, n) {
                         if (null == t) return t;
                         var i = [];
                         return B(t, i, null, e, n), i
                     },
                     forEach: function(t, e, n) {
                         if (null == t) return t;
-                        F(t, z, e = C(null, null, e, n)), A(e)
+                        F(t, L, e = C(null, null, e, n)), A(e)
                     },
                     count: function(t) {
                         return F(t, (function() {
                             return null
                         }), null)
                     },
                     toArray: function(t) {
@@ -6882,46 +6882,46 @@
                 var E = [],
                     D = [],
                     O = 1,
                     C = null,
                     A = 3,
                     P = !1,
                     F = !1,
-                    L = !1;
+                    z = !1;
 
-                function z(t) {
+                function L(t) {
                     for (var e = k(D); null !== e;) {
                         if (null === e.callback) M(D);
                         else {
                             if (!(e.startTime <= t)) break;
                             M(D), e.sortIndex = e.expirationTime, T(E, e)
                         }
                         e = k(D)
                     }
                 }
 
                 function N(t) {
-                    if (L = !1, z(t), !F)
+                    if (z = !1, L(t), !F)
                         if (null !== k(E)) F = !0, n(B);
                         else {
                             var e = k(D);
                             null !== e && i(N, e.startTime - t)
                         }
                 }
 
                 function B(t, n) {
-                    F = !1, L && (L = !1, r()), P = !0;
+                    F = !1, z && (z = !1, r()), P = !0;
                     var o = A;
                     try {
-                        for (z(n), C = k(E); null !== C && (!(C.expirationTime > n) || t && !s());) {
+                        for (L(n), C = k(E); null !== C && (!(C.expirationTime > n) || t && !s());) {
                             var a = C.callback;
                             if (null !== a) {
                                 C.callback = null, A = C.priorityLevel;
                                 var l = a(C.expirationTime <= n);
-                                n = e.unstable_now(), "function" === typeof l ? C.callback = l : C === k(E) && M(E), z(n)
+                                n = e.unstable_now(), "function" === typeof l ? C.callback = l : C === k(E) && M(E), L(n)
                             } else M(E);
                             C = k(E)
                         }
                         if (null !== C) var c = !0;
                         else {
                             var u = k(D);
                             null !== u && i(N, u.startTime - n), c = !1
@@ -6999,18 +6999,18 @@
                     return t = {
                         id: O++,
                         callback: s,
                         priorityLevel: t,
                         startTime: l,
                         expirationTime: o = l + o,
                         sortIndex: -1
-                    }, l > a ? (t.sortIndex = l, T(D, t), null === k(E) && t === k(D) && (L ? r() : L = !0, i(N, l - a))) : (t.sortIndex = o, T(E, t), F || P || (F = !0, n(B))), t
+                    }, l > a ? (t.sortIndex = l, T(D, t), null === k(E) && t === k(D) && (z ? r() : z = !0, i(N, l - a))) : (t.sortIndex = o, T(E, t), F || P || (F = !0, n(B))), t
                 }, e.unstable_shouldYield = function() {
                     var t = e.unstable_now();
-                    z(t);
+                    L(t);
                     var n = k(E);
                     return n !== C && null !== C && null !== n && null !== n.callback && n.startTime <= t && n.expirationTime < C.expirationTime || s()
                 }, e.unstable_wrapCallback = function(t) {
                     var e = A;
                     return function() {
                         var n = A;
                         A = e;
@@ -7126,28 +7126,28 @@
                 }
                 constructor() {
                     throw t()
                 }
             }, !1]
         })(), x = t => "number" === typeof t, _ = t => "boolean" === typeof t, w = t => "function" === typeof t, S = t => null != t && Object(t) === t, T = t => S(t) && w(t.then), k = t => S(t) && w(t[Symbol.iterator]), M = t => S(t) && w(t[Symbol.asyncIterator]), I = t => S(t) && S(t.schema), E = t => S(t) && "done" in t && "value" in t, D = t => S(t) && w(t.stat) && x(t.fd), O = t => S(t) && A(t.body), C = t => "_getDOMStream" in t && "_getNodeStream" in t, A = t => S(t) && w(t.cancel) && w(t.getReader) && !C(t), P = t => S(t) && w(t.read) && w(t.pipe) && _(t.readable) && !C(t), F = t => S(t) && w(t.clear) && w(t.bytes) && w(t.position) && w(t.setPosition) && w(t.capacity) && w(t.getBufferIdentifier) && w(t.createLong);
 
-        function L(t) {
+        function z(t) {
             if (null === t) return "null";
             if (undefined === t) return "undefined";
             switch (typeof t) {
                 case "number":
                 case "bigint":
                     return "".concat(t);
                 case "string":
                     return '"'.concat(t, '"')
             }
-            return "function" === typeof t[Symbol.toPrimitive] ? t[Symbol.toPrimitive]("string") : ArrayBuffer.isView(t) ? "[".concat(t instanceof m || t instanceof b ? [...t].map((t => L(t))) : t, "]") : ArrayBuffer.isView(t) ? "[".concat(t, "]") : JSON.stringify(t, ((t, e) => "bigint" === typeof e ? "".concat(e) : e))
+            return "function" === typeof t[Symbol.toPrimitive] ? t[Symbol.toPrimitive]("string") : ArrayBuffer.isView(t) ? "[".concat(t instanceof m || t instanceof b ? [...t].map((t => z(t))) : t, "]") : ArrayBuffer.isView(t) ? "[".concat(t, "]") : JSON.stringify(t, ((t, e) => "bigint" === typeof e ? "".concat(e) : e))
         }
 
-        function z(t, e, n, i) {
+        function L(t, e, n, i) {
             return new(n || (n = Promise))((function(r, s) {
                 function o(t) {
                     try {
                         l(i.next(t))
                     } catch (e) {
                         s(e)
                     }
@@ -7583,15 +7583,15 @@
                 throw new Error("Unrecognized ".concat(this[Symbol.toStringTag], " type"))
             }
             toString() {
                 return "".concat(this.isSigned ? "I" : "Ui", "nt").concat(this.bitWidth)
             }
         }
         pt = Symbol.toStringTag, Ft[pt] = (t => (t.isSigned = null, t.bitWidth = null, t[Symbol.toStringTag] = "Int"))(Ft.prototype);
-        class Lt extends Ft {
+        class zt extends Ft {
             constructor() {
                 super(!0, 32)
             }
             get ArrayType() {
                 return Int32Array
             }
         }
@@ -7609,15 +7609,15 @@
                 super(!0, 16)
             }
             get ArrayType() {
                 return Int16Array
             }
         }.prototype, "ArrayType", {
             value: Int16Array
-        }), Object.defineProperty(Lt.prototype, "ArrayType", {
+        }), Object.defineProperty(zt.prototype, "ArrayType", {
             value: Int32Array
         }), Object.defineProperty(class extends Ft {
             constructor() {
                 super(!0, 64)
             }
             get ArrayType() {
                 return m
@@ -7657,15 +7657,15 @@
             }
             get ArrayType() {
                 return b
             }
         }.prototype, "ArrayType", {
             value: b
         });
-        class zt extends At {
+        class Lt extends At {
             constructor(t) {
                 super(), this.precision = t
             }
             get typeId() {
                 return c.Float
             }
             get ArrayType() {
@@ -7679,28 +7679,28 @@
                 }
                 throw new Error("Unrecognized ".concat(this[Symbol.toStringTag], " type"))
             }
             toString() {
                 return "Float".concat(this.precision << 5 || 16)
             }
         }
-        gt = Symbol.toStringTag, zt[gt] = (t => (t.precision = null, t[Symbol.toStringTag] = "Float"))(zt.prototype);
-        Object.defineProperty(class extends zt {
+        gt = Symbol.toStringTag, Lt[gt] = (t => (t.precision = null, t[Symbol.toStringTag] = "Float"))(Lt.prototype);
+        Object.defineProperty(class extends Lt {
             constructor() {
                 super(r.HALF)
             }
         }.prototype, "ArrayType", {
             value: Uint16Array
-        }), Object.defineProperty(class extends zt {
+        }), Object.defineProperty(class extends Lt {
             constructor() {
                 super(r.SINGLE)
             }
         }.prototype, "ArrayType", {
             value: Float32Array
-        }), Object.defineProperty(class extends zt {
+        }), Object.defineProperty(class extends Lt {
             constructor() {
                 super(r.DOUBLE)
             }
         }.prototype, "ArrayType", {
             value: Float64Array
         });
         class Nt extends At {
@@ -8537,15 +8537,15 @@
                     i = {};
                 for (let r = -1, s = n.length; ++r < s;) i[n[r].name] = en.visit(e.children[r], t);
                 return i
             }
             toString() {
                 return "{".concat([...this].map((t => {
                     let [e, n] = t;
-                    return "".concat(L(e), ": ").concat(L(n))
+                    return "".concat(z(e), ": ").concat(z(n))
                 })).join(", "), "}")
             } [Symbol.for("nodejs.util.inspect.custom")]() {
                 return this.toString()
             } [Symbol.iterator]() {
                 return new Ae(this[De], this[Oe])
             }
         }
@@ -8619,18 +8619,18 @@
             set(t, e, n) {
                 const i = t[De].type.children.findIndex((t => t.name === e));
                 return -1 !== i ? (Ee.visit(t[De].children[i], t[Oe], n), Reflect.set(t, e, n)) : !(!Reflect.has(t, e) && "symbol" !== typeof e) && Reflect.set(t, e, n)
             }
         }
         class Fe extends ee {}
 
-        function Le(t) {
+        function ze(t) {
             return (e, n) => e.getValid(n) ? t(e, n) : null
         }
-        const ze = (t, e) => 4294967296 * t[e + 1] + (t[e] >>> 0),
+        const Le = (t, e) => 4294967296 * t[e + 1] + (t[e] >>> 0),
             Ne = t => new Date(t),
             Be = (t, e, n) => {
                 if (n + 1 >= e.length) return null;
                 const i = e[n],
                     r = e[n + 1];
                 return t.subarray(i, r)
             },
@@ -8640,15 +8640,15 @@
                 } = t;
                 return ((t, e) => Ne(((t, e) => 864e5 * t[e])(t, e)))(n, e)
             },
             Ue = (t, e) => {
                 let {
                     values: n
                 } = t;
-                return ((t, e) => Ne(ze(t, e)))(n, 2 * e)
+                return ((t, e) => Ne(Le(t, e)))(n, 2 * e)
             },
             Ve = (t, e) => {
                 let {
                     stride: n,
                     values: i
                 } = t;
                 return i[n * e]
@@ -8659,21 +8659,21 @@
                 } = t;
                 return n[e]
             },
             We = (t, e) => {
                 let {
                     values: n
                 } = t;
-                return 1e3 * ze(n, 2 * e)
+                return 1e3 * Le(n, 2 * e)
             },
             He = (t, e) => {
                 let {
                     values: n
                 } = t;
-                return ze(n, 2 * e)
+                return Le(n, 2 * e)
             },
             Ye = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return ((t, e) => t[e + 1] / 1e3 * 4294967296 + (t[e] >>> 0) / 1e3)(n, 2 * e)
             },
@@ -8727,105 +8727,105 @@
                 let {
                     values: n
                 } = t;
                 const i = n[e],
                     r = new Int32Array(2);
                 return r[0] = Math.trunc(i / 12), r[1] = Math.trunc(i % 12), r
             };
-        Fe.prototype.visitNull = Le(((t, e) => null)), Fe.prototype.visitBool = Le(((t, e) => {
+        Fe.prototype.visitNull = ze(((t, e) => null)), Fe.prototype.visitBool = ze(((t, e) => {
             let {
                 offset: n,
                 values: i
             } = t;
             const r = n + e;
             return 0 !== (i[r >> 3] & 1 << r % 8)
-        })), Fe.prototype.visitInt = Le(((t, e) => {
+        })), Fe.prototype.visitInt = ze(((t, e) => {
             let {
                 values: n
             } = t;
             return n[e]
-        })), Fe.prototype.visitInt8 = Le(Ve), Fe.prototype.visitInt16 = Le(Ve), Fe.prototype.visitInt32 = Le(Ve), Fe.prototype.visitInt64 = Le(je), Fe.prototype.visitUint8 = Le(Ve), Fe.prototype.visitUint16 = Le(Ve), Fe.prototype.visitUint32 = Le(Ve), Fe.prototype.visitUint64 = Le(je), Fe.prototype.visitFloat = Le(((t, e) => {
+        })), Fe.prototype.visitInt8 = ze(Ve), Fe.prototype.visitInt16 = ze(Ve), Fe.prototype.visitInt32 = ze(Ve), Fe.prototype.visitInt64 = ze(je), Fe.prototype.visitUint8 = ze(Ve), Fe.prototype.visitUint16 = ze(Ve), Fe.prototype.visitUint32 = ze(Ve), Fe.prototype.visitUint64 = ze(je), Fe.prototype.visitFloat = ze(((t, e) => {
             let {
                 type: n,
                 values: i
             } = t;
             return n.precision !== r.HALF ? i[e] : oe(i[e])
-        })), Fe.prototype.visitFloat16 = Le(((t, e) => {
+        })), Fe.prototype.visitFloat16 = ze(((t, e) => {
             let {
                 stride: n,
                 values: i
             } = t;
             return oe(i[n * e])
-        })), Fe.prototype.visitFloat32 = Le(Ve), Fe.prototype.visitFloat64 = Le(Ve), Fe.prototype.visitUtf8 = Le(((t, e) => {
+        })), Fe.prototype.visitFloat32 = ze(Ve), Fe.prototype.visitFloat64 = ze(Ve), Fe.prototype.visitUtf8 = ze(((t, e) => {
             let {
                 values: n,
                 valueOffsets: i
             } = t;
             const r = Be(n, i, e);
             return null !== r ? W(r) : null
-        })), Fe.prototype.visitBinary = Le(((t, e) => {
+        })), Fe.prototype.visitBinary = ze(((t, e) => {
             let {
                 values: n,
                 valueOffsets: i
             } = t;
             return Be(n, i, e)
-        })), Fe.prototype.visitFixedSizeBinary = Le(((t, e) => {
+        })), Fe.prototype.visitFixedSizeBinary = ze(((t, e) => {
             let {
                 stride: n,
                 values: i
             } = t;
             return i.subarray(n * e, n * (e + 1))
-        })), Fe.prototype.visitDate = Le(((t, e) => t.type.unit === s.DAY ? Re(t, e) : Ue(t, e))), Fe.prototype.visitDateDay = Le(Re), Fe.prototype.visitDateMillisecond = Le(Ue), Fe.prototype.visitTimestamp = Le(((t, e) => {
+        })), Fe.prototype.visitDate = ze(((t, e) => t.type.unit === s.DAY ? Re(t, e) : Ue(t, e))), Fe.prototype.visitDateDay = ze(Re), Fe.prototype.visitDateMillisecond = ze(Ue), Fe.prototype.visitTimestamp = ze(((t, e) => {
             switch (t.type.unit) {
                 case o.SECOND:
                     return We(t, e);
                 case o.MILLISECOND:
                     return He(t, e);
                 case o.MICROSECOND:
                     return Ye(t, e);
                 case o.NANOSECOND:
                     return $e(t, e)
             }
-        })), Fe.prototype.visitTimestampSecond = Le(We), Fe.prototype.visitTimestampMillisecond = Le(He), Fe.prototype.visitTimestampMicrosecond = Le(Ye), Fe.prototype.visitTimestampNanosecond = Le($e), Fe.prototype.visitTime = Le(((t, e) => {
+        })), Fe.prototype.visitTimestampSecond = ze(We), Fe.prototype.visitTimestampMillisecond = ze(He), Fe.prototype.visitTimestampMicrosecond = ze(Ye), Fe.prototype.visitTimestampNanosecond = ze($e), Fe.prototype.visitTime = ze(((t, e) => {
             switch (t.type.unit) {
                 case o.SECOND:
                     return Xe(t, e);
                 case o.MILLISECOND:
                     return qe(t, e);
                 case o.MICROSECOND:
                     return Ke(t, e);
                 case o.NANOSECOND:
                     return Qe(t, e)
             }
-        })), Fe.prototype.visitTimeSecond = Le(Xe), Fe.prototype.visitTimeMillisecond = Le(qe), Fe.prototype.visitTimeMicrosecond = Le(Ke), Fe.prototype.visitTimeNanosecond = Le(Qe), Fe.prototype.visitDecimal = Le(((t, e) => {
+        })), Fe.prototype.visitTimeSecond = ze(Xe), Fe.prototype.visitTimeMillisecond = ze(qe), Fe.prototype.visitTimeMicrosecond = ze(Ke), Fe.prototype.visitTimeNanosecond = ze(Qe), Fe.prototype.visitDecimal = ze(((t, e) => {
             let {
                 values: n,
                 stride: i
             } = t;
             return ht.decimal(n.subarray(i * e, i * (e + 1)))
-        })), Fe.prototype.visitList = Le(((t, e) => {
+        })), Fe.prototype.visitList = ze(((t, e) => {
             const {
                 valueOffsets: n,
                 stride: i,
                 children: r
             } = t, {
                 [e * i]: s,
                 [e * i + 1]: o
             } = n, a = r[0].slice(s, o - s);
             return new $n([a])
-        })), Fe.prototype.visitStruct = Le(((t, e) => new Ce(t, e))), Fe.prototype.visitUnion = Le(((t, e) => t.type.mode === n.Dense ? Ge(t, e) : Ze(t, e))), Fe.prototype.visitDenseUnion = Le(Ge), Fe.prototype.visitSparseUnion = Le(Ze), Fe.prototype.visitDictionary = Le(((t, e) => {
+        })), Fe.prototype.visitStruct = ze(((t, e) => new Ce(t, e))), Fe.prototype.visitUnion = ze(((t, e) => t.type.mode === n.Dense ? Ge(t, e) : Ze(t, e))), Fe.prototype.visitDenseUnion = ze(Ge), Fe.prototype.visitSparseUnion = ze(Ze), Fe.prototype.visitDictionary = ze(((t, e) => {
             var n;
             return null === (n = t.dictionary) || void 0 === n ? void 0 : n.get(t.values[e])
-        })), Fe.prototype.visitInterval = Le(((t, e) => t.type.unit === a.DAY_TIME ? Je(t, e) : tn(t, e))), Fe.prototype.visitIntervalDayTime = Le(Je), Fe.prototype.visitIntervalYearMonth = Le(tn), Fe.prototype.visitFixedSizeList = Le(((t, e) => {
+        })), Fe.prototype.visitInterval = ze(((t, e) => t.type.unit === a.DAY_TIME ? Je(t, e) : tn(t, e))), Fe.prototype.visitIntervalDayTime = ze(Je), Fe.prototype.visitIntervalYearMonth = ze(tn), Fe.prototype.visitFixedSizeList = ze(((t, e) => {
             const {
                 stride: n,
                 children: i
             } = t, r = i[0].slice(e * n, n);
             return new $n([r])
-        })), Fe.prototype.visitMap = Le(((t, e) => {
+        })), Fe.prototype.visitMap = ze(((t, e) => {
             const {
                 valueOffsets: n,
                 children: i
             } = t, {
                 [e]: r,
                 [e + 1]: s
             } = n, o = i[0];
@@ -8852,15 +8852,15 @@
                     n = {};
                 for (let i = -1, r = t.length; ++i < r;) n[t.get(i)] = en.visit(e, i);
                 return n
             }
             toString() {
                 return "{".concat([...this].map((t => {
                     let [e, n] = t;
-                    return "".concat(L(e), ": ").concat(L(n))
+                    return "".concat(z(e), ": ").concat(z(n))
                 })).join(", "), "}")
             } [Symbol.for("nodejs.util.inspect.custom")]() {
                 return this.toString()
             }
         }
         class on {
             constructor(t, e) {
@@ -9235,45 +9235,45 @@
         }
         On.prototype.visitNull = function(t, e) {
             return null === e && t.length > 0 ? 0 : -1
         }, On.prototype.visitBool = Cn, On.prototype.visitInt = Cn, On.prototype.visitInt8 = Cn, On.prototype.visitInt16 = Cn, On.prototype.visitInt32 = Cn, On.prototype.visitInt64 = Cn, On.prototype.visitUint8 = Cn, On.prototype.visitUint16 = Cn, On.prototype.visitUint32 = Cn, On.prototype.visitUint64 = Cn, On.prototype.visitFloat = Cn, On.prototype.visitFloat16 = Cn, On.prototype.visitFloat32 = Cn, On.prototype.visitFloat64 = Cn, On.prototype.visitUtf8 = Cn, On.prototype.visitBinary = Cn, On.prototype.visitFixedSizeBinary = Cn, On.prototype.visitDate = Cn, On.prototype.visitDateDay = Cn, On.prototype.visitDateMillisecond = Cn, On.prototype.visitTimestamp = Cn, On.prototype.visitTimestampSecond = Cn, On.prototype.visitTimestampMillisecond = Cn, On.prototype.visitTimestampMicrosecond = Cn, On.prototype.visitTimestampNanosecond = Cn, On.prototype.visitTime = Cn, On.prototype.visitTimeSecond = Cn, On.prototype.visitTimeMillisecond = Cn, On.prototype.visitTimeMicrosecond = Cn, On.prototype.visitTimeNanosecond = Cn, On.prototype.visitDecimal = Cn, On.prototype.visitList = Cn, On.prototype.visitStruct = Cn, On.prototype.visitUnion = Cn, On.prototype.visitDenseUnion = An, On.prototype.visitSparseUnion = An, On.prototype.visitDictionary = Cn, On.prototype.visitInterval = Cn, On.prototype.visitIntervalDayTime = Cn, On.prototype.visitIntervalYearMonth = Cn, On.prototype.visitFixedSizeList = Cn, On.prototype.visitMap = Cn;
         const Pn = new On;
         class Fn extends ee {}
 
-        function Ln(t) {
+        function zn(t) {
             const {
                 type: e
             } = t;
-            if (0 === t.nullCount && 1 === t.stride && (e.typeId === c.Timestamp || e instanceof Ft && 64 !== e.bitWidth || e instanceof jt && 64 !== e.bitWidth || e instanceof zt && e.precision !== r.HALF)) return new pn(t.data.length, (e => {
+            if (0 === t.nullCount && 1 === t.stride && (e.typeId === c.Timestamp || e instanceof Ft && 64 !== e.bitWidth || e instanceof jt && 64 !== e.bitWidth || e instanceof Lt && e.precision !== r.HALF)) return new pn(t.data.length, (e => {
                 const n = t.data[e];
                 return n.values.subarray(0, n.length)[Symbol.iterator]()
             }));
             let n = 0;
             return new pn(t.data.length, (e => {
                 const i = t.data[e].length,
                     r = t.slice(n, n + i);
-                return n += i, new zn(r)
+                return n += i, new Ln(r)
             }))
         }
-        class zn {
+        class Ln {
             constructor(t) {
                 this.vector = t, this.index = 0
             }
             next() {
                 return this.index < this.vector.length ? {
                     value: this.vector.get(this.index++)
                 } : {
                     done: !0,
                     value: null
                 }
             } [Symbol.iterator]() {
                 return this
             }
         }
-        Fn.prototype.visitNull = Ln, Fn.prototype.visitBool = Ln, Fn.prototype.visitInt = Ln, Fn.prototype.visitInt8 = Ln, Fn.prototype.visitInt16 = Ln, Fn.prototype.visitInt32 = Ln, Fn.prototype.visitInt64 = Ln, Fn.prototype.visitUint8 = Ln, Fn.prototype.visitUint16 = Ln, Fn.prototype.visitUint32 = Ln, Fn.prototype.visitUint64 = Ln, Fn.prototype.visitFloat = Ln, Fn.prototype.visitFloat16 = Ln, Fn.prototype.visitFloat32 = Ln, Fn.prototype.visitFloat64 = Ln, Fn.prototype.visitUtf8 = Ln, Fn.prototype.visitBinary = Ln, Fn.prototype.visitFixedSizeBinary = Ln, Fn.prototype.visitDate = Ln, Fn.prototype.visitDateDay = Ln, Fn.prototype.visitDateMillisecond = Ln, Fn.prototype.visitTimestamp = Ln, Fn.prototype.visitTimestampSecond = Ln, Fn.prototype.visitTimestampMillisecond = Ln, Fn.prototype.visitTimestampMicrosecond = Ln, Fn.prototype.visitTimestampNanosecond = Ln, Fn.prototype.visitTime = Ln, Fn.prototype.visitTimeSecond = Ln, Fn.prototype.visitTimeMillisecond = Ln, Fn.prototype.visitTimeMicrosecond = Ln, Fn.prototype.visitTimeNanosecond = Ln, Fn.prototype.visitDecimal = Ln, Fn.prototype.visitList = Ln, Fn.prototype.visitStruct = Ln, Fn.prototype.visitUnion = Ln, Fn.prototype.visitDenseUnion = Ln, Fn.prototype.visitSparseUnion = Ln, Fn.prototype.visitDictionary = Ln, Fn.prototype.visitInterval = Ln, Fn.prototype.visitIntervalDayTime = Ln, Fn.prototype.visitIntervalYearMonth = Ln, Fn.prototype.visitFixedSizeList = Ln, Fn.prototype.visitMap = Ln;
+        Fn.prototype.visitNull = zn, Fn.prototype.visitBool = zn, Fn.prototype.visitInt = zn, Fn.prototype.visitInt8 = zn, Fn.prototype.visitInt16 = zn, Fn.prototype.visitInt32 = zn, Fn.prototype.visitInt64 = zn, Fn.prototype.visitUint8 = zn, Fn.prototype.visitUint16 = zn, Fn.prototype.visitUint32 = zn, Fn.prototype.visitUint64 = zn, Fn.prototype.visitFloat = zn, Fn.prototype.visitFloat16 = zn, Fn.prototype.visitFloat32 = zn, Fn.prototype.visitFloat64 = zn, Fn.prototype.visitUtf8 = zn, Fn.prototype.visitBinary = zn, Fn.prototype.visitFixedSizeBinary = zn, Fn.prototype.visitDate = zn, Fn.prototype.visitDateDay = zn, Fn.prototype.visitDateMillisecond = zn, Fn.prototype.visitTimestamp = zn, Fn.prototype.visitTimestampSecond = zn, Fn.prototype.visitTimestampMillisecond = zn, Fn.prototype.visitTimestampMicrosecond = zn, Fn.prototype.visitTimestampNanosecond = zn, Fn.prototype.visitTime = zn, Fn.prototype.visitTimeSecond = zn, Fn.prototype.visitTimeMillisecond = zn, Fn.prototype.visitTimeMicrosecond = zn, Fn.prototype.visitTimeNanosecond = zn, Fn.prototype.visitDecimal = zn, Fn.prototype.visitList = zn, Fn.prototype.visitStruct = zn, Fn.prototype.visitUnion = zn, Fn.prototype.visitDenseUnion = zn, Fn.prototype.visitSparseUnion = zn, Fn.prototype.visitDictionary = zn, Fn.prototype.visitInterval = zn, Fn.prototype.visitIntervalDayTime = zn, Fn.prototype.visitIntervalYearMonth = zn, Fn.prototype.visitFixedSizeList = zn, Fn.prototype.visitMap = zn;
         const Nn = new Fn,
             Bn = (t, e) => t + e;
         class Rn extends ee {
             visitNull(t, e) {
                 return 0
             }
             visitInt(t, e) {
@@ -10843,26 +10843,26 @@
                 }
                 return e
             }
             createStructOffsetList(t, e) {
                 return e(this, t.length), this.createObjectOffsetList(t), this.endVector()
             }
         }
-        class Li {
+        class zi {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsKeyValue(t, e) {
-                return (e || new Li).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new zi).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsKeyValue(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Li).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new zi).__init(t.readInt32(t.position()) + t.position(), t)
             }
             key(t) {
                 const e = this.bb.__offset(this.bb_pos, 4);
                 return e ? this.bb.__string(this.bb_pos + e, t) : null
             }
             value(t) {
                 const e = this.bb.__offset(this.bb_pos, 6);
@@ -10877,37 +10877,37 @@
             static addValue(t, e) {
                 t.addFieldOffset(1, e, 0)
             }
             static endKeyValue(t) {
                 return t.endObject()
             }
             static createKeyValue(t, e, n) {
-                return Li.startKeyValue(t), Li.addKey(t, e), Li.addValue(t, n), Li.endKeyValue(t)
+                return zi.startKeyValue(t), zi.addKey(t, e), zi.addValue(t, n), zi.endKeyValue(t)
             }
         }! function(t) {
             t[t.V1 = 0] = "V1", t[t.V2 = 1] = "V2", t[t.V3 = 2] = "V3", t[t.V4 = 3] = "V4", t[t.V5 = 4] = "V5"
         }(Di || (Di = {})),
         function(t) {
             t[t.Little = 0] = "Little", t[t.Big = 1] = "Big"
         }(Oi || (Oi = {})),
         function(t) {
             t[t.DenseArray = 0] = "DenseArray"
         }(Ci || (Ci = {}));
-        class zi {
+        class Li {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsInt(t, e) {
-                return (e || new zi).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Li).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsInt(t, e) {
-                return t.setPosition(t.position() + 4), (e || new zi).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Li).__init(t.readInt32(t.position()) + t.position(), t)
             }
             bitWidth() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return t ? this.bb.readInt32(this.bb_pos + t) : 0
             }
             isSigned() {
                 const t = this.bb.__offset(this.bb_pos, 6);
@@ -10922,15 +10922,15 @@
             static addIsSigned(t, e) {
                 t.addFieldInt8(1, +e, 0)
             }
             static endInt(t) {
                 return t.endObject()
             }
             static createInt(t, e, n) {
-                return zi.startInt(t), zi.addBitWidth(t, e), zi.addIsSigned(t, n), zi.endInt(t)
+                return Li.startInt(t), Li.addBitWidth(t, e), Li.addIsSigned(t, n), Li.endInt(t)
             }
         }
         class Ni {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
@@ -10944,15 +10944,15 @@
             }
             id() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return t ? this.bb.readInt64(this.bb_pos + t) : this.bb.createLong(0, 0)
             }
             indexType(t) {
                 const e = this.bb.__offset(this.bb_pos, 6);
-                return e ? (t || new zi).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
+                return e ? (t || new Li).__init(this.bb.__indirect(this.bb_pos + e), this.bb) : null
             }
             isOrdered() {
                 const t = this.bb.__offset(this.bb_pos, 8);
                 return !!t && !!this.bb.readInt8(this.bb_pos + t)
             }
             dictionaryKind() {
                 const t = this.bb.__offset(this.bb_pos, 10);
@@ -11018,15 +11018,15 @@
             }
             childrenLength() {
                 const t = this.bb.__offset(this.bb_pos, 14);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             customMetadata(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 16);
-                return n ? (e || new Li).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
+                return n ? (e || new zi).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
             }
             customMetadataLength() {
                 const t = this.bb.__offset(this.bb_pos, 16);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             static startField(t) {
                 t.startObject(7)
@@ -11095,15 +11095,15 @@
             }
             fieldsLength() {
                 const t = this.bb.__offset(this.bb_pos, 6);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             customMetadata(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 8);
-                return n ? (e || new Li).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
+                return n ? (e || new zi).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
             }
             customMetadataLength() {
                 const t = this.bb.__offset(this.bb_pos, 8);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             features(t) {
                 const e = this.bb.__offset(this.bb_pos, 10);
@@ -11200,15 +11200,15 @@
             }
             recordBatchesLength() {
                 const t = this.bb.__offset(this.bb_pos, 10);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             customMetadata(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 12);
-                return n ? (e || new Li).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
+                return n ? (e || new zi).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
             }
             customMetadataLength() {
                 const t = this.bb.__offset(this.bb_pos, 12);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             static startFooter(t) {
                 t.startObject(5)
@@ -11502,24 +11502,24 @@
             get closed() {
                 return this.reader ? this.reader.closed.catch((() => {})) : Promise.resolve()
             }
             releaseLock() {
                 this.reader && this.reader.releaseLock(), this.reader = null
             }
             cancel(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     const {
                         reader: e,
                         source: n
                     } = this;
                     e && (yield e.cancel(t).catch((() => {}))), n && n.locked && this.releaseLock()
                 }))
             }
             read(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     if (0 === t) return {
                         done: null == this.reader,
                         value: new Uint8Array(0)
                     };
                     const e = yield this.reader.read();
                     return !e.done && (e.value = G(e)), e
                 }))
@@ -11572,15 +11572,15 @@
             constructor() {
                 super(), this._values = [], this.resolvers = [], this._closedPromise = new Promise((t => this._closedPromiseResolve = t))
             }
             get closed() {
                 return this._closedPromise
             }
             cancel(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     yield this.return(t)
                 }))
             }
             write(t) {
                 this._ensureOpen() && (this.resolvers.length <= 0 ? this._values.push(t) : this.resolvers.shift().resolve({
                     done: !1,
                     value: t
@@ -11608,30 +11608,30 @@
             toDOMStream(t) {
                 return Xi.toDOMStream(this._closedPromiseResolve || this._error ? this : this._values, t)
             }
             toNodeStream(t) {
                 return Xi.toNodeStream(this._closedPromiseResolve || this._error ? this : this._values, t)
             }
             throw (t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return yield this.abort(t), Gi
                 }))
             }
             return (t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return yield this.close(), Gi
                 }))
             }
             read(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return (yield this.next(t, "read")).value
                 }))
             }
             peek(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return (yield this.next(t, "peek")).value
                 }))
             }
             next() {
                 return this._values.length > 0 ? Promise.resolve({
                     done: !1,
                     value: this._values.shift()
@@ -11654,15 +11654,15 @@
             write(t) {
                 if ((t = G(t)).byteLength > 0) return super.write(t)
             }
             toString() {
                 return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? W(this.toUint8Array(!0)) : this.toUint8Array(!1).then(W)
             }
             toUint8Array() {
-                return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? q(this._values)[0] : (() => z(this, void 0, void 0, (function*() {
+                return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? q(this._values)[0] : (() => L(this, void 0, void 0, (function*() {
                     var t, e;
                     const n = [];
                     let i = 0;
                     try {
                         for (var r, s = V(this); !(r = yield s.next()).done;) {
                             const t = r.value;
                             n.push(t), i += t.byteLength
@@ -11760,48 +11760,48 @@
             }
         }
         class sr {
             constructor(t) {
                 this.source = t, this._closedPromise = new Promise((t => this._closedPromiseResolve = t))
             }
             cancel(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     yield this.return(t)
                 }))
             }
             get closed() {
                 return this._closedPromise
             }
             read(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return (yield this.next(t, "read")).value
                 }))
             }
             peek(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return (yield this.next(t, "peek")).value
                 }))
             }
             next(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "read";
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return yield this.source.next({
                         cmd: e,
                         size: t
                     })
                 }))
             }
             throw (t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     const e = this.source.throw && (yield this.source.throw(t)) || Gi;
                     return this._closedPromiseResolve && this._closedPromiseResolve(), this._closedPromiseResolve = void 0, Object.create(e)
                 }))
             }
             return (t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     const e = this.source.return && (yield this.source.return(t)) || Gi;
                     return this._closedPromiseResolve && this._closedPromiseResolve(), this._closedPromiseResolve = void 0, Object.create(e)
                 }))
             }
         }
         class or extends nr {
             constructor(t, e) {
@@ -11844,34 +11844,34 @@
                     done: !0,
                     value: t
                 }
             }
         }
         class ar extends ir {
             constructor(t, e) {
-                super(), this.position = 0, this._handle = t, "number" === typeof e ? this.size = e : this._pending = (() => z(this, void 0, void 0, (function*() {
+                super(), this.position = 0, this._handle = t, "number" === typeof e ? this.size = e : this._pending = (() => L(this, void 0, void 0, (function*() {
                     this.size = (yield t.stat()).size, delete this._pending
                 })))()
             }
             readInt32(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     const {
                         buffer: e,
                         byteOffset: n
                     } = yield this.readAt(t, 4);
                     return new DataView(e, n).getInt32(0, !0)
                 }))
             }
             seek(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return this._pending && (yield this._pending), this.position = Math.min(t, this.size), t < this.size
                 }))
             }
             read(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     this._pending && (yield this._pending);
                     const {
                         _handle: e,
                         size: n,
                         position: i
                     } = this;
                     if (e && i < n) {
@@ -11887,44 +11887,44 @@
                         } = yield e.read(l, s, l.byteLength - s, r));
                         return l
                     }
                     return null
                 }))
             }
             readAt(t, e) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     this._pending && (yield this._pending);
                     const {
                         _handle: n,
                         size: i
                     } = this;
                     if (n && t + e < i) {
                         const r = Math.min(i, t + e),
                             s = new Uint8Array(r - t);
                         return (yield n.read(s, 0, e, t)).buffer
                     }
                     return new Uint8Array(e)
                 }))
             }
             close() {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     const t = this._handle;
                     this._handle = null, t && (yield t.close())
                 }))
             }
             throw (t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return yield this.close(), {
                         done: !0,
                         value: t
                     }
                 }))
             }
             return (t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return yield this.close(), {
                         done: !0,
                         value: t
                     }
                 }))
             }
         }
@@ -12849,26 +12849,26 @@
             }
             static createInterval(t, e) {
                 return Fr.startInterval(t), Fr.addUnit(t, e), Fr.endInterval(t)
             }
         }! function(t) {
             t[t.Sparse = 0] = "Sparse", t[t.Dense = 1] = "Dense"
         }(wr || (wr = {}));
-        class Lr {
+        class zr {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsUnion(t, e) {
-                return (e || new Lr).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new zr).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsUnion(t, e) {
-                return t.setPosition(t.position() + 4), (e || new Lr).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new zr).__init(t.readInt32(t.position()) + t.position(), t)
             }
             mode() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return t ? this.bb.readInt16(this.bb_pos + t) : wr.Sparse
             }
             typeIds(t) {
                 const e = this.bb.__offset(this.bb_pos, 6);
@@ -12899,29 +12899,29 @@
             static startTypeIdsVector(t, e) {
                 t.startVector(4, e, 4)
             }
             static endUnion(t) {
                 return t.endObject()
             }
             static createUnion(t, e, n) {
-                return Lr.startUnion(t), Lr.addMode(t, e), Lr.addTypeIds(t, n), Lr.endUnion(t)
+                return zr.startUnion(t), zr.addMode(t, e), zr.addTypeIds(t, n), zr.endUnion(t)
             }
         }
-        class zr {
+        class Lr {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
                 return this.bb_pos = t, this.bb = e, this
             }
             static getRootAsFixedSizeBinary(t, e) {
-                return (e || new zr).__init(t.readInt32(t.position()) + t.position(), t)
+                return (e || new Lr).__init(t.readInt32(t.position()) + t.position(), t)
             }
             static getSizePrefixedRootAsFixedSizeBinary(t, e) {
-                return t.setPosition(t.position() + 4), (e || new zr).__init(t.readInt32(t.position()) + t.position(), t)
+                return t.setPosition(t.position() + 4), (e || new Lr).__init(t.readInt32(t.position()) + t.position(), t)
             }
             byteWidth() {
                 const t = this.bb.__offset(this.bb_pos, 4);
                 return t ? this.bb.readInt32(this.bb_pos + t) : 0
             }
             static startFixedSizeBinary(t) {
                 t.startObject(1)
@@ -12929,15 +12929,15 @@
             static addByteWidth(t, e) {
                 t.addFieldInt32(0, e, 0)
             }
             static endFixedSizeBinary(t) {
                 return t.endObject()
             }
             static createFixedSizeBinary(t, e) {
-                return zr.startFixedSizeBinary(t), zr.addByteWidth(t, e), zr.endFixedSizeBinary(t)
+                return Lr.startFixedSizeBinary(t), Lr.addByteWidth(t, e), Lr.endFixedSizeBinary(t)
             }
         }
         class Nr {
             constructor() {
                 this.bb = null, this.bb_pos = 0
             }
             __init(t, e) {
@@ -13025,15 +13025,15 @@
             }
             bodyLength() {
                 const t = this.bb.__offset(this.bb_pos, 10);
                 return t ? this.bb.readInt64(this.bb_pos + t) : this.bb.createLong(0, 0)
             }
             customMetadata(t, e) {
                 const n = this.bb.__offset(this.bb_pos, 12);
-                return n ? (e || new Li).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
+                return n ? (e || new zi).__init(this.bb.__indirect(this.bb.__vector(this.bb_pos + n) + 4 * t), this.bb) : null
             }
             customMetadataLength() {
                 const t = this.bb.__offset(this.bb_pos, 12);
                 return t ? this.bb.__vector_len(this.bb_pos + t) : 0
             }
             static startMessage(t) {
                 t.startObject(5)
@@ -13217,15 +13217,15 @@
             visit(t, e) {
                 return null == t || null == e ? void 0 : super.visit(t, e)
             }
             visitNull(t, e) {
                 return Ur.startNull(e), Ur.endNull(e)
             }
             visitInt(t, e) {
-                return zi.startInt(e), zi.addBitWidth(e, t.bitWidth), zi.addIsSigned(e, t.isSigned), zi.endInt(e)
+                return Li.startInt(e), Li.addBitWidth(e, t.bitWidth), Li.addIsSigned(e, t.isSigned), Li.endInt(e)
             }
             visitFloat(t, e) {
                 return Dr.startFloatingPoint(e), Dr.addPrecision(e, t.precision), Dr.endFloatingPoint(e)
             }
             visitBinary(t, e) {
                 return Vr.startBinary(e), Vr.endBinary(e)
             }
@@ -13254,24 +13254,24 @@
             visitList(t, e) {
                 return Hr.startList(e), Hr.endList(e)
             }
             visitStruct(t, e) {
                 return Yr.startStruct_(e), Yr.endStruct_(e)
             }
             visitUnion(t, e) {
-                Lr.startTypeIdsVector(e, t.typeIds.length);
-                const n = Lr.createTypeIdsVector(e, t.typeIds);
-                return Lr.startUnion(e), Lr.addMode(e, t.mode), Lr.addTypeIds(e, n), Lr.endUnion(e)
+                zr.startTypeIdsVector(e, t.typeIds.length);
+                const n = zr.createTypeIdsVector(e, t.typeIds);
+                return zr.startUnion(e), zr.addMode(e, t.mode), zr.addTypeIds(e, n), zr.endUnion(e)
             }
             visitDictionary(t, e) {
                 const n = this.visit(t.indices, e);
                 return Ni.startDictionaryEncoding(e), Ni.addId(e, new $r(t.id, 0)), Ni.addIsOrdered(e, t.isOrdered), void 0 !== n && Ni.addIndexType(e, n), Ni.endDictionaryEncoding(e)
             }
             visitFixedSizeBinary(t, e) {
-                return zr.startFixedSizeBinary(e), zr.addByteWidth(e, t.byteWidth), zr.endFixedSizeBinary(e)
+                return Lr.startFixedSizeBinary(e), Lr.addByteWidth(e, t.byteWidth), Lr.endFixedSizeBinary(e)
             }
             visitFixedSizeList(t, e) {
                 return Nr.startFixedSizeList(e), Nr.addListSize(e, t.listSize), Nr.endFixedSizeList(e)
             }
             visitMap(t, e) {
                 return Br.startMap(e), Br.addKeysSorted(e, t.keysSorted), Br.endMap(e)
             }
@@ -13330,15 +13330,15 @@
             switch (i) {
                 case "int": {
                     const e = t.type;
                     return new Ft(e.isSigned, e.bitWidth)
                 }
                 case "floatingpoint": {
                     const e = t.type;
-                    return new zt(r[e.precision])
+                    return new Lt(r[e.precision])
                 }
                 case "decimal": {
                     const e = t.type;
                     return new Ut(e.scale, e.precision, e.bitWidth)
                 }
                 case "date": {
                     const e = t.type;
@@ -13537,20 +13537,20 @@
                 case Ai.List:
                     return new Yt((e || [])[0]);
                 case Ai.Struct_:
                     return new $t(e || [])
             }
             switch (n) {
                 case Ai.Int: {
-                    const e = t.type(new zi);
+                    const e = t.type(new Li);
                     return new Ft(e.isSigned(), e.bitWidth())
                 }
                 case Ai.FloatingPoint: {
                     const e = t.type(new Dr);
-                    return new zt(e.precision())
+                    return new Lt(e.precision())
                 }
                 case Ai.Decimal: {
                     const e = t.type(new Or);
                     return new Ut(e.scale(), e.precision(), e.bitWidth())
                 }
                 case Ai.Date: {
                     const e = t.type(new Cr);
@@ -13565,19 +13565,19 @@
                     return new Wt(e.unit(), e.timezone())
                 }
                 case Ai.Interval: {
                     const e = t.type(new Fr);
                     return new Ht(e.unit())
                 }
                 case Ai.Union: {
-                    const n = t.type(new Lr);
+                    const n = t.type(new zr);
                     return new Xt(n.mode(), n.typeIdsArray() || [], e || [])
                 }
                 case Ai.FixedSizeBinary: {
-                    const e = t.type(new zr);
+                    const e = t.type(new Lr);
                     return new qt(e.byteWidth())
                 }
                 case Ai.FixedSizeList: {
                     const n = t.type(new Nr);
                     return new Kt(n.listSize(), (e || [])[0])
                 }
                 case Ai.Map: {
@@ -13596,35 +13596,35 @@
             At.isDictionary(s) ? (o = s.dictionary.typeId, r = Xr.visit(s, t), i = Xr.visit(s.dictionary, t)) : i = Xr.visit(s, t);
             const a = (s.children || []).map((e => Zn.encode(t, e))),
                 l = Bi.createChildrenVector(t, a),
                 c = e.metadata && e.metadata.size > 0 ? Bi.createCustomMetadataVector(t, [...e.metadata].map((e => {
                     let [n, i] = e;
                     const r = t.createString("".concat(n)),
                         s = t.createString("".concat(i));
-                    return Li.startKeyValue(t), Li.addKey(t, r), Li.addValue(t, s), Li.endKeyValue(t)
+                    return zi.startKeyValue(t), zi.addKey(t, r), zi.addValue(t, s), zi.endKeyValue(t)
                 }))) : -1;
             e.name && (n = t.createString(e.name));
             Bi.startField(t), Bi.addType(t, i), Bi.addTypeType(t, o), Bi.addChildren(t, l), Bi.addNullable(t, !!e.nullable), -1 !== n && Bi.addName(t, n); - 1 !== r && Bi.addDictionary(t, r); - 1 !== c && Bi.addCustomMetadata(t, c);
             return Bi.endField(t)
         }, Zn.decode = function(t, e) {
             let n, i, r, s, o, a;
-            e && (a = t.dictionary()) ? e.has(n = a.id().low) ? (s = (s = a.indexType()) ? hs(s) : new Lt, o = new Jt(e.get(n), s, n, a.isOrdered()), i = new Zn(t.name(), o, t.nullable(), us(t))) : (s = (s = a.indexType()) ? hs(s) : new Lt, e.set(n, r = ds(t, cs(t, e))), o = new Jt(r, s, n, a.isOrdered()), i = new Zn(t.name(), o, t.nullable(), us(t))) : (r = ds(t, cs(t, e)), i = new Zn(t.name(), r, t.nullable(), us(t)));
+            e && (a = t.dictionary()) ? e.has(n = a.id().low) ? (s = (s = a.indexType()) ? hs(s) : new zt, o = new Jt(e.get(n), s, n, a.isOrdered()), i = new Zn(t.name(), o, t.nullable(), us(t))) : (s = (s = a.indexType()) ? hs(s) : new zt, e.set(n, r = ds(t, cs(t, e))), o = new Jt(r, s, n, a.isOrdered()), i = new Zn(t.name(), o, t.nullable(), us(t))) : (r = ds(t, cs(t, e)), i = new Zn(t.name(), r, t.nullable(), us(t)));
             return i || null
         }, Zn.fromJSON = function(t, e) {
             let n, i, r, s, o, a;
-            return e && (s = t.dictionary) ? e.has(n = s.id) ? (i = (i = s.indexType) ? Jr(i) : new Lt, a = new Jt(e.get(n), i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (i = (i = s.indexType) ? Jr(i) : new Lt, e.set(n, o = ts(t, Kr(t, e))), a = new Jt(o, i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (o = ts(t, Kr(t, e)), r = new Zn(t.name, o, t.nullable, Zr(t.customMetadata))), r || null
+            return e && (s = t.dictionary) ? e.has(n = s.id) ? (i = (i = s.indexType) ? Jr(i) : new zt, a = new Jt(e.get(n), i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (i = (i = s.indexType) ? Jr(i) : new zt, e.set(n, o = ts(t, Kr(t, e))), a = new Jt(o, i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (o = ts(t, Kr(t, e)), r = new Zn(t.name, o, t.nullable, Zr(t.customMetadata))), r || null
         }, Gn.encode = function(t, e) {
             const n = e.fields.map((e => Zn.encode(t, e)));
             Ri.startFieldsVector(t, n.length);
             const i = Ri.createFieldsVector(t, n),
                 r = e.metadata && e.metadata.size > 0 ? Ri.createCustomMetadataVector(t, [...e.metadata].map((e => {
                     let [n, i] = e;
                     const r = t.createString("".concat(n)),
                         s = t.createString("".concat(i));
-                    return Li.startKeyValue(t), Li.addKey(t, r), Li.addValue(t, s), Li.endKeyValue(t)
+                    return zi.startKeyValue(t), zi.addKey(t, r), zi.addValue(t, s), zi.endKeyValue(t)
                 }))) : -1;
             Ri.startSchema(t), Ri.addFields(t, i), Ri.addEndianness(t, fs ? Oi.Little : Oi.Big), -1 !== r && Ri.addCustomMetadata(t, r);
             return Ri.endSchema(t)
         }, Gn.decode = function(t) {
             let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : new Map;
             const n = function(t, e) {
                 const n = [];
@@ -13742,65 +13742,65 @@
         class vs {
             constructor(t, e) {
                 this.source = t instanceof ir ? t : D(t) ? new ar(t, e) : new ir(t)
             } [Symbol.asyncIterator]() {
                 return this
             }
             next() {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     let t;
                     return (t = yield this.readMetadataLength()).done || -1 === t.value && (t = yield this.readMetadataLength()).done || (t = yield this.readMetadata(t.value)).done ? Gi : t
                 }))
             }
             throw (t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return yield this.source.throw(t)
                 }))
             }
             return (t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return yield this.source.return(t)
                 }))
             }
             readMessage(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     let e;
                     if ((e = yield this.next()).done) return null;
                     if (null != t && e.value.headerType !== t) throw new Error(ps(t));
                     return e.value
                 }))
             }
             readMessageBody(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     if (t <= 0) return new Uint8Array(0);
                     const e = G(yield this.source.read(t));
                     if (e.byteLength < t) throw new Error(ys(t, e.byteLength));
                     return e.byteOffset % 8 === 0 && e.byteOffset + e.byteLength <= e.buffer.byteLength ? e : e.slice()
                 }))
             }
             readSchema() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     const e = l.Schema,
                         n = yield this.readMessage(e), i = null === n || void 0 === n ? void 0 : n.header();
                     if (t && !i) throw new Error(gs(e));
                     return i
                 }))
             }
             readMetadataLength() {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     const t = yield this.source.read(_s), e = t && new Pi(t), n = (null === e || void 0 === e ? void 0 : e.readInt32(0)) || 0;
                     return {
                         done: 0 === n,
                         value: n
                     }
                 }))
             }
             readMetadata(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     const e = yield this.source.read(t);
                     if (!e) return Gi;
                     if (e.byteLength < t) throw new Error(ms(t, e.byteLength));
                     return {
                         done: !1,
                         value: rs.decode(e)
                     }
@@ -13958,32 +13958,32 @@
             static throughDOM(t, e) {
                 throw new Error('"throughDOM" not available in this environment')
             }
             static from(t) {
                 return t instanceof Es ? t : I(t) ? function(t) {
                     return new Ds(new Bs(t))
                 }(t) : D(t) ? function(t) {
-                    return z(this, void 0, void 0, (function*() {
+                    return L(this, void 0, void 0, (function*() {
                         const {
                             size: e
                         } = yield t.stat(), n = new ar(t, e);
-                        return e >= Is && Ts(yield n.readAt(0, ks + 7 & -8)) ? new As(new Ns(n)) : new Os(new Ls(n))
+                        return e >= Is && Ts(yield n.readAt(0, ks + 7 & -8)) ? new As(new Ns(n)) : new Os(new zs(n))
                     }))
-                }(t) : T(t) ? (() => z(this, void 0, void 0, (function*() {
+                }(t) : T(t) ? (() => L(this, void 0, void 0, (function*() {
                     return yield Es.from(yield t)
                 })))() : O(t) || A(t) || P(t) || M(t) ? function(t) {
-                    return z(this, void 0, void 0, (function*() {
+                    return L(this, void 0, void 0, (function*() {
                         const e = yield t.peek(ks + 7 & -8);
-                        return e && e.byteLength >= 4 ? Ts(e) ? new Cs(new zs(yield t.read())) : new Os(new Ls(t)) : new Os(new Ls(function() {
+                        return e && e.byteLength >= 4 ? Ts(e) ? new Cs(new Ls(yield t.read())) : new Os(new zs(t)) : new Os(new zs(function() {
                             return R(this, arguments, (function*() {}))
                         }()))
                     }))
                 }(new ir(t)) : function(t) {
                     const e = t.peek(ks + 7 & -8);
-                    return e && e.byteLength >= 4 ? Ts(e) ? new Cs(new zs(t.read())) : new Ds(new Fs(t)) : new Ds(new Fs(function*() {}()))
+                    return e && e.byteLength >= 4 ? Ts(e) ? new Cs(new Ls(t.read())) : new Ds(new Fs(t)) : new Ds(new Fs(function*() {}()))
                 }(new nr(t))
             }
             static readAll(t) {
                 return t instanceof Es ? t.isSync() ? Us(t) : Vs(t) : I(t) || ArrayBuffer.isView(t) || k(t) || E(t) ? Us(t) : Vs(t)
             }
         }
         class Ds extends Es {
@@ -14002,15 +14002,15 @@
         }
         class Os extends Es {
             constructor(t) {
                 super(t), this._impl = t
             }
             readAll() {
                 var t, e;
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     const n = new Array;
                     try {
                         for (var i, r = V(this); !(i = yield r.next()).done;) {
                             const t = i.value;
                             n.push(t)
                         }
                     } catch (s) {
@@ -14150,48 +14150,48 @@
                     value: new bi(this.schema)
                 }) : this.return()
             }
             _readNextMessageAndValidate(t) {
                 return this._reader.readMessage(t)
             }
         }
-        class Ls extends Ps {
+        class zs extends Ps {
             constructor(t, e) {
                 super(e), this._reader = new vs(this._handle = t)
             }
             isAsync() {
                 return !0
             }
             isStream() {
                 return !0
             } [Symbol.asyncIterator]() {
                 return this
             }
             cancel() {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     !this.closed && (this.closed = !0) && (yield this.reset()._reader.return(), this._reader = null, this.dictionaries = null)
                 }))
             }
             open(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return this.closed || (this.autoDestroy = Rs(this, t), this.schema || (this.schema = yield this._reader.readSchema()) || (yield this.cancel())), this
                 }))
             }
             throw (t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return !this.closed && this.autoDestroy && (this.closed = !0) ? yield this.reset()._reader.throw(t): Gi
                 }))
             }
             return (t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return !this.closed && this.autoDestroy && (this.closed = !0) ? yield this.reset()._reader.return(t): Gi
                 }))
             }
             next() {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     if (this.closed) return Gi;
                     let t;
                     const {
                         _reader: e
                     } = this;
                     for (; t = yield this._readNextMessageAndValidate();)
                         if (t.isSchema()) yield this.reset(t.header());
@@ -14214,20 +14214,20 @@
                         } return this.schema && 0 === this._recordBatchIndex ? (this._recordBatchIndex++, {
                         done: !1,
                         value: new bi(this.schema)
                     }) : yield this.return()
                 }))
             }
             _readNextMessageAndValidate(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     return yield this._reader.readMessage(t)
                 }))
             }
         }
-        class zs extends Fs {
+        class Ls extends Fs {
             constructor(t, e) {
                 super(t instanceof or ? t : new or(t), e)
             }
             get footer() {
                 return this._footer
             }
             get numDictionaries() {
@@ -14288,15 +14288,15 @@
                 if (this._footer || this.open(), this._footer && this._recordBatchIndex < this.numRecordBatches) {
                     const n = null === (e = this._footer) || void 0 === e ? void 0 : e.getRecordBatch(this._recordBatchIndex);
                     if (n && this._handle.seek(n.offset)) return this._reader.readMessage(t)
                 }
                 return null
             }
         }
-        class Ns extends Ls {
+        class Ns extends zs {
             constructor(t) {
                 for (var e = arguments.length, n = new Array(e > 1 ? e - 1 : 0), i = 1; i < e; i++) n[i - 1] = arguments[i];
                 const r = "number" !== typeof n[0] ? n.shift() : void 0,
                     s = n[0] instanceof Map ? n.shift() : void 0;
                 super(t instanceof ar ? t : new ar(t, r), s)
             }
             get footer() {
@@ -14316,25 +14316,25 @@
             }
             open(t) {
                 const e = Object.create(null, {
                     open: {
                         get: () => super.open
                     }
                 });
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     if (!this.closed && !this._footer) {
                         this.schema = (this._footer = yield this._readFooter()).schema;
                         for (const t of this._footer.dictionaryBatches()) t && (yield this._readDictionaryBatch(this._dictionaryIndex++))
                     }
                     return yield e.open.call(this, t)
                 }))
             }
             readRecordBatch(t) {
                 var e;
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     if (this.closed) return null;
                     this._footer || (yield this.open());
                     const n = null === (e = this._footer) || void 0 === e ? void 0 : e.getRecordBatch(t);
                     if (n && (yield this._handle.seek(n.offset))) {
                         const t = yield this._reader.readMessage(l.RecordBatch);
                         if (null === t || void 0 === t ? void 0 : t.isRecordBatch()) {
                             const e = t.header(),
@@ -14343,39 +14343,39 @@
                         }
                     }
                     return null
                 }))
             }
             _readDictionaryBatch(t) {
                 var e;
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     const n = null === (e = this._footer) || void 0 === e ? void 0 : e.getDictionaryBatch(t);
                     if (n && (yield this._handle.seek(n.offset))) {
                         const t = yield this._reader.readMessage(l.DictionaryBatch);
                         if (null === t || void 0 === t ? void 0 : t.isDictionaryBatch()) {
                             const e = t.header(),
                                 n = yield this._reader.readMessageBody(t.bodyLength), i = this._loadDictionaryBatch(e, n);
                             this.dictionaries.set(e.id, i)
                         }
                     }
                 }))
             }
             _readFooter() {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     const {
                         _handle: t
                     } = this;
                     t._pending && (yield t._pending);
                     const e = t.size - Ms,
                         n = yield t.readInt32(e), i = yield t.readAt(e - n, n);
                     return Hi.decode(i)
                 }))
             }
             _readNextMessageAndValidate(t) {
-                return z(this, void 0, void 0, (function*() {
+                return L(this, void 0, void 0, (function*() {
                     if (this._footer || (yield this.open()), this._footer && this._recordBatchIndex < this.numRecordBatches) {
                         const e = this._footer.getRecordBatch(this._recordBatchIndex);
                         if (e && (yield this._handle.seek(e.offset))) return yield this._reader.readMessage(t)
                     }
                     return null
                 }))
             }
@@ -14683,15 +14683,15 @@
             e instanceof _i && (n = e.batches, t.reset(void 0, e.schema));
             for (const i of n) t.write(i);
             return t.finish()
         }
 
         function Zs(t, e) {
             var n, i, r, s;
-            return z(this, void 0, void 0, (function*() {
+            return L(this, void 0, void 0, (function*() {
                 try {
                     for (n = V(e); !(i = yield n.next()).done;) {
                         const e = i.value;
                         t.write(e)
                     }
                 } catch (o) {
                     r = {
@@ -15133,15 +15133,15 @@
                 F: "en",
                 K: "ch",
                 G: "arks",
                 H: "ea",
                 I: "ightg",
                 J: "wh"
             },
-            Lo = {
+            zo = {
                 OiceXe: "f0f8ff",
                 antiquewEte: "faebd7",
                 aqua: "ffff",
                 aquamarRe: "7fffd4",
                 azuY: "f0ffff",
                 beige: "f5f5dc",
                 bisque: "ffe4c4",
@@ -15283,29 +15283,29 @@
                 viTet: "ee82ee",
                 JHt: "f5deb3",
                 wEte: "ffffff",
                 wEtesmoke: "f5f5f5",
                 Lw: "ffff00",
                 LwgYF: "9acd32"
             };
-        let zo;
+        let Lo;
 
         function No(t) {
-            zo || (zo = function() {
+            Lo || (Lo = function() {
                 const t = {},
-                    e = Object.keys(Lo),
+                    e = Object.keys(zo),
                     n = Object.keys(Fo);
                 let i, r, s, o, a;
                 for (i = 0; i < e.length; i++) {
                     for (o = a = e[i], r = 0; r < n.length; r++) s = n[r], a = a.replace(s, Fo[s]);
-                    s = parseInt(Lo[o], 16), t[a] = [s >> 16 & 255, s >> 8 & 255, 255 & s]
+                    s = parseInt(zo[o], 16), t[a] = [s >> 16 & 255, s >> 8 & 255, 255 & s]
                 }
                 return t
-            }(), zo.transparent = [0, 0, 0, 0]);
-            const e = zo[t.toLowerCase()];
+            }(), Lo.transparent = [0, 0, 0, 0]);
+            const e = Lo[t.toLowerCase()];
             return e && {
                 r: e[0],
                 g: e[1],
                 b: e[2],
                 a: 4 === e.length ? e[3] : 255
             }
         }
@@ -15678,30 +15678,30 @@
             }
         }
 
         function Fa(t, e) {
             return Math.sqrt(Math.pow(e.x - t.x, 2) + Math.pow(e.y - t.y, 2))
         }
 
-        function La(t, e) {
+        function za(t, e) {
             return (t - e + ba) % ya - ma
         }
 
-        function za(t) {
+        function La(t) {
             return (t % ya + ya) % ya
         }
 
         function Na(t, e, n, i) {
-            const r = za(t),
-                s = za(e),
-                o = za(n),
-                a = za(s - r),
-                l = za(o - r),
-                c = za(r - s),
-                u = za(r - o);
+            const r = La(t),
+                s = La(e),
+                o = La(n),
+                a = La(s - r),
+                l = La(o - r),
+                c = La(r - s),
+                u = La(r - o);
             return r === s || r === o || i && s === o || a > l && c < u
         }
 
         function Ba(t, e, n) {
             return Math.max(e, Math.min(n, t))
         }
 
@@ -16281,36 +16281,36 @@
                 case "px":
                     return t;
                 case "%":
                     t /= 100
             }
             return e * t
         }
-        const Ll = t => +t || 0;
+        const zl = t => +t || 0;
 
-        function zl(t, e) {
+        function Ll(t, e) {
             const n = {},
                 i = Qo(e),
                 r = i ? Object.keys(e) : e,
                 s = Qo(t) ? i ? n => Jo(t[n], t[e[n]]) : e => t[e] : () => t;
-            for (const o of r) n[o] = Ll(s(o));
+            for (const o of r) n[o] = zl(s(o));
             return n
         }
 
         function Nl(t) {
-            return zl(t, {
+            return Ll(t, {
                 top: "y",
                 right: "x",
                 bottom: "y",
                 left: "x"
             })
         }
 
         function Bl(t) {
-            return zl(t, ["topLeft", "topRight", "bottomLeft", "bottomRight"])
+            return Ll(t, ["topLeft", "topRight", "bottomLeft", "bottomRight"])
         }
 
         function Rl(t) {
             const e = Nl(t);
             return e.width = e.left + e.right, e.height = e.top + e.bottom, e
         }
 
@@ -16810,16 +16810,16 @@
         function Ec(t, e) {
             void 0 !== e && (delete t.prevTextDirection, t.canvas.style.setProperty("direction", e[0], e[1]))
         }
 
         function Dc(t) {
             return "angle" === t ? {
                 between: Na,
-                compare: La,
-                normalize: za
+                compare: za,
+                normalize: La
             } : {
                 between: Ra,
                 compare: (t, e) => t - e,
                 normalize: t => t
             }
         }
 
@@ -16946,15 +16946,15 @@
                         t = Fc(i.setContext(jl(r, {
                             type: "segment",
                             p0: e,
                             p1: s,
                             p0DataIndex: (d - 1) % l,
                             p1DataIndex: d % l,
                             datasetIndex: o
-                        }))), Lc(t, u) && f(h, d - 1, p.loop, u), e = s, u = t
+                        }))), zc(t, u) && f(h, d - 1, p.loop, u), e = s, u = t
                     }
                     h < d - 1 && f(h, d - 1, p.loop, u)
                 }
                 return c
             }(t, e, n, i) : e
         }
 
@@ -16966,23 +16966,23 @@
                 borderDashOffset: t.borderDashOffset,
                 borderJoinStyle: t.borderJoinStyle,
                 borderWidth: t.borderWidth,
                 borderColor: t.borderColor
             }
         }
 
-        function Lc(t, e) {
+        function zc(t, e) {
             if (!e) return !1;
             const n = [],
                 i = function(t, e) {
                     return nl(e) ? (n.includes(e) || n.push(e), n.indexOf(e)) : e
                 };
             return JSON.stringify(t, i) !== JSON.stringify(e, i)
         }
-        class zc {
+        class Lc {
             constructor() {
                 this._request = null, this._charts = new Map, this._running = !1, this._lastDate = void 0
             }
             _notify(t, e, n, i) {
                 const r = e.listeners[i],
                     s = e.duration;
                 r.forEach((i => i({
@@ -17048,15 +17048,15 @@
                 for (; i >= 0; --i) n[i].cancel();
                 e.items = [], this._notify(t, e, Date.now(), "complete")
             }
             remove(t) {
                 return this._charts.delete(t)
             }
         }
-        var Nc = new zc;
+        var Nc = new Lc;
         const Bc = "transparent",
             Rc = {
                 boolean: (t, e, n) => n > .5 ? e : t,
                 color(t, e, n) {
                     const i = il(t || Bc),
                         r = i.valid && il(e || Bc);
                     return r && r.valid ? r.mix(i, n).hexString() : e
@@ -19164,15 +19164,15 @@
                 other: u
             } : {
                 same: u,
                 other: c
             }
         }
 
-        function Lu(t, e) {
+        function zu(t, e) {
             const n = e.maxPadding;
 
             function i(t) {
                 const i = {
                     left: 0,
                     top: 0,
                     right: 0,
@@ -19181,26 +19181,26 @@
                 return t.forEach((t => {
                     i[t] = Math.max(e[t], n[t])
                 })), i
             }
             return i(t ? ["left", "right"] : ["top", "bottom"])
         }
 
-        function zu(t, e, n, i) {
+        function Lu(t, e, n, i) {
             const r = [];
             let s, o, a, l, c, u;
             for (s = 0, o = t.length, c = 0; s < o; ++s) {
-                a = t[s], l = a.box, l.update(a.width || e.w, a.height || e.h, Lu(a.horizontal, e));
+                a = t[s], l = a.box, l.update(a.width || e.w, a.height || e.h, zu(a.horizontal, e));
                 const {
                     same: o,
                     other: h
                 } = Fu(e, n, a, i);
                 c |= o && r.length, u = u || h, l.fullSize || r.push(a)
             }
-            return c && zu(r, e, n, i) || u
+            return c && Lu(r, e, n, i) || u
         }
 
         function Nu(t, e, n, i, r) {
             t.top = n, t.left = e, t.right = e + i, t.bottom = n + r, t.width = i, t.height = r
         }
 
         function Bu(t, e, n, i) {
@@ -19309,15 +19309,15 @@
                         maxPadding: d,
                         w: s,
                         h: o,
                         x: r.left,
                         y: r.top
                     }, r),
                     p = Cu(l.concat(c), h);
-                zu(a.fullSize, f, h, p), zu(l, f, h, p), zu(c, f, h, p) && zu(l, f, h, p),
+                Lu(a.fullSize, f, h, p), Lu(l, f, h, p), Lu(c, f, h, p) && Lu(l, f, h, p),
                     function(t) {
                         const e = t.maxPadding;
 
                         function n(n) {
                             const i = Math.max(e[n] - t[n], 0);
                             return t[n] += i, i
                         }
@@ -20899,19 +20899,19 @@
                 }, i.set(r, s)
             }
             return s
         }
         const Ph = t => Qo(t) && Object.getOwnPropertyNames(t).some((e => pa(t[e])));
         const Fh = ["top", "bottom", "left", "right", "chartArea"];
 
-        function Lh(t, e) {
+        function zh(t, e) {
             return "top" === t || "bottom" === t || -1 === Fh.indexOf(t) && "x" === e
         }
 
-        function zh(t, e) {
+        function Lh(t, e) {
             return function(n, i) {
                 return n[t] === i[t] ? n[e] - i[e] : n[t] - i[t]
             }
         }
 
         function Nh(t) {
             const e = t.chart,
@@ -21051,15 +21051,15 @@
                         dtype: r ? "radialLinear" : s ? "category" : "linear"
                     }
                 })))), na(r, (e => {
                     const r = e.options,
                         s = r.id,
                         o = wh(s, r),
                         a = Jo(r.type, e.dtype);
-                    void 0 !== r.position && Lh(r.position, o) === Lh(e.dposition) || (r.position = e.dposition), i[s] = !0;
+                    void 0 !== r.position && zh(r.position, o) === zh(e.dposition) || (r.position = e.dposition), i[s] = !0;
                     let l = null;
                     if (s in n && n[s].type === a) l = n[s];
                     else {
                         l = new(mh.getScale(a))({
                             id: s,
                             type: a,
                             ctx: this.ctx,
@@ -21077,15 +21077,15 @@
                 const t = this._metasets,
                     e = this.data.datasets.length,
                     n = t.length;
                 if (t.sort(((t, e) => t.index - e.index)), n > e) {
                     for (let t = e; t < n; ++t) this._destroyDatasetMeta(t);
                     t.splice(e, n - e)
                 }
-                this._sortedMetasets = t.slice(0).sort(zh("order", "index"))
+                this._sortedMetasets = t.slice(0).sort(Lh("order", "index"))
             }
             _removeUnreferencedMetasets() {
                 const {
                     _metasets: t,
                     data: {
                         datasets: e
                     }
@@ -21143,15 +21143,15 @@
                     } = this.getDatasetMeta(l), e = !i && -1 === r.indexOf(t);
                     t.buildOrUpdateElements(e), s = Math.max(+t.getMaxOverflow(), s)
                 }
                 s = this._minPadding = n.layout.autoPadding ? s : 0, this._updateLayout(s), i || na(r, (t => {
                     t.reset()
                 })), this._updateDatasets(t), this.notifyPlugins("afterUpdate", {
                     mode: t
-                }), this._layers.sort(zh("z", "_idx"));
+                }), this._layers.sort(Lh("z", "_idx"));
                 const {
                     _active: o,
                     _lastEvent: a
                 } = this;
                 a ? this._eventHandler(a, !0) : o.length && this._updateHoverStyles(o, o, !0), this.render()
             }
             _updateScales() {
@@ -21505,15 +21505,15 @@
         }
 
         function Yh() {
             return na(Hh.instances, (t => t._plugins.invalidate()))
         }
 
         function $h(t, e, n, i) {
-            const r = zl(t.options.borderRadius, ["outerStart", "outerEnd", "innerStart", "innerEnd"]);
+            const r = Ll(t.options.borderRadius, ["outerStart", "outerEnd", "innerStart", "innerEnd"]);
             const s = (n - e) / 2,
                 o = Math.min(s, i * e / 2),
                 a = t => {
                     const e = (n - Math.min(s, t)) * i / 2;
                     return Ba(t, 0, Math.min(s, e))
                 };
             return {
@@ -22372,15 +22372,15 @@
             }
         };
 
         function Md(t, e, n, i) {
             if (i) return;
             let r = e[t],
                 s = n[t];
-            return "angle" === t && (r = za(r), s = za(s)), {
+            return "angle" === t && (r = La(r), s = La(s)), {
                 property: t,
                 start: r,
                 end: s
             }
         }
 
         function Id(t, e, n) {
@@ -22507,15 +22507,15 @@
             }
             return {
                 first: a,
                 last: l,
                 point: i
             }
         }
-        class Ld {
+        class zd {
             constructor(t) {
                 this.x = t.x, this.y = t.y, this.radius = t.radius
             }
             pathSegment(t, e, n) {
                 const {
                     x: i,
                     y: r,
@@ -22536,15 +22536,15 @@
                     x: e + Math.cos(r) * i,
                     y: n + Math.sin(r) * i,
                     angle: r
                 }
             }
         }
 
-        function zd(t) {
+        function Ld(t) {
             const {
                 chart: e,
                 fill: n,
                 line: i
             } = t;
             if (Go(n)) return function(t, e) {
                 const n = t.getDatasetMeta(e),
@@ -22588,15 +22588,15 @@
                         fill: n
                     } = t, i = e.options, r = e.getLabels().length, s = i.reverse ? e.max : e.min, o = function(t, e, n) {
                         let i;
                         return i = "start" === t ? n : "end" === t ? e.options.reverse ? e.min : e.max : Qo(t) ? t.value : e.getBaseValue(), i
                     }(n, e, s), a = [];
                     if (i.grid.circular) {
                         const t = e.getPointPositionForValue(0, s);
-                        return new Ld({
+                        return new zd({
                             x: t.x,
                             y: t.y,
                             radius: e.getDistanceFromCenterForValue(o)
                         })
                     }
                     for (let l = 0; l < r; ++l) a.push(e.getPointPositionForValue(l, o));
                     return a
@@ -22615,19 +22615,19 @@
                             x: t ? i : null,
                             y: t ? null : i
                         }
                     }
                     return null
                 }(t)
             }(t);
-            return r instanceof Ld ? r : Dd(r, i)
+            return r instanceof zd ? r : Dd(r, i)
         }
 
         function Nd(t, e, n) {
-            const i = zd(e),
+            const i = Ld(e),
                 {
                     line: r,
                     scale: s,
                     axis: o
                 } = e,
                 a = r.options,
                 l = a.fill,
@@ -24405,15 +24405,15 @@
                 const d = t.getPointPosition(h, t.drawingArea + r[h], a),
                     f = Ul(s.font),
                     p = (l = t.ctx, c = f, u = Ko(u = t._pointLabels[h]) ? u : [u], {
                         w: bl(l, c.string, u),
                         h: u.length * c.lineHeight
                     });
                 i[h] = p;
-                const g = za(t.getIndexAngle(h) + a),
+                const g = La(t.getIndexAngle(h) + a),
                     m = Math.round(Ca(g));
                 Of(n, e, g, Ef(m, d.x, p.w, 0, 180), Ef(m, d.y, p.h, 90, 270))
             }
             var l, c, u;
             t.setCenterPoint(e.l - n.l, n.r - e.r, e.t - n.t, n.b - e.b), t._pointLabelItems = function(t, e, n) {
                 const i = [],
                     r = t._pointLabels.length,
@@ -24449,15 +24449,15 @@
                 {
                     extra: r,
                     additionalAngle: s,
                     padding: o,
                     size: a
                 } = n,
                 l = t.getPointPosition(e, i + r + o, s),
-                c = Math.round(Ca(za(l.angle + _a))),
+                c = Math.round(Ca(La(l.angle + _a))),
                 u = function(t, e, n) {
                     90 === n || 270 === n ? t -= e / 2 : (n > 270 || n < 90) && (t -= e);
                     return t
                 }(l.y, a.h, c),
                 h = function(t) {
                     if (0 === t || 180 === t) return "center";
                     if (t < 180) return "left";
@@ -24544,15 +24544,15 @@
             ticks: {
                 callback: ul.formatters.logarithmic,
                 major: {
                     enabled: !0
                 }
             }
         });
-        class Lf extends vf {
+        class zf extends vf {
             constructor(t) {
                 super(t), this.xCenter = void 0, this.yCenter = void 0, this.drawingArea = void 0, this._pointLabels = [], this._pointLabelItems = []
             }
             setDimensions() {
                 const t = this._padding = Rl(If(this.options) / 2),
                     e = this.width = this.maxWidth - t.width,
                     n = this.height = this.maxHeight - t.height;
@@ -24578,15 +24578,15 @@
                 const t = this.options;
                 t.display && t.pointLabels.display ? Df(this) : this.setCenterPoint(0, 0, 0, 0)
             }
             setCenterPoint(t, e, n, i) {
                 this.xCenter += Math.floor((t - e) / 2), this.yCenter += Math.floor((n - i) / 2), this.drawingArea -= Math.min(this.drawingArea / 2, Math.max(t, e, n, i))
             }
             getIndexAngle(t) {
-                return za(t * (ya / (this._pointLabels.length || 1)) + Oa(this.options.startAngle || 0))
+                return La(t * (ya / (this._pointLabels.length || 1)) + Oa(this.options.startAngle || 0))
             }
             getDistanceFromCenterForValue(t) {
                 if (qo(t)) return NaN;
                 const e = this.drawingArea / (this.max - this.min);
                 return this.options.reverse ? (this.max - t) * e : (t - this.min) * e
             }
             getValueForDistanceFromCenter(t) {
@@ -24732,15 +24732,15 @@
                         strokeColor: a.textStrokeColor,
                         strokeWidth: a.textStrokeWidth
                     })
                 })), t.restore()
             }
             drawTitle() {}
         }
-        ho(Lf, "id", "radialLinear"), ho(Lf, "defaults", {
+        ho(zf, "id", "radialLinear"), ho(zf, "defaults", {
             display: !0,
             animate: !0,
             position: "chartArea",
             angleLines: {
                 display: !0,
                 lineWidth: 1,
                 borderDash: [],
@@ -24761,24 +24761,24 @@
                 font: {
                     size: 10
                 },
                 callback: t => t,
                 padding: 5,
                 centerPointLabels: !1
             }
-        }), ho(Lf, "defaultRoutes", {
+        }), ho(zf, "defaultRoutes", {
             "angleLines.color": "borderColor",
             "pointLabels.color": "color",
             "ticks.color": "color"
-        }), ho(Lf, "descriptors", {
+        }), ho(zf, "descriptors", {
             angleLines: {
                 _fallback: "grid"
             }
         });
-        const zf = {
+        const Lf = {
                 millisecond: {
                     common: !0,
                     size: 1,
                     steps: 1e3
                 },
                 second: {
                     common: !0,
@@ -24816,15 +24816,15 @@
                     steps: 4
                 },
                 year: {
                     common: !0,
                     size: 3154e7
                 }
             },
-            Nf = Object.keys(zf);
+            Nf = Object.keys(Lf);
 
         function Bf(t, e) {
             return t - e
         }
 
         function Rf(t, e) {
             if (qo(e)) return null;
@@ -24837,15 +24837,15 @@
             let o = e;
             return "function" === typeof i && (o = i(o)), Go(o) || (o = "string" === typeof i ? n.parse(o, i) : n.parse(o)), null === o ? null : (r && (o = "week" !== r || !Ea(s) && !0 !== s ? n.startOf(o, r) : n.startOf(o, "isoWeek", s)), +o)
         }
 
         function Uf(t, e, n, i) {
             const r = Nf.length;
             for (let s = Nf.indexOf(t); s < r - 1; ++s) {
-                const t = zf[Nf[s]],
+                const t = Lf[Nf[s]],
                     r = t.steps ? t.steps : Number.MAX_SAFE_INTEGER;
                 if (t.common && Math.ceil((n - e) / (r * t.size)) <= i) return Nf[s]
             }
             return Nf[r - 1]
         }
 
         function Vf(t, e, n) {
@@ -24944,20 +24944,20 @@
                         for (; i < r && t[i] < e;) i++;
                         for (; r > i && t[r - 1] > n;) r--;
                         return i > 0 || r < t.length ? t.slice(i, r) : t
                     }(i, r, this.max);
                 return this._unit = e.unit || (n.autoSkip ? Uf(e.minUnit, this.min, this.max, this._getLabelCapacity(r)) : function(t, e, n, i, r) {
                     for (let s = Nf.length - 1; s >= Nf.indexOf(n); s--) {
                         const n = Nf[s];
-                        if (zf[n].common && t._adapter.diff(r, i, n) >= e - 1) return n
+                        if (Lf[n].common && t._adapter.diff(r, i, n) >= e - 1) return n
                     }
                     return Nf[n ? Nf.indexOf(n) : 0]
                 }(this, s.length, e.minUnit, this.min, this.max)), this._majorUnit = n.major.enabled && "year" !== this._unit ? function(t) {
                     for (let e = Nf.indexOf(t) + 1, n = Nf.length; e < n; ++e)
-                        if (zf[Nf[e]].common) return Nf[e]
+                        if (Lf[Nf[e]].common) return Nf[e]
                 }(this._unit) : void 0, this.initOffsets(i), t.reverse && s.reverse(), jf(this, s, this._majorUnit)
             }
             afterAutoSkip() {
                 this.options.offsetAfterAutoskip && this.initOffsets(this.ticks.map((t => +t.value)))
             }
             initOffsets() {
                 let t, e, n = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : [],
@@ -25168,15 +25168,15 @@
         }
         ho(Yf, "id", "timeseries"), ho(Yf, "defaults", Wf.defaults);
         const $f = [mu, gd, ff, Object.freeze({
             __proto__: null,
             CategoryScale: mf,
             LinearScale: xf,
             LogarithmicScale: Mf,
-            RadialLinearScale: Lf,
+            RadialLinearScale: zf,
             TimeScale: Wf,
             TimeSeriesScale: Yf
         })];
         var Xf = i(895),
             qf = i.n(Xf);
         const Kf = t => t && t.enabled && t.modifierKey,
             Qf = (t, e) => t && e[t + "Key"],
@@ -25701,15 +25701,15 @@
                 return !o || (!(!e.panning && "mouse" === i.pointerType && (Gf(Kf(r), o) || Qf(Kf(s.drag), o))) || (ea(r.onPanRejected, [{
                     chart: t,
                     event: i
                 }]), !1))
             }
         }
 
-        function Lp(t, e, n) {
+        function zp(t, e, n) {
             if (e.scale) {
                 const {
                     center: i,
                     pointers: r
                 } = n, s = 1 / e.scale * n.scale, o = n.target.getBoundingClientRect(), a = function(t, e) {
                     const n = Math.abs(t.clientX - e.clientX),
                         i = Math.abs(t.clientY - e.clientY),
@@ -25727,15 +25727,15 @@
                         x: i.x - o.left,
                         y: i.y - o.top
                     }
                 }), e.scale = n.scale
             }
         }
 
-        function zp(t, e, n) {
+        function Lp(t, e, n) {
             const i = e.delta;
             i && (e.panning = !0, wp(t, {
                 x: n.deltaX - i.x,
                 y: n.deltaY - i.y
             }, e.panScales), e.delta = {
                 x: n.deltaX,
                 y: n.deltaY
@@ -25749,16 +25749,16 @@
                 {
                     pan: r,
                     zoom: s
                 } = e,
                 o = new(qf().Manager)(i);
             s && s.pinch.enabled && (o.add(new(qf().Pinch)), o.on("pinchstart", (() => function(t, e) {
                 e.options.zoom.pinch.enabled && (e.scale = 1)
-            }(0, n))), o.on("pinch", (e => Lp(t, n, e))), o.on("pinchend", (e => function(t, e, n) {
-                e.scale && (Lp(t, e, n), e.scale = null, ea(e.options.zoom.onZoomComplete, [{
+            }(0, n))), o.on("pinch", (e => zp(t, n, e))), o.on("pinchend", (e => function(t, e, n) {
+                e.scale && (zp(t, e, n), e.scale = null, ea(e.options.zoom.onZoomComplete, [{
                     chart: t
                 }]))
             }(t, n, e)))), r && r.enabled && (o.add(new(qf().Pan)({
                 threshold: r.threshold,
                 enable: Fp(t, n)
             })), o.on("panstart", (e => function(t, e, n) {
                 const {
@@ -25779,16 +25779,16 @@
                     }])) return ea(s, [{
                     chart: t,
                     event: n
                 }]);
                 e.panScales = tp(e.options.pan, a, t), e.delta = {
                     x: 0,
                     y: 0
-                }, clearTimeout(e.panEndTimeout), zp(t, e, n)
-            }(t, n, e))), o.on("panmove", (e => zp(t, n, e))), o.on("panend", (() => function(t, e) {
+                }, clearTimeout(e.panEndTimeout), Lp(t, e, n)
+            }(t, n, e))), o.on("panmove", (e => Lp(t, n, e))), o.on("panend", (() => function(t, e) {
                 e.delta = null, e.panning && (e.panEndTimeout = setTimeout((() => e.panning = !1), 500), ea(e.options.pan.onPanComplete, [{
                     chart: t
                 }]))
             }(t, n)))), Np.set(t, o)
         }
 
         function Rp(t, e, n) {
@@ -26564,15 +26564,15 @@
                         h = i.y;
                     return kg.lli8(r, s, o, a, l, c, u, h)
                 },
                 lli: function(t, e) {
                     return kg.lli4(t, t.c, e, e.c)
                 },
                 makeline: function(t, e) {
-                    return new Lg(t.x, t.y, (t.x + e.x) / 2, (t.y + e.y) / 2, e.x, e.y)
+                    return new zg(t.x, t.y, (t.x + e.x) / 2, (t.y + e.y) / 2, e.x, e.y)
                 },
                 findbbox: function(t) {
                     let e = wg,
                         n = wg,
                         i = Sg,
                         r = Sg;
                     return t.forEach((function(t) {
@@ -26892,15 +26892,15 @@
             min: Eg,
             max: Dg,
             cos: Og,
             sin: Cg,
             acos: Ag,
             sqrt: Pg
         } = Math, Fg = Math.PI;
-        class Lg {
+        class zg {
             constructor(t) {
                 let e = t && t.forEach ? t : Array.from(arguments).slice(),
                     n = !1;
                 if ("object" === typeof e[0]) {
                     n = e.length;
                     const t = [];
                     e.forEach((function(e) {
@@ -26933,22 +26933,22 @@
                         p1: o[0],
                         p2: o[l]
                     }),
                     h = kg.dist(o[0], o[l]);
                 this._linear = u.reduce(((t, e) => t + Ig(e.y)), 0) < h / 50, this._lut = [], this._t1 = 0, this._t2 = 1, this.update()
             }
             static quadraticFromPoints(t, e, n, i) {
-                if ("undefined" === typeof i && (i = .5), 0 === i) return new Lg(e, e, n);
-                if (1 === i) return new Lg(t, e, e);
-                const r = Lg.getABC(2, t, e, n, i);
-                return new Lg(t, r.A, n)
+                if ("undefined" === typeof i && (i = .5), 0 === i) return new zg(e, e, n);
+                if (1 === i) return new zg(t, e, e);
+                const r = zg.getABC(2, t, e, n, i);
+                return new zg(t, r.A, n)
             }
             static cubicFromPoints(t, e, n, i, r) {
                 "undefined" === typeof i && (i = .5);
-                const s = Lg.getABC(3, t, e, n, i);
+                const s = zg.getABC(3, t, e, n, i);
                 "undefined" === typeof r && (r = kg.dist(e, s.C));
                 const o = r * (1 - i) / i,
                     a = kg.dist(t, n),
                     l = (n.x - t.x) / a,
                     c = (n.y - t.y) / a,
                     u = r * l,
                     h = r * c,
@@ -26967,21 +26967,21 @@
                         x: t.x + (v - t.x) / i,
                         y: t.y + (x - t.y) / i
                     },
                     T = {
                         x: n.x + (_ - n.x) / (1 - i),
                         y: n.y + (w - n.y) / (1 - i)
                     };
-                return new Lg(t, S, T, n)
+                return new zg(t, S, T, n)
             }
             static getUtils() {
                 return kg
             }
             getUtils() {
-                return Lg.getUtils()
+                return zg.getUtils()
             }
             static get PolyBezier() {
                 return Mg
             }
             valueOf() {
                 return this.toString()
             }
@@ -27043,15 +27043,15 @@
                     E: i
                 }
             }
             getABC(t, e) {
                 e = e || this.get(t);
                 let n = this.points[0],
                     i = this.points[this.order];
-                return Lg.getABC(this.order, n, e, i, t)
+                return zg.getABC(this.order, n, e, i, t)
             }
             getLUT(t) {
                 if (this.verify(), t = t || 100, this._lut.length === t + 1) return this._lut;
                 this._lut = [], t++, this._lut = [];
                 for (let e, n, i = 0; i < t; i++) n = i / (t - 1), e = this.compute(n), e.t = n, this._lut.push(e);
                 return this._lut
             }
@@ -27090,25 +27090,25 @@
                 const t = this.points,
                     e = [t[0]],
                     n = t.length;
                 for (let i, r, s = 1; s < n; s++) i = t[s], r = t[s - 1], e[s] = {
                     x: (n - s) / n * i.x + s / n * r.x,
                     y: (n - s) / n * i.y + s / n * r.y
                 };
-                return e[n] = t[n - 1], new Lg(e)
+                return e[n] = t[n - 1], new zg(e)
             }
             derivative(t) {
                 return kg.compute(t, this.dpoints[0], this._3d)
             }
             dderivative(t) {
                 return kg.compute(t, this.dpoints[1], this._3d)
             }
             align() {
                 let t = this.points;
-                return new Lg(kg.align(t, {
+                return new zg(kg.align(t, {
                     p1: t[0],
                     p2: t[t.length - 1]
                 }))
             }
             curvature(t) {
                 return kg.curvature(t, this.dpoints[0], this.dpoints[1], this._3d)
             }
@@ -27161,16 +27161,16 @@
                 return i
             }
             split(t, e) {
                 if (0 === t && e) return this.split(e).left;
                 if (1 === e) return this.split(t).right;
                 const n = this.hull(t),
                     i = {
-                        left: 2 === this.order ? new Lg([n[0], n[3], n[5]]) : new Lg([n[0], n[4], n[7], n[9]]),
-                        right: 2 === this.order ? new Lg([n[5], n[4], n[2]]) : new Lg([n[9], n[8], n[6], n[3]]),
+                        left: 2 === this.order ? new zg([n[0], n[3], n[5]]) : new zg([n[0], n[4], n[7], n[9]]),
+                        right: 2 === this.order ? new zg([n[5], n[4], n[2]]) : new zg([n[9], n[8], n[6], n[3]]),
                         span: n
                     };
                 return i.left._t1 = kg.map(0, 0, 1, this._t1, this._t2), i.left._t2 = kg.map(t, 0, 1, this._t1, this._t2), i.right._t1 = kg.map(t, 0, 1, this._t1, this._t2), i.right._t2 = kg.map(1, 0, 1, this._t1, this._t2), e ? (e = kg.map(e, t, 1, 0, 1), i.right.split(e).left) : i
             }
             extrema() {
                 const t = {};
                 let e = [];
@@ -27215,15 +27215,15 @@
                         n = this.points.map((function(n) {
                             const i = {
                                 x: n.x + t * e.x,
                                 y: n.y + t * e.y
                             };
                             return n.z && e.z && (i.z = n.z + t * e.z), i
                         }));
-                    return [new Lg(n)]
+                    return [new zg(n)]
                 }
                 return this.reduce().map((function(e) {
                     return e._linear ? e.offset(t)[0] : e.scale(t)
                 }))
             }
             simple() {
                 if (3 === this.order) {
@@ -27254,15 +27254,15 @@
                             } n < 1 && (e = t.split(n, 1), e._t1 = kg.map(n, 0, 1, t._t1, t._t2), e._t2 = t._t2, o.push(e))
                 })), o
             }
             translate(t, e, n) {
                 n = "number" === typeof n ? n : e;
                 const i = this.order;
                 let r = this.points.map(((t, r) => (1 - r / i) * e + r / i * n));
-                return new Lg(this.points.map(((e, n) => ({
+                return new zg(this.points.map(((e, n) => ({
                     x: e.x + t.x * r[n],
                     y: e.y + t.y * r[n]
                 }))))
             }
             scale(t) {
                 const e = this.order;
                 let n = !1;
@@ -27290,24 +27290,24 @@
                         n && !i && (u = -u);
                         var h = Pg(a.x * a.x + a.y * a.y);
                         a.x /= h, a.y /= h, l[s + 1] = {
                             x: o.x + u * a.x,
                             y: o.y + u * a.y
                         }
                     }
-                })), new Lg(l)) : ([0, 1].forEach((t => {
+                })), new zg(l)) : ([0, 1].forEach((t => {
                     if (2 === e && t) return;
                     const n = l[t * e],
                         i = this.derivative(t),
                         s = {
                             x: n.x + i.x,
                             y: n.y + i.y
                         };
                     l[t + 1] = kg.lli4(n, s, c, r[t + 1])
-                })), new Lg(l))
+                })), new zg(l))
             }
             outline(t, e, n, i) {
                 if (e = void 0 === e ? t : e, this._linear) {
                     const r = this.normal(0),
                         s = this.points[0],
                         o = this.points[this.points.length - 1];
                     let a, l, c;
@@ -27331,15 +27331,15 @@
                     }, l = {
                         x: (a.x + c.x) / 2,
                         y: (a.y + c.y) / 2
                     };
                     const h = [c, l, a],
                         d = kg.makeline(h[2], u[0]),
                         f = kg.makeline(u[2], h[0]),
-                        p = [d, new Lg(u), f, new Lg(h)];
+                        p = [d, new zg(u), f, new zg(h)];
                     return new Mg(p)
                 }
                 const r = this.reduce(),
                     s = r.length,
                     o = [];
                 let a, l = [],
                     c = 0,
@@ -27376,15 +27376,15 @@
                 for (let s = 1, o = i.length; s < o / 2; s++) {
                     const t = kg.makeshape(i[s], i[o - s], n);
                     t.startcap.virtual = s > 1, t.endcap.virtual = s < o / 2 - 1, r.push(t)
                 }
                 return r
             }
             intersects(t, e) {
-                return t ? t.p1 && t.p2 ? this.lineIntersects(t) : (t instanceof Lg && (t = t.reduce()), this.curveintersects(this.reduce(), t, e)) : this.selfintersects(e)
+                return t ? t.p1 && t.p2 ? this.lineIntersects(t) : (t instanceof zg && (t = t.reduce()), this.curveintersects(this.reduce(), t, e)) : this.selfintersects(e)
             }
             lineIntersects(t) {
                 const e = Eg(t.p1.x, t.p2.x),
                     n = Eg(t.p1.y, t.p2.y),
                     i = Dg(t.p1.x, t.p2.x),
                     r = Dg(t.p1.y, t.p2.y);
                 return kg.roots(this.points, t).filter((t => {
@@ -27461,15 +27461,15 @@
                     } while (!c && n++ < 100);
                     if (n >= 100) break;
                     l = l || a, e.push(l), i = p
                 } while (r < 1);
                 return e
             }
         }
-        const zg = {
+        const Lg = {
                 aliceblue: [240, 248, 255],
                 antiquewhite: [250, 235, 215],
                 aqua: [0, 255, 255],
                 aquamarine: [127, 255, 212],
                 azure: [240, 255, 255],
                 beige: [245, 245, 220],
                 bisque: [255, 228, 196],
@@ -27624,15 +27624,15 @@
                     alpha: 1
                 };
                 if ("number" === typeof t) return {
                     space: "rgb",
                     values: [t >>> 16, (65280 & t) >>> 8, 255 & t],
                     alpha: 1
                 };
-                if (t = String(t).toLowerCase(), zg[t]) i = zg[t].slice(), n = "rgb";
+                if (t = String(t).toLowerCase(), Lg[t]) i = Lg[t].slice(), n = "rgb";
                 else if ("transparent" === t) r = 0, n = "rgb", i = [0, 0, 0];
                 else if ("#" === t[0]) {
                     var s = t.slice(1),
                         o = s.length;
                     r = 1, o <= 4 ? (i = [parseInt(s[0] + s[0], 16), parseInt(s[1] + s[1], 16), parseInt(s[2] + s[2], 16)], 4 === o && (r = parseInt(s[3] + s[3], 16) / 255)) : (i = [parseInt(s[0] + s[1], 16), parseInt(s[2] + s[3], 16), parseInt(s[4] + s[5], 16)], 8 === o && (r = parseInt(s[6] + s[7], 16) / 255)), i[0] || (i[0] = 0), i[1] || (i[1] = 0), i[2] || (i[2] = 0), n = "rgb"
                 } else if (e = /^((?:rgba?|hs[lvb]a?|hwba?|cmyk?|xy[zy]|gray|lab|lchu?v?|[ly]uv|lms|oklch|oklab|color))\s*\(([^\)]*)\)/.exec(t)) {
                     var a = e[1],
@@ -27747,15 +27747,15 @@
                     const r = i.x.map(((t, e) => ({
                             x: t,
                             y: i.y[e]
                         }))),
                         s = [];
                     for (let a = 0; a < r.length - 2; a += 2) {
                         const t = r.slice(a, a + 3),
-                            e = new Lg(t).getLUT(10);
+                            e = new zg(t).getLUT(10);
                         s.push(...e)
                     }
                     const o = Vg(i.color);
                     return {
                         label: n + " (bezier)",
                         data: s,
                         isControlPoint: !1,
@@ -27870,57 +27870,341 @@
                 r = t[1] / 255,
                 s = t[2] / 255,
                 o = Math.min(i, r, s),
                 a = Math.max(i, r, s),
                 l = a - o;
             return a === o ? e = 0 : i === a ? e = (r - s) / l : r === a ? e = 2 + (s - i) / l : s === a && (e = 4 + (i - r) / l), (e = Math.min(60 * e, 360)) < 0 && (e += 360), n = (o + a) / 2, [e, 100 * (a === o ? 0 : n <= .5 ? l / (a + o) : l / (2 - a - o)), 100 * n]
         }, Hh.register(...$f, Up);
-        const qg = {
+        const qg = class extends ao {
+            constructor(t) {
+                super(t), this.downHandler = t => {
+                    const e = $p(this.chartRef.current, t);
+                    if (e.length > 0) {
+                        this.chartRef.current.data.datasets[e[0].datasetIndex].isControlPoint && (this.setState({
+                            activePoint: e[0]
+                        }), this.togglePan(!1))
+                    }
+                }, this.calculateNewYValue = (t, e, n) => this.map(t.y, e.bottom, e.top, n.min, n.max), this.calculateNewXValue = (t, e, n) => this.map(t.x, e.left, e.right, n.min, n.max), this.updateControlPointPosition = (t, e, n, i) => {
+                    const r = e.datasetIndex,
+                        s = e.index;
+                    t.data.datasets[r].data[s].x = n, t.data.datasets[r].data[s].y = i
+                }, this.updateOriginalData = (t, e) => {
+                    const n = e.datasetIndex,
+                        i = e.index,
+                        r = t.data.datasets[n].label,
+                        s = t.data.datasets[n].data[i].x,
+                        o = t.data.datasets[n].data[i].y;
+                    this.state.originalData[r].x[i] = s, this.state.originalData[r].y[i] = o
+                }, this.moveHandler = t => {
+                    if (this.state.activePoint) {
+                        const e = this.chartRef.current,
+                            n = this.state.activePoint,
+                            i = yc(t, e),
+                            r = e.chartArea,
+                            s = this.calculateNewYValue(i, r, e.scales.y),
+                            o = this.calculateNewXValue(i, r, e.scales.x);
+                        this.updateControlPointPosition(e, n, o, s), this.updateOriginalData(e, n);
+                        const a = Wg(this.state.originalData, this.props.args.options);
+                        this.setState({
+                            bezierData: a
+                        }), e.update("none")
+                    }
+                }, this.upHandler = t => {
+                    this.state.activePoint && (this.sendBezierData(), this.setState({
+                        activePoint: null
+                    }), this.togglePan(!0))
+                }, this.map = (t, e, n, i, r) => i + (t - e) / (n - e) * (r - i), this.chartRef = f.createRef(), this.fixedData = function(t, e) {
+                    const n = e && e.fixed_lines ? e.fixed_lines : [];
+                    return {
+                        datasets: Object.entries(t).filter((t => {
+                            let [e] = t;
+                            return n.includes(e)
+                        })).map(((t, e) => {
+                            let [n, i] = t;
+                            const r = i.x.map(((t, e) => ({
+                                    x: t,
+                                    y: i.y[e]
+                                }))),
+                                s = Vg(i.color);
+                            return {
+                                data: r,
+                                isControlPoint: !1,
+                                label: n,
+                                fill: !1,
+                                tension: .3,
+                                spanGaps: !1,
+                                showLine: !0,
+                                backgroundColor: "rgba(".concat(s[0], ", ").concat(s[1], ", ").concat(s[2], ", 0.5)"),
+                                borderColor: i.color
+                            }
+                        }))
+                    }
+                }(this.props.args.data, this.props.args.options), this.state = {
+                    activePoint: null,
+                    originalData: t.args.data,
+                    controlData: jg(this.props.args.data, this.props.args.options),
+                    bezierData: Wg(this.props.args.data, this.props.args.options),
+                    options: Hg(t.args.options, t.theme)
+                }
+            }
+            componentDidUpdate(t) {
+                ro.setFrameHeight(), this.props.args !== t.args && this.setState({
+                    originalData: this.props.args.data,
+                    controlData: jg(this.props.args.data, this.props.args.options),
+                    bezierData: Wg(this.props.args.data, this.props.args.options),
+                    options: Hg(this.props.args.options, this.props.theme)
+                })
+            }
+            sendBezierData() {
+                const t = this.convertBezierData(this.state.bezierData.datasets);
+                ro.setComponentValue(t)
+            }
+            togglePan(t) {
+                this.chartRef.current.options.plugins.zoom.pan.enabled = t, this.chartRef.current.update("none")
+            }
+            convertBezierData(t) {
+                const e = {};
+                return t.forEach((t => {
+                    const n = t.label.replace(" (bezier)", "");
+                    e[n] = {
+                        x: [],
+                        y: []
+                    }, t.data.forEach((t => {
+                        const {
+                            x: i,
+                            y: r
+                        } = t; - 1 === e[n].x.findIndex(((t, s) => t === i && e[n].y[s] === r)) && (e[n].x.push(i), e[n].y.push(r))
+                    }))
+                })), e
+            }
+            render() {
+                return (0, ig.jsx)(Gp, {
+                    ref: this.chartRef,
+                    data: {
+                        datasets: [...this.fixedData.datasets, ...this.state.controlData.datasets, ...this.state.bezierData.datasets]
+                    },
+                    options: this.state.options,
+                    onPointerDown: this.downHandler,
+                    onPointerUp: this.upHandler,
+                    onPointerMove: this.moveHandler
+                })
+            }
+        };
+
+        function Kg(t, e) {
+            const n = !(!e || !e.fill_gaps) && e.fill_gaps,
+                i = e && e.fixed_lines ? e.fixed_lines : [],
+                r = Object.entries(t).filter((t => {
+                    let [e] = t;
+                    return !i.includes(e)
+                })).map(((t, e) => {
+                    let [i, r] = t;
+                    const s = r.x.map(((t, e) => ({
+                            x: t,
+                            y: r.y[e]
+                        }))),
+                        o = Vg(r.color),
+                        a = "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 1)"),
+                        l = "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.8)");
+                    return {
+                        data: s,
+                        isControlPoint: !0,
+                        label: i,
+                        spanGaps: n,
+                        showLine: !0,
+                        borderDash: [8, 5],
+                        borderWidth: 1.2,
+                        segment: {
+                            borderColor: t => ((t, e, n) => {
+                                const i = t.p1DataIndex;
+                                return i % 3 === 0 && i < n - 1 || i % 3 === 1 || i == n - 1 ? e : void 0
+                            })(t, a, s.length)
+                        },
+                        backgroundColor: l
+                    }
+                }));
+            return {
+                datasets: r
+            }
+        }
+
+        function Qg(t, e) {
+            const n = e && e.fixed_lines ? e.fixed_lines : [];
+            return {
+                datasets: Object.entries(t).filter((t => {
+                    let [e] = t;
+                    return !n.includes(e)
+                })).map(((t, e) => {
+                    let [n, i] = t;
+                    const r = i.x.map(((t, e) => ({
+                            x: t,
+                            y: i.y[e]
+                        }))),
+                        s = [];
+                    for (let a = 0; a < r.length - 3; a += 3) {
+                        const t = r.slice(a, a + 4),
+                            e = new zg(t).getLUT(10);
+                        s.push(...e)
+                    }
+                    const o = Vg(i.color);
+                    return {
+                        label: n + " (bezier)",
+                        data: s,
+                        isControlPoint: !1,
+                        showLine: !0,
+                        tension: .3,
+                        pointRadius: 0,
+                        backgroundColor: "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.7)"),
+                        borderColor: "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.4)")
+                    }
+                }))
+            }
+        }
+
+        function Gg(t, e) {
+            return {
+                responsive: !0,
+                indexAxis: "x",
+                animation: {
+                    duration: 0
+                },
+                onHover: (t, e) => {
+                    e.length > 0 ? t.native.target.style.cursor = "crosshair" : t.native.target.style.cursor = "default"
+                },
+                plugins: {
+                    tooltip: {
+                        filter: function(t) {
+                            return !t.dataset.label.includes("bezier")
+                        }
+                    },
+                    zoom: {
+                        zoom: {
+                            wheel: {
+                                enabled: !0
+                            },
+                            mode: "y"
+                        },
+                        pan: {
+                            enabled: !0
+                        },
+                        limits: {
+                            x: {
+                                min: "original",
+                                max: "original"
+                            },
+                            y: {
+                                min: "original",
+                                max: "original"
+                            }
+                        }
+                    },
+                    title: Zg(t),
+                    legend: Jg(t)
+                },
+                scales: tm(t, e)
+            }
+        }
+
+        function Zg(t) {
+            return {
+                display: !0,
+                text: t.title
+            }
+        }
+
+        function Jg(t) {
+            return {
+                display: t.legend,
+                position: t.legend_position,
+                align: t.legend_align,
+                labels: {
+                    boxWidth: 16,
+                    boxHeight: 8,
+                    padding: 8
+                },
+                onHover: (t, e, n) => {
+                    t.native.target.style.cursor = e ? "pointer" : "default"
+                }
+            }
+        }
+
+        function tm(t, e) {
+            const n = {
+                display: !0,
+                type: t.x_type,
+                title: {
+                    display: !0,
+                    text: t.x_label
+                },
+                grid: {
+                    display: t.x_grid,
+                    color: e.fadedText05
+                }
+            };
+            t.x_labels && (n.min = t.x_labels[0], n.max = t.x_labels[t.x_labels.length - 1]);
+            const i = {
+                display: !0,
+                type: t.y_type,
+                title: {
+                    display: !0,
+                    text: t.y_label
+                },
+                grid: {
+                    display: t.y_grid,
+                    color: e.fadedText05
+                }
+            };
+            return t.y_labels && (i.labels = t.y_labels, i.min = t.y_labels[0], i.max = t.y_labels[t.y_labels.length - 1]), {
+                x: n,
+                y: i
+            }
+        }
+        Hh.register(...$f, Up);
+        const em = {
                 line_chart: rg,
                 scatter_chart: ug,
-                bezier_chart: class extends ao {
+                bezier_chart: qg,
+                cubic_bezier_chart: class extends ao {
                     constructor(t) {
                         super(t), this.downHandler = t => {
                             const e = $p(this.chartRef.current, t);
                             if (e.length > 0) {
                                 this.chartRef.current.data.datasets[e[0].datasetIndex].isControlPoint && (this.setState({
                                     activePoint: e[0]
                                 }), this.togglePan(!1))
                             }
-                        }, this.calculateNewYValue = (t, e, n) => this.map(t.y, e.bottom, e.top, n.min, n.max), this.calculateNewXValue = (t, e, n) => this.map(t.x, e.left, e.right, n.min, n.max), this.updateControlPointPosition = (t, e, n, i) => {
-                            const r = e.datasetIndex,
-                                s = e.index;
-                            t.data.datasets[r].data[s].x = n, t.data.datasets[r].data[s].y = i
-                        }, this.updateOriginalData = (t, e) => {
-                            const n = e.datasetIndex,
-                                i = e.index,
-                                r = t.data.datasets[n].label,
-                                s = t.data.datasets[n].data[i].x,
-                                o = t.data.datasets[n].data[i].y;
-                            this.state.originalData[r].x[i] = s, this.state.originalData[r].y[i] = o
-                        }, this.moveHandler = t => {
+                        }, this.calculateNewYValue = (t, e, n) => this.map(t.y, e.bottom, e.top, n.min, n.max), this.calculateNewXValue = (t, e, n) => this.map(t.x, e.left, e.right, n.min, n.max), this.moveHandler = t => {
                             if (this.state.activePoint) {
                                 const e = this.chartRef.current,
                                     n = this.state.activePoint,
                                     i = yc(t, e),
                                     r = e.chartArea,
                                     s = this.calculateNewYValue(i, r, e.scales.y),
-                                    o = this.calculateNewXValue(i, r, e.scales.x);
-                                this.updateControlPointPosition(e, n, o, s), this.updateOriginalData(e, n);
-                                const a = Wg(this.state.originalData, this.props.args.options);
+                                    o = this.calculateNewXValue(i, r, e.scales.x),
+                                    a = n.datasetIndex,
+                                    l = n.index,
+                                    c = s - e.data.datasets[a].data[l].y,
+                                    u = o - e.data.datasets[a].data[l].x;
+                                e.data.datasets[a].data[l].x = o, e.data.datasets[a].data[l].y = s;
+                                const h = e.data.datasets[a].label,
+                                    d = e.data.datasets[a].data[l].x,
+                                    f = e.data.datasets[a].data[l].y;
+                                this.state.originalData[h].x[l] = d, this.state.originalData[h].y[l] = f;
+                                const p = e.data.datasets[a].data.length;
+                                0 === l ? (e.data.datasets[a].data[l + 1].x += u, e.data.datasets[a].data[l + 1].y += c, this.state.originalData[h].x[l + 1] += u, this.state.originalData[h].y[l + 1] += c) : l === p - 1 ? (e.data.datasets[a].data[l - 1].x += u, e.data.datasets[a].data[l - 1].y += c, this.state.originalData[h].x[l - 1] += u, this.state.originalData[h].y[l - 1] += c) : l % 3 === 0 && 0 != l && l != p - 1 ? (e.data.datasets[a].data[l - 1].x += u, e.data.datasets[a].data[l - 1].y += c, e.data.datasets[a].data[l + 1].x += u, e.data.datasets[a].data[l + 1].y += c, this.state.originalData[h].x[l - 1] += u, this.state.originalData[h].y[l - 1] += c, this.state.originalData[h].x[l + 1] += u, this.state.originalData[h].y[l + 1] += c) : (l + 1) % 3 === 0 && l + 1 != p - 1 ? (e.data.datasets[a].data[l + 2].x -= u, e.data.datasets[a].data[l + 2].y -= c, this.state.originalData[h].x[l + 2] -= u, this.state.originalData[h].y[l + 2] -= c) : (l - 1) % 3 === 0 && l - 1 != 0 && (e.data.datasets[a].data[l - 2].x -= u, e.data.datasets[a].data[l - 2].y -= c, this.state.originalData[h].x[l - 2] -= u, this.state.originalData[h].y[l - 2] -= c);
+                                const g = Qg(this.state.originalData, this.props.args.options);
                                 this.setState({
-                                    bezierData: a
+                                    bezierData: g
                                 }), e.update("none")
                             }
                         }, this.upHandler = t => {
                             this.state.activePoint && (this.sendBezierData(), this.setState({
                                 activePoint: null
                             }), this.togglePan(!0))
                         }, this.map = (t, e, n, i, r) => i + (t - e) / (n - e) * (r - i), this.chartRef = f.createRef(), this.fixedData = function(t, e) {
-                            console.log(t);
                             const n = e && e.fixed_lines ? e.fixed_lines : [];
                             return {
                                 datasets: Object.entries(t).filter((t => {
                                     let [e] = t;
                                     return n.includes(e)
                                 })).map(((t, e) => {
                                     let [n, i] = t;
@@ -27941,25 +28225,25 @@
                                         borderColor: i.color
                                     }
                                 }))
                             }
                         }(this.props.args.data, this.props.args.options), this.state = {
                             activePoint: null,
                             originalData: t.args.data,
-                            controlData: jg(this.props.args.data, this.props.args.options),
-                            bezierData: Wg(this.props.args.data, this.props.args.options),
-                            options: Hg(t.args.options, t.theme)
+                            controlData: Kg(this.props.args.data, this.props.args.options),
+                            bezierData: Qg(this.props.args.data, this.props.args.options),
+                            options: Gg(t.args.options, t.theme)
                         }
                     }
                     componentDidUpdate(t) {
                         ro.setFrameHeight(), this.props.args !== t.args && this.setState({
                             originalData: this.props.args.data,
-                            controlData: jg(this.props.args.data, this.props.args.options),
-                            bezierData: Wg(this.props.args.data, this.props.args.options),
-                            options: Hg(this.props.args.options, this.props.theme)
+                            controlData: Kg(this.props.args.data, this.props.args.options),
+                            bezierData: Qg(this.props.args.data, this.props.args.options),
+                            options: Gg(this.props.args.options, this.props.theme)
                         })
                     }
                     sendBezierData() {
                         const t = this.convertBezierData(this.state.bezierData.datasets);
                         ro.setComponentValue(t)
                     }
                     togglePan(t) {
@@ -27990,15 +28274,15 @@
                             onPointerDown: this.downHandler,
                             onPointerUp: this.upHandler,
                             onPointerMove: this.moveHandler
                         })
                     }
                 }
             },
-            Kg = function(t) {
+            nm = function(t) {
                 var e = function(e) {
                     function n(t) {
                         var n = e.call(this, t) || this;
                         return n.componentDidMount = function() {
                             ro.events.addEventListener(ro.RENDER_EVENT, n.onRenderEvent), ro.setComponentReady()
                         }, n.componentDidUpdate = function() {
                             null != n.state.componentError && ro.setFrameHeight()
@@ -28026,22 +28310,22 @@
                         }
                     }, n
                 }(f.PureComponent);
                 return d()(e, t)
             }((t => {
                 const e = t.args.id,
                     n = t.args.kw,
-                    i = qg[e];
+                    i = em[e];
                 if (void 0 === i) throw new Error("Component with id ".concat(e, " is not defined in componentsMap."));
                 return (0, ig.jsx)(i, {
                     args: {
                         ...n
                     },
                     theme: t.theme
                 })
             }));
         lo.render((0, ig.jsx)(f.StrictMode, {
-            children: (0, ig.jsx)(Kg, {})
+            children: (0, ig.jsx)(nm, {})
         }), document.getElementById("root"))
     })()
 })();
-//# sourceMappingURL=main.ac399b09.js.map
+//# sourceMappingURL=main.96151505.js.map
```

### Comparing `draggable-charts-1.1.1/draggable_charts/frontend/build/static/js/main.ac399b09.js.LICENSE.txt` & `draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.1/draggable_charts/frontend/build/static/js/main.ac399b09.js.map` & `draggable-charts-1.1.2/draggable_charts/frontend/build/static/js/main.96151505.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8536481340009269%*

 * *Differences: {"'file'": "'static/js/main.96151505.js'",*

 * * "'mappings'": "';2BAAA,OAKA,SAAUA,EAAQC,EAAUC,EAAYC,GACtC,aAEF,IA+FIC,EA/FAC,EAAkB,CAAC,GAAI,SAAU,MAAO,KAAM,KAAM,KACpDC,EAAeL,EAASM,cAAc,OAEtCC,EAAgB,WAEhBC,EAAQC,KAAKD,MACbE,EAAMD,KAAKC,IACXC,EAAMC,KAAKD,IASf,SAASE,EAAkBC,EAAIC,EAASC,GACpC,OAAOC,WAAWC,EAAOJ,EAAIE,GAAUD,EAC3C,CAWA,SAASI,EAAeC,EAAKN,EAAIE,GAC7B,QAAIK,MAAMC,QAAQF,KACdG,EAAKH,EAAKJ,EAAQF,GAAKE,IAChB,EAGf,CAQA,SAASO,EAAKC,EAAKC,EAAUT,GACzB,IAAIU,EAEJ,GAAKF,EAIL,GAAIA,EAAIG,QACJH,EAAIG,QAAQF,EAAUT,QACn […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.ac399b09.js",
+    "file": "static/js/main.96151505.js",
     "names": [
         "window",
         "document",
         "exportName",
         "undefined",
         "assign",
         "VENDOR_PREFIXES",
@@ -6095,28 +6095,32 @@
         "isControlPoint",
         "createBezierData",
         "trace",
         "traceData",
         "bezierSegments",
         "bezierPoints",
         "pointRadius",
-        "line_chart",
-        "LineChart",
-        "scatter_chart",
-        "ScatterChart",
-        "bezier_chart",
         "updateControlPointPosition",
         "updateOriginalData",
         "bezierData",
         "sendBezierData",
         "fixedData",
         "createFixedData",
         "controlData",
         "newBezierData",
         "convertBezierData",
+        "lineControl",
+        "line_chart",
+        "LineChart",
+        "scatter_chart",
+        "ScatterChart",
+        "bezier_chart",
+        "BezierChart",
+        "cubic_bezier_chart",
+        "dataLen",
         "StreamlitComponent",
         "WrappedComponent",
         "ComponentWrapper",
         "onRenderEvent",
         "componentError",
         "renderData",
         "innerWidth",
@@ -6331,14 +6335,17 @@
         "../node_modules/color-parse/index.js",
         "../node_modules/color-space/rgb.js",
         "../node_modules/color-space/hsl.js",
         "../node_modules/color-rgba/index.js",
         "BezierChart/chartData.jsx",
         "BezierChart/chartOptions.jsx",
         "BezierChart/BezierChart.jsx",
+        "CubicBezierChart/chartData.jsx",
+        "CubicBezierChart/chartOptions.jsx",
+        "CubicBezierChart/CubicBezierChart.jsx",
         "components.jsx",
         "index.jsx"
     ],
     "sourcesContent": [
         "/*! Hammer.JS - v2.0.7 - 2016-04-22\n * http://hammerjs.github.io/\n *\n * Copyright (c) 2016 Jorik Tangelder;\n * Licensed under the MIT license */\n(function(window, document, exportName, undefined) {\n  'use strict';\n\nvar VENDOR_PREFIXES = ['', 'webkit', 'Moz', 'MS', 'ms', 'o'];\nvar TEST_ELEMENT = document.createElement('div');\n\nvar TYPE_FUNCTION = 'function';\n\nvar round = Math.round;\nvar abs = Math.abs;\nvar now = Date.now;\n\n/**\n * set a timeout with a given scope\n * @param {Function} fn\n * @param {Number} timeout\n * @param {Object} context\n * @returns {number}\n */\nfunction setTimeoutContext(fn, timeout, context) {\n    return setTimeout(bindFn(fn, context), timeout);\n}\n\n/**\n * if the argument is an array, we want to execute the fn on each entry\n * if it aint an array we don't want to do a thing.\n * this is used by all the methods that accept a single and array argument.\n * @param {*|Array} arg\n * @param {String} fn\n * @param {Object} [context]\n * @returns {Boolean}\n */\nfunction invokeArrayArg(arg, fn, context) {\n    if (Array.isArray(arg)) {\n        each(arg, context[fn], context);\n        return true;\n    }\n    return false;\n}\n\n/**\n * walk objects and arrays\n * @param {Object} obj\n * @param {Function} iterator\n * @param {Object} context\n */\nfunction each(obj, iterator, context) {\n    var i;\n\n    if (!obj) {\n        return;\n    }\n\n    if (obj.forEach) {\n        obj.forEach(iterator, context);\n    } else if (obj.length !== undefined) {\n        i = 0;\n        while (i < obj.length) {\n            iterator.call(context, obj[i], i, obj);\n            i++;\n        }\n    } else {\n        for (i in obj) {\n            obj.hasOwnProperty(i) && iterator.call(context, obj[i], i, obj);\n        }\n    }\n}\n\n/**\n * wrap a method with a deprecation warning and stack trace\n * @param {Function} method\n * @param {String} name\n * @param {String} message\n * @returns {Function} A new function wrapping the supplied method.\n */\nfunction deprecate(method, name, message) {\n    var deprecationMessage = 'DEPRECATED METHOD: ' + name + '\\n' + message + ' AT \\n';\n    return function() {\n        var e = new Error('get-stack-trace');\n        var stack = e && e.stack ? e.stack.replace(/^[^\\(]+?[\\n$]/gm, '')\n            .replace(/^\\s+at\\s+/gm, '')\n            .replace(/^Object.<anonymous>\\s*\\(/gm, '{anonymous}()@') : 'Unknown Stack Trace';\n\n        var log = window.console && (window.console.warn || window.console.log);\n        if (log) {\n            log.call(window.console, deprecationMessage, stack);\n        }\n        return method.apply(this, arguments);\n    };\n}\n\n/**\n * extend object.\n * means that properties in dest will be overwritten by the ones in src.\n * @param {Object} target\n * @param {...Object} objects_to_assign\n * @returns {Object} target\n */\nvar assign;\nif (typeof Object.assign !== 'function') {\n    assign = function assign(target) {\n        if (target === undefined || target === null) {\n            throw new TypeError('Cannot convert undefined or null to object');\n        }\n\n        var output = Object(target);\n        for (var index = 1; index < arguments.length; index++) {\n            var source = arguments[index];\n            if (source !== undefined && source !== null) {\n                for (var nextKey in source) {\n                    if (source.hasOwnProperty(nextKey)) {\n                        output[nextKey] = source[nextKey];\n                    }\n                }\n            }\n        }\n        return output;\n    };\n} else {\n    assign = Object.assign;\n}\n\n/**\n * extend object.\n * means that properties in dest will be overwritten by the ones in src.\n * @param {Object} dest\n * @param {Object} src\n * @param {Boolean} [merge=false]\n * @returns {Object} dest\n */\nvar extend = deprecate(function extend(dest, src, merge) {\n    var keys = Object.keys(src);\n    var i = 0;\n    while (i < keys.length) {\n        if (!merge || (merge && dest[keys[i]] === undefined)) {\n            dest[keys[i]] = src[keys[i]];\n        }\n        i++;\n    }\n    return dest;\n}, 'extend', 'Use `assign`.');\n\n/**\n * merge the values from src in the dest.\n * means that properties that exist in dest will not be overwritten by src\n * @param {Object} dest\n * @param {Object} src\n * @returns {Object} dest\n */\nvar merge = deprecate(function merge(dest, src) {\n    return extend(dest, src, true);\n}, 'merge', 'Use `assign`.');\n\n/**\n * simple class inheritance\n * @param {Function} child\n * @param {Function} base\n * @param {Object} [properties]\n */\nfunction inherit(child, base, properties) {\n    var baseP = base.prototype,\n        childP;\n\n    childP = child.prototype = Object.create(baseP);\n    childP.constructor = child;\n    childP._super = baseP;\n\n    if (properties) {\n        assign(childP, properties);\n    }\n}\n\n/**\n * simple function bind\n * @param {Function} fn\n * @param {Object} context\n * @returns {Function}\n */\nfunction bindFn(fn, context) {\n    return function boundFn() {\n        return fn.apply(context, arguments);\n    };\n}\n\n/**\n * let a boolean value also be a function that must return a boolean\n * this first item in args will be used as the context\n * @param {Boolean|Function} val\n * @param {Array} [args]\n * @returns {Boolean}\n */\nfunction boolOrFn(val, args) {\n    if (typeof val == TYPE_FUNCTION) {\n        return val.apply(args ? args[0] || undefined : undefined, args);\n    }\n    return val;\n}\n\n/**\n * use the val2 when val1 is undefined\n * @param {*} val1\n * @param {*} val2\n * @returns {*}\n */\nfunction ifUndefined(val1, val2) {\n    return (val1 === undefined) ? val2 : val1;\n}\n\n/**\n * addEventListener with multiple events at once\n * @param {EventTarget} target\n * @param {String} types\n * @param {Function} handler\n */\nfunction addEventListeners(target, types, handler) {\n    each(splitStr(types), function(type) {\n        target.addEventListener(type, handler, false);\n    });\n}\n\n/**\n * removeEventListener with multiple events at once\n * @param {EventTarget} target\n * @param {String} types\n * @param {Function} handler\n */\nfunction removeEventListeners(target, types, handler) {\n    each(splitStr(types), function(type) {\n        target.removeEventListener(type, handler, false);\n    });\n}\n\n/**\n * find if a node is in the given parent\n * @method hasParent\n * @param {HTMLElement} node\n * @param {HTMLElement} parent\n * @return {Boolean} found\n */\nfunction hasParent(node, parent) {\n    while (node) {\n        if (node == parent) {\n            return true;\n        }\n        node = node.parentNode;\n    }\n    return false;\n}\n\n/**\n * small indexOf wrapper\n * @param {String} str\n * @param {String} find\n * @returns {Boolean} found\n */\nfunction inStr(str, find) {\n    return str.indexOf(find) > -1;\n}\n\n/**\n * split string on whitespace\n * @param {String} str\n * @returns {Array} words\n */\nfunction splitStr(str) {\n    return str.trim().split(/\\s+/g);\n}\n\n/**\n * find if a array contains the object using indexOf or a simple polyFill\n * @param {Array} src\n * @param {String} find\n * @param {String} [findByKey]\n * @return {Boolean|Number} false when not found, or the index\n */\nfunction inArray(src, find, findByKey) {\n    if (src.indexOf && !findByKey) {\n        return src.indexOf(find);\n    } else {\n        var i = 0;\n        while (i < src.length) {\n            if ((findByKey && src[i][findByKey] == find) || (!findByKey && src[i] === find)) {\n                return i;\n            }\n            i++;\n        }\n        return -1;\n    }\n}\n\n/**\n * convert array-like objects to real arrays\n * @param {Object} obj\n * @returns {Array}\n */\nfunction toArray(obj) {\n    return Array.prototype.slice.call(obj, 0);\n}\n\n/**\n * unique array with objects based on a key (like 'id') or just by the array's value\n * @param {Array} src [{id:1},{id:2},{id:1}]\n * @param {String} [key]\n * @param {Boolean} [sort=False]\n * @returns {Array} [{id:1},{id:2}]\n */\nfunction uniqueArray(src, key, sort) {\n    var results = [];\n    var values = [];\n    var i = 0;\n\n    while (i < src.length) {\n        var val = key ? src[i][key] : src[i];\n        if (inArray(values, val) < 0) {\n            results.push(src[i]);\n        }\n        values[i] = val;\n        i++;\n    }\n\n    if (sort) {\n        if (!key) {\n            results = results.sort();\n        } else {\n            results = results.sort(function sortUniqueArray(a, b) {\n                return a[key] > b[key];\n            });\n        }\n    }\n\n    return results;\n}\n\n/**\n * get the prefixed property\n * @param {Object} obj\n * @param {String} property\n * @returns {String|Undefined} prefixed\n */\nfunction prefixed(obj, property) {\n    var prefix, prop;\n    var camelProp = property[0].toUpperCase() + property.slice(1);\n\n    var i = 0;\n    while (i < VENDOR_PREFIXES.length) {\n        prefix = VENDOR_PREFIXES[i];\n        prop = (prefix) ? prefix + camelProp : property;\n\n        if (prop in obj) {\n            return prop;\n        }\n        i++;\n    }\n    return undefined;\n}\n\n/**\n * get a unique id\n * @returns {number} uniqueId\n */\nvar _uniqueId = 1;\nfunction uniqueId() {\n    return _uniqueId++;\n}\n\n/**\n * get the window object of an element\n * @param {HTMLElement} element\n * @returns {DocumentView|Window}\n */\nfunction getWindowForElement(element) {\n    var doc = element.ownerDocument || element;\n    return (doc.defaultView || doc.parentWindow || window);\n}\n\nvar MOBILE_REGEX = /mobile|tablet|ip(ad|hone|od)|android/i;\n\nvar SUPPORT_TOUCH = ('ontouchstart' in window);\nvar SUPPORT_POINTER_EVENTS = prefixed(window, 'PointerEvent') !== undefined;\nvar SUPPORT_ONLY_TOUCH = SUPPORT_TOUCH && MOBILE_REGEX.test(navigator.userAgent);\n\nvar INPUT_TYPE_TOUCH = 'touch';\nvar INPUT_TYPE_PEN = 'pen';\nvar INPUT_TYPE_MOUSE = 'mouse';\nvar INPUT_TYPE_KINECT = 'kinect';\n\nvar COMPUTE_INTERVAL = 25;\n\nvar INPUT_START = 1;\nvar INPUT_MOVE = 2;\nvar INPUT_END = 4;\nvar INPUT_CANCEL = 8;\n\nvar DIRECTION_NONE = 1;\nvar DIRECTION_LEFT = 2;\nvar DIRECTION_RIGHT = 4;\nvar DIRECTION_UP = 8;\nvar DIRECTION_DOWN = 16;\n\nvar DIRECTION_HORIZONTAL = DIRECTION_LEFT | DIRECTION_RIGHT;\nvar DIRECTION_VERTICAL = DIRECTION_UP | DIRECTION_DOWN;\nvar DIRECTION_ALL = DIRECTION_HORIZONTAL | DIRECTION_VERTICAL;\n\nvar PROPS_XY = ['x', 'y'];\nvar PROPS_CLIENT_XY = ['clientX', 'clientY'];\n\n/**\n * create new input type manager\n * @param {Manager} manager\n * @param {Function} callback\n * @returns {Input}\n * @constructor\n */\nfunction Input(manager, callback) {\n    var self = this;\n    this.manager = manager;\n    this.callback = callback;\n    this.element = manager.element;\n    this.target = manager.options.inputTarget;\n\n    // smaller wrapper around the handler, for the scope and the enabled state of the manager,\n    // so when disabled the input events are completely bypassed.\n    this.domHandler = function(ev) {\n        if (boolOrFn(manager.options.enable, [manager])) {\n            self.handler(ev);\n        }\n    };\n\n    this.init();\n\n}\n\nInput.prototype = {\n    /**\n     * should handle the inputEvent data and trigger the callback\n     * @virtual\n     */\n    handler: function() { },\n\n    /**\n     * bind the events\n     */\n    init: function() {\n        this.evEl && addEventListeners(this.element, this.evEl, this.domHandler);\n        this.evTarget && addEventListeners(this.target, this.evTarget, this.domHandler);\n        this.evWin && addEventListeners(getWindowForElement(this.element), this.evWin, this.domHandler);\n    },\n\n    /**\n     * unbind the events\n     */\n    destroy: function() {\n        this.evEl && removeEventListeners(this.element, this.evEl, this.domHandler);\n        this.evTarget && removeEventListeners(this.target, this.evTarget, this.domHandler);\n        this.evWin && removeEventListeners(getWindowForElement(this.element), this.evWin, this.domHandler);\n    }\n};\n\n/**\n * create new input type manager\n * called by the Manager constructor\n * @param {Hammer} manager\n * @returns {Input}\n */\nfunction createInputInstance(manager) {\n    var Type;\n    var inputClass = manager.options.inputClass;\n\n    if (inputClass) {\n        Type = inputClass;\n    } else if (SUPPORT_POINTER_EVENTS) {\n        Type = PointerEventInput;\n    } else if (SUPPORT_ONLY_TOUCH) {\n        Type = TouchInput;\n    } else if (!SUPPORT_TOUCH) {\n        Type = MouseInput;\n    } else {\n        Type = TouchMouseInput;\n    }\n    return new (Type)(manager, inputHandler);\n}\n\n/**\n * handle input events\n * @param {Manager} manager\n * @param {String} eventType\n * @param {Object} input\n */\nfunction inputHandler(manager, eventType, input) {\n    var pointersLen = input.pointers.length;\n    var changedPointersLen = input.changedPointers.length;\n    var isFirst = (eventType & INPUT_START && (pointersLen - changedPointersLen === 0));\n    var isFinal = (eventType & (INPUT_END | INPUT_CANCEL) && (pointersLen - changedPointersLen === 0));\n\n    input.isFirst = !!isFirst;\n    input.isFinal = !!isFinal;\n\n    if (isFirst) {\n        manager.session = {};\n    }\n\n    // source event is the normalized value of the domEvents\n    // like 'touchstart, mouseup, pointerdown'\n    input.eventType = eventType;\n\n    // compute scale, rotation etc\n    computeInputData(manager, input);\n\n    // emit secret event\n    manager.emit('hammer.input', input);\n\n    manager.recognize(input);\n    manager.session.prevInput = input;\n}\n\n/**\n * extend the data with some usable properties like scale, rotate, velocity etc\n * @param {Object} manager\n * @param {Object} input\n */\nfunction computeInputData(manager, input) {\n    var session = manager.session;\n    var pointers = input.pointers;\n    var pointersLength = pointers.length;\n\n    // store the first input to calculate the distance and direction\n    if (!session.firstInput) {\n        session.firstInput = simpleCloneInputData(input);\n    }\n\n    // to compute scale and rotation we need to store the multiple touches\n    if (pointersLength > 1 && !session.firstMultiple) {\n        session.firstMultiple = simpleCloneInputData(input);\n    } else if (pointersLength === 1) {\n        session.firstMultiple = false;\n    }\n\n    var firstInput = session.firstInput;\n    var firstMultiple = session.firstMultiple;\n    var offsetCenter = firstMultiple ? firstMultiple.center : firstInput.center;\n\n    var center = input.center = getCenter(pointers);\n    input.timeStamp = now();\n    input.deltaTime = input.timeStamp - firstInput.timeStamp;\n\n    input.angle = getAngle(offsetCenter, center);\n    input.distance = getDistance(offsetCenter, center);\n\n    computeDeltaXY(session, input);\n    input.offsetDirection = getDirection(input.deltaX, input.deltaY);\n\n    var overallVelocity = getVelocity(input.deltaTime, input.deltaX, input.deltaY);\n    input.overallVelocityX = overallVelocity.x;\n    input.overallVelocityY = overallVelocity.y;\n    input.overallVelocity = (abs(overallVelocity.x) > abs(overallVelocity.y)) ? overallVelocity.x : overallVelocity.y;\n\n    input.scale = firstMultiple ? getScale(firstMultiple.pointers, pointers) : 1;\n    input.rotation = firstMultiple ? getRotation(firstMultiple.pointers, pointers) : 0;\n\n    input.maxPointers = !session.prevInput ? input.pointers.length : ((input.pointers.length >\n        session.prevInput.maxPointers) ? input.pointers.length : session.prevInput.maxPointers);\n\n    computeIntervalInputData(session, input);\n\n    // find the correct target\n    var target = manager.element;\n    if (hasParent(input.srcEvent.target, target)) {\n        target = input.srcEvent.target;\n    }\n    input.target = target;\n}\n\nfunction computeDeltaXY(session, input) {\n    var center = input.center;\n    var offset = session.offsetDelta || {};\n    var prevDelta = session.prevDelta || {};\n    var prevInput = session.prevInput || {};\n\n    if (input.eventType === INPUT_START || prevInput.eventType === INPUT_END) {\n        prevDelta = session.prevDelta = {\n            x: prevInput.deltaX || 0,\n            y: prevInput.deltaY || 0\n        };\n\n        offset = session.offsetDelta = {\n            x: center.x,\n            y: center.y\n        };\n    }\n\n    input.deltaX = prevDelta.x + (center.x - offset.x);\n    input.deltaY = prevDelta.y + (center.y - offset.y);\n}\n\n/**\n * velocity is calculated every x ms\n * @param {Object} session\n * @param {Object} input\n */\nfunction computeIntervalInputData(session, input) {\n    var last = session.lastInterval || input,\n        deltaTime = input.timeStamp - last.timeStamp,\n        velocity, velocityX, velocityY, direction;\n\n    if (input.eventType != INPUT_CANCEL && (deltaTime > COMPUTE_INTERVAL || last.velocity === undefined)) {\n        var deltaX = input.deltaX - last.deltaX;\n        var deltaY = input.deltaY - last.deltaY;\n\n        var v = getVelocity(deltaTime, deltaX, deltaY);\n        velocityX = v.x;\n        velocityY = v.y;\n        velocity = (abs(v.x) > abs(v.y)) ? v.x : v.y;\n        direction = getDirection(deltaX, deltaY);\n\n        session.lastInterval = input;\n    } else {\n        // use latest velocity info if it doesn't overtake a minimum period\n        velocity = last.velocity;\n        velocityX = last.velocityX;\n        velocityY = last.velocityY;\n        direction = last.direction;\n    }\n\n    input.velocity = velocity;\n    input.velocityX = velocityX;\n    input.velocityY = velocityY;\n    input.direction = direction;\n}\n\n/**\n * create a simple clone from the input used for storage of firstInput and firstMultiple\n * @param {Object} input\n * @returns {Object} clonedInputData\n */\nfunction simpleCloneInputData(input) {\n    // make a simple copy of the pointers because we will get a reference if we don't\n    // we only need clientXY for the calculations\n    var pointers = [];\n    var i = 0;\n    while (i < input.pointers.length) {\n        pointers[i] = {\n            clientX: round(input.pointers[i].clientX),\n            clientY: round(input.pointers[i].clientY)\n        };\n        i++;\n    }\n\n    return {\n        timeStamp: now(),\n        pointers: pointers,\n        center: getCenter(pointers),\n        deltaX: input.deltaX,\n        deltaY: input.deltaY\n    };\n}\n\n/**\n * get the center of all the pointers\n * @param {Array} pointers\n * @return {Object} center contains `x` and `y` properties\n */\nfunction getCenter(pointers) {\n    var pointersLength = pointers.length;\n\n    // no need to loop when only one touch\n    if (pointersLength === 1) {\n        return {\n            x: round(pointers[0].clientX),\n            y: round(pointers[0].clientY)\n        };\n    }\n\n    var x = 0, y = 0, i = 0;\n    while (i < pointersLength) {\n        x += pointers[i].clientX;\n        y += pointers[i].clientY;\n        i++;\n    }\n\n    return {\n        x: round(x / pointersLength),\n        y: round(y / pointersLength)\n    };\n}\n\n/**\n * calculate the velocity between two points. unit is in px per ms.\n * @param {Number} deltaTime\n * @param {Number} x\n * @param {Number} y\n * @return {Object} velocity `x` and `y`\n */\nfunction getVelocity(deltaTime, x, y) {\n    return {\n        x: x / deltaTime || 0,\n        y: y / deltaTime || 0\n    };\n}\n\n/**\n * get the direction between two points\n * @param {Number} x\n * @param {Number} y\n * @return {Number} direction\n */\nfunction getDirection(x, y) {\n    if (x === y) {\n        return DIRECTION_NONE;\n    }\n\n    if (abs(x) >= abs(y)) {\n        return x < 0 ? DIRECTION_LEFT : DIRECTION_RIGHT;\n    }\n    return y < 0 ? DIRECTION_UP : DIRECTION_DOWN;\n}\n\n/**\n * calculate the absolute distance between two points\n * @param {Object} p1 {x, y}\n * @param {Object} p2 {x, y}\n * @param {Array} [props] containing x and y keys\n * @return {Number} distance\n */\nfunction getDistance(p1, p2, props) {\n    if (!props) {\n        props = PROPS_XY;\n    }\n    var x = p2[props[0]] - p1[props[0]],\n        y = p2[props[1]] - p1[props[1]];\n\n    return Math.sqrt((x * x) + (y * y));\n}\n\n/**\n * calculate the angle between two coordinates\n * @param {Object} p1\n * @param {Object} p2\n * @param {Array} [props] containing x and y keys\n * @return {Number} angle\n */\nfunction getAngle(p1, p2, props) {\n    if (!props) {\n        props = PROPS_XY;\n    }\n    var x = p2[props[0]] - p1[props[0]],\n        y = p2[props[1]] - p1[props[1]];\n    return Math.atan2(y, x) * 180 / Math.PI;\n}\n\n/**\n * calculate the rotation degrees between two pointersets\n * @param {Array} start array of pointers\n * @param {Array} end array of pointers\n * @return {Number} rotation\n */\nfunction getRotation(start, end) {\n    return getAngle(end[1], end[0], PROPS_CLIENT_XY) + getAngle(start[1], start[0], PROPS_CLIENT_XY);\n}\n\n/**\n * calculate the scale factor between two pointersets\n * no scale is 1, and goes down to 0 when pinched together, and bigger when pinched out\n * @param {Array} start array of pointers\n * @param {Array} end array of pointers\n * @return {Number} scale\n */\nfunction getScale(start, end) {\n    return getDistance(end[0], end[1], PROPS_CLIENT_XY) / getDistance(start[0], start[1], PROPS_CLIENT_XY);\n}\n\nvar MOUSE_INPUT_MAP = {\n    mousedown: INPUT_START,\n    mousemove: INPUT_MOVE,\n    mouseup: INPUT_END\n};\n\nvar MOUSE_ELEMENT_EVENTS = 'mousedown';\nvar MOUSE_WINDOW_EVENTS = 'mousemove mouseup';\n\n/**\n * Mouse events input\n * @constructor\n * @extends Input\n */\nfunction MouseInput() {\n    this.evEl = MOUSE_ELEMENT_EVENTS;\n    this.evWin = MOUSE_WINDOW_EVENTS;\n\n    this.pressed = false; // mousedown state\n\n    Input.apply(this, arguments);\n}\n\ninherit(MouseInput, Input, {\n    /**\n     * handle mouse events\n     * @param {Object} ev\n     */\n    handler: function MEhandler(ev) {\n        var eventType = MOUSE_INPUT_MAP[ev.type];\n\n        // on start we want to have the left mouse button down\n        if (eventType & INPUT_START && ev.button === 0) {\n            this.pressed = true;\n        }\n\n        if (eventType & INPUT_MOVE && ev.which !== 1) {\n            eventType = INPUT_END;\n        }\n\n        // mouse must be down\n        if (!this.pressed) {\n            return;\n        }\n\n        if (eventType & INPUT_END) {\n            this.pressed = false;\n        }\n\n        this.callback(this.manager, eventType, {\n            pointers: [ev],\n            changedPointers: [ev],\n            pointerType: INPUT_TYPE_MOUSE,\n            srcEvent: ev\n        });\n    }\n});\n\nvar POINTER_INPUT_MAP = {\n    pointerdown: INPUT_START,\n    pointermove: INPUT_MOVE,\n    pointerup: INPUT_END,\n    pointercancel: INPUT_CANCEL,\n    pointerout: INPUT_CANCEL\n};\n\n// in IE10 the pointer types is defined as an enum\nvar IE10_POINTER_TYPE_ENUM = {\n    2: INPUT_TYPE_TOUCH,\n    3: INPUT_TYPE_PEN,\n    4: INPUT_TYPE_MOUSE,\n    5: INPUT_TYPE_KINECT // see https://twitter.com/jacobrossi/status/480596438489890816\n};\n\nvar POINTER_ELEMENT_EVENTS = 'pointerdown';\nvar POINTER_WINDOW_EVENTS = 'pointermove pointerup pointercancel';\n\n// IE10 has prefixed support, and case-sensitive\nif (window.MSPointerEvent && !window.PointerEvent) {\n    POINTER_ELEMENT_EVENTS = 'MSPointerDown';\n    POINTER_WINDOW_EVENTS = 'MSPointerMove MSPointerUp MSPointerCancel';\n}\n\n/**\n * Pointer events input\n * @constructor\n * @extends Input\n */\nfunction PointerEventInput() {\n    this.evEl = POINTER_ELEMENT_EVENTS;\n    this.evWin = POINTER_WINDOW_EVENTS;\n\n    Input.apply(this, arguments);\n\n    this.store = (this.manager.session.pointerEvents = []);\n}\n\ninherit(PointerEventInput, Input, {\n    /**\n     * handle mouse events\n     * @param {Object} ev\n     */\n    handler: function PEhandler(ev) {\n        var store = this.store;\n        var removePointer = false;\n\n        var eventTypeNormalized = ev.type.toLowerCase().replace('ms', '');\n        var eventType = POINTER_INPUT_MAP[eventTypeNormalized];\n        var pointerType = IE10_POINTER_TYPE_ENUM[ev.pointerType] || ev.pointerType;\n\n        var isTouch = (pointerType == INPUT_TYPE_TOUCH);\n\n        // get index of the event in the store\n        var storeIndex = inArray(store, ev.pointerId, 'pointerId');\n\n        // start and mouse must be down\n        if (eventType & INPUT_START && (ev.button === 0 || isTouch)) {\n            if (storeIndex < 0) {\n                store.push(ev);\n                storeIndex = store.length - 1;\n            }\n        } else if (eventType & (INPUT_END | INPUT_CANCEL)) {\n            removePointer = true;\n        }\n\n        // it not found, so the pointer hasn't been down (so it's probably a hover)\n        if (storeIndex < 0) {\n            return;\n        }\n\n        // update the event in the store\n        store[storeIndex] = ev;\n\n        this.callback(this.manager, eventType, {\n            pointers: store,\n            changedPointers: [ev],\n            pointerType: pointerType,\n            srcEvent: ev\n        });\n\n        if (removePointer) {\n            // remove from the store\n            store.splice(storeIndex, 1);\n        }\n    }\n});\n\nvar SINGLE_TOUCH_INPUT_MAP = {\n    touchstart: INPUT_START,\n    touchmove: INPUT_MOVE,\n    touchend: INPUT_END,\n    touchcancel: INPUT_CANCEL\n};\n\nvar SINGLE_TOUCH_TARGET_EVENTS = 'touchstart';\nvar SINGLE_TOUCH_WINDOW_EVENTS = 'touchstart touchmove touchend touchcancel';\n\n/**\n * Touch events input\n * @constructor\n * @extends Input\n */\nfunction SingleTouchInput() {\n    this.evTarget = SINGLE_TOUCH_TARGET_EVENTS;\n    this.evWin = SINGLE_TOUCH_WINDOW_EVENTS;\n    this.started = false;\n\n    Input.apply(this, arguments);\n}\n\ninherit(SingleTouchInput, Input, {\n    handler: function TEhandler(ev) {\n        var type = SINGLE_TOUCH_INPUT_MAP[ev.type];\n\n        // should we handle the touch events?\n        if (type === INPUT_START) {\n            this.started = true;\n        }\n\n        if (!this.started) {\n            return;\n        }\n\n        var touches = normalizeSingleTouches.call(this, ev, type);\n\n        // when done, reset the started state\n        if (type & (INPUT_END | INPUT_CANCEL) && touches[0].length - touches[1].length === 0) {\n            this.started = false;\n        }\n\n        this.callback(this.manager, type, {\n            pointers: touches[0],\n            changedPointers: touches[1],\n            pointerType: INPUT_TYPE_TOUCH,\n            srcEvent: ev\n        });\n    }\n});\n\n/**\n * @this {TouchInput}\n * @param {Object} ev\n * @param {Number} type flag\n * @returns {undefined|Array} [all, changed]\n */\nfunction normalizeSingleTouches(ev, type) {\n    var all = toArray(ev.touches);\n    var changed = toArray(ev.changedTouches);\n\n    if (type & (INPUT_END | INPUT_CANCEL)) {\n        all = uniqueArray(all.concat(changed), 'identifier', true);\n    }\n\n    return [all, changed];\n}\n\nvar TOUCH_INPUT_MAP = {\n    touchstart: INPUT_START,\n    touchmove: INPUT_MOVE,\n    touchend: INPUT_END,\n    touchcancel: INPUT_CANCEL\n};\n\nvar TOUCH_TARGET_EVENTS = 'touchstart touchmove touchend touchcancel';\n\n/**\n * Multi-user touch events input\n * @constructor\n * @extends Input\n */\nfunction TouchInput() {\n    this.evTarget = TOUCH_TARGET_EVENTS;\n    this.targetIds = {};\n\n    Input.apply(this, arguments);\n}\n\ninherit(TouchInput, Input, {\n    handler: function MTEhandler(ev) {\n        var type = TOUCH_INPUT_MAP[ev.type];\n        var touches = getTouches.call(this, ev, type);\n        if (!touches) {\n            return;\n        }\n\n        this.callback(this.manager, type, {\n            pointers: touches[0],\n            changedPointers: touches[1],\n            pointerType: INPUT_TYPE_TOUCH,\n            srcEvent: ev\n        });\n    }\n});\n\n/**\n * @this {TouchInput}\n * @param {Object} ev\n * @param {Number} type flag\n * @returns {undefined|Array} [all, changed]\n */\nfunction getTouches(ev, type) {\n    var allTouches = toArray(ev.touches);\n    var targetIds = this.targetIds;\n\n    // when there is only one touch, the process can be simplified\n    if (type & (INPUT_START | INPUT_MOVE) && allTouches.length === 1) {\n        targetIds[allTouches[0].identifier] = true;\n        return [allTouches, allTouches];\n    }\n\n    var i,\n        targetTouches,\n        changedTouches = toArray(ev.changedTouches),\n        changedTargetTouches = [],\n        target = this.target;\n\n    // get target touches from touches\n    targetTouches = allTouches.filter(function(touch) {\n        return hasParent(touch.target, target);\n    });\n\n    // collect touches\n    if (type === INPUT_START) {\n        i = 0;\n        while (i < targetTouches.length) {\n            targetIds[targetTouches[i].identifier] = true;\n            i++;\n        }\n    }\n\n    // filter changed touches to only contain touches that exist in the collected target ids\n    i = 0;\n    while (i < changedTouches.length) {\n        if (targetIds[changedTouches[i].identifier]) {\n            changedTargetTouches.push(changedTouches[i]);\n        }\n\n        // cleanup removed touches\n        if (type & (INPUT_END | INPUT_CANCEL)) {\n            delete targetIds[changedTouches[i].identifier];\n        }\n        i++;\n    }\n\n    if (!changedTargetTouches.length) {\n        return;\n    }\n\n    return [\n        // merge targetTouches with changedTargetTouches so it contains ALL touches, including 'end' and 'cancel'\n        uniqueArray(targetTouches.concat(changedTargetTouches), 'identifier', true),\n        changedTargetTouches\n    ];\n}\n\n/**\n * Combined touch and mouse input\n *\n * Touch has a higher priority then mouse, and while touching no mouse events are allowed.\n * This because touch devices also emit mouse events while doing a touch.\n *\n * @constructor\n * @extends Input\n */\n\nvar DEDUP_TIMEOUT = 2500;\nvar DEDUP_DISTANCE = 25;\n\nfunction TouchMouseInput() {\n    Input.apply(this, arguments);\n\n    var handler = bindFn(this.handler, this);\n    this.touch = new TouchInput(this.manager, handler);\n    this.mouse = new MouseInput(this.manager, handler);\n\n    this.primaryTouch = null;\n    this.lastTouches = [];\n}\n\ninherit(TouchMouseInput, Input, {\n    /**\n     * handle mouse and touch events\n     * @param {Hammer} manager\n     * @param {String} inputEvent\n     * @param {Object} inputData\n     */\n    handler: function TMEhandler(manager, inputEvent, inputData) {\n        var isTouch = (inputData.pointerType == INPUT_TYPE_TOUCH),\n            isMouse = (inputData.pointerType == INPUT_TYPE_MOUSE);\n\n        if (isMouse && inputData.sourceCapabilities && inputData.sourceCapabilities.firesTouchEvents) {\n            return;\n        }\n\n        // when we're in a touch event, record touches to  de-dupe synthetic mouse event\n        if (isTouch) {\n            recordTouches.call(this, inputEvent, inputData);\n        } else if (isMouse && isSyntheticEvent.call(this, inputData)) {\n            return;\n        }\n\n        this.callback(manager, inputEvent, inputData);\n    },\n\n    /**\n     * remove the event listeners\n     */\n    destroy: function destroy() {\n        this.touch.destroy();\n        this.mouse.destroy();\n    }\n});\n\nfunction recordTouches(eventType, eventData) {\n    if (eventType & INPUT_START) {\n        this.primaryTouch = eventData.changedPointers[0].identifier;\n        setLastTouch.call(this, eventData);\n    } else if (eventType & (INPUT_END | INPUT_CANCEL)) {\n        setLastTouch.call(this, eventData);\n    }\n}\n\nfunction setLastTouch(eventData) {\n    var touch = eventData.changedPointers[0];\n\n    if (touch.identifier === this.primaryTouch) {\n        var lastTouch = {x: touch.clientX, y: touch.clientY};\n        this.lastTouches.push(lastTouch);\n        var lts = this.lastTouches;\n        var removeLastTouch = function() {\n            var i = lts.indexOf(lastTouch);\n            if (i > -1) {\n                lts.splice(i, 1);\n            }\n        };\n        setTimeout(removeLastTouch, DEDUP_TIMEOUT);\n    }\n}\n\nfunction isSyntheticEvent(eventData) {\n    var x = eventData.srcEvent.clientX, y = eventData.srcEvent.clientY;\n    for (var i = 0; i < this.lastTouches.length; i++) {\n        var t = this.lastTouches[i];\n        var dx = Math.abs(x - t.x), dy = Math.abs(y - t.y);\n        if (dx <= DEDUP_DISTANCE && dy <= DEDUP_DISTANCE) {\n            return true;\n        }\n    }\n    return false;\n}\n\nvar PREFIXED_TOUCH_ACTION = prefixed(TEST_ELEMENT.style, 'touchAction');\nvar NATIVE_TOUCH_ACTION = PREFIXED_TOUCH_ACTION !== undefined;\n\n// magical touchAction value\nvar TOUCH_ACTION_COMPUTE = 'compute';\nvar TOUCH_ACTION_AUTO = 'auto';\nvar TOUCH_ACTION_MANIPULATION = 'manipulation'; // not implemented\nvar TOUCH_ACTION_NONE = 'none';\nvar TOUCH_ACTION_PAN_X = 'pan-x';\nvar TOUCH_ACTION_PAN_Y = 'pan-y';\nvar TOUCH_ACTION_MAP = getTouchActionProps();\n\n/**\n * Touch Action\n * sets the touchAction property or uses the js alternative\n * @param {Manager} manager\n * @param {String} value\n * @constructor\n */\nfunction TouchAction(manager, value) {\n    this.manager = manager;\n    this.set(value);\n}\n\nTouchAction.prototype = {\n    /**\n     * set the touchAction value on the element or enable the polyfill\n     * @param {String} value\n     */\n    set: function(value) {\n        // find out the touch-action by the event handlers\n        if (value == TOUCH_ACTION_COMPUTE) {\n            value = this.compute();\n        }\n\n        if (NATIVE_TOUCH_ACTION && this.manager.element.style && TOUCH_ACTION_MAP[value]) {\n            this.manager.element.style[PREFIXED_TOUCH_ACTION] = value;\n        }\n        this.actions = value.toLowerCase().trim();\n    },\n\n    /**\n     * just re-set the touchAction value\n     */\n    update: function() {\n        this.set(this.manager.options.touchAction);\n    },\n\n    /**\n     * compute the value for the touchAction property based on the recognizer's settings\n     * @returns {String} value\n     */\n    compute: function() {\n        var actions = [];\n        each(this.manager.recognizers, function(recognizer) {\n            if (boolOrFn(recognizer.options.enable, [recognizer])) {\n                actions = actions.concat(recognizer.getTouchAction());\n            }\n        });\n        return cleanTouchActions(actions.join(' '));\n    },\n\n    /**\n     * this method is called on each input cycle and provides the preventing of the browser behavior\n     * @param {Object} input\n     */\n    preventDefaults: function(input) {\n        var srcEvent = input.srcEvent;\n        var direction = input.offsetDirection;\n\n        // if the touch action did prevented once this session\n        if (this.manager.session.prevented) {\n            srcEvent.preventDefault();\n            return;\n        }\n\n        var actions = this.actions;\n        var hasNone = inStr(actions, TOUCH_ACTION_NONE) && !TOUCH_ACTION_MAP[TOUCH_ACTION_NONE];\n        var hasPanY = inStr(actions, TOUCH_ACTION_PAN_Y) && !TOUCH_ACTION_MAP[TOUCH_ACTION_PAN_Y];\n        var hasPanX = inStr(actions, TOUCH_ACTION_PAN_X) && !TOUCH_ACTION_MAP[TOUCH_ACTION_PAN_X];\n\n        if (hasNone) {\n            //do not prevent defaults if this is a tap gesture\n\n            var isTapPointer = input.pointers.length === 1;\n            var isTapMovement = input.distance < 2;\n            var isTapTouchTime = input.deltaTime < 250;\n\n            if (isTapPointer && isTapMovement && isTapTouchTime) {\n                return;\n            }\n        }\n\n        if (hasPanX && hasPanY) {\n            // `pan-x pan-y` means browser handles all scrolling/panning, do not prevent\n            return;\n        }\n\n        if (hasNone ||\n            (hasPanY && direction & DIRECTION_HORIZONTAL) ||\n            (hasPanX && direction & DIRECTION_VERTICAL)) {\n            return this.preventSrc(srcEvent);\n        }\n    },\n\n    /**\n     * call preventDefault to prevent the browser's default behavior (scrolling in most cases)\n     * @param {Object} srcEvent\n     */\n    preventSrc: function(srcEvent) {\n        this.manager.session.prevented = true;\n        srcEvent.preventDefault();\n    }\n};\n\n/**\n * when the touchActions are collected they are not a valid value, so we need to clean things up. *\n * @param {String} actions\n * @returns {*}\n */\nfunction cleanTouchActions(actions) {\n    // none\n    if (inStr(actions, TOUCH_ACTION_NONE)) {\n        return TOUCH_ACTION_NONE;\n    }\n\n    var hasPanX = inStr(actions, TOUCH_ACTION_PAN_X);\n    var hasPanY = inStr(actions, TOUCH_ACTION_PAN_Y);\n\n    // if both pan-x and pan-y are set (different recognizers\n    // for different directions, e.g. horizontal pan but vertical swipe?)\n    // we need none (as otherwise with pan-x pan-y combined none of these\n    // recognizers will work, since the browser would handle all panning\n    if (hasPanX && hasPanY) {\n        return TOUCH_ACTION_NONE;\n    }\n\n    // pan-x OR pan-y\n    if (hasPanX || hasPanY) {\n        return hasPanX ? TOUCH_ACTION_PAN_X : TOUCH_ACTION_PAN_Y;\n    }\n\n    // manipulation\n    if (inStr(actions, TOUCH_ACTION_MANIPULATION)) {\n        return TOUCH_ACTION_MANIPULATION;\n    }\n\n    return TOUCH_ACTION_AUTO;\n}\n\nfunction getTouchActionProps() {\n    if (!NATIVE_TOUCH_ACTION) {\n        return false;\n    }\n    var touchMap = {};\n    var cssSupports = window.CSS && window.CSS.supports;\n    ['auto', 'manipulation', 'pan-y', 'pan-x', 'pan-x pan-y', 'none'].forEach(function(val) {\n\n        // If css.supports is not supported but there is native touch-action assume it supports\n        // all values. This is the case for IE 10 and 11.\n        touchMap[val] = cssSupports ? window.CSS.supports('touch-action', val) : true;\n    });\n    return touchMap;\n}\n\n/**\n * Recognizer flow explained; *\n * All recognizers have the initial state of POSSIBLE when a input session starts.\n * The definition of a input session is from the first input until the last input, with all it's movement in it. *\n * Example session for mouse-input: mousedown -> mousemove -> mouseup\n *\n * On each recognizing cycle (see Manager.recognize) the .recognize() method is executed\n * which determines with state it should be.\n *\n * If the recognizer has the state FAILED, CANCELLED or RECOGNIZED (equals ENDED), it is reset to\n * POSSIBLE to give it another change on the next cycle.\n *\n *               Possible\n *                  |\n *            +-----+---------------+\n *            |                     |\n *      +-----+-----+               |\n *      |           |               |\n *   Failed      Cancelled          |\n *                          +-------+------+\n *                          |              |\n *                      Recognized       Began\n *                                         |\n *                                      Changed\n *                                         |\n *                                  Ended/Recognized\n */\nvar STATE_POSSIBLE = 1;\nvar STATE_BEGAN = 2;\nvar STATE_CHANGED = 4;\nvar STATE_ENDED = 8;\nvar STATE_RECOGNIZED = STATE_ENDED;\nvar STATE_CANCELLED = 16;\nvar STATE_FAILED = 32;\n\n/**\n * Recognizer\n * Every recognizer needs to extend from this class.\n * @constructor\n * @param {Object} options\n */\nfunction Recognizer(options) {\n    this.options = assign({}, this.defaults, options || {});\n\n    this.id = uniqueId();\n\n    this.manager = null;\n\n    // default is enable true\n    this.options.enable = ifUndefined(this.options.enable, true);\n\n    this.state = STATE_POSSIBLE;\n\n    this.simultaneous = {};\n    this.requireFail = [];\n}\n\nRecognizer.prototype = {\n    /**\n     * @virtual\n     * @type {Object}\n     */\n    defaults: {},\n\n    /**\n     * set options\n     * @param {Object} options\n     * @return {Recognizer}\n     */\n    set: function(options) {\n        assign(this.options, options);\n\n        // also update the touchAction, in case something changed about the directions/enabled state\n        this.manager && this.manager.touchAction.update();\n        return this;\n    },\n\n    /**\n     * recognize simultaneous with an other recognizer.\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    recognizeWith: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'recognizeWith', this)) {\n            return this;\n        }\n\n        var simultaneous = this.simultaneous;\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        if (!simultaneous[otherRecognizer.id]) {\n            simultaneous[otherRecognizer.id] = otherRecognizer;\n            otherRecognizer.recognizeWith(this);\n        }\n        return this;\n    },\n\n    /**\n     * drop the simultaneous link. it doesnt remove the link on the other recognizer.\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    dropRecognizeWith: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'dropRecognizeWith', this)) {\n            return this;\n        }\n\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        delete this.simultaneous[otherRecognizer.id];\n        return this;\n    },\n\n    /**\n     * recognizer can only run when an other is failing\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    requireFailure: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'requireFailure', this)) {\n            return this;\n        }\n\n        var requireFail = this.requireFail;\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        if (inArray(requireFail, otherRecognizer) === -1) {\n            requireFail.push(otherRecognizer);\n            otherRecognizer.requireFailure(this);\n        }\n        return this;\n    },\n\n    /**\n     * drop the requireFailure link. it does not remove the link on the other recognizer.\n     * @param {Recognizer} otherRecognizer\n     * @returns {Recognizer} this\n     */\n    dropRequireFailure: function(otherRecognizer) {\n        if (invokeArrayArg(otherRecognizer, 'dropRequireFailure', this)) {\n            return this;\n        }\n\n        otherRecognizer = getRecognizerByNameIfManager(otherRecognizer, this);\n        var index = inArray(this.requireFail, otherRecognizer);\n        if (index > -1) {\n            this.requireFail.splice(index, 1);\n        }\n        return this;\n    },\n\n    /**\n     * has require failures boolean\n     * @returns {boolean}\n     */\n    hasRequireFailures: function() {\n        return this.requireFail.length > 0;\n    },\n\n    /**\n     * if the recognizer can recognize simultaneous with an other recognizer\n     * @param {Recognizer} otherRecognizer\n     * @returns {Boolean}\n     */\n    canRecognizeWith: function(otherRecognizer) {\n        return !!this.simultaneous[otherRecognizer.id];\n    },\n\n    /**\n     * You should use `tryEmit` instead of `emit` directly to check\n     * that all the needed recognizers has failed before emitting.\n     * @param {Object} input\n     */\n    emit: function(input) {\n        var self = this;\n        var state = this.state;\n\n        function emit(event) {\n            self.manager.emit(event, input);\n        }\n\n        // 'panstart' and 'panmove'\n        if (state < STATE_ENDED) {\n            emit(self.options.event + stateStr(state));\n        }\n\n        emit(self.options.event); // simple 'eventName' events\n\n        if (input.additionalEvent) { // additional event(panleft, panright, pinchin, pinchout...)\n            emit(input.additionalEvent);\n        }\n\n        // panend and pancancel\n        if (state >= STATE_ENDED) {\n            emit(self.options.event + stateStr(state));\n        }\n    },\n\n    /**\n     * Check that all the require failure recognizers has failed,\n     * if true, it emits a gesture event,\n     * otherwise, setup the state to FAILED.\n     * @param {Object} input\n     */\n    tryEmit: function(input) {\n        if (this.canEmit()) {\n            return this.emit(input);\n        }\n        // it's failing anyway\n        this.state = STATE_FAILED;\n    },\n\n    /**\n     * can we emit?\n     * @returns {boolean}\n     */\n    canEmit: function() {\n        var i = 0;\n        while (i < this.requireFail.length) {\n            if (!(this.requireFail[i].state & (STATE_FAILED | STATE_POSSIBLE))) {\n                return false;\n            }\n            i++;\n        }\n        return true;\n    },\n\n    /**\n     * update the recognizer\n     * @param {Object} inputData\n     */\n    recognize: function(inputData) {\n        // make a new copy of the inputData\n        // so we can change the inputData without messing up the other recognizers\n        var inputDataClone = assign({}, inputData);\n\n        // is is enabled and allow recognizing?\n        if (!boolOrFn(this.options.enable, [this, inputDataClone])) {\n            this.reset();\n            this.state = STATE_FAILED;\n            return;\n        }\n\n        // reset when we've reached the end\n        if (this.state & (STATE_RECOGNIZED | STATE_CANCELLED | STATE_FAILED)) {\n            this.state = STATE_POSSIBLE;\n        }\n\n        this.state = this.process(inputDataClone);\n\n        // the recognizer has recognized a gesture\n        // so trigger an event\n        if (this.state & (STATE_BEGAN | STATE_CHANGED | STATE_ENDED | STATE_CANCELLED)) {\n            this.tryEmit(inputDataClone);\n        }\n    },\n\n    /**\n     * return the state of the recognizer\n     * the actual recognizing happens in this method\n     * @virtual\n     * @param {Object} inputData\n     * @returns {Const} STATE\n     */\n    process: function(inputData) { }, // jshint ignore:line\n\n    /**\n     * return the preferred touch-action\n     * @virtual\n     * @returns {Array}\n     */\n    getTouchAction: function() { },\n\n    /**\n     * called when the gesture isn't allowed to recognize\n     * like when another is being recognized or it is disabled\n     * @virtual\n     */\n    reset: function() { }\n};\n\n/**\n * get a usable string, used as event postfix\n * @param {Const} state\n * @returns {String} state\n */\nfunction stateStr(state) {\n    if (state & STATE_CANCELLED) {\n        return 'cancel';\n    } else if (state & STATE_ENDED) {\n        return 'end';\n    } else if (state & STATE_CHANGED) {\n        return 'move';\n    } else if (state & STATE_BEGAN) {\n        return 'start';\n    }\n    return '';\n}\n\n/**\n * direction cons to string\n * @param {Const} direction\n * @returns {String}\n */\nfunction directionStr(direction) {\n    if (direction == DIRECTION_DOWN) {\n        return 'down';\n    } else if (direction == DIRECTION_UP) {\n        return 'up';\n    } else if (direction == DIRECTION_LEFT) {\n        return 'left';\n    } else if (direction == DIRECTION_RIGHT) {\n        return 'right';\n    }\n    return '';\n}\n\n/**\n * get a recognizer by name if it is bound to a manager\n * @param {Recognizer|String} otherRecognizer\n * @param {Recognizer} recognizer\n * @returns {Recognizer}\n */\nfunction getRecognizerByNameIfManager(otherRecognizer, recognizer) {\n    var manager = recognizer.manager;\n    if (manager) {\n        return manager.get(otherRecognizer);\n    }\n    return otherRecognizer;\n}\n\n/**\n * This recognizer is just used as a base for the simple attribute recognizers.\n * @constructor\n * @extends Recognizer\n */\nfunction AttrRecognizer() {\n    Recognizer.apply(this, arguments);\n}\n\ninherit(AttrRecognizer, Recognizer, {\n    /**\n     * @namespace\n     * @memberof AttrRecognizer\n     */\n    defaults: {\n        /**\n         * @type {Number}\n         * @default 1\n         */\n        pointers: 1\n    },\n\n    /**\n     * Used to check if it the recognizer receives valid input, like input.distance > 10.\n     * @memberof AttrRecognizer\n     * @param {Object} input\n     * @returns {Boolean} recognized\n     */\n    attrTest: function(input) {\n        var optionPointers = this.options.pointers;\n        return optionPointers === 0 || input.pointers.length === optionPointers;\n    },\n\n    /**\n     * Process the input and return the state for the recognizer\n     * @memberof AttrRecognizer\n     * @param {Object} input\n     * @returns {*} State\n     */\n    process: function(input) {\n        var state = this.state;\n        var eventType = input.eventType;\n\n        var isRecognized = state & (STATE_BEGAN | STATE_CHANGED);\n        var isValid = this.attrTest(input);\n\n        // on cancel input and we've recognized before, return STATE_CANCELLED\n        if (isRecognized && (eventType & INPUT_CANCEL || !isValid)) {\n            return state | STATE_CANCELLED;\n        } else if (isRecognized || isValid) {\n            if (eventType & INPUT_END) {\n                return state | STATE_ENDED;\n            } else if (!(state & STATE_BEGAN)) {\n                return STATE_BEGAN;\n            }\n            return state | STATE_CHANGED;\n        }\n        return STATE_FAILED;\n    }\n});\n\n/**\n * Pan\n * Recognized when the pointer is down and moved in the allowed direction.\n * @constructor\n * @extends AttrRecognizer\n */\nfunction PanRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n\n    this.pX = null;\n    this.pY = null;\n}\n\ninherit(PanRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof PanRecognizer\n     */\n    defaults: {\n        event: 'pan',\n        threshold: 10,\n        pointers: 1,\n        direction: DIRECTION_ALL\n    },\n\n    getTouchAction: function() {\n        var direction = this.options.direction;\n        var actions = [];\n        if (direction & DIRECTION_HORIZONTAL) {\n            actions.push(TOUCH_ACTION_PAN_Y);\n        }\n        if (direction & DIRECTION_VERTICAL) {\n            actions.push(TOUCH_ACTION_PAN_X);\n        }\n        return actions;\n    },\n\n    directionTest: function(input) {\n        var options = this.options;\n        var hasMoved = true;\n        var distance = input.distance;\n        var direction = input.direction;\n        var x = input.deltaX;\n        var y = input.deltaY;\n\n        // lock to axis?\n        if (!(direction & options.direction)) {\n            if (options.direction & DIRECTION_HORIZONTAL) {\n                direction = (x === 0) ? DIRECTION_NONE : (x < 0) ? DIRECTION_LEFT : DIRECTION_RIGHT;\n                hasMoved = x != this.pX;\n                distance = Math.abs(input.deltaX);\n            } else {\n                direction = (y === 0) ? DIRECTION_NONE : (y < 0) ? DIRECTION_UP : DIRECTION_DOWN;\n                hasMoved = y != this.pY;\n                distance = Math.abs(input.deltaY);\n            }\n        }\n        input.direction = direction;\n        return hasMoved && distance > options.threshold && direction & options.direction;\n    },\n\n    attrTest: function(input) {\n        return AttrRecognizer.prototype.attrTest.call(this, input) &&\n            (this.state & STATE_BEGAN || (!(this.state & STATE_BEGAN) && this.directionTest(input)));\n    },\n\n    emit: function(input) {\n\n        this.pX = input.deltaX;\n        this.pY = input.deltaY;\n\n        var direction = directionStr(input.direction);\n\n        if (direction) {\n            input.additionalEvent = this.options.event + direction;\n        }\n        this._super.emit.call(this, input);\n    }\n});\n\n/**\n * Pinch\n * Recognized when two or more pointers are moving toward (zoom-in) or away from each other (zoom-out).\n * @constructor\n * @extends AttrRecognizer\n */\nfunction PinchRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n}\n\ninherit(PinchRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof PinchRecognizer\n     */\n    defaults: {\n        event: 'pinch',\n        threshold: 0,\n        pointers: 2\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_NONE];\n    },\n\n    attrTest: function(input) {\n        return this._super.attrTest.call(this, input) &&\n            (Math.abs(input.scale - 1) > this.options.threshold || this.state & STATE_BEGAN);\n    },\n\n    emit: function(input) {\n        if (input.scale !== 1) {\n            var inOut = input.scale < 1 ? 'in' : 'out';\n            input.additionalEvent = this.options.event + inOut;\n        }\n        this._super.emit.call(this, input);\n    }\n});\n\n/**\n * Press\n * Recognized when the pointer is down for x ms without any movement.\n * @constructor\n * @extends Recognizer\n */\nfunction PressRecognizer() {\n    Recognizer.apply(this, arguments);\n\n    this._timer = null;\n    this._input = null;\n}\n\ninherit(PressRecognizer, Recognizer, {\n    /**\n     * @namespace\n     * @memberof PressRecognizer\n     */\n    defaults: {\n        event: 'press',\n        pointers: 1,\n        time: 251, // minimal time of the pointer to be pressed\n        threshold: 9 // a minimal movement is ok, but keep it low\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_AUTO];\n    },\n\n    process: function(input) {\n        var options = this.options;\n        var validPointers = input.pointers.length === options.pointers;\n        var validMovement = input.distance < options.threshold;\n        var validTime = input.deltaTime > options.time;\n\n        this._input = input;\n\n        // we only allow little movement\n        // and we've reached an end event, so a tap is possible\n        if (!validMovement || !validPointers || (input.eventType & (INPUT_END | INPUT_CANCEL) && !validTime)) {\n            this.reset();\n        } else if (input.eventType & INPUT_START) {\n            this.reset();\n            this._timer = setTimeoutContext(function() {\n                this.state = STATE_RECOGNIZED;\n                this.tryEmit();\n            }, options.time, this);\n        } else if (input.eventType & INPUT_END) {\n            return STATE_RECOGNIZED;\n        }\n        return STATE_FAILED;\n    },\n\n    reset: function() {\n        clearTimeout(this._timer);\n    },\n\n    emit: function(input) {\n        if (this.state !== STATE_RECOGNIZED) {\n            return;\n        }\n\n        if (input && (input.eventType & INPUT_END)) {\n            this.manager.emit(this.options.event + 'up', input);\n        } else {\n            this._input.timeStamp = now();\n            this.manager.emit(this.options.event, this._input);\n        }\n    }\n});\n\n/**\n * Rotate\n * Recognized when two or more pointer are moving in a circular motion.\n * @constructor\n * @extends AttrRecognizer\n */\nfunction RotateRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n}\n\ninherit(RotateRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof RotateRecognizer\n     */\n    defaults: {\n        event: 'rotate',\n        threshold: 0,\n        pointers: 2\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_NONE];\n    },\n\n    attrTest: function(input) {\n        return this._super.attrTest.call(this, input) &&\n            (Math.abs(input.rotation) > this.options.threshold || this.state & STATE_BEGAN);\n    }\n});\n\n/**\n * Swipe\n * Recognized when the pointer is moving fast (velocity), with enough distance in the allowed direction.\n * @constructor\n * @extends AttrRecognizer\n */\nfunction SwipeRecognizer() {\n    AttrRecognizer.apply(this, arguments);\n}\n\ninherit(SwipeRecognizer, AttrRecognizer, {\n    /**\n     * @namespace\n     * @memberof SwipeRecognizer\n     */\n    defaults: {\n        event: 'swipe',\n        threshold: 10,\n        velocity: 0.3,\n        direction: DIRECTION_HORIZONTAL | DIRECTION_VERTICAL,\n        pointers: 1\n    },\n\n    getTouchAction: function() {\n        return PanRecognizer.prototype.getTouchAction.call(this);\n    },\n\n    attrTest: function(input) {\n        var direction = this.options.direction;\n        var velocity;\n\n        if (direction & (DIRECTION_HORIZONTAL | DIRECTION_VERTICAL)) {\n            velocity = input.overallVelocity;\n        } else if (direction & DIRECTION_HORIZONTAL) {\n            velocity = input.overallVelocityX;\n        } else if (direction & DIRECTION_VERTICAL) {\n            velocity = input.overallVelocityY;\n        }\n\n        return this._super.attrTest.call(this, input) &&\n            direction & input.offsetDirection &&\n            input.distance > this.options.threshold &&\n            input.maxPointers == this.options.pointers &&\n            abs(velocity) > this.options.velocity && input.eventType & INPUT_END;\n    },\n\n    emit: function(input) {\n        var direction = directionStr(input.offsetDirection);\n        if (direction) {\n            this.manager.emit(this.options.event + direction, input);\n        }\n\n        this.manager.emit(this.options.event, input);\n    }\n});\n\n/**\n * A tap is ecognized when the pointer is doing a small tap/click. Multiple taps are recognized if they occur\n * between the given interval and position. The delay option can be used to recognize multi-taps without firing\n * a single tap.\n *\n * The eventData from the emitted event contains the property `tapCount`, which contains the amount of\n * multi-taps being recognized.\n * @constructor\n * @extends Recognizer\n */\nfunction TapRecognizer() {\n    Recognizer.apply(this, arguments);\n\n    // previous time and center,\n    // used for tap counting\n    this.pTime = false;\n    this.pCenter = false;\n\n    this._timer = null;\n    this._input = null;\n    this.count = 0;\n}\n\ninherit(TapRecognizer, Recognizer, {\n    /**\n     * @namespace\n     * @memberof PinchRecognizer\n     */\n    defaults: {\n        event: 'tap',\n        pointers: 1,\n        taps: 1,\n        interval: 300, // max time between the multi-tap taps\n        time: 250, // max time of the pointer to be down (like finger on the screen)\n        threshold: 9, // a minimal movement is ok, but keep it low\n        posThreshold: 10 // a multi-tap can be a bit off the initial position\n    },\n\n    getTouchAction: function() {\n        return [TOUCH_ACTION_MANIPULATION];\n    },\n\n    process: function(input) {\n        var options = this.options;\n\n        var validPointers = input.pointers.length === options.pointers;\n        var validMovement = input.distance < options.threshold;\n        var validTouchTime = input.deltaTime < options.time;\n\n        this.reset();\n\n        if ((input.eventType & INPUT_START) && (this.count === 0)) {\n            return this.failTimeout();\n        }\n\n        // we only allow little movement\n        // and we've reached an end event, so a tap is possible\n        if (validMovement && validTouchTime && validPointers) {\n            if (input.eventType != INPUT_END) {\n                return this.failTimeout();\n            }\n\n            var validInterval = this.pTime ? (input.timeStamp - this.pTime < options.interval) : true;\n            var validMultiTap = !this.pCenter || getDistance(this.pCenter, input.center) < options.posThreshold;\n\n            this.pTime = input.timeStamp;\n            this.pCenter = input.center;\n\n            if (!validMultiTap || !validInterval) {\n                this.count = 1;\n            } else {\n                this.count += 1;\n            }\n\n            this._input = input;\n\n            // if tap count matches we have recognized it,\n            // else it has began recognizing...\n            var tapCount = this.count % options.taps;\n            if (tapCount === 0) {\n                // no failing requirements, immediately trigger the tap event\n                // or wait as long as the multitap interval to trigger\n                if (!this.hasRequireFailures()) {\n                    return STATE_RECOGNIZED;\n                } else {\n                    this._timer = setTimeoutContext(function() {\n                        this.state = STATE_RECOGNIZED;\n                        this.tryEmit();\n                    }, options.interval, this);\n                    return STATE_BEGAN;\n                }\n            }\n        }\n        return STATE_FAILED;\n    },\n\n    failTimeout: function() {\n        this._timer = setTimeoutContext(function() {\n            this.state = STATE_FAILED;\n        }, this.options.interval, this);\n        return STATE_FAILED;\n    },\n\n    reset: function() {\n        clearTimeout(this._timer);\n    },\n\n    emit: function() {\n        if (this.state == STATE_RECOGNIZED) {\n            this._input.tapCount = this.count;\n            this.manager.emit(this.options.event, this._input);\n        }\n    }\n});\n\n/**\n * Simple way to create a manager with a default set of recognizers.\n * @param {HTMLElement} element\n * @param {Object} [options]\n * @constructor\n */\nfunction Hammer(element, options) {\n    options = options || {};\n    options.recognizers = ifUndefined(options.recognizers, Hammer.defaults.preset);\n    return new Manager(element, options);\n}\n\n/**\n * @const {string}\n */\nHammer.VERSION = '2.0.7';\n\n/**\n * default settings\n * @namespace\n */\nHammer.defaults = {\n    /**\n     * set if DOM events are being triggered.\n     * But this is slower and unused by simple implementations, so disabled by default.\n     * @type {Boolean}\n     * @default false\n     */\n    domEvents: false,\n\n    /**\n     * The value for the touchAction property/fallback.\n     * When set to `compute` it will magically set the correct value based on the added recognizers.\n     * @type {String}\n     * @default compute\n     */\n    touchAction: TOUCH_ACTION_COMPUTE,\n\n    /**\n     * @type {Boolean}\n     * @default true\n     */\n    enable: true,\n\n    /**\n     * EXPERIMENTAL FEATURE -- can be removed/changed\n     * Change the parent input target element.\n     * If Null, then it is being set the to main element.\n     * @type {Null|EventTarget}\n     * @default null\n     */\n    inputTarget: null,\n\n    /**\n     * force an input class\n     * @type {Null|Function}\n     * @default null\n     */\n    inputClass: null,\n\n    /**\n     * Default recognizer setup when calling `Hammer()`\n     * When creating a new Manager these will be skipped.\n     * @type {Array}\n     */\n    preset: [\n        // RecognizerClass, options, [recognizeWith, ...], [requireFailure, ...]\n        [RotateRecognizer, {enable: false}],\n        [PinchRecognizer, {enable: false}, ['rotate']],\n        [SwipeRecognizer, {direction: DIRECTION_HORIZONTAL}],\n        [PanRecognizer, {direction: DIRECTION_HORIZONTAL}, ['swipe']],\n        [TapRecognizer],\n        [TapRecognizer, {event: 'doubletap', taps: 2}, ['tap']],\n        [PressRecognizer]\n    ],\n\n    /**\n     * Some CSS properties can be used to improve the working of Hammer.\n     * Add them to this method and they will be set when creating a new Manager.\n     * @namespace\n     */\n    cssProps: {\n        /**\n         * Disables text selection to improve the dragging gesture. Mainly for desktop browsers.\n         * @type {String}\n         * @default 'none'\n         */\n        userSelect: 'none',\n\n        /**\n         * Disable the Windows Phone grippers when pressing an element.\n         * @type {String}\n         * @default 'none'\n         */\n        touchSelect: 'none',\n\n        /**\n         * Disables the default callout shown when you touch and hold a touch target.\n         * On iOS, when you touch and hold a touch target such as a link, Safari displays\n         * a callout containing information about the link. This property allows you to disable that callout.\n         * @type {String}\n         * @default 'none'\n         */\n        touchCallout: 'none',\n\n        /**\n         * Specifies whether zooming is enabled. Used by IE10>\n         * @type {String}\n         * @default 'none'\n         */\n        contentZooming: 'none',\n\n        /**\n         * Specifies that an entire element should be draggable instead of its contents. Mainly for desktop browsers.\n         * @type {String}\n         * @default 'none'\n         */\n        userDrag: 'none',\n\n        /**\n         * Overrides the highlight color shown when the user taps a link or a JavaScript\n         * clickable element in iOS. This property obeys the alpha value, if specified.\n         * @type {String}\n         * @default 'rgba(0,0,0,0)'\n         */\n        tapHighlightColor: 'rgba(0,0,0,0)'\n    }\n};\n\nvar STOP = 1;\nvar FORCED_STOP = 2;\n\n/**\n * Manager\n * @param {HTMLElement} element\n * @param {Object} [options]\n * @constructor\n */\nfunction Manager(element, options) {\n    this.options = assign({}, Hammer.defaults, options || {});\n\n    this.options.inputTarget = this.options.inputTarget || element;\n\n    this.handlers = {};\n    this.session = {};\n    this.recognizers = [];\n    this.oldCssProps = {};\n\n    this.element = element;\n    this.input = createInputInstance(this);\n    this.touchAction = new TouchAction(this, this.options.touchAction);\n\n    toggleCssProps(this, true);\n\n    each(this.options.recognizers, function(item) {\n        var recognizer = this.add(new (item[0])(item[1]));\n        item[2] && recognizer.recognizeWith(item[2]);\n        item[3] && recognizer.requireFailure(item[3]);\n    }, this);\n}\n\nManager.prototype = {\n    /**\n     * set options\n     * @param {Object} options\n     * @returns {Manager}\n     */\n    set: function(options) {\n        assign(this.options, options);\n\n        // Options that need a little more setup\n        if (options.touchAction) {\n            this.touchAction.update();\n        }\n        if (options.inputTarget) {\n            // Clean up existing event listeners and reinitialize\n            this.input.destroy();\n            this.input.target = options.inputTarget;\n            this.input.init();\n        }\n        return this;\n    },\n\n    /**\n     * stop recognizing for this session.\n     * This session will be discarded, when a new [input]start event is fired.\n     * When forced, the recognizer cycle is stopped immediately.\n     * @param {Boolean} [force]\n     */\n    stop: function(force) {\n        this.session.stopped = force ? FORCED_STOP : STOP;\n    },\n\n    /**\n     * run the recognizers!\n     * called by the inputHandler function on every movement of the pointers (touches)\n     * it walks through all the recognizers and tries to detect the gesture that is being made\n     * @param {Object} inputData\n     */\n    recognize: function(inputData) {\n        var session = this.session;\n        if (session.stopped) {\n            return;\n        }\n\n        // run the touch-action polyfill\n        this.touchAction.preventDefaults(inputData);\n\n        var recognizer;\n        var recognizers = this.recognizers;\n\n        // this holds the recognizer that is being recognized.\n        // so the recognizer's state needs to be BEGAN, CHANGED, ENDED or RECOGNIZED\n        // if no recognizer is detecting a thing, it is set to `null`\n        var curRecognizer = session.curRecognizer;\n\n        // reset when the last recognizer is recognized\n        // or when we're in a new session\n        if (!curRecognizer || (curRecognizer && curRecognizer.state & STATE_RECOGNIZED)) {\n            curRecognizer = session.curRecognizer = null;\n        }\n\n        var i = 0;\n        while (i < recognizers.length) {\n            recognizer = recognizers[i];\n\n            // find out if we are allowed try to recognize the input for this one.\n            // 1.   allow if the session is NOT forced stopped (see the .stop() method)\n            // 2.   allow if we still haven't recognized a gesture in this session, or the this recognizer is the one\n            //      that is being recognized.\n            // 3.   allow if the recognizer is allowed to run simultaneous with the current recognized recognizer.\n            //      this can be setup with the `recognizeWith()` method on the recognizer.\n            if (session.stopped !== FORCED_STOP && ( // 1\n                    !curRecognizer || recognizer == curRecognizer || // 2\n                    recognizer.canRecognizeWith(curRecognizer))) { // 3\n                recognizer.recognize(inputData);\n            } else {\n                recognizer.reset();\n            }\n\n            // if the recognizer has been recognizing the input as a valid gesture, we want to store this one as the\n            // current active recognizer. but only if we don't already have an active recognizer\n            if (!curRecognizer && recognizer.state & (STATE_BEGAN | STATE_CHANGED | STATE_ENDED)) {\n                curRecognizer = session.curRecognizer = recognizer;\n            }\n            i++;\n        }\n    },\n\n    /**\n     * get a recognizer by its event name.\n     * @param {Recognizer|String} recognizer\n     * @returns {Recognizer|Null}\n     */\n    get: function(recognizer) {\n        if (recognizer instanceof Recognizer) {\n            return recognizer;\n        }\n\n        var recognizers = this.recognizers;\n        for (var i = 0; i < recognizers.length; i++) {\n            if (recognizers[i].options.event == recognizer) {\n                return recognizers[i];\n            }\n        }\n        return null;\n    },\n\n    /**\n     * add a recognizer to the manager\n     * existing recognizers with the same event name will be removed\n     * @param {Recognizer} recognizer\n     * @returns {Recognizer|Manager}\n     */\n    add: function(recognizer) {\n        if (invokeArrayArg(recognizer, 'add', this)) {\n            return this;\n        }\n\n        // remove existing\n        var existing = this.get(recognizer.options.event);\n        if (existing) {\n            this.remove(existing);\n        }\n\n        this.recognizers.push(recognizer);\n        recognizer.manager = this;\n\n        this.touchAction.update();\n        return recognizer;\n    },\n\n    /**\n     * remove a recognizer by name or instance\n     * @param {Recognizer|String} recognizer\n     * @returns {Manager}\n     */\n    remove: function(recognizer) {\n        if (invokeArrayArg(recognizer, 'remove', this)) {\n            return this;\n        }\n\n        recognizer = this.get(recognizer);\n\n        // let's make sure this recognizer exists\n        if (recognizer) {\n            var recognizers = this.recognizers;\n            var index = inArray(recognizers, recognizer);\n\n            if (index !== -1) {\n                recognizers.splice(index, 1);\n                this.touchAction.update();\n            }\n        }\n\n        return this;\n    },\n\n    /**\n     * bind event\n     * @param {String} events\n     * @param {Function} handler\n     * @returns {EventEmitter} this\n     */\n    on: function(events, handler) {\n        if (events === undefined) {\n            return;\n        }\n        if (handler === undefined) {\n            return;\n        }\n\n        var handlers = this.handlers;\n        each(splitStr(events), function(event) {\n            handlers[event] = handlers[event] || [];\n            handlers[event].push(handler);\n        });\n        return this;\n    },\n\n    /**\n     * unbind event, leave emit blank to remove all handlers\n     * @param {String} events\n     * @param {Function} [handler]\n     * @returns {EventEmitter} this\n     */\n    off: function(events, handler) {\n        if (events === undefined) {\n            return;\n        }\n\n        var handlers = this.handlers;\n        each(splitStr(events), function(event) {\n            if (!handler) {\n                delete handlers[event];\n            } else {\n                handlers[event] && handlers[event].splice(inArray(handlers[event], handler), 1);\n            }\n        });\n        return this;\n    },\n\n    /**\n     * emit event to the listeners\n     * @param {String} event\n     * @param {Object} data\n     */\n    emit: function(event, data) {\n        // we also want to trigger dom events\n        if (this.options.domEvents) {\n            triggerDomEvent(event, data);\n        }\n\n        // no handlers, so skip it all\n        var handlers = this.handlers[event] && this.handlers[event].slice();\n        if (!handlers || !handlers.length) {\n            return;\n        }\n\n        data.type = event;\n        data.preventDefault = function() {\n            data.srcEvent.preventDefault();\n        };\n\n        var i = 0;\n        while (i < handlers.length) {\n            handlers[i](data);\n            i++;\n        }\n    },\n\n    /**\n     * destroy the manager and unbinds all events\n     * it doesn't unbind dom events, that is the user own responsibility\n     */\n    destroy: function() {\n        this.element && toggleCssProps(this, false);\n\n        this.handlers = {};\n        this.session = {};\n        this.input.destroy();\n        this.element = null;\n    }\n};\n\n/**\n * add/remove the css properties as defined in manager.options.cssProps\n * @param {Manager} manager\n * @param {Boolean} add\n */\nfunction toggleCssProps(manager, add) {\n    var element = manager.element;\n    if (!element.style) {\n        return;\n    }\n    var prop;\n    each(manager.options.cssProps, function(value, name) {\n        prop = prefixed(element.style, name);\n        if (add) {\n            manager.oldCssProps[prop] = element.style[prop];\n            element.style[prop] = value;\n        } else {\n            element.style[prop] = manager.oldCssProps[prop] || '';\n        }\n    });\n    if (!add) {\n        manager.oldCssProps = {};\n    }\n}\n\n/**\n * trigger dom event\n * @param {String} event\n * @param {Object} data\n */\nfunction triggerDomEvent(event, data) {\n    var gestureEvent = document.createEvent('Event');\n    gestureEvent.initEvent(event, true, true);\n    gestureEvent.gesture = data;\n    data.target.dispatchEvent(gestureEvent);\n}\n\nassign(Hammer, {\n    INPUT_START: INPUT_START,\n    INPUT_MOVE: INPUT_MOVE,\n    INPUT_END: INPUT_END,\n    INPUT_CANCEL: INPUT_CANCEL,\n\n    STATE_POSSIBLE: STATE_POSSIBLE,\n    STATE_BEGAN: STATE_BEGAN,\n    STATE_CHANGED: STATE_CHANGED,\n    STATE_ENDED: STATE_ENDED,\n    STATE_RECOGNIZED: STATE_RECOGNIZED,\n    STATE_CANCELLED: STATE_CANCELLED,\n    STATE_FAILED: STATE_FAILED,\n\n    DIRECTION_NONE: DIRECTION_NONE,\n    DIRECTION_LEFT: DIRECTION_LEFT,\n    DIRECTION_RIGHT: DIRECTION_RIGHT,\n    DIRECTION_UP: DIRECTION_UP,\n    DIRECTION_DOWN: DIRECTION_DOWN,\n    DIRECTION_HORIZONTAL: DIRECTION_HORIZONTAL,\n    DIRECTION_VERTICAL: DIRECTION_VERTICAL,\n    DIRECTION_ALL: DIRECTION_ALL,\n\n    Manager: Manager,\n    Input: Input,\n    TouchAction: TouchAction,\n\n    TouchInput: TouchInput,\n    MouseInput: MouseInput,\n    PointerEventInput: PointerEventInput,\n    TouchMouseInput: TouchMouseInput,\n    SingleTouchInput: SingleTouchInput,\n\n    Recognizer: Recognizer,\n    AttrRecognizer: AttrRecognizer,\n    Tap: TapRecognizer,\n    Pan: PanRecognizer,\n    Swipe: SwipeRecognizer,\n    Pinch: PinchRecognizer,\n    Rotate: RotateRecognizer,\n    Press: PressRecognizer,\n\n    on: addEventListeners,\n    off: removeEventListeners,\n    each: each,\n    merge: merge,\n    extend: extend,\n    assign: assign,\n    inherit: inherit,\n    bindFn: bindFn,\n    prefixed: prefixed\n});\n\n// this prevents errors when Hammer is loaded in the presence of an AMD\n//  style loader but by script tag, not by the loader.\nvar freeGlobal = (typeof window !== 'undefined' ? window : (typeof self !== 'undefined' ? self : {})); // jshint ignore:line\nfreeGlobal.Hammer = Hammer;\n\nif (typeof define === 'function' && define.amd) {\n    define(function() {\n        return Hammer;\n    });\n} else if (typeof module != 'undefined' && module.exports) {\n    module.exports = Hammer;\n} else {\n    window[exportName] = Hammer;\n}\n\n})(window, document, 'Hammer');\n",
         "'use strict';\n\nvar reactIs = require('react-is');\n\n/**\n * Copyright 2015, Yahoo! Inc.\n * Copyrights licensed under the New BSD License. See the accompanying LICENSE file for terms.\n */\nvar REACT_STATICS = {\n  childContextTypes: true,\n  contextType: true,\n  contextTypes: true,\n  defaultProps: true,\n  displayName: true,\n  getDefaultProps: true,\n  getDerivedStateFromError: true,\n  getDerivedStateFromProps: true,\n  mixins: true,\n  propTypes: true,\n  type: true\n};\nvar KNOWN_STATICS = {\n  name: true,\n  length: true,\n  prototype: true,\n  caller: true,\n  callee: true,\n  arguments: true,\n  arity: true\n};\nvar FORWARD_REF_STATICS = {\n  '$$typeof': true,\n  render: true,\n  defaultProps: true,\n  displayName: true,\n  propTypes: true\n};\nvar MEMO_STATICS = {\n  '$$typeof': true,\n  compare: true,\n  defaultProps: true,\n  displayName: true,\n  propTypes: true,\n  type: true\n};\nvar TYPE_STATICS = {};\nTYPE_STATICS[reactIs.ForwardRef] = FORWARD_REF_STATICS;\nTYPE_STATICS[reactIs.Memo] = MEMO_STATICS;\n\nfunction getStatics(component) {\n  // React v16.11 and below\n  if (reactIs.isMemo(component)) {\n    return MEMO_STATICS;\n  } // React v16.12 and above\n\n\n  return TYPE_STATICS[component['$$typeof']] || REACT_STATICS;\n}\n\nvar defineProperty = Object.defineProperty;\nvar getOwnPropertyNames = Object.getOwnPropertyNames;\nvar getOwnPropertySymbols = Object.getOwnPropertySymbols;\nvar getOwnPropertyDescriptor = Object.getOwnPropertyDescriptor;\nvar getPrototypeOf = Object.getPrototypeOf;\nvar objectPrototype = Object.prototype;\nfunction hoistNonReactStatics(targetComponent, sourceComponent, blacklist) {\n  if (typeof sourceComponent !== 'string') {\n    // don't hoist over string (html) components\n    if (objectPrototype) {\n      var inheritedComponent = getPrototypeOf(sourceComponent);\n\n      if (inheritedComponent && inheritedComponent !== objectPrototype) {\n        hoistNonReactStatics(targetComponent, inheritedComponent, blacklist);\n      }\n    }\n\n    var keys = getOwnPropertyNames(sourceComponent);\n\n    if (getOwnPropertySymbols) {\n      keys = keys.concat(getOwnPropertySymbols(sourceComponent));\n    }\n\n    var targetStatics = getStatics(targetComponent);\n    var sourceStatics = getStatics(sourceComponent);\n\n    for (var i = 0; i < keys.length; ++i) {\n      var key = keys[i];\n\n      if (!KNOWN_STATICS[key] && !(blacklist && blacklist[key]) && !(sourceStatics && sourceStatics[key]) && !(targetStatics && targetStatics[key])) {\n        var descriptor = getOwnPropertyDescriptor(sourceComponent, key);\n\n        try {\n          // Avoid failures from read-only properties\n          defineProperty(targetComponent, key, descriptor);\n        } catch (e) {}\n      }\n    }\n  }\n\n  return targetComponent;\n}\n\nmodule.exports = hoistNonReactStatics;\n",
         "/*\nobject-assign\n(c) Sindre Sorhus\n@license MIT\n*/\n\n'use strict';\n/* eslint-disable no-unused-vars */\nvar getOwnPropertySymbols = Object.getOwnPropertySymbols;\nvar hasOwnProperty = Object.prototype.hasOwnProperty;\nvar propIsEnumerable = Object.prototype.propertyIsEnumerable;\n\nfunction toObject(val) {\n\tif (val === null || val === undefined) {\n\t\tthrow new TypeError('Object.assign cannot be called with null or undefined');\n\t}\n\n\treturn Object(val);\n}\n\nfunction shouldUseNative() {\n\ttry {\n\t\tif (!Object.assign) {\n\t\t\treturn false;\n\t\t}\n\n\t\t// Detect buggy property enumeration order in older V8 versions.\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=4118\n\t\tvar test1 = new String('abc');  // eslint-disable-line no-new-wrappers\n\t\ttest1[5] = 'de';\n\t\tif (Object.getOwnPropertyNames(test1)[0] === '5') {\n\t\t\treturn false;\n\t\t}\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=3056\n\t\tvar test2 = {};\n\t\tfor (var i = 0; i < 10; i++) {\n\t\t\ttest2['_' + String.fromCharCode(i)] = i;\n\t\t}\n\t\tvar order2 = Object.getOwnPropertyNames(test2).map(function (n) {\n\t\t\treturn test2[n];\n\t\t});\n\t\tif (order2.join('') !== '0123456789') {\n\t\t\treturn false;\n\t\t}\n\n\t\t// https://bugs.chromium.org/p/v8/issues/detail?id=3056\n\t\tvar test3 = {};\n\t\t'abcdefghijklmnopqrst'.split('').forEach(function (letter) {\n\t\t\ttest3[letter] = letter;\n\t\t});\n\t\tif (Object.keys(Object.assign({}, test3)).join('') !==\n\t\t\t\t'abcdefghijklmnopqrst') {\n\t\t\treturn false;\n\t\t}\n\n\t\treturn true;\n\t} catch (err) {\n\t\t// We don't expect any of the above to throw, but better to be safe.\n\t\treturn false;\n\t}\n}\n\nmodule.exports = shouldUseNative() ? Object.assign : function (target, source) {\n\tvar from;\n\tvar to = toObject(target);\n\tvar symbols;\n\n\tfor (var s = 1; s < arguments.length; s++) {\n\t\tfrom = Object(arguments[s]);\n\n\t\tfor (var key in from) {\n\t\t\tif (hasOwnProperty.call(from, key)) {\n\t\t\t\tto[key] = from[key];\n\t\t\t}\n\t\t}\n\n\t\tif (getOwnPropertySymbols) {\n\t\t\tsymbols = getOwnPropertySymbols(from);\n\t\t\tfor (var i = 0; i < symbols.length; i++) {\n\t\t\t\tif (propIsEnumerable.call(from, symbols[i])) {\n\t\t\t\t\tto[symbols[i]] = from[symbols[i]];\n\t\t\t\t}\n\t\t\t}\n\t\t}\n\t}\n\n\treturn to;\n};\n",
@@ -6540,15 +6547,18 @@
         "import { utils } from \"./utils.js\";\n\n/**\n * Poly Bezier\n * @param {[type]} curves [description]\n */\nclass PolyBezier {\n  constructor(curves) {\n    this.curves = [];\n    this._3d = false;\n    if (!!curves) {\n      this.curves = curves;\n      this._3d = this.curves[0]._3d;\n    }\n  }\n\n  valueOf() {\n    return this.toString();\n  }\n\n  toString() {\n    return (\n      \"[\" +\n      this.curves\n        .map(function (curve) {\n          return utils.pointsToString(curve.points);\n        })\n        .join(\", \") +\n      \"]\"\n    );\n  }\n\n  addCurve(curve) {\n    this.curves.push(curve);\n    this._3d = this._3d || curve._3d;\n  }\n\n  length() {\n    return this.curves\n      .map(function (v) {\n        return v.length();\n      })\n      .reduce(function (a, b) {\n        return a + b;\n      });\n  }\n\n  curve(idx) {\n    return this.curves[idx];\n  }\n\n  bbox() {\n    const c = this.curves;\n    var bbox = c[0].bbox();\n    for (var i = 1; i < c.length; i++) {\n      utils.expandbox(bbox, c[i].bbox());\n    }\n    return bbox;\n  }\n\n  offset(d) {\n    const offset = [];\n    this.curves.forEach(function (v) {\n      offset.push(...v.offset(d));\n    });\n    return new PolyBezier(offset);\n  }\n}\n\nexport { PolyBezier };\n",
         "/**\n  A javascript Bezier curve library by Pomax.\n\n  Based on http://pomax.github.io/bezierinfo\n\n  This code is MIT licensed.\n**/\n\nimport { utils } from \"./utils.js\";\nimport { PolyBezier } from \"./poly-bezier.js\";\n\n// math-inlining.\nconst { abs, min, max, cos, sin, acos, sqrt } = Math;\nconst pi = Math.PI;\n// a zero coordinate, which is surprisingly useful\nconst ZERO = { x: 0, y: 0, z: 0 };\n\n/**\n * Bezier curve constructor.\n *\n * ...docs pending...\n */\nclass Bezier {\n  constructor(coords) {\n    let args =\n      coords && coords.forEach ? coords : Array.from(arguments).slice();\n    let coordlen = false;\n\n    if (typeof args[0] === \"object\") {\n      coordlen = args.length;\n      const newargs = [];\n      args.forEach(function (point) {\n        [\"x\", \"y\", \"z\"].forEach(function (d) {\n          if (typeof point[d] !== \"undefined\") {\n            newargs.push(point[d]);\n          }\n        });\n      });\n      args = newargs;\n    }\n\n    let higher = false;\n    const len = args.length;\n\n    if (coordlen) {\n      if (coordlen > 4) {\n        if (arguments.length !== 1) {\n          throw new Error(\n            \"Only new Bezier(point[]) is accepted for 4th and higher order curves\"\n          );\n        }\n        higher = true;\n      }\n    } else {\n      if (len !== 6 && len !== 8 && len !== 9 && len !== 12) {\n        if (arguments.length !== 1) {\n          throw new Error(\n            \"Only new Bezier(point[]) is accepted for 4th and higher order curves\"\n          );\n        }\n      }\n    }\n\n    const _3d = (this._3d =\n      (!higher && (len === 9 || len === 12)) ||\n      (coords && coords[0] && typeof coords[0].z !== \"undefined\"));\n\n    const points = (this.points = []);\n    for (let idx = 0, step = _3d ? 3 : 2; idx < len; idx += step) {\n      var point = {\n        x: args[idx],\n        y: args[idx + 1],\n      };\n      if (_3d) {\n        point.z = args[idx + 2];\n      }\n      points.push(point);\n    }\n    const order = (this.order = points.length - 1);\n\n    const dims = (this.dims = [\"x\", \"y\"]);\n    if (_3d) dims.push(\"z\");\n    this.dimlen = dims.length;\n\n    // is this curve, practically speaking, a straight line?\n    const aligned = utils.align(points, { p1: points[0], p2: points[order] });\n    const baselength = utils.dist(points[0], points[order]);\n    this._linear = aligned.reduce((t, p) => t + abs(p.y), 0) < baselength / 50;\n\n    this._lut = [];\n    this._t1 = 0;\n    this._t2 = 1;\n    this.update();\n  }\n\n  static quadraticFromPoints(p1, p2, p3, t) {\n    if (typeof t === \"undefined\") {\n      t = 0.5;\n    }\n    // shortcuts, although they're really dumb\n    if (t === 0) {\n      return new Bezier(p2, p2, p3);\n    }\n    if (t === 1) {\n      return new Bezier(p1, p2, p2);\n    }\n    // real fitting.\n    const abc = Bezier.getABC(2, p1, p2, p3, t);\n    return new Bezier(p1, abc.A, p3);\n  }\n\n  static cubicFromPoints(S, B, E, t, d1) {\n    if (typeof t === \"undefined\") {\n      t = 0.5;\n    }\n    const abc = Bezier.getABC(3, S, B, E, t);\n    if (typeof d1 === \"undefined\") {\n      d1 = utils.dist(B, abc.C);\n    }\n    const d2 = (d1 * (1 - t)) / t;\n\n    const selen = utils.dist(S, E),\n      lx = (E.x - S.x) / selen,\n      ly = (E.y - S.y) / selen,\n      bx1 = d1 * lx,\n      by1 = d1 * ly,\n      bx2 = d2 * lx,\n      by2 = d2 * ly;\n    // derivation of new hull coordinates\n    const e1 = { x: B.x - bx1, y: B.y - by1 },\n      e2 = { x: B.x + bx2, y: B.y + by2 },\n      A = abc.A,\n      v1 = { x: A.x + (e1.x - A.x) / (1 - t), y: A.y + (e1.y - A.y) / (1 - t) },\n      v2 = { x: A.x + (e2.x - A.x) / t, y: A.y + (e2.y - A.y) / t },\n      nc1 = { x: S.x + (v1.x - S.x) / t, y: S.y + (v1.y - S.y) / t },\n      nc2 = {\n        x: E.x + (v2.x - E.x) / (1 - t),\n        y: E.y + (v2.y - E.y) / (1 - t),\n      };\n    // ...done\n    return new Bezier(S, nc1, nc2, E);\n  }\n\n  static getUtils() {\n    return utils;\n  }\n\n  getUtils() {\n    return Bezier.getUtils();\n  }\n\n  static get PolyBezier() {\n    return PolyBezier;\n  }\n\n  valueOf() {\n    return this.toString();\n  }\n\n  toString() {\n    return utils.pointsToString(this.points);\n  }\n\n  toSVG() {\n    if (this._3d) return false;\n    const p = this.points,\n      x = p[0].x,\n      y = p[0].y,\n      s = [\"M\", x, y, this.order === 2 ? \"Q\" : \"C\"];\n    for (let i = 1, last = p.length; i < last; i++) {\n      s.push(p[i].x);\n      s.push(p[i].y);\n    }\n    return s.join(\" \");\n  }\n\n  setRatios(ratios) {\n    if (ratios.length !== this.points.length) {\n      throw new Error(\"incorrect number of ratio values\");\n    }\n    this.ratios = ratios;\n    this._lut = []; //  invalidate any precomputed LUT\n  }\n\n  verify() {\n    const print = this.coordDigest();\n    if (print !== this._print) {\n      this._print = print;\n      this.update();\n    }\n  }\n\n  coordDigest() {\n    return this.points\n      .map(function (c, pos) {\n        return \"\" + pos + c.x + c.y + (c.z ? c.z : 0);\n      })\n      .join(\"\");\n  }\n\n  update() {\n    // invalidate any precomputed LUT\n    this._lut = [];\n    this.dpoints = utils.derive(this.points, this._3d);\n    this.computedirection();\n  }\n\n  computedirection() {\n    const points = this.points;\n    const angle = utils.angle(points[0], points[this.order], points[1]);\n    this.clockwise = angle > 0;\n  }\n\n  length() {\n    return utils.length(this.derivative.bind(this));\n  }\n\n  static getABC(order = 2, S, B, E, t = 0.5) {\n    const u = utils.projectionratio(t, order),\n      um = 1 - u,\n      C = {\n        x: u * S.x + um * E.x,\n        y: u * S.y + um * E.y,\n      },\n      s = utils.abcratio(t, order),\n      A = {\n        x: B.x + (B.x - C.x) / s,\n        y: B.y + (B.y - C.y) / s,\n      };\n    return { A, B, C, S, E };\n  }\n\n  getABC(t, B) {\n    B = B || this.get(t);\n    let S = this.points[0];\n    let E = this.points[this.order];\n    return Bezier.getABC(this.order, S, B, E, t);\n  }\n\n  getLUT(steps) {\n    this.verify();\n    steps = steps || 100;\n    if (this._lut.length === steps + 1) {\n      return this._lut;\n    }\n    this._lut = [];\n    // n steps means n+1 points\n    steps++;\n    this._lut = [];\n    for (let i = 0, p, t; i < steps; i++) {\n      t = i / (steps - 1);\n      p = this.compute(t);\n      p.t = t;\n      this._lut.push(p);\n    }\n    return this._lut;\n  }\n\n  on(point, error) {\n    error = error || 5;\n    const lut = this.getLUT(),\n      hits = [];\n    for (let i = 0, c, t = 0; i < lut.length; i++) {\n      c = lut[i];\n      if (utils.dist(c, point) < error) {\n        hits.push(c);\n        t += i / lut.length;\n      }\n    }\n    if (!hits.length) return false;\n    return (t /= hits.length);\n  }\n\n  project(point) {\n    // step 1: coarse check\n    const LUT = this.getLUT(),\n      l = LUT.length - 1,\n      closest = utils.closest(LUT, point),\n      mpos = closest.mpos,\n      t1 = (mpos - 1) / l,\n      t2 = (mpos + 1) / l,\n      step = 0.1 / l;\n\n    // step 2: fine check\n    let mdist = closest.mdist,\n      t = t1,\n      ft = t,\n      p;\n    mdist += 1;\n    for (let d; t < t2 + step; t += step) {\n      p = this.compute(t);\n      d = utils.dist(point, p);\n      if (d < mdist) {\n        mdist = d;\n        ft = t;\n      }\n    }\n    ft = ft < 0 ? 0 : ft > 1 ? 1 : ft;\n    p = this.compute(ft);\n    p.t = ft;\n    p.d = mdist;\n    return p;\n  }\n\n  get(t) {\n    return this.compute(t);\n  }\n\n  point(idx) {\n    return this.points[idx];\n  }\n\n  compute(t) {\n    if (this.ratios) {\n      return utils.computeWithRatios(t, this.points, this.ratios, this._3d);\n    }\n    return utils.compute(t, this.points, this._3d, this.ratios);\n  }\n\n  raise() {\n    const p = this.points,\n      np = [p[0]],\n      k = p.length;\n    for (let i = 1, pi, pim; i < k; i++) {\n      pi = p[i];\n      pim = p[i - 1];\n      np[i] = {\n        x: ((k - i) / k) * pi.x + (i / k) * pim.x,\n        y: ((k - i) / k) * pi.y + (i / k) * pim.y,\n      };\n    }\n    np[k] = p[k - 1];\n    return new Bezier(np);\n  }\n\n  derivative(t) {\n    return utils.compute(t, this.dpoints[0], this._3d);\n  }\n\n  dderivative(t) {\n    return utils.compute(t, this.dpoints[1], this._3d);\n  }\n\n  align() {\n    let p = this.points;\n    return new Bezier(utils.align(p, { p1: p[0], p2: p[p.length - 1] }));\n  }\n\n  curvature(t) {\n    return utils.curvature(t, this.dpoints[0], this.dpoints[1], this._3d);\n  }\n\n  inflections() {\n    return utils.inflections(this.points);\n  }\n\n  normal(t) {\n    return this._3d ? this.__normal3(t) : this.__normal2(t);\n  }\n\n  __normal2(t) {\n    const d = this.derivative(t);\n    const q = sqrt(d.x * d.x + d.y * d.y);\n    return { t, x: -d.y / q, y: d.x / q };\n  }\n\n  __normal3(t) {\n    // see http://stackoverflow.com/questions/25453159\n    const r1 = this.derivative(t),\n      r2 = this.derivative(t + 0.01),\n      q1 = sqrt(r1.x * r1.x + r1.y * r1.y + r1.z * r1.z),\n      q2 = sqrt(r2.x * r2.x + r2.y * r2.y + r2.z * r2.z);\n    r1.x /= q1;\n    r1.y /= q1;\n    r1.z /= q1;\n    r2.x /= q2;\n    r2.y /= q2;\n    r2.z /= q2;\n    // cross product\n    const c = {\n      x: r2.y * r1.z - r2.z * r1.y,\n      y: r2.z * r1.x - r2.x * r1.z,\n      z: r2.x * r1.y - r2.y * r1.x,\n    };\n    const m = sqrt(c.x * c.x + c.y * c.y + c.z * c.z);\n    c.x /= m;\n    c.y /= m;\n    c.z /= m;\n    // rotation matrix\n    const R = [\n      c.x * c.x,\n      c.x * c.y - c.z,\n      c.x * c.z + c.y,\n      c.x * c.y + c.z,\n      c.y * c.y,\n      c.y * c.z - c.x,\n      c.x * c.z - c.y,\n      c.y * c.z + c.x,\n      c.z * c.z,\n    ];\n    // normal vector:\n    const n = {\n      t,\n      x: R[0] * r1.x + R[1] * r1.y + R[2] * r1.z,\n      y: R[3] * r1.x + R[4] * r1.y + R[5] * r1.z,\n      z: R[6] * r1.x + R[7] * r1.y + R[8] * r1.z,\n    };\n    return n;\n  }\n\n  hull(t) {\n    let p = this.points,\n      _p = [],\n      q = [],\n      idx = 0;\n    q[idx++] = p[0];\n    q[idx++] = p[1];\n    q[idx++] = p[2];\n    if (this.order === 3) {\n      q[idx++] = p[3];\n    }\n    // we lerp between all points at each iteration, until we have 1 point left.\n    while (p.length > 1) {\n      _p = [];\n      for (let i = 0, pt, l = p.length - 1; i < l; i++) {\n        pt = utils.lerp(t, p[i], p[i + 1]);\n        q[idx++] = pt;\n        _p.push(pt);\n      }\n      p = _p;\n    }\n    return q;\n  }\n\n  split(t1, t2) {\n    // shortcuts\n    if (t1 === 0 && !!t2) {\n      return this.split(t2).left;\n    }\n    if (t2 === 1) {\n      return this.split(t1).right;\n    }\n\n    // no shortcut: use \"de Casteljau\" iteration.\n    const q = this.hull(t1);\n    const result = {\n      left:\n        this.order === 2\n          ? new Bezier([q[0], q[3], q[5]])\n          : new Bezier([q[0], q[4], q[7], q[9]]),\n      right:\n        this.order === 2\n          ? new Bezier([q[5], q[4], q[2]])\n          : new Bezier([q[9], q[8], q[6], q[3]]),\n      span: q,\n    };\n\n    // make sure we bind _t1/_t2 information!\n    result.left._t1 = utils.map(0, 0, 1, this._t1, this._t2);\n    result.left._t2 = utils.map(t1, 0, 1, this._t1, this._t2);\n    result.right._t1 = utils.map(t1, 0, 1, this._t1, this._t2);\n    result.right._t2 = utils.map(1, 0, 1, this._t1, this._t2);\n\n    // if we have no t2, we're done\n    if (!t2) {\n      return result;\n    }\n\n    // if we have a t2, split again:\n    t2 = utils.map(t2, t1, 1, 0, 1);\n    return result.right.split(t2).left;\n  }\n\n  extrema() {\n    const result = {};\n    let roots = [];\n\n    this.dims.forEach(\n      function (dim) {\n        let mfn = function (v) {\n          return v[dim];\n        };\n        let p = this.dpoints[0].map(mfn);\n        result[dim] = utils.droots(p);\n        if (this.order === 3) {\n          p = this.dpoints[1].map(mfn);\n          result[dim] = result[dim].concat(utils.droots(p));\n        }\n        result[dim] = result[dim].filter(function (t) {\n          return t >= 0 && t <= 1;\n        });\n        roots = roots.concat(result[dim].sort(utils.numberSort));\n      }.bind(this)\n    );\n\n    result.values = roots.sort(utils.numberSort).filter(function (v, idx) {\n      return roots.indexOf(v) === idx;\n    });\n\n    return result;\n  }\n\n  bbox() {\n    const extrema = this.extrema(),\n      result = {};\n    this.dims.forEach(\n      function (d) {\n        result[d] = utils.getminmax(this, d, extrema[d]);\n      }.bind(this)\n    );\n    return result;\n  }\n\n  overlaps(curve) {\n    const lbbox = this.bbox(),\n      tbbox = curve.bbox();\n    return utils.bboxoverlap(lbbox, tbbox);\n  }\n\n  offset(t, d) {\n    if (typeof d !== \"undefined\") {\n      const c = this.get(t),\n        n = this.normal(t);\n      const ret = {\n        c: c,\n        n: n,\n        x: c.x + n.x * d,\n        y: c.y + n.y * d,\n      };\n      if (this._3d) {\n        ret.z = c.z + n.z * d;\n      }\n      return ret;\n    }\n    if (this._linear) {\n      const nv = this.normal(0),\n        coords = this.points.map(function (p) {\n          const ret = {\n            x: p.x + t * nv.x,\n            y: p.y + t * nv.y,\n          };\n          if (p.z && nv.z) {\n            ret.z = p.z + t * nv.z;\n          }\n          return ret;\n        });\n      return [new Bezier(coords)];\n    }\n    return this.reduce().map(function (s) {\n      if (s._linear) {\n        return s.offset(t)[0];\n      }\n      return s.scale(t);\n    });\n  }\n\n  simple() {\n    if (this.order === 3) {\n      const a1 = utils.angle(this.points[0], this.points[3], this.points[1]);\n      const a2 = utils.angle(this.points[0], this.points[3], this.points[2]);\n      if ((a1 > 0 && a2 < 0) || (a1 < 0 && a2 > 0)) return false;\n    }\n    const n1 = this.normal(0);\n    const n2 = this.normal(1);\n    let s = n1.x * n2.x + n1.y * n2.y;\n    if (this._3d) {\n      s += n1.z * n2.z;\n    }\n    return abs(acos(s)) < pi / 3;\n  }\n\n  reduce() {\n    // TODO: examine these var types in more detail...\n    let i,\n      t1 = 0,\n      t2 = 0,\n      step = 0.01,\n      segment,\n      pass1 = [],\n      pass2 = [];\n    // first pass: split on extrema\n    let extrema = this.extrema().values;\n    if (extrema.indexOf(0) === -1) {\n      extrema = [0].concat(extrema);\n    }\n    if (extrema.indexOf(1) === -1) {\n      extrema.push(1);\n    }\n\n    for (t1 = extrema[0], i = 1; i < extrema.length; i++) {\n      t2 = extrema[i];\n      segment = this.split(t1, t2);\n      segment._t1 = t1;\n      segment._t2 = t2;\n      pass1.push(segment);\n      t1 = t2;\n    }\n\n    // second pass: further reduce these segments to simple segments\n    pass1.forEach(function (p1) {\n      t1 = 0;\n      t2 = 0;\n      while (t2 <= 1) {\n        for (t2 = t1 + step; t2 <= 1 + step; t2 += step) {\n          segment = p1.split(t1, t2);\n          if (!segment.simple()) {\n            t2 -= step;\n            if (abs(t1 - t2) < step) {\n              // we can never form a reduction\n              return [];\n            }\n            segment = p1.split(t1, t2);\n            segment._t1 = utils.map(t1, 0, 1, p1._t1, p1._t2);\n            segment._t2 = utils.map(t2, 0, 1, p1._t1, p1._t2);\n            pass2.push(segment);\n            t1 = t2;\n            break;\n          }\n        }\n      }\n      if (t1 < 1) {\n        segment = p1.split(t1, 1);\n        segment._t1 = utils.map(t1, 0, 1, p1._t1, p1._t2);\n        segment._t2 = p1._t2;\n        pass2.push(segment);\n      }\n    });\n    return pass2;\n  }\n\n  translate(v, d1, d2) {\n    d2 = typeof d2 === \"number\" ? d2 : d1;\n\n    // TODO: make this take curves with control points outside\n    //       of the start-end interval into account\n\n    const o = this.order;\n    let d = this.points.map((_, i) => (1 - i / o) * d1 + (i / o) * d2);\n    return new Bezier(\n      this.points.map((p, i) => ({\n        x: p.x + v.x * d[i],\n        y: p.y + v.y * d[i],\n      }))\n    );\n  }\n\n  scale(d) {\n    const order = this.order;\n    let distanceFn = false;\n    if (typeof d === \"function\") {\n      distanceFn = d;\n    }\n    if (distanceFn && order === 2) {\n      return this.raise().scale(distanceFn);\n    }\n\n    // TODO: add special handling for non-linear degenerate curves.\n\n    const clockwise = this.clockwise;\n    const points = this.points;\n\n    if (this._linear) {\n      return this.translate(\n        this.normal(0),\n        distanceFn ? distanceFn(0) : d,\n        distanceFn ? distanceFn(1) : d\n      );\n    }\n\n    const r1 = distanceFn ? distanceFn(0) : d;\n    const r2 = distanceFn ? distanceFn(1) : d;\n    const v = [this.offset(0, 10), this.offset(1, 10)];\n    const np = [];\n    const o = utils.lli4(v[0], v[0].c, v[1], v[1].c);\n\n    if (!o) {\n      throw new Error(\"cannot scale this curve. Try reducing it first.\");\n    }\n\n    // move all points by distance 'd' wrt the origin 'o',\n    // and move end points by fixed distance along normal.\n    [0, 1].forEach(function (t) {\n      const p = (np[t * order] = utils.copy(points[t * order]));\n      p.x += (t ? r2 : r1) * v[t].n.x;\n      p.y += (t ? r2 : r1) * v[t].n.y;\n    });\n\n    if (!distanceFn) {\n      // move control points to lie on the intersection of the offset\n      // derivative vector, and the origin-through-control vector\n      [0, 1].forEach((t) => {\n        if (order === 2 && !!t) return;\n        const p = np[t * order];\n        const d = this.derivative(t);\n        const p2 = { x: p.x + d.x, y: p.y + d.y };\n        np[t + 1] = utils.lli4(p, p2, o, points[t + 1]);\n      });\n      return new Bezier(np);\n    }\n\n    // move control points by \"however much necessary to\n    // ensure the correct tangent to endpoint\".\n    [0, 1].forEach(function (t) {\n      if (order === 2 && !!t) return;\n      var p = points[t + 1];\n      var ov = {\n        x: p.x - o.x,\n        y: p.y - o.y,\n      };\n      var rc = distanceFn ? distanceFn((t + 1) / order) : d;\n      if (distanceFn && !clockwise) rc = -rc;\n      var m = sqrt(ov.x * ov.x + ov.y * ov.y);\n      ov.x /= m;\n      ov.y /= m;\n      np[t + 1] = {\n        x: p.x + rc * ov.x,\n        y: p.y + rc * ov.y,\n      };\n    });\n    return new Bezier(np);\n  }\n\n  outline(d1, d2, d3, d4) {\n    d2 = d2 === undefined ? d1 : d2;\n\n    if (this._linear) {\n      // TODO: find the actual extrema, because they might\n      //       be before the start, or past the end.\n\n      const n = this.normal(0);\n      const start = this.points[0];\n      const end = this.points[this.points.length - 1];\n      let s, mid, e;\n\n      if (d3 === undefined) {\n        d3 = d1;\n        d4 = d2;\n      }\n\n      s = { x: start.x + n.x * d1, y: start.y + n.y * d1 };\n      e = { x: end.x + n.x * d3, y: end.y + n.y * d3 };\n      mid = { x: (s.x + e.x) / 2, y: (s.y + e.y) / 2 };\n      const fline = [s, mid, e];\n\n      s = { x: start.x - n.x * d2, y: start.y - n.y * d2 };\n      e = { x: end.x - n.x * d4, y: end.y - n.y * d4 };\n      mid = { x: (s.x + e.x) / 2, y: (s.y + e.y) / 2 };\n      const bline = [e, mid, s];\n\n      const ls = utils.makeline(bline[2], fline[0]);\n      const le = utils.makeline(fline[2], bline[0]);\n      const segments = [ls, new Bezier(fline), le, new Bezier(bline)];\n      return new PolyBezier(segments);\n    }\n\n    const reduced = this.reduce(),\n      len = reduced.length,\n      fcurves = [];\n\n    let bcurves = [],\n      p,\n      alen = 0,\n      tlen = this.length();\n\n    const graduated = typeof d3 !== \"undefined\" && typeof d4 !== \"undefined\";\n\n    function linearDistanceFunction(s, e, tlen, alen, slen) {\n      return function (v) {\n        const f1 = alen / tlen,\n          f2 = (alen + slen) / tlen,\n          d = e - s;\n        return utils.map(v, 0, 1, s + f1 * d, s + f2 * d);\n      };\n    }\n\n    // form curve oulines\n    reduced.forEach(function (segment) {\n      const slen = segment.length();\n      if (graduated) {\n        fcurves.push(\n          segment.scale(linearDistanceFunction(d1, d3, tlen, alen, slen))\n        );\n        bcurves.push(\n          segment.scale(linearDistanceFunction(-d2, -d4, tlen, alen, slen))\n        );\n      } else {\n        fcurves.push(segment.scale(d1));\n        bcurves.push(segment.scale(-d2));\n      }\n      alen += slen;\n    });\n\n    // reverse the \"return\" outline\n    bcurves = bcurves\n      .map(function (s) {\n        p = s.points;\n        if (p[3]) {\n          s.points = [p[3], p[2], p[1], p[0]];\n        } else {\n          s.points = [p[2], p[1], p[0]];\n        }\n        return s;\n      })\n      .reverse();\n\n    // form the endcaps as lines\n    const fs = fcurves[0].points[0],\n      fe = fcurves[len - 1].points[fcurves[len - 1].points.length - 1],\n      bs = bcurves[len - 1].points[bcurves[len - 1].points.length - 1],\n      be = bcurves[0].points[0],\n      ls = utils.makeline(bs, fs),\n      le = utils.makeline(fe, be),\n      segments = [ls].concat(fcurves).concat([le]).concat(bcurves);\n\n    return new PolyBezier(segments);\n  }\n\n  outlineshapes(d1, d2, curveIntersectionThreshold) {\n    d2 = d2 || d1;\n    const outline = this.outline(d1, d2).curves;\n    const shapes = [];\n    for (let i = 1, len = outline.length; i < len / 2; i++) {\n      const shape = utils.makeshape(\n        outline[i],\n        outline[len - i],\n        curveIntersectionThreshold\n      );\n      shape.startcap.virtual = i > 1;\n      shape.endcap.virtual = i < len / 2 - 1;\n      shapes.push(shape);\n    }\n    return shapes;\n  }\n\n  intersects(curve, curveIntersectionThreshold) {\n    if (!curve) return this.selfintersects(curveIntersectionThreshold);\n    if (curve.p1 && curve.p2) {\n      return this.lineIntersects(curve);\n    }\n    if (curve instanceof Bezier) {\n      curve = curve.reduce();\n    }\n    return this.curveintersects(\n      this.reduce(),\n      curve,\n      curveIntersectionThreshold\n    );\n  }\n\n  lineIntersects(line) {\n    const mx = min(line.p1.x, line.p2.x),\n      my = min(line.p1.y, line.p2.y),\n      MX = max(line.p1.x, line.p2.x),\n      MY = max(line.p1.y, line.p2.y);\n    return utils.roots(this.points, line).filter((t) => {\n      var p = this.get(t);\n      return utils.between(p.x, mx, MX) && utils.between(p.y, my, MY);\n    });\n  }\n\n  selfintersects(curveIntersectionThreshold) {\n    // \"simple\" curves cannot intersect with their direct\n    // neighbour, so for each segment X we check whether\n    // it intersects [0:x-2][x+2:last].\n\n    const reduced = this.reduce(),\n      len = reduced.length - 2,\n      results = [];\n\n    for (let i = 0, result, left, right; i < len; i++) {\n      left = reduced.slice(i, i + 1);\n      right = reduced.slice(i + 2);\n      result = this.curveintersects(left, right, curveIntersectionThreshold);\n      results.push(...result);\n    }\n    return results;\n  }\n\n  curveintersects(c1, c2, curveIntersectionThreshold) {\n    const pairs = [];\n    // step 1: pair off any overlapping segments\n    c1.forEach(function (l) {\n      c2.forEach(function (r) {\n        if (l.overlaps(r)) {\n          pairs.push({ left: l, right: r });\n        }\n      });\n    });\n    // step 2: for each pairing, run through the convergence algorithm.\n    let intersections = [];\n    pairs.forEach(function (pair) {\n      const result = utils.pairiteration(\n        pair.left,\n        pair.right,\n        curveIntersectionThreshold\n      );\n      if (result.length > 0) {\n        intersections = intersections.concat(result);\n      }\n    });\n    return intersections;\n  }\n\n  arcs(errorThreshold) {\n    errorThreshold = errorThreshold || 0.5;\n    return this._iterate(errorThreshold, []);\n  }\n\n  _error(pc, np1, s, e) {\n    const q = (e - s) / 4,\n      c1 = this.get(s + q),\n      c2 = this.get(e - q),\n      ref = utils.dist(pc, np1),\n      d1 = utils.dist(pc, c1),\n      d2 = utils.dist(pc, c2);\n    return abs(d1 - ref) + abs(d2 - ref);\n  }\n\n  _iterate(errorThreshold, circles) {\n    let t_s = 0,\n      t_e = 1,\n      safety;\n    // we do a binary search to find the \"good `t` closest to no-longer-good\"\n    do {\n      safety = 0;\n\n      // step 1: start with the maximum possible arc\n      t_e = 1;\n\n      // points:\n      let np1 = this.get(t_s),\n        np2,\n        np3,\n        arc,\n        prev_arc;\n\n      // booleans:\n      let curr_good = false,\n        prev_good = false,\n        done;\n\n      // numbers:\n      let t_m = t_e,\n        prev_e = 1,\n        step = 0;\n\n      // step 2: find the best possible arc\n      do {\n        prev_good = curr_good;\n        prev_arc = arc;\n        t_m = (t_s + t_e) / 2;\n        step++;\n\n        np2 = this.get(t_m);\n        np3 = this.get(t_e);\n\n        arc = utils.getccenter(np1, np2, np3);\n\n        //also save the t values\n        arc.interval = {\n          start: t_s,\n          end: t_e,\n        };\n\n        let error = this._error(arc, np1, t_s, t_e);\n        curr_good = error <= errorThreshold;\n\n        done = prev_good && !curr_good;\n        if (!done) prev_e = t_e;\n\n        // this arc is fine: we can move 'e' up to see if we can find a wider arc\n        if (curr_good) {\n          // if e is already at max, then we're done for this arc.\n          if (t_e >= 1) {\n            // make sure we cap at t=1\n            arc.interval.end = prev_e = 1;\n            prev_arc = arc;\n            // if we capped the arc segment to t=1 we also need to make sure that\n            // the arc's end angle is correct with respect to the bezier end point.\n            if (t_e > 1) {\n              let d = {\n                x: arc.x + arc.r * cos(arc.e),\n                y: arc.y + arc.r * sin(arc.e),\n              };\n              arc.e += utils.angle({ x: arc.x, y: arc.y }, d, this.get(1));\n            }\n            break;\n          }\n          // if not, move it up by half the iteration distance\n          t_e = t_e + (t_e - t_s) / 2;\n        } else {\n          // this is a bad arc: we need to move 'e' down to find a good arc\n          t_e = t_m;\n        }\n      } while (!done && safety++ < 100);\n\n      if (safety >= 100) {\n        break;\n      }\n\n      // console.log(\"L835: [F] arc found\", t_s, prev_e, prev_arc.x, prev_arc.y, prev_arc.s, prev_arc.e);\n\n      prev_arc = prev_arc ? prev_arc : arc;\n      circles.push(prev_arc);\n      t_s = prev_e;\n    } while (t_e < 1);\n    return circles;\n  }\n}\n\nexport { Bezier };\n",
         "export default {\n\taliceblue: [240, 248, 255],\n\tantiquewhite: [250, 235, 215],\n\taqua: [0, 255, 255],\n\taquamarine: [127, 255, 212],\n\tazure: [240, 255, 255],\n\tbeige: [245, 245, 220],\n\tbisque: [255, 228, 196],\n\tblack: [0, 0, 0],\n\tblanchedalmond: [255, 235, 205],\n\tblue: [0, 0, 255],\n\tblueviolet: [138, 43, 226],\n\tbrown: [165, 42, 42],\n\tburlywood: [222, 184, 135],\n\tcadetblue: [95, 158, 160],\n\tchartreuse: [127, 255, 0],\n\tchocolate: [210, 105, 30],\n\tcoral: [255, 127, 80],\n\tcornflowerblue: [100, 149, 237],\n\tcornsilk: [255, 248, 220],\n\tcrimson: [220, 20, 60],\n\tcyan: [0, 255, 255],\n\tdarkblue: [0, 0, 139],\n\tdarkcyan: [0, 139, 139],\n\tdarkgoldenrod: [184, 134, 11],\n\tdarkgray: [169, 169, 169],\n\tdarkgreen: [0, 100, 0],\n\tdarkgrey: [169, 169, 169],\n\tdarkkhaki: [189, 183, 107],\n\tdarkmagenta: [139, 0, 139],\n\tdarkolivegreen: [85, 107, 47],\n\tdarkorange: [255, 140, 0],\n\tdarkorchid: [153, 50, 204],\n\tdarkred: [139, 0, 0],\n\tdarksalmon: [233, 150, 122],\n\tdarkseagreen: [143, 188, 143],\n\tdarkslateblue: [72, 61, 139],\n\tdarkslategray: [47, 79, 79],\n\tdarkslategrey: [47, 79, 79],\n\tdarkturquoise: [0, 206, 209],\n\tdarkviolet: [148, 0, 211],\n\tdeeppink: [255, 20, 147],\n\tdeepskyblue: [0, 191, 255],\n\tdimgray: [105, 105, 105],\n\tdimgrey: [105, 105, 105],\n\tdodgerblue: [30, 144, 255],\n\tfirebrick: [178, 34, 34],\n\tfloralwhite: [255, 250, 240],\n\tforestgreen: [34, 139, 34],\n\tfuchsia: [255, 0, 255],\n\tgainsboro: [220, 220, 220],\n\tghostwhite: [248, 248, 255],\n\tgold: [255, 215, 0],\n\tgoldenrod: [218, 165, 32],\n\tgray: [128, 128, 128],\n\tgreen: [0, 128, 0],\n\tgreenyellow: [173, 255, 47],\n\tgrey: [128, 128, 128],\n\thoneydew: [240, 255, 240],\n\thotpink: [255, 105, 180],\n\tindianred: [205, 92, 92],\n\tindigo: [75, 0, 130],\n\tivory: [255, 255, 240],\n\tkhaki: [240, 230, 140],\n\tlavender: [230, 230, 250],\n\tlavenderblush: [255, 240, 245],\n\tlawngreen: [124, 252, 0],\n\tlemonchiffon: [255, 250, 205],\n\tlightblue: [173, 216, 230],\n\tlightcoral: [240, 128, 128],\n\tlightcyan: [224, 255, 255],\n\tlightgoldenrodyellow: [250, 250, 210],\n\tlightgray: [211, 211, 211],\n\tlightgreen: [144, 238, 144],\n\tlightgrey: [211, 211, 211],\n\tlightpink: [255, 182, 193],\n\tlightsalmon: [255, 160, 122],\n\tlightseagreen: [32, 178, 170],\n\tlightskyblue: [135, 206, 250],\n\tlightslategray: [119, 136, 153],\n\tlightslategrey: [119, 136, 153],\n\tlightsteelblue: [176, 196, 222],\n\tlightyellow: [255, 255, 224],\n\tlime: [0, 255, 0],\n\tlimegreen: [50, 205, 50],\n\tlinen: [250, 240, 230],\n\tmagenta: [255, 0, 255],\n\tmaroon: [128, 0, 0],\n\tmediumaquamarine: [102, 205, 170],\n\tmediumblue: [0, 0, 205],\n\tmediumorchid: [186, 85, 211],\n\tmediumpurple: [147, 112, 219],\n\tmediumseagreen: [60, 179, 113],\n\tmediumslateblue: [123, 104, 238],\n\tmediumspringgreen: [0, 250, 154],\n\tmediumturquoise: [72, 209, 204],\n\tmediumvioletred: [199, 21, 133],\n\tmidnightblue: [25, 25, 112],\n\tmintcream: [245, 255, 250],\n\tmistyrose: [255, 228, 225],\n\tmoccasin: [255, 228, 181],\n\tnavajowhite: [255, 222, 173],\n\tnavy: [0, 0, 128],\n\toldlace: [253, 245, 230],\n\tolive: [128, 128, 0],\n\tolivedrab: [107, 142, 35],\n\torange: [255, 165, 0],\n\torangered: [255, 69, 0],\n\torchid: [218, 112, 214],\n\tpalegoldenrod: [238, 232, 170],\n\tpalegreen: [152, 251, 152],\n\tpaleturquoise: [175, 238, 238],\n\tpalevioletred: [219, 112, 147],\n\tpapayawhip: [255, 239, 213],\n\tpeachpuff: [255, 218, 185],\n\tperu: [205, 133, 63],\n\tpink: [255, 192, 203],\n\tplum: [221, 160, 221],\n\tpowderblue: [176, 224, 230],\n\tpurple: [128, 0, 128],\n\trebeccapurple: [102, 51, 153],\n\tred: [255, 0, 0],\n\trosybrown: [188, 143, 143],\n\troyalblue: [65, 105, 225],\n\tsaddlebrown: [139, 69, 19],\n\tsalmon: [250, 128, 114],\n\tsandybrown: [244, 164, 96],\n\tseagreen: [46, 139, 87],\n\tseashell: [255, 245, 238],\n\tsienna: [160, 82, 45],\n\tsilver: [192, 192, 192],\n\tskyblue: [135, 206, 235],\n\tslateblue: [106, 90, 205],\n\tslategray: [112, 128, 144],\n\tslategrey: [112, 128, 144],\n\tsnow: [255, 250, 250],\n\tspringgreen: [0, 255, 127],\n\tsteelblue: [70, 130, 180],\n\ttan: [210, 180, 140],\n\tteal: [0, 128, 128],\n\tthistle: [216, 191, 216],\n\ttomato: [255, 99, 71],\n\tturquoise: [64, 224, 208],\n\tviolet: [238, 130, 238],\n\twheat: [245, 222, 179],\n\twhite: [255, 255, 255],\n\twhitesmoke: [245, 245, 245],\n\tyellow: [255, 255, 0],\n\tyellowgreen: [154, 205, 50]\n}\n",
         "/**\n * @module color-parse\n */\nimport names from 'color-name'\n\nexport default parse\n\n/**\n * Base hues\n * http://dev.w3.org/csswg/css-color/#typedef-named-hue\n */\n//FIXME: use external hue detector\nvar baseHues = {\n\tred: 0,\n\torange: 60,\n\tyellow: 120,\n\tgreen: 180,\n\tblue: 240,\n\tpurple: 300\n}\n\n/**\n * Parse color from the string passed\n *\n * @return {Object} A space indicator `space`, an array `values` and `alpha`\n */\nfunction parse(cstr) {\n\tvar m, parts = [], alpha = 1, space\n\n\t//numeric case\n\tif (typeof cstr === 'number') {\n\t\treturn { space: 'rgb', values: [cstr >>> 16, (cstr & 0x00ff00) >>> 8, cstr & 0x0000ff], alpha: 1 }\n\t}\n\tif (typeof cstr === 'number') return { space: 'rgb', values: [cstr >>> 16, (cstr & 0x00ff00) >>> 8, cstr & 0x0000ff], alpha: 1 }\n\n\tcstr = String(cstr).toLowerCase();\n\n\t//keyword\n\tif (names[cstr]) {\n\t\tparts = names[cstr].slice()\n\t\tspace = 'rgb'\n\t}\n\n\t//reserved words\n\telse if (cstr === 'transparent') {\n\t\talpha = 0\n\t\tspace = 'rgb'\n\t\tparts = [0, 0, 0]\n\t}\n\n\t//hex\n\telse if (cstr[0] === '#') {\n\t\tvar base = cstr.slice(1)\n\t\tvar size = base.length\n\t\tvar isShort = size <= 4\n\t\talpha = 1\n\n\t\tif (isShort) {\n\t\t\tparts = [\n\t\t\t\tparseInt(base[0] + base[0], 16),\n\t\t\t\tparseInt(base[1] + base[1], 16),\n\t\t\t\tparseInt(base[2] + base[2], 16)\n\t\t\t]\n\t\t\tif (size === 4) {\n\t\t\t\talpha = parseInt(base[3] + base[3], 16) / 255\n\t\t\t}\n\t\t}\n\t\telse {\n\t\t\tparts = [\n\t\t\t\tparseInt(base[0] + base[1], 16),\n\t\t\t\tparseInt(base[2] + base[3], 16),\n\t\t\t\tparseInt(base[4] + base[5], 16)\n\t\t\t]\n\t\t\tif (size === 8) {\n\t\t\t\talpha = parseInt(base[6] + base[7], 16) / 255\n\t\t\t}\n\t\t}\n\n\t\tif (!parts[0]) parts[0] = 0\n\t\tif (!parts[1]) parts[1] = 0\n\t\tif (!parts[2]) parts[2] = 0\n\n\t\tspace = 'rgb'\n\t}\n\n\t// color space\n\telse if (m = /^((?:rgba?|hs[lvb]a?|hwba?|cmyk?|xy[zy]|gray|lab|lchu?v?|[ly]uv|lms|oklch|oklab|color))\\s*\\(([^\\)]*)\\)/.exec(cstr)) {\n\t\tvar name = m[1]\n\t\tspace = name.replace(/a$/, '')\n\t\tvar dims = space === 'cmyk' ? 4 : space === 'gray' ? 1 : 3\n\t\tparts = m[2].trim().split(/\\s*[,\\/]\\s*|\\s+/)\n\n\t\t// color(srgb-linear x x x) -> srgb-linear(x x x)\n\t\tif (space === 'color') space = parts.shift()\n\n\t\tparts = parts.map(function (x, i) {\n\t\t\t//<percentage>\n\t\t\tif (x[x.length - 1] === '%') {\n\t\t\t\tx = parseFloat(x) / 100\n\t\t\t\t// alpha -> 0..1\n\t\t\t\tif (i === 3) return x\n\t\t\t\t// rgb -> 0..255\n\t\t\t\tif (space === 'rgb') return x * 255\n\t\t\t\t// hsl, hwb H -> 0..100\n\t\t\t\tif (space[0] === 'h') return x * 100\n\t\t\t\t// lch, lab L -> 0..100\n\t\t\t\tif (space[0] === 'l' && !i) return x * 100\n\t\t\t\t// lab A B -> -125..125\n\t\t\t\tif (space === 'lab') return x * 125\n\t\t\t\t// lch C -> 0..150, H -> 0..360\n\t\t\t\tif (space === 'lch') return i < 2 ? x * 150 : x * 360\n\t\t\t\t// oklch/oklab L -> 0..1\n\t\t\t\tif (space[0] === 'o' && !i) return x\n\t\t\t\t// oklab A B -> -0.4..0.4\n\t\t\t\tif (space === 'oklab') return x * 0.4\n\t\t\t\t// oklch C -> 0..0.4, H -> 0..360\n\t\t\t\tif (space === 'oklch') return i < 2 ? x * 0.4 : x * 360\n\t\t\t\t// color(xxx) -> 0..1\n\t\t\t\treturn x\n\t\t\t}\n\n\t\t\t//hue\n\t\t\tif (space[i] === 'h' || (i === 2 && space[space.length - 1] === 'h')) {\n\t\t\t\t//<base-hue>\n\t\t\t\tif (baseHues[x] !== undefined) return baseHues[x]\n\t\t\t\t//<deg>\n\t\t\t\tif (x.endsWith('deg')) return parseFloat(x)\n\t\t\t\t//<turn>\n\t\t\t\tif (x.endsWith('turn')) return parseFloat(x) * 360\n\t\t\t\tif (x.endsWith('grad')) return parseFloat(x) * 360 / 400\n\t\t\t\tif (x.endsWith('rad')) return parseFloat(x) * 180 / Math.PI\n\t\t\t}\n\t\t\tif (x === 'none') return 0\n\t\t\treturn parseFloat(x)\n\t\t});\n\n\t\talpha = parts.length > dims ? parts.pop() : 1\n\t}\n\n\t//named channels case\n\telse if (/[0-9](?:\\s|\\/|,)/.test(cstr)) {\n\t\tparts = cstr.match(/([0-9]+)/g).map(function (value) {\n\t\t\treturn parseFloat(value)\n\t\t})\n\n\t\tspace = cstr.match(/([a-z])/ig)?.join('')?.toLowerCase() || 'rgb'\n\t}\n\n\treturn {\n\t\tspace,\n\t\tvalues: parts,\n\t\talpha\n\t}\n}\n",
         "/**\n * RGB space.\n *\n * @module  color-space/rgb\n */\n\nexport default {\n\tname: 'rgb',\n\tmin: [0,0,0],\n\tmax: [255,255,255],\n\tchannel: ['red', 'green', 'blue'],\n\talias: ['RGB']\n};\n",
         "/**\n * @module color-space/hsl\n */\nimport rgb from './rgb.js';\n\nexport default {\n\tname: 'hsl',\n\tmin: [0,0,0],\n\tmax: [360,100,100],\n\tchannel: ['hue', 'saturation', 'lightness'],\n\talias: ['HSL'],\n\n\trgb: function(hsl) {\n\t\tvar h = hsl[0]/360, s = hsl[1]/100, l = hsl[2]/100, t1, t2, t3, rgb, val, i=0;\n\n\t\tif (s === 0) return val = l * 255, [val, val, val];\n\n\t\tt2 = l < 0.5 ? l * (1 + s) : l + s - l * s;\n\t\tt1 = 2 * l - t2;\n\n\t\trgb = [0, 0, 0];\n\t\tfor (;i<3;) {\n\t\t\tt3 = h + 1 / 3 * - (i - 1);\n\t\t\tt3 < 0 ? t3++ : t3 > 1 && t3--;\n\t\t\tval = 6 * t3 < 1 ? t1 + (t2 - t1) * 6 * t3 :\n\t\t\t2 * t3 < 1 ? t2 :\n\t\t\t3 * t3 < 2 ?  t1 + (t2 - t1) * (2 / 3 - t3) * 6 :\n\t\t\tt1;\n\t\t\trgb[i++] = val * 255;\n\t\t}\n\n\t\treturn rgb;\n\t}\n};\n\n\n//extend rgb\nrgb.hsl = function(rgb) {\n\tvar r = rgb[0]/255,\n\t\t\tg = rgb[1]/255,\n\t\t\tb = rgb[2]/255,\n\t\t\tmin = Math.min(r, g, b),\n\t\t\tmax = Math.max(r, g, b),\n\t\t\tdelta = max - min,\n\t\t\th, s, l;\n\n\tif (max === min) {\n\t\th = 0;\n\t}\n\telse if (r === max) {\n\t\th = (g - b) / delta;\n\t}\n\telse if (g === max) {\n\t\th = 2 + (b - r) / delta;\n\t}\n\telse if (b === max) {\n\t\th = 4 + (r - g)/ delta;\n\t}\n\n\th = Math.min(h * 60, 360);\n\n\tif (h < 0) {\n\t\th += 360;\n\t}\n\n\tl = (min + max) / 2;\n\n\tif (max === min) {\n\t\ts = 0;\n\t}\n\telse if (l <= 0.5) {\n\t\ts = delta / (max + min);\n\t}\n\telse {\n\t\ts = delta / (2 - max - min);\n\t}\n\n\treturn [h, s * 100, l * 100];\n};\n",
         "/** @module  color-rgba */\nimport parse from 'color-parse'\nimport rgb from 'color-space/rgb.js'\nimport hsl from 'color-space/hsl.js'\n\nexport default function rgba(color) {\n\t// template literals\n\tif (Array.isArray(color) && color.raw) color = String.raw(...arguments)\n\tif (color instanceof Number) color = +color\n\n\tvar values, i, l\n\n\t//attempt to parse non-array arguments\n\tvar parsed = parse(color)\n\n\tif (!parsed.space) return []\n\n\tconst min = parsed.space[0] === 'h' ? hsl.min : rgb.min\n\tconst max = parsed.space[0] === 'h' ? hsl.max : rgb.max\n\n\tvalues = Array(3)\n\tvalues[0] = Math.min(Math.max(parsed.values[0], min[0]), max[0])\n\tvalues[1] = Math.min(Math.max(parsed.values[1], min[1]), max[1])\n\tvalues[2] = Math.min(Math.max(parsed.values[2], min[2]), max[2])\n\n\tif (parsed.space[0] === 'h') {\n\t\tvalues = hsl.rgb(values)\n\t}\n\n\tvalues.push(Math.min(Math.max(parsed.alpha, 0), 1))\n\n\treturn values\n}\n",
-        "import { Bezier } from \"bezier-js\"\r\nimport rgba from \"color-rgba\"\r\n\r\nexport function createFixedData(data, options) {\r\n  console.log(data)\r\n  const fixedLines = options && options.fixed_lines ? options.fixed_lines : []\r\n  const datasets = Object.entries(data)\r\n    .filter(([colName]) => fixedLines.includes(colName))\r\n    .map(([colName, colData], index) => {\r\n      const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n      const colorRGBA = rgba(colData.color)\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.5)`\r\n      return {\r\n        data: data,\r\n        isControlPoint: false,\r\n        label: colName,\r\n        fill: false,\r\n        tension: 0.3,\r\n        spanGaps: false,\r\n        showLine: true,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: colData.color,\r\n      }\r\n    })\r\n\r\n  return {\r\n    datasets: datasets,\r\n  }\r\n}\r\n\r\nexport function createControlData(data, options) {\r\n  const fillGaps = options && options.fill_gaps ? options.fill_gaps : false\r\n  const fixedLines = options && options.fixed_lines ? options.fixed_lines : []\r\n  const datasets = Object.entries(data)\r\n    .filter(([colName]) => !fixedLines.includes(colName))\r\n    .map(([colName, colData], index) => {\r\n      const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n      const colorRGBA = rgba(colData.color)\r\n      const borderColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.7)`\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.5)`\r\n      return {\r\n        data: data,\r\n        isControlPoint: true,\r\n        label: colName,\r\n        fill: false,\r\n        tension: 0,\r\n        cubicInterpolationMode: \"default\",\r\n        spanGaps: fillGaps,\r\n        showLine: true,\r\n        borderDash: [5, 5],\r\n        borderWidth: 1,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: borderColorRGBA,\r\n      }\r\n    })\r\n\r\n  return {\r\n    datasets: datasets,\r\n  }\r\n}\r\n\r\nexport function createBezierData(data, options) {\r\n  const fixedLines = options && options.fixed_lines ? options.fixed_lines : []\r\n  const datasets = Object.entries(data)\r\n    .filter(([trace]) => !fixedLines.includes(trace))\r\n    .map(([trace, traceData], i) => {\r\n      const points = traceData.x.map((x, j) => ({\r\n        x: x,\r\n        y: traceData.y[j],\r\n      }))\r\n\r\n      const bezierSegments = []\r\n      for (let i = 0; i < points.length - 2; i += 2) {\r\n        const bezierPoints = points.slice(i, i + 3)\r\n        const bezier = new Bezier(bezierPoints)\r\n        const lut = bezier.getLUT(10)\r\n        bezierSegments.push(...lut)\r\n      }\r\n      const colorRGBA = rgba(traceData.color)\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.7)`\r\n      const borderColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.4)`\r\n      return {\r\n        label: trace + \" (bezier)\",\r\n        data: bezierSegments,\r\n        isControlPoint: false,\r\n        showLine: true,\r\n        tension: 0.3,\r\n        pointRadius: 0,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: borderColorRGBA,\r\n      }\r\n    })\r\n\r\n  return { datasets }\r\n}\r\n",
+        "import { Bezier } from \"bezier-js\"\r\nimport rgba from \"color-rgba\"\r\n\r\nexport function createFixedData(data, options) {\r\n  const fixedLines = options && options.fixed_lines ? options.fixed_lines : []\r\n  const datasets = Object.entries(data)\r\n    .filter(([colName]) => fixedLines.includes(colName))\r\n    .map(([colName, colData], index) => {\r\n      const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n      const colorRGBA = rgba(colData.color)\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.5)`\r\n      return {\r\n        data: data,\r\n        isControlPoint: false,\r\n        label: colName,\r\n        fill: false,\r\n        tension: 0.3,\r\n        spanGaps: false,\r\n        showLine: true,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: colData.color,\r\n      }\r\n    })\r\n\r\n  return {\r\n    datasets: datasets,\r\n  }\r\n}\r\n\r\nexport function createControlData(data, options) {\r\n  const fillGaps = options && options.fill_gaps ? options.fill_gaps : false\r\n  const fixedLines = options && options.fixed_lines ? options.fixed_lines : []\r\n  const datasets = Object.entries(data)\r\n    .filter(([colName]) => !fixedLines.includes(colName))\r\n    .map(([colName, colData], index) => {\r\n      const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n      const colorRGBA = rgba(colData.color)\r\n      const borderColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.7)`\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.5)`\r\n      return {\r\n        data: data,\r\n        isControlPoint: true,\r\n        label: colName,\r\n        fill: false,\r\n        tension: 0,\r\n        cubicInterpolationMode: \"default\",\r\n        spanGaps: fillGaps,\r\n        showLine: true,\r\n        borderDash: [5, 5],\r\n        borderWidth: 1,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: borderColorRGBA,\r\n      }\r\n    })\r\n\r\n  return {\r\n    datasets: datasets,\r\n  }\r\n}\r\n\r\nexport function createBezierData(data, options) {\r\n  const fixedLines = options && options.fixed_lines ? options.fixed_lines : []\r\n  const datasets = Object.entries(data)\r\n    .filter(([trace]) => !fixedLines.includes(trace))\r\n    .map(([trace, traceData], i) => {\r\n      const points = traceData.x.map((x, j) => ({\r\n        x: x,\r\n        y: traceData.y[j],\r\n      }))\r\n\r\n      const bezierSegments = []\r\n      for (let i = 0; i < points.length - 2; i += 2) {\r\n        const bezierPoints = points.slice(i, i + 3)\r\n        const bezier = new Bezier(bezierPoints)\r\n        const lut = bezier.getLUT(10)\r\n        bezierSegments.push(...lut)\r\n      }\r\n      const colorRGBA = rgba(traceData.color)\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.7)`\r\n      const borderColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.4)`\r\n      return {\r\n        label: trace + \" (bezier)\",\r\n        data: bezierSegments,\r\n        isControlPoint: false,\r\n        showLine: true,\r\n        tension: 0.3,\r\n        pointRadius: 0,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: borderColorRGBA,\r\n      }\r\n    })\r\n\r\n  return { datasets }\r\n}\r\n",
         "export function createOptions(options, theme) {\r\n  return {\r\n    responsive: true,\r\n    indexAxis: \"x\",\r\n    animation: {\r\n      duration: 0,\r\n    },\r\n    tooltips: {\r\n      mode: \"nearest\",\r\n    },\r\n    onHover: createHoverOptions(),\r\n    plugins: {\r\n      zoom: createZoomOptions(),\r\n      title: createTitleOptions(options),\r\n      legend: createLegendOptions(options),\r\n    },\r\n    scales: createScalesOptions(options, theme),\r\n  }\r\n}\r\n\r\nfunction createHoverOptions() {\r\n  return (event, chartElement) => {\r\n    if (chartElement.length > 0) {\r\n      event.native.target.style.cursor = \"crosshair\"\r\n    } else {\r\n      event.native.target.style.cursor = \"default\"\r\n    }\r\n  }\r\n}\r\n\r\nfunction createZoomOptions() {\r\n  return {\r\n    zoom: {\r\n      wheel: {\r\n        enabled: true,\r\n      },\r\n      mode: \"y\",\r\n    },\r\n    pan: {\r\n      enabled: true,\r\n    },\r\n    limits: {\r\n      x: { min: \"original\", max: \"original\" },\r\n      y: { min: \"original\", max: \"original\" },\r\n    },\r\n  }\r\n}\r\n\r\nfunction createTitleOptions(options) {\r\n  return {\r\n    display: true,\r\n    text: options.title,\r\n  }\r\n}\r\n\r\nfunction createLegendOptions(options) {\r\n  return {\r\n    display: options.legend,\r\n    position: options.legend_position,\r\n    align: options.legend_align,\r\n    labels: {\r\n      boxWidth: 16,\r\n      boxHeight: 8,\r\n      padding: 8,\r\n    },\r\n    onHover: (event, legendItem, legend) => {\r\n      if (legendItem) {\r\n        event.native.target.style.cursor = \"pointer\"\r\n      } else {\r\n        event.native.target.style.cursor = \"default\"\r\n      }\r\n    },\r\n  }\r\n}\r\n\r\nfunction createScalesOptions(options, theme) {\r\n  const xScaleOptions = {\r\n    display: true,\r\n    type: options.x_type,\r\n    title: {\r\n      display: true,\r\n      text: options.x_label,\r\n    },\r\n    grid: {\r\n      display: options.x_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.x_labels) {\r\n    xScaleOptions.min = options.x_labels[0]\r\n    xScaleOptions.max = options.x_labels[options.x_labels.length - 1]\r\n  }\r\n\r\n  const yScaleOptions = {\r\n    display: true,\r\n    type: options.y_type,\r\n    title: {\r\n      display: true,\r\n      text: options.y_label,\r\n    },\r\n    grid: {\r\n      display: options.y_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.y_labels) {\r\n    yScaleOptions.labels = options.y_labels\r\n    yScaleOptions.min = options.y_labels[0]\r\n    yScaleOptions.max = options.y_labels[options.y_labels.length - 1]\r\n  }\r\n\r\n  return {\r\n    x: xScaleOptions,\r\n    y: yScaleOptions,\r\n  }\r\n}\r\n",
         "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\n\r\nimport { Scatter, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport {\r\n  createFixedData,\r\n  createControlData,\r\n  createBezierData,\r\n} from \"./chartData\"\r\nimport { createOptions } from \"./chartOptions\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass BezierChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.fixedData = createFixedData(\r\n      this.props.args.data,\r\n      this.props.args.options\r\n    )\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      controlData: createControlData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      bezierData: createBezierData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n    // Return the initial Bezier data:\r\n    // this.sendBezierData()\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        controlData: createControlData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        bezierData: createBezierData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  sendBezierData() {\r\n    const newBezierData = this.convertBezierData(this.state.bezierData.datasets)\r\n    Streamlit.setComponentValue(newBezierData)\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const dataset =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex]\r\n      if (dataset.isControlPoint) {\r\n        this.setState({ activePoint: points[0] })\r\n        this.togglePan(false)\r\n      }\r\n    }\r\n  }\r\n\r\n  calculateNewYValue = (position, chartArea, yAxis) => {\r\n    return this.map(\r\n      position.y,\r\n      chartArea.bottom,\r\n      chartArea.top,\r\n      yAxis.min,\r\n      yAxis.max\r\n    )\r\n  }\r\n\r\n  calculateNewXValue = (position, chartArea, xAxis) => {\r\n    return this.map(\r\n      position.x,\r\n      chartArea.left,\r\n      chartArea.right,\r\n      xAxis.min,\r\n      xAxis.max\r\n    )\r\n  }\r\n\r\n  updateControlPointPosition = (chart, activePoint, newXValue, newYValue) => {\r\n    const datasetIndex = activePoint.datasetIndex\r\n    const pointIndex = activePoint.index\r\n    chart.data.datasets[datasetIndex].data[pointIndex].x = newXValue\r\n    chart.data.datasets[datasetIndex].data[pointIndex].y = newYValue\r\n  }\r\n\r\n  updateOriginalData = (chart, activePoint) => {\r\n    const datasetIndex = activePoint.datasetIndex\r\n    const pointIndex = activePoint.index\r\n    const datasetLabel = chart.data.datasets[datasetIndex].label\r\n    const xValue = chart.data.datasets[datasetIndex].data[pointIndex].x\r\n    const yValue = chart.data.datasets[datasetIndex].data[pointIndex].y\r\n\r\n    this.state.originalData[datasetLabel][\"x\"][pointIndex] = xValue\r\n    this.state.originalData[datasetLabel][\"y\"][pointIndex] = yValue\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const activePoint = this.state.activePoint\r\n      const position = getRelativePosition(event, chart)\r\n      const chartArea = chart.chartArea\r\n\r\n      const newYValue = this.calculateNewYValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.y\r\n      )\r\n\r\n      const newXValue = this.calculateNewXValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.x\r\n      )\r\n\r\n      // Update control point position\r\n      this.updateControlPointPosition(chart, activePoint, newXValue, newYValue)\r\n      // Set new values in originalData\r\n      this.updateOriginalData(chart, activePoint)\r\n\r\n      // Recalculate Bezier data\r\n      const bezierData = createBezierData(\r\n        this.state.originalData,\r\n        this.props.args.options\r\n      )\r\n      // Update state\r\n      this.setState({ bezierData })\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      this.sendBezierData()\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n    }\r\n  }\r\n\r\n  convertBezierData(bezierData) {\r\n    const result = {}\r\n    bezierData.forEach((dataset) => {\r\n      const trace = dataset.label.replace(\" (bezier)\", \"\")\r\n      result[trace] = {\r\n        x: [],\r\n        y: [],\r\n      }\r\n      dataset.data.forEach((point) => {\r\n        const { x, y } = point\r\n        const index = result[trace].x.findIndex(\r\n          (val, i) => val === x && result[trace].y[i] === y\r\n        )\r\n        if (index === -1) {\r\n          result[trace].x.push(x)\r\n          result[trace].y.push(y)\r\n        }\r\n      })\r\n    })\r\n    return result\r\n  }\r\n\r\n  map = (value, start1, stop1, start2, stop2) => {\r\n    return start2 + (stop2 - start2) * ((value - start1) / (stop1 - start1))\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Scatter\r\n        ref={this.chartRef}\r\n        data={{\r\n          datasets: [\r\n            ...this.fixedData.datasets,\r\n            ...this.state.controlData.datasets,\r\n            ...this.state.bezierData.datasets,\r\n          ],\r\n        }}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default BezierChart\r\n",
-        "import LineChart from \"./LineChart/LineChart\";\r\nimport ScatterChart from \"./ScatterChart/ScatterChart\";\r\nimport BezierChart from \"./BezierChart/BezierChart\";\r\n\r\nconst componentsMap = {\r\n  line_chart: LineChart,\r\n  scatter_chart: ScatterChart,\r\n  bezier_chart: BezierChart,\r\n}\r\n\r\nexport default componentsMap\r\n",
+        "import { Bezier } from \"bezier-js\"\r\nimport rgba from \"color-rgba\"\r\n\r\nexport function createFixedData(data, options) {\r\n  const fixedLines = options && options.fixed_lines ? options.fixed_lines : []\r\n  const datasets = Object.entries(data)\r\n    .filter(([colName]) => fixedLines.includes(colName))\r\n    .map(([colName, colData], index) => {\r\n      const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n      const colorRGBA = rgba(colData.color)\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.5)`\r\n      return {\r\n        data: data,\r\n        isControlPoint: false,\r\n        label: colName,\r\n        fill: false,\r\n        tension: 0.3,\r\n        spanGaps: false,\r\n        showLine: true,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: colData.color,\r\n      }\r\n    })\r\n\r\n  return {\r\n    datasets: datasets,\r\n  }\r\n}\r\n\r\nexport function createControlData(data, options) {\r\n  const fillGaps = options && options.fill_gaps ? options.fill_gaps : false\r\n  const fixedLines = options && options.fixed_lines ? options.fixed_lines : []\r\n  const lineControl = (ctx, value, length) => {\r\n    const index = ctx.p1DataIndex\r\n    if (\r\n      (index % 3 === 0 && index < length - 1) ||\r\n      index % 3 === 1 ||\r\n      index == length - 1\r\n    ) {\r\n      return value\r\n    } else {\r\n      return undefined\r\n    }\r\n  }\r\n  const datasets = Object.entries(data)\r\n    .filter(([colName]) => !fixedLines.includes(colName))\r\n    .map(([colName, colData], index) => {\r\n      const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n      const colorRGBA = rgba(colData.color)\r\n      const borderColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 1)`\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.8)`\r\n      return {\r\n        data: data,\r\n        isControlPoint: true,\r\n        label: colName,\r\n        spanGaps: fillGaps,\r\n        showLine: true,\r\n        borderDash: [8, 5],\r\n        borderWidth: 1.2,\r\n        segment: {\r\n          borderColor: (ctx) => lineControl(ctx, borderColorRGBA, data.length),\r\n        },\r\n        backgroundColor: backgroundColorRGBA,\r\n      }\r\n    })\r\n\r\n  return {\r\n    datasets: datasets,\r\n  }\r\n}\r\n\r\nexport function createBezierData(data, options) {\r\n  const fixedLines = options && options.fixed_lines ? options.fixed_lines : []\r\n  const datasets = Object.entries(data)\r\n    .filter(([trace]) => !fixedLines.includes(trace))\r\n    .map(([trace, traceData], i) => {\r\n      const points = traceData.x.map((x, j) => ({\r\n        x: x,\r\n        y: traceData.y[j],\r\n      }))\r\n\r\n      const bezierSegments = []\r\n      for (let i = 0; i < points.length - 3; i += 3) {\r\n        const bezierPoints = points.slice(i, i + 4)\r\n        const bezier = new Bezier(bezierPoints)\r\n        const lut = bezier.getLUT(10)\r\n        bezierSegments.push(...lut)\r\n      }\r\n      const colorRGBA = rgba(traceData.color)\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.7)`\r\n      const borderColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.4)`\r\n      return {\r\n        label: trace + \" (bezier)\",\r\n        data: bezierSegments,\r\n        isControlPoint: false,\r\n        showLine: true,\r\n        tension: 0.3,\r\n        pointRadius: 0,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: borderColorRGBA,\r\n      }\r\n    })\r\n\r\n  return { datasets }\r\n}\r\n",
+        "export function createOptions(options, theme) {\r\n  return {\r\n    responsive: true,\r\n    indexAxis: \"x\",\r\n    animation: {\r\n      duration: 0,\r\n    },\r\n    onHover: createHoverOptions(),\r\n    plugins: {\r\n      tooltip: {\r\n        filter: function (tooltipItem) {\r\n          return !tooltipItem.dataset.label.includes(\"bezier\")\r\n        },\r\n      },\r\n      zoom: createZoomOptions(),\r\n      title: createTitleOptions(options),\r\n      legend: createLegendOptions(options),\r\n    },\r\n    scales: createScalesOptions(options, theme),\r\n  }\r\n}\r\n\r\nfunction createHoverOptions() {\r\n  return (event, chartElement) => {\r\n    if (chartElement.length > 0) {\r\n      event.native.target.style.cursor = \"crosshair\"\r\n    } else {\r\n      event.native.target.style.cursor = \"default\"\r\n    }\r\n  }\r\n}\r\n\r\nfunction createZoomOptions() {\r\n  return {\r\n    zoom: {\r\n      wheel: {\r\n        enabled: true,\r\n      },\r\n      mode: \"y\",\r\n    },\r\n    pan: {\r\n      enabled: true,\r\n    },\r\n    limits: {\r\n      x: { min: \"original\", max: \"original\" },\r\n      y: { min: \"original\", max: \"original\" },\r\n    },\r\n  }\r\n}\r\n\r\nfunction createTitleOptions(options) {\r\n  return {\r\n    display: true,\r\n    text: options.title,\r\n  }\r\n}\r\n\r\nfunction createLegendOptions(options) {\r\n  return {\r\n    display: options.legend,\r\n    position: options.legend_position,\r\n    align: options.legend_align,\r\n    labels: {\r\n      boxWidth: 16,\r\n      boxHeight: 8,\r\n      padding: 8,\r\n    },\r\n    onHover: (event, legendItem, legend) => {\r\n      if (legendItem) {\r\n        event.native.target.style.cursor = \"pointer\"\r\n      } else {\r\n        event.native.target.style.cursor = \"default\"\r\n      }\r\n    },\r\n  }\r\n}\r\n\r\nfunction createScalesOptions(options, theme) {\r\n  const xScaleOptions = {\r\n    display: true,\r\n    type: options.x_type,\r\n    title: {\r\n      display: true,\r\n      text: options.x_label,\r\n    },\r\n    grid: {\r\n      display: options.x_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.x_labels) {\r\n    xScaleOptions.min = options.x_labels[0]\r\n    xScaleOptions.max = options.x_labels[options.x_labels.length - 1]\r\n  }\r\n\r\n  const yScaleOptions = {\r\n    display: true,\r\n    type: options.y_type,\r\n    title: {\r\n      display: true,\r\n      text: options.y_label,\r\n    },\r\n    grid: {\r\n      display: options.y_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.y_labels) {\r\n    yScaleOptions.labels = options.y_labels\r\n    yScaleOptions.min = options.y_labels[0]\r\n    yScaleOptions.max = options.y_labels[options.y_labels.length - 1]\r\n  }\r\n\r\n  return {\r\n    x: xScaleOptions,\r\n    y: yScaleOptions,\r\n  }\r\n}\r\n",
+        "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\n\r\nimport { Scatter, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport {\r\n  createFixedData,\r\n  createControlData,\r\n  createBezierData,\r\n} from \"./chartData\"\r\nimport { createOptions } from \"./chartOptions\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass CubicBezierChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.fixedData = createFixedData(\r\n      this.props.args.data,\r\n      this.props.args.options\r\n    )\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      controlData: createControlData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      bezierData: createBezierData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n    // Return the initial Bezier data:\r\n    // this.sendBezierData()\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        controlData: createControlData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        bezierData: createBezierData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  sendBezierData() {\r\n    const newBezierData = this.convertBezierData(this.state.bezierData.datasets)\r\n    Streamlit.setComponentValue(newBezierData)\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const dataset =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex]\r\n      if (dataset.isControlPoint) {\r\n        this.setState({ activePoint: points[0] })\r\n        this.togglePan(false)\r\n      }\r\n    }\r\n  }\r\n\r\n  calculateNewYValue = (position, chartArea, yAxis) => {\r\n    return this.map(\r\n      position.y,\r\n      chartArea.bottom,\r\n      chartArea.top,\r\n      yAxis.min,\r\n      yAxis.max\r\n    )\r\n  }\r\n\r\n  calculateNewXValue = (position, chartArea, xAxis) => {\r\n    return this.map(\r\n      position.x,\r\n      chartArea.left,\r\n      chartArea.right,\r\n      xAxis.min,\r\n      xAxis.max\r\n    )\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const activePoint = this.state.activePoint\r\n      const position = getRelativePosition(event, chart)\r\n      const chartArea = chart.chartArea\r\n\r\n      const newYValue = this.calculateNewYValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.y\r\n      )\r\n\r\n      const newXValue = this.calculateNewXValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.x\r\n      )\r\n\r\n      // Update control point position\r\n      const datasetIndex = activePoint.datasetIndex\r\n      const pointIndex = activePoint.index\r\n      const deltaY =\r\n        newYValue - chart.data.datasets[datasetIndex].data[pointIndex].y\r\n      const deltaX =\r\n        newXValue - chart.data.datasets[datasetIndex].data[pointIndex].x\r\n\r\n      chart.data.datasets[datasetIndex].data[pointIndex].x = newXValue\r\n      chart.data.datasets[datasetIndex].data[pointIndex].y = newYValue\r\n\r\n      // Set new values in originalData\r\n      const datasetLabel = chart.data.datasets[datasetIndex].label\r\n      const xValue = chart.data.datasets[datasetIndex].data[pointIndex].x\r\n      const yValue = chart.data.datasets[datasetIndex].data[pointIndex].y\r\n      this.state.originalData[datasetLabel][\"x\"][pointIndex] = xValue\r\n      this.state.originalData[datasetLabel][\"y\"][pointIndex] = yValue\r\n\r\n      // If activePoint index is 3, move points 2 and 4 as well\r\n      // If activePoint index is 3, update originalData for points 2 and 4 as well\r\n      const dataLen = chart.data.datasets[datasetIndex].data.length\r\n      if (pointIndex === 0) {\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 1].x += deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 1].y += deltaY\r\n\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex + 1] += deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex + 1] += deltaY\r\n      }\r\n      else if (pointIndex === dataLen - 1) {\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 1].x += deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 1].y += deltaY\r\n\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex - 1] += deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex - 1] += deltaY\r\n      }\r\n      else if (\r\n        pointIndex % 3 === 0 &&\r\n        pointIndex != 0 &&\r\n        pointIndex != dataLen - 1\r\n      ) {\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 1].x += deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 1].y += deltaY\r\n\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 1].x += deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 1].y += deltaY\r\n\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex - 1] += deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex - 1] += deltaY\r\n\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex + 1] += deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex + 1] += deltaY\r\n      } else if ((pointIndex + 1) % 3 === 0 && pointIndex + 1 != dataLen - 1) {\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 2].x -= deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 2].y -= deltaY\r\n\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex + 2] -= deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex + 2] -= deltaY\r\n      } else if ((pointIndex - 1) % 3 === 0 && pointIndex - 1 != 0) {\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 2].x -= deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 2].y -= deltaY\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex - 2] -= deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex - 2] -= deltaY\r\n      }\r\n\r\n      // Recalculate Bezier data\r\n      const bezierData = createBezierData(\r\n        this.state.originalData,\r\n        this.props.args.options\r\n      )\r\n      // Update state\r\n      this.setState({ bezierData })\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      this.sendBezierData()\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n    }\r\n  }\r\n\r\n  convertBezierData(bezierData) {\r\n    const result = {}\r\n    bezierData.forEach((dataset) => {\r\n      const trace = dataset.label.replace(\" (bezier)\", \"\")\r\n      result[trace] = {\r\n        x: [],\r\n        y: [],\r\n      }\r\n      dataset.data.forEach((point) => {\r\n        const { x, y } = point\r\n        const index = result[trace].x.findIndex(\r\n          (val, i) => val === x && result[trace].y[i] === y\r\n        )\r\n        if (index === -1) {\r\n          result[trace].x.push(x)\r\n          result[trace].y.push(y)\r\n        }\r\n      })\r\n    })\r\n    return result\r\n  }\r\n\r\n  map = (value, start1, stop1, start2, stop2) => {\r\n    return start2 + (stop2 - start2) * ((value - start1) / (stop1 - start1))\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Scatter\r\n        ref={this.chartRef}\r\n        data={{\r\n          datasets: [\r\n            ...this.fixedData.datasets,\r\n            ...this.state.controlData.datasets,\r\n            ...this.state.bezierData.datasets,\r\n          ],\r\n        }}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default CubicBezierChart\r\n",
+        "import LineChart from \"./LineChart/LineChart\";\r\nimport ScatterChart from \"./ScatterChart/ScatterChart\";\r\nimport BezierChart from \"./BezierChart/BezierChart\";\r\nimport CubicBezierChart from \"./CubicBezierChart/CubicBezierChart\";\r\n\r\nconst componentsMap = {\r\n  line_chart: LineChart,\r\n  scatter_chart: ScatterChart,\r\n  bezier_chart: BezierChart,\r\n  cubic_bezier_chart: CubicBezierChart,\r\n}\r\n\r\nexport default componentsMap\r\n",
         "import { withStreamlitConnection } from \"streamlit-component-lib\"\r\n\r\nimport React from \"react\"\r\nimport ReactDOM from \"react-dom\"\r\nimport componentsMap from \"./components\"\r\n\r\nconst SelectComponent = (props) => {\r\n  const id = props.args[\"id\"]\r\n  const kw = props.args[\"kw\"]\r\n  const Component = componentsMap[id]\r\n  if (Component === undefined) {\r\n    throw new Error(`Component with id ${id} is not defined in componentsMap.`)\r\n  } else {\r\n    return <Component args={{ ...kw }} theme={props.theme} />\r\n  }\r\n}\r\n\r\nconst StreamlitComponent = withStreamlitConnection(SelectComponent)\r\n\r\nReactDOM.render(\r\n  <React.StrictMode>\r\n    <StreamlitComponent />\r\n  </React.StrictMode>,\r\n  document.getElementById(\"root\")\r\n)\r\n"
     ],
     "version": 3
 }
```

### Comparing `draggable-charts-1.1.1/draggable_charts/utils/callback.py` & `draggable-charts-1.1.2/draggable_charts/utils/callback.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.1/draggable_charts/utils/component_func.py` & `draggable-charts-1.1.2/draggable_charts/utils/component_func.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.1/draggable_charts/widgets/bezierchart.py` & `draggable-charts-1.1.2/draggable_charts/widgets/bezierchart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.1/draggable_charts/widgets/linechart.py` & `draggable-charts-1.1.2/draggable_charts/widgets/linechart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.1/draggable_charts/widgets/scatterchart.py` & `draggable-charts-1.1.2/draggable_charts/widgets/scatterchart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.1.1/draggable_charts.egg-info/PKG-INFO` & `draggable-charts-1.1.2/draggable_charts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `draggable-charts-1.1.1/draggable_charts.egg-info/SOURCES.txt` & `draggable-charts-1.1.2/draggable_charts.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 draggable_charts/__init__.py
-draggable_charts/example.py
 draggable_charts.egg-info/PKG-INFO
 draggable_charts.egg-info/SOURCES.txt
 draggable_charts.egg-info/dependency_links.txt
 draggable_charts.egg-info/requires.txt
 draggable_charts.egg-info/top_level.txt
 draggable_charts/frontend/build/asset-manifest.json
 draggable_charts/frontend/build/bootstrap.min.css
 draggable_charts/frontend/build/index.html
-draggable_charts/frontend/build/static/js/main.ac399b09.js
-draggable_charts/frontend/build/static/js/main.ac399b09.js.LICENSE.txt
-draggable_charts/frontend/build/static/js/main.ac399b09.js.map
+draggable_charts/frontend/build/static/js/main.96151505.js
+draggable_charts/frontend/build/static/js/main.96151505.js.LICENSE.txt
+draggable_charts/frontend/build/static/js/main.96151505.js.map
 draggable_charts/utils/__init__.py
 draggable_charts/utils/callback.py
 draggable_charts/utils/component_func.py
 draggable_charts/widgets/__init__.py
 draggable_charts/widgets/bezierchart.py
+draggable_charts/widgets/cubicbezierchart.py
 draggable_charts/widgets/linechart.py
 draggable_charts/widgets/scatterchart.py
```

### Comparing `draggable-charts-1.1.1/setup.py` & `draggable-charts-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="draggable-charts",
-    version="1.1.1",
+    version="1.1.2",
     author="Brayan Munoz",
     author_email="balexander.munoz@udea.edu.co",
     description="A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/balexandermunoz/draggable-charts",
     packages=setuptools.find_packages(),
```
