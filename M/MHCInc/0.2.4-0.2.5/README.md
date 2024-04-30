# Comparing `tmp/MHCInc-0.2.4.tar.gz` & `tmp/mhcinc-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MHCInc-0.2.4.tar", last modified: Tue Apr 11 21:59:27 2023, max compression
+gzip compressed data, was "mhcinc-0.2.5.tar", last modified: Tue Apr 30 15:19:32 2024, max compression
```

## Comparing `MHCInc-0.2.4.tar` & `mhcinc-0.2.5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2023-04-11 21:59:27.770766 MHCInc-0.2.4/
--rw-r--r--   0 mhcteam    (501) staff       (20)     1073 2022-07-24 07:55:00.000000 MHCInc-0.2.4/LICENSE.txt
-drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2023-04-11 21:59:27.766049 MHCInc-0.2.4/MHCInc/
-drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2023-04-11 21:59:27.769962 MHCInc-0.2.4/MHCInc/MHCInc/
--rw-r--r--   0 mhcteam    (501) staff       (20)     5891 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/GuessGame.py
--rw-r--r--   0 mhcteam    (501) staff       (20)    15461 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/GuessGameEasy.py
--rw-r--r--   0 mhcteam    (501) staff       (20)    11622 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/GuessGameSecondary.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1211 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/MITLicense.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     3734 2022-11-26 10:54:40.000000 MHCInc-0.2.4/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py
--rw-r--r--   0 mhcteam    (501) staff       (20)      808 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/Python3学习示例.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     6222 2023-04-11 21:56:32.000000 MHCInc-0.2.4/MHCInc/MHCInc/__init__.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1028 2022-09-24 03:12:38.000000 MHCInc-0.2.4/MHCInc/MHCInc/animal_guess.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     4058 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/caterpillar.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     2891 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/caterpillar2.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1148 2022-11-13 00:34:45.000000 MHCInc-0.2.4/MHCInc/MHCInc/copyright.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     3274 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/egg_catcher.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     3578 2022-11-26 10:54:22.000000 MHCInc-0.2.4/MHCInc/MHCInc/egg_catcher_perfect.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1936 2022-11-26 10:54:32.000000 MHCInc-0.2.4/MHCInc/MHCInc/matchmaker.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     2917 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/random.py
--rw-r--r--   0 mhcteam    (501) staff       (20)      846 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/rectangle.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1211 2022-11-12 23:06:17.000000 MHCInc-0.2.4/MHCInc/MHCInc/robot_builder.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     4608 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/screen_pet.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     4285 2022-12-24 11:27:44.000000 MHCInc-0.2.4/MHCInc/MHCInc/swift.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1570 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/加密消息.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     4373 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/单词九连猜.py
--rw-r--r--   0 mhcteam    (501) staff       (20)      413 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/圆筒万花筒.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     3245 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/快照抓拍.py
--rw-r--r--   0 mhcteam    (501) staff       (20)      805 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/星光夜空.py
--rw-r--r--   0 mhcteam    (501) staff       (20)      576 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/螺旋万花筒.py
-drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2023-04-11 21:59:27.770457 MHCInc-0.2.4/MHCInc/MHCInc.egg-info/
--rw-r--r--   0 mhcteam    (501) staff       (20)     2864 2023-04-11 21:59:27.000000 MHCInc-0.2.4/MHCInc/MHCInc.egg-info/PKG-INFO
--rw-r--r--   0 mhcteam    (501) staff       (20)      954 2023-04-11 21:59:27.000000 MHCInc-0.2.4/MHCInc/MHCInc.egg-info/SOURCES.txt
--rw-r--r--   0 mhcteam    (501) staff       (20)        1 2023-04-11 21:59:27.000000 MHCInc-0.2.4/MHCInc/MHCInc.egg-info/dependency_links.txt
--rw-r--r--   0 mhcteam    (501) staff       (20)        7 2023-04-11 21:59:27.000000 MHCInc-0.2.4/MHCInc/MHCInc.egg-info/top_level.txt
--rw-r--r--   0 mhcteam    (501) staff       (20)     2864 2023-04-11 21:59:27.770633 MHCInc-0.2.4/PKG-INFO
--rw-r--r--   0 mhcteam    (501) staff       (20)     2310 2022-11-26 10:34:41.000000 MHCInc-0.2.4/README.rst
--rw-r--r--   0 mhcteam    (501) staff       (20)       87 2022-11-13 01:29:47.000000 MHCInc-0.2.4/pyproject.toml
--rw-r--r--   0 mhcteam    (501) staff       (20)       38 2023-04-11 21:59:27.770805 MHCInc-0.2.4/setup.cfg
--rw-r--r--   0 mhcteam    (501) staff       (20)      858 2023-04-11 21:59:21.000000 MHCInc-0.2.4/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:19:32.640518 mhcinc-0.2.5/
+-rw-r--r--   0 mac        (501) staff       (20)     1074 2024-04-30 14:10:51.000000 mhcinc-0.2.5/LICENSE
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:19:32.634658 mhcinc-0.2.5/MHCInc/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:19:32.638940 mhcinc-0.2.5/MHCInc/MHCInc/
+-rw-r--r--   0 mac        (501) staff       (20)     5891 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/GuessGame.py
+-rw-r--r--   0 mac        (501) staff       (20)    15461 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/GuessGameEasy.py
+-rw-r--r--   0 mac        (501) staff       (20)    11622 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/GuessGameSecondary.py
+-rw-r--r--   0 mac        (501) staff       (20)     1211 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/MITLicense.py
+-rw-r--r--   0 mac        (501) staff       (20)     3751 2024-04-30 14:03:53.000000 mhcinc-0.2.5/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py
+-rw-r--r--   0 mac        (501) staff       (20)      808 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/Python3学习示例.py
+-rw-r--r--   0 mac        (501) staff       (20)     4084 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1028 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/animal_guess.py
+-rw-r--r--   0 mac        (501) staff       (20)     4058 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/caterpillar.py
+-rw-r--r--   0 mac        (501) staff       (20)     2891 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/caterpillar2.py
+-rw-r--r--   0 mac        (501) staff       (20)     1148 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/copyright.py
+-rw-r--r--   0 mac        (501) staff       (20)     3274 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/egg_catcher.py
+-rw-r--r--   0 mac        (501) staff       (20)     3533 2024-04-30 14:02:46.000000 mhcinc-0.2.5/MHCInc/MHCInc/egg_catcher_perfect.py
+-rw-r--r--   0 mac        (501) staff       (20)     1953 2024-04-30 14:03:06.000000 mhcinc-0.2.5/MHCInc/MHCInc/matchmaker.py
+-rw-r--r--   0 mac        (501) staff       (20)     2917 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/random.py
+-rw-r--r--   0 mac        (501) staff       (20)      846 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/rectangle.py
+-rw-r--r--   0 mac        (501) staff       (20)     1211 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/robot_builder.py
+-rw-r--r--   0 mac        (501) staff       (20)     4608 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/screen_pet.py
+-rw-r--r--   0 mac        (501) staff       (20)     4285 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/swift.py
+-rw-r--r--   0 mac        (501) staff       (20)     1570 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/加密消息.py
+-rw-r--r--   0 mac        (501) staff       (20)     4373 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/单词九连猜.py
+-rw-r--r--   0 mac        (501) staff       (20)      413 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/圆筒万花筒.py
+-rw-r--r--   0 mac        (501) staff       (20)     3245 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/快照抓拍.py
+-rw-r--r--   0 mac        (501) staff       (20)      805 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/星光夜空.py
+-rw-r--r--   0 mac        (501) staff       (20)      576 2022-12-23 19:29:10.000000 mhcinc-0.2.5/MHCInc/MHCInc/螺旋万花筒.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-04-30 15:19:32.639963 mhcinc-0.2.5/MHCInc/MHCInc.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2906 2024-04-30 15:19:32.000000 mhcinc-0.2.5/MHCInc/MHCInc.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      986 2024-04-30 15:19:32.000000 mhcinc-0.2.5/MHCInc/MHCInc.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-04-30 15:19:32.000000 mhcinc-0.2.5/MHCInc/MHCInc.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       25 2024-04-30 15:19:32.000000 mhcinc-0.2.5/MHCInc/MHCInc.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        7 2024-04-30 15:19:32.000000 mhcinc-0.2.5/MHCInc/MHCInc.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)     2906 2024-04-30 15:19:32.640248 mhcinc-0.2.5/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2310 2024-04-30 14:13:25.000000 mhcinc-0.2.5/README.rst
+-rw-r--r--   0 mac        (501) staff       (20)       87 2022-12-23 19:29:10.000000 mhcinc-0.2.5/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-04-30 15:19:32.640580 mhcinc-0.2.5/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      895 2024-04-30 15:19:10.000000 mhcinc-0.2.5/setup.py
```

### Comparing `MHCInc-0.2.4/LICENSE.txt` & `mhcinc-0.2.5/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 Copyright © 2018 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/GuessGame.py` & `mhcinc-0.2.5/MHCInc/MHCInc/GuessGame.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/GuessGameEasy.py` & `mhcinc-0.2.5/MHCInc/MHCInc/GuessGameEasy.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/GuessGameSecondary.py` & `mhcinc-0.2.5/MHCInc/MHCInc/GuessGameSecondary.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/MITLicense.py` & `mhcinc-0.2.5/MHCInc/MHCInc/MITLicense.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py` & `mhcinc-0.2.5/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 root = tit.Tk()
 root.title('PHYSICAL CONDITION APPLET')
 c = tit.Canvas(root,width=800,height=800,bg='black')
 c.pack()
 c.create_text(50,50,anchor='nw',fill='orange',\
               font='Arial 28 bold underline',text='Welcome to the physical condition applet')
 mixer.init()
