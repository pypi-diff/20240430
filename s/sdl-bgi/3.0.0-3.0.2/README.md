# Comparing `tmp/sdl_bgi-3.0.0.tar.gz` & `tmp/sdl_bgi-3.0.2.tar.gz`

## Comparing `sdl_bgi-3.0.0.tar` & `sdl_bgi-3.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/src/sdl_bgi/__init__.py
--rw-r--r--   0        0        0    40776 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/src/sdl_bgi/sdl_bgi.py
--rwxr-xr-x   0        0        0     1815 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/boo.py
--rwxr-xr-x   0        0        0     2648 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/buffers.py
--rwxr-xr-x   0        0        0     2414 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/buffers_numpy.py
--rwxr-xr-x   0        0        0     3043 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/cellular.py
--rwxr-xr-x   0        0        0     4079 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/dla.py
--rwxr-xr-x   0        0        0     2300 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/fern.py
--rwxr-xr-x   0        0        0     1720 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/floodfilltest.py
--rwxr-xr-x   0        0        0     5619 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/fonts.py
--rwxr-xr-x   0        0        0     2184 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/hopalong.py
--rwxr-xr-x   0        0        0     4168 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/kaleido.py
--rwxr-xr-x   0        0        0     4293 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/life.py
--rwxr-xr-x   0        0        0     3073 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/linebuffers.py
--rwxr-xr-x   0        0        0     8349 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/mandelbrot.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/minimal.py
--rwxr-xr-x   0        0        0     3234 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/mousetest.py
--rwxr-xr-x   0        0        0     2546 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/multiwin.py
--rwxr-xr-x   0        0        0     2406 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/pdj.py
--rwxr-xr-x   0        0        0     1891 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/plasma.py
--rwxr-xr-x   0        0        0     3921 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/psychedelia.py
--rwxr-xr-x   0        0        0     2597 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/rgbpalette.py
--rwxr-xr-x   0        0        0     2932 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/test/simple.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/LICENSE
--rw-r--r--   0        0        0    10455 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/README.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    11816 2020-02-02 00:00:00.000000 sdl_bgi-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/src/sdl_bgi/__init__.py
+-rw-r--r--   0        0        0    41156 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/src/sdl_bgi/sdl_bgi.py
+-rwxr-xr-x   0        0        0     1815 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/boo.py
+-rwxr-xr-x   0        0        0     2648 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/buffers.py
+-rwxr-xr-x   0        0        0     2414 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/buffers_numpy.py
+-rwxr-xr-x   0        0        0     3043 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/cellular.py
+-rwxr-xr-x   0        0        0     4079 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/dla.py
+-rwxr-xr-x   0        0        0     2300 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/fern.py
+-rwxr-xr-x   0        0        0     1720 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/floodfilltest.py
+-rwxr-xr-x   0        0        0     5619 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/fonts.py
+-rwxr-xr-x   0        0        0     2184 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/hopalong.py
+-rwxr-xr-x   0        0        0     4168 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/kaleido.py
+-rwxr-xr-x   0        0        0     4293 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/life.py
+-rwxr-xr-x   0        0        0     3073 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/linebuffers.py
+-rwxr-xr-x   0        0        0     8349 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/mandelbrot.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/minimal.py
+-rwxr-xr-x   0        0        0     3234 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/mousetest.py
+-rwxr-xr-x   0        0        0     2546 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/multiwin.py
+-rwxr-xr-x   0        0        0     2406 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/pdj.py
+-rwxr-xr-x   0        0        0     1891 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/plasma.py
+-rwxr-xr-x   0        0        0     3921 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/psychedelia.py
+-rwxr-xr-x   0        0        0     2597 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/rgbpalette.py
+-rwxr-xr-x   0        0        0     2932 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/test/simple.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/LICENSE
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/README.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11752 2020-02-02 00:00:00.000000 sdl_bgi-3.0.2/PKG-INFO
```

### Comparing `sdl_bgi-3.0.0/src/sdl_bgi/__init__.py` & `sdl_bgi-3.0.2/src/sdl_bgi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 functions can be used alongside `SDL_bgi` functions. `SDL_bgi` can
 also be used in programs written in C++ or Python.
 
 `SDL_bgi` is written in C, and it should compile on any platform
 supported by SDL2; it has been tested on GNU/Linux, MS Windows (MSYS2
 + Mingw-w64, CodeBlocks, Dev-C++), macOS (High Sierra and Catalina),
 Raspios (ARM, i386), and WebAssembly (Emscripten). A few example
