# Comparing `tmp/trimesh-4.3.1.tar.gz` & `tmp/trimesh-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimesh-4.3.1.tar", last modified: Tue Apr 16 18:43:46 2024, max compression
+gzip compressed data, was "trimesh-4.3.2.tar", last modified: Mon Apr 29 23:29:15 2024, max compression
```

## Comparing `trimesh-4.3.1.tar` & `trimesh-4.3.2.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.437662 trimesh-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-16 18:43:30.000000 trimesh-4.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-16 18:43:46.437662 trimesh-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-04-16 18:43:30.000000 trimesh-4.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-16 18:43:30.000000 trimesh-4.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:43:46.437662 trimesh-4.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.405662 trimesh-4.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_3dxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_3mf.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_adjacency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_arc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_binvox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_convex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_crash.py
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_curvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_dae.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_dxf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_except.py
--rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_fill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)    41146 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_gltf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_gmsh.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_inertia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_integralmeancurvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_loaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_medial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_minimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_mutate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_normals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_nsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_path_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_path_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_pbr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_permutate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_ply.py
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_poses.py
--rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_proximity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_ray.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_remesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_runlength.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_scenegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_section.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_splines.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_texture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_thickness.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_trackball.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_triangles.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_unwrap.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_urdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18466 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_vertices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-16 18:43:30.000000 trimesh-4.3.1/tests/test_voxel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.417662 trimesh-4.3.1/trimesh/
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   102604 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/convex.py
--rw-r--r--   0 runner    (1001) docker     (127)    45776 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/curvature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.417662 trimesh-4.3.1/trimesh/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/binvox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/cascade.py
--rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/dae.py
--rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    68462 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/gltf.py
--rw-r--r--   0 runner    (1001) docker     (127)    21659 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    34419 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/off.py
--rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/ply.py
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/stl.py
--rw-r--r--   0 runner    (1001) docker     (127)    15866 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/threedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/threemf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/urdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/xaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/exchange/xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    30523 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    26162 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/inertia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.417662 trimesh-4.3.1/trimesh/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/interfaces/blender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/interfaces/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/interfaces/gmsh.py
--rw-r--r--   0 runner    (1001) docker     (127)    28268 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/intersections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/nsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/parent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.421662 trimesh-4.3.1/trimesh/path/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/arc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.421662 trimesh-4.3.1/trimesh/path/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33119 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/dxf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23095 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/exchange/svg_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/intersections.py
--rw-r--r--   0 runner    (1001) docker     (127)    26100 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    31112 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/segments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/path/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/permutate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19968 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/poses.py
--rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/proximity.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.421662 trimesh-4.3.1/trimesh/ray/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/ray/ray_pyembree.py
--rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/ray/ray_triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/ray/ray_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    40188 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/remesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.425662 trimesh-4.3.1/trimesh/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/creation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.425662 trimesh-4.3.1/trimesh/resources/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    24785 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/gltf2.schema.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.425662 trimesh-4.3.1/trimesh/resources/schema/primitive/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/box.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/capsule.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/cylinder.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/extrusion.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/primitive.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/scenegraph.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/sphere.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/transform.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/trimesh.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/primitive/wkt.polygon.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/schema/urdf.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.425662 trimesh-4.3.1/trimesh/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/base.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/blender_boolean.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/blender_unwrap.py.template
--rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/dxf.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/path.svg
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/ply.json
--rw-r--r--   0 runner    (1001) docker     (127)   167999 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/templates/viewer.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/resources/units_to_inches.json
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.433662 trimesh-4.3.1/trimesh/scene/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/scene/cameras.py
--rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/scene/lighting.py
--rw-r--r--   0 runner    (1001) docker     (127)    48032 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/scene/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/scene/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)    74544 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21710 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/triangles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    66709 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.433662 trimesh-4.3.1/trimesh/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/viewer/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/viewer/trackball.py
--rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/viewer/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    30971 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/viewer/windowed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.433662 trimesh-4.3.1/trimesh/visual/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    29109 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/gloss.py
--rw-r--r--   0 runner    (1001) docker     (127)    34678 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/visual/texture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.433662 trimesh-4.3.1/trimesh/voxel/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)    27755 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/runlength.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-16 18:43:30.000000 trimesh-4.3.1/trimesh/voxel/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:43:46.433662 trimesh-4.3.1/trimesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-16 18:43:46.000000 trimesh-4.3.1/trimesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-16 18:43:46.000000 trimesh-4.3.1/trimesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:43:46.000000 trimesh-4.3.1/trimesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-16 18:43:46.000000 trimesh-4.3.1/trimesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 18:43:46.000000 trimesh-4.3.1/trimesh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.165613 trimesh-4.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-29 23:29:05.000000 trimesh-4.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-29 23:29:15.165613 trimesh-4.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-04-29 23:29:05.000000 trimesh-4.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-29 23:29:05.000000 trimesh-4.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 23:29:15.165613 trimesh-4.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.133612 trimesh-4.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_3dxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_3mf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_adjacency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_binvox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11564 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_convex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_curvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_dae.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_dxf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_except.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_fill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41146 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_gltf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_integralmeancurvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_medial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_mutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_normals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_nsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_path_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_path_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_pbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_permutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_ply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_remesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_runlength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_scenegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_splines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_texture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_trackball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_triangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_unwrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_urdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18466 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_vertices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-29 23:29:05.000000 trimesh-4.3.2/tests/test_voxel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.145613 trimesh-4.3.2/trimesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102599 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/convex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45776 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/curvature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.149613 trimesh-4.3.2/trimesh/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17597 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/binvox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/cascade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/dae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68424 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/gltf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34419 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/off.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/ply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/stl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/threedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/threemf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/urdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/xaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/exchange/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30523 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26162 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/inertia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.149613 trimesh-4.3.2/trimesh/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/interfaces/blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/interfaces/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/interfaces/gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28268 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/intersections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/nsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/parent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.153612 trimesh-4.3.2/trimesh/path/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.153612 trimesh-4.3.2/trimesh/path/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33119 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/dxf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23095 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/exchange/svg_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/intersections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26100 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43902 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31112 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/path/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/permutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19968 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/proximity.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.153612 trimesh-4.3.2/trimesh/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/ray/ray_pyembree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/ray/ray_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/ray/ray_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40277 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/remesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.153612 trimesh-4.3.2/trimesh/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/creation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.153612 trimesh-4.3.2/trimesh/resources/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24785 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/gltf2.schema.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.157612 trimesh-4.3.2/trimesh/resources/schema/primitive/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/box.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/capsule.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/cylinder.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/extrusion.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/primitive.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/scenegraph.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/sphere.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/transform.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/trimesh.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/primitive/wkt.polygon.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/schema/urdf.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.157612 trimesh-4.3.2/trimesh/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/base.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/blender_boolean.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/blender_unwrap.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)    15667 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/dxf.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/path.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/ply.json
+-rw-r--r--   0 runner    (1001) docker     (127)   167999 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/templates/viewer.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/resources/units_to_inches.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.157612 trimesh-4.3.2/trimesh/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/scene/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8471 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/scene/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48032 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/scene/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27630 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/scene/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74542 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21705 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/triangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66702 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.161613 trimesh-4.3.2/trimesh/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/viewer/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/viewer/trackball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/viewer/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30971 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/viewer/windowed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.161613 trimesh-4.3.2/trimesh/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29109 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/gloss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34678 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/visual/texture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.161613 trimesh-4.3.2/trimesh/voxel/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27725 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/runlength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-29 23:29:05.000000 trimesh-4.3.2/trimesh/voxel/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 23:29:15.161613 trimesh-4.3.2/trimesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-29 23:29:15.000000 trimesh-4.3.2/trimesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-29 23:29:15.000000 trimesh-4.3.2/trimesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 23:29:15.000000 trimesh-4.3.2/trimesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-29 23:29:15.000000 trimesh-4.3.2/trimesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 23:29:15.000000 trimesh-4.3.2/trimesh.egg-info/top_level.txt
```

### Comparing `trimesh-4.3.1/LICENSE.md` & `trimesh-4.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/PKG-INFO` & `trimesh-4.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimesh
-Version: 4.3.1
+Version: 4.3.2
 Summary: Import, export, process, analyze and view triangular meshes.
 Author-email: Michael Dawson-Haggerty <mikedh@kerfed.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Michael Dawson-Haggerty
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `trimesh-4.3.1/README.md` & `trimesh-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/pyproject.toml` & `trimesh-4.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools >= 61.0", "wheel"]
 
 [project]
 name = "trimesh"
 requires-python = ">=3.7"
-version = "4.3.1"
+version = "4.3.2"
 authors = [{name = "Michael Dawson-Haggerty", email = "mikedh@kerfed.com"}]
 license = {file = "LICENSE.md"}
 description = "Import, export, process, analyze and view triangular meshes."
 keywords = ["graphics", "mesh", "geometry", "3D"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `trimesh-4.3.1/tests/test_3dxml.py` & `trimesh-4.3.2/tests/test_3dxml.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_3mf.py` & `trimesh-4.3.2/tests/test_3mf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_adjacency.py` & `trimesh-4.3.2/tests/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_align.py` & `trimesh-4.3.2/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_arc.py` & `trimesh-4.3.2/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_base.py` & `trimesh-4.3.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_binvox.py` & `trimesh-4.3.2/tests/test_binvox.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_boolean.py` & `trimesh-4.3.2/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_bounds.py` & `trimesh-4.3.2/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_cache.py` & `trimesh-4.3.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_camera.py` & `trimesh-4.3.2/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_collision.py` & `trimesh-4.3.2/tests/test_collision.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_color.py` & `trimesh-4.3.2/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_convex.py` & `trimesh-4.3.2/tests/test_convex.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_copy.py` & `trimesh-4.3.2/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_crash.py` & `trimesh-4.3.2/tests/test_crash.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_creation.py` & `trimesh-4.3.2/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_curvature.py` & `trimesh-4.3.2/tests/test_curvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_dae.py` & `trimesh-4.3.2/tests/test_dae.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_decomposition.py` & `trimesh-4.3.2/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_dxf.py` & `trimesh-4.3.2/tests/test_dxf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_edges.py` & `trimesh-4.3.2/tests/test_edges.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_encoding.py` & `trimesh-4.3.2/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_except.py` & `trimesh-4.3.2/tests/test_except.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_export.py` & `trimesh-4.3.2/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_extrude.py` & `trimesh-4.3.2/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_facets.py` & `trimesh-4.3.2/tests/test_facets.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_fill.py` & `trimesh-4.3.2/tests/test_fill.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_geom.py` & `trimesh-4.3.2/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_gltf.py` & `trimesh-4.3.2/tests/test_gltf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_gmsh.py` & `trimesh-4.3.2/tests/test_gmsh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_graph.py` & `trimesh-4.3.2/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_grouping.py` & `trimesh-4.3.2/tests/test_grouping.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_html.py` & `trimesh-4.3.2/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_identifier.py` & `trimesh-4.3.2/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_import.py` & `trimesh-4.3.2/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_inertia.py` & `trimesh-4.3.2/tests/test_inertia.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_integralmeancurvature.py` & `trimesh-4.3.2/tests/test_integralmeancurvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_interval.py` & `trimesh-4.3.2/tests/test_interval.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_light.py` & `trimesh-4.3.2/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_loaded.py` & `trimesh-4.3.2/tests/test_loaded.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_medial.py` & `trimesh-4.3.2/tests/test_medial.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_merge.py` & `trimesh-4.3.2/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_mesh.py` & `trimesh-4.3.2/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_meta.py` & `trimesh-4.3.2/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_minimal.py` & `trimesh-4.3.2/tests/test_minimal.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_mutate.py` & `trimesh-4.3.2/tests/test_mutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_normals.py` & `trimesh-4.3.2/tests/test_normals.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_nsphere.py` & `trimesh-4.3.2/tests/test_nsphere.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_obj.py` & `trimesh-4.3.2/tests/test_obj.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_off.py` & `trimesh-4.3.2/tests/test_off.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_operators.py` & `trimesh-4.3.2/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_packing.py` & `trimesh-4.3.2/tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_path_creation.py` & `trimesh-4.3.2/tests/test_path_creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_path_sample.py` & `trimesh-4.3.2/tests/test_path_sample.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_pathlib.py` & `trimesh-4.3.2/tests/test_pathlib.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_paths.py` & `trimesh-4.3.2/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_pbr.py` & `trimesh-4.3.2/tests/test_pbr.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_permutate.py` & `trimesh-4.3.2/tests/test_permutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_ply.py` & `trimesh-4.3.2/tests/test_ply.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_points.py` & `trimesh-4.3.2/tests/test_points.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_polygons.py` & `trimesh-4.3.2/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_poses.py` & `trimesh-4.3.2/tests/test_poses.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_primitives.py` & `trimesh-4.3.2/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_proximity.py` & `trimesh-4.3.2/tests/test_proximity.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_raster.py` & `trimesh-4.3.2/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_ray.py` & `trimesh-4.3.2/tests/test_ray.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_registration.py` & `trimesh-4.3.2/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_remesh.py` & `trimesh-4.3.2/tests/test_remesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_render.py` & `trimesh-4.3.2/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_repair.py` & `trimesh-4.3.2/tests/test_repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_repr.py` & `trimesh-4.3.2/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_resolvers.py` & `trimesh-4.3.2/tests/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_runlength.py` & `trimesh-4.3.2/tests/test_runlength.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_sample.py` & `trimesh-4.3.2/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_scene.py` & `trimesh-4.3.2/tests/test_scene.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_scenegraph.py` & `trimesh-4.3.2/tests/test_scenegraph.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_section.py` & `trimesh-4.3.2/tests/test_section.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_segments.py` & `trimesh-4.3.2/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_simplify.py` & `trimesh-4.3.2/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_smooth.py` & `trimesh-4.3.2/tests/test_smooth.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_smoothing.py` & `trimesh-4.3.2/tests/test_smoothing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_splines.py` & `trimesh-4.3.2/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_step.py` & `trimesh-4.3.2/tests/test_step.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_stl.py` & `trimesh-4.3.2/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_svg.py` & `trimesh-4.3.2/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_sweep.py` & `trimesh-4.3.2/tests/test_sweep.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_texture.py` & `trimesh-4.3.2/tests/test_texture.py`

 * *Files 6% similar despite different names*

```diff
@@ -202,14 +202,44 @@
         m.visual.uv = None
         assert m.visual.uv is None
 
         # should still be None on a copy
         c = m.copy()
         assert c.visual.uv is None
 
