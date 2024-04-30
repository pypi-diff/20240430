# Comparing `tmp/gestionatr-3.8.0.tar.gz` & `tmp/gestionatr-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gestionatr-3.8.0.tar", last modified: Mon Dec  4 08:45:12 2023, max compression
+gzip compressed data, was "gestionatr-3.8.1.tar", last modified: Tue Apr 30 07:34:54 2024, max compression
```

## Comparing `gestionatr-3.8.0.tar` & `gestionatr-3.8.1.tar`

### file list

```diff
@@ -1,301 +1,301 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 08:45:12.481394 gestionatr-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-12-04 08:45:10.000000 gestionatr-3.8.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-04 08:45:10.000000 gestionatr-3.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-12-04 08:45:12.481394 gestionatr-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-04 08:45:10.000000 gestionatr-3.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 08:45:12.437394 gestionatr-3.8.0/gestionatr/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12078 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 08:45:12.465394 gestionatr-3.8.0/gestionatr/data/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A101.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A102.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A102e.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A103.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A104.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A105.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A1224.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    13772 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A1226.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A1350.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A138.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A141.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A142.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A143.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A144.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A1450.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A146.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A148.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A149.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A1550.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A15S50.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    10137 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A1945.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A20.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A202.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A203.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A204.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A205.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A21.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A219.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A238.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A241.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A242.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A243.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A244.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A246.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A248.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A249.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2504.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2505.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2538.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2541.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2542.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2543.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2544.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2548.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2549.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2604.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2605.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2638.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2641.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2642.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2643.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2644.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2648.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2649.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2S02.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2S03.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2S41.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2S42.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A2S49.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A302.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A304.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     9415 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A305.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    11459 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A338.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    13726 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A341.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A342.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A343.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A344.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A348.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A349.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A3S02.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A3S41.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A3S42.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A3S49.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A402.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A404.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A405.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A438.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A441.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A442.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A443.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A444.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A449.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A4S02.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A4S41.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A4S42.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A4S49.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A529.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    10626 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A6161.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    17413 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A629.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A708.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A8009.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A8109.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A8409.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A8509.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/A8609.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionAlta.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionAnulacion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionAnulacionBaja.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionAnulacionReclamacion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      784 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionAportacionLectura.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionBajaSuspension.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionCambiodeComercializadorConCambios.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionCambiodeComercializadorSaliente.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionCambiodeComercializadorSinCambios.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionD1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionDesistimiento.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionModificacionDeATR.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionNotificacionCambiosATRDesdeDistribuidor.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionReclamacion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AceptacionTraspasoCOR.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ActivacionAlta.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ActivacionBaja.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ActivacionBajaSuspension.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ActivacionCambiodeComercializadorConCambios.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ActivacionCambiodeComercializadorSinCambios.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ActivacionComercializadorSaliente.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ActivacionDesistimiento.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ActivacionModificacionDeATR.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ActivacionTraspasoCOR.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      745 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ActivacionTraspasoCORSaliente.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/Alta.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AnulacionSolicitud.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/AnulacionSolicitudReclamacion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/B7031.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/B7032.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/B7033.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      676 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/BajaSuspension.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/CambiodeComercializadorConCambios.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/CambiodeComercializadorSinCambios.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/CierreReclamacion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    70346 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/CommonTagsATCOM.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    80962 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/CommonTagsCONT.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    37855 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/CommonTagsFACT.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     7878 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/CommonTagsPETS.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ContestacionIncidencia.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/EnvioInformacionPS.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/EnvioInformacionReclamacion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    34602 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/Facturacion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/IncidenciasATRDistribuidor.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      690 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ModificacionDeATR.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      746 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/NotificacionActivacionPorDesistimiento.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/NotificacionCambiosATRDesdeDistribuidor.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/PeticionInformacionAdicionalReclamacion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/Rechazo.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/RechazoCambiodeComercializadorSaliente.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/RechazoD1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/RechazoDesistimiento.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/RechazoPeticion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/RechazoReclamacion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      642 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/RechazoTraspasoCOR.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/ReclamacionPeticion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/SaldoLecturasFacturacion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/SolicitudAportacionLectura.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/SolicitudDesistimiento.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/SolicitudInformacionAlRegistroDePS.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      647 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/SolicitudTraspasoCOR.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeA101.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeA102.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeA301.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeA305.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeAceptacion.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeB101.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeB105.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeB201.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeC101.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeC105.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeC201.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeC205.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeE.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeM101.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeM105.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeP002.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeR101.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    14321 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeR105.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeRechazo.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeRechazoCCAA.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeSaliente.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeT101.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TipoMensajeT105.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    54319 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TiposComplejos.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    11518 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TiposComplejosCCAA.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   141142 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TiposSencillos.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    18240 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/TiposSencillosCCAA.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/WebserviceRPS.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/WebserviceSync.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/data/xml.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   103250 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   133588 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/defs_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 08:45:12.465394 gestionatr-3.8.0/gestionatr/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/helpers/funcions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 08:45:12.465394 gestionatr-3.8.0/gestionatr/input/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 08:45:12.473394 gestionatr-3.8.0/gestionatr/input/messages/
--rw-r--r--   0 runner    (1001) docker     (127)    10247 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A12_24.py
--rw-r--r--   0 runner    (1001) docker     (127)     8489 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A12_26.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A13_50.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A19_45.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_02.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_03.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_04.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_05.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_38.py
--rw-r--r--   0 runner    (1001) docker     (127)    26696 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_41.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_42.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_43.py
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_44.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_46.py
--rw-r--r--   0 runner    (1001) docker     (127)    27844 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_48.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A1_49.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A20_36.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A3.py
--rw-r--r--   0 runner    (1001) docker     (127)    19098 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/A5_29.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/B1.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/B2.py
--rw-r--r--   0 runner    (1001) docker     (127)    53323 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/B70.py
--rw-r--r--   0 runner    (1001) docker     (127)    24815 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/C1.py
--rw-r--r--   0 runner    (1001) docker     (127)    17800 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/C2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16155 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/D1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/Deadlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/E1.py
--rw-r--r--   0 runner    (1001) docker     (127)    93514 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/F1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/M1.py
--rw-r--r--   0 runner    (1001) docker     (127)    25263 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/P0.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/Q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    31504 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/R1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/T1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/W1.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19377 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/gestionatr_maker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16369 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9845 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/input/messages/message_gas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 08:45:12.473394 gestionatr-3.8.0/gestionatr/output/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 08:45:12.477394 gestionatr-3.8.0/gestionatr/output/messages/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/base_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_02.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_04.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_05.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_38.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_41.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_42.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_43.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_44.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_46.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_48.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a1_49.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a20_36.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a25_42.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_a5_29.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_b1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_b2.py
--rw-r--r--   0 runner    (1001) docker     (127)    22975 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_c1.py
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_c2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_d1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)    34989 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_f1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_m1.py
--rw-r--r--   0 runner    (1001) docker     (127)    15170 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_p0.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    25200 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_r1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_t1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/output/messages/sw_w1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/parser_xml_defs_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2023-12-04 08:45:10.000000 gestionatr-3.8.0/gestionatr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 08:45:12.437394 gestionatr-3.8.0/gestionatr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-12-04 08:45:12.000000 gestionatr-3.8.0/gestionatr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2023-12-04 08:45:12.000000 gestionatr-3.8.0/gestionatr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 08:45:12.000000 gestionatr-3.8.0/gestionatr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-04 08:45:12.000000 gestionatr-3.8.0/gestionatr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-04 08:45:12.000000 gestionatr-3.8.0/gestionatr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-04 08:45:12.000000 gestionatr-3.8.0/gestionatr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-04 08:45:10.000000 gestionatr-3.8.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-04 08:45:10.000000 gestionatr-3.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-04 08:45:12.481394 gestionatr-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-12-04 08:45:10.000000 gestionatr-3.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 08:45:12.481394 gestionatr-3.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-04 08:45:10.000000 gestionatr-3.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2023-12-04 08:45:10.000000 gestionatr-3.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-12-04 08:45:10.000000 gestionatr-3.8.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)   302647 2023-12-04 08:45:10.000000 gestionatr-3.8.0/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (127)   234857 2023-12-04 08:45:10.000000 gestionatr-3.8.0/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-12-04 08:45:10.000000 gestionatr-3.8.0/tests/test_table_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2023-12-04 08:45:10.000000 gestionatr-3.8.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:34:54.136051 gestionatr-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-30 07:34:53.000000 gestionatr-3.8.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 07:34:53.000000 gestionatr-3.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 07:34:54.136051 gestionatr-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-30 07:34:53.000000 gestionatr-3.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:34:54.092051 gestionatr-3.8.1/gestionatr/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12078 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:34:54.124051 gestionatr-3.8.1/gestionatr/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A101.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A102.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A102e.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A103.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A104.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A105.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A1224.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    13772 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A1226.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A1350.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A138.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A141.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A142.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A143.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A144.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A1450.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A146.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A148.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A149.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A1550.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A15S50.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A1945.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A20.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A202.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A203.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A204.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A205.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A21.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A219.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A238.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A241.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A242.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A243.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A244.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A246.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A248.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A249.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2504.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2505.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2538.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2541.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2542.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2543.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2544.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2548.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2549.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2604.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2605.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2638.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2641.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2642.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2643.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2644.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2648.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2649.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2S02.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2S03.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2S41.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2S42.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A2S49.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A302.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A304.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A305.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A338.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    13726 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A341.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A342.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A343.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A344.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A348.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A349.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A3S02.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A3S41.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A3S42.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A3S49.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A402.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A404.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A405.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A438.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A441.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A442.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A443.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A444.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A449.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A4S02.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A4S41.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A4S42.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A4S49.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A529.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A6161.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    17413 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A629.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A708.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A8009.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A8109.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A8409.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A8509.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/A8609.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionAlta.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionAnulacion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionAnulacionBaja.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionAnulacionReclamacion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionAportacionLectura.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionBajaSuspension.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionCambiodeComercializadorConCambios.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionCambiodeComercializadorSaliente.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionCambiodeComercializadorSinCambios.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionD1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionDesistimiento.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionModificacionDeATR.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionNotificacionCambiosATRDesdeDistribuidor.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionReclamacion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AceptacionTraspasoCOR.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ActivacionAlta.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ActivacionBaja.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ActivacionBajaSuspension.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ActivacionCambiodeComercializadorConCambios.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ActivacionCambiodeComercializadorSinCambios.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ActivacionComercializadorSaliente.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ActivacionDesistimiento.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ActivacionModificacionDeATR.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ActivacionTraspasoCOR.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ActivacionTraspasoCORSaliente.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/Alta.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AnulacionSolicitud.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/AnulacionSolicitudReclamacion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/B7031.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/B7032.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/B7033.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/BajaSuspension.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/CambiodeComercializadorConCambios.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/CambiodeComercializadorSinCambios.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/CierreReclamacion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    70346 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/CommonTagsATCOM.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    80962 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/CommonTagsCONT.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    37855 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/CommonTagsFACT.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     7878 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/CommonTagsPETS.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ContestacionIncidencia.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/EnvioInformacionPS.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/EnvioInformacionReclamacion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    34602 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/Facturacion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/IncidenciasATRDistribuidor.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ModificacionDeATR.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/NotificacionActivacionPorDesistimiento.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/NotificacionCambiosATRDesdeDistribuidor.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/PeticionInformacionAdicionalReclamacion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/Rechazo.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/RechazoCambiodeComercializadorSaliente.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/RechazoD1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/RechazoDesistimiento.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/RechazoPeticion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/RechazoReclamacion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/RechazoTraspasoCOR.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/ReclamacionPeticion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/SaldoLecturasFacturacion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/SolicitudAportacionLectura.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/SolicitudDesistimiento.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/SolicitudInformacionAlRegistroDePS.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/SolicitudTraspasoCOR.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeA101.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeA102.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeA301.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeA305.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeAceptacion.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeB101.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeB105.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeB201.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeC101.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeC105.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeC201.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeC205.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeE.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeM101.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeM105.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeP002.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeR101.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeR105.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeRechazo.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeRechazoCCAA.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeSaliente.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeT101.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TipoMensajeT105.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    54319 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TiposComplejos.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TiposComplejosCCAA.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   141355 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TiposSencillos.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    18240 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/TiposSencillosCCAA.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/WebserviceRPS.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/WebserviceSync.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/data/xml.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   103250 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133583 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/defs_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:34:54.124051 gestionatr-3.8.1/gestionatr/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/helpers/funcions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:34:54.124051 gestionatr-3.8.1/gestionatr/input/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:34:54.128051 gestionatr-3.8.1/gestionatr/input/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A12_24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A12_26.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A13_50.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A19_45.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_03.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_38.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26696 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_41.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_42.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_43.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_44.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_46.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27844 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_48.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A1_49.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A20_36.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19098 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/A5_29.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/B1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/B2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54521 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/B70.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24815 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/C1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17800 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/C2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/D1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/Deadlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/E1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93524 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/F1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/M1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25263 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/P0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/Q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31504 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/R1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/T1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/W1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19377 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/gestionatr_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/input/messages/message_gas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:34:54.128051 gestionatr-3.8.1/gestionatr/output/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:34:54.136051 gestionatr-3.8.1/gestionatr/output/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/base_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_41.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_42.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_43.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_44.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_46.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_48.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a1_49.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a20_36.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a25_42.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_a5_29.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_b1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_b2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22975 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_c1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_c2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_d1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34989 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_f1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_m1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15170 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_p0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25200 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_t1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/output/messages/sw_w1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/parser_xml_defs_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-30 07:34:53.000000 gestionatr-3.8.1/gestionatr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:34:54.096051 gestionatr-3.8.1/gestionatr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 07:34:54.000000 gestionatr-3.8.1/gestionatr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-04-30 07:34:54.000000 gestionatr-3.8.1/gestionatr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:34:54.000000 gestionatr-3.8.1/gestionatr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 07:34:54.000000 gestionatr-3.8.1/gestionatr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 07:34:54.000000 gestionatr-3.8.1/gestionatr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 07:34:54.000000 gestionatr-3.8.1/gestionatr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 07:34:53.000000 gestionatr-3.8.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 07:34:53.000000 gestionatr-3.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:34:54.136051 gestionatr-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-30 07:34:53.000000 gestionatr-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:34:54.136051 gestionatr-3.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 07:34:53.000000 gestionatr-3.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-30 07:34:53.000000 gestionatr-3.8.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-30 07:34:53.000000 gestionatr-3.8.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   302647 2024-04-30 07:34:53.000000 gestionatr-3.8.1/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)   234857 2024-04-30 07:34:53.000000 gestionatr-3.8.1/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-30 07:34:53.000000 gestionatr-3.8.1/tests/test_table_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-30 07:34:53.000000 gestionatr-3.8.1/tests/utils.py
```

### Comparing `gestionatr-3.8.0/COPYING` & `gestionatr-3.8.1/COPYING`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/cli.py` & `gestionatr-3.8.1/gestionatr/cli.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A101.xsd` & `gestionatr-3.8.1/gestionatr/data/A101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A102.xsd` & `gestionatr-3.8.1/gestionatr/data/A102.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A102e.xsd` & `gestionatr-3.8.1/gestionatr/data/A102e.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A103.xsd` & `gestionatr-3.8.1/gestionatr/data/A103.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A104.xsd` & `gestionatr-3.8.1/gestionatr/data/A104.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A105.xsd` & `gestionatr-3.8.1/gestionatr/data/A105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A1224.xsd` & `gestionatr-3.8.1/gestionatr/data/A1224.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A1226.xsd` & `gestionatr-3.8.1/gestionatr/data/A1226.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A1350.xsd` & `gestionatr-3.8.1/gestionatr/data/A1350.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A138.xsd` & `gestionatr-3.8.1/gestionatr/data/A138.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A141.xsd` & `gestionatr-3.8.1/gestionatr/data/A141.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A142.xsd` & `gestionatr-3.8.1/gestionatr/data/A142.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A143.xsd` & `gestionatr-3.8.1/gestionatr/data/A143.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A144.xsd` & `gestionatr-3.8.1/gestionatr/data/A144.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A1450.xsd` & `gestionatr-3.8.1/gestionatr/data/A1450.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A146.xsd` & `gestionatr-3.8.1/gestionatr/data/A146.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A148.xsd` & `gestionatr-3.8.1/gestionatr/data/A148.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A149.xsd` & `gestionatr-3.8.1/gestionatr/data/A149.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A1550.xsd` & `gestionatr-3.8.1/gestionatr/data/A1550.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A15S50.xsd` & `gestionatr-3.8.1/gestionatr/data/A15S50.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A1945.xsd` & `gestionatr-3.8.1/gestionatr/data/A1945.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A20.xsd` & `gestionatr-3.8.1/gestionatr/data/A20.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A202.xsd` & `gestionatr-3.8.1/gestionatr/data/A202.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A203.xsd` & `gestionatr-3.8.1/gestionatr/data/A203.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A204.xsd` & `gestionatr-3.8.1/gestionatr/data/A204.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A205.xsd` & `gestionatr-3.8.1/gestionatr/data/A205.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A21.xsd` & `gestionatr-3.8.1/gestionatr/data/A21.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A219.xsd` & `gestionatr-3.8.1/gestionatr/data/A219.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A238.xsd` & `gestionatr-3.8.1/gestionatr/data/A238.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A241.xsd` & `gestionatr-3.8.1/gestionatr/data/A241.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A242.xsd` & `gestionatr-3.8.1/gestionatr/data/A242.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A243.xsd` & `gestionatr-3.8.1/gestionatr/data/A243.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A244.xsd` & `gestionatr-3.8.1/gestionatr/data/A244.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A246.xsd` & `gestionatr-3.8.1/gestionatr/data/A246.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A248.xsd` & `gestionatr-3.8.1/gestionatr/data/A248.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A249.xsd` & `gestionatr-3.8.1/gestionatr/data/A249.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2504.xsd` & `gestionatr-3.8.1/gestionatr/data/A2504.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2505.xsd` & `gestionatr-3.8.1/gestionatr/data/A2505.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2538.xsd` & `gestionatr-3.8.1/gestionatr/data/A2538.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2541.xsd` & `gestionatr-3.8.1/gestionatr/data/A2541.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2542.xsd` & `gestionatr-3.8.1/gestionatr/data/A2542.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2543.xsd` & `gestionatr-3.8.1/gestionatr/data/A2543.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2544.xsd` & `gestionatr-3.8.1/gestionatr/data/A2544.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2548.xsd` & `gestionatr-3.8.1/gestionatr/data/A2548.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2549.xsd` & `gestionatr-3.8.1/gestionatr/data/A2549.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2604.xsd` & `gestionatr-3.8.1/gestionatr/data/A2604.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2605.xsd` & `gestionatr-3.8.1/gestionatr/data/A2605.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2638.xsd` & `gestionatr-3.8.1/gestionatr/data/A2638.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2641.xsd` & `gestionatr-3.8.1/gestionatr/data/A2641.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2642.xsd` & `gestionatr-3.8.1/gestionatr/data/A2642.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2643.xsd` & `gestionatr-3.8.1/gestionatr/data/A2643.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2644.xsd` & `gestionatr-3.8.1/gestionatr/data/A2644.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2648.xsd` & `gestionatr-3.8.1/gestionatr/data/A2648.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2649.xsd` & `gestionatr-3.8.1/gestionatr/data/A2649.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2S02.xsd` & `gestionatr-3.8.1/gestionatr/data/A2S02.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2S03.xsd` & `gestionatr-3.8.1/gestionatr/data/A2S03.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2S41.xsd` & `gestionatr-3.8.1/gestionatr/data/A2S41.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2S42.xsd` & `gestionatr-3.8.1/gestionatr/data/A2S42.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A2S49.xsd` & `gestionatr-3.8.1/gestionatr/data/A2S49.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A302.xsd` & `gestionatr-3.8.1/gestionatr/data/A302.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A304.xsd` & `gestionatr-3.8.1/gestionatr/data/A304.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A305.xsd` & `gestionatr-3.8.1/gestionatr/data/A305.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A338.xsd` & `gestionatr-3.8.1/gestionatr/data/A338.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A341.xsd` & `gestionatr-3.8.1/gestionatr/data/A341.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A342.xsd` & `gestionatr-3.8.1/gestionatr/data/A342.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A343.xsd` & `gestionatr-3.8.1/gestionatr/data/A343.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A344.xsd` & `gestionatr-3.8.1/gestionatr/data/A344.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A348.xsd` & `gestionatr-3.8.1/gestionatr/data/A348.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A349.xsd` & `gestionatr-3.8.1/gestionatr/data/A349.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A3S02.xsd` & `gestionatr-3.8.1/gestionatr/data/A3S02.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A3S41.xsd` & `gestionatr-3.8.1/gestionatr/data/A3S41.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A3S42.xsd` & `gestionatr-3.8.1/gestionatr/data/A3S42.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A3S49.xsd` & `gestionatr-3.8.1/gestionatr/data/A3S49.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A402.xsd` & `gestionatr-3.8.1/gestionatr/data/A402.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A404.xsd` & `gestionatr-3.8.1/gestionatr/data/A404.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A405.xsd` & `gestionatr-3.8.1/gestionatr/data/A405.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A438.xsd` & `gestionatr-3.8.1/gestionatr/data/A438.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A441.xsd` & `gestionatr-3.8.1/gestionatr/data/A441.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A442.xsd` & `gestionatr-3.8.1/gestionatr/data/A442.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A443.xsd` & `gestionatr-3.8.1/gestionatr/data/A443.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A444.xsd` & `gestionatr-3.8.1/gestionatr/data/A444.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A449.xsd` & `gestionatr-3.8.1/gestionatr/data/A449.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A4S02.xsd` & `gestionatr-3.8.1/gestionatr/data/A4S02.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A4S41.xsd` & `gestionatr-3.8.1/gestionatr/data/A4S41.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A4S42.xsd` & `gestionatr-3.8.1/gestionatr/data/A4S42.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A4S49.xsd` & `gestionatr-3.8.1/gestionatr/data/A4S49.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A529.xsd` & `gestionatr-3.8.1/gestionatr/data/A529.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A6161.xsd` & `gestionatr-3.8.1/gestionatr/data/A6161.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A629.xsd` & `gestionatr-3.8.1/gestionatr/data/A629.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A708.xsd` & `gestionatr-3.8.1/gestionatr/data/A708.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A8009.xsd` & `gestionatr-3.8.1/gestionatr/data/A8009.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A8109.xsd` & `gestionatr-3.8.1/gestionatr/data/A8109.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A8409.xsd` & `gestionatr-3.8.1/gestionatr/data/A8409.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A8509.xsd` & `gestionatr-3.8.1/gestionatr/data/A8509.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/A8609.xsd` & `gestionatr-3.8.1/gestionatr/data/A8609.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionAlta.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionAlta.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionAnulacion.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionAnulacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionAnulacionBaja.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionAnulacionBaja.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionAnulacionReclamacion.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionAnulacionReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionAportacionLectura.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionAportacionLectura.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionBajaSuspension.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionBajaSuspension.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionCambiodeComercializadorConCambios.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionCambiodeComercializadorConCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionCambiodeComercializadorSaliente.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionCambiodeComercializadorSaliente.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionCambiodeComercializadorSinCambios.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionCambiodeComercializadorSinCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionD1.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionD1.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionDesistimiento.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionDesistimiento.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionModificacionDeATR.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionModificacionDeATR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionNotificacionCambiosATRDesdeDistribuidor.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionNotificacionCambiosATRDesdeDistribuidor.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionReclamacion.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AceptacionTraspasoCOR.xsd` & `gestionatr-3.8.1/gestionatr/data/AceptacionTraspasoCOR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ActivacionAlta.xsd` & `gestionatr-3.8.1/gestionatr/data/ActivacionAlta.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ActivacionBaja.xsd` & `gestionatr-3.8.1/gestionatr/data/ActivacionBaja.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ActivacionBajaSuspension.xsd` & `gestionatr-3.8.1/gestionatr/data/ActivacionBajaSuspension.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ActivacionCambiodeComercializadorConCambios.xsd` & `gestionatr-3.8.1/gestionatr/data/ActivacionCambiodeComercializadorConCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ActivacionCambiodeComercializadorSinCambios.xsd` & `gestionatr-3.8.1/gestionatr/data/ActivacionCambiodeComercializadorSinCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ActivacionComercializadorSaliente.xsd` & `gestionatr-3.8.1/gestionatr/data/ActivacionComercializadorSaliente.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ActivacionDesistimiento.xsd` & `gestionatr-3.8.1/gestionatr/data/ActivacionDesistimiento.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ActivacionModificacionDeATR.xsd` & `gestionatr-3.8.1/gestionatr/data/ActivacionModificacionDeATR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ActivacionTraspasoCOR.xsd` & `gestionatr-3.8.1/gestionatr/data/ActivacionTraspasoCOR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ActivacionTraspasoCORSaliente.xsd` & `gestionatr-3.8.1/gestionatr/data/ActivacionTraspasoCORSaliente.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/Alta.xsd` & `gestionatr-3.8.1/gestionatr/data/Alta.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AnulacionSolicitud.xsd` & `gestionatr-3.8.1/gestionatr/data/AnulacionSolicitud.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/AnulacionSolicitudReclamacion.xsd` & `gestionatr-3.8.1/gestionatr/data/AnulacionSolicitudReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/B7031.xsd` & `gestionatr-3.8.1/gestionatr/data/B7031.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/B7032.xsd` & `gestionatr-3.8.1/gestionatr/data/B7032.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/B7033.xsd` & `gestionatr-3.8.1/gestionatr/data/B7033.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/BajaSuspension.xsd` & `gestionatr-3.8.1/gestionatr/data/BajaSuspension.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/CambiodeComercializadorConCambios.xsd` & `gestionatr-3.8.1/gestionatr/data/CambiodeComercializadorConCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/CambiodeComercializadorSinCambios.xsd` & `gestionatr-3.8.1/gestionatr/data/CambiodeComercializadorSinCambios.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/CierreReclamacion.xsd` & `gestionatr-3.8.1/gestionatr/data/CierreReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/CommonTagsATCOM.xsd` & `gestionatr-3.8.1/gestionatr/data/CommonTagsATCOM.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/CommonTagsCONT.xsd` & `gestionatr-3.8.1/gestionatr/data/CommonTagsCONT.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/CommonTagsFACT.xsd` & `gestionatr-3.8.1/gestionatr/data/CommonTagsFACT.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/CommonTagsPETS.xsd` & `gestionatr-3.8.1/gestionatr/data/CommonTagsPETS.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ContestacionIncidencia.xsd` & `gestionatr-3.8.1/gestionatr/data/ContestacionIncidencia.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/EnvioInformacionPS.xsd` & `gestionatr-3.8.1/gestionatr/data/EnvioInformacionPS.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/EnvioInformacionReclamacion.xsd` & `gestionatr-3.8.1/gestionatr/data/EnvioInformacionReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/Facturacion.xsd` & `gestionatr-3.8.1/gestionatr/data/Facturacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/IncidenciasATRDistribuidor.xsd` & `gestionatr-3.8.1/gestionatr/data/IncidenciasATRDistribuidor.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ModificacionDeATR.xsd` & `gestionatr-3.8.1/gestionatr/data/ModificacionDeATR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/NotificacionActivacionPorDesistimiento.xsd` & `gestionatr-3.8.1/gestionatr/data/NotificacionActivacionPorDesistimiento.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/NotificacionCambiosATRDesdeDistribuidor.xsd` & `gestionatr-3.8.1/gestionatr/data/NotificacionCambiosATRDesdeDistribuidor.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/PeticionInformacionAdicionalReclamacion.xsd` & `gestionatr-3.8.1/gestionatr/data/PeticionInformacionAdicionalReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/Rechazo.xsd` & `gestionatr-3.8.1/gestionatr/data/Rechazo.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/RechazoCambiodeComercializadorSaliente.xsd` & `gestionatr-3.8.1/gestionatr/data/RechazoCambiodeComercializadorSaliente.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/RechazoD1.xsd` & `gestionatr-3.8.1/gestionatr/data/RechazoD1.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/RechazoDesistimiento.xsd` & `gestionatr-3.8.1/gestionatr/data/RechazoDesistimiento.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/RechazoPeticion.xsd` & `gestionatr-3.8.1/gestionatr/data/RechazoPeticion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/RechazoReclamacion.xsd` & `gestionatr-3.8.1/gestionatr/data/RechazoReclamacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/RechazoTraspasoCOR.xsd` & `gestionatr-3.8.1/gestionatr/data/RechazoTraspasoCOR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/ReclamacionPeticion.xsd` & `gestionatr-3.8.1/gestionatr/data/ReclamacionPeticion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/SaldoLecturasFacturacion.xsd` & `gestionatr-3.8.1/gestionatr/data/SaldoLecturasFacturacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/SolicitudAportacionLectura.xsd` & `gestionatr-3.8.1/gestionatr/data/SolicitudAportacionLectura.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/SolicitudDesistimiento.xsd` & `gestionatr-3.8.1/gestionatr/data/SolicitudDesistimiento.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/SolicitudInformacionAlRegistroDePS.xsd` & `gestionatr-3.8.1/gestionatr/data/SolicitudInformacionAlRegistroDePS.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/SolicitudTraspasoCOR.xsd` & `gestionatr-3.8.1/gestionatr/data/SolicitudTraspasoCOR.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeA101.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeA101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeA102.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeA102.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeA301.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeA301.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeA305.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeA305.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeAceptacion.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeAceptacion.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeB101.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeB101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeB105.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeB105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeB201.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeB201.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeC101.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeC101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeC105.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeC105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeC201.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeC201.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeC205.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeC205.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeE.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeE.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeM101.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeM101.xsd`

 * *Files 2% similar despite different names*

#### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeM101.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeM101.xsd`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <xs:schema xmlns="http://localhost/elegibilidad" xmlns:xs="http://www.w3.org/2001/XMLSchema" targetNamespace="http://localhost/elegibilidad" elementFormDefault="qualified" attributeFormDefault="unqualified">
   <xs:include schemaLocation="TiposComplejos.xsd"/>
   <xs:include schemaLocation="TiposSencillos.xsd"/>
   <xs:complexType name="ModificacionDeATRM101">
     <xs:sequence>
       <xs:element name="DatosSolicitud" type="DatosModificacionDeATRM101"/>
-      <xs:element name="Contrato" type="ContratoConModificacion"/>
+      <xs:element name="Contrato" type="ContratoConModificacion" minOccurs="0"/>
       <xs:element name="Cliente" type="ClienteConDireccion"/>
       <xs:element name="Medida" type="MedidaResto" minOccurs="0"/>
       <xs:element name="DocTecnica" type="DocTecnica" minOccurs="0"/>
       <xs:element name="Comentarios" type="X4000" minOccurs="0"/>
       <xs:element name="RegistrosDocumento" type="RegistrosDocs" minOccurs="0"/>
     </xs:sequence>
   </xs:complexType>
```

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeM105.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeM105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeP002.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeP002.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeR101.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeR101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeR105.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeR105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeRechazo.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeRechazo.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeRechazoCCAA.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeRechazoCCAA.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeSaliente.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeSaliente.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeT101.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeT101.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TipoMensajeT105.xsd` & `gestionatr-3.8.1/gestionatr/data/TipoMensajeT105.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TiposComplejos.xsd` & `gestionatr-3.8.1/gestionatr/data/TiposComplejos.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TiposComplejosCCAA.xsd` & `gestionatr-3.8.1/gestionatr/data/TiposComplejosCCAA.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/TiposSencillos.xsd` & `gestionatr-3.8.1/gestionatr/data/TiposSencillos.xsd`

 * *Files 0% similar despite different names*

