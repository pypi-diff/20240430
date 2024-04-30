# Comparing `tmp/kintree-1.0.7.tar.gz` & `tmp/kintree-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kintree-1.0.7.tar", max compression
+gzip compressed data, was "kintree-1.1.0.tar", max compression
```

## Comparing `kintree-1.0.7.tar` & `kintree-1.1.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    35149 2024-03-05 20:50:44.436924 kintree-1.0.7/LICENSE
--rw-r--r--   0        0        0    17309 2024-03-05 20:50:44.436924 kintree-1.0.7/README.md
--rw-r--r--   0        0        0       22 2024-03-05 20:50:44.532925 kintree-1.0.7/kintree/__init__.py
--rw-r--r--   0        0        0     5450 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/common/part_tools.py
--rw-r--r--   0        0        0     1214 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/common/progress.py
--rw-r--r--   0        0        0     5540 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/common/tools.py
--rw-r--r--   0        0        0    17359 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/config_interface.py
--rw-r--r--   0        0        0       47 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/digikey/digikey_api.yaml
--rw-r--r--   0        0        0     2745 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/digikey/digikey_categories.yaml
--rw-r--r--   0        0        0      248 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/digikey/digikey_config.yaml
--rw-r--r--   0        0        0       99 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/element14/element14_api.yaml
--rw-r--r--   0        0        0      244 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/element14/element14_config.yaml
--rw-r--r--   0        0        0     1633 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/inventree/categories.yaml
--rw-r--r--   0        0        0      128 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/inventree/inventree_dev.yaml
--rw-r--r--   0        0        0      128 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/inventree/inventree_prod.yaml
--rw-r--r--   0        0        0     1016 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/inventree/parameters.yaml
--rw-r--r--   0        0        0      553 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/inventree/parameters_filters.yaml
--rw-r--r--   0        0        0       21 2024-03-05 20:50:44.444924 kintree-1.0.7/kintree/config/inventree/stock_locations.yaml
--rw-r--r--   0        0        0     5374 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/inventree/supplier_parameters.yaml
--rw-r--r--   0        0        0      267 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/inventree/suppliers.yaml
--rw-r--r--   0        0        0       95 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/kicad/kicad.yaml
--rw-r--r--   0        0        0     1161 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/kicad/kicad_map.yaml
--rw-r--r--   0        0        0       68 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/lcsc/lcsc_api.yaml
--rw-r--r--   0        0        0      256 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/lcsc/lcsc_config.yaml
--rw-r--r--   0        0        0       25 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/mouser/mouser_api.yaml
--rw-r--r--   0        0        0      258 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/mouser/mouser_config.yaml
--rw-r--r--   0        0        0    12419 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/settings.py
--rw-r--r--   0        0        0       81 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/tme/tme_api.yaml
--rw-r--r--   0        0        0      224 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/tme/tme_config.yaml
--rw-r--r--   0        0        0      255 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/user/general.yaml
--rw-r--r--   0        0        0      223 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/user/internal_part_number.yaml
--rw-r--r--   0        0        0       73 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/config/user/search_api.yaml
--rw-r--r--   0        0        0    30741 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/database/inventree_api.py
--rw-r--r--   0        0        0    40401 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/database/inventree_interface.py
--rw-r--r--   0        0        0     3360 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/gui/gui.py
--rw-r--r--   0        0        0    38788 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/gui/logo.png
--rw-r--r--   0        0        0    14544 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/gui/views/common.py
--rw-r--r--   0        0        0    61222 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/gui/views/main.py
--rw-r--r--   0        0        0    35988 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/gui/views/settings.py
--rw-r--r--   0        0        0      416 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/kicad_interface.py
--rw-r--r--   0        0        0     4449 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/kicad_symbol.py
--rw-r--r--   0        0        0     7048 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/LICENSE
--rw-r--r--   0        0        0     3077 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/capacitor-polarized.kicad_sym
--rw-r--r--   0        0        0     2786 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/capacitor.kicad_sym
--rw-r--r--   0        0        0     1089 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/connector.kicad_sym
--rw-r--r--   0        0        0     2540 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/crystal-2p.kicad_sym
--rw-r--r--   0        0        0     1091 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/default.kicad_sym
--rw-r--r--   0        0        0     2647 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/diode-led.kicad_sym
--rw-r--r--   0        0        0     2453 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/diode-schottky.kicad_sym
--rw-r--r--   0        0        0     2251 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/diode-standard.kicad_sym
--rw-r--r--   0        0        0     2445 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/diode-zener.kicad_sym
--rw-r--r--   0        0        0     2116 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/eeprom-sot23.kicad_sym
--rw-r--r--   0        0        0     2445 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/ferrite-bead.kicad_sym
--rw-r--r--   0        0        0     2249 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/fuse.kicad_sym
--rw-r--r--   0        0        0     2258 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/inductor.kicad_sym
--rw-r--r--   0        0        0     1089 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/integrated-circuit.kicad_sym
--rw-r--r--   0        0        0       65 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/library_template.kicad_sym
--rw-r--r--   0        0        0     2140 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/oscillator-4p.kicad_sym
--rw-r--r--   0        0        0     2451 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/protection-unidir.kicad_sym
--rw-r--r--   0        0        0     2233 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/resistor-sm.kicad_sym
--rw-r--r--   0        0        0     2233 2024-03-05 20:50:44.448924 kintree-1.0.7/kintree/kicad/templates/resistor.kicad_sym
--rw-r--r--   0        0        0     4683 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/kicad/templates/transistor-nfet.kicad_sym
--rw-r--r--   0        0        0     2795 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/kicad/templates/transistor-npn.kicad_sym
--rw-r--r--   0        0        0     4986 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/kicad/templates/transistor-pfet.kicad_sym
--rw-r--r--   0        0        0     2800 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/kicad/templates/transistor-pnp.kicad_sym
--rw-r--r--   0        0        0     1981 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/kicad/templates_project/templates_project.kicad_pcb
--rw-r--r--   0        0        0     1201 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/kicad/templates_project/templates_project.kicad_prl
--rw-r--r--   0        0        0     6077 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/kicad/templates_project/templates_project.kicad_pro
--rw-r--r--   0        0        0      187 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/kicad/templates_project/templates_project.kicad_sch
--rw-r--r--   0        0        0      227 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/kintree_gui.py
--rw-r--r--   0        0        0     7072 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/search/digikey_api.py
--rw-r--r--   0        0        0    12187 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/search/element14_api.py
--rw-r--r--   0        0        0     3985 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/search/lcsc_api.py
--rw-r--r--   0        0        0     4349 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/search/mouser_api.py
--rw-r--r--   0        0        0     1243 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/search/search_api.py
--rw-r--r--   0        0        0     4064 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/search/snapeda_api.py
--rw-r--r--   0        0        0     7170 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/search/tme_api.py
--rw-r--r--   0        0        0     2114 2024-03-05 20:50:44.452924 kintree-1.0.7/kintree/setup_inventree.py
--rw-r--r--   0        0        0     1003 2024-03-05 20:50:44.532925 kintree-1.0.7/pyproject.toml
--rw-r--r--   0        0        0    18508 1970-01-01 00:00:00.000000 kintree-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 17:28:24.305549 kintree-1.1.0/LICENSE
+-rw-r--r--   0        0        0    17562 2024-04-30 17:28:24.305549 kintree-1.1.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-30 17:28:24.417552 kintree-1.1.0/kintree/__init__.py
+-rw-r--r--   0        0        0     5450 2024-04-30 17:28:24.309549 kintree-1.1.0/kintree/common/part_tools.py
+-rw-r--r--   0        0        0     1214 2024-04-30 17:28:24.309549 kintree-1.1.0/kintree/common/progress.py
+-rw-r--r--   0        0        0     5540 2024-04-30 17:28:24.309549 kintree-1.1.0/kintree/common/tools.py
+-rw-r--r--   0        0        0    17359 2024-04-30 17:28:24.309549 kintree-1.1.0/kintree/config/config_interface.py
+-rw-r--r--   0        0        0       47 2024-04-30 17:28:24.309549 kintree-1.1.0/kintree/config/digikey/digikey_api.yaml
+-rw-r--r--   0        0        0     2745 2024-04-30 17:28:24.309549 kintree-1.1.0/kintree/config/digikey/digikey_categories.yaml
+-rw-r--r--   0        0        0      248 2024-04-30 17:28:24.309549 kintree-1.1.0/kintree/config/digikey/digikey_config.yaml
+-rw-r--r--   0        0        0       99 2024-04-30 17:28:24.309549 kintree-1.1.0/kintree/config/element14/element14_api.yaml
+-rw-r--r--   0        0        0      244 2024-04-30 17:28:24.309549 kintree-1.1.0/kintree/config/element14/element14_config.yaml
+-rw-r--r--   0        0        0     1633 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/inventree/categories.yaml
+-rw-r--r--   0        0        0      128 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/inventree/inventree_dev.yaml
+-rw-r--r--   0        0        0      128 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/inventree/inventree_prod.yaml
+-rw-r--r--   0        0        0     1016 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/inventree/parameters.yaml
+-rw-r--r--   0        0        0      553 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/inventree/parameters_filters.yaml
+-rw-r--r--   0        0        0       21 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/inventree/stock_locations.yaml
+-rw-r--r--   0        0        0     5374 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/inventree/supplier_parameters.yaml
+-rw-r--r--   0        0        0      267 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/inventree/suppliers.yaml
+-rw-r--r--   0        0        0       95 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/kicad/kicad.yaml
+-rw-r--r--   0        0        0     1161 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/kicad/kicad_map.yaml
+-rw-r--r--   0        0        0       68 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/lcsc/lcsc_api.yaml
+-rw-r--r--   0        0        0      256 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/lcsc/lcsc_config.yaml
+-rw-r--r--   0        0        0       25 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/mouser/mouser_api.yaml
+-rw-r--r--   0        0        0      258 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/mouser/mouser_config.yaml
+-rw-r--r--   0        0        0    12419 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/settings.py
+-rw-r--r--   0        0        0       81 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/tme/tme_api.yaml
+-rw-r--r--   0        0        0      224 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/tme/tme_config.yaml
+-rw-r--r--   0        0        0      255 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/user/general.yaml
+-rw-r--r--   0        0        0      223 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/user/internal_part_number.yaml
+-rw-r--r--   0        0        0       73 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/config/user/search_api.yaml
+-rw-r--r--   0        0        0    30741 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/database/inventree_api.py
+-rw-r--r--   0        0        0    40425 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/database/inventree_interface.py
+-rw-r--r--   0        0        0     3272 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/gui/gui.py
+-rw-r--r--   0        0        0    38788 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/gui/logo.png
+-rw-r--r--   0        0        0    14525 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/gui/views/common.py
+-rw-r--r--   0        0        0    61775 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/gui/views/main.py
+-rw-r--r--   0        0        0    36060 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/gui/views/settings.py
+-rw-r--r--   0        0        0      416 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/kicad_interface.py
+-rw-r--r--   0        0        0     4449 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/kicad_symbol.py
+-rw-r--r--   0        0        0     7048 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/LICENSE
+-rw-r--r--   0        0        0     3077 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/capacitor-polarized.kicad_sym
+-rw-r--r--   0        0        0     2786 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/capacitor.kicad_sym
+-rw-r--r--   0        0        0     1089 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/connector.kicad_sym
+-rw-r--r--   0        0        0     2540 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/crystal-2p.kicad_sym
+-rw-r--r--   0        0        0     1091 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/default.kicad_sym
+-rw-r--r--   0        0        0     2647 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/diode-led.kicad_sym
+-rw-r--r--   0        0        0     2453 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/diode-schottky.kicad_sym
+-rw-r--r--   0        0        0     2251 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/diode-standard.kicad_sym
+-rw-r--r--   0        0        0     2445 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/diode-zener.kicad_sym
+-rw-r--r--   0        0        0     2116 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/eeprom-sot23.kicad_sym
+-rw-r--r--   0        0        0     2445 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/ferrite-bead.kicad_sym
+-rw-r--r--   0        0        0     2249 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/fuse.kicad_sym
+-rw-r--r--   0        0        0     2258 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/inductor.kicad_sym
+-rw-r--r--   0        0        0     1089 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/integrated-circuit.kicad_sym
+-rw-r--r--   0        0        0       65 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/library_template.kicad_sym
+-rw-r--r--   0        0        0     2140 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/oscillator-4p.kicad_sym
+-rw-r--r--   0        0        0     2451 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/protection-unidir.kicad_sym
+-rw-r--r--   0        0        0     2233 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/resistor-sm.kicad_sym
+-rw-r--r--   0        0        0     2233 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/resistor.kicad_sym
+-rw-r--r--   0        0        0     4683 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/transistor-nfet.kicad_sym
+-rw-r--r--   0        0        0     2795 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/transistor-npn.kicad_sym
+-rw-r--r--   0        0        0     4986 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/transistor-pfet.kicad_sym
+-rw-r--r--   0        0        0     2800 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates/transistor-pnp.kicad_sym
+-rw-r--r--   0        0        0     1981 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates_project/templates_project.kicad_pcb
+-rw-r--r--   0        0        0     1201 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates_project/templates_project.kicad_prl
+-rw-r--r--   0        0        0     6077 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates_project/templates_project.kicad_pro
+-rw-r--r--   0        0        0      187 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kicad/templates_project/templates_project.kicad_sch
+-rw-r--r--   0        0        0      227 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/kintree_gui.py
+-rw-r--r--   0        0        0     7072 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/search/digikey_api.py
+-rw-r--r--   0        0        0    12187 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/search/element14_api.py
+-rw-r--r--   0        0        0     3985 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/search/lcsc_api.py
+-rw-r--r--   0        0        0     4409 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/search/mouser_api.py
+-rw-r--r--   0        0        0     1243 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/search/search_api.py
+-rw-r--r--   0        0        0     4064 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/search/snapeda_api.py
+-rw-r--r--   0        0        0     7170 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/search/tme_api.py
+-rw-r--r--   0        0        0     2114 2024-04-30 17:28:24.313550 kintree-1.1.0/kintree/setup_inventree.py
+-rw-r--r--   0        0        0     1005 2024-04-30 17:28:24.417552 kintree-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    18770 1970-01-01 00:00:00.000000 kintree-1.1.0/PKG-INFO
```

### Comparing `kintree-1.0.7/LICENSE` & `kintree-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/README.md` & `kintree-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 5. If you intend to use InvenTree with this tool, click on "Settings > InvenTree" and fill in your InvenTree server address and credentials then click "Save" (optional: click on "Test" to check communication with server)  
   a. It is possible to define a Proxy Server over which all interactions with InvenTree will be routed. To set a proxy server use the "Enable Proxy Support" switch in "Settings > InvenTree" and define the proxy address in the new input field.  
   b. Instead of user credential authentication token authentication is also supported. To use a token add it it to the "Password or Token" field and leave the "Username" empty. You can retrieve your personal access token from your InvenTree server by sending an get-request to its api url `api/user/token/`.
   c. If needed this tool can try to download the parts datasheet from the suppliers and upload it it to the attachment section of each part. For this just activate "Upload Datasheets to InvenTree" in the InvenTree settings
   d. It is also possible to sync the prices in InvenTree with the latest supplier prices. For this enable "Upload Pricing Data to InvenTree"
 6. If your InvenTree server requires a IPN in a specific pattern make sure to adjust "Settings > InvenTree > Internal Part Number" to match it or adjust the servers pattern to the one yo set in Ki-nTree 
 
