# Comparing `tmp/dfpyre-0.6.0.tar.gz` & `tmp/dfpyre-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfpyre-0.6.0.tar", max compression
+gzip compressed data, was "dfpyre-0.6.1.tar", max compression
```

## Comparing `dfpyre-0.6.0.tar` & `dfpyre-0.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1060 2024-04-17 21:20:51.864329 dfpyre-0.6.0/LICENSE
--rw-r--r--   0        0        0    10665 2024-04-18 01:13:01.761353 dfpyre-0.6.0/README.md
--rw-r--r--   0        0        0       25 2024-02-25 02:05:19.117008 dfpyre-0.6.0/dfpyre/__init__.py
--rw-r--r--   0        0        0    30347 2024-02-25 02:05:19.117008 dfpyre-0.6.0/dfpyre/data/data.json
--rw-r--r--   0        0        0     9215 2024-04-17 20:33:13.377155 dfpyre-0.6.0/dfpyre/items.py
--rw-r--r--   0        0        0    16970 2024-04-17 20:38:50.169866 dfpyre-0.6.0/dfpyre/pyre.py
--rw-r--r--   0        0        0     5450 2024-04-17 20:34:34.634288 dfpyre-0.6.0/dfpyre/scriptgen.py
--rw-r--r--   0        0        0      980 2024-03-22 02:24:32.576925 dfpyre-0.6.0/dfpyre/style.py
--rw-r--r--   0        0        0      488 2024-04-18 00:35:46.594471 dfpyre-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    11344 1970-01-01 00:00:00.000000 dfpyre-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-17 21:20:51.864329 dfpyre-0.6.1/LICENSE
+-rw-r--r--   0        0        0    10665 2024-04-18 01:13:01.761353 dfpyre-0.6.1/README.md
+-rw-r--r--   0        0        0       25 2024-02-25 02:05:19.117008 dfpyre-0.6.1/dfpyre/__init__.py
+-rw-r--r--   0        0        0    30347 2024-02-25 02:05:19.117008 dfpyre-0.6.1/dfpyre/data/data.json
+-rw-r--r--   0        0        0     9215 2024-04-17 20:33:13.377155 dfpyre-0.6.1/dfpyre/items.py
+-rw-r--r--   0        0        0    17616 2024-04-30 02:52:18.917313 dfpyre-0.6.1/dfpyre/pyre.py
+-rw-r--r--   0        0        0     5568 2024-04-25 01:07:44.479352 dfpyre-0.6.1/dfpyre/scriptgen.py
+-rw-r--r--   0        0        0      980 2024-03-22 02:24:32.576925 dfpyre-0.6.1/dfpyre/style.py
+-rw-r--r--   0        0        0      488 2024-04-30 02:52:59.545769 dfpyre-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    11344 1970-01-01 00:00:00.000000 dfpyre-0.6.1/PKG-INFO
```

### Comparing `dfpyre-0.6.0/LICENSE` & `dfpyre-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dfpyre-0.6.0/README.md` & `dfpyre-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dfpyre-0.6.0/dfpyre/data/data.json` & `dfpyre-0.6.1/dfpyre/data/data.json`

 * *Files identical despite different names*

### Comparing `dfpyre-0.6.0/dfpyre/items.py` & `dfpyre-0.6.1/dfpyre/items.py`

 * *Files identical despite different names*

### Comparing `dfpyre-0.6.0/dfpyre/pyre.py` & `dfpyre-0.6.1/dfpyre/pyre.py`

 * *Files 9% similar despite different names*

```diff
@@ -222,16 +222,14 @@
         'hypercube:pyre_creation_timestamp': now.timestamp()
     }
     template_item.set_tag('PublicBukkitValues', pbv_tag, raw=True)
 
     return template_item
 
 
-# TODO: 
-# - add inserting codeblocks at any index
 class DFTemplate:
     """
     Represents a DiamondFire code template.
     """
     def __init__(self, name: str=None, author: str='pyre'):
         self.codeblocks: List[CodeBlock] = []
         self.bracket_stack: list[str] = []
@@ -302,170 +300,174 @@
         template_dict = {'blocks': template_dict_blocks}
         first_block = template_dict_blocks[0]
         if first_block['block'] not in TEMPLATE_STARTERS:
             _warn('Template does not start with an event, function, or process.')
 
         self._set_template_name(first_block)
 
-        print(f'{COL_SUCCESS}Template built successfully.{COL_RESET}')
-
         json_string = json.dumps(template_dict, separators=(',', ':'))
         return _df_encode(json_string)
     
 
-    def build_and_send(self, method: Literal['recode', 'codeclient'], includeTags: bool=True) -> int:
+    def build_and_send(self, method: Literal['recode', 'codeclient'], include_tags: bool=True) -> int:
         """
         Builds this template and sends it to DiamondFire automatically.
         
-        :param bool includeTags: If True, include item tags in code blocks. Otherwise omit them.
+        :param bool include_tags: If True, include item tags in code blocks. Otherwise omit them.
         """
