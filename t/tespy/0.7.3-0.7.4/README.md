# Comparing `tmp/tespy-0.7.3.tar.gz` & `tmp/tespy-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tespy-0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tespy-0.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tespy-0.7.3.tar` & `tespy-0.7.4.tar`

### file list

```diff
@@ -1,343 +1,344 @@
--rw-r--r--   0        0        0      265 2021-10-04 06:28:48.000000 tespy-0.7.3/.editorconfig
--rw-r--r--   0        0        0     1446 2021-10-04 06:28:48.000000 tespy-0.7.3/.pep8speaks.yml
--rw-r--r--   0        0        0      341 2023-11-14 11:35:05.186734 tespy-0.7.3/.readthedocs.yml
--rw-r--r--   0        0        0     3269 2021-10-04 06:28:48.000000 tespy-0.7.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      154 2022-01-28 07:48:36.000000 tespy-0.7.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1088 2024-04-15 11:16:02.638416 tespy-0.7.3/LICENSE
--rw-r--r--   0        0        0      281 2023-11-14 11:35:05.190735 tespy-0.7.3/MANIFEST.in
--rw-r--r--   0        0        0      765 2021-10-04 06:28:48.000000 tespy-0.7.3/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     9116 2024-04-15 11:16:02.639417 tespy-0.7.3/README.rst
--rw-r--r--   0        0        0      180 2023-11-14 11:35:05.203247 tespy-0.7.3/docs/_static/css/custom.css
--rw-r--r--   0        0        0   129643 2023-11-14 11:35:05.207242 tespy-0.7.3/docs/_static/images/advanced/exergy/flowsheet.svg
--rw-r--r--   0        0        0   136810 2023-11-14 11:35:05.210242 tespy-0.7.3/docs/_static/images/advanced/exergy/flowsheet_darkmode.svg
--rw-r--r--   0        0        0    32134 2023-11-14 11:35:05.212242 tespy-0.7.3/docs/_static/images/advanced/exergy/sankey.svg
--rw-r--r--   0        0        0    17276 2023-11-14 11:35:05.213286 tespy-0.7.3/docs/_static/images/basics/district_heating.svg
--rw-r--r--   0        0        0    18111 2023-11-14 11:35:05.215279 tespy-0.7.3/docs/_static/images/basics/district_heating_darkmode.svg
--rw-r--r--   0        0        0    69064 2023-11-14 11:35:05.218243 tespy-0.7.3/docs/_static/images/basics/district_heating_partload.svg
--rw-r--r--   0        0        0    71199 2023-11-14 11:35:05.220243 tespy-0.7.3/docs/_static/images/basics/district_heating_partload_darkmode.svg
--rw-r--r--   0        0        0    15810 2023-11-14 11:35:05.222242 tespy-0.7.3/docs/_static/images/basics/gas_turbine.svg
--rw-r--r--   0        0        0    16340 2023-11-14 11:35:05.223244 tespy-0.7.3/docs/_static/images/basics/gas_turbine_darkmode.svg
--rw-r--r--   0        0        0    32095 2023-11-14 11:35:05.225250 tespy-0.7.3/docs/_static/images/basics/gas_turbine_fuel_composition.svg
--rw-r--r--   0        0        0    32756 2023-11-14 11:35:05.227255 tespy-0.7.3/docs/_static/images/basics/gas_turbine_fuel_composition_darkmode.svg
--rw-r--r--   0        0        0    29612 2023-11-14 11:35:05.228284 tespy-0.7.3/docs/_static/images/basics/gas_turbine_oxygen.svg
--rw-r--r--   0        0        0    30202 2023-11-14 11:35:05.230296 tespy-0.7.3/docs/_static/images/basics/gas_turbine_oxygen_darkmode.svg
--rw-r--r--   0        0        0    57559 2023-11-14 11:35:05.231295 tespy-0.7.3/docs/_static/images/basics/gas_turbine_parametric.svg
--rw-r--r--   0        0        0    59255 2023-11-14 11:35:05.233242 tespy-0.7.3/docs/_static/images/basics/gas_turbine_parametric_darkmode.svg
--rw-r--r--   0        0        0    14362 2023-11-14 11:35:05.234243 tespy-0.7.3/docs/_static/images/basics/heat_pump.svg
--rw-r--r--   0        0        0    14866 2023-11-14 11:35:05.236243 tespy-0.7.3/docs/_static/images/basics/heat_pump_darkmode.svg
--rw-r--r--   0        0        0    53423 2023-11-14 11:35:05.237245 tespy-0.7.3/docs/_static/images/basics/heat_pump_parametric.svg
--rw-r--r--   0        0        0    54994 2023-11-14 11:35:05.240244 tespy-0.7.3/docs/_static/images/basics/heat_pump_parametric_darkmode.svg
--rw-r--r--   0        0        0    16030 2023-11-14 11:35:05.241287 tespy-0.7.3/docs/_static/images/basics/modeling_concept.svg
--rw-r--r--   0        0        0    16137 2023-11-14 11:35:05.242303 tespy-0.7.3/docs/_static/images/basics/rankine_cycle.svg
--rw-r--r--   0        0        0    16871 2023-11-14 11:35:05.243245 tespy-0.7.3/docs/_static/images/basics/rankine_cycle_darkmode.svg
--rw-r--r--   0        0        0    59916 2023-11-14 11:35:05.245276 tespy-0.7.3/docs/_static/images/basics/rankine_parametric.svg
--rw-r--r--   0        0        0    61115 2023-11-14 11:35:05.247242 tespy-0.7.3/docs/_static/images/basics/rankine_parametric_darkmode.svg
--rw-r--r--   0        0        0    26962 2023-11-14 11:35:05.248242 tespy-0.7.3/docs/_static/images/basics/rankine_partload.svg
--rw-r--r--   0        0        0    27517 2023-11-14 11:35:05.250241 tespy-0.7.3/docs/_static/images/basics/rankine_partload_darkmode.svg
--rw-r--r--   0        0        0   139795 2023-11-14 11:35:05.254645 tespy-0.7.3/docs/_static/images/examples/GRC_flowsheet.svg
--rw-r--r--   0        0        0   157545 2023-11-14 11:35:05.259751 tespy-0.7.3/docs/_static/images/examples/GRC_flowsheet_darkmode.svg
--rw-r--r--   0        0        0    88269 2023-11-14 11:35:05.262970 tespy-0.7.3/docs/_static/images/examples/ORC_parametric_flowsheet.svg
--rw-r--r--   0        0        0    88176 2023-11-14 11:35:05.266014 tespy-0.7.3/docs/_static/images/examples/ORC_parametric_flowsheet_darkmode.svg
--rw-r--r--   0        0        0   409001 2023-11-14 11:35:05.275027 tespy-0.7.3/docs/_static/images/examples/PM_CAES_graphical-abstract.svg
--rw-r--r--   0        0        0   417664 2023-11-14 11:35:05.283696 tespy-0.7.3/docs/_static/images/examples/PM_CAES_graphical-abstract_darkmode.svg
--rw-r--r--   0        0        0    39020 2023-11-14 11:35:05.284697 tespy-0.7.3/docs/_static/images/logo_tespy_big.svg
--rw-r--r--   0        0        0    39647 2023-11-14 11:35:05.285746 tespy-0.7.3/docs/_static/images/logo_tespy_big_darkmode.svg
--rw-r--r--   0        0        0    17145 2023-11-14 11:35:05.287696 tespy-0.7.3/docs/_static/images/logo_tespy_big_editable_font.svg
--rw-r--r--   0        0        0    23121 2024-04-15 08:10:01.844502 tespy-0.7.3/docs/_static/images/logo_tespy_mid.svg
--rw-r--r--   0        0        0    24693 2024-04-15 11:16:02.639417 tespy-0.7.3/docs/_static/images/logo_tespy_mid_christmas.svg
--rw-r--r--   0        0        0    23260 2023-11-14 11:35:05.289734 tespy-0.7.3/docs/_static/images/logo_tespy_mid_darkmode.svg
--rw-r--r--   0        0        0    24872 2024-04-15 11:16:02.640417 tespy-0.7.3/docs/_static/images/logo_tespy_mid_darkmode_christmas.svg
--rw-r--r--   0        0        0    15239 2023-11-14 11:35:05.290696 tespy-0.7.3/docs/_static/images/logo_tespy_mid_editable_font.svg
--rw-r--r--   0        0        0    13985 2023-11-27 18:42:13.344791 tespy-0.7.3/docs/_static/images/logo_tespy_mini.svg
--rw-r--r--   0        0        0    13302 2023-11-14 11:35:05.293737 tespy-0.7.3/docs/_static/images/logo_tespy_small.svg
--rw-r--r--   0        0        0   157002 2023-11-14 11:35:05.299887 tespy-0.7.3/docs/_static/images/modules/Ts_diagram_states.svg
--rw-r--r--   0        0        0     8644 2023-11-14 11:35:05.301873 tespy-0.7.3/docs/_static/images/modules/characteristics.svg
--rw-r--r--   0        0        0     8414 2023-11-14 11:35:05.302847 tespy-0.7.3/docs/_static/images/modules/characteristics_darkmode.svg
--rw-r--r--   0        0        0    11300 2023-11-14 11:35:05.304847 tespy-0.7.3/docs/_static/images/modules/connections.svg
--rw-r--r--   0        0        0    11315 2023-11-14 11:35:05.305848 tespy-0.7.3/docs/_static/images/modules/connections_darkmode.svg
--rw-r--r--   0        0        0   134345 2023-11-14 11:35:05.308847 tespy-0.7.3/docs/_static/images/modules/fluid_properties.svg
--rw-r--r--   0        0        0   125300 2023-11-14 11:35:05.310847 tespy-0.7.3/docs/_static/images/modules/fluid_properties_darkmode.svg
--rw-r--r--   0        0        0   168665 2023-11-14 11:35:05.315851 tespy-0.7.3/docs/_static/images/modules/logph_diagram_states.svg
--rw-r--r--   0        0        0    17587 2023-11-14 11:35:05.317845 tespy-0.7.3/docs/_static/images/modules/subsystem_waste_heat_generator.svg
--rw-r--r--   0        0        0    17663 2023-11-14 11:35:05.320845 tespy-0.7.3/docs/_static/images/modules/subsystem_waste_heat_generator_darkmode.svg
--rw-r--r--   0        0        0   121692 2023-11-14 11:35:05.322846 tespy-0.7.3/docs/_static/images/modules/ude.svg
--rw-r--r--   0        0        0   125035 2023-11-14 11:35:05.324845 tespy-0.7.3/docs/_static/images/modules/ude_darkmode.svg
--rw-r--r--   0        0        0    33944 2023-11-14 11:35:05.327439 tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs.svg
--rw-r--r--   0        0        0    20206 2023-11-14 11:35:05.329488 tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_closed.svg
--rw-r--r--   0        0        0    12074 2023-11-14 11:35:05.331495 tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_forks.svg
--rw-r--r--   0        0        0    21711 2023-11-14 11:35:05.333492 tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_open.svg
--rw-r--r--   0        0        0   168149 2023-11-14 11:35:05.337492 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/NH3_logph.svg
--rw-r--r--   0        0        0    23347 2023-11-14 11:35:05.338492 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/NH3_sankey.svg
--rw-r--r--   0        0        0    60290 2023-11-14 11:35:05.339484 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D.svg
--rw-r--r--   0        0        0    61853 2023-11-14 11:35:05.340503 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D_darkmode.svg
--rw-r--r--   0        0        0    61177 2023-11-14 11:35:05.342490 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q.svg
--rw-r--r--   0        0        0    62156 2023-11-14 11:35:05.342490 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q_darkmode.svg
--rw-r--r--   0        0        0    66033 2023-11-14 11:35:05.344487 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths.svg
--rw-r--r--   0        0        0    67428 2023-11-14 11:35:05.345486 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths_darkmode.svg
--rw-r--r--   0        0        0    52499 2023-11-14 11:35:05.346490 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo.svg
--rw-r--r--   0        0        0    53372 2023-11-14 11:35:05.347488 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo_darkmode.svg
--rw-r--r--   0        0        0    29826 2023-11-14 11:35:05.348490 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/flowsheet.svg
--rw-r--r--   0        0        0    29835 2023-11-14 11:35:05.349496 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/flowsheet_darkmode.svg
--rw-r--r--   0        0        0    27850 2023-11-14 11:35:05.350453 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf.svg
--rw-r--r--   0        0        0    28404 2023-11-14 11:35:05.351485 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf_darkmode.svg
--rw-r--r--   0        0        0    30290 2023-11-14 11:35:05.352501 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet.svg
--rw-r--r--   0        0        0    30299 2023-11-14 11:35:05.353493 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet_darkmode.svg
--rw-r--r--   0        0        0   227184 2023-11-14 11:35:05.356486 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/logph.svg
--rw-r--r--   0        0        0    46257 2023-11-14 11:35:05.357488 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet.svg
--rw-r--r--   0        0        0    46240 2023-11-14 11:35:05.358489 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_darkmode.svg
--rw-r--r--   0        0        0    46286 2023-11-14 11:35:05.359486 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1.svg
--rw-r--r--   0        0        0    46277 2023-11-14 11:35:05.360489 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1_darkmode.svg
--rw-r--r--   0        0        0    46669 2023-11-14 11:35:05.361488 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2.svg
--rw-r--r--   0        0        0    46657 2023-11-14 11:35:05.362482 tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2_darkmode.svg
--rw-r--r--   0        0        0    52832 2023-11-14 11:35:05.364488 tespy-0.7.3/docs/_static/images/tutorials/osmses-2023.svg
--rw-r--r--   0        0        0    53182 2023-11-14 11:35:05.366491 tespy-0.7.3/docs/_static/images/tutorials/osmses-2023_darkmode.svg
--rw-r--r--   0        0        0    33530 2023-11-14 11:35:05.368487 tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/flowsheet.svg
--rw-r--r--   0        0        0    34684 2023-11-14 11:35:05.369487 tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/flowsheet_darkmode.svg
--rw-r--r--   0        0        0   190475 2023-11-14 11:35:05.371488 tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization.svg
--rw-r--r--   0        0        0   192983 2023-11-14 11:35:05.372490 tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization_darkmode.svg
--rw-r--r--   0        0        0      578 2024-02-08 10:33:11.103316 tespy-0.7.3/docs/_static/js/custom.js
--rw-r--r--   0        0        0        0 2023-11-14 11:35:05.375500 tespy-0.7.3/docs/_templates/index.html
--rw-r--r--   0        0        0    20686 2023-11-27 18:42:13.344791 tespy-0.7.3/docs/advanced/exergy.rst
--rw-r--r--   0        0        0       92 2023-11-14 11:35:05.377489 tespy-0.7.3/docs/advanced/optimization.rst
--rw-r--r--   0        0        0      532 2023-11-27 18:42:13.352886 tespy-0.7.3/docs/api.rst
--rw-r--r--   0        0        0     9313 2023-11-14 11:35:05.380489 tespy-0.7.3/docs/api/_images/CombustionChamber.svg
--rw-r--r--   0        0        0     9682 2023-11-14 11:35:05.380489 tespy-0.7.3/docs/api/_images/CombustionChamber_darkmode.svg
--rw-r--r--   0        0        0    15877 2023-11-14 11:35:05.382455 tespy-0.7.3/docs/api/_images/CombustionEngine.svg
--rw-r--r--   0        0        0    16472 2023-11-14 11:35:05.383486 tespy-0.7.3/docs/api/_images/CombustionEngine_darkmode.svg
--rw-r--r--   0        0        0     7484 2023-11-14 11:35:05.384453 tespy-0.7.3/docs/api/_images/Compressor.svg
--rw-r--r--   0        0        0     7661 2023-11-14 11:35:05.384453 tespy-0.7.3/docs/api/_images/Compressor_darkmode.svg
--rw-r--r--   0        0        0     9565 2023-11-14 11:35:05.385452 tespy-0.7.3/docs/api/_images/Condenser.svg
--rw-r--r--   0        0        0    10115 2023-11-14 11:35:05.386452 tespy-0.7.3/docs/api/_images/Condenser_darkmode.svg
--rw-r--r--   0        0        0     8889 2024-04-15 11:16:02.640417 tespy-0.7.3/docs/api/_images/DropletSeparator.svg
--rw-r--r--   0        0        0     9030 2024-04-15 11:16:02.641417 tespy-0.7.3/docs/api/_images/DropletSeparator_darkmode.svg
--rw-r--r--   0        0        0    10414 2023-11-14 11:35:05.389475 tespy-0.7.3/docs/api/_images/Drum.svg
--rw-r--r--   0        0        0    10583 2023-11-14 11:35:05.389475 tespy-0.7.3/docs/api/_images/Drum_darkmode.svg
--rw-r--r--   0        0        0    15148 2023-11-14 11:35:05.390494 tespy-0.7.3/docs/api/_images/FuelCell.svg
--rw-r--r--   0        0        0    15153 2023-11-14 11:35:05.391488 tespy-0.7.3/docs/api/_images/FuelCell_darkmode.svg
--rw-r--r--   0        0        0    10283 2023-11-14 11:35:05.392501 tespy-0.7.3/docs/api/_images/HeatExchanger.svg
--rw-r--r--   0        0        0    10403 2023-11-14 11:35:05.393481 tespy-0.7.3/docs/api/_images/HeatExchanger_darkmode.svg
--rw-r--r--   0        0        0    12851 2023-11-14 11:35:05.394490 tespy-0.7.3/docs/api/_images/Merge.svg
--rw-r--r--   0        0        0    13017 2023-11-14 11:35:05.394490 tespy-0.7.3/docs/api/_images/Merge_darkmode.svg
--rw-r--r--   0        0        0     8013 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/ORCEvaporator.svg
--rw-r--r--   0        0        0     7643 2023-11-14 11:35:05.396453 tespy-0.7.3/docs/api/_images/ParabolicTrough.svg
--rw-r--r--   0        0        0     7823 2023-11-14 11:35:05.396453 tespy-0.7.3/docs/api/_images/ParabolicTrough_darkmode.svg
--rw-r--r--   0        0        0     6462 2023-11-14 11:35:05.398490 tespy-0.7.3/docs/api/_images/Pipe.svg
--rw-r--r--   0        0        0     6640 2023-11-14 11:35:05.399484 tespy-0.7.3/docs/api/_images/Pipe_darkmode.svg
--rw-r--r--   0        0        0     7414 2023-11-14 11:35:05.400485 tespy-0.7.3/docs/api/_images/Pump.svg
--rw-r--r--   0        0        0     7478 2023-11-14 11:35:05.400485 tespy-0.7.3/docs/api/_images/Pump_darkmode.svg
--rw-r--r--   0        0        0     6810 2023-11-14 11:35:05.401451 tespy-0.7.3/docs/api/_images/SolarCollector.svg
--rw-r--r--   0        0        0     6875 2023-11-14 11:35:05.402487 tespy-0.7.3/docs/api/_images/SolarCollector_darkmode.svg
--rw-r--r--   0        0        0    12813 2023-11-14 11:35:05.403490 tespy-0.7.3/docs/api/_images/Splitter.svg
--rw-r--r--   0        0        0    12979 2023-11-14 11:35:05.404518 tespy-0.7.3/docs/api/_images/Splitter_darkmode.svg
--rw-r--r--   0        0        0    12381 2023-11-14 11:35:05.405488 tespy-0.7.3/docs/api/_images/SubsystemInterface.svg
--rw-r--r--   0        0        0    12558 2023-11-14 11:35:05.405488 tespy-0.7.3/docs/api/_images/SubsystemInterface_darkmode.svg
--rw-r--r--   0        0        0     6668 2023-11-14 11:35:05.406452 tespy-0.7.3/docs/api/_images/Turbine.svg
--rw-r--r--   0        0        0     6677 2023-11-14 11:35:05.407500 tespy-0.7.3/docs/api/_images/Turbine_darkmode.svg
--rw-r--r--   0        0        0     6491 2023-11-14 11:35:05.408451 tespy-0.7.3/docs/api/_images/Valve.svg
--rw-r--r--   0        0        0     6668 2023-11-14 11:35:05.409492 tespy-0.7.3/docs/api/_images/Valve_darkmode.svg
--rw-r--r--   0        0        0    13372 2023-11-14 11:35:05.410490 tespy-0.7.3/docs/api/_images/WaterElectrolyzer.svg
--rw-r--r--   0        0        0    15165 2023-11-14 11:35:05.410490 tespy-0.7.3/docs/api/_images/WaterElectrolyzer_darkmode.svg
--rw-r--r--   0        0        0    40711 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/combustion_engine_Q1_char_DEFAULT.svg
--rw-r--r--   0        0        0    40966 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/combustion_engine_Q2_char_DEFAULT.svg
--rw-r--r--   0        0        0    38781 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/combustion_engine_Qloss_char_DEFAULT.svg
--rw-r--r--   0        0        0    37655 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/combustion_engine_tiP_char_DEFAULT.svg
--rw-r--r--   0        0        0    49048 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/compressor_char_map_eta_s_DEFAULT.svg
--rw-r--r--   0        0        0    46950 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/compressor_char_map_pr_DEFAULT.svg
--rw-r--r--   0        0        0    39251 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/compressor_eta_s_char_DEFAULT.svg
--rw-r--r--   0        0        0    40197 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/condenser_kA_char1_DEFAULT.svg
--rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/condenser_kA_char2_DEFAULT.svg
--rw-r--r--   0        0        0    42372 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/desuperheater_kA_char1_DEFAULT.svg
--rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/desuperheater_kA_char2_DEFAULT.svg
--rw-r--r--   0        0        0    43523 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char1_CONDENSING_FLUID.svg
--rw-r--r--   0        0        0    42372 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char1_DEFAULT.svg
--rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char2_DEFAULT.svg
--rw-r--r--   0        0        0    45010 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char2_EVAPORATING_FLUID.svg
--rw-r--r--   0        0        0    42314 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/heat_exchanger_simple_kA_char_DEFAULT.svg
--rw-r--r--   0        0        0    42314 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/pipe_kA_char_DEFAULT.svg
--rw-r--r--   0        0        0    40653 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/pump_eta_s_char_DEFAULT.svg
--rw-r--r--   0        0        0    39798 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/turbine_eta_s_char_DEFAULT.svg
--rw-r--r--   0        0        0    40222 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/turbine_eta_s_char_TRAUPEL.svg
--rw-r--r--   0        0        0    36210 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/api/_images/water_electrolyzer_eta_char_DEFAULT.svg
--rw-r--r--   0        0        0     6139 2024-04-15 11:16:02.648090 tespy-0.7.3/docs/api/components.rst
--rw-r--r--   0        0        0      496 2023-11-14 11:35:05.412490 tespy-0.7.3/docs/api/connections.rst
--rw-r--r--   0        0        0     4204 2023-11-14 11:35:05.414490 tespy-0.7.3/docs/api/data.rst
--rw-r--r--   0        0        0      493 2023-11-14 11:35:05.415452 tespy-0.7.3/docs/api/networks.rst
--rw-r--r--   0        0        0     2161 2024-04-15 11:16:02.649119 tespy-0.7.3/docs/api/tools.rst
--rw-r--r--   0        0        0     2463 2023-11-14 11:35:05.417470 tespy-0.7.3/docs/basics.rst
--rw-r--r--   0        0        0     5528 2024-04-15 11:16:02.649119 tespy-0.7.3/docs/basics/district_heating.rst
--rw-r--r--   0        0        0    10772 2024-04-15 11:16:02.650113 tespy-0.7.3/docs/basics/gas_turbine.rst
--rw-r--r--   0        0        0     6691 2023-11-27 18:42:13.352886 tespy-0.7.3/docs/basics/heat_pump.rst
--rw-r--r--   0        0        0     7125 2024-04-15 11:16:02.650113 tespy-0.7.3/docs/basics/intro.rst
--rw-r--r--   0        0        0    10668 2024-04-15 11:16:02.652129 tespy-0.7.3/docs/basics/rankine_cycle.rst
--rw-r--r--   0        0        0     2743 2024-04-15 11:16:02.653137 tespy-0.7.3/docs/benchmarks.rst
--rw-r--r--   0        0        0     4695 2024-04-15 11:16:02.653137 tespy-0.7.3/docs/conf.py
--rw-r--r--   0        0        0     7315 2023-11-27 18:42:13.352886 tespy-0.7.3/docs/development/how.rst
--rw-r--r--   0        0        0     3192 2024-04-15 11:16:02.654136 tespy-0.7.3/docs/development/what.rst
--rw-r--r--   0        0        0     4319 2023-11-27 18:42:13.352886 tespy-0.7.3/docs/examples.rst
--rw-r--r--   0        0        0      661 2023-11-14 11:35:05.429456 tespy-0.7.3/docs/index.rst
--rw-r--r--   0        0        0     2890 2023-11-14 11:35:05.431452 tespy-0.7.3/docs/installation.rst
--rw-r--r--   0        0        0     3853 2023-11-27 18:42:13.352886 tespy-0.7.3/docs/introduction.rst
--rw-r--r--   0        0        0     2398 2023-11-14 11:35:05.433499 tespy-0.7.3/docs/modules.rst
--rw-r--r--   0        0        0     5082 2023-11-27 18:42:13.368512 tespy-0.7.3/docs/modules/characteristics.rst
--rw-r--r--   0        0        0    34468 2024-04-15 11:16:02.655136 tespy-0.7.3/docs/modules/components.rst
--rw-r--r--   0        0        0    15728 2024-04-15 11:16:02.655136 tespy-0.7.3/docs/modules/connections.rst
--rw-r--r--   0        0        0    15251 2024-04-15 11:16:02.656135 tespy-0.7.3/docs/modules/fluid_properties.rst
--rw-r--r--   0        0        0    32940 2024-04-15 11:16:02.657137 tespy-0.7.3/docs/modules/networks.rst
--rw-r--r--   0        0        0    12661 2024-04-15 17:02:58.316540 tespy-0.7.3/docs/modules/ude.rst
--rw-r--r--   0        0        0    12186 2024-04-15 11:16:02.658135 tespy-0.7.3/docs/references.bib
--rw-r--r--   0        0        0      886 2023-11-14 11:35:05.443458 tespy-0.7.3/docs/regular_meeting.rst
--rw-r--r--   0        0        0       77 2024-02-08 10:33:11.165315 tespy-0.7.3/docs/requirements.txt
--rw-r--r--   0        0        0     2914 2023-11-14 11:35:05.445457 tespy-0.7.3/docs/scripts/generate_tespy_data_module.py
--rw-r--r--   0        0        0     3594 2023-11-27 18:42:13.369520 tespy-0.7.3/docs/tutorials.rst
--rw-r--r--   0        0        0     2365 2023-11-27 18:42:13.369520 tespy-0.7.3/docs/tutorials/district_heating.rst
--rw-r--r--   0        0        0    32094 2024-04-15 11:16:02.659136 tespy-0.7.3/docs/tutorials/heat_pump_exergy.rst
--rw-r--r--   0        0        0    21439 2024-04-15 11:16:02.660136 tespy-0.7.3/docs/tutorials/heat_pump_steps.rst
--rw-r--r--   0        0        0     7904 2023-11-27 18:42:13.369520 tespy-0.7.3/docs/tutorials/pygmo_optimization.rst
--rw-r--r--   0        0        0     8543 2023-11-27 18:42:13.369520 tespy-0.7.3/docs/tutorials/starting_values.rst
--rw-r--r--   0        0        0     1360 2024-04-15 17:02:58.316540 tespy-0.7.3/docs/whats_new.rst
--rw-r--r--   0        0        0      240 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-0-1.rst
--rw-r--r--   0        0        0     1548 2023-11-14 11:35:05.456506 tespy-0.7.3/docs/whats_new/v0-0-2.rst
--rw-r--r--   0        0        0     4807 2023-11-14 11:35:05.457491 tespy-0.7.3/docs/whats_new/v0-0-3.rst
--rw-r--r--   0        0        0     1994 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-0-4.rst
--rw-r--r--   0        0        0     3293 2023-07-20 10:11:41.150532 tespy-0.7.3/docs/whats_new/v0-0-5.rst
--rw-r--r--   0        0        0     3987 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-1-0.rst
--rw-r--r--   0        0        0     4347 2023-11-14 11:35:05.459497 tespy-0.7.3/docs/whats_new/v0-1-1.rst
--rw-r--r--   0        0        0     3842 2023-11-14 11:35:05.460492 tespy-0.7.3/docs/whats_new/v0-1-2.rst
--rw-r--r--   0        0        0     2675 2023-11-14 11:35:05.462483 tespy-0.7.3/docs/whats_new/v0-1-3.rst
--rw-r--r--   0        0        0      616 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-1-4.rst
--rw-r--r--   0        0        0     8338 2023-11-14 11:35:05.463455 tespy-0.7.3/docs/whats_new/v0-2-0.rst
--rw-r--r--   0        0        0     1982 2022-05-26 10:30:52.000000 tespy-0.7.3/docs/whats_new/v0-2-1.rst
--rw-r--r--   0        0        0     3064 2023-11-14 11:35:05.465487 tespy-0.7.3/docs/whats_new/v0-2-2.rst
--rw-r--r--   0        0        0    11252 2023-11-14 11:35:05.466489 tespy-0.7.3/docs/whats_new/v0-3-0.rst
--rw-r--r--   0        0        0      314 2022-05-26 10:30:52.000000 tespy-0.7.3/docs/whats_new/v0-3-1.rst
--rw-r--r--   0        0        0     2062 2023-07-20 10:11:41.153549 tespy-0.7.3/docs/whats_new/v0-3-2.rst
--rw-r--r--   0        0        0     1345 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-3-3.rst
--rw-r--r--   0        0        0     1471 2023-11-14 11:35:05.467454 tespy-0.7.3/docs/whats_new/v0-3-4.rst
--rw-r--r--   0        0        0    11174 2023-11-14 11:35:05.468458 tespy-0.7.3/docs/whats_new/v0-4-0.rst
--rw-r--r--   0        0        0     1126 2023-11-14 11:35:05.469487 tespy-0.7.3/docs/whats_new/v0-4-1.rst
--rw-r--r--   0        0        0     1589 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-4-2.rst
--rw-r--r--   0        0        0      563 2021-10-04 06:28:48.000000 tespy-0.7.3/docs/whats_new/v0-4-3-001.rst
--rw-r--r--   0        0        0      656 2023-11-14 11:35:05.470480 tespy-0.7.3/docs/whats_new/v0-4-3-003.rst
--rw-r--r--   0        0        0     3355 2023-11-14 11:35:05.471499 tespy-0.7.3/docs/whats_new/v0-4-3.rst
--rw-r--r--   0        0        0     1183 2022-01-28 07:48:36.000000 tespy-0.7.3/docs/whats_new/v0-4-4.rst
--rw-r--r--   0        0        0      801 2022-01-28 07:48:36.000000 tespy-0.7.3/docs/whats_new/v0-5-0.rst
--rw-r--r--   0        0        0      930 2022-05-26 10:30:52.000000 tespy-0.7.3/docs/whats_new/v0-5-1.rst
--rw-r--r--   0        0        0     2644 2023-11-14 11:35:05.473451 tespy-0.7.3/docs/whats_new/v0-6-0.rst
--rw-r--r--   0        0        0     2064 2023-11-14 11:35:05.474453 tespy-0.7.3/docs/whats_new/v0-6-1.rst
--rw-r--r--   0        0        0      385 2023-11-14 11:35:05.475486 tespy-0.7.3/docs/whats_new/v0-6-2.rst
--rw-r--r--   0        0        0     2841 2023-11-14 11:35:05.476510 tespy-0.7.3/docs/whats_new/v0-6-3.rst
--rw-r--r--   0        0        0     4014 2024-04-15 11:16:02.661136 tespy-0.7.3/docs/whats_new/v0-7-0.rst
--rw-r--r--   0        0        0      427 2024-04-15 11:16:02.661136 tespy-0.7.3/docs/whats_new/v0-7-1.rst
--rw-r--r--   0        0        0      841 2024-04-15 11:16:02.662135 tespy-0.7.3/docs/whats_new/v0-7-2.rst
--rw-r--r--   0        0        0      363 2024-04-15 17:01:52.744160 tespy-0.7.3/docs/whats_new/v0-7-3.rst
--rw-r--r--   0        0        0       90 2023-11-14 11:35:05.478498 tespy-0.7.3/docs/zliterature.rst
--rw-r--r--   0        0        0     6582 2023-11-14 11:35:05.480483 tespy-0.7.3/paper.bib
--rw-r--r--   0        0        0    11023 2021-10-04 06:28:48.000000 tespy-0.7.3/paper.md
--rw-r--r--   0        0        0     2607 2024-04-15 17:02:58.327058 tespy-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     1187 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/__init__.py
--rw-r--r--   0        0        0     1655 2024-04-15 11:16:02.664135 tespy-0.7.3/src/tespy/components/__init__.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/basics/__init__.py
--rw-r--r--   0        0        0     5537 2024-02-20 16:14:00.450472 tespy-0.7.3/src/tespy/components/basics/cycle_closer.py
--rw-r--r--   0        0        0     2695 2024-02-08 10:33:11.197316 tespy-0.7.3/src/tespy/components/basics/sink.py
--rw-r--r--   0        0        0     3223 2024-02-20 16:14:00.450472 tespy-0.7.3/src/tespy/components/basics/source.py
--rw-r--r--   0        0        0     5247 2024-02-08 10:33:11.202317 tespy-0.7.3/src/tespy/components/basics/subsystem_interface.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/combustion/__init__.py
--rw-r--r--   0        0        0    47281 2024-04-15 11:16:02.664135 tespy-0.7.3/src/tespy/components/combustion/base.py
--rw-r--r--   0        0        0    13831 2024-02-08 10:33:11.210315 tespy-0.7.3/src/tespy/components/combustion/diabatic.py
--rw-r--r--   0        0        0    55747 2024-04-15 11:16:02.665135 tespy-0.7.3/src/tespy/components/combustion/engine.py
--rw-r--r--   0        0        0    41460 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/components/component.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/customs/__init__.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/heat_exchangers/__init__.py
--rw-r--r--   0        0        0    38259 2024-04-15 11:16:02.666134 tespy-0.7.3/src/tespy/components/heat_exchangers/base.py
--rw-r--r--   0        0        0    18098 2024-04-15 11:16:02.667135 tespy-0.7.3/src/tespy/components/heat_exchangers/condenser.py
--rw-r--r--   0        0        0     8531 2024-04-15 11:16:02.667135 tespy-0.7.3/src/tespy/components/heat_exchangers/desuperheater.py
--rw-r--r--   0        0        0    13129 2024-04-15 11:16:02.667135 tespy-0.7.3/src/tespy/components/heat_exchangers/parabolic_trough.py
--rw-r--r--   0        0        0    43440 2024-04-15 11:16:02.668135 tespy-0.7.3/src/tespy/components/heat_exchangers/simple.py
--rw-r--r--   0        0        0    11356 2024-04-15 11:16:02.668135 tespy-0.7.3/src/tespy/components/heat_exchangers/solar_collector.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/nodes/__init__.py
--rw-r--r--   0        0        0     6116 2024-04-15 11:16:02.669134 tespy-0.7.3/src/tespy/components/nodes/base.py
--rw-r--r--   0        0        0    13308 2024-02-15 15:31:08.395117 tespy-0.7.3/src/tespy/components/nodes/droplet_separator.py
--rw-r--r--   0        0        0    14951 2024-04-15 11:16:02.670135 tespy-0.7.3/src/tespy/components/nodes/drum.py
--rw-r--r--   0        0        0    17177 2024-04-15 11:16:02.670135 tespy-0.7.3/src/tespy/components/nodes/merge.py
--rw-r--r--   0        0        0    11927 2024-04-15 11:16:02.670135 tespy-0.7.3/src/tespy/components/nodes/separator.py
--rw-r--r--   0        0        0     6693 2024-02-15 15:31:08.395117 tespy-0.7.3/src/tespy/components/nodes/splitter.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/piping/__init__.py
--rw-r--r--   0        0        0     5352 2024-02-08 10:33:11.253315 tespy-0.7.3/src/tespy/components/piping/pipe.py
--rw-r--r--   0        0        0    13658 2024-04-15 11:16:02.671136 tespy-0.7.3/src/tespy/components/piping/valve.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/reactors/__init__.py
--rw-r--r--   0        0        0    27777 2024-04-15 11:16:02.671136 tespy-0.7.3/src/tespy/components/reactors/fuel_cell.py
--rw-r--r--   0        0        0    40264 2024-04-15 11:16:02.672134 tespy-0.7.3/src/tespy/components/reactors/water_electrolyzer.py
--rw-r--r--   0        0        0     2343 2024-04-15 11:16:02.673153 tespy-0.7.3/src/tespy/components/subsystem.py
--rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/components/turbomachinery/__init__.py
--rw-r--r--   0        0        0     8475 2024-04-15 11:16:02.674135 tespy-0.7.3/src/tespy/components/turbomachinery/base.py
--rw-r--r--   0        0        0    25801 2024-04-15 11:16:02.674135 tespy-0.7.3/src/tespy/components/turbomachinery/compressor.py
--rw-r--r--   0        0        0    19150 2024-02-20 16:14:00.485473 tespy-0.7.3/src/tespy/components/turbomachinery/pump.py
--rw-r--r--   0        0        0    19110 2024-02-15 15:31:08.411864 tespy-0.7.3/src/tespy/components/turbomachinery/turbine.py
--rw-r--r--   0        0        0      147 2022-01-28 07:48:36.000000 tespy-0.7.3/src/tespy/connections/__init__.py
--rw-r--r--   0        0        0    16918 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/connections/bus.py
--rw-r--r--   0        0        0    44576 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/connections/connection.py
--rw-r--r--   0        0        0     9270 2023-11-14 11:35:05.528493 tespy-0.7.3/src/tespy/data/ChemEx/Ahrendts.json
--rw-r--r--   0        0        0     8407 2023-11-14 11:35:05.530494 tespy-0.7.3/src/tespy/data/ChemEx/Szargut1988.json
--rw-r--r--   0        0        0     8578 2023-11-14 11:35:05.532488 tespy-0.7.3/src/tespy/data/ChemEx/Szargut2007.json
--rw-r--r--   0        0        0     8047 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/data/char_lines.json
--rw-r--r--   0        0        0     3726 2021-10-04 06:28:48.000000 tespy-0.7.3/src/tespy/data/char_maps.json
--rw-r--r--   0        0        0      118 2022-01-28 07:48:36.000000 tespy-0.7.3/src/tespy/networks/__init__.py
--rw-r--r--   0        0        0   107289 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/networks/network.py
--rw-r--r--   0        0        0    15070 2024-04-15 11:16:02.676160 tespy-0.7.3/src/tespy/networks/network_reader.py
--rw-r--r--   0        0        0      940 2024-04-15 17:02:58.327058 tespy-0.7.3/src/tespy/tools/__init__.py
--rw-r--r--   0        0        0    38453 2024-04-15 11:16:02.677134 tespy-0.7.3/src/tespy/tools/analyses.py
--rw-r--r--   0        0        0    17458 2024-04-15 17:02:58.342708 tespy-0.7.3/src/tespy/tools/characteristics.py
--rw-r--r--   0        0        0    17346 2024-04-15 17:02:58.342708 tespy-0.7.3/src/tespy/tools/data_containers.py
--rw-r--r--   0        0        0    38786 2024-02-08 10:33:11.297315 tespy-0.7.3/src/tespy/tools/document_models.py
--rw-r--r--   0        0        0     1046 2024-04-15 11:16:02.678134 tespy-0.7.3/src/tespy/tools/fluid_properties/__init__.py
--rw-r--r--   0        0        0     9666 2024-04-15 11:16:02.678134 tespy-0.7.3/src/tespy/tools/fluid_properties/functions.py
--rw-r--r--   0        0        0     9700 2024-04-15 11:16:02.679134 tespy-0.7.3/src/tespy/tools/fluid_properties/helpers.py
--rw-r--r--   0        0        0    12386 2024-04-15 11:16:02.679134 tespy-0.7.3/src/tespy/tools/fluid_properties/mixtures.py
--rw-r--r--   0        0        0    13368 2024-04-15 11:16:02.680134 tespy-0.7.3/src/tespy/tools/fluid_properties/wrappers.py
--rw-r--r--   0        0        0     3454 2024-04-15 11:16:02.680134 tespy-0.7.3/src/tespy/tools/global_vars.py
--rw-r--r--   0        0        0    20301 2024-04-15 17:02:58.342708 tespy-0.7.3/src/tespy/tools/helpers.py
--rw-r--r--   0        0        0    15049 2024-04-15 11:16:02.681134 tespy-0.7.3/src/tespy/tools/logger.py
--rw-r--r--   0        0        0    10421 2024-04-15 11:16:02.682134 tespy-0.7.3/src/tespy/tools/optimization.py
--rw-r--r--   0        0        0      427 2024-04-15 11:16:02.682134 tespy-0.7.3/tests/test_advanced_tutorials.py
--rw-r--r--   0        0        0     4337 2024-02-08 10:33:11.326315 tespy-0.7.3/tests/test_analyses/test_entropy_analysis.py
--rw-r--r--   0        0        0    24440 2024-02-08 10:33:11.329316 tespy-0.7.3/tests/test_analyses/test_exergy_analysis.py
--rw-r--r--   0        0        0      315 2024-04-15 11:16:02.683135 tespy-0.7.3/tests/test_basic_tutorials.py
--rw-r--r--   0        0        0    10214 2024-04-15 11:16:02.684136 tespy-0.7.3/tests/test_busses.py
--rw-r--r--   0        0        0    11728 2024-04-15 11:16:02.685134 tespy-0.7.3/tests/test_components/test_combustion.py
--rw-r--r--   0        0        0      346 2024-02-08 10:33:11.339314 tespy-0.7.3/tests/test_components/test_customs.py
--rw-r--r--   0        0        0     1627 2024-04-15 11:16:02.685134 tespy-0.7.3/tests/test_components/test_drum.py
--rw-r--r--   0        0        0    23305 2024-02-08 10:33:11.344314 tespy-0.7.3/tests/test_components/test_heat_exchangers.py
--rw-r--r--   0        0        0     4028 2024-04-15 11:16:02.685134 tespy-0.7.3/tests/test_components/test_merge.py
--rw-r--r--   0        0        0     3150 2024-02-08 10:33:11.349315 tespy-0.7.3/tests/test_components/test_piping.py
--rw-r--r--   0        0        0     7107 2024-04-15 11:16:02.686134 tespy-0.7.3/tests/test_components/test_reactors.py
--rw-r--r--   0        0        0    17021 2024-02-08 10:33:11.356315 tespy-0.7.3/tests/test_components/test_turbomachinery.py
--rw-r--r--   0        0        0     4025 2024-04-15 11:16:02.686134 tespy-0.7.3/tests/test_connections.py
--rw-r--r--   0        0        0    20109 2024-04-15 16:52:09.433248 tespy-0.7.3/tests/test_errors.py
--rw-r--r--   0        0        0      455 2024-04-15 11:16:02.686134 tespy-0.7.3/tests/test_heat_pump_exergy.py
--rw-r--r--   0        0        0      996 2023-11-14 11:35:05.574460 tespy-0.7.3/tests/test_models/cgam-ebsilon-results.csv
--rw-r--r--   0        0        0     7604 2024-02-08 10:33:11.365316 tespy-0.7.3/tests/test_models/test_CGAM_model.py
--rw-r--r--   0        0        0    12500 2024-02-08 10:33:11.369315 tespy-0.7.3/tests/test_models/test_heat_pump_model.py
--rw-r--r--   0        0        0    18609 2024-02-08 10:33:11.371315 tespy-0.7.3/tests/test_models/test_solar_energy_generating_system.py
--rw-r--r--   0        0        0     1664 2024-04-15 11:16:02.687135 tespy-0.7.3/tests/test_networks/test_binary_incompressible.py
--rw-r--r--   0        0        0     5571 2024-04-15 11:16:02.688135 tespy-0.7.3/tests/test_networks/test_mixing_rules.py
--rw-r--r--   0        0        0    24711 2024-04-15 11:16:02.688135 tespy-0.7.3/tests/test_networks/test_network.py
--rw-r--r--   0        0        0     7913 2023-11-27 18:42:13.447683 tespy-0.7.3/tests/test_tools/test_characteristics.py
--rw-r--r--   0        0        0    12983 2024-02-08 10:33:11.383315 tespy-0.7.3/tests/test_tools/test_fluid_properties/test_coolprop.py
--rw-r--r--   0        0        0     2106 2024-02-08 10:33:11.385316 tespy-0.7.3/tests/test_tools/test_fluid_properties/test_iapws.py
--rw-r--r--   0        0        0     1385 2024-02-08 10:33:11.387315 tespy-0.7.3/tests/test_tools/test_fluid_properties/test_pyromat.py
--rw-r--r--   0        0        0     2237 2024-04-15 17:02:58.342708 tespy-0.7.3/tests/test_tools/test_helpers.py
--rw-r--r--   0        0        0     2000 2024-02-08 10:33:11.392315 tespy-0.7.3/tox.ini
--rw-r--r--   0        0        0      261 2024-02-08 10:33:11.396315 tespy-0.7.3/tutorial/README.rst
--rw-r--r--   0        0        0     9727 2024-04-15 11:16:02.689135 tespy-0.7.3/tutorial/advanced/optimization_example.py
--rw-r--r--   0        0        0     9541 2024-04-15 11:16:02.690135 tespy-0.7.3/tutorial/advanced/starting_values.py
--rw-r--r--   0        0        0     6090 2024-04-15 11:16:02.691134 tespy-0.7.3/tutorial/advanced/stepwise.py
--rw-r--r--   0        0        0     4264 2024-02-08 10:33:11.406315 tespy-0.7.3/tutorial/basics/district_heating.py
--rw-r--r--   0        0        0     4978 2024-04-15 11:16:02.691134 tespy-0.7.3/tutorial/basics/gas_turbine.py
--rw-r--r--   0        0        0     3216 2024-02-08 10:33:11.411315 tespy-0.7.3/tutorial/basics/heat_pump.py
--rw-r--r--   0        0        0     4661 2024-04-15 11:16:02.692154 tespy-0.7.3/tutorial/basics/rankine.py
--rw-r--r--   0        0        0     4201 2024-02-08 10:33:11.416315 tespy-0.7.3/tutorial/heat_pump_exergy/NH3.py
--rw-r--r--   0        0        0    10920 2024-04-15 11:16:02.693134 tespy-0.7.3/tutorial/heat_pump_exergy/NH3_calculations.py
--rw-r--r--   0        0        0     4217 2024-02-08 10:33:11.421314 tespy-0.7.3/tutorial/heat_pump_exergy/R410A.py
--rw-r--r--   0        0        0    10943 2024-04-15 11:16:02.693134 tespy-0.7.3/tutorial/heat_pump_exergy/R410A_calculations.py
--rw-r--r--   0        0        0     8277 2024-02-08 10:33:11.426314 tespy-0.7.3/tutorial/heat_pump_exergy/plots.py
--rw-r--r--   0        0        0    10587 1970-01-01 00:00:00.000000 tespy-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      265 2021-10-04 06:28:48.000000 tespy-0.7.4/.editorconfig
+-rw-r--r--   0        0        0     1446 2021-10-04 06:28:48.000000 tespy-0.7.4/.pep8speaks.yml
+-rw-r--r--   0        0        0      341 2023-11-14 11:35:05.186734 tespy-0.7.4/.readthedocs.yml
+-rw-r--r--   0        0        0     3269 2021-10-04 06:28:48.000000 tespy-0.7.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      154 2022-01-28 07:48:36.000000 tespy-0.7.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1088 2024-04-16 16:42:16.443578 tespy-0.7.4/LICENSE
+-rw-r--r--   0        0        0      281 2023-11-14 11:35:05.190735 tespy-0.7.4/MANIFEST.in
+-rw-r--r--   0        0        0      765 2021-10-04 06:28:48.000000 tespy-0.7.4/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     9116 2024-04-16 16:42:16.443578 tespy-0.7.4/README.rst
+-rw-r--r--   0        0        0      180 2023-11-14 11:35:05.203247 tespy-0.7.4/docs/_static/css/custom.css
+-rw-r--r--   0        0        0   129643 2023-11-14 11:35:05.207242 tespy-0.7.4/docs/_static/images/advanced/exergy/flowsheet.svg
+-rw-r--r--   0        0        0   136810 2023-11-14 11:35:05.210242 tespy-0.7.4/docs/_static/images/advanced/exergy/flowsheet_darkmode.svg
+-rw-r--r--   0        0        0    32134 2023-11-14 11:35:05.212242 tespy-0.7.4/docs/_static/images/advanced/exergy/sankey.svg
+-rw-r--r--   0        0        0    17276 2023-11-14 11:35:05.213286 tespy-0.7.4/docs/_static/images/basics/district_heating.svg
+-rw-r--r--   0        0        0    18111 2023-11-14 11:35:05.215279 tespy-0.7.4/docs/_static/images/basics/district_heating_darkmode.svg
+-rw-r--r--   0        0        0    69064 2023-11-14 11:35:05.218243 tespy-0.7.4/docs/_static/images/basics/district_heating_partload.svg
+-rw-r--r--   0        0        0    71199 2023-11-14 11:35:05.220243 tespy-0.7.4/docs/_static/images/basics/district_heating_partload_darkmode.svg
+-rw-r--r--   0        0        0    15810 2023-11-14 11:35:05.222242 tespy-0.7.4/docs/_static/images/basics/gas_turbine.svg
+-rw-r--r--   0        0        0    16340 2023-11-14 11:35:05.223244 tespy-0.7.4/docs/_static/images/basics/gas_turbine_darkmode.svg
+-rw-r--r--   0        0        0    32095 2023-11-14 11:35:05.225250 tespy-0.7.4/docs/_static/images/basics/gas_turbine_fuel_composition.svg
+-rw-r--r--   0        0        0    32756 2023-11-14 11:35:05.227255 tespy-0.7.4/docs/_static/images/basics/gas_turbine_fuel_composition_darkmode.svg
+-rw-r--r--   0        0        0    29612 2023-11-14 11:35:05.228284 tespy-0.7.4/docs/_static/images/basics/gas_turbine_oxygen.svg
+-rw-r--r--   0        0        0    30202 2023-11-14 11:35:05.230296 tespy-0.7.4/docs/_static/images/basics/gas_turbine_oxygen_darkmode.svg
+-rw-r--r--   0        0        0    57559 2023-11-14 11:35:05.231295 tespy-0.7.4/docs/_static/images/basics/gas_turbine_parametric.svg
+-rw-r--r--   0        0        0    59255 2023-11-14 11:35:05.233242 tespy-0.7.4/docs/_static/images/basics/gas_turbine_parametric_darkmode.svg
+-rw-r--r--   0        0        0    14362 2023-11-14 11:35:05.234243 tespy-0.7.4/docs/_static/images/basics/heat_pump.svg
+-rw-r--r--   0        0        0    14866 2023-11-14 11:35:05.236243 tespy-0.7.4/docs/_static/images/basics/heat_pump_darkmode.svg
+-rw-r--r--   0        0        0    53423 2023-11-14 11:35:05.237245 tespy-0.7.4/docs/_static/images/basics/heat_pump_parametric.svg
+-rw-r--r--   0        0        0    54994 2023-11-14 11:35:05.240244 tespy-0.7.4/docs/_static/images/basics/heat_pump_parametric_darkmode.svg
+-rw-r--r--   0        0        0    16030 2023-11-14 11:35:05.241287 tespy-0.7.4/docs/_static/images/basics/modeling_concept.svg
+-rw-r--r--   0        0        0    16137 2023-11-14 11:35:05.242303 tespy-0.7.4/docs/_static/images/basics/rankine_cycle.svg
+-rw-r--r--   0        0        0    16871 2023-11-14 11:35:05.243245 tespy-0.7.4/docs/_static/images/basics/rankine_cycle_darkmode.svg
+-rw-r--r--   0        0        0    59916 2023-11-14 11:35:05.245276 tespy-0.7.4/docs/_static/images/basics/rankine_parametric.svg
+-rw-r--r--   0        0        0    61115 2023-11-14 11:35:05.247242 tespy-0.7.4/docs/_static/images/basics/rankine_parametric_darkmode.svg
+-rw-r--r--   0        0        0    26962 2023-11-14 11:35:05.248242 tespy-0.7.4/docs/_static/images/basics/rankine_partload.svg
+-rw-r--r--   0        0        0    27517 2023-11-14 11:35:05.250241 tespy-0.7.4/docs/_static/images/basics/rankine_partload_darkmode.svg
+-rw-r--r--   0        0        0   139795 2023-11-14 11:35:05.254645 tespy-0.7.4/docs/_static/images/examples/GRC_flowsheet.svg
+-rw-r--r--   0        0        0   157545 2023-11-14 11:35:05.259751 tespy-0.7.4/docs/_static/images/examples/GRC_flowsheet_darkmode.svg
+-rw-r--r--   0        0        0    88269 2023-11-14 11:35:05.262970 tespy-0.7.4/docs/_static/images/examples/ORC_parametric_flowsheet.svg
+-rw-r--r--   0        0        0    88176 2023-11-14 11:35:05.266014 tespy-0.7.4/docs/_static/images/examples/ORC_parametric_flowsheet_darkmode.svg
+-rw-r--r--   0        0        0   409001 2023-11-14 11:35:05.275027 tespy-0.7.4/docs/_static/images/examples/PM_CAES_graphical-abstract.svg
+-rw-r--r--   0        0        0   417664 2023-11-14 11:35:05.283696 tespy-0.7.4/docs/_static/images/examples/PM_CAES_graphical-abstract_darkmode.svg
+-rw-r--r--   0        0        0    39020 2023-11-14 11:35:05.284697 tespy-0.7.4/docs/_static/images/logo_tespy_big.svg
+-rw-r--r--   0        0        0    39647 2023-11-14 11:35:05.285746 tespy-0.7.4/docs/_static/images/logo_tespy_big_darkmode.svg
+-rw-r--r--   0        0        0    17145 2023-11-14 11:35:05.287696 tespy-0.7.4/docs/_static/images/logo_tespy_big_editable_font.svg
+-rw-r--r--   0        0        0    23121 2024-04-15 08:10:01.844502 tespy-0.7.4/docs/_static/images/logo_tespy_mid.svg
+-rw-r--r--   0        0        0    24693 2024-04-16 16:42:16.443578 tespy-0.7.4/docs/_static/images/logo_tespy_mid_christmas.svg
+-rw-r--r--   0        0        0    23260 2023-11-14 11:35:05.289734 tespy-0.7.4/docs/_static/images/logo_tespy_mid_darkmode.svg
+-rw-r--r--   0        0        0    24872 2024-04-16 16:42:16.456092 tespy-0.7.4/docs/_static/images/logo_tespy_mid_darkmode_christmas.svg
+-rw-r--r--   0        0        0    15239 2023-11-14 11:35:05.290696 tespy-0.7.4/docs/_static/images/logo_tespy_mid_editable_font.svg
+-rw-r--r--   0        0        0    13985 2023-11-27 18:42:13.344791 tespy-0.7.4/docs/_static/images/logo_tespy_mini.svg
+-rw-r--r--   0        0        0    13302 2023-11-14 11:35:05.293737 tespy-0.7.4/docs/_static/images/logo_tespy_small.svg
+-rw-r--r--   0        0        0   157002 2023-11-14 11:35:05.299887 tespy-0.7.4/docs/_static/images/modules/Ts_diagram_states.svg
+-rw-r--r--   0        0        0     8644 2023-11-14 11:35:05.301873 tespy-0.7.4/docs/_static/images/modules/characteristics.svg
+-rw-r--r--   0        0        0     8414 2023-11-14 11:35:05.302847 tespy-0.7.4/docs/_static/images/modules/characteristics_darkmode.svg
+-rw-r--r--   0        0        0    11300 2023-11-14 11:35:05.304847 tespy-0.7.4/docs/_static/images/modules/connections.svg
+-rw-r--r--   0        0        0    11315 2023-11-14 11:35:05.305848 tespy-0.7.4/docs/_static/images/modules/connections_darkmode.svg
+-rw-r--r--   0        0        0   134345 2023-11-14 11:35:05.308847 tespy-0.7.4/docs/_static/images/modules/fluid_properties.svg
+-rw-r--r--   0        0        0   125300 2023-11-14 11:35:05.310847 tespy-0.7.4/docs/_static/images/modules/fluid_properties_darkmode.svg
+-rw-r--r--   0        0        0   168665 2023-11-14 11:35:05.315851 tespy-0.7.4/docs/_static/images/modules/logph_diagram_states.svg
+-rw-r--r--   0        0        0    17587 2023-11-14 11:35:05.317845 tespy-0.7.4/docs/_static/images/modules/subsystem_waste_heat_generator.svg
+-rw-r--r--   0        0        0    17663 2023-11-14 11:35:05.320845 tespy-0.7.4/docs/_static/images/modules/subsystem_waste_heat_generator_darkmode.svg
+-rw-r--r--   0        0        0   121692 2023-11-14 11:35:05.322846 tespy-0.7.4/docs/_static/images/modules/ude.svg
+-rw-r--r--   0        0        0   125035 2023-11-14 11:35:05.324845 tespy-0.7.4/docs/_static/images/modules/ude_darkmode.svg
+-rw-r--r--   0        0        0    33944 2023-11-14 11:35:05.327439 tespy-0.7.4/docs/_static/images/tutorials/district_heating_system/dhs.svg
+-rw-r--r--   0        0        0    20206 2023-11-14 11:35:05.329488 tespy-0.7.4/docs/_static/images/tutorials/district_heating_system/dhs_closed.svg
+-rw-r--r--   0        0        0    12074 2023-11-14 11:35:05.331495 tespy-0.7.4/docs/_static/images/tutorials/district_heating_system/dhs_forks.svg
+-rw-r--r--   0        0        0    21711 2023-11-14 11:35:05.333492 tespy-0.7.4/docs/_static/images/tutorials/district_heating_system/dhs_open.svg
+-rw-r--r--   0        0        0   168149 2023-11-14 11:35:05.337492 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/NH3_logph.svg
+-rw-r--r--   0        0        0    23347 2023-11-14 11:35:05.338492 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/NH3_sankey.svg
+-rw-r--r--   0        0        0    60290 2023-11-14 11:35:05.339484 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D.svg
+-rw-r--r--   0        0        0    61853 2023-11-14 11:35:05.340503 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D_darkmode.svg
+-rw-r--r--   0        0        0    61177 2023-11-14 11:35:05.342490 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q.svg
+-rw-r--r--   0        0        0    62156 2023-11-14 11:35:05.342490 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q_darkmode.svg
+-rw-r--r--   0        0        0    66033 2023-11-14 11:35:05.344487 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths.svg
+-rw-r--r--   0        0        0    67428 2023-11-14 11:35:05.345486 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths_darkmode.svg
+-rw-r--r--   0        0        0    52499 2023-11-14 11:35:05.346490 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo.svg
+-rw-r--r--   0        0        0    53372 2023-11-14 11:35:05.347488 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo_darkmode.svg
+-rw-r--r--   0        0        0    29826 2023-11-14 11:35:05.348490 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/flowsheet.svg
+-rw-r--r--   0        0        0    29835 2023-11-14 11:35:05.349496 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/flowsheet_darkmode.svg
+-rw-r--r--   0        0        0    27850 2023-11-14 11:35:05.350453 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf.svg
+-rw-r--r--   0        0        0    28404 2023-11-14 11:35:05.351485 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf_darkmode.svg
+-rw-r--r--   0        0        0    30290 2023-11-14 11:35:05.352501 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet.svg
+-rw-r--r--   0        0        0    30299 2023-11-14 11:35:05.353493 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet_darkmode.svg
+-rw-r--r--   0        0        0   227184 2023-11-14 11:35:05.356486 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_starting_values/logph.svg
+-rw-r--r--   0        0        0    46257 2023-11-14 11:35:05.357488 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet.svg
+-rw-r--r--   0        0        0    46240 2023-11-14 11:35:05.358489 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_darkmode.svg
+-rw-r--r--   0        0        0    46286 2023-11-14 11:35:05.359486 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1.svg
+-rw-r--r--   0        0        0    46277 2023-11-14 11:35:05.360489 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1_darkmode.svg
+-rw-r--r--   0        0        0    46669 2023-11-14 11:35:05.361488 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2.svg
+-rw-r--r--   0        0        0    46657 2023-11-14 11:35:05.362482 tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2_darkmode.svg
+-rw-r--r--   0        0        0    52832 2023-11-14 11:35:05.364488 tespy-0.7.4/docs/_static/images/tutorials/osmses-2023.svg
+-rw-r--r--   0        0        0    53182 2023-11-14 11:35:05.366491 tespy-0.7.4/docs/_static/images/tutorials/osmses-2023_darkmode.svg
+-rw-r--r--   0        0        0    33530 2023-11-14 11:35:05.368487 tespy-0.7.4/docs/_static/images/tutorials/pygmo_optimization/flowsheet.svg
+-rw-r--r--   0        0        0    34684 2023-11-14 11:35:05.369487 tespy-0.7.4/docs/_static/images/tutorials/pygmo_optimization/flowsheet_darkmode.svg
+-rw-r--r--   0        0        0   190475 2023-11-14 11:35:05.371488 tespy-0.7.4/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization.svg
+-rw-r--r--   0        0        0   192983 2023-11-14 11:35:05.372490 tespy-0.7.4/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization_darkmode.svg
+-rw-r--r--   0        0        0      578 2024-04-16 16:42:16.456092 tespy-0.7.4/docs/_static/js/custom.js
+-rw-r--r--   0        0        0        0 2023-11-14 11:35:05.375500 tespy-0.7.4/docs/_templates/index.html
+-rw-r--r--   0        0        0    20686 2023-11-27 18:42:13.344791 tespy-0.7.4/docs/advanced/exergy.rst
+-rw-r--r--   0        0        0       92 2023-11-14 11:35:05.377489 tespy-0.7.4/docs/advanced/optimization.rst
+-rw-r--r--   0        0        0      532 2023-11-27 18:42:13.352886 tespy-0.7.4/docs/api.rst
+-rw-r--r--   0        0        0     9313 2023-11-14 11:35:05.380489 tespy-0.7.4/docs/api/_images/CombustionChamber.svg
+-rw-r--r--   0        0        0     9682 2023-11-14 11:35:05.380489 tespy-0.7.4/docs/api/_images/CombustionChamber_darkmode.svg
+-rw-r--r--   0        0        0    15877 2023-11-14 11:35:05.382455 tespy-0.7.4/docs/api/_images/CombustionEngine.svg
+-rw-r--r--   0        0        0    16472 2023-11-14 11:35:05.383486 tespy-0.7.4/docs/api/_images/CombustionEngine_darkmode.svg
+-rw-r--r--   0        0        0     7484 2023-11-14 11:35:05.384453 tespy-0.7.4/docs/api/_images/Compressor.svg
+-rw-r--r--   0        0        0     7661 2023-11-14 11:35:05.384453 tespy-0.7.4/docs/api/_images/Compressor_darkmode.svg
+-rw-r--r--   0        0        0     9565 2023-11-14 11:35:05.385452 tespy-0.7.4/docs/api/_images/Condenser.svg
+-rw-r--r--   0        0        0    10115 2023-11-14 11:35:05.386452 tespy-0.7.4/docs/api/_images/Condenser_darkmode.svg
+-rw-r--r--   0        0        0     8889 2024-04-16 16:42:16.456092 tespy-0.7.4/docs/api/_images/DropletSeparator.svg
+-rw-r--r--   0        0        0     9030 2024-04-16 16:42:16.456092 tespy-0.7.4/docs/api/_images/DropletSeparator_darkmode.svg
+-rw-r--r--   0        0        0    10414 2023-11-14 11:35:05.389475 tespy-0.7.4/docs/api/_images/Drum.svg
+-rw-r--r--   0        0        0    10583 2023-11-14 11:35:05.389475 tespy-0.7.4/docs/api/_images/Drum_darkmode.svg
+-rw-r--r--   0        0        0    15148 2023-11-14 11:35:05.390494 tespy-0.7.4/docs/api/_images/FuelCell.svg
+-rw-r--r--   0        0        0    15153 2023-11-14 11:35:05.391488 tespy-0.7.4/docs/api/_images/FuelCell_darkmode.svg
+-rw-r--r--   0        0        0    10283 2023-11-14 11:35:05.392501 tespy-0.7.4/docs/api/_images/HeatExchanger.svg
+-rw-r--r--   0        0        0    10403 2023-11-14 11:35:05.393481 tespy-0.7.4/docs/api/_images/HeatExchanger_darkmode.svg
+-rw-r--r--   0        0        0    12851 2023-11-14 11:35:05.394490 tespy-0.7.4/docs/api/_images/Merge.svg
+-rw-r--r--   0        0        0    13017 2023-11-14 11:35:05.394490 tespy-0.7.4/docs/api/_images/Merge_darkmode.svg
+-rw-r--r--   0        0        0     8013 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/ORCEvaporator.svg
+-rw-r--r--   0        0        0     7643 2023-11-14 11:35:05.396453 tespy-0.7.4/docs/api/_images/ParabolicTrough.svg
+-rw-r--r--   0        0        0     7823 2023-11-14 11:35:05.396453 tespy-0.7.4/docs/api/_images/ParabolicTrough_darkmode.svg
+-rw-r--r--   0        0        0     6462 2023-11-14 11:35:05.398490 tespy-0.7.4/docs/api/_images/Pipe.svg
+-rw-r--r--   0        0        0     6640 2023-11-14 11:35:05.399484 tespy-0.7.4/docs/api/_images/Pipe_darkmode.svg
+-rw-r--r--   0        0        0     7414 2023-11-14 11:35:05.400485 tespy-0.7.4/docs/api/_images/Pump.svg
+-rw-r--r--   0        0        0     7478 2023-11-14 11:35:05.400485 tespy-0.7.4/docs/api/_images/Pump_darkmode.svg
+-rw-r--r--   0        0        0     6810 2023-11-14 11:35:05.401451 tespy-0.7.4/docs/api/_images/SolarCollector.svg
+-rw-r--r--   0        0        0     6875 2023-11-14 11:35:05.402487 tespy-0.7.4/docs/api/_images/SolarCollector_darkmode.svg
+-rw-r--r--   0        0        0    12813 2023-11-14 11:35:05.403490 tespy-0.7.4/docs/api/_images/Splitter.svg
+-rw-r--r--   0        0        0    12979 2023-11-14 11:35:05.404518 tespy-0.7.4/docs/api/_images/Splitter_darkmode.svg
+-rw-r--r--   0        0        0    12381 2023-11-14 11:35:05.405488 tespy-0.7.4/docs/api/_images/SubsystemInterface.svg
+-rw-r--r--   0        0        0    12558 2023-11-14 11:35:05.405488 tespy-0.7.4/docs/api/_images/SubsystemInterface_darkmode.svg
+-rw-r--r--   0        0        0     6668 2023-11-14 11:35:05.406452 tespy-0.7.4/docs/api/_images/Turbine.svg
+-rw-r--r--   0        0        0     6677 2023-11-14 11:35:05.407500 tespy-0.7.4/docs/api/_images/Turbine_darkmode.svg
+-rw-r--r--   0        0        0     6491 2023-11-14 11:35:05.408451 tespy-0.7.4/docs/api/_images/Valve.svg
+-rw-r--r--   0        0        0     6668 2023-11-14 11:35:05.409492 tespy-0.7.4/docs/api/_images/Valve_darkmode.svg
+-rw-r--r--   0        0        0    13372 2023-11-14 11:35:05.410490 tespy-0.7.4/docs/api/_images/WaterElectrolyzer.svg
+-rw-r--r--   0        0        0    15165 2023-11-14 11:35:05.410490 tespy-0.7.4/docs/api/_images/WaterElectrolyzer_darkmode.svg
+-rw-r--r--   0        0        0    40711 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/combustion_engine_Q1_char_DEFAULT.svg
+-rw-r--r--   0        0        0    40966 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/combustion_engine_Q2_char_DEFAULT.svg
+-rw-r--r--   0        0        0    38781 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/combustion_engine_Qloss_char_DEFAULT.svg
+-rw-r--r--   0        0        0    37655 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/combustion_engine_tiP_char_DEFAULT.svg
+-rw-r--r--   0        0        0    49048 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/compressor_char_map_eta_s_DEFAULT.svg
+-rw-r--r--   0        0        0    46950 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/compressor_char_map_pr_DEFAULT.svg
+-rw-r--r--   0        0        0    39251 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/compressor_eta_s_char_DEFAULT.svg
+-rw-r--r--   0        0        0    40197 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/condenser_kA_char1_DEFAULT.svg
+-rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/condenser_kA_char2_DEFAULT.svg
+-rw-r--r--   0        0        0    42372 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/desuperheater_kA_char1_DEFAULT.svg
+-rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/desuperheater_kA_char2_DEFAULT.svg
+-rw-r--r--   0        0        0    43523 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/heat_exchanger_kA_char1_CONDENSING_FLUID.svg
+-rw-r--r--   0        0        0    42372 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/heat_exchanger_kA_char1_DEFAULT.svg
+-rw-r--r--   0        0        0    41171 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/heat_exchanger_kA_char2_DEFAULT.svg
+-rw-r--r--   0        0        0    45010 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/heat_exchanger_kA_char2_EVAPORATING_FLUID.svg
+-rw-r--r--   0        0        0    42314 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/heat_exchanger_simple_kA_char_DEFAULT.svg
+-rw-r--r--   0        0        0    42314 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/pipe_kA_char_DEFAULT.svg
+-rw-r--r--   0        0        0    40653 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/pump_eta_s_char_DEFAULT.svg
+-rw-r--r--   0        0        0    39798 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/turbine_eta_s_char_DEFAULT.svg
+-rw-r--r--   0        0        0    40222 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/turbine_eta_s_char_TRAUPEL.svg
+-rw-r--r--   0        0        0    36210 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/api/_images/water_electrolyzer_eta_char_DEFAULT.svg
+-rw-r--r--   0        0        0     6139 2024-04-16 16:42:16.456092 tespy-0.7.4/docs/api/components.rst
+-rw-r--r--   0        0        0      496 2023-11-14 11:35:05.412490 tespy-0.7.4/docs/api/connections.rst
+-rw-r--r--   0        0        0     4204 2023-11-14 11:35:05.414490 tespy-0.7.4/docs/api/data.rst
+-rw-r--r--   0        0        0      493 2023-11-14 11:35:05.415452 tespy-0.7.4/docs/api/networks.rst
+-rw-r--r--   0        0        0     2161 2024-04-16 16:42:16.471744 tespy-0.7.4/docs/api/tools.rst
+-rw-r--r--   0        0        0     2463 2023-11-14 11:35:05.417470 tespy-0.7.4/docs/basics.rst
+-rw-r--r--   0        0        0     5528 2024-04-16 16:42:16.471744 tespy-0.7.4/docs/basics/district_heating.rst
+-rw-r--r--   0        0        0    10772 2024-04-16 16:42:16.471744 tespy-0.7.4/docs/basics/gas_turbine.rst
+-rw-r--r--   0        0        0     6691 2023-11-27 18:42:13.352886 tespy-0.7.4/docs/basics/heat_pump.rst
+-rw-r--r--   0        0        0     7125 2024-04-16 16:42:16.471744 tespy-0.7.4/docs/basics/intro.rst
+-rw-r--r--   0        0        0    10668 2024-04-16 16:42:16.487371 tespy-0.7.4/docs/basics/rankine_cycle.rst
+-rw-r--r--   0        0        0     2743 2024-04-16 16:42:16.487371 tespy-0.7.4/docs/benchmarks.rst
+-rw-r--r--   0        0        0     4695 2024-04-16 16:42:16.487371 tespy-0.7.4/docs/conf.py
+-rw-r--r--   0        0        0     7315 2023-11-27 18:42:13.352886 tespy-0.7.4/docs/development/how.rst
+-rw-r--r--   0        0        0     3192 2024-04-16 16:42:16.487371 tespy-0.7.4/docs/development/what.rst
+-rw-r--r--   0        0        0     4319 2023-11-27 18:42:13.352886 tespy-0.7.4/docs/examples.rst
+-rw-r--r--   0        0        0      661 2023-11-14 11:35:05.429456 tespy-0.7.4/docs/index.rst
+-rw-r--r--   0        0        0     2890 2023-11-14 11:35:05.431452 tespy-0.7.4/docs/installation.rst
+-rw-r--r--   0        0        0     3853 2023-11-27 18:42:13.352886 tespy-0.7.4/docs/introduction.rst
+-rw-r--r--   0        0        0     2398 2023-11-14 11:35:05.433499 tespy-0.7.4/docs/modules.rst
+-rw-r--r--   0        0        0     5082 2023-11-27 18:42:13.368512 tespy-0.7.4/docs/modules/characteristics.rst
+-rw-r--r--   0        0        0    34468 2024-04-16 16:42:16.487371 tespy-0.7.4/docs/modules/components.rst
+-rw-r--r--   0        0        0    15728 2024-04-16 16:42:16.502998 tespy-0.7.4/docs/modules/connections.rst
+-rw-r--r--   0        0        0    15251 2024-04-19 10:46:21.757834 tespy-0.7.4/docs/modules/fluid_properties.rst
+-rw-r--r--   0        0        0    32940 2024-04-16 16:42:16.502998 tespy-0.7.4/docs/modules/networks.rst
+-rw-r--r--   0        0        0    12661 2024-04-16 16:42:16.502998 tespy-0.7.4/docs/modules/ude.rst
+-rw-r--r--   0        0        0    12186 2024-04-16 16:42:16.502998 tespy-0.7.4/docs/references.bib
+-rw-r--r--   0        0        0      886 2023-11-14 11:35:05.443458 tespy-0.7.4/docs/regular_meeting.rst
+-rw-r--r--   0        0        0       77 2024-04-16 16:42:16.518623 tespy-0.7.4/docs/requirements.txt
+-rw-r--r--   0        0        0     2906 2024-04-30 16:09:15.292443 tespy-0.7.4/docs/scripts/generate_tespy_data_module.py
+-rw-r--r--   0        0        0     3594 2023-11-27 18:42:13.369520 tespy-0.7.4/docs/tutorials.rst
+-rw-r--r--   0        0        0     2365 2023-11-27 18:42:13.369520 tespy-0.7.4/docs/tutorials/district_heating.rst
+-rw-r--r--   0        0        0    32094 2024-04-16 16:42:16.518623 tespy-0.7.4/docs/tutorials/heat_pump_exergy.rst
+-rw-r--r--   0        0        0    21439 2024-04-16 16:42:16.518623 tespy-0.7.4/docs/tutorials/heat_pump_steps.rst
+-rw-r--r--   0        0        0     7904 2023-11-27 18:42:13.369520 tespy-0.7.4/docs/tutorials/pygmo_optimization.rst
+-rw-r--r--   0        0        0     8543 2023-11-27 18:42:13.369520 tespy-0.7.4/docs/tutorials/starting_values.rst
+-rw-r--r--   0        0        0     1396 2024-04-30 16:09:15.292443 tespy-0.7.4/docs/whats_new.rst
+-rw-r--r--   0        0        0      240 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/whats_new/v0-0-1.rst
+-rw-r--r--   0        0        0     1548 2023-11-14 11:35:05.456506 tespy-0.7.4/docs/whats_new/v0-0-2.rst
+-rw-r--r--   0        0        0     4807 2023-11-14 11:35:05.457491 tespy-0.7.4/docs/whats_new/v0-0-3.rst
+-rw-r--r--   0        0        0     1994 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/whats_new/v0-0-4.rst
+-rw-r--r--   0        0        0     3293 2023-07-20 10:11:41.150532 tespy-0.7.4/docs/whats_new/v0-0-5.rst
+-rw-r--r--   0        0        0     3987 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/whats_new/v0-1-0.rst
+-rw-r--r--   0        0        0     4347 2023-11-14 11:35:05.459497 tespy-0.7.4/docs/whats_new/v0-1-1.rst
+-rw-r--r--   0        0        0     3842 2023-11-14 11:35:05.460492 tespy-0.7.4/docs/whats_new/v0-1-2.rst
+-rw-r--r--   0        0        0     2675 2023-11-14 11:35:05.462483 tespy-0.7.4/docs/whats_new/v0-1-3.rst
+-rw-r--r--   0        0        0      616 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/whats_new/v0-1-4.rst
+-rw-r--r--   0        0        0     8338 2023-11-14 11:35:05.463455 tespy-0.7.4/docs/whats_new/v0-2-0.rst
+-rw-r--r--   0        0        0     1982 2022-05-26 10:30:52.000000 tespy-0.7.4/docs/whats_new/v0-2-1.rst
+-rw-r--r--   0        0        0     3064 2023-11-14 11:35:05.465487 tespy-0.7.4/docs/whats_new/v0-2-2.rst
+-rw-r--r--   0        0        0    11252 2023-11-14 11:35:05.466489 tespy-0.7.4/docs/whats_new/v0-3-0.rst
+-rw-r--r--   0        0        0      314 2022-05-26 10:30:52.000000 tespy-0.7.4/docs/whats_new/v0-3-1.rst
+-rw-r--r--   0        0        0     2062 2023-07-20 10:11:41.153549 tespy-0.7.4/docs/whats_new/v0-3-2.rst
+-rw-r--r--   0        0        0     1345 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/whats_new/v0-3-3.rst
+-rw-r--r--   0        0        0     1471 2023-11-14 11:35:05.467454 tespy-0.7.4/docs/whats_new/v0-3-4.rst
+-rw-r--r--   0        0        0    11174 2023-11-14 11:35:05.468458 tespy-0.7.4/docs/whats_new/v0-4-0.rst
+-rw-r--r--   0        0        0     1126 2023-11-14 11:35:05.469487 tespy-0.7.4/docs/whats_new/v0-4-1.rst
+-rw-r--r--   0        0        0     1589 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/whats_new/v0-4-2.rst
+-rw-r--r--   0        0        0      563 2021-10-04 06:28:48.000000 tespy-0.7.4/docs/whats_new/v0-4-3-001.rst
+-rw-r--r--   0        0        0      656 2023-11-14 11:35:05.470480 tespy-0.7.4/docs/whats_new/v0-4-3-003.rst
+-rw-r--r--   0        0        0     3355 2023-11-14 11:35:05.471499 tespy-0.7.4/docs/whats_new/v0-4-3.rst
+-rw-r--r--   0        0        0     1183 2022-01-28 07:48:36.000000 tespy-0.7.4/docs/whats_new/v0-4-4.rst
+-rw-r--r--   0        0        0      801 2022-01-28 07:48:36.000000 tespy-0.7.4/docs/whats_new/v0-5-0.rst
+-rw-r--r--   0        0        0      930 2022-05-26 10:30:52.000000 tespy-0.7.4/docs/whats_new/v0-5-1.rst
+-rw-r--r--   0        0        0     2644 2023-11-14 11:35:05.473451 tespy-0.7.4/docs/whats_new/v0-6-0.rst
+-rw-r--r--   0        0        0     2064 2023-11-14 11:35:05.474453 tespy-0.7.4/docs/whats_new/v0-6-1.rst
+-rw-r--r--   0        0        0      385 2023-11-14 11:35:05.475486 tespy-0.7.4/docs/whats_new/v0-6-2.rst
+-rw-r--r--   0        0        0     2841 2023-11-14 11:35:05.476510 tespy-0.7.4/docs/whats_new/v0-6-3.rst
+-rw-r--r--   0        0        0     4014 2024-04-16 16:42:16.518623 tespy-0.7.4/docs/whats_new/v0-7-0.rst
+-rw-r--r--   0        0        0      427 2024-04-16 16:42:16.518623 tespy-0.7.4/docs/whats_new/v0-7-1.rst
+-rw-r--r--   0        0        0      841 2024-04-16 16:42:16.534246 tespy-0.7.4/docs/whats_new/v0-7-2.rst
+-rw-r--r--   0        0        0      363 2024-04-16 16:42:16.534246 tespy-0.7.4/docs/whats_new/v0-7-3.rst
+-rw-r--r--   0        0        0     1630 2024-04-30 16:09:15.292443 tespy-0.7.4/docs/whats_new/v0-7-4.rst
+-rw-r--r--   0        0        0       90 2023-11-14 11:35:05.478498 tespy-0.7.4/docs/zliterature.rst
+-rw-r--r--   0        0        0     6582 2023-11-14 11:35:05.480483 tespy-0.7.4/paper.bib
+-rw-r--r--   0        0        0    11023 2021-10-04 06:28:48.000000 tespy-0.7.4/paper.md
+-rw-r--r--   0        0        0     2607 2024-04-30 16:09:15.293427 tespy-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1187 2024-04-30 16:09:15.293427 tespy-0.7.4/src/tespy/__init__.py
+-rw-r--r--   0        0        0     1655 2024-04-16 16:53:10.839173 tespy-0.7.4/src/tespy/components/__init__.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.4/src/tespy/components/basics/__init__.py
+-rw-r--r--   0        0        0     5609 2024-04-30 16:09:15.293427 tespy-0.7.4/src/tespy/components/basics/cycle_closer.py
+-rw-r--r--   0        0        0     2775 2024-04-30 16:09:15.294427 tespy-0.7.4/src/tespy/components/basics/sink.py
+-rw-r--r--   0        0        0     3303 2024-04-30 16:09:15.294427 tespy-0.7.4/src/tespy/components/basics/source.py
+-rw-r--r--   0        0        0     5327 2024-04-30 16:09:15.294427 tespy-0.7.4/src/tespy/components/basics/subsystem_interface.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.4/src/tespy/components/combustion/__init__.py
+-rw-r--r--   0        0        0    47361 2024-04-30 16:09:15.295428 tespy-0.7.4/src/tespy/components/combustion/base.py
+-rw-r--r--   0        0        0    13911 2024-04-30 16:09:15.295428 tespy-0.7.4/src/tespy/components/combustion/diabatic.py
+-rw-r--r--   0        0        0    55778 2024-04-30 16:09:15.296427 tespy-0.7.4/src/tespy/components/combustion/engine.py
+-rw-r--r--   0        0        0    41620 2024-04-30 16:09:15.296427 tespy-0.7.4/src/tespy/components/component.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.4/src/tespy/components/customs/__init__.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.4/src/tespy/components/heat_exchangers/__init__.py
+-rw-r--r--   0        0        0    38339 2024-04-30 16:09:15.297427 tespy-0.7.4/src/tespy/components/heat_exchangers/base.py
+-rw-r--r--   0        0        0    18178 2024-04-30 16:09:15.297427 tespy-0.7.4/src/tespy/components/heat_exchangers/condenser.py
+-rw-r--r--   0        0        0     8611 2024-04-30 16:09:15.298426 tespy-0.7.4/src/tespy/components/heat_exchangers/desuperheater.py
+-rw-r--r--   0        0        0    13113 2024-04-30 16:09:15.298426 tespy-0.7.4/src/tespy/components/heat_exchangers/parabolic_trough.py
+-rw-r--r--   0        0        0    43520 2024-04-30 16:09:15.299429 tespy-0.7.4/src/tespy/components/heat_exchangers/simple.py
+-rw-r--r--   0        0        0    11340 2024-04-30 16:09:15.299429 tespy-0.7.4/src/tespy/components/heat_exchangers/solar_collector.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.4/src/tespy/components/nodes/__init__.py
+-rw-r--r--   0        0        0     6174 2024-04-30 16:09:15.299429 tespy-0.7.4/src/tespy/components/nodes/base.py
+-rw-r--r--   0        0        0    13390 2024-04-30 16:09:15.300428 tespy-0.7.4/src/tespy/components/nodes/droplet_separator.py
+-rw-r--r--   0        0        0    15031 2024-04-30 16:09:15.300428 tespy-0.7.4/src/tespy/components/nodes/drum.py
+-rw-r--r--   0        0        0    17257 2024-04-30 16:09:15.301427 tespy-0.7.4/src/tespy/components/nodes/merge.py
+-rw-r--r--   0        0        0    11985 2024-04-30 16:09:15.301427 tespy-0.7.4/src/tespy/components/nodes/separator.py
+-rw-r--r--   0        0        0     6751 2024-04-30 16:09:15.301427 tespy-0.7.4/src/tespy/components/nodes/splitter.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.4/src/tespy/components/piping/__init__.py
+-rw-r--r--   0        0        0     5432 2024-04-30 16:09:15.302428 tespy-0.7.4/src/tespy/components/piping/pipe.py
+-rw-r--r--   0        0        0    13738 2024-04-30 16:09:15.302428 tespy-0.7.4/src/tespy/components/piping/valve.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.4/src/tespy/components/reactors/__init__.py
+-rw-r--r--   0        0        0    27837 2024-04-30 16:09:15.303426 tespy-0.7.4/src/tespy/components/reactors/fuel_cell.py
+-rw-r--r--   0        0        0    40322 2024-04-30 16:09:15.303426 tespy-0.7.4/src/tespy/components/reactors/water_electrolyzer.py
+-rw-r--r--   0        0        0     2343 2024-04-16 16:42:16.672483 tespy-0.7.4/src/tespy/components/subsystem.py
+-rw-r--r--   0        0        0       21 2021-10-04 06:28:48.000000 tespy-0.7.4/src/tespy/components/turbomachinery/__init__.py
+-rw-r--r--   0        0        0     8555 2024-04-30 16:09:15.304427 tespy-0.7.4/src/tespy/components/turbomachinery/base.py
+-rw-r--r--   0        0        0    25881 2024-04-30 16:09:15.304427 tespy-0.7.4/src/tespy/components/turbomachinery/compressor.py
+-rw-r--r--   0        0        0    19230 2024-04-30 16:09:15.304427 tespy-0.7.4/src/tespy/components/turbomachinery/pump.py
+-rw-r--r--   0        0        0    19188 2024-04-30 16:09:15.305427 tespy-0.7.4/src/tespy/components/turbomachinery/turbine.py
+-rw-r--r--   0        0        0      147 2022-01-28 07:48:36.000000 tespy-0.7.4/src/tespy/connections/__init__.py
+-rw-r--r--   0        0        0    16918 2024-04-16 16:42:16.688064 tespy-0.7.4/src/tespy/connections/bus.py
+-rw-r--r--   0        0        0    44576 2024-04-19 10:46:21.778853 tespy-0.7.4/src/tespy/connections/connection.py
+-rw-r--r--   0        0        0     9270 2023-11-14 11:35:05.528493 tespy-0.7.4/src/tespy/data/ChemEx/Ahrendts.json
+-rw-r--r--   0        0        0     8407 2023-11-14 11:35:05.530494 tespy-0.7.4/src/tespy/data/ChemEx/Szargut1988.json
+-rw-r--r--   0        0        0     8578 2023-11-14 11:35:05.532488 tespy-0.7.4/src/tespy/data/ChemEx/Szargut2007.json
+-rw-r--r--   0        0        0     8047 2021-10-04 06:28:48.000000 tespy-0.7.4/src/tespy/data/char_lines.json
+-rw-r--r--   0        0        0     3726 2021-10-04 06:28:48.000000 tespy-0.7.4/src/tespy/data/char_maps.json
+-rw-r--r--   0        0        0      118 2022-01-28 07:48:36.000000 tespy-0.7.4/src/tespy/networks/__init__.py
+-rw-r--r--   0        0        0   107185 2024-04-30 16:09:15.306426 tespy-0.7.4/src/tespy/networks/network.py
+-rw-r--r--   0        0        0    13366 2024-04-30 16:09:15.306426 tespy-0.7.4/src/tespy/networks/network_reader.py
+-rw-r--r--   0        0        0      940 2024-04-16 16:42:16.703690 tespy-0.7.4/src/tespy/tools/__init__.py
+-rw-r--r--   0        0        0    38453 2024-04-16 16:42:16.703690 tespy-0.7.4/src/tespy/tools/analyses.py
+-rw-r--r--   0        0        0    17442 2024-04-30 16:09:15.307426 tespy-0.7.4/src/tespy/tools/characteristics.py
+-rw-r--r--   0        0        0    17346 2024-04-19 10:46:21.789831 tespy-0.7.4/src/tespy/tools/data_containers.py
+-rw-r--r--   0        0        0    38786 2024-04-16 16:42:16.719318 tespy-0.7.4/src/tespy/tools/document_models.py
+-rw-r--r--   0        0        0     1046 2024-04-16 16:42:16.719318 tespy-0.7.4/src/tespy/tools/fluid_properties/__init__.py
+-rw-r--r--   0        0        0     9666 2024-04-19 10:46:21.793788 tespy-0.7.4/src/tespy/tools/fluid_properties/functions.py
+-rw-r--r--   0        0        0     9700 2024-04-19 10:46:21.796827 tespy-0.7.4/src/tespy/tools/fluid_properties/helpers.py
+-rw-r--r--   0        0        0    12386 2024-04-19 10:46:21.801787 tespy-0.7.4/src/tespy/tools/fluid_properties/mixtures.py
+-rw-r--r--   0        0        0    13577 2024-04-30 16:09:15.308426 tespy-0.7.4/src/tespy/tools/fluid_properties/wrappers.py
+-rw-r--r--   0        0        0     3454 2024-04-19 10:46:21.809837 tespy-0.7.4/src/tespy/tools/global_vars.py
+-rw-r--r--   0        0        0    20301 2024-04-19 10:46:21.813784 tespy-0.7.4/src/tespy/tools/helpers.py
+-rw-r--r--   0        0        0    15049 2024-04-16 16:42:16.734942 tespy-0.7.4/src/tespy/tools/logger.py
+-rw-r--r--   0        0        0    10421 2024-04-16 16:42:16.734942 tespy-0.7.4/src/tespy/tools/optimization.py
+-rw-r--r--   0        0        0      427 2024-04-16 16:42:16.734942 tespy-0.7.4/tests/test_advanced_tutorials.py
+-rw-r--r--   0        0        0     4337 2024-04-16 16:42:16.740965 tespy-0.7.4/tests/test_analyses/test_entropy_analysis.py
+-rw-r--r--   0        0        0    24440 2024-04-16 16:42:16.740965 tespy-0.7.4/tests/test_analyses/test_exergy_analysis.py
+-rw-r--r--   0        0        0      315 2024-04-16 16:42:16.740965 tespy-0.7.4/tests/test_basic_tutorials.py
+-rw-r--r--   0        0        0    10214 2024-04-16 16:42:16.740965 tespy-0.7.4/tests/test_busses.py
+-rw-r--r--   0        0        0    11728 2024-04-16 16:42:16.740965 tespy-0.7.4/tests/test_components/test_combustion.py
+-rw-r--r--   0        0        0      346 2024-04-16 16:42:16.740965 tespy-0.7.4/tests/test_components/test_customs.py
+-rw-r--r--   0        0        0     1627 2024-04-16 16:42:16.757142 tespy-0.7.4/tests/test_components/test_drum.py
+-rw-r--r--   0        0        0    23305 2024-04-16 16:42:16.757142 tespy-0.7.4/tests/test_components/test_heat_exchangers.py
+-rw-r--r--   0        0        0     4028 2024-04-16 16:42:16.757142 tespy-0.7.4/tests/test_components/test_merge.py
+-rw-r--r--   0        0        0     3150 2024-04-16 16:42:16.757142 tespy-0.7.4/tests/test_components/test_piping.py
+-rw-r--r--   0        0        0     7107 2024-04-16 16:42:16.757142 tespy-0.7.4/tests/test_components/test_reactors.py
+-rw-r--r--   0        0        0    17021 2024-04-16 16:42:16.757142 tespy-0.7.4/tests/test_components/test_turbomachinery.py
+-rw-r--r--   0        0        0     4025 2024-04-16 16:42:16.772797 tespy-0.7.4/tests/test_connections.py
+-rw-r--r--   0        0        0    20109 2024-04-19 10:46:21.817783 tespy-0.7.4/tests/test_errors.py
+-rw-r--r--   0        0        0      455 2024-04-16 16:42:16.772797 tespy-0.7.4/tests/test_heat_pump_exergy.py
+-rw-r--r--   0        0        0      996 2023-11-14 11:35:05.574460 tespy-0.7.4/tests/test_models/cgam-ebsilon-results.csv
+-rw-r--r--   0        0        0     7604 2024-04-16 16:42:16.772797 tespy-0.7.4/tests/test_models/test_CGAM_model.py
+-rw-r--r--   0        0        0    12500 2024-04-16 16:42:16.772797 tespy-0.7.4/tests/test_models/test_heat_pump_model.py
+-rw-r--r--   0        0        0    18609 2024-04-19 10:46:21.822788 tespy-0.7.4/tests/test_models/test_solar_energy_generating_system.py
+-rw-r--r--   0        0        0     1664 2024-04-16 16:42:16.772797 tespy-0.7.4/tests/test_networks/test_binary_incompressible.py
+-rw-r--r--   0        0        0     5571 2024-04-16 16:42:16.788418 tespy-0.7.4/tests/test_networks/test_mixing_rules.py
+-rw-r--r--   0        0        0    24711 2024-04-19 10:46:21.825824 tespy-0.7.4/tests/test_networks/test_network.py
+-rw-r--r--   0        0        0     7897 2024-04-30 16:09:15.309426 tespy-0.7.4/tests/test_tools/test_characteristics.py
+-rw-r--r--   0        0        0    12983 2024-04-16 16:42:16.788418 tespy-0.7.4/tests/test_tools/test_fluid_properties/test_coolprop.py
+-rw-r--r--   0        0        0     2106 2024-04-16 16:42:16.788418 tespy-0.7.4/tests/test_tools/test_fluid_properties/test_iapws.py
+-rw-r--r--   0        0        0     1385 2024-04-16 16:42:16.788418 tespy-0.7.4/tests/test_tools/test_fluid_properties/test_pyromat.py
+-rw-r--r--   0        0        0     2237 2024-04-16 16:42:16.788418 tespy-0.7.4/tests/test_tools/test_helpers.py
+-rw-r--r--   0        0        0     2000 2024-04-16 16:42:16.788418 tespy-0.7.4/tox.ini
+-rw-r--r--   0        0        0      261 2024-04-16 16:42:16.804041 tespy-0.7.4/tutorial/README.rst
+-rw-r--r--   0        0        0     9727 2024-04-16 16:42:16.804041 tespy-0.7.4/tutorial/advanced/optimization_example.py
+-rw-r--r--   0        0        0     9541 2024-04-16 16:42:16.804041 tespy-0.7.4/tutorial/advanced/starting_values.py
+-rw-r--r--   0        0        0     6090 2024-04-16 16:42:16.804041 tespy-0.7.4/tutorial/advanced/stepwise.py
+-rw-r--r--   0        0        0     4264 2024-04-16 16:42:16.804041 tespy-0.7.4/tutorial/basics/district_heating.py
+-rw-r--r--   0        0        0     4978 2024-04-16 16:42:16.804041 tespy-0.7.4/tutorial/basics/gas_turbine.py
+-rw-r--r--   0        0        0     3216 2024-04-16 16:42:16.819668 tespy-0.7.4/tutorial/basics/heat_pump.py
+-rw-r--r--   0        0        0     4661 2024-04-16 16:42:16.819668 tespy-0.7.4/tutorial/basics/rankine.py
+-rw-r--r--   0        0        0     4201 2024-04-16 16:42:16.819668 tespy-0.7.4/tutorial/heat_pump_exergy/NH3.py
+-rw-r--r--   0        0        0    10920 2024-04-16 16:42:16.819668 tespy-0.7.4/tutorial/heat_pump_exergy/NH3_calculations.py
+-rw-r--r--   0        0        0     4217 2024-04-16 16:42:16.819668 tespy-0.7.4/tutorial/heat_pump_exergy/R410A.py
+-rw-r--r--   0        0        0    10943 2024-04-16 16:42:16.819668 tespy-0.7.4/tutorial/heat_pump_exergy/R410A_calculations.py
+-rw-r--r--   0        0        0     8277 2024-04-16 16:42:16.819668 tespy-0.7.4/tutorial/heat_pump_exergy/plots.py
+-rw-r--r--   0        0        0    10587 1970-01-01 00:00:00.000000 tespy-0.7.4/PKG-INFO
```

