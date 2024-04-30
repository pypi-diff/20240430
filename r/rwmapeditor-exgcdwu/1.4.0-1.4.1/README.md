# Comparing `tmp/rwmapeditor_exgcdwu-1.4.0.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.4.0.tar", last modified: Sat Apr 27 09:38:35 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.4.1.tar", last modified: Tue Apr 30 14:09:26 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.4.0.tar` & `rwmapeditor_exgcdwu-1.4.1.tar`

### file list

```diff
@@ -1,320 +1,320 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.366977 rwmapeditor_exgcdwu-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    42034 2024-04-27 09:38:35.366977 rwmapeditor_exgcdwu-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.318976 rwmapeditor_exgcdwu-1.4.0/rwmap/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.318976 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.318976 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.318976 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/otgroup_grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/otgroup_grid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.318976 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tile_group_grid/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tile_group_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tile_group_grid/_tile_group_addlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tile_group_grid/_tile_group_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tile_group_grid/_tile_group_one.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.322977 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_mapText.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_mapinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitAdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitDetect.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitRemove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.322977 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.322977 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_city.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_city_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_city_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_city_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_normal_unit_add.py
--rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_refresh_building.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.322977 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_troop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_troop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_troop/_troop_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.322977 rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/_element_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/_element_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_global.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_one_and_acti.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/_otgroup/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_otgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_otgroup/_object_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/_tile/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_tile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_tile/_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_add_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_class_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_etElement_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_list_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_png_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_str_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.326977 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.354977 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/
--rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/bridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/decoration.png
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/deepwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt.png
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt_details.png
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dust.png
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna.png
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna_highland.png
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice.png
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/misc.png
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain.png
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shortgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone.png
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/units.png
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/water.png
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/decoration.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/misc.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.362977 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.366977 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Deep Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Dirt.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Dirt_Details.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Dust.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Ice.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Lava.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Long Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Mountain.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Sand.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Shallow Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Short Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Snow.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Stone.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/units.tsx
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:38:35.366977 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42034 2024-04-27 09:38:35.000000 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14016 2024-04-27 09:38:35.000000 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 09:38:35.000000 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-27 09:38:35.000000 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-27 09:38:35.000000 rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-27 09:38:35.366977 rwmapeditor_exgcdwu-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-27 09:38:31.000000 rwmapeditor_exgcdwu-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.082131 rwmapeditor_exgcdwu-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42034 2024-04-30 14:09:26.082131 rwmapeditor_exgcdwu-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.018130 rwmapeditor_exgcdwu-1.4.1/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/otgroup_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/otgroup_grid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tile_group_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tile_group_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tile_group_grid/_tile_group_addlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tile_group_grid/_tile_group_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tile_group_grid/_tile_group_one.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_mapText.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_mapinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_unitAdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_unitDetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_unitRemove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.022130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.026130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_normal_unit_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15007 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_refresh_building.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.026130 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_troop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_troop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_troop/_troop_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.026130 rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.026130 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_one_and_acti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.026130 rwmapeditor_exgcdwu-1.4.1/rwmap/_otgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_otgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_otgroup/_object_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.030130 rwmapeditor_exgcdwu-1.4.1/rwmap/_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_tile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_tile/_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.030130 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_add_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_list_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.030130 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.030130 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.066130 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/bridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/decoration.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/deepwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt_details.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dust.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna_highland.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/misc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shortgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/units.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/water.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/decoration.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/misc.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.078131 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.078131 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Deep Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Dirt.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Dirt_Details.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Dust.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Ice.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Lava.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Long Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Mountain.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Sand.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Shallow Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Short Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Snow.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Stone.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/units.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:09:26.082131 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42034 2024-04-30 14:09:25.000000 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14016 2024-04-30 14:09:26.000000 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:09:25.000000 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 14:09:25.000000 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 14:09:25.000000 rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-30 14:09:26.082131 rwmapeditor_exgcdwu-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-30 14:09:21.000000 rwmapeditor_exgcdwu-1.4.1/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.4.0/LICENSE` & `rwmapeditor_exgcdwu-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/PKG-INFO` & `rwmapeditor_exgcdwu-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.4.0
+Version: 1.4.1
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rwmapeditor_exgcdwu-1.4.0/README.md` & `rwmapeditor_exgcdwu-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_layer.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_layer.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_object.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_object.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_objectgroup.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_objectgroup.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_case/_tileset.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_case/_tileset.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,17 @@
         return self._size.x() * self._size.y()
 
     def firstgid(self)->int:
         return int(self._properties.returnDefaultProperty("firstgid"))
     
     def endgid(self)->int:
         return self.firstgid() + self.totalgid()
+    
+    def changefirstgid(self, firstgid:int)->None:
+        self._properties.assignDefaultProperty("firstgid", str(firstgid))
 
     def gid_to_tileid(self, gid:int)->tuple[str, int]:
         tileid = gid - self.firstgid()
         if tileid < 0:
             raise IndexError("The gid cannot be loaded into the current tileset.")
         return (self.name(), gid - self.firstgid())
```

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_core.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,20 @@
         return tileset
         
     def get_objectgroup_s(self, name:str)->case.ObjectGroup:
         objectgroup = utility.get_ElementOri_from_list_by_name_s(self._objectGroup_list, name)
         if objectgroup == None:
             raise KeyError("objectgroup name:" + name + " not found")
         return objectgroup