+    def test_pbr_nouv_export(self):
+        # Test that we can properly save and load a pbr material without uv and texture image.
+        material = g.trimesh.visual.material.PBRMaterial(
+            metallicFactor=0.3,
+            roughnessFactor=0.5,
+            baseColorFactor=(0, 255, 0, 255),
+            name="abc",
+        )
+        mesh = g.trimesh.Trimesh(
+            vertices=[[0, 0, 0], [0, 0, 1], [0, 1, 1]],
+            faces=[[0, 1, 2]],
+            process=False,
+            visual=g.trimesh.visual.TextureVisuals(material=material),
+        )
+        scene = g.trimesh.Scene()
+        scene.add_geometry(mesh, geom_name="geom")
+        with g.TemporaryDirectory() as d:
+            # exports by path allow files to be written
+            path = g.os.path.join(d, "tmp.glb")
+            scene.export(path)
+
+            # try reloading
+            r = g.trimesh.load(path)
+            # make sure material survived
+            assert r.geometry["geom"].visual.material.metallicFactor == 0.3
+            assert r.geometry["geom"].visual.material.roughnessFactor == 0.5
+            assert (
+                r.geometry["geom"].visual.material.baseColorFactor == [0, 255, 0, 255]
+            ).all()
+
     def test_pbr_export(self):
         # try loading a textured box
         m = next(iter(g.get_mesh("BoxTextured.glb").geometry.values()))
         # make sure material copy doesn't crash
         m.visual.copy()
 
         with g.TemporaryDirectory() as d:
```

### Comparing `trimesh-4.3.1/tests/test_thickness.py` & `trimesh-4.3.2/tests/test_thickness.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_trackball.py` & `trimesh-4.3.2/tests/test_trackball.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_transformations.py` & `trimesh-4.3.2/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_triangles.py` & `trimesh-4.3.2/tests/test_triangles.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_units.py` & `trimesh-4.3.2/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_unwrap.py` & `trimesh-4.3.2/tests/test_unwrap.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_upstream.py` & `trimesh-4.3.2/tests/test_upstream.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_urdf.py` & `trimesh-4.3.2/tests/test_urdf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_util.py` & `trimesh-4.3.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_vector.py` & `trimesh-4.3.2/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_vertices.py` & `trimesh-4.3.2/tests/test_vertices.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_viewer.py` & `trimesh-4.3.2/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_visual.py` & `trimesh-4.3.2/tests/test_visual.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/tests/test_voxel.py` & `trimesh-4.3.2/tests/test_voxel.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/__init__.py` & `trimesh-4.3.2/trimesh/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/base.py` & `trimesh-4.3.2/trimesh/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         self.nearest = proximity.ProximityQuery(self)
 
         # update the mesh metadata with passed metadata
         self.metadata = {}
         if isinstance(metadata, dict):
             self.metadata.update(metadata)
         elif metadata is not None:
-            raise ValueError("metadata should be a dict or None, got %s" % str(metadata))
+            raise ValueError(f"metadata should be a dict or None, got {metadata!s}")
 
         # store per-face and per-vertex attributes which will
         # be updated when an update_faces call is made
         self.face_attributes = {}
         self.vertex_attributes = {}
         # use update to copy items
         if face_attributes is not None:
```

### Comparing `trimesh-4.3.1/trimesh/boolean.py` & `trimesh-4.3.2/trimesh/boolean.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/bounds.py` & `trimesh-4.3.2/trimesh/bounds.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/caching.py` & `trimesh-4.3.2/trimesh/caching.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/collision.py` & `trimesh-4.3.2/trimesh/collision.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/comparison.py` & `trimesh-4.3.2/trimesh/comparison.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/constants.py` & `trimesh-4.3.2/trimesh/constants.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/convex.py` & `trimesh-4.3.2/trimesh/convex.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/creation.py` & `trimesh-4.3.2/trimesh/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/curvature.py` & `trimesh-4.3.2/trimesh/curvature.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/decomposition.py` & `trimesh-4.3.2/trimesh/decomposition.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exceptions.py` & `trimesh-4.3.2/trimesh/exceptions.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/binvox.py` & `trimesh-4.3.2/trimesh/exchange/binvox.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
     Returns
     --------
     data : bytes
       Suitable for writing to binary file
     """
     if rle_data.dtype != np.uint8:
-        raise ValueError("rle_data.dtype must be np.uint8, got %s" % rle_data.dtype)
+        raise ValueError(f"rle_data.dtype must be np.uint8, got {rle_data.dtype}")
 
     header = binvox_header(shape, translate, scale).encode()
     return header + rle_data.tobytes()
 
 
 def voxel_from_binvox(rle_data, shape, translate=None, scale=1.0, axis_order="xzy"):
     """
@@ -224,15 +224,15 @@
 
     Returns
     ---------
     result : trimesh.voxel.VoxelGrid
       Loaded voxel data
     """
     if file_type is not None and file_type != "binvox":
-        raise ValueError("file_type must be None or binvox, got %s" % file_type)
+        raise ValueError(f"file_type must be None or binvox, got {file_type}")
     data = parse_binvox(file_obj, writeable=True)
     return voxel_from_binvox(
         rle_data=data.rle_data,
         shape=data.shape,
         translate=data.translate,
         scale=data.scale,
         axis_order=axis_order,
@@ -549,23 +549,23 @@
         if provided, this must be empty.
 
     Returns
     ------------
     `VoxelGrid` object resulting.
     """
     if not isinstance(mesh, Trimesh):
-        raise ValueError("mesh must be Trimesh instance, got %s" % str(mesh))
+        raise ValueError(f"mesh must be Trimesh instance, got {mesh!s}")
     if binvoxer is None:
         binvoxer = Binvoxer(**binvoxer_kwargs)
     elif len(binvoxer_kwargs) > 0:
         raise ValueError("Cannot provide binvoxer and binvoxer_kwargs")
     if binvoxer.file_type != "binvox":
         raise ValueError('Only "binvox" binvoxer `file_type` currently supported')
     with TemporaryDirectory() as folder:
-        model_path = os.path.join(folder, "model.%s" % export_type)
+        model_path = os.path.join(folder, f"model.{export_type}")
         with open(model_path, "wb") as fp:
             mesh.export(fp, file_type=export_type)
         out_path = binvoxer(model_path)
         with open(out_path, "rb") as fp:
             out_model = load_binvox(fp)
     return out_model
```

### Comparing `trimesh-4.3.1/trimesh/exchange/cascade.py` & `trimesh-4.3.2/trimesh/exchange/cascade.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/dae.py` & `trimesh-4.3.2/trimesh/exchange/dae.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/export.py` & `trimesh-4.3.2/trimesh/exchange/export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/gltf.py` & `trimesh-4.3.2/trimesh/exchange/gltf.py`

 * *Files 1% similar despite different names*

```diff
@@ -916,16 +916,16 @@
                 buff=buffer_items,
                 blob={"componentType": 5126, "type": "VEC2", "byteOffset": 0},
                 data=uv.astype(float32),
             )
             # add the reference for UV coordinates
             current["primitives"][0]["attributes"]["TEXCOORD_0"] = acc_uv
 
-            # only reference the material if we had UV coordinates
-            current["primitives"][0]["material"] = current_material
+        # reference the material
+        current["primitives"][0]["material"] = current_material
 
     if include_normals or (
         include_normals is None and "vertex_normals" in mesh._cache.cache
     ):
         # store vertex normals if requested
         if unitize_normals:
             normals = util.unitize(mesh.vertex_normals)
```

### Comparing `trimesh-4.3.1/trimesh/exchange/load.py` & `trimesh-4.3.2/trimesh/exchange/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             )
         else:
             if file_type in ["svg", "dxf"]:
                 # call the dummy function to raise the import error
                 # this prevents the exception from being super opaque
                 load_path()
             else:
-                raise ValueError("File type: %s not supported" % file_type)
+                raise ValueError(f"File type: {file_type} not supported")
     finally:
         # close any opened files even if we crashed out
         if opened:
             file_obj.close()
 
     # add load metadata ('file_name') to each loaded geometry
     for i in util.make_sequence(loaded):
