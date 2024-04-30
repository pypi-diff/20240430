# Comparing `tmp/modm-devices-0.9.3.tar.gz` & `tmp/modm-devices-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modm-devices-0.9.3.tar", last modified: Fri Sep 30 17:57:34 2022, max compression
+gzip compressed data, was "modm-devices-0.9.4.tar", last modified: Sun Dec 11 10:48:21 2022, max compression
```

## Comparing `modm-devices-0.9.3.tar` & `modm-devices-0.9.4.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 17:57:34.486061 modm-devices-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-09-30 17:57:25.000000 modm-devices-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7238 2022-09-30 17:57:34.486061 modm-devices-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6264 2022-09-30 17:57:25.000000 modm-devices-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 17:57:34.462061 modm-devices-0.9.3/modm_devices/
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     5174 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/device_file.py
--rw-r--r--   0 runner    (1001) docker     (121)    10770 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/device_identifier.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/pkg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 17:57:34.462061 modm-devices-0.9.3/modm_devices/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/catalog.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 17:57:34.462061 modm-devices-0.9.3/modm_devices/resources/devices/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 17:57:34.466061 modm-devices-0.9.3/modm_devices/resources/devices/avr/
--rw-r--r--   0 runner    (1001) docker     (121)     6364 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/at90-32_64_128-can.xml
--rw-r--r--   0 runner    (1001) docker     (121)     5874 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-128-rfa1.xml
--rw-r--r--   0 runner    (1001) docker     (121)     6890 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-1281_2561.xml
--rw-r--r--   0 runner    (1001) docker     (121)     6457 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-1284-n_p.xml
--rw-r--r--   0 runner    (1001) docker     (121)    11003 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-164_324_644-a_n_p_pa_pv_v.xml
--rw-r--r--   0 runner    (1001) docker     (121)    10138 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-169_329_649.xml
--rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-16_32-u4_u4rc.xml
--rw-r--r--   0 runner    (1001) docker     (121)     6786 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-16_32_64-c1_m1.xml
--rw-r--r--   0 runner    (1001) docker     (121)     9830 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-324-pb.xml
--rw-r--r--   0 runner    (1001) docker     (121)    10469 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-48_88_168_328-a_n_p_pa_pv_v.xml
--rw-r--r--   0 runner    (1001) docker     (121)    10711 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-48_88_168_328-pb.xml
--rw-r--r--   0 runner    (1001) docker     (121)    10792 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-640_1280_2560.xml
--rw-r--r--   0 runner    (1001) docker     (121)     8591 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-64_128-a_l_n.xml
--rw-r--r--   0 runner    (1001) docker     (121)     9340 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-8_16_32-a_l_n.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4639 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-8_16_32-u2.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3343 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-102_104.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-13.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-20.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3909 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-24_44_84.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4363 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-25_45_85.xml
--rw-r--r--   0 runner    (1001) docker     (121)     5557 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-261_461_861.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3540 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-40.xml
--rw-r--r--   0 runner    (1001) docker     (121)     6170 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-441_841.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4945 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-48_88.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-4_5_9_10.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 17:57:34.466061 modm-devices-0.9.3/modm_devices/resources/devices/nrf/
--rw-r--r--   0 runner    (1001) docker     (121)     6388 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52810.xml
--rw-r--r--   0 runner    (1001) docker     (121)     7032 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52811.xml
--rw-r--r--   0 runner    (1001) docker     (121)     7376 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52820.xml
--rw-r--r--   0 runner    (1001) docker     (121)     9114 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52832.xml
--rw-r--r--   0 runner    (1001) docker     (121)    11100 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52833.xml
--rw-r--r--   0 runner    (1001) docker     (121)    11647 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52840.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 17:57:34.466061 modm-devices-0.9.3/modm_devices/resources/devices/rp/
--rw-r--r--   0 runner    (1001) docker     (121)    26360 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/rp/rp2040.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 17:57:34.470061 modm-devices-0.9.3/modm_devices/resources/devices/sam/
--rw-r--r--   0 runner    (1001) docker     (121)    14362 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/sam/samd09.xml
--rw-r--r--   0 runner    (1001) docker     (121)    19206 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/sam/samd10_d11.xml
--rw-r--r--   0 runner    (1001) docker     (121)    36645 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/sam/samd20.xml
--rw-r--r--   0 runner    (1001) docker     (121)    57261 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/sam/samd21.xml
--rw-r--r--   0 runner    (1001) docker     (121)    80151 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/sam/samd51_e51_e53_e54.xml
--rw-r--r--   0 runner    (1001) docker     (121)    29815 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/sam/samda1.xml
--rw-r--r--   0 runner    (1001) docker     (121)    87452 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/sam/same70_s70_v70_v71.xml
--rw-r--r--   0 runner    (1001) docker     (121)    10628 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/sam/samg51_g53_g54.xml
--rw-r--r--   0 runner    (1001) docker     (121)    40329 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/sam/samg55.xml
--rw-r--r--   0 runner    (1001) docker     (121)    40522 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/sam/saml21.xml
--rw-r--r--   0 runner    (1001) docker     (121)    44287 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/sam/saml22.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 17:57:34.486061 modm-devices-0.9.3/modm_devices/resources/devices/stm32/
--rw-r--r--   0 runner    (1001) docker     (121)    41924 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-30.xml
--rw-r--r--   0 runner    (1001) docker     (121)    25906 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-31.xml
--rw-r--r--   0 runner    (1001) docker     (121)    23482 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-38.xml
--rw-r--r--   0 runner    (1001) docker     (121)    32438 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-42.xml
--rw-r--r--   0 runner    (1001) docker     (121)    24473 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-48.xml
--rw-r--r--   0 runner    (1001) docker     (121)    40630 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-51.xml
--rw-r--r--   0 runner    (1001) docker     (121)    31678 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-58.xml
--rw-r--r--   0 runner    (1001) docker     (121)    28182 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-70.xml
--rw-r--r--   0 runner    (1001) docker     (121)    52211 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-71.xml
--rw-r--r--   0 runner    (1001) docker     (121)    55991 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-72.xml
--rw-r--r--   0 runner    (1001) docker     (121)    54894 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-78.xml
--rw-r--r--   0 runner    (1001) docker     (121)    71068 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-91.xml
--rw-r--r--   0 runner    (1001) docker     (121)    70395 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-98.xml
--rw-r--r--   0 runner    (1001) docker     (121)    25221 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-00-4_6.xml
--rw-r--r--   0 runner    (1001) docker     (121)    34965 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-00-8_b.xml
--rw-r--r--   0 runner    (1001) docker     (121)    44386 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-00-c_d_e.xml
--rw-r--r--   0 runner    (1001) docker     (121)    39867 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-01-c_d_e.xml
--rw-r--r--   0 runner    (1001) docker     (121)    41658 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-01-f_g.xml
--rw-r--r--   0 runner    (1001) docker     (121)    20395 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-01_02-4_6.xml
--rw-r--r--   0 runner    (1001) docker     (121)    35422 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-01_02-8_b.xml
--rw-r--r--   0 runner    (1001) docker     (121)    28697 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-03-4_6.xml
--rw-r--r--   0 runner    (1001) docker     (121)    48641 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-03-8_b.xml
--rw-r--r--   0 runner    (1001) docker     (121)    62078 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-03-c_d_e.xml
--rw-r--r--   0 runner    (1001) docker     (121)    55643 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-03-f_g.xml
--rw-r--r--   0 runner    (1001) docker     (121)    41114 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-05_07.xml
--rw-r--r--   0 runner    (1001) docker     (121)    68552 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f2-05.xml
--rw-r--r--   0 runner    (1001) docker     (121)    88970 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f2-07_15_17.xml
--rw-r--r--   0 runner    (1001) docker     (121)    36585 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-01.xml
--rw-r--r--   0 runner    (1001) docker     (121)    35651 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-02-6_8.xml
--rw-r--r--   0 runner    (1001) docker     (121)    79998 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-02-b_c_d_e.xml
--rw-r--r--   0 runner    (1001) docker     (121)    38088 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-03-6_8.xml
--rw-r--r--   0 runner    (1001) docker     (121)   100985 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-03-b_c_d_e.xml
--rw-r--r--   0 runner    (1001) docker     (121)    36334 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-18_28.xml
--rw-r--r--   0 runner    (1001) docker     (121)    41508 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-34.xml
--rw-r--r--   0 runner    (1001) docker     (121)    64413 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-58_98.xml
--rw-r--r--   0 runner    (1001) docker     (121)    60677 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-73_78.xml
--rw-r--r--   0 runner    (1001) docker     (121)    63576 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-01_11.xml
--rw-r--r--   0 runner    (1001) docker     (121)    94217 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-05_07_15_17.xml
--rw-r--r--   0 runner    (1001) docker     (121)    39771 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-10.xml
--rw-r--r--   0 runner    (1001) docker     (121)    88783 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-12.xml
--rw-r--r--   0 runner    (1001) docker     (121)   103803 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-13_23.xml
--rw-r--r--   0 runner    (1001) docker     (121)   135840 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-27_29_37_39.xml
--rw-r--r--   0 runner    (1001) docker     (121)    86009 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-46.xml
--rw-r--r--   0 runner    (1001) docker     (121)   137403 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-69_79.xml
--rw-r--r--   0 runner    (1001) docker     (121)   130611 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f7-22_23_32_33.xml
--rw-r--r--   0 runner    (1001) docker     (121)   127865 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f7-30_50.xml
--rw-r--r--   0 runner    (1001) docker     (121)   141217 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f7-45_46_56.xml
--rw-r--r--   0 runner    (1001) docker     (121)   200867 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f7-65_67_68_69_77_78_79.xml
--rw-r--r--   0 runner    (1001) docker     (121)    28294 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-30.xml
--rw-r--r--   0 runner    (1001) docker     (121)    41983 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-31_41.xml
--rw-r--r--   0 runner    (1001) docker     (121)    28829 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-50.xml
--rw-r--r--   0 runner    (1001) docker     (121)    43050 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-51_61.xml
--rw-r--r--   0 runner    (1001) docker     (121)    58686 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-70_b0.xml
--rw-r--r--   0 runner    (1001) docker     (121)    74426 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-71_81.xml
--rw-r--r--   0 runner    (1001) docker     (121)   116652 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-b1_c1.xml
--rw-r--r--   0 runner    (1001) docker     (121)    83035 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g4-31_41.xml
--rw-r--r--   0 runner    (1001) docker     (121)   107453 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g4-71.xml
--rw-r--r--   0 runner    (1001) docker     (121)   127448 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g4-73_83.xml
--rw-r--r--   0 runner    (1001) docker     (121)   132265 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g4-74_84.xml
--rw-r--r--   0 runner    (1001) docker     (121)    88918 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g4-91_a1.xml
--rw-r--r--   0 runner    (1001) docker     (121)   122761 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-23_33.xml
--rw-r--r--   0 runner    (1001) docker     (121)   184619 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-25_35.xml
--rw-r--r--   0 runner    (1001) docker     (121)   158571 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-30.xml
--rw-r--r--   0 runner    (1001) docker     (121)   158709 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-42.xml
--rw-r--r--   0 runner    (1001) docker     (121)   165431 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-43_53.xml
--rw-r--r--   0 runner    (1001) docker     (121)   165830 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-45_55.xml
--rw-r--r--   0 runner    (1001) docker     (121)   150008 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-47_57.xml
--rw-r--r--   0 runner    (1001) docker     (121)   142638 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-50.xml
--rw-r--r--   0 runner    (1001) docker     (121)   330311 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-a3.xml
--rw-r--r--   0 runner    (1001) docker     (121)   142020 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-b0.xml
--rw-r--r--   0 runner    (1001) docker     (121)   306725 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-b3.xml
--rw-r--r--   0 runner    (1001) docker     (121)    35549 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l0-10.xml
--rw-r--r--   0 runner    (1001) docker     (121)    31121 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l0-11_21.xml
--rw-r--r--   0 runner    (1001) docker     (121)    34494 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l0-31_41.xml
--rw-r--r--   0 runner    (1001) docker     (121)    67543 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l0-51_52_53_62_63.xml
--rw-r--r--   0 runner    (1001) docker     (121)   117415 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l0-71_72_73_81_82_83.xml
--rw-r--r--   0 runner    (1001) docker     (121)    31245 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l1-00.xml
--rw-r--r--   0 runner    (1001) docker     (121)    57691 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l1-51_52-6_8_b.xml
--rw-r--r--   0 runner    (1001) docker     (121)   111217 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l1-51_52_62-c_d_e.xml
--rw-r--r--   0 runner    (1001) docker     (121)    58545 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-12_22.xml
--rw-r--r--   0 runner    (1001) docker     (121)    93009 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-31_33_43.xml
--rw-r--r--   0 runner    (1001) docker     (121)    26747 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-32_42.xml
--rw-r--r--   0 runner    (1001) docker     (121)   120025 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-51_71.xml
--rw-r--r--   0 runner    (1001) docker     (121)    81424 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-52_62.xml
--rw-r--r--   0 runner    (1001) docker     (121)    68400 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-75_85.xml
--rw-r--r--   0 runner    (1001) docker     (121)   165390 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-76_86.xml
--rw-r--r--   0 runner    (1001) docker     (121)   177980 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-96_a6.xml
--rw-r--r--   0 runner    (1001) docker     (121)   147942 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-p5.xml
--rw-r--r--   0 runner    (1001) docker     (121)   142944 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-q5.xml
--rw-r--r--   0 runner    (1001) docker     (121)   205982 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-r5_r7_r9.xml
--rw-r--r--   0 runner    (1001) docker     (121)   163983 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-s5_s7_s9.xml
--rw-r--r--   0 runner    (1001) docker     (121)   175612 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l5-52_62.xml
--rw-r--r--   0 runner    (1001) docker     (121)   204503 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32u5-75_85.xml
--rw-r--r--   0 runner    (1001) docker     (121)    32724 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wb-10_15_1m.xml
--rw-r--r--   0 runner    (1001) docker     (121)    19782 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wb-30_50.xml
--rw-r--r--   0 runner    (1001) docker     (121)    59925 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wb-35_55_5m.xml
--rw-r--r--   0 runner    (1001) docker     (121)    33913 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wl-54_55.xml
--rw-r--r--   0 runner    (1001) docker     (121)    35165 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wl-e4_e5.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 17:57:34.486061 modm-devices-0.9.3/modm_devices/resources/schema/
--rw-r--r--   0 runner    (1001) docker     (121)     9015 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/schema/device.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/schema/xinclude.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-09-30 17:57:25.000000 modm-devices-0.9.3/modm_devices/resources/schema/xml.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 17:57:34.462061 modm-devices-0.9.3/modm_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7238 2022-09-30 17:57:34.000000 modm-devices-0.9.3/modm_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8266 2022-09-30 17:57:34.000000 modm-devices-0.9.3/modm_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 17:57:34.000000 modm-devices-0.9.3/modm_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-30 17:57:34.000000 modm-devices-0.9.3/modm_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-30 17:57:34.000000 modm-devices-0.9.3/modm_devices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-30 17:57:34.486061 modm-devices-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-09-30 17:57:25.000000 modm-devices-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:48:21.287984 modm-devices-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2022-12-11 10:48:09.000000 modm-devices-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2022-12-11 10:48:21.287984 modm-devices-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2022-12-11 10:48:09.000000 modm-devices-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:48:21.263983 modm-devices-0.9.4/modm_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/device_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/device_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/pkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:48:21.267983 modm-devices-0.9.4/modm_devices/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/catalog.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:48:21.263983 modm-devices-0.9.4/modm_devices/resources/devices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:48:21.267983 modm-devices-0.9.4/modm_devices/resources/devices/avr/
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/at90-32_64_128-can.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-128-rfa1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-1281_2561.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-1284-n_p.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-164_324_644-a_n_p_pa_pv_v.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-169_329_649.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-16_32-u4_u4rc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-16_32_64-c1_m1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9830 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-324-pb.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-48_88_168_328-a_n_p_pa_pv_v.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-48_88_168_328-pb.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-640_1280_2560.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-64_128-a_l_n.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-8_16_32-a_l_n.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-8_16_32-u2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-102_104.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-13.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-20.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-24_44_84.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-25_45_85.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-261_461_861.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-40.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-441_841.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-48_88.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-4_5_9_10.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:48:21.267983 modm-devices-0.9.4/modm_devices/resources/devices/nrf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52810.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52811.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52820.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9114 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52832.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52833.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52840.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:48:21.267983 modm-devices-0.9.4/modm_devices/resources/devices/rp/
+-rw-r--r--   0 runner    (1001) docker     (123)    26360 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/rp/rp2040.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:48:21.271983 modm-devices-0.9.4/modm_devices/resources/devices/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)    14362 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/sam/samd09.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    19206 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/sam/samd10_d11.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    36645 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/sam/samd20.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    57261 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/sam/samd21.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    80151 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/sam/samd51_e51_e53_e54.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    29815 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/sam/samda1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    87452 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/sam/same70_s70_v70_v71.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/sam/samg51_g53_g54.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    40329 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/sam/samg55.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    40522 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/sam/saml21.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    44287 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/sam/saml22.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:48:21.287984 modm-devices-0.9.4/modm_devices/resources/devices/stm32/
+-rw-r--r--   0 runner    (1001) docker     (123)    42018 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-30.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    25906 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-31.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    23482 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-38.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    32438 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-42.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    24473 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-48.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    40630 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-51.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    31678 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-58.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    28182 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-70.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    52211 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-71.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    55991 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-72.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    54894 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-78.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    71068 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-91.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    70395 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-98.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    25221 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-00-4_6.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    34965 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-00-8_b.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    44386 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-00-c_d_e.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    39867 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-01-c_d_e.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    41658 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-01-f_g.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    20395 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-01_02-4_6.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    35422 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-01_02-8_b.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    28697 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-03-4_6.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    48641 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-03-8_b.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    62078 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-03-c_d_e.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    55643 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-03-f_g.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    41114 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-05_07.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    68552 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f2-05.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    88970 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f2-07_15_17.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    36585 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-01.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    35651 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-02-6_8.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    79998 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-02-b_c_d_e.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    38088 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-03-6_8.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    96009 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-03-b_c_d_e.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    36334 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-18_28.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    41508 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-34.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    64413 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-58_98.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    60677 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-73_78.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    63576 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-01_11.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    94217 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-05_07_15_17.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    39771 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-10.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    88783 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-12.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   103803 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-13_23.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   135840 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-27_29_37_39.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    86009 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-46.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   137455 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-69_79.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   130611 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f7-22_23_32_33.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   127865 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f7-30_50.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   141217 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f7-45_46_56.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   200867 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f7-65_67_68_69_77_78_79.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    28294 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-30.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    41983 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-31_41.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    28829 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-50.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    43050 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-51_61.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    58686 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-70_b0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    74426 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-71_81.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   116652 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-b1_c1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    83035 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g4-31_41.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   107453 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g4-71.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   127448 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g4-73_83.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   132265 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g4-74_84.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    88918 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g4-91_a1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   122783 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-23_33.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   184641 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-25_35.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   158593 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-30.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   158713 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-42.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   165431 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-43_53.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   165830 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-45_55.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150008 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-47_57.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   142638 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-50.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   330333 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-a3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   142042 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-b0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   306747 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-b3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    35549 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l0-10.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    31121 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l0-11_21.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    34494 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l0-31_41.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    67543 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l0-51_52_53_62_63.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   117415 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l0-71_72_73_81_82_83.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    31229 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l1-00.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    57675 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l1-51_52-6_8_b.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   110659 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l1-51_52_62-c_d_e.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    58545 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-12_22.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    93009 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-31_33_43.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    26747 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-32_42.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   120025 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-51_71.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    81424 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-52_62.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    68400 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-75_85.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   165390 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-76_86.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   177988 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-96_a6.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   147942 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-p5.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   142944 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-q5.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   205982 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-r5_r7_r9.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   163983 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-s5_s7_s9.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   175200 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l5-52_62.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   204503 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32u5-75_85.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    32724 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wb-10_15_1m.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    19782 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wb-30_50.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    59925 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wb-35_55_5m.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    33913 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wl-54_55.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    35165 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wl-e4_e5.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:48:21.287984 modm-devices-0.9.4/modm_devices/resources/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/schema/device.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/schema/xinclude.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2022-12-11 10:48:09.000000 modm-devices-0.9.4/modm_devices/resources/schema/xml.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 10:48:21.267983 modm-devices-0.9.4/modm_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2022-12-11 10:48:21.000000 modm-devices-0.9.4/modm_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2022-12-11 10:48:21.000000 modm-devices-0.9.4/modm_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-11 10:48:21.000000 modm-devices-0.9.4/modm_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-11 10:48:21.000000 modm-devices-0.9.4/modm_devices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-11 10:48:21.000000 modm-devices-0.9.4/modm_devices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-11 10:48:21.287984 modm-devices-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2022-12-11 10:48:09.000000 modm-devices-0.9.4/setup.py
```

### Comparing `modm-devices-0.9.3/LICENSE` & `modm-devices-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/PKG-INFO` & `modm-devices-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modm-devices
-Version: 0.9.3
+Version: 0.9.4
 Summary: Curated data for AVR and ARM Cortex-M devices
 Home-page: https://github.com/modm-io/modm-devices
 Author: Niklas Hauser
 Author-email: niklas@salkinium.com
 License: MPL-2.0
 Keywords: modm lbuild modm-devices stm32 avr sam nrf
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `modm-devices-0.9.3/README.md` & `modm-devices-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/device.py` & `modm-devices-0.9.4/modm_devices/device.py`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/device_file.py` & `modm-devices-0.9.4/modm_devices/device_file.py`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/device_identifier.py` & `modm-devices-0.9.4/modm_devices/device_identifier.py`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/parser.py` & `modm-devices-0.9.4/modm_devices/parser.py`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/pkg.py` & `modm-devices-0.9.4/modm_devices/pkg.py`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/at90-32_64_128-can.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/at90-32_64_128-can.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-128-rfa1.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-128-rfa1.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-1281_2561.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-1281_2561.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-1284-n_p.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-1284-n_p.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-164_324_644-a_n_p_pa_pv_v.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-164_324_644-a_n_p_pa_pv_v.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-169_329_649.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-169_329_649.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-16_32-u4_u4rc.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-16_32-u4_u4rc.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-16_32_64-c1_m1.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-16_32_64-c1_m1.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-324-pb.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-324-pb.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-48_88_168_328-a_n_p_pa_pv_v.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-48_88_168_328-a_n_p_pa_pv_v.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-48_88_168_328-pb.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-48_88_168_328-pb.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-640_1280_2560.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-640_1280_2560.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-64_128-a_l_n.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-64_128-a_l_n.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-8_16_32-a_l_n.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-8_16_32-a_l_n.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/atmega-8_16_32-u2.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/atmega-8_16_32-u2.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-102_104.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-102_104.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-13.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-13.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-20.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-20.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-24_44_84.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-24_44_84.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-25_45_85.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-25_45_85.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-261_461_861.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-261_461_861.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-40.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-40.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-441_841.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-441_841.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-48_88.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-48_88.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/avr/attiny-4_5_9_10.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/avr/attiny-4_5_9_10.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52810.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52810.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52811.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52811.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52820.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52820.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52832.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52832.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52833.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52833.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/nrf/nrf52840.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/nrf/nrf52840.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/rp/rp2040.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/rp/rp2040.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/sam/samd09.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/sam/samd09.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/sam/samd10_d11.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/sam/samd10_d11.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/sam/samd20.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/sam/samd20.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/sam/samd21.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/sam/samd21.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/sam/samd51_e51_e53_e54.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/sam/samd51_e51_e53_e54.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/sam/samda1.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/sam/samda1.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/sam/same70_s70_v70_v71.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/sam/same70_s70_v70_v71.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/sam/samg51_g53_g54.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/sam/samg51_g53_g54.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/sam/samg55.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/sam/samg55.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/sam/saml21.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/sam/saml21.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/sam/saml22.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/sam/saml22.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-30.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-30.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-30.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-30.xml`

```diff
@@ -654,15 +654,16 @@
       <gpio device-pin="r" port="c" pin="6">
         <signal af="0" driver="tim" instance="3" name="ch1"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="7">
         <signal af="0" driver="tim" instance="3" name="ch2"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="8">