-beep=mixer.Sound('MHCInc/200bpm%E6%AD%BB%E4%BA%A1%E4%B9%8B%E6%9B%B2 2.flac')
+beep=mixer.Sound(os.path.abspath('MHCInc/200bpm%E6%AD%BB%E4%BA%A1%E4%B9%8B%E6%9B%B2 2.flac'))
 beep.play()
 time.sleep(5)
 
 def write():
         print('Creating a new file')
         name = 'APPLET'+'.txt'  # Name of text file coerced with +.txt
         try:
```

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/Python3学习示例.py` & `mhcinc-0.2.5/MHCInc/MHCInc/Python3学习示例.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/animal_guess.py` & `mhcinc-0.2.5/MHCInc/MHCInc/animal_guess.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/caterpillar.py` & `mhcinc-0.2.5/MHCInc/MHCInc/caterpillar.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/caterpillar2.py` & `mhcinc-0.2.5/MHCInc/MHCInc/caterpillar2.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/copyright.py` & `mhcinc-0.2.5/MHCInc/MHCInc/copyright.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/egg_catcher.py` & `mhcinc-0.2.5/MHCInc/MHCInc/egg_catcher.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/egg_catcher_perfect.py` & `mhcinc-0.2.5/MHCInc/MHCInc/egg_catcher_perfect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from itertools import cycle
 from random import randrange
 from tkinter import Canvas,Tk,messagebox,font,PhotoImage
 from pygame import mixer
 import time
 
 mixer.init()
-beep=mixer.Sound('MHCInc/200bpm%E6%AD%BB%E4%BA%A1%E4%B9%8B%E6%9B%B2 2.flac')
+
+beep=mixer.Sound(os.path.abspath('MHCInc/200bpm%E6%AD%BB%E4%BA%A1%E4%B9%8B%E6%9B%B2 2.flac'))
 beep.play()
 time.sleep(5)
 
 canvas_width=800
 canvas_height=400
 
 root=Tk()
 root.title('PSYDUCK MADE GAMING')
-photo=PhotoImage(file='/Library/Frameworks/Python.framework/Versions/3.11/lib/python3.11/site-packages/MHCInc/8bq.png')
+photo=PhotoImage(file=os.path.abspath('MHCInc/8bq.png'))
 c=Canvas(root,width=canvas_width,height=canvas_height,background='deep sky blue')
 c.create_image(0,0,anchor='nw',image=photo)
 c.create_oval(-5,canvas_height-100,canvas_width+5,\
                                canvas_height+5,fill='sea green',width=0)
 c.create_oval(-80,-80,120,120,fill='orange',width=0)
 c.pack()
```

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/matchmaker.py` & `mhcinc-0.2.5/MHCInc/MHCInc/matchmaker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import time
 from tkinter import Tk,Button,DISABLED,messagebox
 from pygame import mixer
 
 mixer.init()