```

### Comparing `trimesh-4.3.1/trimesh/exchange/misc.py` & `trimesh-4.3.2/trimesh/exchange/misc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/obj.py` & `trimesh-4.3.2/trimesh/exchange/obj.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/off.py` & `trimesh-4.3.2/trimesh/exchange/off.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/ply.py` & `trimesh-4.3.2/trimesh/exchange/ply.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/stl.py` & `trimesh-4.3.2/trimesh/exchange/stl.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/threedxml.py` & `trimesh-4.3.2/trimesh/exchange/threedxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                     np.uint8
                 )
                 colors[material_id] = rgb
             texture = rend.find("{*}Attr[@Name='TextureImage']")
             if texture is not None:
                 tex_file, tex_id = texture.attrib["Value"].split(":")[-1].split("#")
                 rep_image = as_etree[tex_file].find(
-                    "{*}CATRepImage/{*}CATRepresentationImage[@id='%s']" % tex_id
+                    f"{{*}}CATRepImage/{{*}}CATRepresentationImage[@id='{tex_id}']"
                 )
                 if rep_image is not None:
                     image_file = rep_image.get("associatedFile", "").split(":")[-1]
                     images[material_id] = Image.open(archive[image_file])
 
         # copy indexes for instances of colors
         for MaterialDomainInstance in material_tree.iter("{*}MaterialDomainInstance"):
@@ -163,15 +163,15 @@
         mesh_normals = []
         mesh_vertices = []
         mesh_uv = []
         mesh_image = None
 
         if part_file not in as_etree and part_file in archive:
             # the data is stored in some binary format
-            util.log.warning("unable to load Rep %r" % part_file)
+            util.log.warning(f"unable to load Rep {part_file!r}")
             # data = archive[part_file]
             continue
 
         # the geometry is stored in a Rep
         for Rep in as_etree[part_file].iter("{*}Rep"):
             rep_faces = []  # faces sharing the same list of vertices
             vertices = Rep.find("{*}VertexBuffer/{*}Positions")
```

### Comparing `trimesh-4.3.1/trimesh/exchange/threemf.py` & `trimesh-4.3.2/trimesh/exchange/threemf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/urdf.py` & `trimesh-4.3.2/trimesh/exchange/urdf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/xaml.py` & `trimesh-4.3.2/trimesh/exchange/xaml.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/exchange/xyz.py` & `trimesh-4.3.2/trimesh/exchange/xyz.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/geometry.py` & `trimesh-4.3.2/trimesh/geometry.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/graph.py` & `trimesh-4.3.2/trimesh/graph.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/grouping.py` & `trimesh-4.3.2/trimesh/grouping.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/inertia.py` & `trimesh-4.3.2/trimesh/inertia.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/interfaces/blender.py` & `trimesh-4.3.2/trimesh/interfaces/blender.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,16 +99,16 @@
     Run an unwrap operation using blender.
     """
     if not exists:
         raise ValueError("No blender available!")
 
     # get the template from our resources folder
     template = resources.get_string("templates/blender_unwrap.py.template")
-    script = template.replace("$ANGLE_LIMIT", "%.6f" % angle_limit).replace(
-        "$ISLAND_MARGIN", "%.6f" % island_margin
+    script = template.replace("$ANGLE_LIMIT", f"{angle_limit:.6f}").replace(
+        "$ISLAND_MARGIN", f"{island_margin:.6f}"
     )
 
     with MeshScript(meshes=[mesh], script=script, exchange="obj", debug=debug) as blend:
         result = blend.run(_blender_executable + " --background --python $SCRIPT")
 
     for m in util.make_sequence(result):
         # blender returns actively incorrect face normals
```

### Comparing `trimesh-4.3.1/trimesh/interfaces/generic.py` & `trimesh-4.3.2/trimesh/interfaces/generic.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/interfaces/gmsh.py` & `trimesh-4.3.2/trimesh/interfaces/gmsh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/intersections.py` & `trimesh-4.3.2/trimesh/intersections.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/interval.py` & `trimesh-4.3.2/trimesh/interval.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/nsphere.py` & `trimesh-4.3.2/trimesh/nsphere.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/parent.py` & `trimesh-4.3.2/trimesh/parent.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/arc.py` & `trimesh-4.3.2/trimesh/path/arc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/creation.py` & `trimesh-4.3.2/trimesh/path/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/curve.py` & `trimesh-4.3.2/trimesh/path/curve.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/entities.py` & `trimesh-4.3.2/trimesh/path/entities.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/exchange/dxf.py` & `trimesh-4.3.2/trimesh/path/exchange/dxf.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/exchange/export.py` & `trimesh-4.3.2/trimesh/path/exchange/export.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/exchange/load.py` & `trimesh-4.3.2/trimesh/path/exchange/load.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/exchange/misc.py` & `trimesh-4.3.2/trimesh/path/exchange/misc.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/exchange/svg_io.py` & `trimesh-4.3.2/trimesh/path/exchange/svg_io.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/intersections.py` & `trimesh-4.3.2/trimesh/path/intersections.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/packing.py` & `trimesh-4.3.2/trimesh/path/packing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/path.py` & `trimesh-4.3.2/trimesh/path/path.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/polygons.py` & `trimesh-4.3.2/trimesh/path/polygons.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/raster.py` & `trimesh-4.3.2/trimesh/path/raster.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,20 @@
     Returns
     ------------
     raster : PIL.Image
       Rasterized version of input as `mode 1` image
     """
 
     if pitch is None:
-        pitch = path.extents.max() / 2048
+        if resolution is not None:
+            resolution = np.array(resolution, dtype=np.int64)
+            # establish pitch from passed resolution
+            pitch = (path.extents / (resolution + 2)).max()
+        else:
+            pitch = path.extents.max() / 2048
 
     if origin is None:
         origin = path.bounds[0] - (pitch * 2.0)
 
     # check inputs
     pitch = np.asanyarray(pitch, dtype=np.float64)
     origin = np.asanyarray(origin, dtype=np.float64)