+> Note: All URLs should start with "http://" if they do not have a valid SSL certificate.
 
 #### Get Digi-Key API token
 <details>
 <summary>Show steps (click to expand)</summary>
 <p>
 
 Enter your Digi-Key developer account credentials then login. The following page will appear (`user@email.com` will show your email address):
@@ -200,20 +201,22 @@
 
 Refer to [this file](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/config/inventree/supplier_parameters.yaml) as a starting point / example.
 
 #### Part Number Search
 
 Ki-nTree currently supports APIs for the following electronics suppliers: Digi-Key, Mouser, Element14, TME and LCSC.
 
-1. In the main window, enter the part number and select the supplier in drop-down list, then click "CREATE". It will start by fetching part data using the supplier's API
+1. In the main window, enter the part number and select the supplier in drop-down list, then click the "Submit" button (arrow). It will start by fetching part data using the supplier's API
 2. In the case Digi-Key has been selected and the API token is not found or expired, a browser window will pop-up. To get a new token: [follow those steps](#get-digi-key-api-token)
-3. Once the part data has been successfully fetched from the supplier's API, you will be prompted to add/confirm/edit the part information, followed by the `Category` and `Subcategory` to use for this part (Ki-nTree tries to match them automatically)
-4. Then, you will be prompted with selecting the KiCad symbol library, the template and the footprint library to use for this part
-5. It will take some time to complete the part creation in InvenTree and/or KiCad, once it finishes you'll be notified of the result  
-6. Finally, if the part was created or found in InvenTree, your browser will automatically open a new tab with the part information
+3. Once the part data has been successfully fetched from the supplier's API, you can review the part information in the different fields and edit them, if needed.
+4. Then, go to the Inventree tabl to pick the `Category` and `Subcategory` to use for this part
+5. If you desire to add this part to KiCad, click the KiCad tab and select the KiCad symbol library, the template and the footprint library to use for this part
+6. Finally, go to the Create tab and launch the part creation. It will take some time to complete the process in InvenTree and/or KiCad, once it finishes you'll be notified of the result  
+
+If the part was created or found in InvenTree, and if you have selected this option in the settings, your browser will automatically open and navigate to the new Inventree part page.
 
 #### Kicad Templates
 
 The automatic part generation in KiCad is controlled via templates:
 
 * Template examples are shipped together with Ki-nTree, these can be adjusted to your liking or you also can create completely new ones.
 * Each template has its own library file where the file name defines the templates name.
@@ -240,15 +243,15 @@
 ```
 
 2. Install the requirements into a `poetry`-managed virtual environment
 ``` bash
 poetry install
 Installing dependencies from lock file
 ...
-Installing the current project: kintree (1.0.99)
+Installing the current project: kintree (1.1.99)
 ```
 > Note: the version is not accurate (placeholder only)
 
 3. Run Ki-nTree in the virtual environment
 ```bash
 poetry run python -m kintree_gui
 ```
@@ -259,28 +262,28 @@
 $ python -m kintree_gui
 ```
 
 #### Build
 1. Make sure you followed the previous installation steps, then run:
 ``` bash
 $ poetry build
-Building kintree (1.0.99)
+Building kintree (1.1.99)
   - Building sdist
-  - Built kintree-1.0.99.tar.gz
+  - Built kintree-1.1.99.tar.gz
   - Building wheel
-  - Built kintree-1.0.99-py3-none-any.whl
+  - Built kintree-1.1.99-py3-none-any.whl
 ```
 2. Exit the virtual environment (`Ctrl + D` on Linux; you can also close the
    terminal and reopen it in the same folder).
 
    Run `pip install dist/<wheel_file>.whl` with the file name from the previous
    step. For example:
 
 ```bash
-pip install dist/kintree-1.0.99-py3-none-any.whl
+pip install dist/kintree-1.1.99-py3-none-any.whl
 ```
 
 3. You can now start Ki-nTree by typing `kintree` in the terminal, provided
    that your python dist path is a part of your `$PATH`.
 
 ## License
 The Ki-nTree source code is licensed under the [GPL3.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/LICENSE) as it uses source code under that license:
```

### Comparing `kintree-1.0.7/kintree/common/part_tools.py` & `kintree-1.1.0/kintree/common/part_tools.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/common/progress.py` & `kintree-1.1.0/kintree/common/progress.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/common/tools.py` & `kintree-1.1.0/kintree/common/tools.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/config/config_interface.py` & `kintree-1.1.0/kintree/config/config_interface.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/config/digikey/digikey_categories.yaml` & `kintree-1.1.0/kintree/config/digikey/digikey_categories.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/config/inventree/categories.yaml` & `kintree-1.1.0/kintree/config/inventree/categories.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/config/inventree/parameters.yaml` & `kintree-1.1.0/kintree/config/inventree/parameters.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/config/inventree/parameters_filters.yaml` & `kintree-1.1.0/kintree/config/inventree/parameters_filters.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/config/inventree/supplier_parameters.yaml` & `kintree-1.1.0/kintree/config/inventree/supplier_parameters.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/config/kicad/kicad_map.yaml` & `kintree-1.1.0/kintree/config/kicad/kicad_map.yaml`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/config/settings.py` & `kintree-1.1.0/kintree/config/settings.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/database/inventree_api.py` & `kintree-1.1.0/kintree/database/inventree_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/database/inventree_interface.py` & `kintree-1.1.0/kintree/database/inventree_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,16 @@
         inventree_part['image'] = part_info['image'].replace(' ', '%20')
     except AttributeError:
         # Part image URL is null (no product picture)
         pass
     inventree_part['pricing'] = part_info.get('pricing', {})
     inventree_part['currency'] = part_info.get('currency', 'USD')
 
+    parameters = part_info.get('parameters', {})
+
     # Load parameters map
     if category_tree:
         parameter_map = config_interface.load_category_parameters(
             categories=category_tree,
             supplier_config_path=settings.CONFIG_SUPPLIER_PARAMETERS,
         )
     else:
@@ -331,15 +333,15 @@
                     elif inventree_param == 'image':
                         inventree_part['existing_image'] = supplier_param
                     else:
                         try:
                             parameter_value = part_tools.clean_parameter_value(
                                 category=category_tree[0],
                                 name=supplier_param,
-                                value=part_info['parameters'][supplier_param],
+                                value=parameters[supplier_param],
                             )
                             inventree_part['parameters'][inventree_param] = parameter_value
                         except KeyError:
                             parameters_missing.append(supplier_param)
             if parameters_missing:
                 msg = '[INFO]\tWarning: The following parameters were not found in supplier data:\n'
                 msg += str(parameters_missing)
@@ -350,15 +352,15 @@
                 if inventree_param == 'image':
                     continue
                 if inventree_param not in inventree_part['parameters'].keys():
                     inventree_part['parameters'][inventree_param] = '-'
 
             # Check for extra parameters which weren't mapped
             parameters_unmapped = []
-            for search_param in part_info['parameters'].keys():
+            for search_param in parameters.keys():
                 if search_param not in parameter_map.keys():
                     parameters_unmapped.append(search_param)
             
             if parameters_unmapped:
                 if not settings.SILENT:
                     msg = f'[INFO]\tThe following parameters are not mapped in {inventree_part["supplier_name"]} parameters configuration:\n'
                     msg += str(parameters_unmapped)
```

### Comparing `kintree-1.0.7/kintree/gui/gui.py` & `kintree-1.1.0/kintree/gui/gui.py`

 * *Files 21% similar despite different names*

```diff
@@ -41,72 +41,68 @@
     page.update()
 
 
 def kintree_gui(page: ft.Page):
     '''Ki-nTree GUI'''
     # Init
     init_gui(page)
-    # Views
+    # Create main views
     part_view = PartSearchView(page)
     inventree_view = InventreeView(page)
     kicad_view = KicadView(page)
     create_view = CreateView(page)
-    # Settings
+    # Create settings views
     user_settings_view = UserSettingsView(page)
     supplier_settings_view = SupplierSettingsView(page)
     inventree_settings_view = InvenTreeSettingsView(page)
     kicad_settings_view = KiCadSettingsView(page)
 
+    # Routing
     def route_change(route):
         # print(f'\n--> Routing to {route.route}')
-        if '/main' in page.route:
+        if '/main' in page.route or page.route == '/':
             page.views.clear()
-            if 'part' in page.route:
+            if 'part' in page.route or page.route == '/':
                 page.views.append(part_view)
             if 'inventree' in page.route:
                 page.views.append(inventree_view)
             elif 'kicad' in page.route:
                 page.views.append(kicad_view)
             elif 'create' in page.route:
                 page.views.append(create_view)
         elif '/settings' in page.route:
             if '/settings' in page.views[-1].route:
                 page.views.pop()
-            if page.route == user_settings_view.route:
+            if 'user' in page.route:
                 page.views.append(user_settings_view)
-            elif page.route == supplier_settings_view.route:
+            elif 'supplier' in page.route:
                 page.views.append(supplier_settings_view)
-            elif page.route == inventree_settings_view.route:
+            elif 'inventree' in page.route:
                 page.views.append(inventree_settings_view)
-            elif page.route == kicad_settings_view.route:
+            elif 'kicad' in page.route:
                 page.views.append(kicad_settings_view)
             else:
                 page.views.append(user_settings_view)
-        else:
-            page.views.append(part_view)
-
         page.update()
 
-    def view_pop(e):
+    def view_pop(view):
         '''Pop setting view'''
         page.views.pop()
         top_view = page.views[-1]
         if 'main' in top_view.route:
             handle_transition(page, transition=True)
         # Route and render
         page.go(top_view.route)
         if 'main' in top_view.route:
             handle_transition(
                 page,
                 transition=False,
                 update_page=True,
                 timeout=0.3,
             )
-        if 'part' in top_view.route:
-            part_view.partial_update()
-        elif 'inventree' in top_view.route:
-            inventree_view.partial_update()
+        if '/main/part' in top_view.route or '/main/inventree' in top_view.route:
+            top_view.partial_update()
 
     page.on_route_change = route_change
     page.on_view_pop = view_pop
 
     page.go(page.route)
```

### Comparing `kintree-1.0.7/kintree/gui/logo.png` & `kintree-1.1.0/kintree/gui/logo.png`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/gui/views/common.py` & `kintree-1.1.0/kintree/gui/views/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,39 +75,38 @@
     # Disable transitions by default
     handle_transition(page, transition=False)
 
 
 class CommonView(ft.View):
     '''Common view to all GUI views'''
 
-    page = None
+    _page = None
     navigation_rail = None
-    NAV_BAR_INDEX = None
     title = None
     column = None
     fields = None
     data = None
     dialog = None
     
     def __init__(self, page: ft.Page, appbar: ft.AppBar, navigation_rail: ft.NavigationRail):
         # Store page pointer
-        self.page = page
+        self._page = page
 
         # Init view
         super().__init__(route=self.route, appbar=appbar)
 
         # Set navigation rail
         if not self.navigation_rail:
             self.navigation_rail = navigation_rail
 
     def build_column(self):
         # Empty column (to be set inside the children views)
         self.column = ft.Column()
 
-    def _build(self):
+    def build(self):
         # Build column
         if not self.column:
             self.build_column()
         # Set view controls
         self.controls = [
             ft.Row(
                 controls=[
@@ -160,23 +159,23 @@
             message: Optional[str] = None,
             snackbar=True,
             open=True,
     ):
         if snackbar:
             self.build_snackbar(d_type, message)
         if isinstance(self.dialog, ft.SnackBar):
-            self.page.snack_bar = self.dialog
-            self.page.snack_bar.open = True
+            self._page.snack_bar = self.dialog
+            self._page.snack_bar.open = True
         elif isinstance(self.dialog, ft.Banner):
-            self.page.banner = self.dialog
-            self.page.banner.open = open
+            self._page.banner = self.dialog
+            self._page.banner.open = open
         elif isinstance(self.dialog, ft.AlertDialog):
-            self.page.dialog = self.dialog
-            self.page.dialog.open = open
-        self.page.update()
+            self._page.dialog = self.dialog
+            self._page.dialog.open = open
+        self._page.update()
 
 
 class SwitchWithRefs(ft.Switch):
     '''Link the visibility of other fields to a switch value'''
 
     linked_refs = []
     
@@ -429,15 +428,15 @@
 
     def header_click(self, e):
         self.content.height = None if self.content.height == 0 else 0
         self.content.opacity = 0 if self.content.height == 0 else 1
         self.shevron.rotate = pi / 2 if self.shevron.rotate == 0 else 0
         self.update()
 
-    def _build(self):
+    def build(self):
         title_row = ft.Row()
         if self.icon is not None:
             title_row.controls.append(self.icon)
         if self.radio:
             title_row.controls.append(self.radio)
         else:
             title_row.controls.append(ft.Text(self.title))
@@ -472,15 +471,15 @@
         self.ink = True
         self.on_click = self.item_click
         self.radio = radio
 
     def item_click(self, _):
         pass
 
-    def _build(self):
+    def build(self):
         row = ft.Row()
         if self.icon is not None:
             row.controls.append(self.icon)
         if self.radio:
             row.controls.append(self.radio)
         else:
             row.controls.append(ft.Text(self.title))
```

### Comparing `kintree-1.0.7/kintree/gui/views/main.py` & `kintree-1.1.0/kintree/gui/views/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,19 @@
     },
     'Create': {
         'nav_index': 3,
         'route': '/main/create'
     },
 }
 
+# Load navigation indexes
+NAV_BAR_INDEX = {}
+for view in MAIN_NAVIGATION.values():
+    NAV_BAR_INDEX[view['nav_index']] = view['route']
+
 # Main NavRail
 main_navrail = ft.NavigationRail(
     selected_index=0,
     label_type=ft.NavigationRailLabelType.ALL,
     min_width=100,
     min_extended_width=400,
     group_alignment=-0.9,
@@ -113,47 +118,45 @@
         if not self.appbar.actions:
             self.appbar.actions.append(
                 ft.IconButton(
                     ft.icons.SETTINGS,
                     on_click=self.call_settings,
                 )
             )
-
-        # Load navigation indexes
-        self.NAV_BAR_INDEX = {}
-        for view in MAIN_NAVIGATION.values():
-            self.NAV_BAR_INDEX[view['nav_index']] = view['route']
+        else:
+            self.appbar.actions[0].on_click = self.call_settings
 
         # Update navigation rail
-        if not self.navigation_rail.on_change:
-            self.navigation_rail.on_change = lambda e: self.page.go(self.NAV_BAR_INDEX[e.control.selected_index])
+        self.navigation_rail.on_change = self.nav_rail_redirect
 
         # Init data
         self.data = {}
 
         # Process enable switch
         if 'enable' in self.fields:
             self.fields['enable'].on_change = self.process_enable
 
         # Add floating button to reset view
         self.floating_action_button = ft.FloatingActionButton(
             icon=ft.icons.REPLAY, on_click=self.reset_view,
         )
 
+    def nav_rail_redirect(self, e):
+        self._page.go(NAV_BAR_INDEX[e.control.selected_index])
+
     def call_settings(self, e):
-        handle_transition(self.page, transition=True)
-        self.page.go('/settings')
+        handle_transition(self._page, transition=True)
+        self._page.go('/settings')
 
     def reset_view(self, e, ignore=['enable'], hidden={}):
         def reset_field(field):
             if isinstance(field, ft.ProgressBar):
                 field.value = 0
             else:
                 field.value = None
-            field.update()
 
         for name, field in self.fields.items():
             if isinstance(field, dict):
                 for key, value in field.items():
                     value.disabled = True
                     reset_field(value)
             else:
@@ -165,14 +168,15 @@
                 if not value:
                     self.data[key] = value
                 else:
                     self.data[key] = None
 
         # Clear data
         self.push_data()
+        self._page.update()
 
     def partial_update(self):
         '''Process partial view updates'''
         return
 
     def process_enable(self, e, value=None, ignore=['enable']):
         disabled = False
@@ -208,22 +212,22 @@
 
         # Sanitize data before pushing
         self.sanitize_data()
         # Push
         data_from_views[self.title] = self.data
 
     def did_mount(self, enable=False):
-        handle_transition(self.page, transition=False, update_page=True)
+        handle_transition(self._page, transition=False, update_page=True)
         if self.fields.get('enable', None) is not None:
             # Create enable event
             e = ft.ControlEvent(
                 target=None,
                 name='did_mount_enable',
                 data='true' if enable else 'false',
-                page=self.page,
+                page=self._page,
                 control=self.fields['enable'],
             )
             # Process enable
             self.process_enable(e)
         return super().did_mount()
 
 
@@ -278,21 +282,25 @@
 
     def reset_view(self, e, ignore=['enable']):
         hidden_fields = {
             'searched_part_number': '',
             'custom_part': None,
         }
         self.fields['parameter_form'] = {}
+        try:
+            self.fields['part_number'].focus()
+        except AssertionError:
+            pass
         return super().reset_view(e, ignore=ignore, hidden=hidden_fields)
 
     def enable_search_fields(self):
         for form_field in self.fields['search_form'].values():
             form_field.disabled = False
         self.fields['parameter_view'].disabled = False
-        self.page.update()
+        self._page.update()
         return
 
     def run_search(self, e):
         # Reset view
         self.reset_view(e, ignore=['part_number', 'supplier'])
         self.switch_view()
         # Validate form
@@ -302,16 +310,17 @@
             else:
                 error_msg = 'Missing Supplier'
             self.show_dialog(
                 d_type=DialogType.ERROR,
                 message=error_msg,
             )
         else:
-            self.page.splash.visible = True
-            self.page.update()
+            self.fields['part_number'].value = self.fields['part_number'].value.strip()
+            self._page.splash.visible = True
+            self._page.update()
 
             if not self.fields['part_number'].value and not self.fields['supplier'].value:
                 self.data['custom_part'] = True
                 self.enable_search_fields()
             else:
                 self.data['custom_part'] = False
 
@@ -354,15 +363,15 @@
                     # and pricing
                     if part_supplier_info.get('pricing', None):
                         self.data['pricing'] = part_supplier_info['pricing']
                         self.data['currency'] = part_supplier_info.get('currency', None)
 
             # Add to data buffer
             self.push_data()
-            self.page.splash.visible = False
+            self._page.splash.visible = False
 
             if not self.data['supplier_part_number'] and not self.data['custom_part']:
                 self.show_dialog(
                     d_type=DialogType.ERROR,
                     message='Part not found',
                 )
             elif not self.data['manufacturer_part_number']:
@@ -371,15 +380,15 @@
                     message='Found part has no manufacturer part number',
                 )
             elif self.data['searched_part_number'].lower() != self.data['manufacturer_part_number'].lower():
                 self.show_dialog(
                     d_type=DialogType.WARNING,
                     message='Found manufacturer part number does not match the requested part number',
                 )
-            self.page.update()
+            self._page.update()
         return
 
     def push_data(self, e=None):
         hidden_fields = {
             'searched_part_number': self.fields['part_number'].value,
             'custom_part': self.data.get('custom_part', None),
         }
@@ -425,21 +434,29 @@
         ]
         if not parameters_view:
             for field, text_field in self.fields['search_form'].items():
                 self.column.controls[0].content.controls.append(ft.Row([text_field]))
         else:
             for field, text_field in self.fields['parameter_form'].items():
                 self.column.controls[0].content.controls.append(ft.Row([text_field]))
