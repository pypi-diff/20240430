# Comparing `tmp/kbplacer-0.8.tar.gz` & `tmp/kbplacer-0.9.tar.gz`

## Comparing `kbplacer-0.8.tar` & `kbplacer-0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/__init__.py
--rw-r--r--   0        0        0     9813 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/__main__.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/board_builder.py
--rw-r--r--   0        0        0    18407 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/board_modifier.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/defaults.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/element_position.py
--rw-r--r--   0        0        0     6261 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/help_dialog.py
--rw-r--r--   0        0        0    30153 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/kbplacer_dialog.py
--rw-r--r--   0        0        0    20115 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/key_placer.py
--rw-r--r--   0        0        0    24707 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/kle_serial.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/template_copier.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 kbplacer-0.8/kbplacer/version.txt
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 kbplacer-0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kbplacer-0.8/LICENSE
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 kbplacer-0.8/pyproject.toml
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 kbplacer-0.8/PKG-INFO
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/__init__.py
+-rw-r--r--   0        0        0     9980 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/__main__.py
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/board_builder.py
+-rw-r--r--   0        0        0    19805 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/board_modifier.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/defaults.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/edge_generator.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/element_position.py
+-rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/help_dialog.py
+-rw-r--r--   0        0        0    33946 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/kbplacer_dialog.py
+-rw-r--r--   0        0        0    35310 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/key_placer.py
+-rw-r--r--   0        0        0    30789 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/kle_serial.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/template_copier.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 kbplacer-0.9/kbplacer/version.txt
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 kbplacer-0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kbplacer-0.9/LICENSE
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 kbplacer-0.9/pyproject.toml
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 kbplacer-0.9/PKG-INFO
```

### Comparing `kbplacer-0.8/kbplacer/__init__.py` & `kbplacer-0.9/kbplacer/__init__.py`

 * *Files identical despite different names*

### Comparing `kbplacer-0.8/kbplacer/__main__.py` & `kbplacer-0.9/kbplacer/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import argparse
-import json
 import logging
 import os
 import sys
 from typing import List
 
 import pcbnew
 
 from .board_builder import BoardBuilder
 from .defaults import DEFAULT_DIODE_POSITION, ZERO_POSITION
+from .edge_generator import build_board_outline
 from .element_position import ElementInfo, ElementPosition, Point, PositionOption, Side
 from .key_placer import KeyPlacer
-from .kle_serial import parse_via
-from .template_copier import TemplateCopier
+from .template_copier import copy_from_template_to_board
 
 logger = logging.getLogger(__name__)
 
 
 class ElementInfoAction(argparse.Action):
     def __call__(self, parser, namespace, values: str, option_string=None) -> None:
         try:
@@ -194,15 +193,28 @@
         help=(
             "X and Y key 1U distance in mm, as two space separated numeric values, "
             "19.05 19.05 by default"
         ),
     )
     parser.add_argument("-t", "--template", help="Controller circuit template")
     parser.add_argument(
-        "--create-from-via",
+        "--build-board-outline",
+        required=False,
+        action="store_true",
+        help="Enables board outline generation around switch footprints.",
+    )
+    parser.add_argument(
+        "--outline-delta",
+        required=False,
+        default=0.0,
+        type=float,
+        help="The amount (in millimetres) to inflate/deflate board outline.",
+    )
+    parser.add_argument(
+        "--create-from-annotated-layout",
         required=False,
         action="store_true",
         help=(
             "Enables experimental creation mode, where via-annotated kle layout is used\n"
             "for adding footprints and netlists to the newly created board file.\n"
         ),
     )
@@ -223,60 +235,49 @@
         ),
     )
 
     args = parser.parse_args()
 
     layout_path = args.layout
     board_path = args.board
-    route_switches_with_diodes = args.route_switches_with_diodes
-    route_rows_and_columns = args.route_rows_and_columns
-    diode = args.diode
-    additional_elements = args.additional_elements
-    key_distance = args.key_distance
-    template_path = args.template
-    create_from_via = args.create_from_via
 
     # set up logger
     logging.basicConfig(
         level=logging.DEBUG, format="%(asctime)s: %(message)s", datefmt="%H:%M:%S"
     )
 
-    if layout_path:
-        with open(layout_path, "r") as f:
-            layout = json.load(f)
-    else:
-        layout = {}
-
-    if create_from_via:
+    if args.create_from_annotated_layout:
         if os.path.isfile(board_path):
             logger.error(f"File {board_path} already exist, aborting")
             sys.exit(1)
 
         builder = BoardBuilder(
             switch_footprint=args.switch_footprint,
             diode_footprint=args.diode_footprint,
         )
-        board = builder.create_board(parse_via(layout))
+        board = builder.create_board(layout_path)
         board.Save(board_path)
 
     board = pcbnew.LoadBoard(board_path)
 
-    placer = KeyPlacer(board, key_distance)
+    placer = KeyPlacer(board, args.key_distance)
     placer.run(
-        layout,
-        "SW{}",
-        diode,
-        route_switches_with_diodes,
-        route_rows_and_columns,
-        additional_elements=additional_elements,
+        layout_path,
+        ElementInfo("SW{}", PositionOption.DEFAULT, ZERO_POSITION, ""),
+        args.diode,
+        args.route_switches_with_diodes,
+        args.route_rows_and_columns,
+        additional_elements=args.additional_elements,
     )
 
-    if template_path:
-        copier = TemplateCopier(board, template_path, route_rows_and_columns)
-        copier.run()
+    if args.build_board_outline:
+        build_board_outline(board, args.outline_delta, "SW{}")
+
+    if args.template:
+        copy_from_template_to_board(board, args.template, args.route_rows_and_columns)
 
     pcbnew.Refresh()
     pcbnew.SaveBoard(board_path, board)
 
     logging.shutdown()
```

### Comparing `kbplacer-0.8/kbplacer/board_modifier.py` & `kbplacer-0.9/kbplacer/board_modifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from __future__ import annotations
 
 import builtins
 import itertools
 import logging
 import math
+import re
 from typing import Tuple
 
 import pcbnew
 
 from .element_position import Side
 
-# remove pre-release and build numbers (if present) and split to major-minor-patch tuple
-KICAD_VERSION = tuple(
-    map(int, ((pcbnew.Version().split("+")[0]).split("-")[0]).split("."))
-)
-DEFAULT_CLEARANCE_MM = 0.25
-
 logger = logging.getLogger(__name__)