```

### Comparing `trimesh-4.3.1/trimesh/path/repair.py` & `trimesh-4.3.2/trimesh/path/repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/segments.py` & `trimesh-4.3.2/trimesh/path/segments.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/simplify.py` & `trimesh-4.3.2/trimesh/path/simplify.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/traversal.py` & `trimesh-4.3.2/trimesh/path/traversal.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/path/util.py` & `trimesh-4.3.2/trimesh/path/util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/permutate.py` & `trimesh-4.3.2/trimesh/permutate.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/points.py` & `trimesh-4.3.2/trimesh/points.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/poses.py` & `trimesh-4.3.2/trimesh/poses.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/primitives.py` & `trimesh-4.3.2/trimesh/primitives.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/proximity.py` & `trimesh-4.3.2/trimesh/proximity.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/ray/ray_pyembree.py` & `trimesh-4.3.2/trimesh/ray/ray_pyembree.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/ray/ray_triangle.py` & `trimesh-4.3.2/trimesh/ray/ray_triangle.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/ray/ray_util.py` & `trimesh-4.3.2/trimesh/ray/ray_util.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/registration.py` & `trimesh-4.3.2/trimesh/registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,28 +144,34 @@
         a_to_b = np.dot(
             transformations.transform_around(flip, centroid),
             np.linalg.inv(search_to_points),
         )
 
         # run first pass ICP
         matrix, _junk, cost = icp(
-            a=points, b=search, initial=a_to_b, max_iterations=int(icp_first), scale=scale
+            a=points,
+            b=search,
+            initial=a_to_b,
+            max_iterations=int(icp_first),
+            scale=scale,
+            **kwargs,
         )
 
         # save transform and costs from ICP
         transforms[i] = matrix
         costs[i] = cost
 
     # run a final ICP refinement step
     matrix, _junk, cost = icp(
         a=points,
         b=search,
         initial=transforms[np.argmin(costs)],
         max_iterations=int(icp_final),
         scale=scale,
+        **kwargs,
     )
 
     # convert to per- point distance average
     cost /= len(points)
 
     # we picked the smaller mesh to construct the tree
     # on so we may have calculated a transform backwards
```

### Comparing `trimesh-4.3.1/trimesh/remesh.py` & `trimesh-4.3.2/trimesh/remesh.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/rendering.py` & `trimesh-4.3.2/trimesh/rendering.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/repair.py` & `trimesh-4.3.2/trimesh/repair.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resolvers.py` & `trimesh-4.3.2/trimesh/resolvers.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/__init__.py` & `trimesh-4.3.2/trimesh/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/creation.json` & `trimesh-4.3.2/trimesh/resources/creation.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/schema/gltf2.schema.zip` & `trimesh-4.3.2/trimesh/resources/schema/gltf2.schema.zip`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/schema/primitive/box.schema.json` & `trimesh-4.3.2/trimesh/resources/schema/primitive/box.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/schema/primitive/capsule.schema.json` & `trimesh-4.3.2/trimesh/resources/schema/primitive/capsule.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/schema/primitive/cylinder.schema.json` & `trimesh-4.3.2/trimesh/resources/schema/primitive/cylinder.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/schema/primitive/extrusion.schema.json` & `trimesh-4.3.2/trimesh/resources/schema/primitive/extrusion.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/schema/primitive/scenegraph.schema.json` & `trimesh-4.3.2/trimesh/resources/schema/primitive/scenegraph.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/schema/primitive/sphere.schema.json` & `trimesh-4.3.2/trimesh/resources/schema/primitive/sphere.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/schema/primitive/trimesh.schema.json` & `trimesh-4.3.2/trimesh/resources/schema/primitive/trimesh.schema.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/schema/urdf.xsd` & `trimesh-4.3.2/trimesh/resources/schema/urdf.xsd`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/templates/blender_boolean.py.tmpl` & `trimesh-4.3.2/trimesh/resources/templates/blender_boolean.py.tmpl`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/templates/blender_unwrap.py.template` & `trimesh-4.3.2/trimesh/resources/templates/blender_unwrap.py.template`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/templates/dxf.json` & `trimesh-4.3.2/trimesh/resources/templates/dxf.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/templates/viewer.zip` & `trimesh-4.3.2/trimesh/resources/templates/viewer.zip`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/resources/units_to_inches.json` & `trimesh-4.3.2/trimesh/resources/units_to_inches.json`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/sample.py` & `trimesh-4.3.2/trimesh/sample.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/scene/cameras.py` & `trimesh-4.3.2/trimesh/scene/cameras.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/scene/lighting.py` & `trimesh-4.3.2/trimesh/scene/lighting.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/scene/scene.py` & `trimesh-4.3.2/trimesh/scene/scene.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/scene/transforms.py` & `trimesh-4.3.2/trimesh/scene/transforms.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/schemas.py` & `trimesh-4.3.2/trimesh/schemas.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/smoothing.py` & `trimesh-4.3.2/trimesh/smoothing.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/transformations.py` & `trimesh-4.3.2/trimesh/transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -749,15 +749,15 @@
     M = np.array(matrix, dtype=np.float64, copy=False)
     M33 = M[:3, :3]
     # normal: cross independent eigenvectors corresponding to the eigenvalue 1
     w, V = np.linalg.eig(M33)
 
     i = np.where(abs(np.real(w) - 1.0) < 1e-4)[0]
     if len(i) < 2:
-        raise ValueError("no two linear independent eigenvectors found %s" % w)
+        raise ValueError(f"no two linear independent eigenvectors found {w}")
     V = np.real(V[:, i]).squeeze().T
     lenorm = -1.0
     for i0, i1 in ((0, 1), (0, 2), (1, 2)):
         n = np.cross(V[i0], V[i1])
         w = vector_norm(n)
         if w > lenorm:
             lenorm = w
