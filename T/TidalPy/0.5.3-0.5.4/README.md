# Comparing `tmp/tidalpy-0.5.3.tar.gz` & `tmp/tidalpy-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidalpy-0.5.3.tar", last modified: Sat Apr 27 01:54:16 2024, max compression
+gzip compressed data, was "tidalpy-0.5.4.tar", last modified: Tue Apr 30 03:13:15 2024, max compression
```

## Comparing `tidalpy-0.5.3.tar` & `tidalpy-0.5.4.tar`

### file list

```diff
@@ -1,499 +1,499 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.008261 tidalpy-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.904260 tidalpy-0.5.3/Benchmarks & Performance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.904260 tidalpy-0.5.3/Benchmarks & Performance/Performance/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.920261 tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/multilayer_radial_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/multimode_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_build_world.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_complex_compliance_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_eccentricity_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_quick_calcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/run_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.904260 tidalpy-0.5.3/Documentation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.904260 tidalpy-0.5.3/Documentation/Issues/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.920261 tidalpy-0.5.3/Documentation/Issues/Issue35/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Documentation/Issues/Issue35/subproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Documentation/Issues/Issue35/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18559 2024-04-27 01:54:02.000000 tidalpy-0.5.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-27 01:54:02.000000 tidalpy-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-27 01:54:16.008261 tidalpy-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-04-27 01:54:02.000000 tidalpy-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.908260 tidalpy-0.5.3/Tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.920261 tidalpy-0.5.3/Tests/Test_Functions/
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Functions/test_rheology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.920261 tidalpy-0.5.3/Tests/Test_Math/
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Math/test_utilities_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Math/test_utilities_special.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.908260 tidalpy-0.5.3/Tests/Test_Old/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.920261 tidalpy-0.5.3/Tests/Test_Old/Test_SetA_Package/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetA_Package/test_a_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetA_Package/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetA_Package/test_tidalpy_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.920261 tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_b_utilities_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_b_utilities_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_c_tools_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_c_tools_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_d_basic_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_g_math_special_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_h_voxel_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_i_spherical_mass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.920261 tidalpy-0.5.3/Tests/Test_Old/Test_SetE_Functional/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetE_Functional/test_a_performance_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.904260 tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.920261 tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Dynamics/
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Dynamics/test_dual_dissipation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Dynamics/test_single_dissipation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.924260 tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Rheology/
--rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Rheology/test_compliance_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Rheology/test_partialmelt_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.924260 tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Tides/
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_a_orbital_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_b_dissipation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_c_mode_manipulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.924260 tidalpy-0.5.3/Tests/Test_Old/Test_SetH_QuickCalc/
--rw-r--r--   0 runner    (1001) docker     (127)    17732 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetH_QuickCalc/test_a_quick_dissipation_calc_single_body.py
--rw-r--r--   0 runner    (1001) docker     (127)    22916 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetH_QuickCalc/test_b_quick_dissipation_calc_dual_body.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.924260 tidalpy-0.5.3/Tests/Test_Old/Test_SetK_PlanetBuild/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetK_PlanetBuild/test_a_build_star.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetK_PlanetBuild/test_b_build_layered.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetK_PlanetBuild/test_d_build_burnman_planet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.924260 tidalpy-0.5.3/Tests/Test_Old/Test_SetL_Orbit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.924260 tidalpy-0.5.3/Tests/Test_Old/Test_SetL_Orbit/Test_OrbitClass/
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetL_Orbit/Test_OrbitClass/test_a_orbit_construct.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetL_Orbit/Test_OrbitClass/test_b_orbit_basic_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetL_Orbit/test_orbit_averaging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.924260 tidalpy-0.5.3/Tests/Test_Old/Test_SetO_OOP_Calcs/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetO_OOP_Calcs/test_oop_rheology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetO_OOP_Calcs/test_radiogenic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.924260 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.924260 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/test_a_matrix_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/test_b_fundamental.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/test_c_propagate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.924260 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.928260 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_a_initial_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_b_known_initial_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_c_initial_helper_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_d_initial_value_calc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.928260 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_a_interfaces_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_b_known_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_c_interface_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.928260 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_a_derivatives_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_b_known_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_c_derivative_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.928260 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/test_a_collapse_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/test_b_surface_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/test_c_generalized_collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/test_a_numerical_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/test_b_radial_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/test_d_alma_compare_old.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/test_a_love.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/test_b_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/test_c_nondimensional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.908260 tidalpy-0.5.3/Tests/Test_Old/Test_SetS_Tides/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.928260 tidalpy-0.5.3/Tests/Test_Old/Test_SetS_Tides/Test_Collapse_Modes/
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetS_Tides/Test_Collapse_Modes/test_collapse_mode_freqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.928260 tidalpy-0.5.3/Tests/Test_Old/Test_SetS_Tides/Test_Heating/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetS_Tides/Test_Heating/test_heating.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.928260 tidalpy-0.5.3/Tests/Test_Old/Test_SetS_Tides/Test_Unique_Modes/
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetS_Tides/Test_Unique_Modes/test_unique_freqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.928260 tidalpy-0.5.3/Tests/Test_Old/Test_SetW_OOP_OrbitTides/
--rw-r--r--   0 runner    (1001) docker     (127)    20260 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_a_physics_orbit_global_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_b_physics_orbit_layered_tides.py
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_c_physics_orbit_dual_body_tides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.928260 tidalpy-0.5.3/Tests/Test_Old/Test_SetX_Potential/
--rw-r--r--   0 runner    (1001) docker     (127)    40344 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetX_Potential/test_a_potential.py
--rw-r--r--   0 runner    (1001) docker     (127)    21080 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetX_Potential/test_b_mode_potential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.908260 tidalpy-0.5.3/Tests/Test_Old/Test_SetY_MultiLayer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.932261 tidalpy-0.5.3/Tests/Test_Old/Test_SetY_MultiLayer/Test_Matrix/
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetY_MultiLayer/Test_Matrix/test_d_radial_tidal_heating.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetY_MultiLayer/Test_Matrix/test_e_strain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.932261 tidalpy-0.5.3/Tests/Test_Old/Test_SetY_MultiLayer/Test_Numerical_Int/
--rw-r--r--   0 runner    (1001) docker     (127)    25923 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetY_MultiLayer/Test_Numerical_Int/test_m1_multilayer_modes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.932261 tidalpy-0.5.3/Tests/Test_Old/Test_SetZA_Multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Old/Test_SetZA_Multiprocessing/test_multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.932261 tidalpy-0.5.3/Tests/Test_RadialSolver/
--rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_RadialSolver/test_a_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    16944 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_RadialSolver/test_a_starting_condtions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_RadialSolver/test_b_radial_solver_1layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_RadialSolver/test_d_alma_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_RadialSolver/test_e_radial_solver_3layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.908260 tidalpy-0.5.3/Tests/Test_Utilities/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.932261 tidalpy-0.5.3/Tests/Test_Utilities/Test_Dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Utilities/Test_Dimensions/test_nondimensional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.932261 tidalpy-0.5.3/Tests/Test_Utilities/Test_Exoplanets/
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-27 01:54:02.000000 tidalpy-0.5.3/Tests/Test_Utilities/Test_Exoplanets/test_exoplanet_download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.932261 tidalpy-0.5.3/TidalPy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.936261 tidalpy-0.5.3/TidalPy/Extending/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.936261 tidalpy-0.5.3/TidalPy/Extending/burnman/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/burnman_defaultc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18574 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/burnman_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/burnman_world.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.936261 tidalpy-0.5.3/TidalPy/Extending/burnman/material/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/material/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.936261 tidalpy-0.5.3/TidalPy/Extending/burnman/material/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/material/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/material/custom/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/material/custom/ice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/material/custom/pyrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/material/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/Extending/burnman/package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.944261 tidalpy-0.5.3/TidalPy/RadialSolver/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.944261 tidalpy-0.5.3/TidalPy/RadialSolver/boundaries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/boundaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   202842 2024-04-27 01:54:13.000000 tidalpy-0.5.3/TidalPy/RadialSolver/boundaries/boundaries.c
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/boundaries/boundaries.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/boundaries/boundaries.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.944261 tidalpy-0.5.3/TidalPy/RadialSolver/collapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   190543 2024-04-27 01:54:12.000000 tidalpy-0.5.3/TidalPy/RadialSolver/collapse/collapse.c
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/collapse/collapse.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/collapse/collapse.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.952261 tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1171789 2024-04-27 01:54:13.000000 tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/base.c
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/base.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/base.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1555718 2024-04-27 01:54:13.000000 tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/odes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/odes.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    29872 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/odes.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.952261 tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1124791 2024-04-27 01:54:13.000000 tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/interfaces.c
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/interfaces.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/interfaces.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   221280 2024-04-27 01:54:13.000000 tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/reversed.c
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/reversed.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/reversed.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1021680 2024-04-27 01:54:14.000000 tidalpy-0.5.3/TidalPy/RadialSolver/love.c
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/love.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/love.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   245435 2024-04-27 01:54:13.000000 tidalpy-0.5.3/TidalPy/RadialSolver/solutions.c
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/solutions.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/solutions.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1732510 2024-04-27 01:54:14.000000 tidalpy-0.5.3/TidalPy/RadialSolver/solver.c
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/solver.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    57813 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/solver.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.960261 tidalpy-0.5.3/TidalPy/RadialSolver/starting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   199417 2024-04-27 01:54:13.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/common.c
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/common.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/common.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1109103 2024-04-27 01:54:14.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/driver.c
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/driver.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/driver.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   265907 2024-04-27 01:54:14.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/kamata.c
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/kamata.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    23616 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/kamata.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   170303 2024-04-27 01:54:14.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/saito.c
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/saito.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/saito.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   254021 2024-04-27 01:54:14.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/takeuchi.c
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/takeuchi.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/RadialSolver/starting/takeuchi.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.960261 tidalpy-0.5.3/TidalPy/WorldPack/
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/WorldPack/WorldPack.zip
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.960261 tidalpy-0.5.3/TidalPy/cooling/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/cooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/cooling/cooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/cooling/cooling_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/defaultc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.960261 tidalpy-0.5.3/TidalPy/dynamics/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/dynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/dynamics/dual_dissipation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/dynamics/single_dissipation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.960261 tidalpy-0.5.3/TidalPy/numba_scipy/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/numba_scipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.960261 tidalpy-0.5.3/TidalPy/numba_scipy/special/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/numba_scipy/special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/numba_scipy/special/overloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/numba_scipy/special/signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.960261 tidalpy-0.5.3/TidalPy/orbit/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/orbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/orbit/averaging.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.960261 tidalpy-0.5.3/TidalPy/radial_solver/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/love.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.964261 tidalpy-0.5.3/TidalPy/radial_solver/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22075 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/matrix/fundamental_solid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/matrix/propagate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/nondimensional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.964261 tidalpy-0.5.3/TidalPy/radial_solver/numerical/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.964261 tidalpy-0.5.3/TidalPy/radial_solver/numerical/collapse/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15279 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/collapse/generalized_collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/collapse/surface_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.964261 tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/odes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_dynamic_incomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_static_incomp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.964261 tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26624 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/initial_solution_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/initial_solution_dynamic_incomp.py
--rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/initial_solution_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/initial_solution_static_incomp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.968261 tidalpy-0.5.3/TidalPy/radial_solver/numerical/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8903 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/interfaces/liquid_liquid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/interfaces/liquid_solid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/interfaces/solid_liquid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/interfaces/solid_solid.py
--rw-r--r--   0 runner    (1001) docker     (127)    19267 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/numerical/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radial_solver/sensitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.968261 tidalpy-0.5.3/TidalPy/radiogenics/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radiogenics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radiogenics/radiogenic_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/radiogenics/radiogenics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.972261 tidalpy-0.5.3/TidalPy/rheology/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1182412 2024-04-27 01:54:15.000000 tidalpy-0.5.3/TidalPy/rheology/base.c
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/base.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/base.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.972261 tidalpy-0.5.3/TidalPy/rheology/complex_compliance/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/complex_compliance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/complex_compliance/complex_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)    26732 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/complex_compliance/compliance_models.py
--rw-r--r--   0 runner    (1001) docker     (127)   955206 2024-04-27 01:54:14.000000 tidalpy-0.5.3/TidalPy/rheology/models.c
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/models.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/models.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.972261 tidalpy-0.5.3/TidalPy/rheology/partial_melt/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/partial_melt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/partial_melt/melting_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/partial_melt/partialmelt.py
--rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/rheology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.972261 tidalpy-0.5.3/TidalPy/rheology/viscosity/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/viscosity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/viscosity/viscosity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/rheology/viscosity/viscosity_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.972261 tidalpy-0.5.3/TidalPy/stellar/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/stellar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/stellar/habitability.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/stellar/insolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/stellar/stellar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.972261 tidalpy-0.5.3/TidalPy/structures/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.972261 tidalpy-0.5.3/TidalPy/structures/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/helpers/orbit_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.976261 tidalpy-0.5.3/TidalPy/structures/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16628 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/layers/gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/layers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23529 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/layers/physics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.976261 tidalpy-0.5.3/TidalPy/structures/orbit/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/orbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75444 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/orbit/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26535 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/orbit/physics.py
--rw-r--r--   0 runner    (1001) docker     (127)    31625 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/physical.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.976261 tidalpy-0.5.3/TidalPy/structures/world_builder/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/world_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/world_builder/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/world_builder/iterative_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/world_builder/world_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.976261 tidalpy-0.5.3/TidalPy/structures/world_types/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/world_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34832 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/world_types/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/world_types/gas.py
--rw-r--r--   0 runner    (1001) docker     (127)    20549 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/world_types/layered.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/world_types/stellar.py
--rw-r--r--   0 runner    (1001) docker     (127)    15842 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/structures/world_types/tidal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.976261 tidalpy-0.5.3/TidalPy/tides/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.980261 tidalpy-0.5.3/TidalPy/tides/ctl_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/ctl_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/ctl_funcs/ctl_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/dissipation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.980261 tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)     8899 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49635 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl2.py
--rw-r--r--   0 runner    (1001) docker     (127)    51626 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl3.py
--rw-r--r--   0 runner    (1001) docker     (127)    63234 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl4.py
--rw-r--r--   0 runner    (1001) docker     (127)    72860 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl5.py
--rw-r--r--   0 runner    (1001) docker     (127)    85694 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl6.py
--rw-r--r--   0 runner    (1001) docker     (127)    97164 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl7.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/heating.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.980261 tidalpy-0.5.3/TidalPy/tides/inclination_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/inclination_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl4.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl6.py
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl7.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/love1d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.980261 tidalpy-0.5.3/TidalPy/tides/methods/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31858 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/methods/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19049 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/methods/global_approx.py
--rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/methods/layered.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.984261 tidalpy-0.5.3/TidalPy/tides/modes/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/collapse_modes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.984261 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl4.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl5.py
--rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl6.py
--rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl7.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl7.py
--rw-r--r--   0 runner    (1001) docker     (127)    22504 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/mode_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)    31353 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/modes/multilayer_modes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.984261 tidalpy-0.5.3/TidalPy/tides/multilayer/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/multilayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/multilayer/displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/multilayer/heating.py
--rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/multilayer/stress_strain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.988261 tidalpy-0.5.3/TidalPy/tides/potential/
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/potential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15450 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/potential/nsr_med_eccen_gen_obliquity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13069 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/potential/nsr_med_eccen_med_obliquity.py
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/potential/nsr_med_eccen_no_obliquity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/potential/nsr_modes_low_eccen_gen_obliquity.py
--rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/potential/nsr_modes_med_eccen_gen_obliquity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/potential/nsr_modes_med_eccen_med_obliquity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/potential/nsr_modes_med_eccen_no_obliquity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/potential/synchronous_low_e.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/tides/universal_coeffs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.988261 tidalpy-0.5.3/TidalPy/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33335 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/toolbox/quick_tides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.988261 tidalpy-0.5.3/TidalPy/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.992261 tidalpy-0.5.3/TidalPy/utilities/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/classes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)   373398 2024-04-27 01:54:14.000000 tidalpy-0.5.3/TidalPy/utilities/classes/base_x.c
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/classes/base_x.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/classes/base_x.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.992261 tidalpy-0.5.3/TidalPy/utilities/classes/config/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/classes/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/classes/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.992261 tidalpy-0.5.3/TidalPy/utilities/classes/model/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/classes/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/classes/model/functional_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/classes/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/classes/model/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   163311 2024-04-27 01:54:14.000000 tidalpy-0.5.3/TidalPy/utilities/constants_x.c
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/constants_x.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/constants_x.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.992261 tidalpy-0.5.3/TidalPy/utilities/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/conversions/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)   365422 2024-04-27 01:54:14.000000 tidalpy-0.5.3/TidalPy/utilities/conversions/conversions_x.c
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/conversions/conversions_x.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/conversions/conversions_x.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/conversions/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/dictionary_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.996261 tidalpy-0.5.3/TidalPy/utilities/dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/dimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1323901 2024-04-27 01:54:15.000000 tidalpy-0.5.3/TidalPy/utilities/dimensions/nondimensional.c
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/dimensions/nondimensional.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/dimensions/nondimensional.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.996261 tidalpy-0.5.3/TidalPy/utilities/exoplanets/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/exoplanets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/exoplanets/data_download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:15.996261 tidalpy-0.5.3/TidalPy/utilities/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/graphics/global_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    28144 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/graphics/grid_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.000261 tidalpy-0.5.3/TidalPy/utilities/graphics/multilayer/
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/graphics/multilayer/RN08-Data.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/graphics/multilayer/T05-Data.csv
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/graphics/multilayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/graphics/multilayer/yplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/graphics/phasespace_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/graphics/planet_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.000261 tidalpy-0.5.3/TidalPy/utilities/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/integration/cyrk_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/integration/julia_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/integration/numbalsoda_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/integration/scipy_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.000261 tidalpy-0.5.3/TidalPy/utilities/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/io/pathing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/io/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.000261 tidalpy-0.5.3/TidalPy/utilities/math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   413061 2024-04-27 01:54:15.000000 tidalpy-0.5.3/TidalPy/utilities/math/complex.c
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/math/complex.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/math/complex.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/math/special.py
--rw-r--r--   0 runner    (1001) docker     (127)   289989 2024-04-27 01:54:15.000000 tidalpy-0.5.3/TidalPy/utilities/math/special_x.c
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/math/special_x.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/math/special_x.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.004261 tidalpy-0.5.3/TidalPy/utilities/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19569 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/multiprocessing/multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.004261 tidalpy-0.5.3/TidalPy/utilities/numpy_helper/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/numpy_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/numpy_helper/array_other.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/numpy_helper/array_shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.004261 tidalpy-0.5.3/TidalPy/utilities/performance/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/performance/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/performance/numba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.004261 tidalpy-0.5.3/TidalPy/utilities/performance/special/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/performance/special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/performance/special/factorial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.004261 tidalpy-0.5.3/TidalPy/utilities/spherical_helper/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/spherical_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/spherical_helper/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/spherical_helper/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.004261 tidalpy-0.5.3/TidalPy/utilities/string_helper/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/string_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/string_helper/string_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (127)   167099 2024-04-27 01:54:15.000000 tidalpy-0.5.3/TidalPy/utilities/types_x.c
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/types_x.pxd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:02.000000 tidalpy-0.5.3/TidalPy/utilities/types_x.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:54:16.004261 tidalpy-0.5.3/TidalPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-27 01:54:15.000000 tidalpy-0.5.3/TidalPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-04-27 01:54:15.000000 tidalpy-0.5.3/TidalPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 01:54:15.000000 tidalpy-0.5.3/TidalPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-27 01:54:15.000000 tidalpy-0.5.3/TidalPy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-27 01:54:15.000000 tidalpy-0.5.3/TidalPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-27 01:54:15.000000 tidalpy-0.5.3/TidalPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-27 01:54:02.000000 tidalpy-0.5.3/_build_tidalpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-04-27 01:54:02.000000 tidalpy-0.5.3/cython_extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-27 01:54:02.000000 tidalpy-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 01:54:16.008261 tidalpy-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-27 01:54:02.000000 tidalpy-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.563836 tidalpy-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.471837 tidalpy-0.5.4/Benchmarks & Performance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.471837 tidalpy-0.5.4/Benchmarks & Performance/Performance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.483837 tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-30 03:13:01.000000 tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/multilayer_radial_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-30 03:13:01.000000 tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/multimode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-30 03:13:01.000000 tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-30 03:13:01.000000 tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_build_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-30 03:13:01.000000 tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_complex_compliance_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-30 03:13:01.000000 tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_eccentricity_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-04-30 03:13:01.000000 tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_quick_calcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-30 03:13:01.000000 tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-30 03:13:01.000000 tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/run_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.471837 tidalpy-0.5.4/Documentation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.471837 tidalpy-0.5.4/Documentation/Issues/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.487837 tidalpy-0.5.4/Documentation/Issues/Issue35/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Documentation/Issues/Issue35/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Documentation/Issues/Issue35/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18559 2024-04-30 03:13:02.000000 tidalpy-0.5.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-30 03:13:02.000000 tidalpy-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-30 03:13:15.563836 tidalpy-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-04-30 03:13:02.000000 tidalpy-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.475837 tidalpy-0.5.4/Tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.487837 tidalpy-0.5.4/Tests/Test_Functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Functions/test_rheology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.487837 tidalpy-0.5.4/Tests/Test_Math/
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Math/test_utilities_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Math/test_utilities_special.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.475837 tidalpy-0.5.4/Tests/Test_Old/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.487837 tidalpy-0.5.4/Tests/Test_Old/Test_SetA_Package/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetA_Package/test_a_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetA_Package/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetA_Package/test_tidalpy_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.487837 tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_b_utilities_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_b_utilities_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_c_tools_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_c_tools_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_d_basic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_g_math_special_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_h_voxel_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_i_spherical_mass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.487837 tidalpy-0.5.4/Tests/Test_Old/Test_SetE_Functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetE_Functional/test_a_performance_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.475837 tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.487837 tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Dynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Dynamics/test_dual_dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Dynamics/test_single_dissipation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.487837 tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Rheology/
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Rheology/test_compliance_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Rheology/test_partialmelt_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.487837 tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Tides/
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_a_orbital_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_b_dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_c_mode_manipulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.487837 tidalpy-0.5.4/Tests/Test_Old/Test_SetH_QuickCalc/
+-rw-r--r--   0 runner    (1001) docker     (127)    17732 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetH_QuickCalc/test_a_quick_dissipation_calc_single_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22916 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetH_QuickCalc/test_b_quick_dissipation_calc_dual_body.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.491837 tidalpy-0.5.4/Tests/Test_Old/Test_SetK_PlanetBuild/
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetK_PlanetBuild/test_a_build_star.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetK_PlanetBuild/test_b_build_layered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetK_PlanetBuild/test_d_build_burnman_planet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.491837 tidalpy-0.5.4/Tests/Test_Old/Test_SetL_Orbit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.491837 tidalpy-0.5.4/Tests/Test_Old/Test_SetL_Orbit/Test_OrbitClass/
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetL_Orbit/Test_OrbitClass/test_a_orbit_construct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetL_Orbit/Test_OrbitClass/test_b_orbit_basic_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetL_Orbit/test_orbit_averaging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.491837 tidalpy-0.5.4/Tests/Test_Old/Test_SetO_OOP_Calcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetO_OOP_Calcs/test_oop_rheology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetO_OOP_Calcs/test_radiogenic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.491837 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.491837 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/test_a_matrix_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/test_b_fundamental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/test_c_propagate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.491837 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.491837 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_a_initial_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_b_known_initial_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_c_initial_helper_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_d_initial_value_calc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.491837 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_a_interfaces_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_b_known_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_c_interface_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.491837 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_a_derivatives_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_b_known_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_c_derivative_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/test_a_collapse_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/test_b_surface_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/test_c_generalized_collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/test_a_numerical_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/test_b_radial_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/test_d_alma_compare_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/test_a_love.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/test_b_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/test_c_nondimensional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.475837 tidalpy-0.5.4/Tests/Test_Old/Test_SetS_Tides/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_Old/Test_SetS_Tides/Test_Collapse_Modes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetS_Tides/Test_Collapse_Modes/test_collapse_mode_freqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_Old/Test_SetS_Tides/Test_Heating/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetS_Tides/Test_Heating/test_heating.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_Old/Test_SetS_Tides/Test_Unique_Modes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetS_Tides/Test_Unique_Modes/test_unique_freqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_Old/Test_SetW_OOP_OrbitTides/
+-rw-r--r--   0 runner    (1001) docker     (127)    20260 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_a_physics_orbit_global_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_b_physics_orbit_layered_tides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_c_physics_orbit_dual_body_tides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_Old/Test_SetX_Potential/
+-rw-r--r--   0 runner    (1001) docker     (127)    40344 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetX_Potential/test_a_potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21080 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetX_Potential/test_b_mode_potential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.475837 tidalpy-0.5.4/Tests/Test_Old/Test_SetY_MultiLayer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_Old/Test_SetY_MultiLayer/Test_Matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetY_MultiLayer/Test_Matrix/test_d_radial_tidal_heating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetY_MultiLayer/Test_Matrix/test_e_strain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_Old/Test_SetY_MultiLayer/Test_Numerical_Int/
+-rw-r--r--   0 runner    (1001) docker     (127)    25923 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetY_MultiLayer/Test_Numerical_Int/test_m1_multilayer_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_Old/Test_SetZA_Multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Old/Test_SetZA_Multiprocessing/test_multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_RadialSolver/
+-rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_RadialSolver/test_a_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16944 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_RadialSolver/test_a_starting_condtions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_RadialSolver/test_b_radial_solver_1layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_RadialSolver/test_d_alma_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_RadialSolver/test_e_radial_solver_3layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.475837 tidalpy-0.5.4/Tests/Test_Utilities/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_Utilities/Test_Dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Utilities/Test_Dimensions/test_nondimensional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.495837 tidalpy-0.5.4/Tests/Test_Utilities/Test_Exoplanets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-30 03:13:02.000000 tidalpy-0.5.4/Tests/Test_Utilities/Test_Exoplanets/test_exoplanet_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.499837 tidalpy-0.5.4/TidalPy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.499837 tidalpy-0.5.4/TidalPy/Extending/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.499837 tidalpy-0.5.4/TidalPy/Extending/burnman/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/burnman_defaultc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18574 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/burnman_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/burnman_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.499837 tidalpy-0.5.4/TidalPy/Extending/burnman/material/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/material/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.499837 tidalpy-0.5.4/TidalPy/Extending/burnman/material/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/material/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/material/custom/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/material/custom/ice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/material/custom/pyrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/material/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/Extending/burnman/package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.507837 tidalpy-0.5.4/TidalPy/RadialSolver/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.507837 tidalpy-0.5.4/TidalPy/RadialSolver/boundaries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/boundaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   202842 2024-04-30 03:13:13.000000 tidalpy-0.5.4/TidalPy/RadialSolver/boundaries/boundaries.c
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/boundaries/boundaries.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/boundaries/boundaries.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.507837 tidalpy-0.5.4/TidalPy/RadialSolver/collapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190543 2024-04-30 03:13:12.000000 tidalpy-0.5.4/TidalPy/RadialSolver/collapse/collapse.c
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/collapse/collapse.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/collapse/collapse.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.511837 tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1171789 2024-04-30 03:13:12.000000 tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/base.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/base.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/base.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1555718 2024-04-30 03:13:12.000000 tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/odes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/odes.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    29872 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/odes.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.515837 tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1124791 2024-04-30 03:13:12.000000 tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/interfaces.c
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/interfaces.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/interfaces.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   221280 2024-04-30 03:13:12.000000 tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/reversed.c
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/reversed.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/reversed.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1021680 2024-04-30 03:13:13.000000 tidalpy-0.5.4/TidalPy/RadialSolver/love.c
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/love.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/love.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   245435 2024-04-30 03:13:12.000000 tidalpy-0.5.4/TidalPy/RadialSolver/solutions.c
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/solutions.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/solutions.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1735431 2024-04-30 03:13:13.000000 tidalpy-0.5.4/TidalPy/RadialSolver/solver.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/solver.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    58039 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/solver.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.519837 tidalpy-0.5.4/TidalPy/RadialSolver/starting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   199417 2024-04-30 03:13:13.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/common.c
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/common.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/common.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1109103 2024-04-30 03:13:14.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/driver.c
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/driver.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/driver.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   265907 2024-04-30 03:13:13.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/kamata.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/kamata.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    23616 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/kamata.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   170303 2024-04-30 03:13:13.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/saito.c
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/saito.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/saito.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   254021 2024-04-30 03:13:13.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/takeuchi.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/takeuchi.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    18263 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/RadialSolver/starting/takeuchi.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.519837 tidalpy-0.5.4/TidalPy/WorldPack/
+-rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/WorldPack/WorldPack.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.519837 tidalpy-0.5.4/TidalPy/cooling/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/cooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/cooling/cooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/cooling/cooling_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/defaultc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.519837 tidalpy-0.5.4/TidalPy/dynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/dynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/dynamics/dual_dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/dynamics/single_dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.519837 tidalpy-0.5.4/TidalPy/numba_scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/numba_scipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.519837 tidalpy-0.5.4/TidalPy/numba_scipy/special/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/numba_scipy/special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/numba_scipy/special/overloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/numba_scipy/special/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.523837 tidalpy-0.5.4/TidalPy/orbit/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/orbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/orbit/averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.523837 tidalpy-0.5.4/TidalPy/radial_solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/love.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.523837 tidalpy-0.5.4/TidalPy/radial_solver/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22075 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/matrix/fundamental_solid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/matrix/propagate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/nondimensional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.523837 tidalpy-0.5.4/TidalPy/radial_solver/numerical/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.523837 tidalpy-0.5.4/TidalPy/radial_solver/numerical/collapse/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15279 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/collapse/generalized_collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/collapse/surface_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.523837 tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/odes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_dynamic_incomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_static_incomp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.527837 tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26624 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/initial_solution_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/initial_solution_dynamic_incomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/initial_solution_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/initial_solution_static_incomp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.527837 tidalpy-0.5.4/TidalPy/radial_solver/numerical/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8903 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/interfaces/liquid_liquid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/interfaces/liquid_solid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/interfaces/solid_liquid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/interfaces/solid_solid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19267 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/numerical/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radial_solver/sensitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.527837 tidalpy-0.5.4/TidalPy/radiogenics/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radiogenics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radiogenics/radiogenic_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/radiogenics/radiogenics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.531837 tidalpy-0.5.4/TidalPy/rheology/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1182412 2024-04-30 03:13:14.000000 tidalpy-0.5.4/TidalPy/rheology/base.c
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/base.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/base.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.531837 tidalpy-0.5.4/TidalPy/rheology/complex_compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/complex_compliance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/complex_compliance/complex_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26732 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/complex_compliance/compliance_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)   955206 2024-04-30 03:13:14.000000 tidalpy-0.5.4/TidalPy/rheology/models.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/models.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/models.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.531837 tidalpy-0.5.4/TidalPy/rheology/partial_melt/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/partial_melt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/partial_melt/melting_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/partial_melt/partialmelt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/rheology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.531837 tidalpy-0.5.4/TidalPy/rheology/viscosity/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/viscosity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/viscosity/viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/rheology/viscosity/viscosity_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.531837 tidalpy-0.5.4/TidalPy/stellar/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/stellar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/stellar/habitability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/stellar/insolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/stellar/stellar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.531837 tidalpy-0.5.4/TidalPy/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.531837 tidalpy-0.5.4/TidalPy/structures/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/helpers/orbit_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.535837 tidalpy-0.5.4/TidalPy/structures/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16628 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/layers/gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/layers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23529 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/layers/physics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.535837 tidalpy-0.5.4/TidalPy/structures/orbit/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/orbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75444 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/orbit/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26535 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/orbit/physics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31625 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/physical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.535837 tidalpy-0.5.4/TidalPy/structures/world_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/world_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/world_builder/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/world_builder/iterative_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/world_builder/world_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.535837 tidalpy-0.5.4/TidalPy/structures/world_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/world_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34832 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/world_types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/world_types/gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20549 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/world_types/layered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/world_types/stellar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15842 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/structures/world_types/tidal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.535837 tidalpy-0.5.4/TidalPy/tides/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.535837 tidalpy-0.5.4/TidalPy/tides/ctl_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/ctl_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/ctl_funcs/ctl_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/dissipation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.539837 tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8899 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49635 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51626 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63234 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72860 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85694 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl6.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97164 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/heating.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.539837 tidalpy-0.5.4/TidalPy/tides/inclination_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/inclination_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl6.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/love1d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.539837 tidalpy-0.5.4/TidalPy/tides/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31858 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/methods/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19049 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/methods/global_approx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/methods/layered.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.539837 tidalpy-0.5.4/TidalPy/tides/modes/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/collapse_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.543836 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl7.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22504 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/mode_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31353 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/modes/multilayer_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.543836 tidalpy-0.5.4/TidalPy/tides/multilayer/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/multilayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/multilayer/displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/multilayer/heating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/multilayer/stress_strain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.543836 tidalpy-0.5.4/TidalPy/tides/potential/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/potential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15450 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/potential/nsr_med_eccen_gen_obliquity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13069 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/potential/nsr_med_eccen_med_obliquity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/potential/nsr_med_eccen_no_obliquity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/potential/nsr_modes_low_eccen_gen_obliquity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/potential/nsr_modes_med_eccen_gen_obliquity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13485 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/potential/nsr_modes_med_eccen_med_obliquity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/potential/nsr_modes_med_eccen_no_obliquity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/potential/synchronous_low_e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/tides/universal_coeffs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.543836 tidalpy-0.5.4/TidalPy/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33335 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/toolbox/quick_tides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.547836 tidalpy-0.5.4/TidalPy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.547836 tidalpy-0.5.4/TidalPy/utilities/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/classes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   373398 2024-04-30 03:13:14.000000 tidalpy-0.5.4/TidalPy/utilities/classes/base_x.c
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/classes/base_x.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/classes/base_x.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.547836 tidalpy-0.5.4/TidalPy/utilities/classes/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/classes/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/classes/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.547836 tidalpy-0.5.4/TidalPy/utilities/classes/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/classes/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/classes/model/functional_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/classes/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/classes/model/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   163311 2024-04-30 03:13:14.000000 tidalpy-0.5.4/TidalPy/utilities/constants_x.c
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/constants_x.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/constants_x.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.551837 tidalpy-0.5.4/TidalPy/utilities/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/conversions/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   365422 2024-04-30 03:13:14.000000 tidalpy-0.5.4/TidalPy/utilities/conversions/conversions_x.c
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/conversions/conversions_x.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/conversions/conversions_x.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/conversions/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/dictionary_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.551837 tidalpy-0.5.4/TidalPy/utilities/dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/dimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1323901 2024-04-30 03:13:14.000000 tidalpy-0.5.4/TidalPy/utilities/dimensions/nondimensional.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/dimensions/nondimensional.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/dimensions/nondimensional.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.551837 tidalpy-0.5.4/TidalPy/utilities/exoplanets/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/exoplanets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/exoplanets/data_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.555837 tidalpy-0.5.4/TidalPy/utilities/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13073 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/graphics/global_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28144 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/graphics/grid_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.555837 tidalpy-0.5.4/TidalPy/utilities/graphics/multilayer/
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/graphics/multilayer/RN08-Data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/graphics/multilayer/T05-Data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/graphics/multilayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/graphics/multilayer/yplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/graphics/phasespace_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/graphics/planet_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.555837 tidalpy-0.5.4/TidalPy/utilities/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/integration/cyrk_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/integration/julia_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/integration/numbalsoda_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/integration/scipy_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.555837 tidalpy-0.5.4/TidalPy/utilities/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/io/pathing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/io/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.555837 tidalpy-0.5.4/TidalPy/utilities/math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   413061 2024-04-30 03:13:14.000000 tidalpy-0.5.4/TidalPy/utilities/math/complex.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/math/complex.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/math/complex.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/math/special.py
+-rw-r--r--   0 runner    (1001) docker     (127)   289989 2024-04-30 03:13:14.000000 tidalpy-0.5.4/TidalPy/utilities/math/special_x.c
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/math/special_x.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/math/special_x.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.559836 tidalpy-0.5.4/TidalPy/utilities/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19569 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/multiprocessing/multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.559836 tidalpy-0.5.4/TidalPy/utilities/numpy_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/numpy_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/numpy_helper/array_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/numpy_helper/array_shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.559836 tidalpy-0.5.4/TidalPy/utilities/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/performance/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/performance/numba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.559836 tidalpy-0.5.4/TidalPy/utilities/performance/special/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/performance/special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/performance/special/factorial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.559836 tidalpy-0.5.4/TidalPy/utilities/spherical_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/spherical_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/spherical_helper/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/spherical_helper/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.559836 tidalpy-0.5.4/TidalPy/utilities/string_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/string_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/string_helper/string_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167099 2024-04-30 03:13:14.000000 tidalpy-0.5.4/TidalPy/utilities/types_x.c
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/types_x.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:02.000000 tidalpy-0.5.4/TidalPy/utilities/types_x.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:13:15.559836 tidalpy-0.5.4/TidalPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-30 03:13:15.000000 tidalpy-0.5.4/TidalPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-04-30 03:13:15.000000 tidalpy-0.5.4/TidalPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 03:13:15.000000 tidalpy-0.5.4/TidalPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 03:13:15.000000 tidalpy-0.5.4/TidalPy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-30 03:13:15.000000 tidalpy-0.5.4/TidalPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 03:13:15.000000 tidalpy-0.5.4/TidalPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-30 03:13:02.000000 tidalpy-0.5.4/_build_tidalpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-04-30 03:13:02.000000 tidalpy-0.5.4/cython_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-30 03:13:02.000000 tidalpy-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 03:13:15.563836 tidalpy-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-30 03:13:02.000000 tidalpy-0.5.4/setup.py
```

### Comparing `tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/multilayer_radial_solver.py` & `tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/multilayer_radial_solver.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/multimode_solver.py` & `tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/multimode_solver.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_base.py` & `tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_base.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_build_world.py` & `tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_build_world.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_complex_compliance_func.py` & `tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_complex_compliance_func.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_eccentricity_func.py` & `tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_eccentricity_func.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_quick_calcs.py` & `tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_quick_calcs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/performance_tides.py` & `tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/performance_tides.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Benchmarks & Performance/Performance/performance suite/run_suite.py` & `tidalpy-0.5.4/Benchmarks & Performance/Performance/performance suite/run_suite.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Documentation/Issues/Issue35/subproc.py` & `tidalpy-0.5.4/Documentation/Issues/Issue35/subproc.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Documentation/Issues/Issue35/test.py` & `tidalpy-0.5.4/Documentation/Issues/Issue35/test.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/LICENSE.md` & `tidalpy-0.5.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/PKG-INFO` & `tidalpy-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TidalPy
-Version: 0.5.3
+Version: 0.5.4
 Summary: Tidal Dynamics and Thermal-Orbital Evolution Software Suite Implemented in Cython and Python
 Author-email: "Joe P. Renaud" <TidalPy@gmail.com>
 License: # License
         
         ## Creative Commons Attribution-ShareAlike 4.0 International
         Creative Commons Corporation (“Creative Commons”) is not a law firm and does not provide legal services or legal advice. Distribution of Creative Commons public licenses does not create a lawyer-client or other relationship. Creative Commons makes its licenses and related information available on an “as-is” basis. Creative Commons gives no warranties regarding its licenses, any material licensed under their terms and conditions, or any related information. Creative Commons disclaims all liability for damages resulting from their use to the fullest extent possible.
         