-programs are provided in the `test/` directory.
+programs are provided in the `demo/` directory.
 """
 
 from .sdl_bgi import *
 
 # --- end of file __init__.py
```

### Comparing `sdl_bgi-3.0.0/src/sdl_bgi/sdl_bgi.py` & `sdl_bgi-3.0.2/src/sdl_bgi/sdl_bgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 SDL_bgi is a graphics library (GRAPHICS.H) for C, C++, WebAssembly,
 and Python. It's based on SDL2 and it's portable on many platforms.
 
 By Guido Gonzato, PhD
 Automatic refresh patch, CHR font support:
 Marco Diego Aurélio Mesquita
 
-Latest update: December 12, 2022
+Latest update: May 1, 2024
 
 ZLib License
 
-Copyright (c) 2014-2022 Guido Gonzato, PhD
+Copyright (c) 2014-2024 Guido Gonzato, PhD
 
 This software is provided 'as-is', without any express or implied
 warranty. In no event will the authors be held liable for any damages
 arising from the use of this software.
 
 Permission is granted to anyone to use this software for any purpose,
 including commercial applications, and to alter it and redistribute it
@@ -33,33 +33,34 @@
 
 from ctypes       import *
 from sysconfig    import get_platform
 from random       import randint
 
 # try to load the SDL_bgi library
 
-if get_platform () == 'win-amd64':       # Windows, IDLE
+if get_platform () == 'win-amd64':            # Windows, IDLE
     sdlbgilib = ".\SDL_bgi.dll"
-elif get_platform () == 'mingw_x86_64':  # Windows, MSYS2/Mingw64
-    sdlbgilib = '/msys64/mingw64/bin/SDL_bgi.dll'
+elif get_platform () == 'mingw_x86_64_ucrt':  # Windows, MSYS2/ucrt64
+    sdlbgilib = 'SDL_bgi.dll'
 else: # GNU/Linux, macOS
     sdlbgilib = 'libSDL_bgi.so'
 
 try:
     sb = CDLL (sdlbgilib)
 except:
     print ("The sdl_bgi.py module needs the SDL_bgi library binary;")
     print ("please get it from https://sdl-bgi.sourceforge.io")
     print ("Exiting.")
     quit ()
 
-SDL_BGI_VERSION = "3.0.0"
+SDL_BGI_VERSION = "3.0.2"
 NOPE = False
 YEAH = True
 BGI_WINTITLE_LEN = 512
+PALETTE_SIZE = c_int.in_dll (sb, "PALETTE_SIZE").value
 
 # number of concurrent windows that can be created
 NUM_BGI_WIN = 16
 
 VPAGES = 4
 
 # BGI fonts
@@ -304,15 +305,15 @@
                  ("upattern", c_uint),
                  ("thickness", c_uint) ]
 
 class palettetype (Structure):
     _fields_ = [ ("size", c_ubyte),
                  ("colors", c_uint32 * (MAXCOLORS + 1)) ]
 
-# SDL_bgi extension
+# SDL_bgi extensions
 
 class rgbpalettetype (Structure):
     _fields_ = [ ("size", c_uint),
                  ("colors", c_char_p) ]
 
 class textsettingstype (Structure):
     _fields_ = [ ("font", c_int),
@@ -1246,14 +1247,22 @@
     setcolor(), setbkcolor(), setfillpattern(), and setfillstyle()
     to set a colour from the ARGB palette color entry.
     """
     return sb.RGBPALETTE (int (color))
 
 # -----
 