```

### Comparing `trimesh-4.3.1/trimesh/triangles.py` & `trimesh-4.3.2/trimesh/triangles.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     ----------
     aligned : (n,) bool
       Are normals aligned with triangles
     """
     triangles = np.asanyarray(triangles, dtype=np.float64)
     if not util.is_shape(triangles, (-1, 3, 3), allow_zeros=True):
         raise ValueError(
-            "triangles must have shape (n, 3, 3), got %s" % str(triangles.shape)
+            f"triangles must have shape (n, 3, 3), got {triangles.shape!s}"
         )
     normals_compare = np.asanyarray(normals_compare, dtype=np.float64)
 
     calculated, valid = normals(triangles)
     if normals_compare.shape == (3,):
         # single comparison vector case
         difference = np.dot(calculated, normals_compare)
```

### Comparing `trimesh-4.3.1/trimesh/typed.py` & `trimesh-4.3.2/trimesh/typed.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/units.py` & `trimesh-4.3.2/trimesh/units.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/util.py` & `trimesh-4.3.2/trimesh/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -2254,17 +2254,17 @@
             self[k] = v
 
     def __getitem__(self, key):
         return self._dict[key]
 
     def __setitem__(self, key, value):
         if not isinstance(key, str):
-            raise ValueError("key must be a string, got %s" % str(key))
+            raise ValueError(f"key must be a string, got {key!s}")
         if key in self:
-            raise KeyError("Cannot set new value to existing key %s" % key)
+            raise KeyError(f"Cannot set new value to existing key {key}")
         if not callable(value):
             raise ValueError("Cannot set value which is not callable.")
         self._dict[key] = value
 
     def __iter__(self):
         return iter(self._dict)
```

### Comparing `trimesh-4.3.1/trimesh/version.py` & `trimesh-4.3.2/trimesh/version.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/viewer/__init__.py` & `trimesh-4.3.2/trimesh/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/viewer/notebook.py` & `trimesh-4.3.2/trimesh/viewer/notebook.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/viewer/trackball.py` & `trimesh-4.3.2/trimesh/viewer/trackball.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/viewer/widget.py` & `trimesh-4.3.2/trimesh/viewer/widget.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/viewer/windowed.py` & `trimesh-4.3.2/trimesh/viewer/windowed.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/visual/__init__.py` & `trimesh-4.3.2/trimesh/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/visual/base.py` & `trimesh-4.3.2/trimesh/visual/base.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/visual/color.py` & `trimesh-4.3.2/trimesh/visual/color.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/visual/gloss.py` & `trimesh-4.3.2/trimesh/visual/gloss.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/visual/material.py` & `trimesh-4.3.2/trimesh/visual/material.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/visual/objects.py` & `trimesh-4.3.2/trimesh/visual/objects.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/visual/texture.py` & `trimesh-4.3.2/trimesh/visual/texture.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/voxel/base.py` & `trimesh-4.3.2/trimesh/voxel/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self._cache = caching.Cache(id_function=self._data.__hash__)
 
         self.metadata = {}
         # update the mesh metadata with passed metadata
         if isinstance(metadata, dict):
             self.metadata.update(metadata)
         elif metadata is not None:
-            raise ValueError("metadata should be a dict or None, got %s" % str(metadata))
+            raise ValueError(f"metadata should be a dict or None, got {metadata!s}")
 
     def __hash__(self):
         """
         Get the hash of the current transformation matrix.
 
         Returns
         ------------
@@ -62,21 +62,21 @@
         return self._data["encoding"]
 
     @encoding.setter
     def encoding(self, encoding):
         if isinstance(encoding, np.ndarray):
             encoding = DenseEncoding(encoding)
         elif not isinstance(encoding, Encoding):
-            raise ValueError("encoding must be an Encoding, got %s" % str(encoding))
+            raise ValueError(f"encoding must be an Encoding, got {encoding!s}")
         if len(encoding.shape) != 3:
             raise ValueError(
-                "encoding must be rank 3, got shape %s" % str(encoding.shape)
+                f"encoding must be rank 3, got shape {encoding.shape!s}"
             )
         if encoding.dtype != bool:
-            raise ValueError("encoding must be binary, got %s" % encoding.dtype)
+            raise ValueError(f"encoding must be binary, got {encoding.dtype}")
         self._data["encoding"] = encoding
 
     @property
     def transform(self):
         """4x4 homogeneous transformation matrix."""
         return self._transform.matrix
```

### Comparing `trimesh-4.3.1/trimesh/voxel/creation.py` & `trimesh-4.3.2/trimesh/voxel/creation.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/voxel/encoding.py` & `trimesh-4.3.2/trimesh/voxel/encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         """
         data = caching.DataStore()
         super().__init__(data)
         data["indices"] = indices
         data["values"] = values
         indices = data["indices"]
         if len(indices.shape) != 2:
-            raise ValueError("indices must be 2D, got shaped %s" % str(indices.shape))
+            raise ValueError(f"indices must be 2D, got shaped {indices.shape!s}")
         if data["values"].shape != (indices.shape[0],):
             raise ValueError(
                 "values and indices shapes inconsistent: {} and {}".format(
                     data["values"], data["indices"]
                 )
             )
         if shape is None:
@@ -507,15 +507,15 @@
 
     @caching.cache_decorator
     def size(self):
         return runlength.rle_length(self._data)
 
     def _flip(self, axes):
         if axes != (0,):
-            raise ValueError("encoding is 1D - cannot flip on axis %s" % str(axes))
+            raise ValueError(f"encoding is 1D - cannot flip on axis {axes!s}")
         return RunLengthEncoding(runlength.rle_reverse(self._data))
 
     @caching.cache_decorator
     def sparse_components(self):
         return runlength.rle_to_sparse(self._data)
 
     @caching.cache_decorator
@@ -612,15 +612,15 @@
 
     @caching.cache_decorator
     def size(self):
         return runlength.brle_length(self._data)
 
     def _flip(self, axes):
         if axes != (0,):
-            raise ValueError("encoding is 1D - cannot flip on axis %s" % str(axes))
+            raise ValueError(f"encoding is 1D - cannot flip on axis {axes!s}")
         return BinaryRunLengthEncoding(runlength.brle_reverse(self._data))
 
     @property
     def sparse_components(self):
         return self.sparse_indices, self.sparse_values
 
     @caching.cache_decorator
@@ -812,25 +812,25 @@
 
     Dense equivalent is `np.transpose`
     """
 
     def __init__(self, base_encoding, perm):
         if not isinstance(base_encoding, Encoding):
             raise ValueError(
-                "base_encoding must be an Encoding, got %s" % str(base_encoding)
+                f"base_encoding must be an Encoding, got {base_encoding!s}"
             )
         if len(base_encoding.shape) != len(perm):
             raise ValueError(
                 "base_encoding has %d ndims - cannot transpose with perm %s"
                 % (base_encoding.ndims, str(perm))
             )
         super().__init__(base_encoding)
         perm = np.array(perm, dtype=np.int64)
         if not all(i in perm for i in range(base_encoding.ndims)):
