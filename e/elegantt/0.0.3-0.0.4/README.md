# Comparing `tmp/elegantt-0.0.3.tar.gz` & `tmp/elegantt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elegantt-0.0.3.tar", last modified: Sun Apr 28 14:36:40 2024, max compression
+gzip compressed data, was "elegantt-0.0.4.tar", last modified: Tue Apr 30 13:21:10 2024, max compression
```

## Comparing `elegantt-0.0.3.tar` & `elegantt-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2024-04-28 14:36:40.653662 elegantt-0.0.3/
--rw-rw-r--   0 palau     (1000) palau     (1000)     1065 2023-02-23 05:08:13.000000 elegantt-0.0.3/LICENSE
--rw-rw-r--   0 palau     (1000) palau     (1000)       68 2023-02-25 08:35:15.000000 elegantt-0.0.3/MANIFEST.in
--rw-rw-r--   0 palau     (1000) palau     (1000)     1653 2024-04-28 14:36:40.653662 elegantt-0.0.3/PKG-INFO
--rw-rw-r--   0 palau     (1000) palau     (1000)      801 2023-02-25 13:31:13.000000 elegantt-0.0.3/README.md
-drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2024-04-28 14:36:40.645662 elegantt-0.0.3/elegantt/
--rw-rw-r--   0 palau     (1000) palau     (1000)       91 2023-02-25 13:16:30.000000 elegantt-0.0.3/elegantt/__init__.py
--rw-rw-r--   0 palau     (1000) palau     (1000)      692 2023-02-25 13:50:25.000000 elegantt-0.0.3/elegantt/command.py
--rw-rw-r--   0 palau     (1000) palau     (1000)     7388 2024-04-28 13:53:18.000000 elegantt-0.0.3/elegantt/elegantt.py
-drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2024-04-28 14:36:40.644662 elegantt-0.0.3/elegantt/tests/
-drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2024-04-28 14:36:40.645662 elegantt-0.0.3/elegantt/tests/ipaexg/
--rw-rw-r--   0 palau     (1000) palau     (1000)    20564 2023-02-23 02:32:09.000000 elegantt-0.0.3/elegantt/tests/ipaexg/IPA_Font_License_Agreement_v1.0.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)     1710 2023-02-23 02:32:14.000000 elegantt-0.0.3/elegantt/tests/ipaexg/Readme_ipaexg00401.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)  6099900 2023-02-23 02:32:13.000000 elegantt-0.0.3/elegantt/tests/ipaexg/ipaexg.ttf
--rw-rw-r--   0 palau     (1000) palau     (1000)      701 2023-02-25 12:47:33.000000 elegantt-0.0.3/elegantt/utils.py
-drwxrwxr-x   0 palau     (1000) palau     (1000)        0 2024-04-28 14:36:40.645662 elegantt-0.0.3/elegantt.egg-info/
--rw-rw-r--   0 palau     (1000) palau     (1000)     1653 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/PKG-INFO
--rw-rw-r--   0 palau     (1000) palau     (1000)      448 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/SOURCES.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)        1 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/dependency_links.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)       70 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/entry_points.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)       14 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/requires.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)        9 2024-04-28 14:36:40.000000 elegantt-0.0.3/elegantt.egg-info/top_level.txt
--rw-rw-r--   0 palau     (1000) palau     (1000)       38 2024-04-28 14:36:40.653662 elegantt-0.0.3/setup.cfg
--rw-rw-r--   0 palau     (1000) palau     (1000)      798 2024-04-28 14:31:28.000000 elegantt-0.0.3/setup.py
+drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-04-30 13:21:10.844846 elegantt-0.0.4/
+-rw-r--r--   0 uehara    (1000) uehara    (1000)     1065 2024-04-29 11:20:20.000000 elegantt-0.0.4/LICENSE
+-rw-r--r--   0 uehara    (1000) uehara    (1000)       68 2024-04-29 11:20:20.000000 elegantt-0.0.4/MANIFEST.in
+-rw-r--r--   0 uehara    (1000) uehara    (1000)     1653 2024-04-30 13:21:10.844846 elegantt-0.0.4/PKG-INFO
+-rw-r--r--   0 uehara    (1000) uehara    (1000)      801 2024-04-29 11:20:20.000000 elegantt-0.0.4/README.md
+drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-04-30 13:21:10.564845 elegantt-0.0.4/elegantt/
+-rw-r--r--   0 uehara    (1000) uehara    (1000)       91 2024-04-29 11:20:20.000000 elegantt-0.0.4/elegantt/__init__.py
+-rw-r--r--   0 uehara    (1000) uehara    (1000)      692 2024-04-29 11:20:20.000000 elegantt-0.0.4/elegantt/command.py
+-rw-r--r--   0 uehara    (1000) uehara    (1000)     7525 2024-04-30 12:56:32.000000 elegantt-0.0.4/elegantt/elegantt.py
+drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-04-30 13:21:10.524845 elegantt-0.0.4/elegantt/tests/
+drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-04-30 13:21:10.584845 elegantt-0.0.4/elegantt/tests/ipaexg/
+-rw-r--r--   0 uehara    (1000) uehara    (1000)    20564 2024-04-29 11:20:20.000000 elegantt-0.0.4/elegantt/tests/ipaexg/IPA_Font_License_Agreement_v1.0.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)     1710 2024-04-29 11:20:20.000000 elegantt-0.0.4/elegantt/tests/ipaexg/Readme_ipaexg00401.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)  6099900 2024-04-29 11:20:20.000000 elegantt-0.0.4/elegantt/tests/ipaexg/ipaexg.ttf
+-rw-r--r--   0 uehara    (1000) uehara    (1000)      762 2024-04-30 13:17:52.000000 elegantt-0.0.4/elegantt/utils.py
+drwxr-xr-x   0 uehara    (1000) uehara    (1000)        0 2024-04-30 13:21:10.564845 elegantt-0.0.4/elegantt.egg-info/
+-rw-r--r--   0 uehara    (1000) uehara    (1000)     1653 2024-04-30 13:21:09.000000 elegantt-0.0.4/elegantt.egg-info/PKG-INFO
+-rw-r--r--   0 uehara    (1000) uehara    (1000)      448 2024-04-30 13:21:10.000000 elegantt-0.0.4/elegantt.egg-info/SOURCES.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)        1 2024-04-30 13:21:09.000000 elegantt-0.0.4/elegantt.egg-info/dependency_links.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)       70 2024-04-30 13:21:09.000000 elegantt-0.0.4/elegantt.egg-info/entry_points.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)       14 2024-04-30 13:21:09.000000 elegantt-0.0.4/elegantt.egg-info/requires.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)        9 2024-04-30 13:21:09.000000 elegantt-0.0.4/elegantt.egg-info/top_level.txt
+-rw-r--r--   0 uehara    (1000) uehara    (1000)       38 2024-04-30 13:21:10.844846 elegantt-0.0.4/setup.cfg
+-rw-r--r--   0 uehara    (1000) uehara    (1000)      798 2024-04-30 08:16:51.000000 elegantt-0.0.4/setup.py
```

### Comparing `elegantt-0.0.3/LICENSE` & `elegantt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.3/PKG-INFO` & `elegantt-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elegantt
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a gantt chart drawing library
 Home-page: http://github.com/usop4/elegantt
 Author: Takayuki Uehara
 Author-email: t.uehara@gmail.com
 License: UNKNOWN
 Description: # elegantt