### Comparing `tespy-0.7.3/.pep8speaks.yml` & `tespy-0.7.4/.pep8speaks.yml`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/CODE_OF_CONDUCT.md` & `tespy-0.7.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/LICENSE` & `tespy-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/PULL_REQUEST_TEMPLATE.md` & `tespy-0.7.4/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/README.rst` & `tespy-0.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/advanced/exergy/flowsheet.svg` & `tespy-0.7.4/docs/_static/images/advanced/exergy/flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/advanced/exergy/flowsheet_darkmode.svg` & `tespy-0.7.4/docs/_static/images/advanced/exergy/flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/advanced/exergy/sankey.svg` & `tespy-0.7.4/docs/_static/images/advanced/exergy/sankey.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/district_heating.svg` & `tespy-0.7.4/docs/_static/images/basics/district_heating.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/district_heating_darkmode.svg` & `tespy-0.7.4/docs/_static/images/basics/district_heating_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/district_heating_partload.svg` & `tespy-0.7.4/docs/_static/images/basics/district_heating_partload.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/district_heating_partload_darkmode.svg` & `tespy-0.7.4/docs/_static/images/basics/district_heating_partload_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/gas_turbine.svg` & `tespy-0.7.4/docs/_static/images/basics/gas_turbine.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/gas_turbine_darkmode.svg` & `tespy-0.7.4/docs/_static/images/basics/gas_turbine_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/gas_turbine_fuel_composition.svg` & `tespy-0.7.4/docs/_static/images/basics/gas_turbine_fuel_composition.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/gas_turbine_fuel_composition_darkmode.svg` & `tespy-0.7.4/docs/_static/images/basics/gas_turbine_fuel_composition_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/gas_turbine_oxygen.svg` & `tespy-0.7.4/docs/_static/images/basics/gas_turbine_oxygen.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/gas_turbine_oxygen_darkmode.svg` & `tespy-0.7.4/docs/_static/images/basics/gas_turbine_oxygen_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/gas_turbine_parametric.svg` & `tespy-0.7.4/docs/_static/images/basics/gas_turbine_parametric.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/gas_turbine_parametric_darkmode.svg` & `tespy-0.7.4/docs/_static/images/basics/gas_turbine_parametric_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/heat_pump.svg` & `tespy-0.7.4/docs/_static/images/basics/heat_pump.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/heat_pump_darkmode.svg` & `tespy-0.7.4/docs/_static/images/basics/heat_pump_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/heat_pump_parametric.svg` & `tespy-0.7.4/docs/_static/images/basics/heat_pump_parametric.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/heat_pump_parametric_darkmode.svg` & `tespy-0.7.4/docs/_static/images/basics/heat_pump_parametric_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/modeling_concept.svg` & `tespy-0.7.4/docs/_static/images/basics/modeling_concept.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/rankine_cycle.svg` & `tespy-0.7.4/docs/_static/images/basics/rankine_cycle.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/rankine_cycle_darkmode.svg` & `tespy-0.7.4/docs/_static/images/basics/rankine_cycle_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/rankine_parametric.svg` & `tespy-0.7.4/docs/_static/images/basics/rankine_parametric.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/rankine_parametric_darkmode.svg` & `tespy-0.7.4/docs/_static/images/basics/rankine_parametric_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/rankine_partload.svg` & `tespy-0.7.4/docs/_static/images/basics/rankine_partload.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/basics/rankine_partload_darkmode.svg` & `tespy-0.7.4/docs/_static/images/basics/rankine_partload_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/examples/GRC_flowsheet.svg` & `tespy-0.7.4/docs/_static/images/examples/GRC_flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/examples/GRC_flowsheet_darkmode.svg` & `tespy-0.7.4/docs/_static/images/examples/GRC_flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/examples/ORC_parametric_flowsheet.svg` & `tespy-0.7.4/docs/_static/images/examples/ORC_parametric_flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/examples/ORC_parametric_flowsheet_darkmode.svg` & `tespy-0.7.4/docs/_static/images/examples/ORC_parametric_flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/examples/PM_CAES_graphical-abstract.svg` & `tespy-0.7.4/docs/_static/images/examples/PM_CAES_graphical-abstract.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/examples/PM_CAES_graphical-abstract_darkmode.svg` & `tespy-0.7.4/docs/_static/images/examples/PM_CAES_graphical-abstract_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/logo_tespy_big.svg` & `tespy-0.7.4/docs/_static/images/logo_tespy_big.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/logo_tespy_big_darkmode.svg` & `tespy-0.7.4/docs/_static/images/logo_tespy_big_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/logo_tespy_big_editable_font.svg` & `tespy-0.7.4/docs/_static/images/logo_tespy_big_editable_font.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/logo_tespy_mid.svg` & `tespy-0.7.4/docs/_static/images/logo_tespy_mid.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/logo_tespy_mid_christmas.svg` & `tespy-0.7.4/docs/_static/images/logo_tespy_mid_christmas.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/logo_tespy_mid_darkmode.svg` & `tespy-0.7.4/docs/_static/images/logo_tespy_mid_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/logo_tespy_mid_darkmode_christmas.svg` & `tespy-0.7.4/docs/_static/images/logo_tespy_mid_darkmode_christmas.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/logo_tespy_mid_editable_font.svg` & `tespy-0.7.4/docs/_static/images/logo_tespy_mid_editable_font.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/logo_tespy_mini.svg` & `tespy-0.7.4/docs/_static/images/logo_tespy_mini.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/logo_tespy_small.svg` & `tespy-0.7.4/docs/_static/images/logo_tespy_small.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/Ts_diagram_states.svg` & `tespy-0.7.4/docs/_static/images/modules/Ts_diagram_states.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/characteristics.svg` & `tespy-0.7.4/docs/_static/images/modules/characteristics.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/characteristics_darkmode.svg` & `tespy-0.7.4/docs/_static/images/modules/characteristics_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/connections.svg` & `tespy-0.7.4/docs/_static/images/modules/connections.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/connections_darkmode.svg` & `tespy-0.7.4/docs/_static/images/modules/connections_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/fluid_properties.svg` & `tespy-0.7.4/docs/_static/images/modules/fluid_properties.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/fluid_properties_darkmode.svg` & `tespy-0.7.4/docs/_static/images/modules/fluid_properties_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/logph_diagram_states.svg` & `tespy-0.7.4/docs/_static/images/modules/logph_diagram_states.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/subsystem_waste_heat_generator.svg` & `tespy-0.7.4/docs/_static/images/modules/subsystem_waste_heat_generator.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/subsystem_waste_heat_generator_darkmode.svg` & `tespy-0.7.4/docs/_static/images/modules/subsystem_waste_heat_generator_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/ude.svg` & `tespy-0.7.4/docs/_static/images/modules/ude.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/modules/ude_darkmode.svg` & `tespy-0.7.4/docs/_static/images/modules/ude_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs.svg` & `tespy-0.7.4/docs/_static/images/tutorials/district_heating_system/dhs.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_closed.svg` & `tespy-0.7.4/docs/_static/images/tutorials/district_heating_system/dhs_closed.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_forks.svg` & `tespy-0.7.4/docs/_static/images/tutorials/district_heating_system/dhs_forks.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/district_heating_system/dhs_open.svg` & `tespy-0.7.4/docs/_static/images/tutorials/district_heating_system/dhs_open.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/NH3_logph.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/NH3_logph.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/NH3_sankey.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/NH3_sankey.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_E_D_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Q_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_cop_eps_Tgeo_Ths_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/diagram_eps_Tamb_Tgeo_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/flowsheet.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_exergy/flowsheet_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_exergy/flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_starting_values/COP_by_wf_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_starting_values/flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_starting_values/logph.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_starting_values/logph.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p1_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/heat_pump_stepwise/flowsheet_p2_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/osmses-2023.svg` & `tespy-0.7.4/docs/_static/images/tutorials/osmses-2023.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/osmses-2023_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/osmses-2023_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/flowsheet.svg` & `tespy-0.7.4/docs/_static/images/tutorials/pygmo_optimization/flowsheet.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/flowsheet_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/pygmo_optimization/flowsheet_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization.svg` & `tespy-0.7.4/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization_darkmode.svg` & `tespy-0.7.4/docs/_static/images/tutorials/pygmo_optimization/pygmo_optimization_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/_static/js/custom.js` & `tespy-0.7.4/docs/_static/js/custom.js`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/advanced/exergy.rst` & `tespy-0.7.4/docs/advanced/exergy.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api.rst` & `tespy-0.7.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/CombustionChamber.svg` & `tespy-0.7.4/docs/api/_images/CombustionChamber.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/CombustionChamber_darkmode.svg` & `tespy-0.7.4/docs/api/_images/CombustionChamber_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/CombustionEngine.svg` & `tespy-0.7.4/docs/api/_images/CombustionEngine.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/CombustionEngine_darkmode.svg` & `tespy-0.7.4/docs/api/_images/CombustionEngine_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Compressor.svg` & `tespy-0.7.4/docs/api/_images/Compressor.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Compressor_darkmode.svg` & `tespy-0.7.4/docs/api/_images/Compressor_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Condenser.svg` & `tespy-0.7.4/docs/api/_images/Condenser.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Condenser_darkmode.svg` & `tespy-0.7.4/docs/api/_images/Condenser_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/DropletSeparator.svg` & `tespy-0.7.4/docs/api/_images/DropletSeparator.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/DropletSeparator_darkmode.svg` & `tespy-0.7.4/docs/api/_images/DropletSeparator_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Drum.svg` & `tespy-0.7.4/docs/api/_images/Drum.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Drum_darkmode.svg` & `tespy-0.7.4/docs/api/_images/Drum_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/FuelCell.svg` & `tespy-0.7.4/docs/api/_images/FuelCell.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/FuelCell_darkmode.svg` & `tespy-0.7.4/docs/api/_images/FuelCell_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/HeatExchanger.svg` & `tespy-0.7.4/docs/api/_images/HeatExchanger.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/HeatExchanger_darkmode.svg` & `tespy-0.7.4/docs/api/_images/HeatExchanger_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Merge.svg` & `tespy-0.7.4/docs/api/_images/Merge.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Merge_darkmode.svg` & `tespy-0.7.4/docs/api/_images/Merge_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/ORCEvaporator.svg` & `tespy-0.7.4/docs/api/_images/ORCEvaporator.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/ParabolicTrough.svg` & `tespy-0.7.4/docs/api/_images/ParabolicTrough.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/ParabolicTrough_darkmode.svg` & `tespy-0.7.4/docs/api/_images/ParabolicTrough_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Pipe.svg` & `tespy-0.7.4/docs/api/_images/Pipe.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Pipe_darkmode.svg` & `tespy-0.7.4/docs/api/_images/Pipe_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Pump.svg` & `tespy-0.7.4/docs/api/_images/Pump.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Pump_darkmode.svg` & `tespy-0.7.4/docs/api/_images/Pump_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/SolarCollector.svg` & `tespy-0.7.4/docs/api/_images/SolarCollector.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/SolarCollector_darkmode.svg` & `tespy-0.7.4/docs/api/_images/SolarCollector_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Splitter.svg` & `tespy-0.7.4/docs/api/_images/Splitter.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Splitter_darkmode.svg` & `tespy-0.7.4/docs/api/_images/Splitter_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/SubsystemInterface.svg` & `tespy-0.7.4/docs/api/_images/SubsystemInterface.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/SubsystemInterface_darkmode.svg` & `tespy-0.7.4/docs/api/_images/SubsystemInterface_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Turbine.svg` & `tespy-0.7.4/docs/api/_images/Turbine.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Turbine_darkmode.svg` & `tespy-0.7.4/docs/api/_images/Turbine_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Valve.svg` & `tespy-0.7.4/docs/api/_images/Valve.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/Valve_darkmode.svg` & `tespy-0.7.4/docs/api/_images/Valve_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/WaterElectrolyzer.svg` & `tespy-0.7.4/docs/api/_images/WaterElectrolyzer.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/WaterElectrolyzer_darkmode.svg` & `tespy-0.7.4/docs/api/_images/WaterElectrolyzer_darkmode.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/combustion_engine_Q1_char_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/combustion_engine_Q1_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/combustion_engine_Q2_char_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/combustion_engine_Q2_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/combustion_engine_Qloss_char_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/combustion_engine_Qloss_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/combustion_engine_tiP_char_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/combustion_engine_tiP_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/compressor_char_map_eta_s_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/compressor_char_map_eta_s_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/compressor_char_map_pr_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/compressor_char_map_pr_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/compressor_eta_s_char_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/compressor_eta_s_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/condenser_kA_char1_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/condenser_kA_char1_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/condenser_kA_char2_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/condenser_kA_char2_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/desuperheater_kA_char1_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/desuperheater_kA_char1_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/desuperheater_kA_char2_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/desuperheater_kA_char2_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char1_CONDENSING_FLUID.svg` & `tespy-0.7.4/docs/api/_images/heat_exchanger_kA_char1_CONDENSING_FLUID.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char1_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/heat_exchanger_kA_char1_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char2_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/heat_exchanger_kA_char2_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/heat_exchanger_kA_char2_EVAPORATING_FLUID.svg` & `tespy-0.7.4/docs/api/_images/heat_exchanger_kA_char2_EVAPORATING_FLUID.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/heat_exchanger_simple_kA_char_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/heat_exchanger_simple_kA_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/pipe_kA_char_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/pipe_kA_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/pump_eta_s_char_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/pump_eta_s_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/turbine_eta_s_char_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/turbine_eta_s_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/turbine_eta_s_char_TRAUPEL.svg` & `tespy-0.7.4/docs/api/_images/turbine_eta_s_char_TRAUPEL.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/_images/water_electrolyzer_eta_char_DEFAULT.svg` & `tespy-0.7.4/docs/api/_images/water_electrolyzer_eta_char_DEFAULT.svg`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/components.rst` & `tespy-0.7.4/docs/api/components.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/data.rst` & `tespy-0.7.4/docs/api/data.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/api/tools.rst` & `tespy-0.7.4/docs/api/tools.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/basics.rst` & `tespy-0.7.4/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/basics/district_heating.rst` & `tespy-0.7.4/docs/basics/district_heating.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/basics/gas_turbine.rst` & `tespy-0.7.4/docs/basics/gas_turbine.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/basics/heat_pump.rst` & `tespy-0.7.4/docs/basics/heat_pump.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/basics/intro.rst` & `tespy-0.7.4/docs/basics/intro.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/basics/rankine_cycle.rst` & `tespy-0.7.4/docs/basics/rankine_cycle.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/benchmarks.rst` & `tespy-0.7.4/docs/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/conf.py` & `tespy-0.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/development/how.rst` & `tespy-0.7.4/docs/development/how.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/development/what.rst` & `tespy-0.7.4/docs/development/what.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/examples.rst` & `tespy-0.7.4/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/index.rst` & `tespy-0.7.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/installation.rst` & `tespy-0.7.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/introduction.rst` & `tespy-0.7.4/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/modules.rst` & `tespy-0.7.4/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/modules/characteristics.rst` & `tespy-0.7.4/docs/modules/characteristics.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/modules/components.rst` & `tespy-0.7.4/docs/modules/components.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/modules/connections.rst` & `tespy-0.7.4/docs/modules/connections.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/modules/fluid_properties.rst` & `tespy-0.7.4/docs/modules/fluid_properties.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/modules/networks.rst` & `tespy-0.7.4/docs/modules/networks.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/modules/ude.rst` & `tespy-0.7.4/docs/modules/ude.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/references.bib` & `tespy-0.7.4/docs/references.bib`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/regular_meeting.rst` & `tespy-0.7.4/docs/regular_meeting.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/scripts/generate_tespy_data_module.py` & `tespy-0.7.4/docs/scripts/generate_tespy_data_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import tespy
 
 
 def get_char_data(filename):
     path = resource_filename('tespy.data', filename + '.json')
 
     with open(path) as f:
