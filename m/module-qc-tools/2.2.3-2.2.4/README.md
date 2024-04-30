# Comparing `tmp/module_qc_tools-2.2.3.tar.gz` & `tmp/module_qc_tools-2.2.4.tar.gz`

## Comparing `module_qc_tools-2.2.3.tar` & `module_qc_tools-2.2.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/.gitmodules
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/tbump.toml
--rw-r--r--   0        0        0    30217 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/ADC_CALIBRATION/2024-04-11_144359/20UPGXM1234567.json
--rw-r--r--   0        0        0   321578 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/ANALOG_READBACK/2024-04-11_144351/20UPGXM1234567.json
--rw-r--r--   0        0        0    25387 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/DATA_TRANSMISSION/2024-04-11_144358/20UPGXM1234567.json
--rw-r--r--   0        0        0    23033 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/INJECTION_CAPACITANCE/2024-04-11_144353/20UPGXM1234567.json
--rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/IV_MEASURE/2024-04-11_144408/20UPGXM1234567.json
--rw-r--r--   0        0        0    27694 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/LP_MODE/2024-04-11_144406/20UPGXM1234567.json
--rw-r--r--   0        0        0    24110 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/OVERVOLTAGE_PROTECTION/2024-04-11_144333/20UPGXM1234567.json
--rw-r--r--   0        0        0    82000 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/SLDO/2024-04-11_144328/20UPGXM1234567.json
--rw-r--r--   0        0        0    35394 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/UNDERSHUNT_PROTECTION/2024-04-11_144338/20UPGXM1234567.json
--rw-r--r--   0        0        0   109866 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/VCAL_CALIBRATION/2024-04-11_144330/20UPGXM1234567.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/docs/.gitkeep
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/emulator/README.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/_version.py
--rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    25909 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/DATA_TRANSMISSION.py
--rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/IV_MEASURE.py
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/LP_MODE.py
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/SLDO.py
--rw-r--r--   0        0        0    11922 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/UNDERSHUNT_PROTECTION.py
--rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/__main__.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/globals.py
--rw-r--r--   0        0        0    23129 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/hardware_emulator.py
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/main.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/upload_localdb.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/configs/emulator_merged_vmux.json
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/configs/example_merged_vmux.json
--rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/configs/example_separate_vmux.json
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/module_state_template.json
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
--rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
--rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
--rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
--rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/controller/specCfg-rd53b.json
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/ANALOG_READBACK.json
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/DATA_TRANSMISSION.json
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/IV_MEASURE.json
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/LP_MODE.json
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/SLDO.json
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/UNDERSHUNT_PROTECTION.json
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
--rw-r--r--   0        0        0    30007 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/common.json
--rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/config.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/__init__.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/hardware_control_base.py
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/misc.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/multimeter.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/ntc.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/power_supply.py
--rw-r--r--   0        0        0    18004 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/yarr.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/tests/test_package.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/LICENSE
--rw-r--r--   0        0        0    39352 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/README.md
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/pyproject.toml
--rw-r--r--   0        0        0    41593 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/.gitmodules
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/tbump.toml
+-rw-r--r--   0        0        0    29426 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/Measurements/ADC_CALIBRATION/2024-04-30_161709/20UPGXM1234567.json
+-rw-r--r--   0        0        0   312150 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/Measurements/ANALOG_READBACK/2024-04-30_161711/20UPGXM1234567.json
+-rw-r--r--   0        0        0    25387 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/Measurements/DATA_TRANSMISSION/2024-04-30_161720/20UPGXM1234567.json
+-rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/Measurements/INJECTION_CAPACITANCE/2024-04-30_161710/20UPGXM1234567.json
+-rw-r--r--   0        0        0     9954 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/Measurements/IV_MEASURE/2024-04-30_161653/20UPGXM1234567.json
+-rw-r--r--   0        0        0    27366 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/Measurements/LP_MODE/2024-04-30_161730/20UPGXM1234567.json
+-rw-r--r--   0        0        0    23970 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/Measurements/OVERVOLTAGE_PROTECTION/2024-04-30_161656/20UPGXM1234567.json
+-rw-r--r--   0        0        0    75650 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/Measurements/SLDO/2024-04-30_161717/20UPGXM1234567.json
+-rw-r--r--   0        0        0    34470 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/Measurements/UNDERSHUNT_PROTECTION/2024-04-30_161717/20UPGXM1234567.json
+-rw-r--r--   0        0        0   105818 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/Measurements/VCAL_CALIBRATION/2024-04-30_161707/20UPGXM1234567.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/docs/.gitkeep
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/emulator/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/_version.py
+-rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    25909 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/DATA_TRANSMISSION.py
+-rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/LP_MODE.py
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    11922 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/UNDERSHUNT_PROTECTION.py
+-rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/__main__.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/globals.py
+-rw-r--r--   0        0        0    23129 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/hardware_emulator.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/main.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/cli/upload_localdb.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/configs/emulator_merged_vmux.json
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/configs/example_merged_vmux.json
+-rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/configs/example_separate_vmux.json
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/module_state_template.json
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
+-rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
+-rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
+-rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
+-rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/controller/specCfg-rd53b.json
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/ANALOG_READBACK.json
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/DATA_TRANSMISSION.json
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/IV_MEASURE.json
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/LP_MODE.json
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/SLDO.json
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/UNDERSHUNT_PROTECTION.json
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
+-rw-r--r--   0        0        0    30007 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/common.json
+-rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/data/schema/config.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/utils/__init__.py
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/utils/hardware_control_base.py
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/utils/misc.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/utils/multimeter.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/utils/ntc.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/utils/power_supply.py
+-rw-r--r--   0        0        0    18367 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/src/module_qc_tools/utils/yarr.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/tests/test_package.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/LICENSE
+-rw-r--r--   0        0        0    39352 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/README.md
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0    41593 2020-02-02 00:00:00.000000 module_qc_tools-2.2.4/PKG-INFO
```

### Comparing `module_qc_tools-2.2.3/.gitlab-ci.yml` & `module_qc_tools-2.2.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/.pre-commit-config.yaml` & `module_qc_tools-2.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/tbump.toml` & `module_qc_tools-2.2.4/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2232 2e32 2e33 220a 0a23 2045  t = "2.2.3"..# E
+00000010: 7420 3d20 2232 2e32 2e34 220a 0a23 2045  t = "2.2.4"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -15,15 +15,15 @@
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
 00000140: 6d70 2076 6572 7369 6f6e 3a20 322e 322e  mp version: 2.2.