-        <signal af="0" driver="tim" instance="3" name="ch3"/>
+        <signal device-size="c" af="0" driver="tim" instance="3" name="ch3"/>
+        <signal device-size="8" af="1" driver="tim" instance="3" name="ch3"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="9">
         <signal af="0" driver="tim" instance="3" name="ch4"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="10">
         <signal device-size="c" af="0" driver="usart" instance="4" name="tx"/>
         <signal device-size="c" af="1" driver="usart" instance="3" name="tx"/>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-31.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-31.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-38.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-38.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-42.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-42.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-48.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-48.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-51.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-51.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-51.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-51.xml`

```diff
@@ -526,15 +526,15 @@
       <gpio device-pin="r" port="c" pin="6">
         <signal af="0" driver="tim" instance="3" name="ch1"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="7">
         <signal af="0" driver="tim" instance="3" name="ch2"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="8">
-        <signal af="0" driver="tim" instance="3" name="ch3"/>
+        <signal af="1" driver="tim" instance="3" name="ch3"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="9">
         <signal af="0" driver="tim" instance="3" name="ch4"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="10"/>
       <gpio device-pin="r" port="c" pin="11"/>
       <gpio device-pin="r" port="c" pin="12"/>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-58.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-58.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-58.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-58.xml`

```diff
@@ -464,15 +464,15 @@
       <gpio device-pin="r" port="c" pin="6">
         <signal af="0" driver="tim" instance="3" name="ch1"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="7">
         <signal af="0" driver="tim" instance="3" name="ch2"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="8">
