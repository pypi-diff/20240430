# Comparing `tmp/streamlit-float-0.3.2.tar.gz` & `tmp/streamlit-float-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-float-0.3.2.tar", last modified: Mon Oct  9 18:51:53 2023, max compression
+gzip compressed data, was "streamlit-float-0.3.3.tar", last modified: Mon Apr 29 23:31:16 2024, max compression
```

## Comparing `streamlit-float-0.3.2.tar` & `streamlit-float-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-10-09 18:51:53.760812 streamlit-float-0.3.2/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1067 2023-08-24 16:01:17.000000 streamlit-float-0.3.2/LICENSE.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2290 2023-10-09 18:51:53.760812 streamlit-float-0.3.2/PKG-INFO
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7236 2023-09-19 00:57:43.000000 streamlit-float-0.3.2/README.md
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       38 2023-10-09 18:51:53.760812 streamlit-float-0.3.2/setup.cfg
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      845 2023-10-09 18:51:30.000000 streamlit-float-0.3.2/setup.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-10-09 18:51:53.760812 streamlit-float-0.3.2/streamlit_float/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    13788 2023-10-09 18:48:31.000000 streamlit-float-0.3.2/streamlit_float/__init__.py
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10269 2023-09-25 22:03:34.000000 streamlit-float-0.3.2/streamlit_float/demo.py
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1810 2023-09-19 01:10:41.000000 streamlit-float-0.3.2/streamlit_float/test.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-10-09 18:51:53.760812 streamlit-float-0.3.2/streamlit_float.egg-info/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2290 2023-10-09 18:51:53.000000 streamlit-float-0.3.2/streamlit_float.egg-info/PKG-INFO
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      300 2023-10-09 18:51:53.000000 streamlit-float-0.3.2/streamlit_float.egg-info/SOURCES.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)        1 2023-10-09 18:51:53.000000 streamlit-float-0.3.2/streamlit_float.egg-info/dependency_links.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-10-09 18:51:53.000000 streamlit-float-0.3.2/streamlit_float.egg-info/requires.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-10-09 18:51:53.000000 streamlit-float-0.3.2/streamlit_float.egg-info/top_level.txt
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-04-29 23:31:16.453580 streamlit-float-0.3.3/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     1067 2024-03-04 22:49:07.000000 streamlit-float-0.3.3/LICENSE.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-04-29 23:31:16.453580 streamlit-float-0.3.3/PKG-INFO
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     7236 2024-03-04 22:49:07.000000 streamlit-float-0.3.3/README.md
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       38 2024-04-29 23:31:16.453580 streamlit-float-0.3.3/setup.cfg
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      845 2024-04-29 23:29:43.000000 streamlit-float-0.3.3/setup.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-04-29 23:31:16.453580 streamlit-float-0.3.3/streamlit_float/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)    16191 2024-04-29 23:30:11.000000 streamlit-float-0.3.3/streamlit_float/__init__.py
+-rw-r--r--   0 anasb     (1000) anasb     (1000)    11875 2024-03-04 22:49:07.000000 streamlit-float-0.3.3/streamlit_float/demo.py
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     1810 2024-03-04 22:49:07.000000 streamlit-float-0.3.3/streamlit_float/test.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-04-29 23:31:16.453580 streamlit-float-0.3.3/streamlit_float.egg-info/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-04-29 23:31:16.000000 streamlit-float-0.3.3/streamlit_float.egg-info/PKG-INFO
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      300 2024-04-29 23:31:16.000000 streamlit-float-0.3.3/streamlit_float.egg-info/SOURCES.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)        1 2024-04-29 23:31:16.000000 streamlit-float-0.3.3/streamlit_float.egg-info/dependency_links.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       16 2024-04-29 23:31:16.000000 streamlit-float-0.3.3/streamlit_float.egg-info/requires.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       16 2024-04-29 23:31:16.000000 streamlit-float-0.3.3/streamlit_float.egg-info/top_level.txt
```

### Comparing `streamlit-float-0.3.2/LICENSE.txt` & `streamlit-float-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-float-0.3.2/PKG-INFO` & `streamlit-float-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: streamlit-float
-Version: 0.3.2
+Version: 0.3.3
 Summary: Fix Streamlit containers relative to viewport instead of page
 Home-page: https://github.com/bouzidanas/streamlit-float
 Author: Anas Bouzid
 Author-email: anasbouzid@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 streamlit-float [![PyPi - Downloads](https://img.shields.io/pypi/dm/streamlit-float)](https://pypi.org/project/streamlit-float/#files)
 ============
 
@@ -75,7 +77,8 @@
 
 ```python
 st.markdown('''<div class="floating">..content..</div>''', unsafe_allow_html=True)
 ```
 
 ## License
 This project is licensed under the [MIT License](LICENSE.txt)
+
```

### Comparing `streamlit-float-0.3.2/README.md` & `streamlit-float-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-float-0.3.2/setup.py` & `streamlit-float-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "PROJECT.md").read_text()
 
 setup(
     name='streamlit-float',
-    version='0.3.2',
+    version='0.3.3',
     author='Anas Bouzid',
     author_email='anasbouzid@gmail.com',
     description='Fix Streamlit containers relative to viewport instead of page',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/bouzidanas/streamlit-float",
     packages=find_packages(),
```

### Comparing `streamlit-float-0.3.2/streamlit_float/__init__.py` & `streamlit-float-0.3.3/streamlit_float/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,16 +29,17 @@
                "box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;",
                "box-shadow: rgba(50, 50, 93, 0.25) 0px 30px 60px -12px, rgba(0, 0, 0, 0.3) 0px 18px 36px -18px;",
                "box-shadow: rgba(50, 50, 93, 0.25) 0px 30px 60px -12px inset, rgba(0, 0, 0, 0.3) 0px 18px 36px -18px inset;",
                "box-shadow: rgba(17, 17, 26, 0.1) 0px 4px 16px, rgba(17, 17, 26, 0.05) 0px 8px 32px;"
                ]
 
 transition_list = ["transition-property: all;transition-duration: .5s;transition-timing-function: cubic-bezier(0, 1, 0.5, 1);", 
-                   "transition-property: all;transition-duration: .5s;transition-timing-function: cubic-bezier(0.15, 0.45, 0.85, 0.55);", 
-                   "transition-property: all;transition-duration: .6s;transition-timing-function: ease-in-out;"
+                   "transition-property: all;transition-duration: .5s;transition-timing-function: cubic-bezier(0.2, 0.6, 0.85, 0.55);", 
+                   "transition-property: all;transition-duration: .6s;transition-timing-function: ease-in-out;",
+                   "transition-property: all;transition-duration: .5s;transition-timing-function: cubic-bezier(1.000, 0.010, 0.30, 1.000);"
                    ]
 
 def theme_init(include_unstable_primary=False):
     if include_unstable_primary:
         javascript_end = """
     prev = cont.previousElementSibling;
     first = prev.previousElementSibling;          
@@ -84,14 +85,20 @@
         st.button("", type="primary")
     st.markdown("<div id='elim'></div>", unsafe_allow_html=True)
 
 def float_init(theme=True, include_unstable_primary=False):
 # add css to streamlit app
     html_style = '''
     <style>
+    div.element-container:has(div.float) {
+        position: absolute!important;
+    }
+    div.element-container:has(div.floating) {
+        position: absolute!important;
+    }
     div:has( >.element-container div.float) {
         display: flex;
         flex-direction: column;
         position: fixed;
         z-index: 99;
     }
     div.float, div.elim {
@@ -107,20 +114,20 @@
     </style>
     '''
     st.markdown(html_style, unsafe_allow_html=True)
     if theme:
         theme_init(include_unstable_primary=include_unstable_primary)
 
 # adds empty div to parent in order to target it with css
+# TODO: remove extra gap generated when floating containers. To do this, find the appropriate parent div and set `position: absolute` on it.
 def float_parent(css=None):
     if css is not None:
         new_id = str(uuid.uuid4())[:8]
-        new_css = '<style>\ndiv:has( >.element-container div.flt-' + new_id + ') {' + css + '}\n</style>'
-        st.markdown(new_css, unsafe_allow_html=True)
-        st.markdown('<div class="float flt-' + new_id + '"></div>', unsafe_allow_html=True)
+        new_css = '<style>\ndiv.element-container[data-testid="element-container"]:has(>div div.flt-' + new_id + '){\n  diaplay: none!important;\n}\ndiv:has( >.element-container div.flt-' + new_id + ') {' + css + '}\n</style>'
+        st.markdown(new_css + '\n<div class="float flt-' + new_id + '"></div>', unsafe_allow_html=True)
         js_ = f'''
             <script>
                 float_el = parent.document.querySelectorAll('div[class="float flt-{new_id}"]')
                 float_el_parent_two_levels_up = float_el[0].closest("div > .element-container ").parentNode
                 float_el_parent_two_levels_up.id = "float-this-component-{new_id}"
                 float_el_parent_two_levels_up.style = '{css}'
                 new_float_id_el = parent.document.querySelectorAll('iframe[srcdoc*="{new_id}"]')[0].parentNode
@@ -130,20 +137,20 @@
             </script>
             '''
         st.components.v1.html(js_)
     else:
         st.markdown('<div class="float"></div>', unsafe_allow_html=True)
 
 # float container via its delta generator 
-def float(self, css=None):
+# TODO: remove extra gap generated when floating containers. To do this, find the appropriate parent div and set `position: absolute` on it.
+def sf_float(self, css=None):
     if css is not None:
         new_id = str(uuid.uuid4())[:8]
-        new_css = '<style>\ndiv:has( >.element-container div.flt-' + new_id + ') {' + css + '}\n</style>'
-        st.markdown(new_css, unsafe_allow_html=True)
-        self.markdown('<div class="float flt-' + new_id + '"></div>', unsafe_allow_html=True)
+        new_css = '<style>\ndiv.element-container[data-testid="element-container"]:has(>div div.flt-' + new_id + '){\n  position: absolute!important;\n}\ndiv:has( >.element-container div.flt-' + new_id + ') {' + css + '}\n</style>'
+        self.markdown(new_css + '\n<div class="float flt-' + new_id + '"></div>', unsafe_allow_html=True)
         js_ = f'''
             <script>
                 float_el_delta = parent.document.querySelectorAll('div[class="float flt-{new_id}"]')
                 float_el_parent_two_levels_up = float_el_delta[0].closest("div > .element-container ").parentNode
                 float_el_parent_two_levels_up.id = "float-this-component-{new_id}"
                 float_el_parent_two_levels_up.style = 'display:flex; flex-direction:column; position:fixed; z-index:99; {css}'
                 new_float_id_el = parent.document.querySelectorAll('iframe[srcdoc*="{new_id}"]')[0].parentNode
@@ -153,15 +160,15 @@
             </script>
             '''
         st.components.v1.html(js_)
     else:
         self.markdown('<div class="float"></div>', unsafe_allow_html=True)
 
 # add float method to st.delta_generator.DeltaGenerator class so it can be directly called
-st.delta_generator.DeltaGenerator.float = float
+st.delta_generator.DeltaGenerator.float = sf_float
 
 # create a floating box containing markdown content
 def float_box(markdown, width="300px", height="300px", top=None, left=None, right=None, bottom=None, background=None, border=None, shadow=None, transition=None, z_index=None, sticky=False, css=None):
     jct_css = "width: " + width + "; height: " + height + ";border-radius: 0.5rem;padding: 1rem;padding-left: 1.3rem;padding-right: 1.3rem;"
     if shadow is not None and type(shadow) is int and shadow < len(shadow_list) and shadow >= 0:
         jct_css += shadow_list[int(shadow)]
     elif type(shadow) is str:
@@ -235,38 +242,64 @@
     for key, value in kwargs.items():
         jct_css += f"{key.replace('_', '-')}: {value};"
 
     return jct_css
 
 # Create a floating dialog container 
 # This needs to be fleshed out more. Add more options for positions, transitions, etc.
-def float_dialog(show=False, width=2, background="slategray", transition=2, css=""):
+def float_dialog(show=False, width=2, background="slategray", transition=2, transition_from="top", transition_to="center", css=""):
     float_col_a, float_col_b = st.columns([width, 1])
 
+    if transition_from == "top":
+        hidden_background_pos_css = "top: min(-100vh, -100vi);"
+        hidden_dialog_pos_css = "top: min(-100vh, -100vi);transform: translateX(-50%) translateY(-50%);"
+    elif transition_from == "bottom":
+        hidden_background_pos_css = "bottom: min(-100vh, -100vi);"
+        hidden_dialog_pos_css = "bottom: min(-100vh, -100vi);transform: translateX(-50%) translateY(50%);"
+    elif transition_from == "center":
+        hidden_background_pos_css = "top: 50%;transform: translateY(-50%) scale(0);"
+        hidden_dialog_pos_css = "top: 50%;transform: translateX(-50%) translateY(-50%) scale(0);"
+
+    if transition_to == "top":
+        visible_background_pos_css = "top: 2.3rem;"
+        visible_dialog_pos_css = "top: 2.3rem;transform: translateX(-50%);"
+    elif transition_to == "bottom":
+        visible_background_pos_css = "bottom: -2.3rem;"
+        visible_dialog_pos_css = "bottom: 2.3rem;transform: translateX(-50%);"
+    elif transition_to == "center":
+        if transition_from == "bottom":
+            visible_background_pos_css = "bottom: 50%;transform: translateY(50%) scale(1);"
+            visible_dialog_pos_css = "bottom: 50%;transform: translateX(-50%) translateY(50%) scale(1);"
+        else:
+            visible_background_pos_css = "top: 50%;transform: translateY(-50%) scale(1);"
+            visible_dialog_pos_css = "top: 50%;transform: translateX(-50%) translateY(-50%) scale(1);"
+
     with float_col_a:    
         dialog_container = st.container()
 
     if show:
-        pos_css = "top: 2.3rem;"
+        background_pos_css = visible_background_pos_css
+        dialog_pos_css = visible_dialog_pos_css
     else:
-        pos_css = "top: min(-100vh, -100vi);"
+        background_pos_css = hidden_background_pos_css
+        dialog_pos_css = hidden_dialog_pos_css
 
     if transition is not None and type(transition) is int and transition < len(transition_list) and transition >= 0:
-        tran_css = transition_list[int(transition)]
+        transition_css = transition_list[int(transition)]
     elif type(transition) is str:
-        tran_css = transition
+        transition_css = transition
     else:
-        tran_css = ""
+        transition_css = ""
 
-    float_col_b.float(float_css_helper(width="100%", height="100%", left="0", top="0", background="rgba(0, 0, 0, 0.4)", css="z-index: 999000;" + pos_css))
-    float_col_a.float(pos_css + "padding: 2rem;padding-bottom: 0.9rem;border-radius: 0.5rem;left: 50%;transform: translateX(-50%);z-index: 999900;" + tran_css + css + "transition-property: top;background-color: " + background + ";")
+    float_col_b.float(float_css_helper(width="100%", height="100%", left="0", background="rgba(0, 0, 0, 0.4)", css="z-index: 999000;" + background_pos_css))
+    float_col_a.float("padding: 2rem;padding-bottom: 0.9rem;border-radius: 0.5rem;left: 50%;z-index: 999900;" + dialog_pos_css + transition_css + css + "transition-property: top, bottom;background-color: " + background + ";")
     return dialog_container
 
 
-def float_overlay(show=False, z_index="999989", color="#000000", alpha=0.0, blur="1rem", filter=None):
+def float_overlay(show=False, z_index="999999", color="#000000", alpha=0.0, blur="1rem", filter=None):
     if color.startswith("#"):
         color += ("0%x" % int(255*alpha))[-2:]
     elif color.startswith("rgb"):
         color = color.replace(")", f", {alpha})")
 
     if filter is not None:
         backdrop_filter = filter
```

### Comparing `streamlit-float-0.3.2/streamlit_float/demo.py` & `streamlit-float-0.3.3/streamlit_float/demo.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 st.set_page_config(page_title='streamlit-float demo', initial_sidebar_state='collapsed')
 
 float_init()
 
 if "show" not in st.session_state:
     st.session_state.show = False
+if "tutorial" not in st.session_state:
+    st.session_state.tutorial = False
+if "menusel" not in st.session_state:
+    st.session_state.menusel = 0
 
 # Function to navigate to a new page
 # An improvement here would be to open in new tab
 def nav_to(url):
     nav_script = """
         <meta http-equiv="refresh" content="0; url='%s'">
     """ % (url)
@@ -93,15 +97,14 @@
     button_b_pos = "1rem"
 
 button_css = float_css_helper(width="2.2rem", right="2rem", bottom=button_b_pos, transition=0)
 
 button_container.float(button_css)
 float_box('<iframe width="100%" height="100%" src="https://www.youtube.com/embed/J8TgKxomS2g?si=Ir_bq_E5e9jHAEFw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>',width="29rem", right="2rem", bottom=vid_y_pos, transition=0, shadow=12, css="padding: 0;")
 
-
 # Initialize session variable that will open/close dialog
 if "dialog" not in st.session_state:
     st.session_state.dialog = False
 
 # Button that opens the dialog
 if st.button("Contact us"):
     st.session_state.dialog = True
@@ -113,68 +116,92 @@
 # Add contents of Dialog including button to close it
 with dialog_container:
     st.header("Contact us")
     name_input = st.text_input("Enter your name")
     email_input = st.text_input("Enter your email")
     message = st.text_area("Enter your message")
     if st.button("Send", key="send"):
+        st.session_state.menusel = 0
         st.session_state.dialog = False
         st.experimental_rerun()
 
 # Create a menu container
 menu_container = st.container()
 
 # Add option menu to menu container
 with menu_container:
     menu_selection = option_menu(None, ["Home", "Tutorial", "Video", 'Contact'], 
     icons=['house', 'people', 'play-btn', "chat-square-text"], 
     menu_icon="cast", default_index=0, orientation="horizontal",
+    manual_select=st.session_state.menusel,
     styles={
         "container": {"padding": "0.2rem 0", "background-color": "#22222200"},
            })
 
 # Handle menu selection
 if menu_selection == "Contact":
     st.session_state.menusel = 3
     if not st.session_state.dialog:
         st.session_state.dialog = True
         st.experimental_rerun()
     else:
         st.session_state.dialog = False
+elif menu_selection == "Tutorial":
+    st.session_state.menusel = 1
+    if not st.session_state.tutorial:
+        st.session_state.tutorial = True
 elif menu_selection == "Video":
     st.session_state.menusel = 2
     if not st.session_state.show:
         st.session_state.show = True
         st.experimental_rerun()    
 elif menu_selection == "Home":
     st.session_state.menusel = 0
 
 # Float menu container
 menu_container.float("top: 0.15rem;z-index: 999990;")
 
 # Create a floating links
 float_box('<a href="https://pypi.org/project/streamlit-float/">PYPI</a>・<a href="https://github.com/bouzidanas/streamlit-float">Github</a>・<a href="https://discuss.streamlit.io/t/anybody-interested-in-simple-component-to-float-containers/45013?u=bouzidanas">Community</a> ', width="fit-content", height="2rem", right="-5.6rem", top="12rem", background="transparent", css="flex-direction: row;align-items: center;color: #ffffff99;rotate: 90deg;")
 
-# Create a banner container
-banner_container = st.container()
+# add overlay
+float_overlay(st.session_state.tutorial, alpha=0.2, z_index="999980")
 
-# Add alert banner to banner container
-with banner_container:
-    sac.alert(message='**WARNING! This is a demo. This is not a real article.**', description=None, type='warning', height=None, icon=True, closable=True, banner=True)
+# # Create a banner container
+# banner_container = st.container()
 
-# Float banner container
-banner_container.float("bottom: -1rem;z-index: 999992;")
+# # Add alert banner to banner container
+# with banner_container:
+#     sac.alert(message='**WARNING! This is a demo. This is not a real article.**', description=None, type='warning', height=None, icon=True, closable=True, banner=True)
+
+# # Float banner container
+# banner_container.float("bottom: -1rem;z-index: 999992;")
 
 # Custom styles for floating links
 # Note Float box container has "floating" class
 style = '''<style>
 .floating a {
     color: var(--default-textColor);
     opacity: 0.4;
     text-decoration: none;
 }
 .floating a:hover {
     color: var(--default-textColor)!important;
     opacity: 1;
 }
 </style>'''
-st.markdown(style, unsafe_allow_html=True)
+st.markdown(style, unsafe_allow_html=True)
+
+if st.session_state.tutorial:
+    close_overlay_container = st.container()
+    with close_overlay_container:
+        if st.button("Close", key="close"):
+            st.session_state.tutorial = False
+            st.session_state.menusel = 0
+            st.experimental_rerun()
+
+    # Float close button
+    close_overlay_css = float_css_helper(width="2.2rem", right="4rem", bottom="2rem", z_index="999999")
+    close_overlay_container.float(close_overlay_css)
+
+    float_box('<div>↑</div><div>Place Menus/Navbars in a container and float it to the top or bottom of the page</div>', width="30%", height="2rem", right="50%", top="3rem", background="transparent", css="max-width:50%;width:fit-content;flex-direction: column;align-items: center;color: #ffffff;font-size:1.8rem;z-index:999999;translate: 50%;")
+    float_box('<div style="height:fit-content;">Click close button to exit tutorial </div><div>↴</div>', height="2rem", right="2.7rem", bottom="7.5rem", background="transparent", css="min-width: 25%; width:fit-content;flex-direction: row;justify-content: right;color: #ffffff;font-size:1.8rem;z-index:999999;gap:0.5rem;")
```

### Comparing `streamlit-float-0.3.2/streamlit_float/test.py` & `streamlit-float-0.3.3/streamlit_float/test.py`

 * *Files identical despite different names*

### Comparing `streamlit-float-0.3.2/streamlit_float.egg-info/PKG-INFO` & `streamlit-float-0.3.3/streamlit_float.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: streamlit-float
-Version: 0.3.2
+Version: 0.3.3
 Summary: Fix Streamlit containers relative to viewport instead of page
 Home-page: https://github.com/bouzidanas/streamlit-float
 Author: Anas Bouzid
 Author-email: anasbouzid@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 streamlit-float [![PyPi - Downloads](https://img.shields.io/pypi/dm/streamlit-float)](https://pypi.org/project/streamlit-float/#files)
 ============
 
@@ -75,7 +77,8 @@
 
 ```python
 st.markdown('''<div class="floating">..content..</div>''', unsafe_allow_html=True)
 ```
 
 ## License
 This project is licensed under the [MIT License](LICENSE.txt)
+
```