@@ -244,15 +244,15 @@
     <!--<a href="https://codecov.io/github/jrenaud90/TidalPy" ><img src="https://codecov.io/github/jrenaud90/TidalPy/branch/main/graph/badge.svg?token=35OY4ZLOA5"/></a><br />-->
     <a href="https://doi.org/10.5281/zenodo.7017475"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7017475.svg" alt="DOI"></a>
     <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/Python-3.9|3.10|3.11|3.12-blue" alt="Python Version 3.9-3.12" /></a>
 </div>
 
 ---
 
-<a href="https://github.com/jrenaud90/TidalPy/releases"><img src="https://img.shields.io/badge/TidalPy-0.5.3 Alpha-orange" alt="TidalPy Version 0.5.3 Alpha" /></a>
+<a href="https://github.com/jrenaud90/TidalPy/releases"><img src="https://img.shields.io/badge/TidalPy-0.5.4 Alpha-orange" alt="TidalPy Version 0.5.4 Alpha" /></a>
 
 **Tidal Dynamics and Thermal-Orbital Evolution Software Suite Implemented in Cython and Python**
 
 TidalPy is an open-source software suite that utilizes a semi-analytic approach to estimate tidal heating,
 orbit-rotation evolution, and thermal changes for rocky and icy worlds. It has been used to simulate the thermal-orbital
 evolution of moons within our Solar System as well as exoplanets beyond. TidalPy's `RadialSolver` package can accurately
 estimate the viscoelastic Love and Shida numbers for a multi-layered world, including the effects of liquid layers,
```

### Comparing `tidalpy-0.5.3/README.md` & `tidalpy-0.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <!--<a href="https://codecov.io/github/jrenaud90/TidalPy" ><img src="https://codecov.io/github/jrenaud90/TidalPy/branch/main/graph/badge.svg?token=35OY4ZLOA5"/></a><br />-->
     <a href="https://doi.org/10.5281/zenodo.7017475"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7017475.svg" alt="DOI"></a>
     <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/Python-3.9|3.10|3.11|3.12-blue" alt="Python Version 3.9-3.12" /></a>
 </div>
 
 ---
 
-<a href="https://github.com/jrenaud90/TidalPy/releases"><img src="https://img.shields.io/badge/TidalPy-0.5.3 Alpha-orange" alt="TidalPy Version 0.5.3 Alpha" /></a>
+<a href="https://github.com/jrenaud90/TidalPy/releases"><img src="https://img.shields.io/badge/TidalPy-0.5.4 Alpha-orange" alt="TidalPy Version 0.5.4 Alpha" /></a>
 
 **Tidal Dynamics and Thermal-Orbital Evolution Software Suite Implemented in Cython and Python**
 
 TidalPy is an open-source software suite that utilizes a semi-analytic approach to estimate tidal heating,
 orbit-rotation evolution, and thermal changes for rocky and icy worlds. It has been used to simulate the thermal-orbital
 evolution of moons within our Solar System as well as exoplanets beyond. TidalPy's `RadialSolver` package can accurately
 estimate the viscoelastic Love and Shida numbers for a multi-layered world, including the effects of liquid layers,
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # TidalPy
 _[_W_i_n_d_o_w_s_ _T_e_s_t_s_]_[_M_a_c_O_S_ _T_e_s_t_s_]_[_U_b_u_n_t_u_ _T_e_s_t_s_]
 _[_D_O_I_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_ _3_._9_-_3_._1_2_]
---- _[_T_i_d_a_l_P_y_ _V_e_r_s_i_o_n_ _0_._5_._3_ _A_l_p_h_a_]**Tidal Dynamics and Thermal-Orbital Evolution
+--- _[_T_i_d_a_l_P_y_ _V_e_r_s_i_o_n_ _0_._5_._4_ _A_l_p_h_a_]**Tidal Dynamics and Thermal-Orbital Evolution
 Software Suite Implemented in Cython and Python** TidalPy is an open-source
 software suite that utilizes a semi-analytic approach to estimate tidal
 heating, orbit-rotation evolution, and thermal changes for rocky and icy
 worlds. It has been used to simulate the thermal-orbital evolution of moons
 within our Solar System as well as exoplanets beyond. TidalPy's `RadialSolver`
 package can accurately estimate the viscoelastic Love and Shida numbers for a
 multi-layered world, including the effects of liquid layers, compressibility,