+    
+    def add_tileset(self, tileset:case.TileSet)->None:
+        tileset_n = deepcopy(tileset)
+        firstgid = self._tileset_list[-1].endgid()
+        tileset_n.changefirstgid(firstgid)
+        self._tileset_list.append(tileset_n)
 
     def output_str(self, pngtextnum:int = -1, tilenum:int = -1, output_rectangle:frame.Rectangle = frame.Rectangle(frame.Coordinate(), frame.Coordinate(-1, -1)), objectnum:int = -1)->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         str_ans = str_ans + "\n".join([tileset.output_str(pngtextnum, tilenum) for tileset in self._tileset_list if tileset.isexist()]) + "\n"
         str_ans = str_ans + "\n".join([layer.output_str(output_rectangle) for layer in self._layer_list]) + "\n"
         str_ans = str_ans + "\n".join([tobject.output_str(objectnum) for tobject in self._objectGroup_list]) + "\n"
```

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/const.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/const.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_credit.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_credit.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_mapText.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_mapText.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,13 +2,14 @@
 import rwmap._frame as frame
 import rwmap._data.const as const
 
 class MapText(object.TObject_One):
     def __init__(self, pos:frame.Coordinate, text:str, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                  textColor:str = None, textSize:int = -1, name:str = None,
                  actiBy_s:list[object.TObject_One] = [], deactiBy_s:list[object.TObject_One] = [], 
-                 isalltoacti:bool = False):
+                 isalltoacti:bool = False, reset:int = 1):
         upos = frame.Rectangle(pos - size / 2, size)
         object.TObject_One.__init__(self, object.TObject_Type.init_mapText(text, textColor = textColor, textSize = textSize), 
                                     object.TObject_Pos.init_rectangle(upos), name, 
-                                    object.TObject_Acti.init_acti(actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, isalltoacti = isalltoacti))
+                                    object.TObject_Acti.init_acti(actiBy_s = actiBy_s, deactiBy_s = deactiBy_s, isalltoacti = isalltoacti), 
+                                    object.TObject_Time.init_time(reset = reset))
```

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_mapinfo.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_mapinfo.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_message.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_message.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_node.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_node.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitAdd.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_unitAdd.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitDetect.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_unitDetect.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject/_unitRemove.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject/_unitRemove.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/__init__.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/__init__.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_city.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,77 +150,80 @@
         building_s = refresh_building.RefreshBuildingAllTeam(uadd_s, udetect_s, 
                                                       is_detect_acti_add = is_detect_acti_add, 
                                                       detect_to_text = detect_to_text)
         return cls(building_s, citytext, detect_to_text = detect_to_text)
     
     @classmethod
     def init_base(cls, pos:frame.Coordinate, id:str, teamnum:int, 
-                  text:list[str], warmup_detect:int, warmup_add:int, 
+                  text:Union[str, list[str]], warmup_detect:int, warmup_add:int, 
                   reset_detect:int, reset_add:int, units:str = "supplyDepot", 
                   team_add:int = -1, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                   isonlybuilding:bool = True, name_detect:str = None, 
-                  name_add:str = None, name_text:list[str] = [], unitsnum:int = 1, 
-                  id_group:list[int] = [], textColor:list[str] = [], textSize:int = -1, 
+                  name_add:str = None, name_text:Union[str, list[str]] = [], unitsnum:int = 1, 
+                  id_group:list[int] = [], textColor:Union[str, list[str]] = [], textSize:int = -1, 
                   is_detect_acti_add:bool = False, detect_to_text:list[int] = None):
         building_s = refresh_building.RefreshBuildingAllTeam.init_base\
         (pos, id, teamnum, units, warmup_detect = warmup_detect, warmup_add = warmup_add, 
          reset_detect = reset_detect, reset_add = reset_add, team_add = team_add, size = size, 
          isonlybuilding = isonlybuilding, name_detect = name_detect, name_add = name_add, 
          unitsnum = unitsnum, id_group = id_group, is_detect_acti_add = is_detect_acti_add)
         citytext = _make_citytextallteam_s(pos, text, size = size, textColor = textColor, 
                                   textSize = textSize, name = name_text)
         return cls(building_s, citytext, detect_to_text = detect_to_text)
     
     @classmethod
     def init_bb(cls, building_s:refresh_building.RefreshBuildingAllTeam, 
-                text:list[str], name_text:list[str] = [], 
-                textColor:list[str] = [], textSize:int = -1, 
-                detect_to_text:list[int] = None):
+                text:Union[str, list[str]], name_text:list[str] = [], 
+                textColor:Union[str, list[str]] = [], textSize:int = -1, 
+                detect_to_text:Union[str, list[str]] = None):
         citytext = city_text.CityTextAllTeam(building_s.pos(), text, building_s.size(), textColor = textColor, 
                                       textSize = textSize, name = name_text)
         return cls(building_s, citytext, detect_to_text = detect_to_text)
     
 class CityAllTeamGroup(refresh_building.RefreshBuildingAllTeamGroup, CityAllTeam):
     def __init__(self, building_s:refresh_building.RefreshBuildingAllTeamGroup, 
                  citytext:city_text.CityTextAllTeam):
         if ((not isinstance(building_s, refresh_building.RefreshBuildingAllTeamGroup)) or \
            (not isinstance(citytext, city_text.CityTextAllTeam))):
             raise TypeError("CityAllTeamGroup.__init__:must be allteamgroup/allteam")