```diff
@@ -423,14 +423,16 @@
 			<xs:enumeration value="E7"/>
 			<xs:enumeration value="E8"/>
 			<xs:enumeration value="E9"/>
 			<xs:enumeration value="F1"/>
 			<xs:enumeration value="G1"/>
 			<xs:enumeration value="G2"/>
 			<xs:enumeration value="G3"/>
+			<xs:enumeration value="G4"/>
+			<xs:enumeration value="G5"/>
 			<xs:enumeration value="G6"/>
 			<xs:enumeration value="H4"/>
 			<xs:enumeration value="H5"/>
 			<xs:enumeration value="H6"/>
 		</xs:restriction>
 	</xs:simpleType>
 	<xs:simpleType name="CodigoMotivoRechazoP0">
@@ -3195,20 +3197,24 @@
 	</xs:simpleType>
 	<xs:simpleType name="TipoModificacion">
 		<xs:annotation>
 			<xs:documentation>Tipo de modificacion contractual (tabla 7)	
 				S	Solicitud de modificacion contractual administrativa
 				N	Solicitud de modificacion contractual tecnica
 				A	Solicitud de modificacion tanto administrativa como tecnica
+				M Solicitud de aplicacion SMV
+				B 	Baja de SMV, vuelta a suministro normal
 			</xs:documentation>
 		</xs:annotation>
 		<xs:restriction base="xs:string">
 			<xs:enumeration value="S"/>
 			<xs:enumeration value="N"/>
 			<xs:enumeration value="A"/>
+			<xs:enumeration value="M"/>
+			<xs:enumeration value="B"/>
 		</xs:restriction>
 	</xs:simpleType>
 	<xs:simpleType name="TipoMoneda">
 		<xs:annotation>
 			<xs:documentation> Tipo de moneda (tabla 104)
 			02	Euros
 			</xs:documentation>
```