```

### Comparing `tidalpy-0.5.3/Tests/Test_Functions/test_rheology.py` & `tidalpy-0.5.4/Tests/Test_Functions/test_rheology.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Math/test_utilities_complex.py` & `tidalpy-0.5.4/Tests/Test_Math/test_utilities_complex.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetA_Package/test_io.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetA_Package/test_io.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_b_utilities_functools.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_b_utilities_functools.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_b_utilities_numpy.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_b_utilities_numpy.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_c_tools_conversions.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_c_tools_conversions.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_c_tools_timing.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_c_tools_timing.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_d_basic_classes.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_d_basic_classes.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_g_math_special_funcs.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_g_math_special_funcs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_h_voxel_volume.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_h_voxel_volume.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetB_Package/test_i_spherical_mass.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetB_Package/test_i_spherical_mass.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetE_Functional/test_a_performance_funcs.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetE_Functional/test_a_performance_funcs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Dynamics/test_dual_dissipation.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Dynamics/test_dual_dissipation.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Dynamics/test_single_dissipation.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Dynamics/test_single_dissipation.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Rheology/test_compliance_funcs.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Rheology/test_compliance_funcs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Rheology/test_partialmelt_funcs.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Rheology/test_partialmelt_funcs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_a_orbital_funcs.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_a_orbital_funcs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_b_dissipation.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_b_dissipation.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_c_mode_manipulation.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetF_Functional/Test_Tides/test_c_mode_manipulation.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetH_QuickCalc/test_a_quick_dissipation_calc_single_body.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetH_QuickCalc/test_a_quick_dissipation_calc_single_body.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetH_QuickCalc/test_b_quick_dissipation_calc_dual_body.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetH_QuickCalc/test_b_quick_dissipation_calc_dual_body.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetK_PlanetBuild/test_a_build_star.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetK_PlanetBuild/test_a_build_star.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetK_PlanetBuild/test_b_build_layered.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetK_PlanetBuild/test_b_build_layered.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetK_PlanetBuild/test_d_build_burnman_planet.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetK_PlanetBuild/test_d_build_burnman_planet.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetL_Orbit/Test_OrbitClass/test_a_orbit_construct.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetL_Orbit/Test_OrbitClass/test_a_orbit_construct.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetL_Orbit/Test_OrbitClass/test_b_orbit_basic_manipulation.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetL_Orbit/Test_OrbitClass/test_b_orbit_basic_manipulation.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetL_Orbit/test_orbit_averaging.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetL_Orbit/test_orbit_averaging.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetO_OOP_Calcs/test_oop_rheology.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetO_OOP_Calcs/test_oop_rheology.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetO_OOP_Calcs/test_radiogenic.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetO_OOP_Calcs/test_radiogenic.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/test_b_fundamental.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/test_b_fundamental.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/test_c_propagate.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Matrix/test_c_propagate.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_a_initial_package.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_a_initial_package.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_b_known_initial_funcs.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_b_known_initial_funcs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_c_initial_helper_funcs.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_c_initial_helper_funcs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_d_initial_value_calc.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_a_Initial/test_d_initial_value_calc.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_a_interfaces_package.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_a_interfaces_package.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_b_known_interfaces.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_b_known_interfaces.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_c_interface_funcs.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_b_Interfaces/test_c_interface_funcs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_a_derivatives_package.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_a_derivatives_package.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_b_known_derivatives.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_b_known_derivatives.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_c_derivative_funcs.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_c_Derivatives/test_c_derivative_funcs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/test_b_surface_condition.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/test_b_surface_condition.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/test_c_generalized_collapse.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/Test_d_Collapse/test_c_generalized_collapse.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/test_b_radial_solver.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/test_b_radial_solver.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/test_d_alma_compare_old.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/Test_Numerical/test_d_alma_compare_old.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/test_a_love.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/test_a_love.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/test_b_sensitivity.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/test_b_sensitivity.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetP_RadialSolver/test_c_nondimensional.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetP_RadialSolver/test_c_nondimensional.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetS_Tides/Test_Collapse_Modes/test_collapse_mode_freqs.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetS_Tides/Test_Collapse_Modes/test_collapse_mode_freqs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetS_Tides/Test_Heating/test_heating.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetS_Tides/Test_Heating/test_heating.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetS_Tides/Test_Unique_Modes/test_unique_freqs.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetS_Tides/Test_Unique_Modes/test_unique_freqs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_a_physics_orbit_global_tides.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_a_physics_orbit_global_tides.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_b_physics_orbit_layered_tides.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_b_physics_orbit_layered_tides.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_c_physics_orbit_dual_body_tides.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetW_OOP_OrbitTides/test_c_physics_orbit_dual_body_tides.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetX_Potential/test_a_potential.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetX_Potential/test_a_potential.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetX_Potential/test_b_mode_potential.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetX_Potential/test_b_mode_potential.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetY_MultiLayer/Test_Matrix/test_d_radial_tidal_heating.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetY_MultiLayer/Test_Matrix/test_d_radial_tidal_heating.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetY_MultiLayer/Test_Matrix/test_e_strain.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetY_MultiLayer/Test_Matrix/test_e_strain.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetY_MultiLayer/Test_Numerical_Int/test_m1_multilayer_modes.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetY_MultiLayer/Test_Numerical_Int/test_m1_multilayer_modes.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Old/Test_SetZA_Multiprocessing/test_multiprocessing.py` & `tidalpy-0.5.4/Tests/Test_Old/Test_SetZA_Multiprocessing/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_RadialSolver/test_a_interfaces.py` & `tidalpy-0.5.4/Tests/Test_RadialSolver/test_a_interfaces.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_RadialSolver/test_a_starting_condtions.py` & `tidalpy-0.5.4/Tests/Test_RadialSolver/test_a_starting_condtions.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_RadialSolver/test_b_radial_solver_1layer.py` & `tidalpy-0.5.4/Tests/Test_RadialSolver/test_b_radial_solver_1layer.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_RadialSolver/test_d_alma_compare.py` & `tidalpy-0.5.4/Tests/Test_RadialSolver/test_d_alma_compare.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_RadialSolver/test_e_radial_solver_3layer.py` & `tidalpy-0.5.4/Tests/Test_RadialSolver/test_e_radial_solver_3layer.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Utilities/Test_Dimensions/test_nondimensional.py` & `tidalpy-0.5.4/Tests/Test_Utilities/Test_Dimensions/test_nondimensional.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/Tests/Test_Utilities/Test_Exoplanets/test_exoplanet_download.py` & `tidalpy-0.5.4/Tests/Test_Utilities/Test_Exoplanets/test_exoplanet_download.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/Extending/burnman/build.py` & `tidalpy-0.5.4/TidalPy/Extending/burnman/build.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/Extending/burnman/burnman_defaultc.py` & `tidalpy-0.5.4/TidalPy/Extending/burnman/burnman_defaultc.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/Extending/burnman/burnman_layer.py` & `tidalpy-0.5.4/TidalPy/Extending/burnman/burnman_layer.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/Extending/burnman/burnman_world.py` & `tidalpy-0.5.4/TidalPy/Extending/burnman/burnman_world.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/Extending/burnman/material/custom/constant.py` & `tidalpy-0.5.4/TidalPy/Extending/burnman/material/custom/constant.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/Extending/burnman/material/custom/ice.py` & `tidalpy-0.5.4/TidalPy/Extending/burnman/material/custom/ice.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/Extending/burnman/material/custom/pyrite.py` & `tidalpy-0.5.4/TidalPy/Extending/burnman/material/custom/pyrite.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/Extending/burnman/material/helper.py` & `tidalpy-0.5.4/TidalPy/Extending/burnman/material/helper.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/Extending/burnman/package.py` & `tidalpy-0.5.4/TidalPy/Extending/burnman/package.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/boundaries/boundaries.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/boundaries/boundaries.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/RadialSolver/boundaries",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.boundaries.boundaries",
         "sources": [
             "TidalPy/RadialSolver/boundaries/boundaries.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/boundaries/boundaries.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/boundaries/boundaries.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/collapse/collapse.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/collapse/collapse.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/RadialSolver/collapse",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.collapse.collapse",
         "sources": [
             "TidalPy/RadialSolver/collapse/collapse.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/collapse/collapse.pxd` & `tidalpy-0.5.4/TidalPy/RadialSolver/collapse/collapse.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/collapse/collapse.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/collapse/collapse.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/base.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/base.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,30 +6,30 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/CyRK/array/interp_common.c",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/CyRK/cy/rk_step.c"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/CyRK/array/interp_common.c",
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/CyRK/cy/rk_step.c"
         ],
         "extra_compile_args": [
             "-fopenmp",
             "-O3"
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/CyRK/cy",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/CyRK/array",
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/CyRK/cy",
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/CyRK/array",
             "TidalPy/RadialSolver/derivatives",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.derivatives.base",
         "sources": [
             "TidalPy/RadialSolver/derivatives/base.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/base.pxd` & `tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/base.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/base.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/base.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/odes.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/odes.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,28 +6,28 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/CyRK/cy/rk_step.c"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/CyRK/cy/rk_step.c"
         ],
         "extra_compile_args": [
             "-fopenmp",
             "-O3"
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/CyRK/cy",
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/CyRK/cy",
             "TidalPy/RadialSolver/derivatives",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.derivatives.odes",
         "sources": [
             "TidalPy/RadialSolver/derivatives/odes.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/odes.pxd` & `tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/odes.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/derivatives/odes.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/derivatives/odes.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/interfaces.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/interfaces.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/RadialSolver/interfaces",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.interfaces.interfaces",
         "sources": [
             "TidalPy/RadialSolver/interfaces/interfaces.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/interfaces.pxd` & `tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/interfaces.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/interfaces.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/interfaces.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/reversed.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/reversed.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/RadialSolver/interfaces",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.interfaces.reversed",
         "sources": [
             "TidalPy/RadialSolver/interfaces/reversed.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/reversed.pxd` & `tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/reversed.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/interfaces/reversed.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/interfaces/reversed.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/love.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/love.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/RadialSolver",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.love",
         "sources": [
             "TidalPy/RadialSolver/love.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/love.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/love.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/solutions.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/solutions.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/RadialSolver",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.solutions",
         "sources": [
             "TidalPy/RadialSolver/solutions.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/solutions.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/solutions.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/solver.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/solver.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,33 +6,33 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/CyRK/cy/rk_step.c",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/CyRK/cy/rk_step.c",
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-fopenmp",
             "-O3"
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/CyRK/cy",
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/CyRK/cy",
             "TidalPy/RadialSolver/solver",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.solver",
         "sources": [
             "TidalPy/RadialSolver/solver.pyx"
         ]
     },
@@ -1693,177 +1693,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1907,42 +1907,42 @@
 struct __pyx_obj_7TidalPy_12RadialSolver_11derivatives_4odes_LiquidStaticIncompressible;
 struct __pyx_obj_7TidalPy_12RadialSolver_6solver_RadialSolverSolution;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -4194,14 +4194,15 @@
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_max_step[] = "max_step";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_register[] = "register";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_solution[] = "; solution ";
+static const char __pyx_k_warnings[] = "warnings";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_frequency[] = "frequency";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_solve_for[] = "solve_for";
@@ -4311,15 +4312,15 @@
 static const char __pyx_k_solve_for_argument_must_be_a_tu[] = "`solve_for` argument must be a tuple of strings. For example:\n   (\"tidal\",)  # If you just want tidal Love numbers.\n   (\"tidal\", \"loading\")  # If you just want tidal and loading Love numbers.";
 static const char __pyx_k_All_dimensions_preceding_dimensi[] = "All dimensions preceding dimension %d must be indexed and not sliced";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Cannot_transpose_memoryview_with[] = "Cannot transpose memoryview with indirect dimensions";
-static const char __pyx_k_Dynamic_liquid_layer_detected_in[] = "Dynamic liquid layer detected in RadialSolver for a small frequency. Results may be unstable. Extra care is advised!";
+static const char __pyx_k_Dynamic_liquid_layer_detected_in[] = "Dynamic liquid layer detected in RadialSolver for a small frequency.Results may be unstable. Extra care is advised!";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
 static const char __pyx_k_Error_encountered_while_applying[] = "Error encountered while applying surface boundary condition. ZGESV code: ";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Integration_completed_for_all_la[] = "Integration completed for all layers. Beginning solution collapse.";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got ";
 static const char __pyx_k_NaNs_encountered_after_non_dimen[] = "NaNs encountered after non-dimensionalize call.";
@@ -4391,15 +4392,15 @@
 static PyObject *__pyx_pf_7TidalPy_12RadialSolver_6solver_20RadialSolverSolution_7message___get__(struct __pyx_obj_7TidalPy_12RadialSolver_6solver_RadialSolverSolution *__pyx_v_self); /* proto */
 static int __pyx_pf_7TidalPy_12RadialSolver_6solver_20RadialSolverSolution_7message_2__set__(struct __pyx_obj_7TidalPy_12RadialSolver_6solver_RadialSolverSolution *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_7TidalPy_12RadialSolver_6solver_20RadialSolverSolution_7message_4__del__(struct __pyx_obj_7TidalPy_12RadialSolver_6solver_RadialSolverSolution *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7TidalPy_12RadialSolver_6solver_20RadialSolverSolution_7success___get__(struct __pyx_obj_7TidalPy_12RadialSolver_6solver_RadialSolverSolution *__pyx_v_self); /* proto */
 static int __pyx_pf_7TidalPy_12RadialSolver_6solver_20RadialSolverSolution_7success_2__set__(struct __pyx_obj_7TidalPy_12RadialSolver_6solver_RadialSolverSolution *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_7TidalPy_12RadialSolver_6solver_20RadialSolverSolution_8__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7TidalPy_12RadialSolver_6solver_RadialSolverSolution *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7TidalPy_12RadialSolver_6solver_20RadialSolverSolution_10__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7TidalPy_12RadialSolver_6solver_RadialSolverSolution *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_7TidalPy_12RadialSolver_6solver_radial_solver(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_radius_array, __Pyx_memviewslice __pyx_v_density_array, __Pyx_memviewslice __pyx_v_gravity_array, __Pyx_memviewslice __pyx_v_bulk_modulus_array, __Pyx_memviewslice __pyx_v_complex_shear_modulus_array, double __pyx_v_frequency, double __pyx_v_planet_bulk_density, PyObject *__pyx_v_layer_types, PyObject *__pyx_v_is_static_by_layer, PyObject *__pyx_v_is_incompressible_by_layer, PyObject *__pyx_v_upper_radius_by_layer, unsigned int __pyx_v_degree_l, PyObject *__pyx_v_solve_for, int __pyx_v_use_kamata, PyObject *__pyx_v_integration_method, double __pyx_v_integration_rtol, double __pyx_v_integration_atol, int __pyx_v_scale_rtols_by_layer_type, size_t __pyx_v_max_num_steps, size_t __pyx_v_expected_size, size_t __pyx_v_max_ram_MB, double __pyx_v_max_step, int __pyx_v_limit_solution_to_radius, int __pyx_v_nondimensionalize, int __pyx_v_verbose, int __pyx_v_raise_on_fail); /* proto */
+static PyObject *__pyx_pf_7TidalPy_12RadialSolver_6solver_radial_solver(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_radius_array, __Pyx_memviewslice __pyx_v_density_array, __Pyx_memviewslice __pyx_v_gravity_array, __Pyx_memviewslice __pyx_v_bulk_modulus_array, __Pyx_memviewslice __pyx_v_complex_shear_modulus_array, double __pyx_v_frequency, double __pyx_v_planet_bulk_density, PyObject *__pyx_v_layer_types, PyObject *__pyx_v_is_static_by_layer, PyObject *__pyx_v_is_incompressible_by_layer, PyObject *__pyx_v_upper_radius_by_layer, unsigned int __pyx_v_degree_l, PyObject *__pyx_v_solve_for, int __pyx_v_use_kamata, PyObject *__pyx_v_integration_method, double __pyx_v_integration_rtol, double __pyx_v_integration_atol, int __pyx_v_scale_rtols_by_layer_type, size_t __pyx_v_max_num_steps, size_t __pyx_v_expected_size, size_t __pyx_v_max_ram_MB, double __pyx_v_max_step, int __pyx_v_limit_solution_to_radius, int __pyx_v_nondimensionalize, int __pyx_v_verbose, int __pyx_v_warnings, int __pyx_v_raise_on_fail); /* proto */
 static PyObject *__pyx_tp_new_7TidalPy_12RadialSolver_6solver_RadialSolverSolution(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyUnicode_Type_lower = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
@@ -4752,14 +4753,15 @@
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_s_upper_radius_by_layer;
   PyObject *__pyx_n_s_upper_radius_by_layer_ptr;
   PyObject *__pyx_n_s_use_kamata;
   PyObject *__pyx_n_s_verbose;
   PyObject *__pyx_n_s_version_info;
   PyObject *__pyx_n_s_warning;
+  PyObject *__pyx_n_s_warnings;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
   PyObject *__pyx_int_3;
   PyObject *__pyx_int_112105877;
   PyObject *__pyx_int_136983863;
   PyObject *__pyx_int_184977713;
   PyObject *__pyx_int_neg_1;
@@ -5106,14 +5108,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_s_upper_radius_by_layer);
   Py_CLEAR(clear_module_state->__pyx_n_s_upper_radius_by_layer_ptr);
   Py_CLEAR(clear_module_state->__pyx_n_s_use_kamata);
   Py_CLEAR(clear_module_state->__pyx_n_s_verbose);
   Py_CLEAR(clear_module_state->__pyx_n_s_version_info);
   Py_CLEAR(clear_module_state->__pyx_n_s_warning);
+  Py_CLEAR(clear_module_state->__pyx_n_s_warnings);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_3);
   Py_CLEAR(clear_module_state->__pyx_int_112105877);
   Py_CLEAR(clear_module_state->__pyx_int_136983863);
   Py_CLEAR(clear_module_state->__pyx_int_184977713);
   Py_CLEAR(clear_module_state->__pyx_int_neg_1);
@@ -5438,14 +5441,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_s_upper_radius_by_layer);
   Py_VISIT(traverse_module_state->__pyx_n_s_upper_radius_by_layer_ptr);
   Py_VISIT(traverse_module_state->__pyx_n_s_use_kamata);
   Py_VISIT(traverse_module_state->__pyx_n_s_verbose);
   Py_VISIT(traverse_module_state->__pyx_n_s_version_info);
   Py_VISIT(traverse_module_state->__pyx_n_s_warning);
+  Py_VISIT(traverse_module_state->__pyx_n_s_warnings);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_3);
   Py_VISIT(traverse_module_state->__pyx_int_112105877);
   Py_VISIT(traverse_module_state->__pyx_int_136983863);
   Py_VISIT(traverse_module_state->__pyx_int_184977713);
   Py_VISIT(traverse_module_state->__pyx_int_neg_1);
@@ -5832,14 +5836,15 @@
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_s_upper_radius_by_layer __pyx_mstate_global->__pyx_n_s_upper_radius_by_layer
 #define __pyx_n_s_upper_radius_by_layer_ptr __pyx_mstate_global->__pyx_n_s_upper_radius_by_layer_ptr
 #define __pyx_n_s_use_kamata __pyx_mstate_global->__pyx_n_s_use_kamata
 #define __pyx_n_s_verbose __pyx_mstate_global->__pyx_n_s_verbose
 #define __pyx_n_s_version_info __pyx_mstate_global->__pyx_n_s_version_info
 #define __pyx_n_s_warning __pyx_mstate_global->__pyx_n_s_warning
+#define __pyx_n_s_warnings __pyx_mstate_global->__pyx_n_s_warnings
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_3 __pyx_mstate_global->__pyx_int_3
 #define __pyx_int_112105877 __pyx_mstate_global->__pyx_int_112105877
 #define __pyx_int_136983863 __pyx_mstate_global->__pyx_int_136983863
 #define __pyx_int_184977713 __pyx_mstate_global->__pyx_int_184977713
 #define __pyx_int_neg_1 __pyx_mstate_global->__pyx_int_neg_1
@@ -19870,261 +19875,261 @@
   __Pyx_XDECREF(__pyx_v_parts);
   __Pyx_XDECREF(__pyx_v_extents);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -20133,29 +20138,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -20166,15 +20171,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -20183,29 +20188,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -20216,15 +20221,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -20233,29 +20238,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -20266,15 +20271,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -20283,29 +20288,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -20316,15 +20321,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -20333,29 +20338,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -20366,217 +20371,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -20592,15 +20597,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -20608,68 +20613,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -20677,15 +20682,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -20700,15 +20705,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20724,15 +20729,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -20740,68 +20745,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -20809,15 +20814,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20832,15 +20837,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20856,15 +20861,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -20872,68 +20877,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -20941,15 +20946,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20964,170 +20969,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -28280,15 +28285,15 @@
 static PyObject *__pyx_pw_7TidalPy_12RadialSolver_6solver_1radial_solver(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7TidalPy_12RadialSolver_6solver_radial_solver, "\n    Solves the viscoelastic-gravitational problem for a planet comprised of solid and liquid layers.\n\n    See Takeuchi and Saito (1972) for more details on this method.\n\n    Parameters\n    ----------\n    radius_array : np.ndarray[dtype=np.float64]\n        Radius values defined at slices throughout the planet [m].\n    density_array : np.ndarray[dtype=np.float64]\n        Density at each radius [kg m-3].\n    gravity_array : np.ndarray[dtype=np.float64]\n        Acceleration due to gravity at each radius [m-2].\n    bulk_modulus_array : np.ndarray[dtype=np.float64]\n        Bulk modulus at each radius [Pa].\n    complex_shear_modulus_array : np.ndarray[dtype=np.complex128]\n        Complex shear modulus at each radius [Pa].\n        This should be the result of applying a rheological model to the static shear modulus, viscosity, and\n        forcing frequency.\n    frequency : float64\n        Forcing frequency [rad s-1]\n    planet_bulk_density : float64\n        Bulk density of the planet [kg m-3].\n    layer_types : tuple[string, ...] (Size = number of layers)\n        Indicator of layer type. Current options are:\n            - \"solid\"\n            - \"liquid\"\n    is_static_by_layer : tuple[bool, ...] (Size = number of layers)\n        Flag declaring if each layer uses the static (True) or dynamic (False) assumption.\n    is_incompressible_by_layer : tuple[bool, ...] (Size = number of layers)\n        Flag declaring if each layer is incompressible (True) or compressible (False).\n    upper_radius_by_layer : tuple[float64, ...] (Size = number of layers)\n        Tuple of the upper radius of each layer.\n        Used to determine physical structure of planet.\n    degree_l : uint32, default=2\n        Harmonic degree.\n    solve_for : tuple[str, ...] (Size = number of requested solutions), default=None\n        RadialSolver allows multiple solutions to be solved simultaneously, avoiding repeated integration.\n        This parameter is a tuple of reques""ted solutions. If `None`, then only \"tidal\" will be solved for.\n        Options that are currently supported (note these are case sensitive):\n            - \"tidal\": Tidal forcing boundary conditions.\n            - \"loading\": Surface loading boundary conditions.\n            - \"free\": Free surface boundary conditions.\n        For example, if you want the tidal and loading solutions then you can set \"solve_for=('tidal', 'loading')\".\n    use_kamata : bool, default=False\n        If True, then the starting solution at the core will be based on equations from Kamata et al (2015; JGR:P)\n        Otherwise, starting solution will be based on Takeuchi and Saito (1972)\n    integration_method : int32, default=1\n        Which CyRK integration protocol should be used. Options that are currently available are:\n            - 0: Runge-Kutta 2(3)\n            - 1: Runge-Kutta 4(5)\n            - 2: Runge-Kutta / DOP 8(5/3)\n    integration_rtol : float64, default=1.0e-4\n        Relative integration tolerance. Lower tolerance will lead to more precise results at increased computation.\n    integration_atol : float64, default=1.0e-12\n        Absolute integration tolerance (when solution is near 0).\n    scale_rtols_by_layer_type : bool, default=True\n        If True, then each layer will be imparted with a different relative tolerance. Liquid layers will have a lower\n        rtol which has been found to improve stability.\n    max_num_steps : uint32, default=500,000\n        Maximum number of integration steps allowed before solver forces a failed result.\n        Useful to set to a lower number if running many calls that may be exploring an unstable parameter space for\n        example, during a MCMC run.\n    expected_size : uint32, default=500\n        Anticipated number of integration steps that will be required per solution. Tweaking this may have a minor\n        impact on performance. It is advised to leave it between 200--1000.\n        Setting it too low"" can lead to bad performance.\n    max_ram_MB : uint32, default=500\n        Maximum amount of RAM in MB the integrator is allowed (ignoring some housekeeping usage).\n        The integrator will use this value and the \"max_num_steps\" to determine a true limit on the maximum number\n        steps allowed (picking the lower value.). If system RAM is limited (or if multiple RadialSolvers will run in\n        parallel) it maybe worth setting this lower than the default.\n        The default of 500MB is equivalent to a max_num_steps ~ 5 Mllion.\n    max_step : float64, default=0\n        Maximum step size the adaptive step size integrator is allowed to take. \n        Setting to 0 (default) will tell the integrator to determine an ideal max step size.\n    limit_solution_to_radius : bool, default=True\n        If True, then the solution will be limited to the points passed by the radius array.\n    nondimensionalize : bool, default=True\n        If Ture, then inputs will be non-dimensionalized before integration is performed.\n        Results will be redimensionalized before being returned.\n    verbose : bool, default=False\n        If True, then additioal information will be printed to the terminal during the solution. \n    raise_on_fail : bool, default=False\n        If Ture, then the solver will raise an exception if integration was not successful. By default RadialSolver\n        fails silently. \n\n    Returns\n    -------\n    solution : RadialSolverSolution\n        Solution to the viscoelastic-gravitational problem inside a planet.\n        Solution attributes:\n            - solution.results : complex128, shape=(6 * num_ytypes, n_slice)\n                Numerical solution throughout the planet.\n            - solution.success : bool\n                Flag if integration and subsequent collapse occured without error.\n            - solution.message : str\n                Feedback string useful for debugging.\n    ");
+PyDoc_STRVAR(__pyx_doc_7TidalPy_12RadialSolver_6solver_radial_solver, "\n    Solves the viscoelastic-gravitational problem for a planet comprised of solid and liquid layers.\n\n    See Takeuchi and Saito (1972) for more details on this method.\n\n    Parameters\n    ----------\n    radius_array : np.ndarray[dtype=np.float64]\n        Radius values defined at slices throughout the planet [m].\n    density_array : np.ndarray[dtype=np.float64]\n        Density at each radius [kg m-3].\n    gravity_array : np.ndarray[dtype=np.float64]\n        Acceleration due to gravity at each radius [m-2].\n    bulk_modulus_array : np.ndarray[dtype=np.float64]\n        Bulk modulus at each radius [Pa].\n    complex_shear_modulus_array : np.ndarray[dtype=np.complex128]\n        Complex shear modulus at each radius [Pa].\n        This should be the result of applying a rheological model to the static shear modulus, viscosity, and\n        forcing frequency.\n    frequency : float64\n        Forcing frequency [rad s-1]\n    planet_bulk_density : float64\n        Bulk density of the planet [kg m-3].\n    layer_types : tuple[string, ...] (Size = number of layers)\n        Indicator of layer type. Current options are:\n            - \"solid\"\n            - \"liquid\"\n    is_static_by_layer : tuple[bool, ...] (Size = number of layers)\n        Flag declaring if each layer uses the static (True) or dynamic (False) assumption.\n    is_incompressible_by_layer : tuple[bool, ...] (Size = number of layers)\n        Flag declaring if each layer is incompressible (True) or compressible (False).\n    upper_radius_by_layer : tuple[float64, ...] (Size = number of layers)\n        Tuple of the upper radius of each layer.\n        Used to determine physical structure of planet.\n    degree_l : uint32, default=2\n        Harmonic degree.\n    solve_for : tuple[str, ...] (Size = number of requested solutions), default=None\n        RadialSolver allows multiple solutions to be solved simultaneously, avoiding repeated integration.\n        This parameter is a tuple of reques""ted solutions. If `None`, then only \"tidal\" will be solved for.\n        Options that are currently supported (note these are case sensitive):\n            - \"tidal\": Tidal forcing boundary conditions.\n            - \"loading\": Surface loading boundary conditions.\n            - \"free\": Free surface boundary conditions.\n        For example, if you want the tidal and loading solutions then you can set \"solve_for=('tidal', 'loading')\".\n    use_kamata : bool, default=False\n        If True, then the starting solution at the core will be based on equations from Kamata et al (2015; JGR:P)\n        Otherwise, starting solution will be based on Takeuchi and Saito (1972)\n    integration_method : int32, default=1\n        Which CyRK integration protocol should be used. Options that are currently available are:\n            - 0: Runge-Kutta 2(3)\n            - 1: Runge-Kutta 4(5)\n            - 2: Runge-Kutta / DOP 8(5/3)\n    integration_rtol : float64, default=1.0e-4\n        Relative integration tolerance. Lower tolerance will lead to more precise results at increased computation.\n    integration_atol : float64, default=1.0e-12\n        Absolute integration tolerance (when solution is near 0).\n    scale_rtols_by_layer_type : bool, default=True\n        If True, then each layer will be imparted with a different relative tolerance. Liquid layers will have a lower\n        rtol which has been found to improve stability.\n    max_num_steps : uint32, default=500,000\n        Maximum number of integration steps allowed before solver forces a failed result.\n        Useful to set to a lower number if running many calls that may be exploring an unstable parameter space for\n        example, during a MCMC run.\n    expected_size : uint32, default=500\n        Anticipated number of integration steps that will be required per solution. Tweaking this may have a minor\n        impact on performance. It is advised to leave it between 200--1000.\n        Setting it too low"" can lead to bad performance.\n    max_ram_MB : uint32, default=500\n        Maximum amount of RAM in MB the integrator is allowed (ignoring some housekeeping usage).\n        The integrator will use this value and the \"max_num_steps\" to determine a true limit on the maximum number\n        steps allowed (picking the lower value.). If system RAM is limited (or if multiple RadialSolvers will run in\n        parallel) it maybe worth setting this lower than the default.\n        The default of 500MB is equivalent to a max_num_steps ~ 5 Mllion.\n    max_step : float64, default=0\n        Maximum step size the adaptive step size integrator is allowed to take. \n        Setting to 0 (default) will tell the integrator to determine an ideal max step size.\n    limit_solution_to_radius : bool, default=True\n        If True, then the solution will be limited to the points passed by the radius array.\n    nondimensionalize : bool, default=True\n        If Ture, then inputs will be non-dimensionalized before integration is performed.\n        Results will be redimensionalized before being returned.\n    verbose : bool, default=False\n        If True, then additioal information will be printed to the terminal during the solution. \n    warnings : bool, default=True\n        If True, then warnings will be printed to the terminal during the solution. \n    raise_on_fail : bool, default=False\n        If Ture, then the solver will raise an exception if integration was not successful. By default RadialSolver\n        fails silently. \n\n    Returns\n    -------\n    solution : RadialSolverSolution\n        Solution to the viscoelastic-gravitational problem inside a planet.\n        Solution attributes:\n            - solution.results : complex128, shape=(6 * num_ytypes, n_slice)\n                Numerical solution throughout the planet.\n            - solution.success : bool\n                Flag if integration and subsequent collapse occured without error.\n            - solution"".message : str\n                Feedback string useful for debugging.\n    ");
 static PyMethodDef __pyx_mdef_7TidalPy_12RadialSolver_6solver_1radial_solver = {"radial_solver", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7TidalPy_12RadialSolver_6solver_1radial_solver, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7TidalPy_12RadialSolver_6solver_radial_solver};
 static PyObject *__pyx_pw_7TidalPy_12RadialSolver_6solver_1radial_solver(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
@@ -28314,20 +28319,21 @@
   size_t __pyx_v_max_num_steps;
   size_t __pyx_v_expected_size;
   size_t __pyx_v_max_ram_MB;
   double __pyx_v_max_step;
   int __pyx_v_limit_solution_to_radius;
   int __pyx_v_nondimensionalize;
   int __pyx_v_verbose;
+  int __pyx_v_warnings;
   int __pyx_v_raise_on_fail;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[26] = {0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0};
+  PyObject* values[27] = {0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("radial_solver (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
@@ -28335,28 +28341,30 @@
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_radius_array,&__pyx_n_s_density_array,&__pyx_n_s_gravity_array,&__pyx_n_s_bulk_modulus_array,&__pyx_n_s_complex_shear_modulus_array,&__pyx_n_s_frequency,&__pyx_n_s_planet_bulk_density,&__pyx_n_s_layer_types,&__pyx_n_s_is_static_by_layer,&__pyx_n_s_is_incompressible_by_layer,&__pyx_n_s_upper_radius_by_layer,&__pyx_n_s_degree_l,&__pyx_n_s_solve_for,&__pyx_n_s_use_kamata,&__pyx_n_s_integration_method,&__pyx_n_s_integration_rtol,&__pyx_n_s_integration_atol,&__pyx_n_s_scale_rtols_by_layer_type,&__pyx_n_s_max_num_steps,&__pyx_n_s_expected_size,&__pyx_n_s_max_ram_MB,&__pyx_n_s_max_step,&__pyx_n_s_limit_solution_to_radius,&__pyx_n_s_nondimensionalize,&__pyx_n_s_verbose,&__pyx_n_s_raise_on_fail,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_radius_array,&__pyx_n_s_density_array,&__pyx_n_s_gravity_array,&__pyx_n_s_bulk_modulus_array,&__pyx_n_s_complex_shear_modulus_array,&__pyx_n_s_frequency,&__pyx_n_s_planet_bulk_density,&__pyx_n_s_layer_types,&__pyx_n_s_is_static_by_layer,&__pyx_n_s_is_incompressible_by_layer,&__pyx_n_s_upper_radius_by_layer,&__pyx_n_s_degree_l,&__pyx_n_s_solve_for,&__pyx_n_s_use_kamata,&__pyx_n_s_integration_method,&__pyx_n_s_integration_rtol,&__pyx_n_s_integration_atol,&__pyx_n_s_scale_rtols_by_layer_type,&__pyx_n_s_max_num_steps,&__pyx_n_s_expected_size,&__pyx_n_s_max_ram_MB,&__pyx_n_s_max_step,&__pyx_n_s_limit_solution_to_radius,&__pyx_n_s_nondimensionalize,&__pyx_n_s_verbose,&__pyx_n_s_warnings,&__pyx_n_s_raise_on_fail,0};
 
     /* "TidalPy/RadialSolver/solver.pyx":1068
  *         tuple upper_radius_by_layer,
  *         unsigned int degree_l = 2,
  *         tuple solve_for = None,             # <<<<<<<<<<<<<<
  *         bint use_kamata = False,
  *         str integration_method = 'RK45',
  */
     values[12] = __Pyx_Arg_NewRef_FASTCALL(((PyObject*)Py_None));
     values[14] = __Pyx_Arg_NewRef_FASTCALL(((PyObject*)((PyObject*)__pyx_n_u_RK45)));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
+        case 27: values[26] = __Pyx_Arg_FASTCALL(__pyx_args, 26);
+        CYTHON_FALLTHROUGH;
         case 26: values[25] = __Pyx_Arg_FASTCALL(__pyx_args, 25);
         CYTHON_FALLTHROUGH;
         case 25: values[24] = __Pyx_Arg_FASTCALL(__pyx_args, 24);
         CYTHON_FALLTHROUGH;
         case 24: values[23] = __Pyx_Arg_FASTCALL(__pyx_args, 23);
         CYTHON_FALLTHROUGH;
         case 23: values[22] = __Pyx_Arg_FASTCALL(__pyx_args, 22);
@@ -28421,105 +28429,105 @@
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_density_array)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 26, 1); __PYX_ERR(0, 1055, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 27, 1); __PYX_ERR(0, 1055, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_gravity_array)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 26, 2); __PYX_ERR(0, 1055, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 27, 2); __PYX_ERR(0, 1055, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_bulk_modulus_array)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 26, 3); __PYX_ERR(0, 1055, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 27, 3); __PYX_ERR(0, 1055, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_complex_shear_modulus_array)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 26, 4); __PYX_ERR(0, 1055, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 27, 4); __PYX_ERR(0, 1055, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_frequency)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[5]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 26, 5); __PYX_ERR(0, 1055, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 27, 5); __PYX_ERR(0, 1055, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_planet_bulk_density)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[6]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 26, 6); __PYX_ERR(0, 1055, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 27, 6); __PYX_ERR(0, 1055, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_layer_types)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[7]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 26, 7); __PYX_ERR(0, 1055, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 27, 7); __PYX_ERR(0, 1055, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (likely((values[8] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_is_static_by_layer)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[8]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 26, 8); __PYX_ERR(0, 1055, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 27, 8); __PYX_ERR(0, 1055, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (likely((values[9] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_is_incompressible_by_layer)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[9]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 26, 9); __PYX_ERR(0, 1055, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 27, 9); __PYX_ERR(0, 1055, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 10:
         if (likely((values[10] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_upper_radius_by_layer)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[10]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 26, 10); __PYX_ERR(0, 1055, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 27, 10); __PYX_ERR(0, 1055, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 11:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_degree_l);
           if (value) { values[11] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
@@ -28614,25 +28622,34 @@
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_verbose);
           if (value) { values[24] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 25:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_raise_on_fail);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_warnings);
           if (value) { values[25] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
         }
+        CYTHON_FALLTHROUGH;
+        case 26:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_raise_on_fail);
+          if (value) { values[26] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L3_error)
+        }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "radial_solver") < 0)) __PYX_ERR(0, 1055, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
+        case 27: values[26] = __Pyx_Arg_FASTCALL(__pyx_args, 26);
+        CYTHON_FALLTHROUGH;
         case 26: values[25] = __Pyx_Arg_FASTCALL(__pyx_args, 25);
         CYTHON_FALLTHROUGH;
         case 25: values[24] = __Pyx_Arg_FASTCALL(__pyx_args, 24);
         CYTHON_FALLTHROUGH;
         case 24: values[23] = __Pyx_Arg_FASTCALL(__pyx_args, 23);
         CYTHON_FALLTHROUGH;
         case 23: values[22] = __Pyx_Arg_FASTCALL(__pyx_args, 22);
@@ -28766,48 +28783,61 @@
     } else {
 
       /* "TidalPy/RadialSolver/solver.pyx":1079
  *         double max_step = 0,
  *         bint limit_solution_to_radius = True,
  *         bint nondimensionalize = True,             # <<<<<<<<<<<<<<
  *         bint verbose = False,
- *         bint raise_on_fail = False
+ *         bint warnings = True,
  */
       __pyx_v_nondimensionalize = ((int)((int)1));
     }
     if (values[24]) {
       __pyx_v_verbose = __Pyx_PyObject_IsTrue(values[24]); if (unlikely((__pyx_v_verbose == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1080, __pyx_L3_error)
     } else {
 
       /* "TidalPy/RadialSolver/solver.pyx":1080
  *         bint limit_solution_to_radius = True,
  *         bint nondimensionalize = True,
  *         bint verbose = False,             # <<<<<<<<<<<<<<
+ *         bint warnings = True,
  *         bint raise_on_fail = False
- *         ):
  */
       __pyx_v_verbose = ((int)((int)0));
     }
     if (values[25]) {
-      __pyx_v_raise_on_fail = __Pyx_PyObject_IsTrue(values[25]); if (unlikely((__pyx_v_raise_on_fail == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1081, __pyx_L3_error)
+      __pyx_v_warnings = __Pyx_PyObject_IsTrue(values[25]); if (unlikely((__pyx_v_warnings == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1081, __pyx_L3_error)
     } else {
 
       /* "TidalPy/RadialSolver/solver.pyx":1081
  *         bint nondimensionalize = True,
  *         bint verbose = False,
+ *         bint warnings = True,             # <<<<<<<<<<<<<<
+ *         bint raise_on_fail = False
+ *         ):
+ */
+      __pyx_v_warnings = ((int)((int)1));
+    }
+    if (values[26]) {
+      __pyx_v_raise_on_fail = __Pyx_PyObject_IsTrue(values[26]); if (unlikely((__pyx_v_raise_on_fail == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1082, __pyx_L3_error)
+    } else {
+
+      /* "TidalPy/RadialSolver/solver.pyx":1082
+ *         bint verbose = False,
+ *         bint warnings = True,
  *         bint raise_on_fail = False             # <<<<<<<<<<<<<<
  *         ):
  *     """
  */
       __pyx_v_raise_on_fail = ((int)((int)0));
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 26, __pyx_nargs); __PYX_ERR(0, 1055, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("radial_solver", 0, 11, 27, __pyx_nargs); __PYX_ERR(0, 1055, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -28824,15 +28854,15 @@
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_layer_types), (&PyTuple_Type), 1, "layer_types", 1))) __PYX_ERR(0, 1063, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_is_static_by_layer), (&PyTuple_Type), 1, "is_static_by_layer", 1))) __PYX_ERR(0, 1064, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_is_incompressible_by_layer), (&PyTuple_Type), 1, "is_incompressible_by_layer", 1))) __PYX_ERR(0, 1065, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_upper_radius_by_layer), (&PyTuple_Type), 1, "upper_radius_by_layer", 1))) __PYX_ERR(0, 1066, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_solve_for), (&PyTuple_Type), 1, "solve_for", 1))) __PYX_ERR(0, 1068, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_integration_method), (&PyUnicode_Type), 1, "integration_method", 1))) __PYX_ERR(0, 1070, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7TidalPy_12RadialSolver_6solver_radial_solver(__pyx_self, __pyx_v_radius_array, __pyx_v_density_array, __pyx_v_gravity_array, __pyx_v_bulk_modulus_array, __pyx_v_complex_shear_modulus_array, __pyx_v_frequency, __pyx_v_planet_bulk_density, __pyx_v_layer_types, __pyx_v_is_static_by_layer, __pyx_v_is_incompressible_by_layer, __pyx_v_upper_radius_by_layer, __pyx_v_degree_l, __pyx_v_solve_for, __pyx_v_use_kamata, __pyx_v_integration_method, __pyx_v_integration_rtol, __pyx_v_integration_atol, __pyx_v_scale_rtols_by_layer_type, __pyx_v_max_num_steps, __pyx_v_expected_size, __pyx_v_max_ram_MB, __pyx_v_max_step, __pyx_v_limit_solution_to_radius, __pyx_v_nondimensionalize, __pyx_v_verbose, __pyx_v_raise_on_fail);
+  __pyx_r = __pyx_pf_7TidalPy_12RadialSolver_6solver_radial_solver(__pyx_self, __pyx_v_radius_array, __pyx_v_density_array, __pyx_v_gravity_array, __pyx_v_bulk_modulus_array, __pyx_v_complex_shear_modulus_array, __pyx_v_frequency, __pyx_v_planet_bulk_density, __pyx_v_layer_types, __pyx_v_is_static_by_layer, __pyx_v_is_incompressible_by_layer, __pyx_v_upper_radius_by_layer, __pyx_v_degree_l, __pyx_v_solve_for, __pyx_v_use_kamata, __pyx_v_integration_method, __pyx_v_integration_rtol, __pyx_v_integration_atol, __pyx_v_scale_rtols_by_layer_type, __pyx_v_max_num_steps, __pyx_v_expected_size, __pyx_v_max_ram_MB, __pyx_v_max_step, __pyx_v_limit_solution_to_radius, __pyx_v_nondimensionalize, __pyx_v_verbose, __pyx_v_warnings, __pyx_v_raise_on_fail);
 
   /* "TidalPy/RadialSolver/solver.pyx":1055
  * 
  * 
  * def radial_solver(             # <<<<<<<<<<<<<<
  *         double[::1] radius_array,
  *         double[::1] density_array,
@@ -28854,15 +28884,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7TidalPy_12RadialSolver_6solver_radial_solver(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_radius_array, __Pyx_memviewslice __pyx_v_density_array, __Pyx_memviewslice __pyx_v_gravity_array, __Pyx_memviewslice __pyx_v_bulk_modulus_array, __Pyx_memviewslice __pyx_v_complex_shear_modulus_array, double __pyx_v_frequency, double __pyx_v_planet_bulk_density, PyObject *__pyx_v_layer_types, PyObject *__pyx_v_is_static_by_layer, PyObject *__pyx_v_is_incompressible_by_layer, PyObject *__pyx_v_upper_radius_by_layer, unsigned int __pyx_v_degree_l, PyObject *__pyx_v_solve_for, int __pyx_v_use_kamata, PyObject *__pyx_v_integration_method, double __pyx_v_integration_rtol, double __pyx_v_integration_atol, int __pyx_v_scale_rtols_by_layer_type, size_t __pyx_v_max_num_steps, size_t __pyx_v_expected_size, size_t __pyx_v_max_ram_MB, double __pyx_v_max_step, int __pyx_v_limit_solution_to_radius, int __pyx_v_nondimensionalize, int __pyx_v_verbose, int __pyx_v_raise_on_fail) {
+static PyObject *__pyx_pf_7TidalPy_12RadialSolver_6solver_radial_solver(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_radius_array, __Pyx_memviewslice __pyx_v_density_array, __Pyx_memviewslice __pyx_v_gravity_array, __Pyx_memviewslice __pyx_v_bulk_modulus_array, __Pyx_memviewslice __pyx_v_complex_shear_modulus_array, double __pyx_v_frequency, double __pyx_v_planet_bulk_density, PyObject *__pyx_v_layer_types, PyObject *__pyx_v_is_static_by_layer, PyObject *__pyx_v_is_incompressible_by_layer, PyObject *__pyx_v_upper_radius_by_layer, unsigned int __pyx_v_degree_l, PyObject *__pyx_v_solve_for, int __pyx_v_use_kamata, PyObject *__pyx_v_integration_method, double __pyx_v_integration_rtol, double __pyx_v_integration_atol, int __pyx_v_scale_rtols_by_layer_type, size_t __pyx_v_max_num_steps, size_t __pyx_v_expected_size, size_t __pyx_v_max_ram_MB, double __pyx_v_max_step, int __pyx_v_limit_solution_to_radius, int __pyx_v_nondimensionalize, int __pyx_v_verbose, int __pyx_v_warnings, int __pyx_v_raise_on_fail) {
   size_t __pyx_v_i;
   size_t __pyx_v_total_slices;
   size_t __pyx_v_num_layers;
   int *__pyx_v_layer_assumptions_ptr;
   int *__pyx_v_layer_types_ptr;
   int *__pyx_v_is_static_by_layer_ptr;
   int *__pyx_v_is_incompressible_by_layer_ptr;
@@ -28903,616 +28933,616 @@
   PyObject *__pyx_t_27 = NULL;
   PyObject *__pyx_t_28 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("radial_solver", 1);
 
-  /* "TidalPy/RadialSolver/solver.pyx":1186
+  /* "TidalPy/RadialSolver/solver.pyx":1189
  *     # Perform checks and make conversions from python to c
  *     cdef size_t total_slices
  *     total_slices = radius_array.size             # <<<<<<<<<<<<<<
  *     assert density_array.size               == total_slices
  *     assert gravity_array.size               == total_slices
  */
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_radius_array, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1186, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_radius_array, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1186, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1186, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_size_t(__pyx_t_2); if (unlikely((__pyx_t_3 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 1189, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_total_slices = __pyx_t_3;
 
-  /* "TidalPy/RadialSolver/solver.pyx":1187
+  /* "TidalPy/RadialSolver/solver.pyx":1190
  *     cdef size_t total_slices
  *     total_slices = radius_array.size
  *     assert density_array.size               == total_slices             # <<<<<<<<<<<<<<
  *     assert gravity_array.size               == total_slices
  *     assert bulk_modulus_array.size          == total_slices
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
-    __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_density_array, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1187, __pyx_L1_error)
+    __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_density_array, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1187, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_total_slices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1187, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_total_slices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1187, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1190, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1187, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1190, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_5)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 1187, __pyx_L1_error)
+      __PYX_ERR(0, 1190, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 1187, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 1190, __pyx_L1_error)
   #endif
 
-  /* "TidalPy/RadialSolver/solver.pyx":1188
+  /* "TidalPy/RadialSolver/solver.pyx":1191
  *     total_slices = radius_array.size
  *     assert density_array.size               == total_slices
  *     assert gravity_array.size               == total_slices             # <<<<<<<<<<<<<<
  *     assert bulk_modulus_array.size          == total_slices
  *     assert complex_shear_modulus_array.size == total_slices
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
-    __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_gravity_array, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1188, __pyx_L1_error)
+    __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_gravity_array, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1188, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_total_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1188, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_FromSize_t(__pyx_v_total_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1188, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1191, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1188, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1191, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!__pyx_t_5)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 1188, __pyx_L1_error)
+      __PYX_ERR(0, 1191, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 1188, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 1191, __pyx_L1_error)
   #endif
 
-  /* "TidalPy/RadialSolver/solver.pyx":1189
+  /* "TidalPy/RadialSolver/solver.pyx":1192
  *     assert density_array.size               == total_slices
  *     assert gravity_array.size               == total_slices
  *     assert bulk_modulus_array.size          == total_slices             # <<<<<<<<<<<<<<
  *     assert complex_shear_modulus_array.size == total_slices
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
-    __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_bulk_modulus_array, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1189, __pyx_L1_error)
+    __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_bulk_modulus_array, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1189, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_total_slices); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1189, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_total_slices); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyObject_RichCompare(__pyx_t_4, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1189, __pyx_L1_error)
+    __pyx_t_2 = PyObject_RichCompare(__pyx_t_4, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1192, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1189, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1192, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(!__pyx_t_5)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 1189, __pyx_L1_error)
+      __PYX_ERR(0, 1192, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 1189, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 1192, __pyx_L1_error)
   #endif
 
-  /* "TidalPy/RadialSolver/solver.pyx":1190
+  /* "TidalPy/RadialSolver/solver.pyx":1193
  *     assert gravity_array.size               == total_slices
  *     assert bulk_modulus_array.size          == total_slices
  *     assert complex_shear_modulus_array.size == total_slices             # <<<<<<<<<<<<<<
  * 
  *     # Unpack inefficient user-provided tuples into bool arrays and pass by pointer
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
-    __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_complex_shear_modulus_array, 1, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1190, __pyx_L1_error)
+    __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_complex_shear_modulus_array, 1, (PyObject *(*)(char *)) __pyx_memview_get___pyx_t_double_complex, (int (*)(char *, PyObject *)) __pyx_memview_set___pyx_t_double_complex, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1190, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_total_slices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1190, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_total_slices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1190, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1193, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1190, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1193, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_5)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 1190, __pyx_L1_error)
+      __PYX_ERR(0, 1193, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 1190, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 1193, __pyx_L1_error)
   #endif
 
-  /* "TidalPy/RadialSolver/solver.pyx":1194
+  /* "TidalPy/RadialSolver/solver.pyx":1197
  *     # Unpack inefficient user-provided tuples into bool arrays and pass by pointer
  *     cdef size_t num_layers
  *     num_layers = len(layer_types)             # <<<<<<<<<<<<<<
  * 
  *     # Check that number of assumptions match.
  */
   if (unlikely(__pyx_v_layer_types == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 1194, __pyx_L1_error)
+    __PYX_ERR(0, 1197, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyTuple_GET_SIZE(__pyx_v_layer_types); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1194, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyTuple_GET_SIZE(__pyx_v_layer_types); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1197, __pyx_L1_error)
   __pyx_v_num_layers = __pyx_t_6;
 
-  /* "TidalPy/RadialSolver/solver.pyx":1197
+  /* "TidalPy/RadialSolver/solver.pyx":1200
  * 
  *     # Check that number of assumptions match.
  *     if len(is_static_by_layer) != num_layers:             # <<<<<<<<<<<<<<
  *         raise AttributeError('Number of `is_static_by_layer` must match number of `layer_types`.')
  *     if len(is_incompressible_by_layer) != num_layers:
  */
   if (unlikely(__pyx_v_is_static_by_layer == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 1197, __pyx_L1_error)
+    __PYX_ERR(0, 1200, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyTuple_GET_SIZE(__pyx_v_is_static_by_layer); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1197, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyTuple_GET_SIZE(__pyx_v_is_static_by_layer); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1200, __pyx_L1_error)
   __pyx_t_5 = (__pyx_t_6 != __pyx_v_num_layers);
   if (unlikely(__pyx_t_5)) {
 
-    /* "TidalPy/RadialSolver/solver.pyx":1198
+    /* "TidalPy/RadialSolver/solver.pyx":1201
  *     # Check that number of assumptions match.
  *     if len(is_static_by_layer) != num_layers:
  *         raise AttributeError('Number of `is_static_by_layer` must match number of `layer_types`.')             # <<<<<<<<<<<<<<
  *     if len(is_incompressible_by_layer) != num_layers:
  *         raise AttributeError('Number of `is_incompressible_by_layer` must match number of `layer_types`.')
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_AttributeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1198, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_AttributeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 1198, __pyx_L1_error)
+    __PYX_ERR(0, 1201, __pyx_L1_error)
 
-    /* "TidalPy/RadialSolver/solver.pyx":1197
+    /* "TidalPy/RadialSolver/solver.pyx":1200
  * 
  *     # Check that number of assumptions match.
  *     if len(is_static_by_layer) != num_layers:             # <<<<<<<<<<<<<<
  *         raise AttributeError('Number of `is_static_by_layer` must match number of `layer_types`.')
  *     if len(is_incompressible_by_layer) != num_layers:
  */
   }
 
-  /* "TidalPy/RadialSolver/solver.pyx":1199
+  /* "TidalPy/RadialSolver/solver.pyx":1202
  *     if len(is_static_by_layer) != num_layers:
  *         raise AttributeError('Number of `is_static_by_layer` must match number of `layer_types`.')
  *     if len(is_incompressible_by_layer) != num_layers:             # <<<<<<<<<<<<<<
  *         raise AttributeError('Number of `is_incompressible_by_layer` must match number of `layer_types`.')
  *     if len(upper_radius_by_layer) != num_layers:
  */
   if (unlikely(__pyx_v_is_incompressible_by_layer == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 1199, __pyx_L1_error)
+    __PYX_ERR(0, 1202, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyTuple_GET_SIZE(__pyx_v_is_incompressible_by_layer); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1199, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyTuple_GET_SIZE(__pyx_v_is_incompressible_by_layer); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1202, __pyx_L1_error)
   __pyx_t_5 = (__pyx_t_6 != __pyx_v_num_layers);
   if (unlikely(__pyx_t_5)) {
 
-    /* "TidalPy/RadialSolver/solver.pyx":1200
+    /* "TidalPy/RadialSolver/solver.pyx":1203
  *         raise AttributeError('Number of `is_static_by_layer` must match number of `layer_types`.')
  *     if len(is_incompressible_by_layer) != num_layers:
  *         raise AttributeError('Number of `is_incompressible_by_layer` must match number of `layer_types`.')             # <<<<<<<<<<<<<<
  *     if len(upper_radius_by_layer) != num_layers:
  *         raise AttributeError('Number of `upper_radius_by_layer` must match number of `layer_types`.')
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_AttributeError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1200, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_AttributeError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1203, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 1200, __pyx_L1_error)
+    __PYX_ERR(0, 1203, __pyx_L1_error)
 
-    /* "TidalPy/RadialSolver/solver.pyx":1199
+    /* "TidalPy/RadialSolver/solver.pyx":1202
  *     if len(is_static_by_layer) != num_layers:
  *         raise AttributeError('Number of `is_static_by_layer` must match number of `layer_types`.')
  *     if len(is_incompressible_by_layer) != num_layers:             # <<<<<<<<<<<<<<
  *         raise AttributeError('Number of `is_incompressible_by_layer` must match number of `layer_types`.')
  *     if len(upper_radius_by_layer) != num_layers:
  */
   }
 
-  /* "TidalPy/RadialSolver/solver.pyx":1201
+  /* "TidalPy/RadialSolver/solver.pyx":1204
  *     if len(is_incompressible_by_layer) != num_layers:
  *         raise AttributeError('Number of `is_incompressible_by_layer` must match number of `layer_types`.')
  *     if len(upper_radius_by_layer) != num_layers:             # <<<<<<<<<<<<<<
  *         raise AttributeError('Number of `upper_radius_by_layer` must match number of `layer_types`.')
  * 
  */
   if (unlikely(__pyx_v_upper_radius_by_layer == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 1201, __pyx_L1_error)
+    __PYX_ERR(0, 1204, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyTuple_GET_SIZE(__pyx_v_upper_radius_by_layer); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1201, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyTuple_GET_SIZE(__pyx_v_upper_radius_by_layer); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1204, __pyx_L1_error)
   __pyx_t_5 = (__pyx_t_6 != __pyx_v_num_layers);
   if (unlikely(__pyx_t_5)) {
 
-    /* "TidalPy/RadialSolver/solver.pyx":1202
+    /* "TidalPy/RadialSolver/solver.pyx":1205
  *         raise AttributeError('Number of `is_incompressible_by_layer` must match number of `layer_types`.')
  *     if len(upper_radius_by_layer) != num_layers:
  *         raise AttributeError('Number of `upper_radius_by_layer` must match number of `layer_types`.')             # <<<<<<<<<<<<<<
  * 
  *     # Check that other inputs make sense
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_AttributeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1202, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_AttributeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 1202, __pyx_L1_error)
+    __PYX_ERR(0, 1205, __pyx_L1_error)
 
-    /* "TidalPy/RadialSolver/solver.pyx":1201
+    /* "TidalPy/RadialSolver/solver.pyx":1204
  *     if len(is_incompressible_by_layer) != num_layers:
  *         raise AttributeError('Number of `is_incompressible_by_layer` must match number of `layer_types`.')
  *     if len(upper_radius_by_layer) != num_layers:             # <<<<<<<<<<<<<<
  *         raise AttributeError('Number of `upper_radius_by_layer` must match number of `layer_types`.')
  * 
  */
   }
 
-  /* "TidalPy/RadialSolver/solver.pyx":1205
+  /* "TidalPy/RadialSolver/solver.pyx":1208
  * 
  *     # Check that other inputs make sense
  *     if solve_for is not None:             # <<<<<<<<<<<<<<
  *         if type(solve_for) != tuple:
  *             raise AttributeError(
  */
   __pyx_t_5 = (__pyx_v_solve_for != ((PyObject*)Py_None));
   if (__pyx_t_5) {
 
-    /* "TidalPy/RadialSolver/solver.pyx":1206
+    /* "TidalPy/RadialSolver/solver.pyx":1209
  *     # Check that other inputs make sense
  *     if solve_for is not None:
  *         if type(solve_for) != tuple:             # <<<<<<<<<<<<<<
  *             raise AttributeError(
  *                 '`solve_for` argument must be a tuple of strings. For example:\n'
  */
-    __pyx_t_4 = PyObject_RichCompare(((PyObject *)Py_TYPE(__pyx_v_solve_for)), ((PyObject *)(&PyTuple_Type)), Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1206, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1206, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(((PyObject *)Py_TYPE(__pyx_v_solve_for)), ((PyObject *)(&PyTuple_Type)), Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1209, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1209, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(__pyx_t_5)) {
 
-      /* "TidalPy/RadialSolver/solver.pyx":1207
+      /* "TidalPy/RadialSolver/solver.pyx":1210
  *     if solve_for is not None:
  *         if type(solve_for) != tuple:
  *             raise AttributeError(             # <<<<<<<<<<<<<<
  *                 '`solve_for` argument must be a tuple of strings. For example:\n'
  *                 '   ("tidal",)  # If you just want tidal Love numbers.\n'
  */
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_AttributeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1207, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_AttributeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1210, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 1207, __pyx_L1_error)
+      __PYX_ERR(0, 1210, __pyx_L1_error)
 
-      /* "TidalPy/RadialSolver/solver.pyx":1206
+      /* "TidalPy/RadialSolver/solver.pyx":1209
  *     # Check that other inputs make sense
  *     if solve_for is not None:
  *         if type(solve_for) != tuple:             # <<<<<<<<<<<<<<
  *             raise AttributeError(
  *                 '`solve_for` argument must be a tuple of strings. For example:\n'
  */
     }
 
-    /* "TidalPy/RadialSolver/solver.pyx":1205
+    /* "TidalPy/RadialSolver/solver.pyx":1208
  * 
  *     # Check that other inputs make sense
  *     if solve_for is not None:             # <<<<<<<<<<<<<<
  *         if type(solve_for) != tuple:
  *             raise AttributeError(
  */
   }
 
-  /* "TidalPy/RadialSolver/solver.pyx":1215
+  /* "TidalPy/RadialSolver/solver.pyx":1218
  *     # Build array of assumptions
  *     # OPT: Perhaps set a maximum number of layers then we can put these on the stack rather than heap allocating them.
  *     cdef int* layer_assumptions_ptr = <int *> allocate_mem(             # <<<<<<<<<<<<<<
  *         3 * num_layers * sizeof(int),
  *         'layer_assumptions_ptr (radial_solver; init)'
  */
-  __pyx_t_7 = __pyx_f_4CyRK_5utils_5utils_allocate_mem(((3 * __pyx_v_num_layers) * (sizeof(int))), ((char *)"layer_assumptions_ptr (radial_solver; init)")); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1215, __pyx_L1_error)
+  __pyx_t_7 = __pyx_f_4CyRK_5utils_5utils_allocate_mem(((3 * __pyx_v_num_layers) * (sizeof(int))), ((char *)"layer_assumptions_ptr (radial_solver; init)")); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1218, __pyx_L1_error)
   __pyx_v_layer_assumptions_ptr = ((int *)__pyx_t_7);
 
-  /* "TidalPy/RadialSolver/solver.pyx":1219
+  /* "TidalPy/RadialSolver/solver.pyx":1222
  *         'layer_assumptions_ptr (radial_solver; init)'
  *         )
  *     cdef int* layer_types_ptr                = &layer_assumptions_ptr[0]             # <<<<<<<<<<<<<<
  *     cdef int* is_static_by_layer_ptr         = &layer_assumptions_ptr[num_layers]
  *     cdef int* is_incompressible_by_layer_ptr = &layer_assumptions_ptr[2 * num_layers]
  */
   __pyx_v_layer_types_ptr = (&(__pyx_v_layer_assumptions_ptr[0]));
 
-  /* "TidalPy/RadialSolver/solver.pyx":1220
+  /* "TidalPy/RadialSolver/solver.pyx":1223
  *         )
  *     cdef int* layer_types_ptr                = &layer_assumptions_ptr[0]
  *     cdef int* is_static_by_layer_ptr         = &layer_assumptions_ptr[num_layers]             # <<<<<<<<<<<<<<
  *     cdef int* is_incompressible_by_layer_ptr = &layer_assumptions_ptr[2 * num_layers]
  *     cdef double* upper_radius_by_layer_ptr = <double *> allocate_mem(
  */
   __pyx_v_is_static_by_layer_ptr = (&(__pyx_v_layer_assumptions_ptr[__pyx_v_num_layers]));
 
-  /* "TidalPy/RadialSolver/solver.pyx":1221
+  /* "TidalPy/RadialSolver/solver.pyx":1224
  *     cdef int* layer_types_ptr                = &layer_assumptions_ptr[0]
  *     cdef int* is_static_by_layer_ptr         = &layer_assumptions_ptr[num_layers]
  *     cdef int* is_incompressible_by_layer_ptr = &layer_assumptions_ptr[2 * num_layers]             # <<<<<<<<<<<<<<
  *     cdef double* upper_radius_by_layer_ptr = <double *> allocate_mem(
  *         num_layers * sizeof(double),
  */
   __pyx_v_is_incompressible_by_layer_ptr = (&(__pyx_v_layer_assumptions_ptr[(2 * __pyx_v_num_layers)]));
 
-  /* "TidalPy/RadialSolver/solver.pyx":1222
+  /* "TidalPy/RadialSolver/solver.pyx":1225
  *     cdef int* is_static_by_layer_ptr         = &layer_assumptions_ptr[num_layers]
  *     cdef int* is_incompressible_by_layer_ptr = &layer_assumptions_ptr[2 * num_layers]
  *     cdef double* upper_radius_by_layer_ptr = <double *> allocate_mem(             # <<<<<<<<<<<<<<
  *         num_layers * sizeof(double),
  *         'upper_radius_by_layer_ptr (radial_solver; init)'
  */
-  __pyx_t_7 = __pyx_f_4CyRK_5utils_5utils_allocate_mem((__pyx_v_num_layers * (sizeof(double))), ((char *)"upper_radius_by_layer_ptr (radial_solver; init)")); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1222, __pyx_L1_error)
+  __pyx_t_7 = __pyx_f_4CyRK_5utils_5utils_allocate_mem((__pyx_v_num_layers * (sizeof(double))), ((char *)"upper_radius_by_layer_ptr (radial_solver; init)")); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1225, __pyx_L1_error)
   __pyx_v_upper_radius_by_layer_ptr = ((double *)__pyx_t_7);
 
-  /* "TidalPy/RadialSolver/solver.pyx":1228
+  /* "TidalPy/RadialSolver/solver.pyx":1231
  * 
  *     cdef str layer_type
  *     cdef bint dynamic_liquid = False             # <<<<<<<<<<<<<<
  * 
  *     # Pull out information for each layer and store in heap memory
  */
   __pyx_v_dynamic_liquid = 0;
 
-  /* "TidalPy/RadialSolver/solver.pyx":1231
+  /* "TidalPy/RadialSolver/solver.pyx":1234
  * 
  *     # Pull out information for each layer and store in heap memory
  *     for i in range(num_layers):             # <<<<<<<<<<<<<<
  *         layer_type                        = layer_types[i]
  *         is_static_by_layer_ptr[i]         = is_static_by_layer[i]
  */
   __pyx_t_3 = __pyx_v_num_layers;
   __pyx_t_8 = __pyx_t_3;
   for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
     __pyx_v_i = __pyx_t_9;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1232
+    /* "TidalPy/RadialSolver/solver.pyx":1235
  *     # Pull out information for each layer and store in heap memory
  *     for i in range(num_layers):
  *         layer_type                        = layer_types[i]             # <<<<<<<<<<<<<<
  *         is_static_by_layer_ptr[i]         = is_static_by_layer[i]
  *         is_incompressible_by_layer_ptr[i] = is_incompressible_by_layer[i]
  */
     if (unlikely(__pyx_v_layer_types == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 1232, __pyx_L1_error)
+      __PYX_ERR(0, 1235, __pyx_L1_error)
     }
-    if (!(likely(PyUnicode_CheckExact(PyTuple_GET_ITEM(__pyx_v_layer_types, __pyx_v_i)))||((PyTuple_GET_ITEM(__pyx_v_layer_types, __pyx_v_i)) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", PyTuple_GET_ITEM(__pyx_v_layer_types, __pyx_v_i)))) __PYX_ERR(0, 1232, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(PyTuple_GET_ITEM(__pyx_v_layer_types, __pyx_v_i)))||((PyTuple_GET_ITEM(__pyx_v_layer_types, __pyx_v_i)) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", PyTuple_GET_ITEM(__pyx_v_layer_types, __pyx_v_i)))) __PYX_ERR(0, 1235, __pyx_L1_error)
     __pyx_t_4 = PyTuple_GET_ITEM(__pyx_v_layer_types, __pyx_v_i);
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_XDECREF_SET(__pyx_v_layer_type, ((PyObject*)__pyx_t_4));
     __pyx_t_4 = 0;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1233
+    /* "TidalPy/RadialSolver/solver.pyx":1236
  *     for i in range(num_layers):
  *         layer_type                        = layer_types[i]
  *         is_static_by_layer_ptr[i]         = is_static_by_layer[i]             # <<<<<<<<<<<<<<
  *         is_incompressible_by_layer_ptr[i] = is_incompressible_by_layer[i]
  *         upper_radius_by_layer_ptr[i]      = upper_radius_by_layer[i]
  */
     if (unlikely(__pyx_v_is_static_by_layer == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 1233, __pyx_L1_error)
+      __PYX_ERR(0, 1236, __pyx_L1_error)
     }
-    __pyx_t_10 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v_is_static_by_layer, __pyx_v_i)); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1233, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v_is_static_by_layer, __pyx_v_i)); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1236, __pyx_L1_error)
     (__pyx_v_is_static_by_layer_ptr[__pyx_v_i]) = __pyx_t_10;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1234
