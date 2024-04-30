# Comparing `tmp/iotaa-0.8.0-py3-none-any.whl.zip` & `tmp/iotaa-0.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13911 bytes, number of entries: 9
--rw-r--r--  2.0 unx    19993 b- defN 24-Apr-17 16:16 iotaa/__init__.py
--rw-r--r--  2.0 unx     2409 b- defN 24-Apr-17 16:16 iotaa/demo.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 16:16 iotaa/tests/__init__.py
--rw-r--r--  2.0 unx    24164 b- defN 24-Apr-17 16:16 iotaa/tests/test_iotaa.py
--rw-r--r--  2.0 unx      449 b- defN 24-Apr-17 16:18 iotaa-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 16:18 iotaa-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 24-Apr-17 16:18 iotaa-0.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-17 16:18 iotaa-0.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      686 b- defN 24-Apr-17 16:18 iotaa-0.8.0.dist-info/RECORD
-9 files, 47836 bytes uncompressed, 12733 bytes compressed:  73.4%
+Zip file size: 13878 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    19814 b- defN 24-Apr-30 14:47 iotaa/__init__.py
+-rw-r--r--  2.0 unx     2409 b- defN 24-Apr-30 14:47 iotaa/demo.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-30 14:47 iotaa/tests/__init__.py
+-rw-r--r--  2.0 unx    23994 b- defN 24-Apr-30 14:47 iotaa/tests/test_iotaa.py
+-rw-r--r--  2.0 unx      449 b- defN 24-Apr-30 14:49 iotaa-0.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 14:49 iotaa-0.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 24-Apr-30 14:49 iotaa-0.8.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-30 14:49 iotaa-0.8.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      686 b- defN 24-Apr-30 14:49 iotaa-0.8.1.dist-info/RECORD
+9 files, 47487 bytes uncompressed, 12700 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: iotaa/tests/__init__.py
 Comment: 
 
 Filename: iotaa/tests/test_iotaa.py
 Comment: 
 
-Filename: iotaa-0.8.0.dist-info/METADATA
+Filename: iotaa-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: iotaa-0.8.0.dist-info/WHEEL
+Filename: iotaa-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: iotaa-0.8.0.dist-info/entry_points.txt
+Filename: iotaa-0.8.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: iotaa-0.8.0.dist-info/top_level.txt
+Filename: iotaa-0.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: iotaa-0.8.0.dist-info/RECORD
+Filename: iotaa-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iotaa/__init__.py

```diff
@@ -132,15 +132,15 @@
     def update_from_task(self, taskname: str, assets: _AssetT) -> None:
         """
         Update graph data structures with current task info.
 
         :param taskname: The current task's name.
         :param assets: An asset, a collection of assets, or None.
         """
-        alist = _listify(assets)
+        alist = _flatten(assets)
         self.assets.update({a.ref: a.ready for a in alist})
         self.edges |= set((taskname, a.ref) for a in alist)
         self.tasks.add(taskname)
 
 
 _graph = _Graph()
 
@@ -495,21 +495,26 @@
     try:
         _log.info("%s: Executing", taskname)
         next(g)
     except StopIteration:
         pass
 
 
-def _flatten(assets: _AssetT) -> List[Asset]:
+def _flatten(assets: Union[_AssetT, Dict[str, _AssetT], List[_AssetT]]) -> List[Asset]:
     """
-    Return a simple list of assets formed by collapsing potentially nested lists.
+    Return a simple list of assets formed by collapsing potentially nested collections.
 
     :param assets: An asset, a collection of assets, or None.
     """
-    return list(filter(None, chain(*[_listify(a) for a in _listify(assets)])))
+    if assets is None:
+        return []
+    if isinstance(assets, Asset):
+        return [assets]
+    xs = assets if isinstance(assets, list) else assets.values()
+    return list(filter(None, chain.from_iterable(_flatten(x) for x in xs)))
 
 
 def _formatter(prog: str) -> HelpFormatter:
     """
     Help-message formatter.
 
     :param prog: The program name.
@@ -527,29 +532,14 @@
     if _state.initialized:
         return False
     _state.initialize()
     _graph.reset()
     return True
 
 
-def _listify(assets: _AssetT) -> List[Asset]:
-    """
-    Return a list representation of the provided asset(s) (may be empty).
-
-    :param assets: An asset, a collection of assets, or None.
-    """
-    if assets is None:
-        return []
-    if isinstance(assets, Asset):
-        return [assets]
-    if isinstance(assets, dict):
-        return list(assets.values())
-    return assets
-
-
 def _parse_args(raw: List[str]) -> Namespace:
     """
     Parse command-line arguments.
 
     :param args: Raw command-line arguments.
     :return: Parsed command-line arguments.
     """
```

## iotaa/tests/test_iotaa.py