-        templateCode = self.build(includeTags)
-        templateItem = _get_template_item(templateCode, self.name, self.author)
-        return templateItem.send_to_minecraft(method, 'pyre')
+        template_code = self.build(include_tags)
+        template_item = _get_template_item(template_code, self.name, self.author)
+        return template_item.send_to_minecraft(method, 'pyre')
     
 
     def clear(self):
         """
         Clears this template's data.
         """
         self.__init__()
     
 
-    def _openbracket(self, btype: Literal['norm', 'repeat']='norm'):
+    def _add_codeblock(self, codeblock: CodeBlock, index: int|None):
+        if index is None:
+            self.codeblocks.append(codeblock)
+        else:
+            self.codeblocks.insert(index, codeblock)
+    
+
+    def _openbracket(self, index: int|None, btype: Literal['norm', 'repeat']='norm'):
         bracket = CodeBlock('bracket', data={'id': 'bracket', 'direct': 'open', 'type': btype})
-        self.codeblocks.append(bracket)
+        self._add_codeblock(bracket, index+1)
         self.bracket_stack.append(btype)
     
 
     # command methods
-    def player_event(self, name: str):
+    def player_event(self, name: str, index: int|None=None):
         cmd = CodeBlock(name, data={'id': 'block', 'block': 'event', 'action': name})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
     
 
-    def entity_event(self, name: str):
+    def entity_event(self, name: str, index: int|None=None):
         cmd = CodeBlock(name, data={'id': 'block', 'block': 'entity_event', 'action': name})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
     
 
-    def function(self, name: str, *args):
+    def function(self, name: str, *args, index: int|None=None):
         args = _convert_data_types(args)
         cmd = CodeBlock('func', args, data={'id': 'block', 'block': 'func', 'data': name})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
     
 
-    def process(self, name: str, *args):
+    def process(self, name: str, *args, index: int|None=None):
         args = _convert_data_types(args)
         cmd = CodeBlock('process', args, data={'id': 'block', 'block': 'process', 'data': name})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
     
 
-    def call_function(self, name: str, *args):
+    def call_function(self, name: str, *args, index: int|None=None):
         args = _convert_data_types(args)
         cmd = CodeBlock('call_func', args, data={'id': 'block', 'block': 'call_func', 'data': name})
-        self.codeblocks.append(cmd)
-    
+        self._add_codeblock(cmd, index)    
 
-    def start_process(self, name: str):
+    def start_process(self, name: str, index: int|None=None):
         cmd = CodeBlock('start_process', data={'id': 'block', 'block': 'start_process', 'data': name})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
 
 
-    def player_action(self, name: str, *args, target: Target=DEFAULT_TARGET):
+    def player_action(self, name: str, *args, target: Target=DEFAULT_TARGET, index: int|None=None):
         args = _convert_data_types(args)
         cmd = CodeBlock(name, args, target=target, data={'id': 'block', 'block': 'player_action', 'action': name})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
     
 
-    def game_action(self, name: str, *args):
+    def game_action(self, name: str, *args, index: int|None=None):
         args = _convert_data_types(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'game_action', 'action': name})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
     
 
-    def entity_action(self, name: str, *args, target: Target=DEFAULT_TARGET):
+    def entity_action(self, name: str, *args, target: Target=DEFAULT_TARGET, index: int|None=None):
         args = _convert_data_types(args)
         cmd = CodeBlock(name, args, target=target, data={'id': 'block', 'block': 'entity_action', 'action': name})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
     
 
-    def if_player(self, name: str, *args, target: Target=DEFAULT_TARGET, inverted: bool=False):
+    def if_player(self, name: str, *args, target: Target=DEFAULT_TARGET, inverted: bool=False, index: int|None=None):
         args = _convert_data_types(args)
         data = {'id': 'block', 'block': 'if_player', 'action': name}
         _add_inverted(data, inverted)
         cmd = CodeBlock(name, args, target=target, data=data)
-        self.codeblocks.append(cmd)
-        self._openbracket()
+        self._add_codeblock(cmd, index)
+        self._openbracket(index)
     
 
-    def if_variable(self, name: str, *args, inverted: bool=False):
+    def if_variable(self, name: str, *args, inverted: bool=False, index: int|None=None):
         args = _convert_data_types(args)
         data = {'id': 'block', 'block': 'if_var', 'action': name}
         _add_inverted(data, inverted)
         cmd = CodeBlock(name, args, data=data)
-        self.codeblocks.append(cmd)
-        self._openbracket()
+        self._add_codeblock(cmd, index)
+        self._openbracket(index)
     
 
-    def if_game(self, name: str, *args, inverted: bool=False):
+    def if_game(self, name: str, *args, inverted: bool=False, index: int|None=None):
         args = _convert_data_types(args)
         data = {'id': 'block', 'block': 'if_game', 'action': name}
         _add_inverted(data, inverted)
         cmd = CodeBlock(name, args, data=data)