```

### Comparing `elegantt-0.0.3/README.md` & `elegantt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.3/elegantt/command.py` & `elegantt-0.0.4/elegantt/command.py`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.3/elegantt/elegantt.py` & `elegantt-0.0.4/elegantt/elegantt.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     cell_width = 32
     date_position = 20
     week_position = 40
     box_position = 60
     box_margin = 5
     box_height = 40
     font_size = 12
-    bar_color = (128,128,128)
+    bar_color = (184,184,191)
     font_color = (0,0,0)
     line_color = (0,0,0)
-    holiday_color = (220,220,220)
+    holiday_color = (242,242,244)
     max_day = 14
  
     def __init__(self,size=(512,256),color=(255,255,255),today=False):
         self.im = Image.new("RGB",size,color) #(512, 256), (255, 255, 255)
         self.draw = ImageDraw.Draw(self.im)
 
         self.im_width = size[0]
@@ -45,37 +45,42 @@
         self.monday = self.today - datetime.timedelta(days=self.today.weekday())
 
         self.calendar_height = size[1] - self.top_margin - self.bottom_margin
 
         self.font_regular = elegantt.utils.detectfont()
         self.font_bold = elegantt.utils.detectfont()
 
+    def get_today(self):
+        return self.today
 
     def set_font(self,regular,bold=False):
         self.font_regular = regular
         if bold:
             self.font_bold = bold
         else:
             self.font_bold = regular
 
+    def get_font(self):
+        return self.font_regular
+
     def get_monday(self):
         return self.monday
 
     def set_box_position(self,box_position):
         self.box_position = box_position
 
     def set_max_day(self,max_day):
         self.max_day = max_day
 
     def set_bar_height(self,height):
         self.box_height = height
 
     def set_bar_width(self,width):
         self.cell_width = width
-    
+
     def set_bar_color(self,color):
         self.bar_color = color
 
     def set_line_color(self,color):
         self.line_color = color
 
     def set_holiday_color(self,color):
@@ -191,24 +196,24 @@
             if d == self.today:
                 font = ImageFont.truetype(self.font_bold, self.font_size)
             else:
                 font = ImageFont.truetype(self.font_regular, self.font_size)
 
             self.draw.multiline_text(
                 (
-                    self.left_margin + i*self.cell_width + self.cell_width/2 - self.font_size/2,
+                    self.left_margin + i*self.cell_width + self.cell_width/2 - self.font_size/2,#日付は2文字
                     self.date_position
                 ),
                 d.strftime('%d'),
                 fill=self.font_color, 
                 font=font
             )
             self.draw.multiline_text(
                 (
-                    self.left_margin + i*self.cell_width + self.cell_width/2 - self.font_size/2,
+                    self.left_margin + i*self.cell_width + self.cell_width/2 - self.font_size,#曜日は3文字
                     self.week_position
                 ),
                 week_str[i%7],
                 fill=self.font_color, 
                 font=font
             )
```

