# Comparing `tmp/inspyre_toolbox-1.4.0.tar.gz` & `tmp/inspyre_toolbox-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspyre_toolbox-1.4.0.tar", max compression
+gzip compressed data, was "inspyre_toolbox-1.4.1.tar", max compression
```

## Comparing `inspyre_toolbox-1.4.0.tar` & `inspyre_toolbox-1.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1099 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/LICENSE
--rw-r--r--   0        0        0      202 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/inspyre_toolbox/__about__.py
--rw-r--r--   0        0        0     2524 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/__init__.py
--rw-r--r--   0        0        0       15 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/inspyre_toolbox/api_changes.ini
--rw-r--r--   0        0        0        0 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/inspyre_toolbox/cli/__init__.py
--rw-r--r--   0        0        0     2943 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/inspyre_toolbox/cli/ist_bytes_converter/__init__.py
--rw-r--r--   0        0        0     3311 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/inspyre_toolbox/cli/ist_bytes_converter/arguments.py
--rw-r--r--   0        0        0     1360 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/inspyre_toolbox/cli/ist_bytes_converter/helpers.py
--rw-r--r--   0        0        0        0 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/inspyre_toolbox/common/__init__.py
--rw-r--r--   0        0        0      892 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/inspyre_toolbox/common/meta.py
--rw-r--r--   0        0        0     2714 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/console_kit/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/conversions/__init__.py
--rw-r--r--   0        0        0     4077 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/inspyre_toolbox/conversions/bytes/__init__.py
--rw-r--r--   0        0        0     5129 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/inspyre_toolbox/conversions/roman_numerals/__init__.py
--rw-r--r--   0        0        0     1103 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/conversions/roman_numerals/errors.py
--rw-r--r--   0        0        0        0 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/core/errors/__init__.py
--rw-r--r--   0        0        0     2561 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/core/errors/version.py
--rw-r--r--   0        0        0       96 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/core_helpers/__init__.py
--rw-r--r--   0        0        0      404 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/core_helpers/debugging.py
--rw-r--r--   0        0        0     3945 2024-02-26 02:10:11.475383 inspyre_toolbox-1.4.0/inspyre_toolbox/core_helpers/logging.py
--rw-r--r--   0        0        0     1900 2024-02-26 02:10:11.479383 inspyre_toolbox-1.4.0/inspyre_toolbox/docs/conversions/bytes.md
--rw-r--r--   0        0        0     3348 2024-02-26 02:10:11.479383 inspyre_toolbox-1.4.0/inspyre_toolbox/generations/__init__.py
--rw-r--r--   0        0        0    22229 2024-02-26 02:10:11.479383 inspyre_toolbox-1.4.0/inspyre_toolbox/humanize/__init__.py
--rw-r--r--   0        0        0      254 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/humanize/errors/__init__.py
--rw-r--r--   0        0        0     1881 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/humanize/errors/numerical.py
--rw-r--r--   0        0        0     8957 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/live_timer/__init__.py
--rw-r--r--   0        0        0     1066 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/live_timer/errors.py
--rw-r--r--   0        0        0     2210 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/live_timer/history.py
--rw-r--r--   0        0        0    11144 2024-02-26 02:10:11.479383 inspyre_toolbox-1.4.0/inspyre_toolbox/proc_man/__init__.py
--rw-r--r--   0        0        0      663 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/proc_man/errors.py
--rw-r--r--   0        0        0        0 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/pypi/__init__.py
--rw-r--r--   0        0        0      870 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/pypi/packages.py
--rw-r--r--   0        0        0      587 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/settings.py
--rw-r--r--   0        0        0     1826 2024-02-26 02:10:11.479383 inspyre_toolbox-1.4.0/inspyre_toolbox/solve_kit/__init__.py
--rw-r--r--   0        0        0      169 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/spanners/__init__.py
--rw-r--r--   0        0        0     2151 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/spanners/span_arg_parse.py
--rw-r--r--   0        0        0      973 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/syntactic_sweets/__init__.py
--rw-r--r--   0        0        0     2219 2024-02-26 02:09:43.943558 inspyre_toolbox-1.4.0/inspyre_toolbox/sys_man/__init__.py
--rw-r--r--   0        0        0     6774 2024-02-26 02:10:11.479383 inspyre_toolbox-1.4.0/inspyre_toolbox/version.py
--rw-r--r--   0        0        0     1621 2024-02-26 02:10:11.479383 inspyre_toolbox-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 inspyre_toolbox-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-04-30 20:45:10.403940 inspyre_toolbox-1.4.1/inspyre_toolbox/__about__.py
+-rw-r--r--   0        0        0     2639 2024-04-30 20:44:59.194115 inspyre_toolbox-1.4.1/inspyre_toolbox/__init__.py
+-rw-r--r--   0        0        0       16 2024-04-30 20:45:10.403940 inspyre_toolbox-1.4.1/inspyre_toolbox/api_changes.ini
+-rw-r--r--   0        0        0        0 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.1/inspyre_toolbox/cli/__init__.py
+-rw-r--r--   0        0        0     3005 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.1/inspyre_toolbox/cli/ist_bytes_converter/__init__.py
+-rw-r--r--   0        0        0     3388 2024-04-30 20:45:10.405306 inspyre_toolbox-1.4.1/inspyre_toolbox/cli/ist_bytes_converter/arguments.py
+-rw-r--r--   0        0        0     1425 2024-04-30 20:45:10.406705 inspyre_toolbox-1.4.1/inspyre_toolbox/cli/ist_bytes_converter/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:45:10.406705 inspyre_toolbox-1.4.1/inspyre_toolbox/common/__init__.py
+-rw-r--r--   0        0        0      934 2024-04-30 21:17:34.719515 inspyre_toolbox-1.4.1/inspyre_toolbox/common/meta.py
+-rw-r--r--   0        0        0     2808 2024-04-30 20:44:59.194115 inspyre_toolbox-1.4.1/inspyre_toolbox/console_kit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:44:59.195113 inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/__init__.py
+-rw-r--r--   0        0        0     4240 2024-04-30 20:45:10.407939 inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/bytes/__init__.py
+-rw-r--r--   0        0        0     5299 2024-04-30 20:45:10.407939 inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/roman_numerals/__init__.py
+-rw-r--r--   0        0        0     1143 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/roman_numerals/errors.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.1/inspyre_toolbox/core/errors/__init__.py
+-rw-r--r--   0        0        0     2636 2024-04-30 20:44:59.196112 inspyre_toolbox-1.4.1/inspyre_toolbox/core/errors/version.py
+-rw-r--r--   0        0        0       97 2024-04-30 20:44:59.197472 inspyre_toolbox-1.4.1/inspyre_toolbox/core_helpers/__init__.py
+-rw-r--r--   0        0        0      424 2024-04-30 20:44:59.197472 inspyre_toolbox-1.4.1/inspyre_toolbox/core_helpers/debugging.py
+-rw-r--r--   0        0        0     4065 2024-04-30 20:45:10.409300 inspyre_toolbox-1.4.1/inspyre_toolbox/core_helpers/logging.py
+-rw-r--r--   0        0        0     1951 2024-04-30 20:45:10.409300 inspyre_toolbox-1.4.1/inspyre_toolbox/docs/conversions/bytes.md
+-rw-r--r--   0        0        0     3413 2024-04-30 20:45:10.410790 inspyre_toolbox-1.4.1/inspyre_toolbox/generations/__init__.py
+-rw-r--r--   0        0        0    22944 2024-04-30 20:45:10.410790 inspyre_toolbox-1.4.1/inspyre_toolbox/humanize/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-30 20:44:59.198686 inspyre_toolbox-1.4.1/inspyre_toolbox/humanize/errors/__init__.py
+-rw-r--r--   0        0        0     1927 2024-04-30 20:44:59.199745 inspyre_toolbox-1.4.1/inspyre_toolbox/humanize/errors/numerical.py
+-rw-r--r--   0        0        0     9240 2024-04-30 20:44:59.200756 inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/__init__.py
+-rw-r--r--   0        0        0     1100 2024-04-30 20:44:59.200756 inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/errors.py
+-rw-r--r--   0        0        0     2297 2024-04-30 20:44:59.201755 inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/history.py
+-rw-r--r--   0        0        0    11458 2024-04-30 20:45:10.412229 inspyre_toolbox-1.4.1/inspyre_toolbox/proc_man/__init__.py
+-rw-r--r--   0        0        0      689 2024-04-30 20:44:59.202755 inspyre_toolbox-1.4.1/inspyre_toolbox/proc_man/errors.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:44:59.202755 inspyre_toolbox-1.4.1/inspyre_toolbox/pypi/__init__.py
+-rw-r--r--   0        0        0      900 2024-04-30 20:44:59.203757 inspyre_toolbox-1.4.1/inspyre_toolbox/pypi/packages.py
+-rw-r--r--   0        0        0      596 2024-04-30 20:44:59.203757 inspyre_toolbox-1.4.1/inspyre_toolbox/settings.py
+-rw-r--r--   0        0        0     1868 2024-04-30 20:45:10.412229 inspyre_toolbox-1.4.1/inspyre_toolbox/solve_kit/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.1/inspyre_toolbox/spanners/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.1/inspyre_toolbox/spanners/span_arg_parse.py
+-rw-r--r--   0        0        0     1014 2024-04-30 20:44:59.204758 inspyre_toolbox-1.4.1/inspyre_toolbox/syntactic_sweets/__init__.py
+-rw-r--r--   0        0        0     2265 2024-04-30 20:44:59.205757 inspyre_toolbox-1.4.1/inspyre_toolbox/sys_man/__init__.py
+-rw-r--r--   0        0        0     6999 2024-04-30 20:45:10.413573 inspyre_toolbox-1.4.1/inspyre_toolbox/version.py
+-rw-r--r--   0        0        0     1122 2024-04-30 20:45:10.401205 inspyre_toolbox-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1636 2024-04-30 20:57:32.686977 inspyre_toolbox-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 inspyre_toolbox-1.4.1/PKG-INFO
```

### Comparing `inspyre_toolbox-1.4.0/LICENSE` & `inspyre_toolbox-1.4.1/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# MIT License
-
-_Copyright (c) 2022-2024 Inspyre-Softworks_
-
-----
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-__THE SOFTWARE IS PROVIDED "_AS IS_", _WITHOUT_ WARRANTY OF ANY KIND, _EXPRESS OR
-IMPLIED_, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.__
+# MIT License
+
+_Copyright (c) 2022-2024 Inspyre-Softworks_
+
+----
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+__THE SOFTWARE IS PROVIDED "_AS IS_", _WITHOUT_ WARRANTY OF ANY KIND, _EXPRESS OR
+IMPLIED_, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.__
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/__init__.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-from typing import NewType
-
-
-def __split_evenly(target):
-    """
-    
-    Split a target list down the center.
-    
-    Arguments:
-        target (list):
-            The list you'd like to split.
-
-    Returns:
-        (list, list):
-            Two lists that should be perfectly (or as perfectly as possible
-            while keeping whole numbers) split in two while maintaining
-            its order.
-
-    """
-    length = len(target)
-    mi = length // 2
-
-    list1 = target[:mi]
-    list2 = target[mi:]
-
-    return list1, list2
-
-
-def __split_alt(target):
-    """
-    
-    Split a given list into two columns in an alternating format.
-    
-    
-    ========= ===========
-      Col 1      Col 2
-    ========= ===========
-        1          2
-    --------- -----------
-        3          4
-    ========= ===========
-    
-    Args:
-        target:
-
-    Returns:
-
-    """
-    list1 = []
-    list2 = []
-
-    for item in target:
-        if target.index(item) % 2 == 0:
-            list1.append(item)
-        else:
-            list2.append(item)
-
-    return list1, list2
-
-
-def split_list(target, split_method='middle'):
-    """
-    
-    Split a given list using an indicted method.
-    
-    Args:
-        target:
-        split_method:
-
-    Returns:
-
-    """
-    valid_split_methods = [
-            'alternating_columns',
-            'middle',
-    ]
-    """
-    valid_split_methods:
-        
-        * alternating_columns
-        * middle
-    
-    Note:
-        The values that will be accepted for the 'split_method'
-        parameter are as follows;
-        
-        
-    
-       * alternating_columns:
-        
-          Sort into a number of columns where ordering goes from
-          left-to-right.
-          
-        * middle:
-        
-          Split a list in half results in two smaller lists containing
-          elements from the original in the same order. (The Default
-          parameter value)
-          
-    """
-    if split_method.lower() not in valid_split_methods:
-        raise ValueError(f"The value for 'split_method' must be one of; {', '.join(valid_split_methods)}")
-    if split_method.lower() == 'middle':
-        return __split_evenly(target)
-    elif split_method.lower() == 'alternating_columns':
-        return __split_alt(target)
-
-
-ChunkifiedList = NewType('ChunkifiedList', list)
-
-
-def chunkify(target: list, num_per: int) -> ChunkifiedList:
-    ret_lst = lambda target, num_per: [target[i:i + num_per] for i in range(0, len(target), num_per)]
-
-    return ChunkifiedList(ret_lst(target, num_per))
+from typing import NewType
+
+
+def __split_evenly(target):
+    """
+    
+    Split a target list down the center.
+    
+    Arguments:
+        target (list):
+            The list you'd like to split.
+
+    Returns:
+        (list, list):
+            Two lists that should be perfectly (or as perfectly as possible
+            while keeping whole numbers) split in two while maintaining
+            its order.
+
+    """
+    length = len(target)
+    mi = length // 2
+
+    list1 = target[:mi]
+    list2 = target[mi:]
+
+    return list1, list2
+
+
+def __split_alt(target):
+    """
+    
+    Split a given list into two columns in an alternating format.
+    
+    
+    ========= ===========
+      Col 1      Col 2
+    ========= ===========
+        1          2
+    --------- -----------
+        3          4
+    ========= ===========
+    
+    Args:
+        target:
+
+    Returns:
+
+    """
+    list1 = []
+    list2 = []
+
+    for item in target:
+        if target.index(item) % 2 == 0:
+            list1.append(item)
+        else:
+            list2.append(item)
+
+    return list1, list2
+
+
+def split_list(target, split_method='middle'):
+    """
+    
+    Split a given list using an indicted method.
+    
+    Args:
+        target:
+        split_method:
+
+    Returns:
+
+    """
+    valid_split_methods = [
+            'alternating_columns',
+            'middle',
+    ]
+    """
+    valid_split_methods:
+        
+        * alternating_columns
+        * middle
+    
+    Note:
+        The values that will be accepted for the 'split_method'
+        parameter are as follows;
+        
+        
+    
+       * alternating_columns:
+        
+          Sort into a number of columns where ordering goes from
+          left-to-right.
+          
+        * middle:
+        
+          Split a list in half results in two smaller lists containing
+          elements from the original in the same order. (The Default
+          parameter value)
+          
+    """
+    if split_method.lower() not in valid_split_methods:
+        raise ValueError(f"The value for 'split_method' must be one of; {', '.join(valid_split_methods)}")
+    if split_method.lower() == 'middle':
+        return __split_evenly(target)
+    elif split_method.lower() == 'alternating_columns':
+        return __split_alt(target)
+
+
+ChunkifiedList = NewType('ChunkifiedList', list)
+
+
+def chunkify(target: list, num_per: int) -> ChunkifiedList:
+    ret_lst = lambda target, num_per: [target[i:i + num_per] for i in range(0, len(target), num_per)]
+
+    return ChunkifiedList(ret_lst(target, num_per))
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/cli/ist_bytes_converter/__init__.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/cli/ist_bytes_converter/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-"""
-This script provides a command-line interface to convert between different units of digital information storage.
-It uses the inspyre_toolbox library to perform the conversion and to humanize the numerical output.
-The user can specify the amount and units for conversion, and the script will output the result in the desired unit.
-"""
-
-
-# Our imports
-from inspyre_toolbox.conversions.bytes import ByteConverter
-from inspyre_toolbox.humanize import Numerical
-from inspyre_toolbox.cli.ist_bytes_converter.arguments import Arguments
-from inspyre_toolbox.cli.ist_bytes_converter.helpers import clean_unit_str, convert_if_whole_number
-
-
-# Define a function to handle the main application operations.
-def main(cli_args=None):
-    """
-    Main function that handles the conversion between different units of digital information storage.
-
-    Parameters:
-        cli_args (argparse.Namespace, optional):
-            Parsed command-line arguments. If `None`, the function will parse the arguments itself.
-    
-    Returns:
-        None
-    """
-    # If `cli_args` is `None` we should create an instance 
-    # of the parser.
-    args = Arguments().parsed if cli_args is None else cli_args  # Parse command-line arguments
-
-    # Gather the arguments from the command-line
-    from_unit = clean_unit_str(args.from_unit)  # Clean and standardize the 'from' unit
-    to_unit = clean_unit_str(args.to_unit)  # Clean and standardize the 'to' unit
-
-    # Grab our given amount and pass it to be converted to an integer if
-    # it is a whole number.
-    amount = convert_if_whole_number(args.amount)
-
-    # Create a converter object.
-    converter = ByteConverter(amount, from_unit)  # Initialize the ByteConverter with the specified amount and 'from' unit
-   
-    # Use it to convert from our starting unit to the target unit.
-    result = converter.convert(to_unit)  # Perform the conversion to the 'to' unit
-
-    # Grab our result and pass it to be converted to an integer if it is a whole number.
-    result = convert_if_whole_number(result)
-    
-    # Format our starting string properly by;
-    #   - Passing it through the `Numerical` class,
-    #   - Grabbing the resulting string and break it into a list delimited by a space,
-    #   - Grab the last item in the list that results from the above operation.
-    from_str = Numerical(amount, from_unit, store_as_float=False).count_noun()  # Humanize the 'from' amount and unit
-    
-    # Format out target string properly by;
-    #   - Passing it through the `Numerical` class,
-    #   - Grabbing the resulting string and break it into a list delimited by a space,
-    #   - Grab the last item in the list that results from the above operation.
-    to_str = Numerical(result, to_unit, store_as_float=False).count_noun()  # Humanize the 'to' amount and unit
-
-    # Output the conversion details and result
-    print(f'Converting {from_str} to {to_str.split(" ")[-1]}')
-    print(f'Result: {to_str}')
+"""
+This script provides a command-line interface to convert between different units of digital information storage.
+It uses the inspyre_toolbox library to perform the conversion and to humanize the numerical output.
+The user can specify the amount and units for conversion, and the script will output the result in the desired unit.
+"""
+
+
+# Our imports
+from inspyre_toolbox.conversions.bytes import ByteConverter
+from inspyre_toolbox.humanize import Numerical
+from inspyre_toolbox.cli.ist_bytes_converter.arguments import Arguments
+from inspyre_toolbox.cli.ist_bytes_converter.helpers import clean_unit_str, convert_if_whole_number
+
+
+# Define a function to handle the main application operations.
+def main(cli_args=None):
+    """
+    Main function that handles the conversion between different units of digital information storage.
+
+    Parameters:
+        cli_args (argparse.Namespace, optional):
+            Parsed command-line arguments. If `None`, the function will parse the arguments itself.
+    
+    Returns:
+        None
+    """
+    # If `cli_args` is `None` we should create an instance 
+    # of the parser.
+    args = Arguments().parsed if cli_args is None else cli_args  # Parse command-line arguments
+
+    # Gather the arguments from the command-line
+    from_unit = clean_unit_str(args.from_unit)  # Clean and standardize the 'from' unit
+    to_unit = clean_unit_str(args.to_unit)  # Clean and standardize the 'to' unit
+
+    # Grab our given amount and pass it to be converted to an integer if
+    # it is a whole number.
+    amount = convert_if_whole_number(args.amount)
+
+    # Create a converter object.
+    converter = ByteConverter(amount, from_unit)  # Initialize the ByteConverter with the specified amount and 'from' unit
+   
+    # Use it to convert from our starting unit to the target unit.
+    result = converter.convert(to_unit)  # Perform the conversion to the 'to' unit
+
+    # Grab our result and pass it to be converted to an integer if it is a whole number.
+    result = convert_if_whole_number(result)
+    
+    # Format our starting string properly by;
+    #   - Passing it through the `Numerical` class,
+    #   - Grabbing the resulting string and break it into a list delimited by a space,
+    #   - Grab the last item in the list that results from the above operation.
+    from_str = Numerical(amount, from_unit, store_as_float=False).count_noun()  # Humanize the 'from' amount and unit
+    
+    # Format out target string properly by;
+    #   - Passing it through the `Numerical` class,
+    #   - Grabbing the resulting string and break it into a list delimited by a space,
+    #   - Grab the last item in the list that results from the above operation.
+    to_str = Numerical(result, to_unit, store_as_float=False).count_noun()  # Humanize the 'to' amount and unit
+
+    # Output the conversion details and result
+    print(f'Converting {from_str} to {to_str.split(" ")[-1]}')
+    print(f'Result: {to_str}')
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/cli/ist_bytes_converter/arguments.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/cli/ist_bytes_converter/arguments.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-"""
-This module provides a command-line interface for converting between different information storage units.
-It includes a custom ArgumentParser class that parses the user input, allowing for conversion operations
-between various storage units, with 'bytes' as the default unit to convert from.
-
-Usage:
-    python ist_bytes_converter.py <amount> [<from_unit>] <to_unit>
-
-Example:
-    python ist_bytes_converter.py 1024 bytes KB
-    This will convert 1024 bytes to kilobytes.
-"""
-
-from argparse import ArgumentParser
-
-# Constants for program name and description
-PROG = 'ist-bytes-converter'
-DESCRIPTION = 'Convert between information storage units.'
-
-# Exported names
-__all__ = ['Arguments']
-
-
-class Arguments(ArgumentParser):
-    """
-    Custom ArgumentParser class for parsing command-line arguments for the byte converter program.
-
-    This class inherits from argparse.ArgumentParser and customizes initialization to define specific
-    command-line arguments needed for the conversion between information storage units.
-
-    Attributes:
-        __parsed (argparse.Namespace, optional): A namespace object containing the parsed arguments.
-            It's initially None and gets populated after parsing command-line arguments.
-    
-    Methods:
-        __init__: Initializes the custom ArgumentParser with predefined program name and description,
-            and sets up the command-line arguments.
-        parsed: Parses the command-line arguments if not already done and returns the parsed namespace.
-    """
-
-    def __init__(self, *args, **kwargs):
-        """
-        Initializes the custom ArgumentParser with the program name, description, and command-line arguments.
-
-        The method sets up the argument parser with a specific program name and description. It defines
-        command-line arguments for specifying the amount of storage units to convert, the unit to convert
-        from (optional, defaults to 'bytes'), and the unit to convert to.
-
-        Args:
-            *args: Variable length argument list for ArgumentParser.
-            **kwargs: Arbitrary keyword arguments for ArgumentParser.
-        """
-        super().__init__(prog=PROG, description=DESCRIPTION, *args, **kwargs)
-        
-        # Define the command-line arguments for the program
-        self.add_argument('amount', type=float, help='The amount of storage units to convert.')
-        self.add_argument('from_unit', type=str, nargs='?', default='bytes',
-                          help='The storage unit to convert from. Optional, defaults to "bytes".')
-        self.add_argument('to_unit', type=str, help='The storage unit to convert to.')
-        
-        self.__parsed = None  # Placeholder for parsed arguments
-    
-    @property
-    def parsed(self):
-        """
-        Parses the command-line arguments if not already done and returns the parsed namespace.
-
-        This method checks if the command-line arguments have already been parsed to avoid
-        redundant parsing. If not already parsed, it parses the arguments and stores the result
-        in the `__parsed` attribute.
-
-        Returns:
-            argparse.Namespace: The namespace object containing the parsed arguments.
-        """
-        if self.__parsed is None:
-            self.__parsed = self.parse_args()
-        return self.__parsed
+"""
+This module provides a command-line interface for converting between different information storage units.
+It includes a custom ArgumentParser class that parses the user input, allowing for conversion operations
+between various storage units, with 'bytes' as the default unit to convert from.
+
+Usage:
+    python ist_bytes_converter.py <amount> [<from_unit>] <to_unit>
+
+Example:
+    python ist_bytes_converter.py 1024 bytes KB
+    This will convert 1024 bytes to kilobytes.
+"""
+
+from argparse import ArgumentParser
+
+# Constants for program name and description
+PROG = 'ist-bytes-converter'
+DESCRIPTION = 'Convert between information storage units.'
+
+# Exported names
+__all__ = ['Arguments']
+
+
+class Arguments(ArgumentParser):
+    """
+    Custom ArgumentParser class for parsing command-line arguments for the byte converter program.
+
+    This class inherits from argparse.ArgumentParser and customizes initialization to define specific
+    command-line arguments needed for the conversion between information storage units.
+
+    Attributes:
+        __parsed (argparse.Namespace, optional): A namespace object containing the parsed arguments.
+            It's initially None and gets populated after parsing command-line arguments.
+    
+    Methods:
+        __init__: Initializes the custom ArgumentParser with predefined program name and description,
+            and sets up the command-line arguments.
+        parsed: Parses the command-line arguments if not already done and returns the parsed namespace.
+    """
+
+    def __init__(self, *args, **kwargs):
+        """
+        Initializes the custom ArgumentParser with the program name, description, and command-line arguments.
+
+        The method sets up the argument parser with a specific program name and description. It defines
+        command-line arguments for specifying the amount of storage units to convert, the unit to convert
+        from (optional, defaults to 'bytes'), and the unit to convert to.
+
+        Args:
+            *args: Variable length argument list for ArgumentParser.
+            **kwargs: Arbitrary keyword arguments for ArgumentParser.
+        """
+        super().__init__(prog=PROG, description=DESCRIPTION, *args, **kwargs)
+        
+        # Define the command-line arguments for the program
+        self.add_argument('amount', type=float, help='The amount of storage units to convert.')
+        self.add_argument('from_unit', type=str, nargs='?', default='bytes',
+                          help='The storage unit to convert from. Optional, defaults to "bytes".')
+        self.add_argument('to_unit', type=str, help='The storage unit to convert to.')
+        
+        self.__parsed = None  # Placeholder for parsed arguments
+    
+    @property
+    def parsed(self):
+        """
+        Parses the command-line arguments if not already done and returns the parsed namespace.
+
+        This method checks if the command-line arguments have already been parsed to avoid
+        redundant parsing. If not already parsed, it parses the arguments and stores the result
+        in the `__parsed` attribute.
+
+        Returns:
+            argparse.Namespace: The namespace object containing the parsed arguments.
+        """
+        if self.__parsed is None:
+            self.__parsed = self.parse_args()
+        return self.__parsed
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/console_kit/__init__.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/console_kit/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-# ==============================================================================
-#  Copyright (c) Inspyre Softworks 2022.                                       =
-#                                                                              =
-#  Author:                 T. Blackstone                                       =
-#  Author Email:    <t.blackstone@inspyre.tech>                                =
-#  Created:              2/10/22, 9:42 PM                                      =
-# ==============================================================================
-
-import os
-import random
-import sys
-from time import sleep
-
-
-def __get_delay(fast=False):
-    possible = list(range(45, 100)) if fast else list(range(100, 301))
-    return random.choice(possible) / 1000
-
-
-def clear_console():
-    """
-
-    Clear the current terminal screen.
-
-    Returns
-    -------
-    None.
-
-    """
-    cmd = "cls" if os.name in ("nt", "dos") else "clear"
-
-    os.system(cmd)
-
-
-def animate_typing(
-        message: str,
-        interval: float = None,
-        skip_pre_newline: bool = False,
-        skip_post_newline: bool = False,
-        clear_screen: bool = False,
-        fast_typer: bool = False,
-        override_upper_limit: bool = False,
-):
-    """
-    
-    Animate typing in the terminal/console.
-    
-    Args:
-        message (str):
-            The message you'd like to print through a typing animation.
-
-        interval (Optional(int|float)):
-            The time (in number of seconds as an integer) that you'd like to have pass between characters being printed
-            to the line. (Defaults to random intervals to more realistically simulate typing.
-
-        skip_pre_newline:
-            Don't print a newline before commencing the animation.
-
-        skip_post_newline (Optional(bool)):
-            Don't print a newline after we're finished with the typing animation. (Optional)
-
-        clear_screen:
-
-         fast_typer:
-        override_upper_limit:
-
-    Returns:
-        None
-
-    """
-    # If we were instructed to clear the screen, do it.
-    if clear_screen:
-        clear_console()
-
-    # If we weren't instructed to skip a leading newline, print the newline.
-    if not skip_pre_newline:
-        print("\n")
-
-    for char in message:
-        if interval is None:
-            time_between = __get_delay(fast_typer)
-        else:
-            time_between = interval
-
-            time_between = min(time_between, 0.301)
-            if time_between <= 0:
-                time_between = __get_delay()
-
-        sleep(time_between)
-        sys.stdout.write(char)
-
-    # If we weren't instructed to skip the post-animation newline, print the newline.
-    if not skip_post_newline:
-        print('\n')
+# ==============================================================================
+#  Copyright (c) Inspyre Softworks 2022.                                       =
+#                                                                              =
+#  Author:                 T. Blackstone                                       =
+#  Author Email:    <t.blackstone@inspyre.tech>                                =
+#  Created:              2/10/22, 9:42 PM                                      =
+# ==============================================================================
+
+import os
+import random
+import sys
+from time import sleep
+
+
+def __get_delay(fast=False):
+    possible = list(range(45, 100)) if fast else list(range(100, 301))
+    return random.choice(possible) / 1000
+
+
+def clear_console():
+    """
+
+    Clear the current terminal screen.
+
+    Returns
+    -------
+    None.
+
+    """
+    cmd = "cls" if os.name in ("nt", "dos") else "clear"
+
+    os.system(cmd)
+
+
+def animate_typing(
+        message: str,
+        interval: float = None,
+        skip_pre_newline: bool = False,
+        skip_post_newline: bool = False,
+        clear_screen: bool = False,
+        fast_typer: bool = False,
+        override_upper_limit: bool = False,
+):
+    """
+    
+    Animate typing in the terminal/console.
+    
+    Args:
+        message (str):
+            The message you'd like to print through a typing animation.
+
+        interval (Optional(int|float)):
+            The time (in number of seconds as an integer) that you'd like to have pass between characters being printed
+            to the line. (Defaults to random intervals to more realistically simulate typing.
+
+        skip_pre_newline:
+            Don't print a newline before commencing the animation.
+
+        skip_post_newline (Optional(bool)):
+            Don't print a newline after we're finished with the typing animation. (Optional)
+
+        clear_screen:
+
+         fast_typer:
+        override_upper_limit:
+
+    Returns:
+        None
+
+    """
+    # If we were instructed to clear the screen, do it.
+    if clear_screen:
+        clear_console()
+
+    # If we weren't instructed to skip a leading newline, print the newline.
+    if not skip_pre_newline:
+        print("\n")
+
+    for char in message:
+        if interval is None:
+            time_between = __get_delay(fast_typer)
+        else:
+            time_between = interval
+
+            time_between = min(time_between, 0.301)
+            if time_between <= 0:
+                time_between = __get_delay()
+
+        sleep(time_between)
+        sys.stdout.write(char)
+
+    # If we weren't instructed to skip the post-animation newline, print the newline.
+    if not skip_post_newline:
+        print('\n')
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/conversions/bytes/__init__.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/conversions/bytes/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,255 +1,265 @@
-00000000: 0a63 6c61 7373 2042 7974 6543 6f6e 7665  .class ByteConve
-00000010: 7274 6572 3a0a 2020 2020 2222 220a 2020  rter:.    """.  
-00000020: 2020 4120 636c 6173 7320 746f 2063 6f6e    A class to con
-00000030: 7665 7274 2064 6966 6665 7265 6e74 2075  vert different u
-00000040: 6e69 7473 206f 6620 6469 6769 7461 6c20  nits of digital 
-00000050: 696e 666f 726d 6174 696f 6e2e 0a0a 2020  information...  
-00000060: 2020 2e2e 2e0a 0a20 2020 2041 7474 7269    .....    Attri
-00000070: 6275 7465 730a 2020 2020 2d2d 2d2d 2d2d  butes.    ------
-00000080: 2d2d 2d2d 0a20 2020 2075 6e69 7473 203a  ----.    units :
-00000090: 2064 6963 740a 2020 2020 2020 2020 6120   dict.        a 
-000000a0: 6469 6374 696f 6e61 7279 2068 6f6c 6469  dictionary holdi
-000000b0: 6e67 2074 6865 2063 6f6e 7665 7273 696f  ng the conversio
-000000c0: 6e20 756e 6974 730a 2020 2020 5f5f 6279  n units.    __by
-000000d0: 7465 7320 3a20 696e 740a 2020 2020 2020  tes : int.      
-000000e0: 2020 6120 7072 6976 6174 6520 6174 7472    a private attr
-000000f0: 6962 7574 6520 746f 2068 6f6c 6420 7468  ibute to hold th
-00000100: 6520 7661 6c75 6520 696e 2062 7974 6573  e value in bytes
-00000110: 0a0a 2020 2020 4d65 7468 6f64 730a 2020  ..    Methods.  
-00000120: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 636f    -------.    co
-00000130: 6e76 6572 7428 756e 6974 290a 2020 2020  nvert(unit).    
-00000140: 2020 2020 436f 6e76 6572 7473 2074 6865      Converts the
-00000150: 2062 7974 6573 2076 616c 7565 2074 6f20   bytes value to 
-00000160: 7468 6520 7370 6563 6966 6965 6420 756e  the specified un
-00000170: 6974 2e0a 2020 2020 2222 220a 2020 2020  it..    """.    
-00000180: 2320 4469 6374 696f 6e61 7279 2068 6f6c  # Dictionary hol
-00000190: 6469 6e67 2074 6865 2063 6f6e 7665 7273  ding the convers
-000001a0: 696f 6e20 756e 6974 730a 2020 2020 756e  ion units.    un
-000001b0: 6974 7320 3d20 7b0a 2020 2020 2020 2020  its = {.        
-000001c0: 2762 7974 6527 3a20 312c 0a20 2020 2020  'byte': 1,.     
-000001d0: 2020 2027 6b69 6c6f 6279 7465 273a 2031     'kilobyte': 1
-000001e0: 3032 342c 0a20 2020 2020 2020 2027 6d65  024,.        'me
-000001f0: 6761 6279 7465 273a 2031 3032 342a 2a32  gabyte': 1024**2
-00000200: 2c0a 2020 2020 2020 2020 2767 6967 6162  ,.        'gigab
-00000210: 7974 6527 3a20 3130 3234 2a2a 332c 0a20  yte': 1024**3,. 
-00000220: 2020 2020 2020 2027 7465 7261 6279 7465         'terabyte
-00000230: 273a 2031 3032 342a 2a34 2c0a 2020 2020  ': 1024**4,.    
-00000240: 2020 2020 2770 6574 6162 7974 6527 3a20      'petabyte': 
-00000250: 3130 3234 2a2a 352c 0a20 2020 2020 2020  1024**5,.       
-00000260: 2027 6578 6162 7974 6527 3a20 3130 3234   'exabyte': 1024
-00000270: 2a2a 362c 0a20 2020 2020 2020 2027 7a65  **6,.        'ze
-00000280: 7461 6279 7465 273a 2031 3032 342a 2a37  tabyte': 1024**7
-00000290: 2c0a 2020 2020 2020 2020 2779 6f74 7461  ,.        'yotta
-000002a0: 6279 7465 273a 2031 3032 342a 2a38 2c0a  byte': 1024**8,.
-000002b0: 2020 2020 2020 2020 2762 6974 273a 2031          'bit': 1
-000002c0: 2f38 2c0a 2020 2020 2020 2020 276b 696c  /8,.        'kil
-000002d0: 6f62 6974 273a 2031 3032 342f 382c 0a20  obit': 1024/8,. 
-000002e0: 2020 2020 2020 2027 6d65 6761 6269 7427         'megabit'
-000002f0: 3a20 2831 3032 342a 2a32 292f 382c 0a20  : (1024**2)/8,. 
-00000300: 2020 2020 2020 2027 6769 6761 6269 7427         'gigabit'
-00000310: 3a20 2831 3032 342a 2a33 292f 382c 0a20  : (1024**3)/8,. 
-00000320: 2020 2020 2020 2027 7465 7261 6269 7427         'terabit'
-00000330: 3a20 2831 3032 342a 2a34 292f 382c 0a20  : (1024**4)/8,. 
-00000340: 2020 2020 2020 2027 7065 7461 6269 7427         'petabit'
-00000350: 3a20 2831 3032 342a 2a35 292f 382c 0a20  : (1024**5)/8,. 
-00000360: 2020 2020 2020 2027 6578 6162 6974 273a         'exabit':
-00000370: 2028 3130 3234 2a2a 3629 2f38 2c0a 2020   (1024**6)/8,.  
-00000380: 2020 2020 2020 277a 6574 6162 6974 273a        'zetabit':
-00000390: 2028 3130 3234 2a2a 3729 2f38 2c0a 2020   (1024**7)/8,.  
-000003a0: 2020 2020 2020 2779 6f74 7461 6269 7427        'yottabit'
-000003b0: 3a20 2831 3032 342a 2a38 292f 382c 0a20  : (1024**8)/8,. 
-000003c0: 2020 207d 0a0a 2020 2020 6465 6620 5f5f     }..    def __
-000003d0: 696e 6974 5f5f 2873 656c 662c 2076 616c  init__(self, val
-000003e0: 7565 2c20 756e 6974 293a 0a20 2020 2020  ue, unit):.     
-000003f0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00000400: 6f6e 7374 7275 6374 7320 616c 6c20 7468  onstructs all th
-00000410: 6520 6e65 6365 7373 6172 7920 6174 7472  e necessary attr
-00000420: 6962 7574 6573 2066 6f72 2074 6865 2042  ibutes for the B
-00000430: 7974 6543 6f6e 7665 7274 6572 206f 626a  yteConverter obj
-00000440: 6563 742e 0a0a 2020 2020 2020 2020 5061  ect...        Pa
-00000450: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00000460: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00000470: 2020 2020 2020 2020 7661 6c75 6520 3a20          value : 
-00000480: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00000490: 2020 2020 7468 6520 7661 6c75 6520 746f      the value to
-000004a0: 2062 6520 636f 6e76 6572 7465 640a 2020   be converted.  
-000004b0: 2020 2020 2020 2020 2020 756e 6974 203a            unit :
-000004c0: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
-000004d0: 2020 2020 2074 6865 2075 6e69 7420 6f66       the unit of
-000004e0: 2074 6865 2076 616c 7565 2074 6f20 6265   the value to be
-000004f0: 2063 6f6e 7665 7274 6564 0a20 2020 2020   converted.     
-00000500: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-00000510: 2043 6f6e 7665 7274 2074 6865 2069 6e70   Convert the inp
-00000520: 7574 2076 616c 7565 2074 6f20 6279 7465  ut value to byte
-00000530: 730a 2020 2020 2020 2020 7365 6c66 2e5f  s.        self._
-00000540: 5f62 7974 6573 203d 2076 616c 7565 202a  _bytes = value *
-00000550: 2073 656c 662e 756e 6974 735b 756e 6974   self.units[unit
-00000560: 5d0a 0a20 2020 2064 6566 2063 6f6e 7665  ]..    def conve
-00000570: 7274 2873 656c 662c 2075 6e69 7429 3a0a  rt(self, unit):.
-00000580: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00000590: 2020 2020 436f 6e76 6572 7473 2074 6865      Converts the
-000005a0: 2062 7974 6573 2076 616c 7565 2074 6f20   bytes value to 
-000005b0: 7468 6520 7370 6563 6966 6965 6420 756e  the specified un
-000005c0: 6974 2e0a 0a20 2020 2020 2020 2050 6172  it...        Par
-000005d0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-000005e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-000005f0: 2020 2020 2020 2075 6e69 7420 3a20 7374         unit : st
-00000600: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00000610: 2020 7468 6520 756e 6974 2074 6f20 7768    the unit to wh
-00000620: 6963 6820 7468 6520 7661 6c75 6520 6973  ich the value is
-00000630: 2074 6f20 6265 2063 6f6e 7665 7274 6564   to be converted
-00000640: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00000650: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00000660: 2d0a 2020 2020 2020 2020 2020 2020 666c  -.            fl
-00000670: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
-00000680: 2020 2020 7468 6520 636f 6e76 6572 7465      the converte
-00000690: 6420 7661 6c75 650a 2020 2020 2020 2020  d value.        
-000006a0: 2222 220a 2020 2020 2020 2020 2320 436f  """.        # Co
-000006b0: 6e76 6572 7420 7468 6520 6279 7465 7320  nvert the bytes 
-000006c0: 7661 6c75 6520 746f 2074 6865 2073 7065  value to the spe
-000006d0: 6369 6669 6564 2075 6e69 740a 2020 2020  cified unit.    
-000006e0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000006f0: 5f5f 6279 7465 7320 2f20 7365 6c66 2e75  __bytes / self.u
-00000700: 6e69 7473 5b75 6e69 745d 0a0a 2020 2020  nits[unit]..    
-00000710: 2320 4265 6c6f 7720 6172 6520 7072 6f70  # Below are prop
-00000720: 6572 7479 206d 6574 686f 6473 2074 6861  erty methods tha
-00000730: 7420 7265 7475 726e 2074 6865 2076 616c  t return the val
-00000740: 7565 2069 6e20 6120 7370 6563 6966 6963  ue in a specific
-00000750: 2075 6e69 740a 0a20 2020 2040 7072 6f70   unit..    @prop
-00000760: 6572 7479 0a20 2020 2064 6566 2062 6974  erty.    def bit
-00000770: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-00000780: 2022 2222 5265 7475 726e 7320 7468 6520   """Returns the 
-00000790: 7661 6c75 6520 696e 2062 6974 7322 2222  value in bits"""
-000007a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000007b0: 7365 6c66 2e63 6f6e 7665 7274 2827 6269  self.convert('bi
-000007c0: 7427 290a 0a20 2020 2040 7072 6f70 6572  t')..    @proper
-000007d0: 7479 0a20 2020 2064 6566 206b 696c 6f62  ty.    def kilob
-000007e0: 6974 7328 7365 6c66 293a 0a20 2020 2020  its(self):.     
-000007f0: 2020 2022 2222 5265 7475 726e 7320 7468     """Returns th
-00000800: 6520 7661 6c75 6520 696e 206b 696c 6f62  e value in kilob
-00000810: 6974 7322 2222 0a20 2020 2020 2020 2072  its""".        r
-00000820: 6574 7572 6e20 7365 6c66 2e63 6f6e 7665  eturn self.conve
-00000830: 7274 2827 6b69 6c6f 6269 7427 290a 0a20  rt('kilobit').. 
-00000840: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00000850: 2064 6566 206d 6567 6162 6974 7328 7365   def megabits(se
-00000860: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00000870: 5265 7475 726e 7320 7468 6520 7661 6c75  Returns the valu
-00000880: 6520 696e 206d 6567 6162 6974 7322 2222  e in megabits"""
-00000890: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000008a0: 7365 6c66 2e63 6f6e 7665 7274 2827 6d65  self.convert('me
-000008b0: 6761 6269 7427 290a 0a20 2020 2040 7072  gabit')..    @pr
-000008c0: 6f70 6572 7479 0a20 2020 2064 6566 2067  operty.    def g
-000008d0: 6967 6162 6974 7328 7365 6c66 293a 0a20  igabits(self):. 
-000008e0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-000008f0: 7320 7468 6520 7661 6c75 6520 696e 2067  s the value in g
-00000900: 6967 6162 6974 7322 2222 0a20 2020 2020  igabits""".     
-00000910: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
-00000920: 6f6e 7665 7274 2827 6769 6761 6269 7427  onvert('gigabit'
-00000930: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
-00000940: 0a20 2020 2064 6566 2074 6572 6162 6974  .    def terabit
-00000950: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-00000960: 2022 2222 5265 7475 726e 7320 7468 6520   """Returns the 
-00000970: 7661 6c75 6520 696e 2074 6572 6162 6974  value in terabit
-00000980: 7322 2222 0a20 2020 2020 2020 2072 6574  s""".        ret
-00000990: 7572 6e20 7365 6c66 2e63 6f6e 7665 7274  urn self.convert
-000009a0: 2827 7465 7261 6269 7427 290a 0a20 2020  ('terabit')..   
-000009b0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000009c0: 6566 2070 6574 6162 6974 7328 7365 6c66  ef petabits(self
-000009d0: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
-000009e0: 7475 726e 7320 7468 6520 7661 6c75 6520  turns the value 
-000009f0: 696e 2070 6574 6162 6974 7322 2222 0a20  in petabits""". 
-00000a00: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00000a10: 6c66 2e63 6f6e 7665 7274 2827 7065 7461  lf.convert('peta
-00000a20: 6269 7427 290a 0a20 2020 2040 7072 6f70  bit')..    @prop
-00000a30: 6572 7479 0a20 2020 2064 6566 2065 7861  erty.    def exa
-00000a40: 6269 7473 2873 656c 6629 3a0a 2020 2020  bits(self):.    
-00000a50: 2020 2020 2222 2252 6574 7572 6e73 2074      """Returns t
-00000a60: 6865 2076 616c 7565 2069 6e20 6578 6162  he value in exab
-00000a70: 6974 7322 2222 0a20 2020 2020 2020 2072  its""".        r
-00000a80: 6574 7572 6e20 7365 6c66 2e63 6f6e 7665  eturn self.conve
-00000a90: 7274 2827 6578 6162 6974 2729 0a0a 2020  rt('exabit')..  
-00000aa0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00000ab0: 6465 6620 7a65 7461 6269 7473 2873 656c  def zetabits(sel
-00000ac0: 6629 3a0a 2020 2020 2020 2020 2222 2252  f):.        """R
-00000ad0: 6574 7572 6e73 2074 6865 2076 616c 7565  eturns the value
-00000ae0: 2069 6e20 7a65 7461 6269 7473 2222 220a   in zetabits""".
-00000af0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000b00: 656c 662e 636f 6e76 6572 7428 277a 6574  elf.convert('zet
-00000b10: 6162 6974 2729 0a0a 2020 2020 4070 726f  abit')..    @pro
-00000b20: 7065 7274 790a 2020 2020 6465 6620 796f  perty.    def yo
-00000b30: 7474 6162 6974 7328 7365 6c66 293a 0a20  ttabits(self):. 
-00000b40: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00000b50: 7320 7468 6520 7661 6c75 6520 696e 2079  s the value in y
-00000b60: 6f74 7461 6269 7473 2222 220a 2020 2020  ottabits""".    
-00000b70: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00000b80: 636f 6e76 6572 7428 2779 6f74 7461 6269  convert('yottabi
-00000b90: 7427 290a 0a20 2020 2040 7072 6f70 6572  t')..    @proper
-00000ba0: 7479 0a20 2020 2064 6566 2062 7974 6573  ty.    def bytes
-00000bb0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00000bc0: 2222 2252 6574 7572 6e73 2074 6865 2076  """Returns the v
-00000bd0: 616c 7565 2069 6e20 6279 7465 7322 2222  alue in bytes"""
+00000000: 0d0a 636c 6173 7320 4279 7465 436f 6e76  ..class ByteConv
+00000010: 6572 7465 723a 0d0a 2020 2020 2222 220d  erter:..    """.
+00000020: 0a20 2020 2041 2063 6c61 7373 2074 6f20  .    A class to 
+00000030: 636f 6e76 6572 7420 6469 6666 6572 656e  convert differen
+00000040: 7420 756e 6974 7320 6f66 2064 6967 6974  t units of digit
+00000050: 616c 2069 6e66 6f72 6d61 7469 6f6e 2e0d  al information..
+00000060: 0a0d 0a20 2020 202e 2e2e 0d0a 0d0a 2020  ...    .......  
+00000070: 2020 4174 7472 6962 7574 6573 0d0a 2020    Attributes..  
+00000080: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
+00000090: 2020 756e 6974 7320 3a20 6469 6374 0d0a    units : dict..
+000000a0: 2020 2020 2020 2020 6120 6469 6374 696f          a dictio
+000000b0: 6e61 7279 2068 6f6c 6469 6e67 2074 6865  nary holding the
+000000c0: 2063 6f6e 7665 7273 696f 6e20 756e 6974   conversion unit
+000000d0: 730d 0a20 2020 205f 5f62 7974 6573 203a  s..    __bytes :
+000000e0: 2069 6e74 0d0a 2020 2020 2020 2020 6120   int..        a 
+000000f0: 7072 6976 6174 6520 6174 7472 6962 7574  private attribut
+00000100: 6520 746f 2068 6f6c 6420 7468 6520 7661  e to hold the va
+00000110: 6c75 6520 696e 2062 7974 6573 0d0a 0d0a  lue in bytes....
+00000120: 2020 2020 4d65 7468 6f64 730d 0a20 2020      Methods..   
+00000130: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 636f   -------..    co
+00000140: 6e76 6572 7428 756e 6974 290d 0a20 2020  nvert(unit)..   
+00000150: 2020 2020 2043 6f6e 7665 7274 7320 7468       Converts th
+00000160: 6520 6279 7465 7320 7661 6c75 6520 746f  e bytes value to
+00000170: 2074 6865 2073 7065 6369 6669 6564 2075   the specified u
+00000180: 6e69 742e 0d0a 2020 2020 2222 220d 0a20  nit...    """.. 
+00000190: 2020 2023 2044 6963 7469 6f6e 6172 7920     # Dictionary 
+000001a0: 686f 6c64 696e 6720 7468 6520 636f 6e76  holding the conv
+000001b0: 6572 7369 6f6e 2075 6e69 7473 0d0a 2020  ersion units..  
+000001c0: 2020 756e 6974 7320 3d20 7b0d 0a20 2020    units = {..   
+000001d0: 2020 2020 2027 6279 7465 273a 2031 2c0d       'byte': 1,.
+000001e0: 0a20 2020 2020 2020 2027 6b69 6c6f 6279  .        'kiloby
+000001f0: 7465 273a 2031 3032 342c 0d0a 2020 2020  te': 1024,..    
+00000200: 2020 2020 276d 6567 6162 7974 6527 3a20      'megabyte': 
+00000210: 3130 3234 2a2a 322c 0d0a 2020 2020 2020  1024**2,..      
+00000220: 2020 2767 6967 6162 7974 6527 3a20 3130    'gigabyte': 10
+00000230: 3234 2a2a 332c 0d0a 2020 2020 2020 2020  24**3,..        
+00000240: 2774 6572 6162 7974 6527 3a20 3130 3234  'terabyte': 1024
+00000250: 2a2a 342c 0d0a 2020 2020 2020 2020 2770  **4,..        'p
+00000260: 6574 6162 7974 6527 3a20 3130 3234 2a2a  etabyte': 1024**
+00000270: 352c 0d0a 2020 2020 2020 2020 2765 7861  5,..        'exa
+00000280: 6279 7465 273a 2031 3032 342a 2a36 2c0d  byte': 1024**6,.
+00000290: 0a20 2020 2020 2020 2027 7a65 7461 6279  .        'zetaby
+000002a0: 7465 273a 2031 3032 342a 2a37 2c0d 0a20  te': 1024**7,.. 
+000002b0: 2020 2020 2020 2027 796f 7474 6162 7974         'yottabyt
+000002c0: 6527 3a20 3130 3234 2a2a 382c 0d0a 2020  e': 1024**8,..  
+000002d0: 2020 2020 2020 2762 6974 273a 2031 2f38        'bit': 1/8
+000002e0: 2c0d 0a20 2020 2020 2020 2027 6b69 6c6f  ,..        'kilo
+000002f0: 6269 7427 3a20 3130 3234 2f38 2c0d 0a20  bit': 1024/8,.. 
+00000300: 2020 2020 2020 2027 6d65 6761 6269 7427         'megabit'
+00000310: 3a20 2831 3032 342a 2a32 292f 382c 0d0a  : (1024**2)/8,..
+00000320: 2020 2020 2020 2020 2767 6967 6162 6974          'gigabit
+00000330: 273a 2028 3130 3234 2a2a 3329 2f38 2c0d  ': (1024**3)/8,.
+00000340: 0a20 2020 2020 2020 2027 7465 7261 6269  .        'terabi
+00000350: 7427 3a20 2831 3032 342a 2a34 292f 382c  t': (1024**4)/8,
+00000360: 0d0a 2020 2020 2020 2020 2770 6574 6162  ..        'petab
+00000370: 6974 273a 2028 3130 3234 2a2a 3529 2f38  it': (1024**5)/8
+00000380: 2c0d 0a20 2020 2020 2020 2027 6578 6162  ,..        'exab
+00000390: 6974 273a 2028 3130 3234 2a2a 3629 2f38  it': (1024**6)/8
+000003a0: 2c0d 0a20 2020 2020 2020 2027 7a65 7461  ,..        'zeta
+000003b0: 6269 7427 3a20 2831 3032 342a 2a37 292f  bit': (1024**7)/
+000003c0: 382c 0d0a 2020 2020 2020 2020 2779 6f74  8,..        'yot
+000003d0: 7461 6269 7427 3a20 2831 3032 342a 2a38  tabit': (1024**8
+000003e0: 292f 382c 0d0a 2020 2020 7d0d 0a0d 0a20  )/8,..    }.... 
+000003f0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000400: 7365 6c66 2c20 7661 6c75 652c 2075 6e69  self, value, uni
+00000410: 7429 3a0d 0a20 2020 2020 2020 2022 2222  t):..        """
+00000420: 0d0a 2020 2020 2020 2020 436f 6e73 7472  ..        Constr
+00000430: 7563 7473 2061 6c6c 2074 6865 206e 6563  ucts all the nec
+00000440: 6573 7361 7279 2061 7474 7269 6275 7465  essary attribute
+00000450: 7320 666f 7220 7468 6520 4279 7465 436f  s for the ByteCo
+00000460: 6e76 6572 7465 7220 6f62 6a65 6374 2e0d  nverter object..
+00000470: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00000480: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
+00000490: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
+000004a0: 2020 2020 2020 2076 616c 7565 203a 2069         value : i
+000004b0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+000004c0: 2020 2020 7468 6520 7661 6c75 6520 746f      the value to
+000004d0: 2062 6520 636f 6e76 6572 7465 640d 0a20   be converted.. 
+000004e0: 2020 2020 2020 2020 2020 2075 6e69 7420             unit 
+000004f0: 3a20 7374 720d 0a20 2020 2020 2020 2020  : str..         
+00000500: 2020 2020 2020 2074 6865 2075 6e69 7420         the unit 
+00000510: 6f66 2074 6865 2076 616c 7565 2074 6f20  of the value to 
+00000520: 6265 2063 6f6e 7665 7274 6564 0d0a 2020  be converted..  
+00000530: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00000540: 2020 2023 2043 6f6e 7665 7274 2074 6865     # Convert the
+00000550: 2069 6e70 7574 2076 616c 7565 2074 6f20   input value to 
+00000560: 6279 7465 730d 0a20 2020 2020 2020 2073  bytes..        s
+00000570: 656c 662e 5f5f 6279 7465 7320 3d20 7661  elf.__bytes = va
+00000580: 6c75 6520 2a20 7365 6c66 2e75 6e69 7473  lue * self.units
+00000590: 5b75 6e69 745d 0d0a 0d0a 2020 2020 6465  [unit]....    de
+000005a0: 6620 636f 6e76 6572 7428 7365 6c66 2c20  f convert(self, 
+000005b0: 756e 6974 293a 0d0a 2020 2020 2020 2020  unit):..        
+000005c0: 2222 220d 0a20 2020 2020 2020 2043 6f6e  """..        Con
+000005d0: 7665 7274 7320 7468 6520 6279 7465 7320  verts the bytes 
+000005e0: 7661 6c75 6520 746f 2074 6865 2073 7065  value to the spe
+000005f0: 6369 6669 6564 2075 6e69 742e 0d0a 0d0a  cified unit.....
+00000600: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00000610: 7273 0d0a 2020 2020 2020 2020 2d2d 2d2d  rs..        ----
+00000620: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00000630: 2020 2020 756e 6974 203a 2073 7472 0d0a      unit : str..
+00000640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000650: 7468 6520 756e 6974 2074 6f20 7768 6963  the unit to whic
+00000660: 6820 7468 6520 7661 6c75 6520 6973 2074  h the value is t
+00000670: 6f20 6265 2063 6f6e 7665 7274 6564 0d0a  o be converted..
+00000680: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00000690: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+000006a0: 2d2d 0d0a 2020 2020 2020 2020 2020 2020  --..            
+000006b0: 666c 6f61 740d 0a20 2020 2020 2020 2020  float..         
+000006c0: 2020 2020 2020 2074 6865 2063 6f6e 7665         the conve
+000006d0: 7274 6564 2076 616c 7565 0d0a 2020 2020  rted value..    
+000006e0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000006f0: 2023 2043 6f6e 7665 7274 2074 6865 2062   # Convert the b
+00000700: 7974 6573 2076 616c 7565 2074 6f20 7468  ytes value to th
+00000710: 6520 7370 6563 6966 6965 6420 756e 6974  e specified unit
+00000720: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000730: 2073 656c 662e 5f5f 6279 7465 7320 2f20   self.__bytes / 
+00000740: 7365 6c66 2e75 6e69 7473 5b75 6e69 745d  self.units[unit]
+00000750: 0d0a 0d0a 2020 2020 2320 4265 6c6f 7720  ....    # Below 
+00000760: 6172 6520 7072 6f70 6572 7479 206d 6574  are property met
+00000770: 686f 6473 2074 6861 7420 7265 7475 726e  hods that return
+00000780: 2074 6865 2076 616c 7565 2069 6e20 6120   the value in a 
+00000790: 7370 6563 6966 6963 2075 6e69 740d 0a0d  specific unit...
+000007a0: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+000007b0: 2020 2020 6465 6620 6269 7473 2873 656c      def bits(sel
+000007c0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
+000007d0: 5265 7475 726e 7320 7468 6520 7661 6c75  Returns the valu
+000007e0: 6520 696e 2062 6974 7322 2222 0d0a 2020  e in bits"""..  
+000007f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00000800: 662e 636f 6e76 6572 7428 2762 6974 2729  f.convert('bit')
+00000810: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
+00000820: 790d 0a20 2020 2064 6566 206b 696c 6f62  y..    def kilob
+00000830: 6974 7328 7365 6c66 293a 0d0a 2020 2020  its(self):..    
+00000840: 2020 2020 2222 2252 6574 7572 6e73 2074      """Returns t
+00000850: 6865 2076 616c 7565 2069 6e20 6b69 6c6f  he value in kilo
+00000860: 6269 7473 2222 220d 0a20 2020 2020 2020  bits"""..       
+00000870: 2072 6574 7572 6e20 7365 6c66 2e63 6f6e   return self.con
+00000880: 7665 7274 2827 6b69 6c6f 6269 7427 290d  vert('kilobit').
+00000890: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+000008a0: 0d0a 2020 2020 6465 6620 6d65 6761 6269  ..    def megabi
+000008b0: 7473 2873 656c 6629 3a0d 0a20 2020 2020  ts(self):..     
+000008c0: 2020 2022 2222 5265 7475 726e 7320 7468     """Returns th
+000008d0: 6520 7661 6c75 6520 696e 206d 6567 6162  e value in megab
+000008e0: 6974 7322 2222 0d0a 2020 2020 2020 2020  its"""..        
+000008f0: 7265 7475 726e 2073 656c 662e 636f 6e76  return self.conv
+00000900: 6572 7428 276d 6567 6162 6974 2729 0d0a  ert('megabit')..
+00000910: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
+00000920: 0a20 2020 2064 6566 2067 6967 6162 6974  .    def gigabit
+00000930: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
+00000940: 2020 2222 2252 6574 7572 6e73 2074 6865    """Returns the
+00000950: 2076 616c 7565 2069 6e20 6769 6761 6269   value in gigabi
+00000960: 7473 2222 220d 0a20 2020 2020 2020 2072  ts"""..        r
+00000970: 6574 7572 6e20 7365 6c66 2e63 6f6e 7665  eturn self.conve
+00000980: 7274 2827 6769 6761 6269 7427 290d 0a0d  rt('gigabit')...
+00000990: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+000009a0: 2020 2020 6465 6620 7465 7261 6269 7473      def terabits
+000009b0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000009c0: 2022 2222 5265 7475 726e 7320 7468 6520   """Returns the 
+000009d0: 7661 6c75 6520 696e 2074 6572 6162 6974  value in terabit
+000009e0: 7322 2222 0d0a 2020 2020 2020 2020 7265  s"""..        re
+000009f0: 7475 726e 2073 656c 662e 636f 6e76 6572  turn self.conver
+00000a00: 7428 2774 6572 6162 6974 2729 0d0a 0d0a  t('terabit')....
+00000a10: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+00000a20: 2020 2064 6566 2070 6574 6162 6974 7328     def petabits(
+00000a30: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000a40: 2222 2252 6574 7572 6e73 2074 6865 2076  """Returns the v
+00000a50: 616c 7565 2069 6e20 7065 7461 6269 7473  alue in petabits
+00000a60: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+00000a70: 7572 6e20 7365 6c66 2e63 6f6e 7665 7274  urn self.convert
+00000a80: 2827 7065 7461 6269 7427 290d 0a0d 0a20  ('petabit').... 
+00000a90: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
+00000aa0: 2020 6465 6620 6578 6162 6974 7328 7365    def exabits(se
+00000ab0: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
+00000ac0: 2252 6574 7572 6e73 2074 6865 2076 616c  "Returns the val
+00000ad0: 7565 2069 6e20 6578 6162 6974 7322 2222  ue in exabits"""
+00000ae0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000af0: 2073 656c 662e 636f 6e76 6572 7428 2765   self.convert('e
+00000b00: 7861 6269 7427 290d 0a0d 0a20 2020 2040  xabit')....    @
+00000b10: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+00000b20: 6620 7a65 7461 6269 7473 2873 656c 6629  f zetabits(self)
+00000b30: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+00000b40: 7475 726e 7320 7468 6520 7661 6c75 6520  turns the value 
+00000b50: 696e 207a 6574 6162 6974 7322 2222 0d0a  in zetabits"""..
+00000b60: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00000b70: 656c 662e 636f 6e76 6572 7428 277a 6574  elf.convert('zet
+00000b80: 6162 6974 2729 0d0a 0d0a 2020 2020 4070  abit')....    @p
+00000b90: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00000ba0: 2079 6f74 7461 6269 7473 2873 656c 6629   yottabits(self)
+00000bb0: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+00000bc0: 7475 726e 7320 7468 6520 7661 6c75 6520  turns the value 
+00000bd0: 696e 2079 6f74 7461 6269 7473 2222 220d  in yottabits""".
 00000be0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000bf0: 7365 6c66 2e63 6f6e 7665 7274 2827 6279  self.convert('by
-00000c00: 7465 2729 0a0a 2020 2020 4070 726f 7065  te')..    @prope
-00000c10: 7274 790a 2020 2020 6465 6620 6b69 6c6f  rty.    def kilo
-00000c20: 6279 7465 7328 7365 6c66 293a 0a20 2020  bytes(self):.   
-00000c30: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
-00000c40: 7468 6520 7661 6c75 6520 696e 206b 696c  the value in kil
-00000c50: 6f62 7974 6573 2222 220a 2020 2020 2020  obytes""".      
-00000c60: 2020 7265 7475 726e 2073 656c 662e 636f    return self.co
-00000c70: 6e76 6572 7428 276b 696c 6f62 7974 6527  nvert('kilobyte'
-00000c80: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
-00000c90: 0a20 2020 2064 6566 206d 6567 6162 7974  .    def megabyt
-00000ca0: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
-00000cb0: 2020 2222 2252 6574 7572 6e73 2074 6865    """Returns the
-00000cc0: 2076 616c 7565 2069 6e20 6d65 6761 6279   value in megaby
-00000cd0: 7465 7322 2222 0a20 2020 2020 2020 2072  tes""".        r
-00000ce0: 6574 7572 6e20 7365 6c66 2e63 6f6e 7665  eturn self.conve
-00000cf0: 7274 2827 6d65 6761 6279 7465 2729 0a0a  rt('megabyte')..
-00000d00: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00000d10: 2020 6465 6620 6769 6761 6279 7465 7328    def gigabytes(
-00000d20: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00000d30: 2222 5265 7475 726e 7320 7468 6520 7661  ""Returns the va
-00000d40: 6c75 6520 696e 2067 6967 6162 7974 6573  lue in gigabytes
-00000d50: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00000d60: 726e 2073 656c 662e 636f 6e76 6572 7428  rn self.convert(
-00000d70: 2767 6967 6162 7974 6527 290a 0a20 2020  'gigabyte')..   
-00000d80: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00000d90: 6566 2074 6572 6162 7974 6573 2873 656c  ef terabytes(sel
-00000da0: 6629 3a0a 2020 2020 2020 2020 2222 2252  f):.        """R
-00000db0: 6574 7572 6e73 2074 6865 2076 616c 7565  eturns the value
-00000dc0: 2069 6e20 7465 7261 6279 7465 7322 2222   in terabytes"""
-00000dd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000de0: 7365 6c66 2e63 6f6e 7665 7274 2827 7465  self.convert('te
-00000df0: 7261 6279 7465 2729 0a0a 2020 2020 4070  rabyte')..    @p
-00000e00: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00000e10: 7065 7461 6279 7465 7328 7365 6c66 293a  petabytes(self):
-00000e20: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00000e30: 726e 7320 7468 6520 7661 6c75 6520 696e  rns the value in
-00000e40: 2070 6574 6162 7974 6573 2222 220a 2020   petabytes""".  
-00000e50: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00000e60: 662e 636f 6e76 6572 7428 2770 6574 6162  f.convert('petab
-00000e70: 7974 6527 290a 0a20 2020 2040 7072 6f70  yte')..    @prop
-00000e80: 6572 7479 0a20 2020 2064 6566 2065 7861  erty.    def exa
-00000e90: 6279 7465 7328 7365 6c66 293a 0a20 2020  bytes(self):.   
-00000ea0: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
-00000eb0: 7468 6520 7661 6c75 6520 696e 2065 7861  the value in exa
-00000ec0: 6279 7465 7322 2222 0a20 2020 2020 2020  bytes""".       
-00000ed0: 2072 6574 7572 6e20 7365 6c66 2e63 6f6e   return self.con
-00000ee0: 7665 7274 2827 6578 6162 7974 6527 290a  vert('exabyte').
-00000ef0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00000f00: 2020 2064 6566 207a 6574 6162 7974 6573     def zetabytes
-00000f10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00000f20: 2222 2252 6574 7572 6e73 2074 6865 2076  """Returns the v
-00000f30: 616c 7565 2069 6e20 7a65 7461 6279 7465  alue in zetabyte
-00000f40: 7322 2222 0a20 2020 2020 2020 2072 6574  s""".        ret
-00000f50: 7572 6e20 7365 6c66 2e63 6f6e 7665 7274  urn self.convert
-00000f60: 2827 7a65 7461 6279 7465 2729 0a0a 2020  ('zetabyte')..  
-00000f70: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00000f80: 6465 6620 796f 7474 6162 7974 6573 2873  def yottabytes(s
-00000f90: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00000fa0: 2252 6574 7572 6e73 2074 6865 2076 616c  "Returns the val
-00000fb0: 7565 2069 6e20 796f 7474 6162 7974 6573  ue in yottabytes
-00000fc0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00000fd0: 726e 2073 656c 662e 636f 6e76 6572 7428  rn self.convert(
-00000fe0: 2779 6f74 7461 6279 7465 2729 0a         'yottabyte').
+00000bf0: 7365 6c66 2e63 6f6e 7665 7274 2827 796f  self.convert('yo
+00000c00: 7474 6162 6974 2729 0d0a 0d0a 2020 2020  ttabit')....    
+00000c10: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00000c20: 6566 2062 7974 6573 2873 656c 6629 3a0d  ef bytes(self):.
+00000c30: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00000c40: 726e 7320 7468 6520 7661 6c75 6520 696e  rns the value in
+00000c50: 2062 7974 6573 2222 220d 0a20 2020 2020   bytes"""..     
+00000c60: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
+00000c70: 6f6e 7665 7274 2827 6279 7465 2729 0d0a  onvert('byte')..
+00000c80: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
+00000c90: 0a20 2020 2064 6566 206b 696c 6f62 7974  .    def kilobyt
+00000ca0: 6573 2873 656c 6629 3a0d 0a20 2020 2020  es(self):..     
+00000cb0: 2020 2022 2222 5265 7475 726e 7320 7468     """Returns th
+00000cc0: 6520 7661 6c75 6520 696e 206b 696c 6f62  e value in kilob
+00000cd0: 7974 6573 2222 220d 0a20 2020 2020 2020  ytes"""..       
+00000ce0: 2072 6574 7572 6e20 7365 6c66 2e63 6f6e   return self.con
+00000cf0: 7665 7274 2827 6b69 6c6f 6279 7465 2729  vert('kilobyte')
+00000d00: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
+00000d10: 790d 0a20 2020 2064 6566 206d 6567 6162  y..    def megab
+00000d20: 7974 6573 2873 656c 6629 3a0d 0a20 2020  ytes(self):..   
+00000d30: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
+00000d40: 7468 6520 7661 6c75 6520 696e 206d 6567  the value in meg
+00000d50: 6162 7974 6573 2222 220d 0a20 2020 2020  abytes"""..     
+00000d60: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
+00000d70: 6f6e 7665 7274 2827 6d65 6761 6279 7465  onvert('megabyte
+00000d80: 2729 0d0a 0d0a 2020 2020 4070 726f 7065  ')....    @prope
+00000d90: 7274 790d 0a20 2020 2064 6566 2067 6967  rty..    def gig
+00000da0: 6162 7974 6573 2873 656c 6629 3a0d 0a20  abytes(self):.. 
+00000db0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+00000dc0: 7320 7468 6520 7661 6c75 6520 696e 2067  s the value in g
+00000dd0: 6967 6162 7974 6573 2222 220d 0a20 2020  igabytes"""..   
+00000de0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00000df0: 2e63 6f6e 7665 7274 2827 6769 6761 6279  .convert('gigaby
+00000e00: 7465 2729 0d0a 0d0a 2020 2020 4070 726f  te')....    @pro
+00000e10: 7065 7274 790d 0a20 2020 2064 6566 2074  perty..    def t
+00000e20: 6572 6162 7974 6573 2873 656c 6629 3a0d  erabytes(self):.
+00000e30: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00000e40: 726e 7320 7468 6520 7661 6c75 6520 696e  rns the value in
+00000e50: 2074 6572 6162 7974 6573 2222 220d 0a20   terabytes""".. 
+00000e60: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00000e70: 6c66 2e63 6f6e 7665 7274 2827 7465 7261  lf.convert('tera
+00000e80: 6279 7465 2729 0d0a 0d0a 2020 2020 4070  byte')....    @p
+00000e90: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00000ea0: 2070 6574 6162 7974 6573 2873 656c 6629   petabytes(self)
+00000eb0: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+00000ec0: 7475 726e 7320 7468 6520 7661 6c75 6520  turns the value 
+00000ed0: 696e 2070 6574 6162 7974 6573 2222 220d  in petabytes""".
+00000ee0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000ef0: 7365 6c66 2e63 6f6e 7665 7274 2827 7065  self.convert('pe
+00000f00: 7461 6279 7465 2729 0d0a 0d0a 2020 2020  tabyte')....    
+00000f10: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00000f20: 6566 2065 7861 6279 7465 7328 7365 6c66  ef exabytes(self
+00000f30: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
+00000f40: 6574 7572 6e73 2074 6865 2076 616c 7565  eturns the value
+00000f50: 2069 6e20 6578 6162 7974 6573 2222 220d   in exabytes""".
+00000f60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000f70: 7365 6c66 2e63 6f6e 7665 7274 2827 6578  self.convert('ex
+00000f80: 6162 7974 6527 290d 0a0d 0a20 2020 2040  abyte')....    @
+00000f90: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+00000fa0: 6620 7a65 7461 6279 7465 7328 7365 6c66  f zetabytes(self
+00000fb0: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
+00000fc0: 6574 7572 6e73 2074 6865 2076 616c 7565  eturns the value
+00000fd0: 2069 6e20 7a65 7461 6279 7465 7322 2222   in zetabytes"""
+00000fe0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000ff0: 2073 656c 662e 636f 6e76 6572 7428 277a   self.convert('z
+00001000: 6574 6162 7974 6527 290d 0a0d 0a20 2020  etabyte')....   
+00001010: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
+00001020: 6465 6620 796f 7474 6162 7974 6573 2873  def yottabytes(s
+00001030: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
+00001040: 2222 5265 7475 726e 7320 7468 6520 7661  ""Returns the va
+00001050: 6c75 6520 696e 2079 6f74 7461 6279 7465  lue in yottabyte
+00001060: 7322 2222 0d0a 2020 2020 2020 2020 7265  s"""..        re
+00001070: 7475 726e 2073 656c 662e 636f 6e76 6572  turn self.conver
+00001080: 7428 2779 6f74 7461 6279 7465 2729 0d0a  t('yottabyte')..
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/core/errors/version.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/core/errors/version.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-class InvalidPreReleaseTypeError(Exception):
-
-    message = "The pre-release type found in the VERSION file is not valid."
-
-    def __init__(self, message=None, pr_type=None, skip_print=False):
-        """
-        The __init__ function is the constructor for a class. It is called whenever
-        an instance of a class is created.
-
-        The __init__ function can take arguments, but those arguments are only
-        stored as attributes on the instance.
-
-        Arguments:
-            message (:class:`str`):
-                Provide a custom message for the exception. (Optional, defaults to
-                ``None``)
-
-            pr_type (:class:`str`):
-                The pre-release type found in the VERSION file. (Optional, defaults
-                to ``None``)
-
-            skip_print (:class:`bool`)
-                Prevent the printing of an error message when the exception is
-                raised in a try/except block. (Optional, defaults to ``False``).
-        """
-        if pr_type:
-            self.message = f'The provided pre-release type "{pr_type}" is not valid.'
-        if message:
-            self.message += f"Addditional information from the caller: {message}"
-
-        if not skip_print:
-            print(self.message)
-
-
-
-
-class VersionInfoMismatchError(Exception):
-    message = 'The version number does not match the concatenation of the ' \
-              'minor, major, and patch numbers.'
-
-    def __init__(
-            self,
-            version_number: str,
-            concatenated: str,
-            message=None,
-            skip_print=False,
-            *args, **kwargs):
-        """
-        The :class:`VersionInfoMismatchError` class is used to raise an error if the
-        version number does not match the concatenation of the minor, major,
-        and patch numbers.
-
-        Arguments:
-            version_number:
-                The version number of the current version of
-                                       inspyre_toolbox
-
-        Args:
-            self:
-            version_number:
-            concatenated:
-            message:
-            skip_print:
-            *args:
-            **kwargs:
-
-        Returns:
-
-        """
-        mismatch_statement = f"Ver. Number: {version_number} | " \
-                             f"Concatenated: {concatenated}"
-        from_caller = f"Additional information from caller: {message}" if message else ""
-        self.message = \
-            message or f"{self.message}\n{mismatch_statement}\n{from_caller}"
-        super().__init__(self.message, *args, **kwargs)
+class InvalidPreReleaseTypeError(Exception):
+
+    message = "The pre-release type found in the VERSION file is not valid."
+
+    def __init__(self, message=None, pr_type=None, skip_print=False):
+        """
+        The __init__ function is the constructor for a class. It is called whenever
+        an instance of a class is created.
+
+        The __init__ function can take arguments, but those arguments are only
+        stored as attributes on the instance.
+
+        Arguments:
+            message (:class:`str`):
+                Provide a custom message for the exception. (Optional, defaults to
+                ``None``)
+
+            pr_type (:class:`str`):
+                The pre-release type found in the VERSION file. (Optional, defaults
+                to ``None``)
+
+            skip_print (:class:`bool`)
+                Prevent the printing of an error message when the exception is
+                raised in a try/except block. (Optional, defaults to ``False``).
+        """
+        if pr_type:
+            self.message = f'The provided pre-release type "{pr_type}" is not valid.'
+        if message:
+            self.message += f"Addditional information from the caller: {message}"
+
+        if not skip_print:
+            print(self.message)
+
+
+
+
+class VersionInfoMismatchError(Exception):
+    message = 'The version number does not match the concatenation of the ' \
+              'minor, major, and patch numbers.'
+
+    def __init__(
+            self,
+            version_number: str,
+            concatenated: str,
+            message=None,
+            skip_print=False,
+            *args, **kwargs):
+        """
+        The :class:`VersionInfoMismatchError` class is used to raise an error if the
+        version number does not match the concatenation of the minor, major,
+        and patch numbers.
+
+        Arguments:
+            version_number:
+                The version number of the current version of
+                                       inspyre_toolbox
+
+        Args:
+            self:
+            version_number:
+            concatenated:
+            message:
+            skip_print:
+            *args:
+            **kwargs:
+
+        Returns:
+
+        """
+        mismatch_statement = f"Ver. Number: {version_number} | " \
+                             f"Concatenated: {concatenated}"
+        from_caller = f"Additional information from caller: {message}" if message else ""
+        self.message = \
+            message or f"{self.message}\n{mismatch_statement}\n{from_caller}"
+        super().__init__(self.message, *args, **kwargs)
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/docs/conversions/bytes.md` & `inspyre_toolbox-1.4.1/inspyre_toolbox/docs/conversions/bytes.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-
-# ByteConverter Class Documentation
-
-## Overview
-The `ByteConverter` class is designed to facilitate the conversion between different units of digital information. This utility can be particularly useful in various programming and data processing scenarios where handling data sizes in different units is necessary.
-
-## Features
-- Supports conversion between bytes, kilobytes, megabytes, gigabytes, terabytes, petabytes, exabytes, zetabytes, yottabytes, bits, kilobits, megabits, gigabits, terabits, petabits, exabits, zetabits, and yottabits.
-- Easy to use with a straightforward initialization and conversion method.
-
-## Class Attributes
-- `units`: A dictionary holding the conversion ratios for different units of digital information.
-
-## Methods
-### `__init__(self, value, unit)`
-Initializes a new instance of the `ByteConverter` class.
-
-#### Parameters
-- `value` : `int`  
-  The numeric value to be converted.
-- `unit` : `str`  
-  The unit of the initial value.
-
-### `convert(self, unit)`
-Converts the stored digital information value to the specified unit.
-
-#### Parameters
-- `unit` : `str`  
-  The unit to which the value is to be converted.
-
-#### Returns
-- `float`  
-  The converted value in the specified unit.
-
-## Property Methods
-The class also provides property methods for each unit, allowing easy access to the value in any supported unit without explicitly calling the convert method.
-
-## Usage Examples
-### Converting Bytes to Megabytes
-```python
-converter = ByteConverter(2048, 'byte')
-print(converter.convert('megabyte'))  # Output: 0.001953125
-```
-
-### Initializing with Gigabytes and Accessing Value in Terabytes
-```python
-converter = ByteConverter(1, 'gigabyte')
-print(converter.terabytes)  # Output: 0.0009765625
-```
-
-This class is an effective tool for anyone needing to work with digital information units, offering flexibility and ease of use for various programming needs.
+
+# ByteConverter Class Documentation
+
+## Overview
+The `ByteConverter` class is designed to facilitate the conversion between different units of digital information. This utility can be particularly useful in various programming and data processing scenarios where handling data sizes in different units is necessary.
+
+## Features
+- Supports conversion between bytes, kilobytes, megabytes, gigabytes, terabytes, petabytes, exabytes, zetabytes, yottabytes, bits, kilobits, megabits, gigabits, terabits, petabits, exabits, zetabits, and yottabits.
+- Easy to use with a straightforward initialization and conversion method.
+
+## Class Attributes
+- `units`: A dictionary holding the conversion ratios for different units of digital information.
+
+## Methods
+### `__init__(self, value, unit)`
+Initializes a new instance of the `ByteConverter` class.
+
+#### Parameters
+- `value` : `int`  
+  The numeric value to be converted.
+- `unit` : `str`  
+  The unit of the initial value.
+
+### `convert(self, unit)`
+Converts the stored digital information value to the specified unit.
+
+#### Parameters
+- `unit` : `str`  
+  The unit to which the value is to be converted.
+
+#### Returns
+- `float`  
+  The converted value in the specified unit.
+
+## Property Methods
+The class also provides property methods for each unit, allowing easy access to the value in any supported unit without explicitly calling the convert method.
+
+## Usage Examples
+### Converting Bytes to Megabytes
+```python
+converter = ByteConverter(2048, 'byte')
+print(converter.convert('megabyte'))  # Output: 0.001953125
+```
+
+### Initializing with Gigabytes and Accessing Value in Terabytes
+```python
+converter = ByteConverter(1, 'gigabyte')
+print(converter.terabytes)  # Output: 0.0009765625
+```
+
+This class is an effective tool for anyone needing to work with digital information units, offering flexibility and ease of use for various programming needs.
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/generations/__init__.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/generations/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-"""
-Inspyre-Toolbox Generations Module
-
-This module is part of the Inspyre-Toolbox project. It provides functionalities
-for generating random decimal numbers within a specified range. The main function
-in this module, `generate_random_decimal`, can generate a specified number of
-random decimal numbers, each within a given range.
-
-This module can be useful for various applications, such as creating random
-datasets for testing, generating noise for simulations, or any other situation
-where random decimal numbers are needed.
-
-Function:
-
-generate_random_decimal(number_of_results=1, minimum=0, maximum=1, force_list=False):
-Generates a list of random decimal numbers within a specified range.
-This module is released under The MIT License.
-
-Project: Inspyre-Toolbox
-Author: Inspyre Softworks - https://inspyre.tech
-Created: 5/11/2023 @ 7:48 PM
-File:
-  Name: init.py
-  Path: inspyre_toolbox/generations
-"""
-import random
-
-
-def generate_random_decimal(number_of_results=1, minimum=0, maximum=1, force_list=False):
-    """
-    Generates a list of random decimal numbers within a specified range.
-
-    This function generates a list of random decimal numbers, each of which is
-    between the specified minimum and maximum values. If only one number is
-    requested, the function returns that number directly unless 'force_list'
-    is set to True, in which case a list containing that number is returned.
-
-    Arguments:
-        number_of_results (int, optional): The number of random numbers to generate.
-            (default: 1)
-        minimum (float, optional): The lower bound for the random numbers.
-            (default: 0)
-        maximum (float, optional): The upper bound for the random numbers.
-            (default: 1)
-        force_list (bool, optional): Whether to always return a list, even when
-            only one number is generated. (default: False)
-
-    Returns:
-        float or list of float: A list of random decimal numbers. If only one
-            number is generated and 'force_list' is False, that number is
-            returned directly.
-    """
-    res = [random.uniform(minimum, maximum) for _ in range(number_of_results)]
-    return res[0] if number_of_results == 1 and not force_list else res
-
-
-
-"""
-The MIT License (MIT)
-Copyright © 2023 Inspyre Softworks - https://inspyre.tech
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
+"""
+Inspyre-Toolbox Generations Module
+
+This module is part of the Inspyre-Toolbox project. It provides functionalities
+for generating random decimal numbers within a specified range. The main function
+in this module, `generate_random_decimal`, can generate a specified number of
+random decimal numbers, each within a given range.
+
+This module can be useful for various applications, such as creating random
+datasets for testing, generating noise for simulations, or any other situation
+where random decimal numbers are needed.
+
+Function:
+
+generate_random_decimal(number_of_results=1, minimum=0, maximum=1, force_list=False):
+Generates a list of random decimal numbers within a specified range.
+This module is released under The MIT License.
+
+Project: Inspyre-Toolbox
+Author: Inspyre Softworks - https://inspyre.tech
+Created: 5/11/2023 @ 7:48 PM
+File:
+  Name: init.py
+  Path: inspyre_toolbox/generations
+"""
+import random
+
+
+def generate_random_decimal(number_of_results=1, minimum=0, maximum=1, force_list=False):
+    """
+    Generates a list of random decimal numbers within a specified range.
+
+    This function generates a list of random decimal numbers, each of which is
+    between the specified minimum and maximum values. If only one number is
+    requested, the function returns that number directly unless 'force_list'
+    is set to True, in which case a list containing that number is returned.
+
+    Arguments:
+        number_of_results (int, optional): The number of random numbers to generate.
+            (default: 1)
+        minimum (float, optional): The lower bound for the random numbers.
+            (default: 0)
+        maximum (float, optional): The upper bound for the random numbers.
+            (default: 1)
+        force_list (bool, optional): Whether to always return a list, even when
+            only one number is generated. (default: False)
+
+    Returns:
+        float or list of float: A list of random decimal numbers. If only one
+            number is generated and 'force_list' is False, that number is
+            returned directly.
+    """
+    res = [random.uniform(minimum, maximum) for _ in range(number_of_results)]
+    return res[0] if number_of_results == 1 and not force_list else res
+
+
+
+"""
+The MIT License (MIT)
+Copyright © 2023 Inspyre Softworks - https://inspyre.tech
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/live_timer/__init__.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,283 +1,283 @@
-"""
-File: inspyre_toolbox/live_timer/__init__.py
-Created: ??
-
-Description:
-    inspyre_toolbox.live_timer gives you access to a class and functions that make running a live
-    timer that's not only easily to initialize, but easy to query, reset, and pause your timers.
-    This module also contains a class named 'TimerHistory' that keeps a history of all timer actions.
-    
-    To find out more about usage please see:
-    
-    GIT_REPO_ROOT/examples/live_timer
-
-"""
-
-from time import time
-
-from inspyre_toolbox.core_helpers.logging import ROOT_ISL_DEVICE, add_isl_child
-from inspyre_toolbox.live_timer.errors import TimerNotRunningError, TimerNotStartedError
-from inspyre_toolbox.live_timer.history import TimerHistory
-
-LOG_NAME = 'InspyreToolbox.live_timer'
-
-LOG = add_isl_child(LOG_NAME)
-
-#ROOT_ISL_DEVICE.adjust_level('debug')
-
-LOG.debug('Log started!')
-
-
-def format_seconds_to_hhmmss(seconds):
-    """
-    The format_seconds_to_hhmmss function accepts a number of seconds and returns a string
-    representing the amount of time represented by those seconds in HH:MM:SS format.
-
-    Args:
-        seconds (int):
-            The number of seconds to be converted. (Required)
-
-    Returns:
-        A string with the number of hours, minutes and seconds
-    """
-    hours = seconds // (60 * 60)
-    seconds %= (60 * 60)
-    minutes = seconds // 60
-    seconds %= 60
-    return "%02i:%02i:%02i" % (hours, minutes, seconds)
-
-
-class Timer(object):
-    def __repr__(self):
-        statement = "Timer(" \
-                    f"Started: {self.started} |"
-        if self.started:
-            runtime = time() - self.start_time
-            runtime = format_seconds_to_hhmmss(runtime)
-            statement += f" Started: {self.start_time} - Current Runtime: {runtime}"
-
-    def __init__(self, auto_start=False, history=None):
-
-        self.log_name = f'{LOG_NAME}.Timer'
-
-        # Set up logger
-        self.log = add_isl_child(self.log_name)
-
-        # Define some default attribute values
-
-        self.running = False
-        self.mark_2 = None
-        self.pause_end = None
-        self.pause_start = time()
-        self.paused = False
-        self.start_time = None
-        self.started = False
-        self.stopped = False
-        self.total_pause_time = 0
-        self.was_paused = False
-
-        self.log.debug('Set up class attributes.')
-
-        # Start a Timer history object to track times for resets
-        self.history = TimerHistory(self.__get_elapsed) if history is None else history
-
-        self.log.debug('Timer class instantiated!')
-
-    def __get_elapsed(self, ts=None, sans_pause: bool = False, seconds=False):
-        """
-        The __get_elapsed function is a private function that is called by the public functions
-        start(), pause(), and stop(). It returns the elapsed time in seconds, or as a string if
-        seconds=False. The __get_elapsed function does not take any parameters. If you call this
-        private function directly, it will return an error
-
-        Args:
-            self:
-                Access variables that belongs to the class
-
-            ts (int|float):
-                Pass in the current timestamp, (Optional, defaults to time.time())
-
-            sans_pause (bool):
-                Determine whether or not to include the time that the timer was
-                paused in the elapsed time. (Optional; defaults to True)
-
-            seconds (bool):
-                Return the elapsed time as number of seconds. (Optional; defaults
-                to False)
-
-        Returns:
-            The time elapsed since the start of the timer
-        """
-        log = add_isl_child(f'{self.log_name}__get_elapsed')
-
-        diff_time = self.start_time if ts is None else ts
-
-        # ver1.2.7
-        # If we were running but are now stopped, we will skip marking
-        if not self.stopped:
-            self.mark_2 = time()
-
-        diff = self.mark_2 - diff_time
-
-        if sans_pause:
-            return format_seconds_to_hhmmss(diff)
-
-        tpt = 0
-        # print(self.total_pause_time)
-        if self.paused:
-            tpt += time() - self.pause_start
-
-        tpt += self.total_pause_time
-        diff = diff - tpt
-
-        return diff if seconds else format_seconds_to_hhmmss(diff)
-
-    def get_elapsed(self, *args, **kwargs):
-        """
-        The get_elapsed function returns the elapsed time since the timer was started.
-        If the timer is not running, it returns None. If it has been stopped,
-        it returns the elapsed time from start to stop.
-
-        Args:
-            self: Access the attributes and methods of the class in python
-            *args: Pass a non-keyworded, variable-length argument list
-            **kwargs: Pass a keyworded, variable-length argument list
-
-        Returns:
-            The current elapsed time since the timer was started
-
-        """
-        if not self.running and self.stopped or self.running:
-            self.history.add("QUERY")
-            return self.__get_elapsed(*args, **kwargs)
-        else:
-            try:
-                raise TimerNotStartedError(skip_print=True)
-            except TimerNotStartedError as e:
-                print(e.message)
-
-    def reset(self):
-        """
-
-        Reset the 'self.start_time' attribute to this moment, effectively resetting the timer to '00:00:00'
-
-        """
-        self.history.add(action="RESET")
-
-        return Timer(history=self.history)
-
-        # if self.running:
-        #     self.stop()
-        # self.total_pause_time = 0
-        # self.pause_start = None
-        # self.pause_end = None
-        # self.started = False
-
-    def restart(self):
-        """
-        The restart function resets the timer to its original state and starts it
-        running.
-
-        Returns:
-            None
-        """
-        self.reset()
-        if not self.started:
-            self.start()
-
-    def start(self):
-        """
-
-        Store the time the thread was started and assign the attribute 'self.started' to 'True' to indicate this.
-
-        """
-        self.start_time = time()
-        self.started = True
-        self.history.add()
-        self.running = True
-
-    def pause(self):
-        """
-
-        Pause the running timer.
-
-        This function will pause the running timer.
-
-        What this really means in this context is that this function will fill the
-        'self.pause_start' time with the current time. When you unpause at a later
-        time the 'self.unpause' function will reference 'self.pause_start' for
-        comparison.
-
-        Note:
-            This function also sets the 'self.paused' variable to 'True'.
-
-        """
-        if not self.started:
-            raise TimerNotStartedError()
-        if not self.running:
-            raise TimerNotRunningError()
-        if self.paused:
-            return False
-        self.pause_start = time()
-        self.paused = True
-        self.was_paused = True
-        self.history.add("PAUSE")
-
-    def unpause(self):
-        """
-
-        Un-Pause the running timer.
-
-        This function will unpause the running timer. What that really means in this
-        context is that since it marks the time that one paused the timer previously
-        and this will compare the time elapsed between when the pause function
-        was called and when this is called and keeps track of it.
-
-        Whenever get_elapsed is called, it looks at the amount of seconds that
-        have been added by this function's operation process and removes that
-        total from the number of seconds elapsed before passing them to be
-        naturalized.
-
-        Returns:
-            bool:
-                If;
-                    * True:
-                        The timer was successfully un-paused
-                    * False:
-                        The timer was no successfully un-paused (most likely due to its
-                        state not actually being paused),
-        """
-        if not self.started:
-            raise TimerNotStartedError()
-        if not self.running:
-            raise TimerNotRunningError()
-        if self.paused:
-            self.pause_end = time()
-            diff = self.pause_end - self.pause_start
-            self.total_pause_time += diff
-            self.paused = False
-            self.history.add("UNPAUSE")
-            return True
-        else:
-            return False
-
-    def stop(self):
-        """
-        The 'stop' function stops the timer, but leaves it in a paused state.
-        The 'resume' function resumes the timer from where it was stopped.
-
-        Args:
-            self: Reference the object itself
-
-        Returns:
-            The time when the timer is stopped
-        """
-        if not self.started:
-            raise TimerNotStartedError()
-        if self.running:
-            self.running = False
-            self.paused = False
-            self.stopped = True
-            self.mark_2 = time()
-        else:
-            raise TimerNotRunningError()
+"""
+File: inspyre_toolbox/live_timer/__init__.py
+Created: ??
+
+Description:
+    inspyre_toolbox.live_timer gives you access to a class and functions that make running a live
+    timer that's not only easily to initialize, but easy to query, reset, and pause your timers.
+    This module also contains a class named 'TimerHistory' that keeps a history of all timer actions.
+    
+    To find out more about usage please see:
+    
+    GIT_REPO_ROOT/examples/live_timer
+
+"""
+
+from time import time
+
+from inspyre_toolbox.core_helpers.logging import ROOT_ISL_DEVICE, add_isl_child
+from inspyre_toolbox.live_timer.errors import TimerNotRunningError, TimerNotStartedError
+from inspyre_toolbox.live_timer.history import TimerHistory
+
+LOG_NAME = 'InspyreToolbox.live_timer'
+
+LOG = add_isl_child(LOG_NAME)
+
+#ROOT_ISL_DEVICE.adjust_level('debug')
+
+LOG.debug('Log started!')
+
+
+def format_seconds_to_hhmmss(seconds):
+    """
+    The format_seconds_to_hhmmss function accepts a number of seconds and returns a string
+    representing the amount of time represented by those seconds in HH:MM:SS format.
+
+    Args:
+        seconds (int):
+            The number of seconds to be converted. (Required)
+
+    Returns:
+        A string with the number of hours, minutes and seconds
+    """
+    hours = seconds // (60 * 60)
+    seconds %= (60 * 60)
+    minutes = seconds // 60
+    seconds %= 60
+    return "%02i:%02i:%02i" % (hours, minutes, seconds)
+
+
+class Timer(object):
+    def __repr__(self):
+        statement = "Timer(" \
+                    f"Started: {self.started} |"
+        if self.started:
+            runtime = time() - self.start_time
+            runtime = format_seconds_to_hhmmss(runtime)
+            statement += f" Started: {self.start_time} - Current Runtime: {runtime}"
+
+    def __init__(self, auto_start=False, history=None):
+
+        self.log_name = f'{LOG_NAME}.Timer'
+
+        # Set up logger
+        self.log = add_isl_child(self.log_name)
+
+        # Define some default attribute values
+
+        self.running = False
+        self.mark_2 = None
+        self.pause_end = None
+        self.pause_start = time()
+        self.paused = False
+        self.start_time = None
+        self.started = False
+        self.stopped = False
+        self.total_pause_time = 0
+        self.was_paused = False
+
+        self.log.debug('Set up class attributes.')
+
+        # Start a Timer history object to track times for resets
+        self.history = TimerHistory(self.__get_elapsed) if history is None else history
+
+        self.log.debug('Timer class instantiated!')
+
+    def __get_elapsed(self, ts=None, sans_pause: bool = False, seconds=False):
+        """
+        The __get_elapsed function is a private function that is called by the public functions
+        start(), pause(), and stop(). It returns the elapsed time in seconds, or as a string if
+        seconds=False. The __get_elapsed function does not take any parameters. If you call this
+        private function directly, it will return an error
+
+        Args:
+            self:
+                Access variables that belongs to the class
+
+            ts (int|float):
+                Pass in the current timestamp, (Optional, defaults to time.time())
+
+            sans_pause (bool):
+                Determine whether or not to include the time that the timer was
+                paused in the elapsed time. (Optional; defaults to True)
+
+            seconds (bool):
+                Return the elapsed time as number of seconds. (Optional; defaults
+                to False)
+
+        Returns:
+            The time elapsed since the start of the timer
+        """
+        log = add_isl_child(f'{self.log_name}__get_elapsed')
+
+        diff_time = self.start_time if ts is None else ts
+
+        # ver1.2.7
+        # If we were running but are now stopped, we will skip marking
+        if not self.stopped:
+            self.mark_2 = time()
+
+        diff = self.mark_2 - diff_time
+
+        if sans_pause:
+            return format_seconds_to_hhmmss(diff)
+
+        tpt = 0
+        # print(self.total_pause_time)
+        if self.paused:
+            tpt += time() - self.pause_start
+
+        tpt += self.total_pause_time
+        diff = diff - tpt
+
+        return diff if seconds else format_seconds_to_hhmmss(diff)
+
+    def get_elapsed(self, *args, **kwargs):
+        """
+        The get_elapsed function returns the elapsed time since the timer was started.
+        If the timer is not running, it returns None. If it has been stopped,
+        it returns the elapsed time from start to stop.
+
+        Args:
+            self: Access the attributes and methods of the class in python
+            *args: Pass a non-keyworded, variable-length argument list
+            **kwargs: Pass a keyworded, variable-length argument list
+
+        Returns:
+            The current elapsed time since the timer was started
+
+        """
+        if not self.running and self.stopped or self.running:
+            self.history.add("QUERY")
+            return self.__get_elapsed(*args, **kwargs)
+        else:
+            try:
+                raise TimerNotStartedError(skip_print=True)
+            except TimerNotStartedError as e:
+                print(e.message)
+
+    def reset(self):
+        """
+
+        Reset the 'self.start_time' attribute to this moment, effectively resetting the timer to '00:00:00'
+
+        """
+        self.history.add(action="RESET")
+
+        return Timer(history=self.history)
+
+        # if self.running:
+        #     self.stop()
+        # self.total_pause_time = 0
+        # self.pause_start = None
+        # self.pause_end = None
+        # self.started = False
+
+    def restart(self):
+        """
+        The restart function resets the timer to its original state and starts it
+        running.
+
+        Returns:
+            None
+        """
+        self.reset()
+        if not self.started:
+            self.start()
+
+    def start(self):
+        """
+
+        Store the time the thread was started and assign the attribute 'self.started' to 'True' to indicate this.
+
+        """
+        self.start_time = time()
+        self.started = True
+        self.history.add()
+        self.running = True
+
+    def pause(self):
+        """
+
+        Pause the running timer.
+
+        This function will pause the running timer.
+
+        What this really means in this context is that this function will fill the
+        'self.pause_start' time with the current time. When you unpause at a later
+        time the 'self.unpause' function will reference 'self.pause_start' for
+        comparison.
+
+        Note:
+            This function also sets the 'self.paused' variable to 'True'.
+
+        """
+        if not self.started:
+            raise TimerNotStartedError()
+        if not self.running:
+            raise TimerNotRunningError()
+        if self.paused:
+            return False
+        self.pause_start = time()
+        self.paused = True
+        self.was_paused = True
+        self.history.add("PAUSE")
+
+    def unpause(self):
+        """
+
+        Un-Pause the running timer.
+
+        This function will unpause the running timer. What that really means in this
+        context is that since it marks the time that one paused the timer previously
+        and this will compare the time elapsed between when the pause function
+        was called and when this is called and keeps track of it.
+
+        Whenever get_elapsed is called, it looks at the amount of seconds that
+        have been added by this function's operation process and removes that
+        total from the number of seconds elapsed before passing them to be
+        naturalized.
+
+        Returns:
+            bool:
+                If;
+                    * True:
+                        The timer was successfully un-paused
+                    * False:
+                        The timer was no successfully un-paused (most likely due to its
+                        state not actually being paused),
+        """
+        if not self.started:
+            raise TimerNotStartedError()
+        if not self.running:
+            raise TimerNotRunningError()
+        if self.paused:
+            self.pause_end = time()
+            diff = self.pause_end - self.pause_start
+            self.total_pause_time += diff
+            self.paused = False
+            self.history.add("UNPAUSE")
+            return True
+        else:
+            return False
+
+    def stop(self):
+        """
+        The 'stop' function stops the timer, but leaves it in a paused state.
+        The 'resume' function resumes the timer from where it was stopped.
+
+        Args:
+            self: Reference the object itself
+
+        Returns:
+            The time when the timer is stopped
+        """
+        if not self.started:
+            raise TimerNotStartedError()
+        if self.running:
+            self.running = False
+            self.paused = False
+            self.stopped = True
+            self.mark_2 = time()
+        else:
+            raise TimerNotRunningError()
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/live_timer/errors.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/errors.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-"""
-
-This file contains custom exceptions for Inspyre_Toolbox.live_timer.
-
-"""
-from inspyre_toolbox.core_helpers.debugging import who_rang
-
-
-class TimerNotRunningError(Exception):
-    default_message = 'This timer is not running!'
-
-    def __init__(self, message=default_message, skip_print=False, caller=who_rang()):
-        self.actual_caller = who_rang()
-        self.caller_msg = f'Erroneous call from: {self.actual_caller}'
-
-        if self.actual_caller != caller:
-            self.caller_msg += f' which claims it was called by {caller}'
-
-        msg = f'{self.default_message} {self.caller_msg}'
-
-        if message != self.default_message:
-            msg += f"Further information from caller: {message}"
-
-        self.message = msg
-
-        if not skip_print:
-            print(self.message)
-
-
-class TimerNotStartedError(TimerNotRunningError):
-    default_message = 'Timer has not yet been started!'
-
-    def __init__(self, message=default_message, skip_print=False, caller=who_rang(), **kwargs):
-        super(TimerNotStartedError, self).__init__(kwargs)
+"""
+
+This file contains custom exceptions for Inspyre_Toolbox.live_timer.
+
+"""
+from inspyre_toolbox.core_helpers.debugging import who_rang
+
+
+class TimerNotRunningError(Exception):
+    default_message = 'This timer is not running!'
+
+    def __init__(self, message=default_message, skip_print=False, caller=who_rang()):
+        self.actual_caller = who_rang()
+        self.caller_msg = f'Erroneous call from: {self.actual_caller}'
+
+        if self.actual_caller != caller:
+            self.caller_msg += f' which claims it was called by {caller}'
+
+        msg = f'{self.default_message} {self.caller_msg}'
+
+        if message != self.default_message:
+            msg += f"Further information from caller: {message}"
+
+        self.message = msg
+
+        if not skip_print:
+            print(self.message)
+
+
+class TimerNotStartedError(TimerNotRunningError):
+    default_message = 'Timer has not yet been started!'
+
+    def __init__(self, message=default_message, skip_print=False, caller=who_rang(), **kwargs):
+        super(TimerNotStartedError, self).__init__(kwargs)
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/live_timer/history.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/live_timer/history.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from os import makedirs
-from pathlib import Path
-from time import time
-
-
-class TimerHistory(object):
-
-    def __init__(self, elapsed_method):
-        self.get_elapsed = elapsed_method
-        self.ledger = []
-        self.actions = [
-                "START",
-                "STOP",
-                "PAUSE",
-                "UNPAUSE",
-                "RESET",
-                "CREATE",
-                "QUERY"
-        ]
-        self.add("CREATE")
-
-    def add(self, action: str = "START") -> dict:
-        """
-        The add function adds a new entry to the ledger.
-
-        Args:
-            self:
-                Refer to the object instance
-            action (str):
-                The action you'd like to log to the ledger. (Optional; defaults to 'START')
-
-        Returns:
-            The entry that was just added to the ledger
-
-        """
-        action = action.upper()
-        entry = {
-                "time":               time(),
-                "elapsed_since_last": "",
-                "action":             action,
-                "rt_at_create":       ""
-        }
-        if action == "CREATE":
-            entry['elapsed_since_last'] = 0.00
-        else:
-            entry['elapsed_since_last'] = self.get_elapsed(self.ledger[-1]['time'])
-            entry['rt_at_create'] = self.get_elapsed(self.ledger[0]['time'])
-
-        self.ledger.append(entry)
-
-        return entry
-
-    def write(self):
-        """
-        The write function writes the ledger to a file.
-
-        Args:
-            self:
-                Refer to the object itself
-
-        Returns:
-            None
-        """
-        data_path = Path("~/Inspyre-Softworks/Inspyre-Toolbox/data").expanduser()
-
-        filename = f'ledger_{str(time()).split(".")[0]}'
-        filepath = str(f'{str(data_path)}/{filename}.txt')
-
-        filepath = str(Path(filepath).resolve())
-
-        if not data_path.exists():
-            makedirs(data_path)
-
-        with open(filepath, "w") as fp:
-            fp.write(str(self.ledger))
-
-    def reset(self) -> None:
-        """
-        Clear the ledger
-
-        This literally just runs '.clear()' on 'self.ledger'
-
-        Returns:
-            None
-
-        """
-        self.ledger.clear()
+from os import makedirs
+from pathlib import Path
+from time import time
+
+
+class TimerHistory(object):
+
+    def __init__(self, elapsed_method):
+        self.get_elapsed = elapsed_method
+        self.ledger = []
+        self.actions = [
+                "START",
+                "STOP",
+                "PAUSE",
+                "UNPAUSE",
+                "RESET",
+                "CREATE",
+                "QUERY"
+        ]
+        self.add("CREATE")
+
+    def add(self, action: str = "START") -> dict:
+        """
+        The add function adds a new entry to the ledger.
+
+        Args:
+            self:
+                Refer to the object instance
+            action (str):
+                The action you'd like to log to the ledger. (Optional; defaults to 'START')
+
+        Returns:
+            The entry that was just added to the ledger
+
+        """
+        action = action.upper()
+        entry = {
+                "time":               time(),
+                "elapsed_since_last": "",
+                "action":             action,
+                "rt_at_create":       ""
+        }
+        if action == "CREATE":
+            entry['elapsed_since_last'] = 0.00
+        else:
+            entry['elapsed_since_last'] = self.get_elapsed(self.ledger[-1]['time'])
+            entry['rt_at_create'] = self.get_elapsed(self.ledger[0]['time'])
+
+        self.ledger.append(entry)
+
+        return entry
+
+    def write(self):
+        """
+        The write function writes the ledger to a file.
+
+        Args:
+            self:
+                Refer to the object itself
+
+        Returns:
+            None
+        """
+        data_path = Path("~/Inspyre-Softworks/Inspyre-Toolbox/data").expanduser()
+
+        filename = f'ledger_{str(time()).split(".")[0]}'
+        filepath = str(f'{str(data_path)}/{filename}.txt')
+
+        filepath = str(Path(filepath).resolve())
+
+        if not data_path.exists():
+            makedirs(data_path)
+
+        with open(filepath, "w") as fp:
+            fp.write(str(self.ledger))
+
+    def reset(self) -> None:
+        """
+        Clear the ledger
+
+        This literally just runs '.clear()' on 'self.ledger'
+
+        Returns:
+            None
+
+        """
+        self.ledger.clear()
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/proc_man/__init__.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/proc_man/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,314 +1,314 @@
-#  Copyright (c) 2021. Taylor-Jayde Blackstone <t.blackstone@inspyre.tech> https://inspyre.tech
-import contextlib
-import ctypes
-import os
-from datetime import datetime
-
-import psutil
-from pypattyrn.behavioral.null import Null
-
-import inspyre_toolbox.settings as it_settings
-from inspyre_toolbox.core_helpers.logging import add_isl_child, force_lowkey_log_name, ISL as InspyLogger
-from inspyre_toolbox.humanize import Numerical
-from inspyre_toolbox.proc_man.errors import NoFoundProcessesError
-
-
-fts = datetime.fromtimestamp
-
-ISL = InspyLogger('InspyreToolBox.ProcMan', it_settings.log_level.upper())
-
-LOG = ISL
-
-
-class Colors(object):
-    def __init__(self, return_null=True):
-        """
-        Initializes a Colors object.
-
-        Args:
-            return_null (bool, optional):
-                If True, instantiate the Colors object with Null values for each color attribute.
-
-                If False, instantiate the Colors object with actual color values.Defaults to True.
-        """
-        if return_null:
-            self.red       = Null()
-            self.yellow    = Null()
-            self.blue      = Null()
-            self.green     = Null()
-            self.end_color = Null()
-        else:
-            from inspyred_print import Color, Format
-            color = Color()
-            fmt = Format()
-            self.red       = color.red
-            self.yellow    = color.yellow
-            self.blue      = color.blue
-            self.green     = color.green
-            self.end_color = fmt.end_mod
-
-
-def is_admin() -> bool:
-    """
-    Checks if the current user has administrative privileges.
-
-    Returns:
-        bool:
-            True if the current user has administrative privileges, False otherwise.
-    """
-    try:
-        _is_admin = (os.getuid() == 0)
-    except AttributeError:
-        _is_admin = ctypes.windll.shell32.IsUserAnAdmin() != 0
-    return _is_admin
-
-
-def find_all_by_name(name, case_sensitive=False, inspy_logger_device=None, on_the_dl=False, colorful_logging=False):
-    """
-
-    Find a running program by name.
-
-    Args:
-        name (str):
-            The name of the program you're looking for.
-
-        case_sensitive (bool):
-            Should the function care about letter casing when searching for the given program? (
-            Optional) - Defaults to bool(False)
-
-        inspy_logger_device (inspy_logger.InspyLogger().device):
-            The instantiated device object from the inspy_logger package. (Optional, defaults to None)
-
-            Note:
-                If a value other than NoneType is passed to this parameter, the function will check the
-                InspyLogger.device attribute 'started' to see if the logger has already been started elsewhere. One
-                of three situations could result from this:
-
-                    1) The attribute 'started' exists, and evaluates to bool(False):
-
-                       In this case the function will attempt to start the log-device by calling it's 'start' method
-                       before calling 'add_child' on the log-device in the hopes of receiving it's own logging object.
-
-                    2) The attribute 'started' exists and evaluates to bool(False):
-
-                       In this case the function will attempt to call 'add_child' on the log-device in the hopes of
-                       receiving it's own logging object.
-
-                    3) The attribute 'started' does not exist:
-
-                       In this case, the function will receive a raised AttributeError from the passed object. If
-                       this occurs; the function will raise a more relevant 'InvalidLogDeviceError'
-
-        on_the_dl (bool):
-            Should InspyreToolbox leave itself out of the the logging name? (Optional, Defaults to bool(False))
-
-        colorful_logging (bool):
-            Should the function log colorfully? (Optional, Defaults to bool(False))
-
-
-    Returns:
-        procs_found (list): A list of the currently running processes that match the given name.
-
-    """
-
-    isl_dev = inspy_logger_device
-
-    prefix = '' if on_the_dl else 'InspyreToolbox.'
-    log_name = f'{prefix}proc_man.find_by_name'
-
-    log = add_isl_child(log_name, isl_dev)
-
-    r_null = force_lowkey_log_name or not colorful_logging
-    colors = Colors(return_null=not colorful_logging)
-
-    procs_found = []
-
-    # If we're not being case-sensitive we'll lower the case on 'name'
-    if not case_sensitive:
-        log.debug('Searching in case insensitive mode!')
-        name = name.lower()
-
-    log.debug(f'Search query: {name}')
-
-    # Iterate through the process list
-    for proc in psutil.process_iter():
-        with contextlib.suppress(psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
-            # Gather the information of all the currently running processes
-            proc_info = proc.as_dict(
-                    attrs=['pid', 'name', 'create_time', 'username'])
-            log.debug(proc_info)
-
-            # If we're not caring about case let's go ahead and make both
-            # things we're comparing lowercase.
-            proc_name = proc_info['name'] if case_sensitive else proc_info['name'].lower()
-            if name in proc_name:
-                log.debug(f'{colors.green}Found match: {colors.blue}{proc_info["name"]}'
-                          f'({colors.yellow}{proc_info["pid"]}{colors.blue})')
-
-                # Add find to the list we're returning to the caller.
-                procs_found.append(proc_info)
-
-                log.debug(
-                        f'{colors.green}Added {proc_info["pid"]} to found process list')
-    num_found = Numerical(len(procs_found), noun='process')
-
-    log.debug(f'Found: {colors.yellow}{num_found.count_noun()}')
-
-    # Return found process list to caller
-    return procs_found
-
-
-def kill_all_in_list(kill_list, inspy_logger_device=None, on_the_dl=False, colorful_logging=False):
-    """
-
-    When provided a list of processes, kill each process in the list.
-
-    Args:
-        kill_list:
-            A list of processes in the format of a dictionary
-
-        inspy_logger_device:
-            An instantiated inspy-logger device.
-
-        on_the_dl:
-            Don't include 'InspyreToolbox' in the name of the logger.
-
-        colorful_logging:
-            Should logging be colorful?
-
-    Returns:
-        None
-
-    """
-
-    prefix = '' if on_the_dl else 'InspyreToolbox.'
-    log_name = f'{prefix}ProcMan.kill_all_in_list'
-
-    log = add_isl_child(log_name, ISL.device)
-
-    log.debug('Logging active')
-
-    colors = Colors(return_null=not colorful_logging)
-
-    missing = 0
-
-    for proc in kill_list:
-        log.debug(f'Killing {colors.yellow}{proc["pid"]}')
-        os.kill(proc['pid'], 2)
-        # try:
-        #         subprocess.check_output("Taskkill /PID %d /F" % proc['pid'])
-        #     if os.name == 'nt':
-        #     else:
-        #         os.kill(proc['pid'], 2)
-        # except subprocess.CalledProcessError:
-        #     missing += 1
-        #     if missing >= 20:
-        #         kill_all_by_name(proc['name'])
-        #         break
-        # log.debug(
-        #     f'{colors.green}Kill signal sent to {colors.yellow}{proc["pid"]}')
-
-
-def kill_all_by_name(
-        name,
-        case_sensitive=False,
-        inspy_logger_device=None,
-        on_the_dl=False,
-        colorful_logging=False
-):
-    """
-
-    Kill all currently running programs (and all instances thereof) which have a name containing the string given as a
-    value to the 'name' parameter.
-
-    Note:
-        Unless you are running this as administrator, any programs that you don't have permission to kill will not be
-        killed.
-
-        IF YOU ARE RUNNING AS ADMINISTRATOR EVERY PROCESS THAT MATCHES WILL BE KILLED REGARDLESS OF WHO INSTANTIATED
-        THE PROCESS!!!!
-
-    Args:
-        name (str):
-            The name of the program you'd like to kill all instances of. Whatever
-            you provide here will be used as a query to find all programs that have
-            a name that contains this string.
-
-        case_sensitive (bool):
-            Tell the function that the letter casing is irrelevant to finding matching
-             programs. (Optional, defaults to False)
-
-        inspy_logger_device (inspy_logger.InspyLogger().device):
-            The instantiated device object from the inspy_logger package. (Optional, defaults to None)
-
-            Note:
-                If a value other than NoneType is passed to this parameter, the function will check the
-                InspyLogger.device attribute 'started' to see if the logger has already been started elsewhere. One
-                of three situations could result from this:
-
-                    1) The attribute 'started' exists, and evaluates to bool(False):
-
-                       In this case the function will attempt to start the log-device by calling it's 'start' method
-                       before calling 'add_child' on the log-device in the hopes of receiving it's own logging object.
-
-                    2) The attribute 'started' exists and evaluates to bool(False):
-
-                       In this case the function will attempt to call 'add_child' on the log-device in the hopes of
-                       receiving it's own logging object.
-
-                    3) The attribute 'started' does not exist:
-
-                       In this case, the function will receive a raised AttributeError from the passed object. If
-                       this occurs; the function will raise a more relevant 'InvalidLogDeviceError'
-
-        on_the_dl (bool):
-            Should InspyreToolbox leave itself out of the the logging name? (Optional, Defaults to bool(False))
-
-        colorful_logging (bool):
-            Should the function log colorfully? (Optional, Defaults to bool(False))
-
-    Returns:
-        None
-
-    """
-    from time import sleep
-
-    # Get a logger for logging in logging is enabled.
-    log = add_isl_child('proc_man.kill_all_by_name', inspy_logger_device)
-
-    # Get colors for colorful logging if colorful_logging is bool(True)
-    color = Colors(return_null=not colorful_logging)
-
-    log.debug(f'{color.yellow}Checking to see if there are, any running programs with "'
-              f'{color.green}{name}{color.yellow}" in their name.')
-
-    # Get a list of all the currently running processes that contains 'name' string.
-    procs = find_all_by_name(name, case_sensitive,
-                             inspy_logger_device, on_the_dl, colorful_logging)
-
-    log.debug(procs)
-
-    sleep(5)
-
-    # Get the number of running processes found.
-    num_running = Numerical(len(procs), noun='process')
-
-    log.debug(f'Found {num_running.count_noun()}')
-
-    # Gather the username of the current user.
-    username = os.getlogin()
-
-    # Find out if they are an administrator or not.
-    __is_admin = is_admin()
-
-    started_by_user = []
-
-    if not __is_admin:
-        for proc in procs:
-            log.debug(proc['username'])
-            if proc['username'].endswith(username):
-                started_by_user.append(proc)
-
-    started_by_user.reverse()
-
-    kill_all_in_list(started_by_user)
+#  Copyright (c) 2021. Taylor-Jayde Blackstone <t.blackstone@inspyre.tech> https://inspyre.tech
+import contextlib
+import ctypes
+import os
+from datetime import datetime
+
+import psutil
+from pypattyrn.behavioral.null import Null
+
+import inspyre_toolbox.settings as it_settings
+from inspyre_toolbox.core_helpers.logging import add_isl_child, force_lowkey_log_name, ISL as InspyLogger
+from inspyre_toolbox.humanize import Numerical
+from inspyre_toolbox.proc_man.errors import NoFoundProcessesError
+
+
+fts = datetime.fromtimestamp
+
+ISL = InspyLogger('InspyreToolBox.ProcMan', it_settings.log_level.upper())
+
+LOG = ISL
+
+
+class Colors(object):
+    def __init__(self, return_null=True):
+        """
+        Initializes a Colors object.
+
+        Args:
+            return_null (bool, optional):
+                If True, instantiate the Colors object with Null values for each color attribute.
+
+                If False, instantiate the Colors object with actual color values.Defaults to True.
+        """
+        if return_null:
+            self.red       = Null()
+            self.yellow    = Null()
+            self.blue      = Null()
+            self.green     = Null()
+            self.end_color = Null()
+        else:
+            from inspyred_print import Color, Format
+            color = Color()
+            fmt = Format()
+            self.red       = color.red
+            self.yellow    = color.yellow
+            self.blue      = color.blue
+            self.green     = color.green
+            self.end_color = fmt.end_mod
+
+
+def is_admin() -> bool:
+    """
+    Checks if the current user has administrative privileges.
+
+    Returns:
+        bool:
+            True if the current user has administrative privileges, False otherwise.
+    """
+    try:
+        _is_admin = (os.getuid() == 0)
+    except AttributeError:
+        _is_admin = ctypes.windll.shell32.IsUserAnAdmin() != 0
+    return _is_admin
+
+
+def find_all_by_name(name, case_sensitive=False, inspy_logger_device=None, on_the_dl=False, colorful_logging=False):
+    """
+
+    Find a running program by name.
+
+    Args:
+        name (str):
+            The name of the program you're looking for.
+
+        case_sensitive (bool):
+            Should the function care about letter casing when searching for the given program? (
+            Optional) - Defaults to bool(False)
+
+        inspy_logger_device (inspy_logger.InspyLogger().device):
+            The instantiated device object from the inspy_logger package. (Optional, defaults to None)
+
+            Note:
+                If a value other than NoneType is passed to this parameter, the function will check the
+                InspyLogger.device attribute 'started' to see if the logger has already been started elsewhere. One
+                of three situations could result from this:
+
+                    1) The attribute 'started' exists, and evaluates to bool(False):
+
+                       In this case the function will attempt to start the log-device by calling it's 'start' method
+                       before calling 'add_child' on the log-device in the hopes of receiving it's own logging object.
+
+                    2) The attribute 'started' exists and evaluates to bool(False):
+
+                       In this case the function will attempt to call 'add_child' on the log-device in the hopes of
+                       receiving it's own logging object.
+
+                    3) The attribute 'started' does not exist:
+
+                       In this case, the function will receive a raised AttributeError from the passed object. If
+                       this occurs; the function will raise a more relevant 'InvalidLogDeviceError'
+
+        on_the_dl (bool):
+            Should InspyreToolbox leave itself out of the the logging name? (Optional, Defaults to bool(False))
+
+        colorful_logging (bool):
+            Should the function log colorfully? (Optional, Defaults to bool(False))
+
+
+    Returns:
+        procs_found (list): A list of the currently running processes that match the given name.
+
+    """
+
+    isl_dev = inspy_logger_device
+
+    prefix = '' if on_the_dl else 'InspyreToolbox.'
+    log_name = f'{prefix}proc_man.find_by_name'
+
+    log = add_isl_child(log_name, isl_dev)
+
+    r_null = force_lowkey_log_name or not colorful_logging
+    colors = Colors(return_null=not colorful_logging)
+
+    procs_found = []
+
+    # If we're not being case-sensitive we'll lower the case on 'name'
+    if not case_sensitive:
+        log.debug('Searching in case insensitive mode!')
+        name = name.lower()
+
+    log.debug(f'Search query: {name}')
+
+    # Iterate through the process list
+    for proc in psutil.process_iter():
+        with contextlib.suppress(psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
+            # Gather the information of all the currently running processes
+            proc_info = proc.as_dict(
+                    attrs=['pid', 'name', 'create_time', 'username'])
+            log.debug(proc_info)
+
+            # If we're not caring about case let's go ahead and make both
+            # things we're comparing lowercase.
+            proc_name = proc_info['name'] if case_sensitive else proc_info['name'].lower()
+            if name in proc_name:
+                log.debug(f'{colors.green}Found match: {colors.blue}{proc_info["name"]}'
+                          f'({colors.yellow}{proc_info["pid"]}{colors.blue})')
+
+                # Add find to the list we're returning to the caller.
+                procs_found.append(proc_info)
+
+                log.debug(
+                        f'{colors.green}Added {proc_info["pid"]} to found process list')
+    num_found = Numerical(len(procs_found), noun='process')
+
+    log.debug(f'Found: {colors.yellow}{num_found.count_noun()}')
+
+    # Return found process list to caller
+    return procs_found
+
+
+def kill_all_in_list(kill_list, inspy_logger_device=None, on_the_dl=False, colorful_logging=False):
+    """
+
+    When provided a list of processes, kill each process in the list.
+
+    Args:
+        kill_list:
+            A list of processes in the format of a dictionary
+
+        inspy_logger_device:
+            An instantiated inspy-logger device.
+
+        on_the_dl:
+            Don't include 'InspyreToolbox' in the name of the logger.
+
+        colorful_logging:
+            Should logging be colorful?
+
+    Returns:
+        None
+
+    """
+
+    prefix = '' if on_the_dl else 'InspyreToolbox.'
+    log_name = f'{prefix}ProcMan.kill_all_in_list'
+
+    log = add_isl_child(log_name, ISL.device)
+
+    log.debug('Logging active')
+
+    colors = Colors(return_null=not colorful_logging)
+
+    missing = 0
+
+    for proc in kill_list:
+        log.debug(f'Killing {colors.yellow}{proc["pid"]}')
+        os.kill(proc['pid'], 2)
+        # try:
+        #         subprocess.check_output("Taskkill /PID %d /F" % proc['pid'])
+        #     if os.name == 'nt':
+        #     else:
+        #         os.kill(proc['pid'], 2)
+        # except subprocess.CalledProcessError:
+        #     missing += 1
+        #     if missing >= 20:
+        #         kill_all_by_name(proc['name'])
+        #         break
+        # log.debug(
+        #     f'{colors.green}Kill signal sent to {colors.yellow}{proc["pid"]}')
+
+
+def kill_all_by_name(
+        name,
+        case_sensitive=False,
+        inspy_logger_device=None,
+        on_the_dl=False,
+        colorful_logging=False
+):
+    """
+
+    Kill all currently running programs (and all instances thereof) which have a name containing the string given as a
+    value to the 'name' parameter.
+
+    Note:
+        Unless you are running this as administrator, any programs that you don't have permission to kill will not be
+        killed.
+
+        IF YOU ARE RUNNING AS ADMINISTRATOR EVERY PROCESS THAT MATCHES WILL BE KILLED REGARDLESS OF WHO INSTANTIATED
+        THE PROCESS!!!!
+
+    Args:
+        name (str):
+            The name of the program you'd like to kill all instances of. Whatever
+            you provide here will be used as a query to find all programs that have
+            a name that contains this string.
+
+        case_sensitive (bool):
+            Tell the function that the letter casing is irrelevant to finding matching
+             programs. (Optional, defaults to False)
+
+        inspy_logger_device (inspy_logger.InspyLogger().device):
+            The instantiated device object from the inspy_logger package. (Optional, defaults to None)
+
+            Note:
+                If a value other than NoneType is passed to this parameter, the function will check the
+                InspyLogger.device attribute 'started' to see if the logger has already been started elsewhere. One
+                of three situations could result from this:
+
+                    1) The attribute 'started' exists, and evaluates to bool(False):
+
+                       In this case the function will attempt to start the log-device by calling it's 'start' method
+                       before calling 'add_child' on the log-device in the hopes of receiving it's own logging object.
+
+                    2) The attribute 'started' exists and evaluates to bool(False):
+
+                       In this case the function will attempt to call 'add_child' on the log-device in the hopes of
+                       receiving it's own logging object.
+
+                    3) The attribute 'started' does not exist:
+
+                       In this case, the function will receive a raised AttributeError from the passed object. If
+                       this occurs; the function will raise a more relevant 'InvalidLogDeviceError'
+
+        on_the_dl (bool):
+            Should InspyreToolbox leave itself out of the the logging name? (Optional, Defaults to bool(False))
+
+        colorful_logging (bool):
+            Should the function log colorfully? (Optional, Defaults to bool(False))
+
+    Returns:
+        None
+
+    """
+    from time import sleep
+
+    # Get a logger for logging in logging is enabled.
+    log = add_isl_child('proc_man.kill_all_by_name', inspy_logger_device)
+
+    # Get colors for colorful logging if colorful_logging is bool(True)
+    color = Colors(return_null=not colorful_logging)
+
+    log.debug(f'{color.yellow}Checking to see if there are, any running programs with "'
+              f'{color.green}{name}{color.yellow}" in their name.')
+
+    # Get a list of all the currently running processes that contains 'name' string.
+    procs = find_all_by_name(name, case_sensitive,
+                             inspy_logger_device, on_the_dl, colorful_logging)
+
+    log.debug(procs)
+
+    sleep(5)
+
+    # Get the number of running processes found.
+    num_running = Numerical(len(procs), noun='process')
+
+    log.debug(f'Found {num_running.count_noun()}')
+
+    # Gather the username of the current user.
+    username = os.getlogin()
+
+    # Find out if they are an administrator or not.
+    __is_admin = is_admin()
+
+    started_by_user = []
+
+    if not __is_admin:
+        for proc in procs:
+            log.debug(proc['username'])
+            if proc['username'].endswith(username):
+                started_by_user.append(proc)
+
+    started_by_user.reverse()
+
+    kill_all_in_list(started_by_user)
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/proc_man/errors.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/proc_man/errors.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-#  Copyright (c) 2021. Taylor-Jayde Blackstone <t.blackstone@inspyre.tech> https://inspyre.tech
-"""
-
-This module contains exceptions for 'InspyreToolbox.proc_man'
-
-"""
-
-
-class NoFoundProcessesError(Exception):
-    """
-
-    Raised when 'InspyreToolbox.proc_man.kill_all_by_name' finds no processes that contain the provided string.
-
-    """
-
-    def __init__(self, *args):
-        if args:
-            self.message = args[0]
-        else:
-            self.message = None
-
-    def __str__(self):
-        if self.message:
-            return 'NoFoundProcessesError, {0} '.format(self.message)
-        else:
-            return 'NoFoundProcessesError has been raised!'
+#  Copyright (c) 2021. Taylor-Jayde Blackstone <t.blackstone@inspyre.tech> https://inspyre.tech
+"""
+
+This module contains exceptions for 'InspyreToolbox.proc_man'
+
+"""
+
+
+class NoFoundProcessesError(Exception):
+    """
+
+    Raised when 'InspyreToolbox.proc_man.kill_all_by_name' finds no processes that contain the provided string.
+
+    """
+
+    def __init__(self, *args):
+        if args:
+            self.message = args[0]
+        else:
+            self.message = None
+
+    def __str__(self):
+        if self.message:
+            return 'NoFoundProcessesError, {0} '.format(self.message)
+        else:
+            return 'NoFoundProcessesError has been raised!'
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/pypi/packages.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/pypi/packages.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import subprocess
-import sys
-
-
-def up_to_date(name):
-    latest_version = str(
-        subprocess.run(
-            [sys.executable, '-m', 'pip', 'install', f'{name}==random'],
-            capture_output=True,
-            text=True,
-        )
-    )
-
-    latest_version = latest_version[latest_version.find('(from versions:') + 15:]
-    latest_version = latest_version[:latest_version.find(')')]
-    latest_version = latest_version.replace(' ', '').split(',')[-1]
-
-    current_version = str(
-        subprocess.run(
-            [sys.executable, '-m', 'pip', 'show', f'{name}'],
-            capture_output=True,
-            text=True,
-        )
-    )
-
-    current_version = current_version[current_version.find('Version:') + 8:]
-    current_version = current_version[:current_version.find(
-            '\\n')].replace(' ', '')
-
-    return latest_version == current_version
+import subprocess
+import sys
+
+
+def up_to_date(name):
+    latest_version = str(
+        subprocess.run(
+            [sys.executable, '-m', 'pip', 'install', f'{name}==random'],
+            capture_output=True,
+            text=True,
+        )
+    )
+
+    latest_version = latest_version[latest_version.find('(from versions:') + 15:]
+    latest_version = latest_version[:latest_version.find(')')]
+    latest_version = latest_version.replace(' ', '').split(',')[-1]
+
+    current_version = str(
+        subprocess.run(
+            [sys.executable, '-m', 'pip', 'show', f'{name}'],
+            capture_output=True,
+            text=True,
+        )
+    )
+
+    current_version = current_version[current_version.find('Version:') + 8:]
+    current_version = current_version[:current_version.find(
+            '\\n')].replace(' ', '')
+
+    return latest_version == current_version
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/settings.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/settings.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# ==============================================================================
-#  Copyright (c) Inspyre Softworks 2022.                                       =
-#                                                                              =
-#  Author:                 T. Blackstone                                       =
-#  Author Email:    <t.blackstone@inspyre.tech>                                =
-#  Created:              2/10/22, 9:53 PM                                      =
-# ==============================================================================
-
-log_level = 'info'
+# ==============================================================================
+#  Copyright (c) Inspyre Softworks 2022.                                       =
+#                                                                              =
+#  Author:                 T. Blackstone                                       =
+#  Author Email:    <t.blackstone@inspyre.tech>                                =
+#  Created:              2/10/22, 9:53 PM                                      =
+# ==============================================================================
+
+log_level = 'info'
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/solve_kit/__init__.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/solve_kit/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-Project: Inspyre-Toolbox
-Author: Inspyre Softworks - https://inspyre.tech
-Created: 5/11/2023 @ 8:39 PM
-File:
-  Name: __init__.py
-  Filepath: inspyre_toolbox/solve_kit
-"""
-from statistics import mean
-
-
-def how_many_until(current:list, target=.98, iter_limit=pow(10, 10), delay=0):
-    global iters
-
-    def _process_():
-        global iters
-        cur = list(current)
-        iters = 0
-        while mean(cur) < target and iters < iter_limit:
-            cur.append(1)
-            iters += 1
-        if iters == iter_limit:
-            print('Escaping seemingly infinitely recursive loop')
-        return iters
-
-    try:
-        _process_()
-    except KeyboardInterrupt:
-        iter_limit = iters
-
-
-
-
-
-"""
-The MIT License (MIT)
-Copyright © 2023 Inspyre Softworks - https://inspyre.tech
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
+"""
+Project: Inspyre-Toolbox
+Author: Inspyre Softworks - https://inspyre.tech
+Created: 5/11/2023 @ 8:39 PM
+File:
+  Name: __init__.py
+  Filepath: inspyre_toolbox/solve_kit
+"""
+from statistics import mean
+
+
+def how_many_until(current:list, target=.98, iter_limit=pow(10, 10), delay=0):
+    global iters
+
+    def _process_():
+        global iters
+        cur = list(current)
+        iters = 0
+        while mean(cur) < target and iters < iter_limit:
+            cur.append(1)
+            iters += 1
+        if iters == iter_limit:
+            print('Escaping seemingly infinitely recursive loop')
+        return iters
+
+    try:
+        _process_()
+    except KeyboardInterrupt:
+        iter_limit = iters
+
+
+
+
+
+"""
+The MIT License (MIT)
+Copyright © 2023 Inspyre Softworks - https://inspyre.tech
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/spanners/span_arg_parse.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/spanners/span_arg_parse.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# !/usr/bin/env python
-
-# This file was originally written by jirihnidek (username on GitHub), here are some links
-# regarding the original code:
-#
-# Author's Website:        https://jirihnidek.github.io/
-# Author Gist Page:        https://gist.github.com/jirihnidek
-# Source of Original Code: https://gist.github.com/jirihnidek/3f5d36636198e852280f619847d22d9e
-
-"""Aliases for argparse positional arguments."""
-
-import argparse
-
-
-class SubparserActionAliases(argparse._SubParsersAction):
-    class _AliasedPseudoAction(argparse.Action):
-
-        def __init__(self, name, aliases, help):
-            dest = name
-            if aliases:
-                dest += f" ({','.join(aliases)})"
-            sup = super(SubparserActionAliases._AliasedPseudoAction, self)
-            sup.__init__(option_strings=[], dest=dest, help=help)
-
-    def add_parser(self, name, **kwargs):
-        """
-        The add_parser function adds a parser to the subparsers object.
-        It adds it to the _name_parser_map dictionary, which maps command \
-        name aliases to parsers. It also adds an entry in _choices_actions, which is used by argparse
-        to create help text for each of these commands.
-
-        Args:
-            name:
-                Specify the name of the command
-            **kwargs:
-                Pass a dictionary of keyword arguments to the add_parser function
-
-        Returns:
-            The parser object, which we can then use to add arguments to
-        """
-        if 'aliases' in kwargs:
-            aliases = kwargs['aliases']
-            del kwargs['aliases']
-        else:
-            aliases = []
-
-        parser = super(SubparserActionAliases, self).add_parser(name, **kwargs)
-
-        # Make the aliases work.
-        for alias in aliases:
-            self._name_parser_map[alias] = parser
-        # Make the help text reflect them, first removing old help entry.
-        if 'help' in kwargs:
-            help = kwargs.pop('help')
-            self._choices_actions.pop()
-            pseudo_action = self._AliasedPseudoAction(name, aliases, help)
-            self._choices_actions.append(pseudo_action)
-
-        return parser
+# !/usr/bin/env python
+
+# This file was originally written by jirihnidek (username on GitHub), here are some links
+# regarding the original code:
+#
+# Author's Website:        https://jirihnidek.github.io/
+# Author Gist Page:        https://gist.github.com/jirihnidek
+# Source of Original Code: https://gist.github.com/jirihnidek/3f5d36636198e852280f619847d22d9e
+
+"""Aliases for argparse positional arguments."""
+
+import argparse
+
+
+class SubparserActionAliases(argparse._SubParsersAction):
+    class _AliasedPseudoAction(argparse.Action):
+
+        def __init__(self, name, aliases, help):
+            dest = name
+            if aliases:
+                dest += f" ({','.join(aliases)})"
+            sup = super(SubparserActionAliases._AliasedPseudoAction, self)
+            sup.__init__(option_strings=[], dest=dest, help=help)
+
+    def add_parser(self, name, **kwargs):
+        """
+        The add_parser function adds a parser to the subparsers object.
+        It adds it to the _name_parser_map dictionary, which maps command \
+        name aliases to parsers. It also adds an entry in _choices_actions, which is used by argparse
+        to create help text for each of these commands.
+
+        Args:
+            name:
+                Specify the name of the command
+            **kwargs:
+                Pass a dictionary of keyword arguments to the add_parser function
+
+        Returns:
+            The parser object, which we can then use to add arguments to
+        """
+        if 'aliases' in kwargs:
+            aliases = kwargs['aliases']
+            del kwargs['aliases']
+        else:
+            aliases = []
+
+        parser = super(SubparserActionAliases, self).add_parser(name, **kwargs)
+
+        # Make the aliases work.
+        for alias in aliases:
+            self._name_parser_map[alias] = parser
+        # Make the help text reflect them, first removing old help entry.
+        if 'help' in kwargs:
+            help = kwargs.pop('help')
+            self._choices_actions.pop()
+            pseudo_action = self._AliasedPseudoAction(name, aliases, help)
+            self._choices_actions.append(pseudo_action)
+
+        return parser
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/syntactic_sweets/__init__.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/syntactic_sweets/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-﻿#  Copyright (c) 2021. Taylor-Jayde Blackstone <t.blackstone@inspyre.tech> https://inspyre.tech
-"""
-
-A package containing decorators that are a quick help in programming with Python
-
-"""
-import sys
-from contextlib import contextmanager
-from os import devnull
-
-SUPPRESSED = False
-
-
-@contextmanager
-def suppress_stdout():
-    """
-    The suppress_stdout function is a context manager that redirects stdout to
-    /dev/null.
-
-    This is useful for suppressing output from functions and methods,
-    especially when called in loops.  For example:
-
-        with suppress_stdout():
-            for i in range(10):
-                print(i) # this will not print anything
-
-    Args:
-        ``None``
-    """
-    global SUPPRESSED
-
-    if SUPPRESSED:
-        with open(devnull, "w") as dn:
-            old_stdout = sys.stdout
-            sys.stdout = dn
-            try:
-                yield
-            finally:
-                sys.stdout = old_stdout
-    else:
-        yield
+﻿#  Copyright (c) 2021. Taylor-Jayde Blackstone <t.blackstone@inspyre.tech> https://inspyre.tech
+"""
+
+A package containing decorators that are a quick help in programming with Python
+
+"""
+import sys
+from contextlib import contextmanager
+from os import devnull
+
+SUPPRESSED = False
+
+
+@contextmanager
+def suppress_stdout():
+    """
+    The suppress_stdout function is a context manager that redirects stdout to
+    /dev/null.
+
+    This is useful for suppressing output from functions and methods,
+    especially when called in loops.  For example:
+
+        with suppress_stdout():
+            for i in range(10):
+                print(i) # this will not print anything
+
+    Args:
+        ``None``
+    """
+    global SUPPRESSED
+
+    if SUPPRESSED:
+        with open(devnull, "w") as dn:
+            old_stdout = sys.stdout
+            sys.stdout = dn
+            try:
+                yield
+            finally:
+                sys.stdout = old_stdout
+    else:
+        yield
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/sys_man/__init__.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/sys_man/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-#  Copyright (c) 2021. Taylor-Jayde Blackstone <t.blackstone@inspyre.tech> https://inspyre.tech
-import os
-
-
-def add_to_path(program_path: str):
-    """
-    The add_to_path function adds the program path to the system's PATH variable.
-    This allows for easy access to programs from any terminal window.
-
-    Args:
-        program_path (str):
-            The full path to the directory you'd like to add to your system's PATH
-            environment variable.
-
-    Returns:
-        None
-    """
-    if os.name == "nt":  # Windows systems
-        import winreg  # Allows access to the Windows registry
-        import ctypes  # Allows interface with low-level C APIs
-
-        with winreg.ConnectRegistry(None, winreg.HKEY_CURRENT_USER) as root:  # Get the current user registry
-            with winreg.OpenKey(root, "Environment", 0, winreg.KEY_ALL_ACCESS) as key:  # Go to the environment key
-                existing_path_value = winreg.EnumValue(key, 3)[1]  # Grab the current path value
-
-                # | v |  Takes the current path value and appends the new program
-                # | v |  path
-                new_path_value = existing_path_value + program_path + ";"
-
-                # | v |  Update path variable with update path value | v |
-                winreg.SetValueEx(key, "PATH", 0, winreg.REG_EXPAND_SZ,
-                                  new_path_value)
-
-            # Tell other processes to update their environment
-            HWND_BROADCAST = 0xFFFF
-            WM_SETTINGCHANGE = 0x1A
-            SMTO_ABORTIFHUNG = 0x0002
-            result = ctypes.c_long()
-            SendMessageTimeoutW = ctypes.windll.user32.SendMessageTimeoutW
-            SendMessageTimeoutW(HWND_BROADCAST, WM_SETTINGCHANGE, 0, u"Environment", SMTO_ABORTIFHUNG, 5000,
-                                ctypes.byref(result), )
-    else:  # If system is *nix
-        with open(f"{os.getenv('HOME')}/.bashrc", "a") as bash_file:  # Open bashrc file
-            bash_file.write(f'\nexport PATH="{program_path}:$PATH"\n')  # Add program path to Path variable
-        os.system(f". {os.getenv('HOME')}/.bashrc")  # Update bash source
-    print(f"Added {program_path} to path, please restart shell for changes to take effect")
+#  Copyright (c) 2021. Taylor-Jayde Blackstone <t.blackstone@inspyre.tech> https://inspyre.tech
+import os
+
+
+def add_to_path(program_path: str):
+    """
+    The add_to_path function adds the program path to the system's PATH variable.
+    This allows for easy access to programs from any terminal window.
+
+    Args:
+        program_path (str):
+            The full path to the directory you'd like to add to your system's PATH
+            environment variable.
+
+    Returns:
+        None
+    """
+    if os.name == "nt":  # Windows systems
+        import winreg  # Allows access to the Windows registry
+        import ctypes  # Allows interface with low-level C APIs
+
+        with winreg.ConnectRegistry(None, winreg.HKEY_CURRENT_USER) as root:  # Get the current user registry
+            with winreg.OpenKey(root, "Environment", 0, winreg.KEY_ALL_ACCESS) as key:  # Go to the environment key
+                existing_path_value = winreg.EnumValue(key, 3)[1]  # Grab the current path value
+
+                # | v |  Takes the current path value and appends the new program
+                # | v |  path
+                new_path_value = existing_path_value + program_path + ";"
+
+                # | v |  Update path variable with update path value | v |
+                winreg.SetValueEx(key, "PATH", 0, winreg.REG_EXPAND_SZ,
+                                  new_path_value)
+
+            # Tell other processes to update their environment
+            HWND_BROADCAST = 0xFFFF
+            WM_SETTINGCHANGE = 0x1A
+            SMTO_ABORTIFHUNG = 0x0002
+            result = ctypes.c_long()
+            SendMessageTimeoutW = ctypes.windll.user32.SendMessageTimeoutW
+            SendMessageTimeoutW(HWND_BROADCAST, WM_SETTINGCHANGE, 0, u"Environment", SMTO_ABORTIFHUNG, 5000,
+                                ctypes.byref(result), )
+    else:  # If system is *nix
+        with open(f"{os.getenv('HOME')}/.bashrc", "a") as bash_file:  # Open bashrc file
+            bash_file.write(f'\nexport PATH="{program_path}:$PATH"\n')  # Add program path to Path variable
+        os.system(f". {os.getenv('HOME')}/.bashrc")  # Update bash source
+    print(f"Added {program_path} to path, please restart shell for changes to take effect")
```

### Comparing `inspyre_toolbox-1.4.0/inspyre_toolbox/version.py` & `inspyre_toolbox-1.4.1/inspyre_toolbox/version.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-from inspyre_toolbox.common.meta import VERSION as _VERSION, URLS as _URLS, RELEASE_MAP
-import requests
-from packaging import version as pkg_version
-import sys
-from rich.table import Table
-from rich import print
-
-
-def get_full_version_name():
-    """
-    Gets the full version name.
-
-    Returns:
-        str: The full version name.
-
-    Since:
-        v1.3.2
-    """
-    ver = parse_version()
-    ver = ver.split('-')[0]
-
-    release_type = RELEASE_MAP[_VERSION["release"]]
-    release_num = _VERSION["release_num"]
-    release_str = f" {release_type} {'' if _VERSION['release'].lower() == 'final' else f'({release_num})'}"
-    return f'v{ver}{release_str}'
-
-
-def parse_version() -> str:
-    """
-    Parses the version information into a string.
-
-    Returns:
-        str: The version information.
-
-    Since:
-        v1.3.2
-    """
-    version = f'{_VERSION["major"]}.{_VERSION["minor"]}.{_VERSION["patch"]}'
-
-    if _VERSION['release'] != 'final':
-        version += f'-{_VERSION["release"]}.{_VERSION["release_num"]}'
-
-    return version
-
-
-class PyPiVersionInfo:
-    """
-    A class to represent the version information for this package from PyPi.
-
-    Attributes:
-        latest_stable (packaging.version.Version):
-            The latest stable version of the package on PyPi.
-
-        latest_pre_release (packaging.version.Version):
-            The latest pre-release version of the package.
-    Since:
-        v1.3.1
-    """
-    __all_versions: (list[str], None)
-    __url = f'{_URLS["pypi_url"]}/json'
-    __installed = parse_version()
-    __checked_for_update = False
-    __newer_available_version = None
-
-    def __init__(self, include_pre_release_for_update_check=False):
-        self.__latest_stable = None
-        self.__latest_pre_release = None
-        self.__all_versions = None
-        self.include_pre_release_for_update_check = include_pre_release_for_update_check
-        self.__query_versions()
-
-    @property
-    def all_versions(self):
-        if self.__all_versions is None:
-            self.__query_versions()
-        return sorted([pkg_version.parse(v) for v in self.__all_versions])
-
-    @property
-    def checked_for_update(self):
-        return self.__checked_for_update
-
-    @property
-    def installed(self):
-        """
-        Gets the installed version of the package.
-        """
-        return pkg_version.parse(self.__installed)
-
-    @property
-    def installed_newer_than_latest(self):
-        return self.installed > self.latest
-
-    @property
-    def latest(self):
-        return (
-            self.all_versions[-1]
-            if self.include_pre_release_for_update_check
-            else self.latest_stable
-        )
-
-    @property
-    def latest_stable(self):
-        """
-        Gets the latest stable version of the package on PyPi.
-        """
-        if self.__latest_stable is None:
-            self.__query_versions()
-        return pkg_version.parse(self.__latest_stable)
-
-    @property
-    def latest_pre_release(self):
-        """
-        Gets the latest pre-release version of the package.
-        """
-        if self.__all_versions is None:
-            self.__query_versions()
-        pre_release_versions = [v for v in self.all_versions if v.is_prerelease]
-        return pre_release_versions[-1] if pre_release_versions else None
-
-    @property
-    def newer_available_version(self):
-
-        if self.__newer_available_version is None:
-            self.check_for_update()
-
-        return self.__newer_available_version
-
-    def __query_versions(self):
-        """
-        Queries the versions from PyPi.
-        """
-        try:
-            response = requests.get(self.__url)
-            response.raise_for_status()
-            data = response.json()
-
-            self.__all_versions = list(data['releases'].keys())
-            self.__latest_stable = data['info']['version']
-        except requests.RequestException as e:
-            # Handle connection errors, HTTP errors, etc.
-            print(f"Error querying PyPi: {e}")
-
-    @property
-    def update_available(self):
-        """
-        Checks if an update is available.
-        """
-        if self.__newer_available_version is None:
-            self.check_for_update()
-        return self.__newer_available_version is not None
-
-    def check_for_update(self, include_pre_releases=False):
-        latest_version = self.latest_stable
-
-        if include_pre_releases or self.include_pre_release_for_update_check:
-            latest_version = max(latest_version, self.latest_pre_release)
-
-        if latest_version > self.installed:
-            self.__newer_available_version = latest_version
-
-        self.__checked_for_update = True
-
-        return latest_version > self.installed
-
-    def update(self):
-        """
-        Checks for updates to inspy-logger.
-
-        Returns:
-            None`
-
-        Since:
-            v1.3.2
-        """
-
-        local_newer_statement = 'Local version is newer than latest version. This is likely a development build.'
-
-        if not self.installed_newer_than_latest:
-            local_newer_statement = ''
-
-        try:
-            if self.update_available:
-                print(f'\n\n[bold green]Update Available![/bold green] New version: '
-                      f'[bold cyan]{self.update_available}[/bold cyan]')
-            else:
-                print(f'\n\n[bold green]No update available.[/bold green] Current version: '
-                      f'[bold cyan]{parse_version()}[/bold cyan] {local_newer_statement}')
-
-        except Exception as e:
-            print(f'An error occurred during the update check: {str(e)}')
-
-    def print_version_info(self):
-        """
-        Print version information in a formatted table.
-
-        This function creates a table using the `Table` class and populates it with version information about the current Python environment. It then prints the table to the console.
-
-        Parameters:
-            self: The current instance of the class.
-
-        Returns:
-            None
-        """
-
-        # Create a table
-
-        table = Table(show_header=False, show_lines=True, expand=True, border_style='bright_blue',
-                      row_styles=['none', 'dim'])
-
-        # Add columns
-        table.add_column('Property', style='cyan', width=20)
-        table.add_column('Value', justify='center')
-
-        # Add rows
-        table.add_row('Version', parse_version(), )
-        table.add_row('Full Version Name', get_full_version_name())
-
-        if self.update_available:
-            table.add_row('Update Available', '[bold green]Yes[/bold green]')
-            table.add_row('Latest Version', f'{self.new_version_available_num}')
-
-        table.add_row('Python Executable Path', sys.executable)
-        table.add_row('Python Version', sys.version)
-
-        print(table)
+from inspyre_toolbox.common.meta import VERSION as _VERSION, URLS as _URLS, RELEASE_MAP
+import requests
+from packaging import version as pkg_version
+import sys
+from rich.table import Table
+from rich import print
+
+
+def get_full_version_name():
+    """
+    Gets the full version name.
+
+    Returns:
+        str: The full version name.
+
+    Since:
+        v1.3.2
+    """
+    ver = parse_version()
+    ver = ver.split('-')[0]
+
+    release_type = RELEASE_MAP[_VERSION["release"]]
+    release_num = _VERSION["release_num"]
+    release_str = f" {release_type} {'' if _VERSION['release'].lower() == 'final' else f'({release_num})'}"
+    return f'v{ver}{release_str}'
+
+
+def parse_version() -> str:
+    """
+    Parses the version information into a string.
+
+    Returns:
+        str: The version information.
+
+    Since:
+        v1.3.2
+    """
+    version = f'{_VERSION["major"]}.{_VERSION["minor"]}.{_VERSION["patch"]}'
+
+    if _VERSION['release'] != 'final':
+        version += f'-{_VERSION["release"]}.{_VERSION["release_num"]}'
+
+    return version
+
+
+class PyPiVersionInfo:
+    """
+    A class to represent the version information for this package from PyPi.
+
+    Attributes:
+        latest_stable (packaging.version.Version):
+            The latest stable version of the package on PyPi.
+
+        latest_pre_release (packaging.version.Version):
+            The latest pre-release version of the package.
+    Since:
+        v1.3.1
+    """
+    __all_versions: (list[str], None)
+    __url = f'{_URLS["pypi_url"]}/json'
+    __installed = parse_version()
+    __checked_for_update = False
+    __newer_available_version = None
+
+    def __init__(self, include_pre_release_for_update_check=False):
+        self.__latest_stable = None
+        self.__latest_pre_release = None
+        self.__all_versions = None
+        self.include_pre_release_for_update_check = include_pre_release_for_update_check
+        self.__query_versions()
+
+    @property
+    def all_versions(self):
+        if self.__all_versions is None:
+            self.__query_versions()
+        return sorted([pkg_version.parse(v) for v in self.__all_versions])
+
+    @property
+    def checked_for_update(self):
+        return self.__checked_for_update
+
+    @property
+    def installed(self):
+        """
+        Gets the installed version of the package.
+        """
+        return pkg_version.parse(self.__installed)
+
+    @property
+    def installed_newer_than_latest(self):
+        return self.installed > self.latest
+
+    @property
+    def latest(self):
+        return (
+            self.all_versions[-1]
+            if self.include_pre_release_for_update_check
+            else self.latest_stable
+        )
+
+    @property
+    def latest_stable(self):
+        """
+        Gets the latest stable version of the package on PyPi.
+        """
+        if self.__latest_stable is None:
+            self.__query_versions()
+        return pkg_version.parse(self.__latest_stable)
+
+    @property
+    def latest_pre_release(self):
+        """
+        Gets the latest pre-release version of the package.
+        """
+        if self.__all_versions is None:
+            self.__query_versions()
+        pre_release_versions = [v for v in self.all_versions if v.is_prerelease]
+        return pre_release_versions[-1] if pre_release_versions else None
+
+    @property
+    def newer_available_version(self):
+
+        if self.__newer_available_version is None:
+            self.check_for_update()
+
+        return self.__newer_available_version
+
+    def __query_versions(self):
+        """
+        Queries the versions from PyPi.
+        """
+        try:
+            response = requests.get(self.__url)
+            response.raise_for_status()
+            data = response.json()
+
+            self.__all_versions = list(data['releases'].keys())
+            self.__latest_stable = data['info']['version']
+        except requests.RequestException as e:
+            # Handle connection errors, HTTP errors, etc.
+            print(f"Error querying PyPi: {e}")
+
+    @property
+    def update_available(self):
+        """
+        Checks if an update is available.
+        """
+        if self.__newer_available_version is None:
+            self.check_for_update()
+        return self.__newer_available_version is not None
+
+    def check_for_update(self, include_pre_releases=False):
+        latest_version = self.latest_stable
+
+        if include_pre_releases or self.include_pre_release_for_update_check:
+            latest_version = max(latest_version, self.latest_pre_release)
+
+        if latest_version > self.installed:
+            self.__newer_available_version = latest_version
+
+        self.__checked_for_update = True
+
+        return latest_version > self.installed
+
+    def update(self):
+        """
+        Checks for updates to inspy-logger.
+
+        Returns:
+            None`
+
+        Since:
+            v1.3.2
+        """
+
+        local_newer_statement = 'Local version is newer than latest version. This is likely a development build.'
+
+        if not self.installed_newer_than_latest:
+            local_newer_statement = ''
+
+        try:
+            if self.update_available:
+                print(f'\n\n[bold green]Update Available![/bold green] New version: '
+                      f'[bold cyan]{self.update_available}[/bold cyan]')
+            else:
+                print(f'\n\n[bold green]No update available.[/bold green] Current version: '
+                      f'[bold cyan]{parse_version()}[/bold cyan] {local_newer_statement}')
+
+        except Exception as e:
+            print(f'An error occurred during the update check: {str(e)}')
+
+    def print_version_info(self):
+        """
+        Print version information in a formatted table.
+
+        This function creates a table using the `Table` class and populates it with version information about the current Python environment. It then prints the table to the console.
+
+        Parameters:
+            self: The current instance of the class.
+
+        Returns:
+            None
+        """
+
+        # Create a table
+
+        table = Table(show_header=False, show_lines=True, expand=True, border_style='bright_blue',
+                      row_styles=['none', 'dim'])
+
+        # Add columns
+        table.add_column('Property', style='cyan', width=20)
+        table.add_column('Value', justify='center')
+
+        # Add rows
+        table.add_row('Version', parse_version(), )
+        table.add_row('Full Version Name', get_full_version_name())
+
+        if self.update_available:
+            table.add_row('Update Available', '[bold green]Yes[/bold green]')
+            table.add_row('Latest Version', f'{self.new_version_available_num}')
+
+        table.add_row('Python Executable Path', sys.executable)
+        table.add_row('Python Version', sys.version)
+
+        print(table)
```

### Comparing `inspyre_toolbox-1.4.0/pyproject.toml` & `inspyre_toolbox-1.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-[build-system]
-requires = [ "poetry-core>=1.0.0",]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry]
-name = "inspyre-toolbox"
-version = "v1.4.0"
-description = "A toolbox containing some useful tools for Inspyre Softworks packages. Generally useful to some programmers too."
-authors = [ "T Blackstone <t.blackstone@inspyre.tech>",]
-license = "MIT"
-classifiers = [ "Intended Audience :: Developers", "License :: OSI Approved :: MIT License", "Natural Language :: English", "Operating System :: OS Independent", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.6", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3 :: Only", "Topic :: Scientific/Engineering :: Mathematics", "Topic :: Software Development", "Topic :: Software Development :: Build Tools", "Topic :: Software Development :: Libraries :: Python Modules", "Topic :: Terminals", "Topic :: Utilities",]
-keywords = [ "toolbox", "timer", "commify", "strings", "elapsed",]
-
-[tool.poetry.dependencies]
-python = ">=3.10,<4.0"
-inflect = "^5.3.0"
-psutil = "^5.8.0"
-DateTime = "^4.3"
-pypattyrn = "^1.2"
-tqdm = "^4.64.0"
-inspyred-print = "^1.2.1"
-inspy-logger = "3.0.2.dev1"
-
-[tool.poetry.scripts]
-ist-bytes-converter = "inspyre_toolbox.cli.ist_bytes_converter:main"
-
-[tool.poetry.group.dev.dependencies]
-ptipython = "^1.0.1"
-prompt-toolkit = "^3.0.43"
-ipython = "^8.21.0"
-Sphinx = "^5.0.2"
-sphinx-rtd-theme = "1.0.0"
-sphinxcontrib-fulltoc = "^1.2.0"
-jedi = "^0.18.0"
-parso = "^0.8.2"
-releases = "^1.6.3"
-ipykernel = "^6.29.2"
+[build-system]
+requires = [ "poetry-core>=1.0.0",]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry]
+name = "inspyre-toolbox"
+version = "v1.4.1"
+description = "A toolbox containing some useful tools for Inspyre Softworks packages. Generally useful to some programmers too."
+authors = [ "T Blackstone <t.blackstone@inspyre.tech>",]
+license = "MIT"
+classifiers = [ "Intended Audience :: Developers", "License :: OSI Approved :: MIT License", "Natural Language :: English", "Operating System :: OS Independent", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.6", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3 :: Only", "Topic :: Scientific/Engineering :: Mathematics", "Topic :: Software Development", "Topic :: Software Development :: Build Tools", "Topic :: Software Development :: Libraries :: Python Modules", "Topic :: Terminals", "Topic :: Utilities",]
+keywords = [ "toolbox", "timer", "commify", "strings", "elapsed",]
+
+[tool.poetry.dependencies]
+python = ">=3.9,<4.0"
+inflect = "^5.3.0"
+psutil = "^5.8.0"
+DateTime = "^4.3"
+pypattyrn = "^1.2"
+tqdm = "^4.64.0"
+inspyred-print = "^1.2.1"
+inspy-logger = "3.0.2.dev1"
+
+[tool.poetry.scripts]
+ist-bytes-converter = "inspyre_toolbox.cli.ist_bytes_converter:main"
+
+[tool.poetry.group.dev.dependencies]
+ptipython = "^1.0.1"
+prompt-toolkit = "^3.0.43"
+Sphinx = "^5.0.2"
+sphinx-rtd-theme = "1.0.0"
+sphinxcontrib-fulltoc = "^1.2.0"
+jedi = "^0.18.0"
+parso = "^0.8.2"
+releases = "^1.6.3"
+ipykernel = "^6.29.2"
```

### Comparing `inspyre_toolbox-1.4.0/PKG-INFO` & `inspyre_toolbox-1.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: inspyre-toolbox
-Version: 1.4.0
+Version: 1.4.1
 Summary: A toolbox containing some useful tools for Inspyre Softworks packages. Generally useful to some programmers too.
 License: MIT
 Keywords: toolbox,timer,commify,strings,elapsed
 Author: T Blackstone
 Author-email: t.blackstone@inspyre.tech
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Dist: DateTime (>=4.3,<5.0)
```

