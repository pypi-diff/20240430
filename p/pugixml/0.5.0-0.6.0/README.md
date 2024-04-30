# Comparing `tmp/pugixml-0.5.0.tar.gz` & `tmp/pugixml-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pugixml-0.5.0.tar", last modified: Wed Oct  4 16:11:15 2023, max compression
+gzip compressed data, was "pugixml-0.6.0.tar", last modified: Tue Apr 30 11:30:21 2024, max compression
```

## Comparing `pugixml-0.5.0.tar` & `pugixml-0.6.0.tar`

### file list

```diff
@@ -1,135 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.186065 pugixml-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2023-10-04 16:05:35.000000 pugixml-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-04 16:05:35.000000 pugixml-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-10-04 16:05:35.000000 pugixml-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2023-10-04 16:11:15.186065 pugixml-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2023-10-04 16:05:35.000000 pugixml-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2023-10-04 16:05:35.000000 pugixml-0.5.0/_build.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-10-04 16:05:35.000000 pugixml-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2023-10-04 16:11:15.186065 pugixml-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-10-04 16:05:35.000000 pugixml-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.158064 pugixml-0.5.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2023-10-04 16:05:35.000000 pugixml-0.5.0/src/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-10-04 16:05:35.000000 pugixml-0.5.0/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)   120594 2023-10-04 16:05:35.000000 pugixml-0.5.0/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.158064 pugixml-0.5.0/src/pugixml/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-04 16:05:35.000000 pugixml-0.5.0/src/pugixml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.162064 pugixml-0.5.0/src/pugixml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2023-10-04 16:11:15.000000 pugixml-0.5.0/src/pugixml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2023-10-04 16:11:15.000000 pugixml-0.5.0/src/pugixml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 16:11:15.000000 pugixml-0.5.0/src/pugixml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 16:11:14.000000 pugixml-0.5.0/src/pugixml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-04 16:11:15.000000 pugixml-0.5.0/src/pugixml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.154064 pugixml-0.5.0/src/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.162064 pugixml-0.5.0/src/third_party/pugixml/
--rw-r--r--   0 runner    (1001) docker     (127)     8835 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.166064 pugixml-0.5.0/src/third_party/pugixml/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/archive.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/cocoapods_push.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.170064 pugixml-0.5.0/src/third_party/pugixml/scripts/natvis/
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/natvis/pugixml.natvis
--rw-r--r--   0 runner    (1001) docker     (127)    24078 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/natvis/pugixml_compact.natvis
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.170064 pugixml-0.5.0/src/third_party/pugixml/scripts/nuget/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.154064 pugixml-0.5.0/src/third_party/pugixml/scripts/nuget/build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.170064 pugixml-0.5.0/src/third_party/pugixml/scripts/nuget/build/native/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/nuget/build/native/pugixml-propertiesui.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/nuget/build/native/pugixml.targets
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/nuget/pugixml.nuspec
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/nuget_build.ps1
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/premake4.lua
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml-config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml.podspec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.170064 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml.xcodeproj/
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml.xcodeproj/project.pbxproj
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_airplay.mkf
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_codeblocks.cbp
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_codelite.project
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_dll.rc
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2005.vcproj
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2005_static.vcproj
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2008.vcproj
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2008_static.vcproj
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2010.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2010_static.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2013.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2013_static.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2015.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     8787 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2015_static.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2017.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2017_static.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2019.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2019_static.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2022.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     8614 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2022_static.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.170064 pugixml-0.5.0/src/third_party/pugixml/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/src/pugiconfig.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   346827 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/src/pugixml.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    54297 2023-10-04 16:05:36.000000 pugixml-0.5.0/src/third_party/pugixml/src/pugixml.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.170064 pugixml-0.5.0/src/third_party/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    12067 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.154064 pugixml-0.5.0/src/third_party/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.174064 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    24334 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (127)    67312 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.178064 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (127)    28518 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (127)    53480 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (127)    17859 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (127)    28221 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (127)    48364 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.178064 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/eigen/common.h
--rw-r--r--   0 runner    (1001) docker     (127)    32135 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    18442 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (127)    79725 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (127)   126706 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (127)    98455 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.178064 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (127)    15477 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (127)    29897 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/include/pybind11/type_caster_pyobject_ptr.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.182064 pugixml-0.5.0/src/third_party/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner    (1001) docker     (127)     1423 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)    14449 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-10-04 16:05:37.000000 pugixml-0.5.0/src/third_party/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 16:11:15.182064 pugixml-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-10-04 16:05:35.000000 pugixml-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13209 2023-10-04 16:05:35.000000 pugixml-0.5.0/tests/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2023-10-04 16:05:35.000000 pugixml-0.5.0/tests/test_document.py
--rw-r--r--   0 runner    (1001) docker     (127)    56290 2023-10-04 16:05:35.000000 pugixml-0.5.0/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2023-10-04 16:05:35.000000 pugixml-0.5.0/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    17829 2023-10-04 16:05:35.000000 pugixml-0.5.0/tests/test_xpath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.091216 pugixml-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-30 11:27:11.000000 pugixml-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 11:27:11.000000 pugixml-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-30 11:27:11.000000 pugixml-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-30 11:30:21.091216 pugixml-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-30 11:27:11.000000 pugixml-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-30 11:27:11.000000 pugixml-0.6.0/_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 11:27:11.000000 pugixml-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-30 11:30:21.091216 pugixml-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 11:27:11.000000 pugixml-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.071216 pugixml-0.6.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-30 11:27:11.000000 pugixml-0.6.0/src/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-30 11:27:11.000000 pugixml-0.6.0/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   120583 2024-04-30 11:27:11.000000 pugixml-0.6.0/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.071216 pugixml-0.6.0/src/pugixml/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 11:27:11.000000 pugixml-0.6.0/src/pugixml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.091216 pugixml-0.6.0/src/pugixml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-30 11:30:21.000000 pugixml-0.6.0/src/pugixml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-30 11:30:21.000000 pugixml-0.6.0/src/pugixml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:30:21.000000 pugixml-0.6.0/src/pugixml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:30:20.000000 pugixml-0.6.0/src/pugixml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 11:30:21.000000 pugixml-0.6.0/src/pugixml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.071216 pugixml-0.6.0/src/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.075216 pugixml-0.6.0/src/third_party/pugixml/
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.079216 pugixml-0.6.0/src/third_party/pugixml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/cocoapods_push.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.079216 pugixml-0.6.0/src/third_party/pugixml/scripts/natvis/
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/natvis/pugixml.natvis
+-rw-r--r--   0 runner    (1001) docker     (127)    24078 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/natvis/pugixml_compact.natvis
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.079216 pugixml-0.6.0/src/third_party/pugixml/scripts/nuget/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.071216 pugixml-0.6.0/src/third_party/pugixml/scripts/nuget/build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.079216 pugixml-0.6.0/src/third_party/pugixml/scripts/nuget/build/native/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/nuget/build/native/pugixml-propertiesui.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/nuget/build/native/pugixml.targets
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/nuget/pugixml.nuspec
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/nuget_build.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/premake4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml-config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml.podspec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.079216 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml.xcodeproj/project.pbxproj
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_airplay.mkf
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_codeblocks.cbp
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_codelite.project
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_dll.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2005.vcproj
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2005_static.vcproj
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2008.vcproj
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2008_static.vcproj
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2010.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2010_static.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2013.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2013_static.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2015.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     8787 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2015_static.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2017.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2017_static.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2019.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2019_static.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2022.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2022_static.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.079216 pugixml-0.6.0/src/third_party/pugixml/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/src/pugiconfig.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   346827 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/src/pugixml.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    54297 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pugixml/src/pugixml.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.079216 pugixml-0.6.0/src/third_party/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    14018 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.071216 pugixml-0.6.0/src/third_party/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.083216 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (127)    71139 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.087216 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)    28563 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53771 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29033 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49892 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.087216 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/eigen/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/gil_safe_call_once.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    84243 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (127)   129569 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (127)    98953 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.087216 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28472 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/include/pybind11/typing.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.087216 pugixml-0.6.0/src/third_party/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1423 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2090 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     8569 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-30 11:27:12.000000 pugixml-0.6.0/src/third_party/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:30:21.091216 pugixml-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-30 11:27:11.000000 pugixml-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-04-30 11:27:11.000000 pugixml-0.6.0/tests/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-30 11:27:11.000000 pugixml-0.6.0/tests/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56290 2024-04-30 11:27:11.000000 pugixml-0.6.0/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-30 11:27:11.000000 pugixml-0.6.0/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17829 2024-04-30 11:27:11.000000 pugixml-0.6.0/tests/test_xpath.py
```

### Comparing `pugixml-0.5.0/LICENSE` & `pugixml-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/PKG-INFO` & `pugixml-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: pugixml
-Version: 0.5.0
+Version: 0.6.0
 Summary: Light-weight, simple and fast XML parser with XPath support
 Home-page: https://github.com/miute/pugixml-python
 Author: Tetsuya Miura
 Author-email: miute.dev@gmail.com
 License: MIT
 Keywords: dom,xml,xpath,xml-parser
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup :: XML
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python bindings for pugixml
 
 [![PyPI](https://img.shields.io/pypi/v/pugixml)](https://pypi.org/project/pugixml/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pugixml)](https://pypi.org/project/pugixml/)
```

### Comparing `pugixml-0.5.0/README.md` & `pugixml-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/_build.py` & `pugixml-0.6.0/_build.py`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/setup.cfg` & `pugixml-0.6.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pugixml
-version = 0.5.0
+version = 0.6.0
 description = Light-weight, simple and fast XML parser with XPath support
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Tetsuya Miura
 author_email = miute.dev@gmail.com
 url = https://github.com/miute/pugixml-python
 classifiers = 
@@ -12,15 +12,14 @@
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Programming Language :: C++
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Topic :: Software Development :: Libraries
 	Topic :: Text Processing :: Markup :: XML
@@ -34,15 +33,15 @@
 [options]
 packages = find:
 package_dir = 
 	= src
 include_package_data = True
 zip_safe = False
 install_requires = 
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 where = src
 
 [flake8]
 max-line-length = 88
 ignore = E203,W503
```

### Comparing `pugixml-0.5.0/src/.clang-format` & `pugixml-0.6.0/src/.clang-format`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/CMakeLists.txt` & `pugixml-0.6.0/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/main.cpp` & `pugixml-0.6.0/src/main.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -7156,383 +7156,382 @@
 0001bf30: 7320 7369 7a65 2069 6e20 6279 7465 732e  s size in bytes.
 0001bf40: 0a0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
 0001bf50: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
 0001bf60: 2020 2020 2020 2069 6e74 3a20 5468 6520         int: The 
 0001bf70: 636f 6e74 656e 7473 2073 697a 6520 696e  contents size in
 0001bf80: 2062 7974 6573 2e0a 2020 2020 2020 2020   bytes..        
 0001bf90: 2020 2020 2964 6f63 2229 0a20 2020 2020      )doc").     
-0001bfa0: 202e 6465 6628 0a20 2020 2020 2020 2020   .def(.         
-0001bfb0: 2022 6765 7476 616c 7565 222c 205b 5d28   "getvalue", [](
-0001bfc0: 636f 6e73 7420 4279 7465 7357 7269 7465  const BytesWrite
-0001bfd0: 7220 2673 656c 6629 207b 2072 6574 7572  r &self) { retur
-0001bfe0: 6e20 7079 3a3a 6279 7465 7328 7365 6c66  n py::bytes(self
-0001bff0: 2e63 6f6e 7465 6e74 7329 3b20 7d2c 2052  .contents); }, R
-0001c000: 2264 6f63 280a 2020 2020 2020 2020 2020  "doc(.          
-0001c010: 5265 7475 726e 2074 6865 2065 6e74 6972  Return the entir
-0001c020: 6520 636f 6e74 656e 7473 206f 6620 7468  e contents of th
-0001c030: 6520 6275 6666 6572 2e0a 0a20 2020 2020  e buffer...     
-0001c040: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-0001c050: 2020 2020 2020 2020 2020 2020 6279 7465              byte
-0001c060: 733a 2054 6865 2065 6e74 6972 6520 636f  s: The entire co
-0001c070: 6e74 656e 7473 206f 6620 7468 6520 6275  ntents of the bu
-0001c080: 6666 6572 2e0a 2020 2020 2020 2020 2020  ffer..          
-0001c090: 2964 6f63 2229 3b0a 0a20 202f 2f0a 2020  )doc");..  //.  
-0001c0a0: 2f2f 2046 696c 6557 7269 7465 720a 2020  // FileWriter.  
-0001c0b0: 2f2f 0a20 2073 7472 7563 7420 4669 6c65  //.  struct File
-0001c0c0: 5772 6974 6572 203a 2070 7562 6c69 6320  Writer : public 
-0001c0d0: 786d 6c5f 7772 6974 6572 207b 0a20 2020  xml_writer {.   
-0001c0e0: 2073 7464 3a3a 6f66 7374 7265 616d 2066   std::ofstream f
-0001c0f0: 696c 653b 0a20 2020 2046 696c 6557 7269  ile;.    FileWri
-0001c100: 7465 7228 636f 6e73 7420 6673 3a3a 7061  ter(const fs::pa
-0001c110: 7468 2026 7061 7468 2920 7b0a 2020 2020  th &path) {.    
-0001c120: 2020 7472 7920 7b0a 2020 2020 2020 2020    try {.        
-0001c130: 6669 6c65 2e6f 7065 6e28 7061 7468 2c20  file.open(path, 
-0001c140: 7374 643a 3a69 6f73 5f62 6173 653a 3a6f  std::ios_base::o
-0001c150: 7574 207c 2073 7464 3a3a 696f 735f 6261  ut | std::ios_ba
-0001c160: 7365 3a3a 6269 6e61 7279 293b 0a20 2020  se::binary);.   
-0001c170: 2020 2020 2066 696c 652e 6578 6365 7074       file.except
-0001c180: 696f 6e73 2873 7464 3a3a 696f 735f 6261  ions(std::ios_ba
-0001c190: 7365 3a3a 6661 696c 6269 7420 7c20 7374  se::failbit | st
-0001c1a0: 643a 3a69 6f73 5f62 6173 653a 3a62 6164  d::ios_base::bad
-0001c1b0: 6269 7429 3b0a 2020 2020 2020 7d20 6361  bit);.      } ca
-0001c1c0: 7463 6820 2863 6f6e 7374 2073 7464 3a3a  tch (const std::
-0001c1d0: 6578 6365 7074 696f 6e20 2665 2920 7b0a  exception &e) {.
-0001c1e0: 2020 2020 2020 2020 5079 4572 725f 5365          PyErr_Se
-0001c1f0: 7453 7472 696e 6728 5079 4578 635f 4f53  tString(PyExc_OS
-0001c200: 4572 726f 722c 2065 2e77 6861 7428 2929  Error, e.what())
-0001c210: 3b0a 2020 2020 2020 2020 7468 726f 7720  ;.        throw 
-0001c220: 7079 3a3a 6572 726f 725f 616c 7265 6164  py::error_alread
-0001c230: 795f 7365 7428 293b 0a20 2020 2020 207d  y_set();.      }
-0001c240: 0a20 2020 207d 0a20 2020 2076 6f69 6420  .    }.    void 
-0001c250: 636c 6f73 6528 2920 7b0a 2020 2020 2020  close() {.      
-0001c260: 6966 2028 6669 6c65 2e69 735f 6f70 656e  if (file.is_open
-0001c270: 2829 2920 7b0a 2020 2020 2020 2020 6669  ()) {.        fi
-0001c280: 6c65 2e63 6c6f 7365 2829 3b0a 2020 2020  le.close();.    
-0001c290: 2020 7d0a 2020 2020 7d0a 2020 2020 766f    }.    }.    vo
-0001c2a0: 6964 2077 7269 7465 2863 6f6e 7374 2076  id write(const v
-0001c2b0: 6f69 6420 2a64 6174 612c 2073 697a 655f  oid *data, size_
-0001c2c0: 7420 7369 7a65 2920 6f76 6572 7269 6465  t size) override
-0001c2d0: 207b 0a20 2020 2020 2074 7279 207b 0a20   {.      try {. 
-0001c2e0: 2020 2020 2020 2066 696c 652e 7772 6974         file.writ
-0001c2f0: 6528 7374 6174 6963 5f63 6173 743c 636f  e(static_cast<co
-0001c300: 6e73 7420 6368 6172 202a 3e28 6461 7461  nst char *>(data
-0001c310: 292c 2073 697a 6529 3b0a 2020 2020 2020  ), size);.      
-0001c320: 7d20 6361 7463 6820 2863 6f6e 7374 2073  } catch (const s
-0001c330: 7464 3a3a 6578 6365 7074 696f 6e20 2665  td::exception &e
-0001c340: 2920 7b0a 2020 2020 2020 2020 5079 4572  ) {.        PyEr
-0001c350: 725f 5365 7453 7472 696e 6728 5079 4578  r_SetString(PyEx
-0001c360: 635f 4f53 4572 726f 722c 2065 2e77 6861  c_OSError, e.wha
-0001c370: 7428 2929 3b0a 2020 2020 2020 2020 7468  t());.        th
-0001c380: 726f 7720 7079 3a3a 6572 726f 725f 616c  row py::error_al
-0001c390: 7265 6164 795f 7365 7428 293b 0a20 2020  ready_set();.   
-0001c3a0: 2020 207d 0a20 2020 207d 0a20 207d 3b0a     }.    }.  };.
-0001c3b0: 0a20 2070 793a 3a63 6c61 7373 5f3c 4669  .  py::class_<Fi
-0001c3c0: 6c65 5772 6974 6572 2c20 786d 6c5f 7772  leWriter, xml_wr
-0001c3d0: 6974 6572 3e28 6d2c 2022 4669 6c65 5772  iter>(m, "FileWr
-0001c3e0: 6974 6572 222c 2052 2264 6f63 280a 2020  iter", R"doc(.  
-0001c3f0: 2020 2020 2870 7567 6978 6d6c 2d70 7974      (pugixml-pyt
-0001c400: 686f 6e20 6f6e 6c79 2920 3a63 6c61 7373  hon only) :class
-0001c410: 3a60 584d 4c57 7269 7465 7260 2069 6d70  :`XMLWriter` imp
-0001c420: 6c65 6d65 6e74 6174 696f 6e20 666f 7220  lementation for 
-0001c430: 6120 6669 6c65 2e0a 0a20 2020 2020 2052  a file...      R
-0001c440: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
-0001c450: 204f 5345 7272 6f72 3a20 5768 656e 2061   OSError: When a
-0001c460: 2066 696c 6520 6661 696c 7320 746f 206f   file fails to o
-0001c470: 7065 6e20 6f72 2077 7269 7465 2e0a 0a20  pen or write... 
-0001c480: 2020 2020 2053 6565 2041 6c73 6f3a 0a20       See Also:. 
-0001c490: 2020 2020 2020 2020 203a 6d65 7468 3a60           :meth:`
-0001c4a0: 584d 4c44 6f63 756d 656e 742e 7361 7665  XMLDocument.save
-0001c4b0: 602c 203a 6d65 7468 3a60 584d 4c4e 6f64  `, :meth:`XMLNod
-0001c4c0: 652e 7072 696e 7460 0a0a 2020 2020 2020  e.print`..      
-0001c4d0: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
-0001c4e0: 2020 2020 3e3e 3e20 6672 6f6d 2063 6f6e      >>> from con
-0001c4f0: 7465 7874 6c69 6220 696d 706f 7274 2063  textlib import c
-0001c500: 6c6f 7369 6e67 0a20 2020 2020 2020 2020  losing.         
-0001c510: 203e 3e3e 2066 726f 6d20 7075 6769 786d   >>> from pugixm
-0001c520: 6c20 696d 706f 7274 2070 7567 690a 2020  l import pugi.  
-0001c530: 2020 2020 2020 2020 3e3e 3e20 646f 6320          >>> doc 
-0001c540: 3d20 7075 6769 2e58 4d4c 446f 6375 6d65  = pugi.XMLDocume
-0001c550: 6e74 2829 0a20 2020 2020 2020 2020 203e  nt().          >
-0001c560: 3e3e 2064 6f63 2e6c 6f61 645f 7374 7269  >> doc.load_stri
-0001c570: 6e67 2827 3c6e 6f64 653e 3c63 6869 6c64  ng('<node><child
-0001c580: 3e5c 5530 3030 3166 3330 383c 2f63 6869  >\U0001f308</chi
-0001c590: 6c64 3e3c 2f6e 6f64 653e 2729 0a20 2020  ld></node>').   
-0001c5a0: 2020 2020 2020 203e 3e3e 2077 6974 6820         >>> with 
-0001c5b0: 636c 6f73 696e 6728 7075 6769 2e46 696c  closing(pugi.Fil
-0001c5c0: 6557 7269 7465 7228 2774 7265 652e 786d  eWriter('tree.xm
-0001c5d0: 6c27 2929 2061 7320 7772 6974 6572 3a0a  l')) as writer:.
-0001c5e0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-0001c5f0: 2020 646f 632e 7361 7665 2877 7269 7465    doc.save(write
-0001c600: 7229 0a20 2020 2020 2029 646f 6322 290a  r).      )doc").
-0001c610: 2020 2020 2020 2e64 6566 2870 793a 3a69        .def(py::i
-0001c620: 6e69 743c 636f 6e73 7420 6673 3a3a 7061  nit<const fs::pa
-0001c630: 7468 2026 3e28 292c 2070 793a 3a61 7267  th &>(), py::arg
-0001c640: 2822 6669 6c65 2229 2c20 5222 646f 6328  ("file"), R"doc(
-0001c650: 0a20 2020 2020 2020 2049 6e69 7469 616c  .        Initial
-0001c660: 697a 6520 6060 4669 6c65 5772 6974 6572  ize ``FileWriter
-0001c670: 6060 2e0a 0a20 2020 2020 2020 204f 7065  ``...        Ope
-0001c680: 6e20 6120 6669 6c65 2066 6f72 2077 7269  n a file for wri
-0001c690: 7469 6e67 2061 6e64 2061 7373 6f63 6961  ting and associa
-0001c6a0: 7465 2069 7420 7769 7468 2074 6869 7320  te it with this 
-0001c6b0: 6f62 6a65 6374 2e0a 0a20 2020 2020 2020  object...       
-0001c6c0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0001c6d0: 2020 2066 696c 6520 286f 732e 5061 7468     file (os.Path
-0001c6e0: 4c69 6b65 293a 2054 6865 2070 6174 682d  Like): The path-
-0001c6f0: 6c69 6b65 206f 626a 6563 7420 6f66 2074  like object of t
-0001c700: 6865 2066 696c 6520 746f 2073 6176 6520  he file to save 
-0001c710: 7468 6520 584d 4c20 646f 6375 6d65 6e74  the XML document
-0001c720: 206f 7220 6120 7369 6e67 6c65 2073 7562   or a single sub
-0001c730: 7472 6565 2e0a 0a20 2020 2020 2020 2052  tree...        R
-0001c740: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
-0001c750: 2020 204f 5345 7272 6f72 3a20 5768 656e     OSError: When
-0001c760: 2061 2066 696c 6520 6661 696c 7320 746f   a file fails to
-0001c770: 206f 7065 6e2e 0a20 2020 2020 2020 2029   open..        )
-0001c780: 646f 6322 290a 2020 2020 2020 2e64 6566  doc").      .def
-0001c790: 2822 636c 6f73 6522 2c20 2646 696c 6557  ("close", &FileW
-0001c7a0: 7269 7465 723a 3a63 6c6f 7365 2c20 2243  riter::close, "C
-0001c7b0: 6c6f 7365 2074 6865 2061 7373 6f63 6961  lose the associa
-0001c7c0: 7465 6420 6669 6c65 2e22 293b 0a0a 2020  ted file.");..  
-0001c7d0: 2f2f 0a20 202f 2f20 5072 696e 7457 7269  //.  // PrintWri
-0001c7e0: 7465 720a 2020 2f2f 0a20 2073 7472 7563  ter.  //.  struc
-0001c7f0: 7420 5072 696e 7457 7269 7465 7220 3a20  t PrintWriter : 
-0001c800: 7075 626c 6963 2078 6d6c 5f77 7269 7465  public xml_write
-0001c810: 7220 7b0a 2020 2020 766f 6964 2077 7269  r {.    void wri
-0001c820: 7465 2863 6f6e 7374 2076 6f69 6420 2a64  te(const void *d
-0001c830: 6174 612c 2073 697a 655f 7420 7369 7a65  ata, size_t size
-0001c840: 2920 6f76 6572 7269 6465 207b 0a20 2020  ) override {.   
-0001c850: 2020 2061 7574 6f20 6820 3d20 5079 556e     auto h = PyUn
-0001c860: 6963 6f64 655f 4672 6f6d 5374 7269 6e67  icode_FromString
-0001c870: 416e 6453 697a 6528 7374 6174 6963 5f63  AndSize(static_c
-0001c880: 6173 743c 636f 6e73 7420 6368 6172 202a  ast<const char *
-0001c890: 3e28 6461 7461 292c 2073 697a 6529 3b0a  >(data), size);.
-0001c8a0: 2020 2020 2020 6966 2028 6820 3d3d 206e        if (h == n
-0001c8b0: 756c 6c70 7472 2920 7b0a 2020 2020 2020  ullptr) {.      
-0001c8c0: 2020 7468 726f 7720 7079 3a3a 6572 726f    throw py::erro
-0001c8d0: 725f 616c 7265 6164 795f 7365 7428 293b  r_already_set();
-0001c8e0: 0a20 2020 2020 207d 0a20 2020 2020 2070  .      }.      p
-0001c8f0: 793a 3a70 7269 6e74 2870 793a 3a73 7472  y::print(py::str
-0001c900: 2868 292c 2070 793a 3a61 7267 2822 656e  (h), py::arg("en
-0001c910: 6422 2920 3d20 2222 293b 0a20 2020 207d  d") = "");.    }
-0001c920: 0a20 207d 3b0a 0a20 2070 793a 3a63 6c61  .  };..  py::cla
-0001c930: 7373 5f3c 5072 696e 7457 7269 7465 722c  ss_<PrintWriter,
-0001c940: 2078 6d6c 5f77 7269 7465 723e 286d 2c20   xml_writer>(m, 
-0001c950: 2250 7269 6e74 5772 6974 6572 222c 2052  "PrintWriter", R
-0001c960: 2264 6f63 280a 2020 2020 2020 2870 7567  "doc(.      (pug
-0001c970: 6978 6d6c 2d70 7974 686f 6e20 6f6e 6c79  ixml-python only
-0001c980: 2920 3a63 6c61 7373 3a60 584d 4c57 7269  ) :class:`XMLWri
-0001c990: 7465 7260 2069 6d70 6c65 6d65 6e74 6174  ter` implementat
-0001c9a0: 696f 6e20 666f 7220 3a6f 626a 3a60 7379  ion for :obj:`sy
-0001c9b0: 732e 7374 646f 7574 602e 0a0a 2020 2020  s.stdout`...    
-0001c9c0: 2020 4e6f 7465 3a0a 2020 2020 2020 2020    Note:.        
-0001c9d0: 2020 6060 5072 696e 7457 7269 7465 7260    ``PrintWriter`
-0001c9e0: 6020 776f 726b 7320 6f6e 6c79 2077 6974  ` works only wit
-0001c9f0: 6820 5554 462d 3820 656e 636f 6469 6e67  h UTF-8 encoding
-0001ca00: 2e0a 0a20 2020 2020 2053 6565 2041 6c73  ...      See Als
-0001ca10: 6f3a 0a20 2020 2020 2020 2020 203a 6d65  o:.          :me
-0001ca20: 7468 3a60 584d 4c4e 6f64 652e 7072 696e  th:`XMLNode.prin
-0001ca30: 7460 0a0a 2020 2020 2020 4578 616d 706c  t`..      Exampl
-0001ca40: 6573 3a0a 2020 2020 2020 2020 2020 3e3e  es:.          >>
-0001ca50: 3e20 6672 6f6d 2070 7567 6978 6d6c 2069  > from pugixml i
-0001ca60: 6d70 6f72 7420 7075 6769 0a20 2020 2020  mport pugi.     
-0001ca70: 2020 2020 203e 3e3e 2064 6f63 203d 2070       >>> doc = p
-0001ca80: 7567 692e 584d 4c44 6f63 756d 656e 7428  ugi.XMLDocument(
-0001ca90: 290a 2020 2020 2020 2020 2020 3e3e 3e20  ).          >>> 
-0001caa0: 646f 632e 6170 7065 6e64 5f63 6869 6c64  doc.append_child
-0001cab0: 2827 6e6f 6465 2729 0a20 2020 2020 2020  ('node').       
-0001cac0: 2020 203e 3e3e 2064 6f63 2e63 6869 6c64     >>> doc.child
-0001cad0: 2827 6e6f 6465 2729 2e61 7070 656e 645f  ('node').append_
-0001cae0: 6368 696c 6428 2763 6869 6c64 2729 0a20  child('child'). 
-0001caf0: 2020 2020 2020 2020 203e 3e3e 2064 6f63           >>> doc
-0001cb00: 2e70 7269 6e74 2870 7567 692e 5072 696e  .print(pugi.Prin
-0001cb10: 7457 7269 7465 7228 292c 2069 6e64 656e  tWriter(), inden
-0001cb20: 743d 2720 2729 0a20 2020 2020 2020 2020  t=' ').         
-0001cb30: 203c 6e6f 6465 3e0a 2020 2020 2020 2020   <node>.        
-0001cb40: 2020 203c 6368 696c 6420 2f3e 0a20 2020     <child />.   
-0001cb50: 2020 2020 2020 203c 2f6e 6f64 653e 0a20         </node>. 
-0001cb60: 2020 2020 2029 646f 6322 290a 2020 2020       )doc").    
-0001cb70: 2020 2e64 6566 2870 793a 3a69 6e69 743c    .def(py::init<
-0001cb80: 3e28 292c 2022 496e 6974 6961 6c69 7a65  >(), "Initialize
-0001cb90: 2060 6050 7269 6e74 5772 6974 6572 6060   ``PrintWriter``
-0001cba0: 2e22 293b 0a0a 2020 2f2f 0a20 202f 2f20  .");..  //.  // 
-0001cbb0: 5374 7269 6e67 5772 6974 6572 0a20 202f  StringWriter.  /
-0001cbc0: 2f0a 2020 7374 7275 6374 2053 7472 696e  /.  struct Strin
-0001cbd0: 6757 7269 7465 7220 3a20 7075 626c 6963  gWriter : public
-0001cbe0: 2078 6d6c 5f77 7269 7465 7220 7b0a 2020   xml_writer {.  
-0001cbf0: 2020 7374 643a 3a73 7472 696e 6720 636f    std::string co
-0001cc00: 6e74 656e 7473 3b0a 2020 2020 766f 6964  ntents;.    void
-0001cc10: 2077 7269 7465 2863 6f6e 7374 2076 6f69   write(const voi
-0001cc20: 6420 2a64 6174 612c 2073 697a 655f 7420  d *data, size_t 
-0001cc30: 7369 7a65 2920 6f76 6572 7269 6465 207b  size) override {
-0001cc40: 2063 6f6e 7465 6e74 732e 6170 7065 6e64   contents.append
-0001cc50: 2873 7461 7469 635f 6361 7374 3c63 6f6e  (static_cast<con
-0001cc60: 7374 2063 6861 7220 2a3e 2864 6174 6129  st char *>(data)
-0001cc70: 2c20 7369 7a65 293b 207d 0a20 207d 3b0a  , size); }.  };.
-0001cc80: 0a20 2070 793a 3a63 6c61 7373 5f3c 5374  .  py::class_<St
-0001cc90: 7269 6e67 5772 6974 6572 2c20 786d 6c5f  ringWriter, xml_
-0001cca0: 7772 6974 6572 3e28 6d2c 2022 5374 7269  writer>(m, "Stri
-0001ccb0: 6e67 5772 6974 6572 222c 2052 2264 6f63  ngWriter", R"doc
-0001ccc0: 280a 2020 2020 2020 2870 7567 6978 6d6c  (.      (pugixml
-0001ccd0: 2d70 7974 686f 6e20 6f6e 6c79 2920 3a63  -python only) :c
-0001cce0: 6c61 7373 3a60 584d 4c57 7269 7465 7260  lass:`XMLWriter`
-0001ccf0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-0001cd00: 666f 7220 7374 7269 6e67 2e0a 0a20 2020  for string...   
-0001cd10: 2020 2053 6565 2041 6c73 6f3a 0a20 2020     See Also:.   
-0001cd20: 2020 2020 2020 203a 6d65 7468 3a60 584d         :meth:`XM
-0001cd30: 4c4e 6f64 652e 7072 696e 7460 0a0a 2020  LNode.print`..  
-0001cd40: 2020 2020 4578 616d 706c 6573 3a0a 2020      Examples:.  
-0001cd50: 2020 2020 2020 2020 3e3e 3e20 6672 6f6d          >>> from
-0001cd60: 2070 7567 6978 6d6c 2069 6d70 6f72 7420   pugixml import 
-0001cd70: 7075 6769 0a20 2020 2020 2020 2020 203e  pugi.          >
-0001cd80: 3e3e 2064 6f63 203d 2070 7567 692e 584d  >> doc = pugi.XM
-0001cd90: 4c44 6f63 756d 656e 7428 290a 2020 2020  LDocument().    
-0001cda0: 2020 2020 2020 3e3e 3e20 646f 632e 6170        >>> doc.ap
-0001cdb0: 7065 6e64 5f63 6869 6c64 2827 6e6f 6465  pend_child('node
-0001cdc0: 2729 0a20 2020 2020 2020 2020 203e 3e3e  ').          >>>
-0001cdd0: 2077 7269 7465 7220 3d20 7075 6769 2e53   writer = pugi.S
-0001cde0: 7472 696e 6757 7269 7465 7228 290a 2020  tringWriter().  
-0001cdf0: 2020 2020 2020 2020 3e3e 3e20 646f 632e          >>> doc.
-0001ce00: 7072 696e 7428 7772 6974 6572 2c20 666c  print(writer, fl
-0001ce10: 6167 733d 7075 6769 2e46 4f52 4d41 545f  ags=pugi.FORMAT_
-0001ce20: 5241 5729 0a20 2020 2020 2020 2020 203e  RAW).          >
-0001ce30: 3e3e 2077 7269 7465 722e 6765 7476 616c  >> writer.getval
-0001ce40: 7565 2829 0a20 2020 2020 2020 2020 2027  ue().          '
-0001ce50: 3c6e 6f64 652f 3e27 0a20 2020 2020 2020  <node/>'.       
-0001ce60: 2020 203e 3e3e 2077 7269 7465 7220 3d20     >>> writer = 
-0001ce70: 7075 6769 2e53 7472 696e 6757 7269 7465  pugi.StringWrite
-0001ce80: 7228 290a 2020 2020 2020 2020 2020 3e3e  r().          >>
-0001ce90: 3e20 646f 632e 7072 696e 7428 7772 6974  > doc.print(writ
-0001cea0: 6572 2c20 666c 6167 733d 7075 6769 2e46  er, flags=pugi.F
-0001ceb0: 4f52 4d41 545f 5241 572c 2065 6e63 6f64  ORMAT_RAW, encod
-0001cec0: 696e 673d 7075 6769 2e45 4e43 4f44 494e  ing=pugi.ENCODIN
-0001ced0: 475f 5554 4633 325f 4c45 290a 2020 2020  G_UTF32_LE).    
-0001cee0: 2020 2020 2020 3e3e 3e20 7772 6974 6572        >>> writer
-0001cef0: 2e67 6574 7661 6c75 6528 290a 2020 2020  .getvalue().    
-0001cf00: 2020 2020 2020 273c 5c78 3030 5c78 3030        '<\x00\x00
-0001cf10: 5c78 3030 6e5c 7830 305c 7830 305c 7830  \x00n\x00\x00\x0
-0001cf20: 306f 5c78 3030 5c78 3030 5c78 3030 645c  0o\x00\x00\x00d\
-0001cf30: 7830 305c 7830 305c 7830 3065 5c78 3030  x00\x00\x00e\x00
-0001cf40: 5c78 3030 5c78 3030 2f5c 7830 305c 7830  \x00\x00/\x00\x0
-0001cf50: 305c 7830 303e 5c78 3030 5c78 3030 5c78  0\x00>\x00\x00\x
-0001cf60: 3030 270a 2020 2020 2020 2020 2020 3e3e  00'.          >>
-0001cf70: 3e20 7772 6974 6572 2e67 6574 7661 6c75  > writer.getvalu
-0001cf80: 6528 2775 7466 2d33 326c 6527 290a 2020  e('utf-32le').  
-0001cf90: 2020 2020 2020 2020 273c 6e6f 6465 2f3e          '<node/>
-0001cfa0: 270a 2020 2020 2020 2964 6f63 2229 0a20  '.      )doc"). 
-0001cfb0: 2020 2020 202e 6465 6628 7079 3a3a 696e       .def(py::in
-0001cfc0: 6974 3c3e 2829 2c20 2249 6e69 7469 616c  it<>(), "Initial
-0001cfd0: 697a 6520 6060 5374 7269 6e67 5772 6974  ize ``StringWrit
-0001cfe0: 6572 6060 2e22 290a 2020 2020 2020 2e64  er``.").      .d
-0001cff0: 6566 280a 2020 2020 2020 2020 2020 225f  ef(.          "_
-0001d000: 5f6c 656e 5f5f 222c 205b 5d28 636f 6e73  _len__", [](cons
-0001d010: 7420 5374 7269 6e67 5772 6974 6572 2026  t StringWriter &
-0001d020: 7365 6c66 2920 7b20 7265 7475 726e 2073  self) { return s
-0001d030: 656c 662e 636f 6e74 656e 7473 2e73 697a  elf.contents.siz
-0001d040: 6528 293b 207d 2c20 5222 646f 6328 0a20  e(); }, R"doc(. 
-0001d050: 2020 2020 2020 2020 2020 2052 6574 7572             Retur
-0001d060: 6e20 7468 6520 636f 6e74 656e 7473 2073  n the contents s
-0001d070: 697a 6520 696e 2062 7974 6573 2e0a 0a20  ize in bytes... 
-0001d080: 2020 2020 2020 2020 2020 2052 6574 7572             Retur
-0001d090: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0001d0a0: 2020 2020 696e 743a 2054 6865 2063 6f6e      int: The con
-0001d0b0: 7465 6e74 7320 7369 7a65 2069 6e20 6279  tents size in by
-0001d0c0: 7465 732e 0a20 2020 2020 2020 2020 2020  tes..           
-0001d0d0: 2029 646f 6322 290a 2020 2020 2020 2e64   )doc").      .d
-0001d0e0: 6566 280a 2020 2020 2020 2020 2020 2267  ef(.          "g
-0001d0f0: 6574 7661 6c75 6522 2c0a 2020 2020 2020  etvalue",.      
-0001d100: 2020 2020 5b5d 2863 6f6e 7374 2053 7472      [](const Str
-0001d110: 696e 6757 7269 7465 7220 2673 656c 662c  ingWriter &self,
-0001d120: 2063 6f6e 7374 2063 6861 7220 2a65 6e63   const char *enc
-0001d130: 6f64 696e 672c 2063 6f6e 7374 2063 6861  oding, const cha
-0001d140: 7220 2a65 7272 6f72 7329 207b 0a20 2020  r *errors) {.   
-0001d150: 2020 2020 2020 2020 2061 7574 6f20 6275           auto bu
-0001d160: 6620 3d20 7079 3a3a 6279 7465 7328 7365  f = py::bytes(se
-0001d170: 6c66 2e63 6f6e 7465 6e74 7329 3b0a 2020  lf.contents);.  
-0001d180: 2020 2020 2020 2020 2020 6175 746f 2068            auto h
-0001d190: 203d 2050 7943 6f64 6563 5f44 6563 6f64   = PyCodec_Decod
-0001d1a0: 6528 6275 662e 7074 7228 292c 2065 6e63  e(buf.ptr(), enc
-0001d1b0: 6f64 696e 672c 2065 7272 6f72 7329 3b0a  oding, errors);.
-0001d1c0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-0001d1d0: 6820 3d3d 206e 756c 6c70 7472 2920 7b0a  h == nullptr) {.
-0001d1e0: 2020 2020 2020 2020 2020 2020 2020 7468                th
-0001d1f0: 726f 7720 7079 3a3a 6572 726f 725f 616c  row py::error_al
-0001d200: 7265 6164 795f 7365 7428 293b 0a20 2020  ready_set();.   
-0001d210: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-0001d220: 2020 2020 2020 2072 6574 7572 6e20 7079         return py
-0001d230: 3a3a 7374 7228 6829 3b0a 2020 2020 2020  ::str(h);.      
-0001d240: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-0001d250: 2070 793a 3a61 7267 2822 656e 636f 6469   py::arg("encodi
-0001d260: 6e67 2229 2e6e 6f6e 6528 6661 6c73 6529  ng").none(false)
-0001d270: 203d 2022 7574 662d 3822 2c20 7079 3a3a   = "utf-8", py::
-0001d280: 6172 6728 2265 7272 6f72 7322 2920 3d20  arg("errors") = 
-0001d290: 2273 7472 6963 7422 2c0a 2020 2020 2020  "strict",.      
-0001d2a0: 2020 2020 5222 646f 6328 0a20 2020 2020      R"doc(.     
-0001d2b0: 2020 2020 2052 6574 7572 6e20 6120 3a6f       Return a :o
-0001d2c0: 626a 3a60 7374 7260 2063 6f6e 7461 696e  bj:`str` contain
-0001d2d0: 696e 6720 7468 6520 656e 7469 7265 2063  ing the entire c
-0001d2e0: 6f6e 7465 6e74 7320 6f66 2074 6865 2062  ontents of the b
-0001d2f0: 7566 6665 722e 0a0a 2020 2020 2020 2020  uffer...        
-0001d300: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0001d310: 2020 2020 2020 656e 636f 6469 6e67 2028        encoding (
-0001d320: 7374 7229 3a20 5468 6520 636f 6465 6320  str): The codec 
-0001d330: 7265 6769 7374 6572 6564 2066 6f72 2065  registered for e
-0001d340: 6e63 6f64 696e 6720 746f 2064 6563 6f64  ncoding to decod
-0001d350: 6520 7468 6520 6275 6666 6572 2e0a 2020  e the buffer..  
-0001d360: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-0001d370: 7273 2028 7374 7229 3a20 5468 6520 6465  rs (str): The de
-0001d380: 7369 7265 6420 6572 726f 7220 6861 6e64  sired error hand
-0001d390: 6c69 6e67 2073 6368 656d 652e 2053 6565  ling scheme. See
-0001d3a0: 203a 6675 6e63 3a60 636f 6465 6373 2e64   :func:`codecs.d
-0001d3b0: 6563 6f64 6560 2066 6f72 2064 6574 6169  ecode` for detai
-0001d3c0: 6c73 2e0a 0a20 2020 2020 2020 2020 2052  ls...          R
-0001d3d0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0001d3e0: 2020 2020 2020 7374 723a 2054 6865 2065        str: The e
-0001d3f0: 6e74 6972 6520 636f 6e74 656e 7473 206f  ntire contents o
-0001d400: 6620 7468 6520 6275 6666 6572 2e0a 2020  f the buffer..  
-0001d410: 2020 2020 2020 2020 2964 6f63 2229 3b0a          )doc");.
-0001d420: 0a20 202f 2f0a 2020 2f2f 2070 7567 6978  .  //.  // pugix
-0001d430: 6d6c 2e70 7567 692e 6c69 6d69 7473 2073  ml.pugi.limits s
-0001d440: 7562 6d6f 6475 6c65 0a20 202f 2f0a 2020  ubmodule.  //.  
-0001d450: 6175 746f 206d 3220 3d20 6d2e 6465 665f  auto m2 = m.def_
-0001d460: 7375 626d 6f64 756c 6528 226c 696d 6974  submodule("limit
-0001d470: 7322 293b 0a0a 2020 6d32 2e64 6f63 2829  s");..  m2.doc()
-0001d480: 203d 2022 4d61 7869 6d75 6d20 616e 6420   = "Maximum and 
-0001d490: 6d69 6e69 6d75 6d20 6669 6e69 7465 2076  minimum finite v
-0001d4a0: 616c 7565 732e 223b 0a0a 2020 6d32 2e61  alues.";..  m2.a
-0001d4b0: 7474 7228 2244 424c 5f4d 4158 2229 203d  ttr("DBL_MAX") =
-0001d4c0: 2073 7464 3a3a 6e75 6d65 7269 635f 6c69   std::numeric_li
-0001d4d0: 6d69 7473 3c64 6f75 626c 653e 3a3a 6d61  mits<double>::ma
-0001d4e0: 7828 293b 0a20 206d 322e 6174 7472 2822  x();.  m2.attr("
-0001d4f0: 4442 4c5f 4d49 4e22 2920 3d20 7374 643a  DBL_MIN") = std:
-0001d500: 3a6e 756d 6572 6963 5f6c 696d 6974 733c  :numeric_limits<
-0001d510: 646f 7562 6c65 3e3a 3a6d 696e 2829 3b0a  double>::min();.
-0001d520: 2020 6d32 2e61 7474 7228 2246 4c54 5f4d    m2.attr("FLT_M
-0001d530: 4158 2229 203d 2073 7464 3a3a 6e75 6d65  AX") = std::nume
-0001d540: 7269 635f 6c69 6d69 7473 3c66 6c6f 6174  ric_limits<float
-0001d550: 3e3a 3a6d 6178 2829 3b0a 2020 6d32 2e61  >::max();.  m2.a
-0001d560: 7474 7228 2246 4c54 5f4d 494e 2229 203d  ttr("FLT_MIN") =
-0001d570: 2073 7464 3a3a 6e75 6d65 7269 635f 6c69   std::numeric_li
-0001d580: 6d69 7473 3c66 6c6f 6174 3e3a 3a6d 696e  mits<float>::min
-0001d590: 2829 3b0a 2020 6d32 2e61 7474 7228 2249  ();.  m2.attr("I
-0001d5a0: 4e54 5f4d 4158 2229 203d 2073 7464 3a3a  NT_MAX") = std::
-0001d5b0: 6e75 6d65 7269 635f 6c69 6d69 7473 3c69  numeric_limits<i
-0001d5c0: 6e74 3e3a 3a6d 6178 2829 3b0a 2020 6d32  nt>::max();.  m2
-0001d5d0: 2e61 7474 7228 2249 4e54 5f4d 494e 2229  .attr("INT_MIN")
-0001d5e0: 203d 2073 7464 3a3a 6e75 6d65 7269 635f   = std::numeric_
-0001d5f0: 6c69 6d69 7473 3c69 6e74 3e3a 3a6d 696e  limits<int>::min
-0001d600: 2829 3b0a 2020 6d32 2e61 7474 7228 224c  ();.  m2.attr("L
-0001d610: 4c4f 4e47 5f4d 4158 2229 203d 2073 7464  LONG_MAX") = std
-0001d620: 3a3a 6e75 6d65 7269 635f 6c69 6d69 7473  ::numeric_limits
-0001d630: 3c6c 6f6e 6720 6c6f 6e67 3e3a 3a6d 6178  <long long>::max
-0001d640: 2829 3b0a 2020 6d32 2e61 7474 7228 224c  ();.  m2.attr("L
-0001d650: 4c4f 4e47 5f4d 494e 2229 203d 2073 7464  LONG_MIN") = std
-0001d660: 3a3a 6e75 6d65 7269 635f 6c69 6d69 7473  ::numeric_limits
-0001d670: 3c6c 6f6e 6720 6c6f 6e67 3e3a 3a6d 696e  <long long>::min
-0001d680: 2829 3b0a 2020 6d32 2e61 7474 7228 2255  ();.  m2.attr("U
-0001d690: 494e 545f 4d41 5822 2920 3d20 7374 643a  INT_MAX") = std:
-0001d6a0: 3a6e 756d 6572 6963 5f6c 696d 6974 733c  :numeric_limits<
-0001d6b0: 756e 7369 676e 6564 2069 6e74 3e3a 3a6d  unsigned int>::m
-0001d6c0: 6178 2829 3b0a 2020 6d32 2e61 7474 7228  ax();.  m2.attr(
-0001d6d0: 2255 4c4c 4f4e 475f 4d41 5822 2920 3d20  "ULLONG_MAX") = 
-0001d6e0: 7374 643a 3a6e 756d 6572 6963 5f6c 696d  std::numeric_lim
-0001d6f0: 6974 733c 756e 7369 676e 6564 206c 6f6e  its<unsigned lon
-0001d700: 6720 6c6f 6e67 3e3a 3a6d 6178 2829 3b0a  g long>::max();.
-0001d710: 7d0a                                     }.
+0001bfa0: 202e 6465 6628 2267 6574 7661 6c75 6522   .def("getvalue"
+0001bfb0: 2c20 5b5d 2863 6f6e 7374 2042 7974 6573  , [](const Bytes
+0001bfc0: 5772 6974 6572 2026 7365 6c66 2920 7b20  Writer &self) { 
+0001bfd0: 7265 7475 726e 2070 793a 3a62 7974 6573  return py::bytes
+0001bfe0: 2873 656c 662e 636f 6e74 656e 7473 293b  (self.contents);
+0001bff0: 207d 2c20 5222 646f 6328 0a20 2020 2020   }, R"doc(.     
+0001c000: 2020 2020 2052 6574 7572 6e20 7468 6520       Return the 
+0001c010: 656e 7469 7265 2063 6f6e 7465 6e74 7320  entire contents 
+0001c020: 6f66 2074 6865 2062 7566 6665 722e 0a0a  of the buffer...
+0001c030: 2020 2020 2020 2020 2020 5265 7475 726e            Return
+0001c040: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0001c050: 2062 7974 6573 3a20 5468 6520 656e 7469   bytes: The enti
+0001c060: 7265 2063 6f6e 7465 6e74 7320 6f66 2074  re contents of t
+0001c070: 6865 2062 7566 6665 722e 0a20 2020 2020  he buffer..     
+0001c080: 2020 2020 2029 646f 6322 293b 0a0a 2020       )doc");..  
+0001c090: 2f2f 0a20 202f 2f20 4669 6c65 5772 6974  //.  // FileWrit
+0001c0a0: 6572 0a20 202f 2f0a 2020 7374 7275 6374  er.  //.  struct
+0001c0b0: 2046 696c 6557 7269 7465 7220 3a20 7075   FileWriter : pu
+0001c0c0: 626c 6963 2078 6d6c 5f77 7269 7465 7220  blic xml_writer 
+0001c0d0: 7b0a 2020 2020 7374 643a 3a6f 6673 7472  {.    std::ofstr
+0001c0e0: 6561 6d20 6669 6c65 3b0a 2020 2020 4669  eam file;.    Fi
+0001c0f0: 6c65 5772 6974 6572 2863 6f6e 7374 2066  leWriter(const f
+0001c100: 733a 3a70 6174 6820 2670 6174 6829 207b  s::path &path) {
+0001c110: 0a20 2020 2020 2074 7279 207b 0a20 2020  .      try {.   
+0001c120: 2020 2020 2066 696c 652e 6f70 656e 2870       file.open(p
+0001c130: 6174 682c 2073 7464 3a3a 696f 735f 6261  ath, std::ios_ba
+0001c140: 7365 3a3a 6f75 7420 7c20 7374 643a 3a69  se::out | std::i
+0001c150: 6f73 5f62 6173 653a 3a62 696e 6172 7929  os_base::binary)
+0001c160: 3b0a 2020 2020 2020 2020 6669 6c65 2e65  ;.        file.e
+0001c170: 7863 6570 7469 6f6e 7328 7374 643a 3a69  xceptions(std::i
+0001c180: 6f73 5f62 6173 653a 3a66 6169 6c62 6974  os_base::failbit
+0001c190: 207c 2073 7464 3a3a 696f 735f 6261 7365   | std::ios_base
+0001c1a0: 3a3a 6261 6462 6974 293b 0a20 2020 2020  ::badbit);.     
+0001c1b0: 207d 2063 6174 6368 2028 636f 6e73 7420   } catch (const 
+0001c1c0: 7374 643a 3a65 7863 6570 7469 6f6e 2026  std::exception &
+0001c1d0: 6529 207b 0a20 2020 2020 2020 2050 7945  e) {.        PyE
+0001c1e0: 7272 5f53 6574 5374 7269 6e67 2850 7945  rr_SetString(PyE
+0001c1f0: 7863 5f4f 5345 7272 6f72 2c20 652e 7768  xc_OSError, e.wh
+0001c200: 6174 2829 293b 0a20 2020 2020 2020 2074  at());.        t
+0001c210: 6872 6f77 2070 793a 3a65 7272 6f72 5f61  hrow py::error_a
+0001c220: 6c72 6561 6479 5f73 6574 2829 3b0a 2020  lready_set();.  
+0001c230: 2020 2020 7d0a 2020 2020 7d0a 2020 2020      }.    }.    
+0001c240: 766f 6964 2063 6c6f 7365 2829 207b 0a20  void close() {. 
+0001c250: 2020 2020 2069 6620 2866 696c 652e 6973       if (file.is
+0001c260: 5f6f 7065 6e28 2929 207b 0a20 2020 2020  _open()) {.     
+0001c270: 2020 2066 696c 652e 636c 6f73 6528 293b     file.close();
+0001c280: 0a20 2020 2020 207d 0a20 2020 207d 0a20  .      }.    }. 
+0001c290: 2020 2076 6f69 6420 7772 6974 6528 636f     void write(co
+0001c2a0: 6e73 7420 766f 6964 202a 6461 7461 2c20  nst void *data, 
+0001c2b0: 7369 7a65 5f74 2073 697a 6529 206f 7665  size_t size) ove
+0001c2c0: 7272 6964 6520 7b0a 2020 2020 2020 7472  rride {.      tr
+0001c2d0: 7920 7b0a 2020 2020 2020 2020 6669 6c65  y {.        file
+0001c2e0: 2e77 7269 7465 2873 7461 7469 635f 6361  .write(static_ca
+0001c2f0: 7374 3c63 6f6e 7374 2063 6861 7220 2a3e  st<const char *>
+0001c300: 2864 6174 6129 2c20 7369 7a65 293b 0a20  (data), size);. 
+0001c310: 2020 2020 207d 2063 6174 6368 2028 636f       } catch (co
+0001c320: 6e73 7420 7374 643a 3a65 7863 6570 7469  nst std::excepti
+0001c330: 6f6e 2026 6529 207b 0a20 2020 2020 2020  on &e) {.       
+0001c340: 2050 7945 7272 5f53 6574 5374 7269 6e67   PyErr_SetString
+0001c350: 2850 7945 7863 5f4f 5345 7272 6f72 2c20  (PyExc_OSError, 
+0001c360: 652e 7768 6174 2829 293b 0a20 2020 2020  e.what());.     
+0001c370: 2020 2074 6872 6f77 2070 793a 3a65 7272     throw py::err
+0001c380: 6f72 5f61 6c72 6561 6479 5f73 6574 2829  or_already_set()
+0001c390: 3b0a 2020 2020 2020 7d0a 2020 2020 7d0a  ;.      }.    }.
+0001c3a0: 2020 7d3b 0a0a 2020 7079 3a3a 636c 6173    };..  py::clas
+0001c3b0: 735f 3c46 696c 6557 7269 7465 722c 2078  s_<FileWriter, x
+0001c3c0: 6d6c 5f77 7269 7465 723e 286d 2c20 2246  ml_writer>(m, "F
+0001c3d0: 696c 6557 7269 7465 7222 2c20 5222 646f  ileWriter", R"do
+0001c3e0: 6328 0a20 2020 2020 2028 7075 6769 786d  c(.      (pugixm
+0001c3f0: 6c2d 7079 7468 6f6e 206f 6e6c 7929 203a  l-python only) :
+0001c400: 636c 6173 733a 6058 4d4c 5772 6974 6572  class:`XMLWriter
+0001c410: 6020 696d 706c 656d 656e 7461 7469 6f6e  ` implementation
+0001c420: 2066 6f72 2061 2066 696c 652e 0a0a 2020   for a file...  
+0001c430: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+0001c440: 2020 2020 2020 4f53 4572 726f 723a 2057        OSError: W
+0001c450: 6865 6e20 6120 6669 6c65 2066 6169 6c73  hen a file fails
+0001c460: 2074 6f20 6f70 656e 206f 7220 7772 6974   to open or writ
+0001c470: 652e 0a0a 2020 2020 2020 5365 6520 416c  e...      See Al
+0001c480: 736f 3a0a 2020 2020 2020 2020 2020 3a6d  so:.          :m
+0001c490: 6574 683a 6058 4d4c 446f 6375 6d65 6e74  eth:`XMLDocument
+0001c4a0: 2e73 6176 6560 2c20 3a6d 6574 683a 6058  .save`, :meth:`X
+0001c4b0: 4d4c 4e6f 6465 2e70 7269 6e74 600a 0a20  MLNode.print`.. 
+0001c4c0: 2020 2020 2045 7861 6d70 6c65 733a 0a20       Examples:. 
+0001c4d0: 2020 2020 2020 2020 203e 3e3e 2066 726f           >>> fro
+0001c4e0: 6d20 636f 6e74 6578 746c 6962 2069 6d70  m contextlib imp
+0001c4f0: 6f72 7420 636c 6f73 696e 670a 2020 2020  ort closing.    
+0001c500: 2020 2020 2020 3e3e 3e20 6672 6f6d 2070        >>> from p
+0001c510: 7567 6978 6d6c 2069 6d70 6f72 7420 7075  ugixml import pu
+0001c520: 6769 0a20 2020 2020 2020 2020 203e 3e3e  gi.          >>>
+0001c530: 2064 6f63 203d 2070 7567 692e 584d 4c44   doc = pugi.XMLD
+0001c540: 6f63 756d 656e 7428 290a 2020 2020 2020  ocument().      
+0001c550: 2020 2020 3e3e 3e20 646f 632e 6c6f 6164      >>> doc.load
+0001c560: 5f73 7472 696e 6728 273c 6e6f 6465 3e3c  _string('<node><
+0001c570: 6368 696c 643e 5c55 3030 3031 6633 3038  child>\U0001f308
+0001c580: 3c2f 6368 696c 643e 3c2f 6e6f 6465 3e27  </child></node>'
+0001c590: 290a 2020 2020 2020 2020 2020 3e3e 3e20  ).          >>> 
+0001c5a0: 7769 7468 2063 6c6f 7369 6e67 2870 7567  with closing(pug
+0001c5b0: 692e 4669 6c65 5772 6974 6572 2827 7472  i.FileWriter('tr
+0001c5c0: 6565 2e78 6d6c 2729 2920 6173 2077 7269  ee.xml')) as wri
+0001c5d0: 7465 723a 0a20 2020 2020 2020 2020 202e  ter:.          .
+0001c5e0: 2e2e 2020 2020 2064 6f63 2e73 6176 6528  ..     doc.save(
+0001c5f0: 7772 6974 6572 290a 2020 2020 2020 2964  writer).      )d
+0001c600: 6f63 2229 0a20 2020 2020 202e 6465 6628  oc").      .def(
+0001c610: 7079 3a3a 696e 6974 3c63 6f6e 7374 2066  py::init<const f
+0001c620: 733a 3a70 6174 6820 263e 2829 2c20 7079  s::path &>(), py
+0001c630: 3a3a 6172 6728 2266 696c 6522 292c 2052  ::arg("file"), R
+0001c640: 2264 6f63 280a 2020 2020 2020 2020 496e  "doc(.        In
+0001c650: 6974 6961 6c69 7a65 2060 6046 696c 6557  itialize ``FileW
+0001c660: 7269 7465 7260 602e 0a0a 2020 2020 2020  riter``...      
+0001c670: 2020 4f70 656e 2061 2066 696c 6520 666f    Open a file fo
+0001c680: 7220 7772 6974 696e 6720 616e 6420 6173  r writing and as
+0001c690: 736f 6369 6174 6520 6974 2077 6974 6820  sociate it with 
+0001c6a0: 7468 6973 206f 626a 6563 742e 0a0a 2020  this object...  
+0001c6b0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+0001c6c0: 2020 2020 2020 2020 6669 6c65 2028 6f73          file (os
+0001c6d0: 2e50 6174 684c 696b 6529 3a20 5468 6520  .PathLike): The 
+0001c6e0: 7061 7468 2d6c 696b 6520 6f62 6a65 6374  path-like object
+0001c6f0: 206f 6620 7468 6520 6669 6c65 2074 6f20   of the file to 
+0001c700: 7361 7665 2074 6865 2058 4d4c 2064 6f63  save the XML doc
+0001c710: 756d 656e 7420 6f72 2061 2073 696e 676c  ument or a singl
+0001c720: 6520 7375 6274 7265 652e 0a0a 2020 2020  e subtree...    
+0001c730: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+0001c740: 2020 2020 2020 2020 4f53 4572 726f 723a          OSError:
+0001c750: 2057 6865 6e20 6120 6669 6c65 2066 6169   When a file fai
+0001c760: 6c73 2074 6f20 6f70 656e 2e0a 2020 2020  ls to open..    
+0001c770: 2020 2020 2964 6f63 2229 0a20 2020 2020      )doc").     
+0001c780: 202e 6465 6628 2263 6c6f 7365 222c 2026   .def("close", &
+0001c790: 4669 6c65 5772 6974 6572 3a3a 636c 6f73  FileWriter::clos
+0001c7a0: 652c 2022 436c 6f73 6520 7468 6520 6173  e, "Close the as
+0001c7b0: 736f 6369 6174 6564 2066 696c 652e 2229  sociated file.")
+0001c7c0: 3b0a 0a20 202f 2f0a 2020 2f2f 2050 7269  ;..  //.  // Pri
+0001c7d0: 6e74 5772 6974 6572 0a20 202f 2f0a 2020  ntWriter.  //.  
+0001c7e0: 7374 7275 6374 2050 7269 6e74 5772 6974  struct PrintWrit
+0001c7f0: 6572 203a 2070 7562 6c69 6320 786d 6c5f  er : public xml_
+0001c800: 7772 6974 6572 207b 0a20 2020 2076 6f69  writer {.    voi
+0001c810: 6420 7772 6974 6528 636f 6e73 7420 766f  d write(const vo
+0001c820: 6964 202a 6461 7461 2c20 7369 7a65 5f74  id *data, size_t
+0001c830: 2073 697a 6529 206f 7665 7272 6964 6520   size) override 
+0001c840: 7b0a 2020 2020 2020 6175 746f 2068 203d  {.      auto h =
+0001c850: 2050 7955 6e69 636f 6465 5f46 726f 6d53   PyUnicode_FromS
+0001c860: 7472 696e 6741 6e64 5369 7a65 2873 7461  tringAndSize(sta
+0001c870: 7469 635f 6361 7374 3c63 6f6e 7374 2063  tic_cast<const c
+0001c880: 6861 7220 2a3e 2864 6174 6129 2c20 7369  har *>(data), si
+0001c890: 7a65 293b 0a20 2020 2020 2069 6620 2868  ze);.      if (h
+0001c8a0: 203d 3d20 6e75 6c6c 7074 7229 207b 0a20   == nullptr) {. 
+0001c8b0: 2020 2020 2020 2074 6872 6f77 2070 793a         throw py:
+0001c8c0: 3a65 7272 6f72 5f61 6c72 6561 6479 5f73  :error_already_s
+0001c8d0: 6574 2829 3b0a 2020 2020 2020 7d0a 2020  et();.      }.  
+0001c8e0: 2020 2020 7079 3a3a 7072 696e 7428 7079      py::print(py
+0001c8f0: 3a3a 7374 7228 6829 2c20 7079 3a3a 6172  ::str(h), py::ar
+0001c900: 6728 2265 6e64 2229 203d 2022 2229 3b0a  g("end") = "");.
+0001c910: 2020 2020 7d0a 2020 7d3b 0a0a 2020 7079      }.  };..  py
+0001c920: 3a3a 636c 6173 735f 3c50 7269 6e74 5772  ::class_<PrintWr
+0001c930: 6974 6572 2c20 786d 6c5f 7772 6974 6572  iter, xml_writer
+0001c940: 3e28 6d2c 2022 5072 696e 7457 7269 7465  >(m, "PrintWrite
+0001c950: 7222 2c20 5222 646f 6328 0a20 2020 2020  r", R"doc(.     
+0001c960: 2028 7075 6769 786d 6c2d 7079 7468 6f6e   (pugixml-python
+0001c970: 206f 6e6c 7929 203a 636c 6173 733a 6058   only) :class:`X
+0001c980: 4d4c 5772 6974 6572 6020 696d 706c 656d  MLWriter` implem
+0001c990: 656e 7461 7469 6f6e 2066 6f72 203a 6f62  entation for :ob
+0001c9a0: 6a3a 6073 7973 2e73 7464 6f75 7460 2e0a  j:`sys.stdout`..
+0001c9b0: 0a20 2020 2020 204e 6f74 653a 0a20 2020  .      Note:.   
+0001c9c0: 2020 2020 2020 2060 6050 7269 6e74 5772         ``PrintWr
+0001c9d0: 6974 6572 6060 2077 6f72 6b73 206f 6e6c  iter`` works onl
+0001c9e0: 7920 7769 7468 2055 5446 2d38 2065 6e63  y with UTF-8 enc
+0001c9f0: 6f64 696e 672e 0a0a 2020 2020 2020 5365  oding...      Se
+0001ca00: 6520 416c 736f 3a0a 2020 2020 2020 2020  e Also:.        
+0001ca10: 2020 3a6d 6574 683a 6058 4d4c 4e6f 6465    :meth:`XMLNode
+0001ca20: 2e70 7269 6e74 600a 0a20 2020 2020 2045  .print`..      E
+0001ca30: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
+0001ca40: 2020 203e 3e3e 2066 726f 6d20 7075 6769     >>> from pugi
+0001ca50: 786d 6c20 696d 706f 7274 2070 7567 690a  xml import pugi.
+0001ca60: 2020 2020 2020 2020 2020 3e3e 3e20 646f            >>> do
+0001ca70: 6320 3d20 7075 6769 2e58 4d4c 446f 6375  c = pugi.XMLDocu
+0001ca80: 6d65 6e74 2829 0a20 2020 2020 2020 2020  ment().         
+0001ca90: 203e 3e3e 2064 6f63 2e61 7070 656e 645f   >>> doc.append_
+0001caa0: 6368 696c 6428 276e 6f64 6527 290a 2020  child('node').  
+0001cab0: 2020 2020 2020 2020 3e3e 3e20 646f 632e          >>> doc.
+0001cac0: 6368 696c 6428 276e 6f64 6527 292e 6170  child('node').ap
+0001cad0: 7065 6e64 5f63 6869 6c64 2827 6368 696c  pend_child('chil
+0001cae0: 6427 290a 2020 2020 2020 2020 2020 3e3e  d').          >>
+0001caf0: 3e20 646f 632e 7072 696e 7428 7075 6769  > doc.print(pugi
+0001cb00: 2e50 7269 6e74 5772 6974 6572 2829 2c20  .PrintWriter(), 
+0001cb10: 696e 6465 6e74 3d27 2027 290a 2020 2020  indent=' ').    
+0001cb20: 2020 2020 2020 3c6e 6f64 653e 0a20 2020        <node>.   
+0001cb30: 2020 2020 2020 2020 3c63 6869 6c64 202f          <child /
+0001cb40: 3e0a 2020 2020 2020 2020 2020 3c2f 6e6f  >.          </no
+0001cb50: 6465 3e0a 2020 2020 2020 2964 6f63 2229  de>.      )doc")
+0001cb60: 0a20 2020 2020 202e 6465 6628 7079 3a3a  .      .def(py::
+0001cb70: 696e 6974 3c3e 2829 2c20 2249 6e69 7469  init<>(), "Initi
+0001cb80: 616c 697a 6520 6060 5072 696e 7457 7269  alize ``PrintWri
+0001cb90: 7465 7260 602e 2229 3b0a 0a20 202f 2f0a  ter``.");..  //.
+0001cba0: 2020 2f2f 2053 7472 696e 6757 7269 7465    // StringWrite
+0001cbb0: 720a 2020 2f2f 0a20 2073 7472 7563 7420  r.  //.  struct 
+0001cbc0: 5374 7269 6e67 5772 6974 6572 203a 2070  StringWriter : p
+0001cbd0: 7562 6c69 6320 786d 6c5f 7772 6974 6572  ublic xml_writer
+0001cbe0: 207b 0a20 2020 2073 7464 3a3a 7374 7269   {.    std::stri
+0001cbf0: 6e67 2063 6f6e 7465 6e74 733b 0a20 2020  ng contents;.   
+0001cc00: 2076 6f69 6420 7772 6974 6528 636f 6e73   void write(cons
+0001cc10: 7420 766f 6964 202a 6461 7461 2c20 7369  t void *data, si
+0001cc20: 7a65 5f74 2073 697a 6529 206f 7665 7272  ze_t size) overr
+0001cc30: 6964 6520 7b20 636f 6e74 656e 7473 2e61  ide { contents.a
+0001cc40: 7070 656e 6428 7374 6174 6963 5f63 6173  ppend(static_cas
+0001cc50: 743c 636f 6e73 7420 6368 6172 202a 3e28  t<const char *>(
+0001cc60: 6461 7461 292c 2073 697a 6529 3b20 7d0a  data), size); }.
+0001cc70: 2020 7d3b 0a0a 2020 7079 3a3a 636c 6173    };..  py::clas
+0001cc80: 735f 3c53 7472 696e 6757 7269 7465 722c  s_<StringWriter,
+0001cc90: 2078 6d6c 5f77 7269 7465 723e 286d 2c20   xml_writer>(m, 
+0001cca0: 2253 7472 696e 6757 7269 7465 7222 2c20  "StringWriter", 
+0001ccb0: 5222 646f 6328 0a20 2020 2020 2028 7075  R"doc(.      (pu
+0001ccc0: 6769 786d 6c2d 7079 7468 6f6e 206f 6e6c  gixml-python onl
+0001ccd0: 7929 203a 636c 6173 733a 6058 4d4c 5772  y) :class:`XMLWr
+0001cce0: 6974 6572 6020 696d 706c 656d 656e 7461  iter` implementa
+0001ccf0: 7469 6f6e 2066 6f72 2073 7472 696e 672e  tion for string.
+0001cd00: 0a0a 2020 2020 2020 5365 6520 416c 736f  ..      See Also
+0001cd10: 3a0a 2020 2020 2020 2020 2020 3a6d 6574  :.          :met
+0001cd20: 683a 6058 4d4c 4e6f 6465 2e70 7269 6e74  h:`XMLNode.print
+0001cd30: 600a 0a20 2020 2020 2045 7861 6d70 6c65  `..      Example
+0001cd40: 733a 0a20 2020 2020 2020 2020 203e 3e3e  s:.          >>>
+0001cd50: 2066 726f 6d20 7075 6769 786d 6c20 696d   from pugixml im
+0001cd60: 706f 7274 2070 7567 690a 2020 2020 2020  port pugi.      
+0001cd70: 2020 2020 3e3e 3e20 646f 6320 3d20 7075      >>> doc = pu
+0001cd80: 6769 2e58 4d4c 446f 6375 6d65 6e74 2829  gi.XMLDocument()
+0001cd90: 0a20 2020 2020 2020 2020 203e 3e3e 2064  .          >>> d
+0001cda0: 6f63 2e61 7070 656e 645f 6368 696c 6428  oc.append_child(
+0001cdb0: 276e 6f64 6527 290a 2020 2020 2020 2020  'node').        
+0001cdc0: 2020 3e3e 3e20 7772 6974 6572 203d 2070    >>> writer = p
+0001cdd0: 7567 692e 5374 7269 6e67 5772 6974 6572  ugi.StringWriter
+0001cde0: 2829 0a20 2020 2020 2020 2020 203e 3e3e  ().          >>>
+0001cdf0: 2064 6f63 2e70 7269 6e74 2877 7269 7465   doc.print(write
+0001ce00: 722c 2066 6c61 6773 3d70 7567 692e 464f  r, flags=pugi.FO
+0001ce10: 524d 4154 5f52 4157 290a 2020 2020 2020  RMAT_RAW).      
+0001ce20: 2020 2020 3e3e 3e20 7772 6974 6572 2e67      >>> writer.g
+0001ce30: 6574 7661 6c75 6528 290a 2020 2020 2020  etvalue().      
+0001ce40: 2020 2020 273c 6e6f 6465 2f3e 270a 2020      '<node/>'.  
+0001ce50: 2020 2020 2020 2020 3e3e 3e20 7772 6974          >>> writ
+0001ce60: 6572 203d 2070 7567 692e 5374 7269 6e67  er = pugi.String
+0001ce70: 5772 6974 6572 2829 0a20 2020 2020 2020  Writer().       
+0001ce80: 2020 203e 3e3e 2064 6f63 2e70 7269 6e74     >>> doc.print
+0001ce90: 2877 7269 7465 722c 2066 6c61 6773 3d70  (writer, flags=p
+0001cea0: 7567 692e 464f 524d 4154 5f52 4157 2c20  ugi.FORMAT_RAW, 
+0001ceb0: 656e 636f 6469 6e67 3d70 7567 692e 454e  encoding=pugi.EN
+0001cec0: 434f 4449 4e47 5f55 5446 3332 5f4c 4529  CODING_UTF32_LE)
+0001ced0: 0a20 2020 2020 2020 2020 203e 3e3e 2077  .          >>> w
+0001cee0: 7269 7465 722e 6765 7476 616c 7565 2829  riter.getvalue()
+0001cef0: 0a20 2020 2020 2020 2020 2027 3c5c 7830  .          '<\x0
+0001cf00: 305c 7830 305c 7830 306e 5c78 3030 5c78  0\x00\x00n\x00\x
+0001cf10: 3030 5c78 3030 6f5c 7830 305c 7830 305c  00\x00o\x00\x00\
+0001cf20: 7830 3064 5c78 3030 5c78 3030 5c78 3030  x00d\x00\x00\x00
+0001cf30: 655c 7830 305c 7830 305c 7830 302f 5c78  e\x00\x00\x00/\x
+0001cf40: 3030 5c78 3030 5c78 3030 3e5c 7830 305c  00\x00\x00>\x00\
+0001cf50: 7830 305c 7830 3027 0a20 2020 2020 2020  x00\x00'.       
+0001cf60: 2020 203e 3e3e 2077 7269 7465 722e 6765     >>> writer.ge
+0001cf70: 7476 616c 7565 2827 7574 662d 3332 6c65  tvalue('utf-32le
+0001cf80: 2729 0a20 2020 2020 2020 2020 2027 3c6e  ').          '<n
+0001cf90: 6f64 652f 3e27 0a20 2020 2020 2029 646f  ode/>'.      )do
+0001cfa0: 6322 290a 2020 2020 2020 2e64 6566 2870  c").      .def(p
+0001cfb0: 793a 3a69 6e69 743c 3e28 292c 2022 496e  y::init<>(), "In
+0001cfc0: 6974 6961 6c69 7a65 2060 6053 7472 696e  itialize ``Strin
+0001cfd0: 6757 7269 7465 7260 602e 2229 0a20 2020  gWriter``.").   
+0001cfe0: 2020 202e 6465 6628 0a20 2020 2020 2020     .def(.       
+0001cff0: 2020 2022 5f5f 6c65 6e5f 5f22 2c20 5b5d     "__len__", []
+0001d000: 2863 6f6e 7374 2053 7472 696e 6757 7269  (const StringWri
+0001d010: 7465 7220 2673 656c 6629 207b 2072 6574  ter &self) { ret
+0001d020: 7572 6e20 7365 6c66 2e63 6f6e 7465 6e74  urn self.content
+0001d030: 732e 7369 7a65 2829 3b20 7d2c 2052 2264  s.size(); }, R"d
+0001d040: 6f63 280a 2020 2020 2020 2020 2020 2020  oc(.            
+0001d050: 5265 7475 726e 2074 6865 2063 6f6e 7465  Return the conte
+0001d060: 6e74 7320 7369 7a65 2069 6e20 6279 7465  nts size in byte
+0001d070: 732e 0a0a 2020 2020 2020 2020 2020 2020  s...            
+0001d080: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0001d090: 2020 2020 2020 2020 2069 6e74 3a20 5468           int: Th
+0001d0a0: 6520 636f 6e74 656e 7473 2073 697a 6520  e contents size 
+0001d0b0: 696e 2062 7974 6573 2e0a 2020 2020 2020  in bytes..      
+0001d0c0: 2020 2020 2020 2964 6f63 2229 0a20 2020        )doc").   
+0001d0d0: 2020 202e 6465 6628 0a20 2020 2020 2020     .def(.       
+0001d0e0: 2020 2022 6765 7476 616c 7565 222c 0a20     "getvalue",. 
+0001d0f0: 2020 2020 2020 2020 205b 5d28 636f 6e73           [](cons
+0001d100: 7420 5374 7269 6e67 5772 6974 6572 2026  t StringWriter &
+0001d110: 7365 6c66 2c20 636f 6e73 7420 6368 6172  self, const char
+0001d120: 202a 656e 636f 6469 6e67 2c20 636f 6e73   *encoding, cons
+0001d130: 7420 6368 6172 202a 6572 726f 7273 2920  t char *errors) 
+0001d140: 7b0a 2020 2020 2020 2020 2020 2020 6175  {.            au
+0001d150: 746f 2062 7566 203d 2070 793a 3a62 7974  to buf = py::byt
+0001d160: 6573 2873 656c 662e 636f 6e74 656e 7473  es(self.contents
+0001d170: 293b 0a20 2020 2020 2020 2020 2020 2061  );.            a
+0001d180: 7574 6f20 6820 3d20 5079 436f 6465 635f  uto h = PyCodec_
+0001d190: 4465 636f 6465 2862 7566 2e70 7472 2829  Decode(buf.ptr()
+0001d1a0: 2c20 656e 636f 6469 6e67 2c20 6572 726f  , encoding, erro
+0001d1b0: 7273 293b 0a20 2020 2020 2020 2020 2020  rs);.           
+0001d1c0: 2069 6620 2868 203d 3d20 6e75 6c6c 7074   if (h == nullpt
+0001d1d0: 7229 207b 0a20 2020 2020 2020 2020 2020  r) {.           
+0001d1e0: 2020 2074 6872 6f77 2070 793a 3a65 7272     throw py::err
+0001d1f0: 6f72 5f61 6c72 6561 6479 5f73 6574 2829  or_already_set()
+0001d200: 3b0a 2020 2020 2020 2020 2020 2020 7d0a  ;.            }.
+0001d210: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001d220: 726e 2070 793a 3a73 7472 2868 293b 0a20  rn py::str(h);. 
+0001d230: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+0001d240: 2020 2020 2020 7079 3a3a 6172 6728 2265        py::arg("e
+0001d250: 6e63 6f64 696e 6722 292e 6e6f 6e65 2866  ncoding").none(f
+0001d260: 616c 7365 2920 3d20 2275 7466 2d38 222c  alse) = "utf-8",
+0001d270: 2070 793a 3a61 7267 2822 6572 726f 7273   py::arg("errors
+0001d280: 2229 203d 2022 7374 7269 6374 222c 0a20  ") = "strict",. 
+0001d290: 2020 2020 2020 2020 2052 2264 6f63 280a           R"doc(.
+0001d2a0: 2020 2020 2020 2020 2020 5265 7475 726e            Return
+0001d2b0: 2061 203a 6f62 6a3a 6073 7472 6020 636f   a :obj:`str` co
+0001d2c0: 6e74 6169 6e69 6e67 2074 6865 2065 6e74  ntaining the ent
+0001d2d0: 6972 6520 636f 6e74 656e 7473 206f 6620  ire contents of 
+0001d2e0: 7468 6520 6275 6666 6572 2e0a 0a20 2020  the buffer...   
+0001d2f0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0001d300: 2020 2020 2020 2020 2020 2065 6e63 6f64             encod
+0001d310: 696e 6720 2873 7472 293a 2054 6865 2063  ing (str): The c
+0001d320: 6f64 6563 2072 6567 6973 7465 7265 6420  odec registered 
+0001d330: 666f 7220 656e 636f 6469 6e67 2074 6f20  for encoding to 
+0001d340: 6465 636f 6465 2074 6865 2062 7566 6665  decode the buffe
+0001d350: 722e 0a20 2020 2020 2020 2020 2020 2020  r..             
+0001d360: 2065 7272 6f72 7320 2873 7472 293a 2054   errors (str): T
+0001d370: 6865 2064 6573 6972 6564 2065 7272 6f72  he desired error
+0001d380: 2068 616e 646c 696e 6720 7363 6865 6d65   handling scheme
+0001d390: 2e20 5365 6520 3a66 756e 633a 6063 6f64  . See :func:`cod
+0001d3a0: 6563 732e 6465 636f 6465 6020 666f 7220  ecs.decode` for 
+0001d3b0: 6465 7461 696c 732e 0a0a 2020 2020 2020  details...      
+0001d3c0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0001d3d0: 2020 2020 2020 2020 2020 2073 7472 3a20             str: 
+0001d3e0: 5468 6520 656e 7469 7265 2063 6f6e 7465  The entire conte
+0001d3f0: 6e74 7320 6f66 2074 6865 2062 7566 6665  nts of the buffe
+0001d400: 722e 0a20 2020 2020 2020 2020 2029 646f  r..          )do
+0001d410: 6322 293b 0a0a 2020 2f2f 0a20 202f 2f20  c");..  //.  // 
+0001d420: 7075 6769 786d 6c2e 7075 6769 2e6c 696d  pugixml.pugi.lim
+0001d430: 6974 7320 7375 626d 6f64 756c 650a 2020  its submodule.  
+0001d440: 2f2f 0a20 2061 7574 6f20 6d32 203d 206d  //.  auto m2 = m
+0001d450: 2e64 6566 5f73 7562 6d6f 6475 6c65 2822  .def_submodule("
+0001d460: 6c69 6d69 7473 2229 3b0a 0a20 206d 322e  limits");..  m2.
+0001d470: 646f 6328 2920 3d20 224d 6178 696d 756d  doc() = "Maximum
+0001d480: 2061 6e64 206d 696e 696d 756d 2066 696e   and minimum fin
+0001d490: 6974 6520 7661 6c75 6573 2e22 3b0a 0a20  ite values.";.. 
+0001d4a0: 206d 322e 6174 7472 2822 4442 4c5f 4d41   m2.attr("DBL_MA
+0001d4b0: 5822 2920 3d20 7374 643a 3a6e 756d 6572  X") = std::numer
+0001d4c0: 6963 5f6c 696d 6974 733c 646f 7562 6c65  ic_limits<double
+0001d4d0: 3e3a 3a6d 6178 2829 3b0a 2020 6d32 2e61  >::max();.  m2.a
+0001d4e0: 7474 7228 2244 424c 5f4d 494e 2229 203d  ttr("DBL_MIN") =
+0001d4f0: 2073 7464 3a3a 6e75 6d65 7269 635f 6c69   std::numeric_li
+0001d500: 6d69 7473 3c64 6f75 626c 653e 3a3a 6d69  mits<double>::mi
+0001d510: 6e28 293b 0a20 206d 322e 6174 7472 2822  n();.  m2.attr("
+0001d520: 464c 545f 4d41 5822 2920 3d20 7374 643a  FLT_MAX") = std:
+0001d530: 3a6e 756d 6572 6963 5f6c 696d 6974 733c  :numeric_limits<
+0001d540: 666c 6f61 743e 3a3a 6d61 7828 293b 0a20  float>::max();. 
+0001d550: 206d 322e 6174 7472 2822 464c 545f 4d49   m2.attr("FLT_MI
+0001d560: 4e22 2920 3d20 7374 643a 3a6e 756d 6572  N") = std::numer
+0001d570: 6963 5f6c 696d 6974 733c 666c 6f61 743e  ic_limits<float>
+0001d580: 3a3a 6d69 6e28 293b 0a20 206d 322e 6174  ::min();.  m2.at
+0001d590: 7472 2822 494e 545f 4d41 5822 2920 3d20  tr("INT_MAX") = 
+0001d5a0: 7374 643a 3a6e 756d 6572 6963 5f6c 696d  std::numeric_lim
+0001d5b0: 6974 733c 696e 743e 3a3a 6d61 7828 293b  its<int>::max();
+0001d5c0: 0a20 206d 322e 6174 7472 2822 494e 545f  .  m2.attr("INT_
+0001d5d0: 4d49 4e22 2920 3d20 7374 643a 3a6e 756d  MIN") = std::num
+0001d5e0: 6572 6963 5f6c 696d 6974 733c 696e 743e  eric_limits<int>
+0001d5f0: 3a3a 6d69 6e28 293b 0a20 206d 322e 6174  ::min();.  m2.at
+0001d600: 7472 2822 4c4c 4f4e 475f 4d41 5822 2920  tr("LLONG_MAX") 
+0001d610: 3d20 7374 643a 3a6e 756d 6572 6963 5f6c  = std::numeric_l
+0001d620: 696d 6974 733c 6c6f 6e67 206c 6f6e 673e  imits<long long>
+0001d630: 3a3a 6d61 7828 293b 0a20 206d 322e 6174  ::max();.  m2.at
+0001d640: 7472 2822 4c4c 4f4e 475f 4d49 4e22 2920  tr("LLONG_MIN") 
+0001d650: 3d20 7374 643a 3a6e 756d 6572 6963 5f6c  = std::numeric_l
+0001d660: 696d 6974 733c 6c6f 6e67 206c 6f6e 673e  imits<long long>
+0001d670: 3a3a 6d69 6e28 293b 0a20 206d 322e 6174  ::min();.  m2.at
+0001d680: 7472 2822 5549 4e54 5f4d 4158 2229 203d  tr("UINT_MAX") =
+0001d690: 2073 7464 3a3a 6e75 6d65 7269 635f 6c69   std::numeric_li
+0001d6a0: 6d69 7473 3c75 6e73 6967 6e65 6420 696e  mits<unsigned in
+0001d6b0: 743e 3a3a 6d61 7828 293b 0a20 206d 322e  t>::max();.  m2.
+0001d6c0: 6174 7472 2822 554c 4c4f 4e47 5f4d 4158  attr("ULLONG_MAX
+0001d6d0: 2229 203d 2073 7464 3a3a 6e75 6d65 7269  ") = std::numeri
+0001d6e0: 635f 6c69 6d69 7473 3c75 6e73 6967 6e65  c_limits<unsigne
+0001d6f0: 6420 6c6f 6e67 206c 6f6e 673e 3a3a 6d61  d long long>::ma
+0001d700: 7828 293b 0a7d 0a                        x();.}.
```

### Comparing `pugixml-0.5.0/src/pugixml.egg-info/PKG-INFO` & `pugixml-0.6.0/src/pugixml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: pugixml
-Version: 0.5.0
+Version: 0.6.0
 Summary: Light-weight, simple and fast XML parser with XPath support
 Home-page: https://github.com/miute/pugixml-python
 Author: Tetsuya Miura
 Author-email: miute.dev@gmail.com
 License: MIT
 Keywords: dom,xml,xpath,xml-parser
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup :: XML
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python bindings for pugixml
 
 [![PyPI](https://img.shields.io/pypi/v/pugixml)](https://pypi.org/project/pugixml/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pugixml)](https://pypi.org/project/pugixml/)
```

### Comparing `pugixml-0.5.0/src/pugixml.egg-info/SOURCES.txt` & `pugixml-0.6.0/src/pugixml.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -64,23 +64,25 @@
 src/third_party/pybind11/include/pybind11/common.h
 src/third_party/pybind11/include/pybind11/complex.h
 src/third_party/pybind11/include/pybind11/eigen.h
 src/third_party/pybind11/include/pybind11/embed.h
 src/third_party/pybind11/include/pybind11/eval.h
 src/third_party/pybind11/include/pybind11/functional.h
 src/third_party/pybind11/include/pybind11/gil.h
+src/third_party/pybind11/include/pybind11/gil_safe_call_once.h
 src/third_party/pybind11/include/pybind11/iostream.h
 src/third_party/pybind11/include/pybind11/numpy.h
 src/third_party/pybind11/include/pybind11/operators.h
 src/third_party/pybind11/include/pybind11/options.h
 src/third_party/pybind11/include/pybind11/pybind11.h
 src/third_party/pybind11/include/pybind11/pytypes.h
 src/third_party/pybind11/include/pybind11/stl.h
 src/third_party/pybind11/include/pybind11/stl_bind.h
 src/third_party/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+src/third_party/pybind11/include/pybind11/typing.h
 src/third_party/pybind11/include/pybind11/detail/class.h
 src/third_party/pybind11/include/pybind11/detail/common.h
 src/third_party/pybind11/include/pybind11/detail/descr.h
 src/third_party/pybind11/include/pybind11/detail/init.h
 src/third_party/pybind11/include/pybind11/detail/internals.h
 src/third_party/pybind11/include/pybind11/detail/type_caster_base.h
 src/third_party/pybind11/include/pybind11/detail/typeid.h
```

### Comparing `pugixml-0.5.0/src/third_party/pugixml/CMakeLists.txt` & `pugixml-0.6.0/src/third_party/pugixml/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/LICENSE.md` & `pugixml-0.6.0/src/third_party/pugixml/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/README.md` & `pugixml-0.6.0/src/third_party/pugixml/README.md`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/archive.py` & `pugixml-0.6.0/src/third_party/pugixml/scripts/archive.py`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/natvis/pugixml.natvis` & `pugixml-0.6.0/src/third_party/pugixml/scripts/natvis/pugixml.natvis`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/natvis/pugixml_compact.natvis` & `pugixml-0.6.0/src/third_party/pugixml/scripts/natvis/pugixml_compact.natvis`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/nuget/build/native/pugixml-propertiesui.xml` & `pugixml-0.6.0/src/third_party/pugixml/scripts/nuget/build/native/pugixml-propertiesui.xml`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/nuget/build/native/pugixml.targets` & `pugixml-0.6.0/src/third_party/pugixml/scripts/nuget/build/native/pugixml.targets`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/nuget/pugixml.nuspec` & `pugixml-0.6.0/src/third_party/pugixml/scripts/nuget/pugixml.nuspec`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/nuget_build.ps1` & `pugixml-0.6.0/src/third_party/pugixml/scripts/nuget_build.ps1`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/premake4.lua` & `pugixml-0.6.0/src/third_party/pugixml/scripts/premake4.lua`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml-config.cmake.in` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml-config.cmake.in`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml.xcodeproj/project.pbxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_codeblocks.cbp` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_codeblocks.cbp`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_codelite.project` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_codelite.project`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_dll.rc` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_dll.rc`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2005.vcproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2005.vcproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2005_static.vcproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2005_static.vcproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2008.vcproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2008.vcproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2008_static.vcproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2008_static.vcproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2010.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2010.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2010_static.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2010_static.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2013.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2013.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2013_static.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2013_static.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2015.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2015.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2015_static.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2015_static.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2017.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2017.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2017_static.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2017_static.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2019.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2019.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2019_static.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2019_static.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2022.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2022.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/scripts/pugixml_vs2022_static.vcxproj` & `pugixml-0.6.0/src/third_party/pugixml/scripts/pugixml_vs2022_static.vcxproj`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/src/pugiconfig.hpp` & `pugixml-0.6.0/src/third_party/pugixml/src/pugiconfig.hpp`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/src/pugixml.cpp` & `pugixml-0.6.0/src/third_party/pugixml/src/pugixml.cpp`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pugixml/src/pugixml.hpp` & `pugixml-0.6.0/src/third_party/pugixml/src/pugixml.hpp`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/CMakeLists.txt` & `pugixml-0.6.0/src/third_party/pybind11/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 # CMakeLists.txt -- Build system for the pybind11 modules
 #
 # Copyright (c) 2015 Wenzel Jakob <wenzel@inf.ethz.ch>
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 
+# Propagate this policy (FindPythonInterp removal) so it can be detected later
+if(NOT CMAKE_VERSION VERSION_LESS "3.27")
+  cmake_policy(GET CMP0148 _pybind11_cmp0148)
+endif()
+
 cmake_minimum_required(VERSION 3.5)
 
-# The `cmake_minimum_required(VERSION 3.5...3.26)` syntax does not work with
+# The `cmake_minimum_required(VERSION 3.5...3.27)` syntax does not work with
 # some versions of VS that have a patched CMake 3.11. This forces us to emulate
 # the behavior using the following workaround:
-if(${CMAKE_VERSION} VERSION_LESS 3.26)
+if(${CMAKE_VERSION} VERSION_LESS 3.27)
   cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
 else()
-  cmake_policy(VERSION 3.26)
+  cmake_policy(VERSION 3.27)
+endif()
+
+if(_pybind11_cmp0148)
+  cmake_policy(SET CMP0148 ${_pybind11_cmp0148})
+  unset(_pybind11_cmp0148)
 endif()
 
 # Avoid infinite recursion if tests include this as a subdirectory
 if(DEFINED PYBIND11_MASTER_PROJECT)
   return()
 endif()
 
@@ -78,41 +88,66 @@
     set(CMAKE_CXX_EXTENSIONS OFF)
     set(CMAKE_CXX_STANDARD_REQUIRED ON)
   endif()
 
   set(pybind11_system "")
 
   set_property(GLOBAL PROPERTY USE_FOLDERS ON)
+  if(CMAKE_VERSION VERSION_LESS "3.18")
+    set(_pybind11_findpython_default OFF)
+  else()
+    set(_pybind11_findpython_default ON)
+  endif()
 else()
   set(PYBIND11_MASTER_PROJECT OFF)
   set(pybind11_system SYSTEM)
+  set(_pybind11_findpython_default OFF)
 endif()
 
 # Options
 option(PYBIND11_INSTALL "Install pybind11 header files?" ${PYBIND11_MASTER_PROJECT})
 option(PYBIND11_TEST "Build pybind11 test suite?" ${PYBIND11_MASTER_PROJECT})
 option(PYBIND11_NOPYTHON "Disable search for Python" OFF)
+option(PYBIND11_DISABLE_HANDLE_TYPE_NAME_DEFAULT_IMPLEMENTATION
+       "To enforce that a handle_type_name<> specialization exists" OFF)
 option(PYBIND11_SIMPLE_GIL_MANAGEMENT
        "Use simpler GIL management logic that does not support disassociation" OFF)
+option(PYBIND11_NUMPY_1_ONLY
+       "Disable NumPy 2 support to avoid changes to previous pybind11 versions." OFF)
 set(PYBIND11_INTERNALS_VERSION
     ""
     CACHE STRING "Override the ABI version, may be used to enable the unstable ABI.")
 
+if(PYBIND11_DISABLE_HANDLE_TYPE_NAME_DEFAULT_IMPLEMENTATION)
+  add_compile_definitions(PYBIND11_DISABLE_HANDLE_TYPE_NAME_DEFAULT_IMPLEMENTATION)
+endif()
 if(PYBIND11_SIMPLE_GIL_MANAGEMENT)
   add_compile_definitions(PYBIND11_SIMPLE_GIL_MANAGEMENT)
 endif()
+if(PYBIND11_NUMPY_1_ONLY)
+  add_compile_definitions(PYBIND11_NUMPY_1_ONLY)
+endif()
 
 cmake_dependent_option(
   USE_PYTHON_INCLUDE_DIR
   "Install pybind11 headers in Python include directory instead of default installation prefix"
   OFF "PYBIND11_INSTALL" OFF)
 
-cmake_dependent_option(PYBIND11_FINDPYTHON "Force new FindPython" OFF
+cmake_dependent_option(PYBIND11_FINDPYTHON "Force new FindPython" ${_pybind11_findpython_default}
                        "NOT CMAKE_VERSION VERSION_LESS 3.12" OFF)
 
+# Allow PYTHON_EXECUTABLE if in FINDPYTHON mode and building pybind11's tests
+# (makes transition easier while we support both modes).
+if(PYBIND11_MASTER_PROJECT
+   AND PYBIND11_FINDPYTHON
+   AND DEFINED PYTHON_EXECUTABLE
+   AND NOT DEFINED Python_EXECUTABLE)
+  set(Python_EXECUTABLE "${PYTHON_EXECUTABLE}")
+endif()
+
 # NB: when adding a header don't forget to also add it to setup.py
 set(PYBIND11_HEADERS
     include/pybind11/detail/class.h
     include/pybind11/detail/common.h
     include/pybind11/detail/descr.h
     include/pybind11/detail/init.h
     include/pybind11/detail/internals.h
@@ -128,24 +163,26 @@
     include/pybind11/eigen.h
     include/pybind11/eigen/common.h
     include/pybind11/eigen/matrix.h
     include/pybind11/eigen/tensor.h
     include/pybind11/embed.h
     include/pybind11/eval.h
     include/pybind11/gil.h
+    include/pybind11/gil_safe_call_once.h
     include/pybind11/iostream.h
     include/pybind11/functional.h
     include/pybind11/numpy.h
     include/pybind11/operators.h
     include/pybind11/pybind11.h
     include/pybind11/pytypes.h
     include/pybind11/stl.h
     include/pybind11/stl_bind.h
     include/pybind11/stl/filesystem.h
-    include/pybind11/type_caster_pyobject_ptr.h)
+    include/pybind11/type_caster_pyobject_ptr.h
+    include/pybind11/typing.h)
 
 # Compare with grep and warn if mismatched
 if(PYBIND11_MASTER_PROJECT AND NOT CMAKE_VERSION VERSION_LESS 3.12)
   file(
     GLOB_RECURSE _pybind11_header_check
     LIST_DIRECTORIES false
     RELATIVE "${CMAKE_CURRENT_SOURCE_DIR}"
@@ -273,15 +310,29 @@
   install(
     EXPORT "${PYBIND11_EXPORT_NAME}"
     NAMESPACE "pybind11::"
     DESTINATION ${PYBIND11_CMAKECONFIG_INSTALL_DIR})
 
   # pkg-config support
   if(NOT prefix_for_pc_file)
-    set(prefix_for_pc_file "${CMAKE_INSTALL_PREFIX}")
+    if(IS_ABSOLUTE "${CMAKE_INSTALL_DATAROOTDIR}")
+      set(prefix_for_pc_file "${CMAKE_INSTALL_PREFIX}")
+    else()
+      set(pc_datarootdir "${CMAKE_INSTALL_DATAROOTDIR}")
+      if(CMAKE_VERSION VERSION_LESS 3.20)
+        set(prefix_for_pc_file "\${pcfiledir}/..")
+        while(pc_datarootdir)
+          get_filename_component(pc_datarootdir "${pc_datarootdir}" DIRECTORY)
+          string(APPEND prefix_for_pc_file "/..")
+        endwhile()
+      else()
+        cmake_path(RELATIVE_PATH CMAKE_INSTALL_PREFIX BASE_DIRECTORY CMAKE_INSTALL_DATAROOTDIR
+                   OUTPUT_VARIABLE prefix_for_pc_file)
+      endif()
+    endif()
   endif()
   join_paths(includedir_for_pc_file "\${prefix}" "${CMAKE_INSTALL_INCLUDEDIR}")
   configure_file("${CMAKE_CURRENT_SOURCE_DIR}/tools/pybind11.pc.in"
                  "${CMAKE_CURRENT_BINARY_DIR}/pybind11.pc" @ONLY)
   install(FILES "${CMAKE_CURRENT_BINARY_DIR}/pybind11.pc"
           DESTINATION "${CMAKE_INSTALL_DATAROOTDIR}/pkgconfig/")
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/LICENSE` & `pugixml-0.6.0/src/third_party/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/README.rst` & `pugixml-0.6.0/src/third_party/pybind11/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 dependency.
 
 Think of this library as a tiny self-contained version of Boost.Python
 with everything stripped away that isn't relevant for binding
 generation. Without comments, the core header files only require ~4K
 lines of code and depend on Python (3.6+, or PyPy) and the C++
 standard library. This compact implementation was possible thanks to
-some of the new C++11 language features (specifically: tuples, lambda
-functions and variadic templates). Since its creation, this library has
-grown beyond Boost.Python in many ways, leading to dramatically simpler
-binding code in many common situations.
+some C++11 language features (specifically: tuples, lambda functions and
+variadic templates). Since its creation, this library has grown beyond
+Boost.Python in many ways, leading to dramatically simpler binding code in many
+common situations.
 
 Tutorial and reference documentation is provided at
 `pybind11.readthedocs.io <https://pybind11.readthedocs.io/en/latest>`_.
 A PDF version of the manual is available
 `here <https://pybind11.readthedocs.io/_/downloads/en/latest/pdf/>`_.
 And the source code is always available at
 `github.com/pybind/pybind11 <https://github.com/pybind/pybind11>`_.
@@ -67,14 +67,15 @@
 - Custom operators
 - Single and multiple inheritance
 - STL data structures
 - Smart pointers with reference counting like ``std::shared_ptr``
 - Internal references with correct reference counting
 - C++ classes with virtual (and pure virtual) methods can be extended
   in Python
+- Integrated NumPy support (NumPy 2 requires pybind11 2.12+)
 
 Goodies
 -------
 
 In addition to the core functionality, pybind11 provides some extra
 goodies:
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/attr.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/buffer_info.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/cast.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/cast.h`

 * *Files 6% similar despite different names*

```diff
@@ -38,21 +38,23 @@
 class type_caster : public type_caster_base<type> {};
 template <typename type>
 using make_caster = type_caster<intrinsic_t<type>>;
 
 // Shortcut for calling a caster's `cast_op_type` cast operator for casting a type_caster to a T
 template <typename T>
 typename make_caster<T>::template cast_op_type<T> cast_op(make_caster<T> &caster) {
-    return caster.operator typename make_caster<T>::template cast_op_type<T>();
+    using result_t = typename make_caster<T>::template cast_op_type<T>; // See PR #4893
+    return caster.operator result_t();
 }
 template <typename T>
 typename make_caster<T>::template cast_op_type<typename std::add_rvalue_reference<T>::type>
 cast_op(make_caster<T> &&caster) {
-    return std::move(caster).operator typename make_caster<T>::
-        template cast_op_type<typename std::add_rvalue_reference<T>::type>();
+    using result_t = typename make_caster<T>::template cast_op_type<
+        typename std::add_rvalue_reference<T>::type>; // See PR #4893
+    return std::move(caster).operator result_t();
 }
 
 template <typename type>
 class type_caster<std::reference_wrapper<type>> {
 private:
     using caster_t = make_caster<type>;
     caster_t subcaster;
@@ -321,16 +323,17 @@
             value = true;
             return true;
         }
         if (src.ptr() == Py_False) {
             value = false;
             return true;
         }
-        if (convert || (std::strcmp("numpy.bool_", Py_TYPE(src.ptr())->tp_name) == 0)) {
-            // (allow non-implicit conversion for numpy booleans)
+        if (convert || is_numpy_bool(src)) {
+            // (allow non-implicit conversion for numpy booleans), use strncmp
+            // since NumPy 1.x had an additional trailing underscore.
 
             Py_ssize_t res = -1;
             if (src.is_none()) {
                 res = 0; // None is implicitly converted to False
             }
 #if defined(PYPY_VERSION)
             // On PyPy, check that "__bool__" attr exists
@@ -354,14 +357,23 @@
         }
         return false;
     }
     static handle cast(bool src, return_value_policy /* policy */, handle /* parent */) {
         return handle(src ? Py_True : Py_False).inc_ref();
     }
     PYBIND11_TYPE_CASTER(bool, const_name("bool"));
+
+private:
+    // Test if an object is a NumPy boolean (without fetching the type).
+    static inline bool is_numpy_bool(handle object) {
+        const char *type_name = Py_TYPE(object.ptr())->tp_name;
+        // Name changed to `numpy.bool` in NumPy 2, `numpy.bool_` is needed for 1.x support
+        return std::strcmp("numpy.bool", type_name) == 0
+               || std::strcmp("numpy.bool_", type_name) == 0;
+    }
 };
 
 // Helper class for UTF-{8,16,32} C++ stl strings:
 template <typename StringType, bool IsView = false>
 struct string_caster {
     using CharT = typename StringType::value_type;
 
@@ -656,16 +668,17 @@
             auto h = cast(std::move(*src), policy, parent);
             delete src;
             return h;
         }
         return cast(*src, policy, parent);
     }
 
-    static constexpr auto name
-        = const_name("Tuple[") + concat(make_caster<Ts>::name...) + const_name("]");
+    static constexpr auto name = const_name("tuple[")
+                                 + ::pybind11::detail::concat(make_caster<Ts>::name...)
+                                 + const_name("]");
 
     template <typename T>
     using cast_op_type = type;
 
     explicit operator type() & { return implicit_cast(indices{}); }
     explicit operator type() && { return std::move(*this).implicit_cast(indices{}); }
 
@@ -865,27 +878,74 @@
 template <typename base, typename holder>
 struct is_holder_type
     : std::is_base_of<detail::type_caster_holder<base, holder>, detail::type_caster<holder>> {};
 // Specialization for always-supported unique_ptr holders:
 template <typename base, typename deleter>
 struct is_holder_type<base, std::unique_ptr<base, deleter>> : std::true_type {};
 
+#ifdef PYBIND11_DISABLE_HANDLE_TYPE_NAME_DEFAULT_IMPLEMENTATION // See PR #4888
+
+// This leads to compilation errors if a specialization is missing.
+template <typename T>
+struct handle_type_name;
+
+#else
+
 template <typename T>
 struct handle_type_name {
     static constexpr auto name = const_name<T>();
 };
+
+#endif
+
+template <>
+struct handle_type_name<object> {
+    static constexpr auto name = const_name("object");
+};
+template <>
+struct handle_type_name<list> {
+    static constexpr auto name = const_name("list");
+};
+template <>
+struct handle_type_name<dict> {
+    static constexpr auto name = const_name("dict");
+};
+template <>
+struct handle_type_name<anyset> {
+    static constexpr auto name = const_name("Union[set, frozenset]");
+};
+template <>
+struct handle_type_name<set> {
+    static constexpr auto name = const_name("set");
+};
+template <>
+struct handle_type_name<frozenset> {
+    static constexpr auto name = const_name("frozenset");
+};
+template <>
+struct handle_type_name<str> {
+    static constexpr auto name = const_name("str");
+};
+template <>
+struct handle_type_name<tuple> {
+    static constexpr auto name = const_name("tuple");
+};
 template <>
 struct handle_type_name<bool_> {
     static constexpr auto name = const_name("bool");
 };
 template <>
 struct handle_type_name<bytes> {
     static constexpr auto name = const_name(PYBIND11_BYTES_NAME);
 };
 template <>
+struct handle_type_name<buffer> {
+    static constexpr auto name = const_name("Buffer");
+};
+template <>
 struct handle_type_name<int_> {
     static constexpr auto name = const_name("int");
 };
 template <>
 struct handle_type_name<iterable> {
     static constexpr auto name = const_name("Iterable");
 };
@@ -894,25 +954,89 @@
     static constexpr auto name = const_name("Iterator");
 };
 template <>
 struct handle_type_name<float_> {
     static constexpr auto name = const_name("float");
 };
 template <>
+struct handle_type_name<function> {
+    static constexpr auto name = const_name("Callable");
+};
+template <>
+struct handle_type_name<handle> {
+    static constexpr auto name = handle_type_name<object>::name;
+};
+template <>
 struct handle_type_name<none> {
     static constexpr auto name = const_name("None");
 };
 template <>
+struct handle_type_name<sequence> {
+    static constexpr auto name = const_name("Sequence");
+};
+template <>
+struct handle_type_name<bytearray> {
+    static constexpr auto name = const_name("bytearray");
+};
+template <>
+struct handle_type_name<memoryview> {
+    static constexpr auto name = const_name("memoryview");
+};
+template <>
+struct handle_type_name<slice> {
+    static constexpr auto name = const_name("slice");
+};
+template <>
+struct handle_type_name<type> {
+    static constexpr auto name = const_name("type");
+};
+template <>
+struct handle_type_name<capsule> {
+    static constexpr auto name = const_name("capsule");
+};
+template <>
+struct handle_type_name<ellipsis> {
+    static constexpr auto name = const_name("ellipsis");
+};
+template <>
+struct handle_type_name<weakref> {
+    static constexpr auto name = const_name("weakref");
+};
+template <>
 struct handle_type_name<args> {
     static constexpr auto name = const_name("*args");
 };
 template <>
 struct handle_type_name<kwargs> {
     static constexpr auto name = const_name("**kwargs");
 };
+template <>
+struct handle_type_name<obj_attr_accessor> {
+    static constexpr auto name = const_name<obj_attr_accessor>();
+};
+template <>
+struct handle_type_name<str_attr_accessor> {
+    static constexpr auto name = const_name<str_attr_accessor>();
+};
+template <>
+struct handle_type_name<item_accessor> {
+    static constexpr auto name = const_name<item_accessor>();
+};
+template <>
+struct handle_type_name<sequence_accessor> {
+    static constexpr auto name = const_name<sequence_accessor>();
+};
+template <>
+struct handle_type_name<list_accessor> {
+    static constexpr auto name = const_name<list_accessor>();
+};
+template <>
+struct handle_type_name<tuple_accessor> {
+    static constexpr auto name = const_name<tuple_accessor>();
+};
 
 template <typename type>
 struct pyobject_caster {
     template <typename T = type, enable_if_t<std::is_same<T, handle>::value, int> = 0>
     pyobject_caster() : value() {}
 
     // `type` may not be default constructible (e.g. frozenset, anyset).  Initializing `value`
@@ -1373,15 +1497,23 @@
 template <typename /*unused*/>
 using arg_t = arg_v;
 
 inline namespace literals {
 /** \rst
     String literal version of `arg`
  \endrst */
-constexpr arg operator"" _a(const char *name, size_t) { return arg(name); }
+constexpr arg
+#if !defined(__clang__) && defined(__GNUC__) && __GNUC__ < 5
+operator"" _a // gcc 4.8.5 insists on having a space (hard error).
+#else
+operator""_a // clang 17 generates a deprecation warning if there is a space.
+#endif
+    (const char *name, size_t) {
+    return arg(name);
+}
 } // namespace literals
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <typename T>
 using is_kw_only = std::is_same<intrinsic_t<T>, kw_only>;
 template <typename T>
@@ -1434,15 +1566,16 @@
 
     // py::args argument position; -1 if not present.
     static constexpr int args_pos = constexpr_last<argument_is_args, Args...>();
 
     static_assert(args_pos == -1 || args_pos == constexpr_first<argument_is_args, Args...>(),
                   "py::args cannot be specified more than once");
 
-    static constexpr auto arg_names = concat(type_descr(make_caster<Args>::name)...);
+    static constexpr auto arg_names
+        = ::pybind11::detail::concat(type_descr(make_caster<Args>::name)...);
 
     bool load_args(function_call &call) { return load_impl_sequence(call, indices{}); }
 
     template <typename Return, typename Guard, typename Func>
     // NOLINTNEXTLINE(readability-const-return-type)
     enable_if_t<!std::is_void<Return>::value, Return> call(Func &&f) && {
         return std::move(*this).template call_impl<remove_cv_t<Return>>(
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/chrono.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/complex.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/class.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/class.h`

 * *Files 1% similar despite different names*

```diff
@@ -82,25 +82,24 @@
     auto *type = &heap_type->ht_type;
     type->tp_name = name;
     type->tp_base = type_incref(&PyProperty_Type);
     type->tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HEAPTYPE;
     type->tp_descr_get = pybind11_static_get;
     type->tp_descr_set = pybind11_static_set;
 
-    if (PyType_Ready(type) < 0) {
-        pybind11_fail("make_static_property_type(): failure in PyType_Ready()!");
-    }
-
 #    if PY_VERSION_HEX >= 0x030C0000
-    // PRE 3.12 FEATURE FREEZE. PLEASE REVIEW AFTER FREEZE.
     // Since Python-3.12 property-derived types are required to
     // have dynamic attributes (to set `__doc__`)
     enable_dynamic_attributes(heap_type);
 #    endif
 
+    if (PyType_Ready(type) < 0) {
+        pybind11_fail("make_static_property_type(): failure in PyType_Ready()!");
+    }
+
     setattr((PyObject *) type, "__module__", str("pybind11_builtins"));
     PYBIND11_SET_OLDPY_QUALNAME(type, name_obj);
 
     return type;
 }
 
 #else // PYPY
@@ -185,20 +184,18 @@
 
     // use the default metaclass call to create/initialize the object
     PyObject *self = PyType_Type.tp_call(type, args, kwargs);
     if (self == nullptr) {
         return nullptr;
     }
 
-    // This must be a pybind11 instance
-    auto *instance = reinterpret_cast<detail::instance *>(self);
-
     // Ensure that the base __init__ function(s) were called
-    for (const auto &vh : values_and_holders(instance)) {
-        if (!vh.holder_constructed()) {
+    values_and_holders vhs(self);
+    for (const auto &vh : vhs) {
+        if (!vh.holder_constructed() && !vhs.is_redundant_value_and_holder(vh)) {
             PyErr_Format(PyExc_TypeError,
                          "%.200s.__init__() must be called when overriding __init__",
                          get_fully_qualified_tp_name(vh.type->type).c_str());
             Py_DECREF(self);
             return nullptr;
         }
     }
@@ -371,15 +368,15 @@
 
 /// An `__init__` function constructs the C++ object. Users should provide at least one
 /// of these using `py::init` or directly with `.def(__init__, ...)`. Otherwise, the
 /// following default function will be used which simply throws an exception.
 extern "C" inline int pybind11_object_init(PyObject *self, PyObject *, PyObject *) {
     PyTypeObject *type = Py_TYPE(self);
     std::string msg = get_fully_qualified_tp_name(type) + ": No constructor defined!";
-    PyErr_SetString(PyExc_TypeError, msg.c_str());
+    set_error(PyExc_TypeError, msg.c_str());
     return -1;
 }
 
 inline void add_patient(PyObject *nurse, PyObject *patient) {
     auto &internals = get_internals();
     auto *instance = reinterpret_cast<detail::instance *>(nurse);
     instance->has_patients = true;
@@ -518,27 +515,35 @@
 
     assert(!PyType_HasFeature(type, Py_TPFLAGS_HAVE_GC));
     return (PyObject *) heap_type;
 }
 
 /// dynamic_attr: Allow the garbage collector to traverse the internal instance `__dict__`.
 extern "C" inline int pybind11_traverse(PyObject *self, visitproc visit, void *arg) {
+#if PY_VERSION_HEX >= 0x030D0000
+    PyObject_VisitManagedDict(self, visit, arg);
+#else
     PyObject *&dict = *_PyObject_GetDictPtr(self);
     Py_VISIT(dict);
+#endif
 // https://docs.python.org/3/c-api/typeobj.html#c.PyTypeObject.tp_traverse
 #if PY_VERSION_HEX >= 0x03090000
     Py_VISIT(Py_TYPE(self));
 #endif
     return 0;
 }
 
 /// dynamic_attr: Allow the GC to clear the dictionary.
 extern "C" inline int pybind11_clear(PyObject *self) {
+#if PY_VERSION_HEX >= 0x030D0000
+    PyObject_ClearManagedDict(self);
+#else
     PyObject *&dict = *_PyObject_GetDictPtr(self);
     Py_CLEAR(dict);
+#endif
     return 0;
 }
 
 /// Give instances of this type a `__dict__` and opt into garbage collection.
 inline void enable_dynamic_attributes(PyHeapTypeObject *heap_type) {
     auto *type = &heap_type->ht_type;
     type->tp_flags |= Py_TPFLAGS_HAVE_GC;
@@ -575,23 +580,23 @@
             break;
         }
     }
     if (view == nullptr || !tinfo || !tinfo->get_buffer) {
         if (view) {
             view->obj = nullptr;
         }
-        PyErr_SetString(PyExc_BufferError, "pybind11_getbuffer(): Internal error");
+        set_error(PyExc_BufferError, "pybind11_getbuffer(): Internal error");
         return -1;
     }
     std::memset(view, 0, sizeof(Py_buffer));
     buffer_info *info = tinfo->get_buffer(obj, tinfo->get_buffer_data);
     if ((flags & PyBUF_WRITABLE) == PyBUF_WRITABLE && info->readonly) {
         delete info;
         // view->obj = nullptr;  // Was just memset to 0, so not necessary
-        PyErr_SetString(PyExc_BufferError, "Writable buffer requested for readonly storage");
+        set_error(PyExc_BufferError, "Writable buffer requested for readonly storage");
         return -1;
     }
     view->obj = obj;
     view->ndim = 1;
     view->internal = info;
     view->buf = info->ptr;
     view->itemsize = info->itemsize;
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/common.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/common.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #define PYBIND11_VERSION_MAJOR 2
-#define PYBIND11_VERSION_MINOR 11
-#define PYBIND11_VERSION_PATCH 1
+#define PYBIND11_VERSION_MINOR 12
+#define PYBIND11_VERSION_PATCH 0
 
 // Similar to Python's convention: https://docs.python.org/3/c-api/apiabiversion.html
 // Additional convention: 0xD = dev
-#define PYBIND11_VERSION_HEX 0x020B0100
+#define PYBIND11_VERSION_HEX 0x020C0000
 
 // Define some generic pybind11 helper macros for warning management.
 //
 // Note that compiler-specific push/pop pairs are baked into the
 // PYBIND11_NAMESPACE_BEGIN/PYBIND11_NAMESPACE_END pair of macros. Therefore manual
 // PYBIND11_WARNING_PUSH/PYBIND11_WARNING_POP are usually only needed in `#include` sections.
 //
@@ -114,14 +114,22 @@
 #            if _MSVC_LANG >= 202002L
 #                define PYBIND11_CPP20
 #            endif
 #        endif
 #    endif
 #endif
 
+#if defined(PYBIND11_CPP20)
+#    define PYBIND11_CONSTINIT constinit
+#    define PYBIND11_DTOR_CONSTEXPR constexpr
+#else
+#    define PYBIND11_CONSTINIT
+#    define PYBIND11_DTOR_CONSTEXPR
+#endif
+
 // Compiler version assertions
 #if defined(__INTEL_COMPILER)
 #    if __INTEL_COMPILER < 1800
 #        error pybind11 requires Intel C++ compiler v18 or newer
 #    elif __INTEL_COMPILER < 1900 && defined(PYBIND11_CPP14)
 #        error pybind11 supports only C++11 with Intel C++ compiler v18. Use v19 or newer for C++14.
 #    endif
@@ -284,14 +292,18 @@
 #    undef toupper
 #endif
 
 #if defined(copysign)
 #    undef copysign
 #endif
 
+#if defined(PYBIND11_NUMPY_1_ONLY)
+#    define PYBIND11_INTERNAL_NUMPY_1_ONLY_DETECTED
+#endif
+
 #if defined(PYPY_VERSION) && !defined(PYBIND11_SIMPLE_GIL_MANAGEMENT)
 #    define PYBIND11_SIMPLE_GIL_MANAGEMENT
 #endif
 
 #if defined(_MSC_VER)
 #    if defined(PYBIND11_DEBUG_MARKER)
 #        define _DEBUG
@@ -395,15 +407,15 @@
 
 #define PYBIND11_CATCH_INIT_EXCEPTIONS                                                            \
     catch (pybind11::error_already_set & e) {                                                     \
         pybind11::raise_from(e, PyExc_ImportError, "initialization failed");                      \
         return nullptr;                                                                           \
     }                                                                                             \
     catch (const std::exception &e) {                                                             \
-        PyErr_SetString(PyExc_ImportError, e.what());                                             \
+        ::pybind11::set_error(PyExc_ImportError, e.what());                                       \
         return nullptr;                                                                           \
     }
 
 /** \rst
     ***Deprecated in favor of PYBIND11_MODULE***
 
     This macro creates the entry point that will be invoked when the Python interpreter
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/descr.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/init.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/init.h`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 // Failing fallback version of the above for a no-alias class (always returns false)
 template <typename /*Class*/>
 constexpr bool is_alias(void *) {
     return false;
 }
 
 // Constructs and returns a new object; if the given arguments don't map to a constructor, we fall
-// back to brace aggregate initiailization so that for aggregate initialization can be used with
+// back to brace aggregate initialization so that for aggregate initialization can be used with
 // py::init, e.g.  `py::init<int, int>` to initialize a `struct T { int a; int b; }`.  For
 // non-aggregate types, we need to use an ordinary T(...) constructor (invoking as `T{...}` usually
 // works, but will not do the expected thing when `T` has an `initializer_list<T>` constructor).
 template <typename Class,
           typename... Args,
           detail::enable_if_t<std::is_constructible<Class, Args...>::value, int> = 0>
 inline Class *construct_or_initialize(Args &&...args) {
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/internals.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/internals.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,17 @@
 /// newer ABI.
 ///
 /// WARNING: If you choose to manually increase the ABI version, note that
 /// pybind11 may not be tested as thoroughly with a non-default ABI version, and
 /// further ABI-incompatible changes may be made before the ABI is officially
 /// changed to the new version.
 #ifndef PYBIND11_INTERNALS_VERSION
-#    if PY_VERSION_HEX >= 0x030C0000
+#    if PY_VERSION_HEX >= 0x030C0000 || defined(_MSC_VER)
 // Version bump for Python 3.12+, before first 3.12 beta release.
+// Version bump for MSVC piggy-backed on PR #4779. See comments there.
 #        define PYBIND11_INTERNALS_VERSION 5
 #    else
 #        define PYBIND11_INTERNALS_VERSION 4
 #    endif
 #endif
 
 // This requirement is mainly to reduce the support burden (see PR #4570).
@@ -62,17 +63,22 @@
 // The old Python Thread Local Storage (TLS) API is deprecated in Python 3.7 in favor of the new
 // Thread Specific Storage (TSS) API.
 #if PY_VERSION_HEX >= 0x03070000
 // Avoid unnecessary allocation of `Py_tss_t`, since we cannot use
 // `Py_LIMITED_API` anyway.
 #    if PYBIND11_INTERNALS_VERSION > 4
 #        define PYBIND11_TLS_KEY_REF Py_tss_t &
-#        if defined(__GNUC__) && !defined(__INTEL_COMPILER)
-// Clang on macOS warns due to `Py_tss_NEEDS_INIT` not specifying an initializer
-// for every field.
+#        if defined(__clang__)
+#            define PYBIND11_TLS_KEY_INIT(var)                                                    \
+                _Pragma("clang diagnostic push")                                         /**/     \
+                    _Pragma("clang diagnostic ignored \"-Wmissing-field-initializers\"") /**/     \
+                    Py_tss_t var                                                                  \
+                    = Py_tss_NEEDS_INIT;                                                          \
+                _Pragma("clang diagnostic pop")
+#        elif defined(__GNUC__) && !defined(__INTEL_COMPILER)
 #            define PYBIND11_TLS_KEY_INIT(var)                                                    \
                 _Pragma("GCC diagnostic push")                                         /**/       \
                     _Pragma("GCC diagnostic ignored \"-Wmissing-field-initializers\"") /**/       \
                     Py_tss_t var                                                                  \
                     = Py_tss_NEEDS_INIT;                                                          \
                 _Pragma("GCC diagnostic pop")
 #        else
@@ -287,17 +293,20 @@
 #        define PYBIND11_STDLIB "_libstdcpp"
 #    else
 #        define PYBIND11_STDLIB ""
 #    endif
 #endif
 
 /// On Linux/OSX, changes in __GXX_ABI_VERSION__ indicate ABI incompatibility.
+/// On MSVC, changes in _MSC_VER may indicate ABI incompatibility (#2898).
 #ifndef PYBIND11_BUILD_ABI
 #    if defined(__GXX_ABI_VERSION)
 #        define PYBIND11_BUILD_ABI "_cxxabi" PYBIND11_TOSTRING(__GXX_ABI_VERSION)
+#    elif defined(_MSC_VER)
+#        define PYBIND11_BUILD_ABI "_mscver" PYBIND11_TOSTRING(_MSC_VER)
 #    else
 #        define PYBIND11_BUILD_ABI ""
 #    endif
 #endif
 
 #ifndef PYBIND11_INTERNALS_KIND
 #    if defined(WITH_THREAD)
@@ -348,15 +357,15 @@
 }
 
 inline bool raise_err(PyObject *exc_type, const char *msg) {
     if (PyErr_Occurred()) {
         raise_from(exc_type, msg);
         return true;
     }
-    PyErr_SetString(exc_type, msg);
+    set_error(exc_type, msg);
     return false;
 }
 
 inline void translate_exception(std::exception_ptr p) {
     if (!p) {
         return;
     }
@@ -443,26 +452,28 @@
 #    endif
     if (istate) {
         state_dict = reinterpret_borrow<object>(PyInterpreterState_GetDict(istate));
     }
 #endif
     if (!state_dict) {
         raise_from(PyExc_SystemError, "pybind11::detail::get_python_state_dict() FAILED");
+        throw error_already_set();
     }
     return state_dict;
 }
 
 inline object get_internals_obj_from_state_dict(handle state_dict) {
     return reinterpret_borrow<object>(dict_getitemstring(state_dict.ptr(), PYBIND11_INTERNALS_ID));
 }
 
 inline internals **get_internals_pp_from_capsule(handle obj) {
     void *raw_ptr = PyCapsule_GetPointer(obj.ptr(), /*name=*/nullptr);
     if (raw_ptr == nullptr) {
         raise_from(PyExc_SystemError, "pybind11::detail::get_internals_pp_from_capsule() FAILED");
+        throw error_already_set();
     }
     return static_cast<internals **>(raw_ptr);
 }
 
 /// Return a reference to the current `internals` data
 PYBIND11_NOINLINE internals &get_internals() {
     auto **&internals_pp = get_internals_pp();
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/type_caster_base.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,30 @@
 
 // Gets the cache entry for the given type, creating it if necessary.  The return value is the pair
 // returned by emplace, i.e. an iterator for the entry and a bool set to `true` if the entry was
 // just created.
 inline std::pair<decltype(internals::registered_types_py)::iterator, bool>
 all_type_info_get_cache(PyTypeObject *type);
 
+// Band-aid workaround to fix a subtle but serious bug in a minimalistic fashion. See PR #4762.
+inline void all_type_info_add_base_most_derived_first(std::vector<type_info *> &bases,
+                                                      type_info *addl_base) {
+    for (auto it = bases.begin(); it != bases.end(); it++) {
+        type_info *existing_base = *it;
+        if (PyType_IsSubtype(addl_base->type, existing_base->type) != 0) {
+            bases.insert(it, addl_base);
+            return;
+        }
+    }
+    bases.push_back(addl_base);
+}
+
 // Populates a just-created cache entry.
 PYBIND11_NOINLINE void all_type_info_populate(PyTypeObject *t, std::vector<type_info *> &bases) {
+    assert(bases.empty());
     std::vector<PyTypeObject *> check;
     for (handle parent : reinterpret_borrow<tuple>(t->tp_bases)) {
         check.push_back((PyTypeObject *) parent.ptr());
     }
 
     auto const &type_dict = get_internals().registered_types_py;
     for (size_t i = 0; i < check.size(); i++) {
@@ -132,15 +146,15 @@
                 for (auto *known : bases) {
                     if (known == tinfo) {
                         found = true;
                         break;
                     }
                 }
                 if (!found) {
-                    bases.push_back(tinfo);
+                    all_type_info_add_base_most_derived_first(bases, tinfo);
                 }
             }
         } else if (type->tp_bases) {
             // It's some python type, so keep follow its bases classes to look for one or more
             // registered types
             if (i + 1 == check.size()) {
                 // When we're at the end, we can pop off the current element to avoid growing
@@ -318,26 +332,37 @@
     using type_vec = std::vector<detail::type_info *>;
     const type_vec &tinfo;
 
 public:
     explicit values_and_holders(instance *inst)
         : inst{inst}, tinfo(all_type_info(Py_TYPE(inst))) {}
 
+    explicit values_and_holders(PyObject *obj)
+        : inst{nullptr}, tinfo(all_type_info(Py_TYPE(obj))) {
+        if (!tinfo.empty()) {
+            inst = reinterpret_cast<instance *>(obj);
+        }
+    }
+
     struct iterator {
     private:
         instance *inst = nullptr;
         const type_vec *types = nullptr;
         value_and_holder curr;
         friend struct values_and_holders;
-        iterator(instance *inst, const type_vec *tinfo)
-            : inst{inst}, types{tinfo},
-              curr(inst /* instance */,
-                   types->empty() ? nullptr : (*types)[0] /* type info */,
-                   0, /* vpos: (non-simple types only): the first vptr comes first */
-                   0 /* index */) {}
+        iterator(instance *inst, const type_vec *tinfo) : inst{inst}, types{tinfo} {
+            if (inst != nullptr) {
+                assert(!types->empty());
+                curr = value_and_holder(
+                    inst /* instance */,
+                    (*types)[0] /* type info */,
+                    0, /* vpos: (non-simple types only): the first vptr comes first */
+                    0 /* index */);
+            }
+        }
         // Past-the-end iterator:
         explicit iterator(size_t end) : curr(end) {}
 
     public:
         bool operator==(const iterator &other) const { return curr.index == other.curr.index; }
         bool operator!=(const iterator &other) const { return curr.index != other.curr.index; }
         iterator &operator++() {
@@ -360,14 +385,24 @@
         while (it != endit && it->type != find_type) {
             ++it;
         }
         return it;
     }
 
     size_t size() { return tinfo.size(); }
+
+    // Band-aid workaround to fix a subtle but serious bug in a minimalistic fashion. See PR #4762.
+    bool is_redundant_value_and_holder(const value_and_holder &vh) {
+        for (size_t i = 0; i < vh.index; i++) {
+            if (PyType_IsSubtype(tinfo[i]->type, tinfo[vh.index]->type) != 0) {
+                return true;
+            }
+        }
+        return false;
+    }
 };
 
 /**
  * Extracts C++ value and holder pointer references from an instance (which may contain multiple
  * values/holders for python-side multiple inheritance) that match the given type.  Throws an error
  * if the given type (or ValueType, if omitted) is not a pybind11 base of the given instance.  If
  * `find_type` is omitted (or explicitly specified as nullptr) the first value/holder are returned,
@@ -482,16 +517,18 @@
     }
     return handle();
 }
 
 inline PyThreadState *get_thread_state_unchecked() {
 #if defined(PYPY_VERSION)
     return PyThreadState_GET();
-#else
+#elif PY_VERSION_HEX < 0x030D0000
     return _PyThreadState_UncheckedGet();
+#else
+    return PyThreadState_GetUnchecked();
 #endif
 }
 
 // Forward declarations
 void keep_alive_impl(handle nurse, handle patient);
 inline PyObject *make_new_instance(PyTypeObject *type);
 
@@ -782,15 +819,15 @@
             return {src, const_cast<const type_info *>(tpi)};
         }
 
         // Not found, set error:
         std::string tname = rtti_type ? rtti_type->name() : cast_type.name();
         detail::clean_type_id(tname);
         std::string msg = "Unregistered type : " + tname;
-        PyErr_SetString(PyExc_TypeError, msg.c_str());
+        set_error(PyExc_TypeError, msg.c_str());
         return {nullptr, nullptr};
     }
 
     const type_info *typeinfo = nullptr;
     const std::type_info *cpptype = nullptr;
     void *value = nullptr;
 };
@@ -1160,18 +1197,22 @@
         };
     }
 
     static Constructor make_copy_constructor(...) { return nullptr; }
     static Constructor make_move_constructor(...) { return nullptr; }
 };
 
+inline std::string quote_cpp_type_name(const std::string &cpp_type_name) {
+    return cpp_type_name; // No-op for now. See PR #4888
+}
+
 PYBIND11_NOINLINE std::string type_info_description(const std::type_info &ti) {
     if (auto *type_data = get_type_info(ti)) {
         handle th((PyObject *) type_data->type);
         return th.attr("__module__").cast<std::string>() + '.'
                + th.attr("__qualname__").cast<std::string>();
     }
-    return clean_type_id(ti.name());
+    return quote_cpp_type_name(clean_type_id(ti.name()));
 }
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/detail/typeid.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/eigen/matrix.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/eigen/tensor.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/eigen/tensor.h`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     }
 
     template <typename T>
     struct helper {};
 
     template <size_t... Is>
     struct helper<index_sequence<Is...>> {
-        static constexpr auto value = concat(const_name(((void) Is, "?"))...);
+        static constexpr auto value = ::pybind11::detail::concat(const_name(((void) Is, "?"))...);
     };
 
     static constexpr auto dimensions_descriptor
         = helper<decltype(make_index_sequence<Type::NumIndices>())>::value;
 
     template <typename... Args>
     static Type *alloc(Args &&...args) {
@@ -100,15 +100,16 @@
     }
 
     static bool
     is_correct_shape(const Eigen::DSizes<typename Type::Index, Type::NumIndices> &shape) {
         return get_shape() == shape;
     }
 
-    static constexpr auto dimensions_descriptor = concat(const_name<Indices>()...);
+    static constexpr auto dimensions_descriptor
+        = ::pybind11::detail::concat(const_name<Indices>()...);
 
     template <typename... Args>
     static Type *alloc(Args &&...args) {
         Eigen::aligned_allocator<Type> allocator;
         return ::new (allocator.allocate(1)) Type(std::forward<Args>(args)...);
     }
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/embed.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/eval.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/functional.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/functional.h`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         if (result) {
             return cpp_function(*result, policy).release();
         }
         return cpp_function(std::forward<Func>(f_), policy).release();
     }
 
     PYBIND11_TYPE_CASTER(type,
-                         const_name("Callable[[") + concat(make_caster<Args>::name...)
+                         const_name("Callable[[")
+                             + ::pybind11::detail::concat(make_caster<Args>::name...)
                              + const_name("], ") + make_caster<retval_type>::name
                              + const_name("]"));
 };
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/gil.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/gil.h`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "detail/common.h"
 
+#include <cassert>
+
 #if defined(WITH_THREAD) && !defined(PYBIND11_SIMPLE_GIL_MANAGEMENT)
 #    include "detail/internals.h"
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 PYBIND11_NAMESPACE_BEGIN(detail)
@@ -133,15 +135,17 @@
     PyThreadState *tstate = nullptr;
     bool release = true;
     bool active = true;
 };
 
 class gil_scoped_release {
 public:
+    // PRECONDITION: The GIL must be held when this constructor is called.
     explicit gil_scoped_release(bool disassoc = false) : disassoc(disassoc) {
+        assert(PyGILState_Check());
         // `get_internals()` must be called here unconditionally in order to initialize
         // `internals.tstate` for subsequent `gil_scoped_acquire` calls. Otherwise, an
         // initialization race could occur as multiple threads try `gil_scoped_acquire`.
         auto &internals = detail::get_internals();
         // NOLINTNEXTLINE(cppcoreguidelines-prefer-member-initializer)
         tstate = PyEval_SaveThread();
         if (disassoc) {
@@ -197,15 +201,19 @@
     void disarm() {}
 };
 
 class gil_scoped_release {
     PyThreadState *state;
 
 public:
-    gil_scoped_release() : state{PyEval_SaveThread()} {}
+    // PRECONDITION: The GIL must be held when this constructor is called.
+    gil_scoped_release() {
+        assert(PyGILState_Check());
+        state = PyEval_SaveThread();
+    }
     gil_scoped_release(const gil_scoped_release &) = delete;
     gil_scoped_release &operator=(const gil_scoped_release &) = delete;
     ~gil_scoped_release() { PyEval_RestoreThread(state); }
     void disarm() {}
 };
 
 #    endif // PYBIND11_SIMPLE_GIL_MANAGEMENT
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/iostream.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/numpy.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/numpy.h`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,18 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "pybind11.h"
+#include "detail/common.h"
 #include "complex.h"
+#include "gil_safe_call_once.h"
+#include "pytypes.h"
 
 #include <algorithm>
 #include <array>
 #include <cstdint>
 #include <cstdlib>
 #include <cstring>
 #include <functional>
@@ -22,53 +25,102 @@
 #include <sstream>
 #include <string>
 #include <type_traits>
 #include <typeindex>
 #include <utility>
 #include <vector>
 
+#if defined(PYBIND11_NUMPY_1_ONLY) && !defined(PYBIND11_INTERNAL_NUMPY_1_ONLY_DETECTED)
+#    error PYBIND11_NUMPY_1_ONLY must be defined before any pybind11 header is included.
+#endif
+
 /* This will be true on all flat address space platforms and allows us to reduce the
    whole npy_intp / ssize_t / Py_intptr_t business down to just ssize_t for all size
    and dimension types (e.g. shape, strides, indexing), instead of inflicting this
-   upon the library user. */
+   upon the library user.
+   Note that NumPy 2 now uses ssize_t for `npy_intp` to simplify this. */
 static_assert(sizeof(::pybind11::ssize_t) == sizeof(Py_intptr_t), "ssize_t != Py_intptr_t");
 static_assert(std::is_signed<Py_intptr_t>::value, "Py_intptr_t must be signed");
 // We now can reinterpret_cast between py::ssize_t and Py_intptr_t (MSVC + PyPy cares)
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 PYBIND11_WARNING_DISABLE_MSVC(4127)
 
+class dtype; // Forward declaration
 class array; // Forward declaration
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <>
+struct handle_type_name<dtype> {
+    static constexpr auto name = const_name("numpy.dtype");
+};
+
+template <>
 struct handle_type_name<array> {
     static constexpr auto name = const_name("numpy.ndarray");
 };
 
 template <typename type, typename SFINAE = void>
 struct npy_format_descriptor;
 
-struct PyArrayDescr_Proxy {
+/* NumPy 1 proxy (always includes legacy fields) */
+struct PyArrayDescr1_Proxy {
     PyObject_HEAD
     PyObject *typeobj;
     char kind;
     char type;
     char byteorder;
     char flags;
     int type_num;
     int elsize;
     int alignment;
     char *subarray;
     PyObject *fields;
     PyObject *names;
 };
 
+#ifndef PYBIND11_NUMPY_1_ONLY
+struct PyArrayDescr_Proxy {
+    PyObject_HEAD
+    PyObject *typeobj;
+    char kind;
+    char type;
+    char byteorder;
+    char _former_flags;
+    int type_num;
+    /* Additional fields are NumPy version specific. */
+};
+#else
+/* NumPy 1.x only, we can expose all fields */
+using PyArrayDescr_Proxy = PyArrayDescr1_Proxy;
+#endif
+
+/* NumPy 2 proxy, including legacy fields */
+struct PyArrayDescr2_Proxy {
+    PyObject_HEAD
+    PyObject *typeobj;
+    char kind;
+    char type;
+    char byteorder;
+    char _former_flags;
+    int type_num;
+    std::uint64_t flags;
+    ssize_t elsize;
+    ssize_t alignment;
+    PyObject *metadata;
+    Py_hash_t hash;
+    void *reserved_null[2];
+    /* The following fields only exist if 0 <= type_num < 2056 */
+    char *subarray;
+    PyObject *fields;
+    PyObject *names;
+};
+
 struct PyArray_Proxy {
     PyObject_HEAD
     char *data;
     int nd;
     ssize_t *dimensions;
     ssize_t *strides;
     PyObject *base;
@@ -116,14 +168,36 @@
     static numpy_internals *ptr = nullptr;
     if (!ptr) {
         load_numpy_internals(ptr);
     }
     return *ptr;
 }
 
+PYBIND11_NOINLINE module_ import_numpy_core_submodule(const char *submodule_name) {
+    module_ numpy = module_::import("numpy");
+    str version_string = numpy.attr("__version__");
+
+    module_ numpy_lib = module_::import("numpy.lib");
+    object numpy_version = numpy_lib.attr("NumpyVersion")(version_string);
+    int major_version = numpy_version.attr("major").cast<int>();
+
+#ifdef PYBIND11_NUMPY_1_ONLY
+    if (major_version >= 2) {
+        throw std::runtime_error(
+            "This extension was built with PYBIND11_NUMPY_1_ONLY defined, "
+            "but NumPy 2 is used in this process. For NumPy2 compatibility, "
+            "this extension needs to be rebuilt without the PYBIND11_NUMPY_1_ONLY define.");
+    }
+#endif
+    /* `numpy.core` was renamed to `numpy._core` in NumPy 2.0 as it officially
+        became a private module. */
+    std::string numpy_core_path = major_version >= 2 ? "numpy._core" : "numpy.core";
+    return module_::import((numpy_core_path + "." + submodule_name).c_str());
+}
+
 template <typename T>
 struct same_size {
     template <typename U>
     using as = bool_constant<sizeof(T) == sizeof(U)>;
 };
 
 template <typename Concrete>
@@ -182,22 +256,24 @@
         NPY_INT64_
         = platform_lookup<std::int64_t, long, long long, int>(NPY_LONG_, NPY_LONGLONG_, NPY_INT_),
         NPY_UINT64_
         = platform_lookup<std::uint64_t, unsigned long, unsigned long long, unsigned int>(
             NPY_ULONG_, NPY_ULONGLONG_, NPY_UINT_),
     };
 
+    unsigned int PyArray_RUNTIME_VERSION_;
+
     struct PyArray_Dims {
         Py_intptr_t *ptr;
         int len;
     };
 
     static npy_api &get() {
-        static npy_api api = lookup();
-        return api;
+        PYBIND11_CONSTINIT static gil_safe_call_once_and_store<npy_api> storage;
+        return storage.call_once_and_store_result(lookup).get_stored();
     }
 
     bool PyArray_Check_(PyObject *obj) const {
         return PyObject_TypeCheck(obj, PyArray_Type_) != 0;
     }
     bool PyArrayDescr_Check_(PyObject *obj) const {
         return PyObject_TypeCheck(obj, PyArrayDescr_Type_) != 0;
@@ -220,22 +296,24 @@
     PyTypeObject *PyArray_Type_;
     PyTypeObject *PyVoidArrType_Type_;
     PyTypeObject *PyArrayDescr_Type_;
     PyObject *(*PyArray_DescrFromScalar_)(PyObject *);
     PyObject *(*PyArray_FromAny_)(PyObject *, PyObject *, int, int, int, PyObject *);
     int (*PyArray_DescrConverter_)(PyObject *, PyObject **);
     bool (*PyArray_EquivTypes_)(PyObject *, PyObject *);
+#ifdef PYBIND11_NUMPY_1_ONLY
     int (*PyArray_GetArrayParamsFromObject_)(PyObject *,
                                              PyObject *,
                                              unsigned char,
                                              PyObject **,
                                              int *,
                                              Py_intptr_t *,
                                              PyObject **,
                                              PyObject *);
+#endif
     PyObject *(*PyArray_Squeeze_)(PyObject *);
     // Unused. Not removed because that affects ABI of the class.
     int (*PyArray_SetBaseObject_)(PyObject *, PyObject *);
     PyObject *(*PyArray_Resize_)(PyObject *, PyArray_Dims *, int, int);
     PyObject *(*PyArray_Newshape_)(PyObject *, PyArray_Dims *, int);
     PyObject *(*PyArray_View_)(PyObject *, PyObject *, PyObject *);
 
@@ -245,35 +323,43 @@
         API_PyArray_Type = 2,
         API_PyArrayDescr_Type = 3,
         API_PyVoidArrType_Type = 39,
         API_PyArray_DescrFromType = 45,
         API_PyArray_DescrFromScalar = 57,
         API_PyArray_FromAny = 69,
         API_PyArray_Resize = 80,
-        API_PyArray_CopyInto = 82,
+        // CopyInto was slot 82 and 50 was effectively an alias. NumPy 2 removed 82.
+        API_PyArray_CopyInto = 50,
         API_PyArray_NewCopy = 85,
         API_PyArray_NewFromDescr = 94,
         API_PyArray_DescrNewFromType = 96,
         API_PyArray_Newshape = 135,
         API_PyArray_Squeeze = 136,
         API_PyArray_View = 137,
         API_PyArray_DescrConverter = 174,
         API_PyArray_EquivTypes = 182,
+#ifdef PYBIND11_NUMPY_1_ONLY
         API_PyArray_GetArrayParamsFromObject = 278,
+#endif
         API_PyArray_SetBaseObject = 282
     };
 
     static npy_api lookup() {
-        module_ m = module_::import("numpy.core.multiarray");
+        module_ m = detail::import_numpy_core_submodule("multiarray");
         auto c = m.attr("_ARRAY_API");
         void **api_ptr = (void **) PyCapsule_GetPointer(c.ptr(), nullptr);
+        if (api_ptr == nullptr) {
+            raise_from(PyExc_SystemError, "FAILURE obtaining numpy _ARRAY_API pointer.");
+            throw error_already_set();
+        }
         npy_api api;
 #define DECL_NPY_API(Func) api.Func##_ = (decltype(api.Func##_)) api_ptr[API_##Func];
         DECL_NPY_API(PyArray_GetNDArrayCFeatureVersion);
-        if (api.PyArray_GetNDArrayCFeatureVersion_() < 0x7) {
+        api.PyArray_RUNTIME_VERSION_ = api.PyArray_GetNDArrayCFeatureVersion_();
+        if (api.PyArray_RUNTIME_VERSION_ < 0x7) {
             pybind11_fail("pybind11 numpy support requires numpy >= 1.7.0");
         }
         DECL_NPY_API(PyArray_Type);
         DECL_NPY_API(PyVoidArrType_Type);
         DECL_NPY_API(PyArrayDescr_Type);
         DECL_NPY_API(PyArray_DescrFromType);
         DECL_NPY_API(PyArray_DescrFromScalar);
@@ -284,15 +370,17 @@
         DECL_NPY_API(PyArray_NewFromDescr);
         DECL_NPY_API(PyArray_DescrNewFromType);
         DECL_NPY_API(PyArray_Newshape);
         DECL_NPY_API(PyArray_Squeeze);
         DECL_NPY_API(PyArray_View);
         DECL_NPY_API(PyArray_DescrConverter);
         DECL_NPY_API(PyArray_EquivTypes);
+#ifdef PYBIND11_NUMPY_1_ONLY
         DECL_NPY_API(PyArray_GetArrayParamsFromObject);
+#endif
         DECL_NPY_API(PyArray_SetBaseObject);
 
 #undef DECL_NPY_API
         return api;
     }
 };
 
@@ -306,14 +394,22 @@
     return reinterpret_cast<PyArrayDescr_Proxy *>(ptr);
 }
 
 inline const PyArrayDescr_Proxy *array_descriptor_proxy(const PyObject *ptr) {
     return reinterpret_cast<const PyArrayDescr_Proxy *>(ptr);
 }
 
+inline const PyArrayDescr1_Proxy *array_descriptor1_proxy(const PyObject *ptr) {
+    return reinterpret_cast<const PyArrayDescr1_Proxy *>(ptr);
+}
+
+inline const PyArrayDescr2_Proxy *array_descriptor2_proxy(const PyObject *ptr) {
+    return reinterpret_cast<const PyArrayDescr2_Proxy *>(ptr);
+}
+
 inline bool check_flags(const void *ptr, int flag) {
     return (flag == (array_proxy(ptr)->flags & flag));
 }
 
 template <typename T>
 struct is_std_array : std::false_type {};
 template <typename T, size_t N>
@@ -346,15 +442,15 @@
     // appends the extents to shape
     static void append_extents(list &shape) {
         shape.append(N);
         array_info<T>::append_extents(shape);
     }
 
     static constexpr auto extents = const_name<array_info<T>::is_array>(
-        concat(const_name<N>(), array_info<T>::extents), const_name<N>());
+        ::pybind11::detail::concat(const_name<N>(), array_info<T>::extents), const_name<N>());
 };
 // For numpy we have special handling for arrays of characters, so we don't include
 // the size in the array extents.
 template <size_t N>
 struct array_info<char[N]> : array_info_scalar<char[N]> {};
 template <size_t N>
 struct array_info<std::array<char, N>> : array_info_scalar<std::array<char, N>> {};
@@ -585,18 +681,40 @@
     /// Return dtype associated with a C++ type.
     template <typename T>
     static dtype of() {
         return detail::npy_format_descriptor<typename std::remove_cv<T>::type>::dtype();
     }
 
     /// Size of the data type in bytes.
+#ifdef PYBIND11_NUMPY_1_ONLY
     ssize_t itemsize() const { return detail::array_descriptor_proxy(m_ptr)->elsize; }
+#else
+    ssize_t itemsize() const {
+        if (detail::npy_api::get().PyArray_RUNTIME_VERSION_ < 0x12) {
+            return detail::array_descriptor1_proxy(m_ptr)->elsize;
+        }
+        return detail::array_descriptor2_proxy(m_ptr)->elsize;
+    }
+#endif
 
     /// Returns true for structured data types.
+#ifdef PYBIND11_NUMPY_1_ONLY
     bool has_fields() const { return detail::array_descriptor_proxy(m_ptr)->names != nullptr; }
+#else
+    bool has_fields() const {
+        if (detail::npy_api::get().PyArray_RUNTIME_VERSION_ < 0x12) {
+            return detail::array_descriptor1_proxy(m_ptr)->names != nullptr;
+        }
+        const auto *proxy = detail::array_descriptor2_proxy(m_ptr);
+        if (proxy->type_num < 0 || proxy->type_num >= 2056) {
+            return false;
+        }
+        return proxy->names != nullptr;
+    }
+#endif
 
     /// Single-character code for dtype's kind.
     /// For example, floating point types are 'f' and integral types are 'i'.
     char kind() const { return detail::array_descriptor_proxy(m_ptr)->kind; }
 
     /// Single-character for dtype's type.
     /// For example, ``float`` is 'f', ``double`` 'd', ``int`` 'i', and ``long`` 'l'.
@@ -614,28 +732,47 @@
         // C API (``PyArray_Descr::type_num``).
         return detail::array_descriptor_proxy(m_ptr)->type_num;
     }
 
     /// Single character for byteorder
     char byteorder() const { return detail::array_descriptor_proxy(m_ptr)->byteorder; }
 
-    /// Alignment of the data type
+/// Alignment of the data type
+#ifdef PYBIND11_NUMPY_1_ONLY
     int alignment() const { return detail::array_descriptor_proxy(m_ptr)->alignment; }
+#else
+    ssize_t alignment() const {
+        if (detail::npy_api::get().PyArray_RUNTIME_VERSION_ < 0x12) {
+            return detail::array_descriptor1_proxy(m_ptr)->alignment;
+        }
+        return detail::array_descriptor2_proxy(m_ptr)->alignment;
+    }
+#endif
 
-    /// Flags for the array descriptor
+/// Flags for the array descriptor
+#ifdef PYBIND11_NUMPY_1_ONLY
     char flags() const { return detail::array_descriptor_proxy(m_ptr)->flags; }
+#else
+    std::uint64_t flags() const {
+        if (detail::npy_api::get().PyArray_RUNTIME_VERSION_ < 0x12) {
+            return (unsigned char) detail::array_descriptor1_proxy(m_ptr)->flags;
+        }
+        return detail::array_descriptor2_proxy(m_ptr)->flags;
+    }
+#endif
 
 private:
-    static object _dtype_from_pep3118() {
-        static PyObject *obj = module_::import("numpy.core._internal")
-                                   .attr("_dtype_from_pep3118")
-                                   .cast<object>()
-                                   .release()
-                                   .ptr();
-        return reinterpret_borrow<object>(obj);
+    static object &_dtype_from_pep3118() {
+        PYBIND11_CONSTINIT static gil_safe_call_once_and_store<object> storage;
+        return storage
+            .call_once_and_store_result([]() {
+                return detail::import_numpy_core_submodule("_internal")
+                    .attr("_dtype_from_pep3118");
+            })
+            .get_stored();
     }
 
     dtype strip_padding(ssize_t itemsize) {
         // Recursively strip all void fields with empty names that are generated for
         // padding fields (as of NumPy v1.11).
         if (!has_fields()) {
             return *this;
@@ -784,17 +921,15 @@
 
     /// Total number of elements
     ssize_t size() const {
         return std::accumulate(shape(), shape() + ndim(), (ssize_t) 1, std::multiplies<ssize_t>());
     }
 
     /// Byte size of a single element
-    ssize_t itemsize() const {
-        return detail::array_descriptor_proxy(detail::array_proxy(m_ptr)->descr)->elsize;
-    }
+    ssize_t itemsize() const { return dtype().itemsize(); }
 
     /// Total number of bytes
     ssize_t nbytes() const { return size() * itemsize(); }
 
     /// Number of dimensions
     ssize_t ndim() const { return detail::array_proxy(m_ptr)->nd; }
 
@@ -1004,15 +1139,15 @@
         }
         check_dimensions_impl(axis + 1, shape + 1, index...);
     }
 
     /// Create array from any object -- always returns a new reference
     static PyObject *raw_array(PyObject *ptr, int ExtraFlags = 0) {
         if (ptr == nullptr) {
-            PyErr_SetString(PyExc_ValueError, "cannot create a pybind11::array from a nullptr");
+            set_error(PyExc_ValueError, "cannot create a pybind11::array from a nullptr");
             return nullptr;
         }
         return detail::npy_api::get().PyArray_FromAny_(
             ptr, nullptr, 0, 0, detail::npy_api::NPY_ARRAY_ENSUREARRAY_ | ExtraFlags, nullptr);
     }
 };
 
@@ -1151,15 +1286,15 @@
                && detail::check_flags(h.ptr(), ExtraFlags & (array::c_style | array::f_style));
     }
 
 protected:
     /// Create array from any object -- always returns a new reference
     static PyObject *raw_array_t(PyObject *ptr) {
         if (ptr == nullptr) {
-            PyErr_SetString(PyExc_ValueError, "cannot create a pybind11::array_t from a nullptr");
+            set_error(PyExc_ValueError, "cannot create a pybind11::array_t from a nullptr");
             return nullptr;
         }
         return detail::npy_api::get().PyArray_FromAny_(ptr,
                                                        dtype::of<T>().release().ptr(),
                                                        0,
                                                        0,
                                                        detail::npy_api::NPY_ARRAY_ENSUREARRAY_
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/operators.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/options.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/pybind11.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/pybind11.h`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 #pragma once
 
 #include "detail/class.h"
 #include "detail/init.h"
 #include "attr.h"
 #include "gil.h"
+#include "gil_safe_call_once.h"
 #include "options.h"
+#include "typing.h"
 
 #include <cstdlib>
 #include <cstring>
 #include <memory>
 #include <new>
 #include <string>
 #include <utility>
@@ -48,14 +50,55 @@
 PYBIND11_WARNING_DISABLE_GCC("-Wnoexcept-type")
 #endif
 
 PYBIND11_WARNING_DISABLE_MSVC(4127)
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
+inline std::string replace_newlines_and_squash(const char *text) {
+    const char *whitespaces = " \t\n\r\f\v";
+    std::string result(text);
+    bool previous_is_whitespace = false;
+
+    if (result.size() >= 2) {
+        // Do not modify string representations
+        char first_char = result[0];
+        char last_char = result[result.size() - 1];
+        if (first_char == last_char && first_char == '\'') {
+            return result;
+        }
+    }
+    result.clear();
+
+    // Replace characters in whitespaces array with spaces and squash consecutive spaces
+    while (*text != '\0') {
+        if (std::strchr(whitespaces, *text)) {
+            if (!previous_is_whitespace) {
+                result += ' ';
+                previous_is_whitespace = true;
+            }
+        } else {
+            result += *text;
+            previous_is_whitespace = false;
+        }
+        ++text;
+    }
+
+    // Strip leading and trailing whitespaces
+    const size_t str_begin = result.find_first_not_of(whitespaces);
+    if (str_begin == std::string::npos) {
+        return "";
+    }
+
+    const size_t str_end = result.find_last_not_of(whitespaces);
+    const size_t str_range = str_end - str_begin + 1;
+
+    return result.substr(str_begin, str_range);
+}
+
 // Apply all the extensions translators from a list
 // Return true if one of the translators completed without raising an exception
 // itself. Return of false indicates that if there are other translators
 // available, they should be tried.
 inline bool apply_exception_translators(std::forward_list<ExceptionTranslator> &translators) {
     auto last_exception = std::current_exception();
 
@@ -420,15 +463,15 @@
                     signature += "arg" + std::to_string(arg_index - (rec->is_method ? 1 : 0));
                 }
                 signature += ": ";
             } else if (c == '}') {
                 // Write default value if available.
                 if (!is_starred && arg_index < rec->args.size() && rec->args[arg_index].descr) {
                     signature += " = ";
-                    signature += rec->args[arg_index].descr;
+                    signature += detail::replace_newlines_and_squash(rec->args[arg_index].descr);
                 }
                 // Separator for positional-only arguments (placed after the
                 // argument, rather than before like *
                 if (rec->nargs_pos_only > 0 && (arg_index + 1) == rec->nargs_pos_only) {
                     signature += ", /";
                 }
                 if (!is_starred) {
@@ -445,17 +488,15 @@
                                  + th.attr("__qualname__").cast<std::string>();
                 } else if (rec->is_new_style_constructor && arg_index == 0) {
                     // A new-style `__init__` takes `self` as `value_and_holder`.
                     // Rewrite it to the proper class type.
                     signature += rec->scope.attr("__module__").cast<std::string>() + "."
                                  + rec->scope.attr("__qualname__").cast<std::string>();
                 } else {
-                    std::string tname(t->name());
-                    detail::clean_type_id(tname);
-                    signature += tname;
+                    signature += detail::quote_cpp_type_name(detail::clean_type_id(t->name()));
                 }
             } else {
                 signature += c;
             }
         }
 
         if (arg_index != args - rec->has_args - rec->has_kwargs || types[type_index] != nullptr) {
@@ -676,31 +717,30 @@
     static PyObject *dispatcher(PyObject *self, PyObject *args_in, PyObject *kwargs_in) {
         using namespace detail;
         assert(isinstance<capsule>(self));
 
         /* Iterator over the list of potentially admissible overloads */
         const function_record *overloads = reinterpret_cast<function_record *>(
                                   PyCapsule_GetPointer(self, get_function_record_capsule_name())),
-                              *it = overloads;
+                              *current_overload = overloads;
         assert(overloads != nullptr);
 
         /* Need to know how many arguments + keyword arguments there are to pick the right
            overload */
         const auto n_args_in = (size_t) PyTuple_GET_SIZE(args_in);
 
         handle parent = n_args_in > 0 ? PyTuple_GET_ITEM(args_in, 0) : nullptr,
                result = PYBIND11_TRY_NEXT_OVERLOAD;
 
         auto self_value_and_holder = value_and_holder();
         if (overloads->is_constructor) {
             if (!parent
                 || !PyObject_TypeCheck(parent.ptr(), (PyTypeObject *) overloads->scope.ptr())) {
-                PyErr_SetString(
-                    PyExc_TypeError,
-                    "__init__(self, ...) called with invalid or missing `self` argument");
+                set_error(PyExc_TypeError,
+                          "__init__(self, ...) called with invalid or missing `self` argument");
                 return nullptr;
             }
 
             auto *const tinfo = get_type_info((PyTypeObject *) overloads->scope.ptr());
             auto *const pi = reinterpret_cast<instance *>(parent.ptr());
             self_value_and_holder = pi->get_value_and_holder(tinfo, true);
 
@@ -715,17 +755,18 @@
             // We do this in two passes: in the first pass, we load arguments with `convert=false`;
             // in the second, we allow conversion (except for arguments with an explicit
             // py::arg().noconvert()).  This lets us prefer calls without conversion, with
             // conversion as a fallback.
             std::vector<function_call> second_pass;
 
             // However, if there are no overloads, we can just skip the no-convert pass entirely
-            const bool overloaded = it != nullptr && it->next != nullptr;
+            const bool overloaded
+                = current_overload != nullptr && current_overload->next != nullptr;
 
-            for (; it != nullptr; it = it->next) {
+            for (; current_overload != nullptr; current_overload = current_overload->next) {
 
                 /* For each overload:
                    1. Copy all positional arguments we were given, also checking to make sure that
                       named positional arguments weren't *also* specified via kwarg.
                    2. If we weren't given enough, try to make up the omitted ones by checking
                       whether they were provided by a kwarg matching the `py::arg("name")` name. If
                       so, use it (and remove it from kwargs); if not, see if the function binding
@@ -738,15 +779,15 @@
                       extra tuple or dict at the end of the positional arguments.
                    6. Call the function call dispatcher (function_record::impl)
 
                    If one of these fail, move on to the next overload and keep trying until we get
                    a result other than PYBIND11_TRY_NEXT_OVERLOAD.
                  */
 
-                const function_record &func = *it;
+                const function_record &func = *current_overload;
                 size_t num_args = func.nargs; // Number of positional arguments that we need
                 if (func.has_args) {
                     --num_args; // (but don't count py::args
                 }
                 if (func.has_kwargs) {
                     --num_args; //  or py::kwargs)
                 }
@@ -976,18 +1017,18 @@
                         loader_life_support guard{};
                         result = call.func.impl(call);
                     } catch (reference_cast_error &) {
                         result = PYBIND11_TRY_NEXT_OVERLOAD;
                     }
 
                     if (result.ptr() != PYBIND11_TRY_NEXT_OVERLOAD) {
-                        // The error reporting logic below expects 'it' to be valid, as it would be
-                        // if we'd encountered this failure in the first-pass loop.
+                        // The error reporting logic below expects 'current_overload' to be valid,
+                        // as it would be if we'd encountered this failure in the first-pass loop.
                         if (!result) {
-                            it = &call.func;
+                            current_overload = &call.func;
                         }
                         break;
                     }
                 }
             }
         } catch (error_already_set &e) {
             e.restore();
@@ -1003,15 +1044,15 @@
                registration. If none of the module-locale translators handle
                the exception (or there are no module-locale translators) then
                the global translators will be tried, also in reverse order of
                registration.
 
                A translator may choose to do one of the following:
 
-                - catch the exception and call PyErr_SetString or PyErr_SetObject
+                - catch the exception and call py::set_error()
                   to set a standard (or custom) Python exception, or
                 - do nothing and let the exception fall through to the next translator, or
                 - delegate translation to the next translator by throwing a new type of exception.
              */
 
             auto &local_exception_translators
                 = get_local_internals().registered_exception_translators;
@@ -1019,16 +1060,15 @@
                 return nullptr;
             }
             auto &exception_translators = get_internals().registered_exception_translators;
             if (detail::apply_exception_translators(exception_translators)) {
                 return nullptr;
             }
 
-            PyErr_SetString(PyExc_SystemError,
-                            "Exception escaped from default exception translator!");
+            set_error(PyExc_SystemError, "Exception escaped from default exception translator!");
             return nullptr;
         }
 
         auto append_note_if_missing_header_is_suspected = [](std::string &msg) {
             if (msg.find("std::") != std::string::npos) {
                 msg += "\n\n"
                        "Did you forget to `#include <pybind11/stl.h>`? Or <pybind11/complex.h>,\n"
@@ -1098,15 +1138,15 @@
                 auto kwargs = reinterpret_borrow<dict>(kwargs_in);
                 if (!kwargs.empty()) {
                     if (some_args) {
                         msg += "; ";
                     }
                     msg += "kwargs: ";
                     bool first = true;
-                    for (auto kwarg : kwargs) {
+                    for (const auto &kwarg : kwargs) {
                         if (first) {
                             first = false;
                         } else {
                             msg += ", ";
                         }
                         msg += pybind11::str("{}=").format(kwarg.first);
                         try {
@@ -1121,38 +1161,48 @@
             append_note_if_missing_header_is_suspected(msg);
             // Attach additional error info to the exception if supported
             if (PyErr_Occurred()) {
                 // #HelpAppreciated: unit test coverage for this branch.
                 raise_from(PyExc_TypeError, msg.c_str());
                 return nullptr;
             }
-            PyErr_SetString(PyExc_TypeError, msg.c_str());
+            set_error(PyExc_TypeError, msg.c_str());
             return nullptr;
         }
         if (!result) {
             std::string msg = "Unable to convert function return value to a "
                               "Python type! The signature was\n\t";
-            msg += it->signature;
+            assert(current_overload != nullptr);
+            msg += current_overload->signature;
             append_note_if_missing_header_is_suspected(msg);
             // Attach additional error info to the exception if supported
             if (PyErr_Occurred()) {
                 raise_from(PyExc_TypeError, msg.c_str());
                 return nullptr;
             }
-            PyErr_SetString(PyExc_TypeError, msg.c_str());
+            set_error(PyExc_TypeError, msg.c_str());
             return nullptr;
         }
         if (overloads->is_constructor && !self_value_and_holder.holder_constructed()) {
             auto *pi = reinterpret_cast<instance *>(parent.ptr());
             self_value_and_holder.type->init_instance(pi, nullptr);
         }
         return result.ptr();
     }
 };
 
+PYBIND11_NAMESPACE_BEGIN(detail)
+
+template <>
+struct handle_type_name<cpp_function> {
+    static constexpr auto name = const_name("Callable");
+};
+
+PYBIND11_NAMESPACE_END(detail)
+
 /// Wrapper for Python extension modules
 class module_ : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(module_, object, PyModule_Check)
 
     /// Create a new top-level Python module with the given name and docstring
     PYBIND11_DEPRECATED("Use PYBIND11_MODULE or module_::create_extension_module instead")
@@ -1272,14 +1322,23 @@
         // TODO: Should be reinterpret_steal for Python 3, but Python also steals it again when
         //       returned from PyInit_...
         //       For Python 2, reinterpret_borrow was correct.
         return reinterpret_borrow<module_>(m);
     }
 };
 
+PYBIND11_NAMESPACE_BEGIN(detail)
+
+template <>
+struct handle_type_name<module_> {
+    static constexpr auto name = const_name("module");
+};
+
+PYBIND11_NAMESPACE_END(detail)
+
 // When inside a namespace (or anywhere as long as it's not the first item on a line),
 // C++20 allows "module" to be used. This is provided for backward compatibility, and for
 // simplicity, if someone wants to use py::module for example, that is perfectly safe.
 using module = module_;
 
 /// \ingroup python_builtins
 /// Return a dictionary representing the global variables in the current execution frame,
@@ -1973,15 +2032,15 @@
         m_base.attr("name") = property(cpp_function(&enum_name, name("name"), is_method(m_base)));
 
         m_base.attr("__str__") = cpp_function(
             [](handle arg) -> str {
                 object type_name = type::handle_of(arg).attr("__name__");
                 return pybind11::str("{}.{}").format(std::move(type_name), enum_name(arg));
             },
-            name("name"),
+            name("__str__"),
             is_method(m_base));
 
         if (options::show_enum_members_docstring()) {
             m_base.attr("__doc__") = static_property(
                 cpp_function(
                     [](handle arg) -> std::string {
                         std::string docstring;
@@ -2391,92 +2450,104 @@
                     return Access()(s.it);
                     // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
                 },
                 std::forward<Extra>(extra)...,
                 Policy);
     }
 
-    return cast(state{first, last, true});
+    return cast(state{std::forward<Iterator>(first), std::forward<Sentinel>(last), true});
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 /// Makes a python iterator from a first and past-the-end C++ InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename ValueType = typename detail::iterator_access<Iterator>::result_type,
           typename... Extra>
-iterator make_iterator(Iterator first, Sentinel last, Extra &&...extra) {
+typing::Iterator<ValueType> make_iterator(Iterator first, Sentinel last, Extra &&...extra) {
     return detail::make_iterator_impl<detail::iterator_access<Iterator>,
                                       Policy,
                                       Iterator,
                                       Sentinel,
                                       ValueType,
-                                      Extra...>(first, last, std::forward<Extra>(extra)...);
+                                      Extra...>(std::forward<Iterator>(first),
+                                                std::forward<Sentinel>(last),
+                                                std::forward<Extra>(extra)...);
 }
 
 /// Makes a python iterator over the keys (`.first`) of a iterator over pairs from a
 /// first and past-the-end InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename KeyType = typename detail::iterator_key_access<Iterator>::result_type,
           typename... Extra>
-iterator make_key_iterator(Iterator first, Sentinel last, Extra &&...extra) {
+typing::Iterator<KeyType> make_key_iterator(Iterator first, Sentinel last, Extra &&...extra) {
     return detail::make_iterator_impl<detail::iterator_key_access<Iterator>,
                                       Policy,
                                       Iterator,
                                       Sentinel,
                                       KeyType,
-                                      Extra...>(first, last, std::forward<Extra>(extra)...);
+                                      Extra...>(std::forward<Iterator>(first),
+                                                std::forward<Sentinel>(last),
+                                                std::forward<Extra>(extra)...);
 }
 
 /// Makes a python iterator over the values (`.second`) of a iterator over pairs from a
 /// first and past-the-end InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
           typename ValueType = typename detail::iterator_value_access<Iterator>::result_type,
           typename... Extra>
-iterator make_value_iterator(Iterator first, Sentinel last, Extra &&...extra) {
+typing::Iterator<ValueType> make_value_iterator(Iterator first, Sentinel last, Extra &&...extra) {
     return detail::make_iterator_impl<detail::iterator_value_access<Iterator>,
                                       Policy,
                                       Iterator,
                                       Sentinel,
                                       ValueType,
-                                      Extra...>(first, last, std::forward<Extra>(extra)...);
+                                      Extra...>(std::forward<Iterator>(first),
+                                                std::forward<Sentinel>(last),
+                                                std::forward<Extra>(extra)...);
 }
 
 /// Makes an iterator over values of an stl container or other container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Type,
+          typename ValueType = typename detail::iterator_access<
+              decltype(std::begin(std::declval<Type &>()))>::result_type,
           typename... Extra>
-iterator make_iterator(Type &value, Extra &&...extra) {
+typing::Iterator<ValueType> make_iterator(Type &value, Extra &&...extra) {
     return make_iterator<Policy>(
         std::begin(value), std::end(value), std::forward<Extra>(extra)...);
 }
 
 /// Makes an iterator over the keys (`.first`) of a stl map-like container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Type,
+          typename KeyType = typename detail::iterator_key_access<
+              decltype(std::begin(std::declval<Type &>()))>::result_type,
           typename... Extra>
-iterator make_key_iterator(Type &value, Extra &&...extra) {
+typing::Iterator<KeyType> make_key_iterator(Type &value, Extra &&...extra) {
     return make_key_iterator<Policy>(
         std::begin(value), std::end(value), std::forward<Extra>(extra)...);
 }
 
 /// Makes an iterator over the values (`.second`) of a stl map-like container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Type,
+          typename ValueType = typename detail::iterator_value_access<
+              decltype(std::begin(std::declval<Type &>()))>::result_type,
           typename... Extra>
-iterator make_value_iterator(Type &value, Extra &&...extra) {
+typing::Iterator<ValueType> make_value_iterator(Type &value, Extra &&...extra) {
     return make_value_iterator<Policy>(
         std::begin(value), std::end(value), std::forward<Extra>(extra)...);
 }
 
 template <typename InputType, typename OutputType>
 void implicitly_convertible() {
     struct set_flag {
@@ -2524,15 +2595,15 @@
     detail::get_local_internals().registered_exception_translators.push_front(
         std::forward<ExceptionTranslator>(translator));
 }
 
 /**
  * Wrapper to generate a new Python exception type.
  *
- * This should only be used with PyErr_SetString for now.
+ * This should only be used with py::set_error() for now.
  * It is not (yet) possible to use as a py::base.
  * Template type argument is reserved for future use.
  */
 template <typename type>
 class exception : public object {
 public:
     exception() = default;
@@ -2545,50 +2616,48 @@
                           "definitions with name \""
                           + std::string(name) + "\"");
         }
         scope.attr(name) = *this;
     }
 
     // Sets the current python exception to this exception object with the given message
-    void operator()(const char *message) { PyErr_SetString(m_ptr, message); }
+    PYBIND11_DEPRECATED("Please use py::set_error() instead "
+                        "(https://github.com/pybind/pybind11/pull/4772)")
+    void operator()(const char *message) const { set_error(*this, message); }
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
-// Returns a reference to a function-local static exception object used in the simple
-// register_exception approach below.  (It would be simpler to have the static local variable
-// directly in register_exception, but that makes clang <3.5 segfault - issue #1349).
-template <typename CppException>
-exception<CppException> &get_exception_object() {
-    static exception<CppException> ex;
-    return ex;
-}
+
+template <>
+struct handle_type_name<exception<void>> {
+    static constexpr auto name = const_name("Exception");
+};
 
 // Helper function for register_exception and register_local_exception
 template <typename CppException>
 exception<CppException> &
 register_exception_impl(handle scope, const char *name, handle base, bool isLocal) {
-    auto &ex = detail::get_exception_object<CppException>();
-    if (!ex) {
-        ex = exception<CppException>(scope, name, base);
-    }
+    PYBIND11_CONSTINIT static gil_safe_call_once_and_store<exception<CppException>> exc_storage;
+    exc_storage.call_once_and_store_result(
+        [&]() { return exception<CppException>(scope, name, base); });
 
     auto register_func
         = isLocal ? &register_local_exception_translator : &register_exception_translator;
 
     register_func([](std::exception_ptr p) {
         if (!p) {
             return;
         }
         try {
             std::rethrow_exception(p);
         } catch (const CppException &e) {
-            detail::get_exception_object<CppException>()(e.what());
+            set_error(exc_storage.get_stored(), e.what());
         }
     });
-    return ex;
+    return exc_storage.get_stored();
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 /**
  * Registers a Python exception in `m` of the given `name` and installs a translator to
  * translate the C++ exception to the created Python exception using the what() method.
@@ -2699,15 +2768,19 @@
     PyFrameObject *frame = PyThreadState_GetFrame(PyThreadState_Get());
     if (frame != nullptr) {
         PyCodeObject *f_code = PyFrame_GetCode(frame);
         // f_code is guaranteed to not be NULL
         if ((std::string) str(f_code->co_name) == name && f_code->co_argcount > 0) {
             PyObject *locals = PyEval_GetLocals();
             if (locals != nullptr) {
+#        if PY_VERSION_HEX >= 0x030b0000
+                PyObject *co_varnames = PyCode_GetVarnames(f_code);
+#        else
                 PyObject *co_varnames = PyObject_GetAttrString((PyObject *) f_code, "co_varnames");
+#        endif
                 PyObject *self_arg = PyTuple_GET_ITEM(co_varnames, 0);
                 Py_DECREF(co_varnames);
                 PyObject *self_caller = dict_getitem(locals, self_arg);
                 if (self_caller == self.ptr()) {
                     Py_DECREF(f_code);
                     Py_DECREF(frame);
                     return function();
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/pytypes.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/pytypes.h`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 struct obj_attr;
 struct str_attr;
 struct generic_item;
 struct sequence_item;
 struct list_item;
 struct tuple_item;
 } // namespace accessor_policies
+// PLEASE KEEP handle_type_name SPECIALIZATIONS IN SYNC.
 using obj_attr_accessor = accessor<accessor_policies::obj_attr>;
 using str_attr_accessor = accessor<accessor_policies::str_attr>;
 using item_accessor = accessor<accessor_policies::generic_item>;
 using sequence_accessor = accessor<accessor_policies::sequence_item>;
 using list_accessor = accessor<accessor_policies::list_item>;
 using tuple_accessor = accessor<accessor_policies::tuple_item>;
 
@@ -301,27 +302,27 @@
     void throw_gilstate_error(const std::string &function_name) const {
         fprintf(
             stderr,
             "%s is being called while the GIL is either not held or invalid. Please see "
             "https://pybind11.readthedocs.io/en/stable/advanced/"
             "misc.html#common-sources-of-global-interpreter-lock-errors for debugging advice.\n"
             "If you are convinced there is no bug in your code, you can #define "
-            "PYBIND11_NO_ASSERT_GIL_HELD_INCREF_DECREF"
+            "PYBIND11_NO_ASSERT_GIL_HELD_INCREF_DECREF "
             "to disable this check. In that case you have to ensure this #define is consistently "
             "used for all translation units linked into a given pybind11 extension, otherwise "
             "there will be ODR violations.",
             function_name.c_str());
-        fflush(stderr);
         if (Py_TYPE(m_ptr)->tp_name != nullptr) {
             fprintf(stderr,
-                    "The failing %s call was triggered on a %s object.\n",
+                    " The failing %s call was triggered on a %s object.",
                     function_name.c_str(),
                     Py_TYPE(m_ptr)->tp_name);
-            fflush(stderr);
         }
+        fprintf(stderr, "\n");
+        fflush(stderr);
         throw std::runtime_error(function_name + " PyGILState_Check() failure.");
     }
 #endif
 
 #ifdef PYBIND11_HANDLE_REF_DEBUG
     static std::size_t inc_ref_counter(std::size_t add) {
         thread_local std::size_t counter = 0;
@@ -330,14 +331,22 @@
     }
 
 public:
     static std::size_t inc_ref_counter() { return inc_ref_counter(0); }
 #endif
 };
 
+inline void set_error(const handle &type, const char *message) {
+    PyErr_SetString(type.ptr(), message);
+}
+
+inline void set_error(const handle &type, const handle &value) {
+    PyErr_SetObject(type.ptr(), value.ptr());
+}
+
 /** \rst
     Holds a reference to a Python object (with reference counting)
 
     Like `handle`, the `object` class is a thin wrapper around an arbitrary Python
     object (i.e. a ``PyObject *`` in Python's C API). In contrast to `handle`, it
     optionally increases the object's reference count upon construction, and it
     *always* decreases the reference count when the `object` instance goes out of
@@ -1608,15 +1617,23 @@
 };
 /// @} pytypes
 
 inline namespace literals {
 /** \rst
     String literal version of `str`
  \endrst */
-inline str operator"" _s(const char *s, size_t size) { return {s, size}; }
+inline str
+#if !defined(__clang__) && defined(__GNUC__) && __GNUC__ < 5
+operator"" _s // gcc 4.8.5 insists on having a space (hard error).
+#else
+operator""_s // clang 17 generates a deprecation warning if there is a space.
+#endif
+    (const char *s, size_t size) {
+    return {s, size};
+}
 } // namespace literals
 
 /// \addtogroup pytypes
 /// @{
 class bytes : public object {
 public:
     PYBIND11_OBJECT(bytes, object, PYBIND11_BYTES_CHECK)
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/stl/filesystem.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/stl.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/stl.h`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             if (!value_ || !s.add(std::move(value_))) {
                 return handle();
             }
         }
         return s.release();
     }
 
-    PYBIND11_TYPE_CASTER(type, const_name("Set[") + key_conv::name + const_name("]"));
+    PYBIND11_TYPE_CASTER(type, const_name("set[") + key_conv::name + const_name("]"));
 };
 
 template <typename Type, typename Key, typename Value>
 struct map_caster {
     using key_conv = make_caster<Key>;
     using value_conv = make_caster<Value>;
 
@@ -153,30 +153,30 @@
             }
             d[std::move(key)] = std::move(value);
         }
         return d.release();
     }
 
     PYBIND11_TYPE_CASTER(Type,
-                         const_name("Dict[") + key_conv::name + const_name(", ") + value_conv::name
+                         const_name("dict[") + key_conv::name + const_name(", ") + value_conv::name
                              + const_name("]"));
 };
 
 template <typename Type, typename Value>
 struct list_caster {
     using value_conv = make_caster<Value>;
 
     bool load(handle src, bool convert) {
         if (!isinstance<sequence>(src) || isinstance<bytes>(src) || isinstance<str>(src)) {
             return false;
         }
         auto s = reinterpret_borrow<sequence>(src);
         value.clear();
         reserve_maybe(s, &value);
-        for (auto it : s) {
+        for (const auto &it : s) {
             value_conv conv;
             if (!conv.load(it, convert)) {
                 return false;
             }
             value.push_back(cast_op<Value &&>(std::move(conv)));
         }
         return true;
@@ -204,15 +204,15 @@
                 return handle();
             }
             PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
 
-    PYBIND11_TYPE_CASTER(Type, const_name("List[") + value_conv::name + const_name("]"));
+    PYBIND11_TYPE_CASTER(Type, const_name("list[") + value_conv::name + const_name("]"));
 };
 
 template <typename Type, typename Alloc>
 struct type_caster<std::vector<Type, Alloc>> : list_caster<std::vector<Type, Alloc>, Type> {};
 
 template <typename Type, typename Alloc>
 struct type_caster<std::deque<Type, Alloc>> : list_caster<std::deque<Type, Alloc>, Type> {};
@@ -243,15 +243,15 @@
             return false;
         }
         auto l = reinterpret_borrow<sequence>(src);
         if (!require_size(l.size())) {
             return false;
         }
         size_t ctr = 0;
-        for (auto it : l) {
+        for (const auto &it : l) {
             value_conv conv;
             if (!conv.load(it, convert)) {
                 return false;
             }
             value[ctr++] = cast_op<Value &&>(std::move(conv));
         }
         return true;
@@ -270,15 +270,15 @@
             PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
 
     PYBIND11_TYPE_CASTER(ArrayType,
                          const_name<Resizable>(const_name(""), const_name("Annotated["))
-                             + const_name("List[") + value_conv::name + const_name("]")
+                             + const_name("list[") + value_conv::name + const_name("]")
                              + const_name<Resizable>(const_name(""),
                                                      const_name(", FixedSize(")
                                                          + const_name<Size>() + const_name(")]")));
 };
 
 template <typename Type, size_t Size>
 struct type_caster<std::array<Type, Size>>
@@ -417,15 +417,16 @@
     static handle cast(Variant &&src, return_value_policy policy, handle parent) {
         return visit_helper<V>::call(variant_caster_visitor{policy, parent},
                                      std::forward<Variant>(src));
     }
 
     using Type = V<Ts...>;
     PYBIND11_TYPE_CASTER(Type,
-                         const_name("Union[") + detail::concat(make_caster<Ts>::name...)
+                         const_name("Union[")
+                             + ::pybind11::detail::concat(make_caster<Ts>::name...)
                              + const_name("]"));
 };
 
 #if defined(PYBIND11_HAS_VARIANT)
 template <typename... Ts>
 struct type_caster<std::variant<Ts...>> : variant_caster<std::variant<Ts...>> {};
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/stl_bind.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/stl_bind.h`

 * *Files 6% similar despite different names*

```diff
@@ -521,15 +521,15 @@
     detail::vector_accessor<Vector, Class_>(cl);
 
     cl.def(
         "__bool__",
         [](const Vector &v) -> bool { return !v.empty(); },
         "Check whether the list is nonempty");
 
-    cl.def("__len__", &Vector::size);
+    cl.def("__len__", [](const Vector &vec) { return vec.size(); });
 
 #if 0
     // C++ style functions deprecated, leaving it here as an example
     cl.def(init<size_type>());
 
     cl.def("resize",
          (void (Vector::*) (size_type count)) & Vector::resize,
@@ -641,132 +641,109 @@
             }
             s << '}';
             return s.str();
         },
         "Return the canonical string representation of this map.");
 }
 
-template <typename KeyType>
 struct keys_view {
     virtual size_t len() = 0;
     virtual iterator iter() = 0;
-    virtual bool contains(const KeyType &k) = 0;
-    virtual bool contains(const object &k) = 0;
+    virtual bool contains(const handle &k) = 0;
     virtual ~keys_view() = default;
 };
 
-template <typename MappedType>
 struct values_view {
     virtual size_t len() = 0;
     virtual iterator iter() = 0;
     virtual ~values_view() = default;
 };
 
-template <typename KeyType, typename MappedType>
 struct items_view {
     virtual size_t len() = 0;
     virtual iterator iter() = 0;
     virtual ~items_view() = default;
 };
 
-template <typename Map, typename KeysView>
-struct KeysViewImpl : public KeysView {
+template <typename Map>
+struct KeysViewImpl : public detail::keys_view {
     explicit KeysViewImpl(Map &map) : map(map) {}
     size_t len() override { return map.size(); }
     iterator iter() override { return make_key_iterator(map.begin(), map.end()); }
-    bool contains(const typename Map::key_type &k) override { return map.find(k) != map.end(); }
-    bool contains(const object &) override { return false; }
+    bool contains(const handle &k) override {
+        try {
+            return map.find(k.template cast<typename Map::key_type>()) != map.end();
+        } catch (const cast_error &) {
+            return false;
+        }
+    }
     Map &map;
 };
 
-template <typename Map, typename ValuesView>
-struct ValuesViewImpl : public ValuesView {
+template <typename Map>
+struct ValuesViewImpl : public detail::values_view {
     explicit ValuesViewImpl(Map &map) : map(map) {}
     size_t len() override { return map.size(); }
     iterator iter() override { return make_value_iterator(map.begin(), map.end()); }
     Map &map;
 };
 
-template <typename Map, typename ItemsView>
-struct ItemsViewImpl : public ItemsView {
+template <typename Map>
+struct ItemsViewImpl : public detail::items_view {
     explicit ItemsViewImpl(Map &map) : map(map) {}
     size_t len() override { return map.size(); }
     iterator iter() override { return make_iterator(map.begin(), map.end()); }
     Map &map;
 };
 
 PYBIND11_NAMESPACE_END(detail)
 
 template <typename Map, typename holder_type = std::unique_ptr<Map>, typename... Args>
 class_<Map, holder_type> bind_map(handle scope, const std::string &name, Args &&...args) {
     using KeyType = typename Map::key_type;
     using MappedType = typename Map::mapped_type;
-    using StrippedKeyType = detail::remove_cvref_t<KeyType>;
-    using StrippedMappedType = detail::remove_cvref_t<MappedType>;
-    using KeysView = detail::keys_view<StrippedKeyType>;
-    using ValuesView = detail::values_view<StrippedMappedType>;
-    using ItemsView = detail::items_view<StrippedKeyType, StrippedMappedType>;
+    using KeysView = detail::keys_view;
+    using ValuesView = detail::values_view;
+    using ItemsView = detail::items_view;
     using Class_ = class_<Map, holder_type>;
 
     // If either type is a non-module-local bound type then make the map binding non-local as well;
     // otherwise (e.g. both types are either module-local or converting) the map will be
     // module-local.
     auto *tinfo = detail::get_type_info(typeid(MappedType));
     bool local = !tinfo || tinfo->module_local;
     if (local) {
         tinfo = detail::get_type_info(typeid(KeyType));
         local = !tinfo || tinfo->module_local;
     }
 
     Class_ cl(scope, name.c_str(), pybind11::module_local(local), std::forward<Args>(args)...);
-    static constexpr auto key_type_descr = detail::make_caster<KeyType>::name;
-    static constexpr auto mapped_type_descr = detail::make_caster<MappedType>::name;
-    std::string key_type_name(key_type_descr.text), mapped_type_name(mapped_type_descr.text);
-
-    // If key type isn't properly wrapped, fall back to C++ names
-    if (key_type_name == "%") {
-        key_type_name = detail::type_info_description(typeid(KeyType));
-    }
-    // Similarly for value type:
-    if (mapped_type_name == "%") {
-        mapped_type_name = detail::type_info_description(typeid(MappedType));
-    }
 
-    // Wrap KeysView[KeyType] if it wasn't already wrapped
+    // Wrap KeysView if it wasn't already wrapped
     if (!detail::get_type_info(typeid(KeysView))) {
-        class_<KeysView> keys_view(
-            scope, ("KeysView[" + key_type_name + "]").c_str(), pybind11::module_local(local));
+        class_<KeysView> keys_view(scope, "KeysView", pybind11::module_local(local));
         keys_view.def("__len__", &KeysView::len);
         keys_view.def("__iter__",
                       &KeysView::iter,
                       keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
         );
-        keys_view.def("__contains__",
-                      static_cast<bool (KeysView::*)(const KeyType &)>(&KeysView::contains));
-        // Fallback for when the object is not of the key type
-        keys_view.def("__contains__",
-                      static_cast<bool (KeysView::*)(const object &)>(&KeysView::contains));
+        keys_view.def("__contains__", &KeysView::contains);
     }
     // Similarly for ValuesView:
     if (!detail::get_type_info(typeid(ValuesView))) {
-        class_<ValuesView> values_view(scope,
-                                       ("ValuesView[" + mapped_type_name + "]").c_str(),
-                                       pybind11::module_local(local));
+        class_<ValuesView> values_view(scope, "ValuesView", pybind11::module_local(local));
         values_view.def("__len__", &ValuesView::len);
         values_view.def("__iter__",
                         &ValuesView::iter,
                         keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
         );
     }
     // Similarly for ItemsView:
     if (!detail::get_type_info(typeid(ItemsView))) {
-        class_<ItemsView> items_view(
-            scope,
-            ("ItemsView[" + key_type_name + ", ").append(mapped_type_name + "]").c_str(),
-            pybind11::module_local(local));
+        class_<ItemsView> items_view(scope, "ItemsView", pybind11::module_local(local));
         items_view.def("__len__", &ItemsView::len);
         items_view.def("__iter__",
                        &ItemsView::iter,
                        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
         );
     }
 
@@ -784,33 +761,27 @@
         "__iter__",
         [](Map &m) { return make_key_iterator(m.begin(), m.end()); },
         keep_alive<0, 1>() /* Essential: keep map alive while iterator exists */
     );
 
     cl.def(
         "keys",
-        [](Map &m) {
-            return std::unique_ptr<KeysView>(new detail::KeysViewImpl<Map, KeysView>(m));
-        },
+        [](Map &m) { return std::unique_ptr<KeysView>(new detail::KeysViewImpl<Map>(m)); },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "values",
-        [](Map &m) {
-            return std::unique_ptr<ValuesView>(new detail::ValuesViewImpl<Map, ValuesView>(m));
-        },
+        [](Map &m) { return std::unique_ptr<ValuesView>(new detail::ValuesViewImpl<Map>(m)); },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "items",
-        [](Map &m) {
-            return std::unique_ptr<ItemsView>(new detail::ItemsViewImpl<Map, ItemsView>(m));
-        },
+        [](Map &m) { return std::unique_ptr<ItemsView>(new detail::ItemsViewImpl<Map>(m)); },
         keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def(
         "__getitem__",
         [](Map &m, const KeyType &k) -> MappedType & {
             auto it = m.find(k);
@@ -839,13 +810,14 @@
         auto it = m.find(k);
         if (it == m.end()) {
             throw key_error();
         }
         m.erase(it);
     });
 
-    cl.def("__len__", &Map::size);
+    // Always use a lambda in case of `using` declaration
+    cl.def("__len__", [](const Map &m) { return m.size(); });
 
     return cl;
 }
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `pugixml-0.6.0/src/third_party/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/FindCatch.cmake` & `pugixml-0.6.0/src/third_party/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/FindEigen3.cmake` & `pugixml-0.6.0/src/third_party/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/FindPythonLibsNew.cmake` & `pugixml-0.6.0/src/third_party/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,30 @@
 endif()
 
 # Use the Python interpreter to find the libs.
 if(NOT PythonLibsNew_FIND_VERSION)
   set(PythonLibsNew_FIND_VERSION "3.6")
 endif()
 
+if(NOT CMAKE_VERSION VERSION_LESS "3.27")
+  cmake_policy(GET CMP0148 _pybind11_cmp0148)
+  if(NOT _pybind11_cmp0148)
+    message(
+      AUTHOR_WARNING
+        "Policy CMP0148 is not set: The FindPythonInterp and FindPythonLibs "
+        "modules are removed.  Run \"cmake --help-policy CMP0148\" for policy "
+        "details.  Use the cmake_policy command to set the policy and suppress "
+        "this warning, or preferably upgrade to using FindPython, either by "
+        "calling it explicitly before pybind11, or by setting "
+        "PYBIND11_FINDPYTHON ON before pybind11.")
+  endif()
+  cmake_policy(SET CMP0148 OLD)
+  unset(_pybind11_cmp0148)
+endif()
+
 find_package(PythonInterp ${PythonLibsNew_FIND_VERSION} ${_pythonlibs_required}
              ${_pythonlibs_quiet})
 
 if(NOT PYTHONINTERP_FOUND)
   set(PYTHONLIBS_FOUND FALSE)
   set(PythonLibsNew_FOUND FALSE)
   return()
@@ -168,21 +184,28 @@
 endif()
 string(REGEX REPLACE ";" "\\\\;" _PYTHON_VALUES ${_PYTHON_VALUES})
 string(REGEX REPLACE "\n" ";" _PYTHON_VALUES ${_PYTHON_VALUES})
 _pybind11_get_if_undef(_PYTHON_VALUES 0 _PYTHON_VERSION_LIST)
 _pybind11_get_if_undef(_PYTHON_VALUES 1 PYTHON_PREFIX)
 _pybind11_get_if_undef(_PYTHON_VALUES 2 PYTHON_INCLUDE_DIR)
 _pybind11_get_if_undef(_PYTHON_VALUES 3 PYTHON_SITE_PACKAGES)
-_pybind11_get_if_undef(_PYTHON_VALUES 4 PYTHON_MODULE_EXTENSION)
 _pybind11_get_if_undef(_PYTHON_VALUES 5 PYTHON_IS_DEBUG)
 _pybind11_get_if_undef(_PYTHON_VALUES 6 PYTHON_SIZEOF_VOID_P)
 _pybind11_get_if_undef(_PYTHON_VALUES 7 PYTHON_LIBRARY_SUFFIX)
 _pybind11_get_if_undef(_PYTHON_VALUES 8 PYTHON_LIBDIR)
 _pybind11_get_if_undef(_PYTHON_VALUES 9 PYTHON_MULTIARCH)
 
+list(GET _PYTHON_VALUES 4 _PYTHON_MODULE_EXT_SUFFIX)
+if(PYBIND11_PYTHONLIBS_OVERWRITE OR NOT DEFINED PYTHON_MODULE_DEBUG_POSTFIX)
+  get_filename_component(PYTHON_MODULE_DEBUG_POSTFIX "${_PYTHON_MODULE_EXT_SUFFIX}" NAME_WE)
+endif()
+if(PYBIND11_PYTHONLIBS_OVERWRITE OR NOT DEFINED PYTHON_MODULE_EXTENSION)
+  get_filename_component(PYTHON_MODULE_EXTENSION "${_PYTHON_MODULE_EXT_SUFFIX}" EXT)
+endif()
+
 # Make sure the Python has the same pointer-size as the chosen compiler
 # Skip if CMAKE_SIZEOF_VOID_P is not defined
 # This should be skipped for (non-Apple) cross-compiles (like EMSCRIPTEN)
 if(NOT CMAKE_CROSSCOMPILING
    AND CMAKE_SIZEOF_VOID_P
    AND (NOT "${PYTHON_SIZEOF_VOID_P}" STREQUAL "${CMAKE_SIZEOF_VOID_P}"))
   if(PythonLibsNew_FIND_REQUIRED)
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/JoinPaths.cmake` & `pugixml-0.6.0/src/third_party/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/check-style.sh` & `pugixml-0.6.0/src/third_party/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/cmake_uninstall.cmake.in` & `pugixml-0.6.0/src/third_party/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py` & `pugixml-0.6.0/src/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/libsize.py` & `pugixml-0.6.0/src/third_party/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/pybind11Common.cmake` & `pugixml-0.6.0/src/third_party/pybind11/tools/pybind11Common.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -169,20 +169,24 @@
 else()
   cmake_policy(GET CMP0148 _pybind11_missing_old_python)
 endif()
 
 # Check to see which Python mode we are in, new, old, or no python
 if(PYBIND11_NOPYTHON)
   set(_pybind11_nopython ON)
+  # We won't use new FindPython if PYBIND11_FINDPYTHON is defined and falselike
+  # Otherwise, we use if FindPythonLibs is missing or if FindPython was already used
 elseif(
-  _pybind11_missing_old_python STREQUAL "NEW"
-  OR PYBIND11_FINDPYTHON
-  OR Python_FOUND
-  OR Python2_FOUND
-  OR Python3_FOUND)
+  (NOT DEFINED PYBIND11_FINDPYTHON OR PYBIND11_FINDPYTHON)
+  AND (_pybind11_missing_old_python STREQUAL "NEW"
+       OR PYBIND11_FINDPYTHON
+       OR Python_FOUND
+       OR Python3_FOUND
+      ))
+
   # New mode
   include("${CMAKE_CURRENT_LIST_DIR}/pybind11NewTools.cmake")
 
 else()
 
   # Classic mode
   include("${CMAKE_CURRENT_LIST_DIR}/pybind11Tools.cmake")
@@ -214,16 +218,23 @@
       set(status_level FATAL_ERROR)
     else()
       set(status_level WARNING)
     endif()
 
     execute_process(
       COMMAND
-        ${${_Python}_EXECUTABLE} -c
-        "from pkg_resources import get_distribution; print(get_distribution('${PYPI_NAME}').version)"
+        ${${_Python}_EXECUTABLE} -c "
+try:
+    from importlib.metadata import version
+except ImportError:
+    from pkg_resources import get_distribution
+    def version(s):
+        return get_distribution(s).version
+print(version('${PYPI_NAME}'))
+        "
       RESULT_VARIABLE RESULT_PRESENT
       OUTPUT_VARIABLE PKG_VERSION
       ERROR_QUIET)
 
     string(STRIP "${PKG_VERSION}" PKG_VERSION)
 
     # If a result is present, this failed
@@ -296,29 +307,32 @@
     if(CMAKE_CXX_COMPILER_ID MATCHES "Clang" AND NOT APPLE)
       # Clang Gold plugin does not support -Os; append -O3 to MinSizeRel builds to override it
       set(linker_append ";$<$<CONFIG:MinSizeRel>:-O3>")
     elseif(CMAKE_CXX_COMPILER_ID MATCHES "GNU" AND NOT MINGW)
       set(cxx_append ";-fno-fat-lto-objects")
     endif()
 
-    if(CMAKE_SYSTEM_PROCESSOR MATCHES "ppc64le" OR CMAKE_SYSTEM_PROCESSOR MATCHES "mips64")
-      set(NO_FLTO_ARCH TRUE)
+    if(prefer_thin_lto)
+      set(thin "=thin")
     else()
-      set(NO_FLTO_ARCH FALSE)
+      set(thin "")
     endif()
 
-    if(CMAKE_CXX_COMPILER_ID MATCHES "Clang"
-       AND prefer_thin_lto
-       AND NOT NO_FLTO_ARCH)
+    if(CMAKE_SYSTEM_PROCESSOR MATCHES "ppc64le" OR CMAKE_SYSTEM_PROCESSOR MATCHES "mips64")
+      # Do nothing
+    elseif(CMAKE_SYSTEM_PROCESSOR MATCHES emscripten)
+      # This compile is very costly when cross-compiling, so set this without checking
+      set(PYBIND11_LTO_CXX_FLAGS "-flto${thin}${cxx_append}")
+      set(PYBIND11_LTO_LINKER_FLAGS "-flto${thin}${linker_append}")
+    elseif(CMAKE_CXX_COMPILER_ID MATCHES "Clang")
       _pybind11_return_if_cxx_and_linker_flags_work(
-        HAS_FLTO_THIN "-flto=thin${cxx_append}" "-flto=thin${linker_append}"
+        HAS_FLTO_THIN "-flto${thin}${cxx_append}" "-flto=${thin}${linker_append}"
         PYBIND11_LTO_CXX_FLAGS PYBIND11_LTO_LINKER_FLAGS)
     endif()
-
-    if(NOT HAS_FLTO_THIN AND NOT NO_FLTO_ARCH)
+    if(NOT HAS_FLTO_THIN)
       _pybind11_return_if_cxx_and_linker_flags_work(
         HAS_FLTO "-flto${cxx_append}" "-flto${linker_append}" PYBIND11_LTO_CXX_FLAGS
         PYBIND11_LTO_LINKER_FLAGS)
     endif()
   elseif(CMAKE_CXX_COMPILER_ID MATCHES "IntelLLVM")
     # IntelLLVM equivalent to LTO is called IPO; also IntelLLVM is WIN32/UNIX
     # WARNING/HELP WANTED: This block of code is currently not covered by pybind11 GitHub Actions!
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/pybind11Config.cmake.in` & `pugixml-0.6.0/src/third_party/pybind11/tools/pybind11Config.cmake.in`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
 Add a module and setup all helpers. You can select the type of the library; the
 default is ``MODULE``. There are several options:
 
 ``OPT_SIZE``
   Optimize for size, even if the ``CMAKE_BUILD_TYPE`` is not ``MinSizeRel``.
 ``THIN_LTO``
-  Use thin TLO instead of regular if there's a choice (pybind11's selection
+  Use thin LTO instead of regular if there's a choice (pybind11's selection
   is disabled if ``CMAKE_INTERPROCEDURAL_OPTIMIZATIONS`` is set).
 ``WITHOUT_SOABI``
   Disable the SOABI component (``PYBIND11_NEWPYTHON`` mode only).
 ``NO_EXTRAS``
   Disable all extras, exit immediately after making the module.
 
 pybind11_strip
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/pybind11Tools.cmake` & `pugixml-0.6.0/src/third_party/pybind11/tools/pybind11Tools.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
   set(PYBIND11_PYTHON_VERSION
       ""
       CACHE STRING "Python version to use for compiling modules")
 endif()
 
 # A user can set versions manually too
 set(Python_ADDITIONAL_VERSIONS
-    "3.11;3.10;3.9;3.8;3.7;3.6"
+    "3.12;3.11;3.10;3.9;3.8;3.7;3.6"
     CACHE INTERNAL "")
 
 list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}")
 find_package(PythonLibsNew ${PYBIND11_PYTHON_VERSION} MODULE REQUIRED ${_pybind11_quiet})
 list(REMOVE_AT CMAKE_MODULE_PATH -1)
 
 # Makes a normal variable a cached variable
@@ -61,14 +61,15 @@
 endmacro()
 
 # Cache variables so pybind11_add_module can be used in parent projects
 _pybind11_promote_to_cache(PYTHON_INCLUDE_DIRS)
 _pybind11_promote_to_cache(PYTHON_LIBRARIES)
 _pybind11_promote_to_cache(PYTHON_MODULE_PREFIX)
 _pybind11_promote_to_cache(PYTHON_MODULE_EXTENSION)
+_pybind11_promote_to_cache(PYTHON_MODULE_DEBUG_POSTFIX)
 _pybind11_promote_to_cache(PYTHON_VERSION_MAJOR)
 _pybind11_promote_to_cache(PYTHON_VERSION_MINOR)
 _pybind11_promote_to_cache(PYTHON_VERSION)
 _pybind11_promote_to_cache(PYTHON_IS_DEBUG)
 
 if(PYBIND11_MASTER_PROJECT)
   if(PYTHON_MODULE_EXTENSION MATCHES "pypy")
@@ -144,16 +145,19 @@
 
   target_link_libraries(pybind11::embed INTERFACE pybind11::pybind11
                                                   pybind11::_ClassicPythonLibraries)
 endif()
 
 function(pybind11_extension name)
   # The prefix and extension are provided by FindPythonLibsNew.cmake
-  set_target_properties(${name} PROPERTIES PREFIX "${PYTHON_MODULE_PREFIX}"
-                                           SUFFIX "${PYTHON_MODULE_EXTENSION}")
+  set_target_properties(
+    ${name}
+    PROPERTIES PREFIX "${PYTHON_MODULE_PREFIX}"
+               DEBUG_POSTFIX "${PYTHON_MODULE_DEBUG_POSTFIX}"
+               SUFFIX "${PYTHON_MODULE_EXTENSION}")
 endfunction()
 
 # Build a Python extension module:
 # pybind11_add_module(<name> [MODULE | SHARED] [EXCLUDE_FROM_ALL]
 #                     [NO_EXTRAS] [THIN_LTO] [OPT_SIZE] source1 [source2 ...])
 #
 function(pybind11_add_module target_name)
@@ -208,18 +212,20 @@
     if(ARG_THIN_LTO)
       target_link_libraries(${target_name} PRIVATE pybind11::thin_lto)
     else()
       target_link_libraries(${target_name} PRIVATE pybind11::lto)
     endif()
   endif()
 
-  # Use case-insensitive comparison to match the result of $<CONFIG:cfgs>
-  string(TOUPPER "${CMAKE_BUILD_TYPE}" uppercase_CMAKE_BUILD_TYPE)
-  if(NOT MSVC AND NOT "${uppercase_CMAKE_BUILD_TYPE}" MATCHES DEBUG|RELWITHDEBINFO)
-    pybind11_strip(${target_name})
+  if(DEFINED CMAKE_BUILD_TYPE) # see https://github.com/pybind/pybind11/issues/4454
+    # Use case-insensitive comparison to match the result of $<CONFIG:cfgs>
+    string(TOUPPER "${CMAKE_BUILD_TYPE}" uppercase_CMAKE_BUILD_TYPE)
+    if(NOT MSVC AND NOT "${uppercase_CMAKE_BUILD_TYPE}" MATCHES DEBUG|RELWITHDEBINFO)
+      pybind11_strip(${target_name})
+    endif()
   endif()
 
   if(MSVC)
     target_link_libraries(${target_name} PRIVATE pybind11::windows_extras)
   endif()
 
   if(ARG_OPT_SIZE)
```

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/setup_global.py.in` & `pugixml-0.6.0/src/third_party/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/src/third_party/pybind11/tools/setup_main.py.in` & `pugixml-0.6.0/src/third_party/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/tests/test_attribute.py` & `pugixml-0.6.0/tests/test_attribute.py`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/tests/test_document.py` & `pugixml-0.6.0/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/tests/test_node.py` & `pugixml-0.6.0/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/tests/test_text.py` & `pugixml-0.6.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `pugixml-0.5.0/tests/test_xpath.py` & `pugixml-0.6.0/tests/test_xpath.py`

 * *Files identical despite different names*

