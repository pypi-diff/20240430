# Comparing `tmp/deadpad-0.1.0.tar.gz` & `tmp/deadpad-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadpad-0.1.0.tar", last modified: Sun Apr 28 08:33:20 2024, max compression
+gzip compressed data, was "deadpad-0.2.0.tar", last modified: Tue Apr 30 06:49:24 2024, max compression
```

## Comparing `deadpad-0.1.0.tar` & `deadpad-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:20.499132 deadpad-0.1.0/
--rw-rw-rw-   0        0        0     1070 2024-04-28 02:53:30.000000 deadpad-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      778 2024-04-28 08:33:20.498128 deadpad-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-28 03:44:03.000000 deadpad-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:20.480128 deadpad-0.1.0/deadpad/
--rw-rw-rw-   0        0        0     6320 2024-04-28 08:22:19.000000 deadpad-0.1.0/deadpad/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:20.491128 deadpad-0.1.0/deadpad/parts/
--rw-rw-rw-   0        0        0        0 2024-04-28 08:06:59.000000 deadpad-0.1.0/deadpad/parts/__init__.py
--rw-rw-rw-   0        0        0     7129 2024-04-28 08:23:52.000000 deadpad-0.1.0/deadpad/parts/document.py
--rw-rw-rw-   0        0        0      933 2024-04-28 08:18:12.000000 deadpad-0.1.0/deadpad/parts/input_handler.py
--rw-rw-rw-   0        0        0      570 2024-04-28 08:18:20.000000 deadpad-0.1.0/deadpad/parts/keys.py
--rw-rw-rw-   0        0        0     1052 2024-04-28 08:15:11.000000 deadpad-0.1.0/deadpad/parts/linux_input.py
--rw-rw-rw-   0        0        0     9515 2024-04-28 08:18:54.000000 deadpad-0.1.0/deadpad/parts/textscreen.py
--rw-rw-rw-   0        0        0      700 2024-04-27 21:52:30.000000 deadpad-0.1.0/deadpad/parts/themes.py
--rw-rw-rw-   0        0        0      947 2024-04-28 08:12:42.000000 deadpad-0.1.0/deadpad/parts/windows_input.py
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:20.492129 deadpad-0.1.0/deadpad/themes/
--rw-rw-rw-   0        0        0      313 2024-04-28 03:29:36.000000 deadpad-0.1.0/deadpad/themes/default.json
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:20.498128 deadpad-0.1.0/deadpad.egg-info/
--rw-rw-rw-   0        0        0      778 2024-04-28 08:33:20.000000 deadpad-0.1.0/deadpad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      497 2024-04-28 08:33:20.000000 deadpad-0.1.0/deadpad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 08:33:20.000000 deadpad-0.1.0/deadpad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-28 08:33:20.000000 deadpad-0.1.0/deadpad.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2024-04-28 08:33:20.000000 deadpad-0.1.0/deadpad.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-28 08:33:20.496128 deadpad-0.1.0/preview/
--rw-rw-rw-   0        0        0  1655531 2024-04-27 07:05:58.000000 deadpad-0.1.0/preview/DeadPad1.gif
--rw-rw-rw-   0        0        0  1224693 2024-04-28 03:41:41.000000 deadpad-0.1.0/preview/deadpad2.gif
--rw-rw-rw-   0        0        0      838 2024-04-28 08:33:04.000000 deadpad-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 08:33:20.499132 deadpad-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.524896 deadpad-0.2.0/
+-rw-rw-rw-   0        0        0     1070 2024-04-28 02:53:30.000000 deadpad-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      861 2024-04-30 06:49:24.523899 deadpad-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-29 00:26:13.000000 deadpad-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.502127 deadpad-0.2.0/deadpad/
+-rw-rw-rw-   0        0        0     6920 2024-04-30 05:56:30.000000 deadpad-0.2.0/deadpad/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.497126 deadpad-0.2.0/deadpad/extensions/
+drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.507130 deadpad-0.2.0/deadpad/extensions/python/
+-rw-rw-rw-   0        0        0    11064 2024-04-30 06:38:35.000000 deadpad-0.2.0/deadpad/extensions/python/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.515125 deadpad-0.2.0/deadpad/parts/
+-rw-rw-rw-   0        0        0        0 2024-04-28 08:06:59.000000 deadpad-0.2.0/deadpad/parts/__init__.py
+-rw-rw-rw-   0        0        0     7263 2024-04-30 06:13:50.000000 deadpad-0.2.0/deadpad/parts/document.py
+-rw-rw-rw-   0        0        0      591 2024-04-30 04:42:56.000000 deadpad-0.2.0/deadpad/parts/extension.py
+-rw-rw-rw-   0        0        0      933 2024-04-28 08:18:12.000000 deadpad-0.2.0/deadpad/parts/input_handler.py
+-rw-rw-rw-   0        0        0      570 2024-04-29 00:26:06.000000 deadpad-0.2.0/deadpad/parts/keys.py
+-rw-rw-rw-   0        0        0     1052 2024-04-28 08:15:11.000000 deadpad-0.2.0/deadpad/parts/linux_input.py
+-rw-rw-rw-   0        0        0    10363 2024-04-30 06:29:28.000000 deadpad-0.2.0/deadpad/parts/textscreen.py
+-rw-rw-rw-   0        0        0      700 2024-04-27 21:52:30.000000 deadpad-0.2.0/deadpad/parts/themes.py
+-rw-rw-rw-   0        0        0      947 2024-04-28 08:12:42.000000 deadpad-0.2.0/deadpad/parts/windows_input.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.516124 deadpad-0.2.0/deadpad/themes/
+-rw-rw-rw-   0        0        0      284 2024-04-30 06:08:03.000000 deadpad-0.2.0/deadpad/themes/default.json
+drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.522897 deadpad-0.2.0/deadpad.egg-info/
+-rw-rw-rw-   0        0        0      861 2024-04-30 06:49:24.000000 deadpad-0.2.0/deadpad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2024-04-30 06:49:24.000000 deadpad-0.2.0/deadpad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 06:49:24.000000 deadpad-0.2.0/deadpad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-30 06:49:24.000000 deadpad-0.2.0/deadpad.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2024-04-30 06:49:24.000000 deadpad-0.2.0/deadpad.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 06:49:24.519124 deadpad-0.2.0/preview/
+-rw-rw-rw-   0        0        0  1655531 2024-04-27 07:05:58.000000 deadpad-0.2.0/preview/DeadPad1.gif
+-rw-rw-rw-   0        0        0  1224693 2024-04-28 03:41:41.000000 deadpad-0.2.0/preview/deadpad2.gif
+-rw-rw-rw-   0        0        0      838 2024-04-30 06:49:05.000000 deadpad-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 06:49:24.524896 deadpad-0.2.0/setup.cfg
```

### Comparing `deadpad-0.1.0/LICENSE` & `deadpad-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deadpad-0.1.0/PKG-INFO` & `deadpad-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 Metadata-Version: 2.1
 Name: deadpad