-00000150: 3320 e286 9220 7b6e 6577 5f76 6572 7369  3 ... {new_versi
+00000150: 3420 e286 9220 7b6e 6577 5f76 6572 7369  4 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `module_qc_tools-2.2.3/Measurements/ADC_CALIBRATION/2024-04-11_144359/20UPGXM1234567.json` & `module_qc_tools-2.2.4/Measurements/LP_MODE/2024-04-30_161730/20UPGXM1234567.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8411948204428673%*

 * *Differences: {'0': "{0: {'testType': 'LP_MODE', 'results': {'property': {replace: "*

 * *      "OrderedDict([('LP_MODE_MEASUREMENT_VERSION', '2.2.4')])}, 'Measurements': {'Vmux30': "*

 * *      "{'Values': [0.0]}, 'Temperature': OrderedDict([('X', False), ('Unit', 'C'), ('Values', "*

 * *      "[29.2])]), 'SetCurrent': OrderedDict([('X', False), ('Unit', 'A'), ('Values', [2.1])]), "*

 * *      "'Current': OrderedDict([('X', True), ('Unit', 'A'), ('Values', [2.1])]), 'FailingPixels': "*

 * *      "OrderedDict([('X', False), ('Unit', 'Counts'), ( […]*

```diff
@@ -1,119 +1,113 @@
 [
     [
         {
             "results": {
                 "Measurements": {
-                    "ADC_Vmux30": {
-                        "Unit": "Count",
+                    "Current": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1
+                        ],
+                        "X": true
+                    },
+                    "FailingPixels": {
+                        "Unit": "Counts",
+                        "Values": [
+                            -1
+                        ],
+                        "X": false
+                    },
+                    "Imux0": {
+                        "Unit": "V",
+                        "Values": [
+                            0.04
+                        ],
+                        "X": false
+                    },
+                    "Imux28": {
+                        "Unit": "V",
+                        "Values": [
+                            0.125
+                        ],
+                        "X": false
+                    },
+                    "Imux29": {
+                        "Unit": "V",
+                        "Values": [
+                            0.02403846153846154
+                        ],
+                        "X": false
+                    },
+                    "Imux30": {
+                        "Unit": "V",
+                        "Values": [
+                            0.125
+                        ],
+                        "X": false
+                    },
+                    "Imux31": {
+                        "Unit": "V",
+                        "Values": [
+                            0.02403846153846154
+                        ],
+                        "X": false
+                    },
+                    "Imux63": {
+                        "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
                             0.0
                         ],
                         "X": false
                     },
-                    "ADC_Vmux8": {
-                        "Unit": "Count",
+                    "SetCurrent": {
+                        "Unit": "A",
                         "Values": [
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567
+                            2.1
                         ],
                         "X": false
                     },
-                    "DACs_input": {
-                        "Unit": "Count",
-                        "Values": [
-                            500.0,
-                            700.0,
-                            900.0,
-                            1100.0,
-                            1300.0,
-                            1500.0,
-                            1700.0,
-                            1900.0,
-                            2100.0,
-                            2300.0,
-                            2500.0,
-                            2700.0,
-                            2900.0,
-                            3100.0,
-                            3300.0
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            29.2
                         ],
-                        "X": true
+                        "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
-                    "Vmux8": {
-                        "Unit": "V",
-                        "Values": [
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux36": {
+                        "Unit": "V",
+                        "Values": [
+                            0.25
+                        ],
+                        "X": false
+                    },
+                    "Vmux37": {
+                        "Unit": "V",
+                        "Values": [
+                            0.29571345625
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 29.2,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -129,15 +123,14 @@
                                 "DiffPreampT": 500,
                                 "DiffPreampTL": 500,
                                 "DiffPreampTR": 500,
                                 "EnCoreCol0": 65535,
                                 "EnCoreCol1": 65535,
                                 "EnCoreCol2": 65535,
                                 "EnCoreCol3": 63,
-                                "InjVcalRange": 1,
                                 "MonitorI": 63,
                                 "MonitorV": 1,
                                 "SerEnLane": 4,
                                 "ServiceBlockEn": 1,
                                 "SldoTrimA": 3,
                                 "SldoTrimD": 4
                             },
@@ -171,138 +164,133 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846814,
-                    "TimeStart": 1712846641
+                    "TimeEnd": 1714494049,
+                    "TimeStart": 1714493850,
+                    "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.2.3"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
-            "testType": "ADC_CALIBRATION"
+            "testType": "LP_MODE"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
-                    "ADC_Vmux30": {
-                        "Unit": "Count",
+                    "Current": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1
+                        ],
+                        "X": true
+                    },
+                    "FailingPixels": {
+                        "Unit": "Counts",
+                        "Values": [
+                            -1
+                        ],
+                        "X": false
+                    },
+                    "Imux0": {
+                        "Unit": "V",
+                        "Values": [
+                            0.04
+                        ],
+                        "X": false
+                    },
+                    "Imux28": {
+                        "Unit": "V",
+                        "Values": [
+                            0.125
+                        ],
+                        "X": false
+                    },
+                    "Imux29": {
+                        "Unit": "V",
+                        "Values": [
+                            0.02403846153846154
+                        ],
+                        "X": false
+                    },
+                    "Imux30": {
+                        "Unit": "V",
+                        "Values": [
+                            0.125
+                        ],
+                        "X": false
+                    },
+                    "Imux31": {
+                        "Unit": "V",
+                        "Values": [
+                            0.02403846153846154
+                        ],
+                        "X": false
+                    },
+                    "Imux63": {
+                        "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
                             0.0
                         ],
                         "X": false
                     },
-                    "ADC_Vmux8": {
-                        "Unit": "Count",
+                    "SetCurrent": {
+                        "Unit": "A",
                         "Values": [
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705
+                            2.1
                         ],
                         "X": false
                     },
-                    "DACs_input": {
-                        "Unit": "Count",
-                        "Values": [
-                            500.0,
-                            700.0,
-                            900.0,
-                            1100.0,
-                            1300.0,
-                            1500.0,
-                            1700.0,
-                            1900.0,
-                            2100.0,
-                            2300.0,
-                            2500.0,
-                            2700.0,
-                            2900.0,
-                            3100.0,
-                            3300.0
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            29.2
                         ],
-                        "X": true
+                        "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
-                    "Vmux8": {
-                        "Unit": "V",
-                        "Values": [
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux36": {
+                        "Unit": "V",
+                        "Values": [
+                            0.25
+                        ],
+                        "X": false
+                    },
+                    "Vmux37": {
+                        "Unit": "V",
+                        "Values": [
+                            0.29571345625
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 29.2,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -318,15 +306,14 @@
                                 "DiffPreampT": 500,
                                 "DiffPreampTL": 500,
                                 "DiffPreampTR": 500,
                                 "EnCoreCol0": 65535,
                                 "EnCoreCol1": 65535,
                                 "EnCoreCol2": 65535,
                                 "EnCoreCol3": 63,
-                                "InjVcalRange": 1,
                                 "MonitorI": 63,
                                 "MonitorV": 1,
                                 "SerEnLane": 1,
                                 "ServiceBlockEn": 1,
                                 "SldoTrimA": 4,
                                 "SldoTrimD": 3
                             },
@@ -360,138 +347,133 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846814,
-                    "TimeStart": 1712846641
+                    "TimeEnd": 1714494049,
+                    "TimeStart": 1714493851,
+                    "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.2.3"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
-            "testType": "ADC_CALIBRATION"
+            "testType": "LP_MODE"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
-                    "ADC_Vmux30": {
-                        "Unit": "Count",
+                    "Current": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1
+                        ],
+                        "X": true
+                    },
+                    "FailingPixels": {
+                        "Unit": "Counts",
+                        "Values": [
+                            -1
+                        ],
+                        "X": false
+                    },
+                    "Imux0": {
+                        "Unit": "V",
+                        "Values": [
+                            0.04
+                        ],
+                        "X": false
+                    },
+                    "Imux28": {
+                        "Unit": "V",
+                        "Values": [
+                            0.125
+                        ],
+                        "X": false
+                    },
+                    "Imux29": {
+                        "Unit": "V",
+                        "Values": [
+                            0.02403846153846154
+                        ],
+                        "X": false
+                    },
+                    "Imux30": {
+                        "Unit": "V",
+                        "Values": [
+                            0.125
+                        ],
+                        "X": false
+                    },
+                    "Imux31": {
+                        "Unit": "V",
+                        "Values": [
+                            0.02403846153846154
+                        ],
+                        "X": false
+                    },
+                    "Imux63": {
+                        "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
                             0.0
                         ],
                         "X": false
                     },
-                    "ADC_Vmux8": {
-                        "Unit": "Count",
+                    "SetCurrent": {
+                        "Unit": "A",
                         "Values": [
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933
+                            2.1
                         ],
                         "X": false
                     },
-                    "DACs_input": {
-                        "Unit": "Count",
-                        "Values": [
-                            500.0,
-                            700.0,
-                            900.0,
-                            1100.0,
-                            1300.0,
-                            1500.0,
-                            1700.0,
-                            1900.0,
-                            2100.0,
-                            2300.0,
-                            2500.0,
-                            2700.0,
-                            2900.0,
-                            3100.0,
-                            3300.0
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            29.2
                         ],
-                        "X": true
+                        "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
-                    "Vmux8": {
-                        "Unit": "V",
-                        "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux36": {
+                        "Unit": "V",
+                        "Values": [
+                            0.25
+                        ],
+                        "X": false
+                    },
+                    "Vmux37": {
+                        "Unit": "V",
+                        "Values": [
+                            0.29571345625
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 29.2,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -507,15 +489,14 @@
                                 "DiffPreampT": 500,
                                 "DiffPreampTL": 500,
                                 "DiffPreampTR": 500,
                                 "EnCoreCol0": 65535,
                                 "EnCoreCol1": 65535,
                                 "EnCoreCol2": 65535,
                                 "EnCoreCol3": 65535,
-                                "InjVcalRange": 1,
                                 "MonitorI": 63,
                                 "MonitorV": 1,
                                 "SerEnLane": 8,
                                 "ServiceBlockEn": 1,
                                 "SldoTrimA": 12,
                                 "SldoTrimD": 8
                             },
@@ -549,138 +530,133 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846814,
-                    "TimeStart": 1712846641
+                    "TimeEnd": 1714494049,
+                    "TimeStart": 1714493851,
+                    "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.2.3"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
-            "testType": "ADC_CALIBRATION"
+            "testType": "LP_MODE"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
-                    "ADC_Vmux30": {
-                        "Unit": "Count",
+                    "Current": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1
+                        ],
+                        "X": true
+                    },
+                    "FailingPixels": {
+                        "Unit": "Counts",
+                        "Values": [
+                            -1
+                        ],
+                        "X": false
+                    },
+                    "Imux0": {
+                        "Unit": "V",
+                        "Values": [
+                            0.04
+                        ],
+                        "X": false
+                    },
+                    "Imux28": {
+                        "Unit": "V",
+                        "Values": [
+                            0.125
+                        ],
+                        "X": false
+                    },
+                    "Imux29": {
+                        "Unit": "V",
+                        "Values": [
+                            0.02403846153846154
+                        ],
+                        "X": false
+                    },
+                    "Imux30": {
+                        "Unit": "V",
+                        "Values": [
+                            0.125
+                        ],
+                        "X": false
+                    },
+                    "Imux31": {
+                        "Unit": "V",
+                        "Values": [
+                            0.02403846153846154
+                        ],
+                        "X": false
+                    },
+                    "Imux63": {
+                        "Unit": "V",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
                             0.0
                         ],
                         "X": false
                     },
-                    "ADC_Vmux8": {
-                        "Unit": "Count",
+                    "SetCurrent": {
+                        "Unit": "A",
                         "Values": [
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765
+                            2.1
                         ],
                         "X": false
                     },
-                    "DACs_input": {
-                        "Unit": "Count",
-                        "Values": [
-                            500.0,
-                            700.0,
-                            900.0,
-                            1100.0,
-                            1300.0,
-                            1500.0,
-                            1700.0,
-                            1900.0,
-                            2100.0,
-                            2300.0,
-                            2500.0,
-                            2700.0,
-                            2900.0,
-                            3100.0,
-                            3300.0
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            29.2
                         ],
-                        "X": true
+                        "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
-                    "Vmux8": {
-                        "Unit": "V",
-                        "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux36": {
+                        "Unit": "V",
+                        "Values": [
+                            0.25
+                        ],
+                        "X": false
+                    },
+                    "Vmux37": {
+                        "Unit": "V",
+                        "Values": [
+                            0.29571345625
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 29.2,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -696,15 +672,14 @@
                                 "DiffPreampT": 500,
                                 "DiffPreampTL": 500,
                                 "DiffPreampTR": 500,
                                 "EnCoreCol0": 65535,
                                 "EnCoreCol1": 65535,
                                 "EnCoreCol2": 65535,
                                 "EnCoreCol3": 63,
-                                "InjVcalRange": 1,
                                 "MonitorI": 63,
                                 "MonitorV": 1,
                                 "SerEnLane": 1,
                                 "ServiceBlockEn": 1,
                                 "SldoTrimA": 8,
                                 "SldoTrimD": 5
                             },
@@ -738,21 +713,22 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846814,
-                    "TimeStart": 1712846641
+                    "TimeEnd": 1714494049,
+                    "TimeStart": 1714493851,
+                    "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.2.3"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
-            "testType": "ADC_CALIBRATION"
+            "testType": "LP_MODE"
         }
     ]
 ]
```

### Comparing `module_qc_tools-2.2.3/Measurements/ANALOG_READBACK/2024-04-11_144351/20UPGXM1234567.json` & `module_qc_tools-2.2.4/Measurements/ANALOG_READBACK/2024-04-30_161711/20UPGXM1234567.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9903068313557011%*

 * *Differences: {'0': "{0: {'results': {'property': {'ANALOG_READBACK_MEASUREMENT_VERSION': '2.2.4'}, "*

 * *      "'Measurements': {'Vmux0': {'Values': [0.0]}, 'Vmux3': {'Values': [1.5479120971119267]}, "*

 * *      "'Vmux4': {'Values': [1.5479120971119267]}, 'Vmux5': {'Values': [1.5479120971119267]}, "*

 * *      "'Vmux6': {'Values': [1.5479120971119267]}, 'Vmux7': {'Values': [0.0027395604855596336]}, "*

 * *      "'Vmux8': {'Values': [0.0027395604855596336]}, 'Vmux9': {'Values': [1.5479120971119267]}, "*

 * *      "'Vmux10': {'Values': [1.54791 […]*

```diff
@@ -2,393 +2,393 @@
     [
         {
             "results": {
                 "Measurements": {
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.04
                         ],
                         "X": false
                     },
                     "Imux1": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux10": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux11": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux12": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux13": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux14": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux15": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux16": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux17": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux18": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux19": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux2": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux20": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux21": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux22": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux23": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux24": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux25": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.35000000000000003
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.20576923076923084
                         ],
                         "X": false
                     },
                     "Imux3": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.35000000000000003
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.20576923076923084
                         ],
                         "X": false
                     },
                     "Imux4": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux5": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux6": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Imux7": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux8": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux10": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux11": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux12": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux13": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux15": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux17": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux3": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6006006006006006
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.3779976775
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.25
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.3779976775
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux39": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux4": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux5": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux6": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux7": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0027395604855596336
                         ],
                         "X": false
                     },
                     "Vmux8": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0027395604855596336
                         ],
                         "X": false
                     },
                     "Vmux9": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -450,103 +450,103 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712846635,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714493834,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
             "results": {
                 "Measurements": {
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Imux9": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054
                         ],
                         "X": false
                     },
                     "MonSensAcbDem": {
                         "Unit": "-",
                         "Values": [
                             0,
@@ -811,198 +811,198 @@
                             36.760000000000005
                         ],
                         "X": false
                     },
                     "Vmux14": {
                         "Unit": "V",
                         "Values": [
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux16": {
                         "Unit": "V",
                         "Values": [
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux18": {
                         "Unit": "V",
                         "Values": [
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux2": {
                         "Unit": "V",
                         "Values": [
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -1064,21 +1064,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712847632,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714494916,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -2051,74 +2051,74 @@
                             15
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -2180,414 +2180,414 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712847244,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714494527,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.04
                         ],
                         "X": false
                     },
                     "Imux1": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux10": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux11": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux12": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux13": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux14": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux15": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux16": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux17": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux18": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux19": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux2": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux20": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux21": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux22": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux23": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux24": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux25": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.35000000000000003
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.20576923076923084
                         ],
                         "X": false
                     },
                     "Imux3": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.35000000000000003
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.20576923076923084
                         ],
                         "X": false
                     },
                     "Imux4": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux5": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux6": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Imux7": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux8": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux10": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux11": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux12": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux13": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux15": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux17": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux3": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6006006006006006
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.3779976775
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.25
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.3779976775
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux39": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux4": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux5": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux6": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux7": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0027395604855596336
                         ],
                         "X": false
                     },
                     "Vmux8": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0027395604855596336
                         ],
                         "X": false
                     },
                     "Vmux9": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -2649,103 +2649,103 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712846635,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714493834,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
             "results": {
                 "Measurements": {
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Imux9": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054
                         ],
                         "X": false
                     },
                     "MonSensAcbDem": {
                         "Unit": "-",
                         "Values": [
                             0,
@@ -3010,198 +3010,198 @@
                             36.760000000000005
                         ],
                         "X": false
                     },
                     "Vmux14": {
                         "Unit": "V",
                         "Values": [
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux16": {
                         "Unit": "V",
                         "Values": [
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux18": {
                         "Unit": "V",
                         "Values": [
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux2": {
                         "Unit": "V",
                         "Values": [
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -3263,21 +3263,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712847632,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714494916,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -4250,74 +4250,74 @@
                             15
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -4379,414 +4379,414 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712847244,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714494527,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.04
                         ],
                         "X": false
                     },
                     "Imux1": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux10": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux11": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux12": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux13": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux14": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux15": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux16": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux17": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux18": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux19": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux2": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux20": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux21": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux22": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux23": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux24": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux25": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.35000000000000003
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.20576923076923084
                         ],
                         "X": false
                     },
                     "Imux3": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.35000000000000003
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.20576923076923084
                         ],
                         "X": false
                     },
                     "Imux4": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux5": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux6": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Imux7": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux8": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux10": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux11": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux12": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux13": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux15": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux17": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux3": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6006006006006006
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.3779976775
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.25
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.3779976775
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux39": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux4": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux5": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux6": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux7": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0027395604855596336
                         ],
                         "X": false
                     },
                     "Vmux8": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0027395604855596336
                         ],
                         "X": false
                     },
                     "Vmux9": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -4848,103 +4848,103 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712846635,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714493834,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
             "results": {
                 "Measurements": {
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Imux9": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054
                         ],
                         "X": false
                     },
                     "MonSensAcbDem": {
                         "Unit": "-",
                         "Values": [
                             0,
@@ -5209,198 +5209,198 @@
                             36.760000000000005
                         ],
                         "X": false
                     },
                     "Vmux14": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux16": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux18": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux2": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -5462,21 +5462,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712847632,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714494916,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -6449,74 +6449,74 @@
                             15
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -6578,414 +6578,414 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712847244,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714494527,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.04
                         ],
                         "X": false
                     },
                     "Imux1": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux10": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux11": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux12": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux13": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux14": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux15": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux16": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux17": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux18": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux19": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux2": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux20": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux21": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux22": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux23": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux24": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux25": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.35000000000000003
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.20576923076923084
                         ],
                         "X": false
                     },
                     "Imux3": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.35000000000000003
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.20576923076923084
                         ],
                         "X": false
                     },
                     "Imux4": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux5": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux6": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Imux7": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Imux8": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux10": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux11": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux12": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux13": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux15": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux17": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux3": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6006006006006006
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.3779976775
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux36": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.25
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.3779976775
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux39": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux4": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux5": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux6": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux7": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0027395604855596336
                         ],
                         "X": false
                     },
                     "Vmux8": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0027395604855596336
                         ],
                         "X": false
                     },
                     "Vmux9": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -7047,103 +7047,103 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712846635,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714493834,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
             "results": {
                 "Measurements": {
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Imux9": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054,
+                            0.054
                         ],
                         "X": false
                     },
                     "MonSensAcbDem": {
                         "Unit": "-",
                         "Values": [
                             0,
@@ -7408,198 +7408,198 @@
                             36.760000000000005
                         ],
                         "X": false
                     },
                     "Vmux14": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux16": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux18": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux2": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084,
+                            0.084
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -7661,21 +7661,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712847632,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714494916,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -8648,74 +8648,74 @@
                             15
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6
                         ],
                         "X": false
                     },
                     "Vmux38": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6,
+                            0.6
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -8777,21 +8777,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712848680,
-                    "TimeStart": 1712847244,
+                    "TimeEnd": 1714495956,
+                    "TimeStart": 1714494527,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ]
```

### Comparing `module_qc_tools-2.2.3/Measurements/DATA_TRANSMISSION/2024-04-11_144358/20UPGXM1234567.json` & `module_qc_tools-2.2.4/Measurements/DATA_TRANSMISSION/2024-04-30_161720/20UPGXM1234567.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9912109375%*

 * *Differences: {'0': "{0: {'results': {'property': {'DATA_TRANSMISSION_MEASUREMENT_VERSION': '2.2.4'}, "*

 * *      "'Metadata': {'TimeStart': 1714493842, 'TimeEnd': 1714493853}}}}",*

 * * '1': "{0: {'results': {'property': {'DATA_TRANSMISSION_MEASUREMENT_VERSION': '2.2.4'}, "*

 * *      "'Metadata': {'TimeStart': 1714493842, 'TimeEnd': 1714493853}}}}",*

 * * '2': "{0: {'results': {'property': {'DATA_TRANSMISSION_MEASUREMENT_VERSION': '2.2.4'}, "*

 * *      "'Metadata': {'TimeStart': 1714493842, 'TimeEnd': 1714493853}}}}",*

 * * '3': "{0: {'results':  […]*

```diff
@@ -151,20 +151,20 @@
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "Rx": [
                         2
                     ],
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846649,
-                    "TimeStart": 1712846640
+                    "TimeEnd": 1714493853,
+                    "TimeStart": 1714493842
                 },
                 "comment": "",
                 "property": {
-                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.3"
+                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "DATA_TRANSMISSION"
         }
     ],
@@ -320,20 +320,20 @@
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "Rx": [
                         1
                     ],
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846649,
-                    "TimeStart": 1712846640
+                    "TimeEnd": 1714493853,
+                    "TimeStart": 1714493842
                 },
                 "comment": "",
                 "property": {
-                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.3"
+                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "DATA_TRANSMISSION"
         }
     ],
@@ -489,20 +489,20 @@
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "Rx": [
                         0
                     ],
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846649,
-                    "TimeStart": 1712846640
+                    "TimeEnd": 1714493853,
+                    "TimeStart": 1714493842
                 },
                 "comment": "",
                 "property": {
-                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.3"
+                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "DATA_TRANSMISSION"
         }
     ],
@@ -658,20 +658,20 @@
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "Rx": [
                         3
                     ],
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846649,
-                    "TimeStart": 1712846640
+                    "TimeEnd": 1714493853,
+                    "TimeStart": 1714493842
                 },
                 "comment": "",
                 "property": {
-                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.3"
+                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "DATA_TRANSMISSION"
         }
     ]
```

### Comparing `module_qc_tools-2.2.3/Measurements/IV_MEASURE/2024-04-11_144408/20UPGXM1234567.json` & `module_qc_tools-2.2.4/Measurements/IV_MEASURE/2024-04-30_161653/20UPGXM1234567.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9884079371203214%*

 * *Differences: {'0': "{0: {'results': {'property': {'IV_MEASURE_MEASUREMENT_VERSION': '2.2.4'}, 'Measurements': "*

 * *      "{'time': {'Values': [2.9203546047210693, 8.075310230255127, 13.290433168411255, "*

 * *      '18.49745202064514, 23.678497076034546, 28.8954439163208, 34.10408926010132, '*

 * *      '39.32068061828613, 44.50120306015015, 49.67970561981201, 54.85895252227783, '*

 * *      '60.08108377456665, 65.39267253875732, 70.61978507041931, 75.84810709953308, '*

 * *      '81.08787059783936, 86.37745332717896, 91.7184362411499, 96.961 […]*

```diff
@@ -101,102 +101,102 @@
                             0.0
                         ],
                         "X": false
                     },
                     "temperature": {
                         "Unit": "C",
                         "Values": [
-                            22.653,
-                            23.668,
-                            23.408,
-                            22.379,
-                            23.82,
-                            23.043,
-                            23.347,
-                            22.894,
-                            23.659,
-                            22.302,
+                            22.037,
+                            23.187,
+                            22.26,
+                            23.316,
+                            22.409,
+                            23.323,
+                            22.965,
+                            23.678,
+                            22.726,
+                            23.877,
+                            22.91,
+                            23.66,
+                            22.725,
+                            23.6,
+                            22.546,
+                            23.151,
+                            22.577,
+                            23.586,
+                            23.36,
+                            22.246,
+                            22.598,
+                            23.392,
+                            23.598,
+                            22.41,
+                            23.591,
+                            22.951,
+                            22.989,
+                            22.248,
+                            22.27,
+                            23.609,
+                            22.572,
+                            23.927,
+                            22.752,
                             22.38,
-                            23.582,
-                            23.688,
-                            22.482,
-                            22.279,
-                            23.286,
-                            23.675,
-                            22.473,
-                            23.451,
-                            23.507,
-                            22.899,
-                            22.854,
-                            22.109,
-                            22.799,
-                            22.898,
-                            23.047,
-                            22.995,
-                            22.514,
-                            23.906,
-                            22.16,
-                            23.758,
-                            22.973,
-                            23.775,
-                            23.21,
-                            23.863,
-                            22.509,
-                            23.291,
-                            22.086,
-                            22.961,
-                            22.191,
-                            23.451
+                            22.282,
+                            22.265,
+                            23.146,
+                            23.804,
+                            22.013,
+                            23.827,
+                            23.954
                         ],
                         "X": false
                     },
                     "time": {
                         "Unit": "s",
                         "Values": [
-                            3.4990110397338867,
-                            10.654615640640259,
-                            17.786351203918457,
-                            25.07872724533081,
-                            32.36049175262451,
-                            39.556445837020874,
-                            46.76604914665222,
-                            54.03743767738342,
-                            61.472991704940796,
-                            68.75101113319397,
-                            76.06875991821289,
-                            83.38463735580444,
-                            90.61199283599854,
-                            97.8469467163086,
-                            105.29408407211304,
-                            113.04050135612488,
-                            120.27624917030334,
-                            127.51144671440125,
-                            134.82101464271545,
-                            142.05521869659424,
-                            149.34129238128662,
-                            156.61187052726746,
-                            163.7993233203888,
-                            171.07467675209045,
-                            178.46036911010742,
-                            185.7854447364807,
-                            193.07947754859924,
-                            200.4380919933319,
-                            207.71494221687317,
-                            215.1624174118042,
-                            222.56464743614197,
-                            229.97363090515137,
-                            237.36760926246643,
-                            244.63192176818848,
-                            251.95480060577393,
-                            259.28730869293213,
-                            266.64627504348755,
-                            273.89922976493835,
-                            281.20752596855164,
-                            288.4393994808197,
-                            295.69199085235596
+                            2.9203546047210693,
+                            8.075310230255127,
+                            13.290433168411255,
+                            18.49745202064514,
+                            23.678497076034546,
+                            28.8954439163208,
+                            34.10408926010132,
+                            39.32068061828613,
+                            44.50120306015015,
+                            49.67970561981201,
+                            54.85895252227783,
+                            60.08108377456665,
+                            65.39267253875732,
+                            70.61978507041931,
+                            75.84810709953308,
+                            81.08787059783936,
+                            86.37745332717896,
+                            91.7184362411499,
+                            96.96145749092102,
+                            102.29869413375854,
+                            107.51347875595093,
+                            112.720547914505,
+                            117.99345779418945,
+                            123.26463484764099,
+                            128.53143119812012,
+                            133.78139090538025,
+                            139.02031016349792,
+                            144.2284333705902,
+                            149.38444900512695,
+                            154.608256816864,
+                            159.7714524269104,
+                            164.94910645484924,
+                            170.18090772628784,
+                            175.35154247283936,
+                            180.51533198356628,
+                            185.700101852417,
+                            190.88788032531738,
+                            196.0730106830597,
+                            201.20443868637085,
+                            206.41851568222046,
+                            211.6124792098999
                         ],
                         "X": false
                     },
                     "voltage": {
                         "Unit": "V",
                         "Values": [
                             0.0,
@@ -241,25 +241,25 @@
                             -195.0,
                             -200.0
                         ],
                         "X": true
                     }
                 },
                 "Metadata": {
-                    "AverageTemperature": 23.02987804878049,
+                    "AverageTemperature": 22.993097560975606,
                     "DepletionVoltage": null,
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "SettlingTime": 2,
-                    "TimeEnd": 1712847025,
-                    "TimeStart": 1712846649
+                    "TimeEnd": 1714494075,
+                    "TimeStart": 1714493814
                 },
                 "comment": "",
                 "property": {
-                    "IV_MEASURE_MEASUREMENT_VERSION": "2.2.3"
+                    "IV_MEASURE_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "20UPGXM1234567",
             "subtestType": "",
             "testType": "IV_MEASURE"
         }
     ]
```

### Comparing `module_qc_tools-2.2.3/Measurements/LP_MODE/2024-04-11_144406/20UPGXM1234567.json` & `module_qc_tools-2.2.4/Measurements/UNDERSHUNT_PROTECTION/2024-04-30_161717/20UPGXM1234567.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8522548776455027%*

 * *Differences: {'0': "{0: {'testType': 'UNDERSHUNT_PROTECTION', 'results': {'property': {replace: "*

 * *      "OrderedDict([('UNDERSHUNT_PROTECTION_MEASUREMENT_VERSION', '2.2.4')])}, 'Measurements': "*

 * *      "{'Temperature': {'Values': {insert: [(0, 29.2), (1, 29.2)]}}, 'SetCurrent': {'Values': "*

 * *      "{insert: [(0, 2.1), (1, 2.1)]}}, 'Current': {'Values': {insert: [(0, 2.1), (1, 2.1)]}}, "*

 * *      "'Vmux30': {'Values': [0.0, 0.0, 0.0]}, 'Vmux33': {'Values': [0.29571345625, 0.29571345625, "*

 * *      "0.29571345625]}, 'Vmux37': {'V […]*

```diff
@@ -2,106 +2,152 @@
     [
         {
             "results": {
                 "Measurements": {
                     "Current": {
                         "Unit": "A",
                         "Values": [
+                            2.1,
+                            2.1,
                             2.1
                         ],
                         "X": true
                     },
-                    "FailingPixels": {
-                        "Unit": "Counts",
-                        "Values": [
-                            -1
-                        ],
-                        "X": false
-                    },
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.04,
+                            0.04,
+                            0.04
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.125,
+                            0.125,
+                            0.125
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.02403846153846154,
+                            0.02403846153846154,
+                            0.02403846153846154
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.125,
+                            0.125,
+                            0.125
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.02403846153846154,
+                            0.02403846153846154,
+                            0.02403846153846154
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
+                            2.1,
+                            2.1,
                             2.1
                         ],
                         "X": false
                     },
                     "Temperature": {
                         "Unit": "C",
                         "Values": [
+                            29.2,
+                            29.2,
                             29.2
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.29571345625,
+                            0.29571345625,
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux34": {
+                        "Unit": "V",
+                        "Values": [
+                            0.5914269125,
+                            0.5914269125,
+                            0.5914269125
                         ],
                         "X": false
                     },
-                    "Vmux36": {
+                    "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.29571345625,
+                            0.29571345625,
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux38": {
+                        "Unit": "V",
+                        "Values": [
+                            0.5914269125,
+                            0.5914269125,
+                            0.5914269125
+                        ],
+                        "X": false
+                    },
+                    "Vmux39": {
+                        "Unit": "V",
+                        "Values": [
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 29.2,
                     "ChannelConfig": "",
@@ -164,127 +210,173 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846767,
-                    "TimeStart": 1712846647,
+                    "TimeEnd": 1714494459,
+                    "TimeStart": 1714493837,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.2.3"
+                    "UNDERSHUNT_PROTECTION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
-            "testType": "LP_MODE"
+            "testType": "UNDERSHUNT_PROTECTION"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
                     "Current": {
                         "Unit": "A",
                         "Values": [
+                            2.1,
+                            2.1,
                             2.1
                         ],
                         "X": true
                     },
-                    "FailingPixels": {
-                        "Unit": "Counts",
-                        "Values": [
-                            -1
-                        ],
-                        "X": false
-                    },
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.04,
+                            0.04,
+                            0.04
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.125,
+                            0.125,
+                            0.125
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.02403846153846154,
+                            0.02403846153846154,
+                            0.02403846153846154
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.125,
+                            0.125,
+                            0.125
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.02403846153846154,
+                            0.02403846153846154,
+                            0.02403846153846154
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
+                            2.1,
+                            2.1,
                             2.1
                         ],
                         "X": false
                     },
                     "Temperature": {
                         "Unit": "C",
                         "Values": [
+                            29.2,
+                            29.2,
                             29.2
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.29571345625,
+                            0.29571345625,
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux34": {
+                        "Unit": "V",
+                        "Values": [
+                            0.5914269125,
+                            0.5914269125,
+                            0.5914269125
                         ],
                         "X": false
                     },
-                    "Vmux36": {
+                    "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.29571345625,
+                            0.29571345625,
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux38": {
+                        "Unit": "V",
+                        "Values": [
+                            0.5914269125,
+                            0.5914269125,
+                            0.5914269125
+                        ],
+                        "X": false
+                    },
+                    "Vmux39": {
+                        "Unit": "V",
+                        "Values": [
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 29.2,
                     "ChannelConfig": "",
@@ -347,127 +439,173 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846767,
-                    "TimeStart": 1712846647,
+                    "TimeEnd": 1714494459,
+                    "TimeStart": 1714493837,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.2.3"
+                    "UNDERSHUNT_PROTECTION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
-            "testType": "LP_MODE"
+            "testType": "UNDERSHUNT_PROTECTION"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
                     "Current": {
                         "Unit": "A",
                         "Values": [
+                            2.1,
+                            2.1,
                             2.1
                         ],
                         "X": true
                     },
-                    "FailingPixels": {
-                        "Unit": "Counts",
-                        "Values": [
-                            -1
-                        ],
-                        "X": false
-                    },
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.04,
+                            0.04,
+                            0.04
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.125,
+                            0.125,
+                            0.125
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.02403846153846154,
+                            0.02403846153846154,
+                            0.02403846153846154
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.125,
+                            0.125,
+                            0.125
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.02403846153846154,
+                            0.02403846153846154,
+                            0.02403846153846154
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
+                            2.1,
+                            2.1,
                             2.1
                         ],
                         "X": false
                     },
                     "Temperature": {
                         "Unit": "C",
                         "Values": [
+                            29.2,
+                            29.2,
                             29.2
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.29571345625,
+                            0.29571345625,
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux34": {
+                        "Unit": "V",
+                        "Values": [
+                            0.5914269125,
+                            0.5914269125,
+                            0.5914269125
                         ],
                         "X": false
                     },
-                    "Vmux36": {
+                    "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.29571345625,
+                            0.29571345625,
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux38": {
+                        "Unit": "V",
+                        "Values": [
+                            0.5914269125,
+                            0.5914269125,
+                            0.5914269125
+                        ],
+                        "X": false
+                    },
+                    "Vmux39": {
+                        "Unit": "V",
+                        "Values": [
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 29.2,
                     "ChannelConfig": "",
@@ -530,127 +668,173 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846767,
-                    "TimeStart": 1712846647,
+                    "TimeEnd": 1714494459,
+                    "TimeStart": 1714493837,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.2.3"
+                    "UNDERSHUNT_PROTECTION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
-            "testType": "LP_MODE"
+            "testType": "UNDERSHUNT_PROTECTION"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
                     "Current": {
                         "Unit": "A",
                         "Values": [
+                            2.1,
+                            2.1,
                             2.1
                         ],
                         "X": true
                     },
-                    "FailingPixels": {
-                        "Unit": "Counts",
-                        "Values": [
-                            -1
-                        ],
-                        "X": false
-                    },
                     "Imux0": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.04,
+                            0.04,
+                            0.04
                         ],
                         "X": false
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.125,
+                            0.125,
+                            0.125
                         ],
                         "X": false
                     },
                     "Imux29": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.02403846153846154,
+                            0.02403846153846154,
+                            0.02403846153846154
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.125,
+                            0.125,
+                            0.125
                         ],
                         "X": false
                     },
                     "Imux31": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.02403846153846154,
+                            0.02403846153846154,
+                            0.02403846153846154
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
+                            2.1,
+                            2.1,
                             2.1
                         ],
                         "X": false
                     },
                     "Temperature": {
                         "Unit": "C",
                         "Values": [
+                            29.2,
+                            29.2,
                             29.2
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0,
+                            0.0,
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.29571345625,
+                            0.29571345625,
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux34": {
+                        "Unit": "V",
+                        "Values": [
+                            0.5914269125,
+                            0.5914269125,
+                            0.5914269125
                         ],
                         "X": false
                     },
-                    "Vmux36": {
+                    "Vmux35": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.29571345625,
+                            0.29571345625,
+                            0.29571345625
+                        ],
+                        "X": false
+                    },
+                    "Vmux38": {
+                        "Unit": "V",
+                        "Values": [
+                            0.5914269125,
+                            0.5914269125,
+                            0.5914269125
+                        ],
+                        "X": false
+                    },
+                    "Vmux39": {
+                        "Unit": "V",
+                        "Values": [
+                            1.5479120971119267,
+                            1.5479120971119267,
+                            1.5479120971119267
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 29.2,
                     "ChannelConfig": "",
@@ -713,22 +897,22 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846767,
-                    "TimeStart": 1712846647,
+                    "TimeEnd": 1714494459,
+                    "TimeStart": 1714493837,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.2.3"
+                    "UNDERSHUNT_PROTECTION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
-            "testType": "LP_MODE"
+            "testType": "UNDERSHUNT_PROTECTION"
         }
     ]
 ]
```

### Comparing `module_qc_tools-2.2.3/Measurements/OVERVOLTAGE_PROTECTION/2024-04-11_144333/20UPGXM1234567.json` & `module_qc_tools-2.2.4/Measurements/OVERVOLTAGE_PROTECTION/2024-04-30_161656/20UPGXM1234567.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9901599702380952%*

 * *Differences: {'0': "{0: {'results': {'property': {'OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION': '2.2.4'}, "*

 * *      "'Measurements': {'Vmux30': {'Values': [0.0]}, 'Vmux32': {'Values': [0.6006006006006006]}, "*

 * *      "'Vmux33': {'Values': [0.4023781875]}, 'Vmux37': {'Values': [0.4023781875]}, 'Imux28': "*

 * *      "{'Values': [0.4166666666666666]}, 'Imux30': {'Values': [0.4166666666666666]}, 'Imux63': "*

 * *      "{'Values': [0.0]}}, 'Metadata': {'TimeStart': 1714493817, 'TimeEnd': 1714493873}}}}",*

 * * '1': "{0: {'results': {'property […]*

```diff
@@ -9,29 +9,29 @@
                             6.999999999999999
                         ],
                         "X": true
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4166666666666666
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4166666666666666
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
                             7.0
@@ -44,36 +44,36 @@
                             39.0
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6006006006006006
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4023781875
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4023781875
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 39.0,
                     "ChannelConfig": "",
@@ -136,21 +136,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846665,
-                    "TimeStart": 1712846614,
+                    "TimeEnd": 1714493873,
+                    "TimeStart": 1714493817,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
@@ -164,29 +164,29 @@
                             6.999999999999999
                         ],
                         "X": true
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4166666666666666
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4166666666666666
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
                             7.0
@@ -199,36 +199,36 @@
                             39.0
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6006006006006006
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4023781875
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4023781875
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 39.0,
                     "ChannelConfig": "",
@@ -291,21 +291,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846665,
-                    "TimeStart": 1712846614,
+                    "TimeEnd": 1714493873,
+                    "TimeStart": 1714493817,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
@@ -319,29 +319,29 @@
                             6.999999999999999
                         ],
                         "X": true
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4166666666666666
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4166666666666666
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
                             7.0
@@ -354,36 +354,36 @@
                             39.0
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6006006006006006
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4023781875
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4023781875
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 39.0,
                     "ChannelConfig": "",
@@ -446,21 +446,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846665,
-                    "TimeStart": 1712846614,
+                    "TimeEnd": 1714493873,
+                    "TimeStart": 1714493817,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
@@ -474,29 +474,29 @@
                             6.999999999999999
                         ],
                         "X": true
                     },
                     "Imux28": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4166666666666666
                         ],
                         "X": false
                     },
                     "Imux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4166666666666666
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "SetCurrent": {
                         "Unit": "A",
                         "Values": [
                             7.0
@@ -509,36 +509,36 @@
                             39.0
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.0
                         ],
                         "X": false
                     },
                     "Vmux32": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.6006006006006006
                         ],
                         "X": false
                     },
                     "Vmux33": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4023781875
                         ],
                         "X": false
                     },
                     "Vmux37": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707
+                            0.4023781875
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "AverageTemperature": 39.0,
                     "ChannelConfig": "",
@@ -601,21 +601,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1712846665,
-                    "TimeStart": 1712846614,
+                    "TimeEnd": 1714493873,
+                    "TimeStart": 1714493817,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.4"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ]
```

### Comparing `module_qc_tools-2.2.3/emulator/README.md` & `module_qc_tools-2.2.4/emulator/README.md`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/ADC_CALIBRATION.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/ADC_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/ANALOG_READBACK.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/ANALOG_READBACK.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/DATA_TRANSMISSION.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/DATA_TRANSMISSION.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/IV_MEASURE.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/IV_MEASURE.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/LP_MODE.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/LP_MODE.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/SLDO.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/SLDO.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/UNDERSHUNT_PROTECTION.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/UNDERSHUNT_PROTECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/VCAL_CALIBRATION.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/VCAL_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/globals.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/globals.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/hardware_emulator.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/hardware_emulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
 
 @app.command()
 def write_register(
     _controller: Path = OPTIONS["emulator_controller"],
     connectivity: Path = OPTIONS["emulator_connectivity"],
     chip_position: int = OPTIONS["emulator_chip_position"],
     name: str = typer.Argument(),
-    value: str = typer.Argument(),
+    value: int = typer.Argument(),
 ):
     """
     This function emulates the effect of running YARR write-register
     Currently only emulates register MonitorI, MonitorV. One needs to add a new if statement for a new register name.
     """
     module_state = get_module_state()
```

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/main.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/cli/upload_localdb.py` & `module_qc_tools-2.2.4/src/module_qc_tools/cli/upload_localdb.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/configs/emulator_merged_vmux.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/configs/emulator_merged_vmux.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/configs/example_merged_vmux.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/configs/example_merged_vmux.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/configs/example_separate_vmux.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/configs/example_separate_vmux.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/module_state_template.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/module_state_template.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/controller/specCfg-rd53b.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/emulator/configs/controller/specCfg-rd53b.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/ADC_CALIBRATION.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/ADC_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/ANALOG_READBACK.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/ANALOG_READBACK.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/DATA_TRANSMISSION.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/DATA_TRANSMISSION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/IV_MEASURE.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/IV_MEASURE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/LP_MODE.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/LP_MODE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/SLDO.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/SLDO.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/UNDERSHUNT_PROTECTION.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/UNDERSHUNT_PROTECTION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/common.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/common.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/config.json` & `module_qc_tools-2.2.4/src/module_qc_tools/data/schema/config.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/utils/hardware_control_base.py` & `module_qc_tools-2.2.4/src/module_qc_tools/utils/hardware_control_base.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/utils/misc.py` & `module_qc_tools-2.2.4/src/module_qc_tools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/utils/multimeter.py` & `module_qc_tools-2.2.4/src/module_qc_tools/utils/multimeter.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/utils/ntc.py` & `module_qc_tools-2.2.4/src/module_qc_tools/utils/ntc.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/utils/power_supply.py` & `module_qc_tools-2.2.4/src/module_qc_tools/utils/power_supply.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/src/module_qc_tools/utils/yarr.py` & `module_qc_tools-2.2.4/src/module_qc_tools/utils/yarr.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 
     def running_emulator(self):
         return self.emulator
 
     def configure(self, skip_reset=False):
         cmd = f'{self.scanConsole_exe} -r {self.controller} -c {self.connectivity} {"--skip-reset" if skip_reset else ""}'
 
+        self._register = [{} for chip in range(self._number_of_chips)]
+
         currLevel = log.getEffectiveLevel()
         log.setLevel(logging.DEBUG)
         # Below is the only case where success_code=1 is the default.
         # This is because the exit code of scanConsole for configuring the chip is 1 for success.
         # This will have to be removed once the YARR MR is merged (https://gitlab.cern.ch/YARR/YARR/-/issues/192).
         self.send_command(cmd, purpose="configure module", success_code=1)
         log.setLevel(currLevel)
@@ -102,14 +104,16 @@
 
     def run_scan(self, scan, output=None, skip_reset=False):
         if output:
             cmd = f'{self.scanConsole_exe} -r {self.controller} -c {self.connectivity} -s {scan} -o {output} {"--skip-reset" if skip_reset else ""}'
         else:
             cmd = f'{self.scanConsole_exe} -r {self.controller} -c {self.connectivity} -s {scan} {"--skip-reset" if skip_reset else ""}'
 
+        self._register = [{} for chip in range(self._number_of_chips)]
+
         log.info(f"Running YARR scan: {scan} ...")
         # Always save scan output in log file
         currLevel = log.getEffectiveLevel()
         log.setLevel("DEBUG")
         self.send_command(cmd, purpose="configure module", success_code=0)
         log.setLevel(currLevel)
 
@@ -160,14 +164,16 @@
         _dryrun = ""
         _skipconfig = ""
         _testsize = ""
         if dryrun:
             _dryrun = "-n"
         if skipconfig:
             _skipconfig = "-s"
+        else:
+            self._register = [{} for chip in range(self._number_of_chips)]
         if testsize is not None:
             _testsize = f"-t {testsize!s}"
 
         cmd = f"{self.eyeDiagram_exe} -r {self.controller} -c {self.connectivity} {_dryrun} {_skipconfig} {_testsize}"
         log.debug(cmd)
         return self.send_command_and_read(
             cmd, dtype=str, purpose="eye diagram", success_code=self.success_code
@@ -197,14 +203,18 @@
         #  Fill in values at disabled chip positions
         for i in self._disabled_chip_positions:
             mea.insert(i, -999)
         return mea, status
 
     def set_mux(self, chip_position=None, v_mux=-1, i_mux=-1, reset_other_chips=True):
         for chip in range(self._number_of_chips):
+            if reset_other_chips:
+                self.write_register(name="MonitorV", value=63, chip_position=chip)
+                self.write_register(name="MonitorI", value=63, chip_position=chip)
+        for chip in range(self._number_of_chips):
             if chip == chip_position:
                 # Set Vmux=1 to measure the I_mux pad voltage when a non-negative I_mux value is passed.
                 if i_mux >= 0:
                     v_mux = 1
                 # TODO: Consider this in read-adc script too
                 # Set Imux=63 when measuring NTC pad voltage through Vmux2.
                 if v_mux == 2:
@@ -213,17 +223,14 @@
                         name="MonitorV", value=v_mux, chip_position=chip
                     )
                 self.write_register(name="MonitorV", value=v_mux, chip_position=chip)
                 if i_mux >= 0:
                     self.write_register(
                         name="MonitorI", value=i_mux, chip_position=chip
                     )
-            elif reset_other_chips:
-                self.write_register(name="MonitorV", value=63, chip_position=chip)
-
         return 0
 
     def reset_tempsens_enable(self, chip_position=None):
         self.write_register(
             name="MonSensSldoAnaEn", value=0, chip_position=chip_position
         )
         self.write_register(
@@ -360,15 +367,15 @@
         else:
             msg = "Incorrect VMUX value for setting trim!"
             raise RuntimeError(msg)
 
         return 0
 
     def switchLPM(self, position):
-        cmd = f"{self.switchLPM_exe} -s {self.get_spec()} {position}"
+        cmd = f"{self.switchLPM_exe} {position} -s {self.get_spec()}"
         return self.send_command(cmd, purpose="switch LP mode on/off")
 
     def get_connectivity(self):
         with Path(self.connectivity).open(encoding="utf-8") as file:
             return json.load(file)
 
     def get_config(self, chip_position):
```

### Comparing `module_qc_tools-2.2.3/.gitignore` & `module_qc_tools-2.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/LICENSE` & `module_qc_tools-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/README.md` & `module_qc_tools-2.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-tools v2.2.3
+# module-qc-tools v2.2.4
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -70,15 +70,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 $ python -m venv venv
 $ source venv/bin/activate
 $ python -m pip install -U pip
-$ python -m pip install -U pip module-qc-tools==2.2.3
+$ python -m pip install -U pip module-qc-tools==2.2.4
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
```

### Comparing `module_qc_tools-2.2.3/pyproject.toml` & `module_qc_tools-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.3/PKG-INFO` & `module_qc_tools-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: module_qc_tools
-Version: 2.2.3
+Version: 2.2.4
 Summary: Module qc tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 ATLAS ITk Pixel Modules
@@ -39,15 +39,15 @@
 Requires-Dist: pre-commit
 Requires-Dist: requests
 Requires-Dist: tabulate
 Requires-Dist: typer>=0.9.0
 Requires-Dist: urllib3<2,>=1.26.11; 'el7.x86_64' in platform_release
 Description-Content-Type: text/markdown
 
-# module-qc-tools v2.2.3
+# module-qc-tools v2.2.4
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -115,15 +115,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 $ python -m venv venv
 $ source venv/bin/activate
 $ python -m pip install -U pip
-$ python -m pip install -U pip module-qc-tools==2.2.3
+$ python -m pip install -U pip module-qc-tools==2.2.4
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
```