+version_match = re.search(r"(\d+)\.(\d+)\.(\d+)", pcbnew.Version())
+KICAD_VERSION = tuple(map(int, version_match.groups())) if version_match else ()
+if KICAD_VERSION == ():
+    logger.warning("Could not determine KiCad version")
 
 
 def position_in_rotated_coordinates(
     point: pcbnew.wxPoint, angle: float
 ) -> pcbnew.wxPoint:
     """
     Map position in xy-Cartesian coordinate system to x'y'-Cartesian which
@@ -200,87 +199,82 @@
     # order in tuple, first pad should be from f1, second from f2
     # Some caller might require proper order
     if result:
         return result[1], result[0]
     return result
 
 
+def get_clearance(
+    i1: pcbnew.BOARD_CONNECTED_ITEM, i2: pcbnew.BOARD_CONNECTED_ITEM
+) -> int:
+    if KICAD_VERSION < (7, 0, 0):
+        # workaround for bug in KiCad 6.x python wrapper:
+        import _pcbnew
+
+        def _own_clearance(item: pcbnew.BOARD_CONNECTED_ITEM) -> int:
+            if item.Type() == pcbnew.PCB_PAD_T:
+                return _pcbnew.PAD_GetOwnClearance(item, item.GetLayer())
+            else:
+                return _pcbnew.BOARD_CONNECTED_ITEM_GetOwnClearance(
+                    item, item.GetLayer()
+                )
+
+        return max(_own_clearance(i1), _own_clearance(i2))
+    else:
+        return max(i1.GetOwnClearance(i1.GetLayer()), i2.GetOwnClearance(i2.GetLayer()))
+
+
 class BoardModifier:
     def __init__(self, board: pcbnew.BOARD) -> None:
         self.board = board
 
     def get_connectivity(self):
         self.board.BuildConnectivity()
         return self.board.GetConnectivity()
 
-    def test_track_collision(self, track: pcbnew.PCB_TRACK) -> bool:
+    def _test_collision_track_without_net(self, track: pcbnew.PCB_TRACK) -> bool:
         collide_list = []
         track_shape = track.GetEffectiveShape()
         track_start = track.GetStart()
         track_end = track.GetEnd()
-        track_net_code = track.GetNetCode()
         # connectivity needs to be last,
         # otherwise it will update track net name before we want it to:
         connectivity = self.get_connectivity()
         for f in self.board.GetFootprints():
             reference = f.GetReference()
             hull = f.GetBoundingHull()
             if hit_test_result := hull.Collide(track_shape):
                 for p in f.Pads():
                     pad_name = p.GetName()
                     pad_shape = p.GetEffectiveShape()
 
-                    # track has non default netlist set so we can skip
-                    # collision detection for pad of same netlist:
-                    if track_net_code != 0 and track_net_code == p.GetNetCode():
-                        logger.debug(
-                            f"Track collision ignored, pad {reference}:{pad_name} "
-                            f"on same netlist: {track.GetNetname()}/{p.GetNetname()}"
-                        )
-                        continue
-
                     # if track starts or ends in pad then assume that
                     # this collision is expected, with the exception of case
                     # where track already has netlist set and it is different
                     # than pad's netlist or pad has `NPTH` attribute
                     if p.HitTest(track_start) or p.HitTest(track_end):
-                        if (
-                            track_net_code != 0
-                            and track_net_code != p.GetNetCode()
-                            and p.IsOnLayer(track.GetLayer())
-                        ) or p.GetAttribute() == pcbnew.PAD_ATTRIB_NPTH:
-                            logger.debug(
-                                f"Track collide with pad {reference}:{pad_name}"
-                            )
-                            collide_list.append(p)
-                        else:
-                            logger.debug(
-                                "Track collision ignored, track starts or ends "
-                                f"in pad {reference}:{pad_name}"
-                            )
+                        logger.debug(
+                            "Track collision ignored, track starts or ends "
+                            f"in pad {reference}:{pad_name}"
+                        )
                     else:
                         hit_test_result = pad_shape.Collide(
-                            track_shape, pcbnew.FromMM(DEFAULT_CLEARANCE_MM)
+                            track_shape, get_clearance(p, track)
                         )
                         on_same_layer = p.IsOnLayer(track.GetLayer())
                         if hit_test_result and on_same_layer:
                             logger.debug(
                                 f"Track collide with pad {reference}:{pad_name}"
                             )
                             collide_list.append(p)
         # track ids to clear at the end:
         tracks_to_clear = []
         for t in self.board.GetTracks():
-            # check collision if not itself, on same layer and with different netlist
-            # (unless 'trackNetCode' is default '0' netlist):
-            if (
-                t.m_Uuid != track.m_Uuid
-                and t.IsOnLayer(track.GetLayer())
-                and (track_net_code != t.GetNetCode() or track_net_code == 0)
-            ):
+            # check collision if not itself and on same layer
+            if t.m_Uuid != track.m_Uuid and t.IsOnLayer(track.GetLayer()):
                 track_uuid = t.m_Uuid.AsString()
                 if (
                     track_start == t.GetStart()
                     or track_start == t.GetEnd()
                     or track_end == t.GetStart()
                     or track_end == t.GetEnd()
                 ):
@@ -301,73 +295,102 @@
                         if collision.m_Uuid in connected_pads_ids:
                             logger.debug(
                                 "Pad collision removed due to connection with track "
                                 "which leads to that pad"
                             )
                             collide_list.remove(collision)
                 elif hit_test_result := t.GetEffectiveShape().Collide(
-                    track_shape, pcbnew.FromMM(DEFAULT_CLEARANCE_MM)
+                    track_shape, get_clearance(t, track)
                 ):
                     logger.debug(f"Track collide with another track: {track_uuid}")
                     collide_list.append(t)
         for collision in list(collide_list):
             if collision.m_Uuid in tracks_to_clear:
                 collision_uuid = collision.m_Uuid.AsString()
                 logger.debug(
                     f"Track collision with {collision_uuid} removed due to "
                     "connection with track which leads to it"
                 )
                 collide_list.remove(collision)
         return len(collide_list) != 0
 
+    def _test_collision_track_with_net(self, track: pcbnew.PCB_TRACK) -> bool:
+        track_netcode = track.GetNetCode()
+        track_shape = track.GetEffectiveShape()
+        track_layer = track.GetLayer()
+        for item in self.board.AllConnectedItems():
+            if track_netcode == item.GetNetCode():
+                continue
+
+            item_shape = item.GetEffectiveShape()
+            if item_shape.Collide(track_shape, get_clearance(item, track)):
+                if isinstance(item.Cast(), pcbnew.PCB_TRACK):
+                    if item.GetLayer() == track_layer:
+                        return True
+                elif isinstance(item.Cast(), pcbnew.PAD):
+                    pad = pcbnew.Cast_to_PAD(item)
+                    if (
+                        pad.IsOnLayer(track_layer)
+                        or pad.GetAttribute == pcbnew.PAD_ATTRIB_NPTH
+                    ):
+                        return True
+                # pcbnew.ZONE is remaining possibility but we do not handle it
+        return False
+
+    def test_track_collision(self, track: pcbnew.PCB_TRACK) -> bool:
+        if track.GetNetCode() == 0:
+            return self._test_collision_track_without_net(track)
+        return self._test_collision_track_with_net(track)
+
     def add_track_to_board(self, track: pcbnew.PCB_TRACK):
         """Add track to the board if track passes collision check.
         If track has no set netlist, it would get netlist of a pad
         or other track, on which it started or ended.
         Collision with element of the same netlist will be ignored
         unless it is default '0' netlist.
         This exception about '0' netlist is important because it helps
         to detect collisions with holes.
 
         :param track: A track to be added to board
         :return: End position of added track or None if failed to add.
         """
+        layer_name = self.board.GetLayerName(track.GetLayer())
+        start = track.GetStart()
+        stop = track.GetEnd()
+        logger.info(
+            f"Adding track segment ({layer_name}): [{start}, {stop}]",
+        )
         if not self.test_track_collision(track):
-            layer_name = self.board.GetLayerName(track.GetLayer())
-            start = track.GetStart()
-            stop = track.GetEnd()
-            logger.info(
-                f"Adding track segment ({layer_name}): [{start}, {stop}]",
-            )
             self.board.Add(track)
+            logger.info("Track added")
             return stop
         else:
             logger.warning("Could not add track segment due to detected collision")
             return None
 
     def add_track_segment_by_points(
-        self, start: pcbnew.wxPoint, end: pcbnew.wxPoint, layer=pcbnew.B_Cu
+        self,
+        start: pcbnew.wxPoint,
+        end: pcbnew.wxPoint,
+        layer=pcbnew.B_Cu,
+        netcode: int = 0,
     ):
         track = pcbnew.PCB_TRACK(self.board)
         track.SetWidth(pcbnew.FromMM(0.25))
         track.SetLayer(layer)
+        if netcode:
+            track.SetNetCode(netcode)
         if KICAD_VERSION >= (7, 0, 0):
             track.SetStart(pcbnew.VECTOR2I(start.x, start.y))
             track.SetEnd(pcbnew.VECTOR2I(end.x, end.y))
         else:
             track.SetStart(start)
             track.SetEnd(end)
         return self.add_track_to_board(track)
 
-    def add_track_segment(
-        self, start: pcbnew.wxPoint, vector: list[int], layer=pcbnew.B_Cu
-    ):
-        end = pcbnew.wxPoint(start.x + vector[0], start.y + vector[1])
-        return self.add_track_segment_by_points(start, end, layer)
-
     def route(self, pad1: pcbnew.PAD, pad2: pcbnew.PAD) -> None:
         r"""Simple track router
         If pads are collinear, it will use single track segment.
         If pads are not collinear it will try use two segments track,
         in first try, it will fanout straight segment from `pad1` to
         `pad2` direction and then it will end it with second segment
         at 45degree angle:
@@ -402,70 +425,87 @@
         if not layers:
             logger.warning("Could not route pads, no common layers found")
             return
 
         layer = layers[0]
         logger.debug(f"Routing at {self.board.GetLayerName(layer)} layer")
 
+        if pad1.GetNetCode() != pad2.GetNetCode():
+            logger.warning("Could not route pads of different nets")
+            return
+
+        netcode = pad1.GetNetCode()
+
         def _calculate_corners(
             pos1: pcbnew.wxPoint, pos2: pcbnew.wxPoint
         ) -> Tuple[pcbnew.wxPoint, pcbnew.wxPoint]:
-            x_diff = pos1.x - pos2.x
-            y_diff = pos1.y - pos2.y
+            x_diff = pos2.x - pos1.x
+            y_diff = pos2.y - pos1.y
             x_diff_abs = builtins.abs(x_diff)
             y_diff_abs = builtins.abs(y_diff)
             if x_diff_abs < y_diff_abs:
                 up_or_down = -1 if y_diff > 0 else 1
                 return (
-                    pcbnew.wxPoint(
-                        pos2.x + x_diff,
-                        pos2.y - (up_or_down * x_diff_abs),
-                    ),
-                    pcbnew.wxPoint(pos1.x - x_diff, pos1.y - x_diff),
+                    pcbnew.wxPoint(pos1.x, pos2.y + (up_or_down * x_diff_abs)),
+                    pcbnew.wxPoint(pos2.x, pos1.y - (up_or_down * x_diff_abs)),
                 )
             else:
                 left_or_right = -1 if x_diff > 0 else 1
                 return (
-                    pcbnew.wxPoint(
-                        pos2.x - (left_or_right * y_diff_abs),
-                        pos2.y + y_diff,
-                    ),
-                    pcbnew.wxPoint(pos1.x - y_diff, pos1.y - y_diff),
+                    pcbnew.wxPoint(pos2.x + (left_or_right * y_diff_abs), pos1.y),
+                    pcbnew.wxPoint(pos1.x - (left_or_right * y_diff_abs), pos2.y),
                 )
 
         def _route(
             pos1: pcbnew.wxPoint, pos2: pcbnew.wxPoint, corner: pcbnew.wxPoint
         ) -> bool:
-            if end := self.add_track_segment_by_points(pos1, corner, layer):
-                end = self.add_track_segment_by_points(end, pos2, layer)
+            if end := self.add_track_segment_by_points(pos1, corner, layer, netcode):
+                end = self.add_track_segment_by_points(end, pos2, layer, netcode)
                 return end is not None
             return False
 
+        def _angles_equal(angle1: float, angle2: float) -> bool:
+            return abs(angle1 - angle2) <= 0.1
+
         pos1 = pad1.GetPosition()
         pos2 = pad2.GetPosition()
 
-        orientation1 = get_orientation(pad1.GetParent())
-        orientation2 = get_orientation(pad2.GetParent())
+        parent1 = pad1.GetParent()
+        parent2 = pad2.GetParent()
 
-        if (orientation1 % 90 == 0) and (orientation2 % 90 == 0):
+        if KICAD_VERSION >= (8, 0, 0):
+            parent1 = pcbnew.Cast_to_FOOTPRINT(parent1)
+            parent2 = pcbnew.Cast_to_FOOTPRINT(parent2)
+
+        orientation1 = get_orientation(parent1)
+        orientation2 = get_orientation(parent2)
+
+        if _angles_equal(orientation1 % 90, 0) and _angles_equal(orientation2 % 90, 0):
+            # this could be merged with next elif but being close to zero is special
+            # i.e. we clamp to 0 when near:
             angle = 0
-        elif orientation1 % 90 == orientation2 % 90:
+        elif _angles_equal(orientation1 % 90, orientation2 % 90):
             # if rotations are considered the same use the angle
             angle = (-1 * orientation1 + 360) % 360
         else:
             logger.warning(
-                "Could not route pads when parent footprints not rotated the same"
+                "Could not route pads when parent footprints not rotated the same, "
+                f"orientations: {orientation1} and {orientation2}"
             )
             return
 
-        logger.debug(f"Routing pad {pos1} with pad {pos2} at {angle} degree angle")
+        logger.debug(
+            f"Routing pad '{pad1.GetParentAsString()}:{pad1.GetPadName()}' at {pos1} "
+            f"with pad '{pad2.GetParentAsString()}:{pad2.GetPadName()}' at {pos2} "
+            f"using coordinate system rotated by {angle} degree(s)"
+        )
 
         # if in line, use one track segment
         if pos1.x == pos2.x or pos1.y == pos2.y:
-            self.add_track_segment_by_points(pos1, pos2, layer)
+            self.add_track_segment_by_points(pos1, pos2, layer, netcode)
         else:
             # pads are not in single line, attempt routing with two segment track
             if angle != 0:
                 pos1_r = position_in_rotated_coordinates(pos1, angle)
                 pos2_r = position_in_rotated_coordinates(pos2, angle)
                 corners = _calculate_corners(pos1_r, pos2_r)
                 corners = (
```

### Comparing `kbplacer-0.8/kbplacer/element_position.py` & `kbplacer-0.9/kbplacer/element_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 class PositionOption(str, Enum):
     DEFAULT = "Default"
     RELATIVE = "Relative"
     PRESET = "Preset"
     CUSTOM = "Custom"
-    UNCHANGED = "Unchaged"
+    UNCHANGED = "Unchanged"
 
     def __str__(self) -> str:
         return self.value
 
     @classmethod
     def get(cls, name) -> PositionOption:
         if isinstance(name, str):
```

### Comparing `kbplacer-0.8/kbplacer/help_dialog.py` & `kbplacer-0.9/kbplacer/help_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         name.SetFont(font)
 
         version_file_name = os.path.join(source_dir, "version.txt")
         version_str = self._("<missing>")
         if os.path.isfile(version_file_name):
             with open(version_file_name, "r") as f:
                 version_str = f.read()
-        if not re.match(r"v\d.\d$", version_str):
+        if not re.match(r"\d.\d$", version_str):
             status = ", " + self._("development build")
         else:
             status = ""
         version = wx.StaticText(self, -1, wx_("Version") + f": {version_str}{status}")
 
         name_box = wx.BoxSizer(wx.HORIZONTAL)
         name_box.Add(static_icon_bitmap, 0, wx.ALL, 5)
```

### Comparing `kbplacer-0.8/kbplacer/kbplacer_dialog.py` & `kbplacer-0.9/kbplacer/kbplacer_dialog.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import gettext
 import json
 import logging
 import os
 import string
 import sys
 from enum import Flag
-from typing import List, Optional, Tuple
+from typing import Any, List, Optional, Tuple
 
 import wx
 from wx.lib.embeddedimage import PyEmbeddedImage
 
 from .defaults import DEFAULT_DIODE_POSITION, ZERO_POSITION
 from .element_position import ElementInfo, ElementPosition, Point, PositionOption, Side
 from .help_dialog import HelpDialog
@@ -37,20 +37,27 @@
     "Set Language": "en",
     "Seleccionar idioma": "es",
     "言語設定": "ja",
     "언어 설정": "ko",
     "Ustaw język": "pl",
     "Установить язык": "ru",
     "Nastaviť jazyk": "sk",
+    "Встановити мову": "uk",
     "設定語言": "zh_CN",
 }
 
 
 def get_current_kicad_language():
