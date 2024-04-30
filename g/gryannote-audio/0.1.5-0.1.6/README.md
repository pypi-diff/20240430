# Comparing `tmp/gryannote_audio-0.1.5.tar.gz` & `tmp/gryannote_audio-0.1.6.tar.gz`

## Comparing `gryannote_audio-0.1.5.tar` & `gryannote_audio-0.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/__init__.py
--rw-r--r--   0        0        0    16841 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/annotatedaudio.py
--rw-r--r--   0        0        0    77967 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/annotatedaudio.pyi
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/core.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/__vite-browser-external-2447137e.js
--rw-r--r--   0        0        0   400469 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/index.js
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-2c3384e6.js
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-aafe8b06.js
--rw-r--r--   0        0        0   118992 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-d82531d9.js
--rw-r--r--   0        0        0    24006 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/style.css
--rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/wrapper-6f348d45-19fa94bf.js
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/example/index.js
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/demo/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/demo/app.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/Example.svelte
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/Index.svelte
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/index.ts
--rw-r--r--   0        0        0    48788 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/package-lock.json
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/package.json
--rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/interactive/InteractiveAnnotatedAudio.svelte
--rw-r--r--   0        0        0    20347 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/player/AudioPlayerWithAnnotation.svelte
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/recorder/AudioRecorder.svelte
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/AnnotatedAudioData.ts
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/Audio.svelte
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/Caption.svelte
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/VolumeControl.svelte
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/VolumeLevels.svelte
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/WaveformControls.svelte
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/WaveformRecordControls.svelte
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/audioBufferToWav.ts
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/index.ts
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/types.ts
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/utils.ts
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/icons/Gum.svelte
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/icons/Magnifier.svelte
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/icons/Plus.svelte
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/static/StaticAnnotatedAudio.svelte
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/streaming/StreamAudio.svelte
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/.gitignore
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/README.md
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/__init__.py
+-rw-r--r--   0        0        0    16841 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/annotatedaudio.py
+-rw-r--r--   0        0        0    77967 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/annotatedaudio.pyi
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/core.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/__vite-browser-external-2447137e.js
+-rw-r--r--   0        0        0   400691 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/index.js
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/module-2c3384e6.js
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/module-aafe8b06.js
+-rw-r--r--   0        0        0   118992 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/module-d82531d9.js
+-rw-r--r--   0        0        0    24050 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/style.css
+-rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/wrapper-6f348d45-19fa94bf.js
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/templates/example/index.js
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/backend/gryannote_audio/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/demo/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/demo/app.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/Example.svelte
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/Index.svelte
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/index.ts
+-rw-r--r--   0        0        0    48788 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/package-lock.json
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/package.json
+-rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/interactive/InteractiveAnnotatedAudio.svelte
+-rw-r--r--   0        0        0    20373 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/player/AudioPlayerWithAnnotation.svelte
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/recorder/AudioRecorder.svelte
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/AnnotatedAudioData.ts
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/Audio.svelte
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/Caption.svelte
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/VolumeControl.svelte
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/VolumeLevels.svelte
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/WaveformControls.svelte
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/WaveformRecordControls.svelte
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/audioBufferToWav.ts
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/index.ts
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/types.ts
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/utils.ts
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/icons/Gum.svelte
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/icons/Magnifier.svelte
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/shared/icons/Plus.svelte
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/static/StaticAnnotatedAudio.svelte
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/frontend/streaming/StreamAudio.svelte
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/.gitignore
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/README.md
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 gryannote_audio-0.1.6/PKG-INFO
```

### Comparing `gryannote_audio-0.1.5/backend/gryannote_audio/annotatedaudio.py` & `gryannote_audio-0.1.6/backend/gryannote_audio/annotatedaudio.py`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/backend/gryannote_audio/annotatedaudio.pyi` & `gryannote_audio-0.1.6/backend/gryannote_audio/annotatedaudio.pyi`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/backend/gryannote_audio/core.py` & `gryannote_audio-0.1.6/backend/gryannote_audio/core.py`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/index.js` & `gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -35,16 +35,16 @@
     return {
         ws_protocol: "wss",
         http_protocol: "https:",
         host: t
     };
 }
 const La = /^[^\/]*\/[^\/]*$/,
-    kc = /.*hf\.space\/{0,1}$/;
-async function Ec(t, e) {
+    Cc = /.*hf\.space\/{0,1}$/;
+async function Sc(t, e) {
     const n = {};
     e && (n.Authorization = `Bearer ${e}`);
     const i = t.trim();
     if (La.test(i))
         try {
             const o = await fetch(
                 `https://huggingface.co/api/spaces/${i}/host`, {
@@ -57,15 +57,15 @@
             return {
                 space_id: t,
                 ...Oo(r)
             };
         } catch (o) {
             throw new Error("Space metadata could not be loaded." + o.message);
         }
-    if (kc.test(i)) {
+    if (Cc.test(i)) {
         const {
             ws_protocol: o,
             http_protocol: r,
             host: s
         } = Oo(i);
         return {
             space_id: s.replace(".hf.space", ""),
@@ -76,37 +76,37 @@
     }
     return {
         space_id: !1,
         ...Oo(i)
     };
 }
 
-function Cc(t) {
+function Ac(t) {
     let e = {};
     return t.forEach(({
         api_name: n
     }, i) => {
         n && (e[n] = i);
     }), e;
 }
-const Sc = /^(?=[^]*\b[dD]iscussions{0,1}\b)(?=[^]*\b[dD]isabled\b)[^]*$/;
+const Tc = /^(?=[^]*\b[dD]iscussions{0,1}\b)(?=[^]*\b[dD]isabled\b)[^]*$/;
 async function vs(t) {
     try {
         const n = (await fetch(
             `https://huggingface.co/api/spaces/${t}/discussions`, {
                 method: "HEAD"
             }
         )).headers.get("x-error-message");
-        return !(n && Sc.test(n));
+        return !(n && Tc.test(n));
     } catch {
         return !1;
     }
 }
 
-function Ac(t, e, n, i) {
+function Pc(t, e, n, i) {
     if (e.length === 0) {
         if (n === "replace")
             return i;
         if (n === "append")
             return t + i;
         throw new Error(`Unsupported action: ${n}`);
     }
@@ -129,20 +129,20 @@
             break;
         default:
             throw new Error(`Unknown action: ${n}`);
     }
     return t;
 }
 
-function Tc(t, e) {
+function Lc(t, e) {
     return e.forEach(([n, i, o]) => {
-        t = Ac(t, i, n, o);
+        t = Pc(t, i, n, o);
     }), t;
 }
-async function Ra(t, e, n, i = Lc) {
+async function Ra(t, e, n, i = Bc) {
     let o = (Array.isArray(t) ? t : [t]).map(
         (r) => r.blob
     );
     return await Promise.all(
         await i(e, o, void 0, n).then(
             async (r) => {
                 if (r.error)
@@ -184,15 +184,15 @@
         }, this.path = e, this.url = n, this.orig_name = i, this.size = o, this.blob = n ? void 0 : r, this.is_stream = s, this.mime_type = a, this.alt_text = l;
     }
 }
 const Ma = "This application is too busy. Keep trying!",
     Vt = "Connection errored out.";
 let Da;
 
-function Pc(t, e) {
+function Rc(t, e) {
     return {
         post_data: n,
         upload_files: i,
         client: o,
         handle_blob: r
     };
     async function n(s, a, l) {
@@ -224,698 +224,698 @@
     async function i(s, a, l, u) {
         const c = {};
         l && (c.Authorization = `Bearer ${l}`);
         const f = 1e3,
             h = [];
         for (let _ = 0; _ < a.length; _ += f) {
             const m = a.slice(_, _ + f),
-                v = new FormData();
+                b = new FormData();
             m.forEach((S) => {
-                v.append("files", S);
+                b.append("files", S);
             });
             try {
                 const S = u ? `${s}/upload?upload_id=${u}` : `${s}/upload`;
                 var d = await t(S, {
                     method: "POST",
-                    body: v,
+                    body: b,
                     headers: c
                 });
             } catch {
                 return {
                     error: Vt
                 };
             }
-            const b = await d.json();
-            h.push(...b);
+            const g = await d.json();
+            h.push(...g);
         }
         return {
             files: h
         };
     }
     async function o(s, a = {}) {
         return new Promise(async (l) => {
             const {
                 status_callback: u,
                 hf_token: c
             } = a, f = {
                 predict: X,
                 submit: C,
-                view_api: K,
+                view_api: $,
                 component_server: U
             };
             if ((typeof window > "u" || !("WebSocket" in window)) && !global.Websocket) {
                 const O = await import("./wrapper-6f348d45-19fa94bf.js");
                 Da = (await import("./__vite-browser-external-2447137e.js")).Blob, global.WebSocket = O.WebSocket;
             }
             const {
                 ws_protocol: h,
                 http_protocol: d,
                 host: _,
                 space_id: m
-            } = await Ec(s, c), v = Math.random().toString(36).substring(2), b = {};
+            } = await Sc(s, c), b = Math.random().toString(36).substring(2), g = {};
             let S = !1,
                 w = {},
                 k = {},
                 E = null;
             const y = {},
                 H = /* @__PURE__ */ new Set();
             let L, P = {},
-                M = !1;
-            c && m && (M = await Bc(m, c));
-            async function Z(O) {
-                if (L = O, window.location.protocol === "https:" && (L.root = L.root.replace("http://", "https://")), P = Cc((O == null ? void 0 : O.dependencies) || []), L.auth_required)
+                D = !1;
+            c && m && (D = await Dc(m, c));
+            async function J(O) {
+                if (L = O, window.location.protocol === "https:" && (L.root = L.root.replace("http://", "https://")), P = Ac((O == null ? void 0 : O.dependencies) || []), L.auth_required)
                     return {
                         config: L,
                         ...f
                     };
                 try {
-                    x = await K(L);
-                } catch (J) {
-                    console.error(`Could not get api details: ${J.message}`);
+                    Z = await $(L);
+                } catch (Y) {
+                    console.error(`Could not get api details: ${Y.message}`);
                 }
                 return {
                     config: L,
                     ...f
                 };
             }
-            let x;
+            let Z;
             async function j(O) {
                 if (u && u(O), O.status === "running")
                     try {
                         L = await Es(
                             t,
                             `${d}//${_}`,
                             c
                         );
-                        const J = await Z(L);
-                        l(J);
-                    } catch (J) {
-                        console.error(J), u && u({
+                        const Y = await J(L);
+                        l(Y);
+                    } catch (Y) {
+                        console.error(Y), u && u({
                             status: "error",
                             message: "Could not load this space.",
                             load_status: "error",
                             detail: "NOT_FOUND"
                         });
                     }
             }
             try {
                 L = await Es(
                     t,
                     `${d}//${_}`,
                     c
                 );
-                const O = await Z(L);
+                const O = await J(L);
                 l(O);
             } catch (O) {
                 console.error(O), m ? Rr(
                     m,
                     La.test(m) ? "space_name" : "subdomain",
                     j
                 ) : u && u({
                     status: "error",
                     message: "Could not load this space.",
                     load_status: "error",
                     detail: "NOT_FOUND"
                 });
             }
 
-            function X(O, J, le) {
+            function X(O, Y, se) {
                 let p = !1,
-                    A = !1,
+                    T = !1,
                     q;
                 if (typeof O == "number")
                     q = L.dependencies[O];
                 else {
                     const z = O.replace(/^\//, "");
                     q = L.dependencies[P[z]];
                 }
                 if (q.types.continuous)
                     throw new Error(
                         "Cannot call predict on this function as it may run forever. Use submit instead"
                     );
                 return new Promise((z, he) => {
-                    const _e = C(O, J, le);
+                    const _e = C(O, Y, se);
                     let F;
                     _e.on("data", (ve) => {
-                        A && (_e.destroy(), z(ve)), p = !0, F = ve;
+                        T && (_e.destroy(), z(ve)), p = !0, F = ve;
                     }).on("status", (ve) => {
-                        ve.stage === "error" && he(ve), ve.stage === "complete" && (A = !0, p && (_e.destroy(), z(F)));
+                        ve.stage === "error" && he(ve), ve.stage === "complete" && (T = !0, p && (_e.destroy(), z(F)));
                     });
                 });
             }
 
-            function C(O, J, le, p = null) {
-                let A, q;
+            function C(O, Y, se, p = null) {
+                let T, q;
                 if (typeof O == "number")
-                    A = O, q = x.unnamed_endpoints[A];
+                    T = O, q = Z.unnamed_endpoints[T];
                 else {
-                    const g = O.replace(/^\//, "");
-                    A = P[g], q = x.named_endpoints[O.trim()];
+                    const le = O.replace(/^\//, "");
+                    T = P[le], q = Z.named_endpoints[O.trim()];
                 }
-                if (typeof A != "number")
+                if (typeof T != "number")
                     throw new Error(
                         "There is no endpoint matching that name of fn_index matching that number."
                     );
                 let z, he, _e = L.protocol ?? "ws";
                 const F = typeof O == "number" ? "/predict" : O;
-                let ve, B = null,
-                    R = !1;
+                let ve, M = null,
+                    B = !1;
                 const ce = {};
                 let Se = "";
-                typeof window < "u" && (Se = new URLSearchParams(window.location.search).toString()), r(`${L.root}`, J, q, c).then(
-                    (g) => {
+                typeof window < "u" && (Se = new URLSearchParams(window.location.search).toString()), r(`${L.root}`, Y, q, c).then(
+                    (le) => {
                         if (ve = {
-                                data: g || [],
-                                event_data: le,
-                                fn_index: A,
+                                data: le || [],
+                                event_data: se,
+                                fn_index: T,
                                 trigger_id: p
-                            }, Mc(A, L))
-                            Y({
+                            }, Hc(T, L))
+                            Q({
                                 type: "status",
                                 endpoint: F,
                                 stage: "pending",
                                 queue: !1,
-                                fn_index: A,
+                                fn_index: T,
                                 time: /* @__PURE__ */ new Date()
                             }), n(
                                 `${L.root}/run${F.startsWith("/") ? F : `/${F}`}${Se ? "?" + Se : ""}`, {
                                     ...ve,
-                                    session_hash: v
+                                    session_hash: b
                                 },
                                 c
-                            ).then(([D, N]) => {
-                                const te = D.data;
-                                N == 200 ? (Y({
+                            ).then(([A, R]) => {
+                                const I = A.data;
+                                R == 200 ? (Q({
                                     type: "data",
                                     endpoint: F,
-                                    fn_index: A,
-                                    data: te,
+                                    fn_index: T,
+                                    data: I,
                                     time: /* @__PURE__ */ new Date()
-                                }), Y({
+                                }), Q({
                                     type: "status",
                                     endpoint: F,
-                                    fn_index: A,
+                                    fn_index: T,
                                     stage: "complete",
-                                    eta: D.average_duration,
+                                    eta: A.average_duration,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
-                                })) : Y({
+                                })) : Q({
                                     type: "status",
                                     stage: "error",
                                     endpoint: F,
-                                    fn_index: A,
-                                    message: D.error,
+                                    fn_index: T,
+                                    message: A.error,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
                                 });
-                            }).catch((D) => {
-                                Y({
+                            }).catch((A) => {
+                                Q({
                                     type: "status",
                                     stage: "error",
-                                    message: D.message,
+                                    message: A.message,
                                     endpoint: F,
-                                    fn_index: A,
+                                    fn_index: T,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
                                 });
                             });
                         else if (_e == "ws") {
-                            Y({
+                            Q({
                                 type: "status",
                                 stage: "pending",
                                 queue: !0,
                                 endpoint: F,
-                                fn_index: A,
+                                fn_index: T,
                                 time: /* @__PURE__ */ new Date()
                             });
-                            let D = new URL(`${h}://${Pa(
+                            let A = new URL(`${h}://${Pa(
                 _,
                 L.path,
                 !0
               )}
 							/queue/join${Se ? "?" + Se : ""}`);
-                            M && D.searchParams.set("__sign", M), z = new WebSocket(D), z.onclose = (N) => {
-                                N.wasClean || Y({
+                            D && A.searchParams.set("__sign", D), z = new WebSocket(A), z.onclose = (R) => {
+                                R.wasClean || Q({
                                     type: "status",
                                     stage: "error",
                                     broken: !0,
                                     message: Vt,
                                     queue: !0,
                                     endpoint: F,
-                                    fn_index: A,
+                                    fn_index: T,
                                     time: /* @__PURE__ */ new Date()
                                 });
-                            }, z.onmessage = function(N) {
-                                const te = JSON.parse(N.data),
+                            }, z.onmessage = function(R) {
+                                const I = JSON.parse(R.data),
                                     {
-                                        type: oe,
-                                        status: re,
+                                        type: ee,
+                                        status: x,
                                         data: ae
                                     } = No(
-                                        te,
-                                        b[A]
+                                        I,
+                                        g[T]
                                     );
-                                if (oe === "update" && re && !R)
-                                    Y({
+                                if (ee === "update" && x && !B)
+                                    Q({
                                         type: "status",
                                         endpoint: F,
-                                        fn_index: A,
+                                        fn_index: T,
                                         time: /* @__PURE__ */ new Date(),
-                                        ...re
-                                    }), re.stage === "error" && z.close();
-                                else if (oe === "hash") {
+                                        ...x
+                                    }), x.stage === "error" && z.close();
+                                else if (ee === "hash") {
                                     z.send(JSON.stringify({
-                                        fn_index: A,
-                                        session_hash: v
+                                        fn_index: T,
+                                        session_hash: b
                                     }));
                                     return;
                                 } else
-                                    oe === "data" ? z.send(JSON.stringify({
+                                    ee === "data" ? z.send(JSON.stringify({
                                         ...ve,
-                                        session_hash: v
-                                    })) : oe === "complete" ? R = re : oe === "log" ? Y({
+                                        session_hash: b
+                                    })) : ee === "complete" ? B = x : ee === "log" ? Q({
                                         type: "log",
                                         log: ae.log,
                                         level: ae.level,
                                         endpoint: F,
-                                        fn_index: A
-                                    }) : oe === "generating" && Y({
+                                        fn_index: T
+                                    }) : ee === "generating" && Q({
                                         type: "status",
                                         time: /* @__PURE__ */ new Date(),
-                                        ...re,
-                                        stage: re == null ? void 0 : re.stage,
+                                        ...x,
+                                        stage: x == null ? void 0 : x.stage,
                                         queue: !0,
                                         endpoint: F,
-                                        fn_index: A
+                                        fn_index: T
                                     });
-                                ae && (Y({
+                                ae && (Q({
                                     type: "data",
                                     time: /* @__PURE__ */ new Date(),
                                     data: ae.data,
                                     endpoint: F,
-                                    fn_index: A
-                                }), R && (Y({
+                                    fn_index: T
+                                }), B && (Q({
                                     type: "status",
                                     time: /* @__PURE__ */ new Date(),
-                                    ...R,
-                                    stage: re == null ? void 0 : re.stage,
+                                    ...B,
+                                    stage: x == null ? void 0 : x.stage,
                                     queue: !0,
                                     endpoint: F,
-                                    fn_index: A
+                                    fn_index: T
                                 }), z.close()));
                             }, bs(L.version || "2.0.0", "3.6") < 0 && addEventListener(
                                 "open",
                                 () => z.send(JSON.stringify({
-                                    hash: v
+                                    hash: b
                                 }))
                             );
                         } else if (_e == "sse") {
-                            Y({
+                            Q({
                                 type: "status",
                                 stage: "pending",
                                 queue: !0,
                                 endpoint: F,
-                                fn_index: A,
+                                fn_index: T,
                                 time: /* @__PURE__ */ new Date()
                             });
-                            var T = new URLSearchParams({
-                                fn_index: A.toString(),
-                                session_hash: v
+                            var v = new URLSearchParams({
+                                fn_index: T.toString(),
+                                session_hash: b
                             }).toString();
-                            let D = new URL(
-                                `${L.root}/queue/join?${Se ? Se + "&" : ""}${T}`
+                            let A = new URL(
+                                `${L.root}/queue/join?${Se ? Se + "&" : ""}${v}`
                             );
-                            he = e(D), he.onmessage = async function(N) {
-                                const te = JSON.parse(N.data),
+                            he = e(A), he.onmessage = async function(R) {
+                                const I = JSON.parse(R.data),
                                     {
-                                        type: oe,
-                                        status: re,
+                                        type: ee,
+                                        status: x,
                                         data: ae
                                     } = No(
-                                        te,
-                                        b[A]
+                                        I,
+                                        g[T]
                                     );
-                                if (oe === "update" && re && !R)
-                                    Y({
+                                if (ee === "update" && x && !B)
+                                    Q({
                                         type: "status",
                                         endpoint: F,
-                                        fn_index: A,
+                                        fn_index: T,
                                         time: /* @__PURE__ */ new Date(),
-                                        ...re
-                                    }), re.stage === "error" && he.close();
-                                else if (oe === "data") {
-                                    B = te.event_id;
-                                    let [Wt, yc] = await n(
+                                        ...x
+                                    }), x.stage === "error" && he.close();
+                                else if (ee === "data") {
+                                    M = I.event_id;
+                                    let [Wt, Ec] = await n(
                                         `${L.root}/queue/data`, {
                                             ...ve,
-                                            session_hash: v,
-                                            event_id: B
+                                            session_hash: b,
+                                            event_id: M
                                         },
                                         c
                                     );
-                                    yc !== 200 && (Y({
+                                    Ec !== 200 && (Q({
                                         type: "status",
                                         stage: "error",
                                         message: Vt,
                                         queue: !0,
                                         endpoint: F,
-                                        fn_index: A,
+                                        fn_index: T,
                                         time: /* @__PURE__ */ new Date()
                                     }), he.close());
                                 } else
-                                    oe === "complete" ? R = re : oe === "log" ? Y({
+                                    ee === "complete" ? B = x : ee === "log" ? Q({
                                         type: "log",
                                         log: ae.log,
                                         level: ae.level,
                                         endpoint: F,
-                                        fn_index: A
-                                    }) : oe === "generating" && Y({
+                                        fn_index: T
+                                    }) : ee === "generating" && Q({
                                         type: "status",
                                         time: /* @__PURE__ */ new Date(),
-                                        ...re,
-                                        stage: re == null ? void 0 : re.stage,
+                                        ...x,
+                                        stage: x == null ? void 0 : x.stage,
                                         queue: !0,
                                         endpoint: F,
-                                        fn_index: A
+                                        fn_index: T
                                     });
-                                ae && (Y({
+                                ae && (Q({
                                     type: "data",
                                     time: /* @__PURE__ */ new Date(),
                                     data: ae.data,
                                     endpoint: F,
-                                    fn_index: A
-                                }), R && (Y({
+                                    fn_index: T
+                                }), B && (Q({
                                     type: "status",
                                     time: /* @__PURE__ */ new Date(),
-                                    ...R,
-                                    stage: re == null ? void 0 : re.stage,
+                                    ...B,
+                                    stage: x == null ? void 0 : x.stage,
                                     queue: !0,
                                     endpoint: F,
-                                    fn_index: A
+                                    fn_index: T
                                 }), he.close()));
                             };
                         } else
-                            (_e == "sse_v1" || _e == "sse_v2" || _e == "sse_v2.1" || _e == "sse_v3") && (Y({
+                            (_e == "sse_v1" || _e == "sse_v2" || _e == "sse_v2.1" || _e == "sse_v3") && (Q({
                                 type: "status",
                                 stage: "pending",
                                 queue: !0,
                                 endpoint: F,
-                                fn_index: A,
+                                fn_index: T,
                                 time: /* @__PURE__ */ new Date()
                             }), n(
                                 `${L.root}/queue/join?${Se}`, {
                                     ...ve,
-                                    session_hash: v
+                                    session_hash: b
                                 },
                                 c
-                            ).then(([D, N]) => {
-                                if (N === 503)
-                                    Y({
+                            ).then(([A, R]) => {
+                                if (R === 503)
+                                    Q({
                                         type: "status",
                                         stage: "error",
                                         message: Ma,
                                         queue: !0,
                                         endpoint: F,
-                                        fn_index: A,
+                                        fn_index: T,
                                         time: /* @__PURE__ */ new Date()
                                     });
-                                else if (N !== 200)
-                                    Y({
+                                else if (R !== 200)
+                                    Q({
                                         type: "status",
                                         stage: "error",
                                         message: Vt,
                                         queue: !0,
                                         endpoint: F,
-                                        fn_index: A,
+                                        fn_index: T,
                                         time: /* @__PURE__ */ new Date()
                                     });
                                 else {
-                                    B = D.event_id;
-                                    let te = async function(oe) {
+                                    M = A.event_id;
+                                    let I = async function(ee) {
                                         try {
                                             const {
-                                                type: re,
+                                                type: x,
                                                 status: ae,
                                                 data: Wt
                                             } = No(
-                                                oe,
-                                                b[A]
+                                                ee,
+                                                g[T]
                                             );
-                                            if (re == "heartbeat")
+                                            if (x == "heartbeat")
                                                 return;
-                                            if (re === "update" && ae && !R)
-                                                Y({
+                                            if (x === "update" && ae && !B)
+                                                Q({
                                                     type: "status",
                                                     endpoint: F,
-                                                    fn_index: A,
+                                                    fn_index: T,
                                                     time: /* @__PURE__ */ new Date(),
                                                     ...ae
                                                 });
-                                            else if (re === "complete")
-                                                R = ae;
-                                            else if (re == "unexpected_error")
-                                                console.error("Unexpected error", ae == null ? void 0 : ae.message), Y({
+                                            else if (x === "complete")
+                                                B = ae;
+                                            else if (x == "unexpected_error")
+                                                console.error("Unexpected error", ae == null ? void 0 : ae.message), Q({
                                                     type: "status",
                                                     stage: "error",
                                                     message: (ae == null ? void 0 : ae.message) || "An Unexpected Error Occurred!",
                                                     queue: !0,
                                                     endpoint: F,
-                                                    fn_index: A,
+                                                    fn_index: T,
                                                     time: /* @__PURE__ */ new Date()
                                                 });
-                                            else if (re === "log") {
-                                                Y({
+                                            else if (x === "log") {
+                                                Q({
                                                     type: "log",
                                                     log: Wt.log,
                                                     level: Wt.level,
                                                     endpoint: F,
-                                                    fn_index: A
+                                                    fn_index: T
                                                 });
                                                 return;
                                             } else
-                                                re === "generating" && (Y({
+                                                x === "generating" && (Q({
                                                     type: "status",
                                                     time: /* @__PURE__ */ new Date(),
                                                     ...ae,
                                                     stage: ae == null ? void 0 : ae.stage,
                                                     queue: !0,
                                                     endpoint: F,
-                                                    fn_index: A
-                                                }), Wt && ["sse_v2", "sse_v2.1", "sse_v3"].includes(_e) && wt(B, Wt));
-                                            Wt && (Y({
+                                                    fn_index: T
+                                                }), Wt && ["sse_v2", "sse_v2.1", "sse_v3"].includes(_e) && wt(M, Wt));
+                                            Wt && (Q({
                                                 type: "data",
                                                 time: /* @__PURE__ */ new Date(),
                                                 data: Wt.data,
                                                 endpoint: F,
-                                                fn_index: A
-                                            }), R && Y({
+                                                fn_index: T
+                                            }), B && Q({
                                                 type: "status",
                                                 time: /* @__PURE__ */ new Date(),
-                                                ...R,
+                                                ...B,
                                                 stage: ae == null ? void 0 : ae.stage,
                                                 queue: !0,
                                                 endpoint: F,
-                                                fn_index: A
-                                            })), ((ae == null ? void 0 : ae.stage) === "complete" || (ae == null ? void 0 : ae.stage) === "error") && (y[B] && delete y[B], B in k && delete k[B]);
-                                        } catch (re) {
-                                            console.error("Unexpected client exception", re), Y({
+                                                fn_index: T
+                                            })), ((ae == null ? void 0 : ae.stage) === "complete" || (ae == null ? void 0 : ae.stage) === "error") && (y[M] && delete y[M], M in k && delete k[M]);
+                                        } catch (x) {
+                                            console.error("Unexpected client exception", x), Q({
                                                 type: "status",
                                                 stage: "error",
                                                 message: "An Unexpected Error Occurred!",
                                                 queue: !0,
                                                 endpoint: F,
-                                                fn_index: A,
+                                                fn_index: T,
                                                 time: /* @__PURE__ */ new Date()
-                                            }), ["sse_v2", "sse_v2.1"].includes(_e) && I();
+                                            }), ["sse_v2", "sse_v2.1"].includes(_e) && N();
                                         }
                                     };
-                                    B in w && (w[B].forEach(
-                                        (oe) => te(oe)
-                                    ), delete w[B]), y[B] = te, H.add(B), S || G();
+                                    M in w && (w[M].forEach(
+                                        (ee) => I(ee)
+                                    ), delete w[M]), y[M] = I, H.add(M), S || G();
                                 }
                             }));
                     }
                 );
 
-                function wt(g, T) {
-                    !k[g] ? (k[g] = [], T.data.forEach((N, te) => {
-                        k[g][te] = N;
-                    })) : T.data.forEach((N, te) => {
-                        let oe = Tc(
-                            k[g][te],
-                            N
+                function wt(le, v) {
+                    !k[le] ? (k[le] = [], v.data.forEach((R, I) => {
+                        k[le][I] = R;
+                    })) : v.data.forEach((R, I) => {
+                        let ee = Lc(
+                            k[le][I],
+                            R
                         );
-                        k[g][te] = oe, T.data[te] = oe;
+                        k[le][I] = ee, v.data[I] = ee;
                     });
                 }
 
-                function Y(g) {
-                    const D = ce[g.type] || [];
-                    D == null || D.forEach((N) => N(g));
+                function Q(le) {
+                    const A = ce[le.type] || [];
+                    A == null || A.forEach((R) => R(le));
                 }
 
-                function yt(g, T) {
-                    const D = ce,
-                        N = D[g] || [];
-                    return D[g] = N, N == null || N.push(T), {
+                function yt(le, v) {
+                    const A = ce,
+                        R = A[le] || [];
+                    return A[le] = R, R == null || R.push(v), {
                         on: yt,
                         off: wn,
-                        cancel: ei,
-                        destroy: ti
+                        cancel: ti,
+                        destroy: ni
                     };
                 }
 
-                function wn(g, T) {
-                    const D = ce;
-                    let N = D[g] || [];
-                    return N = N == null ? void 0 : N.filter((te) => te !== T), D[g] = N, {
+                function wn(le, v) {
+                    const A = ce;
+                    let R = A[le] || [];
+                    return R = R == null ? void 0 : R.filter((I) => I !== v), A[le] = R, {
                         on: yt,
                         off: wn,
-                        cancel: ei,
-                        destroy: ti
+                        cancel: ti,
+                        destroy: ni
                     };
                 }
-                async function ei() {
-                    const g = {
+                async function ti() {
+                    const le = {
                         stage: "complete",
                         queue: !1,
                         time: /* @__PURE__ */ new Date()
                     };
-                    R = g, Y({
-                        ...g,
+                    B = le, Q({
+                        ...le,
                         type: "status",
                         endpoint: F,
-                        fn_index: A
+                        fn_index: T
                     });
-                    let T = {};
+                    let v = {};
                     _e === "ws" ? (z && z.readyState === 0 ? z.addEventListener("open", () => {
                         z.close();
-                    }) : z.close(), T = {
-                        fn_index: A,
-                        session_hash: v
-                    }) : (he.close(), T = {
-                        event_id: B
+                    }) : z.close(), v = {
+                        fn_index: T,
+                        session_hash: b
+                    }) : (he.close(), v = {
+                        event_id: M
                     });
                     try {
                         await t(`${L.root}/reset`, {
                             headers: {
                                 "Content-Type": "application/json"
                             },
                             method: "POST",
-                            body: JSON.stringify(T)
+                            body: JSON.stringify(v)
                         });
                     } catch {
                         console.warn(
                             "The `/reset` endpoint could not be called. Subsequent endpoint results may be unreliable."
                         );
                     }
                 }
 
-                function ti() {
-                    for (const g in ce)
-                        ce[g].forEach((T) => {
-                            wn(g, T);
+                function ni() {
+                    for (const le in ce)
+                        ce[le].forEach((v) => {
+                            wn(le, v);
                         });
                 }
                 return {
                     on: yt,
                     off: wn,
-                    cancel: ei,
-                    destroy: ti
+                    cancel: ti,
+                    destroy: ni
                 };
             }
 
             function G() {
                 S = !0;
                 let O = new URLSearchParams({
-                        session_hash: v
+                        session_hash: b
                     }).toString(),
-                    J = new URL(`${L.root}/queue/data?${O}`);
-                E = e(J), E.onmessage = async function(le) {
-                    let p = JSON.parse(le.data);
-                    const A = p.event_id;
-                    if (!A)
+                    Y = new URL(`${L.root}/queue/data?${O}`);
+                E = e(Y), E.onmessage = async function(se) {
+                    let p = JSON.parse(se.data);
+                    const T = p.event_id;
+                    if (!T)
                         await Promise.all(
                             Object.keys(y).map(
                                 (q) => y[q](p)
                             )
                         );
-                    else if (y[A]) {
-                        p.msg === "process_completed" && ["sse", "sse_v1", "sse_v2", "sse_v2.1"].includes(L.protocol) && (H.delete(A), H.size === 0 && I());
-                        let q = y[A];
+                    else if (y[T]) {
+                        p.msg === "process_completed" && ["sse", "sse_v1", "sse_v2", "sse_v2.1"].includes(L.protocol) && (H.delete(T), H.size === 0 && N());
+                        let q = y[T];
                         window.setTimeout(q, 0, p);
                     } else
-                        w[A] || (w[A] = []), w[A].push(p);
-                    p.msg === "close_stream" && I();
-                }, E.onerror = async function(le) {
+                        w[T] || (w[T] = []), w[T].push(p);
+                    p.msg === "close_stream" && N();
+                }, E.onerror = async function(se) {
                     await Promise.all(
                         Object.keys(y).map(
                             (p) => y[p]({
                                 msg: "unexpected_error",
                                 message: Vt
                             })
                         )
-                    ), I();
+                    ), N();
                 };
             }
 
-            function I() {
+            function N() {
                 S = !1, E == null || E.close();
             }
-            async function U(O, J, le) {
+            async function U(O, Y, se) {
                 var p;
-                const A = {
+                const T = {
                     "Content-Type": "application/json"
                 };
-                c && (A.Authorization = `Bearer ${c}`);
+                c && (T.Authorization = `Bearer ${c}`);
                 let q, z = L.components.find(
                     (F) => F.id === O
                 );
                 (p = z == null ? void 0 : z.props) != null && p.root_url ? q = z.props.root_url : q = L.root;
                 const he = await t(
                     `${q}/component_server/`, {
                         method: "POST",
                         body: JSON.stringify({
-                            data: le,
+                            data: se,
                             component_id: O,
-                            fn_name: J,
-                            session_hash: v
+                            fn_name: Y,
+                            session_hash: b
                         }),
-                        headers: A
+                        headers: T
                     }
                 );
                 if (!he.ok)
                     throw new Error(
                         "Could not connect to component server: " + he.statusText
                     );
                 return await he.json();
             }
-            async function K(O) {
-                if (x)
-                    return x;
-                const J = {
+            async function $(O) {
+                if (Z)
+                    return Z;
+                const Y = {
                     "Content-Type": "application/json"
                 };
-                c && (J.Authorization = `Bearer ${c}`);
-                let le;
-                if (bs(O.version || "2.0.0", "3.30") < 0 ? le = await t(
+                c && (Y.Authorization = `Bearer ${c}`);
+                let se;
+                if (bs(O.version || "2.0.0", "3.30") < 0 ? se = await t(
                         "https://gradio-space-api-fetcher-v2.hf.space/api", {
                             method: "POST",
                             body: JSON.stringify({
                                 serialize: !1,
                                 config: JSON.stringify(O)
                             }),
-                            headers: J
+                            headers: Y
                         }
-                    ) : le = await t(`${O.root}/info`, {
-                        headers: J
-                    }), !le.ok)
+                    ) : se = await t(`${O.root}/info`, {
+                        headers: Y
+                    }), !se.ok)
                     throw new Error(Vt);
-                let p = await le.json();
-                return "api" in p && (p = p.api), p.named_endpoints["/predict"] && !p.unnamed_endpoints[0] && (p.unnamed_endpoints[0] = p.named_endpoints["/predict"]), Rc(p, O, P);
+                let p = await se.json();
+                return "api" in p && (p = p.api), p.named_endpoints["/predict"] && !p.unnamed_endpoints[0] && (p.unnamed_endpoints[0] = p.named_endpoints["/predict"]), Mc(p, O, P);
             }
         });
     }
     async function r(s, a, l, u) {
         const c = await Lr(
             a,
             void 0,
@@ -948,29 +948,29 @@
             file_url: d,
             type: _,
             name: m
         }) => {
             if (_ === "Gallery")
                 ks(a, d, h);
             else if (d) {
-                const v = new _o({
+                const b = new _o({
                     path: d,
                     orig_name: m
                 });
-                ks(a, v, h);
+                ks(a, b, h);
             }
         }), a));
     }
 }
 const {
-    post_data: zv,
-    upload_files: Lc,
-    client: Gv,
-    handle_blob: Wv
-} = Pc(
+    post_data: z2,
+    upload_files: Bc,
+    client: G2,
+    handle_blob: W2
+} = Rc(
     fetch,
     (...t) => new EventSource(...t)
 );
 
 function ws(t, e, n, i) {
     switch (t.type) {
         case "string":
@@ -992,15 +992,15 @@
         return i === "parameter" ? "[(Blob | File | Buffer), (string | null)][]" : "[{ name: string; data: string; size?: number; is_file?: boolean; orig_name?: string}, (string | null))][]";
 }
 
 function ys(t, e) {
     return e === "GallerySerializable" ? "array of [file, label] tuples" : e === "ListStringSerializable" ? "array of strings" : e === "FileSerializable" ? "array of files or single file" : t.description;
 }
 
-function Rc(t, e, n) {
+function Mc(t, e, n) {
     const i = {
         named_endpoints: {},
         unnamed_endpoints: {}
     };
     for (const o in t) {
         const r = t[o];
         for (const s in r) {
@@ -1031,15 +1031,15 @@
                     description: ys(f, h)
                 })
             );
         }
     }
     return i;
 }
-async function Bc(t, e) {
+async function Dc(t, e) {
     try {
         return (await (await fetch(`https://huggingface.co/api/spaces/${t}/jwt`, {
             headers: {
                 Authorization: `Bearer ${e}`
             }
         })).json()).token || !1;
     } catch (n) {
@@ -1094,15 +1094,15 @@
                 }
             return r;
         }
     }
     return [];
 }
 
-function Mc(t, e) {
+function Hc(t, e) {
     var n, i, o, r;
     return !(((i = (n = e == null ? void 0 : e.dependencies) == null ? void 0 : n[t]) == null ? void 0 : i.queue) === null ? e.enable_queue : (r = (o = e == null ? void 0 : e.dependencies) == null ? void 0 : o[t]) != null && r.queue) || !1;
 }
 async function Es(t, e, n) {
     const i = {};
     if (n && (i.Authorization = `Bearer ${n}`), typeof window < "u" && window.gradio_config && location.origin !== "http://localhost:9876" && !window.gradio_config.dev_mode) {
         const o = window.gradio_config.root,
@@ -1337,15 +1337,15 @@
             blob: r,
             is_stream: s,
             mime_type: a,
             alt_text: l
         }), this.annotations = null;
     }
 }
-const Dc = [{
+const Oc = [{
         color: "red",
         primary: 600,
         secondary: 100
     }, {
         color: "green",
         primary: 600,
         secondary: 100
@@ -1671,29 +1671,29 @@
             600: "#e11d48",
             700: "#be123c",
             800: "#9f1239",
             900: "#881337",
             950: "#4c0519"
         }
     };
-Dc.reduce(
+Oc.reduce(
     (t, {
         color: e,
         primary: n,
         secondary: i
     }) => ({
         ...t,
         [e]: {
             primary: Ss[e][n],
             secondary: Ss[e][i]
         }
     }), {}
 );
 
-function Hc(t) {
+function Nc(t) {
     let e, n = t[0],
         i = 1;
     for (; i < t.length;) {
         const o = t[i],
             r = t[i + 1];
         if (i += 2, (o === "optionalAccess" || o === "optionalCall") && n == null)
             return;
@@ -1702,45 +1702,45 @@
     return n;
 }
 class Io extends Error {
     constructor(e) {
         super(e), this.name = "ShareError";
     }
 }
-async function Oc(t, e) {
+async function Ic(t, e) {
     if (window.__gradio_space__ == null)
         throw new Io("Must be on Spaces to share.");
     let n, i, o;
     if (e === "url") {
         const l = await fetch(t);
         n = await l.blob(), i = l.headers.get("content-type") || "", o = l.headers.get("content-disposition") || "";
     } else
-        n = Nc(t), i = t.split(";")[0].split(":")[1], o = "file" + i.split("/")[1];
+        n = Uc(t), i = t.split(";")[0].split(":")[1], o = "file" + i.split("/")[1];
     const r = new File([n], o, {
             type: i
         }),
         s = await fetch("https://huggingface.co/uploads", {
             method: "POST",
             body: r,
             headers: {
                 "Content-Type": r.type,
                 "X-Requested-With": "XMLHttpRequest"
             }
         });
     if (!s.ok) {
-        if (Hc([s, "access", (l) => l.headers, "access", (l) => l.get, "call", (l) => l("content-type"), "optionalAccess", (l) => l.includes, "call", (l) => l("application/json")])) {
+        if (Nc([s, "access", (l) => l.headers, "access", (l) => l.get, "call", (l) => l("content-type"), "optionalAccess", (l) => l.includes, "call", (l) => l("application/json")])) {
             const l = await s.json();
             throw new Io(`Upload failed: ${l.error}`);
         }
         throw new Io("Upload failed.");
     }
     return await s.text();
 }
 
-function Nc(t) {
+function Uc(t) {
     for (var e = t.split(","), n = e[0].match(/:(.*?);/)[1], i = atob(e[1]), o = i.length, r = new Uint8Array(o); o--;)
         r[o] = i.charCodeAt(o);
     return new Blob([r], {
         type: n
     });
 }
 const un = (t) => {
@@ -1748,40 +1748,40 @@
         n = Math.floor(t % 3600 / 60),
         i = Math.round(t) % 60,
         o = `${n < 10 ? "0" : ""}${n}`,
         r = `${i < 10 ? "0" : ""}${i}`;
     return e > 0 ? `${e}:${o}:${r}` : `${n}:${r}`;
 };
 const {
-    SvelteComponent: Ic,
-    assign: Uc,
-    create_slot: jc,
-    detach: Fc,
-    element: qc,
-    get_all_dirty_from_scope: zc,
-    get_slot_changes: Gc,
-    get_spread_update: Wc,
-    init: Vc,
-    insert: Xc,
-    safe_not_equal: xc,
+    SvelteComponent: jc,
+    assign: Fc,
+    create_slot: qc,
+    detach: zc,
+    element: Gc,
+    get_all_dirty_from_scope: Wc,
+    get_slot_changes: Vc,
+    get_spread_update: Xc,
+    init: xc,
+    insert: Zc,
+    safe_not_equal: Jc,
     set_dynamic_element_data: As,
     set_style: qe,
     toggle_class: dt,
     transition_in: Ha,
     transition_out: Oa,
-    update_slot_base: Zc
+    update_slot_base: Yc
 } = window.__gradio__svelte__internal;
 
-function Jc(t) {
+function Qc(t) {
     let e, n, i;
     const o = (
             /*#slots*/
             t[18].default
         ),
-        r = jc(
+        r = qc(
             o,
             t,
             /*$$scope*/
             t[17],
             null
         );
     let s = [{
@@ -1796,18 +1796,18 @@
             )
         }, {
             class: n = "block " + /*elem_classes*/
                 t[3].join(" ") + " svelte-nl1om8"
         }],
         a = {};
     for (let l = 0; l < s.length; l += 1)
-        a = Uc(a, s[l]);
+        a = Fc(a, s[l]);
     return {
         c() {
-            e = qc(
+            e = Gc(
                 /*tag*/
                 t[14]
             ), r && r.c(), As(
                 /*tag*/
                 t[14]
             )(e, a), dt(
                 e,
@@ -1861,39 +1861,39 @@
                 "flex-grow",
                 /*scale*/
                 t[12]
             ), qe(e, "min-width", `calc(min(${/*min_width*/
       t[13]}px, 100%))`), qe(e, "border-width", "var(--block-border-width)");
         },
         m(l, u) {
-            Xc(l, e, u), r && r.m(e, null), i = !0;
+            Zc(l, e, u), r && r.m(e, null), i = !0;
         },
         p(l, u) {
             r && r.p && (!i || u & /*$$scope*/
-                    131072) && Zc(
+                    131072) && Yc(
                     r,
                     o,
                     l,
                     /*$$scope*/
                     l[17],
-                    i ? Gc(
+                    i ? Vc(
                         o,
                         /*$$scope*/
                         l[17],
                         u,
                         null
-                    ) : zc(
+                    ) : Wc(
                         /*$$scope*/
                         l[17]
                     ),
                     null
                 ), As(
                     /*tag*/
                     l[14]
-                )(e, a = Wc(s, [
+                )(e, a = Xc(s, [
                     (!i || u & /*test_id*/
                         128) && {
                         "data-testid": (
                             /*test_id*/
                             l[7]
                         )
                     },
@@ -1973,23 +1973,23 @@
         i(l) {
             i || (Ha(r, l), i = !0);
         },
         o(l) {
             Oa(r, l), i = !1;
         },
         d(l) {
-            l && Fc(e), r && r.d(l);
+            l && zc(e), r && r.d(l);
         }
     };
 }
 
-function Yc(t) {
+function Kc(t) {
     let e, n = (
         /*tag*/
-        t[14] && Jc(t)
+        t[14] && Qc(t)
     );
     return {
         c() {
             n && n.c();
         },
         m(i, o) {
             n && n.m(i, o), e = !0;
@@ -2006,15 +2006,15 @@
         },
         d(i) {
             n && n.d(i);
         }
     };
 }
 
-function Qc(t, e, n) {
+function $c(t, e, n) {
     let {
         $$slots: i = {},
         $$scope: o
     } = e, {
         height: r = void 0
     } = e, {
         width: s = void 0
@@ -2033,57 +2033,57 @@
     } = e, {
         test_id: d = void 0
     } = e, {
         explicit_call: _ = !1
     } = e, {
         container: m = !0
     } = e, {
-        visible: v = !0
+        visible: b = !0
     } = e, {
-        allow_overflow: b = !0
+        allow_overflow: g = !0
     } = e, {
         scale: S = null
     } = e, {
         min_width: w = 0
     } = e, k = h === "fieldset" ? "fieldset" : "div";
     const E = (y) => {
         if (y !== void 0) {
             if (typeof y == "number")
                 return y + "px";
             if (typeof y == "string")
                 return y;
         }
     };
     return t.$$set = (y) => {
-        "height" in y && n(0, r = y.height), "width" in y && n(1, s = y.width), "elem_id" in y && n(2, a = y.elem_id), "elem_classes" in y && n(3, l = y.elem_classes), "variant" in y && n(4, u = y.variant), "border_mode" in y && n(5, c = y.border_mode), "padding" in y && n(6, f = y.padding), "type" in y && n(16, h = y.type), "test_id" in y && n(7, d = y.test_id), "explicit_call" in y && n(8, _ = y.explicit_call), "container" in y && n(9, m = y.container), "visible" in y && n(10, v = y.visible), "allow_overflow" in y && n(11, b = y.allow_overflow), "scale" in y && n(12, S = y.scale), "min_width" in y && n(13, w = y.min_width), "$$scope" in y && n(17, o = y.$$scope);
+        "height" in y && n(0, r = y.height), "width" in y && n(1, s = y.width), "elem_id" in y && n(2, a = y.elem_id), "elem_classes" in y && n(3, l = y.elem_classes), "variant" in y && n(4, u = y.variant), "border_mode" in y && n(5, c = y.border_mode), "padding" in y && n(6, f = y.padding), "type" in y && n(16, h = y.type), "test_id" in y && n(7, d = y.test_id), "explicit_call" in y && n(8, _ = y.explicit_call), "container" in y && n(9, m = y.container), "visible" in y && n(10, b = y.visible), "allow_overflow" in y && n(11, g = y.allow_overflow), "scale" in y && n(12, S = y.scale), "min_width" in y && n(13, w = y.min_width), "$$scope" in y && n(17, o = y.$$scope);
     }, [
         r,
         s,
         a,
         l,
         u,
         c,
         f,
         d,
         _,
         m,
-        v,
         b,
+        g,
         S,
         w,
         k,
         E,
         h,
         o,
         i
     ];
 }
-class Na extends Ic {
+class Na extends jc {
     constructor(e) {
-        super(), Vc(this, e, Qc, Yc, xc, {
+        super(), xc(this, e, $c, Kc, Jc, {
             height: 0,
             width: 1,
             elem_id: 2,
             elem_classes: 3,
             variant: 4,
             border_mode: 5,
             padding: 6,
@@ -2095,39 +2095,39 @@
             allow_overflow: 11,
             scale: 12,
             min_width: 13
         });
     }
 }
 const {
-    SvelteComponent: Kc,
+    SvelteComponent: ef,
     append: Uo,
     attr: Ii,
-    create_component: $c,
-    destroy_component: ef,
-    detach: tf,
+    create_component: tf,
+    destroy_component: nf,
+    detach: of,
     element: Ts,
-    init: nf,
-    insert: of,
-    mount_component: rf,
-    safe_not_equal: sf,
-    set_data: lf,
-    space: af,
-    text: uf,
+    init: rf,
+    insert: sf,
+    mount_component: lf,
+    safe_not_equal: af,
+    set_data: uf,
+    space: cf,
+    text: ff,
     toggle_class: Lt,
-    transition_in: cf,
-    transition_out: ff
+    transition_in: df,
+    transition_out: hf
 } = window.__gradio__svelte__internal;
 
-function df(t) {
+function _f(t) {
     let e, n, i, o, r, s;
     return i = new /*Icon*/
     t[1]({}), {
         c() {
-            e = Ts("label"), n = Ts("span"), $c(i.$$.fragment), o = af(), r = uf(
+            e = Ts("label"), n = Ts("span"), tf(i.$$.fragment), o = cf(), r = ff(
                 /*label*/
                 t[0]
             ), Ii(n, "class", "svelte-9gxdi0"), Ii(e, "for", ""), Ii(e, "data-testid", "block-label"), Ii(e, "class", "svelte-9gxdi0"), Lt(e, "hide", ! /*show_label*/
                 t[2]), Lt(e, "sr-only", ! /*show_label*/
                 t[2]), Lt(
                 e,
                 "float",
@@ -2137,19 +2137,19 @@
                 e,
                 "hide-label",
                 /*disable*/
                 t[3]
             );
         },
         m(a, l) {
-            of(a, e, l), Uo(e, n), rf(i, n, null), Uo(e, o), Uo(e, r), s = !0;
+            sf(a, e, l), Uo(e, n), lf(i, n, null), Uo(e, o), Uo(e, r), s = !0;
         },
         p(a, [l]) {
             (!s || l & /*label*/
-                1) && lf(
+                1) && uf(
                 r,
                 /*label*/
                 a[0]
             ), (!s || l & /*show_label*/
                 4) && Lt(e, "hide", ! /*show_label*/
                 a[2]), (!s || l & /*show_label*/
                 4) && Lt(e, "sr-only", ! /*show_label*/
@@ -2164,26 +2164,26 @@
                 e,
                 "hide-label",
                 /*disable*/
                 a[3]
             );
         },
         i(a) {
-            s || (cf(i.$$.fragment, a), s = !0);
+            s || (df(i.$$.fragment, a), s = !0);
         },
         o(a) {
-            ff(i.$$.fragment, a), s = !1;
+            hf(i.$$.fragment, a), s = !1;
         },
         d(a) {
-            a && tf(e), ef(i);
+            a && of(e), nf(i);
         }
     };
 }
 
-function hf(t, e, n) {
+function mf(t, e, n) {
     let {
         label: i = null
     } = e, {
         Icon: o
     } = e, {
         show_label: r = !0
     } = e, {
@@ -2191,83 +2191,83 @@
     } = e, {
         float: a = !0
     } = e;
     return t.$$set = (l) => {
         "label" in l && n(0, i = l.label), "Icon" in l && n(1, o = l.Icon), "show_label" in l && n(2, r = l.show_label), "disable" in l && n(3, s = l.disable), "float" in l && n(4, a = l.float);
     }, [i, o, r, s, a];
 }
-class Ia extends Kc {
+class Ia extends ef {
     constructor(e) {
-        super(), nf(this, e, hf, df, sf, {
+        super(), rf(this, e, mf, _f, af, {
             label: 0,
             Icon: 1,
             show_label: 2,
             disable: 3,
             float: 4
         });
     }
 }
 const {
-    SvelteComponent: _f,
+    SvelteComponent: pf,
     append: Br,
     attr: Et,
-    bubble: mf,
-    create_component: pf,
-    destroy_component: gf,
+    bubble: gf,
+    create_component: bf,
+    destroy_component: vf,
     detach: Ua,
     element: Mr,
-    init: bf,
+    init: wf,
     insert: ja,
-    listen: vf,
-    mount_component: wf,
-    safe_not_equal: yf,
-    set_data: kf,
+    listen: yf,
+    mount_component: kf,
+    safe_not_equal: Ef,
+    set_data: Cf,
     set_style: Ui,
-    space: Ef,
-    text: Cf,
+    space: Sf,
+    text: Af,
     toggle_class: Ge,
-    transition_in: Sf,
-    transition_out: Af
+    transition_in: Tf,
+    transition_out: Pf
 } = window.__gradio__svelte__internal;
 
 function Ps(t) {
     let e, n;
     return {
         c() {
-            e = Mr("span"), n = Cf(
+            e = Mr("span"), n = Af(
                 /*label*/
                 t[1]
             ), Et(e, "class", "svelte-lpi64a");
         },
         m(i, o) {
             ja(i, e, o), Br(e, n);
         },
         p(i, o) {
             o & /*label*/
-                2 && kf(
+                2 && Cf(
                     n,
                     /*label*/
                     i[1]
                 );
         },
         d(i) {
             i && Ua(e);
         }
     };
 }
 
-function Tf(t) {
+function Lf(t) {
     let e, n, i, o, r, s, a, l = (
         /*show_label*/
         t[2] && Ps(t)
     );
     return o = new /*Icon*/
     t[0]({}), {
         c() {
-            e = Mr("button"), l && l.c(), n = Ef(), i = Mr("div"), pf(o.$$.fragment), Et(i, "class", "svelte-lpi64a"), Ge(
+            e = Mr("button"), l && l.c(), n = Sf(), i = Mr("div"), bf(o.$$.fragment), Et(i, "class", "svelte-lpi64a"), Ge(
                     i,
                     "small",
                     /*size*/
                     t[4] === "small"
                 ), Ge(
                     i,
                     "large",
@@ -2317,15 +2317,15 @@
                     ) : "var(--block-label-text-color)"), Ui(e, "--bg-color", /*disabled*/
                     t[7] ? "auto" : (
                         /*background*/
                         t[10]
                     ));
         },
         m(u, c) {
-            ja(u, e, c), l && l.m(e, null), Br(e, n), Br(e, i), wf(o, i, null), r = !0, s || (a = vf(
+            ja(u, e, c), l && l.m(e, null), Br(e, n), Br(e, i), kf(o, i, null), r = !0, s || (a = yf(
                 e,
                 "click",
                 /*click_handler*/
                 t[13]
             ), s = !0);
         },
         p(u, [c]) {
@@ -2396,26 +2396,26 @@
                 1152 && Ui(e, "--bg-color", /*disabled*/
                     u[7] ? "auto" : (
                         /*background*/
                         u[10]
                     ));
         },
         i(u) {
-            r || (Sf(o.$$.fragment, u), r = !0);
+            r || (Tf(o.$$.fragment, u), r = !0);
         },
         o(u) {
-            Af(o.$$.fragment, u), r = !1;
+            Pf(o.$$.fragment, u), r = !1;
         },
         d(u) {
-            u && Ua(e), l && l.d(), gf(o), s = !1, a();
+            u && Ua(e), l && l.d(), vf(o), s = !1, a();
         }
     };
 }
 
-function Pf(t, e, n) {
+function Rf(t, e, n) {
     let i, {
             Icon: o
         } = e,
         {
             label: r = ""
         } = e,
         {
@@ -2445,19 +2445,19 @@
         {
             transparent: _ = !1
         } = e,
         {
             background: m = "var(--background-fill-primary)"
         } = e;
 
-    function v(b) {
-        mf.call(this, t, b);
+    function b(g) {
+        gf.call(this, t, g);
     }
-    return t.$$set = (b) => {
-        "Icon" in b && n(0, o = b.Icon), "label" in b && n(1, r = b.label), "show_label" in b && n(2, s = b.show_label), "pending" in b && n(3, a = b.pending), "size" in b && n(4, l = b.size), "padded" in b && n(5, u = b.padded), "highlight" in b && n(6, c = b.highlight), "disabled" in b && n(7, f = b.disabled), "hasPopup" in b && n(8, h = b.hasPopup), "color" in b && n(12, d = b.color), "transparent" in b && n(9, _ = b.transparent), "background" in b && n(10, m = b.background);
+    return t.$$set = (g) => {
+        "Icon" in g && n(0, o = g.Icon), "label" in g && n(1, r = g.label), "show_label" in g && n(2, s = g.show_label), "pending" in g && n(3, a = g.pending), "size" in g && n(4, l = g.size), "padded" in g && n(5, u = g.padded), "highlight" in g && n(6, c = g.highlight), "disabled" in g && n(7, f = g.disabled), "hasPopup" in g && n(8, h = g.hasPopup), "color" in g && n(12, d = g.color), "transparent" in g && n(9, _ = g.transparent), "background" in g && n(10, m = g.background);
     }, t.$$.update = () => {
         t.$$.dirty & /*highlight, color*/
             4160 && n(11, i = c ? "var(--color-accent)" : d);
     }, [
         o,
         r,
         s,
@@ -2467,20 +2467,20 @@
         c,
         f,
         h,
         _,
         m,
         i,
         d,
-        v
+        b
     ];
 }
-class Ei extends _f {
+class Ei extends pf {
     constructor(e) {
-        super(), bf(this, e, Pf, Tf, yf, {
+        super(), wf(this, e, Rf, Lf, Ef, {
             Icon: 0,
             label: 1,
             show_label: 2,
             pending: 3,
             size: 4,
             padded: 5,
             highlight: 6,
@@ -2489,39 +2489,39 @@
             color: 12,
             transparent: 9,
             background: 10
         });
     }
 }
 const {
-    SvelteComponent: Lf,
-    append: Rf,
+    SvelteComponent: Bf,
+    append: Mf,
     attr: jo,
-    binding_callbacks: Bf,
-    create_slot: Mf,
-    detach: Df,
+    binding_callbacks: Df,
+    create_slot: Hf,
+    detach: Of,
     element: Ls,
-    get_all_dirty_from_scope: Hf,
-    get_slot_changes: Of,
-    init: Nf,
-    insert: If,
-    safe_not_equal: Uf,
+    get_all_dirty_from_scope: Nf,
+    get_slot_changes: If,
+    init: Uf,
+    insert: jf,
+    safe_not_equal: Ff,
     toggle_class: Rt,
-    transition_in: jf,
-    transition_out: Ff,
-    update_slot_base: qf
+    transition_in: qf,
+    transition_out: zf,
+    update_slot_base: Gf
 } = window.__gradio__svelte__internal;
 
-function zf(t) {
+function Wf(t) {
     let e, n, i;
     const o = (
             /*#slots*/
             t[5].default
         ),
-        r = Mf(
+        r = Hf(
             o,
             t,
             /*$$scope*/
             t[4],
             null
         );
     return {
@@ -2545,31 +2545,31 @@
                 e,
                 "small_parent",
                 /*parent_height*/
                 t[3]
             );
         },
         m(s, a) {
-            If(s, e, a), Rf(e, n), r && r.m(n, null), t[6](e), i = !0;
+            jf(s, e, a), Mf(e, n), r && r.m(n, null), t[6](e), i = !0;
         },
         p(s, [a]) {
             r && r.p && (!i || a & /*$$scope*/
-                16) && qf(
+                16) && Gf(
                 r,
                 o,
                 s,
                 /*$$scope*/
                 s[4],
-                i ? Of(
+                i ? If(
                     o,
                     /*$$scope*/
                     s[4],
                     a,
                     null
-                ) : Hf(
+                ) : Nf(
                     /*$$scope*/
                     s[4]
                 ),
                 null
             ), (!i || a & /*size*/
                 1) && Rt(
                 e,
@@ -2593,39 +2593,39 @@
                 e,
                 "small_parent",
                 /*parent_height*/
                 s[3]
             );
         },
         i(s) {
-            i || (jf(r, s), i = !0);
+            i || (qf(r, s), i = !0);
         },
         o(s) {
-            Ff(r, s), i = !1;
+            zf(r, s), i = !1;
         },
         d(s) {
-            s && Df(e), r && r.d(s), t[6](null);
+            s && Of(e), r && r.d(s), t[6](null);
         }
     };
 }
 
-function Gf(t) {
+function Vf(t) {
     let e, n = t[0],
         i = 1;
     for (; i < t.length;) {
         const o = t[i],
             r = t[i + 1];
         if (i += 2, (o === "optionalAccess" || o === "optionalCall") && n == null)
             return;
         o === "access" || o === "optionalAccess" ? (e = n, n = r(n)) : (o === "call" || o === "optionalCall") && (n = r((...s) => n.call(e, ...s)), e = void 0);
     }
     return n;
 }
 
-function Wf(t, e, n) {
+function Xf(t, e, n) {
     let i, {
             $$slots: o = {},
             $$scope: r
         } = e,
         {
             size: s = "small"
         } = e,
@@ -2637,653 +2637,653 @@
     function u(f) {
         if (!f)
             return !1;
         const {
             height: h
         } = f.getBoundingClientRect(), {
             height: d
-        } = Gf([
+        } = Vf([
             f,
             "access",
             (_) => _.parentElement,
             "optionalAccess",
             (_) => _.getBoundingClientRect,
             "call",
             (_) => _()
         ]) || {
             height: h
         };
         return h > d + 2;
     }
 
     function c(f) {
-        Bf[f ? "unshift" : "push"](() => {
+        Df[f ? "unshift" : "push"](() => {
             l = f, n(2, l);
         });
     }
     return t.$$set = (f) => {
         "size" in f && n(0, s = f.size), "unpadded_box" in f && n(1, a = f.unpadded_box), "$$scope" in f && n(4, r = f.$$scope);
     }, t.$$.update = () => {
         t.$$.dirty & /*el*/
             4 && n(3, i = u(l));
     }, [s, a, l, i, r, o, c];
 }
-class Fa extends Lf {
+class Fa extends Bf {
     constructor(e) {
-        super(), Nf(this, e, Wf, zf, Uf, {
+        super(), Uf(this, e, Xf, Wf, Ff, {
             size: 0,
             unpadded_box: 1
         });
     }
 }
 const {
-    SvelteComponent: Vf,
-    append: Xf,
+    SvelteComponent: xf,
+    append: Zf,
     attr: We,
-    detach: xf,
-    init: Zf,
-    insert: Jf,
+    detach: Jf,
+    init: Yf,
+    insert: Qf,
     noop: Fo,
-    safe_not_equal: Yf,
+    safe_not_equal: Kf,
     svg_element: Rs
 } = window.__gradio__svelte__internal;
 
-function Qf(t) {
+function $f(t) {
     let e, n;
     return {
         c() {
             e = Rs("svg"), n = Rs("path"), We(n, "stroke", "currentColor"), We(n, "stroke-width", "1.5"), We(n, "stroke-linecap", "round"), We(n, "stroke-linejoin", "round"), We(n, "d", "M21.044 5.704a.6.6 0 0 1 .956.483v11.626a.6.6 0 0 1-.956.483l-7.889-5.813a.6.6 0 0 1 0-.966l7.89-5.813ZM10.044 5.704a.6.6 0 0 1 .956.483v11.626a.6.6 0 0 1-.956.483l-7.888-5.813a.6.6 0 0 1 0-.966l7.888-5.813Z"), We(e, "xmlns", "http://www.w3.org/2000/svg"), We(e, "width", "24px"), We(e, "height", "24px"), We(e, "fill", "currentColor"), We(e, "stroke-width", "1.5"), We(e, "viewBox", "0 0 24 24"), We(e, "color", "currentColor");
         },
         m(i, o) {
-            Jf(i, e, o), Xf(e, n);
+            Qf(i, e, o), Zf(e, n);
         },
         p: Fo,
         i: Fo,
         o: Fo,
         d(i) {
-            i && xf(e);
+            i && Jf(e);
         }
     };
 }
-class Kf extends Vf {
+class ed extends xf {
     constructor(e) {
-        super(), Zf(this, e, null, Qf, Yf, {});
+        super(), Yf(this, e, null, $f, Kf, {});
     }
 }
 const {
-    SvelteComponent: $f,
+    SvelteComponent: td,
     append: qo,
     attr: et,
-    detach: ed,
-    init: td,
-    insert: nd,
+    detach: nd,
+    init: id,
+    insert: od,
     noop: zo,
-    safe_not_equal: id,
+    safe_not_equal: rd,
     set_style: ht,
     svg_element: ji
 } = window.__gradio__svelte__internal;
 
-function od(t) {
+function sd(t) {
     let e, n, i, o;
     return {
         c() {
             e = ji("svg"), n = ji("g"), i = ji("path"), o = ji("path"), et(i, "d", "M18,6L6.087,17.913"), ht(i, "fill", "none"), ht(i, "fill-rule", "nonzero"), ht(i, "stroke-width", "2px"), et(n, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), et(o, "d", "M4.364,4.364L19.636,19.636"), ht(o, "fill", "none"), ht(o, "fill-rule", "nonzero"), ht(o, "stroke-width", "2px"), et(e, "width", "100%"), et(e, "height", "100%"), et(e, "viewBox", "0 0 24 24"), et(e, "version", "1.1"), et(e, "xmlns", "http://www.w3.org/2000/svg"), et(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), et(e, "xml:space", "preserve"), et(e, "stroke", "currentColor"), ht(e, "fill-rule", "evenodd"), ht(e, "clip-rule", "evenodd"), ht(e, "stroke-linecap", "round"), ht(e, "stroke-linejoin", "round");
         },
         m(r, s) {
-            nd(r, e, s), qo(e, n), qo(n, i), qo(e, o);
+            od(r, e, s), qo(e, n), qo(n, i), qo(e, o);
         },
         p: zo,
         i: zo,
         o: zo,
         d(r) {
-            r && ed(e);
+            r && nd(e);
         }
     };
 }
-class rd extends $f {
+class ld extends td {
     constructor(e) {
-        super(), td(this, e, null, od, id, {});
+        super(), id(this, e, null, sd, rd, {});
     }
 }
 const {
-    SvelteComponent: sd,
-    append: ld,
+    SvelteComponent: ad,
+    append: ud,
     attr: yn,
-    detach: ad,
-    init: ud,
-    insert: cd,
+    detach: cd,
+    init: fd,
+    insert: dd,
     noop: Go,
-    safe_not_equal: fd,
+    safe_not_equal: hd,
     svg_element: Bs
 } = window.__gradio__svelte__internal;
 
-function dd(t) {
+function _d(t) {
     let e, n;
     return {
         c() {
             e = Bs("svg"), n = Bs("path"), yn(n, "fill", "currentColor"), yn(n, "d", "M26 24v4H6v-4H4v4a2 2 0 0 0 2 2h20a2 2 0 0 0 2-2v-4zm0-10l-1.41-1.41L17 20.17V2h-2v18.17l-7.59-7.58L6 14l10 10l10-10z"), yn(e, "xmlns", "http://www.w3.org/2000/svg"), yn(e, "width", "100%"), yn(e, "height", "100%"), yn(e, "viewBox", "0 0 32 32");
         },
         m(i, o) {
-            cd(i, e, o), ld(e, n);
+            dd(i, e, o), ud(e, n);
         },
         p: Go,
         i: Go,
         o: Go,
         d(i) {
-            i && ad(e);
+            i && cd(e);
         }
     };
 }
-class qa extends sd {
+class qa extends ad {
     constructor(e) {
-        super(), ud(this, e, null, dd, fd, {});
+        super(), fd(this, e, null, _d, hd, {});
     }
 }
 const {
-    SvelteComponent: hd,
-    append: _d,
+    SvelteComponent: md,
+    append: pd,
     attr: tt,
-    detach: md,
-    init: pd,
-    insert: gd,
+    detach: gd,
+    init: bd,
+    insert: vd,
     noop: Wo,
-    safe_not_equal: bd,
+    safe_not_equal: wd,
     svg_element: Ms
 } = window.__gradio__svelte__internal;
 
-function vd(t) {
+function yd(t) {
     let e, n;
     return {
         c() {
             e = Ms("svg"), n = Ms("path"), tt(n, "d", "M17 3a2.828 2.828 0 1 1 4 4L7.5 20.5 2 22l1.5-5.5L17 3z"), tt(e, "xmlns", "http://www.w3.org/2000/svg"), tt(e, "width", "100%"), tt(e, "height", "100%"), tt(e, "viewBox", "0 0 24 24"), tt(e, "fill", "none"), tt(e, "stroke", "currentColor"), tt(e, "stroke-width", "1.5"), tt(e, "stroke-linecap", "round"), tt(e, "stroke-linejoin", "round"), tt(e, "class", "feather feather-edit-2");
         },
         m(i, o) {
-            gd(i, e, o), _d(e, n);
+            vd(i, e, o), pd(e, n);
         },
         p: Wo,
         i: Wo,
         o: Wo,
         d(i) {
-            i && md(e);
+            i && gd(e);
         }
     };
 }
-class wd extends hd {
+class kd extends md {
     constructor(e) {
-        super(), pd(this, e, null, vd, bd, {});
+        super(), bd(this, e, null, yd, wd, {});
     }
 }
 const {
-    SvelteComponent: yd,
-    append: kd,
+    SvelteComponent: Ed,
+    append: Cd,
     attr: Ve,
-    detach: Ed,
-    init: Cd,
-    insert: Sd,
+    detach: Sd,
+    init: Ad,
+    insert: Td,
     noop: Vo,
-    safe_not_equal: Ad,
+    safe_not_equal: Pd,
     svg_element: Ds
 } = window.__gradio__svelte__internal;
 
-function Td(t) {
+function Ld(t) {
     let e, n;
     return {
         c() {
             e = Ds("svg"), n = Ds("path"), Ve(n, "stroke", "currentColor"), Ve(n, "stroke-width", "1.5"), Ve(n, "stroke-linecap", "round"), Ve(n, "stroke-linejoin", "round"), Ve(n, "d", "M2.956 5.704A.6.6 0 0 0 2 6.187v11.626a.6.6 0 0 0 .956.483l7.889-5.813a.6.6 0 0 0 0-.966l-7.89-5.813ZM13.956 5.704a.6.6 0 0 0-.956.483v11.626a.6.6 0 0 0 .956.483l7.889-5.813a.6.6 0 0 0 0-.966l-7.89-5.813Z"), Ve(e, "xmlns", "http://www.w3.org/2000/svg"), Ve(e, "width", "24px"), Ve(e, "height", "24px"), Ve(e, "fill", "currentColor"), Ve(e, "stroke-width", "1.5"), Ve(e, "viewBox", "0 0 24 24"), Ve(e, "color", "currentColor");
         },
         m(i, o) {
-            Sd(i, e, o), kd(e, n);
+            Td(i, e, o), Cd(e, n);
         },
         p: Vo,
         i: Vo,
         o: Vo,
         d(i) {
-            i && Ed(e);
+            i && Sd(e);
         }
     };
 }
-class Pd extends yd {
+class Rd extends Ed {
     constructor(e) {
-        super(), Cd(this, e, null, Td, Ad, {});
+        super(), Ad(this, e, null, Ld, Pd, {});
     }
 }
 const {
-    SvelteComponent: Ld,
-    append: Rd,
+    SvelteComponent: Bd,
+    append: Md,
     attr: kn,
-    detach: Bd,
-    init: Md,
-    insert: Dd,
+    detach: Dd,
+    init: Hd,
+    insert: Od,
     noop: Xo,
-    safe_not_equal: Hd,
+    safe_not_equal: Nd,
     svg_element: Hs
 } = window.__gradio__svelte__internal;
 
-function Od(t) {
+function Id(t) {
     let e, n;
     return {
         c() {
             e = Hs("svg"), n = Hs("path"), kn(n, "fill", "currentColor"), kn(n, "d", "M13.75 2a2.25 2.25 0 0 1 2.236 2.002V4h1.764A2.25 2.25 0 0 1 20 6.25V11h-1.5V6.25a.75.75 0 0 0-.75-.75h-2.129c-.404.603-1.091 1-1.871 1h-3.5c-.78 0-1.467-.397-1.871-1H6.25a.75.75 0 0 0-.75.75v13.5c0 .414.336.75.75.75h4.78a3.99 3.99 0 0 0 .505 1.5H6.25A2.25 2.25 0 0 1 4 19.75V6.25A2.25 2.25 0 0 1 6.25 4h1.764a2.25 2.25 0 0 1 2.236-2h3.5Zm2.245 2.096L16 4.25c0-.052-.002-.103-.005-.154ZM13.75 3.5h-3.5a.75.75 0 0 0 0 1.5h3.5a.75.75 0 0 0 0-1.5ZM15 12a3 3 0 0 0-3 3v5c0 .556.151 1.077.415 1.524l3.494-3.494a2.25 2.25 0 0 1 3.182 0l3.494 3.494c.264-.447.415-.968.415-1.524v-5a3 3 0 0 0-3-3h-5Zm0 11a2.985 2.985 0 0 1-1.524-.415l3.494-3.494a.75.75 0 0 1 1.06 0l3.494 3.494A2.985 2.985 0 0 1 20 23h-5Zm5-7a1 1 0 1 1 0-2a1 1 0 0 1 0 2Z"), kn(e, "xmlns", "http://www.w3.org/2000/svg"), kn(e, "width", "100%"), kn(e, "height", "100%"), kn(e, "viewBox", "0 0 24 24");
         },
         m(i, o) {
-            Dd(i, e, o), Rd(e, n);
+            Od(i, e, o), Md(e, n);
         },
         p: Xo,
         i: Xo,
         o: Xo,
         d(i) {
-            i && Bd(e);
+            i && Dd(e);
         }
     };
 }
-class za extends Ld {
+class za extends Bd {
     constructor(e) {
-        super(), Md(this, e, null, Od, Hd, {});
+        super(), Hd(this, e, null, Id, Nd, {});
     }
 }
 const {
-    SvelteComponent: Nd,
+    SvelteComponent: Ud,
     append: Fi,
     attr: me,
-    detach: Id,
-    init: Ud,
-    insert: jd,
+    detach: jd,
+    init: Fd,
+    insert: qd,
     noop: xo,
-    safe_not_equal: Fd,
-    svg_element: ni
+    safe_not_equal: zd,
+    svg_element: ii
 } = window.__gradio__svelte__internal;
 
-function qd(t) {
+function Gd(t) {
     let e, n, i, o, r;
     return {
         c() {
-            e = ni("svg"), n = ni("path"), i = ni("path"), o = ni("line"), r = ni("line"), me(n, "d", "M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"), me(i, "d", "M19 10v2a7 7 0 0 1-14 0v-2"), me(o, "x1", "12"), me(o, "y1", "19"), me(o, "x2", "12"), me(o, "y2", "23"), me(r, "x1", "8"), me(r, "y1", "23"), me(r, "x2", "16"), me(r, "y2", "23"), me(e, "xmlns", "http://www.w3.org/2000/svg"), me(e, "width", "100%"), me(e, "height", "100%"), me(e, "viewBox", "0 0 24 24"), me(e, "fill", "none"), me(e, "stroke", "currentColor"), me(e, "stroke-width", "2"), me(e, "stroke-linecap", "round"), me(e, "stroke-linejoin", "round"), me(e, "class", "feather feather-mic");
+            e = ii("svg"), n = ii("path"), i = ii("path"), o = ii("line"), r = ii("line"), me(n, "d", "M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"), me(i, "d", "M19 10v2a7 7 0 0 1-14 0v-2"), me(o, "x1", "12"), me(o, "y1", "19"), me(o, "x2", "12"), me(o, "y2", "23"), me(r, "x1", "8"), me(r, "y1", "23"), me(r, "x2", "16"), me(r, "y2", "23"), me(e, "xmlns", "http://www.w3.org/2000/svg"), me(e, "width", "100%"), me(e, "height", "100%"), me(e, "viewBox", "0 0 24 24"), me(e, "fill", "none"), me(e, "stroke", "currentColor"), me(e, "stroke-width", "2"), me(e, "stroke-linecap", "round"), me(e, "stroke-linejoin", "round"), me(e, "class", "feather feather-mic");
         },
         m(s, a) {
-            jd(s, e, a), Fi(e, n), Fi(e, i), Fi(e, o), Fi(e, r);
+            qd(s, e, a), Fi(e, n), Fi(e, i), Fi(e, o), Fi(e, r);
         },
         p: xo,
         i: xo,
         o: xo,
         d(s) {
-            s && Id(e);
+            s && jd(e);
         }
     };
 }
-class zd extends Nd {
+class Wd extends Ud {
     constructor(e) {
-        super(), Ud(this, e, null, qd, Fd, {});
+        super(), Fd(this, e, null, Gd, zd, {});
     }
 }
 const {
-    SvelteComponent: Gd,
+    SvelteComponent: Vd,
     append: Zo,
     attr: Pe,
-    detach: Wd,
-    init: Vd,
-    insert: Xd,
+    detach: Xd,
+    init: xd,
+    insert: Zd,
     noop: Jo,
-    safe_not_equal: xd,
+    safe_not_equal: Jd,
     svg_element: qi
 } = window.__gradio__svelte__internal;
 
-function Zd(t) {
+function Yd(t) {
     let e, n, i, o;
     return {
         c() {
             e = qi("svg"), n = qi("path"), i = qi("circle"), o = qi("circle"), Pe(n, "d", "M9 18V5l12-2v13"), Pe(i, "cx", "6"), Pe(i, "cy", "18"), Pe(i, "r", "3"), Pe(o, "cx", "18"), Pe(o, "cy", "16"), Pe(o, "r", "3"), Pe(e, "xmlns", "http://www.w3.org/2000/svg"), Pe(e, "width", "100%"), Pe(e, "height", "100%"), Pe(e, "viewBox", "0 0 24 24"), Pe(e, "fill", "none"), Pe(e, "stroke", "currentColor"), Pe(e, "stroke-width", "1.5"), Pe(e, "stroke-linecap", "round"), Pe(e, "stroke-linejoin", "round"), Pe(e, "class", "feather feather-music");
         },
         m(r, s) {
-            Xd(r, e, s), Zo(e, n), Zo(e, i), Zo(e, o);
+            Zd(r, e, s), Zo(e, n), Zo(e, i), Zo(e, o);
         },
         p: Jo,
         i: Jo,
         o: Jo,
         d(r) {
-            r && Wd(e);
+            r && Xd(e);
         }
     };
 }
-class mo extends Gd {
+class mo extends Vd {
     constructor(e) {
-        super(), Vd(this, e, null, Zd, xd, {});
+        super(), xd(this, e, null, Yd, Jd, {});
     }
 }
 const {
-    SvelteComponent: Jd,
+    SvelteComponent: Qd,
     append: Os,
     attr: Le,
-    detach: Yd,
-    init: Qd,
-    insert: Kd,
+    detach: Kd,
+    init: $d,
+    insert: eh,
     noop: Yo,
-    safe_not_equal: $d,
+    safe_not_equal: th,
     svg_element: Qo
 } = window.__gradio__svelte__internal;
 
-function eh(t) {
+function nh(t) {
     let e, n, i;
     return {
         c() {
             e = Qo("svg"), n = Qo("rect"), i = Qo("rect"), Le(n, "x", "6"), Le(n, "y", "4"), Le(n, "width", "4"), Le(n, "height", "16"), Le(i, "x", "14"), Le(i, "y", "4"), Le(i, "width", "4"), Le(i, "height", "16"), Le(e, "xmlns", "http://www.w3.org/2000/svg"), Le(e, "width", "100%"), Le(e, "height", "100%"), Le(e, "viewBox", "0 0 24 24"), Le(e, "fill", "currentColor"), Le(e, "stroke", "currentColor"), Le(e, "stroke-width", "1.5"), Le(e, "stroke-linecap", "round"), Le(e, "stroke-linejoin", "round");
         },
         m(o, r) {
-            Kd(o, e, r), Os(e, n), Os(e, i);
+            eh(o, e, r), Os(e, n), Os(e, i);
         },
         p: Yo,
         i: Yo,
         o: Yo,
         d(o) {
-            o && Yd(e);
+            o && Kd(e);
         }
     };
 }
-class Ga extends Jd {
+class Ga extends Qd {
     constructor(e) {
-        super(), Qd(this, e, null, eh, $d, {});
+        super(), $d(this, e, null, nh, th, {});
     }
 }
 const {
-    SvelteComponent: th,
-    append: nh,
+    SvelteComponent: ih,
+    append: oh,
     attr: _t,
-    detach: ih,
-    init: oh,
-    insert: rh,
+    detach: rh,
+    init: sh,
+    insert: lh,
     noop: Ko,
-    safe_not_equal: sh,
+    safe_not_equal: ah,
     svg_element: Ns
 } = window.__gradio__svelte__internal;
 
-function lh(t) {
+function uh(t) {
     let e, n;
     return {
         c() {
             e = Ns("svg"), n = Ns("polygon"), _t(n, "points", "5 3 19 12 5 21 5 3"), _t(e, "xmlns", "http://www.w3.org/2000/svg"), _t(e, "width", "100%"), _t(e, "height", "100%"), _t(e, "viewBox", "0 0 24 24"), _t(e, "fill", "currentColor"), _t(e, "stroke", "currentColor"), _t(e, "stroke-width", "1.5"), _t(e, "stroke-linecap", "round"), _t(e, "stroke-linejoin", "round");
         },
         m(i, o) {
-            rh(i, e, o), nh(e, n);
+            lh(i, e, o), oh(e, n);
         },
         p: Ko,
         i: Ko,
         o: Ko,
         d(i) {
-            i && ih(e);
+            i && rh(e);
         }
     };
 }
-class ah extends th {
+class ch extends ih {
     constructor(e) {
-        super(), oh(this, e, null, lh, sh, {});
+        super(), sh(this, e, null, uh, ah, {});
     }
 }
 const {
-    SvelteComponent: uh,
-    append: ii,
-    attr: se,
-    detach: ch,
-    init: fh,
-    insert: dh,
+    SvelteComponent: fh,
+    append: oi,
+    attr: re,
+    detach: dh,
+    init: hh,
+    insert: _h,
     noop: $o,
-    safe_not_equal: hh,
+    safe_not_equal: mh,
     svg_element: En
 } = window.__gradio__svelte__internal;
 
-function _h(t) {
+function ph(t) {
     let e, n, i, o, r, s;
     return {
         c() {
-            e = En("svg"), n = En("circle"), i = En("circle"), o = En("line"), r = En("line"), s = En("line"), se(n, "cx", "6"), se(n, "cy", "6"), se(n, "r", "3"), se(i, "cx", "6"), se(i, "cy", "18"), se(i, "r", "3"), se(o, "x1", "20"), se(o, "y1", "4"), se(o, "x2", "8.12"), se(o, "y2", "15.88"), se(r, "x1", "14.47"), se(r, "y1", "14.48"), se(r, "x2", "20"), se(r, "y2", "20"), se(s, "x1", "8.12"), se(s, "y1", "8.12"), se(s, "x2", "12"), se(s, "y2", "12"), se(e, "xmlns", "http://www.w3.org/2000/svg"), se(e, "width", "100%"), se(e, "height", "100%"), se(e, "viewBox", "0 0 24 24"), se(e, "fill", "none"), se(e, "stroke", "currentColor"), se(e, "stroke-width", "2"), se(e, "stroke-linecap", "round"), se(e, "stroke-linejoin", "round"), se(e, "class", "feather feather-scissors");
+            e = En("svg"), n = En("circle"), i = En("circle"), o = En("line"), r = En("line"), s = En("line"), re(n, "cx", "6"), re(n, "cy", "6"), re(n, "r", "3"), re(i, "cx", "6"), re(i, "cy", "18"), re(i, "r", "3"), re(o, "x1", "20"), re(o, "y1", "4"), re(o, "x2", "8.12"), re(o, "y2", "15.88"), re(r, "x1", "14.47"), re(r, "y1", "14.48"), re(r, "x2", "20"), re(r, "y2", "20"), re(s, "x1", "8.12"), re(s, "y1", "8.12"), re(s, "x2", "12"), re(s, "y2", "12"), re(e, "xmlns", "http://www.w3.org/2000/svg"), re(e, "width", "100%"), re(e, "height", "100%"), re(e, "viewBox", "0 0 24 24"), re(e, "fill", "none"), re(e, "stroke", "currentColor"), re(e, "stroke-width", "2"), re(e, "stroke-linecap", "round"), re(e, "stroke-linejoin", "round"), re(e, "class", "feather feather-scissors");
         },
         m(a, l) {
-            dh(a, e, l), ii(e, n), ii(e, i), ii(e, o), ii(e, r), ii(e, s);
+            _h(a, e, l), oi(e, n), oi(e, i), oi(e, o), oi(e, r), oi(e, s);
         },
         p: $o,
         i: $o,
         o: $o,
         d(a) {
-            a && ch(e);
+            a && dh(e);
         }
     };
 }
-class mh extends uh {
+class gh extends fh {
     constructor(e) {
-        super(), fh(this, e, null, _h, hh, {});
+        super(), hh(this, e, null, ph, mh, {});
     }
 }
 const {
-    SvelteComponent: ph,
+    SvelteComponent: bh,
     append: Is,
     attr: Xe,
-    detach: gh,
-    init: bh,
-    insert: vh,
+    detach: vh,
+    init: wh,
+    insert: yh,
     noop: er,
-    safe_not_equal: wh,
+    safe_not_equal: kh,
     svg_element: tr
 } = window.__gradio__svelte__internal;
 
-function yh(t) {
+function Eh(t) {
     let e, n, i;
     return {
         c() {
             e = tr("svg"), n = tr("polyline"), i = tr("path"), Xe(n, "points", "1 4 1 10 7 10"), Xe(i, "d", "M3.51 15a9 9 0 1 0 2.13-9.36L1 10"), Xe(e, "xmlns", "http://www.w3.org/2000/svg"), Xe(e, "width", "100%"), Xe(e, "height", "100%"), Xe(e, "viewBox", "0 0 24 24"), Xe(e, "fill", "none"), Xe(e, "stroke", "currentColor"), Xe(e, "stroke-width", "2"), Xe(e, "stroke-linecap", "round"), Xe(e, "stroke-linejoin", "round"), Xe(e, "class", "feather feather-rotate-ccw");
         },
         m(o, r) {
-            vh(o, e, r), Is(e, n), Is(e, i);
+            yh(o, e, r), Is(e, n), Is(e, i);
         },
         p: er,
         i: er,
         o: er,
         d(o) {
-            o && gh(e);
+            o && vh(e);
         }
     };
 }
-class Wa extends ph {
+class Wa extends bh {
     constructor(e) {
-        super(), bh(this, e, null, yh, wh, {});
+        super(), wh(this, e, null, Eh, kh, {});
     }
 }
 const {
-    SvelteComponent: kh,
+    SvelteComponent: Ch,
     append: nr,
     attr: Re,
-    detach: Eh,
-    init: Ch,
-    insert: Sh,
+    detach: Sh,
+    init: Ah,
+    insert: Th,
     noop: ir,
-    safe_not_equal: Ah,
+    safe_not_equal: Ph,
     svg_element: zi
 } = window.__gradio__svelte__internal;
 
-function Th(t) {
+function Lh(t) {
     let e, n, i, o;
     return {
         c() {
             e = zi("svg"), n = zi("path"), i = zi("polyline"), o = zi("line"), Re(n, "d", "M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"), Re(i, "points", "17 8 12 3 7 8"), Re(o, "x1", "12"), Re(o, "y1", "3"), Re(o, "x2", "12"), Re(o, "y2", "15"), Re(e, "xmlns", "http://www.w3.org/2000/svg"), Re(e, "width", "90%"), Re(e, "height", "90%"), Re(e, "viewBox", "0 0 24 24"), Re(e, "fill", "none"), Re(e, "stroke", "currentColor"), Re(e, "stroke-width", "2"), Re(e, "stroke-linecap", "round"), Re(e, "stroke-linejoin", "round"), Re(e, "class", "feather feather-upload");
         },
         m(r, s) {
-            Sh(r, e, s), nr(e, n), nr(e, i), nr(e, o);
+            Th(r, e, s), nr(e, n), nr(e, i), nr(e, o);
         },
         p: ir,
         i: ir,
         o: ir,
         d(r) {
-            r && Eh(e);
+            r && Sh(e);
         }
     };
 }
-let Va = class extends kh {
+let Va = class extends Ch {
     constructor(e) {
-        super(), Ch(this, e, null, Th, Ah, {});
+        super(), Ah(this, e, null, Lh, Ph, {});
     }
 };
 const {
-    SvelteComponent: Ph,
+    SvelteComponent: Rh,
     append: Gi,
     attr: Ne,
-    detach: Lh,
-    init: Rh,
-    insert: Bh,
+    detach: Bh,
+    init: Mh,
+    insert: Dh,
     noop: or,
-    safe_not_equal: Mh,
+    safe_not_equal: Hh,
     svg_element: Wi,
-    text: Dh
+    text: Oh
 } = window.__gradio__svelte__internal;
 
-function Hh(t) {
+function Nh(t) {
     let e, n, i, o, r;
     return {
         c() {
-            e = Wi("svg"), n = Wi("title"), i = Dh("Low volume"), o = Wi("path"), r = Wi("path"), Ne(o, "d", "M19.5 7.5C19.5 7.5 21 9 21 11.5C21 14 19.5 15.5 19.5 15.5"), Ne(o, "stroke-width", "1.5"), Ne(o, "stroke-linecap", "round"), Ne(o, "stroke-linejoin", "round"), Ne(r, "d", "M2 13.8571V10.1429C2 9.03829 2.89543 8.14286 4 8.14286H6.9C7.09569 8.14286 7.28708 8.08544 7.45046 7.97772L13.4495 4.02228C14.1144 3.5839 15 4.06075 15 4.85714V19.1429C15 19.9392 14.1144 20.4161 13.4495 19.9777L7.45046 16.0223C7.28708 15.9146 7.09569 15.8571 6.9 15.8571H4C2.89543 15.8571 2 14.9617 2 13.8571Z"), Ne(r, "stroke-width", "1.5"), Ne(e, "width", "100%"), Ne(e, "height", "100%"), Ne(e, "viewBox", "0 0 24 24"), Ne(e, "stroke-width", "1.5"), Ne(e, "fill", "none"), Ne(e, "xmlns", "http://www.w3.org/2000/svg"), Ne(e, "stroke", "currentColor"), Ne(e, "color", "currentColor");
+            e = Wi("svg"), n = Wi("title"), i = Oh("Low volume"), o = Wi("path"), r = Wi("path"), Ne(o, "d", "M19.5 7.5C19.5 7.5 21 9 21 11.5C21 14 19.5 15.5 19.5 15.5"), Ne(o, "stroke-width", "1.5"), Ne(o, "stroke-linecap", "round"), Ne(o, "stroke-linejoin", "round"), Ne(r, "d", "M2 13.8571V10.1429C2 9.03829 2.89543 8.14286 4 8.14286H6.9C7.09569 8.14286 7.28708 8.08544 7.45046 7.97772L13.4495 4.02228C14.1144 3.5839 15 4.06075 15 4.85714V19.1429C15 19.9392 14.1144 20.4161 13.4495 19.9777L7.45046 16.0223C7.28708 15.9146 7.09569 15.8571 6.9 15.8571H4C2.89543 15.8571 2 14.9617 2 13.8571Z"), Ne(r, "stroke-width", "1.5"), Ne(e, "width", "100%"), Ne(e, "height", "100%"), Ne(e, "viewBox", "0 0 24 24"), Ne(e, "stroke-width", "1.5"), Ne(e, "fill", "none"), Ne(e, "xmlns", "http://www.w3.org/2000/svg"), Ne(e, "stroke", "currentColor"), Ne(e, "color", "currentColor");
         },
         m(s, a) {
-            Bh(s, e, a), Gi(e, n), Gi(n, i), Gi(e, o), Gi(e, r);
+            Dh(s, e, a), Gi(e, n), Gi(n, i), Gi(e, o), Gi(e, r);
         },
         p: or,
         i: or,
         o: or,
         d(s) {
-            s && Lh(e);
+            s && Bh(e);
         }
     };
 }
-class Oh extends Ph {
+class Ih extends Rh {
     constructor(e) {
-        super(), Rh(this, e, null, Hh, Mh, {});
+        super(), Mh(this, e, null, Nh, Hh, {});
     }
 }
 const {
-    SvelteComponent: Nh,
-    append: oi,
+    SvelteComponent: Uh,
+    append: ri,
     attr: Ae,
-    detach: Ih,
-    init: Uh,
-    insert: jh,
+    detach: jh,
+    init: Fh,
+    insert: qh,
     noop: rr,
-    safe_not_equal: Fh,
-    svg_element: ri,
-    text: qh
+    safe_not_equal: zh,
+    svg_element: si,
+    text: Gh
 } = window.__gradio__svelte__internal;
 
-function zh(t) {
+function Wh(t) {
     let e, n, i, o, r, s;
     return {
         c() {
-            e = ri("svg"), n = ri("title"), i = qh("High volume"), o = ri("path"), r = ri("path"), s = ri("path"), Ae(o, "d", "M1 13.8571V10.1429C1 9.03829 1.89543 8.14286 3 8.14286H5.9C6.09569 8.14286 6.28708 8.08544 6.45046 7.97772L12.4495 4.02228C13.1144 3.5839 14 4.06075 14 4.85714V19.1429C14 19.9392 13.1144 20.4161 12.4495 19.9777L6.45046 16.0223C6.28708 15.9146 6.09569 15.8571 5.9 15.8571H3C1.89543 15.8571 1 14.9617 1 13.8571Z"), Ae(o, "stroke-width", "1.5"), Ae(r, "d", "M17.5 7.5C17.5 7.5 19 9 19 11.5C19 14 17.5 15.5 17.5 15.5"), Ae(r, "stroke-width", "1.5"), Ae(r, "stroke-linecap", "round"), Ae(r, "stroke-linejoin", "round"), Ae(s, "d", "M20.5 4.5C20.5 4.5 23 7 23 11.5C23 16 20.5 18.5 20.5 18.5"), Ae(s, "stroke-width", "1.5"), Ae(s, "stroke-linecap", "round"), Ae(s, "stroke-linejoin", "round"), Ae(e, "width", "100%"), Ae(e, "height", "100%"), Ae(e, "viewBox", "0 0 24 24"), Ae(e, "stroke-width", "1.5"), Ae(e, "fill", "none"), Ae(e, "stroke", "currentColor"), Ae(e, "xmlns", "http://www.w3.org/2000/svg"), Ae(e, "color", "currentColor");
+            e = si("svg"), n = si("title"), i = Gh("High volume"), o = si("path"), r = si("path"), s = si("path"), Ae(o, "d", "M1 13.8571V10.1429C1 9.03829 1.89543 8.14286 3 8.14286H5.9C6.09569 8.14286 6.28708 8.08544 6.45046 7.97772L12.4495 4.02228C13.1144 3.5839 14 4.06075 14 4.85714V19.1429C14 19.9392 13.1144 20.4161 12.4495 19.9777L6.45046 16.0223C6.28708 15.9146 6.09569 15.8571 5.9 15.8571H3C1.89543 15.8571 1 14.9617 1 13.8571Z"), Ae(o, "stroke-width", "1.5"), Ae(r, "d", "M17.5 7.5C17.5 7.5 19 9 19 11.5C19 14 17.5 15.5 17.5 15.5"), Ae(r, "stroke-width", "1.5"), Ae(r, "stroke-linecap", "round"), Ae(r, "stroke-linejoin", "round"), Ae(s, "d", "M20.5 4.5C20.5 4.5 23 7 23 11.5C23 16 20.5 18.5 20.5 18.5"), Ae(s, "stroke-width", "1.5"), Ae(s, "stroke-linecap", "round"), Ae(s, "stroke-linejoin", "round"), Ae(e, "width", "100%"), Ae(e, "height", "100%"), Ae(e, "viewBox", "0 0 24 24"), Ae(e, "stroke-width", "1.5"), Ae(e, "fill", "none"), Ae(e, "stroke", "currentColor"), Ae(e, "xmlns", "http://www.w3.org/2000/svg"), Ae(e, "color", "currentColor");
         },
         m(a, l) {
-            jh(a, e, l), oi(e, n), oi(n, i), oi(e, o), oi(e, r), oi(e, s);
+            qh(a, e, l), ri(e, n), ri(n, i), ri(e, o), ri(e, r), ri(e, s);
         },
         p: rr,
         i: rr,
         o: rr,
         d(a) {
-            a && Ih(e);
+            a && jh(e);
         }
     };
 }
-class Gh extends Nh {
+class Vh extends Uh {
     constructor(e) {
-        super(), Uh(this, e, null, zh, Fh, {});
+        super(), Fh(this, e, null, Wh, zh, {});
     }
 }
 const {
-    SvelteComponent: Wh,
+    SvelteComponent: Xh,
     append: Bt,
     attr: we,
-    detach: Vh,
-    init: Xh,
-    insert: xh,
+    detach: xh,
+    init: Zh,
+    insert: Jh,
     noop: sr,
-    safe_not_equal: Zh,
+    safe_not_equal: Yh,
     svg_element: Mt,
-    text: Jh
+    text: Qh
 } = window.__gradio__svelte__internal;
 
-function Yh(t) {
+function Kh(t) {
     let e, n, i, o, r, s, a, l, u;
     return {
         c() {
-            e = Mt("svg"), n = Mt("title"), i = Jh("Muted volume"), o = Mt("g"), r = Mt("path"), s = Mt("path"), a = Mt("defs"), l = Mt("clipPath"), u = Mt("rect"), we(r, "d", "M18 14L20.0005 12M22 10L20.0005 12M20.0005 12L18 10M20.0005 12L22 14"), we(r, "stroke-width", "1.5"), we(r, "stroke-linecap", "round"), we(r, "stroke-linejoin", "round"), we(s, "d", "M2 13.8571V10.1429C2 9.03829 2.89543 8.14286 4 8.14286H6.9C7.09569 8.14286 7.28708 8.08544 7.45046 7.97772L13.4495 4.02228C14.1144 3.5839 15 4.06075 15 4.85714V19.1429C15 19.9392 14.1144 20.4161 13.4495 19.9777L7.45046 16.0223C7.28708 15.9146 7.09569 15.8571 6.9 15.8571H4C2.89543 15.8571 2 14.9617 2 13.8571Z"), we(s, "stroke-width", "1.5"), we(o, "clip-path", "url(#clip0_3173_16686)"), we(u, "width", "24"), we(u, "height", "24"), we(u, "fill", "white"), we(l, "id", "clip0_3173_16686"), we(e, "width", "100%"), we(e, "height", "100%"), we(e, "viewBox", "0 0 24 24"), we(e, "stroke-width", "1.5"), we(e, "fill", "none"), we(e, "xmlns", "http://www.w3.org/2000/svg"), we(e, "stroke", "currentColor"), we(e, "color", "currentColor");
+            e = Mt("svg"), n = Mt("title"), i = Qh("Muted volume"), o = Mt("g"), r = Mt("path"), s = Mt("path"), a = Mt("defs"), l = Mt("clipPath"), u = Mt("rect"), we(r, "d", "M18 14L20.0005 12M22 10L20.0005 12M20.0005 12L18 10M20.0005 12L22 14"), we(r, "stroke-width", "1.5"), we(r, "stroke-linecap", "round"), we(r, "stroke-linejoin", "round"), we(s, "d", "M2 13.8571V10.1429C2 9.03829 2.89543 8.14286 4 8.14286H6.9C7.09569 8.14286 7.28708 8.08544 7.45046 7.97772L13.4495 4.02228C14.1144 3.5839 15 4.06075 15 4.85714V19.1429C15 19.9392 14.1144 20.4161 13.4495 19.9777L7.45046 16.0223C7.28708 15.9146 7.09569 15.8571 6.9 15.8571H4C2.89543 15.8571 2 14.9617 2 13.8571Z"), we(s, "stroke-width", "1.5"), we(o, "clip-path", "url(#clip0_3173_16686)"), we(u, "width", "24"), we(u, "height", "24"), we(u, "fill", "white"), we(l, "id", "clip0_3173_16686"), we(e, "width", "100%"), we(e, "height", "100%"), we(e, "viewBox", "0 0 24 24"), we(e, "stroke-width", "1.5"), we(e, "fill", "none"), we(e, "xmlns", "http://www.w3.org/2000/svg"), we(e, "stroke", "currentColor"), we(e, "color", "currentColor");
         },
         m(c, f) {
-            xh(c, e, f), Bt(e, n), Bt(n, i), Bt(e, o), Bt(o, r), Bt(o, s), Bt(e, a), Bt(a, l), Bt(l, u);
+            Jh(c, e, f), Bt(e, n), Bt(n, i), Bt(e, o), Bt(o, r), Bt(o, s), Bt(e, a), Bt(a, l), Bt(l, u);
         },
         p: sr,
         i: sr,
         o: sr,
         d(c) {
-            c && Vh(e);
+            c && xh(e);
         }
     };
 }
-class Qh extends Wh {
+class $h extends Xh {
     constructor(e) {
-        super(), Xh(this, e, null, Yh, Zh, {});
+        super(), Zh(this, e, null, Kh, Yh, {});
     }
 }
 const {
-    SvelteComponent: Kh,
+    SvelteComponent: e_,
     append: Us,
     attr: Dt,
-    detach: $h,
-    init: e_,
-    insert: t_,
+    detach: t_,
+    init: n_,
+    insert: i_,
     noop: lr,
-    safe_not_equal: n_,
+    safe_not_equal: o_,
     svg_element: ar
 } = window.__gradio__svelte__internal;
 
-function i_(t) {
+function r_(t) {
     let e, n, i;
     return {
         c() {
             e = ar("svg"), n = ar("path"), i = ar("path"), Dt(n, "fill", "currentColor"), Dt(n, "d", "M12 2c-4.963 0-9 4.038-9 9c0 3.328 1.82 6.232 4.513 7.79l-2.067 1.378A1 1 0 0 0 6 22h12a1 1 0 0 0 .555-1.832l-2.067-1.378C19.18 17.232 21 14.328 21 11c0-4.962-4.037-9-9-9zm0 16c-3.859 0-7-3.141-7-7c0-3.86 3.141-7 7-7s7 3.14 7 7c0 3.859-3.141 7-7 7z"), Dt(i, "fill", "currentColor"), Dt(i, "d", "M12 6c-2.757 0-5 2.243-5 5s2.243 5 5 5s5-2.243 5-5s-2.243-5-5-5zm0 8c-1.654 0-3-1.346-3-3s1.346-3 3-3s3 1.346 3 3s-1.346 3-3 3z"), Dt(e, "xmlns", "http://www.w3.org/2000/svg"), Dt(e, "width", "100%"), Dt(e, "height", "100%"), Dt(e, "viewBox", "0 0 24 24");
         },
         m(o, r) {
-            t_(o, e, r), Us(e, n), Us(e, i);
+            i_(o, e, r), Us(e, n), Us(e, i);
         },
         p: lr,
         i: lr,
         o: lr,
         d(o) {
-            o && $h(e);
+            o && t_(e);
         }
     };
 }
-class o_ extends Kh {
+class s_ extends e_ {
     constructor(e) {
-        super(), e_(this, e, null, i_, n_, {});
+        super(), n_(this, e, null, r_, o_, {});
     }
 }
 const {
-    SvelteComponent: r_,
+    SvelteComponent: l_,
     append: Kt,
     attr: Dr,
-    check_outros: s_,
+    check_outros: a_,
     create_component: Xa,
     destroy_component: xa,
     detach: Qi,
     element: Hr,
-    group_outros: l_,
-    init: a_,
+    group_outros: u_,
+    init: c_,
     insert: Ki,
     mount_component: Za,
-    safe_not_equal: u_,
+    safe_not_equal: f_,
     set_data: Or,
     space: Nr,
-    text: fi,
+    text: di,
     toggle_class: js,
     transition_in: no,
     transition_out: io
 } = window.__gradio__svelte__internal;
 
-function c_(t) {
+function d_(t) {
     let e, n;
     return e = new Va({}), {
         c() {
             Xa(e.$$.fragment);
         },
         m(i, o) {
             Za(e, i, o), n = !0;
@@ -3296,15 +3296,15 @@
         },
         d(i) {
             xa(e, i);
         }
     };
 }
 
-function f_(t) {
+function h_(t) {
     let e, n;
     return e = new za({}), {
         c() {
             Xa(e.$$.fragment);
         },
         m(i, o) {
             Za(e, i, o), n = !0;
@@ -3330,15 +3330,15 @@
             /*message*/
             (t[2] || /*i18n*/
                 t[1]("upload_text.click_to_upload")) + ""
         ),
         l;
     return {
         c() {
-            e = Hr("span"), n = fi("- "), o = fi(i), r = fi(" -"), s = Nr(), l = fi(a), Dr(e, "class", "or svelte-kzcjhc");
+            e = Hr("span"), n = di("- "), o = di(i), r = di(" -"), s = Nr(), l = di(a), Dr(e, "class", "or svelte-kzcjhc");
         },
         m(u, c) {
             Ki(u, e, c), Kt(e, n), Kt(e, o), Kt(e, r), Ki(u, s, c), Ki(u, l, c);
         },
         p(u, c) {
             c & /*i18n*/
                 2 && i !== (i = /*i18n*/
@@ -3349,28 +3349,28 @@
         },
         d(u) {
             u && (Qi(e), Qi(s), Qi(l));
         }
     };
 }
 
-function d_(t) {
+function __(t) {
     let e, n, i, o, r, s = (
             /*i18n*/
             t[1](
                 /*defs*/
                 t[5][
                     /*type*/
                     t[0]
                 ] || /*defs*/
                 t[5].file
             ) + ""
         ),
         a, l, u;
-    const c = [f_, c_],
+    const c = [h_, d_],
         f = [];
 
     function h(_, m) {
         return (
             /*type*/
             _[0] === "clipboard" ? 0 : 1
         );
@@ -3378,29 +3378,29 @@
     i = h(t), o = f[i] = c[i](t);
     let d = (
         /*mode*/
         t[3] !== "short" && Fs(t)
     );
     return {
         c() {
-            e = Hr("div"), n = Hr("span"), o.c(), r = Nr(), a = fi(s), l = Nr(), d && d.c(), Dr(n, "class", "icon-wrap svelte-kzcjhc"), js(
+            e = Hr("div"), n = Hr("span"), o.c(), r = Nr(), a = di(s), l = Nr(), d && d.c(), Dr(n, "class", "icon-wrap svelte-kzcjhc"), js(
                 n,
                 "hovered",
                 /*hovered*/
                 t[4]
             ), Dr(e, "class", "wrap svelte-kzcjhc");
         },
         m(_, m) {
             Ki(_, e, m), Kt(e, n), f[i].m(n, null), Kt(e, r), Kt(e, a), Kt(e, l), d && d.m(e, null), u = !0;
         },
         p(_, [m]) {
-            let v = i;
-            i = h(_), i !== v && (l_(), io(f[v], 1, 1, () => {
-                    f[v] = null;
-                }), s_(), o = f[i], o || (o = f[i] = c[i](_), o.c()), no(o, 1), o.m(n, null)), (!u || m & /*hovered*/
+            let b = i;
+            i = h(_), i !== b && (u_(), io(f[b], 1, 1, () => {
+                    f[b] = null;
+                }), a_(), o = f[i], o || (o = f[i] = c[i](_), o.c()), no(o, 1), o.m(n, null)), (!u || m & /*hovered*/
                     16) && js(
                     n,
                     "hovered",
                     /*hovered*/
                     _[4]
                 ), (!u || m & /*i18n, type*/
                     3) && s !== (s = /*i18n*/
@@ -3422,15 +3422,15 @@
         },
         d(_) {
             _ && Qi(e), f[i].d(), d && d.d();
         }
     };
 }
 
-function h_(t, e, n) {
+function m_(t, e, n) {
     let {
         type: i = "file"
     } = e, {
         i18n: o
     } = e, {
         message: r = void 0
     } = e, {
@@ -3447,41 +3447,41 @@
         gallery: "upload_text.drop_gallery",
         clipboard: "upload_text.paste_clipboard"
     };
     return t.$$set = (u) => {
         "type" in u && n(0, i = u.type), "i18n" in u && n(1, o = u.i18n), "message" in u && n(2, r = u.message), "mode" in u && n(3, s = u.mode), "hovered" in u && n(4, a = u.hovered);
     }, [i, o, r, s, a, l];
 }
-class __ extends r_ {
+class p_ extends l_ {
     constructor(e) {
-        super(), a_(this, e, h_, d_, u_, {
+        super(), c_(this, e, m_, __, f_, {
             type: 0,
             i18n: 1,
             message: 2,
             mode: 3,
             hovered: 4
         });
     }
 }
 const {
-    SvelteComponent: m_,
+    SvelteComponent: g_,
     append: ur,
     attr: vt,
-    check_outros: di,
+    check_outros: hi,
     create_component: po,
     destroy_component: go,
-    detach: Xn,
+    detach: xn,
     element: Ci,
-    empty: p_,
-    group_outros: hi,
-    init: g_,
-    insert: xn,
+    empty: b_,
+    group_outros: _i,
+    init: v_,
+    insert: Zn,
     listen: bo,
     mount_component: vo,
-    safe_not_equal: b_,
+    safe_not_equal: w_,
     space: cr,
     toggle_class: jt,
     transition_in: ke,
     transition_out: Ue
 } = window.__gradio__svelte__internal;
 
 function qs(t) {
@@ -3506,47 +3506,47 @@
         h = s && Ws(t),
         d = l && Vs(t);
     return {
         c() {
             e = Ci("span"), c && c.c(), i = cr(), f && f.c(), r = cr(), h && h.c(), a = cr(), d && d.c(), vt(e, "class", "source-selection svelte-1jp3vgd"), vt(e, "data-testid", "source-select");
         },
         m(_, m) {
-            xn(_, e, m), c && c.m(e, null), ur(e, i), f && f.m(e, null), ur(e, r), h && h.m(e, null), ur(e, a), d && d.m(e, null), u = !0;
+            Zn(_, e, m), c && c.m(e, null), ur(e, i), f && f.m(e, null), ur(e, r), h && h.m(e, null), ur(e, a), d && d.m(e, null), u = !0;
         },
         p(_, m) {
             m & /*sources*/
                 2 && (n = /*sources*/
                     _[1].includes("upload")), n ? c ? (c.p(_, m), m & /*sources*/
-                    2 && ke(c, 1)) : (c = zs(_), c.c(), ke(c, 1), c.m(e, i)) : c && (hi(), Ue(c, 1, 1, () => {
+                    2 && ke(c, 1)) : (c = zs(_), c.c(), ke(c, 1), c.m(e, i)) : c && (_i(), Ue(c, 1, 1, () => {
                     c = null;
-                }), di()), m & /*sources*/
+                }), hi()), m & /*sources*/
                 2 && (o = /*sources*/
                     _[1].includes("microphone")), o ? f ? (f.p(_, m), m & /*sources*/
-                    2 && ke(f, 1)) : (f = Gs(_), f.c(), ke(f, 1), f.m(e, r)) : f && (hi(), Ue(f, 1, 1, () => {
+                    2 && ke(f, 1)) : (f = Gs(_), f.c(), ke(f, 1), f.m(e, r)) : f && (_i(), Ue(f, 1, 1, () => {
                     f = null;
-                }), di()), m & /*sources*/
+                }), hi()), m & /*sources*/
                 2 && (s = /*sources*/
                     _[1].includes("webcam")), s ? h ? (h.p(_, m), m & /*sources*/
-                    2 && ke(h, 1)) : (h = Ws(_), h.c(), ke(h, 1), h.m(e, a)) : h && (hi(), Ue(h, 1, 1, () => {
+                    2 && ke(h, 1)) : (h = Ws(_), h.c(), ke(h, 1), h.m(e, a)) : h && (_i(), Ue(h, 1, 1, () => {
                     h = null;
-                }), di()), m & /*sources*/
+                }), hi()), m & /*sources*/
                 2 && (l = /*sources*/
                     _[1].includes("clipboard")), l ? d ? (d.p(_, m), m & /*sources*/
-                    2 && ke(d, 1)) : (d = Vs(_), d.c(), ke(d, 1), d.m(e, null)) : d && (hi(), Ue(d, 1, 1, () => {
+                    2 && ke(d, 1)) : (d = Vs(_), d.c(), ke(d, 1), d.m(e, null)) : d && (_i(), Ue(d, 1, 1, () => {
                     d = null;
-                }), di());
+                }), hi());
         },
         i(_) {
             u || (ke(c), ke(f), ke(h), ke(d), u = !0);
         },
         o(_) {
             Ue(c), Ue(f), Ue(h), Ue(d), u = !1;
         },
         d(_) {
-            _ && Xn(e), c && c.d(), f && f.d(), h && h.d(), d && d.d();
+            _ && xn(e), c && c.d(), f && f.d(), h && h.d(), d && d.d();
         }
     };
 }
 
 function zs(t) {
     let e, n, i, o, r;
     return n = new Va({}), {
@@ -3556,15 +3556,15 @@
                 "selected",
                 /*active_source*/
                 t[0] === "upload" || ! /*active_source*/
                 t[0]
             );
         },
         m(s, a) {
-            xn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
+            Zn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
                 e,
                 "click",
                 /*click_handler*/
                 t[6]
             ), o = !0);
         },
         p(s, a) {
@@ -3580,32 +3580,32 @@
         i(s) {
             i || (ke(n.$$.fragment, s), i = !0);
         },
         o(s) {
             Ue(n.$$.fragment, s), i = !1;
         },
         d(s) {
-            s && Xn(e), go(n), o = !1, r();
+            s && xn(e), go(n), o = !1, r();
         }
     };
 }
 
 function Gs(t) {
     let e, n, i, o, r;
-    return n = new zd({}), {
+    return n = new Wd({}), {
         c() {
             e = Ci("button"), po(n.$$.fragment), vt(e, "class", "icon svelte-1jp3vgd"), vt(e, "aria-label", "Record audio"), jt(
                 e,
                 "selected",
                 /*active_source*/
                 t[0] === "microphone"
             );
         },
         m(s, a) {
-            xn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
+            Zn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
                 e,
                 "click",
                 /*click_handler_1*/
                 t[7]
             ), o = !0);
         },
         p(s, a) {
@@ -3620,32 +3620,32 @@
         i(s) {
             i || (ke(n.$$.fragment, s), i = !0);
         },
         o(s) {
             Ue(n.$$.fragment, s), i = !1;
         },
         d(s) {
-            s && Xn(e), go(n), o = !1, r();
+            s && xn(e), go(n), o = !1, r();
         }
     };
 }
 
 function Ws(t) {
     let e, n, i, o, r;
-    return n = new o_({}), {
+    return n = new s_({}), {
         c() {
             e = Ci("button"), po(n.$$.fragment), vt(e, "class", "icon svelte-1jp3vgd"), vt(e, "aria-label", "Capture from camera"), jt(
                 e,
                 "selected",
                 /*active_source*/
                 t[0] === "webcam"
             );
         },
         m(s, a) {
-            xn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
+            Zn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
                 e,
                 "click",
                 /*click_handler_2*/
                 t[8]
             ), o = !0);
         },
         p(s, a) {
@@ -3660,15 +3660,15 @@
         i(s) {
             i || (ke(n.$$.fragment, s), i = !0);
         },
         o(s) {
             Ue(n.$$.fragment, s), i = !1;
         },
         d(s) {
-            s && Xn(e), go(n), o = !1, r();
+            s && xn(e), go(n), o = !1, r();
         }
     };
 }
 
 function Vs(t) {
     let e, n, i, o, r;
     return n = new za({}), {
@@ -3677,15 +3677,15 @@
                 e,
                 "selected",
                 /*active_source*/
                 t[0] === "clipboard"
             );
         },
         m(s, a) {
-            xn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
+            Zn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
                 e,
                 "click",
                 /*click_handler_3*/
                 t[9]
             ), o = !0);
         },
         p(s, a) {
@@ -3700,51 +3700,51 @@
         i(s) {
             i || (ke(n.$$.fragment, s), i = !0);
         },
         o(s) {
             Ue(n.$$.fragment, s), i = !1;
         },
         d(s) {
-            s && Xn(e), go(n), o = !1, r();
+            s && xn(e), go(n), o = !1, r();
         }
     };
 }
 
-function v_(t) {
+function y_(t) {
     let e, n, i = (
         /*unique_sources*/
         t[2].length > 1 && qs(t)
     );
     return {
         c() {
-            i && i.c(), e = p_();
+            i && i.c(), e = b_();
         },
         m(o, r) {
-            i && i.m(o, r), xn(o, e, r), n = !0;
+            i && i.m(o, r), Zn(o, e, r), n = !0;
         },
         p(o, [r]) {
             /*unique_sources*/
             o[2].length > 1 ? i ? (i.p(o, r), r & /*unique_sources*/
-                4 && ke(i, 1)) : (i = qs(o), i.c(), ke(i, 1), i.m(e.parentNode, e)) : i && (hi(), Ue(i, 1, 1, () => {
+                4 && ke(i, 1)) : (i = qs(o), i.c(), ke(i, 1), i.m(e.parentNode, e)) : i && (_i(), Ue(i, 1, 1, () => {
                 i = null;
-            }), di());
+            }), hi());
         },
         i(o) {
             n || (ke(i), n = !0);
         },
         o(o) {
             Ue(i), n = !1;
         },
         d(o) {
-            o && Xn(e), i && i.d(o);
+            o && xn(e), i && i.d(o);
         }
     };
 }
 
-function w_(t, e, n) {
+function k_(t, e, n) {
     let i, {
             sources: o
         } = e,
         {
             active_source: r
         } = e,
         {
@@ -3774,58 +3774,58 @@
         a,
         u,
         c,
         f,
         h
     ];
 }
-class y_ extends m_ {
+class E_ extends g_ {
     constructor(e) {
-        super(), g_(this, e, w_, v_, b_, {
+        super(), v_(this, e, k_, y_, w_, {
             sources: 1,
             active_source: 0,
             handle_clear: 4,
             handle_select: 5
         });
     }
 }
 const {
-    SvelteComponent: k_,
-    append: si,
+    SvelteComponent: C_,
+    append: li,
     attr: nt,
-    detach: E_,
-    init: C_,
-    insert: S_,
+    detach: S_,
+    init: A_,
+    insert: T_,
     noop: fr,
-    safe_not_equal: A_,
+    safe_not_equal: P_,
     svg_element: Cn
 } = window.__gradio__svelte__internal;
 
-function T_(t) {
+function L_(t) {
     let e, n, i, o, r, s;
     return {
         c() {
             e = Cn("svg"), n = Cn("g"), i = Cn("g"), o = Cn("path"), r = Cn("path"), s = Cn("polygon"), nt(o, "d", `M348.994,102.946L250.04,3.993c-5.323-5.323-13.954-5.324-19.277,0l-153.7,153.701l118.23,118.23l153.701-153.7\r
 			C354.317,116.902,354.317,108.271,348.994,102.946z`), nt(r, "d", `M52.646,182.11l-41.64,41.64c-5.324,5.322-5.324,13.953,0,19.275l98.954,98.957c5.323,5.322,13.954,5.32,19.277,0\r
 			l41.639-41.641L52.646,182.11z`), nt(s, "points", "150.133,360 341.767,360 341.767,331.949 182.806,331.949"), nt(e, "version", "1.1"), nt(e, "id", "Capa_1"), nt(e, "xmlns", "http://www.w3.org/2000/svg"), nt(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), nt(e, "width", "100%"), nt(e, "height", "100%"), nt(e, "viewBox", "0 0 360 360"), nt(e, "color", "#9CA3AF");
         },
         m(a, l) {
-            S_(a, e, l), si(e, n), si(n, i), si(i, o), si(i, r), si(i, s);
+            T_(a, e, l), li(e, n), li(n, i), li(i, o), li(i, r), li(i, s);
         },
         p: fr,
         i: fr,
         o: fr,
         d(a) {
-            a && E_(e);
+            a && S_(e);
         }
     };
 }
-class P_ extends k_ {
+class R_ extends C_ {
     constructor(e) {
-        super(), C_(this, e, null, T_, A_, {});
+        super(), A_(this, e, null, L_, P_, {});
     }
 }
 /*! *****************************************************************************
 Copyright (c) Microsoft Corporation.
 
 Permission to use, copy, modify, and/or distribute this software for any
 purpose with or without fee is hereby granted.
@@ -3941,20 +3941,20 @@
     return n;
 }
 
 function xs(t, e, n) {
     const i = Ja(t, e || {});
     return n == null || n.appendChild(i), i;
 }
-var L_ = Object.freeze({
+var B_ = Object.freeze({
     __proto__: null,
     createElement: xs,
     default: xs
 });
-const R_ = {
+const M_ = {
     fetchBlob: function(t, e, n) {
         return Ce(this, void 0, void 0, function*() {
             const i = yield fetch(t, n);
             if (i.status >= 400)
                 throw new Error(`Failed to fetch ${t}: ${i.status} (${i.statusText})`);
             return function(o, r) {
                 Ce(this, void 0, void 0, function*() {
@@ -3979,15 +3979,15 @@
                         });
                     c();
                 });
             }(i.clone(), e), i.blob();
         });
     }
 };
-class B_ extends Si {
+class D_ extends Si {
     constructor(e) {
         super(), this.isExternalMedia = !1, e.media ? (this.media = e.media, this.isExternalMedia = !0) : this.media = document.createElement("audio"), e.mediaControls && (this.media.controls = !0), e.autoplay && (this.media.autoplay = !0), e.playbackRate != null && this.onMediaEvent("canplay", () => {
             e.playbackRate != null && (this.media.playbackRate = e.playbackRate);
         }, {
             once: !0
         });
     }
@@ -4118,47 +4118,47 @@
                 f = 0,
                 h = 0,
                 d = 0;
             const _ = matchMedia("(pointer: coarse)").matches,
                 m = (E) => {
                     E.button === s && (E.stopPropagation(), u = !0, c = !1, d = Date.now(), l = e.getBoundingClientRect(), f = E.clientX - l.left, h = E.clientY - l.top);
                 },
-                v = (E) => {
+                b = (E) => {
                     if (u = !1, d = 0, c) {
                         E.preventDefault(), E.stopPropagation(), setTimeout(() => {
                             c = !1;
                         }, 300);
                         const y = E.clientX - l.left,
                             H = E.clientY - l.top;
                         o == null || o(y, H);
                     }
                 },
-                b = (E) => {
+                g = (E) => {
                     if (!u || _ && Date.now() - d < a)
                         return;
                     E.preventDefault(), E.stopPropagation();
                     const y = E.clientX - l.left,
                         H = E.clientY - l.top,
                         L = y - f,
                         P = H - h;
                     (c || Math.abs(L) > r || Math.abs(P) > r) && (c || (i == null || i(f, h), c = !0), n(L, P, y, H), f = y, h = H);
                 },
                 S = (E) => {
-                    E.relatedTarget && E.relatedTarget !== document.documentElement || v(E);
+                    E.relatedTarget && E.relatedTarget !== document.documentElement || b(E);
                 },
                 w = (E) => {
                     c && E.preventDefault();
                 },
                 k = (E) => {
                     c && (E.stopPropagation(), E.preventDefault());
                 };
-            return e.addEventListener("pointerdown", m), e.addEventListener("click", k, !0), document.addEventListener("click", k, !0), document.addEventListener("pointermove", b), document.addEventListener("touchmove", w, {
+            return e.addEventListener("pointerdown", m), e.addEventListener("click", k, !0), document.addEventListener("click", k, !0), document.addEventListener("pointermove", g), document.addEventListener("touchmove", w, {
                 passive: !1
-            }), document.addEventListener("pointerup", v), document.addEventListener("pointerleave", S), document.addEventListener("pointercancel", v), () => {
-                e.removeEventListener("pointerdown", m), e.removeEventListener("click", k, !0), document.removeEventListener("click", k, !0), document.removeEventListener("pointermove", b), document.removeEventListener("touchmove", w), document.removeEventListener("pointerup", v), document.removeEventListener("pointerleave", S), document.removeEventListener("pointercancel", v);
+            }), document.addEventListener("pointerup", b), document.addEventListener("pointerleave", S), document.addEventListener("pointercancel", b), () => {
+                e.removeEventListener("pointerdown", m), e.removeEventListener("click", k, !0), document.removeEventListener("click", k, !0), document.removeEventListener("pointermove", g), document.removeEventListener("touchmove", w), document.removeEventListener("pointerup", b), document.removeEventListener("pointerleave", S), document.removeEventListener("pointercancel", b);
             };
         }(this.wrapper, (e, n, i) => {
             this.emit("drag", Math.max(0, Math.min(1, i / this.wrapper.getBoundingClientRect().width)));
         }, (e) => {
             this.isDragging = !0, this.emit("dragstart", Math.max(0, Math.min(1, e / this.wrapper.getBoundingClientRect().width)));
         }, (e) => {
             this.isDragging = !1, this.emit("dragend", Math.max(0, Math.min(1, e / this.wrapper.getBoundingClientRect().width)));
@@ -4308,26 +4308,26 @@
             } = i.canvas,
             c = u / 2,
             f = window.devicePixelRatio || 1,
             h = n.barWidth ? n.barWidth * f : 1,
             d = n.barGap ? n.barGap * f : n.barWidth ? h / 2 : 0,
             _ = n.barRadius || 0,
             m = l / (h + d) / a,
-            v = _ && "roundRect" in i ? "roundRect" : "rect";
+            b = _ && "roundRect" in i ? "roundRect" : "rect";
         i.beginPath();
-        let b = 0,
+        let g = 0,
             S = 0,
             w = 0;
         for (let k = 0; k <= a; k++) {
             const E = Math.round(k * m);
-            if (E > b) {
+            if (E > g) {
                 const L = Math.round(S * c * o),
                     P = L + Math.round(w * c * o) || 1;
-                let M = c - L;
-                n.barAlign === "top" ? M = 0 : n.barAlign === "bottom" && (M = u - P), i[v](b * (h + d), M, h, P, _), b = E, S = 0, w = 0;
+                let D = c - L;
+                n.barAlign === "top" ? D = 0 : n.barAlign === "bottom" && (D = u - P), i[b](g * (h + d), D, h, P, _), g = E, S = 0, w = 0;
             }
             const y = Math.abs(r[k] || 0),
                 H = Math.abs(s[k] || 0);
             y > S && (S = y), H > w && (w = H);
         }
         i.fill(), i.closePath();
     }
@@ -4342,19 +4342,19 @@
                 f = i.canvas.width / l;
             i.moveTo(0, c);
             let h = 0,
                 d = 0;
             for (let _ = 0; _ <= l; _++) {
                 const m = Math.round(_ * f);
                 if (m > h) {
-                    const b = c + (Math.round(d * c * o) || 1) * (s === 0 ? -1 : 1);
-                    i.lineTo(h, b), h = m, d = 0;
+                    const g = c + (Math.round(d * c * o) || 1) * (s === 0 ? -1 : 1);
+                    i.lineTo(h, g), h = m, d = 0;
                 }
-                const v = Math.abs(a[_] || 0);
-                v > d && (d = v);
+                const b = Math.abs(a[_] || 0);
+                b > d && (d = b);
             }
             i.lineTo(h, c);
         };
         i.beginPath(), r(0), r(1), i.fill(), i.closePath();
     }
     renderWaveform(e, n, i) {
         if (i.fillStyle = this.convertColorValues(n.waveColor), n.renderFunction)
@@ -4405,28 +4405,28 @@
             if (!this.isScrollable)
                 return void f(0, c);
             const {
                 scrollLeft: h,
                 scrollWidth: d,
                 clientWidth: _
             } = this.scrollContainer, m = c / d;
-            let v = Math.min(wo.MAX_CANVAS_WIDTH, _);
+            let b = Math.min(wo.MAX_CANVAS_WIDTH, _);
             if (s.barWidth || s.barGap) {
                 const k = s.barWidth || 0.5,
                     E = k + (s.barGap || k / 2);
-                v % E != 0 && (v = Math.floor(v / E) * E);
+                b % E != 0 && (b = Math.floor(b / E) * E);
             }
-            const b = Math.floor(Math.abs(h) * m),
-                S = Math.floor(b + v * m),
-                w = S - b;
-            w <= 0 || (f(b, S), yield Promise.all([Ce(this, void 0, void 0, function*() {
-                if (b === 0)
+            const g = Math.floor(Math.abs(h) * m),
+                S = Math.floor(g + b * m),
+                w = S - g;
+            w <= 0 || (f(g, S), yield Promise.all([Ce(this, void 0, void 0, function*() {
+                if (g === 0)
                     return;
                 const k = this.createDelay();
-                for (let E = b; E >= 0; E -= w)
+                for (let E = g; E >= 0; E -= w)
                     yield k(), f(Math.max(0, E - w), E);
             }), Ce(this, void 0, void 0, function*() {
                 if (S === c)
                     return;
                 const k = this.createDelay();
                 for (let E = S; E < c; E += w)
                     yield k(), f(E, Math.min(c, E + w));
@@ -4520,15 +4520,15 @@
                     l ? s(l) : a(new Error("Could not export image"));
                 }, e, n);
             })));
         });
     }
 }
 wo.MAX_CANVAS_WIDTH = 4e3;
-class M_ extends Si {
+class H_ extends Si {
     constructor() {
         super(...arguments), this.unsubscribe = () => {};
     }
     start() {
         this.unsubscribe = this.on("tick", () => {
             requestAnimationFrame(() => {
                 this.emit("tick");
@@ -4643,38 +4643,38 @@
             return e;
         const n = this.buffer.numberOfChannels;
         for (let i = 0; i < n; i++)
             e.push(this.buffer.getChannelData(i));
         return e;
     }
 }
-const D_ = {
+const O_ = {
     waveColor: "#999",
     progressColor: "#555",
     cursorWidth: 1,
     minPxPerSec: 0,
     fillParent: !0,
     interact: !0,
     dragToSeek: !1,
     autoScroll: !0,
     autoCenter: !0,
     sampleRate: 8e3
 };
-class Ft extends B_ {
+class Ft extends D_ {
     static create(e) {
         return new Ft(e);
     }
     constructor(e) {
         const n = e.media || (e.backend === "WebAudio" ? new Zs() : void 0);
         super({
             media: n,
             mediaControls: e.mediaControls,
             autoplay: e.autoplay,
             playbackRate: e.audioRate
-        }), this.plugins = [], this.decodedData = null, this.subscriptions = [], this.mediaSubscriptions = [], this.abortController = null, this.options = Object.assign({}, D_, e), this.timer = new M_();
+        }), this.plugins = [], this.decodedData = null, this.subscriptions = [], this.mediaSubscriptions = [], this.abortController = null, this.options = Object.assign({}, O_, e), this.timer = new H_();
         const i = n ? void 0 : this.getMediaElement();
         this.renderer = new wo(this.options, i), this.initPlayerEvents(), this.initRendererEvents(), this.initTimerEvents(), this.initPlugins(), Promise.resolve().then(() => {
             this.emit("init");
             const o = this.options.url || this.getSrc() || "";
             (o || this.options.peaks && this.options.duration) && this.load(o, this.options.peaks, this.options.duration).catch(() => null);
         });
     }
@@ -4769,15 +4769,15 @@
     loadAudio(e, n, i, o) {
         var r;
         return Ce(this, void 0, void 0, function*() {
             if (this.emit("load", e), !this.options.media && this.isPlaying() && this.pause(), this.decodedData = null, !n && !i) {
                 const a = this.options.fetchParams || {};
                 window.AbortController && !a.signal && (this.abortController = new AbortController(), a.signal = (r = this.abortController) === null || r === void 0 ? void 0 : r.signal);
                 const l = (u) => this.emit("loading", u);
-                n = yield R_.fetchBlob(e, l, a);
+                n = yield M_.fetchBlob(e, l, a);
             }
             this.setSrc(e, n);
             const s = o || this.getDuration() || (yield new Promise((a) => {
                 this.onMediaEvent("loadedmetadata", () => a(this.getDuration()), {
                     once: !0
                 });
             }));
@@ -4896,15 +4896,15 @@
     onInit() {}
     _init(t) {
         this.wavesurfer = t, this.onInit();
     }
     destroy() {
         this.emit("destroy"), this.subscriptions.forEach((t) => t());
     }
-}, Ft.dom = L_;
+}, Ft.dom = B_;
 let Ya = class {
         constructor() {
             this.listeners = {};
         }
         on(e, n, i) {
             if (this.listeners[e] || (this.listeners[e] = /* @__PURE__ */ new Set()), this.listeners[e].add(n), i == null ? void 0 : i.once) {
                 const o = () => {
@@ -4926,15 +4926,15 @@
         unAll() {
             this.listeners = {};
         }
         emit(e, ...n) {
             this.listeners[e] && this.listeners[e].forEach((i) => i(...n));
         }
     },
-    H_ = class extends Ya {
+    N_ = class extends Ya {
         constructor(e) {
             super(), this.subscriptions = [], this.options = e;
         }
         onInit() {}
         _init(e) {
             this.wavesurfer = e, this.onInit();
         }
@@ -4961,52 +4961,52 @@
                     u = !1;
                 }, 300);
                 const E = k.clientX - a.left,
                     y = k.clientY - a.top;
                 i == null || i(E, y);
             }
         },
-        v = (k) => {
+        b = (k) => {
             if (!l || d && Date.now() - h < s)
                 return;
             k.preventDefault(), k.stopPropagation();
             const E = k.clientX - a.left,
                 y = k.clientY - a.top,
                 H = E - c,
                 L = y - f;
             (u || Math.abs(H) > o || Math.abs(L) > o) && (u || (n == null || n(c, f), u = !0), e(H, L, E, y), c = E, f = y);
         },
-        b = (k) => {
+        g = (k) => {
             k.relatedTarget && k.relatedTarget !== document.documentElement || m(k);
         },
         S = (k) => {
             u && k.preventDefault();
         },
         w = (k) => {
             u && (k.stopPropagation(), k.preventDefault());
         };
-    return t.addEventListener("pointerdown", _), t.addEventListener("click", w, !0), document.addEventListener("click", w, !0), document.addEventListener("pointermove", v), document.addEventListener("touchmove", S, {
+    return t.addEventListener("pointerdown", _), t.addEventListener("click", w, !0), document.addEventListener("click", w, !0), document.addEventListener("pointermove", b), document.addEventListener("touchmove", S, {
         passive: !1
-    }), document.addEventListener("pointerup", m), document.addEventListener("pointerleave", b), document.addEventListener("pointercancel", m), () => {
-        t.removeEventListener("pointerdown", _), t.removeEventListener("click", w, !0), document.removeEventListener("click", w, !0), document.removeEventListener("pointermove", v), document.removeEventListener("touchmove", S), document.removeEventListener("pointerup", m), document.removeEventListener("pointerleave", b), document.removeEventListener("pointercancel", m);
+    }), document.addEventListener("pointerup", m), document.addEventListener("pointerleave", g), document.addEventListener("pointercancel", m), () => {
+        t.removeEventListener("pointerdown", _), t.removeEventListener("click", w, !0), document.removeEventListener("click", w, !0), document.removeEventListener("pointermove", b), document.removeEventListener("touchmove", S), document.removeEventListener("pointerup", m), document.removeEventListener("pointerleave", g), document.removeEventListener("pointercancel", m);
     };
 }
 
 function Qa(t, e) {
     const n = e.xmlns ? document.createElementNS(e.xmlns, t) : document.createElement(t);
     for (const [i, o] of Object.entries(e))
         if (i === "children")
             for (const [r, s] of Object.entries(e))
                 typeof s == "string" ? n.appendChild(document.createTextNode(s)) : n.appendChild(Qa(r, s));
         else
             i === "style" ? Object.assign(n.style, o) : i === "textContent" ? n.textContent = o : n.setAttribute(i, o.toString());
     return n;
 }
 
-function _i(t, e, n) {
+function mi(t, e, n) {
     const i = Qa(t, e || {});
     return n == null || n.appendChild(i), i;
 }
 let Js = class extends Ya {
         constructor(e, n, i = 0) {
             var o, r, s, a, l, u, c, f;
             super(), this.totalDuration = n, this.numberOfChannels = i, this.minLength = 0, this.maxLength = 1 / 0, this.contentEditable = !1, this.subscriptions = [], this.subscriptions = [], this.id = e.id || `region-${Math.random().toString(32).slice(2)}`, this.start = this.clampPosition(e.start), this.end = this.clampPosition((o = e.end) !== null && o !== void 0 ? o : e.start), this.drag = (r = e.drag) === null || r === void 0 || r, this.resize = (s = e.resize) === null || s === void 0 || s, this.color = (a = e.color) !== null && a !== void 0 ? a : "rgba(0, 0, 0, 0.1)", this.minLength = (l = e.minLength) !== null && l !== void 0 ? l : this.minLength, this.maxLength = (u = e.maxLength) !== null && u !== void 0 ? u : this.maxLength, this.channelIdx = (c = e.channelIdx) !== null && c !== void 0 ? c : -1, this.contentEditable = (f = e.contentEditable) !== null && f !== void 0 ? f : this.contentEditable, this.element = this.initElement(), this.setContent(e.content), this.setPart(), this.renderPosition(), this.initMouseEvents();
@@ -5024,23 +5024,23 @@
                     zIndex: "2",
                     width: "6px",
                     height: "100%",
                     top: "0",
                     cursor: "ew-resize",
                     wordBreak: "keep-all"
                 },
-                i = _i("div", {
+                i = mi("div", {
                     part: "region-handle region-handle-left",
                     style: Object.assign(Object.assign({}, n), {
                         left: "0",
                         borderLeft: "2px solid rgba(0, 0, 0, 0.5)",
                         borderRadius: "2px 0 0 2px"
                     })
                 }, e),
-                o = _i("div", {
+                o = mi("div", {
                     part: "region-handle region-handle-right",
                     style: Object.assign(Object.assign({}, n), {
                         right: "0",
                         borderRight: "2px solid rgba(0, 0, 0, 0.5)",
                         borderRadius: "0 2px 2px 0"
                     })
                 }, e);
@@ -5052,15 +5052,15 @@
             n && e.removeChild(n), i && e.removeChild(i);
         }
         initElement() {
             const e = this.start === this.end;
             let n = 0,
                 i = 100;
             this.channelIdx >= 0 && this.channelIdx < this.numberOfChannels && (i = 100 / this.numberOfChannels, n = i * this.channelIdx);
-            const o = _i("div", {
+            const o = mi("div", {
                 style: {
                     position: "absolute",
                     top: `${n}%`,
                     height: `${i}%`,
                     backgroundColor: e ? "none" : this.color,
                     borderLeft: e ? "2px solid " + this.color : "none",
                     borderRadius: "2px",
@@ -5119,15 +5119,15 @@
             this.emit("play");
         }
         setContent(e) {
             var n;
             if ((n = this.content) === null || n === void 0 || n.remove(), e) {
                 if (typeof e == "string") {
                     const i = this.start === this.end;
-                    this.content = _i("div", {
+                    this.content = mi("div", {
                         style: {
                             padding: `0.2em ${i ? 0.2 : 0.4}em`,
                             display: "inline-block"
                         },
                         textContent: e
                     });
                 } else
@@ -5147,15 +5147,15 @@
                 this.resize = e.resize, this.resize && !o ? this.addResizeHandles(this.element) : this.removeResizeHandles(this.element);
             }
         }
         remove() {
             this.emit("remove"), this.subscriptions.forEach((e) => e()), this.element.remove(), this.element = null;
         }
     },
-    O_ = class Ka extends H_ {
+    I_ = class Ka extends N_ {
         constructor(e) {
             super(e), this.regions = [], this.regionsContainer = this.initRegionsContainer();
         }
         static create(e) {
             return new Ka(e);
         }
         onInit() {
@@ -5169,15 +5169,15 @@
                     e.includes(o) || this.emit("region-in", o);
                 }), e.forEach((o) => {
                     i.includes(o) || this.emit("region-out", o);
                 }), e = i;
             }));
         }
         initRegionsContainer() {
-            return _i("div", {
+            return mi("div", {
                 style: {
                     position: "absolute",
                     top: "0",
                     left: "0",
                     width: "100%",
                     height: "100%",
                     zIndex: "3",
@@ -5279,49 +5279,49 @@
             this.regions.forEach((e) => e.remove());
         }
         destroy() {
             this.clearRegions(), super.destroy(), this.regionsContainer.remove();
         }
     };
 const {
-    SvelteComponent: N_,
-    append: I_,
+    SvelteComponent: U_,
+    append: j_,
     attr: Ht,
-    detach: U_,
-    init: j_,
-    insert: F_,
+    detach: F_,
+    init: q_,
+    insert: z_,
     noop: dr,
-    safe_not_equal: q_,
+    safe_not_equal: G_,
     svg_element: Ys
 } = window.__gradio__svelte__internal;
 
-function z_(t) {
+function W_(t) {
     let e, n;
     return {
         c() {
             e = Ys("svg"), n = Ys("path"), Ht(n, "d", "m17.545 15.467-3.779-3.779a6.15 6.15 0 0 0 .898-3.21c0-3.417-2.961-6.377-6.378-6.377A6.185 6.185 0 0 0 2.1 8.287c0 3.416 2.961 6.377 6.377 6.377a6.15 6.15 0 0 0 3.115-.844l3.799 3.801a.953.953 0 0 0 1.346 0l.943-.943c.371-.371.236-.84-.135-1.211zM4.004 8.287a4.282 4.282 0 0 1 4.282-4.283c2.366 0 4.474 2.107 4.474 4.474a4.284 4.284 0 0 1-4.283 4.283c-2.366-.001-4.473-2.109-4.473-4.474z"), Ht(e, "version", "1.0"), Ht(e, "xmlns", "http://www.w3.org/2000/svg"), Ht(e, "viewBox", "0 0 20 20"), Ht(e, "id", "magnifier"), Ht(e, "width", "100%"), Ht(e, "height", "100%"), Ht(e, "color", "currentColor");
         },
         m(i, o) {
-            F_(i, e, o), I_(e, n);
+            z_(i, e, o), j_(e, n);
         },
         p: dr,
         i: dr,
         o: dr,
         d(i) {
-            i && U_(e);
+            i && F_(e);
         }
     };
 }
-class G_ extends N_ {
+class V_ extends U_ {
     constructor(e) {
-        super(), j_(this, e, null, z_, q_, {});
+        super(), q_(this, e, null, W_, G_, {});
     }
 }
 
-function W_(t) {
+function X_(t) {
     const e = t.numberOfChannels,
         n = t.length * e * 2 + 44,
         i = new ArrayBuffer(n),
         o = new DataView(i);
     let r = 0;
     const s = function(a, l, u) {
         for (let c = 0; c < u.length; c++)
@@ -5334,15 +5334,15 @@
                 -1,
                 Math.min(1, t.getChannelData(l)[a])
             );
             o.setInt16(r, u * 32767, !0), r += 2;
         }
     return new Uint8Array(i);
 }
-const V_ = async (t, e, n) => {
+const x_ = async (t, e, n) => {
     const i = new AudioContext(),
         o = t.numberOfChannels,
         r = t.sampleRate;
     let s = t.length,
         a = 0;
     e && n && (a = Math.round(e * r), s = Math.round(n * r) - a);
     const l = i.createBuffer(
@@ -5352,36 +5352,36 @@
     );
     for (let u = 0; u < o; u++) {
         const c = t.getChannelData(u),
             f = l.getChannelData(u);
         for (let h = 0; h < s; h++)
             f[h] = c[a + h];
     }
-    return W_(l);
+    return X_(l);
 }, Qs = (t, e) => {
     t && t.skip(e);
 }, Ln = (t, e) => (e || (e = 5), t / 100 * e || 5), {
-    SvelteComponent: X_,
-    check_outros: x_,
+    SvelteComponent: Z_,
+    check_outros: J_,
     create_component: ns,
     destroy_component: is,
-    detach: Z_,
-    empty: J_,
-    group_outros: Y_,
-    init: Q_,
-    insert: K_,
+    detach: Y_,
+    empty: Q_,
+    group_outros: K_,
+    init: $_,
+    insert: e0,
     mount_component: os,
-    safe_not_equal: $_,
+    safe_not_equal: t0,
     transition_in: gi,
     transition_out: bi
 } = window.__gradio__svelte__internal;
 
-function e0(t) {
+function n0(t) {
     let e, n;
-    return e = new Gh({}), {
+    return e = new Vh({}), {
         c() {
             ns(e.$$.fragment);
         },
         m(i, o) {
             os(e, i, o), n = !0;
         },
         i(i) {
@@ -5392,17 +5392,17 @@
         },
         d(i) {
             is(e, i);
         }
     };
 }
 
-function t0(t) {
+function i0(t) {
     let e, n;
-    return e = new Oh({}), {
+    return e = new Ih({}), {
         c() {
             ns(e.$$.fragment);
         },
         m(i, o) {
             os(e, i, o), n = !0;
         },
         i(i) {
@@ -5413,17 +5413,17 @@
         },
         d(i) {
             is(e, i);
         }
     };
 }
 
-function n0(t) {
+function o0(t) {
     let e, n;
-    return e = new Qh({}), {
+    return e = new $h({}), {
         c() {
             ns(e.$$.fragment);
         },
         m(i, o) {
             os(e, i, o), n = !0;
         },
         i(i) {
@@ -5434,17 +5434,17 @@
         },
         d(i) {
             is(e, i);
         }
     };
 }
 
-function i0(t) {
+function r0(t) {
     let e, n, i, o;
-    const r = [n0, t0, e0],
+    const r = [o0, i0, n0],
         s = [];
 
     function a(l, u) {
         return (
             /*currentVolume*/
             l[0] == 0 ? 0 : (
                 /*currentVolume*/
@@ -5453,77 +5453,77 @@
                     l[0] >= 0.5 ? 2 : -1
                 )
             )
         );
     }
     return ~(e = a(t)) && (n = s[e] = r[e](t)), {
         c() {
-            n && n.c(), i = J_();
+            n && n.c(), i = Q_();
         },
         m(l, u) {
-            ~e && s[e].m(l, u), K_(l, i, u), o = !0;
+            ~e && s[e].m(l, u), e0(l, i, u), o = !0;
         },
         p(l, [u]) {
             let c = e;
-            e = a(l), e !== c && (n && (Y_(), bi(s[c], 1, 1, () => {
+            e = a(l), e !== c && (n && (K_(), bi(s[c], 1, 1, () => {
                 s[c] = null;
-            }), x_()), ~e ? (n = s[e], n || (n = s[e] = r[e](l), n.c()), gi(n, 1), n.m(i.parentNode, i)) : n = null);
+            }), J_()), ~e ? (n = s[e], n || (n = s[e] = r[e](l), n.c()), gi(n, 1), n.m(i.parentNode, i)) : n = null);
         },
         i(l) {
             o || (gi(n), o = !0);
         },
         o(l) {
             bi(n), o = !1;
         },
         d(l) {
-            l && Z_(i), ~e && s[e].d(l);
+            l && Y_(i), ~e && s[e].d(l);
         }
     };
 }
 
-function o0(t, e, n) {
+function s0(t, e, n) {
     let {
         currentVolume: i
     } = e;
     return t.$$set = (o) => {
         "currentVolume" in o && n(0, i = o.currentVolume);
     }, [i];
 }
-class r0 extends X_ {
+class l0 extends Z_ {
     constructor(e) {
-        super(), Q_(this, e, o0, i0, $_, {
+        super(), $_(this, e, s0, r0, t0, {
             currentVolume: 0
         });
     }
 }
 const {
-    SvelteComponent: s0,
+    SvelteComponent: a0,
     attr: Sn,
-    binding_callbacks: l0,
-    detach: a0,
-    element: u0,
-    init: c0,
-    insert: f0,
+    binding_callbacks: u0,
+    detach: c0,
+    element: f0,
+    init: d0,
+    insert: h0,
     listen: Ks,
     noop: $s,
-    run_all: d0,
-    safe_not_equal: h0
+    run_all: _0,
+    safe_not_equal: m0
 } = window.__gradio__svelte__internal, {
-    onMount: _0
+    onMount: p0
 } = window.__gradio__svelte__internal;
 
-function m0(t) {
+function g0(t) {
     let e, n, i;
     return {
         c() {
-            e = u0("input"), Sn(e, "id", "volume"), Sn(e, "class", "volume-slider svelte-1xy0951"), Sn(e, "type", "range"), Sn(e, "min", "0"), Sn(e, "max", "1"), Sn(e, "step", "0.01"), e.value = /*currentVolume*/
+            e = f0("input"), Sn(e, "id", "volume"), Sn(e, "class", "volume-slider svelte-1xy0951"), Sn(e, "type", "range"), Sn(e, "min", "0"), Sn(e, "max", "1"), Sn(e, "step", "0.01"), e.value = /*currentVolume*/
                 t[0];
         },
         m(o, r) {
-            f0(o, e, r), t[4](e), n || (i = [
+            h0(o, e, r), t[4](e), n || (i = [
                 Ks(
                     e,
                     "focusout",
                     /*focusout_handler*/
                     t[5]
                 ),
                 Ks(
@@ -5538,37 +5538,37 @@
             r & /*currentVolume*/
                 1 && (e.value = /*currentVolume*/
                     o[0]);
         },
         i: $s,
         o: $s,
         d(o) {
-            o && a0(e), t[4](null), n = !1, d0(i);
+            o && c0(e), t[4](null), n = !1, _0(i);
         }
     };
 }
 
-function p0(t, e, n) {
+function b0(t, e, n) {
     let {
         currentVolume: i = 1
     } = e, {
         show_volume_slider: o = !1
     } = e, {
         waveform: r
     } = e, s;
-    _0(() => {
+    p0(() => {
         a();
     });
     const a = () => {
         let f = s;
         f && (f.style.background = `linear-gradient(to right, var(--color-accent) ${i * 100}%, var(--neutral-400) ${i * 100}%)`);
     };
 
     function l(f) {
-        l0[f ? "unshift" : "push"](() => {
+        u0[f ? "unshift" : "push"](() => {
             s = f, n(3, s);
         });
     }
     const u = () => n(1, o = !1),
         c = (f) => {
             f.target instanceof HTMLInputElement && (n(0, i = parseFloat(f.target.value)), r.setVolume(i));
         };
@@ -5583,52 +5583,52 @@
         r,
         s,
         l,
         u,
         c
     ];
 }
-class g0 extends s0 {
+class v0 extends a0 {
     constructor(e) {
-        super(), c0(this, e, p0, m0, h0, {
+        super(), d0(this, e, b0, g0, m0, {
             currentVolume: 0,
             show_volume_slider: 1,
             waveform: 2
         });
     }
 }
 const {
-    SvelteComponent: b0,
+    SvelteComponent: w0,
     add_flush_callback: el,
     append: ye,
     attr: ue,
     bind: tl,
     binding_callbacks: nl,
     check_outros: il,
     create_component: $t,
     destroy_component: en,
     detach: $a,
     element: xe,
     group_outros: ol,
-    init: v0,
+    init: y0,
     insert: eu,
     listen: pt,
     mount_component: tn,
     run_all: tu,
-    safe_not_equal: w0,
-    set_data: y0,
+    safe_not_equal: k0,
+    set_data: E0,
     set_input_value: rl,
     space: Xt,
     text: sl,
-    to_number: k0,
+    to_number: C0,
     toggle_class: ll,
     transition_in: Je,
     transition_out: rt
 } = window.__gradio__svelte__internal, {
-    onMount: E0
+    onMount: S0
 } = window.__gradio__svelte__internal;
 
 function al(t) {
     let e, n, i, o;
 
     function r(l) {
         t[13](l);
@@ -5644,15 +5644,15 @@
         )
     };
     return (
         /*currentVolume*/
         t[8] !== void 0 && (a.currentVolume = /*currentVolume*/
             t[8]), /*show_volume_slider*/
         t[0] !== void 0 && (a.show_volume_slider = /*show_volume_slider*/
-            t[0]), e = new g0({
+            t[0]), e = new v0({
             props: a
         }), nl.push(() => tl(e, "currentVolume", r)), nl.push(() => tl(e, "show_volume_slider", s)), {
             c() {
                 $t(e.$$.fragment);
             },
             m(l, u) {
                 tn(e, l, u), o = !0;
@@ -5728,17 +5728,17 @@
         },
         d(o) {
             o && $a(e), n = !1, tu(i);
         }
     };
 }
 
-function C0(t) {
+function A0(t) {
     let e, n;
-    return e = new ah({}), {
+    return e = new ch({}), {
         c() {
             $t(e.$$.fragment);
         },
         m(i, o) {
             tn(e, i, o), n = !0;
         },
         i(i) {
@@ -5749,15 +5749,15 @@
         },
         d(i) {
             en(e, i);
         }
     };
 }
 
-function S0(t) {
+function T0(t) {
     let e, n;
     return e = new Ga({}), {
         c() {
             $t(e.$$.fragment);
         },
         m(i, o) {
             tn(e, i, o), n = !0;
@@ -5770,49 +5770,49 @@
         },
         d(i) {
             en(e, i);
         }
     };
 }
 
-function A0(t) {
-    let e, n, i, o, r, s, a, l, u, c, f, h, d, _, m, v, b, S, w, k, E, y, H, L, P, M, Z, x, j, X, C, G, I;
-    o = new r0({
+function P0(t) {
+    let e, n, i, o, r, s, a, l, u, c, f, h, d, _, m, b, g, S, w, k, E, y, H, L, P, D, J, Z, j, X, C, G, N;
+    o = new l0({
         props: {
             currentVolume: (
                 /*currentVolume*/
                 t[8]
             )
         }
     });
     let U = (
         /*show_volume_slider*/
         t[0] && al(t)
     );
-    m = new G_({});
-    let K = (
+    m = new V_({});
+    let $ = (
         /*showZoomSlider*/
         t[1] && ul(t)
     );
-    k = new Kf({});
-    const O = [S0, C0],
-        J = [];
+    k = new ed({});
+    const O = [T0, A0],
+        Y = [];
 
-    function le(p, A) {
+    function se(p, T) {
         return (
             /*playing*/
             p[5] ? 0 : 1
         );
     }
-    return L = le(t), P = J[L] = O[L](t), j = new Pd({}), {
+    return L = se(t), P = Y[L] = O[L](t), j = new Rd({}), {
         c() {
             e = xe("div"), n = xe("div"), i = xe("button"), $t(o.$$.fragment), r = Xt(), U && U.c(), s = Xt(), a = xe("button"), l = xe("span"), u = sl(
                 /*playbackSpeed*/
                 t[7]
-            ), c = sl("x"), h = Xt(), d = xe("div"), _ = xe("button"), $t(m.$$.fragment), v = Xt(), K && K.c(), b = Xt(), S = xe("div"), w = xe("button"), $t(k.$$.fragment), y = Xt(), H = xe("button"), P.c(), Z = Xt(), x = xe("button"), $t(j.$$.fragment), ue(i, "class", "action icon volume svelte-sgfovr"), ue(i, "aria-label", "Adjust volume"), ue(l, "class", "svelte-sgfovr"), ue(a, "class", "playback icon svelte-sgfovr"), ue(a, "aria-label", f = `Adjust playback speed to ${/*playbackSpeeds*/
+            ), c = sl("x"), h = Xt(), d = xe("div"), _ = xe("button"), $t(m.$$.fragment), b = Xt(), $ && $.c(), g = Xt(), S = xe("div"), w = xe("button"), $t(k.$$.fragment), y = Xt(), H = xe("button"), P.c(), J = Xt(), Z = xe("button"), $t(j.$$.fragment), ue(i, "class", "action icon volume svelte-sgfovr"), ue(i, "aria-label", "Adjust volume"), ue(l, "class", "svelte-sgfovr"), ue(a, "class", "playback icon svelte-sgfovr"), ue(a, "aria-label", f = `Adjust playback speed to ${/*playbackSpeeds*/
       t[10][
         /*playbackSpeeds*/
         (t[10].indexOf(
           /*playbackSpeed*/
           t[7]
         ) + 1) % /*playbackSpeeds*/
         t[10].length
@@ -5822,30 +5822,30 @@
                 /*show_volume_slider*/
                 t[0]
             ), ue(_, "class", "zoom-button icon svelte-sgfovr"), ue(d, "class", "zoom-wrapper svelte-sgfovr"), ue(n, "class", "control-wrapper svelte-sgfovr"), ue(w, "class", "rewind icon svelte-sgfovr"), ue(w, "aria-label", E = `Skip backwards by ${Ln(
         /*audio_duration*/
         t[3],
         /*waveform_options*/
         t[6].skip_length
-      )} seconds`), ue(H, "class", "play-pause-button icon svelte-sgfovr"), ue(H, "aria-label", M = /*playing*/
+      )} seconds`), ue(H, "class", "play-pause-button icon svelte-sgfovr"), ue(H, "aria-label", D = /*playing*/
                 t[5] ? (
                     /*i18n*/
                     t[4]("audio.pause")
                 ) : (
                     /*i18n*/
                     t[4]("audio.play")
-                )), ue(x, "class", "skip icon svelte-sgfovr"), ue(x, "aria-label", X = "Skip forward by " + Ln(
+                )), ue(Z, "class", "skip icon svelte-sgfovr"), ue(Z, "aria-label", X = "Skip forward by " + Ln(
                 /*audio_duration*/
                 t[3],
                 /*waveform_options*/
                 t[6].skip_length
             ) + " seconds"), ue(S, "class", "play-pause-wrapper svelte-sgfovr"), ue(e, "class", "controls svelte-sgfovr"), ue(e, "data-testid", "waveform-controls");
         },
-        m(p, A) {
-            eu(p, e, A), ye(e, n), ye(n, i), tn(o, i, null), ye(n, r), U && U.m(n, null), ye(n, s), ye(n, a), ye(a, l), ye(l, u), ye(l, c), ye(n, h), ye(n, d), ye(d, _), tn(m, _, null), ye(d, v), K && K.m(d, null), ye(e, b), ye(e, S), ye(S, w), tn(k, w, null), ye(S, y), ye(S, H), J[L].m(H, null), ye(S, Z), ye(S, x), tn(j, x, null), C = !0, G || (I = [
+        m(p, T) {
+            eu(p, e, T), ye(e, n), ye(n, i), tn(o, i, null), ye(n, r), U && U.m(n, null), ye(n, s), ye(n, a), ye(a, l), ye(l, u), ye(l, c), ye(n, h), ye(n, d), ye(d, _), tn(m, _, null), ye(d, b), $ && $.m(d, null), ye(e, g), ye(e, S), ye(S, w), tn(k, w, null), ye(S, y), ye(S, H), Y[L].m(H, null), ye(S, J), ye(S, Z), tn(j, Z, null), C = !0, G || (N = [
                 pt(
                     i,
                     "click",
                     /*click_handler*/
                     t[12]
                 ),
                 pt(
@@ -5869,92 +5869,92 @@
                 pt(
                     H,
                     "click",
                     /*click_handler_4*/
                     t[21]
                 ),
                 pt(
-                    x,
+                    Z,
                     "click",
                     /*click_handler_5*/
                     t[22]
                 )
             ], G = !0);
         },
-        p(p, [A]) {
+        p(p, [T]) {
             const q = {};
-            A & /*currentVolume*/
+            T & /*currentVolume*/
                 256 && (q.currentVolume = /*currentVolume*/
                     p[8]), o.$set(q), /*show_volume_slider*/
-                p[0] ? U ? (U.p(p, A), A & /*show_volume_slider*/
+                p[0] ? U ? (U.p(p, T), T & /*show_volume_slider*/
                     1 && Je(U, 1)) : (U = al(p), U.c(), Je(U, 1), U.m(n, s)) : U && (ol(), rt(U, 1, 1, () => {
                     U = null;
-                }), il()), (!C || A & /*playbackSpeed*/
-                    128) && y0(
+                }), il()), (!C || T & /*playbackSpeed*/
+                    128) && E0(
                     u,
                     /*playbackSpeed*/
                     p[7]
-                ), (!C || A & /*playbackSpeed*/
+                ), (!C || T & /*playbackSpeed*/
                     128 && f !== (f = `Adjust playback speed to ${/*playbackSpeeds*/
       p[10][
         /*playbackSpeeds*/
         (p[10].indexOf(
           /*playbackSpeed*/
           p[7]
         ) + 1) % /*playbackSpeeds*/
         p[10].length
-      ]}x`)) && ue(a, "aria-label", f), (!C || A & /*show_volume_slider*/
+      ]}x`)) && ue(a, "aria-label", f), (!C || T & /*show_volume_slider*/
                     1) && ll(
                     a,
                     "hidden",
                     /*show_volume_slider*/
                     p[0]
                 ), /*showZoomSlider*/
-                p[1] ? K ? K.p(p, A) : (K = ul(p), K.c(), K.m(d, null)) : K && (K.d(1), K = null), (!C || A & /*audio_duration, waveform_options*/
+                p[1] ? $ ? $.p(p, T) : ($ = ul(p), $.c(), $.m(d, null)) : $ && ($.d(1), $ = null), (!C || T & /*audio_duration, waveform_options*/
                     72 && E !== (E = `Skip backwards by ${Ln(
         /*audio_duration*/
         p[3],
         /*waveform_options*/
         p[6].skip_length
       )} seconds`)) && ue(w, "aria-label", E);
             let z = L;
-            L = le(p), L !== z && (ol(), rt(J[z], 1, 1, () => {
-                J[z] = null;
-            }), il(), P = J[L], P || (P = J[L] = O[L](p), P.c()), Je(P, 1), P.m(H, null)), (!C || A & /*playing, i18n*/
-                48 && M !== (M = /*playing*/
+            L = se(p), L !== z && (ol(), rt(Y[z], 1, 1, () => {
+                Y[z] = null;
+            }), il(), P = Y[L], P || (P = Y[L] = O[L](p), P.c()), Je(P, 1), P.m(H, null)), (!C || T & /*playing, i18n*/
+                48 && D !== (D = /*playing*/
                     p[5] ? (
                         /*i18n*/
                         p[4]("audio.pause")
                     ) : (
                         /*i18n*/
                         p[4]("audio.play")
-                    ))) && ue(H, "aria-label", M), (!C || A & /*audio_duration, waveform_options*/
+                    ))) && ue(H, "aria-label", D), (!C || T & /*audio_duration, waveform_options*/
                 72 && X !== (X = "Skip forward by " + Ln(
                     /*audio_duration*/
                     p[3],
                     /*waveform_options*/
                     p[6].skip_length
-                ) + " seconds")) && ue(x, "aria-label", X);
+                ) + " seconds")) && ue(Z, "aria-label", X);
         },
         i(p) {
             C || (Je(o.$$.fragment, p), Je(U), Je(m.$$.fragment, p), Je(k.$$.fragment, p), Je(P), Je(j.$$.fragment, p), C = !0);
         },
         o(p) {
             rt(o.$$.fragment, p), rt(U), rt(m.$$.fragment, p), rt(k.$$.fragment, p), rt(P), rt(j.$$.fragment, p), C = !1;
         },
         d(p) {
-            p && $a(e), en(o), U && U.d(), en(m), K && K.d(), en(k), J[L].d(), en(j), G = !1, tu(I);
+            p && $a(e), en(o), U && U.d(), en(m), $ && $.d(), en(k), Y[L].d(), en(j), G = !1, tu(N);
         }
     };
 }
 let Ir = 10,
     Ur = 1e4,
     cl = 100;
 
-function T0(t, e, n) {
+function L0(t, e, n) {
     let {
         waveform: i
     } = e, {
         audio_duration: o
     } = e, {
         i18n: r
     } = e, {
@@ -5963,105 +5963,105 @@
         waveform_options: a = {}
     } = e, {
         show_volume_slider: l = !1
     } = e, {
         showZoomSlider: u = !1
     } = e, c = [0.5, 1, 1.5, 2], f = c[1], h = 1, d = 10;
 
-    function _(M) {
-        n(9, d = M), d < Ir ? n(9, d = Ir) : d > Ur && n(9, d = Ur), i.zoom(d);
+    function _(D) {
+        n(9, d = D), d < Ir ? n(9, d = Ir) : d > Ur && n(9, d = Ur), i.zoom(d);
     }
-    E0(() => {
-        window.addEventListener("keydown", (M) => {
-            switch (M.key) {
+    S0(() => {
+        window.addEventListener("keydown", (D) => {
+            switch (D.key) {
                 case " ":
-                    i.playPause(), M.preventDefault();
+                    i.playPause(), D.preventDefault();
                     break;
                 case "ArrowUp":
-                    M.preventDefault(), _(d + cl);
+                    D.preventDefault(), _(d + cl);
                     break;
                 case "ArrowDown":
-                    M.preventDefault(), _(d - cl);
+                    D.preventDefault(), _(d - cl);
                     break;
             }
         });
     });
     const m = () => n(0, l = !l);
 
-    function v(M) {
-        h = M, n(8, h);
+    function b(D) {
+        h = D, n(8, h);
     }
 
-    function b(M) {
-        l = M, n(0, l);
+    function g(D) {
+        l = D, n(0, l);
     }
     const S = () => {
             n(7, f = c[(c.indexOf(f) + 1) % c.length]), i.setPlaybackRate(f);
         },
         w = () => n(1, u = !u);
 
     function k() {
-        d = k0(this.value), n(9, d);
+        d = C0(this.value), n(9, d);
     }
-    const E = (M) => _(M.target.value),
+    const E = (D) => _(D.target.value),
         y = () => n(1, u = !1),
         H = () => i.skip(Ln(o, a.skip_length) * -1),
         L = () => i.playPause(),
         P = () => i.skip(Ln(o, a.skip_length));
-    return t.$$set = (M) => {
-        "waveform" in M && n(2, i = M.waveform), "audio_duration" in M && n(3, o = M.audio_duration), "i18n" in M && n(4, r = M.i18n), "playing" in M && n(5, s = M.playing), "waveform_options" in M && n(6, a = M.waveform_options), "show_volume_slider" in M && n(0, l = M.show_volume_slider), "showZoomSlider" in M && n(1, u = M.showZoomSlider);
+    return t.$$set = (D) => {
+        "waveform" in D && n(2, i = D.waveform), "audio_duration" in D && n(3, o = D.audio_duration), "i18n" in D && n(4, r = D.i18n), "playing" in D && n(5, s = D.playing), "waveform_options" in D && n(6, a = D.waveform_options), "show_volume_slider" in D && n(0, l = D.show_volume_slider), "showZoomSlider" in D && n(1, u = D.showZoomSlider);
     }, [
         l,
         u,
         i,
         o,
         r,
         s,
         a,
         f,
         h,
         d,
         c,
         _,
         m,
-        v,
         b,
+        g,
         S,
         w,
         k,
         E,
         y,
         H,
         L,
         P
     ];
 }
-class nu extends b0 {
+class nu extends w0 {
     constructor(e) {
-        super(), v0(this, e, T0, A0, w0, {
+        super(), y0(this, e, L0, P0, k0, {
             waveform: 2,
             audio_duration: 3,
             i18n: 4,
             playing: 5,
             waveform_options: 6,
             show_volume_slider: 0,
             showZoomSlider: 1
         });
     }
 }
 const {
-    setContext: Yv,
-    getContext: P0
-} = window.__gradio__svelte__internal, L0 = "WORKER_PROXY_CONTEXT_KEY";
+    setContext: Y2,
+    getContext: R0
+} = window.__gradio__svelte__internal, B0 = "WORKER_PROXY_CONTEXT_KEY";
 
 function iu() {
-    return P0(L0);
+    return R0(B0);
 }
 
-function R0(t) {
+function M0(t) {
     return t.host === window.location.host || t.host === "localhost:7860" || t.host === "127.0.0.1:7860" || // Ref: https://github.com/gradio-app/gradio/blob/v3.32.0/js/app/src/Index.svelte#L194
         t.host === "lite.local";
 }
 
 function ou(t, e) {
     const n = e.toLowerCase();
     for (const [i, o] of Object.entries(t))
@@ -6069,15 +6069,15 @@
             return o;
 }
 
 function ru(t) {
     if (t == null)
         return !1;
     const e = new URL(t, window.location.href);
-    return !(!R0(e) || e.protocol !== "http:" && e.protocol !== "https:");
+    return !(!M0(e) || e.protocol !== "http:" && e.protocol !== "https:");
 }
 async function fl(t) {
     if (t == null || !ru(t))
         return t;
     const e = iu();
     if (e == null)
         return t;
@@ -6093,41 +6093,41 @@
         const r = new Blob([o.body], {
             type: ou(o.headers, "content-type")
         });
         return URL.createObjectURL(r);
     });
 }
 const {
-    SvelteComponent: B0,
+    SvelteComponent: D0,
     assign: oo,
     check_outros: su,
     compute_rest_props: dl,
     create_slot: rs,
     detach: yo,
     element: lu,
     empty: au,
-    exclude_internal_props: M0,
+    exclude_internal_props: H0,
     get_all_dirty_from_scope: ss,
     get_slot_changes: ls,
     get_spread_update: uu,
     group_outros: cu,
-    init: D0,
+    init: O0,
     insert: ko,
     listen: fu,
-    prevent_default: H0,
-    safe_not_equal: O0,
+    prevent_default: N0,
+    safe_not_equal: I0,
     set_attributes: ro,
     transition_in: cn,
     transition_out: fn,
     update_slot_base: as
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: N0
+    createEventDispatcher: U0
 } = window.__gradio__svelte__internal;
 
-function I0(t) {
+function j0(t) {
     let e, n, i, o, r;
     const s = (
             /*#slots*/
             t[8].default
         ),
         a = rs(
             s,
@@ -6220,17 +6220,17 @@
         },
         d(c) {
             c && yo(e), a && a.d(c), o = !1, r();
         }
     };
 }
 
-function U0(t) {
+function F0(t) {
     let e, n, i, o;
-    const r = [F0, j0],
+    const r = [z0, q0],
         s = [];
 
     function a(l, u) {
         return (
             /*is_downloading*/
             l[2] ? 0 : 1
         );
@@ -6256,15 +6256,15 @@
         },
         d(l) {
             l && yo(i), s[e].d(l);
         }
     };
 }
 
-function j0(t) {
+function q0(t) {
     let e, n, i, o;
     const r = (
             /*#slots*/
             t[8].default
         ),
         s = rs(
             r,
@@ -6286,15 +6286,15 @@
     for (let u = 0; u < a.length; u += 1)
         l = oo(l, a[u]);
     return {
         c() {
             e = lu("a"), s && s.c(), ro(e, l);
         },
         m(u, c) {
-            ko(u, e, c), s && s.m(e, null), n = !0, i || (o = fu(e, "click", H0(
+            ko(u, e, c), s && s.m(e, null), n = !0, i || (o = fu(e, "click", N0(
                 /*wasm_click_handler*/
                 t[5]
             )), i = !0);
         },
         p(u, c) {
             s && s.p && (!n || c & /*$$scope*/
                 128) && as(
@@ -6335,15 +6335,15 @@
         },
         d(u) {
             u && yo(e), s && s.d(u), i = !1, o();
         }
     };
 }
 
-function F0(t) {
+function z0(t) {
     let e;
     const n = (
             /*#slots*/
             t[8].default
         ),
         i = rs(
             n,
@@ -6388,17 +6388,17 @@
         },
         d(o) {
             i && i.d(o);
         }
     };
 }
 
-function q0(t) {
+function G0(t) {
     let e, n, i, o, r;
-    const s = [U0, I0],
+    const s = [F0, j0],
         a = [];
 
     function l(u, c) {
         return c & /*href*/
             1 && (e = null), e == null && (e = !! /*worker_proxy*/
                 (u[4] && ru(
                     /*href*/
@@ -6426,28 +6426,28 @@
         },
         d(u) {
             u && yo(o), a[n].d(u);
         }
     };
 }
 
-function z0(t, e, n) {
+function W0(t, e, n) {
     const i = ["href", "download"];
     let o = dl(e, i),
         {
             $$slots: r = {},
             $$scope: s
         } = e,
         {
             href: a = void 0
         } = e,
         {
             download: l
         } = e;
-    const u = N0();
+    const u = U0();
     let c = !1;
     const f = iu();
     async function h() {
         if (c)
             return;
         if (u("click"), a == null)
             throw new Error("href is not defined.");
@@ -6458,234 +6458,234 @@
             method: "GET",
             path: _,
             headers: {},
             query_string: ""
         }).then((m) => {
             if (m.status !== 200)
                 throw new Error(`Failed to get file ${_} from the Wasm worker.`);
-            const v = new Blob(
+            const b = new Blob(
                     [m.body], {
                         type: ou(m.headers, "content-type")
                     }
                 ),
-                b = URL.createObjectURL(v),
+                g = URL.createObjectURL(b),
                 S = document.createElement("a");
-            S.href = b, S.download = l, S.click(), URL.revokeObjectURL(b);
+            S.href = g, S.download = l, S.click(), URL.revokeObjectURL(g);
         }).finally(() => {
             n(2, c = !1);
         });
     }
     return t.$$set = (d) => {
-        e = oo(oo({}, e), M0(d)), n(6, o = dl(e, i)), "href" in d && n(0, a = d.href), "download" in d && n(1, l = d.download), "$$scope" in d && n(7, s = d.$$scope);
+        e = oo(oo({}, e), H0(d)), n(6, o = dl(e, i)), "href" in d && n(0, a = d.href), "download" in d && n(1, l = d.download), "$$scope" in d && n(7, s = d.$$scope);
     }, [
         a,
         l,
         c,
         u,
         f,
         h,
         o,
         s,
         r
     ];
 }
-class du extends B0 {
+class du extends D0 {
     constructor(e) {
-        super(), D0(this, e, z0, q0, O0, {
+        super(), O0(this, e, W0, G0, I0, {
             href: 0,
             download: 1
         });
     }
 }
 const {
-    SvelteComponent: G0,
+    SvelteComponent: V0,
     append: hl,
     attr: kt,
-    detach: W0,
-    init: V0,
-    insert: X0,
+    detach: X0,
+    init: x0,
+    insert: Z0,
     noop: hr,
-    safe_not_equal: x0,
+    safe_not_equal: J0,
     svg_element: _r
 } = window.__gradio__svelte__internal;
 
-function Z0(t) {
+function Y0(t) {
     let e, n, i;
     return {
         c() {
             e = _r("svg"), n = _r("g"), i = _r("path"), kt(i, "d", `M41.267,18.557H26.832V4.134C26.832,1.851,24.99,0,22.707,0c-2.283,0-4.124,1.851-4.124,4.135v14.432H4.141\r
 		c-2.283,0-4.139,1.851-4.138,4.135c-0.001,1.141,0.46,2.187,1.207,2.934c0.748,0.749,1.78,1.222,2.92,1.222h14.453V41.27\r
 		c0,1.142,0.453,2.176,1.201,2.922c0.748,0.748,1.777,1.211,2.919,1.211c2.282,0,4.129-1.851,4.129-4.133V26.857h14.435\r
 		c2.283,0,4.134-1.867,4.133-4.15C45.399,20.425,43.548,18.557,41.267,18.557z`), kt(e, "version", "1.1"), kt(e, "id", "Capa_1"), kt(e, "xmlns", "http://www.w3.org/2000/svg"), kt(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), kt(e, "width", "100%"), kt(e, "height", "100%"), kt(e, "viewBox", "0 10 45.402 45.402	"), kt(e, "xml:space", "preserve");
         },
         m(o, r) {
-            X0(o, e, r), hl(e, n), hl(n, i);
+            Z0(o, e, r), hl(e, n), hl(n, i);
         },
         p: hr,
         i: hr,
         o: hr,
         d(o) {
-            o && W0(e);
+            o && X0(e);
         }
     };
 }
-class J0 extends G0 {
+class Q0 extends V0 {
     constructor(e) {
-        super(), V0(this, e, null, Z0, x0, {});
+        super(), x0(this, e, null, Y0, J0, {});
     }
 }
 const {
-    SvelteComponent: Y0,
+    SvelteComponent: K0,
     append: Vi,
     attr: Xi,
-    binding_callbacks: Q0,
-    create_component: K0,
-    destroy_component: $0,
-    detach: em,
+    binding_callbacks: $0,
+    create_component: em,
+    destroy_component: tm,
+    detach: nm,
     element: xi,
-    init: tm,
-    insert: nm,
-    listen: im,
-    mount_component: om,
-    noop: rm,
-    safe_not_equal: sm,
-    space: lm,
-    transition_in: am,
-    transition_out: um
+    init: im,
+    insert: om,
+    listen: rm,
+    mount_component: sm,
+    noop: lm,
+    safe_not_equal: am,
+    space: um,
+    transition_in: cm,
+    transition_out: fm
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: cm,
-    onMount: fm
+    createEventDispatcher: dm,
+    onMount: hm
 } = window.__gradio__svelte__internal;
 
-function dm(t) {
+function _m(t) {
     let e, n, i, o, r, s, a, l, u;
-    return s = new J0({}), {
+    return s = new Q0({}), {
         c() {
-            e = xi("div"), n = xi("div"), i = lm(), o = xi("div"), r = xi("button"), K0(s.$$.fragment), Xi(n, "class", "caption svelte-43he0g"), Xi(r, "class", "create-label svelte-43he0g"), Xi(o, "class", "action-buttons svelte-43he0g"), Xi(e, "class", "caption-container svelte-43he0g");
+            e = xi("div"), n = xi("div"), i = um(), o = xi("div"), r = xi("button"), em(s.$$.fragment), Xi(n, "class", "caption svelte-43he0g"), Xi(r, "class", "create-label svelte-43he0g"), Xi(o, "class", "action-buttons svelte-43he0g"), Xi(e, "class", "caption-container svelte-43he0g");
         },
         m(c, f) {
-            nm(c, e, f), Vi(e, n), t[5](n), Vi(e, i), Vi(e, o), Vi(o, r), om(s, r, null), a = !0, l || (u = im(
+            om(c, e, f), Vi(e, n), t[5](n), Vi(e, i), Vi(e, o), Vi(o, r), sm(s, r, null), a = !0, l || (u = rm(
                 r,
                 "click",
                 /*click_handler*/
                 t[6]
             ), l = !0);
         },
-        p: rm,
+        p: lm,
         i(c) {
-            a || (am(s.$$.fragment, c), a = !0);
+            a || (cm(s.$$.fragment, c), a = !0);
         },
         o(c) {
-            um(s.$$.fragment, c), a = !1;
+            fm(s.$$.fragment, c), a = !1;
         },
         d(c) {
-            c && em(e), t[5](null), $0(s), l = !1, u();
+            c && nm(e), t[5](null), tm(s), l = !1, u();
         }
     };
 }
 
-function hm(t, e, n) {
+function mm(t, e, n) {
     let {
-        value: i = null
+        annotations: i = null
     } = e, o, r = [], s = null, a = 0;
     const l = [
             "rgba(255, 215, 0, 0.5)",
             "rgba(0, 0, 255, 0.5)",
             "rgba(255, 0, 0, 0.5)",
             "rgba(0, 255, 0, 0.5)"
         ],
-        u = cm();
+        u = dm();
 
-    function c(v) {
-        const b = document.createElement("button");
-        b.style.backgroundColor = v.color, b.classList.add("captionLabel"), b.id = v.shortcut, b.innerHTML = '<span style="font-weight: bold;">' + v.shortcut + "</span>: " + v.speaker, b.addEventListener("focusin", () => {
-            d(v.shortcut);
-        }), b.addEventListener("focusout", () => {
+    function c(b) {
+        const g = document.createElement("button");
+        g.style.backgroundColor = b.color, g.classList.add("captionLabel"), g.id = b.shortcut, g.innerHTML = '<span style="font-weight: bold;">' + b.shortcut + "</span>: " + b.speaker, g.addEventListener("focusin", () => {
+            d(b.shortcut);
+        }), g.addEventListener("focusout", () => {
             d("Escape");
-        }), o.appendChild(b);
+        }), o.appendChild(g);
     }
 
-    function f(v, b, S) {
+    function f(b, g, S) {
         if (r.length === 26)
             return;
-        if (v || (v = "SPEAKER_" + a.toString().padStart(2, "0")), b || (b = l[a % l.length]), !S)
+        if (b || (b = "LABEL_" + a.toString().padStart(2, "0")), g || (g = l[a % l.length]), !S)
             for (S = "A"; r.some((k) => k.shortcut === S) && S !== "Z";)
                 S = String.fromCharCode(S.charCodeAt(0) + 1);
         const w = {
-            speaker: v,
-            color: b,
+            speaker: b,
+            color: g,
             shortcut: S
         };
         return r.push(w), c(w), a++, w;
     }
 
-    function h(v) {
-        s && document.getElementById(s.shortcut).classList.remove("active-button"), s = v, document.getElementById(s.shortcut).classList.add("active-button"), u("select", s);
+    function h(b) {
+        s && document.getElementById(s.shortcut).classList.remove("active-button"), s = b, document.getElementById(s.shortcut).classList.add("active-button"), u("select", s);
     }
 
-    function d(v) {
-        let b = null;
-        v !== "Escape" && (b = r.find((S) => S.shortcut === v.toUpperCase()), b || (b = f(void 0, void 0, v.toUpperCase()))), h(b);
+    function d(b) {
+        let g = null;
+        b !== "Escape" && (g = r.find((S) => S.shortcut === b.toUpperCase()), g || (g = f(void 0, void 0, b.toUpperCase()))), h(g);
     }
-    fm(() => {
-        window.addEventListener("keydown", (v) => {
-            (v.key.match(/^[a-zA-Z]$/) || v.key === "Escape") && d(v.key);
+    hm(() => {
+        window.addEventListener("keydown", (b) => {
+            (b.key.match(/^[a-zA-Z]$/) || b.key === "Escape") && d(b.key);
         });
     });
 
-    function _(v) {
-        Q0[v ? "unshift" : "push"](() => {
-            o = v, n(1, o);
+    function _(b) {
+        $0[b ? "unshift" : "push"](() => {
+            o = b, n(1, o);
         });
     }
     const m = () => {
-        const v = f();
-        h(v);
+        const b = f();
+        h(b);
     };
-    return t.$$set = (v) => {
-        "value" in v && n(3, i = v.value);
+    return t.$$set = (b) => {
+        "annotations" in b && n(3, i = b.annotations);
     }, t.$$.update = () => {
-        t.$$.dirty & /*container, value, labels*/
-            26 && o && i && (i.forEach((v) => {
-                r.some((b) => b.speaker === v.speaker) || f(v.speaker, v.color);
-            }), n(4, r = r.sort((v, b) => v.shortcut.localeCompare(b.shortcut))));
+        t.$$.dirty & /*container, annotations, labels*/
+            26 && o && i && (i.forEach((b) => {
+                r.some((g) => g.speaker === b.speaker) || f(b.speaker, b.color);
+            }), n(4, r = r.sort((b, g) => b.shortcut.localeCompare(g.shortcut))));
     }, [
         f,
         o,
         h,
         i,
         r,
         _,
         m
     ];
 }
-class _m extends Y0 {
+class pm extends K0 {
     constructor(e) {
-        super(), tm(this, e, hm, dm, sm, {
-            value: 3,
+        super(), im(this, e, mm, _m, am, {
+            annotations: 3,
             createLabel: 0
         });
     }
     get createLabel() {
         return this.$$.ctx[0];
     }
 }
 const {
-    SvelteComponent: mm,
-    add_flush_callback: pm,
+    SvelteComponent: gm,
+    add_flush_callback: hu,
     append: Ye,
-    attr: ie,
-    bind: gm,
-    binding_callbacks: mi,
+    attr: oe,
+    bind: _u,
+    binding_callbacks: Rn,
     check_outros: so,
     create_component: dn,
     destroy_component: hn,
     detach: ut,
     element: je,
-    empty: hu,
+    empty: mu,
     group_outros: lo,
     init: bm,
     insert: ct,
     listen: jr,
     mount_component: _n,
     noop: _l,
     run_all: vm,
@@ -6703,30 +6703,30 @@
 function Em(t) {
     let e, n, i, o, r, s, a, l, u, c, f, h, d = (
         /*waveform*/
         t[9] && pl(t)
     );
     return {
         c() {
-            e = je("div"), n = je("div"), i = je("div"), o = sn(), r = je("div"), s = je("time"), s.textContent = "0:00", a = sn(), l = je("div"), u = je("time"), u.textContent = "0:00", c = sn(), d && d.c(), ie(i, "id", "waveform"), ie(i, "class", "svelte-1w83umt"), ie(n, "class", "waveform-container svelte-1w83umt"), ie(s, "id", "time"), ie(s, "class", "svelte-1w83umt"), ie(u, "id", "duration"), ie(u, "class", "svelte-1w83umt"), ie(r, "class", "timestamps svelte-1w83umt"), ie(e, "class", "component-wrapper svelte-1w83umt"), ie(e, "data-testid", f = /*label*/
+            e = je("div"), n = je("div"), i = je("div"), o = sn(), r = je("div"), s = je("time"), s.textContent = "0:00", a = sn(), l = je("div"), u = je("time"), u.textContent = "0:00", c = sn(), d && d.c(), oe(i, "id", "waveform"), oe(i, "class", "svelte-15fy58k"), oe(n, "class", "waveform-container svelte-15fy58k"), oe(s, "id", "time"), oe(s, "class", "svelte-15fy58k"), oe(u, "id", "duration"), oe(u, "class", "svelte-15fy58k"), oe(r, "class", "timestamps svelte-15fy58k"), oe(e, "class", "component-wrapper svelte-15fy58k"), oe(e, "data-testid", f = /*label*/
                 t[2] ? "waveform-" + /*label*/
                 t[2] : "unlabelled-audio");
         },
         m(_, m) {
             ct(_, e, m), Ye(e, n), Ye(n, i), t[25](i), Ye(e, o), Ye(e, r), Ye(r, s), t[26](s), Ye(r, a), Ye(r, l), Ye(l, u), t[27](u), Ye(e, c), d && d.m(e, null), h = !0;
         },
         p(_, m) {
             /*waveform*/
             _[9] ? d ? (d.p(_, m), m[0] & /*waveform*/
                 512 && Ee(d, 1)) : (d = pl(_), d.c(), Ee(d, 1), d.m(e, null)) : d && (lo(), Me(d, 1, 1, () => {
                 d = null;
             }), so()), (!h || m[0] & /*label*/
                 4 && f !== (f = /*label*/
                     _[2] ? "waveform-" + /*label*/
-                    _[2] : "unlabelled-audio")) && ie(e, "data-testid", f);
+                    _[2] : "unlabelled-audio")) && oe(e, "data-testid", f);
         },
         i(_) {
             h || (Ee(d), h = !0);
         },
         o(_) {
             Me(d), h = !1;
         },
@@ -6736,25 +6736,25 @@
     };
 }
 
 function Cm(t) {
     let e, n, i;
     return {
         c() {
-            e = je("audio"), ie(e, "class", "standard-player svelte-1w83umt"), ml(e.src, n = /*value*/
-                    t[0].file_data.url) || ie(e, "src", n), e.controls = !0, e.autoplay = i = /*waveform_settings*/
+            e = je("audio"), oe(e, "class", "standard-player svelte-15fy58k"), ml(e.src, n = /*value*/
+                    t[0].file_data.url) || oe(e, "src", n), e.controls = !0, e.autoplay = i = /*waveform_settings*/
                 t[6].autoplay;
         },
         m(o, r) {
             ct(o, e, r);
         },
         p(o, r) {
             r[0] & /*value*/
                 1 && !ml(e.src, n = /*value*/
-                    o[0].file_data.url) && ie(e, "src", n), r[0] & /*waveform_settings*/
+                    o[0].file_data.url) && oe(e, "src", n), r[0] & /*waveform_settings*/
                 64 && i !== (i = /*waveform_settings*/
                     o[6].autoplay) && (e.autoplay = i);
         },
         i: _l,
         o: _l,
         d(o) {
             o && ut(e);
@@ -6780,15 +6780,15 @@
         },
         m(i, o) {
             _n(e, i, o), n = !0;
         },
         p(i, o) {
             const r = {};
             o[1] & /*$$scope*/
-                16777216 && (r.$$scope = {
+                33554432 && (r.$$scope = {
                     dirty: o,
                     ctx: i
                 }), e.$set(r);
         },
         i(i) {
             n || (Ee(e.$$.fragment, i), n = !0);
         },
@@ -6829,47 +6829,47 @@
             t[7]
         )
     };
     /*show_volume_slider*/
     t[14] !== void 0 && (f.show_volume_slider = /*show_volume_slider*/
         t[14]), i = new nu({
         props: f
-    }), mi.push(() => gm(i, "show_volume_slider", c));
+    }), Rn.push(() => _u(i, "show_volume_slider", c));
     let h = (
             /*editable*/
             t[5] && /*interactive*/
             t[4] && /*value*/
             t[0] && gl(t)
         ),
         d = (
             /*value*/
             t[0] && bl(t)
         );
     return {
         c() {
-            e = je("div"), n = je("div"), dn(i.$$.fragment), r = sn(), s = je("div"), h && h.c(), a = sn(), d && d.c(), l = hu(), ie(n, "class", "waveform-controls svelte-1w83umt"), ie(s, "class", "regions-actions svelte-1w83umt"), ie(e, "class", "commands svelte-1w83umt");
+            e = je("div"), n = je("div"), dn(i.$$.fragment), r = sn(), s = je("div"), h && h.c(), a = sn(), d && d.c(), l = mu(), oe(n, "class", "waveform-controls svelte-15fy58k"), oe(s, "class", "regions-actions svelte-15fy58k"), oe(e, "class", "commands svelte-15fy58k");
         },
         m(_, m) {
             ct(_, e, m), Ye(e, n), _n(i, n, null), Ye(e, r), Ye(e, s), h && h.m(s, null), ct(_, a, m), d && d.m(_, m), ct(_, l, m), u = !0;
         },
         p(_, m) {
-            const v = {};
+            const b = {};
             m[0] & /*waveform*/
-                512 && (v.waveform = /*waveform*/
+                512 && (b.waveform = /*waveform*/
                     _[9]), m[0] & /*playing*/
-                8192 && (v.playing = /*playing*/
+                8192 && (b.playing = /*playing*/
                     _[13]), m[0] & /*audio_duration*/
-                4096 && (v.audio_duration = /*audio_duration*/
+                4096 && (b.audio_duration = /*audio_duration*/
                     _[12]), m[0] & /*i18n*/
-                8 && (v.i18n = /*i18n*/
+                8 && (b.i18n = /*i18n*/
                     _[3]), m[0] & /*waveform_options*/
-                128 && (v.waveform_options = /*waveform_options*/
+                128 && (b.waveform_options = /*waveform_options*/
                     _[7]), !o && m[0] & /*show_volume_slider*/
-                16384 && (o = !0, v.show_volume_slider = /*show_volume_slider*/
-                    _[14], pm(() => o = !1)), i.$set(v), /*editable*/
+                16384 && (o = !0, b.show_volume_slider = /*show_volume_slider*/
+                    _[14], hu(() => o = !1)), i.$set(b), /*editable*/
                 _[5] && /*interactive*/
                 _[4] && /*value*/
                 _[0] ? h ? (h.p(_, m), m[0] & /*editable, interactive, value*/
                     49 && Ee(h, 1)) : (h = gl(_), h.c(), Ee(h, 1), h.m(s, null)) : h && (lo(), Me(h, 1, 1, () => {
                     h = null;
                 }), so()), /*value*/
                 _[0] ? d ? (d.p(_, m), m[0] & /*value*/
@@ -6890,18 +6890,18 @@
 }
 
 function gl(t) {
     let e, n, i, o, r, s, a, l, u, c, f, h = (
         /*showRedo*/
         t[17] && Am(t)
     );
-    return i = new P_({}), a = new mh({}), {
+    return i = new R_({}), a = new gh({}), {
         c() {
-            h && h.c(), e = sn(), n = je("button"), dn(i.$$.fragment), r = sn(), s = je("button"), dn(a.$$.fragment), ie(n, "class", "action icon remove-button svelte-1w83umt"), ie(n, "aria-label", "Remove an annotation"), ie(n, "title", o = /*i18n*/
-                t[3]("Remove an annotation")), ie(s, "class", "action icon trim-button svelte-1w83umt"), ie(s, "aria-label", "Split an annotation"), ie(s, "title", l = /*i18n*/
+            h && h.c(), e = sn(), n = je("button"), dn(i.$$.fragment), r = sn(), s = je("button"), dn(a.$$.fragment), oe(n, "class", "action icon remove-button svelte-15fy58k"), oe(n, "aria-label", "Remove an annotation"), oe(n, "title", o = /*i18n*/
+                t[3]("Remove an annotation")), oe(s, "class", "action icon trim-button svelte-15fy58k"), oe(s, "aria-label", "Split an annotation"), oe(s, "title", l = /*i18n*/
                 t[3]("Split an annotation"));
         },
         m(d, _) {
             h && h.m(d, _), ct(d, e, _), ct(d, n, _), _n(i, n, null), ct(d, r, _), ct(d, s, _), _n(a, s, null), u = !0, c || (f = [
                 jr(
                     n,
                     "click",
@@ -6916,17 +6916,17 @@
                 )
             ], c = !0);
         },
         p(d, _) {
             /*showRedo*/
             d[17] && h.p(d, _), (!u || _[0] & /*i18n*/
                 8 && o !== (o = /*i18n*/
-                    d[3]("Remove an annotation"))) && ie(n, "title", o), (!u || _[0] & /*i18n*/
+                    d[3]("Remove an annotation"))) && oe(n, "title", o), (!u || _[0] & /*i18n*/
                 8 && l !== (l = /*i18n*/
-                    d[3]("Split an annotation"))) && ie(s, "title", l);
+                    d[3]("Split an annotation"))) && oe(s, "title", l);
         },
         i(d) {
             u || (Ee(h), Ee(i.$$.fragment, d), Ee(a.$$.fragment, d), u = !0);
         },
         o(d) {
             Me(h), Me(i.$$.fragment, d), Me(a.$$.fragment, d), u = !1;
         },
@@ -6936,82 +6936,86 @@
     };
 }
 
 function Am(t) {
     let e, n, i, o, r, s;
     return n = new Wa({}), {
         c() {
-            e = je("button"), dn(n.$$.fragment), ie(e, "class", "action icon svelte-1w83umt"), ie(e, "aria-label", "Reset annotations"), ie(e, "title", i = /*i18n*/
+            e = je("button"), dn(n.$$.fragment), oe(e, "class", "action icon svelte-15fy58k"), oe(e, "aria-label", "Reset annotations"), oe(e, "title", i = /*i18n*/
                 t[3]("Reset annotations"));
         },
         m(a, l) {
             ct(a, e, l), _n(n, e, null), o = !0, r || (s = jr(
                 e,
                 "click",
                 /*resetRegions*/
                 t[18]
             ), r = !0);
         },
         p(a, l) {
             (!o || l[0] & /*i18n*/
                 8 && i !== (i = /*i18n*/
-                    a[3]("Reset annotations"))) && ie(e, "title", i);
+                    a[3]("Reset annotations"))) && oe(e, "title", i);
         },
         i(a) {
             o || (Ee(n.$$.fragment, a), o = !0);
         },
         o(a) {
             Me(n.$$.fragment, a), o = !1;
         },
         d(a) {
             a && ut(e), hn(n), r = !1, s();
         }
     };
 }
 
 function bl(t) {
-    let e, n, i = {
-        value: (
-            /*value*/
-            t[0].annotations
-        )
-    };
-    return e = new _m({
-        props: i
-    }), t[31](e), e.$on(
-        "select",
-        /*select_handler*/
-        t[32]
-    ), e.$on(
-        "select",
-        /*select_handler_1*/
-        t[33]
-    ), {
-        c() {
-            dn(e.$$.fragment);
-        },
-        m(o, r) {
-            _n(e, o, r), n = !0;
-        },
-        p(o, r) {
-            const s = {};
-            r[0] & /*value*/
-                1 && (s.value = /*value*/
-                    o[0].annotations), e.$set(s);
-        },
-        i(o) {
-            n || (Ee(e.$$.fragment, o), n = !0);
-        },
-        o(o) {
-            Me(e.$$.fragment, o), n = !1;
-        },
-        d(o) {
-            t[31](null), hn(e, o);
+    let e, n, i;
+
+    function o(s) {
+        t[32](s);
+    }
+    let r = {};
+    return (
+        /*value*/
+        t[0].annotations !== void 0 && (r.annotations = /*value*/
+            t[0].annotations), e = new pm({
+            props: r
+        }), t[31](e), Rn.push(() => _u(e, "annotations", o)), e.$on(
+            "select",
+            /*select_handler*/
+            t[33]
+        ), e.$on(
+            "select",
+            /*select_handler_1*/
+            t[34]
+        ), {
+            c() {
+                dn(e.$$.fragment);
+            },
+            m(s, a) {
+                _n(e, s, a), i = !0;
+            },
+            p(s, a) {
+                const l = {};
+                !n && a[0] & /*value*/
+                    1 && (n = !0, l.annotations = /*value*/
+                        s[0].annotations, hu(() => n = !1)), e.$set(l);
+            },
+            i(s) {
+                i || (Ee(e.$$.fragment, s), i = !0);
+            },
+            o(s) {
+                Me(e.$$.fragment, s), i = !1;
+            },
+            d(s) {
+                t[31](null), hn(e, s);
+            }
         }
-    };
+    );
 }
 
 function Tm(t) {
     let e, n;
     return e = new mo({}), {
         c() {
             dn(e.$$.fragment);
@@ -7043,15 +7047,15 @@
                 /*value*/
                 l[0].file_data.is_stream ? 1 : 2
             )
         );
     }
     return e = a(t), n = s[e] = r[e](t), {
         c() {
-            n.c(), i = hu();
+            n.c(), i = mu();
         },
         m(l, u) {
             s[e].m(l, u), ct(l, i, u), o = !0;
         },
         p(l, u) {
             let c = e;
             e = a(l), e === c ? s[e].p(l, u) : (lo(), Me(s[c], 1, 1, () => {
@@ -7111,394 +7115,389 @@
         {
             waveform_options: c
         } = e,
         {
             mode: f = ""
         } = e,
         h, d, _, m = null,
-        v, b, S, w, k, E = !1,
+        b, g, S, w, k, E = !1,
         y = !1,
         H = a,
         L = null,
         P = /* @__PURE__ */ new Map(),
-        M, Z = null,
-        x = null;
+        D, J = null,
+        Z = null;
     const j = km();
 
     function X() {
         n(9, d = Ft.create({
             container: h,
             ...u
-        })), fl(pe([o, "access", (g) => g.file_data, "optionalAccess", (g) => g.url])).then((g) => {
-            if (g && d)
-                return d.load(g);
+        })), fl(pe([o, "access", (v) => v.file_data, "optionalAccess", (v) => v.url])).then((v) => {
+            if (v && d)
+                return d.load(v);
         }), d.on("dblclick", () => {
             U(d.getCurrentTime());
         });
     }
 
-    function C(g) {
-        if (L || (L = [...g]), g.length === 0)
+    function C(v) {
+        if (L || (L = [...v]), v.length === 0)
             return;
-        Z = {
-            speaker: g[0].speaker,
-            color: g[0].color,
+        J = {
+            speaker: v[0].speaker,
+            color: v[0].color,
             shortcut: "A"
         };
-        const T = Array.from(P.values());
-        g = g.filter((D) => !T.some((N) => D.start === N.start && D.end === N.end && D.speaker === N.speaker)), g.forEach((D) => {
-            let N = I({
-                    start: D.start,
-                    end: D.end,
-                    color: D.color,
+        const A = Array.from(P.values());
+        v = v.filter((R) => !A.some((I) => R.start === I.start && R.end === I.end && R.speaker === I.speaker)), v.forEach((R) => {
+            let I = N({
+                    start: R.start,
+                    end: R.end,
+                    color: R.color,
                     drag: !0,
                     resize: !0
                 },
-                D.speaker
+                R.speaker
             );
-            N.element.style.top = (D.level * 10).toString() + "%", N.element.style.height = (100 - (D.numLevels + 1) * 10).toString() + "%";
+            I.element.style.top = (R.level * 10).toString() + "%", I.element.style.height = (100 - (R.numLevels + 1) * 10).toString() + "%";
         });
     }
 
     function G() {
         n(0, o.annotations = Array.from(P.values()), o), j("edit", o);
     }
 
-    function I(g, T) {
-        let D = _.addRegion(g);
-        const N = {
-            start: D.start,
-            end: D.end,
-            speaker: T,
-            color: D.color
+    function N(v, A) {
+        let R = _.addRegion(v);
+        const I = {
+            start: R.start,
+            end: R.end,
+            speaker: A,
+            color: R.color
         };
-        return P.set(D.id, N), L || (L = [N]), G(), D;
+        return P.set(R.id, I), L || (L = [I]), G(), R;
     }
 
-    function U(g) {
-        let T = x !== null ? x : Z;
-        if (T === null) {
-            window.alert('First create a label by clicking on "+" or by pressing A-Z');
-            return;
-        }
-        let D = I({
-                start: g - 1,
-                end: g + 1,
-                color: T.color,
+    function U(v) {
+        let A = Z || J;
+        A || (A = D.createLabel());
+        let R = N({
+                start: v - 1,
+                end: v + 1,
+                color: A.color,
                 drag: !0,
                 resize: !0
             },
-            T.speaker
+            A.speaker
         );
-        p(D);
+        p(R);
     }
 
-    function K(g) {
-        g === m && p(null), P.delete(g.id), g.remove(), G();
+    function $(v) {
+        v === m && p(null), P.delete(v.id), v.remove(), G();
     }
 
-    function O(g, T) {
+    function O(v, A) {
         if (!m)
             return;
-        let D = _.getRegions().find((N) => N.id === m.id);
-        g === "Delete" || g == "Backspace" && T ? q(!1) : q(!0), K(D);
+        let R = _.getRegions().find((I) => I.id === m.id);
+        v === "Delete" || v == "Backspace" && A ? q(!1) : q(!0), $(R);
     }
 
-    function J() {
-        le(), L.forEach((g) => o.annotations.push(Object.assign({}, g))), C(o.annotations), j("edit", o);
+    function Y() {
+        se(), L.forEach((v) => o.annotations.push(Object.assign({}, v))), C(o.annotations), j("edit", o);
     }
 
-    function le() {
-        p(null), pe([_, "optionalAccess", (g) => g.clearRegions, "call", (g) => g()]), n(0, o.annotations = [], o), P.clear();
+    function se() {
+        p(null), pe([_, "optionalAccess", (v) => v.clearRegions, "call", (v) => v()]), n(0, o.annotations = [], o), P.clear();
     }
 
-    function p(g) {
-        if (m !== null && n(21, m.element.style.background = m.color, m), g === null) {
-            n(21, m = g);
-            return;
-        }
-        n(21, m = g), n(21, m.element.style.background = "repeating-linear-gradient(45deg," + g.color + " ," + g.color + " 10px, #ffffff 10px ,#ffffff 15px)", m);
+    function p(v) {
+        m && n(21, m.element.style.background = m.color, m), n(21, m = v), m && n(21, m.element.style.background = "repeating-linear-gradient(45deg," + v.color + " ," + v.color + " 10px, #ffffff 10px ,#ffffff 15px)", m);
     }
 
-    function A(g) {
+    function T(v) {
         if (m !== null) {
             m.setOptions({
                 start: m.start,
                 end: m.end,
-                color: g.color,
+                color: v.color,
                 drag: !0,
                 resize: !0
             }), n(21, m.element.style.background = "repeating-linear-gradient(45deg," + m.color + " ," + m.color + " 10px, #ffffff 10px ,#ffffff 15px)", m);
-            let T = P.get(m.id);
-            T.color = g.color, T.speaker = g.speaker, G();
+            let A = P.get(m.id);
+            A.color = v.color, A.speaker = v.speaker, G();
         }
     }
 
-    function q(g) {
-        var T = g ? -1 : 1,
-            D = _.getRegions().sort((te, oe) => te.start > oe.start ? 1 : -1);
+    function q(v) {
+        var A = v ? -1 : 1,
+            R = _.getRegions().sort((ee, x) => ee.start > x.start ? 1 : -1);
         if (m === null)
-            p(D[0]);
+            p(R[0]);
         else {
-            var N = D.indexOf(m);
-            p(D.at((N + T) % D.length));
+            var I = R.indexOf(m);
+            p(R.at((I + A) % R.length));
         }
     }
 
-    function z(g, T) {
-        if (T < g.start || T > g.end)
+    function z(v, A) {
+        if (A < v.start || A > v.end)
             throw new RangeError("split time out of region bounds");
-        let D = P.get(g.id).speaker;
-        I({
-                start: g.start,
-                end: T,
-                color: g.color,
-                drag: g.drag,
-                resize: g.resize
+        let R = P.get(v.id).speaker;
+        N({
+                start: v.start,
+                end: A,
+                color: v.color,
+                drag: v.drag,
+                resize: v.resize
             },
-            D
+            R
         );
-        let N = I({
-                start: T,
-                end: g.end,
-                color: g.color,
-                drag: g.drag,
-                resize: g.resize
+        let I = N({
+                start: A,
+                end: v.end,
+                color: v.color,
+                drag: v.drag,
+                resize: v.resize
             },
-            D
+            R
         );
-        p(N), K(g);
+        p(I), $(v);
     }
 
-    function he(g) {
-        let T = _.getRegions().find((D) => D.start < g && D.end > g);
-        if (T === void 0) {
+    function he(v) {
+        let A = _.getRegions().find((R) => R.start < v && R.end > v);
+        if (A === void 0) {
             if (m === null)
                 return;
-            T = m, g = T.start + (T.end - T.start) / 2;
+            A = m, v = A.start + (A.end - A.start) / 2;
         }
-        z(T, g);
+        z(A, v);
     }
 
-    function _e(g, T, D) {
-        let N, te, oe = 0.05;
-        T && (oe = oe * 4), D ? g === "ArrowLeft" ? (N = m.start, te = m.end - oe) : (N = m.start, te = m.end + oe) : g === "ArrowLeft" ? (N = m.start - oe, te = m.end) : (N = m.start + oe, te = m.end), N > m.end && (N = m.end - 0.1), te < m.start && (te = m.start + 0.1), m.setOptions({
-            start: N,
-            end: te
+    function _e(v, A, R) {
+        let I, ee, x = 0.05;
+        A && (x = x * 4), R ? v === "ArrowLeft" ? (I = m.start, ee = m.end - x) : (I = m.start, ee = m.end + x) : v === "ArrowLeft" ? (I = m.start - x, ee = m.end) : (I = m.start + x, ee = m.end), I > m.end && (I = m.end - 0.1), ee < m.start && (ee = m.start + 0.1), m.setOptions({
+            start: I,
+            end: ee
         });
     }
 
-    function F(g, T) {
-        let D = d.getCurrentTime(),
-            N, te = 0.05;
-        T && (te = te * 4), g === "ArrowLeft" ? N = D - te : N = D + te, d.setTime(N);
+    function F(v, A) {
+        let R = d.getCurrentTime(),
+            I, ee = 0.05;
+        A && (ee = ee * 4), v === "ArrowLeft" ? I = R - ee : I = R + ee, d.setTime(I);
     }
 
-    function ve(g, T, D) {
+    function ve(v, A, R) {
         if (m) {
-            _e(g, T, D);
+            _e(v, A, R);
             return;
         }
-        F(g, T);
+        F(v, A);
     }
-    async function B(g) {
-        await fl(g).then((T) => {
-            if (!(!T || pe([
+    async function M(v) {
+        await fl(v).then((A) => {
+            if (!(!A || pe([
                     o,
                     "access",
-                    (D) => D.file_data,
+                    (R) => R.file_data,
                     "optionalAccess",
-                    (D) => D.is_stream
+                    (R) => R.is_stream
                 ])))
                 return pe([
                     d,
                     "optionalAccess",
-                    (D) => D.load,
+                    (R) => R.load,
                     "call",
-                    (D) => D(T)
+                    (R) => R(A)
                 ]);
         });
     }
     ym(() => {
-        window.addEventListener("keydown", (g) => {
-            switch (g.key) {
+        window.addEventListener("keydown", (v) => {
+            switch (v.key) {
                 case "ArrowLeft":
-                    ve("ArrowLeft", g.shiftKey, g.altKey);
+                    ve("ArrowLeft", v.shiftKey, v.altKey);
                     break;
                 case "ArrowRight":
-                    ve("ArrowRight", g.shiftKey, g.altKey);
+                    ve("ArrowRight", v.shiftKey, v.altKey);
                     break;
                 case "Escape":
                     p(null);
                     break;
                 case "Tab":
-                    g.preventDefault(), q(g.shiftKey);
+                    v.preventDefault(), q(v.shiftKey);
                     break;
                 case "Delete":
-                    O("Delete", g.shiftKey);
+                    O("Delete", v.shiftKey);
                     break;
                 case "Backspace":
-                    O("Backspace", g.shiftKey);
+                    O("Backspace", v.shiftKey);
                     break;
                 case "Enter":
-                    g.preventDefault(), g.shiftKey ? he(d.getCurrentTime()) : U(d.getCurrentTime());
+                    v.preventDefault(), v.shiftKey ? he(d.getCurrentTime()) : U(d.getCurrentTime());
                     break;
             }
         });
     });
 
-    function R(g) {
-        mi[g ? "unshift" : "push"](() => {
-            h = g, n(8, h), n(9, d);
+    function B(v) {
+        Rn[v ? "unshift" : "push"](() => {
+            h = v, n(8, h), n(9, d);
         });
     }
 
-    function ce(g) {
-        mi[g ? "unshift" : "push"](() => {
-            S = g, n(10, S), n(9, d);
+    function ce(v) {
+        Rn[v ? "unshift" : "push"](() => {
+            S = v, n(10, S), n(9, d);
         });
     }
 
-    function Se(g) {
-        mi[g ? "unshift" : "push"](() => {
-            w = g, n(11, w), n(9, d);
+    function Se(v) {
+        Rn[v ? "unshift" : "push"](() => {
+            w = v, n(11, w), n(9, d);
         });
     }
 
-    function wt(g) {
-        y = g, n(14, y);
+    function wt(v) {
+        y = v, n(14, y);
     }
-    const Y = () => n(1, f = "remove"),
+    const Q = () => n(1, f = "remove"),
         yt = () => n(1, f = "split");
 
-    function wn(g) {
-        mi[g ? "unshift" : "push"](() => {
-            M = g, n(15, M);
+    function wn(v) {
+        Rn[v ? "unshift" : "push"](() => {
+            D = v, n(15, D);
         });
     }
-    const ei = (g) => A(g.detail),
-        ti = (g) => n(16, x = g.detail);
-    return t.$$set = (g) => {
-        "value" in g && n(0, o = g.value), "label" in g && n(2, r = g.label), "i18n" in g && n(3, s = g.i18n), "interactive" in g && n(4, a = g.interactive), "editable" in g && n(5, l = g.editable), "waveform_settings" in g && n(6, u = g.waveform_settings), "waveform_options" in g && n(7, c = g.waveform_options), "mode" in g && n(1, f = g.mode);
+
+    function ti(v) {
+        t.$$.not_equal(o.annotations, v) && (o.annotations = v, n(0, o));
+    }
+    const ni = (v) => T(v.detail),
+        le = (v) => n(16, Z = v.detail);
+    return t.$$set = (v) => {
+        "value" in v && n(0, o = v.value), "label" in v && n(2, r = v.label), "i18n" in v && n(3, s = v.i18n), "interactive" in v && n(4, a = v.interactive), "editable" in v && n(5, l = v.editable), "waveform_settings" in v && n(6, u = v.waveform_settings), "waveform_options" in v && n(7, c = v.waveform_options), "mode" in v && n(1, f = v.mode);
     }, t.$$.update = () => {
         if (t.$$.dirty[0] & /*value*/
-            1 && n(24, i = pe([o, "access", (g) => g.file_data, "optionalAccess", (g) => g.url])), t.$$.dirty[0] & /*container, waveform*/
-            768 && h !== void 0 && (d !== void 0 && d.destroy(), n(8, h.innerHTML = "", h), X(), n(13, E = !1)), t.$$.dirty[0] & /*waveform, wsRegions, waveform_settings*/
-            1049152 && pe([
+            1 && n(24, i = pe([o, "access", (v) => v.file_data, "optionalAccess", (v) => v.url])), t.$$.dirty[0] & /*container, waveform*/
+            768 && h !== void 0 && (d !== void 0 && d.destroy(), n(8, h.innerHTML = "", h), X(), n(13, E = !1)), t.$$.dirty[0] & /*waveform, wsRegions, mode, waveform_settings*/
+            1049154 && pe([
                 d,
                 "optionalAccess",
-                (g) => g.on,
+                (v) => v.on,
                 "call",
-                (g) => g("ready", () => {
-                    _ === void 0 && n(20, _ = d.registerPlugin(O_.create())), u.autoplay ? pe([d, "optionalAccess", (T) => T.play, "call", (T) => T()]) : pe([d, "optionalAccess", (T) => T.stop, "call", (T) => T()]);
+                (v) => v("ready", () => {
+                    _ === void 0 && (n(20, _ = d.registerPlugin(I_.create())), pe([
+                        _,
+                        "optionalAccess",
+                        (A) => A.on,
+                        "call",
+                        (A) => A("region-clicked", (R, I) => {
+                            switch (f) {
+                                case "remove":
+                                    $(R);
+                                    break;
+                                case "split":
+                                    z(R, R.start + (R.end - R.start) / 2);
+                                    break;
+                                default:
+                                    p(R), R.play();
+                            }
+                            n(1, f = "");
+                        })
+                    ]), pe([
+                        _,
+                        "optionalAccess",
+                        (A) => A.on,
+                        "call",
+                        (A) => A("region-updated", (R) => {
+                            var I = P.get(R.id);
+                            I.start = R.start, I.end = R.end, G();
+                        })
+                    ])), u.autoplay ? pe([d, "optionalAccess", (A) => A.play, "call", (A) => A()]) : pe([d, "optionalAccess", (A) => A.stop, "call", (A) => A()]);
                 })
             ]), t.$$.dirty[0] & /*value, wsRegions*/
-            1048577 && pe([o, "optionalAccess", (g) => g.annotations]) !== null && _ && C(o.annotations), t.$$.dirty[0] & /*waveform, durationRef*/
+            1048577 && pe([o, "optionalAccess", (v) => v.annotations]) !== null && _ && C(o.annotations), t.$$.dirty[0] & /*waveform, durationRef*/
             2560 && pe([
                 d,
                 "optionalAccess",
-                (g) => g.on,
+                (v) => v.on,
                 "call",
-                (g) => g("decode", (T) => {
-                    n(12, k = T), w && n(11, w.textContent = vl(T), w);
+                (v) => v("decode", (A) => {
+                    n(12, k = A), w && n(11, w.textContent = vl(A), w);
                 })
             ]), t.$$.dirty[0] & /*waveform, timeRef*/
             1536 && pe([
                 d,
                 "optionalAccess",
-                (g) => g.on,
+                (v) => v.on,
                 "call",
-                (g) => g("timeupdate", (T) => S && n(10, S.textContent = vl(T), S))
+                (v) => v("timeupdate", (A) => S && n(10, S.textContent = vl(A), S))
             ]), t.$$.dirty[0] & /*waveform*/
             512 && pe([
                 d,
                 "optionalAccess",
-                (g) => g.on,
+                (v) => v.on,
                 "call",
-                (g) => g("finish", () => {
+                (v) => v("finish", () => {
                     n(13, E = !1), j("stop");
                 })
             ]), t.$$.dirty[0] & /*waveform*/
             512 && pe([
                 d,
                 "optionalAccess",
-                (g) => g.on,
+                (v) => v.on,
                 "call",
-                (g) => g("pause", () => {
+                (v) => v("pause", () => {
                     n(13, E = !1), j("pause");
                 })
             ]), t.$$.dirty[0] & /*waveform*/
             512 && pe([
                 d,
                 "optionalAccess",
-                (g) => g.on,
+                (v) => v.on,
                 "call",
-                (g) => g("play", () => {
+                (v) => v("play", () => {
                     n(13, E = !0), j("play");
                 })
-            ]), t.$$.dirty[0] & /*wsRegions*/
-            1048576 && pe([
-                _,
-                "optionalAccess",
-                (g) => g.on,
-                "call",
-                (g) => g("region-updated", (T) => {
-                    var D = P.get(T.id);
-                    D.start = T.start, D.end = T.end, G();
-                })
-            ]), t.$$.dirty[0] & /*wsRegions, mode*/
-            1048578 && pe([
-                _,
-                "optionalAccess",
-                (g) => g.on,
-                "call",
-                (g) => g("region-clicked", (T, D) => {
-                    switch (f) {
-                        case "remove":
-                            K(T);
-                            break;
-                        case "split":
-                            z(T, T.start + (T.end - T.start) / 2);
-                            break;
-                        default:
-                            p(T), T.play();
-                    }
-                    n(1, f = "");
-                })
             ]), t.$$.dirty[0] & /*activeRegion, container, leftRegionHandle, rightRegionHandle, wsRegions*/
             15728896 && m) {
-            const g = h.children[0].shadowRoot;
-            n(23, b = g.querySelector('[data-resize="right"]')), n(22, v = g.querySelector('[data-resize="left"]')), v && b && (v.setAttribute("role", "button"), b.setAttribute("role", "button"), pe([
-                v,
+            const v = h.children[0].shadowRoot;
+            n(23, g = v.querySelector('[data-resize="right"]')), n(22, b = v.querySelector('[data-resize="left"]')), b && g && (b.setAttribute("role", "button"), g.setAttribute("role", "button"), pe([
+                b,
                 "optionalAccess",
-                (T) => T.setAttribute,
+                (A) => A.setAttribute,
                 "call",
-                (T) => T("aria-label", "Drag to adjust start time")
+                (A) => A("aria-label", "Drag to adjust start time")
             ]), pe([
-                b,
+                g,
                 "optionalAccess",
-                (T) => T.setAttribute,
+                (A) => A.setAttribute,
                 "call",
-                (T) => T("aria-label", "Drag to adjust end time")
+                (A) => A("aria-label", "Drag to adjust end time")
             ]), pe([
-                v,
+                b,
                 "optionalAccess",
-                (T) => T.setAttribute,
+                (A) => A.setAttribute,
                 "call",
-                (T) => T("tabindex", "0")
+                (A) => A("tabindex", "0")
             ]), pe([
-                b,
+                g,
                 "optionalAccess",
-                (T) => T.setAttribute,
+                (A) => A.setAttribute,
                 "call",
-                (T) => T("tabindex", "0")
-            ]), v.addEventListener("focus", () => {}), b.addEventListener("focus", () => {}));
+                (A) => A("tabindex", "0")
+            ]), b.addEventListener("focus", () => {}), g.addEventListener("focus", () => {}));
         }
         t.$$.dirty[0] & /*url*/
-            16777216 && i && B(i);
+            16777216 && i && M(i);
     }, [
         o,
         f,
         r,
         s,
         a,
         l,
@@ -7507,36 +7506,37 @@
         h,
         d,
         S,
         w,
         k,
         E,
         y,
-        M,
-        x,
+        D,
+        Z,
         H,
-        J,
-        A,
+        Y,
+        T,
         _,
         m,
-        v,
         b,
+        g,
         i,
-        R,
+        B,
         ce,
         Se,
         wt,
-        Y,
+        Q,
         yt,
         wn,
-        ei,
-        ti
+        ti,
+        ni,
+        le
     ];
 }
-class _u extends mm {
+class pu extends gm {
     constructor(e) {
         super(), bm(
             this,
             e,
             Lm,
             Pm,
             wm, {
@@ -7553,26 +7553,26 @@
             [-1, -1]
         );
     }
 }
 const {
     SvelteComponent: Rm,
     append: Bm,
-    attr: mu,
-    bubble: li,
-    check_outros: pu,
-    create_component: Zn,
-    destroy_component: Jn,
+    attr: gu,
+    bubble: ai,
+    check_outros: bu,
+    create_component: Jn,
+    destroy_component: Yn,
     detach: vi,
-    element: gu,
+    element: vu,
     empty: Mm,
-    group_outros: bu,
+    group_outros: wu,
     init: Dm,
     insert: wi,
-    mount_component: Yn,
+    mount_component: Qn,
     safe_not_equal: Hm,
     space: Fr,
     transition_in: Ke,
     transition_out: ft
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: Om
 } = window.__gradio__svelte__internal;
@@ -7587,18 +7587,18 @@
             },
             $$scope: {
                 ctx: t
             }
         }
     }), {
         c() {
-            Zn(e.$$.fragment);
+            Jn(e.$$.fragment);
         },
         m(i, o) {
-            Yn(e, i, o), n = !0;
+            Qn(e, i, o), n = !0;
         },
         p(i, o) {
             const r = {};
             o & /*$$scope*/
                 16384 && (r.$$scope = {
                     dirty: o,
                     ctx: i
@@ -7607,27 +7607,27 @@
         i(i) {
             n || (Ke(e.$$.fragment, i), n = !0);
         },
         o(i) {
             ft(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            Jn(e, i);
+            Yn(e, i);
         }
     };
 }
 
 function Im(t) {
     let e, n, i, o, r, s = (
             /*show_download_button*/
             t[3] && /*value*/
             t[0].file_data !== null && wl(t)
         ),
         a = qm;
-    return o = new _u({
+    return o = new pu({
         props: {
             value: (
                 /*value*/
                 t[0]
             ),
             interactive: !1,
             label: (
@@ -7657,26 +7657,26 @@
         t[11]
     ), o.$on(
         "stop",
         /*stop_handler*/
         t[12]
     ), {
         c() {
-            e = gu("div"), s && s.c(), n = Fr(), i = Fr(), Zn(o.$$.fragment), mu(e, "class", "icon-buttons svelte-1mrvp2o");
+            e = vu("div"), s && s.c(), n = Fr(), i = Fr(), Jn(o.$$.fragment), gu(e, "class", "icon-buttons svelte-1mrvp2o");
         },
         m(l, u) {
-            wi(l, e, u), s && s.m(e, null), Bm(e, n), wi(l, i, u), Yn(o, l, u), r = !0;
+            wi(l, e, u), s && s.m(e, null), Bm(e, n), wi(l, i, u), Qn(o, l, u), r = !0;
         },
         p(l, u) {
             /*show_download_button*/
             l[3] && /*value*/
                 l[0].file_data !== null ? s ? (s.p(l, u), u & /*show_download_button, value*/
-                    9 && Ke(s, 1)) : (s = wl(l), s.c(), Ke(s, 1), s.m(e, n)) : s && (bu(), ft(s, 1, 1, () => {
+                    9 && Ke(s, 1)) : (s = wl(l), s.c(), Ke(s, 1), s.m(e, n)) : s && (wu(), ft(s, 1, 1, () => {
                     s = null;
-                }), pu());
+                }), bu());
             const c = {};
             u & /*value*/
                 1 && (c.value = /*value*/
                     l[0]), u & /*label*/
                 2 && (c.label = /*label*/
                     l[1]), u & /*i18n*/
                 16 && (c.i18n = /*i18n*/
@@ -7689,36 +7689,36 @@
         i(l) {
             r || (Ke(s), Ke(a), Ke(o.$$.fragment, l), r = !0);
         },
         o(l) {
             ft(s), ft(a), ft(o.$$.fragment, l), r = !1;
         },
         d(l) {
-            l && (vi(e), vi(i)), s && s.d(), Jn(o, l);
+            l && (vi(e), vi(i)), s && s.d(), Yn(o, l);
         }
     };
 }
 
 function Um(t) {
     let e, n;
     return e = new mo({}), {
         c() {
-            Zn(e.$$.fragment);
+            Jn(e.$$.fragment);
         },
         m(i, o) {
-            Yn(e, i, o), n = !0;
+            Qn(e, i, o), n = !0;
         },
         i(i) {
             n || (Ke(e.$$.fragment, i), n = !0);
         },
         o(i) {
             ft(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            Jn(e, i);
+            Yn(e, i);
         }
     };
 }
 
 function wl(t) {
     let e, n, i;
     return n = new du({
@@ -7737,18 +7737,18 @@
             },
             $$scope: {
                 ctx: t
             }
         }
     }), {
         c() {
-            e = gu("div"), Zn(n.$$.fragment), mu(e, "class", "download-button");
+            e = vu("div"), Jn(n.$$.fragment), gu(e, "class", "download-button");
         },
         m(o, r) {
-            wi(o, e, r), Yn(n, e, null), i = !0;
+            wi(o, e, r), Qn(n, e, null), i = !0;
         },
         p(o, r) {
             const s = {};
             r & /*value*/
                 1 && (s.href = /*value*/
                     o[0].file_data.url), r & /*value*/
                 1 && (s.download = /*value*/
@@ -7762,15 +7762,15 @@
         i(o) {
             i || (Ke(n.$$.fragment, o), i = !0);
         },
         o(o) {
             ft(n.$$.fragment, o), i = !1;
         },
         d(o) {
-            o && vi(e), Jn(n);
+            o && vi(e), Yn(n);
         }
     };
 }
 
 function jm(t) {
     let e, n;
     return e = new Ei({
@@ -7779,33 +7779,33 @@
             label: (
                 /*i18n*/
                 t[4]("common.download")
             )
         }
     }), {
         c() {
-            Zn(e.$$.fragment);
+            Jn(e.$$.fragment);
         },
         m(i, o) {
-            Yn(e, i, o), n = !0;
+            Qn(e, i, o), n = !0;
         },
         p(i, o) {
             const r = {};
             o & /*i18n*/
                 16 && (r.label = /*i18n*/
                     i[4]("common.download")), e.$set(r);
         },
         i(i) {
             n || (Ke(e.$$.fragment, i), n = !0);
         },
         o(i) {
             ft(e.$$.fragment, i), n = !1;
         },
         d(i) {
-            Jn(e, i);
+            Yn(e, i);
         }
     };
 }
 
 function Fm(t) {
     let e, n, i, o, r, s;
     e = new Ia({
@@ -7830,40 +7830,40 @@
         return (
             /*value*/
             c[0] !== null ? 0 : 1
         );
     }
     return i = u(t), o = l[i] = a[i](t), {
         c() {
-            Zn(e.$$.fragment), n = Fr(), o.c(), r = Mm();
+            Jn(e.$$.fragment), n = Fr(), o.c(), r = Mm();
         },
         m(c, f) {
-            Yn(e, c, f), wi(c, n, f), l[i].m(c, f), wi(c, r, f), s = !0;
+            Qn(e, c, f), wi(c, n, f), l[i].m(c, f), wi(c, r, f), s = !0;
         },
         p(c, [f]) {
             const h = {};
             f & /*show_label*/
                 4 && (h.show_label = /*show_label*/
                     c[2]), f & /*label, i18n*/
                 18 && (h.label = /*label*/
                     c[1] || /*i18n*/
                     c[4]("audio.audio")), e.$set(h);
             let d = i;
-            i = u(c), i === d ? l[i].p(c, f) : (bu(), ft(l[d], 1, 1, () => {
+            i = u(c), i === d ? l[i].p(c, f) : (wu(), ft(l[d], 1, 1, () => {
                 l[d] = null;
-            }), pu(), o = l[i], o ? o.p(c, f) : (o = l[i] = a[i](c), o.c()), Ke(o, 1), o.m(r.parentNode, r));
+            }), bu(), o = l[i], o ? o.p(c, f) : (o = l[i] = a[i](c), o.c()), Ke(o, 1), o.m(r.parentNode, r));
         },
         i(c) {
             s || (Ke(e.$$.fragment, c), Ke(o), s = !0);
         },
         o(c) {
             ft(e.$$.fragment, c), ft(o), s = !1;
         },
         d(c) {
-            c && (vi(n), vi(r)), Jn(e, c), l[i].d(c);
+            c && (vi(n), vi(r)), Yn(e, c), l[i].d(c);
         }
     };
 }
 let qm = !1;
 
 function zm(t, e, n) {
     let {
@@ -7878,37 +7878,37 @@
         i18n: a
     } = e, {
         waveform_settings: l
     } = e, {
         waveform_options: u
     } = e;
     const c = Om(),
-        f = async (b) => b ? `<audio controls src="${await Oc(b.url, "url")}"></audio>` : "";
+        f = async (g) => g ? `<audio controls src="${await Ic(g.url, "url")}"></audio>` : "";
 
-    function h(b) {
-        li.call(this, t, b);
+    function h(g) {
+        ai.call(this, t, g);
     }
 
-    function d(b) {
-        li.call(this, t, b);
+    function d(g) {
+        ai.call(this, t, g);
     }
 
-    function _(b) {
-        li.call(this, t, b);
+    function _(g) {
+        ai.call(this, t, g);
     }
 
-    function m(b) {
-        li.call(this, t, b);
+    function m(g) {
+        ai.call(this, t, g);
     }
 
-    function v(b) {
-        li.call(this, t, b);
+    function b(g) {
+        ai.call(this, t, g);
     }
-    return t.$$set = (b) => {
-        "value" in b && n(0, i = b.value), "label" in b && n(1, o = b.label), "show_label" in b && n(2, r = b.show_label), "show_download_button" in b && n(3, s = b.show_download_button), "i18n" in b && n(4, a = b.i18n), "waveform_settings" in b && n(5, l = b.waveform_settings), "waveform_options" in b && n(6, u = b.waveform_options);
+    return t.$$set = (g) => {
+        "value" in g && n(0, i = g.value), "label" in g && n(1, o = g.label), "show_label" in g && n(2, r = g.show_label), "show_download_button" in g && n(3, s = g.show_download_button), "i18n" in g && n(4, a = g.i18n), "waveform_settings" in g && n(5, l = g.waveform_settings), "waveform_options" in g && n(6, u = g.waveform_options);
     }, t.$$.update = () => {
         t.$$.dirty & /*value*/
             1 && i && c("change", i);
     }, [
         i,
         o,
         r,
@@ -7917,15 +7917,15 @@
         l,
         u,
         f,
         h,
         d,
         _,
         m,
-        v
+        b
     ];
 }
 class Gm extends Rm {
     constructor(e) {
         super(), Dm(this, e, zm, Fm, Hm, {
             value: 0,
             label: 1,
@@ -7961,36 +7961,36 @@
         for (const i of e)
             i(void 0);
         return ln;
     }
     const n = t.subscribe(...e);
     return n.unsubscribe ? () => n.unsubscribe() : n;
 }
-const vu = typeof window < "u";
-let yl = vu ? () => window.performance.now() : () => Date.now(),
-    wu = vu ? (t) => requestAnimationFrame(t) : ln;
-const On = /* @__PURE__ */ new Set();
-
-function yu(t) {
-    On.forEach((e) => {
-        e.c(t) || (On.delete(e), e.f());
-    }), On.size !== 0 && wu(yu);
+const yu = typeof window < "u";
+let yl = yu ? () => window.performance.now() : () => Date.now(),
+    ku = yu ? (t) => requestAnimationFrame(t) : ln;
+const Nn = /* @__PURE__ */ new Set();
+
+function Eu(t) {
+    Nn.forEach((e) => {
+        e.c(t) || (Nn.delete(e), e.f());
+    }), Nn.size !== 0 && ku(Eu);
 }
 
 function Jm(t) {
     let e;
-    return On.size === 0 && wu(yu), {
+    return Nn.size === 0 && ku(Eu), {
         promise: new Promise((n) => {
-            On.add(e = {
+            Nn.add(e = {
                 c: t,
                 f: n
             });
         }),
         abort() {
-            On.delete(e);
+            Nn.delete(e);
         }
     };
 }
 const An = [];
 
 function Ym(t, e) {
     return {
@@ -8028,15 +8028,15 @@
     return {
         set: o,
         update: r,
         subscribe: s
     };
 }
 
-function Qn(t, e, n) {
+function Kn(t, e, n) {
     const i = !Array.isArray(t),
         o = i ? [t] : t;
     if (!o.every(Boolean))
         throw new Error("derived() expects stores as input, got a falsy value");
     const r = e.length < 2;
     return Ym(n, (s, a) => {
         let l = !1;
@@ -8049,16 +8049,16 @@
                 f();
                 const _ = e(i ? u[0] : u, s, a);
                 r ? s(_) : f = Xm(_) ? _ : ln;
             },
             d = o.map(
                 (_, m) => Zm(
                     _,
-                    (v) => {
-                        u[m] = v, c &= ~(1 << m), l && h();
+                    (b) => {
+                        u[m] = b, c &= ~(1 << m), l && h();
                     },
                     () => {
                         c |= 1 << m;
                     }
                 )
             );
         return l = !0, h(),
@@ -8105,18 +8105,18 @@
         } = e;
     let s, a, l, u = t,
         c = t,
         f = 1,
         h = 0,
         d = !1;
 
-    function _(v, b = {}) {
-        c = v;
+    function _(b, g = {}) {
+        c = b;
         const S = l = {};
-        return t == null || b.hard || m.stiffness >= 1 && m.damping >= 1 ? (d = !0, s = yl(), u = v, n.set(t = c), Promise.resolve()) : (b.soft && (h = 1 / ((b.soft === !0 ? 0.5 : +b.soft) * 60), f = 0), a || (s = yl(), d = !1, a = Jm((w) => {
+        return t == null || g.hard || m.stiffness >= 1 && m.damping >= 1 ? (d = !0, s = yl(), u = b, n.set(t = c), Promise.resolve()) : (g.soft && (h = 1 / ((g.soft === !0 ? 0.5 : +g.soft) * 60), f = 0), a || (s = yl(), d = !1, a = Jm((w) => {
             if (d)
                 return d = !1, a = null, !1;
             f = Math.min(f + h, 1);
             const k = {
                     inv_mass: f,
                     opts: m,
                     settled: !0,
@@ -8128,15 +8128,15 @@
             a.promise.then(() => {
                 S === l && w();
             });
         }));
     }
     const m = {
         set: _,
-        update: (v, b) => _(v(c, t), b),
+        update: (b, g) => _(b(c, t), g),
         subscribe: n.subscribe,
         stiffness: i,
         damping: o,
         precision: r
     };
     return m;
 }
@@ -8164,76 +8164,76 @@
 }
 
 function op(t) {
     return Array.isArray(t) ? [] : {};
 }
 
 function yi(t, e) {
-    return e.clone !== !1 && e.isMergeableObject(t) ? In(op(t), t, e) : t;
+    return e.clone !== !1 && e.isMergeableObject(t) ? Un(op(t), t, e) : t;
 }
 
 function rp(t, e, n) {
     return t.concat(e).map(function(i) {
         return yi(i, n);
     });
 }
 
 function sp(t, e) {
     if (!e.customMerge)
-        return In;
+        return Un;
     var n = e.customMerge(t);
-    return typeof n == "function" ? n : In;
+    return typeof n == "function" ? n : Un;
 }
 
 function lp(t) {
     return Object.getOwnPropertySymbols ? Object.getOwnPropertySymbols(t).filter(function(e) {
         return Object.propertyIsEnumerable.call(t, e);
     }) : [];
 }
 
 function Cl(t) {
     return Object.keys(t).concat(lp(t));
 }
 
-function ku(t, e) {
+function Cu(t, e) {
     try {
         return e in t;
     } catch {
         return !1;
     }
 }
 
 function ap(t, e) {
-    return ku(t, e) && !(Object.hasOwnProperty.call(t, e) && Object.propertyIsEnumerable.call(t, e));
+    return Cu(t, e) && !(Object.hasOwnProperty.call(t, e) && Object.propertyIsEnumerable.call(t, e));
 }
 
 function up(t, e, n) {
     var i = {};
     return n.isMergeableObject(t) && Cl(t).forEach(function(o) {
         i[o] = yi(t[o], n);
     }), Cl(e).forEach(function(o) {
-        ap(t, o) || (ku(t, o) && n.isMergeableObject(e[o]) ? i[o] = sp(o, n)(t[o], e[o], n) : i[o] = yi(e[o], n));
+        ap(t, o) || (Cu(t, o) && n.isMergeableObject(e[o]) ? i[o] = sp(o, n)(t[o], e[o], n) : i[o] = yi(e[o], n));
     }), i;
 }
 
-function In(t, e, n) {
+function Un(t, e, n) {
     n = n || {}, n.arrayMerge = n.arrayMerge || rp, n.isMergeableObject = n.isMergeableObject || Km, n.cloneUnlessOtherwiseSpecified = yi;
     var i = Array.isArray(e),
         o = Array.isArray(t),
         r = i === o;
     return r ? i ? n.arrayMerge(t, e, n) : up(t, e, n) : yi(e, n);
 }
-In.all = function(e, n) {
+Un.all = function(e, n) {
     if (!Array.isArray(e))
         throw new Error("first argument should be an array");
     return e.reduce(function(i, o) {
-        return In(i, o, n);
+        return Un(i, o, n);
     }, {});
 };
-var cp = In,
+var cp = Un,
     fp = cp;
 const dp = /* @__PURE__ */ Qm(fp);
 var zr = function(t, e) {
     return zr = Object.setPrototypeOf || {
         __proto__: []
     }
     instanceof Array && function(n, i) {
@@ -8250,88 +8250,88 @@
     zr(t, e);
 
     function n() {
         this.constructor = t;
     }
     t.prototype = e === null ? Object.create(e) : (n.prototype = e.prototype, new n());
 }
-var ne = function() {
-    return ne = Object.assign || function(e) {
+var ie = function() {
+    return ie = Object.assign || function(e) {
         for (var n, i = 1, o = arguments.length; i < o; i++) {
             n = arguments[i];
             for (var r in n)
                 Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r]);
         }
         return e;
-    }, ne.apply(this, arguments);
+    }, ie.apply(this, arguments);
 };
 
 function mr(t, e, n) {
     if (n || arguments.length === 2)
         for (var i = 0, o = e.length, r; i < o; i++)
             (r || !(i in e)) && (r || (r = Array.prototype.slice.call(e, 0, i)), r[i] = e[i]);
     return t.concat(r || Array.prototype.slice.call(e));
 }
-var Q;
+var K;
 (function(t) {
     t[t.EXPECT_ARGUMENT_CLOSING_BRACE = 1] = "EXPECT_ARGUMENT_CLOSING_BRACE", t[t.EMPTY_ARGUMENT = 2] = "EMPTY_ARGUMENT", t[t.MALFORMED_ARGUMENT = 3] = "MALFORMED_ARGUMENT", t[t.EXPECT_ARGUMENT_TYPE = 4] = "EXPECT_ARGUMENT_TYPE", t[t.INVALID_ARGUMENT_TYPE = 5] = "INVALID_ARGUMENT_TYPE", t[t.EXPECT_ARGUMENT_STYLE = 6] = "EXPECT_ARGUMENT_STYLE", t[t.INVALID_NUMBER_SKELETON = 7] = "INVALID_NUMBER_SKELETON", t[t.INVALID_DATE_TIME_SKELETON = 8] = "INVALID_DATE_TIME_SKELETON", t[t.EXPECT_NUMBER_SKELETON = 9] = "EXPECT_NUMBER_SKELETON", t[t.EXPECT_DATE_TIME_SKELETON = 10] = "EXPECT_DATE_TIME_SKELETON", t[t.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE = 11] = "UNCLOSED_QUOTE_IN_ARGUMENT_STYLE", t[t.EXPECT_SELECT_ARGUMENT_OPTIONS = 12] = "EXPECT_SELECT_ARGUMENT_OPTIONS", t[t.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE = 13] = "EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE", t[t.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE = 14] = "INVALID_PLURAL_ARGUMENT_OFFSET_VALUE", t[t.EXPECT_SELECT_ARGUMENT_SELECTOR = 15] = "EXPECT_SELECT_ARGUMENT_SELECTOR", t[t.EXPECT_PLURAL_ARGUMENT_SELECTOR = 16] = "EXPECT_PLURAL_ARGUMENT_SELECTOR", t[t.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT = 17] = "EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT", t[t.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT = 18] = "EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT", t[t.INVALID_PLURAL_ARGUMENT_SELECTOR = 19] = "INVALID_PLURAL_ARGUMENT_SELECTOR", t[t.DUPLICATE_PLURAL_ARGUMENT_SELECTOR = 20] = "DUPLICATE_PLURAL_ARGUMENT_SELECTOR", t[t.DUPLICATE_SELECT_ARGUMENT_SELECTOR = 21] = "DUPLICATE_SELECT_ARGUMENT_SELECTOR", t[t.MISSING_OTHER_CLAUSE = 22] = "MISSING_OTHER_CLAUSE", t[t.INVALID_TAG = 23] = "INVALID_TAG", t[t.INVALID_TAG_NAME = 25] = "INVALID_TAG_NAME", t[t.UNMATCHED_CLOSING_TAG = 26] = "UNMATCHED_CLOSING_TAG", t[t.UNCLOSED_TAG = 27] = "UNCLOSED_TAG";
-})(Q || (Q = {}));
+})(K || (K = {}));
 var fe;
 (function(t) {
     t[t.literal = 0] = "literal", t[t.argument = 1] = "argument", t[t.number = 2] = "number", t[t.date = 3] = "date", t[t.time = 4] = "time", t[t.select = 5] = "select", t[t.plural = 6] = "plural", t[t.pound = 7] = "pound", t[t.tag = 8] = "tag";
 })(fe || (fe = {}));
-var Un;
+var jn;
 (function(t) {
     t[t.number = 0] = "number", t[t.dateTime = 1] = "dateTime";
-})(Un || (Un = {}));
+})(jn || (jn = {}));
 
 function Sl(t) {
     return t.type === fe.literal;
 }
 
 function hp(t) {
     return t.type === fe.argument;
 }
 
-function Eu(t) {
+function Su(t) {
     return t.type === fe.number;
 }
 
-function Cu(t) {
+function Au(t) {
     return t.type === fe.date;
 }
 
-function Su(t) {
+function Tu(t) {
     return t.type === fe.time;
 }
 
-function Au(t) {
+function Pu(t) {
     return t.type === fe.select;
 }
 
-function Tu(t) {
+function Lu(t) {
     return t.type === fe.plural;
 }
 
 function _p(t) {
     return t.type === fe.pound;
 }
 
-function Pu(t) {
+function Ru(t) {
     return t.type === fe.tag;
 }
 
-function Lu(t) {
-    return !!(t && typeof t == "object" && t.type === Un.number);
+function Bu(t) {
+    return !!(t && typeof t == "object" && t.type === jn.number);
 }
 
 function Gr(t) {
-    return !!(t && typeof t == "object" && t.type === Un.dateTime);
+    return !!(t && typeof t == "object" && t.type === jn.dateTime);
 }
-var Ru = /[ \xA0\u1680\u2000-\u200A\u202F\u205F\u3000]/,
+var Mu = /[ \xA0\u1680\u2000-\u200A\u202F\u205F\u3000]/,
     mp = /(?:[Eec]{1,6}|G{1,5}|[Qq]{1,5}|(?:[yYur]+|U{1,5})|[ML]{1,5}|d{1,2}|D{1,3}|F{1}|[abB]{1,5}|[hkHK]{1,2}|w{1,2}|W{1}|m{1,2}|s{1,2}|[zZOvVxX]{1,4})(?=([^']*'[^']*')*[^']*$)/g;
 
 function pp(t) {
     var e = {};
     return t.replace(mp, function(n) {
         var i = n.length;
         switch (n[0]) {
@@ -8446,26 +8446,26 @@
     return n;
 }
 
 function vp(t) {
     return t.replace(/^(.*?)-/, "");
 }
 var Al = /^\.(?:(0+)(\*)?|(#+)|(0+)(#+))$/g,
-    Bu = /^(@+)?(\+|#+)?[rs]?$/g,
+    Du = /^(@+)?(\+|#+)?[rs]?$/g,
     wp = /(\*)(0+)|(#+)(0+)|(0+)/g,
-    Mu = /^(0+)$/;
+    Hu = /^(0+)$/;
 
 function Tl(t) {
     var e = {};
-    return t[t.length - 1] === "r" ? e.roundingPriority = "morePrecision" : t[t.length - 1] === "s" && (e.roundingPriority = "lessPrecision"), t.replace(Bu, function(n, i, o) {
+    return t[t.length - 1] === "r" ? e.roundingPriority = "morePrecision" : t[t.length - 1] === "s" && (e.roundingPriority = "lessPrecision"), t.replace(Du, function(n, i, o) {
         return typeof o != "string" ? (e.minimumSignificantDigits = i.length, e.maximumSignificantDigits = i.length) : o === "+" ? e.minimumSignificantDigits = i.length : i[0] === "#" ? e.maximumSignificantDigits = i.length : (e.minimumSignificantDigits = i.length, e.maximumSignificantDigits = i.length + (typeof o == "string" ? o.length : 0)), "";
     }), e;
 }
 
-function Du(t) {
+function Ou(t) {
     switch (t) {
         case "sign-auto":
             return {
                 signDisplay: "auto"
             };
         case "sign-accounting":
         case "()":
@@ -8506,24 +8506,24 @@
     var e;
     if (t[0] === "E" && t[1] === "E" ? (e = {
             notation: "engineering"
         }, t = t.slice(2)) : t[0] === "E" && (e = {
             notation: "scientific"
         }, t = t.slice(1)), e) {
         var n = t.slice(0, 2);
-        if (n === "+!" ? (e.signDisplay = "always", t = t.slice(2)) : n === "+?" && (e.signDisplay = "exceptZero", t = t.slice(2)), !Mu.test(t))
+        if (n === "+!" ? (e.signDisplay = "always", t = t.slice(2)) : n === "+?" && (e.signDisplay = "exceptZero", t = t.slice(2)), !Hu.test(t))
             throw new Error("Malformed concise eng/scientific notation");
         e.minimumIntegerDigits = t.length;
     }
     return e;
 }
 
 function Pl(t) {
     var e = {},
-        n = Du(t);
+        n = Ou(t);
     return n || e;
 }
 
 function kp(t) {
     for (var e = {}, n = 0, i = t; n < i.length; n++) {
         var o = i[n];
         switch (o.stem) {
@@ -8554,25 +8554,25 @@
                 e.notation = "compact", e.compactDisplay = "short";
                 continue;
             case "compact-long":
             case "KK":
                 e.notation = "compact", e.compactDisplay = "long";
                 continue;
             case "scientific":
-                e = ne(ne(ne({}, e), {
+                e = ie(ie(ie({}, e), {
                     notation: "scientific"
                 }), o.options.reduce(function(l, u) {
-                    return ne(ne({}, l), Pl(u));
+                    return ie(ie({}, l), Pl(u));
                 }, {}));
                 continue;
             case "engineering":
-                e = ne(ne(ne({}, e), {
+                e = ie(ie(ie({}, e), {
                     notation: "engineering"
                 }), o.options.reduce(function(l, u) {
-                    return ne(ne({}, l), Pl(u));
+                    return ie(ie({}, l), Pl(u));
                 }, {}));
                 continue;
             case "notation-simple":
                 e.notation = "standard";
                 continue;
             case "unit-width-narrow":
                 e.currencyDisplay = "narrowSymbol", e.unitDisplay = "narrow";
@@ -8601,38 +8601,38 @@
                         if (d)
                             throw new Error("We currently do not support exact integer digits");
                     }
                     return "";
                 });
                 continue;
         }
-        if (Mu.test(o.stem)) {
+        if (Hu.test(o.stem)) {
             e.minimumIntegerDigits = o.stem.length;
             continue;
         }
         if (Al.test(o.stem)) {
             if (o.options.length > 1)
                 throw new RangeError("Fraction-precision stems only accept a single optional option");
             o.stem.replace(Al, function(l, u, c, f, h, d) {
                 return c === "*" ? e.minimumFractionDigits = u.length : f && f[0] === "#" ? e.maximumFractionDigits = f.length : h && d ? (e.minimumFractionDigits = h.length, e.maximumFractionDigits = h.length + d.length) : (e.minimumFractionDigits = u.length, e.maximumFractionDigits = u.length), "";
             });
             var r = o.options[0];
-            r === "w" ? e = ne(ne({}, e), {
+            r === "w" ? e = ie(ie({}, e), {
                 trailingZeroDisplay: "stripIfInteger"
-            }) : r && (e = ne(ne({}, e), Tl(r)));
+            }) : r && (e = ie(ie({}, e), Tl(r)));
             continue;
         }
-        if (Bu.test(o.stem)) {
-            e = ne(ne({}, e), Tl(o.stem));
+        if (Du.test(o.stem)) {
+            e = ie(ie({}, e), Tl(o.stem));
             continue;
         }
-        var s = Du(o.stem);
-        s && (e = ne(ne({}, e), s));
+        var s = Ou(o.stem);
+        s && (e = ie(ie({}, e), s));
         var a = yp(o.stem);
-        a && (e = ne(ne({}, e), a));
+        a && (e = ie(ie({}, e), a));
     }
     return e;
 }
 var Zi = {
     AX: [
         "H"
     ],
@@ -10009,18 +10009,18 @@
         }
     var n = t.language,
         i;
     n !== "root" && (i = t.maximize().region);
     var o = Zi[i || ""] || Zi[n || ""] || Zi["".concat(n, "-001")] || Zi["001"];
     return o[0];
 }
-var pr, Sp = new RegExp("^".concat(Ru.source, "*")),
-    Ap = new RegExp("".concat(Ru.source, "*$"));
+var pr, Sp = new RegExp("^".concat(Mu.source, "*")),
+    Ap = new RegExp("".concat(Mu.source, "*$"));
 
-function $(t, e) {
+function te(t, e) {
     return {
         start: t,
         end: e
     };
 }
 var Tp = !!String.prototype.startsWith,
     Pp = !!String.fromCodePoint,
@@ -10030,15 +10030,15 @@
     Mp = !!String.prototype.trimEnd,
     Dp = !!Number.isSafeInteger,
     Hp = Dp ? Number.isSafeInteger : function(t) {
         return typeof t == "number" && isFinite(t) && Math.floor(t) === t && Math.abs(t) <= 9007199254740991;
     },
     Wr = !0;
 try {
-    var Op = Ou("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
+    var Op = Iu("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
     Wr = ((pr = Op.exec("a")) === null || pr === void 0 ? void 0 : pr[0]) === "a";
 } catch {
     Wr = !1;
 }
 var Ll = Tp ? (
         // Native
         function(e, n, i) {
@@ -10074,15 +10074,15 @@
                         a = r[1];
                     n[s] = a;
                 }
                 return n;
             }
         )
     ),
-    Hu = Rp ? (
+    Nu = Rp ? (
         // Native
         function(e, n) {
             return e.codePointAt(n);
         }
     ) : (
         // IE 11
         function(e, n) {
@@ -10113,31 +10113,31 @@
     ) : (
         // Ponyfill
         function(e) {
             return e.replace(Ap, "");
         }
     );
 
-function Ou(t, e) {
+function Iu(t, e) {
     return new RegExp(t, e);
 }
 var Xr;
 if (Wr) {
-    var Bl = Ou("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
+    var Bl = Iu("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
     Xr = function(e, n) {
         var i;
         Bl.lastIndex = n;
         var o = Bl.exec(e);
         return (i = o[1]) !== null && i !== void 0 ? i : "";
     };
 } else
     Xr = function(e, n) {
         for (var i = [];;) {
-            var o = Hu(e, n);
-            if (o === void 0 || Nu(o) || qp(o))
+            var o = Nu(e, n);
+            if (o === void 0 || Uu(o) || qp(o))
                 break;
             i.push(o), n += o >= 65536 ? 2 : 1;
         }
         return Vr.apply(void 0, i);
     };
 var Up = (
     /** @class */
@@ -10164,20 +10164,20 @@
                 } else {
                     if (r === 125 && e > 0)
                         break;
                     if (r === 35 && (n === "plural" || n === "selectordinal")) {
                         var a = this.clonePosition();
                         this.bump(), o.push({
                             type: fe.pound,
-                            location: $(a, this.clonePosition())
+                            location: te(a, this.clonePosition())
                         });
                     } else if (r === 60 && !this.ignoreTag && this.peek() === 47) {
                         if (i)
                             break;
-                        return this.error(Q.UNMATCHED_CLOSING_TAG, $(this.clonePosition(), this.clonePosition()));
+                        return this.error(K.UNMATCHED_CLOSING_TAG, te(this.clonePosition(), this.clonePosition()));
                     } else if (r === 60 && !this.ignoreTag && xr(this.peek() || 0)) {
                         var s = this.parseTag(e, n);
                         if (s.err)
                             return s;
                         o.push(s.val);
                     } else {
                         var s = this.parseLiteral(e, n);
@@ -10196,42 +10196,42 @@
             this.bump();
             var o = this.parseTagName();
             if (this.bumpSpace(), this.bumpIf("/>"))
                 return {
                     val: {
                         type: fe.literal,
                         value: "<".concat(o, "/>"),
-                        location: $(i, this.clonePosition())
+                        location: te(i, this.clonePosition())
                     },
                     err: null
                 };
             if (this.bumpIf(">")) {
                 var r = this.parseMessage(e + 1, n, !0);
                 if (r.err)
                     return r;
                 var s = r.val,
                     a = this.clonePosition();
                 if (this.bumpIf("</")) {
                     if (this.isEOF() || !xr(this.char()))
-                        return this.error(Q.INVALID_TAG, $(a, this.clonePosition()));
+                        return this.error(K.INVALID_TAG, te(a, this.clonePosition()));
                     var l = this.clonePosition(),
                         u = this.parseTagName();
-                    return o !== u ? this.error(Q.UNMATCHED_CLOSING_TAG, $(l, this.clonePosition())) : (this.bumpSpace(), this.bumpIf(">") ? {
+                    return o !== u ? this.error(K.UNMATCHED_CLOSING_TAG, te(l, this.clonePosition())) : (this.bumpSpace(), this.bumpIf(">") ? {
                         val: {
                             type: fe.tag,
                             value: o,
                             children: s,
-                            location: $(i, this.clonePosition())
+                            location: te(i, this.clonePosition())
                         },
                         err: null
-                    } : this.error(Q.INVALID_TAG, $(a, this.clonePosition())));
+                    } : this.error(K.INVALID_TAG, te(a, this.clonePosition())));
                 } else
-                    return this.error(Q.UNCLOSED_TAG, $(i, this.clonePosition()));
+                    return this.error(K.UNCLOSED_TAG, te(i, this.clonePosition()));
             } else
-                return this.error(Q.INVALID_TAG, $(i, this.clonePosition()));
+                return this.error(K.INVALID_TAG, te(i, this.clonePosition()));
         }, t.prototype.parseTagName = function() {
             var e = this.offset();
             for (this.bump(); !this.isEOF() && Fp(this.char());)
                 this.bump();
             return this.message.slice(e, this.offset());
         }, t.prototype.parseLiteral = function(e, n) {
             for (var i = this.clonePosition(), o = "";;) {
@@ -10248,15 +10248,15 @@
                 var a = this.tryParseLeftAngleBracket();
                 if (a) {
                     o += a;
                     continue;
                 }
                 break;
             }
-            var l = $(i, this.clonePosition());
+            var l = te(i, this.clonePosition());
             return {
                 val: {
                     type: fe.literal,
                     value: o,
                     location: l
                 },
                 err: null
@@ -10302,104 +10302,104 @@
             if (this.isEOF())
                 return null;
             var i = this.char();
             return i === 60 || i === 123 || i === 35 && (n === "plural" || n === "selectordinal") || i === 125 && e > 0 ? null : (this.bump(), Vr(i));
         }, t.prototype.parseArgument = function(e, n) {
             var i = this.clonePosition();
             if (this.bump(), this.bumpSpace(), this.isEOF())
-                return this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, $(i, this.clonePosition()));
+                return this.error(K.EXPECT_ARGUMENT_CLOSING_BRACE, te(i, this.clonePosition()));
             if (this.char() === 125)
-                return this.bump(), this.error(Q.EMPTY_ARGUMENT, $(i, this.clonePosition()));
+                return this.bump(), this.error(K.EMPTY_ARGUMENT, te(i, this.clonePosition()));
             var o = this.parseIdentifierIfPossible().value;
             if (!o)
-                return this.error(Q.MALFORMED_ARGUMENT, $(i, this.clonePosition()));
+                return this.error(K.MALFORMED_ARGUMENT, te(i, this.clonePosition()));
             if (this.bumpSpace(), this.isEOF())
-                return this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, $(i, this.clonePosition()));
+                return this.error(K.EXPECT_ARGUMENT_CLOSING_BRACE, te(i, this.clonePosition()));
             switch (this.char()) {
                 case 125:
                     return this.bump(), {
                         val: {
                             type: fe.argument,
                             // value does not include the opening and closing braces.
                             value: o,
-                            location: $(i, this.clonePosition())
+                            location: te(i, this.clonePosition())
                         },
                         err: null
                     };
                 case 44:
-                    return this.bump(), this.bumpSpace(), this.isEOF() ? this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, $(i, this.clonePosition())) : this.parseArgumentOptions(e, n, o, i);
+                    return this.bump(), this.bumpSpace(), this.isEOF() ? this.error(K.EXPECT_ARGUMENT_CLOSING_BRACE, te(i, this.clonePosition())) : this.parseArgumentOptions(e, n, o, i);
                 default:
-                    return this.error(Q.MALFORMED_ARGUMENT, $(i, this.clonePosition()));
+                    return this.error(K.MALFORMED_ARGUMENT, te(i, this.clonePosition()));
             }
         }, t.prototype.parseIdentifierIfPossible = function() {
             var e = this.clonePosition(),
                 n = this.offset(),
                 i = Xr(this.message, n),
                 o = n + i.length;
             this.bumpTo(o);
             var r = this.clonePosition(),
-                s = $(e, r);
+                s = te(e, r);
             return {
                 value: i,
                 location: s
             };
         }, t.prototype.parseArgumentOptions = function(e, n, i, o) {
             var r, s = this.clonePosition(),
                 a = this.parseIdentifierIfPossible().value,
                 l = this.clonePosition();
             switch (a) {
                 case "":
-                    return this.error(Q.EXPECT_ARGUMENT_TYPE, $(s, l));
+                    return this.error(K.EXPECT_ARGUMENT_TYPE, te(s, l));
                 case "number":
                 case "date":
                 case "time": {
                     this.bumpSpace();
                     var u = null;
                     if (this.bumpIf(",")) {
                         this.bumpSpace();
                         var c = this.clonePosition(),
                             f = this.parseSimpleArgStyleIfPossible();
                         if (f.err)
                             return f;
                         var h = Ip(f.val);
                         if (h.length === 0)
-                            return this.error(Q.EXPECT_ARGUMENT_STYLE, $(this.clonePosition(), this.clonePosition()));
-                        var d = $(c, this.clonePosition());
+                            return this.error(K.EXPECT_ARGUMENT_STYLE, te(this.clonePosition(), this.clonePosition()));
+                        var d = te(c, this.clonePosition());
                         u = {
                             style: h,
                             styleLocation: d
                         };
                     }
                     var _ = this.tryParseArgumentClose(o);
                     if (_.err)
                         return _;
-                    var m = $(o, this.clonePosition());
+                    var m = te(o, this.clonePosition());
                     if (u && Ll(u == null ? void 0 : u.style, "::", 0)) {
-                        var v = Np(u.style.slice(2));
+                        var b = Np(u.style.slice(2));
                         if (a === "number") {
-                            var f = this.parseNumberSkeletonFromString(v, u.styleLocation);
+                            var f = this.parseNumberSkeletonFromString(b, u.styleLocation);
                             return f.err ? f : {
                                 val: {
                                     type: fe.number,
                                     value: i,
                                     location: m,
                                     style: f.val
                                 },
                                 err: null
                             };
                         } else {
-                            if (v.length === 0)
-                                return this.error(Q.EXPECT_DATE_TIME_SKELETON, m);
-                            var b = v;
-                            this.locale && (b = Ep(v, this.locale));
+                            if (b.length === 0)
+                                return this.error(K.EXPECT_DATE_TIME_SKELETON, m);
+                            var g = b;
+                            this.locale && (g = Ep(b, this.locale));
                             var h = {
-                                    type: Un.dateTime,
-                                    pattern: b,
+                                    type: jn.dateTime,
+                                    pattern: g,
                                     location: u.styleLocation,
-                                    parsedOptions: this.shouldParseSkeletons ? pp(b) : {}
+                                    parsedOptions: this.shouldParseSkeletons ? pp(g) : {}
                                 },
                                 S = a === "date" ? fe.date : fe.time;
                             return {
                                 val: {
                                     type: S,
                                     value: i,
                                     location: m,
@@ -10420,34 +10420,34 @@
                     };
                 }
                 case "plural":
                 case "selectordinal":
                 case "select": {
                     var w = this.clonePosition();
                     if (this.bumpSpace(), !this.bumpIf(","))
-                        return this.error(Q.EXPECT_SELECT_ARGUMENT_OPTIONS, $(w, ne({}, w)));
+                        return this.error(K.EXPECT_SELECT_ARGUMENT_OPTIONS, te(w, ie({}, w)));
                     this.bumpSpace();
                     var k = this.parseIdentifierIfPossible(),
                         E = 0;
                     if (a !== "select" && k.value === "offset") {
                         if (!this.bumpIf(":"))
-                            return this.error(Q.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, $(this.clonePosition(), this.clonePosition()));
+                            return this.error(K.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, te(this.clonePosition(), this.clonePosition()));
                         this.bumpSpace();
-                        var f = this.tryParseDecimalInteger(Q.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, Q.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE);
+                        var f = this.tryParseDecimalInteger(K.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, K.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE);
                         if (f.err)
                             return f;
                         this.bumpSpace(), k = this.parseIdentifierIfPossible(), E = f.val;
                     }
                     var y = this.tryParsePluralOrSelectOptions(e, a, n, k);
                     if (y.err)
                         return y;
                     var _ = this.tryParseArgumentClose(o);
                     if (_.err)
                         return _;
-                    var H = $(o, this.clonePosition());
+                    var H = te(o, this.clonePosition());
                     return a === "select" ? {
                         val: {
                             type: fe.select,
                             value: i,
                             options: Rl(y.val),
                             location: H
                         },
@@ -10461,30 +10461,30 @@
                             pluralType: a === "plural" ? "cardinal" : "ordinal",
                             location: H
                         },
                         err: null
                     };
                 }
                 default:
-                    return this.error(Q.INVALID_ARGUMENT_TYPE, $(s, l));
+                    return this.error(K.INVALID_ARGUMENT_TYPE, te(s, l));
             }
         }, t.prototype.tryParseArgumentClose = function(e) {
-            return this.isEOF() || this.char() !== 125 ? this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, $(e, this.clonePosition())) : (this.bump(), {
+            return this.isEOF() || this.char() !== 125 ? this.error(K.EXPECT_ARGUMENT_CLOSING_BRACE, te(e, this.clonePosition())) : (this.bump(), {
                 val: !0,
                 err: null
             });
         }, t.prototype.parseSimpleArgStyleIfPossible = function() {
             for (var e = 0, n = this.clonePosition(); !this.isEOF();) {
                 var i = this.char();
                 switch (i) {
                     case 39: {
                         this.bump();
                         var o = this.clonePosition();
                         if (!this.bumpUntil("'"))
-                            return this.error(Q.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE, $(o, this.clonePosition()));
+                            return this.error(K.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE, te(o, this.clonePosition()));
                         this.bump();
                         break;
                     }
                     case 123: {
                         e += 1, this.bump();
                         break;
                     }
@@ -10508,72 +10508,72 @@
                 err: null
             };
         }, t.prototype.parseNumberSkeletonFromString = function(e, n) {
             var i = [];
             try {
                 i = bp(e);
             } catch {
-                return this.error(Q.INVALID_NUMBER_SKELETON, n);
+                return this.error(K.INVALID_NUMBER_SKELETON, n);
             }
             return {
                 val: {
-                    type: Un.number,
+                    type: jn.number,
                     tokens: i,
                     location: n,
                     parsedOptions: this.shouldParseSkeletons ? kp(i) : {}
                 },
                 err: null
             };
         }, t.prototype.tryParsePluralOrSelectOptions = function(e, n, i, o) {
             for (var r, s = !1, a = [], l = /* @__PURE__ */ new Set(), u = o.value, c = o.location;;) {
                 if (u.length === 0) {
                     var f = this.clonePosition();
                     if (n !== "select" && this.bumpIf("=")) {
-                        var h = this.tryParseDecimalInteger(Q.EXPECT_PLURAL_ARGUMENT_SELECTOR, Q.INVALID_PLURAL_ARGUMENT_SELECTOR);
+                        var h = this.tryParseDecimalInteger(K.EXPECT_PLURAL_ARGUMENT_SELECTOR, K.INVALID_PLURAL_ARGUMENT_SELECTOR);
                         if (h.err)
                             return h;
-                        c = $(f, this.clonePosition()), u = this.message.slice(f.offset, this.offset());
+                        c = te(f, this.clonePosition()), u = this.message.slice(f.offset, this.offset());
                     } else
                         break;
                 }
                 if (l.has(u))
-                    return this.error(n === "select" ? Q.DUPLICATE_SELECT_ARGUMENT_SELECTOR : Q.DUPLICATE_PLURAL_ARGUMENT_SELECTOR, c);
+                    return this.error(n === "select" ? K.DUPLICATE_SELECT_ARGUMENT_SELECTOR : K.DUPLICATE_PLURAL_ARGUMENT_SELECTOR, c);
                 u === "other" && (s = !0), this.bumpSpace();
                 var d = this.clonePosition();
                 if (!this.bumpIf("{"))
-                    return this.error(n === "select" ? Q.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT : Q.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT, $(this.clonePosition(), this.clonePosition()));
+                    return this.error(n === "select" ? K.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT : K.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT, te(this.clonePosition(), this.clonePosition()));
                 var _ = this.parseMessage(e + 1, n, i);
                 if (_.err)
                     return _;
                 var m = this.tryParseArgumentClose(d);
                 if (m.err)
                     return m;
                 a.push([
                     u, {
                         value: _.val,
-                        location: $(d, this.clonePosition())
+                        location: te(d, this.clonePosition())
                     }
                 ]), l.add(u), this.bumpSpace(), r = this.parseIdentifierIfPossible(), u = r.value, c = r.location;
             }
-            return a.length === 0 ? this.error(n === "select" ? Q.EXPECT_SELECT_ARGUMENT_SELECTOR : Q.EXPECT_PLURAL_ARGUMENT_SELECTOR, $(this.clonePosition(), this.clonePosition())) : this.requiresOtherClause && !s ? this.error(Q.MISSING_OTHER_CLAUSE, $(this.clonePosition(), this.clonePosition())) : {
+            return a.length === 0 ? this.error(n === "select" ? K.EXPECT_SELECT_ARGUMENT_SELECTOR : K.EXPECT_PLURAL_ARGUMENT_SELECTOR, te(this.clonePosition(), this.clonePosition())) : this.requiresOtherClause && !s ? this.error(K.MISSING_OTHER_CLAUSE, te(this.clonePosition(), this.clonePosition())) : {
                 val: a,
                 err: null
             };
         }, t.prototype.tryParseDecimalInteger = function(e, n) {
             var i = 1,
                 o = this.clonePosition();
             this.bumpIf("+") || this.bumpIf("-") && (i = -1);
             for (var r = !1, s = 0; !this.isEOF();) {
                 var a = this.char();
                 if (a >= 48 && a <= 57)
                     r = !0, s = s * 10 + (a - 48), this.bump();
                 else
                     break;
             }
-            var l = $(o, this.clonePosition());
+            var l = te(o, this.clonePosition());
             return r ? (s *= i, Hp(s) ? {
                 val: s,
                 err: null
             } : this.error(n, l)) : this.error(e, l);
         }, t.prototype.offset = function() {
             return this.position.offset;
         }, t.prototype.isEOF = function() {
@@ -10584,15 +10584,15 @@
                 line: this.position.line,
                 column: this.position.column
             };
         }, t.prototype.char = function() {
             var e = this.position.offset;
             if (e >= this.message.length)
                 throw Error("out of bound");
-            var n = Hu(this.message, e);
+            var n = Nu(this.message, e);
             if (n === void 0)
                 throw Error("Offset ".concat(e, " is at invalid UTF-16 code unit boundary"));
             return n;
         }, t.prototype.error = function(e, n) {
             return {
                 val: null,
                 err: {
@@ -10626,15 +10626,15 @@
                     break;
                 if (n > e)
                     throw Error("targetOffset ".concat(e, " is at invalid UTF-16 code unit boundary"));
                 if (this.bump(), this.isEOF())
                     break;
             }
         }, t.prototype.bumpSpace = function() {
-            for (; !this.isEOF() && Nu(this.char());)
+            for (; !this.isEOF() && Uu(this.char());)
                 this.bump();
         }, t.prototype.peek = function() {
             if (this.isEOF())
                 return null;
             var e = this.char(),
                 n = this.offset(),
                 i = this.message.charCodeAt(n + (e >= 65536 ? 2 : 1));
@@ -10651,40 +10651,40 @@
     return xr(t) || t === 47;
 }
 
 function Fp(t) {
     return t === 45 || t === 46 || t >= 48 && t <= 57 || t === 95 || t >= 97 && t <= 122 || t >= 65 && t <= 90 || t == 183 || t >= 192 && t <= 214 || t >= 216 && t <= 246 || t >= 248 && t <= 893 || t >= 895 && t <= 8191 || t >= 8204 && t <= 8205 || t >= 8255 && t <= 8256 || t >= 8304 && t <= 8591 || t >= 11264 && t <= 12271 || t >= 12289 && t <= 55295 || t >= 63744 && t <= 64975 || t >= 65008 && t <= 65533 || t >= 65536 && t <= 983039;
 }
 
-function Nu(t) {
+function Uu(t) {
     return t >= 9 && t <= 13 || t === 32 || t === 133 || t >= 8206 && t <= 8207 || t === 8232 || t === 8233;
 }
 
 function qp(t) {
     return t >= 33 && t <= 35 || t === 36 || t >= 37 && t <= 39 || t === 40 || t === 41 || t === 42 || t === 43 || t === 44 || t === 45 || t >= 46 && t <= 47 || t >= 58 && t <= 59 || t >= 60 && t <= 62 || t >= 63 && t <= 64 || t === 91 || t === 92 || t === 93 || t === 94 || t === 96 || t === 123 || t === 124 || t === 125 || t === 126 || t === 161 || t >= 162 && t <= 165 || t === 166 || t === 167 || t === 169 || t === 171 || t === 172 || t === 174 || t === 176 || t === 177 || t === 182 || t === 187 || t === 191 || t === 215 || t === 247 || t >= 8208 && t <= 8213 || t >= 8214 && t <= 8215 || t === 8216 || t === 8217 || t === 8218 || t >= 8219 && t <= 8220 || t === 8221 || t === 8222 || t === 8223 || t >= 8224 && t <= 8231 || t >= 8240 && t <= 8248 || t === 8249 || t === 8250 || t >= 8251 && t <= 8254 || t >= 8257 && t <= 8259 || t === 8260 || t === 8261 || t === 8262 || t >= 8263 && t <= 8273 || t === 8274 || t === 8275 || t >= 8277 && t <= 8286 || t >= 8592 && t <= 8596 || t >= 8597 && t <= 8601 || t >= 8602 && t <= 8603 || t >= 8604 && t <= 8607 || t === 8608 || t >= 8609 && t <= 8610 || t === 8611 || t >= 8612 && t <= 8613 || t === 8614 || t >= 8615 && t <= 8621 || t === 8622 || t >= 8623 && t <= 8653 || t >= 8654 && t <= 8655 || t >= 8656 && t <= 8657 || t === 8658 || t === 8659 || t === 8660 || t >= 8661 && t <= 8691 || t >= 8692 && t <= 8959 || t >= 8960 && t <= 8967 || t === 8968 || t === 8969 || t === 8970 || t === 8971 || t >= 8972 && t <= 8991 || t >= 8992 && t <= 8993 || t >= 8994 && t <= 9e3 || t === 9001 || t === 9002 || t >= 9003 && t <= 9083 || t === 9084 || t >= 9085 && t <= 9114 || t >= 9115 && t <= 9139 || t >= 9140 && t <= 9179 || t >= 9180 && t <= 9185 || t >= 9186 && t <= 9254 || t >= 9255 && t <= 9279 || t >= 9280 && t <= 9290 || t >= 9291 && t <= 9311 || t >= 9472 && t <= 9654 || t === 9655 || t >= 9656 && t <= 9664 || t === 9665 || t >= 9666 && t <= 9719 || t >= 9720 && t <= 9727 || t >= 9728 && t <= 9838 || t === 9839 || t >= 9840 && t <= 10087 || t === 10088 || t === 10089 || t === 10090 || t === 10091 || t === 10092 || t === 10093 || t === 10094 || t === 10095 || t === 10096 || t === 10097 || t === 10098 || t === 10099 || t === 10100 || t === 10101 || t >= 10132 && t <= 10175 || t >= 10176 && t <= 10180 || t === 10181 || t === 10182 || t >= 10183 && t <= 10213 || t === 10214 || t === 10215 || t === 10216 || t === 10217 || t === 10218 || t === 10219 || t === 10220 || t === 10221 || t === 10222 || t === 10223 || t >= 10224 && t <= 10239 || t >= 10240 && t <= 10495 || t >= 10496 && t <= 10626 || t === 10627 || t === 10628 || t === 10629 || t === 10630 || t === 10631 || t === 10632 || t === 10633 || t === 10634 || t === 10635 || t === 10636 || t === 10637 || t === 10638 || t === 10639 || t === 10640 || t === 10641 || t === 10642 || t === 10643 || t === 10644 || t === 10645 || t === 10646 || t === 10647 || t === 10648 || t >= 10649 && t <= 10711 || t === 10712 || t === 10713 || t === 10714 || t === 10715 || t >= 10716 && t <= 10747 || t === 10748 || t === 10749 || t >= 10750 && t <= 11007 || t >= 11008 && t <= 11055 || t >= 11056 && t <= 11076 || t >= 11077 && t <= 11078 || t >= 11079 && t <= 11084 || t >= 11085 && t <= 11123 || t >= 11124 && t <= 11125 || t >= 11126 && t <= 11157 || t === 11158 || t >= 11159 && t <= 11263 || t >= 11776 && t <= 11777 || t === 11778 || t === 11779 || t === 11780 || t === 11781 || t >= 11782 && t <= 11784 || t === 11785 || t === 11786 || t === 11787 || t === 11788 || t === 11789 || t >= 11790 && t <= 11798 || t === 11799 || t >= 11800 && t <= 11801 || t === 11802 || t === 11803 || t === 11804 || t === 11805 || t >= 11806 && t <= 11807 || t === 11808 || t === 11809 || t === 11810 || t === 11811 || t === 11812 || t === 11813 || t === 11814 || t === 11815 || t === 11816 || t === 11817 || t >= 11818 && t <= 11822 || t === 11823 || t >= 11824 && t <= 11833 || t >= 11834 && t <= 11835 || t >= 11836 && t <= 11839 || t === 11840 || t === 11841 || t === 11842 || t >= 11843 && t <= 11855 || t >= 11856 && t <= 11857 || t === 11858 || t >= 11859 && t <= 11903 || t >= 12289 && t <= 12291 || t === 12296 || t === 12297 || t === 12298 || t === 12299 || t === 12300 || t === 12301 || t === 12302 || t === 12303 || t === 12304 || t === 12305 || t >= 12306 && t <= 12307 || t === 12308 || t === 12309 || t === 12310 || t === 12311 || t === 12312 || t === 12313 || t === 12314 || t === 12315 || t === 12316 || t === 12317 || t >= 12318 && t <= 12319 || t === 12320 || t === 12336 || t === 64830 || t === 64831 || t >= 65093 && t <= 65094;
 }
 
 function Zr(t) {
     t.forEach(function(e) {
-        if (delete e.location, Au(e) || Tu(e))
+        if (delete e.location, Pu(e) || Lu(e))
             for (var n in e.options)
                 delete e.options[n].location, Zr(e.options[n].value);
         else
-            Eu(e) && Lu(e.style) || (Cu(e) || Su(e)) && Gr(e.style) ? delete e.style.location : Pu(e) && Zr(e.children);
+            Su(e) && Bu(e.style) || (Au(e) || Tu(e)) && Gr(e.style) ? delete e.style.location : Ru(e) && Zr(e.children);
     });
 }
 
 function zp(t, e) {
-    e === void 0 && (e = {}), e = ne({
+    e === void 0 && (e = {}), e = ie({
         shouldParseSkeletons: !0,
         requiresOtherClause: !0
     }, e);
     var n = new Up(t, e).parse();
     if (n.err) {
-        var i = SyntaxError(Q[n.err.kind]);
+        var i = SyntaxError(K[n.err.kind]);
         throw i.location = n.err.location, i.originalMessage = n.err.message, i;
     }
     return e != null && e.captureLocation || Zr(n.val), n.val;
 }
 
 function gr(t, e) {
     var n = e && e.cache ? e.cache : Zp,
@@ -10696,42 +10696,42 @@
     });
 }
 
 function Gp(t) {
     return t == null || typeof t == "number" || typeof t == "boolean";
 }
 
-function Iu(t, e, n, i) {
+function ju(t, e, n, i) {
     var o = Gp(i) ? i : n(i),
         r = e.get(o);
     return typeof r > "u" && (r = t.call(this, i), e.set(o, r)), r;
 }
 
-function Uu(t, e, n) {
+function Fu(t, e, n) {
     var i = Array.prototype.slice.call(arguments, 3),
         o = n(i),
         r = e.get(o);
     return typeof r > "u" && (r = t.apply(this, i), e.set(o, r)), r;
 }
 
 function us(t, e, n, i, o) {
     return n.bind(e, t, i, o);
 }
 
 function Wp(t, e) {
-    var n = t.length === 1 ? Iu : Uu;
+    var n = t.length === 1 ? ju : Fu;
     return us(t, this, n, e.cache.create(), e.serializer);
 }
 
 function Vp(t, e) {
-    return us(t, this, Uu, e.cache.create(), e.serializer);
+    return us(t, this, Fu, e.cache.create(), e.serializer);
 }
 
 function Xp(t, e) {
-    return us(t, this, Iu, e.cache.create(), e.serializer);
+    return us(t, this, ju, e.cache.create(), e.serializer);
 }
 var xp = function() {
     return JSON.stringify(arguments);
 };
 
 function cs() {
     this.cache = /* @__PURE__ */ Object.create(null);
@@ -10747,18 +10747,18 @@
             return new cs();
         }
     },
     br = {
         variadic: Vp,
         monadic: Xp
     },
-    jn;
+    Fn;
 (function(t) {
     t.MISSING_VALUE = "MISSING_VALUE", t.INVALID_VALUE = "INVALID_VALUE", t.MISSING_INTL_API = "MISSING_INTL_API";
-})(jn || (jn = {}));
+})(Fn || (Fn = {}));
 var Co = (
         /** @class */
         function(t) {
             Eo(e, t);
 
             function e(n, i, o) {
                 var r = t.call(this, n) || this;
@@ -10771,37 +10771,37 @@
     ),
     Ml = (
         /** @class */
         function(t) {
             Eo(e, t);
 
             function e(n, i, o, r) {
-                return t.call(this, 'Invalid values for "'.concat(n, '": "').concat(i, '". Options are "').concat(Object.keys(o).join('", "'), '"'), jn.INVALID_VALUE, r) || this;
+                return t.call(this, 'Invalid values for "'.concat(n, '": "').concat(i, '". Options are "').concat(Object.keys(o).join('", "'), '"'), Fn.INVALID_VALUE, r) || this;
             }
             return e;
         }(Co)
     ),
     Jp = (
         /** @class */
         function(t) {
             Eo(e, t);
 
             function e(n, i, o) {
-                return t.call(this, 'Value for "'.concat(n, '" must be of type ').concat(i), jn.INVALID_VALUE, o) || this;
+                return t.call(this, 'Value for "'.concat(n, '" must be of type ').concat(i), Fn.INVALID_VALUE, o) || this;
             }
             return e;
         }(Co)
     ),
     Yp = (
         /** @class */
         function(t) {
             Eo(e, t);
 
             function e(n, i) {
-                return t.call(this, 'The intl string context variable "'.concat(n, '" was not provided to the string "').concat(i, '"'), jn.MISSING_VALUE, i) || this;
+                return t.call(this, 'The intl string context variable "'.concat(n, '" was not provided to the string "').concat(i, '"'), Fn.MISSING_VALUE, i) || this;
             }
             return e;
         }(Co)
     ),
     De;
 (function(t) {
     t[t.literal = 0] = "literal", t[t.object = 1] = "object";
@@ -10847,69 +10847,69 @@
         if (hp(c)) {
             (!h || typeof h == "string" || typeof h == "number") && (h = typeof h == "string" || typeof h == "number" ? String(h) : ""), a.push({
                 type: typeof h == "string" ? De.literal : De.object,
                 value: h
             });
             continue;
         }
-        if (Cu(c)) {
+        if (Au(c)) {
             var d = typeof c.style == "string" ? i.date[c.style] : Gr(c.style) ? c.style.parsedOptions : void 0;
             a.push({
                 type: De.literal,
                 value: n.getDateTimeFormat(e, d).format(h)
             });
             continue;
         }
-        if (Su(c)) {
+        if (Tu(c)) {
             var d = typeof c.style == "string" ? i.time[c.style] : Gr(c.style) ? c.style.parsedOptions : i.time.medium;
             a.push({
                 type: De.literal,
                 value: n.getDateTimeFormat(e, d).format(h)
             });
             continue;
         }
-        if (Eu(c)) {
-            var d = typeof c.style == "string" ? i.number[c.style] : Lu(c.style) ? c.style.parsedOptions : void 0;
+        if (Su(c)) {
+            var d = typeof c.style == "string" ? i.number[c.style] : Bu(c.style) ? c.style.parsedOptions : void 0;
             d && d.scale && (h = h * (d.scale || 1)), a.push({
                 type: De.literal,
                 value: n.getNumberFormat(e, d).format(h)
             });
             continue;
         }
-        if (Pu(c)) {
+        if (Ru(c)) {
             var _ = c.children,
                 m = c.value,
-                v = o[m];
-            if (!Kp(v))
+                b = o[m];
+            if (!Kp(b))
                 throw new Jp(m, "function", s);
-            var b = eo(_, e, n, i, o, r),
-                S = v(b.map(function(E) {
+            var g = eo(_, e, n, i, o, r),
+                S = b(g.map(function(E) {
                     return E.value;
                 }));
             Array.isArray(S) || (S = [S]), a.push.apply(a, S.map(function(E) {
                 return {
                     type: typeof E == "string" ? De.literal : De.object,
                     value: E
                 };
             }));
         }
-        if (Au(c)) {
+        if (Pu(c)) {
             var w = c.options[h] || c.options.other;
             if (!w)
                 throw new Ml(c.value, h, Object.keys(c.options), s);
             a.push.apply(a, eo(w.value, e, n, i, o));
             continue;
         }
-        if (Tu(c)) {
+        if (Lu(c)) {
             var w = c.options["=".concat(h)];
             if (!w) {
                 if (!Intl.PluralRules)
                     throw new Co(`Intl.PluralRules is not available in this environment.
 Try polyfilling it using "@formatjs/intl-pluralrules"
-`, jn.MISSING_INTL_API, s);
+`, Fn.MISSING_INTL_API, s);
                 var k = n.getPluralRules(e, {
                     type: c.pluralType
                 }).select(h - (c.offset || 0));
                 w = c.options[k] || c.options.other;
             }
             if (!w)
                 throw new Ml(c.value, h, Object.keys(c.options), s);
@@ -10917,23 +10917,23 @@
             continue;
         }
     }
     return Qp(a);
 }
 
 function $p(t, e) {
-    return e ? ne(ne(ne({}, t || {}), e || {}), Object.keys(t).reduce(function(n, i) {
-        return n[i] = ne(ne({}, t[i]), e[i] || {}), n;
+    return e ? ie(ie(ie({}, t || {}), e || {}), Object.keys(t).reduce(function(n, i) {
+        return n[i] = ie(ie({}, t[i]), e[i] || {}), n;
     }, {})) : t;
 }
 
 function e1(t, e) {
     return e ? Object.keys(t).reduce(function(n, i) {
         return n[i] = $p(t[i], e[i]), n;
-    }, ne({}, t)) : t;
+    }, ie({}, t)) : t;
 }
 
 function vr(t) {
     return {
         create: function() {
             return {
                 get: function(e) {
@@ -11107,15 +11107,15 @@
             i = i[n[o]];
         } else
             i = void 0;
     return i;
 }
 const Nt = {},
     o1 = (t, e, n) => n && (e in Nt || (Nt[e] = {}), t in Nt[e] || (Nt[e][t] = n), n),
-    ju = (t, e) => {
+    qu = (t, e) => {
         if (e == null)
             return;
         if (e in Nt && t in Nt[e])
             return Nt[e][t];
         const n = So(e);
         for (let i = 0; i < n.length; i++) {
             const o = n[i],
@@ -11127,90 +11127,90 @@
 let fs;
 const Ti = Ai({});
 
 function r1(t) {
     return fs[t] || null;
 }
 
-function Fu(t) {
+function zu(t) {
     return t in fs;
 }
 
 function s1(t, e) {
-    if (!Fu(t))
+    if (!zu(t))
         return null;
     const n = r1(t);
     return i1(n, e);
 }
 
 function l1(t) {
     if (t == null)
         return;
     const e = So(t);
     for (let n = 0; n < e.length; n++) {
         const i = e[n];
-        if (Fu(i))
+        if (zu(i))
             return i;
     }
 }
 
 function a1(t, ...e) {
     delete Nt[t], Ti.update((n) => (n[t] = dp.all([n[t] || {}, ...e]), n));
 }
-Qn(
+Kn(
     [Ti],
     ([t]) => Object.keys(t)
 );
 Ti.subscribe((t) => fs = t);
 const to = {};
 
 function u1(t, e) {
     to[t].delete(e), to[t].size === 0 && delete to[t];
 }
 
-function qu(t) {
+function Gu(t) {
     return to[t];
 }
 
 function c1(t) {
     return So(t).map((e) => {
-        const n = qu(e);
+        const n = Gu(e);
         return [e, n ? [...n] : []];
     }).filter(([, e]) => e.length > 0);
 }
 
 function Jr(t) {
     return t == null ? !1 : So(t).some(
         (e) => {
             var n;
-            return (n = qu(e)) == null ? void 0 : n.size;
+            return (n = Gu(e)) == null ? void 0 : n.size;
         }
     );
 }
 
 function f1(t, e) {
     return Promise.all(
         e.map((i) => (u1(t, i), i().then((o) => o.default || o)))
     ).then((i) => a1(t, ...i));
 }
-const ai = {};
+const ui = {};
 
-function zu(t) {
+function Wu(t) {
     if (!Jr(t))
-        return t in ai ? ai[t] : Promise.resolve();
+        return t in ui ? ui[t] : Promise.resolve();
     const e = c1(t);
-    return ai[t] = Promise.all(
+    return ui[t] = Promise.all(
         e.map(
             ([n, i]) => f1(n, i)
         )
     ).then(() => {
         if (Jr(t))
-            return zu(t);
-        delete ai[t];
-    }), ai[t];
+            return Wu(t);
+        delete ui[t];
+    }), ui[t];
 }
 const d1 = {
         number: {
             scientific: {
                 notation: "scientific"
             },
             engineering: {
@@ -11278,15 +11278,15 @@
         formats: d1,
         warnOnMissingMessages: !0,
         handleMissingMessage: void 0,
         ignoreTag: !0
     },
     _1 = h1;
 
-function Fn() {
+function qn() {
     return _1;
 }
 const wr = Ai(!1);
 var m1 = Object.defineProperty,
     p1 = Object.defineProperties,
     g1 = Object.getOwnPropertyDescriptors,
     Dl = Object.getOwnPropertySymbols,
@@ -11310,35 +11310,35 @@
 let Yr;
 const ao = Ai(null);
 
 function Ol(t) {
     return t.split("-").map((e, n, i) => i.slice(0, n + 1).join("-")).reverse();
 }
 
-function So(t, e = Fn().fallbackLocale) {
+function So(t, e = qn().fallbackLocale) {
     const n = Ol(t);
     return e ? [... /* @__PURE__ */ new Set([...n, ...Ol(e)])] : n;
 }
 
 function vn() {
     return Yr ?? void 0;
 }
 ao.subscribe((t) => {
     Yr = t ?? void 0, typeof window < "u" && t != null && document.documentElement.setAttribute("lang", t);
 });
 const k1 = (t) => {
         if (t && l1(t) && Jr(t)) {
             const {
                 loadingDelay: e
-            } = Fn();
+            } = qn();
             let n;
             return typeof window < "u" && vn() != null && e ? n = window.setTimeout(
                 () => wr.set(!0),
                 e
-            ) : wr.set(!0), zu(t).then(() => {
+            ) : wr.set(!0), Wu(t).then(() => {
                 ao.set(t);
             }).finally(() => {
                 clearTimeout(n), wr.set(!1);
             });
         }
         return ao.set(t);
     },
@@ -11350,128 +11350,128 @@
         return (i) => {
             const o = JSON.stringify(i);
             return o in e ? e[o] : e[o] = t(i);
         };
     };
 var E1 = Object.defineProperty,
     uo = Object.getOwnPropertySymbols,
-    Gu = Object.prototype.hasOwnProperty,
-    Wu = Object.prototype.propertyIsEnumerable,
+    Vu = Object.prototype.hasOwnProperty,
+    Xu = Object.prototype.propertyIsEnumerable,
     Nl = (t, e, n) => e in t ? E1(t, e, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
         value: n
     }) : t[e] = n,
     ds = (t, e) => {
         for (var n in e || (e = {}))
-            Gu.call(e, n) && Nl(t, n, e[n]);
+            Vu.call(e, n) && Nl(t, n, e[n]);
         if (uo)
             for (var n of uo(e))
-                Wu.call(e, n) && Nl(t, n, e[n]);
+                Xu.call(e, n) && Nl(t, n, e[n]);
         return t;
     },
-    Kn = (t, e) => {
+    $n = (t, e) => {
         var n = {};
         for (var i in t)
-            Gu.call(t, i) && e.indexOf(i) < 0 && (n[i] = t[i]);
+            Vu.call(t, i) && e.indexOf(i) < 0 && (n[i] = t[i]);
         if (t != null && uo)
             for (var i of uo(t))
-                e.indexOf(i) < 0 && Wu.call(t, i) && (n[i] = t[i]);
+                e.indexOf(i) < 0 && Xu.call(t, i) && (n[i] = t[i]);
         return n;
     };
 const ki = (t, e) => {
         const {
             formats: n
-        } = Fn();
+        } = qn();
         if (t in n && e in n[t])
             return n[t][e];
         throw new Error(`[svelte-i18n] Unknown "${e}" ${t} format.`);
     },
     C1 = Ao(
         (t) => {
             var e = t,
                 {
                     locale: n,
                     format: i
                 } = e,
-                o = Kn(e, ["locale", "format"]);
+                o = $n(e, ["locale", "format"]);
             if (n == null)
                 throw new Error('[svelte-i18n] A "locale" must be set to format numbers');
             return i && (o = ki("number", i)), new Intl.NumberFormat(n, o);
         }
     ),
     S1 = Ao(
         (t) => {
             var e = t,
                 {
                     locale: n,
                     format: i
                 } = e,
-                o = Kn(e, ["locale", "format"]);
+                o = $n(e, ["locale", "format"]);
             if (n == null)
                 throw new Error('[svelte-i18n] A "locale" must be set to format dates');
             return i ? o = ki("date", i) : Object.keys(o).length === 0 && (o = ki("date", "short")), new Intl.DateTimeFormat(n, o);
         }
     ),
     A1 = Ao(
         (t) => {
             var e = t,
                 {
                     locale: n,
                     format: i
                 } = e,
-                o = Kn(e, ["locale", "format"]);
+                o = $n(e, ["locale", "format"]);
             if (n == null)
                 throw new Error(
                     '[svelte-i18n] A "locale" must be set to format time values'
                 );
             return i ? o = ki("time", i) : Object.keys(o).length === 0 && (o = ki("time", "short")), new Intl.DateTimeFormat(n, o);
         }
     ),
     T1 = (t = {}) => {
         var e = t,
             {
                 locale: n = vn()
             } = e,
-            i = Kn(e, [
+            i = $n(e, [
                 "locale"
             ]);
         return C1(ds({
             locale: n
         }, i));
     },
     P1 = (t = {}) => {
         var e = t,
             {
                 locale: n = vn()
             } = e,
-            i = Kn(e, [
+            i = $n(e, [
                 "locale"
             ]);
         return S1(ds({
             locale: n
         }, i));
     },
     L1 = (t = {}) => {
         var e = t,
             {
                 locale: n = vn()
             } = e,
-            i = Kn(e, [
+            i = $n(e, [
                 "locale"
             ]);
         return A1(ds({
             locale: n
         }, i));
     },
     R1 = Ao(
         // eslint-disable-next-line @typescript-eslint/no-non-null-assertion
-        (t, e = vn()) => new n1(t, e, Fn().formats, {
-            ignoreTag: Fn().ignoreTag
+        (t, e = vn()) => new n1(t, e, qn().formats, {
+            ignoreTag: qn().ignoreTag
         })
     ),
     B1 = (t, e = {}) => {
         var n, i, o, r;
         let s = e;
         typeof t == "object" && (s = t, t = s.id);
         const {
@@ -11479,17 +11479,17 @@
             locale: l = vn(),
             default: u
         } = s;
         if (l == null)
             throw new Error(
                 "[svelte-i18n] Cannot format a message without first setting the initial locale."
             );
-        let c = ju(t, l);
+        let c = qu(t, l);
         if (!c)
-            c = (r = (o = (i = (n = Fn()).handleMissingMessage) == null ? void 0 : i.call(n, {
+            c = (r = (o = (i = (n = qn()).handleMissingMessage) == null ? void 0 : i.call(n, {
                 locale: l,
                 id: t,
                 defaultValue: u
             })) != null ? o : u) != null ? r : t;
         else if (typeof c != "string")
             return console.warn(
                 `[svelte-i18n] Message with id "${t}" must be of type "string", found: "${typeof c}". Gettin its value through the "$format" method is deprecated; use the "json" method instead.`
@@ -11506,34 +11506,34 @@
             );
         }
         return f;
     },
     M1 = (t, e) => L1(e).format(t),
     D1 = (t, e) => P1(e).format(t),
     H1 = (t, e) => T1(e).format(t),
-    O1 = (t, e = vn()) => ju(t, e);
-Qn([Pi, Ti], () => B1);
-Qn([Pi], () => M1);
-Qn([Pi], () => D1);
-Qn([Pi], () => H1);
-Qn([Pi, Ti], () => O1);
+    O1 = (t, e = vn()) => qu(t, e);
+Kn([Pi, Ti], () => B1);
+Kn([Pi], () => M1);
+Kn([Pi], () => D1);
+Kn([Pi], () => H1);
+Kn([Pi, Ti], () => O1);
 const {
     SvelteComponent: N1,
     append: Fe,
     attr: Yt,
-    detach: Vu,
+    detach: xu,
     element: Qt,
     init: I1,
-    insert: Xu,
+    insert: Zu,
     noop: Il,
     safe_not_equal: U1,
     set_data: co,
     set_style: yr,
     space: Qr,
-    text: Rn,
+    text: Bn,
     toggle_class: Ul
 } = window.__gradio__svelte__internal, {
     onMount: j1,
     createEventDispatcher: F1,
     getContext: q1
 } = window.__gradio__svelte__internal;
 
@@ -11545,21 +11545,21 @@
         s, a, l, u, c = (
             /*file_to_display*/
             t[2].orig_name + ""
         ),
         f;
     return {
         c() {
-            e = Qt("div"), n = Qt("span"), i = Qt("div"), o = Qt("progress"), s = Rn(r), l = Qr(), u = Qt("span"), f = Rn(c), yr(o, "visibility", "hidden"), yr(o, "height", "0"), yr(o, "width", "0"), o.value = a = pi(
+            e = Qt("div"), n = Qt("span"), i = Qt("div"), o = Qt("progress"), s = Bn(r), l = Qr(), u = Qt("span"), f = Bn(c), yr(o, "visibility", "hidden"), yr(o, "height", "0"), yr(o, "width", "0"), o.value = a = pi(
                 /*file_to_display*/
                 t[2]
             ), Yt(o, "max", "100"), Yt(o, "class", "svelte-cr2edf"), Yt(i, "class", "progress-bar svelte-cr2edf"), Yt(u, "class", "file-name svelte-cr2edf"), Yt(e, "class", "file svelte-cr2edf");
         },
         m(h, d) {
-            Xu(h, e, d), Fe(e, n), Fe(n, i), Fe(i, o), Fe(o, s), Fe(e, l), Fe(e, u), Fe(u, f);
+            Zu(h, e, d), Fe(e, n), Fe(n, i), Fe(i, o), Fe(o, s), Fe(e, l), Fe(e, u), Fe(u, f);
         },
         p(h, d) {
             d & /*file_to_display*/
                 4 && r !== (r = pi(
                     /*file_to_display*/
                     h[2]
                 ) + "") && co(s, r), d & /*file_to_display*/
@@ -11567,15 +11567,15 @@
                     /*file_to_display*/
                     h[2]
                 )) && (o.value = a), d & /*file_to_display*/
                 4 && c !== (c = /*file_to_display*/
                     h[2].orig_name + "") && co(f, c);
         },
         d(h) {
-            h && Vu(e);
+            h && xu(e);
         }
     };
 }
 
 function z1(t) {
     let e, n, i, o = (
             /*files_with_progress*/
@@ -11587,23 +11587,23 @@
         ),
         l, u, c, f = (
             /*file_to_display*/
             t[2] && jl(t)
         );
     return {
         c() {
-            e = Qt("div"), n = Qt("span"), i = Rn("Uploading "), r = Rn(o), s = Qr(), l = Rn(a), u = Rn("..."), c = Qr(), f && f.c(), Yt(n, "class", "uploading svelte-cr2edf"), Yt(e, "class", "wrap svelte-cr2edf"), Ul(
+            e = Qt("div"), n = Qt("span"), i = Bn("Uploading "), r = Bn(o), s = Qr(), l = Bn(a), u = Bn("..."), c = Qr(), f && f.c(), Yt(n, "class", "uploading svelte-cr2edf"), Yt(e, "class", "wrap svelte-cr2edf"), Ul(
                 e,
                 "progress",
                 /*progress*/
                 t[1]
             );
         },
         m(h, d) {
-            Xu(h, e, d), Fe(e, n), Fe(n, i), Fe(n, r), Fe(n, s), Fe(n, l), Fe(n, u), Fe(e, c), f && f.m(e, null);
+            Zu(h, e, d), Fe(e, n), Fe(n, i), Fe(n, r), Fe(n, s), Fe(n, l), Fe(n, u), Fe(e, c), f && f.m(e, null);
         },
         p(h, [d]) {
             d & /*files_with_progress*/
                 1 && o !== (o = /*files_with_progress*/
                     h[0].length + "") && co(r, o), d & /*files_with_progress*/
                 1 && a !== (a = /*files_with_progress*/
                     h[0].length > 1 ? "files" : "file") && co(l, a), /*file_to_display*/
@@ -11614,15 +11614,15 @@
                     /*progress*/
                     h[1]
                 );
         },
         i: Il,
         o: Il,
         d(h) {
-            h && Vu(e), f && f.d();
+            h && xu(e), f && f.d();
         }
     };
 }
 
 function pi(t) {
     return t.progress * 100 / (t.size || 0) || 0;
 }
@@ -11644,15 +11644,15 @@
     } = e, s, a = !1, l, u, c = r.map((_) => ({
         ..._,
         progress: 0
     }));
     const f = F1();
 
     function h(_, m) {
-        n(0, c = c.map((v) => (v.orig_name === _ && (v.progress += m), v)));
+        n(0, c = c.map((b) => (b.orig_name === _ && (b.progress += m), b)));
     }
     const d = q1("EventSource_factory");
     return j1(() => {
         s = d(new URL(`${o}/upload_progress?upload_id=${i}`)), s.onmessage = async function(_) {
             const m = JSON.parse(_.data);
             a || n(1, a = !0), m.msg === "done" ? (s.close(), f("done")) : (n(6, l = m), h(m.orig_name, m.chunk_size));
         };
@@ -11683,51 +11683,51 @@
 }
 const {
     SvelteComponent: X1,
     append: Fl,
     attr: Be,
     binding_callbacks: x1,
     bubble: xt,
-    check_outros: xu,
+    check_outros: Ju,
     create_component: Z1,
-    create_slot: Zu,
+    create_slot: Yu,
     destroy_component: J1,
     detach: To,
     element: Kr,
-    empty: Ju,
-    get_all_dirty_from_scope: Yu,
-    get_slot_changes: Qu,
-    group_outros: Ku,
+    empty: Qu,
+    get_all_dirty_from_scope: Ku,
+    get_slot_changes: $u,
+    group_outros: ec,
     init: Y1,
     insert: Po,
     listen: ze,
     mount_component: Q1,
     prevent_default: Zt,
     run_all: K1,
     safe_not_equal: $1,
-    set_style: $u,
+    set_style: tc,
     space: eg,
     stop_propagation: Jt,
     toggle_class: Te,
     transition_in: Ut,
     transition_out: mn,
-    update_slot_base: ec
+    update_slot_base: nc
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: tg,
     tick: ng,
     getContext: ig
 } = window.__gradio__svelte__internal;
 
 function og(t) {
     let e, n, i, o, r, s, a, l, u, c, f;
     const h = (
             /*#slots*/
             t[22].default
         ),
-        d = Zu(
+        d = Yu(
             h,
             t,
             /*$$scope*/
             t[21],
             null
         );
     return {
@@ -11758,15 +11758,15 @@
                     /*flex*/
                     t[5]
                 ), Te(
                     e,
                     "disable_click",
                     /*disable_click*/
                     t[7]
-                ), $u(e, "height", "100%");
+                ), tc(e, "height", "100%");
         },
         m(_, m) {
             Po(_, e, m), d && d.m(e, null), Fl(e, n), Fl(e, i), t[30](i), u = !0, c || (f = [
                 ze(
                     i,
                     "change",
                     /*load_files_from_upload*/
@@ -11824,27 +11824,27 @@
                     /*updateDragging*/
                     t[15]
                 )
             ], c = !0);
         },
         p(_, m) {
             d && d.p && (!u || m[0] & /*$$scope*/
-                2097152) && ec(
+                2097152) && nc(
                 d,
                 h,
                 _,
                 /*$$scope*/
                 _[21],
-                u ? Qu(
+                u ? $u(
                     h,
                     /*$$scope*/
                     _[21],
                     m,
                     null
-                ) : Yu(
+                ) : Ku(
                     /*$$scope*/
                     _[21]
                 ),
                 null
             ), (!u || m[0] & /*accept_file_types*/
                 16384 && o !== (o = /*accept_file_types*/
                     _[14] || void 0)) && Be(i, "accept", o), (!u || m[0] & /*file_count*/
@@ -11900,24 +11900,24 @@
 }
 
 function rg(t) {
     let e, n, i = ! /*hidden*/
         t[9] && ql(t);
     return {
         c() {
-            i && i.c(), e = Ju();
+            i && i.c(), e = Qu();
         },
         m(o, r) {
             i && i.m(o, r), Po(o, e, r), n = !0;
         },
         p(o, r) {
             /*hidden*/
-            o[9] ? i && (Ku(), mn(i, 1, 1, () => {
+            o[9] ? i && (ec(), mn(i, 1, 1, () => {
                 i = null;
-            }), xu()) : i ? (i.p(o, r), r[0] & /*hidden*/
+            }), Ju()) : i ? (i.p(o, r), r[0] & /*hidden*/
                 512 && Ut(i, 1)) : (i = ql(o), i.c(), Ut(i, 1), i.m(e.parentNode, e));
         },
         i(o) {
             n || (Ut(i), n = !0);
         },
         o(o) {
             mn(i), n = !1;
@@ -11930,15 +11930,15 @@
 
 function sg(t) {
     let e, n, i, o, r;
     const s = (
             /*#slots*/
             t[22].default
         ),
-        a = Zu(
+        a = Yu(
             s,
             t,
             /*$$scope*/
             t[21],
             null
         );
     return {
@@ -11960,39 +11960,39 @@
                 /*boundedheight*/
                 t[3]
             ), Te(
                 e,
                 "flex",
                 /*flex*/
                 t[5]
-            ), $u(e, "height", "100%");
+            ), tc(e, "height", "100%");
         },
         m(l, u) {
             Po(l, e, u), a && a.m(e, null), i = !0, o || (r = ze(
                 e,
                 "click",
                 /*paste_clipboard*/
                 t[10]
             ), o = !0);
         },
         p(l, u) {
             a && a.p && (!i || u[0] & /*$$scope*/
-                2097152) && ec(
+                2097152) && nc(
                 a,
                 s,
                 l,
                 /*$$scope*/
                 l[21],
-                i ? Qu(
+                i ? $u(
                     s,
                     /*$$scope*/
                     l[21],
                     u,
                     null
-                ) : Yu(
+                ) : Ku(
                     /*$$scope*/
                     l[21]
                 ),
                 null
             ), (!i || u[0] & /*hidden*/
                 512 && n !== (n = /*hidden*/
                     l[9] ? -1 : 0)) && Be(e, "tabindex", n), (!i || u[0] & /*hidden*/
@@ -12092,24 +12092,24 @@
                 l[1] && ! /*hidden_upload*/
                 l[2] ? 1 : 2
             )
         );
     }
     return e = a(t), n = s[e] = r[e](t), {
         c() {
-            n.c(), i = Ju();
+            n.c(), i = Qu();
         },
         m(l, u) {
             s[e].m(l, u), Po(l, i, u), o = !0;
         },
         p(l, u) {
             let c = e;
-            e = a(l), e === c ? s[e].p(l, u) : (Ku(), mn(s[c], 1, 1, () => {
+            e = a(l), e === c ? s[e].p(l, u) : (ec(), mn(s[c], 1, 1, () => {
                 s[c] = null;
-            }), xu(), n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), Ut(n, 1), n.m(i.parentNode, i));
+            }), Ju(), n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), Ut(n, 1), n.m(i.parentNode, i));
         },
         i(l) {
             o || (Ut(n), o = !0);
         },
         o(l) {
             mn(n), o = !1;
         },
@@ -12171,149 +12171,149 @@
     } = e, {
         hidden: d = !1
     } = e, {
         format: _ = "file"
     } = e, {
         uploading: m = !1
     } = e, {
-        hidden_upload: v = null
-    } = e, b, S, w;
+        hidden_upload: b = null
+    } = e, g, S, w;
     const k = ig("upload_files"),
         E = tg(),
         y = ["image", "video", "audio", "text", "file"],
         H = (p) => p.startsWith(".") || p.endsWith("/*") ? p : y.includes(p) ? p + "/*" : "." + p;
 
     function L() {
         n(18, s = !s);
     }
 
     function P() {
         navigator.clipboard.read().then(async (p) => {
-            for (let A = 0; A < p.length; A++) {
-                const q = p[A].types.find((z) => z.startsWith("image/"));
+            for (let T = 0; T < p.length; T++) {
+                const q = p[T].types.find((z) => z.startsWith("image/"));
                 if (q) {
-                    p[A].getType(q).then(async (z) => {
+                    p[T].getType(q).then(async (z) => {
                         const he = new File([z], `clipboard.${q.replace("image/", "")}`);
-                        await x([he]);
+                        await Z([he]);
                     });
                     break;
                 }
             }
         });
     }
 
-    function M() {
-        f || v && (n(2, v.value = "", v), v.click());
+    function D() {
+        f || b && (n(2, b.value = "", b), b.click());
     }
-    async function Z(p) {
-        await ng(), n(12, b = Math.random().toString(36).substring(2, 15)), n(1, m = !0);
-        const A = await Ra(p, h, b, k);
-        return E("load", c === "single" ? zl([A, "optionalAccess", (q) => q[0]]) : A), n(1, m = !1), A || [];
+    async function J(p) {
+        await ng(), n(12, g = Math.random().toString(36).substring(2, 15)), n(1, m = !0);
+        const T = await Ra(p, h, g, k);
+        return E("load", c === "single" ? zl([T, "optionalAccess", (q) => q[0]]) : T), n(1, m = !1), T || [];
     }
-    async function x(p) {
+    async function Z(p) {
         if (!p.length)
             return;
-        let A = p.map((q) => new File([q], q.name, {
+        let T = p.map((q) => new File([q], q.name, {
             type: q.type
         }));
-        return n(13, S = await Ba(A)), await Z(S);
+        return n(13, S = await Ba(T)), await J(S);
     }
     async function j(p) {
-        const A = p.target;
-        if (A.files)
+        const T = p.target;
+        if (T.files)
             if (_ != "blob")
-                await x(Array.from(A.files));
+                await Z(Array.from(T.files));
             else {
                 if (c === "single") {
-                    E("load", A.files[0]);
+                    E("load", T.files[0]);
                     return;
                 }
-                E("load", A.files);
+                E("load", T.files);
             }
     }
     async function X(p) {
         if (n(18, s = !1), !zl([p, "access", (q) => q.dataTransfer, "optionalAccess", (q) => q.files]))
             return;
-        const A = Array.from(p.dataTransfer.files).filter((q) => {
+        const T = Array.from(p.dataTransfer.files).filter((q) => {
             const z = "." + q.name.split(".").pop();
             return z && ag(w, z, q.type) || (z && Array.isArray(r) ? r.includes(z) : z === r) ? !0 : (E("error", `Invalid file type only ${r} allowed.`), !1);
         });
-        await x(A);
+        await Z(T);
     }
 
     function C(p) {
         xt.call(this, t, p);
     }
 
     function G(p) {
         xt.call(this, t, p);
     }
 
-    function I(p) {
+    function N(p) {
         xt.call(this, t, p);
     }
 
     function U(p) {
         xt.call(this, t, p);
     }
 
-    function K(p) {
+    function $(p) {
         xt.call(this, t, p);
     }
 
     function O(p) {
         xt.call(this, t, p);
     }
 
-    function J(p) {
+    function Y(p) {
         xt.call(this, t, p);
     }
 
-    function le(p) {
+    function se(p) {
         x1[p ? "unshift" : "push"](() => {
-            v = p, n(2, v);
+            b = p, n(2, b);
         });
     }
     return t.$$set = (p) => {
-        "filetype" in p && n(0, r = p.filetype), "dragging" in p && n(18, s = p.dragging), "boundedheight" in p && n(3, a = p.boundedheight), "center" in p && n(4, l = p.center), "flex" in p && n(5, u = p.flex), "file_count" in p && n(6, c = p.file_count), "disable_click" in p && n(7, f = p.disable_click), "root" in p && n(8, h = p.root), "hidden" in p && n(9, d = p.hidden), "format" in p && n(19, _ = p.format), "uploading" in p && n(1, m = p.uploading), "hidden_upload" in p && n(2, v = p.hidden_upload), "$$scope" in p && n(21, o = p.$$scope);
+        "filetype" in p && n(0, r = p.filetype), "dragging" in p && n(18, s = p.dragging), "boundedheight" in p && n(3, a = p.boundedheight), "center" in p && n(4, l = p.center), "flex" in p && n(5, u = p.flex), "file_count" in p && n(6, c = p.file_count), "disable_click" in p && n(7, f = p.disable_click), "root" in p && n(8, h = p.root), "hidden" in p && n(9, d = p.hidden), "format" in p && n(19, _ = p.format), "uploading" in p && n(1, m = p.uploading), "hidden_upload" in p && n(2, b = p.hidden_upload), "$$scope" in p && n(21, o = p.$$scope);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*filetype*/
             1 && (r == null ? n(14, w = null) : typeof r == "string" ? n(14, w = H(r)) : (n(0, r = r.map(H)), n(14, w = r.join(", "))));
     }, [
         r,
         m,
-        v,
+        b,
         a,
         l,
         u,
         c,
         f,
         h,
         d,
         P,
-        M,
-        b,
+        D,
+        g,
         S,
         w,
         L,
         j,
         X,
         s,
         _,
-        x,
+        Z,
         o,
         i,
         C,
         G,
-        I,
+        N,
         U,
-        K,
+        $,
         O,
-        J,
-        le
+        Y,
+        se
     ];
 }
 class cg extends X1 {
     constructor(e) {
         super(), Y1(
             this,
             e,
@@ -12373,15 +12373,15 @@
     createEventDispatcher: bg
 } = window.__gradio__svelte__internal;
 
 function Vl(t) {
     let e, n;
     return e = new Ei({
         props: {
-            Icon: wd,
+            Icon: kd,
             label: (
                 /*i18n*/
                 t[4]("common.edit")
             )
         }
     }), e.$on(
         "click",
@@ -12542,15 +12542,15 @@
         ),
         u = (
             /*download*/
             t[2] && xl(t)
         );
     return r = new Ei({
         props: {
-            Icon: rd,
+            Icon: ld,
             label: (
                 /*i18n*/
                 t[4]("common.clear")
             )
         }
     }), r.$on(
         "click",
@@ -12636,15 +12636,15 @@
         a,
         l,
         u,
         c,
         f
     ];
 }
-class tc extends fg {
+class ic extends fg {
     constructor(e) {
         super(), mg(this, e, yg, wg, gg, {
             editable: 0,
             undoable: 1,
             download: 2,
             absolute: 3,
             i18n: 4
@@ -12688,15 +12688,15 @@
             u.done ? o(u.value) : (c = u.value, c instanceof n ? c : new n(function(f) {
                 f(c);
             })).then(s, a);
         }
         l((i = i.apply(t, e || [])).next());
     });
 }
-class nc {
+class oc {
     constructor() {
         this.listeners = {};
     }
     on(e, n, i) {
         if (this.listeners[e] || (this.listeners[e] = /* @__PURE__ */ new Set()), this.listeners[e].add(n), i == null ? void 0 : i.once) {
             const o = () => {
                 this.un(e, o), this.un(e, n);
@@ -12717,27 +12717,27 @@
     unAll() {
         this.listeners = {};
     }
     emit(e, ...n) {
         this.listeners[e] && this.listeners[e].forEach((i) => i(...n));
     }
 }
-class kg extends nc {
+class kg extends oc {
     constructor(e) {
         super(), this.subscriptions = [], this.options = e;
     }
     onInit() {}
     _init(e) {
         this.wavesurfer = e, this.onInit();
     }
     destroy() {
         this.emit("destroy"), this.subscriptions.forEach((e) => e());
     }
 }
-class Eg extends nc {
+class Eg extends oc {
     constructor() {
         super(...arguments), this.unsubscribe = () => {};
     }
     start() {
         this.unsubscribe = this.on("tick", () => {
             requestAnimationFrame(() => {
                 this.emit("tick");
@@ -12890,25 +12890,25 @@
         this.wavesurfer && this.originalOptions && (this.wavesurfer.options.cursorWidth = this.originalOptions.cursorWidth, this.wavesurfer.options.interact = this.originalOptions.interact, delete this.originalOptions);
     }
 }
 const {
     SvelteComponent: Sg,
     append: be,
     attr: Ze,
-    binding_callbacks: ui,
+    binding_callbacks: ci,
     create_component: Ag,
     destroy_component: Tg,
     destroy_each: Pg,
     detach: Di,
     element: st,
     empty: Lg,
     ensure_array_like: Zl,
     init: Rg,
     insert: Hi,
-    listen: ci,
+    listen: fi,
     mount_component: Bg,
     run_all: Mg,
     safe_not_equal: Dg,
     set_data: nn,
     set_input_value: $r,
     space: Tn,
     text: on,
@@ -13051,99 +13051,99 @@
             /*i18n*/
             t[1]("audio.stop") + ""
         ),
         u, c, f, h, d = (
             /*i18n*/
             t[1]("audio.stop") + ""
         ),
-        _, m, v, b, S, w, k = (
+        _, m, b, g, S, w, k = (
             /*i18n*/
             t[1]("audio.resume") + ""
         ),
-        E, y, H, L, P, M, Z, x;
-    b = new Ga({});
+        E, y, H, L, P, D, J, Z;
+    g = new Ga({});
     let j = (
         /*timing*/
         t[4] && ! /*show_recording_waveform*/
         t[3] && Yl(t)
     );
 
-    function X(I, U) {
+    function X(N, U) {
         return (
             /*micDevices*/
-            I[5].length === 0 ? Ug : Ig
+            N[5].length === 0 ? Ug : Ig
         );
     }
     let C = X(t),
         G = C(t);
     return {
         c() {
-            e = st("div"), n = st("div"), i = st("button"), r = on(o), s = Tn(), a = st("button"), u = on(l), f = Tn(), h = st("button"), _ = on(d), m = Tn(), v = st("button"), Ag(b.$$.fragment), S = Tn(), w = st("button"), E = on(k), y = Tn(), j && j.c(), H = Tn(), L = st("select"), G.c(), Ze(i, "class", "record record-button svelte-l4xo8n"), Ze(a, "class", c = "stop-button " + /*record*/
-                    (t[0].isPaused() ? "stop-button-paused" : "") + " svelte-l4xo8n"), Ze(h, "id", "stop-paused"), Ze(h, "class", "stop-button-paused svelte-l4xo8n"), Ze(v, "class", "pause-button svelte-l4xo8n"), Ze(w, "class", "resume-button svelte-l4xo8n"), Ze(n, "class", "wrapper svelte-l4xo8n"), Ze(L, "class", "mic-select svelte-l4xo8n"), Ze(L, "aria-label", "Select input device"), L.disabled = P = /*micDevices*/
+            e = st("div"), n = st("div"), i = st("button"), r = on(o), s = Tn(), a = st("button"), u = on(l), f = Tn(), h = st("button"), _ = on(d), m = Tn(), b = st("button"), Ag(g.$$.fragment), S = Tn(), w = st("button"), E = on(k), y = Tn(), j && j.c(), H = Tn(), L = st("select"), G.c(), Ze(i, "class", "record record-button svelte-l4xo8n"), Ze(a, "class", c = "stop-button " + /*record*/
+                    (t[0].isPaused() ? "stop-button-paused" : "") + " svelte-l4xo8n"), Ze(h, "id", "stop-paused"), Ze(h, "class", "stop-button-paused svelte-l4xo8n"), Ze(b, "class", "pause-button svelte-l4xo8n"), Ze(w, "class", "resume-button svelte-l4xo8n"), Ze(n, "class", "wrapper svelte-l4xo8n"), Ze(L, "class", "mic-select svelte-l4xo8n"), Ze(L, "aria-label", "Select input device"), L.disabled = P = /*micDevices*/
                 t[5].length === 0, Ze(e, "class", "controls svelte-l4xo8n");
         },
-        m(I, U) {
-            Hi(I, e, U), be(e, n), be(n, i), be(i, r), t[11](i), be(n, s), be(n, a), be(a, u), t[13](a), be(n, f), be(n, h), be(h, _), t[15](h), be(n, m), be(n, v), Bg(b, v, null), t[17](v), be(n, S), be(n, w), be(w, E), t[19](w), be(n, y), j && j.m(n, null), be(e, H), be(e, L), G.m(L, null), M = !0, Z || (x = [
-                ci(
+        m(N, U) {
+            Hi(N, e, U), be(e, n), be(n, i), be(i, r), t[11](i), be(n, s), be(n, a), be(a, u), t[13](a), be(n, f), be(n, h), be(h, _), t[15](h), be(n, m), be(n, b), Bg(g, b, null), t[17](b), be(n, S), be(n, w), be(w, E), t[19](w), be(n, y), j && j.m(n, null), be(e, H), be(e, L), G.m(L, null), D = !0, J || (Z = [
+                fi(
                     i,
                     "click",
                     /*click_handler*/
                     t[12]
                 ),
-                ci(
+                fi(
                     a,
                     "click",
                     /*click_handler_1*/
                     t[14]
                 ),
-                ci(
+                fi(
                     h,
                     "click",
                     /*click_handler_2*/
                     t[16]
                 ),
-                ci(
-                    v,
+                fi(
+                    b,
                     "click",
                     /*click_handler_3*/
                     t[18]
                 ),
-                ci(
+                fi(
                     w,
                     "click",
                     /*click_handler_4*/
                     t[20]
                 )
-            ], Z = !0);
+            ], J = !0);
         },
-        p(I, [U]) {
-            (!M || U & /*i18n*/
+        p(N, [U]) {
+            (!D || U & /*i18n*/
                 2) && o !== (o = /*i18n*/
-                    I[1]("audio.record") + "") && nn(r, o), (!M || U & /*i18n*/
+                    N[1]("audio.record") + "") && nn(r, o), (!D || U & /*i18n*/
                     2) && l !== (l = /*i18n*/
-                    I[1]("audio.stop") + "") && nn(u, l), (!M || U & /*record*/
+                    N[1]("audio.stop") + "") && nn(u, l), (!D || U & /*record*/
                     1 && c !== (c = "stop-button " + /*record*/
-                        (I[0].isPaused() ? "stop-button-paused" : "") + " svelte-l4xo8n")) && Ze(a, "class", c), (!M || U & /*i18n*/
+                        (N[0].isPaused() ? "stop-button-paused" : "") + " svelte-l4xo8n")) && Ze(a, "class", c), (!D || U & /*i18n*/
                     2) && d !== (d = /*i18n*/
-                    I[1]("audio.stop") + "") && nn(_, d), (!M || U & /*i18n*/
+                    N[1]("audio.stop") + "") && nn(_, d), (!D || U & /*i18n*/
                     2) && k !== (k = /*i18n*/
-                    I[1]("audio.resume") + "") && nn(E, k), /*timing*/
-                I[4] && ! /*show_recording_waveform*/
-                I[3] ? j ? j.p(I, U) : (j = Yl(I), j.c(), j.m(n, null)) : j && (j.d(1), j = null), C === (C = X(I)) && G ? G.p(I, U) : (G.d(1), G = C(I), G && (G.c(), G.m(L, null))), (!M || U & /*micDevices*/
+                    N[1]("audio.resume") + "") && nn(E, k), /*timing*/
+                N[4] && ! /*show_recording_waveform*/
+                N[3] ? j ? j.p(N, U) : (j = Yl(N), j.c(), j.m(n, null)) : j && (j.d(1), j = null), C === (C = X(N)) && G ? G.p(N, U) : (G.d(1), G = C(N), G && (G.c(), G.m(L, null))), (!D || U & /*micDevices*/
                     32 && P !== (P = /*micDevices*/
-                        I[5].length === 0)) && (L.disabled = P);
+                        N[5].length === 0)) && (L.disabled = P);
         },
-        i(I) {
-            M || (Hg(b.$$.fragment, I), M = !0);
+        i(N) {
+            D || (Hg(g.$$.fragment, N), D = !0);
         },
-        o(I) {
-            Og(b.$$.fragment, I), M = !1;
+        o(N) {
+            Og(g.$$.fragment, N), D = !1;
         },
-        d(I) {
-            I && Di(e), t[11](null), t[13](null), t[15](null), Tg(b), t[17](null), t[19](null), j && j.d(), G.d(), Z = !1, Mg(x);
+        d(N) {
+            N && Di(e), t[11](null), t[13](null), t[15](null), Tg(g), t[17](null), t[19](null), j && j.d(), G.d(), J = !1, Mg(Z);
         }
     };
 }
 
 function Fg(t, e, n) {
     let {
         record: i
@@ -13155,61 +13155,61 @@
         show_recording_waveform: h
     } = e, {
         timing: d = !1
     } = e;
     const _ = Ng();
 
     function m(P) {
-        ui[P ? "unshift" : "push"](() => {
+        ci[P ? "unshift" : "push"](() => {
             s = P, n(6, s), n(0, i);
         });
     }
-    const v = () => i.startRecording();
+    const b = () => i.startRecording();
 
-    function b(P) {
-        ui[P ? "unshift" : "push"](() => {
+    function g(P) {
+        ci[P ? "unshift" : "push"](() => {
             u = P, n(9, u), n(0, i);
         });
     }
     const S = () => {
         i.isPaused() && (i.resumeRecording(), i.stopRecording()), i.stopRecording();
     };
 
     function w(P) {
-        ui[P ? "unshift" : "push"](() => {
+        ci[P ? "unshift" : "push"](() => {
             c = P, n(10, c), n(0, i);
         });
     }
     const k = () => {
         i.isPaused() && (i.resumeRecording(), i.stopRecording()), i.stopRecording();
     };
 
     function E(P) {
-        ui[P ? "unshift" : "push"](() => {
+        ci[P ? "unshift" : "push"](() => {
             a = P, n(7, a), n(0, i);
         });
     }
     const y = () => i.pauseRecording();
 
     function H(P) {
-        ui[P ? "unshift" : "push"](() => {
+        ci[P ? "unshift" : "push"](() => {
             l = P, n(8, l), n(0, i);
         });
     }
     const L = () => i.resumeRecording();
     return t.$$set = (P) => {
         "record" in P && n(0, i = P.record), "i18n" in P && n(1, o = P.i18n), "record_time" in P && n(2, f = P.record_time), "show_recording_waveform" in P && n(3, h = P.show_recording_waveform), "timing" in P && n(4, d = P.timing);
     }, t.$$.update = () => {
         if (t.$$.dirty & /*i18n*/
             2)
             try {
                 let P = [];
-                Mi.getAvailableAudioDevices().then((M) => {
-                    n(5, r = M), M.forEach((Z) => {
-                        Z.deviceId && P.push(Z);
+                Mi.getAvailableAudioDevices().then((D) => {
+                    n(5, r = D), D.forEach((J) => {
+                        J.deviceId && P.push(J);
                     }), n(5, r = P);
                 });
             } catch (P) {
                 throw P instanceof DOMException && P.name == "NotAllowedError" && _("error", o("audio.allow_recording_access")), P;
             }
         t.$$.dirty & /*record*/
             1 && i.on("record-start", () => {
@@ -13233,16 +13233,16 @@
         r,
         s,
         a,
         l,
         u,
         c,
         m,
-        v,
         b,
+        g,
         S,
         w,
         k,
         E,
         y,
         H,
         L
@@ -13257,35 +13257,35 @@
             show_recording_waveform: 3,
             timing: 4
         });
     }
 }
 const {
     SvelteComponent: zg,
-    add_flush_callback: ic,
+    add_flush_callback: rc,
     append: at,
     attr: Ct,
-    bind: oc,
-    binding_callbacks: Bn,
+    bind: sc,
+    binding_callbacks: Mn,
     check_outros: Kl,
-    create_component: rc,
-    destroy_component: sc,
+    create_component: lc,
+    destroy_component: ac,
     detach: Oi,
     element: At,
     group_outros: $l,
     init: Gg,
     insert: Ni,
-    mount_component: lc,
-    noop: ac,
+    mount_component: uc,
+    noop: cc,
     safe_not_equal: Wg,
     set_data: Vg,
-    space: Mn,
+    space: Dn,
     text: Xg,
     transition_in: Ot,
-    transition_out: Dn
+    transition_out: Hn
 } = window.__gradio__svelte__internal, {
     onMount: xg
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: Zg
 } = window.__gradio__svelte__internal;
 
 function ea(t) {
@@ -13300,15 +13300,15 @@
             c[13] ? Yg : Jg
         );
     }
     let l = a(t),
         u = l(t);
     return {
         c() {
-            e = At("div"), n = At("time"), n.textContent = "0:00", i = Mn(), o = At("div"), s && s.c(), r = Mn(), u.c(), Ct(n, "class", "time svelte-1z0uz8p"), Ct(e, "class", "timestamps svelte-1z0uz8p");
+            e = At("div"), n = At("time"), n.textContent = "0:00", i = Dn(), o = At("div"), s && s.c(), r = Dn(), u.c(), Ct(n, "class", "time svelte-1z0uz8p"), Ct(e, "class", "timestamps svelte-1z0uz8p");
         },
         m(c, f) {
             Ni(c, e, f), at(e, n), t[19](n), at(e, i), at(e, o), s && s.m(o, null), at(o, r), u.m(o, null);
         },
         p(c, f) {
             /*mode*/
             c[0] === "edit" && es > 0 ? s ? s.p(c, f) : (s = ta(), s.c(), s.m(o, r)) : s && (s.d(1), s = null), l === (l = a(c)) && u ? u.p(c, f) : (u.d(1), u = l(c), u && (u.c(), u.m(o, null)));
@@ -13324,15 +13324,15 @@
     return {
         c() {
             e = At("time"), e.textContent = `${un(es)}`, Ct(e, "class", "trim-duration svelte-1z0uz8p");
         },
         m(n, i) {
             Ni(n, e, i);
         },
-        p: ac,
+        p: cc,
         d(n) {
             n && Oi(e);
         }
     };
 }
 
 function Jg(t) {
@@ -13340,15 +13340,15 @@
     return {
         c() {
             e = At("time"), e.textContent = "0:00", Ct(e, "class", "duration svelte-1z0uz8p");
         },
         m(n, i) {
             Ni(n, e, i), t[20](e);
         },
-        p: ac,
+        p: cc,
         d(n) {
             n && Oi(e), t[20](null);
         }
     };
 }
 
 function Yg(t) {
@@ -13402,20 +13402,20 @@
         )
     };
     return (
         /*record*/
         t[6] !== void 0 && (r.record = /*record*/
             t[6]), e = new qg({
             props: r
-        }), Bn.push(() => oc(e, "record", o)), {
+        }), Mn.push(() => sc(e, "record", o)), {
             c() {
-                rc(e.$$.fragment);
+                lc(e.$$.fragment);
             },
             m(s, a) {
-                lc(e, s, a), i = !0;
+                uc(e, s, a), i = !0;
             },
             p(s, a) {
                 const l = {};
                 a & /*i18n*/
                     2 && (l.i18n = /*i18n*/
                         s[1]), a & /*timing*/
                     8192 && (l.timing = /*timing*/
@@ -13423,24 +13423,24 @@
                     4 && (l.show_recording_waveform = /*waveform_options*/
                         s[2].show_recording_waveform), a & /*seconds*/
                     4096 && (l.record_time = un(
                         /*seconds*/
                         s[12]
                     )), !n && a & /*record*/
                     64 && (n = !0, l.record = /*record*/
-                        s[6], ic(() => n = !1)), e.$set(l);
+                        s[6], rc(() => n = !1)), e.$set(l);
             },
             i(s) {
                 i || (Ot(e.$$.fragment, s), i = !0);
             },
             o(s) {
-                Dn(e.$$.fragment, s), i = !1;
+                Hn(e.$$.fragment, s), i = !1;
             },
             d(s) {
-                sc(e, s);
+                ac(e, s);
             }
         }
     );
 }
 
 function ia(t) {
     let e, n, i;
@@ -13467,43 +13467,43 @@
         )
     };
     return (
         /*recordingWaveform*/
         t[3] !== void 0 && (r.waveform = /*recordingWaveform*/
             t[3]), e = new nu({
             props: r
-        }), Bn.push(() => oc(e, "waveform", o)), {
+        }), Mn.push(() => sc(e, "waveform", o)), {
             c() {
-                rc(e.$$.fragment);
+                lc(e.$$.fragment);
             },
             m(s, a) {
-                lc(e, s, a), i = !0;
+                uc(e, s, a), i = !0;
             },
             p(s, a) {
                 const l = {};
                 a & /*playing*/
                     1024 && (l.playing = /*playing*/
                         s[10]), a & /*audio_duration*/
                     2048 && (l.audio_duration = /*audio_duration*/
                         s[11]), a & /*i18n*/
                     2 && (l.i18n = /*i18n*/
                         s[1]), a & /*waveform_options*/
                     4 && (l.waveform_options = /*waveform_options*/
                         s[2]), !n && a & /*recordingWaveform*/
                     8 && (n = !0, l.waveform = /*recordingWaveform*/
-                        s[3], ic(() => n = !1)), e.$set(l);
+                        s[3], rc(() => n = !1)), e.$set(l);
             },
             i(s) {
                 i || (Ot(e.$$.fragment, s), i = !0);
             },
             o(s) {
-                Dn(e.$$.fragment, s), i = !1;
+                Hn(e.$$.fragment, s), i = !1;
             },
             d(s) {
-                sc(e, s);
+                ac(e, s);
             }
         }
     );
 }
 
 function Qg(t) {
     let e, n, i, o, r, s, a, l, u = (
@@ -13520,40 +13520,40 @@
         f = (
             /*recordingWaveform*/
             t[3] && /*recordedAudio*/
             t[7] && ia(t)
         );
     return {
         c() {
-            e = At("div"), n = At("div"), i = Mn(), o = At("div"), r = Mn(), u && u.c(), s = Mn(), c && c.c(), a = Mn(), f && f.c(), Ct(n, "class", "microphone svelte-1z0uz8p"), Ct(n, "data-testid", "microphone-waveform"), Ct(o, "data-testid", "recording-waveform"), Ct(e, "class", "component-wrapper svelte-1z0uz8p");
+            e = At("div"), n = At("div"), i = Dn(), o = At("div"), r = Dn(), u && u.c(), s = Dn(), c && c.c(), a = Dn(), f && f.c(), Ct(n, "class", "microphone svelte-1z0uz8p"), Ct(n, "data-testid", "microphone-waveform"), Ct(o, "data-testid", "recording-waveform"), Ct(e, "class", "component-wrapper svelte-1z0uz8p");
         },
         m(h, d) {
             Ni(h, e, d), at(e, n), t[17](n), at(e, i), at(e, o), t[18](o), at(e, r), u && u.m(e, null), at(e, s), c && c.m(e, null), at(e, a), f && f.m(e, null), l = !0;
         },
         p(h, [d]) {
             /*timing*/
             (h[13] || /*recordedAudio*/
                 h[7]) && /*waveform_options*/
             h[2].show_recording_waveform ? u ? u.p(h, d) : (u = ea(h), u.c(), u.m(e, s)) : u && (u.d(1), u = null), /*microphoneContainer*/
                 h[5] && ! /*recordedAudio*/
                 h[7] ? c ? (c.p(h, d), d & /*microphoneContainer, recordedAudio*/
-                    160 && Ot(c, 1)) : (c = na(h), c.c(), Ot(c, 1), c.m(e, a)) : c && ($l(), Dn(c, 1, 1, () => {
+                    160 && Ot(c, 1)) : (c = na(h), c.c(), Ot(c, 1), c.m(e, a)) : c && ($l(), Hn(c, 1, 1, () => {
                     c = null;
                 }), Kl()), /*recordingWaveform*/
                 h[3] && /*recordedAudio*/
                 h[7] ? f ? (f.p(h, d), d & /*recordingWaveform, recordedAudio*/
-                    136 && Ot(f, 1)) : (f = ia(h), f.c(), Ot(f, 1), f.m(e, null)) : f && ($l(), Dn(f, 1, 1, () => {
+                    136 && Ot(f, 1)) : (f = ia(h), f.c(), Ot(f, 1), f.m(e, null)) : f && ($l(), Hn(f, 1, 1, () => {
                     f = null;
                 }), Kl());
         },
         i(h) {
             l || (Ot(c), Ot(f), l = !0);
         },
         o(h) {
-            Dn(c), Dn(f), l = !1;
+            Hn(c), Hn(f), l = !1;
         },
         d(h) {
             h && Oi(e), t[17](null), t[18](null), u && u.d(), c && c.d(), f && f.d();
         }
     };
 }
 let es = 0;
@@ -13580,15 +13580,15 @@
         dispatch_blob: r
     } = e, {
         waveform_settings: s
     } = e, {
         waveform_options: a = {
             show_recording_waveform: !0
         }
-    } = e, l, u, c = !1, f, h, d, _ = null, m, v, b, S = 0, w, k = !1;
+    } = e, l, u, c = !1, f, h, d, _ = null, m, b, g, S = 0, w, k = !1;
     const E = () => {
             clearInterval(w), n(16, w = setInterval(
                 () => {
                     n(12, S++, S);
                 },
                 1e3
             ));
@@ -13612,34 +13612,34 @@
     xg(() => {
         H(), window.addEventListener("keydown", (C) => {
             C.key === "ArrowRight" ? Qs(u, 0.1) : C.key === "ArrowLeft" && Qs(u, -0.1);
         });
     });
 
     function P(C) {
-        Bn[C ? "unshift" : "push"](() => {
+        Mn[C ? "unshift" : "push"](() => {
             h = C, n(5, h);
         });
     }
 
-    function M(C) {
-        Bn[C ? "unshift" : "push"](() => {
+    function D(C) {
+        Mn[C ? "unshift" : "push"](() => {
             f = C, n(4, f);
         });
     }
 
-    function Z(C) {
-        Bn[C ? "unshift" : "push"](() => {
+    function J(C) {
+        Mn[C ? "unshift" : "push"](() => {
             m = C, n(8, m), n(3, u);
         });
     }
 
-    function x(C) {
-        Bn[C ? "unshift" : "push"](() => {
-            v = C, n(9, v), n(3, u);
+    function Z(C) {
+        Mn[C ? "unshift" : "push"](() => {
+            b = C, n(9, b), n(3, u);
         });
     }
 
     function j(C) {
         d = C, n(6, d);
     }
 
@@ -13666,23 +13666,23 @@
                 d,
                 "optionalAccess",
                 (C) => C.on,
                 "call",
                 (C) => C("record-end", async (G) => {
                     n(12, S = 0), n(13, k = !1), clearInterval(w);
                     try {
-                        const I = await G.arrayBuffer(),
-                            K = await new AudioContext({
+                        const N = await G.arrayBuffer(),
+                            $ = await new AudioContext({
                                 sampleRate: s.sampleRate
-                            }).decodeAudioData(I);
-                        console.log(K), K && await V_(K).then(async (O) => {
+                            }).decodeAudioData(N);
+                        console.log($), $ && await x_($).then(async (O) => {
                             await r([O], "change"), await r([O], "stop_recording");
                         });
-                    } catch (I) {
-                        console.error(I);
+                    } catch (N) {
+                        console.error(N);
                     }
                 })
             ]), t.$$.dirty & /*record, interval*/
             65600 && mt([
                 d,
                 "optionalAccess",
                 (C) => C.on,
@@ -13702,15 +13702,15 @@
             ]), t.$$.dirty & /*recordingWaveform, durationRef*/
             520 && mt([
                 u,
                 "optionalAccess",
                 (C) => C.on,
                 "call",
                 (C) => C("decode", (G) => {
-                    n(11, b = G), v && n(9, v.textContent = un(G), v);
+                    n(11, g = G), b && n(9, b.textContent = un(G), b);
                 })
             ]), t.$$.dirty & /*recordingWaveform, timeRef*/
             264 && mt([
                 u,
                 "optionalAccess",
                 (C) => C.on,
                 "call",
@@ -13746,41 +13746,41 @@
             240 && mt([
                 d,
                 "optionalAccess",
                 (C) => C.on,
                 "call",
                 (C) => C("record-end", (G) => {
                     n(7, _ = URL.createObjectURL(G));
-                    const I = h,
+                    const N = h,
                         U = f;
-                    I && (I.style.display = "none"), U && _ && (U.innerHTML = "", L());
+                    N && (N.style.display = "none"), U && _ && (U.innerHTML = "", L());
                 })
             ]);
     }, [
         i,
         o,
         a,
         u,
         f,
         h,
         d,
         _,
         m,
-        v,
-        c,
         b,
+        c,
+        g,
         S,
         k,
         r,
         s,
         w,
         P,
-        M,
+        D,
+        J,
         Z,
-        x,
         j,
         X
     ];
 }
 class $g extends zg {
     constructor(e) {
         super(), Gg(this, e, Kg, Qg, Wg, {
@@ -13791,37 +13791,37 @@
             waveform_options: 2
         });
     }
 }
 const {
     SvelteComponent: eb,
     append: an,
-    attr: Nn,
+    attr: In,
     binding_callbacks: tb,
     detach: Lo,
-    element: qn,
+    element: zn,
     init: nb,
     insert: Ro,
-    listen: uc,
+    listen: fc,
     noop: oa,
     null_to_empty: ra,
     safe_not_equal: ib,
-    set_data: cc,
+    set_data: dc,
     set_style: sa,
     space: hs,
-    text: fc
+    text: hc
 } = window.__gradio__svelte__internal, {
     onMount: ob
 } = window.__gradio__svelte__internal;
 
 function la(t) {
     let e;
     return {
         c() {
-            e = qn("div"), sa(
+            e = zn("div"), sa(
                 e,
                 "display",
                 /*recording*/
                 t[0] ? "block" : "none"
             );
         },
         m(n, i) {
@@ -13846,28 +13846,28 @@
     let e, n, i, o = (
             /*i18n*/
             t[4]("audio.record") + ""
         ),
         r, s, a;
     return {
         c() {
-            e = qn("button"), n = qn("span"), n.innerHTML = '<span class="dot"></span>', i = hs(), r = fc(o), Nn(n, "class", "record-icon"), Nn(e, "class", "record-button svelte-4ycsjo");
+            e = zn("button"), n = zn("span"), n.innerHTML = '<span class="dot"></span>', i = hs(), r = hc(o), In(n, "class", "record-icon"), In(e, "class", "record-button svelte-4ycsjo");
         },
         m(l, u) {
-            Ro(l, e, u), an(e, n), an(e, i), an(e, r), s || (a = uc(
+            Ro(l, e, u), an(e, n), an(e, i), an(e, r), s || (a = fc(
                 e,
                 "click",
                 /*click_handler_1*/
                 t[11]
             ), s = !0);
         },
         p(l, u) {
             u & /*i18n*/
                 16 && o !== (o = /*i18n*/
-                    l[4]("audio.record") + "") && cc(r, o);
+                    l[4]("audio.record") + "") && dc(r, o);
         },
         d(l) {
             l && Lo(e), s = !1, a();
         }
     };
 }
 
@@ -13881,21 +13881,21 @@
                 /*i18n*/
                 t[4]("audio.stop")
             )) + ""
         ),
         r, s, a, l;
     return {
         c() {
-            e = qn("button"), n = qn("span"), n.innerHTML = '<span class="pinger"></span> <span class="dot"></span>', i = hs(), r = fc(o), Nn(n, "class", "record-icon"), Nn(e, "class", s = ra(
+            e = zn("button"), n = zn("span"), n.innerHTML = '<span class="pinger"></span> <span class="dot"></span>', i = hs(), r = hc(o), In(n, "class", "record-icon"), In(e, "class", s = ra(
                 /*paused_recording*/
                 t[1] ? "stop-button-paused" : "stop-button"
             ) + " svelte-4ycsjo");
         },
         m(u, c) {
-            Ro(u, e, c), an(e, n), an(e, i), an(e, r), a || (l = uc(
+            Ro(u, e, c), an(e, n), an(e, i), an(e, r), a || (l = fc(
                 e,
                 "click",
                 /*click_handler*/
                 t[10]
             ), a = !0);
         },
         p(u, c) {
@@ -13903,19 +13903,19 @@
                 18 && o !== (o = /*paused_recording*/
                     (u[1] ? (
                         /*i18n*/
                         u[4]("audio.pause")
                     ) : (
                         /*i18n*/
                         u[4]("audio.stop")
-                    )) + "") && cc(r, o), c & /*paused_recording*/
+                    )) + "") && dc(r, o), c & /*paused_recording*/
                 2 && s !== (s = ra(
                     /*paused_recording*/
                     u[1] ? "stop-button-paused" : "stop-button"
-                ) + " svelte-4ycsjo") && Nn(e, "class", s);
+                ) + " svelte-4ycsjo") && In(e, "class", s);
         },
         d(u) {
             u && Lo(e), a = !1, l();
         }
     };
 }
 
@@ -13931,15 +13931,15 @@
             a[0] ? sb : rb
         );
     }
     let r = o(t),
         s = r(t);
     return {
         c() {
-            e = qn("div"), i && i.c(), n = hs(), s.c(), Nn(e, "class", "mic-wrap svelte-4ycsjo");
+            e = zn("div"), i && i.c(), n = hs(), s.c(), In(e, "class", "mic-wrap svelte-4ycsjo");
         },
         m(a, l) {
             Ro(a, e, l), i && i.m(e, null), an(e, n), s.m(e, null);
         },
         p(a, [l]) {
             /*waveform_options*/
             a[5].show_recording_waveform ? i ? i.p(a, l) : (i = la(a), i.c(), i.m(e, n)) : i && (i.d(1), i = null), r === (r = o(a)) && s ? s.p(a, l) : (s.d(1), s = r(a), s && (s.c(), s.m(e, null)));
@@ -13977,40 +13977,40 @@
         c !== void 0 && c.destroy(), h && (c = Ft.create({
             ...l,
             height: 100,
             container: h
         }), n(6, f = c.registerPlugin(Mi.create())));
     };
 
-    function _(b) {
-        tb[b ? "unshift" : "push"](() => {
-            h = b, n(7, h);
+    function _(g) {
+        tb[g ? "unshift" : "push"](() => {
+            h = g, n(7, h);
         });
     }
     const m = () => {
             f == null || f.stopMic(), r();
         },
-        v = () => {
+        b = () => {
             f == null || f.startMic(), s();
         };
-    return t.$$set = (b) => {
-        "recording" in b && n(0, i = b.recording), "paused_recording" in b && n(1, o = b.paused_recording), "stop" in b && n(2, r = b.stop), "record" in b && n(3, s = b.record), "i18n" in b && n(4, a = b.i18n), "waveform_settings" in b && n(8, l = b.waveform_settings), "waveform_options" in b && n(5, u = b.waveform_options);
+    return t.$$set = (g) => {
+        "recording" in g && n(0, i = g.recording), "paused_recording" in g && n(1, o = g.paused_recording), "stop" in g && n(2, r = g.stop), "record" in g && n(3, s = g.record), "i18n" in g && n(4, a = g.i18n), "waveform_settings" in g && n(8, l = g.waveform_settings), "waveform_options" in g && n(5, u = g.waveform_options);
     }, [
         i,
         o,
         r,
         s,
         a,
         u,
         f,
         h,
         l,
         _,
         m,
-        v
+        b
     ];
 }
 class ub extends eb {
     constructor(e) {
         super(), nb(this, e, ab, lb, ib, {
             recording: 0,
             paused_recording: 1,
@@ -14028,36 +14028,36 @@
     bind: Mo,
     binding_callbacks: Do,
     bubble: Tr,
     check_outros: _s,
     create_component: qt,
     create_slot: fb,
     destroy_component: zt,
-    detach: zn,
-    empty: dc,
+    detach: Gn,
+    empty: _c,
     get_all_dirty_from_scope: db,
     get_slot_changes: hb,
     group_outros: ms,
     init: _b,
-    insert: Gn,
+    insert: Wn,
     mount_component: Gt,
     safe_not_equal: mb,
     space: fo,
     transition_in: He,
     transition_out: Oe,
     update_slot_base: pb
 } = window.__gradio__svelte__internal, {
     getContext: gb,
     onDestroy: bb,
     createEventDispatcher: vb
 } = window.__gradio__svelte__internal;
 
 function wb(t) {
     let e, n, i, o, r;
-    e = new tc({
+    e = new ic({
         props: {
             i18n: (
                 /*i18n*/
                 t[9]
             ),
             download: (
                 /*show_download_button*/
@@ -14107,15 +14107,15 @@
             t[12]
         ),
         interactive: !0
     };
     return (
         /*mode*/
         t[14] !== void 0 && (a.mode = /*mode*/
-            t[14]), i = new _u({
+            t[14]), i = new pu({
             props: a
         }), Do.push(() => Mo(i, "mode", s)), i.$on(
             "stop",
             /*stop_handler*/
             t[31]
         ), i.$on(
             "play",
@@ -14130,15 +14130,15 @@
             /*edit_handler_1*/
             t[34]
         ), {
             c() {
                 qt(e.$$.fragment), n = fo(), qt(i.$$.fragment);
             },
             m(l, u) {
-                Gt(e, l, u), Gn(l, n, u), Gt(i, l, u), r = !0;
+                Gt(e, l, u), Wn(l, n, u), Gt(i, l, u), r = !0;
             },
             p(l, u) {
                 const c = {};
                 u[0] & /*i18n*/
                     512 && (c.i18n = /*i18n*/
                         l[9]), u[0] & /*show_download_button, value*/
                     66 && (c.download = /*show_download_button*/
@@ -14166,15 +14166,15 @@
             i(l) {
                 r || (He(e.$$.fragment, l), He(i.$$.fragment, l), r = !0);
             },
             o(l) {
                 Oe(e.$$.fragment, l), Oe(i.$$.fragment, l), r = !1;
             },
             d(l) {
-                l && zn(n), zt(e, l), zt(i, l);
+                l && Gn(n), zt(e, l), zt(i, l);
             }
         }
     );
 }
 
 function yb(t) {
     let e, n, i, o;
@@ -14188,33 +14188,33 @@
                 /*active_source*/
                 l[2] === "upload" ? 1 : -1
             )
         );
     }
     return ~(e = a(t)) && (n = s[e] = r[e](t)), {
         c() {
-            n && n.c(), i = dc();
+            n && n.c(), i = _c();
         },
         m(l, u) {
-            ~e && s[e].m(l, u), Gn(l, i, u), o = !0;
+            ~e && s[e].m(l, u), Wn(l, i, u), o = !0;
         },
         p(l, u) {
             let c = e;
             e = a(l), e === c ? ~e && s[e].p(l, u) : (n && (ms(), Oe(s[c], 1, 1, () => {
                 s[c] = null;
             }), _s()), ~e ? (n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), He(n, 1), n.m(i.parentNode, i)) : n = null);
         },
         i(l) {
             o || (He(n), o = !0);
         },
         o(l) {
             Oe(n), o = !1;
         },
         d(l) {
-            l && zn(i), ~e && s[e].d(l);
+            l && Gn(i), ~e && s[e].d(l);
         }
     };
 }
 
 function kb(t) {
     let e, n, i;
 
@@ -14277,15 +14277,15 @@
             }
         }
     );
 }
 
 function Eb(t) {
     let e, n, i, o, r, s;
-    e = new tc({
+    e = new ic({
         props: {
             i18n: (
                 /*i18n*/
                 t[9]
             ),
             absolute: !0
         }
@@ -14301,18 +14301,18 @@
         return (
             /*streaming*/
             c[8] ? 0 : 1
         );
     }
     return i = u(t), o = l[i] = a[i](t), {
         c() {
-            qt(e.$$.fragment), n = fo(), o.c(), r = dc();
+            qt(e.$$.fragment), n = fo(), o.c(), r = _c();
         },
         m(c, f) {
-            Gt(e, c, f), Gn(c, n, f), l[i].m(c, f), Gn(c, r, f), s = !0;
+            Gt(e, c, f), Wn(c, n, f), l[i].m(c, f), Wn(c, r, f), s = !0;
         },
         p(c, f) {
             const h = {};
             f[0] & /*i18n*/
                 512 && (h.i18n = /*i18n*/
                     c[9]), e.$set(h);
             let d = i;
@@ -14323,15 +14323,15 @@
         i(c) {
             s || (He(e.$$.fragment, c), He(o), s = !0);
         },
         o(c) {
             Oe(e.$$.fragment, c), Oe(o), s = !1;
         },
         d(c) {
-            c && (zn(n), zn(r)), zt(e, c), l[i].d(c);
+            c && (Gn(n), Gn(r)), zt(e, c), l[i].d(c);
         }
     };
 }
 
 function Cb(t) {
     let e;
     const n = (
@@ -14551,37 +14551,37 @@
             /*clear*/
             t[18]
         )
     };
     return (
         /*active_source*/
         t[2] !== void 0 && (d.active_source = /*active_source*/
-            t[2]), s = new y_({
+            t[2]), s = new E_({
             props: d
         }), Do.push(() => Mo(s, "active_source", h)), {
             c() {
                 qt(e.$$.fragment), n = fo(), o.c(), r = fo(), qt(s.$$.fragment);
             },
             m(_, m) {
-                Gt(e, _, m), Gn(_, n, m), c[i].m(_, m), Gn(_, r, m), Gt(s, _, m), l = !0;
+                Gt(e, _, m), Wn(_, n, m), c[i].m(_, m), Wn(_, r, m), Gt(s, _, m), l = !0;
             },
             p(_, m) {
-                const v = {};
+                const b = {};
                 m[0] & /*show_label*/
-                    32 && (v.show_label = /*show_label*/
+                    32 && (b.show_label = /*show_label*/
                         _[5]), m[0] & /*active_source, value*/
-                    6 && (v.float = /*active_source*/
+                    6 && (b.float = /*active_source*/
                         _[2] === "upload" && /*value*/
                         _[1] === null), m[0] & /*label, i18n*/
-                    520 && (v.label = /*label*/
+                    520 && (b.label = /*label*/
                         _[3] || /*i18n*/
-                        _[9]("audio.audio")), e.$set(v);
-                let b = i;
-                i = f(_), i === b ? c[i].p(_, m) : (ms(), Oe(c[b], 1, 1, () => {
-                    c[b] = null;
+                        _[9]("audio.audio")), e.$set(b);
+                let g = i;
+                i = f(_), i === g ? c[i].p(_, m) : (ms(), Oe(c[g], 1, 1, () => {
+                    c[g] = null;
                 }), _s(), o = c[i], o ? o.p(_, m) : (o = c[i] = u[i](_), o.c()), He(o, 1), o.m(r.parentNode, r));
                 const S = {};
                 m[0] & /*sources*/
                     128 && (S.sources = /*sources*/
                         _[7]), !a && m[0] & /*active_source*/
                     4 && (a = !0, S.active_source = /*active_source*/
                         _[2], Bo(() => a = !1)), s.$set(S);
@@ -14589,15 +14589,15 @@
             i(_) {
                 l || (He(e.$$.fragment, _), He(o), He(s.$$.fragment, _), l = !0);
             },
             o(_) {
                 Oe(e.$$.fragment, _), Oe(o), Oe(s.$$.fragment, _), l = !1;
             },
             d(_) {
-                _ && (zn(n), zn(r)), zt(e, _), c[i].d(_), zt(s, _);
+                _ && (Gn(n), Gn(r)), zt(e, _), c[i].d(_), zt(s, _);
             }
         }
     );
 }
 const Pb = 500,
     aa = 44;
 async function Lb(t) {
@@ -14636,162 +14636,162 @@
     } = e, {
         i18n: d
     } = e, {
         waveform_settings: _
     } = e, {
         waveform_options: m = {}
     } = e, {
-        dragging: v
+        dragging: b
     } = e, {
-        active_source: b
+        active_source: g
     } = e, {
         editable: S = !0
     } = e;
     const w = gb("upload_files");
     let k = !1,
         E, y = "",
         H, L = [],
         P = !1,
-        M = !1,
-        Z = [],
-        x;
+        D = !1,
+        J = [],
+        Z;
 
     function j() {
-        x = [
+        Z = [
             import("./module-d82531d9.js"),
             import("./module-aafe8b06.js")
         ];
     }
     h && j();
     const X = vb(),
-        C = async (R, ce) => {
-            let Se = new File(R, "audio.wav");
+        C = async (B, ce) => {
+            let Se = new File(B, "audio.wav");
             const wt = await Ba([Se], ce === "stream");
-            let Y = (await Lb([
+            let Q = (await Lb([
                 await Ra(wt, a, void 0, w),
                 "optionalAccess",
                 async (yt) => yt.filter,
                     "call",
                     async (yt) => yt(Boolean)
             ]))[0];
-            r === null ? n(1, r = new Cs(Y)) : n(1, r.file_data = Y, r), X(ce, r);
+            r === null ? n(1, r = new Cs(Q)) : n(1, r.file_data = Q, r), X(ce, r);
         };
     bb(() => {
         h && E && E.state !== "inactive" && E.stop();
     });
     async function G() {
-        let R;
+        let B;
         try {
-            R = await navigator.mediaDevices.getUserMedia({
+            B = await navigator.mediaDevices.getUserMedia({
                 audio: !0
             });
         } catch (ce) {
             if (!navigator.mediaDevices) {
                 X("error", d("audio.no_device_support"));
                 return;
             }
             if (ce instanceof DOMException && ce.name == "NotAllowedError") {
                 X("error", d("audio.allow_recording_access"));
                 return;
             }
             throw ce;
         }
-        if (R != null) {
+        if (B != null) {
             if (h) {
                 const [{
                     MediaRecorder: ce,
                     register: Se
                 }, {
                     connect: wt
-                }] = await Promise.all(x);
-                await Se(await wt()), E = new ce(R, {
+                }] = await Promise.all(Z);
+                await Se(await wt()), E = new ce(B, {
                     mimeType: "audio/wav"
-                }), E.addEventListener("dataavailable", I);
+                }), E.addEventListener("dataavailable", N);
             } else
-                E = new MediaRecorder(R), E.addEventListener("dataavailable", (ce) => {
-                    Z.push(ce.data);
+                E = new MediaRecorder(B), E.addEventListener("dataavailable", (ce) => {
+                    J.push(ce.data);
                 }), E.addEventListener("stop", async () => {
-                    n(13, k = !1), await C(Z, "change"), await C(Z, "stop_recording"), Z = [];
+                    n(13, k = !1), await C(J, "change"), await C(J, "stop_recording"), J = [];
                 });
-            M = !0;
+            D = !0;
         }
     }
-    async function I(R) {
-        let ce = await R.data.arrayBuffer(),
+    async function N(B) {
+        let ce = await B.data.arrayBuffer(),
             Se = new Uint8Array(ce);
         if (H || (n(22, H = new Uint8Array(ce.slice(0, aa))), Se = new Uint8Array(ce.slice(aa))), f)
             L.push(Se);
         else {
             let wt = [H].concat(L, [Se]);
             C(wt, "stream"), n(23, L = []);
         }
     }
     async function U() {
-        n(13, k = !0), X("start_recording"), M || await G(), n(22, H = void 0), h && E.start(Pb);
+        n(13, k = !0), X("start_recording"), D || await G(), n(22, H = void 0), h && E.start(Pb);
     }
 
-    function K() {
+    function $() {
         X("change", null), X("clear"), n(14, y = ""), n(1, r = null);
     }
 
     function O({
-        detail: R
+        detail: B
     }) {
-        n(1, r = new Cs(R)), X("change", r), X("upload", R);
+        n(1, r = new Cs(B)), X("change", r), X("upload", B);
     }
 
-    function J() {
-        n(13, k = !1), h && (X("stop_recording"), E.stop(), f && n(24, P = !0), C(Z, "stop_recording"), X("clear"), n(14, y = ""));
+    function Y() {
+        n(13, k = !1), h && (X("stop_recording"), E.stop(), f && n(24, P = !0), C(J, "stop_recording"), X("clear"), n(14, y = ""));
     }
 
-    function le(R) {
-        y = R, n(14, y);
+    function se(B) {
+        y = B, n(14, y);
     }
 
-    function p(R) {
-        v = R, n(0, v);
+    function p(B) {
+        b = B, n(0, b);
     }
-    const A = ({
-            detail: R
-        }) => X("error", R),
+    const T = ({
+            detail: B
+        }) => X("error", B),
         q = () => n(14, y = "edit");
 
-    function z(R) {
-        y = R, n(14, y);
+    function z(B) {
+        y = B, n(14, y);
     }
 
-    function he(R) {
-        Tr.call(this, t, R);
+    function he(B) {
+        Tr.call(this, t, B);
     }
 
-    function _e(R) {
-        Tr.call(this, t, R);
+    function _e(B) {
+        Tr.call(this, t, B);
     }
 
-    function F(R) {
-        Tr.call(this, t, R);
+    function F(B) {
+        Tr.call(this, t, B);
     }
-    const ve = (R) => X("edit", R.detail);
+    const ve = (B) => X("edit", B.detail);
 
-    function B(R) {
-        b = R, n(2, b);
+    function M(B) {
+        g = B, n(2, g);
     }
-    return t.$$set = (R) => {
-        "value" in R && n(1, r = R.value), "label" in R && n(3, s = R.label), "root" in R && n(4, a = R.root), "show_label" in R && n(5, l = R.show_label), "show_download_button" in R && n(6, u = R.show_download_button), "sources" in R && n(7, c = R.sources), "pending" in R && n(21, f = R.pending), "streaming" in R && n(8, h = R.streaming), "i18n" in R && n(9, d = R.i18n), "waveform_settings" in R && n(10, _ = R.waveform_settings), "waveform_options" in R && n(11, m = R.waveform_options), "dragging" in R && n(0, v = R.dragging), "active_source" in R && n(2, b = R.active_source), "editable" in R && n(12, S = R.editable), "$$scope" in R && n(36, o = R.$$scope);
+    return t.$$set = (B) => {
+        "value" in B && n(1, r = B.value), "label" in B && n(3, s = B.label), "root" in B && n(4, a = B.root), "show_label" in B && n(5, l = B.show_label), "show_download_button" in B && n(6, u = B.show_download_button), "sources" in B && n(7, c = B.sources), "pending" in B && n(21, f = B.pending), "streaming" in B && n(8, h = B.streaming), "i18n" in B && n(9, d = B.i18n), "waveform_settings" in B && n(10, _ = B.waveform_settings), "waveform_options" in B && n(11, m = B.waveform_options), "dragging" in B && n(0, b = B.dragging), "active_source" in B && n(2, g = B.active_source), "editable" in B && n(12, S = B.editable), "$$scope" in B && n(36, o = B.$$scope);
     }, t.$$.update = () => {
         if (t.$$.dirty[0] & /*dragging*/
-            1 && X("drag", v), t.$$.dirty[0] & /*submit_pending_stream_on_pending_end, pending, header, pending_stream*/
+            1 && X("drag", b), t.$$.dirty[0] & /*submit_pending_stream_on_pending_end, pending, header, pending_stream*/
             31457280 && P && f === !1 && (n(24, P = !1), H && L)) {
-            let R = [H].concat(L);
-            n(23, L = []), C(R, "stream");
+            let B = [H].concat(L);
+            n(23, L = []), C(B, "stream");
         }
     }, [
-        v,
-        r,
         b,
+        r,
+        g,
         s,
         a,
         l,
         u,
         c,
         h,
         d,
@@ -14799,32 +14799,32 @@
         m,
         S,
         k,
         y,
         X,
         C,
         U,
-        K,
+        $,
         O,
-        J,
+        Y,
         f,
         H,
         L,
         P,
         i,
-        le,
+        se,
         p,
-        A,
+        T,
         q,
         z,
         he,
         _e,
         F,
         ve,
-        B,
+        M,
         o
     ];
 }
 class Bb extends cb {
     constructor(e) {
         super(), _b(
             this,
@@ -14849,26 +14849,26 @@
             },
             null,
             [-1, -1]
         );
     }
 }
 
-function Hn(t) {
+function On(t) {
     let e = ["", "k", "M", "G", "T", "P", "E", "Z"],
         n = 0;
     for (; t > 1e3 && n < e.length - 1;)
         t /= 1e3, n++;
     let i = e[n];
     return (Number.isInteger(t) ? t : t.toFixed(1)) + i;
 }
 const {
     SvelteComponent: Mb,
     append: it,
-    attr: ee,
+    attr: ne,
     component_subscribe: ua,
     detach: Db,
     element: Hb,
     init: Ob,
     insert: Nb,
     noop: ca,
     safe_not_equal: Ib,
@@ -14879,19 +14879,19 @@
     onMount: Ub
 } = window.__gradio__svelte__internal;
 
 function jb(t) {
     let e, n, i, o, r, s, a, l, u, c, f, h;
     return {
         c() {
-            e = Hb("div"), n = ot("svg"), i = ot("g"), o = ot("path"), r = ot("path"), s = ot("path"), a = ot("path"), l = ot("g"), u = ot("path"), c = ot("path"), f = ot("path"), h = ot("path"), ee(o, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), ee(o, "fill", "#FF7C00"), ee(o, "fill-opacity", "0.4"), ee(o, "class", "svelte-43sxxs"), ee(r, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), ee(r, "fill", "#FF7C00"), ee(r, "class", "svelte-43sxxs"), ee(s, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), ee(s, "fill", "#FF7C00"), ee(s, "fill-opacity", "0.4"), ee(s, "class", "svelte-43sxxs"), ee(a, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), ee(a, "fill", "#FF7C00"), ee(a, "class", "svelte-43sxxs"), Ji(i, "transform", "translate(" + /*$top*/
+            e = Hb("div"), n = ot("svg"), i = ot("g"), o = ot("path"), r = ot("path"), s = ot("path"), a = ot("path"), l = ot("g"), u = ot("path"), c = ot("path"), f = ot("path"), h = ot("path"), ne(o, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), ne(o, "fill", "#FF7C00"), ne(o, "fill-opacity", "0.4"), ne(o, "class", "svelte-43sxxs"), ne(r, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), ne(r, "fill", "#FF7C00"), ne(r, "class", "svelte-43sxxs"), ne(s, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), ne(s, "fill", "#FF7C00"), ne(s, "fill-opacity", "0.4"), ne(s, "class", "svelte-43sxxs"), ne(a, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), ne(a, "fill", "#FF7C00"), ne(a, "class", "svelte-43sxxs"), Ji(i, "transform", "translate(" + /*$top*/
                 t[1][0] + "px, " + /*$top*/
-                t[1][1] + "px)"), ee(u, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), ee(u, "fill", "#FF7C00"), ee(u, "fill-opacity", "0.4"), ee(u, "class", "svelte-43sxxs"), ee(c, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), ee(c, "fill", "#FF7C00"), ee(c, "class", "svelte-43sxxs"), ee(f, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), ee(f, "fill", "#FF7C00"), ee(f, "fill-opacity", "0.4"), ee(f, "class", "svelte-43sxxs"), ee(h, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), ee(h, "fill", "#FF7C00"), ee(h, "class", "svelte-43sxxs"), Ji(l, "transform", "translate(" + /*$bottom*/
+                t[1][1] + "px)"), ne(u, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), ne(u, "fill", "#FF7C00"), ne(u, "fill-opacity", "0.4"), ne(u, "class", "svelte-43sxxs"), ne(c, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), ne(c, "fill", "#FF7C00"), ne(c, "class", "svelte-43sxxs"), ne(f, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), ne(f, "fill", "#FF7C00"), ne(f, "fill-opacity", "0.4"), ne(f, "class", "svelte-43sxxs"), ne(h, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), ne(h, "fill", "#FF7C00"), ne(h, "class", "svelte-43sxxs"), Ji(l, "transform", "translate(" + /*$bottom*/
                 t[2][0] + "px, " + /*$bottom*/
-                t[2][1] + "px)"), ee(n, "viewBox", "-1200 -1200 3000 3000"), ee(n, "fill", "none"), ee(n, "xmlns", "http://www.w3.org/2000/svg"), ee(n, "class", "svelte-43sxxs"), ee(e, "class", "svelte-43sxxs"), fa(
+                t[2][1] + "px)"), ne(n, "viewBox", "-1200 -1200 3000 3000"), ne(n, "fill", "none"), ne(n, "xmlns", "http://www.w3.org/2000/svg"), ne(n, "class", "svelte-43sxxs"), ne(e, "class", "svelte-43sxxs"), fa(
                 e,
                 "margin",
                 /*margin*/
                 t[0]
             );
         },
         m(d, _) {
@@ -14950,56 +14950,56 @@
     }
 }
 const {
     SvelteComponent: zb,
     append: rn,
     attr: gt,
     binding_callbacks: da,
-    check_outros: hc,
+    check_outros: mc,
     create_component: Gb,
     create_slot: Wb,
     destroy_component: Vb,
-    destroy_each: _c,
+    destroy_each: pc,
     detach: W,
     element: St,
-    empty: $n,
+    empty: ei,
     ensure_array_like: ho,
     get_all_dirty_from_scope: Xb,
     get_slot_changes: xb,
-    group_outros: mc,
+    group_outros: gc,
     init: Zb,
     insert: V,
     mount_component: Jb,
     noop: ts,
     safe_not_equal: Yb,
     set_data: $e,
     set_style: It,
     space: bt,
     text: de,
     toggle_class: Qe,
-    transition_in: Wn,
-    transition_out: Vn,
+    transition_in: Vn,
+    transition_out: Xn,
     update_slot_base: Qb
 } = window.__gradio__svelte__internal, {
     tick: Kb
 } = window.__gradio__svelte__internal, {
     onDestroy: $b
-} = window.__gradio__svelte__internal, ev = (t) => ({}), ha = (t) => ({});
+} = window.__gradio__svelte__internal, e2 = (t) => ({}), ha = (t) => ({});
 
 function _a(t, e, n) {
     const i = t.slice();
     return i[38] = e[n], i[40] = n, i;
 }
 
 function ma(t, e, n) {
     const i = t.slice();
     return i[38] = e[n], i;
 }
 
-function tv(t) {
+function t2(t) {
     let e, n = (
             /*i18n*/
             t[1]("common.error") + ""
         ),
         i, o, r;
     const s = (
             /*#slots*/
@@ -15030,98 +15030,98 @@
                 /*$$scope*/
                 l[28],
                 r ? xb(
                     s,
                     /*$$scope*/
                     l[28],
                     u,
-                    ev
+                    e2
                 ) : Xb(
                     /*$$scope*/
                     l[28]
                 ),
                 ha
             );
         },
         i(l) {
-            r || (Wn(a, l), r = !0);
+            r || (Vn(a, l), r = !0);
         },
         o(l) {
-            Vn(a, l), r = !1;
+            Xn(a, l), r = !1;
         },
         d(l) {
             l && (W(e), W(o)), a && a.d(l);
         }
     };
 }
 
-function nv(t) {
+function n2(t) {
     let e, n, i, o, r, s, a, l, u, c = (
         /*variant*/
         t[8] === "default" && /*show_eta_bar*/
         t[18] && /*show_progress*/
         t[6] === "full" && pa(t)
     );
 
     function f(w, k) {
         if (
             /*progress*/
             w[7]
         )
-            return rv;
+            return r2;
         if (
             /*queue_position*/
             w[2] !== null && /*queue_size*/
             w[3] !== void 0 && /*queue_position*/
             w[2] >= 0
         )
-            return ov;
+            return o2;
         if (
             /*queue_position*/
             w[2] === 0
         )
-            return iv;
+            return i2;
     }
     let h = f(t),
         d = h && h(t),
         _ = (
             /*timer*/
             t[5] && va(t)
         );
-    const m = [uv, av],
-        v = [];
+    const m = [u2, a2],
+        b = [];
 
-    function b(w, k) {
+    function g(w, k) {
         return (
             /*last_progress_level*/
             w[15] != null ? 0 : (
                 /*show_progress*/
                 w[6] === "full" ? 1 : -1
             )
         );
     }
-    ~(r = b(t)) && (s = v[r] = m[r](t));
+    ~(r = g(t)) && (s = b[r] = m[r](t));
     let S = ! /*timer*/
         t[5] && Aa(t);
     return {
         c() {
-            c && c.c(), e = bt(), n = St("div"), d && d.c(), i = bt(), _ && _.c(), o = bt(), s && s.c(), a = bt(), S && S.c(), l = $n(), gt(n, "class", "progress-text svelte-1yserjw"), Qe(
+            c && c.c(), e = bt(), n = St("div"), d && d.c(), i = bt(), _ && _.c(), o = bt(), s && s.c(), a = bt(), S && S.c(), l = ei(), gt(n, "class", "progress-text svelte-1yserjw"), Qe(
                 n,
                 "meta-text-center",
                 /*variant*/
                 t[8] === "center"
             ), Qe(
                 n,
                 "meta-text",
                 /*variant*/
                 t[8] === "default"
             );
         },
         m(w, k) {
-            c && c.m(w, k), V(w, e, k), V(w, n, k), d && d.m(n, null), rn(n, i), _ && _.m(n, null), V(w, o, k), ~r && v[r].m(w, k), V(w, a, k), S && S.m(w, k), V(w, l, k), u = !0;
+            c && c.m(w, k), V(w, e, k), V(w, n, k), d && d.m(n, null), rn(n, i), _ && _.m(n, null), V(w, o, k), ~r && b[r].m(w, k), V(w, a, k), S && S.m(w, k), V(w, l, k), u = !0;
         },
         p(w, k) {
             /*variant*/
             w[8] === "default" && /*show_eta_bar*/
                 w[18] && /*show_progress*/
                 w[6] === "full" ? c ? c.p(w, k) : (c = pa(w), c.c(), c.m(e.parentNode, e)) : c && (c.d(1), c = null), h === (h = f(w)) && d ? d.p(w, k) : (d && d.d(1), d = h && h(w), d && (d.c(), d.m(n, i))), /*timer*/
                 w[5] ? _ ? _.p(w, k) : (_ = va(w), _.c(), _.m(n, null)) : _ && (_.d(1), _ = null), (!u || k[0] & /*variant*/
@@ -15134,27 +15134,27 @@
                     256) && Qe(
                     n,
                     "meta-text",
                     /*variant*/
                     w[8] === "default"
                 );
             let E = r;
-            r = b(w), r === E ? ~r && v[r].p(w, k) : (s && (mc(), Vn(v[E], 1, 1, () => {
-                    v[E] = null;
-                }), hc()), ~r ? (s = v[r], s ? s.p(w, k) : (s = v[r] = m[r](w), s.c()), Wn(s, 1), s.m(a.parentNode, a)) : s = null), /*timer*/
+            r = g(w), r === E ? ~r && b[r].p(w, k) : (s && (gc(), Xn(b[E], 1, 1, () => {
+                    b[E] = null;
+                }), mc()), ~r ? (s = b[r], s ? s.p(w, k) : (s = b[r] = m[r](w), s.c()), Vn(s, 1), s.m(a.parentNode, a)) : s = null), /*timer*/
                 w[5] ? S && (S.d(1), S = null) : S ? S.p(w, k) : (S = Aa(w), S.c(), S.m(l.parentNode, l));
         },
         i(w) {
-            u || (Wn(s), u = !0);
+            u || (Vn(s), u = !0);
         },
         o(w) {
-            Vn(s), u = !1;
+            Xn(s), u = !1;
         },
         d(w) {
-            w && (W(e), W(n), W(o), W(a), W(l)), c && c.d(w), d && d.d(), _ && _.d(), ~r && v[r].d(w), S && S.d(w);
+            w && (W(e), W(n), W(o), W(a), W(l)), c && c.d(w), d && d.d(), _ && _.d(), ~r && b[r].d(w), S && S.d(w);
         }
     };
 }
 
 function pa(t) {
     let e, n = `translateX(${/*eta_level*/
   (t[17] || 0) * 100 - 100}%)`;
@@ -15172,15 +15172,15 @@
         },
         d(i) {
             i && W(e);
         }
     };
 }
 
-function iv(t) {
+function i2(t) {
     let e;
     return {
         c() {
             e = de("processing |");
         },
         m(n, i) {
             V(n, e, i);
@@ -15188,15 +15188,15 @@
         p: ts,
         d(n) {
             n && W(e);
         }
     };
 }
 
-function ov(t) {
+function o2(t) {
     let e, n = (
             /*queue_position*/
             t[2] + 1 + ""
         ),
         i, o, r, s;
     return {
         c() {
@@ -15220,27 +15220,27 @@
         },
         d(a) {
             a && (W(e), W(i), W(o), W(r), W(s));
         }
     };
 }
 
-function rv(t) {
+function r2(t) {
     let e, n = ho(
             /*progress*/
             t[7]
         ),
         i = [];
     for (let o = 0; o < n.length; o += 1)
         i[o] = ba(ma(t, n, o));
     return {
         c() {
             for (let o = 0; o < i.length; o += 1)
                 i[o].c();
-            e = $n();
+            e = ei();
         },
         m(o, r) {
             for (let s = 0; s < i.length; s += 1)
                 i[s] && i[s].m(o, r);
             V(o, e, r);
         },
         p(o, r) {
@@ -15257,15 +15257,15 @@
                 }
                 for (; s < i.length; s += 1)
                     i[s].d(1);
                 i.length = n.length;
             }
         },
         d(o) {
-            o && W(e), _c(i, o);
+            o && W(e), pc(i, o);
         }
     };
 }
 
 function ga(t) {
     let e, n = (
             /*p*/
@@ -15273,15 +15273,15 @@
         ),
         i, o, r = " ",
         s;
 
     function a(c, f) {
         return (
             /*p*/
-            c[38].length != null ? lv : sv
+            c[38].length != null ? l2 : s2
         );
     }
     let l = a(t),
         u = l(t);
     return {
         c() {
             u.c(), e = bt(), i = de(n), o = de(" | "), s = de(r);
@@ -15296,64 +15296,64 @@
         },
         d(c) {
             c && (W(e), W(i), W(o), W(s)), u.d(c);
         }
     };
 }
 
-function sv(t) {
-    let e = Hn(
+function s2(t) {
+    let e = On(
             /*p*/
             t[38].index || 0
         ) + "",
         n;
     return {
         c() {
             n = de(e);
         },
         m(i, o) {
             V(i, n, o);
         },
         p(i, o) {
             o[0] & /*progress*/
-                128 && e !== (e = Hn(
+                128 && e !== (e = On(
                     /*p*/
                     i[38].index || 0
                 ) + "") && $e(n, e);
         },
         d(i) {
             i && W(n);
         }
     };
 }
 
-function lv(t) {
-    let e = Hn(
+function l2(t) {
+    let e = On(
             /*p*/
             t[38].index || 0
         ) + "",
-        n, i, o = Hn(
+        n, i, o = On(
             /*p*/
             t[38].length
         ) + "",
         r;
     return {
         c() {
             n = de(e), i = de("/"), r = de(o);
         },
         m(s, a) {
             V(s, n, a), V(s, i, a), V(s, r, a);
         },
         p(s, a) {
             a[0] & /*progress*/
-                128 && e !== (e = Hn(
+                128 && e !== (e = On(
                     /*p*/
                     s[38].index || 0
                 ) + "") && $e(n, e), a[0] & /*progress*/
-                128 && o !== (o = Hn(
+                128 && o !== (o = On(
                     /*p*/
                     s[38].length
                 ) + "") && $e(r, o);
         },
         d(s) {
             s && (W(n), W(i), W(r));
         }
@@ -15363,15 +15363,15 @@
 function ba(t) {
     let e, n = (
         /*p*/
         t[38].index != null && ga(t)
     );
     return {
         c() {
-            n && n.c(), e = $n();
+            n && n.c(), e = ei();
         },
         m(i, o) {
             n && n.m(i, o), V(i, e, o);
         },
         p(i, o) {
             /*p*/
             i[38].index != null ? n ? n.p(i, o) : (n = ga(i), n.c(), n.m(e.parentNode, e)) : n && (n.d(1), n = null);
@@ -15412,15 +15412,15 @@
         },
         d(r) {
             r && (W(e), W(i), W(o));
         }
     };
 }
 
-function av(t) {
+function a2(t) {
     let e, n;
     return e = new qb({
         props: {
             margin: (
                 /*variant*/
                 t[8] === "default"
             )
@@ -15435,26 +15435,26 @@
         p(i, o) {
             const r = {};
             o[0] & /*variant*/
                 256 && (r.margin = /*variant*/
                     i[8] === "default"), e.$set(r);
         },
         i(i) {
-            n || (Wn(e.$$.fragment, i), n = !0);
+            n || (Vn(e.$$.fragment, i), n = !0);
         },
         o(i) {
-            Vn(e.$$.fragment, i), n = !1;
+            Xn(e.$$.fragment, i), n = !1;
         },
         d(i) {
             Vb(e, i);
         }
     };
 }
 
-function uv(t) {
+function u2(t) {
     let e, n, i, o, r, s = `${/*last_progress_level*/
   t[15] * 100}%`,
         a = (
             /*progress*/
             t[7] != null && wa(t)
         );
     return {
@@ -15486,15 +15486,15 @@
         i = [];
     for (let o = 0; o < n.length; o += 1)
         i[o] = Sa(_a(t, n, o));
     return {
         c() {
             for (let o = 0; o < i.length; o += 1)
                 i[o].c();
-            e = $n();
+            e = ei();
         },
         m(o, r) {
             for (let s = 0; s < i.length; s += 1)
                 i[s] && i[s].m(o, r);
             V(o, e, r);
         },
         p(o, r) {
@@ -15511,23 +15511,23 @@
                 }
                 for (; s < i.length; s += 1)
                     i[s].d(1);
                 i.length = n.length;
             }
         },
         d(o) {
-            o && W(e), _c(i, o);
+            o && W(e), pc(i, o);
         }
     };
 }
 
 function ya(t) {
     let e, n, i, o, r = (
             /*i*/
-            t[40] !== 0 && cv()
+            t[40] !== 0 && c2()
         ),
         s = (
             /*p*/
             t[38].desc != null && ka(t)
         ),
         a = (
             /*p*/
@@ -15540,15 +15540,15 @@
         ),
         l = (
             /*progress_level*/
             t[14] != null && Ca(t)
         );
     return {
         c() {
-            r && r.c(), e = bt(), s && s.c(), n = bt(), a && a.c(), i = bt(), l && l.c(), o = $n();
+            r && r.c(), e = bt(), s && s.c(), n = bt(), a && a.c(), i = bt(), l && l.c(), o = ei();
         },
         m(u, c) {
             r && r.m(u, c), V(u, e, c), s && s.m(u, c), V(u, n, c), a && a.m(u, c), V(u, i, c), l && l.m(u, c), V(u, o, c);
         },
         p(u, c) {
             /*p*/
             u[38].desc != null ? s ? s.p(u, c) : (s = ka(u), s.c(), s.m(n.parentNode, n)) : s && (s.d(1), s = null), /*p*/
@@ -15562,15 +15562,15 @@
         },
         d(u) {
             u && (W(e), W(n), W(i), W(o)), r && r.d(u), s && s.d(u), a && a.d(u), l && l.d(u);
         }
     };
 }
 
-function cv(t) {
+function c2(t) {
     let e;
     return {
         c() {
             e = de(" /");
         },
         m(n, i) {
             V(n, e, i);
@@ -15656,15 +15656,15 @@
             t[14][
                 /*i*/
                 t[40]
             ] != null) && ya(t)
     );
     return {
         c() {
-            n && n.c(), e = $n();
+            n && n.c(), e = ei();
         },
         m(i, o) {
             n && n.m(i, o), V(i, e, o);
         },
         p(i, o) {
             /*p*/
             i[38].desc != null || /*progress_level*/
@@ -15702,17 +15702,17 @@
         },
         d(i) {
             i && W(e);
         }
     };
 }
 
-function fv(t) {
+function f2(t) {
     let e, n, i, o, r;
-    const s = [nv, tv],
+    const s = [n2, t2],
         a = [];
 
     function l(u, c) {
         return (
             /*status*/
             u[4] === "pending" ? 0 : (
                 /*status*/
@@ -15759,17 +15759,17 @@
             );
         },
         m(u, c) {
             V(u, e, c), ~n && a[n].m(e, null), t[31](e), r = !0;
         },
         p(u, c) {
             let f = n;
-            n = l(u), n === f ? ~n && a[n].p(u, c) : (i && (mc(), Vn(a[f], 1, 1, () => {
+            n = l(u), n === f ? ~n && a[n].p(u, c) : (i && (gc(), Xn(a[f], 1, 1, () => {
                     a[f] = null;
-                }), hc()), ~n ? (i = a[n], i ? i.p(u, c) : (i = a[n] = s[n](u), i.c()), Wn(i, 1), i.m(e, null)) : i = null), (!r || c[0] & /*variant, show_progress*/
+                }), mc()), ~n ? (i = a[n], i ? i.p(u, c) : (i = a[n] = s[n](u), i.c()), Vn(i, 1), i.m(e, null)) : i = null), (!r || c[0] & /*variant, show_progress*/
                     320 && o !== (o = "wrap " + /*variant*/
                         u[8] + " " + /*show_progress*/
                         u[6] + " svelte-1yserjw")) && gt(e, "class", o), (!r || c[0] & /*variant, show_progress, status, show_progress*/
                     336) && Qe(e, "hide", ! /*status*/
                     u[4] || /*status*/
                     u[4] === "complete" || /*show_progress*/
                     u[6] === "hidden"), (!r || c[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
@@ -15805,27 +15805,27 @@
                     e,
                     "padding",
                     /*absolute*/
                     u[10] ? "0" : "var(--size-8) 0"
                 );
         },
         i(u) {
-            r || (Wn(i), r = !0);
+            r || (Vn(i), r = !0);
         },
         o(u) {
-            Vn(i), r = !1;
+            Xn(i), r = !1;
         },
         d(u) {
             u && W(e), ~n && a[n].d(), t[31](null);
         }
     };
 }
 let Yi = [],
     Pr = !1;
-async function dv(t, e = !0) {
+async function d2(t, e = !0) {
     if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && e !== !0)) {
         if (Yi.push(t), !Pr)
             Pr = !0;
         else
             return;
         await Kb(), requestAnimationFrame(() => {
             let n = [0, 0];
@@ -15837,15 +15837,15 @@
                 top: n[0] - 20,
                 behavior: "smooth"
             }), Pr = !1, Yi = [];
         });
     }
 }
 
-function hv(t, e, n) {
+function h2(t, e, n) {
     let i, {
             $$slots: o = {},
             $$scope: r
         } = e,
         {
             i18n: s
         } = e,
@@ -15873,18 +15873,18 @@
         {
             message: _ = null
         } = e,
         {
             progress: m = null
         } = e,
         {
-            variant: v = "default"
+            variant: b = "default"
         } = e,
         {
-            loading_text: b = "Loading..."
+            loading_text: g = "Loading..."
         } = e,
         {
             absolute: S = !0
         } = e,
         {
             translucent: w = !1
         } = e,
@@ -15893,108 +15893,108 @@
         } = e,
         {
             autoscroll: E
         } = e,
         y, H = !1,
         L = 0,
         P = 0,
-        M = null,
-        Z = null,
-        x = 0,
+        D = null,
+        J = null,
+        Z = 0,
         j = null,
         X, C = null,
         G = !0;
-    const I = () => {
-        n(0, a = n(26, M = n(19, O = null))), n(24, L = performance.now()), n(25, P = 0), H = !0, U();
+    const N = () => {
+        n(0, a = n(26, D = n(19, O = null))), n(24, L = performance.now()), n(25, P = 0), H = !0, U();
     };
 
     function U() {
         requestAnimationFrame(() => {
             n(25, P = (performance.now() - L) / 1e3), H && U();
         });
     }
 
-    function K() {
-        n(25, P = 0), n(0, a = n(26, M = n(19, O = null))), H && (H = !1);
+    function $() {
+        n(25, P = 0), n(0, a = n(26, D = n(19, O = null))), H && (H = !1);
     }
     $b(() => {
-        H && K();
+        H && $();
     });
     let O = null;
 
-    function J(p) {
+    function Y(p) {
         da[p ? "unshift" : "push"](() => {
             C = p, n(16, C), n(7, m), n(14, j), n(15, X);
         });
     }
 
-    function le(p) {
+    function se(p) {
         da[p ? "unshift" : "push"](() => {
             y = p, n(13, y);
         });
     }
     return t.$$set = (p) => {
-        "i18n" in p && n(1, s = p.i18n), "eta" in p && n(0, a = p.eta), "queue_position" in p && n(2, l = p.queue_position), "queue_size" in p && n(3, u = p.queue_size), "status" in p && n(4, c = p.status), "scroll_to_output" in p && n(21, f = p.scroll_to_output), "timer" in p && n(5, h = p.timer), "show_progress" in p && n(6, d = p.show_progress), "message" in p && n(22, _ = p.message), "progress" in p && n(7, m = p.progress), "variant" in p && n(8, v = p.variant), "loading_text" in p && n(9, b = p.loading_text), "absolute" in p && n(10, S = p.absolute), "translucent" in p && n(11, w = p.translucent), "border" in p && n(12, k = p.border), "autoscroll" in p && n(23, E = p.autoscroll), "$$scope" in p && n(28, r = p.$$scope);
+        "i18n" in p && n(1, s = p.i18n), "eta" in p && n(0, a = p.eta), "queue_position" in p && n(2, l = p.queue_position), "queue_size" in p && n(3, u = p.queue_size), "status" in p && n(4, c = p.status), "scroll_to_output" in p && n(21, f = p.scroll_to_output), "timer" in p && n(5, h = p.timer), "show_progress" in p && n(6, d = p.show_progress), "message" in p && n(22, _ = p.message), "progress" in p && n(7, m = p.progress), "variant" in p && n(8, b = p.variant), "loading_text" in p && n(9, g = p.loading_text), "absolute" in p && n(10, S = p.absolute), "translucent" in p && n(11, w = p.translucent), "border" in p && n(12, k = p.border), "autoscroll" in p && n(23, E = p.autoscroll), "$$scope" in p && n(28, r = p.$$scope);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
-            218103809 && (a === null && n(0, a = M), a != null && M !== a && (n(27, Z = (performance.now() - L) / 1e3 + a), n(19, O = Z.toFixed(1)), n(26, M = a))), t.$$.dirty[0] & /*eta_from_start, timer_diff*/
-            167772160 && n(17, x = Z === null || Z <= 0 || !P ? null : Math.min(P / Z, 1)), t.$$.dirty[0] & /*progress*/
+            218103809 && (a === null && n(0, a = D), a != null && D !== a && (n(27, J = (performance.now() - L) / 1e3 + a), n(19, O = J.toFixed(1)), n(26, D = a))), t.$$.dirty[0] & /*eta_from_start, timer_diff*/
+            167772160 && n(17, Z = J === null || J <= 0 || !P ? null : Math.min(P / J, 1)), t.$$.dirty[0] & /*progress*/
             128 && m != null && n(18, G = !1), t.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
             114816 && (m != null ? n(14, j = m.map((p) => {
                 if (p.index != null && p.length != null)
                     return p.index / p.length;
                 if (p.progress != null)
                     return p.progress;
             })) : n(14, j = null), j ? (n(15, X = j[j.length - 1]), C && (X === 0 ? n(16, C.style.transition = "0", C) : n(16, C.style.transition = "150ms", C))) : n(15, X = void 0)), t.$$.dirty[0] & /*status*/
-            16 && (c === "pending" ? I() : K()), t.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
-            10493968 && y && f && (c === "pending" || c === "complete") && dv(y, E), t.$$.dirty[0] & /*status, message*/
+            16 && (c === "pending" ? N() : $()), t.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
+            10493968 && y && f && (c === "pending" || c === "complete") && d2(y, E), t.$$.dirty[0] & /*status, message*/
             4194320, t.$$.dirty[0] & /*timer_diff*/
             33554432 && n(20, i = P.toFixed(1));
     }, [
         a,
         s,
         l,
         u,
         c,
         h,
         d,
         m,
-        v,
         b,
+        g,
         S,
         w,
         k,
         y,
         j,
         X,
         C,
-        x,
+        Z,
         G,
         O,
         i,
         f,
         _,
         E,
         L,
         P,
-        M,
-        Z,
+        D,
+        J,
         r,
         o,
-        J,
-        le
+        Y,
+        se
     ];
 }
-class pc extends zb {
+class bc extends zb {
     constructor(e) {
         super(), Zb(
             this,
             e,
-            hv,
-            fv,
+            h2,
+            f2,
             Yb, {
                 i18n: 1,
                 eta: 0,
                 queue_position: 2,
                 queue_size: 3,
                 status: 4,
                 scroll_to_output: 21,
@@ -16011,38 +16011,38 @@
             },
             null,
             [-1, -1]
         );
     }
 }
 const {
-    SvelteComponent: _v,
-    add_flush_callback: mv,
-    assign: gc,
-    bind: pv,
-    binding_callbacks: gv,
-    check_outros: bv,
+    SvelteComponent: _2,
+    add_flush_callback: m2,
+    assign: vc,
+    bind: p2,
+    binding_callbacks: g2,
+    check_outros: b2,
     create_component: pn,
     destroy_component: gn,
     detach: ps,
-    empty: vv,
+    empty: v2,
     flush: ge,
-    get_spread_object: bc,
-    get_spread_update: vc,
-    group_outros: wv,
-    init: yv,
+    get_spread_object: wc,
+    get_spread_update: yc,
+    group_outros: w2,
+    init: y2,
     insert: gs,
     mount_component: bn,
-    safe_not_equal: kv,
-    space: wc,
+    safe_not_equal: k2,
+    space: kc,
     transition_in: Tt,
     transition_out: Pt
 } = window.__gradio__svelte__internal;
 
-function Ev(t) {
+function E2(t) {
     let e, n;
     return e = new Na({
         props: {
             variant: (
                 /*value*/
                 t[0] === null && /*active_source*/
                 t[19] === "upload" ? "dashed" : "solid"
@@ -16073,15 +16073,15 @@
                 t[12]
             ),
             min_width: (
                 /*min_width*/
                 t[13]
             ),
             $$slots: {
-                default: [Av]
+                default: [A2]
             },
             $$scope: {
                 ctx: t
             }
         }
     }), {
         c() {
@@ -16124,15 +16124,15 @@
         },
         d(i) {
             gn(e, i);
         }
     };
 }
 
-function Cv(t) {
+function C2(t) {
     let e, n;
     return e = new Na({
         props: {
             variant: "solid",
             border_mode: (
                 /*dragging*/
                 t[20] ? "focus" : "base"
@@ -16159,15 +16159,15 @@
                 t[12]
             ),
             min_width: (
                 /*min_width*/
                 t[13]
             ),
             $$slots: {
-                default: [Tv]
+                default: [T2]
             },
             $$scope: {
                 ctx: t
             }
         }
     }), {
         c() {
@@ -16207,17 +16207,17 @@
         },
         d(i) {
             gn(e, i);
         }
     };
 }
 
-function Sv(t) {
+function S2(t) {
     let e, n;
-    return e = new __({
+    return e = new p_({
         props: {
             i18n: (
                 /*gradio*/
                 t[18].i18n
             ),
             type: "audio"
         }
@@ -16242,15 +16242,15 @@
         },
         d(i) {
             gn(e, i);
         }
     };
 }
 
-function Av(t) {
+function A2(t) {
     let e, n, i, o, r;
     const s = [{
             autoscroll: (
                 /*gradio*/
                 t[18].autoscroll
             )
         }, {
@@ -16260,16 +16260,16 @@
             )
         },
         /*loading_status*/
         t[1]
     ];
     let a = {};
     for (let c = 0; c < s.length; c += 1)
-        a = gc(a, s[c]);
-    e = new pc({
+        a = vc(a, s[c]);
+    e = new bc({
         props: a
     });
 
     function l(c) {
         t[31](c);
     }
     let u = {
@@ -16322,26 +16322,26 @@
             t[21]
         ),
         waveform_options: (
             /*waveform_options*/
             t[15]
         ),
         $$slots: {
-            default: [Sv]
+            default: [S2]
         },
         $$scope: {
             ctx: t
         }
     };
     return (
         /*dragging*/
         t[20] !== void 0 && (u.dragging = /*dragging*/
             t[20]), i = new Bb({
             props: u
-        }), gv.push(() => pv(i, "dragging", l)), i.$on(
+        }), g2.push(() => p2(i, "dragging", l)), i.$on(
             "change",
             /*change_handler*/
             t[32]
         ), i.$on(
             "stream",
             /*stream_handler*/
             t[33]
@@ -16387,22 +16387,22 @@
             t[43]
         ), i.$on(
             "error",
             /*handle_error*/
             t[22]
         ), {
             c() {
-                pn(e.$$.fragment), n = wc(), pn(i.$$.fragment);
+                pn(e.$$.fragment), n = kc(), pn(i.$$.fragment);
             },
             m(c, f) {
                 bn(e, c, f), gs(c, n, f), bn(i, c, f), r = !0;
             },
             p(c, f) {
                 const h = f[0] & /*gradio, loading_status*/
-                    262146 ? vc(s, [
+                    262146 ? yc(s, [
                         f[0] & /*gradio*/
                         262144 && {
                             autoscroll: (
                                 /*gradio*/
                                 c[18].autoscroll
                             )
                         },
@@ -16410,15 +16410,15 @@
                         262144 && {
                             i18n: (
                                 /*gradio*/
                                 c[18].i18n
                             )
                         },
                         f[0] & /*loading_status*/
-                        2 && bc(
+                        2 && wc(
                             /*loading_status*/
                             c[1]
                         )
                     ]) : {};
                 e.$set(h);
                 const d = {};
                 f[0] & /*label*/
@@ -16450,30 +16450,30 @@
                         c[15]), f[0] & /*gradio*/
                     262144 | f[1] & /*$$scope*/
                     16384 && (d.$$scope = {
                         dirty: f,
                         ctx: c
                     }), !o && f[0] & /*dragging*/
                     1048576 && (o = !0, d.dragging = /*dragging*/
-                        c[20], mv(() => o = !1)), i.$set(d);
+                        c[20], m2(() => o = !1)), i.$set(d);
             },
             i(c) {
                 r || (Tt(e.$$.fragment, c), Tt(i.$$.fragment, c), r = !0);
             },
             o(c) {
                 Pt(e.$$.fragment, c), Pt(i.$$.fragment, c), r = !1;
             },
             d(c) {
                 c && ps(n), gn(e, c), gn(i, c);
             }
         }
     );
 }
 
-function Tv(t) {
+function T2(t) {
     let e, n, i, o;
     const r = [{
             autoscroll: (
                 /*gradio*/
                 t[18].autoscroll
             )
         }, {
@@ -16483,16 +16483,16 @@
             )
         },
         /*loading_status*/
         t[1]
     ];
     let s = {};
     for (let a = 0; a < r.length; a += 1)
-        s = gc(s, r[a]);
-    return e = new pc({
+        s = vc(s, r[a]);
+    return e = new bc({
         props: s
     }), i = new Gm({
         props: {
             i18n: (
                 /*gradio*/
                 t[18].i18n
             ),
@@ -16539,22 +16539,22 @@
         t[29]
     ), i.$on(
         "stop",
         /*stop_handler*/
         t[30]
     ), {
         c() {
-            pn(e.$$.fragment), n = wc(), pn(i.$$.fragment);
+            pn(e.$$.fragment), n = kc(), pn(i.$$.fragment);
         },
         m(a, l) {
             bn(e, a, l), gs(a, n, l), bn(i, a, l), o = !0;
         },
         p(a, l) {
             const u = l[0] & /*gradio, loading_status*/
-                262146 ? vc(r, [
+                262146 ? yc(r, [
                     l[0] & /*gradio*/
                     262144 && {
                         autoscroll: (
                             /*gradio*/
                             a[18].autoscroll
                         )
                     },
@@ -16562,15 +16562,15 @@
                     262144 && {
                         i18n: (
                             /*gradio*/
                             a[18].i18n
                         )
                     },
                     l[0] & /*loading_status*/
-                    2 && bc(
+                    2 && wc(
                         /*loading_status*/
                         a[1]
                     )
                 ]) : {};
             e.$set(u);
             const c = {};
             l[0] & /*gradio*/
@@ -16597,51 +16597,51 @@
         },
         d(a) {
             a && ps(n), gn(e, a), gn(i, a);
         }
     };
 }
 
-function Pv(t) {
+function P2(t) {
     let e, n, i, o;
-    const r = [Cv, Ev],
+    const r = [C2, E2],
         s = [];
 
     function a(l, u) {
         return (
             /*interactive*/
             l[5] ? 1 : 0
         );
     }
     return e = a(t), n = s[e] = r[e](t), {
         c() {
-            n.c(), i = vv();
+            n.c(), i = v2();
         },
         m(l, u) {
             s[e].m(l, u), gs(l, i, u), o = !0;
         },
         p(l, u) {
             let c = e;
-            e = a(l), e === c ? s[e].p(l, u) : (wv(), Pt(s[c], 1, 1, () => {
+            e = a(l), e === c ? s[e].p(l, u) : (w2(), Pt(s[c], 1, 1, () => {
                 s[c] = null;
-            }), bv(), n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), Tt(n, 1), n.m(i.parentNode, i));
+            }), b2(), n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), Tt(n, 1), n.m(i.parentNode, i));
         },
         i(l) {
             o || (Tt(n), o = !0);
         },
         o(l) {
             Pt(n), o = !1;
         },
         d(l) {
             l && ps(i), s[e].d(l);
         }
     };
 }
 
-function Lv(t, e, n) {
+function L2(t, e, n) {
     let {
         elem_id: i = ""
     } = e, {
         elem_classes: o = []
     } = e, {
         visible: r = !0
     } = e, {
@@ -16661,89 +16661,89 @@
     } = e, {
         container: d = !0
     } = e, {
         scale: _ = null
     } = e, {
         min_width: m = void 0
     } = e, {
-        loading_status: v
+        loading_status: b
     } = e, {
-        autoplay: b = !1
+        autoplay: g = !1
     } = e, {
         editable: S = !0
     } = e, {
         waveform_options: w = {}
     } = e, {
         pending: k
     } = e, {
         streaming: E
     } = e, {
         gradio: y
-    } = e, H = null, L, P = a, M, Z;
+    } = e, H = null, L, P = a, D, J;
 
-    function x({
-        detail: B
+    function Z({
+        detail: M
     }) {
-        const [R, ce] = B.includes("Invalid file type") ? ["warning", "complete"] : ["error", "error"];
-        n(1, v = v || {}), n(1, v.status = ce, v), n(1, v.message = B, v), y.dispatch(R, B);
+        const [B, ce] = M.includes("Invalid file type") ? ["warning", "complete"] : ["error", "error"];
+        n(1, b = b || {}), n(1, b.status = ce, b), n(1, b.message = M, b), y.dispatch(B, M);
     }
-    const j = (B) => y.dispatch("share", B.detail),
-        X = (B) => y.dispatch("error", B.detail),
+    const j = (M) => y.dispatch("share", M.detail),
+        X = (M) => y.dispatch("error", M.detail),
         C = () => y.dispatch("play"),
         G = () => y.dispatch("pause"),
-        I = () => y.dispatch("stop");
+        N = () => y.dispatch("stop");
 
-    function U(B) {
-        M = B, n(20, M);
+    function U(M) {
+        D = M, n(20, D);
     }
-    const K = ({
-            detail: B
-        }) => n(0, a = B),
+    const $ = ({
+            detail: M
+        }) => n(0, a = M),
         O = ({
-            detail: B
+            detail: M
         }) => {
-            n(0, a = B), y.dispatch("stream", a);
+            n(0, a = M), y.dispatch("stream", a);
         },
-        J = ({
-            detail: B
-        }) => n(20, M = B),
-        le = (B) => y.dispatch("edit", B.detail),
+        Y = ({
+            detail: M
+        }) => n(20, D = M),
+        se = (M) => y.dispatch("edit", M.detail),
         p = () => y.dispatch("play"),
-        A = () => y.dispatch("pause"),
+        T = () => y.dispatch("pause"),
         q = () => y.dispatch("stop"),
         z = () => y.dispatch("start_recording"),
         he = () => y.dispatch("pause_recording"),
-        _e = (B) => y.dispatch("stop_recording", B.detail),
+        _e = (M) => y.dispatch("stop_recording", M.detail),
         F = () => y.dispatch("upload"),
         ve = () => y.dispatch("clear");
-    return t.$$set = (B) => {
-        "elem_id" in B && n(2, i = B.elem_id), "elem_classes" in B && n(3, o = B.elem_classes), "visible" in B && n(4, r = B.visible), "interactive" in B && n(5, s = B.interactive), "value" in B && n(0, a = B.value), "sources" in B && n(6, l = B.sources), "label" in B && n(7, u = B.label), "root" in B && n(8, c = B.root), "show_label" in B && n(9, f = B.show_label), "show_download_button" in B && n(10, h = B.show_download_button), "container" in B && n(11, d = B.container), "scale" in B && n(12, _ = B.scale), "min_width" in B && n(13, m = B.min_width), "loading_status" in B && n(1, v = B.loading_status), "autoplay" in B && n(23, b = B.autoplay), "editable" in B && n(14, S = B.editable), "waveform_options" in B && n(15, w = B.waveform_options), "pending" in B && n(16, k = B.pending), "streaming" in B && n(17, E = B.streaming), "gradio" in B && n(18, y = B.gradio);
+    return t.$$set = (M) => {
+        "elem_id" in M && n(2, i = M.elem_id), "elem_classes" in M && n(3, o = M.elem_classes), "visible" in M && n(4, r = M.visible), "interactive" in M && n(5, s = M.interactive), "value" in M && n(0, a = M.value), "sources" in M && n(6, l = M.sources), "label" in M && n(7, u = M.label), "root" in M && n(8, c = M.root), "show_label" in M && n(9, f = M.show_label), "show_download_button" in M && n(10, h = M.show_download_button), "container" in M && n(11, d = M.container), "scale" in M && n(12, _ = M.scale), "min_width" in M && n(13, m = M.min_width), "loading_status" in M && n(1, b = M.loading_status), "autoplay" in M && n(23, g = M.autoplay), "editable" in M && n(14, S = M.editable), "waveform_options" in M && n(15, w = M.waveform_options), "pending" in M && n(16, k = M.pending), "streaming" in M && n(17, E = M.streaming), "gradio" in M && n(18, y = M.gradio);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*value, initial_value*/
             33554433 && a && P === null && n(25, P = a), t.$$.dirty[0] & /*value, old_value, gradio*/
             17039361 && JSON.stringify(a) !== JSON.stringify(H) && (n(24, H = a), y.dispatch("change")), t.$$.dirty[0] & /*active_source, sources*/
             524352 && !L && l && n(19, L = l[0]), t.$$.dirty[0] & /*waveform_options, autoplay*/
-            8421376 && n(21, Z = {
+            8421376 && n(21, J = {
                 height: 50,
                 waveColor: w.waveform_color || "#9ca3af",
                 progressColor: w.waveform_progress_color || "#f97316",
                 barWidth: 2,
                 barGap: 3,
                 cursorWidth: 2,
                 cursorColor: "#ddd5e9",
-                autoplay: b,
+                autoplay: g,
                 barRadius: 10,
                 dragToSeek: !0,
                 normalize: !0,
                 minPxPerSec: 20,
                 mediaControls: w.show_controls
             });
     }, [
         a,
-        v,
+        b,
         i,
         o,
         r,
         s,
         l,
         u,
         c,
@@ -16754,48 +16754,48 @@
         m,
         S,
         w,
         k,
         E,
         y,
         L,
-        M,
+        D,
+        J,
         Z,
-        x,
-        b,
+        g,
         H,
         P,
         j,
         X,
         C,
         G,
-        I,
+        N,
         U,
-        K,
+        $,
         O,
-        J,
-        le,
+        Y,
+        se,
         p,
-        A,
+        T,
         q,
         z,
         he,
         _e,
         F,
         ve
     ];
 }
-class Qv extends _v {
+class Q2 extends _2 {
     constructor(e) {
-        super(), yv(
+        super(), y2(
             this,
             e,
-            Lv,
-            Pv,
-            kv, {
+            L2,
+            P2,
+            k2, {
                 elem_id: 2,
                 elem_classes: 3,
                 visible: 4,
                 interactive: 5,
                 value: 0,
                 sources: 6,
                 label: 7,
@@ -16975,36 +16975,36 @@
     set gradio(e) {
         this.$$set({
             gradio: e
         }), ge();
     }
 }
 const {
-    SvelteComponent: Rv,
-    append: Bv,
-    attr: Mv,
-    detach: Dv,
-    element: Hv,
-    init: Ov,
-    insert: Nv,
+    SvelteComponent: R2,
+    append: B2,
+    attr: M2,
+    detach: D2,
+    element: H2,
+    init: O2,
+    insert: N2,
     noop: Ta,
-    safe_not_equal: Iv,
-    set_data: Uv,
-    text: jv,
+    safe_not_equal: I2,
+    set_data: U2,
+    text: j2,
     toggle_class: Pn
 } = window.__gradio__svelte__internal;
 
-function Fv(t) {
+function F2(t) {
     let e, n;
     return {
         c() {
-            e = Hv("div"), n = jv(
+            e = H2("div"), n = j2(
                 /*value*/
                 t[0]
-            ), Mv(e, "class", "svelte-1gecy8w"), Pn(
+            ), M2(e, "class", "svelte-1gecy8w"), Pn(
                 e,
                 "table",
                 /*type*/
                 t[1] === "table"
             ), Pn(
                 e,
                 "gallery",
@@ -17014,19 +17014,19 @@
                 e,
                 "selected",
                 /*selected*/
                 t[2]
             );
         },
         m(i, o) {
-            Nv(i, e, o), Bv(e, n);
+            N2(i, e, o), B2(e, n);
         },
         p(i, [o]) {
             o & /*value*/
-                1 && Uv(
+                1 && U2(
                     n,
                     /*value*/
                     i[0]
                 ), o & /*type*/
                 2 && Pn(
                     e,
                     "table",
@@ -17045,41 +17045,41 @@
                     /*selected*/
                     i[2]
                 );
         },
         i: Ta,
         o: Ta,
         d(i) {
-            i && Dv(e);
+            i && D2(e);
         }
     };
 }
 
-function qv(t, e, n) {
+function q2(t, e, n) {
     let {
         value: i
     } = e, {
         type: o
     } = e, {
         selected: r = !1
     } = e;
     return t.$$set = (s) => {
         "value" in s && n(0, i = s.value), "type" in s && n(1, o = s.type), "selected" in s && n(2, r = s.selected);
     }, [i, o, r];
 }
-class Kv extends Rv {
+class K2 extends R2 {
     constructor(e) {
-        super(), Ov(this, e, qv, Fv, Iv, {
+        super(), O2(this, e, q2, F2, I2, {
             value: 0,
             type: 1,
             selected: 2
         });
     }
 }
 export {
-    Kv as BaseExample,
+    K2 as BaseExample,
     Bb as BaseInteractiveAudio,
-    _u as BasePlayer,
+    pu as BasePlayer,
     Gm as BaseStaticAudio,
-    Qv as
+    Q2 as
     default
 };
```

### Comparing `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-2c3384e6.js` & `gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/module-2c3384e6.js`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-aafe8b06.js` & `gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/module-aafe8b06.js`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-d82531d9.js` & `gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/module-d82531d9.js`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/style.css` & `gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-.block.svelte-nl1om8{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-nl1om8{border-color:var(--color-accent)}.block.border_contrast.svelte-nl1om8{border-color:var(--body-text-color)}.padded.svelte-nl1om8{padding:var(--block-padding)}.hidden.svelte-nl1om8{display:none}.hide-container.svelte-nl1om8{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-lpi64a{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-lpi64a{opacity:.5;box-shadow:none}button[disabled].svelte-lpi64a:hover{cursor:not-allowed}.padded.svelte-lpi64a{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-lpi64a:hover,button.highlight.svelte-lpi64a{cursor:pointer;color:var(--color-accent)}.padded.svelte-lpi64a:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-lpi64a{padding:0 1px;font-size:10px}div.svelte-lpi64a{padding:2px;display:flex;align-items:flex-end}.small.svelte-lpi64a{width:14px;height:14px}.large.svelte-lpi64a{width:22px;height:22px}.pending.svelte-lpi64a{animation:svelte-lpi64a-flash .5s infinite}@keyframes svelte-lpi64a-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-lpi64a{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-ipfyu7{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;padding-bottom:var(--spacing-xl);color:var(--block-label-text-color);flex-shrink:0;width:95%}.show_border.svelte-ipfyu7{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}.volume-slider.svelte-1xy0951{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:var(--size-20);accent-color:var(--color-accent);height:4px;cursor:pointer;outline:none;border-radius:15px;background-color:var(--neutral-400)}input[type=range].svelte-1xy0951::-webkit-slider-thumb{-webkit-appearance:none;-moz-appearance:none;appearance:none;height:15px;width:15px;background-color:var(--color-accent);border-radius:50%;border:none;transition:.2s ease-in-out}input[type=range].svelte-1xy0951::-moz-range-thumb{height:15px;width:15px;background-color:var(--color-accent);border-radius:50%;border:none;transition:.2s ease-in-out}.controls.svelte-sgfovr.svelte-sgfovr{display:grid;grid-template-columns:1fr 1fr 1fr;margin-top:5px;align-items:center;position:relative}.hidden.svelte-sgfovr.svelte-sgfovr{display:none}.control-wrapper.svelte-sgfovr.svelte-sgfovr{display:flex;justify-self:self-start;align-items:center;justify-content:space-between}@media (max-width: 375px){.controls.svelte-sgfovr.svelte-sgfovr{display:flex;flex-wrap:wrap}.controls.svelte-sgfovr .svelte-sgfovr{margin:var(--spacing-sm)}}.action.svelte-sgfovr.svelte-sgfovr{width:var(--size-5);color:var(--neutral-400);margin-left:var(--spacing-md)}.icon.svelte-sgfovr.svelte-sgfovr:hover{color:var(--color-accent);fill:var(--color-accent)}.play-pause-wrapper.svelte-sgfovr.svelte-sgfovr{display:flex;justify-self:right}.playback.svelte-sgfovr.svelte-sgfovr{border:1px solid var(--neutral-400);border-radius:var(--radius-sm);width:5.5ch;font-weight:300;font-size:var(--size-3);text-align:center;color:var(--neutral-400);height:var(--size-5);font-weight:700}.playback.svelte-sgfovr.svelte-sgfovr:hover,.playback.svelte-sgfovr.svelte-sgfovr:focus{color:var(--color-accent);border-color:var(--color-accent)}.rewind.svelte-sgfovr.svelte-sgfovr,.skip.svelte-sgfovr.svelte-sgfovr{margin:0 10px;color:var(--neutral-400)}.play-pause-button.svelte-sgfovr.svelte-sgfovr{width:var(--size-8);display:flex;align-items:center;justify-content:center;color:var(--neutral-400);fill:var(--neutral-400)}.volume.svelte-sgfovr.svelte-sgfovr{position:relative;display:flex;justify-content:center;margin-right:var(--spacing-xl)}.zoom-button.svelte-sgfovr.svelte-sgfovr{width:1.75em;fill:var(--neutral-400)}.caption-container.svelte-43he0g{display:flex;justify-content:center;margin-top:1em}div.svelte-43he0g.caption-container button{display:inline-block;padding:0 .5em;margin:.2em .5em}div.svelte-43he0g.caption-container button:hover{border-color:var(--color-accent)}button.active-button{border-width:2px;border-color:var(--color-accent)}.create-label.svelte-43he0g{width:2.25em;height:2.25em;fill:var(--neutral-400)}.create-label.svelte-43he0g:hover{fill:var(--color-accent)}.action.svelte-1w83umt{width:var(--size-5);color:var(--neutral-400);margin-left:var(--spacing-md)}.regions-actions.svelte-1w83umt{display:flex;justify-self:self-end;align-items:center}.commands.svelte-1w83umt{display:flex;justify-content:space-between}.component-wrapper.svelte-1w83umt{padding:4em}.icon.svelte-1w83umt:hover{color:var(--color-accent)}.remove-button.svelte-1w83umt,.trim-button.svelte-1w83umt{fill:var(--neutral-400)}.remove-button.svelte-1w83umt:hover,.remove-button.svelte-1w83umt:focus{fill:var(--color-accent)}.trim-button.svelte-1w83umt:hover,.trim-button.svelte-1w83umt:focus{fill:var(--color-accent)}.timestamps.svelte-1w83umt{display:flex;justify-content:space-between;align-items:center;width:100%;padding:var(--size-1) 0}#time.svelte-1w83umt,#duration.svelte-1w83umt{color:var(--neutral-400)}.waveform-container.svelte-1w83umt{display:flex;align-items:center;justify-content:center;width:var(--size-full)}.waveform-controls.svelte-1w83umt{width:80em}#waveform.svelte-1w83umt{width:100%;height:100%;position:relative}.standard-player.svelte-1w83umt{width:100%;padding:var(--size-2)}.icon-buttons.svelte-1mrvp2o{display:flex;position:absolute;top:6px;right:6px;gap:var(--size-1)}.wrap.svelte-cr2edf.svelte-cr2edf{overflow-y:auto;transition:opacity .5s ease-in-out;background:var(--block-background-fill);position:relative;display:flex;flex-direction:column;align-items:center;justify-content:center;min-height:var(--size-40);width:var(--size-full)}.wrap.svelte-cr2edf.svelte-cr2edf:after{content:"";position:absolute;top:0;left:0;width:var(--upload-progress-width);height:100%;transition:all .5s ease-in-out;z-index:1}.uploading.svelte-cr2edf.svelte-cr2edf{font-size:var(--text-lg);font-family:var(--font);z-index:2}.file-name.svelte-cr2edf.svelte-cr2edf{margin:var(--spacing-md);font-size:var(--text-lg);color:var(--body-text-color-subdued)}.file.svelte-cr2edf.svelte-cr2edf{font-size:var(--text-md);z-index:2;display:flex;align-items:center}.file.svelte-cr2edf progress.svelte-cr2edf{display:inline;height:var(--size-1);width:100%;transition:all .5s ease-in-out;color:var(--color-accent);border:none}.file.svelte-cr2edf progress[value].svelte-cr2edf::-webkit-progress-value{background-color:var(--color-accent);border-radius:20px}.file.svelte-cr2edf progress[value].svelte-cr2edf::-webkit-progress-bar{background-color:var(--border-color-accent);border-radius:20px}.progress-bar.svelte-cr2edf.svelte-cr2edf{width:14px;height:14px;border-radius:50%;background:radial-gradient(closest-side,var(--block-background-fill) 64%,transparent 53% 100%),conic-gradient(var(--color-accent) var(--upload-progress-width),var(--border-color-accent) 0);transition:all .5s ease-in-out}button.svelte-1s26xmt{cursor:pointer;width:var(--size-full)}.hidden.svelte-1s26xmt{display:none;height:0!important;position:absolute;width:0;flex-grow:0}.center.svelte-1s26xmt{display:flex;justify-content:center}.flex.svelte-1s26xmt{display:flex;flex-direction:column;justify-content:center;align-items:center}.disable_click.svelte-1s26xmt{cursor:default}input.svelte-1s26xmt{display:none}div.svelte-1wj0ocy{display:flex;top:var(--size-2);right:var(--size-2);justify-content:flex-end;gap:var(--spacing-sm);z-index:var(--layer-1)}.not-absolute.svelte-1wj0ocy{margin:var(--size-1)}.mic-select.svelte-l4xo8n.svelte-l4xo8n{height:var(--size-8);background:var(--block-background-fill);padding:0px var(--spacing-xxl);border-radius:var(--radius-full);font-size:var(--text-md);border:1px solid var(--neutral-400);margin:var(--size-1) var(--size-1) 0 0}.controls.svelte-l4xo8n.svelte-l4xo8n{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;overflow:hidden}.controls.svelte-l4xo8n select.svelte-l4xo8n{text-overflow:ellipsis;max-width:var(--size-40)}@media (max-width: 375px){.controls.svelte-l4xo8n select.svelte-l4xo8n{width:100%}}.wrapper.svelte-l4xo8n.svelte-l4xo8n{display:flex;align-items:center;flex-wrap:wrap}.record.svelte-l4xo8n.svelte-l4xo8n{margin-right:var(--spacing-md)}.stop-button-paused.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--neutral-400);margin:var(--size-1) var(--size-1) 0 0}.stop-button-paused.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.stop-button.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl);animation:svelte-l4xo8n-scaling 1.8s infinite}.stop-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--primary-600);margin:var(--size-1) var(--size-1) 0 0}.record-button.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.record-button.svelte-l4xo8n.svelte-l4xo8n{height:var(--size-8);width:var(--size-24);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);display:flex;align-items:center;border:1px solid var(--neutral-400)}.stop-button.svelte-l4xo8n.svelte-l4xo8n:disabled{cursor:not-allowed}.record-button.svelte-l4xo8n.svelte-l4xo8n:disabled{cursor:not-allowed;opacity:.5}@keyframes svelte-l4xo8n-scaling{0%{background-color:var(--primary-600);scale:1}50%{background-color:var(--primary-600);scale:1.2}to{background-color:var(--primary-600);scale:1}}.pause-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-md);margin:var(--size-1) var(--size-1) 0 0}.resume-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-xl);line-height:1px;font-size:var(--text-md);margin:var(--size-1) var(--size-1) 0 0}.duration.svelte-l4xo8n.svelte-l4xo8n{display:flex;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-md);align-items:center;justify-content:center;margin:var(--size-1) var(--size-1) 0 0}::part(region){border-radius:var(--radius-md);height:98%!important;border:1px solid var(--color-accent);border-width:0px 0px}::part(region-handle){width:5px!important;border:none}.microphone.svelte-1z0uz8p{width:100%;display:none}.component-wrapper.svelte-1z0uz8p{padding:var(--size-3);width:100%}.timestamps.svelte-1z0uz8p{display:flex;justify-content:space-between;align-items:center;width:100%;padding:var(--size-1) 0;margin:var(--spacing-md) 0}.time.svelte-1z0uz8p,.duration.svelte-1z0uz8p{color:var(--neutral-400)}.trim-duration.svelte-1z0uz8p{color:var(--color-accent);margin-right:var(--spacing-sm)}.mic-wrap.svelte-4ycsjo{display:block;align-items:center;margin:var(--spacing-xl)}.stop-button-paused.svelte-4ycsjo{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--neutral-400);margin-right:5px}.stop-button-paused.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.stop-button.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl);animation:svelte-4ycsjo-scaling 1.8s infinite}.stop-button.svelte-4ycsjo{height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--primary-600);margin-right:5px;display:flex}.record-button.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.record-button.svelte-4ycsjo{height:var(--size-8);width:var(--size-24);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);display:flex;align-items:center;border:1px solid var(--neutral-400)}@keyframes svelte-4ycsjo-scaling{0%{background-color:var(--primary-600);scale:1}50%{background-color:var(--primary-600);scale:1.2}to{background-color:var(--primary-600);scale:1}}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-1yserjw.svelte-1yserjw{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden;pointer-events:none}.wrap.center.svelte-1yserjw.svelte-1yserjw{top:0;right:0;left:0}.wrap.default.svelte-1yserjw.svelte-1yserjw{top:0;right:0;bottom:0;left:0}.hide.svelte-1yserjw.svelte-1yserjw{opacity:0;pointer-events:none}.generating.svelte-1yserjw.svelte-1yserjw{animation:svelte-1yserjw-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent;z-index:var(--layer-1)}.translucent.svelte-1yserjw.svelte-1yserjw{background:none}@keyframes svelte-1yserjw-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-1yserjw.svelte-1yserjw{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-1yserjw.svelte-1yserjw{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-1yserjw.svelte-1yserjw{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-1yserjw.svelte-1yserjw{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-1yserjw.svelte-1yserjw{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-1yserjw.svelte-1yserjw{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-1yserjw.svelte-1yserjw{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-1yserjw.svelte-1yserjw{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-1yserjw.svelte-1yserjw{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-1yserjw .progress-text.svelte-1yserjw{background:var(--block-background-fill)}.border.svelte-1yserjw.svelte-1yserjw{border:1px solid var(--border-color-primary)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}.gallery.svelte-1gecy8w{padding:var(--size-1) var(--size-2)}
+.block.svelte-nl1om8{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-nl1om8{border-color:var(--color-accent)}.block.border_contrast.svelte-nl1om8{border-color:var(--body-text-color)}.padded.svelte-nl1om8{padding:var(--block-padding)}.hidden.svelte-nl1om8{display:none}.hide-container.svelte-nl1om8{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-lpi64a{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-lpi64a{opacity:.5;box-shadow:none}button[disabled].svelte-lpi64a:hover{cursor:not-allowed}.padded.svelte-lpi64a{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-lpi64a:hover,button.highlight.svelte-lpi64a{cursor:pointer;color:var(--color-accent)}.padded.svelte-lpi64a:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-lpi64a{padding:0 1px;font-size:10px}div.svelte-lpi64a{padding:2px;display:flex;align-items:flex-end}.small.svelte-lpi64a{width:14px;height:14px}.large.svelte-lpi64a{width:22px;height:22px}.pending.svelte-lpi64a{animation:svelte-lpi64a-flash .5s infinite}@keyframes svelte-lpi64a-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-lpi64a{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-ipfyu7{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;padding-bottom:var(--spacing-xl);color:var(--block-label-text-color);flex-shrink:0;width:95%}.show_border.svelte-ipfyu7{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}.volume-slider.svelte-1xy0951{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:var(--size-20);accent-color:var(--color-accent);height:4px;cursor:pointer;outline:none;border-radius:15px;background-color:var(--neutral-400)}input[type=range].svelte-1xy0951::-webkit-slider-thumb{-webkit-appearance:none;-moz-appearance:none;appearance:none;height:15px;width:15px;background-color:var(--color-accent);border-radius:50%;border:none;transition:.2s ease-in-out}input[type=range].svelte-1xy0951::-moz-range-thumb{height:15px;width:15px;background-color:var(--color-accent);border-radius:50%;border:none;transition:.2s ease-in-out}.controls.svelte-sgfovr.svelte-sgfovr{display:grid;grid-template-columns:1fr 1fr 1fr;margin-top:5px;align-items:center;position:relative}.hidden.svelte-sgfovr.svelte-sgfovr{display:none}.control-wrapper.svelte-sgfovr.svelte-sgfovr{display:flex;justify-self:self-start;align-items:center;justify-content:space-between}@media (max-width: 375px){.controls.svelte-sgfovr.svelte-sgfovr{display:flex;flex-wrap:wrap}.controls.svelte-sgfovr .svelte-sgfovr{margin:var(--spacing-sm)}}.action.svelte-sgfovr.svelte-sgfovr{width:var(--size-5);color:var(--neutral-400);margin-left:var(--spacing-md)}.icon.svelte-sgfovr.svelte-sgfovr:hover{color:var(--color-accent);fill:var(--color-accent)}.play-pause-wrapper.svelte-sgfovr.svelte-sgfovr{display:flex;justify-self:right}.playback.svelte-sgfovr.svelte-sgfovr{border:1px solid var(--neutral-400);border-radius:var(--radius-sm);width:5.5ch;font-weight:300;font-size:var(--size-3);text-align:center;color:var(--neutral-400);height:var(--size-5);font-weight:700}.playback.svelte-sgfovr.svelte-sgfovr:hover,.playback.svelte-sgfovr.svelte-sgfovr:focus{color:var(--color-accent);border-color:var(--color-accent)}.rewind.svelte-sgfovr.svelte-sgfovr,.skip.svelte-sgfovr.svelte-sgfovr{margin:0 10px;color:var(--neutral-400)}.play-pause-button.svelte-sgfovr.svelte-sgfovr{width:var(--size-8);display:flex;align-items:center;justify-content:center;color:var(--neutral-400);fill:var(--neutral-400)}.volume.svelte-sgfovr.svelte-sgfovr{position:relative;display:flex;justify-content:center;margin-right:var(--spacing-xl)}.zoom-button.svelte-sgfovr.svelte-sgfovr{width:1.75em;fill:var(--neutral-400)}.caption-container.svelte-43he0g{display:flex;justify-content:center;margin-top:1em}div.svelte-43he0g.caption-container button{display:inline-block;padding:0 .5em;margin:.2em .5em}div.svelte-43he0g.caption-container button:hover{border-color:var(--color-accent)}button.active-button{border-width:2px;border-color:var(--color-accent)}.create-label.svelte-43he0g{width:2.25em;height:2.25em;fill:var(--neutral-400)}.create-label.svelte-43he0g:hover{fill:var(--color-accent)}.action.svelte-15fy58k{width:var(--size-5);color:var(--neutral-400);margin-left:var(--spacing-md)}.regions-actions.svelte-15fy58k{display:flex;justify-self:self-end;align-items:center}.commands.svelte-15fy58k{display:flex;justify-content:space-between}.component-wrapper.svelte-15fy58k{padding:4em}.icon.svelte-15fy58k:hover{color:var(--color-accent)}.remove-button.svelte-15fy58k,.trim-button.svelte-15fy58k{fill:var(--neutral-400)}.remove-button.svelte-15fy58k:hover,.remove-button.svelte-15fy58k:focus{fill:var(--color-accent)}.trim-button.svelte-15fy58k:hover,.trim-button.svelte-15fy58k:focus{fill:var(--color-accent)}::part(wrapper){margin-bottom:var(--size-2)}.timestamps.svelte-15fy58k{display:flex;justify-content:space-between;align-items:center;width:100%;padding:var(--size-1) 0}#time.svelte-15fy58k,#duration.svelte-15fy58k{color:var(--neutral-400)}.waveform-container.svelte-15fy58k{display:flex;align-items:center;justify-content:center;width:var(--size-full)}.waveform-controls.svelte-15fy58k{width:80em}#waveform.svelte-15fy58k{width:100%;height:100%;position:relative}.standard-player.svelte-15fy58k{width:100%;padding:var(--size-2)}.icon-buttons.svelte-1mrvp2o{display:flex;position:absolute;top:6px;right:6px;gap:var(--size-1)}.wrap.svelte-cr2edf.svelte-cr2edf{overflow-y:auto;transition:opacity .5s ease-in-out;background:var(--block-background-fill);position:relative;display:flex;flex-direction:column;align-items:center;justify-content:center;min-height:var(--size-40);width:var(--size-full)}.wrap.svelte-cr2edf.svelte-cr2edf:after{content:"";position:absolute;top:0;left:0;width:var(--upload-progress-width);height:100%;transition:all .5s ease-in-out;z-index:1}.uploading.svelte-cr2edf.svelte-cr2edf{font-size:var(--text-lg);font-family:var(--font);z-index:2}.file-name.svelte-cr2edf.svelte-cr2edf{margin:var(--spacing-md);font-size:var(--text-lg);color:var(--body-text-color-subdued)}.file.svelte-cr2edf.svelte-cr2edf{font-size:var(--text-md);z-index:2;display:flex;align-items:center}.file.svelte-cr2edf progress.svelte-cr2edf{display:inline;height:var(--size-1);width:100%;transition:all .5s ease-in-out;color:var(--color-accent);border:none}.file.svelte-cr2edf progress[value].svelte-cr2edf::-webkit-progress-value{background-color:var(--color-accent);border-radius:20px}.file.svelte-cr2edf progress[value].svelte-cr2edf::-webkit-progress-bar{background-color:var(--border-color-accent);border-radius:20px}.progress-bar.svelte-cr2edf.svelte-cr2edf{width:14px;height:14px;border-radius:50%;background:radial-gradient(closest-side,var(--block-background-fill) 64%,transparent 53% 100%),conic-gradient(var(--color-accent) var(--upload-progress-width),var(--border-color-accent) 0);transition:all .5s ease-in-out}button.svelte-1s26xmt{cursor:pointer;width:var(--size-full)}.hidden.svelte-1s26xmt{display:none;height:0!important;position:absolute;width:0;flex-grow:0}.center.svelte-1s26xmt{display:flex;justify-content:center}.flex.svelte-1s26xmt{display:flex;flex-direction:column;justify-content:center;align-items:center}.disable_click.svelte-1s26xmt{cursor:default}input.svelte-1s26xmt{display:none}div.svelte-1wj0ocy{display:flex;top:var(--size-2);right:var(--size-2);justify-content:flex-end;gap:var(--spacing-sm);z-index:var(--layer-1)}.not-absolute.svelte-1wj0ocy{margin:var(--size-1)}.mic-select.svelte-l4xo8n.svelte-l4xo8n{height:var(--size-8);background:var(--block-background-fill);padding:0px var(--spacing-xxl);border-radius:var(--radius-full);font-size:var(--text-md);border:1px solid var(--neutral-400);margin:var(--size-1) var(--size-1) 0 0}.controls.svelte-l4xo8n.svelte-l4xo8n{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;overflow:hidden}.controls.svelte-l4xo8n select.svelte-l4xo8n{text-overflow:ellipsis;max-width:var(--size-40)}@media (max-width: 375px){.controls.svelte-l4xo8n select.svelte-l4xo8n{width:100%}}.wrapper.svelte-l4xo8n.svelte-l4xo8n{display:flex;align-items:center;flex-wrap:wrap}.record.svelte-l4xo8n.svelte-l4xo8n{margin-right:var(--spacing-md)}.stop-button-paused.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--neutral-400);margin:var(--size-1) var(--size-1) 0 0}.stop-button-paused.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.stop-button.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl);animation:svelte-l4xo8n-scaling 1.8s infinite}.stop-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--primary-600);margin:var(--size-1) var(--size-1) 0 0}.record-button.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.record-button.svelte-l4xo8n.svelte-l4xo8n{height:var(--size-8);width:var(--size-24);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);display:flex;align-items:center;border:1px solid var(--neutral-400)}.stop-button.svelte-l4xo8n.svelte-l4xo8n:disabled{cursor:not-allowed}.record-button.svelte-l4xo8n.svelte-l4xo8n:disabled{cursor:not-allowed;opacity:.5}@keyframes svelte-l4xo8n-scaling{0%{background-color:var(--primary-600);scale:1}50%{background-color:var(--primary-600);scale:1.2}to{background-color:var(--primary-600);scale:1}}.pause-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-md);margin:var(--size-1) var(--size-1) 0 0}.resume-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-xl);line-height:1px;font-size:var(--text-md);margin:var(--size-1) var(--size-1) 0 0}.duration.svelte-l4xo8n.svelte-l4xo8n{display:flex;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-md);align-items:center;justify-content:center;margin:var(--size-1) var(--size-1) 0 0}::part(region){border-radius:var(--radius-md);height:98%!important;border:1px solid var(--color-accent);border-width:0px 0px}::part(region-handle){width:5px!important;border:none}.microphone.svelte-1z0uz8p{width:100%;display:none}.component-wrapper.svelte-1z0uz8p{padding:var(--size-3);width:100%}.timestamps.svelte-1z0uz8p{display:flex;justify-content:space-between;align-items:center;width:100%;padding:var(--size-1) 0;margin:var(--spacing-md) 0}.time.svelte-1z0uz8p,.duration.svelte-1z0uz8p{color:var(--neutral-400)}.trim-duration.svelte-1z0uz8p{color:var(--color-accent);margin-right:var(--spacing-sm)}.mic-wrap.svelte-4ycsjo{display:block;align-items:center;margin:var(--spacing-xl)}.stop-button-paused.svelte-4ycsjo{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--neutral-400);margin-right:5px}.stop-button-paused.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.stop-button.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl);animation:svelte-4ycsjo-scaling 1.8s infinite}.stop-button.svelte-4ycsjo{height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--primary-600);margin-right:5px;display:flex}.record-button.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.record-button.svelte-4ycsjo{height:var(--size-8);width:var(--size-24);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);display:flex;align-items:center;border:1px solid var(--neutral-400)}@keyframes svelte-4ycsjo-scaling{0%{background-color:var(--primary-600);scale:1}50%{background-color:var(--primary-600);scale:1.2}to{background-color:var(--primary-600);scale:1}}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-1yserjw.svelte-1yserjw{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden;pointer-events:none}.wrap.center.svelte-1yserjw.svelte-1yserjw{top:0;right:0;left:0}.wrap.default.svelte-1yserjw.svelte-1yserjw{top:0;right:0;bottom:0;left:0}.hide.svelte-1yserjw.svelte-1yserjw{opacity:0;pointer-events:none}.generating.svelte-1yserjw.svelte-1yserjw{animation:svelte-1yserjw-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent;z-index:var(--layer-1)}.translucent.svelte-1yserjw.svelte-1yserjw{background:none}@keyframes svelte-1yserjw-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-1yserjw.svelte-1yserjw{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-1yserjw.svelte-1yserjw{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-1yserjw.svelte-1yserjw{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-1yserjw.svelte-1yserjw{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-1yserjw.svelte-1yserjw{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-1yserjw.svelte-1yserjw{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-1yserjw.svelte-1yserjw{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-1yserjw.svelte-1yserjw{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-1yserjw.svelte-1yserjw{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-1yserjw .progress-text.svelte-1yserjw{background:var(--block-background-fill)}.border.svelte-1yserjw.svelte-1yserjw{border:1px solid var(--border-color-primary)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}.gallery.svelte-1gecy8w{padding:var(--size-1) var(--size-2)}
```

### Comparing `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/wrapper-6f348d45-19fa94bf.js` & `gryannote_audio-0.1.6/backend/gryannote_audio/templates/component/wrapper-6f348d45-19fa94bf.js`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/backend/gryannote_audio/templates/example/index.js` & `gryannote_audio-0.1.6/backend/gryannote_audio/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/Index.svelte` & `gryannote_audio-0.1.6/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/package-lock.json` & `gryannote_audio-0.1.6/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/package.json` & `gryannote_audio-0.1.6/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/interactive/InteractiveAnnotatedAudio.svelte` & `gryannote_audio-0.1.6/frontend/interactive/InteractiveAnnotatedAudio.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/player/AudioPlayerWithAnnotation.svelte` & `gryannote_audio-0.1.6/frontend/player/AudioPlayerWithAnnotation.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 		type RegionParams,
 	} from "wavesurfer.js/dist/plugins/regions.js";
 	import WaveformControls from "../shared/WaveformControls.svelte";
 	import { Empty } from "@gradio/atoms";
 	import { resolve_wasm_src } from "@gradio/wasm/svelte";
 	import AnnotatedAudioData from "../shared/AnnotatedAudioData";
 	import { createEventDispatcher } from "svelte";
-	import Caption  from "../shared/Caption.svelte"
+	import Caption from "../shared/Caption.svelte"
 
 	export let value: null | AnnotatedAudioData = null;
 	$: url = value.file_data?.url;
 	export let label: string;
 	export let i18n: I18nFormatter;
 	export let interactive = true;
 	export let editable = true;
@@ -151,19 +151,18 @@
 	}
 
 	/**
 	 * Handle add region event. The new added region become the active region.
 	 * @param relativeY mouse y-coordinate relative to waveform start
 	 */
 	function handleRegionAdd(relativeY: number): void{
-		let label = (activeLabel !== null ? activeLabel : defaultLabel);
+		let label = (activeLabel ? activeLabel : defaultLabel);
 		// if annotations were not initialized, do nothing
-		if (label === null){
-			window.alert("First create a label by clicking on \"+\" or by pressing A-Z");
-			return;
+		if (!label){
+			label = caption.createLabel();
 		}
 		let region = addRegion({
 			start: relativeY - 1.0,
 			end: relativeY + 1.0,
 			color: label.color,
 			drag: true,
 			resize: true,
@@ -239,23 +238,23 @@
 	};
 
 	/**
 	 * Set active region with specified one.
 	 * @param region the region to activate
 	 */
 	function setActiveRegion(region: Region): void {
-		if(activeRegion !== null){
+		if(activeRegion){
 			activeRegion.element.style.background = activeRegion.color;
 		}
 
-		if(region === null){
-			activeRegion = region;
+		activeRegion = region;
+		if(!activeRegion){
 			return;
 		}
-		activeRegion = region;
+
 		activeRegion.element.style.background = "repeating-linear-gradient(45deg,"
 						+ region.color
 						+ " ,"
 						+ region.color
 						+ " 10px, #ffffff 10px ,#ffffff 15px)";
 	}
 
@@ -485,14 +484,31 @@
 		(currentTime: any) =>
 			timeRef && (timeRef.textContent = formatTime(currentTime))
 	);
 
 	$: waveform?.on("ready", () => {
 		if(wsRegions === undefined ){
 			wsRegions = waveform.registerPlugin(RegionsPlugin.create());
+
+			// add region-clicked event listener
+			wsRegions?.on("region-clicked", (region, e) => {
+				switch(mode){
+					case "remove": removeRegion(region); break;
+					case "split": splitRegion(region, region.start + (region.end - region.start) / 2); break;
+					default: setActiveRegion(region); region.play();
+				}
+				mode = "";
+			});
+
+			wsRegions?.on("region-updated", (region) => {
+				var updatedAnnotation = regionsMap.get(region.id);
+				updatedAnnotation.start = region.start;
+				updatedAnnotation.end = region.end;
+				updateAnnotations();
+			});
 		}
 		if (!waveform_settings.autoplay) {
 			waveform?.stop();
 		} else {
 			waveform?.play();
 		}
 	});
@@ -508,30 +524,14 @@
 	});
 
 	$: waveform?.on("play", () => {
 		playing = true;
 		dispatch("play");
 	});
 
-	$: wsRegions?.on("region-updated", (region) => {
-		var updatedAnnotation = regionsMap.get(region.id);
-		updatedAnnotation.start = region.start;
-		updatedAnnotation.end = region.end;
-		updateAnnotations();
-	});
-
-	$: wsRegions?.on("region-clicked", (region, e) => {
-		switch(mode){
-			case "remove": removeRegion(region); break;
-			case "split": splitRegion(region, region.start + (region.end - region.start) / 2); break;
-			default: setActiveRegion(region); region.play();
-		}
-		mode = "";
-	});
-
 	$: if (activeRegion) {
 		const shadowRoot = container.children[0]!.shadowRoot!;
 
 		rightRegionHandle = shadowRoot.querySelector('[data-resize="right"]');
 		leftRegionHandle = shadowRoot.querySelector('[data-resize="left"]');
 
 		if (leftRegionHandle && rightRegionHandle) {
@@ -652,16 +652,16 @@
 						<Trim/>
 					</button>
 				{/if}
 				</div>
 			</div>
 			{#if value}
 				<Caption
-					value={value.annotations}
 					bind:this={caption}
+					bind:annotations={value.annotations}
 					on:select={(e) => setRegionSpeaker(e.detail)}
 					on:select={(e) => activeLabel = e.detail}
 				/>
 			{/if}
 		{/if}
 	</div>
 {/if}
@@ -701,14 +701,18 @@
 		fill: var(--color-accent);
 	}
 
 	.trim-button:hover, .trim-button:focus {
 		fill: var(--color-accent);
 	}
 
+	:global(::part(wrapper)) {
+			margin-bottom: var(--size-2);
+	}
+
 	.timestamps {
 		display: flex;
 		justify-content: space-between;
 		align-items: center;
 		width: 100%;
 		padding: var(--size-1) 0;
 	}
```

### Comparing `gryannote_audio-0.1.5/frontend/recorder/AudioRecorder.svelte` & `gryannote_audio-0.1.6/frontend/recorder/AudioRecorder.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/shared/AnnotatedAudioData.ts` & `gryannote_audio-0.1.6/frontend/shared/AnnotatedAudioData.ts`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/shared/Audio.svelte` & `gryannote_audio-0.1.6/frontend/shared/Audio.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/shared/Caption.svelte` & `gryannote_audio-0.1.6/frontend/shared/Caption.svelte`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <script lang="ts">
     import type { Annotation, CaptionLabel } from "./types";
     import Plus from "./icons/Plus.svelte";
     import { createEventDispatcher, onMount} from "svelte";
 
-    export let value: Annotation[] | null = null;
+    export let annotations: Annotation[] | null = null;
 
     let container: HTMLDivElement;
 
     let labels: CaptionLabel[] = [];
     let activeLabel = null;
 
     let speakerIdx: number = 0;
@@ -32,15 +32,15 @@
 
     export function createLabel(speaker?: string, color?: string, shortcut?: string): CaptionLabel {
         // if maximum number of labels has been reached, do nothing
         if(labels.length === 26){
             return;
         }
         if(!speaker){
-            speaker = "SPEAKER_" + speakerIdx.toString().padStart(2, "0");
+            speaker = "LABEL_" + speakerIdx.toString().padStart(2, "0");
         }
         if(!color){
             color = colorList[speakerIdx % colorList.length];
         }
         if(!shortcut){
             shortcut = "A";
             //take the first available letter
@@ -85,17 +85,17 @@
                 label = createLabel(undefined, undefined , key.toUpperCase());
             }
         }
         setActiveLabel(label);
     }
 
     $:{
-        if(container && value){
+        if(container && annotations){
             // retrieve speaker list and corresponding annotation color
-            value.forEach(annotation => {
+            annotations.forEach(annotation => {
                 // if annotation has a label that does not already exist in the caption,
                 // create a new label
                 if(!labels.some(label => label.speaker === annotation.speaker)){
                     createLabel(annotation.speaker, annotation.color);
                 }
             });
             labels = labels.sort((i1, i2) => i1.shortcut.localeCompare(i2.shortcut));
```

### Comparing `gryannote_audio-0.1.5/frontend/shared/VolumeControl.svelte` & `gryannote_audio-0.1.6/frontend/shared/VolumeControl.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/shared/WaveformControls.svelte` & `gryannote_audio-0.1.6/frontend/shared/WaveformControls.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/shared/WaveformRecordControls.svelte` & `gryannote_audio-0.1.6/frontend/shared/WaveformRecordControls.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/shared/audioBufferToWav.ts` & `gryannote_audio-0.1.6/frontend/shared/audioBufferToWav.ts`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/shared/utils.ts` & `gryannote_audio-0.1.6/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/shared/icons/Gum.svelte` & `gryannote_audio-0.1.6/frontend/shared/icons/Gum.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/shared/icons/Magnifier.svelte` & `gryannote_audio-0.1.6/frontend/shared/icons/Magnifier.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/shared/icons/Plus.svelte` & `gryannote_audio-0.1.6/frontend/shared/icons/Plus.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/static/StaticAnnotatedAudio.svelte` & `gryannote_audio-0.1.6/frontend/static/StaticAnnotatedAudio.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/frontend/streaming/StreamAudio.svelte` & `gryannote_audio-0.1.6/frontend/streaming/StreamAudio.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/README.md` & `gryannote_audio-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.5/pyproject.toml` & `gryannote_audio-0.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,39 +4,37 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gryannote_audio"
-version = "0.1.5"
+version = "0.1.6"
 description = "audio component with speaker annotations"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "Clément Pagés", email = "clement.pages@irit.fr" }]
 keywords = ["gradio-custom-component", "gradio-template-Audio", "pyannote.audio", "speaker diarization"]
 # Add dependencies here
 dependencies = ["gradio>=4.0,<5.0"]
 classifiers = [
   'Development Status :: 3 - Alpha',
   'License :: OSI Approved :: Apache Software License',
   'Operating System :: OS Independent',
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3 :: Only',
-  'Programming Language :: Python :: 3.8',
-  'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
   'Topic :: Scientific/Engineering',
   'Topic :: Scientific/Engineering :: Artificial Intelligence',
   'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gryannote_audio/templates", "*.pyi", "backend/gryannote_audio/templates", "backend/gryannote_audio/templates"]
+artifacts = ["/backend/gryannote_audio/templates", "*.pyi", "backend/gryannote_audio/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gryannote_audio"]
```

### Comparing `gryannote_audio-0.1.5/PKG-INFO` & `gryannote_audio-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.3
 Name: gryannote_audio
-Version: 0.1.5
+Version: 0.1.6
 Summary: audio component with speaker annotations
 Author-email: Clément Pagés <clement.pages@irit.fr>
 License-Expression: MIT
 Keywords: gradio-custom-component,gradio-template-Audio,pyannote.audio,speaker diarization
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8
 Requires-Dist: gradio<5.0,>=4.0
```

