# Comparing `tmp/stadiamaps-2.1.0.tar.gz` & `tmp/stadiamaps-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadiamaps-2.1.0.tar", last modified: Thu Mar 21 09:18:30 2024, max compression
+gzip compressed data, was "stadiamaps-3.0.0.tar", last modified: Tue Apr 30 07:04:56 2024, max compression
```

## Comparing `stadiamaps-2.1.0.tar` & `stadiamaps-3.0.0.tar`

### file list

```diff
@@ -1,260 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:18:30.640718 stadiamaps-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-21 09:18:30.640718 stadiamaps-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-21 09:18:30.640718 stadiamaps-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:18:30.596718 stadiamaps-2.1.0/stadiamaps/
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:18:30.596718 stadiamaps-2.1.0/stadiamaps/api/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   147742 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/api/geocoding_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29289 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/api/geospatial_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    80984 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/api/routing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25814 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15562 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:18:30.616718 stadiamaps-2.1.0/stadiamaps/models/
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/admin_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/administrative.py
--rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/auto_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/auto_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/base_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/base_trace_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/bicycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/bicycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/bike_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/directions_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/distance_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/edge_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/edge_use.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/end_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/geo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/geo_json_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/geo_json_geometry_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/geo_json_line_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/geo_json_line_string_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/geo_json_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/geo_json_point_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/geo_json_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/geo_json_polygon_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/geocoding_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/height_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/height_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/highway_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/intersecting_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/isochrone_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/isochrone_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/isochrone_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/isochrone_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/isochrone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/locate_detailed_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/locate_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/locate_edge_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/locate_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/locate_node_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/locate_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/maneuver_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/maneuver_sign_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/map_match_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/map_match_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/map_match_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/map_match_route_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/map_match_route_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/map_match_trace_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/map_match_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/map_match_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/matched_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/matrix_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/matrix_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/matrix_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/matrix_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/motor_scooter_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/motor_scooter_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/motorcycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/motorcycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/nearest_roads_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/node_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/node_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/optimized_route_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/pedestrian_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/pelias_geo_json_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/pelias_geo_json_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/pelias_geo_json_properties_addendum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/pelias_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/pelias_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/pelias_response_geocoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/pelias_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/road_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/route_leg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/route_maneuver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/route_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/route_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/route_response_alternates_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/route_response_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/route_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/route_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/routing_response_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/routing_response_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/routing_waypoint_all_of_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/simple_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/simple_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/speeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/trace_attribute_filter_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/trace_attribute_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/trace_attributes_base_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/trace_attributes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/trace_attributes_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/trace_attributes_request_all_of_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/trace_attributes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/trace_attributes_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/trace_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/travel_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/traversability.py
--rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/truck_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/truck_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/tz_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/valhalla_languages.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/valhalla_long_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/models/warning.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/stadiamaps/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:18:30.640718 stadiamaps-2.1.0/stadiamaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-21 09:18:30.000000 stadiamaps-2.1.0/stadiamaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-03-21 09:18:30.000000 stadiamaps-2.1.0/stadiamaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 09:18:30.000000 stadiamaps-2.1.0/stadiamaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-21 09:18:30.000000 stadiamaps-2.1.0/stadiamaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-21 09:18:30.000000 stadiamaps-2.1.0/stadiamaps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:18:30.640718 stadiamaps-2.1.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:18:30.640718 stadiamaps-2.1.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/integration/test_eu_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/integration/test_gecoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/integration/test_geospatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/integration/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_admin_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_administrative.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_auto_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_auto_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_base_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_base_trace_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_bicycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_bicycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_bike_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_directions_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_distance_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_edge_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_edge_use.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_end_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geo_json_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geo_json_geometry_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geo_json_line_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geo_json_line_string_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geo_json_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geo_json_point_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geo_json_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geo_json_polygon_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geocoding_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geocoding_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_geospatial_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_height_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_height_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_highway_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_intersecting_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_isochrone_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_isochrone_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_isochrone_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_isochrone_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_isochrone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_locate_detailed_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_locate_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_locate_edge_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_locate_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_locate_node_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_locate_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_maneuver_sign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_maneuver_sign_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_map_match_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_map_match_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_map_match_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_map_match_route_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_map_match_route_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_map_match_trace_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_map_match_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_map_match_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_matched_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_matrix_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_matrix_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_matrix_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_matrix_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_motor_scooter_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_motor_scooter_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_motorcycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_motorcycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_nearest_roads_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_node_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_node_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_optimized_route_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_pedestrian_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_pelias_geo_json_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_pelias_geo_json_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_pelias_geo_json_properties_addendum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_pelias_geo_json_properties_addendum_osm.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_pelias_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_pelias_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_pelias_response_geocoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_pelias_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_road_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_route_leg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_route_maneuver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_route_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_route_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_route_response_alternates_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_route_response_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_route_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_route_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_routing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_routing_response_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_routing_response_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_routing_waypoint_all_of_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_simple_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_simple_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_speeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_trace_attribute_filter_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_trace_attribute_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_trace_attributes_base_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_trace_attributes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_trace_attributes_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_trace_attributes_request_all_of_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_trace_attributes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_trace_attributes_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_trace_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_travel_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_traversability.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_truck_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_truck_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_tz_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_valhalla_languages.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_valhalla_long_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-21 09:18:25.000000 stadiamaps-2.1.0/test/test_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.947810 stadiamaps-3.0.0/stadiamaps/
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.951810 stadiamaps-3.0.0/stadiamaps/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   147742 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api/geocoding_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29289 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api/geospatial_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80984 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api/routing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25932 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15562 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.971810 stadiamaps-3.0.0/stadiamaps/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/admin_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/administrative.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/auto_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/auto_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/base_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/base_trace_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11693 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/bicycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/bicycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/bike_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/directions_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/distance_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/edge_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/edge_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/end_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_geometry_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_line_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_line_string_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_point_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geo_json_polygon_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/geocoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/height_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/height_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/highway_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/intersecting_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/isochrone_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/isochrone_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/isochrone_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/isochrone_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/isochrone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_detailed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_edge_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_node_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/locate_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/low_speed_vehicle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/maneuver_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/maneuver_sign_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_route_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_trace_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/map_match_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matched_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matrix_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matrix_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matrix_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matrix_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/matrix_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13848 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/motor_scooter_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/motor_scooter_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/motorcycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/motorcycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/nearest_roads_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/node_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/optimized_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pedestrian_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties_addendum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_response_geocoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/pelias_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/road_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_leg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_maneuver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_response_alternates_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_response_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/route_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/routing_response_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/routing_response_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/routing_waypoint_all_of_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/simple_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/simple_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/speeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attribute_filter_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attribute_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request_all_of_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_attributes_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/trace_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/travel_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/traversability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/truck_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/truck_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/tz_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/valhalla_languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/valhalla_long_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/models/warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/stadiamaps/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/stadiamaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-30 07:04:56.000000 stadiamaps-3.0.0/stadiamaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-30 07:04:56.000000 stadiamaps-3.0.0/stadiamaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:04:56.000000 stadiamaps-3.0.0/stadiamaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 07:04:56.000000 stadiamaps-3.0.0/stadiamaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 07:04:56.000000 stadiamaps-3.0.0/stadiamaps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:56.991810 stadiamaps-3.0.0/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/integration/test_eu_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/integration/test_gecoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/integration/test_geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13646 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/integration/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_admin_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_administrative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_auto_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_auto_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_base_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_base_trace_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_bicycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_bicycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_bike_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_directions_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_distance_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_edge_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_edge_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_end_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_geometry_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_line_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_line_string_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_point_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geo_json_polygon_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geocoding_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geocoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_geospatial_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_height_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_height_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_highway_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_intersecting_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_isochrone_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_isochrone_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_isochrone_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_isochrone_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_isochrone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_detailed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_edge_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_node_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_locate_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_low_speed_vehicle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_maneuver_sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_maneuver_sign_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_route_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_trace_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_map_match_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matched_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matrix_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matrix_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matrix_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matrix_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_matrix_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_motor_scooter_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_motor_scooter_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_motorcycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_motorcycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_nearest_roads_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_optimized_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pedestrian_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_geo_json_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_geo_json_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_geo_json_properties_addendum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_geo_json_properties_addendum_osm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_response_geocoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_pelias_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_road_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_leg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_maneuver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_response_alternates_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_response_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_route_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_response_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_response_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_routing_waypoint_all_of_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_simple_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_simple_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_speeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attribute_filter_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attribute_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_request_all_of_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_attributes_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_trace_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_travel_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_traversability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_truck_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_truck_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_tz_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_valhalla_languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_valhalla_long_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-30 07:04:52.000000 stadiamaps-3.0.0/test/test_warning.py
```

### Comparing `stadiamaps-2.1.0/LICENSE.txt` & `stadiamaps-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/PKG-INFO` & `stadiamaps-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadiamaps
-Version: 2.1.0
+Version: 3.0.0
 Summary: Stadia Maps Geospatial APIs
 Home-page: https://github.com/stadiamaps/stadiamaps-api-py
 Author: Stadia Maps Support
 Author-email: support@stadiamaps.com
 Keywords: OpenAPI,OpenAPI-Generator,Stadia Maps Geospatial APIs
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `stadiamaps-2.1.0/README.md` & `stadiamaps-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/pyproject.toml` & `stadiamaps-3.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stadiamaps"
-version = "2.1.0"
+version = "3.0.0"
 description = "Stadia Maps Geospatial APIs"
 authors = ["Stadia Maps Support <support@stadiamaps.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/stadiamaps/stadiamaps-api-py"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Stadia Maps Geospatial APIs"]
 include = ["stadiamaps/py.typed"]
```