+    /* "TidalPy/RadialSolver/solver.pyx":1237
  *         layer_type                        = layer_types[i]
  *         is_static_by_layer_ptr[i]         = is_static_by_layer[i]
  *         is_incompressible_by_layer_ptr[i] = is_incompressible_by_layer[i]             # <<<<<<<<<<<<<<
  *         upper_radius_by_layer_ptr[i]      = upper_radius_by_layer[i]
  * 
  */
     if (unlikely(__pyx_v_is_incompressible_by_layer == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 1234, __pyx_L1_error)
+      __PYX_ERR(0, 1237, __pyx_L1_error)
     }
-    __pyx_t_10 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v_is_incompressible_by_layer, __pyx_v_i)); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1234, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v_is_incompressible_by_layer, __pyx_v_i)); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1237, __pyx_L1_error)
     (__pyx_v_is_incompressible_by_layer_ptr[__pyx_v_i]) = __pyx_t_10;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1235
+    /* "TidalPy/RadialSolver/solver.pyx":1238
  *         is_static_by_layer_ptr[i]         = is_static_by_layer[i]
  *         is_incompressible_by_layer_ptr[i] = is_incompressible_by_layer[i]
  *         upper_radius_by_layer_ptr[i]      = upper_radius_by_layer[i]             # <<<<<<<<<<<<<<
  * 
  *         if not dynamic_liquid:
  */
     if (unlikely(__pyx_v_upper_radius_by_layer == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 1235, __pyx_L1_error)
+      __PYX_ERR(0, 1238, __pyx_L1_error)
     }
