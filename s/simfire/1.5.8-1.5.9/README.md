# Comparing `tmp/simfire-1.5.8.tar.gz` & `tmp/simfire-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfire-1.5.8.tar", max compression
+gzip compressed data, was "simfire-1.5.9.tar", max compression
```

## Comparing `simfire-1.5.8.tar` & `simfire-1.5.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    10789 2024-02-26 20:17:50.740182 simfire-1.5.8/LICENSE
--rw-r--r--   0        0        0     2865 2024-02-26 20:17:50.740182 simfire-1.5.8/README.md
--rw-r--r--   0        0        0     1994 2024-02-26 20:17:50.912181 simfire-1.5.8/pyproject.toml
--rw-r--r--   0        0        0     1111 2024-02-26 20:17:50.912181 simfire-1.5.8/simfire/__init__.py
--rw-r--r--   0        0        0    10729 2024-02-26 20:17:50.912181 simfire-1.5.8/simfire/enums.py
--rw-r--r--   0        0        0       37 2024-02-26 20:17:50.912181 simfire-1.5.8/simfire/game/__init__.py
--rw-r--r--   0        0        0      874 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/_tests/__init__.py
--rw-r--r--   0        0        0    15395 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/_tests/test_game.py
--rw-r--r--   0        0        0     9969 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/_tests/test_sprites.py
--rw-r--r--   0        0        0    15227 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/game.py
--rw-r--r--   0        0        0     1318 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/image.py
--rw-r--r--   0        0        0      379 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/managers/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/managers/_tests/__init__.py
--rw-r--r--   0        0        0    18246 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/managers/_tests/test_fire.py
--rw-r--r--   0        0        0     8141 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/managers/_tests/test_mitigation.py
--rw-r--r--   0        0        0    30951 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/managers/fire.py
--rw-r--r--   0        0        0     7321 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/managers/mitigation.py
--rw-r--r--   0        0        0    15863 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/game/sprites.py
--rw-r--r--   0        0        0       49 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/sim/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/sim/_tests/__init__.py
--rw-r--r--   0        0        0    16480 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/sim/_tests/test_simulation.py
--rw-r--r--   0        0        0    39016 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/sim/simulation.py
--rw-r--r--   0        0        0        0 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/__init__.py
--rw-r--r--   0        0        0     2771 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/test_config.py
--rw-r--r--   0        0        0     1802 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/test_configs/test_config.yml
--rw-r--r--   0        0        0       47 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/test_configs/test_config_bad.yml
--rw-r--r--   0        0        0     1750 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/test_configs/test_config_flat_simple.yml
--rw-r--r--   0        0        0     1751 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/test_configs/test_config_gaussian.yml
--rw-r--r--   0        0        0     1728 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml
--rw-r--r--   0        0        0     4693 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/test_graph.py
--rw-r--r--   0        0        0     8521 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/test_layers.py
--rw-r--r--   0        0        0      622 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/test_log.py
--rw-r--r--   0        0        0     4495 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/test_terrain.py
--rw-r--r--   0        0        0     1472 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/_tests/test_units.py
--rw-r--r--   0        0        0        0 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/assets/__init__.py
--rw-r--r--   0        0        0     1854 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/assets/fireline_logo.png
--rw-r--r--   0        0        0    41213 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/config.py
--rw-r--r--   0        0        0      499 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/decorators.py
--rw-r--r--   0        0        0     4142 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/generate_cfd_wind_layer.py
--rw-r--r--   0        0        0    10189 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/graph.py
--rw-r--r--   0        0        0    23531 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/layers.py
--rw-r--r--   0        0        0     2030 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/log.py
--rw-r--r--   0        0        0   143776 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy
--rw-r--r--   0        0        0   143776 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy
--rw-r--r--   0        0        0     3647 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/terrain.py
--rw-r--r--   0        0        0        0 2024-02-26 20:17:50.916181 simfire-1.5.8/simfire/utils/textures/__init__.py
--rw-r--r--   0        0        0   204702 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/utils/textures/terrain.jpg
--rw-r--r--   0        0        0     2555 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/utils/units.py
--rw-r--r--   0        0        0        0 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/_tests/__init__.py
--rw-r--r--   0        0        0     2180 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/_tests/test_cfd_wind.py
--rw-r--r--   0        0        0     2423 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/_tests/test_elevation_functions.py
--rw-r--r--   0        0        0     2821 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/_tests/test_rothermel.py
--rw-r--r--   0        0        0     1477 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/_tests/test_wind.py
--rw-r--r--   0        0        0     3703 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/elevation_functions.py
--rw-r--r--   0        0        0     1054 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/fuel_array_functions.py
--rw-r--r--   0        0        0     2306 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/parameters.py
--rw-r--r--   0        0        0     2083 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/presets.py
--rw-r--r--   0        0        0     5313 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/rothermel.py
--rw-r--r--   0        0        0        0 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/wind_mechanics/__init__.py
--rw-r--r--   0        0        0     9087 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/wind_mechanics/cfd_wind.py
--rw-r--r--   0        0        0     3155 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/wind_mechanics/perlin_wind.py
--rw-r--r--   0        0        0     6625 2024-02-26 20:17:50.920181 simfire-1.5.8/simfire/world/wind_mechanics/wind_controller.py
--rw-r--r--   0        0        0     4124 1970-01-01 00:00:00.000000 simfire-1.5.8/PKG-INFO
+-rw-r--r--   0        0        0    10789 2024-04-29 23:38:52.318686 simfire-1.5.9/LICENSE
+-rw-r--r--   0        0        0     2865 2024-04-29 23:38:52.318686 simfire-1.5.9/README.md
+-rw-r--r--   0        0        0     2008 2024-04-29 23:38:52.490688 simfire-1.5.9/pyproject.toml
+-rw-r--r--   0        0        0     1111 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/__init__.py
+-rw-r--r--   0        0        0    10730 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/enums.py
+-rw-r--r--   0        0        0       37 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/_tests/__init__.py
+-rw-r--r--   0        0        0    15395 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/_tests/test_game.py
+-rw-r--r--   0        0        0     9969 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/_tests/test_sprites.py
+-rw-r--r--   0        0        0    15227 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/game.py
+-rw-r--r--   0        0        0     1318 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/image.py
+-rw-r--r--   0        0        0      379 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/managers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/managers/_tests/__init__.py
+-rw-r--r--   0        0        0    18246 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/managers/_tests/test_fire.py
+-rw-r--r--   0        0        0     8141 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/managers/_tests/test_mitigation.py
+-rw-r--r--   0        0        0    30954 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/managers/fire.py
+-rw-r--r--   0        0        0     7321 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/managers/mitigation.py
+-rw-r--r--   0        0        0    15863 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/game/sprites.py
+-rw-r--r--   0        0        0       49 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/sim/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/sim/_tests/__init__.py
+-rw-r--r--   0        0        0    16480 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/sim/_tests/test_simulation.py
+-rw-r--r--   0        0        0    39016 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/sim/simulation.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/__init__.py
+-rw-r--r--   0        0        0     2771 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/test_config.py
+-rw-r--r--   0        0        0     1802 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/test_configs/test_config.yml
+-rw-r--r--   0        0        0       47 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/test_configs/test_config_bad.yml
+-rw-r--r--   0        0        0     1750 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/test_configs/test_config_flat_simple.yml
+-rw-r--r--   0        0        0     1751 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/test_configs/test_config_gaussian.yml
+-rw-r--r--   0        0        0     1728 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml
+-rw-r--r--   0        0        0     4693 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/test_graph.py
+-rw-r--r--   0        0        0     8521 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/test_layers.py
+-rw-r--r--   0        0        0      622 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/test_log.py
+-rw-r--r--   0        0        0     4495 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/test_terrain.py
+-rw-r--r--   0        0        0     1472 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/_tests/test_units.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/assets/__init__.py
+-rw-r--r--   0        0        0     1854 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/assets/fireline_logo.png
+-rw-r--r--   0        0        0    41281 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/config.py
+-rw-r--r--   0        0        0      499 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/decorators.py
+-rw-r--r--   0        0        0     4143 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/generate_cfd_wind_layer.py
+-rw-r--r--   0        0        0    10189 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/graph.py
+-rw-r--r--   0        0        0    24576 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/layers.py
+-rw-r--r--   0        0        0     2030 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/log.py
+-rw-r--r--   0        0        0   143776 2024-04-29 23:38:52.494688 simfire-1.5.9/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy
+-rw-r--r--   0        0        0   143776 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy
+-rw-r--r--   0        0        0     3647 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/utils/terrain.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/utils/textures/__init__.py
+-rw-r--r--   0        0        0   204702 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/utils/textures/terrain.jpg
+-rw-r--r--   0        0        0     2555 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/utils/units.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/_tests/__init__.py
+-rw-r--r--   0        0        0     2180 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/_tests/test_cfd_wind.py
+-rw-r--r--   0        0        0     2423 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/_tests/test_elevation_functions.py
+-rw-r--r--   0        0        0     2821 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/_tests/test_rothermel.py
+-rw-r--r--   0        0        0     1477 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/_tests/test_wind.py
+-rw-r--r--   0        0        0     3703 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/elevation_functions.py
+-rw-r--r--   0        0        0     1054 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/fuel_array_functions.py
+-rw-r--r--   0        0        0     2306 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/parameters.py
+-rw-r--r--   0        0        0     2084 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/presets.py
+-rw-r--r--   0        0        0     5313 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/rothermel.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/wind_mechanics/__init__.py
+-rw-r--r--   0        0        0     9087 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/wind_mechanics/cfd_wind.py
+-rw-r--r--   0        0        0     3155 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/wind_mechanics/perlin_wind.py
+-rw-r--r--   0        0        0     6625 2024-04-29 23:38:52.498688 simfire-1.5.9/simfire/world/wind_mechanics/wind_controller.py
+-rw-r--r--   0        0        0     4124 1970-01-01 00:00:00.000000 simfire-1.5.9/PKG-INFO
```

### Comparing `simfire-1.5.8/LICENSE` & `simfire-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/README.md` & `simfire-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/pyproject.toml` & `simfire-1.5.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simfire"
-version = "1.5.8"
+version = "1.5.9"
 description = "Fire simulator built in Python"
 authors = ["Tim Welsh <twelsh@mitre.org>", "Marissa Dotter <mdotter@mitre.org>",
            "Michael Doyle <mdoyle@mitre.org>", "Dhanuj Gandikota <dgandikota@mitre.org>",
            "Chris Kempis <ckempis@mitre.org>", "Lauren Schambach <lschambach@mitre.org>",
            "Alex Tapley <atapley@mitre.org>", "Michael Threet <mthreet@mitre.org>"]
 readme = "README.md"
 include = ["simfire/utils/textures/terrain.jpg", "simfire/utils/assets/fireline_logo.png"]