-        self.page.update()
+        self._page.update()
+
+    def perform_pn_search(self, e):
+        self.run_search(e)
+        try:
+            self.fields['part_number'].focus()
+        except AssertionError:
+            pass
 
     def build_column(self):
         self.update_suppliers()
         # Enable search method
         self.fields['search_button'].on_click = self.run_search
         self.fields['parameter_view'].on_change = self.switch_view
+        self.fields['part_number'].on_submit = self.perform_pn_search
 
         self.column = ft.Column(
             controls=[
                 ft.Container(
                     content=ft.Column(
                         controls=[
                             ft.Row(),
@@ -748,40 +765,40 @@
     def get_stock_location_options(self, reload=False):
         return [
             ft.dropdown.Option(location)
             for location in inventree_interface.build_stock_location_tree(reload=reload)
         ]
         
     def reload_categories(self, e):
-        self.page.splash.visible = True
-        self.page.update()
+        self._page.splash.visible = True
+        self._page.update()
 
         # Check connection
         if not inventree_interface.connect_to_server():
             self.show_dialog(DialogType.ERROR, 'ERROR: Failed to connect to InvenTree server')
         else:
             self.fields['Category'].options = self.get_category_options(reload=True)
             self.fields['Category'].update()
 
-        self.page.splash.visible = False
-        self.page.update()
+        self._page.splash.visible = False
+        self._page.update()
 
     def reload_stock_locations(self, e):
-        self.page.splash.visible = True
-        self.page.update()
+        self._page.splash.visible = True
+        self._page.update()
 
         # Check connection
         if not inventree_interface.connect_to_server():
             self.show_dialog(DialogType.ERROR, 'ERROR: Failed to connect to InvenTree server')
         else:
             self.fields['Stock location'].options = self.get_stock_location_options(reload=True)
             self.fields['Stock location'].update()
 
-        self.page.splash.visible = False
-        self.page.update()
+        self._page.splash.visible = False
+        self._page.update()
 
     def create_ipn_code(self, e):
         # Get switch value
         new_code = True
         if e.data.lower() == 'false':
             new_code = False
 
@@ -982,35 +999,36 @@
             else:
                 modal_msg = ft.Text('Footprint is available on SnapEDA')
         # Build actions
         modal_actions = []
         if download:
             if not symbol and not footprint:
                 if single_result:
-                    modal_actions.append(ft.TextButton('Check Part', on_click=lambda _: self.page.launch_url(download)))
+                    modal_actions.append(ft.TextButton('Check Part', on_click=lambda _: self._page.launch_url(download)))
                 else:
                     modal_msg = ft.Text('Multiple matches found on SnapEDA')
-                    modal_actions.append(ft.TextButton('See Results', on_click=lambda _: self.page.launch_url(download)))
+                    modal_actions.append(ft.TextButton('See Results', on_click=lambda _: self._page.launch_url(download)))
             else:
-                modal_actions.append(ft.TextButton('Download', on_click=lambda _: self.page.launch_url(download)))
+                modal_actions.append(ft.TextButton('Download', on_click=lambda _: self._page.launch_url(download)))
         modal_actions.append(ft.TextButton('Close', on_click=lambda _: self.show_dialog(open=False)))
         
         return ft.AlertDialog(
             modal=True,
             title=modal_msg,
             content=modal_content,
             actions=modal_actions,
             actions_alignment=ft.MainAxisAlignment.END,
             # on_dismiss=None,
         )
     
     def process_enable(self, e, value=None, ignore=['enable']):
         super().process_enable(e, value, ignore)
-        self.fields['Footprint'].disabled = self.fields['New Footprint'].value
-        self.fields['Footprint'].update()
+        if self.fields['enable'].value:
+            self.fields['Footprint'].disabled = self.fields['New Footprint'].value
+            self.fields['Footprint'].update()
         
     def push_data(self, e=None, label=None, value=None):
         super().push_data(e)
         if label or e:
             try:
                 if 'Footprint Library' in [label, e.control.label]:
                     if value:
@@ -1026,26 +1044,26 @@
         if not data_from_views.get('Part Search', {}).get('manufacturer_part_number', ''):
             self.show_dialog(
                 d_type=DialogType.ERROR,
                 message='Missing Manufacturer Part Number',
             )
             return
         
-        self.page.splash.visible = True
-        self.page.update()
+        self._page.splash.visible = True
+        self._page.update()
 
         response = snapeda_api.fetch_snapeda_part_info(data_from_views['Part Search']['manufacturer_part_number'])
         data = snapeda_api.parse_snapeda_response(response)
 
         images = {}
         if data['has_symbol'] or data['has_footprint']:
             images = snapeda_api.download_snapeda_images(data)
 
-        self.page.splash.visible = False
-        self.page.update()
+        self._page.splash.visible = False
+        self._page.update()
         
         self.dialog = self.build_alert_dialog(
             images.get('symbol', ''),
             images.get('footprint', ''),
             data.get('part_url', ''),
             data.get('has_single_result', False),
         )
@@ -1540,15 +1558,15 @@
                 if settings.AUTOMATIC_BROWSER_OPEN:
                     # Auto-Open Browser Window
                     cprint(
                         f'\n[MAIN]\tOpening URL {part_info["inventree_url"]} in browser',
                         silent=settings.SILENT
                     )
                     try:
-                        self.page.launch_url(part_info['inventree_url'])
+                        self._page.launch_url(part_info['inventree_url'])
                     except TypeError:
                         cprint('[INFO]\tError: Failed to open URL', silent=settings.SILENT)
                 else:
                     cprint(f'\n[MAIN]\tPart page URL: {part_info["inventree_url"]}', silent=settings.SILENT)
 
         # Button update
         self.enable_create(True)
```

### Comparing `kintree-1.0.7/kintree/gui/views/settings.py` & `kintree-1.1.0/kintree/gui/views/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,46 +292,48 @@
             selected_icon_content=ft.Icon(name=ft.icons.SETTINGS_INPUT_COMPONENT_OUTLINED, size=GUI_PARAMS['nav_rail_icon_size']),
             padding=GUI_PARAMS['nav_rail_padding'],
         ),
     ],
     on_change=None,
 )
 
+# Navigation indexes (settings)
+NAV_BAR_INDEX = {
+    0: '/settings/user',
+    1: '/settings/supplier',
+    2: '/settings/inventree',
+    3: '/settings/kicad',
+}
+
 
 class SettingsView(CommonView):
     '''Main settings view'''
 
     title = 'Settings'
     route = '/settings'
     settings = None
     settings_file = None
     dialog = None
 
-    # Navigation indexes
-    NAV_BAR_INDEX = {
-        0: '/settings/user',
-        1: '/settings/supplier',
-        2: '/settings/inventree',
-        3: '/settings/kicad',
-    }
-
     def __init__(self, page: ft.Page):
         # Load setting fields
         self.fields = {}
         for field_name, field_data in SETTINGS.get(self.title, {}).items():
             if isinstance(field_data, list) and field_data[0] is not None:
                 self.fields[field_name] = field_data[1]
                 self.fields[field_name].value = self.settings[field_data[0]]
 
         # Init view
         super().__init__(page=page, appbar=settings_appbar, navigation_rail=settings_navrail)
 
         # Update navigation rail
-        if not self.navigation_rail.on_change:
-            self.navigation_rail.on_change = lambda e: self.page.go(self.NAV_BAR_INDEX[e.control.selected_index])
+        self.navigation_rail.on_change = self.nav_rail_redirect
+
+    def nav_rail_redirect(self, e):
+        self._page.go(NAV_BAR_INDEX[e.control.selected_index])
     
     def save(self, settings_file=None, show_dialog=True):
         '''Save settings'''
         if settings_file is not None:
             settings_from_file = config_interface.load_file(settings_file)
         else:
             settings_from_file = config_interface.load_file(self.settings_file)
@@ -355,23 +357,23 @@
                 message=f'{self.title} successfully saved',
             )
 
     def on_dialog_result(self, e: ft.FilePickerResultEvent):
         '''Populate field with user-selected system path'''
         if e.path:
             self.fields[e.control.dialog_title].value = e.path
-            self.page.update()
+            self._page.update()
 
     def path_picker(self, e: ft.ControlEvent, title: str):
         '''Let user browse to a system path'''
-        if self.page.overlay:
-            self.page.overlay.pop()
+        if self._page.overlay:
+            self._page.overlay.pop()
         path_picker = ft.FilePicker(on_result=self.on_dialog_result)
-        self.page.overlay.append(path_picker)
-        self.page.update()
+        self._page.overlay.append(path_picker)
+        self._page.update()
         if self.fields[title].value:
             path_picker.get_directory_path(dialog_title=title, initial_directory=self.fields[title].value)
         else:
             path_picker.get_directory_path(dialog_title=title, initial_directory=global_settings.HOME_DIR)
 
     def init_column(self) -> ft.Column:
         return ft.Column(
@@ -480,15 +482,15 @@
                 self.update_field(name, field, self.column)
 
         # Test and Save buttons
         enable_test = bool(list(SETTINGS[self.title])[-1] == 'Test')
         self.add_buttons(self.column, test=enable_test)
 
     def did_mount(self):
-        handle_transition(self.page, transition=False, timeout=0.05)
+        handle_transition(self._page, transition=False, timeout=0.05)
         return super().did_mount()
     
 
 class PathSettingsView(SettingsView):
     '''Template View for Path Setters'''
 
     def __init__(self, page: ft.Page):
@@ -589,18 +591,20 @@
                     datasheet_row_ref.current = self.column.controls[idx + 1]
                     SETTINGS[self.title]['Save Datasheets to Local Folder'][1].refs = [datasheet_row_ref]
         
         # Save button
         self.add_buttons(self.column, test=False)
 
     def did_mount(self):
-        # Reset Index
-        settings_navrail.selected_index = 0
-        settings_navrail.update()
-
+        try:
+            # Reset Index
+            self.navigation_rail.selected_index = 0
+            self.navigation_rail.update()
+        except AssertionError:
+            pass
         return super().did_mount()
 
 
 class SupplierSettingsView(SettingsView):
     '''Supplier settings view'''
 
     title = 'Supplier Settings'
```

### Comparing `kintree-1.0.7/kintree/kicad/kicad_symbol.py` & `kintree-1.1.0/kintree/kicad/kicad_symbol.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/LICENSE` & `kintree-1.1.0/kintree/kicad/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/capacitor-polarized.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/capacitor-polarized.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/capacitor.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/capacitor.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/connector.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/connector.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/crystal-2p.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/crystal-2p.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/default.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/default.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/diode-led.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/diode-led.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/diode-schottky.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/diode-schottky.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/diode-standard.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/diode-standard.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/diode-zener.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/diode-zener.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/eeprom-sot23.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/eeprom-sot23.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/ferrite-bead.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/ferrite-bead.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/fuse.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/fuse.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/inductor.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/inductor.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/integrated-circuit.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/integrated-circuit.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/oscillator-4p.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/oscillator-4p.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/protection-unidir.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/protection-unidir.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/resistor-sm.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/resistor-sm.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/resistor.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/resistor.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/transistor-nfet.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/transistor-nfet.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/transistor-npn.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/transistor-npn.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/transistor-pfet.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/transistor-pfet.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates/transistor-pnp.kicad_sym` & `kintree-1.1.0/kintree/kicad/templates/transistor-pnp.kicad_sym`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates_project/templates_project.kicad_pcb` & `kintree-1.1.0/kintree/kicad/templates_project/templates_project.kicad_pcb`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates_project/templates_project.kicad_prl` & `kintree-1.1.0/kintree/kicad/templates_project/templates_project.kicad_prl`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/kicad/templates_project/templates_project.kicad_pro` & `kintree-1.1.0/kintree/kicad/templates_project/templates_project.kicad_pro`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/search/digikey_api.py` & `kintree-1.1.0/kintree/search/digikey_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/search/element14_api.py` & `kintree-1.1.0/kintree/search/element14_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/search/lcsc_api.py` & `kintree-1.1.0/kintree/search/lcsc_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/search/mouser_api.py` & `kintree-1.1.0/kintree/search/mouser_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,18 @@
 
 def setup_environment(force=False):
     ''' Setup environmental variables '''
 
     api_key = os.environ.get('MOUSER_PART_API_KEY', None)
     if not api_key or force:
         mouser_api_settings = config_interface.load_file(settings.CONFIG_MOUSER_API)
-        os.environ['MOUSER_PART_API_KEY'] = mouser_api_settings['MOUSER_PART_API_KEY']
+        try:
+            os.environ['MOUSER_PART_API_KEY'] = mouser_api_settings['MOUSER_PART_API_KEY']
+        except TypeError:
+            pass
 
 
 def find_categories(part_details: str):
     ''' Find categories '''
 
     try:
         return part_details['Category'], None
```

### Comparing `kintree-1.0.7/kintree/search/search_api.py` & `kintree-1.1.0/kintree/search/search_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/search/snapeda_api.py` & `kintree-1.1.0/kintree/search/snapeda_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
 def test_snapeda_api() -> bool:
     ''' Test method for SnapEDA API '''
 
     result = False
 
     # Test single result
-    response = fetch_snapeda_part_info('SN74LV4T125PWR')
+    response = fetch_snapeda_part_info('NTR06B2001CTRF')
     data = parse_snapeda_response(response)
     images = download_snapeda_images(data)
 
     if data['part_number'] and data['has_symbol'] and images['symbol']:
         result = True
 
     # Test multiple results
```

### Comparing `kintree-1.0.7/kintree/search/tme_api.py` & `kintree-1.1.0/kintree/search/tme_api.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/kintree/setup_inventree.py` & `kintree-1.1.0/kintree/setup_inventree.py`

 * *Files identical despite different names*

### Comparing `kintree-1.0.7/pyproject.toml` & `kintree-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "kintree"
-version = "1.0.7"
+version = "1.1.0"
 description = "Fast part creation in KiCad and InvenTree"
 authors = ["eeintech <eeintech@eeinte.ch>"]
 maintainers = ["eeintech <eeintech@eeinte.ch>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/sparkmicro/Ki-nTree"
 repository = "https://github.com/sparkmicro/Ki-nTree"
 keywords = ["inventree", "kicad", "digikey", "mouser", "component", "part", "create"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 digikey-api = "^1.0.0"
-flet = "0.7.4"
+flet = "^0.22.0"
 thefuzz = "^0.19.0"
-inventree = "^0.12.1"
+inventree = "^0.13.3"
 kiutils = "^1.4.0"
 mouser = "^0.1.3"
 multiprocess = "^0.70.12"
 pyyaml = "^6.0.1"
 validators = "^0.19.0"
 wrapt_timeout_decorator = "^1.3.12"
```

### Comparing `kintree-1.0.7/PKG-INFO` & `kintree-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kintree
-Version: 1.0.7
+Version: 1.1.0
 Summary: Fast part creation in KiCad and InvenTree
 Home-page: https://github.com/sparkmicro/Ki-nTree
 License: GPL-3.0-or-later
 Keywords: inventree,kicad,digikey,mouser,component,part,create
 Author: eeintech
 Author-email: eeintech@eeinte.ch
 Maintainer: eeintech
@@ -12,16 +12,16 @@
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: digikey-api (>=1.0.0,<2.0.0)
-Requires-Dist: flet (==0.7.4)
-Requires-Dist: inventree (>=0.12.1,<0.13.0)
+Requires-Dist: flet (>=0.22.0,<0.23.0)
+Requires-Dist: inventree (>=0.13.3,<0.14.0)
 Requires-Dist: kiutils (>=1.4.0,<2.0.0)
 Requires-Dist: mouser (>=0.1.3,<0.2.0)
 Requires-Dist: multiprocess (>=0.70.12,<0.71.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: thefuzz (>=0.19.0,<0.20.0)
 Requires-Dist: validators (>=0.19.0,<0.20.0)
 Requires-Dist: wrapt_timeout_decorator (>=1.3.12,<2.0.0)
@@ -187,14 +187,15 @@
 5. If you intend to use InvenTree with this tool, click on "Settings > InvenTree" and fill in your InvenTree server address and credentials then click "Save" (optional: click on "Test" to check communication with server)  
   a. It is possible to define a Proxy Server over which all interactions with InvenTree will be routed. To set a proxy server use the "Enable Proxy Support" switch in "Settings > InvenTree" and define the proxy address in the new input field.  
   b. Instead of user credential authentication token authentication is also supported. To use a token add it it to the "Password or Token" field and leave the "Username" empty. You can retrieve your personal access token from your InvenTree server by sending an get-request to its api url `api/user/token/`.
   c. If needed this tool can try to download the parts datasheet from the suppliers and upload it it to the attachment section of each part. For this just activate "Upload Datasheets to InvenTree" in the InvenTree settings
   d. It is also possible to sync the prices in InvenTree with the latest supplier prices. For this enable "Upload Pricing Data to InvenTree"
 6. If your InvenTree server requires a IPN in a specific pattern make sure to adjust "Settings > InvenTree > Internal Part Number" to match it or adjust the servers pattern to the one yo set in Ki-nTree 
 
+> Note: All URLs should start with "http://" if they do not have a valid SSL certificate.
 
 #### Get Digi-Key API token
 <details>
 <summary>Show steps (click to expand)</summary>
 <p>
 
 Enter your Digi-Key developer account credentials then login. The following page will appear (`user@email.com` will show your email address):
@@ -230,20 +231,22 @@
 
 Refer to [this file](https://github.com/sparkmicro/Ki-nTree/blob/main/kintree/config/inventree/supplier_parameters.yaml) as a starting point / example.
 
 #### Part Number Search
 
 Ki-nTree currently supports APIs for the following electronics suppliers: Digi-Key, Mouser, Element14, TME and LCSC.
 
-1. In the main window, enter the part number and select the supplier in drop-down list, then click "CREATE". It will start by fetching part data using the supplier's API
+1. In the main window, enter the part number and select the supplier in drop-down list, then click the "Submit" button (arrow). It will start by fetching part data using the supplier's API
 2. In the case Digi-Key has been selected and the API token is not found or expired, a browser window will pop-up. To get a new token: [follow those steps](#get-digi-key-api-token)
-3. Once the part data has been successfully fetched from the supplier's API, you will be prompted to add/confirm/edit the part information, followed by the `Category` and `Subcategory` to use for this part (Ki-nTree tries to match them automatically)
-4. Then, you will be prompted with selecting the KiCad symbol library, the template and the footprint library to use for this part
-5. It will take some time to complete the part creation in InvenTree and/or KiCad, once it finishes you'll be notified of the result  
-6. Finally, if the part was created or found in InvenTree, your browser will automatically open a new tab with the part information
+3. Once the part data has been successfully fetched from the supplier's API, you can review the part information in the different fields and edit them, if needed.
+4. Then, go to the Inventree tabl to pick the `Category` and `Subcategory` to use for this part
+5. If you desire to add this part to KiCad, click the KiCad tab and select the KiCad symbol library, the template and the footprint library to use for this part
+6. Finally, go to the Create tab and launch the part creation. It will take some time to complete the process in InvenTree and/or KiCad, once it finishes you'll be notified of the result  
+
+If the part was created or found in InvenTree, and if you have selected this option in the settings, your browser will automatically open and navigate to the new Inventree part page.
 
 #### Kicad Templates
 
 The automatic part generation in KiCad is controlled via templates:
 
 * Template examples are shipped together with Ki-nTree, these can be adjusted to your liking or you also can create completely new ones.
 * Each template has its own library file where the file name defines the templates name.
@@ -270,15 +273,15 @@
 ```
 
 2. Install the requirements into a `poetry`-managed virtual environment
 ``` bash
 poetry install
 Installing dependencies from lock file
 ...
-Installing the current project: kintree (1.0.99)
+Installing the current project: kintree (1.1.99)
 ```
 > Note: the version is not accurate (placeholder only)
 
 3. Run Ki-nTree in the virtual environment
 ```bash
 poetry run python -m kintree_gui
 ```
@@ -289,28 +292,28 @@
 $ python -m kintree_gui
 ```
 
 #### Build
 1. Make sure you followed the previous installation steps, then run:
 ``` bash
 $ poetry build
-Building kintree (1.0.99)
+Building kintree (1.1.99)
   - Building sdist
-  - Built kintree-1.0.99.tar.gz
+  - Built kintree-1.1.99.tar.gz
   - Building wheel
-  - Built kintree-1.0.99-py3-none-any.whl
+  - Built kintree-1.1.99-py3-none-any.whl
 ```
 2. Exit the virtual environment (`Ctrl + D` on Linux; you can also close the
    terminal and reopen it in the same folder).
 
    Run `pip install dist/<wheel_file>.whl` with the file name from the previous
    step. For example:
 
 ```bash
-pip install dist/kintree-1.0.99-py3-none-any.whl
+pip install dist/kintree-1.1.99-py3-none-any.whl
 ```
 
 3. You can now start Ki-nTree by typing `kintree` in the terminal, provided
    that your python dist path is a part of your `$PATH`.
 
 ## License
 The Ki-nTree source code is licensed under the [GPL3.0 license](https://github.com/sparkmicro/Ki-nTree/blob/main/LICENSE) as it uses source code under that license:
```