+def clearmouseclick (kind):
+    """
+    Clears mouse event of 'kind' type.
+    """
+    sb.clearmouseclick (int (kind))
+
+# -----
+
 def closewindow (id):
     """
     Closes the window identified by 'id'.
     """
     sb.closewindow (int (id))
 
 # -----
@@ -1476,20 +1485,24 @@
     """
     Initialises the BGI palette to the standard 16 colours.
     """
     sb.initpalette ()
 
 # -----
 
-def initwindow (width, height) -> int:
+def initwindow (width = None, height = None, title = None) -> int:
     """
     Initializes the graphics system, opening a width x height
     window. Set width or height equal to 0 for fullscreen.
     """
-    return sb.initwindow (int (width), int (height))
+    if width != None and height != None and title == None:
+        return sb._initwin_1 (int (width), int (height))
+    else:
+        return sb._initwin_2 (int (width), int (height),
+                              title.encode ('ascii'))
 
 # -----
 
 def ismouseclick (btn) -> int:
     """
     Returns True if the btn mouse button was clicked.
     """
```

### Comparing `sdl_bgi-3.0.0/test/boo.py` & `sdl_bgi-3.0.2/test/boo.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/buffers.py` & `sdl_bgi-3.0.2/test/buffers.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/buffers_numpy.py` & `sdl_bgi-3.0.2/test/buffers_numpy.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/cellular.py` & `sdl_bgi-3.0.2/test/cellular.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/dla.py` & `sdl_bgi-3.0.2/test/dla.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/fern.py` & `sdl_bgi-3.0.2/test/fern.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/floodfilltest.py` & `sdl_bgi-3.0.2/test/floodfilltest.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/fonts.py` & `sdl_bgi-3.0.2/test/fonts.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/hopalong.py` & `sdl_bgi-3.0.2/test/hopalong.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/kaleido.py` & `sdl_bgi-3.0.2/test/kaleido.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/life.py` & `sdl_bgi-3.0.2/test/life.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/linebuffers.py` & `sdl_bgi-3.0.2/test/linebuffers.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/mandelbrot.py` & `sdl_bgi-3.0.2/test/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/mousetest.py` & `sdl_bgi-3.0.2/test/mousetest.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/multiwin.py` & `sdl_bgi-3.0.2/test/multiwin.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/pdj.py` & `sdl_bgi-3.0.2/test/pdj.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/plasma.py` & `sdl_bgi-3.0.2/test/plasma.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/psychedelia.py` & `sdl_bgi-3.0.2/test/psychedelia.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/rgbpalette.py` & `sdl_bgi-3.0.2/test/rgbpalette.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/test/simple.py` & `sdl_bgi-3.0.2/test/simple.py`

 * *Files identical despite different names*

### Comparing `sdl_bgi-3.0.0/LICENSE` & `sdl_bgi-3.0.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 // ZLib License
 
-Copyright (c) 2014-2021 Guido Gonzato, PhD
+Copyright (c) 2014-2024 Guido Gonzato, PhD
 
 This software is provided 'as-is', without any express or implied
 warranty. In no event will the authors be held liable for any damages
 arising from the use of this software.
 
 Permission is granted to anyone to use this software for any purpose,
 including commercial applications, and to alter it and redistribute it
```

### Comparing `sdl_bgi-3.0.0/README.md` & `sdl_bgi-3.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -286,15 +286,15 @@
 batch file that sets up the proper runtime environment for the
 executable. Run `fern.cmd` to start the program; on MSYS2, use:
 
 ```
 test$ start fern.cmd
 ```
 