@@ -14,15 +14,15 @@
 repository = "https://github.com/mitrefireline/simfire"
 
 [tool.poetry.dependencies]
 python = "~3.9"
 matplotlib = "^3.5.2"
 noise = "^1.2.2"
 numpy = "^1.22.4"
-Pillow = "^9.1.1"
+Pillow = ">=9.1.1,<11.0.0"
 pygame = "^2.1.2"
 PyYAML = "^6.0"
 reportlab = "^3.6.10"
 scikit-image = "^0.19.3"
 svglib = "^1.3.0"
 rich = "^12.5.1"
 wurlitzer = "^3.0.2"
@@ -42,15 +42,15 @@
 sphinx-rtd-theme = "^1.0.0"
 myst-parser = "^0.18.0"
 furo = "^2022.6.4.1"
 sphinxext-opengraph = "^0.9.0"
 sphinx-copybutton = "^0.5.2"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
+black = ">=22.3,<25.0"
 certifi = "^2022.6.15"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
 pre-commit = "^2.19.0"
 pytest = "^7.1.2"
 bandit = "^1.7.4"
 types-setuptools = "^65.3.0"
```

### Comparing `simfire-1.5.8/simfire/__init__.py` & `simfire-1.5.9/simfire/__init__.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/enums.py` & `simfire-1.5.9/simfire/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Enums
 =====
 
 Contains many enumeration classes for use throughout `rothermel_model` that depict pixel
 burn status, the ordering of sprite layers, how much to attenuate the rate of spread on
 different types of control lines, and the current game status.
 """
+
 from dataclasses import dataclass
 from enum import Enum, IntEnum, auto
 from pathlib import Path
 from typing import Tuple
 
 import numpy as np
 import pkg_resources
```

### Comparing `simfire-1.5.8/simfire/game/_tests/__init__.py` & `simfire-1.5.9/simfire/game/_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/game/_tests/test_game.py` & `simfire-1.5.9/simfire/game/_tests/test_game.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/game/_tests/test_sprites.py` & `simfire-1.5.9/simfire/game/_tests/test_sprites.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/game/game.py` & `simfire-1.5.9/simfire/game/game.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/game/image.py` & `simfire-1.5.9/simfire/game/image.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/game/managers/_tests/test_fire.py` & `simfire-1.5.9/simfire/game/managers/_tests/test_fire.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/game/managers/_tests/test_mitigation.py` & `simfire-1.5.9/simfire/game/managers/_tests/test_mitigation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/game/managers/fire.py` & `simfire-1.5.9/simfire/game/managers/fire.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Fire
 ====
 
 Defines the different `FireManager`s (`ConstantSpreadFireManager` and
 `RothermelFireManager`) that determine how a fire moves about a `fire_map`.
 """