### Comparing `gestionatr-3.8.0/gestionatr/data/TiposSencillosCCAA.xsd` & `gestionatr-3.8.1/gestionatr/data/TiposSencillosCCAA.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/WebserviceRPS.xsd` & `gestionatr-3.8.1/gestionatr/data/WebserviceRPS.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/WebserviceSync.xsd` & `gestionatr-3.8.1/gestionatr/data/WebserviceSync.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/data/xml.xsd` & `gestionatr-3.8.1/gestionatr/data/xml.xsd`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/defs.py` & `gestionatr-3.8.1/gestionatr/defs.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/defs_gas.py` & `gestionatr-3.8.1/gestionatr/defs_gas.py`

 * *Files 0% similar despite different names*

```diff
@@ -2821,15 +2821,15 @@
     ('03', 'Respuesta a Solicitud de información necesaria para retipificar'),
 ]
 TAULA_PRIORIDAD = [
     ('0', 'Prioridad normal.'),
     ('1', 'Prioridad alta. '),
 ]
 
-REFUND_RECTIFICATIVE_TYPES = ['A', 'B']  # 'R' ?
+REFUND_RECTIFICATIVE_TYPES = ['A']  # 'R' ?
 
 REQUIRE_REFERENCE_TYPES = [
     'A', 'B', 'R'
 ]
 
 SIGN = {'N': 1, 'R': 1, 'A': -1, 'B': -1}
```