-Version: 0.1.0
+Version: 0.2.0
 Summary: A customizeable lightweight CLI/TUI text editor made without curses or any TUI framework.
 Author: William L.
 Project-URL: Homepage, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor
 Project-URL: Issues, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DeadPad Text Editor
 
+Install:
+```
+pip install deadpad
+```
+
+Run:
+
+```
+deadpad <filename>
+```
+
 > A command line text editor made without curses or any other TUI library.
 
 ![](https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor/blob/main/preview/deadpad2.gif)
```

### Comparing `deadpad-0.1.0/deadpad/__init__.py` & `deadpad-0.2.0/deadpad/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import datetime
+import importlib
 import os
 import platform
 import sys
+import time
+from types import ModuleType
+from deadpad.parts.extension import Extension
 from deadpad.parts.textscreen import TextScreen
 import shutil
 from deadpad.parts.document import Document
 try:
     from deadpad.parts.windows_input import InputHandler
 except ModuleNotFoundError:
     from deadpad.parts.linux_input import InputHandler
 
 opsys = platform.system()
 
-
-
 class Editor:
     "The main class for the python based CLI text editor Dead Pad"
     def __init__(self) -> None:
         self.in_handler = InputHandler()
         self.term_size = shutil.get_terminal_size()
         self.themes_path = f"{os.path.dirname(__file__)}/themes/"
         self.settings = {
@@ -25,37 +27,48 @@
             "show_paragraphs": False,
             "show_tabs": False,
             "line_numbers": True,
             # General config
             "theme": f"default",
             "tab_replace": "\t",
         }
