# Comparing `tmp/magictk-1.0.1.59.tar.gz` & `tmp/magictk-1.0.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-1.0.1.59.tar", last modified: Mon Apr 29 13:15:48 2024, max compression
+gzip compressed data, was "magictk-1.0.1.60.tar", last modified: Tue Apr 30 13:33:29 2024, max compression
```

## Comparing `magictk-1.0.1.59.tar` & `magictk-1.0.1.60.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:15:48.112697 magictk-1.0.1.59/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-29 13:15:47.000000 magictk-1.0.1.59/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-29 13:15:48.112697 magictk-1.0.1.59/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1683 2024-04-29 13:15:47.000000 magictk-1.0.1.59/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:15:48.112697 magictk-1.0.1.59/magictk/
--rw-r--r--   0 root         (0) root         (0)      514 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3363 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    17993 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11247 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     2069 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12242 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)     3725 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)     1890 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/icon.py
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/mtk.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5995 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     8106 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/scrollbar.py
--rw-r--r--   0 root         (0) root         (0)     6178 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)      372 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/style.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10245 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:15:48.112697 magictk-1.0.1.59/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      629 2024-04-29 13:15:48.000000 magictk-1.0.1.59/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 13:15:48.112697 magictk-1.0.1.59/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-29 13:15:47.000000 magictk-1.0.1.59/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:33:29.811309 magictk-1.0.1.60/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-30 13:33:29.000000 magictk-1.0.1.60/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-30 13:33:29.807309 magictk-1.0.1.60/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1683 2024-04-30 13:33:29.000000 magictk-1.0.1.60/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:33:29.807309 magictk-1.0.1.60/magictk/
+-rw-r--r--   0 root         (0) root         (0)      514 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    17577 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11247 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12242 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/icon.py
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5995 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     8106 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/scrollbar.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)      372 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/style.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10245 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 13:33:29.807309 magictk-1.0.1.60/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      629 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-30 13:33:29.000000 magictk-1.0.1.60/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 13:33:29.811309 magictk-1.0.1.60/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-30 13:33:29.000000 magictk-1.0.1.60/setup.py
```

### Comparing `magictk-1.0.1.59/PKG-INFO` & `magictk-1.0.1.60/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 1.0.1.59
+Version: 1.0.1.60
 Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-1.0.1.59/README.md` & `magictk-1.0.1.60/README.md`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/__init__.py` & `magictk-1.0.1.60/magictk/__init__.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/_window_ctl.py` & `magictk-1.0.1.60/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/_window_size.py` & `magictk-1.0.1.60/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/basicwindow.py` & `magictk-1.0.1.60/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/button.py` & `magictk-1.0.1.60/magictk/button.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,418 +1,418 @@
-import json
-import tkinter
-from tkinter import ttk
-
-from magictk import color_tmpl
-from magictk import photoload
-from magictk import fontconfig
-
-
-class Button:
-    color = color_tmpl.default_color
-    hover_mode = 0.0
-    _is_hover = 0
-    _flash_t = 0
-    max_flash = 4
-    _anim_obj_id = -1
-    text = "Button"
-
-    def _draw_corner(self, r_x, r_y, x, y, **kwargs):
-        border_info = json.loads(photoload.loadres("buttonborder"))
-        y_n = 0
-        for i in border_info:
-            x_n = 0
-            for j in i:
-                if (r_x == 0):
-                    px = x+x_n+1
-                else:
-                    px = x+4-x_n-1
-                if (r_y == 0):
-                    py = y+y_n+1
-                else:
-                    py = y+4-y_n-1
-                if (j < 0):
-                    lcolor = -j
-                else:
-                    lcolor = j
-                g_color = color_tmpl.mix_color(
-                    self.color["background"], self.color[self._color_bd], int((1-lcolor/255)*1000)/1000)
-                if (j < 0):
-                    f_color = color_tmpl.mix_color(
-                        self.color[self._color_fg2], self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
-                else:
-                    f_color = color_tmpl.mix_color(
-                        self.color["background"], self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
-                if (j < 0):
-                    h_color = color_tmpl.mix_color(
-                        self.color[self._color_fg2], self.color[self._color_fg], int((1-lcolor/255)*1000)/1000)
-                else:
-                    h_color = color_tmpl.mix_color(
-                        self.color["background"], self.color[self._color_fg], int((1-lcolor/255)*1000)/1000)
-
-                obj = self.canvas.create_rectangle(
-                    px, py, px, py, width=0, fill=g_color)
-
-                def update_color(obj, g_color, f_color, h_color):
-                    if (self._is_hover == 2):
-                        self.canvas.itemconfig(
-                            obj, fill=h_color)
-                    else:
-                        self.canvas.itemconfig(
-                            obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
-
-                self._fill_func.append(update_color)
-                self._fill_gc.append(g_color)
-                self._fill_fc.append(f_color)
-                self._fill_hc.append(h_color)
-                self._fill_obj.append(obj)
-                x_n += 1
-            y_n += 1
-
-    def _draw_icon(self, x, y, name, size, **kwargs):
-        border_info = border_info = json.loads(photoload.loadres(
-            f"icon/{name}@{size}"))
-        y_n = 0
-        for i in border_info:
-            x_n = 0
-            for j in i:
-                px = x+y_n+1
-                py = y+x_n+1
-                lcolor = j
-                g_color = color_tmpl.mix_color(
-                    self.color["regular_text"], self.color["background"], int((1-lcolor/255)*1000)/1000)
-                f_color = color_tmpl.mix_color(
-                    self.color[self._color_fg], self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
-                h_color = color_tmpl.mix_color(
-                    self.color[self._color_fg], self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
-
-                obj = self.canvas.create_rectangle(
-                    px, py, px, py, width=0, fill=g_color)
-
-                def update_color(obj, g_color, f_color, h_color):
-                    if (self._is_hover == 2):
-                        self.canvas.itemconfig(
-                            obj, fill=h_color)
-                    else:
-                        self.canvas.itemconfig(
-                            obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
-
-                self._fill_func.append(update_color)
-                self._fill_gc.append(g_color)
-                self._fill_fc.append(f_color)
-                self._fill_hc.append(h_color)
-                self._fill_obj.append(obj)
-                x_n += 1
-            y_n += 1
-
-    def _update_color(self):
-        n = 0
-        for i in self._fill_func:
-            i(self._fill_obj[n], self._fill_gc[n],
-              self._fill_fc[n], self._fill_hc[n])
-            n += 1
-
-    def __init__(self, master=None, root_anim=None, w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _set_defaultcolor=None, iconname="", iconsize=24):
-        global use_font
-        use_font = fontconfig.getfont()
-        self._fill_obj = []
-        self._fill_func = []
-        self._fill_gc = []
-        self._fill_fc = []
-        self._fill_hc = []
-        self._func = func
-        if (_set_defaultcolor is None):
-            self._color_bd = "border_base"
-            self._color_bg = "background"
-            self._color_bg1 = "background"
-            self._color_fg = "primary"
-            self._color_fg1 = "primary_light"
-            self._color_fg2 = "primary_light2"
-            self._color_fg3 = "primary_light2"
-            self._color_text = None
-        self.w = max(30, w)
-        self.h = h
-        self.text = text
-        self.__master = master
-        if (color_list is not None):
-            self.color = color_list
-        if (root_anim == None):
-            self.root = master.root
-        else:
-            self.root = root_anim
-
-        self.canvas = tkinter.Canvas(
-            master, bg=self.color["background"], width=self.w, height=self.h, borderwidth=0, bd=0, highlightcolor=self.color["background"], highlightthickness=0)
-
-        if (iconname != ''):
-            self.text = ""
-        self._draw()
-        if (iconname != ''):
-            self.size = iconsize
-            self._draw_icon(self.w//2-self.size//2, self.h //
-                            2-self.size//2, iconname, iconsize)
-        self._update_color()
-        self._bind_event()
-        self.bind_anim()
-
-        for event, eventfunc in master.p_event_list:
-            self.canvas.bind(event, eventfunc)
-
-    def pack(self, *args, **kwargs):
-        self.canvas.pack(*args, **kwargs)
-
-    def grid(self, *args, **kwargs):
-        self.canvas.grid(*args, **kwargs)
-
-    def place(self, *args, **kwargs):
-        self.canvas.place(*args, **kwargs)
-
-    def _draw(self, _use_self_text=None):
-        self._draw_corner(0, 0, 0, 0)
-        self._draw_corner(1, 0, self.w-4, 0)
-        self._draw_corner(0, 1, 0, self.h-5)
-        self._draw_corner(1, 1, self.w-4, self.h-5)
-
-        def update_color(obj, g_color, f_color, h_color):
-            if (self._is_hover == 2):
-                self.canvas.itemconfig(
-                    obj, fill=h_color)
-            else:
-                self.canvas.itemconfig(
-                    obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
-        self._fill_fc.append(self.color[self._color_fg1])
-        self._fill_gc.append(self.color[self._color_bd])
-        self._fill_hc.append(self.color[self._color_fg])
-        self._fill_func.append(update_color)
-        self._fill_obj.append(self.canvas.create_line(
-            1, 5, 1, self.h-5, width=1, fill=self.color[self._color_bd]))
-        self._fill_fc.append(self.color[self._color_fg1])
-        self._fill_gc.append(self.color[self._color_bd])
-        self._fill_hc.append(self.color[self._color_fg])
-        self._fill_func.append(update_color)
-        self._fill_obj.append(self.canvas.create_line(
-            5, 1, self.w-4, 1, width=1, fill=self.color[self._color_fg1]))
-        self._fill_fc.append(self.color[self._color_fg1])
-        self._fill_gc.append(self.color[self._color_bd])
-        self._fill_hc.append(self.color[self._color_fg])
-        self._fill_func.append(update_color)
-        self._fill_obj.append(self.canvas.create_line(
-            self.w-1, 5, self.w-1, self.h-5, width=1, fill=self.color[self._color_fg1]))
-        self._fill_fc.append(self.color[self._color_fg1])
-        self._fill_gc.append(self.color[self._color_bd])
-        self._fill_hc.append(self.color[self._color_fg])
-        self._fill_func.append(update_color)
-        self._fill_obj.append(self.canvas.create_line(
-            5, self.h-2, self.w-4, self.h-2, width=1, fill=self.color[self._color_fg1]))
-
-        self._fill_fc.append(self.color[self._color_fg3])
-        self._fill_gc.append(self.color[self._color_bg1])
-        self._fill_hc.append(self.color[self._color_fg2])
-        self._fill_func.append(update_color)
-        self._fill_obj.append(self.canvas.create_rectangle(
-            2, 5, self.w-1, self.h-5, width=0, fill=self.color[self._color_fg2]))
-
-        self._fill_fc.append(self.color[self._color_fg3])
-        self._fill_gc.append(self.color[self._color_bg1])
-        self._fill_hc.append(self.color[self._color_fg2])
-        self._fill_func.append(update_color)
-        self._fill_obj.append(self.canvas.create_rectangle(
-            5, 2, self.w-4, self.h-2, width=0, fill=self.color[self._color_fg2]))
-
-        if (_use_self_text is None):
-            if (self._color_text is None):
-                self._fill_fc.append(self.color[self._color_fg])
-                self._fill_gc.append(self.color["regular_text"])
-                self._fill_hc.append(self.color[self._color_fg])
-            else:
-                self._fill_fc.append(self._color_text)
-                self._fill_gc.append(self._color_text)
-                self._fill_hc.append(self._color_text)
-            self._fill_func.append(update_color)
-            self._fill_obj.append(
-                self.canvas.create_text(int(self.w/2), int(self.h/2), text=self.text, font=(use_font, 10)))
-
-    def bind_anim(self):
-        def anim_magictk():
-            if (self._is_hover == 1 and self._flash_t < self.max_flash):
-                self._flash_t += (1 if (len(self.root.anim) > 6) else 1)
-                self._flash_t = min(self._flash_t, self.max_flash)
-                self.hover_mode = self._flash_t/self.max_flash
-                self._update_color()
-            elif (self._is_hover == 0 and self._flash_t > 0):
-                self._flash_t -= (1 if (len(self.root.anim) > 6) else 1)
-                self._flash_t = max(self._flash_t, 0)
-                self.hover_mode = self._flash_t/self.max_flash
-                self._update_color()
-            else:
-                return -1
-
-        def anim_normal(*args):
-            if (self._is_hover == 1 and self._flash_t < self.max_flash):
-                self._flash_t += 1
-                self.hover_mode = self._flash_t/self.max_flash
-                self._update_color()
-            elif (self._is_hover == 0 and self._flash_t > 0):
-                self._flash_t -= 1
-                self.hover_mode = self._flash_t/self.max_flash
-                self._update_color()
-            self.root.after(anim_normal, 16)
-
-        try:
-            self.root.anim == 0
-        except:
-            self.root.after(anim_normal, 16)
-        else:
-            if (anim_magictk not in self.root.anim):
-                self.root.anim.append(anim_magictk)
-                self._anim_obj_id = self.root.anim[-1]
-
-    def _bind_event(self):
-        def enter_v(*args):
-            self.bind_anim()
-            if (self._is_hover == 0):
-                self._is_hover = 1
-        self.canvas.bind("<Enter>", enter_v)
-
-        def leave_v(*args):
-            self.bind_anim()
-            if (self._is_hover == 1):
-                self._is_hover = 0
-        self.canvas.bind("<Leave>", leave_v)
-
-        def press_v(*args):
-            self._is_hover = 2
-            self._update_color()
-        self.canvas.bind("<Button-1>", press_v)
-
-        def pressrelease_v(*args):
-            self.bind_anim()
-            self._is_hover = 1
-            self._func(self)
-            self._update_color()
-        self.canvas.bind("<ButtonRelease-1>", pressrelease_v)
-
-
-class ButtonFill(Button):
-
-    def _draw_icon(self, x, y, name, size, **kwargs):
-        border_info = border_info = json.loads(photoload.loadres(
-            f"icon/{name}@{size}"))
-        y_n = 0
-        for i in border_info:
-            x_n = 0
-            for j in i:
-                px = x+y_n+1
-                py = y+x_n+1
-                lcolor = j
-                g_color = color_tmpl.mix_color(
-                    self._color_text, self.color[self._color_bd], int((1-lcolor/255)*1000)/1000)
-                f_color = color_tmpl.mix_color(
-                    self._color_text, self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
-                h_color = color_tmpl.mix_color(
-                    self._color_text, self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
-
-                obj = self.canvas.create_rectangle(
-                    px, py, px, py, width=0, fill=g_color)
-
-                def update_color(obj, g_color, f_color, h_color):
-                    if (self._is_hover == 2):
-                        self.canvas.itemconfig(
-                            obj, fill=h_color)
-                    else:
-                        self.canvas.itemconfig(
-                            obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
-
-                self._fill_func.append(update_color)
-                self._fill_gc.append(g_color)
-                self._fill_fc.append(f_color)
-                self._fill_hc.append(h_color)
-                self._fill_obj.append(obj)
-                x_n += 1
-            y_n += 1
-
-    def _draw_corner(self, r_x, r_y, x, y, **kwargs):
-        border_info = json.loads(photoload.loadres("buttonborder"))
-        y_n = 0
-        for i in border_info:
-            x_n = 0
-            for j in i:
-                if (r_x == 0):
-                    px = x+x_n+1
-                else:
-                    px = x+4-x_n-1
-                if (r_y == 0):
-                    py = y+y_n+1
-                else:
-                    py = y+4-y_n-1
-                if (j < 0):
-                    lcolor = -j
-                else:
-                    lcolor = j
-                if (j < 0):
-                    g_color = color_tmpl.mix_color(
-                        self.color[self._color_bg], self.color[self._color_bd], int((1-lcolor/255)*1000)/1000)
-                else:
-                    g_color = color_tmpl.mix_color(
-                        self.color["background"], self.color[self._color_bd], int((1-lcolor/255)*1000)/1000)
-                if (j < 0):
-                    f_color = color_tmpl.mix_color(
-                        self.color[self._color_fg1], self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
-                else:
-                    f_color = color_tmpl.mix_color(
-                        self.color["background"], self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
-                if (j < 0):
-                    h_color = color_tmpl.mix_color(
-                        self.color[self._color_fg2], self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
-                else:
-                    h_color = color_tmpl.mix_color(
-                        self.color["background"], self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
-
-                obj = self.canvas.create_rectangle(
-                    px, py, px, py, width=0, fill=g_color)
-
-                def update_color(obj, g_color, f_color, h_color):
-                    if (self._is_hover == 2):
-                        self.canvas.itemconfig(
-                            obj, fill=h_color)
-                    else:
-                        self.canvas.itemconfig(
-                            obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
-
-                self._fill_func.append(update_color)
-                self._fill_gc.append(g_color)
-                self._fill_fc.append(f_color)
-                self._fill_hc.append(h_color)
-                self._fill_obj.append(obj)
-                x_n += 1
-            y_n += 1
-
-    def __init__(self, master=None, root_anim=None, color_type="plain", w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _dis_color=None, iconname="", iconsize=24):
-        if (_dis_color is None):
-            self._color_bd = color_type
-            self._color_bg = color_type
-            self._color_bg1 = color_type
-            self._color_fg1 = color_type+"_light3"
-            self._color_fg = color_type+"_dark"
-            self._color_fg3 = color_type+"_light3"
-            self._color_fg2 = color_type+"_dark"
-            self._color_text = "#FFFFFF"
-        super().__init__(master=master, root_anim=root_anim, w=w, h=h,
-                         text=text, color_list=color_list, func=func, _set_defaultcolor=True, iconname=iconname, iconsize=iconsize)
-
-
-class ButtonLight(ButtonFill):
-
-    def __init__(self, master=None, root_anim=None, color_type="plain", w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _dis_color=None, iconname="", iconsize=24):
-        if (color_list is not None):
-            self.color = color_list
-        if (_dis_color is None):
-            self._color_bd = "background"
-            self._color_bg = "background"
-            self._color_bg1 = "background"
-            self._color_fg1 = "placeholder_light"
-            self._color_fg = "border_light"
-            self._color_fg3 = "placeholder_light"
-            self._color_fg2 = "border_light"
-            self._color_text = self.color[color_type]
-        super().__init__(master=master, root_anim=root_anim, w=w, h=h,
-                         text=text, color_list=color_list, func=func, _dis_color=True, iconname=iconname, iconsize=iconsize)
+import json
+import tkinter
+from tkinter import ttk
+
+from magictk import color_tmpl
+from magictk import photoload
+from magictk import fontconfig
+
+
+class Button:
+    color = color_tmpl.default_color
+    hover_mode = 0.0
+    _is_hover = 0
+    _flash_t = 0
+    max_flash = 4
+    _anim_obj_id = -1
+    text = "Button"
+
+    def _draw_corner(self, r_x, r_y, x, y, **kwargs):
+        border_info = json.loads(photoload.loadres("buttonborder"))
+        y_n = 0
+        for i in border_info:
+            x_n = 0
+            for j in i:
+                if (r_x == 0):
+                    px = x+x_n+1
+                else:
+                    px = x+4-x_n-1
+                if (r_y == 0):
+                    py = y+y_n+1
+                else:
+                    py = y+4-y_n-1
+                if (j < 0):
+                    lcolor = -j
+                else:
+                    lcolor = j
+                g_color = color_tmpl.mix_color(
+                    self.color["background"], self.color[self._color_bd], int((1-lcolor/255)*1000)/1000)
+                if (j < 0):
+                    f_color = color_tmpl.mix_color(
+                        self.color[self._color_fg2], self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
+                else:
+                    f_color = color_tmpl.mix_color(
+                        self.color["background"], self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
+                if (j < 0):
+                    h_color = color_tmpl.mix_color(
+                        self.color[self._color_fg2], self.color[self._color_fg], int((1-lcolor/255)*1000)/1000)
+                else:
+                    h_color = color_tmpl.mix_color(
+                        self.color["background"], self.color[self._color_fg], int((1-lcolor/255)*1000)/1000)
+
+                obj = self.canvas.create_rectangle(
+                    px, py, px, py, width=0, fill=g_color)
+
+                def update_color(obj, g_color, f_color, h_color):
+                    if (self._is_hover == 2):
+                        self.canvas.itemconfig(
+                            obj, fill=h_color)
+                    else:
+                        self.canvas.itemconfig(
+                            obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
+
+                self._fill_func.append(update_color)
+                self._fill_gc.append(g_color)
+                self._fill_fc.append(f_color)
+                self._fill_hc.append(h_color)
+                self._fill_obj.append(obj)
+                x_n += 1
+            y_n += 1
+
+    def _draw_icon(self, x, y, name, size, **kwargs):
+        border_info = border_info = json.loads(photoload.loadres(
+            f"icon/{name}@{size}"))
+        y_n = 0
+        for i in border_info:
+            x_n = 0
+            for j in i:
+                px = x+y_n+1
+                py = y+x_n+1
+                lcolor = j
+                g_color = color_tmpl.mix_color(
+                    self.color["regular_text"], self.color["background"], int((1-lcolor/255)*1000)/1000)
+                f_color = color_tmpl.mix_color(
+                    self.color[self._color_fg], self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
+                h_color = color_tmpl.mix_color(
+                    self.color[self._color_fg], self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
+
+                obj = self.canvas.create_rectangle(
+                    px, py, px, py, width=0, fill=g_color)
+
+                def update_color(obj, g_color, f_color, h_color):
+                    if (self._is_hover == 2):
+                        self.canvas.itemconfig(
+                            obj, fill=h_color)
+                    else:
+                        self.canvas.itemconfig(
+                            obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
+
+                self._fill_func.append(update_color)
+                self._fill_gc.append(g_color)
+                self._fill_fc.append(f_color)
+                self._fill_hc.append(h_color)
+                self._fill_obj.append(obj)
+                x_n += 1
+            y_n += 1
+
+    def _update_color(self):
+        n = 0
+        for i in self._fill_func:
+            i(self._fill_obj[n], self._fill_gc[n],
+              self._fill_fc[n], self._fill_hc[n])
+            n += 1
+
+    def __init__(self, master=None, root_anim=None, w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _set_defaultcolor=None, iconname="", iconsize=24):
+        global use_font
+        use_font = fontconfig.getfont()
+        self._fill_obj = []
+        self._fill_func = []
+        self._fill_gc = []
+        self._fill_fc = []
+        self._fill_hc = []
+        self._func = func
+        if (_set_defaultcolor is None):
+            self._color_bd = "border_base"
+            self._color_bg = "background"
+            self._color_bg1 = "background"
+            self._color_fg = "primary"
+            self._color_fg1 = "primary_light"
+            self._color_fg2 = "primary_light2"
+            self._color_fg3 = "primary_light2"
+            self._color_text = None
+        self.w = max(30, w)
+        self.h = h
+        self.text = text
+        self.__master = master
+        if (color_list is not None):
+            self.color = color_list
+        if (root_anim == None):
+            self.root = master.root
+        else:
+            self.root = root_anim
+
+        self.canvas = tkinter.Canvas(
+            master, bg=self.color["background"], width=self.w, height=self.h, borderwidth=0, bd=0, highlightcolor=self.color["background"], highlightthickness=0)
+
+        if (iconname != ''):
+            self.text = ""
+        self._draw()
+        if (iconname != ''):
+            self.size = iconsize
+            self._draw_icon(self.w//2-self.size//2, self.h //
+                            2-self.size//2, iconname, iconsize)
+        self._update_color()
+        self._bind_event()
+        self.bind_anim()
+
+        for event, eventfunc in master.p_event_list:
+            self.canvas.bind(event, eventfunc)
+
+    def pack(self, *args, **kwargs):
+        self.canvas.pack(*args, **kwargs)
+
+    def grid(self, *args, **kwargs):
+        self.canvas.grid(*args, **kwargs)
+
+    def place(self, *args, **kwargs):
+        self.canvas.place(*args, **kwargs)
+
+    def _draw(self, _use_self_text=None):
+        self._draw_corner(0, 0, 0, 0)
+        self._draw_corner(1, 0, self.w-4, 0)
+        self._draw_corner(0, 1, 0, self.h-5)
+        self._draw_corner(1, 1, self.w-4, self.h-5)
+
+        def update_color(obj, g_color, f_color, h_color):
+            if (self._is_hover == 2):
+                self.canvas.itemconfig(
+                    obj, fill=h_color)
+            else:
+                self.canvas.itemconfig(
+                    obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
+        self._fill_fc.append(self.color[self._color_fg1])
+        self._fill_gc.append(self.color[self._color_bd])
+        self._fill_hc.append(self.color[self._color_fg])
+        self._fill_func.append(update_color)
+        self._fill_obj.append(self.canvas.create_line(
+            1, 5, 1, self.h-5, width=1, fill=self.color[self._color_bd]))
+        self._fill_fc.append(self.color[self._color_fg1])
+        self._fill_gc.append(self.color[self._color_bd])
+        self._fill_hc.append(self.color[self._color_fg])
+        self._fill_func.append(update_color)
+        self._fill_obj.append(self.canvas.create_line(
+            5, 1, self.w-4, 1, width=1, fill=self.color[self._color_fg1]))
+        self._fill_fc.append(self.color[self._color_fg1])
+        self._fill_gc.append(self.color[self._color_bd])
+        self._fill_hc.append(self.color[self._color_fg])
+        self._fill_func.append(update_color)
+        self._fill_obj.append(self.canvas.create_line(
+            self.w-1, 5, self.w-1, self.h-5, width=1, fill=self.color[self._color_fg1]))
+        self._fill_fc.append(self.color[self._color_fg1])
+        self._fill_gc.append(self.color[self._color_bd])
+        self._fill_hc.append(self.color[self._color_fg])
+        self._fill_func.append(update_color)
+        self._fill_obj.append(self.canvas.create_line(
+            5, self.h-2, self.w-4, self.h-2, width=1, fill=self.color[self._color_fg1]))
+
+        self._fill_fc.append(self.color[self._color_fg3])
+        self._fill_gc.append(self.color[self._color_bg1])
+        self._fill_hc.append(self.color[self._color_fg2])
+        self._fill_func.append(update_color)
+        self._fill_obj.append(self.canvas.create_rectangle(
+            2, 5, self.w-1, self.h-5, width=0, fill=self.color[self._color_fg2]))
+
+        self._fill_fc.append(self.color[self._color_fg3])
+        self._fill_gc.append(self.color[self._color_bg1])
+        self._fill_hc.append(self.color[self._color_fg2])
+        self._fill_func.append(update_color)
+        self._fill_obj.append(self.canvas.create_rectangle(
+            5, 2, self.w-4, self.h-2, width=0, fill=self.color[self._color_fg2]))
+
+        if (_use_self_text is None):
+            if (self._color_text is None):
+                self._fill_fc.append(self.color[self._color_fg])
+                self._fill_gc.append(self.color["regular_text"])
+                self._fill_hc.append(self.color[self._color_fg])
+            else:
+                self._fill_fc.append(self._color_text)
+                self._fill_gc.append(self._color_text)
+                self._fill_hc.append(self._color_text)
+            self._fill_func.append(update_color)
+            self._fill_obj.append(
+                self.canvas.create_text(int(self.w/2), int(self.h/2), text=self.text, font=(use_font, 10)))
+
+    def bind_anim(self):
+        def anim_magictk():
+            if (self._is_hover == 1 and self._flash_t < self.max_flash):
+                self._flash_t += (1 if (len(self.root.anim) > 6) else 1)
+                self._flash_t = min(self._flash_t, self.max_flash)
+                self.hover_mode = self._flash_t/self.max_flash
+                self._update_color()
+            elif (self._is_hover == 0 and self._flash_t > 0):
+                self._flash_t -= (1 if (len(self.root.anim) > 6) else 1)
+                self._flash_t = max(self._flash_t, 0)
+                self.hover_mode = self._flash_t/self.max_flash
+                self._update_color()
+            else:
+                return -1
+
+        def anim_normal(*args):
+            if (self._is_hover == 1 and self._flash_t < self.max_flash):
+                self._flash_t += 1
+                self.hover_mode = self._flash_t/self.max_flash
+                self._update_color()
+            elif (self._is_hover == 0 and self._flash_t > 0):
+                self._flash_t -= 1
+                self.hover_mode = self._flash_t/self.max_flash
+                self._update_color()
+            self.root.after(anim_normal, 16)
+
+        try:
+            self.root.anim == 0
+        except:
+            self.root.after(anim_normal, 16)
+        else:
+            if (anim_magictk not in self.root.anim):
+                self.root.anim.append(anim_magictk)
+                self._anim_obj_id = self.root.anim[-1]
+
+    def _bind_event(self):
+        def enter_v(*args):
+            self.bind_anim()
+            if (self._is_hover == 0):
+                self._is_hover = 1
+        self.canvas.bind("<Enter>", enter_v)
+
+        def leave_v(*args):
+            self.bind_anim()
+            if (self._is_hover == 1):
+                self._is_hover = 0
+        self.canvas.bind("<Leave>", leave_v)
+
+        def press_v(*args):
+            self._is_hover = 2
+            self._update_color()
+        self.canvas.bind("<Button-1>", press_v)
+
+        def pressrelease_v(*args):
+            self.bind_anim()
+            self._is_hover = 1
+            self._func(self)
+            self._update_color()
+        self.canvas.bind("<ButtonRelease-1>", pressrelease_v)
+
+
+class ButtonFill(Button):
+
+    def _draw_icon(self, x, y, name, size, **kwargs):
+        border_info = border_info = json.loads(photoload.loadres(
+            f"icon/{name}@{size}"))
+        y_n = 0
+        for i in border_info:
+            x_n = 0
+            for j in i:
+                px = x+y_n+1
+                py = y+x_n+1
+                lcolor = j
+                g_color = color_tmpl.mix_color(
+                    self._color_text, self.color[self._color_bd], int((1-lcolor/255)*1000)/1000)
+                f_color = color_tmpl.mix_color(
+                    self._color_text, self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
+                h_color = color_tmpl.mix_color(
+                    self._color_text, self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
+
+                obj = self.canvas.create_rectangle(
+                    px, py, px, py, width=0, fill=g_color)
+
+                def update_color(obj, g_color, f_color, h_color):
+                    if (self._is_hover == 2):
+                        self.canvas.itemconfig(
+                            obj, fill=h_color)
+                    else:
+                        self.canvas.itemconfig(
+                            obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
+
+                self._fill_func.append(update_color)
+                self._fill_gc.append(g_color)
+                self._fill_fc.append(f_color)
+                self._fill_hc.append(h_color)
+                self._fill_obj.append(obj)
+                x_n += 1
+            y_n += 1
+
+    def _draw_corner(self, r_x, r_y, x, y, **kwargs):
+        border_info = json.loads(photoload.loadres("buttonborder"))
+        y_n = 0
+        for i in border_info:
+            x_n = 0
+            for j in i:
+                if (r_x == 0):
+                    px = x+x_n+1
+                else:
+                    px = x+4-x_n-1
+                if (r_y == 0):
+                    py = y+y_n+1
+                else:
+                    py = y+4-y_n-1
+                if (j < 0):
+                    lcolor = -j
+                else:
+                    lcolor = j
+                if (j < 0):
+                    g_color = color_tmpl.mix_color(
+                        self.color[self._color_bg], self.color[self._color_bd], int((1-lcolor/255)*1000)/1000)
+                else:
+                    g_color = color_tmpl.mix_color(
+                        self.color["background"], self.color[self._color_bd], int((1-lcolor/255)*1000)/1000)
+                if (j < 0):
+                    f_color = color_tmpl.mix_color(
+                        self.color[self._color_fg1], self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
+                else:
+                    f_color = color_tmpl.mix_color(
+                        self.color["background"], self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
+                if (j < 0):
+                    h_color = color_tmpl.mix_color(
+                        self.color[self._color_fg2], self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
+                else:
+                    h_color = color_tmpl.mix_color(
+                        self.color["background"], self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
+
+                obj = self.canvas.create_rectangle(
+                    px, py, px, py, width=0, fill=g_color)
+
+                def update_color(obj, g_color, f_color, h_color):
+                    if (self._is_hover == 2):
+                        self.canvas.itemconfig(
+                            obj, fill=h_color)
+                    else:
+                        self.canvas.itemconfig(
+                            obj, fill=color_tmpl.mix_color(g_color, f_color, self.hover_mode))
+
+                self._fill_func.append(update_color)
+                self._fill_gc.append(g_color)
+                self._fill_fc.append(f_color)
+                self._fill_hc.append(h_color)
+                self._fill_obj.append(obj)
+                x_n += 1
+            y_n += 1
+
+    def __init__(self, master=None, root_anim=None, color_type="primary", w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _dis_color=None, iconname="", iconsize=24):
+        if (_dis_color is None):
+            self._color_bd = color_type
+            self._color_bg = color_type
+            self._color_bg1 = color_type
+            self._color_fg1 = color_type+"_light3"
+            self._color_fg = color_type+"_dark"
+            self._color_fg3 = color_type+"_light3"
+            self._color_fg2 = color_type+"_dark"
+            self._color_text = "#FFFFFF"
+        super().__init__(master=master, root_anim=root_anim, w=w, h=h,
+                         text=text, color_list=color_list, func=func, _set_defaultcolor=True, iconname=iconname, iconsize=iconsize)
+
+
+class ButtonLight(ButtonFill):
+
+    def __init__(self, master=None, root_anim=None, color_type="plain", w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _dis_color=None, iconname="", iconsize=24):
+        if (color_list is not None):
+            self.color = color_list
+        if (_dis_color is None):
+            self._color_bd = "background"
+            self._color_bg = "background"
+            self._color_bg1 = "background"
+            self._color_fg1 = "placeholder_light"
+            self._color_fg = "border_light"
+            self._color_fg3 = "placeholder_light"
+            self._color_fg2 = "border_light"
+            self._color_text = self.color[color_type]
+        super().__init__(master=master, root_anim=root_anim, w=w, h=h,
+                         text=text, color_list=color_list, func=func, _dis_color=True, iconname=iconname, iconsize=iconsize)
```