+
 import collections
 from dataclasses import astuple
 from typing import Any, List, Optional, Sequence, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pygame
@@ -266,17 +267,17 @@
                 "FireManager._update_rate_of_spread"
             )
             raise AssertionError
 
         factor = np.zeros_like(rate_of_spread)
         if self.attenuate_line_ros:
             factor[np.where(fire_map == BurnStatus.FIRELINE)] = RoSAttenuation.FIRELINE
-            factor[
-                np.where(fire_map == BurnStatus.SCRATCHLINE)
-            ] = RoSAttenuation.SCRATCHLINE
+            factor[np.where(fire_map == BurnStatus.SCRATCHLINE)] = (
+                RoSAttenuation.SCRATCHLINE
+            )
             factor[np.where(fire_map == BurnStatus.WETLINE)] = RoSAttenuation.WETLINE
             rate_of_spread = rate_of_spread - factor
         else:
             rate_of_spread[np.where(fire_map == BurnStatus.FIRELINE)] = 0
             rate_of_spread[np.where(fire_map == BurnStatus.SCRATCHLINE)] = 0
             rate_of_spread[np.where(fire_map == BurnStatus.WETLINE)] = 0
```

### Comparing `simfire-1.5.8/simfire/game/managers/mitigation.py` & `simfire-1.5.9/simfire/game/managers/mitigation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/game/sprites.py` & `simfire-1.5.9/simfire/game/sprites.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/sim/_tests/test_simulation.py` & `simfire-1.5.9/simfire/sim/_tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/sim/simulation.py` & `simfire-1.5.9/simfire/sim/simulation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/_tests/test_config.py` & `simfire-1.5.9/simfire/utils/_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/_tests/test_configs/test_config.yml` & `simfire-1.5.9/simfire/utils/_tests/test_configs/test_config.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/_tests/test_configs/test_config_flat_simple.yml` & `simfire-1.5.9/simfire/utils/_tests/test_configs/test_config_flat_simple.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/_tests/test_configs/test_config_gaussian.yml` & `simfire-1.5.9/simfire/utils/_tests/test_configs/test_config_gaussian.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml` & `simfire-1.5.9/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/_tests/test_graph.py` & `simfire-1.5.9/simfire/utils/_tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/_tests/test_layers.py` & `simfire-1.5.9/simfire/utils/_tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/_tests/test_log.py` & `simfire-1.5.9/simfire/utils/_tests/test_log.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/_tests/test_terrain.py` & `simfire-1.5.9/simfire/utils/_tests/test_terrain.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/_tests/test_units.py` & `simfire-1.5.9/simfire/utils/_tests/test_units.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/assets/fireline_logo.png` & `simfire-1.5.9/simfire/utils/assets/fireline_logo.png`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/config.py` & `simfire-1.5.9/simfire/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module containing all config parsing and dataclass logic.
 """
+
 import dataclasses
 import os
 import random
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, Optional, Tuple, Union
 
@@ -270,17 +271,17 @@
         if (
             self.yaml_data["terrain"]["topography"]["type"] == "operational"
             or self.yaml_data["terrain"]["fuel"]["type"] == "operational"
         ):
             year = self.yaml_data["operational"]["year"]
             self._set_all_combos()
             if self.yaml_data["operational"]["seed"] is not None:
-                points: Tuple[
-                    Tuple[float, float], Tuple[float, float]
-                ] = self._randomly_select_box(self.yaml_data["operational"]["seed"])
+                points: Tuple[Tuple[float, float], Tuple[float, float]] = (
+                    self._randomly_select_box(self.yaml_data["operational"]["seed"])
+                )
                 valid = self._check_lat_long(points)
                 if not valid:
                     if self.landfire_lat_long_box is None:
                         message = (
                             "Lat/Long box is not valid and was not created successfully."
                         )
                         log.error(message)
@@ -311,15 +312,18 @@
                         f"({(tl_lat, tl_lon), (br_lat, br_long) }), "
                         f"and the year {year}."
                     )
                     log.error(message)
                     raise ConfigError(message)
                 else:
                     landfire_lat_long_box = LandFireLatLongBox(
-                        points=((tl_lat, tl_lon), (br_lat, br_long)), year=year
+                        points=((tl_lat, tl_lon), (br_lat, br_long)),
+                        year=year,
+                        height=height,
+                        width=width,
                     )
             return landfire_lat_long_box
         else:
             return None
 
     def _check_lat_long(
         self, points: Tuple[Tuple[float, float], Tuple[float, float]]
@@ -425,16 +429,16 @@
             The YAML data converted to an AreaConfig dataclass
         """
 
         # No processing needed for the AreaConfig
         if self.landfire_lat_long_box is not None:
             # Overwite the screen_size since operational data will determine
             self.yaml_data["area"]["screen_size"] = (
-                self.landfire_lat_long_box.geotiff_data[:, :, -1].shape[0],
-                self.landfire_lat_long_box.geotiff_data[:, :, -1].shape[1],
+                self.landfire_lat_long_box.fuel.shape[0],
+                self.landfire_lat_long_box.fuel.shape[1],
             )
             self.yaml_data["area"]["pixel_scale"] = int(
                 self.yaml_data["operational"]["resolution"] / 0.3048
             )
             # "Clear" the geotiff_data to enable making deepcopy of Config object
             self.landfire_lat_long_box.geotiff_data = None
         return AreaConfig(**self.yaml_data["area"])
```