-        <signal af="0" driver="tim" instance="3" name="ch3"/>
+        <signal af="1" driver="tim" instance="3" name="ch3"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="9">
         <signal af="0" driver="tim" instance="3" name="ch4"/>
       </gpio>
       <gpio device-pin="r" port="c" pin="10"/>
       <gpio device-pin="r" port="c" pin="11"/>
       <gpio device-pin="r" port="c" pin="12"/>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-70.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-70.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-71.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-71.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-72.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-72.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-78.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-78.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-91.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-91.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f0-98.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f0-98.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-00-4_6.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-00-4_6.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-00-8_b.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-00-8_b.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-00-c_d_e.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-00-c_d_e.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-01-c_d_e.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-01-c_d_e.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-01-f_g.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-01-f_g.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-01_02-4_6.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-01_02-4_6.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-01_02-8_b.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-01_02-8_b.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-03-4_6.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-03-4_6.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-03-8_b.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-03-8_b.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-03-c_d_e.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-03-c_d_e.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-03-f_g.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-03-f_g.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f1-05_07.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f1-05_07.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f2-05.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f2-05.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f2-07_15_17.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f2-07_15_17.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-01.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-01.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-02-6_8.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-02-6_8.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-02-b_c_d_e.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-02-b_c_d_e.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-03-6_8.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-03-6_8.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-03-b_c_d_e.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-03-b_c_d_e.xml`

 * *Files 6% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-03-b_c_d_e.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-03-b_c_d_e.xml`