### Comparing `magictk-1.0.1.59/magictk/checkbox.py` & `magictk-1.0.1.60/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/color_tmpl.py` & `magictk-1.0.1.60/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/entry.py` & `magictk-1.0.1.60/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/fontconfig.py` & `magictk-1.0.1.60/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/frame.py` & `magictk-1.0.1.60/magictk/frame.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/icon.ico` & `magictk-1.0.1.60/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/icon.py` & `magictk-1.0.1.60/magictk/icon.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/photoload.py` & `magictk-1.0.1.60/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/progressbar.py` & `magictk-1.0.1.60/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/res.pickle` & `magictk-1.0.1.60/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/scrollbar.py` & `magictk-1.0.1.60/magictk/scrollbar.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/select.py` & `magictk-1.0.1.60/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/submenu.py` & `magictk-1.0.1.60/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/window.py` & `magictk-1.0.1.60/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk/workspace.py` & `magictk-1.0.1.60/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/magictk.egg-info/PKG-INFO` & `magictk-1.0.1.60/magictk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 1.0.1.59
+Version: 1.0.1.60
 Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-1.0.1.59/magictk.egg-info/SOURCES.txt` & `magictk-1.0.1.60/magictk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.59/setup.py` & `magictk-1.0.1.60/setup.py`

 * *Files identical despite different names*