### Comparing `simfire-1.5.8/simfire/utils/generate_cfd_wind_layer.py` & `simfire-1.5.9/simfire/utils/generate_cfd_wind_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Generate CFD Wind Layer
 =======================
 Seperate file to precompute wind layer, currently using wind with a single time slice
 due to processing limitations.
 """
+
 import time
 from pathlib import Path
 
 import numpy as np
 import pygame
 
 from simfire.utils.config import Config
```

### Comparing `simfire-1.5.8/simfire/utils/graph.py` & `simfire-1.5.9/simfire/utils/graph.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/layers.py` & `simfire-1.5.9/simfire/utils/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         self,
         points: Tuple[Tuple[float, float], Tuple[float, float]] = (
             (37.45, -120.44),
             (37.35, -120.22),
         ),
         year: str = "2020",
         layers: Tuple[str, str] = ("fuel", "topographic"),
+        height: int = 4500,
+        width: int = 4500,
     ) -> None:
         """
         This class of methods will get initialized with the config using the lat/long
         bounding box.
 
         Real-world is measured in meters
         Data is measured in pixels corresponding to the resolution
@@ -56,18 +58,28 @@
 
         """
 
         self.points = points
         self.year = year
         self.layers = layers
 
+        # FIX FOR CRS CHANGES
+        # pad the original BR points by a marginal amount of area --> 90 meters each side
+        # to ensure that the output shape matches the specified/desired output shape
+
+        # Padding only one corner allows us to use the TL as a starting point to
+        # crop from
+
+        self.pad_distance = 0.00027777777803598015 * 100
+
         # sepcify the output paths of the Landfire python-client query
         self.product_layers_path = Path(
             f"lf_{abs(self.points[0][1])}_{self.points[0][0]}_"
-            f"{abs(self.points[1][1])}_{self.points[1][0]}.zip"
+            f"{abs(self.points[1][1]+self.pad_distance)}_"
+            f"{self.points[1][0]-self.pad_distance}.zip"
         )
 
         if os.environ.get("SF_HOME") is None:
             sf_path = Path().home() / ".simfire"
         else:
             sf_path = Path(str(os.environ.get("SF_HOME")))
             if not sf_path.exists():
@@ -76,27 +88,39 @@
 
         self.output_path = (
             sf_path / f"landfire/{self.year}/{self.product_layers_path.stem}/"
         )
 
         log.info(f"Saving LandFire data to: {self.output_path}")
 
-        # make each a layer a global varibale that we "fill"
+        # make each a layer a global variable that we "fill"
         self.fuel = np.array([])
         self.topography = np.array([])
 
         # check if we've already pulled this data before
         exists = self._check_paths()
         if exists:
             self._make_data()
         else:
             self.layer_products = self._get_layer_names()
             self.query_lat_lon_layer_data()
             self._make_data()
 
+        # FIX FOR CRS CHANGES
+        # crop data to new pixel_height and pixel_width
+        pixel_height = int(np.floor(height / 30))  # round down to nearest int
+        pixel_width = int(np.floor(width / 30))  # round down to nearest int
+        self.fuel = self.fuel[:pixel_height, :pixel_width]
+        self.topography = self.topography[:pixel_height, :pixel_width]
+
+        print(
+            f"Output shape of Fire Map: {height}m x {width}m "
+            f"--> {self.fuel.shape} in pixel space"
+        )
+
     def _check_paths(self):
         """
         Check to verify if this exact data has already been pulled.
             This is unlikely, but could save time if so.
 
         Assume we always pull at least Fuel and Topography data.
 