-        data = json.loads(f.read())
+        data = json.load(f)
 
     return data
 
 
 def plot_line(component, parameter, name, data):
 
     char = tespy.tools.characteristics.CharLine(x=data['x'], y=data['y'])
```

### Comparing `tespy-0.7.3/docs/tutorials.rst` & `tespy-0.7.4/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/tutorials/district_heating.rst` & `tespy-0.7.4/docs/tutorials/district_heating.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/tutorials/heat_pump_exergy.rst` & `tespy-0.7.4/docs/tutorials/heat_pump_exergy.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/tutorials/heat_pump_steps.rst` & `tespy-0.7.4/docs/tutorials/heat_pump_steps.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/tutorials/pygmo_optimization.rst` & `tespy-0.7.4/docs/tutorials/pygmo_optimization.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/tutorials/starting_values.rst` & `tespy-0.7.4/docs/tutorials/starting_values.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new.rst` & `tespy-0.7.4/docs/whats_new.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 What's New
 ~~~~~~~~~~
 
 Discover notable new features and improvements in each release
 
+.. include::  whats_new/v0-7-4.rst
 .. include::  whats_new/v0-7-3.rst
 .. include::  whats_new/v0-7-2.rst
 .. include::  whats_new/v0-7-1.rst
 .. include::  whats_new/v0-7-0.rst
 .. include::  whats_new/v0-6-3.rst
 .. include::  whats_new/v0-6-2.rst
 .. include::  whats_new/v0-6-1.rst
