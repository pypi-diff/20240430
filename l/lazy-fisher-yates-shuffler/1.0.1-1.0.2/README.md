# Comparing `tmp/lazy_fisher_yates_shuffler-1.0.1.tar.gz` & `tmp/lazy_fisher_yates_shuffler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_fisher_yates_shuffler-1.0.1.tar", max compression
+gzip compressed data, was "lazy_fisher_yates_shuffler-1.0.2.tar", max compression
```

## Comparing `lazy_fisher_yates_shuffler-1.0.1.tar` & `lazy_fisher_yates_shuffler-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10148 2024-04-17 21:16:40.098048 lazy_fisher_yates_shuffler-1.0.1/LICENSE
--rw-r--r--   0        0        0     1383 2024-04-17 21:55:00.901475 lazy_fisher_yates_shuffler-1.0.1/README.md
--rw-r--r--   0        0        0      688 2024-04-17 20:51:04.903549 lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/__init__.py
--rw-r--r--   0        0        0     5845 2024-04-17 18:06:43.304925 lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/bit_manager.py
--rw-r--r--   0        0        0     6087 2024-04-17 19:18:54.761512 lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/persistence.py
--rw-r--r--   0        0        0    28815 2024-04-18 22:25:01.288051 lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/shuffler.py
--rw-r--r--   0        0        0      412 2024-04-18 22:25:38.428455 lazy_fisher_yates_shuffler-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 lazy_fisher_yates_shuffler-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10148 2024-04-17 21:16:40.098048 lazy_fisher_yates_shuffler-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1386 2024-04-30 18:27:17.941835 lazy_fisher_yates_shuffler-1.0.2/README.md
+-rw-r--r--   0        0        0      688 2024-04-17 20:51:04.903549 lazy_fisher_yates_shuffler-1.0.2/lazy_fisher_yates_shuffler/__init__.py
+-rw-r--r--   0        0        0     5845 2024-04-17 18:06:43.304925 lazy_fisher_yates_shuffler-1.0.2/lazy_fisher_yates_shuffler/bit_manager.py
+-rw-r--r--   0        0        0     6087 2024-04-17 19:18:54.761512 lazy_fisher_yates_shuffler-1.0.2/lazy_fisher_yates_shuffler/persistence.py
+-rw-r--r--   0        0        0    28849 2024-04-30 20:55:44.707236 lazy_fisher_yates_shuffler-1.0.2/lazy_fisher_yates_shuffler/shuffler.py
+-rw-r--r--   0        0        0      412 2024-04-30 21:20:04.644902 lazy_fisher_yates_shuffler-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 lazy_fisher_yates_shuffler-1.0.2/PKG-INFO
```

### Comparing `lazy_fisher_yates_shuffler-1.0.1/LICENSE` & `lazy_fisher_yates_shuffler-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lazy_fisher_yates_shuffler-1.0.1/README.md` & `lazy_fisher_yates_shuffler-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from lazy_fisher_yates_shuffler import Shuffler
 
 # Construct a 1,000-element non-cyclic shuffler.
 shuffler = Shuffler(1000, False)
 
 # Determine the value at a given index.
 index = 10
-value = shuffler.value_at(10)
+value = shuffler.value_at(index)
 
 print(value)
 
 # Shuffler is reversible.
 assert index == shuffler.index_of(value)
 
 # Iterate over the entire range of the shuffler (0-999).
```

### Comparing `lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/__init__.py` & `lazy_fisher_yates_shuffler-1.0.2/lazy_fisher_yates_shuffler/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/bit_manager.py` & `lazy_fisher_yates_shuffler-1.0.2/lazy_fisher_yates_shuffler/bit_manager.py`

 * *Files identical despite different names*

### Comparing `lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/persistence.py` & `lazy_fisher_yates_shuffler-1.0.2/lazy_fisher_yates_shuffler/persistence.py`

 * *Files identical despite different names*

### Comparing `lazy_fisher_yates_shuffler-1.0.1/lazy_fisher_yates_shuffler/shuffler.py` & `lazy_fisher_yates_shuffler-1.0.2/lazy_fisher_yates_shuffler/shuffler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Implementation of lazy Fisher-Yates shuffle using a binary tree to manage struck entries. The principal class is
 Shuffler, which maps an index to a value and vice versa, where the association between an index and a value is randomly
 determined the first time the index-to-value mapping is requested. The reverse value-to-index mapping is possible only
 after the corresponding index-to-value mapping is determined.
 
-Copyright (c) 2024 by Dolphin Data Development Ltd.
+Copyright (c) 2024 Dolphin Data Development Ltd.
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the
 License. You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
@@ -72,15 +72,15 @@
 
         self.struck_bitmap: int
         """
         Bitmap of struck entries if this is a terminal node.
         """
 
         # Attempt to restore the node state if indicated.
-        node_state: Final[Optional[NodeState]] = shuffler.persistence_manager.restore_node_state(key)\
+        node_state: Final[Optional[NodeState]] = shuffler.persistence_manager.restore_node_state(key) \
             if restore else \
             None
 
         if node_state is None:
             # Node has no struck count.
             self.struck_count = 0
             self.struck_bitmap = 0
@@ -147,80 +147,80 @@
 
         keys.append(self.key)
 
         if self.struck_count < 0:
             raise Exception("Negative struck count {} at node {}".format(self.struck_count, self.key))
 
         if not self.terminal:
+            bit_manager: Final[BitManager] = self.shuffler.bit_manager
+            bit: Final[int] = bit_manager.bit(self.bit_number)
+
+            right_size: int
+            left_size: int
+
+            if bit_manager.is_set(size, self.bit_number + 1):
+                # Size is the maximum possible and is split evenly between right and left nodes.
+                right_size = bit
+                left_size = bit
+            elif bit_manager.is_set(size, self.bit_number):
+                # Size will fill right node; put remainder in left node (clearing bit is the same as subtraction at
+                # this point).
+                right_size = bit
+                left_size = bit_manager.clear(size, self.bit_number)
+            else:
+                # Size doesn't fill right node; left node will not be created.
+                right_size = size
+                left_size = 0
+
+            right: Optional[_Node]
+            left: Optional[_Node]
+
             if self.struck_count == 0:
                 # Nodes with zero struck count shouldn't have right and/or left nodes in non-cyclic shuffler.
                 if not cyclic and (self._right is not None or self._left is not None):
                     raise Exception("Unexpected right and/or left nodes at non-persisted node {}".format(self.key))
+
+                # Validate nodes that have been created to support cyclic shuffler.
+                right = self._right
+                left = self._left
             else:
-                bit_manager: Final[BitManager] = self.shuffler.bit_manager
-                bit: Final[int] = bit_manager.bit(self.bit_number)
+                right = self.right
+                left = self.left if left_size != 0 else None
 
-                right_size: int
-                left_size: int
+            # Left node should be None if right node can handle this node.
+            if left_size == 0 and (self._left is not None or
+                                   self.shuffler.persistence_manager.restore_node_state(self.key - 1) is not None):
+                raise Exception("Unexpected left node at non-terminal node {}".format(self.key))
+
+            right_left_struck_count: int = (right.struck_count if right is not None else 0) + \
+                                           (left.struck_count if left is not None else 0)
+
+            if self.struck_count != right_left_struck_count:
+                raise Exception("Struck count {} doesn't match sum of right and left struck counts {} at "
+                                "non-terminal node {}".format(self.struck_count, right_left_struck_count,
+                                                              self.key))
 
-                if bit_manager.is_set(size, self.bit_number + 1):
-                    # Size is the maximum possible and is split evenly between right and left nodes.
-                    right_size = bit
-                    left_size = bit
-                elif bit_manager.is_set(size, self.bit_number):
-                    # Size will fill right node; put remainder in left node (clearing bit is the same as subtraction at
-                    # this point).
-                    right_size = bit
-                    left_size = bit_manager.clear(size, self.bit_number)
-                else:
-                    # Size doesn't fill right node; left node will not be created.
-                    right_size = size
-                    left_size = 0
-
-                right: Final[_Node] = self.right
-                left: Optional[_Node]
-
-                right_left_struck_count: int
-
-                if right_size != size:
-                    left = self.left
-
-                    right_left_struck_count = right.struck_count + left.struck_count
-                else:
-                    # Left node should be None if right node can handle this node.
-                    if self._left is not None or \
-                            self.shuffler.persistence_manager.restore_node_state(self.key - 1) is not None:
-                        raise Exception("Unexpected left node at non-terminal node {}".format(self.key))
-
-                    left = None
-
-                    right_left_struck_count = right.struck_count
-
-                if self.struck_count != right_left_struck_count:
-                    raise Exception("Struck count {} doesn't match sum of right and left struck counts {} at "
-                                    "non-terminal node {}".format(self.struck_count, right_left_struck_count,
-                                                                  self.key))
+            if self.struck_bitmap != 0:
+                raise Exception("Non-zero struck bitmap at non-terminal node {}".format(self.key))
 
+            if right is not None:
                 right.validate_state(keys, right_size, cyclic)
 
-                if left is not None:
-                    left.validate_state(keys, left_size, cyclic)
-
-            if self.struck_bitmap != 0:
-                raise Exception("Non-zero struck bitmap at non-terminal node {}".format(self.key))
+            if left is not None:
+                left.validate_state(keys, left_size, cyclic)
         else:
             # Terminal nodes shouldn't have right and/or left nodes.
             if self._right is not None or self._left is not None:
                 raise Exception("Unexpected right and/or left nodes at terminal node {}".format(self.key))
 
             struck_bit_count: Final[int] = self.struck_bitmap.bit_count()
 
-            if struck_bit_count != self.struck_count:
-                raise Exception("Struck bit count {} doesn't match struck count {} at terminal node {}".format(
-                    struck_bit_count, self.struck_count, self.key))
+            if self.struck_count != struck_bit_count:
+                raise Exception("Struck count {} doesn't match struck bit count {} at terminal node {}".format(
+                    self.struck_count, struck_bit_count, self.key))
 
 
 class Shuffler:
     """
     Shuffler. Values are randomly selected across a provided range using a lazy Fisher-Yates shuffle
     (https://en.wikipedia.org/wiki/Fisher%E2%80%93Yates_shuffle), where step 3 of the original method strikes the Kth
     entry not yet struck by building a binary tree on demand with each terminal node managing a 64-bit array
```

### Comparing `lazy_fisher_yates_shuffler-1.0.1/PKG-INFO` & `lazy_fisher_yates_shuffler-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-fisher-yates-shuffler
-Version: 1.0.1
+Version: 1.0.2
 Summary: Lazy Fisher-Yates shuffler
 Home-page: https://github.com/KDean-Dolphin/Python-Shuffler
 License: Apache-2.0
 Author: Kevin Dean
 Author-email: Kevin.Dean@datadevelopment.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -41,15 +41,15 @@
 from lazy_fisher_yates_shuffler import Shuffler
 
 # Construct a 1,000-element non-cyclic shuffler.
 shuffler = Shuffler(1000, False)
 
 # Determine the value at a given index.
 index = 10
-value = shuffler.value_at(10)
+value = shuffler.value_at(index)
 
 print(value)
 
 # Shuffler is reversible.
 assert index == shuffler.index_of(value)
 
 # Iterate over the entire range of the shuffler (0-999).
```