```diff
@@ -156,16 +156,15 @@
     <driver name="flash" type="stm32-v1.0">
       <latency vcore-min="1800">
         <wait-state ws="0" hclk-max="24000000"/>
         <wait-state ws="1" hclk-max="48000000"/>
         <wait-state ws="2" hclk-max="72000000"/>
       </latency>
     </driver>
-    <driver device-pin="v" device-size="d|e" device-package="h|t" name="fmc" type="stm32-v1.0"/>
-    <driver device-pin="z" device-size="d|e" device-package="t" name="fmc" type="stm32-v1.0"/>
+    <driver device-pin="v|z" device-size="d|e" name="fmc" type="stm32-v1.0"/>
     <driver name="i2c" type="stm32-extended">
       <feature value="dnf"/>
       <feature value="fmp"/>
       <instance value="1"/>
       <instance value="2"/>
       <instance device-size="d|e" value="3"/>
     </driver>
@@ -674,16 +673,15 @@
         <signal af="1" driver="tim" instance="17" name="ch1n"/>
         <signal af="2" driver="tim" instance="4" name="ch2"/>
         <signal af="3" driver="tsc" name="g5_io4"/>
         <signal af="4" driver="i2c" instance="1" name="sda"/>
         <signal af="5" driver="tim" instance="8" name="bkin"/>
         <signal af="7" driver="usart" instance="1" name="rx"/>
         <signal af="10" driver="tim" instance="3" name="ch4"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="nl"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="nl"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="nl"/>
       </gpio>
       <gpio port="b" pin="8">
         <signal af="1" driver="tim" instance="16" name="ch1"/>
         <signal af="2" driver="tim" instance="4" name="ch3"/>
         <signal af="3" driver="tsc" name="sync"/>
         <signal af="4" driver="i2c" instance="1" name="scl"/>
         <signal device-size="d|e" af="7" driver="usart" instance="3" name="rx"/>
@@ -864,47 +862,41 @@
       <gpio port="c" pin="14">
         <signal driver="rcc" name="osc32_in"/>
       </gpio>
       <gpio port="c" pin="15">
         <signal driver="rcc" name="osc32_out"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="0">
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da2"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da2"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="da2"/>
         <signal af="7" driver="can" name="rx"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d2"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d2"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="d2"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="1">
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da3"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da3"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="da3"/>
         <signal af="4" driver="tim" instance="8" name="ch4"/>
         <signal af="6" driver="tim" instance="8" name="bkin2"/>
         <signal af="7" driver="can" name="tx"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d3"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d3"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="d3"/>
       </gpio>
       <gpio device-pin="r|v|z" port="d" pin="2">
         <signal af="2" driver="tim" instance="3" name="etr"/>
         <signal af="4" driver="tim" instance="8" name="bkin"/>
         <signal af="5" driver="uart" instance="5" name="rx"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="3">
         <signal af="2" driver="tim" instance="2" name="ch1"/>
         <signal af="2" driver="tim" instance="2" name="etr"/>
         <signal af="7" driver="usart" instance="2" name="cts"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="clk"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="clk"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="clk"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="4">
         <signal af="2" driver="tim" instance="2" name="ch2"/>
         <signal af="7" driver="usart" instance="2" name="de"/>
         <signal af="7" driver="usart" instance="2" name="rts"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="noe"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="noe"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="noe"/>
       </gpio>
       <gpio device-pin="v" device-package="h|t" port="d" pin="5">
         <signal af="7" driver="usart" instance="2" name="tx"/>
         <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="nwe"/>
         <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="nwe"/>
       </gpio>
       <gpio device-pin="z" device-package="t" port="d" pin="5">
@@ -923,18 +915,16 @@
         <signal af="7" driver="usart" instance="2" name="rx"/>
         <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="nwait"/>
         <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="nwait"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="7">
         <signal af="2" driver="tim" instance="2" name="ch3"/>
         <signal af="7" driver="usart" instance="2" name="ck"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="nce2"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="nce2"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="ne1"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="ne1"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="nce2"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="ne1"/>
       </gpio>
       <gpio device-pin="v" device-package="h|t" port="d" pin="8">
         <signal driver="adc" instance="4" name="in12"/>
         <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da13"/>
         <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da13"/>
         <signal driver="opamp" instance="4" name="vinm"/>
         <signal driver="opamp" instance="4" name="vinm_sec"/>
@@ -950,165 +940,141 @@
         <signal driver="opamp" instance="4" name="vinm_sec"/>
         <signal af="7" driver="usart" instance="3" name="tx"/>
         <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d13"/>
         <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d13"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="9">
         <signal driver="adc" instance="4" name="in13"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da14"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da14"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="da14"/>
         <signal af="7" driver="usart" instance="3" name="rx"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d14"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d14"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="d14"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="10">
         <signal driver="adc" instance="3" name="in7"/>
         <signal driver="adc" instance="4" name="in7"/>
         <signal driver="comp" instance="6" name="inm"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da15"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da15"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="da15"/>
         <signal af="7" driver="usart" instance="3" name="ck"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d15"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d15"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="d15"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="11">
         <signal driver="adc" instance="3" name="in8"/>
         <signal driver="adc" instance="4" name="in8"/>
         <signal device-pin="v" device-size="b|c" driver="comp" instance="6" name="inp"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="cle"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="cle"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="cle"/>
         <signal driver="opamp" instance="4" name="vinp"/>
         <signal driver="opamp" instance="4" name="vinp_sec"/>
         <signal af="7" driver="usart" instance="3" name="cts"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="a16"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="a16"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="a16"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="12">
         <signal driver="adc" instance="3" name="in9"/>
         <signal driver="adc" instance="4" name="in9"/>
         <signal device-pin="v" device-size="b|c" driver="comp" instance="5" name="inp"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="ale"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="ale"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="ale"/>
         <signal af="2" driver="tim" instance="4" name="ch1"/>
         <signal af="3" driver="tsc" name="g8_io1"/>
         <signal af="7" driver="usart" instance="3" name="de"/>
         <signal af="7" driver="usart" instance="3" name="rts"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="a17"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="a17"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="a17"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="13">
         <signal driver="adc" instance="3" name="in10"/>
         <signal driver="adc" instance="4" name="in10"/>
         <signal driver="comp" instance="5" name="inm"/>
         <signal af="2" driver="tim" instance="4" name="ch2"/>
         <signal af="3" driver="tsc" name="g8_io2"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="a18"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="a18"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="a18"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="14">
         <signal driver="adc" instance="3" name="in11"/>
         <signal driver="adc" instance="4" name="in11"/>
         <signal device-pin="v" device-size="b|c" driver="comp" instance="3" name="inp"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da0"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da0"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="da0"/>
         <signal driver="opamp" instance="2" name="vinp"/>
         <signal driver="opamp" instance="2" name="vinp_sec"/>
         <signal af="2" driver="tim" instance="4" name="ch3"/>
         <signal af="3" driver="tsc" name="g8_io3"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d0"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d0"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="d0"/>
       </gpio>
       <gpio device-pin="v|z" port="d" pin="15">
         <signal driver="comp" instance="3" name="inm"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da1"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da1"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="da1"/>
         <signal af="2" driver="tim" instance="4" name="ch4"/>
         <signal af="3" driver="tsc" name="g8_io4"/>
         <signal af="6" driver="spi" instance="2" name="nss"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d1"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d1"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="d1"/>
       </gpio>
       <gpio device-pin="v|z" port="e" pin="0">
         <signal af="2" driver="tim" instance="4" name="etr"/>
         <signal af="4" driver="tim" instance="16" name="ch1"/>
         <signal device-pin="v|z" device-size="d|e" af="6" driver="tim" instance="20" name="etr"/>
         <signal af="7" driver="usart" instance="1" name="tx"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="nbl0"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="nbl0"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="nbl0"/>
       </gpio>
       <gpio device-pin="v|z" port="e" pin="1">
         <signal af="4" driver="tim" instance="17" name="ch1"/>
         <signal device-pin="v|z" device-size="d|e" af="6" driver="tim" instance="20" name="ch4"/>
         <signal af="7" driver="usart" instance="1" name="rx"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="nbl1"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="nbl1"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="nbl1"/>
       </gpio>
       <gpio device-pin="v|z" port="e" pin="2">
         <signal af="0" driver="sys" name="traceck"/>
         <signal af="2" driver="tim" instance="3" name="ch1"/>
         <signal af="3" driver="tsc" name="g7_io1"/>
         <signal device-pin="v|z" device-size="d|e" af="5" driver="spi" instance="4" name="sck"/>
         <signal device-pin="v|z" device-size="d|e" af="6" driver="tim" instance="20" name="ch1"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="a23"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="a23"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="a23"/>
       </gpio>
       <gpio device-pin="v|z" port="e" pin="3">
         <signal af="0" driver="sys" name="traced0"/>
         <signal af="2" driver="tim" instance="3" name="ch2"/>
         <signal af="3" driver="tsc" name="g7_io2"/>
         <signal device-pin="v|z" device-size="d|e" af="5" driver="spi" instance="4" name="nss"/>
         <signal device-pin="v|z" device-size="d|e" af="6" driver="tim" instance="20" name="ch2"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="a19"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="a19"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="a19"/>
       </gpio>
       <gpio device-pin="v|z" port="e" pin="4">
         <signal af="0" driver="sys" name="traced1"/>
         <signal af="2" driver="tim" instance="3" name="ch3"/>
         <signal af="3" driver="tsc" name="g7_io3"/>
         <signal device-pin="v|z" device-size="d|e" af="5" driver="spi" instance="4" name="nss"/>
         <signal device-pin="v|z" device-size="d|e" af="6" driver="tim" instance="20" name="ch1n"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="a20"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="a20"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="a20"/>
       </gpio>
       <gpio device-pin="v|z" port="e" pin="5">
         <signal af="0" driver="sys" name="traced2"/>
         <signal af="2" driver="tim" instance="3" name="ch4"/>
         <signal af="3" driver="tsc" name="g7_io4"/>
         <signal device-pin="v|z" device-size="d|e" af="5" driver="spi" instance="4" name="miso"/>
         <signal device-pin="v|z" device-size="d|e" af="6" driver="tim" instance="20" name="ch2n"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="a21"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="a21"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="a21"/>
       </gpio>
       <gpio device-pin="v|z" port="e" pin="6">
         <signal driver="rtc" name="tamp3"/>
         <signal driver="sys" name="wkup3"/>
         <signal af="0" driver="sys" name="traced3"/>
         <signal device-pin="v|z" device-size="d|e" af="5" driver="spi" instance="4" name="mosi"/>
         <signal device-pin="v|z" device-size="d|e" af="6" driver="tim" instance="20" name="ch3n"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="a22"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="a22"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="a22"/>
       </gpio>
       <gpio device-pin="v|z" port="e" pin="7">
         <signal driver="adc" instance="3" name="in13"/>
         <signal device-pin="v" device-size="b|c" driver="comp" instance="4" name="inp"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da4"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da4"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="da4"/>
         <signal af="2" driver="tim" instance="1" name="etr"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d4"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d4"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="d4"/>
       </gpio>
       <gpio device-pin="v|z" port="e" pin="8">
         <signal driver="adc" instance="3" name="in6"/>
         <signal driver="adc" instance="4" name="in6"/>
         <signal driver="comp" instance="4" name="inm"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da5"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da5"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="da5"/>
         <signal af="2" driver="tim" instance="1" name="ch1n"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d5"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d5"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="d5"/>
       </gpio>
       <gpio device-pin="v" device-package="h|t" port="e" pin="9">
         <signal driver="adc" instance="3" name="in2"/>
         <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da6"/>
         <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da6"/>
         <signal af="2" driver="tim" instance="1" name="ch1"/>
         <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d6"/>
@@ -1136,29 +1102,25 @@
         <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da7"/>
         <signal af="2" driver="tim" instance="1" name="ch2n"/>
         <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d7"/>
         <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d7"/>
       </gpio>
       <gpio device-pin="v|z" port="e" pin="11">
         <signal driver="adc" instance="3" name="in15"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da8"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da8"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="da8"/>
         <signal af="2" driver="tim" instance="1" name="ch2"/>
         <signal device-pin="v|z" device-size="d|e" af="5" driver="spi" instance="4" name="nss"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d8"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d8"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="d8"/>
       </gpio>
       <gpio device-pin="v|z" port="e" pin="12">
         <signal driver="adc" instance="3" name="in16"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da9"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da9"/>
+        <signal device-pin="v|z" device-size="d|e" driver="fmc" name="da9"/>
         <signal af="2" driver="tim" instance="1" name="ch3n"/>
         <signal device-pin="v|z" device-size="d|e" af="5" driver="spi" instance="4" name="sck"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="d9"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="d9"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="d9"/>
       </gpio>
       <gpio device-pin="v" device-package="h|t" port="e" pin="13">
         <signal driver="adc" instance="3" name="in3"/>
         <signal device-pin="v" device-size="d|e" device-package="h|t" driver="fmc" name="da10"/>
         <signal device-pin="z" device-size="d|e" device-package="t" driver="fmc" name="da10"/>
         <signal af="2" driver="tim" instance="1" name="ch3"/>
         <signal device-pin="v" device-size="d|e" device-package="h|t" af="5" driver="spi" instance="4" name="miso"/>
@@ -1229,16 +1191,15 @@
         <signal device-size="d|e" af="5" driver="i2s" instance="2" name="ck"/>
         <signal device-size="d|e" af="5" driver="spi" instance="2" name="sck"/>
       </gpio>
       <gpio device-pin="v|z" port="f" pin="2">
         <signal driver="adc" instance="1" name="in10"/>
         <signal driver="adc" instance="2" name="in10"/>
         <signal device-pin="v|z" device-size="d|e" af="2" driver="tim" instance="20" name="ch3"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="a2"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="a2"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="a2"/>
       </gpio>
       <gpio device-pin="z" port="f" pin="3">
         <signal af="2" driver="tim" instance="20" name="ch4"/>
         <signal af="12" driver="fmc" name="a3"/>
       </gpio>
       <gpio device-pin="r|v" device-size="b|c" device-package="t" port="f" pin="4">
         <signal driver="adc" instance="1" name="in5"/>
@@ -1257,38 +1218,35 @@
         <signal af="12" driver="fmc" name="a5"/>
       </gpio>
       <gpio device-pin="v|z" port="f" pin="6">
         <signal af="2" driver="tim" instance="4" name="ch4"/>
         <signal af="4" driver="i2c" instance="2" name="scl"/>
         <signal af="7" driver="usart" instance="3" name="de"/>
         <signal af="7" driver="usart" instance="3" name="rts"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="niord"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="niord"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="niord"/>
       </gpio>
       <gpio device-pin="z" port="f" pin="7">
         <signal af="2" driver="tim" instance="20" name="bkin"/>
         <signal af="12" driver="fmc" name="nreg"/>
       </gpio>
       <gpio device-pin="z" port="f" pin="8">
         <signal af="2" driver="tim" instance="20" name="bkin2"/>
         <signal af="12" driver="fmc" name="niowr"/>
       </gpio>
       <gpio device-pin="v|z" port="f" pin="9">
         <signal device-pin="v|z" device-size="d|e" af="2" driver="tim" instance="20" name="bkin"/>
         <signal af="3" driver="tim" instance="15" name="ch1"/>
         <signal af="5" driver="spi" instance="2" name="sck"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="cd"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="cd"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="cd"/>
       </gpio>
       <gpio device-pin="v|z" port="f" pin="10">
         <signal device-pin="v|z" device-size="d|e" af="2" driver="tim" instance="20" name="bkin2"/>
         <signal af="3" driver="tim" instance="15" name="ch2"/>
         <signal af="5" driver="spi" instance="2" name="sck"/>
-        <signal device-pin="v" device-size="d|e" device-package="h|t" af="12" driver="fmc" name="intr"/>
-        <signal device-pin="z" device-size="d|e" device-package="t" af="12" driver="fmc" name="intr"/>
+        <signal device-pin="v|z" device-size="d|e" af="12" driver="fmc" name="intr"/>
       </gpio>
       <gpio device-pin="z" port="f" pin="11">
         <signal af="2" driver="tim" instance="20" name="etr"/>
       </gpio>
       <gpio device-pin="z" port="f" pin="12">
         <signal af="2" driver="tim" instance="20" name="ch1"/>
         <signal af="12" driver="fmc" name="a6"/>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-18_28.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-18_28.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-34.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-34.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-58_98.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-58_98.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f3-73_78.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f3-73_78.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-01_11.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-01_11.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-05_07_15_17.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-05_07_15_17.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-10.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-10.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-12.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-12.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-13_23.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-13_23.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-27_29_37_39.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-27_29_37_39.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-46.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-46.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-69_79.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-69_79.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f4-69_79.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f4-69_79.xml`