```

### Comparing `tespy-0.7.3/docs/whats_new/v0-0-2.rst` & `tespy-0.7.4/docs/whats_new/v0-0-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-0-3.rst` & `tespy-0.7.4/docs/whats_new/v0-0-3.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-0-4.rst` & `tespy-0.7.4/docs/whats_new/v0-0-4.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-0-5.rst` & `tespy-0.7.4/docs/whats_new/v0-0-5.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-1-0.rst` & `tespy-0.7.4/docs/whats_new/v0-1-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-1-1.rst` & `tespy-0.7.4/docs/whats_new/v0-1-1.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-1-2.rst` & `tespy-0.7.4/docs/whats_new/v0-1-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-1-3.rst` & `tespy-0.7.4/docs/whats_new/v0-1-3.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-1-4.rst` & `tespy-0.7.4/docs/whats_new/v0-1-4.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-2-0.rst` & `tespy-0.7.4/docs/whats_new/v0-2-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-2-1.rst` & `tespy-0.7.4/docs/whats_new/v0-2-1.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-2-2.rst` & `tespy-0.7.4/docs/whats_new/v0-2-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-3-0.rst` & `tespy-0.7.4/docs/whats_new/v0-3-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-3-2.rst` & `tespy-0.7.4/docs/whats_new/v0-3-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-3-3.rst` & `tespy-0.7.4/docs/whats_new/v0-3-3.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-3-4.rst` & `tespy-0.7.4/docs/whats_new/v0-3-4.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-4-0.rst` & `tespy-0.7.4/docs/whats_new/v0-4-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-4-1.rst` & `tespy-0.7.4/docs/whats_new/v0-4-1.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-4-2.rst` & `tespy-0.7.4/docs/whats_new/v0-4-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-4-3-001.rst` & `tespy-0.7.4/docs/whats_new/v0-4-3-001.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-4-3-003.rst` & `tespy-0.7.4/docs/whats_new/v0-4-3-003.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-4-3.rst` & `tespy-0.7.4/docs/whats_new/v0-4-3.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-4-4.rst` & `tespy-0.7.4/docs/whats_new/v0-4-4.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-5-0.rst` & `tespy-0.7.4/docs/whats_new/v0-5-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-5-1.rst` & `tespy-0.7.4/docs/whats_new/v0-5-1.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-6-0.rst` & `tespy-0.7.4/docs/whats_new/v0-6-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-6-1.rst` & `tespy-0.7.4/docs/whats_new/v0-6-1.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-6-3.rst` & `tespy-0.7.4/docs/whats_new/v0-6-3.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-7-0.rst` & `tespy-0.7.4/docs/whats_new/v0-7-0.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/docs/whats_new/v0-7-2.rst` & `tespy-0.7.4/docs/whats_new/v0-7-2.rst`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/paper.bib` & `tespy-0.7.4/paper.bib`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/paper.md` & `tespy-0.7.4/paper.md`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/pyproject.toml` & `tespy-0.7.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "tests/",
     "tutorial/",
 ]
 exclude = ["docs/_build"]
 
 [project]
 name = "tespy"
-version = "0.7.3"
+version = "0.7.4"
 description = "Thermal Engineering Systems in Python (TESPy)"
 readme = "README.rst"
 authors = [
     {name = "Francesco Witte", email = "tespy@witte.sh"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `tespy-0.7.3/src/tespy/__init__.py` & `tespy-0.7.4/src/tespy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8
 import importlib.resources
 import os
 
 __datapath__ = os.path.join(importlib.resources.files("tespy"), "data")