### Comparing `gestionatr-3.8.0/gestionatr/helpers/funcions.py` & `gestionatr-3.8.1/gestionatr/helpers/funcions.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A12_24.py` & `gestionatr-3.8.1/gestionatr/input/messages/A12_24.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A12_26.py` & `gestionatr-3.8.1/gestionatr/input/messages/A12_26.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A19_45.py` & `gestionatr-3.8.1/gestionatr/input/messages/A19_45.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1_02.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1_02.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1_04.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1_04.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1_05.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1_05.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1_38.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1_38.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1_41.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1_41.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1_42.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1_42.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1_43.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1_43.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1_44.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1_44.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1_46.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1_46.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1_48.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1_48.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A1_49.py` & `gestionatr-3.8.1/gestionatr/input/messages/A1_49.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A20_36.py` & `gestionatr-3.8.1/gestionatr/input/messages/A20_36.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/A5_29.py` & `gestionatr-3.8.1/gestionatr/input/messages/A5_29.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/B1.py` & `gestionatr-3.8.1/gestionatr/input/messages/B1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/B2.py` & `gestionatr-3.8.1/gestionatr/input/messages/B2.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/B70.py` & `gestionatr-3.8.1/gestionatr/input/messages/B70.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, unicode_literals
 from .message_gas import MessageGas
 from gestionatr.utils import get_rec_attr