-        
-        detect_to_text = list(range(building_s.group()))
+        teamgroupnum = building_s.group()
+        detect_to_text = [textn % teamgroupnum for textn in range(building_s.length() - 1)]
+        if citytext.length() != teamgroupnum:
+            raise ValueError("Length of citytext is not equal to building.")
         City.__init__(self, building_s, citytext, detect_to_text = detect_to_text)
 
     @classmethod
     def init_adt(cls, uadd_s:city_add.NormalUnitAdd, udetect_s:city_detect.BuildingDetectAllTeamGroup, 
                  citytext:city_text.CityTextAllTeam, is_detect_acti_add:bool = True):
         detect_to_text = list[range(udetect_s.group())]
         building_s = refresh_building.RefreshBuildingAllTeam(uadd_s, udetect_s, 
                                                       is_detect_acti_add = is_detect_acti_add, 
                                                       detect_to_text = detect_to_text)
         return cls(building_s, citytext, detect_to_text = detect_to_text)
     
     @classmethod
     def init_base(cls, pos:frame.Coordinate, id:str, teamnum:int, 
-                  text:list[str], warmup_detect:int, warmup_add:int, 
+                  text:Union[list[str], str], warmup_detect:int, warmup_add:int, 
                   reset_detect:int, reset_add:int, units:str = "supplyDepot", 
                   team_add:int = -1, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                   isonlybuilding:bool = True, name_detect:str = None, 
-                  name_add:str = None, name_text:list[str] = [], unitsnum:int = 1, 
-                  teamgroup:int = 2, textColor:list[str] = [], textSize:int = -1, 
-                  is_detect_acti_add:bool = False):
+                  name_add:str = None, name_text:Union[list[str], str] = [], unitsnum:int = 1, 
+                  teamgroup:int = 2, textColor:Union[list[str], str] = [], textSize:int = -1, 
+                  is_detect_acti_add:bool = False, isacti_accu:bool = False):
         
         building_s = refresh_building.RefreshBuildingAllTeamGroup.init_base\
         (pos, id, teamnum, units, warmup_detect = warmup_detect, warmup_add = warmup_add, 
          reset_detect = reset_detect, reset_add = reset_add, team_add = team_add, size = size, 
          isonlybuilding = isonlybuilding, name_detect = name_detect, name_add = name_add, 
-         unitsnum = unitsnum,teamgroup = teamgroup, is_detect_acti_add = is_detect_acti_add)
+         unitsnum = unitsnum,teamgroup = teamgroup, is_detect_acti_add = is_detect_acti_add, 
+         isacti_accu = isacti_accu)
         citytext = _make_citytextallteam_s(pos, text, size = size, textColor = textColor, 
                                   textSize = textSize, name = name_text)
         return cls(building_s, citytext, teamgroup = teamgroup)
     
     @classmethod
     def init_bb(cls, building_s:refresh_building.RefreshBuildingAllTeamGroup, 
-                text:list[str], name_text:list[str] = [], 
-                textColor:list[str] = [], textSize:int = -1):
+                text:Union[list[str], str], name_text:Union[list[str], str] = [], 
+                textColor:Union[list[str], str] = [], textSize:int = -1):
         citytext = city_text.CityTextAllTeam(building_s.pos(), text, building_s.size(), textColor = textColor, 
                                       textSize = textSize, name = name_text)
         return cls(building_s, citytext)