@@ -189,15 +213,16 @@
 
         """
         if not self.output_path.exists():
             self.output_path.mkdir(parents=True, exist_ok=True)
 
             lf = landfire.Landfire(
                 bbox=f"{self.points[0][1]} {self.points[0][0]} \
-                    {self.points[1][1]} {self.points[1][0]}",
+                    {self.points[1][1]+self.pad_distance} \
+                    {self.points[1][0]-self.pad_distance}",
                 output_crs="4326",
             )
             # assume the order of data retrieval stays the same
             lf.request_data(
                 layers=self.layer_products.values(),
                 output_path=str(self.output_path / self.product_layers_path),
             )
```

### Comparing `simfire-1.5.8/simfire/utils/log.py` & `simfire-1.5.9/simfire/utils/log.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy` & `simfire-1.5.9/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy` & `simfire-1.5.9/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/terrain.py` & `simfire-1.5.9/simfire/utils/terrain.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/textures/terrain.jpg` & `simfire-1.5.9/simfire/utils/textures/terrain.jpg`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/utils/units.py` & `simfire-1.5.9/simfire/utils/units.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/world/_tests/test_cfd_wind.py` & `simfire-1.5.9/simfire/world/_tests/test_cfd_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/world/_tests/test_elevation_functions.py` & `simfire-1.5.9/simfire/world/_tests/test_elevation_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/world/_tests/test_rothermel.py` & `simfire-1.5.9/simfire/world/_tests/test_rothermel.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/world/_tests/test_wind.py` & `simfire-1.5.9/simfire/world/_tests/test_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/world/elevation_functions.py` & `simfire-1.5.9/simfire/world/elevation_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/world/fuel_array_functions.py` & `simfire-1.5.9/simfire/world/fuel_array_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/world/parameters.py` & `simfire-1.5.9/simfire/world/parameters.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/world/presets.py` & `simfire-1.5.9/simfire/world/presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Fir delta, the Fuel bed depth is used
 
 As specified in: https://www.fs.fed.us/rm/pubs_series/rmrs/gtr/rmrs_gtr371.pdf
 
 Urban, Snow/Ice, Agricutlture, Water, Barren are Non-Burnable fuel types as described in:
 https://gacc.nifc.gov/oncc/docs/40-Standard%20Fire%20Behavior%20Fuel%20Models.pdf
 """