-from gestionatr.defs_gas import TIPUS_CONCEPTES, PEAJES_SEMPRE_CAPACIDAD
+from gestionatr.defs_gas import TIPUS_CONCEPTES, PEAJES_SEMPRE_CAPACIDAD, REFUND_RECTIFICATIVE_TYPES
 from datetime import datetime, timedelta
 
 
 class B7031(MessageGas):
 
     @property
     def datosempresaemisora(self):
@@ -635,15 +635,15 @@
                 has_only_conceptes = False
         return has_only_conceptes
 
     def get_create_invoice_params(self):
         return {
             'tipo_rectificadora': self.clasefact or self.indfacturarect or 'N',
             'date_invoice': self.fecfactura,
-            'check_total': -1 * self.importetotal if self.clasefact in ('A', 'B') else self.importetotal,
+            'check_total': -1 * self.importetotal if self.clasefact in REFUND_RECTIFICATIVE_TYPES else self.importetotal,
             'origin': self.get_origin(),
             'origin_date_invoice': self.fecfactura,
             'reference': self.get_origin(),
             'tipo_factura': self.tipofactura
         }
 
     def get_linies_factura_by_type(self):
@@ -1308,14 +1308,15 @@
                 data.append(Numerador(d))
         return data
 
     def get_lectures_info(self):
         res = []
         if not hasattr(self, 'meters'):
             self.meters = [self]