### Comparing `stadiamaps-2.1.0/setup.py` & `stadiamaps-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "stadiamaps"
-VERSION = "2.1.0"
+VERSION = "3.0.0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `stadiamaps-2.1.0/stadiamaps/__init__.py` & `stadiamaps-3.0.0/stadiamaps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2.1.0"
+__version__ = "3.0.0"
 
 # import apis into sdk package
 from stadiamaps.api.geocoding_api import GeocodingApi
 from stadiamaps.api.geospatial_api import GeospatialApi
 from stadiamaps.api.routing_api import RoutingApi
 
 # import ApiClient
@@ -68,26 +68,28 @@
 from stadiamaps.models.isochrone_request import IsochroneRequest
 from stadiamaps.models.isochrone_response import IsochroneResponse
 from stadiamaps.models.locate_detailed_edge import LocateDetailedEdge
 from stadiamaps.models.locate_edge import LocateEdge
 from stadiamaps.models.locate_edge_info import LocateEdgeInfo
 from stadiamaps.models.locate_node import LocateNode
 from stadiamaps.models.locate_object import LocateObject
+from stadiamaps.models.low_speed_vehicle_costing_options import LowSpeedVehicleCostingOptions
 from stadiamaps.models.maneuver_sign import ManeuverSign
 from stadiamaps.models.maneuver_sign_element import ManeuverSignElement
 from stadiamaps.models.map_match_costing_model import MapMatchCostingModel
 from stadiamaps.models.map_match_request import MapMatchRequest
 from stadiamaps.models.map_match_route_response import MapMatchRouteResponse
 from stadiamaps.models.map_match_trace_options import MapMatchTraceOptions
 from stadiamaps.models.map_match_waypoint import MapMatchWaypoint
 from stadiamaps.models.matched_point import MatchedPoint
 from stadiamaps.models.matrix_costing_model import MatrixCostingModel
 from stadiamaps.models.matrix_distance import MatrixDistance
 from stadiamaps.models.matrix_request import MatrixRequest
 from stadiamaps.models.matrix_response import MatrixResponse
+from stadiamaps.models.matrix_waypoint import MatrixWaypoint
 from stadiamaps.models.motor_scooter_costing_options import MotorScooterCostingOptions
 from stadiamaps.models.motorcycle_costing_options import MotorcycleCostingOptions
 from stadiamaps.models.nearest_roads_request import NearestRoadsRequest
 from stadiamaps.models.node_id import NodeId
 from stadiamaps.models.node_type import NodeType
 from stadiamaps.models.optimized_route_request import OptimizedRouteRequest
 from stadiamaps.models.pedestrian_costing_options import PedestrianCostingOptions
```

### Comparing `stadiamaps-2.1.0/stadiamaps/api/geocoding_api.py` & `stadiamaps-3.0.0/stadiamaps/api/geocoding_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `stadiamaps-2.1.0/stadiamaps/api/geospatial_api.py` & `stadiamaps-3.0.0/stadiamaps/api/geospatial_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `stadiamaps-2.1.0/stadiamaps/api/routing_api.py` & `stadiamaps-3.0.0/stadiamaps/api/routing_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `stadiamaps-2.1.0/stadiamaps/api_client.py` & `stadiamaps-3.0.0/stadiamaps/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.1.0/python'
+        self.user_agent = 'OpenAPI-Generator/3.0.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
@@ -477,14 +477,16 @@
         if collection_formats is None:
             collection_formats = {}
         for k, v in params.items() if isinstance(params, dict) else params:
             if isinstance(v, bool):
                 v = str(v).lower()
             if isinstance(v, (int, float)):
                 v = str(v)
+            if isinstance(v, Enum):
+                v = str(v.value)
             if isinstance(v, dict):
                 v = json.dumps(v)
 
             if k in collection_formats:
                 collection_format = collection_formats[k]
                 if collection_format == 'multi':
                     new_params.extend((k, str(value)) for value in v)
@@ -494,15 +496,15 @@
                     elif collection_format == 'tsv':
                         delimiter = '\t'
                     elif collection_format == 'pipes':
                         delimiter = '|'
                     else:  # csv is the default
                         delimiter = ','
                     new_params.append(
-                        (k, delimiter.join(quote(str(value)) for value in v))
+                        (k, delimiter.join(quote(str(value.value) if isinstance(value, Enum) else str(value)) for value in v))
                     )
             else:
                 new_params.append((k, quote(str(v))))
 
         return "&".join(["=".join(map(str, item)) for item in new_params])
 
     def files_parameters(self, files=None):
```