### Comparing `elegantt-0.0.3/elegantt/tests/ipaexg/IPA_Font_License_Agreement_v1.0.txt` & `elegantt-0.0.4/elegantt/tests/ipaexg/IPA_Font_License_Agreement_v1.0.txt`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.3/elegantt/tests/ipaexg/Readme_ipaexg00401.txt` & `elegantt-0.0.4/elegantt/tests/ipaexg/Readme_ipaexg00401.txt`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.3/elegantt/tests/ipaexg/ipaexg.ttf` & `elegantt-0.0.4/elegantt/tests/ipaexg/ipaexg.ttf`

 * *Files identical despite different names*

### Comparing `elegantt-0.0.3/elegantt/utils.py` & `elegantt-0.0.4/elegantt/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import os
 
 def detectfont():
     import glob
     fontdirs = [
+        '/usr/share/fonts/opentype/noto',
         '/usr/share/fonts',
         '/Library/Fonts',
         '/System/Library/Fonts',
         'c:/windows/fonts',
         '/usr/local/share/font-*',
     ]
     fontfiles = [
+        'NotoSansCJK-Regular.ttc',
         'ipaexg.ttf',
         'DejaVuSans.ttf',
-        'NotoSansCJK-Regular.ttc',
     ]
 
     fontpath = None
     globber = (glob.glob(d) for d in fontdirs)
     for fontdir in sum(globber, []):
         for root, _, files in os.walk(fontdir):
             for font in fontfiles:
                 if font in files:
                     fontpath = os.path.join(root, font)
                     break
-
     return fontpath
 
-
 if __name__ == '__main__':
-    print("utils.py")
+    print("utils.py is part of elegantt.")
```

### Comparing `elegantt-0.0.3/elegantt.egg-info/PKG-INFO` & `elegantt-0.0.4/elegantt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elegantt
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a gantt chart drawing library
 Home-page: http://github.com/usop4/elegantt
 Author: Takayuki Uehara
 Author-email: t.uehara@gmail.com
 License: UNKNOWN
 Description: # elegantt
```

### Comparing `elegantt-0.0.3/setup.py` & `elegantt-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='elegantt',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
 
     author='Takayuki Uehara',
     author_email='t.uehara@gmail.com',
 
     url='http://github.com/usop4/elegantt',
```