-beep=mixer.Sound('MHCInc/200bpm%E6%AD%BB%E4%BA%A1%E4%B9%8B%E6%9B%B2 2.flac')
+beep=mixer.Sound(os.path.abspath('MHCInc/200bpm%E6%AD%BB%E4%BA%A1%E4%B9%8B%E6%9B%B2 2.flac'))
 beep.play()
 time.sleep(5)
 
 def show_symbol(x,y):
     global first
     global previousX,previousY
     global moves
```

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/random.py` & `mhcinc-0.2.5/MHCInc/MHCInc/random.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/rectangle.py` & `mhcinc-0.2.5/MHCInc/MHCInc/rectangle.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/robot_builder.py` & `mhcinc-0.2.5/MHCInc/MHCInc/robot_builder.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/screen_pet.py` & `mhcinc-0.2.5/MHCInc/MHCInc/screen_pet.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/swift.py` & `mhcinc-0.2.5/MHCInc/MHCInc/swift.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/加密消息.py` & `mhcinc-0.2.5/MHCInc/MHCInc/加密消息.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/单词九连猜.py` & `mhcinc-0.2.5/MHCInc/MHCInc/单词九连猜.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/快照抓拍.py` & `mhcinc-0.2.5/MHCInc/MHCInc/快照抓拍.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/星光夜空.py` & `mhcinc-0.2.5/MHCInc/MHCInc/星光夜空.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc/螺旋万花筒.py` & `mhcinc-0.2.5/MHCInc/MHCInc/螺旋万花筒.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc.egg-info/PKG-INFO` & `mhcinc-0.2.5/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,13 @@
-Metadata-Version: 2.1
-Name: MHCInc
-Version: 0.2.4
-Summary: 改进漏洞：重复模块引用时无法配置删除的环境，使用MHCInc.module.setup()即可
-Home-page: https://pypi.org/project/MHCInc/
-Author: Mhc-inc
-Author-email: Wf6350177@163.com
-Project-URL: Bug Tracker, https://github.com/Mhc-inc/MHCInc/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 #Swift Apple
 
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Mhc-Inc/MHCInc) ![GitHub License](https://img.shields.io/github/license/Mhc-Inc/MHCInc) ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Mhc-Inc/MHCInc?include_prereleases) ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/Mhc-Inc/MHCInc.svg)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Mhc-Inc/MHCInc)
+![GitHub License](https://img.shields.io/github/license/Mhc-Inc/MHCInc)
+![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Mhc-Inc/MHCInc?include_prereleases)
+![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/Mhc-Inc/MHCInc.svg)
 update Swift-Module-Copiseded
 
 Installation
 ---------------
 
 1.You can use [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/) to write your content.You can use:
```