### Comparing `stadiamaps-2.1.0/stadiamaps/api_response.py` & `stadiamaps-3.0.0/stadiamaps/api_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/configuration.py` & `stadiamaps-3.0.0/stadiamaps/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -395,16 +395,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 6.1.0\n"\
-               "SDK Package Version: 2.1.0".\
+               "Version of the API: 6.3.0\n"\
+               "SDK Package Version: 3.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `stadiamaps-2.1.0/stadiamaps/exceptions.py` & `stadiamaps-3.0.0/stadiamaps/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/__init__.py` & `stadiamaps-3.0.0/stadiamaps/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -49,26 +49,28 @@
 from stadiamaps.models.isochrone_request import IsochroneRequest
 from stadiamaps.models.isochrone_response import IsochroneResponse
 from stadiamaps.models.locate_detailed_edge import LocateDetailedEdge
 from stadiamaps.models.locate_edge import LocateEdge
 from stadiamaps.models.locate_edge_info import LocateEdgeInfo
 from stadiamaps.models.locate_node import LocateNode
 from stadiamaps.models.locate_object import LocateObject
+from stadiamaps.models.low_speed_vehicle_costing_options import LowSpeedVehicleCostingOptions
 from stadiamaps.models.maneuver_sign import ManeuverSign
 from stadiamaps.models.maneuver_sign_element import ManeuverSignElement
 from stadiamaps.models.map_match_costing_model import MapMatchCostingModel
 from stadiamaps.models.map_match_request import MapMatchRequest
 from stadiamaps.models.map_match_route_response import MapMatchRouteResponse
 from stadiamaps.models.map_match_trace_options import MapMatchTraceOptions
 from stadiamaps.models.map_match_waypoint import MapMatchWaypoint
 from stadiamaps.models.matched_point import MatchedPoint
 from stadiamaps.models.matrix_costing_model import MatrixCostingModel
 from stadiamaps.models.matrix_distance import MatrixDistance
 from stadiamaps.models.matrix_request import MatrixRequest
 from stadiamaps.models.matrix_response import MatrixResponse
+from stadiamaps.models.matrix_waypoint import MatrixWaypoint
 from stadiamaps.models.motor_scooter_costing_options import MotorScooterCostingOptions
 from stadiamaps.models.motorcycle_costing_options import MotorcycleCostingOptions
 from stadiamaps.models.nearest_roads_request import NearestRoadsRequest
 from stadiamaps.models.node_id import NodeId
 from stadiamaps.models.node_type import NodeType
 from stadiamaps.models.optimized_route_request import OptimizedRouteRequest
 from stadiamaps.models.pedestrian_costing_options import PedestrianCostingOptions
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/access.py` & `stadiamaps-3.0.0/stadiamaps/models/access.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/admin_region.py` & `stadiamaps-3.0.0/stadiamaps/models/admin_region.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/administrative.py` & `stadiamaps-3.0.0/stadiamaps/models/administrative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/auto_costing_options.py` & `stadiamaps-3.0.0/stadiamaps/models/auto_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/auto_costing_options_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/auto_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/base_costing_options.py` & `stadiamaps-3.0.0/stadiamaps/models/base_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/base_trace_request.py` & `stadiamaps-3.0.0/stadiamaps/models/base_trace_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/bicycle_costing_options.py` & `stadiamaps-3.0.0/stadiamaps/models/bicycle_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/bicycle_costing_options_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/bicycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/bike_network.py` & `stadiamaps-3.0.0/stadiamaps/models/bike_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/contour.py` & `stadiamaps-3.0.0/stadiamaps/models/contour.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/coordinate.py` & `stadiamaps-3.0.0/stadiamaps/models/coordinate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/costing_model.py` & `stadiamaps-3.0.0/stadiamaps/models/costing_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,15 +17,15 @@
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
 class CostingModel(str, Enum):
     """
-    Costing models for determining the most optimal route to take. Note that bikeshare and motorcycle are still in beta. While Valhalla supports multimodal routing, we do not currently process transit data and have excluded it from the list. See https://valhalla.github.io/valhalla/api/turn-by-turn/api-reference/#costing-models for detailed descriptions of each model.
+    A model which influences the routing based on the type of travel. The costing model affects parameters ranging from which roads are legally accessible to preferences based on comfort or speed. See https://valhalla.github.io/valhalla/api/turn-by-turn/api-reference/#costing-models for in-depth descriptions of each costing model.
     """
 
     """
     allowed enum values
     """
     AUTO = 'auto'
     BUS = 'bus'
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/costing_options.py` & `stadiamaps-3.0.0/stadiamaps/models/costing_options.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,14 +18,15 @@
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List, Optional
 from stadiamaps.models.auto_costing_options import AutoCostingOptions
 from stadiamaps.models.bicycle_costing_options import BicycleCostingOptions
+from stadiamaps.models.low_speed_vehicle_costing_options import LowSpeedVehicleCostingOptions
 from stadiamaps.models.motor_scooter_costing_options import MotorScooterCostingOptions
 from stadiamaps.models.motorcycle_costing_options import MotorcycleCostingOptions
 from stadiamaps.models.pedestrian_costing_options import PedestrianCostingOptions
 from stadiamaps.models.truck_costing_options import TruckCostingOptions
 from typing import Optional, Set
 from typing_extensions import Self
 
@@ -37,16 +38,17 @@
     bus: Optional[AutoCostingOptions] = None
     taxi: Optional[AutoCostingOptions] = None
     truck: Optional[TruckCostingOptions] = None
     bicycle: Optional[BicycleCostingOptions] = None
     motor_scooter: Optional[MotorScooterCostingOptions] = None
     motorcycle: Optional[MotorcycleCostingOptions] = None
     pedestrian: Optional[PedestrianCostingOptions] = None
+    low_speed_vehicle: Optional[LowSpeedVehicleCostingOptions] = None
     additional_properties: Dict[str, Any] = {}