-__version__ = '0.7.3 - Newton\'s Nature'
+__version__ = '0.7.4 - Newton\'s Nature'
 
 # tespy data and connections import
 from . import connections  # noqa: F401
 from . import data  # noqa: F401
 # tespy components imports
 from .components import basics  # noqa: F401
 from .components import combustion  # noqa: F401
```

### Comparing `tespy-0.7.3/src/tespy/components/__init__.py` & `tespy-0.7.4/src/tespy/components/__init__.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/components/basics/cycle_closer.py` & `tespy-0.7.4/src/tespy/components/basics/cycle_closer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 SPDX-License-Identifier: MIT
 """
 
 import numpy as np
 
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 
-# %%
-
 
+@component_registry
 class CycleCloser(Component):
     r"""
     Component for closing cycles.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.basics.cycle_closer.CycleCloser.pressure_equality_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/basics/sink.py` & `tespy-0.7.4/src/tespy/components/basics/sink.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 
 SPDX-License-Identifier: MIT
 """
 
 import numpy as np
 
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 
 
+@component_registry
 class Sink(Component):
     r"""
     A flow drains in a Sink.
 
     Parameters
     ----------
     label : str
```

### Comparing `tespy-0.7.3/src/tespy/components/basics/source.py` & `tespy-0.7.4/src/tespy/components/basics/source.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 
 SPDX-License-Identifier: MIT
 """
 
 import numpy as np
 
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 
 
+@component_registry
 class Source(Component):
     r"""
     A flow originates from a Source.
 
     Parameters
     ----------
     label : str