-    return KICAD_TRANSLATIONS_LOOKUP.get(wx_("Set Language"), "en")
+    kicad_lang = KICAD_TRANSLATIONS_LOOKUP.get(wx_("Set Language"), "en")
+    # some languages require additional lookup to detect correctly,
+    # for example es vs es_MX:
+    if kicad_lang == "es" and wx_("Enabled:") == "Activado:":
+        # es: Enabled -> Habilitado, es_MX: Enabled -> Activado
+        kicad_lang = "es_MX"
+    return kicad_lang
 
 
 def get_plugin_translator(lang: str = "en"):
     localedir = os.path.join(os.path.dirname(__file__), "locale")
     trans = gettext.translation(
         "kbplacer", localedir=localedir, languages=(lang,), fallback=True
     )
@@ -172,14 +179,18 @@
         self.label.Enable()
         self.text.Enable()
 
     def Disable(self):
         self.label.Disable()
         self.text.Disable()
 
+    def Hide(self):
+        self.label.Hide()
+        self.text.Hide()
+
 
 class CustomRadioBox(wx.Panel):
     def __init__(self, parent, choices: List[str]) -> None:
         super().__init__(parent)
         self.radio_buttons: dict[str, wx.RadioButton] = {}
 
         for choice in choices:
@@ -213,33 +224,38 @@
 
 
 class ElementPositionWidget(wx.Panel):
     def __init__(
         self,
         parent,
         default_position: Optional[ElementPosition] = None,
+        disable_offsets: bool = False,
     ) -> None:
         super().__init__(parent)
 
         self.default = default_position
         self.x = LabeledTextCtrl(
             self, wx_("Offset X:"), value="", width=5, validator=FloatValidator()
         )
         self.y = LabeledTextCtrl(
             self, wx_("Y:"), value="", width=5, validator=FloatValidator()
         )
         self.orientation = LabeledTextCtrl(
             self, wx_("Orientation:"), value="", width=5, validator=FloatValidator()
         )
+        if disable_offsets:
+            self.x.Hide()
+            self.y.Hide()
         self.side_label = wx.StaticText(self, -1, wx_("Side:"))
         self.side = CustomRadioBox(self, choices=[wx_("Front"), wx_("Back")])
 
         sizer = wx.BoxSizer(wx.HORIZONTAL)
-        sizer.Add(self.x, 0, wx.EXPAND | wx.LEFT, 5)
-        sizer.Add(self.y, 0, wx.EXPAND | wx.LEFT, 5)
+        if not disable_offsets:
+            sizer.Add(self.x, 0, wx.EXPAND | wx.LEFT, 5)
+            sizer.Add(self.y, 0, wx.EXPAND | wx.LEFT, 5)
         sizer.Add(self.orientation, 0, wx.EXPAND | wx.LEFT, 5)
         sizer.Add(self.side_label, 0, wx.LEFT | wx.ALIGN_CENTER_VERTICAL, 5)
         sizer.Add(self.side, 0, wx.EXPAND | wx.LEFT, 5)
 
         self.SetSizer(sizer)
 
     def set_position_by_choice(self, choice: str) -> None:
@@ -347,23 +363,17 @@
 
         sizer = wx.BoxSizer(wx.HORIZONTAL)
         sizer.Add(layout_label, 0, wx.LEFT | wx.RIGHT | wx.ALIGN_CENTER_VERTICAL, 5)
         sizer.Add(layout_picker, 1, wx.EXPAND | wx.ALL, 5)
         self.SetSizer(sizer)
 
         self.__layout_picker = layout_picker
-        self.__picker_type = picker_type
 
     def GetValue(self) -> str:
-        path = self.__layout_picker.GetPath()
-        if self.__picker_type == TemplateType.LOAD and not path:
-            # can't be empty when running in `LOAD` mode
-            msg = "'Load from:' file picker can't be empty"
-            raise ValueError(msg)
-        return path
+        return self.__layout_picker.GetPath()
 
 
 class ElementPositionChoiceWidget(wx.Panel):
     def __init__(
         self,
         parent,
         initial_choice: PositionOption,
@@ -449,18 +459,22 @@
             return self.choice, None, template_path
         return self.choice, self.position.GetValue(), template_path
 
     def Enable(self):
         self.dropdown.Enable()
         if self.dropdown.GetValue() == PositionOption.CUSTOM:
             self.position.Enable()
+        self.load_template.Enable()
+        self.save_template.Enable()
 
     def Disable(self):
         self.dropdown.Disable()
         self.position.Disable()
+        self.load_template.Disable()
+        self.save_template.Disable()
 
 
 class ElementSettingsWidget(wx.Panel):
     def __init__(
         self,
         parent,
         element_info: ElementInfo,
@@ -511,23 +525,29 @@
         language = get_current_kicad_language()
         logger.info(f"Language: {language}")
         self._ = get_plugin_translator(language)
 
         def __get_params(name) -> dict:
             return initial_state.get(name, {}) if initial_state else {}
 
+        def __parse_element_info(params: dict) -> None:
+            if "element_info" in params:
+                try:
+                    params["element_info"] = ElementInfo.from_dict(
+                        params["element_info"]
+                    )
+                except:
+                    params = {}
+
         params: dict = __get_params("switch_section")
+        __parse_element_info(params)
         switch_section: wx.Sizer = self.get_switch_section(**params)
 
         params: dict = __get_params("switch_diodes_section")
-        if "element_info" in params:
-            try:
-                params["element_info"] = ElementInfo.from_dict(params["element_info"])
-            except:
-                params = {}
+        __parse_element_info(params)
         switch_diodes_section: wx.Sizer = self.get_switch_diodes_section(**params)
 
         params: dict = __get_params("additional_elements")
         if "elements_info" in params:
             try:
                 params["elements_info"] = [
                     ElementInfo.from_dict(v) for v in params["elements_info"]
@@ -555,53 +575,68 @@
 
         box.Add(buttons, 0, wx.EXPAND | wx.ALL, 5)
 
         self.SetSizerAndFit(box)
 
     def get_switch_section(
         self,
-        annotation: str = "SW{}",
         layout_path: str = "",
         x_distance: str = "19.05",
         y_distance: str = "19.05",
+        element_info: ElementInfo = ElementInfo(
+            "SW{}", PositionOption.DEFAULT, ZERO_POSITION, ""
+        ),
     ) -> wx.Sizer:
         key_annotation = LabeledTextCtrl(
-            self, wx_("Footprint Annotation") + ":", annotation
+            self, wx_("Footprint Annotation") + ":", element_info.annotation_format
         )
 
         layout_label = wx.StaticText(self, -1, self._("Keyboard layout file:"))
         layout_picker = get_file_picker(
             self,
             -1,
             wildcard="JSON files (*.json)|*.json|All files (*)|*",
             style=wx.FLP_USE_TEXTCTRL,
         )
+        layout_picker.SetMinSize((400, -1))
         if layout_path:
             layout_picker.SetPath(layout_path)
             layout_picker.GetTextCtrl().SetInsertionPointEnd()
 
         key_distance_x = LabeledTextCtrl(
             self, wx_("Step X:"), value=x_distance, width=5, validator=FloatValidator()
         )
         key_distance_y = LabeledTextCtrl(
             self, wx_("Step Y:"), value=y_distance, width=5, validator=FloatValidator()
         )
 
+        key_position = ElementPositionWidget(self, ZERO_POSITION, disable_offsets=True)
+        if element_info.position:
+            key_position.set_position(element_info.position)
+
         box = wx.StaticBox(self, label=self._("Switch settings"))
-        sizer = wx.StaticBoxSizer(box, wx.HORIZONTAL)
-        sizer.Add(key_annotation, 0, wx.EXPAND | wx.LEFT | wx.RIGHT, 5)
-        sizer.Add(layout_label, 0, wx.LEFT | wx.RIGHT | wx.ALIGN_CENTER_VERTICAL, 5)
-        sizer.Add(layout_picker, 1, wx.ALL, 5)
-        sizer.Add(key_distance_x, 0, wx.EXPAND | wx.LEFT | wx.RIGHT, 5)
-        sizer.Add(key_distance_y, 0, wx.EXPAND | wx.LEFT | wx.RIGHT, 5)
+        sizer = wx.StaticBoxSizer(box, wx.VERTICAL)
+
+        row1 = wx.BoxSizer(wx.HORIZONTAL)
+        row1.Add(layout_label, 0, wx.LEFT | wx.RIGHT | wx.ALIGN_CENTER_VERTICAL, 5)
+        row1.Add(layout_picker, 1, wx.ALL, 5)
+        row1.Add(key_distance_x, 0, wx.EXPAND | wx.LEFT | wx.RIGHT, 5)
+        row1.Add(key_distance_y, 0, wx.EXPAND | wx.LEFT | wx.RIGHT, 5)
+        sizer.Add(row1, 0, wx.EXPAND | wx.ALL, 5)
+
+        row2 = wx.BoxSizer(wx.HORIZONTAL)
+        row2.Add(key_annotation, 0, wx.EXPAND | wx.LEFT | wx.RIGHT, 5)
+        row2.Add(key_position, 0, wx.EXPAND | wx.LEFT | wx.RIGHT, 5)
+        sizer.Add(row2, 0, wx.EXPAND | wx.ALL, 5)
 
-        self.__key_annotation_format = key_annotation.text
         self.__layout_picker = layout_picker
         self.__key_distance_x = key_distance_x.text
         self.__key_distance_y = key_distance_y.text
+        self.__key_annotation_format = key_annotation.text
+        self.__key_position = key_position
 
         return sizer
 
     def get_switch_diodes_section(
         self,
         enable: bool = True,
         route_switches_with_diodes: bool = True,
@@ -718,15 +753,19 @@
         buttons_sizer.Add(remove_button, 0, wx.EXPAND | wx.ALL, 0)
 
         sizer.Add(buttons_sizer, 0, wx.EXPAND | wx.ALL, 5)
 
         return sizer
 
     def get_misc_section(
-        self, route_rows_and_columns: bool = True, template_path: str = ""
+        self,
+        route_rows_and_columns: bool = True,
+        template_path: str = "",
+        generate_outline: bool = False,
+        outline_delta: float = 0.0,
     ) -> wx.Sizer:
         row_and_columns_tracks_checkbox = wx.CheckBox(
             self, label=self._("Route rows and columns")
         )
         row_and_columns_tracks_checkbox.SetValue(route_rows_and_columns)
 
         template_label = wx.StaticText(
@@ -738,27 +777,64 @@
             wildcard="KiCad printed circuit board files (*.kicad_pcb)|*.kicad_pcb",
             style=wx.FLP_USE_TEXTCTRL,
         )
         if template_path:
             template_picker.SetPath(template_path)
             template_picker.GetTextCtrl().SetInsertionPointEnd()
 
-        box = wx.StaticBox(self, label=self._("Other settings"))
-        sizer = wx.StaticBoxSizer(box, wx.HORIZONTAL)
+        row1 = wx.BoxSizer(wx.HORIZONTAL)
+        row1.Add(row_and_columns_tracks_checkbox, 0, wx.EXPAND | wx.ALL, 5)
+        row1.Add(wx.StaticLine(self, style=wx.LI_VERTICAL), 0, wx.EXPAND | wx.ALL, 5)
+        row1.Add(template_label, 0, wx.LEFT | wx.RIGHT | wx.ALIGN_CENTER_VERTICAL, 5)
+        row1.Add(template_picker, 1, wx.EXPAND | wx.ALL, 5)
+
+        generate_outline_checkbox = wx.CheckBox(
+            self, label=self._("Build board outline")
+        )
+        generate_outline_checkbox.SetValue(generate_outline)
+        generate_outline_checkbox.Bind(
+            wx.EVT_CHECKBOX, self.on_generate_outline_checkbox
+        )
+        outline_delta_ctrl = LabeledTextCtrl(
+            self,
+            self._("Outline delta:"),
+            value=str(outline_delta),
+            width=5,
+            validator=FloatValidator(),
+        )
+
+        row2 = wx.BoxSizer(wx.HORIZONTAL)
+        row2.Add(generate_outline_checkbox, 0, wx.EXPAND | wx.ALL, 5)
+        row2.Add(wx.StaticLine(self, style=wx.LI_VERTICAL), 0, wx.EXPAND | wx.ALL, 5)
+        row2.Add(outline_delta_ctrl, 0, wx.EXPAND | wx.LEFT | wx.RIGHT, 5)
 
-        sizer.Add(row_and_columns_tracks_checkbox, 0, wx.EXPAND | wx.ALL, 5)
-        sizer.Add(wx.StaticLine(self, style=wx.LI_VERTICAL), 0, wx.EXPAND | wx.ALL, 5)
-        sizer.Add(template_label, 0, wx.LEFT | wx.RIGHT | wx.ALIGN_CENTER_VERTICAL, 5)
-        sizer.Add(template_picker, 1, wx.EXPAND | wx.ALL, 5)
+        box = wx.StaticBox(self, label=self._("Other settings"))
+        sizer = wx.StaticBoxSizer(box, wx.VERTICAL)
+        sizer.Add(row1, 0, wx.EXPAND | wx.ALL, 5)
+        sizer.Add(row2, 0, wx.EXPAND | wx.ALL, 5)
 
         self.__rows_and_columns_tracks_checkbox = row_and_columns_tracks_checkbox
         self.__template_picker = template_picker
+        self.__generate_outline_checkbox = generate_outline_checkbox
+        self.__outline_delta_ctrl = outline_delta_ctrl
+
+        self.__enable_outline_delta(generate_outline)
 
         return sizer
 
+    def __enable_outline_delta(self, enable):
+        if enable:
+            self.__outline_delta_ctrl.Enable()
+        else:
+            self.__outline_delta_ctrl.Disable()
+
+    def on_generate_outline_checkbox(self, event):
+        is_checked = event.GetEventObject().IsChecked()
+        self.__enable_outline_delta(is_checked)
+
     def on_help_button(self, event):
         del event
         help_dialog = HelpDialog(self)
         help_dialog.ShowModal()
         help_dialog.Destroy()
 
     def get_layout_path(self) -> str:
@@ -777,57 +853,88 @@
         x = float(self.__key_distance_x.GetValue())
         y = float(self.__key_distance_y.GetValue())
         return x, y
 
     def get_template_path(self) -> str:
         return self.__template_picker.GetPath()
 
+    def get_key_position_info(
+        self,
+    ) -> ElementInfo:
+        return ElementInfo(
+            self.get_key_annotation_format(),
+            PositionOption.DEFAULT,
+            self.__key_position.GetValue(),
+            "",
+        )
+
     def get_diode_position_info(
         self,
     ) -> ElementInfo:
         element_info = self.__diode_settings.GetValue()
         if not self.__place_diodes_checkbox.GetValue():
             element_info.position_option = PositionOption.UNCHANGED
+            element_info.template_path = ""
         return element_info
 
     def get_additional_elements_info(
         self,
     ) -> List[ElementInfo]:
         return [
             e.GetValue()
             for e in self.__additional_elements
             if e.GetValue().annotation_format != ""
         ]
 
+    def generate_outline(self) -> bool:
+        return self.__generate_outline_checkbox.GetValue()
+
+    def get_outline_delta(self) -> float:
+        return float(self.__outline_delta_ctrl.text.GetValue())
+
     def get_window_state(self):
         window_state = {
             "switch_section": {
-                "annotation": self.get_key_annotation_format(),
                 "layout_path": self.get_layout_path(),
                 "x_distance": self.__key_distance_x.GetValue(),
                 "y_distance": self.__key_distance_y.GetValue(),
+                "element_info": self.get_key_position_info().to_dict(),
             },
             "switch_diodes_section": {
                 "enable": self.__place_diodes_checkbox.GetValue(),
                 "route_switches_with_diodes": self.route_switches_with_diodes(),
                 "element_info": self.__diode_settings.GetValue().to_dict(),
             },
             "additional_elements": {
                 "elements_info": [
                     e.GetValue().to_dict() for e in self.__additional_elements
                 ],
             },
             "misc_section": {
                 "route_rows_and_columns": self.route_rows_and_columns(),
                 "template_path": self.get_template_path(),
+                "generate_outline": self.generate_outline(),
+                "outline_delta": self.get_outline_delta(),
             },
         }
         return json.dumps(window_state, indent=None)
 
 
+def load_window_state_from_log(filepath: str) -> Tuple[Any, bool]:
+    if os.path.isfile(filepath):
+        with open(filepath, "r") as f:
+            for line in f:
+                if "GUI state:" in line:
+                    try:
+                        return json.loads(line[line.find("{") :]), False
+                    except:
+                        return None, True
+    return None, False
+
+
 # used for tests
 if __name__ == "__main__":
     import argparse
     import threading
 
     parser = argparse.ArgumentParser(description="dialog test")
     parser.add_argument("-i", "--initial-state", default="{}", help="Initial gui state")
```

### Comparing `kbplacer-0.8/kbplacer/kle_serial.py` & `kbplacer-0.9/kbplacer/kle_serial.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from __future__ import annotations
 
 import argparse
 import copy
 import json
+import logging
 import pprint
+import re
 import sys
+from collections import defaultdict
 from dataclasses import asdict, dataclass, field, fields
-from typing import Any, List, Optional, Tuple, Type, Union
+from itertools import chain
+from typing import Any, Dict, Iterator, List, Optional, Tuple, Type, Union
+
+logger = logging.getLogger(__name__)
 
 DEFAULT_KEY_COLOR = "#cccccc"
 DEFAULT_TEXT_COLOR = "#000000"
 DEFAULT_TEXT_SIZE = 3
+KEY_MAX_LABELS = 12
 
 # Map from serialized label position to normalized position,
 # depending on the alignment flags.
 # fmt: off
 LABEL_MAP: List[List[int]] = [
     # 0  1  2  3  4  5  6  7  8  9 10 11   # align flags
     [ 0, 6, 2, 8, 9,11, 3, 5, 1, 4, 7,10], # 0 = no centering
@@ -79,14 +86,27 @@
             self.default = KeyDefault(**self.default)
         for field in self.__dataclass_fields__:
             value = getattr(self, field)
             if isinstance(value, float):
                 new_val = round(value, 6)
                 setattr(self, field, new_val)
 
+    def get_label(self: Key, index: int) -> Optional[str]:
+        if len(self.labels) > index:
+            return self.labels[index]
+        return None
+
+    def set_label(self: Key, index: int, value: str) -> None:
+        if index > KEY_MAX_LABELS - 1 or index < 0:
+            msg = "Illegal key label index"
+            raise RuntimeError(msg)
+        labels_to_add = index + 1 - len(self.labels)
+        self.labels += labels_to_add * [""]
+        self.labels[index] = value
+
 
 @dataclass
 class Background:
     name: str = ""
     style: str = ""
 
 
@@ -124,15 +144,15 @@
     def to_json(self: Keyboard, indent: Optional[int] = None) -> str:
         return json.dumps(asdict(self), indent=indent)
 
     def __text_size_changed(self: Keyboard, current: list[Any], new: list[Any]) -> bool:
         current = copy.copy(current)
         new = copy.copy(new)
         for obj in [current, new]:
-            if len_difference := 12 - len(obj):
+            if len_difference := KEY_MAX_LABELS - len(obj):
                 obj.extend(len_difference * [0])
         return current != new
 
     def to_kle(self: Keyboard) -> str:
         row = []
         rows = []
 
@@ -146,16 +166,19 @@
         new_row = True
         current.y -= 1  # will be incremented on first row
 
         for key in self.keys:
             props: dict[str, Any] = {}
 
             def add_prop(name: str, value: Any, default: Any) -> Any:
-                if isinstance(value, float):
-                    value = round(value, 6)
+                def _round(v: Any) -> Any:
+                    return round(v, 6) if isinstance(v, float) else v
+
+                value = _round(value)
+                default = _round(default)
                 if value != default:
                     props[name] = value
                 return value
 
             if key.labels:
                 alignment, labels = find_best_label_alignment(key.labels)
             else:
@@ -277,49 +300,137 @@
         for row in rows:
             result += json.dumps(row, indent=None) + ",\n"
         result = result.strip(",\n")
         return result
 
 
 @dataclass
-class ViaKeyboard(Keyboard):
-    alternative_keys: List[Key] = field(default_factory=list)
+class MatrixAnnotatedKeyboard(Keyboard):
+    MATRIX_COORDINATES_LABEL = 0
+    LAYOUT_OPTION_LABEL = 8
 
-    LAYOUT_LABEL = 8
+    alternative_keys: List[Key] = field(default_factory=list)
 
-    def __post_init__(self: ViaKeyboard) -> None:
+    def __post_init__(self: MatrixAnnotatedKeyboard) -> None:
         for key in list(self.keys):
-            if self.is_alternative(key):
+            if not key.decal:
+                # check if required labels defined correctly
+                MatrixAnnotatedKeyboard.get_matrix_position(key)
+                MatrixAnnotatedKeyboard.get_layout_option(key)
+            if self.__is_alternative(key):
                 self.alternative_keys.append(copy.deepcopy(key))
                 self.keys.remove(key)
 
-    def is_alternative(self, key: Key) -> bool:
-        labels = key.labels
-        if key.decal or len(labels) >= 9 and labels[self.LAYOUT_LABEL]:
+    def __is_alternative(self, key: Key) -> bool:
+        if label := key.get_label(self.LAYOUT_OPTION_LABEL):
             # check if not default layout:
-            if labels[self.LAYOUT_LABEL].split(",")[1] != "0":
+            if label.split(",")[1] != "0":
                 # alternative layout key
                 return True
-
         return False
 
+    def key_iterator(self, *, ignore_alternative: bool) -> Iterator[Key]:
+        if ignore_alternative:
+            return iter(self.keys)
+        else:
+            return chain(self.keys, self.alternative_keys)
+
+    def _get_layout_option_or_none(self, key: Key) -> Optional[Tuple[int, int]]:
+        if label := key.get_label(self.LAYOUT_OPTION_LABEL):
+            return tuple(map(int, label.split(",")))
+        return None
+
+    def _get_layout_options(self) -> Dict[int, Dict[int, List[Key]]]:
+        keys: Dict[int, Dict[int, List[Key]]] = defaultdict(lambda: defaultdict(list))
+        for key in self.key_iterator(ignore_alternative=False):
+            option = self._get_layout_option_or_none(key)
+            if option:
+                keys[option[0]][option[1]].append(key)
+        return keys
+
+    def collapse(self) -> None:
+        """Modify positions of alternative_keys to destination positions
+        i.e. the positions they would take as 'non alternative'
+        and de-duplicate items with equal matrix coordinates and size
+        """
+        seen = {}
+        new_alternatives = []
+
+        def _int(value: float) -> Union[int, float]:
+            return int(value) if int(value) == value else value
+
+        def _key_center(key: Key) -> Tuple[Union[int, float], Union[int, float]]:
+            return (_int(key.x + key.width / 2), _int(key.y + key.height / 2))
+
+        def _key_props(key: Key):
+            props = (
+                key.labels[self.MATRIX_COORDINATES_LABEL],
+                *_key_center(key),
+                key.decal,
+            )
+            return props
+
+        for k in self.keys:
+            seen[_key_props(k)] = True
+
+        layout_keys = self._get_layout_options()
+        for choices in layout_keys.values():
+            anchor = min(choices[0], key=lambda key: (key.x, key.y))
+            for choice, keys in choices.items():
+                if choice != 0:
+                    group_anchor = min(keys, key=lambda key: (key.x, key.y))
+                    move_x = anchor.x - group_anchor.x
+                    move_y = anchor.y - group_anchor.y
+                    for k in keys:
+                        k.x = _int(k.x + move_x)
+                        k.y = _int(k.y + move_y)
+                        props = _key_props(k)
+                        if props not in seen:
+                            seen[props] = True
+                            new_alternatives.append(k)
+
+        for key in list(new_alternatives):
+            if key.decal:
+                new_alternatives.remove(key)
+        self.alternative_keys = new_alternatives
+
+    @staticmethod
+    def get_matrix_position(key: Key) -> Tuple[str, str]:
+        try:
+            label = key.get_label(MatrixAnnotatedKeyboard.MATRIX_COORDINATES_LABEL)
+            split = str(label).split(",")
+            if len(split) != 2:
+                raise RuntimeError
+            return (split[0], split[1])
+        except Exception as e:
+            msg = "Matrix coordinates label missing or invalid"
+            raise RuntimeError(msg) from e
+
+    @staticmethod
+    def get_layout_option(key: Key) -> int:
+        if layout_option_label := key.get_label(
+            MatrixAnnotatedKeyboard.LAYOUT_OPTION_LABEL
+        ):
+            return int(layout_option_label.split(",")[1])
+        return 0
+
 
 def reorder_items(items: List[Any], align: int) -> List[Any]:
-    ret: List[Any] = 12 * [None]
+    ret: List[Any] = KEY_MAX_LABELS * [None]
     for i, item in enumerate(items):
         if item:
             index = LABEL_MAP[align][i]
             ret[index] = item
     while ret and ret[-1] is None:
         ret.pop()
     return ret
 
 
 def reorder_items_kle(items, align) -> List[Any]:
-    ret: List[Any] = 12 * [None]
+    ret: List[Any] = KEY_MAX_LABELS * [None]
     for i, label in enumerate(items):
         if label:
             index = REVERSE_LABEL_MAP[align][i]
             if index == -1:
                 ret = []
                 break
             ret[index] = label
@@ -351,17 +462,17 @@
             if val == getattr(key.default, attribute_name):
                 attribute[i] = None
         while attribute and attribute[-1] is None:
             attribute.pop()
         setattr(key, attribute_name, attribute)
 
 
-def parse_via(layout) -> ViaKeyboard:
+def parse_via(layout) -> MatrixAnnotatedKeyboard:
     keyboard = parse_kle(layout["layouts"]["keymap"])
-    return ViaKeyboard(meta=keyboard.meta, keys=keyboard.keys)
+    return MatrixAnnotatedKeyboard(meta=keyboard.meta, keys=keyboard.keys)
 
 
 def parse_kle(layout) -> Keyboard:
     if not isinstance(layout, list):
         msg = "Expected an list of objects"
         raise RuntimeError(msg)
 
@@ -385,15 +496,24 @@
                     # Calculate some generated values
                     new_key.width2 = (
                         current.width if new_key.width2 == 0 else current.width2
                     )
                     new_key.height2 = (
                         current.height if new_key.height2 == 0 else current.height2
                     )
-                    new_key.labels = reorder_items(item.split("\n"), align)
+                    items = item.split("\n")
+                    if len(items) > KEY_MAX_LABELS:
+                        msg = (
+                            f"Illegal key labels: '{repr(item)}'. "
+                            f"Labels string can contain {KEY_MAX_LABELS} '\n' "
+                            "separated items, ignoring redundant values."
+                        )
+                        logger.warning(msg)
+                        items = items[0:KEY_MAX_LABELS]
+                    new_key.labels = reorder_items(items, align)
                     new_key.textSize = reorder_items(new_key.textSize, align)
 
                     cleanup_key(new_key)
 
                     keys.append(new_key)
 
                     current.x = round(current.x + current.width, 6)
@@ -428,15 +548,15 @@
                         align = item["a"]
                     if "f" in item:
                         current.default.textSize = item["f"]
                         current.textSize = []
                     if "f2" in item:
                         if len(current.textSize) == 0:
                             current.textSize = [None]
-                        for _ in range(1, 12):
+                        for _ in range(1, KEY_MAX_LABELS):
                             current.textSize.append(item["f2"])
                     if "fa" in item:
                         current.textSize = item["fa"]
                     if "p" in item:
                         current.profile = item["p"]
                     if "c" in item:
                         current.color = item["c"]
@@ -491,15 +611,15 @@
         else:
             msg = "Unexpected"
             raise RuntimeError(msg)
 
     return Keyboard(meta=metadata, keys=keys)
 
 
-def parse_ergogen_points(layout: dict) -> Keyboard:
+def parse_ergogen_points(layout: dict, *, zone_filter: str = "") -> Keyboard:
     if not isinstance(layout, dict):
         msg = "Expected an object with nested objects"
         raise RuntimeError(msg)
     if not layout:
         msg = "Expected non-empty object"
         raise RuntimeError(msg)
 
@@ -517,15 +637,19 @@
     # ergogen from bottom
     # store topmost, leftmost key index while iterating, it will be used later
     topmost_leftmost = [0, 0]
 
     def __int(value: float) -> Union[int, float]:
         return int(value) if int(value) == value else value
 
-    for item in layout.values():
+    pattern = re.compile(zone_filter) if zone_filter else None
+
+    for name, item in layout.items():
+        if pattern and not re.match(pattern, name):
+            continue
         if "meta" not in item:
             msg = "Item needs to have meta defined"
             raise RuntimeError(msg)
 
         meta = item["meta"]
 
         # read key spacing only once, assume that it does not change
@@ -553,14 +677,20 @@
             key.y == topmost_leftmost[1] and key.x <= topmost_leftmost[0]
         ):
             topmost_leftmost = [key.x, key.y]
 
         # kle and ergogen rotate in opposite directions
         key.rotation_angle = -1 * item["r"]
 
+        # if column_net and row_net defined, add it to label
+        row = meta.get("row_net", "")
+        column = meta.get("column_net", "")
+        if row and column:
+            key.labels.append(f"{row},{column}")
+
         keys.append(key)
 
     # do some cleanup to be kle compatible
     # adjust coordinates
     for key in keys:
         # reverse top-bottom
         key.y = abs(key.y - topmost_leftmost[1])
@@ -606,14 +736,21 @@
         return parse_ergogen_points(layout)
     except Exception:
         pass
     msg = "Unable to get keyboard layout"
     raise RuntimeError(msg)
 
 
+def get_keyboard_from_file(layout_path: str) -> Keyboard:
+    with open(layout_path, "r") as f:
+        layout = json.load(f)
+    logger.info(f"User layout: {layout}")
+    return get_keyboard(layout)
+
+
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="KLE format converter")
     parser.add_argument("-in", required=True, help="Layout file")
     parser.add_argument(
         "-inform",
         required=False,
         default="RAW",
@@ -627,29 +764,47 @@
         default="KLE_INTERNAL",
         choices=["KLE_RAW", "KLE_INTERNAL"],
         help="Specifies the output format",
     )
     parser.add_argument(
         "-text", required=False, action="store_true", help="Print result"
     )
+    parser.add_argument(
+        "-ergogen-filter",
+        required=False,
+        type=str,
+        help="Ergogen zone filter regular expression, applicable only when -inform ERGOGEN_INTERNAL",
+    )
 
     args = parser.parse_args()
     input_path = getattr(args, "in")
     input_format = args.inform
     output_path = getattr(args, "out")
     output_format = args.outform
     print_result = args.text
+    ergogen_filter = args.ergogen_filter
 
     if input_format == output_format:
         print("Output format equal input format, nothing to do...")
         sys.exit(1)
 
     with open(input_path, "r") as f:
-        text_input = f.read()
-        layout = json.loads(text_input)
+        if input_path.endswith("yaml") or input_path.endswith("yml"):
+            try:
+                import yaml
+
+                layout = yaml.safe_load(f)
+            except Exception as e:
+                msg = (
+                    "Could not load yaml file, make sure that `PyYAML` installed "
+                    "and yaml file format correct"
+                )
+                raise RuntimeError(msg) from e
+        else:
+            layout = json.load(f)
 
         result = ""
         if input_format == "KLE_RAW":  # convert to KLE_INTERNAL
             result = parse_kle(layout)
             result = json.loads(result.to_json())
             if print_result:
                 pprint.pprint(result)
@@ -664,15 +819,15 @@
             print(result)
             # 'to_kle' returns 'raw data' string which can be copy pasted
             # to keyboard-layout-editor, to make json out of it we need
             # to wrap it in list. Then it can be uploaded as JSON.
             result = "[" + result + "]"
             result = json.loads(result)
         else:  # ERGOGEN convert to KLE_RAW or KLE_INTERNAL
-            result = parse_ergogen_points(layout)
+            result = parse_ergogen_points(layout, zone_filter=ergogen_filter)
             if output_format == "KLE_INTERNAL":
                 result = json.loads(result.to_json())
                 if print_result:
                     pprint.pprint(result)
             else:
                 result = result.to_kle()
                 if print_result:
```

### Comparing `kbplacer-0.8/kbplacer/template_copier.py` & `kbplacer-0.9/kbplacer/template_copier.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 import logging
 
 import pcbnew
 
-from .board_modifier import BoardModifier, get_footprint, set_position
+from .board_modifier import get_footprint, set_position
 
 logger = logging.getLogger(__name__)
 
 
-class TemplateCopier(BoardModifier):
-    def __init__(
-        self,
-        board: pcbnew.BOARD,
-        template_path: str,
-        route_tracks: bool,
-    ) -> None:
-        super().__init__(board)
-        self.__template = pcbnew.LoadBoard(template_path)
-        self.__board_nets_by_name = board.GetNetsByName()
-        self.__route_tracks = route_tracks
-
-    # Copy positions of elements and tracks from template to board.
-    # This method does not copy parts itself - parts to be positioned
-    # need to be present in board prior to calling this.
-    def run(self) -> None:
-        footprints = self.__template.GetFootprints()
-
-        for footprint in footprints:
-            reference = footprint.GetReference()
-            destination_footprint = get_footprint(self.board, reference)
-
-            layer = footprint.GetLayerName()
-            position = footprint.GetPosition()
-            orientation = footprint.GetOrientation()
-
-            if layer == "B.Cu" and destination_footprint.GetLayerName() != "B.Cu":
-                destination_footprint.Flip(destination_footprint.GetCenter(), False)
-            set_position(destination_footprint, position)
-            destination_footprint.SetOrientation(orientation)
-
-        if self.__route_tracks:
-            tracks = self.__template.GetTracks()
-            for track in tracks:
-                # Clone track but remap netinfo because net codes in template
-                # might be different. Use net names for remapping
-                # (names in template and board under modification must match)
-                clone = track.Duplicate()
-                net_name = clone.GetNetname()
-                net_code = clone.GetNetCode()
-                net_info_in_board = self.__board_nets_by_name[net_name]
-                logger.info(
-                    f"Cloning track from template: {net_name}:{net_code}"
-                    f"-> {net_info_in_board.GetNetname()}:"
-                    f"{net_info_in_board.GetNetCode()}",
-                )
-                clone.SetNet(net_info_in_board)
-                self.board.Add(clone)
+def copy_from_template_to_board(
+    board: pcbnew.BOARD,
+    template_path: str,
+    route_tracks: bool,
+) -> None:
+    """Copy positions of elements and tracks from template to board.
+    This method does not copy parts itself - parts to be positioned
+    need to be present in board prior to calling this.
+    """
+    template = pcbnew.LoadBoard(template_path)
+    footprints = template.GetFootprints()
+    board_nets_by_name = board.GetNetsByName()
+
+    for footprint in footprints:
+        reference = footprint.GetReference()
+        destination_footprint = get_footprint(board, reference)
+
+        layer = footprint.GetLayerName()
+        position = footprint.GetPosition()
+        orientation = footprint.GetOrientation()
+
+        if layer == "B.Cu" and destination_footprint.GetLayerName() != "B.Cu":
+            destination_footprint.Flip(destination_footprint.GetCenter(), False)
+        set_position(destination_footprint, position)
+        destination_footprint.SetOrientation(orientation)
+
+    if route_tracks:
+        tracks = template.GetTracks()
+        for track in tracks:
+            # Clone track but remap netinfo because net codes in template
+            # might be different. Use net names for remapping
+            # (names in template and board under modification must match)
+            clone = track.Duplicate()
+            net_name = clone.GetNetname()
+            net_code = clone.GetNetCode()
+            net_info_in_board = board_nets_by_name[net_name]
+            logger.info(
+                f"Cloning track from template: {net_name}:{net_code}"
+                f"-> {net_info_in_board.GetNetname()}:"
+                f"{net_info_in_board.GetNetCode()}",
+            )
+            clone.SetNet(net_info_in_board)
+            board.Add(clone)
```

### Comparing `kbplacer-0.8/LICENSE` & `kbplacer-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kbplacer-0.8/pyproject.toml` & `kbplacer-0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -124,7 +124,17 @@
 known-first-party = ["hatch_kicad"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.coverage.run]
 relative_files = true
+
+[tool.hatch.envs.tools]
+dependencies = [
+  "drawsvg==2.3.0",
+  "kicad-skip==0.2.5",
+  "PyYAML==6.0.1",
+]
+[tool.hatch.envs.tools.scripts]
+layout2image = "python tools/layout2image.py {args}"
+layout2schematic = "python tools/layout2schematic.py {args}"
```

#### html2text {}

```diff
@@ -37,8 +37,11 @@
 types --non-interactive {args:kbplacer tests}" style = [ "ruff {args:.}",
 "black --check --diff {args:.}", ] fmt = [ "black {args:.}", "ruff --fix
 {args:.}", "style", ] all = [ "style", "typing", ] [tool.black] target-version
 = ["py37"] line-length = 88 [tool.ruff] select = ["ANN", "E", "F", "I", "N",
 "PL", "W"] [tool.ruff.per-file-ignores] "kbplacer/kbplacer_plugin_action.py" =
 ["N802"] [tool.ruff.isort] known-first-party = ["hatch_kicad"]
 [tool.ruff.flake8-tidy-imports] ban-relative-imports = "all"
-[tool.coverage.run] relative_files = true
+[tool.coverage.run] relative_files = true [tool.hatch.envs.tools] dependencies
+= [ "drawsvg==2.3.0", "kicad-skip==0.2.5", "PyYAML==6.0.1", ]
+[tool.hatch.envs.tools.scripts] layout2image = "python tools/layout2image.py
+{args}" layout2schematic = "python tools/layout2schematic.py {args}"
```

### Comparing `kbplacer-0.8/PKG-INFO` & `kbplacer-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbplacer
-Version: 0.8
+Version: 0.9
 Summary: KiCad plugin for automatic keyboard's key placement
 Project-URL: Homepage, https://github.com/adamws/kicad-kbplacer
 Project-URL: Bug Tracker, https://github.com/adamws/kicad-kbplacer/issues
 Project-URL: Sponsor, https://ko-fi.com/adamws
 Author-email: adamws <adamws@users.noreply.github.com>
 License: GPL-3.0
 License-File: LICENSE
```