-    __properties: ClassVar[List[str]] = ["auto", "bus", "taxi", "truck", "bicycle", "motor_scooter", "motorcycle", "pedestrian"]
+    __properties: ClassVar[List[str]] = ["auto", "bus", "taxi", "truck", "bicycle", "motor_scooter", "motorcycle", "pedestrian", "low_speed_vehicle"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -105,14 +107,17 @@
             _dict['motor_scooter'] = self.motor_scooter.to_dict()
         # override the default output from pydantic by calling `to_dict()` of motorcycle
         if self.motorcycle:
             _dict['motorcycle'] = self.motorcycle.to_dict()
         # override the default output from pydantic by calling `to_dict()` of pedestrian
         if self.pedestrian:
             _dict['pedestrian'] = self.pedestrian.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of low_speed_vehicle
+        if self.low_speed_vehicle:
+            _dict['low_speed_vehicle'] = self.low_speed_vehicle.to_dict()
         # puts key-value pairs in additional_properties in the top level
         if self.additional_properties is not None:
             for _key, _value in self.additional_properties.items():
                 _dict[_key] = _value
 
         return _dict
 
@@ -129,15 +134,16 @@
             "auto": AutoCostingOptions.from_dict(obj["auto"]) if obj.get("auto") is not None else None,
             "bus": AutoCostingOptions.from_dict(obj["bus"]) if obj.get("bus") is not None else None,
             "taxi": AutoCostingOptions.from_dict(obj["taxi"]) if obj.get("taxi") is not None else None,
             "truck": TruckCostingOptions.from_dict(obj["truck"]) if obj.get("truck") is not None else None,
             "bicycle": BicycleCostingOptions.from_dict(obj["bicycle"]) if obj.get("bicycle") is not None else None,
             "motor_scooter": MotorScooterCostingOptions.from_dict(obj["motor_scooter"]) if obj.get("motor_scooter") is not None else None,
             "motorcycle": MotorcycleCostingOptions.from_dict(obj["motorcycle"]) if obj.get("motorcycle") is not None else None,
-            "pedestrian": PedestrianCostingOptions.from_dict(obj["pedestrian"]) if obj.get("pedestrian") is not None else None
+            "pedestrian": PedestrianCostingOptions.from_dict(obj["pedestrian"]) if obj.get("pedestrian") is not None else None,
+            "low_speed_vehicle": LowSpeedVehicleCostingOptions.from_dict(obj["low_speed_vehicle"]) if obj.get("low_speed_vehicle") is not None else None
         })
         # store additional fields in additional_properties
         for _key in obj.keys():
             if _key not in cls.__properties:
                 _obj.additional_properties[_key] = obj.get(_key)
 
         return _obj
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/directions_options.py` & `stadiamaps-3.0.0/stadiamaps/models/directions_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/distance_unit.py` & `stadiamaps-3.0.0/stadiamaps/models/distance_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/edge_sign.py` & `stadiamaps-3.0.0/stadiamaps/models/edge_sign.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/edge_use.py` & `stadiamaps-3.0.0/stadiamaps/models/edge_use.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/end_node.py` & `stadiamaps-3.0.0/stadiamaps/models/end_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/geo_attributes.py` & `stadiamaps-3.0.0/stadiamaps/models/geo_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/geo_json_geometry.py` & `stadiamaps-3.0.0/stadiamaps/models/geo_json_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/geo_json_geometry_base.py` & `stadiamaps-3.0.0/stadiamaps/models/geo_json_geometry_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/geo_json_line_string.py` & `stadiamaps-3.0.0/stadiamaps/models/geo_json_line_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/geo_json_line_string_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/geo_json_line_string_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/geo_json_point.py` & `stadiamaps-3.0.0/stadiamaps/models/geo_json_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/geo_json_point_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/geo_json_point_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/geo_json_polygon.py` & `stadiamaps-3.0.0/stadiamaps/models/geo_json_polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/geo_json_polygon_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/geo_json_polygon_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/geocoding_object.py` & `stadiamaps-3.0.0/stadiamaps/models/geocoding_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/height_request.py` & `stadiamaps-3.0.0/stadiamaps/models/height_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/height_response.py` & `stadiamaps-3.0.0/stadiamaps/models/height_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/highway_classification.py` & `stadiamaps-3.0.0/stadiamaps/models/highway_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/intersecting_edge.py` & `stadiamaps-3.0.0/stadiamaps/models/intersecting_edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/isochrone_costing_model.py` & `stadiamaps-3.0.0/stadiamaps/models/isochrone_costing_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/isochrone_feature.py` & `stadiamaps-3.0.0/stadiamaps/models/isochrone_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/isochrone_properties.py` & `stadiamaps-3.0.0/stadiamaps/models/isochrone_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/isochrone_request.py` & `stadiamaps-3.0.0/stadiamaps/models/isochrone_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/isochrone_response.py` & `stadiamaps-3.0.0/stadiamaps/models/isochrone_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/locate_detailed_edge.py` & `stadiamaps-3.0.0/stadiamaps/models/locate_detailed_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/locate_edge.py` & `stadiamaps-3.0.0/stadiamaps/models/locate_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/locate_edge_info.py` & `stadiamaps-3.0.0/stadiamaps/models/locate_edge_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/locate_node.py` & `stadiamaps-3.0.0/stadiamaps/models/locate_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/locate_node_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/locate_node_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/locate_object.py` & `stadiamaps-3.0.0/stadiamaps/models/locate_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/maneuver_sign.py` & `stadiamaps-3.0.0/stadiamaps/models/maneuver_sign.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/maneuver_sign_element.py` & `stadiamaps-3.0.0/stadiamaps/models/maneuver_sign_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/map_match_costing_model.py` & `stadiamaps-3.0.0/stadiamaps/models/map_match_costing_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/map_match_request.py` & `stadiamaps-3.0.0/stadiamaps/models/map_match_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/map_match_request_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/map_match_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/map_match_route_response.py` & `stadiamaps-3.0.0/stadiamaps/models/map_match_route_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/map_match_route_response_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/map_match_route_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/map_match_trace_options.py` & `stadiamaps-3.0.0/stadiamaps/models/map_match_trace_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/map_match_waypoint.py` & `stadiamaps-3.0.0/stadiamaps/models/map_match_waypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/map_match_waypoint_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/map_match_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/matched_point.py` & `stadiamaps-3.0.0/stadiamaps/models/matched_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/matrix_costing_model.py` & `stadiamaps-3.0.0/stadiamaps/models/matrix_costing_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/matrix_distance.py` & `stadiamaps-3.0.0/stadiamaps/models/matrix_distance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt
-from typing import Any, ClassVar, Dict, List, Union
+from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing import Optional, Set
 from typing_extensions import Self
 
 class MatrixDistance(BaseModel):
     """
     MatrixDistance
     """ # noqa: E501
-    distance: Union[StrictFloat, StrictInt] = Field(description="The distance (in `units`) between the location in `sources` at `from_index` and the location in `targets` at `to_index`.")
-    time: StrictInt = Field(description="The travel time (in seconds) between the location in `sources` at `from_index` and the location in `targets` at `to_index`.")
+    distance: Optional[Union[StrictFloat, StrictInt]] = Field(description="The distance (in `units`) between the location in `sources` at `from_index` and the location in `targets` at `to_index`. This value may be 0 in the case that the source and destination are the same, and `null` if no route was found between the locations.")
+    time: Optional[StrictInt] = Field(description="The travel time (in seconds) between the location in `sources` at `from_index` and the location in `targets` at `to_index`. This value may be 0 in the case that the source and destination are the same, and `null` if no route was found between the locations.")
     from_index: StrictInt = Field(description="The index of the start location in the `sources` array.")
     to_index: StrictInt = Field(description="The index of the end location in the `targets` array.")
     additional_properties: Dict[str, Any] = {}
     __properties: ClassVar[List[str]] = ["distance", "time", "from_index", "to_index"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -76,14 +76,24 @@
             exclude_none=True,
         )
         # puts key-value pairs in additional_properties in the top level
         if self.additional_properties is not None:
             for _key, _value in self.additional_properties.items():
                 _dict[_key] = _value
 