-    __pyx_t_11 = __pyx_PyFloat_AsDouble(PyTuple_GET_ITEM(__pyx_v_upper_radius_by_layer, __pyx_v_i)); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1235, __pyx_L1_error)
+    __pyx_t_11 = __pyx_PyFloat_AsDouble(PyTuple_GET_ITEM(__pyx_v_upper_radius_by_layer, __pyx_v_i)); if (unlikely((__pyx_t_11 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1238, __pyx_L1_error)
     (__pyx_v_upper_radius_by_layer_ptr[__pyx_v_i]) = __pyx_t_11;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1237
+    /* "TidalPy/RadialSolver/solver.pyx":1240
  *         upper_radius_by_layer_ptr[i]      = upper_radius_by_layer[i]
  * 
  *         if not dynamic_liquid:             # <<<<<<<<<<<<<<
- *             if (layer_type != 1) and not is_static_by_layer_ptr[i]:
+ *             if (layer_type == 1) and not is_static_by_layer_ptr[i]:
  *                 # There is at least one dynamic liquid layer
  */
     __pyx_t_5 = (!__pyx_v_dynamic_liquid);
     if (__pyx_t_5) {
 
-      /* "TidalPy/RadialSolver/solver.pyx":1238
+      /* "TidalPy/RadialSolver/solver.pyx":1241
  * 
  *         if not dynamic_liquid:
- *             if (layer_type != 1) and not is_static_by_layer_ptr[i]:             # <<<<<<<<<<<<<<
+ *             if (layer_type == 1) and not is_static_by_layer_ptr[i]:             # <<<<<<<<<<<<<<
  *                 # There is at least one dynamic liquid layer
  *                 dynamic_liquid = True
  */
-      __pyx_t_12 = (__Pyx_PyUnicode_Equals(__pyx_v_layer_type, __pyx_int_1, Py_NE)); if (unlikely((__pyx_t_12 < 0))) __PYX_ERR(0, 1238, __pyx_L1_error)
+      __pyx_t_12 = (__Pyx_PyUnicode_Equals(__pyx_v_layer_type, __pyx_int_1, Py_EQ)); if (unlikely((__pyx_t_12 < 0))) __PYX_ERR(0, 1241, __pyx_L1_error)
       if (__pyx_t_12) {
       } else {
         __pyx_t_5 = __pyx_t_12;
         goto __pyx_L12_bool_binop_done;
       }
       __pyx_t_12 = (!((__pyx_v_is_static_by_layer_ptr[__pyx_v_i]) != 0));
       __pyx_t_5 = __pyx_t_12;
       __pyx_L12_bool_binop_done:;
       if (__pyx_t_5) {
 
-        /* "TidalPy/RadialSolver/solver.pyx":1240
- *             if (layer_type != 1) and not is_static_by_layer_ptr[i]:
+        /* "TidalPy/RadialSolver/solver.pyx":1243
+ *             if (layer_type == 1) and not is_static_by_layer_ptr[i]:
  *                 # There is at least one dynamic liquid layer
  *                 dynamic_liquid = True             # <<<<<<<<<<<<<<
  * 
  *         # Convert user-provided strings to ints for the layer type
  */
         __pyx_v_dynamic_liquid = 1;
 
-        /* "TidalPy/RadialSolver/solver.pyx":1238
+        /* "TidalPy/RadialSolver/solver.pyx":1241
  * 
  *         if not dynamic_liquid:
- *             if (layer_type != 1) and not is_static_by_layer_ptr[i]:             # <<<<<<<<<<<<<<
+ *             if (layer_type == 1) and not is_static_by_layer_ptr[i]:             # <<<<<<<<<<<<<<
  *                 # There is at least one dynamic liquid layer
  *                 dynamic_liquid = True
  */
       }
 
-      /* "TidalPy/RadialSolver/solver.pyx":1237
+      /* "TidalPy/RadialSolver/solver.pyx":1240
  *         upper_radius_by_layer_ptr[i]      = upper_radius_by_layer[i]
  * 
  *         if not dynamic_liquid:             # <<<<<<<<<<<<<<
- *             if (layer_type != 1) and not is_static_by_layer_ptr[i]:
+ *             if (layer_type == 1) and not is_static_by_layer_ptr[i]:
  *                 # There is at least one dynamic liquid layer
  */
     }
 
-    /* "TidalPy/RadialSolver/solver.pyx":1243
+    /* "TidalPy/RadialSolver/solver.pyx":1246
  * 
  *         # Convert user-provided strings to ints for the layer type
  *         if layer_type.lower() == 'solid':             # <<<<<<<<<<<<<<
  *             layer_types_ptr[i] = 0
  *         elif layer_type.lower() == 'liquid':
  */
-    __pyx_t_4 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lower, __pyx_v_layer_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1243, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lower, __pyx_v_layer_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_solid, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1243, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_solid, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1246, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_5) {
 
-      /* "TidalPy/RadialSolver/solver.pyx":1244
+      /* "TidalPy/RadialSolver/solver.pyx":1247
  *         # Convert user-provided strings to ints for the layer type
  *         if layer_type.lower() == 'solid':
  *             layer_types_ptr[i] = 0             # <<<<<<<<<<<<<<
  *         elif layer_type.lower() == 'liquid':
  *             layer_types_ptr[i] = 1
  */
       (__pyx_v_layer_types_ptr[__pyx_v_i]) = 0;
 
-      /* "TidalPy/RadialSolver/solver.pyx":1243
+      /* "TidalPy/RadialSolver/solver.pyx":1246
  * 
  *         # Convert user-provided strings to ints for the layer type
  *         if layer_type.lower() == 'solid':             # <<<<<<<<<<<<<<
  *             layer_types_ptr[i] = 0
  *         elif layer_type.lower() == 'liquid':
  */
       goto __pyx_L14;
     }
 
-    /* "TidalPy/RadialSolver/solver.pyx":1245
+    /* "TidalPy/RadialSolver/solver.pyx":1248
  *         if layer_type.lower() == 'solid':
  *             layer_types_ptr[i] = 0
  *         elif layer_type.lower() == 'liquid':             # <<<<<<<<<<<<<<
  *             layer_types_ptr[i] = 1
  *         else:
  */
-    __pyx_t_4 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lower, __pyx_v_layer_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1245, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lower, __pyx_v_layer_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_liquid, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1245, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_liquid, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1248, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (likely(__pyx_t_5)) {
 
-      /* "TidalPy/RadialSolver/solver.pyx":1246
+      /* "TidalPy/RadialSolver/solver.pyx":1249
  *             layer_types_ptr[i] = 0
  *         elif layer_type.lower() == 'liquid':
  *             layer_types_ptr[i] = 1             # <<<<<<<<<<<<<<
  *         else:
  *             layer_types_ptr[i] = -1
  */
       (__pyx_v_layer_types_ptr[__pyx_v_i]) = 1;
 
-      /* "TidalPy/RadialSolver/solver.pyx":1245
+      /* "TidalPy/RadialSolver/solver.pyx":1248
  *         if layer_type.lower() == 'solid':
  *             layer_types_ptr[i] = 0
  *         elif layer_type.lower() == 'liquid':             # <<<<<<<<<<<<<<
  *             layer_types_ptr[i] = 1
  *         else:
  */
       goto __pyx_L14;
     }
 
-    /* "TidalPy/RadialSolver/solver.pyx":1248
+    /* "TidalPy/RadialSolver/solver.pyx":1251
  *             layer_types_ptr[i] = 1
  *         else:
  *             layer_types_ptr[i] = -1             # <<<<<<<<<<<<<<
  *             log.error(f"Layer type {layer_type} is not supported. Currently supported types: 'solid', 'liquid'.")
  *             raise UnknownModelError(f"Layer type {layer_type} is not supported. Currently supported types: 'solid', 'liquid'.")
  */
     /*else*/ {
       (__pyx_v_layer_types_ptr[__pyx_v_i]) = -1;
 
-      /* "TidalPy/RadialSolver/solver.pyx":1249
+      /* "TidalPy/RadialSolver/solver.pyx":1252
  *         else:
  *             layer_types_ptr[i] = -1
  *             log.error(f"Layer type {layer_type} is not supported. Currently supported types: 'solid', 'liquid'.")             # <<<<<<<<<<<<<<
  *             raise UnknownModelError(f"Layer type {layer_type} is not supported. Currently supported types: 'solid', 'liquid'.")
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1249, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1249, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1249, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_6 = 0;
       __pyx_t_13 = 127;
       __Pyx_INCREF(__pyx_kp_u_Layer_type);
       __pyx_t_6 += 11;
       __Pyx_GIVEREF(__pyx_kp_u_Layer_type);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u_Layer_type);
-      __pyx_t_14 = __Pyx_PyUnicode_Unicode(__pyx_v_layer_type); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1249, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyUnicode_Unicode(__pyx_v_layer_type); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __pyx_t_13 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_14) > __pyx_t_13) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_14) : __pyx_t_13;
       __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_14);
       __Pyx_GIVEREF(__pyx_t_14);
       PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_14);
       __pyx_t_14 = 0;
       __Pyx_INCREF(__pyx_kp_u_is_not_supported_Currently_supp);
       __pyx_t_6 += 64;
       __Pyx_GIVEREF(__pyx_kp_u_is_not_supported_Currently_supp);
       PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u_is_not_supported_Currently_supp);
-      __pyx_t_14 = __Pyx_PyUnicode_Join(__pyx_t_2, 3, __pyx_t_6, __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1249, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyUnicode_Join(__pyx_t_2, 3, __pyx_t_6, __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1252, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       __pyx_t_10 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
@@ -29526,49 +29556,49 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_14};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1249, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1252, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "TidalPy/RadialSolver/solver.pyx":1250
+      /* "TidalPy/RadialSolver/solver.pyx":1253
  *             layer_types_ptr[i] = -1
  *             log.error(f"Layer type {layer_type} is not supported. Currently supported types: 'solid', 'liquid'.")
  *             raise UnknownModelError(f"Layer type {layer_type} is not supported. Currently supported types: 'solid', 'liquid'.")             # <<<<<<<<<<<<<<
  * 
  *     # Check for dynamic liquid layer stability
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UnknownModelError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1250, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UnknownModelError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1253, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_14 = PyTuple_New(3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1250, __pyx_L1_error)
+      __pyx_t_14 = PyTuple_New(3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1253, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __pyx_t_6 = 0;
       __pyx_t_13 = 127;
       __Pyx_INCREF(__pyx_kp_u_Layer_type);
       __pyx_t_6 += 11;
       __Pyx_GIVEREF(__pyx_kp_u_Layer_type);
       PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_kp_u_Layer_type);
-      __pyx_t_2 = __Pyx_PyUnicode_Unicode(__pyx_v_layer_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1250, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyUnicode_Unicode(__pyx_v_layer_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1253, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_13 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_13) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_13;
       __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_2);
       __pyx_t_2 = 0;
       __Pyx_INCREF(__pyx_kp_u_is_not_supported_Currently_supp);
       __pyx_t_6 += 64;
       __Pyx_GIVEREF(__pyx_kp_u_is_not_supported_Currently_supp);
       PyTuple_SET_ITEM(__pyx_t_14, 2, __pyx_kp_u_is_not_supported_Currently_supp);
-      __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_14, 3, __pyx_t_6, __pyx_t_13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1250, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_14, 3, __pyx_t_6, __pyx_t_13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1253, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       __pyx_t_14 = NULL;
       __pyx_t_10 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_1);
@@ -29582,26 +29612,26 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_14, __pyx_t_2};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1250, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1253, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 1250, __pyx_L1_error)
+      __PYX_ERR(0, 1253, __pyx_L1_error)
     }
     __pyx_L14:;
   }
 
-  /* "TidalPy/RadialSolver/solver.pyx":1253
+  /* "TidalPy/RadialSolver/solver.pyx":1256
  * 
  *     # Check for dynamic liquid layer stability
  *     if dynamic_liquid and fabs(frequency) < 2.5e-5:             # <<<<<<<<<<<<<<
  *         # TODO: check that this frequency is a decent cutoff (based on a 3 day period).
  *         #    Initial work suggests that low density layers do not suffer from the same instability problems.
  */
   if (__pyx_v_dynamic_liquid) {
@@ -29610,192 +29640,210 @@
     goto __pyx_L16_bool_binop_done;
   }
   __pyx_t_12 = (fabs(__pyx_v_frequency) < 2.5e-5);
   __pyx_t_5 = __pyx_t_12;
   __pyx_L16_bool_binop_done:;
   if (__pyx_t_5) {
 
-    /* "TidalPy/RadialSolver/solver.pyx":1258
+    /* "TidalPy/RadialSolver/solver.pyx":1261
  *         # TODO: Add density or combo factor to better indicate when a solution is likely to be unstable?
  *         # See Issue #55
- *         log.warning('Dynamic liquid layer detected in RadialSolver for a small frequency. Results may be unstable. Extra care is advised!')             # <<<<<<<<<<<<<<
- * 
- *     # Convert integration method to int
+ *         if warnings:             # <<<<<<<<<<<<<<
+ *             log.warning(
+ *                 'Dynamic liquid layer detected in RadialSolver for a small frequency.'
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1258, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warning); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1258, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = NULL;
-    __pyx_t_10 = 0;
-    #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_1);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
-        __pyx_t_10 = 1;
+    if (__pyx_v_warnings) {
+
+      /* "TidalPy/RadialSolver/solver.pyx":1262
+ *         # See Issue #55
+ *         if warnings:
+ *             log.warning(             # <<<<<<<<<<<<<<
+ *                 'Dynamic liquid layer detected in RadialSolver for a small frequency.'
+ *                 'Results may be unstable. Extra care is advised!'
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1262, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warning); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1262, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = NULL;
+      __pyx_t_10 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_2))) {
+        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
+        if (likely(__pyx_t_1)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+          __Pyx_INCREF(__pyx_t_1);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_2, function);
+          __pyx_t_10 = 1;
+        }
       }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_kp_u_Dynamic_liquid_layer_detected_in};
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
+        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1262, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      }
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "TidalPy/RadialSolver/solver.pyx":1261
+ *         # TODO: Add density or combo factor to better indicate when a solution is likely to be unstable?
+ *         # See Issue #55
+ *         if warnings:             # <<<<<<<<<<<<<<
+ *             log.warning(
+ *                 'Dynamic liquid layer detected in RadialSolver for a small frequency.'
+ */
     }
-    #endif
-    {
-      PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_kp_u_Dynamic_liquid_layer_detected_in};
-      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
-      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1258, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    }
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1253
+    /* "TidalPy/RadialSolver/solver.pyx":1256
  * 
  *     # Check for dynamic liquid layer stability
  *     if dynamic_liquid and fabs(frequency) < 2.5e-5:             # <<<<<<<<<<<<<<
  *         # TODO: check that this frequency is a decent cutoff (based on a 3 day period).
  *         #    Initial work suggests that low density layers do not suffer from the same instability problems.
  */
   }
 