+        factor_ultima_lectura = False
         for meter in self.meters:
             fecha_desde = meter.feclecant
             fecha_actual = meter.feclecact
             if fecha_desde == fecha_actual and meter.horalecact in ("23:00:00", "24:00:00"):
                 # A vegades envien una lectura a les 00 i l'altre a les 23 i son del mateix dia.
                 # Es equivalent a enviar una a les 23 del dia anterior i l'altre a les 23 del dia actual. per tant,
                 # restem un dia a la lectura desde
@@ -1331,15 +1332,15 @@
             qdmaximo = float(meter.qdmaximo)
             fecqdmax = meter.fecqdmax
             dqmedio = float(meter.dqmedio)
             qdcontratado = float(meter.qdcontratado)
             excesocaudal = float(meter.excesocaudal)
             temperatura_gas = float(meter.temp)
             pressio_atmosferica = float(meter.presatm)
-
+            consum_kwh_facturat = float(meter.consumokwh)
             for numerador in meter.listanumeradores:
                 lectura_desde_m3 = float(numerador.lectant)
                 lectura_actual_m3 = float(numerador.lecact)
                 origen_desde = numerador.tipolec
                 origen_actual = numerador.tipolec
                 tipo_lect_num = numerador.tipolecnum
                 lectura_desde = lectura_desde_m3 * float(meter.factorconver)
@@ -1369,26 +1370,40 @@
                     'fecqdmax': fecqdmax,
                     'dqmedio': float(dqmedio),
                     'qdcontratado': float(qdcontratado),
                     'excesocaudal': float(excesocaudal),
                     'temperatura_gas': float(temperatura_gas),
                     'pressio_atmosferica': float(pressio_atmosferica),
                 }
-                # Si el consum que calculem amb el factor_k i el pcs no dona el consum informat en el tag consumokwh
+
+                # Si el consum que calculem amb el factor_k i el pcs no dona el consum calculat amb el factor de conversio
                 # pero si fem servir el factor de conversio informat per la distri si que dona, modfiquem el factor_k perque
                 # el factor de conversio calculat sigui igual al informat i aixi el consum també quadri.
                 # TODO
                 # Revisant un cas concret, sembla que realment ens falta aplicar la zeta, per aixo no quadra.
                 # Normalment es 1 pero pot no ser-ho. Aixó es una mandanga per no ahver de treballar amb la zeta.
-                consum_calculat = round(vals['consum_m3'] * vals['pcs'] * vals['factor_k'], 3)
-                consum_facturat = round(vals['consum'], 3)
-                if consum_facturat != consum_calculat:
+                consum_calculat_sefons_fomrula = round(vals['consum_m3'] * vals['pcs'] * vals['factor_k'], 3)
+                consum_calculat_segons_factor = round(vals['consum'], 3)
+                if consum_calculat_segons_factor != consum_calculat_sefons_fomrula:
                     consum_calculat = round(vals['consum_m3'] * meter.factorconver, 3)