```

### Comparing `tespy-0.7.3/src/tespy/components/basics/subsystem_interface.py` & `tespy-0.7.4/src/tespy/components/basics/subsystem_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 available from its original location
 tespy/components/basics/subsystem_interface.py
 
 SPDX-License-Identifier: MIT
 """
 
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 from tespy.tools.data_containers import SimpleDataContainer as dc_simple
 
 
+@component_registry
 class SubsystemInterface(Component):
     r"""
     The subsystem interface does not change fluid properties.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.component.Component.fluid_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/combustion/base.py` & `tespy-0.7.4/src/tespy/components/combustion/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 """
 import itertools
 
 import CoolProp.CoolProp as CP
 import numpy as np
 
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 from tespy.tools import logger
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import h_mix_pT
 from tespy.tools.fluid_properties import s_mix_pT
 from tespy.tools.fluid_properties.helpers import fluid_structure
 from tespy.tools.global_vars import combustion_gases
 from tespy.tools.helpers import TESPyComponentError
 from tespy.tools.helpers import fluidalias_in_list
 
 
+@component_registry
 class CombustionChamber(Component):
     r"""
     The class CombustionChamber is parent class of all combustion components.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.combustion.base.CombustionChamber.mass_flow_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/combustion/diabatic.py` & `tespy-0.7.4/src/tespy/components/combustion/diabatic.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 
 SPDX-License-Identifier: MIT
 """
 
 import numpy as np
 
 from tespy.components import CombustionChamber
+from tespy.components.component import component_registry
 from tespy.tools import logger
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import h_mix_pT
 
 
+@component_registry
 class DiabaticCombustionChamber(CombustionChamber):
     r"""
     The class CombustionChamber is parent class of all combustion components.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.combustion.base.CombustionChamber.mass_flow_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/combustion/engine.py` & `tespy-0.7.4/src/tespy/components/combustion/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 This file is part of project TESPy (github.com/oemof/tespy). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location
 tespy/components/combustion/engine.py
 
 SPDX-License-Identifier: MIT
 """
+
 import numpy as np
 
 from tespy.components.combustion.base import CombustionChamber
+from tespy.components.component import component_registry
 from tespy.tools import logger
 from tespy.tools.data_containers import ComponentCharacteristics as dc_cc
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.data_containers import SimpleDataContainer as dc_simple
 from tespy.tools.document_models import generate_latex_eq
-from tespy.tools.fluid_properties import h_mix_pT
 from tespy.tools.fluid_properties import s_mix_ph
 from tespy.tools.fluid_properties import s_mix_pT
 
 
+@component_registry
 class CombustionEngine(CombustionChamber):
     r"""
     An internal combustion engine supplies power and heat cogeneration.
 
     The combustion engine produces power and heat in cogeneration from fuel
     combustion. The combustion properties are identical to the combustion
     chamber. Thermal input and power output, heat output and heat losses are