```diff
@@ -762,14 +762,15 @@
         <signal af="2" driver="tim" instance="3" name="ch2"/>
         <signal af="3" driver="tim" instance="8" name="ch1n"/>
         <signal af="5" driver="spi" instance="1" name="mosi"/>
         <signal af="9" driver="tim" instance="14" name="ch1"/>
         <signal af="10" driver="quadspi" name="clk"/>
         <signal device-pin="b|i|n" af="11" driver="eth" name="rcc_crs_dv"/>
         <signal device-pin="b|i|n" af="11" driver="eth" name="rx_dv"/>
+        <signal af="12" driver="fmc" name="sdnwe"/>
       </gpio>
       <gpio port="a" pin="8">
         <signal af="0" driver="rcc" name="mco_1"/>
         <signal af="1" driver="tim" instance="1" name="ch1"/>
         <signal af="4" driver="i2c" instance="3" name="scl"/>
         <signal af="7" driver="usart" instance="1" name="ck"/>
         <signal af="10" driver="usb_otg_fs" name="sof"/>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f7-22_23_32_33.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f7-22_23_32_33.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f7-30_50.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f7-30_50.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f7-45_46_56.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f7-45_46_56.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32f7-65_67_68_69_77_78_79.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32f7-65_67_68_69_77_78_79.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-30.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-30.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-31_41.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-31_41.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-50.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-50.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-51_61.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-51_61.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-70_b0.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-70_b0.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-71_81.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-71_81.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g0-b1_c1.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g0-b1_c1.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g4-31_41.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g4-31_41.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g4-71.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g4-71.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g4-73_83.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g4-73_83.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g4-74_84.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g4-74_84.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32g4-91_a1.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32g4-91_a1.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-23_33.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-23_33.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-23_33.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-23_33.xml`

```diff
@@ -569,15 +569,16 @@
         <request position="73">
           <signal driver="i2c" instance="3" name="rx"/>
         </request>
         <request position="74">
           <signal driver="i2c" instance="3" name="tx"/>
         </request>
         <request position="75">
-          <signal driver="dcmi" name="pssi"/>
+          <signal driver="dcmi"/>
+          <signal driver="pssi"/>
         </request>
         <request device-name="33" position="76">
           <signal driver="cryp" name="in"/>
         </request>
         <request device-name="33" position="77">
           <signal driver="cryp" name="out"/>
         </request>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-25_35.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-25_35.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-25_35.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-25_35.xml`

```diff
@@ -610,15 +610,16 @@
         <request position="73">
           <signal driver="i2c" instance="3" name="rx"/>
         </request>
         <request position="74">
           <signal driver="i2c" instance="3" name="tx"/>
         </request>
         <request position="75">
-          <signal driver="dcmi" name="pssi"/>
+          <signal driver="dcmi"/>
+          <signal driver="pssi"/>
         </request>
         <request device-name="35" position="76">
           <signal driver="cryp" name="in"/>
         </request>
         <request device-name="35" position="77">
           <signal driver="cryp" name="out"/>
         </request>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-30.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-30.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-30.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-30.xml`

```diff
@@ -562,15 +562,16 @@
         <request position="73">
           <signal driver="i2c" instance="3" name="rx"/>
         </request>
         <request position="74">
           <signal driver="i2c" instance="3" name="tx"/>
         </request>
         <request position="75">
-          <signal driver="dcmi" name="pssi"/>
+          <signal driver="dcmi"/>
+          <signal driver="pssi"/>
         </request>
         <request position="76">
           <signal driver="cryp" name="in"/>
         </request>
         <request position="77">
           <signal driver="cryp" name="out"/>
         </request>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-42.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-42.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-42.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-42.xml`

```diff
@@ -2859,15 +2859,15 @@
         <pin position="E12" name="PD1"/>
         <pin position="E13" name="PC8"/>
         <pin position="E14" name="PC9"/>
         <pin position="E15" name="PA8"/>
         <pin position="E16" name="PA12"/>
         <pin position="E17" name="PA11"/>
         <pin position="F1" name="VSS" type="power"/>
-        <pin position="F2" name="NC" type="nc"/>
+        <pin position="F2" name="VSS" type="power"/>
         <pin position="F3" name="PI10"/>
         <pin position="F4" name="PI11"/>
         <pin position="F5" name="VDD" type="power"/>
         <pin position="F13" name="PC7"/>
         <pin position="F14" name="PC6"/>
         <pin position="F15" name="PG8"/>
         <pin position="F16" name="PG7"/>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-43_53.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-43_53.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-45_55.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-45_55.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-47_57.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-47_57.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-50.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-50.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-a3.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-a3.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-a3.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-a3.xml`

```diff
@@ -587,15 +587,16 @@
         <request position="73">
           <signal driver="i2c" instance="3" name="rx"/>
         </request>
         <request position="74">
           <signal driver="i2c" instance="3" name="tx"/>
         </request>
         <request position="75">
-          <signal driver="dcmi" name="pssi"/>
+          <signal driver="dcmi"/>
+          <signal driver="pssi"/>
         </request>
         <request position="79">
           <signal driver="uart" instance="7" name="rx"/>
         </request>
         <request position="80">
           <signal driver="uart" instance="7" name="tx"/>
         </request>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-b0.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-b0.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-b0.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-b0.xml`

```diff
@@ -560,15 +560,16 @@
         <request position="73">
           <signal driver="i2c" instance="3" name="rx"/>
         </request>
         <request position="74">
           <signal driver="i2c" instance="3" name="tx"/>
         </request>
         <request position="75">
-          <signal driver="dcmi" name="pssi"/>
+          <signal driver="dcmi"/>
+          <signal driver="pssi"/>
         </request>
         <request position="76">
           <signal driver="cryp" name="in"/>
         </request>
         <request position="77">
           <signal driver="cryp" name="out"/>
         </request>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-b3.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-b3.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32h7-b3.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32h7-b3.xml`

```diff
@@ -582,15 +582,16 @@
         <request position="73">
           <signal driver="i2c" instance="3" name="rx"/>
         </request>
         <request position="74">
           <signal driver="i2c" instance="3" name="tx"/>
         </request>
         <request position="75">
-          <signal driver="dcmi" name="pssi"/>
+          <signal driver="dcmi"/>
+          <signal driver="pssi"/>
         </request>
         <request position="76">
           <signal driver="cryp" name="in"/>
         </request>
         <request position="77">
           <signal driver="cryp" name="out"/>
         </request>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l0-10.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l0-10.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l0-11_21.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l0-11_21.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l0-31_41.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l0-31_41.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l0-51_52_53_62_63.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l0-51_52_53_62_63.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l0-71_72_73_81_82_83.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l0-71_72_73_81_82_83.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l1-00.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l1-00.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l1-00.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l1-00.xml`

```diff
@@ -300,23 +300,23 @@
       </gpio>
       <gpio port="a" pin="10">
         <signal af="7" driver="usart" instance="1" name="rx"/>
         <signal af="11" driver="lcd" name="com2"/>
         <signal af="14" driver="tim" name="ic3"/>
       </gpio>
       <gpio port="a" pin="11">
+        <signal driver="usb" name="dm"/>
         <signal af="5" driver="spi" instance="1" name="miso"/>
         <signal af="7" driver="usart" instance="1" name="cts"/>
-        <signal af="10" driver="usb" name="dm"/>
         <signal af="14" driver="tim" name="ic4"/>
       </gpio>
       <gpio port="a" pin="12">
+        <signal driver="usb" name="dp"/>
         <signal af="5" driver="spi" instance="1" name="mosi"/>
         <signal af="7" driver="usart" instance="1" name="rts"/>
-        <signal af="10" driver="usb" name="dp"/>
         <signal af="14" driver="tim" name="ic1"/>
       </gpio>
       <gpio port="a" pin="13">
         <signal af="0" driver="sys" name="jtms"/>
         <signal af="0" driver="sys" name="swdio"/>
         <signal af="14" driver="tim" name="ic2"/>
       </gpio>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l1-51_52-6_8_b.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l1-51_52-6_8_b.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l1-51_52-6_8_b.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l1-51_52-6_8_b.xml`