-On my GNU/Linux Mint 20.2 box, Nuitka creates a much smaller
+On my GNU/Linux Mint 21.2 box, Nuitka creates a much smaller
 executable than Pyinstaller does.
 
 
 # Links
 
 0. `SDL_bgi` home page:
    <https://sdl-bgi.sourceforge.io/>;
@@ -305,21 +305,18 @@
 
 2. BGI on Wikipedia:
    <https://en.wikipedia.org/wiki/Borland_Graphics_Interface>
 
 3. WinBGIm, a BGI port for Windows:
    <https://winbgim.codecutter.org/>
 
-4. Xbgi, a BGI XLib port:
-   <http://libxbgi.sourceforge.net/>
+4. Borland Turbo C 2.01 online emulator:
+   <https://archive.org/details/msdos_borland_turbo_c_2.01>
 
 5. PyEasyGraphics, a BGI-like Python port:
    <https://github.com/royqh1979/PyEasyGraphics>
 
-6. Borland Turbo C 2.01 online emulator:
-   <https://archive.org/details/msdos_borland_turbo_c_2.01>
-
 This library is released under the Zlib license; please see the
 enclosed file LICENSE.
 
 Brought to you by Guido Gonzato, PhD
 <guido dot gonzato at gmail dot com>
```

### Comparing `sdl_bgi-3.0.0/pyproject.toml` & `sdl_bgi-3.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name        = "sdl_bgi"
-version     = "3.0.0"
+version     = "3.0.2"
 description = "SDL2-based 'GRAPHICS.H' implementation"
 authors = [
   { name="Guido Gonzato, PhD", email="guido.gonzato@gmail.com" },
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
```

### Comparing `sdl_bgi-3.0.0/PKG-INFO` & `sdl_bgi-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sdl_bgi
-Version: 3.0.0
+Version: 3.0.2
 Summary: SDL2-based 'GRAPHICS.H' implementation
 Project-URL: Homepage, https://sdl-bgi.sourceforge.io/
 Author-email: "Guido Gonzato, PhD" <guido.gonzato@gmail.com>
 License: // ZLib License
         
-        Copyright (c) 2014-2021 Guido Gonzato, PhD
+        Copyright (c) 2014-2024 Guido Gonzato, PhD
         
         This software is provided 'as-is', without any express or implied
         warranty. In no event will the authors be held liable for any damages
         arising from the use of this software.
         
         Permission is granted to anyone to use this software for any purpose,
         including commercial applications, and to alter it and redistribute it
@@ -323,15 +323,15 @@
 batch file that sets up the proper runtime environment for the
 executable. Run `fern.cmd` to start the program; on MSYS2, use:
 
 ```
 test$ start fern.cmd
 ```
 
-On my GNU/Linux Mint 20.2 box, Nuitka creates a much smaller
+On my GNU/Linux Mint 21.2 box, Nuitka creates a much smaller
 executable than Pyinstaller does.
 
 
 # Links
 
 0. `SDL_bgi` home page:
    <https://sdl-bgi.sourceforge.io/>;
@@ -342,21 +342,18 @@
 
 2. BGI on Wikipedia:
    <https://en.wikipedia.org/wiki/Borland_Graphics_Interface>
 
 3. WinBGIm, a BGI port for Windows:
    <https://winbgim.codecutter.org/>
 
-4. Xbgi, a BGI XLib port:
-   <http://libxbgi.sourceforge.net/>
+4. Borland Turbo C 2.01 online emulator:
+   <https://archive.org/details/msdos_borland_turbo_c_2.01>
 
 5. PyEasyGraphics, a BGI-like Python port:
    <https://github.com/royqh1979/PyEasyGraphics>
 
-6. Borland Turbo C 2.01 online emulator:
-   <https://archive.org/details/msdos_borland_turbo_c_2.01>
-
 This library is released under the Zlib license; please see the
 enclosed file LICENSE.
 
 Brought to you by Guido Gonzato, PhD
 <guido dot gonzato at gmail dot com>
```