+
 from .parameters import Fuel
 
 ShortGrass = Fuel(w_0=0.0340, delta=1.000, M_x=0.1200, sigma=3500)
 
 GrassTimberShrubOverstory = Fuel(w_0=0.0918, delta=1.000, M_x=0.1500, sigma=2784)
 
 TallGrass = Fuel(w_0=0.1377, delta=2.500, M_x=0.2500, sigma=1500)
```

### Comparing `simfire-1.5.8/simfire/world/rothermel.py` & `simfire-1.5.9/simfire/world/rothermel.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/world/wind_mechanics/cfd_wind.py` & `simfire-1.5.9/simfire/world/wind_mechanics/cfd_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/world/wind_mechanics/perlin_wind.py` & `simfire-1.5.9/simfire/world/wind_mechanics/perlin_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/simfire/world/wind_mechanics/wind_controller.py` & `simfire-1.5.9/simfire/world/wind_mechanics/wind_controller.py`

 * *Files identical despite different names*

### Comparing `simfire-1.5.8/PKG-INFO` & `simfire-1.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: simfire
-Version: 1.5.8
+Version: 1.5.9
 Summary: Fire simulator built in Python
 Home-page: https://github.com/mitrefireline/simfire
 Keywords: python,reinforcement learning,simulation,fire
 Author: Tim Welsh
 Author-email: twelsh@mitre.org
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Pillow (>=9.1.1,<10.0.0)
+Requires-Dist: Pillow (>=9.1.1,<11.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: geotiff (>=0.2.10,<0.3.0)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: imagecodecs (>=2023.7.10,<2024.0.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: landfire (>=0.5.0,<0.6.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
```

