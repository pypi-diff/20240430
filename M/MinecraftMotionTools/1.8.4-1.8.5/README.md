# Comparing `tmp/MinecraftMotionTools-1.8.4.tar.gz` & `tmp/minecraftmotiontools-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MinecraftMotionTools-1.8.4.tar", last modified: Mon Apr  8 13:08:37 2024, max compression
+gzip compressed data, was "minecraftmotiontools-1.8.5.tar", last modified: Tue Apr 30 00:18:04 2024, max compression
```

## Comparing `MinecraftMotionTools-1.8.4.tar` & `minecraftmotiontools-1.8.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-08 13:08:37.156131 MinecraftMotionTools-1.8.4/
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     1083 2024-04-08 12:39:46.000000 MinecraftMotionTools-1.8.4/LICENSE
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6889 2024-04-08 13:08:37.147014 MinecraftMotionTools-1.8.4/PKG-INFO
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6581 2024-04-08 12:39:46.000000 MinecraftMotionTools-1.8.4/README.md
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      481 2024-04-08 13:05:42.000000 MinecraftMotionTools-1.8.4/pyproject.toml
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       38 2024-04-08 13:08:37.157137 MinecraftMotionTools-1.8.4/setup.cfg
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-08 13:08:36.862990 MinecraftMotionTools-1.8.4/src/
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-08 13:08:37.135614 MinecraftMotionTools-1.8.4/src/MinecraftMotionTools.egg-info/
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6889 2024-04-08 13:08:36.000000 MinecraftMotionTools-1.8.4/src/MinecraftMotionTools.egg-info/PKG-INFO
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      392 2024-04-08 13:08:36.000000 MinecraftMotionTools-1.8.4/src/MinecraftMotionTools.egg-info/SOURCES.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        1 2024-04-08 13:08:36.000000 MinecraftMotionTools-1.8.4/src/MinecraftMotionTools.egg-info/dependency_links.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       14 2024-04-08 13:08:36.000000 MinecraftMotionTools-1.8.4/src/MinecraftMotionTools.egg-info/requires.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       23 2024-04-08 13:08:36.000000 MinecraftMotionTools-1.8.4/src/MinecraftMotionTools.egg-info/top_level.txt
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-08 13:08:37.104965 MinecraftMotionTools-1.8.4/src/minecraft_motion_tools/
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      669 2024-04-08 12:39:46.000000 MinecraftMotionTools-1.8.4/src/minecraft_motion_tools/__init__.py
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    12779 2024-04-08 13:05:24.000000 MinecraftMotionTools-1.8.4/src/minecraft_motion_tools/acceleration.py
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    10267 2024-04-08 12:39:46.000000 MinecraftMotionTools-1.8.4/src/minecraft_motion_tools/velocity.py
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-30 00:18:04.435686 minecraftmotiontools-1.8.5/
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     1083 2024-04-30 00:10:01.000000 minecraftmotiontools-1.8.5/LICENSE
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6474 2024-04-30 00:18:04.426524 minecraftmotiontools-1.8.5/PKG-INFO
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6166 2024-04-30 00:16:29.000000 minecraftmotiontools-1.8.5/README.md
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      481 2024-04-30 00:10:13.000000 minecraftmotiontools-1.8.5/pyproject.toml
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       38 2024-04-30 00:18:04.436693 minecraftmotiontools-1.8.5/setup.cfg
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-30 00:18:04.151221 minecraftmotiontools-1.8.5/src/
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-30 00:18:04.414705 minecraftmotiontools-1.8.5/src/MinecraftMotionTools.egg-info/
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6474 2024-04-30 00:18:04.000000 minecraftmotiontools-1.8.5/src/MinecraftMotionTools.egg-info/PKG-INFO
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      392 2024-04-30 00:18:04.000000 minecraftmotiontools-1.8.5/src/MinecraftMotionTools.egg-info/SOURCES.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        1 2024-04-30 00:18:04.000000 minecraftmotiontools-1.8.5/src/MinecraftMotionTools.egg-info/dependency_links.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       14 2024-04-30 00:18:04.000000 minecraftmotiontools-1.8.5/src/MinecraftMotionTools.egg-info/requires.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       23 2024-04-30 00:18:04.000000 minecraftmotiontools-1.8.5/src/MinecraftMotionTools.egg-info/top_level.txt
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-30 00:18:04.381538 minecraftmotiontools-1.8.5/src/minecraft_motion_tools/
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      669 2024-04-30 00:10:01.000000 minecraftmotiontools-1.8.5/src/minecraft_motion_tools/__init__.py
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    12779 2024-04-30 00:10:01.000000 minecraftmotiontools-1.8.5/src/minecraft_motion_tools/acceleration.py
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    10267 2024-04-30 00:10:01.000000 minecraftmotiontools-1.8.5/src/minecraft_motion_tools/velocity.py
```

### Comparing `MinecraftMotionTools-1.8.4/LICENSE` & `minecraftmotiontools-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MinecraftMotionTools-1.8.4/PKG-INFO` & `minecraftmotiontools-1.8.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinecraftMotionTools
-Version: 1.8.4
+Version: 1.8.5
 Summary: A library to compute entities' motion in Minecraft.
 Author: OrHy3
 Project-URL: Homepage, https://github.com/OrHy3/MinecraftMotionTools
 Project-URL: Issues, https://github.com/OrHy3/MinecraftMotionTools/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,33 +25,33 @@
 
 Finally, [here](https://hackmd.io/1t0ACyplTDKSgo-a1jA7nQ) is the formulas' sheet I wrote down. Take in mind that a fair amount of them make use of [Lambert's W function](https://en.wikipedia.org/wiki/Lambert_W_function).
 
 For the acceleration's formulas refer to [this sheet](https://hackmd.io/vvFAdzekSn6R7vc9Mw8lxg?view) instead.
 # Entities' parameter table
 |Type|Acceleration|Vertical drag|Horizontal drag|Applies drag|k coefficient|
 |-|-|-|-|-|-|
-|Players, mobs and armor stands|0.08|0.019999980926513672|0.0899999737739563|After|0|
-|Entities with slow falling|0.01|0.019999980926513672|0.0899999737739563|After|0|
+|Players, mobs and armor stands|0.08|0.02|0.09|After|0|
+|Entities with slow falling|0.01|0.02|0.09|After|0|
 |Items, falling blocks and TNTs|0.04|0.02|0.02|After|1|
 |Minecarts|0.04|0.05|0.05|After|1|
-|Boats|0.03999999910593033|0|0.10000002384185791|-|1|
-|Thrown eggs, snowballs and ender pearls|0.029999999329447746|0.009999990463256836|0.009999990463256836|Before|0|
-|Thrown potions|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
-|Thrown experience bottles|0.07000000029802322|0.009999990463256836|0.009999990463256836|Before|0|
-|Experience orbs|0.03|0.02|0.019999980926513672|After|1|
+|Boats|0.04|0|0.10|-|1|
+|Thrown eggs, snowballs and ender pearls|0.03|0.01|0.01|Before|0|
+|Thrown potions|0.05|0.01|0.01|Before|0|
+|Thrown experience bottles|0.07|0.01|0.01|Before|0|
+|Experience orbs|0.03|0.02|0.02|After|1|
 |Thrown fishing bobbers|0.03|0.08|0.08|After|1|
-|Llama spit|0.05999999865889549|0.009999990463256836|0.009999990463256836|Before|0|
-|Fired arrows and thrown tridents|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
-|Fireballs, wither skulls and dragon fireballs|0.1|0.050000011920928955|0.050000011920928955|After|0|
-|Dangerous wither skulls|0.1|0.26999998092651367|0.26999998092651367|After|0|
-|Wind charges|0.1|0|0|-|0|
+|Llama spit|0.06|0.01|0.01|Before|0|
+|Fired arrows and thrown tridents|0.05|0.01|0.01|Before|0|
+|Fireballs, wither skulls and dragon fireballs|0.10|0.05|0.05|After|0|
+|Dangerous wither skulls|0.10|0.27|0.27|After|0|
+|Wind charges|0.10|0|0|-|0|
 
 NOTES:
 - For fireballs and alike, use negative acceleration (see [here](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0) why).
-- Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.45399993658065796.
+- Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.454.
 - The maximum general velocity value is 10. Any greater value is reset to 0.
 - Even though 10 is the maximum velocity that can be set, entities with 0 drag force can gain infinite velocity due to acceleration.
 - Minecarts have a maximum horizontal velocity of 0.4. Any greater value is reset to that number.
 - Boats' horizontal position gets updated using next tick's velocity instead of the current one.
 # Function list
 v0: initial velocity<br>
 t: ticks passed<br>
```

### Comparing `MinecraftMotionTools-1.8.4/README.md` & `minecraftmotiontools-1.8.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 
 Finally, [here](https://hackmd.io/1t0ACyplTDKSgo-a1jA7nQ) is the formulas' sheet I wrote down. Take in mind that a fair amount of them make use of [Lambert's W function](https://en.wikipedia.org/wiki/Lambert_W_function).
 
 For the acceleration's formulas refer to [this sheet](https://hackmd.io/vvFAdzekSn6R7vc9Mw8lxg?view) instead.
 # Entities' parameter table
 |Type|Acceleration|Vertical drag|Horizontal drag|Applies drag|k coefficient|
 |-|-|-|-|-|-|
-|Players, mobs and armor stands|0.08|0.019999980926513672|0.0899999737739563|After|0|
-|Entities with slow falling|0.01|0.019999980926513672|0.0899999737739563|After|0|
+|Players, mobs and armor stands|0.08|0.02|0.09|After|0|
+|Entities with slow falling|0.01|0.02|0.09|After|0|
 |Items, falling blocks and TNTs|0.04|0.02|0.02|After|1|
 |Minecarts|0.04|0.05|0.05|After|1|
-|Boats|0.03999999910593033|0|0.10000002384185791|-|1|
-|Thrown eggs, snowballs and ender pearls|0.029999999329447746|0.009999990463256836|0.009999990463256836|Before|0|
-|Thrown potions|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
-|Thrown experience bottles|0.07000000029802322|0.009999990463256836|0.009999990463256836|Before|0|
-|Experience orbs|0.03|0.02|0.019999980926513672|After|1|
+|Boats|0.04|0|0.10|-|1|
+|Thrown eggs, snowballs and ender pearls|0.03|0.01|0.01|Before|0|
+|Thrown potions|0.05|0.01|0.01|Before|0|
+|Thrown experience bottles|0.07|0.01|0.01|Before|0|
+|Experience orbs|0.03|0.02|0.02|After|1|
 |Thrown fishing bobbers|0.03|0.08|0.08|After|1|
-|Llama spit|0.05999999865889549|0.009999990463256836|0.009999990463256836|Before|0|
-|Fired arrows and thrown tridents|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
-|Fireballs, wither skulls and dragon fireballs|0.1|0.050000011920928955|0.050000011920928955|After|0|
-|Dangerous wither skulls|0.1|0.26999998092651367|0.26999998092651367|After|0|
-|Wind charges|0.1|0|0|-|0|
+|Llama spit|0.06|0.01|0.01|Before|0|
+|Fired arrows and thrown tridents|0.05|0.01|0.01|Before|0|
+|Fireballs, wither skulls and dragon fireballs|0.10|0.05|0.05|After|0|
+|Dangerous wither skulls|0.10|0.27|0.27|After|0|
+|Wind charges|0.10|0|0|-|0|
 
 NOTES:
 - For fireballs and alike, use negative acceleration (see [here](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0) why).
-- Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.45399993658065796.
+- Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.454.
 - The maximum general velocity value is 10. Any greater value is reset to 0.
 - Even though 10 is the maximum velocity that can be set, entities with 0 drag force can gain infinite velocity due to acceleration.
 - Minecarts have a maximum horizontal velocity of 0.4. Any greater value is reset to that number.
 - Boats' horizontal position gets updated using next tick's velocity instead of the current one.
 # Function list
 v0: initial velocity<br>
 t: ticks passed<br>
```

### Comparing `MinecraftMotionTools-1.8.4/src/MinecraftMotionTools.egg-info/PKG-INFO` & `minecraftmotiontools-1.8.5/src/MinecraftMotionTools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinecraftMotionTools
-Version: 1.8.4
+Version: 1.8.5
 Summary: A library to compute entities' motion in Minecraft.
 Author: OrHy3
 Project-URL: Homepage, https://github.com/OrHy3/MinecraftMotionTools
 Project-URL: Issues, https://github.com/OrHy3/MinecraftMotionTools/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,33 +25,33 @@
 
 Finally, [here](https://hackmd.io/1t0ACyplTDKSgo-a1jA7nQ) is the formulas' sheet I wrote down. Take in mind that a fair amount of them make use of [Lambert's W function](https://en.wikipedia.org/wiki/Lambert_W_function).
 
 For the acceleration's formulas refer to [this sheet](https://hackmd.io/vvFAdzekSn6R7vc9Mw8lxg?view) instead.
 # Entities' parameter table
 |Type|Acceleration|Vertical drag|Horizontal drag|Applies drag|k coefficient|
 |-|-|-|-|-|-|
-|Players, mobs and armor stands|0.08|0.019999980926513672|0.0899999737739563|After|0|
-|Entities with slow falling|0.01|0.019999980926513672|0.0899999737739563|After|0|
+|Players, mobs and armor stands|0.08|0.02|0.09|After|0|
+|Entities with slow falling|0.01|0.02|0.09|After|0|
 |Items, falling blocks and TNTs|0.04|0.02|0.02|After|1|
 |Minecarts|0.04|0.05|0.05|After|1|
-|Boats|0.03999999910593033|0|0.10000002384185791|-|1|
-|Thrown eggs, snowballs and ender pearls|0.029999999329447746|0.009999990463256836|0.009999990463256836|Before|0|
-|Thrown potions|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
-|Thrown experience bottles|0.07000000029802322|0.009999990463256836|0.009999990463256836|Before|0|
-|Experience orbs|0.03|0.02|0.019999980926513672|After|1|
+|Boats|0.04|0|0.10|-|1|
+|Thrown eggs, snowballs and ender pearls|0.03|0.01|0.01|Before|0|
+|Thrown potions|0.05|0.01|0.01|Before|0|
+|Thrown experience bottles|0.07|0.01|0.01|Before|0|
+|Experience orbs|0.03|0.02|0.02|After|1|
 |Thrown fishing bobbers|0.03|0.08|0.08|After|1|
-|Llama spit|0.05999999865889549|0.009999990463256836|0.009999990463256836|Before|0|
-|Fired arrows and thrown tridents|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
-|Fireballs, wither skulls and dragon fireballs|0.1|0.050000011920928955|0.050000011920928955|After|0|
-|Dangerous wither skulls|0.1|0.26999998092651367|0.26999998092651367|After|0|
-|Wind charges|0.1|0|0|-|0|
+|Llama spit|0.06|0.01|0.01|Before|0|
+|Fired arrows and thrown tridents|0.05|0.01|0.01|Before|0|
+|Fireballs, wither skulls and dragon fireballs|0.10|0.05|0.05|After|0|
+|Dangerous wither skulls|0.10|0.27|0.27|After|0|
+|Wind charges|0.10|0|0|-|0|
 
 NOTES:
 - For fireballs and alike, use negative acceleration (see [here](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0) why).
-- Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.45399993658065796.
+- Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.454.
 - The maximum general velocity value is 10. Any greater value is reset to 0.
 - Even though 10 is the maximum velocity that can be set, entities with 0 drag force can gain infinite velocity due to acceleration.
 - Minecarts have a maximum horizontal velocity of 0.4. Any greater value is reset to that number.
 - Boats' horizontal position gets updated using next tick's velocity instead of the current one.
 # Function list
 v0: initial velocity<br>
 t: ticks passed<br>
```

### Comparing `MinecraftMotionTools-1.8.4/src/minecraft_motion_tools/__init__.py` & `minecraftmotiontools-1.8.5/src/minecraft_motion_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `MinecraftMotionTools-1.8.4/src/minecraft_motion_tools/acceleration.py` & `minecraftmotiontools-1.8.5/src/minecraft_motion_tools/acceleration.py`

 * *Files identical despite different names*

### Comparing `MinecraftMotionTools-1.8.4/src/minecraft_motion_tools/velocity.py` & `minecraftmotiontools-1.8.5/src/minecraft_motion_tools/velocity.py`

 * *Files identical despite different names*