-  /* "TidalPy/RadialSolver/solver.pyx":1261
+  /* "TidalPy/RadialSolver/solver.pyx":1268
  * 
  *     # Convert integration method to int
  *     cdef str integration_method_lower = integration_method.lower()             # <<<<<<<<<<<<<<
  *     cdef unsigned char integration_method_int
  *     if integration_method_lower == 'rk45':
  */
-  __pyx_t_4 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lower, __pyx_v_integration_method); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1261, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lower, __pyx_v_integration_method); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_4))) __PYX_ERR(0, 1261, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_4))) __PYX_ERR(0, 1268, __pyx_L1_error)
   __pyx_v_integration_method_lower = ((PyObject*)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "TidalPy/RadialSolver/solver.pyx":1263
+  /* "TidalPy/RadialSolver/solver.pyx":1270
  *     cdef str integration_method_lower = integration_method.lower()
  *     cdef unsigned char integration_method_int
  *     if integration_method_lower == 'rk45':             # <<<<<<<<<<<<<<
  *         integration_method_int = 1
  *     elif integration_method_lower == 'rk23':
  */
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_integration_method_lower, __pyx_n_u_rk45, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1263, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_integration_method_lower, __pyx_n_u_rk45, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1270, __pyx_L1_error)
   if (__pyx_t_5) {
 
-    /* "TidalPy/RadialSolver/solver.pyx":1264
+    /* "TidalPy/RadialSolver/solver.pyx":1271
  *     cdef unsigned char integration_method_int
  *     if integration_method_lower == 'rk45':
  *         integration_method_int = 1             # <<<<<<<<<<<<<<
  *     elif integration_method_lower == 'rk23':
  *         integration_method_int = 0
  */
     __pyx_v_integration_method_int = 1;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1263
+    /* "TidalPy/RadialSolver/solver.pyx":1270
  *     cdef str integration_method_lower = integration_method.lower()
  *     cdef unsigned char integration_method_int
  *     if integration_method_lower == 'rk45':             # <<<<<<<<<<<<<<
  *         integration_method_int = 1
  *     elif integration_method_lower == 'rk23':
  */
-    goto __pyx_L18;
+    goto __pyx_L19;
   }
 
-  /* "TidalPy/RadialSolver/solver.pyx":1265
+  /* "TidalPy/RadialSolver/solver.pyx":1272
  *     if integration_method_lower == 'rk45':
  *         integration_method_int = 1
  *     elif integration_method_lower == 'rk23':             # <<<<<<<<<<<<<<
  *         integration_method_int = 0
  *     elif integration_method_lower == 'dop853':
  */
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_integration_method_lower, __pyx_n_u_rk23, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1265, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_integration_method_lower, __pyx_n_u_rk23, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1272, __pyx_L1_error)
   if (__pyx_t_5) {
 
-    /* "TidalPy/RadialSolver/solver.pyx":1266
+    /* "TidalPy/RadialSolver/solver.pyx":1273
  *         integration_method_int = 1
  *     elif integration_method_lower == 'rk23':
  *         integration_method_int = 0             # <<<<<<<<<<<<<<
  *     elif integration_method_lower == 'dop853':
  *         integration_method_int = 2
  */
     __pyx_v_integration_method_int = 0;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1265
+    /* "TidalPy/RadialSolver/solver.pyx":1272
  *     if integration_method_lower == 'rk45':
  *         integration_method_int = 1
  *     elif integration_method_lower == 'rk23':             # <<<<<<<<<<<<<<
  *         integration_method_int = 0
  *     elif integration_method_lower == 'dop853':
  */
-    goto __pyx_L18;
+    goto __pyx_L19;
   }
 
-  /* "TidalPy/RadialSolver/solver.pyx":1267
+  /* "TidalPy/RadialSolver/solver.pyx":1274
  *     elif integration_method_lower == 'rk23':
  *         integration_method_int = 0
  *     elif integration_method_lower == 'dop853':             # <<<<<<<<<<<<<<
  *         integration_method_int = 2
  *     else:
  */
-  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_integration_method_lower, __pyx_n_u_dop853, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1267, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_integration_method_lower, __pyx_n_u_dop853, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 1274, __pyx_L1_error)
   if (likely(__pyx_t_5)) {
 
-    /* "TidalPy/RadialSolver/solver.pyx":1268
+    /* "TidalPy/RadialSolver/solver.pyx":1275
  *         integration_method_int = 0
  *     elif integration_method_lower == 'dop853':
  *         integration_method_int = 2             # <<<<<<<<<<<<<<
  *     else:
  *         log.error(f"Unsupported integration method provided: {integration_method_lower}.")
  */
     __pyx_v_integration_method_int = 2;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1267
+    /* "TidalPy/RadialSolver/solver.pyx":1274
  *     elif integration_method_lower == 'rk23':
  *         integration_method_int = 0
  *     elif integration_method_lower == 'dop853':             # <<<<<<<<<<<<<<
  *         integration_method_int = 2
  *     else:
  */
-    goto __pyx_L18;
+    goto __pyx_L19;
   }
 
-  /* "TidalPy/RadialSolver/solver.pyx":1270
+  /* "TidalPy/RadialSolver/solver.pyx":1277
  *         integration_method_int = 2
  *     else:
  *         log.error(f"Unsupported integration method provided: {integration_method_lower}.")             # <<<<<<<<<<<<<<
  *         raise UnknownModelError(f"Unsupported integration method provided: {integration_method_lower}.")
  * 
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1270, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_log); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1270, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1270, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_6 = 0;
     __pyx_t_13 = 127;
     __Pyx_INCREF(__pyx_kp_u_Unsupported_integration_method_p);
     __pyx_t_6 += 41;
     __Pyx_GIVEREF(__pyx_kp_u_Unsupported_integration_method_p);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u_Unsupported_integration_method_p);
-    __pyx_t_14 = __Pyx_PyUnicode_Unicode(__pyx_v_integration_method_lower); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1270, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyUnicode_Unicode(__pyx_v_integration_method_lower); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_14);
     __pyx_t_13 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_14) > __pyx_t_13) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_14) : __pyx_t_13;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_14);
     __Pyx_GIVEREF(__pyx_t_14);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_14);
     __pyx_t_14 = 0;
     __Pyx_INCREF(__pyx_kp_u__2);
     __pyx_t_6 += 1;
     __Pyx_GIVEREF(__pyx_kp_u__2);
     PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u__2);
-    __pyx_t_14 = __Pyx_PyUnicode_Join(__pyx_t_2, 3, __pyx_t_6, __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1270, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyUnicode_Join(__pyx_t_2, 3, __pyx_t_6, __pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_14);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     __pyx_t_10 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
@@ -29809,49 +29857,49 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_14};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1270, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1277, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1271
+    /* "TidalPy/RadialSolver/solver.pyx":1278
  *     else:
  *         log.error(f"Unsupported integration method provided: {integration_method_lower}.")
  *         raise UnknownModelError(f"Unsupported integration method provided: {integration_method_lower}.")             # <<<<<<<<<<<<<<
  * 
  *     # Prepare to run
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UnknownModelError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1271, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UnknownModelError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1278, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_14 = PyTuple_New(3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1271, __pyx_L1_error)
+    __pyx_t_14 = PyTuple_New(3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1278, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_14);
     __pyx_t_6 = 0;
     __pyx_t_13 = 127;
     __Pyx_INCREF(__pyx_kp_u_Unsupported_integration_method_p);
     __pyx_t_6 += 41;
     __Pyx_GIVEREF(__pyx_kp_u_Unsupported_integration_method_p);
     PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_kp_u_Unsupported_integration_method_p);
-    __pyx_t_2 = __Pyx_PyUnicode_Unicode(__pyx_v_integration_method_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1271, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Unicode(__pyx_v_integration_method_lower); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1278, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_13 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_13) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_13;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_2);
     __pyx_t_2 = 0;
     __Pyx_INCREF(__pyx_kp_u__2);
     __pyx_t_6 += 1;
     __Pyx_GIVEREF(__pyx_kp_u__2);
     PyTuple_SET_ITEM(__pyx_t_14, 2, __pyx_kp_u__2);
-    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_14, 3, __pyx_t_6, __pyx_t_13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1271, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_14, 3, __pyx_t_6, __pyx_t_13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1278, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
     __pyx_t_14 = NULL;
     __pyx_t_10 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_1);
@@ -29865,79 +29913,79 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_14, __pyx_t_2};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
       __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1271, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1278, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 1271, __pyx_L1_error)
+    __PYX_ERR(0, 1278, __pyx_L1_error)
   }
-  __pyx_L18:;
+  __pyx_L19:;
 
-  /* "TidalPy/RadialSolver/solver.pyx":1275
+  /* "TidalPy/RadialSolver/solver.pyx":1282
  *     # Prepare to run
  *     cdef RadialSolverSolution result
  *     try:             # <<<<<<<<<<<<<<
  *         result = cf_radial_solver(
  *             total_slices,
  */
   /*try:*/ {
 
-    /* "TidalPy/RadialSolver/solver.pyx":1278
+    /* "TidalPy/RadialSolver/solver.pyx":1285
  *         result = cf_radial_solver(
  *             total_slices,
  *             &radius_array[0],             # <<<<<<<<<<<<<<
  *             &density_array[0],
  *             &gravity_array[0],
  */
     __pyx_t_15 = 0;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1279
+    /* "TidalPy/RadialSolver/solver.pyx":1286
  *             total_slices,
  *             &radius_array[0],
  *             &density_array[0],             # <<<<<<<<<<<<<<
  *             &gravity_array[0],
  *             &bulk_modulus_array[0],
  */
     __pyx_t_16 = 0;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1280
+    /* "TidalPy/RadialSolver/solver.pyx":1287
  *             &radius_array[0],
  *             &density_array[0],
  *             &gravity_array[0],             # <<<<<<<<<<<<<<
  *             &bulk_modulus_array[0],
  *             &complex_shear_modulus_array[0],
  */
     __pyx_t_17 = 0;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1281
+    /* "TidalPy/RadialSolver/solver.pyx":1288
  *             &density_array[0],
  *             &gravity_array[0],
  *             &bulk_modulus_array[0],             # <<<<<<<<<<<<<<
  *             &complex_shear_modulus_array[0],
  *             frequency,
  */
     __pyx_t_18 = 0;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1282
+    /* "TidalPy/RadialSolver/solver.pyx":1289
  *             &gravity_array[0],
  *             &bulk_modulus_array[0],
  *             &complex_shear_modulus_array[0],             # <<<<<<<<<<<<<<
  *             frequency,
  *             planet_bulk_density,
  */
     __pyx_t_19 = 0;
 
-    /* "TidalPy/RadialSolver/solver.pyx":1276
+    /* "TidalPy/RadialSolver/solver.pyx":1283
  *     cdef RadialSolverSolution result
  *     try:
  *         result = cf_radial_solver(             # <<<<<<<<<<<<<<
  *             total_slices,
  *             &radius_array[0],
  */
     __pyx_t_20.__pyx_n = 15;
@@ -29952,125 +30000,125 @@
     __pyx_t_20.expected_size = __pyx_v_expected_size;
     __pyx_t_20.max_ram_MB = __pyx_v_max_ram_MB;
     __pyx_t_20.max_step = __pyx_v_max_step;
     __pyx_t_20.limit_solution_to_radius = __pyx_v_limit_solution_to_radius;
     __pyx_t_20.nondimensionalize = __pyx_v_nondimensionalize;
     __pyx_t_20.verbose = __pyx_v_verbose;
     __pyx_t_20.raise_on_fail = __pyx_v_raise_on_fail;
-    __pyx_t_4 = ((PyObject *)__pyx_f_7TidalPy_12RadialSolver_6solver_cf_radial_solver(__pyx_v_total_slices, (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_radius_array.data) + __pyx_t_15)) )))), (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_density_array.data) + __pyx_t_16)) )))), (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_gravity_array.data) + __pyx_t_17)) )))), (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_bulk_modulus_array.data) + __pyx_t_18)) )))), (&(*((__pyx_t_double_complex *) ( /* dim=0 */ ((char *) (((__pyx_t_double_complex *) __pyx_v_complex_shear_modulus_array.data) + __pyx_t_19)) )))), __pyx_v_frequency, __pyx_v_planet_bulk_density, __pyx_v_num_layers, __pyx_v_layer_types_ptr, __pyx_v_is_static_by_layer_ptr, __pyx_v_is_incompressible_by_layer_ptr, __pyx_v_upper_radius_by_layer_ptr, &__pyx_t_20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1276, __pyx_L20_error)
+    __pyx_t_4 = ((PyObject *)__pyx_f_7TidalPy_12RadialSolver_6solver_cf_radial_solver(__pyx_v_total_slices, (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_radius_array.data) + __pyx_t_15)) )))), (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_density_array.data) + __pyx_t_16)) )))), (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_gravity_array.data) + __pyx_t_17)) )))), (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_bulk_modulus_array.data) + __pyx_t_18)) )))), (&(*((__pyx_t_double_complex *) ( /* dim=0 */ ((char *) (((__pyx_t_double_complex *) __pyx_v_complex_shear_modulus_array.data) + __pyx_t_19)) )))), __pyx_v_frequency, __pyx_v_planet_bulk_density, __pyx_v_num_layers, __pyx_v_layer_types_ptr, __pyx_v_is_static_by_layer_ptr, __pyx_v_is_incompressible_by_layer_ptr, __pyx_v_upper_radius_by_layer_ptr, &__pyx_t_20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1283, __pyx_L21_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_v_result = ((struct __pyx_obj_7TidalPy_12RadialSolver_6solver_RadialSolverSolution *)__pyx_t_4);
     __pyx_t_4 = 0;
   }
 