```diff
@@ -574,14 +574,15 @@
     a = iotaa.asset(ref=None, ready=lambda: True)
     assert iotaa._flatten(None) == []
     assert iotaa._flatten([]) == []
     assert iotaa._flatten({}) == []
     assert iotaa._flatten(a) == [a]
     assert iotaa._flatten([a, a]) == [a, a]
     assert iotaa._flatten({"foo": a, "bar": a}) == [a, a]
+    assert iotaa._flatten([None, a, [a, a], {"foo": a, "bar": a}]) == [a, a, a, a, a]
 
 
 def test__formatter():
     formatter = iotaa._formatter("foo")
     assert isinstance(formatter, iotaa.HelpFormatter)
     assert formatter._prog == "foo"
 
@@ -589,22 +590,14 @@
 @pytest.mark.parametrize("val", [True, False])
 def test__i_am_top_task(val):
     with patch.object(iotaa, "_state", new=iotaa._State()) as _state:
         _state.initialized = not val
         assert iotaa._i_am_top_task() == val
 
 
-def test__listify():
-    a = iotaa.asset(ref=None, ready=lambda: True)
-    assert iotaa._listify(assets=None) == []
-    assert iotaa._listify(assets=a) == [a]
-    assert iotaa._listify(assets=[a]) == [a]
-    assert iotaa._listify(assets={"a": a}) == [a]
-
-
 @pytest.mark.parametrize("graph", [None, "-g", "--graph"])
 @pytest.mark.parametrize("tasks", [None, "-t", "--tasks"])
 @pytest.mark.parametrize("verbose", [None, "-v", "--verbose"])
 def test__parse_args(graph, tasks, verbose):
     raw = ["a_module", "a_function", "arg1", "arg2"]
     if graph:
         raw.append(graph)
@@ -689,18 +682,18 @@
         The foo task.
     """
     assert capsys.readouterr().out.strip() == dedent(expected).strip()
 
 
 @pytest.mark.parametrize("assets", simple_assets())
 def test__task_final(assets):
-    for a in iotaa._listify(assets):
+    for a in iotaa._flatten(assets):
         assert getattr(a, "taskname", None) is None
     assets = iotaa._task_final(False, "task", assets)
-    for a in iotaa._listify(assets):
+    for a in iotaa._flatten(assets):
         assert getattr(a, "taskname") == "task"
 
 
 def test__task_inital():
     def f(taskname, n):
         yield taskname
         yield n
@@ -766,15 +759,15 @@
         assert not _graph.tasks
 
 
 @pytest.mark.parametrize("assets", simple_assets())
 def test__Graph_update_from_requirements(assets, empty_graph):
     taskname_req = "req"
     taskname_this = "task"
-    alist = iotaa._listify(assets)
+    alist = iotaa._flatten(assets)
     edges = {
         0: set(),
         1: {(taskname_this, taskname_req), (taskname_req, "foo")},
         2: {(taskname_this, taskname_req), (taskname_req, "foo"), (taskname_req, "bar")},
     }[len(alist)]
     for a in alist:
         setattr(a, "taskname", taskname_req)
@@ -788,15 +781,15 @@
 @pytest.mark.parametrize("assets", simple_assets())
 def test__Graph_update_from_task(assets, empty_graph):
     taskname = "task"
     with patch.object(iotaa, "_graph", empty_graph):
         iotaa._graph.update_from_task(taskname, assets)
         assert all(a() for a in iotaa._graph.assets.values())
         assert iotaa._graph.tasks == {taskname}
-        assert iotaa._graph.edges == {(taskname, x.ref) for x in iotaa._listify(assets)}
+        assert iotaa._graph.edges == {(taskname, x.ref) for x in iotaa._flatten(assets)}
 
 
 # _State tests
 
 
 def test__State():
     with patch.object(iotaa, "_state", iotaa._State()) as _state:
```

## Comparing `iotaa-0.8.0.dist-info/RECORD` & `iotaa-0.8.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-iotaa/__init__.py,sha256=7FSWpg_MatXuWmgFfHVLSGg3IWQWhMODEiqx476JVIQ,19993
+iotaa/__init__.py,sha256=9clvjserSNyLcYVhz3Mdo4_db5HOBIRuozfPTV6ct6g,19814
 iotaa/demo.py,sha256=y-_t4rWXcxFsBrHl5DYmz8sABNNysx9Ya3u6xT-isIo,2409
 iotaa/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-iotaa/tests/test_iotaa.py,sha256=Ltp_cPW_w557xIXAqGEszjKHUZpJVwYmp29ARjIudFQ,24164
-iotaa-0.8.0.dist-info/METADATA,sha256=QIV0UWiwihCJBun6BlWZ5NmmZsT2P7gMGuGZjWl_V4I,449
-iotaa-0.8.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-iotaa-0.8.0.dist-info/entry_points.txt,sha256=7aF41y1-KNzX5_sdAdduzyo7oD-QHyXsHjYTBhEJpKE,37
-iotaa-0.8.0.dist-info/top_level.txt,sha256=UwHT08GJHaAsxZGUqkQpWHqFCHaWfNw_4aAyAATeuPk,6
-iotaa-0.8.0.dist-info/RECORD,,
+iotaa/tests/test_iotaa.py,sha256=SMNv36RZZE80c7ruwcXQuVNEXRo_UGDwadukZfqLZI4,23994
+iotaa-0.8.1.dist-info/METADATA,sha256=tXyvfscx1vlIXZdIV7BAIHzqx7q9-YcBWKKqoNZ4M8U,449
+iotaa-0.8.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+iotaa-0.8.1.dist-info/entry_points.txt,sha256=7aF41y1-KNzX5_sdAdduzyo7oD-QHyXsHjYTBhEJpKE,37
+iotaa-0.8.1.dist-info/top_level.txt,sha256=UwHT08GJHaAsxZGUqkQpWHqFCHaWfNw_4aAyAATeuPk,6
+iotaa-0.8.1.dist-info/RECORD,,
```