```

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_city_detect.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city_detect.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,16 +95,16 @@
                 if self.idTObject_s_index(index)._name == id]
 
 class BuildingDetectAllTeamGroup(BuildingDetectAllTeam):
     def __init__(self, pos:frame.Coordinate, id:str, teamnum:int, 
                  warmup:int, reset:int, unitType_andob:Union[str, bool] = True, 
                  size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                  name:str = None, teamgroup:int = 2, minUnits:int = None, 
-                 maxUnits:int = None):
+                 maxUnits:int = None, isacti_accu:bool = False):
         self._teamgroup = teamgroup
-        id_group = [team % teamgroup for team in range(teamnum)]
+        id_group = [team % teamgroup for team in range(teamnum)]  if isacti_accu else []
         BuildingDetectAllTeam.__init__(self, pos, id, teamnum, warmup, reset, size = size, 
                                        unitType_andob = unitType_andob, name = name, 
                                        id_group = id_group, minUnits = minUnits, maxUnits = maxUnits)
         
     def group(self)->int:
         return self._teamgroup
```

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_city_text.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_city_text.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,30 +10,33 @@
 
 class CityText(object.TObject_Group):
     def __init__(self, pos:frame.Coordinate, text:Union[list[str], str], 
                  size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                  textColor:Union[list[str], str] = [], textSize:int = -1, 
                  name:Union[list[str], str] = [], 
                  actiBy_s_list:list[Union[list[object.TObject_One], object.TObject_One]] = [], 
-                 deactiBy_s_list:list[Union[list[object.TObject_One], object.TObject_One]] = []):
+                 deactiBy_s_list:list[Union[list[object.TObject_One], object.TObject_One]] = [], 
+                 reset:int = 1):
         name_list = deepcopy(utility.list_variable_s(name))
         text_list = deepcopy(utility.list_variable_s(text))
         textColor_list = deepcopy(utility.list_variable_s(textColor))