-  /* "TidalPy/RadialSolver/solver.pyx":1307
+  /* "TidalPy/RadialSolver/solver.pyx":1314
  *     finally:
  *         # Release heap memory
  *         if not (layer_assumptions_ptr is NULL):             # <<<<<<<<<<<<<<
  *             layer_types_ptr                = NULL
  *             is_static_by_layer_ptr         = NULL
  */
   /*finally:*/ {
     /*normal exit:*/{
       __pyx_t_5 = (__pyx_v_layer_assumptions_ptr != NULL);
       if (__pyx_t_5) {
 
-        /* "TidalPy/RadialSolver/solver.pyx":1308
+        /* "TidalPy/RadialSolver/solver.pyx":1315
  *         # Release heap memory
  *         if not (layer_assumptions_ptr is NULL):
  *             layer_types_ptr                = NULL             # <<<<<<<<<<<<<<
  *             is_static_by_layer_ptr         = NULL
  *             is_incompressible_by_layer_ptr = NULL
  */
         __pyx_v_layer_types_ptr = NULL;
 
-        /* "TidalPy/RadialSolver/solver.pyx":1309
+        /* "TidalPy/RadialSolver/solver.pyx":1316
  *         if not (layer_assumptions_ptr is NULL):
  *             layer_types_ptr                = NULL
  *             is_static_by_layer_ptr         = NULL             # <<<<<<<<<<<<<<
  *             is_incompressible_by_layer_ptr = NULL
  *             PyMem_Free(layer_assumptions_ptr)
  */
         __pyx_v_is_static_by_layer_ptr = NULL;
 
-        /* "TidalPy/RadialSolver/solver.pyx":1310
+        /* "TidalPy/RadialSolver/solver.pyx":1317
  *             layer_types_ptr                = NULL
  *             is_static_by_layer_ptr         = NULL
  *             is_incompressible_by_layer_ptr = NULL             # <<<<<<<<<<<<<<
  *             PyMem_Free(layer_assumptions_ptr)
  *             layer_assumptions_ptr = NULL
  */
         __pyx_v_is_incompressible_by_layer_ptr = NULL;
 
-        /* "TidalPy/RadialSolver/solver.pyx":1311
+        /* "TidalPy/RadialSolver/solver.pyx":1318
  *             is_static_by_layer_ptr         = NULL
  *             is_incompressible_by_layer_ptr = NULL
  *             PyMem_Free(layer_assumptions_ptr)             # <<<<<<<<<<<<<<
  *             layer_assumptions_ptr = NULL
  *         if not (upper_radius_by_layer_ptr is NULL):
  */
         PyMem_Free(__pyx_v_layer_assumptions_ptr);
 
-        /* "TidalPy/RadialSolver/solver.pyx":1312
+        /* "TidalPy/RadialSolver/solver.pyx":1319
  *             is_incompressible_by_layer_ptr = NULL
  *             PyMem_Free(layer_assumptions_ptr)
  *             layer_assumptions_ptr = NULL             # <<<<<<<<<<<<<<
  *         if not (upper_radius_by_layer_ptr is NULL):
  *             PyMem_Free(upper_radius_by_layer_ptr)
  */
         __pyx_v_layer_assumptions_ptr = NULL;
 
-        /* "TidalPy/RadialSolver/solver.pyx":1307
+        /* "TidalPy/RadialSolver/solver.pyx":1314
  *     finally:
  *         # Release heap memory
  *         if not (layer_assumptions_ptr is NULL):             # <<<<<<<<<<<<<<
  *             layer_types_ptr                = NULL
  *             is_static_by_layer_ptr         = NULL
  */
       }
 
-      /* "TidalPy/RadialSolver/solver.pyx":1313
+      /* "TidalPy/RadialSolver/solver.pyx":1320
  *             PyMem_Free(layer_assumptions_ptr)
  *             layer_assumptions_ptr = NULL
  *         if not (upper_radius_by_layer_ptr is NULL):             # <<<<<<<<<<<<<<
  *             PyMem_Free(upper_radius_by_layer_ptr)
  *             upper_radius_by_layer_ptr = NULL
  */
       __pyx_t_5 = (__pyx_v_upper_radius_by_layer_ptr != NULL);
       if (__pyx_t_5) {
 
-        /* "TidalPy/RadialSolver/solver.pyx":1314
+        /* "TidalPy/RadialSolver/solver.pyx":1321
  *             layer_assumptions_ptr = NULL
  *         if not (upper_radius_by_layer_ptr is NULL):
  *             PyMem_Free(upper_radius_by_layer_ptr)             # <<<<<<<<<<<<<<
  *             upper_radius_by_layer_ptr = NULL
  * 
  */
         PyMem_Free(__pyx_v_upper_radius_by_layer_ptr);
 
-        /* "TidalPy/RadialSolver/solver.pyx":1315
+        /* "TidalPy/RadialSolver/solver.pyx":1322
  *         if not (upper_radius_by_layer_ptr is NULL):
  *             PyMem_Free(upper_radius_by_layer_ptr)
  *             upper_radius_by_layer_ptr = NULL             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
         __pyx_v_upper_radius_by_layer_ptr = NULL;
 
-        /* "TidalPy/RadialSolver/solver.pyx":1313
+        /* "TidalPy/RadialSolver/solver.pyx":1320
  *             PyMem_Free(layer_assumptions_ptr)
  *             layer_assumptions_ptr = NULL
  *         if not (upper_radius_by_layer_ptr is NULL):             # <<<<<<<<<<<<<<
  *             PyMem_Free(upper_radius_by_layer_ptr)
  *             upper_radius_by_layer_ptr = NULL
  */
       }
-      goto __pyx_L21;
+      goto __pyx_L22;
     }
-    __pyx_L20_error:;
+    __pyx_L21_error:;
     /*exception exit:*/{
       __Pyx_PyThreadState_declare
       __Pyx_PyThreadState_assign
       __pyx_t_23 = 0; __pyx_t_24 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0; __pyx_t_27 = 0; __pyx_t_28 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -30082,107 +30130,107 @@
       __Pyx_XGOTREF(__pyx_t_25);
       __Pyx_XGOTREF(__pyx_t_26);
       __Pyx_XGOTREF(__pyx_t_27);
       __Pyx_XGOTREF(__pyx_t_28);
       __pyx_t_10 = __pyx_lineno; __pyx_t_21 = __pyx_clineno; __pyx_t_22 = __pyx_filename;
       {
 
-        /* "TidalPy/RadialSolver/solver.pyx":1307
+        /* "TidalPy/RadialSolver/solver.pyx":1314
  *     finally:
  *         # Release heap memory
  *         if not (layer_assumptions_ptr is NULL):             # <<<<<<<<<<<<<<
  *             layer_types_ptr                = NULL
  *             is_static_by_layer_ptr         = NULL
  */
         __pyx_t_5 = (__pyx_v_layer_assumptions_ptr != NULL);
         if (__pyx_t_5) {
 
-          /* "TidalPy/RadialSolver/solver.pyx":1308
+          /* "TidalPy/RadialSolver/solver.pyx":1315
  *         # Release heap memory
  *         if not (layer_assumptions_ptr is NULL):
  *             layer_types_ptr                = NULL             # <<<<<<<<<<<<<<
  *             is_static_by_layer_ptr         = NULL
  *             is_incompressible_by_layer_ptr = NULL
  */
           __pyx_v_layer_types_ptr = NULL;
 
-          /* "TidalPy/RadialSolver/solver.pyx":1309
+          /* "TidalPy/RadialSolver/solver.pyx":1316
  *         if not (layer_assumptions_ptr is NULL):
  *             layer_types_ptr                = NULL
  *             is_static_by_layer_ptr         = NULL             # <<<<<<<<<<<<<<
  *             is_incompressible_by_layer_ptr = NULL
  *             PyMem_Free(layer_assumptions_ptr)
  */
           __pyx_v_is_static_by_layer_ptr = NULL;
 
-          /* "TidalPy/RadialSolver/solver.pyx":1310
+          /* "TidalPy/RadialSolver/solver.pyx":1317
  *             layer_types_ptr                = NULL
  *             is_static_by_layer_ptr         = NULL
  *             is_incompressible_by_layer_ptr = NULL             # <<<<<<<<<<<<<<
  *             PyMem_Free(layer_assumptions_ptr)
  *             layer_assumptions_ptr = NULL
  */
           __pyx_v_is_incompressible_by_layer_ptr = NULL;
 
-          /* "TidalPy/RadialSolver/solver.pyx":1311
+          /* "TidalPy/RadialSolver/solver.pyx":1318
  *             is_static_by_layer_ptr         = NULL
  *             is_incompressible_by_layer_ptr = NULL
  *             PyMem_Free(layer_assumptions_ptr)             # <<<<<<<<<<<<<<
  *             layer_assumptions_ptr = NULL
  *         if not (upper_radius_by_layer_ptr is NULL):
  */
           PyMem_Free(__pyx_v_layer_assumptions_ptr);
 
-          /* "TidalPy/RadialSolver/solver.pyx":1312
+          /* "TidalPy/RadialSolver/solver.pyx":1319
  *             is_incompressible_by_layer_ptr = NULL
  *             PyMem_Free(layer_assumptions_ptr)
  *             layer_assumptions_ptr = NULL             # <<<<<<<<<<<<<<
  *         if not (upper_radius_by_layer_ptr is NULL):
  *             PyMem_Free(upper_radius_by_layer_ptr)
  */
           __pyx_v_layer_assumptions_ptr = NULL;
 
-          /* "TidalPy/RadialSolver/solver.pyx":1307
+          /* "TidalPy/RadialSolver/solver.pyx":1314
  *     finally:
  *         # Release heap memory
  *         if not (layer_assumptions_ptr is NULL):             # <<<<<<<<<<<<<<
  *             layer_types_ptr                = NULL
  *             is_static_by_layer_ptr         = NULL
  */
         }
 
-        /* "TidalPy/RadialSolver/solver.pyx":1313
+        /* "TidalPy/RadialSolver/solver.pyx":1320
  *             PyMem_Free(layer_assumptions_ptr)
  *             layer_assumptions_ptr = NULL
  *         if not (upper_radius_by_layer_ptr is NULL):             # <<<<<<<<<<<<<<
  *             PyMem_Free(upper_radius_by_layer_ptr)
  *             upper_radius_by_layer_ptr = NULL
  */
         __pyx_t_5 = (__pyx_v_upper_radius_by_layer_ptr != NULL);
         if (__pyx_t_5) {
 
-          /* "TidalPy/RadialSolver/solver.pyx":1314
+          /* "TidalPy/RadialSolver/solver.pyx":1321
  *             layer_assumptions_ptr = NULL
  *         if not (upper_radius_by_layer_ptr is NULL):
  *             PyMem_Free(upper_radius_by_layer_ptr)             # <<<<<<<<<<<<<<
  *             upper_radius_by_layer_ptr = NULL
  * 
  */
           PyMem_Free(__pyx_v_upper_radius_by_layer_ptr);
 
-          /* "TidalPy/RadialSolver/solver.pyx":1315
+          /* "TidalPy/RadialSolver/solver.pyx":1322
  *         if not (upper_radius_by_layer_ptr is NULL):
  *             PyMem_Free(upper_radius_by_layer_ptr)
  *             upper_radius_by_layer_ptr = NULL             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
           __pyx_v_upper_radius_by_layer_ptr = NULL;
 
-          /* "TidalPy/RadialSolver/solver.pyx":1313
+          /* "TidalPy/RadialSolver/solver.pyx":1320
  *             PyMem_Free(layer_assumptions_ptr)
  *             layer_assumptions_ptr = NULL
  *         if not (upper_radius_by_layer_ptr is NULL):             # <<<<<<<<<<<<<<
  *             PyMem_Free(upper_radius_by_layer_ptr)
  *             upper_radius_by_layer_ptr = NULL
  */
         }
@@ -30197,18 +30245,18 @@
       __Pyx_XGIVEREF(__pyx_t_24);
       __Pyx_XGIVEREF(__pyx_t_25);
       __Pyx_ErrRestore(__pyx_t_23, __pyx_t_24, __pyx_t_25);
       __pyx_t_23 = 0; __pyx_t_24 = 0; __pyx_t_25 = 0; __pyx_t_26 = 0; __pyx_t_27 = 0; __pyx_t_28 = 0;
       __pyx_lineno = __pyx_t_10; __pyx_clineno = __pyx_t_21; __pyx_filename = __pyx_t_22;
       goto __pyx_L1_error;
     }
-    __pyx_L21:;
+    __pyx_L22:;
   }
 
-  /* "TidalPy/RadialSolver/solver.pyx":1317
+  /* "TidalPy/RadialSolver/solver.pyx":1324
  *             upper_radius_by_layer_ptr = NULL
  * 
  *     return result             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_result);
   __pyx_r = ((PyObject *)__pyx_v_result);
@@ -31705,28 +31753,29 @@
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
     {&__pyx_n_s_upper_radius_by_layer, __pyx_k_upper_radius_by_layer, sizeof(__pyx_k_upper_radius_by_layer), 0, 0, 1, 1},
     {&__pyx_n_s_upper_radius_by_layer_ptr, __pyx_k_upper_radius_by_layer_ptr, sizeof(__pyx_k_upper_radius_by_layer_ptr), 0, 0, 1, 1},
     {&__pyx_n_s_use_kamata, __pyx_k_use_kamata, sizeof(__pyx_k_use_kamata), 0, 0, 1, 1},
     {&__pyx_n_s_verbose, __pyx_k_verbose, sizeof(__pyx_k_verbose), 0, 0, 1, 1},
     {&__pyx_n_s_version_info, __pyx_k_version_info, sizeof(__pyx_k_version_info), 0, 0, 1, 1},
     {&__pyx_n_s_warning, __pyx_k_warning, sizeof(__pyx_k_warning), 0, 0, 1, 1},
+    {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 86, __pyx_L1_error)
   __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(0, 175, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 276, __pyx_L1_error)
   __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 328, __pyx_L1_error)
   __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 516, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 778, __pyx_L1_error)
-  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 1187, __pyx_L1_error)
+  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 1190, __pyx_L1_error)
   __pyx_builtin___import__ = __Pyx_GetBuiltinName(__pyx_n_s_import); if (!__pyx_builtin___import__) __PYX_ERR(1, 100, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 156, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 159, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 618, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 914, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 984, __pyx_L1_error)
@@ -31772,26 +31821,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "../../../../../tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 990, __pyx_L1_error)
@@ -31860,55 +31909,55 @@
  *                              'input arrays.')
  *         num_slices_by_layer_ptr[layer_i] = layer_slices
  */
   __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_u_At_least_three_layer_slices_per); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
 
-  /* "TidalPy/RadialSolver/solver.pyx":1198
+  /* "TidalPy/RadialSolver/solver.pyx":1201
  *     # Check that number of assumptions match.
  *     if len(is_static_by_layer) != num_layers:
  *         raise AttributeError('Number of `is_static_by_layer` must match number of `layer_types`.')             # <<<<<<<<<<<<<<
  *     if len(is_incompressible_by_layer) != num_layers:
  *         raise AttributeError('Number of `is_incompressible_by_layer` must match number of `layer_types`.')
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_u_Number_of_is_static_by_layer_mus); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 1198, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_u_Number_of_is_static_by_layer_mus); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 1201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
 
-  /* "TidalPy/RadialSolver/solver.pyx":1200
+  /* "TidalPy/RadialSolver/solver.pyx":1203
  *         raise AttributeError('Number of `is_static_by_layer` must match number of `layer_types`.')
  *     if len(is_incompressible_by_layer) != num_layers:
  *         raise AttributeError('Number of `is_incompressible_by_layer` must match number of `layer_types`.')             # <<<<<<<<<<<<<<
  *     if len(upper_radius_by_layer) != num_layers:
  *         raise AttributeError('Number of `upper_radius_by_layer` must match number of `layer_types`.')
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_u_Number_of_is_incompressible_by_l); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 1200, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_u_Number_of_is_incompressible_by_l); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 1203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
 
-  /* "TidalPy/RadialSolver/solver.pyx":1202
+  /* "TidalPy/RadialSolver/solver.pyx":1205
  *         raise AttributeError('Number of `is_incompressible_by_layer` must match number of `layer_types`.')
  *     if len(upper_radius_by_layer) != num_layers:
  *         raise AttributeError('Number of `upper_radius_by_layer` must match number of `layer_types`.')             # <<<<<<<<<<<<<<
  * 
  *     # Check that other inputs make sense
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_u_Number_of_upper_radius_by_layer); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 1202, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_u_Number_of_upper_radius_by_layer); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
 
-  /* "TidalPy/RadialSolver/solver.pyx":1207
+  /* "TidalPy/RadialSolver/solver.pyx":1210
  *     if solve_for is not None:
  *         if type(solve_for) != tuple:
  *             raise AttributeError(             # <<<<<<<<<<<<<<
  *                 '`solve_for` argument must be a tuple of strings. For example:\n'
  *                 '   ("tidal",)  # If you just want tidal Love numbers.\n'
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_u_solve_for_argument_must_be_a_tu); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 1207, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_u_solve_for_argument_must_be_a_tu); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 1210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "View.MemoryView":100
  * cdef object __pyx_collections_abc_Sequence "__pyx_collections_abc_Sequence"
  * try:
  *     if __import__("sys").version_info >= (3, 3):             # <<<<<<<<<<<<<<
@@ -32027,18 +32076,18 @@
   /* "TidalPy/RadialSolver/solver.pyx":1055
  * 
  * 
  * def radial_solver(             # <<<<<<<<<<<<<<
  *         double[::1] radius_array,
  *         double[::1] density_array,
  */
-  __pyx_tuple__44 = PyTuple_Pack(39, __pyx_n_s_radius_array, __pyx_n_s_density_array, __pyx_n_s_gravity_array, __pyx_n_s_bulk_modulus_array, __pyx_n_s_complex_shear_modulus_array, __pyx_n_s_frequency, __pyx_n_s_planet_bulk_density, __pyx_n_s_layer_types, __pyx_n_s_is_static_by_layer, __pyx_n_s_is_incompressible_by_layer, __pyx_n_s_upper_radius_by_layer, __pyx_n_s_degree_l, __pyx_n_s_solve_for, __pyx_n_s_use_kamata, __pyx_n_s_integration_method, __pyx_n_s_integration_rtol, __pyx_n_s_integration_atol, __pyx_n_s_scale_rtols_by_layer_type, __pyx_n_s_max_num_steps, __pyx_n_s_expected_size, __pyx_n_s_max_ram_MB, __pyx_n_s_max_step, __pyx_n_s_limit_solution_to_radius, __pyx_n_s_nondimensionalize, __pyx_n_s_verbose, __pyx_n_s_raise_on_fail, __pyx_n_s_i, __pyx_n_s_total_slices, __pyx_n_s_num_layers, __pyx_n_s_layer_assumptions_ptr, __pyx_n_s_layer_types_ptr, __pyx_n_s_is_static_by_layer_ptr, __pyx_n_s_is_incompressible_by_layer_ptr, __pyx_n_s_upper_radius_by_layer_ptr, __pyx_n_s_layer_type, __pyx_n_s_dynamic_liquid, __pyx_n_s_integration_method_lower, __pyx_n_s_integration_method_int, __pyx_n_s_result); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __pyx_tuple__44 = PyTuple_Pack(40, __pyx_n_s_radius_array, __pyx_n_s_density_array, __pyx_n_s_gravity_array, __pyx_n_s_bulk_modulus_array, __pyx_n_s_complex_shear_modulus_array, __pyx_n_s_frequency, __pyx_n_s_planet_bulk_density, __pyx_n_s_layer_types, __pyx_n_s_is_static_by_layer, __pyx_n_s_is_incompressible_by_layer, __pyx_n_s_upper_radius_by_layer, __pyx_n_s_degree_l, __pyx_n_s_solve_for, __pyx_n_s_use_kamata, __pyx_n_s_integration_method, __pyx_n_s_integration_rtol, __pyx_n_s_integration_atol, __pyx_n_s_scale_rtols_by_layer_type, __pyx_n_s_max_num_steps, __pyx_n_s_expected_size, __pyx_n_s_max_ram_MB, __pyx_n_s_max_step, __pyx_n_s_limit_solution_to_radius, __pyx_n_s_nondimensionalize, __pyx_n_s_verbose, __pyx_n_s_warnings, __pyx_n_s_raise_on_fail, __pyx_n_s_i, __pyx_n_s_total_slices, __pyx_n_s_num_layers, __pyx_n_s_layer_assumptions_ptr, __pyx_n_s_layer_types_ptr, __pyx_n_s_is_static_by_layer_ptr, __pyx_n_s_is_incompressible_by_layer_ptr, __pyx_n_s_upper_radius_by_layer_ptr, __pyx_n_s_layer_type, __pyx_n_s_dynamic_liquid, __pyx_n_s_integration_method_lower, __pyx_n_s_integration_method_int, __pyx_n_s_result); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__44);
   __Pyx_GIVEREF(__pyx_tuple__44);
-  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(26, 0, 0, 39, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_TidalPy_RadialSolver_solver_pyx, __pyx_n_s_radial_solver, 1055, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(27, 0, 0, 40, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_TidalPy_RadialSolver_solver_pyx, __pyx_n_s_radial_solver, 1055, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -32686,14 +32735,15 @@
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
+  PyObject *__pyx_t_21 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -33582,109 +33632,122 @@
   __Pyx_GOTREF(__pyx_t_16);
 
   /* "TidalPy/RadialSolver/solver.pyx":1079
  *         double max_step = 0,
  *         bint limit_solution_to_radius = True,
  *         bint nondimensionalize = True,             # <<<<<<<<<<<<<<
  *         bint verbose = False,
- *         bint raise_on_fail = False
+ *         bint warnings = True,
  */
   __pyx_t_17 = __Pyx_PyBool_FromLong(((int)1)); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 1079, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
 
   /* "TidalPy/RadialSolver/solver.pyx":1080
  *         bint limit_solution_to_radius = True,
  *         bint nondimensionalize = True,
  *         bint verbose = False,             # <<<<<<<<<<<<<<
+ *         bint warnings = True,
  *         bint raise_on_fail = False
- *         ):
  */
   __pyx_t_18 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1080, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
 
   /* "TidalPy/RadialSolver/solver.pyx":1081
  *         bint nondimensionalize = True,
  *         bint verbose = False,
+ *         bint warnings = True,             # <<<<<<<<<<<<<<
+ *         bint raise_on_fail = False
+ *         ):
+ */
+  __pyx_t_19 = __Pyx_PyBool_FromLong(((int)1)); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1081, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_19);
+
+  /* "TidalPy/RadialSolver/solver.pyx":1082
+ *         bint verbose = False,
+ *         bint warnings = True,
  *         bint raise_on_fail = False             # <<<<<<<<<<<<<<
  *         ):
  *     """
  */
-  __pyx_t_19 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1081, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_19);
+  __pyx_t_20 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 1082, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_20);
 
   /* "TidalPy/RadialSolver/solver.pyx":1055
  * 
  * 
  * def radial_solver(             # <<<<<<<<<<<<<<
  *         double[::1] radius_array,
  *         double[::1] density_array,
  */
-  __pyx_t_20 = PyTuple_New(15); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 1055, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_20);
+  __pyx_t_21 = PyTuple_New(16); if (unlikely(!__pyx_t_21)) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_21);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 0, __pyx_t_5)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 0, __pyx_t_5)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 1, Py_None)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 1, Py_None)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_7);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 2, __pyx_t_7)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 2, __pyx_t_7)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_INCREF(((PyObject*)__pyx_n_u_RK45));
   __Pyx_GIVEREF(((PyObject*)__pyx_n_u_RK45));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 3, ((PyObject*)__pyx_n_u_RK45))) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 3, ((PyObject*)__pyx_n_u_RK45))) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 4, __pyx_t_4)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 4, __pyx_t_4)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_10);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 5, __pyx_t_10)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 5, __pyx_t_10)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_11);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 6, __pyx_t_11)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 6, __pyx_t_11)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_12);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 7, __pyx_t_12)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 7, __pyx_t_12)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_13);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 8, __pyx_t_13)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 8, __pyx_t_13)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_14);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 9, __pyx_t_14)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 9, __pyx_t_14)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_15);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 10, __pyx_t_15)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 10, __pyx_t_15)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_16);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 11, __pyx_t_16)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 11, __pyx_t_16)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_17);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 12, __pyx_t_17)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 12, __pyx_t_17)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_18);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 13, __pyx_t_18)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 13, __pyx_t_18)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_19);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_20, 14, __pyx_t_19)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 14, __pyx_t_19)) __PYX_ERR(0, 1055, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_20);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_21, 15, __pyx_t_20)) __PYX_ERR(0, 1055, __pyx_L1_error);
   __pyx_t_5 = 0;
   __pyx_t_7 = 0;
   __pyx_t_4 = 0;
   __pyx_t_10 = 0;
   __pyx_t_11 = 0;
   __pyx_t_12 = 0;
   __pyx_t_13 = 0;
   __pyx_t_14 = 0;
   __pyx_t_15 = 0;
   __pyx_t_16 = 0;
   __pyx_t_17 = 0;
   __pyx_t_18 = 0;
   __pyx_t_19 = 0;
-  __pyx_t_19 = __Pyx_CyFunction_New(&__pyx_mdef_7TidalPy_12RadialSolver_6solver_1radial_solver, 0, __pyx_n_s_radial_solver, NULL, __pyx_n_s_TidalPy_RadialSolver_solver, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1055, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_19);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_19, __pyx_t_20);
+  __pyx_t_20 = 0;
+  __pyx_t_20 = __Pyx_CyFunction_New(&__pyx_mdef_7TidalPy_12RadialSolver_6solver_1radial_solver, 0, __pyx_n_s_radial_solver, NULL, __pyx_n_s_TidalPy_RadialSolver_solver, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_20);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_20, __pyx_t_21);
+  __Pyx_DECREF(__pyx_t_21); __pyx_t_21 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_radial_solver, __pyx_t_20) < 0) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_radial_solver, __pyx_t_19) < 0) __PYX_ERR(0, 1055, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
 
   /* "TidalPy/RadialSolver/solver.pyx":1
  * # distutils: language = c             # <<<<<<<<<<<<<<
  * # cython: boundscheck=False, wraparound=False, nonecheck=False, cdivision=True, initializedcheck=False
  * 
  */
-  __pyx_t_19 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_19);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_19) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+  __pyx_t_20 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_20);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_20) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
@@ -33696,14 +33759,15 @@
   __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
   __Pyx_XDECREF(__pyx_t_16);
   __Pyx_XDECREF(__pyx_t_17);
   __Pyx_XDECREF(__pyx_t_18);
   __Pyx_XDECREF(__pyx_t_19);
   __Pyx_XDECREF(__pyx_t_20);
+  __Pyx_XDECREF(__pyx_t_21);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init TidalPy.RadialSolver.solver", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #else
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/solver.pxd` & `tidalpy-0.5.4/TidalPy/RadialSolver/solver.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/solver.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/solver.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1074,14 +1074,15 @@
         size_t max_num_steps = 500_000,
         size_t expected_size = 500,
         size_t max_ram_MB = 500,
         double max_step = 0,
         bint limit_solution_to_radius = True,
         bint nondimensionalize = True,
         bint verbose = False,