```

### Comparing `tespy-0.7.3/src/tespy/components/component.py` & `tespy-0.7.4/src/tespy/components/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,23 @@
 from tespy.tools.global_vars import ERR
 from tespy.tools.helpers import _numeric_deriv
 from tespy.tools.helpers import bus_char_derivative
 from tespy.tools.helpers import bus_char_evaluation
 from tespy.tools.helpers import newton_with_kwargs
 
 
+def component_registry(type):
+    component_registry.items[type.__name__] = type
+    return type
+
+
+component_registry.items = {}
+
+
+@component_registry
 class Component:
     r"""
     Class Component is the base class of all TESPy components.
 
     Parameters
     ----------
     label : str
```

### Comparing `tespy-0.7.3/src/tespy/components/heat_exchangers/base.py` & `tespy-0.7.4/src/tespy/components/heat_exchangers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 tespy/components/heat_exchangers/base.py
 
 SPDX-License-Identifier: MIT
 """
 import numpy as np
 
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 from tespy.tools.data_containers import ComponentCharacteristics as dc_cc
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.data_containers import GroupedComponentCharacteristics as dc_gcc
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import h_mix_pT
 from tespy.tools.fluid_properties import s_mix_ph
 
 
+@component_registry
 class HeatExchanger(Component):
     r"""
     Class for counter current heat exchanger.
 
     The component HeatExchanger is the parent class for the components:
 
     - :py:class:`tespy.components.heat_exchangers.condenser.Condenser`
```

### Comparing `tespy-0.7.3/src/tespy/components/heat_exchangers/condenser.py` & `tespy-0.7.4/src/tespy/components/heat_exchangers/condenser.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 tespy/components/heat_exchangers/condenser.py
 
 SPDX-License-Identifier: MIT
 """
 
 import numpy as np
 
+from tespy.components.component import component_registry
 from tespy.components.heat_exchangers.base import HeatExchanger
 from tespy.tools.data_containers import ComponentCharacteristics as dc_cc
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.data_containers import GroupedComponentCharacteristics as dc_gcc
 from tespy.tools.data_containers import SimpleDataContainer as dc_simple
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import dh_mix_dpQ
 from tespy.tools.fluid_properties import h_mix_pQ
 
 
+@component_registry
 class Condenser(HeatExchanger):
     r"""
     A Condenser cools a fluid until it is in liquid state.
 
     The condensing fluid is cooled by the cold side fluid. The fluid on the hot
     side of the condenser must be pure. Subcooling is available.
```

### Comparing `tespy-0.7.3/src/tespy/components/heat_exchangers/desuperheater.py` & `tespy-0.7.4/src/tespy/components/heat_exchangers/desuperheater.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 by the contributors recorded in the version control history of the file,
 available from its original location
 tespy/components/heat_exchangers/desuperheater.py
 
 SPDX-License-Identifier: MIT
 """
 
+from tespy.components.component import component_registry
 from tespy.components.heat_exchangers.base import HeatExchanger
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import dh_mix_dpQ
 from tespy.tools.fluid_properties import h_mix_pQ
 
 
+@component_registry
 class Desuperheater(HeatExchanger):
     r"""
     The Desuperheater cools a fluid to the saturated gas state.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.heat_exchangers.base.HeatExchanger.energy_balance_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/heat_exchangers/parabolic_trough.py` & `tespy-0.7.4/src/tespy/components/heat_exchangers/parabolic_trough.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 by the contributors recorded in the version control history of the file,
 available from its original location
 tespy/components/heat_exchangers/parabolic_trough.py
 
 SPDX-License-Identifier: MIT
 """
 
-import numpy as np
-
+from tespy.components.component import component_registry
 from tespy.components.heat_exchangers.simple import SimpleHeatExchanger
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.data_containers import GroupedComponentProperties as dc_gcp
-from tespy.tools.data_containers import SimpleDataContainer as dc_simple
 from tespy.tools.document_models import generate_latex_eq
 
 
+@component_registry
 class ParabolicTrough(SimpleHeatExchanger):
     r"""
     The ParabolicTrough calculates heat output from irradiance.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.component.Component.fluid_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/heat_exchangers/simple.py` & `tespy-0.7.4/src/tespy/components/heat_exchangers/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 """
 
 import warnings
 
 import numpy as np
 
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 from tespy.tools import logger
 from tespy.tools.data_containers import ComponentCharacteristics as dc_cc
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.data_containers import GroupedComponentProperties as dc_gcp
 from tespy.tools.data_containers import SimpleDataContainer as dc_simple
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import s_mix_ph
 from tespy.tools.fluid_properties.helpers import darcy_friction_factor as dff
 from tespy.tools.helpers import convert_to_SI
 
 
+@component_registry
 class SimpleHeatExchanger(Component):
     r"""
     A basic heat exchanger representing a heat source or heat sink.
 
     The component SimpleHeatExchanger is the parent class for the components:
 
     - :py:class:`tespy.components.heat_exchangers.solar_collector.SolarCollector`
```

### Comparing `tespy-0.7.3/src/tespy/components/heat_exchangers/solar_collector.py` & `tespy-0.7.4/src/tespy/components/heat_exchangers/solar_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 by the contributors recorded in the version control history of the file,
 available from its original location
 tespy/components/heat_exchangers/solar_collector.py
 
 SPDX-License-Identifier: MIT
 """
 
-import numpy as np
-
+from tespy.components.component import component_registry
 from tespy.components.heat_exchangers.simple import SimpleHeatExchanger
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.data_containers import GroupedComponentProperties as dc_gcp
-from tespy.tools.data_containers import SimpleDataContainer as dc_simple
 from tespy.tools.document_models import generate_latex_eq
 
 
+@component_registry
 class SolarCollector(SimpleHeatExchanger):
     r"""
     The solar collector calculates heat output from irradiance.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.component.Component.fluid_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/nodes/base.py` & `tespy-0.7.4/src/tespy/components/nodes/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 This file is part of project TESPy (github.com/oemof/tespy). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location tespy/components/nodes/base.py
 
 SPDX-License-Identifier: MIT
 """
 
-import numpy as np
-
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 from tespy.tools.document_models import generate_latex_eq
 
 
+@component_registry
 class NodeBase(Component):
     """Class NodeBase is parent class for all components of submodule nodes."""
 
     def mass_flow_func(self):
         r"""
         Calculate the residual value for mass flow balance equation.
```

### Comparing `tespy-0.7.3/src/tespy/components/nodes/droplet_separator.py` & `tespy-0.7.4/src/tespy/components/nodes/droplet_separator.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 This file is part of project TESPy (github.com/oemof/tespy). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location
 tespy/components/nodes/droplet_separator.py
 
 SPDX-License-Identifier: MIT
 """
+
+from tespy.components.component import component_registry
 from tespy.components.nodes.base import NodeBase
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import dh_mix_dpQ
 from tespy.tools.fluid_properties import h_mix_pQ
 
 
+@component_registry
 class DropletSeparator(NodeBase):
     r"""
     Separate liquid phase from gas phase of a single fluid.
 
     This component is the parent component of the Drum.
 
     **Mandatory Equations**
```

### Comparing `tespy-0.7.3/src/tespy/components/nodes/drum.py` & `tespy-0.7.4/src/tespy/components/nodes/drum.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 available from its original location tespy/components/nodes/drum.py
 
 SPDX-License-Identifier: MIT
 """
 
 import numpy as np
 
+from tespy.components.component import component_registry
 from tespy.components.nodes.droplet_separator import DropletSeparator
 from tespy.tools.fluid_properties import h_mix_pQ
 
 
+@component_registry
 class Drum(DropletSeparator):
     r"""
     A drum separates saturated gas from saturated liquid.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.nodes.base.NodeBase.mass_flow_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/nodes/merge.py` & `tespy-0.7.4/src/tespy/components/nodes/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 available from its original location tespy/components/nodes/merge.py
 
 SPDX-License-Identifier: MIT
 """
 
 import numpy as np
 
+from tespy.components.component import component_registry
 from tespy.components.nodes.base import NodeBase
 from tespy.tools.data_containers import SimpleDataContainer as dc_simple
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import s_mix_pT
 
 
+@component_registry
 class Merge(NodeBase):
     r"""
     Class for merge points with multiple inflows and one outflow.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.nodes.base.NodeBase.mass_flow_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/nodes/separator.py` & `tespy-0.7.4/src/tespy/components/nodes/separator.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 This file is part of project TESPy (github.com/oemof/tespy). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location tespy/components/nodes/separator.py
 
 SPDX-License-Identifier: MIT
 """
 
-import numpy as np
-
+from tespy.components.component import component_registry
 from tespy.components.nodes.base import NodeBase
 from tespy.tools.data_containers import SimpleDataContainer as dc_simple
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import dT_mix_dph
 from tespy.tools.fluid_properties import dT_mix_pdh
 
 # from tespy.tools.fluid_properties import dT_mix_ph_dfluid
 
 
+@component_registry
 class Separator(NodeBase):
     r"""
     A separator separates fluid components from a mass flow.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.nodes.base.NodeBase.mass_flow_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/nodes/splitter.py` & `tespy-0.7.4/src/tespy/components/nodes/splitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 This file is part of project TESPy (github.com/oemof/tespy). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location tespy/components/nodes/splitter.py
 
 SPDX-License-Identifier: MIT
 """
 
-import numpy as np
-
+from tespy.components.component import component_registry
 from tespy.components.nodes.base import NodeBase
 from tespy.tools.data_containers import SimpleDataContainer as dc_simple
 from tespy.tools.document_models import generate_latex_eq
 
 
+@component_registry
 class Splitter(NodeBase):
     r"""
     Split up a mass flow in parts of identical enthalpy and fluid composition.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.nodes.base.NodeBase.mass_flow_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/piping/pipe.py` & `tespy-0.7.4/src/tespy/components/piping/pipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 This file is part of project TESPy (github.com/oemof/tespy). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location tespy/components/piping/pipe.py
 
 SPDX-License-Identifier: MIT
 """
 
+from tespy.components.component import component_registry
 from tespy.components.heat_exchangers.simple import SimpleHeatExchanger
 
 
+@component_registry
 class Pipe(SimpleHeatExchanger):
     r"""
     The Pipe is a subclass of a SimpleHeatExchanger.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.component.Component.fluid_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/piping/valve.py` & `tespy-0.7.4/src/tespy/components/piping/valve.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 
 SPDX-License-Identifier: MIT
 """
 
 import numpy as np
 
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 from tespy.tools import logger
 from tespy.tools.data_containers import ComponentCharacteristics as dc_cc
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.document_models import generate_latex_eq
 
 
+@component_registry
 class Valve(Component):
     r"""
     The Valve throttles a fluid without changing enthalpy.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.component.Component.fluid_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/reactors/fuel_cell.py` & `tespy-0.7.4/src/tespy/components/reactors/fuel_cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 This file is part of project TESPy (github.com/oemof/tespy). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location
 tespy/components/reactors/fuel_cell.py
 
 SPDX-License-Identifier: MIT
 """
-import numpy as np
 
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 from tespy.tools import logger
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import h_mix_pT
 
 
+@component_registry
 class FuelCell(Component):
     r"""
     The fuel cell produces power by oxidation of hydrogen.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.reactors.fuel_cell.FuelCell.fluid_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/reactors/water_electrolyzer.py` & `tespy-0.7.4/src/tespy/components/reactors/water_electrolyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 by the contributors recorded in the version control history of the file,
 available from its original location
 tespy/components/reactors/water_electrolyzer.py
 
 SPDX-License-Identifier: MIT
 """
 
-import numpy as np
-
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 from tespy.tools import logger
 from tespy.tools.data_containers import ComponentCharacteristics as dc_cc
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import dT_mix_dph
 from tespy.tools.fluid_properties import dT_mix_pdh
 from tespy.tools.fluid_properties import h_mix_pT
 
 
+@component_registry
 class WaterElectrolyzer(Component):
     r"""
     The water electrolyzer produces hydrogen and oxygen from water and power.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.reactors.water_electrolyzer.WaterElectrolyzer.fluid_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/subsystem.py` & `tespy-0.7.4/src/tespy/components/subsystem.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/components/turbomachinery/base.py` & `tespy-0.7.4/src/tespy/components/turbomachinery/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 available from its original location
 tespy/components/turbomachinery/base.py
 
 SPDX-License-Identifier: MIT
 """
 
 from tespy.components.component import Component
+from tespy.components.component import component_registry
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.document_models import generate_latex_eq
 
 
+@component_registry
 class Turbomachine(Component):
     r"""
     Parent class for compressor, pump and turbine.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.component.Component.fluid_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/turbomachinery/compressor.py` & `tespy-0.7.4/src/tespy/components/turbomachinery/compressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 tespy/components/turbomachinery/compressor.py
 
 SPDX-License-Identifier: MIT
 """
 
 import numpy as np
 
+from tespy.components.component import component_registry
 from tespy.components.turbomachinery.base import Turbomachine
 from tespy.tools import logger
 from tespy.tools.data_containers import ComponentCharacteristicMaps as dc_cm
 from tespy.tools.data_containers import ComponentCharacteristics as dc_cc
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.data_containers import GroupedComponentProperties as dc_gcp
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import isentropic
 
 
+@component_registry
 class Compressor(Turbomachine):
     r"""
     Class for axial or radial compressor.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.component.Component.fluid_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/turbomachinery/pump.py` & `tespy-0.7.4/src/tespy/components/turbomachinery/pump.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 available from its original location tespy/components/turbomachinery/pump.py
 
 SPDX-License-Identifier: MIT
 """
 
 import numpy as np
 
+from tespy.components.component import component_registry
 from tespy.components.turbomachinery.base import Turbomachine
 from tespy.tools import logger
 from tespy.tools.data_containers import ComponentCharacteristics as dc_cc
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import isentropic
 
 
+@component_registry
 class Pump(Turbomachine):
     r"""
     Class for axial or radial pumps.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.component.Component.fluid_func`
```

### Comparing `tespy-0.7.3/src/tespy/components/turbomachinery/turbine.py` & `tespy-0.7.4/src/tespy/components/turbomachinery/turbine.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 This file is part of project TESPy (github.com/oemof/tespy). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location tespy/components/turbomachinery/turbine.py
 
 SPDX-License-Identifier: MIT
 """
 
-
 import numpy as np
 
+from tespy.components.component import component_registry
 from tespy.components.turbomachinery.base import Turbomachine
 from tespy.tools import logger
 from tespy.tools.data_containers import ComponentCharacteristics as dc_cc
 from tespy.tools.data_containers import ComponentProperties as dc_cp
 from tespy.tools.data_containers import SimpleDataContainer as dc_simple
 from tespy.tools.document_models import generate_latex_eq
 from tespy.tools.fluid_properties import isentropic
 
 
+@component_registry
 class Turbine(Turbomachine):
     r"""
     Class for gas or steam turbines.
 
     **Mandatory Equations**
 
     - :py:meth:`tespy.components.component.Component.fluid_func`
```

### Comparing `tespy-0.7.3/src/tespy/connections/bus.py` & `tespy-0.7.4/src/tespy/connections/bus.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/connections/connection.py` & `tespy-0.7.4/src/tespy/connections/connection.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/data/ChemEx/Ahrendts.json` & `tespy-0.7.4/src/tespy/data/ChemEx/Ahrendts.json`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/data/ChemEx/Szargut1988.json` & `tespy-0.7.4/src/tespy/data/ChemEx/Szargut1988.json`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/data/ChemEx/Szargut2007.json` & `tespy-0.7.4/src/tespy/data/ChemEx/Szargut2007.json`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/data/char_lines.json` & `tespy-0.7.4/src/tespy/data/char_lines.json`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/data/char_maps.json` & `tespy-0.7.4/src/tespy/data/char_maps.json`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/networks/network.py` & `tespy-0.7.4/src/tespy/networks/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -2707,15 +2707,15 @@
 
         Parameters
         ----------
         fn : str
             Path/filename for the network configuration file.
         """
         with open(fn + 'network.json', 'w') as f:
-            f.write(json.dumps(self._serialize(), indent=4))
+            json.dump(self._serialize(), f, indent=4)
 
         logger.debug('Network information saved to %s.', fn)
 
     def save_connections(self, fn):
         r"""
         Save the connection properties.
 
@@ -2754,40 +2754,40 @@
         """
         if len(self.busses) > 0:
             bus_data = {}
             for label, bus in self.busses.items():
                 bus_data[label] = self.results[label]["design value"].to_dict()
             fn = fn + 'busses.json'
             with open(fn, "w", encoding="utf-8") as f:
-                f.write(json.dumps(bus_data, indent=4))
+                json.dump(bus_data, f, indent=4)
             logger.debug('Bus information saved to %s.', fn)
 
     def export_connections(self, fn):
         connections = {}
         for c in self.conns["object"]:
             connections.update(c._serialize())
 
         fn = fn + "connections.json"
         with open(fn, "w", encoding="utf-8") as f:
-            f.write(json.dumps(connections, indent=4).replace("NaN", "null"))
+            json.dump(connections, f, indent=4)
         logger.debug('Connection information exported to %s.', fn)
 
     def export_components(self, fn):
         for c in self.comps["comp_type"].unique():
             components = {}
             for cp in self.comps.loc[self.comps["comp_type"] == c, "object"]:
                 components.update(cp._serialize())
 
             fname = f"{fn}{c}.json"
             with open(fname, "w", encoding="utf-8") as f:
-                f.write(json.dumps(components, indent=4).replace("NaN", "null"))
+                json.dump(components, f, indent=4)
             logger.debug('Component information exported to %s.', fname)
 
     def export_busses(self, fn):
         if len(self.busses) > 0:
             busses = {}
             for bus in self.busses.values():
                 busses.update(bus._serialize())
             fn = fn + 'busses.json'
             with open(fn, "w", encoding="utf-8") as f:
-                f.write(json.dumps(busses, indent=4).replace("NaN", "null"))
+                json.dump(busses, f, indent=4)
             logger.debug('Bus information exported to %s.', fn)
```

### Comparing `tespy-0.7.3/src/tespy/networks/network_reader.py` & `tespy-0.7.4/src/tespy/networks/network_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,91 +8,33 @@
 
 This file is part of project TESPy (github.com/oemof/tespy). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location tespy/networks/network_reader.py
 
 SPDX-License-Identifier: MIT
 """
+import importlib
 import json
 import os
 
-import pandas as pd
-
-from tespy.components import CombustionChamber
-from tespy.components import CombustionEngine
-from tespy.components import Compressor
-from tespy.components import Condenser
-from tespy.components import CycleCloser
-from tespy.components import Desuperheater
-from tespy.components import DropletSeparator
-from tespy.components import Drum
-from tespy.components import HeatExchanger
-from tespy.components import HeatExchangerSimple
-from tespy.components import Merge
-from tespy.components import ParabolicTrough
-from tespy.components import Pipe
-from tespy.components import Pump
-from tespy.components import Separator
-from tespy.components import SimpleHeatExchanger
-from tespy.components import Sink
-from tespy.components import SolarCollector
-from tespy.components import Source
-from tespy.components import Splitter
-from tespy.components import SubsystemInterface
-from tespy.components import Turbine
-from tespy.components import Valve
-from tespy.components import WaterElectrolyzer
+from tespy.components.component import component_registry
 from tespy.connections import Bus
 from tespy.connections import Connection
 from tespy.connections import Ref
 from tespy.networks.network import Network
 from tespy.tools import logger
 from tespy.tools.characteristics import CharLine
 from tespy.tools.characteristics import CharMap
 from tespy.tools.data_containers import ComponentCharacteristicMaps as dc_cm
 from tespy.tools.data_containers import ComponentCharacteristics as dc_cc
 from tespy.tools.data_containers import DataContainer as dc
 from tespy.tools.data_containers import FluidProperties as dc_prop
-from tespy.tools.fluid_properties.wrappers import CoolPropWrapper
-from tespy.tools.fluid_properties.wrappers import IAPWSWrapper
-from tespy.tools.fluid_properties.wrappers import PyromatWrapper
+from tespy.tools.fluid_properties.wrappers import wrapper_registry
 from tespy.tools.helpers import modify_path_os
 
-COMP_TARGET_CLASSES = {
-    'CycleCloser': CycleCloser,
-    'Sink': Sink,
-    'Source': Source,
-    'SubsystemInterface': SubsystemInterface,
-    'CombustionChamber': CombustionChamber,
-    'CombustionEngine': CombustionEngine,
-    'Condenser': Condenser,
-    'Desuperheater': Desuperheater,
-    'HeatExchanger': HeatExchanger,
-    'HeatExchangerSimple': HeatExchangerSimple,
-    'SimpleHeatExchanger': SimpleHeatExchanger,
-    'SolarCollector': SolarCollector,
-    'ParabolicTrough': ParabolicTrough,
-    'DropletSeparator': DropletSeparator,
-    'Drum': Drum,
-    'Merge': Merge,
-    'Separator': Separator,
-    'Splitter': Splitter,
-    'Pipe': Pipe,
-    'Valve': Valve,
-    'WaterElectrolyzer': WaterElectrolyzer,
-    'Compressor': Compressor,
-    'Pump': Pump,
-    'Turbine': Turbine
-}
-
-ENGINE_TARGET_CLASSES = {
-    "CoolPropWrapper": CoolPropWrapper,
-    "IAPWSWrapper": IAPWSWrapper,
-    "PyromatWrapper": PyromatWrapper,
-}
 
 def load_network(path):
     r"""
     Load a network from a base path.
 
     Parameters
     ----------
@@ -241,42 +183,46 @@
 
     msg = 'Reading network data from base path ' + path + '.'
     logger.info(msg)
 
     # load components
     comps = {}
 
+    module_name = "tespy.components"
+    module = importlib.import_module(module_name)
+
     files = os.listdir(path_comps)
     for f in files:
         fn = path_comps + f
         component = f.replace(".json", "")
 
         msg = f"Reading component data ({component}) from {fn}."
         logger.debug(msg)
 
         with open(path_comps + f, "r", encoding="utf-8") as c:
-            data = json.loads(c.read())
+            data = json.load(c)
 
-        comps.update(construct_components(component, data))
+        target_class = component_registry.items[component]
+        comps.update(_construct_components(target_class, data))
 
     msg = 'Created network components.'
     logger.info(msg)
 
     # create network
-    nw = construct_network(path)
+    nw = _construct_network(path)
 
     # load connections
     fn = path + 'connections.json'
     msg = f"Reading connection data from {fn}."
     logger.debug(msg)
 
     with open(fn, "r", encoding="utf-8") as c:
-        data = json.loads(c.read())
+        data = json.load(c)
 
-    conns = construct_connections(data, comps)
+    conns = _construct_connections(data, comps)
 
     # add connections to network
     for c in conns.values():
         nw.add_conns(c)
 
     msg = 'Created connections.'
     logger.info(msg)
@@ -285,17 +231,17 @@
     fn = path + 'busses.json'
     if os.path.isfile(fn):
 
         msg = f"Reading bus data from {fn}."
         logger.debug(msg)
 
         with open(fn, "r", encoding="utf-8") as c:
-            data = json.loads(c.read())
+            data = json.load(c)
 
-        busses = construct_busses(data, comps)
+        busses = _construct_busses(data, comps)
         # add busses to network
         for b in busses.values():
             nw.add_busses(b)
 
         msg = 'Created busses.'
         logger.info(msg)
 
@@ -307,15 +253,15 @@
     logger.info(msg)
 
     nw.check_network()
 
     return nw
 
 
-def construct_components(component, data):
+def _construct_components(target_class, data):
     r"""
     Create TESPy component from class name and set parameters.
 
     Parameters
     ----------
     component : str
         Name of the component class to be constructed.
@@ -324,35 +270,35 @@
         Dictionary with component information.
 
     Returns
     -------
     dict
         Dictionary of all components of the specified type.
     """
-    target_class = COMP_TARGET_CLASSES[component]
     instances = {}
     for cp, cp_data in data.items():
         instances[cp] = target_class(cp)
         for param, param_data in cp_data.items():
             container = instances[cp].get_attr(param)
             if isinstance(container, dc):
-                if isinstance(container, dc_cc):
-                    param_data["char_func"] = CharLine(**param_data["char_func"])
-                elif isinstance(container, dc_cm):
-                    param_data["char_func"] = CharMap(**param_data["char_func"])
+                if "char_func" in param_data:
+                    if isinstance(container, dc_cc):
+                        param_data["char_func"] = CharLine(**param_data["char_func"])
+                    elif isinstance(container, dc_cm):
+                        param_data["char_func"] = CharMap(**param_data["char_func"])
                 if isinstance(container, dc_prop):
                     param_data["val0"] = param_data["val"]
                 container.set_attr(**param_data)
             else:
                 instances[cp].set_attr(**{param: param_data})
 
     return instances
 
 
-def construct_network(path):
+def _construct_network(path):
     r"""
     Create TESPy network from the path provided by the user.
 
     Parameters
     ----------
     path : str
         Base-path to stored network data.
@@ -360,21 +306,21 @@
     Returns
     -------
     nw : tespy.networks.network.Network
         TESPy network object.
     """
     # read network .json-file
     with open(path + 'network.json', 'r') as f:
-        data = json.loads(f.read())
+        data = json.load(f)
 
     # create network object with its properties
     return Network(**data)
 
 
-def construct_connections(data, comps):
+def _construct_connections(data, comps):
     r"""
     Create TESPy connection from data in the .json-file and its parameters.
 
     Parameters
     ----------
     data : dict
         Dictionary with connection data.
@@ -391,44 +337,52 @@
 
     arglist = [
         _ for _ in data[list(data.keys())[0]]
         if _ not in ["source", "source_id", "target", "target_id", "label", "fluid"]
         and "ref" not in _
     ]
     arglist_ref = [_ for _ in data[list(data.keys())[0]] if "ref" in _]
+
+    module_name = "tespy.tools.fluid_properties.wrappers"
+    module = importlib.import_module(module_name)
+
     for label, conn in data.items():
         conns[label] = Connection(
             comps[conn["source"]], conn["source_id"],
             comps[conn["target"]], conn["target_id"],
             label=label
         )
         for arg in arglist:
             container = conns[label].get_attr(arg)
             if isinstance(container, dc):
                 container.set_attr(**conn[arg])
             else:
                 conns[label].set_attr(**{arg: conn[arg]})
 
         for f, engine in conn["fluid"]["engine"].items():
-            conn["fluid"]["engine"][f] = ENGINE_TARGET_CLASSES[engine]
+            conn["fluid"]["engine"][f] = wrapper_registry.items[engine]
 
         conns[label].fluid.set_attr(**conn["fluid"])
         conns[label]._create_fluid_wrapper()
 
     for label, conn in data.items():
         for arg in arglist_ref:
             if len(conn[arg]) > 0:
                 param = arg.replace("_ref", "")
-                ref = Ref(conns[conn[arg]["conn"]], conn[arg]["factor"], conn[arg]["delta"])
+                ref = Ref(
+                    conns[conn[arg]["conn"]],
+                    conn[arg]["factor"],
+                    conn[arg]["delta"]
+                )
                 conns[label].set_attr(**{param: ref})
 
     return conns
 
 
-def construct_busses(data, comps):
+def _construct_busses(data, comps):
     r"""
     Create busses of the network.
 
     Parameters
     ----------
     data : dict
         Bus information from .json file.
```

### Comparing `tespy-0.7.3/src/tespy/tools/__init__.py` & `tespy-0.7.4/src/tespy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/tools/analyses.py` & `tespy-0.7.4/src/tespy/tools/analyses.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/tools/characteristics.py` & `tespy-0.7.4/src/tespy/tools/characteristics.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
     """
     if char_type == CharLine:
         path = os.path.join(__datapath__, 'char_lines.json')
     else:
         path = os.path.join(__datapath__, 'char_maps.json')
 
     with open(path) as f:
-        data = json.loads(f.read())
+        data = json.load(f)
 
     if char_type == CharLine:
         x = data[component][parameter][function_name]['x']
         y = data[component][parameter][function_name]['y']
         obj = CharLine(x, y)
 
     else:
@@ -542,15 +542,15 @@
         path = os.path.join(path, 'char_lines.json')
     else:
         path = os.path.join(path, 'char_maps.json')
 
     if os.path.isfile(path):
 
         with open(path) as f:
-            data = json.loads(f.read())
+            data = json.load(f)
 
         if char_type == CharLine:
             x = data[name]['x']
             y = data[name]['y']
             obj = CharLine(x, y)
 
         else:
```

### Comparing `tespy-0.7.3/src/tespy/tools/data_containers.py` & `tespy-0.7.4/src/tespy/tools/data_containers.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/tools/document_models.py` & `tespy-0.7.4/src/tespy/tools/document_models.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/tools/fluid_properties/__init__.py` & `tespy-0.7.4/src/tespy/tools/fluid_properties/__init__.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/tools/fluid_properties/functions.py` & `tespy-0.7.4/src/tespy/tools/fluid_properties/functions.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/tools/fluid_properties/helpers.py` & `tespy-0.7.4/src/tespy/tools/fluid_properties/helpers.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/tools/fluid_properties/mixtures.py` & `tespy-0.7.4/src/tespy/tools/fluid_properties/mixtures.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/tools/fluid_properties/wrappers.py` & `tespy-0.7.4/src/tespy/tools/fluid_properties/wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,24 +12,33 @@
 """
 
 import CoolProp as CP
 
 from tespy.tools.global_vars import ERR
 
 
+def wrapper_registry(type):
+    wrapper_registry.items[type.__name__] = type
+    return type
+
+
+wrapper_registry.items = {}
+
+
 class SerializableAbstractState(CP.AbstractState):
 
     def __init__(self, back_end, fluid_name):
         self.back_end = back_end
         self.fluid_name = fluid_name
 
     def __reduce__(self):
         return (self.__class__, (self.back_end, self.fluid_name))
 
 
+@wrapper_registry
 class FluidPropertyWrapper:
 
     def __init__(self, fluid, back_end=None) -> None:
         """Base class for fluid property wrappers
 
         Parameters
         ----------
@@ -102,14 +111,15 @@
     def s_ph(self, p, h):
         self._not_implemented()
 
     def s_pT(self, p, T):
         self._not_implemented()
 
 
+@wrapper_registry
 class CoolPropWrapper(FluidPropertyWrapper):
 
     def __init__(self, fluid, back_end=None) -> None:
         """Wrapper for CoolProp.CoolProp.AbstractState instance calls
 
         Parameters
         ----------
@@ -244,14 +254,15 @@
         return self.AS.smass()
 
     def s_pT(self, p, T):
         self.AS.update(CP.PT_INPUTS, p, T)
         return self.AS.smass()
 
 
+@wrapper_registry
 class IAPWSWrapper(FluidPropertyWrapper):
 
 
     def __init__(self, fluid, back_end=None) -> None:
         """Wrapper for iapws library calls
 
         Parameters
@@ -362,14 +373,15 @@
     def s_ph(self, p, h):
         return self.AS(P=p / 1e6, h=h / 1e3).s * 1e3
 
     def s_pT(self, p, T):
         return self.AS(P=p / 1e6, T=T).s * 1e3
 
 
+@wrapper_registry
 class PyromatWrapper(FluidPropertyWrapper):
 
     def __init__(self, fluid, back_end=None) -> None:
         """_summary_
 
         Parameters
         ----------
```

### Comparing `tespy-0.7.3/src/tespy/tools/global_vars.py` & `tespy-0.7.4/src/tespy/tools/global_vars.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/tools/helpers.py` & `tespy-0.7.4/src/tespy/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/tools/logger.py` & `tespy-0.7.4/src/tespy/tools/logger.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/src/tespy/tools/optimization.py` & `tespy-0.7.4/src/tespy/tools/optimization.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_analyses/test_entropy_analysis.py` & `tespy-0.7.4/tests/test_analyses/test_entropy_analysis.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_analyses/test_exergy_analysis.py` & `tespy-0.7.4/tests/test_analyses/test_exergy_analysis.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_busses.py` & `tespy-0.7.4/tests/test_busses.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_components/test_combustion.py` & `tespy-0.7.4/tests/test_components/test_combustion.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_components/test_drum.py` & `tespy-0.7.4/tests/test_components/test_drum.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_components/test_heat_exchangers.py` & `tespy-0.7.4/tests/test_components/test_heat_exchangers.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_components/test_merge.py` & `tespy-0.7.4/tests/test_components/test_merge.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_components/test_piping.py` & `tespy-0.7.4/tests/test_components/test_piping.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_components/test_reactors.py` & `tespy-0.7.4/tests/test_components/test_reactors.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_components/test_turbomachinery.py` & `tespy-0.7.4/tests/test_components/test_turbomachinery.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_connections.py` & `tespy-0.7.4/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_errors.py` & `tespy-0.7.4/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_models/cgam-ebsilon-results.csv` & `tespy-0.7.4/tests/test_models/cgam-ebsilon-results.csv`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_models/test_CGAM_model.py` & `tespy-0.7.4/tests/test_models/test_CGAM_model.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_models/test_heat_pump_model.py` & `tespy-0.7.4/tests/test_models/test_heat_pump_model.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_models/test_solar_energy_generating_system.py` & `tespy-0.7.4/tests/test_models/test_solar_energy_generating_system.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_networks/test_binary_incompressible.py` & `tespy-0.7.4/tests/test_networks/test_binary_incompressible.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_networks/test_mixing_rules.py` & `tespy-0.7.4/tests/test_networks/test_mixing_rules.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_networks/test_network.py` & `tespy-0.7.4/tests/test_networks/test_network.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_tools/test_characteristics.py` & `tespy-0.7.4/tests/test_tools/test_characteristics.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     tmp_path = extend_basic_path('tmp_dir_for_testing')
 
     if os.path.exists(path):
         for f in os.listdir(path):
             shutil.copy(src=path + '/' + f, dst=tmp_path)
 
     with open(data_path) as f:
-        raw_data = json.loads(f.read())
+        raw_data = json.load(f)
 
     data = raw_data['heat exchanger']['kA_char2']
     with open(os.path.join(path, 'char_lines.json'), 'w') as outfile:
         json.dump(data, outfile)
 
     char_original = load_default_char('heat exchanger', 'kA_char2',
                                       'EVAPORATING FLUID', CharLine)
@@ -80,15 +80,15 @@
     tmp_path = extend_basic_path('tmp_dir_for_testing')
 
     if os.path.exists(path):
         for f in os.listdir(path):
             shutil.copy(src=path + '/' + f, dst=tmp_path)
 
     with open(data_path) as f:
-        raw_data = json.loads(f.read())
+        raw_data = json.load(f)
 
     data = raw_data['compressor']['char_map_pr']
     with open(os.path.join(path, 'char_maps.json'), 'w') as outfile:
         json.dump(data, outfile)
 
     char_original = load_default_char(
         'compressor', 'char_map_pr', 'DEFAULT', CharMap)
```

### Comparing `tespy-0.7.3/tests/test_tools/test_fluid_properties/test_coolprop.py` & `tespy-0.7.4/tests/test_tools/test_fluid_properties/test_coolprop.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_tools/test_fluid_properties/test_iapws.py` & `tespy-0.7.4/tests/test_tools/test_fluid_properties/test_iapws.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_tools/test_fluid_properties/test_pyromat.py` & `tespy-0.7.4/tests/test_tools/test_fluid_properties/test_pyromat.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tests/test_tools/test_helpers.py` & `tespy-0.7.4/tests/test_tools/test_helpers.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tox.ini` & `tespy-0.7.4/tox.ini`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/advanced/optimization_example.py` & `tespy-0.7.4/tutorial/advanced/optimization_example.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/advanced/starting_values.py` & `tespy-0.7.4/tutorial/advanced/starting_values.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/advanced/stepwise.py` & `tespy-0.7.4/tutorial/advanced/stepwise.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/basics/district_heating.py` & `tespy-0.7.4/tutorial/basics/district_heating.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/basics/gas_turbine.py` & `tespy-0.7.4/tutorial/basics/gas_turbine.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/basics/heat_pump.py` & `tespy-0.7.4/tutorial/basics/heat_pump.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/basics/rankine.py` & `tespy-0.7.4/tutorial/basics/rankine.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/heat_pump_exergy/NH3.py` & `tespy-0.7.4/tutorial/heat_pump_exergy/NH3.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/heat_pump_exergy/NH3_calculations.py` & `tespy-0.7.4/tutorial/heat_pump_exergy/NH3_calculations.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/heat_pump_exergy/R410A.py` & `tespy-0.7.4/tutorial/heat_pump_exergy/R410A.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/heat_pump_exergy/R410A_calculations.py` & `tespy-0.7.4/tutorial/heat_pump_exergy/R410A_calculations.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/tutorial/heat_pump_exergy/plots.py` & `tespy-0.7.4/tutorial/heat_pump_exergy/plots.py`

 * *Files identical despite different names*

### Comparing `tespy-0.7.3/PKG-INFO` & `tespy-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tespy
-Version: 0.7.3
+Version: 0.7.4
 Summary: Thermal Engineering Systems in Python (TESPy)
 Author-email: Francesco Witte <tespy@witte.sh>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