```diff
@@ -345,23 +345,23 @@
       <gpio port="a" pin="10">
         <signal af="7" driver="usart" instance="1" name="rx"/>
         <signal device-name="52" af="11" driver="lcd" name="com2"/>
         <signal af="14" driver="tim" name="ic3"/>
         <signal af="14" driver="ts" name="g4_io3"/>
       </gpio>
       <gpio port="a" pin="11">
+        <signal driver="usb" name="dm"/>
         <signal af="5" driver="spi" instance="1" name="miso"/>
         <signal af="7" driver="usart" instance="1" name="cts"/>
-        <signal af="10" driver="usb" name="dm"/>
         <signal af="14" driver="tim" name="ic4"/>
       </gpio>
       <gpio port="a" pin="12">
+        <signal driver="usb" name="dp"/>
         <signal af="5" driver="spi" instance="1" name="mosi"/>
         <signal af="7" driver="usart" instance="1" name="rts"/>
-        <signal af="10" driver="usb" name="dp"/>
         <signal af="14" driver="tim" name="ic1"/>
       </gpio>
       <gpio port="a" pin="13">
         <signal af="0" driver="sys" name="jtms"/>
         <signal af="0" driver="sys" name="swdio"/>
         <signal af="14" driver="tim" name="ic2"/>
         <signal af="14" driver="ts" name="g5_io1"/>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l1-51_52_62-c_d_e.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l1-51_52_62-c_d_e.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l1-51_52_62-c_d_e.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l1-51_52_62-c_d_e.xml`

```diff
@@ -459,29 +459,23 @@
       <gpio port="a" pin="10">
         <signal af="7" driver="usart" instance="1" name="rx"/>
         <signal device-name="52|62" af="11" driver="lcd" name="com2"/>
         <signal af="14" driver="tim" name="ic3"/>
         <signal af="14" driver="ts" name="g4_io3"/>
       </gpio>
       <gpio port="a" pin="11">
-        <signal device-size="d" device-variant="x" driver="usb" name="dm"/>
-        <signal device-size="e" device-variant="" driver="usb" name="dm"/>
+        <signal driver="usb" name="dm"/>
         <signal af="5" driver="spi" instance="1" name="miso"/>
         <signal af="7" driver="usart" instance="1" name="cts"/>
-        <signal device-size="c|d" device-variant="" af="10" driver="usb" name="dm"/>
-        <signal device-size="c" device-variant="a" af="10" driver="usb" name="dm"/>
         <signal af="14" driver="tim" name="ic4"/>
       </gpio>
       <gpio port="a" pin="12">
-        <signal device-size="d" device-variant="x" driver="usb" name="dp"/>
-        <signal device-size="e" device-variant="" driver="usb" name="dp"/>
+        <signal driver="usb" name="dp"/>
         <signal af="5" driver="spi" instance="1" name="mosi"/>
         <signal af="7" driver="usart" instance="1" name="rts"/>
-        <signal device-size="c|d" device-variant="" af="10" driver="usb" name="dp"/>
-        <signal device-size="c" device-variant="a" af="10" driver="usb" name="dp"/>
         <signal af="14" driver="tim" name="ic1"/>
       </gpio>
       <gpio port="a" pin="13">
         <signal af="0" driver="sys" name="jtms"/>
         <signal af="0" driver="sys" name="swdio"/>
         <signal af="14" driver="tim" name="ic2"/>
         <signal af="14" driver="ts" name="g5_io1"/>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-12_22.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-12_22.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-31_33_43.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-31_33_43.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-32_42.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-32_42.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-51_71.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-51_71.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-52_62.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-52_62.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-75_85.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-75_85.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-76_86.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-76_86.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-96_a6.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-96_a6.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-96_a6.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-96_a6.xml`

```diff
@@ -1042,15 +1042,15 @@
         <signal af="6" driver="dfsdm" instance="1" name="ckin7"/>
         <signal af="7" driver="usart" instance="3" name="rx"/>
         <signal af="8" driver="lpuart" instance="1" name="tx"/>
         <signal af="10" driver="quadspi" name="bk1_ncs"/>
         <signal af="11" driver="lcd" name="seg11"/>
         <signal af="12" driver="comp" instance="2" name="out"/>
       </gpio>
-      <gpio device-pin="q" device-package="i" device-variant="" port="b" pin="11">
+      <gpio device-pin="q" device-package="i" device-variant="|s" port="b" pin="11">
         <signal af="1" driver="tim" instance="2" name="ch4"/>
         <signal af="3" driver="i2c" instance="4" name="sda"/>
         <signal af="4" driver="i2c" instance="2" name="sda"/>
         <signal af="6" driver="dfsdm" instance="1" name="ckin7"/>
         <signal af="7" driver="usart" instance="3" name="rx"/>
         <signal af="8" driver="lpuart" instance="1" name="tx"/>
         <signal af="10" driver="quadspi" name="bk1_ncs"/>
@@ -1954,15 +1954,15 @@
         <signal af="7" driver="usart" instance="1" name="ck"/>
         <signal af="12" driver="fmc" name="a24"/>
       </gpio>
       <gpio device-pin="a|z" device-variant="|p" port="g" pin="14">
         <signal af="4" driver="i2c" instance="1" name="scl"/>
         <signal af="12" driver="fmc" name="a25"/>
       </gpio>
-      <gpio device-pin="q" device-variant="" port="g" pin="14">
+      <gpio device-pin="q" device-variant="|s" port="g" pin="14">
         <signal af="4" driver="i2c" instance="1" name="scl"/>
         <signal af="12" driver="fmc" name="a25"/>
       </gpio>
       <gpio device-pin="w" device-variant="p" port="g" pin="14">
         <signal af="4" driver="i2c" instance="1" name="scl"/>
         <signal af="12" driver="fmc" name="a25"/>
       </gpio>
@@ -2530,18 +2530,18 @@
         <pin position="B11" name="PC10"/>
         <pin position="B12" name="PA11"/>
         <pin position="C1" name="PC13"/>
         <pin position="C2" name="PE5"/>
         <pin position="C3" name="PE0"/>
         <pin position="C4" name="VDD" type="power"/>
         <pin position="C5" name="PB5"/>
-        <pin device-name="96" device-size="g" device-temperature="3|6|7" device-variant="p|s" position="C6" name="VDD12" type="power"/>
+        <pin device-name="96" device-size="g" device-temperature="3|6|7" device-variant="p" position="C6" name="VDD12" type="power"/>
         <pin device-name="a6" device-size="g" device-temperature="6" device-variant="p" position="C6" name="VDD12" type="power"/>
         <pin device-name="96" device-size="e|g" device-temperature="6" device-variant="" position="C6" name="PG14"/>
-        <pin device-name="96" device-size="g" device-temperature="3|7" device-variant="" position="C6" name="PG14"/>
+        <pin device-name="96" device-size="g" device-temperature="3|6|7" device-variant="|s" position="C6" name="PG14"/>
         <pin device-name="a6" device-size="g" device-temperature="6" device-variant="" position="C6" name="PG14"/>
         <pin position="C7" name="PG13"/>
         <pin position="C8" name="PD2"/>
         <pin position="C9" name="PD0"/>
         <pin position="C10" name="PC11"/>
         <pin position="C11" name="VDDUSB" type="power"/>
         <pin position="C12" name="PA10"/>
@@ -2623,18 +2623,18 @@
         <pin position="L4" name="PA6"/>
         <pin position="L5" name="PC5"/>
         <pin position="L6" name="PB2"/>
         <pin position="L7" name="PE8"/>
         <pin position="L8" name="PE10"/>
         <pin position="L9" name="PE12"/>
         <pin position="L10" name="PB10"/>
-        <pin device-name="96" device-size="g" device-temperature="3|6|7" device-variant="p|s" position="L11" name="VDD12" type="power"/>
+        <pin device-name="96" device-size="g" device-temperature="3|6|7" device-variant="p" position="L11" name="VDD12" type="power"/>
         <pin device-name="a6" device-size="g" device-temperature="6" device-variant="p" position="L11" name="VDD12" type="power"/>
         <pin device-name="96" device-size="e|g" device-temperature="6" device-variant="" position="L11" name="PB11"/>
-        <pin device-name="96" device-size="g" device-temperature="3|7" device-variant="" position="L11" name="PB11"/>
+        <pin device-name="96" device-size="g" device-temperature="3|6|7" device-variant="|s" position="L11" name="PB11"/>
         <pin device-name="a6" device-size="g" device-temperature="6" device-variant="" position="L11" name="PB11"/>
         <pin position="L12" name="PB12"/>
         <pin position="M1" name="VDDA" type="power"/>
         <pin position="M2" name="PA1"/>
         <pin position="M3" name="OPAMP1_VINM" type="monoio"/>
         <pin position="M4" name="OPAMP2_VINM" type="monoio"/>
         <pin position="M5" name="PB0"/>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-p5.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-p5.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-q5.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-q5.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-r5_r7_r9.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-r5_r7_r9.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l4-s5_s7_s9.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l4-s5_s7_s9.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l5-52_62.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l5-52_62.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32l5-52_62.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32l5-52_62.xml`

