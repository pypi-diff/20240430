# Comparing `tmp/open_samus_returns_rando-1.2.0.tar.gz` & `tmp/open_samus_returns_rando-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_samus_returns_rando-1.2.0.tar", last modified: Sun Apr 21 14:15:38 2024, max compression
+gzip compressed data, was "open_samus_returns_rando-1.2.1.tar", last modified: Tue Apr 30 00:18:16 2024, max compression
```

## Comparing `open_samus_returns_rando-1.2.0.tar` & `open_samus_returns_rando-1.2.1.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.515809 open_samus_returns_rando-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.515809 open_samus_returns_rando-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.519809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.519809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/__pyinstaller/hook-open_samus_returns_rando.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.519809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.519809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/doors.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/guilib.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/heatzone.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/room_names.lua
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/savestation.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/scenario.lua
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/ship.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/sprites_splashes.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.523809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/
--rw-r--r--   0 runner    (1001) docker     (127)    26259 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s000_surface.lua
--rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s010_area1.lua
--rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s020_area2.lua
--rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s025_area2b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s028_area2c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    27509 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s030_area3.lua
--rw-r--r--   0 runner    (1001) docker     (127)    40894 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s033_area3b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s036_area3c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s040_area4.lua
--rw-r--r--   0 runner    (1001) docker     (127)    34925 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s050_area5.lua
--rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s060_area6.lua
--rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s065_area6b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    18231 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s067_area6c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    41935 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s070_area7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s090_area9.lua
--rw-r--r--   0 runner    (1001) docker     (127)    39148 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s100_area10.lua
--rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.527809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerbabyhatchling.lua
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerenergyshield.lua
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerenergywave.lua
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerphasedisplacement.lua
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerreservetankm.lua
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerscanningpulse.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersuit.lua
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.527809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.527809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.527809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    43927 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.515809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/gui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.527809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/gui/textures/
--rw-r--r--   0 runner    (1001) docker     (127)   524553 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    22654 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.531809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/cc_to_room_name.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/chozoseal_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/cosmetics.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/custom_init.lua
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/elevators.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/metroid_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/progressive_model_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/lua_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.531809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/collision_camera_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/elevators.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/exefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/spawn_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/text_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/patch_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.531809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/custom_pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/model_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/samus_returns_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.531809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/door_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/game_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/heat_room_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/hint_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/map_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/metroid_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/static_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/tunable_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/tests/test_files/item_models_test.json
--rw-r--r--   0 runner    (1001) docker     (127)   147194 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/tests/test_files/starter_preset_patcher.json
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/tests/test_lua_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.626991 open_samus_returns_rando-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.606991 open_samus_returns_rando-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.606991 open_samus_returns_rando-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-30 00:18:16.626991 open_samus_returns_rando-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 00:18:16.626991 open_samus_returns_rando-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.602991 open_samus_returns_rando-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.606991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.610991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/__pyinstaller/hook-open_samus_returns_rando.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.610991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.610991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/doors.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/guilib.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/heatzone.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/room_names.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/savestation.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/scenario.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/ship.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/sprites_splashes.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.614991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/
+-rw-r--r--   0 runner    (1001) docker     (127)    26259 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s000_surface.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s010_area1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s020_area2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s025_area2b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s028_area2c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    27509 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s030_area3.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    40894 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s033_area3b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s036_area3c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s040_area4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    34925 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s050_area5.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s060_area6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s065_area6b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18231 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s067_area6c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    41935 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s070_area7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s090_area9.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    39148 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s100_area10.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.618991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerbabyhatchling.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerenergyshield.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerenergywave.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerphasedisplacement.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerreservetankm.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerscanningpulse.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizersuit.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.602991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.602991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.602991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.602991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.618991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.618991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.602991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.602991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.602991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.618991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    43927 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.602991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/gui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.618991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/gui/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)   524553 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    22654 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.622991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/cc_to_room_name.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/chozoseal_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/cosmetics.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/custom_init.lua
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/elevators.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/metroid_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/progressive_model_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/lua_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.622991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/collision_camera_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/elevators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/exefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/spawn_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/text_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.622991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/pickups/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/pickups/custom_pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/pickups/model_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/pickups/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/samus_returns_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.626991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/door_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/game_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/heat_room_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/hint_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/map_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/metroid_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/static_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/tunable_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 00:18:16.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.626991 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-30 00:18:16.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-30 00:18:16.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:18:16.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-30 00:18:16.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 00:18:16.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 00:18:16.000000 open_samus_returns_rando-1.2.1/src/open_samus_returns_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.626991 open_samus_returns_rando-1.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:18:16.626991 open_samus_returns_rando-1.2.1/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/tests/test_files/item_models_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)   147194 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/tests/test_files/starter_preset_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 00:18:01.000000 open_samus_returns_rando-1.2.1/tests/test_lua_util.py
```

### Comparing `open_samus_returns_rando-1.2.0/.github/dependabot.yml` & `open_samus_returns_rando-1.2.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/.github/workflows/python.yml` & `open_samus_returns_rando-1.2.1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/.gitignore` & `open_samus_returns_rando-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/LICENSE` & `open_samus_returns_rando-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/PKG-INFO` & `open_samus_returns_rando-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_samus_returns_rando
-Version: 1.2.0
+Version: 1.2.1
 Summary: An open source randomizer patcher for Metroid: Samus Returns.
 Project-URL: Homepage, https://github.com/randovania/open-samus-returns-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -13,19 +13,22 @@
 Requires-Dist: mercury-engine-data-structures>=0.27.0
 Requires-Dist: jsonschema>=4.0.0
 Requires-Dist: ips.py>=0.1.2
 
 # Open Samus Returns Rando
 Open Source randomizer patcher for Metroid: Samus Returns. Intended for use in [Randovania](https://github.com/randovania).
 Currently supports patching the following:
-- Starting items
-- Starting location
-- Pickups
+- Starting Items
+- Starting Location
+- Pickups (Vanilla and Custom)
 - Items on Metroids
-- Shuffled DNA/Baby Metroid
+- Shuffled DNA
+- Shuffled Baby Metroid
+- Elevator Destinations
+- Door Types
 
 ## Installation and Usage
 `pip install open-samus-returns-rando`
 
 You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-samus-returns-rando/blob/main/src/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
 
 The patcher expects a path to an extracted romfs directory of Metroid: Samus Returns as well as the desired output directory. Output files are in a format compatible with either Luma3DS or Citra.
```

### Comparing `open_samus_returns_rando-1.2.0/README.md` & `open_samus_returns_rando-1.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Open Samus Returns Rando
 Open Source randomizer patcher for Metroid: Samus Returns. Intended for use in [Randovania](https://github.com/randovania).
 Currently supports patching the following:
-- Starting items
-- Starting location
-- Pickups
+- Starting Items
+- Starting Location
+- Pickups (Vanilla and Custom)
 - Items on Metroids
-- Shuffled DNA/Baby Metroid
+- Shuffled DNA
+- Shuffled Baby Metroid
+- Elevator Destinations
+- Door Types
 
 ## Installation and Usage
 `pip install open-samus-returns-rando`
 
 You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-samus-returns-rando/blob/main/src/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
 
 The patcher expects a path to an extracted romfs directory of Metroid: Samus Returns as well as the desired output directory. Output files are in a format compatible with either Luma3DS or Citra.
```

### Comparing `open_samus_returns_rando-1.2.0/pyproject.toml` & `open_samus_returns_rando-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/cli.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/constants.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/constants.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/debug.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/debug.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/doors.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/doors.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/guilib.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/guilib.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/heatzone.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/heatzone.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/room_names.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/room_names.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/savestation.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/savestation.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/scenario.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/scenario.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/ship.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/ship.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/sprites_splashes.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/custom/sprites_splashes.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s000_surface.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s000_surface.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s010_area1.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s010_area1.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s020_area2.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s020_area2.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s025_area2b.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s025_area2b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s028_area2c.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s028_area2c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s030_area3.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s030_area3.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s033_area3b.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s033_area3b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s036_area3c.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s036_area3c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s040_area4.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s040_area4.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s050_area5.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s050_area5.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s060_area6.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s060_area6.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s065_area6b.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s065_area6b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s067_area6c.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s067_area6c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s070_area7.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s070_area7.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s090_area9.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s090_area9.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s100_area10.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s100_area10.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersuit.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizersuit.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/schema.json` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/schema.json`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/chozoseal_template.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/chozoseal_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/cosmetics.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/cosmetics.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/custom_init.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/custom_init.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/metroid_template.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/metroid_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/lua_editor.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/lua_editor.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/collision_camera_table.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/collision_camera_table.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/credits.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/credits.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/elevators.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/elevators.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/lua_util.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/lua_util.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/spawn_points.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/spawn_points.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/text_patches.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/misc_patches/text_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/patch_util.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/patch_util.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/patcher_editor.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/model_data.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/pickups/model_data.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/pickup.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/pickups/pickup.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/samus_returns_patcher.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/samus_returns_patcher.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/door_patches.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/door_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/game_patches.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/game_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/heat_room_patches.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/heat_room_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/map_icons.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/map_icons.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/static_fixes.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/static_fixes.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         # All other enemies excluding Blobthrower
         else:
             drop["fPowerBombProbability"]["value"] *= 2
 
 
 def fix_wrong_cc_actor_deletions(editor: PatcherEditor):
     # Prevents hidden item actors from being deleted when its block is broken from an adjacent cc
-    BOMB_BLOCK = Container({
+    CUSTOM_BLOCK = Container({
         "pos": ListContainer([
             -10350.0,
             -1850.0,
             0.0,
         ]),
         "unk2": 0,
         "unk3": 0,
@@ -216,16 +216,26 @@
         "name1": "sg_casca38",
         "name2": ""
     })
     BOMB_GROUP = Container(
         unk_bool=True,
         types=ListContainer([Container(block_type='bomb', blocks=ListContainer([]))])
     )
+    BEAM_GROUP = Container(
+        unk_bool=True,
+        types=ListContainer([Container(block_type='powerbeam', blocks=ListContainer([]))])
+    )
+    BMSBK_GROUP = Container(
+        name="bg_SubArea_collision_camera_023", entries=ListContainer([])
+    )
 
     scenario_powerup_eg = {
+        "s000_surface": [
+            {"powerup_name": "HiddenPowerup001", "cc": "collision_camera_023"},
+        ],
         "s010_area1": [
             {"powerup_name": "HiddenPowerup001", "cc": "collision_camera_018"},
         ],
         "s025_area2b": [
             {"powerup_name": "HP_Item_001", "cc": "collision_camera012"},
         ],
         "s050_area5": [
@@ -245,31 +255,36 @@
 
             powerup_actor = next(
                 actor for layer, actor_name, actor in scenario.all_actors() if actor_name == powerup_name
             )
             # Make actor freestanding
             powerup_actor["components"][0]["arguments"][0]["value"] = ""
 
-            # add block on top of item
+            # Add block on top of item
             bmsbk = editor.get_file(
                 f"maps/levels/c10_samus/{scenario_name}/{scenario_name}.bmsbk", Bmsbk
             )
             sg_casca = powerup_actor.components[0].arguments[2].value
             pos = powerup_actor.position
-            new_group = copy.deepcopy(BOMB_GROUP)
-            new_block = copy.deepcopy(BOMB_BLOCK)
+            # Edge case for the beam block in Surface
+            if scenario_name == "s000_surface":
+                new_group = copy.deepcopy(BEAM_GROUP)
+                # Add the missing collision_camera entry
+                bmsbk.raw.collision_cameras.append(BMSBK_GROUP)
+            else:
+                new_group = copy.deepcopy(BOMB_GROUP)
+            new_block = copy.deepcopy(CUSTOM_BLOCK)
             new_block.pos = pos
             new_block.name1 = sg_casca
             new_group.types[0].blocks.append(new_block)
             bmsbk.raw.block_groups.append(new_group)
             bmsbk_cc_obj = next(cc_obj for cc_obj in bmsbk.raw.collision_cameras if cc_name in cc_obj.name)
             bmsbk_cc_obj.entries.append(len(bmsbk.raw.block_groups) - 1)
 
 
-
 def apply_static_fixes(editor: PatcherEditor):
     patch_multi_room_gammas(editor)
     patch_pickup_rotation(editor)
     patch_pickup_position(editor)
     remove_area7_grapple_block(editor)
     patch_a7_save_screw_blocks(editor)
     shoot_supers_without_missiles(editor)
```

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/tunable_patches.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/specific_patches/tunable_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/validator_with_default.py` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/PKG-INFO` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_samus_returns_rando
-Version: 1.2.0
+Version: 1.2.1
 Summary: An open source randomizer patcher for Metroid: Samus Returns.
 Project-URL: Homepage, https://github.com/randovania/open-samus-returns-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -13,19 +13,22 @@
 Requires-Dist: mercury-engine-data-structures>=0.27.0
 Requires-Dist: jsonschema>=4.0.0
 Requires-Dist: ips.py>=0.1.2
 
 # Open Samus Returns Rando
 Open Source randomizer patcher for Metroid: Samus Returns. Intended for use in [Randovania](https://github.com/randovania).
 Currently supports patching the following:
-- Starting items
-- Starting location
-- Pickups
+- Starting Items
+- Starting Location
+- Pickups (Vanilla and Custom)
 - Items on Metroids
-- Shuffled DNA/Baby Metroid
+- Shuffled DNA
+- Shuffled Baby Metroid
+- Elevator Destinations
+- Door Types
 
 ## Installation and Usage
 `pip install open-samus-returns-rando`
 
 You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-samus-returns-rando/blob/main/src/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
 
 The patcher expects a path to an extracted romfs directory of Metroid: Samus Returns as well as the desired output directory. Output files are in a format compatible with either Luma3DS or Citra.
```

### Comparing `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/SOURCES.txt` & `open_samus_returns_rando-1.2.1/src/open_samus_returns_rando.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/tests/test_files/item_models_test.json` & `open_samus_returns_rando-1.2.1/tests/test_files/item_models_test.json`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.2.0/tests/test_files/starter_preset_patcher.json` & `open_samus_returns_rando-1.2.1/tests/test_files/starter_preset_patcher.json`

 * *Files identical despite different names*