+        if len(textColor_list) > len(text_list):
+            raise ValueError("the length of textColor is longer than text")
         maptext = []
         for index in range(len(text_list)):
             name = utility.list_get_s(name_list, index)
             text = utility.list_get_s(text_list, index)
             textColor = utility.list_get_s(textColor_list, index)
             actiBy_s =  deepcopy(utility.list_variable_s(utility.list_get_s(actiBy_s_list, index)))
             deactiBy_s =  deepcopy(utility.list_variable_s(utility.list_get_s(deactiBy_s_list, index)))
             actiBy_s = [] if actiBy_s == None else actiBy_s
             deactiBy_s = [] if deactiBy_s == None else deactiBy_s
             maptext.append(tobject.MapText(pos, text, size = size, textColor = textColor, 
                                            textSize = textSize, name = name, actiBy_s = actiBy_s, 
-                                           deactiBy_s = deactiBy_s))
+                                           deactiBy_s = deactiBy_s, reset = reset))
         object.TObject_Group.__init__(self, maptext)
     
     def pos(self)->frame.Coordinate:
         return self._TObject_One_list[0]._pos.pos()
 
     def size(self)->frame.Coordinate:
         return self._TObject_One_list[0]._pos.size()
@@ -55,18 +58,20 @@
             self.maptext(index).add_deactiBy_s(deactiBy_s)
 
     
 class CityTextNoTeam(CityText):
     def __init__(self, pos:frame.Coordinate, text:str, 
                  size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                  textColor:str = None, textSize:int = -1, 
-                 name:str = None):
+                 name:str = None, reset:int = 1):
         CityText.__init__(self, pos, text, size = size, textColor = textColor, textSize = textSize, 
-                        name = name)
+                        name = name, reset = reset)
     
 class CityTextAllTeam(CityText):