```diff
@@ -669,15 +669,14 @@
         <signal driver="rcc" name="lsco"/>
         <signal af="1" driver="tim" instance="2" name="ch3"/>
         <signal af="2" driver="tim" instance="5" name="ch3"/>
         <signal af="7" driver="usart" instance="2" name="tx"/>
         <signal af="8" driver="lpuart" instance="1" name="tx"/>
         <signal af="10" driver="octospi" instance="1" name="ncs"/>
         <signal af="11" driver="ucpd" instance="1" name="frstx1"/>
-        <signal af="11" driver="ucpd" instance="1" name="frstx2"/>
         <signal af="13" driver="sai" instance="2" name="extclk"/>
         <signal af="14" driver="tim" instance="15" name="ch1"/>
       </gpio>
       <gpio port="a" pin="3">
         <signal driver="adc" instance="1" name="in8"/>
         <signal driver="adc" instance="2" name="in8"/>
         <signal driver="opamp" instance="1" name="vout"/>
@@ -838,15 +837,14 @@
         <signal driver="comp" instance="1" name="inp"/>
         <signal driver="rtc" name="out2"/>
         <signal af="1" driver="lptim" instance="1" name="out"/>
         <signal af="4" driver="i2c" instance="3" name="smba"/>
         <signal af="6" driver="dfsdm" instance="1" name="ckin0"/>
         <signal af="10" driver="octospi" instance="1" name="dqs"/>
         <signal af="11" driver="ucpd" instance="1" name="frstx1"/>
-        <signal af="11" driver="ucpd" instance="1" name="frstx2"/>
       </gpio>
       <gpio port="b" pin="3">
         <signal driver="comp" instance="2" name="inm"/>
         <signal af="0" driver="debug" name="jtdo"/>
         <signal af="0" driver="debug" name="swo"/>
         <signal af="1" driver="tim" instance="2" name="ch2"/>
         <signal af="5" driver="spi" instance="1" name="sck"/>
@@ -1106,15 +1104,14 @@
         <signal af="4" driver="i2c" instance="2" name="scl"/>
         <signal af="5" driver="spi" instance="2" name="sck"/>
         <signal af="6" driver="dfsdm" instance="1" name="ckin1"/>
         <signal af="7" driver="usart" instance="3" name="cts"/>
         <signal af="7" driver="usart" instance="3" name="nss"/>
         <signal af="8" driver="lpuart" instance="1" name="cts"/>
         <signal af="9" driver="tsc" name="g1_io2"/>
-        <signal af="11" driver="ucpd" instance="1" name="frstx1"/>
         <signal af="11" driver="ucpd" instance="1" name="frstx2"/>
         <signal af="13" driver="sai" instance="2" name="sck_a"/>
         <signal af="14" driver="tim" instance="15" name="ch1n"/>
       </gpio>
       <gpio port="b" pin="14">
         <signal driver="ucpd" instance="1" name="dbcc2"/>
         <signal af="1" driver="tim" instance="1" name="ch2n"/>
@@ -1301,15 +1298,14 @@
       <gpio device-pin="m|q|r|v|z" port="c" pin="11">
         <signal af="2" driver="lptim" instance="3" name="in1"/>
         <signal af="5" driver="octospi" instance="1" name="ncs"/>
         <signal af="6" driver="spi" instance="3" name="miso"/>
         <signal af="7" driver="usart" instance="3" name="rx"/>
         <signal af="8" driver="uart" instance="4" name="rx"/>
         <signal af="9" driver="tsc" name="g3_io3"/>
-        <signal af="11" driver="ucpd" instance="1" name="frstx1"/>
         <signal af="11" driver="ucpd" instance="1" name="frstx2"/>
         <signal device-pin="r|v|z" device-variant="|q" af="12" driver="sdmmc" instance="1" name="d3"/>
         <signal device-pin="m" device-variant="p|q" af="12" driver="sdmmc" instance="1" name="d3"/>
         <signal device-pin="q" device-variant="|p|q" af="12" driver="sdmmc" instance="1" name="d3"/>
         <signal af="13" driver="sai" instance="2" name="mclk_b"/>
       </gpio>
       <gpio device-pin="m|q|r|v|z" port="c" pin="12">
@@ -1752,22 +1748,20 @@
       </gpio>
       <gpio device-pin="q|z" port="g" pin="6">
         <signal af="3" driver="octospi" instance="1" name="dqs"/>
         <signal af="4" driver="i2c" instance="3" name="smba"/>
         <signal af="8" driver="lpuart" instance="1" name="de"/>
         <signal af="8" driver="lpuart" instance="1" name="rts"/>
         <signal af="11" driver="ucpd" instance="1" name="frstx1"/>
-        <signal af="11" driver="ucpd" instance="1" name="frstx2"/>
       </gpio>
       <gpio device-pin="q|z" port="g" pin="7">
         <signal af="3" driver="sai" instance="1" name="ck1"/>
         <signal af="4" driver="i2c" instance="3" name="scl"/>
         <signal af="6" driver="dfsdm" instance="1" name="ckout"/>
         <signal af="8" driver="lpuart" instance="1" name="tx"/>
-        <signal af="11" driver="ucpd" instance="1" name="frstx1"/>
         <signal af="11" driver="ucpd" instance="1" name="frstx2"/>
         <signal af="12" driver="fmc" name="int"/>
         <signal af="13" driver="sai" instance="1" name="mclk_a"/>
       </gpio>
       <gpio device-pin="q|z" port="g" pin="8">
         <signal af="4" driver="i2c" instance="3" name="sda"/>
         <signal af="8" driver="lpuart" instance="1" name="rx"/>
@@ -1904,22 +1898,22 @@
         <pin position="16" name="PC1"/>
         <pin position="17" name="PC2"/>
         <pin position="18" name="PC3"/>
         <pin device-name="52" device-size="c|e" device-variant="q" position="19" name="VSSA/VREF-" type="power"/>
         <pin device-name="52" device-size="e" device-variant="" position="19" name="VSSA/VREF-" type="power"/>
         <pin device-name="62" device-size="e" device-variant="q" position="19" name="VSSA/VREF-" type="power"/>
         <pin device-name="62" device-size="e" device-variant="" position="19" name="VSSA" type="power"/>
-        <pin device-name="52" device-size="c|e" device-variant="q" position="20" name="VREF+" type="monoio"/>
-        <pin device-name="52" device-size="e" device-variant="" position="20" name="VREF+" type="monoio"/>
-        <pin device-name="62" device-size="e" device-variant="q" position="20" name="VREF+" type="monoio"/>
+        <pin device-name="52" device-size="c|e" device-variant="q" position="20" name="VREF+" type="power"/>
+        <pin device-name="52" device-size="e" device-variant="" position="20" name="VREF+" type="power"/>
+        <pin device-name="62" device-size="e" device-variant="q" position="20" name="VREF+" type="power"/>
         <pin device-name="62" device-size="e" device-variant="" position="20" name="VREF-" type="power"/>
         <pin device-name="52" device-size="c|e" device-variant="q" position="21" name="VDDA" type="power"/>
         <pin device-name="52" device-size="e" device-variant="" position="21" name="VDDA" type="power"/>
         <pin device-name="62" device-size="e" device-variant="q" position="21" name="VDDA" type="power"/>
-        <pin device-name="62" device-size="e" device-variant="" position="21" name="VREF+" type="monoio"/>
+        <pin device-name="62" device-size="e" device-variant="" position="21" name="VREF+" type="power"/>
         <pin device-name="52" device-size="c|e" device-variant="q" position="22" name="PA0"/>
         <pin device-name="52" device-size="e" device-variant="" position="22" name="PA0"/>
         <pin device-name="62" device-size="e" device-variant="q" position="22" name="PA0"/>
         <pin device-name="62" device-size="e" device-variant="" position="22" name="VDDA" type="power"/>
         <pin device-name="52" device-size="c|e" device-variant="q" position="23" name="PA1"/>
         <pin device-name="52" device-size="e" device-variant="" position="23" name="PA1"/>
         <pin device-name="62" device-size="e" device-variant="q" position="23" name="PA1"/>
@@ -2119,22 +2113,22 @@
         <pin position="27" name="PC1"/>
         <pin position="28" name="PC2"/>
         <pin position="29" name="PC3"/>
         <pin device-name="52" device-size="c|e" device-temperature="6" device-variant="q" position="30" name="VSSA/VREF-" type="power"/>
         <pin device-name="52" device-size="e" device-temperature="3|6|7" device-variant="|q" position="30" name="VSSA/VREF-" type="power"/>
         <pin device-name="62" device-size="e" device-temperature="6" device-variant="q" position="30" name="VSSA/VREF-" type="power"/>
         <pin device-name="62" device-size="e" device-temperature="6" device-variant="" position="30" name="VSSA" type="power"/>
-        <pin device-name="52" device-size="c|e" device-temperature="6" device-variant="q" position="31" name="VREF+" type="monoio"/>
-        <pin device-name="52" device-size="e" device-temperature="3|6|7" device-variant="|q" position="31" name="VREF+" type="monoio"/>
-        <pin device-name="62" device-size="e" device-temperature="6" device-variant="q" position="31" name="VREF+" type="monoio"/>
+        <pin device-name="52" device-size="c|e" device-temperature="6" device-variant="q" position="31" name="VREF+" type="power"/>
+        <pin device-name="52" device-size="e" device-temperature="3|6|7" device-variant="|q" position="31" name="VREF+" type="power"/>
+        <pin device-name="62" device-size="e" device-temperature="6" device-variant="q" position="31" name="VREF+" type="power"/>
         <pin device-name="62" device-size="e" device-temperature="6" device-variant="" position="31" name="VREF-" type="power"/>
         <pin device-name="52" device-size="c|e" device-temperature="6" device-variant="q" position="32" name="VDDA" type="power"/>
         <pin device-name="52" device-size="e" device-temperature="3|6|7" device-variant="|q" position="32" name="VDDA" type="power"/>
         <pin device-name="62" device-size="e" device-temperature="6" device-variant="q" position="32" name="VDDA" type="power"/>
-        <pin device-name="62" device-size="e" device-temperature="6" device-variant="" position="32" name="VREF+" type="monoio"/>
+        <pin device-name="62" device-size="e" device-temperature="6" device-variant="" position="32" name="VREF+" type="power"/>
         <pin device-name="52" device-size="c|e" device-temperature="6" device-variant="q" position="33" name="PA0"/>
         <pin device-name="52" device-size="e" device-temperature="3|6|7" device-variant="|q" position="33" name="PA0"/>
         <pin device-name="62" device-size="e" device-temperature="6" device-variant="q" position="33" name="PA0"/>
         <pin device-name="62" device-size="e" device-temperature="6" device-variant="" position="33" name="VDDA" type="power"/>
         <pin device-name="52" device-size="c|e" device-temperature="6" device-variant="q" position="34" name="PA1"/>
         <pin device-name="52" device-size="e" device-temperature="3|6|7" device-variant="|q" position="34" name="PA1"/>
         <pin device-name="62" device-size="e" device-temperature="6" device-variant="q" position="34" name="PA1"/>
@@ -2670,15 +2664,15 @@
         <pin position="H2" name="PC0"/>
         <pin position="H3" name="OPAMP1_VINM" type="monoio"/>
         <pin position="H4" name="VSS" type="power"/>
         <pin position="H9" name="VSS" type="power"/>
         <pin position="H10" name="PD14"/>
         <pin position="H11" name="PD13"/>
         <pin position="H12" name="PD15"/>
-        <pin position="J1" name="VREF+" type="monoio"/>
+        <pin position="J1" name="VREF+" type="power"/>
         <pin position="J2" name="PA0"/>
         <pin position="J3" name="PC5"/>
         <pin position="J4" name="VDD" type="power"/>
         <pin position="J5" name="PF14"/>
         <pin position="J6" name="PE8"/>
         <pin position="J7" name="PE10"/>
         <pin position="J8" name="PE12"/>
@@ -2854,15 +2848,15 @@
         <pin position="G1" name="PB14"/>
         <pin position="G2" name="PB12"/>
         <pin position="G3" name="PC9"/>
         <pin position="G4" name="PC4"/>
         <pin position="G5" name="PA6"/>
         <pin position="G6" name="PA2"/>
         <pin position="G7" name="PC3"/>
-        <pin position="G8" name="VREF+" type="monoio"/>
+        <pin position="G8" name="VREF+" type="power"/>
         <pin position="G9" name="VSSA/VREF-" type="power"/>
         <pin position="H1" name="VDD" type="power"/>
         <pin position="H2" name="VSS" type="power"/>
         <pin device-name="52|62" device-variant="q" position="H3" name="VLXSMPS" type="power"/>
         <pin device-name="52|62" device-variant="p" position="H3" name="PE15"/>
         <pin device-name="52|62" device-variant="q" position="H4" name="PB11"/>
         <pin device-name="52|62" device-variant="p" position="H4" name="PE14"/>
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32u5-75_85.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32u5-75_85.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wb-10_15_1m.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wb-10_15_1m.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wb-30_50.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wb-30_50.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wb-35_55_5m.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wb-35_55_5m.xml`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wl-54_55.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wl-54_55.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wl-54_55.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wl-54_55.xml`

```diff
@@ -55,15 +55,15 @@
       <vector position="27" name="USART1"/>
       <vector position="28" name="USART2"/>
       <vector position="29" name="LPUART1"/>
       <vector position="30" name="SUBGHZSPI"/>
       <vector position="31" name="SUBGHZ_Radio"/>
     </driver>
     <driver name="adc" type="stm32"/>