-        
+        self.extensions:dict[str, Extension] = self.get_extensions()
+
         self.screen = TextScreen(self, self.term_size.columns, self.term_size.lines, Document(self, self.term_size.columns, sys.argv[1]))
+        
+
+    def get_extensions(self):
+        modules:dict[str, Extension] = {}
+        for extension in os.listdir(f"{os.path.dirname(__file__)}/extensions"):
+            modules[extension] = Extension(self, extension, importlib.import_module(f"deadpad.extensions.{extension}"))
+        return modules
 
     def run_command(self, command_str:str):
         tokens = self.get_tokens(command_str)
         if len(tokens) > 0:
             match tokens[0]: # command name
                 case "set": # changes a setting
                     self.settings[tokens[1]] = (val:=self.parse_literal(tokens[2]))
                     self.screen.footer_string = f"Set {tokens[1]} to {repr(val)}"
                 case "toggle": # toggles a setting
                     self.settings[tokens[1]] = not self.settings[tokens[1]]
                 case "exit":
                     self.screen.footer_string = f"EXITING"
                     self.screen.running = False
                 case "save":
-                    self.screen.footer_string = f"Last saved to '{self.screen.document.file_path}' at {datetime.datetime.now()}. 📀"
+                    self.screen.footer_string = f"Last saved '{self.screen.document.file_path[:7]}' at {datetime.datetime.now()}. 📀"
                     self.screen.document.save()
                 case "refresh":
                     self.screen.refresh()
                     self.screen.footer_string = f"Dead Pad Themes, Plugins, and Config refreshed."
                 case "edit":
                     self.screen.open_document(tokens[1])
+                
+                case "ls":
+                    self.screen.footer_string = ", ".join(os.listdir())
                 case _:
                     self.screen.footer_string = f"Unknown command \"{tokens[0]}\""
                     
 
     def parse_literal(self, tok:str):
         if tok == "true":
             return True
@@ -163,12 +176,13 @@
          or term_size.lines != self.term_size.lines\
          or term_size.columns != self.term_size.columns:
             self.term_size = term_size
             clear_str = "\033[F\033[K" * (self.term_size.lines)
             self.screen.render(self.term_size.columns, self.term_size.lines)
             sys.stdout.write(f"{clear_str}{self.screen.render(self.term_size.columns, self.term_size.lines)}")
 
+
 def main():
     editor = Editor()
     editor.run()
 if __name__ == "__main__":
     main()
```

### Comparing `deadpad-0.1.0/deadpad/parts/document.py` & `deadpad-0.2.0/deadpad/parts/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from typing import TYPE_CHECKING
 
 from deadpad.parts import keys
 if TYPE_CHECKING:
     from deadpad.parts.textscreen import TextScreen
     from deadpad import Editor
 
+# TODO Make a property for the state that runs all activated extensions on the code before the state is used by the TextScreen
+
+
 def chrweight(char:str):
     match char:
         case "\t":
             return 3
         case None: # equivalent of space in textscreen
             return 1
         case _:
@@ -110,14 +113,15 @@
         self.file = open(self.file_path, "r+", encoding="utf8")
         t_str_state = self.file.read()
         self.str_state = t_str_state if t_str_state[-1] == "\n" else t_str_state + "\n"
         self.state = newline_chunkstring(self.str_state, self.render_width)
         self.master = master
         self.updated = True
 