### Comparing `MHCInc-0.2.4/MHCInc/MHCInc.egg-info/SOURCES.txt` & `mhcinc-0.2.5/MHCInc/MHCInc.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENSE.txt
+LICENSE
 README.rst
 pyproject.toml
 setup.py
 MHCInc/MHCInc/GuessGame.py
 MHCInc/MHCInc/GuessGameEasy.py
 MHCInc/MHCInc/GuessGameSecondary.py
 MHCInc/MHCInc/MITLicense.py
@@ -26,8 +26,9 @@
 MHCInc/MHCInc/圆筒万花筒.py
 MHCInc/MHCInc/快照抓拍.py
 MHCInc/MHCInc/星光夜空.py
 MHCInc/MHCInc/螺旋万花筒.py
 MHCInc/MHCInc.egg-info/PKG-INFO
 MHCInc/MHCInc.egg-info/SOURCES.txt
 MHCInc/MHCInc.egg-info/dependency_links.txt
+MHCInc/MHCInc.egg-info/requires.txt
 MHCInc/MHCInc.egg-info/top_level.txt
```

### Comparing `MHCInc-0.2.4/PKG-INFO` & `mhcinc-0.2.5/MHCInc/MHCInc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: MHCInc
-Version: 0.2.4
-Summary: 改进漏洞：重复模块引用时无法配置删除的环境，使用MHCInc.module.setup()即可
+Version: 0.2.5
+Summary: 改进漏洞：将使用模块功能时找不到文件优化
 Home-page: https://pypi.org/project/MHCInc/
 Author: Mhc-inc
 Author-email: Wf6350177@163.com
 Project-URL: Bug Tracker, https://github.com/Mhc-inc/MHCInc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
+Requires-Dist: lxml
+Requires-Dist: requests
+Requires-Dist: bs4
+Requires-Dist: pygame
 
 #Swift Apple
 
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Mhc-Inc/MHCInc) ![GitHub License](https://img.shields.io/github/license/Mhc-Inc/MHCInc) ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Mhc-Inc/MHCInc?include_prereleases) ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/Mhc-Inc/MHCInc.svg)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Mhc-Inc/MHCInc)
+![GitHub License](https://img.shields.io/github/license/Mhc-Inc/MHCInc)
+![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Mhc-Inc/MHCInc?include_prereleases)
+![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/Mhc-Inc/MHCInc.svg)
 update Swift-Module-Copiseded
 
 Installation
 ---------------
 
 1.You can use [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/) to write your content.You can use:
```

### Comparing `MHCInc-0.2.4/setup.py` & `mhcinc-0.2.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import setuptools
 
 with open("README.rst", "r",encoding = "UTF-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="MHCInc",
-    version="0.2.4",
+    version="0.2.5",
     author="Mhc-inc",
     author_email="Wf6350177@163.com",
-    description="改进漏洞：重复模块引用时无法配置删除的环境，使用MHCInc.module.setup()即可",
+    description="改进漏洞：将使用模块功能时找不到文件优化",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/MHCInc/",
     project_urls={
         "Bug Tracker": "https://github.com/Mhc-inc/MHCInc/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    install_requires=['lxml',
+                  'requests','bs4','pygame'],
     package_dir={"": "MHCInc"},
     packages=setuptools.find_packages(where="MHCInc"),
     python_requires=">=3.9",
 )
```