+        # set to None if distance (nullable) is None
+        # and model_fields_set contains the field
+        if self.distance is None and "distance" in self.model_fields_set:
+            _dict['distance'] = None
+
+        # set to None if time (nullable) is None
+        # and model_fields_set contains the field
+        if self.time is None and "time" in self.model_fields_set:
+            _dict['time'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of MatrixDistance from a dict"""
         if obj is None:
             return None
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/matrix_request.py` & `stadiamaps-3.0.0/stadiamaps/models/matrix_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,32 +17,32 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
-from stadiamaps.models.coordinate import Coordinate
 from stadiamaps.models.costing_options import CostingOptions
 from stadiamaps.models.distance_unit import DistanceUnit
 from stadiamaps.models.matrix_costing_model import MatrixCostingModel
+from stadiamaps.models.matrix_waypoint import MatrixWaypoint
 from stadiamaps.models.valhalla_languages import ValhallaLanguages
 from typing import Optional, Set
 from typing_extensions import Self
 
 class MatrixRequest(BaseModel):
     """
     MatrixRequest
     """ # noqa: E501
     units: Optional[DistanceUnit] = None
     language: Optional[ValhallaLanguages] = None
     directions_type: Optional[StrictStr] = Field(default='instructions', description="The level of directional narrative to include. Locations and times will always be returned, but narrative generation verbosity can be controlled with this parameter.")
     id: Optional[StrictStr] = Field(default=None, description="An identifier to disambiguate requests (echoed by the server).")
-    sources: Annotated[List[Coordinate], Field(min_length=1)] = Field(description="The list of starting locations")
-    targets: Annotated[List[Coordinate], Field(min_length=1)] = Field(description="The list of ending locations")
+    sources: Annotated[List[MatrixWaypoint], Field(min_length=1)] = Field(description="The list of starting locations")
+    targets: Annotated[List[MatrixWaypoint], Field(min_length=1)] = Field(description="The list of ending locations")
     costing: MatrixCostingModel
     costing_options: Optional[CostingOptions] = None
     matrix_locations: Optional[StrictInt] = Field(default=None, description="Only applicable to one-to-many or many-to-one requests. This defaults to all locations. When specified explicitly, this option allows a partial result to be returned. This is basically equivalent to \"find the closest/best locations out of the full set.\" This can have a dramatic improvement for large requests.")
     additional_properties: Dict[str, Any] = {}
     __properties: ClassVar[List[str]] = ["units", "language", "directions_type", "id", "sources", "targets", "costing", "costing_options", "matrix_locations"]
 
     @field_validator('directions_type')
@@ -130,16 +130,16 @@
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "units": obj.get("units"),
             "language": obj.get("language"),
             "directions_type": obj.get("directions_type") if obj.get("directions_type") is not None else 'instructions',
             "id": obj.get("id"),
-            "sources": [Coordinate.from_dict(_item) for _item in obj["sources"]] if obj.get("sources") is not None else None,
-            "targets": [Coordinate.from_dict(_item) for _item in obj["targets"]] if obj.get("targets") is not None else None,
+            "sources": [MatrixWaypoint.from_dict(_item) for _item in obj["sources"]] if obj.get("sources") is not None else None,
+            "targets": [MatrixWaypoint.from_dict(_item) for _item in obj["targets"]] if obj.get("targets") is not None else None,
             "costing": obj.get("costing"),
             "costing_options": CostingOptions.from_dict(obj["costing_options"]) if obj.get("costing_options") is not None else None,
             "matrix_locations": obj.get("matrix_locations")
         })
         # store additional fields in additional_properties
         for _key in obj.keys():
             if _key not in cls.__properties:
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/matrix_response.py` & `stadiamaps-3.0.0/stadiamaps/models/matrix_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/motor_scooter_costing_options.py` & `stadiamaps-3.0.0/stadiamaps/models/motor_scooter_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/motor_scooter_costing_options_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/motor_scooter_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/motorcycle_costing_options.py` & `stadiamaps-3.0.0/stadiamaps/models/motorcycle_costing_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/motorcycle_costing_options_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/motorcycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/nearest_roads_request.py` & `stadiamaps-3.0.0/stadiamaps/models/nearest_roads_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/node_id.py` & `stadiamaps-3.0.0/stadiamaps/models/node_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/node_type.py` & `stadiamaps-3.0.0/stadiamaps/models/node_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/optimized_route_request.py` & `stadiamaps-3.0.0/stadiamaps/models/optimized_route_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/pedestrian_costing_options.py` & `stadiamaps-3.0.0/stadiamaps/models/pedestrian_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/pelias_geo_json_feature.py` & `stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/pelias_geo_json_properties.py` & `stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/pelias_geo_json_properties_addendum.py` & `stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties_addendum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py` & `stadiamaps-3.0.0/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/pelias_layer.py` & `stadiamaps-3.0.0/stadiamaps/models/pelias_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/pelias_response.py` & `stadiamaps-3.0.0/stadiamaps/models/pelias_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/pelias_response_geocoding.py` & `stadiamaps-3.0.0/stadiamaps/models/pelias_response_geocoding.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/pelias_source.py` & `stadiamaps-3.0.0/stadiamaps/models/pelias_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/restrictions.py` & `stadiamaps-3.0.0/stadiamaps/models/restrictions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/road_class.py` & `stadiamaps-3.0.0/stadiamaps/models/road_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/route_leg.py` & `stadiamaps-3.0.0/stadiamaps/models/route_leg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/route_maneuver.py` & `stadiamaps-3.0.0/stadiamaps/models/route_maneuver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/route_request.py` & `stadiamaps-3.0.0/stadiamaps/models/route_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/route_response.py` & `stadiamaps-3.0.0/stadiamaps/models/route_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/route_response_alternates_inner.py` & `stadiamaps-3.0.0/stadiamaps/models/route_response_alternates_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/route_response_trip.py` & `stadiamaps-3.0.0/stadiamaps/models/route_response_trip.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/route_summary.py` & `stadiamaps-3.0.0/stadiamaps/models/route_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/route_trip.py` & `stadiamaps-3.0.0/stadiamaps/models/route_trip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/routing_response_waypoint.py` & `stadiamaps-3.0.0/stadiamaps/models/routing_response_waypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/routing_response_waypoint_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/routing_response_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/routing_waypoint.py` & `stadiamaps-3.0.0/stadiamaps/models/routing_waypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/routing_waypoint_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/routing_waypoint_all_of_search_filter.py` & `stadiamaps-3.0.0/stadiamaps/models/routing_waypoint_all_of_search_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/simple_routing_waypoint.py` & `stadiamaps-3.0.0/stadiamaps/models/simple_routing_waypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/simple_routing_waypoint_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/simple_routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/speeds.py` & `stadiamaps-3.0.0/stadiamaps/models/speeds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/trace_attribute_filter_options.py` & `stadiamaps-3.0.0/stadiamaps/models/trace_attribute_filter_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/trace_attribute_key.py` & `stadiamaps-3.0.0/stadiamaps/models/trace_attribute_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/trace_attributes_base_response.py` & `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_base_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/trace_attributes_request.py` & `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/trace_attributes_request_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/trace_attributes_request_all_of_filters.py` & `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_request_all_of_filters.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/trace_attributes_response.py` & `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/trace_attributes_response_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/trace_attributes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/trace_edge.py` & `stadiamaps-3.0.0/stadiamaps/models/trace_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/travel_mode.py` & `stadiamaps-3.0.0/stadiamaps/models/travel_mode.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/traversability.py` & `stadiamaps-3.0.0/stadiamaps/models/traversability.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/truck_costing_options.py` & `stadiamaps-3.0.0/stadiamaps/models/truck_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/truck_costing_options_all_of.py` & `stadiamaps-3.0.0/stadiamaps/models/truck_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/stadiamaps/models/tz_response.py` & `stadiamaps-3.0.0/stadiamaps/models/tz_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/valhalla_languages.py` & `stadiamaps-3.0.0/stadiamaps/models/valhalla_languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/valhalla_long_units.py` & `stadiamaps-3.0.0/stadiamaps/models/valhalla_long_units.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/models/warning.py` & `stadiamaps-3.0.0/stadiamaps/models/warning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps/rest.py` & `stadiamaps-3.0.0/stadiamaps/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.
 
-    The version of the OpenAPI document: 6.1.0
+    The version of the OpenAPI document: 6.3.0
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `stadiamaps-2.1.0/stadiamaps.egg-info/PKG-INFO` & `stadiamaps-3.0.0/stadiamaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadiamaps
-Version: 2.1.0
+Version: 3.0.0
 Summary: Stadia Maps Geospatial APIs
 Home-page: https://github.com/stadiamaps/stadiamaps-api-py
 Author: Stadia Maps Support
 Author-email: support@stadiamaps.com
 Keywords: OpenAPI,OpenAPI-Generator,Stadia Maps Geospatial APIs
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `stadiamaps-2.1.0/stadiamaps.egg-info/SOURCES.txt` & `stadiamaps-3.0.0/stadiamaps.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 stadiamaps/models/isochrone_response.py
 stadiamaps/models/locate_detailed_edge.py
 stadiamaps/models/locate_edge.py
 stadiamaps/models/locate_edge_info.py
 stadiamaps/models/locate_node.py
 stadiamaps/models/locate_node_all_of.py
 stadiamaps/models/locate_object.py
+stadiamaps/models/low_speed_vehicle_costing_options.py
 stadiamaps/models/maneuver_sign.py
 stadiamaps/models/maneuver_sign_element.py
 stadiamaps/models/map_match_costing_model.py
 stadiamaps/models/map_match_request.py
 stadiamaps/models/map_match_request_all_of.py
 stadiamaps/models/map_match_route_response.py
 stadiamaps/models/map_match_route_response_all_of.py
@@ -75,14 +76,15 @@
 stadiamaps/models/map_match_waypoint.py
 stadiamaps/models/map_match_waypoint_all_of.py
 stadiamaps/models/matched_point.py
 stadiamaps/models/matrix_costing_model.py
 stadiamaps/models/matrix_distance.py
 stadiamaps/models/matrix_request.py
 stadiamaps/models/matrix_response.py
+stadiamaps/models/matrix_waypoint.py
 stadiamaps/models/motor_scooter_costing_options.py
 stadiamaps/models/motor_scooter_costing_options_all_of.py
 stadiamaps/models/motorcycle_costing_options.py
 stadiamaps/models/motorcycle_costing_options_all_of.py
 stadiamaps/models/nearest_roads_request.py
 stadiamaps/models/node_id.py
 stadiamaps/models/node_type.py
@@ -173,14 +175,15 @@
 test/test_isochrone_response.py
 test/test_locate_detailed_edge.py
 test/test_locate_edge.py
 test/test_locate_edge_info.py
 test/test_locate_node.py
 test/test_locate_node_all_of.py
 test/test_locate_object.py
+test/test_low_speed_vehicle_costing_options.py
 test/test_maneuver_sign.py
 test/test_maneuver_sign_element.py
 test/test_map_match_costing_model.py
 test/test_map_match_request.py
 test/test_map_match_request_all_of.py
 test/test_map_match_route_response.py
 test/test_map_match_route_response_all_of.py
@@ -188,14 +191,15 @@
 test/test_map_match_waypoint.py
 test/test_map_match_waypoint_all_of.py
 test/test_matched_point.py
 test/test_matrix_costing_model.py
 test/test_matrix_distance.py
 test/test_matrix_request.py
 test/test_matrix_response.py
+test/test_matrix_waypoint.py
 test/test_motor_scooter_costing_options.py
 test/test_motor_scooter_costing_options_all_of.py
 test/test_motorcycle_costing_options.py
 test/test_motorcycle_costing_options_all_of.py
 test/test_nearest_roads_request.py
 test/test_node_id.py
 test/test_node_type.py
```

### Comparing `stadiamaps-2.1.0/test/integration/test_eu_endpoint.py` & `stadiamaps-3.0.0/test/integration/test_eu_endpoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/integration/test_gecoding.py` & `stadiamaps-3.0.0/test/integration/test_gecoding.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,22 @@
         with stadiamaps.ApiClient(self.configuration) as api_client:
             api_instance = stadiamaps.GeocodingApi(api_client)
 
             res = api_instance.reverse(59.444351, 24.750645)
             self.assertEqual("Estonia", res.features[0].properties.country)
             self.assertEqual("address", res.features[0].properties.layer)
 
+    def testReverseWithLayerFilter(self):
+        with stadiamaps.ApiClient(self.configuration) as api_client:
+            api_instance = stadiamaps.GeocodingApi(api_client)
+
+            res = api_instance.reverse(59.444351, 24.750645, layers=[stadiamaps.PeliasLayer.ADDRESS, stadiamaps.PeliasLayer.OCEAN])
+            self.assertEqual("Estonia", res.features[0].properties.country)
+            self.assertEqual("address", res.features[0].properties.layer)
+
     def testReverseUncommonLayer(self):
         with stadiamaps.ApiClient(self.configuration) as api_client:
             api_instance = stadiamaps.GeocodingApi(api_client)
 
             # Middle of the Gulf of Oman
             res = api_instance.reverse(24.750645, 59.444351)
             self.assertEqual("marinearea", res.features[0].properties.layer)
```

### Comparing `stadiamaps-2.1.0/test/integration/test_geospatial.py` & `stadiamaps-3.0.0/test/integration/test_geospatial.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/integration/test_routing.py` & `stadiamaps-3.0.0/test/integration/test_routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,16 @@
             req = stadiamaps.RouteRequest(
                 id="route",
                 locations=[
                     stadiamaps.RoutingWaypoint.from_dict(location_a),
                     stadiamaps.RoutingWaypoint.from_dict(location_b)
                 ],
                 costing=stadiamaps.CostingModel.BICYCLE,
-                costing_options=stadiamaps.CostingOptions(bicycle=stadiamaps.BicycleCostingOptions(bicycle_type='Hybrid', use_roads=0.4, use_hills=0.6)),
+                costing_options=stadiamaps.CostingOptions(
+                    bicycle=stadiamaps.BicycleCostingOptions(bicycle_type='Hybrid', use_roads=0.4, use_hills=0.6)),
                 units=stadiamaps.DistanceUnit.KM,
             )
 
             res = api_instance.route(req)
             self.assertEqual(req.id, res.id)
             self.assertEqual(0, res.trip.status)
             self.assertEqual("kilometers", res.trip.units)
@@ -109,48 +110,84 @@
     def testTimeDistanceMatrix(self):
         with stadiamaps.ApiClient(self.configuration) as api_client:
             api_instance = stadiamaps.RoutingApi(api_client)
 
             req = stadiamaps.MatrixRequest(
                 id="matrix",
                 sources=[
-                    stadiamaps.Coordinate.from_dict(location_a),
+                    stadiamaps.MatrixWaypoint.from_dict(location_a),
                 ],
                 targets=[
-                    stadiamaps.Coordinate.from_dict(location_b),
-                    stadiamaps.Coordinate.from_dict(location_c),
+                    stadiamaps.MatrixWaypoint.from_dict(location_b),
+                    stadiamaps.MatrixWaypoint.from_dict(location_c),
                 ],
                 costing=stadiamaps.MatrixCostingModel.PEDESTRIAN,
             )
 
             res = api_instance.time_distance_matrix(req)
             self.assertEqual(req.id, res.id)
             self.assertEqual(len(req.sources), len(res.sources))
             self.assertEqual(len(req.targets), len(res.targets))
             self.assertGreater(len(res.sources_to_targets[0]), 1)
             self.assertEqual("kilometers", res.units)
 
+    def testTimeDistanceMatrixWithUnroutableLegs(self):
+        with stadiamaps.ApiClient(self.configuration) as api_client:
+            api_instance = stadiamaps.RoutingApi(api_client)
+
+            # At least one of these is not routable; make sure we handle it gracefully
+            req = stadiamaps.MatrixRequest(
+                id="matrix",
+                sources=[
+                    stadiamaps.MatrixWaypoint.from_dict({
+                        "lon": 22.726262,
+                        "lat": 58.891957
+                    }),
+                    stadiamaps.MatrixWaypoint.from_dict({
+                        "lon": 23.762758,
+                        "lat": 59.1558
+                    }),
+                ],
+                targets=[
+                    stadiamaps.MatrixWaypoint.from_dict({
+                        "lon": 23.846605,
+                        "lat": 59.176153
+                    }),
+                    stadiamaps.MatrixWaypoint.from_dict({
+                        "lon": 23.096114,
+                        "lat": 59.562853
+                    }),
+                ],
+                costing=stadiamaps.MatrixCostingModel.BICYCLE,
+            )
+
+            res = api_instance.time_distance_matrix(req)
+            self.assertEqual(req.id, res.id)
+            self.assertEqual(len(req.sources), len(res.sources))
+            self.assertGreater(len(res.sources_to_targets[0]), 1)
+            self.assertEqual("kilometers", res.units)
+
     def testNearestRoads(self):
         with stadiamaps.ApiClient(self.configuration) as api_client:
             api_instance = stadiamaps.RoutingApi(api_client)
 
             req = stadiamaps.NearestRoadsRequest(
-                locations=[location_a, location_b, location_c]
+                locations=[stadiamaps.Coordinate.from_dict(loc) for loc in (location_a, location_b, location_c)]
             )
             res = api_instance.nearest_roads(req)
             self.assertEqual(len(res), 3)
             self.assertGreaterEqual(len(res[0].edges), 1)
 
     def testIsochrone(self):
         with stadiamaps.ApiClient(self.configuration) as api_client:
             api_instance = stadiamaps.RoutingApi(api_client)
 
             req = stadiamaps.IsochroneRequest(
                 id="isochrone",
-                locations=[location_a],
+                locations=[stadiamaps.Coordinate.from_dict(location_a)],
                 costing=stadiamaps.IsochroneCostingModel.PEDESTRIAN,
                 contours=[
                     stadiamaps.Contour(time=5, color="aabbcc")
                 ],
                 polygons=True,
             )
             res = api_instance.isochrone(req)
```

### Comparing `stadiamaps-2.1.0/test/test_access.py` & `stadiamaps-3.0.0/test/test_access.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_admin_region.py` & `stadiamaps-3.0.0/test/test_admin_region.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_administrative.py` & `stadiamaps-3.0.0/test/test_administrative.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_auto_costing_options.py` & `stadiamaps-3.0.0/test/test_auto_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_auto_costing_options_all_of.py` & `stadiamaps-3.0.0/test/test_auto_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_base_costing_options.py` & `stadiamaps-3.0.0/test/test_base_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_base_trace_request.py` & `stadiamaps-3.0.0/test/test_base_trace_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_bicycle_costing_options.py` & `stadiamaps-3.0.0/test/test_bicycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_bicycle_costing_options_all_of.py` & `stadiamaps-3.0.0/test/test_bicycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_bike_network.py` & `stadiamaps-3.0.0/test/test_bike_network.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_contour.py` & `stadiamaps-3.0.0/test/test_contour.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_coordinate.py` & `stadiamaps-3.0.0/test/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_costing_model.py` & `stadiamaps-3.0.0/test/test_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_costing_options.py` & `stadiamaps-3.0.0/test/test_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_directions_options.py` & `stadiamaps-3.0.0/test/test_directions_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_distance_unit.py` & `stadiamaps-3.0.0/test/test_distance_unit.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_edge_sign.py` & `stadiamaps-3.0.0/test/test_edge_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_edge_use.py` & `stadiamaps-3.0.0/test/test_edge_use.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_end_node.py` & `stadiamaps-3.0.0/test/test_end_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geo_attributes.py` & `stadiamaps-3.0.0/test/test_geo_attributes.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geo_json_geometry.py` & `stadiamaps-3.0.0/test/test_geo_json_geometry.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geo_json_geometry_base.py` & `stadiamaps-3.0.0/test/test_geo_json_geometry_base.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geo_json_line_string.py` & `stadiamaps-3.0.0/test/test_geo_json_line_string.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geo_json_line_string_all_of.py` & `stadiamaps-3.0.0/test/test_geo_json_line_string_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geo_json_point.py` & `stadiamaps-3.0.0/test/test_geo_json_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geo_json_point_all_of.py` & `stadiamaps-3.0.0/test/test_geo_json_point_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geo_json_polygon.py` & `stadiamaps-3.0.0/test/test_geo_json_polygon.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geo_json_polygon_all_of.py` & `stadiamaps-3.0.0/test/test_geo_json_polygon_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geocoding_api.py` & `stadiamaps-3.0.0/test/test_geocoding_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geocoding_object.py` & `stadiamaps-3.0.0/test/test_geocoding_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_geospatial_api.py` & `stadiamaps-3.0.0/test/test_geospatial_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_height_request.py` & `stadiamaps-3.0.0/test/test_height_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_height_response.py` & `stadiamaps-3.0.0/test/test_height_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_highway_classification.py` & `stadiamaps-3.0.0/test/test_highway_classification.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_intersecting_edge.py` & `stadiamaps-3.0.0/test/test_intersecting_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_isochrone_costing_model.py` & `stadiamaps-3.0.0/test/test_isochrone_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_isochrone_feature.py` & `stadiamaps-3.0.0/test/test_isochrone_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_isochrone_properties.py` & `stadiamaps-3.0.0/test/test_isochrone_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_isochrone_request.py` & `stadiamaps-3.0.0/test/test_isochrone_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_isochrone_response.py` & `stadiamaps-3.0.0/test/test_isochrone_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_locate_detailed_edge.py` & `stadiamaps-3.0.0/test/test_locate_detailed_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_locate_edge.py` & `stadiamaps-3.0.0/test/test_locate_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_locate_edge_info.py` & `stadiamaps-3.0.0/test/test_locate_edge_info.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_locate_node.py` & `stadiamaps-3.0.0/test/test_locate_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_locate_node_all_of.py` & `stadiamaps-3.0.0/test/test_locate_node_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_locate_object.py` & `stadiamaps-3.0.0/test/test_locate_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_maneuver_sign.py` & `stadiamaps-3.0.0/test/test_maneuver_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_maneuver_sign_element.py` & `stadiamaps-3.0.0/test/test_maneuver_sign_element.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_map_match_costing_model.py` & `stadiamaps-3.0.0/test/test_map_match_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_map_match_request.py` & `stadiamaps-3.0.0/test/test_map_match_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_map_match_request_all_of.py` & `stadiamaps-3.0.0/test/test_map_match_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_map_match_route_response.py` & `stadiamaps-3.0.0/test/test_map_match_route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_map_match_route_response_all_of.py` & `stadiamaps-3.0.0/test/test_map_match_route_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_map_match_trace_options.py` & `stadiamaps-3.0.0/test/test_map_match_trace_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_map_match_waypoint.py` & `stadiamaps-3.0.0/test/test_map_match_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_map_match_waypoint_all_of.py` & `stadiamaps-3.0.0/test/test_map_match_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_matched_point.py` & `stadiamaps-3.0.0/test/test_matched_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_matrix_costing_model.py` & `stadiamaps-3.0.0/test/test_matrix_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_matrix_distance.py` & `stadiamaps-3.0.0/test/test_matrix_distance.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_matrix_request.py` & `stadiamaps-3.0.0/test/test_matrix_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_matrix_response.py` & `stadiamaps-3.0.0/test/test_matrix_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_motor_scooter_costing_options.py` & `stadiamaps-3.0.0/test/test_motor_scooter_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_motor_scooter_costing_options_all_of.py` & `stadiamaps-3.0.0/test/test_motor_scooter_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_motorcycle_costing_options.py` & `stadiamaps-3.0.0/test/test_motorcycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_motorcycle_costing_options_all_of.py` & `stadiamaps-3.0.0/test/test_motorcycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_nearest_roads_request.py` & `stadiamaps-3.0.0/test/test_nearest_roads_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_node_id.py` & `stadiamaps-3.0.0/test/test_node_id.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_node_type.py` & `stadiamaps-3.0.0/test/test_node_type.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_optimized_route_request.py` & `stadiamaps-3.0.0/test/test_optimized_route_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_pedestrian_costing_options.py` & `stadiamaps-3.0.0/test/test_pedestrian_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_pelias_geo_json_feature.py` & `stadiamaps-3.0.0/test/test_pelias_geo_json_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_pelias_geo_json_properties.py` & `stadiamaps-3.0.0/test/test_pelias_geo_json_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_pelias_geo_json_properties_addendum.py` & `stadiamaps-3.0.0/test/test_pelias_geo_json_properties_addendum.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_pelias_geo_json_properties_addendum_osm.py` & `stadiamaps-3.0.0/test/test_pelias_geo_json_properties_addendum_osm.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_pelias_layer.py` & `stadiamaps-3.0.0/test/test_pelias_layer.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_pelias_response.py` & `stadiamaps-3.0.0/test/test_pelias_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_pelias_response_geocoding.py` & `stadiamaps-3.0.0/test/test_pelias_response_geocoding.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_pelias_source.py` & `stadiamaps-3.0.0/test/test_pelias_source.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_restrictions.py` & `stadiamaps-3.0.0/test/test_restrictions.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_road_class.py` & `stadiamaps-3.0.0/test/test_road_class.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_route_leg.py` & `stadiamaps-3.0.0/test/test_route_leg.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_route_maneuver.py` & `stadiamaps-3.0.0/test/test_route_maneuver.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_route_request.py` & `stadiamaps-3.0.0/test/test_route_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_route_response.py` & `stadiamaps-3.0.0/test/test_route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_route_response_alternates_inner.py` & `stadiamaps-3.0.0/test/test_route_response_alternates_inner.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_route_response_trip.py` & `stadiamaps-3.0.0/test/test_route_response_trip.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_route_summary.py` & `stadiamaps-3.0.0/test/test_route_summary.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_route_trip.py` & `stadiamaps-3.0.0/test/test_route_trip.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_routing_api.py` & `stadiamaps-3.0.0/test/test_routing_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_routing_response_waypoint.py` & `stadiamaps-3.0.0/test/test_routing_response_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_routing_response_waypoint_all_of.py` & `stadiamaps-3.0.0/test/test_routing_response_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_routing_waypoint.py` & `stadiamaps-3.0.0/test/test_routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_routing_waypoint_all_of.py` & `stadiamaps-3.0.0/test/test_routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_routing_waypoint_all_of_search_filter.py` & `stadiamaps-3.0.0/test/test_routing_waypoint_all_of_search_filter.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_simple_routing_waypoint.py` & `stadiamaps-3.0.0/test/test_simple_routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_simple_routing_waypoint_all_of.py` & `stadiamaps-3.0.0/test/test_simple_routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_speeds.py` & `stadiamaps-3.0.0/test/test_speeds.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_trace_attribute_filter_options.py` & `stadiamaps-3.0.0/test/test_trace_attribute_filter_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_trace_attribute_key.py` & `stadiamaps-3.0.0/test/test_trace_attribute_key.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_trace_attributes_base_response.py` & `stadiamaps-3.0.0/test/test_trace_attributes_base_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_trace_attributes_request.py` & `stadiamaps-3.0.0/test/test_trace_attributes_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_trace_attributes_request_all_of.py` & `stadiamaps-3.0.0/test/test_trace_attributes_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_trace_attributes_request_all_of_filters.py` & `stadiamaps-3.0.0/test/test_trace_attributes_request_all_of_filters.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_trace_attributes_response.py` & `stadiamaps-3.0.0/test/test_trace_attributes_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_trace_attributes_response_all_of.py` & `stadiamaps-3.0.0/test/test_trace_attributes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_trace_edge.py` & `stadiamaps-3.0.0/test/test_trace_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_travel_mode.py` & `stadiamaps-3.0.0/test/test_travel_mode.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_traversability.py` & `stadiamaps-3.0.0/test/test_traversability.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_truck_costing_options.py` & `stadiamaps-3.0.0/test/test_truck_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_truck_costing_options_all_of.py` & `stadiamaps-3.0.0/test/test_truck_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_tz_response.py` & `stadiamaps-3.0.0/test/test_tz_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_valhalla_languages.py` & `stadiamaps-3.0.0/test/test_valhalla_languages.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_valhalla_long_units.py` & `stadiamaps-3.0.0/test/test_valhalla_long_units.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-2.1.0/test/test_warning.py` & `stadiamaps-3.0.0/test/test_warning.py`

 * *Files identical despite different names*