-    <driver name="adv_trace" type="stm32-v1.0"/>
+    <driver name="adv_trace" type="stm32-v1.1"/>
     <driver name="aes" type="stm32-v1.0"/>
     <driver name="comp" type="stm32-tsmc90_wlxx_cube">
       <instance value="1"/>
       <instance value="2"/>
     </driver>
     <driver name="crc" type="stm32"/>
     <driver name="dac" type="stm32">
@@ -95,15 +95,15 @@
     <driver name="i2s" type="stm32-v3.5">
       <instance value="2"/>
     </driver>
     <driver name="ipcc" type="stm32-v1.0"/>
     <driver name="irtim" type="stm32-v1.0"/>
     <driver name="iwdg" type="stm32"/>
     <driver name="kms" type="stm32-v1.1"/>
-    <driver device-name="55" name="lorawan" type="stm32-v2.4"/>
+    <driver device-name="55" name="lorawan" type="stm32-v2.5"/>
     <driver name="lptim" type="stm32-v2.1">
       <instance value="1"/>
       <instance value="2"/>
       <instance value="3"/>
     </driver>
     <driver name="lpuart" type="stm32-v1.3">
       <instance value="1"/>
@@ -113,43 +113,43 @@
     <driver name="pwr" type="stm32-v1.0"/>
     <driver name="rcc" type="stm32-v1.0">
       <max-frequency device-core="m0" value="48000000"/>
       <max-frequency device-core="m4" value="24000000"/>
     </driver>
     <driver name="rng" type="stm32"/>
     <driver name="rtc" type="stm32-v3.0"/>
-    <driver name="sequencer" type="stm32-v1.0">
+    <driver name="sequencer" type="stm32-v1.1">
       <instance value="cortex-m0plus"/>
       <instance value="cortex-m4"/>
     </driver>
-    <driver name="sigfox" type="stm32-v1.7"/>
+    <driver name="sigfox" type="stm32-v1.8"/>
     <driver name="spi" type="stm32">
       <instance value="1"/>
       <instance value="2"/>
     </driver>
     <driver name="subghz" type="stm32-v1.0"/>
-    <driver name="subghz_phy" type="stm32-v1.2"/>
+    <driver name="subghz_phy" type="stm32-v1.3"/>
     <driver name="sys" type="stm32">
       <feature value="exti"/>
     </driver>
     <driver name="sysm0p" type="stm32-v1.0">
       <instance value="plus"/>
     </driver>
     <driver name="tim" type="stm32-advanced">
       <instance value="1"/>
     </driver>
     <driver name="tim" type="stm32-general-purpose">
       <instance value="2"/>
       <instance value="16"/>
       <instance value="17"/>
     </driver>
-    <driver name="tim" type="stm32-v1.0">
+    <driver name="tim" type="stm32-v1.1">
       <instance value="er"/>
     </driver>
-    <driver name="tiny_lpm" type="stm32-v1.0"/>
+    <driver name="tiny_lpm" type="stm32-v1.1"/>
     <driver name="usart" type="stm32">
       <instance value="1"/>
       <instance value="2"/>
     </driver>
     <driver name="vrefbuf" type="stm32-v1.0"/>
     <driver name="wwdg" type="stm32-v2.0"/>
     <driver name="dma" type="stm32-mux">
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wl-e4_e5.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wl-e4_e5.xml`

 * *Files 0% similar despite different names*

#### Comparing `modm-devices-0.9.3/modm_devices/resources/devices/stm32/stm32wl-e4_e5.xml` & `modm-devices-0.9.4/modm_devices/resources/devices/stm32/stm32wl-e4_e5.xml`

```diff
@@ -86,15 +86,15 @@
       <vector position="57" name="DMA2_Channel4"/>
       <vector position="58" name="DMA2_Channel5"/>
       <vector position="59" name="DMA2_Channel6"/>
       <vector position="60" name="DMA2_Channel7"/>
       <vector position="61" name="DMAMUX1_OVR"/>
     </driver>
     <driver name="adc" type="stm32"/>
-    <driver name="adv_trace" type="stm32-v1.0"/>
+    <driver name="adv_trace" type="stm32-v1.1"/>
     <driver name="aes" type="stm32-v1.0"/>
     <driver name="comp" type="stm32-tsmc90_wlxx_cube">
       <instance value="1"/>
       <instance value="2"/>
     </driver>
     <driver name="crc" type="stm32"/>
     <driver name="dac" type="stm32">
@@ -121,15 +121,15 @@
     </driver>
     <driver name="i2s" type="stm32-v3.5">
       <instance value="2"/>
     </driver>
     <driver name="irtim" type="stm32-v1.0"/>
     <driver name="iwdg" type="stm32"/>
     <driver name="kms" type="stm32-v1.1"/>
-    <driver device-name="e5" name="lorawan" type="stm32-v2.4"/>
+    <driver device-name="e5" name="lorawan" type="stm32-v2.5"/>
     <driver name="lptim" type="stm32-v2.1">
       <instance value="1"/>
       <instance value="2"/>
       <instance value="3"/>
     </driver>
     <driver name="lpuart" type="stm32-v1.3">
       <instance value="1"/>
@@ -138,37 +138,37 @@
     <driver name="pka" type="stm32-v1.0"/>
     <driver name="pwr" type="stm32-v1.0"/>
     <driver name="rcc" type="stm32-v1.0">
       <max-frequency value="48000000"/>
     </driver>
     <driver name="rng" type="stm32"/>
     <driver name="rtc" type="stm32-v3.0"/>
-    <driver name="sequencer" type="stm32-v1.0"/>
-    <driver name="sigfox" type="stm32-v1.7"/>
+    <driver name="sequencer" type="stm32-v1.1"/>
+    <driver name="sigfox" type="stm32-v1.8"/>
     <driver name="spi" type="stm32">
       <instance value="1"/>
       <instance value="2"/>
     </driver>
     <driver name="subghz" type="stm32-v1.0"/>
-    <driver name="subghz_phy" type="stm32-v1.2"/>
+    <driver name="subghz_phy" type="stm32-v1.3"/>
     <driver name="sys" type="stm32">
       <feature value="exti"/>
     </driver>
     <driver name="tim" type="stm32-advanced">
       <instance value="1"/>
     </driver>
     <driver name="tim" type="stm32-general-purpose">
       <instance value="2"/>
       <instance value="16"/>
       <instance value="17"/>
     </driver>
-    <driver name="tim" type="stm32-v1.0">
+    <driver name="tim" type="stm32-v1.1">
       <instance value="er"/>
     </driver>
-    <driver name="tiny_lpm" type="stm32-v1.0"/>
+    <driver name="tiny_lpm" type="stm32-v1.1"/>
     <driver name="usart" type="stm32">
       <instance value="1"/>
       <instance value="2"/>
     </driver>
     <driver name="vrefbuf" type="stm32-v1.0"/>
     <driver name="wwdg" type="stm32-v2.0"/>
     <driver name="dma" type="stm32-mux">
```

### Comparing `modm-devices-0.9.3/modm_devices/resources/schema/device.xsd` & `modm-devices-0.9.4/modm_devices/resources/schema/device.xsd`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/schema/xinclude.xsd` & `modm-devices-0.9.4/modm_devices/resources/schema/xinclude.xsd`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices/resources/schema/xml.xsd` & `modm-devices-0.9.4/modm_devices/resources/schema/xml.xsd`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/modm_devices.egg-info/PKG-INFO` & `modm-devices-0.9.4/modm_devices.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modm-devices
-Version: 0.9.3
+Version: 0.9.4
 Summary: Curated data for AVR and ARM Cortex-M devices
 Home-page: https://github.com/modm-io/modm-devices
 Author: Niklas Hauser
 Author-email: niklas@salkinium.com
 License: MPL-2.0
 Keywords: modm lbuild modm-devices stm32 avr sam nrf
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `modm-devices-0.9.3/modm_devices.egg-info/SOURCES.txt` & `modm-devices-0.9.4/modm_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modm-devices-0.9.3/setup.py` & `modm-devices-0.9.4/setup.py`

 * *Files identical despite different names*