-            raise ValueError("perm %s is not a valid permutation" % str(perm))
+            raise ValueError(f"perm {perm!s} is not a valid permutation")
         inv_perm = np.empty_like(perm)
         inv_perm[perm] = np.arange(base_encoding.ndims)
         self._perm = perm
         self._inv_perm = inv_perm
 
     def transpose(self, perm):
         return _transposed(self._data, [self._perm[p] for p in perm])
@@ -892,15 +892,15 @@
         if isinstance(axes, np.ndarray) and axes.size == 1:
             axes = (axes.item(),)
         elif isinstance(axes, int):
             axes = (axes,)
         axes = tuple(a + ndims if a < 0 else a for a in axes)
         self._axes = tuple(sorted(axes))
         if len(set(self._axes)) != len(self._axes):
-            raise ValueError("Axes cannot contain duplicates, got %s" % str(self._axes))
+            raise ValueError(f"Axes cannot contain duplicates, got {self._axes!s}")
         super().__init__(encoding)
         if not all(0 <= a < self._data.ndims for a in axes):
             raise ValueError(
                 "Invalid axes %s for %d-d encoding" % (str(axes), self._data.ndims)
             )
 
     def _to_base_indices(self, indices):
```

### Comparing `trimesh-4.3.1/trimesh/voxel/morphology.py` & `trimesh-4.3.2/trimesh/voxel/morphology.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,43 +19,43 @@
 def _dense(encoding, rank=None):
     if isinstance(encoding, np.ndarray):
         dense = encoding
     elif isinstance(encoding, enc.Encoding):
         dense = encoding.dense
     else:
         raise ValueError(
-            "encoding must be np.ndarray or Encoding, got %s" % str(encoding)
+            f"encoding must be np.ndarray or Encoding, got {encoding!s}"
         )
     if rank:
         _assert_rank(dense, rank)
     return dense
 
 
 def _sparse_indices(encoding, rank=None):
     if isinstance(encoding, np.ndarray):
         sparse_indices = encoding
     elif isinstance(encoding, enc.Encoding):
         sparse_indices = encoding.sparse_indices
     else:
         raise ValueError(
-            "encoding must be np.ndarray or Encoding, got %s" % str(encoding)
+            f"encoding must be np.ndarray or Encoding, got {encoding!s}"
         )
 
     _assert_sparse_rank(sparse_indices, 3)
     return sparse_indices
 
 
 def _assert_rank(value, rank):
     if len(value.shape) != rank:
         raise ValueError("Expected rank %d, got shape %s" % (rank, str(value.shape)))
 
 
 def _assert_sparse_rank(value, rank=None):
     if len(value.shape) != 2:
-        raise ValueError("sparse_indices must be rank 2, got shape %s" % str(value.shape))
+        raise ValueError(f"sparse_indices must be rank 2, got shape {value.shape!s}")
     if rank is not None:
         if value.shape[-1] != rank:
             raise ValueError(
                 "sparse_indices.shape[1] must be %d, got %d" % (rank, value.shape[-1])
             )
```

### Comparing `trimesh-4.3.1/trimesh/voxel/ops.py` & `trimesh-4.3.2/trimesh/voxel/ops.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh/voxel/runlength.py` & `trimesh-4.3.2/trimesh/voxel/runlength.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     ValueError if vals it not None and shape is not (2,)
     """
     if vals is None:
         vals = _ft
     else:
         vals = np.asarray(vals)
         if vals.shape != (2,):
-            raise ValueError("vals.shape must be (2,), got %s" % (vals.shape))
+            raise ValueError(f"vals.shape must be (2,), got {vals.shape}")
     ft = np.repeat(_ft[np.newaxis, :], (len(brle_data) + 1) // 2, axis=0).flatten()
     return np.repeat(ft[: len(brle_data)], brle_data).flatten()
 
 
 def rle_to_dense(rle_data, dtype=np.int64):
     """Get the dense decoding of the associated run length encoded data."""
     values, counts = np.split(np.reshape(rle_data, (-1, 2)), 2, axis=-1)
```

### Comparing `trimesh-4.3.1/trimesh/voxel/transforms.py` & `trimesh-4.3.2/trimesh/voxel/transforms.py`

 * *Files identical despite different names*

### Comparing `trimesh-4.3.1/trimesh.egg-info/PKG-INFO` & `trimesh-4.3.2/trimesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimesh
-Version: 4.3.1
+Version: 4.3.2
 Summary: Import, export, process, analyze and view triangular meshes.
 Author-email: Michael Dawson-Haggerty <mikedh@kerfed.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Michael Dawson-Haggerty
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `trimesh-4.3.1/trimesh.egg-info/SOURCES.txt` & `trimesh-4.3.2/trimesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