+
     def __del__(self):
         self.file.close()
 
     def save(self):
         "Saves the document."
         self.file.seek(0)
         self.file.write(self.str_state)
```

### Comparing `deadpad-0.1.0/deadpad/parts/input_handler.py` & `deadpad-0.2.0/deadpad/parts/input_handler.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.1.0/deadpad/parts/keys.py` & `deadpad-0.2.0/deadpad/parts/keys.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.1.0/deadpad/parts/linux_input.py` & `deadpad-0.2.0/deadpad/parts/linux_input.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.1.0/deadpad/parts/textscreen.py` & `deadpad-0.2.0/deadpad/parts/textscreen.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime
 from enum import Enum
 import json
 import math
 import sys
 import time
 import shutil
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Callable
 from deadpad.parts import keys
 from deadpad.parts.document import Document, str_weight
 from deadpad.parts.themes import RESET_STYLE, get_style
 if TYPE_CHECKING:
     from deadpad import Editor
 
 def move_cursor(y:int, x:int):
@@ -53,14 +53,15 @@
         f_p.close()
         self.updated = True
         
         self.state = [[] for _ in range(self.height)]    
         self.document.render_width = self.width
         self.document.update_state()
         sys.stdout.write("\033c")
+        self.get_extensions()
         
 
     def check_update(self):
         updated = self.updated or self.document.updated
         self.updated = False
         self.document.updated = False
         return updated
@@ -68,14 +69,26 @@
     def open_document(self, path:str):
         self._y_pos = 0
         self.document = Document(self.master, self.width, path)
         self.state = [[] for _ in range(self.height)]
         self.footer_string = self.document.file_path
         sys.stdout.write("\033c")
         self.updated = True
+        self.get_extensions()
+        
+    def get_extensions(self):
+        self.highlight:Callable[[str], str] = lambda src: src
+        "The current active syntax highlighter."
+
+        file_ext = self.document.file_path.split(".")[-1]
+        for extension in self.master.extensions.values():
+            if extension.FILE_EXT == file_ext:
+                if extension.parser:
+                    self.highlight = extension.parser.highlight
+                    
     
     def refresh(self):
         self.theme_data = json.load(f_p:=open(f"{self.master.themes_path}{self.master.settings['theme']}.json", "r", encoding="utf8"))
         f_p.close()
         self.updated = True
 
     @property
@@ -125,55 +138,61 @@
             self.state[ln].extend([None for _ in range(self.width - str_weight(self.state[ln]))])
             ln += 1
             
 
         for y, row in enumerate(self.state):
             if self.master.settings["line_numbers"]:
 
-                screen += f"{get_style(bg=self.theme_data['line_number_bg'])}{(y+self.y_pos+1):^4}{get_style(bg=self.theme_data['editor_bg'])}|"
+                screen += f"{get_style(bg=self.theme_data['line_number_bg'])}{(y+self.y_pos+1):^4}{RESET_STYLE}|"
+            src_line = ""
             for x, col in enumerate(row):
                 if col != None:
                     if y == self.cursor_y and x == self.cursor_x:
                         if col in {'\n', ' '}:
-                            screen += self.theme_data["cursor_sym"]
+                            src_line += self.theme_data["cursor_sym"]
                         elif col == '\t':
-                            screen += self.theme_data["cursor_sym"] + self.theme_data["tab_sym"][1:len(self.theme_data["tab_sym"])] if self.master.settings["show_tabs"] else self.theme_data["cursor_sym"] + (' ' * (len(self.theme_data["tab_sym"])-1))
+                            src_line += self.theme_data["cursor_sym"] + self.theme_data["tab_sym"][1:len(self.theme_data["tab_sym"])] if self.master.settings["show_tabs"] else self.theme_data["cursor_sym"] + (' ' * (len(self.theme_data["tab_sym"])-1))
                         else:
-                            screen += self.theme_data["cursor_sym"] + col
+                            src_line += self.theme_data["cursor_sym"] + col
                     else:
                         match col:
                             case '\n':