-    def __init__(self, pos:frame.Coordinate, text:list[str], 
-                 size:frame.Coordinate = const.COO.SIZE_STANDARD, textColor:list[str] = [], \
-                 textSize:int = -1, name:list[str] = [], actiBy_s_list:list[Union[list[object.TObject_One], object.TObject_One]] = [], 
-                 deactiBy_s_list:list[Union[list[object.TObject_One], object.TObject_One]] = []):
+    def __init__(self, pos:frame.Coordinate, text:Union[list[str], str], 
+                 size:frame.Coordinate = const.COO.SIZE_STANDARD, textColor:Union[list[str], str] = [], \
+                 textSize:int = -1, name:Union[list[str], str] = [], actiBy_s_list:list[Union[list[object.TObject_One], object.TObject_One]] = [], 
+                 deactiBy_s_list:list[Union[list[object.TObject_One], object.TObject_One]] = [], 
+                 reset:int = 1):
         CityText.__init__(self, pos, text, size = size, textColor = textColor, textSize = textSize, 
-                        name = name, actiBy_s_list = actiBy_s_list, deactiBy_s_list = deactiBy_s_list)
+                        name = name, actiBy_s_list = actiBy_s_list, deactiBy_s_list = deactiBy_s_list, 
+                        reset = reset)
```

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_normal_unit_add.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_normal_unit_add.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_city/_refresh_building.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_city/_refresh_building.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,24 +71,24 @@
         return udetect_s
 
 def _make_udetectallteamgroup_s(pos:frame.Coordinate, id:str, teamnum:int, units:str, 
                     warmup:int, reset:int, 
                     size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                     isonlybuilding:bool = True, name:str = [], teamgroup:int = 2, 
                     unitsnum:int = 1, 
-                    is_detect_acti_add:bool = False)->city_detect.BuildingDetectAllTeam:
+                    is_detect_acti_add:bool = False, isacti_accu:bool = False)->city_detect.BuildingDetectAllTeam:
         
         minUnits = unitsnum if not is_detect_acti_add else None
         maxUnits = unitsnum - 1 if is_detect_acti_add else None
         unitType_andob = units if not isonlybuilding else True
 
         udetect_s = city_detect.BuildingDetectAllTeamGroup(pos, id, teamnum, warmup, reset, size = size, 
                                                       unitType_andob = unitType_andob, name = name, 
                                                       teamgroup = teamgroup, minUnits = minUnits, 
-                                                      maxUnits = maxUnits)
+                                                      maxUnits = maxUnits, isacti_accu = isacti_accu)
 
         return udetect_s
 
 class RefreshBuilding(object.TObject_Group):
     pass
 
 class RefreshBuilding(object.TObject_Group):
@@ -246,23 +246,24 @@
     
     @classmethod
     def init_base(cls, pos:frame.Coordinate, id:str, teamnum:int, units:str, 
                  warmup_detect:int, warmup_add:int, reset_detect:int, reset_add:int, 
                  team_add:int = -1, size:frame.Coordinate = const.COO.SIZE_STANDARD, 
                  isonlybuilding:bool = True, name_detect:str = None, 
                  name_add:str = None, unitsnum:int = 1, teamgroup:int = 2, 
-                 is_detect_acti_add:bool = False):
+                 is_detect_acti_add:bool = False, isacti_accu:bool = False):
 
         uadd_s = _make_uadd_s(pos, warmup_add, reset_add, units, team = team_add, 
                               size = size, name = name_add, unitsnum = unitsnum)
         
         udetect_s = _make_udetectallteamgroup_s(pos, id, teamnum, units, warmup_detect, reset_detect, 
                                            size = size, isonlybuilding = isonlybuilding, 
                                            name = name_detect, teamgroup = teamgroup,
-                                           unitsnum = unitsnum, is_detect_acti_add = is_detect_acti_add)
+                                           unitsnum = unitsnum, is_detect_acti_add = is_detect_acti_add, 
+                                           isacti_accu = isacti_accu)
 
         return cls(uadd_s, udetect_s, is_detect_acti_add)
     
     def unitDetect_s(self)->city_detect.BuildingDetectAllTeamGroup:
         return self._TObject_Group_list[1]
     
     def group(self)->int:
```

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_data/tobject_group/_troop/_troop_add.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_data/tobject_group/_troop/_troop_add.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/_coordinate.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/_coordinate.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_frame/_element_property.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_frame/_element_property.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_global.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_global.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_group.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_group.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_one_and_acti.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_one_and_acti.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_pos.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_pos.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_time.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_time.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_object/_object_type.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_object/_object_type.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_tile/_tile_group.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_tile/_tile_group.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_util/__init__.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_add_dict.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_add_dict.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_etElement_process.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_etElement_process.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_list_util.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_list_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/_util/_str_util.py` & `rwmapeditor_exgcdwu-1.4.1/rwmap/_util/_str_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/bridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/bridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/decoration.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/decoration.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/deepwater.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/deepwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dirt_details.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dirt_details.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/dust.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/dust.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna_dark.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/fauna_highland.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/fauna_highland.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/lava2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/lava2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/misc.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/misc.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2road_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2road_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2_old.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_hill.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sand_dark.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sand_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/shortgrass.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/shortgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_hill.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2lava.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/units.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/units.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/water.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/water.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/misc.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/misc.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/terrain/Lava.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/terrain/Lava.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmap/other_data/maps/units.tsx` & `rwmapeditor_exgcdwu-1.4.1/rwmap/other_data/maps/units.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO` & `rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.4.0
+Version: 1.4.1
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rwmapeditor_exgcdwu-1.4.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt` & `rwmapeditor_exgcdwu-1.4.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.0/setup.py` & `rwmapeditor_exgcdwu-1.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 import os
 from setuptools import setup, find_packages
 
-__version__ = '1.4.0'
+__version__ = '1.4.1'
 
 def read_file(file:str):
     with open(file) as file:
         return file.read()
 
 def readline_file(file:str):
     with open(file) as file:
```