-        self.codeblocks.append(cmd)
-        self._openbracket()
+        self._add_codeblock(cmd, index)
+        self._openbracket(index)
     
 
-    def if_entity(self, name: str, *args, target: Target=DEFAULT_TARGET, inverted: bool=False):
+    def if_entity(self, name: str, *args, target: Target=DEFAULT_TARGET, inverted: bool=False, index: int|None=None):
         args = _convert_data_types(args)
         data = {'id': 'block', 'block': 'if_entity', 'action': name}
         _add_inverted(data, inverted)
         cmd = CodeBlock(name, args, target=target, data=data)
-        self.codeblocks.append(cmd)
-        self._openbracket()
+        self._add_codeblock(cmd, index)
+        self._openbracket(index)
 
 
-    def else_(self):
+    def else_(self, index: int|None=None):
         cmd = CodeBlock('else', data={'id': 'block', 'block': 'else'})
-        self.codeblocks.append(cmd)
-        self._openbracket()
+        self._add_codeblock(cmd, index)
+        self._openbracket(index)
     
 
-    def repeat(self, name: str, *args, sub_action: str=None):
+    def repeat(self, name: str, *args, sub_action: str=None, index: int|None=None):
         args = _convert_data_types(args)
         data = {'id': 'block', 'block': 'repeat', 'action': name}
         if sub_action is not None:
             data['subAction'] = sub_action
         cmd = CodeBlock(name, args, data=data)
-        self.codeblocks.append(cmd)
-        self._openbracket('repeat')
+        self._add_codeblock(cmd, index)
+        self._openbracket(index, 'repeat')
 
 
-    def bracket(self, *args):
+    def bracket(self, *args, index: int|None=None):
         args = _convert_data_types(args)
         cmd = CodeBlock('bracket', data={'id': 'bracket', 'direct': 'close', 'type': self.bracket_stack.pop()})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
     
 
-    def control(self, name: str, *args):
+    def control(self, name: str, *args, index: int|None=None):
         args = _convert_data_types(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'control', 'action': name})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
     
 
-    def select_object(self, name: str, *args):
+    def select_object(self, name: str, *args, index: int|None=None):
         args = _convert_data_types(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'select_obj', 'action': name})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
     
 
-    def set_variable(self, name: str, *args):
+    def set_variable(self, name: str, *args, index: int|None=None):
         args = _convert_data_types(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'set_var', 'action': name})
-        self.codeblocks.append(cmd)
+        self._add_codeblock(cmd, index)
     
     
     def generate_script(self, output_path: str, indent_size: int=4, literal_shorthand: bool=True, var_shorthand: bool=False):
         """
         Generate an equivalent python script for this template.
 
         :param str output_path: The file path to write the script to.
```

### Comparing `dfpyre-0.6.0/dfpyre/scriptgen.py` & `dfpyre-0.6.1/dfpyre/scriptgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,20 +41,22 @@
 
 def argument_item_to_string(flags: GeneratorFlags, arg_item: object) -> str:
     class_name = arg_item.__class__.__name__
     if isinstance(arg_item, item):
         return f'{class_name}.from_nbt("""{arg_item.get_nbt()}""")'
     
     if isinstance(arg_item, string):
-        return f'{class_name}("{arg_item.value}")'
+        value = arg_item.value.replace('\n', '\\n')
+        return f'{class_name}("{value}")'
     
     if isinstance(arg_item, text):
+        value = arg_item.value.replace('\n', '\\n')
         if flags.literal_shorthand:
-            return f'"{arg_item.value}"'
-        return f'{class_name}("{arg_item.value}")'
+            return f'"{value}"'
+        return f'{class_name}("{value}")'
     
     if isinstance(arg_item, num):
         if not re.match(NUMBER_REGEX, str(arg_item.value)):
             return f'{class_name}("{arg_item.value}")' 
         if flags.literal_shorthand:
             return str(arg_item.value)
         return f'{class_name}({arg_item.value})'
@@ -132,13 +134,13 @@
         method_args = [f'"{codeblock.name}"']
         if codeblock.name in SINGLE_NAME_CODEBLOCKS:
             method_args[0] = f'"{codeblock.data["data"]}"'
         
         codeblock_args = [argument_item_to_string(flags, i) for i in codeblock.args]
         if codeblock_args:
             method_args.extend(codeblock_args)
-        if method_name in TARGET_CODEBLOCKS:
+        if method_name in TARGET_CODEBLOCKS and codeblock.target.name != 'SELECTION':
             method_args.append(f'target=Target.{codeblock.target.name}')
         
         line = f't.{method_name}({", ".join(method_args)})'
         add_script_line(flags, script_lines, indent_level, line)
     return SCRIPT_START + '\n'.join(script_lines)
```

### Comparing `dfpyre-0.6.0/dfpyre/style.py` & `dfpyre-0.6.1/dfpyre/style.py`

 * *Files identical despite different names*

### Comparing `dfpyre-0.6.0/PKG-INFO` & `dfpyre-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfpyre
-Version: 0.6.0
+Version: 0.6.1
 Summary: A package for external creation of code templates for the DiamondFire Minecraft server.
 Home-page: https://github.com/Amp63/pyre
 License: MIT
 Keywords: diamondfire,minecraft,template,item
 Author: Amp
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