-                                screen += self.theme_data["paragraph_sym"] if self.master.settings["show_paragraphs"] else ''
+                                src_line += self.theme_data["paragraph_sym"] if self.master.settings["show_paragraphs"] else ''
 
                             case '\t':
-                                screen += self.theme_data["tab_sym"] if self.master.settings["show_tabs"] else (' ' * len(self.theme_data["tab_sym"]))
-
+                                src_line += self.theme_data["tab_sym"] if self.master.settings["show_tabs"] else (' ' * len(self.theme_data["tab_sym"]))
                             case _:
-                                screen += col
+                                src_line += col
                 elif y == self.cursor_y and x == self.cursor_x:
-                    screen += self.theme_data["cursor_sym"]
-                else:
-                    screen += ' '
+                    src_line += self.theme_data["cursor_sym"]
+            screen += self.highlight(src_line).replace(" ", " ")
             if col != '\n':
                 screen += f'\n{RESET_STYLE}'
 
+        
+
+        # command bar
         bchar = self.theme_data['CLI_bar_filler_char']
         footer_bg = bchar * (self.width - len(self.footer_string)-5)
         padding = ' ' if self.footer_string != "" else ''
+        
         return f"{screen}\033[K{self.theme_data['emblem']} {bchar}{padding}{self.footer_string}{padding}{footer_bg}\n\033[K{' '*self.width}"
-    
+
     def handle_key(self, key:bytes):
         if key != None:
             self.updated = True
         if self.edit_mode:
             self.footer_string = self.document.file_path if self.footer_string in {"COMMAND MODE",self.document.file_path} else self.footer_string
             
             match key:
                 case keys.CTRL_W: # ctrl w
-                    self.footer_string = f"Last saved to '{self.document.file_path}' at {datetime.datetime.now()}. 📀"
+                    # TODO make save message show maximum ammount of characters in file path.
+                    flpw = math.floor(self.width/8)
+                    filep = (self.document.file_path[:flpw]+'...') if len(self.document.file_path) > (flpw+3) else self.document.file_path    
+                    self.footer_string = f"Last saved '{filep}' at {datetime.datetime.now()}. 📀"
                 case keys.ESC: # esc
                     self.footer_string = f"EXITING"
                     self.running = False
                 case b'\n': # enter
                     if self.cursor_y == self.height:
                         self.y_pos += 1
                 case keys.BACKSPACE: # backspace
```

### Comparing `deadpad-0.1.0/deadpad/parts/themes.py` & `deadpad-0.2.0/deadpad/parts/themes.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.1.0/deadpad/parts/windows_input.py` & `deadpad-0.2.0/deadpad/parts/windows_input.py`

 * *Files identical despite different names*

### Comparing `deadpad-0.1.0/deadpad.egg-info/PKG-INFO` & `deadpad-0.2.0/deadpad.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 Metadata-Version: 2.1
 Name: deadpad
-Version: 0.1.0
+Version: 0.2.0
 Summary: A customizeable lightweight CLI/TUI text editor made without curses or any TUI framework.
 Author: William L.
 Project-URL: Homepage, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor
 Project-URL: Issues, https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DeadPad Text Editor
 
+Install:
+```
+pip install deadpad
+```
+
+Run:
+
+```
+deadpad <filename>
+```
+
 > A command line text editor made without curses or any other TUI library.
 
 ![](https://github.com/FrewtyPebbles/DeadPad-CLI-Text-Editor/blob/main/preview/deadpad2.gif)
```

### Comparing `deadpad-0.1.0/preview/DeadPad1.gif` & `deadpad-0.2.0/preview/DeadPad1.gif`

 * *Files identical despite different names*

### Comparing `deadpad-0.1.0/preview/deadpad2.gif` & `deadpad-0.2.0/preview/deadpad2.gif`

 * *Files identical despite different names*

### Comparing `deadpad-0.1.0/pyproject.toml` & `deadpad-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deadpad"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="William L." },
 ]
 description = "A customizeable lightweight CLI/TUI text editor made without curses or any TUI framework."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