-                    if consum_facturat == consum_calculat:
+                    if consum_calculat_segons_factor == consum_calculat:
                         vals['factor_k'] = meter.factorconver / vals['pcs']
+
+                # Unaltre cas concret de ***
+                # Hi ha distris que tot i tindre lectures diaries no apliquen el factor de conversio registart en
+                # cada dia, sino que paliquen a totes les lectures de tots els dies el factor de conversio de la
+                # ultima lectura
+                # Per tant: si el consum facturat per la distri no coincideix amb el consum calculat, ero aplicant
+                # el faactor de conversio del ultim dia siq ue aplica, recalculem el factor k perque quadri tot.
+                if consum_kwh_facturat != consum_calculat_segons_factor:
+                    if not factor_ultima_lectura and self.meters[-1].factorconver:
+                        factor_ultima_lectura = float(self.meters[-1].factorconver)
+                    if factor_ultima_lectura:
+                        vals['factor_k'] = consum_kwh_facturat / (vals['consum_m3'] * vals['pcs'])
+                        vals['consum'] = consum_kwh_facturat
                 res.append(vals)
         return res
 
     def get_giro(self):
         return max([10**int(l.digmed) for l in self.listanumeradores])
```

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/C1.py` & `gestionatr-3.8.1/gestionatr/input/messages/C1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/C2.py` & `gestionatr-3.8.1/gestionatr/input/messages/C2.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/D1.py` & `gestionatr-3.8.1/gestionatr/input/messages/D1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/Deadlines.py` & `gestionatr-3.8.1/gestionatr/input/messages/Deadlines.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/E1.py` & `gestionatr-3.8.1/gestionatr/input/messages/E1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/F1.py` & `gestionatr-3.8.1/gestionatr/input/messages/F1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1633,15 +1633,15 @@
         if (not tipus or "S" in tipus) and self.factura and self.factura.get_consum_facturat(tipus='S', periode=None) \
                 and not self.factura.has_AS_lectures():
             # Si no tenim lectures AS pero si que ens han cobrat excedents,
             # creem unes lectures AS ficticies a 0 (puta ENDESA)
             lectures.extend(self.factura.get_fake_AS_lectures())
         if (not tipus or "S" in tipus) and self.factura and self.factura.has_AS_lectures_only_p0() \
                 and len(self.factura.get_consum_facturat(tipus='S', periode=None)) > 1 \
-                and self.factura.datos_factura.tarifa_atr_fact not in ['001', '005']:
+                and self.factura.datos_factura.tarifa_atr_fact in ['004', '006', '007', '008']:
             # Si nomes ens envien el P0 de excedents pero ens cobren varis periodes
             # creem una lectura e P2 AS ficticies a 0 (puta FENOSA)
             lectures.extend(self.factura.get_fake_AS_p2_lectures())
 
         if not force_no_transforma_no_td_a_td and self.factura:
             lectures = self.factura.transforma_no_td_a_td(lectures, tipus=tipus)
         lectures = sorted(lectures, key=lambda x: x.lectura_desde.fecha)
```

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/M1.py` & `gestionatr-3.8.1/gestionatr/input/messages/M1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/P0.py` & `gestionatr-3.8.1/gestionatr/input/messages/P0.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/Q1.py` & `gestionatr-3.8.1/gestionatr/input/messages/Q1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/R1.py` & `gestionatr-3.8.1/gestionatr/input/messages/R1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/T1.py` & `gestionatr-3.8.1/gestionatr/input/messages/T1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/W1.py` & `gestionatr-3.8.1/gestionatr/input/messages/W1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/__init__.py` & `gestionatr-3.8.1/gestionatr/input/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/defs.py` & `gestionatr-3.8.1/gestionatr/input/messages/defs.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/gestionatr_maker.py` & `gestionatr-3.8.1/gestionatr/input/messages/gestionatr_maker.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/message.py` & `gestionatr-3.8.1/gestionatr/input/messages/message.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/input/messages/message_gas.py` & `gestionatr-3.8.1/gestionatr/input/messages/message_gas.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/base.py` & `gestionatr-3.8.1/gestionatr/output/messages/base.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/base_gas.py` & `gestionatr-3.8.1/gestionatr/output/messages/base_gas.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_02.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_02.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_03.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_03.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_04.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_04.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_05.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_05.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_38.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_38.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_41.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_41.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_42.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_42.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_43.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_43.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_44.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_44.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_46.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_46.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_48.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_48.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a1_49.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a1_49.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a20_36.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a20_36.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a25_42.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a25_42.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a3.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a3.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_a5_29.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_a5_29.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_b1.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_b1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_b2.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_b2.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_c1.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_c1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_c2.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_c2.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_d1.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_d1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_e1.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_e1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_f1.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_f1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_m1.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_m1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_p0.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_p0.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_q1.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_q1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_r1.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_r1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_t1.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_t1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/output/messages/sw_w1.py` & `gestionatr-3.8.1/gestionatr/output/messages/sw_w1.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/parser_xml_defs_gas.py` & `gestionatr-3.8.1/gestionatr/parser_xml_defs_gas.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr/utils.py` & `gestionatr-3.8.1/gestionatr/utils.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/gestionatr.egg-info/SOURCES.txt` & `gestionatr-3.8.1/gestionatr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/setup.py` & `gestionatr-3.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/tests/test_cli.py` & `gestionatr-3.8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/tests/test_helpers.py` & `gestionatr-3.8.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/tests/test_input.py` & `gestionatr-3.8.1/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/tests/test_output.py` & `gestionatr-3.8.1/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/tests/test_table_description.py` & `gestionatr-3.8.1/tests/test_table_description.py`

 * *Files identical despite different names*

### Comparing `gestionatr-3.8.0/tests/utils.py` & `gestionatr-3.8.1/tests/utils.py`

 * *Files identical despite different names*