+        bint warnings = True,
         bint raise_on_fail = False
         ):
     """
     Solves the viscoelastic-gravitational problem for a planet comprised of solid and liquid layers.
 
     See Takeuchi and Saito (1972) for more details on this method.
 
@@ -1159,14 +1160,16 @@
     limit_solution_to_radius : bool, default=True
         If True, then the solution will be limited to the points passed by the radius array.
     nondimensionalize : bool, default=True
         If Ture, then inputs will be non-dimensionalized before integration is performed.
         Results will be redimensionalized before being returned.
     verbose : bool, default=False
         If True, then additioal information will be printed to the terminal during the solution. 
+    warnings : bool, default=True
+        If True, then warnings will be printed to the terminal during the solution. 
     raise_on_fail : bool, default=False
         If Ture, then the solver will raise an exception if integration was not successful. By default RadialSolver
         fails silently. 
 
     Returns
     -------
     solution : RadialSolverSolution
@@ -1231,15 +1234,15 @@
     for i in range(num_layers):
         layer_type                        = layer_types[i]
         is_static_by_layer_ptr[i]         = is_static_by_layer[i]
         is_incompressible_by_layer_ptr[i] = is_incompressible_by_layer[i]
         upper_radius_by_layer_ptr[i]      = upper_radius_by_layer[i]
 
         if not dynamic_liquid:
-            if (layer_type != 1) and not is_static_by_layer_ptr[i]:
+            if (layer_type == 1) and not is_static_by_layer_ptr[i]:
                 # There is at least one dynamic liquid layer
                 dynamic_liquid = True
 
         # Convert user-provided strings to ints for the layer type
         if layer_type.lower() == 'solid':
             layer_types_ptr[i] = 0
         elif layer_type.lower() == 'liquid':
@@ -1251,15 +1254,19 @@
     
     # Check for dynamic liquid layer stability
     if dynamic_liquid and fabs(frequency) < 2.5e-5:
         # TODO: check that this frequency is a decent cutoff (based on a 3 day period).
         #    Initial work suggests that low density layers do not suffer from the same instability problems.
         # TODO: Add density or combo factor to better indicate when a solution is likely to be unstable?
         # See Issue #55
-        log.warning('Dynamic liquid layer detected in RadialSolver for a small frequency. Results may be unstable. Extra care is advised!')
+        if warnings:
+            log.warning(
+                'Dynamic liquid layer detected in RadialSolver for a small frequency.'
+                'Results may be unstable. Extra care is advised!'
+                )
     
     # Convert integration method to int
     cdef str integration_method_lower = integration_method.lower()
     cdef unsigned char integration_method_int
     if integration_method_lower == 'rk45':
         integration_method_int = 1
     elif integration_method_lower == 'rk23':
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/common.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/common.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/RadialSolver/starting",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.starting.common",
         "sources": [
             "TidalPy/RadialSolver/starting/common.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/common.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/common.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/driver.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/driver.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/RadialSolver/starting",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.starting.driver",
         "sources": [
             "TidalPy/RadialSolver/starting/driver.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/driver.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/driver.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/kamata.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/kamata.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/RadialSolver/starting",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.starting.kamata",
         "sources": [
             "TidalPy/RadialSolver/starting/kamata.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/kamata.pxd` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/kamata.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/kamata.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/kamata.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/saito.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/saito.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/RadialSolver/starting",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.starting.saito",
         "sources": [
             "TidalPy/RadialSolver/starting/saito.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/saito.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/saito.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/takeuchi.c` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/takeuchi.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/RadialSolver/starting",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.RadialSolver.starting.takeuchi",
         "sources": [
             "TidalPy/RadialSolver/starting/takeuchi.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/takeuchi.pxd` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/takeuchi.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/RadialSolver/starting/takeuchi.pyx` & `tidalpy-0.5.4/TidalPy/RadialSolver/starting/takeuchi.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/WorldPack/WorldPack.zip` & `tidalpy-0.5.4/TidalPy/WorldPack/WorldPack.zip`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/__init__.py` & `tidalpy-0.5.4/TidalPy/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/cache.py` & `tidalpy-0.5.4/TidalPy/cache.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/configurations.py` & `tidalpy-0.5.4/TidalPy/configurations.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/constants.py` & `tidalpy-0.5.4/TidalPy/constants.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/cooling/__init__.py` & `tidalpy-0.5.4/TidalPy/cooling/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/cooling/cooling.py` & `tidalpy-0.5.4/TidalPy/cooling/cooling.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/cooling/cooling_models.py` & `tidalpy-0.5.4/TidalPy/cooling/cooling_models.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/defaultc.py` & `tidalpy-0.5.4/TidalPy/defaultc.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/dynamics/dual_dissipation.py` & `tidalpy-0.5.4/TidalPy/dynamics/dual_dissipation.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/dynamics/single_dissipation.py` & `tidalpy-0.5.4/TidalPy/dynamics/single_dissipation.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/exceptions.py` & `tidalpy-0.5.4/TidalPy/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/initialize.py` & `tidalpy-0.5.4/TidalPy/initialize.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/logger.py` & `tidalpy-0.5.4/TidalPy/logger.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/numba_scipy/special/overloads.py` & `tidalpy-0.5.4/TidalPy/numba_scipy/special/overloads.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/numba_scipy/special/signatures.py` & `tidalpy-0.5.4/TidalPy/numba_scipy/special/signatures.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/orbit/averaging.py` & `tidalpy-0.5.4/TidalPy/orbit/averaging.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/output.py` & `tidalpy-0.5.4/TidalPy/output.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/paths.py` & `tidalpy-0.5.4/TidalPy/paths.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/love.py` & `tidalpy-0.5.4/TidalPy/radial_solver/love.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/matrix/fundamental_solid.py` & `tidalpy-0.5.4/TidalPy/radial_solver/matrix/fundamental_solid.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/matrix/propagate.py` & `tidalpy-0.5.4/TidalPy/radial_solver/matrix/propagate.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/nondimensional.py` & `tidalpy-0.5.4/TidalPy/radial_solver/nondimensional.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/collapse/generalized_collapse.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/collapse/generalized_collapse.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/collapse/surface_condition.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/collapse/surface_condition.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/__init__.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/odes.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/odes.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_dynamic.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_dynamic.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_dynamic_incomp.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_dynamic_incomp.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_static.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_static.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_static_incomp.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/derivatives/radial_derivatives_static_incomp.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/__init__.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/functions.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/functions.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/initial_solution_dynamic.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/initial_solution_dynamic.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/initial_solution_dynamic_incomp.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/initial_solution_dynamic_incomp.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/initial_solution_static.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/initial_solution_static.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/initial/initial_solution_static_incomp.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/initial/initial_solution_static_incomp.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/interfaces/__init__.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/interfaces/liquid_liquid.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/interfaces/liquid_liquid.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/interfaces/liquid_solid.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/interfaces/liquid_solid.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/interfaces/solid_liquid.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/interfaces/solid_liquid.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/interfaces/solid_solid.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/interfaces/solid_solid.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/numerical/solver.py` & `tidalpy-0.5.4/TidalPy/radial_solver/numerical/solver.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radial_solver/sensitivity.py` & `tidalpy-0.5.4/TidalPy/radial_solver/sensitivity.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radiogenics/radiogenic_models.py` & `tidalpy-0.5.4/TidalPy/radiogenics/radiogenic_models.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/radiogenics/radiogenics.py` & `tidalpy-0.5.4/TidalPy/radiogenics/radiogenics.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/base.c` & `tidalpy-0.5.4/TidalPy/rheology/base.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/rheology/base",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.rheology.base",
         "sources": [
             "TidalPy/rheology/base.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/rheology/base.pxd` & `tidalpy-0.5.4/TidalPy/rheology/base.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/base.pyx` & `tidalpy-0.5.4/TidalPy/rheology/base.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/complex_compliance/__init__.py` & `tidalpy-0.5.4/TidalPy/rheology/complex_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/complex_compliance/complex_compliance.py` & `tidalpy-0.5.4/TidalPy/rheology/complex_compliance/complex_compliance.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/complex_compliance/compliance_models.py` & `tidalpy-0.5.4/TidalPy/rheology/complex_compliance/compliance_models.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/models.c` & `tidalpy-0.5.4/TidalPy/rheology/models.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/rheology/models",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.rheology.models",
         "sources": [
             "TidalPy/rheology/models.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/rheology/models.pxd` & `tidalpy-0.5.4/TidalPy/rheology/models.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/models.pyx` & `tidalpy-0.5.4/TidalPy/rheology/models.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/partial_melt/__init__.py` & `tidalpy-0.5.4/TidalPy/rheology/partial_melt/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/partial_melt/melting_models.py` & `tidalpy-0.5.4/TidalPy/rheology/partial_melt/melting_models.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/partial_melt/partialmelt.py` & `tidalpy-0.5.4/TidalPy/rheology/partial_melt/partialmelt.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/rheology.py` & `tidalpy-0.5.4/TidalPy/rheology/rheology.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/viscosity/__init__.py` & `tidalpy-0.5.4/TidalPy/rheology/viscosity/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/viscosity/viscosity.py` & `tidalpy-0.5.4/TidalPy/rheology/viscosity/viscosity.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/rheology/viscosity/viscosity_models.py` & `tidalpy-0.5.4/TidalPy/rheology/viscosity/viscosity_models.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/stellar/__init__.py` & `tidalpy-0.5.4/TidalPy/stellar/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/stellar/insolation.py` & `tidalpy-0.5.4/TidalPy/stellar/insolation.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/stellar/stellar.py` & `tidalpy-0.5.4/TidalPy/stellar/stellar.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/helpers/orbit_config.py` & `tidalpy-0.5.4/TidalPy/structures/helpers/orbit_config.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/layers/basic.py` & `tidalpy-0.5.4/TidalPy/structures/layers/basic.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/layers/gas.py` & `tidalpy-0.5.4/TidalPy/structures/layers/gas.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/layers/helper.py` & `tidalpy-0.5.4/TidalPy/structures/layers/helper.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/layers/physics.py` & `tidalpy-0.5.4/TidalPy/structures/layers/physics.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/orbit/base.py` & `tidalpy-0.5.4/TidalPy/structures/orbit/base.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/orbit/physics.py` & `tidalpy-0.5.4/TidalPy/structures/orbit/physics.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/physical.py` & `tidalpy-0.5.4/TidalPy/structures/physical.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/world_builder/config_handler.py` & `tidalpy-0.5.4/TidalPy/structures/world_builder/config_handler.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/world_builder/iterative_builder.py` & `tidalpy-0.5.4/TidalPy/structures/world_builder/iterative_builder.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/world_builder/world_builder.py` & `tidalpy-0.5.4/TidalPy/structures/world_builder/world_builder.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/world_types/__init__.py` & `tidalpy-0.5.4/TidalPy/structures/world_types/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/world_types/basic.py` & `tidalpy-0.5.4/TidalPy/structures/world_types/basic.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/world_types/gas.py` & `tidalpy-0.5.4/TidalPy/structures/world_types/gas.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/world_types/layered.py` & `tidalpy-0.5.4/TidalPy/structures/world_types/layered.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/world_types/stellar.py` & `tidalpy-0.5.4/TidalPy/structures/world_types/stellar.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/structures/world_types/tidal.py` & `tidalpy-0.5.4/TidalPy/structures/world_types/tidal.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/__init__.py` & `tidalpy-0.5.4/TidalPy/tides/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/ctl_funcs/ctl_funcs.py` & `tidalpy-0.5.4/TidalPy/tides/ctl_funcs/ctl_funcs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/dissipation.py` & `tidalpy-0.5.4/TidalPy/tides/dissipation.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/__init__.py` & `tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl2.py` & `tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl2.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl3.py` & `tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl3.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl4.py` & `tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl4.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl5.py` & `tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl5.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl6.py` & `tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl6.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/eccentricity_funcs/orderl7.py` & `tidalpy-0.5.4/TidalPy/tides/eccentricity_funcs/orderl7.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/heating.py` & `tidalpy-0.5.4/TidalPy/tides/heating.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/inclination_funcs/__init__.py` & `tidalpy-0.5.4/TidalPy/tides/inclination_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl2.py` & `tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl2.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl3.py` & `tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl3.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl4.py` & `tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl4.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl5.py` & `tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl5.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl6.py` & `tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl6.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/inclination_funcs/orderl7.py` & `tidalpy-0.5.4/TidalPy/tides/inclination_funcs/orderl7.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/love1d.py` & `tidalpy-0.5.4/TidalPy/tides/love1d.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/methods/base.py` & `tidalpy-0.5.4/TidalPy/tides/methods/base.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/methods/global_approx.py` & `tidalpy-0.5.4/TidalPy/tides/methods/global_approx.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/methods/layered.py` & `tidalpy-0.5.4/TidalPy/tides/methods/layered.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/collapse_modes.py` & `tidalpy-0.5.4/TidalPy/tides/modes/collapse_modes.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/__init__.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl2.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl2.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl3.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl3.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl4.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl4.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl5.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl5.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl6.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl6.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl7.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/eccen_calc_orderl7.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl2.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl2.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl3.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl3.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl4.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl4.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl5.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl5.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl6.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl6.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl7.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_calc_helper/inclin_calc_orderl7.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/mode_manipulation.py` & `tidalpy-0.5.4/TidalPy/tides/modes/mode_manipulation.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/modes.py` & `tidalpy-0.5.4/TidalPy/tides/modes/modes.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/modes/multilayer_modes.py` & `tidalpy-0.5.4/TidalPy/tides/modes/multilayer_modes.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/multilayer/displacements.py` & `tidalpy-0.5.4/TidalPy/tides/multilayer/displacements.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/multilayer/heating.py` & `tidalpy-0.5.4/TidalPy/tides/multilayer/heating.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/multilayer/stress_strain.py` & `tidalpy-0.5.4/TidalPy/tides/multilayer/stress_strain.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/potential/__init__.py` & `tidalpy-0.5.4/TidalPy/tides/potential/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/potential/nsr_med_eccen_gen_obliquity.py` & `tidalpy-0.5.4/TidalPy/tides/potential/nsr_med_eccen_gen_obliquity.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/potential/nsr_med_eccen_med_obliquity.py` & `tidalpy-0.5.4/TidalPy/tides/potential/nsr_med_eccen_med_obliquity.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/potential/nsr_med_eccen_no_obliquity.py` & `tidalpy-0.5.4/TidalPy/tides/potential/nsr_med_eccen_no_obliquity.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/potential/nsr_modes_low_eccen_gen_obliquity.py` & `tidalpy-0.5.4/TidalPy/tides/potential/nsr_modes_low_eccen_gen_obliquity.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/potential/nsr_modes_med_eccen_gen_obliquity.py` & `tidalpy-0.5.4/TidalPy/tides/potential/nsr_modes_med_eccen_gen_obliquity.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/potential/nsr_modes_med_eccen_med_obliquity.py` & `tidalpy-0.5.4/TidalPy/tides/potential/nsr_modes_med_eccen_med_obliquity.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/potential/nsr_modes_med_eccen_no_obliquity.py` & `tidalpy-0.5.4/TidalPy/tides/potential/nsr_modes_med_eccen_no_obliquity.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/potential/synchronous_low_e.py` & `tidalpy-0.5.4/TidalPy/tides/potential/synchronous_low_e.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/tides/universal_coeffs.py` & `tidalpy-0.5.4/TidalPy/tides/universal_coeffs.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/toolbox/quick_tides.py` & `tidalpy-0.5.4/TidalPy/toolbox/quick_tides.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/classes/base_x.c` & `tidalpy-0.5.4/TidalPy/utilities/classes/base_x.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/utilities/classes",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.utilities.classes.base_x",
         "sources": [
             "TidalPy/utilities/classes/base_x.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/utilities/classes/base_x.pyx` & `tidalpy-0.5.4/TidalPy/utilities/classes/base_x.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/classes/config/config.py` & `tidalpy-0.5.4/TidalPy/utilities/classes/config/config.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/classes/model/functional_utils.py` & `tidalpy-0.5.4/TidalPy/utilities/classes/model/functional_utils.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/classes/model/model.py` & `tidalpy-0.5.4/TidalPy/utilities/classes/model/model.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/classes/model/model_utils.py` & `tidalpy-0.5.4/TidalPy/utilities/classes/model/model_utils.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/constants_x.c` & `tidalpy-0.5.4/TidalPy/utilities/constants_x.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/utilities",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.utilities.constants_x",
         "sources": [
             "TidalPy/utilities/constants_x.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/utilities/constants_x.pyx` & `tidalpy-0.5.4/TidalPy/utilities/constants_x.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/conversions/conversions.py` & `tidalpy-0.5.4/TidalPy/utilities/conversions/conversions.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/conversions/conversions_x.c` & `tidalpy-0.5.4/TidalPy/utilities/conversions/conversions_x.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/utilities/conversions",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.utilities.conversions.conversions_x",
         "sources": [
             "TidalPy/utilities/conversions/conversions_x.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/utilities/conversions/conversions_x.pxd` & `tidalpy-0.5.4/TidalPy/utilities/conversions/conversions_x.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/conversions/conversions_x.pyx` & `tidalpy-0.5.4/TidalPy/utilities/conversions/conversions_x.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/conversions/timing.py` & `tidalpy-0.5.4/TidalPy/utilities/conversions/timing.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/dictionary_utils.py` & `tidalpy-0.5.4/TidalPy/utilities/dictionary_utils.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/dimensions/nondimensional.c` & `tidalpy-0.5.4/TidalPy/utilities/dimensions/nondimensional.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/utilities/dimensions",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "TidalPy.utilities.dimensions.nondimensional",
         "sources": [
             "TidalPy/utilities/dimensions/nondimensional.pyx"
         ]
     },
     "module_name": "TidalPy.utilities.dimensions.nondimensional"
```

### Comparing `tidalpy-0.5.3/TidalPy/utilities/dimensions/nondimensional.pxd` & `tidalpy-0.5.4/TidalPy/utilities/dimensions/nondimensional.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/dimensions/nondimensional.pyx` & `tidalpy-0.5.4/TidalPy/utilities/dimensions/nondimensional.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/exoplanets/data_download.py` & `tidalpy-0.5.4/TidalPy/utilities/exoplanets/data_download.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/graphics/global_map.py` & `tidalpy-0.5.4/TidalPy/utilities/graphics/global_map.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/graphics/grid_plot.py` & `tidalpy-0.5.4/TidalPy/utilities/graphics/grid_plot.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/graphics/multilayer/RN08-Data.csv` & `tidalpy-0.5.4/TidalPy/utilities/graphics/multilayer/RN08-Data.csv`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/graphics/multilayer/T05-Data.csv` & `tidalpy-0.5.4/TidalPy/utilities/graphics/multilayer/T05-Data.csv`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/graphics/multilayer/yplot.py` & `tidalpy-0.5.4/TidalPy/utilities/graphics/multilayer/yplot.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/graphics/phasespace_plot.py` & `tidalpy-0.5.4/TidalPy/utilities/graphics/phasespace_plot.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/graphics/planet_plot.py` & `tidalpy-0.5.4/TidalPy/utilities/graphics/planet_plot.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/integration/__init__.py` & `tidalpy-0.5.4/TidalPy/utilities/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/integration/cyrk_helper.py` & `tidalpy-0.5.4/TidalPy/utilities/integration/cyrk_helper.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/integration/julia_helper.py` & `tidalpy-0.5.4/TidalPy/utilities/integration/julia_helper.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/integration/numbalsoda_helper.py` & `tidalpy-0.5.4/TidalPy/utilities/integration/numbalsoda_helper.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/integration/scipy_helper.py` & `tidalpy-0.5.4/TidalPy/utilities/integration/scipy_helper.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/io/pathing.py` & `tidalpy-0.5.4/TidalPy/utilities/io/pathing.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/io/progress.py` & `tidalpy-0.5.4/TidalPy/utilities/io/progress.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/math/complex.c` & `tidalpy-0.5.4/TidalPy/utilities/math/complex.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/utilities/math",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c",
         "name": "TidalPy.utilities.math.complex",
         "sources": [
             "TidalPy/utilities/math/complex.pyx"
         ]
     },
```

### Comparing `tidalpy-0.5.3/TidalPy/utilities/math/complex.pxd` & `tidalpy-0.5.4/TidalPy/utilities/math/complex.pxd`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/math/complex.pyx` & `tidalpy-0.5.4/TidalPy/utilities/math/complex.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/math/special.py` & `tidalpy-0.5.4/TidalPy/utilities/math/special.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/math/special_x.c` & `tidalpy-0.5.4/TidalPy/utilities/math/special_x.c`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/utilities/math",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "TidalPy.utilities.math.special_x",
         "sources": [
             "TidalPy/utilities/math/special_x.pyx"
         ]
     },
     "module_name": "TidalPy.utilities.math.special_x"
```

### Comparing `tidalpy-0.5.3/TidalPy/utilities/math/special_x.pyx` & `tidalpy-0.5.4/TidalPy/utilities/math/special_x.pyx`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/multiprocessing/__init__.py` & `tidalpy-0.5.4/TidalPy/utilities/multiprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/multiprocessing/multiprocessing.py` & `tidalpy-0.5.4/TidalPy/utilities/multiprocessing/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/numpy_helper/array_other.py` & `tidalpy-0.5.4/TidalPy/utilities/numpy_helper/array_other.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/numpy_helper/array_shape.py` & `tidalpy-0.5.4/TidalPy/utilities/numpy_helper/array_shape.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/performance/memory.py` & `tidalpy-0.5.4/TidalPy/utilities/performance/memory.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/performance/numba.py` & `tidalpy-0.5.4/TidalPy/utilities/performance/numba.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/performance/special/factorial.py` & `tidalpy-0.5.4/TidalPy/utilities/performance/special/factorial.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/spherical_helper/mass.py` & `tidalpy-0.5.4/TidalPy/utilities/spherical_helper/mass.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/spherical_helper/volume.py` & `tidalpy-0.5.4/TidalPy/utilities/spherical_helper/volume.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/string_helper/string_helper.py` & `tidalpy-0.5.4/TidalPy/utilities/string_helper/string_helper.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/types.py` & `tidalpy-0.5.4/TidalPy/utilities/types.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/TidalPy/utilities/types_x.c` & `tidalpy-0.5.4/TidalPy/utilities/types_x.c`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         ],
         "extra_link_args": [
             "-fopenmp",
             "-O3"
         ],
         "include_dirs": [
             "TidalPy/utilities",
-            "/tmp/build-env-a4pe7e8f/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-grxfilx9/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "TidalPy.utilities.types_x",
         "sources": [
             "TidalPy/utilities/types_x.pyx"
         ]
     },
     "module_name": "TidalPy.utilities.types_x"
```

### Comparing `tidalpy-0.5.3/TidalPy.egg-info/PKG-INFO` & `tidalpy-0.5.4/TidalPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TidalPy
-Version: 0.5.3
+Version: 0.5.4
 Summary: Tidal Dynamics and Thermal-Orbital Evolution Software Suite Implemented in Cython and Python
 Author-email: "Joe P. Renaud" <TidalPy@gmail.com>
 License: # License
         
         ## Creative Commons Attribution-ShareAlike 4.0 International
         Creative Commons Corporation (“Creative Commons”) is not a law firm and does not provide legal services or legal advice. Distribution of Creative Commons public licenses does not create a lawyer-client or other relationship. Creative Commons makes its licenses and related information available on an “as-is” basis. Creative Commons gives no warranties regarding its licenses, any material licensed under their terms and conditions, or any related information. Creative Commons disclaims all liability for damages resulting from their use to the fullest extent possible.
         
@@ -244,15 +244,15 @@
     <!--<a href="https://codecov.io/github/jrenaud90/TidalPy" ><img src="https://codecov.io/github/jrenaud90/TidalPy/branch/main/graph/badge.svg?token=35OY4ZLOA5"/></a><br />-->
     <a href="https://doi.org/10.5281/zenodo.7017475"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7017475.svg" alt="DOI"></a>
     <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/Python-3.9|3.10|3.11|3.12-blue" alt="Python Version 3.9-3.12" /></a>
 </div>
 
 ---
 
-<a href="https://github.com/jrenaud90/TidalPy/releases"><img src="https://img.shields.io/badge/TidalPy-0.5.3 Alpha-orange" alt="TidalPy Version 0.5.3 Alpha" /></a>
+<a href="https://github.com/jrenaud90/TidalPy/releases"><img src="https://img.shields.io/badge/TidalPy-0.5.4 Alpha-orange" alt="TidalPy Version 0.5.4 Alpha" /></a>
 
 **Tidal Dynamics and Thermal-Orbital Evolution Software Suite Implemented in Cython and Python**
 
 TidalPy is an open-source software suite that utilizes a semi-analytic approach to estimate tidal heating,
 orbit-rotation evolution, and thermal changes for rocky and icy worlds. It has been used to simulate the thermal-orbital
 evolution of moons within our Solar System as well as exoplanets beyond. TidalPy's `RadialSolver` package can accurately
 estimate the viscoelastic Love and Shida numbers for a multi-layered world, including the effects of liquid layers,
```

### Comparing `tidalpy-0.5.3/TidalPy.egg-info/SOURCES.txt` & `tidalpy-0.5.4/TidalPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/_build_tidalpy.py` & `tidalpy-0.5.4/_build_tidalpy.py`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/cython_extensions.json` & `tidalpy-0.5.4/cython_extensions.json`

 * *Files identical despite different names*

### Comparing `tidalpy-0.5.3/pyproject.toml` & `tidalpy-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name='TidalPy'
-version = '0.5.3'
+version = '0.5.4'
 description='Tidal Dynamics and Thermal-Orbital Evolution Software Suite Implemented in Cython and Python'
 authors= [ 
     {name = 'Joe P. Renaud', email = 'TidalPy@gmail.com'}
     ]
 requires-python = ">=3.9,<3.13"
 dependencies = [
     # Scientific and computing resources
```

### Comparing `tidalpy-0.5.3/setup.py` & `tidalpy-0.5.4/setup.py`

 * *Files identical despite different names*

